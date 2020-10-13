# `buildpack-deps:jessie-scm`

## Docker Metadata

- Image ID: `sha256:95a28fcb6dc864d03e5815110bb7f679e5cb32ae4936b0b45a9a5fb75876df46`
- Created: `2020-10-13T02:20:12.421317986Z`
- Virtual Size: ~ 293.29 Mb  
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

### `dpkg` source package: `bzip2=1.0.6-7+deb8u2`

Binary Packages:

- `libbz2-1.0:amd64=1.0.6-7+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`)

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

### `dpkg` source package: `db5.3=5.3.28-9+deb8u1`

Binary Packages:

- `libdb5.3:amd64=5.3.28-9+deb8u1`

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

### `dpkg` source package: `dpkg=1.17.27`

Binary Packages:

- `dpkg=1.17.27`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

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

- `e2fslibs:amd64=1.42.12-2+deb8u2`
- `e2fsprogs=1.42.12-2+deb8u2`
- `libcomerr2:amd64=1.42.12-2+deb8u2`
- `libss2:amd64=1.42.12-2+deb8u2`

Licenses: (parsed from: `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

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

- `gcc-4.9-base:amd64=4.9.2-10+deb8u2`
- `libgcc1:amd64=1:4.9.2-10+deb8u2`
- `libstdc++6:amd64=4.9.2-10+deb8u2`

Licenses: (parsed from: `/usr/share/doc/gcc-4.9-base/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

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

### `dpkg` source package: `gdbm=1.8.3-13.1`

Binary Packages:

- `libgdbm3:amd64=1.8.3-13.1`

Licenses: (parsed from: `/usr/share/doc/libgdbm3/copyright`)

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

### `dpkg` source package: `glibc=2.19-18+deb8u10`

Binary Packages:

- `libc-bin=2.19-18+deb8u10`
- `libc6:amd64=2.19-18+deb8u10`
- `multiarch-support=2.19-18+deb8u10`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/multiarch-support/copyright`)

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

- `libgmp10:amd64=2:6.0.0+dfsg-6`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

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

- `libgssapi-krb5-2:amd64=1.12.1+dfsg-19+deb8u5`
- `libk5crypto3:amd64=1.12.1+dfsg-19+deb8u5`
- `libkrb5-3:amd64=1.12.1+dfsg-19+deb8u5`
- `libkrb5support0:amd64=1.12.1+dfsg-19+deb8u5`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

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

### `dpkg` source package: `libffi=3.1-2+deb8u1`

Binary Packages:

- `libffi6:amd64=3.1-2+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

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

### `dpkg` source package: `ncurses=5.9+20140913-1+deb8u3`

Binary Packages:

- `libncurses5:amd64=5.9+20140913-1+deb8u3`
- `libncursesw5:amd64=5.9+20140913-1+deb8u3`
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

### `dpkg` source package: `pcre3=2:8.35-3.3+deb8u4`

Binary Packages:

- `libpcre3:amd64=2:8.35-3.3+deb8u4`

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

- `libreadline6:amd64=6.3-8+b3`
- `readline-common=6.3-8`

Licenses: (parsed from: `/usr/share/doc/libreadline6/copyright`, `/usr/share/doc/readline-common/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

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

### `dpkg` source package: `xz-utils=5.1.1alpha+20120614-2`

Binary Packages:

- `liblzma5:amd64=5.1.1alpha+20120614-2+b3`

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
