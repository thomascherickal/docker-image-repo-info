# `jetty:9.2.28-jre7`

## Docker Metadata

- Image ID: `sha256:00659b0295385e477a75db0c645a362aa56a429dade512df9939b5341ff72e9b`
- Created: `2019-05-14T00:58:14.98267366Z`
- Virtual Size: ~ 343.41 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
- Command: `["java","-jar","/usr/local/jetty/start.jar"]`
- Environment:
  - `PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `JAVA_HOME=/docker-java-home/jre`
  - `JAVA_VERSION=7u221`
  - `JAVA_DEBIAN_VERSION=7u221-2.6.18-1~deb8u1`
  - `JETTY_HOME=/usr/local/jetty`
  - `JETTY_VERSION=9.2.28.v20190418`
  - `JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-distribution/9.2.28.v20190418/jetty-distribution-9.2.28.v20190418.tar.gz`
  - `JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	FBA2B18D238AB852DF95745C76157BDF03D0DCD6 	5C9579B3DB2E506429319AAEF33B071B29559E1E`
  - `JETTY_BASE=/var/lib/jetty`
  - `TMPDIR=/tmp/jetty`

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

### `dpkg` source package: `alsa-lib=1.0.28-1`

Binary Packages:

- `libasound2:amd64=1.0.28-1`
- `libasound2-data=1.0.28-1`

Licenses: (parsed from: `/usr/share/doc/libasound2/copyright`, `/usr/share/doc/libasound2-data/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris alsa-lib=1.0.28-1
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.0.28-1.dsc' alsa-lib_1.0.28-1.dsc 1758 SHA256:20592488800cc3b17968864c7f543339f1b844c14658b013571bd7dc9dd3ebde
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.0.28.orig.tar.bz2' alsa-lib_1.0.28.orig.tar.bz2 903786 SHA256:3c074b85dde1b30e78ef4995579765833e5b693fbbd8f834c335e080cb734a6d
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.0.28-1.debian.tar.xz' alsa-lib_1.0.28-1.debian.tar.xz 51448 SHA256:a0d8d3282ff3866de47ff44ca5084647ccc8d8c0848498e77ddd40f739388470
```

Other potentially useful URLs:

- https://sources.debian.net/src/alsa-lib/1.0.28-1/ (for browsing the source)
- https://sources.debian.net/src/alsa-lib/1.0.28-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/alsa-lib/1.0.28-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=1.0.9.8.5`

Binary Packages:

- `apt=1.0.9.8.5`
- `libapt-pkg4.12:amd64=1.0.9.8.5`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg4.12/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.0.9.8.5
'http://security.debian.org/debian-security/pool/updates/main/a/apt/apt_1.0.9.8.5.dsc' apt_1.0.9.8.5.dsc 2396 SHA256:57375233b57c22cd93539ce6d9ab26c4f3f5dac604c0a9b1479dc4da7b60fda3
'http://security.debian.org/debian-security/pool/updates/main/a/apt/apt_1.0.9.8.5.tar.xz' apt_1.0.9.8.5.tar.xz 1783540 SHA256:d4e9dc57b0704e713895aa10de821c804b9a5c367772c36667cddbef96e79bd2
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/1.0.9.8.5/ (for browsing the source)
- https://sources.debian.net/src/apt/1.0.9.8.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/1.0.9.8.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `atk1.0=2.14.0-1`

Binary Packages:

- `libatk1.0-0:amd64=2.14.0-1`
- `libatk1.0-data=2.14.0-1`

Licenses: (parsed from: `/usr/share/doc/libatk1.0-0/copyright`, `/usr/share/doc/libatk1.0-data/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris atk1.0=2.14.0-1
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.14.0-1.dsc' atk1.0_2.14.0-1.dsc 2037 SHA256:4535882fa01ef66455fca326aa7576c34181045a0814ecf16bdf99f5fbdc9ba5
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.14.0.orig.tar.xz' atk1.0_2.14.0.orig.tar.xz 696064 SHA256:2875cc0b32bfb173c066c22a337f79793e0c99d2cc5e81c4dac0d5a523b8fbad
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.14.0-1.debian.tar.xz' atk1.0_2.14.0-1.debian.tar.xz 10372 SHA256:d17bd76ea933603f5426497039219bd9aa9693d91a4ae585c490b5500dc9aa92
```

Other potentially useful URLs:

- https://sources.debian.net/src/atk1.0/2.14.0-1/ (for browsing the source)
- https://sources.debian.net/src/atk1.0/2.14.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/atk1.0/2.14.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `avahi=0.6.31-5`

Binary Packages:

- `libavahi-client3:amd64=0.6.31-5`
- `libavahi-common-data:amd64=0.6.31-5`
- `libavahi-common3:amd64=0.6.31-5`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.6.31-5
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.31-5.dsc' avahi_0.6.31-5.dsc 4069 SHA256:0fd83a73ecc0378fa9db09b59c0679ed52230601e23d43dabb62ba7dcf8e9383
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.31.orig.tar.gz' avahi_0.6.31.orig.tar.gz 1268686 SHA256:8372719b24e2dd75de6f59bb1315e600db4fd092805bd1201ed0cb651a2dab48
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.31-5.debian.tar.xz' avahi_0.6.31-5.debian.tar.xz 31300 SHA256:3fd413d85ab8650d448adbdf82fddbff688d159d19a3f2c8ba26c1a49ee7605d
```

Other potentially useful URLs:

- https://sources.debian.net/src/avahi/0.6.31-5/ (for browsing the source)
- https://sources.debian.net/src/avahi/0.6.31-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/avahi/0.6.31-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `bzip2=1.0.6-7`

Binary Packages:

- `bzip2=1.0.6-7+b3`
- `libbz2-1.0:amd64=1.0.6-7+b3`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-7
'http://security.debian.org/debian-security/pool/updates/main/b/bzip2/bzip2_1.0.6-7+deb8u2.dsc' bzip2_1.0.6-7+deb8u2.dsc 2462 SHA256:7f1f29e1c032ca64068eb0aa7b9e025b0c9e41218974d8fff3d255397fc691f5
'http://security.debian.org/debian-security/pool/updates/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://security.debian.org/debian-security/pool/updates/main/b/bzip2/bzip2_1.0.6-7+deb8u2.debian.tar.bz2' bzip2_1.0.6-7+deb8u2.debian.tar.bz2 61298 SHA256:49b18ae614a6a92beaf846ae2d5df29687c6d09a158f57db548ff52b882f51b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.6-7/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.6-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.6-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates-java=20140324`

Binary Packages:

- `ca-certificates-java=20140324`

Licenses: (parsed from: `/usr/share/doc/ca-certificates-java/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates-java=20140324
'http://deb.debian.org/debian/pool/main/c/ca-certificates-java/ca-certificates-java_20140324.dsc' ca-certificates-java_20140324.dsc 1839 SHA256:c43e617f08f2201bd484fc9943535bbb2750ce3093cdbcdeee3d1d4b1046f0cf
'http://deb.debian.org/debian/pool/main/c/ca-certificates-java/ca-certificates-java_20140324.tar.xz' ca-certificates-java_20140324.tar.xz 15632 SHA256:fd369f31b30dcfcf73465bc1f9edaab2867d9fed8373ebc5326dac4c96ffc08e
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates-java/20140324/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates-java/20140324/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates-java/20140324/ (for access to the source package after it no longer exists in the archive)

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

- `libcairo2:amd64=1.14.0-2.1+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libcairo2/copyright`)

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

### `dpkg` source package: `cups=1.7.5-11+deb8u4`

Binary Packages:

- `libcups2:amd64=1.7.5-11+deb8u4`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`)

- `GPL-2`
- `GPL-2 with exceptions`
- `LGPL-2`
- `LGPL-2 with exceptions`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cups/1.7.5-11+deb8u4/


### `dpkg` source package: `curl=7.38.0-4+deb8u14`

Binary Packages:

- `curl=7.38.0-4+deb8u14`
- `libcurl3:amd64=7.38.0-4+deb8u14`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/curl/7.38.0-4+deb8u14/


### `dpkg` source package: `cyrus-sasl2=2.1.26.dfsg1-13+deb8u1`

Binary Packages:

- `libsasl2-2:amd64=2.1.26.dfsg1-13+deb8u1`
- `libsasl2-modules-db:amd64=2.1.26.dfsg1-13+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.26.dfsg1-13+deb8u1
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.dsc' cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.dsc 3461 SHA256:ed1cba2b699aaf1ad08b99ea82d40c583c02817f6fbd765b9bbcd940d72fc3f3
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz' cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz 1494337 SHA256:172c39555012f479543ce7305949db75df708771fe8f8b34248027f09e53bb85
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.debian.tar.xz' cyrus-sasl2_2.1.26.dfsg1-13+deb8u1.debian.tar.xz 94284 SHA256:14e00798c41b6fae965211f1af8b47a67d22001146d0019f81af0fc7be9f162f
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.26.dfsg1-13+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.26.dfsg1-13+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.26.dfsg1-13+deb8u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `dbus=1.8.22-0+deb8u1`

Binary Packages:

- `libdbus-1-3:amd64=1.8.22-0+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libdbus-1-3/copyright`)

- `AFL-2.1`
- `AFL-2.1,`
- `BSD-3-clause`
- `BSD-3-clause-generic`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `Tcl-BSDish`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris dbus=1.8.22-0+deb8u1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.8.22-0+deb8u1.dsc' dbus_1.8.22-0+deb8u1.dsc 2889 SHA256:13cf18c13043baccf6fb26d18ea4e0fcb4b6859942175b3b735a1f63608c75c1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.8.22.orig.tar.gz' dbus_1.8.22.orig.tar.gz 1894768 SHA256:19a52e5a42b2a2faf15a54745a098bb8cf55a76598fa4a0b8b6d886adcbe1d53
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.8.22-0+deb8u1.debian.tar.xz' dbus_1.8.22-0+deb8u1.debian.tar.xz 38168 SHA256:9c702fd70d8b451351bf8566dae78ef57e129d7cad9fcde000923575131fda5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus/1.8.22-0+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/dbus/1.8.22-0+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus/1.8.22-0+deb8u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `e2fsprogs=1.42.12-2`

Binary Packages:

- `e2fslibs:amd64=1.42.12-2+b1`
- `e2fsprogs=1.42.12-2+b1`
- `libcomerr2:amd64=1.42.12-2+b1`
- `libss2:amd64=1.42.12-2+b1`

Licenses: (parsed from: `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.42.12-2
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.42.12-2+deb8u1.dsc' e2fsprogs_1.42.12-2+deb8u1.dsc 2747 SHA256:f3c40ff73088858d41c1d936c79836e066bdffe8f9b6351ad67d4fa73184c5b8
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.42.12.orig.tar.gz' e2fsprogs_1.42.12.orig.tar.gz 6381695 SHA256:e17846d91a0edd89fa59b064bde8f8e5cec5851e35f587bcccb4014dbd63186c
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.42.12-2+deb8u1.debian.tar.xz' e2fsprogs_1.42.12-2+deb8u1.debian.tar.xz 70292 SHA256:250ad73c0d8577b83bfb9004be0691667cb2ec913fecf9947903ba250cfc013c
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.42.12-2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.42.12-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.42.12-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.1.0-6+deb8u4`

Binary Packages:

- `libexpat1:amd64=2.1.0-6+deb8u4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.1.0-6+deb8u4
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.1.0-6+deb8u4.dsc' expat_2.1.0-6+deb8u4.dsc 2292 SHA256:7f7a5fed696e3b17f50e576dbae7013793e59517b04818e8b1688d9581792245
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.1.0.orig.tar.gz' expat_2.1.0.orig.tar.gz 562616 SHA256:823705472f816df21c8f6aa026dd162b280806838bb55b3432b0fb1fcca7eb86
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.1.0-6+deb8u4.debian.tar.xz' expat_2.1.0-6+deb8u4.debian.tar.xz 22672 SHA256:e832a0c7f1645bb915310628c38ecc6183f6854b0788332a7be470d06d4d149b
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.1.0-6+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/expat/2.1.0-6+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.1.0-6+deb8u4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `flac=1.3.0-3`

Binary Packages:

- `libflac8:amd64=1.3.0-3`

Licenses: (parsed from: `/usr/share/doc/libflac8/copyright`)

- `GFDL-1.2`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris flac=1.3.0-3
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.0-3.dsc' flac_1.3.0-3.dsc 2259 SHA256:9dafbe2aa5bfd1aff558b6d0c50598a54ec66c89346648f3e51ccea153dbc8ce
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.0.orig.tar.xz' flac_1.3.0.orig.tar.xz 1084256 SHA256:fa2d64aac1f77e31dfbb270aeb08f5b32e27036a52ad15e69a77e309528010dc
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.0-3.debian.tar.xz' flac_1.3.0-3.debian.tar.xz 14772 SHA256:4be6690850e4646764a740bdfa14688cd16c8913af5c9f26f539c30c69c879f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/flac/1.3.0-3/ (for browsing the source)
- https://sources.debian.net/src/flac/1.3.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/flac/1.3.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fontconfig=2.11.0-6.3+deb8u1`

Binary Packages:

- `fontconfig=2.11.0-6.3+deb8u1`
- `fontconfig-config=2.11.0-6.3+deb8u1`
- `libfontconfig1:amd64=2.11.0-6.3+deb8u1`

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

### `dpkg` source package: `freetype=2.5.2-3+deb8u2`

Binary Packages:

- `libfreetype6:amd64=2.5.2-3+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

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
$ apt-get source -qq --print-uris freetype=2.5.2-3+deb8u2
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.5.2-3+deb8u2.dsc' freetype_2.5.2-3+deb8u2.dsc 2283 SHA256:e63b0cc18482fe5971880271c2dbacd6957288608fef8c40fe127db79a9008dd
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.5.2.orig.tar.gz' freetype_2.5.2.orig.tar.gz 1971155 SHA256:5fda4996e43cfdf9b602a0eb5abde014f1a3c3b2d82bbb9b86942011c63f5c3a
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.5.2-3+deb8u2.diff.gz' freetype_2.5.2-3+deb8u2.diff.gz 70170 SHA256:0247f57efcb83b208fc1967520a53ecf21c5aca9ee2c433238914622e6938259
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.5.2-3+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.5.2-3+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.5.2-3+deb8u2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gdk-pixbuf=2.31.1-2+deb8u7`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.31.1-2+deb8u7`
- `libgdk-pixbuf2.0-common=2.31.1-2+deb8u7`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.31.1-2+deb8u7
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1-2+deb8u7.dsc' gdk-pixbuf_2.31.1-2+deb8u7.dsc 2873 SHA256:44783fee79e7771618adcab02a54d315579924c54e92f5345612d43519426bd8
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1.orig.tar.xz' gdk-pixbuf_2.31.1.orig.tar.xz 1340056 SHA256:25a75e3c61dac11e6ff6416ad846951ccafac6486b1c6a1bfb0b213b99db52cd
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.31.1-2+deb8u7.debian.tar.xz' gdk-pixbuf_2.31.1-2+deb8u7.debian.tar.xz 19404 SHA256:4b8882df906b40645d23faa5b1e0bd28a92e737b19957aa85eba615b0cfcef73
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdk-pixbuf/2.31.1-2+deb8u7/ (for browsing the source)
- https://sources.debian.net/src/gdk-pixbuf/2.31.1-2+deb8u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdk-pixbuf/2.31.1-2+deb8u7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `giflib=4.1.6-11+deb8u1`

Binary Packages:

- `libgif4:amd64=4.1.6-11+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgif4/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris giflib=4.1.6-11+deb8u1
'http://deb.debian.org/debian/pool/main/g/giflib/giflib_4.1.6-11+deb8u1.dsc' giflib_4.1.6-11+deb8u1.dsc 2039 SHA256:58f18c5c6bb24dbce21b13c7252319cb659fb0e86174ebbf8ccee8c7fea38cbb
'http://deb.debian.org/debian/pool/main/g/giflib/giflib_4.1.6.orig.tar.gz' giflib_4.1.6.orig.tar.gz 636030 SHA256:ceca77dcd29eb6f6d0336414dfecc9094413f71c3b589afcf96bb72fbfb08ce0
'http://deb.debian.org/debian/pool/main/g/giflib/giflib_4.1.6-11+deb8u1.debian.tar.xz' giflib_4.1.6-11+deb8u1.debian.tar.xz 9240 SHA256:c1b25cc01096d9d70e86035040358785bc6b620af5647c92af0ccb9c37d6892c
```

Other potentially useful URLs:

- https://sources.debian.net/src/giflib/4.1.6-11+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/giflib/4.1.6-11+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/giflib/4.1.6-11+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.42.1-1`

Binary Packages:

- `libglib2.0-0:amd64=2.42.1-1+b1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.42.1-1
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.42.1-1.dsc' glib2.0_2.42.1-1.dsc 3119 SHA256:61b01cb94e8bb8b9fdd1799b2e1bed907371dc45d364beec4b79a129745f588f
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.42.1.orig.tar.xz' glib2.0_2.42.1.orig.tar.xz 6985120 SHA256:8f3f0865280e45b8ce840e176ef83bcfd511148918cc8d39df2ee89b67dcf89a
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.42.1-1.debian.tar.xz' glib2.0_2.42.1-1.debian.tar.xz 68072 SHA256:1cd368c2bce6100c07b8a07ff7f3f38572679d88563356b8784560606fcfac56
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.42.1-1/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.42.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.42.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gtk+2.0=2.24.25-3+deb8u2`

Binary Packages:

- `libgtk2.0-0:amd64=2.24.25-3+deb8u2`
- `libgtk2.0-common=2.24.25-3+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

- `LGPL-2`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+2.0=2.24.25-3+deb8u2
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.25-3+deb8u2.dsc' gtk+2.0_2.24.25-3+deb8u2.dsc 3713 SHA256:4f34396790f0a739403088c883e56255fdc098f83881213fe9ede85df661d6da
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.25.orig.tar.xz' gtk+2.0_2.24.25.orig.tar.xz 13327832 SHA256:38af1020cb8ff3d10dda2c8807f11e92af9d2fa4045de61c62eedb7fbc7ea5b3
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.25-3+deb8u2.debian.tar.xz' gtk+2.0_2.24.25-3+deb8u2.debian.tar.xz 92176 SHA256:683ef3d1cd629f09035671b333b8c93b85a5a3836691d82385326444dfa57097
```

Other potentially useful URLs:

- https://sources.debian.net/src/gtk+2.0/2.24.25-3+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/gtk+2.0/2.24.25-3+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gtk+2.0/2.24.25-3+deb8u2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `harfbuzz=0.9.35-2`

Binary Packages:

- `libharfbuzz0b:amd64=0.9.35-2`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=0.9.35-2
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_0.9.35-2.dsc' harfbuzz_0.9.35-2.dsc 2303 SHA256:6e9428c29ecbb4beeb186a00121fda23362eebb4d389eb6f24f398cef1e1b9ec
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_0.9.35.orig.tar.bz2' harfbuzz_0.9.35.orig.tar.bz2 1165359 SHA256:0aa1a8aba6f502321cf6fef3c9d2c73dde48389c5ed1d3615a7691944c2a06ed
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_0.9.35-2.debian.tar.xz' harfbuzz_0.9.35-2.debian.tar.xz 7440 SHA256:a51eef8e3a9565865fc10d19fcd0d8d5be421a715f3f1445a9015274a8778532
```

Other potentially useful URLs:

- https://sources.debian.net/src/harfbuzz/0.9.35-2/ (for browsing the source)
- https://sources.debian.net/src/harfbuzz/0.9.35-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/harfbuzz/0.9.35-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `icu=52.1-8+deb8u7`

Binary Packages:

- `libicu52:amd64=52.1-8+deb8u7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=52.1-8+deb8u7
'http://deb.debian.org/debian/pool/main/i/icu/icu_52.1-8+deb8u7.dsc' icu_52.1-8+deb8u7.dsc 2015 SHA256:6962e61f1a0d2be8aba69ff118bfca747f92953fae78d37b15faa670c3ac0619
'http://deb.debian.org/debian/pool/main/i/icu/icu_52.1.orig.tar.gz' icu_52.1.orig.tar.gz 23875368 SHA256:2f4d5e68d4698e87759dbdc1a586d053d96935787f79961d192c477b029d8092
'http://deb.debian.org/debian/pool/main/i/icu/icu_52.1-8+deb8u7.debian.tar.xz' icu_52.1-8+deb8u7.debian.tar.xz 39320 SHA256:55e88af0c29a614f150f0b39579f1f946560dd75bc2b96ded28ebd96449f2692
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/52.1-8+deb8u7/ (for browsing the source)
- https://sources.debian.net/src/icu/52.1-8+deb8u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/52.1-8+deb8u7/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `jasper=1.900.1-debian1-2.4+deb8u6`

Binary Packages:

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

### `dpkg` source package: `java-atk-wrapper=0.30.5-1`

Binary Packages:

- `libatk-wrapper-java=0.30.5-1`
- `libatk-wrapper-java-jni:amd64=0.30.5-1`

Licenses: (parsed from: `/usr/share/doc/libatk-wrapper-java/copyright`, `/usr/share/doc/libatk-wrapper-java-jni/copyright`)

- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris java-atk-wrapper=0.30.5-1
'http://deb.debian.org/debian/pool/main/j/java-atk-wrapper/java-atk-wrapper_0.30.5-1.dsc' java-atk-wrapper_0.30.5-1.dsc 2222 SHA256:3ae50d3868b53fea19bc14fe85a294eda0514998691cdbe271f6f105b8132681
'http://deb.debian.org/debian/pool/main/j/java-atk-wrapper/java-atk-wrapper_0.30.5.orig.tar.xz' java-atk-wrapper_0.30.5.orig.tar.xz 259340 SHA256:0feec305ec253ae3f84b7faa67afe8f6693e9252e417bcb069174d9f1d03afd3
'http://deb.debian.org/debian/pool/main/j/java-atk-wrapper/java-atk-wrapper_0.30.5-1.debian.tar.bz2' java-atk-wrapper_0.30.5-1.debian.tar.bz2 3030 SHA256:bd12179c8cc9f03145edb706609402b40bfc629cae77ba1e438e27ea4669495c
```

Other potentially useful URLs:

- https://sources.debian.net/src/java-atk-wrapper/0.30.5-1/ (for browsing the source)
- https://sources.debian.net/src/java-atk-wrapper/0.30.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/java-atk-wrapper/0.30.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `java-common=0.52`

Binary Packages:

- `java-common=0.52`

Licenses: (parsed from: `/usr/share/doc/java-common/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris java-common=0.52
'http://deb.debian.org/debian/pool/main/j/java-common/java-common_0.52.dsc' java-common_0.52.dsc 2085 SHA256:348d6709b0d7ed5f4a944dc59f3cbf896f622b328d0c0bc4c2578980753b376d
'http://deb.debian.org/debian/pool/main/j/java-common/java-common_0.52.tar.xz' java-common_0.52.tar.xz 47380 SHA256:1118793faa2f41b9424c7014558713cdea0a401b3e2d904925fc20cf68464143
```

Other potentially useful URLs:

- https://sources.debian.net/src/java-common/0.52/ (for browsing the source)
- https://sources.debian.net/src/java-common/0.52/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/java-common/0.52/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jbigkit=2.1-3.1`

Binary Packages:

- `libjbig0:amd64=2.1-3.1`

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

### `dpkg` source package: `json-c=0.11-4`

Binary Packages:

- `libjson-c2:amd64=0.11-4`

Licenses: (parsed from: `/usr/share/doc/libjson-c2/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris json-c=0.11-4
'http://deb.debian.org/debian/pool/main/j/json-c/json-c_0.11-4.dsc' json-c_0.11-4.dsc 2139 SHA256:d21817e227168b4fed37e2e05c2dafbcf67e3148adf516c16c05d1014d1cbbba
'http://deb.debian.org/debian/pool/main/j/json-c/json-c_0.11.orig.tar.gz' json-c_0.11.orig.tar.gz 557263 SHA256:28dfc65145dc0d4df1dfe7701ac173c4e5f9347176c8983edbfac9149494448c
'http://deb.debian.org/debian/pool/main/j/json-c/json-c_0.11-4.debian.tar.xz' json-c_0.11-4.debian.tar.xz 272656 SHA256:4d6d8e24146b1a708b62a46b7061d0199f505cbdfe88221e10f1a8805071b984
```

Other potentially useful URLs:

- https://sources.debian.net/src/json-c/0.11-4/ (for browsing the source)
- https://sources.debian.net/src/json-c/0.11-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/json-c/0.11-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `lcms2=2.6-3+deb8u2`

Binary Packages:

- `liblcms2-2:amd64=2.6-3+deb8u2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

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

### `dpkg` source package: `libasyncns=0.8-5`

Binary Packages:

- `libasyncns0:amd64=0.8-5`

Licenses: (parsed from: `/usr/share/doc/libasyncns0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libasyncns=0.8-5
'http://deb.debian.org/debian/pool/main/liba/libasyncns/libasyncns_0.8-5.dsc' libasyncns_0.8-5.dsc 1909 SHA256:d4a02c1cca193187a9a75241950e5a31340ec204e7b41e7261934b86d752dc6f
'http://deb.debian.org/debian/pool/main/liba/libasyncns/libasyncns_0.8.orig.tar.gz' libasyncns_0.8.orig.tar.gz 341591 SHA256:4f1a66e746cbe54ff3c2fbada5843df4fbbbe7481d80be003e8d11161935ab74
'http://deb.debian.org/debian/pool/main/liba/libasyncns/libasyncns_0.8-5.debian.tar.xz' libasyncns_0.8-5.debian.tar.xz 4144 SHA256:aafa8cffc7139dc95b593674cd71e273e2503c65a3a7a36e29f21f8869b5889a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libasyncns/0.8-5/ (for browsing the source)
- https://sources.debian.net/src/libasyncns/0.8-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libasyncns/0.8-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libdrm=2.4.58-2`

Binary Packages:

- `libdrm2:amd64=2.4.58-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libdrm=2.4.58-2
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.58-2.dsc' libdrm_2.4.58-2.dsc 3002 SHA256:1286092e26403ea459a77df792fabfcad35ae68c05313d60362947d8eaa04c72
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.58.orig.tar.gz' libdrm_2.4.58.orig.tar.gz 732395 SHA256:e6f6901b0dd431d4e21f6e81ae5a5aef65885ed5f066e8d9751ca69ba9a71186
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.58-2.diff.gz' libdrm_2.4.58-2.diff.gz 18700 SHA256:51f9a553461a26cd3757c05e792187c3fdec4744cefda6ce1e103f201ef7c0f0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdrm/2.4.58-2/ (for browsing the source)
- https://sources.debian.net/src/libdrm/2.4.58-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdrm/2.4.58-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libgcrypt20=1.6.3-2+deb8u5`

Binary Packages:

- `libgcrypt20:amd64=1.6.3-2+deb8u5`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libgcrypt20/1.6.3-2+deb8u5/


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

### `dpkg` source package: `libice=2:1.0.9-1`

Binary Packages:

- `libice6:amd64=2:1.0.9-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-1
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9-1.dsc' libice_1.0.9-1.dsc 2140 SHA256:f90a79944f147b5db208677d92381fd0886c201616172bac0b28ef0e85912ebd
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://deb.debian.org/debian/pool/main/libi/libice/libice_1.0.9-1.diff.gz' libice_1.0.9-1.diff.gz 6260 SHA256:85d68a69d5e6b25b352eb98c6c33fa7a324da8dd913d7e84a049852fb87287e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libice/2:1.0.9-1/ (for browsing the source)
- https://sources.debian.net/src/libice/2:1.0.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libice/2:1.0.9-1/ (for access to the source package after it no longer exists in the archive)

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

- `libjpeg62-turbo:amd64=1:1.3.1-12+deb8u2`

Licenses: (parsed from: `/usr/share/doc/libjpeg62-turbo/copyright`)

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

### `dpkg` source package: `libogg=1.3.2-1`

Binary Packages:

- `libogg0:amd64=1.3.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libogg=1.3.2-1
'http://deb.debian.org/debian/pool/main/libo/libogg/libogg_1.3.2-1.dsc' libogg_1.3.2-1.dsc 1230 SHA256:dacc2059f8f92d1f6b18805432f2f40ac45fb9d52a1a61f14dc8c7c6a1aecb58
'http://deb.debian.org/debian/pool/main/libo/libogg/libogg_1.3.2.orig.tar.gz' libogg_1.3.2.orig.tar.gz 557232 SHA256:bf253517df60ef1e6f5ae328bac7477595465de30638818948574e05f502dfa3
'http://deb.debian.org/debian/pool/main/libo/libogg/libogg_1.3.2-1.diff.gz' libogg_1.3.2-1.diff.gz 6824 SHA256:9bee2f473a5ed92f1c744105447f15fe38feea8935e740a9eea2d840fa2d15c7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libogg/1.3.2-1/ (for browsing the source)
- https://sources.debian.net/src/libogg/1.3.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libogg/1.3.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng=1.2.50-2+deb8u3`

Binary Packages:

- `libpng12-0:amd64=1.2.50-2+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libpng12-0/copyright`)

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

### `dpkg` source package: `libsm=2:1.2.2-1`

Binary Packages:

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

### `dpkg` source package: `libsndfile=1.0.25-9.1+deb8u4`

Binary Packages:

- `libsndfile1:amd64=1.0.25-9.1+deb8u4`

Licenses: (parsed from: `/usr/share/doc/libsndfile1/copyright`)

- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libsndfile=1.0.25-9.1+deb8u4
'http://security.debian.org/debian-security/pool/updates/main/libs/libsndfile/libsndfile_1.0.25-9.1+deb8u4.dsc' libsndfile_1.0.25-9.1+deb8u4.dsc 2153 SHA256:a6f5600c0dca8db6ba83d318b023dea53f446aa9e1fda16e079966efd852cf67
'http://security.debian.org/debian-security/pool/updates/main/libs/libsndfile/libsndfile_1.0.25.orig.tar.gz' libsndfile_1.0.25.orig.tar.gz 1060692 SHA256:59016dbd326abe7e2366ded5c344c853829bebfd1702ef26a07ef662d6aa4882
'http://security.debian.org/debian-security/pool/updates/main/libs/libsndfile/libsndfile_1.0.25-9.1+deb8u4.debian.tar.xz' libsndfile_1.0.25-9.1+deb8u4.debian.tar.xz 15512 SHA256:3b35e907aeba4e6bfff74374187b3b06a6cc495ce36d4aee7a66a362557d4f61
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsndfile/1.0.25-9.1+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/libsndfile/1.0.25-9.1+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsndfile/1.0.25-9.1+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libssh2=1.4.3-4.1+deb8u3`

Binary Packages:

- `libssh2-1:amd64=1.4.3-4.1+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libssh2/1.4.3-4.1+deb8u3/


### `dpkg` source package: `libtasn1-6=4.2-3+deb8u3`

Binary Packages:

- `libtasn1-6:amd64=4.2-3+deb8u3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.2-3+deb8u3
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.2-3+deb8u3.dsc' libtasn1-6_4.2-3+deb8u3.dsc 2607 SHA256:dee600f7bdacd1fa75d40a13425e6c81d36b979fd23aab468000a1bfc18706ba
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.2.orig.tar.gz' libtasn1-6_4.2.orig.tar.gz 1866192 SHA256:693b41cb36c2ac02d5990180b0712a79a591168e93d85f7fcbb75a0a0be4cdbb
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.2-3+deb8u3.debian.tar.xz' libtasn1-6_4.2-3+deb8u3.debian.tar.xz 59144 SHA256:59ba69bafbe22542f58bc63eab30b70b5ce15673f8b7b8332c21b72e33572d28
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.2-3+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.2-3+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.2-3+deb8u3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libvorbis=1.3.4-2+deb8u1`

Binary Packages:

- `libvorbis0a:amd64=1.3.4-2+deb8u1`
- `libvorbisenc2:amd64=1.3.4-2+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libvorbis=1.3.4-2+deb8u1
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.4-2+deb8u1.dsc' libvorbis_1.3.4-2+deb8u1.dsc 2455 SHA256:0f7d44d5b182d060206437ae92a1d2e5f6ef74637195c7554483a7134d81e8b8
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.4.orig.tar.gz' libvorbis_1.3.4.orig.tar.gz 1632091 SHA256:eee09a0a13ec38662ff949168fe897a25d2526529bc7e805305f381c219a1ecb
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.4-2+deb8u1.debian.tar.xz' libvorbis_1.3.4-2+deb8u1.debian.tar.xz 12664 SHA256:09ce07a86b4be1764d6a7c4bfcdca9c528fa10e947c695ce8b7dac0548fad7f0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvorbis/1.3.4-2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libvorbis/1.3.4-2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvorbis/1.3.4-2+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.6.2-3+deb8u2`

Binary Packages:

- `libx11-6:amd64=2:1.6.2-3+deb8u2`
- `libx11-data=2:1.6.2-3+deb8u2`
- `libx11-xcb1:amd64=2:1.6.2-3+deb8u2`

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

- `libxcb-dri2-0:amd64=1.10-3+b1`
- `libxcb-dri3-0:amd64=1.10-3+b1`
- `libxcb-glx0:amd64=1.10-3+b1`
- `libxcb-present0:amd64=1.10-3+b1`
- `libxcb-render0:amd64=1.10-3+b1`
- `libxcb-shm0:amd64=1.10-3+b1`
- `libxcb-sync1:amd64=1.10-3+b1`
- `libxcb1:amd64=1.10-3+b1`

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

### `dpkg` source package: `libxcomposite=1:0.4.4-1`

Binary Packages:

- `libxcomposite1:amd64=1:0.4.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcomposite=1:0.4.4-1
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.dsc' libxcomposite_0.4.4-1.dsc 2170 SHA256:b304040285ca2d6e2667bfec45097814bdd017380c629a5972993407c656469a
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4.orig.tar.gz' libxcomposite_0.4.4.orig.tar.gz 354584 SHA256:83c04649819c6f52cda1b0ce8bcdcc48ad8618428ad803fb07f20b802f1bdad1
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.diff.gz' libxcomposite_0.4.4-1.diff.gz 15633 SHA256:09fe6dd7d98d935e7307d57f926912d477b929f06c159962840d3a398f376988
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcomposite/1:0.4.4-1/ (for browsing the source)
- https://sources.debian.net/src/libxcomposite/1:0.4.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcomposite/1:0.4.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcursor=1:1.1.14-1+deb8u2`

Binary Packages:

- `libxcursor1:amd64=1:1.1.14-1+deb8u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcursor=1:1.1.14-1+deb8u2
'http://security.debian.org/debian-security/pool/updates/main/libx/libxcursor/libxcursor_1.1.14-1+deb8u2.dsc' libxcursor_1.1.14-1+deb8u2.dsc 2334 SHA256:6254d854b9bfbf522a49e0b8f9c5213e58e83d8f27677cc24518b586673de8ff
'http://security.debian.org/debian-security/pool/updates/main/libx/libxcursor/libxcursor_1.1.14.orig.tar.gz' libxcursor_1.1.14.orig.tar.gz 374910 SHA256:be0954faf274969ffa6d95b9606b9c0cfee28c13b6fc014f15606a0c8b05c17b
'http://security.debian.org/debian-security/pool/updates/main/libx/libxcursor/libxcursor_1.1.14-1+deb8u2.diff.gz' libxcursor_1.1.14-1+deb8u2.diff.gz 19797 SHA256:d9238239b35374e4fb433999698d524b7eded95edca46ec248bb369b677920fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcursor/1:1.1.14-1+deb8u2/ (for browsing the source)
- https://sources.debian.net/src/libxcursor/1:1.1.14-1+deb8u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcursor/1:1.1.14-1+deb8u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdamage=1:1.1.4-2`

Binary Packages:

- `libxdamage1:amd64=1:1.1.4-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdamage=1:1.1.4-2
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4-2.dsc' libxdamage_1.1.4-2.dsc 2127 SHA256:43cbefb5c69f51d89a11cf84718fe0c42058fc9b6ec7c0076e7c37b9e829feb5
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4.orig.tar.gz' libxdamage_1.1.4.orig.tar.gz 339060 SHA256:4bb3e9d917f5f593df2277d452926ee6ad96de7b7cd1017cbcf4579fe5d3442b
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4-2.diff.gz' libxdamage_1.1.4-2.diff.gz 14930 SHA256:d238c1a266c30cd124ede7e6c86635bfaa108fa552c4a82919101cebf22670e9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxdamage/1:1.1.4-2/ (for browsing the source)
- https://sources.debian.net/src/libxdamage/1:1.1.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxdamage/1:1.1.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdmcp=1:1.1.1-1`

Binary Packages:

- `libxdmcp6:amd64=1:1.1.1-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.1-1
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.1-1.dsc' libxdmcp_1.1.1-1.dsc 2102 SHA256:1713ac047ad1d235fe51476f2224d0dc0f170e9623c0735d1941c474942b24d3
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.1.orig.tar.gz' libxdmcp_1.1.1.orig.tar.gz 376525 SHA256:ae6e677911e2696a2976b2f565f116ba9ce99e89cc7e140c4a791270c3aff96f
'http://deb.debian.org/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.1-1.diff.gz' libxdmcp_1.1.1-1.diff.gz 14891 SHA256:bb79bc8439d63d5bed6bf7544f1ed14b4606c246f724523da2fa921cc9929f19
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxdmcp/1:1.1.1-1/ (for browsing the source)
- https://sources.debian.net/src/libxdmcp/1:1.1.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxdmcp/1:1.1.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

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

### `dpkg` source package: `libxfixes=1:5.0.1-2+deb8u1`

Binary Packages:

- `libxfixes3:amd64=1:5.0.1-2+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxfixes=1:5.0.1-2+deb8u1
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.1-2+deb8u1.dsc' libxfixes_5.0.1-2+deb8u1.dsc 2204 SHA256:6ec8d4442582687a427fcb5f422324f34718afc55f44ec23017a0e4f9022fd8c
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.1.orig.tar.gz' libxfixes_5.0.1.orig.tar.gz 352057 SHA256:81b692856c0e7ab2778a34a32aa6b3f455b9b58cf388f009cba872ed933ae9c0
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.1-2+deb8u1.diff.gz' libxfixes_5.0.1-2+deb8u1.diff.gz 6911 SHA256:32c2763fe19f1ecb01efc47d6fe0278dc04b9ea9036762ed125a3cdc1cb338a9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxfixes/1:5.0.1-2+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libxfixes/1:5.0.1-2+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxfixes/1:5.0.1-2+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxi=2:1.7.4-1+deb8u1`

Binary Packages:

- `libxi6:amd64=2:1.7.4-1+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxi=2:1.7.4-1+deb8u1
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.4-1+deb8u1.dsc' libxi_1.7.4-1+deb8u1.dsc 2358 SHA256:f6467707d533f5dc4544363b80ca4d2ec9207d847aa1a20a423f68ba24d9312d
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.4.orig.tar.gz' libxi_1.7.4.orig.tar.gz 574645 SHA256:ddf7c56bc0d7206308c22365f694c1a1f177eb3b801fc22d42ead378440aca54
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.4-1+deb8u1.diff.gz' libxi_1.7.4-1+deb8u1.diff.gz 22247 SHA256:6e83bacce44189770e78bfe9843806eba7e3e3a140e9ffe17a66fba657ee185a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxi/2:1.7.4-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libxi/2:1.7.4-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxi/2:1.7.4-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxinerama=2:1.1.3-1`

Binary Packages:

- `libxinerama1:amd64=2:1.1.3-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxinerama=2:1.1.3-1
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.3-1.dsc' libxinerama_1.1.3-1.dsc 2198 SHA256:4cf9a3558bd7ce1b4f55a581175c05e4b4a172364458a21ff4b657b714688fbb
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.3.orig.tar.gz' libxinerama_1.1.3.orig.tar.gz 350141 SHA256:0ba243222ae5aba4c6a3d7a394c32c8b69220a6872dbb00b7abae8753aca9a44
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.3-1.diff.gz' libxinerama_1.1.3-1.diff.gz 15738 SHA256:2b1487e3511ddabfec666a62f6e5e8ac4f97536b0d53c51f7bf4cbe07508a130
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxinerama/2:1.1.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxinerama/2:1.1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxinerama/2:1.1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxml2=2.9.1+dfsg1-5+deb8u7`

Binary Packages:

- `libxml2:amd64=2.9.1+dfsg1-5+deb8u7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxml2/2.9.1+dfsg1-5+deb8u7/


### `dpkg` source package: `libxrandr=2:1.4.2-1+deb8u1`

Binary Packages:

- `libxrandr2:amd64=2:1.4.2-1+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrandr=2:1.4.2-1+deb8u1
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.4.2-1+deb8u1.dsc' libxrandr_1.4.2-1+deb8u1.dsc 2158 SHA256:4e50b61d9e5aae141587336ad93ef429e53ea7d7fdce96091da8313fc2787211
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.4.2.orig.tar.gz' libxrandr_1.4.2.orig.tar.gz 384543 SHA256:fdccecde43daf8caf5697884fe7855c6560e4804957c57f71f65439544b847d4
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.4.2-1+deb8u1.diff.gz' libxrandr_1.4.2-1+deb8u1.diff.gz 18675 SHA256:d5891bb8d4ef14fdbe886d1964a350c4d8f0d6aca649911a43bf541a267ff6a9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxrandr/2:1.4.2-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libxrandr/2:1.4.2-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxrandr/2:1.4.2-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxrender=1:0.9.8-1`

Binary Packages:

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

### `dpkg` source package: `libxshmfence=1.1-4`

Binary Packages:

- `libxshmfence1:amd64=1.1-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxshmfence=1.1-4
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.1-4.dsc' libxshmfence_1.1-4.dsc 2125 SHA256:b4d136498a488b4c946871c2ec25c6df882558dce587be844d213a98fcdbce7d
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.1.orig.tar.gz' libxshmfence_1.1.orig.tar.gz 353601 SHA256:36a6c67c71c6f262be0f2f29349d33ad157ba1fea64a55acd35b90c3816a4cdc
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.1-4.diff.gz' libxshmfence_1.1-4.diff.gz 2483 SHA256:10f0926dd70c1cced73470c012e8b021c32d0badffecc2a3509b259c332aaf3c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxshmfence/1.1-4/ (for browsing the source)
- https://sources.debian.net/src/libxshmfence/1.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxshmfence/1.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxtst=2:1.2.2-1+deb8u1`

Binary Packages:

- `libxtst6:amd64=2:1.2.2-1+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxtst=2:1.2.2-1+deb8u1
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.2-1+deb8u1.dsc' libxtst_1.2.2-1+deb8u1.dsc 2371 SHA256:a4352ba73052ae9772a75320a08733db0b8d41803b8b19f230291a5900ec0fb3
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.2.orig.tar.gz' libxtst_1.2.2.orig.tar.gz 392569 SHA256:221838960c7b9058cd6795c1c3ee8e25bae1c68106be314bc3036a4f26be0e6c
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.2-1+deb8u1.diff.gz' libxtst_1.2.2-1+deb8u1.diff.gz 17982 SHA256:12477b5b066e5a551a60add9792d5d38920580d6f2014ae3c060491ea2c25249
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxtst/2:1.2.2-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/libxtst/2:1.2.2-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxtst/2:1.2.2-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxxf86vm=1:1.1.3-1`

Binary Packages:

- `libxxf86vm1:amd64=1:1.1.3-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxxf86vm=1:1.1.3-1
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.3-1.dsc' libxxf86vm_1.1.3-1.dsc 2094 SHA256:4b75f3b4f18f5c80a240e279e3edd222523b791e2ed2657a45716310fe7db430
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.3.orig.tar.gz' libxxf86vm_1.1.3.orig.tar.gz 354937 SHA256:26ffbb4baaee0256ef9cdd7b8631aa3fa7bbb32e87125cfdb37fa644a623570e
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.3-1.diff.gz' libxxf86vm_1.1.3-1.diff.gz 5115 SHA256:5b51cc770666430c2c40e9a58395c72d7591f81bc5e7fd494397bbaf794b38e2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxxf86vm/1:1.1.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxxf86vm/1:1.1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxxf86vm/1:1.1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lksctp-tools=1.0.16+dfsg-2`

Binary Packages:

- `libsctp1:amd64=1.0.16+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libsctp1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris lksctp-tools=1.0.16+dfsg-2
'http://deb.debian.org/debian/pool/main/l/lksctp-tools/lksctp-tools_1.0.16+dfsg-2.dsc' lksctp-tools_1.0.16+dfsg-2.dsc 1999 SHA256:bf6eba41ed567134acf657a99c4960d8d04d59972469496cf10520ac8e784009
'http://deb.debian.org/debian/pool/main/l/lksctp-tools/lksctp-tools_1.0.16+dfsg.orig.tar.gz' lksctp-tools_1.0.16+dfsg.orig.tar.gz 206656 SHA256:6935a57bdc052805796f538257eb78e23af02481e01f3d72dc0fa00688bdd502
'http://deb.debian.org/debian/pool/main/l/lksctp-tools/lksctp-tools_1.0.16+dfsg-2.debian.tar.xz' lksctp-tools_1.0.16+dfsg-2.debian.tar.xz 9240 SHA256:d14deebc1dc8f0b8937c2efdd45a9d0075c48979219dbd23f23f3a77dd5ca856
```

Other potentially useful URLs:

- https://sources.debian.net/src/lksctp-tools/1.0.16+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/lksctp-tools/1.0.16+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lksctp-tools/1.0.16+dfsg-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mesa=10.3.2-1+deb8u1`

Binary Packages:

- `libgl1-mesa-glx:amd64=10.3.2-1+deb8u1`
- `libglapi-mesa:amd64=10.3.2-1+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libgl1-mesa-glx/copyright`, `/usr/share/doc/libglapi-mesa/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris mesa=10.3.2-1+deb8u1
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_10.3.2-1+deb8u1.dsc' mesa_10.3.2-1+deb8u1.dsc 5461 SHA256:f9b14951df390dc25aac9562e08237e162e06b9526b4136ac58e0df27bea7d36
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_10.3.2.orig.tar.gz' mesa_10.3.2.orig.tar.gz 9649735 SHA256:e65f8e691f06f111c1aeb3a376b13c9cc88cb162bee2709e0e7e6b0e6628ca75
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_10.3.2-1+deb8u1.diff.gz' mesa_10.3.2-1+deb8u1.diff.gz 82262 SHA256:e9d66405fe9b41a41a022ba452769a4627c97c289d92b1c27dca60c6dccea997
```

Other potentially useful URLs:

- https://sources.debian.net/src/mesa/10.3.2-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/mesa/10.3.2-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mesa/10.3.2-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `nspr=2:4.12-1+debu8u1`

Binary Packages:

- `libnspr4:amd64=2:4.12-1+debu8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.12-1+debu8u1
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12-1+debu8u1.dsc' nspr_4.12-1+debu8u1.dsc 1792 SHA256:421dcd3e6bf4c26793d7c06dddf28945d4cb46829b06160d80a07a8b26244563
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12.orig.tar.gz' nspr_4.12.orig.tar.gz 1135458 SHA256:e0b10a1e569153668ff8bdea6c7e491b389fab69c2f18285a1ebf7c2ea4269de
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.12-1+debu8u1.debian.tar.xz' nspr_4.12-1+debu8u1.debian.tar.xz 14276 SHA256:d69e39fd076a58b4aab9809d7defe6505fc327edc421bdfc5b8348ff2d843cf3
```

Other potentially useful URLs:

- https://sources.debian.net/src/nspr/2:4.12-1+debu8u1/ (for browsing the source)
- https://sources.debian.net/src/nspr/2:4.12-1+debu8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nspr/2:4.12-1+debu8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nss=2:3.26-1+debu8u4`

Binary Packages:

- `libnss3:amd64=2:3.26-1+debu8u4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/nss/2:3.26-1+debu8u4/


### `dpkg` source package: `openjdk-7=7u221-2.6.18-1~deb8u1`

Binary Packages:

- `openjdk-7-jre:amd64=7u221-2.6.18-1~deb8u1`
- `openjdk-7-jre-headless:amd64=7u221-2.6.18-1~deb8u1`

Licenses: (parsed from: `/usr/share/doc/openjdk-7-jre/copyright`, `/usr/share/doc/openjdk-7-jre-headless/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openjdk-7/7u221-2.6.18-1~deb8u1/


### `dpkg` source package: `openldap=2.4.40+dfsg-1+deb8u4`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.40+dfsg-1+deb8u4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.40+dfsg-1+deb8u4
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.40+dfsg-1+deb8u4.dsc' openldap_2.4.40+dfsg-1+deb8u4.dsc 2856 SHA256:adb061ec11d3ec69644919ff7a35ae451c30a0891c269fe00b5043649083bcba
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.40+dfsg.orig.tar.gz' openldap_2.4.40+dfsg.orig.tar.gz 4797667 SHA256:86c0326dc3dc5f1a9b3c25f7106b96f3eafcdf5da090b1fc586dec57d56e0e7f
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.40+dfsg-1+deb8u4.diff.gz' openldap_2.4.40+dfsg-1+deb8u4.diff.gz 181350 SHA256:dffbdc8a502302724d3b2faf1c08a0383daf41cc690ffac47516813048b7d372
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.40+dfsg-1+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.40+dfsg-1+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.40+dfsg-1+deb8u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.0.1t-1+deb8u11`

Binary Packages:

- `libssl1.0.0:amd64=1.0.1t-1+deb8u11`
- `openssl=1.0.1t-1+deb8u11`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openssl/1.0.1t-1+deb8u11/


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

### `dpkg` source package: `pcsc-lite=1.8.13-1+deb8u1`

Binary Packages:

- `libpcsclite1:amd64=1.8.13-1+deb8u1`

Licenses: (parsed from: `/usr/share/doc/libpcsclite1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris pcsc-lite=1.8.13-1+deb8u1
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.13-1+deb8u1.dsc' pcsc-lite_1.8.13-1+deb8u1.dsc 2252 SHA256:325efa1f879f04a80447077b4fae1bcac2b6886cd9c7b3459ee22ca3050df268
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.13.orig.tar.bz2' pcsc-lite_1.8.13.orig.tar.bz2 584083 SHA256:f315047e808d63a3262c4a040f77548af2e04d1fd707e0c2759369b926fbbc3b
'http://deb.debian.org/debian/pool/main/p/pcsc-lite/pcsc-lite_1.8.13-1+deb8u1.debian.tar.xz' pcsc-lite_1.8.13-1+deb8u1.debian.tar.xz 15700 SHA256:61e89cdd33e5f189de19ad3465d3bd40f2a5326c84dcc04e8d6519f7a74edf66
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcsc-lite/1.8.13-1+deb8u1/ (for browsing the source)
- https://sources.debian.net/src/pcsc-lite/1.8.13-1+deb8u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcsc-lite/1.8.13-1+deb8u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.20.2-3+deb8u12`

Binary Packages:

- `perl-base=5.20.2-3+deb8u12`

Licenses: (parsed from: `/usr/share/doc/perl-base/copyright`)

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

### `dpkg` source package: `pulseaudio=5.0-13`

Binary Packages:

- `libpulse0:amd64=5.0-13`

Licenses: (parsed from: `/usr/share/doc/libpulse0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris pulseaudio=5.0-13
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_5.0-13.dsc' pulseaudio_5.0-13.dsc 4694 SHA256:9e5e4f29305b631a6b6bfc975136994498480f46fb482656f99911f628760a3a
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_5.0.orig.tar.xz' pulseaudio_5.0.orig.tar.xz 1455428 SHA256:99c13a8b1249ddbd724f195579df79484e9af6418cecf6a15f003a7f36caf939
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_5.0-13.debian.tar.xz' pulseaudio_5.0-13.debian.tar.xz 41296 SHA256:689a61a48d6042cb26dbe2c73361edea12459301718bbf5ae84df24758605a03
```

Other potentially useful URLs:

- https://sources.debian.net/src/pulseaudio/5.0-13/ (for browsing the source)
- https://sources.debian.net/src/pulseaudio/5.0-13/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pulseaudio/5.0-13/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `sqlite3=3.8.7.1-1+deb8u4`

Binary Packages:

- `libsqlite3-0:amd64=3.8.7.1-1+deb8u4`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.8.7.1-1+deb8u4
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1-1+deb8u4.dsc' sqlite3_3.8.7.1-1+deb8u4.dsc 2705 SHA256:e4b52b1144ea546f92e1f7e7239b1f45a6ff83732bd03d5b549ab953274ee293
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1.orig-www.tar.bz2' sqlite3_3.8.7.1.orig-www.tar.bz2 3337784 SHA256:e642657752f20144f42d002895510ea635e0384b14f276f1a2f281b73252bc64
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1.orig.tar.bz2' sqlite3_3.8.7.1.orig.tar.bz2 4082068 SHA256:2632a999feba925aa0f1828fa669a091b165a719676765fb542f538345bfa7b9
'http://security.debian.org/debian-security/pool/updates/main/s/sqlite3/sqlite3_3.8.7.1-1+deb8u4.debian.tar.xz' sqlite3_3.8.7.1-1+deb8u4.debian.tar.xz 24436 SHA256:8d9be049e9abe6221b39f84d564ff310ecbbd328bd5876b672f8294e55ba1953
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.8.7.1-1+deb8u4/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.8.7.1-1+deb8u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.8.7.1-1+deb8u4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `tcp-wrappers=7.6.q-25`

Binary Packages:

- `libwrap0:amd64=7.6.q-25`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcp-wrappers=7.6.q-25
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-25.dsc' tcp-wrappers_7.6.q-25.dsc 1132 SHA256:77e162fcb2fcbe34448cf445f10e746d417a61ec0d79f46fd8ac5883ffc720c7
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q.orig.tar.gz' tcp-wrappers_7.6.q.orig.tar.gz 99438 SHA256:9543d7adedf78a6de0b221ccbbd1952e08b5138717f4ade814039bb489a4315d
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-25.debian.tar.xz' tcp-wrappers_7.6.q-25.debian.tar.xz 35504 SHA256:fb7bb73c586a0c00c76c730ab93ffd73c300e8c4fd83df76222e305a2466c7bb
```

Other potentially useful URLs:

- https://sources.debian.net/src/tcp-wrappers/7.6.q-25/ (for browsing the source)
- https://sources.debian.net/src/tcp-wrappers/7.6.q-25/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tcp-wrappers/7.6.q-25/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.0.3-12.3+deb8u8`

Binary Packages:

- `libtiff5:amd64=4.0.3-12.3+deb8u8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tiff/4.0.3-12.3+deb8u8/


### `dpkg` source package: `tzdata=2019a-0+deb8u1`

Binary Packages:

- `tzdata=2019a-0+deb8u1`
- `tzdata-java=2019a-0+deb8u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tzdata/2019a-0+deb8u1/


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

### `dpkg` source package: `unzip=6.0-16+deb8u3`

Binary Packages:

- `unzip=6.0-16+deb8u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-16+deb8u3
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-16+deb8u3.dsc' unzip_6.0-16+deb8u3.dsc 1339 SHA256:b1a3191a99f7c245d8e29ee0866d5c2b8e9deb191095ae8312dd59a95e616b79
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-16+deb8u3.debian.tar.xz' unzip_6.0-16+deb8u3.debian.tar.xz 16120 SHA256:8e50ca0ac7d8e00d595a329c91dec7a7e1a1b998857f54062cd26b88c2e3d3b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-16+deb8u3/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-16+deb8u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-16+deb8u3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `wget=1.16-1+deb8u6`

Binary Packages:

- `wget=1.16-1+deb8u6`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.16-1+deb8u6
'http://security.debian.org/debian-security/pool/updates/main/w/wget/wget_1.16-1+deb8u6.dsc' wget_1.16-1+deb8u6.dsc 1942 SHA256:df5fb85bc5e7d4230ca5064415f70846d33f7a3222f45156b302d5e699257653
'http://security.debian.org/debian-security/pool/updates/main/w/wget/wget_1.16.orig.tar.gz' wget_1.16.orig.tar.gz 3325041 SHA256:b977fc10ac7a72d987d48136251aeb332f2dced1aabd50d6d56bdf72e2b79101
'http://security.debian.org/debian-security/pool/updates/main/w/wget/wget_1.16-1+deb8u6.debian.tar.xz' wget_1.16-1+deb8u6.debian.tar.xz 24260 SHA256:88c778c49633860b8b6fb5966bfaf72e15e543f19dca456892285cb8b37eef16
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.16-1+deb8u6/ (for browsing the source)
- https://sources.debian.net/src/wget/1.16-1+deb8u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.16-1+deb8u6/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xz-utils=5.1.1alpha+20120614-2`

Binary Packages:

- `liblzma5:amd64=5.1.1alpha+20120614-2+b3`
- `xz-utils=5.1.1alpha+20120614-2+b3`

Licenses: (parsed from: `/usr/share/doc/liblzma5/copyright`, `/usr/share/doc/xz-utils/copyright`)

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

### `dpkg` source package: `zlib=1:1.2.8.dfsg-2`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.8.dfsg-2
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-2.dsc' zlib_1.2.8.dfsg-2.dsc 2458 SHA256:5dddd28d2b15fc0881177d720a3b5bf41a87eee7aaec296e4b20719a9fe18b7e
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg.orig.tar.gz' zlib_1.2.8.dfsg.orig.tar.gz 361943 SHA256:2caecc2c3f1ef8b87b8f72b128a03e61c307e8c14f5ec9b422ef7914ba75cf9f
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.8.dfsg-2.debian.tar.xz' zlib_1.2.8.dfsg-2.debian.tar.xz 14768 SHA256:39af7ea4b264c229f856ed342bb316a796cb2f1e1278a059f2dc5a4f3ffc9f31
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.8.dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.8.dfsg-2/ (for access to the source package after it no longer exists in the archive)
