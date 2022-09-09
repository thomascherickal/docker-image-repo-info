# `buildpack-deps:bookworm-scm`

## Docker Metadata

- Image ID: `sha256:5065f8a27ab438502224d3d8c878db108e01f3cc1d35cb19090300d6ba573049`
- Created: `2022-08-23T00:46:34.49188277Z`
- Virtual Size: ~ 318.02 Mb  
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

### `dpkg` source package: `adduser=3.123`

Binary Packages:

- `adduser=3.123`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/adduser/3.123/


### `dpkg` source package: `apr-util=1.6.1-5`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5+b2`

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

### `dpkg` source package: `apt=2.5.2`

Binary Packages:

- `apt=2.5.2`
- `libapt-pkg6.0:amd64=2.5.2`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.5.2
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.5.2.dsc' apt_2.5.2.dsc 2933 SHA256:5bc7d3737d6e281a32ca59c785747cc9f23eafaa5b71ee2d9016b7290f2c54fe
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.5.2.tar.xz' apt_2.5.2.tar.xz 2252960 SHA256:cc5c374c2831c9e390d9c5f08029a81c3ca2b778abc0dd1426c81c657628fe9d
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/2.5.2/ (for browsing the source)
- https://sources.debian.net/src/apt/2.5.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/2.5.2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `audit=1:3.0.7-1`

Binary Packages:

- `libaudit-common=1:3.0.7-1`
- `libaudit1:amd64=1:3.0.7-1+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0.7-1
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.7-1.dsc' audit_3.0.7-1.dsc 2401 SHA256:26295f1e194787a177ec8f8fedb610a0b6543918b37f8eab59bc51e2afce0656
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.7.orig.tar.gz' audit_3.0.7.orig.tar.gz 1180226 SHA256:8b4c78632a9301a1c7f859b0e38fc0b9c260b8214d6b7c771bf28b3d73a62597
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.7-1.debian.tar.xz' audit_3.0.7-1.debian.tar.xz 17700 SHA256:8cc9ce5b529c3c5062a58a2cb0e6ac10f010c334cf973ae3a48d7ebb5a10f57c
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:3.0.7-1/ (for browsing the source)
- https://sources.debian.net/src/audit/1:3.0.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:3.0.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=12.2`

Binary Packages:

- `base-files=12.2`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=12.2
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_12.2.dsc' base-files_12.2.dsc 1078 SHA256:bce25568b596e80923f764c1a2ecfb5022ccee0c4387e8e4785598250852ea7f
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_12.2.tar.xz' base-files_12.2.tar.xz 65760 SHA256:ed45674c39c6051591d6037aac3fb7e97e3ef868c51d3112e8b3234d2e275ac6
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/12.2/ (for browsing the source)
- https://sources.debian.net/src/base-files/12.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/12.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.52`

Binary Packages:

- `base-passwd=3.5.52`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-passwd/3.5.52/


### `dpkg` source package: `bash=5.1-6.1`

Binary Packages:

- `bash=5.1-6.1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/bash/5.1-6.1/


### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2+b4`

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

### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `libbz2-1.0:amd64=1.0.8-5`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

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

### `dpkg` source package: `cdebconf=0.263`

Binary Packages:

- `libdebconfclient0:amd64=0.263`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.263
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.263.dsc' cdebconf_0.263.dsc 2678 SHA256:2a9899e086c2050c97f4eded0677b46ccb5cc54cd6c689fc69b51fa12ca3aa86
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.263.tar.xz' cdebconf_0.263.tar.xz 281880 SHA256:829fdef1c21b822b1f2421857ee62fbf14df246836e8831e44e464fd1f705b05
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.263/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.263/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.263/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `curl=7.84.0-2`

Binary Packages:

- `curl=7.84.0-2`
- `libcurl3-gnutls:amd64=7.84.0-2`
- `libcurl4:amd64=7.84.0-2`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/curl/7.84.0-2/


### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg-7`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg-7`
- `libsasl2-modules-db:amd64=2.1.28+dfsg-7`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-2.2-clause`
- `BSD-3-clause`
- `BSD-3-clause-JANET`
- `BSD-3-clause-PADL`
- `BSD-4-clause`
- `BSD-4-clause-KTH`
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cyrus-sasl2/2.1.28+dfsg-7/


### `dpkg` source package: `dash=0.5.11+git20210903+057cd650a4ed-8`

Binary Packages:

- `dash=0.5.11+git20210903+057cd650a4ed-8`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `Expat`
- `FSFUL`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/dash/0.5.11+git20210903+057cd650a4ed-8/


### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.10`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.10`

Licenses: (parsed from: `/usr/share/doc/libdb5.3/copyright`)

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
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.10
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.10.dsc' db5.3_5.3.28+dfsg1-0.10.dsc 2964 SHA256:7bab820246eb763be7d04fcb2893bedb414f9b3cf7a29327e3530adfbca1963e
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.10.debian.tar.xz' db5.3_5.3.28+dfsg1-0.10.debian.tar.xz 34656 SHA256:2d2b3c6b4643e9c94db58f9540332e23a780d63afdc3fcabe66df01a343d6c65
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.10/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.10/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `debianutils=5.7-0.3`

Binary Packages:

- `debianutils=5.7-0.3`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.7-0.3
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.3.dsc' debianutils_5.7-0.3.dsc 1887 SHA256:134707c6467fb895332cf7520dbb2da33fb8b38b7844dec88e64ceb50647512a
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7.orig.tar.gz' debianutils_5.7.orig.tar.gz 257231 SHA256:27ec9e0e7e44dc8ab611aa576330471bacb07e4491ffecf0d3aa6909c92f9022
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.3.debian.tar.xz' debianutils_5.7-0.3.debian.tar.xz 22120 SHA256:c7117659c2913660e2ffa83aa1362c7a2b49a3f1e20fadcf72e64e589540ffe9
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/5.7-0.3/ (for browsing the source)
- https://sources.debian.net/src/debianutils/5.7-0.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/5.7-0.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.8-1`

Binary Packages:

- `diffutils=1:3.8-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.8-1
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8-1.dsc' diffutils_3.8-1.dsc 1705 SHA256:f00b310d95fce4312f44c4940b374fa3c2b5ccfcb53b6daa4e4a98e2bb47b58a
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz' diffutils_3.8.orig.tar.xz 1585120 SHA256:a6bdd7d1b31266d11c4f4de6c1b748d4607ab0231af5188fc2533d0ae2438fec
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz.asc' diffutils_3.8.orig.tar.xz.asc 833 SHA256:500f423d0ffa8d28966d916ed5fc6b79fb160a20ed5cb74eeb1c94a30c340311
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8-1.debian.tar.xz' diffutils_3.8-1.debian.tar.xz 11004 SHA256:120b1eaecd0cb09eb60cddaf616d269684f2f2b796ee6d9ca7aa4e16af517767
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.8-1/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.21.9`

Binary Packages:

- `dpkg=1.21.9`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.9
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.9.dsc' dpkg_1.21.9.dsc 2120 SHA256:065ee6146fecf372c587fd6f2083cda8704f9b3e20d1816f0972307cdee0c0ac
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.9.tar.xz' dpkg_1.21.9.tar.xz 5084044 SHA256:a0aba375625459260cbc89933a12b3188a713c840e3aaefc14bf2d9adee19642
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.21.9/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.21.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.21.9/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `expat=2.4.8-1`

Binary Packages:

- `libexpat1:amd64=2.4.8-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.4.8-1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.4.8-1.dsc' expat_2.4.8-1.dsc 1981 SHA256:50839f5d81756a26f9ae5ade08bd517ffb23afa07651b71c12a3fa12b0cc2851
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.4.8.orig.tar.gz' expat_2.4.8.orig.tar.gz 8316762 SHA256:122d8ae7a0170b9835cb45b216d856c1f83dd83792f8f0f80c31e98283efbe87
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.4.8-1.debian.tar.xz' expat_2.4.8-1.debian.tar.xz 12556 SHA256:80a1ca6068c2407294d033d3b577fe9d482436a44c16d59eeca94b18487d06c9
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.4.8-1/ (for browsing the source)
- https://sources.debian.net/src/expat/2.4.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.4.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.9.0-3`

Binary Packages:

- `findutils=4.9.0-3`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.9.0-3
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-3.dsc' findutils_4.9.0-3.dsc 2304 SHA256:509979a2aeae2883c16b4bf6e96b4b8df9173a6c56e936e957ce86f25b2b4125
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA256:a2bfb8c09d436770edc59f50fa483e785b161a3b7b9d547573cb08065fd462fe
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA256:924c3719d066eda1b3e47175f8b83e90e9a23f0a639ebe7445621917b283c385
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-3.debian.tar.xz' findutils_4.9.0-3.debian.tar.xz 27980 SHA256:d10dfc7a728d372b60d5455b190b6ee78bc65de0ee3ca4974e1addd90389c675
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.9.0-3/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.9.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.9.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-12=12.1.0-8`

Binary Packages:

- `gcc-12-base:amd64=12.1.0-8`
- `libgcc-s1:amd64=12.1.0-8`
- `libstdc++6:amd64=12.1.0-8`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12.1.0-8
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.1.0-8.dsc' gcc-12_12.1.0-8.dsc 27405 SHA256:75e2dd9b522005d5839bd4c9be5001cfb6490b0dbfd0b59df905cf9971946f0f
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.1.0.orig.tar.gz' gcc-12_12.1.0.orig.tar.gz 87107706 SHA256:90fa78ff37c489553228e8b80dc3c2756dad3d5e704194ecae34f1c27417d517
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.1.0-8.debian.tar.xz' gcc-12_12.1.0-8.debian.tar.xz 1805332 SHA256:b7c3e1baefbb267c2944ee3301a3057108e6c20dd1cbb7ef88aaeb7c0200c95b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-12/12.1.0-8/ (for browsing the source)
- https://sources.debian.net/src/gcc-12/12.1.0-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-12/12.1.0-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.23-1`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-1+b1`
- `libgdbm6:amd64=1.23-1+b1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gdbm/1.23-1/


### `dpkg` source package: `git=1:2.35.1-1`

Binary Packages:

- `git=1:2.35.1-1`
- `git-man=1:2.35.1-1`

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
$ apt-get source -qq --print-uris git=1:2.35.1-1
'http://deb.debian.org/debian/pool/main/g/git/git_2.35.1-1.dsc' git_2.35.1-1.dsc 2825 SHA256:7729b160cbcdd798f0b180ae8c40542321d73e55c00dbd0ec483ddfaf7b7d117
'http://deb.debian.org/debian/pool/main/g/git/git_2.35.1.orig.tar.xz' git_2.35.1.orig.tar.xz 6874520 SHA256:d768528e6443f65a203036266f1ca50f9d127ba89751e32ead37117ed9191080
'http://deb.debian.org/debian/pool/main/g/git/git_2.35.1-1.debian.tar.xz' git_2.35.1-1.debian.tar.xz 708244 SHA256:33b241bcf5b8a8483396878ae44ba204c252735f9b2c10af5b6387e0543579b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.35.1-1/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.35.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.35.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.34-3`

Binary Packages:

- `libc-bin=2.34-3`
- `libc6:amd64=2.34-3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.34-3
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.34-3.dsc' glibc_2.34-3.dsc 9673 SHA256:6e6641424381d7593124f2ffb5b2a19bbcc24ecbcbdba59731980935318195c2
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.34.orig.tar.xz' glibc_2.34.orig.tar.xz 17949940 SHA256:cc13047c7d42748108fc18cf1a4de8ca92f9e5c9bfcee09d6fada21d9a479878
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.34-3.debian.tar.xz' glibc_2.34-3.debian.tar.xz 995252 SHA256:464eb5482bfe62d66a4529937a7fdb08fecebf5d822aa9dd063b6c34c7aca761
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.34-3/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.34-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.34-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.1+dfsg1-1`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg1-1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg1-1
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.dsc' gmp_6.2.1+dfsg1-1.dsc 2230 SHA256:7a2ca2112db9f7ddf46c14d56ee3ed5ffbc7f4b4b33f843c6167533cc4334ae8
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1.orig.tar.xz' gmp_6.2.1+dfsg1.orig.tar.xz 1787428 SHA256:471b9e463e04362a0124f215afc5f0a4b99caedeeb62634c61bbc12988efa64c
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.debian.tar.xz' gmp_6.2.1+dfsg1-1.debian.tar.xz 19244 SHA256:35a11ed82eb0b612cb39e6136099880c4693035ea29d79828a050300a8b6dd6b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg1-1/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.35-3`

Binary Packages:

- `dirmngr=2.2.35-3`
- `gnupg=2.2.35-3`
- `gnupg-l10n=2.2.35-3`
- `gnupg-utils=2.2.35-3`
- `gpg=2.2.35-3`
- `gpg-agent=2.2.35-3`
- `gpg-wks-client=2.2.35-3`
- `gpg-wks-server=2.2.35-3`
- `gpgconf=2.2.35-3`
- `gpgsm=2.2.35-3`
- `gpgv=2.2.35-3`

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

- http://snapshot.debian.org/package/gnupg2/2.2.35-3/


### `dpkg` source package: `gnutls28=3.7.7-2`

Binary Packages:

- `libgnutls30:amd64=3.7.7-2`

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
$ apt-get source -qq --print-uris gnutls28=3.7.7-2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7-2.dsc' gnutls28_3.7.7-2.dsc 3442 SHA256:caf3872d06109c778a247fa690c5056105095cb1e182541e251550675af8fd60
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7.orig.tar.xz' gnutls28_3.7.7.orig.tar.xz 6351664 SHA256:be9143d0d58eab64dba9b77114aaafac529b6c0d7e81de6bdf1c9b59027d2106
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7.orig.tar.xz.asc' gnutls28_3.7.7.orig.tar.xz.asc 996 SHA256:2ca7cc33027c6a2316db52869a4b721f73560e0ade2b7bd758228dbbcebc36e0
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7-2.debian.tar.xz' gnutls28_3.7.7-2.debian.tar.xz 67348 SHA256:54f6f6fc220ad9df6acbb17b6a8d50152eed2150120d4ed2ca89d982c1ccb6ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.7-2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.7-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `init-system-helpers=1.64`

Binary Packages:

- `init-system-helpers=1.64`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.64
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.64.dsc' init-system-helpers_1.64.dsc 1993 SHA256:e2285c0f17182d85aceee57357bba65fe7007d62a0b9fc4ef7e5b10bcfadf1d9
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.64.tar.xz' init-system-helpers_1.64.tar.xz 43400 SHA256:79dee58d7cda9fac5de7e0045e1346b93cf079efc542db21c4bc16acc7358e2a
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.64/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.64/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.64/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.6.3-1`

Binary Packages:

- `libkeyutils1:amd64=1.6.3-1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.3-1
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3-1.dsc' keyutils_1.6.3-1.dsc 2055 SHA256:2c0e828b11a4483b5d1c949384f77d49412559c9f6a7193a1321476830f742be
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3.orig.tar.gz' keyutils_1.6.3.orig.tar.gz 137022 SHA256:a61d5706136ae4c05bd48f86186bcfdbd88dd8bd5107e3e195c924cfc1b39bb4
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3-1.debian.tar.xz' keyutils_1.6.3-1.debian.tar.xz 13136 SHA256:e11ef757e2db97c8c5cd381cc29f3e5e125aa485f8446dc62777ba5a16678a63
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.6.3-1/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.6.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.6.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.20-1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.20-1`
- `libk5crypto3:amd64=1.20-1`
- `libkrb5-3:amd64=1.20-1`
- `libkrb5support0:amd64=1.20-1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20-1
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20-1.dsc' krb5_1.20-1.dsc 3150 SHA256:bcfd574ef97a80f0edf34b90d8cc15b319ca388eab75dae4487711115402460d
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20.orig.tar.gz' krb5_1.20.orig.tar.gz 8660756 SHA256:7e022bdd3c851830173f9faaa006a230a0e0fdad4c953e85bff4bf0da036e12f
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20.orig.tar.gz.asc' krb5_1.20.orig.tar.gz.asc 833 SHA256:ecfecebc6c837952788accf519ba5034a982c46270907e15fe7e2abfa2f468b3
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.20-1.debian.tar.xz' krb5_1.20-1.debian.tar.xz 104112 SHA256:f0c714364e382d277464b69486692730f3abb3f31efd4f733aad32f271d82182
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.20-1/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.20-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.20-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.5.5-4`

Binary Packages:

- `libassuan0:amd64=2.5.5-4`

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
$ apt-get source -qq --print-uris libassuan=2.5.5-4
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-4.dsc' libassuan_2.5.5-4.dsc 1997 SHA256:c4f06cdb1684b44ca17acb7804ee593e2164db5b6911b0a9ed338f840931630f
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2' libassuan_2.5.5.orig.tar.bz2 572263 SHA256:8e8c2fcc982f9ca67dcbb1d95e2dc746b1739a4668bc20b3a3c5be632edb34e4
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2.asc' libassuan_2.5.5.orig.tar.bz2.asc 228 SHA256:8bb0d1d818ac91fa27a8ebed2975dac12eac9a6e075dfba225cc488ac9b4133f
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-4.debian.tar.xz' libassuan_2.5.5-4.debian.tar.xz 13976 SHA256:d9d46edba0c5bff1aec978fb9a894662fe144b1abe2f2e21bea8c98dae3e508c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.5-4/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.5-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.5-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.11.6-1`

Binary Packages:

- `libbsd0:amd64=0.11.6-1`

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
$ apt-get source -qq --print-uris libbsd=0.11.6-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.6-1.dsc' libbsd_0.11.6-1.dsc 2308 SHA256:87136c10fb842fdc55694414ee137d2519c7cee8f0fa6d267cc1e96a532c60ea
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.6.orig.tar.xz' libbsd_0.11.6.orig.tar.xz 416600 SHA256:19b38f3172eaf693e6e1c68714636190c7e48851e45224d720b3b5bc0499b5df
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.6.orig.tar.xz.asc' libbsd_0.11.6.orig.tar.xz.asc 833 SHA256:dd418029c6a0f48831ebdbacfc1b86d35888dfefa40d5dd6f5a26d583dea297c
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.6-1.debian.tar.xz' libbsd_0.11.6-1.debian.tar.xz 17676 SHA256:0dc8631313b5a44e42fcf45af833dae47e22ba04accd2e4223c69f25dcc7a0f3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.11.6-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.11.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.11.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.8.3-1`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1+b1`

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

### `dpkg` source package: `libcbor=0.8.0-2`

Binary Packages:

- `libcbor0.8:amd64=0.8.0-2`

Licenses: (parsed from: `/usr/share/doc/libcbor0.8/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.8.0-2
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0-2.dsc' libcbor_0.8.0-2.dsc 2114 SHA256:ea9cbadf7d9cd9a3f7dcf7467f3e71dd7aab6d06cad15d01b2f0c19a0ad749a7
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0.orig.tar.gz' libcbor_0.8.0.orig.tar.gz 267044 SHA256:618097166ea4a54499646998ccaa949a5816e6a665cf1d6df383690895217c8b
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0-2.debian.tar.xz' libcbor_0.8.0-2.debian.tar.xz 4024 SHA256:48df3ff85250d1e6274a19d9bcc18b5b582a368667120b7bd21d798ca6feccb0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcbor/0.8.0-2/ (for browsing the source)
- https://sources.debian.net/src/libcbor/0.8.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcbor/0.8.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libfido2=1.11.0-1`

Binary Packages:

- `libfido2-1:amd64=1.11.0-1+b1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.11.0-1
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.11.0-1.dsc' libfido2_1.11.0-1.dsc 2588 SHA256:48fe5e1426c45d4fefa14fb7c9b47796a064d36af71d219f7f1c75afdcc9fac6
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.11.0.orig.tar.gz' libfido2_1.11.0.orig.tar.gz 624148 SHA256:0830c5853e3b44099a97166e0cec54a65b54b7faaac07071872f77b8e4d7b302
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.11.0.orig.tar.gz.asc' libfido2_1.11.0.orig.tar.gz.asc 833 SHA256:6628c9a0f479907cd7e92a9bf6c043c007e0b6098d610402b49edfe44929da3b
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.11.0-1.debian.tar.xz' libfido2_1.11.0-1.debian.tar.xz 52472 SHA256:2ec1aaf588e9ed0f9239f623bd0715e87330640a66fd108207b0fee83d2e54d1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfido2/1.11.0-1/ (for browsing the source)
- https://sources.debian.net/src/libfido2/1.11.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfido2/1.11.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.10.1-2`

Binary Packages:

- `libgcrypt20:amd64=1.10.1-2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.1-2
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-2.dsc' libgcrypt20_1.10.1-2.dsc 2790 SHA256:aa95c53382f51ed57490496df3ccb47d0ce11de1995cef78b87f7875eba416fb
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2' libgcrypt20_1.10.1.orig.tar.bz2 3778457 SHA256:ef14ae546b0084cd84259f61a55e07a38c3b53afc0f546bffcef2f01baffe9de
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2.asc' libgcrypt20_1.10.1.orig.tar.bz2.asc 228 SHA256:9da6ae5e8b1c253607be7e951b568932740c143ee519f6b3392ece8211e84e33
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-2.debian.tar.xz' libgcrypt20_1.10.1-2.debian.tar.xz 36788 SHA256:96875b4209984bfd192ce05a06f72f86f2ac2279b987f6d8e2e07cb0c95e2f68
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.10.1-2/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.10.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.10.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.45-2`

Binary Packages:

- `libgpg-error0:amd64=1.45-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.45-2
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45-2.dsc' libgpg-error_1.45-2.dsc 2273 SHA256:aacc0e1d60caf48ada2f8c73fa35bcb0f5e6368dfd301a624f5ede9419835144
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45.orig.tar.bz2' libgpg-error_1.45.orig.tar.bz2 1015954 SHA256:570f8ee4fb4bff7b7495cff920c275002aea2147e9a1d220c068213267f80a26
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45.orig.tar.bz2.asc' libgpg-error_1.45.orig.tar.bz2.asc 390 SHA256:3a4bfe4d36842a74a9f48a961df517efae812f1d6e097d274f8db5783a828508
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45-2.debian.tar.xz' libgpg-error_1.45-2.debian.tar.xz 18820 SHA256:677493c9636cdcbbd7124ee460703dcdf990d4a0982819f006701f94f6285c45
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.45-2/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.45-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.45-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn2=2.3.3-1`

Binary Packages:

- `libidn2-0:amd64=2.3.3-1`

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
$ apt-get source -qq --print-uris libidn2=2.3.3-1
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3-1.dsc' libidn2_2.3.3-1.dsc 2206 SHA256:13865e96a0fed8dcb82767db65c946b56ed44fc1806d80d407c512ded2a83984
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz' libidn2_2.3.3.orig.tar.gz 2116946 SHA256:f3ac987522c00d33d44b323cae424e2cffcb4c63c6aa6cd1376edacbf1c36eb0
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz.asc' libidn2_2.3.3.orig.tar.gz.asc 228 SHA256:e8f2bdce5def6c239c2cc3220e808b19b14d3f7eb3a0e14851dd5c16fc9ad0ec
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3-1.debian.tar.xz' libidn2_2.3.3-1.debian.tar.xz 15964 SHA256:b040c12276e1128394c2f84c97f7e45f340867fa9d0d0a0b9d8f043b1977db99
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libksba=1.6.0-3`

Binary Packages:

- `libksba8:amd64=1.6.0-3`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.0-3
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0-3.dsc' libksba_1.6.0-3.dsc 2472 SHA256:de87d32fced6fe9593815552043eec226aafc7e6a7f6b258c0f1dcf96adb0da5
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2' libksba_1.6.0.orig.tar.bz2 662120 SHA256:dad683e6f2d915d880aa4bed5cea9a115690b8935b78a1bbe01669189307a48b
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2.asc' libksba_1.6.0.orig.tar.bz2.asc 228 SHA256:c695098f67cc837071d899f0e15d993bcf29eaac8f1ca7428ee793d9c62c795c
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0-3.debian.tar.xz' libksba_1.6.0-3.debian.tar.xz 15004 SHA256:17f8f9679d0dcaaa46d9f4974d2090e23d538206c37014177146b6a5201cf414
```

Other potentially useful URLs:

- https://sources.debian.net/src/libksba/1.6.0-3/ (for browsing the source)
- https://sources.debian.net/src/libksba/1.6.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libksba/1.6.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmd=1.0.4-2`

Binary Packages:

- `libmd0:amd64=1.0.4-2`

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
$ apt-get source -qq --print-uris libmd=1.0.4-2
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4-2.dsc' libmd_1.0.4-2.dsc 2264 SHA256:5e060cb277f31e67b91033e05ece00832ca8056decba873b1698a5680414a177
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz' libmd_1.0.4.orig.tar.xz 264472 SHA256:f51c921042e34beddeded4b75557656559cf5b1f2448033b4c1eec11c07e530f
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz.asc' libmd_1.0.4.orig.tar.xz.asc 833 SHA256:32deebe1cfab127ee69a3e8c8caf439e459b7cdcdd7535fe021cb485adc14057
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4-2.debian.tar.xz' libmd_1.0.4-2.debian.tar.xz 10204 SHA256:a27a2221b1a81e192455e2e93da2e313b21e489f6ac2bcf84b0b813dc3fe261b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmd/1.0.4-2/ (for browsing the source)
- https://sources.debian.net/src/libmd/1.0.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmd/1.0.4-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libseccomp=2.5.4-1`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.4-1
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-1.dsc' libseccomp_2.5.4-1.dsc 2676 SHA256:2986473126cb5f3e358fed40ec1482816e1068dbdfe938bf9f80c50afcf32b80
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz' libseccomp_2.5.4.orig.tar.gz 637228 SHA256:d82902400405cf0068574ef3dc1fe5f5926207543ba1ae6f8e7a1576351dcbdb
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz.asc' libseccomp_2.5.4.orig.tar.gz.asc 833 SHA256:af37e70eb422e6f983c1f135a3abb342c3b787716520b71bd774e4906003807f
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-1.debian.tar.xz' libseccomp_2.5.4-1.debian.tar.xz 16264 SHA256:fd7abe7b26a08ca514457fd13302d348d59401616ce3f6809ce15f54e6ebe77d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.5.4-1/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.5.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.5.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.4-1`

Binary Packages:

- `libselinux1:amd64=3.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.4-1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4-1.dsc' libselinux_3.4-1.dsc 2534 SHA256:4035af53388d343f9b5c46ca2867ba32823cf4a2d218ddd590b34ae59c899157
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz' libselinux_3.4.orig.tar.gz 210061 SHA256:77c294a927e6795c2e98f74b5c3adde9c8839690e9255b767c5fca6acff9b779
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz.asc' libselinux_3.4.orig.tar.gz.asc 833 SHA256:5c370bdef7b756697445e6838ba1b2d934f668b244461e36e245f589ec994a24
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4-1.debian.tar.xz' libselinux_3.4-1.debian.tar.xz 29416 SHA256:046ace4ad0092104bdfb0c6e5187131910216c89b8b81a4bce3c2067615c9196
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/3.4-1/ (for browsing the source)
- https://sources.debian.net/src/libselinux/3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=3.4-1`

Binary Packages:

- `libsemanage-common=3.4-1`
- `libsemanage2:amd64=3.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.4-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4-1.dsc' libsemanage_3.4-1.dsc 2570 SHA256:be300e01bbd08706fb6f0ecd349b3585a535d9ff0957265a7c634545ac3515c8
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz' libsemanage_3.4.orig.tar.gz 185177 SHA256:93b423a21600b8e3fb59bb925d4583d1258f45bebf63c29bde304dfd3d52efd6
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz.asc' libsemanage_3.4.orig.tar.gz.asc 833 SHA256:58da87dd662c135b70c065a0b1ca800cd4b075b365f3d71e0ff02d71c7457883
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4-1.debian.tar.xz' libsemanage_3.4-1.debian.tar.xz 23248 SHA256:531c5294d5ec881ef4bc4396a9e1f38895558cd88c4fd6d3f6a673a4b2297a5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/3.4-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=3.4-2`

Binary Packages:

- `libsepol2:amd64=3.4-2`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.4-2
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4-2.dsc' libsepol_3.4-2.dsc 2005 SHA256:c43db54870c37a4b6441b1980bfd41932e7851244ba1fda0df86c5f17dd67e8a
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz' libsepol_3.4.orig.tar.gz 490628 SHA256:fc277ac5b52d59d2cd81eec8b1cccd450301d8b54d9dd48a993aea0577cf0336
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz.asc' libsepol_3.4.orig.tar.gz.asc 833 SHA256:ed127c08353dbc2c442d47d77e323e79e5bd47791a0a5bd4dfd077868f4346bc
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4-2.debian.tar.xz' libsepol_3.4-2.debian.tar.xz 21516 SHA256:fdf943b513b8d0fc6b74fd6a007ba35c9601909c0b3fd6e7726b4b09b1243502
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/3.4-2/ (for browsing the source)
- https://sources.debian.net/src/libsepol/3.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/3.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libssh2=1.10.0-3`

Binary Packages:

- `libssh2-1:amd64=1.10.0-3+b1`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.10.0-3
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0-3.dsc' libssh2_1.10.0-3.dsc 2283 SHA256:a0fe68f402a2f44dd6bd2219457fb8677b2149a83e7b009e93ff0635de940766
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz' libssh2_1.10.0.orig.tar.gz 965044 SHA256:2d64e90f3ded394b91d3a2e774ca203a4179f69aebee03003e5a6fa621e41d51
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz.asc' libssh2_1.10.0.orig.tar.gz.asc 488 SHA256:75702eaf490fa8c1e69b889c5c6366c2c3f3b089bc715f9f9be081c88f115f81
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0-3.debian.tar.xz' libssh2_1.10.0-3.debian.tar.xz 8416 SHA256:c0bea31fe565273656349484d1000b557e489ee322834b40c4d7d33317a56940
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.10.0-3/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.10.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.10.0-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libtirpc=1.3.3+ds-1`

Binary Packages:

- `libtirpc-common=1.3.3+ds-1`
- `libtirpc3:amd64=1.3.3+ds-1`

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
$ apt-get source -qq --print-uris libtirpc=1.3.3+ds-1
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.dsc' libtirpc_1.3.3+ds-1.dsc 2129 SHA256:c05c5d76027d4162d5a29d73eef90076559bde0fa5133b2e0045d82155e1b2af
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds.orig.tar.gz' libtirpc_1.3.3+ds.orig.tar.gz 699030 SHA256:facd98473c3a16fe6564c6458ef96ebb84d144345d1171f034fa019424bba027
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.debian.tar.xz' libtirpc_1.3.3+ds-1.debian.tar.xz 11232 SHA256:fd1865c49e905951a641082981c1dab7f018caea1a5e23af1791728a3320800e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtirpc/1.3.3+ds-1/ (for browsing the source)
- https://sources.debian.net/src/libtirpc/1.3.3+ds-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtirpc/1.3.3+ds-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=1.0-1`

Binary Packages:

- `libunistring2:amd64=1.0-1`

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
$ apt-get source -qq --print-uris libunistring=1.0-1
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.0-1.dsc' libunistring_1.0-1.dsc 1928 SHA256:d93859cde749a30f55404ea1ef0ed4f02e58d2475a7c7e088b264d4df0626061
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz' libunistring_1.0.orig.tar.xz 2367800 SHA256:5bab55b49f75d77ed26b257997e919b693f29fd4a1bc22e0e6e024c246c72741
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.0-1.debian.tar.xz' libunistring_1.0-1.debian.tar.xz 42004 SHA256:7cf35dfd1de973ee3944930d215750c7de27ececd91616ad129ac5a238b1538f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/1.0-1/ (for browsing the source)
- https://sources.debian.net/src/libunistring/1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/1.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcrypt=1:4.4.28-2`

Binary Packages:

- `libcrypt1:amd64=1:4.4.28-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.28-2
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.28-2.dsc' libxcrypt_4.4.28-2.dsc 1613 SHA256:b668e66960c61b6980fbb6f2ea2cd7602e390f363e843798eca85f6cc6200a87
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.28.orig.tar.xz' libxcrypt_4.4.28.orig.tar.xz 391484 SHA256:2bf09c6c3ea139d11134d2598745a0793f4cf17245720880394c00490dbcb4df
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.28-2.debian.tar.xz' libxcrypt_4.4.28-2.debian.tar.xz 8088 SHA256:d5f8c1c1e2cb9ef9e99da9f3c7f28fc4142781337a72c22a67d841a8a8fee4d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.28-2/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.28-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.28-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.5.2+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.5.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.2+dfsg-1
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg-1.dsc' libzstd_1.5.2+dfsg-1.dsc 2173 SHA256:135c6d3ef18470e2eb4289b2aca6256eb9abba28478b08d99b0e1b8257af0b69
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg.orig.tar.xz' libzstd_1.5.2+dfsg.orig.tar.xz 1404564 SHA256:b59caaee4a6176bbe67bf5440b56ca8814da9d2ad2d943eb7b3ee8a0a83e4224
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg-1.debian.tar.xz' libzstd_1.5.2+dfsg-1.debian.tar.xz 11820 SHA256:286c2cc82fd3b0d76d172102efa8004325875bb0db1d12b5a52bbfc050f61a28
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.5.2+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.5.2+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.5.2+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lsb=11.2`

Binary Packages:

- `lsb-base=11.2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.2
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_11.2.dsc' lsb_11.2.dsc 1760 SHA256:8c48cbef560af3ed07075b32fdbb8e2e84ab923d6f8e6607c550d867590872f4
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_11.2.tar.xz' lsb_11.2.tar.xz 42812 SHA256:7f1c6ebbc56fde6aeb011f3a8c7d30b8715f2adbaaaa0b67c7a71cc56d8f2155
```

Other potentially useful URLs:

- https://sources.debian.net/src/lsb/11.2/ (for browsing the source)
- https://sources.debian.net/src/lsb/11.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lsb/11.2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mawk=1.3.4.20200120-3.1`

Binary Packages:

- `mawk=1.3.4.20200120-3.1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-3.1
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.dsc' mawk_1.3.4.20200120-3.1.dsc 1776 SHA256:ed0543e3111f718e918a73033292fe2616760c8791c13efa0da3818ca835cdc1
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.debian.tar.xz' mawk_1.3.4.20200120-3.1.debian.tar.xz 14080 SHA256:7850d7c44aa826635c79a6666b0d457a03524bcb0307697b062dd717d6d9d491
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.4.20200120-3.1/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.4.20200120-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.4.20200120-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `media-types=8.0.0`

Binary Packages:

- `media-types=8.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=8.0.0
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_8.0.0.dsc' media-types_8.0.0.dsc 1620 SHA256:e80b1ac65060ce4a6d12184ca9ee564f38073b736e4ddd473be081931b50ffed
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_8.0.0.tar.xz' media-types_8.0.0.tar.xz 56364 SHA256:85f9b3ccbb6bc8dc0fff47105726ca1877ac2011cc7e8244ab276d5583f4890e
```

Other potentially useful URLs:

- https://sources.debian.net/src/media-types/8.0.0/ (for browsing the source)
- https://sources.debian.net/src/media-types/8.0.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/media-types/8.0.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mercurial=6.1.3-1`

Binary Packages:

- `mercurial=6.1.3-1`
- `mercurial-common=6.1.3-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/mercurial/6.1.3-1/


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

### `dpkg` source package: `ncurses=6.3+20220423-2`

Binary Packages:

- `libncurses6:amd64=6.3+20220423-2`
- `libncursesw6:amd64=6.3+20220423-2`
- `libtinfo6:amd64=6.3+20220423-2`
- `ncurses-base=6.3+20220423-2`
- `ncurses-bin=6.3+20220423-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.3+20220423-2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423-2.dsc' ncurses_6.3+20220423-2.dsc 4200 SHA256:bdd7ba478c9328689bd47231328efbf87ab970c4c26f5489b40abb4f4fdd79fa
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423.orig.tar.gz' ncurses_6.3+20220423.orig.tar.gz 3611993 SHA256:a6bdfe499ae98ee937fed4729de09ffea08201317a9d16ed5d0142ac8b8b30e1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423.orig.tar.gz.asc' ncurses_6.3+20220423.orig.tar.gz.asc 729 SHA256:6771460069f300048dd7c7a41027cd38250b4f28d5f1dcef9cf8edb9b5ca691c
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423-2.debian.tar.xz' ncurses_6.3+20220423-2.debian.tar.xz 54600 SHA256:0a211bbd63949d81d6363a0fe2bf95f8592162f1dd34ded7252ec1d3340036c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.3+20220423-2/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.3+20220423-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.3+20220423-2/ (for access to the source package after it no longer exists in the archive)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/nettle/3.7.3-1/


### `dpkg` source package: `nghttp2=1.48.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.48.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `SIL-OFL-1.1`
- `all-permissive`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/nghttp2/1.48.0-1/


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

### `dpkg` source package: `openldap=2.5.12+dfsg-2`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.12+dfsg-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.12+dfsg-2
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.12%2bdfsg-2.dsc' openldap_2.5.12+dfsg-2.dsc 3179 SHA256:140e78550e434b2366af9973567952439c9e88fbbf91c9abc8673b89c0a94318
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.12%2bdfsg.orig.tar.gz' openldap_2.5.12+dfsg.orig.tar.gz 5612581 SHA256:e22c3a35319ed1b7f7148b508bf2298f7180f3a82fbba34c272f437b979f49aa
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.12%2bdfsg-2.debian.tar.xz' openldap_2.5.12+dfsg-2.debian.tar.xz 157900 SHA256:f4a0ffc8e00fcea2d7a3629e714ff1d1c440614510e590230bf4c9f2f7adc574
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.5.12+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.5.12+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.5.12+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:9.0p1-1`

Binary Packages:

- `openssh-client=1:9.0p1-1+b1`

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
$ apt-get source -qq --print-uris openssh=1:9.0p1-1
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.0p1-1.dsc' openssh_9.0p1-1.dsc 3347 SHA256:ff368f3247c89eea2be10cd2ad2fcb9d0811fc6652c9cab9d01d087203e28fdd
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.0p1.orig.tar.gz' openssh_9.0p1.orig.tar.gz 1822183 SHA256:03974302161e9ecce32153cfa10012f1e65c8f3750f573a73ab1befd5972a28a
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.0p1.orig.tar.gz.asc' openssh_9.0p1.orig.tar.gz.asc 833 SHA256:5db3a2eb3e8e9c8ae62527ea55f5a6fa41c395ebd0bbb65f4b3dfebeeee5fa00
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.0p1-1.debian.tar.xz' openssh_9.0p1-1.debian.tar.xz 176128 SHA256:46f24ab534892c55c82ebafdac23564579f9be73a7cc0230730a2e6aa64e17ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:9.0p1-1/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:9.0p1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:9.0p1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=3.0.5-2`

Binary Packages:

- `libssl3:amd64=3.0.5-2`
- `openssl=3.0.5-2`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.5-2
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.5-2.dsc' openssl_3.0.5-2.dsc 2604 SHA256:14240475ff239f45bc71a340c38a56a5a79e8b77d3e8a4848dbe3bdad77bf9ff
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.5.orig.tar.gz' openssl_3.0.5.orig.tar.gz 15074407 SHA256:aa7d8d9bef71ad6525c55ba11e5f4397889ce49c2c9349dcea6d3e4f0b024a7a
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.5.orig.tar.gz.asc' openssl_3.0.5.orig.tar.gz.asc 862 SHA256:95f23bb4eb6faa8d0f1ca1b83cfb00a2bed4b53e124a4f13e1499abc0b426129
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.5-2.debian.tar.xz' openssl_3.0.5-2.debian.tar.xz 122744 SHA256:89efb42889b989a32ed3ec54ee59e56e42dd1411f283aa91f38b961c93f1c664
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/3.0.5-2/ (for browsing the source)
- https://sources.debian.net/src/openssl/3.0.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/3.0.5-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.24.1-1`

Binary Packages:

- `libp11-kit0:amd64=0.24.1-1`

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
$ apt-get source -qq --print-uris p11-kit=0.24.1-1
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1-1.dsc' p11-kit_0.24.1-1.dsc 2501 SHA256:6d4336ed2799503c65dfb0518d623e3af46bac03e0e1a0ea9ce432044261d55b
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz' p11-kit_0.24.1.orig.tar.xz 838304 SHA256:d8be783efd5cd4ae534cee4132338e3f40f182c3205d23b200094ec85faaaef8
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz.asc' p11-kit_0.24.1.orig.tar.xz.asc 833 SHA256:48041a234bac05f70519b0d4727e78a129ea80a51baf92c7d419f80b7cbdf0ab
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1-1.debian.tar.xz' p11-kit_0.24.1-1.debian.tar.xz 23200 SHA256:769674df62c3caeada0e5885a992302cbde63a81a09972bf6b78f8797ebc40bd
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.24.1-1/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.24.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.24.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.4.0-13`

Binary Packages:

- `libpam-modules:amd64=1.4.0-13`
- `libpam-modules-bin=1.4.0-13`
- `libpam-runtime=1.4.0-13`
- `libpam0g:amd64=1.4.0-13`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pam/1.4.0-13/


### `dpkg` source package: `pcre2=10.40-1`

Binary Packages:

- `libpcre2-8-0:amd64=10.40-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.40-1
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40-1.dsc' pcre2_10.40-1.dsc 2286 SHA256:0c880d9bc04175400921d8d6af2c24f1268a9c8678154b607d0df910d97bcbef
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40.orig.tar.gz' pcre2_10.40.orig.tar.gz 2359622 SHA256:ded42661cab30ada2e72ebff9e725e745b4b16ce831993635136f2ef86177724
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40-1.diff.gz' pcre2_10.40-1.diff.gz 7134 SHA256:6fe586fd149e20d18d42a60d2845b29ff5862511b851bfb80dd64d72359dc1c4
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.40-1/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.40-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.40-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.39-14`

Binary Packages:

- `libpcre3:amd64=2:8.39-14`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-14
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-14.dsc' pcre3_8.39-14.dsc 2226 SHA256:d94bb6081f26cdd05738aab33cee1cfbd6129a0ccd340b777c2814f4b6b7dc3d
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-14.debian.tar.gz' pcre3_8.39-14.debian.tar.gz 27185 SHA256:51369d53bb668d9a41de0adf094450f7bed57541a2d4e2cabc8dccec5026a1cf
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre3/2:8.39-14/ (for browsing the source)
- https://sources.debian.net/src/pcre3/2:8.39-14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre3/2:8.39-14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.34.0-5`

Binary Packages:

- `libperl5.34:amd64=5.34.0-5`
- `perl=5.34.0-5`
- `perl-base=5.34.0-5`
- `perl-modules-5.34=5.34.0-5`

Licenses: (parsed from: `/usr/share/doc/libperl5.34/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.34/copyright`)

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
$ apt-get source -qq --print-uris perl=5.34.0-5
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0-5.dsc' perl_5.34.0-5.dsc 2886 SHA256:fa744b5d2786d0dda1bfdb2960e0c2b66a734c4e268ec5de8e378366f680f021
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0.orig-regen-configure.tar.xz' perl_5.34.0.orig-regen-configure.tar.xz 415412 SHA256:b168f566401fdccc13d0616c258854c1e1a461276922babca617097cd9dfd85b
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0.orig.tar.xz' perl_5.34.0.orig.tar.xz 12881416 SHA256:82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0-5.debian.tar.xz' perl_5.34.0-5.debian.tar.xz 167484 SHA256:dbbb6c9c5218faef00bf5ee38b1c4e76bb02733742368984517b6e2449708f93
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.34.0-5/ (for browsing the source)
- https://sources.debian.net/src/perl/5.34.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.34.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.2.0-2`

Binary Packages:

- `pinentry-curses=1.2.0-2`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.2.0-2
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0-2.dsc' pinentry_1.2.0-2.dsc 2242 SHA256:43d974d725f0e261449ea1aa340b00e9e53c0e567f12db7da41942ecc07bd755
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0.orig.tar.bz2' pinentry_1.2.0.orig.tar.bz2 498390 SHA256:10072045a3e043d0581f91cd5676fcac7ffee957a16636adedaa4f583a616470
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0.orig.tar.bz2.asc' pinentry_1.2.0.orig.tar.bz2.asc 228 SHA256:d917a96c24e796daba7bab36bacc75d8106ef24d2afc485d13448d3cf8bd8a86
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0-2.debian.tar.xz' pinentry_1.2.0-2.debian.tar.xz 19160 SHA256:628541197becd30a5da77a79b878d9e9df4954334792db7b4f740bc3109bdc4d
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.2.0-2/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.2.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.2.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.17-7`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-7+b1`
- `procps=2:3.3.17-7+b1`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-7
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-7.dsc' procps_3.3.17-7.dsc 2136 SHA256:732d511886d3141ca96d189706232eada1b73dc44e3671ca7ef2ffd6838d01f7
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA256:4518b3e7aafd34ec07d0063d250fd474999b20b200218c3ae56f5d2113f141b4
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-7.debian.tar.xz' procps_3.3.17-7.debian.tar.xz 29196 SHA256:43148a05c2694b946dd485aea135a3c0645019e785b80064d0ebffa88426f6a9
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.17-7/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.17-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.17-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.10.5-3`

Binary Packages:

- `libpython3-stdlib:amd64=3.10.5-3`
- `python3=3.10.5-3`
- `python3-minimal=3.10.5-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-defaults/3.10.5-3/


### `dpkg` source package: `python3.10=3.10.6-1`

Binary Packages:

- `libpython3.10-minimal:amd64=3.10.6-1`
- `libpython3.10-stdlib:amd64=3.10.6-1`
- `python3.10=3.10.6-1`
- `python3.10-minimal=3.10.6-1`

Licenses: (parsed from: `/usr/share/doc/libpython3.10-minimal/copyright`, `/usr/share/doc/libpython3.10-stdlib/copyright`, `/usr/share/doc/python3.10/copyright`, `/usr/share/doc/python3.10-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.10=3.10.6-1
'http://deb.debian.org/debian/pool/main/p/python3.10/python3.10_3.10.6-1.dsc' python3.10_3.10.6-1.dsc 3639 SHA256:39d0abe62c698c58ff34662a947d0605de860f10ceac878267e5056fd6e106cd
'http://deb.debian.org/debian/pool/main/p/python3.10/python3.10_3.10.6.orig.tar.xz' python3.10_3.10.6.orig.tar.xz 19600672 SHA256:f795ff87d11d4b0c7c33bc8851b0c28648d8a4583aa2100a98c22b4326b6d3f3
'http://deb.debian.org/debian/pool/main/p/python3.10/python3.10_3.10.6-1.debian.tar.xz' python3.10_3.10.6-1.debian.tar.xz 219472 SHA256:eb89828e0273113e38e4557864b2befaecb53f61b0504cea2a965d8a9be5e3a2
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.10/3.10.6-1/ (for browsing the source)
- https://sources.debian.net/src/python3.10/3.10.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.10/3.10.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.1.2-1.2`

Binary Packages:

- `libreadline8:amd64=8.1.2-1.2`
- `readline-common=8.1.2-1.2`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/readline/8.1.2-1.2/


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

### `dpkg` source package: `serf=1.3.9-11`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-11`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-11/


### `dpkg` source package: `sgml-base=1.30`

Binary Packages:

- `sgml-base=1.30`

Licenses: (parsed from: `/usr/share/doc/sgml-base/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sgml-base=1.30
'http://deb.debian.org/debian/pool/main/s/sgml-base/sgml-base_1.30.dsc' sgml-base_1.30.dsc 1541 SHA256:4bb8cb33a49a14ad50642f93930f26f8aef039350a847640487cb9a596b1e103
'http://deb.debian.org/debian/pool/main/s/sgml-base/sgml-base_1.30.tar.xz' sgml-base_1.30.tar.xz 12536 SHA256:a125fadaeac4c15580ff278e24b807e8cbae4c5d220aed9568518cc1f115d082
```

Other potentially useful URLs:

- https://sources.debian.net/src/sgml-base/1.30/ (for browsing the source)
- https://sources.debian.net/src/sgml-base/1.30/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sgml-base/1.30/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shadow=1:4.11.1+dfsg1-2`

Binary Packages:

- `login=1:4.11.1+dfsg1-2`
- `passwd=1:4.11.1+dfsg1-2`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.11.1+dfsg1-2
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.11.1%2bdfsg1-2.dsc' shadow_4.11.1+dfsg1-2.dsc 2416 SHA256:55091e85ca7ff9f9a9d6673a18aee56bc9006ce254b8a9e16abc7b745de1cfda
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.11.1%2bdfsg1.orig.tar.xz' shadow_4.11.1+dfsg1.orig.tar.xz 1704716 SHA256:2605c11ff70d9d934147c74bc2d91771497460efbba29198d069e64ff9cd88ab
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.11.1%2bdfsg1-2.debian.tar.xz' shadow_4.11.1+dfsg1-2.debian.tar.xz 77852 SHA256:e0a1521bf22af1d88d6644fdd438f9afbe4a01b1ee0c468477d4938d80a28ecf
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.11.1+dfsg1-2/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.11.1+dfsg1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.11.1+dfsg1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.39.2-1`

Binary Packages:

- `libsqlite3-0:amd64=3.39.2-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.39.2-1
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.39.2-1.dsc' sqlite3_3.39.2-1.dsc 2487 SHA256:e646c885f97db9e045d6c1e8fc18b4c373279119d3a7969f94937017a242b7c5
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.39.2.orig-www.tar.xz' sqlite3_3.39.2.orig-www.tar.xz 5853576 SHA256:10d0d2d010c5aee87d8987cd534b89bd1aca23ef268b210baf7de610562aba25
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.39.2.orig.tar.xz' sqlite3_3.39.2.orig.tar.xz 7770608 SHA256:d84a79699b044c903ea4bc5417a6ff1753519d5fc5188b2737fb92f14d2a8061
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.39.2-1.debian.tar.xz' sqlite3_3.39.2-1.debian.tar.xz 29532 SHA256:b034b7241ba499df497ea9b04a2f8be2069113f20f720ae43d17c05a5980d2d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.39.2-1/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.39.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.39.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `subversion=1.14.2-3`

Binary Packages:

- `libsvn1:amd64=1.14.2-3+b1`
- `subversion=1.14.2-3+b1`

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
$ apt-get source -qq --print-uris subversion=1.14.2-3
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2-3.dsc' subversion_1.14.2-3.dsc 4046 SHA256:09b88f161ce31aa691728d2decf9a78a16078da0812eeb68f93d9af0dd74431d
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2.orig.tar.gz' subversion_1.14.2.orig.tar.gz 11626792 SHA256:fd826afad03db7a580722839927dc664f3e93398fe88b66905732c8530971353
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2.orig.tar.gz.asc' subversion_1.14.2.orig.tar.gz.asc 3215 SHA256:da6a0a5ff56f671ad2d1eae708f8d1cc1abf0485b029a163ff8272cba5475861
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2-3.debian.tar.xz' subversion_1.14.2-3.debian.tar.xz 336384 SHA256:bab721201e0673a74b64263ae9dd460b1193d71f905c2cc76c7a21f0d6e7acc0
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.14.2-3/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.14.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.14.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=251.3-1`

Binary Packages:

- `libsystemd0:amd64=251.3-1`
- `libudev1:amd64=251.3-1`

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

- http://snapshot.debian.org/package/systemd/251.3-1/


### `dpkg` source package: `sysvinit=3.04-1`

Binary Packages:

- `sysvinit-utils=3.04-1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.04-1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.04-1.dsc' sysvinit_3.04-1.dsc 2367 SHA256:b31fb6eb9b0d919336f2a930bbf1bb6043630a3a7fbfd734575d1a3c9201dac1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.04.orig.tar.gz' sysvinit_3.04.orig.tar.gz 465162 SHA256:6ec16f2598d6f9dfb4707e9e9dd2e59f553d1cf0f04161f496ed63bcaa4f61f1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.04-1.debian.tar.xz' sysvinit_3.04-1.debian.tar.xz 128008 SHA256:6e3be2686502eb2b674bfd7fafe3b4633e18a59038ca6e3946b170672b9d33e0
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/3.04-1/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/3.04-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/3.04-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `tzdata=2022c-1`

Binary Packages:

- `tzdata=2022c-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2022c-1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022c-1.dsc' tzdata_2022c-1.dsc 2205 SHA256:77cd066ea4b32eebb1f0bcd940760ee798d296d9f41e47d63a57e01f3fe14861
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022c.orig.tar.gz' tzdata_2022c.orig.tar.gz 432721 SHA256:6974f4e348bf2323274b56dff9e7500247e3159eaa4b485dfa0cd66e75c14bfe
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022c.orig.tar.gz.asc' tzdata_2022c.orig.tar.gz.asc 833 SHA256:f68abba02768861fd6c77800fffacfb298270a60eebf9f4c3078aa9be53adec9
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022c-1.debian.tar.xz' tzdata_2022c-1.debian.tar.xz 111928 SHA256:a9404aed669281a24dfe637846efe067e7600456c5935286998beb7260a7d7c2
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2022c-1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2022c-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2022c-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `utf8proc=2.7.0-3`

Binary Packages:

- `libutf8proc2:amd64=2.7.0-3`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.7.0-3
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.7.0-3.dsc' utf8proc_2.7.0-3.dsc 2162 SHA256:95642d5aebbae9e1f3cb4bfcc3888291214644c508950944625d3544528fc4c7
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.7.0.orig.tar.gz' utf8proc_2.7.0.orig.tar.gz 187906 SHA256:4bb121e297293c0fd55f08f83afab6d35d48f0af4ecc07523ad8ec99aa2b12a1
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.7.0-3.debian.tar.xz' utf8proc_2.7.0-3.debian.tar.xz 5608 SHA256:66ed859302f2b28b68e70ed2fce30af4ee45d71a045216e77c6ad81614b326f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/utf8proc/2.7.0-3/ (for browsing the source)
- https://sources.debian.net/src/utf8proc/2.7.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/utf8proc/2.7.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.38.1-1`

Binary Packages:

- `bsdutils=1:2.38.1-1`
- `libblkid1:amd64=2.38.1-1`
- `libmount1:amd64=2.38.1-1`
- `libsmartcols1:amd64=2.38.1-1`
- `libuuid1:amd64=2.38.1-1`
- `mount=2.38.1-1`
- `util-linux=2.38.1-1`
- `util-linux-extra=2.38.1-1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/util-linux-extra/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.38.1-1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1-1.dsc' util-linux_2.38.1-1.dsc 4520 SHA256:45d9335fa92e30b7b12a79c45e4d6303c1e5fe6ac83721f3fb88e5e6aabae557
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1.orig.tar.xz' util-linux_2.38.1.orig.tar.xz 7495904 SHA256:60492a19b44e6cf9a3ddff68325b333b8b52b6c59ce3ebd6a0ecaa4c5117e84f
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1-1.debian.tar.xz' util-linux_2.38.1-1.debian.tar.xz 95928 SHA256:c7a87ca093e565fbaed813b7e8b220f5e875437dd418ded2aefef6322f8aa0b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.38.1-1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.38.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.38.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.21.3-1`

Binary Packages:

- `wget=1.21.3-1+b2`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21.3-1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3-1.dsc' wget_1.21.3-1.dsc 2167 SHA256:e294772dac85a4d59fa64269515aa4a93664789f1f4612cfe309785384fd1f55
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3.orig.tar.gz' wget_1.21.3.orig.tar.gz 5079864 SHA256:5726bb8bc5ca0f6dc7110f6416e4bb7019e2d2ff5bf93d1ca2ffcc6656f220e5
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3.orig.tar.gz.asc' wget_1.21.3.orig.tar.gz.asc 854 SHA256:a4d96f04bc5a034310eae177df9adc79ef7a6f0fad7bf7669bf0ac318fa22ccd
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3-1.debian.tar.xz' wget_1.21.3-1.debian.tar.xz 60660 SHA256:30901c12ded6e455d55fe73c40245b51d2fd53e20e30713a10e066fdfadb9d20
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.21.3-1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.21.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.21.3-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xz-utils=5.2.5-2.1`

Binary Packages:

- `liblzma5:amd64=5.2.5-2.1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2.1
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.dsc' xz-utils_5.2.5-2.1.dsc 2402 SHA256:338b5ec72d0d48a5fbb004926ebac8850eecd9626e38f6b50960ed975513b081
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA256:3e1e518ffc912f86608a8cb35e4bd41ad1aec210df2a47aaa1f95e7f5576ef56
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.debian.tar.xz' xz-utils_5.2.5-2.1.debian.tar.xz 34916 SHA256:24a1950b365b0922c3ef7f1475930bbcc64cdef04929f081b8ad5e2628ef2413
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.5-2.1/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.5-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.5-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.11.dfsg-4`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-4`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-4
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-4.dsc' zlib_1.2.11.dfsg-4.dsc 2397 SHA256:3ce1b7907cf1b35ffa95b06104d951314c48aa3463b78eddc0025ae59e9537cd
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-4.debian.tar.xz' zlib_1.2.11.dfsg-4.debian.tar.xz 23316 SHA256:b2e66b33c5aeeafa1cd00b2e06e671faf1345fc1ac13e5e2dcb12360df2fd677
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-4/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.11.dfsg-4/ (for access to the source package after it no longer exists in the archive)
