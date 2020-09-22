# `ros:dashing-ros1-bridge`

## Docker Metadata

- Image ID: `sha256:c60a3d1963d419b15a9f23da630d35553668b728eadfb2f0da58fac7b5029b2d`
- Created: `2020-09-17T01:51:04.775846703Z`
- Virtual Size: ~ 1.36 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/ros_entrypoint.sh"]`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `LC_ALL=C.UTF-8`
  - `ROS_DISTRO=dashing`
  - `ROS1_DISTRO=melodic`
  - `ROS2_DISTRO=dashing`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3build1`

Binary Packages:

- `libacl1:amd64=2.2.52-3build1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3build1.dsc' acl_2.2.52-3build1.dsc 2031 SHA256:864215f3e68d6b169a044bd952e78be9b0b1cf527a2cbf25866cab919e78e64b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3build1.debian.tar.xz' acl_2.2.52-3build1.debian.tar.xz 8788 SHA256:0729d8c850aa26bc9f1b22ce632efb1616a3f97dc5fca1d9edfda45b582b7f37
```

### `dpkg` source package: `adduser=3.116ubuntu1`

Binary Packages:

- `adduser=3.116ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.116ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.116ubuntu1.dsc' adduser_3.116ubuntu1.dsc 1845 SHA256:fc44097093d74fc2e36fc37dceb54cf6bcb70a434240b14fd91beb64849cf2fd
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.116ubuntu1.tar.xz' adduser_3.116ubuntu1.tar.xz 216868 SHA256:f34f1d95e96ecae3b068a3dd666848f82f06cbb26152c56a6b72bd71555a8f18
```

### `dpkg` source package: `apr-util=1.6.1-2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-2`
- `libaprutil1-dev=1.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`, `/usr/share/doc/libaprutil1-dev/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-2.dsc' apr-util_1.6.1-2.dsc 2851 SHA256:7a3a7d0dccc0d89ad751988163cb57d34b32094893d08c4d0ac79e9bfee6d8f4
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2.asc' apr-util_1.6.1.orig.tar.bz2.asc 801 SHA256:47837b605290c0d7659b73734e4a9d5e6c0c24c13185cd4d91837afe63c07ca4
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-2.debian.tar.xz' apr-util_1.6.1-2.debian.tar.xz 211832 SHA256:e30e919e7e049a8a7056b7184e77d69b82660d71a4bf9654d1c9bfccf2fcde30
```

### `dpkg` source package: `apr=1.6.3-2`

Binary Packages:

- `libapr1:amd64=1.6.3-2`
- `libapr1-dev=1.6.3-2`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`, `/usr/share/doc/libapr1-dev/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.3-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3-2.dsc' apr_1.6.3-2.dsc 2305 SHA256:0597703f9ea3bc3b30fcd7e055c67c2113e5c4255df5ff42738ce6a396bf5afc
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3.orig.tar.bz2' apr_1.6.3.orig.tar.bz2 854100 SHA256:131f06d16d7aabd097fa992a33eec2b6af3962f93e6d570a9bd4d85e95993172
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3.orig.tar.bz2.asc' apr_1.6.3.orig.tar.bz2.asc 801 SHA256:33db39162f7ca9acdccaa4f19630a67045542791b262116d3512c8b5d7c3fca1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3-2.debian.tar.xz' apr_1.6.3-2.debian.tar.xz 213068 SHA256:ac515f888f7157586631e3de9792ee01d239f9cbf1e768be31ee6daac61f2597
```

### `dpkg` source package: `apt=1.6.12ubuntu0.1`

Binary Packages:

- `apt=1.6.12ubuntu0.1`
- `libapt-pkg5.0:amd64=1.6.12ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.6.12ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.dsc' apt_1.6.12ubuntu0.1.dsc 2561 SHA256:4f14aab7fb35be3b4de7b9c73074a632f956ea284c460b1d2453bb03af8e04ab
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.tar.xz' apt_1.6.12ubuntu0.1.tar.xz 2172208 SHA256:207daf6cdc6488b65e2b5bffbb721670ee7034507f3d9b460e36fff5668d0360
```

### `dpkg` source package: `asn1crypto=0.24.0-1`

Binary Packages:

- `python-asn1crypto=0.24.0-1`

Licenses: (parsed from: `/usr/share/doc/python-asn1crypto/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris asn1crypto=0.24.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/asn1crypto/asn1crypto_0.24.0-1.dsc' asn1crypto_0.24.0-1.dsc 1960 SHA256:71bef30ecadbb81ed4a656230892c1d7d4fde3dd74eaa546c94ae93c43591045
'http://archive.ubuntu.com/ubuntu/pool/main/a/asn1crypto/asn1crypto_0.24.0.orig.tar.gz' asn1crypto_0.24.0.orig.tar.gz 104964 SHA256:9d5c20441baf0cb60a4ac34cc447c6c189024b6b4c6cd7877034f4965c464e49
'http://archive.ubuntu.com/ubuntu/pool/main/a/asn1crypto/asn1crypto_0.24.0-1.debian.tar.xz' asn1crypto_0.24.0-1.debian.tar.xz 2288 SHA256:72a5e503943aa519acbd51971b83e51345aa53270f93d4e1313e1e7f7a05ab29
```

### `dpkg` source package: `attr=1:2.4.47-2build1`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2build1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2build1.dsc' attr_2.4.47-2build1.dsc 2033 SHA256:b78dbf07b789010caabc12c1ab0b2a944072058fe47ac6b5d345209c16f4e1f5
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2build1.debian.tar.xz' attr_2.4.47-2build1.debian.tar.xz 8168 SHA256:6732a8874190a1f792c7f9cb95fadc1dc852baf2e164b0d7b4bcea525f5c0882
```

### `dpkg` source package: `audit=1:2.8.2-1ubuntu1`

Binary Packages:

- `libaudit-common=1:2.8.2-1ubuntu1`
- `libaudit1:amd64=1:2.8.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2-1ubuntu1.dsc' audit_2.8.2-1ubuntu1.dsc 2903 SHA256:454c231dc2268ee4862f87d65720354699be9b807a411556a536bc2b4e581a90
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2.orig.tar.gz' audit_2.8.2.orig.tar.gz 1121970 SHA256:67b59b2b77afee9ed87afa4d80ffc8e6f3a1f4bbedd5f2871f387c952147bcba
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2-1ubuntu1.debian.tar.xz' audit_2.8.2-1ubuntu1.debian.tar.xz 21344 SHA256:2bc93230e3bf01eef5e9a5acff8f904af074e6e39003f1db8941118fbd041ec2
```

### `dpkg` source package: `base-files=10.1ubuntu2.10`

Binary Packages:

- `base-files=10.1ubuntu2.10`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=10.1ubuntu2.10
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_10.1ubuntu2.10.dsc' base-files_10.1ubuntu2.10.dsc 1688 SHA256:f6d4715c4dbe63584bcc6cd1852cda4d84081990eb02354445cb03f57e566793
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_10.1ubuntu2.10.tar.xz' base-files_10.1ubuntu2.10.tar.xz 79780 SHA256:b1735b09b972f818eadb2bc99b3f974b49561341a53abea476afe2a6da87273e
```

### `dpkg` source package: `base-passwd=3.5.44`

Binary Packages:

- `base-passwd=3.5.44`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.44
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.44.dsc' base-passwd_3.5.44.dsc 1685 SHA256:22a5db1e9bb71fa8a4d682b3f9c01470a61b8041eb6212471181c6808b268c13
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.44.tar.xz' base-passwd_3.5.44.tar.xz 52644 SHA256:f17a0746024572e86e60e4614cf226a81ffe682ceaf1a1fce9dc1a8002683e90
```

### `dpkg` source package: `bash=4.4.18-2ubuntu1.2`

Binary Packages:

- `bash=4.4.18-2ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.4.18-2ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.dsc' bash_4.4.18-2ubuntu1.2.dsc 2434 SHA256:febc739ab69e09853f8f1d4b1db7038937911bee7d715926f1e7ff461b63c82f
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18.orig.tar.xz' bash_4.4.18.orig.tar.xz 5036272 SHA256:704143a7170041ac9f1025455d6d23ff0f353711a3dc557b47d6e6322f24cd02
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.debian.tar.xz' bash_4.4.18-2ubuntu1.2.debian.tar.xz 65236 SHA256:b0191aab30dd0531d7acbeab7c64014a1c9e484f417678a18ad1655a77b7b6f9
```

### `dpkg` source package: `binutils=2.30-21ubuntu1~18.04.4`

Binary Packages:

- `binutils=2.30-21ubuntu1~18.04.4`
- `binutils-common:amd64=2.30-21ubuntu1~18.04.4`
- `binutils-x86-64-linux-gnu=2.30-21ubuntu1~18.04.4`
- `libbinutils:amd64=2.30-21ubuntu1~18.04.4`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.30-21ubuntu1~18.04.4
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.30-21ubuntu1~18.04.4.dsc' binutils_2.30-21ubuntu1~18.04.4.dsc 11670 SHA256:38a196915f030c1656aa4f9d022bcce4a8951b5fcc3bf10971dae20346697f3a
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.30.orig.tar.xz' binutils_2.30.orig.tar.xz 20286700 SHA256:6e46b8aeae2f727a36f0bd9505e405768a72218f1796f0d09757d45209871ae6
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.30-21ubuntu1~18.04.4.debian.tar.xz' binutils_2.30-21ubuntu1~18.04.4.debian.tar.xz 622680 SHA256:2a8e35eb1446d870c09792d06d4c9b65d8bc717eea2b86fa982c101a278a2f33
```

### `dpkg` source package: `boost-defaults=1.65.1.0ubuntu1`

Binary Packages:

- `libboost-all-dev=1.65.1.0ubuntu1`
- `libboost-atomic-dev:amd64=1.65.1.0ubuntu1`
- `libboost-chrono-dev:amd64=1.65.1.0ubuntu1`
- `libboost-container-dev:amd64=1.65.1.0ubuntu1`
- `libboost-context-dev:amd64=1.65.1.0ubuntu1`
- `libboost-coroutine-dev:amd64=1.65.1.0ubuntu1`
- `libboost-date-time-dev:amd64=1.65.1.0ubuntu1`
- `libboost-dev:amd64=1.65.1.0ubuntu1`
- `libboost-exception-dev:amd64=1.65.1.0ubuntu1`
- `libboost-fiber-dev:amd64=1.65.1.0ubuntu1`
- `libboost-filesystem-dev:amd64=1.65.1.0ubuntu1`
- `libboost-graph-dev:amd64=1.65.1.0ubuntu1`
- `libboost-graph-parallel-dev=1.65.1.0ubuntu1`
- `libboost-iostreams-dev:amd64=1.65.1.0ubuntu1`
- `libboost-locale-dev:amd64=1.65.1.0ubuntu1`
- `libboost-log-dev=1.65.1.0ubuntu1`
- `libboost-math-dev:amd64=1.65.1.0ubuntu1`
- `libboost-mpi-dev=1.65.1.0ubuntu1`
- `libboost-mpi-python-dev=1.65.1.0ubuntu1`
- `libboost-numpy-dev=1.65.1.0ubuntu1`
- `libboost-program-options-dev:amd64=1.65.1.0ubuntu1`
- `libboost-python-dev=1.65.1.0ubuntu1`
- `libboost-random-dev:amd64=1.65.1.0ubuntu1`
- `libboost-regex-dev:amd64=1.65.1.0ubuntu1`
- `libboost-serialization-dev:amd64=1.65.1.0ubuntu1`
- `libboost-signals-dev:amd64=1.65.1.0ubuntu1`
- `libboost-stacktrace-dev:amd64=1.65.1.0ubuntu1`
- `libboost-system-dev:amd64=1.65.1.0ubuntu1`
- `libboost-test-dev:amd64=1.65.1.0ubuntu1`
- `libboost-thread-dev:amd64=1.65.1.0ubuntu1`
- `libboost-timer-dev:amd64=1.65.1.0ubuntu1`
- `libboost-tools-dev=1.65.1.0ubuntu1`
- `libboost-type-erasure-dev:amd64=1.65.1.0ubuntu1`
- `libboost-wave-dev:amd64=1.65.1.0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris boost-defaults=1.65.1.0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost-defaults/boost-defaults_1.65.1.0ubuntu1.dsc' boost-defaults_1.65.1.0ubuntu1.dsc 4037 SHA256:0e1e6bde4468c802a8cb0795e15a3deb56ef29288f051f539a18a0b1b24edd6c
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost-defaults/boost-defaults_1.65.1.0ubuntu1.tar.gz' boost-defaults_1.65.1.0ubuntu1.tar.gz 12172 SHA256:2554c6a67a4b6939d2090d37445cc0fc366c1448c4080f62ebe2ca189d691a7a
```

### `dpkg` source package: `boost1.65.1=1.65.1+dfsg-0ubuntu5`

Binary Packages:

- `libboost-atomic1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-atomic1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-chrono1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-chrono1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-container1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-container1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-context1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-context1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-coroutine1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-coroutine1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-date-time1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-date-time1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-exception1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-fiber1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-fiber1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-filesystem1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-filesystem1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-graph-parallel1.65-dev=1.65.1+dfsg-0ubuntu5`
- `libboost-graph-parallel1.65.1=1.65.1+dfsg-0ubuntu5`
- `libboost-graph1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-graph1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-iostreams1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-iostreams1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-locale1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-locale1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-log1.65-dev=1.65.1+dfsg-0ubuntu5`
- `libboost-log1.65.1=1.65.1+dfsg-0ubuntu5`
- `libboost-math1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-math1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-mpi-python1.65-dev=1.65.1+dfsg-0ubuntu5`
- `libboost-mpi-python1.65.1=1.65.1+dfsg-0ubuntu5`
- `libboost-mpi1.65-dev=1.65.1+dfsg-0ubuntu5`
- `libboost-mpi1.65.1=1.65.1+dfsg-0ubuntu5`
- `libboost-numpy1.65-dev=1.65.1+dfsg-0ubuntu5`
- `libboost-numpy1.65.1=1.65.1+dfsg-0ubuntu5`
- `libboost-program-options1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-program-options1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-python1.65-dev=1.65.1+dfsg-0ubuntu5`
- `libboost-python1.65.1=1.65.1+dfsg-0ubuntu5`
- `libboost-random1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-random1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-regex1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-regex1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-serialization1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-serialization1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-signals1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-signals1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-stacktrace1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-stacktrace1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-system1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-system1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-test1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-test1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-thread1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-thread1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-timer1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-timer1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-type-erasure1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-type-erasure1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-wave1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-wave1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost1.65-dev:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost1.65-tools-dev=1.65.1+dfsg-0ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libboost-atomic1.65-dev/copyright`, `/usr/share/doc/libboost-atomic1.65.1/copyright`, `/usr/share/doc/libboost-chrono1.65-dev/copyright`, `/usr/share/doc/libboost-chrono1.65.1/copyright`, `/usr/share/doc/libboost-container1.65-dev/copyright`, `/usr/share/doc/libboost-container1.65.1/copyright`, `/usr/share/doc/libboost-context1.65-dev/copyright`, `/usr/share/doc/libboost-context1.65.1/copyright`, `/usr/share/doc/libboost-coroutine1.65-dev/copyright`, `/usr/share/doc/libboost-coroutine1.65.1/copyright`, `/usr/share/doc/libboost-date-time1.65-dev/copyright`, `/usr/share/doc/libboost-date-time1.65.1/copyright`, `/usr/share/doc/libboost-exception1.65-dev/copyright`, `/usr/share/doc/libboost-fiber1.65-dev/copyright`, `/usr/share/doc/libboost-fiber1.65.1/copyright`, `/usr/share/doc/libboost-filesystem1.65-dev/copyright`, `/usr/share/doc/libboost-filesystem1.65.1/copyright`, `/usr/share/doc/libboost-graph-parallel1.65-dev/copyright`, `/usr/share/doc/libboost-graph-parallel1.65.1/copyright`, `/usr/share/doc/libboost-graph1.65-dev/copyright`, `/usr/share/doc/libboost-graph1.65.1/copyright`, `/usr/share/doc/libboost-iostreams1.65-dev/copyright`, `/usr/share/doc/libboost-iostreams1.65.1/copyright`, `/usr/share/doc/libboost-locale1.65-dev/copyright`, `/usr/share/doc/libboost-locale1.65.1/copyright`, `/usr/share/doc/libboost-log1.65-dev/copyright`, `/usr/share/doc/libboost-log1.65.1/copyright`, `/usr/share/doc/libboost-math1.65-dev/copyright`, `/usr/share/doc/libboost-math1.65.1/copyright`, `/usr/share/doc/libboost-mpi-python1.65-dev/copyright`, `/usr/share/doc/libboost-mpi-python1.65.1/copyright`, `/usr/share/doc/libboost-mpi1.65-dev/copyright`, `/usr/share/doc/libboost-mpi1.65.1/copyright`, `/usr/share/doc/libboost-numpy1.65-dev/copyright`, `/usr/share/doc/libboost-numpy1.65.1/copyright`, `/usr/share/doc/libboost-program-options1.65-dev/copyright`, `/usr/share/doc/libboost-program-options1.65.1/copyright`, `/usr/share/doc/libboost-python1.65-dev/copyright`, `/usr/share/doc/libboost-python1.65.1/copyright`, `/usr/share/doc/libboost-random1.65-dev/copyright`, `/usr/share/doc/libboost-random1.65.1/copyright`, `/usr/share/doc/libboost-regex1.65-dev/copyright`, `/usr/share/doc/libboost-regex1.65.1/copyright`, `/usr/share/doc/libboost-serialization1.65-dev/copyright`, `/usr/share/doc/libboost-serialization1.65.1/copyright`, `/usr/share/doc/libboost-signals1.65-dev/copyright`, `/usr/share/doc/libboost-signals1.65.1/copyright`, `/usr/share/doc/libboost-stacktrace1.65-dev/copyright`, `/usr/share/doc/libboost-stacktrace1.65.1/copyright`, `/usr/share/doc/libboost-system1.65-dev/copyright`, `/usr/share/doc/libboost-system1.65.1/copyright`, `/usr/share/doc/libboost-test1.65-dev/copyright`, `/usr/share/doc/libboost-test1.65.1/copyright`, `/usr/share/doc/libboost-thread1.65-dev/copyright`, `/usr/share/doc/libboost-thread1.65.1/copyright`, `/usr/share/doc/libboost-timer1.65-dev/copyright`, `/usr/share/doc/libboost-timer1.65.1/copyright`, `/usr/share/doc/libboost-type-erasure1.65-dev/copyright`, `/usr/share/doc/libboost-type-erasure1.65.1/copyright`, `/usr/share/doc/libboost-wave1.65-dev/copyright`, `/usr/share/doc/libboost-wave1.65.1/copyright`, `/usr/share/doc/libboost1.65-dev/copyright`, `/usr/share/doc/libboost1.65-tools-dev/copyright`)

- `Boost`
- `bjam`
- `boostbook`

Source:

```console
$ apt-get source -qq --print-uris boost1.65.1=1.65.1+dfsg-0ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.65.1/boost1.65.1_1.65.1+dfsg-0ubuntu5.dsc' boost1.65.1_1.65.1+dfsg-0ubuntu5.dsc 7825 SHA256:e046822facd57a5810416328f6e440f5ae5a4017215d1ea3ca7bec59e090c598
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.65.1/boost1.65.1_1.65.1+dfsg.orig.tar.bz2' boost1.65.1_1.65.1+dfsg.orig.tar.bz2 82120283 SHA256:c7709bf6b416e0609fac4bcc0c0093a890ccbeaeebbeabe45877cffc5d06f43c
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.65.1/boost1.65.1_1.65.1+dfsg-0ubuntu5.debian.tar.xz' boost1.65.1_1.65.1+dfsg-0ubuntu5.debian.tar.xz 105524 SHA256:c238e8a63c232911402cef6f8ea7763bddf572f7062b5353147ee9ed9a79afdb
```

### `dpkg` source package: `build-essential=12.4ubuntu1`

Binary Packages:

- `build-essential=12.4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/build-essential/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris build-essential=12.4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.4ubuntu1.dsc' build-essential_12.4ubuntu1.dsc 2032 SHA256:93ee6ef55a672f52722fbc37d1ec3172e685226ee7f44f028db43bea0791c30e
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.4ubuntu1.tar.gz' build-essential_12.4ubuntu1.tar.gz 64966 SHA256:890a4bb7b72ffa4fa152d6bb0a9cca8835b9e9c0f4e110c487a22de9903dce0a
```

### `dpkg` source package: `bzip2=1.0.6-8.1ubuntu0.2`

Binary Packages:

- `bzip2=1.0.6-8.1ubuntu0.2`
- `libbz2-1.0:amd64=1.0.6-8.1ubuntu0.2`
- `libbz2-dev:amd64=1.0.6-8.1ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8.1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.dsc' bzip2_1.0.6-8.1ubuntu0.2.dsc 2181 SHA256:62f49d3ded30713bbae8a0aaab69bebdc5533afe6e488ceb0aa03bce7c2c5ff3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2' bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2 61477 SHA256:b4fede4240afa43e0e666e5a539da8d9744b2b2917388cfe93574f967e328e6a
```

### `dpkg` source package: `ca-certificates=20190110~18.04.1`

Binary Packages:

- `ca-certificates=20190110~18.04.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~18.04.1.dsc' ca-certificates_20190110~18.04.1.dsc 1830 SHA256:b5bcd791eb1c232b228766301a7513b404a376fe380c8b19bce504fd1f2312c6
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~18.04.1.tar.xz' ca-certificates_20190110~18.04.1.tar.xz 243664 SHA256:ec23bbc58d8e6bc8b6aa8c0a9081965635a54b474cfd99829e51e2aa25ca6550
```

### `dpkg` source package: `cdebconf=0.213ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.213ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.213ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.213ubuntu1.dsc' cdebconf_0.213ubuntu1.dsc 2769 SHA256:76cb3f0b1685629220b0e4c3105757b95714f7350df4e7863d5310f1f581fee0
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.213ubuntu1.tar.xz' cdebconf_0.213ubuntu1.tar.xz 272596 SHA256:624feaf9e7e5f407271f99e06e54d5002fcce51345553a626caf7b4a65f0afd1
```

### `dpkg` source package: `cmake=3.10.2-1ubuntu2.18.04.1`

Binary Packages:

- `cmake=3.10.2-1ubuntu2.18.04.1`
- `cmake-data=3.10.2-1ubuntu2.18.04.1`

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
$ apt-get source -qq --print-uris cmake=3.10.2-1ubuntu2.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.10.2-1ubuntu2.18.04.1.dsc' cmake_3.10.2-1ubuntu2.18.04.1.dsc 3128 SHA256:7bfca7d610549dcec19d3b4d9e243fc715dd5ccecb23fe90f60355c3ea6f1b28
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.10.2.orig.tar.gz' cmake_3.10.2.orig.tar.gz 7824452 SHA256:80d0faad4ab56de07aa21a7fc692c88c4ce6156d42b0579c6962004a70a3218b
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.10.2-1ubuntu2.18.04.1.debian.tar.xz' cmake_3.10.2-1ubuntu2.18.04.1.debian.tar.xz 30048 SHA256:94840f8fd049baf3b6a535e590442a17c097094b91e5c745a82d3827a3d97999
```

### `dpkg` source package: `console-bridge=0.4.0+dfsg-2`

Binary Packages:

- `libconsole-bridge-dev:amd64=0.4.0+dfsg-2`
- `libconsole-bridge0.4:amd64=0.4.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libconsole-bridge-dev/copyright`, `/usr/share/doc/libconsole-bridge0.4/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris console-bridge=0.4.0+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.4.0+dfsg-2.dsc' console-bridge_0.4.0+dfsg-2.dsc 1949 SHA256:5cfb1b8f43d210c5c1c72bdccb909092b40f361759372211331f75859f29ff91
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.4.0+dfsg.orig.tar.gz' console-bridge_0.4.0+dfsg.orig.tar.gz 6042 SHA256:172eecc6c185de2f6d43aed10c3110b8573e53a49f77c48c3f81a83e0e6e63c2
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.4.0+dfsg-2.debian.tar.xz' console-bridge_0.4.0+dfsg-2.debian.tar.xz 3628 SHA256:56bdfbf50a6e7a83c1f4d1f9052b5b605b8f61846cce7042af0bb6ab661707f7
```

### `dpkg` source package: `coreutils=8.28-1ubuntu1`

Binary Packages:

- `coreutils=8.28-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.28-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28-1ubuntu1.dsc' coreutils_8.28-1ubuntu1.dsc 2302 SHA256:9a7154fd8a458295b686383767f9305095e6ea929a08c8f56cf51640c3fe209f
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz' coreutils_8.28.orig.tar.xz 5252336 SHA256:1117b1a16039ddd84d51a9923948307cfa28c2cea03d1a2438742253df0a0c65
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz.asc' coreutils_8.28.orig.tar.xz.asc 1196 SHA256:505b1a530a55732a9ed659d419ff4973d1b15059078d2060675927058db9607d
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28-1ubuntu1.debian.tar.xz' coreutils_8.28-1ubuntu1.debian.tar.xz 37940 SHA256:71ba2e83edc675a79e1e0556aff326ab2ae812332692e3db29615e8ed1b427f4
```

### `dpkg` source package: `cov-core=1.15.0-2`

Binary Packages:

- `python3-cov-core=1.15.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-cov-core/copyright`)

- `Expat/MIT`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris cov-core=1.15.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cov-core/cov-core_1.15.0-2.dsc' cov-core_1.15.0-2.dsc 2143 SHA256:d9cda18b39093d558319afc2b73222e06ac1a984d2ac233c715c5208862bd32f
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cov-core/cov-core_1.15.0.orig.tar.gz' cov-core_1.15.0.orig.tar.gz 5890 SHA256:4a14c67d520fda9d42b0da6134638578caae1d374b9bb462d8de00587dba764c
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cov-core/cov-core_1.15.0-2.debian.tar.xz' cov-core_1.15.0-2.debian.tar.xz 3944 SHA256:2871a8ff57db7a6ed51bff48222e061c4a23cb7f21bcbb55d1afbdc7d4a47471
```

### `dpkg` source package: `cppcheck=1.82-1`

Binary Packages:

- `cppcheck=1.82-1`

Licenses: (parsed from: `/usr/share/doc/cppcheck/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris cppcheck=1.82-1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cppcheck/cppcheck_1.82-1.dsc' cppcheck_1.82-1.dsc 1941 SHA256:dc93e753bd9d090395d1d2a0b21edc39d8b0d5af0904e7e2658a4a1aa78f24ac
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cppcheck/cppcheck_1.82.orig.tar.gz' cppcheck_1.82.orig.tar.gz 1937115 SHA256:1307f6f3d2caa15dd1380af16a634585570a93f221029ed7b26dbf640da660e7
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cppcheck/cppcheck_1.82-1.debian.tar.xz' cppcheck_1.82-1.debian.tar.xz 368008 SHA256:905c4e2449308660437ade973f1567dcd57381705144a7710a36eabc46024059
```

### `dpkg` source package: `curl=7.58.0-2ubuntu3.10`

Binary Packages:

- `libcurl3-gnutls:amd64=7.58.0-2ubuntu3.10`
- `libcurl4:amd64=7.58.0-2ubuntu3.10`

Licenses: (parsed from: `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.58.0-2ubuntu3.10
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.dsc' curl_7.58.0-2ubuntu3.10.dsc 2781 SHA256:0f80b3add0f3a8c471d1ae4f0aac8d473a3fcba72e9fba398355f16bfcd4615e
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0.orig.tar.gz' curl_7.58.0.orig.tar.gz 3879728 SHA256:cc245bf9a1a42a45df491501d97d5593392a03f7b4f07b952793518d97666115
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.debian.tar.xz' curl_7.58.0-2ubuntu3.10.debian.tar.xz 41908 SHA256:0aca9be6c8fdb0ab69b109b34d4424c99097c894ba8487fd7e28f83bc27f4850
```

### `dpkg` source package: `cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`
- `libsasl2-modules-db:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc 3297 SHA256:2f101f60d7c7245946f9ba90f29d3585b2ef7cb1593275001acb224feb7231e1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz 1143888 SHA256:69f34971f768e7ee6a6b647ec2d16a5a72a854ecd4602b019d5f79ba61063fdc
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz 95712 SHA256:a44bdbd8cfa996c30e617cd0d2fe292819511cc364f42b8169d334bfa7e28e1b
```

### `dpkg` source package: `dash=0.5.8-2.10`

Binary Packages:

- `dash=0.5.8-2.10`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.8-2.10
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.10.dsc' dash_0.5.8-2.10.dsc 1618 SHA256:1e8fdac0880d57d8ed5eb11f9f1750a67c71a7200180cf3ed5aa3e74dab3e4c5
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8.orig.tar.gz' dash_0.5.8.orig.tar.gz 223028 SHA256:c6db3a237747b02d20382a761397563d813b306c020ae28ce25a1c3915fac60f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.10.debian.tar.xz' dash_0.5.8-2.10.debian.tar.xz 43920 SHA256:0d870b0cf9b3ad40e4d4f1e3d4d9097f4d62151693a48f34cb1d49865fd4abdb
```

### `dpkg` source package: `db5.3=5.3.28-13.1ubuntu1.1`

Binary Packages:

- `libdb5.3:amd64=5.3.28-13.1ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-13.1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.dsc' db5.3_5.3.28-13.1ubuntu1.1.dsc 3068 SHA256:1f438506524139f9cb87d3566a6f593186a6543070046e90e1c14c04740d7a0f
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz' db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz 29444 SHA256:d5b19e81a0d94bb29965b84e03855219b80b3bc782aea47e12ad2ace9995b099
```

### `dpkg` source package: `dbus-python=1.2.6-1`

Binary Packages:

- `python3-dbus=1.2.6-1`

Licenses: (parsed from: `/usr/share/doc/python3-dbus/copyright`)

- `AFL-2.1`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dbus-python=1.2.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.6-1.dsc' dbus-python_1.2.6-1.dsc 3278 SHA256:a81fd35d3ca142910d1f7e3f8de57b99596d6e927173a57a44a2917c57eeb72f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.6.orig.tar.gz' dbus-python_1.2.6.orig.tar.gz 778893 SHA256:32f29c17172cdb9cb61c68b1f1a71dfe7351506fc830869029c47449bd04faeb
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.6.orig.tar.gz.asc' dbus-python_1.2.6.orig.tar.gz.asc 833 SHA256:f8a1a9bd38a96361d000f8b69a29201356869a995c0a2b4ce8b47063c53801c3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.6-1.debian.tar.xz' dbus-python_1.2.6-1.debian.tar.xz 32772 SHA256:d342f25b63dbddb8664e6e1bdf400d8c7da081919124b8f56e27252d313a0533
```

### `dpkg` source package: `dbus=1.12.2-1ubuntu1.2`

Binary Packages:

- `libdbus-1-3:amd64=1.12.2-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libdbus-1-3/copyright`)

- `AFL-2.1`
- `AFL-2.1,`
- `BSD-3-clause`
- `BSD-3-clause-generic`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `Tcl-BSDish`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris dbus=1.12.2-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2-1ubuntu1.2.dsc' dbus_1.12.2-1ubuntu1.2.dsc 3561 SHA256:b32c5ff7b7e6ffb950839e5de9487bb40512b158477e1c47c1502a26752c3628
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2.orig.tar.gz' dbus_1.12.2.orig.tar.gz 2063143 SHA256:272bb5091770b047c8188b926d5e6038fa4fe6745488b2add96b23e2d9a83d88
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2-1ubuntu1.2.debian.tar.xz' dbus_1.12.2-1ubuntu1.2.debian.tar.xz 67596 SHA256:8a61cf6c3a0d8def6dc3e2405640e9eaaf8fb4532d670103f80cad3a48d20da2
```

### `dpkg` source package: `debconf=1.5.66ubuntu1`

Binary Packages:

- `debconf=1.5.66ubuntu1`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.66ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.dsc' debconf_1.5.66ubuntu1.dsc 2087 SHA256:6bc588eaa2e880ac33800384328b95a50542097baaba5e89d363798840bb05a2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.tar.xz' debconf_1.5.66ubuntu1.tar.xz 572556 SHA256:d044d6707a6f44a58022575899c852d256ee5b88f4e136f5394652f263e17a95
```

### `dpkg` source package: `debianutils=4.8.4`

Binary Packages:

- `debianutils=4.8.4`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.4
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.4.dsc' debianutils_4.8.4.dsc 1764 SHA256:8b12921fe6e4f51d295bfd4213706d588a6c9b8bab659b0ee1fe525f37e9fbcc
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.4.tar.xz' debianutils_4.8.4.tar.xz 156344 SHA256:c061ab99aea61f892043b7624b021ab5b193e9c6bbfd474da0fbcdd506be1eb2
```

### `dpkg` source package: `defusedxml=0.5.0-1ubuntu1`

Binary Packages:

- `python-defusedxml=0.5.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python-defusedxml/copyright`)

- `Python`

Source:

```console
$ apt-get source -qq --print-uris defusedxml=0.5.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.5.0-1ubuntu1.dsc' defusedxml_0.5.0-1ubuntu1.dsc 2272 SHA256:053ec3c34cd46a2a8f9513180622110fa9331b3092fcfcacbb8bbb370345de0b
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.5.0.orig.tar.gz' defusedxml_0.5.0.orig.tar.gz 60405 SHA256:24d7f2f94f7f3cb6061acb215685e5125fbcdc40a857eff9de22518820b0a4f4
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.5.0-1ubuntu1.debian.tar.xz' defusedxml_0.5.0-1ubuntu1.debian.tar.xz 89668 SHA256:b44231646f08618496da99bc7b014524e9ac0d789eb174f4765cd154ee0971c2
```

### `dpkg` source package: `dh-python=3.20180325ubuntu2`

Binary Packages:

- `dh-python=3.20180325ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dh-python/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris dh-python=3.20180325ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dh-python/dh-python_3.20180325ubuntu2.dsc' dh-python_3.20180325ubuntu2.dsc 1935 SHA256:9600437f909a29468d5e2037e08bf9a2f29869922376a680212bf80c2061de6d
'http://archive.ubuntu.com/ubuntu/pool/main/d/dh-python/dh-python_3.20180325ubuntu2.tar.xz' dh-python_3.20180325ubuntu2.tar.xz 95292 SHA256:aee28c975e9ee74608fad868c1bdfcfacb8c9d771733b210e13b51c9fc5b99d1
```

### `dpkg` source package: `diffutils=1:3.6-1`

Binary Packages:

- `diffutils=1:3.6-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6-1.dsc' diffutils_3.6-1.dsc 1453 SHA256:26fe7690b45748dc92cee6af224192e78db2ac574e16ae0aeb8ed6a472c883cd
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6.orig.tar.xz' diffutils_3.6.orig.tar.xz 1398296 SHA256:d621e8bdd4b573918c8145f7ae61817d1be9deb4c8d2328a65cea8e11d783bd6
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6-1.debian.tar.xz' diffutils_3.6-1.debian.tar.xz 10808 SHA256:f6ab546a134bde18a87ca8e3c98919680e79d81a65a24801ae06ef69b33f24d8
```

### `dpkg` source package: `distlib=0.2.6-1`

Binary Packages:

- `python3-distlib=0.2.6-1`

Licenses: (parsed from: `/usr/share/doc/python3-distlib/copyright`)

- `BSD-3-clause`
- `Python`

Source:

```console
$ apt-get source -qq --print-uris distlib=0.2.6-1
'http://archive.ubuntu.com/ubuntu/pool/universe/d/distlib/distlib_0.2.6-1.dsc' distlib_0.2.6-1.dsc 2032 SHA256:cda699817dbd5b2dfbaa0a6bc9c31cbe9807b01d5990727aea8f0b4cc7b3e9d2
'http://archive.ubuntu.com/ubuntu/pool/universe/d/distlib/distlib_0.2.6.orig.tar.xz' distlib_0.2.6.orig.tar.xz 338504 SHA256:f73a12598ca5c739f5761e0d707d5c707f4640b158a4d61b9cb90b747c5e2fef
'http://archive.ubuntu.com/ubuntu/pool/universe/d/distlib/distlib_0.2.6-1.debian.tar.xz' distlib_0.2.6-1.debian.tar.xz 6340 SHA256:49ff764447c3268455f57d4f33d81b7549adf72ba6fb9c722772c156cb5b71e9
```

### `dpkg` source package: `distro-info-data=0.37ubuntu0.7`

Binary Packages:

- `distro-info-data=0.37ubuntu0.7`

Licenses: (parsed from: `/usr/share/doc/distro-info-data/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris distro-info-data=0.37ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.37ubuntu0.7.dsc' distro-info-data_0.37ubuntu0.7.dsc 1758 SHA256:e101cc4b56ce7f9c243ec59142f5d6894914b9886c729d7a9de0f16d60f4b6c9
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.37ubuntu0.7.tar.xz' distro-info-data_0.37ubuntu0.7.tar.xz 7160 SHA256:1e2409a3a1f1df0255a00ebf645558005e8d777f45cb3a3a95d4203ebb86ed01
```

### `dpkg` source package: `dpkg=1.19.0.5ubuntu2.3`

Binary Packages:

- `dpkg=1.19.0.5ubuntu2.3`
- `dpkg-dev=1.19.0.5ubuntu2.3`
- `libdpkg-perl=1.19.0.5ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.0.5ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.dsc' dpkg_1.19.0.5ubuntu2.3.dsc 2144 SHA256:ac37d92c336bf4360cedce228d94ba4af248da265e5c161f33b06ed929fbe401
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.tar.xz' dpkg_1.19.0.5ubuntu2.3.tar.xz 4571256 SHA256:4945a605113fac66d275937b5de3678398f32ded55352cd773619c30ab1bd9a5
```

### `dpkg` source package: `e2fsprogs=1.44.1-1ubuntu1.3`

Binary Packages:

- `e2fsprogs=1.44.1-1ubuntu1.3`
- `libcom-err2:amd64=1.44.1-1ubuntu1.3`
- `libext2fs2:amd64=1.44.1-1ubuntu1.3`
- `libss2:amd64=1.44.1-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.44.1-1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.dsc' e2fsprogs_1.44.1-1ubuntu1.3.dsc 3188 SHA256:91385415b8464ff34676bb5129d6bd16e5db599b9a01ef82198e5f5517fd6191
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz' e2fsprogs_1.44.1.orig.tar.gz 7544908 SHA256:a5a8068dfe105050d8c63d67515a0ae5fff3f37232f725e0aa72b389eeb6c1e6
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz.asc' e2fsprogs_1.44.1.orig.tar.gz.asc 488 SHA256:6e8eb8df52f5cd577f5eae489108c6fbe2c5381e01f83c325873e034d5a84e46
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz' e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz 81152 SHA256:923cef16c7ce15022672ed0992f9ce9202f9331eead7c88b47bba52106189eac
```

### `dpkg` source package: `eigen3=3.3.4-4`

Binary Packages:

- `libeigen3-dev=3.3.4-4`

Licenses: (parsed from: `/usr/share/doc/libeigen3-dev/copyright`)

- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-2`

Source:

```console
$ apt-get source -qq --print-uris eigen3=3.3.4-4
'http://archive.ubuntu.com/ubuntu/pool/universe/e/eigen3/eigen3_3.3.4-4.dsc' eigen3_3.3.4-4.dsc 2188 SHA256:83cdceb0249d063984d43dcb6c8803ef1518d7f15764ef5362dab9980e64b3b8
'http://archive.ubuntu.com/ubuntu/pool/universe/e/eigen3/eigen3_3.3.4.orig.tar.bz2' eigen3_3.3.4.orig.tar.bz2 1657543 SHA256:dd254beb0bafc695d0f62ae1a222ff85b52dbaa3a16f76e781dce22d0d20a4a6
'http://archive.ubuntu.com/ubuntu/pool/universe/e/eigen3/eigen3_3.3.4-4.debian.tar.xz' eigen3_3.3.4-4.debian.tar.xz 44568 SHA256:37108f240488e9185e17f357742e41b390b78ccce148f0ccd722f4c1b905a285
```

### `dpkg` source package: `elfutils=0.170-0.4ubuntu0.1`

Binary Packages:

- `libelf1:amd64=0.170-0.4ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.170-0.4ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170-0.4ubuntu0.1.dsc' elfutils_0.170-0.4ubuntu0.1.dsc 2422 SHA256:2c856af4e5833a5546ed8d82886fe8e7e3017375b1f2572d1873790bbf124b12
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170.orig.tar.bz2' elfutils_0.170.orig.tar.bz2 8358001 SHA256:1f844775576b79bdc9f9c717a50058d08620323c1e935458223a12f249c9e066
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170-0.4ubuntu0.1.debian.tar.xz' elfutils_0.170-0.4ubuntu0.1.debian.tar.xz 51740 SHA256:9978a38393fac9df0bcb6eeb08741cf29d3161beeb463e2d8e26cb1a7fe8a3cc
```

### `dpkg` source package: `empy=3.3.2-1build1`

Binary Packages:

- `python-empy=3.3.2-1build1`
- `python3-empy=3.3.2-1build1`

Licenses: (parsed from: `/usr/share/doc/python-empy/copyright`, `/usr/share/doc/python3-empy/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris empy=3.3.2-1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2-1build1.dsc' empy_3.3.2-1build1.dsc 2161 SHA256:4fee77941fc5406214e9d2387b631040165329e0084319e5f5af52c0df948862
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2.orig.tar.gz' empy_3.3.2.orig.tar.gz 138168 SHA256:99f016af2770c48ab57a65df7aae251360dc69a1514c15851458a71d4ddfea9c
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2-1build1.debian.tar.xz' empy_3.3.2-1build1.debian.tar.xz 4688 SHA256:50eae836a5dbde23d563ef04b96e6e1f7bfc2cab6ab6ed1d62c68aacc235af21
```

### `dpkg` source package: `enum34=1.1.6-2`

Binary Packages:

- `python-enum34=1.1.6-2`

Licenses: (parsed from: `/usr/share/doc/python-enum34/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris enum34=1.1.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/e/enum34/enum34_1.1.6-2.dsc' enum34_1.1.6-2.dsc 2194 SHA256:b3a8c78fd3289f68e6d2f4a21797ed74503c9cfd90d0e427ecb4a0106f3b1143
'http://archive.ubuntu.com/ubuntu/pool/main/e/enum34/enum34_1.1.6.orig.tar.gz' enum34_1.1.6.orig.tar.gz 40048 SHA256:8ad8c4783bf61ded74527bffb48ed9b54166685e4230386a9ed9b1279e2df5b1
'http://archive.ubuntu.com/ubuntu/pool/main/e/enum34/enum34_1.1.6-2.debian.tar.xz' enum34_1.1.6-2.debian.tar.xz 4036 SHA256:2b2a7b18652a66a81c23b665b9dfcc35bfd3d3d6d2262b6b4faf32cf0bc97ab7
```

### `dpkg` source package: `expat=2.2.5-3ubuntu0.2`

Binary Packages:

- `libexpat1:amd64=2.2.5-3ubuntu0.2`
- `libexpat1-dev:amd64=2.2.5-3ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.5-3ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.dsc' expat_2.2.5-3ubuntu0.2.dsc 2198 SHA256:680793c534c3f2ccee1251f6b03c445454250d320e31021a30f8b2fe571e75d5
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5.orig.tar.gz' expat_2.2.5.orig.tar.gz 8273003 SHA256:b3781742738611eaa737543ee94264dd511c52a3ba7e53111f7d705f6bff65a8
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.debian.tar.xz' expat_2.2.5-3ubuntu0.2.debian.tar.xz 12024 SHA256:9d9b040636ebf98fe3e401e6ebacc53073a2d508385bc91bde0fcb6b2aaa5675
```

### `dpkg` source package: `findutils=4.6.0+git+20170828-2`

Binary Packages:

- `findutils=4.6.0+git+20170828-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20170828-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828-2.dsc' findutils_4.6.0+git+20170828-2.dsc 2221 SHA256:6997072de2f1b24457073275f7b8f15ad2f0569389dcb277ebe99dd1846e2ee9
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828.orig.tar.xz' findutils_4.6.0+git+20170828.orig.tar.xz 1865192 SHA256:8d6571ffd5105307bcb1b20c4b7d5c2d0b5152e463b082801268bd3ec9e2bbfd
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828-2.debian.tar.xz' findutils_4.6.0+git+20170828-2.debian.tar.xz 26532 SHA256:5b13792a14edec982fddcf74fe01b4380b909703d76aaba2860da51c6248de73
```

### `dpkg` source package: `freetype=2.8.1-2ubuntu2`

Binary Packages:

- `libfreetype6:amd64=2.8.1-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `Catharon-OSL`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GZip`
- `OpenGroup-BSD-like`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.8.1-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1-2ubuntu2.dsc' freetype_2.8.1-2ubuntu2.dsc 2288 SHA256:f7a1e8715cc35405d814fd97478e37ff22fad2bb639c049e058298c9f5847015
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1.orig.tar.gz' freetype_2.8.1.orig.tar.gz 4242784 SHA256:a7531cb8c2f6b709896f018380ad97e677e243847ff8a098d1b8b5d23e9d74d7
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1-2ubuntu2.diff.gz' freetype_2.8.1-2ubuntu2.diff.gz 44335 SHA256:ec498da97b3c1715b67f8d6ed85e6d9a2eb8b709cabce38519a8ab5ca995b85a
```

### `dpkg` source package: `gcc-7=7.5.0-3ubuntu1~18.04`

Binary Packages:

- `cpp-7=7.5.0-3ubuntu1~18.04`
- `g++-7=7.5.0-3ubuntu1~18.04`
- `gcc-7=7.5.0-3ubuntu1~18.04`
- `gcc-7-base:amd64=7.5.0-3ubuntu1~18.04`
- `libasan4:amd64=7.5.0-3ubuntu1~18.04`
- `libcilkrts5:amd64=7.5.0-3ubuntu1~18.04`
- `libgcc-7-dev:amd64=7.5.0-3ubuntu1~18.04`
- `libgfortran4:amd64=7.5.0-3ubuntu1~18.04`
- `libstdc++-7-dev:amd64=7.5.0-3ubuntu1~18.04`
- `libubsan0:amd64=7.5.0-3ubuntu1~18.04`

Licenses: (parsed from: `/usr/share/doc/cpp-7/copyright`, `/usr/share/doc/g++-7/copyright`, `/usr/share/doc/gcc-7/copyright`, `/usr/share/doc/gcc-7-base/copyright`, `/usr/share/doc/libasan4/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-7-dev/copyright`, `/usr/share/doc/libgfortran4/copyright`, `/usr/share/doc/libstdc++-7-dev/copyright`, `/usr/share/doc/libubsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-7=7.5.0-3ubuntu1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0-3ubuntu1~18.04.dsc' gcc-7_7.5.0-3ubuntu1~18.04.dsc 28071 SHA256:3e93f39cd8c8ac5d05e5f1af16674864c9cfe7fdbe23274c756cf07e1ff81548
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0.orig.tar.gz' gcc-7_7.5.0.orig.tar.gz 73877115 SHA256:dd7f095be2cd6aa61bd914b5b8e78daccae741a816cf19357cd767bef24ec390
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0-3ubuntu1~18.04.diff.gz' gcc-7_7.5.0-3ubuntu1~18.04.diff.gz 574614 SHA256:42d3fef17cd5561df6187ce0c11bdb61f78cbb2da56bfd6e9983b138077f82f2
```

### `dpkg` source package: `gcc-8=8.4.0-1ubuntu1~18.04`

Binary Packages:

- `gcc-8-base:amd64=8.4.0-1ubuntu1~18.04`
- `libatomic1:amd64=8.4.0-1ubuntu1~18.04`
- `libcc1-0:amd64=8.4.0-1ubuntu1~18.04`
- `libgcc1:amd64=1:8.4.0-1ubuntu1~18.04`
- `libgomp1:amd64=8.4.0-1ubuntu1~18.04`
- `libitm1:amd64=8.4.0-1ubuntu1~18.04`
- `liblsan0:amd64=8.4.0-1ubuntu1~18.04`
- `libmpx2:amd64=8.4.0-1ubuntu1~18.04`
- `libquadmath0:amd64=8.4.0-1ubuntu1~18.04`
- `libstdc++6:amd64=8.4.0-1ubuntu1~18.04`
- `libtsan0:amd64=8.4.0-1ubuntu1~18.04`

Licenses: (parsed from: `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libmpx2/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-8=8.4.0-1ubuntu1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.dsc' gcc-8_8.4.0-1ubuntu1~18.04.dsc 36382 SHA256:bf7f453948fc746550c79b00c0af3940a2ff00c2f1692a376ebb90393963355a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0.orig.tar.gz' gcc-8_8.4.0.orig.tar.gz 85278215 SHA256:eb917ceb079e90afe1e524dee295e2360c63b923c611ae231144385be37dde2a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.diff.gz' gcc-8_8.4.0-1ubuntu1~18.04.diff.gz 510634 SHA256:5dbda7df03e650d72ad7c54ad8d8a48389ee358ebfad18a40bf6d8bb57c8c2ad
```

### `dpkg` source package: `gcc-defaults=1.176ubuntu2.3`

Binary Packages:

- `cpp=4:7.4.0-1ubuntu2.3`
- `g++=4:7.4.0-1ubuntu2.3`
- `gcc=4:7.4.0-1ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.176ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.176ubuntu2.3.dsc' gcc-defaults_1.176ubuntu2.3.dsc 15463 SHA256:effaa8ad1f705006442122375b445d02a500d20ef9565e6613cd04d0b201b660
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.176ubuntu2.3.tar.gz' gcc-defaults_1.176ubuntu2.3.tar.gz 208597 SHA256:5ddfada25e49d0cbc842ebbf3a8885cfdd7ba5f500ffdbfa2e20758d268254fa
```

### `dpkg` source package: `gdbm=1.14.1-6`

Binary Packages:

- `libgdbm-compat4:amd64=1.14.1-6`
- `libgdbm5:amd64=1.14.1-6`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm5/copyright`)

- `GFDL-1.3+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.14.1-6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1-6.dsc' gdbm_1.14.1-6.dsc 2293 SHA256:85fc353e81fc54b49d9c13c71f4247836fb1aac2693e98416a6821de8cfe7b41
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1.orig.tar.gz' gdbm_1.14.1.orig.tar.gz 894412 SHA256:cdceff00ffe014495bed3aed71c7910aa88bf29379f795abc0f46d4ee5f8bc5f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1-6.debian.tar.xz' gdbm_1.14.1-6.debian.tar.xz 27492 SHA256:c9da59f11d5e40ecd877f1256c53ea4750b9d614c7885800e42d0f1885996658
```

### `dpkg` source package: `git=1:2.17.1-1ubuntu0.7`

Binary Packages:

- `git=1:2.17.1-1ubuntu0.7`
- `git-man=1:2.17.1-1ubuntu0.7`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-2-clause`
- `Boost`
- `EDL-1.0`
- `Expat`
- `GPL`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `dlmalloc`
- `mingw-runtime`

Source:

```console
$ apt-get source -qq --print-uris git=1:2.17.1-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.17.1-1ubuntu0.7.dsc' git_2.17.1-1ubuntu0.7.dsc 2959 SHA256:b1458c126514fe76de4fb2be7b2850f6b69ecaa35f89f64defb37200a46da2e3
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.17.1.orig.tar.xz' git_2.17.1.orig.tar.xz 5015484 SHA256:79136e7aa83abae4d8a25c8111f113d3c5a63aeb5fd93cc72c26d49c6d5ba65e
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.17.1-1ubuntu0.7.debian.tar.xz' git_2.17.1-1ubuntu0.7.debian.tar.xz 614088 SHA256:169a0d8139dbe57dc4e7300b3677f100b1fdc660dae66e6b81b338d4eaa9c54a
```

### `dpkg` source package: `glib2.0=2.56.4-0ubuntu0.18.04.6`

Binary Packages:

- `libglib2.0-0:amd64=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-bin=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-data=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-dev:amd64=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-dev-bin=2.56.4-0ubuntu0.18.04.6`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.56.4-0ubuntu0.18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.dsc' glib2.0_2.56.4-0ubuntu0.18.04.6.dsc 3301 SHA256:a4cc68dbc3255f458789213e5eaa1ff1c409d8fc49688c9b136cfa4ef30dafa1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4.orig.tar.xz' glib2.0_2.56.4.orig.tar.xz 7029768 SHA256:27f703d125efb07f8a743666b580df0b4095c59fc8750e8890132c91d437504c
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz' glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz 89540 SHA256:57f17e1760946894ae729e988798ac11339460e8ee71421c6b0a5b6cdde9af36
```

### `dpkg` source package: `glibc=2.27-3ubuntu1.2`

Binary Packages:

- `libc-bin=2.27-3ubuntu1.2`
- `libc-dev-bin=2.27-3ubuntu1.2`
- `libc6:amd64=2.27-3ubuntu1.2`
- `libc6-dev:amd64=2.27-3ubuntu1.2`
- `multiarch-support=2.27-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.27-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.2.dsc' glibc_2.27-3ubuntu1.2.dsc 9364 SHA256:2ac325cce2251c710dd041f4725925cdbccefba6f6f0f0d95a2a5a09e2050c2e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27.orig.tar.xz' glibc_2.27.orig.tar.xz 15923832 SHA256:0e9826488e3ffedb4d14a426d741b7b1cf15f6973ab30762af9a188ad47633ed
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.2.debian.tar.xz' glibc_2.27-3ubuntu1.2.debian.tar.xz 1014508 SHA256:e488a6293dfb3b8074b9be03655ffd3c98f2d0a5b8bb2a29cf4c526fbf01dcb0
```

### `dpkg` source package: `gmp=2:6.1.2+dfsg-2`

Binary Packages:

- `libgmp10:amd64=2:6.1.2+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-2.dsc' gmp_6.1.2+dfsg-2.dsc 2152 SHA256:d1e7b69c619c2d07b3eaf9f051159cde1884cf9c68109f1dee278bf7a59b632b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-2.debian.tar.xz' gmp_6.1.2+dfsg-2.debian.tar.xz 20744 SHA256:33cf6cc65827c9df744e4e07b216ca2d02eb57327a949f80a7b7dddd0485ee85
```

### `dpkg` source package: `gnupg2=2.2.4-1ubuntu1.2`

Binary Packages:

- `dirmngr=2.2.4-1ubuntu1.2`
- `gnupg=2.2.4-1ubuntu1.2`
- `gnupg-l10n=2.2.4-1ubuntu1.2`
- `gnupg-utils=2.2.4-1ubuntu1.2`
- `gnupg2=2.2.4-1ubuntu1.2`
- `gpg=2.2.4-1ubuntu1.2`
- `gpg-agent=2.2.4-1ubuntu1.2`
- `gpg-wks-client=2.2.4-1ubuntu1.2`
- `gpg-wks-server=2.2.4-1ubuntu1.2`
- `gpgconf=2.2.4-1ubuntu1.2`
- `gpgsm=2.2.4-1ubuntu1.2`
- `gpgv=2.2.4-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-l10n/copyright`, `/usr/share/doc/gnupg-utils/copyright`, `/usr/share/doc/gnupg2/copyright`, `/usr/share/doc/gpg/copyright`, `/usr/share/doc/gpg-agent/copyright`, `/usr/share/doc/gpg-wks-client/copyright`, `/usr/share/doc/gpg-wks-server/copyright`, `/usr/share/doc/gpgconf/copyright`, `/usr/share/doc/gpgsm/copyright`, `/usr/share/doc/gpgv/copyright`)

- `BSD-3-clause`
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gnutls28=3.5.18-1ubuntu1.4`

Binary Packages:

- `libgnutls30:amd64=3.5.18-1ubuntu1.4`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The MIT License (MIT)`
- `The main library is licensed under GNU Lesser`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.5.18-1ubuntu1.4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.dsc' gnutls28_3.5.18-1ubuntu1.4.dsc 2780 SHA256:6c58a44e5790eb86989318bf660e2391561c04518d4d8c7b85fb495a4efcd5ae
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz' gnutls28_3.5.18.orig.tar.xz 7261980 SHA256:ae2248d9e78747cf9c469dde81ff8f90b56838b707a0637f3f7d4eee90e80234
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz.asc' gnutls28_3.5.18.orig.tar.xz.asc 534 SHA256:50bb942469be0639bbab925de630fb921aa8cac5f40072cb1c2cf1fb7ae7977b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz' gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz 83784 SHA256:3ff4cbd5e9b6d9d51479fdae70486598ad7c11dae50aa06e98f000290f30cd05
```

### `dpkg` source package: `gobject-introspection=1.56.1-1`

Binary Packages:

- `gir1.2-glib-2.0:amd64=1.56.1-1`
- `libgirepository-1.0-1:amd64=1.56.1-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.56.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.56.1-1.dsc' gobject-introspection_1.56.1-1.dsc 2915 SHA256:978c16c9988d7bc6fed4f112012d9027d5add7e783d405057c4757e8d377a5a5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.56.1.orig.tar.xz' gobject-introspection_1.56.1.orig.tar.xz 1397812 SHA256:5b2875ccff99ff7baab63a34b67f8c920def240e178ff50add809e267d9ea24b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.56.1-1.debian.tar.xz' gobject-introspection_1.56.1-1.debian.tar.xz 20460 SHA256:20fb97a39c69106ab3b008b31e0409bc6de47989a888004c24dba64397151d86
```

### `dpkg` source package: `googletest=1.8.0-6`

Binary Packages:

- `google-mock:amd64=1.8.0-6`
- `googletest:amd64=1.8.0-6`
- `libgtest-dev:amd64=1.8.0-6`

Licenses: (parsed from: `/usr/share/doc/google-mock/copyright`, `/usr/share/doc/googletest/copyright`, `/usr/share/doc/libgtest-dev/copyright`)

- `Apache`
- `BSD-C3`
- `GAP`

Source:

```console
$ apt-get source -qq --print-uris googletest=1.8.0-6
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.8.0-6.dsc' googletest_1.8.0-6.dsc 2077 SHA256:80407dd39851eee21860f05b4f3d88e9c3fb905d3aa33c4a19496ddc33da66d4
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.8.0.orig.tar.gz' googletest_1.8.0.orig.tar.gz 1281617 SHA256:58a6f4277ca2bc8565222b3bbd58a177609e9c488e8a72649359ba51450db7d8
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.8.0-6.debian.tar.xz' googletest_1.8.0-6.debian.tar.xz 8492 SHA256:0b11f825aae0c84d1b0be43ffc3e6b288d2c3b064f94ac5f241a72493a51b253
```

### `dpkg` source package: `gpgme1.0=1.10.0-1ubuntu2`

Binary Packages:

- `libgpgme-dev=1.10.0-1ubuntu2`
- `libgpgme11:amd64=1.10.0-1ubuntu2`

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
$ apt-get source -qq --print-uris gpgme1.0=1.10.0-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0-1ubuntu2.dsc' gpgme1.0_1.10.0-1ubuntu2.dsc 3046 SHA256:fe60f76894d4f8b089e456762978f7fb5e78592cf0fa039b8980edca72c3448b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0.orig.tar.bz2' gpgme1.0_1.10.0.orig.tar.bz2 1370162 SHA256:1a8fed1197c3b99c35f403066bb344a26224d292afc048cfdfc4ccd5690a0693
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0.orig.tar.bz2.asc' gpgme1.0_1.10.0.orig.tar.bz2.asc 534 SHA256:a7058cd592ae81c35fc05bcc6b32019a025ab5ef65a01402ceeb533a104a50b5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0-1ubuntu2.debian.tar.xz' gpgme1.0_1.10.0-1ubuntu2.debian.tar.xz 18372 SHA256:792b744cc5b0a8af5f125641e5bc4a86c3862b7a9cf3ae6ba74ee0f16d3553c1
```

### `dpkg` source package: `graphite2=1.3.11-2`

Binary Packages:

- `libgraphite2-3:amd64=1.3.11-2`
- `libgraphite2-dev:amd64=1.3.11-2`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`, `/usr/share/doc/libgraphite2-dev/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-2.1+ `
- `MPL-1.1`
- `custom-sil-open-font-license`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.11-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11-2.dsc' graphite2_1.3.11-2.dsc 2367 SHA256:3c2f5ed2b6021e9a18456215d5d01354434f14577dbc862f7f53c8ce62200d71
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11.orig.tar.gz' graphite2_1.3.11.orig.tar.gz 4236768 SHA256:945c01d3647b355d68e5541773fc99a7f29ede6a264bcbd735156a7c493459ff
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11-2.debian.tar.xz' graphite2_1.3.11-2.debian.tar.xz 14068 SHA256:c47ef4ae6edfa6ce02483f347e67786b0fce089515087370ccc10f22ad711f90
```

### `dpkg` source package: `grep=3.1-2build1`

Binary Packages:

- `grep=3.1-2build1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.dsc' grep_3.1-2build1.dsc 2116 SHA256:b9dff3a4089e3491a057c76fe2d941bbc669c1f9d934f5929052d32abd952961
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1.orig.tar.xz' grep_3.1.orig.tar.xz 1370880 SHA256:db625c7ab3bb3ee757b3926a5cfa8d9e1c3991ad24707a83dde8a5ef2bf7a07e
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.debian.tar.bz2' grep_3.1-2build1.debian.tar.bz2 110087 SHA256:699bbd6681e4ef27a24b9876b6b2c3b1ce1be1b140676cd051170e5cc05dd876
```

### `dpkg` source package: `gzip=1.6-5ubuntu1`

Binary Packages:

- `gzip=1.6-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-5ubuntu1.dsc' gzip_1.6-5ubuntu1.dsc 2023 SHA256:439e340fce084b9b30e22a5537712f9b4727a20e77952addeea7633a4e9ef073
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-5ubuntu1.debian.tar.xz' gzip_1.6-5ubuntu1.debian.tar.xz 15516 SHA256:db01e3f2195cf0ebcf43ad38d07a70059b6b5b292706f2412de34928b9146db5
```

### `dpkg` source package: `harfbuzz=1.7.2-1ubuntu1`

Binary Packages:

- `gir1.2-harfbuzz-0.0:amd64=1.7.2-1ubuntu1`
- `libharfbuzz-dev:amd64=1.7.2-1ubuntu1`
- `libharfbuzz-gobject0:amd64=1.7.2-1ubuntu1`
- `libharfbuzz-icu0:amd64=1.7.2-1ubuntu1`
- `libharfbuzz0b:amd64=1.7.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-harfbuzz-0.0/copyright`, `/usr/share/doc/libharfbuzz-dev/copyright`, `/usr/share/doc/libharfbuzz-gobject0/copyright`, `/usr/share/doc/libharfbuzz-icu0/copyright`, `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=1.7.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2-1ubuntu1.dsc' harfbuzz_1.7.2-1ubuntu1.dsc 2825 SHA256:0222317c07eecbb164a537694dcb01ff4c658a56e577f9667cbb8ec144d287fa
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2.orig.tar.bz2' harfbuzz_1.7.2.orig.tar.bz2 1708416 SHA256:a790585e35c1a87f0dcc23580c84b7cc2324e6f67a2946178d278c2a36c790cb
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2-1ubuntu1.debian.tar.xz' harfbuzz_1.7.2-1ubuntu1.debian.tar.xz 9168 SHA256:f94a2a0990fd0b39fdef14444fa39b0bd1d15f6c79e74b697856ba2cef06b0bf
```

### `dpkg` source package: `heimdal=7.5.0+dfsg-1`

Binary Packages:

- `libasn1-8-heimdal:amd64=7.5.0+dfsg-1`
- `libgssapi3-heimdal:amd64=7.5.0+dfsg-1`
- `libhcrypto4-heimdal:amd64=7.5.0+dfsg-1`
- `libheimbase1-heimdal:amd64=7.5.0+dfsg-1`
- `libheimntlm0-heimdal:amd64=7.5.0+dfsg-1`
- `libhx509-5-heimdal:amd64=7.5.0+dfsg-1`
- `libkrb5-26-heimdal:amd64=7.5.0+dfsg-1`
- `libroken18-heimdal:amd64=7.5.0+dfsg-1`
- `libwind0-heimdal:amd64=7.5.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libasn1-8-heimdal/copyright`, `/usr/share/doc/libgssapi3-heimdal/copyright`, `/usr/share/doc/libhcrypto4-heimdal/copyright`, `/usr/share/doc/libheimbase1-heimdal/copyright`, `/usr/share/doc/libheimntlm0-heimdal/copyright`, `/usr/share/doc/libhx509-5-heimdal/copyright`, `/usr/share/doc/libkrb5-26-heimdal/copyright`, `/usr/share/doc/libroken18-heimdal/copyright`, `/usr/share/doc/libwind0-heimdal/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `custom`
- `none`

Source:

```console
$ apt-get source -qq --print-uris heimdal=7.5.0+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-1.dsc' heimdal_7.5.0+dfsg-1.dsc 3674 SHA256:98ce6bf21ac01400ec10a3620fe3c047da4cf63269f521ba96c59bbcaed822bf
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg.orig.tar.gz' heimdal_7.5.0+dfsg.orig.tar.gz 8955005 SHA256:489119b7a1a900b88163765654dc59cba9a321b078fafc76629e2b85ef140867
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-1.debian.tar.xz' heimdal_7.5.0+dfsg-1.debian.tar.xz 125776 SHA256:7ad6c3f3968989ff06181409e1515a3feaf5a630d27ade7f2f018c9241f8c225
```

### `dpkg` source package: `hostname=3.20`

Binary Packages:

- `hostname=3.20`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.20
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.20.dsc' hostname_3.20.dsc 1429 SHA256:1fd7b0b2b61e58aa0e50de4d375072c938cb3cc4b722bc73e085e3a3691d9114
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.20.tar.gz' hostname_3.20.tar.gz 13336 SHA256:e7ed56f8c532573ff34d9bd6e7a10d04fbbb2c7fae187898805868e5fed24ab0
```

### `dpkg` source package: `hwloc=1.11.9-1`

Binary Packages:

- `libhwloc-dev:amd64=1.11.9-1`
- `libhwloc-plugins=1.11.9-1`
- `libhwloc5:amd64=1.11.9-1`

Licenses: (parsed from: `/usr/share/doc/libhwloc-dev/copyright`, `/usr/share/doc/libhwloc-plugins/copyright`, `/usr/share/doc/libhwloc5/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris hwloc=1.11.9-1
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_1.11.9-1.dsc' hwloc_1.11.9-1.dsc 2661 SHA256:96705c8bef41c088d215dab615f4a813658cdb4ad5b6d18ec8d463eac6bf88f5
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_1.11.9.orig.tar.bz2' hwloc_1.11.9.orig.tar.bz2 4221902 SHA256:394333184248d63cb2708a976e57f05337d03bb50c33aa3097ff5c5a74a85164
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_1.11.9-1.debian.tar.bz2' hwloc_1.11.9-1.debian.tar.bz2 10200 SHA256:82d20f317a796b196e19c1b6029a2c694a95aaee59be7f36c04a3021efa83ef6
```

### `dpkg` source package: `icu-le-hb=1.0.3+git161113-4`

Binary Packages:

- `libicu-le-hb-dev:amd64=1.0.3+git161113-4`
- `libicu-le-hb0:amd64=1.0.3+git161113-4`

Licenses: (parsed from: `/usr/share/doc/libicu-le-hb-dev/copyright`, `/usr/share/doc/libicu-le-hb0/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu-le-hb=1.0.3+git161113-4
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu-le-hb/icu-le-hb_1.0.3+git161113-4.dsc' icu-le-hb_1.0.3+git161113-4.dsc 1929 SHA256:e486c93a9795a26347607ea19ad2ca97e043b6de3dcbbc8bf70b0826d740ed50
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu-le-hb/icu-le-hb_1.0.3+git161113.orig.tar.xz' icu-le-hb_1.0.3+git161113.orig.tar.xz 31460 SHA256:777cdb6fecedb6400cab85894a8407bb70771e38a0e99b837ccf9e4a55f8578c
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu-le-hb/icu-le-hb_1.0.3+git161113-4.debian.tar.xz' icu-le-hb_1.0.3+git161113-4.debian.tar.xz 3176 SHA256:e140404464ff5c26af2f7f2f974cb4447e833a64f4529e85564ad367fb483ee5
```

### `dpkg` source package: `icu=60.2-3ubuntu3.1`

Binary Packages:

- `icu-devtools=60.2-3ubuntu3.1`
- `libicu-dev=60.2-3ubuntu3.1`
- `libicu60:amd64=60.2-3ubuntu3.1`
- `libiculx60:amd64=60.2-3ubuntu3.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=60.2-3ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.dsc' icu_60.2-3ubuntu3.1.dsc 2149 SHA256:eb8ac79f5fdbd30cfedbf8e5f2c3997dac813115aab9b583dfeced859889ac57
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2.orig.tar.gz' icu_60.2.orig.tar.gz 23315541 SHA256:a8c2ddbdf2be01c7ddcfded837afe46362e1069ea6093f66816b2d1caa8272ae
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.debian.tar.xz' icu_60.2-3ubuntu3.1.debian.tar.xz 29068 SHA256:b93559560abae724d3466f3d84a362282f97bb6562a82e99da06846f0dc6c09c
```

### `dpkg` source package: `infinipath-psm=3.3+20.604758e7-5`

Binary Packages:

- `libpsm-infinipath1=3.3+20.604758e7-5`

Licenses: (parsed from: `/usr/share/doc/libpsm-infinipath1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris infinipath-psm=3.3+20.604758e7-5
'http://archive.ubuntu.com/ubuntu/pool/universe/i/infinipath-psm/infinipath-psm_3.3+20.604758e7-5.dsc' infinipath-psm_3.3+20.604758e7-5.dsc 2284 SHA256:5b42b5d421a2bcc86999a019adfeeb0194584ac586374a285d6ae54ac018e2ac
'http://archive.ubuntu.com/ubuntu/pool/universe/i/infinipath-psm/infinipath-psm_3.3+20.604758e7.orig.tar.xz' infinipath-psm_3.3+20.604758e7.orig.tar.xz 287112 SHA256:2fb37b3436866b7f6d7244edded875bf7ebc89e7a09a1f372ace548d0f90481d
'http://archive.ubuntu.com/ubuntu/pool/universe/i/infinipath-psm/infinipath-psm_3.3+20.604758e7-5.debian.tar.xz' infinipath-psm_3.3+20.604758e7-5.debian.tar.xz 9312 SHA256:d1cc95c8f929d86ebdd3ea12214ee7a9d4493db1f2cd2b9332f89c56ccab0a63
```

### `dpkg` source package: `init-system-helpers=1.51`

Binary Packages:

- `init-system-helpers=1.51`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.51
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.51.dsc' init-system-helpers_1.51.dsc 1963 SHA256:82f0e30fef2ad14c65f9c7d8ccafd43549451041fdf661dca28b963a6cef02e4
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.51.tar.xz' init-system-helpers_1.51.tar.xz 37468 SHA256:e18b28efe8df087146d9c1e4e9c25386ee1b7312f518d48a2a38469a6c661be0
```

### `dpkg` source package: `isl=0.19-1`

Binary Packages:

- `libisl19:amd64=0.19-1`

Licenses: (parsed from: `/usr/share/doc/libisl19/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.19-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19-1.dsc' isl_0.19-1.dsc 1833 SHA256:f9786677430e2ea7295c6ad9480e7e710582f84b5b850a5ddfe1f21b3d726b0f
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19.orig.tar.xz' isl_0.19.orig.tar.xz 1515156 SHA256:6d6c1aa00e2a6dfc509fa46d9a9dbe93af0c451e196a670577a148feecf6b8a5
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19-1.debian.tar.xz' isl_0.19-1.debian.tar.xz 22388 SHA256:aa034a5700c63867aae836a1f985fccc50ccacd1abe57a2a016e076fa745feb0
```

### `dpkg` source package: `jquery-goodies=12-1`

Binary Packages:

- `libjs-jquery-metadata=12-1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-metadata/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris jquery-goodies=12-1
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-goodies/jquery-goodies_12-1.dsc' jquery-goodies_12-1.dsc 3270 SHA256:0e1f2f4667a5a615b8d6ba6671554d634ede413e71e3d1ebea272593c6e096d2
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-goodies/jquery-goodies_12.orig.tar.xz' jquery-goodies_12.orig.tar.xz 1238604 SHA256:d9d986d075e2b2d534b713433f2c0ab47ffb0c3a1ce12ebea4c9e40aecd1bcbf
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-goodies/jquery-goodies_12-1.debian.tar.xz' jquery-goodies_12-1.debian.tar.xz 12604 SHA256:347e65a996b8fe60015e34a86000ba544926054478b64bbf93deeb09f89dbf33
```

### `dpkg` source package: `jquery-tablesorter=1:2.29.5+dfsg1-1`

Binary Packages:

- `libjs-jquery-tablesorter=1:2.29.5+dfsg1-1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-tablesorter/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-2+`
- `expat`

Source:

```console
$ apt-get source -qq --print-uris jquery-tablesorter=1:2.29.5+dfsg1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-tablesorter/jquery-tablesorter_2.29.5+dfsg1-1.dsc' jquery-tablesorter_2.29.5+dfsg1-1.dsc 1870 SHA256:e42d559c920996804b4ca797de9f13fb07b06ea3dd8f304c42f61b31d9401b99
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-tablesorter/jquery-tablesorter_2.29.5+dfsg1.orig.tar.gz' jquery-tablesorter_2.29.5+dfsg1.orig.tar.gz 957573 SHA256:b37805b85bac328a5d45a57f55e1a6e3923ce20cefdb42620304e8aab3242c20
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-tablesorter/jquery-tablesorter_2.29.5+dfsg1-1.debian.tar.xz' jquery-tablesorter_2.29.5+dfsg1-1.debian.tar.xz 4396 SHA256:2fa0cee31ccf525abd94af77c9c2d682a5587efeaabe7226c49e79dee3b45ffd
```

### `dpkg` source package: `jquery-throttle-debounce=1.1+dfsg.1-1`

Binary Packages:

- `libjs-jquery-throttle-debounce=1.1+dfsg.1-1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-throttle-debounce/copyright`)

- `Expat`
- `GPL`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris jquery-throttle-debounce=1.1+dfsg.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-throttle-debounce/jquery-throttle-debounce_1.1+dfsg.1-1.dsc' jquery-throttle-debounce_1.1+dfsg.1-1.dsc 2073 SHA256:b758eb8a8e5d4ade98bef3ed697b488653b197e3817b02f8b2a6ee908f954018
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-throttle-debounce/jquery-throttle-debounce_1.1+dfsg.1.orig.tar.gz' jquery-throttle-debounce_1.1+dfsg.1.orig.tar.gz 16990 SHA256:8e8e935ca82eb33d0ca1956a989bd5c0a789c9715ee700aeba80c4dc952a8665
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-throttle-debounce/jquery-throttle-debounce_1.1+dfsg.1-1.debian.tar.xz' jquery-throttle-debounce_1.1+dfsg.1-1.debian.tar.xz 4476 SHA256:9c5031db2d1d60df7b14cf0a3e5fd235e092169768a69070b0ea6fec02943894
```

### `dpkg` source package: `jquery=3.2.1-1`

Binary Packages:

- `libjs-jquery=3.2.1-1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris jquery=3.2.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jquery/jquery_3.2.1-1.dsc' jquery_3.2.1-1.dsc 2066 SHA256:b529818a547bc3f1ca70743b75e4772199e1ef61f3cc67366de25cc4e112410a
'http://archive.ubuntu.com/ubuntu/pool/main/j/jquery/jquery_3.2.1.orig.tar.xz' jquery_3.2.1.orig.tar.xz 298688 SHA256:3b645c4dcea9b22ee7ed09c6f391a1b5d23f7556cf0ae8f3afd43002491a597d
'http://archive.ubuntu.com/ubuntu/pool/main/j/jquery/jquery_3.2.1-1.debian.tar.xz' jquery_3.2.1-1.debian.tar.xz 9068 SHA256:f4c84ab960c21ecd46aa694a5abc397e84178e7185e78a1f546d064ed65d9ab5
```

### `dpkg` source package: `keyutils=1.5.9-9.2ubuntu2`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-9.2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-9.2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-9.2ubuntu2.dsc' keyutils_1.5.9-9.2ubuntu2.dsc 2237 SHA256:67cb7c4b1dadc2c0ca85286ef8f11f7e71f91b67d47fca58ecd41e1bd83271ad
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-9.2ubuntu2.debian.tar.xz' keyutils_1.5.9-9.2ubuntu2.debian.tar.xz 18492 SHA256:51706bd0d480913584d3fa8fcfe32dcf210742bb75c08e6a2d5f022748654086
```

### `dpkg` source package: `krb5=1.16-2ubuntu0.1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.16-2ubuntu0.1`
- `libk5crypto3:amd64=1.16-2ubuntu0.1`
- `libkrb5-3:amd64=1.16-2ubuntu0.1`
- `libkrb5support0:amd64=1.16-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.16-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.1.dsc' krb5_1.16-2ubuntu0.1.dsc 3563 SHA256:2c955da3464e506961ee80a769bd5139b2df6770ed51947a510f48f451be70c0
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16.orig.tar.gz' krb5_1.16.orig.tar.gz 9474479 SHA256:faeb125f83b0fb4cdb2f99f088140631bb47d975982de0956d18c85842969e08
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.1.debian.tar.xz' krb5_1.16-2ubuntu0.1.debian.tar.xz 99820 SHA256:9e3a973805af340fab23cd28737187567214adb98452d1564ada05652036fc0c
```

### `dpkg` source package: `lapack=3.7.1-4ubuntu1`

Binary Packages:

- `libblas3:amd64=3.7.1-4ubuntu1`
- `liblapack3:amd64=3.7.1-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.7.1-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.7.1-4ubuntu1.dsc' lapack_3.7.1-4ubuntu1.dsc 2920 SHA256:e33bcdea935109083a85442f1826cb4fef865c7e56fb5b38e75a08a8defc3fcd
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.7.1.orig.tar.gz' lapack_3.7.1.orig.tar.gz 9137261 SHA256:f6c53fd9f56932f3ddb3d5e24c1c07e4cd9b3b08e7f89de9c867125eecc9a1c8
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.7.1-4ubuntu1.debian.tar.xz' lapack_3.7.1-4ubuntu1.debian.tar.xz 20956 SHA256:0b981a911d7a8cde6b1addd3d823be88d29807f50c19e71e1a8a233e469c3a6d
```

### `dpkg` source package: `lark-parser=0.7.2-1osrf~bionic`

Binary Packages:

- `python3-lark-parser=0.7.2-1osrf~bionic`

Licenses: (parsed from: `/usr/share/doc/python3-lark-parser/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libarchive=3.2.2-3.1ubuntu0.6`

Binary Packages:

- `libarchive13:amd64=3.2.2-3.1ubuntu0.6`

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
$ apt-get source -qq --print-uris libarchive=3.2.2-3.1ubuntu0.6
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.2.2-3.1ubuntu0.6.dsc' libarchive_3.2.2-3.1ubuntu0.6.dsc 2457 SHA256:1314853f1d1e7ce909f8ed415df42793a0d78998419aae96ae472e0b4c05ba75
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.2.2.orig.tar.gz' libarchive_3.2.2.orig.tar.gz 5458241 SHA256:691c194ee132d1f0f7a42541f091db811bc2e56f7107e9121be2bc8c04f1060f
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.2.2-3.1ubuntu0.6.debian.tar.xz' libarchive_3.2.2-3.1ubuntu0.6.debian.tar.xz 24980 SHA256:535a31e44b43ef1cd1e6ac4b9c3e7ad484d2f326dffad64ee18347df45b505fc
```

### `dpkg` source package: `libassuan=2.5.1-2`

Binary Packages:

- `libassuan-dev=2.5.1-2`
- `libassuan0:amd64=2.5.1-2`

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
$ apt-get source -qq --print-uris libassuan=2.5.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1-2.dsc' libassuan_2.5.1-2.dsc 2215 SHA256:e954a7ef30815e62832ca4a1d2959142e264795e7ec78ba369752353135beb68
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1.orig.tar.bz2' libassuan_2.5.1.orig.tar.bz2 564857 SHA256:47f96c37b4f2aac289f0bc1bacfa8bd8b4b209a488d3d15e2229cb6cc9b26449
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1-2.debian.tar.xz' libassuan_2.5.1-2.debian.tar.xz 15236 SHA256:4a67901dcb0e92cd40e0d5d7148ebe6f929378671df373eb68b48acb560d641f
```

### `dpkg` source package: `libcap-ng=0.7.7-3.1`

Binary Packages:

- `libcap-ng0:amd64=0.7.7-3.1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.7-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.1.dsc' libcap-ng_0.7.7-3.1.dsc 2266 SHA256:f545d107ed3e6160b16aac09e242d1ccc054bfca76f6d70731a83c031b416f53
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7.orig.tar.gz' libcap-ng_0.7.7.orig.tar.gz 420178 SHA256:615549ce39b333f6b78baee0c0b4ef18bc726c6bf1cca123dfd89dd963f6d06b
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.1.debian.tar.xz' libcap-ng_0.7.7-3.1.debian.tar.xz 5432 SHA256:074bf729c3081af729e7e0fbbe3354ddecc16e045245e7d4f44003b9f1f1adc6
```

### `dpkg` source package: `liberror-perl=0.17025-1`

Binary Packages:

- `liberror-perl=0.17025-1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17025-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17025-1.dsc' liberror-perl_0.17025-1.dsc 2077 SHA256:994800c0123fe452ca1f1019e5bf71755c3200231d84999a31dd19be16ada41b
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17025.orig.tar.gz' liberror-perl_0.17025.orig.tar.gz 32013 SHA256:6c9f474ad3d4fe0cabff6b6be532cb1dd348245986d4a6b600ad921d5cfdefaf
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17025-1.debian.tar.xz' liberror-perl_0.17025-1.debian.tar.xz 4108 SHA256:0288dcf7eeff5cddfaf8c6bdfbe9fc170a1d333bb6d88489ca8158c929a44f76
```

### `dpkg` source package: `libfabric=1.5.3-1`

Binary Packages:

- `libfabric1=1.5.3-1`

Licenses: (parsed from: `/usr/share/doc/libfabric1/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libfabric=1.5.3-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libf/libfabric/libfabric_1.5.3-1.dsc' libfabric_1.5.3-1.dsc 2143 SHA256:4dcd9d9a757fa4a0896ee2072a0339c3402e6b1e3243d3ed85b93b63ff76a827
'http://archive.ubuntu.com/ubuntu/pool/universe/libf/libfabric/libfabric_1.5.3.orig.tar.xz' libfabric_1.5.3.orig.tar.xz 930228 SHA256:68bf2b4e465ff08a0403175553d535dccee39d6597f2b0a4619b43c522c29128
'http://archive.ubuntu.com/ubuntu/pool/universe/libf/libfabric/libfabric_1.5.3-1.debian.tar.xz' libfabric_1.5.3-1.debian.tar.xz 8836 SHA256:630681fa87d7dbd91190f42fe39946794e20727f2a35fb51ea108cec5c4d70df
```

### `dpkg` source package: `libffi=3.2.1-8`

Binary Packages:

- `libffi6:amd64=3.2.1-8`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-8
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-8.dsc' libffi_3.2.1-8.dsc 1959 SHA256:a07201eb5374cfab35703a6f4c88a494bb23ece91da5481497bc25404c57eaf4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-8.debian.tar.xz' libffi_3.2.1-8.debian.tar.xz 11660 SHA256:1eb0b13e0c0fc989ed98011d18dcddf8a05af17380fe1258883761a8d16586b4
```

### `dpkg` source package: `libgcrypt20=1.8.1-4ubuntu1.2`

Binary Packages:

- `libgcrypt20:amd64=1.8.1-4ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.1-4ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.dsc' libgcrypt20_1.8.1-4ubuntu1.2.dsc 3035 SHA256:2033925196ff659631496ea66d2feea91112512ab36fcefbcac84fb98b8523dc
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2' libgcrypt20_1.8.1.orig.tar.bz2 2967344 SHA256:7a2875f8b1ae0301732e878c0cca2c9664ff09ef71408f085c50e332656a78b3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2.asc' libgcrypt20_1.8.1.orig.tar.bz2.asc 310 SHA256:9e08f467824855084594a14c4a0455963dac9a359d543e8c2a91ca3498ad031b
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz' libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz 33112 SHA256:e1b2d8ea9bb06c9370bf76934be994458f596162bfaac27061c9047a2ac45c25
```

### `dpkg` source package: `libgpg-error=1.27-6`

Binary Packages:

- `libgpg-error-dev=1.27-6`
- `libgpg-error0:amd64=1.27-6`

Licenses: (parsed from: `/usr/share/doc/libgpg-error-dev/copyright`, `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.27-6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27-6.dsc' libgpg-error_1.27-6.dsc 2343 SHA256:d4cc2c1691b295f558d5b347df8a8ad2f0260cf57146180bed223b94ffacafbb
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27.orig.tar.bz2' libgpg-error_1.27.orig.tar.bz2 813060 SHA256:4f93aac6fecb7da2b92871bb9ee33032be6a87b174f54abf8ddf0911a22d29d2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27-6.debian.tar.xz' libgpg-error_1.27-6.debian.tar.xz 20556 SHA256:89bc57dc3df449febf037226daf1aee830455c4efa493c0e3bdeab2a48971479
```

### `dpkg` source package: `libidn2=2.0.4-1.1ubuntu0.2`

Binary Packages:

- `libidn2-0:amd64=2.0.4-1.1ubuntu0.2`

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
$ apt-get source -qq --print-uris libidn2=2.0.4-1.1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.dsc' libidn2_2.0.4-1.1ubuntu0.2.dsc 2391 SHA256:013191e4a413de9928b5f76b2ab7237055d2e51ed1f82c7bd5ddddff6615d7c8
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4.orig.tar.gz' libidn2_2.0.4.orig.tar.gz 2008524 SHA256:644b6b03b285fb0ace02d241d59483d98bc462729d8bb3608d5cad5532f3d2f0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz' libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz 10290460 SHA256:45c587e0bf489b0367a7a1c2eadbd2efcc774c035ef4868c95ea5b0e0f399be2
```

### `dpkg` source package: `libjs-jquery-hotkeys=0~20130707+git2d51e3a9+dfsg-2ubuntu1`

Binary Packages:

- `libjs-jquery-hotkeys=0~20130707+git2d51e3a9+dfsg-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-hotkeys/copyright`)

- `GPL-2`
- `MIT-or-GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libjs-jquery-hotkeys=0~20130707+git2d51e3a9+dfsg-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-hotkeys/libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg-2ubuntu1.dsc' libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg-2ubuntu1.dsc 1658 SHA256:067bec0c8b142a5ccd85993be6eed75b3a3b8270caf60cf99bde9463c94bc158
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-hotkeys/libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg.orig.tar.xz' libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg.orig.tar.xz 8604 SHA256:d4821b5255baf3156f0affaf7b37eb4d7ffded0cad8addcdb4805f73df6e6e26
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-hotkeys/libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg-2ubuntu1.debian.tar.gz' libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg-2ubuntu1.debian.tar.gz 4768 SHA256:4967ea87d31b6d83486aaf27708c45665ba6cc99158af0bb202593e4da5fd38c
```

### `dpkg` source package: `libjs-jquery-isonscreen=1.2.0-1`

Binary Packages:

- `libjs-jquery-isonscreen=1.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-isonscreen/copyright`)

- `GPL-2`
- `MIT-or-GPL`

Source:

```console
$ apt-get source -qq --print-uris libjs-jquery-isonscreen=1.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-isonscreen/libjs-jquery-isonscreen_1.2.0-1.dsc' libjs-jquery-isonscreen_1.2.0-1.dsc 1460 SHA256:ac0729c251147f96d9899105fe1bbfcc796e0b95df166cd2d09b3596d0f24d1e
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-isonscreen/libjs-jquery-isonscreen_1.2.0.orig.tar.gz' libjs-jquery-isonscreen_1.2.0.orig.tar.gz 727 SHA256:5c0a3ff8d813baa78ac0ef3ccc5cba83001cbbcf9a610324b9af5624e1d19091
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-isonscreen/libjs-jquery-isonscreen_1.2.0-1.debian.tar.gz' libjs-jquery-isonscreen_1.2.0-1.debian.tar.gz 2107 SHA256:ce19ecb03d97223a3c30413529af73d24c6c089327614613ba81b859267d1de6
```

### `dpkg` source package: `libjsoncpp=1.7.4-3`

Binary Packages:

- `libjsoncpp1:amd64=1.7.4-3`

Licenses: (parsed from: `/usr/share/doc/libjsoncpp1/copyright`)

- `Expat_or_PublicDomain_or_DualExpatPD`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libjsoncpp=1.7.4-3
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.4-3.dsc' libjsoncpp_1.7.4-3.dsc 2137 SHA256:8f8d17cb824b288e140988e489b953f7ca084b094a06cc39867a4af1faf1f421
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.4.orig.tar.gz' libjsoncpp_1.7.4.orig.tar.gz 205752 SHA256:10dcd0677e80727e572a1e462193e51a5fde3e023b99e144b2ee1a469835f769
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.4-3.debian.tar.xz' libjsoncpp_1.7.4-3.debian.tar.xz 7828 SHA256:4d99ab057737a02512e75404315ee0b723823f6caed4401c25e46925c4c8857e
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

### `dpkg` source package: `libnl3=3.2.29-0ubuntu3`

Binary Packages:

- `libnl-3-200:amd64=3.2.29-0ubuntu3`
- `libnl-route-3-200:amd64=3.2.29-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libnl-3-200/copyright`, `/usr/share/doc/libnl-route-3-200/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libnl3=3.2.29-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnl3/libnl3_3.2.29-0ubuntu3.dsc' libnl3_3.2.29-0ubuntu3.dsc 3149 SHA256:4b342949deb676eab1475ab10e7ff088ce2bba798fdb87b800b0a821c8ad65e4
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnl3/libnl3_3.2.29.orig.tar.gz' libnl3_3.2.29.orig.tar.gz 963681 SHA256:0beb593dc6abfffa18a5c787b27884979c1b7e7f1fd468c801e3cc938a685922
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnl3/libnl3_3.2.29-0ubuntu3.debian.tar.xz' libnl3_3.2.29-0ubuntu3.debian.tar.xz 20156 SHA256:77b157013f0274525580b17d97b057c1600eda8a256eec07cbd0d2e9cc442d6b
```

### `dpkg` source package: `libpciaccess=0.14-1`

Binary Packages:

- `libpciaccess0:amd64=0.14-1`

Licenses: (parsed from: `/usr/share/doc/libpciaccess0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpciaccess=0.14-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.14-1.dsc' libpciaccess_0.14-1.dsc 2062 SHA256:1cbfd426e4efcc958b6c9fd4889877b533035175370fa0505f361b89e1aeaa4f
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.14.orig.tar.gz' libpciaccess_0.14.orig.tar.gz 461764 SHA256:8d86e64893917be3dfb1c5e837888d1275399c818783474002203d751312b03c
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.14-1.diff.gz' libpciaccess_0.14-1.diff.gz 25039 SHA256:fea9483fbfb202040a8e5eef3ec3b434b3e897f301e735753568db2106e1512d
```

### `dpkg` source package: `libpng1.6=1.6.34-1ubuntu0.18.04.2`

Binary Packages:

- `libpng16-16:amd64=1.6.34-1ubuntu0.18.04.2`

Licenses: (parsed from: `/usr/share/doc/libpng16-16/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `BSD-like-with-advertising-clause`
- `GPL-2`
- `GPL-2+`
- `expat`
- `libpng`
- `libpng OR Apache-2.0 OR BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libpng1.6=1.6.34-1ubuntu0.18.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc' libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc 2362 SHA256:d121cf079c097f868b33f234601baadc6e34d5e96320f427eb3482e28900c321
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34.orig.tar.xz' libpng1.6_1.6.34.orig.tar.xz 997968 SHA256:2f1e960d92ce3b3abd03d06dfec9637dfbd22febf107a536b44f7a47c60659f6
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz' libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz 24572 SHA256:08abc3815a3ce53c46717a3a5c1b2044782c5659639afc9f6f9cb6fdcb386d90
```

### `dpkg` source package: `libpsl=0.19.1-5build1`

Binary Packages:

- `libpsl5:amd64=0.19.1-5build1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.19.1-5build1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1-5build1.dsc' libpsl_0.19.1-5build1.dsc 2229 SHA256:cb9bcc439b8e37ee27bd3e69a8afa6dd2a59c90ba45de4d533df256f61c8a4f5
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1.orig.tar.gz' libpsl_0.19.1.orig.tar.gz 8578385 SHA256:e370181114b8ef9daf2bb6db49b1edb842335839c15a088e7ec0a35e04e9a227
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1-5build1.debian.tar.xz' libpsl_0.19.1-5build1.debian.tar.xz 9860 SHA256:53285bee66ac22a25dd41f7778cc4e94ae3d61929eb6701a8064a38a964e40e2
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3.18.04.3`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3.18.04.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu3.18.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.dsc' libseccomp_2.4.3-1ubuntu3.18.04.3.dsc 1951 SHA256:a21ac1a2c77ed23af125630a6fe63035e35cd8312d5023efdb5c9434c2d3d30e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA256:cf15d1421997fac45b936515af61d209c4fd788af11005d212b3d0fd71e7991d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz 27652 SHA256:9110a31f32f7c63318f75c09493c021e454fa46d7bb0ccca4b0874610c85a71c
```

### `dpkg` source package: `libselinux=2.7-2build2`

Binary Packages:

- `libselinux1:amd64=2.7-2build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.7-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7-2build2.dsc' libselinux_2.7-2build2.dsc 2468 SHA256:86f2d8422230927aa3274773e2b8a9ed15cb539804c378e75515afcd28545c37
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7.orig.tar.gz' libselinux_2.7.orig.tar.gz 187574 SHA256:d0fec0769b3ad60aa7baf9b9a4b7a056827769dc2dadda0dc0eb59b3d1c18c57
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7-2build2.debian.tar.xz' libselinux_2.7-2build2.debian.tar.xz 23176 SHA256:ef7a781c247797b66f4d68907d8dd6fec7188d0a08e2a8541437d5f7f6796105
```

### `dpkg` source package: `libsemanage=2.7-2build2`

Binary Packages:

- `libsemanage-common=2.7-2build2`
- `libsemanage1:amd64=2.7-2build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.7-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7-2build2.dsc' libsemanage_2.7-2build2.dsc 2555 SHA256:4454d11e7228df1e5166907867bbd1be4e6cc8b20c6834dc690fb0dcf19d1c43
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7.orig.tar.gz' libsemanage_2.7.orig.tar.gz 153465 SHA256:07e9477714ce6a4557a1fe924ea4cb06501b62d0fa0e3c0dc32a2cf47cb8d476
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7-2build2.debian.tar.xz' libsemanage_2.7-2build2.debian.tar.xz 17136 SHA256:d6d11ecc5687baa3b07a2a2360a9cbc4b93424a9728aa17b81cd9faf13855c3a
```

### `dpkg` source package: `libsepol=2.7-1`

Binary Packages:

- `libsepol1:amd64=2.7-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7-1.dsc' libsepol_2.7-1.dsc 1814 SHA256:7de809477acd60d256eca160d5fc6986e5e65227706b1cdb23f8139bb49d2782
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7.orig.tar.gz' libsepol_2.7.orig.tar.gz 471147 SHA256:d69d3bd8ec901a3bd5adf2be2fb47fb1a685ed73066ab482e7e505371a48f9e7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7-1.debian.tar.xz' libsepol_2.7-1.debian.tar.xz 13944 SHA256:56b1c2b0e492b2089f23a0d7a95a260377a0e3adefc60e90c0ff6eff6be08450
```

### `dpkg` source package: `libtasn1-6=4.13-2`

Binary Packages:

- `libtasn1-6:amd64=4.13-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.13-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13-2.dsc' libtasn1-6_4.13-2.dsc 2574 SHA256:8f583c0ae8568ccf7fcf66c387963ef949d644cfca56d66512a17cb91c3a44fd
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz' libtasn1-6_4.13.orig.tar.gz 1891703 SHA256:7e528e8c317ddd156230c4e31d082cd13e7ddeb7a54824be82632209550c8cca
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz.asc' libtasn1-6_4.13.orig.tar.gz.asc 774 SHA256:90261376528edf44831d1369847088cc2fb48669860d343961daca42e674b226
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13-2.debian.tar.xz' libtasn1-6_4.13-2.debian.tar.xz 63332 SHA256:f36a43fb898c031b6b1a5f43b35af1aea95ac164bb2b57c7f07d1c098ed9f7eb
```

### `dpkg` source package: `libtool=2.4.6-2`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-2`
- `libltdl7:amd64=2.4.6-2`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-2.dsc' libtool_2.4.6-2.dsc 2324 SHA256:caa2b9d5c32e491388d0627e2f808b6cb2f260dd1b0b9fdafc9bff957f05bb29
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-2.debian.tar.xz' libtool_2.4.6-2.debian.tar.xz 36024 SHA256:6227fb1240a90ef06855567e71ee96e4950dd53c4399348f36c1ec39367cd8ea
```

### `dpkg` source package: `libunistring=0.9.9-0ubuntu2`

Binary Packages:

- `libunistring2:amd64=0.9.9-0ubuntu2`

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
$ apt-get source -qq --print-uris libunistring=0.9.9-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.dsc' libunistring_0.9.9-0ubuntu2.dsc 2006 SHA256:b2c297bb30b94a8b4435bb749f0f65564376049fbaf262e9689435217d55a38b
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9.orig.tar.xz' libunistring_0.9.9.orig.tar.xz 2042992 SHA256:a4d993ecfce16cf503ff7579f5da64619cee66226fb3b998dafb706190d9a833
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.debian.tar.xz' libunistring_0.9.9-0ubuntu2.debian.tar.xz 40424 SHA256:cb7a56608d98804e4dc83e1cae6035ef6b89e18f3dcbcd44afb16e32313ed4ba
```

### `dpkg` source package: `libuv1=1.18.0-3`

Binary Packages:

- `libuv1:amd64=1.18.0-3`

Licenses: (parsed from: `/usr/share/doc/libuv1/copyright`)

- `BSD-1-clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris libuv1=1.18.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.18.0-3.dsc' libuv1_1.18.0-3.dsc 2053 SHA256:92f4dfae07b870fc4190fcc5bf53edf963ee978b9f9dbc999ad169c9679482da
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.18.0.orig.tar.gz' libuv1_1.18.0.orig.tar.gz 1167975 SHA256:0b9aef32e63619c328b65d85583653e295ca091cf9b15315c3c518e02a59c17c
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.18.0-3.debian.tar.xz' libuv1_1.18.0-3.debian.tar.xz 12380 SHA256:9ae1087c696cc2612f406eb0041264aaa9c36efa4cbfb5026dbaf7d9f4626b0a
```

### `dpkg` source package: `libxml2=2.9.4+dfsg1-6.1ubuntu1.3`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-6.1ubuntu1.3`
- `libxml2-utils=2.9.4+dfsg1-6.1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-utils/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.4+dfsg1-6.1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc 3151 SHA256:dd8d75ce7c2e568642ffd8a84ce7d8d6372babc32ee726884a539d5d24698169
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA256:a74ad55e346aa0b2b41903e66d21f8f3d2a736b3f41e32496376861ab484184e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz 39680 SHA256:f746e94d2dd252b2e605f2d2fb265b7e788f6fadd45e76588928e2b889349917
```

### `dpkg` source package: `libxslt=1.1.29-5ubuntu0.2`

Binary Packages:

- `libxslt1.1:amd64=1.1.29-5ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.29-5ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.dsc' libxslt_1.1.29-5ubuntu0.2.dsc 2502 SHA256:2b8253a9387cf6dfd96696fa39c1a228249d9463293f33536a5cf5978c96d259
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29.orig.tar.gz' libxslt_1.1.29.orig.tar.gz 3428524 SHA256:b5976e3857837e7617b29f2249ebb5eeac34e249208d31f1fbf7a6ba7a4090ce
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.debian.tar.xz' libxslt_1.1.29-5ubuntu0.2.debian.tar.xz 36520 SHA256:d6fcf48ac5c8a6e8af41c57dba2add6a8d608939370210c9a1d0d888f5088863
```

### `dpkg` source package: `libyaml=0.1.7-2ubuntu3`

Binary Packages:

- `libyaml-0-2:amd64=0.1.7-2ubuntu3`
- `libyaml-dev:amd64=0.1.7-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.1.7-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.7-2ubuntu3.dsc' libyaml_0.1.7-2ubuntu3.dsc 2019 SHA256:122f3c4ddc6b6f069382587fdde2ba9ed4800b303bce92c3d11d4fee1c1c0c5c
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.7.orig.tar.gz' libyaml_0.1.7.orig.tar.gz 527518 SHA256:8088e457264a98ba451a90b8661fcb4f9d6f478f7265d48322a196cec2480729
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.7-2ubuntu3.debian.tar.xz' libyaml_0.1.7-2ubuntu3.debian.tar.xz 4288 SHA256:d1b9caa9e645c2c306417068bcdd85e56e6065d74771c15cc970652e52f8259b
```

### `dpkg` source package: `libzstd=1.3.3+dfsg-2ubuntu1.1`

Binary Packages:

- `libzstd1:amd64=1.3.3+dfsg-2ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause-with-patent-grant`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.3.3+dfsg-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.dsc' libzstd_1.3.3+dfsg-2ubuntu1.1.dsc 2390 SHA256:625d37dcb1b8b26dea3e9b38c9a10db4f4dfa275d889f98dd0f62db3d0e2fa31
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg.orig.tar.xz' libzstd_1.3.3+dfsg.orig.tar.xz 1333584 SHA256:e236191547a0ab53cc52c0207ead0d51305dbe9452b5f34d4ea9eb1f51031a93
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz' libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz 12808 SHA256:9c7421170f0a1e6234147a89ba7fa5933c0771177423e962e6faf3fd13dcbb64
```

### `dpkg` source package: `linux=4.15.0-117.118`

Binary Packages:

- `linux-libc-dev:amd64=4.15.0-117.118`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lksctp-tools=1.0.17+dfsg-2`

Binary Packages:

- `libsctp-dev:amd64=1.0.17+dfsg-2`
- `libsctp1:amd64=1.0.17+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libsctp-dev/copyright`, `/usr/share/doc/libsctp1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris lksctp-tools=1.0.17+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.17+dfsg-2.dsc' lksctp-tools_1.0.17+dfsg-2.dsc 2014 SHA256:f9180a1d047ac7bdb853a000cd4c4f6a53143f2604bd7cd08bc0800a36abd0e7
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.17+dfsg.orig.tar.gz' lksctp-tools_1.0.17+dfsg.orig.tar.gz 556428 SHA256:f7c537bc08bf57a8eddf49b232f19920e51b0e4ca55e7d47377ce64546d04e1d
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.17+dfsg-2.debian.tar.xz' lksctp-tools_1.0.17+dfsg-2.debian.tar.xz 9436 SHA256:c8e05a29ffbca99428cf2c59a50dd26a4bf73f42487db8231b810882a5f5c779
```

### `dpkg` source package: `log4cxx=0.10.0-13ubuntu2`

Binary Packages:

- `liblog4cxx-dev:amd64=0.10.0-13ubuntu2`
- `liblog4cxx10v5:amd64=0.10.0-13ubuntu2`

Licenses: (parsed from: `/usr/share/doc/liblog4cxx-dev/copyright`, `/usr/share/doc/liblog4cxx10v5/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris log4cxx=0.10.0-13ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0-13ubuntu2.dsc' log4cxx_0.10.0-13ubuntu2.dsc 2262 SHA256:79dbfa3b2684e6aaec543e7b4cd23520fc56d351606439127cee8b1b11df933c
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0.orig.tar.gz' log4cxx_0.10.0.orig.tar.gz 1667425 SHA256:0de0396220a9566a580166e66b39674cb40efd2176f52ad2c65486c99c920c8c
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0-13ubuntu2.debian.tar.xz' log4cxx_0.10.0-13ubuntu2.debian.tar.xz 16488 SHA256:4303722b0541512cda99c39212074528fd96aff81f5e4c0b8837eb89adddce05
```

### `dpkg` source package: `lsb=9.20170808ubuntu1`

Binary Packages:

- `lsb-base=9.20170808ubuntu1`
- `lsb-release=9.20170808ubuntu1`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`, `/usr/share/doc/lsb-release/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20170808ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20170808ubuntu1.dsc' lsb_9.20170808ubuntu1.dsc 2126 SHA256:9b98df7b442472d172612bf6855b4dbc3cd6d5892d8073605dda786fec94af5f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20170808ubuntu1.tar.xz' lsb_9.20170808ubuntu1.tar.xz 45492 SHA256:b26bcb746e0bff05ad3e15dfbeb0ba7ea2a8d031f765a6cfa568c57d14c522c4
```

### `dpkg` source package: `lxml=4.2.1-1ubuntu0.1`

Binary Packages:

- `python3-lxml:amd64=4.2.1-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/python3-lxml/copyright`)

- `GPL`
- `GPL2`
- `later`

Source:

```console
$ apt-get source -qq --print-uris lxml=4.2.1-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lxml/lxml_4.2.1-1ubuntu0.1.dsc' lxml_4.2.1-1ubuntu0.1.dsc 2336 SHA256:3c8f63ad63a0f96fbf10dcc80606955cd784775c7a97138bc8875c791718bf49
'http://archive.ubuntu.com/ubuntu/pool/main/l/lxml/lxml_4.2.1.orig.tar.gz' lxml_4.2.1.orig.tar.gz 4284267 SHA256:e2629cdbcad82b83922a3488937632a4983ecc0fed3e5cfbf430d069382eeb9b
'http://archive.ubuntu.com/ubuntu/pool/main/l/lxml/lxml_4.2.1-1ubuntu0.1.debian.tar.xz' lxml_4.2.1-1ubuntu0.1.debian.tar.xz 8320 SHA256:9e95f418a40e4e3c1d713a9aca776a0eef4fca08a43595c1183fd5eb5bee124a
```

### `dpkg` source package: `lz4=0.0~r131-2ubuntu3`

Binary Packages:

- `liblz4-1:amd64=0.0~r131-2ubuntu3`
- `liblz4-dev:amd64=0.0~r131-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`, `/usr/share/doc/liblz4-dev/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=0.0~r131-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu3.dsc' lz4_0.0~r131-2ubuntu3.dsc 2129 SHA256:b6f9a71053ff1414f695790833e689dc8bd4c48169b05a8df8de47edba7a7b58
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131.orig.tar.gz' lz4_0.0~r131.orig.tar.gz 133784 SHA256:9d4d00614d6b9dec3114b33d1224b6262b99ace24434c53487a0c8fd0b18cfed
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu3.debian.tar.xz' lz4_0.0~r131-2ubuntu3.debian.tar.xz 5340 SHA256:94834bac922397529ffc185f9c4c7e7a6eb1ef3bc527f3fcd26e36fc9430afa7
```

### `dpkg` source package: `lzo2=2.08-1.2`

Binary Packages:

- `liblzo2-2:amd64=2.08-1.2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.08-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.08-1.2.dsc' lzo2_2.08-1.2.dsc 1804 SHA256:09eabe81d6f631a29cc603843b27ab914704726a1400a2219cf83b1da4e72892
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.08.orig.tar.gz' lzo2_2.08.orig.tar.gz 589045 SHA256:ac1b3e4dee46febe9fd28737eb7f5692d3232ef1a01da10444394c3d47536614
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.08-1.2.debian.tar.xz' lzo2_2.08-1.2.debian.tar.xz 5996 SHA256:5a9aa3a2432f5d4f689b24c64ea3daec7646e736da37721388ae88b670dd99bc
```

### `dpkg` source package: `make-dfsg=4.1-9.1ubuntu1`

Binary Packages:

- `make=4.1-9.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.1-9.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-9.1ubuntu1.dsc' make-dfsg_4.1-9.1ubuntu1.dsc 2079 SHA256:d8ca40c89cb2b808b28264b7097a001f00a517a68d5bc2657b5c5e1bbfd0ce8b
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1.orig.tar.gz' make-dfsg_4.1.orig.tar.gz 1350231 SHA256:b3ed04fb6718289e4a430afbe2df6ecba9177aad9f6d09aaf38e5409262ca8a3
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-9.1ubuntu1.diff.gz' make-dfsg_4.1-9.1ubuntu1.diff.gz 46399 SHA256:6adc229835bd4cf04cefab0767534f9e6934989413002dd5525ec557010af5e8
```

### `dpkg` source package: `mawk=1.3.3-17ubuntu3`

Binary Packages:

- `mawk=1.3.3-17ubuntu3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu3.dsc' mawk_1.3.3-17ubuntu3.dsc 1970 SHA256:2893a0c18b75c41d480be67d5d4edb7124ed7e9b5ed643d2670aa34481f7a77c
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu3.diff.gz' mawk_1.3.3-17ubuntu3.diff.gz 64052 SHA256:d1be148525885cb1869e35514f55005b5043f3310b08c444625005a3e14c81fc
```

### `dpkg` source package: `mime-support=3.60ubuntu1`

Binary Packages:

- `mime-support=3.60ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.60ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.60ubuntu1.dsc' mime-support_3.60ubuntu1.dsc 1712 SHA256:1e58e26d0f87f25ebe6c08007e9d354a24457ab73d40a1eb3b9ab62ea0d366d5
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.60ubuntu1.tar.gz' mime-support_3.60ubuntu1.tar.gz 37743 SHA256:cb1bc122ac2dc7046f6c0c06146ac0897a3c1c02e7e5e53cdd30817db2c62d33
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

### `dpkg` source package: `mpdecimal=2.4.2-1ubuntu1`

Binary Packages:

- `libmpdec2:amd64=2.4.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1ubuntu1.dsc' mpdecimal_2.4.2-1ubuntu1.dsc 2051 SHA256:6a1a2c1b839492e178d601dc6b9de26a3173124b35659ccd21362167a4fabda9
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1ubuntu1.debian.tar.xz' mpdecimal_2.4.2-1ubuntu1.debian.tar.xz 5328 SHA256:091414d364411f1d05b496f877e04d8ad22d52441cb698d739929907e94e0fc7
```

### `dpkg` source package: `mpfr4=4.0.1-1`

Binary Packages:

- `libmpfr6:amd64=4.0.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.0.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1-1.dsc' mpfr4_4.0.1-1.dsc 1972 SHA256:85d8dad92d3f9ace96ac78b2f4ec00eafef228fa53e0344ae4255fc4d3f75626
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1.orig.tar.xz' mpfr4_4.0.1.orig.tar.xz 1412692 SHA256:67874a60826303ee2fb6affc6dc0ddd3e749e9bfcb4c8655e3953d0458a6e16e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1-1.debian.tar.xz' mpfr4_4.0.1-1.debian.tar.xz 10460 SHA256:9e0d582dea7e88958b8bc1f3782ada59b9c7175f01b4e06e8487fc6cbfc5a2d7
```

### `dpkg` source package: `mpi-defaults=1.10`

Binary Packages:

- `mpi-default-bin=1.10`
- `mpi-default-dev=1.10`

Licenses: (parsed from: `/usr/share/doc/mpi-default-bin/copyright`, `/usr/share/doc/mpi-default-dev/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpi-defaults=1.10
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mpi-defaults/mpi-defaults_1.10.dsc' mpi-defaults_1.10.dsc 2680 SHA256:fa42bc3bff329ad4b8f028c47f492a7b61d8c63f2467e7e02f043dfe7e9dfb8d
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mpi-defaults/mpi-defaults_1.10.tar.xz' mpi-defaults_1.10.tar.xz 4864 SHA256:ca4410036cc8f63ce7e3205238612b25a32b300b9bce73ec8d5b00738e0902c4
```

### `dpkg` source package: `mysql-5.7=5.7.31-0ubuntu0.18.04.1`

Binary Packages:

- `libmysqlclient-dev=5.7.31-0ubuntu0.18.04.1`
- `libmysqlclient20:amd64=5.7.31-0ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libmysqlclient-dev/copyright`, `/usr/share/doc/libmysqlclient20/copyright`)

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
- `SWsoft`
- `public-domain`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris mysql-5.7=5.7.31-0ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.31-0ubuntu0.18.04.1.dsc' mysql-5.7_5.7.31-0ubuntu0.18.04.1.dsc 3446 SHA256:55560786c7397d034b77ad2bbeeef9f08b3c3be5ca3f2244a093c3da96d14a1e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.31.orig.tar.gz' mysql-5.7_5.7.31.orig.tar.gz 51382559 SHA256:85bd222e61846313d7ad7c095ad664c89ca8f52dd9c21b7ac343ead62d701200
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.31-0ubuntu0.18.04.1.debian.tar.xz' mysql-5.7_5.7.31-0ubuntu0.18.04.1.debian.tar.xz 156460 SHA256:05bcfcfbe054ac9b645212dabb7329328e6513b758f46ff3192b19370b81f54b
```

### `dpkg` source package: `mysql-defaults=1.0.4`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.4`
- `mysql-common=5.8+1.0.4`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.4.dsc' mysql-defaults_1.0.4.dsc 2213 SHA256:c0cb0ba90874c858c30cfc71ccbd078c1fb1b45fbfdc6414af75811101d6f01f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.4.tar.xz' mysql-defaults_1.0.4.tar.xz 7084 SHA256:01b92a09aaa08fd589610c0d7cbe55e05dce64db57ff2dfa6f794bcf857e002a
```

### `dpkg` source package: `ncurses=6.1-1ubuntu1.18.04`

Binary Packages:

- `libncurses5:amd64=6.1-1ubuntu1.18.04`
- `libncursesw5:amd64=6.1-1ubuntu1.18.04`
- `libtinfo5:amd64=6.1-1ubuntu1.18.04`
- `ncurses-base=6.1-1ubuntu1.18.04`
- `ncurses-bin=6.1-1ubuntu1.18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1-1ubuntu1.18.04
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.dsc' ncurses_6.1-1ubuntu1.18.04.dsc 4702 SHA256:9ff732e257304efa8ab3e5dba1ee85f6a360866466261c6a19f1a5d45b62d8f7
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz' ncurses_6.1.orig.tar.gz 3365395 SHA256:aa057eeeb4a14d470101eff4597d5833dcef5965331be3528c08d99cebaa0d17
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz.asc' ncurses_6.1.orig.tar.gz.asc 251 SHA256:47fd6ab5c2b08758f9c372c2bb75f2f0dbcd5cf58ae30b08f791a903da0259a4
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.debian.tar.xz' ncurses_6.1-1ubuntu1.18.04.debian.tar.xz 57464 SHA256:5f6822a052024372aa181f32dbe689ba3efd47920b5ffd3bae3c57c07f913983
```

### `dpkg` source package: `netifaces=0.10.4-0.1build4`

Binary Packages:

- `python-netifaces=0.10.4-0.1build4`

Licenses: (parsed from: `/usr/share/doc/python-netifaces/copyright`)

- `MIT-style`

Source:

```console
$ apt-get source -qq --print-uris netifaces=0.10.4-0.1build4
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4-0.1build4.dsc' netifaces_0.10.4-0.1build4.dsc 2445 SHA256:f2d0307065fb71ad2859aa356983134dca48cc131ecd9b23973a96012241f8f7
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4.orig.tar.gz' netifaces_0.10.4.orig.tar.gz 22969 SHA256:9656a169cb83da34d732b0eb72b39373d48774aee009a3d1272b7ea2ce109cde
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4-0.1build4.debian.tar.xz' netifaces_0.10.4-0.1build4.debian.tar.xz 8436 SHA256:516521d6ac087265a5a40225f36ffdc969a15f715eed0ecdf80a1039c9eb5835
```

### `dpkg` source package: `nettle=3.4-1`

Binary Packages:

- `libhogweed4:amd64=3.4-1`
- `libnettle6:amd64=3.4-1`

Licenses: (parsed from: `/usr/share/doc/libhogweed4/copyright`, `/usr/share/doc/libnettle6/copyright`)

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
$ apt-get source -qq --print-uris nettle=3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4-1.dsc' nettle_3.4-1.dsc 2238 SHA256:0ceb4600fdedf43916e95fb6b354ebb4038f00f5814433582d0481b510310e86
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.orig.tar.gz' nettle_3.4.orig.tar.gz 1935069 SHA256:ae7a42df026550b85daca8389b6a60ba6313b0567f374392e54918588a411e94
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.orig.tar.gz.asc' nettle_3.4.orig.tar.gz.asc 1238 SHA256:86d7441c7334dd95d16b1ca488fd94ec45ed6406714d4ed9887c7212e337eb2a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4-1.debian.tar.xz' nettle_3.4-1.debian.tar.xz 19884 SHA256:9bfc25562ed36449e75741b0473e0e558bc9ef5c20ca24e7c650fea87d631c03
```

### `dpkg` source package: `nghttp2=1.30.0-1ubuntu1`

Binary Packages:

- `libnghttp2-14:amd64=1.30.0-1ubuntu1`

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
$ apt-get source -qq --print-uris nghttp2=1.30.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0-1ubuntu1.dsc' nghttp2_1.30.0-1ubuntu1.dsc 2674 SHA256:1848fdc28933b7ee23dbebe3c9dcd0ca9182f95a278d627758d5ccfa2e0b44ad
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0.orig.tar.bz2' nghttp2_1.30.0.orig.tar.bz2 1839714 SHA256:f66918dd03773f4847da1d069295c758ce478cbd1fe58298a37d65e1dce056d8
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0-1ubuntu1.debian.tar.xz' nghttp2_1.30.0-1ubuntu1.debian.tar.xz 13244 SHA256:eb99f2c10cd872ce750964fc59734aa70b89ad04179291a23bfbee0e1a2903d3
```

### `dpkg` source package: `nose2=0.7.4-1`

Binary Packages:

- `python3-nose2=0.7.4-1`

Licenses: (parsed from: `/usr/share/doc/python3-nose2/copyright`)

- `BSD-2-clause`
- `Python`

Source:

```console
$ apt-get source -qq --print-uris nose2=0.7.4-1
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose2/nose2_0.7.4-1.dsc' nose2_0.7.4-1.dsc 2344 SHA256:7dcef699568ce5a67a6c98b7e7aadcd9232d2ccfd076fab98d57557036eed999
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose2/nose2_0.7.4.orig.tar.gz' nose2_0.7.4.orig.tar.gz 141719 SHA256:954a62cfb2d2ac06dad32995cbc822bf00cc11e20d543963515932fd4eff33fa
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose2/nose2_0.7.4-1.debian.tar.xz' nose2_0.7.4-1.debian.tar.xz 7428 SHA256:976994933f573c25f856054b921f4837e0fdf93ffd29ab2a2c35b47d4b50b04d
```

### `dpkg` source package: `nose=1.3.7-3`

Binary Packages:

- `python-nose=1.3.7-3`

Licenses: (parsed from: `/usr/share/doc/python-nose/copyright`)

- `Expat`
- `LGPL`
- `LGPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nose=1.3.7-3
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose/nose_1.3.7-3.dsc' nose_1.3.7-3.dsc 2334 SHA256:0b50c376c21270ec857fcf28516f49d250d5ddb4db4f93a2181687bba3d776ff
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose/nose_1.3.7.orig.tar.gz' nose_1.3.7.orig.tar.gz 280488 SHA256:f1bffef9cbc82628f6e7d7b40d7e255aefaa1adb6a1b1d26c69a8b79e6208a98
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose/nose_1.3.7-3.debian.tar.xz' nose_1.3.7-3.debian.tar.xz 12080 SHA256:5e1f6fa1ce29d8a4ad6315544d5d7db634be5233ec9900e21540b890b5058338
```

### `dpkg` source package: `npth=1.5-3`

Binary Packages:

- `libnpth0:amd64=1.5-3`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.5-3
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5-3.dsc' npth_1.5-3.dsc 1954 SHA256:98e02623d39451685321ab638e12cd0b85f7829f6b174d03dbb806b8d899ae3f
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5.orig.tar.bz2' npth_1.5.orig.tar.bz2 299308 SHA256:294a690c1f537b92ed829d867bee537e46be93fbd60b16c04630fbbfcd9db3c2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5-3.debian.tar.xz' npth_1.5-3.debian.tar.xz 10480 SHA256:5cbaf91c95c90ab82053110eeec5ac72f5a3cab36829edb0579f1fb759ec5fec
```

### `dpkg` source package: `numactl=2.0.11-2.1ubuntu0.1`

Binary Packages:

- `libnuma-dev:amd64=2.0.11-2.1ubuntu0.1`
- `libnuma1:amd64=2.0.11-2.1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libnuma-dev/copyright`, `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.11-2.1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-2.1ubuntu0.1.dsc' numactl_2.0.11-2.1ubuntu0.1.dsc 1970 SHA256:57656dc476766ef49640d83ea3a8e7566d1e467f9d90e7f284e57df0cffd442a
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11.orig.tar.gz' numactl_2.0.11.orig.tar.gz 408175 SHA256:450c091235f891ee874a8651b179c30f57a1391ca5c4673354740ba65e527861
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-2.1ubuntu0.1.debian.tar.xz' numactl_2.0.11-2.1ubuntu0.1.debian.tar.xz 9504 SHA256:f212b9699986291b474d1ae99eaa96f48e9845d0dde5aa2430a1b8e50e201b11
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

### `dpkg` source package: `openldap=2.4.45+dfsg-1ubuntu1.6`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.45+dfsg-1ubuntu1.6`
- `libldap-common=2.4.45+dfsg-1ubuntu1.6`
- `libldap2-dev:amd64=2.4.45+dfsg-1ubuntu1.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.45+dfsg-1ubuntu1.6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg-1ubuntu1.6.dsc' openldap_2.4.45+dfsg-1ubuntu1.6.dsc 2884 SHA256:7f7b47c9ca3e1e61c7e1955813148f4f127e9c29e96efcb22b797fded2282630
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg.orig.tar.gz' openldap_2.4.45+dfsg.orig.tar.gz 4846458 SHA256:d51c70423aa0554d454fd3d43e7f2e940523b4ef07979305b48c233ae44b2b32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg-1ubuntu1.6.debian.tar.xz' openldap_2.4.45+dfsg-1ubuntu1.6.debian.tar.xz 179188 SHA256:959cf67aceadf0af09caf85615d61161df4b91ef9ff2153ea420ae7eec8b9f2d
```

### `dpkg` source package: `openmpi=2.1.1-8`

Binary Packages:

- `libopenmpi-dev=2.1.1-8`
- `libopenmpi2:amd64=2.1.1-8`
- `openmpi-bin=2.1.1-8`
- `openmpi-common=2.1.1-8`

Licenses: (parsed from: `/usr/share/doc/libopenmpi-dev/copyright`, `/usr/share/doc/libopenmpi2/copyright`, `/usr/share/doc/openmpi-bin/copyright`, `/usr/share/doc/openmpi-common/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris openmpi=2.1.1-8
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_2.1.1-8.dsc' openmpi_2.1.1-8.dsc 2618 SHA256:2133456247dc953bf4c5d5c4cbeb8727498b11be044a0c96d7d470f2ebaa6339
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_2.1.1.orig.tar.xz' openmpi_2.1.1.orig.tar.xz 5419544 SHA256:0a64746082725ee25f36b79956da30297dd18d4d27b38ab5b74e2faad694574b
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_2.1.1-8.debian.tar.xz' openmpi_2.1.1-8.debian.tar.xz 60008 SHA256:33ee9c1ebc8c5c5a8c60faa25efbcc8abfea101331b9318abae2e3a458fc937f
```

### `dpkg` source package: `openssl=1.1.1-1ubuntu2.1~18.04.6`

Binary Packages:

- `libssl-dev:amd64=1.1.1-1ubuntu2.1~18.04.6`
- `libssl1.1:amd64=1.1.1-1ubuntu2.1~18.04.6`
- `openssl=1.1.1-1ubuntu2.1~18.04.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1-1ubuntu2.1~18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.dsc' openssl_1.1.1-1ubuntu2.1~18.04.6.dsc 2754 SHA256:e35516df9f2b2798065730bbc87f1b5a6b87ff4716f5ae2d3ed4a2ce32f7029f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz' openssl_1.1.1.orig.tar.gz 8337920 SHA256:2836875a0f89c03d0fdf483941512613a50cfb421d6fd94b9f41d7279d586a3d
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz.asc' openssl_1.1.1.orig.tar.gz.asc 488 SHA256:f3296150114069ea73a72eafbfdcbb295b770e7cbf3266f9590f3d0932498b3e
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz' openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz 104692 SHA256:8251b6f87af26364a341f7beeeef26ed99c7f90819804dba3c1e6bf2f698bb99
```

### `dpkg` source package: `p11-kit=0.23.9-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.9-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9-2.dsc' p11-kit_0.23.9-2.dsc 2458 SHA256:e4c271a89abf52a95d23cca02bd6fb6ea5d5611b139ac63b0db728e7d9895449
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9.orig.tar.gz' p11-kit_0.23.9.orig.tar.gz 1091561 SHA256:e1c1649c335107a8d33cf3762eb7f57b2d0681f0c7d8353627293a58d6b4db63
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9.orig.tar.gz.asc' p11-kit_0.23.9.orig.tar.gz.asc 900 SHA256:334562f6a37f96339173a33a90b246466e0b2673e03658b205d75ebbb63bad10
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9-2.debian.tar.xz' p11-kit_0.23.9-2.debian.tar.xz 21704 SHA256:fa6af69f96f6ccdce95d61e39662a38768b05f8872b2b2008d56cc4fff0ed3fd
```

### `dpkg` source package: `pam=1.1.8-3.6ubuntu2.18.04.2`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.6ubuntu2.18.04.2`
- `libpam-modules-bin=1.1.8-3.6ubuntu2.18.04.2`
- `libpam-runtime=1.1.8-3.6ubuntu2.18.04.2`
- `libpam0g:amd64=1.1.8-3.6ubuntu2.18.04.2`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.6ubuntu2.18.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.1.8-3.6ubuntu2.18.04.2.dsc' pam_1.1.8-3.6ubuntu2.18.04.2.dsc 2557 SHA256:5c46f04306f829f2226773f206d598fcca0e982585c62b48dcda683912dfd662
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.1.8-3.6ubuntu2.18.04.2.tar.gz' pam_1.1.8-3.6ubuntu2.18.04.2.tar.gz 1991026 SHA256:fbd0f113c84beeb8cea5a09e0ad8672e79a12519cd53510389591f915fdcdeef
```

### `dpkg` source package: `paramiko=2.0.0-1ubuntu1.2`

Binary Packages:

- `python-paramiko=2.0.0-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/python-paramiko/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris paramiko=2.0.0-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_2.0.0-1ubuntu1.2.dsc' paramiko_2.0.0-1ubuntu1.2.dsc 2511 SHA256:ac7f549d431683b6c3464e855bd9f9794d1b89d919157b4372e712fdd95b80d3
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_2.0.0.orig.tar.gz' paramiko_2.0.0.orig.tar.gz 273791 SHA256:acf3866621794d68ce42bd5bcb769b6f9ff7e362cc1064e1b1af4185cdc4ed3b
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_2.0.0-1ubuntu1.2.debian.tar.xz' paramiko_2.0.0-1ubuntu1.2.debian.tar.xz 12624 SHA256:b9f85f391a3499a860e7e19bc666750327494a1c929514f8b7e15fbed415b543
```

### `dpkg` source package: `patch=2.7.6-2ubuntu1.1`

Binary Packages:

- `patch=2.7.6-2ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-2ubuntu1.1.dsc' patch_2.7.6-2ubuntu1.1.dsc 1798 SHA256:4c7196107cc0c9a6ec1f8d1da109b8b459e97ad73afd4431eef5cd5f155820b5
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-2ubuntu1.1.debian.tar.xz' patch_2.7.6-2ubuntu1.1.debian.tar.xz 12356 SHA256:23ce948efcf40acc3b25fd97e79a299044d66602db01e5f80c6fd5881cc77b54
```

### `dpkg` source package: `pcre3=2:8.39-9`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-9`
- `libpcre3:amd64=2:8.39-9`
- `libpcre3-dev:amd64=2:8.39-9`
- `libpcre32-3:amd64=2:8.39-9`
- `libpcrecpp0v5:amd64=2:8.39-9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-9
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-9.dsc' pcre3_8.39-9.dsc 2224 SHA256:cfbe37b2022027f62f236d74bb6af90befd2964161d77b2fd459c75ae7c36e36
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-9.debian.tar.gz' pcre3_8.39-9.debian.tar.gz 26333 SHA256:68be90799b722a8d5a075c3d2f48718cb21e2e736e0edf1e7e46a87c51215f55
```

### `dpkg` source package: `perl=5.26.1-6ubuntu0.3`

Binary Packages:

- `libperl5.26:amd64=5.26.1-6ubuntu0.3`
- `perl=5.26.1-6ubuntu0.3`
- `perl-base=5.26.1-6ubuntu0.3`
- `perl-modules-5.26=5.26.1-6ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/libperl5.26/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.26/copyright`)

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
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.26.1-6ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1-6ubuntu0.3.dsc' perl_5.26.1-6ubuntu0.3.dsc 2768 SHA256:76badc610c519409d121d4c9b965614a798f6a681d8427d5a63a898ef3f963e8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1.orig-regen-configure.tar.gz' perl_5.26.1.orig-regen-configure.tar.gz 712883 SHA256:918f054a64b2835bc1c6ed79c1e082e7dcdb76735a95b54ee39c25ea9e245ca4
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1.orig.tar.xz' perl_5.26.1.orig.tar.xz 11922848 SHA256:fe8208133e73e47afc3251c08d2c21c5a60160165a8ab8b669c43a420e4ec680
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1-6ubuntu0.3.debian.tar.xz' perl_5.26.1-6ubuntu0.3.debian.tar.xz 174240 SHA256:9f509fc771c8b46cea480cf464f4ddb83bd33160673607a02431e42a7fba9d61
```

### `dpkg` source package: `pinentry=1.1.0-1`

Binary Packages:

- `pinentry-curses=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-1.dsc' pinentry_1.1.0-1.dsc 2910 SHA256:8cda3442923c0e18f9c3d5a2817a97a54db7447046b9c469e890abd19c680247
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2.asc' pinentry_1.1.0.orig.tar.bz2.asc 534 SHA256:0e3a7633b9fddf9c01c3dcf74aeb94888cc6d5d233f0b8357b0b9c1a1fed9a73
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-1.debian.tar.xz' pinentry_1.1.0-1.debian.tar.xz 15408 SHA256:ddee92638e762f125ac09b86b4f3b31e2d240e8d2dcce940302293bb2ea0873e
```

### `dpkg` source package: `pkg-config=0.29.1-0ubuntu2`

Binary Packages:

- `pkg-config=0.29.1-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.1-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu2.dsc' pkg-config_0.29.1-0ubuntu2.dsc 1824 SHA256:91f07d5a80083fbe86c93d9f107890920f4740df8f3d1e6b162a5d703afc3b89
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1.orig.tar.gz' pkg-config_0.29.1.orig.tar.gz 2013454 SHA256:beb43c9e064555469bd4390dcfd8030b1536e0aa103f08d7abf7ae8cac0cb001
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu2.diff.gz' pkg-config_0.29.1-0ubuntu2.diff.gz 12715 SHA256:8d5645ccad7bdbcaf3bd83b1b18c7f7d0e2a813e9813b5d4603aa646fc5ff5ea
```

### `dpkg` source package: `poco=1.8.0.1-1ubuntu4`

Binary Packages:

- `libpoco-dev=1.8.0.1-1ubuntu4`
- `libpococrypto50=1.8.0.1-1ubuntu4`
- `libpocodata50=1.8.0.1-1ubuntu4`
- `libpocodatamysql50=1.8.0.1-1ubuntu4`
- `libpocodataodbc50=1.8.0.1-1ubuntu4`
- `libpocodatasqlite50=1.8.0.1-1ubuntu4`
- `libpocofoundation50=1.8.0.1-1ubuntu4`
- `libpocojson50=1.8.0.1-1ubuntu4`
- `libpocomongodb50=1.8.0.1-1ubuntu4`
- `libpoconet50=1.8.0.1-1ubuntu4`
- `libpoconetssl50=1.8.0.1-1ubuntu4`
- `libpocoredis50=1.8.0.1-1ubuntu4`
- `libpocoutil50=1.8.0.1-1ubuntu4`
- `libpocoxml50=1.8.0.1-1ubuntu4`
- `libpocozip50=1.8.0.1-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libpoco-dev/copyright`, `/usr/share/doc/libpococrypto50/copyright`, `/usr/share/doc/libpocodata50/copyright`, `/usr/share/doc/libpocodatamysql50/copyright`, `/usr/share/doc/libpocodataodbc50/copyright`, `/usr/share/doc/libpocodatasqlite50/copyright`, `/usr/share/doc/libpocofoundation50/copyright`, `/usr/share/doc/libpocojson50/copyright`, `/usr/share/doc/libpocomongodb50/copyright`, `/usr/share/doc/libpoconet50/copyright`, `/usr/share/doc/libpoconetssl50/copyright`, `/usr/share/doc/libpocoredis50/copyright`, `/usr/share/doc/libpocoutil50/copyright`, `/usr/share/doc/libpocoxml50/copyright`, `/usr/share/doc/libpocozip50/copyright`)

- `BSD-3-clause`
- `BSL-1.0`
- `Expat`
- `MIT`
- `RSA-MD`
- `Zlib`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris poco=1.8.0.1-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.8.0.1-1ubuntu4.dsc' poco_1.8.0.1-1ubuntu4.dsc 3051 SHA256:fe990610bab8ca4c3c05b0af1ddb52eba946f43439a9e1e094936c03d214339d
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.8.0.1.orig.tar.bz2' poco_1.8.0.1.orig.tar.bz2 4520334 SHA256:61f1e26e25af2201295b6a58a8e2bf74063ad3bf49c8e969ba08af42310716c2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.8.0.1-1ubuntu4.debian.tar.xz' poco_1.8.0.1-1ubuntu4.debian.tar.xz 12716 SHA256:f45010c5cf15a5fe434f007bb4ada1088b3e3cecbe0788fe116649f12ac0efd2
```

### `dpkg` source package: `procps=2:3.3.12-3ubuntu1.2`

Binary Packages:

- `libprocps6:amd64=2:3.3.12-3ubuntu1.2`
- `procps=2:3.3.12-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libprocps6/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.12-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.dsc' procps_3.3.12-3ubuntu1.2.dsc 1920 SHA256:90aeb0430ae305b135a648772fe57255c64cbd6bd8dc900f86d92fd7448ac84c
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12.orig.tar.xz' procps_3.3.12.orig.tar.xz 840540 SHA256:042fcc93e1850aee4c193c51c03f369293fb64fe47e37b38852be6693d12a3af
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.debian.tar.xz' procps_3.3.12-3ubuntu1.2.debian.tar.xz 37736 SHA256:8773c939de7b2cb2b26709452ede19a6e315a83f5fb318e9968f4f4fca16ada4
```

### `dpkg` source package: `pyasn1=0.4.2-3`

Binary Packages:

- `python-pyasn1=0.4.2-3`

Licenses: (parsed from: `/usr/share/doc/python-pyasn1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris pyasn1=0.4.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyasn1/pyasn1_0.4.2-3.dsc' pyasn1_0.4.2-3.dsc 2233 SHA256:888517922336ade422fa159960d48a58bc2bc971a9242b3b32f531b7ab7bfd3c
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyasn1/pyasn1_0.4.2.orig.tar.gz' pyasn1_0.4.2.orig.tar.gz 118404 SHA256:d258b0a71994f7770599835249cece1caef3c70def868c4915e6e5ca49b67d15
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyasn1/pyasn1_0.4.2-3.debian.tar.xz' pyasn1_0.4.2-3.debian.tar.xz 5404 SHA256:c4769523a4353d9aabda5728f456c22882c242ff49aa3457595f0685c5d065a2
```

### `dpkg` source package: `pycodestyle=2.3.1-2`

Binary Packages:

- `python3-pycodestyle=2.3.1-2`

Licenses: (parsed from: `/usr/share/doc/python3-pycodestyle/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris pycodestyle=2.3.1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pycodestyle/pycodestyle_2.3.1-2.dsc' pycodestyle_2.3.1-2.dsc 2225 SHA256:8e3af50b81210e3087818ab5956ead071b8a436679d49a57d1081389f08ced67
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pycodestyle/pycodestyle_2.3.1.orig.tar.gz' pycodestyle_2.3.1.orig.tar.gz 89460 SHA256:682256a5b318149ca0d2a9185d365d8864a768a28db66a84a2ea946bcc426766
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pycodestyle/pycodestyle_2.3.1-2.debian.tar.xz' pycodestyle_2.3.1-2.debian.tar.xz 3772 SHA256:8ff080619bcf2dac5e5c5651e7778fe448394f2d588925d2ca6e5333023818dd
```

### `dpkg` source package: `pycryptodome=3.4.7-1ubuntu1`

Binary Packages:

- `python-pycryptodome=3.4.7-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python-pycryptodome/copyright`)

- `BSD-2-clause`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pycryptodome=3.4.7-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pycryptodome/pycryptodome_3.4.7-1ubuntu1.dsc' pycryptodome_3.4.7-1ubuntu1.dsc 2690 SHA256:b18bdc048bc039ca4f7566adfd07ec9527b0f6617bbe1242fd1261dbc20eaa09
'http://archive.ubuntu.com/ubuntu/pool/main/p/pycryptodome/pycryptodome_3.4.7.orig.tar.gz' pycryptodome_3.4.7.orig.tar.gz 6483140 SHA256:18d8dfe31bf0cb53d58694903e526be68f3cf48e6e3c6dfbbc1e7042b1693af7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pycryptodome/pycryptodome_3.4.7.orig.tar.gz.asc' pycryptodome_3.4.7.orig.tar.gz.asc 862 SHA256:2a0cb959984893539f396039815eadcda26b9fc6f3375d672c1ffa55c636a681
'http://archive.ubuntu.com/ubuntu/pool/main/p/pycryptodome/pycryptodome_3.4.7-1ubuntu1.debian.tar.xz' pycryptodome_3.4.7-1ubuntu1.debian.tar.xz 9972 SHA256:f7510afa5034769b845b4fa2a912c5f14d13ebf84716a4d865e035af660eb000
```

### `dpkg` source package: `pydocstyle=2.0.0-1`

Binary Packages:

- `pydocstyle=2.0.0-1`
- `python3-pydocstyle=2.0.0-1`

Licenses: (parsed from: `/usr/share/doc/pydocstyle/copyright`, `/usr/share/doc/python3-pydocstyle/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris pydocstyle=2.0.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pydocstyle/pydocstyle_2.0.0-1.dsc' pydocstyle_2.0.0-1.dsc 2250 SHA256:b88373d24e38e500b1fce3bfb54645a3bee1d52bb54ffc311179e7a8ffeb6dda
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pydocstyle/pydocstyle_2.0.0.orig.tar.gz' pydocstyle_2.0.0.orig.tar.gz 53137 SHA256:04bdf81c9676165d455433e18359383235d6d1431942fd72e60c67d9447f176e
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pydocstyle/pydocstyle_2.0.0-1.debian.tar.xz' pydocstyle_2.0.0-1.debian.tar.xz 3672 SHA256:f8ab0e880143940c81d4c7bce6dfc6f74d71bc9e58d2964c55e2969974d0828f
```

### `dpkg` source package: `pyflakes=1.6.0-1`

Binary Packages:

- `python3-pyflakes=1.6.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-pyflakes/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris pyflakes=1.6.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pyflakes/pyflakes_1.6.0-1.dsc' pyflakes_1.6.0-1.dsc 2333 SHA256:7b14757a544324f33f7c048198202e85b903b46db90d200c11265c61dbe4cf29
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pyflakes/pyflakes_1.6.0.orig.tar.gz' pyflakes_1.6.0.orig.tar.gz 48184 SHA256:8d616a382f243dbf19b54743f280b80198be0bca3a5396f1d2e1fca6223e8805
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pyflakes/pyflakes_1.6.0-1.debian.tar.xz' pyflakes_1.6.0-1.debian.tar.xz 6836 SHA256:9ea9d5400364ce92f5dc58cc87cc80950ee63b75c33f8479c29f099fe623f260
```

### `dpkg` source package: `pygments=2.2.0+dfsg-1`

Binary Packages:

- `python3-pygments=2.2.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/python3-pygments/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris pygments=2.2.0+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pygments/pygments_2.2.0+dfsg-1.dsc' pygments_2.2.0+dfsg-1.dsc 2381 SHA256:9dd9de375bf5c5c67a08633db98297fb7898cc5ead594f30fba3f7755044142b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pygments/pygments_2.2.0+dfsg.orig.tar.gz' pygments_2.2.0+dfsg.orig.tar.gz 1098631 SHA256:bccdfae9dc1a81812185c33dca06b66f1675a385749b16a6ae089e0055fceefe
'http://archive.ubuntu.com/ubuntu/pool/main/p/pygments/pygments_2.2.0+dfsg-1.debian.tar.xz' pygments_2.2.0+dfsg-1.debian.tar.xz 7368 SHA256:572ab7970d9ea22d49924bdb884e229cdc0d7f558f64d8fc6bd9393a804addc1
```

### `dpkg` source package: `pyparsing=2.2.0+dfsg1-2`

Binary Packages:

- `python-pyparsing=2.2.0+dfsg1-2`
- `python3-pyparsing=2.2.0+dfsg1-2`

Licenses: (parsed from: `/usr/share/doc/python-pyparsing/copyright`, `/usr/share/doc/python3-pyparsing/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-3`
- `ellis-and-grant`
- `salvolainen`

Source:

```console
$ apt-get source -qq --print-uris pyparsing=2.2.0+dfsg1-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.2.0+dfsg1-2.dsc' pyparsing_2.2.0+dfsg1-2.dsc 2429 SHA256:fb7dbda8c89bbddf2d96fab4bf770a59f53b08a8f727652556de98e20e1e74ea
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.2.0+dfsg1.orig.tar.gz' pyparsing_2.2.0+dfsg1.orig.tar.gz 1146636 SHA256:8cf2bde582aa28b854cb96d225606caae902956136e5050ca62125371b06ef8c
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.2.0+dfsg1-2.debian.tar.xz' pyparsing_2.2.0+dfsg1-2.debian.tar.xz 7984 SHA256:f968a17566c942a919fe7024a15bbbb2f1cce5af9c50e01e57ad9580b1e12591
```

### `dpkg` source package: `pytest=3.3.2-2`

Binary Packages:

- `python3-pytest=3.3.2-2`

Licenses: (parsed from: `/usr/share/doc/python3-pytest/copyright`)

- `BSD-3-clause`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris pytest=3.3.2-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pytest/pytest_3.3.2-2.dsc' pytest_3.3.2-2.dsc 2928 SHA256:469a97b5e4989b494856e635f315d0588fcc607dd1027e0ac5d3b9c38ea1cd69
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pytest/pytest_3.3.2.orig.tar.gz' pytest_3.3.2.orig.tar.gz 800095 SHA256:53548280ede7818f4dc2ad96608b9f08ae2cc2ca3874f2ceb6f97e3583f25bc4
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pytest/pytest_3.3.2-2.debian.tar.xz' pytest_3.3.2-2.debian.tar.xz 10000 SHA256:f05a67e9424de4df27e0ab5ccba988b14f419e8a09c9bcaf91b448ae6be29430
```

### `dpkg` source package: `python-argcomplete=1.8.1-1ubuntu1`

Binary Packages:

- `python3-argcomplete=1.8.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python3-argcomplete/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris python-argcomplete=1.8.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-argcomplete/python-argcomplete_1.8.1-1ubuntu1.dsc' python-argcomplete_1.8.1-1ubuntu1.dsc 2310 SHA256:3d333ad4515e799337309c8c63d45f4134d5513235c4eb64446b9c096729dc15
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-argcomplete/python-argcomplete_1.8.1.orig.tar.gz' python-argcomplete_1.8.1.orig.tar.gz 53282 SHA256:2997cc0e17d8a2db4789dc84cfe02a0b1579f1f17d79b0b993e722d0acee0649
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-argcomplete/python-argcomplete_1.8.1-1ubuntu1.debian.tar.xz' python-argcomplete_1.8.1-1ubuntu1.debian.tar.xz 6584 SHA256:09435564b8da869a16c672af024d99213e9af80e406617c191ecbb717bcc6d7f
```

### `dpkg` source package: `python-attrs=17.4.0-2`

Binary Packages:

- `python3-attr=17.4.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-attr/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-attrs=17.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-attrs/python-attrs_17.4.0-2.dsc' python-attrs_17.4.0-2.dsc 2639 SHA256:d36062c2a69d4af57a3994f3dce7a06904f44e8305a1763d4b1e86f2c049a66a
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-attrs/python-attrs_17.4.0.orig.tar.gz' python-attrs_17.4.0.orig.tar.gz 90280 SHA256:110aba2541f69caabe061caf6d034dcdf5890464432dcae9297bffef3e8abf17
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-attrs/python-attrs_17.4.0-2.debian.tar.xz' python-attrs_17.4.0-2.debian.tar.xz 4084 SHA256:a9046e718b3fbdabdc2c7da669f8552c1347549f1e6f0f43605fd0e04138db30
```

### `dpkg` source package: `python-catkin-pkg-modules=0.4.22-1`

Binary Packages:

- `python-catkin-pkg-modules=0.4.22-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-catkin-pkg-modules=0.4.22-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-catkin-pkg-modules/python-catkin-pkg-modules_0.4.22-1.debian.tar.xz' python-catkin-pkg-modules_0.4.22-1.debian.tar.xz 2012 SHA512:196cb36b8058d89a4d11e009329ccc62479830eaa28c88e8f8b53bc10c2160bed2187cbc263d66b6fd855e03d9003b64bcb26c2c43b9f07948479a93a6052a6b
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-catkin-pkg-modules/python-catkin-pkg-modules_0.4.22-1.dsc' python-catkin-pkg-modules_0.4.22-1.dsc 998 SHA512:bdcf8472f0932d8cb008c87c3eaf63ca61cb0f77c1e93e600987568087ea22cb6307b53478c0bebbe3d79ea130e58f51c8c27c54f982190fb4079370e051d7aa
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-catkin-pkg-modules/python-catkin-pkg-modules_0.4.22.orig.tar.gz' python-catkin-pkg-modules_0.4.22.orig.tar.gz 61251 SHA512:a1b16232b3707b8acfaed581a9315406e4e8efa08d69e19a98ffb9970cf19320795abf2e6f6e73c0cba563fc66538835fc074824053086926f293a40d5dde91b
```

### `dpkg` source package: `python-catkin-pkg=0.4.22-100`

Binary Packages:

- `python-catkin-pkg=0.4.22-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-catkin-pkg=0.4.22-100
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-catkin-pkg/python-catkin-pkg_0.4.22-100.debian.tar.xz' python-catkin-pkg_0.4.22-100.debian.tar.xz 1996 SHA512:c3b798b53cd0dc7b9a077537dd0ffd16a2b77824a3a4b07f6d86f78274684f246508360503bedeb8d89e12cb401b2b3a3c2a67c17e8de3c71da67b96cc7f4fae
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-catkin-pkg/python-catkin-pkg_0.4.22-100.dsc' python-catkin-pkg_0.4.22-100.dsc 938 SHA512:d9270066f6a8946d7b705f3137316ca1d7cbe797f976dc91a03d13e4a3e802b469b98bbb3b05dcb9bc780bd943bddb0cd067f184d0c198e75c1269544bd6ca18
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-catkin-pkg/python-catkin-pkg_0.4.22.orig.tar.gz' python-catkin-pkg_0.4.22.orig.tar.gz 13730 SHA512:61b65d1c444e76e346098175534be3eb71b83f6c82f8f336e9ac87632705761552b9bb670f13f3d51885f1f8e63153475b1243ad299c48353bce662b73bb8872
```

### `dpkg` source package: `python-cffi=1.11.5-1`

Binary Packages:

- `python-cffi-backend=1.11.5-1`

Licenses: (parsed from: `/usr/share/doc/python-cffi-backend/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-cffi=1.11.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.11.5-1.dsc' python-cffi_1.11.5-1.dsc 2566 SHA256:ea78c9d66e5e6f567e96e7ce940766234efb60b9acfc58b1e144ae8ab6c541c2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.11.5.orig.tar.gz' python-cffi_1.11.5.orig.tar.gz 438498 SHA256:e90f17980e6ab0f3c2f3730e56d1fe9bcba1891eeea58966e89d352492cc74f4
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.11.5-1.debian.tar.xz' python-cffi_1.11.5-1.debian.tar.xz 5692 SHA256:e4771d799b765f449ce46bc20e671b771bfcc7b5e4d829ffb26280e6de215648
```

### `dpkg` source package: `python-coverage=4.5+dfsg.1-3`

Binary Packages:

- `python3-coverage=4.5+dfsg.1-3`

Licenses: (parsed from: `/usr/share/doc/python3-coverage/copyright`)

- `Apache-2`
- `Apache-2.0`
- `Expat`
- `GPL-2`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris python-coverage=4.5+dfsg.1-3
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-coverage/python-coverage_4.5+dfsg.1-3.dsc' python-coverage_4.5+dfsg.1-3.dsc 2554 SHA256:674c3ecb4328b1ec57f46ddaf30e9ae6b2d5defc46c09521c79409f77f8e9071
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-coverage/python-coverage_4.5+dfsg.1.orig.tar.gz' python-coverage_4.5+dfsg.1.orig.tar.gz 340322 SHA256:11f0384cbd8b06b84e96ce4a1860fa698297623a5444a4b63ce686a067753fbc
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-coverage/python-coverage_4.5+dfsg.1-3.debian.tar.xz' python-coverage_4.5+dfsg.1-3.debian.tar.xz 21196 SHA256:bc969efe651fb9a83754d4644d0cd49de4f652310ce64a727ee30bb598bfd3db
```

### `dpkg` source package: `python-cryptography=2.1.4-1ubuntu1.3`

Binary Packages:

- `python-cryptography=2.1.4-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/python-cryptography/copyright`)

- `Apache`
- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-cryptography=2.1.4-1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_2.1.4-1ubuntu1.3.dsc' python-cryptography_2.1.4-1ubuntu1.3.dsc 3320 SHA256:f737d3ad9ed01268700c4eeaed159eaee65d8f925500b0acb498399b4d01d369
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_2.1.4.orig.tar.gz' python-cryptography_2.1.4.orig.tar.gz 441557 SHA256:e4d967371c5b6b2e67855066471d844c5d52d210c36c28d49a8507b96e2c5291
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_2.1.4-1ubuntu1.3.debian.tar.xz' python-cryptography_2.1.4-1ubuntu1.3.debian.tar.xz 28008 SHA256:5a6facc3be61feda9640674a6ef179cdf7210460b931386aa5c7e600dccfe106
```

### `dpkg` source package: `python-dateutil=2.6.1-1`

Binary Packages:

- `python-dateutil=2.6.1-1`
- `python3-dateutil=2.6.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-dateutil=2.6.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.6.1-1.dsc' python-dateutil_2.6.1-1.dsc 2128 SHA256:17e9a795c53c1c4e4832e8926cb321138934b4d09457dfff45194182b937a311
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.6.1.orig.tar.gz' python-dateutil_2.6.1.orig.tar.gz 241428 SHA256:891c38b2a02f5bb1be3e4793866c8df49c7d19baabf9c1bad62547e0b4866aca
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.6.1-1.debian.tar.xz' python-dateutil_2.6.1-1.debian.tar.xz 13648 SHA256:ef4fcc1f8a6fc095b15953986d1dd24d05f51c167f0ee212e3f8fef772c43f26
```

### `dpkg` source package: `python-defaults=2.7.15~rc1-1`

Binary Packages:

- `libpython-dev:amd64=2.7.15~rc1-1`
- `libpython-stdlib:amd64=2.7.15~rc1-1`
- `python=2.7.15~rc1-1`
- `python-dev=2.7.15~rc1-1`
- `python-minimal=2.7.15~rc1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.15~rc1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.15~rc1-1.dsc' python-defaults_2.7.15~rc1-1.dsc 2633 SHA256:1089e25a274fb86e8dfbab1b661ecb5ef2b7610e1b6e3fbf8388f875758f7c2c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.15~rc1-1.tar.gz' python-defaults_2.7.15~rc1-1.tar.gz 1958015 SHA256:f3bed2b81091821d2e514c2e17c6846f7e744487fd15f7d3c48fa1c91b9cd49b
```

### `dpkg` source package: `python-docutils=0.14+dfsg-3`

Binary Packages:

- `docutils-common=0.14+dfsg-3`
- `python-docutils=0.14+dfsg-3`
- `python3-docutils=0.14+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/docutils-common/copyright`, `/usr/share/doc/python-docutils/copyright`, `/usr/share/doc/python3-docutils/copyright`)

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
$ apt-get source -qq --print-uris python-docutils=0.14+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.14+dfsg-3.dsc' python-docutils_0.14+dfsg-3.dsc 2446 SHA256:400dc1214c70e86c13dd34dd134e4ece07fbbc0119f2c7ed0bf173fb7618bd5d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.14+dfsg.orig.tar.gz' python-docutils_0.14+dfsg.orig.tar.gz 1739255 SHA256:9731d30e7d958c7fe8fcc20c1689064e130053c954e61df20ac5362eb6305760
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.14+dfsg-3.debian.tar.xz' python-docutils_0.14+dfsg-3.debian.tar.xz 31188 SHA256:3e73e6211785b227dc0c9258e1a69b0adbbd129a401b5b09886981789569e024
```

### `dpkg` source package: `python-flake8=3.5.0-1`

Binary Packages:

- `python3-flake8=3.5.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-flake8/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-flake8=3.5.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-flake8/python-flake8_3.5.0-1.dsc' python-flake8_3.5.0-1.dsc 2663 SHA256:f6adee6a00a8f8b90bf8543cf1243484af9d4325b8b6dfc486edb9a264c16669
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-flake8/python-flake8_3.5.0.orig.tar.gz' python-flake8_3.5.0.orig.tar.gz 140608 SHA256:7253265f7abd8b313e3892944044a365e3f4ac3fcdcfb4298f55ee9ddf188ba0
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-flake8/python-flake8_3.5.0-1.debian.tar.xz' python-flake8_3.5.0-1.debian.tar.xz 7792 SHA256:fd7a410138d42c7eb32f07e79e9e6d036e4714dd695ef224af55d22387ad0568
```

### `dpkg` source package: `python-funcsigs=1.0.2-4`

Binary Packages:

- `python-funcsigs=1.0.2-4`

Licenses: (parsed from: `/usr/share/doc/python-funcsigs/copyright`)

- `Apache-2`
- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris python-funcsigs=1.0.2-4
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-funcsigs/python-funcsigs_1.0.2-4.dsc' python-funcsigs_1.0.2-4.dsc 2438 SHA256:0535606459f0cc83dce3b8a20fc499bee2e54ca525510c34ab611108dc4236eb
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-funcsigs/python-funcsigs_1.0.2.orig.tar.xz' python-funcsigs_1.0.2.orig.tar.xz 20668 SHA256:8493ee895349929854f9a4b362bcd92c9527c70e3eefbd7524a10692c24f6eab
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-funcsigs/python-funcsigs_1.0.2-4.debian.tar.xz' python-funcsigs_1.0.2-4.debian.tar.xz 3860 SHA256:396fe62f4ae0ac23e3e12bab27f984e7181f805bbcf72b22df691bb15237e8f2
```

### `dpkg` source package: `python-gnupg=0.4.1-1ubuntu1.18.04.1`

Binary Packages:

- `python-gnupg=0.4.1-1ubuntu1.18.04.1`

Licenses: (parsed from: `/usr/share/doc/python-gnupg/copyright`)

- `BSD-3-clause`
- `pycrypto`

Source:

```console
$ apt-get source -qq --print-uris python-gnupg=0.4.1-1ubuntu1.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-gnupg/python-gnupg_0.4.1-1ubuntu1.18.04.1.dsc' python-gnupg_0.4.1-1ubuntu1.18.04.1.dsc 2285 SHA256:dbea9c9edd833ba916878f269ec78432bcc0d8b5bf30722127b8c92fff27b1df
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-gnupg/python-gnupg_0.4.1.orig.tar.gz' python-gnupg_0.4.1.orig.tar.gz 44534 SHA256:ef47b02eaf41dee3cf4b02ddf83130827318de9fe3eae89d01a3f05859e20e1a
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-gnupg/python-gnupg_0.4.1-1ubuntu1.18.04.1.debian.tar.xz' python-gnupg_0.4.1-1ubuntu1.18.04.1.debian.tar.xz 9992 SHA256:fe6d8bc444465238e391024f4da116f46e2470bfeb3529c45fad34a19499878c
```

### `dpkg` source package: `python-idna=2.6-1`

Binary Packages:

- `python-idna=2.6-1`

Licenses: (parsed from: `/usr/share/doc/python-idna/copyright`)

- `BSD-3-clause`
- `PSF-2`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris python-idna=2.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-idna/python-idna_2.6-1.dsc' python-idna_2.6-1.dsc 2211 SHA256:e53dc537db7f178ca67efb2e728985644234290aea8b3ae03dfe393181b8a825
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-idna/python-idna_2.6.orig.tar.gz' python-idna_2.6.orig.tar.gz 135992 SHA256:2c6a5de3089009e3da7c5dde64a141dbc8551d5b7f6cf4ed7c2568d0cc520a8f
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-idna/python-idna_2.6-1.debian.tar.xz' python-idna_2.6-1.debian.tar.xz 4472 SHA256:64740dad9d18032de36a6f81f0bcbbc3356a27705b65da792673be510929ae8c
```

### `dpkg` source package: `python-ipaddress=1.0.17-1`

Binary Packages:

- `python-ipaddress=1.0.17-1`

Licenses: (parsed from: `/usr/share/doc/python-ipaddress/copyright`)

- `Expat`
- `PSF-2`

Source:

```console
$ apt-get source -qq --print-uris python-ipaddress=1.0.17-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-ipaddress/python-ipaddress_1.0.17-1.dsc' python-ipaddress_1.0.17-1.dsc 2146 SHA256:c2737119d84971270b25ff6ddcbdd37d33cf364e24d9861beeffb06c164e83e4
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-ipaddress/python-ipaddress_1.0.17.orig.tar.gz' python-ipaddress_1.0.17.orig.tar.gz 32434 SHA256:3a21c5a15f433710aaa26f1ae174b615973a25182006ae7f9c26de151cd51716
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-ipaddress/python-ipaddress_1.0.17-1.debian.tar.xz' python-ipaddress_1.0.17-1.debian.tar.xz 3624 SHA256:0eb6e0b886d4c6cae9274fdd3aacf78dc7efb559bd2fea2612c312095f9a3f0c
```

### `dpkg` source package: `python-mccabe=0.6.1-2`

Binary Packages:

- `python3-mccabe=0.6.1-2`

Licenses: (parsed from: `/usr/share/doc/python3-mccabe/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-mccabe=0.6.1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mccabe/python-mccabe_0.6.1-2.dsc' python-mccabe_0.6.1-2.dsc 2256 SHA256:b73285046565cb1836c03030aba33b0fe1d0591035a63e054bfbac1b7fe80e18
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mccabe/python-mccabe_0.6.1.orig.tar.gz' python-mccabe_0.6.1.orig.tar.gz 8612 SHA256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mccabe/python-mccabe_0.6.1-2.debian.tar.xz' python-mccabe_0.6.1-2.debian.tar.xz 2664 SHA256:c5d148691ce33088de869eb4d7312f7c1133224693ff3efd658da523b442d636
```

### `dpkg` source package: `python-mock=2.0.0-3`

Binary Packages:

- `python-mock=2.0.0-3`

Licenses: (parsed from: `/usr/share/doc/python-mock/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris python-mock=2.0.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-mock/python-mock_2.0.0-3.dsc' python-mock_2.0.0-3.dsc 2449 SHA256:7c8d5206402f697f9f2d6202b39a31a81211f680b9e960deb68141042a0a08a5
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-mock/python-mock_2.0.0.orig.tar.gz' python-mock_2.0.0.orig.tar.gz 73684 SHA256:b158b6df76edd239b8208d481dc46b6afd45a846b7812ff0ce58971cf5bc8bba
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-mock/python-mock_2.0.0-3.debian.tar.xz' python-mock_2.0.0-3.debian.tar.xz 16008 SHA256:03ddc534c620681c7a0870917b84ab20869722e255a5912080846b35f4e0f7f3
```

### `dpkg` source package: `python-notify2=0.3-3`

Binary Packages:

- `python3-notify2=0.3-3`

Licenses: (parsed from: `/usr/share/doc/python3-notify2/copyright`)

- `BSD-3-Clause`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris python-notify2=0.3-3
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-notify2/python-notify2_0.3-3.dsc' python-notify2_0.3-3.dsc 2210 SHA256:71f75c5e80171e0320ddf1792d71c0f9c0a0ef35f8807bec105baedb56bc40f8
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-notify2/python-notify2_0.3.orig.tar.gz' python-notify2_0.3.orig.tar.gz 8798 SHA256:684281f91c51fc60bc7909a35bd21d043a2a421f4e269de1ed1f13845d1d6321
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-notify2/python-notify2_0.3-3.debian.tar.xz' python-notify2_0.3-3.debian.tar.xz 3260 SHA256:0a127940fc81420d388d9c99d4902b57a4ad7e367edc6fcd797ee312c635b9f8
```

### `dpkg` source package: `python-numpy=1:1.13.3-2ubuntu1`

Binary Packages:

- `python-numpy=1:1.13.3-2ubuntu1`
- `python3-numpy=1:1.13.3-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python-numpy/copyright`, `/usr/share/doc/python3-numpy/copyright`)

- `PSF`

Source:

```console
$ apt-get source -qq --print-uris python-numpy=1:1.13.3-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-numpy/python-numpy_1.13.3-2ubuntu1.dsc' python-numpy_1.13.3-2ubuntu1.dsc 3000 SHA256:5cbbdaa075dc0a5732bf4dc703a49c5c4f0a4c3c0af2616e773be339fa5cdca3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-numpy/python-numpy_1.13.3.orig.tar.gz' python-numpy_1.13.3.orig.tar.gz 4520295 SHA256:5e3cb4c3797a4f0da082cab65ab00fa4a9d7552391876e2bb53f39a35bdc78cf
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-numpy/python-numpy_1.13.3-2ubuntu1.debian.tar.xz' python-numpy_1.13.3-2ubuntu1.debian.tar.xz 144196 SHA256:7dc98e90991b19f413137e8289a81ec2a9bfc7679719235d914af98d96dea33f
```

### `dpkg` source package: `python-pbr=3.1.1-3ubuntu3`

Binary Packages:

- `python-pbr=3.1.1-3ubuntu3`

Licenses: (parsed from: `/usr/share/doc/python-pbr/copyright`)

- `Apache-2`
- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris python-pbr=3.1.1-3ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-pbr/python-pbr_3.1.1-3ubuntu3.dsc' python-pbr_3.1.1-3ubuntu3.dsc 2914 SHA256:cd1815dfbf991fcba479216385ae66f3665f328c13ae46b28da7ea7b34434dd3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-pbr/python-pbr_3.1.1.orig.tar.xz' python-pbr_3.1.1.orig.tar.xz 72404 SHA256:ed8126ebd7a9eef94bf002c93d98b6d67471f9875c81d924d26a89fcab70f301
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-pbr/python-pbr_3.1.1-3ubuntu3.debian.tar.xz' python-pbr_3.1.1-3ubuntu3.debian.tar.xz 8088 SHA256:5fde52db13d8b8a1c8b42ecc1d10ad4323bedbfe7785e2f0793bf40a32682485
```

### `dpkg` source package: `python-pluggy=0.6.0-1`

Binary Packages:

- `python3-pluggy=0.6.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-pluggy/copyright`)

- `Expat`
- `MIT/Expat`

Source:

```console
$ apt-get source -qq --print-uris python-pluggy=0.6.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pluggy/python-pluggy_0.6.0-1.dsc' python-pluggy_0.6.0-1.dsc 2270 SHA256:757e414727bcc16df4e79552d25a6838170312985c7c269352bc6236f887cc1b
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pluggy/python-pluggy_0.6.0.orig.tar.gz' python-pluggy_0.6.0.orig.tar.gz 19678 SHA256:7f8ae7f5bdf75671a718d2daf0a64b7885f74510bcd98b1a0bb420eb9a9d0cff
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pluggy/python-pluggy_0.6.0-1.debian.tar.xz' python-pluggy_0.6.0-1.debian.tar.xz 2484 SHA256:e6023e4f30da1d72a4b3ba799dfb666d90db764a6e25863a702b4571ab7272a8
```

### `dpkg` source package: `python-py=1.5.2-1`

Binary Packages:

- `python3-py=1.5.2-1`

Licenses: (parsed from: `/usr/share/doc/python3-py/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-py=1.5.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-py/python-py_1.5.2-1.dsc' python-py_1.5.2-1.dsc 2267 SHA256:fb37869e73c13ff1b73e6ac11db524c90b5da73f74b3e59151ae69c4c3fd5f7e
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-py/python-py_1.5.2.orig.tar.gz' python-py_1.5.2.orig.tar.gz 189542 SHA256:ca18943e28235417756316bfada6cd96b23ce60dd532642690dcfdaba988a76d
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-py/python-py_1.5.2-1.debian.tar.xz' python-py_1.5.2-1.debian.tar.xz 6972 SHA256:95134eff689e0537255f73e222c7b82b832fbeabef7beaeae7fbc218e723beb0
```

### `dpkg` source package: `python-pytest-cov=2.5.1-1`

Binary Packages:

- `python3-pytest-cov=2.5.1-1`

Licenses: (parsed from: `/usr/share/doc/python3-pytest-cov/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris python-pytest-cov=2.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pytest-cov/python-pytest-cov_2.5.1-1.dsc' python-pytest-cov_2.5.1-1.dsc 2164 SHA256:d1aa2b0d3c866e38335f27940fd186e36c9508463d5421f17d7959babba2c4e7
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pytest-cov/python-pytest-cov_2.5.1.orig.tar.gz' python-pytest-cov_2.5.1.orig.tar.gz 28668 SHA256:a2a52fa5a893e6192dd4801f5598e6affffe1b6f4142ade2345f2455e6a75b91
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pytest-cov/python-pytest-cov_2.5.1-1.debian.tar.xz' python-pytest-cov_2.5.1-1.debian.tar.xz 2252 SHA256:a0b1dfb7bcdba83a3fde89817024976f6630b04ca56a259bba24218f263789b1
```

### `dpkg` source package: `python-roman=2.0.0-3`

Binary Packages:

- `python-roman=2.0.0-3`
- `python3-roman=2.0.0-3`

Licenses: (parsed from: `/usr/share/doc/python-roman/copyright`, `/usr/share/doc/python3-roman/copyright`)

- `Python-2.1.1`
- `ZPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris python-roman=2.0.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0-3.dsc' python-roman_2.0.0-3.dsc 2132 SHA256:0470c89ad49bfbcf20bb59cb86f5de4d2f7d597ffc7519ecb07064ef313f252e
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0.orig.tar.gz' python-roman_2.0.0.orig.tar.gz 4968 SHA256:98f2c0fb3cdcfba465d12c85b3b7139fc4cd2177f1325f1bacfe00878c8fa7b9
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0-3.debian.tar.xz' python-roman_2.0.0-3.debian.tar.xz 8596 SHA256:fa6c16b3e4d328a8cfe16fbed994add1a2c9cb5a5955bff374244794a6cddf31
```

### `dpkg` source package: `python-rosdep-modules=0.19.0-1`

Binary Packages:

- `python-rosdep-modules=0.19.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-rosdep-modules=0.19.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdep-modules/python-rosdep-modules_0.19.0-1.debian.tar.xz' python-rosdep-modules_0.19.0-1.debian.tar.xz 1992 SHA512:c43f273c17ceb8e1543d1d350765b68f7167a264d840abb494df7efc82c494a0e02c24b446815b6b824fbfe76dbdd72a00eb07e5c3f549b6cc7b07be97f8f377
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdep-modules/python-rosdep-modules_0.19.0-1.dsc' python-rosdep-modules_0.19.0-1.dsc 973 SHA512:940b0ab729fd9b4b3e3ea4b7116b1663af4adccc47a193800a4cb3344d87b22657bdfbc7fd846c399d735b5b446beacd912662ddeba826431b579f32ee928d9f
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdep-modules/python-rosdep-modules_0.19.0.orig.tar.gz' python-rosdep-modules_0.19.0.orig.tar.gz 87964 SHA512:a837139da1a8c5fb7bad413214155e8849a15a6f98a420b68caebc61e5793655fba3ae4167baf3bed0eb398bcb3ff24012ed83e92747de4e52b32938588cdb08
```

### `dpkg` source package: `python-rosdep=0.19.0-1`

Binary Packages:

- `python-rosdep=0.19.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-rosdep=0.19.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdep/python-rosdep_0.19.0-1.debian.tar.xz' python-rosdep_0.19.0-1.debian.tar.xz 1932 SHA512:e556c1a78ca6117db0ed7aa1124443b664ef7507eb55f04aae0297e4319a672d291ef64ab4e1186eb1b61f11c6ceafb73169cffbd32f1866754cfe12e699c6ef
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdep/python-rosdep_0.19.0-1.dsc' python-rosdep_0.19.0-1.dsc 905 SHA512:29a9593dfad67df290105fad315acb8a20bd9c51aaba1a7984cd82ccfddcbfdb326d880279f453c6e59fdd099ad1ef5f86eb225372f8a986ed745db44bf15378
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdep/python-rosdep_0.19.0.orig.tar.gz' python-rosdep_0.19.0.orig.tar.gz 31450 SHA512:061dba206671ce4e8221b369240e7b64a7752539329bbe2e8c1a282619b8aca9d35c0aa4d46c27bd51c9ee6f8d39dc6a323c8d023a70b8eacc80272254030724
```

### `dpkg` source package: `python-rosdistro-modules=0.8.2-1`

Binary Packages:

- `python-rosdistro-modules=0.8.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-rosdistro-modules=0.8.2-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdistro-modules/python-rosdistro-modules_0.8.2-1.debian.tar.xz' python-rosdistro-modules_0.8.2-1.debian.tar.xz 1988 SHA512:a339a999fb7149b0c41aee71da8871b7c4000545204850ce5ea1f0f9ff5b4bd07a100dff71e6b41c6168230b76d0fe159906cf1e1776c6ef931cfd76981efcfb
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdistro-modules/python-rosdistro-modules_0.8.2-1.dsc' python-rosdistro-modules_0.8.2-1.dsc 982 SHA512:f72d4f790e2aa31edb5e6edb1d54de1999a02a4da3b31910f881ff1e39d38b6fe8347906c171a5eb2734127d305d6086bf97e81cda66a509c4b0e3d76df2ca69
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdistro-modules/python-rosdistro-modules_0.8.2.orig.tar.gz' python-rosdistro-modules_0.8.2.orig.tar.gz 42056 SHA512:a4c8402c8fab84ca70b32e6d1e2354d609dbbc66d853c7e7815dff1b7625d75158958a75a850556d4e44160d9a9b435739a1b64d9186d7230a1233530d9f283a
```

### `dpkg` source package: `python-rosdistro=0.8.2-100`

Binary Packages:

- `python-rosdistro=0.8.2-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-rosdistro=0.8.2-100
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdistro/python-rosdistro_0.8.2-100.debian.tar.xz' python-rosdistro_0.8.2-100.debian.tar.xz 1976 SHA512:4da9b7ed5b168b813e7565939836eba5d37c29987a0f42603b1e947da2097b09d73efd66cd63e1409b3df80f96f2fa43837364000be5d82bb4eae3242a3e2d20
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdistro/python-rosdistro_0.8.2-100.dsc' python-rosdistro_0.8.2-100.dsc 922 SHA512:847f8f603e6c42cc2e4947e4f005a70f68df780ded4ffc6b2cb30b81b1aa081db63eb6fe89dbdf2e6945e50ef0c11ed79e45c4b381b509fd148b20a22929aba7
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosdistro/python-rosdistro_0.8.2.orig.tar.gz' python-rosdistro_0.8.2.orig.tar.gz 10001 SHA512:cc5a5c0e617bc34f48850d2c36da06a3e99d96c890db2429a7f4ad7b7a508ec71b892f5d0b50673f4b372506161667d7253e1ce4bfe1324e4591a53e813ed70d
```

### `dpkg` source package: `python-rospkg-modules=1.2.8-1`

Binary Packages:

- `python-rospkg-modules=1.2.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-rospkg-modules=1.2.8-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rospkg-modules/python-rospkg-modules_1.2.8-1.debian.tar.xz' python-rospkg-modules_1.2.8-1.debian.tar.xz 1164 SHA512:ee9e4934f1ecff828877fd043093928e8d38b32f1d67039bbad8c8f793132a1edbcfa6c0ae2bad83e662a57a9aa4619f10fa14ae8ebd52b25da0cda9f378414f
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rospkg-modules/python-rospkg-modules_1.2.8-1.dsc' python-rospkg-modules_1.2.8-1.dsc 953 SHA512:2eacc13c7a5ea2450a7aec8b29807a8bf354e3bfb8be8975db36516085dc9c7e56caa567765ab16fb28decfbd9440ee8cd421e1f2a17f269f158c60bd68e8c07
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rospkg-modules/python-rospkg-modules_1.2.8.orig.tar.gz' python-rospkg-modules_1.2.8.orig.tar.gz 41310 SHA512:0aa1cdab428424ab289ca81ef59d41207e53e45b0007d584b5d163703a7decce351030ddd1b30b31de2da0b75ee0b7ea101268a73ec63d484692442c0660e524
```

### `dpkg` source package: `python-rospkg=1.2.8-100`

Binary Packages:

- `python-rospkg=1.2.8-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-rospkg=1.2.8-100
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rospkg/python-rospkg_1.2.8-100.debian.tar.xz' python-rospkg_1.2.8-100.debian.tar.xz 1140 SHA512:250cdb129cb9fe485bb14ea2c62330ad020ff1e59c906d252fb060db637baed72edbb6f688ca255c9eea0798900db3d59ee7f6d4399a6314d0235a29c1fa83eb
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rospkg/python-rospkg_1.2.8-100.dsc' python-rospkg_1.2.8-100.dsc 889 SHA512:4686f00e08aafedd7e1beb914b97dfc3fcebafcd43c9e8140b5b0295e1bf22859d972f7cceff9e9cbae50ed0c4fa73944ea905dc4fd7f98df1238c8fb93568fd
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rospkg/python-rospkg_1.2.8.orig.tar.gz' python-rospkg_1.2.8.orig.tar.gz 17431 SHA512:9e6eecb516b81bc026e545b1fa7e3d39ee12eabc8985556e12d2abf920c58f5285b7c33d02c4f535049f55db7a9640905f1d9f6992389c93ca9dbee655851094
```

### `dpkg` source package: `python-setuptools=39.0.1-2`

Binary Packages:

- `python-pkg-resources=39.0.1-2`
- `python-setuptools=39.0.1-2`
- `python3-pkg-resources=39.0.1-2`
- `python3-setuptools=39.0.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-setuptools=39.0.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-setuptools/python-setuptools_39.0.1-2.dsc' python-setuptools_39.0.1-2.dsc 2394 SHA256:ff5d172461544d2d847e6d3ecef3356141a4487dcc3047a88db61744986cf999
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-setuptools/python-setuptools_39.0.1.orig.tar.xz' python-setuptools_39.0.1.orig.tar.xz 454544 SHA256:b79bf38d5d74f348f534ba92b49ca21f124046acbb66d54f845aa910af49adff
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-setuptools/python-setuptools_39.0.1-2.debian.tar.xz' python-setuptools_39.0.1-2.debian.tar.xz 15040 SHA256:2e997b64dd6b9ff88672eb965c23ab505558ca45b34d47c87a18e90751fe189a
```

### `dpkg` source package: `python-snowballstemmer=1.2.1-1`

Binary Packages:

- `python3-snowballstemmer=1.2.1-1`

Licenses: (parsed from: `/usr/share/doc/python3-snowballstemmer/copyright`)

- `BSD-2-Clause`

Source:

```console
$ apt-get source -qq --print-uris python-snowballstemmer=1.2.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-snowballstemmer/python-snowballstemmer_1.2.1-1.dsc' python-snowballstemmer_1.2.1-1.dsc 2165 SHA256:efd11cc1667d71771243599e442f8a75ca23d40092ac18172a2242b7b2a80151
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-snowballstemmer/python-snowballstemmer_1.2.1.orig.tar.gz' python-snowballstemmer_1.2.1.orig.tar.gz 49626 SHA256:919f26a68b2c17a7634da993d91339e288964f93c274f1343e3bbbe2096e1128
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-snowballstemmer/python-snowballstemmer_1.2.1-1.debian.tar.xz' python-snowballstemmer_1.2.1-1.debian.tar.xz 1976 SHA256:d5f3115a2b43b9462a1c0a963a9489e42bfa1ded461ed947ae4f94de79f34d91
```

### `dpkg` source package: `python2.7=2.7.17-1~18.04ubuntu1.1`

Binary Packages:

- `libpython2.7:amd64=2.7.17-1~18.04ubuntu1.1`
- `libpython2.7-dev:amd64=2.7.17-1~18.04ubuntu1.1`
- `libpython2.7-minimal:amd64=2.7.17-1~18.04ubuntu1.1`
- `libpython2.7-stdlib:amd64=2.7.17-1~18.04ubuntu1.1`
- `python2.7=2.7.17-1~18.04ubuntu1.1`
- `python2.7-dev=2.7.17-1~18.04ubuntu1.1`
- `python2.7-minimal=2.7.17-1~18.04ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libpython2.7/copyright`, `/usr/share/doc/libpython2.7-dev/copyright`, `/usr/share/doc/libpython2.7-minimal/copyright`, `/usr/share/doc/libpython2.7-stdlib/copyright`, `/usr/share/doc/python2.7/copyright`, `/usr/share/doc/python2.7-dev/copyright`, `/usr/share/doc/python2.7-minimal/copyright`)

- `# Licensed to PSF under a Contributor Agreement`
- `* Permission to use this software in any way is granted without`
- `Apache`
- `Apache-2`
- `Apache-2.0`
- `Expat`
- `GPL-2`
- `ISC`
- `LGPL-2.1+`
- `PSF-2`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Python`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `implied`
- `see above, some license as Python`

Source:

```console
$ apt-get source -qq --print-uris python2.7=2.7.17-1~18.04ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.17-1~18.04ubuntu1.1.dsc' python2.7_2.7.17-1~18.04ubuntu1.1.dsc 3483 SHA256:510b3b29af9ceabe92aba0f7dd2f9899ae8f46ec9354f4dd7662e50b78701671
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.17.orig.tar.gz' python2.7_2.7.17.orig.tar.gz 17535962 SHA256:f22059d09cdf9625e0a7284d24a13062044f5bf59d93a7f3382190dfa94cecde
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.17-1~18.04ubuntu1.1.diff.gz' python2.7_2.7.17-1~18.04ubuntu1.1.diff.gz 292136 SHA256:e183d38788146b5ab09108a17b8ad979e918c5abbe43ae2ad172404effed101e
```

### `dpkg` source package: `python3-catkin-pkg-modules=0.4.22-1`

Binary Packages:

- `python3-catkin-pkg-modules=0.4.22-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-catkin-pkg-modules=0.4.22-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-catkin-pkg-modules/python3-catkin-pkg-modules_0.4.22-1.debian.tar.xz' python3-catkin-pkg-modules_0.4.22-1.debian.tar.xz 2004 SHA512:7a77f11205e8eff570202c663f6e8e3edb34424381e0850e9487ab00729b88f477a04ede6a1ce82383716afccfe523e2d844508e2aa8f59368c81d971a09d479
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-catkin-pkg-modules/python3-catkin-pkg-modules_0.4.22-1.dsc' python3-catkin-pkg-modules_0.4.22-1.dsc 985 SHA512:42f76df4c7afb24a9f56b1a1443ae1750c39368517e062d211aed5115d1de1db736b3f013fb0a32738c884aae8ce4bac21b227e25146399554aea012f6e44c55
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-catkin-pkg-modules/python3-catkin-pkg-modules_0.4.22.orig.tar.gz' python3-catkin-pkg-modules_0.4.22.orig.tar.gz 62662 SHA512:36c56194105e564fdcde7e254e88bd25a3c50f138bbf5d62e7e0a70c747db4dcc529300e8573f187a6e0852776170a5ec251d1905be4b4ae3c37870e61111409
```

### `dpkg` source package: `python3-colcon-argcomplete=0.3.3-1`

Binary Packages:

- `python3-colcon-argcomplete=0.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-argcomplete=0.3.3-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-argcomplete/python3-colcon-argcomplete_0.3.3-1.debian.tar.xz' python3-colcon-argcomplete_0.3.3-1.debian.tar.xz 1612 SHA512:71ead0b0756a14fa54111a023c1c77ea9040c48e138f1076b630b351b1c59cf2991389b0811776ce979d9ca91887d69883b1208e3ef32c0a2e8518c6c53c7a4b
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-argcomplete/python3-colcon-argcomplete_0.3.3-1.dsc' python3-colcon-argcomplete_0.3.3-1.dsc 969 SHA512:f34a1b95c076c28bf9b45793f87818f21f5054421cbead38e59e1ceae1c37fa15ee21ddf33fb72e400fd731dd8c8918c3f32f34c6a2b83e4eaf05e85870ca038
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-argcomplete/python3-colcon-argcomplete_0.3.3.orig.tar.gz' python3-colcon-argcomplete_0.3.3.orig.tar.gz 7577 SHA512:fea054c099f8d950537ec34186e3ee05d2c514cc4680b958736ec4bf0e4cc4a4122f86a7581d2622dea0bd55fcc5c17b840bbf00c29bcbfb9f7af8a8868cea90
```

### `dpkg` source package: `python3-colcon-bash=0.4.2-1`

Binary Packages:

- `python3-colcon-bash=0.4.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-bash=0.4.2-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-bash/python3-colcon-bash_0.4.2-1.debian.tar.xz' python3-colcon-bash_0.4.2-1.debian.tar.xz 1076 SHA512:7cbe01513c86ad51fec1fc5626d22237c7316fcf4cd4f46028bcc0471184465f575299c4983d4aed3fa1c8ccd7690f8b0380bbddfb2a292e8057c3d820b89809
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-bash/python3-colcon-bash_0.4.2-1.dsc' python3-colcon-bash_0.4.2-1.dsc 906 SHA512:52864f34d65ae34f44921ce5215ced8cfa3886feecfa0e086a323eea8cad24d2436fa38caf3fc4311c0956356fb8f8b1654950cc55daf93a69531e794db2ed56
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-bash/python3-colcon-bash_0.4.2.orig.tar.gz' python3-colcon-bash_0.4.2.orig.tar.gz 5641 SHA512:81e6492d9a73a72751fd40cc0ecdbd23b15563ed7ede0b50ce9695b0fdc68465855396b56917b4089a4fe65ae8c7748737417345b4cda86a3c5ae18096809c07
```

### `dpkg` source package: `python3-colcon-cd=0.1.1-1`

Binary Packages:

- `python3-colcon-cd=0.1.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-cd=0.1.1-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-cd/python3-colcon-cd_0.1.1-1.debian.tar.xz' python3-colcon-cd_0.1.1-1.debian.tar.xz 1076 SHA512:19f3e96910d5fe2707a9b3a88e6bf5672f2f36f0a0e2153738088c42368a1ec3314ec44ea6308fc7b7831a6b104cb205b02a001b27dc649f8382854de5efee22
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-cd/python3-colcon-cd_0.1.1-1.dsc' python3-colcon-cd_0.1.1-1.dsc 888 SHA512:78a294acc17528efe01ac305576c9dda813bfdf88c1b9d58d2f31090d81b92b53942ca4d116ccaa746659b97f123da2c1d6ceace677aa20589e3e332caceed7e
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-cd/python3-colcon-cd_0.1.1.orig.tar.gz' python3-colcon-cd_0.1.1.orig.tar.gz 4215 SHA512:e6a212126570d8f459ffc1b46f796a6ec403e660ed7ed6bf3f965e3160c697888d9248a3f0253e4693c1183b99e861619383670e1c2ceca41962caea90d2c3bf
```

### `dpkg` source package: `python3-colcon-cmake=0.2.25-1`

Binary Packages:

- `python3-colcon-cmake=0.2.25-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-cmake=0.2.25-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-cmake/python3-colcon-cmake_0.2.25-1.debian.tar.xz' python3-colcon-cmake_0.2.25-1.debian.tar.xz 1096 SHA512:cca8553aca841709d2d353a072446a151e4c47f950abff05cf30012ab7d8474f7898bb914302aecfcbc5bac363cdd9a31299cc5c3ff69c0dab1ea2f819628dd8
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-cmake/python3-colcon-cmake_0.2.25-1.dsc' python3-colcon-cmake_0.2.25-1.dsc 925 SHA512:c1698c109375f061e1db949666e0558808c6d158540b11d93eced9f3526917cd59ba2aef643918c9ef137869ef1e2d09193dcf81d01f08a8222469a0b3d0df9e
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-cmake/python3-colcon-cmake_0.2.25.orig.tar.gz' python3-colcon-cmake_0.2.25.orig.tar.gz 17790 SHA512:e8ee9bbe33f19628316487878c1ca5863d6cd4af433f1e25d28f4878e0f08357196b601d1e04c31ecb6657dfa9e787cbe17bd3507f58b957dfa558600ceb7a8a
```

### `dpkg` source package: `python3-colcon-common-extensions=0.2.1-1`

Binary Packages:

- `python3-colcon-common-extensions=0.2.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-common-extensions=0.2.1-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-common-extensions/python3-colcon-common-extensions_0.2.1-1.debian.tar.xz' python3-colcon-common-extensions_0.2.1-1.debian.tar.xz 1204 SHA512:b5963a1f450299fa4a2c06caee7a7292e16844261641edf1315e5799f99aad5aa7be10f2b947cb62384f20a0b012107873aedfd6c932607501236c94d96f7bd9
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-common-extensions/python3-colcon-common-extensions_0.2.1-1.dsc' python3-colcon-common-extensions_0.2.1-1.dsc 1023 SHA512:d40498a4519032da4b2c11a2bfe7a79b4aeda3e622c75423546e76a6a89993a6dad62464b936d54fef2806bd3b3cbca23bee0fe66145e9af0d42531f3be5f6d6
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-common-extensions/python3-colcon-common-extensions_0.2.1.orig.tar.gz' python3-colcon-common-extensions_0.2.1.orig.tar.gz 1662 SHA512:df2c17decf64d3d6d5a3f78a53033b422b30cc89e6089da68f740bf78d3a99814e332c98b3a5b9b7ba6a7887f2f9a86567587edcdfa95575817217bdb8d42167
```

### `dpkg` source package: `python3-colcon-core=0.6.0-1`

Binary Packages:

- `python3-colcon-core=0.6.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-core=0.6.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-core/python3-colcon-core_0.6.0-1.debian.tar.xz' python3-colcon-core_0.6.0-1.debian.tar.xz 1580 SHA512:22736faa1305d9d87c919158c333d6224c250012d438554d8723c27ef3ecfe17b6e18854883aea5d349b45dc3d7e23fd85f36c74a0b672a98636230848b2c0ec
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-core/python3-colcon-core_0.6.0-1.dsc' python3-colcon-core_0.6.0-1.dsc 916 SHA512:d1f85811f1ddd3d5b03032c3675e4ddbfb52b6fb4cf91e7f65eee808225b5c855efd4495ba082ab20d2099c330c2fb094f2e5738351017e0a3b2b1a1882dfd38
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-core/python3-colcon-core_0.6.0.orig.tar.gz' python3-colcon-core_0.6.0.orig.tar.gz 102404 SHA512:feea5506033cbfe5f84bbd020b857f97c56fdc96d71029bd2cb76f3060a292260997b2d9844cb3bf2e1eca74c80d2303495d5729d3057e6d273f2cf4385c507c
```

### `dpkg` source package: `python3-colcon-defaults=0.2.5-1`

Binary Packages:

- `python3-colcon-defaults=0.2.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-defaults=0.2.5-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-defaults/python3-colcon-defaults_0.2.5-1.debian.tar.xz' python3-colcon-defaults_0.2.5-1.debian.tar.xz 1180 SHA512:c79395e205f6b8d39e4cbfc7792c4eddae0fd13f4f55b7f92a052c1613c48fac1eaced696ab996eebfd84ab118d6401ac0b4e5c7936377ca795e33ba3ba66a47
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-defaults/python3-colcon-defaults_0.2.5-1.dsc' python3-colcon-defaults_0.2.5-1.dsc 942 SHA512:00fbb831e6d16b1fa833c330fdf6c47d04930608c7ae92542a42bedb52b1916dd4ae868a914385d89d7725aefad12a7a15a3593ce1bdc79e84b4dff84b3265f7
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-defaults/python3-colcon-defaults_0.2.5.orig.tar.gz' python3-colcon-defaults_0.2.5.orig.tar.gz 5926 SHA512:683a13ac89a065462cefbb3fcc4ed809b23ff374ad8cc8c02853a721497b173d11da8b02674a02a818e9a78e684203861450dd91e73a8d5c7307efcc0133268d
```

### `dpkg` source package: `python3-colcon-devtools=0.2.2-1`

Binary Packages:

- `python3-colcon-devtools=0.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-devtools=0.2.2-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-devtools/python3-colcon-devtools_0.2.2-1.debian.tar.xz' python3-colcon-devtools_0.2.2-1.debian.tar.xz 1072 SHA512:2b0d5d8d57649c07e70ffa72d458bc034be4c3ae88bdb988c862bf7b95bf582d89a8732ca2a32bd8ee6f4b0a646a010e001245dcd1f74c7d385ae553166c4d80
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-devtools/python3-colcon-devtools_0.2.2-1.dsc' python3-colcon-devtools_0.2.2-1.dsc 942 SHA512:8abaeff2a306e0eac3ffe11131388ccf14f9dfda603a12f3e573c1020ef3bafe4fcd7f900f02518379dd3f7790a82a425720a952147e5d0c990bd5b1a7423737
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-devtools/python3-colcon-devtools_0.2.2.orig.tar.gz' python3-colcon-devtools_0.2.2.orig.tar.gz 4834 SHA512:44fb064a0f9bb58ab90e3440e68f11a457c676e000ecc57e51adb8fd0979d86beb4ec8669628c0c4c0fc46f2b28fba71e92a62129bb6907f697e9ff804964499
```

### `dpkg` source package: `python3-colcon-library-path=0.2.1-1`

Binary Packages:

- `python3-colcon-library-path=0.2.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-library-path=0.2.1-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-library-path/python3-colcon-library-path_0.2.1-1.debian.tar.xz' python3-colcon-library-path_0.2.1-1.debian.tar.xz 1000 SHA512:f0e4df16b6139d403f5fad5f581632eb5cd31df8ebc648c705d4da7c9eefdf6a005095e4301322cba03780114baff6d58e49f884cec6ac3ba2959ed4d638b292
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-library-path/python3-colcon-library-path_0.2.1-1.dsc' python3-colcon-library-path_0.2.1-1.dsc 1029 SHA512:3672203f9f0f35df233df0c54ac056fb37744be7ac56eab1d325d6b575b381b4816d07b59c4def12687dcc2e64ff627a4c012df3a9f23f7a031c6ec19f7b297d
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-library-path/python3-colcon-library-path_0.2.1.orig.tar.gz' python3-colcon-library-path_0.2.1.orig.tar.gz 3783 SHA512:60922210d6184263705493bd6764df4c3c7c07da3676217267452a339da35bece4ff308d2bd8db0446f363e53b54ddd068272f47fa99414bdccffef0c5cb36c6
```

### `dpkg` source package: `python3-colcon-metadata=0.2.5-1`

Binary Packages:

- `python3-colcon-metadata=0.2.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-metadata=0.2.5-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-metadata/python3-colcon-metadata_0.2.5-1.debian.tar.xz' python3-colcon-metadata_0.2.5-1.debian.tar.xz 1112 SHA512:ce98b0e24312a8e0ba11c2f01693448c5701a81aba8d6bb2f0a73679ef1ae0e94e5e75637271850c7f5a868f899cde49e9e9e025cc7cd63f057ac069239296a5
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-metadata/python3-colcon-metadata_0.2.5-1.dsc' python3-colcon-metadata_0.2.5-1.dsc 945 SHA512:17b64c85f88192dffc1b33542744a1a7f5fff0b68913cdd8259c4137c6f025c66e70fdaf54ed1356f1177abfd46cd64b108375ef99ef8c36fbd37c9ebb26de24
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-metadata/python3-colcon-metadata_0.2.5.orig.tar.gz' python3-colcon-metadata_0.2.5.orig.tar.gz 10846 SHA512:ba84f2c15a4981dfc0f4dbf10e68186705e8c3704e96182d620ff2f18971e5c145dfbdb1f04f71dacc18b262193c0c308ab39f113282974234e13a4a7dd77ef8
```

### `dpkg` source package: `python3-colcon-mixin=0.2.0-1`

Binary Packages:

- `python3-colcon-mixin=0.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-mixin=0.2.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-mixin/python3-colcon-mixin_0.2.0-1.debian.tar.xz' python3-colcon-mixin_0.2.0-1.debian.tar.xz 1120 SHA512:9067121ea29647355d03831b60ff31422963787725cc5d4975fb5b44f3224a236b6a145d63212003b1fd6a90931c0cdd0c44554cfea0908560bc491a4d199551
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-mixin/python3-colcon-mixin_0.2.0-1.dsc' python3-colcon-mixin_0.2.0-1.dsc 918 SHA512:e66b95dc58ad053e044dbb5cfa4b9ae0d573f129b2be43ec3727ba56054a0298cf8861a88349e9fff5bf449df7c193ef04257af5836f03a62782c211504c7171
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-mixin/python3-colcon-mixin_0.2.0.orig.tar.gz' python3-colcon-mixin_0.2.0.orig.tar.gz 12190 SHA512:e1ecbc113652394fd59b658ee4a09ac25681ec2c4ada64273fdf716c978765be76683cdcbde7ef1b957eb1c45f0a801781279c693b5a932e9a9e386b02fa645a
```

### `dpkg` source package: `python3-colcon-notification=0.2.13-1`

Binary Packages:

- `python3-colcon-notification=0.2.13-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-notification=0.2.13-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-notification/python3-colcon-notification_0.2.13-1.debian.tar.xz' python3-colcon-notification_0.2.13-1.debian.tar.xz 1596 SHA512:c2357d364eb5c8481d795e503005160f789a41556c34ad1046d5d7205cb7e6c2faaf09c71f4955a8c299017f73dfeb124eacdba95da72ea4ff62115be10108f6
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-notification/python3-colcon-notification_0.2.13-1.dsc' python3-colcon-notification_0.2.13-1.dsc 988 SHA512:22f3506620a501e67c9131bca8565c3137fe50a4ac0039adbec937ff1f0d9d0e2bca75e03e83e8e32cfa6f491ea62bfbcd66d3b277bfef20a5f4cb3d415f56c5
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-notification/python3-colcon-notification_0.2.13.orig.tar.gz' python3-colcon-notification_0.2.13.orig.tar.gz 54427 SHA512:b406b72b53085888c4a3393e4a3d01245828dca7bbf58679004a0fa0c14cad7cfd661b06360b66ade77dc11bd19c9d0108fc34a27cf03d7884bcbd9479a981fd
```

### `dpkg` source package: `python3-colcon-output=0.2.11-1`

Binary Packages:

- `python3-colcon-output=0.2.11-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-output=0.2.11-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-output/python3-colcon-output_0.2.11-1.debian.tar.xz' python3-colcon-output_0.2.11-1.debian.tar.xz 1068 SHA512:1e4099b156f6d2c495f00806c49824699c95273630bf276995c1b11d17399cc1311297f5cf6c22e86c09b7e3342ddbc604f98a236c619d07a9544b805c51216a
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-output/python3-colcon-output_0.2.11-1.dsc' python3-colcon-output_0.2.11-1.dsc 931 SHA512:a8015095b6d734030a9ae2e4a2f83683f8d2dedf2de4049153fdef97fac16a875a2d31020de0fb17bfb75b15c66fc12b70dce55bf957cb7d0de7e13048de5794
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-output/python3-colcon-output_0.2.11.orig.tar.gz' python3-colcon-output_0.2.11.orig.tar.gz 7706 SHA512:54bf354c3da6e23ca36849e6b4713264a8a918bfa14425a0c32557a9958dfd8ac3d6b104b401fc97937675b5072db33fcfd826e6e9dfd7c1ba69b57890d234fb
```

### `dpkg` source package: `python3-colcon-package-information=0.3.3-1`

Binary Packages:

- `python3-colcon-package-information=0.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-package-information=0.3.3-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-package-information/python3-colcon-package-information_0.3.3-1.debian.tar.xz' python3-colcon-package-information_0.3.3-1.debian.tar.xz 1072 SHA512:f15b4a25d26b8dd5bf27a6299d826e7079271b50f7c2530f2dd31d207fa8793d5717bf8da0f8f9aabd9840209d6e60300beb4b1b4c61ae20021c89923a88b0fd
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-package-information/python3-colcon-package-information_0.3.3-1.dsc' python3-colcon-package-information_0.3.3-1.dsc 1041 SHA512:04da1b58e811773dc724568f2cec9174689ea1c0f12c6576f461fa8b5d169ea7b60daf63ead44fa1c49103f33aa753d8aa0c4248dd891985b8e0cca1b4e21622
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-package-information/python3-colcon-package-information_0.3.3.orig.tar.gz' python3-colcon-package-information_0.3.3.orig.tar.gz 9863 SHA512:a98f6ac8cd41fc2d6b4bb6fdbebe7a4dbf12582cf103646ebde2d9b4d68df567fc056bda0c7ac0793c9ea9a206bfff48daabf551afbe73a614123d6d7bc6b803
```

### `dpkg` source package: `python3-colcon-package-selection=0.2.8-1`

Binary Packages:

- `python3-colcon-package-selection=0.2.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-package-selection=0.2.8-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-package-selection/python3-colcon-package-selection_0.2.8-1.debian.tar.xz' python3-colcon-package-selection_0.2.8-1.debian.tar.xz 1076 SHA512:6e7ab3c4b67bc6fa83765bc7ef9f58f03944be0c3fa0a6516382c4159d6eb8c7c20f475144ded2c9ec01560028b3dc2ce3f1f883a4b82c0b28c4c9f8202c45d5
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-package-selection/python3-colcon-package-selection_0.2.8-1.dsc' python3-colcon-package-selection_0.2.8-1.dsc 1023 SHA512:0918e7a235a281e6b9b1790a4cd13b945b31bb7ecc4e9a281a5248135404af44be2c681a06c1238e6e246015bb41cbc0a9801708595c8d0f256d70fed6cc7750
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-package-selection/python3-colcon-package-selection_0.2.8.orig.tar.gz' python3-colcon-package-selection_0.2.8.orig.tar.gz 8964 SHA512:485dcb8c2a5639f74d76206ce61b1f37d0c40a332b197d04b6bafe1baeed7f70c95f7f328b9d29e625dccd5081e91ce405261c40644de26bcb2aff31188e19b3
```

### `dpkg` source package: `python3-colcon-parallel-executor=0.2.4-1`

Binary Packages:

- `python3-colcon-parallel-executor=0.2.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-parallel-executor=0.2.4-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-parallel-executor/python3-colcon-parallel-executor_0.2.4-1.debian.tar.xz' python3-colcon-parallel-executor_0.2.4-1.debian.tar.xz 1068 SHA512:98570b66c1fedf3cb7ad95135d2968b86e5e0f680b7b150423d26ab403082a9c7772e7b33656fe59be947aea877c07e404e222e59ee6487106b6a8e7b7b6c599
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-parallel-executor/python3-colcon-parallel-executor_0.2.4-1.dsc' python3-colcon-parallel-executor_0.2.4-1.dsc 1023 SHA512:499b154e09e32168cf6d67fd0eb8f740e2f59b5852f3a76fcfeb6b72b42a82f4c2698bddfe9f0aa0e5fe3c73695d0f1c5ecc84f15273f830c4146f05f4c74f09
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-parallel-executor/python3-colcon-parallel-executor_0.2.4.orig.tar.gz' python3-colcon-parallel-executor_0.2.4.orig.tar.gz 5647 SHA512:a1e05a52e110485bfbfea6e27270dec5f735e7318c24615db8ca8468569cff26af27188b171c86458bd1e58da578b05828a2a5b614961e43097445a94fb67fed
```

### `dpkg` source package: `python3-colcon-pkg-config=0.1.0-1`

Binary Packages:

- `python3-colcon-pkg-config=0.1.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-pkg-config=0.1.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-pkg-config/python3-colcon-pkg-config_0.1.0-1.debian.tar.xz' python3-colcon-pkg-config_0.1.0-1.debian.tar.xz 984 SHA512:98a9ffd7457c80c063489f04a73e69acc4725d936c11b0666b64f1ba71e8ee51ac5d3b2ba2692ca057c84a3d27ebe966f68ab39f8958c6e60bb9fbec5d8e24d6
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-pkg-config/python3-colcon-pkg-config_0.1.0-1.dsc' python3-colcon-pkg-config_0.1.0-1.dsc 1008 SHA512:d42b9ff2a0c59744a6e9dce84b4c9b02ad2982119c8100bad5ec7fd6811ac81e61198ac9d0b7c131a500189b0d2450e45576598930c8af60ad67ad895784f58d
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-pkg-config/python3-colcon-pkg-config_0.1.0.orig.tar.gz' python3-colcon-pkg-config_0.1.0.orig.tar.gz 3408 SHA512:0f6df04ed403172f4a4922b0edb504a67e82d30e24e159dacfc3700dbe59f11862bb5f62a34a359e8a05d368259912a77a9cfd6084093a4c99d65b50b07608e1
```

### `dpkg` source package: `python3-colcon-powershell=0.3.6-1`

Binary Packages:

- `python3-colcon-powershell=0.3.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-powershell=0.3.6-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-powershell/python3-colcon-powershell_0.3.6-1.debian.tar.xz' python3-colcon-powershell_0.3.6-1.debian.tar.xz 1080 SHA512:b83c16cb866b45a823911c874914cc3991b8ee71f53ac7dbf6ef9dc85731e23153fce635ffbc4aa0ac99e9497ac404051421d29883f54471c60c45ce0ac152a6
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-powershell/python3-colcon-powershell_0.3.6-1.dsc' python3-colcon-powershell_0.3.6-1.dsc 960 SHA512:1be2c8b3a7e03af2dd5fab9d5d813a3bce9363b14a8f1604db528f5c47643a2c88c9ab8783ccd5670b8c79d76b083e00fa2bed2cc181209da3e01ed6c37c2b15
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-powershell/python3-colcon-powershell_0.3.6.orig.tar.gz' python3-colcon-powershell_0.3.6.orig.tar.gz 7168 SHA512:577b764a08f75d195ec39d13df86cb3af79d4747c38a7d018d3999b2aee4a0ae5e83ae2a0280dc81f1a9efab938d1f4c38175a582bef028f4f5f61dca9a6c9d4
```

### `dpkg` source package: `python3-colcon-python-setup-py=0.2.6-1`

Binary Packages:

- `python3-colcon-python-setup-py=0.2.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-python-setup-py=0.2.6-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-python-setup-py/python3-colcon-python-setup-py_0.2.6-1.debian.tar.xz' python3-colcon-python-setup-py_0.2.6-1.debian.tar.xz 1152 SHA512:85a5f1fcedbc92ce23730e7efe15fb6dd41a65eee2d343898c7f325e982df6c4289843e75fcfd96b8bcb9101181c715e49aa5d9c41498396768724febec0b505
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-python-setup-py/python3-colcon-python-setup-py_0.2.6-1.dsc' python3-colcon-python-setup-py_0.2.6-1.dsc 1005 SHA512:46ea600444049941b4fdf889b193da3dbd3c2d48ed72d62a45722c1e96001f8d2df015c79e2f3a7e719e5bc9899bf3a39a316e79c45e41c4874eaa0bf39d2748
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-python-setup-py/python3-colcon-python-setup-py_0.2.6.orig.tar.gz' python3-colcon-python-setup-py_0.2.6.orig.tar.gz 6794 SHA512:1ef245f9614b02b661d1aa226a8eeee61a1ef3a0e054b12625bc9b7fb07c3febef321e5c68115c204b714672cded54a211e0fb2a54a2bf78a8a9dd9b1fa2a9b0
```

### `dpkg` source package: `python3-colcon-recursive-crawl=0.2.1-1`

Binary Packages:

- `python3-colcon-recursive-crawl=0.2.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-recursive-crawl=0.2.1-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-recursive-crawl/python3-colcon-recursive-crawl_0.2.1-1.debian.tar.xz' python3-colcon-recursive-crawl_0.2.1-1.debian.tar.xz 1072 SHA512:aad1aafbd5ed8f2aa08bf79513c3c40929bafd4e10bbda2e1936a5a5a7e202b09b0beb81efdced49d80ab7aecba0e0bebf8489276636aef0798c4f7ddb23960d
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-recursive-crawl/python3-colcon-recursive-crawl_0.2.1-1.dsc' python3-colcon-recursive-crawl_0.2.1-1.dsc 1005 SHA512:763ecc90bdca9c57ba2fc15d22851071fdce0b92bb4b3b8c1b9bf5e25144417e86536b42ea04bcc7bccc68389cfd662da461ea1d6201cd138c386bd7fa6215b4
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-recursive-crawl/python3-colcon-recursive-crawl_0.2.1.orig.tar.gz' python3-colcon-recursive-crawl_0.2.1.orig.tar.gz 4100 SHA512:7af4783e49b1b59f961b710dd7dca307d169261d1a4d3d3e8538716905df01776dd8c806053f0d21996fb5f5f4c75a2c6e411a2538a7ccd17bf1eb3391ce7ea5
```

### `dpkg` source package: `python3-colcon-ros=0.3.19-1`

Binary Packages:

- `python3-colcon-ros=0.3.19-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-ros=0.3.19-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-ros/python3-colcon-ros_0.3.19-1.debian.tar.xz' python3-colcon-ros_0.3.19-1.debian.tar.xz 1568 SHA512:b77becafc284d1996804d0ae7ec9d1d578a4c7e093a20f5a92b9841881419a0fcd07efdd91b7038e9b8eb8d5df4bc321c46aaf1fd270b74e98379f008f83c222
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-ros/python3-colcon-ros_0.3.19-1.dsc' python3-colcon-ros_0.3.19-1.dsc 907 SHA512:3560e69bc2c6952893b96a034dd08289391aed2abc6a014f0f3e746f4cf3d41c6f36b3709b1dff6098dd414026b5e1d133276a1471a067e11299f8c51810ca75
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-ros/python3-colcon-ros_0.3.19.orig.tar.gz' python3-colcon-ros_0.3.19.orig.tar.gz 14135 SHA512:2e96195a89f1211ff97ce075ecc2bc71adc0d87bf61bbaf40050a8e77a43989878f808600512aadaeea5d3a1c61554a1efc039a031261682d428615c485d9c88
```

### `dpkg` source package: `python3-colcon-test-result=0.3.8-1`

Binary Packages:

- `python3-colcon-test-result=0.3.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-test-result=0.3.8-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-test-result/python3-colcon-test-result_0.3.8-1.debian.tar.xz' python3-colcon-test-result_0.3.8-1.debian.tar.xz 1076 SHA512:a53a5a1415b08a053b783dd9052b601c316b0e277511c2b5f995baf51cf19011f535811efe8d066b68c57f133e44fc364a2d2bd02d5a3e15dcdad6d5fcd329b6
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-test-result/python3-colcon-test-result_0.3.8-1.dsc' python3-colcon-test-result_0.3.8-1.dsc 969 SHA512:44515222f5c096d7e076bbc9c6911316bd4d09b47402983e9d0b4a34eff440a37565a494930a28146fcd2404b0ee6e26c36c647d8dec9fce464d30acc3e6f86c
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-test-result/python3-colcon-test-result_0.3.8.orig.tar.gz' python3-colcon-test-result_0.3.8.orig.tar.gz 8075 SHA512:c54342d8cdbd71255510510a71bbbd29664469368553d133ecfd7f67cf04ccbc8e07fa25bc62474114450020a40b4271d7048a2382380d641bcf0f8e1445b8d6
```

### `dpkg` source package: `python3-colcon-zsh=0.4.0-1`

Binary Packages:

- `python3-colcon-zsh=0.4.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-zsh=0.4.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-zsh/python3-colcon-zsh_0.4.0-1.debian.tar.xz' python3-colcon-zsh_0.4.0-1.debian.tar.xz 1076 SHA512:3edcc749368472a4b77cb15cf8281286b11ed536254d7b4b40b08da33f703efa49ee997f8def1191e6df45f91d0ed61fdf00f69e7b3ac7d660c6e7c58b8cba1b
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-zsh/python3-colcon-zsh_0.4.0-1.dsc' python3-colcon-zsh_0.4.0-1.dsc 897 SHA512:1895a2b60e11448c282bb48a5cd98a66d1c8f655ffe3d7ad3b7e0b033daa902fbcad0c605b73c00a21d1e3ea0e9bf8cb04ecf25b0d16530e30c46e9d12829485
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-colcon-zsh/python3-colcon-zsh_0.4.0.orig.tar.gz' python3-colcon-zsh_0.4.0.orig.tar.gz 5654 SHA512:dafb711ecd6a8411147d592b064011efd8db4666e8cc8358243841f46cc3aa5427a7a56b1b7e4f71d27b5f88e401f4556d7d26e7af26074d83e68d9dfffae35a
```

### `dpkg` source package: `python3-defaults=3.6.7-1~18.04`

Binary Packages:

- `libpython3-dev:amd64=3.6.7-1~18.04`
- `libpython3-stdlib:amd64=3.6.7-1~18.04`
- `python3=3.6.7-1~18.04`
- `python3-dev=3.6.7-1~18.04`
- `python3-minimal=3.6.7-1~18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.6.7-1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.dsc' python3-defaults_3.6.7-1~18.04.dsc 2896 SHA256:a4dad3f3681c698e3f1232a4e56934877954e39c21e330f4491ba8e916bb1655
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.tar.gz' python3-defaults_3.6.7-1~18.04.tar.gz 137600 SHA256:df14f4993ac87537415f1abaa69d80790fb01e51033416bc123038f731286ed4
```

### `dpkg` source package: `python3-rosdistro-modules=0.8.2-1`

Binary Packages:

- `python3-rosdistro-modules=0.8.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rosdistro-modules=0.8.2-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdistro-modules/python3-rosdistro-modules_0.8.2-1.debian.tar.xz' python3-rosdistro-modules_0.8.2-1.debian.tar.xz 1980 SHA512:4fbd28a6fee4ffe5a6c004da0f32725c8a229ea981e4031cc7693704749239c53c250c56330e7face22a8415d9c4e4b9b54638547443d54fa8c327211a632634
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdistro-modules/python3-rosdistro-modules_0.8.2-1.dsc' python3-rosdistro-modules_0.8.2-1.dsc 969 SHA512:b30384e5c7e2c29dc589879e39385ead1fbe532fd370fcb54f1f4da83fe6161acedc57a9f0c3e22d676d2e4ea4e320b060d3564b08f53eba096275ca9c744a18
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdistro-modules/python3-rosdistro-modules_0.8.2.orig.tar.gz' python3-rosdistro-modules_0.8.2.orig.tar.gz 44116 SHA512:5137d83d0cc6b689fabae2cd22d17cfe303b98883fca7bbc78d6aeee4f9a10bfcafa8e72190111c8dd709e88aa25ae6f2435e995a63ca55283b1656eb0f138a5
```

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

### `dpkg` source package: `python3-stdlib-extensions=3.6.9-1~18.04`

Binary Packages:

- `python3-distutils=3.6.9-1~18.04`
- `python3-lib2to3=3.6.9-1~18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.6.9-1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.6.9-1~18.04.dsc' python3-stdlib-extensions_3.6.9-1~18.04.dsc 2624 SHA256:9e5055cbfdf3e0e904ff12788090e1df88182f6eb178aca0551cbd0fef9f059c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.6.9.orig.tar.bz2' python3-stdlib-extensions_3.6.9.orig.tar.bz2 4237908 SHA256:124756562de67dda09de9d992d69f7f8bcdbcc04f155f71ebf81a22dcfb77984
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.6.9-1~18.04.debian.tar.xz' python3-stdlib-extensions_3.6.9-1~18.04.debian.tar.xz 16908 SHA256:befdd346165a9baa7fc42b54c24db9b975870651c9578b03d0511e0b77578f84
```

### `dpkg` source package: `python3-vcstool=0.2.14-1`

Binary Packages:

- `python3-vcstool=0.2.14-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-vcstool=0.2.14-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-vcstool/python3-vcstool_0.2.14-1.debian.tar.xz' python3-vcstool_0.2.14-1.debian.tar.xz 1112 SHA512:62528247129c614b0093fac31c3ea038db3accae9e3ccd3ebafaf43871ac26805ae3fcbd8a135a7121788bc58d489f61ee0a429ea44d07da5f8ac90979b4f23d
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-vcstool/python3-vcstool_0.2.14-1.dsc' python3-vcstool_0.2.14-1.dsc 884 SHA512:e14f2c556f1e68f40e77b0004605844e0ee5ce577b65ddce444f8f0f5dbb91a706fc3f20693e8994cac63e599ba28fe14623026e247944c41bf2e5f07bca8118
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-vcstool/python3-vcstool_0.2.14.orig.tar.gz' python3-vcstool_0.2.14.orig.tar.gz 31698 SHA512:1f8470422fa2f2a733ea593c3df2533b1e61c1b2ba37e106997ed7ea1f301e2d0ddb865c4931c084f86164b8b754858d8394b45540c4546f4bd9e1a97028edbe
```

### `dpkg` source package: `python3.6=3.6.9-1~18.04ubuntu1.1`

Binary Packages:

- `libpython3.6:amd64=3.6.9-1~18.04ubuntu1.1`
- `libpython3.6-dev:amd64=3.6.9-1~18.04ubuntu1.1`
- `libpython3.6-minimal:amd64=3.6.9-1~18.04ubuntu1.1`
- `libpython3.6-stdlib:amd64=3.6.9-1~18.04ubuntu1.1`
- `python3.6=3.6.9-1~18.04ubuntu1.1`
- `python3.6-dev=3.6.9-1~18.04ubuntu1.1`
- `python3.6-minimal=3.6.9-1~18.04ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libpython3.6/copyright`, `/usr/share/doc/libpython3.6-dev/copyright`, `/usr/share/doc/libpython3.6-minimal/copyright`, `/usr/share/doc/libpython3.6-stdlib/copyright`, `/usr/share/doc/python3.6/copyright`, `/usr/share/doc/python3.6-dev/copyright`, `/usr/share/doc/python3.6-minimal/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris python3.6=3.6.9-1~18.04ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9-1~18.04ubuntu1.1.dsc' python3.6_3.6.9-1~18.04ubuntu1.1.dsc 3470 SHA256:e780132c4fd5341e24b354d7ca37fb3d5d22f4178c1a180c0f530b18c9586e30
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9.orig.tar.xz' python3.6_3.6.9.orig.tar.xz 17212164 SHA256:5e2f5f554e3f8f7f0296f7e73d8600c4e9acbaee6b2555b83206edf5153870da
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9-1~18.04ubuntu1.1.debian.tar.xz' python3.6_3.6.9-1~18.04ubuntu1.1.debian.tar.xz 218936 SHA256:63afea0ff02387fb269d4e96a1732b0ba42740d1f7046f75d5cfcbfd719459e7
```

### `dpkg` source package: `pyyaml=3.12-1build2`

Binary Packages:

- `python-yaml=3.12-1build2`
- `python3-yaml=3.12-1build2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pyyaml=3.12-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_3.12-1build2.dsc' pyyaml_3.12-1build2.dsc 2301 SHA256:05dadbe75f65a9989490de951abf10889e9113cf345e0eb9bf09e65febe5021d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_3.12.orig.tar.gz' pyyaml_3.12.orig.tar.gz 253011 SHA256:592766c6303207a20efc445587778322d7f73b161bd994f227adaa341ba212ab
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_3.12-1build2.debian.tar.xz' pyyaml_3.12-1build2.debian.tar.xz 7272 SHA256:ecaaf2c0725aaa0573ca24f5f477da76af7f3b281e90e2f04496fe4bc86a298b
```

### `dpkg` source package: `rdma-core=17.1-1ubuntu0.2`

Binary Packages:

- `ibverbs-providers:amd64=17.1-1ubuntu0.2`
- `libibverbs-dev:amd64=17.1-1ubuntu0.2`
- `libibverbs1:amd64=17.1-1ubuntu0.2`
- `librdmacm1:amd64=17.1-1ubuntu0.2`

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
$ apt-get source -qq --print-uris rdma-core=17.1-1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rdma-core/rdma-core_17.1-1ubuntu0.2.dsc' rdma-core_17.1-1ubuntu0.2.dsc 2762 SHA256:e0662733332aa3953a389dd9631f3a3480b93f992cb378bb76d008743de89c2f
'http://archive.ubuntu.com/ubuntu/pool/main/r/rdma-core/rdma-core_17.1.orig.tar.gz' rdma-core_17.1.orig.tar.gz 1027903 SHA256:b47444b7c05d3906deb8771eec3e634984dd83f5e620d5e37d3a83f74f0cc1ba
'http://archive.ubuntu.com/ubuntu/pool/main/r/rdma-core/rdma-core_17.1-1ubuntu0.2.debian.tar.xz' rdma-core_17.1-1ubuntu0.2.debian.tar.xz 18696 SHA256:d9e7d151be854278f61db12e7348cbd58cffcc2bb25674693b50b7c726b11b72
```

### `dpkg` source package: `readline=7.0-3`

Binary Packages:

- `libreadline7:amd64=7.0-3`
- `readline-common=7.0-3`

Licenses: (parsed from: `/usr/share/doc/libreadline7/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=7.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0-3.dsc' readline_7.0-3.dsc 2538 SHA256:f27a5dc9053b88641e3effc6c03b7840cbbbd887e8dcaf05d9e336c7bc7c6a53
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0.orig.tar.gz' readline_7.0.orig.tar.gz 2910016 SHA256:750d437185286f40a369e1e4f4764eda932b9459b5ec9a731628393dd3d32334
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0-3.debian.tar.xz' readline_7.0-3.debian.tar.xz 30012 SHA256:bf166310d6ca7716f2bd0e9e06cee2458b0157f7989d028730fc305643560175
```

### `dpkg` source package: `rhash=1.3.6-2`

Binary Packages:

- `librhash0:amd64=1.3.6-2`

Licenses: (parsed from: `/usr/share/doc/librhash0/copyright`)

- `RHash`

Source:

```console
$ apt-get source -qq --print-uris rhash=1.3.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.3.6-2.dsc' rhash_1.3.6-2.dsc 1747 SHA256:57e77023e0c769513949dec63b2d0d7368a47b048367d7d252f80b91257c8843
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.3.6.orig.tar.gz' rhash_1.3.6.orig.tar.gz 328097 SHA256:964df972b60569b5cb35ec989ced195ab8ea514fc46a74eab98e86569ffbcf92
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.3.6-2.debian.tar.xz' rhash_1.3.6-2.debian.tar.xz 9672 SHA256:fcccfa3d3a5a7ac16395ec54fcfb4217a5ccf5718e762f3670276366061e5638
```

### `dpkg` source package: `ros-dashing-action-msgs=0.7.4-1bionic.20200711.054724`

Binary Packages:

- `ros-dashing-action-msgs=0.7.4-1bionic.20200711.054724`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-actionlib-msgs=0.7.0-1bionic.20200711.061553`

Binary Packages:

- `ros-dashing-actionlib-msgs=0.7.0-1bionic.20200711.061553`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-auto=0.7.5-1bionic.20200711.044927`

Binary Packages:

- `ros-dashing-ament-cmake-auto=0.7.5-1bionic.20200711.044927`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-copyright=0.7.12-1bionic.20200711.045213`

Binary Packages:

- `ros-dashing-ament-cmake-copyright=0.7.12-1bionic.20200711.045213`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-core=0.7.5-1bionic.20200711.043737`

Binary Packages:

- `ros-dashing-ament-cmake-core=0.7.5-1bionic.20200711.043737`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-cppcheck=0.7.12-1bionic.20200711.045333`

Binary Packages:

- `ros-dashing-ament-cmake-cppcheck=0.7.12-1bionic.20200711.045333`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-cpplint=0.7.12-1bionic.20200711.045352`

Binary Packages:

- `ros-dashing-ament-cmake-cpplint=0.7.12-1bionic.20200711.045352`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-export-definitions=0.7.5-1bionic.20200711.044202`

Binary Packages:

- `ros-dashing-ament-cmake-export-definitions=0.7.5-1bionic.20200711.044202`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-export-dependencies=0.7.5-1bionic.20200711.044333`

Binary Packages:

- `ros-dashing-ament-cmake-export-dependencies=0.7.5-1bionic.20200711.044333`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-export-include-directories=0.7.5-1bionic.20200711.044217`

Binary Packages:

- `ros-dashing-ament-cmake-export-include-directories=0.7.5-1bionic.20200711.044217`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-export-interfaces=0.7.5-1bionic.20200711.044352`

Binary Packages:

- `ros-dashing-ament-cmake-export-interfaces=0.7.5-1bionic.20200711.044352`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-export-libraries=0.7.5-1bionic.20200711.044220`

Binary Packages:

- `ros-dashing-ament-cmake-export-libraries=0.7.5-1bionic.20200711.044220`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-export-link-flags=0.7.5-1bionic.20200711.044130`

Binary Packages:

- `ros-dashing-ament-cmake-export-link-flags=0.7.5-1bionic.20200711.044130`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-flake8=0.7.12-1bionic.20200711.045420`

Binary Packages:

- `ros-dashing-ament-cmake-flake8=0.7.12-1bionic.20200711.045420`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-gmock=0.7.5-1bionic.20200711.050015`

Binary Packages:

- `ros-dashing-ament-cmake-gmock=0.7.5-1bionic.20200711.050015`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-gtest=0.7.5-1bionic.20200711.045821`

Binary Packages:

- `ros-dashing-ament-cmake-gtest=0.7.5-1bionic.20200711.045821`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-include-directories=0.7.5-1bionic.20200711.044227`

Binary Packages:

- `ros-dashing-ament-cmake-include-directories=0.7.5-1bionic.20200711.044227`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-libraries=0.7.5-1bionic.20200711.044210`

Binary Packages:

- `ros-dashing-ament-cmake-libraries=0.7.5-1bionic.20200711.044210`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-lint-cmake=0.7.12-1bionic.20200711.045055`

Binary Packages:

- `ros-dashing-ament-cmake-lint-cmake=0.7.12-1bionic.20200711.045055`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-pep257=0.7.12-1bionic.20200711.045449`

Binary Packages:

- `ros-dashing-ament-cmake-pep257=0.7.12-1bionic.20200711.045449`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-pytest=0.7.5-1bionic.20200711.044539`

Binary Packages:

- `ros-dashing-ament-cmake-pytest=0.7.5-1bionic.20200711.044539`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-python=0.7.5-1bionic.20200711.044144`

Binary Packages:

- `ros-dashing-ament-cmake-python=0.7.5-1bionic.20200711.044144`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-ros=0.7.0-1bionic.20200711.050118`

Binary Packages:

- `ros-dashing-ament-cmake-ros=0.7.0-1bionic.20200711.050118`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-target-dependencies=0.7.5-1bionic.20200711.044400`

Binary Packages:

- `ros-dashing-ament-cmake-target-dependencies=0.7.5-1bionic.20200711.044400`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-test=0.7.5-1bionic.20200711.044300`

Binary Packages:

- `ros-dashing-ament-cmake-test=0.7.5-1bionic.20200711.044300`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-uncrustify=0.7.12-1bionic.20200711.045844`

Binary Packages:

- `ros-dashing-ament-cmake-uncrustify=0.7.12-1bionic.20200711.045844`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake-xmllint=0.7.12-1bionic.20200711.045511`

Binary Packages:

- `ros-dashing-ament-cmake-xmllint=0.7.12-1bionic.20200711.045511`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cmake=0.7.5-1bionic.20200711.044555`

Binary Packages:

- `ros-dashing-ament-cmake=0.7.5-1bionic.20200711.044555`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-copyright=0.7.12-1bionic.20200711.044624`

Binary Packages:

- `ros-dashing-ament-copyright=0.7.12-1bionic.20200711.044624`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cppcheck=0.7.12-1bionic.20200711.044234`

Binary Packages:

- `ros-dashing-ament-cppcheck=0.7.12-1bionic.20200711.044234`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-cpplint=0.7.12-1bionic.20200711.044933`

Binary Packages:

- `ros-dashing-ament-cpplint=0.7.12-1bionic.20200711.044933`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-flake8=0.7.12-1bionic.20200711.044312`

Binary Packages:

- `ros-dashing-ament-flake8=0.7.12-1bionic.20200711.044312`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-index-cpp=0.7.2-1bionic.20200711.050118`

Binary Packages:

- `ros-dashing-ament-index-cpp=0.7.2-1bionic.20200711.050118`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-index-python=0.7.2-1bionic.20200711.044628`

Binary Packages:

- `ros-dashing-ament-index-python=0.7.2-1bionic.20200711.044628`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-lint-auto=0.7.12-1bionic.20200711.044542`

Binary Packages:

- `ros-dashing-ament-lint-auto=0.7.12-1bionic.20200711.044542`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-lint-cmake=0.7.12-1bionic.20200711.044943`

Binary Packages:

- `ros-dashing-ament-lint-cmake=0.7.12-1bionic.20200711.044943`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-lint-common=0.7.12-1bionic.20200711.045936`

Binary Packages:

- `ros-dashing-ament-lint-common=0.7.12-1bionic.20200711.045936`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-lint=0.7.12-1bionic.20200711.044155`

Binary Packages:

- `ros-dashing-ament-lint=0.7.12-1bionic.20200711.044155`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-package=0.7.3-1bionic.20191011.215024`

Binary Packages:

- `ros-dashing-ament-package=0.7.3-1bionic.20191011.215024`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-pep257=0.7.12-1bionic.20200711.044439`

Binary Packages:

- `ros-dashing-ament-pep257=0.7.12-1bionic.20200711.044439`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-uncrustify=0.7.12-1bionic.20200711.045803`

Binary Packages:

- `ros-dashing-ament-uncrustify=0.7.12-1bionic.20200711.045803`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ament-xmllint=0.7.12-1bionic.20200711.045010`

Binary Packages:

- `ros-dashing-ament-xmllint=0.7.12-1bionic.20200711.045010`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-builtin-interfaces=0.7.4-1bionic.20200711.054125`

Binary Packages:

- `ros-dashing-builtin-interfaces=0.7.4-1bionic.20200711.054125`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-class-loader=1.3.3-1bionic.20200711.050139`

Binary Packages:

- `ros-dashing-class-loader=1.3.3-1bionic.20200711.050139`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-common-interfaces=0.7.0-1bionic.20200711.065909`

Binary Packages:

- `ros-dashing-common-interfaces=0.7.0-1bionic.20200711.065909`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-composition-interfaces=0.7.4-1bionic.20200711.055709`

Binary Packages:

- `ros-dashing-composition-interfaces=0.7.4-1bionic.20200711.055709`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-console-bridge-vendor=1.2.0-1bionic.20200711.045109`

Binary Packages:

- `ros-dashing-console-bridge-vendor=1.2.0-1bionic.20200711.045109`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-demo-nodes-cpp=0.7.9-1bionic.20200711.114608`

Binary Packages:

- `ros-dashing-demo-nodes-cpp=0.7.9-1bionic.20200711.114608`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-demo-nodes-py=0.7.9-1bionic.20200711.114149`

Binary Packages:

- `ros-dashing-demo-nodes-py=0.7.9-1bionic.20200711.114149`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-diagnostic-msgs=0.7.0-1bionic.20200711.062733`

Binary Packages:

- `ros-dashing-diagnostic-msgs=0.7.0-1bionic.20200711.062733`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-eigen3-cmake-module=0.1.1-1bionic.20200711.045524`

Binary Packages:

- `ros-dashing-eigen3-cmake-module=0.1.1-1bionic.20200711.045524`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-example-interfaces=0.7.1-1bionic.20200711.055210`

Binary Packages:

- `ros-dashing-example-interfaces=0.7.1-1bionic.20200711.055210`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-fastcdr=1.0.11-1bionic.20200711.044347`

Binary Packages:

- `ros-dashing-fastcdr=1.0.11-1bionic.20200711.044347`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-fastrtps-cmake-module=0.7.1-1bionic.20200711.050614`

Binary Packages:

- `ros-dashing-fastrtps-cmake-module=0.7.1-1bionic.20200711.050614`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-fastrtps=1.8.2-1bionic.20200711.044545`

Binary Packages:

- `ros-dashing-fastrtps=1.8.2-1bionic.20200711.044545`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-gazebo-msgs=3.3.5-3bionic.20200711.064545`

Binary Packages:

- `ros-dashing-gazebo-msgs=3.3.5-3bionic.20200711.064545`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-geometry-msgs=0.7.0-1bionic.20200711.061011`

Binary Packages:

- `ros-dashing-geometry-msgs=0.7.0-1bionic.20200711.061011`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-gmock-vendor=1.8.9000-1bionic.20200711.045931`

Binary Packages:

- `ros-dashing-gmock-vendor=1.8.9000-1bionic.20200711.045931`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-gtest-vendor=1.8.9000-1bionic.20200711.044523`

Binary Packages:

- `ros-dashing-gtest-vendor=1.8.9000-1bionic.20200711.044523`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-kdl-parser=2.2.1-1bionic.20200721.211423`

Binary Packages:

- `ros-dashing-kdl-parser=2.2.1-1bionic.20200721.211423`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-launch-ros=0.8.8-1bionic.20200711.113914`

Binary Packages:

- `ros-dashing-launch-ros=0.8.8-1bionic.20200711.113914`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-launch=0.8.7-1bionic.20200711.045812`

Binary Packages:

- `ros-dashing-launch=0.8.7-1bionic.20200711.045812`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-libyaml-vendor=1.0.0-1bionic.20200711.045238`

Binary Packages:

- `ros-dashing-libyaml-vendor=1.0.0-1bionic.20200711.045238`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-lifecycle-msgs=0.7.4-1bionic.20200711.054321`

Binary Packages:

- `ros-dashing-lifecycle-msgs=0.7.4-1bionic.20200711.054321`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-message-filters=3.1.3-1bionic.20200711.114538`

Binary Packages:

- `ros-dashing-message-filters=3.1.3-1bionic.20200711.114538`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-nav-msgs=0.7.0-1bionic.20200711.063052`

Binary Packages:

- `ros-dashing-nav-msgs=0.7.0-1bionic.20200711.063052`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-orocos-kdl=3.2.2-1bionic.20200711.045705`

Binary Packages:

- `ros-dashing-orocos-kdl=3.2.2-1bionic.20200711.045705`

Licenses: (parsed from: `/usr/share/doc/ros-dashing-orocos-kdl/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-osrf-pycommon=0.1.9-1bionic.20200711.044610`

Binary Packages:

- `ros-dashing-osrf-pycommon=0.1.9-1bionic.20200711.044610`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-pluginlib=2.3.3-1bionic.20200711.051616`

Binary Packages:

- `ros-dashing-pluginlib=2.3.3-1bionic.20200711.051616`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-poco-vendor=1.2.0-1bionic.20200711.050022`

Binary Packages:

- `ros-dashing-poco-vendor=1.2.0-1bionic.20200711.050022`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-python-cmake-module=0.7.10-1bionic.20200711.050632`

Binary Packages:

- `ros-dashing-python-cmake-module=0.7.10-1bionic.20200711.050632`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcl-action=0.7.9-1bionic.20200711.113149`

Binary Packages:

- `ros-dashing-rcl-action=0.7.9-1bionic.20200711.113149`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcl-interfaces=0.7.4-1bionic.20200711.055224`

Binary Packages:

- `ros-dashing-rcl-interfaces=0.7.4-1bionic.20200711.055224`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcl-lifecycle=0.7.9-1bionic.20200711.113014`

Binary Packages:

- `ros-dashing-rcl-lifecycle=0.7.9-1bionic.20200711.113014`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcl-logging-noop=0.2.1-1bionic.20200711.051451`

Binary Packages:

- `ros-dashing-rcl-logging-noop=0.2.1-1bionic.20200711.051451`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcl-yaml-param-parser=0.7.9-1bionic.20200711.113149`

Binary Packages:

- `ros-dashing-rcl-yaml-param-parser=0.7.9-1bionic.20200711.113149`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcl=0.7.9-1bionic.20200711.112814`

Binary Packages:

- `ros-dashing-rcl=0.7.9-1bionic.20200711.112814`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rclcpp-components=0.7.14-1bionic.20200711.120320`

Binary Packages:

- `ros-dashing-rclcpp-components=0.7.14-1bionic.20200711.120320`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rclcpp-lifecycle=0.7.14-1bionic.20200711.114551`

Binary Packages:

- `ros-dashing-rclcpp-lifecycle=0.7.14-1bionic.20200711.114551`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rclcpp=0.7.14-1bionic.20200711.114140`

Binary Packages:

- `ros-dashing-rclcpp=0.7.14-1bionic.20200711.114140`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rclpy=0.7.11-1bionic.20200711.113636`

Binary Packages:

- `ros-dashing-rclpy=0.7.11-1bionic.20200711.113636`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcpputils=0.1.1-1bionic.20200711.050650`

Binary Packages:

- `ros-dashing-rcpputils=0.1.1-1bionic.20200711.050650`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rcutils=0.7.5-1bionic.20200711.051002`

Binary Packages:

- `ros-dashing-rcutils=0.7.5-1bionic.20200711.051002`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rmw-fastrtps-cpp=0.7.7-1bionic.20200711.052656`

Binary Packages:

- `ros-dashing-rmw-fastrtps-cpp=0.7.7-1bionic.20200711.052656`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rmw-fastrtps-shared-cpp=0.7.7-1bionic.20200711.052022`

Binary Packages:

- `ros-dashing-rmw-fastrtps-shared-cpp=0.7.7-1bionic.20200711.052022`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rmw-implementation-cmake=0.7.2-1bionic.20200711.050826`

Binary Packages:

- `ros-dashing-rmw-implementation-cmake=0.7.2-1bionic.20200711.050826`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rmw-implementation=0.7.2-1bionic.20200711.053058`

Binary Packages:

- `ros-dashing-rmw-implementation=0.7.2-1bionic.20200711.053058`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rmw=0.7.2-1bionic.20200711.051928`

Binary Packages:

- `ros-dashing-rmw=0.7.2-1bionic.20200711.051928`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-robot-state-publisher=2.2.5-1bionic.20200721.211546`

Binary Packages:

- `ros-dashing-robot-state-publisher=2.2.5-1bionic.20200721.211546`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros-base=0.7.4-1bionic.20200721.211852`

Binary Packages:

- `ros-dashing-ros-base=0.7.4-1bionic.20200721.211852`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros-core=0.7.4-1bionic.20200711.120803`

Binary Packages:

- `ros-dashing-ros-core=0.7.4-1bionic.20200711.120803`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros-environment=2.3.0-1bionic.20200711.051124`

Binary Packages:

- `ros-dashing-ros-environment=2.3.0-1bionic.20200711.051124`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros-workspace=0.7.2-1bionic.20200711.043848`

Binary Packages:

- `ros-dashing-ros-workspace=0.7.2-1bionic.20200711.043848`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros1-bridge=0.7.6-1bionic.20200711.115032`

Binary Packages:

- `ros-dashing-ros1-bridge=0.7.6-1bionic.20200711.115032`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2action=0.7.11-1bionic.20200711.114107`

Binary Packages:

- `ros-dashing-ros2action=0.7.11-1bionic.20200711.114107`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2cli=0.7.11-1bionic.20200711.113941`

Binary Packages:

- `ros-dashing-ros2cli=0.7.11-1bionic.20200711.113941`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2component=0.7.11-1bionic.20200711.120638`

Binary Packages:

- `ros-dashing-ros2component=0.7.11-1bionic.20200711.120638`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2launch=0.8.8-1bionic.20200711.114636`

Binary Packages:

- `ros-dashing-ros2launch=0.8.8-1bionic.20200711.114636`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2lifecycle=0.7.11-1bionic.20200711.114804`

Binary Packages:

- `ros-dashing-ros2lifecycle=0.7.11-1bionic.20200711.114804`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2msg=0.7.11-1bionic.20200711.114340`

Binary Packages:

- `ros-dashing-ros2msg=0.7.11-1bionic.20200711.114340`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2multicast=0.7.11-1bionic.20200711.114401`

Binary Packages:

- `ros-dashing-ros2multicast=0.7.11-1bionic.20200711.114401`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2node=0.7.11-1bionic.20200711.114409`

Binary Packages:

- `ros-dashing-ros2node=0.7.11-1bionic.20200711.114409`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2param=0.7.11-1bionic.20200711.114818`

Binary Packages:

- `ros-dashing-ros2param=0.7.11-1bionic.20200711.114818`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2pkg=0.7.11-1bionic.20200711.114417`

Binary Packages:

- `ros-dashing-ros2pkg=0.7.11-1bionic.20200711.114417`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2run=0.7.11-1bionic.20200711.114657`

Binary Packages:

- `ros-dashing-ros2run=0.7.11-1bionic.20200711.114657`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2service=0.7.11-1bionic.20200711.114612`

Binary Packages:

- `ros-dashing-ros2service=0.7.11-1bionic.20200711.114612`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2srv=0.7.11-1bionic.20200711.114424`

Binary Packages:

- `ros-dashing-ros2srv=0.7.11-1bionic.20200711.114424`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-ros2topic=0.7.11-1bionic.20200711.114558`

Binary Packages:

- `ros-dashing-ros2topic=0.7.11-1bionic.20200711.114558`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosgraph-msgs=0.7.4-1bionic.20200711.054525`

Binary Packages:

- `ros-dashing-rosgraph-msgs=0.7.4-1bionic.20200711.054525`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-adapter=0.7.9-1bionic.20200711.050824`

Binary Packages:

- `ros-dashing-rosidl-adapter=0.7.9-1bionic.20200711.050824`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-cmake=0.7.9-1bionic.20200711.051231`

Binary Packages:

- `ros-dashing-rosidl-cmake=0.7.9-1bionic.20200711.051231`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-default-generators=0.7.0-1bionic.20200711.053709`

Binary Packages:

- `ros-dashing-rosidl-default-generators=0.7.0-1bionic.20200711.053709`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-default-runtime=0.7.0-1bionic.20200711.053702`

Binary Packages:

- `ros-dashing-rosidl-default-runtime=0.7.0-1bionic.20200711.053702`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-generator-c=0.7.9-1bionic.20200711.051612`

Binary Packages:

- `ros-dashing-rosidl-generator-c=0.7.9-1bionic.20200711.051612`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-generator-cpp=0.7.9-1bionic.20200711.051937`

Binary Packages:

- `ros-dashing-rosidl-generator-cpp=0.7.9-1bionic.20200711.051937`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-generator-py=0.7.10-1bionic.20200711.053530`

Binary Packages:

- `ros-dashing-rosidl-generator-py=0.7.10-1bionic.20200711.053530`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-parser=0.7.9-1bionic.20200711.051046`

Binary Packages:

- `ros-dashing-rosidl-parser=0.7.9-1bionic.20200711.051046`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-runtime-py=0.7.10-1bionic.20200711.062726`

Binary Packages:

- `ros-dashing-rosidl-runtime-py=0.7.10-1bionic.20200711.062726`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-typesupport-c=0.7.1-1bionic.20200711.053303`

Binary Packages:

- `ros-dashing-rosidl-typesupport-c=0.7.1-1bionic.20200711.053303`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-typesupport-cpp=0.7.1-1bionic.20200711.053512`

Binary Packages:

- `ros-dashing-rosidl-typesupport-cpp=0.7.1-1bionic.20200711.053512`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-typesupport-fastrtps-c=0.7.1-1bionic.20200711.052441`

Binary Packages:

- `ros-dashing-rosidl-typesupport-fastrtps-c=0.7.1-1bionic.20200711.052441`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-typesupport-fastrtps-cpp=0.7.1-1bionic.20200711.052117`

Binary Packages:

- `ros-dashing-rosidl-typesupport-fastrtps-cpp=0.7.1-1bionic.20200711.052117`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-typesupport-interface=0.7.9-1bionic.20200711.050850`

Binary Packages:

- `ros-dashing-rosidl-typesupport-interface=0.7.9-1bionic.20200711.050850`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-typesupport-introspection-c=0.7.9-1bionic.20200711.051904`

Binary Packages:

- `ros-dashing-rosidl-typesupport-introspection-c=0.7.9-1bionic.20200711.051904`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-rosidl-typesupport-introspection-cpp=0.7.9-1bionic.20200711.052139`

Binary Packages:

- `ros-dashing-rosidl-typesupport-introspection-cpp=0.7.9-1bionic.20200711.052139`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-sensor-msgs=0.7.0-1bionic.20200711.063052`

Binary Packages:

- `ros-dashing-sensor-msgs=0.7.0-1bionic.20200711.063052`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-shape-msgs=0.7.0-1bionic.20200711.062238`

Binary Packages:

- `ros-dashing-shape-msgs=0.7.0-1bionic.20200711.062238`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-sros2-cmake=0.7.2-1bionic.20200711.114718`

Binary Packages:

- `ros-dashing-sros2-cmake=0.7.2-1bionic.20200711.114718`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-sros2=0.7.2-1bionic.20200711.114113`

Binary Packages:

- `ros-dashing-sros2=0.7.2-1bionic.20200711.114113`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-std-msgs=0.7.0-1bionic.20200711.055335`

Binary Packages:

- `ros-dashing-std-msgs=0.7.0-1bionic.20200711.055335`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-std-srvs=0.7.0-1bionic.20200711.054100`

Binary Packages:

- `ros-dashing-std-srvs=0.7.0-1bionic.20200711.054100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-stereo-msgs=0.7.0-1bionic.20200711.065618`

Binary Packages:

- `ros-dashing-stereo-msgs=0.7.0-1bionic.20200711.065618`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tf2-eigen=0.11.6-1bionic.20200711.121703`

Binary Packages:

- `ros-dashing-tf2-eigen=0.11.6-1bionic.20200711.121703`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tf2-geometry-msgs=0.11.6-1bionic.20200711.121715`

Binary Packages:

- `ros-dashing-tf2-geometry-msgs=0.11.6-1bionic.20200711.121715`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tf2-kdl=0.11.6-1bionic.20200711.115450`

Binary Packages:

- `ros-dashing-tf2-kdl=0.11.6-1bionic.20200711.115450`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tf2-msgs=0.11.6-1bionic.20200711.062730`

Binary Packages:

- `ros-dashing-tf2-msgs=0.11.6-1bionic.20200711.062730`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tf2-ros=0.11.6-1bionic.20200711.114955`

Binary Packages:

- `ros-dashing-tf2-ros=0.11.6-1bionic.20200711.114955`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tf2=0.11.6-1bionic.20200711.063916`

Binary Packages:

- `ros-dashing-tf2=0.11.6-1bionic.20200711.063916`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tinydir-vendor=1.1.0-1bionic.20200711.051237`

Binary Packages:

- `ros-dashing-tinydir-vendor=1.1.0-1bionic.20200711.051237`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tinyxml-vendor=0.7.0-1bionic.20200711.051316`

Binary Packages:

- `ros-dashing-tinyxml-vendor=0.7.0-1bionic.20200711.051316`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-tinyxml2-vendor=0.6.1-1bionic.20200711.051249`

Binary Packages:

- `ros-dashing-tinyxml2-vendor=0.6.1-1bionic.20200711.051249`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-trajectory-msgs=0.7.0-1bionic.20200711.064017`

Binary Packages:

- `ros-dashing-trajectory-msgs=0.7.0-1bionic.20200711.064017`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-uncrustify-vendor=1.2.0-1bionic.20200711.045559`

Binary Packages:

- `ros-dashing-uncrustify-vendor=1.2.0-1bionic.20200711.045559`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-unique-identifier-msgs=2.1.1-1bionic.20200711.054108`

Binary Packages:

- `ros-dashing-unique-identifier-msgs=2.1.1-1bionic.20200711.054108`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-urdf=2.2.0-1bionic.20200711.051750`

Binary Packages:

- `ros-dashing-urdf=2.2.0-1bionic.20200711.051750`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-urdfdom-headers=1.0.4-1bionic.20200711.044149`

Binary Packages:

- `ros-dashing-urdfdom-headers=1.0.4-1bionic.20200711.044149`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-urdfdom=2.2.0-1bionic.20200711.051427`

Binary Packages:

- `ros-dashing-urdfdom=2.2.0-1bionic.20200711.051427`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-dashing-visualization-msgs=0.7.0-1bionic.20200711.064027`

Binary Packages:

- `ros-dashing-visualization-msgs=0.7.0-1bionic.20200711.064027`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-actionlib-msgs=1.12.7-0bionic.20200812.173125`

Binary Packages:

- `ros-melodic-actionlib-msgs=1.12.7-0bionic.20200812.173125`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-catkin=0.7.28-1bionic.20200731.223830`

Binary Packages:

- `ros-melodic-catkin=0.7.28-1bionic.20200731.223830`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-class-loader=0.4.1-0bionic.20200801.042322`

Binary Packages:

- `ros-melodic-class-loader=0.4.1-0bionic.20200801.042322`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-common-msgs=1.12.7-0bionic.20200821.052334`

Binary Packages:

- `ros-melodic-common-msgs=1.12.7-0bionic.20200821.052334`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-cpp-common=0.6.14-1bionic.20200801.035855`

Binary Packages:

- `ros-melodic-cpp-common=0.6.14-1bionic.20200801.035855`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-diagnostic-msgs=1.12.7-0bionic.20200812.173616`

Binary Packages:

- `ros-melodic-diagnostic-msgs=1.12.7-0bionic.20200812.173616`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-gazebo-msgs=2.8.7-1bionic.20200821.041158`

Binary Packages:

- `ros-melodic-gazebo-msgs=2.8.7-1bionic.20200821.041158`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-gencpp=0.6.5-1bionic.20200801.032957`

Binary Packages:

- `ros-melodic-gencpp=0.6.5-1bionic.20200801.032957`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-geneus=2.2.6-0bionic.20200801.045720`

Binary Packages:

- `ros-melodic-geneus=2.2.6-0bionic.20200801.045720`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-genlisp=0.4.16-0bionic.20200801.045634`

Binary Packages:

- `ros-melodic-genlisp=0.4.16-0bionic.20200801.045634`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-genmsg=0.5.16-1bionic.20200801.024608`

Binary Packages:

- `ros-melodic-genmsg=0.5.16-1bionic.20200801.024608`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-gennodejs=2.0.1-0bionic.20200801.033035`

Binary Packages:

- `ros-melodic-gennodejs=2.0.1-0bionic.20200801.033035`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-genpy=0.6.14-1bionic.20200812.160538`

Binary Packages:

- `ros-melodic-genpy=0.6.14-1bionic.20200812.160538`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-geometry-msgs=1.12.7-0bionic.20200812.174659`

Binary Packages:

- `ros-melodic-geometry-msgs=1.12.7-0bionic.20200812.174659`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-message-filters=1.14.9-1bionic.20200820.220853`

Binary Packages:

- `ros-melodic-message-filters=1.14.9-1bionic.20200820.220853`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-message-generation=0.4.1-1bionic.20200812.162033`

Binary Packages:

- `ros-melodic-message-generation=0.4.1-1bionic.20200812.162033`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-message-runtime=0.4.12-0bionic.20200812.162010`

Binary Packages:

- `ros-melodic-message-runtime=0.4.12-0bionic.20200812.162010`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-mk=1.14.9-1bionic.20200812.164708`

Binary Packages:

- `ros-melodic-mk=1.14.9-1bionic.20200812.164708`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-nav-msgs=1.12.7-0bionic.20200812.180738`

Binary Packages:

- `ros-melodic-nav-msgs=1.12.7-0bionic.20200812.180738`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-pluginlib=1.12.1-0bionic.20200813.002811`

Binary Packages:

- `ros-melodic-pluginlib=1.12.1-0bionic.20200813.002811`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-ros-comm=1.14.9-1bionic.20200820.232057`

Binary Packages:

- `ros-melodic-ros-comm=1.14.9-1bionic.20200820.232057`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-ros-environment=1.2.2-1bionic.20200801.022105`

Binary Packages:

- `ros-melodic-ros-environment=1.2.2-1bionic.20200801.022105`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-ros=1.14.9-1bionic.20200812.193254`

Binary Packages:

- `ros-melodic-ros=1.14.9-1bionic.20200812.193254`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosbag-migration-rule=1.0.0-0bionic.20200801.040144`

Binary Packages:

- `ros-melodic-rosbag-migration-rule=1.0.0-0bionic.20200801.040144`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosbag-storage=1.14.9-1bionic.20200820.220910`

Binary Packages:

- `ros-melodic-rosbag-storage=1.14.9-1bionic.20200820.220910`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosbag=1.14.9-1bionic.20200820.222501`

Binary Packages:

- `ros-melodic-rosbag=1.14.9-1bionic.20200820.222501`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosbash=1.14.9-1bionic.20200801.045055`

Binary Packages:

- `ros-melodic-rosbash=1.14.9-1bionic.20200801.045055`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosboost-cfg=1.14.9-1bionic.20200801.011112`

Binary Packages:

- `ros-melodic-rosboost-cfg=1.14.9-1bionic.20200801.011112`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosbuild=1.14.9-1bionic.20200812.163351`

Binary Packages:

- `ros-melodic-rosbuild=1.14.9-1bionic.20200812.163351`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosclean=1.14.9-1bionic.20200801.023033`

Binary Packages:

- `ros-melodic-rosclean=1.14.9-1bionic.20200801.023033`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosconsole=1.13.17-1bionic.20200812.193255`

Binary Packages:

- `ros-melodic-rosconsole=1.13.17-1bionic.20200812.193255`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roscpp-serialization=0.6.14-1bionic.20200801.063506`

Binary Packages:

- `ros-melodic-roscpp-serialization=0.6.14-1bionic.20200801.063506`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roscpp-traits=0.6.14-1bionic.20200801.063118`

Binary Packages:

- `ros-melodic-roscpp-traits=0.6.14-1bionic.20200801.063118`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roscpp-tutorials=0.9.3-1bionic.20200820.212531`

Binary Packages:

- `ros-melodic-roscpp-tutorials=0.9.3-1bionic.20200820.212531`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roscpp=1.14.9-1bionic.20200820.210119`

Binary Packages:

- `ros-melodic-roscpp=1.14.9-1bionic.20200820.210119`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roscreate=1.14.9-1bionic.20200801.033820`

Binary Packages:

- `ros-melodic-roscreate=1.14.9-1bionic.20200801.033820`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosgraph-msgs=1.11.2-0bionic.20200812.191236`

Binary Packages:

- `ros-melodic-rosgraph-msgs=1.11.2-0bionic.20200812.191236`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosgraph=1.14.9-1bionic.20200820.205150`

Binary Packages:

- `ros-melodic-rosgraph=1.14.9-1bionic.20200820.205150`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roslang=1.14.9-1bionic.20200801.033220`

Binary Packages:

- `ros-melodic-roslang=1.14.9-1bionic.20200801.033220`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roslaunch=1.14.9-1bionic.20200820.211308`

Binary Packages:

- `ros-melodic-roslaunch=1.14.9-1bionic.20200820.211308`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roslib=1.14.9-1bionic.20200801.032024`

Binary Packages:

- `ros-melodic-roslib=1.14.9-1bionic.20200801.032024`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roslisp=1.9.24-1bionic.20200812.195815`

Binary Packages:

- `ros-melodic-roslisp=1.9.24-1bionic.20200812.195815`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roslz4=1.14.9-1bionic.20200820.205210`

Binary Packages:

- `ros-melodic-roslz4=1.14.9-1bionic.20200820.205210`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosmake=1.14.9-1bionic.20200801.022349`

Binary Packages:

- `ros-melodic-rosmake=1.14.9-1bionic.20200801.022349`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosmaster=1.14.9-1bionic.20200820.205634`

Binary Packages:

- `ros-melodic-rosmaster=1.14.9-1bionic.20200820.205634`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosmsg=1.14.9-1bionic.20200820.223956`

Binary Packages:

- `ros-melodic-rosmsg=1.14.9-1bionic.20200820.223956`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosnode=1.14.9-1bionic.20200820.225251`

Binary Packages:

- `ros-melodic-rosnode=1.14.9-1bionic.20200820.225251`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosout=1.14.9-1bionic.20200820.210239`

Binary Packages:

- `ros-melodic-rosout=1.14.9-1bionic.20200820.210239`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rospack=2.5.6-1bionic.20200801.023428`

Binary Packages:

- `ros-melodic-rospack=2.5.6-1bionic.20200801.023428`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosparam=1.14.9-1bionic.20200820.205624`

Binary Packages:

- `ros-melodic-rosparam=1.14.9-1bionic.20200820.205624`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rospy-tutorials=0.9.3-1bionic.20200820.224502`

Binary Packages:

- `ros-melodic-rospy-tutorials=0.9.3-1bionic.20200820.224502`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rospy=1.14.9-1bionic.20200820.212623`

Binary Packages:

- `ros-melodic-rospy=1.14.9-1bionic.20200820.212623`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosservice=1.14.9-1bionic.20200820.225242`

Binary Packages:

- `ros-melodic-rosservice=1.14.9-1bionic.20200820.225242`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rostest=1.14.9-1bionic.20200820.215554`

Binary Packages:

- `ros-melodic-rostest=1.14.9-1bionic.20200820.215554`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rostime=0.6.14-1bionic.20200801.051100`

Binary Packages:

- `ros-melodic-rostime=0.6.14-1bionic.20200801.051100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rostopic=1.14.9-1bionic.20200820.223955`

Binary Packages:

- `ros-melodic-rostopic=1.14.9-1bionic.20200820.223955`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-rosunit=1.14.9-1bionic.20200801.033831`

Binary Packages:

- `ros-melodic-rosunit=1.14.9-1bionic.20200801.033831`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-roswtf=1.14.9-1bionic.20200820.230552`

Binary Packages:

- `ros-melodic-roswtf=1.14.9-1bionic.20200820.230552`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-sensor-msgs=1.12.7-0bionic.20200821.002808`

Binary Packages:

- `ros-melodic-sensor-msgs=1.12.7-0bionic.20200821.002808`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-shape-msgs=1.12.7-0bionic.20200812.182711`

Binary Packages:

- `ros-melodic-shape-msgs=1.12.7-0bionic.20200812.182711`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-std-msgs=0.5.12-0bionic.20200812.163541`

Binary Packages:

- `ros-melodic-std-msgs=0.5.12-0bionic.20200812.163541`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-std-srvs=1.11.2-0bionic.20200812.163548`

Binary Packages:

- `ros-melodic-std-srvs=1.11.2-0bionic.20200812.163548`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-stereo-msgs=1.12.7-0bionic.20200821.042337`

Binary Packages:

- `ros-melodic-stereo-msgs=1.12.7-0bionic.20200821.042337`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-tf2-msgs=0.6.5-0bionic.20200812.193051`

Binary Packages:

- `ros-melodic-tf2-msgs=0.6.5-0bionic.20200812.193051`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-topic-tools=1.14.9-1bionic.20200820.220846`

Binary Packages:

- `ros-melodic-topic-tools=1.14.9-1bionic.20200820.220846`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-trajectory-msgs=1.12.7-0bionic.20200812.183427`

Binary Packages:

- `ros-melodic-trajectory-msgs=1.12.7-0bionic.20200812.183427`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-visualization-msgs=1.12.7-0bionic.20200812.183804`

Binary Packages:

- `ros-melodic-visualization-msgs=1.12.7-0bionic.20200812.183804`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-melodic-xmlrpcpp=1.14.9-1bionic.20200820.205124`

Binary Packages:

- `ros-melodic-xmlrpcpp=1.14.9-1bionic.20200820.205124`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc 2315 SHA256:e56822b88625bf6a51f06652fc36fa2a1348b4325ac76541800cd078192aa3d2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz 8044 SHA256:675847f5cddb860256cbf2e7d5b85918aa53b59b0fd97a466b39a5c77a399537
```

### `dpkg` source package: `sbcl=2:1.4.5-1`

Binary Packages:

- `sbcl=2:1.4.5-1`

Licenses: (parsed from: `/usr/share/doc/sbcl/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `Expat`
- `NTP`
- `NTP~disclaimer`
- `permissive-xerox`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sbcl=2:1.4.5-1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_1.4.5-1.dsc' sbcl_1.4.5-1.dsc 2352 SHA256:dc7421f1dcd2d7b30393f6846e766efe7bf114aaf411e878e99b8203af924baa
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_1.4.5.orig.tar.bz2' sbcl_1.4.5.orig.tar.bz2 5998856 SHA256:96192effd17f3e457f77bcff0619784ce6e7293e27e0e6c1546a542b3d8ac540
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_1.4.5-1.debian.tar.xz' sbcl_1.4.5-1.debian.tar.xz 71404 SHA256:1dbe1e4d6a6e65e199f8748c098ba8874892399e187ec163784e996c7aeeb681
```

### `dpkg` source package: `sed=4.4-2`

Binary Packages:

- `sed=4.4-2`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4-2.dsc' sed_4.4-2.dsc 2006 SHA256:0e025a69a04c867048f918778771e2ba79d6ddfd62cb5ce6c3a6e255c005706c
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4.orig.tar.xz' sed_4.4.orig.tar.xz 1181664 SHA256:cbd6ebc5aaf080ed60d0162d7f6aeae58211a1ee9ba9bb25623daa6cd942683b
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4-2.debian.tar.xz' sed_4.4-2.debian.tar.xz 59600 SHA256:9f9b8bec0438ea0d0bd4315548de519543385c8196bcfcc61362f38f4cc6e7ed
```

### `dpkg` source package: `sensible-utils=0.0.12`

Binary Packages:

- `sensible-utils=0.0.12`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.12
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.dsc' sensible-utils_0.0.12.dsc 1732 SHA256:1b62cc5f7561b3f5692a6edaec942e2e97e8368dabff8c865867d428eecb1221
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.tar.xz' sensible-utils_0.0.12.tar.xz 62152 SHA256:99ba2ebf8c57447c69d426b99b84ff9dc817be0bc4988ec6890a14558c529e2e
```

### `dpkg` source package: `sgml-base=1.29`

Binary Packages:

- `sgml-base=1.29`

Licenses: (parsed from: `/usr/share/doc/sgml-base/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sgml-base=1.29
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.29.dsc' sgml-base_1.29.dsc 1387 SHA256:5fa519d3de7365d2256c7b9e74b6234a5c81bd115efb6305a53444584c32f8b1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.29.tar.xz' sgml-base_1.29.tar.xz 12224 SHA256:33808f1d51407ae105d471bf53cab526fe8903b003b78bc7ac4fd1429b7986b4
```

### `dpkg` source package: `shadow=1:4.5-1ubuntu2`

Binary Packages:

- `login=1:4.5-1ubuntu2`
- `passwd=1:4.5-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.5-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.dsc' shadow_4.5-1ubuntu2.dsc 2426 SHA256:34cc68fd24c6376c16311720f20dcb345e5da19adbe39edae249a49e45cee9e1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA256:22b0952dc944b163e2370bb911b11ca275fc80ad024267cf21e496b28c23d500
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.debian.tar.xz' shadow_4.5-1ubuntu2.debian.tar.xz 471472 SHA256:0025e344b478aae6e2d9ad7657b5e1fd0ebd1fda7a55e7fc144840f75b92d358
```

### `dpkg` source package: `six=1.11.0-2`

Binary Packages:

- `python-six=1.11.0-2`
- `python3-six=1.11.0-2`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`, `/usr/share/doc/python3-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.11.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.11.0-2.dsc' six_1.11.0-2.dsc 2316 SHA256:c0391b38bc251a3df586bdb163cb250af78aee69bbb27880215a350caaea53f2
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.11.0.orig.tar.gz' six_1.11.0.orig.tar.gz 29860 SHA256:70e8a77beed4562e7f14fe23a786b54f6296e34344c23bc42f07b15018ff98e9
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.11.0-2.debian.tar.xz' six_1.11.0-2.debian.tar.xz 4176 SHA256:bbd91dcb509a1f083bf531062b77dfdf2cbd2badca0fbe5d81957fe852ac4a7a
```

### `dpkg` source package: `sqlite3=3.22.0-1ubuntu0.4`

Binary Packages:

- `libsqlite3-0:amd64=3.22.0-1ubuntu0.4`
- `libsqlite3-dev:amd64=3.22.0-1ubuntu0.4`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.22.0-1ubuntu0.4
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.dsc' sqlite3_3.22.0-1ubuntu0.4.dsc 2512 SHA256:d3d351ccddcb3fc1f08f0cd7f98e1e28a4f5d310609882933a719864cd386ae9
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig-www.tar.xz' sqlite3_3.22.0.orig-www.tar.xz 3564688 SHA256:a61a14d6f457bb31ca32f4844398140050597fe4403dc0ee19576111f407e231
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig.tar.xz' sqlite3_3.22.0.orig.tar.xz 6019648 SHA256:f973ba63b5a1ea1d72e80c585bfb945e71d3f8b74fbecccdf345a84f8c91e5d1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz' sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz 47632 SHA256:3fddb7f76857daed76685d157320271706c72529aaec2e843a83ea92bc05b689
```

### `dpkg` source package: `sudo=1.8.21p2-3ubuntu1.2`

Binary Packages:

- `sudo=1.8.21p2-3ubuntu1.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris sudo=1.8.21p2-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.21p2-3ubuntu1.2.dsc' sudo_1.8.21p2-3ubuntu1.2.dsc 2129 SHA256:356e0955987c04887ebc59fe0dcb1acb6f31d175f7b37788574a80fbcdbf394b
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.21p2.orig.tar.gz' sudo_1.8.21p2.orig.tar.gz 3008808 SHA256:0d17b4b1c720de4150f5e1d35627cf8b3a6495041cb0d842f3172eeeb459359d
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.21p2-3ubuntu1.2.debian.tar.xz' sudo_1.8.21p2-3ubuntu1.2.debian.tar.xz 34188 SHA256:addb12923ff5c24aa08858c94107eca7423665069e564260ef4f379bac84500d
```

### `dpkg` source package: `systemd=237-3ubuntu10.42`

Binary Packages:

- `libsystemd0:amd64=237-3ubuntu10.42`
- `libudev1:amd64=237-3ubuntu10.42`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=237-3ubuntu10.42
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.42.dsc' systemd_237-3ubuntu10.42.dsc 5182 SHA256:38073197625912794aacfe4522006680aae20d1743699fa9b0de71f14536fa74
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237.orig.tar.gz' systemd_237.orig.tar.gz 6871350 SHA256:c83dabbe1c9de6b9db1dafdb7e04140c7d0535705c68842f6c0768653ba4913c
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.42.debian.tar.xz' systemd_237-3ubuntu10.42.debian.tar.xz 275288 SHA256:8f408963e65e7cd4435df53e43c17f39b4a5d3df0cf66fba99f91a8f5956f685
```

### `dpkg` source package: `sysvinit=2.88dsf-59.10ubuntu1`

Binary Packages:

- `sysvinit-utils=2.88dsf-59.10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.10ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10ubuntu1.dsc' sysvinit_2.88dsf-59.10ubuntu1.dsc 2428 SHA256:030f4e8a71381529da3141988344d6e1d0e05ba437e0cdd38d2f3786185bf285
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10ubuntu1.debian.tar.xz' sysvinit_2.88dsf-59.10ubuntu1.debian.tar.xz 132736 SHA256:faee591309aa0065aa43f44a1e840eb01db7f55379af2b45949534bd0317b734
```

### `dpkg` source package: `tar=1.29b-2ubuntu0.1`

Binary Packages:

- `tar=1.29b-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.29b-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.dsc' tar_1.29b-2ubuntu0.1.dsc 1426 SHA256:a926fddb2d770936f8925c84bb665bb7cf6fae020ff7573dd85126a54aa6acb5
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b.orig.tar.xz' tar_1.29b.orig.tar.xz 1822008 SHA256:6a59706ebee384a6cd2fb3ee1dbfbfc20c5c66c7efd7cedb28edc054fca8ba00
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.debian.tar.xz' tar_1.29b-2ubuntu0.1.debian.tar.xz 31672 SHA256:4fbae6a9aaf492dabed71d6a5e07fb1d5bad89d88eaea4c398791cd326fe44d5
```

### `dpkg` source package: `tinyxml2=6.0.0+dfsg-1`

Binary Packages:

- `libtinyxml2-6:amd64=6.0.0+dfsg-1`
- `libtinyxml2-dev:amd64=6.0.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libtinyxml2-6/copyright`, `/usr/share/doc/libtinyxml2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris tinyxml2=6.0.0+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_6.0.0+dfsg-1.dsc' tinyxml2_6.0.0+dfsg-1.dsc 1999 SHA256:d103b12a55f1225e61a87cabf184237be9213233972e3d7bd35a4cc926736aec
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_6.0.0+dfsg.orig.tar.gz' tinyxml2_6.0.0+dfsg.orig.tar.gz 352041 SHA256:ef930de291e18acef913a79bba1d2d8e387cd19cfd9fef7618895a21c909164b
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_6.0.0+dfsg-1.debian.tar.xz' tinyxml2_6.0.0+dfsg-1.debian.tar.xz 5532 SHA256:6e6052241bc2d7cefbf915b101474185bd5a7369456fbac0f0efa53b8a3c75a6
```

### `dpkg` source package: `tinyxml=2.6.2-4`

Binary Packages:

- `libtinyxml-dev:amd64=2.6.2-4`
- `libtinyxml2.6.2v5:amd64=2.6.2-4`

Licenses: (parsed from: `/usr/share/doc/libtinyxml-dev/copyright`, `/usr/share/doc/libtinyxml2.6.2v5/copyright`)

- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris tinyxml=2.6.2-4
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml/tinyxml_2.6.2-4.dsc' tinyxml_2.6.2-4.dsc 2037 SHA256:20b92fb0ce6365ba6bd780bf5fe68bdc8c013317203eaa1b955adf72ccdb3d8a
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml/tinyxml_2.6.2.orig.tar.gz' tinyxml_2.6.2.orig.tar.gz 210124 SHA256:15bdfdcec58a7da30adc87ac2b078e4417dbe5392f3afb719f9ba6d062645593
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml/tinyxml_2.6.2-4.debian.tar.xz' tinyxml_2.6.2-4.debian.tar.xz 4344 SHA256:ceb250b862165f89d0fd081d4d3174fe5843ca0573517c9acb765b5af1723002
```

### `dpkg` source package: `tzdata=2020a-0ubuntu0.18.04`

Binary Packages:

- `tzdata=2020a-0ubuntu0.18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2020a-0ubuntu0.18.04
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.18.04.dsc' tzdata_2020a-0ubuntu0.18.04.dsc 2363 SHA256:2cda7350a6124fa6b930e51904ee56034c302101fb7357c08f9c3828c87ffc1a
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz' tzdata_2020a.orig.tar.gz 397245 SHA256:547161eca24d344e0b5f96aff6a76b454da295dc14ed4ca50c2355043fb899a2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz.asc' tzdata_2020a.orig.tar.gz.asc 833 SHA256:a92f085fe1e7f8bc0f0a0bc4432f27e6cf2d69e64d4a90958bd023eb0ccf45f9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.18.04.debian.tar.xz' tzdata_2020a-0ubuntu0.18.04.debian.tar.xz 104992 SHA256:a983c500ec5b85f5b111350edc7b59533557e0c439bad23ccfeb940f93b6b73f
```

### `dpkg` source package: `ubuntu-keyring=2018.09.18.1~18.04.0`

Binary Packages:

- `ubuntu-keyring=2018.09.18.1~18.04.0`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2018.09.18.1~18.04.0
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.dsc' ubuntu-keyring_2018.09.18.1~18.04.0.dsc 1503 SHA256:1c9a599b6b3c98fdc920756c8031678d2556b6267eb55f057d0369cfc64e0263
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz' ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz 34238 SHA256:7095b786c02816bb6933b3a73ed6c9e302542e8fc1edb8346f7ddab49e95b3bd
```

### `dpkg` source package: `uncrustify=0.66.1+dfsg1-1`

Binary Packages:

- `uncrustify=0.66.1+dfsg1-1`

Licenses: (parsed from: `/usr/share/doc/uncrustify/copyright`)

- `Artistic`
- `GPL`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris uncrustify=0.66.1+dfsg1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/u/uncrustify/uncrustify_0.66.1+dfsg1-1.dsc' uncrustify_0.66.1+dfsg1-1.dsc 1632 SHA256:225931ff5f0398061b8b6f8e9950e71658b067c352e78ea8e7ba36f69fd001d5
'http://archive.ubuntu.com/ubuntu/pool/universe/u/uncrustify/uncrustify_0.66.1+dfsg1.orig.tar.xz' uncrustify_0.66.1+dfsg1.orig.tar.xz 700912 SHA256:f2599bee3ab0c529042742125e2d6325cd39ed8e2821c7dcff51405186ce02bc
'http://archive.ubuntu.com/ubuntu/pool/universe/u/uncrustify/uncrustify_0.66.1+dfsg1-1.debian.tar.xz' uncrustify_0.66.1+dfsg1-1.debian.tar.xz 4480 SHA256:e7e2101198f0250470f0b6d0b5ffe6f8cd02ebc475dfe1fa88dd341de2dacd09
```

### `dpkg` source package: `unixodbc=2.3.4-1.1ubuntu3`

Binary Packages:

- `libodbc1:amd64=2.3.4-1.1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libodbc1/copyright`)

- `GPL`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris unixodbc=2.3.4-1.1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.4-1.1ubuntu3.dsc' unixodbc_2.3.4-1.1ubuntu3.dsc 2213 SHA256:82ff3dc47665081d287c98f2d8c1390819c176d4d23378a65010b7860827b06f
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.4.orig.tar.gz' unixodbc_2.3.4.orig.tar.gz 1830660 SHA256:2e1509a96bb18d248bf08ead0d74804957304ff7c6f8b2e5965309c632421e39
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.4-1.1ubuntu3.diff.gz' unixodbc_2.3.4-1.1ubuntu3.diff.gz 19700 SHA256:7b533e947f1a0c49541668924b3679e8fe7dac75a3759081a6ac82f0c55f9184
```

### `dpkg` source package: `util-linux=2.31.1-0.4ubuntu3.6`

Binary Packages:

- `bsdutils=1:2.31.1-0.4ubuntu3.6`
- `fdisk=2.31.1-0.4ubuntu3.6`
- `libblkid1:amd64=2.31.1-0.4ubuntu3.6`
- `libfdisk1:amd64=2.31.1-0.4ubuntu3.6`
- `libmount1:amd64=2.31.1-0.4ubuntu3.6`
- `libsmartcols1:amd64=2.31.1-0.4ubuntu3.6`
- `libuuid1:amd64=2.31.1-0.4ubuntu3.6`
- `mount=2.31.1-0.4ubuntu3.6`
- `util-linux=2.31.1-0.4ubuntu3.6`
- `uuid-dev:amd64=2.31.1-0.4ubuntu3.6`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `xml-core=0.18`

Binary Packages:

- `xml-core=0.18`

Licenses: (parsed from: `/usr/share/doc/xml-core/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xml-core=0.18
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.18.dsc' xml-core_0.18.dsc 1564 SHA256:109b93880b90e7ec07c7efe9508ed74e1c69de72b6be3e77ebff0c8f0ddcf4a9
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.18.tar.xz' xml-core_0.18.tar.xz 23804 SHA256:353f05dbb03c642649a6bec28b1acf3c57e489ffdd1401f5e9624dcc90af72cd
```

### `dpkg` source package: `xz-utils=5.2.2-1.3`

Binary Packages:

- `liblzma5:amd64=5.2.2-1.3`
- `xz-utils=5.2.2-1.3`

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
$ apt-get source -qq --print-uris xz-utils=5.2.2-1.3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.dsc' xz-utils_5.2.2-1.3.dsc 2575 SHA256:3ea4e6a32f6265b152f89ceafe78c8839e5f4bb1cad137b159fe2013817f9342
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz' xz-utils_5.2.2.orig.tar.xz 1016404 SHA256:f341b1906ebcdde291dd619399ae944600edc9193619dd0c0110a5f05bfcc89e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz.asc' xz-utils_5.2.2.orig.tar.xz.asc 543 SHA256:2cc0575556e1331b3f468e6e7dca5969ce86efcc315d62672279b4e68b2e449f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.debian.tar.xz' xz-utils_5.2.2-1.3.debian.tar.xz 108680 SHA256:d76c3acf39d0999c14384695394970e8f98853fd6736ba91972d3e67106bc6f6
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-0ubuntu2`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-0ubuntu2`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-0ubuntu2.dsc' zlib_1.2.11.dfsg-0ubuntu2.dsc 2676 SHA256:e733161caf3c6864deec55f40f80c0872f7c83bd9c6e9f937472f227ad912281
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.xz' zlib_1.2.11.dfsg.orig.tar.xz 287216 SHA256:881c8a90f488def83488aa91fd68563c023013a4b9b07a040f6da2727d76ad60
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-0ubuntu2.debian.tar.xz' zlib_1.2.11.dfsg-0ubuntu2.debian.tar.xz 18344 SHA256:afad42904f793d13a0b631e082e575d90a7c7c443973d08a00061a9bbb5ca380
```
