# `buildpack-deps:trixie`

## Docker Metadata

- Image ID: `sha256:907c0f75ea1d81f1449afa092e16b57f12ebecbbfaba6b0dedb480d03ed40193`
- Created: `2023-11-21T10:00:09.874535882Z`
- Virtual Size: ~ 1.02 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.3.1-3`

Binary Packages:

- `libacl1:amd64=2.3.1-3`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.3.1-3
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-3.dsc' acl_2.3.1-3.dsc 2508 SHA256:7820eee88cce7244e0b8eb25cc4f51bdf10aff7a6c1a497f3d18c36bdce712cc
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz' acl_2.3.1.orig.tar.xz 355676 SHA256:c0234042e17f11306c23c038b08e5e070edb7be44bef6697fb8734dcff1c66b1
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz.asc' acl_2.3.1.orig.tar.xz.asc 833 SHA256:54fb8fcd6ae6901f2257e18d503e5e18ad956babf8d80d2ea29f280fc7264662
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-3.debian.tar.xz' acl_2.3.1-3.debian.tar.xz 30968 SHA256:2eb052bba784a4b873e951b1f91af2abef62e4bf4b83c93f9821eea26f66c8e2
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.3.1-3/ (for browsing the source)
- https://sources.debian.net/src/acl/2.3.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.3.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.137`

Binary Packages:

- `adduser=3.137`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.137
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.137.dsc' adduser_3.137.dsc 1671 SHA256:e4be6fbfa9db7ca7054a1c31dd2f1503340187b547112c960f2482ce3642f837
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.137.tar.xz' adduser_3.137.tar.xz 279192 SHA256:229a61803664c2850f7d8d93e6650cd0b340ea3bbd1b954271719679ea3b0dd0
```

Other potentially useful URLs:

- https://sources.debian.net/src/adduser/3.137/ (for browsing the source)
- https://sources.debian.net/src/adduser/3.137/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adduser/3.137/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr-util=1.6.3-1`

Binary Packages:

- `libaprutil1:amd64=1.6.3-1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.3-1
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.3-1.dsc' apr-util_1.6.3-1.dsc 2760 SHA256:e43ecafbe39a8d47fbe5faee705295435ac753e6b40c9b4c8d483a769ad8253e
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.3.orig.tar.bz2' apr-util_1.6.3.orig.tar.bz2 432692 SHA256:a41076e3710746326c3945042994ad9a4fcac0ce0277dd8fea076fec3c9772b5
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.3.orig.tar.bz2.asc' apr-util_1.6.3.orig.tar.bz2.asc 833 SHA256:5fd08491a2cb35fdbf9fa93d753cfd25e59fe58a75a3f3ed62582ebf2a5b3a51
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.3-1.debian.tar.xz' apr-util_1.6.3-1.debian.tar.xz 340808 SHA256:51400024f722f3427a720f485bd20874d846f38320e7fe52a290b8c9c7b201f5
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr-util/1.6.3-1/ (for browsing the source)
- https://sources.debian.net/src/apr-util/1.6.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr-util/1.6.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr=1.7.2-3`

Binary Packages:

- `libapr1:amd64=1.7.2-3`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.2-3
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.2-3.dsc' apr_1.7.2-3.dsc 2262 SHA256:8602db2a98e9e1bf7c8d1d0113f06a36ceb206ffd98580e38169a4c32ae05791
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.2.orig.tar.bz2' apr_1.7.2.orig.tar.bz2 890218 SHA256:75e77cc86776c030c0a5c408dfbd0bf2a0b75eed5351e52d5439fa1e5509a43e
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.2.orig.tar.bz2.asc' apr_1.7.2.orig.tar.bz2.asc 833 SHA256:3e45e804041cfd112d3710db11424e861a6f96e5b8908fcb73bc558f7d480f37
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.2-3.debian.tar.xz' apr_1.7.2-3.debian.tar.xz 54404 SHA256:5d7671b61847982c96666fcc271820ed88fe31e9092e0d01f3bfb19e20905ec9
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.7.2-3/ (for browsing the source)
- https://sources.debian.net/src/apr/1.7.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.7.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=2.7.6`

Binary Packages:

- `apt=2.7.6`
- `libapt-pkg6.0:amd64=2.7.6`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.7.6
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.7.6.dsc' apt_2.7.6.dsc 2945 SHA256:bdc573f2113e70fb648a819437d36b14427d492695460811f74214f174caf7fe
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.7.6.tar.xz' apt_2.7.6.tar.xz 2345736 SHA256:8683f54eff0bf54e51e025b348bd0774d0fd437799616f48512956cf15c05f67
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/2.7.6/ (for browsing the source)
- https://sources.debian.net/src/apt/2.7.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/2.7.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `attr=1:2.5.1-4`

Binary Packages:

- `libattr1:amd64=1:2.5.1-4`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.5.1-4
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-4.dsc' attr_2.5.1-4.dsc 2477 SHA256:0e1486bff1649602cb5cbb6224dbb641436dc8cd28d5c336ad85d650e07d23dd
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA256:db448a626f9313a1a970d636767316a8da32aede70518b8050fa0de7947adc32
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA256:67bc632e754efbadba846d0b40138b3fc3e306c3b909a9ba868c6dba1e2689d0
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-4.debian.tar.xz' attr_2.5.1-4.debian.tar.xz 32152 SHA256:aea02a3c980a82804a5a333bf02e9e2737a8c5808671625595511290863d6791
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.5.1-4/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.5.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.5.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:3.1.1-1`

Binary Packages:

- `libaudit-common=1:3.1.1-1`
- `libaudit1:amd64=1:3.1.1-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.1.1-1
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.1.1-1.dsc' audit_3.1.1-1.dsc 2402 SHA256:61ae8d226039ab2c4c241266c699d22a80a5a85db94dd030cff44ca7a8729bd5
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.1.1.orig.tar.gz' audit_3.1.1.orig.tar.gz 1218111 SHA256:46e46b37623cce09e6ee134e78d668afc34f4e1c870c853ef12e4193078cfe87
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.1.1-1.debian.tar.xz' audit_3.1.1-1.debian.tar.xz 18944 SHA256:b16ea47b6562a2530ec48e752ef6f31cd72b5dcdeec49b8720911584a54769cb
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:3.1.1-1/ (for browsing the source)
- https://sources.debian.net/src/audit/1:3.1.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:3.1.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `autoconf=2.71-3`

Binary Packages:

- `autoconf=2.71-3`

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
$ apt-get source -qq --print-uris autoconf=2.71-3
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.71-3.dsc' autoconf_2.71-3.dsc 1988 SHA256:2230ca8950e9b1abeeba54844c9e8184891fa2474a101c25f5d125bdacb92ef2
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.71.orig.tar.gz' autoconf_2.71.orig.tar.gz 2003781 SHA256:431075ad0bf529ef13cb41e9042c542381103e80015686222b8a9d4abef42a1c
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.71-3.debian.tar.xz' autoconf_2.71-3.debian.tar.xz 23896 SHA256:3c12ade6e26e8ccacd8e35de3eb93a1fcf360b02364cbe4690b958a749daf4d7
```

Other potentially useful URLs:

- https://sources.debian.net/src/autoconf/2.71-3/ (for browsing the source)
- https://sources.debian.net/src/autoconf/2.71-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autoconf/2.71-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `automake-1.16=1:1.16.5-1.3`

Binary Packages:

- `automake=1:1.16.5-1.3`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.5-1.3
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.3.dsc' automake-1.16_1.16.5-1.3.dsc 1973 SHA256:88bb6aad124dc9c8f8f37910f66bf79f19e1c4a1e5c69860e3e9005d2adc4d8d
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz' automake-1.16_1.16.5.orig.tar.xz 1601740 SHA256:f01d58cd6d9d77fbdca9eb4bbd5ead1988228fdb73d6f7a201f5f8d6b118b469
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz.asc' automake-1.16_1.16.5.orig.tar.xz.asc 833 SHA256:3a161ab65921eed55e1a94251d97c8451d4ba3431b55ca560e95a951b5f1d73a
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.3.debian.tar.xz' automake-1.16_1.16.5-1.3.debian.tar.xz 14164 SHA256:357d34b964943f5c46f518e3a7ddaa9342de76f1a01bac83039dc338ca84d421
```

Other potentially useful URLs:

- https://sources.debian.net/src/automake-1.16/1:1.16.5-1.3/ (for browsing the source)
- https://sources.debian.net/src/automake-1.16/1:1.16.5-1.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/automake-1.16/1:1.16.5-1.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `autotools-dev=20220109.1`

Binary Packages:

- `autotools-dev=20220109.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20220109.1
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20220109.1.dsc' autotools-dev_20220109.1.dsc 1661 SHA256:f9ccc67437ff52a7882d6b91e7ca8bf0a316c0c1452093992bd5c5fc3b29c090
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20220109.1.tar.xz' autotools-dev_20220109.1.tar.xz 87340 SHA256:8b05e5ad56cd7d9a15e9b2931eb429b6324bb89f1b46de3baf3651286dead8c1
```

Other potentially useful URLs:

- https://sources.debian.net/src/autotools-dev/20220109.1/ (for browsing the source)
- https://sources.debian.net/src/autotools-dev/20220109.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autotools-dev/20220109.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=13`

Binary Packages:

- `base-files=13`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=13
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_13.dsc' base-files_13.dsc 1093 SHA256:9a355f5c19670ce338c4febb196c427cc5f67940953478b515d555fba9fbdddc
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_13.tar.xz' base-files_13.tar.xz 66064 SHA256:439153bdf296481135cb0b801fe46765dc83f8b9914a0275d6a162339de12f56
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/13/ (for browsing the source)
- https://sources.debian.net/src/base-files/13/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/13/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.6.2`

Binary Packages:

- `base-passwd=3.6.2`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.6.2
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.6.2.dsc' base-passwd_3.6.2.dsc 1762 SHA256:b22ce63f0617fd06570b598412ba6a63b1237fe6849040eeb5651d02a8ef7de2
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.6.2.tar.xz' base-passwd_3.6.2.tar.xz 58264 SHA256:06dc78352bf38a8df76ff295e15ab5654cdefe41e62368b15bfcbbab8e4ec2a0
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.6.2/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.6.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.6.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.2.15-2`

Binary Packages:

- `bash=5.2.15-2+b6`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `BSD-4-clause-UC`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `Latex2e`
- `MIT-like`
- `permissive`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/bash/5.2.15-2/


### `dpkg` source package: `binutils=2.41-6`

Binary Packages:

- `binutils=2.41-6`
- `binutils-common:amd64=2.41-6`
- `binutils-x86-64-linux-gnu=2.41-6`
- `libbinutils:amd64=2.41-6`
- `libctf-nobfd0:amd64=2.41-6`
- `libctf0:amd64=2.41-6`
- `libgprofng0:amd64=2.41-6`
- `libsframe1:amd64=2.41-6`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`, `/usr/share/doc/libgprofng0/copyright`, `/usr/share/doc/libsframe1/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.41-6
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.41-6.dsc' binutils_2.41-6.dsc 12422 SHA256:b6bb464bc4bd66901c4a5277314176008e371369e79e63ac9af0ed101cbb397b
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.41.orig.tar.xz' binutils_2.41.orig.tar.xz 26902888 SHA256:f87777e6b11c92081692fa6a5239271961eab8354c91ca52f916b9e875cf79dc
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.41-6.debian.tar.xz' binutils_2.41-6.debian.tar.xz 188520 SHA256:1c94686fb9197b844fdfbae379a0198e648a3f6c5407f8a8602947dffdbc8334
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.41-6/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.41-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.41-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `boost1.74=1.74.0+ds1-23`

Binary Packages:

- `libboost-python1.74.0=1.74.0+ds1-23`

Licenses: (parsed from: `/usr/share/doc/libboost-python1.74.0/copyright`)

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
$ apt-get source -qq --print-uris boost1.74=1.74.0+ds1-23
'http://deb.debian.org/debian/pool/main/b/boost1.74/boost1.74_1.74.0%2bds1-23.dsc' boost1.74_1.74.0+ds1-23.dsc 8452 SHA256:b229698139f1f02cf67feaa0005dda221d8793734275d23c36396a65dff2c62d
'http://deb.debian.org/debian/pool/main/b/boost1.74/boost1.74_1.74.0%2bds1.orig.tar.xz' boost1.74_1.74.0+ds1.orig.tar.xz 60678948 SHA256:192f5df504d282cb81288f88232d8af45b64a9ab531e1c7cf8ae955f16f6bb28
'http://deb.debian.org/debian/pool/main/b/boost1.74/boost1.74_1.74.0%2bds1-23.debian.tar.xz' boost1.74_1.74.0+ds1-23.debian.tar.xz 375820 SHA256:e92ed5751dc2e245211e0fb42fd2eeeee7aa55704d14b2337ee7d9e3cb1a9bb7
```

Other potentially useful URLs:

- https://sources.debian.net/src/boost1.74/1.74.0+ds1-23/ (for browsing the source)
- https://sources.debian.net/src/boost1.74/1.74.0+ds1-23/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/boost1.74/1.74.0+ds1-23/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2+b6`
- `libbrotli1:amd64=1.0.9-2+b6`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/brotli/1.0.9-2/


### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `bzip2=1.0.8-5+b1`
- `libbz2-1.0:amd64=1.0.8-5+b1`
- `libbz2-dev:amd64=1.0.8-5+b1`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-5
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-5.dsc' bzip2_1.0.8-5.dsc 2206 SHA256:ed9c40f4de3f9e064535e15eac1c61a0f606763db98f4579dbc04067b94a8944
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-5.debian.tar.bz2' bzip2_1.0.8-5.debian.tar.bz2 26787 SHA256:d68c6eba11d70e14319e24ef1451880a03023b2b75364646adb117086db36039
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.8-5/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.8-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.8-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20230311`

Binary Packages:

- `ca-certificates=20230311`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20230311
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20230311.dsc' ca-certificates_20230311.dsc 1768 SHA256:bf44adb22fce619310b0f8d7bb6952b0a80907de9e3ecb773143769e98478a3b
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20230311.tar.xz' ca-certificates_20230311.tar.xz 257772 SHA256:83de934afa186e279d1ed08ea0d73f5cf43a6fbfb5f00874b6db3711c64576f3
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20230311/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20230311/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20230311/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cairo=1.18.0-1`

Binary Packages:

- `libcairo-gobject2:amd64=1.18.0-1`
- `libcairo-script-interpreter2:amd64=1.18.0-1`
- `libcairo2:amd64=1.18.0-1`
- `libcairo2-dev:amd64=1.18.0-1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.18.0-1
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.18.0-1.dsc' cairo_1.18.0-1.dsc 2772 SHA256:524223b43506f55b644770626b215cb694e6b8d52c57dbf149150453622a99da
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.18.0.orig.tar.xz' cairo_1.18.0.orig.tar.xz 33761148 SHA256:243a0736b978a33dee29f9cca7521733b78a65b5418206fef7bd1c3d4cf10b64
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.18.0-1.debian.tar.xz' cairo_1.18.0-1.debian.tar.xz 29720 SHA256:6cb6c2f74294818f9b6322b2431f994665ff12ac8d931e665e6feefbd0c6e3e4
```

Other potentially useful URLs:

- https://sources.debian.net/src/cairo/1.18.0-1/ (for browsing the source)
- https://sources.debian.net/src/cairo/1.18.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cairo/1.18.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.271`

Binary Packages:

- `libdebconfclient0:amd64=0.271`

Licenses: (parsed from: `/usr/share/doc/libdebconfclient0/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.271
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.271.dsc' cdebconf_0.271.dsc 2707 SHA256:626c8da9b0fd07f37c94940401a8ba92bc3c454673c266e9c927934139e2a079
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.271.tar.xz' cdebconf_0.271.tar.xz 284308 SHA256:b66fd2ea674d22f64a01672fe6c1891ef54ca906fb5c49d8362cba0d78b270c8
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.271/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.271/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.271/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=9.1-1`

Binary Packages:

- `coreutils=9.1-1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `BSD-4-clause-UC`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris coreutils=9.1-1
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_9.1-1.dsc' coreutils_9.1-1.dsc 1848 SHA256:2f2fca0a07a1a3f38e3ebeb4cbd97e97e675e77bed84f3e9d0b7e5da4cde75fc
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_9.1.orig.tar.xz' coreutils_9.1.orig.tar.xz 5712104 SHA256:61a1f410d78ba7e7f37a5a4f50e6d1320aca33375484a3255eddf17a38580423
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_9.1-1.debian.tar.xz' coreutils_9.1-1.debian.tar.xz 30624 SHA256:45d4ae88d933a7d713ef038943e818a2488e759b6196a409788744cbc6df1832
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/9.1-1/ (for browsing the source)
- https://sources.debian.net/src/coreutils/9.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/9.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=8.4.0-2`

Binary Packages:

- `curl=8.4.0-2`
- `libcurl3-gnutls:amd64=8.4.0-2`
- `libcurl4:amd64=8.4.0-2`
- `libcurl4-openssl-dev:amd64=8.4.0-2`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `BSD-4-Clause-UC`
- `FSFULLR`
- `GPL-2`
- `GPL-2+ with Autoconf-data exception`
- `GPL-2+ with Libtool exception`
- `GPL-3+ with Autoconf-data exception`
- `ISC`
- `OLDAP-2.8`
- `X11`
- `curl`

Source:

```console
$ apt-get source -qq --print-uris curl=8.4.0-2
'http://deb.debian.org/debian/pool/main/c/curl/curl_8.4.0-2.dsc' curl_8.4.0-2.dsc 3044 SHA256:9d5b6ba82646f045a14d8f3df4edddf9b7b2b900a47d61493e7e57cf6a1c52ab
'http://deb.debian.org/debian/pool/main/c/curl/curl_8.4.0.orig.tar.gz' curl_8.4.0.orig.tar.gz 4424232 SHA256:816e41809c043ff285e8c0f06a75a1fa250211bbfb2dc0a037eeef39f1a9e427
'http://deb.debian.org/debian/pool/main/c/curl/curl_8.4.0.orig.tar.gz.asc' curl_8.4.0.orig.tar.gz.asc 488 SHA256:904d8cb18dbc2b3d30087a73042bffe402ca8800e8ab32613aa97e0b225402af
'http://deb.debian.org/debian/pool/main/c/curl/curl_8.4.0-2.debian.tar.xz' curl_8.4.0-2.debian.tar.xz 45320 SHA256:fa8280c76863be15a824bec714ef8b3ec208bafaa32742c477542f3c3fa7f637
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/8.4.0-2/ (for browsing the source)
- https://sources.debian.net/src/curl/8.4.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/8.4.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg1-4`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg1-4`
- `libsasl2-modules-db:amd64=2.1.28+dfsg1-4`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-2.2-clause`
- `BSD-3-Clause-Attribution`
- `BSD-3-clause`
- `BSD-3-clause-JANET`
- `BSD-3-clause-PADL`
- `BSD-4-clause-UC`
- `FSFULLR`
- `GPL-3`
- `GPL-3+`
- `IBM-as-is`
- `MIT-CMU`
- `MIT-Export`
- `MIT-OpenVision`
- `OpenLDAP`
- `RSA-MD`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg1-4
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1-4.dsc' cyrus-sasl2_2.1.28+dfsg1-4.dsc 3224 SHA256:d2169fde5404f07f71ae5265e308f0239e2788c0f8115fa3f10ce83ba4c1fd5d
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg1.orig.tar.xz 794540 SHA256:e796a5d85d1a85e1b433d43504e467f9075c7ebc0b45730a3996cf11b1deada4
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1-4.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg1-4.debian.tar.xz 96688 SHA256:10f7765c85fb0601c0e9cf9d0ac250d194cd7d190f4656ca52dcd993c731ff4c
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg1-4/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.28+dfsg1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.12-6`

Binary Packages:

- `dash=0.5.12-6`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.12-6
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.12-6.dsc' dash_0.5.12-6.dsc 1520 SHA256:dfca9cb9a537d09c190baa9fb15848ecaa55f301843779f26260b1429cd72746
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.12.orig.tar.gz' dash_0.5.12.orig.tar.gz 246054 SHA256:6a474ac46e8b0b32916c4c60df694c82058d3297d8b385b74508030ca4a8f28a
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.12-6.debian.tar.xz' dash_0.5.12-6.debian.tar.xz 39116 SHA256:155173292d95943d2c737c0f7f4733bb6b39244522f810ee4a64f7be0f4865ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.12-6/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.12-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.12-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dav1d=1.3.0-2`

Binary Packages:

- `libdav1d7:amd64=1.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libdav1d7/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dav1d=1.3.0-2
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_1.3.0-2.dsc' dav1d_1.3.0-2.dsc 2287 SHA256:1003897eded2bb21a34dad143f2578ccdbbbfa675ce1c93a97bbffab9eabf443
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_1.3.0.orig.tar.xz' dav1d_1.3.0.orig.tar.xz 885220 SHA256:6d8be2741c505c47f8f1ced3c9cc427759243436553d01d1acce201f87b39e71
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_1.3.0.orig.tar.xz.asc' dav1d_1.3.0.orig.tar.xz.asc 195 SHA256:43c11852cb564ac740c36711e185ea44022dbb88b54b47a3ef398972f526ebaa
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_1.3.0-2.debian.tar.xz' dav1d_1.3.0-2.debian.tar.xz 8204 SHA256:c9877af2c01ed67a946126c2f5e8b5f5394bf54eb1dcd2c6b5659d939098e407
```

Other potentially useful URLs:

- https://sources.debian.net/src/dav1d/1.3.0-2/ (for browsing the source)
- https://sources.debian.net/src/dav1d/1.3.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dav1d/1.3.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db-defaults=5.3.3`

Binary Packages:

- `libdb-dev:amd64=5.3.3`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=5.3.3
'http://deb.debian.org/debian/pool/main/d/db-defaults/db-defaults_5.3.3.dsc' db-defaults_5.3.3.dsc 1321 SHA256:774706cfb3a12d52a9cfa7c915aa001652e89c56887ca080a314744881a3e21b
'http://deb.debian.org/debian/pool/main/d/db-defaults/db-defaults_5.3.3.tar.xz' db-defaults_5.3.3.tar.xz 2432 SHA256:f4a44815b88fb3ae516ea5612b87882cceb9c54afa9184e91d7fdb3d1942f6a5
```

Other potentially useful URLs:

- https://sources.debian.net/src/db-defaults/5.3.3/ (for browsing the source)
- https://sources.debian.net/src/db-defaults/5.3.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db-defaults/5.3.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg2-4`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg2-4`
- `libdb5.3-dev=5.3.28+dfsg2-4`

Licenses: (parsed from: `/usr/share/doc/libdb5.3/copyright`, `/usr/share/doc/libdb5.3-dev/copyright`)

- `Artistic`
- `BSD-3-clause`
- `BSD-3-clause-fjord`
- `GPL`
- `GPL-3`
- `MIT-old`
- `Ms-PL`
- `Sleepycat`
- `TCL-like`
- `X11`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg2-4
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-4.dsc' db5.3_5.3.28+dfsg2-4.dsc 2190 SHA256:c25a3d8a199e6ea7a251a192acb6c8e5e130271dfa190b6486ac08dbb81a861b
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2.orig.tar.xz' db5.3_5.3.28+dfsg2.orig.tar.xz 21287688 SHA256:ad41b507415dec8316e828b2230242af2251d2c86eefa3c7aa9ef47c5239ef33
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-4.debian.tar.xz' db5.3_5.3.28+dfsg2-4.debian.tar.xz 33624 SHA256:1cab3a408ba22a1307d4b55c5aff986423a75f8b95cc58b7bcaa143817bc1aa4
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg2-4/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.82`

Binary Packages:

- `debconf=1.5.82`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.82
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.82.dsc' debconf_1.5.82.dsc 2035 SHA256:ed6e8cc6e073344a25ab932602b3b814f25cfa1a7bfd69e464f9bad65f250dea
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.82.tar.xz' debconf_1.5.82.tar.xz 571540 SHA256:2d0550c4e2fb98d12055b245907978b28ee2d2b07b62e46be7523384d2ce985e
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.82/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.82/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.82/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debian-archive-keyring=2023.4`

Binary Packages:

- `debian-archive-keyring=2023.4`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2023.4
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2023.4.dsc' debian-archive-keyring_2023.4.dsc 1261 SHA256:c97d048486078fcc6866a477df83b19270ae872102f4ed64b5a5e9995ff79afa
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2023.4.tar.xz' debian-archive-keyring_2023.4.tar.xz 177568 SHA256:7f9b64d7c5e748b0cb99fd0674d872111c219e119f296912c59fc61ab49bb78a
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2023.4/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2023.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2023.4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=5.14`

Binary Packages:

- `debianutils=5.14`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`
- `GPL-2+`
- `SMAIL-GPL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.14
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.14.dsc' debianutils_5.14.dsc 1631 SHA256:328e7aabb75e6bd284ee2a4e7661091a202c16edb8e18e4402f7209b01d965d6
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.14.tar.xz' debianutils_5.14.tar.xz 79676 SHA256:531a9542b4054bfb4c26a9fd5f1e6489fc728f52785270ddd9434c14a56b1108
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/5.14/ (for browsing the source)
- https://sources.debian.net/src/debianutils/5.14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/5.14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.10-1`

Binary Packages:

- `diffutils=1:3.10-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `FSFAP`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with autoconf exception`
- `GPL-3+ with texinfo exception`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3.0+`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.10-1
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.10-1.dsc' diffutils_3.10-1.dsc 1715 SHA256:f7542884c67d44f0af356c5365a3fef8a298f1fbcbebf9df81cfbc6d6937f05f
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.10.orig.tar.xz' diffutils_3.10.orig.tar.xz 1624240 SHA256:90e5e93cc724e4ebe12ede80df1634063c7a855692685919bfe60b556c9bd09e
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.10.orig.tar.xz.asc' diffutils_3.10.orig.tar.xz.asc 833 SHA256:a94faf8f1baa04ff220f7b2ccb137c16337284e023ebc4a1d5df475c08d810f7
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.10-1.debian.tar.xz' diffutils_3.10-1.debian.tar.xz 13952 SHA256:ebf51a7ceff8c882f997ca428232fd3b58ac59a70840c4b10f8fcfaa881598ce
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.10-1/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `djvulibre=3.5.28-2`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.28-2+b1`
- `libdjvulibre-text=3.5.28-2`
- `libdjvulibre21:amd64=3.5.28-2+b1`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.28-2
'http://deb.debian.org/debian/pool/main/d/djvulibre/djvulibre_3.5.28-2.dsc' djvulibre_3.5.28-2.dsc 2388 SHA256:0b5f31e70a8f81afec47e67e9465dbece7756f0c7f88da643f0dda82bf78a1ba
'http://deb.debian.org/debian/pool/main/d/djvulibre/djvulibre_3.5.28.orig.tar.xz' djvulibre_3.5.28.orig.tar.xz 2959024 SHA256:1223b7bf7c8dfe2e290882f3bfb88ba2468b30495a1bf8dfd54dc7e810987887
'http://deb.debian.org/debian/pool/main/d/djvulibre/djvulibre_3.5.28-2.debian.tar.xz' djvulibre_3.5.28-2.debian.tar.xz 17420 SHA256:6f85dcd7cdb856cc3e4a31fc381e73a6cab717c90e058f474fb4d2ab29635d91
```

Other potentially useful URLs:

- https://sources.debian.net/src/djvulibre/3.5.28-2/ (for browsing the source)
- https://sources.debian.net/src/djvulibre/3.5.28-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/djvulibre/3.5.28-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.22.1`

Binary Packages:

- `dpkg=1.22.1`
- `dpkg-dev=1.22.1`
- `libdpkg-perl=1.22.1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.22.1
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.22.1.dsc' dpkg_1.22.1.dsc 3041 SHA256:cf386e2b809b470e3a06fde62928e1603967203a9db464d3622b13f3b15d4142
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.22.1.tar.xz' dpkg_1.22.1.tar.xz 5584944 SHA256:5a4824e9869494e501953c7466ab1960a7fa23d9b0b911b8a6f113094e0226cf
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.22.1/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.22.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.22.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.47.0-2`

Binary Packages:

- `comerr-dev:amd64=2.1-1.47.0-2+b1`
- `e2fsprogs=1.47.0-2+b1`
- `libcom-err2:amd64=1.47.0-2+b1`
- `libext2fs2:amd64=1.47.0-2+b1`
- `libss2:amd64=1.47.0-2+b1`
- `logsave=1.47.0-2+b1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `Apache-2`
- `Apache-2.0`
- `BSD-3-Clause`
- `GPL`
- `GPL-2`
- `GPL-2+ with Texinfo exception`
- `ISC`
- `Kazlib`
- `LGPL-2`
- `Latex2e`
- `MIT-US-export`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.47.0-2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0-2.dsc' e2fsprogs_1.47.0-2.dsc 2846 SHA256:35b4de254e021f721362b767994598e249fea02e38ac446197cd9c22be1130fd
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0.orig.tar.gz' e2fsprogs_1.47.0.orig.tar.gz 9637717 SHA256:6667afde56eef0c6af26684974400e4d2288ea49e9441bf5e6229195d51a3578
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0.orig.tar.gz.asc' e2fsprogs_1.47.0.orig.tar.gz.asc 488 SHA256:704928204a52ddaa0ac8ef549c1bfba3c38e66c361d3853c8a4c38e6082b90f1
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0-2.debian.tar.xz' e2fsprogs_1.47.0-2.debian.tar.xz 87328 SHA256:3a756e08d300666039e34577293d11d70c7a1da7850fad478580a81af6348277
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.47.0-2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.47.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.47.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `elfutils=0.189-4`

Binary Packages:

- `libelf1:amd64=0.189-4`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `BSD-2-clause`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/elfutils/0.189-4/


### `dpkg` source package: `expat=2.5.0-2`

Binary Packages:

- `libexpat1:amd64=2.5.0-2`
- `libexpat1-dev:amd64=2.5.0-2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.5.0-2
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.5.0-2.dsc' expat_2.5.0-2.dsc 1964 SHA256:b4aab5ad11812b0593128742f08be007a0c1663d683b7ef705d0660db6e94544
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.5.0.orig.tar.gz' expat_2.5.0.orig.tar.gz 8320988 SHA256:ab00ee05c7067fd10a35c5d2a4922ebba746ddd50ff83b79c828da17bbdf1757
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.5.0-2.debian.tar.xz' expat_2.5.0-2.debian.tar.xz 12804 SHA256:605973555634c2197ce219736cbb7eb17464894768c5fe2c4b8b8279f052ece5
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.5.0-2/ (for browsing the source)
- https://sources.debian.net/src/expat/2.5.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.5.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fftw3=3.3.10-1`

Binary Packages:

- `libfftw3-double3:amd64=3.3.10-1`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.10-1
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.10-1.dsc' fftw3_3.3.10-1.dsc 2771 SHA256:5c6a64c8047e33f122fb1eebd4316178e3da86da16de70da0527906adcf22924
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.10.orig.tar.gz' fftw3_3.3.10.orig.tar.gz 4144100 SHA256:56c932549852cddcfafdab3820b0200c7742675be92179e59e6215b340e26467
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.10-1.debian.tar.xz' fftw3_3.3.10-1.debian.tar.xz 14520 SHA256:a19c2fa4eebb123626a8df89387e3437369d234f68799d3b2c0c9fb84b9ca875
```

Other potentially useful URLs:

- https://sources.debian.net/src/fftw3/3.3.10-1/ (for browsing the source)
- https://sources.debian.net/src/fftw3/3.3.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fftw3/3.3.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `file=1:5.45-2`

Binary Packages:

- `file=1:5.45-2`
- `libmagic-mgc=1:5.45-2`
- `libmagic1:amd64=1:5.45-2`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.45-2
'http://deb.debian.org/debian/pool/main/f/file/file_5.45-2.dsc' file_5.45-2.dsc 2240 SHA256:19e9b54d226b31f6cb9740330135bdf382213e27d5e6a73b47a94dd4c500f892
'http://deb.debian.org/debian/pool/main/f/file/file_5.45.orig.tar.gz' file_5.45.orig.tar.gz 1246503 SHA256:fc97f51029bb0e2c9f4e3bffefdaf678f0e039ee872b9de5c002a6d09c784d82
'http://deb.debian.org/debian/pool/main/f/file/file_5.45.orig.tar.gz.asc' file_5.45.orig.tar.gz.asc 169 SHA256:81aacbee95911bd9825e81748d42f41dadf846ba13165462dc428467ed9ee075
'http://deb.debian.org/debian/pool/main/f/file/file_5.45-2.debian.tar.xz' file_5.45-2.debian.tar.xz 34452 SHA256:ae29610c9a6b82fff65b17140ba1cd91e01cda6406c66c12baeb3aadcdf82787
```

Other potentially useful URLs:

- https://sources.debian.net/src/file/1:5.45-2/ (for browsing the source)
- https://sources.debian.net/src/file/1:5.45-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/file/1:5.45-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.9.0-5`

Binary Packages:

- `findutils=4.9.0-5`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `BSD-3-clause`
- `BSD-3-clause and/or GPL-3+`
- `FSFAP`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL with automake exception`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf-data exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Autoconf-data exception`
- `GPL-3+ with Bison-2.2 exception`
- `ISC`
- `ISC and/or LGPL-2.1+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.9.0-5
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-5.dsc' findutils_4.9.0-5.dsc 2272 SHA256:7d723c60c50b8b624250ad7d6fbb1ca404756a7b69209753e57c8403e06a07a5
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA256:a2bfb8c09d436770edc59f50fa483e785b161a3b7b9d547573cb08065fd462fe
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA256:924c3719d066eda1b3e47175f8b83e90e9a23f0a639ebe7445621917b283c385
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-5.debian.tar.xz' findutils_4.9.0-5.debian.tar.xz 32744 SHA256:456831869d49d8906a98beb2bcbb61e5911d9c44082c4b716615bc23f26c4f20
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.9.0-5/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.9.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.9.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fontconfig=2.14.2-6`

Binary Packages:

- `fontconfig=2.14.2-6`
- `fontconfig-config=2.14.2-6`
- `libfontconfig-dev:amd64=2.14.2-6`
- `libfontconfig1:amd64=2.14.2-6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.14.2-6
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.14.2-6.dsc' fontconfig_2.14.2-6.dsc 2323 SHA256:45f357363d06b8ea6efa02e081c8713dfcf05a5a7df97262fd31d4b35d1eb002
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.14.2.orig.tar.xz' fontconfig_2.14.2.orig.tar.xz 1440844 SHA256:dba695b57bce15023d2ceedef82062c2b925e51f5d4cc4aef736cf13f60a468b
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.14.2-6.debian.tar.xz' fontconfig_2.14.2-6.debian.tar.xz 57916 SHA256:09287ffc3dcee05a78e70d078e1f4c4a18766821177ce7a9764bc318a6bf4fe3
```

Other potentially useful URLs:

- https://sources.debian.net/src/fontconfig/2.14.2-6/ (for browsing the source)
- https://sources.debian.net/src/fontconfig/2.14.2-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fontconfig/2.14.2-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fonts-dejavu=2.37-8`

Binary Packages:

- `fonts-dejavu-core=2.37-8`
- `fonts-dejavu-mono=2.37-8`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`, `/usr/share/doc/fonts-dejavu-mono/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-8
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-8.dsc' fonts-dejavu_2.37-8.dsc 2156 SHA256:219f7f8fba98827caaa296520730171ec230d3090ed8b6d663edb66839b48847
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-8.debian.tar.xz' fonts-dejavu_2.37-8.debian.tar.xz 13176 SHA256:2401402245dec8a59fc5f0f8eff76d203a38440797f7f223e1d044e07c2d41fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/fonts-dejavu/2.37-8/ (for browsing the source)
- https://sources.debian.net/src/fonts-dejavu/2.37-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fonts-dejavu/2.37-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `freetype=2.13.2+dfsg-1`

Binary Packages:

- `libfreetype-dev:amd64=2.13.2+dfsg-1`
- `libfreetype6:amd64=2.13.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`)

- `BSD-3-Clause`
- `BSL-1.0`
- `Expat`
- `FSFAP`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT-Modern-Variant`
- `MIT-SMC`
- `OpenGroup-MIT`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.13.2+dfsg-1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.13.2%2bdfsg-1.dsc' freetype_2.13.2+dfsg-1.dsc 3686 SHA256:0e00399f7835b49c2606053b6681d2ef43693c6d5d7e6c86c29d1784c5e95e5a
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.13.2%2bdfsg.orig-ft2demos.tar.xz' freetype_2.13.2+dfsg.orig-ft2demos.tar.xz 341140 SHA256:99ee2ed8b98bcfad17bc57c2d9699d764f20fe29ad304c69b8eb28834ca3b48e
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.13.2%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.13.2+dfsg.orig-ft2demos.tar.xz.asc 833 SHA256:e58ba462f7bdcdc5899f777d33453c1ce6f6e46b080047580f45c9fd9f2dc08c
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.13.2%2bdfsg.orig-ft2docs.tar.xz' freetype_2.13.2+dfsg.orig-ft2docs.tar.xz 2173920 SHA256:685c25e1035a5076e5097186b3143b9c06878f3f9087d0a81e4d8538d5d15424
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.13.2%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.13.2+dfsg.orig-ft2docs.tar.xz.asc 833 SHA256:d7e17c8a3bce50181530ebe06346f506cbfc92ecc5ca7cc395c7dbb24a71a5c0
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.13.2%2bdfsg.orig.tar.xz' freetype_2.13.2+dfsg.orig.tar.xz 2220368 SHA256:48c78a4194adfcd15a4d089f3206dab8454c311f5577f3ef7eaef95f777f86e6
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.13.2%2bdfsg-1.debian.tar.xz' freetype_2.13.2+dfsg-1.debian.tar.xz 43824 SHA256:c1db3a2bf2a754fc3666b06757f4055fa7f964b256aaa520f6b7142b68e3c0bb
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.13.2+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.13.2+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.13.2+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fribidi=1.0.13-3`

Binary Packages:

- `libfribidi0:amd64=1.0.13-3`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.13-3
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.13-3.dsc' fribidi_1.0.13-3.dsc 2007 SHA256:05a44442861c66fa72d7764ff4c4ad4cf46114eb7fb53268b8c46bc3e3fa06b9
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.13.orig.tar.xz' fribidi_1.0.13.orig.tar.xz 1170100 SHA256:7fa16c80c81bd622f7b198d31356da139cc318a63fc7761217af4130903f54a2
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.13-3.debian.tar.xz' fribidi_1.0.13-3.debian.tar.xz 8848 SHA256:6e1e94396207a0acfbaa4dcbbb06ccc110fd9f285fd39ca313b5a8a3da9936fa
```

Other potentially useful URLs:

- https://sources.debian.net/src/fribidi/1.0.13-3/ (for browsing the source)
- https://sources.debian.net/src/fribidi/1.0.13-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fribidi/1.0.13-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-13=13.2.0-5`

Binary Packages:

- `cpp-13=13.2.0-5`
- `g++-13=13.2.0-5`
- `gcc-13=13.2.0-5`
- `gcc-13-base:amd64=13.2.0-5`
- `libasan8:amd64=13.2.0-5`
- `libatomic1:amd64=13.2.0-5`
- `libcc1-0:amd64=13.2.0-5`
- `libgcc-13-dev:amd64=13.2.0-5`
- `libgcc-s1:amd64=13.2.0-5`
- `libgfortran5:amd64=13.2.0-5`
- `libgomp1:amd64=13.2.0-5`
- `libhwasan0:amd64=13.2.0-5`
- `libitm1:amd64=13.2.0-5`
- `liblsan0:amd64=13.2.0-5`
- `libquadmath0:amd64=13.2.0-5`
- `libstdc++-13-dev:amd64=13.2.0-5`
- `libstdc++6:amd64=13.2.0-5`
- `libtsan2:amd64=13.2.0-5`
- `libubsan1:amd64=13.2.0-5`

Licenses: (parsed from: `/usr/share/doc/cpp-13/copyright`, `/usr/share/doc/g++-13/copyright`, `/usr/share/doc/gcc-13/copyright`, `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libasan8/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-13-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libhwasan0/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-13-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan2/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-13=13.2.0-5
'http://deb.debian.org/debian/pool/main/g/gcc-13/gcc-13_13.2.0-5.dsc' gcc-13_13.2.0-5.dsc 27214 SHA256:7d45361cd63ef53a5d30d14841c95098deae5fde475b4e0b8f9579c28214740e
'http://deb.debian.org/debian/pool/main/g/gcc-13/gcc-13_13.2.0.orig.tar.gz' gcc-13_13.2.0.orig.tar.gz 89714914 SHA256:eb19e797d4277a1ad26b1992bbf22dc66d11cce0c238491e746e50a7599aa064
'http://deb.debian.org/debian/pool/main/g/gcc-13/gcc-13_13.2.0-5.debian.tar.xz' gcc-13_13.2.0-5.debian.tar.xz 1634052 SHA256:a33816756c60309818ec7db50d8c7743a32164c19872efa6555dbb4c89c84d4e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-13/13.2.0-5/ (for browsing the source)
- https://sources.debian.net/src/gcc-13/13.2.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-13/13.2.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-defaults=1.208`

Binary Packages:

- `cpp=4:13.2.0-1`
- `g++=4:13.2.0-1`
- `gcc=4:13.2.0-1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gcc-defaults/1.208/


### `dpkg` source package: `gdbm=1.23-3`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-3`
- `libgdbm-dev:amd64=1.23-3`
- `libgdbm6:amd64=1.23-3`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gdbm/1.23-3/


### `dpkg` source package: `gdk-pixbuf=2.42.10+dfsg-3`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.42.10+dfsg-3`
- `libgdk-pixbuf-2.0-0:amd64=2.42.10+dfsg-3`
- `libgdk-pixbuf-2.0-dev:amd64=2.42.10+dfsg-3`
- `libgdk-pixbuf2.0-bin=2.42.10+dfsg-3`
- `libgdk-pixbuf2.0-common=2.42.10+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-dev/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `CC0-1.0`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.42.10+dfsg-3
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.10%2bdfsg-3.dsc' gdk-pixbuf_2.42.10+dfsg-3.dsc 3214 SHA256:cba4d9dbbc0a35d8e55137c9fa1da06d73881baf4b4f483f7a7ddd5ecaa2d98f
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.10%2bdfsg.orig.tar.xz' gdk-pixbuf_2.42.10+dfsg.orig.tar.xz 6439240 SHA256:46663e445468e92f4a0ca876b02aed4f8758595ee3acfaa6ef3ba2b29e1c1930
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.10%2bdfsg-3.debian.tar.xz' gdk-pixbuf_2.42.10+dfsg-3.debian.tar.xz 21336 SHA256:dd8003ae4be59c261ad6502d379065623681576679371109470085aa8ac94bc8
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdk-pixbuf/2.42.10+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/gdk-pixbuf/2.42.10+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdk-pixbuf/2.42.10+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.42.0-1`

Binary Packages:

- `git=1:2.42.0-1`
- `git-man=1:2.42.0-1`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-3-clause`
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
- `Zlib`
- `dlmalloc`
- `mingw-runtime`

Source:

```console
$ apt-get source -qq --print-uris git=1:2.42.0-1
'http://deb.debian.org/debian/pool/main/g/git/git_2.42.0-1.dsc' git_2.42.0-1.dsc 2825 SHA256:b5bc4f48d8ee242ec7d485e5bceb3e1bd96cfdcaa2a545591fa4d902b3f6c48a
'http://deb.debian.org/debian/pool/main/g/git/git_2.42.0.orig.tar.xz' git_2.42.0.orig.tar.xz 7346760 SHA256:3278210e9fd2994b8484dd7e3ddd9ea8b940ef52170cdb606daa94d887c93b0d
'http://deb.debian.org/debian/pool/main/g/git/git_2.42.0-1.debian.tar.xz' git_2.42.0-1.debian.tar.xz 757596 SHA256:db6b5bdacb87cd716453c8bdd5d5652da9f8c3b1be062ee3b2624056889103b4
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.42.0-1/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.42.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.42.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.78.1-4`

Binary Packages:

- `libglib2.0-0:amd64=2.78.1-4`
- `libglib2.0-bin=2.78.1-4`
- `libglib2.0-data=2.78.1-4`
- `libglib2.0-dev:amd64=2.78.1-4`
- `libglib2.0-dev-bin=2.78.1-4`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `AFL-2.0`
- `Apache-2.0`
- `Apache-2.0 with LLVM exception`
- `BSD-3-clause-pcre`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `Expat`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `Iconv-PD`
- `Janik-permissive`
- `Kuchling-PD`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `Mingw-PD`
- `Old-GLib-Tests-permissive`
- `Plumb-PD`
- `Unicode-DFS-2016`
- `bzip2-1.0.6`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.78.1-4
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.78.1-4.dsc' glib2.0_2.78.1-4.dsc 3648 SHA256:83726c95a55e9c623b63bdee774a514b6493b1c889356ae0af01eb8056c7bbbb
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.78.1.orig-unicode-data.tar.xz' glib2.0_2.78.1.orig-unicode-data.tar.xz 267604 SHA256:f10f77c45e96ccd4866dad2cb79a314b57180a05929a612dfe86d89e471406b5
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.78.1.orig.tar.xz' glib2.0_2.78.1.orig.tar.xz 5320740 SHA256:915bc3d0f8507d650ead3832e2f8fb670fce59aac4d7754a7dab6f1e6fed78b2
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.78.1-4.debian.tar.xz' glib2.0_2.78.1-4.debian.tar.xz 126452 SHA256:b819f71aa9014dce4026cc32ed3921dccbb937a1aa6309793b86d9426854479c
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.78.1-4/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.78.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.78.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.37-12`

Binary Packages:

- `libc-bin=2.37-12`
- `libc-dev-bin=2.37-12`
- `libc6:amd64=2.37-12`
- `libc6-dev:amd64=2.37-12`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.37-12
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.37-12.dsc' glibc_2.37-12.dsc 8963 SHA256:db193e8739478594bc075c1e5f8b20260d4eabaa4ae65f8d44c2c9c59593cc8b
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.37.orig.tar.xz' glibc_2.37.orig.tar.xz 19503016 SHA256:d05f010158c16cef110fa1ab560c31477249ee2105360101858a5146aa6fe7d0
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.37-12.debian.tar.xz' glibc_2.37-12.debian.tar.xz 412360 SHA256:a3e674efb034c53e2d6643a25064b50ae0a833290edff5e8e8892b72804e00a8
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.37-12/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.37-12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.37-12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.3.0+dfsg-2`

Binary Packages:

- `libgmp-dev:amd64=2:6.3.0+dfsg-2`
- `libgmp10:amd64=2:6.3.0+dfsg-2`
- `libgmpxx4ldbl:amd64=2:6.3.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.3.0+dfsg-2
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.3.0%2bdfsg-2.dsc' gmp_6.3.0+dfsg-2.dsc 2251 SHA256:31bf88a2899f7a6eb2dc0db438ba2b27f87562dfe73815a3bbc8b65675ba1a51
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.3.0%2bdfsg.orig.tar.xz' gmp_6.3.0+dfsg.orig.tar.xz 1870556 SHA256:bd2966e6d277f79328e894a5a9f3ba3fbf2ed2be81def5f48623e30c23fb1572
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.3.0%2bdfsg-2.debian.tar.xz' gmp_6.3.0+dfsg-2.debian.tar.xz 19156 SHA256:07fbc1f67c1c076575f8196f3b5a2d2be0268be10940ca59293d7f1669365f4e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.3.0+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.3.0+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.3.0+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.40-1.1`

Binary Packages:

- `dirmngr=2.2.40-1.1`
- `gnupg=2.2.40-1.1`
- `gnupg-l10n=2.2.40-1.1`
- `gnupg-utils=2.2.40-1.1`
- `gpg=2.2.40-1.1`
- `gpg-agent=2.2.40-1.1`
- `gpg-wks-client=2.2.40-1.1`
- `gpg-wks-server=2.2.40-1.1`
- `gpgconf=2.2.40-1.1`
- `gpgsm=2.2.40-1.1`
- `gpgv=2.2.40-1.1`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-l10n/copyright`, `/usr/share/doc/gnupg-utils/copyright`, `/usr/share/doc/gpg/copyright`, `/usr/share/doc/gpg-agent/copyright`, `/usr/share/doc/gpg-wks-client/copyright`, `/usr/share/doc/gpg-wks-server/copyright`, `/usr/share/doc/gpgconf/copyright`, `/usr/share/doc/gpgsm/copyright`, `/usr/share/doc/gpgv/copyright`)

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
$ apt-get source -qq --print-uris gnupg2=2.2.40-1.1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.1.dsc' gnupg2_2.2.40-1.1.dsc 3832 SHA256:89bdffd4176066d37fb5d250a1e5512c428529d10f13413a12893f86a757697f
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2' gnupg2_2.2.40.orig.tar.bz2 7301631 SHA256:1164b29a75e8ab93ea15033300149e1872a7ef6bdda3d7c78229a735f8204c28
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2.asc' gnupg2_2.2.40.orig.tar.bz2.asc 228 SHA256:3907dc165299cd53c0b4aec862323c3bce6037c411600ec87dc5eed7a55eba4a
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.1.debian.tar.xz' gnupg2_2.2.40-1.1.debian.tar.xz 62368 SHA256:356b7c86afdbaab286c5b92816cd1e1f4616cb67d22407c616618ef4d1680a9b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.40-1.1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.40-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.40-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.8.1-4`

Binary Packages:

- `libgnutls30:amd64=3.8.1-4+b1`

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
$ apt-get source -qq --print-uris gnutls28=3.8.1-4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.8.1-4.dsc' gnutls28_3.8.1-4.dsc 3231 SHA256:a3dee2df5bea6be410d26e4a73fa2e548cc62b23bfb421decd50fa9d974cb165
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.8.1.orig.tar.xz' gnutls28_3.8.1.orig.tar.xz 6447056 SHA256:ba8b9e15ae20aba88f44661978f5b5863494316fe7e722ede9d069fe6294829c
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.8.1.orig.tar.xz.asc' gnutls28_3.8.1.orig.tar.xz.asc 996 SHA256:3b6357c19431736099929e13ff8340e9ed4b36e4e22b34ae7b46e1f85a1d2884
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.8.1-4.debian.tar.xz' gnutls28_3.8.1-4.debian.tar.xz 69016 SHA256:ec0123f4f50eb89f0708b1d63657d1070ac562cd4be2912c4460a7e526f85a4b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.8.1-4/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.8.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.8.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gobject-introspection=1.78.1-5`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.78.1-5`
- `gir1.2-glib-2.0:amd64=1.78.1-5`
- `libgirepository-1.0-1:amd64=1.78.1-5`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `AFL-2.0`
- `Apache-2.0`
- `Apache-2.0 with LLVM exception`
- `BSD-2-clause`
- `BSD-3-clause-pcre`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `Expat`
- `FSFAP`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `Kuchling-PD`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `MPL-1.1`
- `Plumb-PD`
- `Unicode-DFS-2016`
- `bzip2-1.0.6`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.78.1-5
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.78.1-5.dsc' gobject-introspection_1.78.1-5.dsc 3535 SHA256:1ad9d9be000ad5c70a3c8b4b8340cf57f0c407b38937dd3a7419c24efb38fb6d
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.78.1.orig-glib.tar.xz' gobject-introspection_1.78.1.orig-glib.tar.xz 5327096 SHA256:44eaab8b720877ce303c5540b657b126f12dc94972d9880b52959f43fb537b30
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.78.1.orig.tar.xz' gobject-introspection_1.78.1.orig.tar.xz 1060296 SHA256:bd7babd99af7258e76819e45ba4a6bc399608fe762d83fde3cac033c50841bb4
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.78.1-5.debian.tar.xz' gobject-introspection_1.78.1-5.debian.tar.xz 43960 SHA256:63c578605aa05c812a11ed2c8a0fc070d86f4a3af3b18c4b7db76634f6e66f38
```

Other potentially useful URLs:

- https://sources.debian.net/src/gobject-introspection/1.78.1-5/ (for browsing the source)
- https://sources.debian.net/src/gobject-introspection/1.78.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gobject-introspection/1.78.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `graphite2=1.3.14-1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.14-1`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.1`
- `custom-sil-open-font-license`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.14-1
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.14-1.dsc' graphite2_1.3.14-1.dsc 2608 SHA256:3a622b8aa7d693d6d60d3cd29b49a7d9d7873ea6089cb52ce7a223261e605152
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.14.orig.tar.gz' graphite2_1.3.14.orig.tar.gz 6629829 SHA256:7a3b342c5681921ce2e0c2496509d30b5b078399d5a7bd2358f95166d57d91df
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.14-1.debian.tar.xz' graphite2_1.3.14-1.debian.tar.xz 12068 SHA256:94d584e6c748fa7e2f851c3bb39cb2cdb437b4f91d1d636f3d842357724cd9bd
```

Other potentially useful URLs:

- https://sources.debian.net/src/graphite2/1.3.14-1/ (for browsing the source)
- https://sources.debian.net/src/graphite2/1.3.14-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/graphite2/1.3.14-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.11-3`

Binary Packages:

- `grep=3.11-3`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.11-3
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.11-3.dsc' grep_3.11-3.dsc 1618 SHA256:bd3ec403c9ed5199a7c1009082abf254d8bc8909849de306c7960c37409e3c8d
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.11.orig.tar.xz' grep_3.11.orig.tar.xz 1703776 SHA256:1db2aedde89d0dea42b16d9528f894c8d15dae4e190b59aecc78f5a951276eab
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.11.orig.tar.xz.asc' grep_3.11.orig.tar.xz.asc 833 SHA256:89ec23ffd59b68822732dc8204fc89883c3af30a90ae390feb94346d9d09a589
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.11-3.debian.tar.xz' grep_3.11-3.debian.tar.xz 20592 SHA256:92d9ce74a9d546b7e188e9148979f7762b3e6b8534c7367b749e8766fe4ea097
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.11-3/ (for browsing the source)
- https://sources.debian.net/src/grep/3.11-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.11-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.12-1`

Binary Packages:

- `gzip=1.12-1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.12-1
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12-1.dsc' gzip_1.12-1.dsc 2009 SHA256:49a287787a0b4fc816eb576c011c472d1f630ec1778dfa120bd7fce4a844c253
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12.orig.tar.xz' gzip_1.12.orig.tar.xz 825548 SHA256:ce5e03e519f637e1f814011ace35c4f87b33c0bbabeec35baf5fbd3479e91956
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12.orig.tar.xz.asc' gzip_1.12.orig.tar.xz.asc 833 SHA256:3ed9ab54452576e0be0d477c772c9f47baa36415133fef7dd1fcf7b15480ba32
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12-1.debian.tar.xz' gzip_1.12-1.debian.tar.xz 18736 SHA256:fcf2317e8eeddd66766ec5f3853025b109bd13815ec86ed6563e1af68d17193a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.12-1/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.12-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `harfbuzz=8.0.1-1`

Binary Packages:

- `libharfbuzz0b:amd64=8.0.1-1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `Apache-2.0`
- `CC0-1.0`
- `Expat`
- `FSFAP`
- `FSFUL`
- `FSFULLR`
- `GPL-2`
- `GPL-2+ with AutoConf exception`
- `GPL-2+ with Font exception`
- `GPL-2+ with LibTool exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with AutoConf exception`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `Monotype`
- `OFL-1.1`
- `UFL-1.0`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=8.0.1-1
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_8.0.1-1.dsc' harfbuzz_8.0.1-1.dsc 2542 SHA256:19ed7817867ceff5a76891a6e93635f6228a38b898d95b57a9437460812b0a1c
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_8.0.1.orig.tar.xz' harfbuzz_8.0.1.orig.tar.xz 18792332 SHA256:c1ce780acd385569f25b9a29603d1d5bc71e6940e55bfdd4f7266fad50e42620
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_8.0.1-1.debian.tar.xz' harfbuzz_8.0.1-1.debian.tar.xz 19644 SHA256:2f1d87b00396e8524a4ec2fb4a55cc776b0703788a18e77dffb098da1c2071c6
```

Other potentially useful URLs:

- https://sources.debian.net/src/harfbuzz/8.0.1-1/ (for browsing the source)
- https://sources.debian.net/src/harfbuzz/8.0.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/harfbuzz/8.0.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hicolor-icon-theme=0.17-2`

Binary Packages:

- `hicolor-icon-theme=0.17-2`

Licenses: (parsed from: `/usr/share/doc/hicolor-icon-theme/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris hicolor-icon-theme=0.17-2
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.dsc' hicolor-icon-theme_0.17-2.dsc 2053 SHA256:9df02b466f82cd6fa13930bc197d001ed8ddac1abc7f8dde3db45ed1708336bd
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17.orig.tar.xz' hicolor-icon-theme_0.17.orig.tar.xz 53016 SHA256:317484352271d18cbbcfac3868eab798d67fff1b8402e740baa6ff41d588a9d8
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.debian.tar.xz' hicolor-icon-theme_0.17-2.debian.tar.xz 3536 SHA256:97eec9852a2923b95bd13fc59c30fb1b9063ffd1f8a04748544d4975a84e98f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/hicolor-icon-theme/0.17-2/ (for browsing the source)
- https://sources.debian.net/src/hicolor-icon-theme/0.17-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hicolor-icon-theme/0.17-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hostname=3.23+nmu1`

Binary Packages:

- `hostname=3.23+nmu1`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23+nmu1
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.23%2bnmu1.dsc' hostname_3.23+nmu1.dsc 1281 SHA256:56f2189eaeee638e86d29a05356e7001632e33b2132a41a4634a9ff839264ea6
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.23%2bnmu1.tar.xz' hostname_3.23+nmu1.tar.xz 12876 SHA256:f3fb39f30b00ba7dba2cec013195d7e1bb215f241153208ccd52da3eedfe7a7d
```

Other potentially useful URLs:

- https://sources.debian.net/src/hostname/3.23+nmu1/ (for browsing the source)
- https://sources.debian.net/src/hostname/3.23+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hostname/3.23+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `icu=72.1-4`

Binary Packages:

- `icu-devtools=72.1-4`
- `libicu-dev:amd64=72.1-4`
- `libicu72:amd64=72.1-4`

Licenses: (parsed from: `/usr/share/doc/icu-devtools/copyright`, `/usr/share/doc/libicu-dev/copyright`, `/usr/share/doc/libicu72/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu=72.1-4
'http://deb.debian.org/debian/pool/main/i/icu/icu_72.1-4.dsc' icu_72.1-4.dsc 2252 SHA256:a6c7b8575cf6743674635fde3dca6edc3a3236de07df9f5a19d27dedcda923c2
'http://deb.debian.org/debian/pool/main/i/icu/icu_72.1.orig.tar.gz' icu_72.1.orig.tar.gz 26303933 SHA256:a2d2d38217092a7ed56635e34467f92f976b370e20182ad325edea6681a71d68
'http://deb.debian.org/debian/pool/main/i/icu/icu_72.1.orig.tar.gz.asc' icu_72.1.orig.tar.gz.asc 659 SHA256:87b6ff610d587292cec0444fa8cbbfb12994cb89bade40578f5ba6470de245c7
'http://deb.debian.org/debian/pool/main/i/icu/icu_72.1-4.debian.tar.xz' icu_72.1-4.debian.tar.xz 62456 SHA256:df53fade18c408471c169b1edb569769f3b58edb27db73bfc5bc3a6534f82676
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/72.1-4/ (for browsing the source)
- https://sources.debian.net/src/icu/72.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/72.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `imagemagick=8:6.9.12.98+dfsg1-3`

Binary Packages:

- `imagemagick=8:6.9.12.98+dfsg1-3`
- `imagemagick-6-common=8:6.9.12.98+dfsg1-3`
- `imagemagick-6.q16=8:6.9.12.98+dfsg1-3`
- `libmagickcore-6-arch-config:amd64=8:6.9.12.98+dfsg1-3`
- `libmagickcore-6-headers=8:6.9.12.98+dfsg1-3`
- `libmagickcore-6.q16-7:amd64=8:6.9.12.98+dfsg1-3`
- `libmagickcore-6.q16-7-extra:amd64=8:6.9.12.98+dfsg1-3`
- `libmagickcore-6.q16-dev:amd64=8:6.9.12.98+dfsg1-3`
- `libmagickcore-dev=8:6.9.12.98+dfsg1-3`
- `libmagickwand-6-headers=8:6.9.12.98+dfsg1-3`
- `libmagickwand-6.q16-7:amd64=8:6.9.12.98+dfsg1-3`
- `libmagickwand-6.q16-dev:amd64=8:6.9.12.98+dfsg1-3`
- `libmagickwand-dev=8:6.9.12.98+dfsg1-3`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/libmagickcore-6-arch-config/copyright`, `/usr/share/doc/libmagickcore-6-headers/copyright`, `/usr/share/doc/libmagickcore-6.q16-7/copyright`, `/usr/share/doc/libmagickcore-6.q16-7-extra/copyright`, `/usr/share/doc/libmagickcore-6.q16-dev/copyright`, `/usr/share/doc/libmagickcore-dev/copyright`, `/usr/share/doc/libmagickwand-6-headers/copyright`, `/usr/share/doc/libmagickwand-6.q16-7/copyright`, `/usr/share/doc/libmagickwand-6.q16-dev/copyright`, `/usr/share/doc/libmagickwand-dev/copyright`)

- `Artistic`
- `BSD-with-FSF-change-public-domain`
- `GNU-All-Permissive-License`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL2+-with-Autoconf-Macros-exception`
- `GPL3+-with-Autoconf-Macros-exception`
- `GPL3+-with-Autoconf-Macros-exception-GNU`
- `ImageMagick`
- `ImageMagickLicensePartEZXML`
- `ImageMagickLicensePartFIG`
- `ImageMagickLicensePartGsview`
- `ImageMagickLicensePartOpenSSH`
- `ImageMagickPartGraphicsMagick`
- `ImageMagickPartlibjpeg`
- `ImageMagickPartlibsquish`
- `Imagemagick`
- `LGPL-3`
- `LGPL-3+`
- `Magick++`
- `Makefile-in`
- `Perllikelicence`
- `aclocal`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/imagemagick/8:6.9.12.98+dfsg1-3/


### `dpkg` source package: `imath=3.1.9-3`

Binary Packages:

- `libimath-3-1-29:amd64=3.1.9-3`
- `libimath-dev:amd64=3.1.9-3`
- `python3-imath:amd64=3.1.9-3`

Licenses: (parsed from: `/usr/share/doc/libimath-3-1-29/copyright`, `/usr/share/doc/libimath-dev/copyright`, `/usr/share/doc/python3-imath/copyright`)

- `imath`

Source:

```console
$ apt-get source -qq --print-uris imath=3.1.9-3
'http://deb.debian.org/debian/pool/main/i/imath/imath_3.1.9-3.dsc' imath_3.1.9-3.dsc 2640 SHA256:a5c7d2cc3a0ee533d900e99e3bdcc82064a4fe2ed90db5264c85884ad7cd362b
'http://deb.debian.org/debian/pool/main/i/imath/imath_3.1.9.orig.tar.gz' imath_3.1.9.orig.tar.gz 598497 SHA256:f1d8aacd46afed958babfced3190d2d3c8209b66da451f556abd6da94c165cf3
'http://deb.debian.org/debian/pool/main/i/imath/imath_3.1.9.orig.tar.gz.asc' imath_3.1.9.orig.tar.gz.asc 287 SHA256:a2c4ac5151789903ca8ab3093a2798491463ccf2abfd003a20f96453e505dd5f
'http://deb.debian.org/debian/pool/main/i/imath/imath_3.1.9-3.debian.tar.xz' imath_3.1.9-3.debian.tar.xz 8904 SHA256:ba252109bd0b2d511d2ee1a9e9bc62dd60a9886f10210f08e44aaf262202b626
```

Other potentially useful URLs:

- https://sources.debian.net/src/imath/3.1.9-3/ (for browsing the source)
- https://sources.debian.net/src/imath/3.1.9-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/imath/3.1.9-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `init-system-helpers=1.65.2`

Binary Packages:

- `init-system-helpers=1.65.2`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/init-system-helpers/1.65.2/


### `dpkg` source package: `isl=0.26-3`

Binary Packages:

- `libisl23:amd64=0.26-3`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.26-3
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.26-3.dsc' isl_0.26-3.dsc 1832 SHA256:b943ed41e0d04bd86ea1a9a10e49a0ac1996ac534b67b968df4320880ec6e6e7
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.26.orig.tar.xz' isl_0.26.orig.tar.xz 2035560 SHA256:a0b5cb06d24f9fa9e77b55fabbe9a3c94a336190345c2555f9915bb38e976504
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.26-3.debian.tar.xz' isl_0.26-3.debian.tar.xz 24700 SHA256:c4a9367d892a12da46c54cbf6475f447e137ac3eff857baa91af94c99daed0a5
```

Other potentially useful URLs:

- https://sources.debian.net/src/isl/0.26-3/ (for browsing the source)
- https://sources.debian.net/src/isl/0.26-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/isl/0.26-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jansson=2.14-2`

Binary Packages:

- `libjansson4:amd64=2.14-2`

Licenses: (parsed from: `/usr/share/doc/libjansson4/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris jansson=2.14-2
'http://deb.debian.org/debian/pool/main/j/jansson/jansson_2.14-2.dsc' jansson_2.14-2.dsc 1980 SHA256:6296ddd9c0a022bd1b70074aefb171cfcdf5694a04ffd32b35fd66097621af87
'http://deb.debian.org/debian/pool/main/j/jansson/jansson_2.14.orig.tar.gz' jansson_2.14.orig.tar.gz 141500 SHA256:c739578bf6b764aa0752db9a2fdadcfe921c78f1228c7ec0bb47fa804c55d17b
'http://deb.debian.org/debian/pool/main/j/jansson/jansson_2.14-2.debian.tar.xz' jansson_2.14-2.debian.tar.xz 5428 SHA256:e89fe4fd8221f6934ddb50f2e7f8404311928d0e23e49a5599f3d3d14ee8cb88
```

Other potentially useful URLs:

- https://sources.debian.net/src/jansson/2.14-2/ (for browsing the source)
- https://sources.debian.net/src/jansson/2.14-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jansson/2.14-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jbigkit=2.1-6.1`

Binary Packages:

- `libjbig-dev:amd64=2.1-6.1`
- `libjbig0:amd64=2.1-6.1`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-6.1
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1-6.1.dsc' jbigkit_2.1-6.1.dsc 2089 SHA256:8dea586c47cb4b2436f77fd33ef4a702b9da936d74de8332a72a8ddbe8124e09
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1-6.1.debian.tar.xz' jbigkit_2.1-6.1.debian.tar.xz 9244 SHA256:c9ba99e84d18b1affdc97b26b625721ed06b41a92996d9b426b62c0dbe3868cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/jbigkit/2.1-6.1/ (for browsing the source)
- https://sources.debian.net/src/jbigkit/2.1-6.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jbigkit/2.1-6.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.6.3-2`

Binary Packages:

- `libkeyutils1:amd64=1.6.3-2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.3-2
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3-2.dsc' keyutils_1.6.3-2.dsc 2079 SHA256:77e6f0e5018f0f6cfb5a3689d7f185a014b2437d0a097609ffda32bfd3a64f28
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3.orig.tar.gz' keyutils_1.6.3.orig.tar.gz 137022 SHA256:a61d5706136ae4c05bd48f86186bcfdbd88dd8bd5107e3e195c924cfc1b39bb4
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3-2.debian.tar.xz' keyutils_1.6.3-2.debian.tar.xz 13196 SHA256:9b9b40729465d4895860838e82e13d2ee4ffc44a97c9acd1d47a51bd33ade899
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.6.3-2/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.6.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.6.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.20.1-5`

Binary Packages:

- `krb5-multidev:amd64=1.20.1-5`
- `libgssapi-krb5-2:amd64=1.20.1-5`
- `libgssrpc4:amd64=1.20.1-5`
- `libk5crypto3:amd64=1.20.1-5`
- `libkadm5clnt-mit12:amd64=1.20.1-5`
- `libkadm5srv-mit12:amd64=1.20.1-5`
- `libkdb5-10:amd64=1.20.1-5`
- `libkrb5-3:amd64=1.20.1-5`
- `libkrb5-dev:amd64=1.20.1-5`
- `libkrb5support0:amd64=1.20.1-5`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit12/copyright`, `/usr/share/doc/libkadm5srv-mit12/copyright`, `/usr/share/doc/libkdb5-10/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20.1-5
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20.1-5.dsc' krb5_1.20.1-5.dsc 3304 SHA256:014d2e50cd3fe911c1499bb203f63ddd3b9f306650451bfb1d8c33d7449a6b10
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz' krb5_1.20.1.orig.tar.gz 8661660 SHA256:704aed49b19eb5a7178b34b2873620ec299db08752d6a8574f95d41879ab8851
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz.asc' krb5_1.20.1.orig.tar.gz.asc 833 SHA256:2afeec5dbc586cc40b7975645e02b4c41c4d719dd02213e828c72d8239d55666
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20.1-5.debian.tar.xz' krb5_1.20.1-5.debian.tar.xz 104484 SHA256:aba9f1047af6733679eeffd2ff9dae6ede5089f8f57e8b1117a9ac935b136105
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.20.1-5/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.20.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.20.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lapack=3.11.0-2`

Binary Packages:

- `libblas3:amd64=3.11.0-2`
- `liblapack3:amd64=3.11.0-2`

Licenses: (parsed from: `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.11.0-2
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.11.0-2.dsc' lapack_3.11.0-2.dsc 3307 SHA256:664d828b9015f9d7db00dd53d42ee7ae0b30e90725fa5300fce35a833ecd5ecf
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.11.0.orig.tar.gz' lapack_3.11.0.orig.tar.gz 7723808 SHA256:4b9ba79bfd4921ca820e83979db76ab3363155709444a787979e81c22285ffa9
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.11.0-2.debian.tar.xz' lapack_3.11.0-2.debian.tar.xz 32936 SHA256:36825c7cb768267fe7d322145a4160d4e564a21730b16d78a59090102cc35dfd
```

Other potentially useful URLs:

- https://sources.debian.net/src/lapack/3.11.0-2/ (for browsing the source)
- https://sources.debian.net/src/lapack/3.11.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lapack/3.11.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.14-2`

Binary Packages:

- `liblcms2-2:amd64=2.14-2`
- `liblcms2-dev:amd64=2.14-2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `IJG`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.14-2
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.14-2.dsc' lcms2_2.14-2.dsc 1944 SHA256:65d7bd751c1dd0d0b70eaeb3a743849d19446b454c7bcf736de194e047784934
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.14.orig.tar.gz' lcms2_2.14.orig.tar.gz 7406694 SHA256:28474ea6f6591c4d4cee972123587001a4e6e353412a41b3e9e82219818d5740
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.14-2.debian.tar.xz' lcms2_2.14-2.debian.tar.xz 11728 SHA256:06ce5d9b473dce422f2387c2e18d646b7f639deae10e5a80bb2e4c5e45f1f6b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.14-2/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.14-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.14-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lerc=4.0.0+ds-3`

Binary Packages:

- `liblerc-dev:amd64=4.0.0+ds-3`
- `liblerc4:amd64=4.0.0+ds-3`

Licenses: (parsed from: `/usr/share/doc/liblerc-dev/copyright`, `/usr/share/doc/liblerc4/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris lerc=4.0.0+ds-3
'http://deb.debian.org/debian/pool/main/l/lerc/lerc_4.0.0%2bds-3.dsc' lerc_4.0.0+ds-3.dsc 2638 SHA256:49d68994f4570a72d781914aecdbfd0cb2a40b2c9dd81344f9517d97643f9c57
'http://deb.debian.org/debian/pool/main/l/lerc/lerc_4.0.0%2bds.orig.tar.xz' lerc_4.0.0+ds.orig.tar.xz 348140 SHA256:acf855502fd3b950ee78f0b67bc9e9b39316b3526fbf6d8b8b1a9482fb756723
'http://deb.debian.org/debian/pool/main/l/lerc/lerc_4.0.0%2bds-3.debian.tar.xz' lerc_4.0.0+ds-3.debian.tar.xz 8024 SHA256:1d6ed278a6dde4f7c703a77d4e9fab10dcf1b61881572a8da4f2103b2ee4da65
```

Other potentially useful URLs:

- https://sources.debian.net/src/lerc/4.0.0+ds-3/ (for browsing the source)
- https://sources.debian.net/src/lerc/4.0.0+ds-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lerc/4.0.0+ds-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.5.6-1`

Binary Packages:

- `libassuan0:amd64=2.5.6-1`

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
$ apt-get source -qq --print-uris libassuan=2.5.6-1
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.6-1.dsc' libassuan_2.5.6-1.dsc 1997 SHA256:5216dd7bca769143cf39673b018a11b2601fde867fd4b62226088bb9177415b5
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.6.orig.tar.bz2' libassuan_2.5.6.orig.tar.bz2 577012 SHA256:e9fd27218d5394904e4e39788f9b1742711c3e6b41689a31aa3380bd5aa4f426
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.6.orig.tar.bz2.asc' libassuan_2.5.6.orig.tar.bz2.asc 228 SHA256:a1be6f5611de2f563a904c539e0415dd5823d9e1c4c0c1071418e7412174eaea
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.6-1.debian.tar.xz' libassuan_2.5.6-1.debian.tar.xz 14284 SHA256:58a3077b2ecda637de25f54320a3ad2087a250f6f8118271ea22968a4e994ca7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.6-1/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.11.7-4`

Binary Packages:

- `libbsd0:amd64=0.11.7-4`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
- `BSD-3-clause-Regents`
- `BSD-3-clause-author`
- `BSD-4-clause-Niels-Provos`
- `Beerware`
- `Expat`
- `ISC`
- `ISC-Original`
- `libutil-David-Nugent`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.11.7-4
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7-4.dsc' libbsd_0.11.7-4.dsc 2350 SHA256:55e06d162bbcadc897886811e5656835fa58f9149d31d63244bb83187d1fbce5
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz' libbsd_0.11.7.orig.tar.xz 418508 SHA256:9baa186059ebbf25c06308e9f991fda31f7183c0f24931826d83aa6abd8a0261
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz.asc' libbsd_0.11.7.orig.tar.xz.asc 833 SHA256:b470d3fa5ad6948de7a85891e652970828f26eb7057028d57b94fa8644af934a
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7-4.debian.tar.xz' libbsd_0.11.7-4.debian.tar.xz 21596 SHA256:fe83e1418016393b1f39febbde49311f940b74650d1eceb12a7c5857c47ac716
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.11.7-4/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.11.7-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.11.7-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.8.3-1`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1+b3`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.8.3-1
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1.dsc' libcap-ng_0.8.3-1.dsc 1634 SHA256:1bf38dbc0c30bcbc776d2d5c25e31d89202de0858f9ca9379c993d55103d7ef0
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3.orig.tar.gz' libcap-ng_0.8.3.orig.tar.gz 455383 SHA256:bed6f6848e22bb2f83b5f764b2aef0ed393054e803a8e3a8711cb2a39e6b492d
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1.debian.tar.xz' libcap-ng_0.8.3-1.debian.tar.xz 10488 SHA256:710577902c260f50f8cfc9d7e264131f880eab0581d12ceab17ebe48e2ac53c6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap-ng/0.8.3-1/ (for browsing the source)
- https://sources.debian.net/src/libcap-ng/0.8.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap-ng/0.8.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap2=1:2.66-4`

Binary Packages:

- `libcap2:amd64=1:2.66-4`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.66-4
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.66-4.dsc' libcap2_2.66-4.dsc 2204 SHA256:ab4aaa349c824acaebfb63bec2d2bc10e7cee10ec6725ac6f21f1fe12aa9d8fb
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.66.orig.tar.xz' libcap2_2.66.orig.tar.xz 181592 SHA256:15c40ededb3003d70a283fe587a36b7d19c8b3b554e33f86129c059a4bb466b2
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.66-4.debian.tar.xz' libcap2_2.66-4.debian.tar.xz 21468 SHA256:5379eec3a05e40c2485ebe451506883c1f2f99d552c6ded29607080fd278dd7c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.66-4/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.66-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.66-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcbor=0.10.2-1.1`

Binary Packages:

- `libcbor0.10:amd64=0.10.2-1.1`

Licenses: (parsed from: `/usr/share/doc/libcbor0.10/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.10.2-1.1
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.10.2-1.1.dsc' libcbor_0.10.2-1.1.dsc 1761 SHA256:02961a5d969749a46e3d241478801b762b6e5472c7968ee848dd29dbfd87a126
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.10.2.orig.tar.gz' libcbor_0.10.2.orig.tar.gz 289450 SHA256:e75f712215d7b7e5c89ef322a09b701f7159f028b8b48978865725f00f79875b
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.10.2-1.1.debian.tar.xz' libcbor_0.10.2-1.1.debian.tar.xz 4304 SHA256:a666c4c1ef4e948c45d0b910c40ae898b29c259569ee6579f85295172b533374
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcbor/0.10.2-1.1/ (for browsing the source)
- https://sources.debian.net/src/libcbor/0.10.2-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcbor/0.10.2-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdatrie=0.2.13-2`

Binary Packages:

- `libdatrie1:amd64=0.2.13-2+b1`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.13-2
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.13-2.dsc' libdatrie_0.2.13-2.dsc 2239 SHA256:d359689deccfa654ab844d6e955fff5e826d9a5dc9a74408d1b6a095f78ab0e5
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.13.orig.tar.xz' libdatrie_0.2.13.orig.tar.xz 314072 SHA256:12231bb2be2581a7f0fb9904092d24b0ed2a271a16835071ed97bed65267f4be
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.13-2.debian.tar.xz' libdatrie_0.2.13-2.debian.tar.xz 9604 SHA256:3f341eb067c5365345e0a416a3c835a8e785c3220aca27c8fb2a01499d0214e9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdatrie/0.2.13-2/ (for browsing the source)
- https://sources.debian.net/src/libdatrie/0.2.13-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdatrie/0.2.13-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libde265=1.0.12-2`

Binary Packages:

- `libde265-0:amd64=1.0.12-2`

Licenses: (parsed from: `/usr/share/doc/libde265-0/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `other-1`
- `public-domain-1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libde265/1.0.12-2/


### `dpkg` source package: `libdeflate=1.18-1`

Binary Packages:

- `libdeflate-dev:amd64=1.18-1`
- `libdeflate0:amd64=1.18-1`

Licenses: (parsed from: `/usr/share/doc/libdeflate-dev/copyright`, `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.18-1
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.18-1.dsc' libdeflate_1.18-1.dsc 2196 SHA256:a5c2eb47274cb08515906097b8e8bac5db6bef9046741669a635efdedc3998f4
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.18.orig.tar.gz' libdeflate_1.18.orig.tar.gz 184924 SHA256:225d982bcaf553221c76726358d2ea139bb34913180b20823c782cede060affd
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.18-1.debian.tar.xz' libdeflate_1.18-1.debian.tar.xz 4756 SHA256:0a570e79b9fe0377fcf26888b1e5160779dfcfe6cf069892796016c2958eac0f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdeflate/1.18-1/ (for browsing the source)
- https://sources.debian.net/src/libdeflate/1.18-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdeflate/1.18-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20230828-1`

Binary Packages:

- `libedit2:amd64=3.1-20230828-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20230828-1
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20230828-1.dsc' libedit_3.1-20230828-1.dsc 2267 SHA256:568783d99f719055b4b4705d85be7349578d32eb73ad9da6347691bf7bd5f298
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20230828.orig.tar.gz' libedit_3.1-20230828.orig.tar.gz 534072 SHA256:4ee8182b6e569290e7d1f44f0f78dac8716b35f656b76528f699c69c98814dad
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20230828-1.debian.tar.xz' libedit_3.1-20230828-1.debian.tar.xz 16624 SHA256:8d94a472a1ddee433c61c2801405164780085044d1432c949666355abed9362d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20230828-1/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20230828-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20230828-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liberror-perl=0.17029-2`

Binary Packages:

- `liberror-perl=0.17029-2`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17029-2
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029-2.dsc' liberror-perl_0.17029-2.dsc 2085 SHA256:48c6ca66e03144a8bec4f32b2419f34d70e8a00500b01ea3bb6a5cab0c03e164
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA256:1a23f7913032aed6d4b68321373a3899ca66590f4727391a091ec19c95bf7adc
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029-2.debian.tar.xz' liberror-perl_0.17029-2.debian.tar.xz 4608 SHA256:60deb5d5cbc4b478f8db4cfa0ac6c512e85eea5fcd7fc7285c26a9942d3b8b67
```

Other potentially useful URLs:

- https://sources.debian.net/src/liberror-perl/0.17029-2/ (for browsing the source)
- https://sources.debian.net/src/liberror-perl/0.17029-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liberror-perl/0.17029-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libevent=2.1.12-stable-8`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.12-stable-8`
- `libevent-core-2.1-7:amd64=2.1.12-stable-8`
- `libevent-dev=2.1.12-stable-8`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-8`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-8`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-8`

Licenses: (parsed from: `/usr/share/doc/libevent-2.1-7/copyright`, `/usr/share/doc/libevent-core-2.1-7/copyright`, `/usr/share/doc/libevent-dev/copyright`, `/usr/share/doc/libevent-extra-2.1-7/copyright`, `/usr/share/doc/libevent-openssl-2.1-7/copyright`, `/usr/share/doc/libevent-pthreads-2.1-7/copyright`)

- `BSD-2-clause`
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
$ apt-get source -qq --print-uris libevent=2.1.12-stable-8
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.12-stable-8.dsc' libevent_2.1.12-stable-8.dsc 2356 SHA256:a2821f5bf8adacd775317ae6a85d19097a2043ba5206fcf840387f4a2da5a2c5
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA256:92e6de1be9ec176428fd2367677e61ceffc2ee1cb119035037a27d346b0403bb
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.12-stable-8.debian.tar.xz' libevent_2.1.12-stable-8.debian.tar.xz 17632 SHA256:5faf34177d3f232853b411fa324b59874eda3010de9809cf4277bcc4a0a554c1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libevent/2.1.12-stable-8/ (for browsing the source)
- https://sources.debian.net/src/libevent/2.1.12-stable-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libevent/2.1.12-stable-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libexif=0.6.24-1`

Binary Packages:

- `libexif-dev:amd64=0.6.24-1+b1`
- `libexif12:amd64=0.6.24-1+b1`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.24-1
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.24-1.dsc' libexif_0.6.24-1.dsc 2116 SHA256:81f5fa53f45e786ed0b2bdf4b94c25d6b25eafda7ab15ce47e94501a276ff93d
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.24.orig.tar.gz' libexif_0.6.24.orig.tar.gz 1140079 SHA256:d3fb7c47829ec4d2def39aa38f4c35a0891763448a05dbf216a329a12bf198f9
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.24-1.debian.tar.xz' libexif_0.6.24-1.debian.tar.xz 11720 SHA256:9f0aca42c1221865ce4c0738301d5e0e99ff2ebed7e3bbbcce7e68605b991784
```

Other potentially useful URLs:

- https://sources.debian.net/src/libexif/0.6.24-1/ (for browsing the source)
- https://sources.debian.net/src/libexif/0.6.24-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libexif/0.6.24-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.4.4-1`

Binary Packages:

- `libffi-dev:amd64=3.4.4-1`
- `libffi8:amd64=3.4.4-1`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi8/copyright`)

- `Expat`
- `GPL`
- `GPL-2+`
- `GPL-3+`
- `LGPL-2.1+`
- `MPL-1.1`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.4-1
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.4-1.dsc' libffi_3.4.4-1.dsc 1951 SHA256:21c9ef156b6766535cb014e0765142c8104ffbcd73f003ecfa80cfb314baa4f0
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.4.orig.tar.gz' libffi_3.4.4.orig.tar.gz 1362394 SHA256:d66c56ad259a82cf2a9dfc408b32bf5da52371500b84745f7fb8b645712df676
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.4-1.debian.tar.xz' libffi_3.4.4-1.debian.tar.xz 10380 SHA256:161b210bfd2ada0b15b0d2a2a98ffc779cd4a68661a7fdf46f61732493db0895
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.4.4-1/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.4.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.4.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libfido2=1.13.0-1`

Binary Packages:

- `libfido2-1:amd64=1.13.0-1+b1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libfido2/1.13.0-1/


### `dpkg` source package: `libgcrypt20=1.10.2-3`

Binary Packages:

- `libgcrypt20:amd64=1.10.2-3`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.2-3
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2-3.dsc' libgcrypt20_1.10.2-3.dsc 2799 SHA256:fb0d993a060bd43f39fd978522bb6506731c0fe633179206aa21411f56575c32
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2.orig.tar.bz2' libgcrypt20_1.10.2.orig.tar.bz2 3795164 SHA256:3b9c02a004b68c256add99701de00b383accccf37177e0d6c58289664cce0c03
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2.orig.tar.bz2.asc' libgcrypt20_1.10.2.orig.tar.bz2.asc 228 SHA256:3b5b729d3969b3e828acc483709a686678cecaf20e8559eb525da905c7aa2bcb
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2-3.debian.tar.xz' libgcrypt20_1.10.2-3.debian.tar.xz 36016 SHA256:126314acd71a9d856c998bf01898059e4ab1860ce8359d1dc7ed50540776b414
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.10.2-3/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.10.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.10.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.47-2`

Binary Packages:

- `libgpg-error0:amd64=1.47-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libgpg-error/1.47-2/


### `dpkg` source package: `libheif=1.17.1-1`

Binary Packages:

- `libheif-plugin-dav1d:amd64=1.17.1-1+b1`
- `libheif-plugin-libde265:amd64=1.17.1-1+b1`
- `libheif1:amd64=1.17.1-1+b1`

Licenses: (parsed from: `/usr/share/doc/libheif-plugin-dav1d/copyright`, `/usr/share/doc/libheif-plugin-libde265/copyright`, `/usr/share/doc/libheif1/copyright`)

- `BOOST-1.0`
- `BSD-3-clause`
- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libheif=1.17.1-1
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.17.1-1.dsc' libheif_1.17.1-1.dsc 3416 SHA256:e9079cc228400c6a61d75a863519a7df3048144e9f5c5ec42a1eee68860c4b43
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.17.1.orig.tar.gz' libheif_1.17.1.orig.tar.gz 1430684 SHA256:97d74c58a346887c1bbf98dcf0322c13b728286153d0f1be2b350f7107e49dba
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.17.1-1.debian.tar.xz' libheif_1.17.1-1.debian.tar.xz 9340 SHA256:a17bd22714882206a8405ebd8ab1f1248fe5fffef50d0aa6f3f5e7518065e05f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libheif/1.17.1-1/ (for browsing the source)
- https://sources.debian.net/src/libheif/1.17.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libheif/1.17.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libice=2:1.0.10-1`

Binary Packages:

- `libice-dev:amd64=2:1.0.10-1`
- `libice6:amd64=2:1.0.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.10-1
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.10-1.dsc' libice_1.0.10-1.dsc 2049 SHA256:adb7b4e250db838a476a44b5a941c8f935ac2b20858186f09228cd3e0696034d
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.10.orig.tar.gz' libice_1.0.10.orig.tar.gz 481960 SHA256:1116bc64c772fd127a0d0c0ffa2833479905e3d3d8197740b3abd5f292f22d2d
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.10-1.diff.gz' libice_1.0.10-1.diff.gz 11349 SHA256:d186b3877416a7e80f1923fe2fc736d576e585a41450bcf4cd5e74f9dd099362
```

Other potentially useful URLs:

- https://sources.debian.net/src/libice/2:1.0.10-1/ (for browsing the source)
- https://sources.debian.net/src/libice/2:1.0.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libice/2:1.0.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn2=2.3.4-1`

Binary Packages:

- `libidn2-0:amd64=2.3.4-1+b1`

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
$ apt-get source -qq --print-uris libidn2=2.3.4-1
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.4-1.dsc' libidn2_2.3.4-1.dsc 1915 SHA256:b7c1c506ea6691c9481176171490c3fde53ef8e51e1a28fb1d4e19dda61f7d59
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.4.orig.tar.gz' libidn2_2.3.4.orig.tar.gz 2083823 SHA256:93caba72b4e051d1f8d4f5a076ab63c99b77faee019b72b9783b267986dbb45f
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.4.orig.tar.gz.asc' libidn2_2.3.4.orig.tar.gz.asc 228 SHA256:c55c8cd14f398186407808f188ed5325faa01a62d88e79bb700bd8c839f75ceb
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.4-1.debian.tar.xz' libidn2_2.3.4-1.debian.tar.xz 16024 SHA256:a928219502f43e337aa3476098b96a250776d9be0b92255bd701c7fee572df68
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.3.4-1/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libjpeg-turbo=1:2.1.5-2`

Binary Packages:

- `libjpeg-dev:amd64=1:2.1.5-2`
- `libjpeg62-turbo:amd64=1:2.1.5-2`
- `libjpeg62-turbo-dev:amd64=1:2.1.5-2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3-clause`
- `BSD-BY-LC-NE`
- `Expat`
- `NTP`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:2.1.5-2
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5-2.dsc' libjpeg-turbo_2.1.5-2.dsc 2493 SHA256:d718ead0dfbcbc8523665c02a7f7152e31039ded641d022868722623bb3b486d
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5.orig.tar.gz' libjpeg-turbo_2.1.5.orig.tar.gz 2264471 SHA256:254f3642b04e309fee775123133c6464181addc150499561020312ec61c1bf7c
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5-2.debian.tar.xz' libjpeg-turbo_2.1.5-2.debian.tar.xz 107768 SHA256:cdb2433c2f7101345c1ffa14efb943787c675b86354691a32490845fe4bc9237
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:2.1.5-2/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:2.1.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:2.1.5-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libksba=1.6.4-2`

Binary Packages:

- `libksba8:amd64=1.6.4-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.4-2
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.4-2.dsc' libksba_1.6.4-2.dsc 2482 SHA256:0fa874c62277bc3183824ab4abfddf37ebd2bc59c3595a8f2fb8d8313fba606f
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.4.orig.tar.bz2' libksba_1.6.4.orig.tar.bz2 668445 SHA256:bbb43f032b9164d86c781ffe42213a83bf4f2fee91455edfa4654521b8b03b6b
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.4.orig.tar.bz2.asc' libksba_1.6.4.orig.tar.bz2.asc 228 SHA256:f6e892a76842f81955f369f628386f5657cdcf4cc3b1b7d911d1168d773e7d87
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.4-2.debian.tar.xz' libksba_1.6.4-2.debian.tar.xz 14652 SHA256:45fed2acfff4735fdb5404e8597f9d129e3ef5500bf656f2c113097d64755493
```

Other potentially useful URLs:

- https://sources.debian.net/src/libksba/1.6.4-2/ (for browsing the source)
- https://sources.debian.net/src/libksba/1.6.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libksba/1.6.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liblqr=0.4.2-2.1`

Binary Packages:

- `liblqr-1-0:amd64=0.4.2-2.1`
- `liblqr-1-0-dev:amd64=0.4.2-2.1`

Licenses: (parsed from: `/usr/share/doc/liblqr-1-0/copyright`, `/usr/share/doc/liblqr-1-0-dev/copyright`)

- `GPL-3`
- `GPLv3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris liblqr=0.4.2-2.1
'http://deb.debian.org/debian/pool/main/libl/liblqr/liblqr_0.4.2-2.1.dsc' liblqr_0.4.2-2.1.dsc 2095 SHA256:c54c34cd2f7470a29366eeacde2ca4859a97d684a406fb81a918b970c01d617c
'http://deb.debian.org/debian/pool/main/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA256:d4c22373432cca749e4326cd41fce365e6ff857c0bfd7a5302b8eb34b69f0336
'http://deb.debian.org/debian/pool/main/libl/liblqr/liblqr_0.4.2-2.1.debian.tar.xz' liblqr_0.4.2-2.1.debian.tar.xz 5300 SHA256:284a002f1ecac63ac17b1aafbb230da9ce7bd9efe2d5b94e8cad49b607eb2564
```

Other potentially useful URLs:

- https://sources.debian.net/src/liblqr/0.4.2-2.1/ (for browsing the source)
- https://sources.debian.net/src/liblqr/0.4.2-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liblqr/0.4.2-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmaxminddb=1.8.0-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.8.0-1`
- `libmaxminddb0:amd64=1.8.0-1`

Licenses: (parsed from: `/usr/share/doc/libmaxminddb-dev/copyright`, `/usr/share/doc/libmaxminddb0/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `CC-BY-SA-3.0`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmaxminddb=1.8.0-1
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.8.0-1.dsc' libmaxminddb_1.8.0-1.dsc 2322 SHA256:812eb5aff4c4644e2b0e1a66ec2c0a01f6bdf3fed96bc8354cd3d7e6a115193c
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.8.0.orig.tar.gz' libmaxminddb_1.8.0.orig.tar.gz 243661 SHA256:6d0d060534f3a82ee58ba1563008af0926ed4b6ff42d1df5783b6b3918251a95
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.8.0-1.debian.tar.xz' libmaxminddb_1.8.0-1.debian.tar.xz 12472 SHA256:1e1729a1adcaee998880932fd921729f097dec471645a31279c027bf2c64ce0c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmaxminddb/1.8.0-1/ (for browsing the source)
- https://sources.debian.net/src/libmaxminddb/1.8.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmaxminddb/1.8.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmd=1.1.0-1`

Binary Packages:

- `libmd0:amd64=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libmd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-3-clause`
- `BSD-3-clause-Aaron-D-Gifford`
- `Beerware`
- `ISC`
- `public-domain-md4`
- `public-domain-md5`
- `public-domain-sha1`

Source:

```console
$ apt-get source -qq --print-uris libmd=1.1.0-1
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0-1.dsc' libmd_1.1.0-1.dsc 2283 SHA256:abb74aa06e06dbb88f4c1a7764e1d93c753bdcb60e7151a1897fe247750f5ef1
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0.orig.tar.xz' libmd_1.1.0.orig.tar.xz 271228 SHA256:1bd6aa42275313af3141c7cf2e5b964e8b1fd488025caf2f971f43b00776b332
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0.orig.tar.xz.asc' libmd_1.1.0.orig.tar.xz.asc 833 SHA256:402fd3024e43ab975733d09e661804a58ca58697194e4b15216b1217cfe1dadb
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0-1.debian.tar.xz' libmd_1.1.0-1.debian.tar.xz 8156 SHA256:4e9403dcdd277ae81bb83bc7f4ba9fe5fd6640b74118d8349904f029510596dc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmd/1.1.0-1/ (for browsing the source)
- https://sources.debian.net/src/libmd/1.1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmd/1.1.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libnsl=1.3.0-3`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-3`
- `libnsl2:amd64=1.3.0-3`

Licenses: (parsed from: `/usr/share/doc/libnsl-dev/copyright`, `/usr/share/doc/libnsl2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+-autoconf-exception`
- `GPL-2+-libtool-exception`
- `GPL-3`
- `GPL-3+-autoconf-exception`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `permissive-autoconf-m4`
- `permissive-autoconf-m4-no-warranty`
- `permissive-configure`
- `permissive-fsf`
- `permissive-makefile-in`

Source:

```console
$ apt-get source -qq --print-uris libnsl=1.3.0-3
'http://deb.debian.org/debian/pool/main/libn/libnsl/libnsl_1.3.0-3.dsc' libnsl_1.3.0-3.dsc 1955 SHA256:32ef29339eb7aa7aa8a150d4c71592475fdefc0cc45509b517f470dbdd88b371
'http://deb.debian.org/debian/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA256:eac3062957fa302c62eff4aed718a07bacbf9ceb0a058289f12a19bfdda3c8e2
'http://deb.debian.org/debian/pool/main/libn/libnsl/libnsl_1.3.0-3.debian.tar.xz' libnsl_1.3.0-3.debian.tar.xz 4748 SHA256:a9172c5b27236cae278effdbe74447bdb2536afea8ad4c2a44d9661e02ae2d89
```

Other potentially useful URLs:

- https://sources.debian.net/src/libnsl/1.3.0-3/ (for browsing the source)
- https://sources.debian.net/src/libnsl/1.3.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libnsl/1.3.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng1.6=1.6.40-2`

Binary Packages:

- `libpng-dev:amd64=1.6.40-2`
- `libpng16-16:amd64=1.6.40-2`

Licenses: (parsed from: `/usr/share/doc/libpng-dev/copyright`, `/usr/share/doc/libpng16-16/copyright`)

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
$ apt-get source -qq --print-uris libpng1.6=1.6.40-2
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.40-2.dsc' libpng1.6_1.6.40-2.dsc 2241 SHA256:894dacfee1ea43139751269eec9d94bb74b9a8dd7ea9d8aec0a2b0c81d7e43d0
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.40.orig.tar.gz' libpng1.6_1.6.40.orig.tar.gz 1520834 SHA256:62d25af25e636454b005c93cae51ddcd5383c40fa14aa3dae8f6576feb5692c2
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.40-2.debian.tar.xz' libpng1.6_1.6.40-2.debian.tar.xz 31148 SHA256:542a1c4abae513369b18f4399aa95f653b17739f711d668802c338a989e6c0f6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpng1.6/1.6.40-2/ (for browsing the source)
- https://sources.debian.net/src/libpng1.6/1.6.40-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpng1.6/1.6.40-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpsl=0.21.2-1`

Binary Packages:

- `libpsl5:amd64=0.21.2-1+b1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`
- `gnulib`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.2-1
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.21.2-1.dsc' libpsl_0.21.2-1.dsc 1622 SHA256:1ddb578f5865a447b11078993cef2138107c82f8590ec2516af6f9970a2d4e0f
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.21.2.orig.tar.xz' libpsl_0.21.2.orig.tar.xz 1870352 SHA256:11e34380f2c81d6e72c710464aae3b680df4ddcc1007826c630fb03c7ca6aa54
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.21.2-1.debian.tar.xz' libpsl_0.21.2-1.debian.tar.xz 11940 SHA256:78327367c83ce2dc6a8404f479a7589eacb0266f1d4a25619d5f6f00f98ab7b6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpsl/0.21.2-1/ (for browsing the source)
- https://sources.debian.net/src/libpsl/0.21.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpsl/0.21.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpthread-stubs=0.4-1`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.4-1
'http://deb.debian.org/debian/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.dsc' libpthread-stubs_0.4-1.dsc 1927 SHA256:8923683ac365475d2cc515e5f16f4adc8bd8e37453e1a2a6bedeb9246922829f
'http://deb.debian.org/debian/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4.orig.tar.gz' libpthread-stubs_0.4.orig.tar.gz 71252 SHA256:50d5686b79019ccea08bcbd7b02fe5a40634abcfd4146b6e75c6420cc170e9d9
'http://deb.debian.org/debian/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.diff.gz' libpthread-stubs_0.4-1.diff.gz 2346 SHA256:ec435ba2852ad4b0522010943a5b7d39fc7e088067367879778cf10e57f5cc3f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpthread-stubs/0.4-1/ (for browsing the source)
- https://sources.debian.net/src/libpthread-stubs/0.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpthread-stubs/0.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libraw=0.21.1-7`

Binary Packages:

- `libraw23:amd64=0.21.1-7`

Licenses: (parsed from: `/usr/share/doc/libraw23/copyright`)

- `CC-BY-SA-3.0`
- `CDDL-1.0`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libraw=0.21.1-7
'http://deb.debian.org/debian/pool/main/libr/libraw/libraw_0.21.1-7.dsc' libraw_0.21.1-7.dsc 2339 SHA256:4456052d940f8d1483a7310611245dfd42bdaa0d3208913d565f245b2dbc31e9
'http://deb.debian.org/debian/pool/main/libr/libraw/libraw_0.21.1.orig.tar.gz' libraw_0.21.1.orig.tar.gz 564541 SHA256:b63d7ffa43463f74afcc02f9083048c231349b41cc9255dec0840cf8a67b52e0
'http://deb.debian.org/debian/pool/main/libr/libraw/libraw_0.21.1-7.debian.tar.xz' libraw_0.21.1-7.debian.tar.xz 24252 SHA256:fbfac8b2f9289f2262d207131a140bddde0448456396bddb7679856415477168
```

Other potentially useful URLs:

- https://sources.debian.net/src/libraw/0.21.1-7/ (for browsing the source)
- https://sources.debian.net/src/libraw/0.21.1-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libraw/0.21.1-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `librsvg=2.54.7+dfsg-2`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.54.7+dfsg-2`
- `librsvg2-2:amd64=2.54.7+dfsg-2`
- `librsvg2-common:amd64=2.54.7+dfsg-2`
- `librsvg2-dev:amd64=2.54.7+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `0BSD`
- `0BSD,`
- `Apache-2.0`
- `Apache-2.0,`
- `BSD-2-clause`
- `BSD-2-clause,`
- `BSD-3-clause`
- `BSD-3-clause,`
- `Boost-1.0`
- `Boost-1.0,`
- `CC-BY-3.0`
- `CC-zero-waive-1.0-us`
- `Expat`
- `Expat,`
- `FSFAP`
- `LGPL-2`
- `LGPL-2+`
- `MPL-2.0`
- `MPL-2.0,`
- `OFL-1.1`
- `Sun-permissive`
- `Sun-permissive,`
- `Unlicense`
- `Unlicense,`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.54.7+dfsg-2
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.54.7%2bdfsg-2.dsc' librsvg_2.54.7+dfsg-2.dsc 2960 SHA256:c8b4d66fb90b93a53014f3eadd88d6b35940060522d957c8d87bda3721bcf9fb
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.54.7%2bdfsg.orig.tar.xz' librsvg_2.54.7+dfsg.orig.tar.xz 14342756 SHA256:799f93b73ed24c03efda1c707d8c40630fdee18c7e7532dda4ad1ce9671e98c2
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.54.7%2bdfsg-2.debian.tar.xz' librsvg_2.54.7+dfsg-2.debian.tar.xz 35544 SHA256:671f8fa2bafadeb4687cdaa135a2e729180281b6dc249fb2291aafc36e7632b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/librsvg/2.54.7+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/librsvg/2.54.7+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librsvg/2.54.7+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.5.4-2`

Binary Packages:

- `libseccomp2:amd64=2.5.4-2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.4-2
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-2.dsc' libseccomp_2.5.4-2.dsc 2708 SHA256:48e3d00b42f561caafddc9149b514234c52f067ea05dd6c6c35c984a5a48c7f4
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz' libseccomp_2.5.4.orig.tar.gz 637228 SHA256:d82902400405cf0068574ef3dc1fe5f5926207543ba1ae6f8e7a1576351dcbdb
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz.asc' libseccomp_2.5.4.orig.tar.gz.asc 833 SHA256:af37e70eb422e6f983c1f135a3abb342c3b787716520b71bd774e4906003807f
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-2.debian.tar.xz' libseccomp_2.5.4-2.debian.tar.xz 17584 SHA256:0b9d98cdc5c9be32652733c08f11d8b788b229e427aa4b2d31df5fc523d498df
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.5.4-2/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.5.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.5.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.5-1`

Binary Packages:

- `libselinux1:amd64=3.5-1`
- `libselinux1-dev:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.5-1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.5-1.dsc' libselinux_3.5-1.dsc 2662 SHA256:b73314f88bb9def34b861fddcd0ead37ee13a7e12c94508f3a6436147c4cdf02
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.5.orig.tar.gz' libselinux_3.5.orig.tar.gz 211453 SHA256:9a3a3705ac13a2ccca2de6d652b6356fead10f36fb33115c185c5ccdf29eec19
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.5.orig.tar.gz.asc' libselinux_3.5.orig.tar.gz.asc 981 SHA256:fd37d441e0c08cabe9ac8f7815f52355bab2011549ec5792424fe18be9e1e015
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.5-1.debian.tar.xz' libselinux_3.5-1.debian.tar.xz 35804 SHA256:7e78f55b93bdbc8b991b24ec708e312604a6c39784abcf9cc6b83cd9eae3db0e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/3.5-1/ (for browsing the source)
- https://sources.debian.net/src/libselinux/3.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/3.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=3.5-1`

Binary Packages:

- `libsemanage-common=3.5-1`
- `libsemanage2:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.5-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.5-1.dsc' libsemanage_3.5-1.dsc 2644 SHA256:7415394f12030387ebca4ab7845830984b1ceb7ec3256d30a1733ba7f59d18c1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.5.orig.tar.gz' libsemanage_3.5.orig.tar.gz 185060 SHA256:f53534e50247538280ed0d76c6ce81d8fb3939bd64cadb89da10dba42e40dd9c
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.5.orig.tar.gz.asc' libsemanage_3.5.orig.tar.gz.asc 981 SHA256:f9126c861c666f3308b60cea4405c5e686a056113ca3cbd0a5b0e4af7600c8f5
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.5-1.debian.tar.xz' libsemanage_3.5-1.debian.tar.xz 29956 SHA256:78b11321d014bd52e1fb67c38db5ec6518b0b566b58c6e35a18e894dacc24aee
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/3.5-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/3.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/3.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=3.5-1`

Binary Packages:

- `libsepol-dev:amd64=3.5-1`
- `libsepol2:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libsepol-dev/copyright`, `/usr/share/doc/libsepol2/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.5-1
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.5-1.dsc' libsepol_3.5-1.dsc 2005 SHA256:6978aceb3966056e816731234c43737b6b3ffc0dba694c015b8edf3adf5ef914
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.5.orig.tar.gz' libsepol_3.5.orig.tar.gz 497522 SHA256:78fdaf69924db780bac78546e43d9c44074bad798c2c415d0b9bb96d065ee8a2
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.5.orig.tar.gz.asc' libsepol_3.5.orig.tar.gz.asc 981 SHA256:2309ab5e7cd38e2eb9196f92a60e00d4508cb293f1181d34a5a050128c9b7b24
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.5-1.debian.tar.xz' libsepol_3.5-1.debian.tar.xz 27500 SHA256:bb7abe2c205d055dde0495e8a2126529acf91658023278d9d919034794785e33
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/3.5-1/ (for browsing the source)
- https://sources.debian.net/src/libsepol/3.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/3.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsm=2:1.2.3-1`

Binary Packages:

- `libsm-dev:amd64=2:1.2.3-1`
- `libsm6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.3-1
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.3-1.dsc' libsm_1.2.3-1.dsc 2063 SHA256:5488f8de81d53c32cbb5f062b6a6f262cd067283b8082041392dc60f0d04002c
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.3.orig.tar.gz' libsm_1.2.3.orig.tar.gz 445362 SHA256:1e92408417cb6c6c477a8a6104291001a40b3bb56a4a60608fdd9cd2c5a0f320
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.3-1.diff.gz' libsm_1.2.3-1.diff.gz 8929 SHA256:7eb99ab50b19f26d1470f89e4b46891f6a697cb1794a58ed0d1376cceaf1b6a9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsm/2:1.2.3-1/ (for browsing the source)
- https://sources.debian.net/src/libsm/2:1.2.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsm/2:1.2.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libssh2=1.11.0-2`

Binary Packages:

- `libssh2-1:amd64=1.11.0-2`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libssh2/1.11.0-2/


### `dpkg` source package: `libtasn1-6=4.19.0-3`

Binary Packages:

- `libtasn1-6:amd64=4.19.0-3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.19.0-3
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-3.dsc' libtasn1-6_4.19.0-3.dsc 2662 SHA256:7fd9618be5b99035c7387d969b73365a57b1f6f01ec4abe0af332829af718190
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz' libtasn1-6_4.19.0.orig.tar.gz 1786576 SHA256:1613f0ac1cf484d6ec0ce3b8c06d56263cc7242f1c23b30d82d23de345a63f7a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz.asc' libtasn1-6_4.19.0.orig.tar.gz.asc 228 SHA256:8410c0c004f3509c218a98b276b3308b9c46f48068e8b1a6d9ebfd61ea9f357a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-3.debian.tar.xz' libtasn1-6_4.19.0-3.debian.tar.xz 22084 SHA256:acb32dc03d8c2aeb10e0fb1c2a0247efdab0a6dc5e8f8a4d3cdcfe5ad26bb0df
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.19.0-3/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.19.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.19.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libthai=0.1.29-1`

Binary Packages:

- `libthai-data=0.1.29-1`
- `libthai0:amd64=0.1.29-1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.29-1
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.29-1.dsc' libthai_0.1.29-1.dsc 2325 SHA256:470b853bcb84ce88c63720da51ee5b0001fd1ebec8f8679a986b155d0be1ff06
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.29.orig.tar.xz' libthai_0.1.29.orig.tar.xz 417728 SHA256:fc80cc7dcb50e11302b417cebd24f2d30a8b987292e77e003267b9100d0f4bcd
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.29-1.debian.tar.xz' libthai_0.1.29-1.debian.tar.xz 12564 SHA256:5c86bd1c2af7972e29cead559823c8f85b9dd9363efad0d90ab7ad86e35840ef
```

Other potentially useful URLs:

- https://sources.debian.net/src/libthai/0.1.29-1/ (for browsing the source)
- https://sources.debian.net/src/libthai/0.1.29-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libthai/0.1.29-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtirpc=1.3.4+ds-1`

Binary Packages:

- `libtirpc-common=1.3.4+ds-1`
- `libtirpc-dev:amd64=1.3.4+ds-1`
- `libtirpc3:amd64=1.3.4+ds-1`

Licenses: (parsed from: `/usr/share/doc/libtirpc-common/copyright`, `/usr/share/doc/libtirpc-dev/copyright`, `/usr/share/doc/libtirpc3/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `BSD-4-Clause`
- `GPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `PERMISSIVE`
- `__AUTO_PERMISSIVE__`

Source:

```console
$ apt-get source -qq --print-uris libtirpc=1.3.4+ds-1
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.4%2bds-1.dsc' libtirpc_1.3.4+ds-1.dsc 2129 SHA256:543919b82d61d1dfcdbf7baac1ca2f9c65fa5840fd16eca2975bd2e1b5c37998
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.4%2bds.orig.tar.gz' libtirpc_1.3.4+ds.orig.tar.gz 700735 SHA256:730101dbb756b258164e496109bfdeee87eb0fcc05cd5a820e5f34537a1e637d
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.4%2bds-1.debian.tar.xz' libtirpc_1.3.4+ds-1.debian.tar.xz 11436 SHA256:1072d8af8e50a795d7c85f8ad5879ce9596ff0faa37f99fde745d090dcafd0c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtirpc/1.3.4+ds-1/ (for browsing the source)
- https://sources.debian.net/src/libtirpc/1.3.4+ds-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtirpc/1.3.4+ds-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtool=2.4.7-7`

Binary Packages:

- `libltdl-dev:amd64=2.4.7-7`
- `libltdl7:amd64=2.4.7-7`
- `libtool=2.4.7-7`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.7-7
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.7-7.dsc' libtool_2.4.7-7.dsc 2257 SHA256:c6045c55f34fcd3b7a4194059d498085d4a6d0bc4c6a0cb3825fb3859461dc7a
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.7.orig.tar.xz' libtool_2.4.7.orig.tar.xz 1026028 SHA256:dd637e270439b208907ceead3f163470ed2ce5723ef97ffbda6463c64b57128a
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.7-7.debian.tar.xz' libtool_2.4.7-7.debian.tar.xz 40916 SHA256:217a33c2f4474f4f23c69fa0bc694f9d380885003f02785ed69248b0dfb1d449
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtool/2.4.7-7/ (for browsing the source)
- https://sources.debian.net/src/libtool/2.4.7-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtool/2.4.7-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=1.1-2`

Binary Packages:

- `libunistring5:amd64=1.1-2`

Licenses: (parsed from: `/usr/share/doc/libunistring5/copyright`)

- `FreeSoftware`
- `GFDL-1.2`
- `GFDL-NIV-1.2+`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with distribution exception`
- `GPL-2+ with distribution exception, Expat`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris libunistring=1.1-2
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.1-2.dsc' libunistring_1.1-2.dsc 2031 SHA256:2d8f1274fdc9b7434e9dcc4a0a6891e36aa015f43e4a0638ec4de6837873bd98
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.1.orig.tar.xz' libunistring_1.1.orig.tar.xz 2397676 SHA256:827c1eb9cb6e7c738b171745dac0888aa58c5924df2e59239318383de0729b98
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.1.orig.tar.xz.asc' libunistring_1.1.orig.tar.xz.asc 833 SHA256:dadae6c38f85f9e8776231436c601c386924ceb44d511456c61c9be73608933d
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.1-2.debian.tar.xz' libunistring_1.1-2.debian.tar.xz 14008 SHA256:93dd1881e69e6046e2d2ec20ce99f2ae07e4ba078c506cd40104e19e08c681d1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/1.1-2/ (for browsing the source)
- https://sources.debian.net/src/libunistring/1.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/1.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwebp=1.3.2-0.3`

Binary Packages:

- `libsharpyuv-dev:amd64=1.3.2-0.3`
- `libsharpyuv0:amd64=1.3.2-0.3`
- `libwebp-dev:amd64=1.3.2-0.3`
- `libwebp7:amd64=1.3.2-0.3`
- `libwebpdecoder3:amd64=1.3.2-0.3`
- `libwebpdemux2:amd64=1.3.2-0.3`
- `libwebpmux3:amd64=1.3.2-0.3`

Licenses: (parsed from: `/usr/share/doc/libsharpyuv-dev/copyright`, `/usr/share/doc/libsharpyuv0/copyright`, `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp7/copyright`, `/usr/share/doc/libwebpdecoder3/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`

Source:

```console
$ apt-get source -qq --print-uris libwebp=1.3.2-0.3
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_1.3.2-0.3.dsc' libwebp_1.3.2-0.3.dsc 2461 SHA256:5fde1afa1af8f1608b26a0040775573b896f97c843fa6f050bd0f4523ac4b6a5
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_1.3.2.orig.tar.gz' libwebp_1.3.2.orig.tar.gz 4162949 SHA256:2a499607df669e40258e53d0ade8035ba4ec0175244869d1025d460562aa09b4
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_1.3.2-0.3.debian.tar.xz' libwebp_1.3.2-0.3.debian.tar.xz 15524 SHA256:cacf877660813a005658e18975faa4ffe30b01286a17cf767ffd666e270ce5d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwebp/1.3.2-0.3/ (for browsing the source)
- https://sources.debian.net/src/libwebp/1.3.2-0.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwebp/1.3.2-0.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwmf=0.2.13-1.1`

Binary Packages:

- `libwmf-0.2-7:amd64=0.2.13-1.1`
- `libwmf-dev=0.2.13-1.1`
- `libwmflite-0.2-7:amd64=0.2.13-1.1`

Licenses: (parsed from: `/usr/share/doc/libwmf-0.2-7/copyright`, `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmflite-0.2-7/copyright`)

- `AGPL-3 with Font exception`
- `GD`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.13-1.1
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.13-1.1.dsc' libwmf_0.2.13-1.1.dsc 2345 SHA256:05907248aae50ef26e44f518b628008b86cb8666513e568473fb62dfdee504af
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.13.orig.tar.gz' libwmf_0.2.13.orig.tar.gz 3044235 SHA256:18ba69febd2f515d98a2352de284a8051896062ac9728d2ead07bc39ea75a068
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.13-1.1.debian.tar.xz' libwmf_0.2.13-1.1.debian.tar.xz 25784 SHA256:0032481fbf98810ca446ab8931392acd13bfee29d1df4000fb783b7126f8e0f4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwmf/0.2.13-1.1/ (for browsing the source)
- https://sources.debian.net/src/libwmf/0.2.13-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwmf/0.2.13-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.8.7-1`

Binary Packages:

- `libx11-6:amd64=2:1.8.7-1`
- `libx11-data=2:1.8.7-1`
- `libx11-dev:amd64=2:1.8.7-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.8.7-1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.8.7-1.dsc' libx11_1.8.7-1.dsc 2480 SHA256:96eddec7e55ab344ce654c5043d59bc8da6470eb7849a578c843af965dda79d1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.8.7.orig.tar.gz' libx11_1.8.7.orig.tar.gz 3185363 SHA256:793ebebf569f12c864b77401798d38814b51790fce206e01a431e5feb982e20b
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.8.7.orig.tar.gz.asc' libx11_1.8.7.orig.tar.gz.asc 833 SHA256:c1cba69555c89e503abac81ebf1113a756f2fafd72677e7862b40f12208e0260
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.8.7-1.diff.gz' libx11_1.8.7-1.diff.gz 74344 SHA256:57adc62acb0ba21a4cf444aaf03ea4adc7f732215df22afa8b8d6fd31d799d95
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.8.7-1/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.8.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.8.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxau=1:1.0.9-1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.9-1`
- `libxau6:amd64=1:1.0.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-1
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.9-1.dsc' libxau_1.0.9-1.dsc 2183 SHA256:e6e059652cda7e5a49b6c9a70667639f32d629c20320487d16c642a06c1ebf85
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA256:1f123d8304b082ad63a9e89376400a3b1d4c29e67e3ea07b3f659cccca690eea
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz.asc' libxau_1.0.9.orig.tar.gz.asc 801 SHA256:af6104aaf3c5ede529e381237dd60f49640ec96593a84502fa493b86582b2f04
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.9-1.diff.gz' libxau_1.0.9-1.diff.gz 10193 SHA256:7b34899563f172e8f11d061de41b58fe1c32f8683d985e57686677ccb7299a9a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxau/1:1.0.9-1/ (for browsing the source)
- https://sources.debian.net/src/libxau/1:1.0.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxau/1:1.0.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcb=1.15-1`

Binary Packages:

- `libxcb-render0:amd64=1.15-1`
- `libxcb-render0-dev:amd64=1.15-1`
- `libxcb-shm0:amd64=1.15-1`
- `libxcb-shm0-dev:amd64=1.15-1`
- `libxcb1:amd64=1.15-1`
- `libxcb1-dev:amd64=1.15-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.15-1
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.15-1.dsc' libxcb_1.15-1.dsc 5344 SHA256:f689569f33e70ca4c95c91b094d0659eb49a958d9ac43186640338f9290e298b
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.15.orig.tar.gz' libxcb_1.15.orig.tar.gz 650774 SHA256:1cb65df8543a69ec0555ac696123ee386321dfac1964a3da39976c9a05ad724d
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.15-1.diff.gz' libxcb_1.15-1.diff.gz 26267 SHA256:639c719ed06ffc397b200a209abd1a049e21e9e19431fb14c9ca870de01a6eac
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcb/1.15-1/ (for browsing the source)
- https://sources.debian.net/src/libxcb/1.15-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcb/1.15-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcrypt=1:4.4.36-2`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.36-2`
- `libcrypt1:amd64=1:4.4.36-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.36-2
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.36-2.dsc' libxcrypt_4.4.36-2.dsc 1563 SHA256:7a1c78fcd9029f5828f22d5697ec02aacaec276c23ab06af82f13e1a77026ea2
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.36.orig.tar.xz' libxcrypt_4.4.36.orig.tar.xz 392732 SHA256:7b7abbc89f13f5194211aa6861ed954e4fa3a210a4cb64f7e13dc8cf413e7f2a
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.36-2.debian.tar.xz' libxcrypt_4.4.36-2.debian.tar.xz 8284 SHA256:c91f86abf83fc71f69fe80d38f92354042436b6eca8a3ef666ffc86e319dd267
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.36-2/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.36-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.36-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdmcp=1:1.1.2-3`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.2-3`
- `libxdmcp6:amd64=1:1.1.2-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.2-3
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.dsc' libxdmcp_1.1.2-3.dsc 2145 SHA256:f9697dca6a275aeee9a3eee9fb2d55e0f77485481e8b84efc6950fc9b1988460
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2.orig.tar.gz' libxdmcp_1.1.2.orig.tar.gz 404115 SHA256:6f7c7e491a23035a26284d247779174dedc67e34e93cc3548b648ffdb6fc57c0
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.diff.gz' libxdmcp_1.1.2-3.diff.gz 18017 SHA256:5844df115c17e5ba40ac116f80373304d821c607e763ef6f40562421f5cc0cf3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxdmcp/1:1.1.2-3/ (for browsing the source)
- https://sources.debian.net/src/libxdmcp/1:1.1.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxdmcp/1:1.1.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxext=2:1.3.4-1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.4-1+b1`
- `libxext6:amd64=2:1.3.4-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-1
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.4-1.dsc' libxext_1.3.4-1.dsc 2118 SHA256:25024f57d955739c6b858822bf93ec3c71400b56fc0d666826f440e3661fd7c0
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA256:8ef0789f282826661ff40a8eef22430378516ac580167da35cc948be9041aac1
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.4-1.diff.gz' libxext_1.3.4-1.diff.gz 12509 SHA256:b975870d6a7b791ffbe2d57efdf6e20c250c5e76d12e45b04c8655f593bb8337
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxext/2:1.3.4-1/ (for browsing the source)
- https://sources.debian.net/src/libxext/2:1.3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxext/2:1.3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxml2=2.9.14+dfsg-1.3`

Binary Packages:

- `libxml2:amd64=2.9.14+dfsg-1.3`
- `libxml2-dev:amd64=2.9.14+dfsg-1.3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.14+dfsg-1.3
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.3.dsc' libxml2_2.9.14+dfsg-1.3.dsc 3078 SHA256:e0e234b80e36389ec771edb6df0adde03f56ba5ad9b41f2d739de56a70850b68
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg.orig.tar.xz' libxml2_2.9.14+dfsg.orig.tar.xz 2351200 SHA256:4fe913dec8b1ab89d13b489b419a8203176ea39e931eaa0d25b17eafb9c279e9
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.3.debian.tar.xz' libxml2_2.9.14+dfsg-1.3.debian.tar.xz 35076 SHA256:138dbd0f7c116058ae3306ee0ad3a2fed9754645a129784aff0a69fcf63e53e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxml2/2.9.14+dfsg-1.3/ (for browsing the source)
- https://sources.debian.net/src/libxml2/2.9.14+dfsg-1.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxml2/2.9.14+dfsg-1.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxrender=1:0.9.10-1.1`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1.1`
- `libxrender1:amd64=1:0.9.10-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1.1
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.1.dsc' libxrender_0.9.10-1.1.dsc 2072 SHA256:348ab15d05f1d802da485e4c6abdb9d5419691fb7c8ce44ca5b17b2b7f889ce8
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA256:770527cce42500790433df84ec3521e8bf095dfe5079454a92236494ab296adf
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.1.diff.gz' libxrender_0.9.10-1.1.diff.gz 15201 SHA256:caf8c84085b3b0d073f738fa12d32d4eca2d8b669cb3c7f1b1cd2ce64b7b10b7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxrender/1:0.9.10-1.1/ (for browsing the source)
- https://sources.debian.net/src/libxrender/1:0.9.10-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxrender/1:0.9.10-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxslt=1.1.35-1`

Binary Packages:

- `libxslt1-dev:amd64=1.1.35-1`
- `libxslt1.1:amd64=1.1.35-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.35-1
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.35-1.dsc' libxslt_1.1.35-1.dsc 2155 SHA256:d0aaa627a3b18a440019ab82b61c7f7953ec78369aaa92b0680b04e1a20b3df1
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.35.orig.tar.xz' libxslt_1.1.35.orig.tar.xz 1827548 SHA256:8247f33e9a872c6ac859aa45018bc4c4d00b97e2feac9eebc10c93ce1f34dd79
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.35-1.debian.tar.xz' libxslt_1.1.35-1.debian.tar.xz 21420 SHA256:ed2821ca0d0c9235eed907117c6dfbf5a54e15702aa0937293c5dfa52335a315
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxslt/1.1.35-1/ (for browsing the source)
- https://sources.debian.net/src/libxslt/1.1.35-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxslt/1.1.35-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxt=1:1.2.1-1.1`

Binary Packages:

- `libxt-dev:amd64=1:1.2.1-1.1`
- `libxt6:amd64=1:1.2.1-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.1-1.1
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.1-1.1.dsc' libxt_1.2.1-1.1.dsc 2170 SHA256:62859ce41aa5914f32715fadb9dc60a54cc1ef3331b2122969ffbe31e5d53be7
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz' libxt_1.2.1.orig.tar.gz 1024473 SHA256:6da1bfa9dd0ed87430a5ce95b129485086394df308998ebe34d98e378e3dfb33
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz.asc' libxt_1.2.1.orig.tar.gz.asc 358 SHA256:da406cc94c25ca6773bb37c2055e2eb5665491f7ca6dfc9ea04f0f30ea3fd098
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.1-1.1.diff.gz' libxt_1.2.1-1.1.diff.gz 45585 SHA256:ae7993031f3d77fcdbc2540f9d1b6b4a0afafddd747f1de444e4ffe2fa678fca
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxt/1:1.2.1-1.1/ (for browsing the source)
- https://sources.debian.net/src/libxt/1:1.2.1-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxt/1:1.2.1-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libyaml=0.2.5-1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.5-1`
- `libyaml-dev:amd64=0.2.5-1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.5-1
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.2.5-1.dsc' libyaml_0.2.5-1.dsc 2071 SHA256:1edbf86e5cd76937ff62892ba6c2537456d645d834d4cd4a82430b8be7051bf4
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.2.5.orig.tar.gz' libyaml_0.2.5.orig.tar.gz 85055 SHA256:fa240dbf262be053f3898006d502d514936c818e422afdcf33921c63bed9bf2e
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.2.5-1.debian.tar.xz' libyaml_0.2.5-1.debian.tar.xz 5324 SHA256:8730e0510129e516c3c7c1cda7428e02a0a122699e57ed203f835a338a686d1f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libyaml/0.2.5-1/ (for browsing the source)
- https://sources.debian.net/src/libyaml/0.2.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libyaml/0.2.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.5.5+dfsg2-2`

Binary Packages:

- `libzstd-dev:amd64=1.5.5+dfsg2-2`
- `libzstd1:amd64=1.5.5+dfsg2-2`

Licenses: (parsed from: `/usr/share/doc/libzstd-dev/copyright`, `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.5+dfsg2-2
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-2.dsc' libzstd_1.5.5+dfsg2-2.dsc 2375 SHA256:4e27ea0c5e2564dd6cc93d95fddc56ef85c5388ea4a4a60d8cca0b4c18c1da4f
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2.orig.tar.xz' libzstd_1.5.5+dfsg2.orig.tar.xz 1784164 SHA256:d7cf3c10d416fd999cb8fcf7685d9268ba7bec8eb78121fc2d0d916fa393d22b
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-2.debian.tar.xz' libzstd_1.5.5+dfsg2-2.debian.tar.xz 21068 SHA256:0a72f44f83cbd2dce66722f5c7844aaf8e5937066a795ca6b3d2b0eba69b9e73
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.5.5+dfsg2-2/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.5.5+dfsg2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.5.5+dfsg2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `linux=6.5.10-1`

Binary Packages:

- `linux-libc-dev:amd64=6.5.10-1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `BSD-2-clause`
- `CRYPTOGAMS`
- `GPL-2`
- `GPL-2+-or-X11`
- `LGPL-2.1`
- `Unicode-data`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=6.5.10-1
'http://deb.debian.org/debian/pool/main/l/linux/linux_6.5.10-1.dsc' linux_6.5.10-1.dsc 285873 SHA256:74ab38a1a63df5d30c2197522f2474078d6644d57db840b72a0cdf3a351b0a2e
'http://deb.debian.org/debian/pool/main/l/linux/linux_6.5.10.orig.tar.xz' linux_6.5.10.orig.tar.xz 141512408 SHA256:f6bf9109e7f5f7602eff38597931fecdfc0bcaf342cc9e8e009136429045a36b
'http://deb.debian.org/debian/pool/main/l/linux/linux_6.5.10-1.debian.tar.xz' linux_6.5.10-1.debian.tar.xz 1510832 SHA256:7ccdd3340ef5f0c1510c0fc5d6b1e2bc02ec60a99fb6975c5e5793f545e285cf
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/6.5.10-1/ (for browsing the source)
- https://sources.debian.net/src/linux/6.5.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/6.5.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lz4=1.9.4-1`

Binary Packages:

- `liblz4-1:amd64=1.9.4-1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.4-1
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.4-1.dsc' lz4_1.9.4-1.dsc 1951 SHA256:e16302bca544d08d106efc216541f4a0403c8f8a5fad5eaac7588223a55af263
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.4.orig.tar.gz' lz4_1.9.4.orig.tar.gz 354063 SHA256:0b0e3aa07c8c063ddf40b082bdf7e37a1562bda40a0ff5272957f3e987e0e54b
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.4-1.debian.tar.xz' lz4_1.9.4-1.debian.tar.xz 8128 SHA256:47ceec5b95f42598f7b9280b03df9659f2ee6852720ec181488e83bd643f0e5f
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.9.4-1/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.9.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.9.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lzo2=2.10-2`

Binary Packages:

- `liblzo2-2:amd64=2.10-2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.10-2
'http://deb.debian.org/debian/pool/main/l/lzo2/lzo2_2.10-2.dsc' lzo2_2.10-2.dsc 1926 SHA256:65a35d9d2511a88f30d4b10313f807c184d1906062e2421833797dafc2682166
'http://deb.debian.org/debian/pool/main/l/lzo2/lzo2_2.10.orig.tar.gz' lzo2_2.10.orig.tar.gz 600622 SHA256:c0f892943208266f9b6543b3ae308fab6284c5c90e627931446fb49b4221a072
'http://deb.debian.org/debian/pool/main/l/lzo2/lzo2_2.10-2.debian.tar.xz' lzo2_2.10-2.debian.tar.xz 6880 SHA256:095b2bf2012138f6892fcf226a0d1eae5d29406d7afe7129d51d64116e61c472
```

Other potentially useful URLs:

- https://sources.debian.net/src/lzo2/2.10-2/ (for browsing the source)
- https://sources.debian.net/src/lzo2/2.10-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lzo2/2.10-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `m4=1.4.19-4`

Binary Packages:

- `m4=1.4.19-4`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.19-4
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.19-4.dsc' m4_1.4.19-4.dsc 1637 SHA256:a52a24925928296b2574462d72bb1393e0cd54527a1ed2278aa2708bac543176
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.19.orig.tar.xz' m4_1.4.19.orig.tar.xz 1654908 SHA256:63aede5c6d33b6d9b13511cd0be2cac046f2e70fd0a07aa9573a04a82783af96
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.19.orig.tar.xz.asc' m4_1.4.19.orig.tar.xz.asc 488 SHA256:9700ba4dca539b06e033b4e3ab37fa5b983becb6c14569a8b8aa02dee6ab666c
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.19-4.debian.tar.xz' m4_1.4.19-4.debian.tar.xz 17308 SHA256:c3fe8fe88dc5ba0d4dc114bea085dbc8421b7044b566a9a60b23499ff174c72f
```

Other potentially useful URLs:

- https://sources.debian.net/src/m4/1.4.19-4/ (for browsing the source)
- https://sources.debian.net/src/m4/1.4.19-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/m4/1.4.19-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `make-dfsg=4.3-4.1`

Binary Packages:

- `make=4.3-4.1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.3-4.1
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.3-4.1.dsc' make-dfsg_4.3-4.1.dsc 2019 SHA256:d2523d94f4d4198df6801f238d36cf0dea2ab5521f1d19ee76b2e8ee1f1918bb
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA256:be4c17542578824e745f83bcd2a9ba264206187247cb6a5f5df99b0a9d1f9047
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.3-4.1.diff.gz' make-dfsg_4.3-4.1.diff.gz 50940 SHA256:753c254ecaba425ebe2e0a0fb4d299847701e1c3eeb43df563e39975cae56b4c
```

Other potentially useful URLs:

- https://sources.debian.net/src/make-dfsg/4.3-4.1/ (for browsing the source)
- https://sources.debian.net/src/make-dfsg/4.3-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/make-dfsg/4.3-4.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mariadb=1:10.11.5-3`

Binary Packages:

- `libmariadb-dev=1:10.11.5-3`
- `libmariadb-dev-compat=1:10.11.5-3`
- `libmariadb3:amd64=1:10.11.5-3`
- `mariadb-common=1:10.11.5-3`

Licenses: (parsed from: `/usr/share/doc/libmariadb-dev/copyright`, `/usr/share/doc/libmariadb-dev-compat/copyright`, `/usr/share/doc/libmariadb3/copyright`, `/usr/share/doc/mariadb-common/copyright`)

- `Artistic`
- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-2+-with-bison-exception`
- `GPL-3+-with-bison-exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `SWsoft`
- `public-domain`
- `unlimited-free-doc`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris mariadb=1:10.11.5-3
'http://deb.debian.org/debian/pool/main/m/mariadb/mariadb_10.11.5-3.dsc' mariadb_10.11.5-3.dsc 5305 SHA256:b6db1a61d0fbc5d64bbf07e2e8fac2d615f8566539ae036b8e1c679519b2373d
'http://deb.debian.org/debian/pool/main/m/mariadb/mariadb_10.11.5.orig.tar.gz' mariadb_10.11.5.orig.tar.gz 96193384 SHA256:5be50c6aed5c37db35afc70c0678cf18860f1e78a228fd84e6d7a49583fdf411
'http://deb.debian.org/debian/pool/main/m/mariadb/mariadb_10.11.5.orig.tar.gz.asc' mariadb_10.11.5.orig.tar.gz.asc 833 SHA256:2ba7eea6cc775f7ee67fd06a05f195e5bcc32df88b2b6771b5b32cbdd32b7ca0
'http://deb.debian.org/debian/pool/main/m/mariadb/mariadb_10.11.5-3.debian.tar.xz' mariadb_10.11.5-3.debian.tar.xz 276652 SHA256:9b8d4ce8cf7338ac4122d20d61dd0b443af2a9515acb6fb7f60538b0c42be5da
```

Other potentially useful URLs:

- https://sources.debian.net/src/mariadb/1:10.11.5-3/ (for browsing the source)
- https://sources.debian.net/src/mariadb/1:10.11.5-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mariadb/1:10.11.5-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mawk=1.3.4.20231102-1`

Binary Packages:

- `mawk=1.3.4.20231102-1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `GPL-2.0-only`
- `X11`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/mawk/1.3.4.20231102-1/


### `dpkg` source package: `media-types=10.1.0`

Binary Packages:

- `media-types=10.1.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=10.1.0
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_10.1.0.dsc' media-types_10.1.0.dsc 1624 SHA256:1470ba869117eed57ba24c1e54664116a7ab6b4417e4b911e8c8051ffe19d626
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_10.1.0.tar.xz' media-types_10.1.0.tar.xz 59052 SHA256:c35ec1ae0d0446aa903322f8f91a908a0d4270444326bfbad24b61fbe5600a0d
```

Other potentially useful URLs:

- https://sources.debian.net/src/media-types/10.1.0/ (for browsing the source)
- https://sources.debian.net/src/media-types/10.1.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/media-types/10.1.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mercurial=6.5.2-2`

Binary Packages:

- `mercurial=6.5.2-2`
- `mercurial-common=6.5.2-2`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=6.5.2-2
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.5.2-2.dsc' mercurial_6.5.2-2.dsc 2806 SHA256:fc56db9252a8124669bf03a4dfba36ada6405fc9ee9f53b7a52c57f20882e13f
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.5.2.orig.tar.gz' mercurial_6.5.2.orig.tar.gz 8233023 SHA256:afc39d7067976593c8332b8e97a12afd393b55037c5fb9c3cab1a42c7560f60a
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.5.2.orig.tar.gz.asc' mercurial_6.5.2.orig.tar.gz.asc 659 SHA256:c61c80e2e1b45c18345238bd19c835e4cc4cfdc6ef3ef3ef004bcb16da0eeeb1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.5.2-2.debian.tar.xz' mercurial_6.5.2-2.debian.tar.xz 69132 SHA256:c8382c93a0448cab79c20ec24cffa9ab60446d7d87ada187230cd7d7eb0c6adf
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/6.5.2-2/ (for browsing the source)
- https://sources.debian.net/src/mercurial/6.5.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/6.5.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpclib3=1.3.1-1`

Binary Packages:

- `libmpc3:amd64=1.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.3.1-1
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.3.1-1.dsc' mpclib3_1.3.1-1.dsc 1877 SHA256:b2252a499fd0f8e92ce2cf7d8e68477ffc9dd06127803a91f0a1115822efec75
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.3.1.orig.tar.gz' mpclib3_1.3.1.orig.tar.gz 773573 SHA256:ab642492f5cf882b74aa0cb730cd410a81edcdbec895183ce930e706c1c759b8
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.3.1-1.debian.tar.xz' mpclib3_1.3.1-1.debian.tar.xz 4656 SHA256:25adb496258adacad69c022d712f96fbc465bcef9fd4751829dc351d9ce6a45d
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpclib3/1.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/mpclib3/1.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpclib3/1.3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpfr4=4.2.1-1`

Binary Packages:

- `libmpfr6:amd64=4.2.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.2.1-1
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.2.1-1.dsc' mpfr4_4.2.1-1.dsc 1959 SHA256:2fb0ea6c37591f03c7f3445fc6a298a10dbd9d7662ccb441f7da0e514d71986a
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.2.1.orig.tar.xz' mpfr4_4.2.1.orig.tar.xz 1493608 SHA256:277807353a6726978996945af13e52829e3abd7a9a5b7fb2793894e18f1fcbb2
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.2.1-1.debian.tar.xz' mpfr4_4.2.1-1.debian.tar.xz 12556 SHA256:06c6c90efe3653d44527bcd6cfd66563d62409bbb348eb32f33b480e30ad9993
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpfr4/4.2.1-1/ (for browsing the source)
- https://sources.debian.net/src/mpfr4/4.2.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpfr4/4.2.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mysql-defaults=1.1.0`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.1.0`
- `mysql-common=5.8+1.1.0`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.1.0
'http://deb.debian.org/debian/pool/main/m/mysql-defaults/mysql-defaults_1.1.0.dsc' mysql-defaults_1.1.0.dsc 2279 SHA256:b93b3ec5deca87cf63da03b7c349b68ffd9cc78bb36ec967bae8015717c70111
'http://deb.debian.org/debian/pool/main/m/mysql-defaults/mysql-defaults_1.1.0.tar.xz' mysql-defaults_1.1.0.tar.xz 7396 SHA256:093f1c30172ba5dbfb4c19a2dfe6d533bb207102232ae5f080eb0bc0476f02e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/mysql-defaults/1.1.0/ (for browsing the source)
- https://sources.debian.net/src/mysql-defaults/1.1.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mysql-defaults/1.1.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.4+20231016-1`

Binary Packages:

- `libncurses-dev:amd64=6.4+20231016-1`
- `libncurses6:amd64=6.4+20231016-1`
- `libncursesw6:amd64=6.4+20231016-1`
- `libtinfo6:amd64=6.4+20231016-1`
- `ncurses-base=6.4+20231016-1`
- `ncurses-bin=6.4+20231016-1`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ncurses/6.4+20231016-1/


### `dpkg` source package: `netbase=6.4`

Binary Packages:

- `netbase=6.4`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.4
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.4.dsc' netbase_6.4.dsc 898 SHA256:dc26cfcaa49fd874cc27c65216b2f8b6d3ad62845b78da4bdf0aea55592af756
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.4.tar.xz' netbase_6.4.tar.xz 32712 SHA256:fa6621826ff1150e581bd90bc3c8a4ecafe5df90404f207db6dcdf2c75f26ad7
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/6.4/ (for browsing the source)
- https://sources.debian.net/src/netbase/6.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/6.4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.9.1-2`

Binary Packages:

- `libhogweed6:amd64=3.9.1-2`
- `libnettle8:amd64=3.9.1-2`

Licenses: (parsed from: `/usr/share/doc/libhogweed6/copyright`, `/usr/share/doc/libnettle8/copyright`)

- `Expat`
- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3+ with Autoconf exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-3+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=3.9.1-2
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.9.1-2.dsc' nettle_3.9.1-2.dsc 2274 SHA256:8ba0494afc18b086ef61d61c3b14a27f1c999ee89fbc55288b7a81eff395e521
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.9.1.orig.tar.gz' nettle_3.9.1.orig.tar.gz 2396741 SHA256:ccfeff981b0ca71bbd6fbcb054f407c60ffb644389a5be80d6716d5b550c6ce3
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.9.1.orig.tar.gz.asc' nettle_3.9.1.orig.tar.gz.asc 573 SHA256:9746017a1a7fe60aad4b929ea592bc6ac51e12ea7179f289944eb44828d958af
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.9.1-2.debian.tar.xz' nettle_3.9.1-2.debian.tar.xz 24440 SHA256:75e4612ae51801a674c1697bd189811606e81e72e7ac25ef6c056b7a2a9b2986
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.9.1-2/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.9.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.9.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nghttp2=1.58.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.58.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `all-permissive`

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.58.0-1
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.58.0-1.dsc' nghttp2_1.58.0-1.dsc 2534 SHA256:6230357ee97d470d55f33c1b49b49a00e494721e191f60cedf5f9e82b99f5c4f
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.58.0.orig.tar.gz' nghttp2_1.58.0.orig.tar.gz 1061810 SHA256:7da19947b33a07ddcf97b9791331bfee8a8545e6b394275a9971f43cae9d636b
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.58.0-1.debian.tar.xz' nghttp2_1.58.0-1.debian.tar.xz 11788 SHA256:967aa46cc926e71b6fccfbce81bb69a2c4793a3be979722d3f53c77d3e61f138
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.58.0-1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.58.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.58.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `npth=1.6-3`

Binary Packages:

- `libnpth0:amd64=1.6-3`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-3
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6-3.dsc' npth_1.6-3.dsc 1931 SHA256:002c2a7936d1499ebb5d72dbb9c7ca3e00ed5fe3b0aa48f20b7279fc90aa9e90
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA256:1393abd9adcf0762d34798dc34fdcf4d0d22a8410721e76f1e3afcd1daa4e2d1
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6-3.debian.tar.xz' npth_1.6-3.debian.tar.xz 10712 SHA256:efa188104de503add9c49c17bec7bec0df814f7d1db9fdc2017574a0af98155c
```

Other potentially useful URLs:

- https://sources.debian.net/src/npth/1.6-3/ (for browsing the source)
- https://sources.debian.net/src/npth/1.6-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/npth/1.6-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `numpy=1:1.24.2-1`

Binary Packages:

- `python3-numpy=1:1.24.2-1`

Licenses: (parsed from: `/usr/share/doc/python3-numpy/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `MIT`
- `Public-Domain`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris numpy=1:1.24.2-1
'http://deb.debian.org/debian/pool/main/n/numpy/numpy_1.24.2-1.dsc' numpy_1.24.2-1.dsc 2462 SHA256:33f8acc8cb64f72787b965e8713dd9dbb4f1dd0d54018fbdcbe99c55aff2541b
'http://deb.debian.org/debian/pool/main/n/numpy/numpy_1.24.2.orig.tar.xz' numpy_1.24.2.orig.tar.xz 8239412 SHA256:a7c88b0cf7c7c5ea03a76593ce4065af3beb8f50c25db6a7ee72369b2c936c65
'http://deb.debian.org/debian/pool/main/n/numpy/numpy_1.24.2-1.debian.tar.xz' numpy_1.24.2-1.debian.tar.xz 31632 SHA256:f87ec8c98f283b2d04eef73db7fdffd5c90c35db778dd0ddec04a0aaa15d14ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/numpy/1:1.24.2-1/ (for browsing the source)
- https://sources.debian.net/src/numpy/1:1.24.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/numpy/1:1.24.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openexr=3.1.5-5.1`

Binary Packages:

- `libopenexr-3-1-30:amd64=3.1.5-5.1`
- `libopenexr-dev=3.1.5-5.1`

Licenses: (parsed from: `/usr/share/doc/libopenexr-3-1-30/copyright`, `/usr/share/doc/libopenexr-dev/copyright`)

- `BSD-3-clause`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=3.1.5-5.1
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_3.1.5-5.1.dsc' openexr_3.1.5-5.1.dsc 2489 SHA256:aca9636b9d8c54158342ba15547a01d86765203ce94af9e404924c39df54d040
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_3.1.5.orig.tar.gz' openexr_3.1.5.orig.tar.gz 20327926 SHA256:93925805c1fc4f8162b35f0ae109c4a75344e6decae5a240afdfce25f8a433ec
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_3.1.5.orig.tar.gz.asc' openexr_3.1.5.orig.tar.gz.asc 287 SHA256:a2c4ac5151789903ca8ab3093a2798491463ccf2abfd003a20f96453e505dd5f
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_3.1.5-5.1.debian.tar.xz' openexr_3.1.5-5.1.debian.tar.xz 18828 SHA256:f4ab9368399d9915e122b6b2da5962c1832c58dac20564fa6c88b1c8c70fdf40
```

Other potentially useful URLs:

- https://sources.debian.net/src/openexr/3.1.5-5.1/ (for browsing the source)
- https://sources.debian.net/src/openexr/3.1.5-5.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openexr/3.1.5-5.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openjpeg2=2.5.0-2`

Binary Packages:

- `libopenjp2-7:amd64=2.5.0-2`
- `libopenjp2-7-dev:amd64=2.5.0-2`

Licenses: (parsed from: `/usr/share/doc/libopenjp2-7/copyright`, `/usr/share/doc/libopenjp2-7-dev/copyright`)

- `BSD-2`
- `BSD-3`
- `LIBPNG`
- `LIBTIFF`
- `LIBTIFF-GLARSON`
- `LIBTIFF-PIXAR`
- `MIT`
- `ZLIB`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openjpeg2=2.5.0-2
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.5.0-2.dsc' openjpeg2_2.5.0-2.dsc 2673 SHA256:c29fc2afc7bf6fa1a3d02e9c78dd2159db2ef12a5fe62bc786500c91f01ffc04
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.5.0.orig.tar.xz' openjpeg2_2.5.0.orig.tar.xz 1221108 SHA256:007e19d772c8b6b22e35379630b06ff3549e49ba719d96453607a36ad7b4de73
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.5.0-2.debian.tar.xz' openjpeg2_2.5.0-2.debian.tar.xz 17388 SHA256:7bedc8ba24e39dddc65e3e87f70c5dcced44661d360379efd5077fd24333ee9c
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjpeg2/2.5.0-2/ (for browsing the source)
- https://sources.debian.net/src/openjpeg2/2.5.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjpeg2/2.5.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.5.13+dfsg-5`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.13+dfsg-5`

Licenses: (parsed from: `/usr/share/doc/libldap-2.5-0/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-California`
- `BSD-3-clause-variant`
- `BSD-4-clause-California`
- `Beerware`
- `Expat`
- `Expat-ISC`
- `Expat-UNM`
- `F5`
- `FSF-unlimited`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `GPL-2+ with Libtool exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Autoconf exception`
- `GPL-3+ with Libtool exception`
- `JCG`
- `MIT-XC`
- `NeoSoft-permissive`
- `OpenLDAP-2.8`
- `UMich`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.13+dfsg-5
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg-5.dsc' openldap_2.5.13+dfsg-5.dsc 3233 SHA256:3192f78a46825039c6c9de6808ae98ab3d1c8846f43d2109ed654fd9c33fe472
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg.orig.tar.xz' openldap_2.5.13+dfsg.orig.tar.xz 3727704 SHA256:1d95c400a3eae6730246614ef16883de3dbd1b14b01a1ebe3a9aa1ccad2c13ec
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg-5.debian.tar.xz' openldap_2.5.13+dfsg-5.debian.tar.xz 164516 SHA256:161e22c1c79e2f7c6013cfc2bbf0265d6bbb78d91a0fcfa9ca866837f2c31d88
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.5.13+dfsg-5/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.5.13+dfsg-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.5.13+dfsg-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:9.4p1-1`

Binary Packages:

- `openssh-client=1:9.4p1-1`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:9.4p1-1
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.4p1-1.dsc' openssh_9.4p1-1.dsc 3311 SHA256:1b5f4527537b2e1aee79ba7db11c28ecfd8ba7ee968114ddb494dfd02600d933
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.4p1.orig.tar.gz' openssh_9.4p1.orig.tar.gz 1845094 SHA256:3608fd9088db2163ceb3e600c85ab79d0de3d221e59192ea1923e23263866a85
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.4p1.orig.tar.gz.asc' openssh_9.4p1.orig.tar.gz.asc 833 SHA256:d92592d82bee81745a71bbf249ede02afcdbf933f0de18841a7f17b15b975a03
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.4p1-1.debian.tar.xz' openssh_9.4p1-1.debian.tar.xz 185012 SHA256:3f6b3b4311c3df3eb583228f35ebb5baf3e14c46018ec8ce31e4815f1aa6aa13
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:9.4p1-1/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:9.4p1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:9.4p1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=3.0.11-1`

Binary Packages:

- `libssl-dev:amd64=3.0.11-1`
- `libssl3:amd64=3.0.11-1`
- `openssl=3.0.11-1`

Licenses: (parsed from: `/usr/share/doc/libssl-dev/copyright`, `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.11-1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.11-1.dsc' openssl_3.0.11-1.dsc 2461 SHA256:5f2989f33b3d13f4ad178c2fca493248a801c196b3a7e043844d946e786a6449
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.11.orig.tar.gz' openssl_3.0.11.orig.tar.gz 15198318 SHA256:b3425d3bb4a2218d0697eb41f7fc0cdede016ed19ca49d168b78e8d947887f55
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.11.orig.tar.gz.asc' openssl_3.0.11.orig.tar.gz.asc 833 SHA256:4d8d8d2717a42340af8e94beae3e004b77efc86b19f338411b69a848d06eb609
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.11-1.debian.tar.xz' openssl_3.0.11-1.debian.tar.xz 69048 SHA256:648dcb738546998fa4e8a8a0da2f6e33f3998e074580bb1f22f72ebe6b5a1779
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/3.0.11-1/ (for browsing the source)
- https://sources.debian.net/src/openssl/3.0.11-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/3.0.11-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.25.0-5`

Binary Packages:

- `libp11-kit0:amd64=0.25.0-5`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `LGPL-2.1`
- `LGPL-2.1+`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.25.0-5
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.25.0-5.dsc' p11-kit_0.25.0-5.dsc 2525 SHA256:15c8be6c896e57e317a04e2b6fc7a2b640861a6b99783e2db98d4a9dcf7d4854
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.25.0.orig.tar.xz' p11-kit_0.25.0.orig.tar.xz 958940 SHA256:d55583bcdde83d86579cabe3a8f7f2638675fef01d23cace733ff748fc354706
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.25.0.orig.tar.xz.asc' p11-kit_0.25.0.orig.tar.xz.asc 228 SHA256:ee893a62a368fb807abc678a29279b1c04808ab626b68d5d7085b8b4ab4174c9
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.25.0-5.debian.tar.xz' p11-kit_0.25.0-5.debian.tar.xz 26060 SHA256:5981d442c1af2aa6c3c7b2517f6d7afcddfdf7d036c1fd8378750d74eba28b99
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.25.0-5/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.25.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.25.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.5.2-9.1`

Binary Packages:

- `libpam-modules:amd64=1.5.2-9.1`
- `libpam-modules-bin=1.5.2-9.1`
- `libpam-runtime=1.5.2-9.1`
- `libpam0g:amd64=1.5.2-9.1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `BSD-3-clause`
- `BSD-tcp_wrappers`
- `Beerware`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+ with Bison exception`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pam=1.5.2-9.1
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-9.1.dsc' pam_1.5.2-9.1.dsc 2502 SHA256:d4b7fa6507e266e715b5d8474ef251d18478e5b69f494f41bbcc49122e4ca42b
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA256:e4ec7131a91da44512574268f493c6d8ca105c87091691b8e9b56ca685d4f94d
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-9.1.debian.tar.xz' pam_1.5.2-9.1.debian.tar.xz 130160 SHA256:075dbb4cc5b9cd3260861e9e1f65db17f934ff5c02c574a9fdfe0cb334c2f1b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.5.2-9.1/ (for browsing the source)
- https://sources.debian.net/src/pam/1.5.2-9.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.5.2-9.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pango1.0=1.51.0+ds-3`

Binary Packages:

- `libpango-1.0-0:amd64=1.51.0+ds-3`
- `libpangocairo-1.0-0:amd64=1.51.0+ds-3`
- `libpangoft2-1.0-0:amd64=1.51.0+ds-3`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Apache-2`
- `Apache-2.0`
- `Bitstream-Vera`
- `CC0-1.0`
- `Chromium-BSD-style`
- `Example`
- `GPL-2+`
- `GPL-2.0`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `OFL-1.1`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.51.0+ds-3
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.51.0%2bds-3.dsc' pango1.0_1.51.0+ds-3.dsc 3469 SHA256:71df7252c894a467f82a0192eb0d8cbb7a965c1459e945fc81b80ea9e03f01a4
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.51.0%2bds.orig.tar.xz' pango1.0_1.51.0+ds.orig.tar.xz 1731104 SHA256:df51bb6819e91fda4f6c8ba8d2bd51e437e6f7daa86419d69a15e33a99002170
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.51.0%2bds-3.debian.tar.xz' pango1.0_1.51.0+ds-3.debian.tar.xz 41176 SHA256:ac6cb54c5b31eb5790ff7b9581ff16da0d3d0d7b621b1153be1a65b750c20229
```

Other potentially useful URLs:

- https://sources.debian.net/src/pango1.0/1.51.0+ds-3/ (for browsing the source)
- https://sources.debian.net/src/pango1.0/1.51.0+ds-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pango1.0/1.51.0+ds-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `patch=2.7.6-7`

Binary Packages:

- `patch=2.7.6-7`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-7
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-7.dsc' patch_2.7.6-7.dsc 1706 SHA256:d954fd576d935ac54b7d44d4976eb52d0da84a57f7bad90c6e5bd5e33595030a
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-7.debian.tar.xz' patch_2.7.6-7.debian.tar.xz 15084 SHA256:7725f30b042d8cf63516e480036e93ca2ff0ce5ad3754db4a4e69d33e96a2624
```

Other potentially useful URLs:

- https://sources.debian.net/src/patch/2.7.6-7/ (for browsing the source)
- https://sources.debian.net/src/patch/2.7.6-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/patch/2.7.6-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.42-4`

Binary Packages:

- `libpcre2-16-0:amd64=10.42-4`
- `libpcre2-32-0:amd64=10.42-4`
- `libpcre2-8-0:amd64=10.42-4`
- `libpcre2-dev:amd64=10.42-4`
- `libpcre2-posix3:amd64=10.42-4`

Licenses: (parsed from: `/usr/share/doc/libpcre2-16-0/copyright`, `/usr/share/doc/libpcre2-32-0/copyright`, `/usr/share/doc/libpcre2-8-0/copyright`, `/usr/share/doc/libpcre2-dev/copyright`, `/usr/share/doc/libpcre2-posix3/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-3-clause-Cambridge with BINARY LIBRARY-LIKE PACKAGES exception`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pcre2=10.42-4
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.42-4.dsc' pcre2_10.42-4.dsc 2302 SHA256:2796d9332a4b4abe5eeada4aa287e8f9765a497b4363e3c49815a6bca5845cfe
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.42.orig.tar.gz' pcre2_10.42.orig.tar.gz 2397194 SHA256:c33b418e3b936ee3153de2c61cc638e7e4fe3156022a5c77d0711bcbb9d64f1f
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.42-4.diff.gz' pcre2_10.42-4.diff.gz 8111 SHA256:b583a75e90b029616c6867eccfeb21031e62df98dd4462f9d13ccb95bb2f09e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.42-4/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.42-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.42-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.36.0-9`

Binary Packages:

- `libperl5.36:amd64=5.36.0-9`
- `perl=5.36.0-9`
- `perl-base=5.36.0-9`
- `perl-modules-5.36=5.36.0-9`

Licenses: (parsed from: `/usr/share/doc/libperl5.36/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.36/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/perl/5.36.0-9/


### `dpkg` source package: `pinentry=1.2.1-3`

Binary Packages:

- `pinentry-curses=1.2.1-3`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.2.1-3
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1-3.dsc' pinentry_1.2.1-3.dsc 3170 SHA256:679a692b8a34c68a9146869347a09164d952a4b79dd2daa6ca20a1caa6aed8e8
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1.orig.tar.bz2' pinentry_1.2.1.orig.tar.bz2 547698 SHA256:457a185e5a85238fb945a955dc6352ab962dc8b48720b62fc9fa48c7540a4067
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1.orig.tar.bz2.asc' pinentry_1.2.1.orig.tar.bz2.asc 390 SHA256:9f7d9c7509e4ff4161a043893d76183bd975230fcad671b643c90f78e500ba95
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1-3.debian.tar.xz' pinentry_1.2.1-3.debian.tar.xz 18864 SHA256:7919390ebf6fdf2f8e4e05231bc1348edb119396d29d66718478775bb4c9a0ba
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.2.1-3/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.2.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.2.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pixman=0.42.2-1`

Binary Packages:

- `libpixman-1-0:amd64=0.42.2-1`
- `libpixman-1-dev:amd64=0.42.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.42.2-1
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.42.2-1.dsc' pixman_0.42.2-1.dsc 2021 SHA256:393302f5ba22d1206c456902baa02cdd577cb74fe35ec6659f587cce67b91b3d
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.42.2.orig.tar.gz' pixman_0.42.2.orig.tar.gz 959669 SHA256:ea1480efada2fd948bc75366f7c349e1c96d3297d09a3fe62626e38e234a625e
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.42.2-1.diff.gz' pixman_0.42.2-1.diff.gz 319616 SHA256:dd6472676c68260a298e52f45c485d3cc85c4bf25df8af0f68e37acff7bfed8a
```

Other potentially useful URLs:

- https://sources.debian.net/src/pixman/0.42.2-1/ (for browsing the source)
- https://sources.debian.net/src/pixman/0.42.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pixman/0.42.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pkgconf=1.8.1-1`

Binary Packages:

- `libpkgconf3:amd64=1.8.1-1`
- `pkg-config:amd64=1.8.1-1`
- `pkgconf:amd64=1.8.1-1`
- `pkgconf-bin=1.8.1-1`

Licenses: (parsed from: `/usr/share/doc/libpkgconf3/copyright`, `/usr/share/doc/pkg-config/copyright`, `/usr/share/doc/pkgconf/copyright`, `/usr/share/doc/pkgconf-bin/copyright`)

- `BSD-2`
- `BSD-4`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pkgconf=1.8.1-1
'http://deb.debian.org/debian/pool/main/p/pkgconf/pkgconf_1.8.1-1.dsc' pkgconf_1.8.1-1.dsc 1570 SHA256:cf1f645d7a9522354a334130a55d16be7d62e304070d6675f826844b143dc47e
'http://deb.debian.org/debian/pool/main/p/pkgconf/pkgconf_1.8.1.orig.tar.xz' pkgconf_1.8.1.orig.tar.xz 302372 SHA256:644361ada2942be05655d4452eb018791647c31bba429b287f1f68deb2dc6840
'http://deb.debian.org/debian/pool/main/p/pkgconf/pkgconf_1.8.1-1.debian.tar.xz' pkgconf_1.8.1-1.debian.tar.xz 15060 SHA256:bd9330105d17bf4b9a9d2aaba4a150b35da21b7ba4b45d4bf7e034fa6e53ba2f
```

Other potentially useful URLs:

- https://sources.debian.net/src/pkgconf/1.8.1-1/ (for browsing the source)
- https://sources.debian.net/src/pkgconf/1.8.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pkgconf/1.8.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `postgresql-16=16.1-1`

Binary Packages:

- `libpq-dev=16.1-1`
- `libpq5:amd64=16.1-1`

Licenses: (parsed from: `/usr/share/doc/libpq-dev/copyright`, `/usr/share/doc/libpq5/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-Clause`
- `BSD-3-clause`
- `Custom-Unicode`
- `Custom-pg_dump`
- `Custom-regex`
- `GPL-1`
- `PostgreSQL`
- `Tcl`
- `double-metaphone`
- `nagaysau-ishii`

Source:

```console
$ apt-get source -qq --print-uris postgresql-16=16.1-1
'http://deb.debian.org/debian/pool/main/p/postgresql-16/postgresql-16_16.1-1.dsc' postgresql-16_16.1-1.dsc 4187 SHA256:ca8f7b31e77c2ff09c6ded2c0964fcfd5a61a30b7bd865e9b6debd9c754910cf
'http://deb.debian.org/debian/pool/main/p/postgresql-16/postgresql-16_16.1.orig.tar.bz2' postgresql-16_16.1.orig.tar.bz2 24605482 SHA256:ce3c4d85d19b0121fe0d3f8ef1fa601f71989e86f8a66f7dc3ad546dd5564fec
'http://deb.debian.org/debian/pool/main/p/postgresql-16/postgresql-16_16.1-1.debian.tar.xz' postgresql-16_16.1-1.debian.tar.xz 30640 SHA256:86eb655649921d52b6027e7fa40403ec44e743647962158df5a8c4ebf4ff5294
```

Other potentially useful URLs:

- https://sources.debian.net/src/postgresql-16/16.1-1/ (for browsing the source)
- https://sources.debian.net/src/postgresql-16/16.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/postgresql-16/16.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:4.0.4-2`

Binary Packages:

- `libproc2-0:amd64=2:4.0.4-2`
- `procps=2:4.0.4-2`

Licenses: (parsed from: `/usr/share/doc/libproc2-0/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:4.0.4-2
'http://deb.debian.org/debian/pool/main/p/procps/procps_4.0.4-2.dsc' procps_4.0.4-2.dsc 2136 SHA256:a7f3565d90babda1d74d1b5768771ddbe94f287ea3753ba7c77633d9393d7a5b
'http://deb.debian.org/debian/pool/main/p/procps/procps_4.0.4.orig.tar.xz' procps_4.0.4.orig.tar.xz 1401540 SHA256:22870d6feb2478adb617ce4f09a787addaf2d260c5a8aa7b17d889a962c5e42e
'http://deb.debian.org/debian/pool/main/p/procps/procps_4.0.4-2.debian.tar.xz' procps_4.0.4-2.debian.tar.xz 30368 SHA256:cebb203a49661f27816333b39460a9cc010ac8e425bcbc8ceae92a8c62b8293b
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:4.0.4-2/ (for browsing the source)
- https://sources.debian.net/src/procps/2:4.0.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:4.0.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.11.4-5`

Binary Packages:

- `libpython3-stdlib:amd64=3.11.4-5+b1`
- `python3=3.11.4-5+b1`
- `python3-minimal=3.11.4-5+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.11.4-5
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.11.4-5.dsc' python3-defaults_3.11.4-5.dsc 3001 SHA256:b59a38fa9c9c638e47cdbde5e869d879092ebc09decd32065a2c90ded3574fb8
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.11.4-5.tar.gz' python3-defaults_3.11.4-5.tar.gz 146763 SHA256:170f676b5fdb0c3562aa14ae594f44c01e26e40ddc42ee407add512693cddb25
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3-defaults/3.11.4-5/ (for browsing the source)
- https://sources.debian.net/src/python3-defaults/3.11.4-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3-defaults/3.11.4-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-stdlib-extensions=3.11.5-1`

Binary Packages:

- `python3-distutils=3.11.5-1`
- `python3-lib2to3=3.11.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.11.5-1
'http://deb.debian.org/debian/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.11.5-1.dsc' python3-stdlib-extensions_3.11.5-1.dsc 2563 SHA256:77bcdd358726c6d32e745d0f939ffa2ae72ab04cd585ebfacee0a3ef325b9779
'http://deb.debian.org/debian/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.11.5.orig.tar.xz' python3-stdlib-extensions_3.11.5.orig.tar.xz 1784144 SHA256:563161811d9d8752ad45727130801705b74a60c0cd368560de17f085a10c85c4
'http://deb.debian.org/debian/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.11.5-1.debian.tar.xz' python3-stdlib-extensions_3.11.5-1.debian.tar.xz 29120 SHA256:ebce9a486ed0c0f100a395b9d7feb3992c1104d0b6877b578c0bdbc7f02ef0fe
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3-stdlib-extensions/3.11.5-1/ (for browsing the source)
- https://sources.debian.net/src/python3-stdlib-extensions/3.11.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3-stdlib-extensions/3.11.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3.11=3.11.6-3`

Binary Packages:

- `libpython3.11:amd64=3.11.6-3`
- `libpython3.11-minimal:amd64=3.11.6-3`
- `libpython3.11-stdlib:amd64=3.11.6-3`
- `python3.11=3.11.6-3`
- `python3.11-minimal=3.11.6-3`

Licenses: (parsed from: `/usr/share/doc/libpython3.11/copyright`, `/usr/share/doc/libpython3.11-minimal/copyright`, `/usr/share/doc/libpython3.11-stdlib/copyright`, `/usr/share/doc/python3.11/copyright`, `/usr/share/doc/python3.11-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.11=3.11.6-3
'http://deb.debian.org/debian/pool/main/p/python3.11/python3.11_3.11.6-3.dsc' python3.11_3.11.6-3.dsc 3655 SHA256:6dccbe0a9171577e3a99c794ac4fd1b428651b3f1c04c4e46556f688c2455208
'http://deb.debian.org/debian/pool/main/p/python3.11/python3.11_3.11.6.orig.tar.xz' python3.11_3.11.6.orig.tar.xz 20067204 SHA256:0fab78fa7f133f4f38210c6260d90d7c0d5c7198446419ce057ec7ac2e6f5f38
'http://deb.debian.org/debian/pool/main/p/python3.11/python3.11_3.11.6-3.debian.tar.xz' python3.11_3.11.6-3.debian.tar.xz 213928 SHA256:8175199337b83a7fa566742a5a80b949334076c6fdb87cc9d4c6f01a8d915b61
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.11/3.11.6-3/ (for browsing the source)
- https://sources.debian.net/src/python3.11/3.11.6-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.11/3.11.6-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.2-1.3`

Binary Packages:

- `libreadline-dev:amd64=8.2-1.3`
- `libreadline8:amd64=8.2-1.3`
- `readline-common=8.2-1.3`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ISC-no-attribution`

Source:

```console
$ apt-get source -qq --print-uris readline=8.2-1.3
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.2-1.3.dsc' readline_8.2-1.3.dsc 2553 SHA256:05497ea99bef3f14b8d502cbe3f84fe7bbc0bce1c4f139ca32f0fd60dcac977e
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.2.orig.tar.gz' readline_8.2.orig.tar.gz 3043952 SHA256:3feb7171f16a84ee82ca18a36d7b9be109a52c04f492a053331d7d1095007c35
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.2-1.3.debian.tar.xz' readline_8.2-1.3.debian.tar.xz 30016 SHA256:8cd3c02d6c07b4cf57da607de168a9e347ee05c31857f0f6236fe3df4fc207d9
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/8.2-1.3/ (for browsing the source)
- https://sources.debian.net/src/readline/8.2-1.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/8.2-1.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rpcsvc-proto=1.4.3-1`

Binary Packages:

- `rpcsvc-proto=1.4.3-1`

Licenses: (parsed from: `/usr/share/doc/rpcsvc-proto/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+-autoconf-exception`
- `GPL-3`
- `GPL-3+-autoconf-exception`
- `MIT`
- `permissive-autoconf-m4`
- `permissive-autoconf-m4-no-warranty`
- `permissive-configure`
- `permissive-fsf`
- `permissive-makefile-in`

Source:

```console
$ apt-get source -qq --print-uris rpcsvc-proto=1.4.3-1
'http://deb.debian.org/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.3-1.dsc' rpcsvc-proto_1.4.3-1.dsc 1999 SHA256:7d8e122bd18b02fe0de6d467a0ecdafff74035b3e1ed0da1c0c792d9c015682f
'http://deb.debian.org/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.3.orig.tar.xz' rpcsvc-proto_1.4.3.orig.tar.xz 167964 SHA256:69315e94430f4e79c74d43422f4a36e6259e97e67e2677b2c7d7060436bd99b1
'http://deb.debian.org/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.3-1.debian.tar.xz' rpcsvc-proto_1.4.3-1.debian.tar.xz 4228 SHA256:02034b9dadcf3af5424f72eb65c3842c8d7117b6b78e7a3c798316ceb60843d1
```

Other potentially useful URLs:

- https://sources.debian.net/src/rpcsvc-proto/1.4.3-1/ (for browsing the source)
- https://sources.debian.net/src/rpcsvc-proto/1.4.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rpcsvc-proto/1.4.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2+b2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc 2299 SHA256:a296819cd2ab5880b67ad963ef0867cb10e462f4403e52565aa863eb05bb1370
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz 8096 SHA256:26d47de07d16285e4ca55b0828cbbf1ba35e671f9b3500a87e301fe755d26882
```

Other potentially useful URLs:

- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for browsing the source)
- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rust-sequoia-sq=0.31.0-1`

Binary Packages:

- `sq=0.31.0-1`

Licenses: (parsed from: `/usr/share/doc/sq/copyright`)

- `GPL-2`
- `GPL-2.0-or-later`

Source:

```console
$ apt-get source -qq --print-uris rust-sequoia-sq=0.31.0-1
'http://deb.debian.org/debian/pool/main/r/rust-sequoia-sq/rust-sequoia-sq_0.31.0-1.dsc' rust-sequoia-sq_0.31.0-1.dsc 3484 SHA256:3a7bc61f40ff0153604638a59d5f9be9a3437551e6911dfc06b2bca8164564c6
'http://deb.debian.org/debian/pool/main/r/rust-sequoia-sq/rust-sequoia-sq_0.31.0.orig.tar.gz' rust-sequoia-sq_0.31.0.orig.tar.gz 369161 SHA256:38ce1b60431fcda2821cb257f9d124a3046e3b57d84a1a356f9d54d1cff6a6c4
'http://deb.debian.org/debian/pool/main/r/rust-sequoia-sq/rust-sequoia-sq_0.31.0-1.debian.tar.xz' rust-sequoia-sq_0.31.0-1.debian.tar.xz 4144 SHA256:201210cc51a60cbab26abdcc60b85d86ac31b8bb653f02cc30ddf09652d06eb6
```

Other potentially useful URLs:

- https://sources.debian.net/src/rust-sequoia-sq/0.31.0-1/ (for browsing the source)
- https://sources.debian.net/src/rust-sequoia-sq/0.31.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rust-sequoia-sq/0.31.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.9-1`

Binary Packages:

- `sed=4.9-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `BSD-4-clause-UC`
- `BSL-1`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `X11`
- `pcre`

Source:

```console
$ apt-get source -qq --print-uris sed=4.9-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9-1.dsc' sed_4.9-1.dsc 2077 SHA256:f0670e00c1ad51321e5b741a737e977cdb3b0eef47964b2269535f7820df576a
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9.orig.tar.xz' sed_4.9.orig.tar.xz 1397092 SHA256:6e226b732e1cd739464ad6862bd1a1aba42d7982922da7a53519631d24975181
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9.orig.tar.xz.asc' sed_4.9.orig.tar.xz.asc 833 SHA256:9ea64f215b308ae0a80cd958daaac23bb13491d69a472a0195974d107890a8c6
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9-1.debian.tar.xz' sed_4.9-1.debian.tar.xz 62616 SHA256:24cdd6a3b40909ec374bd87df62364904bbe18fc12ba66111e9f9f617ff7f679
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.9-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sensible-utils=0.0.20`

Binary Packages:

- `sensible-utils=0.0.20`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.20
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.20.dsc' sensible-utils_0.0.20.dsc 1737 SHA256:8021b5c0ee69ed3429e0a48a4bfa0fe0e8f3937ec24b29a82eb144e86a3afe7b
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.20.tar.xz' sensible-utils_0.0.20.tar.xz 70608 SHA256:b8cfd2dd268b3d982cc8e94af573b3e72e7917b2fa6f28eaa5e056ad99212edb
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.20/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.20/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.20/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serf=1.3.10-1`

Binary Packages:

- `libserf-1-1:amd64=1.3.10-1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.10-1/


### `dpkg` source package: `setuptools=68.1.2-2`

Binary Packages:

- `python3-pkg-resources=68.1.2-2`

Licenses: (parsed from: `/usr/share/doc/python3-pkg-resources/copyright`)

- `Apache-2.0`
- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris setuptools=68.1.2-2
'http://deb.debian.org/debian/pool/main/s/setuptools/setuptools_68.1.2-2.dsc' setuptools_68.1.2-2.dsc 2237 SHA256:ca80c8179d0499e8d386245b3f9fc4ae2021e7388bebe4c8d5ce9e8f6c360bad
'http://deb.debian.org/debian/pool/main/s/setuptools/setuptools_68.1.2.orig.tar.gz' setuptools_68.1.2.orig.tar.gz 2198001 SHA256:3d4dfa6d95f1b101d695a6160a7626e15583af71a5f52176efa5d39a054d475d
'http://deb.debian.org/debian/pool/main/s/setuptools/setuptools_68.1.2-2.debian.tar.xz' setuptools_68.1.2-2.debian.tar.xz 14160 SHA256:a0ba63b09f24281a4535783fe581b93d58a48144c40c469028deeeaf865bc297
```

Other potentially useful URLs:

- https://sources.debian.net/src/setuptools/68.1.2-2/ (for browsing the source)
- https://sources.debian.net/src/setuptools/68.1.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/setuptools/68.1.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shadow=1:4.13+dfsg1-3`

Binary Packages:

- `login=1:4.13+dfsg1-3`
- `passwd=1:4.13+dfsg1-3`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.13+dfsg1-3
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1-3.dsc' shadow_4.13+dfsg1-3.dsc 2407 SHA256:13f79d61847c6ea525dcde26bb71b99d24b4d15cbbebf5070537c9a8caa50a52
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1.orig.tar.xz' shadow_4.13+dfsg1.orig.tar.xz 1811752 SHA256:a8bb3a2aceff1cbe39d0f50687dcc1d7e7be0516a9d954d8e2eedb93f5906207
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1-3.debian.tar.xz' shadow_4.13+dfsg1-3.debian.tar.xz 82360 SHA256:4fac3636727d73b660d18d084532e2bcc7d6bf5632b5e3c2897aae9cad4a9d8e
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.13+dfsg1-3/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.13+dfsg1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.13+dfsg1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shared-mime-info=2.2-1`

Binary Packages:

- `shared-mime-info=2.2-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/shared-mime-info/2.2-1/


### `dpkg` source package: `sqlite3=3.44.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.44.0-1`
- `libsqlite3-dev:amd64=3.44.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.44.0-1
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.44.0-1.dsc' sqlite3_3.44.0-1.dsc 2486 SHA256:96a38faad95351e5f582ef7e2b47818de46dd95970e250439257d0f9a75f9322
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.44.0.orig-www.tar.xz' sqlite3_3.44.0.orig-www.tar.xz 5666172 SHA256:cf24a5656149b30e3400213b69f67d962d11655b04f95314bba60ed17d15128f
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.44.0.orig.tar.xz' sqlite3_3.44.0.orig.tar.xz 8207892 SHA256:03dad73b293bd1cb87a0e304f554af7886b2158980c92779fe6ec0373d9a9dad
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.44.0-1.debian.tar.xz' sqlite3_3.44.0-1.debian.tar.xz 30180 SHA256:80cdbf341d29e3f67d675326b0e4c5822da6002c6a6dfbc27576fdd09bbbb68a
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.44.0-1/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.44.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.44.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `subversion=1.14.2-5`

Binary Packages:

- `libsvn1:amd64=1.14.2-5`
- `subversion=1.14.2-5`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `AFL-3`
- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BoostAcMacros`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `Svnwrap`
- `Unicode`
- `Utfwidth`

Source:

```console
$ apt-get source -qq --print-uris subversion=1.14.2-5
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2-5.dsc' subversion_1.14.2-5.dsc 4046 SHA256:440238a21f27f8c77d47a7349930e78efbdbad944211aed3ab5a8b3a238d9283
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2.orig.tar.gz' subversion_1.14.2.orig.tar.gz 11626792 SHA256:fd826afad03db7a580722839927dc664f3e93398fe88b66905732c8530971353
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2.orig.tar.gz.asc' subversion_1.14.2.orig.tar.gz.asc 3215 SHA256:da6a0a5ff56f671ad2d1eae708f8d1cc1abf0485b029a163ff8272cba5475861
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2-5.debian.tar.xz' subversion_1.14.2-5.debian.tar.xz 337732 SHA256:a898a4f010a730860bd592eda28822c55751c1b83303d4cf050f9684cf8692e5
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.14.2-5/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.14.2-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.14.2-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=254.5-1`

Binary Packages:

- `libsystemd0:amd64=254.5-1`
- `libudev1:amd64=254.5-1`

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
$ apt-get source -qq --print-uris systemd=254.5-1
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_254.5-1.dsc' systemd_254.5-1.dsc 6890 SHA256:ee14c2e5e98ada43cb95004fcf8ada5ba7819973aa84328f78c056e85a1602c8
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_254.5.orig.tar.gz' systemd_254.5.orig.tar.gz 14334696 SHA256:41873783aa1c680e10d2f2626797a1c2fef8018d69b68c8c77639e140ee7846d
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_254.5-1.debian.tar.xz' systemd_254.5-1.debian.tar.xz 163340 SHA256:1132c18a30ad454307df343f4b6182eb2d9d8028c0b33835730a35f447d450e8
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/254.5-1/ (for browsing the source)
- https://sources.debian.net/src/systemd/254.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/254.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=3.08-3`

Binary Packages:

- `sysvinit-utils=3.08-3`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.08-3
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.08-3.dsc' sysvinit_3.08-3.dsc 2359 SHA256:d2a262316ce2a141b46f21c4cbaa0a9308fd8de47fb1a61eba8ea17eca52006e
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.08.orig.tar.gz' sysvinit_3.08.orig.tar.gz 513674 SHA256:325e42ae4ae5ae3e4d989e0604aeb5e4eae5f3ee21e401db3c79000718f8c836
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.08-3.debian.tar.xz' sysvinit_3.08-3.debian.tar.xz 137976 SHA256:56d9e48a636ddb13f0bdba837692020f39501605b378142416a7848725075d28
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/3.08-3/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/3.08-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/3.08-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.34+dfsg-1.2`

Binary Packages:

- `tar=1.34+dfsg-1.2`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1.2
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg-1.2.dsc' tar_1.34+dfsg-1.2.dsc 1768 SHA256:4e7999f6d8a7fef2d09aa5b915877357a80c68ab0a339ee802b304d0e99e7517
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA256:7d57029540cb928394defb3b377b3531237c947e795b51aa8acac0c5ba0e4844
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg-1.2.debian.tar.xz' tar_1.34+dfsg-1.2.debian.tar.xz 20336 SHA256:6e32291771f375a7e08cc4cabad1a658327d3dd7a4ff1b557a338ffe0675a25c
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.34+dfsg-1.2/ (for browsing the source)
- https://sources.debian.net/src/tar/1.34+dfsg-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.34+dfsg-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.5.1+git230720-1`

Binary Packages:

- `libtiff-dev:amd64=4.5.1+git230720-1`
- `libtiff6:amd64=4.5.1+git230720-1`
- `libtiffxx6:amd64=4.5.1+git230720-1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff6/copyright`, `/usr/share/doc/libtiffxx6/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.5.1+git230720-1
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.5.1%2bgit230720-1.dsc' tiff_4.5.1+git230720-1.dsc 2322 SHA256:4c19ac8cd08472e55ed12ad449d883cd2cabb7d7c0845234847e24817a9e0511
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.5.1%2bgit230720.orig.tar.xz' tiff_4.5.1+git230720.orig.tar.xz 1781896 SHA256:0e51bcf3a3ffa5fc76ea6aeb74a797f95c84544fcc8b6a1ec5def967a78e9e12
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.5.1%2bgit230720-1.debian.tar.xz' tiff_4.5.1+git230720-1.debian.tar.xz 21964 SHA256:eb3299ba003f5a6ac414ef10bc2e4fb6607ef7366a4c8dc6127a82fa916e3c73
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.5.1+git230720-1/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.5.1+git230720-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.5.1+git230720-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2023c-10`

Binary Packages:

- `tzdata=2023c-10`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tzdata/2023c-10/


### `dpkg` source package: `ucf=3.0043+nmu1`

Binary Packages:

- `ucf=3.0043+nmu1`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0043+nmu1
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0043%2bnmu1.dsc' ucf_3.0043+nmu1.dsc 1567 SHA256:5ef70fa7a58cd3f162932661453a1e9d21d749b47a1aa84198f7c4cd9eac20ee
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0043%2bnmu1.tar.xz' ucf_3.0043+nmu1.tar.xz 70916 SHA256:a07143046236cb082517e346362306cb3fe4d3634cad1add40c905b0e0ecf58c
```

Other potentially useful URLs:

- https://sources.debian.net/src/ucf/3.0043+nmu1/ (for browsing the source)
- https://sources.debian.net/src/ucf/3.0043+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ucf/3.0043+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unzip=6.0-28`

Binary Packages:

- `unzip=6.0-28`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-28
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-28.dsc' unzip_6.0-28.dsc 1359 SHA256:f5b486028b61a145b591fdd96aaeaf89ef6eef164a299f43bd5e6704bdefc8a2
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-28.debian.tar.xz' unzip_6.0-28.debian.tar.xz 25032 SHA256:e51364116c84739c591728ecc841113a914fa11358fd10ff0d6813524d811bb9
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-28/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-28/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-28/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `usrmerge=38`

Binary Packages:

- `usr-is-merged=38`

Licenses: (parsed from: `/usr/share/doc/usr-is-merged/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=38
'http://deb.debian.org/debian/pool/main/u/usrmerge/usrmerge_38.dsc' usrmerge_38.dsc 981 SHA256:c23401bc61750179515ec2bb12303e42f6f839542c5d413ce5db7192ff1527bc
'http://deb.debian.org/debian/pool/main/u/usrmerge/usrmerge_38.tar.xz' usrmerge_38.tar.xz 14804 SHA256:bc1a7973777560f5be67763abd9c1c1ff239d423f72e9209ad755f94e921d4e0
```

Other potentially useful URLs:

- https://sources.debian.net/src/usrmerge/38/ (for browsing the source)
- https://sources.debian.net/src/usrmerge/38/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/usrmerge/38/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `utf8proc=2.9.0-1`

Binary Packages:

- `libutf8proc3:amd64=2.9.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc3/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.9.0-1
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.9.0-1.dsc' utf8proc_2.9.0-1.dsc 2187 SHA256:bb9fd54cb4584ee7c677901312608249f503aa910ca60db043d3273b86dd228a
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.9.0.orig.tar.gz' utf8proc_2.9.0.orig.tar.gz 193465 SHA256:18c1626e9fc5a2e192311e36b3010bfc698078f692888940f1fa150547abb0c1
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.9.0-1.debian.tar.xz' utf8proc_2.9.0-1.debian.tar.xz 5836 SHA256:b285489bb5d293ce24d2eea42450f3ef15ff13a23fc422de6a0cf5760872f789
```

Other potentially useful URLs:

- https://sources.debian.net/src/utf8proc/2.9.0-1/ (for browsing the source)
- https://sources.debian.net/src/utf8proc/2.9.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/utf8proc/2.9.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.39.2-6`

Binary Packages:

- `bsdutils=1:2.39.2-6`
- `libblkid-dev:amd64=2.39.2-6`
- `libblkid1:amd64=2.39.2-6`
- `libmount-dev:amd64=2.39.2-6`
- `libmount1:amd64=2.39.2-6`
- `libsmartcols1:amd64=2.39.2-6`
- `libuuid1:amd64=2.39.2-6`
- `mount=2.39.2-6`
- `util-linux=2.39.2-6`
- `uuid-dev:amd64=2.39.2-6`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

- `BSD-3-clause`
- `BSD-4-clause`
- `BSLA`
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
$ apt-get source -qq --print-uris util-linux=2.39.2-6
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.39.2-6.dsc' util-linux_2.39.2-6.dsc 4601 SHA256:42b2a38031c85c2383bfdd4eba1f75d1e06946e6ebf9b9fb4ecd48b5fb3eee39
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.39.2.orig.tar.xz' util-linux_2.39.2.orig.tar.xz 8362220 SHA256:87abdfaa8e490f8be6dde976f7c80b9b5ff9f301e1b67e3899e1f05a59a1531f
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.39.2-6.debian.tar.xz' util-linux_2.39.2-6.debian.tar.xz 99836 SHA256:47143ceff6893470cd29d7afdff010df62ac18f84bedc6a9f9ac32e1c1d6039c
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.39.2-6/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.39.2-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.39.2-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.21.4-1`

Binary Packages:

- `wget=1.21.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21.4-1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.4-1.dsc' wget_1.21.4-1.dsc 2167 SHA256:885f3b8acfeaa27119296d18e2624cc80788670e585692375e82f381d2b99f3b
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.4.orig.tar.gz' wget_1.21.4.orig.tar.gz 5059591 SHA256:81542f5cefb8faacc39bbbc6c82ded80e3e4a88505ae72ea51df27525bcde04c
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.4.orig.tar.gz.asc' wget_1.21.4.orig.tar.gz.asc 854 SHA256:fb1ce21577dee962be8bf95cbf86f806815778264622a5d756324ff8dd3bfc57
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.4-1.debian.tar.xz' wget_1.21.4-1.debian.tar.xz 60692 SHA256:88857f1f61992bbbaa591149be2caf1cad9327c8c02c68a5ae6d078ed8f3678c
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.21.4-1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.21.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.21.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorg-sgml-doctools=1:1.11-1.1`

Binary Packages:

- `xorg-sgml-doctools=1:1.11-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xorg-sgml-doctools=1:1.11-1.1
'http://deb.debian.org/debian/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.1.dsc' xorg-sgml-doctools_1.11-1.1.dsc 1987 SHA256:6aac68e597386c10b02646d2026a833d301749a938701f4ca8efd4d19ad34295
'http://deb.debian.org/debian/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11.orig.tar.gz' xorg-sgml-doctools_1.11.orig.tar.gz 150367 SHA256:986326d7b4dd2ad298f61d8d41fe3929ac6191c6000d6d7e47a8ffc0c34e7426
'http://deb.debian.org/debian/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.1.diff.gz' xorg-sgml-doctools_1.11-1.1.diff.gz 3296 SHA256:0c11e15d4f9aaacd38452a6a37d064f1a07058dcead7ab1e2aca223ec0a94d11
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg-sgml-doctools/1:1.11-1.1/ (for browsing the source)
- https://sources.debian.net/src/xorg-sgml-doctools/1:1.11-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg-sgml-doctools/1:1.11-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorg=1:7.7+23`

Binary Packages:

- `x11-common=1:7.7+23`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+23
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7%2b23.dsc' xorg_7.7+23.dsc 1975 SHA256:b06ef48b56736e0a0a48bcbc1afd2cf6dcd70959c2b52e195456a0392076469c
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7%2b23.tar.gz' xorg_7.7+23.tar.gz 287306 SHA256:8458b8798d7d6098cd5259abc447d6c7a371e20e641cac82cf635296a71f468e
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg/1:7.7+23/ (for browsing the source)
- https://sources.debian.net/src/xorg/1:7.7+23/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg/1:7.7+23/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorgproto=2023.2-1`

Binary Packages:

- `x11proto-core-dev=2023.2-1`
- `x11proto-dev=2023.2-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2023.2-1
'http://deb.debian.org/debian/pool/main/x/xorgproto/xorgproto_2023.2-1.dsc' xorgproto_2023.2-1.dsc 3336 SHA256:5523815aa46b9117908d8d40293b7839521c6e0bbaa9215c2e930f82d9a6a96d
'http://deb.debian.org/debian/pool/main/x/xorgproto/xorgproto_2023.2.orig.tar.gz' xorgproto_2023.2.orig.tar.gz 1150326 SHA256:c791aad9b5847781175388ebe2de85cb5f024f8dabf526d5d699c4f942660cc3
'http://deb.debian.org/debian/pool/main/x/xorgproto/xorgproto_2023.2.orig.tar.gz.asc' xorgproto_2023.2.orig.tar.gz.asc 195 SHA256:a544543e30994ee840253b85b8a96b05bd3eef07c3259ea53a143ffed76d85e6
'http://deb.debian.org/debian/pool/main/x/xorgproto/xorgproto_2023.2-1.diff.gz' xorgproto_2023.2-1.diff.gz 25092 SHA256:82e5698318de7e2566a782f5c117d555130cba6bb7721cfea4c5dab49b302803
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorgproto/2023.2-1/ (for browsing the source)
- https://sources.debian.net/src/xorgproto/2023.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorgproto/2023.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xtrans=1.4.0-1`

Binary Packages:

- `xtrans-dev=1.4.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xtrans=1.4.0-1
'http://deb.debian.org/debian/pool/main/x/xtrans/xtrans_1.4.0-1.dsc' xtrans_1.4.0-1.dsc 1919 SHA256:dd74ab9199e8f45215b566a9317cac7953bf063ce6893c185eccaf0fb4d84d8f
'http://deb.debian.org/debian/pool/main/x/xtrans/xtrans_1.4.0.orig.tar.gz' xtrans_1.4.0.orig.tar.gz 225941 SHA256:48ed850ce772fef1b44ca23639b0a57e38884045ed2cbb18ab137ef33ec713f9
'http://deb.debian.org/debian/pool/main/x/xtrans/xtrans_1.4.0-1.diff.gz' xtrans_1.4.0-1.diff.gz 9522 SHA256:0dac18165654d79e0796b80fab4c1104998d29e6d0b098af0426a1d72399521e
```

Other potentially useful URLs:

- https://sources.debian.net/src/xtrans/1.4.0-1/ (for browsing the source)
- https://sources.debian.net/src/xtrans/1.4.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xtrans/1.4.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xxhash=0.8.2-2`

Binary Packages:

- `libxxhash0:amd64=0.8.2-2`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.2-2
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.2-2.dsc' xxhash_0.8.2-2.dsc 1969 SHA256:8fbf9f5a50a4cf48e771e157e386bd2b2938e46cecd4bc53117ee1a4a615af1d
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.2.orig.tar.gz' xxhash_0.8.2.orig.tar.gz 1141188 SHA256:baee0c6afd4f03165de7a4e67988d16f0f2b257b51d0e3cb91909302a26a79c4
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.2-2.debian.tar.xz' xxhash_0.8.2-2.debian.tar.xz 4920 SHA256:fcbdd52df60936173524743680f6d3c504b9a90553fe113cd0aa531faf4f2c4d
```

Other potentially useful URLs:

- https://sources.debian.net/src/xxhash/0.8.2-2/ (for browsing the source)
- https://sources.debian.net/src/xxhash/0.8.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xxhash/0.8.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.4.4-0.1`

Binary Packages:

- `liblzma-dev:amd64=5.4.4-0.1`
- `liblzma5:amd64=5.4.4-0.1`
- `xz-utils=5.4.4-0.1`

Licenses: (parsed from: `/usr/share/doc/liblzma-dev/copyright`, `/usr/share/doc/liblzma5/copyright`, `/usr/share/doc/xz-utils/copyright`)

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
$ apt-get source -qq --print-uris xz-utils=5.4.4-0.1
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.4-0.1.dsc' xz-utils_5.4.4-0.1.dsc 2451 SHA256:226881b3eb04cf6daa86452391225ee9831a824f20016623924cf31ad2119e63
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.4.orig.tar.xz' xz-utils_5.4.4.orig.tar.xz 1661456 SHA256:705d0d96e94e1840e64dec75fc8d5832d34f6649833bec1ced9c3e08cf88132e
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.4.orig.tar.xz.asc' xz-utils_5.4.4.orig.tar.xz.asc 833 SHA256:549a8014a39535bb1489151d543d4e4ba71a83dc690600e39ab8f4890fa90979
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.4-0.1.debian.tar.xz' xz-utils_5.4.4-0.1.debian.tar.xz 26840 SHA256:ff9ac3ebbfdf6766706ec7538fb4083837b1ce179e2bc724f19e3c2c01fcbc5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.4.4-0.1/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.4.4-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.4.4-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.13.dfsg-3`

Binary Packages:

- `zlib1g:amd64=1:1.2.13.dfsg-3`
- `zlib1g-dev:amd64=1:1.2.13.dfsg-3`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.13.dfsg-3
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.13.dfsg-3.dsc' zlib_1.2.13.dfsg-3.dsc 2571 SHA256:c8727df9e01126381fb0f2f9aa5f21f09c2e562ec0a0e7b23c0729328b5dfb83
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.13.dfsg.orig.tar.bz2' zlib_1.2.13.dfsg.orig.tar.bz2 1239825 SHA256:71feb7947e3c00ef125f83b79a4e529bde31171e5babe48b391f06758d1ab0a1
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.13.dfsg-3.debian.tar.xz' zlib_1.2.13.dfsg-3.debian.tar.xz 16688 SHA256:ee3d6f346c3efc09ea92a42e1937db602ea5895c383e524ba9048df80069a8b4
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.13.dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.13.dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.13.dfsg-3/ (for access to the source package after it no longer exists in the archive)
