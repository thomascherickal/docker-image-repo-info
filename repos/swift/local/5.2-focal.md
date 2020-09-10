# `swift:5.2.5-focal`

## Docker Metadata

- Image ID: `sha256:2783a09518908ae5cb89647a1c6fa73889008bb73eed34576d1671ef4605b322`
- Created: `2020-08-20T01:20:51.353291228Z`
- Virtual Size: ~ 1.58 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `SWIFT_SIGNING_KEY=A62AE125BBBFBB96A6E042EC925CC1CCED3D1561`
  - `SWIFT_PLATFORM=ubuntu20.04`
  - `SWIFT_BRANCH=swift-5.2.5-release`
  - `SWIFT_VERSION=swift-5.2.5-RELEASE`
  - `SWIFT_WEBROOT=https://swift.org/builds/`
- Labels:
  - `description=Docker Container for the Swift programming language`
  - `maintainer=Swift Infrastructure <swift-infrastructure@swift.org>`

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
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.0.2ubuntu0.1.dsc' apt_2.0.2ubuntu0.1.dsc 2542 SHA256:db278b3b0a049a284a653013b282a8eefe06c3d970c1c21a3d47d4b501b3dc55
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.0.2ubuntu0.1.tar.xz' apt_2.0.2ubuntu0.1.tar.xz 2169516 SHA256:5e4ac597e285088a44ec12a7e013ccc174b1653f1863da6354eee0a53aa519c0
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

### `dpkg` source package: `base-files=11ubuntu5.1`

Binary Packages:

- `base-files=11ubuntu5.1`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu1.1.dsc' bash_5.0-6ubuntu1.1.dsc 2418 SHA256:6ed4321c4a335f34ec05103e336c1b2ef3ef980b1d9bd36aa3b8610a01ff9389
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA256:893858ba233d65bda38039e99dd96a4102b2f6a2d5e6c1c546e0794a60beed97
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu1.1.debian.tar.xz' bash_5.0-6ubuntu1.1.debian.tar.xz 74356 SHA256:b2208096205b625756e2a211d69cb801a273443094c273a275af9c49916911b6
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

### `dpkg` source package: `bzip2=1.0.8-2`

Binary Packages:

- `bzip2=1.0.8-2`
- `libbz2-1.0:amd64=1.0.8-2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110ubuntu1.1.dsc' ca-certificates_20190110ubuntu1.1.dsc 1921 SHA256:d72b01f57c872d4db413c851a8acaf0f0393520c45489dfca18fa5e6f52095c2
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110ubuntu1.1.tar.xz' ca-certificates_20190110ubuntu1.1.tar.xz 243736 SHA256:fc7e6b238b3838d1af74773ffb0a155c9583269a5c1b498fac0870ddfe904da3
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

- `libcurl3-gnutls:amd64=7.68.0-1ubuntu2.2`
- `libcurl4:amd64=7.68.0-1ubuntu2.2`

Licenses: (parsed from: `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.68.0-1ubuntu2.2
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu2.2.dsc' curl_7.68.0-1ubuntu2.2.dsc 2733 SHA256:7d00c4b9ad285d449cc101cf2bd0f5c8d14e6d08d16c8e6c5013bd8fd8b292ab
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0.orig.tar.gz' curl_7.68.0.orig.tar.gz 4096350 SHA256:1dd7604e418b0b9a9077f62f763f6684c1b092a7bc17e3f354b8ad5c964d7358
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu2.2.debian.tar.xz' curl_7.68.0-1ubuntu2.2.debian.tar.xz 34624 SHA256:713b79597c36ae16d1d1618cca60a0cf6de2bbd280151087e89cfbd9a4a826d5
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2`
- `libsasl2-modules:amd64=2.1.27+dfsg-2`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

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

### `dpkg` source package: `dpkg=1.19.7ubuntu3`

Binary Packages:

- `dpkg=1.19.7ubuntu3`
- `libdpkg-perl=1.19.7ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

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

### `dpkg` source package: `expat=2.2.9-1build1`

Binary Packages:

- `libexpat1:amd64=2.2.9-1build1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.9-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.dsc' expat_2.2.9-1build1.dsc 1998 SHA256:9f2d2e3bf2aec22907e3bf818fac7acc5f1e917821907bdea016f69a5cfe4da0
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9.orig.tar.gz' expat_2.2.9.orig.tar.gz 8273174 SHA256:c341ac8c79e021cc3392a6d76e138e62d1dd287592cb455148540331756a2208
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.debian.tar.xz' expat_2.2.9-1build1.debian.tar.xz 10780 SHA256:400872937adfb41255914391a172237cfe317e57f129562ff2ec66773b2b5bbf
```

### `dpkg` source package: `file=1:5.38-4`

Binary Packages:

- `file=1:5.38-4`
- `libmagic-mgc=1:5.38-4`
- `libmagic1:amd64=1:5.38-4`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.38-4
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38-4.dsc' file_5.38-4.dsc 2237 SHA256:d84b2734b112384230e3678beb1c8c5d3a17d4cdec8b6ef21304f2c0b72fda26
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38.orig.tar.gz' file_5.38.orig.tar.gz 932528 SHA256:593c2ffc2ab349c5aea0f55fedfe4d681737b6b62376a9b3ad1e77b2cc19fa34
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38.orig.tar.gz.asc' file_5.38.orig.tar.gz.asc 169 SHA256:b9c78e39970abda091ec8752401f5241349cef4709a2e1267a378f7ab25115d8
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38-4.debian.tar.xz' file_5.38-4.debian.tar.xz 34488 SHA256:b9dfd0dd070ee17a6cc69ecf4d61c329b3f567ca16fdc121f3b31d0111df9381
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
- `libgcc-s1:amd64=10-20200411-0ubuntu1`
- `libgomp1:amd64=10-20200411-0ubuntu1`
- `libitm1:amd64=10-20200411-0ubuntu1`
- `liblsan0:amd64=10-20200411-0ubuntu1`
- `libquadmath0:amd64=10-20200411-0ubuntu1`
- `libstdc++6:amd64=10-20200411-0ubuntu1`
- `libtsan0:amd64=10-20200411-0ubuntu1`
- `libubsan1:amd64=10-20200411-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

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

### `dpkg` source package: `gcc-9=9.3.0-10ubuntu2`

Binary Packages:

- `gcc-9-base:amd64=9.3.0-10ubuntu2`
- `libasan5:amd64=9.3.0-10ubuntu2`
- `libgcc-9-dev:amd64=9.3.0-10ubuntu2`
- `libstdc++-9-dev:amd64=9.3.0-10ubuntu2`

Licenses: (parsed from: `/usr/share/doc/gcc-9-base/copyright`, `/usr/share/doc/libasan5/copyright`, `/usr/share/doc/libgcc-9-dev/copyright`, `/usr/share/doc/libstdc++-9-dev/copyright`)

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

### `dpkg` source package: `git=1:2.25.1-1ubuntu3`

Binary Packages:

- `git=1:2.25.1-1ubuntu3`
- `git-man=1:2.25.1-1ubuntu3`

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
$ apt-get source -qq --print-uris git=1:2.25.1-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.25.1-1ubuntu3.dsc' git_2.25.1-1ubuntu3.dsc 2954 SHA256:7f47dc333299979e969f9b87a8cfd8926312e6bee01e44eef6d5a60c19bc7316
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.25.1.orig.tar.xz' git_2.25.1.orig.tar.xz 5875548 SHA256:222796cc6e3bf2f9fd765f8f097daa3c3999bb7865ac88a8c974d98182e29f26
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.25.1-1ubuntu3.debian.tar.xz' git_2.25.1-1ubuntu3.debian.tar.xz 650520 SHA256:384e8710d6136d7b0b2541cc950de8a0b9f8bc680cc7b889b059eb758b35792c
```

### `dpkg` source package: `glib2.0=2.64.3-1~ubuntu20.04.1`

Binary Packages:

- `libglib2.0-0:amd64=2.64.3-1~ubuntu20.04.1`
- `libglib2.0-data=2.64.3-1~ubuntu20.04.1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-data/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.64.3-1~ubuntu20.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.3-1~ubuntu20.04.1.dsc' glib2.0_2.64.3-1~ubuntu20.04.1.dsc 3256 SHA256:500313a354ec904281df5ac246cf92f66179a55a8ba693bf4aed322144c6d3e2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.3.orig.tar.xz' glib2.0_2.64.3.orig.tar.xz 4778964 SHA256:fe9cbc97925d14c804935f067a3ad77ef55c0bbe9befe68962318f5a767ceb22
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.3-1~ubuntu20.04.1.debian.tar.xz' glib2.0_2.64.3-1~ubuntu20.04.1.debian.tar.xz 91792 SHA256:1bd92474c85b7f500d6a27677e4d41cd81d447dc5cbcdce7124d5f493d0fbd3f
```

### `dpkg` source package: `glibc=2.31-0ubuntu9`

Binary Packages:

- `libc-bin=2.31-0ubuntu9`
- `libc-dev-bin=2.31-0ubuntu9`
- `libc6:amd64=2.31-0ubuntu9`
- `libc6-dev:amd64=2.31-0ubuntu9`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.31-0ubuntu9
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu9.dsc' glibc_2.31-0ubuntu9.dsc 9280 SHA256:be5c141ac961304c9c91218d7c49d0059f49895752720b1e58a834fb1d108bcd
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31.orig.tar.xz' glibc_2.31.orig.tar.xz 17317924 SHA256:2b22c7b04a36747d6c74796a73193a6f8856bfd1efc551b5db96baefa053fe5e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu9.debian.tar.xz' glibc_2.31-0ubuntu9.debian.tar.xz 840996 SHA256:63c9cb78c131faec608ba47cfd2a15a9807ff6fcc41204a0429fa0c17b87b4d8
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

### `dpkg` source package: `gnutls28=3.6.13-2ubuntu1.2`

Binary Packages:

- `libgnutls30:amd64=3.6.13-2ubuntu1.2`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `icu=66.1-2ubuntu2`

Binary Packages:

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

- `krb5-locales=1.17-6ubuntu4`
- `libgssapi-krb5-2:amd64=1.17-6ubuntu4`
- `libk5crypto3:amd64=1.17-6ubuntu4`
- `libkrb5-3:amd64=1.17-6ubuntu4`
- `libkrb5support0:amd64=1.17-6ubuntu4`

Licenses: (parsed from: `/usr/share/doc/krb5-locales/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-6ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-6ubuntu4.dsc' krb5_1.17-6ubuntu4.dsc 3654 SHA256:e2e56f3faf968072ef89201a04e85cd59e003d123bd5a06e3a05f59a01c94301
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA256:5a6e2284a53de5702d3dc2be3b9339c963f9b5397d3fbbc53beb249380a781f5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-6ubuntu4.debian.tar.xz' krb5_1.17-6ubuntu4.debian.tar.xz 144560 SHA256:17d09fbe6a54de93fe2f21f1c384a55d0913862dec7ca96b2c0489266f3c16fd
```

### `dpkg` source package: `less=551-1ubuntu0.1`

Binary Packages:

- `less=551-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/less/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris less=551-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/less/less_551-1ubuntu0.1.dsc' less_551-1ubuntu0.1.dsc 1896 SHA256:1ad1cfcc490b5095a5adc5ecdf4f7523ffdfe4a13871b28486cfb153a9789a05
'http://archive.ubuntu.com/ubuntu/pool/main/l/less/less_551.orig.tar.gz' less_551.orig.tar.gz 347007 SHA256:ff165275859381a63f19135a8f1f6c5a194d53ec3187f94121ecd8ef0795fe3d
'http://archive.ubuntu.com/ubuntu/pool/main/l/less/less_551-1ubuntu0.1.debian.tar.xz' less_551-1ubuntu0.1.debian.tar.xz 18896 SHA256:c48389abace49b71514f3719b0567367e1d08d0c7429c536c12ec32dfcb01708
```

### `dpkg` source package: `libassuan=2.5.3-7ubuntu2`

Binary Packages:

- `libassuan0:amd64=2.5.3-7ubuntu2`

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

### `dpkg` source package: `liberror-perl=0.17029-1`

Binary Packages:

- `liberror-perl=0.17029-1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17029-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.dsc' liberror-perl_0.17029-1.dsc 2336 SHA256:0590467fe8c5f81bff9336e991462b2a9994b4876f4b732c8b8b31e927987cd7
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA256:1a23f7913032aed6d4b68321373a3899ca66590f4727391a091ec19c95bf7adc
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.debian.tar.xz' liberror-perl_0.17029-1.debian.tar.xz 4552 SHA256:a753b142c4c33ebf9cc98ae5f7a08da13b7c9ca2823ec26e45c96efb9c15c42e
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

### `dpkg` source package: `libfile-fcntllock-perl=0.22-3build4`

Binary Packages:

- `libfile-fcntllock-perl=0.22-3build4`

Licenses: (parsed from: `/usr/share/doc/libfile-fcntllock-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libfile-fcntllock-perl=0.22-3build4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-fcntllock-perl/libfile-fcntllock-perl_0.22-3build4.dsc' libfile-fcntllock-perl_0.22-3build4.dsc 2182 SHA256:13527148ee48099c8fb1286ed5ca7ce14cd6bc0be311b4ed64d3743ad2dc15cb
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-fcntllock-perl/libfile-fcntllock-perl_0.22.orig.tar.gz' libfile-fcntllock-perl_0.22.orig.tar.gz 16994 SHA256:9a9abb2efff93ab73741a128d3f700e525273546c15d04e7c51c704ab09dbcdf
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-fcntllock-perl/libfile-fcntllock-perl_0.22-3build4.debian.tar.xz' libfile-fcntllock-perl_0.22-3build4.debian.tar.xz 2624 SHA256:d041ccb595201ddbce307223c7ce9fe506e2ecf9ab952587c716b6d2b52eb5c7
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

- `libgpg-error0:amd64=1.37-1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

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

### `dpkg` source package: `liblocale-gettext-perl=1.07-4`

Binary Packages:

- `liblocale-gettext-perl=1.07-4`

Licenses: (parsed from: `/usr/share/doc/liblocale-gettext-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris liblocale-gettext-perl=1.07-4
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.07-4.dsc' liblocale-gettext-perl_1.07-4.dsc 2322 SHA256:6559edd2a7c4700b436dcdd6f2563c3f4721d47aecabe79c82eba949b4652603
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.07.orig.tar.gz' liblocale-gettext-perl_1.07.orig.tar.gz 8651 SHA256:909d47954697e7c04218f972915b787bd1244d75e3bd01620bc167d5bbc49c15
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.07-4.debian.tar.xz' liblocale-gettext-perl_1.07-4.debian.tar.xz 5336 SHA256:b6dc78d5f90f5f0efa5cb5a9e4ec7182cb6d557b567c477e33a310440b08c24e
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

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3.20.04.3`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3.20.04.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu3.20.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.20.04.3.dsc' libseccomp_2.4.3-1ubuntu3.20.04.3.dsc 2226 SHA256:6d1692ad720075c24d7c7beeaaaae041eac3df1963fbf90bde024171e05ec395
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA256:cf15d1421997fac45b936515af61d209c4fd788af11005d212b3d0fd71e7991d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.20.04.3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.20.04.3.debian.tar.xz 36444 SHA256:6231018b3d3e4fbb853a9f739fd6a76e67052d31362dfa3eefe774782baed7ce
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
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.3-2ubuntu2.1.dsc' libssh_0.9.3-2ubuntu2.1.dsc 2538 SHA256:978e0ac5e2a3ba50bdcfb5a8e4ef7e7bc1a4f407bf353a0450c53c43b302702c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.3.orig.tar.xz' libssh_0.9.3.orig.tar.xz 500068 SHA256:2c8b5f894dced58b3d629f16f3afa6562c20b4bdc894639163cf657833688f0c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.3-2ubuntu2.1.debian.tar.xz' libssh_0.9.3-2ubuntu2.1.debian.tar.xz 28488 SHA256:fb2383a264121d025854632311a8e3ae0d8a537278c32387b49b808e810f9405
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

### `dpkg` source package: `libx11=2:1.6.9-2ubuntu1`

Binary Packages:

- `libx11-6:amd64=2:1.6.9-2ubuntu1`
- `libx11-data=2:1.6.9-2ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.9-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9-2ubuntu1.dsc' libx11_1.6.9-2ubuntu1.dsc 2584 SHA256:e0d4ff552c8a2e0742bd01053d1abc8cfc8b32dc5302cd1fe90c524a91ae0999
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9.orig.tar.gz' libx11_1.6.9.orig.tar.gz 2994329 SHA256:b8c0930a9b25de15f3d773288cacd5e2f0a4158e194935615c52aeceafd1107b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9.orig.tar.gz.asc' libx11_1.6.9.orig.tar.gz.asc 659 SHA256:5dca08f1a18bcfd9aabbb9b61c78948180db4e0a3e6710df695a48badb1ea8df
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9-2ubuntu1.diff.gz' libx11_1.6.9-2ubuntu1.diff.gz 60547 SHA256:6af57abf40eabe9d1ddc09d70754ad473ef7b7edc898d88ca9069d9acbd60d9e
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

### `dpkg` source package: `libxmu=2:1.1.3-0ubuntu1`

Binary Packages:

- `libxmuu1:amd64=2:1.1.3-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxmu=2:1.1.3-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.3-0ubuntu1.dsc' libxmu_1.1.3-0ubuntu1.dsc 1797 SHA256:ba64fdbc1b602eac436ae7ea58f57d72a45ee23b016eba542ce8b704508f717c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.3.orig.tar.gz' libxmu_1.1.3.orig.tar.gz 497343 SHA256:5bd9d4ed1ceaac9ea023d86bf1c1632cd3b172dce4a193a72a94e1d9df87a62e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.3-0ubuntu1.diff.gz' libxmu_1.1.3-0ubuntu1.diff.gz 6373 SHA256:7519cc7be957da29adc420426b57e1366228448c6205c5e4b89d04bfa948ffa7
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

### `dpkg` source package: `linux=5.4.0-42.46`

Binary Packages:

- `linux-libc-dev:amd64=5.4.0-42.46`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lsb=11.1.0ubuntu2`

Binary Packages:

- `lsb-base=11.1.0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

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

### `dpkg` source package: `manpages=5.05-1`

Binary Packages:

- `manpages=5.05-1`
- `manpages-dev=5.05-1`

Licenses: (parsed from: `/usr/share/doc/manpages/copyright`, `/usr/share/doc/manpages-dev/copyright`)

- `BSD-3-clause`
- `BSD-4-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LDPv1`
- `freely-redistributable`
- `henry-spencer-regex`
- `public-domain`
- `verbatim`

Source:

```console
$ apt-get source -qq --print-uris manpages=5.05-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/manpages/manpages_5.05-1.dsc' manpages_5.05-1.dsc 1882 SHA256:b6c7408cab682e8f38dd57850707f63098700e6362530ed7e4344f70f902d571
'http://archive.ubuntu.com/ubuntu/pool/main/m/manpages/manpages_5.05.orig.tar.xz' manpages_5.05.orig.tar.xz 1687960 SHA256:d5b135b1196d9258138610dbc47190d8b9ac9dee7f8ee6d9196f7fc6a036eb47
'http://archive.ubuntu.com/ubuntu/pool/main/m/manpages/manpages_5.05-1.debian.tar.xz' manpages_5.05-1.debian.tar.xz 76200 SHA256:f1ce4e0e2b16e3666931b0d02ecad7759ef3476ceedeb1772309e44bd19a62d0
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

### `dpkg` source package: `netbase=6.1`

Binary Packages:

- `netbase=6.1`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.dsc' netbase_6.1.dsc 1480 SHA256:d3d24cf00001259d3311c0509b4e23ac150cffea27b546e3a204864f52824556
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.tar.xz' netbase_6.1.tar.xz 31984 SHA256:084d743bd84d4d9380bac4c71c51e57406dce44f5a69289bb823c903e9b035d8
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

### `dpkg` source package: `openldap=2.4.49+dfsg-2ubuntu1.3`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.49+dfsg-2ubuntu1.3`
- `libldap-common=2.4.49+dfsg-2ubuntu1.3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.49+dfsg-2ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.49+dfsg-2ubuntu1.3.dsc' openldap_2.4.49+dfsg-2ubuntu1.3.dsc 3136 SHA256:ea972b78e05fccb356e64846fb9a8522b16a4a616ca9c7f61231517f057dee97
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.49+dfsg.orig.tar.gz' openldap_2.4.49+dfsg.orig.tar.gz 4844726 SHA256:240022395b438f327aa860a631c1d4eef9b17e63ec8965d3aca2aa983e6d81e6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.49+dfsg-2ubuntu1.3.debian.tar.xz' openldap_2.4.49+dfsg-2ubuntu1.3.debian.tar.xz 182112 SHA256:56f7c59b4585508dc2dbd24b7c9b7ff7662792a3ed97a0db48b79388c48e8670
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
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.2p1-4ubuntu0.1.dsc' openssh_8.2p1-4ubuntu0.1.dsc 3098 SHA256:f3516ad35e15ff7aff40210f6cc47603ae939e85bf7c56c16740ad6c177e3490
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.2p1.orig.tar.gz' openssh_8.2p1.orig.tar.gz 1701197 SHA256:43925151e6cf6cee1450190c0e9af4dc36b41c12737619edff8bcebdff64e671
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.2p1-4ubuntu0.1.debian.tar.xz' openssh_8.2p1-4ubuntu0.1.debian.tar.xz 174784 SHA256:799e59e8913c2cae5412233a570e9d52cbd907b7335a6981074f8863f522b04f
```

### `dpkg` source package: `openssl=1.1.1f-1ubuntu2`

Binary Packages:

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

### `dpkg` source package: `pam=1.3.1-5ubuntu4`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu4`
- `libpam-modules-bin=1.3.1-5ubuntu4`
- `libpam-runtime=1.3.1-5ubuntu4`
- `libpam0g:amd64=1.3.1-5ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu4.dsc' pam_1.3.1-5ubuntu4.dsc 2699 SHA256:b0d51a23352d570209f00156b796e685cee249dfcc36872154de0138f0b27e4b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA256:eff47a4ecd833fbf18de9686632a70ee8d0794b79aecb217ebd0ce11db4cd0db
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu4.debian.tar.xz' pam_1.3.1-5ubuntu4.debian.tar.xz 159780 SHA256:d5c539ac0bb5d05b62a2e9f936145d1cc8dbf94a91e0268e7ae98f043dbe8b0b
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

- `libpcre3:amd64=2:8.39-12build1`

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

### `dpkg` source package: `publicsuffix=20200303.0012-1`

Binary Packages:

- `publicsuffix=20200303.0012-1`

Licenses: (parsed from: `/usr/share/doc/publicsuffix/copyright`)

- `CC0`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris publicsuffix=20200303.0012-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/publicsuffix/publicsuffix_20200303.0012-1.dsc' publicsuffix_20200303.0012-1.dsc 1406 SHA256:ada2841021e758d6ebb15063d3caf243f545b01b5edf6adf65ecdf187fa2493c
'http://archive.ubuntu.com/ubuntu/pool/main/p/publicsuffix/publicsuffix_20200303.0012.orig.tar.gz' publicsuffix_20200303.0012.orig.tar.gz 94164 SHA256:048bf6efaf055c4cfed1c79b204f4c1f8f2d1f66ad0424979a227f43ef8df243
'http://archive.ubuntu.com/ubuntu/pool/main/p/publicsuffix/publicsuffix_20200303.0012-1.debian.tar.xz' publicsuffix_20200303.0012-1.debian.tar.xz 15328 SHA256:3dbbd7b1e20bafc3e5ad73732cb026a4b8e6e5dafa25a9047151e9a28b251647
```

### `dpkg` source package: `python2.7=2.7.18~rc1-2`

Binary Packages:

- `libpython2.7:amd64=2.7.18~rc1-2`
- `libpython2.7-minimal:amd64=2.7.18~rc1-2`
- `libpython2.7-stdlib:amd64=2.7.18~rc1-2`

Licenses: (parsed from: `/usr/share/doc/libpython2.7/copyright`, `/usr/share/doc/libpython2.7-minimal/copyright`, `/usr/share/doc/libpython2.7-stdlib/copyright`)

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
$ apt-get source -qq --print-uris python2.7=2.7.18~rc1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.18~rc1-2.dsc' python2.7_2.7.18~rc1-2.dsc 3318 SHA256:edd6bb77243841b0e130ddf827bf05925bfaf5611b22a932c7cd0771e4572a94
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.18~rc1.orig.tar.gz' python2.7_2.7.18~rc1.orig.tar.gz 17538275 SHA256:fb8f47668ccb2ab22d8b1f72e0ca9b0022eeafce5b3fe8c422ab935cba62ff3d
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.18~rc1-2.diff.gz' python2.7_2.7.18~rc1-2.diff.gz 286573 SHA256:0de99970280590fe68622cd7ffe16df8e68e8962cefc241285fc8965bdedd7dc
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

### `dpkg` source package: `shadow=1:4.8.1-1ubuntu5.20.04`

Binary Packages:

- `login=1:4.8.1-1ubuntu5.20.04`
- `passwd=1:4.8.1-1ubuntu5.20.04`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1ubuntu5.20.04
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu5.20.04.dsc' shadow_4.8.1-1ubuntu5.20.04.dsc 1729 SHA256:c72f775ec9bff0d88f805426d370e1b66b8bef2c8d3ff77af180987173245130
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA256:a3ad4630bdc41372f02a647278a8c3514844295d36eefe68ece6c3a641c1ae62
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu5.20.04.debian.tar.xz' shadow_4.8.1-1ubuntu5.20.04.debian.tar.xz 85640 SHA256:d930def27e0015314820151132e6635cff5297cef7540d0d64d25d63f8100773
```

### `dpkg` source package: `shared-mime-info=1.15-1`

Binary Packages:

- `shared-mime-info=1.15-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.15-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15-1.dsc' shared-mime-info_1.15-1.dsc 2198 SHA256:dca6ea0156110b4a2694dd96a721d34ad4f42b51f3d3a20d0d711b77bde5115d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15.orig.tar.xz' shared-mime-info_1.15.orig.tar.xz 772708 SHA256:f482b027437c99e53b81037a9843fccd549243fd52145d016e9c7174a4f5db90
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15-1.debian.tar.xz' shared-mime-info_1.15-1.debian.tar.xz 9728 SHA256:02c4fa8b2b3073c745287dd0e00c69c9f1ba028c7c6496105e3ecdcc02d9f1dd
```

### `dpkg` source package: `sqlite3=3.31.1-4ubuntu0.2`

Binary Packages:

- `libsqlite3-0:amd64=3.31.1-4ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.31.1-4ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1-4ubuntu0.2.dsc' sqlite3_3.31.1-4ubuntu0.2.dsc 2519 SHA256:f7da60b389f3bebbdeef048f599246b044471507330fba66fd749538b29a7428
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1.orig-www.tar.xz' sqlite3_3.31.1.orig-www.tar.xz 5764424 SHA256:cab01c285fad4eb08bd1e3659cde5a44e17e024badbe9ed01b2de9c625ed0831
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1.orig.tar.xz' sqlite3_3.31.1.orig.tar.xz 7108036 SHA256:dfa6eda312d391d33b7790b061f533d723dc5c30b60720ddd98c89a6fb29272f
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1-4ubuntu0.2.debian.tar.xz' sqlite3_3.31.1-4ubuntu0.2.debian.tar.xz 33492 SHA256:c21a01d084df0a1d6be1e29e420c462277213cbd082c3a49a8501c2f023e80c1
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
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.4-4ubuntu3.2.dsc' systemd_245.4-4ubuntu3.2.dsc 5291 SHA256:4403949784fe55c2f460be3515bac0c79b6df40c4d5e51e75a38f32efc1815ff
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.4.orig.tar.gz' systemd_245.4.orig.tar.gz 9000780 SHA256:bd1c467045989ab986b29d003f17960ccb201bc923093db978b4cfb299ae8a63
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.4-4ubuntu3.2.debian.tar.xz' systemd_245.4-4ubuntu3.2.debian.tar.xz 217140 SHA256:3fe613d3a2b30d714d777ecffb25e1a16fc14162de61d2ff70ea0e26b98af51b
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

### `dpkg` source package: `tzdata=2020a-0ubuntu0.20.04`

Binary Packages:

- `tzdata=2020a-0ubuntu0.20.04`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2020a-0ubuntu0.20.04
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.20.04.dsc' tzdata_2020a-0ubuntu0.20.04.dsc 2382 SHA256:e9e5e880bb214ae4bf343a4f312647f83e8f11aca7e5605075c1f22d19a8b0fc
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz' tzdata_2020a.orig.tar.gz 397245 SHA256:547161eca24d344e0b5f96aff6a76b454da295dc14ed4ca50c2355043fb899a2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz.asc' tzdata_2020a.orig.tar.gz.asc 833 SHA256:a92f085fe1e7f8bc0f0a0bc4432f27e6cf2d69e64d4a90958bd023eb0ccf45f9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.20.04.debian.tar.xz' tzdata_2020a-0ubuntu0.20.04.debian.tar.xz 164392 SHA256:e3f2be806b7c70908a89aac2c3d07d663bb3f0e96a3b7abf76802925bc8c5ffb
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

### `dpkg` source package: `util-linux=2.34-0.1ubuntu9`

Binary Packages:

- `bsdutils=1:2.34-0.1ubuntu9`
- `fdisk=2.34-0.1ubuntu9`
- `libblkid1:amd64=2.34-0.1ubuntu9`
- `libfdisk1:amd64=2.34-0.1ubuntu9`
- `libmount1:amd64=2.34-0.1ubuntu9`
- `libsmartcols1:amd64=2.34-0.1ubuntu9`
- `libuuid1:amd64=2.34-0.1ubuntu9`
- `mount=2.34-0.1ubuntu9`
- `util-linux=2.34-0.1ubuntu9`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.34-0.1ubuntu9
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu9.dsc' util-linux_2.34-0.1ubuntu9.dsc 3380 SHA256:d6afdba4e84e53a0e8bb153383173d2409de9ab2679d503a683ebcbaa972b225
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34.orig.tar.xz' util-linux_2.34.orig.tar.xz 4974812 SHA256:743f9d0c7252b6db246b659c1e1ce0bd45d8d4508b4dfa427bbb4a3e9b9f62b5
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu9.debian.tar.xz' util-linux_2.34-0.1ubuntu9.debian.tar.xz 90728 SHA256:23a6c2f493ad0b4600a4b0d0d75b9337a1f24735e5a02ddd8cbff4fd34b6c5d7
```

### `dpkg` source package: `xauth=1:1.1-0ubuntu1`

Binary Packages:

- `xauth=1:1.1-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xauth=1:1.1-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xauth/xauth_1.1-0ubuntu1.dsc' xauth_1.1-0ubuntu1.dsc 1359 SHA256:1e2528d5258ff18cf8939dd0b8b66448aee8cfeb327a15ef5a447bcab7d99d5c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xauth/xauth_1.1.orig.tar.gz' xauth_1.1.orig.tar.gz 204146 SHA256:e9fce796c8c5c9368594b9e8bbba237fb54b6615f5fd60e8d0a5b3c52a92c5ef
'http://archive.ubuntu.com/ubuntu/pool/main/x/xauth/xauth_1.1-0ubuntu1.diff.gz' xauth_1.1-0ubuntu1.diff.gz 7640 SHA256:56610712799d940bf8dc86c0408cb2a084cbea101a638d68445f32f8ac03114c
```

### `dpkg` source package: `xdg-user-dirs=0.17-2ubuntu1`

Binary Packages:

- `xdg-user-dirs=0.17-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/xdg-user-dirs/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xdg-user-dirs=0.17-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.17-2ubuntu1.dsc' xdg-user-dirs_0.17-2ubuntu1.dsc 1671 SHA256:47a6d5715554995558197b0a79735a3335d9ff248cef3db1e34cb8be286ffa23
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.17.orig.tar.gz' xdg-user-dirs_0.17.orig.tar.gz 257291 SHA256:2a07052823788e8614925c5a19ef5b968d8db734fdee656699ea4f97d132418c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.17-2ubuntu1.debian.tar.xz' xdg-user-dirs_0.17-2ubuntu1.debian.tar.xz 28704 SHA256:4883d7162a09f35c2640c25103c3a9914b916f13170ee63f873213823d6550fc
```

### `dpkg` source package: `xz-utils=5.2.4-1`

Binary Packages:

- `liblzma5:amd64=5.2.4-1`

Licenses: (parsed from: `/usr/share/doc/liblzma5/copyright`)

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
$ apt-get source -qq --print-uris xz-utils=5.2.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1.dsc' xz-utils_5.2.4-1.dsc 2518 SHA256:b1572c4efb3c8ebf6f0e044b70e1e0451c919a99d3f80be03b624a54dd7ea593
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA256:9717ae363760dedf573dad241420c5fea86256b65bc21d2cf71b2b12f0544f4b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA256:88290c1deeaf674ae2a4821f4373fe0e4cc2a94199eae6dcc26df1e70cc15303
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1.debian.tar.xz' xz-utils_5.2.4-1.debian.tar.xz 135296 SHA256:d37b558444b76e88a69601df008cf1c0343c58cb7765b7bbb2099b0a19619361
```

### `dpkg` source package: `xz-utils=5.2.4-1ubuntu1`

Binary Packages:

- `xz-utils=5.2.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/xz-utils/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.dsc' xz-utils_5.2.4-1ubuntu1.dsc 2629 SHA256:ef1afb534aae085f0f1265a0b282be3c839b97f5fd30ed652826aeb81b132724
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA256:9717ae363760dedf573dad241420c5fea86256b65bc21d2cf71b2b12f0544f4b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA256:88290c1deeaf674ae2a4821f4373fe0e4cc2a94199eae6dcc26df1e70cc15303
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.debian.tar.xz' xz-utils_5.2.4-1ubuntu1.debian.tar.xz 135512 SHA256:daaa79e97b131e18381c05ed3b7cb878acd6c6f7341779039d7a2af765f37627
```

### `dpkg` source package: `z3=4.8.7-4build1`

Binary Packages:

- `libz3-4:amd64=4.8.7-4build1`
- `libz3-dev:amd64=4.8.7-4build1`

Licenses: (parsed from: `/usr/share/doc/libz3-4/copyright`, `/usr/share/doc/libz3-dev/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris z3=4.8.7-4build1
'http://archive.ubuntu.com/ubuntu/pool/universe/z/z3/z3_4.8.7-4build1.dsc' z3_4.8.7-4build1.dsc 2594 SHA256:bbd775d6c9d8298e258ca1ba44aa179dc63857ff55be5c6af8250e3b9cb7e789
'http://archive.ubuntu.com/ubuntu/pool/universe/z/z3/z3_4.8.7.orig.tar.gz' z3_4.8.7.orig.tar.gz 4343720 SHA256:8c1c49a1eccf5d8b952dadadba3552b0eac67482b8a29eaad62aa7343a0732c3
'http://archive.ubuntu.com/ubuntu/pool/universe/z/z3/z3_4.8.7-4build1.debian.tar.xz' z3_4.8.7-4build1.debian.tar.xz 10080 SHA256:62269275955ed4d2cf9bfe5d1903e3f5bffd6981c7f14660d778365099ebe333
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
