# `buildpack-deps:sid-scm`

## Docker Metadata

- Image ID: `sha256:e50568bd6d28ffaf3141079eff64147ee46760740d1b099fdce09a05ec419723`
- Created: `2022-03-01T06:30:19.085330916Z`
- Virtual Size: ~ 315.06 Mb  
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/adduser/3.118/


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

### `dpkg` source package: `apt=2.4.0`

Binary Packages:

- `apt=2.4.0`
- `libapt-pkg6.0:amd64=2.4.0`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.4.0/


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
- `libaudit1:amd64=1:3.0.7-1`

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

### `dpkg` source package: `curl=7.81.0-1`

Binary Packages:

- `curl=7.81.0-1`
- `libcurl3-gnutls:amd64=7.81.0-1`
- `libcurl4:amd64=7.81.0-1`

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

- http://snapshot.debian.org/package/curl/7.81.0-1/


### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg-2`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg-2`
- `libsasl2-modules-db:amd64=2.1.28+dfsg-2`

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
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg-2
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-2.dsc' cyrus-sasl2_2.1.28+dfsg-2.dsc 3253 SHA256:8eba3ffafa70f1ac1eac4b6f244b4e936b2fcb2c1c4bdcb71c42e19d7a3856c8
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg.orig.tar.xz 797472 SHA256:a15886d7da5958bd27f35b7c871dd872f6dc5b9917c9b6b15e3de014c7dab3d9
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-2.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg-2.debian.tar.xz 86396 SHA256:ae83dfd0038a0013477eb58d1b33a77f9cf9f69ba4830172a9f66e3e6e769a34
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.28+dfsg-2/ (for access to the source package after it no longer exists in the archive)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/dash/0.5.11+git20210903+057cd650a4ed-3/


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

### `dpkg` source package: `debianutils=5.7-0.1`

Binary Packages:

- `debianutils=5.7-0.1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.7-0.1
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.1.dsc' debianutils_5.7-0.1.dsc 1542 SHA256:437dd4a5bae8a592ca1b844f98975605497009cd45fdca9325178c382d49bca1
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7.orig.tar.gz' debianutils_5.7.orig.tar.gz 257231 SHA256:27ec9e0e7e44dc8ab611aa576330471bacb07e4491ffecf0d3aa6909c92f9022
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.1.debian.tar.xz' debianutils_5.7-0.1.debian.tar.xz 21564 SHA256:43e959668d0731072613ff910e4c9354164ee7c8df7d805505ca0e2604bea8c4
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/5.7-0.1/ (for browsing the source)
- https://sources.debian.net/src/debianutils/5.7-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/5.7-0.1/ (for access to the source package after it no longer exists in the archive)

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

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/dpkg/1.21.1/


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

### `dpkg` source package: `expat=2.4.6-1`

Binary Packages:

- `libexpat1:amd64=2.4.6-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/expat/2.4.6-1/


### `dpkg` source package: `findutils=4.9.0-2`

Binary Packages:

- `findutils=4.9.0-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.9.0-2
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-2.dsc' findutils_4.9.0-2.dsc 2304 SHA256:85d8c92104d56af1dacf3be544c3aea5d1b71186d170cdd92bdeac9be5f4981a
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA256:a2bfb8c09d436770edc59f50fa483e785b161a3b7b9d547573cb08065fd462fe
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA256:924c3719d066eda1b3e47175f8b83e90e9a23f0a639ebe7445621917b283c385
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-2.debian.tar.xz' findutils_4.9.0-2.debian.tar.xz 27584 SHA256:173aa2ac4ee290804f48bb9ea51d23dae38e8d5bd94f24f6af39bd68c170a6e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.9.0-2/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.9.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.9.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gcc-12=12-20220222-1`

Binary Packages:

- `gcc-12-base:amd64=12-20220222-1`
- `libgcc-s1:amd64=12-20220222-1`
- `libstdc++6:amd64=12-20220222-1`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12-20220222-1
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12-20220222-1.dsc' gcc-12_12-20220222-1.dsc 27388 SHA256:96927db4634a80762cb7c92771cb930f0bcdf226a07f639a8a866043b64feecb
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12-20220222.orig.tar.gz' gcc-12_12-20220222.orig.tar.gz 84511385 SHA256:aa55b7635312827f4c42e2dc55bb6f2f002bb98f05e3c55966df42bb317c2815
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12-20220222-1.debian.tar.xz' gcc-12_12-20220222-1.debian.tar.xz 559416 SHA256:a9d63045deef4e5f3824d2b03c827c99209097efbeaa6d407b39630f6be751d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-12/12-20220222-1/ (for browsing the source)
- https://sources.debian.net/src/gcc-12/12-20220222-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-12/12-20220222-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-9=9.4.0-5`

Binary Packages:

- `gcc-9-base:amd64=9.4.0-5`

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
$ apt-get source -qq --print-uris gcc-9=9.4.0-5
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.4.0-5.dsc' gcc-9_9.4.0-5.dsc 21922 SHA256:47e4af49e8604a3f62ad0f52ea1f56a02e7b5429ce539ca9634de222cf4e7313
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.4.0.orig.tar.gz' gcc-9_9.4.0.orig.tar.gz 88736226 SHA256:7ef28e618cecddbb538359d03998a61648edb10b570b995aa4f4016c4a0d823e
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.4.0-5.debian.tar.xz' gcc-9_9.4.0-5.debian.tar.xz 646384 SHA256:4c220443cdc21b8cda8c6402e422049ba08be9aaff38a35f6a4cb0d5b97ca19d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-9/9.4.0-5/ (for browsing the source)
- https://sources.debian.net/src/gcc-9/9.4.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-9/9.4.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.23-1`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-1`
- `libgdbm6:amd64=1.23-1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.23-1
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23-1.dsc' gdbm_1.23-1.dsc 2583 SHA256:fae26cb50da1af1d7b152495dbb2bca0301e65973d0a6a6d6d771e7e58a82d72
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz' gdbm_1.23.orig.tar.gz 1115854 SHA256:74b1081d21fff13ae4bd7c16e5d6e504a4c26f7cde1dca0d963a484174bbcacd
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz.asc' gdbm_1.23.orig.tar.gz.asc 181 SHA256:64ebb68cc68e8915d62cb20ea40323c00b56051f844589ee0a52169fff34cecb
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23-1.debian.tar.xz' gdbm_1.23-1.debian.tar.xz 18484 SHA256:cc86b10814c2045967d29571ea7bed810fc4ec917d2918d056b8eb3e5622eb1c
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.23-1/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.23-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.23-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `glibc=2.33-7`

Binary Packages:

- `libc-bin=2.33-7`
- `libc6:amd64=2.33-7`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.33-7
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.33-7.dsc' glibc_2.33-7.dsc 9631 SHA256:2c63cf9c2abada5fa7dd0e24c59eaddc1356da1d2d67a8484a61021c548e2e55
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.33.orig.tar.xz' glibc_2.33.orig.tar.xz 17643172 SHA256:5bd6d6b7fb0350308aa7abd067e081d57ba6ac1e0372ed372d197bccb86e5c14
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.33-7.debian.tar.xz' glibc_2.33-7.debian.tar.xz 857788 SHA256:c4dd741a08918861796cf62a8d3209a56d41d807344a7db481b73a4d17f726bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.33-7/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.33-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.33-7/ (for access to the source package after it no longer exists in the archive)

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

- `dirmngr=2.2.27-3`
- `gnupg=2.2.27-3`
- `gnupg-l10n=2.2.27-3`
- `gnupg-utils=2.2.27-3`
- `gpg=2.2.27-3`
- `gpg-agent=2.2.27-3`
- `gpg-wks-client=2.2.27-3`
- `gpg-wks-server=2.2.27-3`
- `gpgconf=2.2.27-3`
- `gpgsm=2.2.27-3`
- `gpgv=2.2.27-3`

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
$ apt-get source -qq --print-uris gnupg2=2.2.27-3
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-3.dsc' gnupg2_2.2.27-3.dsc 3630 SHA256:c3fcf3c8f0aad05bb86f7bdcd67bdc9dd67cb35b0605778de3ee5b07ba621934
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2' gnupg2_2.2.27.orig.tar.bz2 7191555 SHA256:34e60009014ea16402069136e0a5f63d9b65f90096244975db5cea74b3d02399
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-3.debian.tar.xz' gnupg2_2.2.27-3.debian.tar.xz 63396 SHA256:ef72e1094b7c47c9394d1d46bfda1ca46fbea53165f3e40fe169372f8fa3f62b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.27-3/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.27-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.27-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.3-4`

Binary Packages:

- `libgnutls30:amd64=3.7.3-4+b1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.3-4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.3-4.dsc' gnutls28_3.7.3-4.dsc 3457 SHA256:f855b4f36a392459465c610235b6f9de569232a83eef7be4629daca192f0ad8c
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.3.orig.tar.xz' gnutls28_3.7.3.orig.tar.xz 6119292 SHA256:fc59c43bc31ab20a6977ff083029277a31935b8355ce387b634fa433f8f6c49a
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.3.orig.tar.xz.asc' gnutls28_3.7.3.orig.tar.xz.asc 833 SHA256:a2f95ac5d7dd951bddef01ec9930616dd1a5226173b3dc7896b3bed411c91d9a
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.3-4.debian.tar.xz' gnutls28_3.7.3-4.debian.tar.xz 66780 SHA256:0c2dbafae29ba7bb82568a6fabf6be270633af74366e7f580f86f1c13f176084
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.3-4/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.3-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `init-system-helpers=1.62`

Binary Packages:

- `init-system-helpers=1.62`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.62
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.62.dsc' init-system-helpers_1.62.dsc 1993 SHA256:98b0149e9d8f9b75b604ac2cedeef32f40e7f18f64f02b1ec819d4dd49b249a1
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.62.tar.xz' init-system-helpers_1.62.tar.xz 42144 SHA256:195db496bc40fe5a37bcdab26c275643cd119edfceb0551cacf6206ba36447e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.62/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.62/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.62/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.6.1-2`

Binary Packages:

- `libkeyutils1:amd64=1.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/keyutils/1.6.1-2/


### `dpkg` source package: `krb5=1.19.2-2`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.19.2-2`
- `libk5crypto3:amd64=1.19.2-2`
- `libkrb5-3:amd64=1.19.2-2`
- `libkrb5support0:amd64=1.19.2-2`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.19.2-2
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.19.2-2.dsc' krb5_1.19.2-2.dsc 3170 SHA256:1332e77708c493968ba744f48438c5a83c2b4c08c4d90e03c01d84b6bb0a506f
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz' krb5_1.19.2.orig.tar.gz 8741053 SHA256:10453fee4e3a8f8ce6129059e5c050b8a65dab1c257df68b99b3112eaa0cdf6a
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz.asc' krb5_1.19.2.orig.tar.gz.asc 833 SHA256:afaa581a1551eba22c1f193c04f913193785e2dce12677ff2aed80503a99a8f8
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.19.2-2.debian.tar.xz' krb5_1.19.2-2.debian.tar.xz 106876 SHA256:1118a2525352c4f5b5e15b38f9b2ac1b3ef773ef9001abac694af3b09fa4b4ac
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.19.2-2/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.19.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.19.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libbsd=0.11.5-1`

Binary Packages:

- `libbsd0:amd64=0.11.5-1+b1`

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
$ apt-get source -qq --print-uris libbsd=0.11.5-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.5-1.dsc' libbsd_0.11.5-1.dsc 2292 SHA256:51479863a91fc2293da337d926862465e460bf4afdc3c0b362939749bfee6c53
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.5.orig.tar.xz' libbsd_0.11.5.orig.tar.xz 409972 SHA256:1a9c952525635c1bb6770cb22e969b938d8e6a9d7912362b98ee8370599b0efd
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.5.orig.tar.xz.asc' libbsd_0.11.5.orig.tar.xz.asc 833 SHA256:95e418668c1d3f16a63dca24b9149119bdaf5095a3e1f3f84673be1a108a0916
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.5-1.debian.tar.xz' libbsd_0.11.5-1.debian.tar.xz 17604 SHA256:83d6f3205c8e0119de85763831f3e09a8152a695d2cebc5a55069472e97e6d0c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.11.5-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.11.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.11.5-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libfido2=1.10.0-1`

Binary Packages:

- `libfido2-1:amd64=1.10.0-1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.10.0-1
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.10.0-1.dsc' libfido2_1.10.0-1.dsc 2588 SHA256:b138152c6697d51750fad315cf4ac445b7ad063d665579b06b0631cb378a2093
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.10.0.orig.tar.gz' libfido2_1.10.0.orig.tar.gz 591372 SHA256:526efd3d56af706c05d09f3d21f18ee3b0b15ac0c1f5c5da1acbc27c2730b99b
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.10.0.orig.tar.gz.asc' libfido2_1.10.0.orig.tar.gz.asc 833 SHA256:cb37e6950164449ca7034c2f926c133ff2a9d2731540c34f6b53ff551a983ca8
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.10.0-1.debian.tar.xz' libfido2_1.10.0-1.debian.tar.xz 52432 SHA256:99ecd71741e1157b1e35cf133d2a9f1292978d28075708568c3922e0077a398c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfido2/1.10.0-1/ (for browsing the source)
- https://sources.debian.net/src/libfido2/1.10.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfido2/1.10.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libssh2=1.10.0-2`

Binary Packages:

- `libssh2-1:amd64=1.10.0-2`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libssh2/1.10.0-2/


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

### `dpkg` source package: `libxcrypt=1:4.4.27-1.1`

Binary Packages:

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

### `dpkg` source package: `mawk=1.3.4.20200120-3`

Binary Packages:

- `mawk=1.3.4.20200120-3+b1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-3
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.dsc' mawk_1.3.4.20200120-3.dsc 1915 SHA256:f4abc66a6fec057b0e53ec19af866a71e17c21693f8892dd4c645bd45f832bf5
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.debian.tar.xz' mawk_1.3.4.20200120-3.debian.tar.xz 7520 SHA256:8704bade64d28252f8a49d673049e52e61b6451ccd2ba3a2c0062a36e28aed34
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.4.20200120-3/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.4.20200120-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.4.20200120-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `media-types=5.0.0`

Binary Packages:

- `media-types=5.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/media-types/5.0.0/


### `dpkg` source package: `mercurial=6.0.2-1`

Binary Packages:

- `mercurial=6.0.2-1`
- `mercurial-common=6.0.2-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=6.0.2-1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.0.2-1.dsc' mercurial_6.0.2-1.dsc 2799 SHA256:cb572b9668a7b639e12894ee249baf68e241be0bd0307bbc6749edef6aa55ce8
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.0.2.orig.tar.gz' mercurial_6.0.2.orig.tar.gz 8089180 SHA256:5fb4c36d3856292ebf584051d59306d96ad8aa32b5537452b1d9c476f95ab11a
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.0.2.orig.tar.gz.asc' mercurial_6.0.2.orig.tar.gz.asc 659 SHA256:1eb4697e4847cee637eae38ada61fa9326ed840bd47247304953512858c0f5bc
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.0.2-1.debian.tar.xz' mercurial_6.0.2-1.debian.tar.xz 68420 SHA256:bc0dc4a170748be3d63076b1aa4d9f3097b4525bd1db1d48144ca447122f5a66
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/6.0.2-1/ (for browsing the source)
- https://sources.debian.net/src/mercurial/6.0.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/6.0.2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ncurses=6.3-2`

Binary Packages:

- `libncurses6:amd64=6.3-2`
- `libncursesw6:amd64=6.3-2`
- `libtinfo6:amd64=6.3-2`
- `ncurses-base=6.3-2`
- `ncurses-bin=6.3-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

- `libldap-2.4-2:amd64=2.4.59+dfsg-1+b1`

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

### `dpkg` source package: `openssh=1:8.9p1-3`

Binary Packages:

- `openssh-client=1:8.9p1-3`

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
$ apt-get source -qq --print-uris openssh=1:8.9p1-3
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.9p1-3.dsc' openssh_8.9p1-3.dsc 3347 SHA256:a2a80fc6996b7515d78ba95a9af0bb2118c77c0c7667ec88800289cb3b37116a
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.9p1.orig.tar.gz' openssh_8.9p1.orig.tar.gz 1820282 SHA256:fd497654b7ab1686dac672fb83dfb4ba4096e8b5ffcdaccd262380ae58bec5e7
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.9p1.orig.tar.gz.asc' openssh_8.9p1.orig.tar.gz.asc 833 SHA256:ed9b972e9a1c1474d279fa97f2a03431e14e888e1b18eff93570962843320d58
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.9p1-3.debian.tar.xz' openssh_8.9p1-3.debian.tar.xz 187396 SHA256:622cf1c9ab5e804d39400d97ca2a57324c02773af0f27c60c20dcff22c82ca97
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:8.9p1-3/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:8.9p1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:8.9p1-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `pcre2=10.39-3`

Binary Packages:

- `libpcre2-8-0:amd64=10.39-3`

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

### `dpkg` source package: `perl=5.34.0-3`

Binary Packages:

- `libperl5.34:amd64=5.34.0-3`
- `perl=5.34.0-3`
- `perl-base=5.34.0-3`
- `perl-modules-5.34=5.34.0-3`

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
$ apt-get source -qq --print-uris perl=5.34.0-3
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0-3.dsc' perl_5.34.0-3.dsc 2886 SHA256:acb529cd657abf922f1de02acf69a41de852c737e77d3f210aa3bf37eea16b92
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0.orig-regen-configure.tar.xz' perl_5.34.0.orig-regen-configure.tar.xz 415412 SHA256:b168f566401fdccc13d0616c258854c1e1a461276922babca617097cd9dfd85b
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0.orig.tar.xz' perl_5.34.0.orig.tar.xz 12881416 SHA256:82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0-3.debian.tar.xz' perl_5.34.0-3.debian.tar.xz 166688 SHA256:08d20f11e429ccbf10c070b1de88016124360d367130b24abb22850addc8fd2b
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.34.0-3/ (for browsing the source)
- https://sources.debian.net/src/perl/5.34.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.34.0-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `procps=2:3.3.17-6`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-6`
- `procps=2:3.3.17-6`

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

- http://snapshot.debian.org/package/procps/2:3.3.17-6/


### `dpkg` source package: `python3-defaults=3.9.8-1`

Binary Packages:

- `libpython3-stdlib:amd64=3.9.8-1`
- `python3=3.9.8-1`
- `python3-minimal=3.9.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.9.8-1
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.9.8-1.dsc' python3-defaults_3.9.8-1.dsc 2879 SHA256:396f523c062fe7fccd14ea3a4e24d4943c690090511d15794555aaa4f18aef4d
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.9.8-1.tar.gz' python3-defaults_3.9.8-1.tar.gz 141222 SHA256:e9e9fb0d525d05f2790e89726d68425cb3469e1b157705752561bd62937f8fcd
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3-defaults/3.9.8-1/ (for browsing the source)
- https://sources.debian.net/src/python3-defaults/3.9.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3-defaults/3.9.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3.9=3.9.10-2`

Binary Packages:

- `libpython3.9-minimal:amd64=3.9.10-2`
- `libpython3.9-stdlib:amd64=3.9.10-2`
- `python3.9=3.9.10-2`
- `python3.9-minimal=3.9.10-2`

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
$ apt-get source -qq --print-uris python3.9=3.9.10-2
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.10-2.dsc' python3.9_3.9.10-2.dsc 3500 SHA256:6b21331e9c00e63e3a79537bf2236c78c37e3f26cd2cc6def56d31f0c6bb6393
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.10.orig.tar.xz' python3.9_3.9.10.orig.tar.xz 19154136 SHA256:0a8fbfb5287ebc3a13e9baf3d54e08fa06778ffeccf6311aef821bb3a6586cc8
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.10-2.debian.tar.xz' python3.9_3.9.10-2.debian.tar.xz 213192 SHA256:0f4924ef9ad48792552fa7b89cb9401f81629056cf0affa49a3d837209f0c54f
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.9/3.9.10-2/ (for browsing the source)
- https://sources.debian.net/src/python3.9/3.9.10-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.9/3.9.10-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.1.2-1`

Binary Packages:

- `libreadline8:amd64=8.1.2-1`
- `readline-common=8.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

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


### `dpkg` source package: `shadow=1:4.11.1+dfsg1-1`

Binary Packages:

- `login=1:4.11.1+dfsg1-1`
- `passwd=1:4.11.1+dfsg1-1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/shadow/1:4.11.1+dfsg1-1/


### `dpkg` source package: `sqlite3=3.38.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.38.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.38.0-1/


### `dpkg` source package: `subversion=1.14.1-3`

Binary Packages:

- `libsvn1:amd64=1.14.1-3+b4`
- `subversion=1.14.1-3+b4`

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

### `dpkg` source package: `systemd=250.3-2`

Binary Packages:

- `libsystemd0:amd64=250.3-2`
- `libudev1:amd64=250.3-2`

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
$ apt-get source -qq --print-uris systemd=250.3-2
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_250.3-2.dsc' systemd_250.3-2.dsc 5721 SHA256:1c764f2a4b7ecf3282ab13bab6918552d06aa5d2926a915c3e69d8f06e694ef2
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_250.3.orig.tar.gz' systemd_250.3.orig.tar.gz 11125151 SHA256:87b0eee7b6e5aaab2ab56d158f9536daa6bfd5de011f2a5fc6ccdd81ee1e7a24
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_250.3-2.debian.tar.xz' systemd_250.3-2.debian.tar.xz 165052 SHA256:47b504a06e84a5b6f818cb46135262383153c04ac3b2f4db90283824364ec5b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/250.3-2/ (for browsing the source)
- https://sources.debian.net/src/systemd/250.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/250.3-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `util-linux=2.37.3-1`

Binary Packages:

- `bsdutils=1:2.37.3-1+b1`
- `libblkid1:amd64=2.37.3-1+b1`
- `libmount1:amd64=2.37.3-1+b1`
- `libsmartcols1:amd64=2.37.3-1+b1`
- `libuuid1:amd64=2.37.3-1+b1`
- `mount=2.37.3-1+b1`
- `util-linux=2.37.3-1+b1`

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

Source:

```console
$ apt-get source -qq --print-uris util-linux=2.37.3-1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.3-1.dsc' util-linux_2.37.3-1.dsc 4454 SHA256:9f97d1679da1ac683605256d0cfdbf11a1892cc461812a728f6911a6cf05f8b6
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.3.orig.tar.xz' util-linux_2.37.3.orig.tar.xz 6126260 SHA256:590c592e58cd6bf38519cb467af05ce6a1ab18040e3e3418f24bcfb2f55f9776
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.37.3-1.debian.tar.xz' util-linux_2.37.3-1.debian.tar.xz 99240 SHA256:7ba53657ebefb530b52269834443218f573335b3ae844f3bd421600417f1fb01
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.37.3-1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.37.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.37.3-1/ (for access to the source package after it no longer exists in the archive)

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
