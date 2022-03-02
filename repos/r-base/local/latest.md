# `r-base:4.1.2`

## Docker Metadata

- Image ID: `sha256:4b361dfebd4fbd65e91e96956dcb1954f79b587c6b2a781b2c2cb8cc27bf9eca`
- Created: `2022-01-26T22:40:13.048249298Z`
- Virtual Size: ~ 766.85 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["R"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LC_ALL=en_US.UTF-8`
  - `LANG=en_US.UTF-8`
  - `R_BASE_VERSION=4.1.2`
- Labels:
  - `org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>`
  - `org.opencontainers.image.licenses=GPL-2.0-or-later`
  - `org.opencontainers.image.source=https://github.com/rocker-org/rocker`
  - `org.opencontainers.image.vendor=Rocker Project`

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

### `dpkg` source package: `apt=2.3.14`

Binary Packages:

- `apt=2.3.14`
- `libapt-pkg6.0:amd64=2.3.14`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.3.14/


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
- `libaudit1:amd64=1:3.0.6-1+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/audit/1:3.0.6-1/


### `dpkg` source package: `base-files=12`

Binary Packages:

- `base-files=12`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-files/12/


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

### `dpkg` source package: `bash=5.1-6`

Binary Packages:

- `bash=5.1-6`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-6
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-6.dsc' bash_5.1-6.dsc 2292 SHA256:f1a717dd6f67c39b5b72af43fd62d23e2e492019c701068c7f8eb0e06033ec23
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA256:d5eeee4f953c09826409d572e2e8996a2140d67eb8f382ce1f3a9d23883ad696
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-6.debian.tar.xz' bash_5.1-6.debian.tar.xz 93524 SHA256:929c7ff828d449f17f7cbe76a34634c62722b899d5429488704a393a534a0ae6
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/5.1-6/ (for browsing the source)
- https://sources.debian.net/src/bash/5.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/5.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `binutils=2.37.50.20220106-2`

Binary Packages:

- `binutils=2.37.50.20220106-2`
- `binutils-common:amd64=2.37.50.20220106-2`
- `binutils-x86-64-linux-gnu=2.37.50.20220106-2`
- `libbinutils:amd64=2.37.50.20220106-2`
- `libctf-nobfd0:amd64=2.37.50.20220106-2`
- `libctf0:amd64=2.37.50.20220106-2`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.37.50.20220106-2
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.37.50.20220106-2.dsc' binutils_2.37.50.20220106-2.dsc 11360 SHA256:0e1ad493b14eae31b08e50d76378f8561ef6f856c86e7b629c28c1580afa9f42
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.37.50.20220106.orig.tar.xz' binutils_2.37.50.20220106.orig.tar.xz 22410088 SHA256:64a6d71bdecca17be54452f5a901fcc90e55b4723a99978665bc63befc38b08f
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.37.50.20220106-2.debian.tar.xz' binutils_2.37.50.20220106-2.debian.tar.xz 181928 SHA256:0f14a550ce46c6e477ba728e94848cd3354da2a8743c0879ad6006b13b6012fd
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.37.50.20220106-2/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.37.50.20220106-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.37.50.20220106-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `boot=1.3-28-2`

Binary Packages:

- `r-cran-boot=1.3-28-2`

Licenses: (parsed from: `/usr/share/doc/r-cran-boot/copyright`)

- `'unlimited distribution'`

Source:

```console
$ apt-get source -qq --print-uris boot=1.3-28-2
'http://deb.debian.org/debian/pool/main/b/boot/boot_1.3-28-2.dsc' boot_1.3-28-2.dsc 1802 SHA256:ceeb6723addbf4de10f640d6b0c0abcab3b9d069239cac15e97e45d05a8f16d4
'http://deb.debian.org/debian/pool/main/b/boot/boot_1.3-28.orig.tar.gz' boot_1.3-28.orig.tar.gz 236842 SHA256:9f7158fd2714659f590c3955651893dc24bd8f39196bc5a4cc35b0b031744a32
'http://deb.debian.org/debian/pool/main/b/boot/boot_1.3-28-2.debian.tar.xz' boot_1.3-28-2.debian.tar.xz 5316 SHA256:ec34c243ea04a6cf650076aa922a3af6aa55efb287550d21540828b4911ac23f
```

Other potentially useful URLs:

- https://sources.debian.net/src/boot/1.3-28-2/ (for browsing the source)
- https://sources.debian.net/src/boot/1.3-28-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/boot/1.3-28-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2+b3`

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

### `dpkg` source package: `build-essential=12.9`

Binary Packages:

- `build-essential=12.9`

Licenses: (parsed from: `/usr/share/doc/build-essential/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris build-essential=12.9
'http://deb.debian.org/debian/pool/main/b/build-essential/build-essential_12.9.dsc' build-essential_12.9.dsc 2220 SHA256:1e4ad67c69001a162b2eb3a2019f037e53c8a1e312073ba1a2110d1e21971555
'http://deb.debian.org/debian/pool/main/b/build-essential/build-essential_12.9.tar.xz' build-essential_12.9.tar.xz 51532 SHA256:938da370b4ef883687d141723d1b7470ad76bec7a54158d3d6b9b38f9c9eedb2
```

Other potentially useful URLs:

- https://sources.debian.net/src/build-essential/12.9/ (for browsing the source)
- https://sources.debian.net/src/build-essential/12.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/build-essential/12.9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `bzip2=1.0.8-5`
- `libbz2-1.0:amd64=1.0.8-5`
- `libbz2-dev:amd64=1.0.8-5`

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

### `dpkg` source package: `ca-certificates=20210119`

Binary Packages:

- `ca-certificates=20210119`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20210119
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20210119.dsc' ca-certificates_20210119.dsc 1868 SHA256:51e5c099ab976f50f4d2f3c5ea0ad49853024cdb3e630322cbd7e02b05a034f4
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20210119.tar.xz' ca-certificates_20210119.tar.xz 232964 SHA256:daa3afae563711c30a0586ddae4336e8e3974c2b627faaca404c4e0141b64665
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20210119/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20210119/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20210119/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cairo=1.16.0-5`

Binary Packages:

- `libcairo2:amd64=1.16.0-5`

Licenses: (parsed from: `/usr/share/doc/libcairo2/copyright`)

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

### `dpkg` source package: `cluster=2.1.2-2`

Binary Packages:

- `r-cran-cluster=2.1.2-2`

Licenses: (parsed from: `/usr/share/doc/r-cran-cluster/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cluster=2.1.2-2
'http://deb.debian.org/debian/pool/main/c/cluster/cluster_2.1.2-2.dsc' cluster_2.1.2-2.dsc 1831 SHA256:d7c13326fcd08c506c944e046c4784a8fdbcaff5fe097914286cc248aa84d156
'http://deb.debian.org/debian/pool/main/c/cluster/cluster_2.1.2.orig.tar.gz' cluster_2.1.2.orig.tar.gz 402667 SHA256:5c8aa760fb6dda4fcfe6196e561ffcd2dc12b1a6c7659cb90be2cde747311499
'http://deb.debian.org/debian/pool/main/c/cluster/cluster_2.1.2-2.debian.tar.xz' cluster_2.1.2-2.debian.tar.xz 4300 SHA256:9a38fe971e18d9ea3589cb5e89f4e120b4f3b0f2a9a8fc3559cd2b71fc80ce62
```

Other potentially useful URLs:

- https://sources.debian.net/src/cluster/2.1.2-2/ (for browsing the source)
- https://sources.debian.net/src/cluster/2.1.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cluster/2.1.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `codetools=0.2-18-1`

Binary Packages:

- `r-cran-codetools=0.2-18-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-codetools/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris codetools=0.2-18-1
'http://deb.debian.org/debian/pool/main/c/codetools/codetools_0.2-18-1.dsc' codetools_0.2-18-1.dsc 1859 SHA256:c5dbbfdad52751ac6af3af2fa3a3dbb3267f136e024289a2102addc41b3e1ecf
'http://deb.debian.org/debian/pool/main/c/codetools/codetools_0.2-18.orig.tar.gz' codetools_0.2-18.orig.tar.gz 38175 SHA256:1a9ea6b9792dbd1688078455929385acc3a5e4bef945c77bec1261fa4a084c28
'http://deb.debian.org/debian/pool/main/c/codetools/codetools_0.2-18-1.debian.tar.xz' codetools_0.2-18-1.debian.tar.xz 2868 SHA256:be07b14194de74900cbcc6a7fb67f52be0be88a103cf4f71682997ebfb576718
```

Other potentially useful URLs:

- https://sources.debian.net/src/codetools/0.2-18-1/ (for browsing the source)
- https://sources.debian.net/src/codetools/0.2-18-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/codetools/0.2-18-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `curl=7.81.0-1`

Binary Packages:

- `libcurl4:amd64=7.81.0-1`

Licenses: (parsed from: `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.81.0-1
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.81.0-1.dsc' curl_7.81.0-1.dsc 3024 SHA256:11ad80d0f83a1ded31dc43c0bc5e3cb64edeb34798e9dbf23706d7c4f12d71fc
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.81.0.orig.tar.gz' curl_7.81.0.orig.tar.gz 4188040 SHA256:ac8e1087711084548d788ef18b9b732c8de887457b81f616fc681d1044b32f98
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.81.0.orig.tar.gz.asc' curl_7.81.0.orig.tar.gz.asc 488 SHA256:e0f0053bef0afd5c8bed7973f94f92a731c91b9152d64ce9c55fd3bb633aa735
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.81.0-1.debian.tar.xz' curl_7.81.0-1.debian.tar.xz 36364 SHA256:21178fef36132b3284b21e04e208cf67a1bfbaee2c59204cc037c79764e8b773
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.81.0-1/ (for browsing the source)
- https://sources.debian.net/src/curl/7.81.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.81.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg2-3`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg2-3`
- `libsasl2-modules-db:amd64=2.1.27+dfsg2-3`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-2.2-clause`
- `BSD-3-clause`
- `BSD-3-clause-JANET`
- `BSD-3-clause-PADL`
- `BSD-4-clause`
- `BSD-4-clause-UC`
- `FSFULLR`
- `GPL-3`
- `GPL-3+`
- `IBM-as-is`
- `MIT-CMU`
- `MIT-Export`
- `MIT-OpenVision`
- `OpenLDAP`
- `OpenSSL`
- `RSA-MD`
- `SSLeay`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg2-3
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg2-3.dsc' cyrus-sasl2_2.1.27+dfsg2-3.dsc 3260 SHA256:61732a1f7b6fd0dff2878edc9304ae97406fbdb0b514a01a8dc45222fb82d7a2
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg2.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg2.orig.tar.xz 829892 SHA256:f3d90671718e7dc1d46db7ccbad548d60ffe1edd1e9a620e5d3b779e6a0a9326
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg2-3.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg2-3.debian.tar.xz 92560 SHA256:532313c78b38b7952adf9693ebd2cf6e8e70f247333fdf2729e099427e427a00
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg2-3/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg2-3/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-3.dsc' dash_0.5.11+git20210903+057cd650a4ed-3.dsc 1686 SHA256:c73521b15349e1271ea4c123eecd0686eb47c98cb8f7f0089fc008194269d612
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed.orig.tar.xz' dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz 133320 SHA256:4fb06697f33f14fcd6b96cd4dfdd5b343c848a4bb69b7c04f1717767e4a117d3
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-3.debian.tar.xz' dash_0.5.11+git20210903+057cd650a4ed-3.debian.tar.xz 42656 SHA256:3f0cd26fce95a29e2e0a1e01268d97fb5429625b7f984e41cc3f05a6704841e1
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.11+git20210903+057cd650a4ed-3/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.11+git20210903+057cd650a4ed-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.11+git20210903+057cd650a4ed-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.8
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.8.dsc' db5.3_5.3.28+dfsg1-0.8.dsc 3113 SHA256:5189bebd157e3b51c075804d1affebc87cdbfb782808c621e131660719c24374
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.8.debian.tar.xz' db5.3_5.3.28+dfsg1-0.8.debian.tar.xz 30748 SHA256:073c0c87283bf5e606f3ce6d1814315b40b9685c943601ae3fd81e2da4e612d4
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

### `dpkg` source package: `debianutils=4.11.2`

Binary Packages:

- `debianutils=4.11.2`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debianutils/4.11.2/


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

### `dpkg` source package: `dpkg=1.21.1`

Binary Packages:

- `dpkg=1.21.1`
- `dpkg-dev=1.21.1`
- `libdpkg-perl=1.21.1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.1
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.1.dsc' dpkg_1.21.1.dsc 2120 SHA256:4a18d3c84a982a5510ee96d490b3ff9c103e1086f165051e7e9d3b1801e1950b
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.1.tar.xz' dpkg_1.21.1.tar.xz 4986936 SHA256:1eb9fd5228b3199284ea5134904bb45b7a5bc12fb044b8e4964d89d2e5bbb563
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.21.1/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.21.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.21.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.46.5-2`

Binary Packages:

- `e2fsprogs=1.46.5-2`
- `libcom-err2:amd64=1.46.5-2`
- `libext2fs2:amd64=1.46.5-2`
- `libss2:amd64=1.46.5-2`
- `logsave=1.46.5-2`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.5-2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.5-2.dsc' e2fsprogs_1.46.5-2.dsc 2846 SHA256:6be9066b5b608aeb053e9c25bfd69c11123d8a945d191ff12657e73efb3480c3
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.5.orig.tar.gz' e2fsprogs_1.46.5.orig.tar.gz 9530158 SHA256:b7430d1e6b7b5817ce8e36d7c8c7c3249b3051d0808a96ffd6e5c398e4e2fbb9
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.5.orig.tar.gz.asc' e2fsprogs_1.46.5.orig.tar.gz.asc 488 SHA256:b1e248ed73d4d67ac0cf7760e780e0a5cd2db85bbb9a5dcc235538b596128916
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.5-2.debian.tar.xz' e2fsprogs_1.46.5-2.debian.tar.xz 83972 SHA256:0d635367a58eead808e5c780003a63d00fd37aaa20a3270d5f2ec796fe3f22ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.46.5-2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.46.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.46.5-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ed=1.17-1`

Binary Packages:

- `ed=1.17-1`

Licenses: (parsed from: `/usr/share/doc/ed/copyright`)

- `BSD-2-Clause`
- `FCONF`
- `FDOC`
- `FLOG`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ed/1.17-1/


### `dpkg` source package: `expat=2.4.3-1`

Binary Packages:

- `libexpat1:amd64=2.4.3-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/expat/2.4.3-1/


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
- `libfontconfig1:amd64=2.13.1-4.2`

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

### `dpkg` source package: `foreign=0.8.82-1`

Binary Packages:

- `r-cran-foreign=0.8.82-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-foreign/copyright`)

- `GPL`
- `GPL `

Source:

```console
$ apt-get source -qq --print-uris foreign=0.8.82-1
'http://deb.debian.org/debian/pool/main/f/foreign/foreign_0.8.82-1.dsc' foreign_0.8.82-1.dsc 1838 SHA256:2722081f98a59fb4dd40e052ca17dcf7408d1a904ffaf10f1132c5489502dd22
'http://deb.debian.org/debian/pool/main/f/foreign/foreign_0.8.82.orig.tar.gz' foreign_0.8.82.orig.tar.gz 361598 SHA256:f8ed0684d59bec7f3a39cde1aa5ec7b3e6e36aaecacb28120c9c54f7b13f80fb
'http://deb.debian.org/debian/pool/main/f/foreign/foreign_0.8.82-1.debian.tar.xz' foreign_0.8.82-1.debian.tar.xz 4288 SHA256:c91ca94f537050502a95f023d6ae00b762a4495f2584018a9c071876f82336c7
```

Other potentially useful URLs:

- https://sources.debian.net/src/foreign/0.8.82-1/ (for browsing the source)
- https://sources.debian.net/src/foreign/0.8.82-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/foreign/0.8.82-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `freetype=2.11.1+dfsg-1`

Binary Packages:

- `libfreetype6:amd64=2.11.1+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

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
$ apt-get source -qq --print-uris freetype=2.11.1+dfsg-1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.1%2bdfsg-1.dsc' freetype_2.11.1+dfsg-1.dsc 3713 SHA256:e293bdd821cd52b9be28d66bb2ffff61600d5ed45fc645450f5414354091c76c
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2demos.tar.xz' freetype_2.11.1+dfsg.orig-ft2demos.tar.xz 257240 SHA256:c60620d49d0f16d95586eb868c01b129569409e6cfdcb87a78e0482a12604672
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.11.1+dfsg.orig-ft2demos.tar.xz.asc 195 SHA256:d911a95830c50efcf60398e51db4ec307bbf4d24168377b515aded0611e977c0
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2docs.tar.xz' freetype_2.11.1+dfsg.orig-ft2docs.tar.xz 2038348 SHA256:755e29908093c19138a38775784b0accf7e838ffa28a25b8722b3dfe651d80fa
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.11.1+dfsg.orig-ft2docs.tar.xz.asc 195 SHA256:67cbc2f192460dc4d46129e7debe55b40a9fa6e224ffeed70b4cf397ebaccab5
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig.tar.xz' freetype_2.11.1+dfsg.orig.tar.xz 1988020 SHA256:ef93541237834445eb7ff355e7d4139d48844f9c977a485dea1316df54994473
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.11.1%2bdfsg-1.debian.tar.xz' freetype_2.11.1+dfsg-1.debian.tar.xz 40132 SHA256:fe505af845e1414dee38c42cd266508924ac795a21678e9f71dfc205fcef83ae
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.11.1+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.11.1+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.11.1+dfsg-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gcc-10=10.3.0-14`

Binary Packages:

- `gcc-10-base:amd64=10.3.0-14`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.3.0-14
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0-14.dsc' gcc-10_10.3.0-14.dsc 21839 SHA256:a25a3c3104918823820ad68f928ebd80a442015f822dfe64e095e4c4f23340d4
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0.orig.tar.gz' gcc-10_10.3.0.orig.tar.gz 79796443 SHA256:9ace579357cc2e976e4d2576fc1d519b6856495d98ccf11d1a67c5a9b4f79b8c
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.3.0-14.debian.tar.xz' gcc-10_10.3.0-14.debian.tar.xz 843552 SHA256:e00120c8e141f51fe5d42647f8a00a63612274fcf48fdc85f1f43a8632d2c3d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-10/10.3.0-14/ (for browsing the source)
- https://sources.debian.net/src/gcc-10/10.3.0-14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-10/10.3.0-14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-11=11.2.0-14`

Binary Packages:

- `cpp-11=11.2.0-14`
- `g++-11=11.2.0-14`
- `gcc-11=11.2.0-14`
- `gcc-11-base:amd64=11.2.0-14`
- `gfortran-11=11.2.0-14`
- `libasan6:amd64=11.2.0-14`
- `libatomic1:amd64=11.2.0-14`
- `libcc1-0:amd64=11.2.0-14`
- `libgcc-11-dev:amd64=11.2.0-14`
- `libgcc-s1:amd64=11.2.0-14`
- `libgfortran-11-dev:amd64=11.2.0-14`
- `libgfortran5:amd64=11.2.0-14`
- `libgomp1:amd64=11.2.0-14`
- `libitm1:amd64=11.2.0-14`
- `liblsan0:amd64=11.2.0-14`
- `libquadmath0:amd64=11.2.0-14`
- `libstdc++-11-dev:amd64=11.2.0-14`
- `libstdc++6:amd64=11.2.0-14`
- `libtsan0:amd64=11.2.0-14`
- `libubsan1:amd64=11.2.0-14`

Licenses: (parsed from: `/usr/share/doc/cpp-11/copyright`, `/usr/share/doc/g++-11/copyright`, `/usr/share/doc/gcc-11/copyright`, `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/gfortran-11/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-11-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgfortran-11-dev/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-11-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.2.0-14
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0-14.dsc' gcc-11_11.2.0-14.dsc 27514 SHA256:7d479aee3d13e327c332f312794877617113096676c1e85ca2ee81adcf6714c7
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0.orig.tar.gz' gcc-11_11.2.0.orig.tar.gz 83874319 SHA256:61bbc68194e52a9149a91571b5e1eb4db520017ed4bcdc021c175a1845605e47
'http://deb.debian.org/debian/pool/main/g/gcc-11/gcc-11_11.2.0-14.debian.tar.xz' gcc-11_11.2.0-14.debian.tar.xz 2005360 SHA256:fc05ab9385538ec4d83d5c161efbfe27cfe0e5c136289555c2a31fd85e2153cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-11/11.2.0-14/ (for browsing the source)
- https://sources.debian.net/src/gcc-11/11.2.0-14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-11/11.2.0-14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-defaults=1.194`

Binary Packages:

- `cpp=4:11.2.0-2`
- `g++=4:11.2.0-2`
- `gcc=4:11.2.0-2`
- `gfortran=4:11.2.0-2`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`, `/usr/share/doc/gfortran/copyright`)

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
- `libgdbm6:amd64=1.22-1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gdbm/1.22-1/


### `dpkg` source package: `glib2.0=2.70.2-1`

Binary Packages:

- `libglib2.0-0:amd64=2.70.2-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.70.2-1
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.70.2-1.dsc' glib2.0_2.70.2-1.dsc 3408 SHA256:d7add74ff133aa5b93831477a213c5dbcae38503178db83752d11723f3619c90
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.70.2.orig.tar.xz' glib2.0_2.70.2.orig.tar.xz 4822356 SHA256:0551459c85cd3da3d58ddc9016fd28be5af503f5e1615a71ba5b512ac945806f
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.70.2-1.debian.tar.xz' glib2.0_2.70.2-1.debian.tar.xz 102352 SHA256:0ad5684ab508474f4209849ac2079c47cddfe16d2f00e45d007b2774fe056489
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.70.2-1/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.70.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.70.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.33-3`

Binary Packages:

- `libc-bin=2.33-3`
- `libc-dev-bin=2.33-3`
- `libc-l10n=2.33-3`
- `libc6:amd64=2.33-3`
- `libc6-dev:amd64=2.33-3`
- `locales=2.33-3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc-l10n/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/locales/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.33-3
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.33-3.dsc' glibc_2.33-3.dsc 9631 SHA256:5f2f07b974f79975369ea77a7dd5dddb5d85b6fec5e390da5c295529932c16c5
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.33.orig.tar.xz' glibc_2.33.orig.tar.xz 17643172 SHA256:5bd6d6b7fb0350308aa7abd067e081d57ba6ac1e0372ed372d197bccb86e5c14
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.33-3.debian.tar.xz' glibc_2.33-3.debian.tar.xz 815404 SHA256:4b184b55337cec4786c15c162314d05421a5b734089ad5dd54a34d49e37a81ff
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.33-3/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.33-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.33-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.1+dfsg-3`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg-3
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg-3.dsc' gmp_6.2.1+dfsg-3.dsc 2223 SHA256:b91dae1d6298e5ff75dee503c7f8128e822000e343e0a5b5d5146cc1713334bb
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA256:c6ba08e3f079260ab90ff44ab8801eae134cd62cd78f4aa56317c0e70daa40cb
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg-3.debian.tar.xz' gmp_6.2.1+dfsg-3.debian.tar.xz 18356 SHA256:32d75d4e7a383a5cea701aff4a4bf609933c4d15d1f5e3b6168eed51857bc8f0
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.27-3`

Binary Packages:

- `gpgv=2.2.27-3`

Licenses: (parsed from: `/usr/share/doc/gpgv/copyright`)

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
$ apt-get source -qq --print-uris gnupg2=2.2.27-3
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-3.dsc' gnupg2_2.2.27-3.dsc 3630 SHA256:c3fcf3c8f0aad05bb86f7bdcd67bdc9dd67cb35b0605778de3ee5b07ba621934
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2' gnupg2_2.2.27.orig.tar.bz2 7191555 SHA256:34e60009014ea16402069136e0a5f63d9b65f90096244975db5cea74b3d02399
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-3.debian.tar.xz' gnupg2_2.2.27-3.debian.tar.xz 63396 SHA256:ef72e1094b7c47c9394d1d46bfda1ca46fbea53165f3e40fe169372f8fa3f62b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.27-3/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.27-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.27-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.2-5`

Binary Packages:

- `libgnutls30:amd64=3.7.2-5`

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
$ apt-get source -qq --print-uris gnutls28=3.7.2-5
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2-5.dsc' gnutls28_3.7.2-5.dsc 3467 SHA256:1b5f26b3222d3b45b1e77e2727ed688d143cb81298bdb6230698d7541fd5be96
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2.orig.tar.xz' gnutls28_3.7.2.orig.tar.xz 6091508 SHA256:646e6c5a9a185faa4cea796d378a1ba8e1148dbb197ca6605f95986a25af2752
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2.orig.tar.xz.asc' gnutls28_3.7.2.orig.tar.xz.asc 833 SHA256:015e4f3390469126a94014e4aa1182ed4b238f940ff09093884cc04f8fefedf0
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.2-5.debian.tar.xz' gnutls28_3.7.2-5.debian.tar.xz 65704 SHA256:1c1fa71f8b69938747b24786154e08900f92347e5c34177a7a1fc7e81ecb3939
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.2-5/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.2-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.2-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `init-system-helpers=1.61`

Binary Packages:

- `init-system-helpers=1.61`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/init-system-helpers/1.61/


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

- `libjbig0:amd64=2.1-3.1+b2`

Licenses: (parsed from: `/usr/share/doc/libjbig0/copyright`)

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

### `dpkg` source package: `kernsmooth=2.23-20-1`

Binary Packages:

- `r-cran-kernsmooth=2.23-20-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris kernsmooth=2.23-20-1
'http://deb.debian.org/debian/pool/main/k/kernsmooth/kernsmooth_2.23-20-1.dsc' kernsmooth_2.23-20-1.dsc 1891 SHA256:2b09ccd2ac359365bd3cb32aa688b1cabb89beb2e25e21a5768da6604cf11c1d
'http://deb.debian.org/debian/pool/main/k/kernsmooth/kernsmooth_2.23-20.orig.tar.gz' kernsmooth_2.23-20.orig.tar.gz 25946 SHA256:20eb75051e2473933d41eedc9945b03c632847fd581e2207d452cf317fa5ec39
'http://deb.debian.org/debian/pool/main/k/kernsmooth/kernsmooth_2.23-20-1.debian.tar.xz' kernsmooth_2.23-20-1.debian.tar.xz 3356 SHA256:900201f86061c4ebdbe9f0bfd888574169fb0ed5f254e993a00c80a0b59a8942
```

Other potentially useful URLs:

- https://sources.debian.net/src/kernsmooth/2.23-20-1/ (for browsing the source)
- https://sources.debian.net/src/kernsmooth/2.23-20-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/kernsmooth/2.23-20-1/ (for access to the source package after it no longer exists in the archive)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/krb5/1.18.3-7/


### `dpkg` source package: `lapack=3.10.0-2`

Binary Packages:

- `libblas-dev:amd64=3.10.0-2`
- `libblas3:amd64=3.10.0-2`
- `liblapack-dev:amd64=3.10.0-2`
- `liblapack3:amd64=3.10.0-2`

Licenses: (parsed from: `/usr/share/doc/libblas-dev/copyright`, `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack-dev/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.10.0-2
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.10.0-2.dsc' lapack_3.10.0-2.dsc 3367 SHA256:31f1c05d4d90534a77b9ce0476fad5edcfdac3bb23b23c4665603a1a1b85f877
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.10.0.orig.tar.gz' lapack_3.10.0.orig.tar.gz 7630775 SHA256:328c1bea493a32cac5257d84157dc686cc3ab0b004e2bea22044e0a59f6f8a19
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.10.0-2.debian.tar.xz' lapack_3.10.0-2.debian.tar.xz 28892 SHA256:884a5f1322652ba954d81643d945c804edbad1f5b8d4ce4f85d49ba646ec19cf
```

Other potentially useful URLs:

- https://sources.debian.net/src/lapack/3.10.0-2/ (for browsing the source)
- https://sources.debian.net/src/lapack/3.10.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lapack/3.10.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lattice=0.20-45-1`

Binary Packages:

- `r-cran-lattice=0.20-45-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-lattice/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris lattice=0.20-45-1
'http://deb.debian.org/debian/pool/main/l/lattice/lattice_0.20-45-1.dsc' lattice_0.20-45-1.dsc 1845 SHA256:91059569a3f5c48b5335b21d9327768917eae28074a9dde645814b9de4273b0a
'http://deb.debian.org/debian/pool/main/l/lattice/lattice_0.20-45.orig.tar.gz' lattice_0.20-45.orig.tar.gz 399470 SHA256:22388d92bdb7d3959da84d7308d9026dd8226ef07580783729e8ad2f7d7507ad
'http://deb.debian.org/debian/pool/main/l/lattice/lattice_0.20-45-1.debian.tar.xz' lattice_0.20-45-1.debian.tar.xz 5248 SHA256:812679c35b8b87c4f01427521703f08b01a499578e9a3d7582b1d6b59162434e
```

Other potentially useful URLs:

- https://sources.debian.net/src/lattice/0.20-45-1/ (for browsing the source)
- https://sources.debian.net/src/lattice/0.20-45-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lattice/0.20-45-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `less=590-1`

Binary Packages:

- `less=590-1`

Licenses: (parsed from: `/usr/share/doc/less/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris less=590-1
'http://deb.debian.org/debian/pool/main/l/less/less_590-1.dsc' less_590-1.dsc 1631 SHA256:b5af7821e53e5b8c12470b0959eb2663433806da494e096c3a07e3c9eaddadd2
'http://deb.debian.org/debian/pool/main/l/less/less_590.orig.tar.gz' less_590.orig.tar.gz 352574 SHA256:6aadf54be8bf57d0e2999a3c5d67b1de63808bb90deb8f77b028eafae3a08e10
'http://deb.debian.org/debian/pool/main/l/less/less_590-1.debian.tar.xz' less_590-1.debian.tar.xz 19016 SHA256:2cd2a158b05fae31416ed1d861633ed909a5b4d5b0ed22986742ceabcf5ac55a
```

Other potentially useful URLs:

- https://sources.debian.net/src/less/590-1/ (for browsing the source)
- https://sources.debian.net/src/less/590-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/less/590-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.11.4-1`

Binary Packages:

- `libbsd0:amd64=0.11.4-1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libbsd/0.11.4-1/


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

### `dpkg` source package: `libdeflate=1.8-1`

Binary Packages:

- `libdeflate0:amd64=1.8-1`

Licenses: (parsed from: `/usr/share/doc/libdeflate0/copyright`)

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

### `dpkg` source package: `libffi=3.4.2-4`

Binary Packages:

- `libffi8:amd64=3.4.2-4`

Licenses: (parsed from: `/usr/share/doc/libffi8/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.2-4
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2-4.dsc' libffi_3.4.2-4.dsc 1948 SHA256:c7c4890a434795e41a77bddbca949fb904b022a70d8446c5a005ec0f9ed4c554
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2.orig.tar.gz' libffi_3.4.2.orig.tar.gz 1351355 SHA256:540fb721619a6aba3bdeef7d940d8e9e0e6d2c193595bc243241b77ff9e93620
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2-4.debian.tar.xz' libffi_3.4.2-4.debian.tar.xz 8164 SHA256:06d936d00d43e7999d0bce0aa2e0f1550109295b8093de77e6453acb9eacfd19
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.4.2-4/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.4.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.4.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.9.4-5`

Binary Packages:

- `libgcrypt20:amd64=1.9.4-5`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.9.4-5
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4-5.dsc' libgcrypt20_1.9.4-5.dsc 2800 SHA256:809342159731b6fd7921ee576a0e836a10760703ac07b363bce05bbb188c8484
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4.orig.tar.bz2' libgcrypt20_1.9.4.orig.tar.bz2 3239704 SHA256:ea849c83a72454e3ed4267697e8ca03390aee972ab421e7df69dfe42b65caaf7
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4.orig.tar.bz2.asc' libgcrypt20_1.9.4.orig.tar.bz2.asc 228 SHA256:aa44cb00b779b4e75f3e63abeedd4112b10b4b92914dad8f23438fd0217a9fec
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4-5.debian.tar.xz' libgcrypt20_1.9.4-5.debian.tar.xz 35768 SHA256:f03349a3eb9940fc45419da0a5a2ff49ee78bdaa7e79a8fcf403cd1d3a611f36
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.9.4-5/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.9.4-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.9.4-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.43-3`

Binary Packages:

- `libgpg-error0:amd64=1.43-3`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.43-3
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.43-3.dsc' libgpg-error_1.43-3.dsc 2270 SHA256:4cebb44aa01a2dfc75eae5b5758ac73f353778e1391e55726264fabf06944a23
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.43.orig.tar.bz2' libgpg-error_1.43.orig.tar.bz2 999006 SHA256:a9ab83ca7acc442a5bd846a75b920285ff79bdb4e3d34aa382be88ed2c3aebaf
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.43.orig.tar.bz2.asc' libgpg-error_1.43.orig.tar.bz2.asc 238 SHA256:6f1f0354aee0abc946d7f0e604fa69d5826a312baabcc0bb4fad4f97899cfa80
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.43-3.debian.tar.xz' libgpg-error_1.43-3.debian.tar.xz 19264 SHA256:d9d4efa45fc8d58152cbfa3bbaa68ed1977d8c56b7d59a579ef4feb4ffe7ec83
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.43-3/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.43-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.43-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libice=2:1.0.10-1`

Binary Packages:

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

### `dpkg` source package: `libjpeg-turbo=1:2.1.2-1`

Binary Packages:

- `libjpeg-dev:amd64=1:2.1.2-1`
- `libjpeg62-turbo:amd64=1:2.1.2-1`
- `libjpeg62-turbo-dev:amd64=1:2.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3-clause`
- `BSD-BY-LC-NE`
- `BSD-BY-LC-NE `
- `Expat`
- `NTP`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:2.1.2-1
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2-1.dsc' libjpeg-turbo_2.1.2-1.dsc 2490 SHA256:e40ec3e3b73570ac9ac1e414e8a2e70e42e83463b97890ba1f2138f67aa14c4b
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2.orig.tar.gz' libjpeg-turbo_2.1.2.orig.tar.gz 2257645 SHA256:e7fdc8a255c45bc8fbd9aa11c1a49c23092fcd7379296aeaeb14d3343a3d1bed
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2-1.debian.tar.xz' libjpeg-turbo_2.1.2-1.debian.tar.xz 98752 SHA256:2bb65a55a3faff6470e34b74cd7756e6b1db79df41d90cd2c4fce2f394f25d73
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:2.1.2-1/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:2.1.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:2.1.2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libpaper=1.1.28`

Binary Packages:

- `libpaper-utils=1.1.28+b1`
- `libpaper1:amd64=1.1.28+b1`

Licenses: (parsed from: `/usr/share/doc/libpaper-utils/copyright`, `/usr/share/doc/libpaper1/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libpaper=1.1.28
'http://deb.debian.org/debian/pool/main/libp/libpaper/libpaper_1.1.28.dsc' libpaper_1.1.28.dsc 1633 SHA256:298d6347d84ece2f55088e371facc13362c8f4731d80f94c6ad84190309de8b4
'http://deb.debian.org/debian/pool/main/libp/libpaper/libpaper_1.1.28.tar.gz' libpaper_1.1.28.tar.gz 42356 SHA256:c8bb946ec93d3c2c72bbb1d7257e90172a22a44a07a07fb6b802a5bb2c95fddc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpaper/1.1.28/ (for browsing the source)
- https://sources.debian.net/src/libpaper/1.1.28/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpaper/1.1.28/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libseccomp=2.5.3-2`

Binary Packages:

- `libseccomp2:amd64=2.5.3-2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.3-2
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.3-2.dsc' libseccomp_2.5.3-2.dsc 2676 SHA256:d6325664ec9ff84e6b9787b78e0a431424c414217a6dd0f4098ea32df53db26f
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.3.orig.tar.gz' libseccomp_2.5.3.orig.tar.gz 637572 SHA256:59065c8733364725e9721ba48c3a99bbc52af921daf48df4b1e012fbc7b10a76
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.3.orig.tar.gz.asc' libseccomp_2.5.3.orig.tar.gz.asc 833 SHA256:cc1cbe9d9eb6a67b78de107eb37b2bc8d7599e3c1d36699ae2528db489cb5d44
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.3-2.debian.tar.xz' libseccomp_2.5.3-2.debian.tar.xz 16268 SHA256:b0e094e78c3e4f2c94288c1543dd879dabac7d11a22b7e0fb685d7560a1d24ba
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.5.3-2/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.5.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.5.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.3-1`

Binary Packages:

- `libselinux1:amd64=3.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

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
- `libsemanage2:amd64=3.3-1+b1`

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

- `libsepol2:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

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

### `dpkg` source package: `libsm=2:1.2.3-1`

Binary Packages:

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libunistring/0.9.10-6/


### `dpkg` source package: `libwebp=0.6.1-2.1`

Binary Packages:

- `libwebp6:amd64=0.6.1-2.1`

Licenses: (parsed from: `/usr/share/doc/libwebp6/copyright`)

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

### `dpkg` source package: `libx11=2:1.7.2-2`

Binary Packages:

- `libx11-6:amd64=2:1.7.2-2+b1`
- `libx11-data=2:1.7.2-2`

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
- `libxcb-shm0:amd64=1.14-3`
- `libxcb1:amd64=1.14-3`

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

### `dpkg` source package: `libxcrypt=1:4.4.27-1.1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.27-1.1`
- `libcrypt1:amd64=1:4.4.27-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.27-1.1
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.27-1.1.dsc' libxcrypt_4.4.27-1.1.dsc 2138 SHA256:ce8324ad21185e045991347e412ac83313dd0061357951a70655847577ba087e
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.27.orig.tar.xz' libxcrypt_4.4.27.orig.tar.xz 391772 SHA256:cc0762a751224a5cb45329fb731f25016a8d8292749d8b4010f4b68144db6961
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.27-1.1.debian.tar.xz' libxcrypt_4.4.27-1.1.debian.tar.xz 7880 SHA256:55ef3306bb49772e2cf602f336a202a0b1de94c61cb5e8c1de7899b556c97c20
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.27-1.1/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.27-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.27-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdmcp=1:1.1.2-3`

Binary Packages:

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

### `dpkg` source package: `libxmu=2:1.1.2-2`

Binary Packages:

- `libxmuu1:amd64=2:1.1.2-2+b3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxmu/2:1.1.2-2/


### `dpkg` source package: `libxrender=1:0.9.10-1`

Binary Packages:

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

### `dpkg` source package: `libxss=1:1.2.3-1`

Binary Packages:

- `libxss1:amd64=1:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxss=1:1.2.3-1
'http://deb.debian.org/debian/pool/main/libx/libxss/libxss_1.2.3-1.dsc' libxss_1.2.3-1.dsc 2203 SHA256:783dbcd49a0934d994693af676ee98734dad070ab2434a6afe831c2de0ecca1d
'http://deb.debian.org/debian/pool/main/libx/libxss/libxss_1.2.3.orig.tar.gz' libxss_1.2.3.orig.tar.gz 385215 SHA256:4f74e7e412144591d8e0616db27f433cfc9f45aae6669c6c4bb03e6bf9be809a
'http://deb.debian.org/debian/pool/main/libx/libxss/libxss_1.2.3.orig.tar.gz.asc' libxss_1.2.3.orig.tar.gz.asc 705 SHA256:4e900524d56c8e7263365267efa91bb3671110c9eb28ccab58f70e2188f0b91b
'http://deb.debian.org/debian/pool/main/libx/libxss/libxss_1.2.3-1.diff.gz' libxss_1.2.3-1.diff.gz 7145 SHA256:9d381b48f1377f27c506113e1f9b7d6ee286b856421f7f2b27017f01dccfef04
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxss/1:1.2.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxss/1:1.2.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxss/1:1.2.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxt=1:1.2.0-1`

Binary Packages:

- `libxt6:amd64=1:1.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxt/1:1.2.0-1/


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
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-3.dsc' libzstd_1.4.8+dfsg-3.dsc 2291 SHA256:03a5589a689fb0e6480ee26af40104ce67a435f7b70d2bdd156221666d9d530a
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA256:1e8ce5c4880a6d5bd8d3186e4186607dd19b64fc98a3877fc13aeefd566d67c5
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-3.debian.tar.xz' libzstd_1.4.8+dfsg-3.debian.tar.xz 12184 SHA256:fecd87a469d5a07b6deeeef53ed24b2f1a74ee097ce11528fe3b58540f05c147
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.4.8+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.4.8+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.4.8+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `linux=5.15.15-1`

Binary Packages:

- `linux-libc-dev:amd64=5.15.15-1`

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
$ apt-get source -qq --print-uris linux=5.15.15-1
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.15.15-1.dsc' linux_5.15.15-1.dsc 194415 SHA256:d2e96180c0dfa964e3004e0ce298d3a6b6a6f632f01865c587e5ab7ba02e5332
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.15.15.orig.tar.xz' linux_5.15.15.orig.tar.xz 127780628 SHA256:12c2da3d97032f91d30f5dce68fa9f35c80a0533f9ca651a09c3c48c5b1b0f05
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.15.15-1.debian.tar.xz' linux_5.15.15-1.debian.tar.xz 1318828 SHA256:f23941ba6d4fafbafc1294b22536b62819e699742d78870a2a1311560f65faf6
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/5.15.15-1/ (for browsing the source)
- https://sources.debian.net/src/linux/5.15.15-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/5.15.15-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `littler=0.3.15-1`

Binary Packages:

- `littler=0.3.15-1`
- `r-cran-littler=0.3.15-1`

Licenses: (parsed from: `/usr/share/doc/littler/copyright`, `/usr/share/doc/r-cran-littler/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris littler=0.3.15-1
'http://deb.debian.org/debian/pool/main/l/littler/littler_0.3.15-1.dsc' littler_0.3.15-1.dsc 1874 SHA256:2b5a8a689a5f4a6eca6588291fffbb399ca1ff8d2257f7b440292b330ac6d1bc
'http://deb.debian.org/debian/pool/main/l/littler/littler_0.3.15.orig.tar.gz' littler_0.3.15.orig.tar.gz 113843 SHA256:89e80f59394db434fdb37578e3d86e8daae828991bf148763ecff5edcb1e2f91
'http://deb.debian.org/debian/pool/main/l/littler/littler_0.3.15-1.debian.tar.xz' littler_0.3.15-1.debian.tar.xz 7000 SHA256:aae8cf40a551edf18bd249542f31f193876f62af1c6fc44dba0fc370c7136d40
```

Other potentially useful URLs:

- https://sources.debian.net/src/littler/0.3.15-1/ (for browsing the source)
- https://sources.debian.net/src/littler/0.3.15-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/littler/0.3.15-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mawk=1.3.4.20200120-2`

Binary Packages:

- `mawk=1.3.4.20200120-2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/mawk/1.3.4.20200120-2/


### `dpkg` source package: `mgcv=1.8-38-1`

Binary Packages:

- `r-cran-mgcv=1.8-38-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-mgcv/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris mgcv=1.8-38-1
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-38-1.dsc' mgcv_1.8-38-1.dsc 1833 SHA256:d7d74e69d86814c638d6015567ba6f889829521c298c04465444c825770734b7
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-38.orig.tar.gz' mgcv_1.8-38.orig.tar.gz 1207405 SHA256:cd12ed5787d6fdcead34e782e48b62b3f9efd523616c906e2da77bd9c142ddbb
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-38-1.debian.tar.xz' mgcv_1.8-38-1.debian.tar.xz 5408 SHA256:f8dd3de5e87fbc259a51254daaa5fa2c19b929fb7fb3700d833c40480e0df441
```

Other potentially useful URLs:

- https://sources.debian.net/src/mgcv/1.8-38-1/ (for browsing the source)
- https://sources.debian.net/src/mgcv/1.8-38-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mgcv/1.8-38-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ncurses=6.3-2`

Binary Packages:

- `libncurses-dev:amd64=6.3-2`
- `libncurses5-dev:amd64=6.3-2`
- `libncurses6:amd64=6.3-2`
- `libncursesw6:amd64=6.3-2`
- `libtinfo6:amd64=6.3-2`
- `ncurses-base=6.3-2`
- `ncurses-bin=6.3-2`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.3-2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3-2.dsc' ncurses_6.3-2.dsc 4136 SHA256:a4e3cfede146d1b7bfc45ca93f029d8344e2c209a657a2fc09fbe90bbebd9c0b
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3.orig.tar.gz' ncurses_6.3.orig.tar.gz 3583550 SHA256:97fc51ac2b085d4cde31ef4d2c3122c21abc217e9090a43a30fc5ec21684e059
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3.orig.tar.gz.asc' ncurses_6.3.orig.tar.gz.asc 729 SHA256:37b9e80c11fa02fbd8caf42ab9573427f54f2c7212eb4aeec9f455b5d79dee14
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3-2.debian.tar.xz' ncurses_6.3-2.debian.tar.xz 54136 SHA256:d76896693ce0b05f294512328efeb5940b1e0cbf695b6c9b118b2dc18f27df22
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.3-2/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.3-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `nlme=3.1.155-1`

Binary Packages:

- `r-cran-nlme=3.1.155-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-nlme/copyright`)

- `GPL`
- `GPL `

Source:

```console
$ apt-get source -qq --print-uris nlme=3.1.155-1
'http://deb.debian.org/debian/pool/main/n/nlme/nlme_3.1.155-1.dsc' nlme_3.1.155-1.dsc 1840 SHA256:99e9879ec36827d35e32dc48c4236807582a8afce7a9d0eefb4c74cee3b79d52
'http://deb.debian.org/debian/pool/main/n/nlme/nlme_3.1.155.orig.tar.gz' nlme_3.1.155.orig.tar.gz 806854 SHA256:9f390f842852422921b5845130ea73c1f006d7bb5e988e82f728093a0cbdff4f
'http://deb.debian.org/debian/pool/main/n/nlme/nlme_3.1.155-1.debian.tar.xz' nlme_3.1.155-1.debian.tar.xz 7188 SHA256:2ff006849d827550f008e782eb6d545b7515d7457586b00d7cec6d6091955e65
```

Other potentially useful URLs:

- https://sources.debian.net/src/nlme/3.1.155-1/ (for browsing the source)
- https://sources.debian.net/src/nlme/3.1.155-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nlme/3.1.155-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openblas=0.3.19+ds-3`

Binary Packages:

- `libopenblas0-pthread:amd64=0.3.19+ds-3`

Licenses: (parsed from: `/usr/share/doc/libopenblas0-pthread/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-2-clause-texas`
- `BSD-3-clause`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openblas/0.3.19+ds-3/


### `dpkg` source package: `openldap=2.4.59+dfsg-1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.59+dfsg-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.59+dfsg-1
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.59%2bdfsg-1.dsc' openldap_2.4.59+dfsg-1.dsc 3113 SHA256:cc2578c30b177406eb9cc1341cca710e4c4ac66230c40633f11a2a26290a6336
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.59%2bdfsg.orig.tar.gz' openldap_2.4.59+dfsg.orig.tar.gz 5056324 SHA256:cdeac7531ff072b0cdde29fcc19534d6ac00e9002ecd554d2ff69f897607bf6d
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.59%2bdfsg-1.debian.tar.xz' openldap_2.4.59+dfsg-1.debian.tar.xz 170320 SHA256:f57e80ab6ecdad5a0a3aed41d1ae9962129d0f3c9e5631ff6c56c2de19d10d60
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.59+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.59+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.59+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.1m-1`

Binary Packages:

- `libssl1.1:amd64=1.1.1m-1`
- `openssl=1.1.1m-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1m-1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1m-1.dsc' openssl_1.1.1m-1.dsc 2620 SHA256:a2e12c68b44d7bb6ef049a7583cd02b85201ce83ad11b57ce4c87ec6b05a0b1d
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1m.orig.tar.gz' openssl_1.1.1m.orig.tar.gz 9847315 SHA256:f89199be8b23ca45fc7cb9f1d8d3ee67312318286ad030f5316aca6462db6c96
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1m.orig.tar.gz.asc' openssl_1.1.1m.orig.tar.gz.asc 488 SHA256:49f209fe54825f6645f788f124ff6c3e1fab698434732cf3685dc63639d42820
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1m-1.debian.tar.xz' openssl_1.1.1m-1.debian.tar.xz 84744 SHA256:d2f6f2ec533bb840b7cfd37818eef23d6f226f308046328d20e0849feef6007e
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.1m-1/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.1m-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.1m-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.24.0-6`

Binary Packages:

- `libp11-kit0:amd64=0.24.0-6`

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
$ apt-get source -qq --print-uris p11-kit=0.24.0-6
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0-6.dsc' p11-kit_0.24.0-6.dsc 2501 SHA256:c313e3ab1b9405633abe103ce44608f29556aca65c45fcc349b749bd1c114ff6
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0.orig.tar.xz' p11-kit_0.24.0.orig.tar.xz 834392 SHA256:81e6140584f635e4e956a1b93a32239acf3811ff5b2d3a5c6094e94e99d2c685
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0.orig.tar.xz.asc' p11-kit_0.24.0.orig.tar.xz.asc 833 SHA256:f9996976ae08e48ac652d2aad3f0528a75f87eaa6c17cf076ec00e7ce2fbaeed
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.0-6.debian.tar.xz' p11-kit_0.24.0-6.debian.tar.xz 23176 SHA256:076d61ccfcc53193cd40d57976a850d9c4d361b84acf6f9070c1e59930be61b1
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.24.0-6/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.24.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.24.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.4.0-11`

Binary Packages:

- `libpam-modules:amd64=1.4.0-11`
- `libpam-modules-bin=1.4.0-11`
- `libpam-runtime=1.4.0-11`
- `libpam0g:amd64=1.4.0-11`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.4.0-11
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-11.dsc' pam_1.4.0-11.dsc 2543 SHA256:49f996d03d8781d8dda78a58ea4eca3c16c4ea8430556b8ad915b4bbbb069056
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0.orig.tar.xz' pam_1.4.0.orig.tar.xz 988908 SHA256:cd6d928c51e64139be3bdb38692c68183a509b83d4f2c221024ccd4bcddfd034
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-11.debian.tar.xz' pam_1.4.0-11.debian.tar.xz 121324 SHA256:c190f584ceb5d667f1af0f9dd91f220bbb557a7e4b642263a142b702f5ee0dee
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.4.0-11/ (for browsing the source)
- https://sources.debian.net/src/pam/1.4.0-11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.4.0-11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pango1.0=1.50.3+ds1-4`

Binary Packages:

- `libpango-1.0-0:amd64=1.50.3+ds1-4`
- `libpangocairo-1.0-0:amd64=1.50.3+ds1-4`
- `libpangoft2-1.0-0:amd64=1.50.3+ds1-4`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Apache-2`
- `Apache-2.0`
- `Bitstream-Vera`
- `CC-BY-SA-3.0`
- `CC-BY-SA-3.0,`
- `CC0-1.0`
- `CC0-1.0,`
- `Chromium-BSD-style`
- `Example`
- `Expat`
- `GPL-2+`
- `GPL-2+,`
- `GPL-2.0`
- `GPL-3.0`
- `GPL-3.0+`
- `GPL-3.0+,`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2+,`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.1`
- `OFL-1.1`
- `TCL`
- `Unicode`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pango1.0/1.50.3+ds1-4/


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

### `dpkg` source package: `pcre2=10.39-3`

Binary Packages:

- `libpcre2-16-0:amd64=10.39-3`
- `libpcre2-32-0:amd64=10.39-3`
- `libpcre2-8-0:amd64=10.39-3`
- `libpcre2-dev:amd64=10.39-3`
- `libpcre2-posix3:amd64=10.39-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.39-3
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.39-3.dsc' pcre2_10.39-3.dsc 2286 SHA256:fdb34ea12f4cd80570f22228990bfbc2fa4cf9ebfd14495c94646687495d61ef
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.39.orig.tar.gz' pcre2_10.39.orig.tar.gz 2309964 SHA256:0781bd2536ef5279b1943471fdcdbd9961a2845e1d2c9ad849b9bd98ba1a9bd4
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.39-3.diff.gz' pcre2_10.39-3.diff.gz 7080 SHA256:04c45c7ce5f7acef85902bd0292713232a036dd26d20dae171167f06adb6378e
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.39-3/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.39-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.39-3/ (for access to the source package after it no longer exists in the archive)

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
'http://http.debian.net/debian/pool/main/p/perl/perl_5.32.1-6.dsc' perl_5.32.1-6.dsc 2886 SHA256:dba78a9b8d7c091ec4a435add1cad82108534275bd321a956c12e66a5a9bfe19
'http://http.debian.net/debian/pool/main/p/perl/perl_5.32.1.orig-regen-configure.tar.gz' perl_5.32.1.orig-regen-configure.tar.gz 871331 SHA256:1d179b41283f12ad83f9758430f6ddc49bdf20db5c396aeae7e51ebb4e4afd29
'http://http.debian.net/debian/pool/main/p/perl/perl_5.32.1.orig.tar.xz' perl_5.32.1.orig.tar.xz 12610988 SHA256:57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309
'http://http.debian.net/debian/pool/main/p/perl/perl_5.32.1-6.debian.tar.xz' perl_5.32.1-6.debian.tar.xz 167612 SHA256:d39878f0651b41c8a87aa48daec0b577baa720d6e7f3f14c40fd40fe025bb785
```

### `dpkg` source package: `pixman=0.40.0-1`

Binary Packages:

- `libpixman-1-0:amd64=0.40.0-1`

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

### `dpkg` source package: `r-base=4.1.2-1`

Binary Packages:

- `r-base=4.1.2-1`
- `r-base-core=4.1.2-1`
- `r-base-dev=4.1.2-1`
- `r-recommended=4.1.2-1`

Licenses: (parsed from: `/usr/share/doc/r-base/copyright`, `/usr/share/doc/r-base-core/copyright`, `/usr/share/doc/r-base-dev/copyright`, `/usr/share/doc/r-recommended/copyright`)

- `Artistic`
- `GPL-2`
- `GPL-3`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/r-base/4.1.2-1/


### `dpkg` source package: `r-cran-class=7.3-20-1`

Binary Packages:

- `r-cran-class=7.3-20-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-class/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-class=7.3-20-1
'http://deb.debian.org/debian/pool/main/r/r-cran-class/r-cran-class_7.3-20-1.dsc' r-cran-class_7.3-20-1.dsc 1873 SHA256:dbac95f40d16224325935c142e594f5266ba969604d15a5f4a9b64b284814c9d
'http://deb.debian.org/debian/pool/main/r/r-cran-class/r-cran-class_7.3-20.orig.tar.gz' r-cran-class_7.3-20.orig.tar.gz 20769 SHA256:e65b046bc72b312ff0c5dc7feba4fa3e9bc63387274d44911493782b85f65483
'http://deb.debian.org/debian/pool/main/r/r-cran-class/r-cran-class_7.3-20-1.debian.tar.xz' r-cran-class_7.3-20-1.debian.tar.xz 3220 SHA256:745027c11ceb5cd7a6fa34bc252bfc6183234bb036ffaecf36c553ca434a1f97
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-class/7.3-20-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-class/7.3-20-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-class/7.3-20-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-mass=7.3-55-1`

Binary Packages:

- `r-cran-mass=7.3-55-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-mass/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-mass=7.3-55-1
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-55-1.dsc' r-cran-mass_7.3-55-1.dsc 1851 SHA256:1d1bcc2742909947ccf2cf7dfb4563a64566d25a70f6b82a46ca886d43efa448
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-55.orig.tar.gz' r-cran-mass_7.3-55.orig.tar.gz 508478 SHA256:65299cbc8f3fd5e09cb3535eabcb3faad2308e01d5ba9422145cc04d7d0c31a4
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-55-1.debian.tar.xz' r-cran-mass_7.3-55-1.debian.tar.xz 6400 SHA256:1b1e555e31dc78aa425c16b98020025aa8c44267f40195881e8fcbf4a5989d5f
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-mass/7.3-55-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-mass/7.3-55-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-mass/7.3-55-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-nnet=7.3-17-1`

Binary Packages:

- `r-cran-nnet=7.3-17-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-nnet/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-nnet=7.3-17-1
'http://deb.debian.org/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-17-1.dsc' r-cran-nnet_7.3-17-1.dsc 1848 SHA256:3e098e2c9f19fbd5f7efde7b114116972d11db3f0901d377e4f78a73fc50617a
'http://deb.debian.org/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-17.orig.tar.gz' r-cran-nnet_7.3-17.orig.tar.gz 29099 SHA256:ee750bb8164aa058edf93823af987ab2c7ec64128dce2abeaae1b7d3661e9a67
'http://deb.debian.org/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-17-1.debian.tar.xz' r-cran-nnet_7.3-17-1.debian.tar.xz 3256 SHA256:ce23a6b2a4ec588bdaa9916274cd61781500964ab049ab7eac0a58124a557a11
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-nnet/7.3-17-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-nnet/7.3-17-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-nnet/7.3-17-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-spatial=7.3-15-1`

Binary Packages:

- `r-cran-spatial=7.3-15-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-spatial/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-spatial=7.3-15-1
'http://deb.debian.org/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-15-1.dsc' r-cran-spatial_7.3-15-1.dsc 1884 SHA256:1d661b20136cb8c3889b045c4addcb5fbf4128e916eb28b38ba50b272356322a
'http://deb.debian.org/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-15.orig.tar.gz' r-cran-spatial_7.3-15.orig.tar.gz 44618 SHA256:e5613be94d6f5c1f54813dadc96e4a86b3417dea28106cc90cb24dfd6c3c8cef
'http://deb.debian.org/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-15-1.debian.tar.xz' r-cran-spatial_7.3-15-1.debian.tar.xz 3184 SHA256:2d1af14fe71a5d721fc42845f2649f6068593a27b2bae2b0273a9818e19a13a2
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-spatial/7.3-15-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-spatial/7.3-15-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-spatial/7.3-15-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.1.2-1`

Binary Packages:

- `libreadline-dev:amd64=8.1.2-1`
- `libreadline8:amd64=8.1.2-1`
- `readline-common=8.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1.2-1
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1.2-1.dsc' readline_8.1.2-1.dsc 2432 SHA256:8558058b41165ffbbf406e744e726326e649a55c0f2c1490a467c01d314adec2
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1.2.orig.tar.gz' readline_8.1.2.orig.tar.gz 2993073 SHA256:7589a2381a8419e68654a47623ce7dfcb756815c8fee726b98f90bf668af7bc6
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1.2-1.debian.tar.xz' readline_8.1.2-1.debian.tar.xz 29292 SHA256:0c39840fbed2abd3f93083d75c974e39855fd41aa6df5fa1be06d147e86071ca
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/8.1.2-1/ (for browsing the source)
- https://sources.debian.net/src/readline/8.1.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/8.1.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rmatrix=1.4-0-1`

Binary Packages:

- `r-cran-matrix=1.4-0-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-matrix/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rmatrix=1.4-0-1
'http://deb.debian.org/debian/pool/main/r/rmatrix/rmatrix_1.4-0-1.dsc' rmatrix_1.4-0-1.dsc 1860 SHA256:c1975150d340669e1f9174948833c81f958a8efc5567714d16cd88dc3b4b8cf0
'http://deb.debian.org/debian/pool/main/r/rmatrix/rmatrix_1.4-0.orig.tar.gz' rmatrix_1.4-0.orig.tar.gz 2849865 SHA256:c2b463702e4051b621f5e2b091a33f883f1caa97703d65f7a52b78caf81206f6
'http://deb.debian.org/debian/pool/main/r/rmatrix/rmatrix_1.4-0-1.debian.tar.xz' rmatrix_1.4-0-1.debian.tar.xz 5704 SHA256:30a9faccd02fabf48f992d7147fc31998cc93dbe5d8a59dad3fa75c684c552ec
```

Other potentially useful URLs:

- https://sources.debian.net/src/rmatrix/1.4-0-1/ (for browsing the source)
- https://sources.debian.net/src/rmatrix/1.4-0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rmatrix/1.4-0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rpart=4.1-15-2`

Binary Packages:

- `r-cran-rpart=4.1-15-2+b1`

Licenses: (parsed from: `/usr/share/doc/r-cran-rpart/copyright`)

- `GPL-2`
- `GPL-2 | license included below`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/rpart/4.1-15-2/


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
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc 2299 SHA256:a296819cd2ab5880b67ad963ef0867cb10e462f4403e52565aa863eb05bb1370
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz 8096 SHA256:26d47de07d16285e4ca55b0828cbbf1ba35e671f9b3500a87e301fe755d26882
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

### `dpkg` source package: `shadow=1:4.8.1-2`

Binary Packages:

- `login=1:4.8.1-2`
- `passwd=1:4.8.1-2`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/shadow/1:4.8.1-2/


### `dpkg` source package: `survival=3.2-13-1`

Binary Packages:

- `r-cran-survival=3.2-13-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-survival/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris survival=3.2-13-1
'http://deb.debian.org/debian/pool/main/s/survival/survival_3.2-13-1.dsc' survival_3.2-13-1.dsc 1868 SHA256:fffe821caf20496457adaf056d9a0a2c331307bf164f4cc6e8966bb6c2247cba
'http://deb.debian.org/debian/pool/main/s/survival/survival_3.2-13.orig.tar.gz' survival_3.2-13.orig.tar.gz 6545339 SHA256:3fab9c0ba2c4e2b6a475207e2629a7f06a104c70093dfb768f50a7caac9a317f
'http://deb.debian.org/debian/pool/main/s/survival/survival_3.2-13-1.debian.tar.xz' survival_3.2-13-1.debian.tar.xz 6164 SHA256:b449d1d5dc4dbb905ea1c0a5c239ff4afb767c25042938bafd07d86dd1e14ad6
```

Other potentially useful URLs:

- https://sources.debian.net/src/survival/3.2-13-1/ (for browsing the source)
- https://sources.debian.net/src/survival/3.2-13-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/survival/3.2-13-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=250.3-1`

Binary Packages:

- `libsystemd0:amd64=250.3-1`
- `libudev1:amd64=250.3-1`

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

- http://snapshot.debian.org/package/systemd/250.3-1/


### `dpkg` source package: `sysvinit=3.01-1`

Binary Packages:

- `sysvinit-utils=3.01-1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.01-1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.01-1.dsc' sysvinit_3.01-1.dsc 2376 SHA256:3940946b5ba9c3f9c2053d6d5cb3b64a89cd1a2afa26c80abf6b956f35d04f22
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.01.orig.tar.xz' sysvinit_3.01.orig.tar.xz 126400 SHA256:4cc39f1c49f66c29e63360aea7a264a35ba2b853b41117251b9d23cf6d640b94
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.01-1.debian.tar.xz' sysvinit_3.01-1.debian.tar.xz 130496 SHA256:14aeeb78eab8621a04cdb9df9008a2c517dbee043a5f96741d4bbec6893bca5a
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/3.01-1/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/3.01-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/3.01-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.34+dfsg-1`

Binary Packages:

- `tar=1.34+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg-1.dsc' tar_1.34+dfsg-1.dsc 2015 SHA256:12d709cd77e38e5d1753325a9f266b340b5c095a426f438c677b42c031949d89
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA256:7d57029540cb928394defb3b377b3531237c947e795b51aa8acac0c5ba0e4844
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg-1.debian.tar.xz' tar_1.34+dfsg-1.debian.tar.xz 19192 SHA256:7228f5cbd36f937dfc1fec042dee8b3e02d92a06afdd44c586c2c8cfb1905538
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.34+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/tar/1.34+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.34+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tcl8.6=8.6.12+dfsg-1`

Binary Packages:

- `libtcl8.6:amd64=8.6.12+dfsg-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcl8.6=8.6.12+dfsg-1
'http://deb.debian.org/debian/pool/main/t/tcl8.6/tcl8.6_8.6.12%2bdfsg-1.dsc' tcl8.6_8.6.12+dfsg-1.dsc 2118 SHA256:2d3d155437fc21a2c4ce4117d4176ba3f0a125685c5c9c5f32d1707798e59033
'http://deb.debian.org/debian/pool/main/t/tcl8.6/tcl8.6_8.6.12%2bdfsg.orig.tar.gz' tcl8.6_8.6.12+dfsg.orig.tar.gz 6075478 SHA256:63e5d1392c5b1d0135cdf845542b1b6be821207c2991f76280657716bb271ae1
'http://deb.debian.org/debian/pool/main/t/tcl8.6/tcl8.6_8.6.12%2bdfsg-1.debian.tar.xz' tcl8.6_8.6.12+dfsg-1.debian.tar.xz 14388 SHA256:795fd4e564558ca450662b01ae3cbe83aae96d283b4945ee2d276641926ef61b
```

Other potentially useful URLs:

- https://sources.debian.net/src/tcl8.6/8.6.12+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/tcl8.6/8.6.12+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tcl8.6/8.6.12+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tex-gyre=20180621-3.1`

Binary Packages:

- `fonts-texgyre=20180621-3.1`

Licenses: (parsed from: `/usr/share/doc/fonts-texgyre/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris tex-gyre=20180621-3.1
'http://deb.debian.org/debian/pool/main/t/tex-gyre/tex-gyre_20180621-3.1.dsc' tex-gyre_20180621-3.1.dsc 2039 SHA256:d34500d573c01e0b608817b902f19c36880b7f833e91b36e20e99a0c4b2b1063
'http://deb.debian.org/debian/pool/main/t/tex-gyre/tex-gyre_20180621.orig.tar.gz' tex-gyre_20180621.orig.tar.gz 24033627 SHA256:fe6b0f8ca6890d4a369f36c3b45bc30470069701a2f59042178ad5933fc9cdb8
'http://deb.debian.org/debian/pool/main/t/tex-gyre/tex-gyre_20180621-3.1.debian.tar.xz' tex-gyre_20180621-3.1.debian.tar.xz 11096 SHA256:52d232bef3d92ad68589904ce906fbe0520c551ebc1ac07a6d1dd4c6694b048a
```

Other potentially useful URLs:

- https://sources.debian.net/src/tex-gyre/20180621-3.1/ (for browsing the source)
- https://sources.debian.net/src/tex-gyre/20180621-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tex-gyre/20180621-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.3.0-2`

Binary Packages:

- `libtiff5:amd64=4.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tiff/4.3.0-2/


### `dpkg` source package: `tk8.6=8.6.12-1`

Binary Packages:

- `libtk8.6:amd64=8.6.12-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tk8.6=8.6.12-1
'http://deb.debian.org/debian/pool/main/t/tk8.6/tk8.6_8.6.12-1.dsc' tk8.6_8.6.12-1.dsc 2153 SHA256:dcc8a036fe87bff6079d030a614983bde5e418e70f57587cf7cb87fb45db77f4
'http://deb.debian.org/debian/pool/main/t/tk8.6/tk8.6_8.6.12.orig.tar.gz' tk8.6_8.6.12.orig.tar.gz 4515393 SHA256:12395c1f3fcb6bed2938689f797ea3cdf41ed5cb6c4766eec8ac949560310630
'http://deb.debian.org/debian/pool/main/t/tk8.6/tk8.6_8.6.12-1.debian.tar.xz' tk8.6_8.6.12-1.debian.tar.xz 10764 SHA256:b0f5f3c6d29ffb51067b855b4355ed084705a041ecaec30f12d3d07146afb7a2
```

Other potentially useful URLs:

- https://sources.debian.net/src/tk8.6/8.6.12-1/ (for browsing the source)
- https://sources.debian.net/src/tk8.6/8.6.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tk8.6/8.6.12-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `util-linux=2.37.2-6`

Binary Packages:

- `bsdutils=1:2.37.2-6`
- `libblkid1:amd64=2.37.2-6`
- `libmount1:amd64=2.37.2-6`
- `libsmartcols1:amd64=2.37.2-6`
- `libuuid1:amd64=2.37.2-6`
- `mount=2.37.2-6`
- `util-linux=2.37.2-6`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/util-linux/2.37.2-6/


### `dpkg` source package: `vim=2:8.2.3995-1`

Binary Packages:

- `vim-common=2:8.2.3995-1`
- `vim-tiny=2:8.2.3995-1`
- `xxd=2:8.2.3995-1`

Licenses: (parsed from: `/usr/share/doc/vim-common/copyright`, `/usr/share/doc/vim-tiny/copyright`, `/usr/share/doc/xxd/copyright`)

- `Apache`
- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-2-clause`
- `BSD-3-clause`
- `Compaq`
- `EDL-1`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `OPL-1+`
- `SRA`
- `UC`
- `Vim`
- `Vim-Regexp`
- `X11`
- `XPM`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris vim=2:8.2.3995-1
'http://deb.debian.org/debian/pool/main/v/vim/vim_8.2.3995-1.dsc' vim_8.2.3995-1.dsc 3044 SHA256:da4a7f9c8216842eb2ae243246f4d97a32231f202916a50ab94c46a52a616615
'http://deb.debian.org/debian/pool/main/v/vim/vim_8.2.3995.orig.tar.xz' vim_8.2.3995.orig.tar.xz 10377164 SHA256:a9d4993d94a212c1e284fe19d7127508dc9c911cddaf91f2a6f72d0b9b71b8ce
'http://deb.debian.org/debian/pool/main/v/vim/vim_8.2.3995-1.debian.tar.xz' vim_8.2.3995-1.debian.tar.xz 211600 SHA256:a09a72d3e71617e065ef6b82fae151413168f7a5832ae7c6f602e11c3ca2acec
```

Other potentially useful URLs:

- https://sources.debian.net/src/vim/2:8.2.3995-1/ (for browsing the source)
- https://sources.debian.net/src/vim/2:8.2.3995-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/vim/2:8.2.3995-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xauth=1:1.1-1`

Binary Packages:

- `xauth=1:1.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xauth=1:1.1-1
'http://deb.debian.org/debian/pool/main/x/xauth/xauth_1.1-1.dsc' xauth_1.1-1.dsc 1878 SHA256:59f36197de42b36757aa37b142e187181ea49e7765c5f16a3e00f4576694d49d
'http://deb.debian.org/debian/pool/main/x/xauth/xauth_1.1.orig.tar.gz' xauth_1.1.orig.tar.gz 204146 SHA256:e9fce796c8c5c9368594b9e8bbba237fb54b6615f5fd60e8d0a5b3c52a92c5ef
'http://deb.debian.org/debian/pool/main/x/xauth/xauth_1.1-1.diff.gz' xauth_1.1-1.diff.gz 13752 SHA256:80f52f736ca3d5b5e79ccee802a271e16f4421748ab985709541cb77e965bf24
```

Other potentially useful URLs:

- https://sources.debian.net/src/xauth/1:1.1-1/ (for browsing the source)
- https://sources.debian.net/src/xauth/1:1.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xauth/1:1.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xdg-utils=1.1.3-4.1`

Binary Packages:

- `xdg-utils=1.1.3-4.1`

Licenses: (parsed from: `/usr/share/doc/xdg-utils/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris xdg-utils=1.1.3-4.1
'http://deb.debian.org/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3-4.1.dsc' xdg-utils_1.1.3-4.1.dsc 1756 SHA256:c54ae65034c4c3e9f2208a44990111d34fc5ed1e689efd3907a2a8e5e965ccac
'http://deb.debian.org/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3.orig.tar.gz' xdg-utils_1.1.3.orig.tar.gz 297170 SHA256:d798b08af8a8e2063ddde6c9fa3398ca81484f27dec642c5627ffcaa0d4051d9
'http://deb.debian.org/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3-4.1.debian.tar.xz' xdg-utils_1.1.3-4.1.debian.tar.xz 15660 SHA256:0ea0b550719ab75f9a0fe58ed907673c5bcfc2bd87537845534694c502740aed
```

Other potentially useful URLs:

- https://sources.debian.net/src/xdg-utils/1.1.3-4.1/ (for browsing the source)
- https://sources.debian.net/src/xdg-utils/1.1.3-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xdg-utils/1.1.3-4.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xft=2.3.2-2`

Binary Packages:

- `libxft2:amd64=2.3.2-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xft=2.3.2-2
'http://deb.debian.org/debian/pool/main/x/xft/xft_2.3.2-2.dsc' xft_2.3.2-2.dsc 2000 SHA256:56c1f34591cdc307e83abaabb28e22e190cabcf528241e18dfcd5dca9e530f89
'http://deb.debian.org/debian/pool/main/x/xft/xft_2.3.2.orig.tar.gz' xft_2.3.2.orig.tar.gz 402454 SHA256:26cdddcc70b187833cbe9dc54df1864ba4c03a7175b2ca9276de9f05dce74507
'http://deb.debian.org/debian/pool/main/x/xft/xft_2.3.2-2.diff.gz' xft_2.3.2-2.diff.gz 10327 SHA256:e94bd505f05507b5691dca9380c2bd4595ba1fd267c09831ab6e3be4bfd87062
```

Other potentially useful URLs:

- https://sources.debian.net/src/xft/2.3.2-2/ (for browsing the source)
- https://sources.debian.net/src/xft/2.3.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xft/2.3.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xxhash=0.8.1-1`

Binary Packages:

- `libxxhash0:amd64=0.8.1-1`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.1-1
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.1-1.dsc' xxhash_0.8.1-1.dsc 1966 SHA256:4a961627c06efc8fa3bc4b06ee9dba6cfaf092f2550b88d63e9218a2728721b4
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.1.orig.tar.gz' xxhash_0.8.1.orig.tar.gz 171552 SHA256:3bb6b7d6f30c591dd65aaaff1c8b7a5b94d81687998ca9400082c739a690436c
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.1-1.debian.tar.xz' xxhash_0.8.1-1.debian.tar.xz 4572 SHA256:d40aa223e90b85435082857b64573541ba9a995841717496e8975aed97241550
```

Other potentially useful URLs:

- https://sources.debian.net/src/xxhash/0.8.1-1/ (for browsing the source)
- https://sources.debian.net/src/xxhash/0.8.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xxhash/0.8.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `zip=3.0-12`

Binary Packages:

- `zip=3.0-12`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zip=3.0-12
'http://deb.debian.org/debian/pool/main/z/zip/zip_3.0-12.dsc' zip_3.0-12.dsc 1328 SHA256:529b19003979b7eae4a305e05d0d9fda81917e2d55a16a6d65588d69380ab80f
'http://deb.debian.org/debian/pool/main/z/zip/zip_3.0.orig.tar.gz' zip_3.0.orig.tar.gz 1118845 SHA256:f0e8bb1f9b7eb0b01285495a2699df3a4b766784c1765a8f1aeedf63c0806369
'http://deb.debian.org/debian/pool/main/z/zip/zip_3.0-12.debian.tar.xz' zip_3.0-12.debian.tar.xz 8628 SHA256:522174080773f72882bd240ca384e698134f61ad6405ce8f995e1d21c9ba41d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/zip/3.0-12/ (for browsing the source)
- https://sources.debian.net/src/zip/3.0-12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zip/3.0-12/ (for access to the source package after it no longer exists in the archive)

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
