# `sentry:9.1.2-onbuild`

## Docker Metadata

- Image ID: `sha256:a7a01fc9c574a74f3863b4c5b32b6a2841470de1e8057c9209c4c97829a2d646`
- Created: `2019-10-19T09:00:54.914843642Z`
- Virtual Size: ~ 868.75 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/entrypoint.sh"]`
- Command: `["run","web"]`
- Environment:
  - `PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `PYTHONIOENCODING=UTF-8`
  - `GPG_KEY=C01E1CAD5EA2C4F0B8E3571504C367C218ADD4FF`
  - `PYTHON_VERSION=2.7.16`
  - `PYTHON_PIP_VERSION=19.3.1`
  - `PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/ffe826207a010164265d9cc807978e3604d18ca0/get-pip.py`
  - `PYTHON_GET_PIP_SHA256=b86f36cc4345ae87bfd4f10ef6b2dbfa7a872fbff70608a1e43944d283fd0eee`
  - `PIP_NO_CACHE_DIR=off`
  - `PIP_DISABLE_PIP_VERSION_CHECK=on`
  - `SENTRY_VERSION=9.1.2`
  - `SENTRY_CONF=/etc/sentry`
  - `SENTRY_FILESTORE_DIR=/var/lib/sentry/files`
  - `PYTHONPATH=/usr/src/sentry`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3`

Binary Packages:

- `libacl1:amd64=2.2.52-3+b1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-3.dsc' acl_2.2.52-3.dsc 2025 SHA256:82e344b9ab176559a85630b74ee5a68d678d7f24b6fe8139f2fd9fcf38a48095
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-3.debian.tar.xz' acl_2.2.52-3.debian.tar.xz 8740 SHA256:fc3f1178d18288993fc4ce4853b7f9dcdf0bd1fd26e4f69349a4e4e5916d1fa8
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.52-3/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.52-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.52-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.115`

Binary Packages:

- `adduser=3.115`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.115
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.115.dsc' adduser_3.115.dsc 1701 SHA256:754698aa19d7521080ecacc8033baa20cfa4a963021de6061c68ffa6ee15e9a1
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.115.tar.xz' adduser_3.115.tar.xz 213620 SHA256:e7288281d4d1eec2948ba3687452ca33a8224d40c98d321bc3fbaefcf6d4c0db
```

Other potentially useful URLs:

- https://sources.debian.net/src/adduser/3.115/ (for browsing the source)
- https://sources.debian.net/src/adduser/3.115/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adduser/3.115/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=1.4.9`

Binary Packages:

- `apt=1.4.9`
- `libapt-pkg5.0:amd64=1.4.9`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/1.4.9/


### `dpkg` source package: `attr=1:2.4.47-2`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2+b2`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47-2.dsc' attr_2.4.47-2.dsc 2027 SHA256:ee842d6d62d473acf02b494c432cf33128fa46455a09d3172c77c252449fa1a6
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.47-2.debian.tar.xz' attr_2.4.47-2.debian.tar.xz 8096 SHA256:f65909562def601b1556393f5656032c058dc574ba622414ad3eb80c7b05a42a
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.4.47-2/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.4.47-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.4.47-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:2.6.7-2`

Binary Packages:

- `libaudit-common=1:2.6.7-2`
- `libaudit1:amd64=1:2.6.7-2`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.6.7-2
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.6.7-2.dsc' audit_2.6.7-2.dsc 2485 SHA256:3cc48a56a06f29cff62d35267471d1775a5b201cd947385566fc8f8d49bc1280
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.6.7.orig.tar.gz' audit_2.6.7.orig.tar.gz 1080848 SHA256:8923917332daa7833bbc0c1d9eb012167093fbad000da4a9630fb3356aff8cdc
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.6.7-2.debian.tar.xz' audit_2.6.7-2.debian.tar.xz 18820 SHA256:04b40b6ae73625c6a27a9949b28c751a83c97220f59a712b2ea9c03f5cab0fcf
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:2.6.7-2/ (for browsing the source)
- https://sources.debian.net/src/audit/1:2.6.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:2.6.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=9.9+deb9u11`

Binary Packages:

- `base-files=9.9+deb9u11`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-files/9.9+deb9u11/


### `dpkg` source package: `base-passwd=3.5.43`

Binary Packages:

- `base-passwd=3.5.43`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.43
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.43.dsc' base-passwd_3.5.43.dsc 1749 SHA256:174a03d0df0d0f36cc186592e36472339632de094d60f9fcab370e1101a2430d
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.43.tar.xz' base-passwd_3.5.43.tar.xz 52596 SHA256:7768d10e2c08469cc81342e391e059f0426afdb6eb74a3102beef59ac45ab994
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.43/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.43/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.43/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=4.4-5`

Binary Packages:

- `bash=4.4-5`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.4-5
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4-5.dsc' bash_4.4-5.dsc 2251 SHA256:1605c608c48f3d866e23a3d6989d23c1d910d58b2a64eee13ad0efd2d98d4b06
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4.orig.tar.xz' bash_4.4.orig.tar.xz 4878580 SHA256:819ebb6a23799e9e4ca56ac579778c46902005bd5ade4f131ed293d9f77108e7
'http://deb.debian.org/debian/pool/main/b/bash/bash_4.4-5.debian.tar.xz' bash_4.4-5.debian.tar.xz 65640 SHA256:e01cc0f49941d81bee4e81f3eeefede280a91ad9365947234f29f1cb783f9dd8
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/4.4-5/ (for browsing the source)
- https://sources.debian.net/src/bash/4.4-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/4.4-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `binutils=2.28-5`

Binary Packages:

- `binutils=2.28-5`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.28-5
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.28-5.dsc' binutils_2.28-5.dsc 4380 SHA256:a835d9d6e2d102a4c04c07259c7a2810c11935d70f43fdb31c5b01c4c01da380
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.28.orig.tar.gz' binutils_2.28.orig.tar.gz 37814356 SHA256:db29588b0214fa69baa1a9351122cd6d0f081f2e675e6ad2aefc316ddeaf327a
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.28-5.diff.gz' binutils_2.28-5.diff.gz 129501 SHA256:7cb92a4ca5b3afdd1c6a735ff7876b7751f83aaa887d6eb5cf0ec919bf850a35
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.28-5/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.28-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.28-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.6-8.1`

Binary Packages:

- `libbz2-1.0:amd64=1.0.6-8.1`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8.1
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-8.1.dsc' bzip2_1.0.6-8.1.dsc 2082 SHA256:d80deed11a1419ad090cb486dd2335850fd8719b809c32002dea04b485f55dbd
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-8.1.debian.tar.bz2' bzip2_1.0.6-8.1.debian.tar.bz2 59875 SHA256:bdbe7bf29e014e44d79bb7c733fe63cae990ab50882a4a07867cf69c61ad72b7
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.6-8.1/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.6-8.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.6-8.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20161130+nmu1+deb9u1`

Binary Packages:

- `ca-certificates=20161130+nmu1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ca-certificates/20161130+nmu1+deb9u1/


### `dpkg` source package: `cdebconf=0.227`

Binary Packages:

- `libdebconfclient0:amd64=0.227`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.227
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.227.dsc' cdebconf_0.227.dsc 2662 SHA256:23531e6cbf4acb4edc5a2c3eda7a5095b82c396d801ade72d669b6fcf2c5aaa2
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.227.tar.xz' cdebconf_0.227.tar.xz 272716 SHA256:df2092bb5d4fe76c318adfd1cc756f78b48a668704b6e71e161143e7c782da58
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.227/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.227/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.227/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.26-3`

Binary Packages:

- `coreutils=8.26-3`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.26-3
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.26-3.dsc' coreutils_8.26-3.dsc 1955 SHA256:f62ab642e46e02c470cc045316643de530a0be50446151a5e449ca12da6485c4
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.26.orig.tar.xz' coreutils_8.26.orig.tar.xz 5810244 SHA256:155e94d748f8e2bc327c66e0cbebdb8d6ab265d2f37c3c928f7bf6c3beba9a8e
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.26-3.debian.tar.xz' coreutils_8.26-3.debian.tar.xz 22392 SHA256:cef6a15eb95d9e7bc992bca95010bc5ea9e25e98d8f4f668a698eee534d14b93
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/8.26-3/ (for browsing the source)
- https://sources.debian.net/src/coreutils/8.26-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/8.26-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.52.1-5+deb9u9`

Binary Packages:

- `libcurl3-gnutls:amd64=7.52.1-5+deb9u9`

Licenses: (parsed from: `/usr/share/doc/libcurl3-gnutls/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/curl/7.52.1-5+deb9u9/


### `dpkg` source package: `cyrus-sasl2=2.1.27~101-g0780600+dfsg-3`

Binary Packages:

- `libsasl2-2:amd64=2.1.27~101-g0780600+dfsg-3`
- `libsasl2-modules-db:amd64=2.1.27~101-g0780600+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3/


### `dpkg` source package: `dash=0.5.8-2.4`

Binary Packages:

- `dash=0.5.8-2.4`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.8-2.4
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.8-2.4.dsc' dash_0.5.8-2.4.dsc 1461 SHA256:c83f68c3727e9fd3691117d1f67a2bd049ae2411d2137d50ea6d36122cec6482
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.8.orig.tar.gz' dash_0.5.8.orig.tar.gz 223028 SHA256:c6db3a237747b02d20382a761397563d813b306c020ae28ce25a1c3915fac60f
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.8-2.4.diff.gz' dash_0.5.8-2.4.diff.gz 44058 SHA256:230717c04af659a6a09b2c39158d9167fdd3392a6716c0ff36fe40dff1ca8b9d
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.8-2.4/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.8-2.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.8-2.4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28-12+deb9u1`

Binary Packages:

- `libdb5.3:amd64=5.3.28-12+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-12+deb9u1
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-12+deb9u1.dsc' db5.3_5.3.28-12+deb9u1.dsc 3266 SHA256:22284095ad8d13f640736d3a3d2b05598497f4ce1a5b370f174217b497d8ccc7
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-12+deb9u1.debian.tar.xz' db5.3_5.3.28-12+deb9u1.debian.tar.xz 28348 SHA256:66b31f416940b48f3c09e8c1780feabe8e928742e5e819dde4ee1004ad828f3e
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28-12+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28-12+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28-12+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.61`

Binary Packages:

- `debconf=1.5.61`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.61
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.61.dsc' debconf_1.5.61.dsc 1932 SHA256:a350712c205bf21f045c80f4a64e24cef27e35e38fd51080c79076178c63ef1b
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.61.tar.xz' debconf_1.5.61.tar.xz 570372 SHA256:7622a3fe231b46e6255a83b3d153159c10be6bc17b2152ab3937b8928bf87e10
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.61/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.61/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.61/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debian-archive-keyring=2017.5+deb9u1`

Binary Packages:

- `debian-archive-keyring=2017.5+deb9u1`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2017.5+deb9u1
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.5+deb9u1.dsc' debian-archive-keyring_2017.5+deb9u1.dsc 1827 SHA256:bc03dac3958c0d9de0a161fbd1ea3d69cd8e9146df4ce6fa4b69f80189c6b21b
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.5+deb9u1.tar.xz' debian-archive-keyring_2017.5+deb9u1.tar.xz 116344 SHA256:dcfffc87cc382bda49de654d205abb586519c0859d6c570f1eabdfa997350806
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2017.5+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2017.5+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2017.5+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=4.8.1.1`

Binary Packages:

- `debianutils=4.8.1.1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.1.1
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.1.1.dsc' debianutils_4.8.1.1.dsc 1739 SHA256:506d5e6c18e38831eb45ab1ecc35dd8cc3e931b0fe7367136fb7d42520130a84
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.1.1.tar.xz' debianutils_4.8.1.1.tar.xz 156256 SHA256:06446cd4c0d309fd31a0682c5c2f07f7613fb867f769414b9cc51f155ad73172
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.8.1.1/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.8.1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.8.1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.5-3`

Binary Packages:

- `diffutils=1:3.5-3`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.5-3
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.5-3.dsc' diffutils_3.5-3.dsc 1453 SHA256:8b8e4d9d48ab35fd2c5759a3d0854e7d85c33b3fa09a185c20865793090feff9
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.5.orig.tar.xz' diffutils_3.5.orig.tar.xz 1360996 SHA256:dad398ccd5b9faca6b0ab219a036453f62a602a56203ac659b43e889bec35533
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.5-3.debian.tar.xz' diffutils_3.5-3.debian.tar.xz 10796 SHA256:5c8464482951de1dcf3c1c53643cd7d0939cd8f7568a7ef84982d368c5cb6695
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.5-3/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.5-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.5-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.18.25`

Binary Packages:

- `dpkg=1.18.25`
- `libdpkg-perl=1.18.25`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.18.25
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.18.25.dsc' dpkg_1.18.25.dsc 2048 SHA256:5cf6ac260dc3adae91516b777f9e3b6fcb783d867f811fa8fd0787f570a059a6
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.18.25.tar.xz' dpkg_1.18.25.tar.xz 4541640 SHA256:c49c371953aea03f543814dcae37c069e86069333fb2e24e9252e76647663492
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.18.25/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.18.25/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.18.25/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.43.4-2+deb9u1`

Binary Packages:

- `e2fslibs:amd64=1.43.4-2+deb9u1`
- `e2fsprogs=1.43.4-2+deb9u1`
- `libcomerr2:amd64=1.43.4-2+deb9u1`
- `libss2:amd64=1.43.4-2+deb9u1`

Licenses: (parsed from: `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.43.4-2+deb9u1
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.43.4-2+deb9u1.dsc' e2fsprogs_1.43.4-2+deb9u1.dsc 2071 SHA256:b3d4d80f72ef552369448b0f2ecc2b68e3a670fdab5a14705fcaf8607579cc32
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.43.4.orig.tar.gz' e2fsprogs_1.43.4.orig.tar.gz 7552218 SHA256:484ab0bc1bc07c64267b18cfe7871b6b975bf0a705c5a4563001f035071cdc7c
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.43.4-2+deb9u1.debian.tar.xz' e2fsprogs_1.43.4-2+deb9u1.debian.tar.xz 78168 SHA256:d238b0872e2aad029fbcd02a9e83242befb3b2cc445bbaa4712a90f2741fbeeb
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.43.4-2+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.43.4-2+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.43.4-2+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.0-2+deb9u3`

Binary Packages:

- `libexpat1:amd64=2.2.0-2+deb9u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.2.0-2+deb9u3
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.0-2+deb9u3.dsc' expat_2.2.0-2+deb9u3.dsc 2450 SHA256:11f83d0c9912cf287b53b72636dc8049656477d05bffd3ecf56c29709bfec33f
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.0.orig.tar.bz2' expat_2.2.0.orig.tar.bz2 414352 SHA256:d9e50ff2d19b3538bd2127902a89987474e1a4db8e43a66a4d1a712ab9a504ff
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.0-2+deb9u3.debian.tar.xz' expat_2.2.0-2+deb9u3.debian.tar.xz 12608 SHA256:68800c47feebefea7318e767d6837b7c84ad875ab53d188e951d4859eddba241
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.0-2+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.0-2+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.0-2+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.6.0+git+20161106-2`

Binary Packages:

- `findutils=4.6.0+git+20161106-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20161106-2
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20161106-2.dsc' findutils_4.6.0+git+20161106-2.dsc 2220 SHA256:f92d95f03e56357bb72e897f4d8b363995f280cfdf6dedfabdec3164f3a7651a
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20161106.orig.tar.xz' findutils_4.6.0+git+20161106.orig.tar.xz 1828956 SHA256:96a3aa120d7300863f39fe56ccb6674d8cde4730b485f4f81083c1a6d33097e3
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20161106-2.debian.tar.xz' findutils_4.6.0+git+20161106-2.debian.tar.xz 26812 SHA256:aca885ac24582f5c393dbbfa362264712ee4922da0ff7aa1fc602e629c89b71b
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.6.0+git+20161106-2/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.6.0+git+20161106-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.6.0+git+20161106-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-6=6.3.0-18+deb9u1`

Binary Packages:

- `cpp-6=6.3.0-18+deb9u1`
- `gcc-6=6.3.0-18+deb9u1`
- `gcc-6-base:amd64=6.3.0-18+deb9u1`
- `libasan3:amd64=6.3.0-18+deb9u1`
- `libatomic1:amd64=6.3.0-18+deb9u1`
- `libcc1-0:amd64=6.3.0-18+deb9u1`
- `libcilkrts5:amd64=6.3.0-18+deb9u1`
- `libgcc-6-dev:amd64=6.3.0-18+deb9u1`
- `libgcc1:amd64=1:6.3.0-18+deb9u1`
- `libgomp1:amd64=6.3.0-18+deb9u1`
- `libitm1:amd64=6.3.0-18+deb9u1`
- `liblsan0:amd64=6.3.0-18+deb9u1`
- `libmpx2:amd64=6.3.0-18+deb9u1`
- `libquadmath0:amd64=6.3.0-18+deb9u1`
- `libstdc++-6-dev:amd64=6.3.0-18+deb9u1`
- `libstdc++6:amd64=6.3.0-18+deb9u1`
- `libtsan0:amd64=6.3.0-18+deb9u1`
- `libubsan0:amd64=6.3.0-18+deb9u1`

Licenses: (parsed from: `/usr/share/doc/cpp-6/copyright`, `/usr/share/doc/gcc-6/copyright`, `/usr/share/doc/gcc-6-base/copyright`, `/usr/share/doc/libasan3/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-6-dev/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libmpx2/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-6-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-6=6.3.0-18+deb9u1
'http://deb.debian.org/debian/pool/main/g/gcc-6/gcc-6_6.3.0-18+deb9u1.dsc' gcc-6_6.3.0-18+deb9u1.dsc 27148 SHA256:8145f139255d35dac4c922321cb98ba11a73296a886a76563a5eef309e1d5bec
'http://deb.debian.org/debian/pool/main/g/gcc-6/gcc-6_6.3.0.orig.tar.gz' gcc-6_6.3.0.orig.tar.gz 81587460 SHA256:04552f04baf6974fb7521191859fb54717385ad659afd822b2995b66ee4e4151
'http://deb.debian.org/debian/pool/main/g/gcc-6/gcc-6_6.3.0-18+deb9u1.diff.gz' gcc-6_6.3.0-18+deb9u1.diff.gz 2075943 SHA256:8c705553bf211e064f3270e51e81a6b2a0bf122f39f7c98ce7f2fbdfd9fa9564
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-6/6.3.0-18+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/gcc-6/6.3.0-18+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-6/6.3.0-18+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-defaults=1.168`

Binary Packages:

- `cpp=4:6.3.0-4`
- `gcc=4:6.3.0-4`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.168
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.168.dsc' gcc-defaults_1.168.dsc 13173 SHA256:05a2a34278108aec64227a63cb61d9562bca9380f8539562e7e42023dca2d1c8
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.168.tar.gz' gcc-defaults_1.168.tar.gz 69321 SHA256:4ecc5edafbf47d43c8b872e36c9a87c95691bed94eaa6e8f55adfc8fd64e5587
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-defaults/1.168/ (for browsing the source)
- https://sources.debian.net/src/gcc-defaults/1.168/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-defaults/1.168/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.8.3-14`

Binary Packages:

- `libgdbm3:amd64=1.8.3-14`

Licenses: (parsed from: `/usr/share/doc/libgdbm3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.8.3-14
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3-14.dsc' gdbm_1.8.3-14.dsc 1841 SHA256:312d3d28e287d287ee66e8ae3f25769676b1680ec1adc8c0815b5e9808405b13
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3.orig.tar.bz2' gdbm_1.8.3.orig.tar.bz2 172796 SHA256:1d5995b6e9e6be4ff62c8126d019f184a083dd8e6f75f6c74b9fe023b5b9440e
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3-14.debian.tar.xz' gdbm_1.8.3-14.debian.tar.xz 15308 SHA256:1c0570dd53947ea5980111f51b67356d647c4f21c502443b02397041dde0bf31
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.8.3-14/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.8.3-14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.8.3-14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.11.0-3+deb9u4`

Binary Packages:

- `git=1:2.11.0-3+deb9u4`
- `git-man=1:2.11.0-3+deb9u4`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/git/1:2.11.0-3+deb9u4/


### `dpkg` source package: `glib2.0=2.50.3-2+deb9u1`

Binary Packages:

- `libglib2.0-0:amd64=2.50.3-2+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.50.3-2+deb9u1
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.50.3-2+deb9u1.dsc' glib2.0_2.50.3-2+deb9u1.dsc 3451 SHA256:1ec772f446253b189271f35106e39aa84a74a57796c9b1d09f3fe4b6f608c1bb
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.50.3.orig.tar.xz' glib2.0_2.50.3.orig.tar.xz 7589284 SHA256:82ee94bf4c01459b6b00cb9db0545c2237921e3060c0b74cff13fbc020cfd999
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.50.3-2+deb9u1.debian.tar.xz' glib2.0_2.50.3-2+deb9u1.debian.tar.xz 74472 SHA256:305398721ed8c790b677e44850228fd04efd1b9da7181bb0eedd9822ad7ff5d7
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.50.3-2+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.50.3-2+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.50.3-2+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.24-11+deb9u4`

Binary Packages:

- `libc-bin=2.24-11+deb9u4`
- `libc-dev-bin=2.24-11+deb9u4`
- `libc6:amd64=2.24-11+deb9u4`
- `libc6-dev:amd64=2.24-11+deb9u4`
- `multiarch-support=2.24-11+deb9u4`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.24-11+deb9u4
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.24-11+deb9u4.dsc' glibc_2.24-11+deb9u4.dsc 8386 SHA256:0cfc10b8f713f41c087476a0a9f6687b4ccb22c5652502bfe8e5c0798f8b097f
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.24.orig.tar.xz' glibc_2.24.orig.tar.xz 13921912 SHA256:ed71e8afd2b270f7947a2cea2457a31e1ca4fac08e2731d80edd7ec1730ec84f
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.24-11+deb9u4.debian.tar.xz' glibc_2.24-11+deb9u4.debian.tar.xz 1060620 SHA256:bcf78fb5157cd84d26cdc4b3366b1d5e92fc13609a465ac63ff322a5adac3cbc
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.24-11+deb9u4/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.24-11+deb9u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.24-11+deb9u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.1.2+dfsg-1`

Binary Packages:

- `libgmp-dev:amd64=2:6.1.2+dfsg-1`
- `libgmp10:amd64=2:6.1.2+dfsg-1`
- `libgmpxx4ldbl:amd64=2:6.1.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-1
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-1.dsc' gmp_6.1.2+dfsg-1.dsc 2183 SHA256:3a53f6c74c9b2465c1c61446aa9bdc6182fdec8b04075849d4cbf224a73b6fbe
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-1.debian.tar.xz' gmp_6.1.2+dfsg-1.debian.tar.xz 20652 SHA256:79e73f74197e7628b2f0c02edf01b6eea3716c13152044ed8e0e0ee4178394df
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.1.2+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.1.18-8~deb9u4`

Binary Packages:

- `gpgv=2.1.18-8~deb9u4`

Licenses: (parsed from: `/usr/share/doc/gpgv/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris gnupg2=2.1.18-8~deb9u4
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.1.18-8~deb9u4.dsc' gnupg2_2.1.18-8~deb9u4.dsc 2561 SHA256:e42240a13af866a3c9db1704bfbbd2230abb071dca3c24d7c2a3b27e94d8aaa3
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.1.18.orig.tar.bz2' gnupg2_2.1.18.orig.tar.bz2 6308666 SHA256:d04c6fab7e5562ce4b915b22020e34d4c1a256847690cf149842264fc7cef994
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.1.18-8~deb9u4.debian.tar.bz2' gnupg2_2.1.18-8~deb9u4.debian.tar.bz2 122023 SHA256:81f6cf52bc22d77332a413ec2cd423e2127faea950705b50b50f84c8ed43521e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.1.18-8~deb9u4/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.1.18-8~deb9u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.1.18-8~deb9u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.5.8-5+deb9u4`

Binary Packages:

- `libgnutls-dane0:amd64=3.5.8-5+deb9u4`
- `libgnutls-openssl27:amd64=3.5.8-5+deb9u4`
- `libgnutls28-dev:amd64=3.5.8-5+deb9u4`
- `libgnutls30:amd64=3.5.8-5+deb9u4`
- `libgnutlsxx28:amd64=3.5.8-5+deb9u4`

Licenses: (parsed from: `/usr/share/doc/libgnutls-dane0/copyright`, `/usr/share/doc/libgnutls-openssl27/copyright`, `/usr/share/doc/libgnutls28-dev/copyright`, `/usr/share/doc/libgnutls30/copyright`, `/usr/share/doc/libgnutlsxx28/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The MIT License (MIT)`
- `The main library is licensed under GNU Lesser`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gnutls28/3.5.8-5+deb9u4/


### `dpkg` source package: `grep=2.27-2`

Binary Packages:

- `grep=2.27-2`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=2.27-2
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.27-2.dsc' grep_2.27-2.dsc 2053 SHA256:c048a1ad8c39877c2fb0279887c8ea93e59591788fdb08e2f75249ebdcecdea7
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.27.orig.tar.xz' grep_2.27.orig.tar.xz 1360388 SHA256:ad4cc44d23074a1c3a8baae8fbafff2a8c60f38a9a6108f985eef6fbee6dcaeb
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.27-2.debian.tar.bz2' grep_2.27-2.debian.tar.bz2 112728 SHA256:445eaf71811df5ca18242fb5adc417d35e349e49810201977bf7086746b967f4
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/2.27-2/ (for browsing the source)
- https://sources.debian.net/src/grep/2.27-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/2.27-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.6-5`

Binary Packages:

- `gzip=1.6-5+b1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-5
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-5.dsc' gzip_1.6-5.dsc 1867 SHA256:922751ee5fc426d623e824c55f7822fa60f26f35b5389b37c8b15feff639608c
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-5.debian.tar.xz' gzip_1.6-5.debian.tar.xz 14684 SHA256:ac5282c32083ff58fc01317ee402b687b3806555aa1d4e80a62bb0f2ad93167e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.6-5/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.6-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.6-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hostname=3.18`

Binary Packages:

- `hostname=3.18+b1`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.18
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.18.dsc' hostname_3.18.dsc 1446 SHA256:4d3d5c8ded08ffc2ebfb39817ba1994b5fc1966652b132ff3e16389b70af28d7
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.18.tar.gz' hostname_3.18.tar.gz 13732 SHA256:5cc3ec120967b8f911e86b9561b53977bcc77191c84fe9c607177ccd09f8d207
```

Other potentially useful URLs:

- https://sources.debian.net/src/hostname/3.18/ (for browsing the source)
- https://sources.debian.net/src/hostname/3.18/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hostname/3.18/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `icu=57.1-6+deb9u3`

Binary Packages:

- `icu-devtools=57.1-6+deb9u3`
- `libicu-dev=57.1-6+deb9u3`
- `libicu57:amd64=57.1-6+deb9u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/icu/57.1-6+deb9u3/


### `dpkg` source package: `init-system-helpers=1.48`

Binary Packages:

- `init-system-helpers=1.48`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.48
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.48.dsc' init-system-helpers_1.48.dsc 1916 SHA256:aefcef5270cfae3380f9dfd98336de20580086dbdc65c0dfd7fe1c10f0722bd0
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.48.tar.xz' init-system-helpers_1.48.tar.xz 43384 SHA256:20b4ff9df037cfa64d6c9637e383cb09135cb97114d932032160cdfaf01d08b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.48/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.48/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.48/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `isl=0.18-1`

Binary Packages:

- `libisl15:amd64=0.18-1`

Licenses: (parsed from: `/usr/share/doc/libisl15/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.18-1
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.18-1.dsc' isl_0.18-1.dsc 1882 SHA256:aed8295d019805686fd795652d930b1440bc0ae3be4373332d97784645d7c583
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.18.orig.tar.xz' isl_0.18.orig.tar.xz 1475708 SHA256:0f35051cc030b87c673ac1f187de40e386a1482a0cfdf2c552dd6031b307ddc4
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.18-1.debian.tar.xz' isl_0.18-1.debian.tar.xz 21860 SHA256:eac951311a871bb6d7886c98068290f771aaf78616516855b472d2500b84f53c
```

Other potentially useful URLs:

- https://sources.debian.net/src/isl/0.18-1/ (for browsing the source)
- https://sources.debian.net/src/isl/0.18-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/isl/0.18-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.5.9-9`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-9`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-9
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-9.dsc' keyutils_1.5.9-9.dsc 2033 SHA256:5fe3b2578a7ec662b7f495b11b7d861c3ee68c9550d4dec20c10ff4f3b3ca3dd
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-9.debian.tar.xz' keyutils_1.5.9-9.debian.tar.xz 17588 SHA256:2e9db3f51d902a4d8fa4bef3b914353f9f83ed53b9003f24b5fc44748f4d6d80
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.5.9-9/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.5.9-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.5.9-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.15-1+deb9u1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.15-1+deb9u1`
- `libk5crypto3:amd64=1.15-1+deb9u1`
- `libkrb5-3:amd64=1.15-1+deb9u1`
- `libkrb5support0:amd64=1.15-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.15-1+deb9u1
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.15-1+deb9u1.dsc' krb5_1.15-1+deb9u1.dsc 3373 SHA256:cb69444c826f380c9d3ea7c5e6bf04105ca2fceb26ecc14b293f458f337f34c2
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.15.orig.tar.gz' krb5_1.15.orig.tar.gz 9327157 SHA256:fd34752774c808ab4f6f864f935c49945f5a56b62240b1ad4ab1af7b4ded127c
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.15-1+deb9u1.debian.tar.xz' krb5_1.15-1+deb9u1.debian.tar.xz 144944 SHA256:f04183b2ecfd0fe488975338eb4f900d5f605c81a9ae279451ceda948d99a21c
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.15-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.15-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.15-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.7.7-3`

Binary Packages:

- `libcap-ng0:amd64=0.7.7-3+b1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.7-3
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.dsc' libcap-ng_0.7.7-3.dsc 1722 SHA256:6f5262f0ed2792c135e9b6bf7d30461cc3015249832f381505d21b9217a67685
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.7.orig.tar.gz' libcap-ng_0.7.7.orig.tar.gz 420178 SHA256:615549ce39b333f6b78baee0c0b4ef18bc726c6bf1cca123dfd89dd963f6d06b
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.debian.tar.xz' libcap-ng_0.7.7-3.debian.tar.xz 5248 SHA256:b7a0846dbd0451903bcbbe3a2696341f4e6000ebd64bed259c7fbf9dfc818363
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap-ng/0.7.7-3/ (for browsing the source)
- https://sources.debian.net/src/libcap-ng/0.7.7-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap-ng/0.7.7-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liberror-perl=0.17024-1`

Binary Packages:

- `liberror-perl=0.17024-1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17024-1
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17024-1.dsc' liberror-perl_0.17024-1.dsc 2193 SHA256:3d269abc34facfde4e4caf5d2eac38dbce07739d3fe2167ff982140af513d17e
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17024.orig.tar.gz' liberror-perl_0.17024.orig.tar.gz 31269 SHA256:074db7c783a67b0667eca64a4f6a0c3de94998afc92c01d6453163eb04b9150d
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17024-1.debian.tar.xz' liberror-perl_0.17024-1.debian.tar.xz 4028 SHA256:7b490f3655df007a1153883608161822036837eaf49f7d6014d3a096be4a65cb
```

Other potentially useful URLs:

- https://sources.debian.net/src/liberror-perl/0.17024-1/ (for browsing the source)
- https://sources.debian.net/src/liberror-perl/0.17024-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liberror-perl/0.17024-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.2.1-6`

Binary Packages:

- `libffi-dev:amd64=3.2.1-6`
- `libffi6:amd64=3.2.1-6`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-6
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-6.dsc' libffi_3.2.1-6.dsc 1923 SHA256:f901298b078c7d7f3f75459b5ff74cc804f6f2cfd65ed619d2082d5f77089954
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-6.debian.tar.xz' libffi_3.2.1-6.debian.tar.xz 11252 SHA256:477709fa90f8c7631fa226a48cdf38737c9f195f3686f62aa76714bcffaee512
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.2.1-6/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.2.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.2.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.7.6-2+deb9u3`

Binary Packages:

- `libgcrypt20:amd64=1.7.6-2+deb9u3`
- `libgcrypt20-dev=1.7.6-2+deb9u3`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`, `/usr/share/doc/libgcrypt20-dev/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.7.6-2+deb9u3
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.7.6-2+deb9u3.dsc' libgcrypt20_1.7.6-2+deb9u3.dsc 2838 SHA256:55ab5150f7ff08345d819db2d8b68ae7d443265ca35c2e6ca0c0052a59b3c1f6
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.7.6.orig.tar.bz2' libgcrypt20_1.7.6.orig.tar.bz2 2897695 SHA256:626aafee84af9d2ce253d2c143dc1c0902dda045780cc241f39970fc60be05bc
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.7.6-2+deb9u3.debian.tar.xz' libgcrypt20_1.7.6-2+deb9u3.debian.tar.xz 32760 SHA256:5947ca05db069293a0cd2c4cbb561072d5e5a13933849039e6f054290b90b57f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.7.6-2+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.7.6-2+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.7.6-2+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.26-2`

Binary Packages:

- `libgpg-error-dev=1.26-2`
- `libgpg-error0:amd64=1.26-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error-dev/copyright`, `/usr/share/doc/libgpg-error0/copyright`)

- `GPL-2.1+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.26-2
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.26-2.dsc' libgpg-error_1.26-2.dsc 2454 SHA256:ea53df72d922f224cf0bb69df5a20100a2a5826e890741277425269d70eade20
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.26.orig.tar.bz2' libgpg-error_1.26.orig.tar.bz2 798096 SHA256:4c4bcbc90116932e3acd37b37812d8653b1b189c1904985898e860af818aee69
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.26-2.debian.tar.xz' libgpg-error_1.26-2.debian.tar.xz 12740 SHA256:20a73d5bcc4f523ae16b9279698c01b37dd5cffd2b7dc317c65923aa115ca46c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.26-2/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.26-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.26-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn2-0=0.16-1+deb9u1`

Binary Packages:

- `libidn2-0:amd64=0.16-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libidn2-0/copyright`)

- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-3+`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris libidn2-0=0.16-1+deb9u1
'http://deb.debian.org/debian/pool/main/libi/libidn2-0/libidn2-0_0.16-1+deb9u1.dsc' libidn2-0_0.16-1+deb9u1.dsc 2339 SHA256:70c6e54e5a1bf1727fc79d74722e658b1ec087ea9c8e5f9eb5c506b9a3e64a79
'http://deb.debian.org/debian/pool/main/libi/libidn2-0/libidn2-0_0.16.orig.tar.gz' libidn2-0_0.16.orig.tar.gz 1494295 SHA256:2fad9efff4082ae2143f69df76339ca99379e0e0f4231455f5d3d9d2089c688f
'http://deb.debian.org/debian/pool/main/libi/libidn2-0/libidn2-0_0.16-1+deb9u1.debian.tar.xz' libidn2-0_0.16-1+deb9u1.debian.tar.xz 57988 SHA256:cfc2f155f4c97f759ce58909c624b586e1815bc5db98528a76bd12a8095844b1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2-0/0.16-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libidn2-0/0.16-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2-0/0.16-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn=1.33-1`

Binary Packages:

- `libidn11:amd64=1.33-1`
- `libidn11-dev=1.33-1`

Licenses: (parsed from: `/usr/share/doc/libidn11/copyright`, `/usr/share/doc/libidn11-dev/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libidn/1.33-1/


### `dpkg` source package: `libjpeg-turbo=1:1.5.1-2`

Binary Packages:

- `libjpeg-dev=1:1.5.1-2`
- `libjpeg62-turbo:amd64=1:1.5.1-2`
- `libjpeg62-turbo-dev:amd64=1:1.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3`
- `BSD-BY-LC-NE`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:1.5.1-2
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.1-2.dsc' libjpeg-turbo_1.5.1-2.dsc 2420 SHA256:9f755bfafa4795f91c689cb742194559f6e543e35ba135e0d30f6b51eed1eba2
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.1.orig.tar.gz' libjpeg-turbo_1.5.1.orig.tar.gz 1650647 SHA256:41429d3d253017433f66e3d472b8c7d998491d2f41caa7306b8d9a6f2a2c666c
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.1-2.debian.tar.xz' libjpeg-turbo_1.5.1-2.debian.tar.xz 78576 SHA256:0077c9e2b7ec2abe25c7a591e65a08750045a28dcd00207a928079a3d31b3cc4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:1.5.1-2/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:1.5.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:1.5.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmaxminddb=1.2.0-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.2.0-1+b1`
- `libmaxminddb0:amd64=1.2.0-1+b1`

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
$ apt-get source -qq --print-uris libmaxminddb=1.2.0-1
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.2.0-1.dsc' libmaxminddb_1.2.0-1.dsc 2115 SHA256:0c191c97687ec3bf9280d6564823c34ff203b91accf8915684b4358e84c2ab7e
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.2.0.orig.tar.gz' libmaxminddb_1.2.0.orig.tar.gz 310051 SHA256:27726894d30644be604058fb3c9c90d1afe42beb071890dbc29c7e27fbf55fa9
'http://deb.debian.org/debian/pool/main/libm/libmaxminddb/libmaxminddb_1.2.0-1.debian.tar.xz' libmaxminddb_1.2.0-1.debian.tar.xz 4228 SHA256:21f9cb39d1ae5d9e4da58b2a4d567b4db48f885b8f031e83e0a5c1ec6806ae48
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmaxminddb/1.2.0-1/ (for browsing the source)
- https://sources.debian.net/src/libmaxminddb/1.2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmaxminddb/1.2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpsl=0.17.0-3`

Binary Packages:

- `libpsl5:amd64=0.17.0-3`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.17.0-3
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.17.0-3.dsc' libpsl_0.17.0-3.dsc 2224 SHA256:20a4c84ba8348ed3839dd79fdafc230f7a0463a68f5af6a2b81b81ba33f77501
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.17.0.orig.tar.gz' libpsl_0.17.0.orig.tar.gz 49087 SHA256:7731e28393e1b4ca363eaffecd6c7570023a7c18c017b45d683ac7d2ba1f0bd1
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.17.0-3.debian.tar.xz' libpsl_0.17.0-3.debian.tar.xz 8516 SHA256:d0bd2abdaccadf2603f566e119b949a02523177199455e01c13a9c9deac1e6c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpsl/0.17.0-3/ (for browsing the source)
- https://sources.debian.net/src/libpsl/0.17.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpsl/0.17.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=2.6-3`

Binary Packages:

- `libselinux1:amd64=2.6-3+b3`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.6-3
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.6-3.dsc' libselinux_2.6-3.dsc 2217 SHA256:91bb53feba8031bfc7b0110fc4e0e1dae4a8e2906f4a524f83252a95ae0e639c
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.6.orig.tar.gz' libselinux_2.6.orig.tar.gz 203119 SHA256:4ea2dde50665c202253ba5caac7738370ea0337c47b251ba981c60d24e1a118a
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.6-3.debian.tar.xz' libselinux_2.6-3.debian.tar.xz 24396 SHA256:5a06841565e7907bc0dae9f8ed5940d040316192bd9662df59c79af7c212a171
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/2.6-3/ (for browsing the source)
- https://sources.debian.net/src/libselinux/2.6-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/2.6-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=2.6-2`

Binary Packages:

- `libsemanage-common=2.6-2`
- `libsemanage1:amd64=2.6-2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.6-2
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.6-2.dsc' libsemanage_2.6-2.dsc 2338 SHA256:2806bf3591dc7eb4c80d647a9e65df13d03657cfa6e049de1035165e0d8484d0
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.6.orig.tar.gz' libsemanage_2.6.orig.tar.gz 155897 SHA256:4f81541047290b751f2ffb926fcd381c186f22db18d9fe671b0b4a6a54e8cfce
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.6-2.debian.tar.xz' libsemanage_2.6-2.debian.tar.xz 17088 SHA256:3d1c4c5ea5d4f27a521b64ba3fc499c8b662257ffec773706501f466032db8cf
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/2.6-2/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/2.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/2.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=2.6-2`

Binary Packages:

- `libsepol1:amd64=2.6-2`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.6-2
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.6-2.dsc' libsepol_2.6-2.dsc 1814 SHA256:197ddaf44a5139d7ca6c12ce6b29fca0589f72c59ac588a7fa39d11b2e65778a
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.6.orig.tar.gz' libsepol_2.6.orig.tar.gz 442549 SHA256:d856d6506054f52abeaa3543ea2f2344595a3dc05d0d873ed7f724f7a16b1874
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.6-2.debian.tar.xz' libsepol_2.6-2.debian.tar.xz 14320 SHA256:d7a1022d03eb53a8d30262e06f14f691e553b3db684ca0f3549cd17b93fb7465
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/2.6-2/ (for browsing the source)
- https://sources.debian.net/src/libsepol/2.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/2.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libssh2=1.7.0-1+deb9u1`

Binary Packages:

- `libssh2-1:amd64=1.7.0-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.7.0-1+deb9u1
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.7.0-1+deb9u1.dsc' libssh2_1.7.0-1+deb9u1.dsc 2046 SHA256:dc4db042d18ecd49012df85a8de5b8dd3b512300688b0e9f527a4c505fabe5f1
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.7.0.orig.tar.gz' libssh2_1.7.0.orig.tar.gz 811714 SHA256:e4561fd43a50539a8c2ceb37841691baf03ecb7daf043766da1b112e4280d584
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.7.0-1+deb9u1.debian.tar.xz' libssh2_1.7.0-1+deb9u1.debian.tar.xz 13008 SHA256:e0291b5d7ff5a67abd318b923650569d2d4c112122a7b7b97cc3c563f10ae296
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.7.0-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.7.0-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.7.0-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.10-1.1+deb9u1`

Binary Packages:

- `libtasn1-6:amd64=4.10-1.1+deb9u1`
- `libtasn1-6-dev:amd64=4.10-1.1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`, `/usr/share/doc/libtasn1-6-dev/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.10-1.1+deb9u1
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.10-1.1+deb9u1.dsc' libtasn1-6_4.10-1.1+deb9u1.dsc 2614 SHA256:e9095d4d79e1015c2c2d3e8868d3c50f3b43510387a9ec9191d83ff57024fb39
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.10.orig.tar.gz' libtasn1-6_4.10.orig.tar.gz 1887057 SHA256:681a4d9a0d259f2125713f2e5766c5809f151b3a1392fd91390f780b4b8f5a02
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.10-1.1+deb9u1.debian.tar.xz' libtasn1-6_4.10-1.1+deb9u1.debian.tar.xz 59716 SHA256:fed5f50904fbfecc50d253aa4bc62221849e363430f71125039ada1512807937
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.10-1.1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.10-1.1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.10-1.1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=0.9.6+really0.9.3-0.1`

Binary Packages:

- `libunistring0:amd64=0.9.6+really0.9.3-0.1`

Licenses: (parsed from: `/usr/share/doc/libunistring0/copyright`)

- `GFDL-1.2`
- `GFDL-1.2+`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with exception`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libunistring=0.9.6+really0.9.3-0.1
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.6+really0.9.3-0.1.dsc' libunistring_0.9.6+really0.9.3-0.1.dsc 2109 SHA256:bf73a89a416333268ac9b457a06d1d92e5402c4f392187ad30e6146ffd3600ae
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.6+really0.9.3.orig.tar.gz' libunistring_0.9.6+really0.9.3.orig.tar.gz 2555215 SHA256:610d3ec724fbdaa654afe3cff20b9f4d504be3fd296fded2e0f7f764041006a3
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.6+really0.9.3-0.1.debian.tar.xz' libunistring_0.9.6+really0.9.3-0.1.debian.tar.xz 35372 SHA256:2d7636b16a56f1ad09748121a2181db4c2687fa83324c2f17bf451ee01b9de93
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/0.9.6+really0.9.3-0.1/ (for browsing the source)
- https://sources.debian.net/src/libunistring/0.9.6+really0.9.3-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/0.9.6+really0.9.3-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxml2=2.9.4+dfsg1-2.2+deb9u2`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-2.2+deb9u2`
- `libxml2-dev:amd64=2.9.4+dfsg1-2.2+deb9u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.4+dfsg1-2.2+deb9u2
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-2.2+deb9u2.dsc' libxml2_2.9.4+dfsg1-2.2+deb9u2.dsc 3049 SHA256:53d34e06270572861dd0cb59f99b35caa40f85f928151827f59686fc3642d6b1
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA256:a74ad55e346aa0b2b41903e66d21f8f3d2a736b3f41e32496376861ab484184e
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-2.2+deb9u2.debian.tar.xz' libxml2_2.9.4+dfsg1-2.2+deb9u2.debian.tar.xz 33996 SHA256:d178b2d7c9a3bfd929762e15b8f99a139a54a9bcf988820e4f4febb051090b62
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxml2/2.9.4+dfsg1-2.2+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/libxml2/2.9.4+dfsg1-2.2+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxml2/2.9.4+dfsg1-2.2+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxslt=1.1.29-2.1+deb9u1`

Binary Packages:

- `libxslt1-dev:amd64=1.1.29-2.1+deb9u1`
- `libxslt1.1:amd64=1.1.29-2.1+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxslt/1.1.29-2.1+deb9u1/


### `dpkg` source package: `libyaml=0.1.7-2`

Binary Packages:

- `libyaml-0-2:amd64=0.1.7-2`
- `libyaml-dev:amd64=0.1.7-2`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.1.7-2
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.1.7-2.dsc' libyaml_0.1.7-2.dsc 1820 SHA256:f2e599adcf8336c4be374987112a0c823b4609dc0f5a944e5827651241d91645
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.1.7.orig.tar.gz' libyaml_0.1.7.orig.tar.gz 527518 SHA256:8088e457264a98ba451a90b8661fcb4f9d6f478f7265d48322a196cec2480729
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.1.7-2.debian.tar.xz' libyaml_0.1.7-2.debian.tar.xz 4016 SHA256:6fc7065491dd6f86b46e6f231ae8ab60f8aafbef2dcf4721598644024485b801
```

Other potentially useful URLs:

- https://sources.debian.net/src/libyaml/0.1.7-2/ (for browsing the source)
- https://sources.debian.net/src/libyaml/0.1.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libyaml/0.1.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `linux=4.9.189-3+deb9u1`

Binary Packages:

- `linux-libc-dev:amd64=4.9.189-3+deb9u1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `CRYPTOGAMS`
- `GPL-2`
- `LGPL-2.1`
- `Unicode-data`
- `Xen-interface`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/linux/4.9.189-3+deb9u1/


### `dpkg` source package: `lsb=9.20161125`

Binary Packages:

- `lsb-base=9.20161125`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20161125
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_9.20161125.dsc' lsb_9.20161125.dsc 1697 SHA256:f2dd58084b1beabe966136cfd2e1b355002c1fb1635a6db5ef159b09ed94864f
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_9.20161125.tar.xz' lsb_9.20161125.tar.xz 43096 SHA256:0f9889ff1922da54d1f1538c11a57aa21dc5adf621e6201b18026f6633088bbd
```

Other potentially useful URLs:

- https://sources.debian.net/src/lsb/9.20161125/ (for browsing the source)
- https://sources.debian.net/src/lsb/9.20161125/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lsb/9.20161125/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lz4=0.0~r131-2`

Binary Packages:

- `liblz4-1:amd64=0.0~r131-2+b1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=0.0~r131-2
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_0.0~r131-2.dsc' lz4_0.0~r131-2.dsc 1973 SHA256:304cf9dddee387377929adf3f2cef0ae19fb2e56b6cc9eab05798845b58bd9b6
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_0.0~r131.orig.tar.gz' lz4_0.0~r131.orig.tar.gz 133784 SHA256:9d4d00614d6b9dec3114b33d1224b6262b99ace24434c53487a0c8fd0b18cfed
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_0.0~r131-2.debian.tar.xz' lz4_0.0~r131-2.debian.tar.xz 4936 SHA256:966df055dd8fa7f292c283452b43a5d2d2047d542fe49e97025006e69525e224
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/0.0~r131-2/ (for browsing the source)
- https://sources.debian.net/src/lz4/0.0~r131-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/0.0~r131-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mawk=1.3.3-17`

Binary Packages:

- `mawk=1.3.3-17+b3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.dsc' mawk_1.3.3-17.dsc 1801 SHA256:f98ce6e153e8ac1faf8165bbf77447a4279313f1c18f6bfeec0c5ce35e4b9c03
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.3-17.diff.gz' mawk_1.3.3-17.diff.gz 63506 SHA256:13cb66b6eb5ee654d5626621d5ef476ede6b0bebac18ce765516de810e58490c
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.3-17/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.3-17/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.3-17/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpclib3=1.0.3-1`

Binary Packages:

- `libmpc3:amd64=1.0.3-1+b2`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.0.3-1
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.0.3-1.dsc' mpclib3_1.0.3-1.dsc 1940 SHA256:4b424e1c6063d48fd0d045b5afe37004346dae267ced0994fa8e11ff41cada45
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.0.3.orig.tar.gz' mpclib3_1.0.3.orig.tar.gz 669925 SHA256:617decc6ea09889fb08ede330917a00b16809b8db88c29c31bfbb49cbf88ecc3
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.0.3-1.diff.gz' mpclib3_1.0.3-1.diff.gz 3684 SHA256:5a3fe9a7eddb4428d42e95f5919cce517f17411acdb2a73013a8f1a2bb246565
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpclib3/1.0.3-1/ (for browsing the source)
- https://sources.debian.net/src/mpclib3/1.0.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpclib3/1.0.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpfr4=3.1.5-1`

Binary Packages:

- `libmpfr4:amd64=3.1.5-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr4/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=3.1.5-1
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_3.1.5-1.dsc' mpfr4_3.1.5-1.dsc 1971 SHA256:40c1a87b1fc06ca9447f7fb1827fc13a0c557af8541f0bccbb3022b029b73582
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_3.1.5.orig.tar.xz' mpfr4_3.1.5.orig.tar.xz 1126668 SHA256:015fde82b3979fbe5f83501986d328331ba8ddf008c1ff3da3c238f49ca062bc
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_3.1.5-1.debian.tar.xz' mpfr4_3.1.5-1.debian.tar.xz 9672 SHA256:e5b0d755ec3b3aea15aab137328f7fe65c6b800a1b897bbf50fa4fd478589bd4
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpfr4/3.1.5-1/ (for browsing the source)
- https://sources.debian.net/src/mpfr4/3.1.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpfr4/3.1.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.0+20161126-1+deb9u2`

Binary Packages:

- `libncursesw5:amd64=6.0+20161126-1+deb9u2`
- `libtinfo5:amd64=6.0+20161126-1+deb9u2`
- `ncurses-base=6.0+20161126-1+deb9u2`
- `ncurses-bin=6.0+20161126-1+deb9u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.0+20161126-1+deb9u2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.0+20161126-1+deb9u2.dsc' ncurses_6.0+20161126-1+deb9u2.dsc 3784 SHA256:8cd721a065bea8275bf8daae9f01018b5fa2e9e020ac7c09fb61220804c9b9f5
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.0+20161126.orig.tar.gz' ncurses_6.0+20161126.orig.tar.gz 3192242 SHA256:e4b9cf1cfcf5a2db7df1d36402967783ba759246c8ff5a17a85ffd7e79296ec0
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.0+20161126-1+deb9u2.debian.tar.xz' ncurses_6.0+20161126-1+deb9u2.debian.tar.xz 59324 SHA256:04e6b5acf08d730c34f200ddb92144465ec346c0a3c1c2b9cbcd72ed9ddab1e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.0+20161126-1+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.0+20161126-1+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.0+20161126-1+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `netbase=5.4`

Binary Packages:

- `netbase=5.4`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.4
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.4.dsc' netbase_5.4.dsc 1326 SHA256:ebe29d45e65b661d64636cbce3840997d8079cf338efbfa347b4c73ed2831b7b
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.4.tar.xz' netbase_5.4.tar.xz 31524 SHA256:66ff73d2d162e2d49db43988d8b8cd328cf7fffca042db73397f14c71825e80d
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/5.4/ (for browsing the source)
- https://sources.debian.net/src/netbase/5.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/5.4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.3-1`

Binary Packages:

- `libhogweed4:amd64=3.3-1+b2`
- `libnettle6:amd64=3.3-1+b2`
- `nettle-dev=3.3-1+b2`

Licenses: (parsed from: `/usr/share/doc/libhogweed4/copyright`, `/usr/share/doc/libnettle6/copyright`, `/usr/share/doc/nettle-dev/copyright`)

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
$ apt-get source -qq --print-uris nettle=3.3-1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.3-1.dsc' nettle_3.3-1.dsc 2043 SHA256:3336bc6e8e5b1acad66afa97a05f934e4d758c614fd468d5650b5a38049f1161
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.3.orig.tar.gz' nettle_3.3.orig.tar.gz 1887927 SHA256:46942627d5d0ca11720fec18d81fc38f7ef837ea4197c1f630e71ce0d470b11e
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.3-1.debian.tar.xz' nettle_3.3-1.debian.tar.xz 19428 SHA256:42fef549318af6cfdf76336eb348501d09454a1d873a84f66440b9a791a0ff1b
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.3-1/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nghttp2=1.18.1-1+deb9u1`

Binary Packages:

- `libnghttp2-14:amd64=1.18.1-1+deb9u1`

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
$ apt-get source -qq --print-uris nghttp2=1.18.1-1+deb9u1
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.18.1-1+deb9u1.dsc' nghttp2_1.18.1-1+deb9u1.dsc 2657 SHA256:fc99fa8d124d322f7cd872c3088a268ea86f42e71229fc98d8a90869950d0a14
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.18.1.orig.tar.bz2' nghttp2_1.18.1.orig.tar.bz2 1780766 SHA256:5d8bb930eb90c552ec836c7b1862406b69cafcda5520bf266c8f5d914d9b447c
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.18.1-1+deb9u1.debian.tar.xz' nghttp2_1.18.1-1+deb9u1.debian.tar.xz 12300 SHA256:94cf473ee6a78181ebdddc18676df356fb788540cf426b7eca944573f2808733
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.18.1-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.18.1-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.18.1-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nspr=2:4.12-6`

Binary Packages:

- `libnspr4:amd64=2:4.12-6`
- `libnspr4-dev=2:4.12-6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.12-6
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12-6.dsc' nspr_4.12-6.dsc 2038 SHA256:c2b7b566e45ad153effa12b5e206bc213a215543aff01e29bc0f47c68162b160
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12.orig.tar.gz' nspr_4.12.orig.tar.gz 1135458 SHA256:e0b10a1e569153668ff8bdea6c7e491b389fab69c2f18285a1ebf7c2ea4269de
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12-6.debian.tar.xz' nspr_4.12-6.debian.tar.xz 15756 SHA256:02840f8938d7f6d6bd35f60d78ec804ba6318f8f390359e8fa6bb19ccb1060f7
```

Other potentially useful URLs:

- https://sources.debian.net/src/nspr/2:4.12-6/ (for browsing the source)
- https://sources.debian.net/src/nspr/2:4.12-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nspr/2:4.12-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nss=2:3.26.2-1.1+deb9u1`

Binary Packages:

- `libnss3:amd64=2:3.26.2-1.1+deb9u1`
- `libnss3-dev:amd64=2:3.26.2-1.1+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nss=2:3.26.2-1.1+deb9u1
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.26.2-1.1+deb9u1.dsc' nss_3.26.2-1.1+deb9u1.dsc 2428 SHA256:4b77f525bb3d67ddec4bf5f108d8fc7873191de997e0c0aec07c494425b089de
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.26.2.orig.tar.gz' nss_3.26.2.orig.tar.gz 7388390 SHA256:13a40a2f97edf5fab3d4c7fdd928e77df36dc539cd8354b6b5d79ab93a131a5a
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.26.2-1.1+deb9u1.debian.tar.xz' nss_3.26.2-1.1+deb9u1.debian.tar.xz 30820 SHA256:f87d64233afcbb25bf9253064a1508c3adf49f01ed6068d4968231d09ff0d87c
```

Other potentially useful URLs:

- https://sources.debian.net/src/nss/2:3.26.2-1.1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/nss/2:3.26.2-1.1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nss/2:3.26.2-1.1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.44+dfsg-5+deb9u3`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.44+dfsg-5+deb9u3`
- `libldap-common=2.4.44+dfsg-5+deb9u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openldap/2.4.44+dfsg-5+deb9u3/


### `dpkg` source package: `openssl=1.1.0l-1~deb9u1`

Binary Packages:

- `libssl-dev:amd64=1.1.0l-1~deb9u1`
- `libssl1.1:amd64=1.1.0l-1~deb9u1`
- `openssl=1.1.0l-1~deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.0l-1~deb9u1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0l-1~deb9u1.dsc' openssl_1.1.0l-1~deb9u1.dsc 2437 SHA256:9ae8fb3e89110ad3c75ba6a52b8f40cc5419b56f31c5c8b6f6aca0949cd90ea7
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0l.orig.tar.gz' openssl_1.1.0l.orig.tar.gz 5294857 SHA256:74a2f756c64fd7386a29184dc0344f4831192d61dc2481a93a4c5dd727f41148
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0l.orig.tar.gz.asc' openssl_1.1.0l.orig.tar.gz.asc 488 SHA256:afc83de9f9f1ef5f79ab8a31bbdeb26f9ac9a07cfdab7628a773267d31f85e42
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.0l-1~deb9u1.debian.tar.xz' openssl_1.1.0l-1~deb9u1.debian.tar.xz 72100 SHA256:78290d8a50219fe9c1c5676084a5567b23aff12f701bcd975e4c0d32264d5116
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.0l-1~deb9u1/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.0l-1~deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.0l-1~deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.3-2`

Binary Packages:

- `libp11-kit-dev:amd64=0.23.3-2`
- `libp11-kit0:amd64=0.23.3-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit-dev/copyright`, `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.3-2
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.3-2.dsc' p11-kit_0.23.3-2.dsc 2452 SHA256:fc8e87147d30de8d33e78adb805530d582655999762129b75097a9824679b0cc
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.3.orig.tar.gz' p11-kit_0.23.3.orig.tar.gz 1047441 SHA256:d487f04dba3f9e8256f53034c59c944ca45fd7b8434c095da6a74079644dcd82
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.3.orig.tar.gz.asc' p11-kit_0.23.3.orig.tar.gz.asc 543 SHA256:a9268313ad8e6c3dae5f4cf9006d8a773861e567c98786482304b3cc91883647
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.3-2.debian.tar.xz' p11-kit_0.23.3-2.debian.tar.xz 19784 SHA256:952f55f8c5e2cdc03c8388b59b0bd77bb53eb8f2c2ca2a686cfc91b52100e257
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.23.3-2/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.23.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.23.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.1.8-3.6`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.6`
- `libpam-modules-bin=1.1.8-3.6`
- `libpam-runtime=1.1.8-3.6`
- `libpam0g:amd64=1.1.8-3.6`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.6
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.6.dsc' pam_1.1.8-3.6.dsc 2572 SHA256:7bd7a3059c6ea5b97f5ce0460cbe20788f21bc59bd31ef5a28d7968f53373f5f
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8.orig.tar.gz' pam_1.1.8.orig.tar.gz 1892765 SHA256:4183409a450708a976eca5af561dbf4f0490141a08e86e4a1e649c7c1b094876
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.6.diff.gz' pam_1.1.8-3.6.diff.gz 139492 SHA256:beba99299941c5648ff412d75ebd3407e4d769f5e5ab1fce6a5f2e58c40341ae
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.1.8-3.6/ (for browsing the source)
- https://sources.debian.net/src/pam/1.1.8-3.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.1.8-3.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.39-3`

Binary Packages:

- `libpcre3:amd64=2:8.39-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-3
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-3.dsc' pcre3_8.39-3.dsc 2133 SHA256:3180a023c33b5eb7f0a853bec887be867d00a68da8d119d989909e40c6168fd7
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.39-3.debian.tar.gz' pcre3_8.39-3.debian.tar.gz 25025 SHA256:a9f0e1a96b6a017965fe69233e267682c289f2cfeb33b46fb78aedcb8cf2c16a
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre3/2:8.39-3/ (for browsing the source)
- https://sources.debian.net/src/pcre3/2:8.39-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre3/2:8.39-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.24.1-3+deb9u5`

Binary Packages:

- `libperl5.24:amd64=5.24.1-3+deb9u5`
- `perl=5.24.1-3+deb9u5`
- `perl-base=5.24.1-3+deb9u5`
- `perl-modules-5.24=5.24.1-3+deb9u5`

Licenses: (parsed from: `/usr/share/doc/libperl5.24/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.24/copyright`)

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
- `RRA-KEEP-THIS-NOTICE`
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.24.1-3+deb9u5
'http://security.debian.org/debian-security/pool/updates/main/p/perl/perl_5.24.1-3+deb9u5.dsc' perl_5.24.1-3+deb9u5.dsc 2393 SHA256:d30a446b21afb8f3c0da9bc117244646ef34a05c440a18bcd5c114ee87f8293f
'http://security.debian.org/debian-security/pool/updates/main/p/perl/perl_5.24.1.orig.tar.xz' perl_5.24.1.orig.tar.xz 11569284 SHA256:03a77bac4505c270f1890ece75afc7d4b555090b41aa41ea478747e23b2afb3f
'http://security.debian.org/debian-security/pool/updates/main/p/perl/perl_5.24.1-3+deb9u5.debian.tar.xz' perl_5.24.1-3+deb9u5.debian.tar.xz 185316 SHA256:fbb78d029b5a9a94e32feba2e360d3628a8a6de90066f90ff22e78d4918aab69
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.24.1-3+deb9u5/ (for browsing the source)
- https://sources.debian.net/src/perl/5.24.1-3+deb9u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.24.1-3+deb9u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pkg-config=0.29-4`

Binary Packages:

- `pkg-config=0.29-4+b1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29-4
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29-4.dsc' pkg-config_0.29-4.dsc 1718 SHA256:6a00ca4f4813c9d531b7f99072e1b6b443a8eea045c97e7d2b9d34f9a960deb5
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.orig.tar.gz' pkg-config_0.29.orig.tar.gz 1973875 SHA256:c8507705d2a10c67f385d66ca2aae31e81770cc0734b4191eb8c489e864a006b
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29-4.diff.gz' pkg-config_0.29-4.diff.gz 7560 SHA256:0c1253e3755942d3bf407d5c6465568e97ee960c8d9829c53cbae8ff26dc3762
```

Other potentially useful URLs:

- https://sources.debian.net/src/pkg-config/0.29-4/ (for browsing the source)
- https://sources.debian.net/src/pkg-config/0.29-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pkg-config/0.29-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `postgresql-9.6=9.6.15-0+deb9u1`

Binary Packages:

- `libpq-dev=9.6.15-0+deb9u1`
- `libpq5:amd64=9.6.15-0+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libpq-dev/copyright`, `/usr/share/doc/libpq5/copyright`)

- `Artistic`
- `BSD-2-clause`
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/postgresql-9.6/9.6.15-0+deb9u1/


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
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0-3.dsc' readline_7.0-3.dsc 2538 SHA256:f27a5dc9053b88641e3effc6c03b7840cbbbd887e8dcaf05d9e336c7bc7c6a53
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0.orig.tar.gz' readline_7.0.orig.tar.gz 2910016 SHA256:750d437185286f40a369e1e4f4764eda932b9459b5ec9a731628393dd3d32334
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0-3.debian.tar.xz' readline_7.0-3.debian.tar.xz 30012 SHA256:bf166310d6ca7716f2bd0e9e06cee2458b0157f7989d028730fc305643560175
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/7.0-3/ (for browsing the source)
- https://sources.debian.net/src/readline/7.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/7.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-1+b1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-1
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc 2315 SHA256:e56822b88625bf6a51f06652fc36fa2a1348b4325ac76541800cd078192aa3d2
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz 8044 SHA256:675847f5cddb860256cbf2e7d5b85918aa53b59b0fd97a466b39a5c77a399537
```

Other potentially useful URLs:

- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-1/ (for browsing the source)
- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rtmpdump/2.4+20151223.gitfa8646d.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.4-1`

Binary Packages:

- `sed=4.4-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.4-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.4-1.dsc' sed_4.4-1.dsc 2048 SHA256:bb2a11d04f3aeba73cc994e097219fde8c5e0fd1bcf42e0ecc8a4f2282c00fc9
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.4.orig.tar.xz' sed_4.4.orig.tar.xz 1181664 SHA256:cbd6ebc5aaf080ed60d0162d7f6aeae58211a1ee9ba9bb25623daa6cd942683b
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.4-1.debian.tar.xz' sed_4.4-1.debian.tar.xz 59552 SHA256:56dd1f91c5e33b419f38cde93afc90d6fad9064ef4594a877424a0ab2ac9a4bf
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.4-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sensible-utils=0.0.9+deb9u1`

Binary Packages:

- `sensible-utils=0.0.9+deb9u1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.9+deb9u1
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.9+deb9u1.dsc' sensible-utils_0.0.9+deb9u1.dsc 1590 SHA256:93641a0b5bb3b24b6f01daaf6d99cc1221678b150f19fc8a5c603cacdaecd6e2
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.9+deb9u1.tar.xz' sensible-utils_0.0.9+deb9u1.tar.xz 53564 SHA256:103a4666ddad53452b849d20c2509a6356d9aa6a60c515df9983bd0ca897a3db
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.9+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.9+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.9+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shadow=1:4.4-4.1`

Binary Packages:

- `login=1:4.4-4.1`
- `passwd=1:4.4-4.1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.4-4.1
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.4-4.1.dsc' shadow_4.4-4.1.dsc 2453 SHA256:6760f8ee90562ed02cb3902b81167e6153923a979c61dc06671426321e575f74
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.4.orig.tar.gz' shadow_4.4.orig.tar.gz 3003036 SHA256:1323e7e932836e03dbfa441f7eeb349ede2c92d62b788ade0732411fd516be3d
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.4-4.1.debian.tar.xz' shadow_4.4-4.1.debian.tar.xz 600560 SHA256:42610e666c762b88b9e60ea878b522b0639240dc9a74fe627b1ac497dd3d7424
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.4-4.1/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.4-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.4-4.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.16.2-5+deb9u1`

Binary Packages:

- `libsqlite3-0:amd64=3.16.2-5+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.16.2-5+deb9u1
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.16.2-5+deb9u1.dsc' sqlite3_3.16.2-5+deb9u1.dsc 2538 SHA256:aafd7c33e9091a0c8703a9b2dbfaf1b1592d8fc1df18bf92d3bfd2ffc350cc96
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.16.2.orig-www.tar.xz' sqlite3_3.16.2.orig-www.tar.xz 3383968 SHA256:d5dd3de405c55c63c9f99fbfcf3defc91a54a81b5656c510cd46544aaed134fa
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.16.2.orig.tar.xz' sqlite3_3.16.2.orig.tar.xz 5634120 SHA256:bf7b1e8ea7577253b7f8a8287d111d542d1792cf1768edc66541ac851ff92453
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.16.2-5+deb9u1.debian.tar.xz' sqlite3_3.16.2-5+deb9u1.debian.tar.xz 22128 SHA256:66358aca4f46ead86ba909bc5899bd312c10c46e620ad017120efe3b8714d44e
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.16.2-5+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.16.2-5+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.16.2-5+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=232-25+deb9u12`

Binary Packages:

- `libsystemd0:amd64=232-25+deb9u12`
- `libudev1:amd64=232-25+deb9u12`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=232-25+deb9u12
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_232-25+deb9u12.dsc' systemd_232-25+deb9u12.dsc 4801 SHA256:c280f20392fd51135a9cd5b03e8666545be05cc1fa73e4ed195f2002036a3cd7
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_232.orig.tar.gz' systemd_232.orig.tar.gz 4529048 SHA256:1172c7c7d5d72fbded53186e7599d5272231f04cc8b72f9a0fb2c5c20dfc4880
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_232-25+deb9u12.debian.tar.xz' systemd_232-25+deb9u12.debian.tar.xz 221868 SHA256:0fed4bffee2e7c2cdfac03f2b6fe8252aad96366edb783512c0d9bb7a40b8a6a
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/232-25+deb9u12/ (for browsing the source)
- https://sources.debian.net/src/systemd/232-25+deb9u12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/232-25+deb9u12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=2.88dsf-59.9`

Binary Packages:

- `sysvinit-utils=2.88dsf-59.9`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.9
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.9.dsc' sysvinit_2.88dsf-59.9.dsc 2123 SHA256:a943edeac16668d3e55583daa4033ad46469e84ffad014e0e2007d9c3167e63d
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.9.debian.tar.xz' sysvinit_2.88dsf-59.9.debian.tar.xz 132584 SHA256:fbd5c085680d896ec6ee1c5a55ae2d8a5a6b9fd5a7ec1e13010dace24fdbcd5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.88dsf-59.9/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.88dsf-59.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.88dsf-59.9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.29b-1.1`

Binary Packages:

- `tar=1.29b-1.1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.29b-1.1
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.29b-1.1.dsc' tar_1.29b-1.1.dsc 2057 SHA256:9474ed422017e23e8208785c071b9f7765d73d704b9bb19da22699c6581d73ef
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.29b.orig.tar.xz' tar_1.29b.orig.tar.xz 1822008 SHA256:6a59706ebee384a6cd2fb3ee1dbfbfc20c5c66c7efd7cedb28edc054fca8ba00
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.29b-1.1.debian.tar.xz' tar_1.29b-1.1.debian.tar.xz 28484 SHA256:380f80af0e87446796f05ba384c5d130ea2ad5978b8cfdcf315503966333ebb9
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.29b-1.1/ (for browsing the source)
- https://sources.debian.net/src/tar/1.29b-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.29b-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2019c-0+deb9u1`

Binary Packages:

- `tzdata=2019c-0+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tzdata/2019c-0+deb9u1/


### `dpkg` source package: `unbound=1.6.0-3+deb9u2`

Binary Packages:

- `libunbound2:amd64=1.6.0-3+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libunbound2/copyright`)

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
$ apt-get source -qq --print-uris unbound=1.6.0-3+deb9u2
'http://deb.debian.org/debian/pool/main/u/unbound/unbound_1.6.0-3+deb9u2.dsc' unbound_1.6.0-3+deb9u2.dsc 3049 SHA256:6a5da7fe8f00b7f7f1800112ceae9b52acebf6393a693bfa024170c9a29616dd
'http://deb.debian.org/debian/pool/main/u/unbound/unbound_1.6.0.orig.tar.gz' unbound_1.6.0.orig.tar.gz 5063253 SHA256:6b7db874e6debda742fee8869d722e5a17faf1086e93c911b8564532aeeffab7
'http://deb.debian.org/debian/pool/main/u/unbound/unbound_1.6.0-3+deb9u2.debian.tar.xz' unbound_1.6.0-3+deb9u2.debian.tar.xz 25084 SHA256:7051775537aca2e8f7ee6efaec30d71b5c86940064e265617abcef5fcc313f20
```

Other potentially useful URLs:

- https://sources.debian.net/src/unbound/1.6.0-3+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/unbound/1.6.0-3+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unbound/1.6.0-3+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ustr=1.0.4-6`

Binary Packages:

- `libustr-1.0-1:amd64=1.0.4-6`

Licenses: (parsed from: `/usr/share/doc/libustr-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris ustr=1.0.4-6
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4-6.dsc' ustr_1.0.4-6.dsc 2029 SHA256:87a854fc03dc059d5d4f135dfd36353c8c09f88a6eb216c6dcea8adadbe6ba59
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4.orig.tar.gz' ustr_1.0.4.orig.tar.gz 301345 SHA256:4d293b6b9d9fe51d58441f4b09b1f0005fcad8256ae8048587789bf5dbefb62e
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4-6.debian.tar.xz' ustr_1.0.4-6.debian.tar.xz 25608 SHA256:75aa6be2c70eba632ac63078e55ecb4b5a45e6624501a8ed6d81b9a2014d149e
```

Other potentially useful URLs:

- https://sources.debian.net/src/ustr/1.0.4-6/ (for browsing the source)
- https://sources.debian.net/src/ustr/1.0.4-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ustr/1.0.4-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.29.2-1+deb9u1`

Binary Packages:

- `bsdutils=1:2.29.2-1+deb9u1`
- `libblkid1:amd64=2.29.2-1+deb9u1`
- `libfdisk1:amd64=2.29.2-1+deb9u1`
- `libmount1:amd64=2.29.2-1+deb9u1`
- `libsmartcols1:amd64=2.29.2-1+deb9u1`
- `libuuid1:amd64=2.29.2-1+deb9u1`
- `mount=2.29.2-1+deb9u1`
- `util-linux=2.29.2-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.29.2-1+deb9u1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.29.2-1+deb9u1.dsc' util-linux_2.29.2-1+deb9u1.dsc 4101 SHA256:f84985e3b01d7758bf835484a5861d687ffee07778dadab5adc10a7e312da950
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.29.2.orig.tar.xz' util-linux_2.29.2.orig.tar.xz 4277668 SHA256:accea4d678209f97f634f40a93b7e9fcad5915d1f4749f6c47bee6bf110fe8e3
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.29.2-1+deb9u1.debian.tar.xz' util-linux_2.29.2-1+deb9u1.debian.tar.xz 74280 SHA256:33867c063f828a1937c1dd4797b3cd977a2e7da31eb1227c396f7dbf06dde3a6
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.29.2-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.29.2-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.29.2-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xmlsec1=1.2.23-0.1`

Binary Packages:

- `libxmlsec1=1.2.23-0.1`
- `libxmlsec1-dev=1.2.23-0.1`
- `libxmlsec1-gcrypt=1.2.23-0.1`
- `libxmlsec1-gnutls=1.2.23-0.1`
- `libxmlsec1-nss=1.2.23-0.1`
- `libxmlsec1-openssl=1.2.23-0.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xmlsec1=1.2.23-0.1
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.23-0.1.dsc' xmlsec1_1.2.23-0.1.dsc 2248 SHA256:f5674907250353af272e932bfc322f3fc4c59ea3a4394b7194aa3a5b81ec095c
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.23.orig.tar.gz' xmlsec1_1.2.23.orig.tar.gz 1794694 SHA256:41d463d16c9894cd3317098d027c038039c6d896b9cbb9bad9c4e29959e10e9f
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.23-0.1.debian.tar.xz' xmlsec1_1.2.23-0.1.debian.tar.xz 5996 SHA256:916e99122d181ba8011965026282aae1678f7c0bb6a37c144e77a20c8b1560c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/xmlsec1/1.2.23-0.1/ (for browsing the source)
- https://sources.debian.net/src/xmlsec1/1.2.23-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xmlsec1/1.2.23-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.2-1.2`

Binary Packages:

- `liblzma5:amd64=5.2.2-1.2+b1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.2-1.2
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2-1.2.dsc' xz-utils_5.2.2-1.2.dsc 2550 SHA256:13c8d8d0c243af78dc89b6e2cd670c8d8a2522379e1fcd196957c95d988d5961
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz' xz-utils_5.2.2.orig.tar.xz 1016404 SHA256:f341b1906ebcdde291dd619399ae944600edc9193619dd0c0110a5f05bfcc89e
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz.asc' xz-utils_5.2.2.orig.tar.xz.asc 543 SHA256:2cc0575556e1331b3f468e6e7dca5969ce86efcc315d62672279b4e68b2e449f
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.2-1.2.debian.tar.xz' xz-utils_5.2.2-1.2.debian.tar.xz 108632 SHA256:231c08d5c2c4e5c8ef5d6d58cac91aaeb2e4fcddc35e1ed3c69d730a2375c948
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.2-1.2/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.2-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.2-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.8.dfsg-5`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-5`
- `zlib1g-dev:amd64=1:1.2.8.dfsg-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.8.dfsg-5
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-5.dsc' zlib_1.2.8.dfsg-5.dsc 2259 SHA256:35ebfdbb74b3563d344b2bb946909f5d3221cdf971876549ea7ccec01fabcbec
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg.orig.tar.gz' zlib_1.2.8.dfsg.orig.tar.gz 361943 SHA256:2caecc2c3f1ef8b87b8f72b128a03e61c307e8c14f5ec9b422ef7914ba75cf9f
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-5.debian.tar.xz' zlib_1.2.8.dfsg-5.debian.tar.xz 18500 SHA256:7b88f58d1bfe8e873b8362ede3d0bc569793decc60094189fad1a110599cdd95
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-5/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.8.dfsg-5/ (for access to the source package after it no longer exists in the archive)
