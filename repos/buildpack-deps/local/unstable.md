# `buildpack-deps:sid`

## Docker Metadata

- Image ID: `sha256:54138805f9191923bd18fae65421f211dad9ebf7d18c4e55fc9f640874f0b585`
- Created: `2021-11-17T03:19:08.873877437Z`
- Virtual Size: ~ 1.20 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.3.1-1`

Binary Packages:

- `libacl1:amd64=2.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.3.1-1
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-1.dsc' acl_2.3.1-1.dsc 2486 SHA256:6299780e84c240e79aae9886deaacc1bd8439a2a58f6a23749156f8a4d62572e
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz' acl_2.3.1.orig.tar.xz 355676 SHA256:c0234042e17f11306c23c038b08e5e070edb7be44bef6697fb8734dcff1c66b1
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz.asc' acl_2.3.1.orig.tar.xz.asc 833 SHA256:54fb8fcd6ae6901f2257e18d503e5e18ad956babf8d80d2ea29f280fc7264662
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-1.debian.tar.xz' acl_2.3.1-1.debian.tar.xz 27732 SHA256:900e8993f3a8b95e2c83fc7f530cc15b5cd165b6f517a639239f51cd60d06f2a
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/acl/2.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.118`

Binary Packages:

- `adduser=3.118`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.118
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.118.dsc' adduser_3.118.dsc 1670 SHA256:fc79bc37fcf5e5700546c78a80670bb7b34836d012595b343fe2304cac82917d
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.118.tar.xz' adduser_3.118.tar.xz 212280 SHA256:3e9eea661c9aac6b2c791bfcc1de3a9c6a422d45c8f3d38ed417737ed3166ffc
```

Other potentially useful URLs:

- https://sources.debian.net/src/adduser/3.118/ (for browsing the source)
- https://sources.debian.net/src/adduser/3.118/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adduser/3.118/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `aom=3.2.0-1`

Binary Packages:

- `libaom3:amd64=3.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libaom3/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `ISC`
- `public-domain-md5`

Source:

```console
$ apt-get source -qq --print-uris aom=3.2.0-1
'http://deb.debian.org/debian/pool/main/a/aom/aom_3.2.0-1.dsc' aom_3.2.0-1.dsc 2178 SHA256:ae7cbb1d1ba1227f4c43e8cc31a21c0269e6451a1a08b4c784aaa0d863418b4e
'http://deb.debian.org/debian/pool/main/a/aom/aom_3.2.0.orig.tar.gz' aom_3.2.0.orig.tar.gz 4728473 SHA256:ef49182f99f73c231e650211584a80fdedd6ab319be06b3fad4ffcb56dbc3627
'http://deb.debian.org/debian/pool/main/a/aom/aom_3.2.0-1.debian.tar.xz' aom_3.2.0-1.debian.tar.xz 10836 SHA256:dbcbca1999bfa2dd21ae7994c17558195573b6d689c8f9f1d217cb779e25de26
```

Other potentially useful URLs:

- https://sources.debian.net/src/aom/3.2.0-1/ (for browsing the source)
- https://sources.debian.net/src/aom/3.2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/aom/3.2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr-util=1.6.1-5`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-5
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1-5.dsc' apr-util_1.6.1-5.dsc 2754 SHA256:dab17dcb495ae31448ceb506448a5b1a6155ae9771073950227c47e09241b9d6
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2.asc' apr-util_1.6.1.orig.tar.bz2.asc 801 SHA256:47837b605290c0d7659b73734e4a9d5e6c0c24c13185cd4d91837afe63c07ca4
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1-5.debian.tar.xz' apr-util_1.6.1-5.debian.tar.xz 342000 SHA256:9489fa1228c0e7362f4a4d099c015b7552b928b7d73c9d79b6d4c16b52edce3b
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr-util/1.6.1-5/ (for browsing the source)
- https://sources.debian.net/src/apr-util/1.6.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr-util/1.6.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr=1.7.0-8`

Binary Packages:

- `libapr1:amd64=1.7.0-8`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-8
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0-8.dsc' apr_1.7.0-8.dsc 2272 SHA256:f13890ccea0e69493c1d2172bf5b733e4b989931c44d150eb496bf88db55a528
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA256:e2e148f0b2e99b8e5c6caa09f6d4fb4dd3e83f744aa72a952f94f5a14436f7ea
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA256:5a6c4e721ed82116d7877254ae11c076014040af2ff816ea15ec81e77a4a7d43
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0-8.debian.tar.xz' apr_1.7.0-8.debian.tar.xz 215848 SHA256:a412ee67df3c7159d67e698293be83a3edc33ee086a35a385420de1a81a11b08
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.7.0-8/ (for browsing the source)
- https://sources.debian.net/src/apr/1.7.0-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.7.0-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=2.3.11`

Binary Packages:

- `apt=2.3.11`
- `libapt-pkg6.0:amd64=2.3.11`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.3.11/


### `dpkg` source package: `attr=1:2.5.1-1`

Binary Packages:

- `libattr1:amd64=1:2.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.5.1-1
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-1.dsc' attr_2.5.1-1.dsc 2455 SHA256:c0bd0dcb0309cdcbd286b31bd97b2c93552ebb7f7634964f351098cd9191e132
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA256:db448a626f9313a1a970d636767316a8da32aede70518b8050fa0de7947adc32
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA256:67bc632e754efbadba846d0b40138b3fc3e306c3b909a9ba868c6dba1e2689d0
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-1.debian.tar.xz' attr_2.5.1-1.debian.tar.xz 27948 SHA256:7eb32437dca67cd24667432150dcb07d8c7d0526e1d3284ecef6833b35214cdf
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.5.1-1/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.5.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.5.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:3.0.6-1`

Binary Packages:

- `libaudit-common=1:3.0.6-1`
- `libaudit1:amd64=1:3.0.6-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0.6-1
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.6-1.dsc' audit_3.0.6-1.dsc 2401 SHA256:20e84a2933e4c9bf40fb18830e513f031cd328204db8e7d216d8c4ad36b93c1b
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.6.orig.tar.gz' audit_3.0.6.orig.tar.gz 1190011 SHA256:c3e44d77513a42401d417dd0ceb203cf23886cb89402dea7b9494faa3f4fcc5e
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.6-1.debian.tar.xz' audit_3.0.6-1.debian.tar.xz 17644 SHA256:5db82720581a87fb5338a229f1f4f47fdb1b2358ca52eee2219b39d3b4694358
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:3.0.6-1/ (for browsing the source)
- https://sources.debian.net/src/audit/1:3.0.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:3.0.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `autoconf=2.71-2`

Binary Packages:

- `autoconf=2.71-2`

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
$ apt-get source -qq --print-uris autoconf=2.71-2
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.71-2.dsc' autoconf_2.71-2.dsc 1988 SHA256:1b0263feeaedb0ab187f648015bf1f4a2751589fd2de5d24b9753a42367fa0f4
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.71.orig.tar.gz' autoconf_2.71.orig.tar.gz 2003781 SHA256:431075ad0bf529ef13cb41e9042c542381103e80015686222b8a9d4abef42a1c
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.71-2.debian.tar.xz' autoconf_2.71-2.debian.tar.xz 23588 SHA256:89237343fc74050a83c0e43221d3fff46e7441391d90b099efc5ceedab0f8efc
```

Other potentially useful URLs:

- https://sources.debian.net/src/autoconf/2.71-2/ (for browsing the source)
- https://sources.debian.net/src/autoconf/2.71-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autoconf/2.71-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `automake-1.16=1:1.16.5-1.1`

Binary Packages:

- `automake=1:1.16.5-1.1`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.5-1.1
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.1.dsc' automake-1.16_1.16.5-1.1.dsc 2575 SHA256:f96f0c588fac5d96f912a26b5ad1bd2bd2a3a29d4e30959e008d1878ab34a90b
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz' automake-1.16_1.16.5.orig.tar.xz 1601740 SHA256:f01d58cd6d9d77fbdca9eb4bbd5ead1988228fdb73d6f7a201f5f8d6b118b469
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz.asc' automake-1.16_1.16.5.orig.tar.xz.asc 833 SHA256:3a161ab65921eed55e1a94251d97c8451d4ba3431b55ca560e95a951b5f1d73a
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.1.debian.tar.xz' automake-1.16_1.16.5-1.1.debian.tar.xz 13320 SHA256:208b8e5e74c30232e6d9c671e274fe4e5c842f6e0ea5620813fefa1f1d77eb7c
```

Other potentially useful URLs:

- https://sources.debian.net/src/automake-1.16/1:1.16.5-1.1/ (for browsing the source)
- https://sources.debian.net/src/automake-1.16/1:1.16.5-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/automake-1.16/1:1.16.5-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `autotools-dev=20180224.1+nmu1`

Binary Packages:

- `autotools-dev=20180224.1+nmu1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1+nmu1
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20180224.1+nmu1.dsc' autotools-dev_20180224.1+nmu1.dsc 1663 SHA256:622d1a0b778f7a6b253d37cecb0855d90feb24f15f100d909a18d247085a318c
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20180224.1+nmu1.tar.xz' autotools-dev_20180224.1+nmu1.tar.xz 68356 SHA256:f2ad12c23d0867b59568f9c7959233446c90556dededc78f588cec7468d04fd5
```

Other potentially useful URLs:

- https://sources.debian.net/src/autotools-dev/20180224.1+nmu1/ (for browsing the source)
- https://sources.debian.net/src/autotools-dev/20180224.1+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autotools-dev/20180224.1+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=12`

Binary Packages:

- `base-files=12`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=12
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_12.dsc' base-files_12.dsc 1070 SHA256:e6395fdfd68ae68fcc274496fefc3cacbcb6381563d44d8037ba234f1a1ff138
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_12.tar.xz' base-files_12.tar.xz 65564 SHA256:4daebec9549c4f52c39a869bc811bceb2a0e1ac7fce5f4d6e37ddf1fdad7335d
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/12/ (for browsing the source)
- https://sources.debian.net/src/base-files/12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.52`

Binary Packages:

- `base-passwd=3.5.52`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.52
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.52.dsc' base-passwd_3.5.52.dsc 1757 SHA256:a62beb1b7131e457c445df5aed4792c9aa673521174179205f805d6ec5900f54
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.52.tar.xz' base-passwd_3.5.52.tar.xz 54336 SHA256:5dfec6556b5a16ecf14dd3f7c95b591d929270289268123f31a3d6317f95ccea
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.52/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.52/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.52/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.1-3.1`

Binary Packages:

- `bash=5.1-3.1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-3.1
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-3.1.dsc' bash_5.1-3.1.dsc 2304 SHA256:f4dccc92d9afa8d73eecb727e1b40881c64b9c0f405cca6f323d7c52fe4abe74
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA256:d5eeee4f953c09826409d572e2e8996a2140d67eb8f382ce1f3a9d23883ad696
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-3.1.debian.tar.xz' bash_5.1-3.1.debian.tar.xz 91012 SHA256:e287087297570be5a4abf4697f5c7bedd051148a18b2a0626f6ed5365b3c33e2
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/5.1-3.1/ (for browsing the source)
- https://sources.debian.net/src/bash/5.1-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/5.1-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `binutils=2.37-9`

Binary Packages:

- `binutils=2.37-9`
- `binutils-common:amd64=2.37-9`
- `binutils-x86-64-linux-gnu=2.37-9`
- `libbinutils:amd64=2.37-9`
- `libctf-nobfd0:amd64=2.37-9`
- `libctf0:amd64=2.37-9`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.37-9
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.37-9.dsc' binutils_2.37-9.dsc 11295 SHA256:68cd5f260a96e2b686927c6c14e8dff58cbe21eaf3bba011c776f59a1ff9ca29
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.37.orig.tar.xz' binutils_2.37.orig.tar.xz 24345744 SHA256:220124d1e23f360a3be80b2e2506b379164b0832cc6ff2767360e6a3a747b914
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.37-9.debian.tar.xz' binutils_2.37-9.debian.tar.xz 183584 SHA256:62a7fa43d4bdfe4dd138c4230d335e765fcc1391e3dd08ee7fe2700a1e4556c5
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.37-9/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.37-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.37-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2+b2`
- `libbrotli1:amd64=1.0.9-2+b2`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2
'http://deb.debian.org/debian/pool/main/b/brotli/brotli_1.0.9-2.dsc' brotli_1.0.9-2.dsc 2261 SHA256:8c4c86748ec9770e08b60233d658593650444b04a452dc5b607ed5b5537b683e
'http://deb.debian.org/debian/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA256:f9e8d81d0405ba66d181529af42a3354f838c939095ff99930da6aa9cdf6fe46
'http://deb.debian.org/debian/pool/main/b/brotli/brotli_1.0.9-2.debian.tar.xz' brotli_1.0.9-2.debian.tar.xz 5552 SHA256:ab81b1db852c8d01e0fa5b0b650bb486f32a232b35336828423af50af6fecca0
```

Other potentially useful URLs:

- https://sources.debian.net/src/brotli/1.0.9-2/ (for browsing the source)
- https://sources.debian.net/src/brotli/1.0.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/brotli/1.0.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.8-4`

Binary Packages:

- `bzip2=1.0.8-4`
- `libbz2-1.0:amd64=1.0.8-4`
- `libbz2-dev:amd64=1.0.8-4`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-4
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-4.dsc' bzip2_1.0.8-4.dsc 1603 SHA256:662c5e656a87db884fdc070239f5112cba1e616f20ff260de602876f70415c7b
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-4.debian.tar.bz2' bzip2_1.0.8-4.debian.tar.bz2 26515 SHA256:3f3b26d83120260c7b2e69a5c89649bb818a79955b960fb34a5fae106f008a5d
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.8-4/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.8-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.8-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20211016`

Binary Packages:

- `ca-certificates=20211016`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20211016
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20211016.dsc' ca-certificates_20211016.dsc 1890 SHA256:3d665bb54fa36529dc62fab8cf02a9d54c3a8530b17d9f3f93d170a97727b98c
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20211016.tar.xz' ca-certificates_20211016.tar.xz 239608 SHA256:2ae9b6dc5f40c25d6d7fe55e07b54f12a8967d1955d3b7b2f42ee46266eeef88
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20211016/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20211016/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20211016/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cairo=1.16.0-5`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-5`
- `libcairo-script-interpreter2:amd64=1.16.0-5`
- `libcairo2:amd64=1.16.0-5`
- `libcairo2-dev:amd64=1.16.0-5`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-5
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.16.0-5.dsc' cairo_1.16.0-5.dsc 2939 SHA256:1bcd6dbe5544ad02170d18226ba544b96e2a48bd239407c4ee40c5eb9a441a06
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA256:5e7b29b3f113ef870d1e3ecf8adf21f923396401604bda16d44be45e66052331
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.16.0-5.debian.tar.xz' cairo_1.16.0-5.debian.tar.xz 33144 SHA256:544726514b4b8cfdd151941714c2f910f995ddd4562e6de464c9487e9331fe9f
```

Other potentially useful URLs:

- https://sources.debian.net/src/cairo/1.16.0-5/ (for browsing the source)
- https://sources.debian.net/src/cairo/1.16.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cairo/1.16.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.261`

Binary Packages:

- `libdebconfclient0:amd64=0.261`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.261
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.261.dsc' cdebconf_0.261.dsc 2721 SHA256:a25f06a76b6a3aca915c9131a9915b04630fd1d845cb4a46906f3e44be26c477
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.261.tar.xz' cdebconf_0.261.tar.xz 295304 SHA256:850bb82c279a868bb461ea604964fe71f86970127bcef7e7b6d22a73ec4b2e13
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.261/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.261/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.261/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.32-4.1`

Binary Packages:

- `coreutils=8.32-4.1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.32-4.1
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32-4.1.dsc' coreutils_8.32-4.1.dsc 2104 SHA256:3f518b32292c1be81069ee884acd1aac09f3d949280dc1a7fc1488160eeb495e
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz' coreutils_8.32.orig.tar.xz 5547836 SHA256:4458d8de7849df44ccab15e16b1548b285224dbba5f08fac070c1c0e0bcc4cfa
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz.asc' coreutils_8.32.orig.tar.xz.asc 833 SHA256:71b944375b322ba77c9c56b687b48df885c676d4fd7c465b3706713a9b62ce0a
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32-4.1.debian.tar.xz' coreutils_8.32-4.1.debian.tar.xz 33124 SHA256:79fb30407aa09ed82a37deb11c8f105d7bda6a731a92f6274ceee6ac610aacf6
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/8.32-4.1/ (for browsing the source)
- https://sources.debian.net/src/coreutils/8.32-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/8.32-4.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.79.1-2`

Binary Packages:

- `curl=7.79.1-2`
- `libcurl3-gnutls:amd64=7.79.1-2`
- `libcurl4:amd64=7.79.1-2`
- `libcurl4-openssl-dev:amd64=7.79.1-2`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.79.1-2
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.79.1-2.dsc' curl_7.79.1-2.dsc 2790 SHA256:6545e2688c86d11273fa71f406c38a325bc1607888f16e1f71c7240b20778a9d
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.79.1.orig.tar.gz' curl_7.79.1.orig.tar.gz 4144744 SHA256:370b11201349816287fb0ccc995e420277fbfcaf76206e309b3f60f0eda090c2
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.79.1-2.debian.tar.xz' curl_7.79.1-2.debian.tar.xz 36776 SHA256:e5979630c06c081e82d00c3142f5436d746d09a4a418028d2ffe534ce2800383
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.79.1-2/ (for browsing the source)
- https://sources.debian.net/src/curl/7.79.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.79.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2.3`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2.3`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2.3`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg-2.3/


### `dpkg` source package: `dash=0.5.11+git20210903+057cd650a4ed-3`

Binary Packages:

- `dash=0.5.11+git20210903+057cd650a4ed-3`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `Expat`
- `FSFUL`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.11+git20210903+057cd650a4ed-3
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20210903+057cd650a4ed-3.dsc' dash_0.5.11+git20210903+057cd650a4ed-3.dsc 1686 SHA256:c73521b15349e1271ea4c123eecd0686eb47c98cb8f7f0089fc008194269d612
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz' dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz 133320 SHA256:4fb06697f33f14fcd6b96cd4dfdd5b343c848a4bb69b7c04f1717767e4a117d3
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20210903+057cd650a4ed-3.debian.tar.xz' dash_0.5.11+git20210903+057cd650a4ed-3.debian.tar.xz 42656 SHA256:3f0cd26fce95a29e2e0a1e01268d97fb5429625b7f984e41cc3f05a6704841e1
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.11+git20210903+057cd650a4ed-3/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.11+git20210903+057cd650a4ed-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.11+git20210903+057cd650a4ed-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dav1d=0.9.2-1`

Binary Packages:

- `libdav1d5:amd64=0.9.2-1+b1`

Licenses: (parsed from: `/usr/share/doc/libdav1d5/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dav1d=0.9.2-1
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_0.9.2-1.dsc' dav1d_0.9.2-1.dsc 2332 SHA256:c368585f17b1d1b598b4f5cfedbaefe740fa721033a567b61435caf4adcb6fbb
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_0.9.2.orig.tar.xz' dav1d_0.9.2.orig.tar.xz 713352 SHA256:e3235ab6c43c0135b0db1d131e1923fad4c84db9d85683e30b91b33a52d61c71
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_0.9.2.orig.tar.xz.asc' dav1d_0.9.2.orig.tar.xz.asc 195 SHA256:4eb1d0dfa39bef5634005064d44939be9e5278bf606eb67a06be33a47998b019
'http://deb.debian.org/debian/pool/main/d/dav1d/dav1d_0.9.2-1.debian.tar.xz' dav1d_0.9.2-1.debian.tar.xz 7896 SHA256:e0f958cda906b439c12633aa7c35e718803e3a2103f8f1d82333ef2acaed3b6b
```

Other potentially useful URLs:

- https://sources.debian.net/src/dav1d/0.9.2-1/ (for browsing the source)
- https://sources.debian.net/src/dav1d/0.9.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dav1d/0.9.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db-defaults=5.3.1+nmu1`

Binary Packages:

- `libdb-dev:amd64=5.3.1+nmu1`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=5.3.1+nmu1
'http://deb.debian.org/debian/pool/main/d/db-defaults/db-defaults_5.3.1+nmu1.dsc' db-defaults_5.3.1+nmu1.dsc 1598 SHA256:908f749faf9e8c20638dff514b225c48b163613cad556beb9a54513cb3a249f3
'http://deb.debian.org/debian/pool/main/d/db-defaults/db-defaults_5.3.1+nmu1.tar.xz' db-defaults_5.3.1+nmu1.tar.xz 2864 SHA256:e1e6993f7ae1d055624392a8759b220e21ab7e1c96dba622139c6aaa340c1738
```

Other potentially useful URLs:

- https://sources.debian.net/src/db-defaults/5.3.1+nmu1/ (for browsing the source)
- https://sources.debian.net/src/db-defaults/5.3.1+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db-defaults/5.3.1+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8`
- `libdb5.3-dev=5.3.28+dfsg1-0.8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.8
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8.dsc' db5.3_5.3.28+dfsg1-0.8.dsc 3113 SHA256:5189bebd157e3b51c075804d1affebc87cdbfb782808c621e131660719c24374
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8.debian.tar.xz' db5.3_5.3.28+dfsg1-0.8.debian.tar.xz 30748 SHA256:073c0c87283bf5e606f3ce6d1814315b40b9685c943601ae3fd81e2da4e612d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.8/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.79`

Binary Packages:

- `debconf=1.5.79`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.79
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.79.dsc' debconf_1.5.79.dsc 2082 SHA256:b6a438542c61b8ff8a58cc33dca17859875783945a0e516239369b7d80e3ca7c
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.79.tar.xz' debconf_1.5.79.tar.xz 570588 SHA256:3456338d4bc329b4140c87d91e76068852c3d354348f77aa3cfb98619c069164
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.79/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.79/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.79/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debian-archive-keyring=2021.1.1`

Binary Packages:

- `debian-archive-keyring=2021.1.1`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2021.1.1
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2021.1.1.dsc' debian-archive-keyring_2021.1.1.dsc 1854 SHA256:a17a062b6dabe2d1092ee362412b8f2c9d4a44c7bd18ef2bbb45340c2ee4c512
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2021.1.1.tar.xz' debian-archive-keyring_2021.1.1.tar.xz 151340 SHA256:5fe6011f7caf516b19b8f2c545bd215f4b6f8022b161d1ce5262ac2c51c4dbcf
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2021.1.1/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2021.1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2021.1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=5.5-1`

Binary Packages:

- `debianutils=5.5-1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.5-1
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.5-1.dsc' debianutils_5.5-1.dsc 1879 SHA256:db5048cb0425d07dc61ac336c950d587a7b7cdf94a734a3c58f39909b1916986
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.5.orig.tar.xz' debianutils_5.5.orig.tar.xz 104448 SHA256:2b0fad5c00eb2b8461523b2950e6f06e6ddbb0ac3384c5a3377867d51098d102
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.5-1.debian.tar.xz' debianutils_5.5-1.debian.tar.xz 21672 SHA256:0be92076584828f98008492bd1f0eda7983c343eda47d7f53c660a3a54bdbe46
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/5.5-1/ (for browsing the source)
- https://sources.debian.net/src/debianutils/5.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/5.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.7-5`

Binary Packages:

- `diffutils=1:3.7-5`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.7-5
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.7-5.dsc' diffutils_3.7-5.dsc 1714 SHA256:5476ed004e300f291b5f0a356074a8ba8944a8b34514bb0fe95d274455adbf5d
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz' diffutils_3.7.orig.tar.xz 1448828 SHA256:b3a7a6221c3dc916085f0d205abf6b8e1ba443d4dd965118da364a1dc1cb3a26
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz.asc' diffutils_3.7.orig.tar.xz.asc 833 SHA256:c89b9d60a1d67cf8b2dd108a8b918e4cce34cba6c9e1f67e2ca482c52c0258a7
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.7-5.debian.tar.xz' diffutils_3.7-5.debian.tar.xz 89004 SHA256:c90fd39d677702226b89d7559c124d7eb0b88195c381853ca1e5c8ca08e90a3a
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.7-5/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.7-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.7-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `djvulibre=3.5.28-2`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.28-2`
- `libdjvulibre-text=3.5.28-2`
- `libdjvulibre21:amd64=3.5.28-2`

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

### `dpkg` source package: `dpkg=1.20.9`

Binary Packages:

- `dpkg=1.20.9`
- `dpkg-dev=1.20.9`
- `libdpkg-perl=1.20.9`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.20.9
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.20.9.dsc' dpkg_1.20.9.dsc 2120 SHA256:87f21320f3165d1c57dae2314b7fd1849b49da9416fee3fb57c4b1e4192b4285
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.20.9.tar.xz' dpkg_1.20.9.tar.xz 4954428 SHA256:5ce242830f213b5620f08e6c4183adb1ef4dc9da28d31988a27c87c71fe534ce
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.20.9/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.20.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.20.9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.46.4-1`

Binary Packages:

- `comerr-dev:amd64=2.1-1.46.4-1`
- `e2fsprogs=1.46.4-1`
- `libcom-err2:amd64=1.46.4-1`
- `libext2fs2:amd64=1.46.4-1`
- `libss2:amd64=1.46.4-1`
- `logsave=1.46.4-1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.4-1
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.4-1.dsc' e2fsprogs_1.46.4-1.dsc 2846 SHA256:d3ec9a1c778d5c1f71b76a6736eb0d396ff76543ceb9fc9c05fb706d5c4cbf65
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.4.orig.tar.gz' e2fsprogs_1.46.4.orig.tar.gz 9521023 SHA256:7524520b291e901431ce59ea085955b601126de371bf3cfc0f5e4fad78684265
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.4.orig.tar.gz.asc' e2fsprogs_1.46.4.orig.tar.gz.asc 488 SHA256:e544606bc7fe48134a16d95d79e19fb1ea5d284d3ef47a05ccc1051ccb01ae67
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.4-1.debian.tar.xz' e2fsprogs_1.46.4-1.debian.tar.xz 83128 SHA256:ce747152024765e5a6b33ef5fc63bd7ceba107152811e822c4d3fea54b4ecae9
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.46.4-1/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.46.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.46.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `elfutils=0.185-2`

Binary Packages:

- `libelf1:amd64=0.185-2`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/elfutils/0.185-2/


### `dpkg` source package: `expat=2.4.1-3`

Binary Packages:

- `libexpat1:amd64=2.4.1-3`
- `libexpat1-dev:amd64=2.4.1-3`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.4.1-3
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.4.1-3.dsc' expat_2.4.1-3.dsc 1981 SHA256:b3a1c62a87c55eaf53b49c90076aa0f7a5ab7d163ed04384990a579aba46dd17
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.4.1.orig.tar.gz' expat_2.4.1.orig.tar.gz 8307804 SHA256:660e5852b26125f4508183dfa134e18eb33a892dbd8e06786ea38d92dbbb5b07
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.4.1-3.debian.tar.xz' expat_2.4.1-3.debian.tar.xz 11940 SHA256:94a50cba92c8f01f52f3c68a20c4f1163bc528b88df1abb01fa7931bfc84f334
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.4.1-3/ (for browsing the source)
- https://sources.debian.net/src/expat/2.4.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.4.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fftw3=3.3.8-2`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.8-2.dsc' fftw3_3.3.8-2.dsc 2978 SHA256:b4367efbcc2bbbc44b62a9416a1c37764f5214628632553070c35893df786f68
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA256:6113262f6e92c5bd474f2875fa1b01054c4ad5040f6b0da7c03c98821d9ae303
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.8-2.debian.tar.xz' fftw3_3.3.8-2.debian.tar.xz 13696 SHA256:684dede6b4124f309033d128dc7bdf1eb394984e6e8dd79e1fd5d73b95b12461
```

Other potentially useful URLs:

- https://sources.debian.net/src/fftw3/3.3.8-2/ (for browsing the source)
- https://sources.debian.net/src/fftw3/3.3.8-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fftw3/3.3.8-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `file=1:5.39-3`

Binary Packages:

- `file=1:5.39-3`
- `libmagic-mgc=1:5.39-3`
- `libmagic1:amd64=1:5.39-3`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.39-3
'http://deb.debian.org/debian/pool/main/f/file/file_5.39-3.dsc' file_5.39-3.dsc 2237 SHA256:19952c131cffa14cf4b64f3fa2d35c975388985e5b5ee154e2e0cef5ccde697e
'http://deb.debian.org/debian/pool/main/f/file/file_5.39.orig.tar.gz' file_5.39.orig.tar.gz 954266 SHA256:f05d286a76d9556243d0cb05814929c2ecf3a5ba07963f8f70bfaaa70517fad1
'http://deb.debian.org/debian/pool/main/f/file/file_5.39.orig.tar.gz.asc' file_5.39.orig.tar.gz.asc 169 SHA256:409232b54cabe3082f38f1e7ec4c69e7d937f26d039da691f7349d142b48df83
'http://deb.debian.org/debian/pool/main/f/file/file_5.39-3.debian.tar.xz' file_5.39-3.debian.tar.xz 34420 SHA256:92657787e04b444d7ec3b6cac0519d1655cb6fc2ae08de76bc3f4f90acf0c545
```

Other potentially useful URLs:

- https://sources.debian.net/src/file/1:5.39-3/ (for browsing the source)
- https://sources.debian.net/src/file/1:5.39-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/file/1:5.39-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.8.0-1`

Binary Packages:

- `findutils=4.8.0-1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.8.0-1
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.8.0-1.dsc' findutils_4.8.0-1.dsc 2302 SHA256:47f342ec5146f4138f5004dbefe5838656057b502dfe225884b9f56840e29a3b
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz' findutils_4.8.0.orig.tar.xz 1983096 SHA256:57127b7e97d91282c6ace556378d5455a9509898297e46e10443016ea1387164
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz.asc' findutils_4.8.0.orig.tar.xz.asc 488 SHA256:dc0d5251026532d2b115e447eea70a934d3df6a0efcaf225c9d585eeedeefe62
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.8.0-1.debian.tar.xz' findutils_4.8.0-1.debian.tar.xz 27296 SHA256:c99753f13f9e79653f79a398d1aafb15294c8f7953ad86948c7bf4cb0032bb43
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.8.0-1/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.8.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.8.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fontconfig=2.13.1-4.2`

Binary Packages:

- `fontconfig=2.13.1-4.2`
- `fontconfig-config=2.13.1-4.2`
- `libfontconfig-dev:amd64=2.13.1-4.2`
- `libfontconfig1:amd64=2.13.1-4.2`
- `libfontconfig1-dev:amd64=2.13.1-4.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-4.2
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.13.1-4.2.dsc' fontconfig_2.13.1-4.2.dsc 2716 SHA256:d22e6441f0aa03b569d886fbb3227330dd2305e7aa10513e177ced28b8b52d63
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA256:f655dd2a986d7aa97e052261b36aa67b0a64989496361eca8d604e6414006741
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.13.1-4.2.debian.tar.xz' fontconfig_2.13.1-4.2.debian.tar.xz 55124 SHA256:f1ec69a2a0affd86189d3b75ced77b30bbcbc3a6fc0508490e570d4786464b58
```

Other potentially useful URLs:

- https://sources.debian.net/src/fontconfig/2.13.1-4.2/ (for browsing the source)
- https://sources.debian.net/src/fontconfig/2.13.1-4.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fontconfig/2.13.1-4.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fonts-dejavu=2.37-2`

Binary Packages:

- `fonts-dejavu-core=2.37-2`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-2
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.dsc' fonts-dejavu_2.37-2.dsc 2387 SHA256:13948768dbf1a9aa3ae9fe592a4c6c904b1dd075acb689a49b85e0ae73b1756c
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.debian.tar.xz' fonts-dejavu_2.37-2.debian.tar.xz 11408 SHA256:428cf37685df891574d2dcb32aa9366e4e95985fda7d87069903313bb03470ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/fonts-dejavu/2.37-2/ (for browsing the source)
- https://sources.debian.net/src/fonts-dejavu/2.37-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fonts-dejavu/2.37-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `freetype=2.11.0+dfsg-1`

Binary Packages:

- `libfreetype-dev:amd64=2.11.0+dfsg-1`
- `libfreetype6:amd64=2.11.0+dfsg-1`
- `libfreetype6-dev:amd64=2.11.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

- `BSD-3-Clause`
- `BSL-1.0`
- `FSFAP`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `OpenGroup-BSD-like`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.11.0+dfsg-1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.0+dfsg-1.dsc' freetype_2.11.0+dfsg-1.dsc 3730 SHA256:46187f314e2e561d3552d5a2cece1155546b0ada1f295ff2f1359ea5d3724a19
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.0+dfsg.orig-ft2demos.tar.xz' freetype_2.11.0+dfsg.orig-ft2demos.tar.xz 257316 SHA256:eb0622296c6dfb38fc305c99ebbfb5c770db7e344b94f63042ec03f3db164550
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.0+dfsg.orig-ft2demos.tar.xz.asc' freetype_2.11.0+dfsg.orig-ft2demos.tar.xz.asc 195 SHA256:7a365d04c6dc35f1e272eb6637c46355e9576b84c0014edc014375d89dac6659
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.0+dfsg.orig-ft2docs.tar.xz' freetype_2.11.0+dfsg.orig-ft2docs.tar.xz 2070604 SHA256:5b0b5f504f3547ab6123049917b36cfe6944837eaa7baa86ae742a596b5c206c
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.0+dfsg.orig-ft2docs.tar.xz.asc' freetype_2.11.0+dfsg.orig-ft2docs.tar.xz.asc 195 SHA256:6998b16c75c4968a36c17824db473d76c809f1db9996ccc9ff72f8c42921c428
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.0+dfsg.orig.tar.xz' freetype_2.11.0+dfsg.orig.tar.xz 1974064 SHA256:4f61192f625a73151bfca252f7030e5739b00d49037ef407bc107236abe5ece7
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.0+dfsg-1.debian.tar.xz' freetype_2.11.0+dfsg-1.debian.tar.xz 114440 SHA256:8447a212decb2365ab2ad6a6b0818ba9c42aa4bd7f4d6e52cb4d924953b41867
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.11.0+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.11.0+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.11.0+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fribidi=1.0.8-2`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.8-2.dsc' fribidi_1.0.8-2.dsc 1987 SHA256:f1b396620cda57e93799725abad47089902429295f7b3555bc3d5b3f00a79340
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA256:94c7b68d86ad2a9613b4dcffe7bbeb03523d63b5b37918bdf2e4ef34195c1e6c
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.8-2.debian.tar.xz' fribidi_1.0.8-2.debian.tar.xz 8980 SHA256:898fc0b48625ce31e29d2f9501f17b9991b16b03816db6467faaedb85d22f00b
```

Other potentially useful URLs:

- https://sources.debian.net/src/fribidi/1.0.8-2/ (for browsing the source)
- https://sources.debian.net/src/fribidi/1.0.8-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fribidi/1.0.8-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-10=10.3.0-12`

Binary Packages:

- `gcc-10-base:amd64=10.3.0-12`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.3.0-12
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0-12.dsc' gcc-10_10.3.0-12.dsc 21839 SHA256:07395f48f47fc06b9df76b080fd8826d06d37bf7b66939f7358e70083dacd877
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0.orig.tar.gz' gcc-10_10.3.0.orig.tar.gz 79796443 SHA256:9ace579357cc2e976e4d2576fc1d519b6856495d98ccf11d1a67c5a9b4f79b8c
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0-12.debian.tar.xz' gcc-10_10.3.0-12.debian.tar.xz 813316 SHA256:f3c84f363a92e5d98460aafad7d2fd62a563d53ee1ba9f26c6ca9e0e7665daac
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-10/10.3.0-12/ (for browsing the source)
- https://sources.debian.net/src/gcc-10/10.3.0-12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-10/10.3.0-12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-11=11.2.0-10`

Binary Packages:

- `cpp-11=11.2.0-10`
- `g++-11=11.2.0-10`
- `gcc-11=11.2.0-10`
- `gcc-11-base:amd64=11.2.0-10`
- `libasan6:amd64=11.2.0-10`
- `libatomic1:amd64=11.2.0-10`
- `libcc1-0:amd64=11.2.0-10`
- `libgcc-11-dev:amd64=11.2.0-10`
- `libgcc-s1:amd64=11.2.0-10`
- `libgomp1:amd64=11.2.0-10`
- `libitm1:amd64=11.2.0-10`
- `liblsan0:amd64=11.2.0-10`
- `libquadmath0:amd64=11.2.0-10`
- `libstdc++-11-dev:amd64=11.2.0-10`
- `libstdc++6:amd64=11.2.0-10`
- `libtsan0:amd64=11.2.0-10`
- `libubsan1:amd64=11.2.0-10`

Licenses: (parsed from: `/usr/share/doc/cpp-11/copyright`, `/usr/share/doc/g++-11/copyright`, `/usr/share/doc/gcc-11/copyright`, `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-11-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-11-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.2.0-10
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0-10.dsc' gcc-11_11.2.0-10.dsc 27453 SHA256:957e5ea9fcacc0f93b35f390790e2d0488f89ccdca20eb955b9724e4cf4e644a
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0.orig.tar.gz' gcc-11_11.2.0.orig.tar.gz 83874319 SHA256:61bbc68194e52a9149a91571b5e1eb4db520017ed4bcdc021c175a1845605e47
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0-10.debian.tar.xz' gcc-11_11.2.0-10.debian.tar.xz 1897060 SHA256:0a240e65ce23f7a7a1f0b00a63a2ecfc3496244dd877364de3acbd956f063a0a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-11/11.2.0-10/ (for browsing the source)
- https://sources.debian.net/src/gcc-11/11.2.0-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-11/11.2.0-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-9=9.4.0-3`

Binary Packages:

- `gcc-9-base:amd64=9.4.0-3`

Licenses: (parsed from: `/usr/share/doc/gcc-9-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gcc-9=9.4.0-3
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.4.0-3.dsc' gcc-9_9.4.0-3.dsc 21922 SHA256:984c2fecdbc021a2e702218f871d2fcf6dfbd2d5ba31343b7f991d18a044f10f
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.4.0.orig.tar.gz' gcc-9_9.4.0.orig.tar.gz 88736226 SHA256:7ef28e618cecddbb538359d03998a61648edb10b570b995aa4f4016c4a0d823e
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.4.0-3.debian.tar.xz' gcc-9_9.4.0-3.debian.tar.xz 615476 SHA256:18d633bc3c5be551176ddb513d5481b735f72435ba405a1dd05f6ace0ae2d56a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-9/9.4.0-3/ (for browsing the source)
- https://sources.debian.net/src/gcc-9/9.4.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-9/9.4.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-defaults=1.194`

Binary Packages:

- `cpp=4:11.2.0-2`
- `g++=4:11.2.0-2`
- `gcc=4:11.2.0-2`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.194
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.194.dsc' gcc-defaults_1.194.dsc 12639 SHA256:e98726befd3c6b7f32fd863dd0cfd87e19163f208e2983e13df30f4f62f8d415
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.194.tar.xz' gcc-defaults_1.194.tar.xz 45200 SHA256:ef25edf2ad31a51abdcc0bc5237233daedc8cc6ed2a7194e49d83150dde2a445
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-defaults/1.194/ (for browsing the source)
- https://sources.debian.net/src/gcc-defaults/1.194/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-defaults/1.194/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.22-1`

Binary Packages:

- `libgdbm-compat4:amd64=1.22-1`
- `libgdbm-dev:amd64=1.22-1`
- `libgdbm6:amd64=1.22-1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.22-1
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.22-1.dsc' gdbm_1.22-1.dsc 2583 SHA256:d3e8996eea0571e5caefeb7665a705097734278d81f366826cf4a025131f282f
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.22.orig.tar.gz' gdbm_1.22.orig.tar.gz 1090100 SHA256:f366c823a6724af313b6bbe975b2809f9a157e5f6a43612a72949138d161d762
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.22.orig.tar.gz.asc' gdbm_1.22.orig.tar.gz.asc 181 SHA256:0e66b54bc503377c0e13e001c6807f6c908c1cfb51a892446e69ee9400229c3a
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.22-1.debian.tar.xz' gdbm_1.22-1.debian.tar.xz 18484 SHA256:8fa2953bf9801b65293b3a759e065c0a04ba798b0ad3aab2553a1621cab51588
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.22-1/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.22-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.22-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdk-pixbuf=2.42.6+dfsg-2`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.42.6+dfsg-2`
- `libgdk-pixbuf-2.0-0:amd64=2.42.6+dfsg-2`
- `libgdk-pixbuf-2.0-dev:amd64=2.42.6+dfsg-2`
- `libgdk-pixbuf2.0-bin=2.42.6+dfsg-2`
- `libgdk-pixbuf2.0-common=2.42.6+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-dev/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `Apache-2.0`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `CC0-1.0,`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3.0`
- `GPL-3.0+`
- `GPL-3.0+,`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.42.6+dfsg-2
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6+dfsg-2.dsc' gdk-pixbuf_2.42.6+dfsg-2.dsc 3406 SHA256:ecdc7c011dbf6497cbed36ed634d87f79e30e133013ecf7db5c7b84ed5e481b5
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6+dfsg.orig.tar.xz' gdk-pixbuf_2.42.6+dfsg.orig.tar.xz 6527432 SHA256:9f73b7d60d88f0bf6108731d7751934e6a6dc2eb44c6714aefe740b82221ffbb
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6+dfsg-2.debian.tar.xz' gdk-pixbuf_2.42.6+dfsg-2.debian.tar.xz 29756 SHA256:9344e3c9dc787f83a3b53ec4392c96f0295a60115a7dfc18f8116136fd62029e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdk-pixbuf/2.42.6+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/gdk-pixbuf/2.42.6+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdk-pixbuf/2.42.6+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.33.1-1`

Binary Packages:

- `git=1:2.33.1-1`
- `git-man=1:2.33.1-1`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
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
$ apt-get source -qq --print-uris git=1:2.33.1-1
'http://deb.debian.org/debian/pool/main/g/git/git_2.33.1-1.dsc' git_2.33.1-1.dsc 2825 SHA256:dc156f4b49bfd7307fdd787d9329152ef1f09a31584e46c5341e33815d363500
'http://deb.debian.org/debian/pool/main/g/git/git_2.33.1.orig.tar.xz' git_2.33.1.orig.tar.xz 6558636 SHA256:e054a6e6c2b088bd1bff5f61ed9ba5aa91c9a3cd509539a4b41c5ddf02201f2f
'http://deb.debian.org/debian/pool/main/g/git/git_2.33.1-1.debian.tar.xz' git_2.33.1-1.debian.tar.xz 692124 SHA256:6e7e38e04804c89698dab5436691d75cc1095ae6d641b025c202485b67f96eb2
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.33.1-1/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.33.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.33.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.70.1-1`

Binary Packages:

- `libglib2.0-0:amd64=2.70.1-1`
- `libglib2.0-bin=2.70.1-1`
- `libglib2.0-data=2.70.1-1`
- `libglib2.0-dev:amd64=2.70.1-1`
- `libglib2.0-dev-bin=2.70.1-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.70.1-1
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.70.1-1.dsc' glib2.0_2.70.1-1.dsc 3486 SHA256:0ad12055052e20888e1d13636205f30c901857744a620a6b17b92e6f33344303
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.70.1.orig.tar.xz' glib2.0_2.70.1.orig.tar.xz 4797752 SHA256:f9b7bce7f51753a1f43853bbcaca8bf09e15e994268e29cfd7a76f65636263c0
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.70.1-1.debian.tar.xz' glib2.0_2.70.1-1.debian.tar.xz 102452 SHA256:f642e2b61c8f8268e659ae1b0fba4494594c076dbda537b796fe4155c2bbf480
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.70.1-1/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.70.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.70.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.32-4`

Binary Packages:

- `libc-bin=2.32-4`
- `libc-dev-bin=2.32-4`
- `libc6:amd64=2.32-4`
- `libc6-dev:amd64=2.32-4`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.32-4
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.32-4.dsc' glibc_2.32-4.dsc 9617 SHA256:bb861648fe09205bc9ad561f203f633163939ca431189893a68d0241bdb36e90
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.32.orig.tar.xz' glibc_2.32.orig.tar.xz 17339504 SHA256:98367884c13188ae59a90b59a1628bb109f67fa14fceba42f0cbeb08412bb69c
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.32-4.debian.tar.xz' glibc_2.32-4.debian.tar.xz 842152 SHA256:2abfe70d32eb9ad2dad60a110da69c42f9d62e9653548a849dee3aef7a32a006
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.32-4/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.32-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.32-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.1+dfsg-3`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.1+dfsg-3`
- `libgmp10:amd64=2:6.2.1+dfsg-3`
- `libgmpxx4ldbl:amd64=2:6.2.1+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg-3
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg-3.dsc' gmp_6.2.1+dfsg-3.dsc 2223 SHA256:b91dae1d6298e5ff75dee503c7f8128e822000e343e0a5b5d5146cc1713334bb
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA256:c6ba08e3f079260ab90ff44ab8801eae134cd62cd78f4aa56317c0e70daa40cb
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg-3.debian.tar.xz' gmp_6.2.1+dfsg-3.debian.tar.xz 18356 SHA256:32d75d4e7a383a5cea701aff4a4bf609933c4d15d1f5e3b6168eed51857bc8f0
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.27-2`

Binary Packages:

- `dirmngr=2.2.27-2`
- `gnupg=2.2.27-2`
- `gnupg-l10n=2.2.27-2`
- `gnupg-utils=2.2.27-2`
- `gpg=2.2.27-2`
- `gpg-agent=2.2.27-2`
- `gpg-wks-client=2.2.27-2`
- `gpg-wks-server=2.2.27-2`
- `gpgconf=2.2.27-2`
- `gpgsm=2.2.27-2`
- `gpgv=2.2.27-2`

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
$ apt-get source -qq --print-uris gnupg2=2.2.27-2
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-2.dsc' gnupg2_2.2.27-2.dsc 3644 SHA256:f8a99fd0976958c5656925ea576b26667ac075d0cb145981a9043f0c89a06911
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2' gnupg2_2.2.27.orig.tar.bz2 7191555 SHA256:34e60009014ea16402069136e0a5f63d9b65f90096244975db5cea74b3d02399
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-2.debian.tar.xz' gnupg2_2.2.27-2.debian.tar.xz 62720 SHA256:6c67a7acbcab01116a640894751cdf54438caa265fae656d580d42010582591c
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.27-2/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.27-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.27-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.2-2`

Binary Packages:

- `libgnutls30:amd64=3.7.2-2`

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
$ apt-get source -qq --print-uris gnutls28=3.7.2-2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2-2.dsc' gnutls28_3.7.2-2.dsc 3487 SHA256:f2c1cfd399a5631133f37590d470929ba0344c94ae30ae89c4673711613409d7
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2.orig.tar.xz' gnutls28_3.7.2.orig.tar.xz 6091508 SHA256:646e6c5a9a185faa4cea796d378a1ba8e1148dbb197ca6605f95986a25af2752
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2.orig.tar.xz.asc' gnutls28_3.7.2.orig.tar.xz.asc 833 SHA256:015e4f3390469126a94014e4aa1182ed4b238f940ff09093884cc04f8fefedf0
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2-2.debian.tar.xz' gnutls28_3.7.2-2.debian.tar.xz 65144 SHA256:900fdef4138494346a4e513a62a7583c8be97c0bbebe475d37ff6b093b19944a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.2-2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gobject-introspection=1.70.0-2`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.70.0-2`
- `gir1.2-glib-2.0:amd64=1.70.0-2`
- `libgirepository-1.0-1:amd64=1.70.0-2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.70.0-2
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.70.0-2.dsc' gobject-introspection_1.70.0-2.dsc 3120 SHA256:7b5e11a5a34c64074b422d197e32e6dd64829ba6e14d624e6a2b87ae15b42e33
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.70.0.orig.tar.xz' gobject-introspection_1.70.0.orig.tar.xz 1029372 SHA256:902b4906e3102d17aa2fcb6dad1c19971c70f2a82a159ddc4a94df73a3cafc4a
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.70.0-2.debian.tar.xz' gobject-introspection_1.70.0-2.debian.tar.xz 25576 SHA256:176240fefffe8968d569a4d25d9b91062b2d6cfc9c2f788647d01d56c2f8a2dc
```

Other potentially useful URLs:

- https://sources.debian.net/src/gobject-introspection/1.70.0-2/ (for browsing the source)
- https://sources.debian.net/src/gobject-introspection/1.70.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gobject-introspection/1.70.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `grep=3.7-1`

Binary Packages:

- `grep=3.7-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.7-1
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.7-1.dsc' grep_3.7-1.dsc 1644 SHA256:f1fbf4f6d2362e6057bae9e09d6672d221f9efec41dade6ec3c294c6dd8e99e9
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.7.orig.tar.xz' grep_3.7.orig.tar.xz 1641196 SHA256:5c10da312460aec721984d5d83246d24520ec438dd48d7ab5a05dbc0d6d6823c
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.7.orig.tar.xz.asc' grep_3.7.orig.tar.xz.asc 833 SHA256:d79a0137eb803938ff47dc366825d05d1a042457f74acc264a361a84428a5de7
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.7-1.debian.tar.xz' grep_3.7-1.debian.tar.xz 18104 SHA256:064cfebccc2f5a66978f72ea0b601fa9e5d59588b6e9ff86bf2b4ea7f303ca3f
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.7-1/ (for browsing the source)
- https://sources.debian.net/src/grep/3.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.10-4`

Binary Packages:

- `gzip=1.10-4`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-4
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.10-4.dsc' gzip_1.10-4.dsc 1780 SHA256:c2728d6a042bf41e43f8bf86f520682a312235f981cca26a60fc0745ff536459
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA256:c91f74430bf7bc20402e1f657d0b252cb80aa66ba333a25704512af346633c68
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.10-4.debian.tar.xz' gzip_1.10-4.debian.tar.xz 19300 SHA256:f3e40d75fe3f695c76f028194b2031a2016a302b3c95d28ebc52b8538331a708
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.10-4/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.10-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.10-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `harfbuzz=2.7.4-1`

Binary Packages:

- `libharfbuzz0b:amd64=2.7.4-1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.7.4-1
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.7.4-1.dsc' harfbuzz_2.7.4-1.dsc 2740 SHA256:d8b7efb43ad01cf6b7377f5c14bc0d0541489315026ed87f5f652f1a1aff59c7
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.7.4.orig.tar.xz' harfbuzz_2.7.4.orig.tar.xz 9532468 SHA256:6ad11d653347bd25d8317589df4e431a2de372c0cf9be3543368e07ec23bb8e7
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.7.4-1.debian.tar.xz' harfbuzz_2.7.4-1.debian.tar.xz 10508 SHA256:a756f72db035c105209470836df62aa607d2aceacadfee5b17020c634eb4bef0
```

Other potentially useful URLs:

- https://sources.debian.net/src/harfbuzz/2.7.4-1/ (for browsing the source)
- https://sources.debian.net/src/harfbuzz/2.7.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/harfbuzz/2.7.4-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `hostname=3.23`

Binary Packages:

- `hostname=3.23`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.23.dsc' hostname_3.23.dsc 1402 SHA256:0694c083fad82da1fd33204557a30bfc745a689a64030ba360062daafe03ede0
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.23.tar.gz' hostname_3.23.tar.gz 13672 SHA256:bc6d1954b22849869ff8b2a602e39f08b1702f686d4b58dd7927cdeb5b4876ef
```

Other potentially useful URLs:

- https://sources.debian.net/src/hostname/3.23/ (for browsing the source)
- https://sources.debian.net/src/hostname/3.23/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hostname/3.23/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `icu=67.1-7`

Binary Packages:

- `icu-devtools=67.1-7`
- `libicu-dev:amd64=67.1-7`
- `libicu67:amd64=67.1-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=67.1-7
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1-7.dsc' icu_67.1-7.dsc 2236 SHA256:3213915e2b2b07ab1d5fe81ba4e310d8146c0a799fd65ac1f1dbb0c32f56cff1
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1.orig.tar.gz' icu_67.1.orig.tar.gz 24518055 SHA256:94a80cd6f251a53bd2a997f6f1b5ac6653fe791dfab66e1eb0227740fb86d5dc
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1.orig.tar.gz.asc' icu_67.1.orig.tar.gz.asc 833 SHA256:0044119f3df92ff3055dc3609f527fa1290177f6ef1b6650ea136698b245e537
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1-7.debian.tar.xz' icu_67.1-7.debian.tar.xz 30256 SHA256:9836cbc00bf8da459734c82ccd435d09674e85e268f272decf16dbfa0bda730e
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/67.1-7/ (for browsing the source)
- https://sources.debian.net/src/icu/67.1-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/67.1-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ilmbase=2.5.7-2`

Binary Packages:

- `libilmbase-dev:amd64=2.5.7-2`
- `libilmbase25:amd64=2.5.7-2`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase25/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.5.7-2
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.5.7-2.dsc' ilmbase_2.5.7-2.dsc 2483 SHA256:9318d71240c12652d6d38f76e9541cc10bb6be430e8338210a1cbf12958ffc48
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.5.7.orig.tar.gz' ilmbase_2.5.7.orig.tar.gz 27539574 SHA256:36ecb2290cba6fc92b2ec9357f8dc0e364b4f9a90d727bf9a57c84760695272d
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.5.7.orig.tar.gz.asc' ilmbase_2.5.7.orig.tar.gz.asc 27539574 SHA256:36ecb2290cba6fc92b2ec9357f8dc0e364b4f9a90d727bf9a57c84760695272d
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.5.7-2.debian.tar.xz' ilmbase_2.5.7-2.debian.tar.xz 14484 SHA256:4f33b949ab07ae118d7ba5da0f03cdaa880e1073369dea5538d0a16316ed2d6c
```

Other potentially useful URLs:

- https://sources.debian.net/src/ilmbase/2.5.7-2/ (for browsing the source)
- https://sources.debian.net/src/ilmbase/2.5.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ilmbase/2.5.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `imagemagick=8:6.9.11.60+dfsg-1.3`

Binary Packages:

- `imagemagick=8:6.9.11.60+dfsg-1.3`
- `imagemagick-6-common=8:6.9.11.60+dfsg-1.3`
- `imagemagick-6.q16=8:6.9.11.60+dfsg-1.3`
- `libmagickcore-6-arch-config:amd64=8:6.9.11.60+dfsg-1.3`
- `libmagickcore-6-headers=8:6.9.11.60+dfsg-1.3`
- `libmagickcore-6.q16-6:amd64=8:6.9.11.60+dfsg-1.3`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.11.60+dfsg-1.3`
- `libmagickcore-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.3`
- `libmagickcore-dev=8:6.9.11.60+dfsg-1.3`
- `libmagickwand-6-headers=8:6.9.11.60+dfsg-1.3`
- `libmagickwand-6.q16-6:amd64=8:6.9.11.60+dfsg-1.3`
- `libmagickwand-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.3`
- `libmagickwand-dev=8:6.9.11.60+dfsg-1.3`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/libmagickcore-6-arch-config/copyright`, `/usr/share/doc/libmagickcore-6-headers/copyright`, `/usr/share/doc/libmagickcore-6.q16-6/copyright`, `/usr/share/doc/libmagickcore-6.q16-6-extra/copyright`, `/usr/share/doc/libmagickcore-6.q16-dev/copyright`, `/usr/share/doc/libmagickcore-dev/copyright`, `/usr/share/doc/libmagickwand-6-headers/copyright`, `/usr/share/doc/libmagickwand-6.q16-6/copyright`, `/usr/share/doc/libmagickwand-6.q16-dev/copyright`, `/usr/share/doc/libmagickwand-dev/copyright`)

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
- `TatcherUlrichPublicDomain`
- `aclocal`

Source:

```console
$ apt-get source -qq --print-uris imagemagick=8:6.9.11.60+dfsg-1.3
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.11.60+dfsg-1.3.dsc' imagemagick_6.9.11.60+dfsg-1.3.dsc 5229 SHA256:5e09025a6861ace28ac9dc51db730172801e875842ba1faec5c9b736b2918269
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.11.60+dfsg.orig.tar.xz' imagemagick_6.9.11.60+dfsg.orig.tar.xz 9395144 SHA256:472fb516df842ee9c819ed80099c188463b9e961303511c36ae24d0eaa8959c4
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.11.60+dfsg-1.3.debian.tar.xz' imagemagick_6.9.11.60+dfsg-1.3.debian.tar.xz 246928 SHA256:a85cb23dc8633a89349517378b4b973235a59fc4969b908be660c7bde0f2b36c
```

Other potentially useful URLs:

- https://sources.debian.net/src/imagemagick/8:6.9.11.60+dfsg-1.3/ (for browsing the source)
- https://sources.debian.net/src/imagemagick/8:6.9.11.60+dfsg-1.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/imagemagick/8:6.9.11.60+dfsg-1.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `init-system-helpers=1.60`

Binary Packages:

- `init-system-helpers=1.60`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.60
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.60.dsc' init-system-helpers_1.60.dsc 1902 SHA256:51dd15cc34daf5e58e40560563785d422fb27ac8a2f6ce4e73350a800cbf3265
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.60.tar.xz' init-system-helpers_1.60.tar.xz 40584 SHA256:2cf987e5ec2412faab8e99d6f26598b6ae65afe1af2073133575224997082172
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.60/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.60/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.60/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `isl=0.24-2`

Binary Packages:

- `libisl23:amd64=0.24-2`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.24-2
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.24-2.dsc' isl_0.24-2.dsc 1832 SHA256:dfb7409828a6f733e80ed0240311f9ab64f2496cfb5c7d3c878fadc35e578ae3
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.24.orig.tar.xz' isl_0.24.orig.tar.xz 1930956 SHA256:043105cc544f416b48736fff8caf077fb0663a717d06b1113f16e391ac99ebad
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.24-2.debian.tar.xz' isl_0.24-2.debian.tar.xz 26476 SHA256:dc20a4d6dbddf6e40665626b3b2523fc464090cb4f8bda6844c64d1584aa2af4
```

Other potentially useful URLs:

- https://sources.debian.net/src/isl/0.24-2/ (for browsing the source)
- https://sources.debian.net/src/isl/0.24-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/isl/0.24-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jbigkit=2.1-3.1`

Binary Packages:

- `libjbig-dev:amd64=2.1-3.1+b2`
- `libjbig0:amd64=2.1-3.1+b2`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1-3.1.dsc' jbigkit_2.1-3.1.dsc 1299 SHA256:62c8812d508958c5d35f2b1579dc3052fb5bd8d2e77d023fad064c4b48c8c3f8
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://deb.debian.org/debian/pool/main/j/jbigkit/jbigkit_2.1-3.1.debian.tar.xz' jbigkit_2.1-3.1.debian.tar.xz 7600 SHA256:ebc3c52deaf37d52baea54d648a713640dc262926abda7bf05cd08e7db5dd1ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/jbigkit/2.1-3.1/ (for browsing the source)
- https://sources.debian.net/src/jbigkit/2.1-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jbigkit/2.1-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.6.1-2`

Binary Packages:

- `libkeyutils1:amd64=1.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.1-2
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.1-2.dsc' keyutils_1.6.1-2.dsc 2076 SHA256:6dd531f522fb3c5d8cfaaaf726e9277b64f50bff8c05d06269f42a677f65a4a8
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.1.orig.tar.bz2' keyutils_1.6.1.orig.tar.bz2 97232 SHA256:c8b15722ae51d95b9ad76cc6d49a4c2cc19b0c60f72f61fb9bf43eea7cbd64ce
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.1-2.debian.tar.xz' keyutils_1.6.1-2.debian.tar.xz 13412 SHA256:862442538428b514bb33a1c8488d4528c5ea48feca0ea5e60d8d34fd440f2355
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.6.1-2/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.6.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.6.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.18.3-7`

Binary Packages:

- `krb5-multidev:amd64=1.18.3-7`
- `libgssapi-krb5-2:amd64=1.18.3-7`
- `libgssrpc4:amd64=1.18.3-7`
- `libk5crypto3:amd64=1.18.3-7`
- `libkadm5clnt-mit12:amd64=1.18.3-7`
- `libkadm5srv-mit12:amd64=1.18.3-7`
- `libkdb5-10:amd64=1.18.3-7`
- `libkrb5-3:amd64=1.18.3-7`
- `libkrb5-dev:amd64=1.18.3-7`
- `libkrb5support0:amd64=1.18.3-7`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit12/copyright`, `/usr/share/doc/libkadm5srv-mit12/copyright`, `/usr/share/doc/libkdb5-10/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.18.3-7
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3-7.dsc' krb5_1.18.3-7.dsc 3160 SHA256:a5c8382335fb37e99f15266f2bf295700a1b2fda7d7db87899dd79a7f35514e9
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz' krb5_1.18.3.orig.tar.gz 8715312 SHA256:e61783c292b5efd9afb45c555a80dd267ac67eebabca42185362bee6c4fbd719
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz.asc' krb5_1.18.3.orig.tar.gz.asc 833 SHA256:ded19808ba7320ad0bb3ddfb5202845b2ff36a50613af7832f78dd3cb4437419
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3-7.debian.tar.xz' krb5_1.18.3-7.debian.tar.xz 106316 SHA256:6a40d855d2154b353f958f383741d09b5e0c252b263dccefa23ddc1ae77f77c2
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.18.3-7/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.18.3-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.18.3-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.12~rc1-2`

Binary Packages:

- `liblcms2-2:amd64=2.12~rc1-2`
- `liblcms2-dev:amd64=2.12~rc1-2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3 (GPL-3 for the fast_float plugin only)`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.12~rc1-2
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.12~rc1-2.dsc' lcms2_2.12~rc1-2.dsc 1988 SHA256:57b0b3cde709d8b7c43b195ba7f628d2d79323ee0db883050f253ee9f9acd48a
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.12~rc1.orig.tar.gz' lcms2_2.12~rc1.orig.tar.gz 7417767 SHA256:3300ddd8c51d60ebcc206d20d185b1b19939c4cec1576d1f5b95297b0fbdfe19
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.12~rc1-2.debian.tar.xz' lcms2_2.12~rc1-2.debian.tar.xz 10420 SHA256:dddb5b18a42fc7308e732f00643b29ac9f2638cf246569683cb50f13520c2cca
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.12~rc1-2/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.12~rc1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.12~rc1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.5.5-1`

Binary Packages:

- `libassuan0:amd64=2.5.5-1`

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
$ apt-get source -qq --print-uris libassuan=2.5.5-1
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-1.dsc' libassuan_2.5.5-1.dsc 2621 SHA256:b553cbb1dafea4a633ecbb47b829e7e8e570e956b831786b0f1bc02921076fc9
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2' libassuan_2.5.5.orig.tar.bz2 572263 SHA256:8e8c2fcc982f9ca67dcbb1d95e2dc746b1739a4668bc20b3a3c5be632edb34e4
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2.asc' libassuan_2.5.5.orig.tar.bz2.asc 228 SHA256:8bb0d1d818ac91fa27a8ebed2975dac12eac9a6e075dfba225cc488ac9b4133f
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-1.debian.tar.xz' libassuan_2.5.5-1.debian.tar.xz 14312 SHA256:66e6acbe39dadc7786dc9eab73f29a7f30b5fc00a96792f0faeb8643334e3a90
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.5-1/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.11.3-1`

Binary Packages:

- `libbsd0:amd64=0.11.3-1`

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

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.11.3-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3-1.dsc' libbsd_0.11.3-1.dsc 2292 SHA256:714c9cee71ddcea7a91593c56ca9ab297856e4f597743a32cda909544fe04ccb
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3.orig.tar.xz' libbsd_0.11.3.orig.tar.xz 399712 SHA256:ff95cf8184151dacae4247832f8d4ea8800fa127dbd15033ecfe839f285b42a1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3.orig.tar.xz.asc' libbsd_0.11.3.orig.tar.xz.asc 833 SHA256:213f30c9537e2a180ebdad6445402ea879f83c3a85907f7509ae7f7304f7ce1b
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3-1.debian.tar.xz' libbsd_0.11.3-1.debian.tar.xz 17504 SHA256:b414f384d71ebd8ed67b759526df4c83529946414c71cc3c5e5b98bc9323ad3b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.11.3-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.11.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.11.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.7.9-2.2`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.2+b1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.2
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.dsc' libcap-ng_0.7.9-2.2.dsc 2081 SHA256:d573ce59d83d2c117515e7c57dde1c990e9c5a34e0f53ac09f6b4d3e153e9aae
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.debian.tar.xz' libcap-ng_0.7.9-2.2.debian.tar.xz 6308 SHA256:6d7b5cfcf435fe996e5dc78770a9ab1ab614ced5bee56e3e0ba4e09d8c832a0a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap-ng/0.7.9-2.2/ (for browsing the source)
- https://sources.debian.net/src/libcap-ng/0.7.9-2.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap-ng/0.7.9-2.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap2=1:2.44-1`

Binary Packages:

- `libcap2:amd64=1:2.44-1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.44-1
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.44-1.dsc' libcap2_2.44-1.dsc 2179 SHA256:c356b4239be3c35ef4b7ef5b9f7ea1677da41a68ef9761a8cabc96023076ac83
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.44.orig.tar.xz' libcap2_2.44.orig.tar.xz 125568 SHA256:92188359cd5be86e8e5bd3f6483ac6ce582264f912398937ef763def2205c8e1
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.44-1.debian.tar.xz' libcap2_2.44-1.debian.tar.xz 21116 SHA256:f612c54d31b44b4f508342a3415f5d51deeffaf939d4b47068909bbb1fd6c0f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.44-1/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.44-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.44-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcbor=0.8.0-1`

Binary Packages:

- `libcbor0.8:amd64=0.8.0-1`

Licenses: (parsed from: `/usr/share/doc/libcbor0.8/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.8.0-1
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0-1.dsc' libcbor_0.8.0-1.dsc 2114 SHA256:ac9c9fc4f485846b085ad547a5fb4be4e0d9b9201759db3f07f5d181a5df2882
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0.orig.tar.gz' libcbor_0.8.0.orig.tar.gz 267044 SHA256:618097166ea4a54499646998ccaa949a5816e6a665cf1d6df383690895217c8b
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0-1.debian.tar.xz' libcbor_0.8.0-1.debian.tar.xz 4000 SHA256:fffb790f3c366c851fed63b204a436f916d0efe09050424902c9b2a00cf367fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcbor/0.8.0-1/ (for browsing the source)
- https://sources.debian.net/src/libcbor/0.8.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcbor/0.8.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdatrie=0.2.13-2`

Binary Packages:

- `libdatrie1:amd64=0.2.13-2`

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

### `dpkg` source package: `libde265=1.0.8-1`

Binary Packages:

- `libde265-0:amd64=1.0.8-1`

Licenses: (parsed from: `/usr/share/doc/libde265-0/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `other-1`
- `public-domain-1`
- `public-domain-2`

Source:

```console
$ apt-get source -qq --print-uris libde265=1.0.8-1
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.8-1.dsc' libde265_1.0.8-1.dsc 2216 SHA256:fea3b9010b68c3f0ab8f577c9a9fd1b89bfac1ae7b6814360d10cc0742528112
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.8.orig.tar.gz' libde265_1.0.8.orig.tar.gz 837878 SHA256:24c791dd334fa521762320ff54f0febfd3c09fc978880a8c5fbc40a88f21d905
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.8-1.debian.tar.xz' libde265_1.0.8-1.debian.tar.xz 8184 SHA256:cd82689cc5012a9aa726f9d3888552ab64866a273478e2da2e2ee99e07477ac9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libde265/1.0.8-1/ (for browsing the source)
- https://sources.debian.net/src/libde265/1.0.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libde265/1.0.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdeflate=1.8-1`

Binary Packages:

- `libdeflate-dev:amd64=1.8-1`
- `libdeflate0:amd64=1.8-1`

Licenses: (parsed from: `/usr/share/doc/libdeflate-dev/copyright`, `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.8-1
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.8-1.dsc' libdeflate_1.8-1.dsc 2188 SHA256:d88651a173ca65945a9cd6b0d87637a989855a872fff85cd98a48b12d682e81c
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.8.orig.tar.gz' libdeflate_1.8.orig.tar.gz 145823 SHA256:50711ad4e9d3862f8dfb11b97eb53631a86ee3ce49c0e68ec2b6d059a9662f61
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.8-1.debian.tar.xz' libdeflate_1.8-1.debian.tar.xz 4228 SHA256:300c0e15f1f22bbfca2e6edc6abae2cfe71692ca86c67dcccbb39bf846568add
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdeflate/1.8-1/ (for browsing the source)
- https://sources.debian.net/src/libdeflate/1.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdeflate/1.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20210910-1`

Binary Packages:

- `libedit2:amd64=3.1-20210910-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20210910-1
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20210910-1.dsc' libedit_3.1-20210910-1.dsc 2208 SHA256:abf92b2ddfccff4b50563e28bb7d6259ea69ce88d08691854a692cc2cfd45243
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20210910.orig.tar.gz' libedit_3.1-20210910.orig.tar.gz 524722 SHA256:6792a6a992050762edcca28ff3318cdb7de37dccf7bc30db59fcd7017eed13c5
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20210910-1.debian.tar.xz' libedit_3.1-20210910-1.debian.tar.xz 15080 SHA256:45ba2fb5e8ed56d9dff07be0bdb56bc566d7b7262e9f6b13f47b1042757f6199
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20210910-1/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20210910-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20210910-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.dsc' liberror-perl_0.17029-1.dsc 2336 SHA256:0590467fe8c5f81bff9336e991462b2a9994b4876f4b732c8b8b31e927987cd7
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA256:1a23f7913032aed6d4b68321373a3899ca66590f4727391a091ec19c95bf7adc
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.debian.tar.xz' liberror-perl_0.17029-1.debian.tar.xz 4552 SHA256:a753b142c4c33ebf9cc98ae5f7a08da13b7c9ca2823ec26e45c96efb9c15c42e
```

Other potentially useful URLs:

- https://sources.debian.net/src/liberror-perl/0.17029-1/ (for browsing the source)
- https://sources.debian.net/src/liberror-perl/0.17029-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liberror-perl/0.17029-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libevent=2.1.12-stable-1`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.12-stable-1`
- `libevent-core-2.1-7:amd64=2.1.12-stable-1`
- `libevent-dev=2.1.12-stable-1`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-1`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-1`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-1`

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
$ apt-get source -qq --print-uris libevent=2.1.12-stable-1
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.12-stable-1.dsc' libevent_2.1.12-stable-1.dsc 2527 SHA256:e82d9dc2160de05b1827b04894a954079e23ede0d5e2b5a1d9e9b2021e7c4e10
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA256:92e6de1be9ec176428fd2367677e61ceffc2ee1cb119035037a27d346b0403bb
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz.asc' libevent_2.1.12-stable.orig.tar.gz.asc 488 SHA256:3cd3d764777540305813495912cd5f7ea7d16edb456d6c88b331a1aa8974dfc2
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.12-stable-1.debian.tar.xz' libevent_2.1.12-stable-1.debian.tar.xz 17764 SHA256:cc608fff85ed5b262dee671fe17444aa6734dbc3be232e0b6ecca41252a62438
```

Other potentially useful URLs:

- https://sources.debian.net/src/libevent/2.1.12-stable-1/ (for browsing the source)
- https://sources.debian.net/src/libevent/2.1.12-stable-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libevent/2.1.12-stable-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libexif=0.6.23-1`

Binary Packages:

- `libexif-dev:amd64=0.6.23-1`
- `libexif12:amd64=0.6.23-1`

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
$ apt-get source -qq --print-uris libexif=0.6.23-1
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.23-1.dsc' libexif_0.6.23-1.dsc 2079 SHA256:7c17350b3049527e762ec4689c596f680ce6efbf925de0d9494348eaef0fbe29
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.23.orig.tar.gz' libexif_0.6.23.orig.tar.gz 1120548 SHA256:7701ec4b7071b1ac4f253c6d2478851c3baa5287302c336f68dd1810e8902bae
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.23-1.debian.tar.xz' libexif_0.6.23-1.debian.tar.xz 11672 SHA256:0f9d67618496755515d82463e9c743ed4f566c760e6091edcc93170076c9c879
```

Other potentially useful URLs:

- https://sources.debian.net/src/libexif/0.6.23-1/ (for browsing the source)
- https://sources.debian.net/src/libexif/0.6.23-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libexif/0.6.23-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.4.2-3`

Binary Packages:

- `libffi-dev:amd64=3.4.2-3`
- `libffi8:amd64=3.4.2-3`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi8/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.2-3
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2-3.dsc' libffi_3.4.2-3.dsc 1948 SHA256:afe7d32ea3ced400134b86395be11e61ba2ef0f06fa7867a276a71700632c3da
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2.orig.tar.gz' libffi_3.4.2.orig.tar.gz 1351355 SHA256:540fb721619a6aba3bdeef7d940d8e9e0e6d2c193595bc243241b77ff9e93620
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2-3.debian.tar.xz' libffi_3.4.2-3.debian.tar.xz 8128 SHA256:2d27d9690c5346b3919f4a8bc73642bfaed45f95e6f32cadb1dbfe9ba92c8370
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.4.2-3/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.4.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.4.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libfido2=1.9.0-1`

Binary Packages:

- `libfido2-1:amd64=1.9.0-1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.9.0-1
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.9.0-1.dsc' libfido2_1.9.0-1.dsc 2577 SHA256:7f8f891ce709f3cbf438497677e6e75bf1ad579880182cce73b23bc4d9203ab8
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.9.0.orig.tar.gz' libfido2_1.9.0.orig.tar.gz 576088 SHA256:ba39e3af3736d2dfc8ad3d1cb6e3be7eccc09588610a3b07c865d0ed3e58c2d2
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.9.0.orig.tar.gz.asc' libfido2_1.9.0.orig.tar.gz.asc 833 SHA256:7786065096a18c5fa2124a4f11288e06530432b57804c5b58616f90d1e51219d
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.9.0-1.debian.tar.xz' libfido2_1.9.0-1.debian.tar.xz 52328 SHA256:3cbcd00f6e82a2e867f6f693a28d0537bce679563c0152527a91ef40e78fe03f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfido2/1.9.0-1/ (for browsing the source)
- https://sources.debian.net/src/libfido2/1.9.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfido2/1.9.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.9.4-3`

Binary Packages:

- `libgcrypt20:amd64=1.9.4-3+b1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.9.4-3
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4-3.dsc' libgcrypt20_1.9.4-3.dsc 2800 SHA256:394c4e0742c70fe3c5582846b2874bd15d7b64128d9d7344a5a5167c4fddcf5e
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4.orig.tar.bz2' libgcrypt20_1.9.4.orig.tar.bz2 3239704 SHA256:ea849c83a72454e3ed4267697e8ca03390aee972ab421e7df69dfe42b65caaf7
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4.orig.tar.bz2.asc' libgcrypt20_1.9.4.orig.tar.bz2.asc 228 SHA256:aa44cb00b779b4e75f3e63abeedd4112b10b4b92914dad8f23438fd0217a9fec
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4-3.debian.tar.xz' libgcrypt20_1.9.4-3.debian.tar.xz 32624 SHA256:8fb19e3255ff6b3511f25f810c16de2f8ecb7fcabda218f1b091470c1d89598b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.9.4-3/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.9.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.9.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.42-3`

Binary Packages:

- `libgpg-error0:amd64=1.42-3`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.42-3
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.42-3.dsc' libgpg-error_1.42-3.dsc 2616 SHA256:fd2cf41359714da2ec9513b653264091e554c2adb97487b0f8f218a06165c29e
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.42.orig.tar.bz2' libgpg-error_1.42.orig.tar.bz2 973996 SHA256:fc07e70f6c615f8c4f590a8e37a9b8dd2e2ca1e9408f8e60459c67452b925e23
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.42-3.debian.tar.xz' libgpg-error_1.42-3.debian.tar.xz 19020 SHA256:067b323d85cf1f26adb128ffaf69f287f5c6e0ec8c398cffc8350de16e4c1d67
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.42-3/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.42-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.42-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libheif=1.12.0-2`

Binary Packages:

- `libheif1:amd64=1.12.0-2+b3`

Licenses: (parsed from: `/usr/share/doc/libheif1/copyright`)

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
$ apt-get source -qq --print-uris libheif=1.12.0-2
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.12.0-2.dsc' libheif_1.12.0-2.dsc 2283 SHA256:9cf77cca0efcb50632330d880143312545b6daa2201d1a2418fc18ecd5bad17e
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.12.0.orig.tar.gz' libheif_1.12.0.orig.tar.gz 1684355 SHA256:e1ac2abb354fdc8ccdca71363ebad7503ad731c84022cf460837f0839e171718
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.12.0-2.debian.tar.xz' libheif_1.12.0-2.debian.tar.xz 7012 SHA256:3f61679c2dd3d2b624a178756092799e1172924bb38e4870eb935ff38d51281c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libheif/1.12.0-2/ (for browsing the source)
- https://sources.debian.net/src/libheif/1.12.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libheif/1.12.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libidn2=2.3.2-2`

Binary Packages:

- `libidn2-0:amd64=2.3.2-2`

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
$ apt-get source -qq --print-uris libidn2=2.3.2-2
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.2-2.dsc' libidn2_2.3.2-2.dsc 2206 SHA256:43d4c3fed774f3204bc356a5b8963181227e85bee3be606011e683f561414861
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.2.orig.tar.gz' libidn2_2.3.2.orig.tar.gz 2169556 SHA256:76940cd4e778e8093579a9d195b25fff5e936e9dc6242068528b437a76764f91
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.2.orig.tar.gz.asc' libidn2_2.3.2.orig.tar.gz.asc 488 SHA256:3d533d0b18e031e90fbee0e552e1a034ef0b5bb11298019f0b99c0c85132ff9a
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.2-2.debian.tar.xz' libidn2_2.3.2-2.debian.tar.xz 15840 SHA256:d782cd5a3b0b316f56e1134da64d664c018db5b9cd2757b6dcb8cd54d4be1f2e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.3.2-2/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.3.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.3.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libjpeg-turbo=1:2.1.1-2`

Binary Packages:

- `libjpeg-dev:amd64=1:2.1.1-2`
- `libjpeg62-turbo:amd64=1:2.1.1-2`
- `libjpeg62-turbo-dev:amd64=1:2.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3-clause`
- `BSD-BY-LC-NE`
- `BSD-BY-LC-NE `
- `Expat`
- `NTP`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:2.1.1-2
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.1-2.dsc' libjpeg-turbo_2.1.1-2.dsc 2480 SHA256:f1249ab28bc6f47e6c058c76e59faf49392094090aa4a90d943a065418178a0f
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.1.orig.tar.gz' libjpeg-turbo_2.1.1.orig.tar.gz 2256321 SHA256:20e9cd3e5f517950dfb7a300ad344543d88719c254407ffb5ad88d891bf701c4
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.1-2.debian.tar.xz' libjpeg-turbo_2.1.1-2.debian.tar.xz 99720 SHA256:5484cc4adb537776bb69628bd622d2738acb91de2033b1d0f00b864991b0e55d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:2.1.1-2/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:2.1.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:2.1.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libksba=1.6.0-2`

Binary Packages:

- `libksba8:amd64=1.6.0-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.0-2
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0-2.dsc' libksba_1.6.0-2.dsc 2470 SHA256:0f8d4feca82987e43fb51fd6b63b5b2a93ecf825de45d958620e13df7866e31b
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2' libksba_1.6.0.orig.tar.bz2 662120 SHA256:dad683e6f2d915d880aa4bed5cea9a115690b8935b78a1bbe01669189307a48b
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2.asc' libksba_1.6.0.orig.tar.bz2.asc 228 SHA256:c695098f67cc837071d899f0e15d993bcf29eaac8f1ca7428ee793d9c62c795c
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0-2.debian.tar.xz' libksba_1.6.0-2.debian.tar.xz 14524 SHA256:59b54f92324bf527f9edc898d9b3113eee93bf0521e2443bda6e9aedf695ea79
```

Other potentially useful URLs:

- https://sources.debian.net/src/libksba/1.6.0-2/ (for browsing the source)
- https://sources.debian.net/src/libksba/1.6.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libksba/1.6.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libmaxminddb=1.5.2-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.5.2-1`
- `libmaxminddb0:amd64=1.5.2-1`

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
$ apt-get source -qq --print-uris libmaxminddb=1.5.2-1
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1.dsc' libmaxminddb_1.5.2-1.dsc 2322 SHA256:ffffa20e13b85b62961a39edd2caa59ae2fd4ff43abdc08f5a615ae6eab358c1
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2.orig.tar.gz' libmaxminddb_1.5.2.orig.tar.gz 249507 SHA256:afbbaa34875a379ed443bfa43b38aae44ed2b547592ac3213c27c2e531f620d5
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1.debian.tar.xz' libmaxminddb_1.5.2-1.debian.tar.xz 12328 SHA256:4ad8792791f91d7ed9ed8991076fe2abc8220ae80ac9a12bd339e89d71f05bfb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmaxminddb/1.5.2-1/ (for browsing the source)
- https://sources.debian.net/src/libmaxminddb/1.5.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmaxminddb/1.5.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmd=1.0.4-1`

Binary Packages:

- `libmd0:amd64=1.0.4-1`

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
$ apt-get source -qq --print-uris libmd=1.0.4-1
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4-1.dsc' libmd_1.0.4-1.dsc 2248 SHA256:2c3d69599f06af43417773ac3e5831696a5a3f9a6a7e5a6256bb3a6c6d18b3a1
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz' libmd_1.0.4.orig.tar.xz 264472 SHA256:f51c921042e34beddeded4b75557656559cf5b1f2448033b4c1eec11c07e530f
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz.asc' libmd_1.0.4.orig.tar.xz.asc 833 SHA256:32deebe1cfab127ee69a3e8c8caf439e459b7cdcdd7535fe021cb485adc14057
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4-1.debian.tar.xz' libmd_1.0.4-1.debian.tar.xz 10144 SHA256:a682fecf339adf56b5227934f3d994b5c144ba3798a80a7970ccbd04848c22a5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmd/1.0.4-1/ (for browsing the source)
- https://sources.debian.net/src/libmd/1.0.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmd/1.0.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libnsl=1.3.0-2`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-2`
- `libnsl2:amd64=1.3.0-2`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-2
'http://deb.debian.org/debian/pool/main/libn/libnsl/libnsl_1.3.0-2.dsc' libnsl_1.3.0-2.dsc 1955 SHA256:1da570eed6693c774cce51f3c33f989d1aa4bf1dcb8660818d8a834a1a3728ef
'http://deb.debian.org/debian/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA256:eac3062957fa302c62eff4aed718a07bacbf9ceb0a058289f12a19bfdda3c8e2
'http://deb.debian.org/debian/pool/main/libn/libnsl/libnsl_1.3.0-2.debian.tar.xz' libnsl_1.3.0-2.debian.tar.xz 4692 SHA256:7f8dccc706931b9e206448ffb475487a4a0abaded27cf611d418f4a34415dca7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libnsl/1.3.0-2/ (for browsing the source)
- https://sources.debian.net/src/libnsl/1.3.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libnsl/1.3.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng1.6=1.6.37-3`

Binary Packages:

- `libpng-dev:amd64=1.6.37-3`
- `libpng16-16:amd64=1.6.37-3`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.37-3
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3.dsc' libpng1.6_1.6.37-3.dsc 2225 SHA256:d6fac534b155e680849e700e4d2c87314e0ff20ab1b89fc22f1dfd2c24c1727b
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA256:ca74a0dace179a8422187671aee97dd3892b53e168627145271cad5b5ac81307
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3.debian.tar.xz' libpng1.6_1.6.37-3.debian.tar.xz 32272 SHA256:d28b11e41dba39c53d8d87be5f70cc96a246f296307855f55d86db03b24680d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpng1.6/1.6.37-3/ (for browsing the source)
- https://sources.debian.net/src/libpng1.6/1.6.37-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpng1.6/1.6.37-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpsl=0.21.0-1.2`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.2`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1.2
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.21.0-1.2.dsc' libpsl_0.21.0-1.2.dsc 2216 SHA256:d46b69dd1cb43dc48375d70c4895d0a0d5964131196a7de4e0ad1ea2912d6df4
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA256:055aa87ec166c7afb985d0816c07ff440e1eb899881a318c51c69a0aeea8e279
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.21.0-1.2.debian.tar.xz' libpsl_0.21.0-1.2.debian.tar.xz 12724 SHA256:012d3b6ec5634c59e6a4aa9f854d756ef23f08edf21d70ae5a888c55e95abd5d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpsl/0.21.0-1.2/ (for browsing the source)
- https://sources.debian.net/src/libpsl/0.21.0-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpsl/0.21.0-1.2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `librsvg=2.50.7+dfsg-2`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.50.7+dfsg-2`
- `librsvg2-2:amd64=2.50.7+dfsg-2`
- `librsvg2-common:amd64=2.50.7+dfsg-2`
- `librsvg2-dev:amd64=2.50.7+dfsg-2`

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
- `Expat`
- `Expat,`
- `LGPL-2`
- `LGPL-2+`
- `MPL-2.0`
- `MPL-2.0,`
- `Sun-permissive`
- `Sun-permissive,`
- `Unlicense`
- `Unlicense,`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.50.7+dfsg-2
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.50.7+dfsg-2.dsc' librsvg_2.50.7+dfsg-2.dsc 3120 SHA256:78616931c5d4c4d327032b612400e865a3797b2b71b124263c4e4e7fb6721932
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.50.7+dfsg.orig.tar.xz' librsvg_2.50.7+dfsg.orig.tar.xz 19827956 SHA256:30b26a213133163d5c8fa3e1ba943c9d96ce0977104211d5d1c96e07263bf521
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.50.7+dfsg-2.debian.tar.xz' librsvg_2.50.7+dfsg-2.debian.tar.xz 30188 SHA256:e093780d2273657d64c06265894fba6fa02798bec0b0f114ce4a2932346822a1
```

Other potentially useful URLs:

- https://sources.debian.net/src/librsvg/2.50.7+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/librsvg/2.50.7+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librsvg/2.50.7+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.5.2-2`

Binary Packages:

- `libseccomp2:amd64=2.5.2-2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.2-2
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.2-2.dsc' libseccomp_2.5.2-2.dsc 2676 SHA256:fe35f84dea6f5b9e4e7c30481c45e96f4c6ce77d351d2bf242a47251ed1a6b0a
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.2.orig.tar.gz' libseccomp_2.5.2.orig.tar.gz 640305 SHA256:17a652dfb491d96be893960e9b791914936ee16c13b777a3caf562fe48cb87df
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.2.orig.tar.gz.asc' libseccomp_2.5.2.orig.tar.gz.asc 833 SHA256:fad8440f5670296259288842d64c94d611dcdfc7707d52d4c249f4e810c6775d
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.2-2.debian.tar.xz' libseccomp_2.5.2-2.debian.tar.xz 27776 SHA256:70718c5e060d0b275a9e5dccdf109a8dc6720043392736cc474f61f74853c1ce
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.5.2-2/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.5.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.5.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.3-1`

Binary Packages:

- `libselinux1:amd64=3.3-1`
- `libselinux1-dev:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.3-1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.3-1.dsc' libselinux_3.3-1.dsc 2299 SHA256:7baed134b1b3ca0ab91810fc3ac5f7d936823c5a6b03020a0a07687902fdf0ac
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.3.orig.tar.gz' libselinux_3.3.orig.tar.gz 206826 SHA256:acfdee27633d2496508c28727c3d41d3748076f66d42fccde2e6b9f3463a7057
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.3-1.debian.tar.xz' libselinux_3.3-1.debian.tar.xz 23920 SHA256:d5fd8dc9de77c91c2cf56a497d30de9771e4d5f8c03be3cb6c99591aa5b42134
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libselinux/3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=3.3-1`

Binary Packages:

- `libsemanage-common=3.3-1`
- `libsemanage2:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.3-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.3-1.dsc' libsemanage_3.3-1.dsc 2320 SHA256:54c3a1cbaba0b05ed79b8f648d8e1b4d2a2dfb077ac4df1e696b99669ea3f8eb
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.3.orig.tar.gz' libsemanage_3.3.orig.tar.gz 178890 SHA256:84d0ec5afa34bbbb471f602d8c1bf317d12443d07852a34b60741d428d597ce8
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.3-1.debian.tar.xz' libsemanage_3.3-1.debian.tar.xz 17780 SHA256:198662d615e80e1b56d37624a97fbaddf680fe3900cbc939ce0bdf8c6996f021
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=3.3-1`

Binary Packages:

- `libsepol-dev:amd64=3.3-1`
- `libsepol2:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libsepol-dev/copyright`, `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.3-1
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.3-1.dsc' libsepol_3.3-1.dsc 1764 SHA256:38e1ced77afe590efc6037b38f07828389ba5c3ec137f990b00e6961939b7c53
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.3.orig.tar.gz' libsepol_3.3.orig.tar.gz 482546 SHA256:2d97df3eb8466169b389c3660acbb90c54200ac96e452eca9f41a9639f4f238b
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.3-1.debian.tar.xz' libsepol_3.3-1.debian.tar.xz 14956 SHA256:693e8394f88cc1430a16eb94f20c09f748ef73d73292956a8e7a0f8bd71f39e2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libsepol/3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsigsegv=2.13-1`

Binary Packages:

- `libsigsegv2:amd64=2.13-1`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.13-1
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.13-1.dsc' libsigsegv_2.13-1.dsc 2338 SHA256:6e22271eb31721e6b55b401c830aa2459654d3d08bd53688e86037b71fef5170
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.13.orig.tar.gz' libsigsegv_2.13.orig.tar.gz 460736 SHA256:be78ee4176b05f7c75ff03298d84874db90f4b6c9d5503f0da1226b3a3c48119
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.13.orig.tar.gz.asc' libsigsegv_2.13.orig.tar.gz.asc 819 SHA256:f63cbbc68da4a53b685dc373b5c11d0b0cdf467be9391efc89c88c440d74df36
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.13-1.debian.tar.xz' libsigsegv_2.13-1.debian.tar.xz 8572 SHA256:4210f5c3b99fd2521490f52345b4faca591f2fabb09b19a14e5644e8da8ac59a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsigsegv/2.13-1/ (for browsing the source)
- https://sources.debian.net/src/libsigsegv/2.13-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsigsegv/2.13-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libssh2=1.10.0-2`

Binary Packages:

- `libssh2-1:amd64=1.10.0-2`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.10.0-2
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0-2.dsc' libssh2_1.10.0-2.dsc 2251 SHA256:92aa9d2420ea476e72ef1d848a9cf0bc108be8b43a411bdbbc07aa65908cb2d5
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz' libssh2_1.10.0.orig.tar.gz 965044 SHA256:2d64e90f3ded394b91d3a2e774ca203a4179f69aebee03003e5a6fa621e41d51
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz.asc' libssh2_1.10.0.orig.tar.gz.asc 488 SHA256:75702eaf490fa8c1e69b889c5c6366c2c3f3b089bc715f9f9be081c88f115f81
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0-2.debian.tar.xz' libssh2_1.10.0-2.debian.tar.xz 8108 SHA256:9851cb16b52c978fdffdee0fbc0438db0ebb3045a9011842ba25a707fe0250a4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.10.0-2/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.10.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.10.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.18.0-4`

Binary Packages:

- `libtasn1-6:amd64=4.18.0-4`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.18.0-4
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0-4.dsc' libtasn1-6_4.18.0-4.dsc 2662 SHA256:bcb8a762bee62682d90c706bd1d03776e321d34a71e1847a9a3257cfcb99c557
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0.orig.tar.gz' libtasn1-6_4.18.0.orig.tar.gz 1724441 SHA256:4365c154953563d64c67a024b607d1ee75c6db76e0d0f65709ea80a334cd1898
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0.orig.tar.gz.asc' libtasn1-6_4.18.0.orig.tar.gz.asc 228 SHA256:68edccaf988071e0c0154495e82be0b783553a49762381435accc79f2fdb463d
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0-4.debian.tar.xz' libtasn1-6_4.18.0-4.debian.tar.xz 22020 SHA256:2a8dc71e52182787a53954fd3aca3195dc78173d13a1dc61ddda2719ce88014a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.18.0-4/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.18.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.18.0-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libthai=0.1.28-4.1`

Binary Packages:

- `libthai-data=0.1.28-4.1`
- `libthai0:amd64=0.1.28-4.1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.28-4.1
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28-4.1.dsc' libthai_0.1.28-4.1.dsc 2333 SHA256:0198b1fd8f623cfc246518e1eaf582287b21d7b11e4bb701e3b2308c6fdf2ff4
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28.orig.tar.xz' libthai_0.1.28.orig.tar.xz 413592 SHA256:ffe0a17b4b5aa11b153c15986800eca19f6c93a4025ffa5cf2cab2dcdf1ae911
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28-4.1.debian.tar.xz' libthai_0.1.28-4.1.debian.tar.xz 12852 SHA256:3e8fc1f49ea78ec16ca79414a6ea0632a92c67de8610ada1b841df4139bce33e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libthai/0.1.28-4.1/ (for browsing the source)
- https://sources.debian.net/src/libthai/0.1.28-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libthai/0.1.28-4.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtirpc=1.3.2-2`

Binary Packages:

- `libtirpc-common=1.3.2-2`
- `libtirpc-dev:amd64=1.3.2-2`
- `libtirpc3:amd64=1.3.2-2`

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
$ apt-get source -qq --print-uris libtirpc=1.3.2-2
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.2-2.dsc' libtirpc_1.3.2-2.dsc 2111 SHA256:830223f0db2a95266185d18cc75691d37ba1ae001616df7f11a42cd1e9dd3394
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.2.orig.tar.bz2' libtirpc_1.3.2.orig.tar.bz2 513151 SHA256:e24eb88b8ce7db3b7ca6eb80115dd1284abc5ec32a8deccfed2224fc2532b9fd
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.2-2.debian.tar.xz' libtirpc_1.3.2-2.debian.tar.xz 10996 SHA256:ad8da93212dae510e8568f242abb4aef2694981aab45a6c0357d73d5f9d2d517
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtirpc/1.3.2-2/ (for browsing the source)
- https://sources.debian.net/src/libtirpc/1.3.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtirpc/1.3.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtool=2.4.6-15`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-15`
- `libltdl7:amd64=2.4.6-15`
- `libtool=2.4.6-15`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-15
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-15.dsc' libtool_2.4.6-15.dsc 2502 SHA256:c499bd88103239f5d9743c70fd9e84260b0237e43df47c44980ef4ac9ff5f8e0
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-15.debian.tar.xz' libtool_2.4.6-15.debian.tar.xz 53924 SHA256:3955615804746d1440f2880f5cc0cd19e50dbaffe689afbec45dfcaaf5ee0d35
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtool/2.4.6-15/ (for browsing the source)
- https://sources.debian.net/src/libtool/2.4.6-15/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtool/2.4.6-15/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=0.9.10-6`

Binary Packages:

- `libunistring2:amd64=0.9.10-6`

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
$ apt-get source -qq --print-uris libunistring=0.9.10-6
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-6.dsc' libunistring_0.9.10-6.dsc 2212 SHA256:68c06ffeb5dad6aa1af21e59543389028a34d2fadeb1a0bbefcc96b4b8501060
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-6.debian.tar.xz' libunistring_0.9.10-6.debian.tar.xz 41588 SHA256:fb58a310ffeff4aa93b154a852612bcdc0fdff4c24ea9acc9521fbdae54998f1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/0.9.10-6/ (for browsing the source)
- https://sources.debian.net/src/libunistring/0.9.10-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/0.9.10-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwebp=0.6.1-2.1`

Binary Packages:

- `libwebp-dev:amd64=0.6.1-2.1`
- `libwebp6:amd64=0.6.1-2.1`
- `libwebpdemux2:amd64=0.6.1-2.1`
- `libwebpmux3:amd64=0.6.1-2.1`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.6.1-2.1
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.6.1-2.1.dsc' libwebp_0.6.1-2.1.dsc 2054 SHA256:b1045ce17d7f16666347813a6b7da16cba304ec33b28e12bda6e83c40243d46f
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA256:a86045e3ec24704bddbaa369ca30980d6bf4f2625f4cdca03715e91f9c08bbb4
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.6.1-2.1.debian.tar.xz' libwebp_0.6.1-2.1.debian.tar.xz 13616 SHA256:239203fd35a0b26b9e627a509b91a27efa10d996ebc068779bff024af9570ad8
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwebp/0.6.1-2.1/ (for browsing the source)
- https://sources.debian.net/src/libwebp/0.6.1-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwebp/0.6.1-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwmf=0.2.8.4-17`

Binary Packages:

- `libwmf-dev=0.2.8.4-17+b1`
- `libwmf0.2-7:amd64=0.2.8.4-17+b1`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-17
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.8.4-17.dsc' libwmf_0.2.8.4-17.dsc 2268 SHA256:1d48da0032093725c16f1c389152cc4041e60323a8453c550310286a0cfafa6a
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.8.4-17.debian.tar.xz' libwmf_0.2.8.4-17.debian.tar.xz 12900 SHA256:d32d2b4c948abb929911c7b23ef9490863d86e3c6b6302aa3549d25301e0fed1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwmf/0.2.8.4-17/ (for browsing the source)
- https://sources.debian.net/src/libwmf/0.2.8.4-17/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwmf/0.2.8.4-17/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.7.2-2`

Binary Packages:

- `libx11-6:amd64=2:1.7.2-2+b1`
- `libx11-data=2:1.7.2-2`
- `libx11-dev:amd64=2:1.7.2-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.7.2-2
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2-2.dsc' libx11_1.7.2-2.dsc 2539 SHA256:0bd21cfab5aa081cc63e01ee468e7c858c7ef70f8243de1908ba037554db840b
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz' libx11_1.7.2.orig.tar.gz 3181228 SHA256:2c26ccd08f43a6214de89110554fbe97c71692eeb7e7d4829f3004ae6fafd2c0
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz.asc' libx11_1.7.2.orig.tar.gz.asc 833 SHA256:509d0ed983ff3aed0dbfb070dabfce82b5787e626f2fd0bfb2a5887918fcd967
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2-2.diff.gz' libx11_1.7.2-2.diff.gz 78109 SHA256:c73eb4758eaa9939060fe89b1aa1d03cb5f3f3ce9e701d7abcf9cdc28cd2048c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.7.2-2/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.7.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.7.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxcb=1.14-3`

Binary Packages:

- `libxcb-render0:amd64=1.14-3`
- `libxcb-render0-dev:amd64=1.14-3`
- `libxcb-shm0:amd64=1.14-3`
- `libxcb-shm0-dev:amd64=1.14-3`
- `libxcb1:amd64=1.14-3`
- `libxcb1-dev:amd64=1.14-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-3
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.14-3.dsc' libxcb_1.14-3.dsc 5373 SHA256:25030a957600e3afcfecd095e3c1187885818a8a3fe8346ae965fe62c3a3b2eb
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA256:2c7fcddd1da34d9b238c9caeda20d3bd7486456fc50b3cc6567185dbd5b0ad02
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.14-3.diff.gz' libxcb_1.14-3.diff.gz 26583 SHA256:aed546fff9cf733c52188ad4f0d869a5ee8ffec52b54a6fa8f666a87adda82a3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcb/1.14-3/ (for browsing the source)
- https://sources.debian.net/src/libxcb/1.14-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcb/1.14-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcrypt=1:4.4.26-1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.26-1`
- `libcrypt1:amd64=1:4.4.26-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.26-1
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.26-1.dsc' libxcrypt_4.4.26-1.dsc 1525 SHA256:8008957728d5a27a75c0774bc58527686a5d011fbc881cab3caf2e6308689d48
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.26.orig.tar.xz' libxcrypt_4.4.26.orig.tar.xz 390592 SHA256:72cc109c883829cd86817a4f597e6cb69cfc2611160e700121bc50fe5aa21583
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.26-1.debian.tar.xz' libxcrypt_4.4.26-1.debian.tar.xz 7744 SHA256:5997396f7c0de5f73613c04c913bba1f95b8447a8cab1e078218ba52996ac41a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.26-1/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.26-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.26-1/ (for access to the source package after it no longer exists in the archive)

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

- `libxext-dev:amd64=2:1.3.4-1`
- `libxext6:amd64=2:1.3.4-1`

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

### `dpkg` source package: `libxml2=2.9.12+dfsg-5`

Binary Packages:

- `libxml2:amd64=2.9.12+dfsg-5`
- `libxml2-dev:amd64=2.9.12+dfsg-5`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.12+dfsg-5
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.12+dfsg-5.dsc' libxml2_2.9.12+dfsg-5.dsc 2576 SHA256:a8ed15cbe14a997109d5a81fde9af5fcd0adafc2026fd9f4932adb3e2b0a4f28
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.12+dfsg.orig.tar.xz' libxml2_2.9.12+dfsg.orig.tar.xz 2535044 SHA256:e25d1b3e476f01f3c8c6b34950fa1be5535c13ef5207825cafe285bc88fd4ed0
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.12+dfsg-5.debian.tar.xz' libxml2_2.9.12+dfsg-5.debian.tar.xz 32960 SHA256:ba1b6ec8ea12312cdffd1d7b24dbdfed2702ba920bab6f2029940be8159d2851
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxml2/2.9.12+dfsg-5/ (for browsing the source)
- https://sources.debian.net/src/libxml2/2.9.12+dfsg-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxml2/2.9.12+dfsg-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxrender=1:0.9.10-1`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1`
- `libxrender1:amd64=1:0.9.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.dsc' libxrender_0.9.10-1.dsc 2064 SHA256:95d6471218b44f4e60c48cea60cfb4865bbe861530add23f6c859515bee92dbd
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA256:770527cce42500790433df84ec3521e8bf095dfe5079454a92236494ab296adf
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.diff.gz' libxrender_0.9.10-1.diff.gz 15399 SHA256:ff56a0a00119383adc5f1731e86155ae5c2de069e1d059a9da1d777917430588
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxrender/1:0.9.10-1/ (for browsing the source)
- https://sources.debian.net/src/libxrender/1:0.9.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxrender/1:0.9.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxslt=1.1.34-4`

Binary Packages:

- `libxslt1-dev:amd64=1.1.34-4`
- `libxslt1.1:amd64=1.1.34-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.34-4
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34-4.dsc' libxslt_1.1.34-4.dsc 2375 SHA256:29447f928b2fd534bd819aaf74005ff286f3786689a2684b9cbc61c1c65c2212
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA256:98b1bd46d6792925ad2dfe9a87452ea2adebf69dcb9919ffd55bf926a7f93f7f
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA256:673d1477552bdd5b0cc665704e77ca70e6be5d2f257e6a5a341c846719d747cf
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34-4.debian.tar.xz' libxslt_1.1.34-4.debian.tar.xz 21464 SHA256:24d5490d6e33f42391d2ce449dd8fec0830ced115a6af886ee03af985a727dc9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxslt/1.1.34-4/ (for browsing the source)
- https://sources.debian.net/src/libxslt/1.1.34-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxslt/1.1.34-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxt=1:1.2.0-1`

Binary Packages:

- `libxt-dev:amd64=1:1.2.0-1`
- `libxt6:amd64=1:1.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.0-1
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0-1.dsc' libxt_1.2.0-1.dsc 2298 SHA256:945650656e7f24f1276a1c100067e7fa728d50d7af93b4fcc149e5a5323df165
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz' libxt_1.2.0.orig.tar.gz 1016961 SHA256:d4bee88898fc5e1dc470e361430c72fbc529b9cdbbb6c0ed3affea3a39f97d8d
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz.asc' libxt_1.2.0.orig.tar.gz.asc 195 SHA256:4c5fe1bceef4aa507d5a95d2636e7ce257ee4f2b5522989ec4a7281cbe860564
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0-1.diff.gz' libxt_1.2.0-1.diff.gz 31129 SHA256:eb723d0651e39c56d1e81fb7519e5093fd7e0177d42fd458d539163512076e52
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxt/1:1.2.0-1/ (for browsing the source)
- https://sources.debian.net/src/libxt/1:1.2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxt/1:1.2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libyaml=0.2.2-1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.2-1`
- `libyaml-dev:amd64=0.2.2-1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.2-1
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.2.2-1.dsc' libyaml_0.2.2-1.dsc 1833 SHA256:b4baba985391f52409013a0c9303191e34aaa4c1c9200e4c01c4963df801db09
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.2.2.orig.tar.gz' libyaml_0.2.2.orig.tar.gz 602509 SHA256:689ef3ebdecfa81f3789ccd2481acc81fc0f22f3f5c947eed95c4c0802e356b8
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.2.2-1.debian.tar.xz' libyaml_0.2.2-1.debian.tar.xz 4112 SHA256:186aad3e4bcd95891a8c59249c59f862f5f71601058fda0bf020a9e9e39320fe
```

Other potentially useful URLs:

- https://sources.debian.net/src/libyaml/0.2.2-1/ (for browsing the source)
- https://sources.debian.net/src/libyaml/0.2.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libyaml/0.2.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.4.8+dfsg-3`

Binary Packages:

- `libzstd1:amd64=1.4.8+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.8+dfsg-3
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-3.dsc' libzstd_1.4.8+dfsg-3.dsc 2291 SHA256:03a5589a689fb0e6480ee26af40104ce67a435f7b70d2bdd156221666d9d530a
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8+dfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA256:1e8ce5c4880a6d5bd8d3186e4186607dd19b64fc98a3877fc13aeefd566d67c5
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-3.debian.tar.xz' libzstd_1.4.8+dfsg-3.debian.tar.xz 12184 SHA256:fecd87a469d5a07b6deeeef53ed24b2f1a74ee097ce11528fe3b58540f05c147
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.4.8+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.4.8+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.4.8+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `linux=5.14.16-1`

Binary Packages:

- `linux-libc-dev:amd64=5.14.16-1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `BSD-2-clause`
- `CRYPTOGAMS`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `Unicode-data`
- `X11`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=5.14.16-1
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.14.16-1.dsc' linux_5.14.16-1.dsc 191803 SHA256:d39b6cbb8a5720d7b5a06f853774bd06ce06a5aadfe2dfde7d1b21f3b3799fdd
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.14.16.orig.tar.xz' linux_5.14.16.orig.tar.xz 126466584 SHA256:09586fa02ed391b1dcda3344d8f471566b64a822aec372b7ab0ad8b7c3eb136f
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.14.16-1.debian.tar.xz' linux_5.14.16-1.debian.tar.xz 1421140 SHA256:6240dfbd11237255ea6d23981d7adb29cd6e57ac178d35c4f096474df759d936
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/5.14.16-1/ (for browsing the source)
- https://sources.debian.net/src/linux/5.14.16-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/5.14.16-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lsb=11.1.0`

Binary Packages:

- `lsb-base=11.1.0`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_11.1.0.dsc' lsb_11.1.0.dsc 1800 SHA256:5cb5679dcc92e30aa878f892f73081d6b4d5299841549f6d53a886d51509feb1
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_11.1.0.tar.xz' lsb_11.1.0.tar.xz 42452 SHA256:c7926d511228862892630070f7708c425db9473ceefc70872868c448b5145b57
```

Other potentially useful URLs:

- https://sources.debian.net/src/lsb/11.1.0/ (for browsing the source)
- https://sources.debian.net/src/lsb/11.1.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lsb/11.1.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lz4=1.9.3-2`

Binary Packages:

- `liblz4-1:amd64=1.9.3-2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.3-2
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.3-2.dsc' lz4_1.9.3-2.dsc 1959 SHA256:215e1f0be1bb40e2b89182f3a1bf630463d8acdc0917f1f928ad1bf9ef3e1b0c
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.3.orig.tar.gz' lz4_1.9.3.orig.tar.gz 320958 SHA256:030644df4611007ff7dc962d981f390361e6c97a34e5cbc393ddfbe019ffe2c1
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.3-2.debian.tar.xz' lz4_1.9.3-2.debian.tar.xz 13928 SHA256:d7754a7b7b1fa196666d6459705107355e15fef162352e363e43722e012a04e3
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.9.3-2/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.9.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.9.3-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `m4=1.4.18-5`

Binary Packages:

- `m4=1.4.18-5`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-5
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-5.dsc' m4_1.4.18-5.dsc 1637 SHA256:ebc66cf67735240e2129cfbf20b8441e5144ef75c9fca0782a81eece8ae0f9d5
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA256:a2a9fff657e65ff25a8f3734f484dbd3ede8f8290786af71626de367dcd74267
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-5.debian.tar.xz' m4_1.4.18-5.debian.tar.xz 17468 SHA256:94861648b7e3bc0e47eb0746d3c5717c879e74e59928be69064fa9968bc8f228
```

Other potentially useful URLs:

- https://sources.debian.net/src/m4/1.4.18-5/ (for browsing the source)
- https://sources.debian.net/src/m4/1.4.18-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/m4/1.4.18-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mariadb-10.6=1:10.6.4-1`

Binary Packages:

- `libmariadb-dev=1:10.6.4-1+b1`
- `libmariadb-dev-compat:amd64=1:10.6.4-1+b1`
- `libmariadb3:amd64=1:10.6.4-1+b1`
- `mariadb-common=1:10.6.4-1`

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
$ apt-get source -qq --print-uris mariadb-10.6=1:10.6.4-1
'http://deb.debian.org/debian/pool/main/m/mariadb-10.6/mariadb-10.6_10.6.4-1.dsc' mariadb-10.6_10.6.4-1.dsc 4573 SHA256:c56d9a204f27b4f8d5f7ac07bdda0f0ff8c092264724a3eec3611c9d9a1d223b
'http://deb.debian.org/debian/pool/main/m/mariadb-10.6/mariadb-10.6_10.6.4.orig.tar.gz' mariadb-10.6_10.6.4.orig.tar.gz 81768627 SHA256:55179fc9487439c3a96c4f19277f47eef6495fef8dc123ad269c28acfe52d752
'http://deb.debian.org/debian/pool/main/m/mariadb-10.6/mariadb-10.6_10.6.4-1.debian.tar.xz' mariadb-10.6_10.6.4-1.debian.tar.xz 223516 SHA256:f4ea10939c36ab7b490f1dadbf47490feb281245a2250b8feddffab3bcf4ffc2
```

Other potentially useful URLs:

- https://sources.debian.net/src/mariadb-10.6/1:10.6.4-1/ (for browsing the source)
- https://sources.debian.net/src/mariadb-10.6/1:10.6.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mariadb-10.6/1:10.6.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mawk=1.3.4.20200120-2`

Binary Packages:

- `mawk=1.3.4.20200120-2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-2
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-2.dsc' mawk_1.3.4.20200120-2.dsc 1915 SHA256:5069c46872ac74f5221250dfb88b31b1f2dbb8a2617c1e013f8f80cc34638c6d
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-2.debian.tar.xz' mawk_1.3.4.20200120-2.debian.tar.xz 7504 SHA256:b772ed2f016b0286980c46cbc1f1f4ae62887ef2aa3dff6ef10cae638f923f26
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.4.20200120-2/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.4.20200120-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.4.20200120-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `media-types=4.0.0`

Binary Packages:

- `media-types=4.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=4.0.0
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_4.0.0.dsc' media-types_4.0.0.dsc 1620 SHA256:422edc1275dcc6bf07ac1b30612f501624cba04cfca2331eb87f1ca3af89e701
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_4.0.0.tar.xz' media-types_4.0.0.tar.xz 33988 SHA256:b5eb14fd6addb8f10c1665ebaa113cd0ebfb47f692cf27d9ac47405b13ce4e31
```

Other potentially useful URLs:

- https://sources.debian.net/src/media-types/4.0.0/ (for browsing the source)
- https://sources.debian.net/src/media-types/4.0.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/media-types/4.0.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mercurial=5.9.3-1`

Binary Packages:

- `mercurial=5.9.3-1`
- `mercurial-common=5.9.3-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=5.9.3-1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.9.3-1.dsc' mercurial_5.9.3-1.dsc 2764 SHA256:22ebb3a426e13886a4082905c72e7a138f72f6fc1467f9ecf41a7e5772b31cd4
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.9.3.orig.tar.gz' mercurial_5.9.3.orig.tar.gz 8126023 SHA256:3b43f68977ad0fa75aa7f1e5c8f0a83ba935621ab2396129abb498e56d1be08e
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.9.3.orig.tar.gz.asc' mercurial_5.9.3.orig.tar.gz.asc 833 SHA256:2a6aa63ecf7216f18819a86be13f085e3391b91c315f274f03610f82e5c2bbe8
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.9.3-1.debian.tar.xz' mercurial_5.9.3-1.debian.tar.xz 69492 SHA256:0746fe2c9ee8cf7fb439564b81a96d62228e52e1e7cbb4daada50f617710812d
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/5.9.3-1/ (for browsing the source)
- https://sources.debian.net/src/mercurial/5.9.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/5.9.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpclib3=1.2.1-1`

Binary Packages:

- `libmpc3:amd64=1.2.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.1-1
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.2.1-1.dsc' mpclib3_1.2.1-1.dsc 1851 SHA256:335b35bafc6b678a64b7d23c9a9baabf1162f0bdf25015df04d3aa4b517cd52f
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.2.1.orig.tar.gz' mpclib3_1.2.1.orig.tar.gz 838731 SHA256:17503d2c395dfcf106b622dc142683c1199431d095367c6aacba6eec30340459
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.2.1-1.diff.gz' mpclib3_1.2.1-1.diff.gz 4264 SHA256:1be20027ddaa518d4520449134b3bf701617b71b47632613c4ac72120f60b1cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpclib3/1.2.1-1/ (for browsing the source)
- https://sources.debian.net/src/mpclib3/1.2.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpclib3/1.2.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpdecimal=2.5.1-2`

Binary Packages:

- `libmpdec3:amd64=2.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libmpdec3/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.5.1-2
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1-2.dsc' mpdecimal_2.5.1-2.dsc 1919 SHA256:293054eddc70e50d3a482d1fec446a7f10202b9c6f7ceaf92600f60b429f8919
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1.orig.tar.gz' mpdecimal_2.5.1.orig.tar.gz 2584021 SHA256:9f9cd4c041f99b5c49ffb7b59d9f12d95b683d88585608aa56a6307667b2b21f
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1-2.debian.tar.xz' mpdecimal_2.5.1-2.debian.tar.xz 6696 SHA256:5ff6a2502605579d140614e7c023c14d363f520253cc2ef8e844651807237321
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpdecimal/2.5.1-2/ (for browsing the source)
- https://sources.debian.net/src/mpdecimal/2.5.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpdecimal/2.5.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpfr4=4.1.0-3`

Binary Packages:

- `libmpfr6:amd64=4.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.1.0-3
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.1.0-3.dsc' mpfr4_4.1.0-3.dsc 1959 SHA256:6d2727cf53e788020f671a2cba644ff5dd4e28a2531e66c3ed32d98ce2b5bf4e
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA256:0c98a3f1732ff6ca4ea690552079da9c597872d30e96ec28414ee23c95558a7f
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.1.0-3.debian.tar.xz' mpfr4_4.1.0-3.debian.tar.xz 12372 SHA256:b329dd24cba377ed4160c0819a5ec110e029fb52c93e9a141847d5ed2a2068e8
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpfr4/4.1.0-3/ (for browsing the source)
- https://sources.debian.net/src/mpfr4/4.1.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpfr4/4.1.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mysql-defaults=1.0.7`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.7`
- `mysql-common=5.8+1.0.7`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.7
'http://deb.debian.org/debian/pool/main/m/mysql-defaults/mysql-defaults_1.0.7.dsc' mysql-defaults_1.0.7.dsc 2266 SHA256:969c5682e991967f5b9488c04b784e63148c952fc597f7b7e5483e4204726649
'http://deb.debian.org/debian/pool/main/m/mysql-defaults/mysql-defaults_1.0.7.tar.xz' mysql-defaults_1.0.7.tar.xz 7220 SHA256:e2942479d614756e2e49698a6a3819b6e00b1285802799dab5519e0d2925437b
```

Other potentially useful URLs:

- https://sources.debian.net/src/mysql-defaults/1.0.7/ (for browsing the source)
- https://sources.debian.net/src/mysql-defaults/1.0.7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mysql-defaults/1.0.7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.2+20210905-1`

Binary Packages:

- `ncurses-base=6.2+20210905-1`

Licenses: (parsed from: `/usr/share/doc/ncurses-base/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2+20210905-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20210905-1.dsc' ncurses_6.2+20210905-1.dsc 4200 SHA256:1504cd85b5f051be5f330064b188853be7722198aa3486856aa422dd693d672b
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20210905.orig.tar.gz' ncurses_6.2+20210905.orig.tar.gz 3595045 SHA256:a3bc85840d14463994f4172389bf62592d6df94e6883aedb4328aa555e0839bd
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20210905.orig.tar.gz.asc' ncurses_6.2+20210905.orig.tar.gz.asc 729 SHA256:b48b912eeb72d8c447249e35d1f4a380bc73d26670d2db1f3a9890eb44fc00a3
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20210905-1.debian.tar.xz' ncurses_6.2+20210905-1.debian.tar.xz 54176 SHA256:33f2b0313c33ccb41f03c3038c164d6e64fc76b1df9d973857b7347b73eae696
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.2+20210905-1/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.2+20210905-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.2+20210905-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.3-1`

Binary Packages:

- `libncurses-dev:amd64=6.3-1`
- `libncurses5-dev:amd64=6.3-1`
- `libncurses6:amd64=6.3-1`
- `libncursesw5-dev:amd64=6.3-1`
- `libncursesw6:amd64=6.3-1`
- `libtinfo6:amd64=6.3-1`
- `ncurses-bin=6.3-1`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.3-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3-1.dsc' ncurses_6.3-1.dsc 4110 SHA256:6f299776baeb75c8b77eb7fe02b411f878aa9582e6e80d36f7b559ae6276fc9f
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3.orig.tar.gz' ncurses_6.3.orig.tar.gz 3583550 SHA256:97fc51ac2b085d4cde31ef4d2c3122c21abc217e9090a43a30fc5ec21684e059
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3.orig.tar.gz.asc' ncurses_6.3.orig.tar.gz.asc 729 SHA256:37b9e80c11fa02fbd8caf42ab9573427f54f2c7212eb4aeec9f455b5d79dee14
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3-1.debian.tar.xz' ncurses_6.3-1.debian.tar.xz 54216 SHA256:371007cd56b353965874d483d1417580dd00dbe78c20698fafb46dc70913cc78
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.3-1/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `netbase=6.3`

Binary Packages:

- `netbase=6.3`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.3
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.3.dsc' netbase_6.3.dsc 875 SHA256:f16f43e8b51814911d679d91cbfa9e9be4930a7c59c294c70b6af43ae7a1d42f
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.3.tar.xz' netbase_6.3.tar.xz 31968 SHA256:7c42a6a1cafa0c64103c71cab6431fc8613179b2449a1a00e55e3584e860d81c
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/6.3/ (for browsing the source)
- https://sources.debian.net/src/netbase/6.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/6.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.7.3-1`

Binary Packages:

- `libhogweed6:amd64=3.7.3-1`
- `libnettle8:amd64=3.7.3-1`

Licenses: (parsed from: `/usr/share/doc/libhogweed6/copyright`, `/usr/share/doc/libnettle8/copyright`)

- `Expat`
- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3+`
- `GPL-3+ with Autoconf exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-3+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=3.7.3-1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.7.3-1.dsc' nettle_3.7.3-1.dsc 2033 SHA256:63a1a80f37b6484f479dfa1cbd30152feff3b1a5a2161fdab05b90edde212c1f
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.7.3.orig.tar.gz' nettle_3.7.3.orig.tar.gz 2383985 SHA256:661f5eb03f048a3b924c3a8ad2515d4068e40f67e774e8a26827658007e3bcf0
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.7.3-1.debian.tar.xz' nettle_3.7.3-1.debian.tar.xz 21956 SHA256:97af0e306aec6f6c5d8e73a7a3ce2856c76bcff9cdcfa7640e932a5a3aee9f24
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.7.3-1/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.7.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.7.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nghttp2=1.43.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.43.0-1`

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
$ apt-get source -qq --print-uris nghttp2=1.43.0-1
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.43.0-1.dsc' nghttp2_1.43.0-1.dsc 2548 SHA256:287a6fa84523ad2e6bb2215bcfc7ecc413a536fc9af20b0b20f0984e64bb034d
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.43.0.orig.tar.bz2' nghttp2_1.43.0.orig.tar.bz2 4521786 SHA256:556f24653397c71ebb8270b3c5e5507f0893e6eac2c6eeda6be2ecf6e1f50f62
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.43.0-1.debian.tar.xz' nghttp2_1.43.0-1.debian.tar.xz 16308 SHA256:5dbb013a6f2152354fee33a2ecf08817738d4f8f4d78bec0cd0cb3bcac690821
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.43.0-1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.43.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.43.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `numactl=2.0.14-3`

Binary Packages:

- `libnuma1:amd64=2.0.14-3`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.14-3
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.14-3.dsc' numactl_2.0.14-3.dsc 1974 SHA256:912fbd67b2a0e555d3af71aa40d0d86518943a752fc9946d0bdbee57b4db28e2
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.14.orig.tar.gz' numactl_2.0.14.orig.tar.gz 107593 SHA256:159799e9101faf123454bc0193c8c941b4c676552bc8178e5e8a3d68691e1020
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.14-3.debian.tar.xz' numactl_2.0.14-3.debian.tar.xz 6992 SHA256:1cbe8d7a5cba6f42ef3c4c116ebed1313dc5b4df7220f2b420dc7bf16a4b3327
```

Other potentially useful URLs:

- https://sources.debian.net/src/numactl/2.0.14-3/ (for browsing the source)
- https://sources.debian.net/src/numactl/2.0.14-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/numactl/2.0.14-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openexr=2.5.7-1`

Binary Packages:

- `libopenexr-dev=2.5.7-1`
- `libopenexr25:amd64=2.5.7-1`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr25/copyright`)

- `BSD-3-clause`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.5.7-1
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.5.7-1.dsc' openexr_2.5.7-1.dsc 2683 SHA256:dd0b42162ad701bed78787414609b2d784e44d6e1693c4cf3992572f5cf62caa
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.5.7.orig.tar.gz' openexr_2.5.7.orig.tar.gz 27539574 SHA256:36ecb2290cba6fc92b2ec9357f8dc0e364b4f9a90d727bf9a57c84760695272d
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.5.7.orig.tar.gz.asc' openexr_2.5.7.orig.tar.gz.asc 287 SHA256:a2c4ac5151789903ca8ab3093a2798491463ccf2abfd003a20f96453e505dd5f
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.5.7-1.debian.tar.xz' openexr_2.5.7-1.debian.tar.xz 22096 SHA256:6168e2eb9d8974e11f1ea69a1a5bbe41b33e3bc63efa2a2073863c1f9dc45585
```

Other potentially useful URLs:

- https://sources.debian.net/src/openexr/2.5.7-1/ (for browsing the source)
- https://sources.debian.net/src/openexr/2.5.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openexr/2.5.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openjpeg2=2.4.0-3`

Binary Packages:

- `libopenjp2-7:amd64=2.4.0-3`
- `libopenjp2-7-dev=2.4.0-3`

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
$ apt-get source -qq --print-uris openjpeg2=2.4.0-3
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.4.0-3.dsc' openjpeg2_2.4.0-3.dsc 2768 SHA256:c2de7ec896d9fccad5a9d58761593446a0271564babf218fd4ab200b6fe92a05
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.4.0.orig.tar.xz' openjpeg2_2.4.0.orig.tar.xz 1396964 SHA256:4b89da8abea5ea4e8dd5b214f1633a492554d784b5aebc22cb6495a1e5fe681c
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.4.0-3.debian.tar.xz' openjpeg2_2.4.0-3.debian.tar.xz 19712 SHA256:99b94d26c341babae8b5599ca7f8f0e1bb2021eb282ceff5d3c91086d1a3bcfc
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjpeg2/2.4.0-3/ (for browsing the source)
- https://sources.debian.net/src/openjpeg2/2.4.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjpeg2/2.4.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.59+dfsg-1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.59+dfsg-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.59+dfsg-1
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.59+dfsg-1.dsc' openldap_2.4.59+dfsg-1.dsc 3113 SHA256:cc2578c30b177406eb9cc1341cca710e4c4ac66230c40633f11a2a26290a6336
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.59+dfsg.orig.tar.gz' openldap_2.4.59+dfsg.orig.tar.gz 5056324 SHA256:cdeac7531ff072b0cdde29fcc19534d6ac00e9002ecd554d2ff69f897607bf6d
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.59+dfsg-1.debian.tar.xz' openldap_2.4.59+dfsg-1.debian.tar.xz 170320 SHA256:f57e80ab6ecdad5a0a3aed41d1ae9962129d0f3c9e5631ff6c56c2de19d10d60
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.59+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.59+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.59+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:8.7p1-2`

Binary Packages:

- `openssh-client=1:8.7p1-2`

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
$ apt-get source -qq --print-uris openssh=1:8.7p1-2
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.7p1-2.dsc' openssh_8.7p1-2.dsc 3382 SHA256:3fb75e98b98e1154c1d682c5b78e241a1ddd61a819913cc8fcf6a8be2e3bd1e7
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.7p1.orig.tar.gz' openssh_8.7p1.orig.tar.gz 1814595 SHA256:7ca34b8bb24ae9e50f33792b7091b3841d7e1b440ff57bc9fabddf01e2ed1e24
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.7p1.orig.tar.gz.asc' openssh_8.7p1.orig.tar.gz.asc 833 SHA256:bb18c454a3e5d3738cb26a1c89e17c467d7a59529ec92251b26461ae04771eba
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.7p1-2.debian.tar.xz' openssh_8.7p1-2.debian.tar.xz 186492 SHA256:0c35841b4096b6d6bda6b37c9d30f777888e256e90c15fa43f481520280222e1
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:8.7p1-2/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:8.7p1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:8.7p1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.1l-1`

Binary Packages:

- `libssl-dev:amd64=1.1.1l-1`
- `libssl1.1:amd64=1.1.1l-1`
- `openssl=1.1.1l-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1l-1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1l-1.dsc' openssl_1.1.1l-1.dsc 2620 SHA256:ad1ba49cef4a57ddd134368b79d9fc170122f00c9b6956e177ddf06a6dc86ad9
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1l.orig.tar.gz' openssl_1.1.1l.orig.tar.gz 9834044 SHA256:0b7a3e5e59c34827fe0c3a74b7ec8baef302b98fa80088d7f9153aa16fa76bd1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1l.orig.tar.gz.asc' openssl_1.1.1l.orig.tar.gz.asc 488 SHA256:e2ae0ea526223843245dd80224b19a55283f4910dd56b7ee7b23187164f69fda
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1l-1.debian.tar.xz' openssl_1.1.1l-1.debian.tar.xz 84676 SHA256:0738932c86bcca51a17d6a0a840839db192bb8a0e036470fcf6fa4119fb20cd4
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.1l-1/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.1l-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.1l-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.24.0-5`

Binary Packages:

- `libp11-kit0:amd64=0.24.0-5`

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
$ apt-get source -qq --print-uris p11-kit=0.24.0-5
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0-5.dsc' p11-kit_0.24.0-5.dsc 2499 SHA256:8aa9718d4ae9555631391da499605d3b5db29e07282639496bdc77892939f962
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0.orig.tar.xz' p11-kit_0.24.0.orig.tar.xz 834392 SHA256:81e6140584f635e4e956a1b93a32239acf3811ff5b2d3a5c6094e94e99d2c685
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0.orig.tar.xz.asc' p11-kit_0.24.0.orig.tar.xz.asc 833 SHA256:f9996976ae08e48ac652d2aad3f0528a75f87eaa6c17cf076ec00e7ce2fbaeed
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0-5.debian.tar.xz' p11-kit_0.24.0-5.debian.tar.xz 23124 SHA256:2cc526247f78037cd93e2735cdd1d6b43aae73eb9c76f1c02b4a56acae0d5169
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.24.0-5/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.24.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.24.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.4.0-10`

Binary Packages:

- `libpam-modules:amd64=1.4.0-10`
- `libpam-modules-bin=1.4.0-10`
- `libpam-runtime=1.4.0-10`
- `libpam0g:amd64=1.4.0-10`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.4.0-10
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-10.dsc' pam_1.4.0-10.dsc 1913 SHA256:66f226023a80a4524e5c0a8a9f280fa7292ecb8dd4bdeacb2a4e6255f87949b8
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0.orig.tar.xz' pam_1.4.0.orig.tar.xz 988908 SHA256:cd6d928c51e64139be3bdb38692c68183a509b83d4f2c221024ccd4bcddfd034
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-10.debian.tar.xz' pam_1.4.0-10.debian.tar.xz 120896 SHA256:67bc2fba683b98059968b280a3d8f94829fcb625cbc57fdd6ba792c77131d56d
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.4.0-10/ (for browsing the source)
- https://sources.debian.net/src/pam/1.4.0-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.4.0-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pango1.0=1.48.10+ds1-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.48.10+ds1-1`
- `libpangocairo-1.0-0:amd64=1.48.10+ds1-1`
- `libpangoft2-1.0-0:amd64=1.48.10+ds1-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Apache-2.0`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `CC0-1.0 and, CC-BY-SA-3.0,`
- `Chromium-BSD-style`
- `Example`
- `Expat`
- `GPL-3.0`
- `GPL-3.0+`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.48.10+ds1-1
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.48.10+ds1-1.dsc' pango1.0_1.48.10+ds1-1.dsc 3765 SHA256:1ac8a65a0b95998e6865a83a1169fbf0984aace60d0fd9e4a1d84730f270cfac
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.48.10+ds1.orig.tar.xz' pango1.0_1.48.10+ds1.orig.tar.xz 721676 SHA256:a91eccbeca5350c1eb32b06d0de9389f89ac9ec41345abf3ef1198d1ed22a10d
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.48.10+ds1-1.debian.tar.xz' pango1.0_1.48.10+ds1-1.debian.tar.xz 46588 SHA256:541a26b833fdb41f29aa9d2f912f12759eb655534a3d089791e457d26fc33fb2
```

Other potentially useful URLs:

- https://sources.debian.net/src/pango1.0/1.48.10+ds1-1/ (for browsing the source)
- https://sources.debian.net/src/pango1.0/1.48.10+ds1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pango1.0/1.48.10+ds1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `pcre2=10.39-2`

Binary Packages:

- `libpcre2-16-0:amd64=10.39-2`
- `libpcre2-32-0:amd64=10.39-2`
- `libpcre2-8-0:amd64=10.39-2`
- `libpcre2-dev:amd64=10.39-2`
- `libpcre2-posix3:amd64=10.39-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pcre2/10.39-2/


### `dpkg` source package: `pcre3=2:8.39-13`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-13`
- `libpcre3:amd64=2:8.39-13`
- `libpcre3-dev:amd64=2:8.39-13`
- `libpcre32-3:amd64=2:8.39-13`
- `libpcrecpp0v5:amd64=2:8.39-13`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-13
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-13.dsc' pcre3_8.39-13.dsc 2226 SHA256:c3a2eb4f02de5b2e00787ed2a35eb82f04ee4b5e99b8ff279bae3c6453aad93b
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-13.debian.tar.gz' pcre3_8.39-13.debian.tar.gz 27002 SHA256:a2143d7358d69b61955a4f977980050447f8891c0e6737080f2b14b920fbde87
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre3/2:8.39-13/ (for browsing the source)
- https://sources.debian.net/src/pcre3/2:8.39-13/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre3/2:8.39-13/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.32.1-6`

Binary Packages:

- `libperl5.32:amd64=5.32.1-6`
- `perl=5.32.1-6`
- `perl-base=5.32.1-6`
- `perl-modules-5.32=5.32.1-6`

Licenses: (parsed from: `/usr/share/doc/libperl5.32/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.32/copyright`)

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
$ apt-get source -qq --print-uris perl=5.32.1-6
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1-6.dsc' perl_5.32.1-6.dsc 2886 SHA256:dba78a9b8d7c091ec4a435add1cad82108534275bd321a956c12e66a5a9bfe19
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1.orig-regen-configure.tar.gz' perl_5.32.1.orig-regen-configure.tar.gz 871331 SHA256:1d179b41283f12ad83f9758430f6ddc49bdf20db5c396aeae7e51ebb4e4afd29
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1.orig.tar.xz' perl_5.32.1.orig.tar.xz 12610988 SHA256:57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1-6.debian.tar.xz' perl_5.32.1-6.debian.tar.xz 167612 SHA256:d39878f0651b41c8a87aa48daec0b577baa720d6e7f3f14c40fd40fe025bb785
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.32.1-6/ (for browsing the source)
- https://sources.debian.net/src/perl/5.32.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.32.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.1.0-4`

Binary Packages:

- `pinentry-curses=1.1.0-4`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-4
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-4.dsc' pinentry_1.1.0-4.dsc 2216 SHA256:81af8caf54fb2ddc6ac27d768999b3aa5d3bbeec7f2edac839b2c6792a3cf787
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2.asc' pinentry_1.1.0.orig.tar.bz2.asc 488 SHA256:2e9ee3454f9e0be2f6cbc0e289fa5e0620d765e537286ff2c5c28b382f96106a
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-4.debian.tar.xz' pinentry_1.1.0-4.debian.tar.xz 17240 SHA256:b3e36d239219ab35f824c5f9b3dd0c335a4394c59b7628e845831794335b8a8e
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.1.0-4/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.1.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.1.0-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pixman=0.40.0-1`

Binary Packages:

- `libpixman-1-0:amd64=0.40.0-1`
- `libpixman-1-dev:amd64=0.40.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.40.0-1
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.40.0-1.dsc' pixman_0.40.0-1.dsc 2021 SHA256:908752b9c69211606daa8ee92bd929d80ad5f1c4d68f87b98f4fb33e01d4e455
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.40.0.orig.tar.gz' pixman_0.40.0.orig.tar.gz 913976 SHA256:6d200dec3740d9ec4ec8d1180e25779c00bc749f94278c8b9021f5534db223fc
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.40.0-1.diff.gz' pixman_0.40.0-1.diff.gz 319428 SHA256:66a769eee187ce84ff416752f6913ad2ac6165f3bb61696cf1b43bdef48c41ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/pixman/0.40.0-1/ (for browsing the source)
- https://sources.debian.net/src/pixman/0.40.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pixman/0.40.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pkg-config=0.29.2-1`

Binary Packages:

- `pkg-config=0.29.2-1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.2-1
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.2-1.dsc' pkg-config_0.29.2-1.dsc 1771 SHA256:e4feeda94c3882e2aca55eab907900508a2e35111f927a79076154870f8fe373
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.2.orig.tar.gz' pkg-config_0.29.2.orig.tar.gz 2016830 SHA256:6fc69c01688c9458a57eb9a1664c9aba372ccda420a02bf4429fe610e7e7d591
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.2-1.diff.gz' pkg-config_0.29.2-1.diff.gz 9202 SHA256:6ecdd3463718e8922b53fca8d2fd37db4ba178f078b5e3ccd38c1a6efffb94ad
```

Other potentially useful URLs:

- https://sources.debian.net/src/pkg-config/0.29.2-1/ (for browsing the source)
- https://sources.debian.net/src/pkg-config/0.29.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pkg-config/0.29.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `postgresql-14=14.1-1`

Binary Packages:

- `libpq-dev=14.1-1`
- `libpq5:amd64=14.1-1`

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
- `blf`
- `double-metaphone`
- `imath`
- `nagaysau-ishii`
- `rijndael`

Source:

```console
$ apt-get source -qq --print-uris postgresql-14=14.1-1
'http://deb.debian.org/debian/pool/main/p/postgresql-14/postgresql-14_14.1-1.dsc' postgresql-14_14.1-1.dsc 3684 SHA256:d6c1167bbd31d4c02ef0c864d1d302dcec8e1c18fa876c2d4f0476c342fd1439
'http://deb.debian.org/debian/pool/main/p/postgresql-14/postgresql-14_14.1.orig.tar.bz2' postgresql-14_14.1.orig.tar.bz2 21887101 SHA256:4d3c101ea7ae38982f06bdc73758b53727fb6402ecd9382006fa5ecc7c2ca41f
'http://deb.debian.org/debian/pool/main/p/postgresql-14/postgresql-14_14.1-1.debian.tar.xz' postgresql-14_14.1-1.debian.tar.xz 25904 SHA256:5e40b8e428e50a407e0797964fe305921abbe26f99c8691b4b238b38ff0211f3
```

Other potentially useful URLs:

- https://sources.debian.net/src/postgresql-14/14.1-1/ (for browsing the source)
- https://sources.debian.net/src/postgresql-14/14.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/postgresql-14/14.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.17-5`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-5`
- `procps=2:3.3.17-5`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-5
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-5.dsc' procps_3.3.17-5.dsc 2136 SHA256:3b1d9a3d3bc9ec24360ed20721d4235fcd4b4dbb9a86c1eba6c42899a50ecff8
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA256:4518b3e7aafd34ec07d0063d250fd474999b20b200218c3ae56f5d2113f141b4
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-5.debian.tar.xz' procps_3.3.17-5.debian.tar.xz 28608 SHA256:e6b5f9ef22eca9f03f79dc79b4c389249368216df8702a8cc380e10f29eda8c9
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.17-5/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.17-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.17-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.9.7-1`

Binary Packages:

- `libpython3-stdlib:amd64=3.9.7-1`
- `python3=3.9.7-1`
- `python3-minimal=3.9.7-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-defaults/3.9.7-1/


### `dpkg` source package: `python3-stdlib-extensions=3.9.8-1`

Binary Packages:

- `python3-distutils=3.9.8-1`
- `python3-lib2to3=3.9.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-stdlib-extensions/3.9.8-1/


### `dpkg` source package: `python3.9=3.9.9-1`

Binary Packages:

- `libpython3.9-minimal:amd64=3.9.9-1`
- `libpython3.9-stdlib:amd64=3.9.9-1`
- `python3.9=3.9.9-1`
- `python3.9-minimal=3.9.9-1`

Licenses: (parsed from: `/usr/share/doc/libpython3.9-minimal/copyright`, `/usr/share/doc/libpython3.9-stdlib/copyright`, `/usr/share/doc/python3.9/copyright`, `/usr/share/doc/python3.9-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.9=3.9.9-1
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.9-1.dsc' python3.9_3.9.9-1.dsc 3493 SHA256:01090c7278c6c616db52a0b3b61ecac1dbd48b0c3f071f442ed71b90aa1a3985
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.9.orig.tar.xz' python3.9_3.9.9.orig.tar.xz 19144372 SHA256:06828c04a573c073a4e51c4292a27c1be4ae26621c3edc7cf9318418ce3b6d27
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.9-1.debian.tar.xz' python3.9_3.9.9-1.debian.tar.xz 212284 SHA256:bbef753ca15eeee209e2a8d07a21b96ebd554be85ddc8adf458798db9ef6ab26
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.9/3.9.9-1/ (for browsing the source)
- https://sources.debian.net/src/python3.9/3.9.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.9/3.9.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.1-2`

Binary Packages:

- `libreadline-dev:amd64=8.1-2`
- `libreadline8:amd64=8.1-2`
- `readline-common=8.1-2`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1-2
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1-2.dsc' readline_8.1-2.dsc 2418 SHA256:cefa72ab21f0fccab401c49ce559b7e7e4ae45cd1e20c92cba807de64f6169eb
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1.orig.tar.gz' readline_8.1.orig.tar.gz 2993288 SHA256:f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1-2.debian.tar.xz' readline_8.1-2.debian.tar.xz 29800 SHA256:7ff7b7e48727bf8e634cd9721dceb2e4f9e9c2c941664be140ec947267cf26d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/8.1-2/ (for browsing the source)
- https://sources.debian.net/src/readline/8.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/8.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rpcsvc-proto=1.4.2-4`

Binary Packages:

- `rpcsvc-proto=1.4.2-4`

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
$ apt-get source -qq --print-uris rpcsvc-proto=1.4.2-4
'http://deb.debian.org/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-4.dsc' rpcsvc-proto_1.4.2-4.dsc 1977 SHA256:b0d3d6fa0ea3e41fde23b6b38665031f9200bd16371a4718c453d2cc840e27fc
'http://deb.debian.org/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2.orig.tar.xz' rpcsvc-proto_1.4.2.orig.tar.xz 171620 SHA256:678851b9f7ddf4410d2859c12016b65a6dd1a0728d478f18aeb54d165352f17c
'http://deb.debian.org/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-4.debian.tar.xz' rpcsvc-proto_1.4.2-4.debian.tar.xz 4004 SHA256:96b1bc0f1a727c7c11733e3bed86095e78dbcd8b98ab179ffaf2ee4fc556e484
```

Other potentially useful URLs:

- https://sources.debian.net/src/rpcsvc-proto/1.4.2-4/ (for browsing the source)
- https://sources.debian.net/src/rpcsvc-proto/1.4.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rpcsvc-proto/1.4.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2+b2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc 2299 SHA256:a296819cd2ab5880b67ad963ef0867cb10e462f4403e52565aa863eb05bb1370
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz 8096 SHA256:26d47de07d16285e4ca55b0828cbbf1ba35e671f9b3500a87e301fe755d26882
```

Other potentially useful URLs:

- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for browsing the source)
- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.8-1`

Binary Packages:

- `sed=4.8-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.8-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8-1.dsc' sed_4.8-1.dsc 2213 SHA256:f3939fedfca116d7e0efdc2a4088432518a2ea52ffb3a52e14626729781dbf24
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8.orig.tar.xz' sed_4.8.orig.tar.xz 1348048 SHA256:f79b0cfea71b37a8eeec8490db6c5f7ae7719c35587f21edb0617f370eeff633
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8.orig.tar.xz.asc' sed_4.8.orig.tar.xz.asc 833 SHA256:dc256e914030bda14ce4135e655ffcc210e185a9f7de12ed0c4c9f352dc23e08
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8-1.debian.tar.xz' sed_4.8-1.debian.tar.xz 60148 SHA256:a0c09e5dfa8de8544d464d118114dd53c617b11a369e562b6ba8c29899c6c47e
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.8-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sensible-utils=0.0.17`

Binary Packages:

- `sensible-utils=0.0.17`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.17
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.17.dsc' sensible-utils_0.0.17.dsc 1733 SHA256:e4754f4763f77d57fdb29093ec78eb0a84bac4e3aa94e4c251f0d00f11a4b231
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.17.tar.xz' sensible-utils_0.0.17.tar.xz 66648 SHA256:5edf1f6043eeb88957ffe0b0e8793fbbdf40c8ff83f5bf9b36c9421c2d977626
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.17/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.17/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.17/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serf=1.3.9-10`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-10`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-10/


### `dpkg` source package: `shadow=1:4.8.1-2`

Binary Packages:

- `login=1:4.8.1-2`
- `passwd=1:4.8.1-2`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-2
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.8.1-2.dsc' shadow_4.8.1-2.dsc 2218 SHA256:6cca7aecb3faa89684333cc6ae01931a56fdf435f1181734613fb7bb2bab8ce6
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA256:a3ad4630bdc41372f02a647278a8c3514844295d36eefe68ece6c3a641c1ae62
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.8.1-2.debian.tar.xz' shadow_4.8.1-2.debian.tar.xz 74476 SHA256:e230a5fe3945587140dcec2b42dbd0b6bd371bb5976f1b5fb99f5799a2ec4d89
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.8.1-2/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.8.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.8.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shared-mime-info=2.0-1`

Binary Packages:

- `shared-mime-info=2.0-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=2.0-1
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_2.0-1.dsc' shared-mime-info_2.0-1.dsc 2223 SHA256:59f5546a13eff9c7bf8986abf0752f463a4e513a078cc442884629799c6997c0
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_2.0.orig.tar.xz' shared-mime-info_2.0.orig.tar.xz 5015272 SHA256:23c1cb7919f31cf97aeb5225548f75705f706aa5cc7d1c4c503364bcc8681e06
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_2.0-1.debian.tar.xz' shared-mime-info_2.0-1.debian.tar.xz 10612 SHA256:3dcdd64cde8d65907230e4f8ae73734775bef987bae0dbcb86c458d551e6c622
```

Other potentially useful URLs:

- https://sources.debian.net/src/shared-mime-info/2.0-1/ (for browsing the source)
- https://sources.debian.net/src/shared-mime-info/2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shared-mime-info/2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.36.0-2`

Binary Packages:

- `libsqlite3-0:amd64=3.36.0-2`
- `libsqlite3-dev:amd64=3.36.0-2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.36.0-2
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.36.0-2.dsc' sqlite3_3.36.0-2.dsc 2410 SHA256:3135ab1c5ea4f2835f49ebb9a684a1ac15908581f66020bb11a1b8768a2b1263
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.36.0.orig-www.tar.xz' sqlite3_3.36.0.orig-www.tar.xz 6400672 SHA256:d6d67caf958f89a983aa864d49d267a59c98d48ca1988db336a7eb63dd3ed5ec
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.36.0.orig.tar.xz' sqlite3_3.36.0.orig.tar.xz 7554916 SHA256:aef80343f590cbf5f131db152744bc72945130a795db5f36c25ab107f99fb6fa
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.36.0-2.debian.tar.xz' sqlite3_3.36.0-2.debian.tar.xz 22348 SHA256:51dd2e0364d0a6d7c486f479cada6f316d4ac78699fcb0ccfab6514307e07f7a
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.36.0-2/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.36.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.36.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `subversion=1.14.1-3`

Binary Packages:

- `libsvn1:amd64=1.14.1-3+b1`
- `subversion=1.14.1-3+b1`

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
$ apt-get source -qq --print-uris subversion=1.14.1-3
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.1-3.dsc' subversion_1.14.1-3.dsc 3807 SHA256:caf86f3c500a4ffce464fd93aa68ae5ddf2373dda10a5d1a3d2cafe857520bd3
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.1.orig.tar.gz' subversion_1.14.1.orig.tar.gz 11534165 SHA256:dee2796abaa1f5351e6cc2a60b1917beb8238af548b20d3e1ec22760ab2f0cad
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.1.orig.tar.gz.asc' subversion_1.14.1.orig.tar.gz.asc 1288 SHA256:4dafc04642e634f3b75d70d3d707ba8eacc63a4925026402afcb94566f445fa6
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.1-3.debian.tar.xz' subversion_1.14.1-3.debian.tar.xz 430084 SHA256:a309677ab7ca24948e033dcac6c327561ab3cf933547cdeea1d2114b8acbfd5d
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.14.1-3/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.14.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.14.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=249.6-2`

Binary Packages:

- `libsystemd0:amd64=249.6-2`
- `libudev1:amd64=249.6-2`

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
$ apt-get source -qq --print-uris systemd=249.6-2
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_249.6-2.dsc' systemd_249.6-2.dsc 5438 SHA256:32b14da071601e7658e2dc73eb9aeae49efdd333dfcddcb575b843aef32ad750
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_249.6.orig.tar.gz' systemd_249.6.orig.tar.gz 10599611 SHA256:37ec7f7c641935f75f605333c561b7d29894146cc03ae46e6489da3f7dba6016
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_249.6-2.debian.tar.xz' systemd_249.6-2.debian.tar.xz 167036 SHA256:aad30d3b6ce2a88d680b8636a49a5d764b0dadf082fd30ff03f8bf8889553a5d
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/249.6-2/ (for browsing the source)
- https://sources.debian.net/src/systemd/249.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/249.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=3.00-1`

Binary Packages:

- `sysvinit-utils=3.00-1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.00-1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.00-1.dsc' sysvinit_3.00-1.dsc 2376 SHA256:599b9ee804c3ec3db40be1be6d65cc50b98bdaf2f94bda92557bb346058e68f7
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.00.orig.tar.xz' sysvinit_3.00.orig.tar.xz 126544 SHA256:d575f34e91736f019f6e4327f74fadd7cf6f464cdfc8c16a796860b504bd9fd4
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.00-1.debian.tar.xz' sysvinit_3.00-1.debian.tar.xz 129592 SHA256:e79c7d0f7ea0f122f36c4fe2b3726187bfc5a2e9f5f68132fc764790e28cce49
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/3.00-1/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/3.00-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/3.00-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.34+dfsg-1`

Binary Packages:

- `tar=1.34+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34+dfsg-1.dsc' tar_1.34+dfsg-1.dsc 2015 SHA256:12d709cd77e38e5d1753325a9f266b340b5c095a426f438c677b42c031949d89
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34+dfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA256:7d57029540cb928394defb3b377b3531237c947e795b51aa8acac0c5ba0e4844
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34+dfsg-1.debian.tar.xz' tar_1.34+dfsg-1.debian.tar.xz 19192 SHA256:7228f5cbd36f937dfc1fec042dee8b3e02d92a06afdd44c586c2c8cfb1905538
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.34+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/tar/1.34+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.34+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.3.0-2`

Binary Packages:

- `libtiff-dev:amd64=4.3.0-2`
- `libtiff5:amd64=4.3.0-2`
- `libtiffxx5:amd64=4.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.3.0-2
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.3.0-2.dsc' tiff_4.3.0-2.dsc 2429 SHA256:68340f57b5b35407c297b89472e03ea277283754cd1c6c2843399338f494985a
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz' tiff_4.3.0.orig.tar.gz 2808254 SHA256:0e46e5acb087ce7d1ac53cf4f56a09b221537fc86dfc5daaad1c2e89e1b37ac8
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz.asc' tiff_4.3.0.orig.tar.gz.asc 488 SHA256:6e41d0a4c042d2903f28534eb696a16409ccde9aaa2d02d06b5daaabbfb94aa7
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.3.0-2.debian.tar.xz' tiff_4.3.0-2.debian.tar.xz 19596 SHA256:84e02cd055dedd45e87f662ec34097fb1b4c339feb904d5ec6e33aba30b0b995
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.3.0-2/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.3.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.3.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2021e-1`

Binary Packages:

- `tzdata=2021e-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2021e-1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021e-1.dsc' tzdata_2021e-1.dsc 2205 SHA256:6c539a9f0d13aa425a6e4591a20b9bb47d602fafa89e9fbc8137279b90764068
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021e.orig.tar.gz' tzdata_2021e.orig.tar.gz 422509 SHA256:07ec42b737d0d3c6be9c337f8abb5f00554a0f9cc4fcf01a703d69403b6bb2b1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021e.orig.tar.gz.asc' tzdata_2021e.orig.tar.gz.asc 833 SHA256:5bb972b0675203b5d57f3e66e9e7bbc24649c711233ea0077c3ba9a32aec3cd3
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021e-1.debian.tar.xz' tzdata_2021e-1.debian.tar.xz 111832 SHA256:70cc9293783c1b9e4b7f1038d5c67edb4bf0642e780b6a94533529c3ac042aff
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2021e-1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2021e-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2021e-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ucf=3.0043`

Binary Packages:

- `ucf=3.0043`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0043
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0043.dsc' ucf_3.0043.dsc 1423 SHA256:5954508238ff1b8e2c61e1f533268911ba06709e821c02de014fd15d2ead81fd
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0043.tar.xz' ucf_3.0043.tar.xz 70560 SHA256:0294cc11a6cf032ea99ca5064f73a4ede5b28bc2d4ad0a12e8493c7520c7a2a4
```

Other potentially useful URLs:

- https://sources.debian.net/src/ucf/3.0043/ (for browsing the source)
- https://sources.debian.net/src/ucf/3.0043/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ucf/3.0043/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unzip=6.0-26`

Binary Packages:

- `unzip=6.0-26`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-26
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-26.dsc' unzip_6.0-26.dsc 1351 SHA256:403c8373da48b2976144569c1f44d065e6bb4ba874d9637c5497dcc34de618b5
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-26.debian.tar.xz' unzip_6.0-26.debian.tar.xz 23708 SHA256:88cb7c0f1fd13252b662dfd224b64b352f9e75cd86389557fcb23fa6d2638599
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-26/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-26/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-26/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `utf8proc=2.5.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.5.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.5.0-1
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.5.0-1.dsc' utf8proc_2.5.0-1.dsc 2154 SHA256:2137104a3712875650629305fe7d7ef37d4d99328846c18b087b289c0ddbf27c
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.5.0.orig.tar.gz' utf8proc_2.5.0.orig.tar.gz 155485 SHA256:d4e8dfc898cfd062493cb7f42d95d70ccdd3a4cd4d90bec0c71b47cca688f1be
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.5.0-1.debian.tar.xz' utf8proc_2.5.0-1.debian.tar.xz 5240 SHA256:333496cf4e178b5ccf4972fa52523d07a21a0cabf0cb123133c6c71f98e92eff
```

Other potentially useful URLs:

- https://sources.debian.net/src/utf8proc/2.5.0-1/ (for browsing the source)
- https://sources.debian.net/src/utf8proc/2.5.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/utf8proc/2.5.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.37.2-4`

Binary Packages:

- `bsdutils=1:2.37.2-4`
- `libblkid-dev:amd64=2.37.2-4`
- `libblkid1:amd64=2.37.2-4`
- `libmount-dev:amd64=2.37.2-4`
- `libmount1:amd64=2.37.2-4`
- `libsmartcols1:amd64=2.37.2-4`
- `libuuid1:amd64=2.37.2-4`
- `mount=2.37.2-4`
- `util-linux=2.37.2-4`
- `uuid-dev:amd64=2.37.2-4`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.37.2-4
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.2-4.dsc' util-linux_2.37.2-4.dsc 4454 SHA256:a312bd385e6730207c6a96808367714af6bd0b318c09b8b87dd5f02f4ba9e91c
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.2.orig.tar.xz' util-linux_2.37.2.orig.tar.xz 5621624 SHA256:6a0764c1aae7fb607ef8a6dd2c0f6c47d5e5fd27aa08820abaad9ec14e28e9d9
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.2-4.debian.tar.xz' util-linux_2.37.2-4.debian.tar.xz 97648 SHA256:2639bef2d22c57f6e5394e51f892f7d2df39050d663df4864361fbaac3fd5897
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.37.2-4/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.37.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.37.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.21.2-2`

Binary Packages:

- `wget=1.21.2-2+b1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21.2-2
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.2-2.dsc' wget_1.21.2-2.dsc 2167 SHA256:163ced65ad67e242401ff2e0a94350f8865d51cd6b5d3e00b0256396742f13be
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.2.orig.tar.gz' wget_1.21.2.orig.tar.gz 5004576 SHA256:e6d4c76be82c676dd7e8c61a29b2ac8510ae108a810b5d1d18fc9a1d2c9a2497
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.2.orig.tar.gz.asc' wget_1.21.2.orig.tar.gz.asc 833 SHA256:877e0b2580655a0ef71628f3975d2f629f56f5338b169667f97c2742e9970137
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.2-2.debian.tar.xz' wget_1.21.2-2.debian.tar.xz 61048 SHA256:c1eaf8288894ea516db3b0a6f5f733ce5a0f08c8773beac86a17594958fb1323
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.21.2-2/ (for browsing the source)
- https://sources.debian.net/src/wget/1.21.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.21.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x265=3.5-2`

Binary Packages:

- `libx265-199:amd64=3.5-2`

Licenses: (parsed from: `/usr/share/doc/libx265-199/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=3.5-2
'http://deb.debian.org/debian/pool/main/x/x265/x265_3.5-2.dsc' x265_3.5-2.dsc 2234 SHA256:718fea5fdb221871d1d53f74365d429ee9917040586259d32c6fb6183736d87b
'http://deb.debian.org/debian/pool/main/x/x265/x265_3.5.orig.tar.gz' x265_3.5.orig.tar.gz 1537044 SHA256:e70a3335cacacbba0b3a20ec6fecd6783932288ebc8163ad74bcc9606477cae8
'http://deb.debian.org/debian/pool/main/x/x265/x265_3.5-2.debian.tar.xz' x265_3.5-2.debian.tar.xz 13536 SHA256:47a111b9c3e7fd95e4e3e5db43aeb7019a4031820a80badc6dea5c5719de9264
```

Other potentially useful URLs:

- https://sources.debian.net/src/x265/3.5-2/ (for browsing the source)
- https://sources.debian.net/src/x265/3.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x265/3.5-2/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+23.dsc' xorg_7.7+23.dsc 1975 SHA256:b06ef48b56736e0a0a48bcbc1afd2cf6dcd70959c2b52e195456a0392076469c
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+23.tar.gz' xorg_7.7+23.tar.gz 287306 SHA256:8458b8798d7d6098cd5259abc447d6c7a371e20e641cac82cf635296a71f468e
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg/1:7.7+23/ (for browsing the source)
- https://sources.debian.net/src/xorg/1:7.7+23/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg/1:7.7+23/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorgproto=2021.5-1`

Binary Packages:

- `x11proto-dev=2021.5-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2021.5-1
'http://deb.debian.org/debian/pool/main/x/xorgproto/xorgproto_2021.5-1.dsc' xorgproto_2021.5-1.dsc 3157 SHA256:baf6081f2614513ebae99f4d91245aaaad54be83936001086f3d4b9a532d2dd5
'http://deb.debian.org/debian/pool/main/x/xorgproto/xorgproto_2021.5.orig.tar.gz' xorgproto_2021.5.orig.tar.gz 1132811 SHA256:be6ddd6590881452fdfa170c1c9ff87209a98d36155332cbf2ccbc431add86ff
'http://deb.debian.org/debian/pool/main/x/xorgproto/xorgproto_2021.5-1.diff.gz' xorgproto_2021.5-1.diff.gz 22934 SHA256:3a8287632a36d219ca429adc57aee6a791bb4e5c45fb7085cb3c7087bcf67aff
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorgproto/2021.5-1/ (for browsing the source)
- https://sources.debian.net/src/xorgproto/2021.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorgproto/2021.5-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xxhash=0.8.0-2`

Binary Packages:

- `libxxhash0:amd64=0.8.0-2`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.0-2
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.0-2.dsc' xxhash_0.8.0-2.dsc 1601 SHA256:91c696b5371558ebb12c323b0bd4e15eece0a439ef49c6aa5a6d0c1cf6c7762a
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.0.orig.tar.gz' xxhash_0.8.0.orig.tar.gz 145909 SHA256:7054c3ebd169c97b64a92d7b994ab63c70dd53a06974f1f630ab782c28db0f4f
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.0-2.debian.tar.xz' xxhash_0.8.0-2.debian.tar.xz 4160 SHA256:5c427c2c08019a945412afac02326a24c72b65a83bff59447009db303233aecd
```

Other potentially useful URLs:

- https://sources.debian.net/src/xxhash/0.8.0-2/ (for browsing the source)
- https://sources.debian.net/src/xxhash/0.8.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xxhash/0.8.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.5-2`

Binary Packages:

- `liblzma-dev:amd64=5.2.5-2`
- `liblzma5:amd64=5.2.5-2`
- `xz-utils=5.2.5-2`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.dsc' xz-utils_5.2.5-2.dsc 2312 SHA256:fa2706f0c863bee4715460bc9103c6fb73ad2cbc12d8d6d7d5dced81ab349949
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA256:3e1e518ffc912f86608a8cb35e4bd41ad1aec210df2a47aaa1f95e7f5576ef56
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz.asc' xz-utils_5.2.5.orig.tar.xz.asc 833 SHA256:6efc0075a58912e640119d2b52ef7d1518b260d8720fadc73df21ab7fc727624
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.debian.tar.xz' xz-utils_5.2.5-2.debian.tar.xz 33532 SHA256:7bf06a86c35cc6b21a7731df9e11d241f8d3c16b0fe6ed78d64506d1bc29b06e
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.5-2/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.5-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-2.dsc' zlib_1.2.11.dfsg-2.dsc 2397 SHA256:ce8c40737357aeaf17e9ca952a631c9bde4bcfc352c2bbe963836202b12c10a7
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-2.debian.tar.xz' zlib_1.2.11.dfsg-2.debian.tar.xz 19244 SHA256:8602accb97cb92bd52e0d48fa958e67ccad4382a948cca716d5dd24bd0b43bd7
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.11.dfsg-2/ (for access to the source package after it no longer exists in the archive)
