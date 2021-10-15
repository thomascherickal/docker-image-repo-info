# `buildpack-deps:sid-curl`

## Docker Metadata

- Image ID: `sha256:8c7ed886b06be71d7f89507d8ab5487d762ad922aef3dccffc9f98cb80795f99`
- Created: `2021-10-12T15:46:40.44157313Z`
- Virtual Size: ~ 154.86 Mb  
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

### `dpkg` source package: `apt=2.3.9`

Binary Packages:

- `apt=2.3.9`
- `libapt-pkg6.0:amd64=2.3.9`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.3.9
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.3.9.dsc' apt_2.3.9.dsc 2797 SHA256:d7bbed1070148c8dd5b3d3d6f65a1ec6c1acb8ec136d85ebdb011411f3b41b98
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.3.9.tar.xz' apt_2.3.9.tar.xz 2204328 SHA256:28597fe803a652f55f618dd7a44bd2fb2712dbd91c258dfa5981cb75356291e3
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/2.3.9/ (for browsing the source)
- https://sources.debian.net/src/apt/2.3.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/2.3.9/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `bash=5.1-3`

Binary Packages:

- `bash=5.1-3+b2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-3
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-3.dsc' bash_5.1-3.dsc 2296 SHA256:bf92eeca4955f1e9432ca10db63cbff699172cea4ab7bdd6e378f7e2b904f3e0
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA256:d5eeee4f953c09826409d572e2e8996a2140d67eb8f382ce1f3a9d23883ad696
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-3.debian.tar.xz' bash_5.1-3.debian.tar.xz 92188 SHA256:9a2fba0e8391759bb432b6632adbd70b577da2bc5437961c291e13e5ba610b5b
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/5.1-3/ (for browsing the source)
- https://sources.debian.net/src/bash/5.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/5.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2+b2`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

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

- `libbz2-1.0:amd64=1.0.8-4`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

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

### `dpkg` source package: `ca-certificates=20211004`

Binary Packages:

- `ca-certificates=20211004`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20211004
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20211004.dsc' ca-certificates_20211004.dsc 1890 SHA256:ad2ab803a679273acb5f213d3ddd46a1d0c0f95642c6976f53048f558132896b
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20211004.tar.xz' ca-certificates_20211004.tar.xz 239384 SHA256:bc07ae1b555e27591634cd133dd2781f3d3fbc3310e4b5f9ac173ae9c6bed6bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20211004/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20211004/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20211004/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.260`

Binary Packages:

- `libdebconfclient0:amd64=0.260`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.260
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.260.dsc' cdebconf_0.260.dsc 2750 SHA256:0c0a3d76e19685f998e3b85834200255268f36b09eedfa9157fe0213958b7ea5
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.260.tar.xz' cdebconf_0.260.tar.xz 279824 SHA256:ac8a9d7449c76eeaa8ed4ef0bbbf4c16b1b816b9905690c732dea2f341ac079b
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.260/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.260/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.260/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.32-4`

Binary Packages:

- `coreutils=8.32-4+b1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.32-4
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32-4.dsc' coreutils_8.32-4.dsc 2096 SHA256:ea8cafd14b693ec2d8b6e33ee8564c1fa5f102e65574252b0d524aaee04ba7e9
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz' coreutils_8.32.orig.tar.xz 5547836 SHA256:4458d8de7849df44ccab15e16b1548b285224dbba5f08fac070c1c0e0bcc4cfa
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz.asc' coreutils_8.32.orig.tar.xz.asc 833 SHA256:71b944375b322ba77c9c56b687b48df885c676d4fd7c465b3706713a9b62ce0a
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.32-4.debian.tar.xz' coreutils_8.32-4.debian.tar.xz 33028 SHA256:2d5337067b675e0b3fa7c88df164e7738ed4715a39e88e1e82dc9185e4e1b951
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/8.32-4/ (for browsing the source)
- https://sources.debian.net/src/coreutils/8.32-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/8.32-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.74.0-1.3`

Binary Packages:

- `curl=7.74.0-1.3+b1`
- `libcurl4:amd64=7.74.0-1.3+b1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.74.0-1.3
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0-1.3.dsc' curl_7.74.0-1.3.dsc 2435 SHA256:5b2743bad178f7d682ec8067e292ae2e6fb3039d5c6fe94dc1ecbae23fbed9df
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0.orig.tar.gz' curl_7.74.0.orig.tar.gz 4043409 SHA256:e56b3921eeb7a2951959c02db0912b5fcd5fdba5aca071da819e1accf338bbd7
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0-1.3.debian.tar.xz' curl_7.74.0-1.3.debian.tar.xz 36944 SHA256:9013432cb208df97d20c0dfb05c4ba0b93807c17744891a6528d1173eb58d95d
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.74.0-1.3/ (for browsing the source)
- https://sources.debian.net/src/curl/7.74.0-1.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.74.0-1.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2.1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2.1
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.1.dsc' cyrus-sasl2_2.1.27+dfsg-2.1.dsc 3433 SHA256:714b4f59fdf5e3c436b0f10d15535f0048f5164a9a40763f2537fadbd2175da8
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.1.debian.tar.xz 101356 SHA256:0b2cf5e3118a8d99fc39a8133e5508de298b90507fb8c0846d4dae840bf4ec60
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2.1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.11+git20210120+802ebd4-1`

Binary Packages:

- `dash=0.5.11+git20210120+802ebd4-1`

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
$ apt-get source -qq --print-uris dash=0.5.11+git20210120+802ebd4-1
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20210120+802ebd4-1.dsc' dash_0.5.11+git20210120+802ebd4-1.dsc 1646 SHA256:2d08964cf9ad4f59c7ea11f65248b6b95f25265be41214b14464f89b55d4609e
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20210120+802ebd4.orig.tar.xz' dash_0.5.11+git20210120+802ebd4.orig.tar.xz 133332 SHA256:eb30fbd87ea01f0f8b55e34f8fa68745c1134cd756b6bbeba3d3938563912431
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20210120+802ebd4-1.debian.tar.xz' dash_0.5.11+git20210120+802ebd4-1.debian.tar.xz 42504 SHA256:8f5551046677b8ef24aa92d19f6b7ff59f241ec3f6515593307bb69138cb514a
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.11+git20210120+802ebd4-1/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.11+git20210120+802ebd4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.11+git20210120+802ebd4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8`

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

### `dpkg` source package: `debconf=1.5.77`

Binary Packages:

- `debconf=1.5.77`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.77
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.77.dsc' debconf_1.5.77.dsc 2082 SHA256:2797e40ac2122a0ca6c1aa27bd63203e9da4342bb60e614efb848452a5696e41
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.77.tar.xz' debconf_1.5.77.tar.xz 571412 SHA256:03482934c645140dd4cb8cae4970f81f576995b757ac7b89192067e72aa1d067
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.77/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.77/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.77/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `dpkg=1.20.9`

Binary Packages:

- `dpkg=1.20.9`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

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

- `e2fsprogs=1.46.4-1`
- `libcom-err2:amd64=1.46.4-1`
- `libext2fs2:amd64=1.46.4-1`
- `libss2:amd64=1.46.4-1`
- `logsave=1.46.4-1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

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

### `dpkg` source package: `gcc-10=10.3.0-11`

Binary Packages:

- `gcc-10-base:amd64=10.3.0-11`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.3.0-11
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0-11.dsc' gcc-10_10.3.0-11.dsc 22014 SHA256:e872bc018a4601ba4cea4dbab72622cff0f906a63fa8c99dab313d1bc20f29f7
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0.orig.tar.gz' gcc-10_10.3.0.orig.tar.gz 79796443 SHA256:9ace579357cc2e976e4d2576fc1d519b6856495d98ccf11d1a67c5a9b4f79b8c
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0-11.debian.tar.xz' gcc-10_10.3.0-11.debian.tar.xz 788824 SHA256:60da42d65713a2ba999de8a103858bd1f28c423bc4b726086823221ede357b03
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-10/10.3.0-11/ (for browsing the source)
- https://sources.debian.net/src/gcc-10/10.3.0-11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-10/10.3.0-11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-11=11.2.0-8`

Binary Packages:

- `gcc-11-base:amd64=11.2.0-8`
- `libgcc-s1:amd64=11.2.0-8`
- `libstdc++6:amd64=11.2.0-8`

Licenses: (parsed from: `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.2.0-8
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0-8.dsc' gcc-11_11.2.0-8.dsc 27453 SHA256:7f18768fe6b923a2653c4d169eede714608e2fadb8e6cc001cb3163f851aab2f
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0.orig.tar.gz' gcc-11_11.2.0.orig.tar.gz 83874319 SHA256:61bbc68194e52a9149a91571b5e1eb4db520017ed4bcdc021c175a1845605e47
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0-8.debian.tar.xz' gcc-11_11.2.0-8.debian.tar.xz 1817460 SHA256:a24ef7bd791b6945ab38b97e0af8a0bc754a9c354035c7a560a38e2628282a40
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-11/11.2.0-8/ (for browsing the source)
- https://sources.debian.net/src/gcc-11/11.2.0-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-11/11.2.0-8/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `glibc=2.32-4`

Binary Packages:

- `libc-bin=2.32-4`
- `libc6:amd64=2.32-4`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

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

### `dpkg` source package: `gmp=2:6.2.1+dfsg-2`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg-2
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg-2.dsc' gmp_6.2.1+dfsg-2.dsc 2216 SHA256:93c10ac02cf306aec88d5b348bf532478fd444350cd62f379bb98c7f208a519c
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA256:c6ba08e3f079260ab90ff44ab8801eae134cd62cd78f4aa56317c0e70daa40cb
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg-2.debian.tar.xz' gmp_6.2.1+dfsg-2.debian.tar.xz 17824 SHA256:e8fa7b70b13e3d7e48c5ce269b2cebad19dac579829d305ca74f133611d379e1
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg-2/ (for access to the source package after it no longer exists in the archive)

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

- `libgssapi-krb5-2:amd64=1.18.3-7`
- `libk5crypto3:amd64=1.18.3-7`
- `libkrb5-3:amd64=1.18.3-7`
- `libkrb5support0:amd64=1.18.3-7`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

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

### `dpkg` source package: `libffi=3.4.2-2`

Binary Packages:

- `libffi8:amd64=3.4.2-2`

Licenses: (parsed from: `/usr/share/doc/libffi8/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libffi/3.4.2-2/


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

### `dpkg` source package: `libnsl=1.3.0-2`

Binary Packages:

- `libnsl2:amd64=1.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libnsl2/copyright`)

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

### `dpkg` source package: `libselinux=3.1-3`

Binary Packages:

- `libselinux1:amd64=3.1-3`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.1-3
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.1-3.dsc' libselinux_3.1-3.dsc 2300 SHA256:42810484f3776af09a2e0ab726e3be877fc8a54d6bf51702e46c22f945ab5177
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.1.orig.tar.gz' libselinux_3.1.orig.tar.gz 204703 SHA256:ea5dcbb4d859e3f999c26a13c630da2f16dff9462e3cc8cb7b458ac157d112e7
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.1-3.debian.tar.xz' libselinux_3.1-3.debian.tar.xz 24176 SHA256:7170ab6914f0d2e93de169da312df961f799f5d58cc0a4c552e3f8a7882f3c81
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/3.1-3/ (for browsing the source)
- https://sources.debian.net/src/libselinux/3.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/3.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=3.1-1`

Binary Packages:

- `libsemanage-common=3.1-1`
- `libsemanage1:amd64=3.1-1+b2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.1-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.1-1.dsc' libsemanage_3.1-1.dsc 2339 SHA256:d49f9c29d0ad9c8b42145e0926919df962b58823e9fc22002bbb00333276170d
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.1.orig.tar.gz' libsemanage_3.1.orig.tar.gz 179601 SHA256:22d6c75526e40d1781c30bcf29abf97171bdfe6780923f11c8e1c76a75a21ff8
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.1-1.debian.tar.xz' libsemanage_3.1-1.debian.tar.xz 17556 SHA256:185b151158faaaf3d8f9ff939f29efd3eb5dbb050d01a87d3fde6cf40e778648
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/3.1-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=3.1-1`

Binary Packages:

- `libsepol1:amd64=3.1-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.1-1
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.1-1.dsc' libsepol_3.1-1.dsc 1776 SHA256:37bfb6797af8a96eada6c6ace374292b8a16a6bfb557b1e8ab9fd29e72d5888a
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA256:ae6778d01443fdd38cd30eeee846494e19f4d407b09872580372f4aa4bf8a3cc
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.1-1.debian.tar.xz' libsepol_3.1-1.debian.tar.xz 14584 SHA256:9351a0b6207f6a5da2951292d3ec5655feb89df5aabc9010094766d811156166
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/3.1-1/ (for browsing the source)
- https://sources.debian.net/src/libsepol/3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/3.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libtasn1-6=4.17.0-2`

Binary Packages:

- `libtasn1-6:amd64=4.17.0-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.17.0-2
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.17.0-2.dsc' libtasn1-6_4.17.0-2.dsc 2586 SHA256:3094abb781ad3146d60c068fc5181d317001a0ab47dd4ff7edb0bf7f531c8f14
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.17.0.orig.tar.gz' libtasn1-6_4.17.0.orig.tar.gz 1906654 SHA256:ece7551cea7922b8e10d7ebc70bc2248d1fdd73351646a2d6a8d68a9421c45a5
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.17.0.orig.tar.gz.asc' libtasn1-6_4.17.0.orig.tar.gz.asc 488 SHA256:bacbaa3ffe63df9a876b65246668968e3580032f69fbac4b0a2044831855b69a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.17.0-2.debian.tar.xz' libtasn1-6_4.17.0-2.debian.tar.xz 20168 SHA256:29419f61d6f15bdea299e6ad12f9d408337e865828d362ca475f52e2fc5651df
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.17.0-2/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.17.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.17.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtirpc=1.3.2-2`

Binary Packages:

- `libtirpc-common=1.3.2-2`
- `libtirpc3:amd64=1.3.2-2`

Licenses: (parsed from: `/usr/share/doc/libtirpc-common/copyright`, `/usr/share/doc/libtirpc3/copyright`)

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

### `dpkg` source package: `libxcrypt=1:4.4.25-2`

Binary Packages:

- `libcrypt1:amd64=1:4.4.25-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.25-2
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.25-2.dsc' libxcrypt_4.4.25-2.dsc 1525 SHA256:8160446ad08ca293986c62d8c06bc1515787ef3fb25d7a4344d2c3cf224110b9
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.25.orig.tar.xz' libxcrypt_4.4.25.orig.tar.xz 390024 SHA256:82af8b3b39c30ff81ef59cbe9f515b7ad1a9a34997c6c66ac8aa9c48deebff59
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.25-2.debian.tar.xz' libxcrypt_4.4.25-2.debian.tar.xz 7728 SHA256:8c9306712fc7d4f368487685c8cba3e3fd9fab89d5515e0e006d480abc72c740
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.25-2/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.25-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.25-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ncurses=6.2+20210905-1`

Binary Packages:

- `libncursesw6:amd64=6.2+20210905-1`
- `libtinfo6:amd64=6.2+20210905-1`
- `ncurses-base=6.2+20210905-1`
- `ncurses-bin=6.2+20210905-1`

Licenses: (parsed from: `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

### `dpkg` source package: `openssl=1.1.1l-1`

Binary Packages:

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

### `dpkg` source package: `pcre2=10.36-2`

Binary Packages:

- `libpcre2-8-0:amd64=10.36-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.36-2
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.36-2.dsc' pcre2_10.36-2.dsc 2286 SHA256:317f27fd2c578c87b3753a267da2290dc6970c16c81f1f1761694c977a4be4f5
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.36.orig.tar.gz' pcre2_10.36.orig.tar.gz 2290719 SHA256:b95ddb9414f91a967a887d69617059fb672b914f56fa3d613812c1ee8e8a1a37
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.36-2.diff.gz' pcre2_10.36-2.diff.gz 6799 SHA256:9a39c9972fac99b020b900bcba16cb18a5ef8d0c8ac7a6df1060193b9fa6ba83
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.36-2/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.36-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.36-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.39-13`

Binary Packages:

- `libpcre3:amd64=2:8.39-13`

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

- `perl-base=5.32.1-6`

Licenses: (parsed from: `/usr/share/doc/perl-base/copyright`)

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

### `dpkg` source package: `readline=8.1-2`

Binary Packages:

- `libreadline8:amd64=8.1-2`
- `readline-common=8.1-2`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

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

### `dpkg` source package: `shadow=1:4.8.1-1`

Binary Packages:

- `login=1:4.8.1-1`
- `passwd=1:4.8.1-1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.8.1-1.dsc' shadow_4.8.1-1.dsc 2215 SHA256:5c9568dc183781ba654b7daeba6d5d6768d4e0417cc8d8b6f2e534dae6fcdaa6
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA256:a3ad4630bdc41372f02a647278a8c3514844295d36eefe68ece6c3a641c1ae62
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.8.1-1.debian.tar.xz' shadow_4.8.1-1.debian.tar.xz 74752 SHA256:fdbccadc28fcca744f365e0529f3828d0c82bc3513b28976dca7308b40ea4773
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.8.1-1/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.8.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.8.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.36.0-2`

Binary Packages:

- `libsqlite3-0:amd64=3.36.0-2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

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

### `dpkg` source package: `systemd=247.9-4`

Binary Packages:

- `libsystemd0:amd64=247.9-4`
- `libudev1:amd64=247.9-4`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2 with Linux-syscall-note exception`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/systemd/247.9-4/


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

### `dpkg` source package: `tzdata=2021c-2`

Binary Packages:

- `tzdata=2021c-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2021c-2
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021c-2.dsc' tzdata_2021c-2.dsc 2205 SHA256:49567fde17c5438a00232c3ec9d87d765f9b51909555f54d8baefa8551575d4f
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021c.orig.tar.gz' tzdata_2021c.orig.tar.gz 421791 SHA256:b4f1d1c8cb11c3500276dac862d8c7e6f88c69b1e8ee4c5e9d1daad17fbe3542
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021c.orig.tar.gz.asc' tzdata_2021c.orig.tar.gz.asc 833 SHA256:1bcfa0f79ef685cdb5049d80eac6c7afd60768f6169a580ad2d48f6bd7838b7f
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021c-2.debian.tar.xz' tzdata_2021c-2.debian.tar.xz 106292 SHA256:7b9e23696471397ccf1da2e58869a85be7bf0d32cf46e6ebe6dcfcd2dc2e5a3b
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2021c-2/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2021c-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2021c-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.37.2-3`

Binary Packages:

- `bsdutils=1:2.37.2-3`
- `libblkid1:amd64=2.37.2-3`
- `libmount1:amd64=2.37.2-3`
- `libsmartcols1:amd64=2.37.2-3`
- `libuuid1:amd64=2.37.2-3`
- `mount=2.37.2-3`
- `util-linux=2.37.2-3`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.37.2-3
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.2-3.dsc' util-linux_2.37.2-3.dsc 4453 SHA256:ce3d6fc1d2fa2329c4dfbb69b87454a450834554032905eb776acf6a5c6e8273
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.2.orig.tar.xz' util-linux_2.37.2.orig.tar.xz 5621624 SHA256:6a0764c1aae7fb607ef8a6dd2c0f6c47d5e5fd27aa08820abaad9ec14e28e9d9
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.2-3.debian.tar.xz' util-linux_2.37.2-3.debian.tar.xz 96948 SHA256:b6ba987cdf3177963fe3e256b872e13165af8d70131334042cdc003e19cb609e
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.37.2-3/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.37.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.37.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.21.2-1`

Binary Packages:

- `wget=1.21.2-1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/wget/1.21.2-1/


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

- `liblzma5:amd64=5.2.5-2`

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

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

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
