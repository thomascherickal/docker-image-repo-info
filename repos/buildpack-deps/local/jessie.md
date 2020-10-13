# `buildpack-deps:jessie`

## Docker Metadata

- Image ID: `sha256:5aa202761897af59d0cafa1553ea926d345d33402e247f7da6ed022422311a1c`
- Created: `2020-10-13T02:22:41.857157626Z`
- Virtual Size: ~ 615.05 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-2`

Binary Packages:

- `acl=2.2.52-2`
- `libacl1:amd64=2.2.52-2`

Licenses: (parsed from: `/usr/share/doc/acl/copyright`, `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-2
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-2.dsc' acl_2.2.52-2.dsc 2025 SHA256:015097e04740e84fefbe6c890d02c603f79edece45c51cbb5c18431647cd7aad
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.52-2.debian.tar.xz' acl_2.2.52-2.debian.tar.xz 8524 SHA256:de81ec13cab6d33538db24a53c17838c5bdb32dd0e00e0b0b5d3325114e64e10
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.52-2/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.52-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.52-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.113+nmu3`

Binary Packages:

- `adduser=3.113+nmu3`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.113+nmu3
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.113+nmu3.dsc' adduser_3.113+nmu3.dsc 1733 SHA256:7f9fa8841080591834389fd56352e2d05ca3d86eb4df15d2f13bea9faf4a6f2d
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.113+nmu3.tar.gz' adduser_3.113+nmu3.tar.gz 342554 SHA256:02682be3f51f3e732121f20a3e4922bb8bef15cfacb8767fc250a01d09502122
```

Other potentially useful URLs:

- https://sources.debian.net/src/adduser/3.113+nmu3/ (for browsing the source)
- https://sources.debian.net/src/adduser/3.113+nmu3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adduser/3.113+nmu3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr-util=1.5.4-1`

Binary Packages:

- `libaprutil1:amd64=1.5.4-1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.5.4-1
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.5.4-1.dsc' apr-util_1.5.4-1.dsc 2610 SHA256:4bef658a072d22814a7548b90d114f5ca85a053594789fb2af97fec5993afa5a
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.5.4.orig.tar.bz2' apr-util_1.5.4.orig.tar.bz2 694427 SHA256:a6cf327189ca0df2fb9d5633d7326c460fe2b61684745fd7963e79a6dd0dc82e
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.5.4-1.debian.tar.xz' apr-util_1.5.4-1.debian.tar.xz 16452 SHA256:83b625e3c3b7093562e31413c858ff586a245cc4c99e348844dd891d40112741
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr-util/1.5.4-1/ (for browsing the source)
- https://sources.debian.net/src/apr-util/1.5.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr-util/1.5.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr=1.5.1-3`

Binary Packages:

- `libapr1:amd64=1.5.1-3`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.5.1-3
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.1-3.dsc' apr_1.5.1-3.dsc 2090 SHA256:f3f78ab76365a17a233220357eb2b7f3102d7e9d21c59b3f82d9f0300c554433
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.1.orig.tar.bz2' apr_1.5.1.orig.tar.bz2 817569 SHA256:e94abe431d4da48425fcccdb27b469bd0f8151488f82e5630a56f26590e198ac
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.1-3.debian.tar.xz' apr_1.5.1-3.debian.tar.xz 17844 SHA256:c7f270ab445e2646bd7dfdfaf9ea44b2642a43c48012689c6f3bf52fe8c9e9c5
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.5.1-3/ (for browsing the source)
- https://sources.debian.net/src/apr/1.5.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.5.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=1.0.9.8.6`

Binary Packages:

- `apt=1.0.9.8.6`
- `libapt-pkg4.12:amd64=1.0.9.8.6`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg4.12/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.0.9.8.6
'http://security.debian.org/debian-security/pool/updates/main/a/apt/apt_1.0.9.8.6.dsc' apt_1.0.9.8.6.dsc 2396 SHA256:252f09e9a52a1470e1d38a98d313a7fe5e1737c775946f3348d0e10251d3ccfd
'http://security.debian.org/debian-security/pool/updates/main/a/apt/apt_1.0.9.8.6.tar.xz' apt_1.0.9.8.6.tar.xz 1784448 SHA256:b1a430b0d2b54008f1cdc2b58e48a94bcc259f5b0c95cfa5450f00f5aa14e283
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/1.0.9.8.6/ (for browsing the source)
- https://sources.debian.net/src/apt/1.0.9.8.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/1.0.9.8.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `attr=1:2.4.47-2`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2`

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

### `dpkg` source package: `audit=1:2.4-1`

Binary Packages:

- `libaudit-common=1:2.4-1`
- `libaudit1:amd64=1:2.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.4-1
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.4-1.dsc' audit_2.4-1.dsc 2068 SHA256:01d240bd783697b8ab4cd941f944612eebc81e1f535a8afb36b25ab3021cd15f
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.4.orig.tar.gz' audit_2.4.orig.tar.gz 937809 SHA256:6e5d39e7af9d00477ef60f824be8c93bd23a227869d6993ff36b7e7fa28fe99b
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.4-1.debian.tar.xz' audit_2.4-1.debian.tar.xz 15808 SHA256:c18c1b88c41f3b8be9e59d3041563599f822994cb10574ffc17f00f0a157c12c
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:2.4-1/ (for browsing the source)
- https://sources.debian.net/src/audit/1:2.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:2.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `autoconf=2.69-8`

Binary Packages:

- `autoconf=2.69-8`

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
$ apt-get source -qq --print-uris autoconf=2.69-8
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-8.dsc' autoconf_2.69-8.dsc 1961 SHA256:cdf9c0f1959925e1f80746eac03dea2e95c2b7a12b1d14c78134e7ea813ca9ad
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-8.debian.tar.xz' autoconf_2.69-8.debian.tar.xz 21220 SHA256:5ae055184f30a0c54523cf88e44aca6efdb772f02ed83991fc39b56a39ebe3f1
```

Other potentially useful URLs:

- https://sources.debian.net/src/autoconf/2.69-8/ (for browsing the source)
- https://sources.debian.net/src/autoconf/2.69-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autoconf/2.69-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `automake-1.14=1:1.14.1-4+deb8u1`

Binary Packages:

- `automake=1:1.14.1-4+deb8u1`

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
$ apt-get source -qq --print-uris automake-1.14=1:1.14.1-4+deb8u1
'http://deb.debian.org/debian/pool/main/a/automake-1.14/automake-1.14_1.14.1-4+deb8u1.dsc' automake-1.14_1.14.1-4+deb8u1.dsc 2280 SHA256:f1d22a310c137d2e45119a170d6e28db88a3e051c45c3b4fa2ba1aabbd7b2b13
'http://deb.debian.org/debian/pool/main/a/automake-1.14/automake-1.14_1.14.1.orig.tar.xz' automake-1.14_1.14.1.orig.tar.xz 1488984 SHA256:a9b4f04b8b69cac2e832a38a718943aa976dbdad0097211f8b3448afdacf0669
'http://deb.debian.org/debian/pool/main/a/automake-1.14/automake-1.14_1.14.1-4+deb8u1.debian.tar.xz' automake-1.14_1.14.1-4+deb8u1.debian.tar.xz 12640 SHA256:9938ab32632e2e78b2b9a4adce710287db29356ee593c1bca9df4d43e874f119
```

Other potentially useful URLs:

- https://sources.debian.net/src/automake-1.14/1:1.14.1-4+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/automake-1.14/1:1.14.1-4+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/automake-1.14/1:1.14.1-4+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `autotools-dev=20140911.1`

Binary Packages:

- `autotools-dev=20140911.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20140911.1
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20140911.1.dsc' autotools-dev_20140911.1.dsc 1312 SHA256:93531ae9bda81f4abc834d16f156aa036817ca8147ec77345b95da44f2b16e2f
'http://deb.debian.org/debian/pool/main/a/autotools-dev/autotools-dev_20140911.1.tar.xz' autotools-dev_20140911.1.tar.xz 60344 SHA256:b4b907bc7f87e00acbbd6a6cf148c23c3ce585fd639cc2bdc9c91f6c33d2b587
```

Other potentially useful URLs:

- https://sources.debian.net/src/autotools-dev/20140911.1/ (for browsing the source)
- https://sources.debian.net/src/autotools-dev/20140911.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autotools-dev/20140911.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=8+deb8u11`

Binary Packages:

- `base-files=8+deb8u11`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=8+deb8u11
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_8+deb8u11.dsc' base-files_8+deb8u11.dsc 1030 SHA256:15eb9515f3d06e1cd09e23f8b6263ad5355d07f3bf6e3631ede2bf850235e2cd
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_8+deb8u11.tar.xz' base-files_8+deb8u11.tar.xz 53192 SHA256:361b53e18719b4a37ff5a0e2544ab238b412c2a75b7d63f8500c958590230e64
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/8+deb8u11/ (for browsing the source)
- https://sources.debian.net/src/base-files/8+deb8u11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/8+deb8u11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.37`

Binary Packages:

- `base-passwd=3.5.37`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.37
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.37.dsc' base-passwd_3.5.37.dsc 1733 SHA256:211a49b6a3bbfdb61a91e9b5d9994c59d8a511a047c2cfc489c03c4c379d6cfe
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.37.tar.xz' base-passwd_3.5.37.tar.xz 51392 SHA256:7cb1cdd8e4aee39b5f59a3dc42d63619590fc4a2136db482fdb6be6e74bb3d04
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.37/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.37/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.37/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=4.3-11+deb8u2`

Binary Packages:

- `bash=4.3-11+deb8u2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.3-11+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/b/bash/bash_4.3-11+deb8u2.dsc' bash_4.3-11+deb8u2.dsc 2222 SHA256:281ad9ae160e98fc77e5bcb8538a002d5673ac44ba0ea98afc00e46467247756
'http://security.debian.org/debian-security/pool/updates/main/b/bash/bash_4.3.orig.tar.gz' bash_4.3.orig.tar.gz 7516231 SHA256:b2fe79ddf9e7abdb4695e3070afa866d2a94a58d1cc9d731585330c753815491
'http://security.debian.org/debian-security/pool/updates/main/b/bash/bash_4.3-11+deb8u2.debian.tar.xz' bash_4.3-11+deb8u2.debian.tar.xz 80512 SHA256:5d4a93a98944179aea4ce7a66a8db6e7981ff795137c00a51724596b57e3faeb
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/4.3-11+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/bash/4.3-11+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/4.3-11+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `binutils=2.25-5+deb8u1`

Binary Packages:

- `binutils=2.25-5+deb8u1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.25-5+deb8u1
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.25-5+deb8u1.dsc' binutils_2.25-5+deb8u1.dsc 2394 SHA256:a64dfe3d58408a03842aa96a68d14216847c34f6363f5622d3277caf0359f7ae
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.25.orig.tar.gz' binutils_2.25.orig.tar.gz 34179370 SHA256:a608164c4858bfe42fcac4639c341482ba6207118dadeca624fdfabf39cd7281
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.25-5+deb8u1.diff.gz' binutils_2.25-5+deb8u1.diff.gz 146765 SHA256:6c46154ae2ef9e8d8933bc546192caac9f37d4bf36a2b2d154da97b336589b39
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.25-5+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.25-5+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.25-5+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.6-7+deb8u2`

Binary Packages:

- `bzip2=1.0.6-7+deb8u2`
- `libbz2-1.0:amd64=1.0.6-7+deb8u2`
- `libbz2-dev:amd64=1.0.6-7+deb8u2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-7+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/b/bzip2/bzip2_1.0.6-7+deb8u2.dsc' bzip2_1.0.6-7+deb8u2.dsc 2462 SHA256:7f1f29e1c032ca64068eb0aa7b9e025b0c9e41218974d8fff3d255397fc691f5
'http://security.debian.org/debian-security/pool/updates/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://security.debian.org/debian-security/pool/updates/main/b/bzip2/bzip2_1.0.6-7+deb8u2.debian.tar.bz2' bzip2_1.0.6-7+deb8u2.debian.tar.bz2 61298 SHA256:49b18ae614a6a92beaf846ae2d5df29687c6d09a158f57db548ff52b882f51b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.6-7+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.6-7+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.6-7+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzr=2.6.0+bzr6595-6+deb8u1`

Binary Packages:

- `bzr=2.6.0+bzr6595-6+deb8u1`
- `python-bzrlib=2.6.0+bzr6595-6+deb8u1`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`, `/usr/share/doc/python-bzrlib/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.6.0+bzr6595-6+deb8u1
'http://deb.debian.org/debian/pool/main/b/bzr/bzr_2.6.0+bzr6595-6+deb8u1.dsc' bzr_2.6.0+bzr6595-6+deb8u1.dsc 2914 SHA256:ebe83be4c7036e4f90f0a8ebeab997768fa47f835db5fa8f4de9d880b5c5f251
'http://deb.debian.org/debian/pool/main/b/bzr/bzr_2.6.0+bzr6595.orig.tar.gz' bzr_2.6.0+bzr6595.orig.tar.gz 10944820 SHA256:0016ae484fa08afad9c13ba83871ab424ff0151dee30064af9dd355ec65bdcec
'http://deb.debian.org/debian/pool/main/b/bzr/bzr_2.6.0+bzr6595-6+deb8u1.debian.tar.xz' bzr_2.6.0+bzr6595-6+deb8u1.debian.tar.xz 64608 SHA256:58861deceaa2c9c6e3046b2a705b8150b217dc719e1aaa3e5e26113e291957f3
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzr/2.6.0+bzr6595-6+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/bzr/2.6.0+bzr6595-6+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzr/2.6.0+bzr6595-6+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20141019+deb8u4`

Binary Packages:

- `ca-certificates=20141019+deb8u4`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20141019+deb8u4
'http://security.debian.org/debian-security/pool/updates/main/c/ca-certificates/ca-certificates_20141019+deb8u4.dsc' ca-certificates_20141019+deb8u4.dsc 1754 SHA256:4f2bec1a926ff2be32571ef25fddaaf3656cfe28a040efa96ffc493194930b43
'http://security.debian.org/debian-security/pool/updates/main/c/ca-certificates/ca-certificates_20141019+deb8u4.tar.xz' ca-certificates_20141019+deb8u4.tar.xz 248648 SHA256:12af9462236667ee617e34a4befb447bb9519dceefc76190a62bc16343f27650
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20141019+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20141019+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20141019+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cairo=1.14.0-2.1+deb8u2`

Binary Packages:

- `libcairo-gobject2:amd64=1.14.0-2.1+deb8u2`
- `libcairo-script-interpreter2:amd64=1.14.0-2.1+deb8u2`
- `libcairo2:amd64=1.14.0-2.1+deb8u2`
- `libcairo2-dev=1.14.0-2.1+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.14.0-2.1+deb8u2
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.0-2.1+deb8u2.dsc' cairo_1.14.0-2.1+deb8u2.dsc 3069 SHA256:c5440748278b608bf060193a7515222cc9e1967f3fec7585219f1b5278a229d5
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.0.orig.tar.xz' cairo_1.14.0.orig.tar.xz 36584076 SHA256:2cf5f81432e77ea4359af9dcd0f4faf37d015934501391c311bfd2d19a0134b7
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.0-2.1+deb8u2.debian.tar.xz' cairo_1.14.0-2.1+deb8u2.debian.tar.xz 31872 SHA256:66f6a5f01b351b0ba53fbbb146d6fb5ac46146bf0a974016d0f318a387f17abf
```

Other potentially useful URLs:

- https://sources.debian.net/src/cairo/1.14.0-2.1+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/cairo/1.14.0-2.1+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cairo/1.14.0-2.1+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.192`

Binary Packages:

- `libdebconfclient0:amd64=0.192`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.192
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.192.dsc' cdebconf_0.192.dsc 2574 SHA256:85d39068de77c67036b6e2ca5ebdf3990e19a6c5b0f01422608ff7656c166dbd
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.192.tar.xz' cdebconf_0.192.tar.xz 266320 SHA256:bb09e6c04b514dd12684dbc6eacde57fb03e282f67f0199e67078c13ffffd667
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.192/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.192/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.192/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cloog=0.18.2-1`

Binary Packages:

- `libcloog-isl4:amd64=0.18.2-1+b2`

Licenses: (parsed from: `/usr/share/doc/libcloog-isl4/copyright`)

- `GFDL`
- `GPL`
- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cloog=0.18.2-1
'http://deb.debian.org/debian/pool/main/c/cloog/cloog_0.18.2-1.dsc' cloog_0.18.2-1.dsc 1299 SHA256:a7a186409b4436bc4202c01f6fca47380916176d18fc457805469596c151fd6e
'http://deb.debian.org/debian/pool/main/c/cloog/cloog_0.18.2.orig.tar.gz' cloog_0.18.2.orig.tar.gz 2376691 SHA256:ba3cc2d3750dfcb51f65ce029f0dda31347b8eeed216b1bac6170ab12d967581
'http://deb.debian.org/debian/pool/main/c/cloog/cloog_0.18.2-1.debian.tar.xz' cloog_0.18.2-1.debian.tar.xz 7824 SHA256:45cb83d37782fc705aac74942b8adfaa22680089f5b5537f0539daec89c08438
```

Other potentially useful URLs:

- https://sources.debian.net/src/cloog/0.18.2-1/ (for browsing the source)
- https://sources.debian.net/src/cloog/0.18.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cloog/0.18.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `configobj=5.0.6-1`

Binary Packages:

- `python-configobj=5.0.6-1`

Licenses: (parsed from: `/usr/share/doc/python-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-1
'http://deb.debian.org/debian/pool/main/c/configobj/configobj_5.0.6-1.dsc' configobj_5.0.6-1.dsc 2379 SHA256:82ddde99df9549259a3eb607b8d89b58416952ace18d611d14100928166aeb8c
'http://deb.debian.org/debian/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA256:2e140354efcca6f558ff9ee941b435ae09a617bc071797bef62c8d6ed2033d5e
'http://deb.debian.org/debian/pool/main/c/configobj/configobj_5.0.6-1.debian.tar.xz' configobj_5.0.6-1.debian.tar.xz 7396 SHA256:027c425f9153b034957ce5a2db2fc9dc8839cc4bafb7da62cd29c07317855cab
```

Other potentially useful URLs:

- https://sources.debian.net/src/configobj/5.0.6-1/ (for browsing the source)
- https://sources.debian.net/src/configobj/5.0.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/configobj/5.0.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.23-4`

Binary Packages:

- `coreutils=8.23-4`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.23-4
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.23-4.dsc' coreutils_8.23-4.dsc 1942 SHA256:280ace2d2f1740c2319338e96da6b5000b9e65ddb9549c772917123633afe772
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.23.orig.tar.gz' coreutils_8.23.orig.tar.gz 12582141 SHA256:d606551dccd8c4ed079d7aa8d74af152b1d16215cae763d86b40b26fdbde9c73
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_8.23-4.diff.gz' coreutils_8.23-4.diff.gz 48759 SHA256:19ab6ff1b82f29e8a8f8107f925eec91b1eaad53b690f2d7154ab07101bf8c01
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/8.23-4/ (for browsing the source)
- https://sources.debian.net/src/coreutils/8.23-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/8.23-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cryptsetup=2:1.6.6-5`

Binary Packages:

- `libcryptsetup4:amd64=2:1.6.6-5`

Licenses: (parsed from: `/usr/share/doc/libcryptsetup4/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cryptsetup=2:1.6.6-5
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.6.6-5.dsc' cryptsetup_1.6.6-5.dsc 2624 SHA256:f7582c8becb38fecaed22aa531bd748dee2ebdbdac64e00c7e39e45afe7eaae1
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.6.6.orig.tar.xz' cryptsetup_1.6.6.orig.tar.xz 1145940 SHA256:2d2ce28e4e1137dd599d87884b62ef6dbf14fd7848b2a2bf7d61cf125fbd8e6f
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.6.6-5.debian.tar.xz' cryptsetup_1.6.6-5.debian.tar.xz 82944 SHA256:fa12da2f5448e0b02e1e5c89357de3749f854b2b96441f9c56737766c11cded0
```

Other potentially useful URLs:

- https://sources.debian.net/src/cryptsetup/2:1.6.6-5/ (for browsing the source)
- https://sources.debian.net/src/cryptsetup/2:1.6.6-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cryptsetup/2:1.6.6-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.38.0-4+deb8u16`

Binary Packages:

- `curl=7.38.0-4+deb8u16`
- `libcurl3:amd64=7.38.0-4+deb8u16`
- `libcurl3-gnutls:amd64=7.38.0-4+deb8u16`
- `libcurl4-openssl-dev:amd64=7.38.0-4+deb8u16`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`

Source:

```console
$ apt-get source -qq --print-uris curl=7.38.0-4+deb8u16
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.38.0-4+deb8u16.dsc' curl_7.38.0-4+deb8u16.dsc 2673 SHA256:3db130cd472eca668fca688a05abc4015e21bb2c71a31dd7922a7e20f28a0f9d
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.38.0.orig.tar.gz' curl_7.38.0.orig.tar.gz 4094034 SHA256:5661028aa6532882fa228cd23c99ddbb8b87643dbb1a7ea55c068d34a943dff1
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.38.0-4+deb8u16.debian.tar.xz' curl_7.38.0-4+deb8u16.debian.tar.xz 57984 SHA256:2952dba7f69e877ad1d03e3cb41458b52cf7a000226a24be3938c3152136ccc2
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.38.0-4+deb8u16/ (for browsing the source)
- https://sources.debian.net/src/curl/7.38.0-4+deb8u16/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.38.0-4+deb8u16/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.26.dfsg1-13+deb8u2`

Binary Packages:

- `libsasl2-2:amd64=2.1.26.dfsg1-13+deb8u2`
- `libsasl2-modules-db:amd64=2.1.26.dfsg1-13+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.26.dfsg1-13+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-13+deb8u2.dsc' cyrus-sasl2_2.1.26.dfsg1-13+deb8u2.dsc 3374 SHA256:fbffac72f4f1a2a89a7efe5c140a2c462d24461bdc86f520ba1f2f8d3e706dee
'http://security.debian.org/debian-security/pool/updates/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz' cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz 1494337 SHA256:172c39555012f479543ce7305949db75df708771fe8f8b34248027f09e53bb85
'http://security.debian.org/debian-security/pool/updates/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-13+deb8u2.debian.tar.xz' cyrus-sasl2_2.1.26.dfsg1-13+deb8u2.debian.tar.xz 94624 SHA256:65ae9250eb6f49bbec2fdc64390f016d4e3b00e51a6b9a90d85604cb805d4cf3
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.26.dfsg1-13+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.26.dfsg1-13+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.26.dfsg1-13+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.7-4`

Binary Packages:

- `dash=0.5.7-4+b1`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.7-4
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.7-4.dsc' dash_0.5.7-4.dsc 1105 SHA256:c77f4baef8cbdc105a783bf6e4d3253ae10671ad98c27bf8537c8c731f073310
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.7.orig.tar.gz' dash_0.5.7.orig.tar.gz 223794 SHA256:ae89fa9f1145b7748cf0740e1df04cd52fdf8a285da4911dd0f04983efba4e39
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.7-4.diff.gz' dash_0.5.7-4.diff.gz 42834 SHA256:649d97aa0c48dc0db73c08d7e89a004b9d413279a823388161940342016284f0
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.7-4/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.7-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.7-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db-defaults=5.3.0`

Binary Packages:

- `libdb-dev:amd64=5.3.0+b1`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=5.3.0
'http://deb.debian.org/debian/pool/main/d/db-defaults/db-defaults_5.3.0.dsc' db-defaults_5.3.0.dsc 1229 SHA256:ecf0c453ff92425ab15fc8a81c591e7ca512b410b202acc6c72c8a2c068476e8
'http://deb.debian.org/debian/pool/main/d/db-defaults/db-defaults_5.3.0.tar.gz' db-defaults_5.3.0.tar.gz 2869 SHA256:2fa889708084e694718141760e620ba2a4bb2988d5511b0342a63a8daf6adcb9
```

Other potentially useful URLs:

- https://sources.debian.net/src/db-defaults/5.3.0/ (for browsing the source)
- https://sources.debian.net/src/db-defaults/5.3.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db-defaults/5.3.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28-9+deb8u1`

Binary Packages:

- `libdb5.3:amd64=5.3.28-9+deb8u1`
- `libdb5.3-dev=5.3.28-9+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-9+deb8u1
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-9+deb8u1.dsc' db5.3_5.3.28-9+deb8u1.dsc 3233 SHA256:48ce55c383ff32df4fb5a205de982f6edfa483c007bc45711d9066ced2365ec2
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28-9+deb8u1.debian.tar.xz' db5.3_5.3.28-9+deb8u1.debian.tar.xz 28416 SHA256:b44fcf3ad7fe36f4513d50bb648b2f408f1b7682fe44ef84a18ccbe74934d9cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28-9+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28-9+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28-9+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.56+deb8u1`

Binary Packages:

- `debconf=1.5.56+deb8u1`
- `debconf-i18n=1.5.56+deb8u1`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`, `/usr/share/doc/debconf-i18n/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.56+deb8u1
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.56+deb8u1.dsc' debconf_1.5.56+deb8u1.dsc 1941 SHA256:d10cef7aafd28153cd6edd2721bfb70ccd0120cdb9766eecb6d51d7035d79843
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.56+deb8u1.tar.gz' debconf_1.5.56+deb8u1.tar.gz 1004750 SHA256:936f79533fe79a87b86cfb1b16d69c39a8dc586cdaa07e2b4b3b0e28917aec4a
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.56+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.56+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.56+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debian-archive-keyring=2017.5~deb8u1`

Binary Packages:

- `debian-archive-keyring=2017.5~deb8u1`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2017.5~deb8u1
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.5~deb8u1.dsc' debian-archive-keyring_2017.5~deb8u1.dsc 1639 SHA256:d03d8d53a0e20a4155a95d6fcea2a4c4773f2852025d6b2aee38be7a5818937e
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2017.5~deb8u1.tar.xz' debian-archive-keyring_2017.5~deb8u1.tar.xz 79444 SHA256:9db751cf3479351a2d60ff5fc6b59e0b780bc2cffc94103f0e02b0b12a25245b
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2017.5~deb8u1/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2017.5~deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2017.5~deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=4.4`

Binary Packages:

- `debianutils=4.4+b1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.4
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.4.dsc' debianutils_4.4.dsc 1560 SHA256:e365ad42af528f46eb117ef244216aaf265372f2b92635b28452a8f0d981bb17
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.4.tar.gz' debianutils_4.4.tar.gz 272098 SHA256:190850cdd6b5302e0a1ba1aaed1bc7074d67d3bd8d04c613f242f7145afa53a6
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.4/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.3-1`

Binary Packages:

- `diffutils=1:3.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.3-1
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.3-1.dsc' diffutils_3.3-1.dsc 1427 SHA256:72df1fed003b47509a063dfa8aa89108c884cd3bf52a06ce40e1ffb61f5a256c
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.3.orig.tar.xz' diffutils_3.3.orig.tar.xz 1197832 SHA256:a25e89a8ab65fded1731e4186be1bb25cda967834b6df973599cdcd5abdfc19c
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.3-1.debian.tar.gz' diffutils_3.3-1.debian.tar.gz 10584 SHA256:23765ea43cd1b4e5e504ce0984a16e27d5c01e9272cba489ebbebd217f227fc7
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.3-1/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `djvulibre=3.5.25.4-4+deb8u2`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.25.4-4+deb8u2`
- `libdjvulibre-text=3.5.25.4-4+deb8u2`
- `libdjvulibre21:amd64=3.5.25.4-4+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.25.4-4+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/d/djvulibre/djvulibre_3.5.25.4-4+deb8u2.dsc' djvulibre_3.5.25.4-4+deb8u2.dsc 2487 SHA256:30a1aaa4896e9c0b042c6f34024e20b77e33f709848e8020c09ef3de542a0299
'http://security.debian.org/debian-security/pool/updates/main/d/djvulibre/djvulibre_3.5.25.4.orig.tar.gz' djvulibre_3.5.25.4.orig.tar.gz 3575460 SHA256:6d8b3414d8ec87c5a40d3dde6fee54beebee6cbf6ec56aa7851dfbca9aaa3f36
'http://security.debian.org/debian-security/pool/updates/main/d/djvulibre/djvulibre_3.5.25.4-4+deb8u2.debian.tar.xz' djvulibre_3.5.25.4-4+deb8u2.debian.tar.xz 84264 SHA256:5c3b67bdb1e16245e5f32107d7ea8a8c63616b2d6dbcace571b6cbcfbcfa2195
```

Other potentially useful URLs:

- https://sources.debian.net/src/djvulibre/3.5.25.4-4+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/djvulibre/3.5.25.4-4+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/djvulibre/3.5.25.4-4+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.17.27`

Binary Packages:

- `dpkg=1.17.27`
- `dpkg-dev=1.17.27`
- `libdpkg-perl=1.17.27`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.17.27
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.17.27.dsc' dpkg_1.17.27.dsc 2018 SHA256:730ad9445990322551acf79a752515d27ffca5c8b6d978b3276d28e88d60e34f
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.17.27.tar.xz' dpkg_1.17.27.tar.xz 4413092 SHA256:90749c31b9f1fceb46dd9fab5b50de34272efef333cc16d9e144f514fd944bb6
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.17.27/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.17.27/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.17.27/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.42.12-2+deb8u2`

Binary Packages:

- `comerr-dev=2.1-1.42.12-2+deb8u2`
- `e2fslibs:amd64=1.42.12-2+deb8u2`
- `e2fsprogs=1.42.12-2+deb8u2`
- `libcomerr2:amd64=1.42.12-2+deb8u2`
- `libss2:amd64=1.42.12-2+deb8u2`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.42.12-2+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.42.12-2+deb8u2.dsc' e2fsprogs_1.42.12-2+deb8u2.dsc 2747 SHA256:fb5ac1998defa86a99046f08f537a7ec22a41fc30401a7e28117107af3a2aea6
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.42.12.orig.tar.gz' e2fsprogs_1.42.12.orig.tar.gz 6381695 SHA256:e17846d91a0edd89fa59b064bde8f8e5cec5851e35f587bcccb4014dbd63186c
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.42.12-2+deb8u2.debian.tar.xz' e2fsprogs_1.42.12-2+deb8u2.debian.tar.xz 71488 SHA256:a86df6f1b0734b42b79f0a06da52667666c73c79f394c66f9a4450e505f34848
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.42.12-2+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.42.12-2+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.42.12-2+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.1.0-6+deb8u6`

Binary Packages:

- `libexpat1:amd64=2.1.0-6+deb8u6`
- `libexpat1-dev:amd64=2.1.0-6+deb8u6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.1.0-6+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/e/expat/expat_2.1.0-6+deb8u6.dsc' expat_2.1.0-6+deb8u6.dsc 2292 SHA256:b54613edbbacde7b879be9d21b5d711c2cb2c90ed3d5e0968bdaf4c55bbcd8be
'http://security.debian.org/debian-security/pool/updates/main/e/expat/expat_2.1.0.orig.tar.gz' expat_2.1.0.orig.tar.gz 562616 SHA256:823705472f816df21c8f6aa026dd162b280806838bb55b3432b0fb1fcca7eb86
'http://security.debian.org/debian-security/pool/updates/main/e/expat/expat_2.1.0-6+deb8u6.debian.tar.xz' expat_2.1.0-6+deb8u6.debian.tar.xz 23672 SHA256:7d61123e76076598e3026fff5570ccdfbb90a540a1fdd310e13224b28e52c24a
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.1.0-6+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/expat/2.1.0-6+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.1.0-6+deb8u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `explorercanvas=0.r3-3`

Binary Packages:

- `libjs-excanvas=0.r3-3`

Licenses: (parsed from: `/usr/share/doc/libjs-excanvas/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris explorercanvas=0.r3-3
'http://deb.debian.org/debian/pool/main/e/explorercanvas/explorercanvas_0.r3-3.dsc' explorercanvas_0.r3-3.dsc 1969 SHA256:bbbd16706f59fe553ec666ac8f0fc804ba2869f0f1a56f7a7cc6428bc48414fa
'http://deb.debian.org/debian/pool/main/e/explorercanvas/explorercanvas_0.r3.orig.tar.gz' explorercanvas_0.r3.orig.tar.gz 50748 SHA256:687af8084781b8eb3451fc55c88f6dfddc2b84428d197daf2c4c33fd5c55fed8
'http://deb.debian.org/debian/pool/main/e/explorercanvas/explorercanvas_0.r3-3.debian.tar.gz' explorercanvas_0.r3-3.debian.tar.gz 1918 SHA256:78275294c9edb87bed4be5ad2883a9e971fab8095ce4fb306dbba64eba7afc66
```

Other potentially useful URLs:

- https://sources.debian.net/src/explorercanvas/0.r3-3/ (for browsing the source)
- https://sources.debian.net/src/explorercanvas/0.r3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/explorercanvas/0.r3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fftw3=3.3.4-2`

Binary Packages:

- `libfftw3-double3:amd64=3.3.4-2`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.4-2
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.4-2.dsc' fftw3_3.3.4-2.dsc 2860 SHA256:56e65d2b02fc7dae23a76eb082aee6ea3cdb6613897ed7f5f777beb462eaaf2b
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.4.orig.tar.gz' fftw3_3.3.4.orig.tar.gz 3940427 SHA256:8f0cde90929bc05587c3368d2f15cd0530a60b8a9912a8e2979a72dbe5af0982
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.4-2.debian.tar.xz' fftw3_3.3.4-2.debian.tar.xz 12568 SHA256:788fe6fdf0a0070436e14407ed0065e65876f46a935b24bed0c9753f07887e7e
```

Other potentially useful URLs:

- https://sources.debian.net/src/fftw3/3.3.4-2/ (for browsing the source)
- https://sources.debian.net/src/fftw3/3.3.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fftw3/3.3.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `file=1:5.22+15-2+deb8u7`

Binary Packages:

- `file=1:5.22+15-2+deb8u7`
- `libmagic1:amd64=1:5.22+15-2+deb8u7`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.22+15-2+deb8u7
'http://security.debian.org/debian-security/pool/updates/main/f/file/file_5.22+15-2+deb8u7.dsc' file_5.22+15-2+deb8u7.dsc 2096 SHA256:7e5f2b4e061ba0d0ed19b24a2dd828ddc1aa0ba119892deac3269b1996c3cbd6
'http://security.debian.org/debian-security/pool/updates/main/f/file/file_5.22+15.orig.tar.xz' file_5.22+15.orig.tar.xz 569332 SHA256:c021e9f73b3eb3b6cc2532c5d9a77af1a92902935013c2740ba3fef83f1804d2
'http://security.debian.org/debian-security/pool/updates/main/f/file/file_5.22+15-2+deb8u7.debian.tar.xz' file_5.22+15-2+deb8u7.debian.tar.xz 32588 SHA256:2d7ce2cf8a78e782bb59ff3ad54ebfe8ec1f931b77ceb9e48f19c8fc69cbd4aa
```

Other potentially useful URLs:

- https://sources.debian.net/src/file/1:5.22+15-2+deb8u7/ (for browsing the source)
- https://sources.debian.net/src/file/1:5.22+15-2+deb8u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/file/1:5.22+15-2+deb8u7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.4.2-9`

Binary Packages:

- `findutils=4.4.2-9+b1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.2`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.4.2-9
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.4.2-9.dsc' findutils_4.4.2-9.dsc 1996 SHA256:0dd9d96af8260d2e81c5819d2e5536f95cb894e771c9adcab44ba70726adb13e
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.4.2.orig.tar.gz' findutils_4.4.2.orig.tar.gz 2149838 SHA256:434f32d171cbc0a5e72cfc5372c6fc4cb0e681f8dce566a0de5b6fccd702b62a
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.4.2-9.debian.tar.xz' findutils_4.4.2-9.debian.tar.xz 27384 SHA256:8a9f5fb20c255b833994d7dfff1999b3f4f95dea6008495f2b0ef6c549d62c34
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.4.2-9/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.4.2-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.4.2-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fontconfig=2.11.0-6.3+deb8u1`

Binary Packages:

- `fontconfig=2.11.0-6.3+deb8u1`
- `fontconfig-config=2.11.0-6.3+deb8u1`
- `libfontconfig1:amd64=2.11.0-6.3+deb8u1`
- `libfontconfig1-dev:amd64=2.11.0-6.3+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.11.0-6.3+deb8u1
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0-6.3+deb8u1.dsc' fontconfig_2.11.0-6.3+deb8u1.dsc 2235 SHA256:c496170e75ece48a19c5b60745eef5522b62ae1a817c23125ebd9745bc255fcd
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0.orig.tar.xz' fontconfig_2.11.0.orig.tar.xz 319652 SHA256:f19c7366d59dc4e79eaf3eedabd44b6375b238f29316db5020a183c7d9a78db9
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0-6.3+deb8u1.debian.tar.xz' fontconfig_2.11.0-6.3+deb8u1.debian.tar.xz 1073796 SHA256:a8140c4576a2c43614930e8a307966018551ae71ad448af5f75faf4f47f70173
```

Other potentially useful URLs:

- https://sources.debian.net/src/fontconfig/2.11.0-6.3+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/fontconfig/2.11.0-6.3+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fontconfig/2.11.0-6.3+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fonts-dejavu=2.34-1`

Binary Packages:

- `fonts-dejavu-core=2.34-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.34-1
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.34-1.dsc' fonts-dejavu_2.34-1.dsc 2484 SHA256:843b22fff349667b83f66cf3ab2e93a187ff016f4bd90fbfbe9001bf82a9d66d
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.34.orig.tar.bz2' fonts-dejavu_2.34.orig.tar.bz2 11329547 SHA256:b5ca9e671635a9fe04c791cdc82c707ba57380c2cc8de3f92451a039134b9027
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.34-1.debian.tar.gz' fonts-dejavu_2.34-1.debian.tar.gz 11231 SHA256:46044164bdc385037a1694a07e8c5a1c183511cb68743914219ebb93750dac19
```

Other potentially useful URLs:

- https://sources.debian.net/src/fonts-dejavu/2.34-1/ (for browsing the source)
- https://sources.debian.net/src/fonts-dejavu/2.34-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fonts-dejavu/2.34-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `freetype=2.5.2-3+deb8u4`

Binary Packages:

- `libfreetype6:amd64=2.5.2-3+deb8u4`
- `libfreetype6-dev=2.5.2-3+deb8u4`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

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
$ apt-get source -qq --print-uris freetype=2.5.2-3+deb8u4
'http://security.debian.org/debian-security/pool/updates/main/f/freetype/freetype_2.5.2-3+deb8u4.dsc' freetype_2.5.2-3+deb8u4.dsc 1783 SHA256:ba32ac993642ed5e1712b064b6072f0f67c95c01eafcaa3d5a1d63b2c03c9e5d
'http://security.debian.org/debian-security/pool/updates/main/f/freetype/freetype_2.5.2.orig.tar.gz' freetype_2.5.2.orig.tar.gz 1971155 SHA256:5fda4996e43cfdf9b602a0eb5abde014f1a3c3b2d82bbb9b86942011c63f5c3a
'http://security.debian.org/debian-security/pool/updates/main/f/freetype/freetype_2.5.2-3+deb8u4.diff.gz' freetype_2.5.2-3+deb8u4.diff.gz 72104 SHA256:9160b5c1069c763e2b3b55a8e825fa46f054764bf37d8d2d4df3b003859b7e21
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.5.2-3+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.5.2-3+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.5.2-3+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-4.8=4.8.4-1`

Binary Packages:

- `gcc-4.8-base:amd64=4.8.4-1`

Licenses: (parsed from: `/usr/share/doc/gcc-4.8-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-4.8=4.8.4-1
'http://deb.debian.org/debian/pool/main/g/gcc-4.8/gcc-4.8_4.8.4-1.dsc' gcc-4.8_4.8.4-1.dsc 10638 SHA256:9ba284727055aba04bb3122ef7f857587a403a5c9a2f924948829da49ca2ef02
'http://deb.debian.org/debian/pool/main/g/gcc-4.8/gcc-4.8_4.8.4-1.tar.gz' gcc-4.8_4.8.4-1.tar.gz 187653934 SHA256:c38d9687b6fef3010f250adaf89a3f1bd0f12c9cd82ed531a52e7d394b8226cf
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-4.8/4.8.4-1/ (for browsing the source)
- https://sources.debian.net/src/gcc-4.8/4.8.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-4.8/4.8.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-4.9=4.9.2-10+deb8u2`

Binary Packages:

- `cpp-4.9=4.9.2-10+deb8u2`
- `g++-4.9=4.9.2-10+deb8u2`
- `gcc-4.9=4.9.2-10+deb8u2`
- `gcc-4.9-base:amd64=4.9.2-10+deb8u2`
- `libasan1:amd64=4.9.2-10+deb8u2`
- `libatomic1:amd64=4.9.2-10+deb8u2`
- `libcilkrts5:amd64=4.9.2-10+deb8u2`
- `libgcc-4.9-dev:amd64=4.9.2-10+deb8u2`
- `libgcc1:amd64=1:4.9.2-10+deb8u2`
- `libgomp1:amd64=4.9.2-10+deb8u2`
- `libitm1:amd64=4.9.2-10+deb8u2`
- `liblsan0:amd64=4.9.2-10+deb8u2`
- `libquadmath0:amd64=4.9.2-10+deb8u2`
- `libstdc++-4.9-dev:amd64=4.9.2-10+deb8u2`
- `libstdc++6:amd64=4.9.2-10+deb8u2`
- `libtsan0:amd64=4.9.2-10+deb8u2`
- `libubsan0:amd64=4.9.2-10+deb8u2`

Licenses: (parsed from: `/usr/share/doc/cpp-4.9/copyright`, `/usr/share/doc/g++-4.9/copyright`, `/usr/share/doc/gcc-4.9/copyright`, `/usr/share/doc/gcc-4.9-base/copyright`, `/usr/share/doc/libasan1/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-4.9-dev/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-4.9-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-4.9=4.9.2-10+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/g/gcc-4.9/gcc-4.9_4.9.2-10+deb8u2.dsc' gcc-4.9_4.9.2-10+deb8u2.dsc 19264 SHA256:900b6da5b21d5e15e1cb14ea6f17f56c85bbb82394ad6f091b98b05a6246961e
'http://security.debian.org/debian-security/pool/updates/main/g/gcc-4.9/gcc-4.9_4.9.2.orig.tar.gz' gcc-4.9_4.9.2.orig.tar.gz 73565212 SHA256:861aa811d5f9e9ecf32d8195d2346fc434eba7e17330878ed3d876c49a32ec4e
'http://security.debian.org/debian-security/pool/updates/main/g/gcc-4.9/gcc-4.9_4.9.2-10+deb8u2.diff.gz' gcc-4.9_4.9.2-10+deb8u2.diff.gz 883134 SHA256:bd151e4ec61e40a96a49dc4a8275da688380ffd9668670b3cfe78c622e3812ae
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-4.9/4.9.2-10+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/gcc-4.9/4.9.2-10+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-4.9/4.9.2-10+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-defaults=1.136`

Binary Packages:

- `cpp=4:4.9.2-2`
- `g++=4:4.9.2-2`
- `gcc=4:4.9.2-2`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.136
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.136.dsc' gcc-defaults_1.136.dsc 3255 SHA256:5ac9089c83ce76445a7b3dcb546460e85352bce22fa0ce26fc26c1a8812d484a
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.136.tar.gz' gcc-defaults_1.136.tar.gz 64341 SHA256:7146bd9f988928c0c9e765677d9997edec7bd23472306dbec9be54bdaa21e558
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-defaults/1.136/ (for browsing the source)
- https://sources.debian.net/src/gcc-defaults/1.136/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-defaults/1.136/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.8.3-13.1`

Binary Packages:

- `libgdbm-dev=1.8.3-13.1`
- `libgdbm3:amd64=1.8.3-13.1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.8.3-13.1
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3-13.1.dsc' gdbm_1.8.3-13.1.dsc 1830 SHA256:b1d8bef30edc491315c337930cbe2b61f44f55035adfc26ae945bab5ca57d5c9
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3.orig.tar.bz2' gdbm_1.8.3.orig.tar.bz2 172796 SHA256:1d5995b6e9e6be4ff62c8126d019f184a083dd8e6f75f6c74b9fe023b5b9440e
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.8.3-13.1.debian.tar.xz' gdbm_1.8.3-13.1.debian.tar.xz 14748 SHA256:251401e1f5210226f384e936b1b7ea1df40119a918d9f3dbf48b2e51d4df8983
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.8.3-13.1/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.8.3-13.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.8.3-13.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdk-pixbuf=2.31.1-2+deb8u9`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0=2.31.1-2+deb8u9`
- `libgdk-pixbuf2.0-0:amd64=2.31.1-2+deb8u9`
- `libgdk-pixbuf2.0-common=2.31.1-2+deb8u9`
- `libgdk-pixbuf2.0-dev=2.31.1-2+deb8u9`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.31.1-2+deb8u9
'http://security.debian.org/debian-security/pool/updates/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1-2+deb8u9.dsc' gdk-pixbuf_2.31.1-2+deb8u9.dsc 2998 SHA256:01cde50802a78812acff087ed30c71f3d00f4baa5d8bcd137b1dcea6b1c9d728
'http://security.debian.org/debian-security/pool/updates/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1.orig.tar.xz' gdk-pixbuf_2.31.1.orig.tar.xz 1340056 SHA256:25a75e3c61dac11e6ff6416ad846951ccafac6486b1c6a1bfb0b213b99db52cd
'http://security.debian.org/debian-security/pool/updates/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1-2+deb8u9.debian.tar.xz' gdk-pixbuf_2.31.1-2+deb8u9.debian.tar.xz 22912 SHA256:f9987018d9e309a62bc1b3211e4afdc407a7bc903f6067ed8e12a172920bd630
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdk-pixbuf/2.31.1-2+deb8u9/ (for browsing the source)
- https://sources.debian.net/src/gdk-pixbuf/2.31.1-2+deb8u9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdk-pixbuf/2.31.1-2+deb8u9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.1.4-2.1+deb8u10`

Binary Packages:

- `git=1:2.1.4-2.1+deb8u10`
- `git-man=1:2.1.4-2.1+deb8u10`

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
$ apt-get source -qq --print-uris git=1:2.1.4-2.1+deb8u10
'http://security.debian.org/debian-security/pool/updates/main/g/git/git_2.1.4-2.1+deb8u10.dsc' git_2.1.4-2.1+deb8u10.dsc 2821 SHA256:0f3e537b9001411e940fd6ba60dc4e04c3227b5ff455b3e5b53b7e6959faa484
'http://security.debian.org/debian-security/pool/updates/main/g/git/git_2.1.4.orig.tar.xz' git_2.1.4.orig.tar.xz 3544804 SHA256:a04968b9b10cbcb31a7054aa3a0d11ac47c83556ecd270ddef1987df5d3d053e
'http://security.debian.org/debian-security/pool/updates/main/g/git/git_2.1.4-2.1+deb8u10.debian.tar.xz' git_2.1.4-2.1+deb8u10.debian.tar.xz 534760 SHA256:16620383020360e4bbc94d7d012ea89d44c5823e62e1724e5f730b57b398ec13
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.1.4-2.1+deb8u10/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.1.4-2.1+deb8u10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.1.4-2.1+deb8u10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.42.1-1+deb8u3`

Binary Packages:

- `libglib2.0-0:amd64=2.42.1-1+deb8u3`
- `libglib2.0-bin=2.42.1-1+deb8u3`
- `libglib2.0-data=2.42.1-1+deb8u3`
- `libglib2.0-dev=2.42.1-1+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.42.1-1+deb8u3
'http://security.debian.org/debian-security/pool/updates/main/g/glib2.0/glib2.0_2.42.1-1+deb8u3.dsc' glib2.0_2.42.1-1+deb8u3.dsc 3190 SHA256:264c7a3c38289154d104d5f1a8bb1fc7b527ed55801db871b18d5f1d0ce78617
'http://security.debian.org/debian-security/pool/updates/main/g/glib2.0/glib2.0_2.42.1.orig.tar.xz' glib2.0_2.42.1.orig.tar.xz 6985120 SHA256:8f3f0865280e45b8ce840e176ef83bcfd511148918cc8d39df2ee89b67dcf89a
'http://security.debian.org/debian-security/pool/updates/main/g/glib2.0/glib2.0_2.42.1-1+deb8u3.debian.tar.xz' glib2.0_2.42.1-1+deb8u3.debian.tar.xz 71104 SHA256:c1f4e14d8c5640838203e680ff9f2a547464a42e927a9525fabea0ae722b2113
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.42.1-1+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.42.1-1+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.42.1-1+deb8u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.19-18+deb8u10`

Binary Packages:

- `libc-bin=2.19-18+deb8u10`
- `libc-dev-bin=2.19-18+deb8u10`
- `libc6:amd64=2.19-18+deb8u10`
- `libc6-dev:amd64=2.19-18+deb8u10`
- `multiarch-support=2.19-18+deb8u10`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.19-18+deb8u10
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.19-18+deb8u10.dsc' glibc_2.19-18+deb8u10.dsc 8256 SHA256:cfc796163f67f367f0f59f89e4cdcf59f3f77d14a4cfdad1c870c8c2feafde0b
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.19.orig.tar.xz' glibc_2.19.orig.tar.xz 12387008 SHA256:746e52bb4fc9b2f30bcd33d415172a40ab56c5fff6c494052d31b0795593cc60
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.19-18+deb8u10.debian.tar.xz' glibc_2.19-18+deb8u10.debian.tar.xz 1059340 SHA256:b5110a37901189fc092748592b117fb10684b9c92a876ea64d4030ffa00d01c1
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.19-18+deb8u10/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.19-18+deb8u10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.19-18+deb8u10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.0.0+dfsg-6`

Binary Packages:

- `libgmp-dev:amd64=2:6.0.0+dfsg-6`
- `libgmp10:amd64=2:6.0.0+dfsg-6`
- `libgmpxx4ldbl:amd64=2:6.0.0+dfsg-6`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.0.0+dfsg-6
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.0.0+dfsg-6.dsc' gmp_6.0.0+dfsg-6.dsc 1840 SHA256:40f44bfae4ed9df69a8c64fe9bf9deded10cc4a75844c95bbfbfc3307976f53a
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.0.0+dfsg.orig.tar.xz' gmp_6.0.0+dfsg.orig.tar.xz 1756792 SHA256:7539e094815fc321f4dc64b0a6968db9e1bee85a459bc64d4cc2b9dd0f6729a5
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.0.0+dfsg-6.debian.tar.xz' gmp_6.0.0+dfsg-6.debian.tar.xz 21024 SHA256:83219073eab9fb886dd1123b6b571b45fbe2f7c290c4201b07696784ffcf7fd1
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.0.0+dfsg-6/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.0.0+dfsg-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.0.0+dfsg-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg=1.4.18-7+deb8u5`

Binary Packages:

- `gnupg=1.4.18-7+deb8u5`
- `gpgv=1.4.18-7+deb8u5`

Licenses: (parsed from: `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gpgv/copyright`)

- `GPL-3`
- `GPL-3+ with OpenSSL exception`
- `RFC-Reference`

Source:

```console
$ apt-get source -qq --print-uris gnupg=1.4.18-7+deb8u5
'http://deb.debian.org/debian/pool/main/g/gnupg/gnupg_1.4.18-7+deb8u5.dsc' gnupg_1.4.18-7+deb8u5.dsc 2591 SHA256:63cb3c6d7ee52b38bee3ade03c8d0ef4befd1d3bf56129bd11d260ac46e22f8b
'http://deb.debian.org/debian/pool/main/g/gnupg/gnupg_1.4.18.orig.tar.gz' gnupg_1.4.18.orig.tar.gz 5047888 SHA256:10a8936b76ccadb98521535b5f41cc5b41b3c159a6c2915f062bd4dc8ac12d12
'http://deb.debian.org/debian/pool/main/g/gnupg/gnupg_1.4.18-7+deb8u5.debian.tar.xz' gnupg_1.4.18-7+deb8u5.debian.tar.xz 305056 SHA256:6e63f0543ca283511c0be22c87ac802c34819808f1a4e17fc7fce75b11a22c90
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg/1.4.18-7+deb8u5/ (for browsing the source)
- https://sources.debian.net/src/gnupg/1.4.18-7+deb8u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg/1.4.18-7+deb8u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.3.30-0+deb8u1`

Binary Packages:

- `libgnutls-deb0-28:amd64=3.3.30-0+deb8u1`
- `libgnutls-openssl27:amd64=3.3.30-0+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgnutls-deb0-28/copyright`, `/usr/share/doc/libgnutls-openssl27/copyright`)

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
$ apt-get source -qq --print-uris gnutls28=3.3.30-0+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/g/gnutls28/gnutls28_3.3.30-0+deb8u1.dsc' gnutls28_3.3.30-0+deb8u1.dsc 2628 SHA256:01be8c173d3ffbe984b5dddb3ada3f6e984e1219daf9d9af14c0512b965a3dbb
'http://security.debian.org/debian-security/pool/updates/main/g/gnutls28/gnutls28_3.3.30.orig.tar.xz' gnutls28_3.3.30.orig.tar.xz 6392748 SHA256:41d70107ead3de2f12390909a05eefc9a88def6cd1f0d90ea82a7dac8b8effee
'http://security.debian.org/debian-security/pool/updates/main/g/gnutls28/gnutls28_3.3.30-0+deb8u1.debian.tar.xz' gnutls28_3.3.30-0+deb8u1.debian.tar.xz 46352 SHA256:f3055451c76ba5c805f558b676bc5b83fbbc5cce9332d2fc0bece2c180165d6f
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.3.30-0+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.3.30-0+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.3.30-0+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gobject-introspection=1.42.0-2.2`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.42.0-2.2`
- `gir1.2-glib-2.0:amd64=1.42.0-2.2`
- `libgirepository-1.0-1:amd64=1.42.0-2.2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.42.0-2.2
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.42.0-2.2.dsc' gobject-introspection_1.42.0-2.2.dsc 2856 SHA256:93ea9071f61d4b2280fb20f306eac3c64b4cd4272492e38655d2c451f9c86e4a
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.42.0.orig.tar.xz' gobject-introspection_1.42.0.orig.tar.xz 1308056 SHA256:3ba2edfad4f71d4f0de16960b5d5f2511335fa646b2c49bbb93ce5942b3f95f7
'http://deb.debian.org/debian/pool/main/g/gobject-introspection/gobject-introspection_1.42.0-2.2.debian.tar.xz' gobject-introspection_1.42.0-2.2.debian.tar.xz 19868 SHA256:e529aa1de821dc37805ddfecd9c2032662c43a5f55510f854fa9c4e0fb45dc86
```

Other potentially useful URLs:

- https://sources.debian.net/src/gobject-introspection/1.42.0-2.2/ (for browsing the source)
- https://sources.debian.net/src/gobject-introspection/1.42.0-2.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gobject-introspection/1.42.0-2.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `graphite2=1.3.10-1~deb8u1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.10-1~deb8u1`

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
$ apt-get source -qq --print-uris graphite2=1.3.10-1~deb8u1
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.10-1~deb8u1.dsc' graphite2_1.3.10-1~deb8u1.dsc 2232 SHA256:546b58d828f20103703029a74b70a2b81b27ecbeb7130cee89acf02c16cda075
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.10.orig.tar.gz' graphite2_1.3.10.orig.tar.gz 3889647 SHA256:90fde3b2f9ea95d68ffb19278d07d9b8a7efa5ba0e413bebcea802ce05cda1ae
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.10-1~deb8u1.debian.tar.xz' graphite2_1.3.10-1~deb8u1.debian.tar.xz 10448 SHA256:8aedda28f1a77a16fe9a0cd0245332af588db636341eb97891dadddf43739d15
```

Other potentially useful URLs:

- https://sources.debian.net/src/graphite2/1.3.10-1~deb8u1/ (for browsing the source)
- https://sources.debian.net/src/graphite2/1.3.10-1~deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/graphite2/1.3.10-1~deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `graphviz=2.38.0-7`

Binary Packages:

- `libcdt5=2.38.0-7`
- `libcgraph6=2.38.0-7`
- `libgraphviz-dev=2.38.0-7`
- `libgvc6=2.38.0-7`
- `libgvpr2=2.38.0-7`
- `libpathplan4=2.38.0-7`
- `libxdot4=2.38.0-7`

Licenses: (parsed from: `/usr/share/doc/libcdt5/copyright`, `/usr/share/doc/libcgraph6/copyright`, `/usr/share/doc/libgraphviz-dev/copyright`, `/usr/share/doc/libgvc6/copyright`, `/usr/share/doc/libgvpr2/copyright`, `/usr/share/doc/libpathplan4/copyright`, `/usr/share/doc/libxdot4/copyright`)

- `GPL-2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris graphviz=2.38.0-7
'http://deb.debian.org/debian/pool/main/g/graphviz/graphviz_2.38.0-7.dsc' graphviz_2.38.0-7.dsc 3266 SHA256:62883ac0dd3915c6cf67cda5cadd8c6423314c004bd791b781618d8743674bdc
'http://deb.debian.org/debian/pool/main/g/graphviz/graphviz_2.38.0.orig.tar.gz' graphviz_2.38.0.orig.tar.gz 25848858 SHA256:81aa238d9d4a010afa73a9d2a704fc3221c731e1e06577c2ab3496bdef67859e
'http://deb.debian.org/debian/pool/main/g/graphviz/graphviz_2.38.0-7.debian.tar.xz' graphviz_2.38.0-7.debian.tar.xz 44120 SHA256:312ab8215fbe1800664675cfc284aecfeff3ce699407523b5bdefee64cf1a53c
```

Other potentially useful URLs:

- https://sources.debian.net/src/graphviz/2.38.0-7/ (for browsing the source)
- https://sources.debian.net/src/graphviz/2.38.0-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/graphviz/2.38.0-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=2.20-4.1`

Binary Packages:

- `grep=2.20-4.1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=2.20-4.1
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.20-4.1.dsc' grep_2.20-4.1.dsc 2627 SHA256:62ae6c19839e940462d27b2a234e925210cdb9209e2a4080b695fcec439c1d04
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.20.orig.tar.xz' grep_2.20.orig.tar.xz 1237196 SHA256:f0af452bc0d09464b6d089b6d56a0a3c16672e9ed9118fbe37b0b6aeaf069a65
'http://deb.debian.org/debian/pool/main/g/grep/grep_2.20-4.1.debian.tar.bz2' grep_2.20-4.1.debian.tar.bz2 113054 SHA256:4aa8c4487d05dc82498668deeb485a9d4891a74df29466adf74e2faf738d2917
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/2.20-4.1/ (for browsing the source)
- https://sources.debian.net/src/grep/2.20-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/2.20-4.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.6-4`

Binary Packages:

- `gzip=1.6-4`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-4
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-4.dsc' gzip_1.6-4.dsc 1853 SHA256:9605bb67aa336e3f1dd68429fa713a80dff3439d67f944160895b14c98503147
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.6-4.debian.tar.xz' gzip_1.6-4.debian.tar.xz 14476 SHA256:20a474283cc0063de7db623ccc3b17da7df6bc15f681de4e9e1da12b990a2743
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.6-4/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.6-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.6-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `harfbuzz=0.9.35-2+deb8u1`

Binary Packages:

- `libharfbuzz0b:amd64=0.9.35-2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=0.9.35-2+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/h/harfbuzz/harfbuzz_0.9.35-2+deb8u1.dsc' harfbuzz_0.9.35-2+deb8u1.dsc 2850 SHA256:8b96ed6020b9a9ea9a7e6143528e7281369a2f0fb8722e45c4892edd86d6c54e
'http://security.debian.org/debian-security/pool/updates/main/h/harfbuzz/harfbuzz_0.9.35.orig.tar.bz2' harfbuzz_0.9.35.orig.tar.bz2 1165359 SHA256:0aa1a8aba6f502321cf6fef3c9d2c73dde48389c5ed1d3615a7691944c2a06ed
'http://security.debian.org/debian-security/pool/updates/main/h/harfbuzz/harfbuzz_0.9.35-2+deb8u1.debian.tar.xz' harfbuzz_0.9.35-2+deb8u1.debian.tar.xz 7872 SHA256:02915188c2e048db3eb12b152a8809c07099d35b9367f790c53afc5013c4cf97
```

Other potentially useful URLs:

- https://sources.debian.net/src/harfbuzz/0.9.35-2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/harfbuzz/0.9.35-2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/harfbuzz/0.9.35-2+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hicolor-icon-theme=0.13-1`

Binary Packages:

- `hicolor-icon-theme=0.13-1`

Licenses: (parsed from: `/usr/share/doc/hicolor-icon-theme/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris hicolor-icon-theme=0.13-1
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.13-1.dsc' hicolor-icon-theme_0.13-1.dsc 1259 SHA256:68c0f360fb2ac7775e32c5f14ac4356ef58aa38939b15b5572aef0ced9d70394
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.13.orig.tar.gz' hicolor-icon-theme_0.13.orig.tar.gz 40709 SHA256:a38b038915480d1ddd4e3c421562560a14d42ace0449a5acc07c50f57f9c3406
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.13-1.debian.tar.gz' hicolor-icon-theme_0.13-1.debian.tar.gz 3342 SHA256:ead36be120055516f938a0fd9075ccc51b4d14c2b93483a255b9ab1b5c4c51e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/hicolor-icon-theme/0.13-1/ (for browsing the source)
- https://sources.debian.net/src/hicolor-icon-theme/0.13-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hicolor-icon-theme/0.13-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hostname=3.15`

Binary Packages:

- `hostname=3.15`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.15
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.15.dsc' hostname_3.15.dsc 804 SHA256:e787dec3ac9ee20ff564d6d7afde242103e71830907ee8fa63367162b04e9844
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.15.tar.gz' hostname_3.15.tar.gz 13039 SHA256:b6d10114ed14306b21745d2cac1b9adf7a2546f16b9fd719bec14bd7cec61d20
```

Other potentially useful URLs:

- https://sources.debian.net/src/hostname/3.15/ (for browsing the source)
- https://sources.debian.net/src/hostname/3.15/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hostname/3.15/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `icu=52.1-8+deb8u8`

Binary Packages:

- `libicu52:amd64=52.1-8+deb8u8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=52.1-8+deb8u8
'http://security.debian.org/debian-security/pool/updates/main/i/icu/icu_52.1-8+deb8u8.dsc' icu_52.1-8+deb8u8.dsc 2015 SHA256:56a5b2c5bdd0e80a23296a59b77d876d15a288c7386ad5283ec95ae037a0780e
'http://security.debian.org/debian-security/pool/updates/main/i/icu/icu_52.1.orig.tar.gz' icu_52.1.orig.tar.gz 23875368 SHA256:2f4d5e68d4698e87759dbdc1a586d053d96935787f79961d192c477b029d8092
'http://security.debian.org/debian-security/pool/updates/main/i/icu/icu_52.1-8+deb8u8.debian.tar.xz' icu_52.1-8+deb8u8.debian.tar.xz 39736 SHA256:48c47216c5768505d437cd421d268e27b23966796d3dc55beaf9597d3b6e2ad6
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/52.1-8+deb8u8/ (for browsing the source)
- https://sources.debian.net/src/icu/52.1-8+deb8u8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/52.1-8+deb8u8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ilmbase=1.0.1-6.1`

Binary Packages:

- `libilmbase-dev=1.0.1-6.1`
- `libilmbase6:amd64=1.0.1-6.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ilmbase=1.0.1-6.1
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_1.0.1-6.1.dsc' ilmbase_1.0.1-6.1.dsc 1381 SHA256:5ab67af57aac8855dacf4dbfd53c71f8bb28fff447b15424de59af02afcc9e8b
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_1.0.1.orig.tar.gz' ilmbase_1.0.1.orig.tar.gz 463275 SHA256:4f14fc7b26a37a391ec5f979697148e6774bc36bc052de26e40ffabe401e397d
'http://deb.debian.org/debian/pool/main/i/ilmbase/ilmbase_1.0.1-6.1.debian.tar.xz' ilmbase_1.0.1-6.1.debian.tar.xz 5636 SHA256:a7e7cdc3d517cb2fd639f8958920f92c8ebb9a537763089aec2715113e031724
```

Other potentially useful URLs:

- https://sources.debian.net/src/ilmbase/1.0.1-6.1/ (for browsing the source)
- https://sources.debian.net/src/ilmbase/1.0.1-6.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ilmbase/1.0.1-6.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `imagemagick=8:6.8.9.9-5+deb8u19`

Binary Packages:

- `imagemagick=8:6.8.9.9-5+deb8u19`
- `imagemagick-6.q16=8:6.8.9.9-5+deb8u19`
- `imagemagick-common=8:6.8.9.9-5+deb8u19`
- `libmagickcore-6-arch-config:amd64=8:6.8.9.9-5+deb8u19`
- `libmagickcore-6-headers=8:6.8.9.9-5+deb8u19`
- `libmagickcore-6.q16-2:amd64=8:6.8.9.9-5+deb8u19`
- `libmagickcore-6.q16-2-extra:amd64=8:6.8.9.9-5+deb8u19`
- `libmagickcore-6.q16-dev:amd64=8:6.8.9.9-5+deb8u19`
- `libmagickcore-dev=8:6.8.9.9-5+deb8u19`
- `libmagickwand-6-headers=8:6.8.9.9-5+deb8u19`
- `libmagickwand-6.q16-2:amd64=8:6.8.9.9-5+deb8u19`
- `libmagickwand-6.q16-dev:amd64=8:6.8.9.9-5+deb8u19`
- `libmagickwand-dev=8:6.8.9.9-5+deb8u19`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/imagemagick-common/copyright`, `/usr/share/doc/libmagickcore-6-arch-config/copyright`, `/usr/share/doc/libmagickcore-6-headers/copyright`, `/usr/share/doc/libmagickcore-6.q16-2/copyright`, `/usr/share/doc/libmagickcore-6.q16-2-extra/copyright`, `/usr/share/doc/libmagickcore-6.q16-dev/copyright`, `/usr/share/doc/libmagickcore-dev/copyright`, `/usr/share/doc/libmagickwand-6-headers/copyright`, `/usr/share/doc/libmagickwand-6.q16-2/copyright`, `/usr/share/doc/libmagickwand-6.q16-dev/copyright`, `/usr/share/doc/libmagickwand-dev/copyright`)

- `Artistic`
- `GPL-1`
- `ImageMagick`
- `ImageMagickLicensePartEZXML`
- `ImageMagickLicensePartFIG`
- `ImageMagickLicensePartGsview`
- `ImageMagickLicensePartOpenSSH`
- `ImageMagickPartGraphicsMagick`
- `ImageMagickPartlibjpeg`
- `ImageMagickPartlibsquish`
- `Magick++`
- `Perllikelicence`
- `TatcherUlrichPublicDomain`

Source:

```console
$ apt-get source -qq --print-uris imagemagick=8:6.8.9.9-5+deb8u19
'http://security.debian.org/debian-security/pool/updates/main/i/imagemagick/imagemagick_6.8.9.9-5+deb8u19.dsc' imagemagick_6.8.9.9-5+deb8u19.dsc 4078 SHA256:235b248bc25b8c514d22b6c2dae02b2ccd21a905075cf2c9903d2d1e169f247c
'http://security.debian.org/debian-security/pool/updates/main/i/imagemagick/imagemagick_6.8.9.9.orig.tar.xz' imagemagick_6.8.9.9.orig.tar.xz 7891624 SHA256:a4cccc70179ff2c67550e063cdcb2e62907338ef3e68b45bb1c41931e515b3eb
'http://security.debian.org/debian-security/pool/updates/main/i/imagemagick/imagemagick_6.8.9.9-5+deb8u19.debian.tar.xz' imagemagick_6.8.9.9-5+deb8u19.debian.tar.xz 327808 SHA256:15231f1801ae9517e19862ef9a5896ff4504dc7b7ed62e0925e5eafb4a073f28
```

Other potentially useful URLs:

- https://sources.debian.net/src/imagemagick/8:6.8.9.9-5+deb8u19/ (for browsing the source)
- https://sources.debian.net/src/imagemagick/8:6.8.9.9-5+deb8u19/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/imagemagick/8:6.8.9.9-5+deb8u19/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `init-system-helpers=1.22`

Binary Packages:

- `init=1.22`

Licenses: (parsed from: `/usr/share/doc/init/copyright`)

- `BSD`
- `GPL`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.22
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.22.dsc' init-system-helpers_1.22.dsc 1880 SHA256:f2ba7e0e1804b56d9c2967ed60be92274619068d7d3894c2dc750f31dbb0ff25
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.22.tar.xz' init-system-helpers_1.22.tar.xz 30728 SHA256:4f64b9fd86f2c68a3996903e03d6024d73f637ff8a06f1bd4f73bedcf8154124
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.22/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.22/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.22/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `insserv=1.14.0-5`

Binary Packages:

- `insserv=1.14.0-5`

Licenses: (parsed from: `/usr/share/doc/insserv/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris insserv=1.14.0-5
'http://deb.debian.org/debian/pool/main/i/insserv/insserv_1.14.0-5.dsc' insserv_1.14.0-5.dsc 1947 SHA256:183dbcd57db6061d61e781197231275fe49c321f6600ec147546d5c24a8ba021
'http://deb.debian.org/debian/pool/main/i/insserv/insserv_1.14.0.orig.tar.gz' insserv_1.14.0.orig.tar.gz 53851 SHA256:da74dcf5225a00aa8aef4d5afc6a20e009b2ed9af328dabd55fef1cb3a32140e
'http://deb.debian.org/debian/pool/main/i/insserv/insserv_1.14.0-5.debian.tar.gz' insserv_1.14.0-5.debian.tar.gz 53943 SHA256:496a3ece3cf4b53ff19f45eeffab6b5a7714785d1db524087c9cbe9cbdd88b2a
```

Other potentially useful URLs:

- https://sources.debian.net/src/insserv/1.14.0-5/ (for browsing the source)
- https://sources.debian.net/src/insserv/1.14.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/insserv/1.14.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iproute2=3.16.0-2`

Binary Packages:

- `iproute2=3.16.0-2`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris iproute2=3.16.0-2
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_3.16.0-2.dsc' iproute2_3.16.0-2.dsc 1693 SHA256:dd657e1707a85c7a15a3a2ba17e3e02fbf133aac4513ed86e4d8b1d6e4cd6a45
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_3.16.0.orig.tar.xz' iproute2_3.16.0.orig.tar.xz 438820 SHA256:1f0a8a6c0e872166f75433f5cbf9766f3002b5c2f13501b3bb8c51846a127b79
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_3.16.0-2.debian.tar.xz' iproute2_3.16.0-2.debian.tar.xz 27032 SHA256:9e5c631b4465ee258a2d61150f6a591f37d116b1b465b363f9e50d496e0359ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/iproute2/3.16.0-2/ (for browsing the source)
- https://sources.debian.net/src/iproute2/3.16.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iproute2/3.16.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iputils=3:20121221-5`

Binary Packages:

- `iputils-ping=3:20121221-5+b2`

Licenses: (parsed from: `/usr/share/doc/iputils-ping/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris iputils=3:20121221-5
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20121221-5.dsc' iputils_20121221-5.dsc 1379 SHA256:fda05ad679d9e20ba415e84fc51e7e3cc4eefbdc9efc560426fd8c4a1cd43ca9
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20121221.orig.tar.bz2' iputils_20121221.orig.tar.bz2 155344 SHA256:450f549fc5b620c23c5929aa6d54b7ddfc7ee1cb1e8efdc5e8bb21d8d0c5319f
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20121221-5.debian.tar.xz' iputils_20121221-5.debian.tar.xz 14360 SHA256:b249a00004cdd96d0f86ed93f45feb7bc9ce76b9a27b513c76aa94869c6064d6
```

Other potentially useful URLs:

- https://sources.debian.net/src/iputils/3:20121221-5/ (for browsing the source)
- https://sources.debian.net/src/iputils/3:20121221-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iputils/3:20121221-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `isl=0.12.2-2`

Binary Packages:

- `libisl10:amd64=0.12.2-2`

Licenses: (parsed from: `/usr/share/doc/libisl10/copyright`)

- `2-clause BSD`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.12.2-2
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.12.2-2.dsc' isl_0.12.2-2.dsc 1245 SHA256:7c6f6a2baeb9ca7f5501fe2262d8e6e28772a4cc19bd1455ee5df6e5b6a60322
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.12.2.orig.tar.bz2' isl_0.12.2.orig.tar.bz2 1319434 SHA256:f4b3dbee9712850006e44f0db2103441ab3d13b406f77996d1df19ee89d11fb4
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.12.2-2.debian.tar.xz' isl_0.12.2-2.debian.tar.xz 17296 SHA256:b91528d5f201c3883f0d57b0c2a44985a933c9e50836ca98000d3db9377784b1
```

Other potentially useful URLs:

- https://sources.debian.net/src/isl/0.12.2-2/ (for browsing the source)
- https://sources.debian.net/src/isl/0.12.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/isl/0.12.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jasper=1.900.1-debian1-2.4+deb8u6`

Binary Packages:

- `libjasper-dev=1.900.1-debian1-2.4+deb8u6`
- `libjasper1:amd64=1.900.1-debian1-2.4+deb8u6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris jasper=1.900.1-debian1-2.4+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/j/jasper/jasper_1.900.1-debian1-2.4+deb8u6.dsc' jasper_1.900.1-debian1-2.4+deb8u6.dsc 2120 SHA256:4b184dd7f8691c356cb7168f3886b543c0743ba8620681c95e57251bb4fa9dc7
'http://security.debian.org/debian-security/pool/updates/main/j/jasper/jasper_1.900.1-debian1.orig.tar.gz' jasper_1.900.1-debian1.orig.tar.gz 1140771 SHA256:7276e8407080d8263b39aeac8305032b0534c7df25bf02718b3944711e3c81d7
'http://security.debian.org/debian-security/pool/updates/main/j/jasper/jasper_1.900.1-debian1-2.4+deb8u6.debian.tar.xz' jasper_1.900.1-debian1-2.4+deb8u6.debian.tar.xz 40280 SHA256:8848691c4284c0927e5393233a8f66d6b82732243d36765ab9a7d6216aa5680f
```

Other potentially useful URLs:

- https://sources.debian.net/src/jasper/1.900.1-debian1-2.4+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/jasper/1.900.1-debian1-2.4+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jasper/1.900.1-debian1-2.4+deb8u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jbigkit=2.1-3.1`

Binary Packages:

- `libjbig-dev:amd64=2.1-3.1`
- `libjbig0:amd64=2.1-3.1`

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

### `dpkg` source package: `jquery=1.7.2+dfsg-3.2+deb8u7`

Binary Packages:

- `libjs-jquery=1.7.2+dfsg-3.2+deb8u7`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery/copyright`)

- `BSD`
- `GPL-2`
- `MIT`
- `MIT,`

Source:

```console
$ apt-get source -qq --print-uris jquery=1.7.2+dfsg-3.2+deb8u7
'http://security.debian.org/debian-security/pool/updates/main/j/jquery/jquery_1.7.2+dfsg-3.2+deb8u7.dsc' jquery_1.7.2+dfsg-3.2+deb8u7.dsc 2028 SHA256:4b7f7e2744f98983b61ba710869672c2301f04fd86e61618732f2deffe699738
'http://security.debian.org/debian-security/pool/updates/main/j/jquery/jquery_1.7.2+dfsg.orig.tar.gz' jquery_1.7.2+dfsg.orig.tar.gz 147053 SHA256:43384d8c975c723a3b7d6f46e7ff1518d161760e0781a37675eeda1a05a503fe
'http://security.debian.org/debian-security/pool/updates/main/j/jquery/jquery_1.7.2+dfsg-3.2+deb8u7.debian.tar.xz' jquery_1.7.2+dfsg-3.2+deb8u7.debian.tar.xz 6520 SHA256:0893dc1605fd0d82c3a4fedbe8c944c97bd0eca93a4dfc516cc62171cf30a1dd
```

Other potentially useful URLs:

- https://sources.debian.net/src/jquery/1.7.2+dfsg-3.2+deb8u7/ (for browsing the source)
- https://sources.debian.net/src/jquery/1.7.2+dfsg-3.2+deb8u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jquery/1.7.2+dfsg-3.2+deb8u7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.5.9-5`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-5+b1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-5
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-5.dsc' keyutils_1.5.9-5.dsc 2080 SHA256:8c8ca9ef9274046901b107f143260bd1255387939ee517ae842829bd167fd49d
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.5.9-5.debian.tar.xz' keyutils_1.5.9-5.debian.tar.xz 14596 SHA256:8cef47fc1fd688cc54e36cbb7cee26f38b38d10a1c59af8d8dc0869a0e4359fc
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.5.9-5/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.5.9-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.5.9-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `kmod=18-3`

Binary Packages:

- `libkmod2:amd64=18-3`

Licenses: (parsed from: `/usr/share/doc/libkmod2/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris kmod=18-3
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_18-3.dsc' kmod_18-3.dsc 1865 SHA256:f16ef133e00db0fa360dcfb0d4723afc31e3803141b5f864e4df6a8b810eaeea
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_18.orig.tar.gz' kmod_18.orig.tar.gz 3692996 SHA256:cdd7c8627e9bbfe5e39232886d08db2c87b4cc2ea7e9f8d3034577324809f2c0
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_18-3.debian.tar.xz' kmod_18-3.debian.tar.xz 10468 SHA256:7a55a9d2c97913cdfde6e29d2784b5b82c7fdad6581d466b4aa571eef3270ea2
```

Other potentially useful URLs:

- https://sources.debian.net/src/kmod/18-3/ (for browsing the source)
- https://sources.debian.net/src/kmod/18-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/kmod/18-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.12.1+dfsg-19+deb8u5`

Binary Packages:

- `krb5-multidev=1.12.1+dfsg-19+deb8u5`
- `libgssapi-krb5-2:amd64=1.12.1+dfsg-19+deb8u5`
- `libgssrpc4:amd64=1.12.1+dfsg-19+deb8u5`
- `libk5crypto3:amd64=1.12.1+dfsg-19+deb8u5`
- `libkadm5clnt-mit9:amd64=1.12.1+dfsg-19+deb8u5`
- `libkadm5srv-mit9:amd64=1.12.1+dfsg-19+deb8u5`
- `libkdb5-7:amd64=1.12.1+dfsg-19+deb8u5`
- `libkrb5-3:amd64=1.12.1+dfsg-19+deb8u5`
- `libkrb5-dev=1.12.1+dfsg-19+deb8u5`
- `libkrb5support0:amd64=1.12.1+dfsg-19+deb8u5`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit9/copyright`, `/usr/share/doc/libkadm5srv-mit9/copyright`, `/usr/share/doc/libkdb5-7/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.12.1+dfsg-19+deb8u5
'http://security.debian.org/debian-security/pool/updates/main/k/krb5/krb5_1.12.1+dfsg-19+deb8u5.dsc' krb5_1.12.1+dfsg-19+deb8u5.dsc 3541 SHA256:1009a2a8874570750f69f59f80ba9dd2651f58108f3b1f065495c7ed08f0c777
'http://security.debian.org/debian-security/pool/updates/main/k/krb5/krb5_1.12.1+dfsg.orig.tar.gz' krb5_1.12.1+dfsg.orig.tar.gz 11792370 SHA256:eb29959f1e9f8d71e7401f5809daefae067296eb5b0da1176366280a16bdd784
'http://security.debian.org/debian-security/pool/updates/main/k/krb5/krb5_1.12.1+dfsg-19+deb8u5.debian.tar.xz' krb5_1.12.1+dfsg-19+deb8u5.debian.tar.xz 129708 SHA256:e4d511b15cf9f812e81ff98076604325f2dfa46e72f713d3c60eaa875e78f380
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.12.1+dfsg-19+deb8u5/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.12.1+dfsg-19+deb8u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.12.1+dfsg-19+deb8u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.6-3+deb8u2`

Binary Packages:

- `liblcms2-2:amd64=2.6-3+deb8u2`
- `liblcms2-dev:amd64=2.6-3+deb8u2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.6-3+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/l/lcms2/lcms2_2.6-3+deb8u2.dsc' lcms2_2.6-3+deb8u2.dsc 2132 SHA256:28a0f90176b2ad36544bfab0d08dfcdabe552c4b9e843fc1bf52d51861e30acb
'http://security.debian.org/debian-security/pool/updates/main/l/lcms2/lcms2_2.6.orig.tar.gz' lcms2_2.6.orig.tar.gz 4583389 SHA256:5172528839647c54c3da211837225e221be93e4733f5b5e9f57668f7107e14b1
'http://security.debian.org/debian-security/pool/updates/main/l/lcms2/lcms2_2.6-3+deb8u2.debian.tar.xz' lcms2_2.6-3+deb8u2.debian.tar.xz 2417368 SHA256:ad24110e3a97dd1061e6338ec74e209c26b2aeb70acca8feedd0f6105197dca0
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.6-3+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.6-3+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.6-3+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.7.0-2+deb8u1`

Binary Packages:

- `libbsd0:amd64=0.7.0-2+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libbsd=0.7.0-2+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/libb/libbsd/libbsd_0.7.0-2+deb8u1.dsc' libbsd_0.7.0-2+deb8u1.dsc 2208 SHA256:4536b43cad550b9e54292ba2028fdb73e58df9afda863f4ed2f67323d484acc9
'http://security.debian.org/debian-security/pool/updates/main/libb/libbsd/libbsd_0.7.0.orig.tar.xz' libbsd_0.7.0.orig.tar.xz 322908 SHA256:0f3b0e17e5c34c038126e0a04351b11e23c6101a7d0ce3beeab29bb6415c10bb
'http://security.debian.org/debian-security/pool/updates/main/libb/libbsd/libbsd_0.7.0-2+deb8u1.debian.tar.xz' libbsd_0.7.0-2+deb8u1.debian.tar.xz 17076 SHA256:e4ead0d6595c0fe281f030c31ffd39b4a0e11bf8e0c57d176bce86230c06f6a3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.7.0-2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.7.0-2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.7.0-2+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap2=1:2.24-8`

Binary Packages:

- `libcap2:amd64=1:2.24-8`
- `libcap2-bin=1:2.24-8`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.24-8
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.24-8.dsc' libcap2_2.24-8.dsc 2134 SHA256:b042a6c89079d02113bd15ec52948f265edb6c725830d1b79434af06c4e6006a
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.24.orig.tar.xz' libcap2_2.24.orig.tar.xz 63264 SHA256:51cd1c568a2baf1e687573bd6117a94b07f33b46a05acaa50ee208792a830b79
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.24-8.debian.tar.xz' libcap2_2.24-8.debian.tar.xz 17528 SHA256:d1dd71eb19ce4cb7ea37f827c155382773e7724d5356619539874dca647aa94e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.24-8/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.24-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.24-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcroco=0.6.8-3`

Binary Packages:

- `libcroco3:amd64=0.6.8-3+b1`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.8-3
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.8-3.dsc' libcroco_0.6.8-3.dsc 1680 SHA256:c82786e4bca2ee80dde79fa06ce5bb170bb7018c75f78c2c274cee5911d93133
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.8.orig.tar.xz' libcroco_0.6.8.orig.tar.xz 464992 SHA256:ea6e1b858c55219cefd7109756bff5bc1a774ba7a55f7d3ccd734d6b871b8570
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.8-3.debian.tar.xz' libcroco_0.6.8-3.debian.tar.xz 6568 SHA256:b180f787fe4244ac57e342bfad2fa89f2a2fee4bf9eeb8170ccf57c483c08917
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcroco/0.6.8-3/ (for browsing the source)
- https://sources.debian.net/src/libcroco/0.6.8-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcroco/0.6.8-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdatrie=0.2.8-1`

Binary Packages:

- `libdatrie1:amd64=0.2.8-1`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.8-1
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.8-1.dsc' libdatrie_0.2.8-1.dsc 2082 SHA256:4cea8f61d67778ae16fa24eb28c413b5c3cc3203f84a50ba0944956a9bba05a2
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.8.orig.tar.xz' libdatrie_0.2.8.orig.tar.xz 286428 SHA256:6a14d55c5687fc325216fffb5db0cf55d31b108cce65314a6d5c8042417ab7c2
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.8-1.debian.tar.gz' libdatrie_0.2.8-1.debian.tar.gz 7651 SHA256:7563b262c917cb507d17b35437a484c54c2964cff9994ffbbac1f78fb5f3c59b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdatrie/0.2.8-1/ (for browsing the source)
- https://sources.debian.net/src/libdatrie/0.2.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdatrie/0.2.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20140620-2`

Binary Packages:

- `libedit2:amd64=3.1-20140620-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20140620-2
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20140620-2.dsc' libedit_3.1-20140620-2.dsc 2235 SHA256:ca5af1e511d53595d6f518c9f4805feba66af23d3c468a92d9e84c1987af7512
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20140620.orig.tar.gz' libedit_3.1-20140620.orig.tar.gz 483857 SHA256:a22b9b2a8cf4aec9ff51a57e8c848b69640d0195282159d245d8137a19bfcaf2
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20140620-2.debian.tar.bz2' libedit_3.1-20140620-2.debian.tar.bz2 17637 SHA256:610d08273c7f73a83dad62b322a520497c12b9714bb1d9b54918c7bc0b3bb6ff
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20140620-2/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20140620-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20140620-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libelf=0.8.13-5`

Binary Packages:

- `libelfg0:amd64=0.8.13-5`

Licenses: (parsed from: `/usr/share/doc/libelfg0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libelf=0.8.13-5
'http://deb.debian.org/debian/pool/main/libe/libelf/libelf_0.8.13-5.dsc' libelf_0.8.13-5.dsc 1068 SHA256:cee33bd0bb5964e66bad8b405cccf9ffc8472e25b4e2b3119c15cfb3bc5ec9f7
'http://deb.debian.org/debian/pool/main/libe/libelf/libelf_0.8.13.orig.tar.gz' libelf_0.8.13.orig.tar.gz 149591 SHA256:559073b1796bf961aeded2117dfb84eb71936f199ce49e8b40d8d6096ed01c84
'http://deb.debian.org/debian/pool/main/libe/libelf/libelf_0.8.13-5.diff.gz' libelf_0.8.13-5.diff.gz 90192 SHA256:587f4d1dc689d1bc23e6bda5a76a33aa2f2566cc86382ee408d1acfe515f487b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libelf/0.8.13-5/ (for browsing the source)
- https://sources.debian.net/src/libelf/0.8.13-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libelf/0.8.13-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liberror-perl=0.17-1.1`

Binary Packages:

- `liberror-perl=0.17-1.1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17-1.1
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17-1.1.dsc' liberror-perl_0.17-1.1.dsc 1707 SHA256:b042cdc85fca61bbc96765dfa9dc1043319b0259485d502b26856addc2ad1969
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17.orig.tar.gz' liberror-perl_0.17.orig.tar.gz 17266 SHA256:2e8157981a77e87d37d26d8b6b3183560dddc541b491b0b32fcda010730b257c
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17-1.1.diff.gz' liberror-perl_0.17-1.1.diff.gz 3541 SHA256:ff276a25fc81edf38681f03a9f44346516226b5ab3c95f552d8d7f24686ab7d9
```

Other potentially useful URLs:

- https://sources.debian.net/src/liberror-perl/0.17-1.1/ (for browsing the source)
- https://sources.debian.net/src/liberror-perl/0.17-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liberror-perl/0.17-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libevent=2.0.21-stable-2+deb8u1`

Binary Packages:

- `libevent-2.0-5:amd64=2.0.21-stable-2+deb8u1`
- `libevent-core-2.0-5:amd64=2.0.21-stable-2+deb8u1`
- `libevent-dev=2.0.21-stable-2+deb8u1`
- `libevent-extra-2.0-5:amd64=2.0.21-stable-2+deb8u1`
- `libevent-openssl-2.0-5:amd64=2.0.21-stable-2+deb8u1`
- `libevent-pthreads-2.0-5:amd64=2.0.21-stable-2+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libevent=2.0.21-stable-2+deb8u1
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.0.21-stable-2+deb8u1.dsc' libevent_2.0.21-stable-2+deb8u1.dsc 2460 SHA256:54c4e18472229cfc33b4eef8f0e6191ce362cd71ab8995c3b4f6ba79e5feb69e
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.0.21-stable.orig.tar.gz' libevent_2.0.21-stable.orig.tar.gz 850772 SHA256:22a530a8a5ba1cb9c080cba033206b17dacd21437762155c6d30ee6469f574f5
'http://deb.debian.org/debian/pool/main/libe/libevent/libevent_2.0.21-stable-2+deb8u1.debian.tar.xz' libevent_2.0.21-stable-2+deb8u1.debian.tar.xz 13900 SHA256:5cf722d138ffd789ea54d0b6703e1187bc0170d1580e528d3db635d397f8aaf6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libevent/2.0.21-stable-2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libevent/2.0.21-stable-2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libevent/2.0.21-stable-2+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libexif=0.6.21-2+deb8u4`

Binary Packages:

- `libexif-dev=0.6.21-2+deb8u4`
- `libexif12:amd64=0.6.21-2+deb8u4`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.21-2+deb8u4
'http://security.debian.org/debian-security/pool/updates/main/libe/libexif/libexif_0.6.21-2+deb8u4.dsc' libexif_0.6.21-2+deb8u4.dsc 2098 SHA256:0551ba7f793ca4d9c7846323a96321e65fbf0bb6720e704e29eb1b2962363b97
'http://security.debian.org/debian-security/pool/updates/main/libe/libexif/libexif_0.6.21.orig.tar.gz' libexif_0.6.21.orig.tar.gz 2081615 SHA256:edb7eb13664cf950a6edd132b75e99afe61c5effe2f16494e6d27bc404b287bf
'http://security.debian.org/debian-security/pool/updates/main/libe/libexif/libexif_0.6.21-2+deb8u4.debian.tar.xz' libexif_0.6.21-2+deb8u4.debian.tar.xz 16732 SHA256:b898554dc0736ac3b5bc2bef508eb1a3e714c4c0a43704995d30b15b99315a05
```

Other potentially useful URLs:

- https://sources.debian.net/src/libexif/0.6.21-2+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/libexif/0.6.21-2+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libexif/0.6.21-2+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.1-2+deb8u1`

Binary Packages:

- `libffi-dev:amd64=3.1-2+deb8u1`
- `libffi6:amd64=3.1-2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.1-2+deb8u1
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.1-2+deb8u1.dsc' libffi_3.1-2+deb8u1.dsc 1691 SHA256:db5a3fe5558d7858cb8d9cdc7e0cf5c1c51622c3b313c0a0ac64eb7ff5298a63
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.1.orig.tar.gz' libffi_3.1.orig.tar.gz 937214 SHA256:97feeeadca5e21870fa4433bc953d1b3af3f698d5df8a428f68b73cd60aef6eb
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.1-2+deb8u1.debian.tar.xz' libffi_3.1-2+deb8u1.debian.tar.xz 8948 SHA256:71ab991f52edbdf0e19408b6c947650d92c766842581eb172ab9a44bf0ce3ab8
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.1-2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.1-2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.1-2+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.6.3-2+deb8u8`

Binary Packages:

- `libgcrypt20:amd64=1.6.3-2+deb8u8`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.6.3-2+deb8u8
'http://security.debian.org/debian-security/pool/updates/main/libg/libgcrypt20/libgcrypt20_1.6.3-2+deb8u8.dsc' libgcrypt20_1.6.3-2+deb8u8.dsc 2587 SHA256:ea55179c07cf8938d197c81024dd3090c40d1bfbbc6b3dad13f2abb9b48f5eda
'http://security.debian.org/debian-security/pool/updates/main/libg/libgcrypt20/libgcrypt20_1.6.3.orig.tar.bz2' libgcrypt20_1.6.3.orig.tar.bz2 2494052 SHA256:41b4917b93ae34c6a0e2127378d7a4d66d805a2a86a09911d4f9bd871db7025f
'http://security.debian.org/debian-security/pool/updates/main/libg/libgcrypt20/libgcrypt20_1.6.3-2+deb8u8.debian.tar.xz' libgcrypt20_1.6.3-2+deb8u8.debian.tar.xz 36572 SHA256:fbaadf6c59fd0bbcfa7bd57329f00c94829cf1ab9b0f17699af30c469db03e76
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.6.3-2+deb8u8/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.6.3-2+deb8u8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.6.3-2+deb8u8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgd2=2.1.0-5+deb8u14`

Binary Packages:

- `libgd3:amd64=2.1.0-5+deb8u14`

Licenses: (parsed from: `/usr/share/doc/libgd3/copyright`)

- `BSD-3-clause`
- `GAP~Makefile.in`
- `GAP~configure`
- `GD`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `HPND`
- `MIT`
- `WEBP`
- `XFIG`

Source:

```console
$ apt-get source -qq --print-uris libgd2=2.1.0-5+deb8u14
'http://security.debian.org/debian-security/pool/updates/main/libg/libgd2/libgd2_2.1.0-5+deb8u14.dsc' libgd2_2.1.0-5+deb8u14.dsc 2355 SHA256:f29cf1be1c2577a55289129cfb7558dc5ccbd9d646aeaab51891bbbed96f3f9f
'http://security.debian.org/debian-security/pool/updates/main/libg/libgd2/libgd2_2.1.0.orig.tar.xz' libgd2_2.1.0.orig.tar.xz 2004304 SHA256:fa6665dfe3d898019671293c84d77067a3d2ede50884dbcb6df899d508370e5a
'http://security.debian.org/debian-security/pool/updates/main/libg/libgd2/libgd2_2.1.0-5+deb8u14.debian.tar.xz' libgd2_2.1.0-5+deb8u14.debian.tar.xz 44828 SHA256:4953cdcde1a6f362c44411c9e803832c35d9dc04ecd4d2d8fa69e7c1648aab16
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgd2/2.1.0-5+deb8u14/ (for browsing the source)
- https://sources.debian.net/src/libgd2/2.1.0-5+deb8u14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgd2/2.1.0-5+deb8u14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.17-3`

Binary Packages:

- `libgpg-error0:amd64=1.17-3`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `GPL-2.1+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.17-3
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.17-3.dsc' libgpg-error_1.17-3.dsc 2344 SHA256:42d9ff8517b1149b453d947b515cef088b83ac6a6b4fdcbd143570c42e2216c9
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.17.orig.tar.bz2' libgpg-error_1.17.orig.tar.bz2 669914 SHA256:3ff4e5a71116eb862cd14185fcd282850927b8608e3b4186834fd940fbef57b5
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.17-3.debian.tar.xz' libgpg-error_1.17-3.debian.tar.xz 38460 SHA256:3e0af89c65e61ed2b53555eaecd5dc7fa19519490ef447313f441728ae490f29
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.17-3/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.17-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.17-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libice=2:1.0.9-1+deb8u1`

Binary Packages:

- `libice-dev:amd64=2:1.0.9-1+deb8u1`
- `libice6:amd64=2:1.0.9-1+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-1+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/libi/libice/libice_1.0.9-1+deb8u1.dsc' libice_1.0.9-1+deb8u1.dsc 2355 SHA256:222dfba0f569e89356becbc805a1dc709a8188c66c0242ffa38a2ff19afb74b9
'http://security.debian.org/debian-security/pool/updates/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://security.debian.org/debian-security/pool/updates/main/libi/libice/libice_1.0.9-1+deb8u1.diff.gz' libice_1.0.9-1+deb8u1.diff.gz 6413 SHA256:94bb2b47d111e6f6a2460ed2154bf8894db866ec6abb37465c8c1cb937c671ec
```

Other potentially useful URLs:

- https://sources.debian.net/src/libice/2:1.0.9-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libice/2:1.0.9-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libice/2:1.0.9-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn=1.29-1+deb8u3`

Binary Packages:

- `libidn11:amd64=1.29-1+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libidn11/copyright`)

- `GAP`
- `GFDL-1.3`
- `GFDL-1.3+`
- `GPL-2`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+ | GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libidn=1.29-1+deb8u3
'http://security.debian.org/debian-security/pool/updates/main/libi/libidn/libidn_1.29-1+deb8u3.dsc' libidn_1.29-1+deb8u3.dsc 2181 SHA256:ddbc55c4bbf8697d21eb1da1716a501b089b40550f4dfaa8d211716043e5919c
'http://security.debian.org/debian-security/pool/updates/main/libi/libidn/libidn_1.29.orig.tar.gz' libidn_1.29.orig.tar.gz 3474087 SHA256:fb82747dbbf9b36f703ed27293317d818d7e851d4f5773dedf3efa4db32a7c7c
'http://security.debian.org/debian-security/pool/updates/main/libi/libidn/libidn_1.29-1+deb8u3.debian.tar.xz' libidn_1.29-1+deb8u3.debian.tar.xz 71392 SHA256:8296ad1847cf52b8c284705c986549a27b854dcf36993431c789b18a314e49db
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn/1.29-1+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/libidn/1.29-1+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn/1.29-1+deb8u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libjpeg-turbo=1:1.3.1-12+deb8u2`

Binary Packages:

- `libjpeg-dev=1:1.3.1-12+deb8u2`
- `libjpeg62-turbo:amd64=1:1.3.1-12+deb8u2`
- `libjpeg62-turbo-dev:amd64=1:1.3.1-12+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3`
- `BSD-BY-LC-NE`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:1.3.1-12+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/libj/libjpeg-turbo/libjpeg-turbo_1.3.1-12+deb8u2.dsc' libjpeg-turbo_1.3.1-12+deb8u2.dsc 2562 SHA256:fcf692f2e671abb057b6364af915e05ba2b1638c019305938f0e21e1bb94ad0e
'http://security.debian.org/debian-security/pool/updates/main/libj/libjpeg-turbo/libjpeg-turbo_1.3.1.orig.tar.gz' libjpeg-turbo_1.3.1.orig.tar.gz 1390282 SHA256:c132907417ddc40ed552fe53d6b91d5fecbb14a356a60ddc7ea50d6be9666fb9
'http://security.debian.org/debian-security/pool/updates/main/libj/libjpeg-turbo/libjpeg-turbo_1.3.1-12+deb8u2.debian.tar.xz' libjpeg-turbo_1.3.1-12+deb8u2.debian.tar.xz 81956 SHA256:7878e86dcfdc6239bc35bfecf5409fdd968f4f9b2e1979e60261854d788ddbda
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:1.3.1-12+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:1.3.1-12+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:1.3.1-12+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liblocale-gettext-perl=1.05-8`

Binary Packages:

- `liblocale-gettext-perl=1.05-8+b1`

Licenses: (parsed from: `/usr/share/doc/liblocale-gettext-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris liblocale-gettext-perl=1.05-8
'http://deb.debian.org/debian/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.05-8.dsc' liblocale-gettext-perl_1.05-8.dsc 2114 SHA256:0549ab2b517c1aed9fb12e2fee3ee2eded5efa80758491089f531b3ca10cc4ab
'http://deb.debian.org/debian/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.05.orig.tar.gz' liblocale-gettext-perl_1.05.orig.tar.gz 7693 SHA256:27367f3dc1be79c9ed178732756e37e4cfce45f9e2a27ebf26e1f40d80124694
'http://deb.debian.org/debian/pool/main/libl/liblocale-gettext-perl/liblocale-gettext-perl_1.05-8.debian.tar.xz' liblocale-gettext-perl_1.05-8.debian.tar.xz 5472 SHA256:2bd28828012a6289052e1905779f0505d2e09f279d77a79611990ad8d2f27ba1
```

Other potentially useful URLs:

- https://sources.debian.net/src/liblocale-gettext-perl/1.05-8/ (for browsing the source)
- https://sources.debian.net/src/liblocale-gettext-perl/1.05-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liblocale-gettext-perl/1.05-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liblqr=0.4.2-2`

Binary Packages:

- `liblqr-1-0:amd64=0.4.2-2`
- `liblqr-1-0-dev=0.4.2-2`

Licenses: (parsed from: `/usr/share/doc/liblqr-1-0/copyright`, `/usr/share/doc/liblqr-1-0-dev/copyright`)

- `GPL-3`
- `GPLv3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris liblqr=0.4.2-2
'http://deb.debian.org/debian/pool/main/libl/liblqr/liblqr_0.4.2-2.dsc' liblqr_0.4.2-2.dsc 2024 SHA256:7e203605ebe40cde3e467db4298d7ee3f83f3d3082b05f8984868cdef1606245
'http://deb.debian.org/debian/pool/main/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA256:d4c22373432cca749e4326cd41fce365e6ff857c0bfd7a5302b8eb34b69f0336
'http://deb.debian.org/debian/pool/main/libl/liblqr/liblqr_0.4.2-2.debian.tar.xz' liblqr_0.4.2-2.debian.tar.xz 5860 SHA256:2c886ee88f65eade9e1cd10965bf572a3cc178d6119b9342c8469b6b41d2bb62
```

Other potentially useful URLs:

- https://sources.debian.net/src/liblqr/0.4.2-2/ (for browsing the source)
- https://sources.debian.net/src/liblqr/0.4.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liblqr/0.4.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng=1.2.50-2+deb8u3`

Binary Packages:

- `libpng12-0:amd64=1.2.50-2+deb8u3`
- `libpng12-dev:amd64=1.2.50-2+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libpng12-0/copyright`, `/usr/share/doc/libpng12-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libpng=1.2.50-2+deb8u3
'http://deb.debian.org/debian/pool/main/libp/libpng/libpng_1.2.50-2+deb8u3.dsc' libpng_1.2.50-2+deb8u3.dsc 2036 SHA256:0db1eafb75ca276bc5b3e69810149ab53cc7344effa67e94269cde0c162fc720
'http://deb.debian.org/debian/pool/main/libp/libpng/libpng_1.2.50.orig.tar.xz' libpng_1.2.50.orig.tar.xz 539152 SHA256:4724f81f8c92ac7f360ad1fbf173396ea7c535923424db9fbaff07bfd9d8e8e7
'http://deb.debian.org/debian/pool/main/libp/libpng/libpng_1.2.50-2+deb8u3.debian.tar.xz' libpng_1.2.50-2+deb8u3.debian.tar.xz 21788 SHA256:b47238628a87fac02640b05bb4af5ada003c5180958a143ef670780ad4208cd7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpng/1.2.50-2+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/libpng/1.2.50-2+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpng/1.2.50-2+deb8u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpsl=0.5.1-1`

Binary Packages:

- `libpsl0:amd64=0.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libpsl0/copyright`)

- `CC0`
- `MIT`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.5.1-1
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.5.1-1.dsc' libpsl_0.5.1-1.dsc 2201 SHA256:bf97e1fca2374470955b08c654877d38d4cc31b82fe51bbe89d8338ea79211d5
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.5.1.orig.tar.gz' libpsl_0.5.1.orig.tar.gz 81875 SHA256:c4e33bc2c2a04e6a989a0dac529d8ca6604a77e59b638ce263a71153d3a48ceb
'http://deb.debian.org/debian/pool/main/libp/libpsl/libpsl_0.5.1-1.debian.tar.xz' libpsl_0.5.1-1.debian.tar.xz 9972 SHA256:b6a49905a56c3da3d3292b6b50f471cdbdca25d426ca937be3f0f961ba94c0bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpsl/0.5.1-1/ (for browsing the source)
- https://sources.debian.net/src/libpsl/0.5.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpsl/0.5.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpthread-stubs=0.3-4`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.3-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.3-4
'http://deb.debian.org/debian/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3-4.dsc' libpthread-stubs_0.3-4.dsc 1925 SHA256:e72310a5492e641076c199561977703947174c6acc3633073d909f6f5ab3c676
'http://deb.debian.org/debian/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3.orig.tar.gz' libpthread-stubs_0.3.orig.tar.gz 272939 SHA256:3031f466cf0b06de6b3ccbf2019d15c4fcf75229b7d226a711bc1885b3a82cde
'http://deb.debian.org/debian/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3-4.diff.gz' libpthread-stubs_0.3-4.diff.gz 2413 SHA256:ce3eb8bdc0f1a4347d42c5736d056973fae46908b764a9f2be83e1bd210f2024
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpthread-stubs/0.3-4/ (for browsing the source)
- https://sources.debian.net/src/libpthread-stubs/0.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpthread-stubs/0.3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `librsvg=2.40.5-1+deb8u2`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.40.5-1+deb8u2`
- `librsvg2-2:amd64=2.40.5-1+deb8u2`
- `librsvg2-common:amd64=2.40.5-1+deb8u2`
- `librsvg2-dev:amd64=2.40.5-1+deb8u2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.40.5-1+deb8u2
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.40.5-1+deb8u2.dsc' librsvg_2.40.5-1+deb8u2.dsc 2800 SHA256:7c027829c963f08180f65efe66dcc22ae19a7a8758127f7cc0856cfed7ad3b85
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.40.5.orig.tar.xz' librsvg_2.40.5.orig.tar.xz 509556 SHA256:d14d7b3e25023ce34302022fd7c9b3a468629c94dff6c177874629686bfc71a7
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.40.5-1+deb8u2.debian.tar.xz' librsvg_2.40.5-1+deb8u2.debian.tar.xz 18540 SHA256:7fa36cd67efbce435edcb1a430eb339608ede51516a55332368a385a1d968bc7
```

Other potentially useful URLs:

- https://sources.debian.net/src/librsvg/2.40.5-1+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/librsvg/2.40.5-1+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librsvg/2.40.5-1+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=2.3-2`

Binary Packages:

- `libselinux1:amd64=2.3-2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.3-2
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.3-2.dsc' libselinux_2.3-2.dsc 2024 SHA256:aea0e0502dd1d4df17be644efb0bfe2d38e32ba2e0769eaaf8a2b64a0eb99786
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.3.orig.tar.gz' libselinux_2.3.orig.tar.gz 171254 SHA256:0b1e0b43ecd84a812713d09564019b08e7c205d89072b5cbcd07b052cd8e77b2
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.3-2.debian.tar.xz' libselinux_2.3-2.debian.tar.xz 24384 SHA256:8ec4bdb5acc066d1b369877e9a94ec1a723e4d31691753e0e1861d0884b3fd1a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/2.3-2/ (for browsing the source)
- https://sources.debian.net/src/libselinux/2.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/2.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=2.3-1`

Binary Packages:

- `libsemanage-common=2.3-1`
- `libsemanage1:amd64=2.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.3-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.3-1.dsc' libsemanage_2.3-1.dsc 2131 SHA256:21b321c61399deeb3d1b04b76a0c9f43e968371f3afc8a8eb859e3cc79f295aa
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.3.orig.tar.gz' libsemanage_2.3.orig.tar.gz 138231 SHA256:03e09e35e611c286e446bef92b6023ef2623815996f5a53394bb02e49a312e4b
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.3-1.debian.tar.xz' libsemanage_2.3-1.debian.tar.xz 14848 SHA256:e6e8002ae5084daf6628ac836e4724005dd7591f9a015203bb55e445508e55e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/2.3-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/2.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/2.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=2.3-2`

Binary Packages:

- `libsepol1:amd64=2.3-2`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.3-2
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.3-2.dsc' libsepol_2.3-2.dsc 1762 SHA256:115ab27d7662fc03e64d9e70ed20b5dcb2adb6206155ba2577072352a5b79b6a
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.3.orig.tar.gz' libsepol_2.3.orig.tar.gz 209570 SHA256:cc8d8642c3b7b95d6928d65dcbca2ab0627abc1c05166637851e63c1a6eae68f
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.3-2.debian.tar.xz' libsepol_2.3-2.debian.tar.xz 12904 SHA256:4fea6f6de03cf6a8ba80579988ad56202d3652fe3153b0d2f8c65c89bba097a5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/2.3-2/ (for browsing the source)
- https://sources.debian.net/src/libsepol/2.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/2.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsigsegv=2.10-4`

Binary Packages:

- `libsigsegv2:amd64=2.10-4+b1`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.10-4
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.10-4.dsc' libsigsegv_2.10-4.dsc 2166 SHA256:54837482677ed4d42203c80bb10ba0308431a00cb8ccca3256cce8a3bdfa8d8e
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.10.orig.tar.gz' libsigsegv_2.10.orig.tar.gz 402279 SHA256:8460a4a3dd4954c3d96d7a4f5dd5bc4d9b76f5754196aa245287553b26d2199a
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.10-4.debian.tar.xz' libsigsegv_2.10-4.debian.tar.xz 9532 SHA256:abc74f39b89e7dc5ee46cf4e9cf9e6b9dcc00122ffe87e49036647c5e9a10d36
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsigsegv/2.10-4/ (for browsing the source)
- https://sources.debian.net/src/libsigsegv/2.10-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsigsegv/2.10-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsm=2:1.2.2-1`

Binary Packages:

- `libsm-dev:amd64=2:1.2.2-1+b1`
- `libsm6:amd64=2:1.2.2-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.2-1
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.2-1.dsc' libsm_1.2.2-1.dsc 2107 SHA256:1347efa550751179c0a3f1042a9f8ae43ee0c22cf0c2283921fa83e52a68433f
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.2.orig.tar.gz' libsm_1.2.2.orig.tar.gz 415990 SHA256:14bb7c669ce2b8ff712fbdbf48120e3742a77edcd5e025d6b3325ed30cf120f4
'http://deb.debian.org/debian/pool/main/libs/libsm/libsm_1.2.2-1.diff.gz' libsm_1.2.2-1.diff.gz 6183 SHA256:9848714292ead15fcc48ab2d337f2cc5fc08910abbdfaf69d3ef1b89d3fdb2d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsm/2:1.2.2-1/ (for browsing the source)
- https://sources.debian.net/src/libsm/2:1.2.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsm/2:1.2.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libssh2=1.4.3-4.1+deb8u6`

Binary Packages:

- `libssh2-1:amd64=1.4.3-4.1+deb8u6`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.4.3-4.1+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/libs/libssh2/libssh2_1.4.3-4.1+deb8u6.dsc' libssh2_1.4.3-4.1+deb8u6.dsc 1928 SHA256:472132e47027254028064c6e7ff9e08f3788bdf3a7d9126a31a60fc4d4318601
'http://security.debian.org/debian-security/pool/updates/main/libs/libssh2/libssh2_1.4.3.orig.tar.gz' libssh2_1.4.3.orig.tar.gz 685712 SHA256:eac6f85f9df9db2e6386906a6227eb2cd7b3245739561cad7d6dc1d5d021b96d
'http://security.debian.org/debian-security/pool/updates/main/libs/libssh2/libssh2_1.4.3-4.1+deb8u6.debian.tar.xz' libssh2_1.4.3-4.1+deb8u6.debian.tar.xz 22832 SHA256:a4784e7a346017251f032e67efc8b5a293189e2a2e25f7c2c0df87f1539d7d99
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.4.3-4.1+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.4.3-4.1+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.4.3-4.1+deb8u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.2-3+deb8u4`

Binary Packages:

- `libtasn1-6:amd64=4.2-3+deb8u4`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.2-3+deb8u4
'http://security.debian.org/debian-security/pool/updates/main/libt/libtasn1-6/libtasn1-6_4.2-3+deb8u4.dsc' libtasn1-6_4.2-3+deb8u4.dsc 2607 SHA256:9fe778ed52ad7ce359e8e28fddf9bf9d50fb52cb649a6df92f25e0614c83a07a
'http://security.debian.org/debian-security/pool/updates/main/libt/libtasn1-6/libtasn1-6_4.2.orig.tar.gz' libtasn1-6_4.2.orig.tar.gz 1866192 SHA256:693b41cb36c2ac02d5990180b0712a79a591168e93d85f7fcbb75a0a0be4cdbb
'http://security.debian.org/debian-security/pool/updates/main/libt/libtasn1-6/libtasn1-6_4.2-3+deb8u4.debian.tar.xz' libtasn1-6_4.2-3+deb8u4.debian.tar.xz 59628 SHA256:5adf560fc2a5d92b7740c243c6c5872d01edcdfc21e17597508fc3fe4a533345
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.2-3+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.2-3+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.2-3+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtext-charwidth-perl=0.04-7`

Binary Packages:

- `libtext-charwidth-perl=0.04-7+b3`

Licenses: (parsed from: `/usr/share/doc/libtext-charwidth-perl/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libtext-charwidth-perl=0.04-7
'http://deb.debian.org/debian/pool/main/libt/libtext-charwidth-perl/libtext-charwidth-perl_0.04-7.dsc' libtext-charwidth-perl_0.04-7.dsc 1810 SHA256:482493991d54786bc12b38f26b90d2bbc9234ac87c3e54e0474ac00cd979dd68
'http://deb.debian.org/debian/pool/main/libt/libtext-charwidth-perl/libtext-charwidth-perl_0.04.orig.tar.bz2' libtext-charwidth-perl_0.04.orig.tar.bz2 8327 SHA256:2990c13c3f4a5479d7dbc5a94b86c23798cf0dc7df54ffe54e065f072558b6ed
'http://deb.debian.org/debian/pool/main/libt/libtext-charwidth-perl/libtext-charwidth-perl_0.04-7.debian.tar.bz2' libtext-charwidth-perl_0.04-7.debian.tar.bz2 3220 SHA256:4aa60af66136cad15d3c9ed73696b822c9f944a3b8484b03c388393302fa6038
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtext-charwidth-perl/0.04-7/ (for browsing the source)
- https://sources.debian.net/src/libtext-charwidth-perl/0.04-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtext-charwidth-perl/0.04-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtext-iconv-perl=1.7-5`

Binary Packages:

- `libtext-iconv-perl=1.7-5+b2`

Licenses: (parsed from: `/usr/share/doc/libtext-iconv-perl/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libtext-iconv-perl=1.7-5
'http://deb.debian.org/debian/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7-5.dsc' libtext-iconv-perl_1.7-5.dsc 1828 SHA256:6f049f3ed556a9c429f00c88a28ce595446f26996f2f5173e02f51f51277749d
'http://deb.debian.org/debian/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7.orig.tar.bz2' libtext-iconv-perl_1.7.orig.tar.bz2 9977 SHA256:815c5169b7afc40bc6f681b4c615ff8fb0e073d87422280c8c759a4666567490
'http://deb.debian.org/debian/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7-5.debian.tar.bz2' libtext-iconv-perl_1.7-5.debian.tar.bz2 3157 SHA256:e0ee2ae3908bbde6d43098a6491284fdc7a0a117229053d1e9c539eb66127092
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtext-iconv-perl/1.7-5/ (for browsing the source)
- https://sources.debian.net/src/libtext-iconv-perl/1.7-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtext-iconv-perl/1.7-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtext-wrapi18n-perl=0.06-7`

Binary Packages:

- `libtext-wrapi18n-perl=0.06-7`

Licenses: (parsed from: `/usr/share/doc/libtext-wrapi18n-perl/copyright`)

- `Artistic`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtext-wrapi18n-perl=0.06-7
'http://deb.debian.org/debian/pool/main/libt/libtext-wrapi18n-perl/libtext-wrapi18n-perl_0.06-7.dsc' libtext-wrapi18n-perl_0.06-7.dsc 1156 SHA256:777dd5309172c3fa6ccea73b3c821cf6533ddb72b4adbe4def9d45fd8902b544
'http://deb.debian.org/debian/pool/main/libt/libtext-wrapi18n-perl/libtext-wrapi18n-perl_0.06.orig.tar.gz' libtext-wrapi18n-perl_0.06.orig.tar.gz 3797 SHA256:432c2a801efe9f12d631124c1163439eac4c99449ba13d80133c45ecacc627f5
'http://deb.debian.org/debian/pool/main/libt/libtext-wrapi18n-perl/libtext-wrapi18n-perl_0.06-7.diff.gz' libtext-wrapi18n-perl_0.06-7.diff.gz 3031 SHA256:fae1a435e8b2604bf78666e58e4603728990495db302a9799d63cb099e3b4001
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtext-wrapi18n-perl/0.06-7/ (for browsing the source)
- https://sources.debian.net/src/libtext-wrapi18n-perl/0.06-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtext-wrapi18n-perl/0.06-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libthai=0.1.21-1`

Binary Packages:

- `libthai-data=0.1.21-1`
- `libthai0:amd64=0.1.21-1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.21-1
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.21-1.dsc' libthai_0.1.21-1.dsc 2161 SHA256:ad9171fb789a184ed1061ced80c453e6229d0b4b299d7e91fcb39655f5f29e83
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.21.orig.tar.xz' libthai_0.1.21.orig.tar.xz 385384 SHA256:ff0e41143a8be7e01a785778c2addae48945c8bad4a275d2135afec35959fae3
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.21-1.debian.tar.xz' libthai_0.1.21-1.debian.tar.xz 10024 SHA256:5ad02dcfe536379884f43b1a540c641567a29a17ef6d3fcceb814c67bd2959b3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libthai/0.1.21-1/ (for browsing the source)
- https://sources.debian.net/src/libthai/0.1.21-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libthai/0.1.21-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtimedate-perl=2.3000-2`

Binary Packages:

- `libtimedate-perl=2.3000-2`

Licenses: (parsed from: `/usr/share/doc/libtimedate-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libtimedate-perl=2.3000-2
'http://deb.debian.org/debian/pool/main/libt/libtimedate-perl/libtimedate-perl_2.3000-2.dsc' libtimedate-perl_2.3000-2.dsc 2136 SHA256:0d7961456d3d45cd1c0e6b4a39ed56290d0722d9e44e3b75645f6608c15455f5
'http://deb.debian.org/debian/pool/main/libt/libtimedate-perl/libtimedate-perl_2.3000.orig.tar.gz' libtimedate-perl_2.3000.orig.tar.gz 31109 SHA256:75bd254871cb5853a6aa0403ac0be270cdd75c9d1b6639f18ecba63c15298e86
'http://deb.debian.org/debian/pool/main/libt/libtimedate-perl/libtimedate-perl_2.3000-2.debian.tar.xz' libtimedate-perl_2.3000-2.debian.tar.xz 4580 SHA256:092bd262925ed3677fabbfd867ffdc6b5b8ead2ffe2fca912cd20651bca2e2cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtimedate-perl/2.3000-2/ (for browsing the source)
- https://sources.debian.net/src/libtimedate-perl/2.3000-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtimedate-perl/2.3000-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtool=2.4.2-1.11`

Binary Packages:

- `libltdl-dev:amd64=2.4.2-1.11+b1`
- `libltdl7:amd64=2.4.2-1.11+b1`
- `libtool=2.4.2-1.11`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.2-1.11
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.2-1.11.dsc' libtool_2.4.2-1.11.dsc 1467 SHA256:155ccf84638725c278b641fbd1c5c76a98d612cacf00f5f00a10f8e6826e643f
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.2.orig.tar.gz' libtool_2.4.2.orig.tar.gz 2632347 SHA256:b38de44862a987293cd3d8dfae1c409d514b6c4e794ebc93648febf9afc38918
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.2-1.11.debian.tar.xz' libtool_2.4.2-1.11.debian.tar.xz 17408 SHA256:524c916ae9bdf39311aa9e713024ca7b48b0367481c8e6217f407e194e908a7b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtool/2.4.2-1.11/ (for browsing the source)
- https://sources.debian.net/src/libtool/2.4.2-1.11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtool/2.4.2-1.11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libusb=2:0.1.12-25`

Binary Packages:

- `libusb-0.1-4:amd64=2:0.1.12-25`

Licenses: (parsed from: `/usr/share/doc/libusb-0.1-4/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libusb=2:0.1.12-25
'http://deb.debian.org/debian/pool/main/libu/libusb/libusb_0.1.12-25.dsc' libusb_0.1.12-25.dsc 1958 SHA256:905e7cc36c9ba24f6d58e416f8882bc2522673cfb9f63687b48c62c9e3b6c80c
'http://deb.debian.org/debian/pool/main/libu/libusb/libusb_0.1.12.orig.tar.gz' libusb_0.1.12.orig.tar.gz 389343 SHA256:37f6f7d9de74196eb5fc0bbe0aea9b5c939de7f500acba3af6fd643f3b538b44
'http://deb.debian.org/debian/pool/main/libu/libusb/libusb_0.1.12-25.debian.tar.xz' libusb_0.1.12-25.debian.tar.xz 22008 SHA256:9e42ea2a8e0ec85b13cb8c9df7dc3aff58ee82e3692a7656558ae91ceeabf7d1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libusb/2:0.1.12-25/ (for browsing the source)
- https://sources.debian.net/src/libusb/2:0.1.12-25/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libusb/2:0.1.12-25/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvpx=1.3.0-3+deb8u3`

Binary Packages:

- `libvpx1:amd64=1.3.0-3+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libvpx1/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libvpx=1.3.0-3+deb8u3
'http://security.debian.org/debian-security/pool/updates/main/libv/libvpx/libvpx_1.3.0-3+deb8u3.dsc' libvpx_1.3.0-3+deb8u3.dsc 2041 SHA256:b9be36d941f9b1b64d80dddfe17a35bfc239384c0f34308d4769b1ad3df4b69a
'http://security.debian.org/debian-security/pool/updates/main/libv/libvpx/libvpx_1.3.0.orig.tar.bz2' libvpx_1.3.0.orig.tar.bz2 2077846 SHA256:bd5af97b74d53a111b48852dfcd1791b2c758f1fe972833b363fe34a83a7750a
'http://security.debian.org/debian-security/pool/updates/main/libv/libvpx/libvpx_1.3.0-3+deb8u3.debian.tar.xz' libvpx_1.3.0-3+deb8u3.debian.tar.xz 13144 SHA256:5b7d62567f4bfb357a9344815b4cef5416c7bee82832ec6671340f6bba083182
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvpx/1.3.0-3+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/libvpx/1.3.0-3+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvpx/1.3.0-3+deb8u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwebp=0.4.1-1.2`

Binary Packages:

- `libwebp-dev:amd64=0.4.1-1.2+b2`
- `libwebp5:amd64=0.4.1-1.2+b2`
- `libwebpdemux1:amd64=0.4.1-1.2+b2`
- `libwebpmux1:amd64=0.4.1-1.2+b2`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp5/copyright`, `/usr/share/doc/libwebpdemux1/copyright`, `/usr/share/doc/libwebpmux1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.4.1-1.2
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.4.1-1.2.dsc' libwebp_0.4.1-1.2.dsc 2070 SHA256:8dd2b0c27d80c56934433512db1a11ef16a2871edf0bdc91753ce16e3e9dfb2a
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.4.1.orig.tar.gz' libwebp_0.4.1.orig.tar.gz 966358 SHA256:00b646e6f66550a8faa998711fe70aabee9ed3bc562a8437c89042901674d027
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.4.1-1.2.debian.tar.xz' libwebp_0.4.1-1.2.debian.tar.xz 4328 SHA256:5e8f7c18da9a6da0c839864a583c76d7831fdfe89847170186d44404b80e37e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwebp/0.4.1-1.2/ (for browsing the source)
- https://sources.debian.net/src/libwebp/0.4.1-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwebp/0.4.1-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwmf=0.2.8.4-10.3+deb8u2`

Binary Packages:

- `libwmf-dev=0.2.8.4-10.3+deb8u2`
- `libwmf0.2-7:amd64=0.2.8.4-10.3+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-10.3+deb8u2
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.8.4-10.3+deb8u2.dsc' libwmf_0.2.8.4-10.3+deb8u2.dsc 2094 SHA256:6ade76bd09b35003d47c14159dacd1682ce167354b2eb7360cb9a5751e86e527
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://deb.debian.org/debian/pool/main/libw/libwmf/libwmf_0.2.8.4-10.3+deb8u2.debian.tar.xz' libwmf_0.2.8.4-10.3+deb8u2.debian.tar.xz 11236 SHA256:fb9cbf819c377c229153b16f8a1b3b9b029d7d4ef61360108654bcf8612ae95d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwmf/0.2.8.4-10.3+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/libwmf/0.2.8.4-10.3+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwmf/0.2.8.4-10.3+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.6.2-3+deb8u2`

Binary Packages:

- `libx11-6:amd64=2:1.6.2-3+deb8u2`
- `libx11-data=2:1.6.2-3+deb8u2`
- `libx11-dev:amd64=2:1.6.2-3+deb8u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.2-3+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/libx/libx11/libx11_1.6.2-3+deb8u2.dsc' libx11_1.6.2-3+deb8u2.dsc 2688 SHA256:2a1f803b76d186b025d6c66172e2e6865cc5b65c7f03a0cdcece166f7cfdcfa6
'http://security.debian.org/debian-security/pool/updates/main/libx/libx11/libx11_1.6.2.orig.tar.gz' libx11_1.6.2.orig.tar.gz 3119924 SHA256:b93739bcd517723121f508bcaf0c213c1bae9c5eacffdca571ff0d86c30ead3e
'http://security.debian.org/debian-security/pool/updates/main/libx/libx11/libx11_1.6.2-3+deb8u2.diff.gz' libx11_1.6.2-3+deb8u2.diff.gz 75641 SHA256:04a564142214edc6e3f0817eccb1c6f6263c882731b6c1d1eeddf57de7ed55c2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.6.2-3+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.6.2-3+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.6.2-3+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxau=1:1.0.8-1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.8-1`
- `libxau6:amd64=1:1.0.8-1`

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

### `dpkg` source package: `libxcb=1.10-3`

Binary Packages:

- `libxcb-render0:amd64=1.10-3+b1`
- `libxcb-render0-dev:amd64=1.10-3+b1`
- `libxcb-shm0:amd64=1.10-3+b1`
- `libxcb-shm0-dev:amd64=1.10-3+b1`
- `libxcb1:amd64=1.10-3+b1`
- `libxcb1-dev:amd64=1.10-3+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.10-3
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.10-3.dsc' libxcb_1.10-3.dsc 6940 SHA256:d9915049a5efb76badb8c05d1cf2cdc695910cae5c1c4719a37be1256abdbeab
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.10.orig.tar.gz' libxcb_1.10.orig.tar.gz 601241 SHA256:c4cd324ac7bf810e95b1c1b56f413b13850eaa1d7eca60ddc46c61ac9d5f4441
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.10-3.diff.gz' libxcb_1.10-3.diff.gz 24425 SHA256:c9c6dc0fedfe20e4a00dc96cb37dfe96ee2980063e941a07f0758b3e6bec57cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcb/1.10-3/ (for browsing the source)
- https://sources.debian.net/src/libxcb/1.10-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcb/1.10-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdmcp=1:1.1.1-1+deb8u1`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.1-1+deb8u1`
- `libxdmcp6:amd64=1:1.1.1-1+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.1-1+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/libx/libxdmcp/libxdmcp_1.1.1-1+deb8u1.dsc' libxdmcp_1.1.1-1+deb8u1.dsc 2330 SHA256:5d04cc119c583c4f4a36aabb321479756ca5f9dd3653ba0f3d2fe5ea4b281964
'http://security.debian.org/debian-security/pool/updates/main/libx/libxdmcp/libxdmcp_1.1.1.orig.tar.gz' libxdmcp_1.1.1.orig.tar.gz 376525 SHA256:ae6e677911e2696a2976b2f565f116ba9ce99e89cc7e140c4a791270c3aff96f
'http://security.debian.org/debian-security/pool/updates/main/libx/libxdmcp/libxdmcp_1.1.1-1+deb8u1.diff.gz' libxdmcp_1.1.1-1+deb8u1.diff.gz 15593 SHA256:08c77d8e489f8d7986188276b5cc85a5d2df8eb2ecf1f6c3612c7569507e24c2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxdmcp/1:1.1.1-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libxdmcp/1:1.1.1-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxdmcp/1:1.1.1-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.3-1`
- `libxext6:amd64=2:1.3.3-1`

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

### `dpkg` source package: `libxml2=2.9.1+dfsg1-5+deb8u8`

Binary Packages:

- `libxml2:amd64=2.9.1+dfsg1-5+deb8u8`
- `libxml2-dev:amd64=2.9.1+dfsg1-5+deb8u8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.1+dfsg1-5+deb8u8
'http://security.debian.org/debian-security/pool/updates/main/libx/libxml2/libxml2_2.9.1+dfsg1-5+deb8u8.dsc' libxml2_2.9.1+dfsg1-5+deb8u8.dsc 2605 SHA256:0e4f410941b3fa5ad759c0c8d2d583bd3b7eb75efe13f7be92887c848ded125e
'http://security.debian.org/debian-security/pool/updates/main/libx/libxml2/libxml2_2.9.1+dfsg1.orig.tar.gz' libxml2_2.9.1+dfsg1.orig.tar.gz 3793894 SHA256:f3ec5256412192f74833286c4490672500b232ed1c9195214db2c641df064a28
'http://security.debian.org/debian-security/pool/updates/main/libx/libxml2/libxml2_2.9.1+dfsg1-5+deb8u8.debian.tar.xz' libxml2_2.9.1+dfsg1-5+deb8u8.debian.tar.xz 72004 SHA256:916a77bcafaea6720f9792aa5bb143aabd57733024f66129460de2b59c3a7706
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxml2/2.9.1+dfsg1-5+deb8u8/ (for browsing the source)
- https://sources.debian.net/src/libxml2/2.9.1+dfsg1-5+deb8u8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxml2/2.9.1+dfsg1-5+deb8u8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxpm=1:3.5.12-0+deb8u1`

Binary Packages:

- `libxpm4:amd64=1:3.5.12-0+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxpm=1:3.5.12-0+deb8u1
'http://deb.debian.org/debian/pool/main/libx/libxpm/libxpm_3.5.12-0+deb8u1.dsc' libxpm_3.5.12-0+deb8u1.dsc 2309 SHA256:e7e77c196f043ab06cf27cfce298aa8e9692bbf4976552e3a4571dc99a982c56
'http://deb.debian.org/debian/pool/main/libx/libxpm/libxpm_3.5.12.orig.tar.gz' libxpm_3.5.12.orig.tar.gz 529302 SHA256:2523acc780eac01db5163267b36f5b94374bfb0de26fc0b5a7bee76649fd8501
'http://deb.debian.org/debian/pool/main/libx/libxpm/libxpm_3.5.12-0+deb8u1.diff.gz' libxpm_3.5.12-0+deb8u1.diff.gz 15312 SHA256:398d880297c9082a88507f41f19dde5aaf55fac973d55053a746e018ac260b1e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxpm/1:3.5.12-0+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libxpm/1:3.5.12-0+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxpm/1:3.5.12-0+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxrender=1:0.9.8-1`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.8-1+b1`
- `libxrender1:amd64=1:0.9.8-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.8-1
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.8-1.dsc' libxrender_0.9.8-1.dsc 2161 SHA256:af7f6e3d257cc75eb70fc964d8db281d69eb204f0c9af7677419c8462a90e69f
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.8.orig.tar.gz' libxrender_0.9.8.orig.tar.gz 363551 SHA256:c3acffff4cd5c91585e8c4fdf1ec29fc234482f661ed548112b4d52db19963d1
'http://deb.debian.org/debian/pool/main/libx/libxrender/libxrender_0.9.8-1.diff.gz' libxrender_0.9.8-1.diff.gz 18898 SHA256:e3d0fe59c5bb680e0fd1e115c54a6cb2fa2c9fe208679b7fbe7b8de7040ffe16
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxrender/1:0.9.8-1/ (for browsing the source)
- https://sources.debian.net/src/libxrender/1:0.9.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxrender/1:0.9.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxslt=1.1.28-2+deb8u6`

Binary Packages:

- `libxslt1-dev:amd64=1.1.28-2+deb8u6`
- `libxslt1.1:amd64=1.1.28-2+deb8u6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.28-2+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/libx/libxslt/libxslt_1.1.28-2+deb8u6.dsc' libxslt_1.1.28-2+deb8u6.dsc 2554 SHA256:ff3073e4ee00c3b3a43867e65c69886c104ce71cd02d0960610345a00f974e66
'http://security.debian.org/debian-security/pool/updates/main/libx/libxslt/libxslt_1.1.28.orig.tar.gz' libxslt_1.1.28.orig.tar.gz 3435907 SHA256:5fc7151a57b89c03d7b825df5a0fae0a8d5f05674c0e7cf2937ecec4d54a028c
'http://security.debian.org/debian-security/pool/updates/main/libx/libxslt/libxslt_1.1.28-2+deb8u6.debian.tar.xz' libxslt_1.1.28-2+deb8u6.debian.tar.xz 41288 SHA256:43c944cc8671b1ba89b34d385629baa276cf5d58d48d5c70403ec4b95e564658
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxslt/1.1.28-2+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/libxslt/1.1.28-2+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxslt/1.1.28-2+deb8u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxt=1:1.1.4-1`

Binary Packages:

- `libxt-dev:amd64=1:1.1.4-1+b1`
- `libxt6:amd64=1:1.1.4-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.1.4-1
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.4-1.dsc' libxt_1.1.4-1.dsc 2130 SHA256:2158838b3cc889d51bc267c2a1832b753a38a507b22274daa5b9341d88b2109e
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.4.orig.tar.gz' libxt_1.1.4.orig.tar.gz 950463 SHA256:823109a0d14dfaef7ede1b3fd28318078daa2cc2f005c439a21c33bdac3d3784
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.1.4-1.diff.gz' libxt_1.1.4-1.diff.gz 11246 SHA256:4414e80a2d36a7122de644d3fe67dadbd12a636d80366eda9b6840f1c7d328bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxt/1:1.1.4-1/ (for browsing the source)
- https://sources.debian.net/src/libxt/1:1.1.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxt/1:1.1.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libyaml=0.1.6-3`

Binary Packages:

- `libyaml-0-2:amd64=0.1.6-3`
- `libyaml-dev:amd64=0.1.6-3`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.1.6-3
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.1.6-3.dsc' libyaml_0.1.6-3.dsc 1893 SHA256:ed5bc299d3bcc0b038206f8780639d4682e65f521dff571b9336e2f8626d0011
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.1.6.orig.tar.gz' libyaml_0.1.6.orig.tar.gz 503012 SHA256:7da6971b4bd08a986dd2a61353bc422362bd0edcc67d7ebaac68c95f74182749
'http://deb.debian.org/debian/pool/main/liby/libyaml/libyaml_0.1.6-3.debian.tar.xz' libyaml_0.1.6-3.debian.tar.xz 4268 SHA256:fd567e6918903833e5c4f1f87254c550eca07c2bba1ccbe6031da33243cf4297
```

Other potentially useful URLs:

- https://sources.debian.net/src/libyaml/0.1.6-3/ (for browsing the source)
- https://sources.debian.net/src/libyaml/0.1.6-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libyaml/0.1.6-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `linux=3.16.84-1`

Binary Packages:

- `linux-libc-dev:amd64=3.16.84-1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`
- `Unicode-data`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=3.16.84-1
'http://security.debian.org/debian-security/pool/updates/main/l/linux/linux_3.16.84-1.dsc' linux_3.16.84-1.dsc 143027 SHA256:1181b4ab818eaca2a8d7de7d1a3b751077dc1389fcb1d8111924d5df36c7d720
'http://security.debian.org/debian-security/pool/updates/main/l/linux/linux_3.16.84.orig.tar.xz' linux_3.16.84.orig.tar.xz 82095884 SHA256:17f0a7a1c8279c971509801eef4f60af49f85fec41649cbec77bc95a5db887f9
'http://security.debian.org/debian-security/pool/updates/main/l/linux/linux_3.16.84-1.debian.tar.xz' linux_3.16.84-1.debian.tar.xz 1231412 SHA256:f8c5f05043084d4b1e6468fddaf471d61935a38f5f81357bd2b271481a567947
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/3.16.84-1/ (for browsing the source)
- https://sources.debian.net/src/linux/3.16.84-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/3.16.84-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lsb=4.1+Debian13+nmu1`

Binary Packages:

- `lsb-base=4.1+Debian13+nmu1`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=4.1+Debian13+nmu1
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_4.1+Debian13+nmu1.dsc' lsb_4.1+Debian13+nmu1.dsc 2449 SHA256:ef70a3302cf4b50c02ad3cfb90d7997968dd509dc0dbb77562b76f23b617c254
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_4.1+Debian13+nmu1.tar.xz' lsb_4.1+Debian13+nmu1.tar.xz 59880 SHA256:7f5fbd13c04de166d0f658c0b71ed97c3fe07e01e165f5c0bd68ff5977bee72d
```

Other potentially useful URLs:

- https://sources.debian.net/src/lsb/4.1+Debian13+nmu1/ (for browsing the source)
- https://sources.debian.net/src/lsb/4.1+Debian13+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lsb/4.1+Debian13+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lvm2=2.02.111-2.2+deb8u1`

Binary Packages:

- `dmsetup=2:1.02.90-2.2+deb8u1`
- `libdevmapper1.02.1:amd64=2:1.02.90-2.2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/dmsetup/copyright`, `/usr/share/doc/libdevmapper1.02.1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris lvm2=2.02.111-2.2+deb8u1
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.111-2.2+deb8u1.dsc' lvm2_2.02.111-2.2+deb8u1.dsc 2474 SHA256:9e67627d50ef43b88f29a42b5ff4d48b0bfeeb35d98c09da33c6ce51e99c5d96
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.111.orig.tar.gz' lvm2_2.02.111.orig.tar.gz 1497626 SHA256:ff358054ee821503ada8a33b327688cd4d64a2fc448c667a85c332c545aae4f6
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.111-2.2+deb8u1.debian.tar.xz' lvm2_2.02.111-2.2+deb8u1.debian.tar.xz 29476 SHA256:df657682e06f9559d04719c1543285e8bcb51fb4647f673b787538fb34ebe26f
```

Other potentially useful URLs:

- https://sources.debian.net/src/lvm2/2.02.111-2.2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/lvm2/2.02.111-2.2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lvm2/2.02.111-2.2+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lzo2=2.08-1.2`

Binary Packages:

- `liblzo2-2:amd64=2.08-1.2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.08-1.2
'http://deb.debian.org/debian/pool/main/l/lzo2/lzo2_2.08-1.2.dsc' lzo2_2.08-1.2.dsc 1804 SHA256:09eabe81d6f631a29cc603843b27ab914704726a1400a2219cf83b1da4e72892
'http://deb.debian.org/debian/pool/main/l/lzo2/lzo2_2.08.orig.tar.gz' lzo2_2.08.orig.tar.gz 589045 SHA256:ac1b3e4dee46febe9fd28737eb7f5692d3232ef1a01da10444394c3d47536614
'http://deb.debian.org/debian/pool/main/l/lzo2/lzo2_2.08-1.2.debian.tar.xz' lzo2_2.08-1.2.debian.tar.xz 5996 SHA256:5a9aa3a2432f5d4f689b24c64ea3daec7646e736da37721388ae88b670dd99bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/lzo2/2.08-1.2/ (for browsing the source)
- https://sources.debian.net/src/lzo2/2.08-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lzo2/2.08-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `m4=1.4.17-4`

Binary Packages:

- `m4=1.4.17-4`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.17-4
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.17-4.dsc' m4_1.4.17-4.dsc 1412 SHA256:5b668aa9c59b053a1ff7a7bccda986f2d4cf1702e42d80cace78eeced9518ef8
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.17.orig.tar.xz' m4_1.4.17.orig.tar.xz 1149088 SHA256:f0543c3beb51fa6b3337d8025331591e0e18d8ec2886ed391f1aade43477d508
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.17-4.debian.tar.xz' m4_1.4.17-4.debian.tar.xz 9572 SHA256:6ceab2d3c2d1d7a7ab083b134df1aaf083f93b0ac1346a4eeb5dafbdc9418a06
```

Other potentially useful URLs:

- https://sources.debian.net/src/m4/1.4.17-4/ (for browsing the source)
- https://sources.debian.net/src/m4/1.4.17-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/m4/1.4.17-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `make-dfsg=4.0-8.1`

Binary Packages:

- `make=4.0-8.1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.0-8.1
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.0-8.1.dsc' make-dfsg_4.0-8.1.dsc 2021 SHA256:ae258d9abb68e756d1ff5195dc3060748b3d4b019ccce19a249d4de23039a0ce
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.0.orig.tar.gz' make-dfsg_4.0.orig.tar.gz 1401242 SHA256:6916aa026d930cfc5a4f93aba24fc231d47a0486c3b8e5b69112dd1f7b81c4fe
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.0-8.1.debian.tar.xz' make-dfsg_4.0-8.1.debian.tar.xz 42200 SHA256:3cf5a779102c7acb3a00711a417aab85618c8da4d3f1d04bf85b2d95c4a98f09
```

Other potentially useful URLs:

- https://sources.debian.net/src/make-dfsg/4.0-8.1/ (for browsing the source)
- https://sources.debian.net/src/make-dfsg/4.0-8.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/make-dfsg/4.0-8.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mawk=1.3.3-17`

Binary Packages:

- `mawk=1.3.3-17`

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

### `dpkg` source package: `mercurial=3.1.2-2+deb8u7`

Binary Packages:

- `mercurial=3.1.2-2+deb8u7`
- `mercurial-common=3.1.2-2+deb8u7`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=3.1.2-2+deb8u7
'http://security.debian.org/debian-security/pool/updates/main/m/mercurial/mercurial_3.1.2-2+deb8u7.dsc' mercurial_3.1.2-2+deb8u7.dsc 2287 SHA256:33a015ea156747c770ca254e17b9871c779db15be9e6b6aa679d7496140bce28
'http://security.debian.org/debian-security/pool/updates/main/m/mercurial/mercurial_3.1.2.orig.tar.gz' mercurial_3.1.2.orig.tar.gz 3983825 SHA256:5dbe5ceb3707e378528dc9346af280919760aa1a8bcc27be12c1fe2bafa78d3a
'http://security.debian.org/debian-security/pool/updates/main/m/mercurial/mercurial_3.1.2-2+deb8u7.debian.tar.xz' mercurial_3.1.2-2+deb8u7.debian.tar.xz 74408 SHA256:5193356d426b700e7d402eb9e591c729ecf59567f28234c87a5a664cf8769678
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/3.1.2-2+deb8u7/ (for browsing the source)
- https://sources.debian.net/src/mercurial/3.1.2-2+deb8u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/3.1.2-2+deb8u7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mime-support=3.58`

Binary Packages:

- `mime-support=3.58`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.58
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.58.dsc' mime-support_3.58.dsc 1604 SHA256:3279480870a7bd6c7e2a85f7f1e5deba50c3cb5edcbd6ce69a3cfc7fe0266284
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.58.tar.gz' mime-support_3.58.tar.gz 34995 SHA256:3d9ca5115e93edb3ada3fb120cde88ac3d866903e18a41ca124428d77dd1721e
```

Other potentially useful URLs:

- https://sources.debian.net/src/mime-support/3.58/ (for browsing the source)
- https://sources.debian.net/src/mime-support/3.58/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mime-support/3.58/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpclib3=1.0.2-1`

Binary Packages:

- `libmpc3:amd64=1.0.2-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.0.2-1
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.0.2-1.dsc' mpclib3_1.0.2-1.dsc 1239 SHA256:480e3b32fe3c67b503635d2a0aa0e87503475cf54ddf7943be0255e453c42fe5
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.0.2.orig.tar.gz' mpclib3_1.0.2.orig.tar.gz 633173 SHA256:b561f54d8a479cee3bc891ee52735f18ff86712ba30f036f8b8537bae380c488
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.0.2-1.diff.gz' mpclib3_1.0.2-1.diff.gz 3370 SHA256:22e1db34773adaf27cc16a2260ae4e8f22cc80476b861a0856f93aa08ec8cc91
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpclib3/1.0.2-1/ (for browsing the source)
- https://sources.debian.net/src/mpclib3/1.0.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpclib3/1.0.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpfr4=3.1.2-2`

Binary Packages:

- `libmpfr4:amd64=3.1.2-2`

Licenses: (parsed from: `/usr/share/doc/libmpfr4/copyright`)

- `GFDL`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=3.1.2-2
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_3.1.2-2.dsc' mpfr4_3.1.2-2.dsc 2116 SHA256:fcbf025b0daf6dc95715ac226d4e4a8f86cda4b796115ad5b9d8271da6de9c7b
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_3.1.2.orig.tar.xz' mpfr4_3.1.2.orig.tar.xz 1074388 SHA256:399d0f47ef6608cc01d29ed1b99c7faff36d9994c45f36f41ba250147100453b
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_3.1.2-2.debian.tar.xz' mpfr4_3.1.2-2.debian.tar.xz 12804 SHA256:49efd1d2032c8576868b64419e3403869dd5a62e1974b341f836852f7f2fd097
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpfr4/3.1.2-2/ (for browsing the source)
- https://sources.debian.net/src/mpfr4/3.1.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpfr4/3.1.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mysql-5.5=5.5.62-0+deb8u1`

Binary Packages:

- `libmysqlclient-dev=5.5.62-0+deb8u1`
- `libmysqlclient18:amd64=5.5.62-0+deb8u1`
- `mysql-common=5.5.62-0+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libmysqlclient-dev/copyright`, `/usr/share/doc/libmysqlclient18/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `Artistic`
- `BSD (2 clause)`
- `BSD (3 clause)`
- `BSD (4 clause)`
- `BSD-like`
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
$ apt-get source -qq --print-uris mysql-5.5=5.5.62-0+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/m/mysql-5.5/mysql-5.5_5.5.62-0+deb8u1.dsc' mysql-5.5_5.5.62-0+deb8u1.dsc 3107 SHA256:2c8f0559cbc3f16644987e19fcf5a7e503bbbb959e88847c8d3cf9a669fa260b
'http://security.debian.org/debian-security/pool/updates/main/m/mysql-5.5/mysql-5.5_5.5.62.orig.tar.gz' mysql-5.5_5.5.62.orig.tar.gz 21111902 SHA256:b1e7853bc1f04aabf6771e0ad947f35ac8d237f4b35d0706d1095c9526ff99d7
'http://security.debian.org/debian-security/pool/updates/main/m/mysql-5.5/mysql-5.5_5.5.62-0+deb8u1.debian.tar.xz' mysql-5.5_5.5.62-0+deb8u1.debian.tar.xz 232748 SHA256:914f49ce61764c2dd375943287e4ffdbfb46011bc5d30f55a4accf3d6a7cbde6
```

Other potentially useful URLs:

- https://sources.debian.net/src/mysql-5.5/5.5.62-0+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/mysql-5.5/5.5.62-0+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mysql-5.5/5.5.62-0+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=5.9+20140913-1+deb8u3`

Binary Packages:

- `libncurses5:amd64=5.9+20140913-1+deb8u3`
- `libncurses5-dev:amd64=5.9+20140913-1+deb8u3`
- `libncursesw5:amd64=5.9+20140913-1+deb8u3`
- `libncursesw5-dev:amd64=5.9+20140913-1+deb8u3`
- `libtinfo-dev:amd64=5.9+20140913-1+deb8u3`
- `libtinfo5:amd64=5.9+20140913-1+deb8u3`
- `ncurses-base=5.9+20140913-1+deb8u3`
- `ncurses-bin=5.9+20140913-1+deb8u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=5.9+20140913-1+deb8u3
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_5.9+20140913-1+deb8u3.dsc' ncurses_5.9+20140913-1+deb8u3.dsc 3505 SHA256:a4136ac92fd361e7b3c61f7e5a08e145841d960b2feefe014174f8109a997f0b
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_5.9+20140913.orig.tar.gz' ncurses_5.9+20140913.orig.tar.gz 2987249 SHA256:c4247ad81ee9d743caba8a2db6dd96d36878530b2e76e376af1c00b067a2dec9
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_5.9+20140913-1+deb8u3.debian.tar.xz' ncurses_5.9+20140913-1+deb8u3.debian.tar.xz 57136 SHA256:5edac557abf72e2f22c37423a9c8441f4da4509506e01b59b71d5120bd21a8ea
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/5.9+20140913-1+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/ncurses/5.9+20140913-1+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/5.9+20140913-1+deb8u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `netbase=5.3`

Binary Packages:

- `netbase=5.3`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.3
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.3.dsc' netbase_5.3.dsc 1308 SHA256:fcb9c97fe55277f775fd5a39933ca0189b9a983c6cf1abc8184fc29b8e1d77cb
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.3.tar.xz' netbase_5.3.tar.xz 31292 SHA256:81f6c69795044d62b8ad959cf9daf049d0545fd466c52860ad3f933b1e97b88b
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/5.3/ (for browsing the source)
- https://sources.debian.net/src/netbase/5.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/5.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=2.7.1-5+deb8u2`

Binary Packages:

- `libhogweed2:amd64=2.7.1-5+deb8u2`
- `libnettle4:amd64=2.7.1-5+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libhogweed2/copyright`, `/usr/share/doc/libnettle4/copyright`)

- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1+`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=2.7.1-5+deb8u2
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_2.7.1-5+deb8u2.dsc' nettle_2.7.1-5+deb8u2.dsc 2078 SHA256:9169cedb90e4eb552f4383172b56107c4365a7a43769c9e6d113072abc975223
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_2.7.1.orig.tar.gz' nettle_2.7.1.orig.tar.gz 1558863 SHA256:bc71ebd43435537d767799e414fce88e521b7278d48c860651216e1fc6555b40
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_2.7.1-5+deb8u2.debian.tar.xz' nettle_2.7.1-5+deb8u2.debian.tar.xz 20496 SHA256:0edb103b1268e6b3e8909883c1e9c7416dd75a51c9116047ca60031377e01141
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/2.7.1-5+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/nettle/2.7.1-5+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/2.7.1-5+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openexr=1.6.1-8`

Binary Packages:

- `libopenexr-dev=1.6.1-8`
- `libopenexr6:amd64=1.6.1-8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openexr=1.6.1-8
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_1.6.1-8.dsc' openexr_1.6.1-8.dsc 2023 SHA256:ff2ea7bf8bfaaa2f320a2af786047bb42f3153e5a8ce8287bcedfb789dd78db3
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_1.6.1.orig.tar.gz' openexr_1.6.1.orig.tar.gz 13632660 SHA256:c616906ab958de9c37bb86ca7547cfedbdfbad5e1ca2a4ab98983c9afa6a5950
'http://deb.debian.org/debian/pool/main/o/openexr/openexr_1.6.1-8.debian.tar.xz' openexr_1.6.1-8.debian.tar.xz 13900 SHA256:9770c16dbd6082ef8fed710f067f0c36a774423b0d9a7d7eda2fcef9c34b44d1
```

Other potentially useful URLs:

- https://sources.debian.net/src/openexr/1.6.1-8/ (for browsing the source)
- https://sources.debian.net/src/openexr/1.6.1-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openexr/1.6.1-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.40+dfsg-1+deb8u6`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.40+dfsg-1+deb8u6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.40+dfsg-1+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/o/openldap/openldap_2.4.40+dfsg-1+deb8u6.dsc' openldap_2.4.40+dfsg-1+deb8u6.dsc 2835 SHA256:2d743d14044303954ed7abd9f24cbe333af4e97c38d78398178d1ca992b25f1d
'http://security.debian.org/debian-security/pool/updates/main/o/openldap/openldap_2.4.40+dfsg.orig.tar.gz' openldap_2.4.40+dfsg.orig.tar.gz 4797667 SHA256:86c0326dc3dc5f1a9b3c25f7106b96f3eafcdf5da090b1fc586dec57d56e0e7f
'http://security.debian.org/debian-security/pool/updates/main/o/openldap/openldap_2.4.40+dfsg-1+deb8u6.diff.gz' openldap_2.4.40+dfsg-1+deb8u6.diff.gz 185074 SHA256:559621ba5e00388e3663e025b93a579b56076219c217bfe1274caa2e767acc30
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.40+dfsg-1+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.40+dfsg-1+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.40+dfsg-1+deb8u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:6.7p1-5+deb8u8`

Binary Packages:

- `openssh-client=1:6.7p1-5+deb8u8`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:6.7p1-5+deb8u8
'http://security.debian.org/debian-security/pool/updates/main/o/openssh/openssh_6.7p1-5+deb8u8.dsc' openssh_6.7p1-5+deb8u8.dsc 2752 SHA256:c5f97a39da07b386f11cd0da09d6ca9915f6c33b62dab6b86abfa33499cd7f17
'http://security.debian.org/debian-security/pool/updates/main/o/openssh/openssh_6.7p1.orig.tar.gz' openssh_6.7p1.orig.tar.gz 1351367 SHA256:b2f8394eae858dabbdef7dac10b99aec00c95462753e80342e530bbb6f725507
'http://security.debian.org/debian-security/pool/updates/main/o/openssh/openssh_6.7p1-5+deb8u8.debian.tar.xz' openssh_6.7p1-5+deb8u8.debian.tar.xz 177024 SHA256:64a4d6fb4dd402bc95a23c3e3422ba177e3d59b294249fd80009b7d28f9810b0
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:6.7p1-5+deb8u8/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:6.7p1-5+deb8u8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:6.7p1-5+deb8u8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.0.1t-1+deb8u12`

Binary Packages:

- `libssl-dev:amd64=1.0.1t-1+deb8u12`
- `libssl1.0.0:amd64=1.0.1t-1+deb8u12`
- `openssl=1.0.1t-1+deb8u12`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.0.1t-1+deb8u12
'http://security.debian.org/debian-security/pool/updates/main/o/openssl/openssl_1.0.1t-1+deb8u12.dsc' openssl_1.0.1t-1+deb8u12.dsc 2427 SHA256:224da86e423639a661759e10d07e344a4d969f3b9125518701b718f158da2228
'http://security.debian.org/debian-security/pool/updates/main/o/openssl/openssl_1.0.1t.orig.tar.gz' openssl_1.0.1t.orig.tar.gz 4556447 SHA256:4a6ee491a2fdb22e519c76fdc2a628bb3cec12762cd456861d207996c8a07088
'http://security.debian.org/debian-security/pool/updates/main/o/openssl/openssl_1.0.1t-1+deb8u12.debian.tar.xz' openssl_1.0.1t-1+deb8u12.debian.tar.xz 118796 SHA256:28bcb0510fe598a7ba4b2d6e6241f8e7d9d22d142a4cd1cd8e9d23a73a6ad0b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.0.1t-1+deb8u12/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.0.1t-1+deb8u12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.0.1t-1+deb8u12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.20.7-1`

Binary Packages:

- `libp11-kit0:amd64=0.20.7-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `This file is distributed under the same license as the debian`
- `This file is distributed under the same license as the p11-kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.20.7-1
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.20.7-1.dsc' p11-kit_0.20.7-1.dsc 2221 SHA256:459d56241f560163471eb5ec789eb5691ca97c5aa9a1bca98dabcf613a2d4bc3
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.20.7.orig.tar.gz' p11-kit_0.20.7.orig.tar.gz 986731 SHA256:68405492fe466b33927d461302aa98e703db3b8a596411585508bc33084484d2
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.20.7-1.debian.tar.xz' p11-kit_0.20.7-1.debian.tar.xz 14208 SHA256:515dfcc279d284bfbee4d172c9cf1db3befe52d55e6d3f50d024c8f72d56574d
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.20.7-1/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.20.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.20.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.1.8-3.1+deb8u2`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.1+deb8u2+b1`
- `libpam-modules-bin=1.1.8-3.1+deb8u2+b1`
- `libpam-runtime=1.1.8-3.1+deb8u2`
- `libpam0g:amd64=1.1.8-3.1+deb8u2+b1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.1+deb8u2
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.1+deb8u2.dsc' pam_1.1.8-3.1+deb8u2.dsc 2504 SHA256:0dcab55550af17b5f2779b5749930a69ea54302d8f8ef1bdd1a8dea3ed4e0619
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8.orig.tar.gz' pam_1.1.8.orig.tar.gz 1892765 SHA256:4183409a450708a976eca5af561dbf4f0490141a08e86e4a1e649c7c1b094876
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.1.8-3.1+deb8u2.diff.gz' pam_1.1.8-3.1+deb8u2.diff.gz 134897 SHA256:84a455ce53c7701d2a536fc33909a6ce19c1a6b7c18e6be8d2d0fc2294260610
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.1.8-3.1+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/pam/1.1.8-3.1+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.1.8-3.1+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pango1.0=1.36.8-3`

Binary Packages:

- `libpango-1.0-0:amd64=1.36.8-3`
- `libpangocairo-1.0-0:amd64=1.36.8-3`
- `libpangoft2-1.0-0:amd64=1.36.8-3`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.36.8-3
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.36.8-3.dsc' pango1.0_1.36.8-3.dsc 3169 SHA256:8a0e51c2c4a33e4136dd4cabe670b265e48cf92e740d6d9889623c2183940a1e
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.36.8.orig.tar.xz' pango1.0_1.36.8.orig.tar.xz 1033528 SHA256:18dbb51b8ae12bae0ab7a958e7cf3317c9acfc8a1e1103ec2f147164a0fc2d07
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.36.8-3.debian.tar.xz' pango1.0_1.36.8-3.debian.tar.xz 31668 SHA256:4249e9e29a186994abe8d5d57debc81c446916a6c7ea872171597c4df4d8f6ea
```

Other potentially useful URLs:

- https://sources.debian.net/src/pango1.0/1.36.8-3/ (for browsing the source)
- https://sources.debian.net/src/pango1.0/1.36.8-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pango1.0/1.36.8-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `patch=2.7.5-1+deb8u3`

Binary Packages:

- `patch=2.7.5-1+deb8u3`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.5-1+deb8u3
'http://security.debian.org/debian-security/pool/updates/main/p/patch/patch_2.7.5-1+deb8u3.dsc' patch_2.7.5-1+deb8u3.dsc 2019 SHA256:473fdf97f57e584799c72150397562d16bb1b8aa728a299f3b3d8c90ab7c6c47
'http://security.debian.org/debian-security/pool/updates/main/p/patch/patch_2.7.5.orig.tar.xz' patch_2.7.5.orig.tar.xz 727704 SHA256:fd95153655d6b95567e623843a0e77b81612d502ecf78a489a4aed7867caa299
'http://security.debian.org/debian-security/pool/updates/main/p/patch/patch_2.7.5-1+deb8u3.debian.tar.xz' patch_2.7.5-1+deb8u3.debian.tar.xz 11976 SHA256:fa8c2a0814ce98a4db137ea9859a60487cd5027bf259ae8d0a7b474a8d68791b
```

Other potentially useful URLs:

- https://sources.debian.net/src/patch/2.7.5-1+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/patch/2.7.5-1+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/patch/2.7.5-1+deb8u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.35-3.3+deb8u4`

Binary Packages:

- `libpcre3:amd64=2:8.35-3.3+deb8u4`
- `libpcre3-dev:amd64=2:8.35-3.3+deb8u4`
- `libpcrecpp0:amd64=2:8.35-3.3+deb8u4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.35-3.3+deb8u4
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.35-3.3+deb8u4.dsc' pcre3_8.35-3.3+deb8u4.dsc 1985 SHA256:862ee7365c8cc9916f58856617701e2e2f3dcd384a34375379ddfa52b642c649
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.35.orig.tar.gz' pcre3_8.35.orig.tar.gz 1996552 SHA256:1c9ee292943ba2737f127b481a3f72f44c13fbd09a7b5b4eb8fa58650cfa56a0
'http://deb.debian.org/debian/pool/main/p/pcre3/pcre3_8.35-3.3+deb8u4.debian.tar.gz' pcre3_8.35-3.3+deb8u4.debian.tar.gz 38081 SHA256:93e38ad38d4cdb21d346226eebc7e2ad419cbfe0261b27d2910e8e5c3a946fb9
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre3/2:8.35-3.3+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/pcre3/2:8.35-3.3+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre3/2:8.35-3.3+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.20.2-3+deb8u12`

Binary Packages:

- `perl=5.20.2-3+deb8u12`
- `perl-base=5.20.2-3+deb8u12`
- `perl-modules=5.20.2-3+deb8u12`

Licenses: (parsed from: `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules/copyright`)

- `Artistic`
- `Artistic,`
- `Artistic-2`
- `BSD-3-clause`
- `BSD-3-clause-GENERIC`
- `BSD-4-clause`
- `BSD-4-clause-POWERDOG`
- `BZIP`
- `DONT-CHANGE-THE-GPL`
- `Expat`
- `GPL-1`
- `GPL-1+`
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
$ apt-get source -qq --print-uris perl=5.20.2-3+deb8u12
'http://security.debian.org/debian-security/pool/updates/main/p/perl/perl_5.20.2-3+deb8u12.dsc' perl_5.20.2-3+deb8u12.dsc 2377 SHA256:b3e2ae82349e60575b28e62712e61aa1e862351e50eb7013004c75a951196cdb
'http://security.debian.org/debian-security/pool/updates/main/p/perl/perl_5.20.2.orig.tar.bz2' perl_5.20.2.orig.tar.bz2 13717128 SHA256:e5a4713bc65e1da98ebd833dce425c000768bfe84d17ec5183ec5ca249db71ab
'http://security.debian.org/debian-security/pool/updates/main/p/perl/perl_5.20.2-3+deb8u12.debian.tar.xz' perl_5.20.2-3+deb8u12.debian.tar.xz 158872 SHA256:b93b828b4ebd8171ca7ef5f8f195d529c368e83cd86f276d4a25470a6b7aaa6d
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.20.2-3+deb8u12/ (for browsing the source)
- https://sources.debian.net/src/perl/5.20.2-3+deb8u12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.20.2-3+deb8u12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pixman=0.32.6-3+deb8u1`

Binary Packages:

- `libpixman-1-0:amd64=0.32.6-3+deb8u1`
- `libpixman-1-dev=0.32.6-3+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.32.6-3+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/p/pixman/pixman_0.32.6-3+deb8u1.dsc' pixman_0.32.6-3+deb8u1.dsc 2205 SHA256:fee04be8aa089c32a66aeb17eda6bff21e135d03ed606c91a08a8ede7e67010f
'http://security.debian.org/debian-security/pool/updates/main/p/pixman/pixman_0.32.6.orig.tar.gz' pixman_0.32.6.orig.tar.gz 816702 SHA256:3dfed13b8060eadabf0a4945c7045b7793cc7e3e910e748a8bb0f0dc3e794904
'http://security.debian.org/debian-security/pool/updates/main/p/pixman/pixman_0.32.6-3+deb8u1.diff.gz' pixman_0.32.6-3+deb8u1.diff.gz 284680 SHA256:c36a6931b078c0e9db5e00984ddde4c80c4c294fb4f6bcf8e7704f0c05db7920
```

Other potentially useful URLs:

- https://sources.debian.net/src/pixman/0.32.6-3+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/pixman/0.32.6-3+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pixman/0.32.6-3+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pkg-config=0.28-1`

Binary Packages:

- `pkg-config=0.28-1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.28-1
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.28-1.dsc' pkg-config_0.28-1.dsc 1733 SHA256:d4a855310665e61dea83b858b70465cf7174797b322f75142863e9853ca35960
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.28.orig.tar.gz' pkg-config_0.28.orig.tar.gz 1931203 SHA256:6b6eb31c6ec4421174578652c7e141fdaae2dabad1021f420d8713206ac1f845
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.28-1.diff.gz' pkg-config_0.28-1.diff.gz 5942 SHA256:c5f6afcbadeded6a9cf192efc3bd882095e9ba73576de0544e393184e989992f
```

Other potentially useful URLs:

- https://sources.debian.net/src/pkg-config/0.28-1/ (for browsing the source)
- https://sources.debian.net/src/pkg-config/0.28-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pkg-config/0.28-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `postgresql-9.4=9.4.26-0+deb8u1`

Binary Packages:

- `libpq-dev=9.4.26-0+deb8u1`
- `libpq5:amd64=9.4.26-0+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libpq-dev/copyright`, `/usr/share/doc/libpq5/copyright`)

- `Tcl`
- `almost exclusively BSD`

Source:

```console
$ apt-get source -qq --print-uris postgresql-9.4=9.4.26-0+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/p/postgresql-9.4/postgresql-9.4_9.4.26-0+deb8u1.dsc' postgresql-9.4_9.4.26-0+deb8u1.dsc 3521 SHA256:e96f4d5be48b596e868dcb8b02596a68664db5242d8a75407945435ec34c0d0f
'http://security.debian.org/debian-security/pool/updates/main/p/postgresql-9.4/postgresql-9.4_9.4.26.orig.tar.bz2' postgresql-9.4_9.4.26.orig.tar.bz2 16871195 SHA256:f5c014fc4a5c94e8cf11314cbadcade4d84213cfcc82081c9123e1b8847a20b9
'http://security.debian.org/debian-security/pool/updates/main/p/postgresql-9.4/postgresql-9.4_9.4.26-0+deb8u1.debian.tar.xz' postgresql-9.4_9.4.26-0+deb8u1.debian.tar.xz 32408 SHA256:de260323c54611ca8d4af9f5e88358d3a684147f54caf8cec0b0fb099ec57ede
```

Other potentially useful URLs:

- https://sources.debian.net/src/postgresql-9.4/9.4.26-0+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/postgresql-9.4/9.4.26-0+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/postgresql-9.4/9.4.26-0+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.9-9+deb8u1`

Binary Packages:

- `libprocps3:amd64=2:3.3.9-9+deb8u1`
- `procps=2:3.3.9-9+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libprocps3/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.9-9+deb8u1
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.9-9+deb8u1.dsc' procps_3.3.9-9+deb8u1.dsc 2249 SHA256:1137afe6cd82a3f2f70402f6091c9f7a4898c6da9dcf4b89c39cb315e5432d16
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.9.orig.tar.xz' procps_3.3.9.orig.tar.xz 560812 SHA256:00f0cb0fadf968ddf605b0ef119846af07386629244d4f3da711a2cecf4e8663
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.9-9+deb8u1.debian.tar.xz' procps_3.3.9-9+deb8u1.debian.tar.xz 41180 SHA256:41aeb4ebb60ebad15e9c30fb736ee15b4a5d8045c39d3ecf31e8b1237752bc28
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.9-9+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.9-9+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.9-9+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python-defaults=2.7.9-1`

Binary Packages:

- `libpython-stdlib:amd64=2.7.9-1`
- `python=2.7.9-1`
- `python-minimal=2.7.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.9-1
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.9-1.dsc' python-defaults_2.7.9-1.dsc 2625 SHA256:1bd64d97e03fd08b1563adba7213117020779b786eb0855facc2bbd382739612
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.9-1.tar.gz' python-defaults_2.7.9-1.tar.gz 280698 SHA256:8e3d58c49b65744867edb5ee8713affd51ad068b2efd09201f56f12a57ef24e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/python-defaults/2.7.9-1/ (for browsing the source)
- https://sources.debian.net/src/python-defaults/2.7.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python-defaults/2.7.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python2.7=2.7.9-2+deb8u5`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.9-2+deb8u5`
- `libpython2.7-stdlib:amd64=2.7.9-2+deb8u5`
- `python2.7=2.7.9-2+deb8u5`
- `python2.7-minimal=2.7.9-2+deb8u5`

Licenses: (parsed from: `/usr/share/doc/libpython2.7-minimal/copyright`, `/usr/share/doc/libpython2.7-stdlib/copyright`, `/usr/share/doc/python2.7/copyright`, `/usr/share/doc/python2.7-minimal/copyright`)

- `# Licensed to PSF under a Contributor Agreement`
- `* Permission to use this software in any way is granted without`
- `Apache-2.0`
- `GPL-2`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `implied`

Source:

```console
$ apt-get source -qq --print-uris python2.7=2.7.9-2+deb8u5
'http://security.debian.org/debian-security/pool/updates/main/p/python2.7/python2.7_2.7.9-2+deb8u5.dsc' python2.7_2.7.9-2+deb8u5.dsc 3285 SHA256:20f901dff6a79b1495922fe081048ce702110f19cf39c6575eb99eec7371a153
'http://security.debian.org/debian-security/pool/updates/main/p/python2.7/python2.7_2.7.9.orig.tar.gz' python2.7_2.7.9.orig.tar.gz 15148821 SHA256:46454dc4cb20e1f9b85aef63985890fa7e247f5941991761afd97d68e69b1901
'http://security.debian.org/debian-security/pool/updates/main/p/python2.7/python2.7_2.7.9-2+deb8u5.diff.gz' python2.7_2.7.9-2+deb8u5.diff.gz 283376 SHA256:7f1201056c9b44d5add74eb2f9a5c64372f8125787efbe45b11e43abc41d1d26
```

Other potentially useful URLs:

- https://sources.debian.net/src/python2.7/2.7.9-2+deb8u5/ (for browsing the source)
- https://sources.debian.net/src/python2.7/2.7.9-2+deb8u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python2.7/2.7.9-2+deb8u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline6=6.3-8`

Binary Packages:

- `libreadline-dev:amd64=6.3-8+b3`
- `libreadline6:amd64=6.3-8+b3`
- `libreadline6-dev:amd64=6.3-8+b3`
- `readline-common=6.3-8`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline6/copyright`, `/usr/share/doc/libreadline6-dev/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline6=6.3-8
'http://deb.debian.org/debian/pool/main/r/readline6/readline6_6.3-8.dsc' readline6_6.3-8.dsc 1941 SHA256:f7ab77b8580cbdb10b3906f40c3da12d0acc93bef786ff217c65aabc32973cec
'http://deb.debian.org/debian/pool/main/r/readline6/readline6_6.3.orig.tar.gz' readline6_6.3.orig.tar.gz 2468560 SHA256:56ba6071b9462f980c5a72ab0023893b65ba6debb4eeb475d7a563dc65cafd43
'http://deb.debian.org/debian/pool/main/r/readline6/readline6_6.3-8.debian.tar.xz' readline6_6.3-8.debian.tar.xz 30576 SHA256:c2b55fdd221136f46fa1e0cbf0bf2e37b70ddf97929312fbab6032e9129d58b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline6/6.3-8/ (for browsing the source)
- https://sources.debian.net/src/readline6/6.3-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline6/6.3-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rtmpdump=2.4+20150115.gita107cef-1+deb8u1`

Binary Packages:

- `librtmp1:amd64=2.4+20150115.gita107cef-1+deb8u1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20150115.gita107cef-1+deb8u1
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20150115.gita107cef-1+deb8u1.dsc' rtmpdump_2.4+20150115.gita107cef-1+deb8u1.dsc 2299 SHA256:8f22675e50ccf221489c79a51180561b4ae58a57a6e9d52e8b3a5e3d42860ca4
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20150115.gita107cef.orig.tar.gz' rtmpdump_2.4+20150115.gita107cef.orig.tar.gz 142030 SHA256:d47ef3a07815079bf73eb5d053001c4341407fcbebf39f34e6213c4b772cb29a
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4+20150115.gita107cef-1+deb8u1.debian.tar.xz' rtmpdump_2.4+20150115.gita107cef-1+deb8u1.debian.tar.xz 8160 SHA256:b20bf79b1d8d6536f16d94af6073f3105aef91c297a67b4a6c2304de42e8d96b
```

Other potentially useful URLs:

- https://sources.debian.net/src/rtmpdump/2.4+20150115.gita107cef-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/rtmpdump/2.4+20150115.gita107cef-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rtmpdump/2.4+20150115.gita107cef-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.2.2-4+deb8u1`

Binary Packages:

- `sed=4.2.2-4+deb8u1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris sed=4.2.2-4+deb8u1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.2.2-4+deb8u1.dsc' sed_4.2.2-4+deb8u1.dsc 1495 SHA256:c8f47bac04e1b1d59fc433de2f977c6d08e40eefbdb10cabb7650297c0c12929
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.2.2.orig.tar.bz2' sed_4.2.2.orig.tar.bz2 1059414 SHA256:f048d1838da284c8bc9753e4506b85a1e0cc1ea8999d36f6995bcb9460cddbd7
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.2.2-4+deb8u1.debian.tar.xz' sed_4.2.2-4+deb8u1.debian.tar.xz 57724 SHA256:ba9b84ebb251edc7c78b3b4c715cfacc6fdd263997a92269a0282469d226557d
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.2.2-4+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.2.2-4+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.2.2-4+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sensible-utils=0.0.9+deb8u1`

Binary Packages:

- `sensible-utils=0.0.9+deb8u1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.9+deb8u1
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.9+deb8u1.dsc' sensible-utils_0.0.9+deb8u1.dsc 1590 SHA256:1d1d3d7e71c53cceb922dc33db5064cb5be76450a2918f8e3f998824237f09b0
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.9+deb8u1.tar.xz' sensible-utils_0.0.9+deb8u1.tar.xz 53544 SHA256:f4b505ecc1c5015df2e5d3595da12cceca54be8729270b054179d31d8d661ab9
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.9+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.9+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.9+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serf=1.3.8-1`

Binary Packages:

- `libserf-1-1:amd64=1.3.8-1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris serf=1.3.8-1
'http://deb.debian.org/debian/pool/main/s/serf/serf_1.3.8-1.dsc' serf_1.3.8-1.dsc 2174 SHA256:067afd128fff053de1d625f563c60cd8d1ee6c8e1ca5a9566165e9036c3e1041
'http://deb.debian.org/debian/pool/main/s/serf/serf_1.3.8.orig.tar.gz' serf_1.3.8.orig.tar.gz 184817 SHA256:77134cd5010664ca023585bce50978bd4005906ed280ff889f591f86df7c59e4
'http://deb.debian.org/debian/pool/main/s/serf/serf_1.3.8-1.diff.gz' serf_1.3.8-1.diff.gz 8249 SHA256:1f9c55374198c094746b48fa7957b48ec7334f2b92be92d5f813aec85d0e3b07
```

Other potentially useful URLs:

- https://sources.debian.net/src/serf/1.3.8-1/ (for browsing the source)
- https://sources.debian.net/src/serf/1.3.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/serf/1.3.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shadow=1:4.2-3+deb8u4`

Binary Packages:

- `login=1:4.2-3+deb8u4`
- `passwd=1:4.2-3+deb8u4`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.2-3+deb8u4
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.2-3+deb8u4.dsc' shadow_4.2-3+deb8u4.dsc 2492 SHA256:5f5c2c412e567a6f7b49141f11927202b52a8941befec39f6841b3e20a0ccea4
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.2.orig.tar.xz' shadow_4.2.orig.tar.xz 1088696 SHA256:c5bd72c4ecb438b99289e4630b22ea0626987a378d084910dbe59eceaa34be1d
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.2-3+deb8u4.debian.tar.xz' shadow_4.2-3+deb8u4.debian.tar.xz 498804 SHA256:b694aea58176f3a2703cd6461401951e52d78ad80626c39a04c0b88368957106
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.2-3+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.2-3+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.2-3+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shared-mime-info=1.3-1`

Binary Packages:

- `shared-mime-info=1.3-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.3-1
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.3-1.dsc' shared-mime-info_1.3-1.dsc 2265 SHA256:76ca2921de722cd4e17bcffadbb55f74e4730e99d8fe5cff13ad05178785c691
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.3.orig.tar.xz' shared-mime-info_1.3.orig.tar.xz 517420 SHA256:4fd49c8c7ca9ecb10c59845094a18dbb73b69c72b4bad3db5e864f2111cb323a
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.3-1.debian.tar.xz' shared-mime-info_1.3-1.debian.tar.xz 10060 SHA256:ba82b382b1fcf6a27bb410155f11b7e7d6499c3302781990e9b747b342c2e7d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/shared-mime-info/1.3-1/ (for browsing the source)
- https://sources.debian.net/src/shared-mime-info/1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shared-mime-info/1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `six=1.8.0-1`

Binary Packages:

- `python-six=1.8.0-1`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.8.0-1
'http://deb.debian.org/debian/pool/main/s/six/six_1.8.0-1.dsc' six_1.8.0-1.dsc 2190 SHA256:0a834968d7b904daeef77c2c1747483b24354e2502ddac3345247482f50ca53f
'http://deb.debian.org/debian/pool/main/s/six/six_1.8.0.orig.tar.gz' six_1.8.0.orig.tar.gz 26925 SHA256:047bbbba41bac37c444c75ddfdf0573dd6e2f1fbd824e6247bb26fa7d8fa3830
'http://deb.debian.org/debian/pool/main/s/six/six_1.8.0-1.debian.tar.xz' six_1.8.0-1.debian.tar.xz 2868 SHA256:0b1c06ec11d8d8369d8cace4bcf135ac093b848e0129390f0913a4f4b0a8e4ae
```

Other potentially useful URLs:

- https://sources.debian.net/src/six/1.8.0-1/ (for browsing the source)
- https://sources.debian.net/src/six/1.8.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/six/1.8.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `slang2=2.3.0-2`

Binary Packages:

- `libslang2:amd64=2.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libslang2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris slang2=2.3.0-2
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.0-2.dsc' slang2_2.3.0-2.dsc 2329 SHA256:2d6ede702782aec9758a3fb6001837ef6d2191d3989db63aa55333da74d5b05e
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.0.orig.tar.xz' slang2_2.3.0.orig.tar.xz 1250392 SHA256:cdd5b9582959b3afdae403ee6f4be9de8efc7e205e4a7de18c1a847ea5ef0472
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.0-2.debian.tar.xz' slang2_2.3.0-2.debian.tar.xz 21864 SHA256:8b088f54be2a284eedee56d74968feb4cc662410d352280a7e351cc02bef57b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/slang2/2.3.0-2/ (for browsing the source)
- https://sources.debian.net/src/slang2/2.3.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/slang2/2.3.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.8.7.1-1+deb8u6`

Binary Packages:

- `libsqlite3-0:amd64=3.8.7.1-1+deb8u6`
- `libsqlite3-dev:amd64=3.8.7.1-1+deb8u6`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.8.7.1-1+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1-1+deb8u6.dsc' sqlite3_3.8.7.1-1+deb8u6.dsc 2583 SHA256:682112f02141ed64f29f17b9426138cf849cade6cd1ad2adda539680b4eaa164
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1.orig-www.tar.bz2' sqlite3_3.8.7.1.orig-www.tar.bz2 3337784 SHA256:e642657752f20144f42d002895510ea635e0384b14f276f1a2f281b73252bc64
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1.orig.tar.bz2' sqlite3_3.8.7.1.orig.tar.bz2 4082068 SHA256:2632a999feba925aa0f1828fa669a091b165a719676765fb542f538345bfa7b9
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1-1+deb8u6.debian.tar.xz' sqlite3_3.8.7.1-1+deb8u6.debian.tar.xz 25212 SHA256:9fbaea758d4aaf411afbe731b442c15f4c9f5544ca466759ae131276c95e0dff
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.8.7.1-1+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.8.7.1-1+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.8.7.1-1+deb8u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `startpar=0.59-3`

Binary Packages:

- `startpar=0.59-3`

Licenses: (parsed from: `/usr/share/doc/startpar/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris startpar=0.59-3
'http://deb.debian.org/debian/pool/main/s/startpar/startpar_0.59-3.dsc' startpar_0.59-3.dsc 1496 SHA256:f8fdfac7902c1b0cf5d627421893deaa8e041e9e23096ae60a33fe84464526ff
'http://deb.debian.org/debian/pool/main/s/startpar/startpar_0.59.orig.tar.bz2' startpar_0.59.orig.tar.bz2 22747 SHA256:30a30c8d27a694e3743c1839fb6f60563b2882cddf0e61c698120c4cbde1d7b9
'http://deb.debian.org/debian/pool/main/s/startpar/startpar_0.59-3.debian.tar.xz' startpar_0.59-3.debian.tar.xz 38428 SHA256:abd4650e507cd4e63e7caf2199972b6ee5367aea34ae8f53a19caf126bd2248c
```

Other potentially useful URLs:

- https://sources.debian.net/src/startpar/0.59-3/ (for browsing the source)
- https://sources.debian.net/src/startpar/0.59-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/startpar/0.59-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `subversion=1.8.10-6+deb8u7`

Binary Packages:

- `libsvn1:amd64=1.8.10-6+deb8u7`
- `subversion=1.8.10-6+deb8u7`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris subversion=1.8.10-6+deb8u7
'http://security.debian.org/debian-security/pool/updates/main/s/subversion/subversion_1.8.10-6+deb8u7.dsc' subversion_1.8.10-6+deb8u7.dsc 3035 SHA256:da5e655efd0221b37e594dda3844c88b23260fd98a965016e31527077148aaf4
'http://security.debian.org/debian-security/pool/updates/main/s/subversion/subversion_1.8.10.orig.tar.gz' subversion_1.8.10.orig.tar.gz 9331079 SHA256:d0efa2533225c0bfba2ac27bcc004255997cbbde58f4f970dfb9dc3cc825005f
'http://security.debian.org/debian-security/pool/updates/main/s/subversion/subversion_1.8.10-6+deb8u7.diff.gz' subversion_1.8.10-6+deb8u7.diff.gz 306950 SHA256:4806824ffa7f70c7f8327f86dbfbefa0ba19b86fa967f1b0f9ce4dbb1e8d10b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.8.10-6+deb8u7/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.8.10-6+deb8u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.8.10-6+deb8u7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=215-17+deb8u13`

Binary Packages:

- `libsystemd0:amd64=215-17+deb8u13`
- `libudev1:amd64=215-17+deb8u13`
- `systemd=215-17+deb8u13`
- `systemd-sysv=215-17+deb8u13`
- `udev=215-17+deb8u13`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`, `/usr/share/doc/systemd/copyright`, `/usr/share/doc/systemd-sysv/copyright`, `/usr/share/doc/udev/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=215-17+deb8u13
'http://security.debian.org/debian-security/pool/updates/main/s/systemd/systemd_215-17+deb8u13.dsc' systemd_215-17+deb8u13.dsc 4182 SHA256:d8c3f700871e3962b7c16fbaf8e7c8aaa0fb95a4410dff04d54e229169451ec3
'http://security.debian.org/debian-security/pool/updates/main/s/systemd/systemd_215.orig.tar.xz' systemd_215.orig.tar.xz 2888652 SHA256:ce76a3c05e7d4adc806a3446a5510c0c9b76a33f19adc32754b69a0945124505
'http://security.debian.org/debian-security/pool/updates/main/s/systemd/systemd_215-17+deb8u13.debian.tar.xz' systemd_215-17+deb8u13.debian.tar.xz 248816 SHA256:7274d5e33a526b06d37558999325b15f8dd773ad9ddd61cc7f5e12f1bca839db
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/215-17+deb8u13/ (for browsing the source)
- https://sources.debian.net/src/systemd/215-17+deb8u13/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/215-17+deb8u13/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=2.88dsf-59`

Binary Packages:

- `initscripts=2.88dsf-59`
- `sysv-rc=2.88dsf-59`
- `sysvinit-utils=2.88dsf-59`

Licenses: (parsed from: `/usr/share/doc/initscripts/copyright`, `/usr/share/doc/sysv-rc/copyright`, `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.dsc' sysvinit_2.88dsf-59.dsc 2467 SHA256:0201f6d34c1be692ac0e594a4006e7e0b921eda7ffb37b4373abc949bf7181b2
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.88dsf-59.debian.tar.xz' sysvinit_2.88dsf-59.debian.tar.xz 152316 SHA256:cfd1ff3423b7cfb2239f2311088eba8e5b8abde1835cb25806fb0983d159635f
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.88dsf-59/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.88dsf-59/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.88dsf-59/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.27.1-2+deb8u2`

Binary Packages:

- `tar=1.27.1-2+deb8u2`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.27.1-2+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/t/tar/tar_1.27.1-2+deb8u2.dsc' tar_1.27.1-2+deb8u2.dsc 1923 SHA256:bde1870e1a78c8f0967166ab8e0c8f22ca54e789bbc2aaa3a92afe6521304dfa
'http://security.debian.org/debian-security/pool/updates/main/t/tar/tar_1.27.1.orig.tar.xz' tar_1.27.1.orig.tar.xz 1704252 SHA256:58169c5a03c04be20d3fb91010b01e822c6a58060a96e7cf2f9c1944de0151ab
'http://security.debian.org/debian-security/pool/updates/main/t/tar/tar_1.27.1-2+deb8u2.debian.tar.xz' tar_1.27.1-2+deb8u2.debian.tar.xz 33736 SHA256:2459839d37230c8677d087eb02d9e5e7efa18bcb147ed81aa33b9c4720763947
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.27.1-2+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/tar/1.27.1-2+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.27.1-2+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.0.3-12.3+deb8u10`

Binary Packages:

- `libtiff5:amd64=4.0.3-12.3+deb8u10`
- `libtiff5-dev:amd64=4.0.3-12.3+deb8u10`
- `libtiffxx5:amd64=4.0.3-12.3+deb8u10`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.3-12.3+deb8u10
'http://security.debian.org/debian-security/pool/updates/main/t/tiff/tiff_4.0.3-12.3+deb8u10.dsc' tiff_4.0.3-12.3+deb8u10.dsc 2403 SHA256:40404d8248af7d7747f4e26e7f565309a101b5c319a6c83e98f255418d47a0f1
'http://security.debian.org/debian-security/pool/updates/main/t/tiff/tiff_4.0.3.orig.tar.gz' tiff_4.0.3.orig.tar.gz 2051630 SHA256:ea1aebe282319537fb2d4d7805f478dd4e0e05c33d0928baba76a7c963684872
'http://security.debian.org/debian-security/pool/updates/main/t/tiff/tiff_4.0.3-12.3+deb8u10.debian.tar.xz' tiff_4.0.3-12.3+deb8u10.debian.tar.xz 72116 SHA256:82cb1167bd84eb8583c4b937a7c7a8d37fe78c2a2392a167b16c40dd02dfc62b
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.0.3-12.3+deb8u10/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.0.3-12.3+deb8u10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.0.3-12.3+deb8u10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2019c-0+deb8u1`

Binary Packages:

- `tzdata=2019c-0+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2019c-0+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/t/tzdata/tzdata_2019c-0+deb8u1.dsc' tzdata_2019c-0+deb8u1.dsc 1985 SHA256:554948d9fdd1ceaa3a6aa3b5134c46f3608bd35365159ec2fe63b2e06bf2d4ab
'http://security.debian.org/debian-security/pool/updates/main/t/tzdata/tzdata_2019c.orig.tar.gz' tzdata_2019c.orig.tar.gz 392087 SHA256:79c7806dab09072308da0e3d22c37d3b245015a591891ea147d3b133b60ffc7c
'http://security.debian.org/debian-security/pool/updates/main/t/tzdata/tzdata_2019c-0+deb8u1.debian.tar.xz' tzdata_2019c-0+deb8u1.debian.tar.xz 103804 SHA256:104ee8c849bbcea67914610ac439ccff4d3a716026d190c8321a60a047ddd16b
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2019c-0+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2019c-0+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2019c-0+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ucf=3.0030`

Binary Packages:

- `ucf=3.0030`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0030
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0030.dsc' ucf_3.0030.dsc 1300 SHA256:7e1861964217317a6be7fe83c1baaeb578e27a33850c33f14d168e40811b9115
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0030.tar.xz' ucf_3.0030.tar.xz 63524 SHA256:65b681c509f49bca586f12d57c5244ad93cf0d047f886e307fb2018abf3d802d
```

Other potentially useful URLs:

- https://sources.debian.net/src/ucf/3.0030/ (for browsing the source)
- https://sources.debian.net/src/ucf/3.0030/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ucf/3.0030/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unzip=6.0-16+deb8u6`

Binary Packages:

- `unzip=6.0-16+deb8u6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-16+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/u/unzip/unzip_6.0-16+deb8u6.dsc' unzip_6.0-16+deb8u6.dsc 1858 SHA256:915a41fc41fb3545904bd59f2e21f763311a8616f9e09d33f3bba5532758c1c9
'http://security.debian.org/debian-security/pool/updates/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://security.debian.org/debian-security/pool/updates/main/u/unzip/unzip_6.0-16+deb8u6.debian.tar.xz' unzip_6.0-16+deb8u6.debian.tar.xz 21552 SHA256:e8f461f9ccc39dba230c71014023481bff7f59fdfabac016a685a43d31c8bf05
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-16+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-16+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-16+deb8u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ustr=1.0.4-3`

Binary Packages:

- `libustr-1.0-1:amd64=1.0.4-3+b2`

Licenses: (parsed from: `/usr/share/doc/libustr-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris ustr=1.0.4-3
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4-3.dsc' ustr_1.0.4-3.dsc 1992 SHA256:ca6043d523fd9f677446b6cac95ce5263768f3ccc5ee38ef10e1551b2cf1c00a
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4.orig.tar.gz' ustr_1.0.4.orig.tar.gz 301345 SHA256:4d293b6b9d9fe51d58441f4b09b1f0005fcad8256ae8048587789bf5dbefb62e
'http://deb.debian.org/debian/pool/main/u/ustr/ustr_1.0.4-3.diff.gz' ustr_1.0.4-3.diff.gz 11415 SHA256:8349cbdef416e9b919d434c6a88c7e29700a00df3e81f21b7d8127ffd7e4945a
```

Other potentially useful URLs:

- https://sources.debian.net/src/ustr/1.0.4-3/ (for browsing the source)
- https://sources.debian.net/src/ustr/1.0.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ustr/1.0.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.25.2-6`

Binary Packages:

- `bsdutils=1:2.25.2-6`
- `libblkid1:amd64=2.25.2-6`
- `libmount1:amd64=2.25.2-6`
- `libsmartcols1:amd64=2.25.2-6`
- `libuuid1:amd64=2.25.2-6`
- `mount=2.25.2-6`
- `util-linux=2.25.2-6`

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
$ apt-get source -qq --print-uris util-linux=2.25.2-6
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.25.2-6.dsc' util-linux_2.25.2-6.dsc 3443 SHA256:742a9c6378132c30d4bfc31722904e73a608c2fee1eab89d1d832c5e5672a82f
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.25.2.orig.tar.xz' util-linux_2.25.2.orig.tar.xz 3703644 SHA256:e0457f715b73f4a349e1acb08cb410bf0edc9a74a3f75c357070f31f70e33cd6
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.25.2-6.debian.tar.xz' util-linux_2.25.2-6.debian.tar.xz 304292 SHA256:b500d70a60f2814d6552492cee5f40c27063029ef74ddea53bc713503680527b
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.25.2-6/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.25.2-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.25.2-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.16-1+deb8u7`

Binary Packages:

- `wget=1.16-1+deb8u7`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.16-1+deb8u7
'http://security.debian.org/debian-security/pool/updates/main/w/wget/wget_1.16-1+deb8u7.dsc' wget_1.16-1+deb8u7.dsc 1942 SHA256:f866d6e5ee2d6d769f29de7697778732d466a3f7864babdf478942b814ec42e7
'http://security.debian.org/debian-security/pool/updates/main/w/wget/wget_1.16.orig.tar.gz' wget_1.16.orig.tar.gz 3325041 SHA256:b977fc10ac7a72d987d48136251aeb332f2dced1aabd50d6d56bdf72e2b79101
'http://security.debian.org/debian-security/pool/updates/main/w/wget/wget_1.16-1+deb8u7.debian.tar.xz' wget_1.16-1+deb8u7.debian.tar.xz 24840 SHA256:7abcc58ac8fa94653b2b2407a4a9bf312e53dd60243bc0d3244f10b166fbc83c
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.16-1+deb8u7/ (for browsing the source)
- https://sources.debian.net/src/wget/1.16-1+deb8u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.16-1+deb8u7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x11proto-core=7.0.26-1`

Binary Packages:

- `x11proto-core-dev=7.0.26-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-core=7.0.26-1
'http://deb.debian.org/debian/pool/main/x/x11proto-core/x11proto-core_7.0.26-1.dsc' x11proto-core_7.0.26-1.dsc 1985 SHA256:00a740d85a012605e2074a384c54fdda16901cc36c6483a65e4af28f043dd021
'http://deb.debian.org/debian/pool/main/x/x11proto-core/x11proto-core_7.0.26.orig.tar.gz' x11proto-core_7.0.26.orig.tar.gz 366843 SHA256:ea39fae5edf841f56525ab76590d8edbf53b8ec1a7fca0ab815917000ef02666
'http://deb.debian.org/debian/pool/main/x/x11proto-core/x11proto-core_7.0.26-1.diff.gz' x11proto-core_7.0.26-1.diff.gz 6501 SHA256:cf4d058d8562c69a89e00d02a62763c0a85ac0fe06184a00c98f213a25c8dc67
```

Other potentially useful URLs:

- https://sources.debian.net/src/x11proto-core/7.0.26-1/ (for browsing the source)
- https://sources.debian.net/src/x11proto-core/7.0.26-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x11proto-core/7.0.26-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x11proto-input=2.3.1-1`

Binary Packages:

- `x11proto-input-dev=2.3.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-input=2.3.1-1
'http://deb.debian.org/debian/pool/main/x/x11proto-input/x11proto-input_2.3.1-1.dsc' x11proto-input_2.3.1-1.dsc 1937 SHA256:c43dcce256561df0c239d24a5d9653cf651bfc949dc1a98bb450b1f23dda0b21
'http://deb.debian.org/debian/pool/main/x/x11proto-input/x11proto-input_2.3.1.orig.tar.gz' x11proto-input_2.3.1.orig.tar.gz 236302 SHA256:23f65ac55c36ea8c378e30b4a4fd85317c95923134e3fe46569741b94c8ed4ca
'http://deb.debian.org/debian/pool/main/x/x11proto-input/x11proto-input_2.3.1-1.diff.gz' x11proto-input_2.3.1-1.diff.gz 5603 SHA256:c92b1b97ce557f3564bd5252f921c1bc510df00ef1a81323078181754b4a31ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/x11proto-input/2.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/x11proto-input/2.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x11proto-input/2.3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x11proto-kb=1.0.6-2`

Binary Packages:

- `x11proto-kb-dev=1.0.6-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-kb=1.0.6-2
'http://deb.debian.org/debian/pool/main/x/x11proto-kb/x11proto-kb_1.0.6-2.dsc' x11proto-kb_1.0.6-2.dsc 1327 SHA256:4cf714aa520a551e5eefa76c38f07d882ca36e1ccf029baf0517b59a688a1dfc
'http://deb.debian.org/debian/pool/main/x/x11proto-kb/x11proto-kb_1.0.6.orig.tar.gz' x11proto-kb_1.0.6.orig.tar.gz 315728 SHA256:01fd22286ca9c2a93ca7bb686dbb2f3c108ceb944cd3dfdc9ceeb50f9b7f4505
'http://deb.debian.org/debian/pool/main/x/x11proto-kb/x11proto-kb_1.0.6-2.diff.gz' x11proto-kb_1.0.6-2.diff.gz 14128 SHA256:a33fddbe8c2cb0fb92137343e7fd86c52041152121ac427de5b55241f445d17b
```

Other potentially useful URLs:

- https://sources.debian.net/src/x11proto-kb/1.0.6-2/ (for browsing the source)
- https://sources.debian.net/src/x11proto-kb/1.0.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x11proto-kb/1.0.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x11proto-render=2:0.11.1-2`

Binary Packages:

- `x11proto-render-dev=2:0.11.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-render=2:0.11.1-2
'http://deb.debian.org/debian/pool/main/x/x11proto-render/x11proto-render_0.11.1-2.dsc' x11proto-render_0.11.1-2.dsc 1979 SHA256:5cebbcce7928bd468b0eb447d9da403e5228af1691549a529a9012d2f7d18948
'http://deb.debian.org/debian/pool/main/x/x11proto-render/x11proto-render_0.11.1.orig.tar.gz' x11proto-render_0.11.1.orig.tar.gz 124436 SHA256:a0a4be3cad9381ae28279ba5582e679491fc2bec9aab8a65993108bf8dbce5fe
'http://deb.debian.org/debian/pool/main/x/x11proto-render/x11proto-render_0.11.1-2.diff.gz' x11proto-render_0.11.1-2.diff.gz 14527 SHA256:614b7adf6f08bdf25bc7fb565f048e2f94e290c3bd056fa2485e093eb887c54f
```

Other potentially useful URLs:

- https://sources.debian.net/src/x11proto-render/2:0.11.1-2/ (for browsing the source)
- https://sources.debian.net/src/x11proto-render/2:0.11.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x11proto-render/2:0.11.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x11proto-xext=7.3.0-1`

Binary Packages:

- `x11proto-xext-dev=7.3.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-xext=7.3.0-1
'http://deb.debian.org/debian/pool/main/x/x11proto-xext/x11proto-xext_7.3.0-1.dsc' x11proto-xext_7.3.0-1.dsc 1997 SHA256:4b806c7f17f7dd466901111ce0862117541098025470601c251499d76affe9fc
'http://deb.debian.org/debian/pool/main/x/x11proto-xext/x11proto-xext_7.3.0.orig.tar.gz' x11proto-xext_7.3.0.orig.tar.gz 290814 SHA256:1b1bcdf91221e78c6c33738667a57bd9aaa63d5953174ad8ed9929296741c9f5
'http://deb.debian.org/debian/pool/main/x/x11proto-xext/x11proto-xext_7.3.0-1.diff.gz' x11proto-xext_7.3.0-1.diff.gz 16644 SHA256:68eec9363c7f8bcfbbaba68d6661284eb78fffccbddb293b95a6c85647cfcf6c
```

Other potentially useful URLs:

- https://sources.debian.net/src/x11proto-xext/7.3.0-1/ (for browsing the source)
- https://sources.debian.net/src/x11proto-xext/7.3.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x11proto-xext/7.3.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xorg=1:7.7+7`

Binary Packages:

- `x11-common=1:7.7+7`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+7
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+7.dsc' xorg_7.7+7.dsc 1934 SHA256:fdba3ef7ef9309f4d038d56b028935d3a2e06c2f68f4168d8f27683c9279da3c
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+7.tar.gz' xorg_7.7+7.tar.gz 919132 SHA256:ac9dd34ee30176e71a954bc1b922f7ccb81d759bd57674d1972bc14a93916667
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg/1:7.7+7/ (for browsing the source)
- https://sources.debian.net/src/xorg/1:7.7+7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg/1:7.7+7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xtrans=1.3.4-1`

Binary Packages:

- `xtrans-dev=1.3.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xtrans=1.3.4-1
'http://deb.debian.org/debian/pool/main/x/xtrans/xtrans_1.3.4-1.dsc' xtrans_1.3.4-1.dsc 1896 SHA256:5e0b8b3e16c51e7304b7565df3592cfa7cc743836b92e1a8565b9acdabbe0e13
'http://deb.debian.org/debian/pool/main/x/xtrans/xtrans_1.3.4.orig.tar.gz' xtrans_1.3.4.orig.tar.gz 223528 SHA256:13b908cccb79eadd667c6722df6d1d933586477b16bd8815aa85195c2de8ca08
'http://deb.debian.org/debian/pool/main/x/xtrans/xtrans_1.3.4-1.diff.gz' xtrans_1.3.4-1.diff.gz 15937 SHA256:be419f602b4d0d9731f5626b112c95b63625b40505df02d421dbae29f828b7aa
```

Other potentially useful URLs:

- https://sources.debian.net/src/xtrans/1.3.4-1/ (for browsing the source)
- https://sources.debian.net/src/xtrans/1.3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xtrans/1.3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.1.1alpha+20120614-2`

Binary Packages:

- `liblzma-dev:amd64=5.1.1alpha+20120614-2+b3`
- `liblzma5:amd64=5.1.1alpha+20120614-2+b3`
- `xz-utils=5.1.1alpha+20120614-2+b3`

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
$ apt-get source -qq --print-uris xz-utils=5.1.1alpha+20120614-2
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2.dsc' xz-utils_5.1.1alpha+20120614-2.dsc 2325 SHA256:d7d87c6c7aa6d2fe45d8d55a8929ab12f0688f7f17bcfc6233ecfa94f6f7a298
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614.orig.tar.gz' xz-utils_5.1.1alpha+20120614.orig.tar.gz 556454 SHA256:b168e63400db449a6e7b3a06e668f557ca27e3d70accbd29d2b5a98e15c00fee
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2.debian.tar.gz' xz-utils_5.1.1alpha+20120614-2.debian.tar.gz 154298 SHA256:4e2873ab7b1ee44b7d580caf2a5ca761b10cb2725691b2c2a9b21edb0d771f39
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.1.1alpha+20120614-2/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.1.1alpha+20120614-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.1.1alpha+20120614-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.8.dfsg-2+deb8u1`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-2+deb8u1`
- `zlib1g-dev:amd64=1:1.2.8.dfsg-2+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.8.dfsg-2+deb8u1
'http://security.debian.org/debian-security/pool/updates/main/z/zlib/zlib_1.2.8.dfsg-2+deb8u1.dsc' zlib_1.2.8.dfsg-2+deb8u1.dsc 2661 SHA256:30356ac08b7b18f9f1f0ca1f2a4d9a85a7b2554a94001938c4ec95b69e3c787b
'http://security.debian.org/debian-security/pool/updates/main/z/zlib/zlib_1.2.8.dfsg.orig.tar.gz' zlib_1.2.8.dfsg.orig.tar.gz 361943 SHA256:2caecc2c3f1ef8b87b8f72b128a03e61c307e8c14f5ec9b422ef7914ba75cf9f
'http://security.debian.org/debian-security/pool/updates/main/z/zlib/zlib_1.2.8.dfsg-2+deb8u1.debian.tar.xz' zlib_1.2.8.dfsg-2+deb8u1.debian.tar.xz 17444 SHA256:81a745765a43f8ff16c66d7dbac7ef735bda39adefa52bb2734e3a4c13cf545b
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.8.dfsg-2+deb8u1/ (for access to the source package after it no longer exists in the archive)
