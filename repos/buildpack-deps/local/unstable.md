# `buildpack-deps:sid`

## Docker Metadata

- Image ID: `sha256:f1c7083f117725b1c794ae5c9c26d1b9ae5cb2a951f06bd47713bcb72eb9b34f`
- Created: `2020-02-26T01:16:45.124093436Z`
- Virtual Size: ~ 826.74 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-5`

Binary Packages:

- `libacl1:amd64=2.2.53-5`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/acl/2.2.53-5/


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

### `dpkg` source package: `apr-util=1.6.1-4`

Binary Packages:

- `libaprutil1:amd64=1.6.1-4+b1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-4
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1-4.dsc' apr-util_1.6.1-4.dsc 2828 SHA256:2176a12a657b70c030493ad0a068cebc61f99667112a39e17ada10cf689d028d
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2.asc' apr-util_1.6.1.orig.tar.bz2.asc 801 SHA256:47837b605290c0d7659b73734e4a9d5e6c0c24c13185cd4d91837afe63c07ca4
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1-4.debian.tar.xz' apr-util_1.6.1-4.debian.tar.xz 212464 SHA256:44d304947ba9fd62b1d54e5205a41227357d8e0033e7895cba4f2fae7a39b658
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr-util/1.6.1-4/ (for browsing the source)
- https://sources.debian.net/src/apr-util/1.6.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr-util/1.6.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr=1.6.5-1`

Binary Packages:

- `libapr1:amd64=1.6.5-1+b1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.5-1
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.5-1.dsc' apr_1.6.5-1.dsc 2296 SHA256:80c471107d7f90ab5de012e4211559f4f6852ca2b7fd6911f06420aa66d27ec0
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.5.orig.tar.bz2' apr_1.6.5.orig.tar.bz2 855393 SHA256:a67ca9fcf9c4ff59bce7f428a323c8b5e18667fdea7b0ebad47d194371b0a105
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.5.orig.tar.bz2.asc' apr_1.6.5.orig.tar.bz2.asc 801 SHA256:9beff0bb06f4cbbb006176af93258d946d33b7fb54aac13a4c90cfba1cfd0c88
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.6.5-1.debian.tar.xz' apr_1.6.5-1.debian.tar.xz 213168 SHA256:cb03a6ad0b8c525c67744e7d3f7c52af446e73bd6d4eeb6fd4622677df60db2b
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.6.5-1/ (for browsing the source)
- https://sources.debian.net/src/apr/1.6.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.6.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=1.8.4`

Binary Packages:

- `apt=1.8.4`
- `libapt-pkg5.0:amd64=1.8.4`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.8.4
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.8.4.dsc' apt_1.8.4.dsc 2766 SHA256:492d4d6de28a26d46b63ac360c3ea3bcc106970a6521f3812dd86ae33cbeaccc
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.8.4.tar.xz' apt_1.8.4.tar.xz 2188876 SHA256:f40fe4475f3ab775a915569911326ff31c12c09eb8518bd82ba87aa570d6c43e
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/1.8.4/ (for browsing the source)
- https://sources.debian.net/src/apt/1.8.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/1.8.4/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-5.dsc' attr_2.4.48-5.dsc 2433 SHA256:0b20a285b758083e2e202ffdd2930cef1bf84fee498791fc3e26b69a3bced01d
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-5.debian.tar.xz' attr_2.4.48-5.debian.tar.xz 25560 SHA256:02238253d324250dabdc0434f7de045d85df93458995a465ac434f2a3978a312
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.4.48-5/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.4.48-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.4.48-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:2.8.5-2`

Binary Packages:

- `libaudit-common=1:2.8.5-2`
- `libaudit1:amd64=1:2.8.5-2+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.5-2
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.5-2.dsc' audit_2.8.5-2.dsc 2311 SHA256:c3b566cad955fc631f4a17207378e6039169dfeb8b2e7712ec17f422a92955f3
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.5.orig.tar.gz' audit_2.8.5.orig.tar.gz 1140694 SHA256:0e5d4103646e00f8d1981e1cd2faea7a2ae28e854c31a803e907a383c5e2ecb7
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.5-2.debian.tar.xz' audit_2.8.5-2.debian.tar.xz 16304 SHA256:d54bbc862779f872239676ebf9757784144a7c00012bf2769d3b1eb5ff7aca5a
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:2.8.5-2/ (for browsing the source)
- https://sources.debian.net/src/audit/1:2.8.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:2.8.5-2/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-11.1.dsc' autoconf_2.69-11.1.dsc 1735 SHA256:06ab6e617ed8d07eecbc29a1669cd748b7ce11ab457c186e7e8794fe02b231ba
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-11.1.debian.tar.xz' autoconf_2.69-11.1.debian.tar.xz 23488 SHA256:ff76de2fc2956773dc6f47301b66822ea3074a2e556dc2e761cb411342d2228b
```

Other potentially useful URLs:

- https://sources.debian.net/src/autoconf/2.69-11.1/ (for browsing the source)
- https://sources.debian.net/src/autoconf/2.69-11.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autoconf/2.69-11.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `automake-1.16=1:1.16.1-4`

Binary Packages:

- `automake=1:1.16.1-4`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.1-4
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.1-4.dsc' automake-1.16_1.16.1-4.dsc 2274 SHA256:a130f56cbf41534f70f5484e30e8da473fd7d4e3ff1f25f29791bf3bc306214f
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.1.orig.tar.xz' automake-1.16_1.16.1.orig.tar.xz 1534936 SHA256:5d05bb38a23fd3312b10aea93840feec685bdf4a41146e78882848165d3ae921
'http://deb.debian.org/debian/pool/main/a/automake-1.16/automake-1.16_1.16.1-4.debian.tar.xz' automake-1.16_1.16.1-4.debian.tar.xz 14692 SHA256:18641eabde4266f6c0a493b8b3e6796b74a962a5be946463856a2d428df96552
```

Other potentially useful URLs:

- https://sources.debian.net/src/automake-1.16/1:1.16.1-4/ (for browsing the source)
- https://sources.debian.net/src/automake-1.16/1:1.16.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/automake-1.16/1:1.16.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `autotools-dev=20180224.1`

Binary Packages:

- `autotools-dev=20180224.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20180224.1.dsc' autotools-dev_20180224.1.dsc 1643 SHA256:795f558377bf6c90280c293b2711afc094cd1bf6ae486a395e1361ffd242cd2f
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20180224.1.tar.xz' autotools-dev_20180224.1.tar.xz 68256 SHA256:355a4d8461dfedebd2c5194603197712a10f71e20de73a35ab6e90b7acf3e837
```

Other potentially useful URLs:

- https://sources.debian.net/src/autotools-dev/20180224.1/ (for browsing the source)
- https://sources.debian.net/src/autotools-dev/20180224.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autotools-dev/20180224.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=11`

Binary Packages:

- `base-files=11`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_11.dsc' base-files_11.dsc 1063 SHA256:8c3da5c6c17db756e8369ccdef4c706ed3e71d5480ca50fec3fe451073e3d94d
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_11.tar.xz' base-files_11.tar.xz 65368 SHA256:cf610763b6fc4e7f6c066fd6bed1d580f6b0fd9e1f91c26a18900117a3d5622e
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/11/ (for browsing the source)
- https://sources.debian.net/src/base-files/11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.47`

Binary Packages:

- `base-passwd=3.5.47`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.47
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.47.dsc' base-passwd_3.5.47.dsc 1757 SHA256:5a77a4cce51d1eb72e9d96d4083c641435c05888922c7bd3fa6b4395bf9afad3
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.47.tar.xz' base-passwd_3.5.47.tar.xz 53024 SHA256:9810ae0216e96bf9fc7ca6163d47ef8ec7d1677f533451af5911d8202a490a23
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.47/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.47/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.47/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.0-5`

Binary Packages:

- `bash=5.0-5`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/bash/5.0-5/


### `dpkg` source package: `binutils=2.34-3`

Binary Packages:

- `binutils=2.34-3`
- `binutils-common:amd64=2.34-3`
- `binutils-x86-64-linux-gnu=2.34-3`
- `libbinutils:amd64=2.34-3`
- `libctf-nobfd0:amd64=2.34-3`
- `libctf0:amd64=2.34-3`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.34-3
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.34-3.dsc' binutils_2.34-3.dsc 11244 SHA256:dac3a9aa7010e7086ba6c9e4bc2351f88126a1deb5408ceaa93b20698ec7c694
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.34.orig.tar.xz' binutils_2.34.orig.tar.xz 23144772 SHA256:bc79b3cf950e1601257c0056315b5aa2dc073ebec9c2dba292b6ff30eaeb0899
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.34-3.debian.tar.xz' binutils_2.34-3.debian.tar.xz 144748 SHA256:172a8ecafeea5546d5c481c481522ff9a6c33a5bcb7045a326887537829390fa
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.34-3/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.34-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.34-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `brotli=1.0.7-6`

Binary Packages:

- `libbrotli1:amd64=1.0.7-6`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.7-6
'http://deb.debian.org/debian/pool/main/b/brotli/brotli_1.0.7-6.dsc' brotli_1.0.7-6.dsc 2267 SHA256:5fc1691617c3d77056877f67aacb3ffa44462d6cabd16012bc3905881f44edd2
'http://deb.debian.org/debian/pool/main/b/brotli/brotli_1.0.7.orig.tar.gz' brotli_1.0.7.orig.tar.gz 23827908 SHA256:4c61bfb0faca87219ea587326c467b95acb25555b53d1a421ffa3c8a9296ee2c
'http://deb.debian.org/debian/pool/main/b/brotli/brotli_1.0.7-6.debian.tar.xz' brotli_1.0.7-6.debian.tar.xz 4344 SHA256:0717dafec2519f55f4b27f92ada9b5fb2294d8b29f93c3aa4007e4027130147a
```

Other potentially useful URLs:

- https://sources.debian.net/src/brotli/1.0.7-6/ (for browsing the source)
- https://sources.debian.net/src/brotli/1.0.7-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/brotli/1.0.7-6/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-2.dsc' bzip2_1.0.8-2.dsc 2180 SHA256:646cdcbb786a89a647cfafb280ef467143c06c445c4bf6fe69ec4a7882943064
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-2.debian.tar.bz2' bzip2_1.0.8-2.debian.tar.bz2 26032 SHA256:237c8619bc9bc16f357b1077064a3e58aa1a230dadb4b9bb3bd8dc8f454afc0b
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.8-2/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.8-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.8-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20190110`

Binary Packages:

- `ca-certificates=20190110`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20190110.dsc' ca-certificates_20190110.dsc 1805 SHA256:bffbfe63a1ad2a07c6094502f05899c65edba93aefe58682f440e000fc65f6f0
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20190110.tar.xz' ca-certificates_20190110.tar.xz 243472 SHA256:ee4bf0f4c6398005f5b5ca4e0b87b82837ac5c3b0280a1cb3a63c47555c3a675
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20190110/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20190110/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20190110/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cairo=1.16.0-4`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-4`
- `libcairo-script-interpreter2:amd64=1.16.0-4`
- `libcairo2:amd64=1.16.0-4`
- `libcairo2-dev:amd64=1.16.0-4`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-4
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.16.0-4.dsc' cairo_1.16.0-4.dsc 2806 SHA256:cd511a989ea189a15527f0b745196185df71dd3ab7396228cee0709d8b1c9616
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA256:5e7b29b3f113ef870d1e3ecf8adf21f923396401604bda16d44be45e66052331
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.16.0-4.debian.tar.xz' cairo_1.16.0-4.debian.tar.xz 30248 SHA256:e2b4c5aae085857e91de4529c00043997b55bb17ebccd3744bf04ac4ccfd31df
```

Other potentially useful URLs:

- https://sources.debian.net/src/cairo/1.16.0-4/ (for browsing the source)
- https://sources.debian.net/src/cairo/1.16.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cairo/1.16.0-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.251`

Binary Packages:

- `libdebconfclient0:amd64=0.251`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.251
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.251.dsc' cdebconf_0.251.dsc 2743 SHA256:00594d5edbb403baa4290d61eb27f708d16bfe247b5ae64dfeabefd94a2167ff
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.251.tar.xz' cdebconf_0.251.tar.xz 275468 SHA256:0d06addfe6e17e9b52f275e09667d35dd31c8672c7a112c8ba3c8b2255106c94
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.251/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.251/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.251/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.30-3`

Binary Packages:

- `coreutils=8.30-3+b1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.30-3
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.30-3.dsc' coreutils_8.30-3.dsc 1861 SHA256:106031a57a2ab2ba46b61083035e2ccb438c85a2b3506a8198b67868dde1546d
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.30.orig.tar.xz' coreutils_8.30.orig.tar.xz 5359532 SHA256:e831b3a86091496cdba720411f9748de81507798f6130adeaef872d206e1b057
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.30-3.debian.tar.xz' coreutils_8.30-3.debian.tar.xz 32808 SHA256:9179d45fb51d07a8743c4d58464459330eb6d4b489d59641d70c3bd9f579b694
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/8.30-3/ (for browsing the source)
- https://sources.debian.net/src/coreutils/8.30-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/8.30-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.68.0-1`

Binary Packages:

- `curl=7.68.0-1`
- `libcurl3-gnutls:amd64=7.68.0-1`
- `libcurl4:amd64=7.68.0-1`
- `libcurl4-openssl-dev:amd64=7.68.0-1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.68.0-1
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.68.0-1.dsc' curl_7.68.0-1.dsc 2646 SHA256:cdf08a9a1b11246cf051125280f8a039a9e357631ccf2a06dc50bb66f46f284e
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.68.0.orig.tar.gz' curl_7.68.0.orig.tar.gz 4096350 SHA256:1dd7604e418b0b9a9077f62f763f6684c1b092a7bc17e3f354b8ad5c964d7358
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.68.0-1.debian.tar.xz' curl_7.68.0-1.debian.tar.xz 29304 SHA256:fb8f6cd5ce44422a75de12330fdca0e0ce56e81ed89faa7ee24b71a8ba8dd42e
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.68.0-1/ (for browsing the source)
- https://sources.debian.net/src/curl/7.68.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.68.0-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.dsc' cyrus-sasl2_2.1.27+dfsg-2.dsc 3393 SHA256:e7e09491a1c2589c9947164db091d0f9b21b7d122f128841b6eac1adfc51b6c2
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz 99956 SHA256:ee894aeee645e842e39b434d5130e1bd15ea24b84c8eeeea3f5077511a87341a
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.10.2-6`

Binary Packages:

- `dash=0.5.10.2-6`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.10.2-6
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2-6.dsc' dash_0.5.10.2-6.dsc 1756 SHA256:d509a23ebdc4f107c911914590c1400e5a24383f35c5d6904e48d2afeff168ac
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA256:3c663919dc5c66ec991da14c7cf7e0be8ad00f3db73986a987c118862b5f6071
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2-6.debian.tar.xz' dash_0.5.10.2-6.debian.tar.xz 44232 SHA256:1448fbfc2541be52787da81ce03bb81ad6b1f380cba1b7e747abefdcd44f6c86
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.10.2-6/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.10.2-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.10.2-6/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6`
- `libdb5.3-dev=5.3.28+dfsg1-0.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6.dsc' db5.3_5.3.28+dfsg1-0.6.dsc 3138 SHA256:0cd8010ff17180156bc2d91518ca15c4e32bdee7638a1289cdc5c0a803f50279
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6.debian.tar.xz 29196 SHA256:8e7264cfd368d04133a818cdbd3191b874c534f4ad7f83cfdbb3cccf12b5f052
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.6/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.73`

Binary Packages:

- `debconf=1.5.73`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.73
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.73.dsc' debconf_1.5.73.dsc 2081 SHA256:cdd4c049414cd167a4a9479d883e205bf5cebb19fc4bb6f132000a56291eb670
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.73.tar.xz' debconf_1.5.73.tar.xz 570780 SHA256:513895b2b77d9fb72542152390e7d4c67fe1e08de75fdad44d54ce1e7d83ecef
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.73/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.73/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.73/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debian-archive-keyring=2019.1`

Binary Packages:

- `debian-archive-keyring=2019.1`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2019.1
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2019.1.dsc' debian-archive-keyring_2019.1.dsc 1808 SHA256:c41d15f22974aa3c8b2a6535327f8c4b6bdeea050e3bf070c4bc6c4d8860f598
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2019.1.tar.xz' debian-archive-keyring_2019.1.tar.xz 116772 SHA256:cdb12d8b78889593dc9a37f639cbd9efd164cfc058c07b039f74581dc22a4b6e
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2019.1/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2019.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2019.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=4.9.1`

Binary Packages:

- `debianutils=4.9.1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.9.1
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.9.1.dsc' debianutils_4.9.1.dsc 1592 SHA256:d30866ea0352263fa7756010e8743ade350024b2fd491bc5befcbaa9a97626b7
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.9.1.tar.xz' debianutils_4.9.1.tar.xz 157516 SHA256:af826685d9c56abfa873e84cd392539cd363cb0ba04a09d21187377e1b764091
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.9.1/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.9.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.9.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.7-3`

Binary Packages:

- `diffutils=1:3.7-3`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.7-3
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.7-3.dsc' diffutils_3.7-3.dsc 1453 SHA256:99dee94cec05454a65a9cb542bea1720dbd4c511d13f9784c9e3741e76a9b9ba
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz' diffutils_3.7.orig.tar.xz 1448828 SHA256:b3a7a6221c3dc916085f0d205abf6b8e1ba443d4dd965118da364a1dc1cb3a26
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.7-3.debian.tar.xz' diffutils_3.7-3.debian.tar.xz 11116 SHA256:a455228f12283b5f3c0165db4ab9b12071adc37fb9dd50dcb5e1b8851c524f1f
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.7-3/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.7-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.7-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `djvulibre=3.5.27.1-14`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.27.1-14`
- `libdjvulibre-text=3.5.27.1-14`
- `libdjvulibre21:amd64=3.5.27.1-14`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-14
'http://deb.debian.org/debian/pool/main/d/djvulibre/djvulibre_3.5.27.1-14.dsc' djvulibre_3.5.27.1-14.dsc 2406 SHA256:ccb6659a2bbf2ac63223f8dc91b2d59f40ff77c2c25dbb7f6b531c4b2d46bc08
'http://deb.debian.org/debian/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA256:77f07de3f1039aa19eba2eb3170d9ce9a0918ba7b704a59cfaf08f42fcc52144
'http://deb.debian.org/debian/pool/main/d/djvulibre/djvulibre_3.5.27.1-14.debian.tar.xz' djvulibre_3.5.27.1-14.debian.tar.xz 76272 SHA256:72f7680b069de1e51b15098fd6711e15205c62ab388ae5b66afdb29e8cb02300
```

Other potentially useful URLs:

- https://sources.debian.net/src/djvulibre/3.5.27.1-14/ (for browsing the source)
- https://sources.debian.net/src/djvulibre/3.5.27.1-14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/djvulibre/3.5.27.1-14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.19.7`

Binary Packages:

- `dpkg=1.19.7`
- `dpkg-dev=1.19.7`
- `libdpkg-perl=1.19.7`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.7
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.19.7.dsc' dpkg_1.19.7.dsc 2103 SHA256:098b285d5fc7add8972e5b2b3678027bba3f3fe01962e5176db2fbff33bbd8e3
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.19.7.tar.xz' dpkg_1.19.7.tar.xz 4716724 SHA256:4c27fededf620c0aa522fff1a48577ba08144445341257502e7730f2b1a296e8
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.19.7/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.19.7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.19.7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.45.5-2`

Binary Packages:

- `comerr-dev:amd64=2.1-1.45.5-2`
- `e2fsprogs=1.45.5-2`
- `libcom-err2:amd64=1.45.5-2`
- `libext2fs2:amd64=1.45.5-2`
- `libss2:amd64=1.45.5-2`
- `logsave=1.45.5-2`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.5-2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.5-2.dsc' e2fsprogs_1.45.5-2.dsc 2969 SHA256:8aaed11ca66ef98d171db0f6331b8826d6544ca9e4862b762a18730b11f0cd29
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.5.orig.tar.gz' e2fsprogs_1.45.5.orig.tar.gz 7938826 SHA256:91e72a2f6fee21b89624d8ece5a4b3751a17b28775d32cd048921050b4760ed9
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.5.orig.tar.gz.asc' e2fsprogs_1.45.5.orig.tar.gz.asc 488 SHA256:0f900698a89e3e1996cd86966e5ae0dc6f8d866e2cd8a0f4285c23e7ea696720
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.5-2.debian.tar.xz' e2fsprogs_1.45.5-2.debian.tar.xz 80748 SHA256:2b929d6471a3d432a6dc7d632503e609df9c25ba8f9c2d9e0a4735a744bd7b62
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.45.5-2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.45.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.45.5-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `elfutils=0.176-1.1`

Binary Packages:

- `libelf1:amd64=0.176-1.1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.176-1.1
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.176-1.1.dsc' elfutils_0.176-1.1.dsc 2584 SHA256:6d9fa4741e921f58a3e291def1f92a87bed888db15e73d6e29d46fc48b5f615a
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.176.orig.tar.bz2' elfutils_0.176.orig.tar.bz2 8646075 SHA256:eb5747c371b0af0f71e86215a5ebb88728533c3a104a43d4231963f308cd1023
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.176.orig.tar.bz2.asc' elfutils_0.176.orig.tar.bz2.asc 455 SHA256:51474b579b25fc799de0777e241c83605427d2903f8d28524ef6af42f75931fd
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.176-1.1.debian.tar.xz' elfutils_0.176-1.1.debian.tar.xz 31644 SHA256:06d7057e744d3a6138cf43d30237e2b327b6bfe3041a9a4b210414429c1267f1
```

Other potentially useful URLs:

- https://sources.debian.net/src/elfutils/0.176-1.1/ (for browsing the source)
- https://sources.debian.net/src/elfutils/0.176-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/elfutils/0.176-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.9-1`

Binary Packages:

- `libexpat1:amd64=2.2.9-1`
- `libexpat1-dev:amd64=2.2.9-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.9-1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.9-1.dsc' expat_2.2.9-1.dsc 1949 SHA256:58db7b5ac8431570f47921ff545493334d09070a9afab9aaf8282e3c1dfc66ad
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.9.orig.tar.gz' expat_2.2.9.orig.tar.gz 8273174 SHA256:c341ac8c79e021cc3392a6d76e138e62d1dd287592cb455148540331756a2208
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.9-1.debian.tar.xz' expat_2.2.9-1.debian.tar.xz 10740 SHA256:85d13af9777815b77a478044604902d9a04eb05f4f0dbcaedcbe1193670239d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.9-1/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.9-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/f/file/file_5.38-4.dsc' file_5.38-4.dsc 2237 SHA256:d84b2734b112384230e3678beb1c8c5d3a17d4cdec8b6ef21304f2c0b72fda26
'http://deb.debian.org/debian/pool/main/f/file/file_5.38.orig.tar.gz' file_5.38.orig.tar.gz 932528 SHA256:593c2ffc2ab349c5aea0f55fedfe4d681737b6b62376a9b3ad1e77b2cc19fa34
'http://deb.debian.org/debian/pool/main/f/file/file_5.38.orig.tar.gz.asc' file_5.38.orig.tar.gz.asc 169 SHA256:b9c78e39970abda091ec8752401f5241349cef4709a2e1267a378f7ab25115d8
'http://deb.debian.org/debian/pool/main/f/file/file_5.38-4.debian.tar.xz' file_5.38-4.debian.tar.xz 34488 SHA256:b9dfd0dd070ee17a6cc69ecf4d61c329b3f567ca16fdc121f3b31d0111df9381
```

Other potentially useful URLs:

- https://sources.debian.net/src/file/1:5.38-4/ (for browsing the source)
- https://sources.debian.net/src/file/1:5.38-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/file/1:5.38-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.7.0-1`

Binary Packages:

- `findutils=4.7.0-1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.7.0-1
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0-1.dsc' findutils_4.7.0-1.dsc 2302 SHA256:867867005890a464599024bbc9d3bbc82493e255ca812a906112b9a5eda15169
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz' findutils_4.7.0.orig.tar.xz 1895048 SHA256:c5fefbdf9858f7e4feb86f036e1247a54c79fc2d8e4b7064d5aaa1f47dfa789a
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz.asc' findutils_4.7.0.orig.tar.xz.asc 488 SHA256:2f620e6d941e241fac52344a89149ab1ffeefb0fb9e42174e17a508d59a31d0f
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0-1.debian.tar.xz' findutils_4.7.0-1.debian.tar.xz 27536 SHA256:3503f8ff7b1020c140055fbe06f107c73cd827f50761cf9a3c5296f6890bf0af
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.7.0-1/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.7.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.7.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fontconfig=2.13.1-2`

Binary Packages:

- `fontconfig=2.13.1-2+b1`
- `fontconfig-config=2.13.1-2`
- `libfontconfig1:amd64=2.13.1-2+b1`
- `libfontconfig1-dev:amd64=2.13.1-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-2
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.13.1-2.dsc' fontconfig_2.13.1-2.dsc 2185 SHA256:4c9ee914941b8f129ab54a13ecc889eb3165588bf4a7b3ae049226c7972ac486
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA256:f655dd2a986d7aa97e052261b36aa67b0a64989496361eca8d604e6414006741
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.13.1-2.debian.tar.xz' fontconfig_2.13.1-2.debian.tar.xz 53600 SHA256:9da208343c570b2e8d48c6c8b4cf49b0647ae334df505b2ec6a171e73453e498
```

Other potentially useful URLs:

- https://sources.debian.net/src/fontconfig/2.13.1-2/ (for browsing the source)
- https://sources.debian.net/src/fontconfig/2.13.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fontconfig/2.13.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fonts-dejavu=2.37-1`

Binary Packages:

- `fonts-dejavu-core=2.37-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-1
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.dsc' fonts-dejavu_2.37-1.dsc 2575 SHA256:f35ff7b2c8dbfda6564c9dedf088ba06cc6d279fdd8e7cccbd1ae08ded1bb71c
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.debian.tar.xz' fonts-dejavu_2.37-1.debian.tar.xz 10424 SHA256:5105cdbfc086f4a83ab6871eb39cc904bf02aa52762402b7cacf33d0938122f7
```

Other potentially useful URLs:

- https://sources.debian.net/src/fonts-dejavu/2.37-1/ (for browsing the source)
- https://sources.debian.net/src/fonts-dejavu/2.37-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fonts-dejavu/2.37-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `freetype=2.10.1-2`

Binary Packages:

- `libfreetype-dev:amd64=2.10.1-2`
- `libfreetype6:amd64=2.10.1-2`
- `libfreetype6-dev:amd64=2.10.1-2`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `FSFUL`
- `FSFULLR`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `MPL-1.1`
- `OFL-1.1`
- `OpenGroup-BSD-like`
- `Permissive`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.10.1-2
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1-2.dsc' freetype_2.10.1-2.dsc 3749 SHA256:3515097c45d05c7f82f8636a7fa65c12ed70868affbc270fe6788bf61b5d4cd8
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1.orig-ft2demos.tar.gz' freetype_2.10.1.orig-ft2demos.tar.gz 305328 SHA256:5e9e94a2db9d1a945293a1644a502f6664a2173a454d4a55b19695e2e2f4a0bc
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1.orig-ft2demos.tar.gz.asc' freetype_2.10.1.orig-ft2demos.tar.gz.asc 195 SHA256:ccee51c4b4101b89a66ba5f2bdd54d127e93e120086982db57fa33761f310e9e
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1.orig-ft2docs.tar.gz' freetype_2.10.1.orig-ft2docs.tar.gz 2123885 SHA256:a4e4a8e69c7bf833eba7c158254a572fd43131d5e9b8791bd2ecbb03546ce155
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1.orig-ft2docs.tar.gz.asc' freetype_2.10.1.orig-ft2docs.tar.gz.asc 195 SHA256:aaedd84036d9e615fbb5acf71081dd05c9d7333686593432e445ee89655a79c9
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1.orig.tar.gz' freetype_2.10.1.orig.tar.gz 3478158 SHA256:3a60d391fd579440561bf0e7f31af2222bc610ad6ce4d9d7bd2165bca8669110
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1.orig.tar.gz.asc' freetype_2.10.1.orig.tar.gz.asc 195 SHA256:3952cc2651536ef5157601143d1efc453a7fe5ca64eaf765d034c417aabd4210
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.1-2.debian.tar.xz' freetype_2.10.1-2.debian.tar.xz 114884 SHA256:3d1405fe90e17ee290e06f4fd65a16ff38d9f9604aff12c40a0574edb3dbbe62
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.10.1-2/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.10.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.10.1-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gcc-10=10-20200222-1`

Binary Packages:

- `gcc-10-base:amd64=10-20200222-1`
- `libatomic1:amd64=10-20200222-1`
- `libcc1-0:amd64=10-20200222-1`
- `libgcc-s1:amd64=10-20200222-1`
- `libgcc1=1:10-20200222-1`
- `libgomp1:amd64=10-20200222-1`
- `libitm1:amd64=10-20200222-1`
- `liblsan0:amd64=10-20200222-1`
- `libquadmath0:amd64=10-20200222-1`
- `libstdc++6:amd64=10-20200222-1`
- `libtsan0:amd64=10-20200222-1`
- `libubsan1:amd64=10-20200222-1`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10-20200222-1
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10-20200222-1.dsc' gcc-10_10-20200222-1.dsc 27973 SHA256:2bc097210263b7fc706933aaad5084fc3078fd0aca1bdd863db34a2d8796b4bf
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10-20200222.orig.tar.gz' gcc-10_10-20200222.orig.tar.gz 75848571 SHA256:35647e1a11870a542dca6c8b1cdd84a91f6fd6059d9fe55286d1b061c055b790
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10-20200222-1.debian.tar.xz' gcc-10_10-20200222-1.debian.tar.xz 556632 SHA256:fb0399fee90b3e31e6debbac64fb7e21ebf4ab9d5e9e59a1ab465a507dd5430d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-10/10-20200222-1/ (for browsing the source)
- https://sources.debian.net/src/gcc-10/10-20200222-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-10/10-20200222-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-9=9.2.1-30`

Binary Packages:

- `cpp-9=9.2.1-30`
- `g++-9=9.2.1-30`
- `gcc-9=9.2.1-30`
- `gcc-9-base:amd64=9.2.1-30`
- `libasan5:amd64=9.2.1-30`
- `libgcc-9-dev:amd64=9.2.1-30`
- `libstdc++-9-dev:amd64=9.2.1-30`

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
$ apt-get source -qq --print-uris gcc-9=9.2.1-30
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.2.1-30.dsc' gcc-9_9.2.1-30.dsc 22431 SHA256:7de087464ba3d24e69c016b458c832bae35ac0aadbb08917f75e01968f24d61d
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.2.1.orig.tar.gz' gcc-9_9.2.1.orig.tar.gz 92887421 SHA256:f259d1c6344f5d89fee3a182d7a211925f507d477d3659d53ac64c76cea8bb11
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.2.1-30.debian.tar.xz' gcc-9_9.2.1-30.debian.tar.xz 988772 SHA256:7e442ef60948e6738bacdeb8941d7ff8aa70c83bc69cd427c89bbea745ef357a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-9/9.2.1-30/ (for browsing the source)
- https://sources.debian.net/src/gcc-9/9.2.1-30/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-9/9.2.1-30/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-defaults=1.185.1`

Binary Packages:

- `cpp=4:9.2.1-3.1`
- `g++=4:9.2.1-3.1`
- `gcc=4:9.2.1-3.1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.185.1
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.185.1.dsc' gcc-defaults_1.185.1.dsc 11989 SHA256:471b39e0d91871f9b0054b8d3d2f7c27c190fc751f46a1c7c7ecdcba6de7aa4d
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.185.1.tar.gz' gcc-defaults_1.185.1.tar.gz 54512 SHA256:6e1bbc04f51b63cb0a8ac26c635c9f0e9a3a45f5d01b013b1946bb0c42e6cc77
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-defaults/1.185.1/ (for browsing the source)
- https://sources.debian.net/src/gcc-defaults/1.185.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-defaults/1.185.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.18.1-5`

Binary Packages:

- `libgdbm-compat4:amd64=1.18.1-5`
- `libgdbm-dev:amd64=1.18.1-5`
- `libgdbm6:amd64=1.18.1-5`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.18.1-5
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1-5.dsc' gdbm_1.18.1-5.dsc 2635 SHA256:4c0c4498378c673c9d2d8dfb5b319a4830d2dd21e65faaaa8e0f09cb7f71606b
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz' gdbm_1.18.1.orig.tar.gz 941863 SHA256:86e613527e5dba544e73208f42b78b7c022d4fa5a6d5498bf18c8d6f745b91dc
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz.asc' gdbm_1.18.1.orig.tar.gz.asc 412 SHA256:3254738e7689e44ac65e78a766806828b8282e6bb1c0e5bb6156a99e567889a5
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1-5.debian.tar.xz' gdbm_1.18.1-5.debian.tar.xz 16348 SHA256:3c1a0e05b40a97ee51ce77c736c72c37738ba31b2720111d3bc99175a2c3a3ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.18.1-5/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.18.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.18.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdk-pixbuf=2.40.0+dfsg-2`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.40.0+dfsg-2`
- `libgdk-pixbuf2.0-0:amd64=2.40.0+dfsg-2`
- `libgdk-pixbuf2.0-bin=2.40.0+dfsg-2`
- `libgdk-pixbuf2.0-common=2.40.0+dfsg-2`
- `libgdk-pixbuf2.0-dev:amd64=2.40.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.40.0+dfsg-2
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-2.dsc' gdk-pixbuf_2.40.0+dfsg-2.dsc 3055 SHA256:0932d7d1f8cada563aeb1bb766d5de55286a34c09a4248f0fdd5202e2770035d
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg.orig.tar.xz' gdk-pixbuf_2.40.0+dfsg.orig.tar.xz 5626144 SHA256:bdb3820005dc3c02ec8b1e2916a1d060f65f44d30ba48ab88704c3380d5a47b8
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-2.debian.tar.xz' gdk-pixbuf_2.40.0+dfsg-2.debian.tar.xz 17236 SHA256:d21d7d6cf39c6a921a475e6038e9fba96a54890063c708dd5b0e46735bcbe3d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdk-pixbuf/2.40.0+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/gdk-pixbuf/2.40.0+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdk-pixbuf/2.40.0+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.25.1-1`

Binary Packages:

- `git=1:2.25.1-1`
- `git-man=1:2.25.1-1`

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
$ apt-get source -qq --print-uris git=1:2.25.1-1
'http://deb.debian.org/debian/pool/main/g/git/git_2.25.1-1.dsc' git_2.25.1-1.dsc 2860 SHA256:32e936cf974b36b0868f2430cfa9d818c89a4871560744bc9d54c70651f0e17e
'http://deb.debian.org/debian/pool/main/g/git/git_2.25.1.orig.tar.xz' git_2.25.1.orig.tar.xz 5875548 SHA256:222796cc6e3bf2f9fd765f8f097daa3c3999bb7865ac88a8c974d98182e29f26
'http://deb.debian.org/debian/pool/main/g/git/git_2.25.1-1.debian.tar.xz' git_2.25.1-1.debian.tar.xz 637500 SHA256:aa08f0b28fc95e0172e7419e1de61dea2bc12b469a19db71d289a8cba3eb700c
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.25.1-1/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.25.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.25.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.62.5-1`

Binary Packages:

- `libglib2.0-0:amd64=2.62.5-1`
- `libglib2.0-bin=2.62.5-1`
- `libglib2.0-data=2.62.5-1`
- `libglib2.0-dev:amd64=2.62.5-1`
- `libglib2.0-dev-bin=2.62.5-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.62.5-1
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.62.5-1.dsc' glib2.0_2.62.5-1.dsc 3444 SHA256:152bcee5717e85c23b056b110f0d37338d02639c06327951dd54e8144779acc4
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.62.5.orig.tar.xz' glib2.0_2.62.5.orig.tar.xz 4702492 SHA256:b8d1cdafa46658b63d7512efbe2cd21bd36cd7be83140e44930c47b79f82452e
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.62.5-1.debian.tar.xz' glib2.0_2.62.5-1.debian.tar.xz 92412 SHA256:6ea8bfecc89dd4bfe6bfc1c35f93396d9a352be40fab586d1ab374360cc269c9
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.62.5-1/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.62.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.62.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.29-10`

Binary Packages:

- `libc-bin=2.29-10`
- `libc-dev-bin=2.29-10`
- `libc6:amd64=2.29-10`
- `libc6-dev:amd64=2.29-10`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.29-10
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.29-10.dsc' glibc_2.29-10.dsc 8739 SHA256:4365adda24264fd57faabafd0429a5f123635790fc6391d8abc2ecc15072f2b3
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.29.orig.tar.xz' glibc_2.29.orig.tar.xz 17103228 SHA256:c1eb5652c94680cb40bad4393b06d838237645f0f5760b8d0e6a98a1463e09f3
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.29-10.debian.tar.xz' glibc_2.29-10.debian.tar.xz 868696 SHA256:d66ef632e204670b237b8f1a9e76e1aa9e7d5fc96d271f33128a10474740ea62
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.29-10/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.29-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.29-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.0+dfsg-4`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.0+dfsg-4`
- `libgmp10:amd64=2:6.2.0+dfsg-4`
- `libgmpxx4ldbl:amd64=2:6.2.0+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.0+dfsg-4
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.0+dfsg-4.dsc' gmp_6.2.0+dfsg-4.dsc 2144 SHA256:4ca8c5bca982c78eb7679256a5d41b2c9363a6c3e3ee15ed765515bc328e9989
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.0+dfsg.orig.tar.xz' gmp_6.2.0+dfsg.orig.tar.xz 1842912 SHA256:5d7610449498a79aa62d4b9a8f6baaef91b8716726e1009e02b879962dff32ab
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.0+dfsg-4.debian.tar.xz' gmp_6.2.0+dfsg-4.debian.tar.xz 21120 SHA256:a0772595583dbcf2147e8457602ccf4b524b18227d6804c4a74050df64ece912
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.0+dfsg-4/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.0+dfsg-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.0+dfsg-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.19-1`

Binary Packages:

- `dirmngr=2.2.19-1`
- `gnupg=2.2.19-1`
- `gnupg-l10n=2.2.19-1`
- `gnupg-utils=2.2.19-1`
- `gpg=2.2.19-1`
- `gpg-agent=2.2.19-1`
- `gpg-wks-client=2.2.19-1`
- `gpg-wks-server=2.2.19-1`
- `gpgconf=2.2.19-1`
- `gpgsm=2.2.19-1`
- `gpgv=2.2.19-1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gnupg2/2.2.19-1/


### `dpkg` source package: `gnutls28=3.6.12-2`

Binary Packages:

- `libgnutls-dane0:amd64=3.6.12-2`
- `libgnutls-openssl27:amd64=3.6.12-2`
- `libgnutls28-dev:amd64=3.6.12-2`
- `libgnutls30:amd64=3.6.12-2`
- `libgnutlsxx28:amd64=3.6.12-2`

Licenses: (parsed from: `/usr/share/doc/libgnutls-dane0/copyright`, `/usr/share/doc/libgnutls-openssl27/copyright`, `/usr/share/doc/libgnutls28-dev/copyright`, `/usr/share/doc/libgnutls30/copyright`, `/usr/share/doc/libgnutlsxx28/copyright`)

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
$ apt-get source -qq --print-uris gnutls28=3.6.12-2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.12-2.dsc' gnutls28_3.6.12-2.dsc 3479 SHA256:79f63f438da4f770a38933620a294e48aecd3d03ea98a94cfc16a8305c299e99
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.12.orig.tar.xz' gnutls28_3.6.12.orig.tar.xz 5942064 SHA256:bfacf16e342949ffd977a9232556092c47164bd26e166736cf3459a870506c4b
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.12.orig.tar.xz.asc' gnutls28_3.6.12.orig.tar.xz.asc 488 SHA256:5dbf3c4e473dfc45268a524298be83210aeec09a1d2b6bf15d31ae1c1d1e8333
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.12-2.debian.tar.xz' gnutls28_3.6.12-2.debian.tar.xz 60708 SHA256:52ab28b6d3c344fb830e02f7f669bcd7663ce0a677fe28fc78003e5949ec9443
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.6.12-2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.6.12-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.6.12-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gobject-introspection=1.62.0-5`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.62.0-5`
- `gir1.2-glib-2.0:amd64=1.62.0-5`
- `libgirepository-1.0-1:amd64=1.62.0-5`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.62.0-5
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.62.0-5.dsc' gobject-introspection_1.62.0-5.dsc 3046 SHA256:6eb4e0c04a9b223fde9a880200a6f7b4d7c38c02fd870aa1d240039b9e7b371c
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.62.0.orig.tar.xz' gobject-introspection_1.62.0.orig.tar.xz 980732 SHA256:b1ee7ed257fdbc008702bdff0ff3e78a660e7e602efa8f211dc89b9d1e7d90a2
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.62.0-5.debian.tar.xz' gobject-introspection_1.62.0-5.debian.tar.xz 22692 SHA256:757d4d648ff2ff681ac7742da87c2372fb277c22bb793528419c5209f993270d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gobject-introspection/1.62.0-5/ (for browsing the source)
- https://sources.debian.net/src/gobject-introspection/1.62.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gobject-introspection/1.62.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `graphite2=1.3.13-11`

Binary Packages:

- `libgraphite2-3:amd64=1.3.13-11`

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
$ apt-get source -qq --print-uris graphite2=1.3.13-11
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.13-11.dsc' graphite2_1.3.13-11.dsc 2587 SHA256:cfd46b34cf1a33e2c54be2815c17573b68fe567362b4fdb4f19f841271302691
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.13.orig.tar.gz' graphite2_1.3.13.orig.tar.gz 6664941 SHA256:2f9f609deeddfe2b193502adc8df3b0396694b799a433c36e85fd1242e654cd9
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.13-11.debian.tar.xz' graphite2_1.3.13-11.debian.tar.xz 12068 SHA256:ecac95e52d550a271ec5c506489c82c1561301c641df3caf0048ea0d572abc11
```

Other potentially useful URLs:

- https://sources.debian.net/src/graphite2/1.3.13-11/ (for browsing the source)
- https://sources.debian.net/src/graphite2/1.3.13-11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/graphite2/1.3.13-11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.4-1`

Binary Packages:

- `grep=3.4-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.4-1
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4-1.dsc' grep_3.4-1.dsc 1674 SHA256:785f527cede9631f075bdd6c7f35e65e6b82897d009682766cf35839a393277d
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4.orig.tar.xz' grep_3.4.orig.tar.xz 1555820 SHA256:58e6751c41a7c25bfc6e9363a41786cff3ba5709cf11d5ad903cf7cce31cc3fb
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4.orig.tar.xz.asc' grep_3.4.orig.tar.xz.asc 833 SHA256:4c1871ff6b79c5e5ce0a192272c171d06ec20762b4b258688b1ca2e47d94b23e
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4-1.debian.tar.xz' grep_3.4-1.debian.tar.xz 104364 SHA256:582d181804ce72fcfc4c6a9f13ea1dd73ad04c2723b5da346b69ee5cd24a7d08
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.4-1/ (for browsing the source)
- https://sources.debian.net/src/grep/3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.9-3`

Binary Packages:

- `gzip=1.9-3+b1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.9-3
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.9-3.dsc' gzip_1.9-3.dsc 1960 SHA256:fb4702653d4d5475db22dc5cb054b7321b9dc2ca2067540e31d9460bc11246c2
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.9.orig.tar.gz' gzip_1.9.orig.tar.gz 1181937 SHA256:5d2d3a3432ef32f24cdb060d278834507b481a75adeca18850c73592f778f6ad
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.9-3.debian.tar.xz' gzip_1.9-3.debian.tar.xz 14420 SHA256:45996a08643cad9339a30606c9f523984b2f421c6d58e5949471efab75c1ac52
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.9-3/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.9-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.9-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `harfbuzz=2.6.4-1`

Binary Packages:

- `libharfbuzz0b:amd64=2.6.4-1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.6.4-1
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.6.4-1.dsc' harfbuzz_2.6.4-1.dsc 2308 SHA256:a4d3170871ae826d1a482ca483f7f0af573461b134db30993b481b7607ca17b0
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.6.4.orig.tar.xz' harfbuzz_2.6.4.orig.tar.xz 5967468 SHA256:9413b8d96132d699687ef914ebb8c50440efc87b3f775d25856d7ec347c03c12
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.6.4-1.debian.tar.xz' harfbuzz_2.6.4-1.debian.tar.xz 10960 SHA256:e5c4247ff445f239690edced9948caeb3a66fcdc66b160030448d73c00f19fbe
```

Other potentially useful URLs:

- https://sources.debian.net/src/harfbuzz/2.6.4-1/ (for browsing the source)
- https://sources.debian.net/src/harfbuzz/2.6.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/harfbuzz/2.6.4-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `icu=63.2-2`

Binary Packages:

- `icu-devtools=63.2-2`
- `libicu-dev:amd64=63.2-2`
- `libicu63:amd64=63.2-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=63.2-2
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.2-2.dsc' icu_63.2-2.dsc 1965 SHA256:b11e7fb65cce3bf22e7549c8291a5e058171a8eaf9e37ca8c30b45971e4ad97f
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.2.orig.tar.xz' icu_63.2.orig.tar.xz 13630108 SHA256:ab79c7bf11eacc0e3368b29ebba5cff67f41860a522f6a3957377353d5bc8d71
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.2-2.debian.tar.xz' icu_63.2-2.debian.tar.xz 34300 SHA256:2a9fb8ab29527e985b24dc7b15dd116be0b4a2edd9f106dca77c6f75b9baab7d
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/63.2-2/ (for browsing the source)
- https://sources.debian.net/src/icu/63.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/63.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ilmbase=2.3.0-6`

Binary Packages:

- `libilmbase-dev:amd64=2.3.0-6`
- `libilmbase24:amd64=2.3.0-6`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase24/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.3.0-6
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.3.0-6.dsc' ilmbase_2.3.0-6.dsc 2473 SHA256:1651b6968fdca9a273be866b7ab6aa887f6b916ab48f160bae5a79d83f87fe58
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.3.0.orig.tar.gz' ilmbase_2.3.0.orig.tar.gz 596749 SHA256:0ea21166799bbdd920e7a38a7026236566aafdd6e8638f54c9da1af2219fae82
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.3.0.orig.tar.gz.asc' ilmbase_2.3.0.orig.tar.gz.asc 566 SHA256:c7ee3f4432322d4f7c63dd1b0ca2188a8d1c4a018821c3c12a3d9db746b54bee
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_2.3.0-6.debian.tar.xz' ilmbase_2.3.0-6.debian.tar.xz 14184 SHA256:58c947fd6ff46a5a71564f70fd69f2df19bd139c428c8019c4f8a088c50358f1
```

Other potentially useful URLs:

- https://sources.debian.net/src/ilmbase/2.3.0-6/ (for browsing the source)
- https://sources.debian.net/src/ilmbase/2.3.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ilmbase/2.3.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1`

Binary Packages:

- `imagemagick=8:6.9.10.23+dfsg-2.1+b2`
- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1`
- `imagemagick-6.q16=8:6.9.10.23+dfsg-2.1+b2`
- `libmagickcore-6-arch-config:amd64=8:6.9.10.23+dfsg-2.1+b2`
- `libmagickcore-6-headers=8:6.9.10.23+dfsg-2.1`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1+b2`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.10.23+dfsg-2.1+b2`
- `libmagickcore-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1+b2`
- `libmagickcore-dev=8:6.9.10.23+dfsg-2.1`
- `libmagickwand-6-headers=8:6.9.10.23+dfsg-2.1`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1+b2`
- `libmagickwand-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1+b2`
- `libmagickwand-dev=8:6.9.10.23+dfsg-2.1`

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.10.23+dfsg-2.1
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1.dsc' imagemagick_6.9.10.23+dfsg-2.1.dsc 5285 SHA256:b926af69cf3e16be391ad6b87e8b9411cf3490910d1d07cdc1fb31aafebb8be4
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg.orig.tar.xz' imagemagick_6.9.10.23+dfsg.orig.tar.xz 9081188 SHA256:44249112b624f2cc315573fa96685e547da27ebb321432259290c407023c531e
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1.debian.tar.xz' imagemagick_6.9.10.23+dfsg-2.1.debian.tar.xz 222844 SHA256:11d75c3143aabc281d714b2a4b060e59fc2c787eff1319d50b67f505bf463f48
```

Other potentially useful URLs:

- https://sources.debian.net/src/imagemagick/8:6.9.10.23+dfsg-2.1/ (for browsing the source)
- https://sources.debian.net/src/imagemagick/8:6.9.10.23+dfsg-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/imagemagick/8:6.9.10.23+dfsg-2.1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.57.dsc' init-system-helpers_1.57.dsc 1896 SHA256:88bb5af040c99f010b6d6947ff5c80ae4863ff787e0eeae91e99dcd15a10dbb8
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.57.tar.xz' init-system-helpers_1.57.tar.xz 40460 SHA256:e9d83fd8756a42666fb5d19a8835813823295846659b4e58f138bb9b54e9f5dd
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.57/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.57/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.57/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iproute2=5.5.0-1`

Binary Packages:

- `iproute2=5.5.0-1`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris iproute2=5.5.0-1
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_5.5.0-1.dsc' iproute2_5.5.0-1.dsc 1833 SHA256:2752a4084366fd76bac502838e01626ec9a0df6869338494955d1afdb0808e76
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_5.5.0.orig.tar.xz' iproute2_5.5.0.orig.tar.xz 747756 SHA256:bac543435cac208a11db44c9cc8e35aa902befef8750594654ee71941c388f7b
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_5.5.0-1.debian.tar.xz' iproute2_5.5.0-1.debian.tar.xz 144400 SHA256:33b6ba2e5acee2401f66049618b5fc5a26c92f9bd5972fd86fc7fc492cf886e9
```

Other potentially useful URLs:

- https://sources.debian.net/src/iproute2/5.5.0-1/ (for browsing the source)
- https://sources.debian.net/src/iproute2/5.5.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iproute2/5.5.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iptables=1.8.4-3`

Binary Packages:

- `libxtables12:amd64=1.8.4-3`

Licenses: (parsed from: `/usr/share/doc/libxtables12/copyright`)

- `Artistic`
- `GPL-2`
- `GPL-2+`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris iptables=1.8.4-3
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.4-3.dsc' iptables_1.8.4-3.dsc 2719 SHA256:0d0c9ae69f984d7ad8aef1f4361e56b01dfbb3908f2640644b02c62c0623f723
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.4.orig.tar.bz2' iptables_1.8.4.orig.tar.bz2 704312 SHA256:993a3a5490a544c2cbf2ef15cf7e7ed21af1845baf228318d5c36ef8827e157c
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.4-3.debian.tar.xz' iptables_1.8.4-3.debian.tar.xz 65296 SHA256:1d7018909d55f4f578f811ee5eff7591d91af79a6283a947d1c8c2c5f5a4ffab
```

Other potentially useful URLs:

- https://sources.debian.net/src/iptables/1.8.4-3/ (for browsing the source)
- https://sources.debian.net/src/iptables/1.8.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iptables/1.8.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iputils=3:20190709-3`

Binary Packages:

- `iputils-ping=3:20190709-3`

Licenses: (parsed from: `/usr/share/doc/iputils-ping/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris iputils=3:20190709-3
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20190709-3.dsc' iputils_20190709-3.dsc 2081 SHA256:e169a409efd0238b6c547ffad7de017d402a8506ac9162559de523e884ed0efc
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20190709.orig.tar.xz' iputils_20190709.orig.tar.xz 361144 SHA256:bec0321ee1489c8f73e88f7d34b6fd40fbec7b3af5b3a1940306bd8d8835c3c0
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20190709-3.debian.tar.xz' iputils_20190709-3.debian.tar.xz 13816 SHA256:34c3ec0b516db540a748f0934ba2ada6b8c99379941016b26a6fb065be70fb13
```

Other potentially useful URLs:

- https://sources.debian.net/src/iputils/3:20190709-3/ (for browsing the source)
- https://sources.debian.net/src/iputils/3:20190709-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iputils/3:20190709-3/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.22.1-1.dsc' isl_0.22.1-1.dsc 1860 SHA256:9e9925317ef448cf679040edb6572a2874d497f758b613d9fc633bdafab197cb
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.22.1.orig.tar.xz' isl_0.22.1.orig.tar.xz 1676948 SHA256:28658ce0f0bdb95b51fd2eb15df24211c53284f6ca2ac5e897acc3169e55b60f
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.22.1-1.debian.tar.xz' isl_0.22.1-1.debian.tar.xz 25252 SHA256:bbeb62cfc95e51c25448e127c29fa8ac8009a6f471861de28f326bab2404a406
```

Other potentially useful URLs:

- https://sources.debian.net/src/isl/0.22.1-1/ (for browsing the source)
- https://sources.debian.net/src/isl/0.22.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/isl/0.22.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `krb5=1.17-6`

Binary Packages:

- `krb5-multidev:amd64=1.17-6`
- `libgssapi-krb5-2:amd64=1.17-6`
- `libgssrpc4:amd64=1.17-6`
- `libk5crypto3:amd64=1.17-6`
- `libkadm5clnt-mit11:amd64=1.17-6`
- `libkadm5srv-mit11:amd64=1.17-6`
- `libkdb5-9:amd64=1.17-6`
- `libkrb5-3:amd64=1.17-6`
- `libkrb5-dev:amd64=1.17-6`
- `libkrb5support0:amd64=1.17-6`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit11/copyright`, `/usr/share/doc/libkadm5srv-mit11/copyright`, `/usr/share/doc/libkdb5-9/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-6
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.17-6.dsc' krb5_1.17-6.dsc 3173 SHA256:413a7eea29e609ebcb622308da9e2dd98a3a73861f5ee52b121c2f32ee9d2abf
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA256:5a6e2284a53de5702d3dc2be3b9339c963f9b5397d3fbbc53beb249380a781f5
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.17-6.debian.tar.xz' krb5_1.17-6.debian.tar.xz 143328 SHA256:0419148ef3a7908dad511eca3d9127b318ac1b697a67f719e19a1ff380c00086
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.17-6/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.17-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.17-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.9-4`

Binary Packages:

- `liblcms2-2:amd64=2.9-4`
- `liblcms2-dev:amd64=2.9-4`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.9-4
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.9-4.dsc' lcms2_2.9-4.dsc 1956 SHA256:6db871353515693e8813911a8f81668b92e8c09fa9e6752e701fa8b14247775d
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.9.orig.tar.gz' lcms2_2.9.orig.tar.gz 10974649 SHA256:48c6fdf98396fa245ed86e622028caf49b96fa22f3e5734f853f806fbc8e7d20
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.9-4.debian.tar.xz' lcms2_2.9-4.debian.tar.xz 10748 SHA256:3dd811c431bed101269937299d28708dfe91f32070cf9786680bec26f408b65b
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.9-4/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.9-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.9-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.5.3-7`

Binary Packages:

- `libassuan0:amd64=2.5.3-7`

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
$ apt-get source -qq --print-uris libassuan=2.5.3-7
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3-7.dsc' libassuan_2.5.3-7.dsc 2014 SHA256:f23373705283a028f78b8286e662c563fdbb520fab46f3e679023821653bf2fa
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA256:91bcb0403866b4e7c4bc1cc52ed4c364a9b5414b3994f718c70303f7f765e702
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA256:53b16a6619a2690b4f22da645a1d0c14b5664825c87b165ca5bd0de32607888a
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3-7.debian.tar.xz' libassuan_2.5.3-7.debian.tar.xz 13732 SHA256:6a617dab31e06d3db0258e90f3ec87531978d4c28fd0c00f92641fae1d3ebb45
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.3-7/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.3-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.3-7/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0-1.dsc' libbsd_0.10.0-1.dsc 2197 SHA256:7c05e2c73658f64cbd4e1762b716cc7c4c1d68391191e82c7d266a351430edd6
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz' libbsd_0.10.0.orig.tar.xz 393576 SHA256:34b8adc726883d0e85b3118fa13605e179a62b31ba51f676136ecb2d0bc1a887
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz.asc' libbsd_0.10.0.orig.tar.xz.asc 833 SHA256:4362f6d811ffc06659ac5cf777d8d01157bedfc28720b41fb485afb0a5acc0c7
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0-1.debian.tar.xz' libbsd_0.10.0-1.debian.tar.xz 16660 SHA256:4cf37d6d5b72702b31b07384612e07173e94e081feef71fec206f86ab38f2411
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.10.0-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.10.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.10.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.7.9-2.1`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.1+b1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.1
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.1.dsc' libcap-ng_0.7.9-2.1.dsc 2109 SHA256:eb2c6bc4c96d0b80a3b36963c94763a1675567c38248a3313492b1e5414427d0
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.1.debian.tar.xz' libcap-ng_0.7.9-2.1.debian.tar.xz 6204 SHA256:529f686a5af51b999ad96ee3166445ffcb9c221af10f36e5c7fd7f3bf61154d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap-ng/0.7.9-2.1/ (for browsing the source)
- https://sources.debian.net/src/libcap-ng/0.7.9-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap-ng/0.7.9-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap2=1:2.32-1`

Binary Packages:

- `libcap2:amd64=1:2.32-1`
- `libcap2-bin=1:2.32-1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.32-1
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.32-1.dsc' libcap2_2.32-1.dsc 2197 SHA256:7753a4dd83fca414a014579005d91653d71e95adfdbfd8d6c5c833f2372eb6da
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.32.orig.tar.xz' libcap2_2.32.orig.tar.xz 99708 SHA256:1005e3d227f2340ad1e3360ef8b69d15e3c72a29c09f4894d7aac038bd26e2be
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.32-1.debian.tar.xz' libcap2_2.32-1.debian.tar.xz 27924 SHA256:827c711e65830910ef953cdf81aeb75b77234b55a56ddfb27541bb8f487cd22c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.32-1/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.32-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.32-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcbor=0.5.0+dfsg-2`

Binary Packages:

- `libcbor0:amd64=0.5.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libcbor0/copyright`)

- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.5.0+dfsg-2
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.5.0+dfsg-2.dsc' libcbor_0.5.0+dfsg-2.dsc 2057 SHA256:c1ad2786b340b65d55761ecc3d090a9d997b3a0e5218ff1d39f5cd19df900d73
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.5.0+dfsg.orig.tar.gz' libcbor_0.5.0+dfsg.orig.tar.gz 261201 SHA256:2bd1fb795d121a72fc127ccd0e6ce5f5742d5970d0913759bcdc729c700804fb
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.5.0+dfsg-2.debian.tar.xz' libcbor_0.5.0+dfsg-2.debian.tar.xz 3944 SHA256:c06d0890b369183142d09fc6a460d68fdaf32bb22f9885ee1cc203d00adc543d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcbor/0.5.0+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/libcbor/0.5.0+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcbor/0.5.0+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcroco=0.6.13-1`

Binary Packages:

- `libcroco3:amd64=0.6.13-1`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.13-1
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.13-1.dsc' libcroco_0.6.13-1.dsc 2216 SHA256:1f9a861643c65b432221f779ad9a6a0a1585724efbb01a10dfe22f69e3fbc18c
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.13.orig.tar.xz' libcroco_0.6.13.orig.tar.xz 487840 SHA256:767ec234ae7aa684695b3a735548224888132e063f92db585759b422570621d4
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.13-1.debian.tar.xz' libcroco_0.6.13-1.debian.tar.xz 7192 SHA256:922d4f962f7608e1ff46700dc26aa6198aa1a5099aaceebe75e9695ce3b8e374
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcroco/0.6.13-1/ (for browsing the source)
- https://sources.debian.net/src/libcroco/0.6.13-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcroco/0.6.13-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdatrie=0.2.12-3`

Binary Packages:

- `libdatrie1:amd64=0.2.12-3`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.12-3
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.12-3.dsc' libdatrie_0.2.12-3.dsc 2260 SHA256:631b3aa1b0cf12bcb04df8a19a8370445801a176edce830e74c01f6a55f778aa
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.12.orig.tar.xz' libdatrie_0.2.12.orig.tar.xz 310236 SHA256:452dcc4d3a96c01f80f7c291b42be11863cd1554ff78b93e110becce6e00b149
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.12-3.debian.tar.xz' libdatrie_0.2.12-3.debian.tar.xz 9188 SHA256:10409d93b3762b8ac8e0851bb2b71f76c2c5b57df8999bf8b9686d951c8b7476
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdatrie/0.2.12-3/ (for browsing the source)
- https://sources.debian.net/src/libdatrie/0.2.12-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdatrie/0.2.12-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libde265=1.0.4-1`

Binary Packages:

- `libde265-0:amd64=1.0.4-1`

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
$ apt-get source -qq --print-uris libde265=1.0.4-1
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.4-1.dsc' libde265_1.0.4-1.dsc 2216 SHA256:7fbccf0f722a9d82477db9db5f9cc58745aeca40f31ec292fb6873b8d3c652bf
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.4.orig.tar.gz' libde265_1.0.4.orig.tar.gz 856952 SHA256:c3f033bd59777624859c8d04a5b7ce4210adbce4a500943d2e211c4d517d0116
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.4-1.debian.tar.xz' libde265_1.0.4-1.debian.tar.xz 8224 SHA256:b52d670c562423b682f100ad3f5ead2b0da5a1d27fbd30df94042a639943b590
```

Other potentially useful URLs:

- https://sources.debian.net/src/libde265/1.0.4-1/ (for browsing the source)
- https://sources.debian.net/src/libde265/1.0.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libde265/1.0.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20191231-1`

Binary Packages:

- `libedit2:amd64=3.1-20191231-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-1
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20191231-1.dsc' libedit_3.1-20191231-1.dsc 2129 SHA256:1be31eebf9cf3b38a9e7c3c4d4b37f002e3f89df48f00dec32506cbe9337ae38
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA256:dbb82cb7e116a5f8025d35ef5b4f7d4a3cdd0a3909a146a39112095a2d229071
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20191231-1.debian.tar.xz' libedit_3.1-20191231-1.debian.tar.xz 14168 SHA256:f815baa1932f9df5d4cdb316a85ebd3cc91441c4d83ba2c8454f342573ed0eab
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20191231-1/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20191231-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20191231-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.11-stable-1.dsc' libevent_2.1.11-stable-1.dsc 2526 SHA256:b07a15f54f2ab403eed9aa648a1ea9bee05a5a5362570d334a76597e79a1d795
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.11-stable.orig.tar.gz' libevent_2.1.11-stable.orig.tar.gz 1082234 SHA256:a65bac6202ea8c5609fd5c7e480e6d25de467ea1917c08290c521752f147283d
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.11-stable.orig.tar.gz.asc' libevent_2.1.11-stable.orig.tar.gz.asc 488 SHA256:9add12a6852022f675e4388cb1ac0fdcd68c6c1bc6e5212fae78d3f1c00f2826
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.1.11-stable-1.debian.tar.xz' libevent_2.1.11-stable-1.debian.tar.xz 17264 SHA256:fae364ea17e708a73572dd8b0add7fcded427c9e2b2405679738459c6f02de8d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libevent/2.1.11-stable-1/ (for browsing the source)
- https://sources.debian.net/src/libevent/2.1.11-stable-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libevent/2.1.11-stable-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libexif=0.6.21-6`

Binary Packages:

- `libexif-dev:amd64=0.6.21-6`
- `libexif12:amd64=0.6.21-6`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.21-6
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.21-6.dsc' libexif_0.6.21-6.dsc 2114 SHA256:aa9fb80b036a5162782edf08055ddc54bd55881b7850a4cca4dc47a6a4ea10a4
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.21.orig.tar.gz' libexif_0.6.21.orig.tar.gz 2081615 SHA256:edb7eb13664cf950a6edd132b75e99afe61c5effe2f16494e6d27bc404b287bf
'http://deb.debian.org/debian/pool/main/libe/libexif/libexif_0.6.21-6.debian.tar.xz' libexif_0.6.21-6.debian.tar.xz 14412 SHA256:42ec61a88746a23d211dfded1ef620797959f45b90497d888562968eb3dfe17c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libexif/0.6.21-6/ (for browsing the source)
- https://sources.debian.net/src/libexif/0.6.21-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libexif/0.6.21-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.3-3`

Binary Packages:

- `libffi-dev:amd64=3.3-3`
- `libffi7:amd64=3.3-3`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi7/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.3-3
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-3.dsc' libffi_3.3-3.dsc 1932 SHA256:002e9218eab7ca0440c9726cc55fa629c807a60bb38d79515a4334bbd82bc867
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3.orig.tar.gz' libffi_3.3.orig.tar.gz 1305466 SHA256:72fba7922703ddfa7a028d513ac15a85c8d54c8d67f55fa5a4802885dc652056
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-3.debian.tar.xz' libffi_3.3-3.debian.tar.xz 8444 SHA256:9fbf04105d806f1ae5829bc3eddc16490311208b7efe26e0dba14bd8190087c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.3-3/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libfido2=1.3.1-1`

Binary Packages:

- `libfido2-1:amd64=1.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.3.1-1
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.3.1-1.dsc' libfido2_1.3.1-1.dsc 2208 SHA256:575e1ed1023b69697c1914440371924249da1d40bd9f84ac30de45da671e922d
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.3.1.orig.tar.gz' libfido2_1.3.1.orig.tar.gz 1512676 SHA256:ba35e22016b60c1e4be66dff3cd6a60c1fe4bfa0d91ec0b89ca9da25ebeaaf41
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.3.1-1.debian.tar.xz' libfido2_1.3.1-1.debian.tar.xz 73224 SHA256:7a2438e587862d76208719b82b31d157524c5087df4a0c7cf91e4d5f5964fa3e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfido2/1.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/libfido2/1.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfido2/1.3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.8.5-5`

Binary Packages:

- `libgcrypt20:amd64=1.8.5-5`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.5-5
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5.dsc' libgcrypt20_1.8.5-5.dsc 2800 SHA256:2dbecc03c700bc4f355eaab221dd53b7f1bf607e28fdd49d81b36cc2bd119daf
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2' libgcrypt20_1.8.5.orig.tar.bz2 2991291 SHA256:3b4a2a94cb637eff5bdebbcaf46f4d95c4f25206f459809339cdada0eb577ac3
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2.asc' libgcrypt20_1.8.5.orig.tar.bz2.asc 488 SHA256:4b24fda7847cd2b70ab19f4c38004a76bbdac46a1ddccff973ae88ba1296a22d
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5.debian.tar.xz' libgcrypt20_1.8.5-5.debian.tar.xz 32048 SHA256:9e3855d57a06d043f98fa162444ca23efe420151efe402373b892436a6457bec
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.8.5-5/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.8.5-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.8.5-5/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.37-1.dsc' libgpg-error_1.37-1.dsc 2220 SHA256:e789ed6bf791c90e9ba28dc3923f54379862ca65bd286495942176dcfad5d8a7
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.37.orig.tar.bz2' libgpg-error_1.37.orig.tar.bz2 937282 SHA256:b32d6ff72a73cf79797f7f2d039e95e9c6f92f0c1450215410840ab62aea9763
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.37.orig.tar.bz2.asc' libgpg-error_1.37.orig.tar.bz2.asc 488 SHA256:394f0904c386f88e2b2db5042880a2a302cbc6e4ab902bacf3d338ded038066b
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.37-1.debian.tar.xz' libgpg-error_1.37-1.debian.tar.xz 17332 SHA256:09843b599726c1ab7b1fcd86ce617bd91d6378ff754c6da0b7e536ed1c3b6c16
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.37-1/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.37-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.37-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libheif=1.6.1-1`

Binary Packages:

- `libheif1:amd64=1.6.1-1`

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
$ apt-get source -qq --print-uris libheif=1.6.1-1
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.6.1-1.dsc' libheif_1.6.1-1.dsc 2239 SHA256:5fc76d1cc1bc0a057d93a0abbdd46d6a29c1f1525d9d56f52ba628bf5a97704c
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.6.1.orig.tar.gz' libheif_1.6.1.orig.tar.gz 1514950 SHA256:a22611289464da08fa7e580c95ea5e1b1b522b96ee6807de9b3b4605efb621d1
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.6.1-1.debian.tar.xz' libheif_1.6.1-1.debian.tar.xz 6416 SHA256:c3baf69ae32e11c65db7de64c62ff55bb991ea8e7d61305e93236989ce4bf346
```

Other potentially useful URLs:

- https://sources.debian.net/src/libheif/1.6.1-1/ (for browsing the source)
- https://sources.debian.net/src/libheif/1.6.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libheif/1.6.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libice=2:1.0.9-2`

Binary Packages:

- `libice-dev:amd64=2:1.0.9-2`
- `libice6:amd64=2:1.0.9-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-2
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9-2.dsc' libice_1.0.9-2.dsc 2130 SHA256:116595cd54be23edad0b55e1cd4bc1929f277fa5c2d00d8f187b0bc5dd39ad6c
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9-2.diff.gz' libice_1.0.9-2.diff.gz 6384 SHA256:777f13e08aada3103c32a0b93a26782ca959027bcd98c2c1ddaade8f944fa40a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libice/2:1.0.9-2/ (for browsing the source)
- https://sources.debian.net/src/libice/2:1.0.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libice/2:1.0.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn2=2.2.0-2`

Binary Packages:

- `libidn2-0:amd64=2.2.0-2`
- `libidn2-dev:amd64=2.2.0-2`

Licenses: (parsed from: `/usr/share/doc/libidn2-0/copyright`, `/usr/share/doc/libidn2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `Unicode`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libidn2/2.2.0-2/


### `dpkg` source package: `libjpeg-turbo=1:1.5.2-2`

Binary Packages:

- `libjpeg-dev=1:1.5.2-2`
- `libjpeg62-turbo:amd64=1:1.5.2-2+b1`
- `libjpeg62-turbo-dev:amd64=1:1.5.2-2+b1`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3`
- `BSD-BY-LC-NE`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:1.5.2-2
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-2.dsc' libjpeg-turbo_1.5.2-2.dsc 2434 SHA256:f975bd4b2192e3f1aeacef7f0de33035f386225035aea6157b413b1c500d46a1
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2.orig.tar.gz' libjpeg-turbo_1.5.2.orig.tar.gz 1657235 SHA256:9098943b270388727ae61de82adec73cf9f0dbb240b3bc8b172595ebf405b528
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-2.debian.tar.xz' libjpeg-turbo_1.5.2-2.debian.tar.xz 78360 SHA256:964a2d747f8e74cbd558f343afd11b7dfe37212a611eeca863f1908eba66f728
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:1.5.2-2/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:1.5.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:1.5.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libksba=1.3.5-2`

Binary Packages:

- `libksba8:amd64=1.3.5-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.3.5-2
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5-2.dsc' libksba_1.3.5-2.dsc 2526 SHA256:4fd08fd129f97ab1df86c220b88b7b2c6e4e04aa90bfd3ae364d18022256bef8
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2' libksba_1.3.5.orig.tar.bz2 620649 SHA256:41444fd7a6ff73a79ad9728f985e71c9ba8cd3e5e53358e70d5f066d35c1a340
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2.asc' libksba_1.3.5.orig.tar.bz2.asc 287 SHA256:a954b03144ee882c838853da24fd7b6868b78df72a18c71079217d968698a76f
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.3.5-2.debian.tar.xz' libksba_1.3.5-2.debian.tar.xz 13852 SHA256:98c985bff973be1aecc702fa15887ff1e5b8de481d1dc3e99423a587754eaabd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libksba/1.3.5-2/ (for browsing the source)
- https://sources.debian.net/src/libksba/1.3.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libksba/1.3.5-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libmaxminddb=1.3.2-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.3.2-1`
- `libmaxminddb0:amd64=1.3.2-1`

Licenses: (parsed from: `/usr/share/doc/libmaxminddb-dev/copyright`, `/usr/share/doc/libmaxminddb0/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `CC-BY-SA`
- `GPL`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmaxminddb=1.3.2-1
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.3.2-1.dsc' libmaxminddb_1.3.2-1.dsc 2104 SHA256:c75309a506da7a68fe74b13ab3f8f3024a377859ec9fb77aa2e4c057550c1158
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.3.2.orig.tar.gz' libmaxminddb_1.3.2.orig.tar.gz 248665 SHA256:5fa35b5e7ae3ed11b9c392d6ea38572966c1ceaeab4e2598174911978ea0c027
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.3.2-1.debian.tar.xz' libmaxminddb_1.3.2-1.debian.tar.xz 4868 SHA256:25b816d507995b6fe8d8430f43215f79cc1191e0f931e130e70a7060fa2992ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmaxminddb/1.3.2-1/ (for browsing the source)
- https://sources.debian.net/src/libmaxminddb/1.3.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmaxminddb/1.3.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmnl=1.0.4-2`

Binary Packages:

- `libmnl0:amd64=1.0.4-2+b1`

Licenses: (parsed from: `/usr/share/doc/libmnl0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libmnl=1.0.4-2
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4-2.dsc' libmnl_1.0.4-2.dsc 1994 SHA256:131106bb7eb4a94fa8e8c135f92c38068d0b42681f166eb159137f171c568630
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4.orig.tar.bz2' libmnl_1.0.4.orig.tar.bz2 301270 SHA256:171f89699f286a5854b72b91d06e8f8e3683064c5901fb09d954a9ab6f551f81
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4-2.debian.tar.xz' libmnl_1.0.4-2.debian.tar.xz 7512 SHA256:208d62777081ffe6d7dffde0d7370cefb03fe0a6a0486a1b50f6b7b8e9a5b068
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmnl/1.0.4-2/ (for browsing the source)
- https://sources.debian.net/src/libmnl/1.0.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmnl/1.0.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng1.6=1.6.37-2`

Binary Packages:

- `libpng-dev:amd64=1.6.37-2`
- `libpng16-16:amd64=1.6.37-2`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.37-2
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.37-2.dsc' libpng1.6_1.6.37-2.dsc 2225 SHA256:4567a54b5804e068e61477e9cd78346557b85b72add10ef10f130a5be169662e
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA256:ca74a0dace179a8422187671aee97dd3892b53e168627145271cad5b5ac81307
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.37-2.debian.tar.xz' libpng1.6_1.6.37-2.debian.tar.xz 31844 SHA256:097cee0f0da4013d0231d37e090204ab3fa592b4fecdaaed3fca8d13affcaae8
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpng1.6/1.6.37-2/ (for browsing the source)
- https://sources.debian.net/src/libpng1.6/1.6.37-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpng1.6/1.6.37-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpsl=0.20.2-2`

Binary Packages:

- `libpsl5:amd64=0.20.2-2`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.20.2-2
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.20.2-2.dsc' libpsl_0.20.2-2.dsc 1637 SHA256:ae401852522d748f1222b91734bc5bd7c6db0de843dd675adc180f2a1884c94d
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.20.2.orig.tar.gz' libpsl_0.20.2.orig.tar.gz 8590430 SHA256:94d2b5e00e9aa761ae7efbaa67edc00d5298487ed9706eb4789e349012993c31
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.20.2-2.debian.tar.xz' libpsl_0.20.2-2.debian.tar.xz 9920 SHA256:1f008454fdb973964202020fb700d5028e001b7eaa4e77eeab8ebc99b749ea51
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpsl/0.20.2-2/ (for browsing the source)
- https://sources.debian.net/src/libpsl/0.20.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpsl/0.20.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `librsvg=2.46.4-1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.46.4-1`
- `librsvg2-2:amd64=2.46.4-1`
- `librsvg2-common:amd64=2.46.4-1`
- `librsvg2-dev:amd64=2.46.4-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `Boost-1.0`
- `Expat`
- `LGPL-2`
- `LGPL-2+`
- `MPL-2.0`
- `Sun-permissive`
- `Unlicense`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.46.4-1
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.46.4-1.dsc' librsvg_2.46.4-1.dsc 2843 SHA256:f24180cd730fb805af8aee79a3e577031f065982f1ad2d65f74f8537a1e14afd
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.46.4.orig.tar.xz' librsvg_2.46.4.orig.tar.xz 12680904 SHA256:b45b9ee3b64c58baaf800bcdff5fcd04d79930dba4c56e46e0d3b0aead40cc29
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.46.4-1.debian.tar.xz' librsvg_2.46.4-1.debian.tar.xz 22876 SHA256:f120e434c898aeb6b1a13a2dbcb2024c425aabbdb99d51a3b393a0301084ecb5
```

Other potentially useful URLs:

- https://sources.debian.net/src/librsvg/2.46.4-1/ (for browsing the source)
- https://sources.debian.net/src/librsvg/2.46.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librsvg/2.46.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.4.2-2`

Binary Packages:

- `libseccomp2:amd64=2.4.2-2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.2-2
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.4.2-2.dsc' libseccomp_2.4.2-2.dsc 2413 SHA256:cb9c0bc4e318250850ec3a13bff5fe2494fd3e46bedeb453bdb0bb13c69de08b
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.4.2.orig.tar.gz' libseccomp_2.4.2.orig.tar.gz 601014 SHA256:b54f27b53884caacc932e75e6b44304ac83586e2abe7a83eca6daecc5440585b
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.4.2-2.debian.tar.xz' libseccomp_2.4.2-2.debian.tar.xz 7736 SHA256:7bbc0a96fbb8123ce11a946547d6479f481367b5a1342f2ad2a06f8f80de833f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.4.2-2/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.4.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.4.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.0-1`

Binary Packages:

- `libselinux1:amd64=3.0-1+b1`
- `libselinux1-dev:amd64=3.0-1+b1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.0-1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.0-1.dsc' libselinux_3.0-1.dsc 2220 SHA256:9f147a02241eb6e3db4b2bcad55cf5fd516702788f6561abbe82e9fd5faed6d7
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.0.orig.tar.gz' libselinux_3.0.orig.tar.gz 212096 SHA256:2ea2b30f671dae9d6b1391cbe8fb2ce5d36a3ee4fb1cd3c32f0d933c31b82433
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.0-1.debian.tar.xz' libselinux_3.0-1.debian.tar.xz 23568 SHA256:765b937149864b2fe265c1e9df7d8f5f8f1d384c1ef351458a996f284a4392ef
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/3.0-1/ (for browsing the source)
- https://sources.debian.net/src/libselinux/3.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/3.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=3.0-1`

Binary Packages:

- `libsemanage-common=3.0-1`
- `libsemanage1:amd64=3.0-1+b1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.0-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.0-1.dsc' libsemanage_3.0-1.dsc 2333 SHA256:269c958d0f0a8e8fff34e75c88153c060eb8054127bfadf183903a49c390fd06
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.0.orig.tar.gz' libsemanage_3.0.orig.tar.gz 180745 SHA256:a497b0720d54eac427f1f3f618eed417e50ed8f4e47ed0f7a1d391bd416e84cf
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.0-1.debian.tar.xz' libsemanage_3.0-1.debian.tar.xz 17040 SHA256:d6dd598f84fa642d10d27c5f9ef4155ceef80d8127a48075b3c5a918d93a513a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/3.0-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/3.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/3.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=3.0-1`

Binary Packages:

- `libsepol1:amd64=3.0-1`
- `libsepol1-dev:amd64=3.0-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`, `/usr/share/doc/libsepol1-dev/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.0-1
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.0-1.dsc' libsepol_3.0-1.dsc 1770 SHA256:0073de5844605d380dd56f6630678ad91459496dc768fa9eb4d8cc7f693f5c1a
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.0.orig.tar.gz' libsepol_3.0.orig.tar.gz 473864 SHA256:5b7ae1881909f1048b06f7a0c364c5c8a86ec12e0ec76e740fe9595a6033eb79
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.0-1.debian.tar.xz' libsepol_3.0-1.debian.tar.xz 14224 SHA256:a16b5bc3c041e016d01794d1a1b9826ed4426862622c05526e93607c325ec328
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/3.0-1/ (for browsing the source)
- https://sources.debian.net/src/libsepol/3.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/3.0-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12-2.dsc' libsigsegv_2.12-2.dsc 2363 SHA256:b081b244de2f427345838f379405d8438c29db1fa746a4e270167ae7cb10c079
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz' libsigsegv_2.12.orig.tar.gz 451408 SHA256:3ae1af359eebaa4ffc5896a1aee3568c052c99879316a1ab57f8fe1789c390b6
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz.asc' libsigsegv_2.12.orig.tar.gz.asc 2442 SHA256:1861a9a182bbb7a24a18f7e43fe0fa3eb6f6fd53780b30e01990677112694dfc
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12-2.debian.tar.xz' libsigsegv_2.12-2.debian.tar.xz 8340 SHA256:73940fb346f7afd90c93a341164cd175349e0507de8b1c05b0834b598c372260
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsigsegv/2.12-2/ (for browsing the source)
- https://sources.debian.net/src/libsigsegv/2.12-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsigsegv/2.12-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libssh2=1.8.0-2.1`

Binary Packages:

- `libssh2-1:amd64=1.8.0-2.1`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.8.0-2.1
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.8.0-2.1.dsc' libssh2_1.8.0-2.1.dsc 1958 SHA256:33f070a4a32db5d3952457986d8f80c9cf874dd144d81f5bce062171564b35d9
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.8.0.orig.tar.gz' libssh2_1.8.0.orig.tar.gz 846989 SHA256:4382d33de790b28f862e53ed59ffbd65f3def7a06e8b6e9ca1b6f70453b4d5e0
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.8.0-2.1.debian.tar.xz' libssh2_1.8.0-2.1.debian.tar.xz 13988 SHA256:e3c34166cddaba7f2162132ef4f4bdc1490c499ee6610bde81f773adef43489e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.8.0-2.1/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.8.0-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.8.0-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.16.0-2`

Binary Packages:

- `libtasn1-6:amd64=4.16.0-2`
- `libtasn1-6-dev:amd64=4.16.0-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`, `/usr/share/doc/libtasn1-6-dev/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.16.0-2
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.dsc' libtasn1-6_4.16.0-2.dsc 2586 SHA256:fd4a387c71f95c3eceb1072a3f42c7021d73128027ea41a18d6efc6cbfdd764a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz' libtasn1-6_4.16.0.orig.tar.gz 1812442 SHA256:0e0fb0903839117cb6e3b56e68222771bebf22ad7fc2295a0ed7d576e8d4329d
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz.asc' libtasn1-6_4.16.0.orig.tar.gz.asc 488 SHA256:06c201e8c3b43c27465ed79294d4c4ec8dcd3e95e4a6176ecbf273229ee3e2d0
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.debian.tar.xz' libtasn1-6_4.16.0-2.debian.tar.xz 17740 SHA256:c1a89b0bac0fb7c83ebac4eafbca0475c24350ade6ccaef31266424725610624
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.16.0-2/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.16.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.16.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libthai=0.1.28-3`

Binary Packages:

- `libthai-data=0.1.28-3`
- `libthai0:amd64=0.1.28-3`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.28-3
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28-3.dsc' libthai_0.1.28-3.dsc 2346 SHA256:a6317b6a8e4ba40cedb10a9a659fc23885bfbe5eb8cf3a8b325a86064b0a542d
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28.orig.tar.xz' libthai_0.1.28.orig.tar.xz 413592 SHA256:ffe0a17b4b5aa11b153c15986800eca19f6c93a4025ffa5cf2cab2dcdf1ae911
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28-3.debian.tar.xz' libthai_0.1.28-3.debian.tar.xz 12128 SHA256:bca48abd9d040e844ebcb1f91a6ab4bcdfad66e36c1143f79d60461e933fddf9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libthai/0.1.28-3/ (for browsing the source)
- https://sources.debian.net/src/libthai/0.1.28-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libthai/0.1.28-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtool=2.4.6-13`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-13`
- `libltdl7:amd64=2.4.6-13`
- `libtool=2.4.6-13`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libtool/2.4.6-13/


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
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-2.dsc' libunistring_0.9.10-2.dsc 2206 SHA256:c6faf64e2d978ec074ebf88264730121dfd03cc1639df94b5dc3eb05b1678532
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-2.debian.tar.xz' libunistring_0.9.10-2.debian.tar.xz 40708 SHA256:5e291a1a15549d12c64575c72868a8c94586715d35062b5efb48fe9a9d09924e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/0.9.10-2/ (for browsing the source)
- https://sources.debian.net/src/libunistring/0.9.10-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/0.9.10-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwebp=0.6.1-2`

Binary Packages:

- `libwebp-dev:amd64=0.6.1-2+b1`
- `libwebp6:amd64=0.6.1-2+b1`
- `libwebpdemux2:amd64=0.6.1-2+b1`
- `libwebpmux3:amd64=0.6.1-2+b1`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.6.1-2
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.6.1-2.dsc' libwebp_0.6.1-2.dsc 2064 SHA256:321ee69e44f0d037d5fec47692251e35ed22c9ad0bbf0a6bf0fae990a52319f4
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA256:a86045e3ec24704bddbaa369ca30980d6bf4f2625f4cdca03715e91f9c08bbb4
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.6.1-2.debian.tar.xz' libwebp_0.6.1-2.debian.tar.xz 9532 SHA256:5af543e277abb97f6b2c72ca0d7ce95de79108d88da383d511ef729683fa7a45
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwebp/0.6.1-2/ (for browsing the source)
- https://sources.debian.net/src/libwebp/0.6.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwebp/0.6.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwmf=0.2.8.4-17`

Binary Packages:

- `libwmf-dev=0.2.8.4-17`
- `libwmf0.2-7:amd64=0.2.8.4-17`

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

### `dpkg` source package: `libx11=2:1.6.8-1`

Binary Packages:

- `libx11-6:amd64=2:1.6.8-1`
- `libx11-data=2:1.6.8-1`
- `libx11-dev:amd64=2:1.6.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.8-1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.8-1.dsc' libx11_1.6.8-1.dsc 2639 SHA256:4c64049b12059e10fa6986afab53f16a88f8d67ab4ba5778773d840dc1dd1dcc
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.8.orig.tar.gz' libx11_1.6.8.orig.tar.gz 3144482 SHA256:69d1a27cba722dca897198a23fa8d3cad3ec0c715e00205ea4398ec68a4258a5
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.8.orig.tar.gz.asc' libx11_1.6.8.orig.tar.gz.asc 358 SHA256:acbbc22289a43defbb0b2fcdc083587492feec31dfef49e9829009986be84f79
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.8-1.diff.gz' libx11_1.6.8-1.diff.gz 56202 SHA256:0f43c4539885873d8bbc6e0387313bc9379ee2054e5c1ab4eab724386e2b1ba3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.6.8-1/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.6.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.6.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxau=1:1.0.8-1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.8-1+b2`
- `libxau6:amd64=1:1.0.8-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8-1.dsc' libxau_1.0.8-1.dsc 2040 SHA256:3ddb5f2c7a49ef7507b8d1e63e891238db877b4d1bb1c5486a3e3242c8523602
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA256:c343b4ef66d66a6b3e0e27aa46b37ad5cab0f11a5c565eafb4a1c7590bc71d7b
'http://deb.debian.org/debian/pool/main/libx/libxau/libxau_1.0.8-1.diff.gz' libxau_1.0.8-1.diff.gz 15287 SHA256:b493479d6a52a0e753dd357ad8a4bc5c4296015f3f7b96cf546f7c5c5843cbb0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxau/1:1.0.8-1/ (for browsing the source)
- https://sources.debian.net/src/libxau/1:1.0.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxau/1:1.0.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcb=1.13.1-5`

Binary Packages:

- `libxcb-render0:amd64=1.13.1-5`
- `libxcb-render0-dev:amd64=1.13.1-5`
- `libxcb-shm0:amd64=1.13.1-5`
- `libxcb-shm0-dev:amd64=1.13.1-5`
- `libxcb1:amd64=1.13.1-5`
- `libxcb1-dev:amd64=1.13.1-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.13.1-5
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.13.1-5.dsc' libxcb_1.13.1-5.dsc 5352 SHA256:6edc6dba78dbc148595e0eb4d114f114c0ab7003f3c9f5a58ef37c85bde93dae
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.13.1.orig.tar.gz' libxcb_1.13.1.orig.tar.gz 636748 SHA256:f09a76971437780a602303170fd51b5f7474051722bc39d566a272d2c4bde1b5
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.13.1-5.diff.gz' libxcb_1.13.1-5.diff.gz 25648 SHA256:ddb658e0dc260b585a332de00427521d657891643a2ee04e99dc88ede75921a8
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcb/1.13.1-5/ (for browsing the source)
- https://sources.debian.net/src/libxcb/1.13.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcb/1.13.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcrypt=1:4.4.10-10`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.10-10`
- `libcrypt1:amd64=1:4.4.10-10`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxcrypt/1:4.4.10-10/


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

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.3-1+b2`
- `libxext6:amd64=2:1.3.3-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.3-1
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.dsc' libxext_1.3.3-1.dsc 2221 SHA256:47106df75b8f3db1e43803e8e94a2e966cd23f7daa8cfc393af739a9e33ef955
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3.orig.tar.gz' libxext_1.3.3.orig.tar.gz 468441 SHA256:eb0b88050491fef4716da4b06a4d92b4fc9e76f880d6310b2157df604342cfe5
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.diff.gz' libxext_1.3.3-1.diff.gz 20763 SHA256:e294a4884eb68acbd151312cb0c973aad63268b637b15ccf1911864b7197557e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxext/2:1.3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxext/2:1.3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxext/2:1.3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxml2=2.9.10+dfsg-3`

Binary Packages:

- `libxml2:amd64=2.9.10+dfsg-3`
- `libxml2-dev:amd64=2.9.10+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxml2/2.9.10+dfsg-3/


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

### `dpkg` source package: `libxslt=1.1.34-3`

Binary Packages:

- `libxslt1-dev:amd64=1.1.34-3`
- `libxslt1.1:amd64=1.1.34-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.34-3
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34-3.dsc' libxslt_1.1.34-3.dsc 2375 SHA256:90607cffb5ee500f5a0063ca18e3b91689d39cb1367b31ebd61de08fc7c0f7d9
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA256:98b1bd46d6792925ad2dfe9a87452ea2adebf69dcb9919ffd55bf926a7f93f7f
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA256:673d1477552bdd5b0cc665704e77ca70e6be5d2f257e6a5a341c846719d747cf
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34-3.debian.tar.xz' libxslt_1.1.34-3.debian.tar.xz 20912 SHA256:33f39a1cdbdc64ba46f1bea7ace668bd0bfac6969cd5fdc4a7e0ea0b1d05906d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxslt/1.1.34-3/ (for browsing the source)
- https://sources.debian.net/src/libxslt/1.1.34-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxslt/1.1.34-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxt=1:1.1.5-1`

Binary Packages:

- `libxt-dev:amd64=1:1.1.5-1+b3`
- `libxt6:amd64=1:1.1.5-1+b3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.1.5-1
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.5-1.dsc' libxt_1.1.5-1.dsc 2109 SHA256:f44ae1393c9fd02c0b3dd03576c7b26e6c7b09de3271a87e018efadeed311639
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.5.orig.tar.gz' libxt_1.1.5.orig.tar.gz 962169 SHA256:b59bee38a9935565fa49dc1bfe84cb30173e2e07e1dcdf801430d4b54eb0caa3
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.5-1.diff.gz' libxt_1.1.5-1.diff.gz 14462 SHA256:822fe813d1ea9213e6fde91cbb607c0b6874341dc19b77b0f6649b8be8472d82
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxt/1:1.1.5-1/ (for browsing the source)
- https://sources.debian.net/src/libxt/1:1.1.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxt/1:1.1.5-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.4+dfsg-3.dsc' libzstd_1.4.4+dfsg-3.dsc 2266 SHA256:f6e3cc2b022b9812daca4f427a00fc6e109e6e1e72e64d6a254add040853b110
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.4+dfsg.orig.tar.xz' libzstd_1.4.4+dfsg.orig.tar.xz 1357144 SHA256:be9f9bfd3f6816f21e1108869a9acad6efdc4882ed3f7a1f58ec752f67864890
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.4+dfsg-3.debian.tar.xz' libzstd_1.4.4+dfsg-3.debian.tar.xz 16068 SHA256:f7fec89f1fae04dfa551d124973167e09e84c864a25961aa20727cc91277b0e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.4.4+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.4.4+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.4.4+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `linux=5.4.19-1`

Binary Packages:

- `linux-libc-dev:amd64=5.4.19-1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `CRYPTOGAMS`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `Unicode-data`
- `X11`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=5.4.19-1
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.4.19-1.dsc' linux_5.4.19-1.dsc 200853 SHA256:bffb240099fcd60d8d410f2a16d2a9f61efcf4fc78f8797456d4eea92a8e288a
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.4.19.orig.tar.xz' linux_5.4.19.orig.tar.xz 113678372 SHA256:e46d6cbfc4f3466c88d4ec366df10218424331d86d8f31a6da3b07f2948a5431
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.4.19-1.debian.tar.xz' linux_5.4.19-1.debian.tar.xz 1208900 SHA256:31fdcf5a84cdfe02344cfda8ad8a89c2f4bd69afbd5c2a3a5825e7f04f6a5144
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/5.4.19-1/ (for browsing the source)
- https://sources.debian.net/src/linux/5.4.19-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/5.4.19-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.2-2.dsc' lz4_1.9.2-2.dsc 1956 SHA256:103fa80edbf501cf6e6d9ee0ed3d75d6111cd06026b00aaccaa11fe5555b71a6
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.2.orig.tar.gz' lz4_1.9.2.orig.tar.gz 305796 SHA256:658ba6191fa44c92280d4aa2c271b0f4fbc0e34d249578dd05e50e76d0e5efcc
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.2-2.debian.tar.xz' lz4_1.9.2-2.debian.tar.xz 12712 SHA256:8970a0afc2f1633bbc8b7f55fa36ba711fb4d0c1811e591ad8f52d1d1968592c
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.9.2-2/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.9.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.9.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `m4=1.4.18-4`

Binary Packages:

- `m4=1.4.18-4`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-4
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-4.dsc' m4_1.4.18-4.dsc 1638 SHA256:11925f50e25f93d6b9a72336e7b9fd0de72a813d5d5f3204ecc3996f9ca3bbde
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA256:a2a9fff657e65ff25a8f3734f484dbd3ede8f8290786af71626de367dcd74267
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-4.debian.tar.xz' m4_1.4.18-4.debian.tar.xz 17240 SHA256:6543f074d5a3eed4ee7984f8a147c58e005c88254dfcf5bc3778c60b9ed07efd
```

Other potentially useful URLs:

- https://sources.debian.net/src/m4/1.4.18-4/ (for browsing the source)
- https://sources.debian.net/src/m4/1.4.18-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/m4/1.4.18-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `make-dfsg=4.2.1-1.2`

Binary Packages:

- `make=4.2.1-1.2`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.2.1-1.2
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.dsc' make-dfsg_4.2.1-1.2.dsc 2019 SHA256:0c8a2da5d51e03bf43e2929322d5a8406f08e5ee2d81a71ed6e5a8734f1b05cb
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.2.1.orig.tar.gz' make-dfsg_4.2.1.orig.tar.gz 1485018 SHA256:480405e8995796ea47cc54b281b7855280f0d815d296a1af1993eeeb72074e39
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.diff.gz' make-dfsg_4.2.1-1.2.diff.gz 53108 SHA256:80e0b96cee381391a5d3322317075e23d8474c92c5fa4fecd334bc2e0920887b
```

Other potentially useful URLs:

- https://sources.debian.net/src/make-dfsg/4.2.1-1.2/ (for browsing the source)
- https://sources.debian.net/src/make-dfsg/4.2.1-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/make-dfsg/4.2.1-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mariadb-10.3=1:10.3.22-1`

Binary Packages:

- `libmariadb-dev=1:10.3.22-1`
- `libmariadb-dev-compat:amd64=1:10.3.22-1`
- `libmariadb3:amd64=1:10.3.22-1`
- `mariadb-common=1:10.3.22-1`

Licenses: (parsed from: `/usr/share/doc/libmariadb-dev/copyright`, `/usr/share/doc/libmariadb-dev-compat/copyright`, `/usr/share/doc/libmariadb3/copyright`, `/usr/share/doc/mariadb-common/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-2+-with-bison-exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+-with-bison-exception`
- `GPL-verbatim`
- `LGPL`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT/X11`
- `SWsoft`
- `public-domain`
- `unlimited-free-doc`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris mariadb-10.3=1:10.3.22-1
'http://deb.debian.org/debian/pool/main/m/mariadb-10.3/mariadb-10.3_10.3.22-1.dsc' mariadb-10.3_10.3.22-1.dsc 4780 SHA256:395d56066fbd4a35e9ff9e4b1619e41857b412a47387fcf16c34265b93d67dd0
'http://deb.debian.org/debian/pool/main/m/mariadb-10.3/mariadb-10.3_10.3.22.orig.tar.gz' mariadb-10.3_10.3.22.orig.tar.gz 72050820 SHA256:3200055dbdc27746981b3bb4bc182e2cb79dcf28ea88014b641a5b81280ccec7
'http://deb.debian.org/debian/pool/main/m/mariadb-10.3/mariadb-10.3_10.3.22.orig.tar.gz.asc' mariadb-10.3_10.3.22.orig.tar.gz.asc 195 SHA256:1ede70600162de2876f875984a1f719665d257334612bae00583ebe658b67ea7
'http://deb.debian.org/debian/pool/main/m/mariadb-10.3/mariadb-10.3_10.3.22-1.debian.tar.xz' mariadb-10.3_10.3.22-1.debian.tar.xz 216264 SHA256:1b56b2d3dc406c84d6e2d5cd6c3abaf3cb7459d0974285178b81c2bdfb308927
```

Other potentially useful URLs:

- https://sources.debian.net/src/mariadb-10.3/1:10.3.22-1/ (for browsing the source)
- https://sources.debian.net/src/mariadb-10.3/1:10.3.22-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mariadb-10.3/1:10.3.22-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mercurial=5.2.2-1`

Binary Packages:

- `mercurial=5.2.2-1`
- `mercurial-common=5.2.2-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=5.2.2-1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.2.2-1.dsc' mercurial_5.2.2-1.dsc 2771 SHA256:317bdac2a46617dedaaca4104f4c753d9292537aa956f6d07fee10ec69af11d9
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.2.2.orig.tar.gz' mercurial_5.2.2.orig.tar.gz 7333065 SHA256:ffc5ff47488c7b5dae6ead3d99f08ef469500d6567592a25311838320106c03b
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.2.2.orig.tar.gz.asc' mercurial_5.2.2.orig.tar.gz.asc 833 SHA256:eb0b593430b961624d37df6328846df217c25a99d4f5c2ba92a22ac6661e4417
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.2.2-1.debian.tar.xz' mercurial_5.2.2-1.debian.tar.xz 59492 SHA256:5bc0d3182531409ddb59229736c06875435875f8edd76ceeb2b43d647d79c372
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/5.2.2-1/ (for browsing the source)
- https://sources.debian.net/src/mercurial/5.2.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/5.2.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mime-support=3.64`

Binary Packages:

- `mime-support=3.64`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.64
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.64.dsc' mime-support_3.64.dsc 1585 SHA256:34cf61a73c394487614e9927a36de971f5239726cb67ae5c7e704c2012e30405
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.64.tar.xz' mime-support_3.64.tar.xz 33036 SHA256:587f35aabd25e9cabd9be485ce94539fb783d5b8d23492798dbec320ee6b1e88
```

Other potentially useful URLs:

- https://sources.debian.net/src/mime-support/3.64/ (for browsing the source)
- https://sources.debian.net/src/mime-support/3.64/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mime-support/3.64/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpclib3=1.1.0-1`

Binary Packages:

- `libmpc3:amd64=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.1.0-1
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.1.0-1.dsc' mpclib3_1.1.0-1.dsc 1990 SHA256:bb57824015b735bf72399a53f8c6a241e6a8bd402753b0fdcdaa5b99d0aef790
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.1.0.orig.tar.gz' mpclib3_1.1.0.orig.tar.gz 701263 SHA256:6985c538143c1208dcb1ac42cedad6ff52e267b47e5f970183a3e75125b43c2e
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.1.0-1.diff.gz' mpclib3_1.1.0-1.diff.gz 3794 SHA256:84b10a4ae958b3015e136b75be5fee22961255d19be655f7d0adae8d4f3bc977
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpclib3/1.1.0-1/ (for browsing the source)
- https://sources.debian.net/src/mpclib3/1.1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpclib3/1.1.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpdecimal=2.4.2-2`

Binary Packages:

- `libmpdec2:amd64=2.4.2-2`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/mpdecimal/2.4.2-2/


### `dpkg` source package: `mpfr4=4.0.2-1`

Binary Packages:

- `libmpfr6:amd64=4.0.2-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.0.2-1
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.0.2-1.dsc' mpfr4_4.0.2-1.dsc 1972 SHA256:9021ec2462ed0e73ea1379266740473abf5f826be819226497729f6c6b02e672
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.0.2.orig.tar.xz' mpfr4_4.0.2.orig.tar.xz 1441996 SHA256:1d3be708604eae0e42d578ba93b390c2a145f17743a744d8f3f8c2ad5855a38a
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.0.2-1.debian.tar.xz' mpfr4_4.0.2-1.debian.tar.xz 10544 SHA256:99c4d35654f33340f0efdec67142a34753157b20334cadad9018f5eab29738da
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpfr4/4.0.2-1/ (for browsing the source)
- https://sources.debian.net/src/mpfr4/4.0.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpfr4/4.0.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mysql-defaults=1.0.5`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.5`
- `mysql-common=5.8+1.0.5`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.5
'http://deb.debian.org/debian/pool/main/m/mysql-defaults/mysql-defaults_1.0.5.dsc' mysql-defaults_1.0.5.dsc 2235 SHA256:b6aaf2e08ed89079594f909ce2ec52e2c1232748c6f8e0691796bbb0764e4ef9
'http://deb.debian.org/debian/pool/main/m/mysql-defaults/mysql-defaults_1.0.5.tar.xz' mysql-defaults_1.0.5.tar.xz 7100 SHA256:71dd3115beba9facd1a9d75ae3178f6f9fa72c01d6be81c08472300e6c29fa2e
```

Other potentially useful URLs:

- https://sources.debian.net/src/mysql-defaults/1.0.5/ (for browsing the source)
- https://sources.debian.net/src/mysql-defaults/1.0.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mysql-defaults/1.0.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.1+20191019-1`

Binary Packages:

- `libncurses-dev:amd64=6.1+20191019-1`
- `libncurses5-dev:amd64=6.1+20191019-1`
- `libncurses6:amd64=6.1+20191019-1`
- `libncursesw5-dev:amd64=6.1+20191019-1`
- `libncursesw6:amd64=6.1+20191019-1`
- `libtinfo6:amd64=6.1+20191019-1`
- `ncurses-base=6.1+20191019-1`
- `ncurses-bin=6.1+20191019-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1+20191019-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20191019-1.dsc' ncurses_6.1+20191019-1.dsc 4106 SHA256:84153ab02140a0caf6755b593b149dda32a5120d264cc9c2a31b61edf20256f2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20191019.orig.tar.gz' ncurses_6.1+20191019.orig.tar.gz 3463374 SHA256:b42ca297f1823c1b1f2baaf46da5a61f690dc857600c7eb95d02432bd9905d3a
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20191019.orig.tar.gz.asc' ncurses_6.1+20191019.orig.tar.gz.asc 265 SHA256:670ab32ca07bf61d08d62731b1beef62194f684761bb73b2de1143949b0e88b6
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20191019-1.debian.tar.xz' ncurses_6.1+20191019-1.debian.tar.xz 61096 SHA256:a650c2a0e3c2fe8ddeb63ce6387aa411edfc0cff0220df210cff43f60781d10f
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.1+20191019-1/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.1+20191019-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.1+20191019-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `netbase=6.1`

Binary Packages:

- `netbase=6.1`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.1
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.1.dsc' netbase_6.1.dsc 1480 SHA256:d3d24cf00001259d3311c0509b4e23ac150cffea27b546e3a204864f52824556
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.1.tar.xz' netbase_6.1.tar.xz 31984 SHA256:084d743bd84d4d9380bac4c71c51e57406dce44f5a69289bb823c903e9b035d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/6.1/ (for browsing the source)
- https://sources.debian.net/src/netbase/6.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/6.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.5.1+really3.5.1-2`

Binary Packages:

- `libhogweed5:amd64=3.5.1+really3.5.1-2`
- `libnettle7:amd64=3.5.1+really3.5.1-2`
- `nettle-dev:amd64=3.5.1+really3.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libhogweed5/copyright`, `/usr/share/doc/libnettle7/copyright`, `/usr/share/doc/nettle-dev/copyright`)

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
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.dsc' nettle_3.5.1+really3.5.1-2.dsc 2375 SHA256:a64c789e3997a2bba012e0c136de9c11b1bc95cf03069c35d26b00582481eecf
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz' nettle_3.5.1+really3.5.1.orig.tar.gz 1989593 SHA256:75cca1998761b02e16f2db56da52992aef622bf55a3b45ec538bc2eedadc9419
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz.asc' nettle_3.5.1+really3.5.1.orig.tar.gz.asc 573 SHA256:557116e471c7c4556148866b5cec056d6de5f26d080e5930154018be6a9d893e
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.debian.tar.xz' nettle_3.5.1+really3.5.1-2.debian.tar.xz 20044 SHA256:7e816adb06d13913bcd350ca6cb777230b82508ca2d358a4062e5676bf335529
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.5.1+really3.5.1-2/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.5.1+really3.5.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.5.1+really3.5.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nghttp2=1.40.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.40.0-1`

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
$ apt-get source -qq --print-uris nghttp2=1.40.0-1
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.40.0-1.dsc' nghttp2_1.40.0-1.dsc 2548 SHA256:92de95dcdf9e2a84a7ea1be6a52df510910e376937ec1f75bc75654f04f846ea
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.40.0.orig.tar.bz2' nghttp2_1.40.0.orig.tar.bz2 1937537 SHA256:82758e13727945f2408d0612762e4655180b039f058d5ff40d055fa1497bd94f
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.40.0-1.debian.tar.xz' nghttp2_1.40.0-1.debian.tar.xz 12692 SHA256:7c8589297f5da5f0995aa8bd08bfbe4764da6d841338df61d7b69ab1f5fcfedb
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.40.0-1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.40.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.40.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `npth=1.6-1`

Binary Packages:

- `libnpth0:amd64=1.6-1`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-1
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6-1.dsc' npth_1.6-1.dsc 1925 SHA256:2c327ce494f702482e79ed620445cba303c4449dd0768fecee3ee7d5ade2544a
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA256:1393abd9adcf0762d34798dc34fdcf4d0d22a8410721e76f1e3afcd1daa4e2d1
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.6-1.debian.tar.xz' npth_1.6-1.debian.tar.xz 10532 SHA256:d312d4a3cf1d082e2f2cf3ea752c41d34f7e120f77a941c6c1680e6093834353
```

Other potentially useful URLs:

- https://sources.debian.net/src/npth/1.6-1/ (for browsing the source)
- https://sources.debian.net/src/npth/1.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/npth/1.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `numactl=2.0.12-1`

Binary Packages:

- `libnuma1:amd64=2.0.12-1+b1`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.12-1
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.12-1.dsc' numactl_2.0.12-1.dsc 2033 SHA256:3b308b110de0728c5524b3135d871e55ebb6e4b93cdc583e93c4222219fe4d08
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.12.orig.tar.gz' numactl_2.0.12.orig.tar.gz 421425 SHA256:2e67513a62168de4777da20d89cdab66d75bcd3badc4256f6b190a8111cd93f8
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.12-1.debian.tar.xz' numactl_2.0.12-1.debian.tar.xz 6756 SHA256:966724cac8f309b33959ae9922b3e5ab58ea821e2e802d96425e1eaada639a33
```

Other potentially useful URLs:

- https://sources.debian.net/src/numactl/2.0.12-1/ (for browsing the source)
- https://sources.debian.net/src/numactl/2.0.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/numactl/2.0.12-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openexr=2.3.0-6`

Binary Packages:

- `libopenexr-dev=2.3.0-6`
- `libopenexr24:amd64=2.3.0-6`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr24/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.3.0-6
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.3.0-6.dsc' openexr_2.3.0-6.dsc 2678 SHA256:e02a733dff068fbc45286b1f1b99610e4a8234abd2720ba7a6317f483c2369d1
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.3.0.orig.tar.gz' openexr_2.3.0.orig.tar.gz 18416222 SHA256:1dea3145eb3962025e27edb99c97e8cfc67d6310403bbd643e97c364ebf8ff09
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.3.0.orig.tar.gz.asc' openexr_2.3.0.orig.tar.gz.asc 566 SHA256:809172c26aacae76d2caf92d13015ec829853f1ea9b25512c0307c66005e4dcc
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_2.3.0-6.debian.tar.xz' openexr_2.3.0-6.debian.tar.xz 20968 SHA256:38fc6e887d7bb8c0003e353f90cfbbfb61c986e7d0e349182426e64a2f1c48e8
```

Other potentially useful URLs:

- https://sources.debian.net/src/openexr/2.3.0-6/ (for browsing the source)
- https://sources.debian.net/src/openexr/2.3.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openexr/2.3.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openjpeg2=2.3.1-1`

Binary Packages:

- `libopenjp2-7:amd64=2.3.1-1`
- `libopenjp2-7-dev=2.3.1-1`

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
$ apt-get source -qq --print-uris openjpeg2=2.3.1-1
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.3.1-1.dsc' openjpeg2_2.3.1-1.dsc 2585 SHA256:5d7d50db6a138c9f7a92563375cd95955651f63131a765e83e1722ef4aa72b1c
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.3.1.orig.tar.xz' openjpeg2_2.3.1.orig.tar.xz 1381768 SHA256:69d39843a25f1a482e1b568fd042eb34837ffc0d708ab7717edeb52e592ecbeb
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.3.1-1.debian.tar.xz' openjpeg2_2.3.1-1.debian.tar.xz 18456 SHA256:ae77564e1fb581fbed5a6bc09e6948de018f0c457f6b7c9d34721985d236c9fe
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjpeg2/2.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/openjpeg2/2.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjpeg2/2.3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.49+dfsg-1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.49+dfsg-1`
- `libldap-common=2.4.49+dfsg-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.49+dfsg-1
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.49+dfsg-1.dsc' openldap_2.4.49+dfsg-1.dsc 3021 SHA256:7de1a33e64558670082c02565c3cabf5d8e16f20b6bd621742276ad0865a92b8
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.49+dfsg.orig.tar.gz' openldap_2.4.49+dfsg.orig.tar.gz 4844726 SHA256:240022395b438f327aa860a631c1d4eef9b17e63ec8965d3aca2aa983e6d81e6
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.49+dfsg-1.debian.tar.xz' openldap_2.4.49+dfsg-1.debian.tar.xz 166556 SHA256:28a6a0c853b8b934958121ead4c62d6ea50091775c389b5b4f1bb78f08d7d74a
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.49+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.49+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.49+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:8.2p1-3`

Binary Packages:

- `openssh-client=1:8.2p1-3`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Beer-ware`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openssh/1:8.2p1-3/


### `dpkg` source package: `openssl=1.1.1d-2`

Binary Packages:

- `libssl-dev:amd64=1.1.1d-2`
- `libssl1.1:amd64=1.1.1d-2`
- `openssl=1.1.1d-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1d-2
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d-2.dsc' openssl_1.1.1d-2.dsc 2440 SHA256:8d23913ef62095e8b3fd21cbc07f84af5e9af60a2cf50c437a23732f0110e065
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d.orig.tar.gz' openssl_1.1.1d.orig.tar.gz 8845861 SHA256:1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d.orig.tar.gz.asc' openssl_1.1.1d.orig.tar.gz.asc 488 SHA256:f3fd3299a79421fffd51d35f62636b8e987dab1d3033d93a19d7685868e15395
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d-2.debian.tar.xz' openssl_1.1.1d-2.debian.tar.xz 84860 SHA256:2f091763c82f28944b6a126aba1beda07573edd417d4929415cd2f13d9bc14ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.1d-2/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.1d-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.1d-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.20-1`

Binary Packages:

- `libp11-kit-dev:amd64=0.23.20-1`
- `libp11-kit0:amd64=0.23.20-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit-dev/copyright`, `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.20-1
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.20-1.dsc' p11-kit_0.23.20-1.dsc 2417 SHA256:daeef2f874a7346062402ed262b9487b442c026ecd74081c1ab37c0dcefc0f5e
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.20.orig.tar.xz' p11-kit_0.23.20.orig.tar.xz 822588 SHA256:14d86024c3dfd6b967d9bc0b4ec7b2973014fe7423481f4d230a1a63b8aa6104
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.20.orig.tar.xz.asc' p11-kit_0.23.20.orig.tar.xz.asc 854 SHA256:6429a15c3c071629add6712ed75916df90043d47250edb9235d89ee197f613b8
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.20-1.debian.tar.xz' p11-kit_0.23.20-1.debian.tar.xz 21940 SHA256:beed598e93d4fee5b49c42099b41c66f634057a424ec90fbd78643cf0dc5c4b0
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.23.20-1/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.23.20-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.23.20-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.3.1-5`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5`
- `libpam-modules-bin=1.3.1-5`
- `libpam-runtime=1.3.1-5`
- `libpam0g:amd64=1.3.1-5`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.3.1-5.dsc' pam_1.3.1-5.dsc 2648 SHA256:6be33a9db415ff3e474a10d1a0c41fca3dbe90ae8c9ddd9a4a997892b11d67ab
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA256:eff47a4ecd833fbf18de9686632a70ee8d0794b79aecb217ebd0ce11db4cd0db
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.3.1-5.debian.tar.xz' pam_1.3.1-5.debian.tar.xz 114384 SHA256:be2c2b27efd6bea02f9d102d7d8c58374557beb7245b2a9d75ecc829e9449f62
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.3.1-5/ (for browsing the source)
- https://sources.debian.net/src/pam/1.3.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.3.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pango1.0=1.42.4-8`

Binary Packages:

- `libpango-1.0-0:amd64=1.42.4-8`
- `libpangocairo-1.0-0:amd64=1.42.4-8`
- `libpangoft2-1.0-0:amd64=1.42.4-8`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Example`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.42.4-8
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.42.4-8.dsc' pango1.0_1.42.4-8.dsc 3428 SHA256:e754f04afe84a7794b461e1cb9baf65fe2fc6e63e74f96378f8a4cd49118e8c3
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.42.4.orig.tar.xz' pango1.0_1.42.4.orig.tar.xz 833876 SHA256:1d2b74cd63e8bd41961f2f8d952355aa0f9be6002b52c8aa7699d9f5da597c9d
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.42.4-8.debian.tar.xz' pango1.0_1.42.4-8.debian.tar.xz 51148 SHA256:5c82cabf356785d8a6688643472e421da35db1208266453f876db6585d53d5b6
```

Other potentially useful URLs:

- https://sources.debian.net/src/pango1.0/1.42.4-8/ (for browsing the source)
- https://sources.debian.net/src/pango1.0/1.42.4-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pango1.0/1.42.4-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `patch=2.7.6-6`

Binary Packages:

- `patch=2.7.6-6`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-6
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-6.dsc' patch_2.7.6-6.dsc 1699 SHA256:ad31c243b982ad8dede14f7b4dfe5bb798bb1dc6d4e28c51a797c3af58477c13
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-6.debian.tar.xz' patch_2.7.6-6.debian.tar.xz 14464 SHA256:75ea94b265763b65005381f1eceeaf3351a70ec5c3243bc161d702776414db02
```

Other potentially useful URLs:

- https://sources.debian.net/src/patch/2.7.6-6/ (for browsing the source)
- https://sources.debian.net/src/patch/2.7.6-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/patch/2.7.6-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.34-7`

Binary Packages:

- `libpcre2-16-0:amd64=10.34-7`
- `libpcre2-32-0:amd64=10.34-7`
- `libpcre2-8-0:amd64=10.34-7`
- `libpcre2-dev:amd64=10.34-7`
- `libpcre2-posix2:amd64=10.34-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.34-7
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.34-7.dsc' pcre2_10.34-7.dsc 2286 SHA256:c3e2bfd8fabf594238b3f17074dc8ac483aaf80a9f12dbfe927b80a74558732e
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.34.orig.tar.gz' pcre2_10.34.orig.tar.gz 2271533 SHA256:da6aba7ba2509e918e41f4f744a59fa41a2425c59a298a232e7fe85691e00379
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.34-7.diff.gz' pcre2_10.34-7.diff.gz 7068 SHA256:7d44ac1b171ef7f7051213a3a8505b28f3809ed3e2fb348567a29fdf5f2b5fdf
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.34-7/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.34-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.34-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.39-12`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-12+b1`
- `libpcre3:amd64=2:8.39-12+b1`
- `libpcre3-dev:amd64=2:8.39-12+b1`
- `libpcre32-3:amd64=2:8.39-12+b1`
- `libpcrecpp0v5:amd64=2:8.39-12+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-12
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-12.dsc' pcre3_8.39-12.dsc 2226 SHA256:7660921533f286d211bc129318327041ceb80d3d21e91c1ae7c10f284342c5e0
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-12.debian.tar.gz' pcre3_8.39-12.debian.tar.gz 26509 SHA256:ee193ddee446f0bdb966fca5987ef871da7a528a473304285619988102371c4c
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre3/2:8.39-12/ (for browsing the source)
- https://sources.debian.net/src/pcre3/2:8.39-12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre3/2:8.39-12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.30.0-9`

Binary Packages:

- `libperl5.30:amd64=5.30.0-9`
- `perl=5.30.0-9`
- `perl-base=5.30.0-9`
- `perl-modules-5.30=5.30.0-9`

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
$ apt-get source -qq --print-uris perl=5.30.0-9
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.0-9.dsc' perl_5.30.0-9.dsc 2983 SHA256:05eb4e5e304ed6d5d198405fa2f85d0d3decc7342536508d240c3f41e07906b1
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.0.orig-regen-configure.tar.gz' perl_5.30.0.orig-regen-configure.tar.gz 833235 SHA256:fc55a7309f9e2c404119b005774fc85a8488bad047aee611d17bbe2d608bf4de
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.0.orig.tar.xz' perl_5.30.0.orig.tar.xz 12419868 SHA256:ac501cad4af904d33370a9ea39dbb7a8ad4cb19bc7bc8a9c17d8dc3e81ef6306
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.0-9.debian.tar.xz' perl_5.30.0-9.debian.tar.xz 161876 SHA256:6140c1b94ba811aad5cab98041f5ccae26a86f619fc738194956ef7fb707b552
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.30.0-9/ (for browsing the source)
- https://sources.debian.net/src/perl/5.30.0-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.30.0-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.1.0-3`

Binary Packages:

- `pinentry-curses=1.1.0-3+b1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-3
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-3.dsc' pinentry_1.1.0-3.dsc 2060 SHA256:007e0ef8f0c289d8df814c2ef6fc66c880eb587f4b2ffcab2e229ea324076921
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-3.debian.tar.xz' pinentry_1.1.0-3.debian.tar.xz 17124 SHA256:41315d69b0c0c06f2c1bff846b2d87519a6fa59e8d295d9e6d1a6b7e343b6168
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.1.0-3/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.1.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.1.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pixman=0.36.0-1`

Binary Packages:

- `libpixman-1-0:amd64=0.36.0-1`
- `libpixman-1-dev:amd64=0.36.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.36.0-1
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.36.0-1.dsc' pixman_0.36.0-1.dsc 2040 SHA256:cd14652763bce32b699778c9a2d73d1bd01384754b1c259ab86cebba083c4aaf
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.36.0.orig.tar.gz' pixman_0.36.0.orig.tar.gz 881544 SHA256:1ca19c8d4d37682adfbc42741d24977903fec1169b4153ec05bb690d4acf9fae
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.36.0-1.diff.gz' pixman_0.36.0-1.diff.gz 322741 SHA256:59b44243d485e97bd47ffa845da9e300a18bce37e4cb49793eb0cd2ac5c6de43
```

Other potentially useful URLs:

- https://sources.debian.net/src/pixman/0.36.0-1/ (for browsing the source)
- https://sources.debian.net/src/pixman/0.36.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pixman/0.36.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pkg-config=0.29-6`

Binary Packages:

- `pkg-config=0.29-6`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29-6
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29-6.dsc' pkg-config_0.29-6.dsc 1757 SHA256:a5f1a8f976f3d8ad579341ba73514eb3af9dbc6bad8d2b5828699ac24196624f
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.orig.tar.gz' pkg-config_0.29.orig.tar.gz 1973875 SHA256:c8507705d2a10c67f385d66ca2aae31e81770cc0734b4191eb8c489e864a006b
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29-6.diff.gz' pkg-config_0.29-6.diff.gz 8145 SHA256:c06146d878fb7faa4ac3edb5e45188b184cc650a752384d5c1053f41edf590bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/pkg-config/0.29-6/ (for browsing the source)
- https://sources.debian.net/src/pkg-config/0.29-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pkg-config/0.29-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `postgresql-12=12.2-1`

Binary Packages:

- `libpq-dev=12.2-1`
- `libpq5:amd64=12.2-1`

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
$ apt-get source -qq --print-uris postgresql-12=12.2-1
'http://deb.debian.org/debian/pool/main/p/postgresql-12/postgresql-12_12.2-1.dsc' postgresql-12_12.2-1.dsc 3591 SHA256:2a1f0fe2f9187579b7d6be5811c2c9e8246a4fc6576bf866d5b041080b0173c4
'http://deb.debian.org/debian/pool/main/p/postgresql-12/postgresql-12_12.2.orig.tar.bz2' postgresql-12_12.2.orig.tar.bz2 20363545 SHA256:ad1dcc4c4fc500786b745635a9e1eba950195ce20b8913f50345bb7d5369b5de
'http://deb.debian.org/debian/pool/main/p/postgresql-12/postgresql-12_12.2-1.debian.tar.xz' postgresql-12_12.2-1.debian.tar.xz 22796 SHA256:cf7bba725dfd2d8094ef0d1c808761f20868a001f0de2ca0affe046fb5407648
```

Other potentially useful URLs:

- https://sources.debian.net/src/postgresql-12/12.2-1/ (for browsing the source)
- https://sources.debian.net/src/postgresql-12/12.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/postgresql-12/12.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.16-1`

Binary Packages:

- `libprocps8:amd64=2:3.3.16-1+b1`
- `procps=2:3.3.16-1+b1`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/procps/2:3.3.16-1/


### `dpkg` source package: `python-defaults=2.7.17-2`

Binary Packages:

- `libpython-stdlib:amd64=2.7.17-2`
- `libpython2-stdlib:amd64=2.7.17-2`
- `python=2.7.17-2`
- `python-minimal=2.7.17-2`
- `python2=2.7.17-2`
- `python2-minimal=2.7.17-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.17-2
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.17-2.dsc' python-defaults_2.7.17-2.dsc 2921 SHA256:f28ab77861331f7111235d694b64a43a49eaf89ad180cbc193f9f97ff4648f1b
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.17-2.tar.gz' python-defaults_2.7.17-2.tar.gz 82775 SHA256:8a779233c0e1a2ef64ac77c78c1482aeac82ee55f7917a9316ad73f8b73d41f3
```

Other potentially useful URLs:

- https://sources.debian.net/src/python-defaults/2.7.17-2/ (for browsing the source)
- https://sources.debian.net/src/python-defaults/2.7.17-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python-defaults/2.7.17-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python2.7=2.7.17-1`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.17-1+b1`
- `libpython2.7-stdlib:amd64=2.7.17-1+b1`
- `python2.7=2.7.17-1+b1`
- `python2.7-minimal=2.7.17-1+b1`

Licenses: (parsed from: `/usr/share/doc/libpython2.7-minimal/copyright`, `/usr/share/doc/libpython2.7-stdlib/copyright`, `/usr/share/doc/python2.7/copyright`, `/usr/share/doc/python2.7-minimal/copyright`)

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
$ apt-get source -qq --print-uris python2.7=2.7.17-1
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.17-1.dsc' python2.7_2.7.17-1.dsc 3365 SHA256:edf165ecac0f41f5f2ee605dbb66b6e148f7437b1ebe16a6f1444fb8a6a6da22
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.17.orig.tar.gz' python2.7_2.7.17.orig.tar.gz 17535962 SHA256:f22059d09cdf9625e0a7284d24a13062044f5bf59d93a7f3382190dfa94cecde
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.17-1.diff.gz' python2.7_2.7.17-1.diff.gz 286003 SHA256:a71d752753f7aaf0c6bb49bae5dfa2f35db4265742b4709bbd12d816f9cef5c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/python2.7/2.7.17-1/ (for browsing the source)
- https://sources.debian.net/src/python2.7/2.7.17-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python2.7/2.7.17-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.7.5-3`

Binary Packages:

- `libpython3-stdlib:amd64=3.7.5-3`
- `python3=3.7.5-3`
- `python3-minimal=3.7.5-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-defaults/3.7.5-3/


### `dpkg` source package: `python3-stdlib-extensions=3.8.0-1`

Binary Packages:

- `python3-distutils=3.8.0-1`
- `python3-lib2to3=3.8.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-stdlib-extensions/3.8.0-1/


### `dpkg` source package: `python3.7=3.7.6-1`

Binary Packages:

- `libpython3.7-minimal:amd64=3.7.6-1+b1`
- `libpython3.7-stdlib:amd64=3.7.6-1+b1`
- `python3.7=3.7.6-1+b1`
- `python3.7-minimal=3.7.6-1+b1`

Licenses: (parsed from: `/usr/share/doc/libpython3.7-minimal/copyright`, `/usr/share/doc/libpython3.7-stdlib/copyright`, `/usr/share/doc/python3.7/copyright`, `/usr/share/doc/python3.7-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.7=3.7.6-1
'http://deb.debian.org/debian/pool/main/p/python3.7/python3.7_3.7.6-1.dsc' python3.7_3.7.6-1.dsc 3419 SHA256:876813147196de00c6a170f7dfb1a64f1b15e89762cd5b24e7b65f086340ee70
'http://deb.debian.org/debian/pool/main/p/python3.7/python3.7_3.7.6.orig.tar.xz' python3.7_3.7.6.orig.tar.xz 17246360 SHA256:55a2cce72049f0794e9a11a84862e9039af9183603b78bc60d89539f82cf533f
'http://deb.debian.org/debian/pool/main/p/python3.7/python3.7_3.7.6-1.debian.tar.xz' python3.7_3.7.6-1.debian.tar.xz 210836 SHA256:79d6a096101ac426a15a8d58971455715170d5ccc291a70b3d5b4700b203395f
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.7/3.7.6-1/ (for browsing the source)
- https://sources.debian.net/src/python3.7/3.7.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.7/3.7.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.0-4`

Binary Packages:

- `libreadline-dev:amd64=8.0-4`
- `libreadline8:amd64=8.0-4`
- `readline-common=8.0-4`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.0-4
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.0-4.dsc' readline_8.0-4.dsc 2434 SHA256:ac9c7bb7380fe740aef09f54becf482eb81032a33dc11f1a8f00e933c5f168f4
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.0.orig.tar.gz' readline_8.0.orig.tar.gz 2975937 SHA256:e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.0-4.debian.tar.xz' readline_8.0-4.debian.tar.xz 30408 SHA256:60ed18dab6d6b7fc998a263d917f06d9cce6e1ccd19cd8bf4a9d33c5350cf8d6
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/8.0-4/ (for browsing the source)
- https://sources.debian.net/src/readline/8.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/8.0-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2+b1`

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

### `dpkg` source package: `sed=4.7-1`

Binary Packages:

- `sed=4.7-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.7-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.7-1.dsc' sed_4.7-1.dsc 1880 SHA256:dd0e8daed987929920f7729771f9c7a5b48d094923aaf686efd2ab19db776108
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.7.orig.tar.xz' sed_4.7.orig.tar.xz 1298316 SHA256:2885768cd0a29ff8d58a6280a270ff161f6a3deb5690b2be6c49f46d4c67bd6a
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.7-1.debian.tar.xz' sed_4.7-1.debian.tar.xz 59824 SHA256:a2ab8d50807fd2242f86d6c6257399e790445ab6f8932f7f487d34361b4fc483
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.7-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.7-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.12+nmu1.dsc' sensible-utils_0.0.12+nmu1.dsc 1753 SHA256:68bcb3e542e29a8a0bf281d9145d0e4cd9def529af2ba0cfe0afee3c5af958bc
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.12+nmu1.tar.xz' sensible-utils_0.0.12+nmu1.tar.xz 61988 SHA256:53c6606facf083adbbf0da04e6d774b31ff3f46c7ba36a82d3f182779f4c3f5b
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.12+nmu1/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.12+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.12+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serf=1.3.9-8`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-8`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-8/


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

### `dpkg` source package: `shared-mime-info=1.10-1`

Binary Packages:

- `shared-mime-info=1.10-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.10-1
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.10-1.dsc' shared-mime-info_1.10-1.dsc 2197 SHA256:49efdf90a3b97a58fbe8a5b241f721d89d43f03ad52dc8254a4642f12a20d641
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.10.orig.tar.xz' shared-mime-info_1.10.orig.tar.xz 616800 SHA256:c625a83b4838befc8cafcd54e3619946515d9e44d63d61c4adf7f5513ddfbebf
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.10-1.debian.tar.xz' shared-mime-info_1.10-1.debian.tar.xz 10020 SHA256:7b78639aeac9ba261bcccd572739c2cac813541a7ae7799e8e56de0df693295d
```

Other potentially useful URLs:

- https://sources.debian.net/src/shared-mime-info/1.10-1/ (for browsing the source)
- https://sources.debian.net/src/shared-mime-info/1.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shared-mime-info/1.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.31.1-3`

Binary Packages:

- `libsqlite3-0:amd64=3.31.1-3`
- `libsqlite3-dev:amd64=3.31.1-3`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.31.1-3
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.31.1-3.dsc' sqlite3_3.31.1-3.dsc 2404 SHA256:7d16c28595f8f1c7b478e77dbbdf3b65cc66a50be8333e47533d9c702f12cc28
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.31.1.orig-www.tar.xz' sqlite3_3.31.1.orig-www.tar.xz 5764424 SHA256:cab01c285fad4eb08bd1e3659cde5a44e17e024badbe9ed01b2de9c625ed0831
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.31.1.orig.tar.xz' sqlite3_3.31.1.orig.tar.xz 7108036 SHA256:dfa6eda312d391d33b7790b061f533d723dc5c30b60720ddd98c89a6fb29272f
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.31.1-3.debian.tar.xz' sqlite3_3.31.1-3.debian.tar.xz 24920 SHA256:01d8e3fa88c420d869d1cfab833e7824726e1003cf56904d77bf4586620cceaa
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.31.1-3/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.31.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.31.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `subversion=1.13.0-2`

Binary Packages:

- `libsvn1:amd64=1.13.0-2+b1`
- `subversion=1.13.0-2+b1`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `AFL-3`
- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
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
$ apt-get source -qq --print-uris subversion=1.13.0-2
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.13.0-2.dsc' subversion_1.13.0-2.dsc 3642 SHA256:456d79d9e611853b3078189a0570a90b8fdc17a531f202bb210dfc45fb070267
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.13.0.orig.tar.gz' subversion_1.13.0.orig.tar.gz 11544359 SHA256:daad440c03b8a86fcca804ea82217bb1902cfcae1b7d28c624143c58dcb96931
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.13.0.orig.tar.gz.asc' subversion_1.13.0.orig.tar.gz.asc 2954 SHA256:ed4f87b947b8172fcaa4c741d8ccc7929914b18cf1ccffc32b4f159fdee3070d
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.13.0-2.debian.tar.xz' subversion_1.13.0-2.debian.tar.xz 420740 SHA256:56f1555b9adfa8dc10a4ff6773022a35befa45cd47b7b43024507a686d0f78bb
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.13.0-2/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.13.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.13.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=244.3-1`

Binary Packages:

- `libsystemd0:amd64=244.3-1`
- `libudev1:amd64=244.3-1`

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
$ apt-get source -qq --print-uris systemd=244.3-1
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_244.3-1.dsc' systemd_244.3-1.dsc 5021 SHA256:d7d85eec660b8ef508ddeaeb74352d31dd1fc8d471c547d9cb5d0fad422e3cfd
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_244.3.orig.tar.gz' systemd_244.3.orig.tar.gz 8484735 SHA256:e6b463733da5eb37075352a64112d030b8612935a54e5b3468279a4f15a4cec4
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_244.3-1.debian.tar.xz' systemd_244.3-1.debian.tar.xz 146912 SHA256:d2626042bf41acaf5a9c83dfaa4792e3cf89722e267356b4e2a8f48fc09f1475
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/244.3-1/ (for browsing the source)
- https://sources.debian.net/src/systemd/244.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/244.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=2.96-2.1`

Binary Packages:

- `sysvinit-utils=2.96-2.1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-2.1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-2.1.dsc' sysvinit_2.96-2.1.dsc 2607 SHA256:fe5e8f60f225dc1a2af6b68f5d99e0af4e09e02f8da0a4883a52e579819d8f97
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA256:2a2e26b72aa235a23ab1c8471005f890309ce1196c83fbc9413c57b9ab62b587
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA256:dfc184b95da12c8c888c8ae6b0f26fe8a23b07fbcdd240f6600a8a78b9439fa0
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-2.1.debian.tar.xz' sysvinit_2.96-2.1.debian.tar.xz 128084 SHA256:f2459926be2d0ce07c75b2c93548ac7fedd1e445f17879109ab28dde8fe4829b
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.96-2.1/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.96-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.96-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.30+dfsg-6`

Binary Packages:

- `tar=1.30+dfsg-6+b1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.30+dfsg-6
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg-6.dsc' tar_1.30+dfsg-6.dsc 1995 SHA256:1515951c8a2fc9a43e822efd82d9043cdec4bec47ddca9e7f1311c73e6b00d0c
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA256:c02f3747ffe02017878303dde8b78e79cd220364c5e8048cf92320232e38912d
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg-6.debian.tar.xz' tar_1.30+dfsg-6.debian.tar.xz 22124 SHA256:b7caae6287992536353413e7a9b21301b29c32066bb6f36b7190074af9dd5c50
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.30+dfsg-6/ (for browsing the source)
- https://sources.debian.net/src/tar/1.30+dfsg-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.30+dfsg-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.1.0+git191117-2`

Binary Packages:

- `libtiff-dev:amd64=4.1.0+git191117-2`
- `libtiff5:amd64=4.1.0+git191117-2`
- `libtiffxx5:amd64=4.1.0+git191117-2`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.1.0+git191117-2
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.1.0+git191117-2.dsc' tiff_4.1.0+git191117-2.dsc 2242 SHA256:b206142f5d27dc3e5cdc005266a848afdc59a23f42f9fb9e93de33c38aaf85f6
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.1.0+git191117.orig.tar.xz' tiff_4.1.0+git191117.orig.tar.xz 1533524 SHA256:67e1d045e994adb7144b0cca228d70dd6d520aaf8c75c342064bc0fd601e6e42
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.1.0+git191117-2.debian.tar.xz' tiff_4.1.0+git191117-2.debian.tar.xz 19384 SHA256:faaeeccdd5d1484b4ef2e8c4c6e31a3ebbad2ae947c5e4caba6de564c8958a00
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.1.0+git191117-2/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.1.0+git191117-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.1.0+git191117-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2019c-3`

Binary Packages:

- `tzdata=2019c-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2019c-3
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c-3.dsc' tzdata_2019c-3.dsc 2237 SHA256:a8386447081f524b10fd3dc4070a8de25d511613b7a127430485af00a45012f1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c.orig.tar.gz' tzdata_2019c.orig.tar.gz 392087 SHA256:79c7806dab09072308da0e3d22c37d3b245015a591891ea147d3b133b60ffc7c
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c.orig.tar.gz.asc' tzdata_2019c.orig.tar.gz.asc 833 SHA256:cd31deaeee229d45e4f4b973441189e7619ef81679359e9c8b47b2a87aaf6a07
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c-3.debian.tar.xz' tzdata_2019c-3.debian.tar.xz 105024 SHA256:50020c99a5babd90c73829cb47225f69669eb0e95c5fae272a06226837c7dd3d
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2019c-3/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2019c-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2019c-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ucf=3.0038+nmu1`

Binary Packages:

- `ucf=3.0038+nmu1`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0038+nmu1
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0038+nmu1.dsc' ucf_3.0038+nmu1.dsc 1420 SHA256:89b6f921a30e04a946f62e6996be7c16f2f7c383d20783cd4704b502c6d5b125
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0038+nmu1.tar.xz' ucf_3.0038+nmu1.tar.xz 65860 SHA256:d00bc3dd8d2f91317f52b5352fe129023c72babad55bc0dd4ece7b34183c7436
```

Other potentially useful URLs:

- https://sources.debian.net/src/ucf/3.0038+nmu1/ (for browsing the source)
- https://sources.debian.net/src/ucf/3.0038+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ucf/3.0038+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unbound=1.9.6-2`

Binary Packages:

- `libunbound8:amd64=1.9.6-2`

Licenses: (parsed from: `/usr/share/doc/libunbound8/copyright`)

- `BSD-2-VUT`
- `BSD-3-ADG`
- `BSD-3-CZ.NIC`
- `BSD-3-Farsight`
- `BSD-3-NLnetLabs`
- `BSD-3-NLnetLabs-Mekking`
- `BSD-3-Regents-DEC`
- `BSD-3-Todd-Miller`
- `BSD-3-VUT`
- `BSD-3-Viagénie`
- `BSD-3-WIDE`
- `GPL-3`
- `GPL-3+ with Bison exception`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris unbound=1.9.6-2
'http://deb.debian.org/debian/pool/main/u/unbound/unbound_1.9.6-2.dsc' unbound_1.9.6-2.dsc 3233 SHA256:2c55fa00478addd9562a7729c5657e24547f0cb216e4b51b6650e3943b4e3920
'http://deb.debian.org/debian/pool/main/u/unbound/unbound_1.9.6.orig.tar.gz' unbound_1.9.6.orig.tar.gz 5680145 SHA256:1d98fc6ea99197a20b4a0e540e87022cf523085786e0fc26de6ebb2720f5aaf0
'http://deb.debian.org/debian/pool/main/u/unbound/unbound_1.9.6.orig.tar.gz.asc' unbound_1.9.6.orig.tar.gz.asc 488 SHA256:0662b11ef0e366f311948ea2ca03ffbad0a015c31bf0b9efc09723b65aa2ecf6
'http://deb.debian.org/debian/pool/main/u/unbound/unbound_1.9.6-2.debian.tar.xz' unbound_1.9.6-2.debian.tar.xz 20712 SHA256:7e7f2a323f3a006d02b011a42d783a2468c086517db2bcedfeeb8fe95e337e24
```

Other potentially useful URLs:

- https://sources.debian.net/src/unbound/1.9.6-2/ (for browsing the source)
- https://sources.debian.net/src/unbound/1.9.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unbound/1.9.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unzip=6.0-25`

Binary Packages:

- `unzip=6.0-25`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-25
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-25.dsc' unzip_6.0-25.dsc 1344 SHA256:ed68c01c7adf04f1599760975facac5a6164351baa2e5035a5239905f14108bb
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-25.debian.tar.xz' unzip_6.0-25.debian.tar.xz 23096 SHA256:0783e4d11d755cb43904e3f59a60dbb92ee9c6b08ac54d86bc61f9848216f37b
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-25/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-25/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-25/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `utf8proc=2.4.0-2`

Binary Packages:

- `libutf8proc2:amd64=2.4.0-2`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.4.0-2
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.4.0-2.dsc' utf8proc_2.4.0-2.dsc 2179 SHA256:0659ec6e1bb112c3ba3c34c8437fff9a29e4091d26f52707951105a776af5a49
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.4.0.orig.tar.gz' utf8proc_2.4.0.orig.tar.gz 154936 SHA256:b2e5d547c1d94762a6d03a7e05cea46092aab68636460ff8648f1295e2cdfbd7
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.4.0-2.debian.tar.xz' utf8proc_2.4.0-2.debian.tar.xz 5176 SHA256:c7bc0f534b4be6574c91250b57902c47a6552a66faa95385218fb7f9d7a9063d
```

Other potentially useful URLs:

- https://sources.debian.net/src/utf8proc/2.4.0-2/ (for browsing the source)
- https://sources.debian.net/src/utf8proc/2.4.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/utf8proc/2.4.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.34-0.1`

Binary Packages:

- `bsdutils=1:2.34-0.1`
- `fdisk=2.34-0.1`
- `libblkid-dev:amd64=2.34-0.1`
- `libblkid1:amd64=2.34-0.1`
- `libfdisk1:amd64=2.34-0.1`
- `libmount-dev:amd64=2.34-0.1`
- `libmount1:amd64=2.34-0.1`
- `libsmartcols1:amd64=2.34-0.1`
- `libuuid1:amd64=2.34-0.1`
- `mount=2.34-0.1`
- `util-linux=2.34-0.1`
- `uuid-dev:amd64=2.34-0.1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.34-0.1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.34-0.1.dsc' util-linux_2.34-0.1.dsc 3949 SHA256:9f7476f7820aade0c688c6defb2337cb08f275e8eede4743368d91ec46a44563
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.34.orig.tar.xz' util-linux_2.34.orig.tar.xz 4974812 SHA256:743f9d0c7252b6db246b659c1e1ce0bd45d8d4508b4dfa427bbb4a3e9b9f62b5
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.34-0.1.debian.tar.xz' util-linux_2.34-0.1.debian.tar.xz 82012 SHA256:06d686fd64c43d129c67162bca90ec405fa50177f08449b91fc748a1acad48ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.34-0.1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.34-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.34-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.20.3-1`

Binary Packages:

- `wget=1.20.3-1+b2`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.20.3-1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.20.3-1.dsc' wget_1.20.3-1.dsc 2167 SHA256:4c27fab3592ff0289ebda9925f7139a514291e47ecdc796fdb56ba6330022e67
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.20.3.orig.tar.gz' wget_1.20.3.orig.tar.gz 4489249 SHA256:31cccfc6630528db1c8e3a06f6decf2a370060b982841cfab2b8677400a5092e
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.20.3.orig.tar.gz.asc' wget_1.20.3.orig.tar.gz.asc 833 SHA256:7b295c84ab6f90c328a203e234e4b2f5f45cb8d2e29eac43a977073933cd49a2
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.20.3-1.debian.tar.xz' wget_1.20.3-1.debian.tar.xz 60416 SHA256:0dcc2df1280dda94deb812c154b42cc819af9abdaa0d57e963db4edca1c0fb1d
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.20.3-1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.20.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.20.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x265=3.2.1-1`

Binary Packages:

- `libx265-179:amd64=3.2.1-1`

Licenses: (parsed from: `/usr/share/doc/libx265-179/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=3.2.1-1
'http://deb.debian.org/debian/pool/main/x/x265/x265_3.2.1-1.dsc' x265_3.2.1-1.dsc 2243 SHA256:e463f9ced3bf7638b1c25dbaaa470b6b49aba04acb5e5fa7d30a0c1d80d9ba01
'http://deb.debian.org/debian/pool/main/x/x265/x265_3.2.1.orig.tar.gz' x265_3.2.1.orig.tar.gz 1426255 SHA256:fb9badcf92364fd3567f8b5aa0e5e952aeea7a39a2b864387cec31e3b58cbbcc
'http://deb.debian.org/debian/pool/main/x/x265/x265_3.2.1-1.debian.tar.xz' x265_3.2.1-1.debian.tar.xz 13092 SHA256:e9e81b61d589f0db50a8283a18ba57fff18cbdc172c15f178360c2d75157e7ac
```

Other potentially useful URLs:

- https://sources.debian.net/src/x265/3.2.1-1/ (for browsing the source)
- https://sources.debian.net/src/x265/3.2.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x265/3.2.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorg-sgml-doctools=1:1.11-1`

Binary Packages:

- `xorg-sgml-doctools=1:1.11-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xorg-sgml-doctools=1:1.11-1
'http://deb.debian.org/debian/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.dsc' xorg-sgml-doctools_1.11-1.dsc 1975 SHA256:1f4a12a38420b0ddab35553b9588fdf43ab39577958aed70fca435c9a747141a
'http://deb.debian.org/debian/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11.orig.tar.gz' xorg-sgml-doctools_1.11.orig.tar.gz 150367 SHA256:986326d7b4dd2ad298f61d8d41fe3929ac6191c6000d6d7e47a8ffc0c34e7426
'http://deb.debian.org/debian/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.diff.gz' xorg-sgml-doctools_1.11-1.diff.gz 3194 SHA256:18eeb355cb0efff9f47f8ed8e852eee322d9733a427419f4b39f43bc4df630c1
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg-sgml-doctools/1:1.11-1/ (for browsing the source)
- https://sources.debian.net/src/xorg-sgml-doctools/1:1.11-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg-sgml-doctools/1:1.11-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorg=1:7.7+20`

Binary Packages:

- `x11-common=1:7.7+20`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+20
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+20.dsc' xorg_7.7+20.dsc 1969 SHA256:e24781dcf02522f070811acdeaba7113b560c61148a692c6b74719aacd85bd0b
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+20.tar.gz' xorg_7.7+20.tar.gz 286646 SHA256:2da7138a6f437ce7ccf63e36786b17053ffbdbcf177dab4874260bfa54595b5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg/1:7.7+20/ (for browsing the source)
- https://sources.debian.net/src/xorg/1:7.7+20/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg/1:7.7+20/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorgproto=2018.4-4`

Binary Packages:

- `x11proto-core-dev=2018.4-4`
- `x11proto-dev=2018.4-4`
- `x11proto-xext-dev=2018.4-4`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`, `/usr/share/doc/x11proto-xext-dev/copyright`)

- `MIT`
- `SGI`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/xorgproto/2018.4-4/


### `dpkg` source package: `xtrans=1.3.5-1`

Binary Packages:

- `xtrans-dev=1.3.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/xtrans/1.3.5-1/


### `dpkg` source package: `xz-utils=5.2.4-1`

Binary Packages:

- `liblzma-dev:amd64=5.2.4-1+b1`
- `liblzma5:amd64=5.2.4-1+b1`
- `xz-utils=5.2.4-1+b1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.4-1
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.4-1.dsc' xz-utils_5.2.4-1.dsc 2518 SHA256:b1572c4efb3c8ebf6f0e044b70e1e0451c919a99d3f80be03b624a54dd7ea593
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA256:9717ae363760dedf573dad241420c5fea86256b65bc21d2cf71b2b12f0544f4b
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA256:88290c1deeaf674ae2a4821f4373fe0e4cc2a94199eae6dcc26df1e70cc15303
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.4-1.debian.tar.xz' xz-utils_5.2.4-1.debian.tar.xz 135296 SHA256:d37b558444b76e88a69601df008cf1c0343c58cb7765b7bbb2099b0a19619361
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.4-1/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.4-1/ (for access to the source package after it no longer exists in the archive)

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
