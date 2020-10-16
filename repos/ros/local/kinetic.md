# `ros:kinetic-ros-base`

## Docker Metadata

- Image ID: `sha256:818be0efb8921ba4f558c5721da0475399ddaef426ff4f0551a0c831d7384261`
- Created: `2020-09-26T01:32:03.654692639Z`
- Virtual Size: ~ 1.12 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/ros_entrypoint.sh"]`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `LC_ALL=C.UTF-8`
  - `ROS_DISTRO=kinetic`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3`

Binary Packages:

- `libacl1:amd64=2.2.52-3`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3.dsc' acl_2.2.52-3.dsc 2025 SHA256:82e344b9ab176559a85630b74ee5a68d678d7f24b6fe8139f2fd9fcf38a48095
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3.debian.tar.xz' acl_2.2.52-3.debian.tar.xz 8740 SHA256:fc3f1178d18288993fc4ce4853b7f9dcdf0bd1fd26e4f69349a4e4e5916d1fa8
```

### `dpkg` source package: `adduser=3.113+nmu3ubuntu4`

Binary Packages:

- `adduser=3.113+nmu3ubuntu4`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.113+nmu3ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.113+nmu3ubuntu4.dsc' adduser_3.113+nmu3ubuntu4.dsc 1856 SHA256:323f327b25e1fbeba38278eae5813be6238a7c5959e7c10af041999408440247
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.113+nmu3ubuntu4.tar.gz' adduser_3.113+nmu3ubuntu4.tar.gz 367980 SHA256:6e4d44c8388b9ba85fc175fa4a48ed43bf6500913c2c631fda0e4419ae63c65a
```

### `dpkg` source package: `apparmor=2.10.95-0ubuntu2.11`

Binary Packages:

- `libapparmor1:amd64=2.10.95-0ubuntu2.11`

Licenses: (parsed from: `/usr/share/doc/libapparmor1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris apparmor=2.10.95-0ubuntu2.11
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.10.95-0ubuntu2.11.dsc' apparmor_2.10.95-0ubuntu2.11.dsc 3256 SHA512:29ab3be3ce0698980cc80eeb713a7c471e5aae4802f74aefce020c488d819f4ee81e89fb27f2188619f8206104771d0632b207eb71d09a696e274402235486d7
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.10.95.orig.tar.gz' apparmor_2.10.95.orig.tar.gz 4502268 SHA512:bd8b4223c0de15b76784a42e4ca1ad7da19ae0d12e1f592dc4af14b76c9d549da381cfe50365d75a16fb6bbb42c00d3f1f379a9c785d51cf512e0c8f96013084
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.10.95-0ubuntu2.11.debian.tar.xz' apparmor_2.10.95-0ubuntu2.11.debian.tar.xz 98980 SHA512:6e410dd41e0d7f09d08ee1e1ad3cd6e82496a82afe158a37af7a3992d93095dbff11d22797fb19fac6d3b158e6ba80f840c380d99e703b41c428f182b22e42aa
```

### `dpkg` source package: `apr-util=1.5.4-1build1`

Binary Packages:

- `libaprutil1:amd64=1.5.4-1build1`
- `libaprutil1-dev=1.5.4-1build1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`, `/usr/share/doc/libaprutil1-dev/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.5.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.5.4-1build1.dsc' apr-util_1.5.4-1build1.dsc 2642 SHA256:f464c7a9fb9293c117e80d9669450ca61191ad456cf40dd74777caf06e5f18db
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.5.4.orig.tar.bz2' apr-util_1.5.4.orig.tar.bz2 694427 SHA256:a6cf327189ca0df2fb9d5633d7326c460fe2b61684745fd7963e79a6dd0dc82e
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.5.4-1build1.debian.tar.xz' apr-util_1.5.4-1build1.debian.tar.xz 16564 SHA256:562bd9b543a16edf8218deda292c606aabe5265a369cf7b2559f13c1cc300e3c
```

### `dpkg` source package: `apr=1.5.2-3`

Binary Packages:

- `libapr1:amd64=1.5.2-3`
- `libapr1-dev=1.5.2-3`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`, `/usr/share/doc/libapr1-dev/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.5.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.5.2-3.dsc' apr_1.5.2-3.dsc 2090 SHA256:2344484f62544881344defbb1076ca6cce51f930f1a5abd359e65eafb0e169cb
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.5.2.orig.tar.bz2' apr_1.5.2.orig.tar.bz2 826885 SHA256:7d03ed29c22a7152be45b8e50431063736df9e1daa1ddf93f6a547ba7a28f67a
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.5.2-3.debian.tar.xz' apr_1.5.2-3.debian.tar.xz 18572 SHA256:442ffb9a7225cf405fe7a2b4a4624543fcb93e6f14cccf22acd57916cfa8348d
```

### `dpkg` source package: `apt=1.2.32ubuntu0.1`

Binary Packages:

- `apt=1.2.32ubuntu0.1`
- `libapt-pkg5.0:amd64=1.2.32ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.2.32ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.2.32ubuntu0.1.dsc' apt_1.2.32ubuntu0.1.dsc 2218 SHA512:0d0925594dc5c4d188928cac86d5a0c4176f3877b26af1bc119b6dde1bf64b5d94375b39c26276e8b21fe5dd11106f9d26be05d570a831b4e7e1dd1de88db67a
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.2.32ubuntu0.1.tar.xz' apt_1.2.32ubuntu0.1.tar.xz 2095712 SHA512:8f28f0c96148186621ed8cc65e3913322154fc467e2fb414ef67bac492a953480a539de358b3ef8432e1b0b10baa03d9e2c7b495705f82608f009f9061c67c07
```

### `dpkg` source package: `atk1.0=2.18.0-1`

Binary Packages:

- `libatk1.0-0:amd64=2.18.0-1`
- `libatk1.0-data=2.18.0-1`

Licenses: (parsed from: `/usr/share/doc/libatk1.0-0/copyright`, `/usr/share/doc/libatk1.0-data/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris atk1.0=2.18.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.18.0-1.dsc' atk1.0_2.18.0-1.dsc 2738 SHA256:3d58e1e9e653705df8a092ed6942e2e518b1e539196e467fc60f20721ccaa84c
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.18.0.orig.tar.xz' atk1.0_2.18.0.orig.tar.xz 687932 SHA256:ce6c48d77bf951083029d5a396dd552d836fff3c1715d3a7022e917e46d0c92b
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.18.0-1.debian.tar.xz' atk1.0_2.18.0-1.debian.tar.xz 10520 SHA256:84ebc674126d71a27994b856274d05c801782ab4cbd3b78351c987525243ed1d
```

### `dpkg` source package: `attr=1:2.4.47-2`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2.dsc' attr_2.4.47-2.dsc 2027 SHA256:ee842d6d62d473acf02b494c432cf33128fa46455a09d3172c77c252449fa1a6
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2.debian.tar.xz' attr_2.4.47-2.debian.tar.xz 8096 SHA256:f65909562def601b1556393f5656032c058dc574ba622414ad3eb80c7b05a42a
```

### `dpkg` source package: `audit=1:2.4.5-1ubuntu2.1`

Binary Packages:

- `libaudit-common=1:2.4.5-1ubuntu2.1`
- `libaudit1:amd64=1:2.4.5-1ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.4.5-1ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.4.5-1ubuntu2.1.dsc' audit_2.4.5-1ubuntu2.1.dsc 2753 SHA512:dcba64d5208c60d9720ca9dca2646e4766ddb13513f1e970bcf042f4cf825291ffaca269a7c159225de2d3bb9cdc0b0125918f9a222990d6c7267bcd32fb9285
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.4.5.orig.tar.gz' audit_2.4.5.orig.tar.gz 1030113 SHA512:9d4ff4b19c027e34d4b7537fb4113116e8f56e3da8047a8d19ce394954648df8aa3dd8f8b8eb0af0c04bf1b7b6031916db6a168a28f065879ca6744bc2b04f15
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.4.5-1ubuntu2.1.debian.tar.xz' audit_2.4.5-1ubuntu2.1.debian.tar.xz 19292 SHA512:3537dfd29b5ed6c19e3ccf302c07cc46e33c6ff27384f24fa41516b2f0e0dae7eca321daef7be0fff72d83692490f69a1fadd0fdbb55891ce38d94c4977d8e5c
```

### `dpkg` source package: `avahi=0.6.32~rc+dfsg-1ubuntu2.3`

Binary Packages:

- `libavahi-client3:amd64=0.6.32~rc+dfsg-1ubuntu2.3`
- `libavahi-common-data:amd64=0.6.32~rc+dfsg-1ubuntu2.3`
- `libavahi-common3:amd64=0.6.32~rc+dfsg-1ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.6.32~rc+dfsg-1ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.6.32~rc+dfsg-1ubuntu2.3.dsc' avahi_0.6.32~rc+dfsg-1ubuntu2.3.dsc 4414 SHA512:0d252662c0613c8d8be051c38f4b890843e146e00f0d46dcd98879321c1127fc4476621704f5ffb9722a076eb9270d9ec0a2af9d0556af9a56302a3734e62195
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.6.32~rc+dfsg.orig.tar.gz' avahi_0.6.32~rc+dfsg.orig.tar.gz 665175 SHA512:37c1fb2f383af68a191660387dd8d9850e5c57e496626612679576b031c8d84c2c1e6071b4cab3c46b70dd249b4f7aceecb93e3314dc5aa8d0173ca7fb2ebbfc
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.6.32~rc+dfsg-1ubuntu2.3.debian.tar.xz' avahi_0.6.32~rc+dfsg-1ubuntu2.3.debian.tar.xz 34628 SHA512:3723abe8a1b4513118b57ed426c56acbebb0492fa0e2f477205670802f38d1cad2d8d5122e0876f587d34c99cf365a9105a6b9b9cea8199c918c5def316c68f5
```

### `dpkg` source package: `base-files=9.4ubuntu4.13`

Binary Packages:

- `base-files=9.4ubuntu4.13`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=9.4ubuntu4.13
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_9.4ubuntu4.13.dsc' base-files_9.4ubuntu4.13.dsc 1639 SHA512:53e170545731c3531e1d4550120d68ba03ce35f97b179f3b0927fc93d762d7933a390417f68eb8114a426178362e7f7168ca23c9b5aec07a7b8f4a2e6c73ed2f
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_9.4ubuntu4.13.tar.xz' base-files_9.4ubuntu4.13.tar.xz 67184 SHA512:82572c771f79098406f6b52cd686fc70c4dfcdfadf3dfe6823c67a89c497867650868d908f451a23451d3c3d1f33e37bf39b48f331bc9872178152b1d42b8117
```

### `dpkg` source package: `base-passwd=3.5.39`

Binary Packages:

- `base-passwd=3.5.39`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.39
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.39.dsc' base-passwd_3.5.39.dsc 1720 SHA256:cfb464663fd23f5b64b7fdeb8860a754b28ee77b346bf2a362c36ceccb7a65ea
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.39.tar.xz' base-passwd_3.5.39.tar.xz 51560 SHA256:d827ce2d7b9b4b572527b2071f0e1354840a14c3a43a5081bcb31de400112803
```

### `dpkg` source package: `bash=4.3-14ubuntu1.4`

Binary Packages:

- `bash=4.3-14ubuntu1.4`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.3-14ubuntu1.4
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.3-14ubuntu1.4.dsc' bash_4.3-14ubuntu1.4.dsc 2346 SHA512:6a43b082f254950ec2bf6d1503fe23b0e1dae9f8cdaaae89f5f0ab2ad6c6ee16a292d0a525c0e9d12e9df24e1616c79f426182e7e03874e75fd50c87750e797d
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.3.orig.tar.gz' bash_4.3.orig.tar.gz 7516231 SHA512:1281b8bfe01c9b533824ff7de21752b9a4663589dc198e994faf09c0aed7f43d1b843929555b31e0c70c4b50eac943cc3df9224faee71cb19fa55dce4046d90e
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.3-14ubuntu1.4.debian.tar.xz' bash_4.3-14ubuntu1.4.debian.tar.xz 94248 SHA512:631ae6193f1b892fc33ae27398017fe9885d423ba3b2c01875de8f403f9de359d9db2c2125a2b5064c5761aee143af5347d16a335ffd3e0d91a938d12441a91c
```

### `dpkg` source package: `binutils=2.26.1-1ubuntu1~16.04.8`

Binary Packages:

- `binutils=2.26.1-1ubuntu1~16.04.8`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.26.1-1ubuntu1~16.04.8
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.26.1-1ubuntu1~16.04.8.dsc' binutils_2.26.1-1ubuntu1~16.04.8.dsc 4078 SHA512:eff1dc6a040835272e69765763161ac031d0aac024e705ec30f6fa62d2bd040b3ec8c9824928cf51029e1992514f14d7da3fb9088a5938eaacbeb422d0d3ffe2
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.26.1.orig.tar.gz' binutils_2.26.1.orig.tar.gz 34868933 SHA512:6c964a81b107684f64e371233157c93510214b250e6af6548f2797ad317c10fa3490b21c148d5343d133483979c4da0d70bccd5cc421911bf8066346b4ad9042
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.26.1-1ubuntu1~16.04.8.diff.gz' binutils_2.26.1-1ubuntu1~16.04.8.diff.gz 235088 SHA512:1750dd819809b369dfb419df98486fa8268bee2b5154e9f4cb5d924ac62a0bc91e5ebf5b2de7474e1aa3413dbbd7a6f68fc3ce6d127c7d10398a4efd45b0c6bc
```

### `dpkg` source package: `boost-defaults=1.58.0.1ubuntu1`

Binary Packages:

- `libboost-all-dev=1.58.0.1ubuntu1`
- `libboost-atomic-dev:amd64=1.58.0.1ubuntu1`
- `libboost-chrono-dev:amd64=1.58.0.1ubuntu1`
- `libboost-context-dev:amd64=1.58.0.1ubuntu1`
- `libboost-coroutine-dev:amd64=1.58.0.1ubuntu1`
- `libboost-date-time-dev:amd64=1.58.0.1ubuntu1`
- `libboost-dev:amd64=1.58.0.1ubuntu1`
- `libboost-exception-dev:amd64=1.58.0.1ubuntu1`
- `libboost-filesystem-dev:amd64=1.58.0.1ubuntu1`
- `libboost-graph-dev:amd64=1.58.0.1ubuntu1`
- `libboost-graph-parallel-dev=1.58.0.1ubuntu1`
- `libboost-iostreams-dev:amd64=1.58.0.1ubuntu1`
- `libboost-locale-dev:amd64=1.58.0.1ubuntu1`
- `libboost-log-dev=1.58.0.1ubuntu1`
- `libboost-math-dev:amd64=1.58.0.1ubuntu1`
- `libboost-mpi-dev=1.58.0.1ubuntu1`
- `libboost-mpi-python-dev=1.58.0.1ubuntu1`
- `libboost-program-options-dev:amd64=1.58.0.1ubuntu1`
- `libboost-python-dev=1.58.0.1ubuntu1`
- `libboost-random-dev:amd64=1.58.0.1ubuntu1`
- `libboost-regex-dev:amd64=1.58.0.1ubuntu1`
- `libboost-serialization-dev:amd64=1.58.0.1ubuntu1`
- `libboost-signals-dev:amd64=1.58.0.1ubuntu1`
- `libboost-system-dev:amd64=1.58.0.1ubuntu1`
- `libboost-test-dev:amd64=1.58.0.1ubuntu1`
- `libboost-thread-dev:amd64=1.58.0.1ubuntu1`
- `libboost-timer-dev:amd64=1.58.0.1ubuntu1`
- `libboost-tools-dev=1.58.0.1ubuntu1`
- `libboost-wave-dev:amd64=1.58.0.1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris boost-defaults=1.58.0.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost-defaults/boost-defaults_1.58.0.1ubuntu1.dsc' boost-defaults_1.58.0.1ubuntu1.dsc 3502 SHA256:b54fa784ab7c95c4b52a796c1caa503be2dc9b3460084d12e5a23eebb325b0f0
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost-defaults/boost-defaults_1.58.0.1ubuntu1.tar.gz' boost-defaults_1.58.0.1ubuntu1.tar.gz 10619 SHA256:60e743d2ec613928cfc9f514afe0e10da82c59c6d3546f2063ad8e388e2fc959
```

### `dpkg` source package: `boost1.58=1.58.0+dfsg-5ubuntu3.1`

Binary Packages:

- `libboost-atomic1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-atomic1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-chrono1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-chrono1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-context1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-context1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-coroutine1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-coroutine1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-date-time1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-date-time1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-exception1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-filesystem1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-filesystem1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-graph-parallel1.58-dev=1.58.0+dfsg-5ubuntu3.1`
- `libboost-graph-parallel1.58.0=1.58.0+dfsg-5ubuntu3.1`
- `libboost-graph1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-graph1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-iostreams1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-iostreams1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-locale1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-locale1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-log1.58-dev=1.58.0+dfsg-5ubuntu3.1`
- `libboost-log1.58.0=1.58.0+dfsg-5ubuntu3.1`
- `libboost-math1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-math1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-mpi-python1.58-dev=1.58.0+dfsg-5ubuntu3.1`
- `libboost-mpi-python1.58.0=1.58.0+dfsg-5ubuntu3.1`
- `libboost-mpi1.58-dev=1.58.0+dfsg-5ubuntu3.1`
- `libboost-mpi1.58.0=1.58.0+dfsg-5ubuntu3.1`
- `libboost-program-options1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-program-options1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-python1.58-dev=1.58.0+dfsg-5ubuntu3.1`
- `libboost-python1.58.0=1.58.0+dfsg-5ubuntu3.1`
- `libboost-random1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-random1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-regex1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-regex1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-serialization1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-serialization1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-signals1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-signals1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-system1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-system1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-test1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-test1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-thread1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-thread1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-timer1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-timer1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-wave1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost-wave1.58.0:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost1.58-dev:amd64=1.58.0+dfsg-5ubuntu3.1`
- `libboost1.58-tools-dev=1.58.0+dfsg-5ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/libboost-atomic1.58-dev/copyright`, `/usr/share/doc/libboost-atomic1.58.0/copyright`, `/usr/share/doc/libboost-chrono1.58-dev/copyright`, `/usr/share/doc/libboost-chrono1.58.0/copyright`, `/usr/share/doc/libboost-context1.58-dev/copyright`, `/usr/share/doc/libboost-context1.58.0/copyright`, `/usr/share/doc/libboost-coroutine1.58-dev/copyright`, `/usr/share/doc/libboost-coroutine1.58.0/copyright`, `/usr/share/doc/libboost-date-time1.58-dev/copyright`, `/usr/share/doc/libboost-date-time1.58.0/copyright`, `/usr/share/doc/libboost-exception1.58-dev/copyright`, `/usr/share/doc/libboost-filesystem1.58-dev/copyright`, `/usr/share/doc/libboost-filesystem1.58.0/copyright`, `/usr/share/doc/libboost-graph-parallel1.58-dev/copyright`, `/usr/share/doc/libboost-graph-parallel1.58.0/copyright`, `/usr/share/doc/libboost-graph1.58-dev/copyright`, `/usr/share/doc/libboost-graph1.58.0/copyright`, `/usr/share/doc/libboost-iostreams1.58-dev/copyright`, `/usr/share/doc/libboost-iostreams1.58.0/copyright`, `/usr/share/doc/libboost-locale1.58-dev/copyright`, `/usr/share/doc/libboost-locale1.58.0/copyright`, `/usr/share/doc/libboost-log1.58-dev/copyright`, `/usr/share/doc/libboost-log1.58.0/copyright`, `/usr/share/doc/libboost-math1.58-dev/copyright`, `/usr/share/doc/libboost-math1.58.0/copyright`, `/usr/share/doc/libboost-mpi-python1.58-dev/copyright`, `/usr/share/doc/libboost-mpi-python1.58.0/copyright`, `/usr/share/doc/libboost-mpi1.58-dev/copyright`, `/usr/share/doc/libboost-mpi1.58.0/copyright`, `/usr/share/doc/libboost-program-options1.58-dev/copyright`, `/usr/share/doc/libboost-program-options1.58.0/copyright`, `/usr/share/doc/libboost-python1.58-dev/copyright`, `/usr/share/doc/libboost-python1.58.0/copyright`, `/usr/share/doc/libboost-random1.58-dev/copyright`, `/usr/share/doc/libboost-random1.58.0/copyright`, `/usr/share/doc/libboost-regex1.58-dev/copyright`, `/usr/share/doc/libboost-regex1.58.0/copyright`, `/usr/share/doc/libboost-serialization1.58-dev/copyright`, `/usr/share/doc/libboost-serialization1.58.0/copyright`, `/usr/share/doc/libboost-signals1.58-dev/copyright`, `/usr/share/doc/libboost-signals1.58.0/copyright`, `/usr/share/doc/libboost-system1.58-dev/copyright`, `/usr/share/doc/libboost-system1.58.0/copyright`, `/usr/share/doc/libboost-test1.58-dev/copyright`, `/usr/share/doc/libboost-test1.58.0/copyright`, `/usr/share/doc/libboost-thread1.58-dev/copyright`, `/usr/share/doc/libboost-thread1.58.0/copyright`, `/usr/share/doc/libboost-timer1.58-dev/copyright`, `/usr/share/doc/libboost-timer1.58.0/copyright`, `/usr/share/doc/libboost-wave1.58-dev/copyright`, `/usr/share/doc/libboost-wave1.58.0/copyright`, `/usr/share/doc/libboost1.58-dev/copyright`, `/usr/share/doc/libboost1.58-tools-dev/copyright`)

- `Boost`

Source:

```console
$ apt-get source -qq --print-uris boost1.58=1.58.0+dfsg-5ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.58/boost1.58_1.58.0+dfsg-5ubuntu3.1.dsc' boost1.58_1.58.0+dfsg-5ubuntu3.1.dsc 6701 SHA512:ea3ae284550eda6324289cb3133e8723d00cf39dfb041a7da80d58e9a7ce97001213698687f2aef099797f9f0c0eff42583446ee3ec08b91c045c16e2d01b5de
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.58/boost1.58_1.58.0+dfsg.orig.tar.gz' boost1.58_1.58.0+dfsg.orig.tar.gz 82693055 SHA512:661052cf943d274d7eb3543f91272743ac4624a6791d52aa79b1d07630f685cbe6060c97ac858e486de71c1fba30cb7c9a8928582bb228dbdbd2d6b5f0e1fd31
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.58/boost1.58_1.58.0+dfsg-5ubuntu3.1.debian.tar.xz' boost1.58_1.58.0+dfsg-5ubuntu3.1.debian.tar.xz 158824 SHA512:593c2b6ead8112b1a7907542a99f59293df1f0e5b0695bd78bd05c100e5c73c5286a0675b0171a0cf1e9ddd58be75bbdd4e3644167018179411db18873d630b2
```

### `dpkg` source package: `build-essential=12.1ubuntu2`

Binary Packages:

- `build-essential=12.1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/build-essential/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris build-essential=12.1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.1ubuntu2.dsc' build-essential_12.1ubuntu2.dsc 2034 SHA256:c8a82bee0fffde9e74b3a06167bfa42f0d9c3b17b042878062256e70b699b43b
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.1ubuntu2.tar.gz' build-essential_12.1ubuntu2.tar.gz 66237 SHA256:32efeda3394258cb5459df0d4019e346dace80249db8ef263755803d0e85da91
```

### `dpkg` source package: `bzip2=1.0.6-8ubuntu0.2`

Binary Packages:

- `bzip2=1.0.6-8ubuntu0.2`
- `libbz2-1.0:amd64=1.0.6-8ubuntu0.2`
- `libbz2-dev:amd64=1.0.6-8ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8ubuntu0.2.dsc' bzip2_1.0.6-8ubuntu0.2.dsc 2173 SHA512:8d0b0d48bdde4510d239669d4f60fd952f1efeaf3ead4a4130493c9e14d7973fb67885e55c8faa2c87ace5841660989c3615c29788e3db856096913880150bb7
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA512:b1108c392a7f45218b86196498657f50333c870db4ab555ce4859a3fe76c17b4a3430b8a075b7f1c86d9ded006bdf17001b73bfcf261e2d2ee7de4998ad604fd
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8ubuntu0.2.debian.tar.bz2' bzip2_1.0.6-8ubuntu0.2.debian.tar.bz2 61599 SHA512:3c9ee464d8303a7c2c7a6dbaffd4bdd88752a65f1a2f968f8c4ed8084d732fb0c72614e5a88f4b9ee43228befb07ec5c283ab1e5995d38f7cd8239eab9c5101b
```

### `dpkg` source package: `bzr=2.7.0-2ubuntu3.1`

Binary Packages:

- `bzr=2.7.0-2ubuntu3.1`
- `python-bzrlib=2.7.0-2ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`, `/usr/share/doc/python-bzrlib/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.7.0-2ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0-2ubuntu3.1.dsc' bzr_2.7.0-2ubuntu3.1.dsc 2669 SHA512:83df8e0460915ea5b429b59a41ec8e9b84bf27ec1b1232dfc85d8ce5ae23d5c550e9ef0d5a791cca979790d04bce090b291e00afb646b0c7b6ee0ac0b1ede41c
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0.orig.tar.gz' bzr_2.7.0.orig.tar.gz 10944322 SHA512:824f740ec3521d5cbaf69f79a627a167a68a116df818aa4b3a391da459ce2e267851808199e3b250abce772813f1257cf3392efbfc5d2bfb495afcb98144d3bd
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0-2ubuntu3.1.debian.tar.xz' bzr_2.7.0-2ubuntu3.1.debian.tar.xz 42660 SHA512:3d6f07cadfac56c0aea0b8a02921d558ad6a16665abf6ce2b88b3277b8ae3fd9fe1d8cbd98571e3e637b361281a78996a69da15b9d469110716b4d5fcd727a7f
```

### `dpkg` source package: `ca-certificates=20190110~16.04.1`

Binary Packages:

- `ca-certificates=20190110~16.04.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~16.04.1.dsc' ca-certificates_20190110~16.04.1.dsc 1969 SHA512:612f47339876a9feddcce8d62f505e0b4d12fb21dbd173920aab0c6b050416270d92bf4fa24b457cc530ad141696d8eae5e5cb0a0856063f6ab350d77dcdebdf
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~16.04.1.tar.xz' ca-certificates_20190110~16.04.1.tar.xz 243584 SHA512:0bc6167a5c5c46a5cec8ba72e091c5ba4fc4707cd2f9f59cfb1a5bec42050b803987a76db8c42f6a88b115a33ba0b45f225294d06b45c54c051cdc4b6d851487
```

### `dpkg` source package: `cairo=1.14.6-1`

Binary Packages:

- `libcairo2:amd64=1.14.6-1`

Licenses: (parsed from: `/usr/share/doc/libcairo2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.14.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.14.6-1.dsc' cairo_1.14.6-1.dsc 2865 SHA256:1e3f66a22c364646c05a127bc1fcfecd04476a994e30b2e251c03f9ff09d55ce
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.14.6.orig.tar.xz' cairo_1.14.6.orig.tar.xz 36040596 SHA256:613cb38447b76a93ff7235e17acd55a78b52ea84a9df128c3f2257f8eaa7b252
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.14.6-1.debian.tar.xz' cairo_1.14.6-1.debian.tar.xz 27704 SHA256:83dbaa90cf79127db9c87edf3a4d38c193abc2d346555ab70bb619e899da5070
```

### `dpkg` source package: `cdebconf=0.198ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.198ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.198ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.198ubuntu1.dsc' cdebconf_0.198ubuntu1.dsc 2825 SHA256:d595d3afcad97026a763909a3efe66e296b02e432827d66a49c6f7088023a21e
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.198ubuntu1.tar.xz' cdebconf_0.198ubuntu1.tar.xz 269256 SHA256:2f3490411599195bd31fb1a29770694888c8295f9bf5012bfb4fa22ebd3990f1
```

### `dpkg` source package: `cmake=3.5.1-1ubuntu3`

Binary Packages:

- `cmake=3.5.1-1ubuntu3`
- `cmake-data=3.5.1-1ubuntu3`

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
$ apt-get source -qq --print-uris cmake=3.5.1-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.5.1-1ubuntu3.dsc' cmake_3.5.1-1ubuntu3.dsc 2556 SHA512:6601c99c03077d9741c61d4a7dfd247a02f7677cbf3ac1eba7999871a354f9ee385925946a30cb082157dafbb71ba9b4496d024a77806ceaa577e9c421e56f48
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.5.1.orig.tar.gz' cmake_3.5.1.orig.tar.gz 6863121 SHA512:f78185eb1a2344167888b13ce2a0e8657594bc9c4195c99f5a2be3f953dd2ff630081c2d63b180215851eec8c9565fab8ee1c481ca4c0e6eb9dc27b574d45616
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.5.1-1ubuntu3.debian.tar.xz' cmake_3.5.1-1ubuntu3.debian.tar.xz 34716 SHA512:58de72af90875ab654d234db8e30b26f8f5681e7845c028cdfa40f6bdbe36b7b56a622da966b21486f79d9e3fdc2c9b9b287741af218c808b9ffdab7070803d6
```

### `dpkg` source package: `configobj=5.0.6-2`

Binary Packages:

- `python-configobj=5.0.6-2`

Licenses: (parsed from: `/usr/share/doc/python-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-2.dsc' configobj_5.0.6-2.dsc 2381 SHA256:9bb8577128460ff33326d3d90b8454376c83f4d41b1da61aeabdbfcbfb5e0087
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA256:2e140354efcca6f558ff9ee941b435ae09a617bc071797bef62c8d6ed2033d5e
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-2.debian.tar.xz' configobj_5.0.6-2.debian.tar.xz 7436 SHA256:dc677cd329b4a3aacebe10c5a169d9d092cc27888c3f3f9203930cacd6a0eab8
```

### `dpkg` source package: `console-bridge=0.3.2-1`

Binary Packages:

- `libconsole-bridge-dev:amd64=0.3.2-1`
- `libconsole-bridge0.2v5:amd64=0.3.2-1`

Licenses: (parsed from: `/usr/share/doc/libconsole-bridge-dev/copyright`, `/usr/share/doc/libconsole-bridge0.2v5/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris console-bridge=0.3.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.3.2-1.dsc' console-bridge_0.3.2-1.dsc 1947 SHA256:4287ea47563a53e505d1c416b0be23292e367721b5d5541894155c4e76c7206f
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.3.2.orig.tar.gz' console-bridge_0.3.2.orig.tar.gz 231243 SHA256:fd12e48c672cb9c5d516d90429c4a7ad605859583fc23d98258c3fa7a12d89f4
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.3.2-1.debian.tar.xz' console-bridge_0.3.2-1.debian.tar.xz 4016 SHA256:e399cdf7fcbead93301e1061aac0460ed49f85c58f6911b120776a7e3cf02ad0
```

### `dpkg` source package: `coreutils=8.25-2ubuntu3~16.04`

Binary Packages:

- `coreutils=8.25-2ubuntu3~16.04`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.25-2ubuntu3~16.04
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.25-2ubuntu3~16.04.dsc' coreutils_8.25-2ubuntu3~16.04.dsc 2095 SHA512:c1b3746ab480ee4385d2d8549f7a756d3ecea36e800664d4fb329c65d7f9ce764cd1dfd71d284505b86c3b6150a23a7ed7c4e07e7c4e99fe7eb68b0faff9c58b
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.25.orig.tar.xz' coreutils_8.25.orig.tar.xz 5725008 SHA512:571f95d44987d373081ed4c6ac82155ad3dcd95621d7b1a7163597e80ecbbafef2cd74b2ef594587a443a1a4355083879f898a286bb0230c48112d43d076ccd6
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.25-2ubuntu3~16.04.debian.tar.xz' coreutils_8.25-2ubuntu3~16.04.debian.tar.xz 28336 SHA512:b92193304dcc20f01f2bdb49dae686d9c129abb059394523f23c251854714c9e3bda9304a46e13c685935afa215a533efc5969553c398a49d86447e298d9a3ee
```

### `dpkg` source package: `cryptsetup=2:1.6.6-5ubuntu2.1`

Binary Packages:

- `libcryptsetup4:amd64=2:1.6.6-5ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libcryptsetup4/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cryptsetup=2:1.6.6-5ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cryptsetup/cryptsetup_1.6.6-5ubuntu2.1.dsc' cryptsetup_1.6.6-5ubuntu2.1.dsc 2650 SHA512:e5836598fec56c67677d462f38d51eb997c708a5c7e5a44789cd62c18ceaf30080be61b98c92932122b7f3d563f80210fbfaed2b6c441490e38317ff61201277
'http://archive.ubuntu.com/ubuntu/pool/main/c/cryptsetup/cryptsetup_1.6.6.orig.tar.xz' cryptsetup_1.6.6.orig.tar.xz 1145940 SHA512:6ee6b4e8fe4f721bb97d1cf47c5e2d1c96001dd3ac48154d414f64d23620ac3ec3eeea2ad584a1a3111e07a086c8a4fdbfabdf4859cda58ba2bd6765b1f009a8
'http://archive.ubuntu.com/ubuntu/pool/main/c/cryptsetup/cryptsetup_1.6.6-5ubuntu2.1.debian.tar.xz' cryptsetup_1.6.6-5ubuntu2.1.debian.tar.xz 91808 SHA512:c17d030969620bdebe5e2822ab37d6996d15ac2d2483f91be86080c6f5793915b4b922e43d7e567abaea762076bee98d01c68e1d0f4cd058c3a2b8fbcfd5cf22
```

### `dpkg` source package: `cups=2.1.3-4ubuntu0.11`

Binary Packages:

- `libcups2:amd64=2.1.3-4ubuntu0.11`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.1.3-4ubuntu0.11
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3-4ubuntu0.11.dsc' cups_2.1.3-4ubuntu0.11.dsc 3755 SHA512:83bfa0f1ab5310d79ac3b00b6ee058ccb88431fe5f3f278bd30e35f73070a741c75856dd0f6fa0a9d76762ec384c7bd87349b8e542a6b768c2be4f04010526bc
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3.orig.tar.bz2' cups_2.1.3.orig.tar.bz2 8832400 SHA512:5cc715b8521b4d6af29a97a8abf7a1b0973840c00727ee8e7926e89a4a9da8e67565d14cc4b57ab7cfb40b238d4faaed7608b9ab95947cc3671ed87b710f8f36
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3-4ubuntu0.11.debian.tar.xz' cups_2.1.3-4ubuntu0.11.debian.tar.xz 356476 SHA512:b57ab661a003b62d60c90c0d22bdea4f046b0b052326f821070ed7c08b2a208fb2cfb789613f5a9ebec2c694916602d119862c9880904f45d266fdcff2e4ea9a
```

### `dpkg` source package: `curl=7.47.0-1ubuntu2.16`

Binary Packages:

- `libcurl3:amd64=7.47.0-1ubuntu2.16`
- `libcurl3-gnutls:amd64=7.47.0-1ubuntu2.16`

Licenses: (parsed from: `/usr/share/doc/libcurl3/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.47.0-1ubuntu2.16
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.47.0-1ubuntu2.16.dsc' curl_7.47.0-1ubuntu2.16.dsc 2733 SHA512:3421dcd95e341597dbd531b0c6056e299f7e61ed3e15d06a59f231988fc7508d337230658f50d3b1b90bb8d1346cd2ee4a58ef1c34cb553b0dd79579c939b4dc
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.47.0.orig.tar.gz' curl_7.47.0.orig.tar.gz 4563163 SHA512:567d6a17bad1439147a419eff7e3b4a8f81104e903d856a33a1ccfaf77723cc70004fa697505443a5edcee1b644eba2c79484b41c00e35320bec6ef928db43d9
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.47.0-1ubuntu2.16.debian.tar.xz' curl_7.47.0-1ubuntu2.16.debian.tar.xz 57440 SHA512:2a15355264bd5a4ab8fcabdbe3da4d94694b7606fc172fb12b1c4ed2692dc6174bd4cddf3b1adaa3ee40d250f1af6d84fe67b51e9876bf5a484ee108e6674c43
```

### `dpkg` source package: `cyrus-sasl2=2.1.26.dfsg1-14ubuntu0.2`

Binary Packages:

- `libsasl2-2:amd64=2.1.26.dfsg1-14ubuntu0.2`
- `libsasl2-modules-db:amd64=2.1.26.dfsg1-14ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.26.dfsg1-14ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.dsc' cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.dsc 3416 SHA512:fd0ce2535908f464fa0335848b002c7bf49c16d60eabebc1812e2d75cb0a61fea27586bba3e49102660af7d90319d7b9f32e4a05d2abfac75a7982c80ebd701a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz' cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz 1494337 SHA512:244b081cb8c58f2cc59e0a0c18bc91fc3b0659d2419e3aa435d4e39ab86c565141d96bad50295a90046b86dcad7e773b26a88e8271917d89c065988b8c9599ec
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.debian.tar.xz' cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.debian.tar.xz 95360 SHA512:f72b8e64cd49541046b9a759873aa61ee27db9ec230e17cbe240d8cc61b7da93be0754d51d692bee6557993829a565f052de5ec7a55230094ee53e256ca53e8d
```

### `dpkg` source package: `dash=0.5.8-2.1ubuntu2`

Binary Packages:

- `dash=0.5.8-2.1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.8-2.1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.1ubuntu2.dsc' dash_0.5.8-2.1ubuntu2.dsc 1882 SHA256:16cb7f56041a9daa198728715318a5d88c19da01eb3ffccbc71f67304b077564
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8.orig.tar.gz' dash_0.5.8.orig.tar.gz 223028 SHA256:c6db3a237747b02d20382a761397563d813b306c020ae28ce25a1c3915fac60f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.1ubuntu2.diff.gz' dash_0.5.8-2.1ubuntu2.diff.gz 73054 SHA256:3c200a0b9c88b2e421bce9c717bf2ace7a9378c271a9b60463913e312424565a
```

### `dpkg` source package: `db5.3=5.3.28-11ubuntu0.2`

Binary Packages:

- `libdb5.3:amd64=5.3.28-11ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-11ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-11ubuntu0.2.dsc' db5.3_5.3.28-11ubuntu0.2.dsc 3182 SHA512:6b376d9d7286bf3a09ed1d1c8113a8bfaa99276424691e42d952393fcab04d9f317de621d24bfd7c33b1a2f6ac92c3d781c83f904c0dc8af55c8ea99eaa530da
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA512:080483cac3119569e04c3c22c95e97e5e448c88d87a443933d0ef2c71b506f309428584d6a8fb9c236c616dd82beffa1b30361b4c918756745983fcf54a3f8da
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-11ubuntu0.2.debian.tar.xz' db5.3_5.3.28-11ubuntu0.2.debian.tar.xz 29312 SHA512:63be9f279a67cc56ddacccd3a4b419d83e1a081c7b104c0a05d845a4e65c81aab51fc46e676a27c51f52cad038041e10f2ffbca64cbde6d006537cb0a53d2b66
```

### `dpkg` source package: `dbus=1.10.6-1ubuntu3.6`

Binary Packages:

- `libdbus-1-3:amd64=1.10.6-1ubuntu3.6`

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
$ apt-get source -qq --print-uris dbus=1.10.6-1ubuntu3.6
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6-1ubuntu3.6.dsc' dbus_1.10.6-1ubuntu3.6.dsc 3090 SHA512:c0e69e543f96117580c2db0bb037c24ec9b83f63a3562c1f2e101503615c2bdff0d419d8fe5e286966d47e779a3be3529c7a6152e647742a715ba4b3b81cb03c
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6.orig.tar.gz' dbus_1.10.6.orig.tar.gz 1952608 SHA512:56108dde5097b063b25ef6e42e573b7e1affd5b5a6ce3c745e2de21b434d86542ac6b7c384572826f867a5c471692cc7468c74c4b0cf4a1f60a1a41b0394fb3c
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6-1ubuntu3.6.debian.tar.xz' dbus_1.10.6-1ubuntu3.6.debian.tar.xz 66784 SHA512:db7a48f3dd0ec0faa1f5270ae4a2863119c7badc0ed68c357cc16361bea2b5bada8e39f6005161443b20322861e063b51258f2d7e5fec9217b026e0a7f016c5d
```

### `dpkg` source package: `debconf=1.5.58ubuntu2`

Binary Packages:

- `debconf=1.5.58ubuntu2`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.58ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.58ubuntu2.dsc' debconf_1.5.58ubuntu2.dsc 2076 SHA512:5703f7ec92cd0247f94ee8384bbb395d37fb0d98ad6ca891cdd597e3dc124e64fa2f2b91687a2e5e10e196feef1dd32ebf9ee7565f8e7a39584e01002b43ea9d
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.58ubuntu2.tar.gz' debconf_1.5.58ubuntu2.tar.gz 1007295 SHA512:1b1f8f779e0cc2fb1580a7381599a47b0c27a0f68da90f07023edb178ea8bffe9a205c3ecf002f6496445225b158c3dc4a827cca24f2f1755384bfc67b3000ef
```

### `dpkg` source package: `debianutils=4.7`

Binary Packages:

- `debianutils=4.7`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.7
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.7.dsc' debianutils_4.7.dsc 1703 SHA256:8dd1d66186f56bfe11bce5151b50c6909787d690bf90cc90212ea6deec186460
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.7.tar.xz' debianutils_4.7.tar.xz 156276 SHA256:a269cacd40f52f2fa5d5636357714a49e8538459c16d77772efaa23711fe53d9
```

### `dpkg` source package: `defusedxml=0.4.1-2ubuntu0.16.04.1`

Binary Packages:

- `python-defusedxml=0.4.1-2ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/python-defusedxml/copyright`)

- `Python`

Source:

```console
$ apt-get source -qq --print-uris defusedxml=0.4.1-2ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.4.1-2ubuntu0.16.04.1.dsc' defusedxml_0.4.1-2ubuntu0.16.04.1.dsc 2284 SHA512:f3b5ba671d9b6ce9bdab03d38acbea4bd6019c02b0423b2b61afc535c1ea0c27272b19495c0d10b95afae9fbe9b9a47b46abadd3a0075f1e426e8479c9aa32f1
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.4.1.orig.tar.gz' defusedxml_0.4.1.orig.tar.gz 48889 SHA512:78a7a1f3d1eed9d7cda00afaaccf8153c7f616303c53d3918341d75970d532932b04effcfc8b1b8ed88ba6d730cb56400e9e4ecee8aa7d2181c7577f1d535783
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.4.1-2ubuntu0.16.04.1.debian.tar.xz' defusedxml_0.4.1-2ubuntu0.16.04.1.debian.tar.xz 15700 SHA512:86e8b47872d84a1d1bf2fa547c85ffade5f06071b417da6dd2f3b05acdc3267cc4ad7aff8b8f5ae3ba845800a94336dc27e2a020405a955466dd31126c0da1c4
```

### `dpkg` source package: `dh-python=2.20151103ubuntu1.2`

Binary Packages:

- `dh-python=2.20151103ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/dh-python/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris dh-python=2.20151103ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dh-python/dh-python_2.20151103ubuntu1.2.dsc' dh-python_2.20151103ubuntu1.2.dsc 1834 SHA512:9e3faac414ba96ce4588a19d450bb48a4b21d405a2d1ff1f7bc3fc20db496788d19f7685ac47fd97c09d1d994e204f0e0f9ad62e4b607d55137461b21d590c09
'http://archive.ubuntu.com/ubuntu/pool/main/d/dh-python/dh-python_2.20151103ubuntu1.2.tar.xz' dh-python_2.20151103ubuntu1.2.tar.xz 79844 SHA512:61236ba062a85d0476d8b8ff0e262192726382296a908809b16c27c0586a7da29af2d0c7af2cd5273d3f6266be610bbaba87c9e1247429f7bf4f2e4287527e2f
```

### `dpkg` source package: `diffutils=1:3.3-3`

Binary Packages:

- `diffutils=1:3.3-3`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.3-3
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.3-3.dsc' diffutils_3.3-3.dsc 1438 SHA256:2ac1b096ab1f6f0c628d6952fe65336d0c792a3d4814fb73a81a3f1f518eff91
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.3.orig.tar.xz' diffutils_3.3.orig.tar.xz 1197832 SHA256:a25e89a8ab65fded1731e4186be1bb25cda967834b6df973599cdcd5abdfc19c
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.3-3.debian.tar.xz' diffutils_3.3-3.debian.tar.xz 18356 SHA256:a0d1946979196f793a8ca55b21ab7891227de08f15bac2578ed84f4911e8b755
```

### `dpkg` source package: `distro-info-data=0.28ubuntu0.14`

Binary Packages:

- `distro-info-data=0.28ubuntu0.14`

Licenses: (parsed from: `/usr/share/doc/distro-info-data/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris distro-info-data=0.28ubuntu0.14
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.28ubuntu0.14.dsc' distro-info-data_0.28ubuntu0.14.dsc 1761 SHA512:3b4b9997d809ff28276131d5308dc1a7f89b5d6164fc712a833abb1417ca25aa67d44a5de6c43dcca69795cd2f215e4b5a69bea9fb659268036cb7ace4d795b6
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.28ubuntu0.14.tar.xz' distro-info-data_0.28ubuntu0.14.tar.xz 7280 SHA512:5a3b34ad67e6e2ee2080dffbb577be798cd8c10227ed9391f57967b31798248165f9c037bfae7a3867df624ce90d9cc9e33140ab467e1e5b6d6ddab769cb9c50
```

### `dpkg` source package: `dpkg=1.18.4ubuntu1.6`

Binary Packages:

- `dpkg=1.18.4ubuntu1.6`
- `dpkg-dev=1.18.4ubuntu1.6`
- `libdpkg-perl=1.18.4ubuntu1.6`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.18.4ubuntu1.6
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.18.4ubuntu1.6.dsc' dpkg_1.18.4ubuntu1.6.dsc 2211 SHA512:aad304d96fcfb39f53f04b3ee90b0d648f52881fa66d0dcd8543afaac6b785fc34783b79070e40bb26352a0b7a00f08be4c221edccf11b6f9c8c3a9fa39b45f1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.18.4ubuntu1.6.tar.xz' dpkg_1.18.4ubuntu1.6.tar.xz 4297512 SHA512:6b270f36d7d65e93dc8d70c695d1cdb160f7b168588df6cfbf62d8800de130bee01176332e9b13177f47e0c036ec2a3dc586cec2a6c6e18f00f79b3cd7bf6365
```

### `dpkg` source package: `e2fsprogs=1.42.13-1ubuntu1.2`

Binary Packages:

- `e2fslibs:amd64=1.42.13-1ubuntu1.2`
- `e2fsprogs=1.42.13-1ubuntu1.2`
- `libcomerr2:amd64=1.42.13-1ubuntu1.2`
- `libss2:amd64=1.42.13-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.42.13-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.42.13-1ubuntu1.2.dsc' e2fsprogs_1.42.13-1ubuntu1.2.dsc 2606 SHA512:02793a1deac21bdbd72aea42f684673c945f7ab33d659bef5245caa42a30d752d5bdfcfd6c672c87907508822819025bb3ce75603e7be61ea4d61717167ed06d
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.42.13.orig.tar.gz' e2fsprogs_1.42.13.orig.tar.gz 6511931 SHA512:d341790f55c3bff34425369063757280b9ba6ac08f405e14f94f299345ae76c0dc6e90871b746cc98c73467448d888fe5bc029688b5eed5fd22c3c37bf285cd0
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.42.13-1ubuntu1.2.debian.tar.xz' e2fsprogs_1.42.13-1ubuntu1.2.debian.tar.xz 72228 SHA512:db80956f2ed3e90ee888017843a1269f09dbb3e03f6adf2596983309189f8e131f68c06490673d69af7edae336d66446aea6e8fe488b1ad17cf2ba79bbd6ae98
```

### `dpkg` source package: `elfutils=0.165-3ubuntu1.2`

Binary Packages:

- `libelf1:amd64=0.165-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.165-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.165-3ubuntu1.2.dsc' elfutils_0.165-3ubuntu1.2.dsc 2393 SHA512:5f37104f950b615598a51c9f2d88996c4ad0db614bd63d8996e7cc7230dee3543d5c36705906a6c8f6dd6066ecbacd328c2fc6455e22302c7cf43b2f0723bf5f
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.165.orig.tar.bz2' elfutils_0.165.orig.tar.bz2 6481128 SHA512:89d42a32f1d77d3419473165e1ac15782765ce6ec842d63f03962260806fbfdf16d17b8abec8527d8b125b9195c24a56252070b0c6ae860ffcf0dd74943da32a
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.165-3ubuntu1.2.debian.tar.xz' elfutils_0.165-3ubuntu1.2.debian.tar.xz 52004 SHA512:acd8f208ffd461307216cfad95bb84c16ab77d6dfad17787bf75c0a571f57e33f95024f4245d043fe720dc53ed77f237b50e02d5655736d71e6e4fd100bcacba
```

### `dpkg` source package: `empy=3.3.2-1build1`

Binary Packages:

- `python-empy=3.3.2-1build1`

Licenses: (parsed from: `/usr/share/doc/python-empy/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris empy=3.3.2-1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2-1build1.dsc' empy_3.3.2-1build1.dsc 2161 SHA256:4fee77941fc5406214e9d2387b631040165329e0084319e5f5af52c0df948862
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2.orig.tar.gz' empy_3.3.2.orig.tar.gz 138168 SHA256:99f016af2770c48ab57a65df7aae251360dc69a1514c15851458a71d4ddfea9c
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2-1build1.debian.tar.xz' empy_3.3.2-1build1.debian.tar.xz 4688 SHA256:50eae836a5dbde23d563ef04b96e6e1f7bfc2cab6ab6ed1d62c68aacc235af21
```

### `dpkg` source package: `expat=2.1.0-7ubuntu0.16.04.5`

Binary Packages:

- `libexpat1:amd64=2.1.0-7ubuntu0.16.04.5`
- `libexpat1-dev:amd64=2.1.0-7ubuntu0.16.04.5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.1.0-7ubuntu0.16.04.5
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0-7ubuntu0.16.04.5.dsc' expat_2.1.0-7ubuntu0.16.04.5.dsc 2387 SHA512:8b3d97e198ef1d6024f39c8797c7cba4ceda7b6483fdeb8a4a27d706209c397669aa969e1e7ca4a3b15de6d894766881914fdcf574af8a3191f5a23b5b8ab9b3
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0.orig.tar.gz' expat_2.1.0.orig.tar.gz 562616 SHA512:2a9ad2b44b87b84087979fe4114d661838df3b03dbdcb74d590cb74096bf35ce9d5a86617b0941a2655ea441a94537bcbcd78252da92342238823be36de2d09d
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0-7ubuntu0.16.04.5.debian.tar.xz' expat_2.1.0-7ubuntu0.16.04.5.debian.tar.xz 23116 SHA512:fd79b62dde2cde33ca7d14c5b5fd99d0ad14d4d63b0332470e5ed103d64f1ed0d39670ac8a313a39193a3f4cf1c3c67b5f24d4db4eb64200b6f8c2f1f9d9daea
```

### `dpkg` source package: `explorercanvas=0.r3-4`

Binary Packages:

- `libjs-excanvas=0.r3-4`

Licenses: (parsed from: `/usr/share/doc/libjs-excanvas/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris explorercanvas=0.r3-4
'http://archive.ubuntu.com/ubuntu/pool/universe/e/explorercanvas/explorercanvas_0.r3-4.dsc' explorercanvas_0.r3-4.dsc 2000 SHA256:d168011ed1f110f82b5039a6b070167f1f262d2a35d7fa25a6b5462f73761637
'http://archive.ubuntu.com/ubuntu/pool/universe/e/explorercanvas/explorercanvas_0.r3.orig.tar.gz' explorercanvas_0.r3.orig.tar.gz 50748 SHA256:687af8084781b8eb3451fc55c88f6dfddc2b84428d197daf2c4c33fd5c55fed8
'http://archive.ubuntu.com/ubuntu/pool/universe/e/explorercanvas/explorercanvas_0.r3-4.debian.tar.xz' explorercanvas_0.r3-4.debian.tar.xz 2040 SHA256:afcaa3e229d9b423988fc30439aeee1599c9dac8ad94430309404f9cf9f0c11f
```

### `dpkg` source package: `findutils=4.6.0+git+20160126-2`

Binary Packages:

- `findutils=4.6.0+git+20160126-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20160126-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20160126-2.dsc' findutils_4.6.0+git+20160126-2.dsc 2163 SHA256:b4b644696cb66bdf72c59b25efe61800ae20fadfcc8e633cde240e4a956567a7
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20160126.orig.tar.xz' findutils_4.6.0+git+20160126.orig.tar.xz 1710188 SHA256:3d25cef1e0d5e098e323b06f66aea9f02f993a0cf6f13a437d712a8a722cd67e
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20160126-2.debian.tar.xz' findutils_4.6.0+git+20160126-2.debian.tar.xz 25080 SHA256:58bf1e7a07fbac6a68693b099ec6fc9a6166e0b1b60cebe6bac3b90287a8dc3f
```

### `dpkg` source package: `fontconfig=2.11.94-0ubuntu1.1`

Binary Packages:

- `fontconfig=2.11.94-0ubuntu1.1`
- `fontconfig-config=2.11.94-0ubuntu1.1`
- `libfontconfig1:amd64=2.11.94-0ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.11.94-0ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.11.94-0ubuntu1.1.dsc' fontconfig_2.11.94-0ubuntu1.1.dsc 2287 SHA512:2bdd80817fff2184ecb2169cfa1236f4498ada9c75723598b9f29603f96d395451366c8da164950b79f203abae72d2f425333bd9b401b08d455e8252223ec49f
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.11.94.orig.tar.bz2' fontconfig_2.11.94.orig.tar.bz2 1567540 SHA512:ab0639afbe37c46197aa31178f928a000e0662edf794bcd421e396bae2298edc23851ff58deeb448cc14ac1206683494817a64a75ab9f7bb9bce6321ccf5c1f2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.11.94-0ubuntu1.1.debian.tar.xz' fontconfig_2.11.94-0ubuntu1.1.debian.tar.xz 27932 SHA512:dd1759cff6acc99a2d3a0698cbf161dfa261ae96492651c4f72fd2749972f8012fdc187dc1a1c8542d767bb07684e766a9bfbbf50353781cd80c8b13df57b136
```

### `dpkg` source package: `fonts-dejavu=2.35-1`

Binary Packages:

- `fonts-dejavu-core=2.35-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.35-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.35-1.dsc' fonts-dejavu_2.35-1.dsc 2583 SHA256:b02163fb4033175371a6cb6e39e193d438d910ab907eed5d14b47a3a5e57b392
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.35.orig.tar.bz2' fonts-dejavu_2.35.orig.tar.bz2 11493699 SHA256:646f5f52fbba7c6c82580a22cedb487f31ecf28aa28c71da5c38e04c2989abf5
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.35-1.debian.tar.xz' fonts-dejavu_2.35-1.debian.tar.xz 10276 SHA256:5922af28fff7db4c5845c17623fe882028742f90db658f4183c21648e0cafd3d
```

### `dpkg` source package: `freetype=2.6.1-0.1ubuntu2.4`

Binary Packages:

- `libfreetype6:amd64=2.6.1-0.1ubuntu2.4`

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
$ apt-get source -qq --print-uris freetype=2.6.1-0.1ubuntu2.4
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.6.1-0.1ubuntu2.4.dsc' freetype_2.6.1-0.1ubuntu2.4.dsc 2236 SHA512:2e8d7964b960f23307c407ead2bcb2b8eded34d8201b8263f4c37dbc566a92e7f80ef03dd31d3a38d8841425188c5db9d7234073b35890c42a0991cda1016889
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.6.1.orig.tar.gz' freetype_2.6.1.orig.tar.gz 2411537 SHA512:526dfe1aa98631f1e4af7d01d00dc93128df426f4df00e41b4a2132914e9218945fbd92e06a4ad7adcd84812752613d0f5c7938c8d69626a802cf01e1dc527ef
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.6.1-0.1ubuntu2.4.diff.gz' freetype_2.6.1-0.1ubuntu2.4.diff.gz 45130 SHA512:382d19492cc089922e771d7f1d8fd41781d83bc80edc2362040b9f24eb9cccfc124ec578f3c67015c86e8ef337c1cb283eccbdc26c40cef2690d7cb9034fd420
```

### `dpkg` source package: `gcc-4.8=4.8.5-4ubuntu2`

Binary Packages:

- `gcc-4.8-base:amd64=4.8.5-4ubuntu2`
- `libasan0:amd64=4.8.5-4ubuntu2`
- `libgcc-4.8-dev:amd64=4.8.5-4ubuntu2`
- `libstdc++-4.8-dev:amd64=4.8.5-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/gcc-4.8-base/copyright`, `/usr/share/doc/libasan0/copyright`, `/usr/share/doc/libgcc-4.8-dev/copyright`, `/usr/share/doc/libstdc++-4.8-dev/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-4.8=4.8.5-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-4.8/gcc-4.8_4.8.5-4ubuntu2.dsc' gcc-4.8_4.8.5-4ubuntu2.dsc 12216 SHA256:d0a98e616e0f87c434149ff4c352e814e8ee41c877f069f8fb53df0ea9bc41ae
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-4.8/gcc-4.8_4.8.5.orig.tar.gz' gcc-4.8_4.8.5.orig.tar.gz 66569326 SHA256:9c3263058e5fc8a89147fdc03afafcf1cfc6912c3d034e2ceabe40966d4bb4f7
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-4.8/gcc-4.8_4.8.5-4ubuntu2.diff.gz' gcc-4.8_4.8.5-4ubuntu2.diff.gz 950839 SHA256:ee26de30eb1e0b5d73f73e387853539b6e609fcb25ec581c11081f49c9332a9a
```

### `dpkg` source package: `gcc-5=5.4.0-6ubuntu1~16.04.12`

Binary Packages:

- `cpp-5=5.4.0-6ubuntu1~16.04.12`
- `g++-5=5.4.0-6ubuntu1~16.04.12`
- `gcc-5=5.4.0-6ubuntu1~16.04.12`
- `gcc-5-base:amd64=5.4.0-6ubuntu1~16.04.12`
- `libasan2:amd64=5.4.0-6ubuntu1~16.04.12`
- `libatomic1:amd64=5.4.0-6ubuntu1~16.04.12`
- `libcc1-0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libcilkrts5:amd64=5.4.0-6ubuntu1~16.04.12`
- `libgcc-5-dev:amd64=5.4.0-6ubuntu1~16.04.12`
- `libgfortran3:amd64=5.4.0-6ubuntu1~16.04.12`
- `libgomp1:amd64=5.4.0-6ubuntu1~16.04.12`
- `libitm1:amd64=5.4.0-6ubuntu1~16.04.12`
- `liblsan0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libmpx0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libquadmath0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libstdc++-5-dev:amd64=5.4.0-6ubuntu1~16.04.12`
- `libstdc++6:amd64=5.4.0-6ubuntu1~16.04.12`
- `libtsan0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libubsan0:amd64=5.4.0-6ubuntu1~16.04.12`

Licenses: (parsed from: `/usr/share/doc/cpp-5/copyright`, `/usr/share/doc/g++-5/copyright`, `/usr/share/doc/gcc-5/copyright`, `/usr/share/doc/gcc-5-base/copyright`, `/usr/share/doc/libasan2/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-5-dev/copyright`, `/usr/share/doc/libgfortran3/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libmpx0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-5-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-5=5.4.0-6ubuntu1~16.04.12
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-5/gcc-5_5.4.0-6ubuntu1~16.04.12.dsc' gcc-5_5.4.0-6ubuntu1~16.04.12.dsc 28298 SHA512:d1f8116726cfad5d406849be8dd47fa6a0c5e40db65e284eaca6cb71e86b03ad854a9f843199d7f46c430fb72a5047f8eb9be27a0f9f656b8a781d6f9eed3a0b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-5/gcc-5_5.4.0.orig.tar.gz' gcc-5_5.4.0.orig.tar.gz 73530162 SHA512:8ce644f7b67b999036d134443518da4fd4ccc3c838f9015dc18bf15dc8ef006e8a53bb4dd7dd1fcc4a8cfd9bd2b6e5e223e57c0474ea7c5c74f7b26d669bbdef
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-5/gcc-5_5.4.0-6ubuntu1~16.04.12.diff.gz' gcc-5_5.4.0-6ubuntu1~16.04.12.diff.gz 1486130 SHA512:bb05d04b8f0f0a3f333754d46bbb28365d8d6f4ea67b57c0c0f0d48fda9ba5f884b3eb1324a3fef259b8ae90497a70b44693aed5491639113502466b191473bf
```

### `dpkg` source package: `gcc-defaults=1.150ubuntu1`

Binary Packages:

- `cpp=4:5.3.1-1ubuntu1`
- `g++=4:5.3.1-1ubuntu1`
- `gcc=4:5.3.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.150ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.150ubuntu1.dsc' gcc-defaults_1.150ubuntu1.dsc 12634 SHA256:5f538e1bb59109b47d820cdd056993d462f24468c67f6a1a005db389dffa8ee2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.150ubuntu1.tar.gz' gcc-defaults_1.150ubuntu1.tar.gz 73857 SHA256:cadaf435151fb1b901b0351d20a9981fe33d94fbb1ab14bd9960095b673ce6ed
```

### `dpkg` source package: `gccgo-6=6.0.1-0ubuntu1`

Binary Packages:

- `gcc-6-base:amd64=6.0.1-0ubuntu1`
- `libgcc1:amd64=1:6.0.1-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-6-base/copyright`, `/usr/share/doc/libgcc1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gccgo-6=6.0.1-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gccgo-6/gccgo-6_6.0.1-0ubuntu1.dsc' gccgo-6_6.0.1-0ubuntu1.dsc 11285 SHA256:4c02817baac83492323ebe7800d44de609eca147518682307a3bad2bd5134129
'http://archive.ubuntu.com/ubuntu/pool/main/g/gccgo-6/gccgo-6_6.0.1.orig.tar.gz' gccgo-6_6.0.1.orig.tar.gz 76335555 SHA256:daff7478ce52d00572683547c810bf50652a9057c33e3ce703c9f0baae28f4c3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gccgo-6/gccgo-6_6.0.1-0ubuntu1.diff.gz' gccgo-6_6.0.1-0ubuntu1.diff.gz 633954 SHA256:839eea6c2d23670f09b642864ff61e3097b47391cb508a5997538750ff8678f6
```

### `dpkg` source package: `gdbm=1.8.3-13.1`

Binary Packages:

- `libgdbm3:amd64=1.8.3-13.1`

Licenses: (parsed from: `/usr/share/doc/libgdbm3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.8.3-13.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.8.3-13.1.dsc' gdbm_1.8.3-13.1.dsc 1830 SHA256:b1d8bef30edc491315c337930cbe2b61f44f55035adfc26ae945bab5ca57d5c9
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.8.3.orig.tar.bz2' gdbm_1.8.3.orig.tar.bz2 172796 SHA256:1d5995b6e9e6be4ff62c8126d019f184a083dd8e6f75f6c74b9fe023b5b9440e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.8.3-13.1.debian.tar.xz' gdbm_1.8.3-13.1.debian.tar.xz 14748 SHA256:251401e1f5210226f384e936b1b7ea1df40119a918d9f3dbf48b2e51d4df8983
```

### `dpkg` source package: `gdk-pixbuf=2.32.2-1ubuntu1.6`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.32.2-1ubuntu1.6`
- `libgdk-pixbuf2.0-common=2.32.2-1ubuntu1.6`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.32.2-1ubuntu1.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2-1ubuntu1.6.dsc' gdk-pixbuf_2.32.2-1ubuntu1.6.dsc 2912 SHA512:1b85fb61d682862068166c135c098b1030c82f510f1d22f2afa306ca6959706cc93c7d91d98dafdc6c1867fed9b80a48cc9c4aaa96b1a2fbaae47e07893cb3ac
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2.orig.tar.xz' gdk-pixbuf_2.32.2.orig.tar.xz 2429268 SHA512:146cbddc1b4a68715a827fc53d98f213f5e27f4f4a8b3fe6148b96c866b4ca4ab624613ddf196d4b0a01bbddfc6f8438b96ad436d23dfced02d584ff8c2fdf3d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2-1ubuntu1.6.debian.tar.xz' gdk-pixbuf_2.32.2-1ubuntu1.6.debian.tar.xz 19956 SHA512:11f46e2d5e92606ecf8e1c3978e00f71af0e926cc89339de710d46f0a8ef930306f2027a3f7a37920ed6f5f94ed4edc1c257f551acef19f1a45e1ef649a19437
```

### `dpkg` source package: `git=1:2.7.4-0ubuntu1.9`

Binary Packages:

- `git=1:2.7.4-0ubuntu1.9`
- `git-core=1:2.7.4-0ubuntu1.9`
- `git-man=1:2.7.4-0ubuntu1.9`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-core/copyright`, `/usr/share/doc/git-man/copyright`)

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
$ apt-get source -qq --print-uris git=1:2.7.4-0ubuntu1.9
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.7.4-0ubuntu1.9.dsc' git_2.7.4-0ubuntu1.9.dsc 2897 SHA512:d7abca57876573c5230b6b04e863bd44025fd3c49126347e3f8caa674a7cabd37437c0da5df9ff661038c596971d6a9c792c714cda6f923d57d49d44a2ddf5fd
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.7.4.orig.tar.xz' git_2.7.4.orig.tar.xz 3909636 SHA512:82a646140834e909bf1748a017e86f37f0711c759fe0a6ad03529beb57c79742cb7bf77c2dba29ccd84fcf3d5f18ad9c85c00f002d3b257be42e058750423da7
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.7.4-0ubuntu1.9.debian.tar.xz' git_2.7.4-0ubuntu1.9.debian.tar.xz 572052 SHA512:0a9453fef5e580632d25251f73b84db8ddf0f57fb0e84d35bdc13d021f819a92284be45f9e6ed4128629d12a969af63c5cfa18c2620ce2baa8705d80a23e6a0e
```

### `dpkg` source package: `glib2.0=2.48.2-0ubuntu4.6`

Binary Packages:

- `libglib2.0-0:amd64=2.48.2-0ubuntu4.6`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.48.2-0ubuntu4.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2-0ubuntu4.6.dsc' glib2.0_2.48.2-0ubuntu4.6.dsc 2865 SHA512:27ebceac33635ecddd3d157990d1c0e2adc76de62c0cc103606f7c5e35ecab87325556209d2673e8b0f94117f5eb8a2d5d3eaf369325b9cba4521777b9226c28
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2.orig.tar.xz' glib2.0_2.48.2.orig.tar.xz 6408644 SHA512:2eac104eb2207d0a6488992e48069a34b417f51e141364f281ab7b0953a6de88be177b1c694dd9464a856c9a5d8021e3cf0193a8d9c5aaf6ea11f1f9ff743c43
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2-0ubuntu4.6.debian.tar.xz' glib2.0_2.48.2-0ubuntu4.6.debian.tar.xz 77696 SHA512:6590daeac98ac079af9fdc69f9ab8f6e0a23e8629a839596593a0fde6b907891465c807bf40e6f8667edeef8ba2ee337c067ff0ebea10569fa343cbafa1b6905
```

### `dpkg` source package: `glibc=2.23-0ubuntu11.2`

Binary Packages:

- `libc-bin=2.23-0ubuntu11.2`
- `libc-dev-bin=2.23-0ubuntu11.2`
- `libc6:amd64=2.23-0ubuntu11.2`
- `libc6-dev:amd64=2.23-0ubuntu11.2`
- `multiarch-support=2.23-0ubuntu11.2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.23-0ubuntu11.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23-0ubuntu11.2.dsc' glibc_2.23-0ubuntu11.2.dsc 8547 SHA512:ffec943c7f38c6f9dbec447b1bacbb9470207d09fbc3ba65b577a9f1135a5e099029bf54eb8e645ad6f25a9e92543f2ead8d3bd6454a359456c305dec85abffc
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23.orig.tar.xz' glibc_2.23.orig.tar.xz 13849968 SHA512:f2c3460d04226cbb5ff54755efb6f337356d9c063d71f736d8e5f631aaa85bfa89c4e2da1cd29f93383310994a18b21327512efd145d4c8dffd6c1412a002191
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23-0ubuntu11.2.debian.tar.xz' glibc_2.23-0ubuntu11.2.debian.tar.xz 1357888 SHA512:65e33ec8c2b9f4f94ec39cc6f330e14d651dc3aba5237d54a3a825b3e9c92afdf489c83d9115ec1324c8e1d602ad7fd43baa120dd03775f1aa47220514c45b02
```

### `dpkg` source package: `gmp=2:6.1.0+dfsg-2`

Binary Packages:

- `libgmp10:amd64=2:6.1.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.0+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.0+dfsg-2.dsc' gmp_6.1.0+dfsg-2.dsc 2161 SHA256:a790b4fea2792f968014a3ef41ea749dcc6687bcb33aa5bea59400ccd101337e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.0+dfsg.orig.tar.xz' gmp_6.1.0+dfsg.orig.tar.xz 1786120 SHA256:78a74cfd933bbdf7e93909a6069e53e8aba8389e9b3880300c926da7a7d55632
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.0+dfsg-2.debian.tar.xz' gmp_6.1.0+dfsg-2.debian.tar.xz 20576 SHA256:c933e3cb45cd4101cc0604b5bc0fb96d6067b3614e730dbf26588985720ba581
```

### `dpkg` source package: `gnupg2=2.1.11-6ubuntu2.1`

Binary Packages:

- `dirmngr=2.1.11-6ubuntu2.1`
- `gnupg-agent=2.1.11-6ubuntu2.1`
- `gnupg2=2.1.11-6ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg-agent/copyright`, `/usr/share/doc/gnupg2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `RFC-Reference`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris gnupg2=2.1.11-6ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.1.11-6ubuntu2.1.dsc' gnupg2_2.1.11-6ubuntu2.1.dsc 2725 SHA512:95c7b89084a63a0c7b394a8b972d47471a053cff02dcec35a1e60b8385aa8639e107191da9ca63e2374d128edbdc71ea6b6fa439d30bd1309ef538dfa2e04b29
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.1.11.orig.tar.bz2' gnupg2_2.1.11.orig.tar.bz2 5224007 SHA512:b39f3fb461ad879b1909808434c4b03dab4d1d79aa674fbc88e3d50960184c0c25a840206ff32b760672f1b2153253f4d7a88eb726d8662f629fa04b6739ad31
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.1.11-6ubuntu2.1.debian.tar.bz2' gnupg2_2.1.11-6ubuntu2.1.debian.tar.bz2 34752 SHA512:05e12ddfef0609ed06782acf5b346a02fb581109fdd3be83648215a87acb4043680a09df64f2e55c1b869d5f52cfaaf4e7ab5d33010687634ff6e0fbf7c646dd
```

### `dpkg` source package: `gnupg=1.4.20-1ubuntu3.3`

Binary Packages:

- `gnupg=1.4.20-1ubuntu3.3`
- `gpgv=1.4.20-1ubuntu3.3`

Licenses: (parsed from: `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gpgv/copyright`)

- `GPL-3`
- `GPL-3+ with OpenSSL exception`
- `RFC-Reference`

Source:

```console
$ apt-get source -qq --print-uris gnupg=1.4.20-1ubuntu3.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg/gnupg_1.4.20-1ubuntu3.3.dsc' gnupg_1.4.20-1ubuntu3.3.dsc 2166 SHA512:e5e296ded101c8ca30f0a9ddc77ada39a858723af939770c68beb04337df05fb1559b2cc13404b9719e45e3b983121a115414aef196fe1b61f09374a340f43dd
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg/gnupg_1.4.20.orig.tar.gz' gnupg_1.4.20.orig.tar.gz 5156447 SHA512:878a704ca5d69dc56f857b4b7af8927a38c19da78a0096451c8ccb23bc1df83d229a3d12546a4af41270b4d5b237d054e9ccb5e694d7d9f2b30b1c31baeb8cc5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg/gnupg_1.4.20-1ubuntu3.3.debian.tar.xz' gnupg_1.4.20-1ubuntu3.3.debian.tar.xz 42452 SHA512:22bd977c1e092c97c2e9409f4a10e38d9ee45826c036e2cf6eb8f0955a768e850fb4864525352a524a684668e582058abcf2bae8813bdf8358042a38aafc1e6f
```

### `dpkg` source package: `gnutls28=3.4.10-4ubuntu1.8`

Binary Packages:

- `libgnutls30:amd64=3.4.10-4ubuntu1.8`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `GPLv3+`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The main library is licensed under GNU Lesser`
- `nonstandard, see below`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.4.10-4ubuntu1.8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.4.10-4ubuntu1.8.dsc' gnutls28_3.4.10-4ubuntu1.8.dsc 2439 SHA512:03544c1f1f795de1604bbcba4750ee5e6e5ca3f9a75f9dd9d0c623c3510e55912ae578abb2287727870fbf079c4c3df9bde8c63251f884adcddd1d35a4dd8579
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.4.10.orig.tar.xz' gnutls28_3.4.10.orig.tar.xz 6645892 SHA512:e5cd60240ebbcac9d8f7c28fdbf023a499e3c58a352a43c24d075b248a0a903161b1745641bf263519293c0014424cc23dbb67274c8934aaf273a523ad0a2925
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.4.10-4ubuntu1.8.debian.tar.xz' gnutls28_3.4.10-4ubuntu1.8.debian.tar.xz 113000 SHA512:5ac07e360614f7ad60c917c2c373c00b6dc1dad07f34b1b761d8c6e9a8154f0e6f714b4542d22e4b4d7c31b8d4111b59e086fb0503064131bf8207002457fe0f
```

### `dpkg` source package: `google-mock=1.7.0-18092013-1`

Binary Packages:

- `google-mock:amd64=1.7.0-18092013-1`

Licenses: (parsed from: `/usr/share/doc/google-mock/copyright`)

- `Apache`
- `GPL-3`
- `see "/usr/share/common-licenses/Apache"`

Source:

```console
$ apt-get source -qq --print-uris google-mock=1.7.0-18092013-1
'http://archive.ubuntu.com/ubuntu/pool/universe/g/google-mock/google-mock_1.7.0-18092013-1.dsc' google-mock_1.7.0-18092013-1.dsc 1192 SHA256:f042a8c57ef36c61f335c5e1022971d52a6e721215c5ffa6eaea0f5af269cc88
'http://archive.ubuntu.com/ubuntu/pool/universe/g/google-mock/google-mock_1.7.0-18092013.orig.tar.bz2' google-mock_1.7.0-18092013.orig.tar.bz2 1490983 SHA256:91b1f35431fde037eb833fb19d6af27d23f88055a1ce6c5bad6ddfc6c3308a4e
'http://archive.ubuntu.com/ubuntu/pool/universe/g/google-mock/google-mock_1.7.0-18092013-1.debian.tar.xz' google-mock_1.7.0-18092013-1.debian.tar.xz 5408 SHA256:19c6eb45039de1ec94ffb0e97f46950e864750fa53b8ab44598811fc79a69871
```

### `dpkg` source package: `graphite2=1.3.10-0ubuntu0.16.04.1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.10-0ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`)

- `Artistic`
- `GPL`
- `GPL-1+`
- `GPL1+ | Artistic`
- `LGPL | other`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1 | GPL-2 | LGPL-2.1`
- `other`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.10-0ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.10-0ubuntu0.16.04.1.dsc' graphite2_1.3.10-0ubuntu0.16.04.1.dsc 2238 SHA512:f7e6ae2e48bab6d1a7121056dae176528a00aeed54ac81f105b4923ff6685548376cad4597e6b3ea5eb33aa47960a454bfb77fb6f3263611c6c157f0ff6e2f39
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.10.orig.tar.gz' graphite2_1.3.10.orig.tar.gz 3889647 SHA512:d6d578feaa2d9304dc9bcd3926958070b8c23b27437a9fcb801e08e62f33a5549b7a6aa9636c7f8eb80a2a2c6d5cac97d58050fb30fd102b9fd0f8c558f4252b
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.10-0ubuntu0.16.04.1.debian.tar.xz' graphite2_1.3.10-0ubuntu0.16.04.1.debian.tar.xz 10016 SHA512:a71bb0302388813a3d9a314fcce57fa4d3b4b41920e3c6dc50de610dca10f6c1e2c274170c027921baa051e6bc6afe6b7438582baa2a77ee1f8c37431d862c2b
```

### `dpkg` source package: `grep=2.25-1~16.04.1`

Binary Packages:

- `grep=2.25-1~16.04.1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=2.25-1~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_2.25-1~16.04.1.dsc' grep_2.25-1~16.04.1.dsc 1971 SHA512:86ca38fcab2aba322c91093a29a7dd1f3e8a0fef39236c8fda4a01e8af6c1b817600e4f92cb87ac8f0bb97d35300f8fdce48b10a6b4fba5e4c60aee728da0c70
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_2.25.orig.tar.xz' grep_2.25.orig.tar.xz 1327856 SHA512:7a738f938dde350ae71eb87083586e25768ba392113cba973a4e567b476c788ca66e0736d63f5e0e12a7847fa70379dc0b6568ec92431ea4604acd2cbedd66c1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_2.25-1~16.04.1.debian.tar.bz2' grep_2.25-1~16.04.1.debian.tar.bz2 108236 SHA512:adb04fb20d83908d46da9d8e7e58679103d57a33b69eb2c2352db1c1f71c478408f306f95ed5a1b1da479132019456cdf89eccda68a58dc6f404ab494d80ef83
```

### `dpkg` source package: `gtest=1.7.0-4ubuntu1`

Binary Packages:

- `libgtest-dev:amd64=1.7.0-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgtest-dev/copyright`)

- `BSD-C3`
- `GAP`

Source:

```console
$ apt-get source -qq --print-uris gtest=1.7.0-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gtest/gtest_1.7.0-4ubuntu1.dsc' gtest_1.7.0-4ubuntu1.dsc 1354 SHA256:9f4622d03b42cd79e81e702aa4adfb93323c485f1870bc628591496b80b0c8c7
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gtest/gtest_1.7.0.orig.tar.bz2' gtest_1.7.0.orig.tar.bz2 794603 SHA256:84671fbda864fd0cb2ad7dfba57d0c51821c867f15c2532ac4196ba3cfa56f91
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gtest/gtest_1.7.0-4ubuntu1.debian.tar.xz' gtest_1.7.0-4ubuntu1.debian.tar.xz 7032 SHA256:f357ca4c4ba1855602f97de5298475af20fdd3d31dfeddbbb13ef2b4d720ff38
```

### `dpkg` source package: `gtk+2.0=2.24.30-1ubuntu1.16.04.2`

Binary Packages:

- `libgtk2.0-0:amd64=2.24.30-1ubuntu1.16.04.2`
- `libgtk2.0-common=2.24.30-1ubuntu1.16.04.2`

Licenses: (parsed from: `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

- `LGPL-2`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+2.0=2.24.30-1ubuntu1.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.30-1ubuntu1.16.04.2.dsc' gtk+2.0_2.24.30-1ubuntu1.16.04.2.dsc 3981 SHA512:50a24d012a0d51ddd046820268bcc7c41eaa147ebfd972dcf0696b85facfbe206d0daf88698421d8460b74c1d4a17598dd2be0435237e0722d10e44a0c7c28a8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.30.orig.tar.xz' gtk+2.0_2.24.30.orig.tar.xz 12800276 SHA512:13373e4809b48acefdbf09f18f0f18b562f05b3ce2e3169c5aa80722a262405b3b4a220ecee54c59ef03ef89be9850dc659f6da9251abaf7c577599b7a4319b1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.30-1ubuntu1.16.04.2.debian.tar.xz' gtk+2.0_2.24.30-1ubuntu1.16.04.2.debian.tar.xz 107272 SHA512:3ba0de124c81078669f0a67c331dedd9d4ad43d08ae638f4bbcd31315841e61024e66c5bbc2ba713b8619a698a688e8afdc39bc21da6ca74bd335c4b1ed170e3
```

### `dpkg` source package: `gzip=1.6-4ubuntu1`

Binary Packages:

- `gzip=1.6-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-4ubuntu1.dsc' gzip_1.6-4ubuntu1.dsc 1907 SHA256:77c1d15c52947d50656365597802c586249d26a4f56c8075f5d94b4634d11465
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-4ubuntu1.debian.tar.xz' gzip_1.6-4ubuntu1.debian.tar.xz 14932 SHA256:9a3e558c87a78bf65f9b9c48d718b3ef0bb69e0cf07617f44e37f41ba5f7b006
```

### `dpkg` source package: `harfbuzz=1.0.1-1ubuntu0.1`

Binary Packages:

- `libharfbuzz0b:amd64=1.0.1-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=1.0.1-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.0.1-1ubuntu0.1.dsc' harfbuzz_1.0.1-1ubuntu0.1.dsc 2820 SHA512:6b48ffb72239a8c45812768a5fe4d9abd073b74633033345f382faed284e0ad81d2cda6a0cdb532ac41f6d508a420dbc56487bd0728b09fb4539ee15d63571cc
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.0.1.orig.tar.bz2' harfbuzz_1.0.1.orig.tar.bz2 1211877 SHA512:6de8d38c64772687701789d38001327a20c225e08d77bd4bb919c61613172e9cb57dd6f4dd5cedcaaad6db8228d91546d8a395dcc21033107496d0a37ded0291
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.0.1-1ubuntu0.1.debian.tar.xz' harfbuzz_1.0.1-1ubuntu0.1.debian.tar.xz 8952 SHA512:2fdaf41953d830f7bfc25e15f0f5e2126f54d8e1e9b88176085ab7d366eb8d556c4ac9f68370f1bcf5cb4d8aecababb85f9e13b1683926bd05e1e66405d93c7d
```

### `dpkg` source package: `heimdal=1.7~git20150920+dfsg-4ubuntu1.16.04.1`

Binary Packages:

- `libasn1-8-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libgssapi3-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libhcrypto4-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libheimbase1-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libheimntlm0-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libhx509-5-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libkrb5-26-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libroken18-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libwind0-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris heimdal=1.7~git20150920+dfsg-4ubuntu1.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.dsc' heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.dsc 3766 SHA512:25d7c4546f575b9e94f80b79cc4cbe0f24960289ddc704017986557a9cd4675c2871228d54142a3fb0b2db98b728271b9271fe7df37160754252b988a848b72b
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_1.7~git20150920+dfsg.orig.tar.gz' heimdal_1.7~git20150920+dfsg.orig.tar.gz 8979556 SHA512:a2d76adf60df36c5758f0090425a2ac421d2ae972adbf25c900490310bf283a9283c5055891167487f9f1a0813c3b033b31d28adcce497119e4e437be8a39837
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.debian.tar.xz' heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.debian.tar.xz 65512 SHA512:faa8cb96a99eb3f5f9bf20935eea298adb1d2087a0e6eecf6db6efd13f82705b18f2741342e3fc7dad68428798339eb8dbeecaafb2e0766f9f728656775a7d1f
```

### `dpkg` source package: `hostname=3.16ubuntu2`

Binary Packages:

- `hostname=3.16ubuntu2`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.16ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.16ubuntu2.dsc' hostname_3.16ubuntu2.dsc 1573 SHA256:dcffca698d9f428a83b744d638ef2069252395d9b5d1a3098578f01b0cb347a5
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.16ubuntu2.tar.gz' hostname_3.16ubuntu2.tar.gz 14378 SHA256:e0a38fa03b66abd428e119e5af2cccb78a0462cdb58e2e540e66d964e2719195
```

### `dpkg` source package: `hwloc=1.11.2-3`

Binary Packages:

- `libhwloc-dev:amd64=1.11.2-3`
- `libhwloc5:amd64=1.11.2-3`

Licenses: (parsed from: `/usr/share/doc/libhwloc-dev/copyright`, `/usr/share/doc/libhwloc5/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris hwloc=1.11.2-3
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_1.11.2-3.dsc' hwloc_1.11.2-3.dsc 2542 SHA256:0cfb84c46465ef78d9167826c8d2f17525eda14d8580649e3bcca3b9ec2fecc2
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_1.11.2.orig.tar.bz2' hwloc_1.11.2.orig.tar.bz2 4019136 SHA256:8c029b6b1638245837707bfa6c865f448af4e49e7d352335e019d818b51fecf8
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_1.11.2-3.debian.tar.bz2' hwloc_1.11.2-3.debian.tar.bz2 10090 SHA256:11df92b1a4cb818586c2caa3d5f67e7c7693e5f551cd52e729356666c1ba06e7
```

### `dpkg` source package: `icu=55.1-7ubuntu0.5`

Binary Packages:

- `icu-devtools=55.1-7ubuntu0.5`
- `libicu-dev:amd64=55.1-7ubuntu0.5`
- `libicu55:amd64=55.1-7ubuntu0.5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=55.1-7ubuntu0.5
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1-7ubuntu0.5.dsc' icu_55.1-7ubuntu0.5.dsc 2162 SHA512:1a430be8449c2dab85aa46b3d3469b5d540245c2a7ccd75735a800ad8637cf18625189003494fdc91653eaaf008748863d798d84cd172b543336a012d1ee613e
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1.orig.tar.gz' icu_55.1.orig.tar.gz 25600847 SHA512:21a3eb2c3678cd27b659eed073f8f1bd99c9751291d077820e9a370fd90b7d9b3bf414cc03dec4acb7fa61087e02d04f9f40e91a32c5180c718e2102fbd0cd35
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1-7ubuntu0.5.debian.tar.xz' icu_55.1-7ubuntu0.5.debian.tar.xz 32320 SHA512:dc361dcbc2277e371d446508730ecfdd233469a9019fb01c0e474969815d61bf427f3b14b73fe69a0d764875ee533f6dbabce4cb2551b5d0c9b1f8cdd7487512
```

### `dpkg` source package: `init-system-helpers=1.29ubuntu4`

Binary Packages:

- `init=1.29ubuntu4`
- `init-system-helpers=1.29ubuntu4`

Licenses: (parsed from: `/usr/share/doc/init/copyright`, `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.29ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.29ubuntu4.dsc' init-system-helpers_1.29ubuntu4.dsc 2047 SHA512:cdd02bb1deb55b73ded4d622e73b2f2b7e864d43f6e166d856e403d74d37b0aee3b58807ef18f170cf941991d800eeb179b8a7b47f9ed848cc6eacb1c3f3aea8
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.29ubuntu4.tar.xz' init-system-helpers_1.29ubuntu4.tar.xz 58648 SHA512:7749796e6a77d58ea3439832663ac06b9d11cc2c51ac7dabf8a5ad3c6038a90febcfc64469ec80a4501394bb122d3ba3656c427cdb7395e3794b42094c900008
```

### `dpkg` source package: `insserv=1.14.0-5ubuntu3`

Binary Packages:

- `insserv=1.14.0-5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/insserv/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris insserv=1.14.0-5ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/i/insserv/insserv_1.14.0-5ubuntu3.dsc' insserv_1.14.0-5ubuntu3.dsc 2033 SHA256:30a8e6edc9c105803dfc98d733ba0ed8f0aaf81c4aa4f5ba132241b9a1fcb3a2
'http://archive.ubuntu.com/ubuntu/pool/main/i/insserv/insserv_1.14.0.orig.tar.gz' insserv_1.14.0.orig.tar.gz 53851 SHA256:da74dcf5225a00aa8aef4d5afc6a20e009b2ed9af328dabd55fef1cb3a32140e
'http://archive.ubuntu.com/ubuntu/pool/main/i/insserv/insserv_1.14.0-5ubuntu3.debian.tar.xz' insserv_1.14.0-5ubuntu3.debian.tar.xz 48124 SHA256:a4d0d0703fa398819ab7b4cad573f334feee80aac5520202457519e737b4648a
```

### `dpkg` source package: `isl=0.16.1-1`

Binary Packages:

- `libisl15:amd64=0.16.1-1`

Licenses: (parsed from: `/usr/share/doc/libisl15/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.16.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.16.1-1.dsc' isl_0.16.1-1.dsc 1857 SHA256:d6428f2a18db18cdfbff3be72b33dbc4b1838d5efea97ae5715c24115250be91
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.16.1.orig.tar.gz' isl_0.16.1.orig.tar.gz 1889136 SHA256:fb34703bd694622aef92164bad983c15ec04274edbe19e614d9ecda54b85603d
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.16.1-1.debian.tar.xz' isl_0.16.1-1.debian.tar.xz 21152 SHA256:d1ee2fd3a5b7289ba7f66fe443f57f5b6f4297a3a9164d840fafc9c37d3ec632
```

### `dpkg` source package: `jbigkit=2.1-3.1`

Binary Packages:

- `libjbig0:amd64=2.1-3.1`

Licenses: (parsed from: `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1.dsc' jbigkit_2.1-3.1.dsc 1299 SHA256:62c8812d508958c5d35f2b1579dc3052fb5bd8d2e77d023fad064c4b48c8c3f8
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1.debian.tar.xz' jbigkit_2.1-3.1.debian.tar.xz 7600 SHA256:ebc3c52deaf37d52baea54d648a713640dc262926abda7bf05cd08e7db5dd1ee
```

### `dpkg` source package: `keyutils=1.5.9-8ubuntu1`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-8ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-8ubuntu1.dsc' keyutils_1.5.9-8ubuntu1.dsc 1548 SHA256:dd06e9b6a773ed745cd74dbce13d585469aa508f2afbc6fa51a58939b295ce07
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-8ubuntu1.debian.tar.xz' keyutils_1.5.9-8ubuntu1.debian.tar.xz 16716 SHA256:36f69846dfeb1e7abdd39dace57a43f9637e426cf4c5252dd9990af36488249b
```

### `dpkg` source package: `kmod=22-1ubuntu5.2`

Binary Packages:

- `libkmod2:amd64=22-1ubuntu5.2`

Licenses: (parsed from: `/usr/share/doc/libkmod2/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris kmod=22-1ubuntu5.2
'http://archive.ubuntu.com/ubuntu/pool/main/k/kmod/kmod_22-1ubuntu5.2.dsc' kmod_22-1ubuntu5.2.dsc 2165 SHA512:b8558b3e1968d95e0d2a084ecfc32d3d7b5988d75a794d5f528d63951bd6194f2bf8386c3d22664ad4422099315d79f1958d612a696a31b65f1f8da2b26252a4
'http://archive.ubuntu.com/ubuntu/pool/main/k/kmod/kmod_22.orig.tar.xz' kmod_22.orig.tar.xz 160576 SHA512:f34bcc05325b27c739d898e3c42ff02c3ac754fccab823f1e2d11ef9f9112871f4ace1d65a1c6e02af5097aa91b0fc794c7e916cdb6de169a527309db813ec42
'http://archive.ubuntu.com/ubuntu/pool/main/k/kmod/kmod_22-1ubuntu5.2.debian.tar.xz' kmod_22-1ubuntu5.2.debian.tar.xz 14524 SHA512:184d70264a6cf50b8df6e8bf19950c295c8c404633c2a782f75188e1c9fec639e6c673f594995f398e85c82613ffb4565131b62b7b8062dbae3de079c8778565
```

### `dpkg` source package: `krb5=1.13.2+dfsg-5ubuntu2.1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libk5crypto3:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkrb5-3:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkrb5support0:amd64=1.13.2+dfsg-5ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.13.2+dfsg-5ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg-5ubuntu2.1.dsc' krb5_1.13.2+dfsg-5ubuntu2.1.dsc 3520 SHA512:1f00e7694e015d400d73503a54503aeb3fd32deb5927110fc1f805abb5d90a6112fff2829aec4fff7afcd7ec66559cb2b5153fd86cb9548deb6d246131a51b34
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg.orig.tar.gz' krb5_1.13.2+dfsg.orig.tar.gz 11884064 SHA512:d9562deaee7144c786c279e6e3415fe248fa1a71db8868ff05d1d7ef651274146d9e2c96f37c045fefd43364662ec41714bdd2d59a5ff16634ad7a510d4b3eab
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg-5ubuntu2.1.debian.tar.xz' krb5_1.13.2+dfsg-5ubuntu2.1.debian.tar.xz 113600 SHA512:2cc82e691667bb37f52e70b9fd9e1529ea07e981945becbbd7ecf2907e0d2dd23755779c114269c4cdbdf0b168766888582d8274b48f82126f7d87d4ce31bdcc
```

### `dpkg` source package: `lapack=3.6.0-2ubuntu2`

Binary Packages:

- `libblas-common=3.6.0-2ubuntu2`
- `libblas3=3.6.0-2ubuntu2`
- `liblapack3=3.6.0-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libblas-common/copyright`, `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.6.0-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.6.0-2ubuntu2.dsc' lapack_3.6.0-2ubuntu2.dsc 2873 SHA256:a2ef88a09b242d0527748a8bff88ed432dab1dc5b200e918c4ac7ca30af691a2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.6.0.orig.tar.gz' lapack_3.6.0.orig.tar.gz 6792324 SHA256:a9a0082c918fe14e377bbd570057616768dca76cbdc713457d8199aaa233ffc3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.6.0-2ubuntu2.debian.tar.xz' lapack_3.6.0-2ubuntu2.debian.tar.xz 24556 SHA256:a713e29f24fca14d59937595a54f03cf0479416188c5911d5220f61299f31c47
```

### `dpkg` source package: `libarchive=3.1.2-11ubuntu0.16.04.8`

Binary Packages:

- `libarchive13:amd64=3.1.2-11ubuntu0.16.04.8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libarchive=3.1.2-11ubuntu0.16.04.8
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.1.2-11ubuntu0.16.04.8.dsc' libarchive_3.1.2-11ubuntu0.16.04.8.dsc 2422 SHA512:637cc4fb7325fd64edd0283b7808f9acd2244d79d9eda016d01d6a49d4e7d658a0ca0ce44c3c1b294c80a7c0deba242708ef6a03dfe7039d03f2754b19fe6e4b
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.1.2.orig.tar.gz' libarchive_3.1.2.orig.tar.gz 4527540 SHA512:1f3c2a675031f93c7d42ae2ed06742b0b1e2236ff57d9117791d62fb8ae77d6cafffbcb5d45b5bd98daa908bd18c576cf82e01a9b1eba699705e23eff3688114
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.1.2-11ubuntu0.16.04.8.debian.tar.xz' libarchive_3.1.2-11ubuntu0.16.04.8.debian.tar.xz 46116 SHA512:a4ffa14241d3d9279a4e45ab6518332004940e1e2d7d5af5e2aef5a7507711f1ebb25e1b8cc40bc219e68efbf51e5da0f717dd2861101b0636886e0557226501
```

### `dpkg` source package: `libassuan=2.4.2-2`

Binary Packages:

- `libassuan0:amd64=2.4.2-2`

Licenses: (parsed from: `/usr/share/doc/libassuan0/copyright`)

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
$ apt-get source -qq --print-uris libassuan=2.4.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.4.2-2.dsc' libassuan_2.4.2-2.dsc 2104 SHA256:5a741a94b2faf19626691bf5b9121e7fd2e82335c3e34c5d84644488228bb713
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.4.2.orig.tar.bz2' libassuan_2.4.2.orig.tar.bz2 587631 SHA256:bb06dc81380b74bf1b64d5849be5c0409a336f3b4c45f20ac688e86d1b5bcb20
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.4.2-2.debian.tar.xz' libassuan_2.4.2-2.debian.tar.xz 12168 SHA256:39b6f31517857bde39ff86f1b4b5d122a676d91477dc79caafb720e4e36cd3d1
```

### `dpkg` source package: `libbsd=0.8.2-1ubuntu0.1`

Binary Packages:

- `libbsd0:amd64=0.8.2-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-Peter-Wemm`
- `BSD-3-clause-Regents`
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
$ apt-get source -qq --print-uris libbsd=0.8.2-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2-1ubuntu0.1.dsc' libbsd_0.8.2-1ubuntu0.1.dsc 2083 SHA512:7d5f09928b1d742ea60f9155829d3488fbd95e06be963f4dac415826142dd1677395da81412edd2f75149239ee534bee741d887c215b6419a1d8fe594fddf6b9
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2.orig.tar.xz' libbsd_0.8.2.orig.tar.xz 344292 SHA512:2230d51a30a0c3a8518c7e325036d2b578c8c2b47525c2d0d5f530d28d82227ad48b50341e44521db21f99208fe7c0df7313254c90e3c92da1c8664a8cbb87c5
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2-1ubuntu0.1.debian.tar.xz' libbsd_0.8.2-1ubuntu0.1.debian.tar.xz 15652 SHA512:009907249c54bc1158e88c3220ce99a52a99d660d76e4774e85c52e25602943e04094de3acc24fed6ae7f4e95125980608796dd90c4b5af1dbfb47611b37ae59
```

### `dpkg` source package: `libcap2=1:2.24-12`

Binary Packages:

- `libcap2:amd64=1:2.24-12`
- `libcap2-bin=1:2.24-12`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.24-12
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.24-12.dsc' libcap2_2.24-12.dsc 2211 SHA256:4db68746bd1fe7df6d29ae15c3605e4e1d0e44723580c05166144735c773ae14
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.24.orig.tar.xz' libcap2_2.24.orig.tar.xz 63264 SHA256:51cd1c568a2baf1e687573bd6117a94b07f33b46a05acaa50ee208792a830b79
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.24-12.debian.tar.xz' libcap2_2.24-12.debian.tar.xz 18704 SHA256:34be2e791ec96095cc0b405e532874e8c79aeb2125981ebc6896a0ad0b999cf2
```

### `dpkg` source package: `libdatrie=0.2.10-2`

Binary Packages:

- `libdatrie1:amd64=0.2.10-2`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.10-2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-2.dsc' libdatrie_0.2.10-2.dsc 2216 SHA256:28028afb148bbe42e31a32c9c28ebc19bd0448694fe136e9180bd162345f95c2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10.orig.tar.xz' libdatrie_0.2.10.orig.tar.xz 294380 SHA256:180eff7b0309ca19a02d5864e744185d715f021398a096fec6cf960f8ebfaa2b
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-2.debian.tar.xz' libdatrie_0.2.10-2.debian.tar.xz 7132 SHA256:9f4b854767fa683853c74f5fb7b477694b9d7b3279315dd56fd6c51aa9a43ff0
```

### `dpkg` source package: `libdrm=2.4.91-2~16.04.1`

Binary Packages:

- `libdrm-amdgpu1:amd64=2.4.91-2~16.04.1`
- `libdrm-common=2.4.91-2~16.04.1`
- `libdrm-intel1:amd64=2.4.91-2~16.04.1`
- `libdrm-nouveau2:amd64=2.4.91-2~16.04.1`
- `libdrm-radeon1:amd64=2.4.91-2~16.04.1`
- `libdrm2:amd64=2.4.91-2~16.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libdrm=2.4.91-2~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91-2~16.04.1.dsc' libdrm_2.4.91-2~16.04.1.dsc 3293 SHA512:d7867e2aeb3d5169c6ed0be056e67ea660ecd3aee90484430b550fe8618c81c69e141d0a9971a14e25998edfe62c34f19d9114161bbc09950be92af195d3d704
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91.orig.tar.gz' libdrm_2.4.91.orig.tar.gz 1088866 SHA512:276cb0e0a6542a00ce5b9addc64b322bd25ceabdae2d86dda733bfe5d346bfbfc2a113d630c1a12761d31c7d4bda850bf3c26ed4b141f14e37fc8afbde6dbfc9
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91.orig.tar.gz.asc' libdrm_2.4.91.orig.tar.gz.asc 879 SHA512:364b36b26e7f7a0f5d41d6ea6c069c66df5391e100b2c6cd5c412ea0d6d356a89d01acc1fa6ee431446e179144742bf5781a8de4210eec7f5ba24ee3eb70d5a4
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91-2~16.04.1.diff.gz' libdrm_2.4.91-2~16.04.1.diff.gz 49908 SHA512:83ca15352cd6af889393d6e2432898c184a0553474420490e0011c6c1bda5ea05e18251590deeb27c2c7ce41b5e36ee1577dee4bfd3b0222b1d568327af5d1c8
```

### `dpkg` source package: `libedit=3.1-20150325-1ubuntu2`

Binary Packages:

- `libedit2:amd64=3.1-20150325-1ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20150325-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20150325-1ubuntu2.dsc' libedit_3.1-20150325-1ubuntu2.dsc 2342 SHA256:58a27a139b3b1e216a9b9d95fc8f0a0e0bccb244b016b382e6957d0e5a8cdb04
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20150325.orig.tar.gz' libedit_3.1-20150325.orig.tar.gz 502792 SHA256:c88a5e4af83c5f40dda8455886ac98923a9c33125699742603a88a0253fcc8c5
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20150325-1ubuntu2.debian.tar.bz2' libedit_3.1-20150325-1ubuntu2.debian.tar.bz2 10946 SHA256:97d03ee621a5ec98b2683052b57c151462ec690a8e94e7d52bae76c79975f8b3
```

### `dpkg` source package: `liberror-perl=0.17-1.2`

Binary Packages:

- `liberror-perl=0.17-1.2`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17-1.2.dsc' liberror-perl_0.17-1.2.dsc 1825 SHA256:d024e770bb970061e338798934a1862b5dd51ca99f04f6cdab1c5a58b30b4eba
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17.orig.tar.gz' liberror-perl_0.17.orig.tar.gz 17266 SHA256:2e8157981a77e87d37d26d8b6b3183560dddc541b491b0b32fcda010730b257c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17-1.2.diff.gz' liberror-perl_0.17-1.2.diff.gz 3645 SHA256:26664db91daa76fdf78be37196df02067b2283deae1b4ac766923d7ef08c3fb8
```

### `dpkg` source package: `libffi=3.2.1-4`

Binary Packages:

- `libffi6:amd64=3.2.1-4`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-4.dsc' libffi_3.2.1-4.dsc 1914 SHA256:e2bdb4202f1c8be9d3cec5bf459a4a1619f494241938d982d6029e15a8b1da9e
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-4.debian.tar.xz' libffi_3.2.1-4.debian.tar.xz 8932 SHA256:4d7d5f9172e8a8d3e412ed47e14755e27a0657054a7786b578eb6327b0d08b2d
```

### `dpkg` source package: `libgcrypt20=1.6.5-2ubuntu0.6`

Binary Packages:

- `libgcrypt20:amd64=1.6.5-2ubuntu0.6`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.6.5-2ubuntu0.6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.6.5-2ubuntu0.6.dsc' libgcrypt20_1.6.5-2ubuntu0.6.dsc 2653 SHA512:6ae3ce26176c486771c3e0c2f675595e49603934bec483b1333e0f8c22dc3c5b0ef013c53e0afc434c2afaa6a45365901aff7fcd247fe3a2475f6755caa74be0
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.6.5.orig.tar.bz2' libgcrypt20_1.6.5.orig.tar.bz2 2549601 SHA512:1b76640a68514369da3b6be51d66e7040b64d03eba68d6b0d1b1ba88336c9da3ef41b21170a9eb641dae5a36a7c53cb167e15c8da964a5a6793aec947afe91f4
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.6.5-2ubuntu0.6.debian.tar.xz' libgcrypt20_1.6.5-2ubuntu0.6.debian.tar.xz 38412 SHA512:de1031f5e21d8f61f4e6a8a1de7bdafeebfebfcc8951dda10d149341d4e69876cd5568d074c2ecda22d40d4a97a521f9718fe1af6f4948eb4a866daac599f21d
```

### `dpkg` source package: `libgpg-error=1.21-2ubuntu1`

Binary Packages:

- `libgpg-error0:amd64=1.21-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `GPL-2.1+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.21-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.21-2ubuntu1.dsc' libgpg-error_1.21-2ubuntu1.dsc 2306 SHA256:591fc35e29c7314e9dcbea0ed929afc563dd5e0a6be18d65d2480762353bd71f
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.21.orig.tar.bz2' libgpg-error_1.21.orig.tar.bz2 763186 SHA256:b7dbdb3cad63a740e9f0c632a1da32d4afdb694ec86c8625c98ea0691713b84d
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.21-2ubuntu1.debian.tar.xz' libgpg-error_1.21-2ubuntu1.debian.tar.xz 11988 SHA256:b67f4686d39ec678e860b28d05e07567ec6d43025c18b82c1e9a5dda07a00ed9
```

### `dpkg` source package: `libibverbs=1.1.8-1.1ubuntu2`

Binary Packages:

- `libibverbs-dev=1.1.8-1.1ubuntu2`
- `libibverbs1=1.1.8-1.1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libibverbs-dev/copyright`, `/usr/share/doc/libibverbs1/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libibverbs=1.1.8-1.1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libibverbs/libibverbs_1.1.8-1.1ubuntu2.dsc' libibverbs_1.1.8-1.1ubuntu2.dsc 1666 SHA256:85d0a6840eaf23064a577e4bbe031d8c79fc2d2fd19996f891639a87067d9437
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libibverbs/libibverbs_1.1.8.orig.tar.gz' libibverbs_1.1.8.orig.tar.gz 406548 SHA256:7c766e679e1e6dbcb37bdfc624c64310787e3a380baf7ee1eebde39c6991828f
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libibverbs/libibverbs_1.1.8-1.1ubuntu2.debian.tar.xz' libibverbs_1.1.8-1.1ubuntu2.debian.tar.xz 6952 SHA256:9149a3a6353b55aa3704e259c60f2dd3fdb3fad74e9e6cb01cbdf030cdcd7f47
```

### `dpkg` source package: `libice=2:1.0.9-1`

Binary Packages:

- `libice6:amd64=2:1.0.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-1.dsc' libice_1.0.9-1.dsc 2140 SHA256:f90a79944f147b5db208677d92381fd0886c201616172bac0b28ef0e85912ebd
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-1.diff.gz' libice_1.0.9-1.diff.gz 6260 SHA256:85d68a69d5e6b25b352eb98c6c33fa7a324da8dd913d7e84a049852fb87287e7
```

### `dpkg` source package: `libidn=1.32-3ubuntu1.2`

Binary Packages:

- `libidn11:amd64=1.32-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libidn11/copyright`)

- `GAP`
- `GFDL-1.3`
- `GFDL-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libidn=1.32-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.32-3ubuntu1.2.dsc' libidn_1.32-3ubuntu1.2.dsc 2303 SHA512:1c2cfc31a222bcdc47d5693bcb8cf3eb3338ca4faa27bf52bf096f225a2e7388124303238c6dca783f81494435687cd7af42f2dd2748e0a30d6ce6aabdd6d701
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.32.orig.tar.gz' libidn_1.32.orig.tar.gz 3483155 SHA512:fd48665b65f88210ea504675fc1cd667bd4042b1df3e386847070a465d6753efcec735e6e8572f45f9432235e813c61ef7df09596274935467fdc6f12f80b9bd
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.32-3ubuntu1.2.debian.tar.xz' libidn_1.32-3ubuntu1.2.debian.tar.xz 84724 SHA512:01614e1555d443f94e5380fd76827737e89774c6361ef72e551fec7ec0c82e99b514ec45d8f8b4f02dfa7b7573ea355476b0590ece35235b1ac4a5a03971cd04
```

### `dpkg` source package: `libjpeg-turbo=1.4.2-0ubuntu3.4`

Binary Packages:

- `libjpeg-turbo8:amd64=1.4.2-0ubuntu3.4`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1.4.2-0ubuntu3.4
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2-0ubuntu3.4.dsc' libjpeg-turbo_1.4.2-0ubuntu3.4.dsc 2302 SHA512:b38aea3ad6f874764d9a270f554c8ddf921bf303709dee30f1c7fb34666f313865c7841d8ad59997af3db0b7b18da4e67b3f3372d9a0d75f70a4db94d79a0d24
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2.orig.tar.gz' libjpeg-turbo_1.4.2.orig.tar.gz 1569306 SHA512:9bd27c917c29125c425469eb0fdf99b802f25095f187fb416bd7c05e4af95a32404bbb0d06b77343d35d3461029500decf3481337b2eade9e57b58dea69719ee
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2-0ubuntu3.4.debian.tar.xz' libjpeg-turbo_1.4.2-0ubuntu3.4.debian.tar.xz 30156 SHA512:621e4d1b6326524c5c73811c7bb66df7f50037c8e71a52dec1e45c657864b4b88b6c899ea05abf42373ac1d591983f873d07cc976576bc818a3643757515d529
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu8`

Binary Packages:

- `libjpeg8:amd64=8c-2ubuntu8`

Licenses: (parsed from: `/usr/share/doc/libjpeg8/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg8-empty=8c-2ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.dsc' libjpeg8-empty_8c-2ubuntu8.dsc 1637 SHA256:e7f575dcb3e0d462513b6f928179baa0ff1d145273934b1041b714515096b407
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.tar.gz' libjpeg8-empty_8c-2ubuntu8.tar.gz 1770 SHA256:48a4227e9fc70851a4f304b10624e02875bf6f4e2debfcbe4ba0dd85a3ec05c6
```

### `dpkg` source package: `libjsoncpp=1.7.2-1`

Binary Packages:

- `libjsoncpp1:amd64=1.7.2-1`

Licenses: (parsed from: `/usr/share/doc/libjsoncpp1/copyright`)

- `Expat_or_PublicDomain_or_DualExpatPD`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libjsoncpp=1.7.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.2-1.dsc' libjsoncpp_1.7.2-1.dsc 2078 SHA256:1a639f002cb4405c80b6ab9d0db8739b692ff83a5c7221aca325ba1dfc90b760
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.2.orig.tar.gz' libjsoncpp_1.7.2.orig.tar.gz 205391 SHA256:2179a7df19c1c6dc87e02c65b847efc914625a9b87df3e443d9610fc70c0f557
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.2-1.debian.tar.xz' libjsoncpp_1.7.2-1.debian.tar.xz 7312 SHA256:fc2ce2284d00dffb1f18f894052aa51162b8d009f9d150d2d80dfda8285d8a37
```

### `dpkg` source package: `libksba=1.3.3-1ubuntu0.16.04.1`

Binary Packages:

- `libksba8:amd64=1.3.3-1ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.3.3-1ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.3-1ubuntu0.16.04.1.dsc' libksba_1.3.3-1ubuntu0.16.04.1.dsc 2266 SHA512:a4ee24793de88e4f8b8ed63a40b55f723bf424f7950d436adb3a4deb19a6880b7ff3786a0f2e0d0effdaae3ec35e1b6bcf69ec2f01b2e2f647fa9c2da307ebd0
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.3.orig.tar.bz2' libksba_1.3.3.orig.tar.bz2 618698 SHA512:57de827a67a88dddf9227a5409bb86220e773f18b53d3d06c45699677e3052f94abe78bcd1895c3bd7594c5e728b4c8232dd3bd3b1cd22cf47f8110e2aec9db7
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.3-1ubuntu0.16.04.1.debian.tar.xz' libksba_1.3.3-1ubuntu0.16.04.1.debian.tar.xz 13460 SHA512:a995819e9616e5e9894c0bb17911796f20cf5b0f7df734d5ca3f7a93c8673e00d1a539c642d7c5231a5f6ef6faba76cf8d95cc6a44201ea5b49a047f94d1bcf1
```

### `dpkg` source package: `libnotify=0.7.6-2svn1`

Binary Packages:

- `libnotify4:amd64=0.7.6-2svn1`

Licenses: (parsed from: `/usr/share/doc/libnotify4/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libnotify=0.7.6-2svn1
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnotify/libnotify_0.7.6-2svn1.dsc' libnotify_0.7.6-2svn1.dsc 2551 SHA256:d818b3256586cd471ed9223185a0425166a36f272828928b032a658f1cf03951
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnotify/libnotify_0.7.6.orig.tar.xz' libnotify_0.7.6.orig.tar.xz 280388 SHA256:0ef61ca400d30e28217979bfa0e73a7406b19c32dd76150654ec5b2bdf47d837
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnotify/libnotify_0.7.6-2svn1.debian.tar.xz' libnotify_0.7.6-2svn1.debian.tar.xz 8092 SHA256:dc21881c3eec70f4e423d28a24c32bc1b01e16132f1472fd48ebddc55ed3c510
```

### `dpkg` source package: `libpciaccess=0.13.4-1`

Binary Packages:

- `libpciaccess0:amd64=0.13.4-1`

Licenses: (parsed from: `/usr/share/doc/libpciaccess0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpciaccess=0.13.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.13.4-1.dsc' libpciaccess_0.13.4-1.dsc 2060 SHA256:c7413e1b3804ae83667d0144eabb5bcba046a16c12f20f94d861edb71a9f67e8
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.13.4.orig.tar.gz' libpciaccess_0.13.4.orig.tar.gz 440390 SHA256:74d92bda448e6fdb64fee4e0091255f48d625d07146a121653022ed3a0ca1f2f
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.13.4-1.diff.gz' libpciaccess_0.13.4-1.diff.gz 24145 SHA256:72e06952d417e15ee23766815f8f10555c2504189f9420a3b6df0be25e972650
```

### `dpkg` source package: `libpng=1.2.54-1ubuntu1.1`

Binary Packages:

- `libpng12-0:amd64=1.2.54-1ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libpng12-0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libpng=1.2.54-1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng/libpng_1.2.54-1ubuntu1.1.dsc' libpng_1.2.54-1ubuntu1.1.dsc 2121 SHA512:bbfd410f3c521b11620196f80a6102fa05434a76c16733f4222d48371e5f96e29ebaf26708528352aff7a599fe79dff5cefe3a0b1aff0aff57a7f9a5524a1d90
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng/libpng_1.2.54.orig.tar.xz' libpng_1.2.54.orig.tar.xz 571448 SHA512:3fde161bae1c61c0c099344518a59a312ac5bcd6063d7d01be156fd4e048fdaafed8a27e10bf2750d4ef678389e2782137c9e6540b7fd0859b820bb8d9443497
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng/libpng_1.2.54-1ubuntu1.1.debian.tar.xz' libpng_1.2.54-1ubuntu1.1.debian.tar.xz 18820 SHA512:42b4f5f16310adf2e41f12656f7deb6900f85346a5a106d495d5b3f545e0841d4d8b22845df41e04d5b3ceb939d745e5b1c5efdca004f38305ad58608c271a2a
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3.16.04.3`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3.16.04.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu3.16.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.16.04.3.dsc' libseccomp_2.4.3-1ubuntu3.16.04.3.dsc 1951 SHA512:41c8a65ea259c373628221db6834524d25dc780de408d880a508fb2d5d8e35dbb280863168f2c045f2bbedef6fd692e0f39888bdbed6569c5696ea43dcf125d1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA512:7b7af2e98493243ffe1934fefff5723b24ae9b9bdc4bf039343ee8456c15acb0ea34e81ec292a41143848272aeca794ef92ad38fc3f42c77465170cb540479ef
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.16.04.3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.16.04.3.debian.tar.xz 27452 SHA512:ffb534c30fced0f5651f4ac41f3a7d00e468dcff833445b0e2207dcfaa25bc31a77b5d481a9d4a38fbb37cf9e96f62ebccb2bb4b0660c69e1f15dc90ac094678
```

### `dpkg` source package: `libselinux=2.4-3build2`

Binary Packages:

- `libselinux1:amd64=2.4-3build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.4-3build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.4-3build2.dsc' libselinux_2.4-3build2.dsc 2491 SHA256:c14dbd5eff5dfd66c41b9ed3d09e1186975b233c8a2a59720ccb8b318c85883c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.4.orig.tar.gz' libselinux_2.4.orig.tar.gz 165931 SHA256:46043091f4c5ba4f43e8d3715f30d665a2d571c9126c1f03945c9ea4ed380f7b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.4-3build2.debian.tar.xz' libselinux_2.4-3build2.debian.tar.xz 23216 SHA256:96f1c0526970460e6b5f64ea4d2f7ecabe06e80e23e83e4feccecb955e1ca956
```

### `dpkg` source package: `libsemanage=2.3-1build3`

Binary Packages:

- `libsemanage-common=2.3-1build3`
- `libsemanage1:amd64=2.3-1build3`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.3-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.3-1build3.dsc' libsemanage_2.3-1build3.dsc 2497 SHA256:920f1f389316617711778cbe83eb36f62d59a2ebb3b1488f75c41014c0bc684c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.3.orig.tar.gz' libsemanage_2.3.orig.tar.gz 138231 SHA256:03e09e35e611c286e446bef92b6023ef2623815996f5a53394bb02e49a312e4b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.3-1build3.debian.tar.xz' libsemanage_2.3-1build3.debian.tar.xz 15056 SHA256:d4f90c66ba911f72c5195da957cdcacd91a583e64ad06c01bf5b692387ee3d33
```

### `dpkg` source package: `libsepol=2.4-2`

Binary Packages:

- `libsepol1:amd64=2.4-2`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.4-2.dsc' libsepol_2.4-2.dsc 1768 SHA256:fca86fc62f736baf96ac2061327553b74b1b34f7ace89d982baa5374c24e2841
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.4.orig.tar.gz' libsepol_2.4.orig.tar.gz 570822 SHA256:299015d59932404c6b69d365fdecffe5c0e2f9c44e08b47286a4bfc02ee49659
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.4-2.debian.tar.xz' libsepol_2.4-2.debian.tar.xz 13188 SHA256:85e50e42c49dee9b21b5dda5fb754ce6d10482a4641e9f088da103b9178c2c1d
```

### `dpkg` source package: `libsm=2:1.2.2-1`

Binary Packages:

- `libsm6:amd64=2:1.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2-1.dsc' libsm_1.2.2-1.dsc 2107 SHA256:1347efa550751179c0a3f1042a9f8ae43ee0c22cf0c2283921fa83e52a68433f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2.orig.tar.gz' libsm_1.2.2.orig.tar.gz 415990 SHA256:14bb7c669ce2b8ff712fbdbf48120e3742a77edcd5e025d6b3325ed30cf120f4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2-1.diff.gz' libsm_1.2.2-1.diff.gz 6183 SHA256:9848714292ead15fcc48ab2d337f2cc5fc08910abbdfaf69d3ef1b89d3fdb2d5
```

### `dpkg` source package: `libtasn1-6=4.7-3ubuntu0.16.04.3`

Binary Packages:

- `libtasn1-6:amd64=4.7-3ubuntu0.16.04.3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.7-3ubuntu0.16.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.7-3ubuntu0.16.04.3.dsc' libtasn1-6_4.7-3ubuntu0.16.04.3.dsc 2495 SHA512:0309d18c3829079a188b37a6fbcf613d3e0b3143a44b845a5be4a619105197536c68b0d4febcc8a46fdc5718244df847601ec19e0689f987b9986f0ff1ad6f02
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.7.orig.tar.gz' libtasn1-6_4.7.orig.tar.gz 1851611 SHA512:9e93264bfad250d88c528550db4731d07c5c1b2ec319b892e9b536dc3d46b2a4166241ebf3470127c4f662067b7dabaa407ce1f16bdf05ee31495881eefe5572
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.7-3ubuntu0.16.04.3.debian.tar.xz' libtasn1-6_4.7-3ubuntu0.16.04.3.debian.tar.xz 60468 SHA512:9059324cc9e9048a014c86ebc923f068ed837929bd48dff7a670a0e5a45e492f5d8b53510e3a5b07844d3d24276eeb9810c710a4b46c83721726d8194f6fe3a1
```

### `dpkg` source package: `libthai=0.1.24-2`

Binary Packages:

- `libthai-data=0.1.24-2`
- `libthai0:amd64=0.1.24-2`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.24-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.24-2.dsc' libthai_0.1.24-2.dsc 2341 SHA256:4e760ef914d56d7a83fbbbf2ff25446e7669335e5404d2accf89445b81874c9c
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.24.orig.tar.xz' libthai_0.1.24.orig.tar.xz 394672 SHA256:a2dd95f79084a27ac077cc206e66e30ee193b70738676ed39792acc9a1c2af0d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.24-2.debian.tar.xz' libthai_0.1.24-2.debian.tar.xz 10780 SHA256:94ff719ca7679150ceab23ee45c3eeeb7c13196fbc206310e150bd32574eeebd
```

### `dpkg` source package: `libtool=2.4.6-0.1`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-0.1`
- `libltdl7:amd64=2.4.6-0.1`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-0.1.dsc' libtool_2.4.6-0.1.dsc 2080 SHA256:c0ec24bc1e892564840061e64cf288e018484d733208d97815f3b12f043088b6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-0.1.debian.tar.xz' libtool_2.4.6-0.1.debian.tar.xz 19332 SHA256:1b9d3e0f9d177d259206cdda69d6cec8dd04df14cbb064b71869936ca5f2722f
```

### `dpkg` source package: `libusb=2:0.1.12-28`

Binary Packages:

- `libusb-0.1-4:amd64=2:0.1.12-28`

Licenses: (parsed from: `/usr/share/doc/libusb-0.1-4/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libusb=2:0.1.12-28
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb/libusb_0.1.12-28.dsc' libusb_0.1.12-28.dsc 2012 SHA256:be0a89935a8764dc64d40a28959397e6582261eef2152c4ce90a13490471dc5f
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb/libusb_0.1.12.orig.tar.gz' libusb_0.1.12.orig.tar.gz 389343 SHA256:37f6f7d9de74196eb5fc0bbe0aea9b5c939de7f500acba3af6fd643f3b538b44
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb/libusb_0.1.12-28.debian.tar.xz' libusb_0.1.12-28.debian.tar.xz 21524 SHA256:eaf2314902b0bb9de3e1fa8c9abfcecea7b78c9824048016beaca34f7cc4351b
```

### `dpkg` source package: `libx11=2:1.6.3-1ubuntu2.2`

Binary Packages:

- `libx11-6:amd64=2:1.6.3-1ubuntu2.2`
- `libx11-data=2:1.6.3-1ubuntu2.2`
- `libx11-xcb1:amd64=2:1.6.3-1ubuntu2.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.3-1ubuntu2.2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.3-1ubuntu2.2.dsc' libx11_1.6.3-1ubuntu2.2.dsc 2619 SHA512:2c99d0db111ee13c5de8cab3955108c6602749f761f122dc3e629792dfc861636b114df4cbbd9f1158ebcbebfcd2bcc16579b41c5a9fc6a7df46642c2d4d77b7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.3.orig.tar.gz' libx11_1.6.3.orig.tar.gz 3105928 SHA512:ee3bc82bb2d818dd25cffe1581260c301c24f25264da0a102ecbe897bcd6b2f203532caf8267d776725a6416ae04fc88f23ceecc0174198a66e49fb8447d3016
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.3-1ubuntu2.2.diff.gz' libx11_1.6.3-1ubuntu2.2.diff.gz 49296 SHA512:544f21bbbde2a329c4f75d0cc4c805ca4c3af5fbacb8a2abfac08ebfe98f795af0393e0f43494acf8ecc69b9b961e174ddca1285b8467dd2cec5d79a8fd40c07
```

### `dpkg` source package: `libxau=1:1.0.8-1`

Binary Packages:

- `libxau6:amd64=1:1.0.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1.dsc' libxau_1.0.8-1.dsc 2040 SHA256:3ddb5f2c7a49ef7507b8d1e63e891238db877b4d1bb1c5486a3e3242c8523602
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA256:c343b4ef66d66a6b3e0e27aa46b37ad5cab0f11a5c565eafb4a1c7590bc71d7b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1.diff.gz' libxau_1.0.8-1.diff.gz 15287 SHA256:b493479d6a52a0e753dd357ad8a4bc5c4296015f3f7b96cf546f7c5c5843cbb0
```

### `dpkg` source package: `libxcb=1.11.1-1ubuntu1`

Binary Packages:

- `libxcb-dri2-0:amd64=1.11.1-1ubuntu1`
- `libxcb-dri3-0:amd64=1.11.1-1ubuntu1`
- `libxcb-glx0:amd64=1.11.1-1ubuntu1`
- `libxcb-present0:amd64=1.11.1-1ubuntu1`
- `libxcb-render0:amd64=1.11.1-1ubuntu1`
- `libxcb-shm0:amd64=1.11.1-1ubuntu1`
- `libxcb-sync1:amd64=1.11.1-1ubuntu1`
- `libxcb1:amd64=1.11.1-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.11.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.11.1-1ubuntu1.dsc' libxcb_1.11.1-1ubuntu1.dsc 6434 SHA256:d059cea4a732eb2600d829d023af89956b46d85399d90be122a887a6baf59a26
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.11.1.orig.tar.gz' libxcb_1.11.1.orig.tar.gz 633057 SHA256:660312d5e64d0a5800262488042c1707a0261fa01a759bad265b1b75dd4844dd
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.11.1-1ubuntu1.diff.gz' libxcb_1.11.1-1ubuntu1.diff.gz 25030 SHA256:017d57e8d555e9f003b1d1ef394b81eddecf9029b6b7e582400dd51e17d63401
```

### `dpkg` source package: `libxcomposite=1:0.4.4-1`

Binary Packages:

- `libxcomposite1:amd64=1:0.4.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcomposite=1:0.4.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.dsc' libxcomposite_0.4.4-1.dsc 2170 SHA256:b304040285ca2d6e2667bfec45097814bdd017380c629a5972993407c656469a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4.orig.tar.gz' libxcomposite_0.4.4.orig.tar.gz 354584 SHA256:83c04649819c6f52cda1b0ce8bcdcc48ad8618428ad803fb07f20b802f1bdad1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.diff.gz' libxcomposite_0.4.4-1.diff.gz 15633 SHA256:09fe6dd7d98d935e7307d57f926912d477b929f06c159962840d3a398f376988
```

### `dpkg` source package: `libxcursor=1:1.1.14-1ubuntu0.16.04.2`

Binary Packages:

- `libxcursor1:amd64=1:1.1.14-1ubuntu0.16.04.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcursor=1:1.1.14-1ubuntu0.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.14-1ubuntu0.16.04.2.dsc' libxcursor_1.1.14-1ubuntu0.16.04.2.dsc 2429 SHA512:176793e157220d8a6d922407ee154cc11cec2d107479ad818581a3863b7eec1575c9d80ef70dfc654a60025246562c25458e90e1661ae6db9bd25dd1bf7d456f
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.14.orig.tar.gz' libxcursor_1.1.14.orig.tar.gz 374910 SHA512:dfd4e538118a5c4aef3f089c9b029f4e80a62bff163950b2a0ed6450acf0217d59d15128f9df31211e88d93daa22cedf6ec65ce27fd3e20a426531d24fe58043
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.14-1ubuntu0.16.04.2.diff.gz' libxcursor_1.1.14-1ubuntu0.16.04.2.diff.gz 19882 SHA512:fe8f9436ce2904c2390c313477f83bf2cfa024a4064de2c9a7bac88845d8afbc7026840201cb98e9950e84eb3f67641382c8174e751f81d1902efa03cd25056c
```

### `dpkg` source package: `libxdamage=1:1.1.4-2`

Binary Packages:

- `libxdamage1:amd64=1:1.1.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdamage=1:1.1.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4-2.dsc' libxdamage_1.1.4-2.dsc 2127 SHA256:43cbefb5c69f51d89a11cf84718fe0c42058fc9b6ec7c0076e7c37b9e829feb5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4.orig.tar.gz' libxdamage_1.1.4.orig.tar.gz 339060 SHA256:4bb3e9d917f5f593df2277d452926ee6ad96de7b7cd1017cbcf4579fe5d3442b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4-2.diff.gz' libxdamage_1.1.4-2.diff.gz 14930 SHA256:d238c1a266c30cd124ede7e6c86635bfaa108fa552c4a82919101cebf22670e9
```

### `dpkg` source package: `libxdmcp=1:1.1.2-1.1`

Binary Packages:

- `libxdmcp6:amd64=1:1.1.2-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.2-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-1.1.dsc' libxdmcp_1.1.2-1.1.dsc 2098 SHA256:605175ee859f00ace43a4c35dc2d7c60971c0e1f21769b508b5bce2303979436
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2.orig.tar.gz' libxdmcp_1.1.2.orig.tar.gz 404115 SHA256:6f7c7e491a23035a26284d247779174dedc67e34e93cc3548b648ffdb6fc57c0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-1.1.diff.gz' libxdmcp_1.1.2-1.1.diff.gz 17944 SHA256:d764e8d251d06c9e5a50783cee393c621b7288bc3369d158b6a1d2e4372f3c9e
```

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

- `libxext6:amd64=2:1.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3-1.dsc' libxext_1.3.3-1.dsc 2221 SHA256:47106df75b8f3db1e43803e8e94a2e966cd23f7daa8cfc393af739a9e33ef955
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3.orig.tar.gz' libxext_1.3.3.orig.tar.gz 468441 SHA256:eb0b88050491fef4716da4b06a4d92b4fc9e76f880d6310b2157df604342cfe5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3-1.diff.gz' libxext_1.3.3-1.diff.gz 20763 SHA256:e294a4884eb68acbd151312cb0c973aad63268b637b15ccf1911864b7197557e
```

### `dpkg` source package: `libxfixes=1:5.0.1-2`

Binary Packages:

- `libxfixes3:amd64=1:5.0.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxfixes=1:5.0.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.1-2.dsc' libxfixes_5.0.1-2.dsc 2160 SHA256:1569c87546b8d59ee7f60b395b10ea1a6f9d52418aed9d7cf2d633b14a1f1f25
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.1.orig.tar.gz' libxfixes_5.0.1.orig.tar.gz 352057 SHA256:81b692856c0e7ab2778a34a32aa6b3f455b9b58cf388f009cba872ed933ae9c0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.1-2.diff.gz' libxfixes_5.0.1-2.diff.gz 6564 SHA256:df62260744ac03e8354b004685d439c32588e826c9dc570b6109070447601ce0
```

### `dpkg` source package: `libxi=2:1.7.6-1`

Binary Packages:

- `libxi6:amd64=2:1.7.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxi=2:1.7.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.6-1.dsc' libxi_1.7.6-1.dsc 2269 SHA256:b0d205346b418dbfbdd36dadc164e6050bcfa5cd691f190c9aa0ac91d2a0e5e8
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.6.orig.tar.gz' libxi_1.7.6.orig.tar.gz 601628 SHA256:4e88fa7decd287e58140ea72238f8d54e4791de302938c83695fc0c9ac102b7e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.6-1.diff.gz' libxi_1.7.6-1.diff.gz 10149 SHA256:ae61f11cd06263d7a4caf25835fdd8ba4e8ad319781acb1e0cd177eab82ce8a7
```

### `dpkg` source package: `libxinerama=2:1.1.3-1`

Binary Packages:

- `libxinerama1:amd64=2:1.1.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxinerama=2:1.1.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3-1.dsc' libxinerama_1.1.3-1.dsc 2198 SHA256:4cf9a3558bd7ce1b4f55a581175c05e4b4a172364458a21ff4b657b714688fbb
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3.orig.tar.gz' libxinerama_1.1.3.orig.tar.gz 350141 SHA256:0ba243222ae5aba4c6a3d7a394c32c8b69220a6872dbb00b7abae8753aca9a44
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3-1.diff.gz' libxinerama_1.1.3-1.diff.gz 15738 SHA256:2b1487e3511ddabfec666a62f6e5e8ac4f97536b0d53c51f7bf4cbe07508a130
```

### `dpkg` source package: `libxml2=2.9.3+dfsg1-1ubuntu0.7`

Binary Packages:

- `libxml2:amd64=2.9.3+dfsg1-1ubuntu0.7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.3+dfsg1-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1-1ubuntu0.7.dsc' libxml2_2.9.3+dfsg1-1ubuntu0.7.dsc 2756 SHA512:1a2083bfc7196c9bf9074cbfc1c8d4adf22469c8b3a4983cdaa30e8b9e8a4a2c36015c58bb1eb5a7df39fd07b9ad11ea304cd64337af75ef08850f2ef0c384c8
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1.orig.tar.xz' libxml2_2.9.3+dfsg1.orig.tar.xz 2475440 SHA512:e6766405ce0dd462679e9097a83a782440315ca685a95950725f4fe9e51fd1f83928f9d690ab7ce46c2f491b793c9bb7917081d3e2bb8811409c75727af680a7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1-1ubuntu0.7.debian.tar.xz' libxml2_2.9.3+dfsg1-1ubuntu0.7.debian.tar.xz 57976 SHA512:4c4ece08dd2d7b8ffcd6964fbeebdda3854c0c2ce46781b4e96c47e9130f829da1b3e7c5036e3f25d61c5f099f76fe2991f1e12e6404ee582ad2ea3069c4c6f6
```

### `dpkg` source package: `libxrandr=2:1.5.0-1`

Binary Packages:

- `libxrandr2:amd64=2:1.5.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrandr=2:1.5.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.0-1.dsc' libxrandr_1.5.0-1.dsc 2125 SHA256:e1fe17d69676e15108ff6c6c3eedc2c3c72fef8a9dd9bde1ac9f4f4467efdfd1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.0.orig.tar.gz' libxrandr_1.5.0.orig.tar.gz 382147 SHA256:1b594a149e6b124aab7149446f2fd886461e2935eca8dca43fe83a70cf8ec451
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.0-1.diff.gz' libxrandr_1.5.0-1.diff.gz 13507 SHA256:f04e5dccdee7db84d534aa4423b927710fbffe513c0ec632f92129a70323334e
```

### `dpkg` source package: `libxrender=1:0.9.9-0ubuntu1`

Binary Packages:

- `libxrender1:amd64=1:0.9.9-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.9-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.9-0ubuntu1.dsc' libxrender_0.9.9-0ubuntu1.dsc 1562 SHA256:3b9304baa99c34df694a673aeffc1e44d7564f1e0efa71ac542435afcfd0f334
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.9.orig.tar.gz' libxrender_0.9.9.orig.tar.gz 371568 SHA256:beeac64ff8d225f775019eb7c688782dee9f4cc7b412a65538f8dde7be4e90fe
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.9-0ubuntu1.diff.gz' libxrender_0.9.9-0ubuntu1.diff.gz 18873 SHA256:b02577c21b37a46cd0b554ab25ad4bfd49545e02774b4ab2b80c2deae93abd91
```

### `dpkg` source package: `libxshmfence=1.2-1`

Binary Packages:

- `libxshmfence1:amd64=1.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxshmfence=1.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.2-1.dsc' libxshmfence_1.2-1.dsc 2128 SHA256:85a28d2f6211ebbf0a115d0f72d874cce179178958bcb2a77094e3499464b25d
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.2.orig.tar.gz' libxshmfence_1.2.orig.tar.gz 355356 SHA256:58467a0e36fc4ec749dc55f81a4ab3b822c82b6dfb7d36bdb6b28c9fd2a5ccaf
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.2-1.diff.gz' libxshmfence_1.2-1.diff.gz 13284 SHA256:65db7e07c5c5b12d0b1f93cdb0c4e3e448429240044247ea2f64a89c0cce5f8e
```

### `dpkg` source package: `libxxf86vm=1:1.1.4-1`

Binary Packages:

- `libxxf86vm1:amd64=1:1.1.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxxf86vm=1:1.1.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.dsc' libxxf86vm_1.1.4-1.dsc 2078 SHA256:5a3aded030a415b0d6c201d2b9d3af36f241dc981f10052fd4c2b56d59597838
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4.orig.tar.gz' libxxf86vm_1.1.4.orig.tar.gz 363146 SHA256:5108553c378a25688dcb57dca383664c36e293d60b1505815f67980ba9318a99
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.diff.gz' libxxf86vm_1.1.4-1.diff.gz 8040 SHA256:e0f11739d28c7a4475820ebda26e6f29e6cfa80b99a3513c075471132c81725b
```

### `dpkg` source package: `libyaml=0.1.6-3`

Binary Packages:

- `libyaml-0-2:amd64=0.1.6-3`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.1.6-3
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.6-3.dsc' libyaml_0.1.6-3.dsc 1893 SHA256:ed5bc299d3bcc0b038206f8780639d4682e65f521dff571b9336e2f8626d0011
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.6.orig.tar.gz' libyaml_0.1.6.orig.tar.gz 503012 SHA256:7da6971b4bd08a986dd2a61353bc422362bd0edcc67d7ebaac68c95f74182749
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.6-3.debian.tar.xz' libyaml_0.1.6-3.debian.tar.xz 4268 SHA256:fd567e6918903833e5c4f1f87254c550eca07c2bba1ccbe6031da33243cf4297
```

### `dpkg` source package: `linux=4.4.0-190.220`

Binary Packages:

- `linux-libc-dev:amd64=4.4.0-190.220`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`
- `redpine-signals`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lksctp-tools=1.0.16+dfsg-3`

Binary Packages:

- `libsctp-dev=1.0.16+dfsg-3`
- `libsctp1:amd64=1.0.16+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libsctp-dev/copyright`, `/usr/share/doc/libsctp1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris lksctp-tools=1.0.16+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.16+dfsg-3.dsc' lksctp-tools_1.0.16+dfsg-3.dsc 2037 SHA256:8c77a6faa221ae9c1ab8f404585badd88542d1507f37d583c23b0c816a562c78
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.16+dfsg.orig.tar.gz' lksctp-tools_1.0.16+dfsg.orig.tar.gz 206656 SHA256:6935a57bdc052805796f538257eb78e23af02481e01f3d72dc0fa00688bdd502
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.16+dfsg-3.debian.tar.xz' lksctp-tools_1.0.16+dfsg-3.debian.tar.xz 9300 SHA256:27fd297b40e1087b447c5eabe5029ed8c4e33f8513324b6801750efa89589378
```

### `dpkg` source package: `llvm-toolchain-6.0=1:6.0-1ubuntu2~16.04.1`

Binary Packages:

- `libllvm6.0:amd64=1:6.0-1ubuntu2~16.04.1`

Licenses: (parsed from: `/usr/share/doc/libllvm6.0/copyright`)

- `ARM`
- `Apple`
- `BSD-3-Clause`
- `BSD-3-clause`
- `Expat`
- `LLVM`
- `MIT`
- `NCSA`
- `Polly`
- `Python`
- `U-OF-I-BSD-LIKE`
- `public-domain`
- `solar-public-domain`

Source:

```console
$ apt-get source -qq --print-uris llvm-toolchain-6.0=1:6.0-1ubuntu2~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.dsc' llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.dsc 6967 SHA512:d8adfb5a3568d149cc74f37091fd9c986cbe388af373c1dfd40eb663b9d1adbce14b185a71519c743543a53e440974c93fbb5112fdbed6f3a832b2f7e8100064
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-clang-tools-extra.tar.bz2' llvm-toolchain-6.0_6.0.orig-clang-tools-extra.tar.bz2 808825 SHA512:59bcc4d379115cbf2effa912d4a475a03809832e109dd86df661db3f2dc5915def1c6379a61c389d0b744a1e6fc0365a390ac7d793258343a3e9b9aeec3e25c3
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-clang.tar.bz2' llvm-toolchain-6.0_6.0.orig-clang.tar.bz2 13228782 SHA512:5f1c5e4258b8f4132bf2e40878862ee9108381c0c50b1e3ace6c6f5287a83c6325896815ed69f0dc01db4a4dbe0c0d68f045770fd2ad64e9d055775ed3dc8146
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-compiler-rt.tar.bz2' llvm-toolchain-6.0_6.0.orig-compiler-rt.tar.bz2 2145520 SHA512:a9cc0688a105a6204781297ee4d3fa57b14a018a9aa3a8a83f67be823ac83ffa5f396a8f591cb0a9810abd98b342799a595a324f1197b69a329db54aa02a3a3d
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-lld.tar.bz2' llvm-toolchain-6.0_6.0.orig-lld.tar.bz2 853733 SHA512:376cf5657e06e12e4e3bf91bd788b4028e8b2e09a4a2a87024284e3ab09abd2d0598d5b5e3500d73dbb8b97ba3d5843a826419b44838350b5d56b8305ab67fae
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-lldb.tar.bz2' llvm-toolchain-6.0_6.0.orig-lldb.tar.bz2 11238461 SHA512:4fa69c8f1ff35951440536accf2b4218e984d03d9d75007715a86270d417e7bf1dab8ed2604b03c3eefb8addbce7e499c07c53ebd6f0ead5e4ae9d83f212b753
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-polly.tar.bz2' llvm-toolchain-6.0_6.0.orig-polly.tar.bz2 3253870 SHA512:0099b77390d8cd04adf6609b54f30bfa4352bed994f2aa6ced785a364fa3fdf548c0cf4540959c90d8131c2eef256c204614fd5907c762caaa6cab1a4800028d
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig.tar.bz2' llvm-toolchain-6.0_6.0.orig.tar.bz2 29853313 SHA512:8d948ee0bd3e4c53806f6b267832dc6b7729a36e88f1131c019fcb849f3a4b7328e8ea4333921eb85f91a21be48f9d422b4c17a630f46552c250c401180a0200
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.debian.tar.xz' llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.debian.tar.xz 70280 SHA512:8b75a9dda27d97e9865077582060a0a9ef8336dc3b897c0dab8d43d93d11d7ec2346343981b57c600f70906339079f7b89ecfee3b87c034ee6040354df6b7d72
```

### `dpkg` source package: `lm-sensors=1:3.4.0-2`

Binary Packages:

- `libsensors4:amd64=1:3.4.0-2`

Licenses: (parsed from: `/usr/share/doc/libsensors4/copyright`)

- `GPL`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lm-sensors=1:3.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0-2.dsc' lm-sensors_3.4.0-2.dsc 1964 SHA256:bd3cecc8bbef17a0213d1ec38bdaca3a1cafae93cab116d17b5d7eec9a62d60f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0.orig.tar.bz2' lm-sensors_3.4.0.orig.tar.bz2 175802 SHA256:e0579016081a262dd23eafe1d22b41ebde78921e73a1dcef71e05e424340061f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0-2.debian.tar.xz' lm-sensors_3.4.0-2.debian.tar.xz 28484 SHA256:efdb87b87c37be8a1eb478d78046838c3ab0178ffad23dce3f159fbf89e24d9c
```

### `dpkg` source package: `log4cxx=0.10.0-10ubuntu1`

Binary Packages:

- `liblog4cxx-dev=0.10.0-10ubuntu1`
- `liblog4cxx10-dev=0.10.0-10ubuntu1`
- `liblog4cxx10v5:amd64=0.10.0-10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/liblog4cxx-dev/copyright`, `/usr/share/doc/liblog4cxx10-dev/copyright`, `/usr/share/doc/liblog4cxx10v5/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris log4cxx=0.10.0-10ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0-10ubuntu1.dsc' log4cxx_0.10.0-10ubuntu1.dsc 2357 SHA256:1542a14c438984569db723d75b30759caec87c9fa026816051e7645fe68baf94
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0.orig.tar.gz' log4cxx_0.10.0.orig.tar.gz 1667425 SHA256:0de0396220a9566a580166e66b39674cb40efd2176f52ad2c65486c99c920c8c
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0-10ubuntu1.debian.tar.xz' log4cxx_0.10.0-10ubuntu1.debian.tar.xz 14580 SHA256:246017b62c4ce215310bf888b20642f668007b7736f7c70ab221b468cb42becb
```

### `dpkg` source package: `lsb=9.20160110ubuntu0.2`

Binary Packages:

- `lsb-base=9.20160110ubuntu0.2`
- `lsb-release=9.20160110ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`, `/usr/share/doc/lsb-release/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20160110ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20160110ubuntu0.2.dsc' lsb_9.20160110ubuntu0.2.dsc 2160 SHA512:27e7a82161c88850592a04d1d326859723ac1b4b897f006c1e66f7ebe6d325907da5566bc877d6e4edcdeb55328a3960952fc4286a2827100b119c73553e9e89
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20160110ubuntu0.2.tar.xz' lsb_9.20160110ubuntu0.2.tar.xz 57832 SHA512:b794cdbba25bf9079eb17f2b695490a8b35d10afb90ff5ca6f5c7188c1f9a80fb3d2b59749f87c88188733a05563cf81964e6a66beed4def020d7218aa20a253
```

### `dpkg` source package: `lvm2=2.02.133-1ubuntu10`

Binary Packages:

- `libdevmapper1.02.1:amd64=2:1.02.110-1ubuntu10`

Licenses: (parsed from: `/usr/share/doc/libdevmapper1.02.1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris lvm2=2.02.133-1ubuntu10
'http://archive.ubuntu.com/ubuntu/pool/main/l/lvm2/lvm2_2.02.133-1ubuntu10.dsc' lvm2_2.02.133-1ubuntu10.dsc 3151 SHA256:49b49c886da1f5b5d078875a025ee5f37d049e77c3abe49568b3b6fd7babb5de
'http://archive.ubuntu.com/ubuntu/pool/main/l/lvm2/lvm2_2.02.133.orig.tar.xz' lvm2_2.02.133.orig.tar.xz 1356636 SHA256:79c6fc85f28b6af1870d7e3b06d8339270746a5028f47a5b412f4394156ed846
'http://archive.ubuntu.com/ubuntu/pool/main/l/lvm2/lvm2_2.02.133-1ubuntu10.debian.tar.xz' lvm2_2.02.133-1ubuntu10.debian.tar.xz 42320 SHA256:54f13369a8576c98472dcc9121e3ac4fd69f3af02d2aa4a7aeb0224e87176d1e
```

### `dpkg` source package: `lz4=0.0~r131-2ubuntu2`

Binary Packages:

- `liblz4-1:amd64=0.0~r131-2ubuntu2`
- `liblz4-dev:amd64=0.0~r131-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`, `/usr/share/doc/liblz4-dev/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=0.0~r131-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu2.dsc' lz4_0.0~r131-2ubuntu2.dsc 2007 SHA256:123f23834f83a4dca6d74a611cc0294491bd339d2e0be04d65783d6debbccc02
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131.orig.tar.gz' lz4_0.0~r131.orig.tar.gz 133784 SHA256:9d4d00614d6b9dec3114b33d1224b6262b99ace24434c53487a0c8fd0b18cfed
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu2.debian.tar.xz' lz4_0.0~r131-2ubuntu2.debian.tar.xz 5224 SHA256:c0afb4a440b1e7b803e2d9dcf616be539c1d16baebc681cdf837000e4c5077b7
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

### `dpkg` source package: `make-dfsg=4.1-6`

Binary Packages:

- `make=4.1-6`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.1-6
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-6.dsc' make-dfsg_4.1-6.dsc 1840 SHA256:c28066ebe2002e4791ac3a4e808d8a5f0bed75eff8e0462449a08ab767153361
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1.orig.tar.gz' make-dfsg_4.1.orig.tar.gz 1350231 SHA256:b3ed04fb6718289e4a430afbe2df6ecba9177aad9f6d09aaf38e5409262ca8a3
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-6.diff.gz' make-dfsg_4.1-6.diff.gz 42552 SHA256:b647e6961a9707ea009de85fb65f8156143deab139be1636a200abdffe5e91c3
```

### `dpkg` source package: `makedev=2.3.1-93ubuntu2~ubuntu16.04.1`

Binary Packages:

- `makedev=2.3.1-93ubuntu2~ubuntu16.04.1`

Licenses: (parsed from: `/usr/share/doc/makedev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris makedev=2.3.1-93ubuntu2~ubuntu16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/makedev/makedev_2.3.1-93ubuntu2~ubuntu16.04.1.dsc' makedev_2.3.1-93ubuntu2~ubuntu16.04.1.dsc 1855 SHA512:af060ae534668d751781e0fe8577a0250d62b6a5a7a6849b617a3b1fbc378899950fca46dbd9937288bc94c7b66c42f1fc7ef4400ad3dc6031d3fb2e36addb00
'http://archive.ubuntu.com/ubuntu/pool/main/m/makedev/makedev_2.3.1.orig.tar.gz' makedev_2.3.1.orig.tar.gz 9924 SHA512:640df51e214dfa3be1b7425fb9cd6477f1b4da57441a58243913aae12e1b2c0b7ef35906384cb79975fda4f6c747534f9f72dde59b742ac3bc26c87cb69f65f5
'http://archive.ubuntu.com/ubuntu/pool/main/m/makedev/makedev_2.3.1-93ubuntu2~ubuntu16.04.1.diff.gz' makedev_2.3.1-93ubuntu2~ubuntu16.04.1.diff.gz 50340 SHA512:384886ff3f0792cf67cdf5126af5f8d4dbf31ede75fdb339c1b53fdd15e7f0abc91d53297a3c5bf908e2c3c21be51f0766a37da51b92f5c8f7a5e6d81c916912
```

### `dpkg` source package: `mawk=1.3.3-17ubuntu2`

Binary Packages:

- `mawk=1.3.3-17ubuntu2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu2.dsc' mawk_1.3.3-17ubuntu2.dsc 1843 SHA256:d9058945d45b0e9ee5dd1c9c2e16d8f28b96d5c2e777f743594096fa2a5e277b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu2.diff.gz' mawk_1.3.3-17ubuntu2.diff.gz 63882 SHA256:670103046767474be29e80f2143dc67e3d0b958972f5942c3df94883f978eded
```

### `dpkg` source package: `mercurial=3.7.3-1ubuntu1.2`

Binary Packages:

- `mercurial=3.7.3-1ubuntu1.2`
- `mercurial-common=3.7.3-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=3.7.3-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_3.7.3-1ubuntu1.2.dsc' mercurial_3.7.3-1ubuntu1.2.dsc 2387 SHA512:c9cafa2ee08866a91a02d0a3f4362e643d21f389e8ac59e045ec8c5d4993de2a424ebddfba2c8dd7636be6db86ccc989a1458ee2809e1339a04fc341427303f0
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_3.7.3.orig.tar.gz' mercurial_3.7.3.orig.tar.gz 4636732 SHA512:7f9f97229e40c7092c16ccf227b19a08a9839d8ce19a9d057341fff75876bff32241ee9aa10eab293f779ea3e8a1d97577597187bd96251fb499cbb1075a82cf
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_3.7.3-1ubuntu1.2.debian.tar.xz' mercurial_3.7.3-1ubuntu1.2.debian.tar.xz 65164 SHA512:f21eb0f5ee75b090add089e14d2ec8547f11c6e0b9f305636d10a75a0dce9b4d7b5113fb58b94742c73f3df730f171b5ba1487e8db10992e507938195fe5f253
```

### `dpkg` source package: `mesa=18.0.5-0ubuntu0~16.04.1`

Binary Packages:

- `libgl1-mesa-dri:amd64=18.0.5-0ubuntu0~16.04.1`
- `libgl1-mesa-glx:amd64=18.0.5-0ubuntu0~16.04.1`
- `libglapi-mesa:amd64=18.0.5-0ubuntu0~16.04.1`

Licenses: (parsed from: `/usr/share/doc/libgl1-mesa-dri/copyright`, `/usr/share/doc/libgl1-mesa-glx/copyright`, `/usr/share/doc/libglapi-mesa/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris mesa=18.0.5-0ubuntu0~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5-0ubuntu0~16.04.1.dsc' mesa_18.0.5-0ubuntu0~16.04.1.dsc 5261 SHA512:5ecfdbb5e84056c2560394dcb894c5e4a074a616d0942a08851c6d824bc546d909e0575d027b09f838c5cfee8bb052519d6f93947dd0502cda0a7355536078a7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5.orig.tar.gz' mesa_18.0.5.orig.tar.gz 19123780 SHA512:a8fff267edf1b34a3f27e5d579200105039a9f64de561a84343a9609d50d2f30d4eba31b2f862fbee9f73157f2061bc37ea1b8ecd75b556dae03bcb40f0a6b6b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5.orig.tar.gz.asc' mesa_18.0.5.orig.tar.gz.asc 879 SHA512:e8064d859e71f214114a24fcc00238cda4a02f5a86f04f0dbcf52d0831a45a9f712e70d94a12cd57fb0efff2df26274d756240b5e010c9d0da1540561d583274
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5-0ubuntu0~16.04.1.diff.gz' mesa_18.0.5-0ubuntu0~16.04.1.diff.gz 144399 SHA512:f9c0271b842bbd0e35ca04eac5f94d615ae9d5b22bf737db4c575985f1918ba08f885a1412f46b0daa96ef53b80ea4ae2b7f05a619e2021db916fafddb24932b
```

### `dpkg` source package: `mime-support=3.59ubuntu1`

Binary Packages:

- `mime-support=3.59ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.59ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.59ubuntu1.dsc' mime-support_3.59ubuntu1.dsc 1711 SHA256:37703b2273222f23dd8ad048f898a381412df0a76473047e0b7757a8043ff354
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.59ubuntu1.tar.gz' mime-support_3.59ubuntu1.tar.gz 37508 SHA256:55ee4350da8425fb65e7c9b60518e20de09c5a72d08148e644fcefe7abf9c83d
```

### `dpkg` source package: `mpclib3=1.0.3-1`

Binary Packages:

- `libmpc3:amd64=1.0.3-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.0.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.0.3-1.dsc' mpclib3_1.0.3-1.dsc 1940 SHA256:4b424e1c6063d48fd0d045b5afe37004346dae267ced0994fa8e11ff41cada45
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.0.3.orig.tar.gz' mpclib3_1.0.3.orig.tar.gz 669925 SHA256:617decc6ea09889fb08ede330917a00b16809b8db88c29c31bfbb49cbf88ecc3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.0.3-1.diff.gz' mpclib3_1.0.3-1.diff.gz 3684 SHA256:5a3fe9a7eddb4428d42e95f5919cce517f17411acdb2a73013a8f1a2bb246565
```

### `dpkg` source package: `mpdecimal=2.4.2-1`

Binary Packages:

- `libmpdec2:amd64=2.4.2-1`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1.dsc' mpdecimal_2.4.2-1.dsc 1893 SHA256:5bc782829357ebc9f0c12084642319e5ac89784a119433f8bfba7a11008d7c13
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1.debian.tar.xz' mpdecimal_2.4.2-1.debian.tar.xz 5172 SHA256:b95fb775fd04a7ad34fa5bd2c222b49ee2dfd7f0e15295dbd3f7fb86a9b0194b
```

### `dpkg` source package: `mpfr4=3.1.4-1`

Binary Packages:

- `libmpfr4:amd64=3.1.4-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr4/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=3.1.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_3.1.4-1.dsc' mpfr4_3.1.4-1.dsc 1965 SHA256:98c867cd9e2d82fd9f1bae851a3ec8e76aa35d9e54d9e0d75a2fcd97f08992a9
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_3.1.4.orig.tar.xz' mpfr4_3.1.4.orig.tar.xz 1122152 SHA256:761413b16d749c53e2bfd2b1dfaa3b027b0e793e404b90b5fbaeef60af6517f5
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_3.1.4-1.debian.tar.xz' mpfr4_3.1.4-1.debian.tar.xz 9656 SHA256:e0562521ac0ef9fc2039ef1305962ee1ad529ae2210e197cee0080b1facc4d60
```

### `dpkg` source package: `mpi-defaults=1.4`

Binary Packages:

- `mpi-default-bin=1.4`
- `mpi-default-dev=1.4`

Licenses: (parsed from: `/usr/share/doc/mpi-default-bin/copyright`, `/usr/share/doc/mpi-default-dev/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpi-defaults=1.4
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mpi-defaults/mpi-defaults_1.4.dsc' mpi-defaults_1.4.dsc 2569 SHA256:89e9088d21d774eefebcf9c487c67a3f133a1991466bf474c68a987dd672ef08
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mpi-defaults/mpi-defaults_1.4.tar.xz' mpi-defaults_1.4.tar.xz 4544 SHA256:aa85c486ad60c23eb6d8c44353e5fa1985e935314d54b2d5b86f8fb844386ce3
```

### `dpkg` source package: `mysql-5.7=5.7.31-0ubuntu0.16.04.1`

Binary Packages:

- `libmysqlclient20:amd64=5.7.31-0ubuntu0.16.04.1`
- `mysql-common=5.7.31-0ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libmysqlclient20/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-like`
- `Boost`
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
$ apt-get source -qq --print-uris mysql-5.7=5.7.31-0ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.31-0ubuntu0.16.04.1.dsc' mysql-5.7_5.7.31-0ubuntu0.16.04.1.dsc 3380 SHA512:018062a4d992af874db3535d2b3627a43ec840c4a9fd4da6556a179fab77cabd58136d2a95fcdc40c4d5a41935e63bfddbfc1ee784a4ab34bd89ee32869b7f7b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.31.orig.tar.gz' mysql-5.7_5.7.31.orig.tar.gz 51382559 SHA512:d7fc1927c860562d121658031bcbd58d36a942340423bf7b692cef84c29e67b56d009c9f9bb10cde8acabd6f9db58c67eb542349eccc4719fb38c8570738700a
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.31-0ubuntu0.16.04.1.debian.tar.xz' mysql-5.7_5.7.31-0ubuntu0.16.04.1.debian.tar.xz 251200 SHA512:0d161e70ab28b02f7d04e2b1c975d4f0dce714d51a98de48b9e76856698b4a1b0f72ab8d652646152b6111430d69641d9e20738e2da7dbfca992a38410b95c8e
```

### `dpkg` source package: `ncurses=6.0+20160213-1ubuntu1`

Binary Packages:

- `libncurses5:amd64=6.0+20160213-1ubuntu1`
- `libncursesw5:amd64=6.0+20160213-1ubuntu1`
- `libtinfo5:amd64=6.0+20160213-1ubuntu1`
- `ncurses-base=6.0+20160213-1ubuntu1`
- `ncurses-bin=6.0+20160213-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.0+20160213-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.0+20160213-1ubuntu1.dsc' ncurses_6.0+20160213-1ubuntu1.dsc 4379 SHA256:16628fbe5a690f6f8d147a54d0ba6900a0afeaa51d318475781ce3f14df1ca79
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.0+20160213.orig.tar.gz' ncurses_6.0+20160213.orig.tar.gz 3153008 SHA256:20269c2dd62a311b9a3fb9f25638d35a057a5ece5f8d6caf4e70a3da6f01082c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.0+20160213-1ubuntu1.debian.tar.xz' ncurses_6.0+20160213-1ubuntu1.debian.tar.xz 54496 SHA256:9551738e1bdc425d12897cc459ce5ce40b5e12530b144b731c0a7b3e077c07c7
```

### `dpkg` source package: `netifaces=0.10.4-0.1build2`

Binary Packages:

- `python-netifaces=0.10.4-0.1build2`

Licenses: (parsed from: `/usr/share/doc/python-netifaces/copyright`)

- `MIT-style`

Source:

```console
$ apt-get source -qq --print-uris netifaces=0.10.4-0.1build2
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4-0.1build2.dsc' netifaces_0.10.4-0.1build2.dsc 2445 SHA256:e46a3f6cc4610341fbcc2ef2a2ef9f02749e502f36d23bcc8237692dd9ad4b38
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4.orig.tar.gz' netifaces_0.10.4.orig.tar.gz 22969 SHA256:9656a169cb83da34d732b0eb72b39373d48774aee009a3d1272b7ea2ce109cde
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4-0.1build2.debian.tar.xz' netifaces_0.10.4-0.1build2.debian.tar.xz 8392 SHA256:74683411b2e5e3ddeaea0ff59152406437899abec98cc7e5b93eeeef7c7d437c
```

### `dpkg` source package: `nettle=3.2-1ubuntu0.16.04.1`

Binary Packages:

- `libhogweed4:amd64=3.2-1ubuntu0.16.04.1`
- `libnettle6:amd64=3.2-1ubuntu0.16.04.1`

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
$ apt-get source -qq --print-uris nettle=3.2-1ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.2-1ubuntu0.16.04.1.dsc' nettle_3.2-1ubuntu0.16.04.1.dsc 2200 SHA512:5908a35a2f45bccb890a1b1c7df32d4501e5eaf99d08a8f2c33a3cd2322efed1d5a42e8a8900e0e5c30cacb6e86f96e2e810c3e36f4a6f8d0a2e9e0ed5bdbbeb
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.2.orig.tar.gz' nettle_3.2.orig.tar.gz 1879604 SHA512:9f2c802e8b683d1c2fd8d16ab33b2a1efda33a1bf33196be39031a2d0677f2e78d67221a718997780e157aa72973da7d9d549429e706fcfcdff97ee3bbef615a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.2-1ubuntu0.16.04.1.debian.tar.xz' nettle_3.2-1ubuntu0.16.04.1.debian.tar.xz 21340 SHA512:97a4c851a63dad2298809aa29f2ab8a37367fc21f5d134ad297124f648991e5da648a628a068e423fd3375633ed364ba920cdd03bb36f3ad349c9b598d21ff67
```

### `dpkg` source package: `nose=1.3.7-1`

Binary Packages:

- `python-nose=1.3.7-1`

Licenses: (parsed from: `/usr/share/doc/python-nose/copyright`)

- `Expat`
- `LGPL`
- `LGPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nose=1.3.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nose/nose_1.3.7-1.dsc' nose_1.3.7-1.dsc 2321 SHA256:ac09eaf25a19adfbf5dd712035fb1daaeae515d8b0a24829702c011162a62031
'http://archive.ubuntu.com/ubuntu/pool/main/n/nose/nose_1.3.7.orig.tar.gz' nose_1.3.7.orig.tar.gz 280488 SHA256:f1bffef9cbc82628f6e7d7b40d7e255aefaa1adb6a1b1d26c69a8b79e6208a98
'http://archive.ubuntu.com/ubuntu/pool/main/n/nose/nose_1.3.7-1.debian.tar.xz' nose_1.3.7-1.debian.tar.xz 11148 SHA256:02ffafd1f53e7be0b8967f1fc0c4d028f358ed32ea3fb1da43fe6a7090934b47
```

### `dpkg` source package: `npth=1.2-3`

Binary Packages:

- `libnpth0:amd64=1.2-3`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.2-3.dsc' npth_1.2-3.dsc 1960 SHA256:457abe6599eda4ab9f4dc73a4ee1e250269febe333e8a660716544a16d8552de
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.2.orig.tar.bz2' npth_1.2.orig.tar.bz2 298735 SHA256:6ddbdddb2cf49a4723f9d1ad6563c480d6760dcb63cb7726b8fc3bc2e1b6c08a
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.2-3.debian.tar.xz' npth_1.2-3.debian.tar.xz 10216 SHA256:b63d662bf8b2ad834c1dce75ae53af592c4b2d9d1e70ddc6ef82c98d7321045b
```

### `dpkg` source package: `numactl=2.0.11-1ubuntu1.1`

Binary Packages:

- `libnuma-dev:amd64=2.0.11-1ubuntu1.1`
- `libnuma1:amd64=2.0.11-1ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libnuma-dev/copyright`, `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.11-1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-1ubuntu1.1.dsc' numactl_2.0.11-1ubuntu1.1.dsc 2215 SHA512:1461e44244a711932e77144963086402a14dd2ab225fd2821484ce5a52e1bb34710092e03e223d413659f1d3d1a9fb24b07d5e5805f066bbdfb9908f14d7941f
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11.orig.tar.gz' numactl_2.0.11.orig.tar.gz 408175 SHA512:1969d7ee0ff3de0d6f1fa42ec089a17cdb3f92cb35d453b8f8b2eec49724c43787ecbd213357013a8f2500a260b0df9844d515815ca3a0376314a0eed050a0d4
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-1ubuntu1.1.diff.gz' numactl_2.0.11-1ubuntu1.1.diff.gz 7106 SHA512:0978c76dcf4baae21e12fbf02e9cda341c9d73199b912b546b08a3f836f1ec1786e3a7ee78ae158ba339b2f6fa521660b32fad9972ed0fd8e09b93966051a1c9
```

### `dpkg` source package: `openldap=2.4.42+dfsg-2ubuntu3.9`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.42+dfsg-2ubuntu3.9`
- `libldap2-dev:amd64=2.4.42+dfsg-2ubuntu3.9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.42+dfsg-2ubuntu3.9
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.42+dfsg-2ubuntu3.9.dsc' openldap_2.4.42+dfsg-2ubuntu3.9.dsc 3054 SHA512:e27501e68d3274a2b2ed321feadd2f5127f15557accd7c5dc94fa16c37d4551932ffd136adbea0904f321530613908f10a61853ce76ce9952de36021546962d3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.42+dfsg.orig.tar.gz' openldap_2.4.42+dfsg.orig.tar.gz 4813173 SHA512:4ed671baef513927cc340dac15b8979dba766d4fd629cae0bad1e125d09bc4ae61fda6912e06c53f8ef2cee6c2e28379b4e0c419c00c8254dc0cc0c715caf200
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.42+dfsg-2ubuntu3.9.debian.tar.xz' openldap_2.4.42+dfsg-2ubuntu3.9.debian.tar.xz 181648 SHA512:7c05acbe23c869b7089de6c5ee91b5d7be10e3c5497b9c2ef0f0937b10e71c36820aa9d23bae0392f2b888afec560136a98a6ff1fff6fca407ef09e11d8f0ab7
```

### `dpkg` source package: `openmpi=1.10.2-8ubuntu1`

Binary Packages:

- `libopenmpi-dev=1.10.2-8ubuntu1`
- `libopenmpi1.10=1.10.2-8ubuntu1`
- `openmpi-bin=1.10.2-8ubuntu1`
- `openmpi-common=1.10.2-8ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libopenmpi-dev/copyright`, `/usr/share/doc/libopenmpi1.10/copyright`, `/usr/share/doc/openmpi-bin/copyright`, `/usr/share/doc/openmpi-common/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris openmpi=1.10.2-8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_1.10.2-8ubuntu1.dsc' openmpi_1.10.2-8ubuntu1.dsc 2639 SHA256:0d45a031372bfdf0a5fc07f8b8320819a4755449b4efb2450b0a8b9ee272d1b5
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_1.10.2.orig.tar.gz' openmpi_1.10.2.orig.tar.gz 20143146 SHA256:218136734653fde6304cc26137b292b0893cb2d401290bad983ac90de9bcafee
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_1.10.2-8ubuntu1.debian.tar.xz' openmpi_1.10.2-8ubuntu1.debian.tar.xz 31736 SHA256:b402ee58b24798c198e64f033a5df1928b3949795eca2c0930c9fdcfa99b89f2
```

### `dpkg` source package: `openssl=1.0.2g-1ubuntu4.17`

Binary Packages:

- `libssl1.0.0:amd64=1.0.2g-1ubuntu4.17`
- `openssl=1.0.2g-1ubuntu4.17`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.0.2g-1ubuntu4.17
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g-1ubuntu4.17.dsc' openssl_1.0.2g-1ubuntu4.17.dsc 2453 SHA512:05d469083cecdd1f237fe539778b8f6fe69b073e6e147a26a225d86d91de76602db37ae93cbfffcadfb97ad139895c81a9ff1ed158eec7cb1c90829f950d4e2a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g.orig.tar.gz' openssl_1.0.2g.orig.tar.gz 5266102 SHA512:4d96b6c8a232203483d6e8bee81da01ba10977bfbac92f25304a36dec9ea584b7ef917bc45e097cc7dbe681d71a4570d649c22244c178393ae91fab48323f735
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g-1ubuntu4.17.debian.tar.xz' openssl_1.0.2g-1ubuntu4.17.debian.tar.xz 137312 SHA512:ddd764c12d0057253d233c2b3e6af93cf7440a4815875ed2550ecef297401353d0c8a6d652ae23a159060ddeebfee5e1a5831d59359d8cd7bad2c06b9dae99fe
```

### `dpkg` source package: `p11-kit=0.23.2-5~ubuntu16.04.1`

Binary Packages:

- `libp11-kit0:amd64=0.23.2-5~ubuntu16.04.1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.2-5~ubuntu16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.2-5~ubuntu16.04.1.dsc' p11-kit_0.23.2-5~ubuntu16.04.1.dsc 2326 SHA512:e9563291cf8752d08dc5632652c87f8f8552f27f7b54209339ee1b1d67ec8674882621c4a7f381f455e3454acb6afd6f232c61b71ae84b16f3eecdd209247bd3
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.2.orig.tar.gz' p11-kit_0.23.2.orig.tar.gz 1022733 SHA512:b665d89f0d752a41b01ec53e29c801c4fdcaf3f21fce524984b10acef0477ad5dbac085edd35ffb747423d0e1e09660b8d29501c979cf54937d3b9d2561cf18f
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.2-5~ubuntu16.04.1.debian.tar.xz' p11-kit_0.23.2-5~ubuntu16.04.1.debian.tar.xz 15208 SHA512:26514c75dd90eb2816a66b4e7fc37087600092111fd7a4b47919bee6c9e2c62a5f67d2f167ecdce4c449eb0b7f08c0286e08eaccdc334eadfd3f1a1e39c9242b
```

### `dpkg` source package: `pam=1.1.8-3.2ubuntu2.1`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.2ubuntu2.1`
- `libpam-modules-bin=1.1.8-3.2ubuntu2.1`
- `libpam-runtime=1.1.8-3.2ubuntu2.1`
- `libpam0g:amd64=1.1.8-3.2ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pango1.0=1.38.1-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.38.1-1`
- `libpangocairo-1.0-0:amd64=1.38.1-1`
- `libpangoft2-1.0-0:amd64=1.38.1-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.38.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.38.1-1.dsc' pango1.0_1.38.1-1.dsc 3171 SHA256:786e84e8a00ab1b062f05356dbd371b771ef3fe3cf09144ba1de6b0668929e24
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.38.1.orig.tar.xz' pango1.0_1.38.1.orig.tar.xz 1047372 SHA256:1320569f6c6d75d6b66172b2d28e59c56ee864ee9df202b76799c4506a214eb7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.38.1-1.debian.tar.xz' pango1.0_1.38.1-1.debian.tar.xz 29216 SHA256:673a39fb35b469af653a819a65e778563fc4be3fa8265e7321006f9be06df143
```

### `dpkg` source package: `paramiko=1.16.0-1ubuntu0.2`

Binary Packages:

- `python-paramiko=1.16.0-1ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/python-paramiko/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris paramiko=1.16.0-1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_1.16.0-1ubuntu0.2.dsc' paramiko_1.16.0-1ubuntu0.2.dsc 2451 SHA512:68c222022e817b129a85dbe055b68c984778073f08059a09a320c3aeb65282e4d4b37dc81ffa4e9d4b7be384d522186e09787b48245421e130f9c21b4b87d6a9
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_1.16.0.orig.tar.gz' paramiko_1.16.0.orig.tar.gz 266200 SHA512:d7088cdd444a2b3c495c79bcc002167721e0d15cb517f4b719c6fbbfaba3b0d578d080988bee3f2606ccc18c2c255055543c4066a5a8ce56f593da4b6a089d46
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_1.16.0-1ubuntu0.2.debian.tar.xz' paramiko_1.16.0-1ubuntu0.2.debian.tar.xz 12380 SHA512:82351f8dfc954a9a90374a3a34219c6772aed57cfa0314c15131be79a0b1c9a61ffb75505532b7a0319a3de0e30135eaa30063c11e25d6af2da318e913be1553
```

### `dpkg` source package: `patch=2.7.5-1ubuntu0.16.04.2`

Binary Packages:

- `patch=2.7.5-1ubuntu0.16.04.2`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.5-1ubuntu0.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.5-1ubuntu0.16.04.2.dsc' patch_2.7.5-1ubuntu0.16.04.2.dsc 1950 SHA512:f55ca716b52f58d0a6e6fbf6ed9f60a73ce5f337f47ec312f3c090dc4601d1d91df4de0d808dce0fda1f892388e7e2043bcd037a8a93854a3477d1beca6ff930
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.5.orig.tar.xz' patch_2.7.5.orig.tar.xz 727704 SHA512:6620ac8101f60c0b456ce339fa5e371f40be0b391e2e9728f34f3625f9907e516de61dac2f91bc76e6fd28a9bd1224efc3ba827cfaa606d857730c1af4195a0f
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.5-1ubuntu0.16.04.2.debian.tar.xz' patch_2.7.5-1ubuntu0.16.04.2.debian.tar.xz 12588 SHA512:473af88a4c06f86236dee935178a4b688d25c8ed99e0a7b5072012d10220f0b382e9e00d79394df3ea674dadda61e515a6aa9851c710d5b9163c16eee360caa8
```

### `dpkg` source package: `pcre3=2:8.38-3.1`

Binary Packages:

- `libpcre3:amd64=2:8.38-3.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.38-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38-3.1.dsc' pcre3_8.38-3.1.dsc 2074 SHA256:6a46bc62c33198fe38257f0dddecb4c534825f8f066bf88f2a45ad935b879885
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38.orig.tar.gz' pcre3_8.38.orig.tar.gz 2053336 SHA256:9883e419c336c63b0cb5202b09537c140966d585e4d0da66147dc513da13e629
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38-3.1.debian.tar.gz' pcre3_8.38-3.1.debian.tar.gz 32289 SHA256:9ee1b838c1de50cb5f6641016d0dd21b06f1038b9b7c3b1098e0a89b9c24b39f
```

### `dpkg` source package: `perl=5.22.1-9ubuntu0.6`

Binary Packages:

- `libperl5.22:amd64=5.22.1-9ubuntu0.6`
- `perl=5.22.1-9ubuntu0.6`
- `perl-base=5.22.1-9ubuntu0.6`
- `perl-modules-5.22=5.22.1-9ubuntu0.6`

Licenses: (parsed from: `/usr/share/doc/libperl5.22/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.22/copyright`)

- `Artistic`
- `Artistic,`
- `Artistic-2`
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
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.22.1-9ubuntu0.6
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.22.1-9ubuntu0.6.dsc' perl_5.22.1-9ubuntu0.6.dsc 2480 SHA512:f7a1e1711cf72b49da8491e70c8d7f15855bf02c066935f22fc31513f859c51870d092fe4197c92390e0e05a9f122275648086506819ca66f7fd6709bfac51bf
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.22.1.orig.tar.xz' perl_5.22.1.orig.tar.xz 11223940 SHA512:f214bf6959e582a04034c9343a270fcc4fdcf959a8fbb393433865446e634024809d194cfd07ab614b2c09a5a73caec0a74945bbbb3d690663a5f6f10eb168b8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.22.1-9ubuntu0.6.debian.tar.xz' perl_5.22.1-9ubuntu0.6.debian.tar.xz 161972 SHA512:a38e8ce74b247c4215aad6753dc3418929388c9354120716bda1731302c08e661ae6cecc6cc5010e685a64cbdf461714eb291b128e8ebe819bf3974b79bfe749
```

### `dpkg` source package: `pinentry=0.9.7-3`

Binary Packages:

- `pinentry-curses=0.9.7-3`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=0.9.7-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_0.9.7-3.dsc' pinentry_0.9.7-3.dsc 2662 SHA256:67506f8c21b87a274aa7d9bc7a40a2da094dcbcf32e5b0a8f9c94512404ea747
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_0.9.7.orig.tar.bz2' pinentry_0.9.7.orig.tar.bz2 432978 SHA256:6398208394972bbf897c3325780195584682a0d0c164ca5a0da35b93b1e4e7b2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_0.9.7-3.debian.tar.xz' pinentry_0.9.7-3.debian.tar.xz 13032 SHA256:1d3f5b2ad83234537482ec0b78c5b411b25c84e91dfa1fdbebb1dbc8f1677b8f
```

### `dpkg` source package: `pixman=0.33.6-1`

Binary Packages:

- `libpixman-1-0:amd64=0.33.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.33.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6-1.dsc' pixman_0.33.6-1.dsc 2085 SHA256:08e94c263c3cde1c841458512705fa6a52a78c8f48e31f0bf3a2ae8a518eb51e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6.orig.tar.gz' pixman_0.33.6.orig.tar.gz 878996 SHA256:4e1e72c0ed31d10944f304976e87e6c87b441c853713eeecf115e22c23d4b17d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6-1.diff.gz' pixman_0.33.6-1.diff.gz 315093 SHA256:f382e753698aa95fae9019128a4b463935695b4c906785397f3eaa04e05a06d5
```

### `dpkg` source package: `pkg-config=0.29.1-0ubuntu1`

Binary Packages:

- `pkg-config=0.29.1-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.1-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu1.dsc' pkg-config_0.29.1-0ubuntu1.dsc 1842 SHA256:0ade40d184e9684f9e22e622022f1b798123cc63cd37d669f664f47dddc5e072
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1.orig.tar.gz' pkg-config_0.29.1.orig.tar.gz 2013454 SHA256:beb43c9e064555469bd4390dcfd8030b1536e0aa103f08d7abf7ae8cac0cb001
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu1.diff.gz' pkg-config_0.29.1-0ubuntu1.diff.gz 12597 SHA256:1c44aeeec1896a69f21861e9b9e18bb783258d57f4bd678b173b3890f1a209bf
```

### `dpkg` source package: `poco=1.3.6p1-5.1ubuntu0.1`

Binary Packages:

- `libpoco-dev=1.3.6p1-5.1ubuntu0.1`
- `libpococrypto9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocodata9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocofoundation9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocomysql9v5=1.3.6p1-5.1ubuntu0.1`
- `libpoconet9v5=1.3.6p1-5.1ubuntu0.1`
- `libpoconetssl9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocoodbc9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocosqlite9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocoutil9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocoxml9v5=1.3.6p1-5.1ubuntu0.1`
- `libpocozip9v5=1.3.6p1-5.1ubuntu0.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris poco=1.3.6p1-5.1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.3.6p1-5.1ubuntu0.1.dsc' poco_1.3.6p1-5.1ubuntu0.1.dsc 3581 SHA512:453dba94ec44e0cd18432c88de8658de70886c0eba9b8971aa311c989f2f8cdfc073808a005a0dddfd6e205854634ce689a46714c89533217c5b1a6737a06943
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.3.6p1.orig.tar.gz' poco_1.3.6p1.orig.tar.gz 3057466 SHA512:260073f596bde3d0732a5e25200f96d74067bfee6ceea4773dca18bc654d742f8642d431a26eafbb0390f8ff4962280024ace2cc5a8187816a13a07392b836d9
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.3.6p1-5.1ubuntu0.1.diff.gz' poco_1.3.6p1-5.1ubuntu0.1.diff.gz 16150 SHA512:85289358302e26bdf4fc14368b3800c125f1ea828ad1ab60e1395e60ec0b043a9387e022a55d83b58cf5905e45fd80e15e14975c5797915953d8942b1af088d9
```

### `dpkg` source package: `procps=2:3.3.10-4ubuntu2.5`

Binary Packages:

- `libprocps4:amd64=2:3.3.10-4ubuntu2.5`
- `procps=2:3.3.10-4ubuntu2.5`

Licenses: (parsed from: `/usr/share/doc/libprocps4/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.10-4ubuntu2.5
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10-4ubuntu2.5.dsc' procps_3.3.10-4ubuntu2.5.dsc 2227 SHA512:a247fdd9aa5c23eaa2aa5110e102db86de1f8162f738d2278af9bce2e8c0a1aa2a59903cd338344a2453f64121a5946d43211638a045850b97a9813616c0cb2c
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10.orig.tar.xz' procps_3.3.10.orig.tar.xz 814816 SHA512:ab7627e46301d479a56a073cd7e6ff02dc85e7cba73cf0b9a0ca9288cd1aef2f6dac9413cefd8ee75ca84a3d1c5f38e5afc5c4969e31c96b276ce21c79ac5c34
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10-4ubuntu2.5.debian.tar.xz' procps_3.3.10-4ubuntu2.5.debian.tar.xz 44704 SHA512:4ded69c9fb63c4ae7410b7304271454060f4ec51f54dc49ebd60393ce54aa45d5ec6a4a7f763900572a3e92cb704143e5410b1fb3ab519d54d2c588b0afea401
```

### `dpkg` source package: `pyparsing=2.0.3+dfsg1-1ubuntu0.1`

Binary Packages:

- `python-pyparsing=2.0.3+dfsg1-1ubuntu0.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python-catkin-pkg-modules=0.4.22-1`

Binary Packages:

- `python-catkin-pkg-modules=0.4.22-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python-catkin-pkg=0.4.22-100`

Binary Packages:

- `python-catkin-pkg=0.4.22-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python-crypto=2.6.1-6ubuntu0.16.04.3`

Binary Packages:

- `python-crypto=2.6.1-6ubuntu0.16.04.3`

Licenses: (parsed from: `/usr/share/doc/python-crypto/copyright`)

- `BSD-3-clause`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris python-crypto=2.6.1-6ubuntu0.16.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-crypto/python-crypto_2.6.1-6ubuntu0.16.04.3.dsc' python-crypto_2.6.1-6ubuntu0.16.04.3.dsc 2484 SHA512:adbda54ecbb44f2d82412f4a7bdd3eeca34b255b3f50035e12e6102c094b454f3e2f3aa08e2bc0162a5e03ab9c6d0937ece936b6489fcdfcacbcb197626ea050
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-crypto/python-crypto_2.6.1.orig.tar.gz' python-crypto_2.6.1.orig.tar.gz 446240 SHA512:20a4aed4dac4e9e61d773ebc1d48ea577e9870c33f396be53d075a9bf8487d93e75e200179882d81e452efd0f6751789bac434f6f431b3e7c1c8ef9dba392847
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-crypto/python-crypto_2.6.1-6ubuntu0.16.04.3.debian.tar.xz' python-crypto_2.6.1-6ubuntu0.16.04.3.debian.tar.xz 23680 SHA512:f1eebeb0cb095cfcd42edb4f7f6bd1aaa1e73062dcf28494360448f83aec015d5f63070c1338b529423673f7ed226511d7a80be32ca902c2399cca119fd6fa2c
```

### `dpkg` source package: `python-dateutil=2.4.2-1`

Binary Packages:

- `python-dateutil=2.4.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-dateutil=2.4.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.4.2-1.dsc' python-dateutil_2.4.2-1.dsc 2028 SHA256:34c1175aa8c7eb7bf271cce80a4a91c7baf07109fd5ee1f2cd9f6637eeac7f7e
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.4.2.orig.tar.gz' python-dateutil_2.4.2.orig.tar.gz 209120 SHA256:3e95445c1db500a344079a47b171c45ef18f57d188dffdb0e4165c71bea8eb3d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.4.2-1.debian.tar.xz' python-dateutil_2.4.2-1.debian.tar.xz 13052 SHA256:7fe7a48fea9086fe1b827435f75414e1501cab94b62377d49834edefaa335996
```

### `dpkg` source package: `python-defaults=2.7.12-1~16.04`

Binary Packages:

- `libpython-dev:amd64=2.7.12-1~16.04`
- `libpython-stdlib:amd64=2.7.12-1~16.04`
- `python=2.7.12-1~16.04`
- `python-dev=2.7.12-1~16.04`
- `python-minimal=2.7.12-1~16.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.12-1~16.04
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.12-1~16.04.dsc' python-defaults_2.7.12-1~16.04.dsc 2659 SHA512:408cd2d8aca9ea0573c68b4a14a3ceb98d7199e427350b3fa530b680a78641af1a5e16f3614c79723aaf0c0f44779844ab86874d2e6bb90d996bd3f6bd5e7b74
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.12-1~16.04.tar.gz' python-defaults_2.7.12-1~16.04.tar.gz 280070 SHA512:92fa75b66b29205348f1a13542b82ede82ce8233f0f4df56e4482774bf991dc295152137500cdd4d2a8ce3bccff028302a5b5323648ec8038b84cca6aca92adb
```

### `dpkg` source package: `python-docutils=0.12+dfsg-1`

Binary Packages:

- `docutils-common=0.12+dfsg-1`
- `python-docutils=0.12+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/docutils-common/copyright`, `/usr/share/doc/python-docutils/copyright`)

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
$ apt-get source -qq --print-uris python-docutils=0.12+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.12+dfsg-1.dsc' python-docutils_0.12+dfsg-1.dsc 2413 SHA256:31a1084d7612de374d876c540fcc18cfaf17f7a8cca7c8f8a15b4bad9cb16711
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.12+dfsg.orig.tar.gz' python-docutils_0.12+dfsg.orig.tar.gz 1624713 SHA256:644b21131ce0503047b754613d017852a943807bb73e616f7f0c3b3e8a22b21d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.12+dfsg-1.debian.tar.xz' python-docutils_0.12+dfsg-1.debian.tar.xz 29520 SHA256:b5a9e07208579f92d76d8689c35b16635ee6cbdbfe8f8f2a4d5277007f0cc489
```

### `dpkg` source package: `python-ecdsa=0.13-2ubuntu0.16.04.1`

Binary Packages:

- `python-ecdsa=0.13-2ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/python-ecdsa/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-ecdsa=0.13-2ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-ecdsa/python-ecdsa_0.13-2ubuntu0.16.04.1.dsc' python-ecdsa_0.13-2ubuntu0.16.04.1.dsc 2310 SHA512:c8d89809c1b477b90cc5bdd07257034dcb923c95651f88fb5167bc14b90fb00807c8b342ed15d217afa666011a51b27426182d78afdbeceb4c579876db44e0fa
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-ecdsa/python-ecdsa_0.13.orig.tar.gz' python-ecdsa_0.13.orig.tar.gz 55579 SHA512:f21d4d196404455135a1a2255c889ffa26160ea1e9b9d16c914ea82614831816acb6d27c86aac68cdaafa8b1d5fefe065b5f49ce45acaae4a035cd7f08a97594
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-ecdsa/python-ecdsa_0.13-2ubuntu0.16.04.1.debian.tar.xz' python-ecdsa_0.13-2ubuntu0.16.04.1.debian.tar.xz 10816 SHA512:69d2a1effcc5ce133802966bae6daa2528955fd00971262ef30acad592b06d5d4351df2afd7fa3ff9bcbe3d616edd46ff215319f86bc24526af7983ecfcd4c0b
```

### `dpkg` source package: `python-numpy=1:1.11.0-1ubuntu1`

Binary Packages:

- `python-numpy=1:1.11.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python-numpy/copyright`)

- `PSF`

Source:

```console
$ apt-get source -qq --print-uris python-numpy=1:1.11.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-numpy/python-numpy_1.11.0-1ubuntu1.dsc' python-numpy_1.11.0-1ubuntu1.dsc 2749 SHA256:fa52a860df53f5c4f037b45352f837952dc932a54126e75d245c1363379025c9
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-numpy/python-numpy_1.11.0.orig.tar.gz' python-numpy_1.11.0.orig.tar.gz 4169494 SHA256:a1d1268d200816bfb9727a7a27b78d8e37ecec2e4d5ebd33eb64e2789e0db43e
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-numpy/python-numpy_1.11.0-1ubuntu1.debian.tar.xz' python-numpy_1.11.0-1ubuntu1.debian.tar.xz 143480 SHA256:3539a4c6cf92305f8a671c318cfda9767b029819366cf10db7a584effa9e55d8
```

### `dpkg` source package: `python-roman=2.0.0-2`

Binary Packages:

- `python-roman=2.0.0-2`

Licenses: (parsed from: `/usr/share/doc/python-roman/copyright`)

- `Python-2.1.1`
- `ZPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris python-roman=2.0.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0-2.dsc' python-roman_2.0.0-2.dsc 2138 SHA256:d522dccc7e20d45208bd5dcb58fec644142c90223b1e7841282ed1b73bdfbc9b
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0.orig.tar.gz' python-roman_2.0.0.orig.tar.gz 4968 SHA256:98f2c0fb3cdcfba465d12c85b3b7139fc4cd2177f1325f1bacfe00878c8fa7b9
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0-2.debian.tar.xz' python-roman_2.0.0-2.debian.tar.xz 8508 SHA256:fdb23384ad4ab4701214c5776bb2b181e794a347d024fc0483e4ebe5055f4362
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


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python-rosdistro=0.8.2-100`

Binary Packages:

- `python-rosdistro=0.8.2-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python-rosinstall=0.7.8-1`

Binary Packages:

- `python-rosinstall=0.7.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-rosinstall=0.7.8-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosinstall/python-rosinstall_0.7.8-1.debian.tar.gz' python-rosinstall_0.7.8-1.debian.tar.gz 1008 SHA512:44bebf6ed0d14fa358e766096319cc304e70cd370c2f4ae13befdb5db0cbda1a4bda03d96b5ce57c0b0b4a7a82e96aa0ba280a9714c35460de6b59548a6a098d
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosinstall/python-rosinstall_0.7.8-1.dsc' python-rosinstall_0.7.8-1.dsc 917 SHA512:cadb27334167a8b5bbee35303642f09dbbb5d6cf827852400146d14f400d1a2dc5ce8e880889141cadfd072518541e9004af8458114a713eee63866b15288ebd
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-rosinstall/python-rosinstall_0.7.8.orig.tar.gz' python-rosinstall_0.7.8.orig.tar.gz 26425 SHA512:013b313b9e442e9b68f7aad0a372d2c1dfb9efeb66b9f20d01943bf58808e0e0bc69db848ba1c2460f0ecfaba89d385e987ccb574a7139b6500d5f958eda4d1b
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

### `dpkg` source package: `python-setuptools=20.7.0-1`

Binary Packages:

- `python-pkg-resources=20.7.0-1`
- `python-setuptools=20.7.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-setuptools=20.7.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-setuptools/python-setuptools_20.7.0-1.dsc' python-setuptools_20.7.0-1.dsc 2338 SHA256:0251fd94c77aacd604e5a5f851136c21048879491628f2732bd95dd72d8256c1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-setuptools/python-setuptools_20.7.0.orig.tar.gz' python-setuptools_20.7.0.orig.tar.gz 645861 SHA256:505cdf282c5f6e3a056e79f0244b8945f3632257bba8469386c6b9b396400233
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-setuptools/python-setuptools_20.7.0-1.debian.tar.xz' python-setuptools_20.7.0-1.debian.tar.xz 38772 SHA256:6fe8762b58c0a5582aae975f4d97a2ef7ad66df221b0455366727ce7d17cb0aa
```

### `dpkg` source package: `python-vcstools=0.1.42-1`

Binary Packages:

- `python-vcstools=0.1.42-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-vcstools=0.1.42-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-vcstools/python-vcstools_0.1.42-1.debian.tar.xz' python-vcstools_0.1.42-1.debian.tar.xz 1212 SHA512:0a1122589d1e95fb4448af5d7d6551abe52533ea7e065bf09e00e042dac1ecac0eb691ac580b818130ca214f970dee0c4cd07f49966dbe122d95023ad01d7c9a
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-vcstools/python-vcstools_0.1.42-1.dsc' python-vcstools_0.1.42-1.dsc 935 SHA512:398ed97732ecd681cdfa6ea6d6f90709dada18d2c4287eb732de42d5dcb997d69e5f135927a949fc7734b375113ca3a74c9fa4ae7dae8c1b6bc90bdf3edc8232
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-vcstools/python-vcstools_0.1.42.orig.tar.gz' python-vcstools_0.1.42.orig.tar.gz 54462 SHA512:92f1eb9edb1c39c6179b8ca05169e0ad053a141f71309c91647c67a380abaa504953ff87d742dce846fa8d7116616e8f4656cc232cf73bb81f6920f6bd795f80
```

### `dpkg` source package: `python-wstool=0.1.17-1`

Binary Packages:

- `python-wstool=0.1.17-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-wstool=0.1.17-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-wstool/python-wstool_0.1.17-1.debian.tar.gz' python-wstool_0.1.17-1.debian.tar.gz 1045 SHA512:aba9c213555c16dbcc326422f14fcf76ab2ddf943d5fe38f4fe75f30cb885b14b4008a0e21029091be6030fa2eb1a0e6a35403aed84a6dfb0ef862025bdaacd8
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-wstool/python-wstool_0.1.17-1.dsc' python-wstool_0.1.17-1.dsc 888 SHA512:41d47d5a14b274454c2f8e01d3e429b8ae8e61da66c3bb6442ceba232645cec4a7efb13848de16c21ca5f8fee7a312ac0628a812800aaf9b41fa54b5b3b75547
'http://packages.ros.org/ros/ubuntu/pool/main/p/python-wstool/python-wstool_0.1.17.orig.tar.gz' python-wstool_0.1.17.orig.tar.gz 53327 SHA512:e2512ac47376c409e49c3b2ad88f696335509f2b7d8b934d6e730208bf6a47f821f5ce65e153dea50b8fe3554af228e356df5ee54e90a708f8eda5f5b5fee9c1
```

### `dpkg` source package: `python2.7=2.7.12-1ubuntu0~16.04.12`

Binary Packages:

- `libpython2.7:amd64=2.7.12-1ubuntu0~16.04.12`
- `libpython2.7-dev:amd64=2.7.12-1ubuntu0~16.04.12`
- `libpython2.7-minimal:amd64=2.7.12-1ubuntu0~16.04.12`
- `libpython2.7-stdlib:amd64=2.7.12-1ubuntu0~16.04.12`
- `python2.7=2.7.12-1ubuntu0~16.04.12`
- `python2.7-dev=2.7.12-1ubuntu0~16.04.12`
- `python2.7-minimal=2.7.12-1ubuntu0~16.04.12`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python3-defaults=3.5.1-3`

Binary Packages:

- `libpython3-stdlib:amd64=3.5.1-3`
- `python3=3.5.1-3`
- `python3-minimal=3.5.1-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.5.1-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.5.1-3.dsc' python3-defaults_3.5.1-3.dsc 2715 SHA256:e1da92b6e0a03c096ad1442b2ee9ea00ea7f8f02a5f8ce59bc3a75db276e8556
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.5.1-3.tar.gz' python3-defaults_3.5.1-3.tar.gz 924115 SHA256:8d1284430b77775d4cea62a33b0685e0523b8dfa2ebcc092d382af5cb5b4f237
```

### `dpkg` source package: `python3.5=3.5.2-2ubuntu0~16.04.11`

Binary Packages:

- `libpython3.5-minimal:amd64=3.5.2-2ubuntu0~16.04.11`
- `libpython3.5-stdlib:amd64=3.5.2-2ubuntu0~16.04.11`
- `python3.5=3.5.2-2ubuntu0~16.04.11`
- `python3.5-minimal=3.5.2-2ubuntu0~16.04.11`

Licenses: (parsed from: `/usr/share/doc/libpython3.5-minimal/copyright`, `/usr/share/doc/libpython3.5-stdlib/copyright`, `/usr/share/doc/python3.5/copyright`, `/usr/share/doc/python3.5-minimal/copyright`)

- `* Permission to use this software in any way is granted without`
- `Apache`
- `Apache-2`
- `Apache-2.0`
- `By obtaining, using, and/or copying this software and/or its`
- `Expat`
- `GPL-2`
- `ISC`
- `LGPL-2.1+`
- `PSF-2`
- `Permission  is  hereby granted,  free  of charge,  to  any person`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Permission to use, copy, modify,`
- `Python`
- `Redistribution`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `binary forms, with`
- `distribute this software`
- `distribute this software and`
- `distribute this software for any`
- `implied`
- `its`
- `see above, some license as Python`
- `use in source`
- `without`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pyyaml=3.11-3build1`

Binary Packages:

- `python-yaml=3.11-3build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pyyaml=3.11-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_3.11-3build1.dsc' pyyaml_3.11-3build1.dsc 2272 SHA256:9c1032cfb1feef2378838948bf11ee1f09713e8a31aff8758937a556712d9b91
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_3.11.orig.tar.gz' pyyaml_3.11.orig.tar.gz 248685 SHA256:c36c938a872e5ff494938b33b14aaa156cb439ec67548fcab3535bb78b0846e8
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_3.11-3build1.debian.tar.xz' pyyaml_3.11-3build1.debian.tar.xz 8328 SHA256:d9153073ce67e76e120ad6aedb9fd91a9aa2a60066be88b3cf51cef7aa7acc13
```

### `dpkg` source package: `readline6=6.3-8ubuntu2`

Binary Packages:

- `libreadline6:amd64=6.3-8ubuntu2`
- `readline-common=6.3-8ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libreadline6/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline6=6.3-8ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline6/readline6_6.3-8ubuntu2.dsc' readline6_6.3-8ubuntu2.dsc 2566 SHA256:3c7e3168dd1510f040325c1ab1e28c7fbde34d1a899005a98a894a9f27bd98f6
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline6/readline6_6.3.orig.tar.gz' readline6_6.3.orig.tar.gz 2468560 SHA256:56ba6071b9462f980c5a72ab0023893b65ba6debb4eeb475d7a563dc65cafd43
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline6/readline6_6.3-8ubuntu2.debian.tar.xz' readline6_6.3-8ubuntu2.debian.tar.xz 31232 SHA256:32d4f30dc92d79d722b04c2b678883245d2eccff2ed4f8591faebca7e6d81948
```

### `dpkg` source package: `ros-kinetic-actionlib-msgs=1.12.7-0xenial-20200811-174009+0000`

Binary Packages:

- `ros-kinetic-actionlib-msgs=1.12.7-0xenial-20200811-174009+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-actionlib=1.11.16-2xenial-20200828-002304+0000`

Binary Packages:

- `ros-kinetic-actionlib=1.11.16-2xenial-20200828-002304+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-bond-core=1.8.3-0xenial-20200828-012244+0000`

Binary Packages:

- `ros-kinetic-bond-core=1.8.3-0xenial-20200828-012244+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-bond=1.8.3-0xenial-20200811-174425+0000`

Binary Packages:

- `ros-kinetic-bond=1.8.3-0xenial-20200811-174425+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-bondcpp=1.8.3-0xenial-20200827-215303+0000`

Binary Packages:

- `ros-kinetic-bondcpp=1.8.3-0xenial-20200827-215303+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-bondpy=1.8.3-0xenial-20200827-222636+0000`

Binary Packages:

- `ros-kinetic-bondpy=1.8.3-0xenial-20200827-222636+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-catkin=0.7.20-1xenial-20191213-232805+0000`

Binary Packages:

- `ros-kinetic-catkin=0.7.20-1xenial-20191213-232805+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-class-loader=0.3.9-0xenial-20191214-003009+0000`

Binary Packages:

- `ros-kinetic-class-loader=0.3.9-0xenial-20191214-003009+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-cmake-modules=0.4.2-0xenial-20191214-002351+0000`

Binary Packages:

- `ros-kinetic-cmake-modules=0.4.2-0xenial-20191214-002351+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-common-msgs=1.12.7-0xenial-20200828-151604+0000`

Binary Packages:

- `ros-kinetic-common-msgs=1.12.7-0xenial-20200828-151604+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-cpp-common=0.6.11-0xenial-20191214-013837+0000`

Binary Packages:

- `ros-kinetic-cpp-common=0.6.11-0xenial-20191214-013837+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-diagnostic-msgs=1.12.7-0xenial-20200811-174226+0000`

Binary Packages:

- `ros-kinetic-diagnostic-msgs=1.12.7-0xenial-20200811-174226+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-dynamic-reconfigure=1.5.50-0xenial-20200828-002154+0000`

Binary Packages:

- `ros-kinetic-dynamic-reconfigure=1.5.50-0xenial-20200828-002154+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-gencpp=0.6.0-0xenial-20191214-033928+0000`

Binary Packages:

- `ros-kinetic-gencpp=0.6.0-0xenial-20191214-033928+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-geneus=2.2.6-0xenial-20191214-033904+0000`

Binary Packages:

- `ros-kinetic-geneus=2.2.6-0xenial-20191214-033904+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-genlisp=0.4.16-0xenial-20191214-033115+0000`

Binary Packages:

- `ros-kinetic-genlisp=0.4.16-0xenial-20191214-033115+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-genmsg=0.5.11-0xenial-20191214-013936+0000`

Binary Packages:

- `ros-kinetic-genmsg=0.5.11-0xenial-20191214-013936+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-gennodejs=2.0.1-0xenial-20191214-033136+0000`

Binary Packages:

- `ros-kinetic-gennodejs=2.0.1-0xenial-20191214-033136+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-genpy=0.6.14-1xenial-20200811-173012+0000`

Binary Packages:

- `ros-kinetic-genpy=0.6.14-1xenial-20200811-173012+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-geometry-msgs=1.12.7-0xenial-20200811-174526+0000`

Binary Packages:

- `ros-kinetic-geometry-msgs=1.12.7-0xenial-20200811-174526+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-message-filters=1.12.16-1xenial-20200827-232712+0000`

Binary Packages:

- `ros-kinetic-message-filters=1.12.16-1xenial-20200827-232712+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-message-generation=0.4.0-0xenial-20200811-173417+0000`

Binary Packages:

- `ros-kinetic-message-generation=0.4.0-0xenial-20200811-173417+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-message-runtime=0.4.12-0xenial-20200811-173307+0000`

Binary Packages:

- `ros-kinetic-message-runtime=0.4.12-0xenial-20200811-173307+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-mk=1.14.6-1xenial-20200811-180622+0000`

Binary Packages:

- `ros-kinetic-mk=1.14.6-1xenial-20200811-180622+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-nav-msgs=1.12.7-0xenial-20200811-174832+0000`

Binary Packages:

- `ros-kinetic-nav-msgs=1.12.7-0xenial-20200811-174832+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-nodelet-core=1.9.14-0xenial-20200828-012906+0000`

Binary Packages:

- `ros-kinetic-nodelet-core=1.9.14-0xenial-20200828-012906+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-nodelet-topic-tools=1.9.14-0xenial-20200828-003603+0000`

Binary Packages:

- `ros-kinetic-nodelet-topic-tools=1.9.14-0xenial-20200828-003603+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-nodelet=1.9.14-0xenial-20200827-220739+0000`

Binary Packages:

- `ros-kinetic-nodelet=1.9.14-0xenial-20200827-220739+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-pluginlib=1.11.3-0xenial-20200827-202801+0000`

Binary Packages:

- `ros-kinetic-pluginlib=1.11.3-0xenial-20200827-202801+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-ros-base=1.3.2-0xenial-20200828-154142+0000`

Binary Packages:

- `ros-kinetic-ros-base=1.3.2-0xenial-20200828-154142+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-ros-comm=1.12.16-1xenial-20200828-062249+0000`

Binary Packages:

- `ros-kinetic-ros-comm=1.12.16-1xenial-20200828-062249+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-ros-core=1.3.2-0xenial-20200828-152655+0000`

Binary Packages:

- `ros-kinetic-ros-core=1.3.2-0xenial-20200828-152655+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-ros-environment=1.0.1-1xenial-20191214-013549+0000`

Binary Packages:

- `ros-kinetic-ros-environment=1.0.1-1xenial-20191214-013549+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-ros=1.14.6-1xenial-20200811-181251+0000`

Binary Packages:

- `ros-kinetic-ros=1.14.6-1xenial-20200811-181251+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosbag-migration-rule=1.0.0-0xenial-20191214-002240+0000`

Binary Packages:

- `ros-kinetic-rosbag-migration-rule=1.0.0-0xenial-20191214-002240+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosbag-storage=1.12.16-1xenial-20200827-200332+0000`

Binary Packages:

- `ros-kinetic-rosbag-storage=1.12.16-1xenial-20200827-200332+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosbag=1.12.16-1xenial-20200827-234335+0000`

Binary Packages:

- `ros-kinetic-rosbag=1.12.16-1xenial-20200827-234335+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosbash=1.14.6-1xenial-20191214-033021+0000`

Binary Packages:

- `ros-kinetic-rosbash=1.14.6-1xenial-20191214-033021+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosboost-cfg=1.14.6-1xenial-20191214-013600+0000`

Binary Packages:

- `ros-kinetic-rosboost-cfg=1.14.6-1xenial-20191214-013600+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosbuild=1.14.6-1xenial-20200811-173837+0000`

Binary Packages:

- `ros-kinetic-rosbuild=1.14.6-1xenial-20200811-173837+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosclean=1.14.6-1xenial-20191214-001017+0000`

Binary Packages:

- `ros-kinetic-rosclean=1.14.6-1xenial-20191214-001017+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosconsole-bridge=0.5.2-0xenial-20200827-202929+0000`

Binary Packages:

- `ros-kinetic-rosconsole-bridge=0.5.2-0xenial-20200827-202929+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosconsole=1.12.16-1xenial-20200827-195233+0000`

Binary Packages:

- `ros-kinetic-rosconsole=1.12.16-1xenial-20200827-195233+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roscpp-core=0.6.11-0xenial-20191214-040930+0000`

Binary Packages:

- `ros-kinetic-roscpp-core=0.6.11-0xenial-20191214-040930+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roscpp-serialization=0.6.11-0xenial-20191214-040238+0000`

Binary Packages:

- `ros-kinetic-roscpp-serialization=0.6.11-0xenial-20191214-040238+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roscpp-traits=0.6.11-0xenial-20191214-035847+0000`

Binary Packages:

- `ros-kinetic-roscpp-traits=0.6.11-0xenial-20191214-035847+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roscpp=1.12.16-1xenial-20200827-200531+0000`

Binary Packages:

- `ros-kinetic-roscpp=1.12.16-1xenial-20200827-200531+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roscreate=1.14.6-1xenial-20191214-033755+0000`

Binary Packages:

- `ros-kinetic-roscreate=1.14.6-1xenial-20191214-033755+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosgraph-msgs=1.11.2-0xenial-20200811-180129+0000`

Binary Packages:

- `ros-kinetic-rosgraph-msgs=1.11.2-0xenial-20200811-180129+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosgraph=1.12.16-1xenial-20200827-195320+0000`

Binary Packages:

- `ros-kinetic-rosgraph=1.12.16-1xenial-20200827-195320+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roslang=1.14.6-1xenial-20191214-033123+0000`

Binary Packages:

- `ros-kinetic-roslang=1.14.6-1xenial-20191214-033123+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roslaunch=1.12.16-1xenial-20200827-202544+0000`

Binary Packages:

- `ros-kinetic-roslaunch=1.12.16-1xenial-20200827-202544+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roslib=1.14.6-1xenial-20191214-032958+0000`

Binary Packages:

- `ros-kinetic-roslib=1.14.6-1xenial-20191214-032958+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roslisp=1.9.23-1xenial-20200811-180828+0000`

Binary Packages:

- `ros-kinetic-roslisp=1.9.23-1xenial-20200811-180828+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roslz4=1.12.16-1xenial-20200827-195325+0000`

Binary Packages:

- `ros-kinetic-roslz4=1.12.16-1xenial-20200827-195325+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosmake=1.14.6-1xenial-20191214-014327+0000`

Binary Packages:

- `ros-kinetic-rosmake=1.14.6-1xenial-20191214-014327+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosmaster=1.12.16-1xenial-20200827-200617+0000`

Binary Packages:

- `ros-kinetic-rosmaster=1.12.16-1xenial-20200827-200617+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosmsg=1.12.16-1xenial-20200827-235855+0000`

Binary Packages:

- `ros-kinetic-rosmsg=1.12.16-1xenial-20200827-235855+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosnode=1.12.16-1xenial-20200828-001152+0000`

Binary Packages:

- `ros-kinetic-rosnode=1.12.16-1xenial-20200828-001152+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosout=1.12.16-1xenial-20200827-201816+0000`

Binary Packages:

- `ros-kinetic-rosout=1.12.16-1xenial-20200827-201816+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rospack=2.4.5-1xenial-20191214-014035+0000`

Binary Packages:

- `ros-kinetic-rospack=2.4.5-1xenial-20191214-014035+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosparam=1.12.16-1xenial-20200827-200621+0000`

Binary Packages:

- `ros-kinetic-rosparam=1.12.16-1xenial-20200827-200621+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rospy=1.12.16-1xenial-20200827-202400+0000`

Binary Packages:

- `ros-kinetic-rospy=1.12.16-1xenial-20200827-202400+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosservice=1.12.16-1xenial-20200828-001154+0000`

Binary Packages:

- `ros-kinetic-rosservice=1.12.16-1xenial-20200828-001154+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rostest=1.12.16-1xenial-20200827-231500+0000`

Binary Packages:

- `ros-kinetic-rostest=1.12.16-1xenial-20200827-231500+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rostime=0.6.11-0xenial-20191214-033908+0000`

Binary Packages:

- `ros-kinetic-rostime=0.6.11-0xenial-20191214-033908+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rostopic=1.12.16-1xenial-20200827-235904+0000`

Binary Packages:

- `ros-kinetic-rostopic=1.12.16-1xenial-20200827-235904+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-rosunit=1.14.6-1xenial-20191214-033816+0000`

Binary Packages:

- `ros-kinetic-rosunit=1.14.6-1xenial-20191214-033816+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-roswtf=1.12.16-1xenial-20200828-060500+0000`

Binary Packages:

- `ros-kinetic-roswtf=1.12.16-1xenial-20200828-060500+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-sensor-msgs=1.12.7-0xenial-20200828-055911+0000`

Binary Packages:

- `ros-kinetic-sensor-msgs=1.12.7-0xenial-20200828-055911+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-shape-msgs=1.12.7-0xenial-20200811-175504+0000`

Binary Packages:

- `ros-kinetic-shape-msgs=1.12.7-0xenial-20200811-175504+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-smclib=1.8.3-0xenial-20191214-041046+0000`

Binary Packages:

- `ros-kinetic-smclib=1.8.3-0xenial-20191214-041046+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-std-msgs=0.5.11-0xenial-20200811-173756+0000`

Binary Packages:

- `ros-kinetic-std-msgs=0.5.11-0xenial-20200811-173756+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-std-srvs=1.11.2-0xenial-20200811-173805+0000`

Binary Packages:

- `ros-kinetic-std-srvs=1.11.2-0xenial-20200811-173805+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-stereo-msgs=1.12.7-0xenial-20200828-140916+0000`

Binary Packages:

- `ros-kinetic-stereo-msgs=1.12.7-0xenial-20200828-140916+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-topic-tools=1.12.16-1xenial-20200827-232751+0000`

Binary Packages:

- `ros-kinetic-topic-tools=1.12.16-1xenial-20200827-232751+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-trajectory-msgs=1.12.7-0xenial-20200811-175515+0000`

Binary Packages:

- `ros-kinetic-trajectory-msgs=1.12.7-0xenial-20200811-175515+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-visualization-msgs=1.12.7-0xenial-20200811-175658+0000`

Binary Packages:

- `ros-kinetic-visualization-msgs=1.12.7-0xenial-20200811-175658+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-kinetic-xmlrpcpp=1.12.16-1xenial-20200827-195703+0000`

Binary Packages:

- `ros-kinetic-xmlrpcpp=1.12.16-1xenial-20200827-195703+0000`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d-1ubuntu0.1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.dsc' rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.dsc 2408 SHA512:51585f82a47b5c050148ff861fca899d13d0e77ce5095f782a5986e40df05afb45f23fd7bff9fcafadc5996eb3b8d369e9a6f0bca2a56f7576bcb205be6cd18b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.orig.tar.gz 149016 SHA512:dbafe796c99f61c75f12eb7f4b424b72c4538da09a732eeb1ed0a259139b6dc683d036b504593a4a5a1d6656ca72bf40b00117b6f6c4040e9061e5d07f889530
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.debian.tar.xz 9000 SHA512:d8bc31759d07b4b65b2f941126c0a6978bb5d33b1457aa541e2f7e20c5ebb99b4893f5eb73c482fd796ae8dc4ec5899421281b60a43b9c9f1da054b3c877699a
```

### `dpkg` source package: `sbcl=2:1.3.1-1ubuntu2`

Binary Packages:

- `sbcl=2:1.3.1-1ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris sbcl=2:1.3.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_1.3.1-1ubuntu2.dsc' sbcl_1.3.1-1ubuntu2.dsc 2136 SHA256:bf7fd7626842cc1192a3bb60b9188d9d57ed6f2dd1718fc570005d37f18d46b9
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_1.3.1.orig.tar.bz2' sbcl_1.3.1.orig.tar.bz2 5725055 SHA256:a2e547e471a368349a43b1feee78ca6139aae0c60b8fcaa6ab0fd0e5b8e0ed3d
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_1.3.1-1ubuntu2.debian.tar.xz' sbcl_1.3.1-1ubuntu2.debian.tar.xz 77924 SHA256:f0e6ad821b349dbfb226cd2610a91d81f9bca89ad44cba997c435a8fa0e5ac93
```

### `dpkg` source package: `sed=4.2.2-7`

Binary Packages:

- `sed=4.2.2-7`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris sed=4.2.2-7
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.2.2-7.dsc' sed_4.2.2-7.dsc 1974 SHA256:42f5764a279ac3f9b31d9e922024b519b950b35e82830e552839cd41fbb8e0b0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.2.2.orig.tar.bz2' sed_4.2.2.orig.tar.bz2 1059414 SHA256:f048d1838da284c8bc9753e4506b85a1e0cc1ea8999d36f6995bcb9460cddbd7
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.2.2-7.debian.tar.xz' sed_4.2.2-7.debian.tar.xz 85048 SHA256:416b70f601b40246c1daf7261f117ea9ff01564f574bd34871573fc5c9f74db7
```

### `dpkg` source package: `sensible-utils=0.0.9ubuntu0.16.04.1`

Binary Packages:

- `sensible-utils=0.0.9ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.9ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.9ubuntu0.16.04.1.dsc' sensible-utils_0.0.9ubuntu0.16.04.1.dsc 1514 SHA512:b888a311da2a29f7c79483c20148eaa0ca6d359f108c507bdca2fa6251b3fa24082513433e403c3f4176df91f21e0abe2665b3813007a84c370b18b3053de796
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.9ubuntu0.16.04.1.tar.xz' sensible-utils_0.0.9ubuntu0.16.04.1.tar.xz 54048 SHA512:2a928fdae2355e494b2c6c62d147c0e00286ed2d956262bc92c941692ce86499fd1f3b98d5b2bc89f113686fbcd882f5a7e5d65235159a521a84882c40cdb971
```

### `dpkg` source package: `serf=1.3.8-1`

Binary Packages:

- `libserf-1-1:amd64=1.3.8-1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache-2.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.8-1/


### `dpkg` source package: `sgml-base=1.26+nmu4ubuntu1`

Binary Packages:

- `sgml-base=1.26+nmu4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sgml-base/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris sgml-base=1.26+nmu4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.26+nmu4ubuntu1.dsc' sgml-base_1.26+nmu4ubuntu1.dsc 957 SHA256:0b11ab50b2c014793e6593f489f0a4dde796d351cab7520d9fa0629476982f00
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.26+nmu4ubuntu1.tar.gz' sgml-base_1.26+nmu4ubuntu1.tar.gz 12912 SHA256:93d99ea554da5fea0c8abe424042ba8237c86faebaa02976fb92db3d198a47b4
```

### `dpkg` source package: `shadow=1:4.2-3.1ubuntu5.4`

Binary Packages:

- `login=1:4.2-3.1ubuntu5.4`
- `passwd=1:4.2-3.1ubuntu5.4`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.2-3.1ubuntu5.4
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.2-3.1ubuntu5.4.dsc' shadow_4.2-3.1ubuntu5.4.dsc 2513 SHA512:b7de769873bc0941f55d5c64251fedbd434a72824d921ecd6d19f806a0412a878c64a61a6ed7632e67c1b3be48163d0f50834001641ca2876185f63b270b1b9a
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.2.orig.tar.xz' shadow_4.2.orig.tar.xz 1088696 SHA512:8c9b482c6006198766efe44df68c863116f7e4c8ee7056e7f9cd8f66af166944aab119f567da6f96cd34fb5dcf19fba9f5e3d7c226f0bc48e3aef4906497ae16
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.2-3.1ubuntu5.4.debian.tar.xz' shadow_4.2-3.1ubuntu5.4.debian.tar.xz 506364 SHA512:3502e415aa519109e421b383356d55d69e82f276a225cafad89a36af28a95be7a0695abec9ea2fc0fdbc02d20c68e385dc7a4bbc6c725b043daf65a66dc1b01f
```

### `dpkg` source package: `shared-mime-info=1.5-2ubuntu0.2`

Binary Packages:

- `shared-mime-info=1.5-2ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.5-2ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.5-2ubuntu0.2.dsc' shared-mime-info_1.5-2ubuntu0.2.dsc 2289 SHA512:5ea1898f91b3d8b182e57444206ee2ab3c98ce0337d33926dba657de37193e065697201a09d7330b541e7fcd82faa954e9c549e379ae147c3f3bcf7fd1fe1b7a
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.5.orig.tar.xz' shared-mime-info_1.5.orig.tar.xz 559040 SHA512:8a97c8fa5a60eede056a42c36d9f8d015bf2788feca4630397ef71ba2cfe29ad469fb1669c368674edd4661af6b2f6823377cc27525f44c61788533c0c28e22a
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.5-2ubuntu0.2.debian.tar.xz' shared-mime-info_1.5-2ubuntu0.2.debian.tar.xz 10548 SHA512:972127d29b38c599f27ae63a92b7965c59391babf5961acc9064b90b82358e311ca4913e001cfe53c2dcd3aee04aece7c3aeab1dcad6fd7003dfd21b86af6e5b
```

### `dpkg` source package: `six=1.10.0-3`

Binary Packages:

- `python-six=1.10.0-3`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.10.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.10.0-3.dsc' six_1.10.0-3.dsc 2158 SHA256:71f2d5ff8b999c471cc2e92712befe482351a5ae226321e0e795bc683c8729cb
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.10.0.orig.tar.gz' six_1.10.0.orig.tar.gz 29630 SHA256:105f8d68616f8248e24bf0e9372ef04d3cc10104f1980f54d57b2ce73a5ad56a
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.10.0-3.debian.tar.xz' six_1.10.0-3.debian.tar.xz 3668 SHA256:860cc57244ea4e69eb4ee3ad1b823472c20d868c1cc25745b236ba6c9e1f3563
```

### `dpkg` source package: `sqlite3=3.11.0-1ubuntu1.5`

Binary Packages:

- `libsqlite3-0:amd64=3.11.0-1ubuntu1.5`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.11.0-1ubuntu1.5
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0-1ubuntu1.5.dsc' sqlite3_3.11.0-1ubuntu1.5.dsc 2625 SHA512:45dea33802cee1cd37c14550c817283d43d41c11b58398c754e5c23ebc2eaeada2478217c9739a4e80534bcc3b9667adb904d59a6e8b6efe42293c8faaaa76a9
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0.orig-www.tar.xz' sqlite3_3.11.0.orig-www.tar.xz 3135012 SHA512:132ea8354b5c541b88e21af14ac3db5c741f904271c1027c06a10f19772aea839e0b88398791670fd68ccd9e01473431f5d5f67784f955dcab781c28ef551e03
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0.orig.tar.xz' sqlite3_3.11.0.orig.tar.xz 5122440 SHA512:6d918b52f0dc10e49a43ed5c10f177424bdc1373d48367b57580937c64aaed4836c23c06b4643549ca4bca1913233056fb23314be2023a22ba51ee19eb32b949
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0-1ubuntu1.5.debian.tar.xz' sqlite3_3.11.0-1ubuntu1.5.debian.tar.xz 45984 SHA512:54535155d3aa3626d1642224d339aff1a492c27589fbb55450de0e074bccb19162c01a2e23cd815a0dc7fdcd574f4cac283eaf7315cf94764b755eca5834040f
```

### `dpkg` source package: `subversion=1.9.3-2ubuntu1.3`

Binary Packages:

- `libsvn1:amd64=1.9.3-2ubuntu1.3`
- `subversion=1.9.3-2ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris subversion=1.9.3-2ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/s/subversion/subversion_1.9.3-2ubuntu1.3.dsc' subversion_1.9.3-2ubuntu1.3.dsc 3287 SHA512:7fa279007cd2cbac724c284842f09ae7629f1228c30ec23e52ec9151bcdadeaab6d8005b0124e3a114a2e76de86f83e7db14ea9cda3d31afaaf0ec34e8809e6c
'http://archive.ubuntu.com/ubuntu/pool/main/s/subversion/subversion_1.9.3.orig.tar.gz' subversion_1.9.3.orig.tar.gz 10600934 SHA512:999698ca9ec67fc450b511c1a936d3565dfbe4db1d05d110a4e11fdec3e0aefafa6669593f06502df42de8cc87610375844cf9aad691514e9bf1a71757b16552
'http://archive.ubuntu.com/ubuntu/pool/main/s/subversion/subversion_1.9.3-2ubuntu1.3.diff.gz' subversion_1.9.3-2ubuntu1.3.diff.gz 2434888 SHA512:8edc6185f5093ffc84c68a0593c01a1d9d7d8bf0705ce5a7a176b05ef36816050843d843630fdc9c91511de51474d119014660e107feb6e79d702108cd63a400
```

### `dpkg` source package: `sudo=1.8.16-0ubuntu1.9`

Binary Packages:

- `sudo=1.8.16-0ubuntu1.9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris sudo=1.8.16-0ubuntu1.9
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.16-0ubuntu1.9.dsc' sudo_1.8.16-0ubuntu1.9.dsc 2106 SHA512:7b1050f64f163686c2ea906ca5af5ab4adef815cf35ac83a7f7b4f9e4513f183f7e3185509e0616151200ca8e45e4942fa2e4fdd31962b151e5a10a9e63f0349
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.16.orig.tar.gz' sudo_1.8.16.orig.tar.gz 2707358 SHA512:7cf5399eb65c4b39071213c27c34d35ed2ea9c4578f19f6e8d3777179914fa30a2848c042e9f85e90e3b5d056322b9eb6c79e2d3b9b210a795e9921a1b00200b
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.16-0ubuntu1.9.debian.tar.xz' sudo_1.8.16-0ubuntu1.9.debian.tar.xz 42552 SHA512:70e93b519e3d66144f2c9c014ebcebdd2b9efc55954bd7a57bae9b9e0fd7a7b4d2c84d16a83b6b4739a473b80621021bd9f790aec5a7a1c80b16c6164acdd4cd
```

### `dpkg` source package: `systemd=229-4ubuntu21.29`

Binary Packages:

- `libsystemd0:amd64=229-4ubuntu21.29`
- `libudev1:amd64=229-4ubuntu21.29`
- `systemd=229-4ubuntu21.29`
- `systemd-sysv=229-4ubuntu21.29`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`, `/usr/share/doc/systemd/copyright`, `/usr/share/doc/systemd-sysv/copyright`)

- `CC0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=229-4ubuntu21.29
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229-4ubuntu21.29.dsc' systemd_229-4ubuntu21.29.dsc 4610 SHA512:4de075f03abef6b07064b3cf84aa5bd03a0f694f5d6e00420463d8c8e5b824d296896d132c1f4ff1541d367a039f2f4a7092df6867a3a2ad0106dccf21228aae
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229.orig.tar.gz' systemd_229.orig.tar.gz 4319173 SHA512:d692c0c9fc82f2fce64a5ec1caa4a0f8cf9edaeb1bdaaa1c462669db8f78b3dd6b33c87ef926ff21823582d0460f7b63aa3755792f9ae2cd6fb813ba08a35c39
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229-4ubuntu21.29.debian.tar.xz' systemd_229-4ubuntu21.29.debian.tar.xz 315232 SHA512:bf59936c22343bf236c49993b41ea1cbb03b4a50d4cb8e04a3d986c0045eef5aaea07d66a5f3bcedf08ea27674d8df67d3a048d27c7c973436ee44a9b3f6f434
```

### `dpkg` source package: `sysvinit=2.88dsf-59.3ubuntu2`

Binary Packages:

- `initscripts=2.88dsf-59.3ubuntu2`
- `sysv-rc=2.88dsf-59.3ubuntu2`
- `sysvinit-utils=2.88dsf-59.3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/initscripts/copyright`, `/usr/share/doc/sysv-rc/copyright`, `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.3ubuntu2.dsc' sysvinit_2.88dsf-59.3ubuntu2.dsc 2284 SHA256:a64f0c2c11c14c8bf57fee7c583ae38ea710ec3288c3d840daeeec5a2eab1676
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.3ubuntu2.debian.tar.xz' sysvinit_2.88dsf-59.3ubuntu2.debian.tar.xz 134864 SHA256:d4cf7aa3d6c1f8727cbd699395053d541844a9ff02ea5e6a1119eb90604586b8
```

### `dpkg` source package: `tar=1.28-2.1ubuntu0.1`

Binary Packages:

- `tar=1.28-2.1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.28-2.1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.28-2.1ubuntu0.1.dsc' tar_1.28-2.1ubuntu0.1.dsc 2025 SHA512:8684a8b31fe8068e852f3cddaf58906b7cbff7bae57d949ed5c74e4f57ba346527e10eaa82ca590d4f14d8265a98f8621e0d64608ea6eee805812ae822582e45
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.28.orig.tar.xz' tar_1.28.orig.tar.xz 1756440 SHA512:dc91045b84bf5df513ae936be14977b029644a77ac03f58d21d34e61e50d8069f95526b9e706f2da7d41d3d0ed7de88bf13c2c066e63a80e5651a24077e604c2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.28-2.1ubuntu0.1.debian.tar.xz' tar_1.28-2.1ubuntu0.1.debian.tar.xz 36868 SHA512:17c96a2fec2c40c92f4f28a5c054811b8a6623cf5c5f6eb7b1f782fb41a1f5e6f516a38fae96dee8b4250acbe0f4dd162801406fcc495a0ffcf1a7257e1206dd
```

### `dpkg` source package: `tiff=4.0.6-1ubuntu0.7`

Binary Packages:

- `libtiff5:amd64=4.0.6-1ubuntu0.7`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.6-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6-1ubuntu0.7.dsc' tiff_4.0.6-1ubuntu0.7.dsc 2399 SHA512:4e81b6c50f1e84e1a58e034c92f2acaacdb916ac169987c190725b0774b47757bc490b2dd810cf2b479ca882662ee6dee2c9f679c06606310934eb79b0c26e4b
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6.orig.tar.gz' tiff_4.0.6.orig.tar.gz 2192991 SHA512:2c8dbaaaab9f82a7722bfe8cb6fcfcf67472beb692f1b7dafaf322759e7016dad1bc58457c0f03db50aa5bd088fef2b37358fcbc1524e20e9e14a9620373fdf8
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6-1ubuntu0.7.debian.tar.xz' tiff_4.0.6-1ubuntu0.7.debian.tar.xz 63940 SHA512:ca2b3fc10697d4254854308d084c1a90d39a2fed4784457189edde377abc98f2fca001d73d25a38963153ff95e96403135bb6c4e3ff1facb7c142d00b17cde05
```

### `dpkg` source package: `tinyxml2=2.2.0-1.1ubuntu1`

Binary Packages:

- `libtinyxml2-2v5:amd64=2.2.0-1.1ubuntu1`
- `libtinyxml2-dev:amd64=2.2.0-1.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libtinyxml2-2v5/copyright`, `/usr/share/doc/libtinyxml2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris tinyxml2=2.2.0-1.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_2.2.0-1.1ubuntu1.dsc' tinyxml2_2.2.0-1.1ubuntu1.dsc 1968 SHA256:5ccede2b8baeb174c4fcc24e0555c9f229bb832cc5bc6bbb8477e2fb15bcb3fa
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_2.2.0.orig.tar.gz' tinyxml2_2.2.0.orig.tar.gz 455226 SHA256:f891224f32e7a06bf279290619cec80cc8ddc335c13696872195ffb87f5bce67
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_2.2.0-1.1ubuntu1.debian.tar.xz' tinyxml2_2.2.0-1.1ubuntu1.debian.tar.xz 4896 SHA256:2e2ecb4f405be569a5fb55f2494d625d43e65b2ff620e751ace79fb0f1df6160
```

### `dpkg` source package: `tinyxml=2.6.2-3`

Binary Packages:

- `libtinyxml-dev:amd64=2.6.2-3`
- `libtinyxml2.6.2v5:amd64=2.6.2-3`

Licenses: (parsed from: `/usr/share/doc/libtinyxml-dev/copyright`, `/usr/share/doc/libtinyxml2.6.2v5/copyright`)

- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris tinyxml=2.6.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/t/tinyxml/tinyxml_2.6.2-3.dsc' tinyxml_2.6.2-3.dsc 2059 SHA256:0299e682a6e38511f180e5f0ecab4372236574bec0b8b07f25534780361098ea
'http://archive.ubuntu.com/ubuntu/pool/main/t/tinyxml/tinyxml_2.6.2.orig.tar.gz' tinyxml_2.6.2.orig.tar.gz 210124 SHA256:15bdfdcec58a7da30adc87ac2b078e4417dbe5392f3afb719f9ba6d062645593
'http://archive.ubuntu.com/ubuntu/pool/main/t/tinyxml/tinyxml_2.6.2-3.debian.tar.xz' tinyxml_2.6.2-3.debian.tar.xz 4152 SHA256:f592529ece8b36a0ae2bacfb9d13ebb67ee3d4409af10c92f7bb9f73f3ba1423
```

### `dpkg` source package: `tzdata=2020a-0ubuntu0.16.04`

Binary Packages:

- `tzdata=2020a-0ubuntu0.16.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2020a-0ubuntu0.16.04
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.16.04.dsc' tzdata_2020a-0ubuntu0.16.04.dsc 2377 SHA512:7684916ec2917a30fb435a3c24cae92bccd97ffc14c31464eb54557d0faccf2f6e43694394cdebdabda705efd999bedd018c889b4b97af6164731515434d4392
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz' tzdata_2020a.orig.tar.gz 397245 SHA512:2a2fc2e3ad8a6e4c574242296c847ad582c2c1d86add9c556e65c812d19b9528522e3c4dddb5239017091825d2acc5a2ccaf21dc41b900b6c300ef4264cc5a9d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz.asc' tzdata_2020a.orig.tar.gz.asc 833 SHA512:54c6539c4ed78f5ab8006f0a6ad99911a7002e742b185119bb3c77ba7c637777b2c7dce9867e16fd58088ad3f9d062d74c03f80e3225a599a3fc28581d87e366
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.16.04.debian.tar.xz' tzdata_2020a-0ubuntu0.16.04.debian.tar.xz 100504 SHA512:0556fb8547df913bec565fad4b6386e284761f29502bd992d85764c650e91af58a35bad79c7ed445514a7cfa18b0e8c39d5bf6b3d4271c361cd53a177a135e6c
```

### `dpkg` source package: `ubuntu-keyring=2012.05.19.1`

Binary Packages:

- `ubuntu-keyring=2012.05.19.1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2012.05.19.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2012.05.19.1.dsc' ubuntu-keyring_2012.05.19.1.dsc 1505 SHA512:42d1e29ed8de0f37c17ccf2284e11a465dd42f9bcda222991696f0b41ab0cf57e0b6d09b2ccf377c6f578c0527bdc4fbd3c1caf1ddb8f9ad3da9406d27fe5f92
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2012.05.19.1.tar.gz' ubuntu-keyring_2012.05.19.1.tar.gz 21072 SHA512:62a9e816ef2a5f882f0974e940b15240aecdcf556d5a84c250fbe7c82dadd2154e22a0c3799bac832aa53f9782062d8433f1a8f3d1e407471d7292a315a59351
```

### `dpkg` source package: `ucf=3.0036`

Binary Packages:

- `ucf=3.0036`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0036
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0036.dsc' ucf_3.0036.dsc 1343 SHA256:e67a8a3012ac357c7759dabd93d258422b1003bad8c3f17f25fc2a289eeda3bb
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0036.tar.xz' ucf_3.0036.tar.xz 65020 SHA256:34aa44416106f1205376918386b2896edf21dd42b633133b5f8fedecae17fca8
```

### `dpkg` source package: `unixodbc=2.3.1-4.1`

Binary Packages:

- `libodbc1:amd64=2.3.1-4.1`

Licenses: (parsed from: `/usr/share/doc/libodbc1/copyright`)

- `GPL`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris unixodbc=2.3.1-4.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.1-4.1.dsc' unixodbc_2.3.1-4.1.dsc 2124 SHA256:e48ae9b7711b9bf5d2a486b1fa393f4efc4c6e5c50847af94b7d5e3b000c99fc
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.1.orig.tar.gz' unixodbc_2.3.1.orig.tar.gz 1813380 SHA256:1f5be3edecff9e31072ef738ea1d8019594c4f0c2e3ab427e6eef153491db6a2
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.1-4.1.diff.gz' unixodbc_2.3.1-4.1.diff.gz 384817 SHA256:a82169101ead03fb39365677d4419a26de21560eecb70c8107280daae49d3c3e
```

### `dpkg` source package: `ustr=1.0.4-5`

Binary Packages:

- `libustr-1.0-1:amd64=1.0.4-5`

Licenses: (parsed from: `/usr/share/doc/libustr-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris ustr=1.0.4-5
'http://archive.ubuntu.com/ubuntu/pool/main/u/ustr/ustr_1.0.4-5.dsc' ustr_1.0.4-5.dsc 2016 SHA256:3c06f54e4c05e76bf7c4d7192bbf3a7b259372c7448a4245e8317115808cf7c9
'http://archive.ubuntu.com/ubuntu/pool/main/u/ustr/ustr_1.0.4.orig.tar.gz' ustr_1.0.4.orig.tar.gz 301345 SHA256:4d293b6b9d9fe51d58441f4b09b1f0005fcad8256ae8048587789bf5dbefb62e
'http://archive.ubuntu.com/ubuntu/pool/main/u/ustr/ustr_1.0.4-5.debian.tar.xz' ustr_1.0.4-5.debian.tar.xz 24948 SHA256:a21e78acf82dcccef2893932ef7b85852419bfd9b18382e63c34e7710c1d7762
```

### `dpkg` source package: `util-linux=2.27.1-6ubuntu3.10`

Binary Packages:

- `bsdutils=1:2.27.1-6ubuntu3.10`
- `libblkid1:amd64=2.27.1-6ubuntu3.10`
- `libfdisk1:amd64=2.27.1-6ubuntu3.10`
- `libmount1:amd64=2.27.1-6ubuntu3.10`
- `libsmartcols1:amd64=2.27.1-6ubuntu3.10`
- `libuuid1:amd64=2.27.1-6ubuntu3.10`
- `mount=2.27.1-6ubuntu3.10`
- `util-linux=2.27.1-6ubuntu3.10`
- `uuid-dev:amd64=2.27.1-6ubuntu3.10`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.27.1-6ubuntu3.10
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1-6ubuntu3.10.dsc' util-linux_2.27.1-6ubuntu3.10.dsc 3960 SHA512:e715cf0d8eb23bc832a860c2f25541082fc97e026518bc7ae7924003801173d6547a53c04fcff64efaa73ac8ea64ca4c76dc15c8c35f299d87f6b3016e84bc7a
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1.orig.tar.xz' util-linux_2.27.1.orig.tar.xz 3964512 SHA512:a450a0c2d26a6deaf5e53b8f6bddf59409aefb1f0aaf07393f68a418408fbc62c5da353c8ba53c7cac8ea6e3dddfad59161753d888c31f5ccea445e81accbad8
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1-6ubuntu3.10.debian.tar.xz' util-linux_2.27.1-6ubuntu3.10.debian.tar.xz 89428 SHA512:649416382fee72ba67cbf251b3234918f12d6ec530aabbfe8c9c4ab040c70428dcacf89dfdc4d2a0eee463a66e4ae73a3f8706307e23b7edb77968408cd632fb
```

### `dpkg` source package: `wxpython3.0=3.0.2.0+dfsg-1build1`

Binary Packages:

- `python-wxgtk3.0=3.0.2.0+dfsg-1build1`
- `python-wxtools=3.0.2.0+dfsg-1build1`
- `python-wxversion=3.0.2.0+dfsg-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris wxpython3.0=3.0.2.0+dfsg-1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/w/wxpython3.0/wxpython3.0_3.0.2.0+dfsg-1build1.dsc' wxpython3.0_3.0.2.0+dfsg-1build1.dsc 2403 SHA256:c71a920a5a3346c0a0fd4238641905ddc2517e0bc3904ee949c5f130b622dbac
'http://archive.ubuntu.com/ubuntu/pool/universe/w/wxpython3.0/wxpython3.0_3.0.2.0+dfsg.orig.tar.xz' wxpython3.0_3.0.2.0+dfsg.orig.tar.xz 28961444 SHA256:c3e2f622ac449c535cf3a6261d30f052e4fba11bdcc145897038bf1b2c50708e
'http://archive.ubuntu.com/ubuntu/pool/universe/w/wxpython3.0/wxpython3.0_3.0.2.0+dfsg-1build1.debian.tar.xz' wxpython3.0_3.0.2.0+dfsg-1build1.debian.tar.xz 32980 SHA256:7d642d34cba620875eb7b8195056aaff73fef7ebe2bbecbc2faa89d99e42259f
```

### `dpkg` source package: `wxwidgets3.0=3.0.2+dfsg-1.3ubuntu0.1`

Binary Packages:

- `libwxbase3.0-0v5:amd64=3.0.2+dfsg-1.3ubuntu0.1`
- `libwxgtk3.0-0v5:amd64=3.0.2+dfsg-1.3ubuntu0.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris wxwidgets3.0=3.0.2+dfsg-1.3ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/universe/w/wxwidgets3.0/wxwidgets3.0_3.0.2+dfsg-1.3ubuntu0.1.dsc' wxwidgets3.0_3.0.2+dfsg-1.3ubuntu0.1.dsc 3539 SHA512:aca218743c48156e8dc2b3e08da3d550e59eb1238fd2055b11224b75e38353102a91cb94cef63208c27e208dcada283d8cd782a7fb598e7c869ec07ddbf21671
'http://archive.ubuntu.com/ubuntu/pool/universe/w/wxwidgets3.0/wxwidgets3.0_3.0.2+dfsg.orig.tar.xz' wxwidgets3.0_3.0.2+dfsg.orig.tar.xz 12883376 SHA512:d42a82c96ca443660c5103319da86881bb9ca271773baa169d511b44b1cf52ad8092156cdcdf5f6ad545da5b9ba9b5fb79e2b75f2ce1e5d8082384701d15532f
'http://archive.ubuntu.com/ubuntu/pool/universe/w/wxwidgets3.0/wxwidgets3.0_3.0.2+dfsg-1.3ubuntu0.1.debian.tar.xz' wxwidgets3.0_3.0.2+dfsg-1.3ubuntu0.1.debian.tar.xz 48096 SHA512:19f346c79dc86dfc7d4eaae1eadee76a5a8763d1134ef27c256aa80dd962df5a398f1e485c8e7333eef8c4b5bc3208c2e95e1ada8e1fd3692c9fdc70cfe08768
```

### `dpkg` source package: `xml-core=0.13+nmu2`

Binary Packages:

- `xml-core=0.13+nmu2`

Licenses: (parsed from: `/usr/share/doc/xml-core/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xml-core=0.13+nmu2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.13+nmu2.dsc' xml-core_0.13+nmu2.dsc 1738 SHA256:edf913f3aee9865480143bdd91f5f6a0838ca61ddc8674ea316e48a22d65fecb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.13+nmu2.tar.gz' xml-core_0.13+nmu2.tar.gz 23436 SHA256:cd3f5402265a9ab0e7e4a6efafdc5eb9cb02d33c3e75d1ff1ecb0ac0899e242b
```

### `dpkg` source package: `xorg=1:7.7+13ubuntu3.1`

Binary Packages:

- `x11-common=1:7.7+13ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+13ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+13ubuntu3.1.dsc' xorg_7.7+13ubuntu3.1.dsc 2112 SHA512:f44f01592aa31bd39e8ba2bf895b4a2aba8d6e459bd366efcd42832265432dc9e4971a65b33a00018ff18398eb12a464b1fd24bbce12ad288afa07774a6a8220
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+13ubuntu3.1.tar.gz' xorg_7.7+13ubuntu3.1.tar.gz 289897 SHA512:23b97e0aef38e353c595ff2dc8277bafa79d7faf41613743989170d8d6d10aa06f365ff804f459b903428ec047f4c0ac9e2e879ba8cd4567f0baf70e7bccc823
```

### `dpkg` source package: `xz-utils=5.1.1alpha+20120614-2ubuntu2`

Binary Packages:

- `liblzma5:amd64=5.1.1alpha+20120614-2ubuntu2`
- `xz-utils=5.1.1alpha+20120614-2ubuntu2`

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
$ apt-get source -qq --print-uris xz-utils=5.1.1alpha+20120614-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2ubuntu2.dsc' xz-utils_5.1.1alpha+20120614-2ubuntu2.dsc 2409 SHA256:0a8cb3d928d1327f70b998b713c10afd9cd064056f5973d48075cd3d0f7872ca
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614.orig.tar.gz' xz-utils_5.1.1alpha+20120614.orig.tar.gz 556454 SHA256:b168e63400db449a6e7b3a06e668f557ca27e3d70accbd29d2b5a98e15c00fee
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2ubuntu2.debian.tar.gz' xz-utils_5.1.1alpha+20120614-2ubuntu2.debian.tar.gz 156001 SHA256:e7743d4a96276ccffc4e171812e402a1f503f87df3b668ef0e58db6629146a18
```

### `dpkg` source package: `zlib=1:1.2.8.dfsg-2ubuntu4.3`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-2ubuntu4.3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.8.dfsg-2ubuntu4.3
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.8.dfsg-2ubuntu4.3.dsc' zlib_1.2.8.dfsg-2ubuntu4.3.dsc 2535 SHA512:c4c661746b4883b35d3e8c54d1f0203a4487e76c15839f558c930b600d8716b0e8357e3452988b90c0eb99fbc0a6451dad3521cca8777dfbdb5df3fc78ad2951
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.8.dfsg.orig.tar.gz' zlib_1.2.8.dfsg.orig.tar.gz 361943 SHA512:a6abfd2d2d65ed711f82dccd75f366f491f7c53a0f5f8fb76d77e629f86a8de28fd19028b8d76ee7d8ab2eb2d5789698402104d42b8ef000dfe362af2d7c3fab
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.8.dfsg-2ubuntu4.3.debian.tar.xz' zlib_1.2.8.dfsg-2ubuntu4.3.debian.tar.xz 19128 SHA512:c0472b7614851e7e4c8905847da63bd13a9f8ec46a9746ded69cee62994061d2ae028d2b6413b70dd993cb99fc5c9db519411aa1539048de17e1c8a482b6d062
```
