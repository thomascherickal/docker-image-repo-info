# `nuxeo:10.10`

## Docker Metadata

- Image ID: `sha256:9287e15ff89c604c53c176308470144ed36fd42083de4c58627f6aad3597d6d2`
- Created: `2020-01-23T04:00:28.333725844Z`
- Virtual Size: ~ 1.67 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
- Command: `["nuxeoctl","console"]`
- Environment:
  - `PATH=/opt/nuxeo/server/bin:/usr/local/openjdk-8/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `JAVA_HOME=/usr/local/openjdk-8`
  - `JAVA_VERSION=8u242`
  - `JAVA_BASE_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u242-b08/OpenJDK8U-jdk_`
  - `JAVA_URL_VERSION=8u242b08`
  - `NUXEO_USER=nuxeo`
  - `NUXEO_HOME=/opt/nuxeo/server`
  - `HOME=/opt/nuxeo/server`
  - `NUXEO_CONF=/etc/nuxeo/nuxeo.conf`

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

### `dpkg` source package: `adwaita-icon-theme=3.22.0-1+deb9u1`

Binary Packages:

- `adwaita-icon-theme=3.22.0-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/adwaita-icon-theme/copyright`)

- `CC-BY-3.0-US`
- `CC-BY-SA-2.0-IT`
- `CC-BY-SA-2.0-IT,`
- `CC-BY-SA-3.0`
- `CC-BY-SA-3.0-US`
- `CC-BY-SA-3.0-Unported`
- `GFDL-1.2`
- `GFDL-1.2+`
- `GPL`
- `GPL-unspecified`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris adwaita-icon-theme=3.22.0-1+deb9u1
'http://deb.debian.org/debian/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.22.0-1+deb9u1.dsc' adwaita-icon-theme_3.22.0-1+deb9u1.dsc 2003 SHA256:986b64e91644161b76f8bd5046ee6d66abe18caa8dd6d1a40299214874ad365b
'http://deb.debian.org/debian/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.22.0.orig.tar.xz' adwaita-icon-theme_3.22.0.orig.tar.xz 18395856 SHA256:c18bf6e26087d9819a962c77288b291efab25d0419b73d909dd771716a45dcb7
'http://deb.debian.org/debian/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.22.0-1+deb9u1.debian.tar.xz' adwaita-icon-theme_3.22.0-1+deb9u1.debian.tar.xz 28744 SHA256:ee36f3caa32b15f60ef4155805a56fb51272bd0dc43933c9468e06fa64f2251d
```

Other potentially useful URLs:

- https://sources.debian.net/src/adwaita-icon-theme/3.22.0-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/adwaita-icon-theme/3.22.0-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adwaita-icon-theme/3.22.0-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `alsa-lib=1.1.3-5`

Binary Packages:

- `libasound2:amd64=1.1.3-5`
- `libasound2-data=1.1.3-5`

Licenses: (parsed from: `/usr/share/doc/libasound2/copyright`, `/usr/share/doc/libasound2-data/copyright`)

- `LGPL-2.1`
- `LPGL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris alsa-lib=1.1.3-5
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.1.3-5.dsc' alsa-lib_1.1.3-5.dsc 2497 SHA256:6d08434ad6ff6bd9e766462d88a0967f9a1628f47e507b208817499696ed1f52
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.1.3.orig.tar.bz2' alsa-lib_1.1.3.orig.tar.bz2 962001 SHA256:71282502184c592c1a008e256c22ed0ba5728ca65e05273ceb480c70f515969c
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.1.3-5.debian.tar.xz' alsa-lib_1.1.3-5.debian.tar.xz 134356 SHA256:9be3fd176b3f846c11af15c0a2a93a4c3f1b75796287807fe5ccf700f0b0a1d6
```

Other potentially useful URLs:

- https://sources.debian.net/src/alsa-lib/1.1.3-5/ (for browsing the source)
- https://sources.debian.net/src/alsa-lib/1.1.3-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/alsa-lib/1.1.3-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apparmor=2.11.0-3+deb9u2`

Binary Packages:

- `libapparmor1:amd64=2.11.0-3+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libapparmor1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris apparmor=2.11.0-3+deb9u2
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.11.0-3+deb9u2.dsc' apparmor_2.11.0-3+deb9u2.dsc 3126 SHA256:ba1462cce0c4dae145b40915142b01acb9bb91955a36997f1b088a6fe5dfb0bf
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.11.0.orig.tar.gz' apparmor_2.11.0.orig.tar.gz 5013297 SHA256:b1c489ea11e7771b8e6b181532cafbf9ebe6603e3cb00e2558f21b7a5bdd739a
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.11.0-3+deb9u2.debian.tar.xz' apparmor_2.11.0-3+deb9u2.debian.tar.xz 82784 SHA256:d44188c2716a40976d1eecc50ca8a2203133ef54def2f3f74e9564bd4d2ddcce
```

Other potentially useful URLs:

- https://sources.debian.net/src/apparmor/2.11.0-3+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/apparmor/2.11.0-3+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apparmor/2.11.0-3+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr-util=1.5.4-3`

Binary Packages:

- `libaprutil1:amd64=1.5.4-3`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.5.4-3
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.5.4-3.dsc' apr-util_1.5.4-3.dsc 2646 SHA256:352bbbdf8d4e18014614d5a92da11b599cd04bb30ee03d9f04f26a75626371c7
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.5.4.orig.tar.bz2' apr-util_1.5.4.orig.tar.bz2 694427 SHA256:a6cf327189ca0df2fb9d5633d7326c460fe2b61684745fd7963e79a6dd0dc82e
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.5.4-3.debian.tar.xz' apr-util_1.5.4-3.debian.tar.xz 212220 SHA256:c5e7bfcdafb16104e324ddb6825b94577a57a5b77b809dc0330e38ecab030efa
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr-util/1.5.4-3/ (for browsing the source)
- https://sources.debian.net/src/apr-util/1.5.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr-util/1.5.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr=1.5.2-5`

Binary Packages:

- `libapr1:amd64=1.5.2-5`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.5.2-5
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.2-5.dsc' apr_1.5.2-5.dsc 2115 SHA256:b58bb3209c8a28bff47666de6a9bf32292303fdc2433c9fafb15f2a9e6c16ca6
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.2.orig.tar.bz2' apr_1.5.2.orig.tar.bz2 826885 SHA256:7d03ed29c22a7152be45b8e50431063736df9e1daa1ddf93f6a547ba7a28f67a
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.5.2-5.debian.tar.xz' apr_1.5.2-5.debian.tar.xz 212856 SHA256:5b253cd3acc284241c3cb4a84d9d16f9c5c7775c8f7a26b3a0068ff174bacf76
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.5.2-5/ (for browsing the source)
- https://sources.debian.net/src/apr/1.5.2-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.5.2-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=1.4.9`

Binary Packages:

- `apt=1.4.9`
- `libapt-pkg5.0:amd64=1.4.9`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.4.9
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.4.9.dsc' apt_1.4.9.dsc 2549 SHA256:986d98b00caac809341f65acb3d14321d645ce8e87e411c26c66bf149a10dfea
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.4.9.tar.xz' apt_1.4.9.tar.xz 2079572 SHA256:d4d65e7c84da86f3e6dcc933bba46a08db429c9d933b667c864f5c0e880bac0d
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/1.4.9/ (for browsing the source)
- https://sources.debian.net/src/apt/1.4.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/1.4.9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `at-spi2-atk=2.22.0-2`

Binary Packages:

- `libatk-bridge2.0-0:amd64=2.22.0-2`

Licenses: (parsed from: `/usr/share/doc/libatk-bridge2.0-0/copyright`)

- `GPL-2`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris at-spi2-atk=2.22.0-2
'http://deb.debian.org/debian/pool/main/a/at-spi2-atk/at-spi2-atk_2.22.0-2.dsc' at-spi2-atk_2.22.0-2.dsc 2578 SHA256:abbf67124fa754cf8b82fec45e331498987b64822233f08efd26392d3430b4c5
'http://deb.debian.org/debian/pool/main/a/at-spi2-atk/at-spi2-atk_2.22.0.orig.tar.xz' at-spi2-atk_2.22.0.orig.tar.xz 306148 SHA256:e8bdedbeb873eb229eb08c88e11d07713ec25ae175251648ad1a9da6c21113c1
'http://deb.debian.org/debian/pool/main/a/at-spi2-atk/at-spi2-atk_2.22.0-2.debian.tar.xz' at-spi2-atk_2.22.0-2.debian.tar.xz 10012 SHA256:b9e994d7e1521b99858279b8442e8669ccc45d515abc8713fd7e28500c16ed62
```

Other potentially useful URLs:

- https://sources.debian.net/src/at-spi2-atk/2.22.0-2/ (for browsing the source)
- https://sources.debian.net/src/at-spi2-atk/2.22.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/at-spi2-atk/2.22.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `at-spi2-core=2.22.0-6+deb9u1`

Binary Packages:

- `libatspi2.0-0:amd64=2.22.0-6+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libatspi2.0-0/copyright`)

- `GPL-2`
- `LGPL-2`
- `LGPL-2+`
- `Public domain`

Source:

```console
$ apt-get source -qq --print-uris at-spi2-core=2.22.0-6+deb9u1
'http://deb.debian.org/debian/pool/main/a/at-spi2-core/at-spi2-core_2.22.0-6+deb9u1.dsc' at-spi2-core_2.22.0-6+deb9u1.dsc 2585 SHA256:7b1c5acdd88ec61ceab7a7ee3c76a868d5376c73d85f841d8347577a75b396e8
'http://deb.debian.org/debian/pool/main/a/at-spi2-core/at-spi2-core_2.22.0.orig.tar.xz' at-spi2-core_2.22.0.orig.tar.xz 449364 SHA256:415ea3af21318308798e098be8b3a17b2f0cf2fe16cecde5ad840cf4e0f2c80a
'http://deb.debian.org/debian/pool/main/a/at-spi2-core/at-spi2-core_2.22.0-6+deb9u1.debian.tar.xz' at-spi2-core_2.22.0-6+deb9u1.debian.tar.xz 9984 SHA256:1b765499d343a36d626d3c3828b9f1a39efca124b3e4bab8dc3f2a878eeee5fd
```

Other potentially useful URLs:

- https://sources.debian.net/src/at-spi2-core/2.22.0-6+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/at-spi2-core/2.22.0-6+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/at-spi2-core/2.22.0-6+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `atk1.0=2.22.0-1`

Binary Packages:

- `libatk1.0-0:amd64=2.22.0-1`
- `libatk1.0-data=2.22.0-1`

Licenses: (parsed from: `/usr/share/doc/libatk1.0-0/copyright`, `/usr/share/doc/libatk1.0-data/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris atk1.0=2.22.0-1
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.22.0-1.dsc' atk1.0_2.22.0-1.dsc 2725 SHA256:4d316bd64cbe9775c515b56ef233d5d88d2c4aad4376703aba7d5b1cd261cd5f
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.22.0.orig.tar.xz' atk1.0_2.22.0.orig.tar.xz 745572 SHA256:d349f5ca4974c9c76a4963e5b254720523b0c78672cbc0e1a3475dbd9b3d44b6
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.22.0-1.debian.tar.xz' atk1.0_2.22.0-1.debian.tar.xz 10580 SHA256:b72e1dd99b186105ca9a7af36af53d5bf1d4c0e90cd7176a79b8f81a21f73818
```

Other potentially useful URLs:

- https://sources.debian.net/src/atk1.0/2.22.0-1/ (for browsing the source)
- https://sources.debian.net/src/atk1.0/2.22.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/atk1.0/2.22.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `avahi=0.6.32-2`

Binary Packages:

- `libavahi-client3:amd64=0.6.32-2`
- `libavahi-common-data:amd64=0.6.32-2`
- `libavahi-common3:amd64=0.6.32-2`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.6.32-2
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.32-2.dsc' avahi_0.6.32-2.dsc 4263 SHA256:d369e30da54617a519796af49dcb4daa7e12f85314a4653c6504ec5567aab502
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.32.orig.tar.gz' avahi_0.6.32.orig.tar.gz 1297169 SHA256:d54991185d514a0aba54ebeb408d7575b60f5818a772e28fa0e18b98bc1db454
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.6.32-2.debian.tar.xz' avahi_0.6.32-2.debian.tar.xz 29348 SHA256:59434a4796ebc34f4b0fa92e8ca57b4c6c54adc1d2167db0dae3445aeac3318a
```

Other potentially useful URLs:

- https://sources.debian.net/src/avahi/0.6.32-2/ (for browsing the source)
- https://sources.debian.net/src/avahi/0.6.32-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/avahi/0.6.32-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=9.9+deb9u11`

Binary Packages:

- `base-files=9.9+deb9u11`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=9.9+deb9u11
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_9.9+deb9u11.dsc' base-files_9.9+deb9u11.dsc 1444 SHA256:3dea64df32bddd8e55c22a1a5cf5acbf42fcdf73446db0eb735e7536ad4dc57a
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_9.9+deb9u11.tar.xz' base-files_9.9+deb9u11.tar.xz 63196 SHA256:7892391146fb734d79090ef382c285b37bcf12e310c9c3c61ed903aa56a9aa52
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/9.9+deb9u11/ (for browsing the source)
- https://sources.debian.net/src/base-files/9.9+deb9u11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/9.9+deb9u11/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `boost1.62=1.62.0+dfsg-4`

Binary Packages:

- `libboost-date-time1.62.0:amd64=1.62.0+dfsg-4`
- `libboost-filesystem1.62.0:amd64=1.62.0+dfsg-4`
- `libboost-iostreams1.62.0:amd64=1.62.0+dfsg-4`
- `libboost-system1.62.0:amd64=1.62.0+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libboost-date-time1.62.0/copyright`, `/usr/share/doc/libboost-filesystem1.62.0/copyright`, `/usr/share/doc/libboost-iostreams1.62.0/copyright`, `/usr/share/doc/libboost-system1.62.0/copyright`)

- `Boost`
- `bjam`
- `boostbook`

Source:

```console
$ apt-get source -qq --print-uris boost1.62=1.62.0+dfsg-4
'http://deb.debian.org/debian/pool/main/b/boost1.62/boost1.62_1.62.0+dfsg-4.dsc' boost1.62_1.62.0+dfsg-4.dsc 7244 SHA256:fb3ff976a0a52a693eb0ec0d3f0a33919ed6280a0a573f5d542f53b67b8dd9fc
'http://deb.debian.org/debian/pool/main/b/boost1.62/boost1.62_1.62.0+dfsg.orig.tar.bz2' boost1.62_1.62.0+dfsg.orig.tar.bz2 83837238 SHA256:203e8f9670988d57b277e4205a19336b4fba39497159ec5252ffa1e9b6158d03
'http://deb.debian.org/debian/pool/main/b/boost1.62/boost1.62_1.62.0+dfsg-4.debian.tar.xz' boost1.62_1.62.0+dfsg-4.debian.tar.xz 106484 SHA256:3eaf28f6e211bcbce50580a4a59cb52aaa0185530b2ce9fc4c6447945b661ae1
```

Other potentially useful URLs:

- https://sources.debian.net/src/boost1.62/1.62.0+dfsg-4/ (for browsing the source)
- https://sources.debian.net/src/boost1.62/1.62.0+dfsg-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/boost1.62/1.62.0+dfsg-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.6-8.1`

Binary Packages:

- `bzip2=1.0.6-8.1`
- `libbz2-1.0:amd64=1.0.6-8.1`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

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

### `dpkg` source package: `bzr=2.7.0+bzr6619-7+deb9u1`

Binary Packages:

- `bzr=2.7.0+bzr6619-7+deb9u1`
- `python-bzrlib=2.7.0+bzr6619-7+deb9u1`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`, `/usr/share/doc/python-bzrlib/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.7.0+bzr6619-7+deb9u1
'http://deb.debian.org/debian/pool/main/b/bzr/bzr_2.7.0+bzr6619-7+deb9u1.dsc' bzr_2.7.0+bzr6619-7+deb9u1.dsc 3033 SHA256:b13644e5d249743102646f3d01ae66b9ddb6d1911f3ee2d6fe0e5ac8b9bd6273
'http://deb.debian.org/debian/pool/main/b/bzr/bzr_2.7.0+bzr6619.orig.tar.gz' bzr_2.7.0+bzr6619.orig.tar.gz 10945598 SHA256:a0192999245457fbd564702518bc96453ac0f9b38ea031a466679839b346fa14
'http://deb.debian.org/debian/pool/main/b/bzr/bzr_2.7.0+bzr6619-7+deb9u1.debian.tar.xz' bzr_2.7.0+bzr6619-7+deb9u1.debian.tar.xz 92072 SHA256:c59743abd33483852c1fdc0647a96599e8b7adccde266b32fc78f639e369584d
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzr/2.7.0+bzr6619-7+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/bzr/2.7.0+bzr6619-7+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzr/2.7.0+bzr6619-7+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ca-certificates=20161130+nmu1+deb9u1`

Binary Packages:

- `ca-certificates=20161130+nmu1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20161130+nmu1+deb9u1
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20161130+nmu1+deb9u1.dsc' ca-certificates_20161130+nmu1+deb9u1.dsc 1900 SHA256:c2f23c84c06abb9e982fa54ea6b061369711824d472039e89aa3fe46d2f37715
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20161130+nmu1+deb9u1.tar.xz' ca-certificates_20161130+nmu1+deb9u1.tar.xz 247788 SHA256:3b9b56e55a92acdabdae700340f36c5243105c2a022993407632bb08bb4c0197
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20161130+nmu1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20161130+nmu1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20161130+nmu1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cairo=1.14.8-1`

Binary Packages:

- `libcairo-gobject2:amd64=1.14.8-1`
- `libcairo2:amd64=1.14.8-1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.14.8-1
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.8-1.dsc' cairo_1.14.8-1.dsc 2879 SHA256:a24470ae5240afe8693d07bb5a0972e966c2ef27f12b95ffbd7882900afd405c
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.8.orig.tar.xz' cairo_1.14.8.orig.tar.xz 35392464 SHA256:d1f2d98ae9a4111564f6de4e013d639cf77155baf2556582295a0f00a9bc5e20
'http://deb.debian.org/debian/pool/main/c/cairo/cairo_1.14.8-1.debian.tar.xz' cairo_1.14.8-1.debian.tar.xz 28880 SHA256:7b7079075c15615b3e476235ebab30b8845a7ad8886fe3e87fe1d4c9c2b9bebc
```

Other potentially useful URLs:

- https://sources.debian.net/src/cairo/1.14.8-1/ (for browsing the source)
- https://sources.debian.net/src/cairo/1.14.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cairo/1.14.8-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `cgmanager=0.41-2`

Binary Packages:

- `cgmanager=0.41-2`
- `libcgmanager0:amd64=0.41-2`

Licenses: (parsed from: `/usr/share/doc/cgmanager/copyright`, `/usr/share/doc/libcgmanager0/copyright`)

- `GPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris cgmanager=0.41-2
'http://deb.debian.org/debian/pool/main/c/cgmanager/cgmanager_0.41-2.dsc' cgmanager_0.41-2.dsc 2232 SHA256:5f82cf2287e65d42fb755315356b7ce70d6a88954b46199fb8c8bc612a7086bb
'http://deb.debian.org/debian/pool/main/c/cgmanager/cgmanager_0.41.orig.tar.gz' cgmanager_0.41.orig.tar.gz 461805 SHA256:29b155befb3ac233d5d29dbca7c791c8138bab01bfa78ea4757ebb88ce23b458
'http://deb.debian.org/debian/pool/main/c/cgmanager/cgmanager_0.41-2.debian.tar.xz' cgmanager_0.41-2.debian.tar.xz 11920 SHA256:09de69dbb15a1d1abeb5caa3f1c180ae9dea75318a984b03a80965155b6154dc
```

Other potentially useful URLs:

- https://sources.debian.net/src/cgmanager/0.41-2/ (for browsing the source)
- https://sources.debian.net/src/cgmanager/0.41-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cgmanager/0.41-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `chromaprint=1.4.2-1`

Binary Packages:

- `libchromaprint1:amd64=1.4.2-1`

Licenses: (parsed from: `/usr/share/doc/libchromaprint1/copyright`)

- `BSD-3-clause`
- `Expat`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris chromaprint=1.4.2-1
'http://deb.debian.org/debian/pool/main/c/chromaprint/chromaprint_1.4.2-1.dsc' chromaprint_1.4.2-1.dsc 2253 SHA256:344cfac1fbf1d19ad7918b05f6dbe6f07710e978f0f25f9815cc26b54f1b21b6
'http://deb.debian.org/debian/pool/main/c/chromaprint/chromaprint_1.4.2.orig.tar.gz' chromaprint_1.4.2.orig.tar.gz 613367 SHA256:989609a7e841dd75b34ee793bd1d049ce99a8f0d444b3cea39d57c3e5d26b4d4
'http://deb.debian.org/debian/pool/main/c/chromaprint/chromaprint_1.4.2-1.debian.tar.xz' chromaprint_1.4.2-1.debian.tar.xz 5492 SHA256:ab3a91076783cb6255fe68eb418be907fa8a19c6647a3bae1cb216ff21f72765
```

Other potentially useful URLs:

- https://sources.debian.net/src/chromaprint/1.4.2-1/ (for browsing the source)
- https://sources.debian.net/src/chromaprint/1.4.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/chromaprint/1.4.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `clp=1.15.10-3`

Binary Packages:

- `coinor-libclp1=1.15.10-3+b1`

Licenses: (parsed from: `/usr/share/doc/coinor-libclp1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris clp=1.15.10-3
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.15.10-3.dsc' clp_1.15.10-3.dsc 2345 SHA256:4703689e318bedb4ee6318f75f9c39d1fc8e5711ec3fa74e0f8db4a50d9d0aec
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.15.10.orig.tar.gz' clp_1.15.10.orig.tar.gz 1856909 SHA256:44b6f7e05ac64a9eed63eb67b8175a3a7d054ae1928156a5cc1dce5ee044706c
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.15.10-3.debian.tar.xz' clp_1.15.10-3.debian.tar.xz 9644 SHA256:5057729dbe99be7fba95cf44e8145f8c1256de973700299868f4def44f5d7346
```

Other potentially useful URLs:

- https://sources.debian.net/src/clp/1.15.10-3/ (for browsing the source)
- https://sources.debian.net/src/clp/1.15.10-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/clp/1.15.10-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `clucene-core=2.3.3.4+dfsg-1`

Binary Packages:

- `libclucene-contribs1v5:amd64=2.3.3.4+dfsg-1`
- `libclucene-core1v5:amd64=2.3.3.4+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libclucene-contribs1v5/copyright`, `/usr/share/doc/libclucene-core1v5/copyright`)

- `Apache-2.0`
- `LGPL-2.1`
- `Reuters-21578 - Distribution 1.0`

Source:

```console
$ apt-get source -qq --print-uris clucene-core=2.3.3.4+dfsg-1
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4+dfsg-1.dsc' clucene-core_2.3.3.4+dfsg-1.dsc 2019 SHA256:5158409a1b0c6913f82e5e0562ace6f3ff0cab197cf72b86e039b9fb9a73e1ed
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4+dfsg.orig.tar.xz' clucene-core_2.3.3.4+dfsg.orig.tar.xz 826688 SHA256:c70b8202c0afca27f9fa2f1a5d09a41bc4cc57a8f68c854379891ea2e24f1490
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4+dfsg-1.debian.tar.xz' clucene-core_2.3.3.4+dfsg-1.debian.tar.xz 8736 SHA256:a7d25d096e70105464a911e908fee7e5eb25adf3682ae75b1b514d6a5846b076
```

Other potentially useful URLs:

- https://sources.debian.net/src/clucene-core/2.3.3.4+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/clucene-core/2.3.3.4+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/clucene-core/2.3.3.4+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinmp=1.7.6+dfsg1-2`

Binary Packages:

- `coinor-libcoinmp1v5:amd64=1.7.6+dfsg1-2`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinmp1v5/copyright`)

- `CPL-1`
- `EPL-1`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris coinmp=1.7.6+dfsg1-2
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.7.6+dfsg1-2.dsc' coinmp_1.7.6+dfsg1-2.dsc 2027 SHA256:c3ea83d7ba4d080e89792075cec7efe3f378a1e2ae2adafaa43f4e57ab968cc2
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.7.6+dfsg1.orig.tar.gz' coinmp_1.7.6+dfsg1.orig.tar.gz 659163 SHA256:859ed08310ec47da0b57dceb9ca60e9db8f53ea0e0e76b7cffa41cbaf569caa2
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.7.6+dfsg1-2.debian.tar.xz' coinmp_1.7.6+dfsg1-2.debian.tar.xz 7732 SHA256:58f9e86014cc0948061038dcfcab774a9d9f5f54ece157c0e49fcf545f153c00
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinmp/1.7.6+dfsg1-2/ (for browsing the source)
- https://sources.debian.net/src/coinmp/1.7.6+dfsg1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinmp/1.7.6+dfsg1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-cbc=2.8.12-1`

Binary Packages:

- `coinor-libcbc3=2.8.12-1+b2`

Licenses: (parsed from: `/usr/share/doc/coinor-libcbc3/copyright`)

- `EPL-1`
- `GPL-3`
- `LUCENT`

Source:

```console
$ apt-get source -qq --print-uris coinor-cbc=2.8.12-1
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.8.12-1.dsc' coinor-cbc_2.8.12-1.dsc 2438 SHA256:226034354ccd2faa4d74a8d32bf54fa7ebb806b328e2e04f991ec042f092c4ff
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.8.12.orig.tar.gz' coinor-cbc_2.8.12.orig.tar.gz 1344877 SHA256:50618a41d23022cdf5be4306b4a3cb75157c33876fdcaca26955ef7349bdbc7f
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.8.12-1.debian.tar.xz' coinor-cbc_2.8.12-1.debian.tar.xz 10616 SHA256:5c805bf73e9029750b1fa077013a0db5ee646cd2d83d3f364491973c50e98a30
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-cbc/2.8.12-1/ (for browsing the source)
- https://sources.debian.net/src/coinor-cbc/2.8.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-cbc/2.8.12-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-cgl=0.58.9-1`

Binary Packages:

- `coinor-libcgl1=0.58.9-1+b1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcgl1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-cgl=0.58.9-1
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.58.9-1.dsc' coinor-cgl_0.58.9-1.dsc 2289 SHA256:cfb321193be4a6450c811c088f770bb8437d907e470ccc6eaa91777370ee7c38
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.58.9.orig.tar.gz' coinor-cgl_0.58.9.orig.tar.gz 982607 SHA256:d23d621f9f80bb3753536f1fa34008ed56202bc01ef99e72e4c4241b18c269fc
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.58.9-1.debian.tar.xz' coinor-cgl_0.58.9-1.debian.tar.xz 7504 SHA256:b24e2d67aec8a23e23dc3c0648a8cdd06625a3f8f1d9bb330b39651036f20dda
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-cgl/0.58.9-1/ (for browsing the source)
- https://sources.debian.net/src/coinor-cgl/0.58.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-cgl/0.58.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-osi=0.106.9-2`

Binary Packages:

- `coinor-libosi1v5=0.106.9-2+b1`

Licenses: (parsed from: `/usr/share/doc/coinor-libosi1v5/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-osi=0.106.9-2
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.106.9-2.dsc' coinor-osi_0.106.9-2.dsc 2290 SHA256:b00141057ffae4fe2ca78c5f1e51538ecdc298891fc750a3f1ca7e7cc135a02e
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.106.9.orig.tar.gz' coinor-osi_0.106.9.orig.tar.gz 751902 SHA256:3e7db33360a63d1315d3b0f64fe0031ff96c8bbc7af9fc5faf036a4fcf7fe68e
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.106.9-2.debian.tar.xz' coinor-osi_0.106.9-2.debian.tar.xz 7720 SHA256:0a8acd061066a35a0e551cc6a41eb1c6b1388c689fba7159e1287492e303013d
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-osi/0.106.9-2/ (for browsing the source)
- https://sources.debian.net/src/coinor-osi/0.106.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-osi/0.106.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinutils=2.9.15-4`

Binary Packages:

- `coinor-libcoinutils3v5=2.9.15-4`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinutils3v5/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinutils=2.9.15-4
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.9.15-4.dsc' coinutils_2.9.15-4.dsc 2257 SHA256:5e88953148004142ea3489d01489007c47e3746afd9e6449fab369d5b64f6054
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.9.15.orig.tar.gz' coinutils_2.9.15.orig.tar.gz 1742562 SHA256:db1a0504f3334929462b7ee72a6c6f6c2ad23331716f829c5be8899193bf414d
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.9.15-4.debian.tar.xz' coinutils_2.9.15-4.debian.tar.xz 8520 SHA256:656822ecd982850818f6c0735b7dfe4aaf5e4d355ffa541d233412264ad1aff1
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinutils/2.9.15-4/ (for browsing the source)
- https://sources.debian.net/src/coinutils/2.9.15-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinutils/2.9.15-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `colord=1.3.3-2`

Binary Packages:

- `libcolord2:amd64=1.3.3-2`

Licenses: (parsed from: `/usr/share/doc/libcolord2/copyright`)

- `CC0`
- `GFDL-NIV`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris colord=1.3.3-2
'http://deb.debian.org/debian/pool/main/c/colord/colord_1.3.3-2.dsc' colord_1.3.3-2.dsc 2960 SHA256:fa10c1ab6cff57871be9bd4a6b1cc2577477a6297d3092286deb20bf2c7a9031
'http://deb.debian.org/debian/pool/main/c/colord/colord_1.3.3.orig.tar.xz' colord_1.3.3.orig.tar.xz 1240104 SHA256:d1848e797106a036b0d6ebed99a789a6ae07d60f1d9cc59be5b257efe7ec31a4
'http://deb.debian.org/debian/pool/main/c/colord/colord_1.3.3-2.debian.tar.xz' colord_1.3.3-2.debian.tar.xz 26800 SHA256:41b902be527e153484d8412a0df729c358c49c9ac2c7e9281849d2473e0dd403
```

Other potentially useful URLs:

- https://sources.debian.net/src/colord/1.3.3-2/ (for browsing the source)
- https://sources.debian.net/src/colord/1.3.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/colord/1.3.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `configobj=5.0.6-2`

Binary Packages:

- `python-configobj=5.0.6-2`

Licenses: (parsed from: `/usr/share/doc/python-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-2
'http://deb.debian.org/debian/pool/main/c/configobj/configobj_5.0.6-2.dsc' configobj_5.0.6-2.dsc 2381 SHA256:9bb8577128460ff33326d3d90b8454376c83f4d41b1da61aeabdbfcbfb5e0087
'http://deb.debian.org/debian/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA256:2e140354efcca6f558ff9ee941b435ae09a617bc071797bef62c8d6ed2033d5e
'http://deb.debian.org/debian/pool/main/c/configobj/configobj_5.0.6-2.debian.tar.xz' configobj_5.0.6-2.debian.tar.xz 7436 SHA256:dc677cd329b4a3aacebe10c5a169d9d092cc27888c3f3f9203930cacd6a0eab8
```

Other potentially useful URLs:

- https://sources.debian.net/src/configobj/5.0.6-2/ (for browsing the source)
- https://sources.debian.net/src/configobj/5.0.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/configobj/5.0.6-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `cryptsetup=2:1.7.3-4`

Binary Packages:

- `libcryptsetup4:amd64=2:1.7.3-4`

Licenses: (parsed from: `/usr/share/doc/libcryptsetup4/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris cryptsetup=2:1.7.3-4
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.7.3-4.dsc' cryptsetup_1.7.3-4.dsc 2708 SHA256:7e7bb358041f5e9f84a73c297acf92e90d40c9e2a88cf14278fd7c696c5e40b2
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.7.3.orig.tar.gz' cryptsetup_1.7.3.orig.tar.gz 1102318 SHA256:58921825d268701af151e4de034f508aa8cb4d9f2e1c11847f4f8ae82866043d
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_1.7.3-4.debian.tar.xz' cryptsetup_1.7.3-4.debian.tar.xz 93956 SHA256:2820ec19ebbc21ac5703c56382c02abb4511683f733766a2de85b2c80cfc0596
```

Other potentially useful URLs:

- https://sources.debian.net/src/cryptsetup/2:1.7.3-4/ (for browsing the source)
- https://sources.debian.net/src/cryptsetup/2:1.7.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cryptsetup/2:1.7.3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `crystalhd=1:0.0~git20110715.fdd2f19-12`

Binary Packages:

- `libcrystalhd3:amd64=1:0.0~git20110715.fdd2f19-12`

Licenses: (parsed from: `/usr/share/doc/libcrystalhd3/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris crystalhd=1:0.0~git20110715.fdd2f19-12
'http://deb.debian.org/debian/pool/main/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-12.dsc' crystalhd_0.0~git20110715.fdd2f19-12.dsc 2356 SHA256:24d2413fe865d91f54366f906f04ebaa8cb9a2c28b3359a83f3754581474f621
'http://deb.debian.org/debian/pool/main/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz' crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz 1186072 SHA256:a1c22908b85085dcc4591bc033fe054be63eab59b7d35f0a9ab3fcb2600722b7
'http://deb.debian.org/debian/pool/main/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-12.debian.tar.xz' crystalhd_0.0~git20110715.fdd2f19-12.debian.tar.xz 15260 SHA256:b634af1ff394c6e44445e29e7e6b27648d35f58e475ed1749eeaf3dc80ca15a1
```

Other potentially useful URLs:

- https://sources.debian.net/src/crystalhd/1:0.0~git20110715.fdd2f19-12/ (for browsing the source)
- https://sources.debian.net/src/crystalhd/1:0.0~git20110715.fdd2f19-12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/crystalhd/1:0.0~git20110715.fdd2f19-12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cups=2.2.1-8+deb9u4`

Binary Packages:

- `libcups2:amd64=2.2.1-8+deb9u4`
- `libcupsimage2:amd64=2.2.1-8+deb9u4`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`, `/usr/share/doc/libcupsimage2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.2.1-8+deb9u4
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.1-8+deb9u4.dsc' cups_2.2.1-8+deb9u4.dsc 3424 SHA256:9770e8589f9c5270f902e5449ffc4d66626bb5694c027b5c1f2a26be6b4a3962
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.1.orig.tar.gz' cups_2.2.1.orig.tar.gz 9486635 SHA256:83b8730aa977cc055e7410df6a3a682548994c113994ca630a16513017e419d5
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.1.orig.tar.gz.asc' cups_2.2.1.orig.tar.gz.asc 797 SHA256:37c2e6215b2794c33864e543bc0caf6aefa724844e41b4c9659c87f28d125c2a
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.1-8+deb9u4.debian.tar.xz' cups_2.2.1-8+deb9u4.debian.tar.xz 367156 SHA256:f559e1674deab2abd95c3d688c3812cdd93ad79d2277d55769e44d2cdbafc08e
```

Other potentially useful URLs:

- https://sources.debian.net/src/cups/2.2.1-8+deb9u4/ (for browsing the source)
- https://sources.debian.net/src/cups/2.2.1-8+deb9u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cups/2.2.1-8+deb9u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.52.1-5+deb9u9`

Binary Packages:

- `curl=7.52.1-5+deb9u9`
- `libcurl3:amd64=7.52.1-5+deb9u9`
- `libcurl3-gnutls:amd64=7.52.1-5+deb9u9`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.52.1-5+deb9u9
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.52.1-5+deb9u9.dsc' curl_7.52.1-5+deb9u9.dsc 2818 SHA256:21182689e9ce9d67fff055d61a1c425afa3b7451481bb786382a0d9f171db1d8
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.52.1.orig.tar.gz' curl_7.52.1.orig.tar.gz 3504621 SHA256:a8984e8b20880b621f61a62d95ff3c0763a3152093a9f9ce4287cfd614add6ae
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.52.1-5+deb9u9.debian.tar.xz' curl_7.52.1-5+deb9u9.debian.tar.xz 42388 SHA256:5b0da2572739b3614cac1b266042e05d842aba3c3225949158ddb51e86eb31d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.52.1-5+deb9u9/ (for browsing the source)
- https://sources.debian.net/src/curl/7.52.1-5+deb9u9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.52.1-5+deb9u9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27~101-g0780600+dfsg-3+deb9u1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27~101-g0780600+dfsg-3+deb9u1`
- `libsasl2-modules-db:amd64=2.1.27~101-g0780600+dfsg-3+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27~101-g0780600+dfsg-3+deb9u1
'http://security.debian.org/debian-security/pool/updates/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.dsc' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.dsc 3381 SHA256:a331441098ece65be5bf13d871b486115af68daf06a0145adf6cda8ef71d73e4
'http://security.debian.org/debian-security/pool/updates/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz 1143888 SHA256:69f34971f768e7ee6a6b647ec2d16a5a72a854ecd4602b019d5f79ba61063fdc
'http://security.debian.org/debian-security/pool/updates/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.debian.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.debian.tar.xz 94992 SHA256:be1ba4b3bfcc4740354342686deac73ca2e46c4871219599229efe8cfe98df6f
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `d-conf=0.26.0-2`

Binary Packages:

- `dconf-gsettings-backend:amd64=0.26.0-2+b1`
- `dconf-service=0.26.0-2+b1`
- `libdconf1:amd64=0.26.0-2+b1`

Licenses: (parsed from: `/usr/share/doc/dconf-gsettings-backend/copyright`, `/usr/share/doc/dconf-service/copyright`, `/usr/share/doc/libdconf1/copyright`)

- `GPL-3`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris d-conf=0.26.0-2
'http://deb.debian.org/debian/pool/main/d/d-conf/d-conf_0.26.0-2.dsc' d-conf_0.26.0-2.dsc 2630 SHA256:c6c9b1879673ee1cf5edbffa3bb9def982ed90dc111a3dc24c5585bf72cbf409
'http://deb.debian.org/debian/pool/main/d/d-conf/d-conf_0.26.0.orig.tar.xz' d-conf_0.26.0.orig.tar.xz 219688 SHA256:8683292eb31a3fae31e561f0a4220d8569b0f6d882e9958b68373f9043d658c9
'http://deb.debian.org/debian/pool/main/d/d-conf/d-conf_0.26.0-2.debian.tar.xz' d-conf_0.26.0-2.debian.tar.xz 8792 SHA256:54b1fc27d417ef7528408296552297ae6988dbe12404e04143dbbf040caf6bbc
```

Other potentially useful URLs:

- https://sources.debian.net/src/d-conf/0.26.0-2/ (for browsing the source)
- https://sources.debian.net/src/d-conf/0.26.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/d-conf/0.26.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `dbus-glib=0.108-2`

Binary Packages:

- `libdbus-glib-1-2:amd64=0.108-2`

Licenses: (parsed from: `/usr/share/doc/libdbus-glib-1-2/copyright`)

- `AFL-2.1`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dbus-glib=0.108-2
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.108-2.dsc' dbus-glib_0.108-2.dsc 2332 SHA256:19ca2b01722ce34feb4673d6df79067a698e4855bc5f0850f5f6e1002a9fd6b0
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.108.orig.tar.gz' dbus-glib_0.108.orig.tar.gz 812488 SHA256:9f340c7e2352e9cdf113893ca77ca9075d9f8d5e81476bf2bf361099383c602c
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.108-2.debian.tar.xz' dbus-glib_0.108-2.debian.tar.xz 19124 SHA256:6d7dc13f5c7333836d021aa3545f7cfccea83be1d5c8bf7dc761fab378aff5a9
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus-glib/0.108-2/ (for browsing the source)
- https://sources.debian.net/src/dbus-glib/0.108-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus-glib/0.108-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dbus=1.10.28-0+deb9u1`

Binary Packages:

- `dbus=1.10.28-0+deb9u1`
- `dbus-user-session=1.10.28-0+deb9u1`
- `libdbus-1-3:amd64=1.10.28-0+deb9u1`

Licenses: (parsed from: `/usr/share/doc/dbus/copyright`, `/usr/share/doc/dbus-user-session/copyright`, `/usr/share/doc/libdbus-1-3/copyright`)

- `AFL-2.1`
- `AFL-2.1,`
- `BSD-3-clause`
- `BSD-3-clause-generic`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `Tcl-BSDish`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris dbus=1.10.28-0+deb9u1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.10.28-0+deb9u1.dsc' dbus_1.10.28-0+deb9u1.dsc 3345 SHA256:a4758356f5a71e87804f3b55e1f83f41c10b19ddb84595e322eeb2cd44cdb367
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.10.28.orig.tar.gz' dbus_1.10.28.orig.tar.gz 1998830 SHA256:63f5b1d57360be5c147ef561e67f8efdd9034e1f12b7aba41feb42b376324552
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.10.28.orig.tar.gz.asc' dbus_1.10.28.orig.tar.gz.asc 833 SHA256:5da985dafdf223b7f5e0c6e51c608fd7d87e681e0c1eccfa2970be2978c0bed9
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.10.28-0+deb9u1.debian.tar.xz' dbus_1.10.28-0+deb9u1.debian.tar.xz 57500 SHA256:83c883431ee58fbfd7dcae4c763baa904e14b835023edff0dd495270d56d59b3
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus/1.10.28-0+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/dbus/1.10.28-0+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus/1.10.28-0+deb9u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `desktop-file-utils=0.23-1`

Binary Packages:

- `desktop-file-utils=0.23-1`

Licenses: (parsed from: `/usr/share/doc/desktop-file-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris desktop-file-utils=0.23-1
'http://deb.debian.org/debian/pool/main/d/desktop-file-utils/desktop-file-utils_0.23-1.dsc' desktop-file-utils_0.23-1.dsc 2119 SHA256:f022e4b8dde3acf46b9491f6c9ee6ab22e757c3115e87399516e64bec97e21c1
'http://deb.debian.org/debian/pool/main/d/desktop-file-utils/desktop-file-utils_0.23.orig.tar.xz' desktop-file-utils_0.23.orig.tar.xz 132000 SHA256:6c094031bdec46c9f621708f919084e1cb5294e2c5b1e4c883b3e70cb8903385
'http://deb.debian.org/debian/pool/main/d/desktop-file-utils/desktop-file-utils_0.23-1.debian.tar.xz' desktop-file-utils_0.23-1.debian.tar.xz 4972 SHA256:1b6fa9b4e947860daf18ede1604db95cfd9e5aefc411f7b262de70927a7f5e10
```

Other potentially useful URLs:

- https://sources.debian.net/src/desktop-file-utils/0.23-1/ (for browsing the source)
- https://sources.debian.net/src/desktop-file-utils/0.23-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/desktop-file-utils/0.23-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dh-python=2.20170125`

Binary Packages:

- `dh-python=2.20170125`

Licenses: (parsed from: `/usr/share/doc/dh-python/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris dh-python=2.20170125
'http://deb.debian.org/debian/pool/main/d/dh-python/dh-python_2.20170125.dsc' dh-python_2.20170125.dsc 1908 SHA256:ef4f2951cea36ae4aac29126a1017505f98b595432fb5bdac0f21b4b4d72c1b4
'http://deb.debian.org/debian/pool/main/d/dh-python/dh-python_2.20170125.tar.xz' dh-python_2.20170125.tar.xz 91332 SHA256:2e09c162ee2442a03511b7ebe83896e1e3c1df79ce97a22d2f8a8b4cfec9f1e3
```

Other potentially useful URLs:

- https://sources.debian.net/src/dh-python/2.20170125/ (for browsing the source)
- https://sources.debian.net/src/dh-python/2.20170125/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dh-python/2.20170125/ (for access to the source package after it no longer exists in the archive)

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

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

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
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.43.4-2+deb9u1.dsc' e2fsprogs_1.43.4-2+deb9u1.dsc 2071 SHA256:b3d4d80f72ef552369448b0f2ecc2b68e3a670fdab5a14705fcaf8607579cc32
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.43.4.orig.tar.gz' e2fsprogs_1.43.4.orig.tar.gz 7552218 SHA256:484ab0bc1bc07c64267b18cfe7871b6b975bf0a705c5a4563001f035071cdc7c
'http://security.debian.org/debian-security/pool/updates/main/e/e2fsprogs/e2fsprogs_1.43.4-2+deb9u1.debian.tar.xz' e2fsprogs_1.43.4-2+deb9u1.debian.tar.xz 78168 SHA256:d238b0872e2aad029fbcd02a9e83242befb3b2cc445bbaa4712a90f2741fbeeb
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.43.4-2+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.43.4-2+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.43.4-2+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `elfutils=0.168-1`

Binary Packages:

- `libelf1:amd64=0.168-1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.168-1
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.168-1.dsc' elfutils_0.168-1.dsc 2549 SHA256:b29e03a3d515d9accd52019ff7c75762ae5e61285453518ff90d538e9878ad7f
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.168.orig.tar.bz2' elfutils_0.168.orig.tar.bz2 6840399 SHA256:b88d07893ba1373c7dd69a7855974706d05377766568a7d9002706d5de72c276
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.168.orig.tar.bz2.asc' elfutils_0.168.orig.tar.bz2.asc 473 SHA256:f455fc014b59a0d80ab921935d20f26e64f411a424d4be29ec5bf3a1378f3002
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.168-1.debian.tar.xz' elfutils_0.168-1.debian.tar.xz 39964 SHA256:5517922b1025d32903759c46f9a1f656e3e367c5ea036dc54b32cbbe68a5f300
```

Other potentially useful URLs:

- https://sources.debian.net/src/elfutils/0.168-1/ (for browsing the source)
- https://sources.debian.net/src/elfutils/0.168-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/elfutils/0.168-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `exiv2=0.25-3.1+deb9u1`

Binary Packages:

- `libexiv2-14:amd64=0.25-3.1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libexiv2-14/copyright`)

- `BSD-3-clause`
- `BSD-4-clause`
- `Expat`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-2+_AutoConfException_LibToolException`
- `GPL-2+_LibToolException`
- `Gettext`
- `LGNU_GPL`
- `MPL-2.0`
- `Permissive`

Source:

```console
$ apt-get source -qq --print-uris exiv2=0.25-3.1+deb9u1
'http://deb.debian.org/debian/pool/main/e/exiv2/exiv2_0.25-3.1+deb9u1.dsc' exiv2_0.25-3.1+deb9u1.dsc 2304 SHA256:2b6c0b81178506feab3c69724a42443200fe5aa91665028a7aa1618e39fab607
'http://deb.debian.org/debian/pool/main/e/exiv2/exiv2_0.25.orig.tar.gz' exiv2_0.25.orig.tar.gz 5434325 SHA256:c80bfc778a15fdb06f71265db2c3d49d8493c382e516cb99b8c9f9cbde36efa4
'http://deb.debian.org/debian/pool/main/e/exiv2/exiv2_0.25-3.1+deb9u1.debian.tar.xz' exiv2_0.25-3.1+deb9u1.debian.tar.xz 26540 SHA256:2a24fa184ae4a38b1d1292c3286f089100b626ae056355de8c5be73ba0e4b0b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/exiv2/0.25-3.1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/exiv2/0.25-3.1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/exiv2/0.25-3.1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.0-2+deb9u3`

Binary Packages:

- `libexpat1:amd64=2.2.0-2+deb9u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.2.0-2+deb9u3
'http://security.debian.org/debian-security/pool/updates/main/e/expat/expat_2.2.0-2+deb9u3.dsc' expat_2.2.0-2+deb9u3.dsc 2450 SHA256:11f83d0c9912cf287b53b72636dc8049656477d05bffd3ecf56c29709bfec33f
'http://security.debian.org/debian-security/pool/updates/main/e/expat/expat_2.2.0.orig.tar.bz2' expat_2.2.0.orig.tar.bz2 414352 SHA256:d9e50ff2d19b3538bd2127902a89987474e1a4db8e43a66a4d1a712ab9a504ff
'http://security.debian.org/debian-security/pool/updates/main/e/expat/expat_2.2.0-2+deb9u3.debian.tar.xz' expat_2.2.0-2+deb9u3.debian.tar.xz 12608 SHA256:68800c47feebefea7318e767d6837b7c84ad875ab53d188e951d4859eddba241
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.0-2+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.0-2+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.0-2+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `explorercanvas=0.r3-4`

Binary Packages:

- `libjs-excanvas=0.r3-4`

Licenses: (parsed from: `/usr/share/doc/libjs-excanvas/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris explorercanvas=0.r3-4
'http://deb.debian.org/debian/pool/main/e/explorercanvas/explorercanvas_0.r3-4.dsc' explorercanvas_0.r3-4.dsc 2000 SHA256:d168011ed1f110f82b5039a6b070167f1f262d2a35d7fa25a6b5462f73761637
'http://deb.debian.org/debian/pool/main/e/explorercanvas/explorercanvas_0.r3.orig.tar.gz' explorercanvas_0.r3.orig.tar.gz 50748 SHA256:687af8084781b8eb3451fc55c88f6dfddc2b84428d197daf2c4c33fd5c55fed8
'http://deb.debian.org/debian/pool/main/e/explorercanvas/explorercanvas_0.r3-4.debian.tar.xz' explorercanvas_0.r3-4.debian.tar.xz 2040 SHA256:afcaa3e229d9b423988fc30439aeee1599c9dac8ad94430309404f9cf9f0c11f
```

Other potentially useful URLs:

- https://sources.debian.net/src/explorercanvas/0.r3-4/ (for browsing the source)
- https://sources.debian.net/src/explorercanvas/0.r3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/explorercanvas/0.r3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ffmpeg2theora=0.30-1`

Binary Packages:

- `ffmpeg2theora=0.30-1+b2`

Licenses: (parsed from: `/usr/share/doc/ffmpeg2theora/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ffmpeg2theora=0.30-1
'http://deb.debian.org/debian/pool/main/f/ffmpeg2theora/ffmpeg2theora_0.30-1.dsc' ffmpeg2theora_0.30-1.dsc 2299 SHA256:d05184357819db6e2741c18edfbad7b40e00580a85df733af6514497ab150863
'http://deb.debian.org/debian/pool/main/f/ffmpeg2theora/ffmpeg2theora_0.30.orig.tar.bz2' ffmpeg2theora_0.30.orig.tar.bz2 91269 SHA256:4f6464b444acab5d778e0a3359d836e0867a3dcec4ad8f1cdcf87cb711ccc6df
'http://deb.debian.org/debian/pool/main/f/ffmpeg2theora/ffmpeg2theora_0.30-1.debian.tar.xz' ffmpeg2theora_0.30-1.debian.tar.xz 3920 SHA256:6becfa2bc2f7efc669a9a72e173c1edb41e8132b67b0e3146069156bdaec7c92
```

Other potentially useful URLs:

- https://sources.debian.net/src/ffmpeg2theora/0.30-1/ (for browsing the source)
- https://sources.debian.net/src/ffmpeg2theora/0.30-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ffmpeg2theora/0.30-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ffmpeg=7:3.2.14-1~deb9u1`

Binary Packages:

- `ffmpeg=7:3.2.14-1~deb9u1`
- `libavcodec57:amd64=7:3.2.14-1~deb9u1`
- `libavdevice57:amd64=7:3.2.14-1~deb9u1`
- `libavfilter6:amd64=7:3.2.14-1~deb9u1`
- `libavformat57:amd64=7:3.2.14-1~deb9u1`
- `libavresample3:amd64=7:3.2.14-1~deb9u1`
- `libavutil55:amd64=7:3.2.14-1~deb9u1`
- `libpostproc54:amd64=7:3.2.14-1~deb9u1`
- `libswresample2:amd64=7:3.2.14-1~deb9u1`
- `libswscale4:amd64=7:3.2.14-1~deb9u1`

Licenses: (parsed from: `/usr/share/doc/ffmpeg/copyright`, `/usr/share/doc/libavcodec57/copyright`, `/usr/share/doc/libavdevice57/copyright`, `/usr/share/doc/libavfilter6/copyright`, `/usr/share/doc/libavformat57/copyright`, `/usr/share/doc/libavresample3/copyright`, `/usr/share/doc/libavutil55/copyright`, `/usr/share/doc/libpostproc54/copyright`, `/usr/share/doc/libswresample2/copyright`, `/usr/share/doc/libswscale4/copyright`)

- `BSD-1-clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSL`
- `Expat`
- `FSF`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Avisynth exception`
- `GPL-3`
- `GPL-3+`
- `IJG`
- `ISC`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Sundry`
- `Zlib`
- `man-page`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris ffmpeg=7:3.2.14-1~deb9u1
'http://deb.debian.org/debian/pool/main/f/ffmpeg/ffmpeg_3.2.14-1~deb9u1.dsc' ffmpeg_3.2.14-1~deb9u1.dsc 4914 SHA256:2cc4f796f8a8f1dcb17f0a33a0a93a3125802ba59cb4f26add74a3f3ea773bf0
'http://deb.debian.org/debian/pool/main/f/ffmpeg/ffmpeg_3.2.14.orig.tar.xz' ffmpeg_3.2.14.orig.tar.xz 8039380 SHA256:a0047aa0215538a13d10da2fe48674af574e8e94b7ecf3071bdf1addb056be92
'http://deb.debian.org/debian/pool/main/f/ffmpeg/ffmpeg_3.2.14-1~deb9u1.debian.tar.xz' ffmpeg_3.2.14-1~deb9u1.debian.tar.xz 39716 SHA256:1bc8465d4304e235f56eef92d84b8a320aecf81ff7c08dda4cf8daa3de52c5f5
```

Other potentially useful URLs:

- https://sources.debian.net/src/ffmpeg/7:3.2.14-1~deb9u1/ (for browsing the source)
- https://sources.debian.net/src/ffmpeg/7:3.2.14-1~deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ffmpeg/7:3.2.14-1~deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ffms2=2.23-1`

Binary Packages:

- `libffms2-4:amd64=2.23-1`

Licenses: (parsed from: `/usr/share/doc/libffms2-4/copyright`)

- `Expat`
- `GPL-2`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris ffms2=2.23-1
'http://deb.debian.org/debian/pool/main/f/ffms2/ffms2_2.23-1.dsc' ffms2_2.23-1.dsc 2254 SHA256:bbef9076354ef02db9677b379d8eb442301e482c39d03b324b17e11442688711
'http://deb.debian.org/debian/pool/main/f/ffms2/ffms2_2.23.orig.tar.gz' ffms2_2.23.orig.tar.gz 488940 SHA256:b09b2aa2b1c6f87f94a0a0dd8284b3c791cbe77f0f3df57af99ddebcd15273ed
'http://deb.debian.org/debian/pool/main/f/ffms2/ffms2_2.23-1.debian.tar.xz' ffms2_2.23-1.debian.tar.xz 9924 SHA256:7bad7d6e4d267364b44bfbd5151b8a151c74a987c3bce7d41bb739dd1c61bd1a
```

Other potentially useful URLs:

- https://sources.debian.net/src/ffms2/2.23-1/ (for browsing the source)
- https://sources.debian.net/src/ffms2/2.23-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ffms2/2.23-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fftw3=3.3.5-3`

Binary Packages:

- `libfftw3-double3:amd64=3.3.5-3`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.5-3
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.5-3.dsc' fftw3_3.3.5-3.dsc 2880 SHA256:6cfd2233e6ad4f12b922c785f5a1ce64ada28059221b67667159aafa33c70bd9
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.5.orig.tar.gz' fftw3_3.3.5.orig.tar.gz 4148447 SHA256:8ecfe1b04732ec3f5b7d279fdb8efcad536d555f9d1e8fabd027037d45ea8bcf
'http://deb.debian.org/debian/pool/main/f/fftw3/fftw3_3.3.5-3.debian.tar.xz' fftw3_3.3.5-3.debian.tar.xz 12700 SHA256:7d5098f2740b6648df4cc000fa5d7a358296e5bd7c9287b7be8fe7fee2a251ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/fftw3/3.3.5-3/ (for browsing the source)
- https://sources.debian.net/src/fftw3/3.3.5-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fftw3/3.3.5-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `flac=1.3.2-1`

Binary Packages:

- `libflac8:amd64=1.3.2-1`

Licenses: (parsed from: `/usr/share/doc/libflac8/copyright`)

- `BSD-3-clause`
- `GFDL-1.1+`
- `GFDL-1.2`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Public-domain`

Source:

```console
$ apt-get source -qq --print-uris flac=1.3.2-1
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.2-1.dsc' flac_1.3.2-1.dsc 2268 SHA256:a3fc6aa13a3e871c3e2b2a8adbae76ce9aec25f11329298831c74e8c4ba65293
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.2.orig.tar.xz' flac_1.3.2.orig.tar.xz 776192 SHA256:91cfc3ed61dc40f47f050a109b08610667d73477af6ef36dcad31c31a4a8d53f
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.2-1.debian.tar.xz' flac_1.3.2-1.debian.tar.xz 16840 SHA256:33580dfc82808cbb87b4afe24e4bf9e9c8941f9cede035235c76046f1908559f
```

Other potentially useful URLs:

- https://sources.debian.net/src/flac/1.3.2-1/ (for browsing the source)
- https://sources.debian.net/src/flac/1.3.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/flac/1.3.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `flite=2.0.0-release-3`

Binary Packages:

- `libflite1:amd64=2.0.0-release-3+b1`

Licenses: (parsed from: `/usr/share/doc/libflite1/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris flite=2.0.0-release-3
'http://deb.debian.org/debian/pool/main/f/flite/flite_2.0.0-release-3.dsc' flite_2.0.0-release-3.dsc 2209 SHA256:d0679eaaeca6b46e215d885a378e3636c831f8b5730f6d57b3546636ee53772f
'http://deb.debian.org/debian/pool/main/f/flite/flite_2.0.0-release.orig.tar.bz2' flite_2.0.0-release.orig.tar.bz2 14761376 SHA256:678c3860fd539402b5d1699b921239072af6acb4e72dc4720494112807cae411
'http://deb.debian.org/debian/pool/main/f/flite/flite_2.0.0-release-3.debian.tar.xz' flite_2.0.0-release-3.debian.tar.xz 30688 SHA256:be9fcd747d39b323e69cb11435fe0b8628a97276096faf635048e72e5bd2ef5b
```

Other potentially useful URLs:

- https://sources.debian.net/src/flite/2.0.0-release-3/ (for browsing the source)
- https://sources.debian.net/src/flite/2.0.0-release-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/flite/2.0.0-release-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fontconfig=2.11.0-6.7`

Binary Packages:

- `fontconfig=2.11.0-6.7+b1`
- `fontconfig-config=2.11.0-6.7`
- `libfontconfig1:amd64=2.11.0-6.7+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.11.0-6.7
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0-6.7.dsc' fontconfig_2.11.0-6.7.dsc 1851 SHA256:3e60036d03fb610d5ed398b7be0cfe0f9dea0ce9b25cb612acec6df11963a101
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0.orig.tar.xz' fontconfig_2.11.0.orig.tar.xz 319652 SHA256:f19c7366d59dc4e79eaf3eedabd44b6375b238f29316db5020a183c7d9a78db9
'http://deb.debian.org/debian/pool/main/f/fontconfig/fontconfig_2.11.0-6.7.debian.tar.xz' fontconfig_2.11.0-6.7.debian.tar.xz 1074508 SHA256:170c1e1a6221e0d3209b2a36507128aa3454135ca3dcd1eb2b06556e46c0c30e
```

Other potentially useful URLs:

- https://sources.debian.net/src/fontconfig/2.11.0-6.7/ (for browsing the source)
- https://sources.debian.net/src/fontconfig/2.11.0-6.7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fontconfig/2.11.0-6.7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fonts-dejavu=2.37-1`

Binary Packages:

- `fonts-dejavu=2.37-1`
- `fonts-dejavu-core=2.37-1`
- `fonts-dejavu-extra=2.37-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu/copyright`, `/usr/share/doc/fonts-dejavu-core/copyright`, `/usr/share/doc/fonts-dejavu-extra/copyright`)

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

### `dpkg` source package: `freetype=2.6.3-3.2`

Binary Packages:

- `libfreetype6:amd64=2.6.3-3.2`

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
$ apt-get source -qq --print-uris freetype=2.6.3-3.2
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.6.3-3.2.dsc' freetype_2.6.3-3.2.dsc 2292 SHA256:631d4fa321885bb0b950abc4061eb1a720fd249a14b940e4aa10dd78ce2a19b2
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.6.3.orig.tar.gz' freetype_2.6.3.orig.tar.gz 7313547 SHA256:814a22aad85e8ca2cb4acfc2e9dc59caa6eded4f6619590f7bd0a721e4b076a3
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.6.3-3.2.diff.gz' freetype_2.6.3-3.2.diff.gz 40027 SHA256:ca45f666d5bf5bcdadbff72f0c8d7335c36e2174e9fd07ef658a9def6eac6aff
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.6.3-3.2/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.6.3-3.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.6.3-3.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fribidi=0.19.7-1+deb9u1`

Binary Packages:

- `libfribidi0:amd64=0.19.7-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=0.19.7-1+deb9u1
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_0.19.7-1+deb9u1.dsc' fribidi_0.19.7-1+deb9u1.dsc 2310 SHA256:06a62577db1262c09f0cce69f859606011d8f2c98330ceee311de2b5a9836a83
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_0.19.7.orig.tar.bz2' fribidi_0.19.7.orig.tar.bz2 648299 SHA256:08222a6212bbc2276a2d55c3bf370109ae4a35b689acbc66571ad2a670595a8e
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_0.19.7-1+deb9u1.debian.tar.xz' fribidi_0.19.7-1+deb9u1.debian.tar.xz 7472 SHA256:3cf606035747c8b4de0cad7e6096acce2daa6e5b7a70fdcbc2b0e84ecce64839
```

Other potentially useful URLs:

- https://sources.debian.net/src/fribidi/0.19.7-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/fribidi/0.19.7-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fribidi/0.19.7-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `game-music-emu=0.6.0-4`

Binary Packages:

- `libgme0:amd64=0.6.0-4`

Licenses: (parsed from: `/usr/share/doc/libgme0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris game-music-emu=0.6.0-4
'http://deb.debian.org/debian/pool/main/g/game-music-emu/game-music-emu_0.6.0-4.dsc' game-music-emu_0.6.0-4.dsc 2009 SHA256:2bfc72d0b621b9a8f2b9974bec3508d0d775ddabac5c5bcce5b722251eeb3a19
'http://deb.debian.org/debian/pool/main/g/game-music-emu/game-music-emu_0.6.0.orig.tar.bz2' game-music-emu_0.6.0.orig.tar.bz2 170202 SHA256:506e81d0c61e1a26d503fbf5351503e0b31f9fbb374cb1f09979758b46a24987
'http://deb.debian.org/debian/pool/main/g/game-music-emu/game-music-emu_0.6.0-4.debian.tar.xz' game-music-emu_0.6.0-4.debian.tar.xz 5500 SHA256:f590ac6f3c9fa317927ca706fff614cd2968a6fca09c48b3e3a9afbc53b621b6
```

Other potentially useful URLs:

- https://sources.debian.net/src/game-music-emu/0.6.0-4/ (for browsing the source)
- https://sources.debian.net/src/game-music-emu/0.6.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/game-music-emu/0.6.0-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-6=6.3.0-18+deb9u1`

Binary Packages:

- `gcc-6-base:amd64=6.3.0-18+deb9u1`
- `libatomic1:amd64=6.3.0-18+deb9u1`
- `libgcc1:amd64=1:6.3.0-18+deb9u1`
- `libgfortran3:amd64=6.3.0-18+deb9u1`
- `libgomp1:amd64=6.3.0-18+deb9u1`
- `libquadmath0:amd64=6.3.0-18+deb9u1`
- `libstdc++6:amd64=6.3.0-18+deb9u1`

Licenses: (parsed from: `/usr/share/doc/gcc-6-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgfortran3/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`)

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

### `dpkg` source package: `gconf=3.2.6-4`

Binary Packages:

- `gconf-service=3.2.6-4+b1`
- `gconf2=3.2.6-4+b1`
- `gconf2-common=3.2.6-4`
- `libgconf-2-4:amd64=3.2.6-4+b1`

Licenses: (parsed from: `/usr/share/doc/gconf-service/copyright`, `/usr/share/doc/gconf2/copyright`, `/usr/share/doc/gconf2-common/copyright`, `/usr/share/doc/libgconf-2-4/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gconf=3.2.6-4
'http://deb.debian.org/debian/pool/main/g/gconf/gconf_3.2.6-4.dsc' gconf_3.2.6-4.dsc 2753 SHA256:383be6e1ef0781b024d48e00d2a06bb2f55f25af5797efca07361f2b77a018c7
'http://deb.debian.org/debian/pool/main/g/gconf/gconf_3.2.6.orig.tar.xz' gconf_3.2.6.orig.tar.xz 1559904 SHA256:1912b91803ab09a5eed34d364bf09fe3a2a9c96751fde03a4e0cfa51a04d784c
'http://deb.debian.org/debian/pool/main/g/gconf/gconf_3.2.6-4.debian.tar.xz' gconf_3.2.6-4.debian.tar.xz 25668 SHA256:70292212af5fc5e00819997ed60be98e889a92a88ba6a8cd1989b21a2e0d9872
```

Other potentially useful URLs:

- https://sources.debian.net/src/gconf/3.2.6-4/ (for browsing the source)
- https://sources.debian.net/src/gconf/3.2.6-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gconf/3.2.6-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gdk-pixbuf=2.36.5-2+deb9u2`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.36.5-2+deb9u2`
- `libgdk-pixbuf2.0-common=2.36.5-2+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.36.5-2+deb9u2
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.5-2+deb9u2.dsc' gdk-pixbuf_2.36.5-2+deb9u2.dsc 2841 SHA256:195f9aaa11064ce76b43b772851c0d786a7e40bc6205f16df6430d9f0740ec9c
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.5.orig.tar.xz' gdk-pixbuf_2.36.5.orig.tar.xz 5165640 SHA256:7ace06170291a1f21771552768bace072ecdea9bd4a02f7658939b9a314c40fc
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.5-2+deb9u2.debian.tar.xz' gdk-pixbuf_2.36.5-2+deb9u2.debian.tar.xz 15900 SHA256:bf3450ffdd075990f078c6e14f6a793513baaab469965308acfa4241b8e0cbdc
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdk-pixbuf/2.36.5-2+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/gdk-pixbuf/2.36.5-2+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdk-pixbuf/2.36.5-2+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ghostscript=9.26a~dfsg-0+deb9u6`

Binary Packages:

- `ghostscript=9.26a~dfsg-0+deb9u6`
- `libgs9:amd64=9.26a~dfsg-0+deb9u6`
- `libgs9-common=9.26a~dfsg-0+deb9u6`

Licenses: (parsed from: `/usr/share/doc/ghostscript/copyright`, `/usr/share/doc/libgs9/copyright`, `/usr/share/doc/libgs9-common/copyright`)

- `AGPL-3`
- `AGPL-3+`
- `AGPL-3+ with font exception`
- `Apache-2.0`
- `BSD-3-Clause`
- `BSD-3-Clause~Adobe`
- `Expat`
- `Expat~Ghostgum`
- `Expat~SunSoft`
- `Expat~SunSoft with SunSoft exception`
- `FTL`
- `GAP~configure`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `LGPL-2.1`
- `NTP~Lucent`
- `NTP~Open`
- `NTP~WSU`
- `ZLIB`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris ghostscript=9.26a~dfsg-0+deb9u6
'http://security.debian.org/debian-security/pool/updates/main/g/ghostscript/ghostscript_9.26a~dfsg-0+deb9u6.dsc' ghostscript_9.26a~dfsg-0+deb9u6.dsc 3052 SHA256:e01edd0554f12655d7dec2346e40da52e517dd569d60fdbf41745a9b9b586034
'http://security.debian.org/debian-security/pool/updates/main/g/ghostscript/ghostscript_9.26a~dfsg.orig.tar.xz' ghostscript_9.26a~dfsg.orig.tar.xz 17614652 SHA256:1c3647c42a3f894df22a7a12473f60ff4be38c38ed97232ecfab9b7f3a4fc8f4
'http://security.debian.org/debian-security/pool/updates/main/g/ghostscript/ghostscript_9.26a~dfsg-0+deb9u6.debian.tar.xz' ghostscript_9.26a~dfsg-0+deb9u6.debian.tar.xz 121476 SHA256:2edc57568f6f101ae1ed7df28ff29d4f373b336a3df688fa0533fee773719358
```

Other potentially useful URLs:

- https://sources.debian.net/src/ghostscript/9.26a~dfsg-0+deb9u6/ (for browsing the source)
- https://sources.debian.net/src/ghostscript/9.26a~dfsg-0+deb9u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ghostscript/9.26a~dfsg-0+deb9u6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.11.0-3+deb9u5`

Binary Packages:

- `git=1:2.11.0-3+deb9u5`
- `git-man=1:2.11.0-3+deb9u5`

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
$ apt-get source -qq --print-uris git=1:2.11.0-3+deb9u5
'http://security.debian.org/debian-security/pool/updates/main/g/git/git_2.11.0-3+deb9u5.dsc' git_2.11.0-3+deb9u5.dsc 2944 SHA256:0a0eeebee1b417f964ab45a0cec7c2a0835639960da68b86db618776bae6521f
'http://security.debian.org/debian-security/pool/updates/main/g/git/git_2.11.0.orig.tar.xz' git_2.11.0.orig.tar.xz 4197984 SHA256:7e7e8d69d494892373b87007674be5820a4bc1ef596a0117d03ea3169119fd0b
'http://security.debian.org/debian-security/pool/updates/main/g/git/git_2.11.0-3+deb9u5.debian.tar.xz' git_2.11.0-3+deb9u5.debian.tar.xz 572380 SHA256:ccf9c4a9c59ddc34df84b72e8bf8226328359abbf91205c397fabbb7c8168d8d
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.11.0-3+deb9u5/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.11.0-3+deb9u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.11.0-3+deb9u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glew=2.0.0-3`

Binary Packages:

- `libglew2.0:amd64=2.0.0-3+b1`

Licenses: (parsed from: `/usr/share/doc/libglew2.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `Mesa`

Source:

```console
$ apt-get source -qq --print-uris glew=2.0.0-3
'http://deb.debian.org/debian/pool/main/g/glew/glew_2.0.0-3.dsc' glew_2.0.0-3.dsc 2222 SHA256:019d48edeef4290a4900a9ce065bb7f27d2f5e7104dd51f902f75bb7e58e2818
'http://deb.debian.org/debian/pool/main/g/glew/glew_2.0.0.orig.tar.gz' glew_2.0.0.orig.tar.gz 667340 SHA256:c572c30a4e64689c342ba1624130ac98936d7af90c3103f9ce12b8a0c5736764
'http://deb.debian.org/debian/pool/main/g/glew/glew_2.0.0-3.debian.tar.xz' glew_2.0.0-3.debian.tar.xz 24528 SHA256:57f990a42a2b5a122b5dda15390445e1ffa8c81871a530d5a64eb4aa3f75f4c7
```

Other potentially useful URLs:

- https://sources.debian.net/src/glew/2.0.0-3/ (for browsing the source)
- https://sources.debian.net/src/glew/2.0.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glew/2.0.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib-networking=2.50.0-1`

Binary Packages:

- `glib-networking:amd64=2.50.0-1+b1`
- `glib-networking-common=2.50.0-1`
- `glib-networking-services=2.50.0-1+b1`

Licenses: (parsed from: `/usr/share/doc/glib-networking/copyright`, `/usr/share/doc/glib-networking-common/copyright`, `/usr/share/doc/glib-networking-services/copyright`)

- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris glib-networking=2.50.0-1
'http://deb.debian.org/debian/pool/main/g/glib-networking/glib-networking_2.50.0-1.dsc' glib-networking_2.50.0-1.dsc 2520 SHA256:aae08878a86aaf065939e0ffb84b02c79c416548318f3bc8247ab83b953f7529
'http://deb.debian.org/debian/pool/main/g/glib-networking/glib-networking_2.50.0.orig.tar.xz' glib-networking_2.50.0.orig.tar.xz 435380 SHA256:3f1a442f3c2a734946983532ce59ed49120319fdb10c938447c373d5e5286bee
'http://deb.debian.org/debian/pool/main/g/glib-networking/glib-networking_2.50.0-1.debian.tar.xz' glib-networking_2.50.0-1.debian.tar.xz 7260 SHA256:bfb77daa2b3272fc1a519ed141903dcc0bfc30732df0024276fc279af2e8d40f
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib-networking/2.50.0-1/ (for browsing the source)
- https://sources.debian.net/src/glib-networking/2.50.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib-networking/2.50.0-1/ (for access to the source package after it no longer exists in the archive)

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
- `libc-l10n=2.24-11+deb9u4`
- `libc6:amd64=2.24-11+deb9u4`
- `locales=2.24-11+deb9u4`
- `multiarch-support=2.24-11+deb9u4`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-l10n/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/locales/copyright`, `/usr/share/doc/multiarch-support/copyright`)

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

- `libgmp10:amd64=2:6.1.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

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

- `dirmngr=2.1.18-8~deb9u4`
- `gnupg=2.1.18-8~deb9u4`
- `gnupg-agent=2.1.18-8~deb9u4`
- `gpgv=2.1.18-8~deb9u4`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-agent/copyright`, `/usr/share/doc/gpgv/copyright`)

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

- `libgnutls30:amd64=3.5.8-5+deb9u4`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The MIT License (MIT)`
- `The main library is licensed under GNU Lesser`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.5.8-5+deb9u4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.8-5+deb9u4.dsc' gnutls28_3.5.8-5+deb9u4.dsc 3286 SHA256:688284aba04d8ff84c6636d354c844c06e691031eb9a2fccc2e41547ed2fac9e
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.8.orig.tar.xz' gnutls28_3.5.8.orig.tar.xz 7264448 SHA256:0e97f243ae72b70307d684b84c7fe679385aa7a7a0e37e5be810193dcc17d4ff
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.8.orig.tar.xz.asc' gnutls28_3.5.8.orig.tar.xz.asc 287 SHA256:417da9db564a841128edb2dc2c98465a5749541f7d71492cb7c4905a0bfeac82
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.5.8-5+deb9u4.debian.tar.xz' gnutls28_3.5.8-5+deb9u4.debian.tar.xz 111484 SHA256:9013debe7c67edcd8aff039ab250d294b61313e52f7bbbd212d68d0b4fcee187
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.5.8-5+deb9u4/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.5.8-5+deb9u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.5.8-5+deb9u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gpac=0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1`

Binary Packages:

- `libgpac4:amd64=0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libgpac4/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-3-clause-axiomatic`
- `BSD-3-clause-intel`
- `FreeType-License`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `JPEG-License`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.1`
- `OpenSSL-License`
- `Zlib`
- `other-3`
- `other-nonfree-1`
- `public-domain`
- `wxWidgets`

Source:

```console
$ apt-get source -qq --print-uris gpac=0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1
'http://deb.debian.org/debian/pool/main/g/gpac/gpac_0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1.dsc' gpac_0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1.dsc 2737 SHA256:fbe4e36d3f551b475806bf91c2a9a12aa4c7038e5b1694fd29fc156887824e09
'http://deb.debian.org/debian/pool/main/g/gpac/gpac_0.5.2-426-gc5ad4e4+dfsg5.orig.tar.xz' gpac_0.5.2-426-gc5ad4e4+dfsg5.orig.tar.xz 3607392 SHA256:964173b9fc2439daa0366951deed08f84235cc554b18e30a62197ba3afd35e00
'http://deb.debian.org/debian/pool/main/g/gpac/gpac_0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1.debian.tar.xz' gpac_0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1.debian.tar.xz 41400 SHA256:b4fb5a1fdfa5f35b4ce1936d7fdc8c1f253cfebf72103303daef5f48b68b5fe4
```

Other potentially useful URLs:

- https://sources.debian.net/src/gpac/0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/gpac/0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gpac/0.5.2-426-gc5ad4e4+dfsg5-3+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `graphite2=1.3.10-1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.10-1`

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
$ apt-get source -qq --print-uris graphite2=1.3.10-1
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.10-1.dsc' graphite2_1.3.10-1.dsc 2147 SHA256:09cb1f55860690770011475b0a298698787d9e1dccdb532c40c8f56e08b452a0
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.10.orig.tar.gz' graphite2_1.3.10.orig.tar.gz 3889647 SHA256:90fde3b2f9ea95d68ffb19278d07d9b8a7efa5ba0e413bebcea802ce05cda1ae
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.10-1.debian.tar.xz' graphite2_1.3.10-1.debian.tar.xz 10376 SHA256:ac48155885b8d091b779f419f64cfb3be9cb1b2512b85e28baa172c3c561acc7
```

Other potentially useful URLs:

- https://sources.debian.net/src/graphite2/1.3.10-1/ (for browsing the source)
- https://sources.debian.net/src/graphite2/1.3.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/graphite2/1.3.10-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gsettings-desktop-schemas=3.22.0-1`

Binary Packages:

- `gsettings-desktop-schemas=3.22.0-1`

Licenses: (parsed from: `/usr/share/doc/gsettings-desktop-schemas/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gsettings-desktop-schemas=3.22.0-1
'http://deb.debian.org/debian/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.22.0-1.dsc' gsettings-desktop-schemas_3.22.0-1.dsc 2488 SHA256:4e42e6d16e00afd77260855583d0de5202a9d1537be86073e45573a3332a4d88
'http://deb.debian.org/debian/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.22.0.orig.tar.xz' gsettings-desktop-schemas_3.22.0.orig.tar.xz 598412 SHA256:0f06c7ba34c3a99e4d58b10889496133c9aaad6698ea2d8405d481c7f1a7eae1
'http://deb.debian.org/debian/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.22.0-1.debian.tar.xz' gsettings-desktop-schemas_3.22.0-1.debian.tar.xz 4420 SHA256:72b4b20a2cc8978f54ecc3978b970ecfb0e474ebbd1292705e8616196d07adb9
```

Other potentially useful URLs:

- https://sources.debian.net/src/gsettings-desktop-schemas/3.22.0-1/ (for browsing the source)
- https://sources.debian.net/src/gsettings-desktop-schemas/3.22.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gsettings-desktop-schemas/3.22.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gst-plugins-base1.0=1.10.4-1+deb9u1`

Binary Packages:

- `libgstreamer-plugins-base1.0-0:amd64=1.10.4-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer-plugins-base1.0-0/copyright`)

- `BSD (2 clause)`
- `BSD (3 clause)`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`
- `MIT/X11 (BSD like) LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gst-plugins-base1.0=1.10.4-1+deb9u1
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.10.4-1+deb9u1.dsc' gst-plugins-base1.0_1.10.4-1+deb9u1.dsc 3809 SHA256:90b434da8135e2cb4275e0095c383de2e01f1263e79d61708a200142a9876ed9
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.10.4.orig.tar.xz' gst-plugins-base1.0_1.10.4.orig.tar.xz 3059368 SHA256:f6d245b6b3d4cb733f81ebb021074c525ece83db0c10e932794b339b8d935eb7
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.10.4-1+deb9u1.debian.tar.xz' gst-plugins-base1.0_1.10.4-1+deb9u1.debian.tar.xz 41944 SHA256:43951ef55643a21a5ff99e9ff5e3829f70839659769e772de069761f0e7a21a3
```

Other potentially useful URLs:

- https://sources.debian.net/src/gst-plugins-base1.0/1.10.4-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/gst-plugins-base1.0/1.10.4-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gst-plugins-base1.0/1.10.4-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gstreamer1.0=1.10.4-1`

Binary Packages:

- `libgstreamer1.0-0:amd64=1.10.4-1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer1.0-0/copyright`)

- `GPL-2+`
- `GPL-3+`
- `LGPL`
- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gstreamer1.0=1.10.4-1
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.10.4-1.dsc' gstreamer1.0_1.10.4-1.dsc 3188 SHA256:7de937f39bdb5e664f35a745af213bcf97055fe7b5219ffad27cdc576b6816f2
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.10.4.orig.tar.xz' gstreamer1.0_1.10.4.orig.tar.xz 3797376 SHA256:50c2f5af50a6cc6c0a3f3ed43bdd8b5e2bff00bacfb766d4be139ec06d8b5218
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.10.4-1.debian.tar.xz' gstreamer1.0_1.10.4-1.debian.tar.xz 42656 SHA256:feac223d9913500fa0489db4e099e1c05a8c2237d80416aebc752e572465ed59
```

Other potentially useful URLs:

- https://sources.debian.net/src/gstreamer1.0/1.10.4-1/ (for browsing the source)
- https://sources.debian.net/src/gstreamer1.0/1.10.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gstreamer1.0/1.10.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gtk+2.0=2.24.31-2`

Binary Packages:

- `libgtk2.0-0:amd64=2.24.31-2`
- `libgtk2.0-common=2.24.31-2`

Licenses: (parsed from: `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

- `LGPL-2`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+2.0=2.24.31-2
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.31-2.dsc' gtk+2.0_2.24.31-2.dsc 3839 SHA256:1588a80a0f8ef6b1ddeb92c629fc9da1930e13e5bba5cb0f7bbbee335e161d09
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.31.orig.tar.xz' gtk+2.0_2.24.31.orig.tar.xz 12805344 SHA256:68c1922732c7efc08df4656a5366dcc3afdc8791513400dac276009b40954658
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.31-2.debian.tar.xz' gtk+2.0_2.24.31-2.debian.tar.xz 87400 SHA256:56f1296c0f6fc3c319abee130fbd6c776b502ee53d8c8709ea42cd0f98b9d130
```

Other potentially useful URLs:

- https://sources.debian.net/src/gtk+2.0/2.24.31-2/ (for browsing the source)
- https://sources.debian.net/src/gtk+2.0/2.24.31-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gtk+2.0/2.24.31-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gtk+3.0=3.22.11-1`

Binary Packages:

- `gtk-update-icon-cache=3.22.11-1`
- `libgtk-3-0:amd64=3.22.11-1`
- `libgtk-3-common=3.22.11-1`

Licenses: (parsed from: `/usr/share/doc/gtk-update-icon-cache/copyright`, `/usr/share/doc/libgtk-3-0/copyright`, `/usr/share/doc/libgtk-3-common/copyright`)

- `Apache-2.0`
- `Expat`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+3.0=3.22.11-1
'http://deb.debian.org/debian/pool/main/g/gtk+3.0/gtk+3.0_3.22.11-1.dsc' gtk+3.0_3.22.11-1.dsc 3839 SHA256:afd63912ea63c668bec5da9025815c02fa3b964886eef866873e22633d18c122
'http://deb.debian.org/debian/pool/main/g/gtk+3.0/gtk+3.0_3.22.11.orig.tar.xz' gtk+3.0_3.22.11.orig.tar.xz 18250068 SHA256:db440670cb6f3c098b076df3735fbc4e69359bd605385e87c90ee48344a804ca
'http://deb.debian.org/debian/pool/main/g/gtk+3.0/gtk+3.0_3.22.11-1.debian.tar.xz' gtk+3.0_3.22.11-1.debian.tar.xz 143736 SHA256:347da5778d745b85a3b91940f4b302381219113d2bff4caf0a5f079660bc4cb0
```

Other potentially useful URLs:

- https://sources.debian.net/src/gtk+3.0/3.22.11-1/ (for browsing the source)
- https://sources.debian.net/src/gtk+3.0/3.22.11-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gtk+3.0/3.22.11-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gtkimageview=1.6.4+dfsg-1.1`

Binary Packages:

- `libgtkimageview0=1.6.4+dfsg-1.1`

Licenses: (parsed from: `/usr/share/doc/libgtkimageview0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris gtkimageview=1.6.4+dfsg-1.1
'http://deb.debian.org/debian/pool/main/g/gtkimageview/gtkimageview_1.6.4+dfsg-1.1.dsc' gtkimageview_1.6.4+dfsg-1.1.dsc 1915 SHA256:b1b3d76245faad76c9a2b41ade645f11dabc1b011e05f4777ded896f952fd924
'http://deb.debian.org/debian/pool/main/g/gtkimageview/gtkimageview_1.6.4+dfsg.orig.tar.gz' gtkimageview_1.6.4+dfsg.orig.tar.gz 1172925 SHA256:9336fe986658862ecf5abbc25a3d6dab12668c72b284d2f88b058d1abf4c5ef6
'http://deb.debian.org/debian/pool/main/g/gtkimageview/gtkimageview_1.6.4+dfsg-1.1.debian.tar.xz' gtkimageview_1.6.4+dfsg-1.1.debian.tar.xz 4852 SHA256:14d607911c611edd5d0e166cf45e0359876654f920885b5932150a9b3ed1b619
```

Other potentially useful URLs:

- https://sources.debian.net/src/gtkimageview/1.6.4+dfsg-1.1/ (for browsing the source)
- https://sources.debian.net/src/gtkimageview/1.6.4+dfsg-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gtkimageview/1.6.4+dfsg-1.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `harfbuzz=1.4.2-1`

Binary Packages:

- `libharfbuzz-icu0:amd64=1.4.2-1`
- `libharfbuzz0b:amd64=1.4.2-1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz-icu0/copyright`, `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=1.4.2-1
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_1.4.2-1.dsc' harfbuzz_1.4.2-1.dsc 2655 SHA256:48379f7aee8abee1b869745e12607ba81b02a3adf23b100558804f881dc5c9f1
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_1.4.2.orig.tar.bz2' harfbuzz_1.4.2.orig.tar.bz2 1446752 SHA256:8f234dcfab000fdec24d43674fffa2fdbdbd654eb176afbde30e8826339cb7b3
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_1.4.2-1.debian.tar.xz' harfbuzz_1.4.2-1.debian.tar.xz 8436 SHA256:f72ed9a6392e66816264c4f04a7926ec747a2a7b8eaf7ed1faf0bdacc788cf51
```

Other potentially useful URLs:

- https://sources.debian.net/src/harfbuzz/1.4.2-1/ (for browsing the source)
- https://sources.debian.net/src/harfbuzz/1.4.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/harfbuzz/1.4.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hicolor-icon-theme=0.15-1`

Binary Packages:

- `hicolor-icon-theme=0.15-1`

Licenses: (parsed from: `/usr/share/doc/hicolor-icon-theme/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris hicolor-icon-theme=0.15-1
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.15-1.dsc' hicolor-icon-theme_0.15-1.dsc 1588 SHA256:14450b4a0230793c4ba07d8aa87c657bdae60ae440f211fc693fdeb9fc3420d0
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.15.orig.tar.xz' hicolor-icon-theme_0.15.orig.tar.xz 51056 SHA256:9cc45ac3318c31212ea2d8cb99e64020732393ee7630fa6c1810af5f987033cc
'http://deb.debian.org/debian/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.15-1.debian.tar.xz' hicolor-icon-theme_0.15-1.debian.tar.xz 3524 SHA256:e11a79b49ba145e0c6985288abdf99447e4ff98bbb105eff82b402b55b99e0e2
```

Other potentially useful URLs:

- https://sources.debian.net/src/hicolor-icon-theme/0.15-1/ (for browsing the source)
- https://sources.debian.net/src/hicolor-icon-theme/0.15-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hicolor-icon-theme/0.15-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `hunspell=1.4.1-2`

Binary Packages:

- `libhunspell-1.4-0:amd64=1.4.1-2+b2`

Licenses: (parsed from: `/usr/share/doc/libhunspell-1.4-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris hunspell=1.4.1-2
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.4.1-2.dsc' hunspell_1.4.1-2.dsc 2098 SHA256:c47ec10e00197d43d5f8e06aae32abd25493befd5e9c0b5da20e8d4398326bfe
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.4.1.orig.tar.gz' hunspell_1.4.1.orig.tar.gz 1000647 SHA256:c4476aff0ced52eec334eae1e8d3fdaaebdd90f5ecd0b57cf2a92a6fd220d1bb
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.4.1-2.debian.tar.xz' hunspell_1.4.1-2.debian.tar.xz 20780 SHA256:459494f2fd3e307de5923713d0a7e8fed29db695542b0317eb508497033b7c8d
```

Other potentially useful URLs:

- https://sources.debian.net/src/hunspell/1.4.1-2/ (for browsing the source)
- https://sources.debian.net/src/hunspell/1.4.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hunspell/1.4.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hyphen=2.8.8-5`

Binary Packages:

- `libhyphen0:amd64=2.8.8-5`

Licenses: (parsed from: `/usr/share/doc/libhyphen0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.1+`

Source:

```console
$ apt-get source -qq --print-uris hyphen=2.8.8-5
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8-5.dsc' hyphen_2.8.8-5.dsc 2097 SHA256:f2d4b3129b865d87babdb4fa1142e9b3dafd7cc9739c1fbf534a09e8a64e936b
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8.orig.tar.gz' hyphen_2.8.8.orig.tar.gz 638369 SHA256:304636d4eccd81a14b6914d07b84c79ebb815288c76fe027b9ebff6ff24d5705
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8-5.debian.tar.xz' hyphen_2.8.8-5.debian.tar.xz 12012 SHA256:ab8848f6e7cd71a6f806ab17c51c871f773e4d0ad58bb02b75bdd051c001460e
```

Other potentially useful URLs:

- https://sources.debian.net/src/hyphen/2.8.8-5/ (for browsing the source)
- https://sources.debian.net/src/hyphen/2.8.8-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hyphen/2.8.8-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `icu=57.1-6+deb9u3`

Binary Packages:

- `libicu57:amd64=57.1-6+deb9u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=57.1-6+deb9u3
'http://deb.debian.org/debian/pool/main/i/icu/icu_57.1-6+deb9u3.dsc' icu_57.1-6+deb9u3.dsc 2133 SHA256:4bde9bfbe39f0449010d5fb6863965674a2b7636cb5f55728d3f1ea790a4c1c0
'http://deb.debian.org/debian/pool/main/i/icu/icu_57.1.orig.tar.gz' icu_57.1.orig.tar.gz 22360664 SHA256:ff8c67cb65949b1e7808f2359f2b80f722697048e90e7cfc382ec1fe229e9581
'http://deb.debian.org/debian/pool/main/i/icu/icu_57.1-6+deb9u3.debian.tar.xz' icu_57.1-6+deb9u3.debian.tar.xz 34972 SHA256:8e24064ea1bc6ac1e96feede642723106bd7890718859ae0c36778ddca708ecc
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/57.1-6+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/icu/57.1-6+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/57.1-6+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ijs=0.35-12`

Binary Packages:

- `libijs-0.35:amd64=0.35-12`

Licenses: (parsed from: `/usr/share/doc/libijs-0.35/copyright`)

- `Expat`
- `Expat~X`
- `Expat~X with X exception`
- `GAP`
- `GAP~Makefile.in`
- `GAP~configure`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`

Source:

```console
$ apt-get source -qq --print-uris ijs=0.35-12
'http://deb.debian.org/debian/pool/main/i/ijs/ijs_0.35-12.dsc' ijs_0.35-12.dsc 1912 SHA256:e61103c05c58a623430262e7f7678899e23dd320b9ad0a931b6e8de143706a96
'http://deb.debian.org/debian/pool/main/i/ijs/ijs_0.35.orig.tar.gz' ijs_0.35.orig.tar.gz 344262 SHA256:901fffb73e42dae343a8285a31d9c4e82dc3856d36be30adbdb564bdd27161d6
'http://deb.debian.org/debian/pool/main/i/ijs/ijs_0.35-12.debian.tar.xz' ijs_0.35-12.debian.tar.xz 7812 SHA256:1007ae4f8dbabab90b2d2acf234031260bba26a05c2f31be822e63e27907e8ac
```

Other potentially useful URLs:

- https://sources.debian.net/src/ijs/0.35-12/ (for browsing the source)
- https://sources.debian.net/src/ijs/0.35-12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ijs/0.35-12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `imagemagick=8:6.9.7.4+dfsg-11+deb9u7`

Binary Packages:

- `imagemagick=8:6.9.7.4+dfsg-11+deb9u7`
- `imagemagick-6-common=8:6.9.7.4+dfsg-11+deb9u7`
- `imagemagick-6.q16=8:6.9.7.4+dfsg-11+deb9u7`
- `libmagickcore-6.q16-3:amd64=8:6.9.7.4+dfsg-11+deb9u7`
- `libmagickwand-6.q16-3:amd64=8:6.9.7.4+dfsg-11+deb9u7`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/libmagickcore-6.q16-3/copyright`, `/usr/share/doc/libmagickwand-6.q16-3/copyright`)

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
- `LGPL-3`
- `LGPL-3+`
- `Magick++`
- `Perllikelicence`
- `TatcherUlrichPublicDomain`

Source:

```console
$ apt-get source -qq --print-uris imagemagick=8:6.9.7.4+dfsg-11+deb9u7
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg-11+deb9u7.dsc' imagemagick_6.9.7.4+dfsg-11+deb9u7.dsc 5165 SHA256:fdc1447a6b42d535ccec23dd0b526361606f339cc0df01b9152d3dd27c776424
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg.orig.tar.xz' imagemagick_6.9.7.4+dfsg.orig.tar.xz 8929800 SHA256:47fb2cdd26f5913318c4504f16ea363e04d1f400dda9ec52e461ab661d724026
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg-11+deb9u7.debian.tar.xz' imagemagick_6.9.7.4+dfsg-11+deb9u7.debian.tar.xz 245624 SHA256:3112539cad0b68c31d420721a299c553fdc390bcc2fb9e26d7453e4918f69228
```

Other potentially useful URLs:

- https://sources.debian.net/src/imagemagick/8:6.9.7.4+dfsg-11+deb9u7/ (for browsing the source)
- https://sources.debian.net/src/imagemagick/8:6.9.7.4+dfsg-11+deb9u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/imagemagick/8:6.9.7.4+dfsg-11+deb9u7/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `iproute2=4.9.0-1+deb9u1`

Binary Packages:

- `iproute2=4.9.0-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris iproute2=4.9.0-1+deb9u1
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_4.9.0-1+deb9u1.dsc' iproute2_4.9.0-1+deb9u1.dsc 2425 SHA256:ad3365cc61f116f8dc8cc2a615549ffc9ed0217223393078b68e1d96649b2ce7
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_4.9.0.orig.tar.xz' iproute2_4.9.0.orig.tar.xz 613032 SHA256:c0f30f043f7767cc1b2cd2197b08d4e9b2392c95823fabe30bbce308c30116c4
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_4.9.0-1+deb9u1.debian.tar.xz' iproute2_4.9.0-1+deb9u1.debian.tar.xz 28316 SHA256:c5056293c85daf0a96550c0bfa6ae2851c78cec4ed5932909c976607caa1e561
```

Other potentially useful URLs:

- https://sources.debian.net/src/iproute2/4.9.0-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/iproute2/4.9.0-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iproute2/4.9.0-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iptables=1.6.0+snapshot20161117-6`

Binary Packages:

- `libip4tc0:amd64=1.6.0+snapshot20161117-6`

Licenses: (parsed from: `/usr/share/doc/libip4tc0/copyright`)

- `Artistic-2`
- `GPL-2`
- `GPL-2+`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris iptables=1.6.0+snapshot20161117-6
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.6.0+snapshot20161117-6.dsc' iptables_1.6.0+snapshot20161117-6.dsc 2818 SHA256:5ba41a2377437d3fa26d16029562de52df33dd4b870cbc8de062a5d591aed004
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.6.0+snapshot20161117.orig.tar.bz2' iptables_1.6.0+snapshot20161117.orig.tar.bz2 337604 SHA256:4279f8a732edd01091dbc11e6766529b71b342337ad016d09653636d77339983
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.6.0+snapshot20161117-6.debian.tar.xz' iptables_1.6.0+snapshot20161117-6.debian.tar.xz 62052 SHA256:fc9d7816f840ff1777e5b110a82a5900f11f4fa503f2c3e55cd7d21935ae9f51
```

Other potentially useful URLs:

- https://sources.debian.net/src/iptables/1.6.0+snapshot20161117-6/ (for browsing the source)
- https://sources.debian.net/src/iptables/1.6.0+snapshot20161117-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iptables/1.6.0+snapshot20161117-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iputils=3:20161105-1`

Binary Packages:

- `iputils-ping=3:20161105-1`

Licenses: (parsed from: `/usr/share/doc/iputils-ping/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris iputils=3:20161105-1
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20161105-1.dsc' iputils_20161105-1.dsc 2086 SHA256:7e810cf28c14f1e5fb7b51620dd4af748a97202967ee4fb5d4ee3111eb66f4ae
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20161105.orig.tar.bz2' iputils_20161105.orig.tar.bz2 159944 SHA256:fc193249341d240b227ce4246d7b0ceb30c1186608c7deff7261c8a2607ad02e
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20161105-1.debian.tar.xz' iputils_20161105-1.debian.tar.xz 10976 SHA256:1216eb9d51a85004524fea30320bad3ea45adaf5a17ec5a9ea3bafad697fd612
```

Other potentially useful URLs:

- https://sources.debian.net/src/iputils/3:20161105-1/ (for browsing the source)
- https://sources.debian.net/src/iputils/3:20161105-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iputils/3:20161105-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iso-codes=3.75-1`

Binary Packages:

- `iso-codes=3.75-1`

Licenses: (parsed from: `/usr/share/doc/iso-codes/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris iso-codes=3.75-1
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_3.75-1.dsc' iso-codes_3.75-1.dsc 1972 SHA256:61ed2941f3803ce9fc143f539fd154e4f49cee4ec8e8434f98c9af28b56bd309
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_3.75.orig.tar.xz' iso-codes_3.75.orig.tar.xz 3461424 SHA256:7335e0301cd77cd4ee019bf5d3709aa79309d49dd66e85ba350caf67e00b00cd
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_3.75-1.debian.tar.xz' iso-codes_3.75-1.debian.tar.xz 23084 SHA256:4a6485818ef95d50a053981876505e8fcdb6ba84dc4f53a12fca1196a79e94e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/iso-codes/3.75-1/ (for browsing the source)
- https://sources.debian.net/src/iso-codes/3.75-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iso-codes/3.75-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jackd2=1.9.10+20150825git1ed50c92~dfsg-5`

Binary Packages:

- `libjack-jackd2-0:amd64=1.9.10+20150825git1ed50c92~dfsg-5`

Licenses: (parsed from: `/usr/share/doc/libjack-jackd2-0/copyright`)

- `BSD-3-clause`
- `Expat`
- `Expat~modrequest`
- `GPL-2`
- `GPL-2+`
- `GPL-2~either`
- `GPL-2~jack-audio-connection-kit`
- `GPL-2~jackd2`
- `GPL-2~or`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `None`
- `public-domain~Kroon`

Source:

```console
$ apt-get source -qq --print-uris jackd2=1.9.10+20150825git1ed50c92~dfsg-5
'http://deb.debian.org/debian/pool/main/j/jackd2/jackd2_1.9.10+20150825git1ed50c92~dfsg-5.dsc' jackd2_1.9.10+20150825git1ed50c92~dfsg-5.dsc 2692 SHA256:b14ad633aa2edf943bfd7de664fa832ae93b9191a6c083f5f88ed3938d45ee00
'http://deb.debian.org/debian/pool/main/j/jackd2/jackd2_1.9.10+20150825git1ed50c92~dfsg.orig.tar.gz' jackd2_1.9.10+20150825git1ed50c92~dfsg.orig.tar.gz 1323432 SHA256:7127ecc608775de8f47ea4f88f1ad75b17eb660745236e2cad3e14d8b98fe791
'http://deb.debian.org/debian/pool/main/j/jackd2/jackd2_1.9.10+20150825git1ed50c92~dfsg-5.debian.tar.xz' jackd2_1.9.10+20150825git1ed50c92~dfsg-5.debian.tar.xz 40188 SHA256:17e7641eecaf680278e98611a1ae65dbe0a32eb45eeded8c1215cf0821ac74ce
```

Other potentially useful URLs:

- https://sources.debian.net/src/jackd2/1.9.10+20150825git1ed50c92~dfsg-5/ (for browsing the source)
- https://sources.debian.net/src/jackd2/1.9.10+20150825git1ed50c92~dfsg-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jackd2/1.9.10+20150825git1ed50c92~dfsg-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jbig2dec=0.13-4.1`

Binary Packages:

- `libjbig2dec0:amd64=0.13-4.1`

Licenses: (parsed from: `/usr/share/doc/libjbig2dec0/copyright`)

- `AGPL-3`
- `AGPL-3+`
- `BSD-2-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `pubic-domain`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris jbig2dec=0.13-4.1
'http://deb.debian.org/debian/pool/main/j/jbig2dec/jbig2dec_0.13-4.1.dsc' jbig2dec_0.13-4.1.dsc 2291 SHA256:4fca01f41a817e412d79fa4148567f9945594d02b0f45b02ec307908d66a5f73
'http://deb.debian.org/debian/pool/main/j/jbig2dec/jbig2dec_0.13.orig.tar.gz' jbig2dec_0.13.orig.tar.gz 122387 SHA256:c8b13b78d4bfd85df088943370cf93768e19c6f5dfe74178d7088e54b6db4ffb
'http://deb.debian.org/debian/pool/main/j/jbig2dec/jbig2dec_0.13-4.1.debian.tar.xz' jbig2dec_0.13-4.1.debian.tar.xz 25568 SHA256:41114245b7410a03196c5f7def10efa78c9da12b4bac9d21d6fbe96ded4232dd
```

Other potentially useful URLs:

- https://sources.debian.net/src/jbig2dec/0.13-4.1/ (for browsing the source)
- https://sources.debian.net/src/jbig2dec/0.13-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jbig2dec/0.13-4.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `json-glib=1.2.6-1`

Binary Packages:

- `libjson-glib-1.0-0:amd64=1.2.6-1`
- `libjson-glib-1.0-common=1.2.6-1`

Licenses: (parsed from: `/usr/share/doc/libjson-glib-1.0-0/copyright`, `/usr/share/doc/libjson-glib-1.0-common/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris json-glib=1.2.6-1
'http://deb.debian.org/debian/pool/main/j/json-glib/json-glib_1.2.6-1.dsc' json-glib_1.2.6-1.dsc 2675 SHA256:210306e8bafda8598469cf467add883a4046871fd7574c2b8d2a6f173a0ab25e
'http://deb.debian.org/debian/pool/main/j/json-glib/json-glib_1.2.6.orig.tar.xz' json-glib_1.2.6.orig.tar.xz 601188 SHA256:958fa59909ef28399c811aff29a5340b330b20660ca3586b4c5aa3a53997776c
'http://deb.debian.org/debian/pool/main/j/json-glib/json-glib_1.2.6-1.debian.tar.xz' json-glib_1.2.6-1.debian.tar.xz 6072 SHA256:07b3e5a0c75214bb6523a51a38908538fd9d4c7bc691f581f9d2f9628c9ca43d
```

Other potentially useful URLs:

- https://sources.debian.net/src/json-glib/1.2.6-1/ (for browsing the source)
- https://sources.debian.net/src/json-glib/1.2.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/json-glib/1.2.6-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `kmod=23-2`

Binary Packages:

- `libkmod2:amd64=23-2`

Licenses: (parsed from: `/usr/share/doc/libkmod2/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris kmod=23-2
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_23-2.dsc' kmod_23-2.dsc 1806 SHA256:fc0489b30b10c593c857f4b970bbfa7e486fdbffbbac17587ceb135847ce5cf4
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_23.orig.tar.xz' kmod_23.orig.tar.xz 160848 SHA256:d9a3440d09ea5e203ed03f7c75018001f7d6c923507b3bc8aaa428424c7c67df
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_23-2.debian.tar.xz' kmod_23-2.debian.tar.xz 9352 SHA256:93e06db753f9cf817821f65071bef9502b999d2d5b5d5bf908711716c70b0342
```

Other potentially useful URLs:

- https://sources.debian.net/src/kmod/23-2/ (for browsing the source)
- https://sources.debian.net/src/kmod/23-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/kmod/23-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `lame=3.99.5+repack1-9`

Binary Packages:

- `libmp3lame0:amd64=3.99.5+repack1-9+b2`

Licenses: (parsed from: `/usr/share/doc/libmp3lame0/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-1+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris lame=3.99.5+repack1-9
'http://deb.debian.org/debian/pool/main/l/lame/lame_3.99.5+repack1-9.dsc' lame_3.99.5+repack1-9.dsc 2274 SHA256:4ab9e3ebade5b00923ee516cbf801691fa8a5063edc7b126077a4fe11bbf5326
'http://deb.debian.org/debian/pool/main/l/lame/lame_3.99.5+repack1.orig.tar.gz' lame_3.99.5+repack1.orig.tar.gz 1464016 SHA256:01c1a34dc5ced11a487f04514cb948d38f6f559daebc85ae23c1c8a6c8280c95
'http://deb.debian.org/debian/pool/main/l/lame/lame_3.99.5+repack1-9.debian.tar.xz' lame_3.99.5+repack1-9.debian.tar.xz 15404 SHA256:ad2db943c9c9a1c09195bfc26330dc96f25a19b5631132dcb81a29ee10230272
```

Other potentially useful URLs:

- https://sources.debian.net/src/lame/3.99.5+repack1-9/ (for browsing the source)
- https://sources.debian.net/src/lame/3.99.5+repack1-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lame/3.99.5+repack1-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lapack=3.7.0-2`

Binary Packages:

- `libblas-common=3.7.0-2`
- `libblas3=3.7.0-2`
- `liblapack3=3.7.0-2`

Licenses: (parsed from: `/usr/share/doc/libblas-common/copyright`, `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.7.0-2
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.7.0-2.dsc' lapack_3.7.0-2.dsc 2900 SHA256:8e6a856bbf932f19456de2bad5b2955ae0ccb36e740d38afe011444be10fac9f
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.7.0.orig.tar.gz' lapack_3.7.0.orig.tar.gz 7359812 SHA256:ed967e4307e986474ab02eb810eed1d1adc73f5e1e3bc78fb009f6fe766db3be
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.7.0-2.debian.tar.xz' lapack_3.7.0-2.debian.tar.xz 21100 SHA256:bc423933dd01b179bee02649675f5b87f669945530b291aeb95229f5e8d51035
```

Other potentially useful URLs:

- https://sources.debian.net/src/lapack/3.7.0-2/ (for browsing the source)
- https://sources.debian.net/src/lapack/3.7.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lapack/3.7.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.8-4+deb9u1`

Binary Packages:

- `liblcms2-2:amd64=2.8-4+deb9u1`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.8-4+deb9u1
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.8-4+deb9u1.dsc' lcms2_2.8-4+deb9u1.dsc 2025 SHA256:47144a3cf2a008da72f32747f7e07be6e940bdc4fbeef80c07c2c65346f8ec43
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.8.orig.tar.gz' lcms2_2.8.orig.tar.gz 6687005 SHA256:66d02b229d2ea9474e62c2b6cd6720fde946155cd1d0d2bffdab829790a0fb22
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.8-4+deb9u1.debian.tar.xz' lcms2_2.8-4+deb9u1.debian.tar.xz 11492 SHA256:9e1d8156c301000aec3af9c861c5db4984bb820caca724e5d5bc8bd39cb5fed3
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.8-4+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.8-4+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.8-4+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lensfun=0.3.2-3`

Binary Packages:

- `liblensfun-data-v1=0.3.2-3`
- `liblensfun1:amd64=0.3.2-3`

Licenses: (parsed from: `/usr/share/doc/liblensfun-data-v1/copyright`, `/usr/share/doc/liblensfun1/copyright`)

- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris lensfun=0.3.2-3
'http://deb.debian.org/debian/pool/main/l/lensfun/lensfun_0.3.2-3.dsc' lensfun_0.3.2-3.dsc 2328 SHA256:ba6a7ac2098d7a224131f7d4ee0182ff8aa0efc737f5e74d5844d631786a2f57
'http://deb.debian.org/debian/pool/main/l/lensfun/lensfun_0.3.2.orig.tar.gz' lensfun_0.3.2.orig.tar.gz 784825 SHA256:ae8bcad46614ca47f5bda65b00af4a257a9564a61725df9c74cb260da544d331
'http://deb.debian.org/debian/pool/main/l/lensfun/lensfun_0.3.2-3.debian.tar.xz' lensfun_0.3.2-3.debian.tar.xz 13036 SHA256:74ebf5d6438a0325e1ff6d2ff85bc40a5e24bd112d966d55cb8bb0bf63b0007b
```

Other potentially useful URLs:

- https://sources.debian.net/src/lensfun/0.3.2-3/ (for browsing the source)
- https://sources.debian.net/src/lensfun/0.3.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lensfun/0.3.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libabw=0.1.1-4`

Binary Packages:

- `libabw-0.1-1:amd64=0.1.1-4`

Licenses: (parsed from: `/usr/share/doc/libabw-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3 | LGPL-3`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libabw=0.1.1-4
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.1-4.dsc' libabw_0.1.1-4.dsc 1952 SHA256:bf776861001f864fa1bf7a61e0d673d6012ffb2690d42d3e1a718ebc86141667
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.1.orig.tar.bz2' libabw_0.1.1.orig.tar.bz2 369311 SHA256:7a3d3415cf82ab9894f601d1b3057c4615060304d5279efdec6275e01b96a199
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.1-4.debian.tar.xz' libabw_0.1.1-4.debian.tar.xz 12984 SHA256:d56d9aacf51252b429963a1aca0d8636cfe6b20ab5586bca24ede460a0ce13c7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libabw/0.1.1-4/ (for browsing the source)
- https://sources.debian.net/src/libabw/0.1.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libabw/0.1.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libass=1:0.13.4-2`

Binary Packages:

- `libass5:amd64=1:0.13.4-2`

Licenses: (parsed from: `/usr/share/doc/libass5/copyright`)

- `GPL-2`
- `GPL-2+`
- `ISC`
- `other-1`

Source:

```console
$ apt-get source -qq --print-uris libass=1:0.13.4-2
'http://deb.debian.org/debian/pool/main/liba/libass/libass_0.13.4-2.dsc' libass_0.13.4-2.dsc 2143 SHA256:915eb1470f0667598e47d29ddefc2d083d534c92dfa9ed70e5d2eb33c9639cdd
'http://deb.debian.org/debian/pool/main/liba/libass/libass_0.13.4.orig.tar.xz' libass_0.13.4.orig.tar.xz 350840 SHA256:d84a2fc89011b99d87fc47af91906622707c165d1860e9f774825ebbbc9c9fb6
'http://deb.debian.org/debian/pool/main/liba/libass/libass_0.13.4-2.debian.tar.xz' libass_0.13.4-2.debian.tar.xz 5632 SHA256:4cde3bb53620c29b38b5134b7a2769673936edc13fe06ced1a1c64c434efb479
```

Other potentially useful URLs:

- https://sources.debian.net/src/libass/1:0.13.4-2/ (for browsing the source)
- https://sources.debian.net/src/libass/1:0.13.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libass/1:0.13.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.4.3-2`

Binary Packages:

- `libassuan0:amd64=2.4.3-2`

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
$ apt-get source -qq --print-uris libassuan=2.4.3-2
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.4.3-2.dsc' libassuan_2.4.3-2.dsc 2412 SHA256:fc057ff6bd548161cd978f7847682928222d31db96bd94d7ec0fc84b176bbcc7
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.4.3.orig.tar.bz2' libassuan_2.4.3.orig.tar.bz2 559867 SHA256:22843a3bdb256f59be49842abf24da76700354293a066d82ade8134bb5aa2b71
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.4.3-2.debian.tar.xz' libassuan_2.4.3-2.debian.tar.xz 15076 SHA256:16dd66909cf3b79c71d5169f35d94be64d079d882f027577c00c23bff3148012
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.4.3-2/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.4.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.4.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libasyncns=0.8-6`

Binary Packages:

- `libasyncns0:amd64=0.8-6`

Licenses: (parsed from: `/usr/share/doc/libasyncns0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libasyncns=0.8-6
'http://deb.debian.org/debian/pool/main/liba/libasyncns/libasyncns_0.8-6.dsc' libasyncns_0.8-6.dsc 1921 SHA256:d6a3cccafadceda0bd1542c6325c6238ec34a8ff85276d6f2e5914e282c67dc6
'http://deb.debian.org/debian/pool/main/liba/libasyncns/libasyncns_0.8.orig.tar.gz' libasyncns_0.8.orig.tar.gz 341591 SHA256:4f1a66e746cbe54ff3c2fbada5843df4fbbbe7481d80be003e8d11161935ab74
'http://deb.debian.org/debian/pool/main/liba/libasyncns/libasyncns_0.8-6.debian.tar.xz' libasyncns_0.8-6.debian.tar.xz 4564 SHA256:69b23a155b8a3da3bf68b1e440283e117c55e92bd3b4aa308605fe3f1164485e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libasyncns/0.8-6/ (for browsing the source)
- https://sources.debian.net/src/libasyncns/0.8-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libasyncns/0.8-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libavc1394=0.5.4-4`

Binary Packages:

- `libavc1394-0:amd64=0.5.4-4+b1`

Licenses: (parsed from: `/usr/share/doc/libavc1394-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libavc1394=0.5.4-4
'http://deb.debian.org/debian/pool/main/liba/libavc1394/libavc1394_0.5.4-4.dsc' libavc1394_0.5.4-4.dsc 2153 SHA256:e0fcaa8cfbf5b681575b8e56cdae9235baa6d8d0f5832ac08c7c8438276f0d7b
'http://deb.debian.org/debian/pool/main/liba/libavc1394/libavc1394_0.5.4.orig.tar.gz' libavc1394_0.5.4.orig.tar.gz 341679 SHA256:7cb1ff09506ae911ca9860bef4af08c2403f3e131f6c913a2cbd6ddca4215b53
'http://deb.debian.org/debian/pool/main/liba/libavc1394/libavc1394_0.5.4-4.debian.tar.xz' libavc1394_0.5.4-4.debian.tar.xz 6504 SHA256:2fd8771875db51024e01ac35b47ac873ce555a6bc8d2919346269cc1c450a472
```

Other potentially useful URLs:

- https://sources.debian.net/src/libavc1394/0.5.4-4/ (for browsing the source)
- https://sources.debian.net/src/libavc1394/0.5.4-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libavc1394/0.5.4-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbluray=1:0.9.3-3`

Binary Packages:

- `libbluray1:amd64=1:0.9.3-3`

Licenses: (parsed from: `/usr/share/doc/libbluray1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.0`

Source:

```console
$ apt-get source -qq --print-uris libbluray=1:0.9.3-3
'http://deb.debian.org/debian/pool/main/libb/libbluray/libbluray_0.9.3-3.dsc' libbluray_0.9.3-3.dsc 2556 SHA256:24059aaeb9859ca243bb4439aef9213d9daf2fae0adae21b40f939a8168ded60
'http://deb.debian.org/debian/pool/main/libb/libbluray/libbluray_0.9.3.orig.tar.bz2' libbluray_0.9.3.orig.tar.bz2 722686 SHA256:a6366614ec45484b51fe94fcd1975b3b8716f90f038a33b24d59978de3863ce0
'http://deb.debian.org/debian/pool/main/libb/libbluray/libbluray_0.9.3-3.debian.tar.xz' libbluray_0.9.3-3.debian.tar.xz 16792 SHA256:d3f8749e9e825452a91dceaf1e0489c88c727fa3f05ca5391a28707f8e73119f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbluray/1:0.9.3-3/ (for browsing the source)
- https://sources.debian.net/src/libbluray/1:0.9.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbluray/1:0.9.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbs2b=3.1.0+dfsg-2.2`

Binary Packages:

- `libbs2b0:amd64=3.1.0+dfsg-2.2`

Licenses: (parsed from: `/usr/share/doc/libbs2b0/copyright`)

- `FSF-unlimited`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `MIT+FSF-public`

Source:

```console
$ apt-get source -qq --print-uris libbs2b=3.1.0+dfsg-2.2
'http://deb.debian.org/debian/pool/main/libb/libbs2b/libbs2b_3.1.0+dfsg-2.2.dsc' libbs2b_3.1.0+dfsg-2.2.dsc 1939 SHA256:a5fa01cf653b4161bb8595509be5ee91d1f47b8a9ff2b8c98b7fdd60b290e643
'http://deb.debian.org/debian/pool/main/libb/libbs2b/libbs2b_3.1.0+dfsg.orig.tar.gz' libbs2b_3.1.0+dfsg.orig.tar.gz 330675 SHA256:c23faf614f787342c1a1a40f83064f2e5a49391733c029dc31d09fba759cee0a
'http://deb.debian.org/debian/pool/main/libb/libbs2b/libbs2b_3.1.0+dfsg-2.2.debian.tar.xz' libbs2b_3.1.0+dfsg-2.2.debian.tar.xz 4632 SHA256:37d7d8da3d0ab030ca49944e98c83b4ae8a4463d3a70c301af79da20e05b0440
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbs2b/3.1.0+dfsg-2.2/ (for browsing the source)
- https://sources.debian.net/src/libbs2b/3.1.0+dfsg-2.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbs2b/3.1.0+dfsg-2.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.8.3-1`

Binary Packages:

- `libbsd0:amd64=0.8.3-1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-Peter-Wemm`
- `BSD-3-clause-Regents`
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
$ apt-get source -qq --print-uris libbsd=0.8.3-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.3-1.dsc' libbsd_0.8.3-1.dsc 2212 SHA256:8b53b3731a95f00a0f47195e6afdf8dc4bcb3ed3b9b0d3e7046d8c9c98e5c8f2
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.3.orig.tar.xz' libbsd_0.8.3.orig.tar.xz 356772 SHA256:934b634f4dfd865b6482650b8f522c70ae65c463529de8be907b53c89c3a34a8
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.3.orig.tar.xz.asc' libbsd_0.8.3.orig.tar.xz.asc 819 SHA256:c0e26a577d19404d05515e0559b9224106a59ecd30910d6896694c4a5a4b021d
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.8.3-1.debian.tar.xz' libbsd_0.8.3-1.debian.tar.xz 14924 SHA256:c2beb8b2c4678c9f700b09834d1083fb6b1f883b112e493bd1ed1177355114fc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.8.3-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.8.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.8.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcaca=0.99.beta19-2.1~deb9u1`

Binary Packages:

- `libcaca0:amd64=0.99.beta19-2.1~deb9u1`

Licenses: (parsed from: `/usr/share/doc/libcaca0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcaca=0.99.beta19-2.1~deb9u1
'http://deb.debian.org/debian/pool/main/libc/libcaca/libcaca_0.99.beta19-2.1~deb9u1.dsc' libcaca_0.99.beta19-2.1~deb9u1.dsc 2277 SHA256:e898d3cc99ab8845d415c5e6487eebafc37d8776ce863da9bf46862040b920ab
'http://deb.debian.org/debian/pool/main/libc/libcaca/libcaca_0.99.beta19.orig.tar.gz' libcaca_0.99.beta19.orig.tar.gz 1203495 SHA256:128b467c4ed03264c187405172a4e83049342cc8cc2f655f53a2d0ee9d3772f4
'http://deb.debian.org/debian/pool/main/libc/libcaca/libcaca_0.99.beta19-2.1~deb9u1.debian.tar.xz' libcaca_0.99.beta19-2.1~deb9u1.debian.tar.xz 12664 SHA256:0953344df9c0385a54d6e928f2f20bb8a3f4fb755afceb5f8747172456aa606f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcaca/0.99.beta19-2.1~deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libcaca/0.99.beta19-2.1~deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcaca/0.99.beta19-2.1~deb9u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libcap2=1:2.25-1`

Binary Packages:

- `libcap2:amd64=1:2.25-1`
- `libcap2-bin=1:2.25-1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.25-1
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25-1.dsc' libcap2_2.25-1.dsc 2140 SHA256:85f73e9d273cbad49a67ceefa152df9b230c81f05c8d8dd1da0122c1574bc728
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25.orig.tar.xz' libcap2_2.25.orig.tar.xz 63672 SHA256:693c8ac51e983ee678205571ef272439d83afe62dd8e424ea14ad9790bc35162
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25-1.debian.tar.xz' libcap2_2.25-1.debian.tar.xz 20688 SHA256:0ff39428e7e531791db4450ee6dbaabf6bdc9f30e6e3be6c25bad18c333842ff
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.25-1/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.25-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.25-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcdio=0.83-4.3`

Binary Packages:

- `libcdio-cdda1:amd64=0.83-4.3+b1`
- `libcdio-paranoia1:amd64=0.83-4.3+b1`
- `libcdio13:amd64=0.83-4.3+b1`

Licenses: (parsed from: `/usr/share/doc/libcdio-cdda1/copyright`, `/usr/share/doc/libcdio-paranoia1/copyright`, `/usr/share/doc/libcdio13/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libcdio=0.83-4.3
'http://deb.debian.org/debian/pool/main/libc/libcdio/libcdio_0.83-4.3.dsc' libcdio_0.83-4.3.dsc 2416 SHA256:61d2fcc20666e630d84f730d850e73baab8a9cabe0b96de6b4dab575af98c6f5
'http://deb.debian.org/debian/pool/main/libc/libcdio/libcdio_0.83.orig.tar.gz' libcdio_0.83.orig.tar.gz 2323747 SHA256:235017e3eccb86424f9c108f2c5d5fca62630bda8c9dcf23b425ba9c5e2482c0
'http://deb.debian.org/debian/pool/main/libc/libcdio/libcdio_0.83-4.3.debian.tar.xz' libcdio_0.83-4.3.debian.tar.xz 11780 SHA256:b9a251c0b37d3ce770af7a5ac7ab316f922a688bad40f09ed2792749573f6cda
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcdio/0.83-4.3/ (for browsing the source)
- https://sources.debian.net/src/libcdio/0.83-4.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcdio/0.83-4.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcdr=0.1.3-3`

Binary Packages:

- `libcdr-0.1-1:amd64=0.1.3-3+b1`

Licenses: (parsed from: `/usr/share/doc/libcdr-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libcdr=0.1.3-3
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.3-3.dsc' libcdr_0.1.3-3.dsc 2097 SHA256:3b7a8cee554e1a6096a403ad421f29ea37f482de0f312b068124525049f85280
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.3.orig.tar.bz2' libcdr_0.1.3.orig.tar.bz2 731755 SHA256:5160bbbfefe52bd4880840fad2b07a512813e37bfaf8ccac062fca238f230f4d
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.3-3.debian.tar.xz' libcdr_0.1.3-3.debian.tar.xz 7704 SHA256:6a9c5be7bd40f2b43fae0786334d50fcce1ca1171da90304c3cf5ade7ebd6119
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcdr/0.1.3-3/ (for browsing the source)
- https://sources.debian.net/src/libcdr/0.1.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcdr/0.1.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcmis=0.5.1+git20160603-3`

Binary Packages:

- `libcmis-0.5-5v5=0.5.1+git20160603-3+b1`

Licenses: (parsed from: `/usr/share/doc/libcmis-0.5-5v5/copyright`)

- `GPL`
- `LGPL`
- `MPL | GPL2+ | LGPL2+`

Source:

```console
$ apt-get source -qq --print-uris libcmis=0.5.1+git20160603-3
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.1+git20160603-3.dsc' libcmis_0.5.1+git20160603-3.dsc 2205 SHA256:f8ec9c6ecd677cbe80e20849bb9eec6c6dd9dd05854e5595bf5ea18436a8442e
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.1+git20160603.orig.tar.bz2' libcmis_0.5.1+git20160603.orig.tar.bz2 208196 SHA256:a916526d4379ce720599164e38c904f9571924e7aedcf0654d73387b64d2ce2a
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.1+git20160603-3.debian.tar.xz' libcmis_0.5.1+git20160603-3.debian.tar.xz 4332 SHA256:cc70630e08abfe9b8f824043cb78576f4be45adaa35b911c356cfbd280c3f725
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcmis/0.5.1+git20160603-3/ (for browsing the source)
- https://sources.debian.net/src/libcmis/0.5.1+git20160603-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcmis/0.5.1+git20160603-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcroco=0.6.11-3`

Binary Packages:

- `libcroco3:amd64=0.6.11-3`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.11-3
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.11-3.dsc' libcroco_0.6.11-3.dsc 2264 SHA256:6f9a86ee343586a7e0405cbfce42e8dacfb81826aaa68372545809338f71da35
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.11.orig.tar.xz' libcroco_0.6.11.orig.tar.xz 477312 SHA256:132b528a948586b0dfa05d7e9e059901bca5a3be675b6071a90a90b81ae5a056
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.11-3.debian.tar.xz' libcroco_0.6.11-3.debian.tar.xz 7960 SHA256:dadcd41e83ccc4e22f1a6756c35009d4a75553745588d62129461522bd850b02
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcroco/0.6.11-3/ (for browsing the source)
- https://sources.debian.net/src/libcroco/0.6.11-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcroco/0.6.11-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdatrie=0.2.10-4`

Binary Packages:

- `libdatrie1:amd64=0.2.10-4+b1`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.10-4
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.10-4.dsc' libdatrie_0.2.10-4.dsc 2195 SHA256:2d80d21cfb574258e2602239c11e3df638b79334c5495430d2490763dff6b1a4
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.10.orig.tar.xz' libdatrie_0.2.10.orig.tar.xz 294380 SHA256:180eff7b0309ca19a02d5864e744185d715f021398a096fec6cf960f8ebfaa2b
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.10-4.debian.tar.xz' libdatrie_0.2.10-4.debian.tar.xz 7364 SHA256:52da724dc19ec0a27860b29b1192f2f529eeeaf27a848b75253711e9195578be
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdatrie/0.2.10-4/ (for browsing the source)
- https://sources.debian.net/src/libdatrie/0.2.10-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdatrie/0.2.10-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdc1394-22=2.2.5-1`

Binary Packages:

- `libdc1394-22:amd64=2.2.5-1`

Licenses: (parsed from: `/usr/share/doc/libdc1394-22/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libdc1394-22=2.2.5-1
'http://deb.debian.org/debian/pool/main/libd/libdc1394-22/libdc1394-22_2.2.5-1.dsc' libdc1394-22_2.2.5-1.dsc 2244 SHA256:210d37ef0e48144be2c46bb547d563ac1a67fa1ec8c893461100de8c971ad006
'http://deb.debian.org/debian/pool/main/libd/libdc1394-22/libdc1394-22_2.2.5.orig.tar.gz' libdc1394-22_2.2.5.orig.tar.gz 611918 SHA256:350cc8d08aee5ffc4e1f3049e2e1c2bc6660642d424595157da97ab5b1263337
'http://deb.debian.org/debian/pool/main/libd/libdc1394-22/libdc1394-22_2.2.5-1.debian.tar.xz' libdc1394-22_2.2.5-1.debian.tar.xz 8244 SHA256:895eeea4458059ae65a879a7d1c625508b854eb5f3d472192b94bd5ba281e316
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdc1394-22/2.2.5-1/ (for browsing the source)
- https://sources.debian.net/src/libdc1394-22/2.2.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdc1394-22/2.2.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdrm=2.4.74-1`

Binary Packages:

- `libdrm2:amd64=2.4.74-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libdrm=2.4.74-1
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.74-1.dsc' libdrm_2.4.74-1.dsc 3572 SHA256:6922553494ca71ff8ec981d0d2e4f61952053b11a9b7f9935e210ac9dbcdd260
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.74.orig.tar.gz' libdrm_2.4.74.orig.tar.gz 1056909 SHA256:3c8fdf5a89826797a8060e6f3455ca22db9ae49576cfcda1c78e3e2ce59af0f1
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.74-1.diff.gz' libdrm_2.4.74-1.diff.gz 46060 SHA256:9d5cb3ef2060a5c92f465eaf672add69c337843a6a0cad0bf15a8c9862fcd751
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdrm/2.4.74-1/ (for browsing the source)
- https://sources.debian.net/src/libdrm/2.4.74-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdrm/2.4.74-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libe-book=0.1.2-4`

Binary Packages:

- `libe-book-0.1-1:amd64=0.1.2-4`

Licenses: (parsed from: `/usr/share/doc/libe-book-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libe-book=0.1.2-4
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.2-4.dsc' libe-book_0.1.2-4.dsc 2014 SHA256:844ed48d1b29b1d01645ad49350ac698d787804c06b6962470e35e2ba2d857ad
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.2.orig.tar.bz2' libe-book_0.1.2.orig.tar.bz2 465922 SHA256:b710a57c633205b933015474d0ac0862253d1c52114d535dd09b20939a0d1850
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.2-4.debian.tar.xz' libe-book_0.1.2-4.debian.tar.xz 7148 SHA256:9041866b5d70654c156e46bfb15a1a5b9678c57c4020b3616e64e8609626da3e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libe-book/0.1.2-4/ (for browsing the source)
- https://sources.debian.net/src/libe-book/0.1.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libe-book/0.1.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libebur128=1.2.2-2`

Binary Packages:

- `libebur128-1:amd64=1.2.2-2`

Licenses: (parsed from: `/usr/share/doc/libebur128-1/copyright`)

- `BSD-3-clause`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libebur128=1.2.2-2
'http://deb.debian.org/debian/pool/main/libe/libebur128/libebur128_1.2.2-2.dsc' libebur128_1.2.2-2.dsc 2095 SHA256:bd7e5e8fb1564786a9c9a245681b00a8ee9721c7cc77721efc1a96ed6291fc02
'http://deb.debian.org/debian/pool/main/libe/libebur128/libebur128_1.2.2.orig.tar.gz' libebur128_1.2.2.orig.tar.gz 21738 SHA256:1d0d7e855da04010a2432e11fbc596502caf11b61c3b571ccbcb10095fe44b43
'http://deb.debian.org/debian/pool/main/libe/libebur128/libebur128_1.2.2-2.debian.tar.xz' libebur128_1.2.2-2.debian.tar.xz 4228 SHA256:1d8e577d8b5affea7e2b390f0f52eeba39d31d93aacac0c71a9a634c37dd5523
```

Other potentially useful URLs:

- https://sources.debian.net/src/libebur128/1.2.2-2/ (for browsing the source)
- https://sources.debian.net/src/libebur128/1.2.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libebur128/1.2.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20160903-3`

Binary Packages:

- `libedit2:amd64=3.1-20160903-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20160903-3
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20160903-3.dsc' libedit_3.1-20160903-3.dsc 2240 SHA256:d143cac52af230cce5ee3d8f181f5b496da675dd6abc1d30a14d5bbb0926a71a
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20160903.orig.tar.gz' libedit_3.1-20160903.orig.tar.gz 508108 SHA256:0ccbd2e7d46097f136fcb1aaa0d5bc24e23bb73f57d25bee5a852a683eaa7567
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20160903-3.debian.tar.bz2' libedit_3.1-20160903-3.debian.tar.bz2 11290 SHA256:6508b14c90bd756b6a5b3d3e7183b167276958e445a78ca753e460482da774f4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20160903-3/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20160903-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20160903-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libeot=0.01-4`

Binary Packages:

- `libeot0:amd64=0.01-4+b1`

Licenses: (parsed from: `/usr/share/doc/libeot0/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libeot=0.01-4
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01-4.dsc' libeot_0.01-4.dsc 1825 SHA256:358b78e5fd47acea4a6994c4ac4d541229fc88e7b8ec7d0824fe0da158892724
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01.orig.tar.bz2' libeot_0.01.orig.tar.bz2 260288 SHA256:cf5091fa8e7dcdbe667335eb90a2cfdd0a3fe8f8c7c8d1ece44d9d055736a06a
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01-4.debian.tar.xz' libeot_0.01-4.debian.tar.xz 7412 SHA256:d9e3e0abe2d2b373a90bfb1183f5f362ff137985b699a275d5c8516795c570d9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libeot/0.01-4/ (for browsing the source)
- https://sources.debian.net/src/libeot/0.01-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libeot/0.01-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libepoxy=1.3.1-2`

Binary Packages:

- `libepoxy0:amd64=1.3.1-2`

Licenses: (parsed from: `/usr/share/doc/libepoxy0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libepoxy=1.3.1-2
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.3.1-2.dsc' libepoxy_1.3.1-2.dsc 2064 SHA256:63814887cc01b183c7883964d87ba0adff06753662c9f5403f33bfd536658ba0
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.3.1.orig.tar.bz2' libepoxy_1.3.1.orig.tar.bz2 820119 SHA256:1d8668b0a259c709899e1c4bab62d756d9002d546ce4f59c9665e2fc5f001a64
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.3.1-2.debian.tar.xz' libepoxy_1.3.1-2.debian.tar.xz 16796 SHA256:67413ec6a5362ad9f0c94ff8d82f31d47daeaa39e65d576310e9194e7d5ce792
```

Other potentially useful URLs:

- https://sources.debian.net/src/libepoxy/1.3.1-2/ (for browsing the source)
- https://sources.debian.net/src/libepoxy/1.3.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libepoxy/1.3.1-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libetonyek=0.1.6-5`

Binary Packages:

- `libetonyek-0.1-1:amd64=0.1.6-5`

Licenses: (parsed from: `/usr/share/doc/libetonyek-0.1-1/copyright`)

- `MPL 2.0`

Source:

```console
$ apt-get source -qq --print-uris libetonyek=0.1.6-5
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.6-5.dsc' libetonyek_0.1.6-5.dsc 2076 SHA256:94a376d416508de0d9f1ff9ef015a9f100fa9dfc8514e6bcec64d1e1eb7a6eaa
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.6.orig.tar.bz2' libetonyek_0.1.6.orig.tar.bz2 1696455 SHA256:032f53e8d7691e48a73ddbe74fa84c906ff6ff32a33e6ee2a935b6fdb6aecb78
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.6-5.debian.tar.xz' libetonyek_0.1.6-5.debian.tar.xz 300296 SHA256:17efe39b630bfa84ea3dfd27476e6d179e00b354cbf4561996d8f0ac77c45bc7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libetonyek/0.1.6-5/ (for browsing the source)
- https://sources.debian.net/src/libetonyek/0.1.6-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libetonyek/0.1.6-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libexttextcat=3.4.4-2`

Binary Packages:

- `libexttextcat-2.0-0:amd64=3.4.4-2+b1`
- `libexttextcat-data=3.4.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libexttextcat=3.4.4-2
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.4-2.dsc' libexttextcat_3.4.4-2.dsc 2088 SHA256:5690241546ab5ce24a90542a21707135bafd73e4943d98bd36ae48b25f78d9bc
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.4.orig.tar.bz2' libexttextcat_3.4.4.orig.tar.bz2 1129140 SHA256:9595601c41051356d03d0a7d5dcad334fe1b420d221f6885d143c14bb8d62163
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.4-2.debian.tar.xz' libexttextcat_3.4.4-2.debian.tar.xz 7200 SHA256:9dacb6319d8b4612ec5bc210e742b01bdb6cb5e069ff24ca495de54ae9d1566a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libexttextcat/3.4.4-2/ (for browsing the source)
- https://sources.debian.net/src/libexttextcat/3.4.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libexttextcat/3.4.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.2.1-6`

Binary Packages:

- `libffi6:amd64=3.2.1-6`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

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

### `dpkg` source package: `libfreehand=0.1.1-2`

Binary Packages:

- `libfreehand-0.1-1=0.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libfreehand-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libfreehand=0.1.1-2
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.1-2.dsc' libfreehand_0.1.1-2.dsc 2012 SHA256:d72f018545de664298b75662cbd9e717d264ebfa014e0369fc7150af4debeb1b
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.1.orig.tar.bz2' libfreehand_0.1.1.orig.tar.bz2 597212 SHA256:45dab0e5d632eb51eeb00847972ca03835d6791149e9e714f093a9df2b445877
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.1-2.debian.tar.xz' libfreehand_0.1.1-2.debian.tar.xz 12824 SHA256:b95bf85bd479a182ee3c94d9d43881622c207ef66a04b475f9032b479b2715f9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfreehand/0.1.1-2/ (for browsing the source)
- https://sources.debian.net/src/libfreehand/0.1.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfreehand/0.1.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.7.6-2+deb9u3`

Binary Packages:

- `libgcrypt20:amd64=1.7.6-2+deb9u3`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

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

### `dpkg` source package: `libgltf=0.0.2-5`

Binary Packages:

- `libgltf-0.0-0v5:amd64=0.0.2-5`

Licenses: (parsed from: `/usr/share/doc/libgltf-0.0-0v5/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libgltf=0.0.2-5
'http://deb.debian.org/debian/pool/main/libg/libgltf/libgltf_0.0.2-5.dsc' libgltf_0.0.2-5.dsc 1859 SHA256:e655676eb1059e3f8655aa0ddc2cfea287fdafc16c79d925fa0e00fa139c9760
'http://deb.debian.org/debian/pool/main/libg/libgltf/libgltf_0.0.2.orig.tar.bz2' libgltf_0.0.2.orig.tar.bz2 538040 SHA256:d1cc7297ed1921aa969e26413b4c4e18afc882ce4d2f5a2aa2a2905706f7206b
'http://deb.debian.org/debian/pool/main/libg/libgltf/libgltf_0.0.2-5.debian.tar.xz' libgltf_0.0.2-5.debian.tar.xz 8664 SHA256:02982c318451f056ff9b1a889dd6beb404ff3f8049e416752bc570e58bc36f22
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgltf/0.0.2-5/ (for browsing the source)
- https://sources.debian.net/src/libgltf/0.0.2-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgltf/0.0.2-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libglu=9.0.0-2.1`

Binary Packages:

- `libglu1-mesa:amd64=9.0.0-2.1`

Licenses: (parsed from: `/usr/share/doc/libglu1-mesa/copyright`)

- `GPL-2`
- `LGPL-2`
- `SGI-1.1`
- `SGI-2`

Source:

```console
$ apt-get source -qq --print-uris libglu=9.0.0-2.1
'http://deb.debian.org/debian/pool/main/libg/libglu/libglu_9.0.0-2.1.dsc' libglu_9.0.0-2.1.dsc 1914 SHA256:6644a3e00d6d312fe8bbd232b6b39afbda88cc51b77bbaaf88fe8d30e0ecc47f
'http://deb.debian.org/debian/pool/main/libg/libglu/libglu_9.0.0.orig.tar.gz' libglu_9.0.0.orig.tar.gz 626786 SHA256:4387476a1933f36fec1531178ea204057bbeb04cc2d8396c9ea32720a1f7e264
'http://deb.debian.org/debian/pool/main/libg/libglu/libglu_9.0.0-2.1.diff.gz' libglu_9.0.0-2.1.diff.gz 14631 SHA256:ba605e71dd9cd007fc389b1f0f52b0b445df6d770ccd5a240d61ef7f3bb596a7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libglu/9.0.0-2.1/ (for browsing the source)
- https://sources.debian.net/src/libglu/9.0.0-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libglu/9.0.0-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.26-2`

Binary Packages:

- `libgpg-error0:amd64=1.26-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

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

### `dpkg` source package: `libgsm=1.0.13-4`

Binary Packages:

- `libgsm1:amd64=1.0.13-4+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libgsm=1.0.13-4
'http://deb.debian.org/debian/pool/main/libg/libgsm/libgsm_1.0.13-4.dsc' libgsm_1.0.13-4.dsc 1140 SHA256:807be0900ebfc0d96ffa86fed633c389f465da6db7ee57adc275b479be3ccff0
'http://deb.debian.org/debian/pool/main/libg/libgsm/libgsm_1.0.13.orig.tar.gz' libgsm_1.0.13.orig.tar.gz 65318 SHA256:52c518244d428c2e56c543b98c9135f4a76ff780c32455580b793f60a0a092ad
'http://deb.debian.org/debian/pool/main/libg/libgsm/libgsm_1.0.13-4.debian.tar.gz' libgsm_1.0.13-4.debian.tar.gz 10333 SHA256:10baf466030802440a0de1b5a11e46292a82525f922bf9e0a182f509e0bc8514
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgsm/1.0.13-4/ (for browsing the source)
- https://sources.debian.net/src/libgsm/1.0.13-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgsm/1.0.13-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libice=2:1.0.9-2`

Binary Packages:

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

Licenses: (parsed from: `/usr/share/doc/libidn11/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris libidn=1.33-1
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33-1.dsc' libidn_1.33-1.dsc 1848 SHA256:f076f7dddc45717542a48123d7dddb638beebe8521f5fba29f2d148fdcf12bf0
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33.orig.tar.gz' libidn_1.33.orig.tar.gz 3501056 SHA256:44a7aab635bb721ceef6beecc4d49dfd19478325e1b47f3196f7d2acc4930e19
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33-1.debian.tar.xz' libidn_1.33-1.debian.tar.xz 60264 SHA256:a50ee1e2598670ca1166d218e546c4cc031c658188b1193b73d98175d4405ef0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn/1.33-1/ (for browsing the source)
- https://sources.debian.net/src/libidn/1.33-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn/1.33-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libiec61883=1.2.0-2`

Binary Packages:

- `libiec61883-0:amd64=1.2.0-2`

Licenses: (parsed from: `/usr/share/doc/libiec61883-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libiec61883=1.2.0-2
'http://deb.debian.org/debian/pool/main/libi/libiec61883/libiec61883_1.2.0-2.dsc' libiec61883_1.2.0-2.dsc 1928 SHA256:1137ced1712a1e805379c97df8e06ca5287fc8f951414d9aa85ed7ef6e4a09ce
'http://deb.debian.org/debian/pool/main/libi/libiec61883/libiec61883_1.2.0.orig.tar.gz' libiec61883_1.2.0.orig.tar.gz 339064 SHA256:7c7879c6b9add3148baea697dfbfdcefffbc8ac74e8e6bcf46125ec1d21b373a
'http://deb.debian.org/debian/pool/main/libi/libiec61883/libiec61883_1.2.0-2.debian.tar.xz' libiec61883_1.2.0-2.debian.tar.xz 14708 SHA256:f913b26d2724871dbf617e5af9e6c15d5e4ab6404648b3fce810d70cf39c104f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libiec61883/1.2.0-2/ (for browsing the source)
- https://sources.debian.net/src/libiec61883/1.2.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libiec61883/1.2.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libimage-exiftool-perl=10.40-1`

Binary Packages:

- `libimage-exiftool-perl=10.40-1`

Licenses: (parsed from: `/usr/share/doc/libimage-exiftool-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libimage-exiftool-perl=10.40-1
'http://deb.debian.org/debian/pool/main/libi/libimage-exiftool-perl/libimage-exiftool-perl_10.40-1.dsc' libimage-exiftool-perl_10.40-1.dsc 2363 SHA256:909f75fc0a950634d1617f6ac3dc068ea72d3745f5e9f78df0669b438fa5e34a
'http://deb.debian.org/debian/pool/main/libi/libimage-exiftool-perl/libimage-exiftool-perl_10.40.orig.tar.gz' libimage-exiftool-perl_10.40.orig.tar.gz 4220341 SHA256:9e3619e2f9c838b37f67ab55fd541b5472b328d5f464468442367292666a05dc
'http://deb.debian.org/debian/pool/main/libi/libimage-exiftool-perl/libimage-exiftool-perl_10.40-1.debian.tar.xz' libimage-exiftool-perl_10.40-1.debian.tar.xz 6636 SHA256:8b6d15e1d9ed500a62b134e4c05777941ca15ea290116704e95dc0d8b0ff8c8f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libimage-exiftool-perl/10.40-1/ (for browsing the source)
- https://sources.debian.net/src/libimage-exiftool-perl/10.40-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libimage-exiftool-perl/10.40-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libjpeg-turbo=1:1.5.1-2`

Binary Packages:

- `libjpeg62-turbo:amd64=1:1.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libjpeg62-turbo/copyright`)

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

### `dpkg` source package: `libkate=0.4.1-7`

Binary Packages:

- `libkate1:amd64=0.4.1-7+b1`
- `liboggkate1:amd64=0.4.1-7+b1`

Licenses: (parsed from: `/usr/share/doc/libkate1/copyright`, `/usr/share/doc/liboggkate1/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libkate=0.4.1-7
'http://deb.debian.org/debian/pool/main/libk/libkate/libkate_0.4.1-7.dsc' libkate_0.4.1-7.dsc 2424 SHA256:a79d1d890ab7753e9d70f81ba7b748c08b0ed23fbc818d66f002f02120b98762
'http://deb.debian.org/debian/pool/main/libk/libkate/libkate_0.4.1.orig.tar.gz' libkate_0.4.1.orig.tar.gz 906896 SHA256:c40e81d5866c3d4bf744e76ce0068d8f388f0e25f7e258ce0c8e76d7adc87b68
'http://deb.debian.org/debian/pool/main/libk/libkate/libkate_0.4.1-7.debian.tar.xz' libkate_0.4.1-7.debian.tar.xz 7608 SHA256:a5525dfbaf0b9f83202f86162a5d1430fb6dfd4eea0474a6bca4722058484b2b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libkate/0.4.1-7/ (for browsing the source)
- https://sources.debian.net/src/libkate/0.4.1-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libkate/0.4.1-7/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `liblangtag=0.6.2-1`

Binary Packages:

- `liblangtag-common=0.6.2-1`
- `liblangtag1:amd64=0.6.2-1`

Licenses: (parsed from: `/usr/share/doc/liblangtag-common/copyright`, `/usr/share/doc/liblangtag1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL | MPL`

Source:

```console
$ apt-get source -qq --print-uris liblangtag=0.6.2-1
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.6.2-1.dsc' liblangtag_0.6.2-1.dsc 2370 SHA256:a0909825917c4ead4be851f4885ddfe501af65cadda1add6b45facd2af4ff6c4
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.6.2.orig.tar.bz2' liblangtag_0.6.2.orig.tar.bz2 766080 SHA256:d6242790324f1432fb0a6fae71b6851f520b2c5a87675497cf8ea14c2924d52e
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.6.2-1.debian.tar.xz' liblangtag_0.6.2-1.debian.tar.xz 6072 SHA256:003688ddf23bdbfcc27816ea7e9714f58930ca26d36d1685f06d28760fbff81a
```

Other potentially useful URLs:

- https://sources.debian.net/src/liblangtag/0.6.2-1/ (for browsing the source)
- https://sources.debian.net/src/liblangtag/0.6.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liblangtag/0.6.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liblqr=0.4.2-2`

Binary Packages:

- `liblqr-1-0:amd64=0.4.2-2+b2`

Licenses: (parsed from: `/usr/share/doc/liblqr-1-0/copyright`)

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

### `dpkg` source package: `libmnl=1.0.4-2`

Binary Packages:

- `libmnl0:amd64=1.0.4-2`

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

### `dpkg` source package: `libmspub=0.1.2-4`

Binary Packages:

- `libmspub-0.1-1:amd64=0.1.2-4+b1`

Licenses: (parsed from: `/usr/share/doc/libmspub-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libmspub=0.1.2-4
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.2-4.dsc' libmspub_0.1.2-4.dsc 2094 SHA256:a756c8ea383ab930535b9a3c4ed6dafa6abff5e4666d6093b891851b8ea45cd5
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.2.orig.tar.bz2' libmspub_0.1.2.orig.tar.bz2 429360 SHA256:26d488527ffbb0b41686d4bab756e3e6aaeb99f88adeb169d0c16d2cde96859a
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.2-4.debian.tar.xz' libmspub_0.1.2-4.debian.tar.xz 7132 SHA256:b31e8367c15e466a3cc97efa2f09d4953ddafbd0794754f7bbeec5447bccd963
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmspub/0.1.2-4/ (for browsing the source)
- https://sources.debian.net/src/libmspub/0.1.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmspub/0.1.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmwaw=0.3.9-2`

Binary Packages:

- `libmwaw-0.3-3:amd64=0.3.9-2`

Licenses: (parsed from: `/usr/share/doc/libmwaw-0.3-3/copyright`)

- `BSD`
- `LGPL`
- `MPL2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmwaw=0.3.9-2
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.9-2.dsc' libmwaw_0.3.9-2.dsc 2068 SHA256:2a7768051a60c31ffd71ef4c0424e93beda7a303e7a179556b686ec4d98ca5f7
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.9.orig.tar.bz2' libmwaw_0.3.9.orig.tar.bz2 1463662 SHA256:11a1f318431a052e1d623385351c8e659377d36db3e71e188af55da87ce9461f
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.9-2.debian.tar.xz' libmwaw_0.3.9-2.debian.tar.xz 8300 SHA256:7a8b398acf11115a6e08576afd97ac49ac201f4367584e51059e49c9d735349c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmwaw/0.3.9-2/ (for browsing the source)
- https://sources.debian.net/src/libmwaw/0.3.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmwaw/0.3.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libnih=1.0.3-8`

Binary Packages:

- `libnih-dbus1=1.0.3-8`
- `libnih1=1.0.3-8`

Licenses: (parsed from: `/usr/share/doc/libnih-dbus1/copyright`, `/usr/share/doc/libnih1/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libnih=1.0.3-8
'http://deb.debian.org/debian/pool/main/libn/libnih/libnih_1.0.3-8.dsc' libnih_1.0.3-8.dsc 2158 SHA256:81387e3d760780e77e49835815e9881a265702bc3f3373ff19ff07708064c117
'http://deb.debian.org/debian/pool/main/libn/libnih/libnih_1.0.3.orig.tar.gz' libnih_1.0.3.orig.tar.gz 1187624 SHA256:897572df7565c0a90a81532671e23c63f99b4efde2eecbbf11e7857fbc61f405
'http://deb.debian.org/debian/pool/main/libn/libnih/libnih_1.0.3-8.debian.tar.xz' libnih_1.0.3-8.debian.tar.xz 8944 SHA256:ab65944ae17f8f128e021d8a245f17c1d2b0f75210c64443e99dfef7c32ee207
```

Other potentially useful URLs:

- https://sources.debian.net/src/libnih/1.0.3-8/ (for browsing the source)
- https://sources.debian.net/src/libnih/1.0.3-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libnih/1.0.3-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libodfgen=0.1.6-2`

Binary Packages:

- `libodfgen-0.1-1:amd64=0.1.6-2`

Licenses: (parsed from: `/usr/share/doc/libodfgen-0.1-1/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libodfgen=0.1.6-2
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.6-2.dsc' libodfgen_0.1.6-2.dsc 1925 SHA256:e63c30d5461b53a11fdc83e3dd585735273e94b80812e5e2627d6e96eaf5e838
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.6.orig.tar.bz2' libodfgen_0.1.6.orig.tar.bz2 446705 SHA256:2c7b21892f84a4c67546f84611eccdad6259875c971e98ddb027da66ea0ac9c2
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.6-2.debian.tar.xz' libodfgen_0.1.6-2.debian.tar.xz 6868 SHA256:97ee71689bd24694abfee2c7b736ebeb45aa2cd215a338edd8183342a9ecea8f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libodfgen/0.1.6-2/ (for browsing the source)
- https://sources.debian.net/src/libodfgen/0.1.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libodfgen/0.1.6-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libopenmpt=0.2.7386~beta20.3-3+deb9u3`

Binary Packages:

- `libopenmpt0:amd64=0.2.7386~beta20.3-3+deb9u3`

Licenses: (parsed from: `/usr/share/doc/libopenmpt0/copyright`)

- `BSD-3-clause`
- `GNU-All-Permissive-License`
- `GNU-All-Permissive-License-FSF`
- `GPL-2`
- `GPL-3`
- `GPL2+-libtool`
- `GPL2+-with-Autoconf-exception`
- `GPL3+-with-Autoconf-Macros-exception`
- `GPL3+-with-Autoconf-exception`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris libopenmpt=0.2.7386~beta20.3-3+deb9u3
'http://deb.debian.org/debian/pool/main/libo/libopenmpt/libopenmpt_0.2.7386~beta20.3-3+deb9u3.dsc' libopenmpt_0.2.7386~beta20.3-3+deb9u3.dsc 2721 SHA256:cd48ba2b9e319687195402e7579b520507941589ac056cce8ebab37c81db93d1
'http://deb.debian.org/debian/pool/main/libo/libopenmpt/libopenmpt_0.2.7386~beta20.3.orig.tar.gz' libopenmpt_0.2.7386~beta20.3.orig.tar.gz 1267363 SHA256:a6a7e6da1ae66e1cf46985ee92c182e50652d71b96135e9fa6048e132d844753
'http://deb.debian.org/debian/pool/main/libo/libopenmpt/libopenmpt_0.2.7386~beta20.3-3+deb9u3.debian.tar.xz' libopenmpt_0.2.7386~beta20.3-3+deb9u3.debian.tar.xz 15604 SHA256:288a50918943329406f9d605f8f479e7ca102d9bc6a7e1be88ff0fbab6b38630
```

Other potentially useful URLs:

- https://sources.debian.net/src/libopenmpt/0.2.7386~beta20.3-3+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/libopenmpt/0.2.7386~beta20.3-3+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libopenmpt/0.2.7386~beta20.3-3+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liborcus=0.11.2-3`

Binary Packages:

- `liborcus-0.11-0:amd64=0.11.2-3+b1`

Licenses: (parsed from: `/usr/share/doc/liborcus-0.11-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3+`
- `MIT`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris liborcus=0.11.2-3
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.11.2-3.dsc' liborcus_0.11.2-3.dsc 2249 SHA256:54f3a72f2adb4d2bdfbc6007d09fb0e56cfb586f2a757d77a8fbb52e2df99985
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.11.2.orig.tar.xz' liborcus_0.11.2.orig.tar.xz 1376164 SHA256:1a182cf44c7f100aea38ce71355c4a58583b5dd44441b70bb7691f14c2f77d75
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.11.2-3.debian.tar.xz' liborcus_0.11.2-3.debian.tar.xz 10164 SHA256:4b73fde1a691fc3df4dc0e92cb8d783ea7b8143d6b42253e223cf65f7058c01a
```

Other potentially useful URLs:

- https://sources.debian.net/src/liborcus/0.11.2-3/ (for browsing the source)
- https://sources.debian.net/src/liborcus/0.11.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liborcus/0.11.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpagemaker=0.0.3-2`

Binary Packages:

- `libpagemaker-0.0-0:amd64=0.0.3-2`

Licenses: (parsed from: `/usr/share/doc/libpagemaker-0.0-0/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libpagemaker=0.0.3-2
'http://deb.debian.org/debian/pool/main/libp/libpagemaker/libpagemaker_0.0.3-2.dsc' libpagemaker_0.0.3-2.dsc 1997 SHA256:0b074335869109d0ac5139a63eac573e6711022fc4be01c4c050496399c7be94
'http://deb.debian.org/debian/pool/main/libp/libpagemaker/libpagemaker_0.0.3.orig.tar.bz2' libpagemaker_0.0.3.orig.tar.bz2 376953 SHA256:3b5de037692f8e156777a75e162f6b110fa24c01749e4a66d7eb83f364e52a33
'http://deb.debian.org/debian/pool/main/libp/libpagemaker/libpagemaker_0.0.3-2.debian.tar.xz' libpagemaker_0.0.3-2.debian.tar.xz 6628 SHA256:107f39699dc6dad778ae970f1d496d614b9466437755c929403bb5f930b2e50e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpagemaker/0.0.3-2/ (for browsing the source)
- https://sources.debian.net/src/libpagemaker/0.0.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpagemaker/0.0.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpaper=1.1.24+nmu5`

Binary Packages:

- `libpaper1:amd64=1.1.24+nmu5`

Licenses: (parsed from: `/usr/share/doc/libpaper1/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpaper=1.1.24+nmu5
'http://deb.debian.org/debian/pool/main/libp/libpaper/libpaper_1.1.24+nmu5.dsc' libpaper_1.1.24+nmu5.dsc 1597 SHA256:50edeb41f092954a636fb64bbd1cf27ca80b47a9600dcc9392c4df9b15059582
'http://deb.debian.org/debian/pool/main/libp/libpaper/libpaper_1.1.24+nmu5.tar.gz' libpaper_1.1.24+nmu5.tar.gz 49032 SHA256:e29deda4cd7350189c71af0925cbf4a4473f9841d1419a922e1e8ff1954db1f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpaper/1.1.24+nmu5/ (for browsing the source)
- https://sources.debian.net/src/libpaper/1.1.24+nmu5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpaper/1.1.24+nmu5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpgm=5.2.122~dfsg-2`

Binary Packages:

- `libpgm-5.2-0:amd64=5.2.122~dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libpgm-5.2-0/copyright`)

- `BSD-3-clause`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libpgm=5.2.122~dfsg-2
'http://deb.debian.org/debian/pool/main/libp/libpgm/libpgm_5.2.122~dfsg-2.dsc' libpgm_5.2.122~dfsg-2.dsc 1870 SHA256:2d6eb667fd66046c4c35215068cfa562decd8d0838ec864a35796cdad354fc49
'http://deb.debian.org/debian/pool/main/libp/libpgm/libpgm_5.2.122~dfsg.orig.tar.xz' libpgm_5.2.122~dfsg.orig.tar.xz 550996 SHA256:d6e5ec0918216d4e9b14459f5742f6f8416df965f03ac4d854bd5d111709b507
'http://deb.debian.org/debian/pool/main/libp/libpgm/libpgm_5.2.122~dfsg-2.debian.tar.xz' libpgm_5.2.122~dfsg-2.debian.tar.xz 6568 SHA256:5f02e1055a199f545d99f4f709330abe5e31c7073a3cb2ed737a4fbb5b7d2857
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpgm/5.2.122~dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/libpgm/5.2.122~dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpgm/5.2.122~dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng1.6=1.6.28-1+deb9u1`

Binary Packages:

- `libpng16-16:amd64=1.6.28-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libpng16-16/copyright`)

- `BSD-like-with-advertising-clause`
- `GPL-2`
- `GPL-2+`
- `expat`
- `libpng`

Source:

```console
$ apt-get source -qq --print-uris libpng1.6=1.6.28-1+deb9u1
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.28-1+deb9u1.dsc' libpng1.6_1.6.28-1+deb9u1.dsc 2403 SHA256:e33f21a69c0406eaee4ca7157c7234c3a078bab83f57c399cd2ddc8d7c868ddf
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.28.orig.tar.xz' libpng1.6_1.6.28.orig.tar.xz 984536 SHA256:d8d3ec9de6b5db740fefac702c37ffcf96ae46cb17c18c1544635a3852f78f7a
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.28-1+deb9u1.debian.tar.xz' libpng1.6_1.6.28-1+deb9u1.debian.tar.xz 22844 SHA256:c082fb471028f37bfb9510057f7d4854e1200b5115d2c308da9c2837375585e9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpng1.6/1.6.28-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libpng1.6/1.6.28-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpng1.6/1.6.28-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libproxy=0.4.14-2`

Binary Packages:

- `libproxy1v5:amd64=0.4.14-2`

Licenses: (parsed from: `/usr/share/doc/libproxy1v5/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libproxy=0.4.14-2
'http://deb.debian.org/debian/pool/main/libp/libproxy/libproxy_0.4.14-2.dsc' libproxy_0.4.14-2.dsc 3123 SHA256:18143cde4c1f0e74fdb9c17a0bc5f60dbf05c7530fc3780a865309206940514b
'http://deb.debian.org/debian/pool/main/libp/libproxy/libproxy_0.4.14.orig.tar.gz' libproxy_0.4.14.orig.tar.gz 92783 SHA256:6220a6cab837a8996116a0568324cadfd09a07ec16b930d2a330e16d5c2e1eb6
'http://deb.debian.org/debian/pool/main/libp/libproxy/libproxy_0.4.14-2.debian.tar.xz' libproxy_0.4.14-2.debian.tar.xz 10340 SHA256:b84c8096cef89325c107293ec0af9d63c0f1ac1437fe0dce7ec1767fb0df59f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libproxy/0.4.14-2/ (for browsing the source)
- https://sources.debian.net/src/libproxy/0.4.14-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libproxy/0.4.14-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libraw1394=2.1.2-1`

Binary Packages:

- `libraw1394-11:amd64=2.1.2-1+b1`

Licenses: (parsed from: `/usr/share/doc/libraw1394-11/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libraw1394=2.1.2-1
'http://deb.debian.org/debian/pool/main/libr/libraw1394/libraw1394_2.1.2-1.dsc' libraw1394_2.1.2-1.dsc 2080 SHA256:d8b7cb13f4a73fa0dae8d61d5b4ded82b3f02d6b3584ac77c671432d250988f4
'http://deb.debian.org/debian/pool/main/libr/libraw1394/libraw1394_2.1.2.orig.tar.gz' libraw1394_2.1.2.orig.tar.gz 458134 SHA256:ddc4e32721cdfe680d964aaede68ac606a20cd17dd2ba70e2d7e0692086ab57c
'http://deb.debian.org/debian/pool/main/libr/libraw1394/libraw1394_2.1.2-1.debian.tar.xz' libraw1394_2.1.2-1.debian.tar.xz 8760 SHA256:5cee0e0049d820a8e4e5d3dbd94fb2c3d7b782ec09134c6c714ed523829dc1c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libraw1394/2.1.2-1/ (for browsing the source)
- https://sources.debian.net/src/libraw1394/2.1.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libraw1394/2.1.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libreoffice=1:5.2.7-1+deb9u11`

Binary Packages:

- `fonts-opensymbol=2:102.7+LibO5.2.7-1+deb9u11`
- `libreoffice=1:5.2.7-1+deb9u11`
- `libreoffice-avmedia-backend-gstreamer=1:5.2.7-1+deb9u11`
- `libreoffice-base=1:5.2.7-1+deb9u11`
- `libreoffice-base-core=1:5.2.7-1+deb9u11`
- `libreoffice-base-drivers=1:5.2.7-1+deb9u11`
- `libreoffice-calc=1:5.2.7-1+deb9u11`
- `libreoffice-common=1:5.2.7-1+deb9u11`
- `libreoffice-core=1:5.2.7-1+deb9u11`
- `libreoffice-draw=1:5.2.7-1+deb9u11`
- `libreoffice-impress=1:5.2.7-1+deb9u11`
- `libreoffice-java-common=1:5.2.7-1+deb9u11`
- `libreoffice-math=1:5.2.7-1+deb9u11`
- `libreoffice-report-builder-bin=1:5.2.7-1+deb9u11`
- `libreoffice-style-galaxy=1:5.2.7-1+deb9u11`
- `libreoffice-writer=1:5.2.7-1+deb9u11`
- `python3-uno=1:5.2.7-1+deb9u11`
- `uno-libs3=5.2.7-1+deb9u11`
- `ure=5.2.7-1+deb9u11`

Licenses: (parsed from: `/usr/share/doc/fonts-opensymbol/copyright`, `/usr/share/doc/libreoffice/copyright`, `/usr/share/doc/libreoffice-avmedia-backend-gstreamer/copyright`, `/usr/share/doc/libreoffice-base/copyright`, `/usr/share/doc/libreoffice-base-core/copyright`, `/usr/share/doc/libreoffice-base-drivers/copyright`, `/usr/share/doc/libreoffice-calc/copyright`, `/usr/share/doc/libreoffice-common/copyright`, `/usr/share/doc/libreoffice-core/copyright`, `/usr/share/doc/libreoffice-draw/copyright`, `/usr/share/doc/libreoffice-impress/copyright`, `/usr/share/doc/libreoffice-java-common/copyright`, `/usr/share/doc/libreoffice-math/copyright`, `/usr/share/doc/libreoffice-report-builder-bin/copyright`, `/usr/share/doc/libreoffice-style-galaxy/copyright`, `/usr/share/doc/libreoffice-writer/copyright`, `/usr/share/doc/python3-uno/copyright`, `/usr/share/doc/uno-libs3/copyright`, `/usr/share/doc/ure/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `MPL-1.1 | GPL-2 | LGPL-2`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libreoffice=1:5.2.7-1+deb9u11
'http://security.debian.org/debian-security/pool/updates/main/libr/libreoffice/libreoffice_5.2.7-1+deb9u11.dsc' libreoffice_5.2.7-1+deb9u11.dsc 28373 SHA256:16a2fb515814ffcecd453aaadb0e1a9fd289621220fb4bb6c92469eb3b3035ea
'http://security.debian.org/debian-security/pool/updates/main/libr/libreoffice/libreoffice_5.2.7.orig-helpcontent2.tar.xz' libreoffice_5.2.7.orig-helpcontent2.tar.xz 1446232 SHA256:a25de3b0fc788d1246ecb160718097e8f882b559d4a6536e1521fb0548d1b33a
'http://security.debian.org/debian-security/pool/updates/main/libr/libreoffice/libreoffice_5.2.7.orig-translations.tar.xz' libreoffice_5.2.7.orig-translations.tar.xz 141705808 SHA256:df52c5491e438ac2f33e3c5ee8bb78cb0e0b530bf1a925a360ceba3c1775b867
'http://security.debian.org/debian-security/pool/updates/main/libr/libreoffice/libreoffice_5.2.7.orig.tar.xz' libreoffice_5.2.7.orig.tar.xz 184589464 SHA256:106154a72a329605166a49bfa31c6d1cc03133d600ad0ef340b45e4e2a92891d
'http://security.debian.org/debian-security/pool/updates/main/libr/libreoffice/libreoffice_5.2.7.orig.tar.xz.asc' libreoffice_5.2.7.orig.tar.xz.asc 836 SHA256:317b474e90b32fee6e3b189fe29b2cb6eba3634fada977b05b837ba6318baa52
'http://security.debian.org/debian-security/pool/updates/main/libr/libreoffice/libreoffice_5.2.7-1+deb9u11.debian.tar.xz' libreoffice_5.2.7-1+deb9u11.debian.tar.xz 5405056 SHA256:77911a7554604d748c1cf2066510bd97a7571e3ab3e6337dbd0884e003f9a173
```

Other potentially useful URLs:

- https://sources.debian.net/src/libreoffice/1:5.2.7-1+deb9u11/ (for browsing the source)
- https://sources.debian.net/src/libreoffice/1:5.2.7-1+deb9u11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libreoffice/1:5.2.7-1+deb9u11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `librest=0.8.0-2`

Binary Packages:

- `librest-0.7-0:amd64=0.8.0-2`

Licenses: (parsed from: `/usr/share/doc/librest-0.7-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris librest=0.8.0-2
'http://deb.debian.org/debian/pool/main/libr/librest/librest_0.8.0-2.dsc' librest_0.8.0-2.dsc 2455 SHA256:5b07238bde6883684aad271a518b0924dd05d36c7581d56a0e57c1ed8b56b6f6
'http://deb.debian.org/debian/pool/main/libr/librest/librest_0.8.0.orig.tar.xz' librest_0.8.0.orig.tar.xz 334024 SHA256:e7b89b200c1417073aef739e8a27ff2ab578056c27796ec74f5886a5e0dff647
'http://deb.debian.org/debian/pool/main/libr/librest/librest_0.8.0-2.debian.tar.xz' librest_0.8.0-2.debian.tar.xz 6536 SHA256:233b15b5c4b36fa6b2ac026305fd5db043e4de22a14f947d304956adba640827
```

Other potentially useful URLs:

- https://sources.debian.net/src/librest/0.8.0-2/ (for browsing the source)
- https://sources.debian.net/src/librest/0.8.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librest/0.8.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `librevenge=0.0.4-6`

Binary Packages:

- `librevenge-0.0-0:amd64=0.0.4-6`

Licenses: (parsed from: `/usr/share/doc/librevenge-0.0-0/copyright`)

- `LGPL-2.1`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris librevenge=0.0.4-6
'http://deb.debian.org/debian/pool/main/libr/librevenge/librevenge_0.0.4-6.dsc' librevenge_0.0.4-6.dsc 2001 SHA256:50d81189825c40607677288d3a3c6d39645d94d966a3894008671c85b6ad159a
'http://deb.debian.org/debian/pool/main/libr/librevenge/librevenge_0.0.4.orig.tar.bz2' librevenge_0.0.4.orig.tar.bz2 529833 SHA256:c51601cd08320b75702812c64aae0653409164da7825fd0f451ac2c5dbe77cbf
'http://deb.debian.org/debian/pool/main/libr/librevenge/librevenge_0.0.4-6.debian.tar.xz' librevenge_0.0.4-6.debian.tar.xz 13456 SHA256:ab71bf043ba34f897f7367a548fe7e06505b22e5e37502a0d49ff7d8f46a69fd
```

Other potentially useful URLs:

- https://sources.debian.net/src/librevenge/0.0.4-6/ (for browsing the source)
- https://sources.debian.net/src/librevenge/0.0.4-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librevenge/0.0.4-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `librsvg=2.40.16-1`

Binary Packages:

- `librsvg2-2:amd64=2.40.16-1+b1`
- `librsvg2-common:amd64=2.40.16-1+b1`

Licenses: (parsed from: `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.40.16-1
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.40.16-1.dsc' librsvg_2.40.16-1.dsc 2738 SHA256:d5447c5867087a53dad2ec237d21f581c22a689d8fa1e2509903c0eef9e2b398
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.40.16.orig.tar.xz' librsvg_2.40.16.orig.tar.xz 560800 SHA256:d48bcf6b03fa98f07df10332fb49d8c010786ddca6ab34cbba217684f533ff2e
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.40.16-1.debian.tar.xz' librsvg_2.40.16-1.debian.tar.xz 14296 SHA256:4618fae8afecef179c5cf5cfb7d1ca9719a7c8821457cf706656a864fcaae079
```

Other potentially useful URLs:

- https://sources.debian.net/src/librsvg/2.40.16-1/ (for browsing the source)
- https://sources.debian.net/src/librsvg/2.40.16-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librsvg/2.40.16-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsamplerate=0.1.8-8`

Binary Packages:

- `libsamplerate0:amd64=0.1.8-8+b2`

Licenses: (parsed from: `/usr/share/doc/libsamplerate0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libsamplerate=0.1.8-8
'http://deb.debian.org/debian/pool/main/libs/libsamplerate/libsamplerate_0.1.8-8.dsc' libsamplerate_0.1.8-8.dsc 1940 SHA256:f13b419b19e18d7023b577382f7d2e65a6554b30793fde197338c7982c515660
'http://deb.debian.org/debian/pool/main/libs/libsamplerate/libsamplerate_0.1.8.orig.tar.gz' libsamplerate_0.1.8.orig.tar.gz 4303330 SHA256:93b54bdf46d5e6d2354b7034395fe329c222a966790de34520702bb9642f1c06
'http://deb.debian.org/debian/pool/main/libs/libsamplerate/libsamplerate_0.1.8-8.debian.tar.xz' libsamplerate_0.1.8-8.debian.tar.xz 5836 SHA256:d41c73e86687265491780fe507178513b320325108b026bb9d8f6672287c2225
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsamplerate/0.1.8-8/ (for browsing the source)
- https://sources.debian.net/src/libsamplerate/0.1.8-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsamplerate/0.1.8-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsdl2=2.0.5+dfsg1-2`

Binary Packages:

- `libsdl2-2.0-0:amd64=2.0.5+dfsg1-2`

Licenses: (parsed from: `/usr/share/doc/libsdl2-2.0-0/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-chromium`
- `BrownUn_UnCalifornia_ErikCorry`
- `Expat-like`
- `Gareth_McCaughan`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT/X11`
- `PublicDomain_David_Ludwig`
- `PublicDomain_Edgar_Simo`
- `PublicDomain_Sam_Lantinga`
- `RSA_Data_Security`
- `SGI-Free-Software-License-B`
- `SunPro`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris libsdl2=2.0.5+dfsg1-2
'http://deb.debian.org/debian/pool/main/libs/libsdl2/libsdl2_2.0.5+dfsg1-2.dsc' libsdl2_2.0.5+dfsg1-2.dsc 2685 SHA256:898b6f9265c3a953cce3bb935329720770ecc3736086fc6436bf320e6c18d0de
'http://deb.debian.org/debian/pool/main/libs/libsdl2/libsdl2_2.0.5+dfsg1.orig.tar.xz' libsdl2_2.0.5+dfsg1.orig.tar.xz 1668828 SHA256:73b893f95eca1f5704a3a17d5440c342b4f12609b47ba661f9169b97e84c08da
'http://deb.debian.org/debian/pool/main/libs/libsdl2/libsdl2_2.0.5+dfsg1-2.debian.tar.xz' libsdl2_2.0.5+dfsg1-2.debian.tar.xz 14680 SHA256:b9ad45b421c1cbeaedb9138403f95e8639cdf691e83dbb0884f84897d7d3567a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsdl2/2.0.5+dfsg1-2/ (for browsing the source)
- https://sources.debian.net/src/libsdl2/2.0.5+dfsg1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsdl2/2.0.5+dfsg1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.3.1-2.1+deb9u1`

Binary Packages:

- `libseccomp2:amd64=2.3.1-2.1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.3.1-2.1+deb9u1
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.1-2.1+deb9u1.dsc' libseccomp_2.3.1-2.1+deb9u1.dsc 2108 SHA256:2496d6f5726512b1d85a7b0920f258be254b7ca41d61b48edee75e603f2a4731
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.1.orig.tar.gz' libseccomp_2.3.1.orig.tar.gz 552299 SHA256:ff5bdd2168790f1979e24eaa498f8606c2f2d96f08a8dc4006a2e88affa4562b
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.1-2.1+deb9u1.debian.tar.xz' libseccomp_2.3.1-2.1+deb9u1.debian.tar.xz 13532 SHA256:d00fed62c387f3ee525b370325ceac962cfcee8dcfebc5f3ca4b2af0602cc0ff
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.3.1-2.1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.3.1-2.1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.3.1-2.1+deb9u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libsm=2:1.2.2-1`

Binary Packages:

- `libsm6:amd64=2:1.2.2-1+b3`

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

### `dpkg` source package: `libsndfile=1.0.27-3`

Binary Packages:

- `libsndfile1:amd64=1.0.27-3`

Licenses: (parsed from: `/usr/share/doc/libsndfile1/copyright`)

- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libsndfile=1.0.27-3
'http://deb.debian.org/debian/pool/main/libs/libsndfile/libsndfile_1.0.27-3.dsc' libsndfile_1.0.27-3.dsc 2325 SHA256:2aad1627be9e40b1d46351cf66e8be1c98c9c0c997a4e29560d7bb17b47700e5
'http://deb.debian.org/debian/pool/main/libs/libsndfile/libsndfile_1.0.27.orig.tar.gz' libsndfile_1.0.27.orig.tar.gz 1192337 SHA256:a391952f27f4a92ceb2b4c06493ac107896ed6c76be9a613a4731f076d30fac0
'http://deb.debian.org/debian/pool/main/libs/libsndfile/libsndfile_1.0.27-3.debian.tar.xz' libsndfile_1.0.27-3.debian.tar.xz 14944 SHA256:f0dfb219d920423161d3ecbe5c576cbc7fe0a8169335b9efcad4528ca7e8e463
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsndfile/1.0.27-3/ (for browsing the source)
- https://sources.debian.net/src/libsndfile/1.0.27-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsndfile/1.0.27-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsodium=1.0.11-2`

Binary Packages:

- `libsodium18:amd64=1.0.11-2`

Licenses: (parsed from: `/usr/share/doc/libsodium18/copyright`)

- `BSD-2-clause`
- `CC0`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libsodium=1.0.11-2
'http://deb.debian.org/debian/pool/main/libs/libsodium/libsodium_1.0.11-2.dsc' libsodium_1.0.11-2.dsc 1981 SHA256:c27e29c0d33b4b541ec209263f8537a74b435e43250970ce4baaa3a043340fac
'http://deb.debian.org/debian/pool/main/libs/libsodium/libsodium_1.0.11.orig.tar.gz' libsodium_1.0.11.orig.tar.gz 1445598 SHA256:7ad3340938af851186318b09fe977e1bd48acc3f21068f3961afa42ed37a3a65
'http://deb.debian.org/debian/pool/main/libs/libsodium/libsodium_1.0.11-2.debian.tar.xz' libsodium_1.0.11-2.debian.tar.xz 6120 SHA256:36802b06c9b10b9bf413124418c1d5cbbfa9f35ee9d20641d9c4f8897d37d573
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsodium/1.0.11-2/ (for browsing the source)
- https://sources.debian.net/src/libsodium/1.0.11-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsodium/1.0.11-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsoup2.4=2.56.0-2+deb9u2`

Binary Packages:

- `libsoup-gnome2.4-1:amd64=2.56.0-2+deb9u2`
- `libsoup2.4-1:amd64=2.56.0-2+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libsoup-gnome2.4-1/copyright`, `/usr/share/doc/libsoup2.4-1/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libsoup2.4=2.56.0-2+deb9u2
'http://deb.debian.org/debian/pool/main/libs/libsoup2.4/libsoup2.4_2.56.0-2+deb9u2.dsc' libsoup2.4_2.56.0-2+deb9u2.dsc 2725 SHA256:3b533fd4d3c5f362edf745de8758706421f1faf8dcd3bb9e64deb1cc8def5b22
'http://deb.debian.org/debian/pool/main/libs/libsoup2.4/libsoup2.4_2.56.0.orig.tar.xz' libsoup2.4_2.56.0.orig.tar.xz 1821412 SHA256:d8216b71de8247bc6f274ec054c08547b2e04369c1f8add713e9350c8ef81fe5
'http://deb.debian.org/debian/pool/main/libs/libsoup2.4/libsoup2.4_2.56.0-2+deb9u2.debian.tar.xz' libsoup2.4_2.56.0-2+deb9u2.debian.tar.xz 20520 SHA256:070772b8fde95c2fa194187b19f4eba76bfabae2aa2e0d4d4a33d8bf8537a9c2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsoup2.4/2.56.0-2+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/libsoup2.4/2.56.0-2+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsoup2.4/2.56.0-2+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsoxr=0.1.2-2`

Binary Packages:

- `libsoxr0:amd64=0.1.2-2`

Licenses: (parsed from: `/usr/share/doc/libsoxr0/copyright`)

- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Spherepack`
- `permissive1`
- `permissive2`

Source:

```console
$ apt-get source -qq --print-uris libsoxr=0.1.2-2
'http://deb.debian.org/debian/pool/main/libs/libsoxr/libsoxr_0.1.2-2.dsc' libsoxr_0.1.2-2.dsc 2138 SHA256:34f7c82934389b39061fd7ad0efc0d0428458a9824677cea18a2b13879234eca
'http://deb.debian.org/debian/pool/main/libs/libsoxr/libsoxr_0.1.2.orig.tar.xz' libsoxr_0.1.2.orig.tar.xz 83760 SHA256:54e6f434f1c491388cd92f0e3c47f1ade082cc24327bdc43762f7d1eefe0c275
'http://deb.debian.org/debian/pool/main/libs/libsoxr/libsoxr_0.1.2-2.debian.tar.xz' libsoxr_0.1.2-2.debian.tar.xz 4608 SHA256:1f0ec46d44770f2de9d00fd2ec11a4e0b9d97c6168549b86f74cbce80aae9b49
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsoxr/0.1.2-2/ (for browsing the source)
- https://sources.debian.net/src/libsoxr/0.1.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsoxr/0.1.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libssh=0.7.3-2+deb9u2`

Binary Packages:

- `libssh-gcrypt-4:amd64=0.7.3-2+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libssh-gcrypt-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.7.3-2+deb9u2
'http://deb.debian.org/debian/pool/main/libs/libssh/libssh_0.7.3-2+deb9u2.dsc' libssh_0.7.3-2+deb9u2.dsc 2463 SHA256:3f145b85528f349028ffbb1b9755f117a3072e74513de13b107f6d3e47f637f4
'http://deb.debian.org/debian/pool/main/libs/libssh/libssh_0.7.3.orig.tar.xz' libssh_0.7.3.orig.tar.xz 350464 SHA256:26ef46be555da21112c01e4b9f5e3abba9194485c8822ab55ba3d6496222af98
'http://deb.debian.org/debian/pool/main/libs/libssh/libssh_0.7.3-2+deb9u2.debian.tar.xz' libssh_0.7.3-2+deb9u2.debian.tar.xz 25428 SHA256:80d2164b969415b9c81adee7195799f87c32bc35454049f255cfc0e055e7b2c9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh/0.7.3-2+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/libssh/0.7.3-2+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh/0.7.3-2+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.10-1.1+deb9u1`

Binary Packages:

- `libtasn1-6:amd64=4.10-1.1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

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

### `dpkg` source package: `libthai=0.1.26-1`

Binary Packages:

- `libthai-data=0.1.26-1`
- `libthai0:amd64=0.1.26-1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.26-1
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.26-1.dsc' libthai_0.1.26-1.dsc 2352 SHA256:a26a4478c773418a19dcd7acd6d82202b29636b6f712cf3bc17b98850ff3afa2
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.26.orig.tar.xz' libthai_0.1.26.orig.tar.xz 409380 SHA256:8710112c836b272db1740a9ea3e6c7ebb65b64eee0e143fc2b2c60f99f6bfe2a
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.26-1.debian.tar.xz' libthai_0.1.26-1.debian.tar.xz 10772 SHA256:65f94dd05830509da7dcfbef6956584baeefddb1b0e1fa6645c3a6ec065cf635
```

Other potentially useful URLs:

- https://sources.debian.net/src/libthai/0.1.26-1/ (for browsing the source)
- https://sources.debian.net/src/libthai/0.1.26-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libthai/0.1.26-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtheora=1.1.1+dfsg.1-14`

Binary Packages:

- `libtheora0:amd64=1.1.1+dfsg.1-14+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libtheora=1.1.1+dfsg.1-14
'http://deb.debian.org/debian/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-14.dsc' libtheora_1.1.1+dfsg.1-14.dsc 2592 SHA256:20992f97c4ea622cb2336e6795dd5d816eaf29499ed5278d05dd684218c8e91a
'http://deb.debian.org/debian/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1.orig.tar.gz' libtheora_1.1.1+dfsg.1.orig.tar.gz 2100495 SHA256:c59b0f07a7314dfe2ade15c41bc9f637f8a450fc6b340af61b81760629f28f90
'http://deb.debian.org/debian/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-14.debian.tar.xz' libtheora_1.1.1+dfsg.1-14.debian.tar.xz 10532 SHA256:51d8d8bc6a613c42857a5c37e93b013e9239c2bb24c24873161adeee08319bc5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtheora/1.1.1+dfsg.1-14/ (for browsing the source)
- https://sources.debian.net/src/libtheora/1.1.1+dfsg.1-14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtheora/1.1.1+dfsg.1-14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtool=2.4.6-2`

Binary Packages:

- `libltdl7:amd64=2.4.6-2`

Licenses: (parsed from: `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-2
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-2.dsc' libtool_2.4.6-2.dsc 2324 SHA256:caa2b9d5c32e491388d0627e2f808b6cb2f260dd1b0b9fdafc9bff957f05bb29
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-2.debian.tar.xz' libtool_2.4.6-2.debian.tar.xz 36024 SHA256:6227fb1240a90ef06855567e71ee96e4950dd53c4399348f36c1ec39367cd8ea
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtool/2.4.6-2/ (for browsing the source)
- https://sources.debian.net/src/libtool/2.4.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtool/2.4.6-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libusb-1.0=2:1.0.21-1`

Binary Packages:

- `libusb-1.0-0:amd64=2:1.0.21-1`

Licenses: (parsed from: `/usr/share/doc/libusb-1.0-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libusb-1.0=2:1.0.21-1
'http://deb.debian.org/debian/pool/main/libu/libusb-1.0/libusb-1.0_1.0.21-1.dsc' libusb-1.0_1.0.21-1.dsc 2049 SHA256:f20835d4f3b24b82ff286924cff884f66a28a686786bef92495b916f7e0f7d28
'http://deb.debian.org/debian/pool/main/libu/libusb-1.0/libusb-1.0_1.0.21.orig.tar.bz2' libusb-1.0_1.0.21.orig.tar.bz2 607417 SHA256:7dce9cce9a81194b7065ee912bcd55eeffebab694ea403ffb91b67db66b1824b
'http://deb.debian.org/debian/pool/main/libu/libusb-1.0/libusb-1.0_1.0.21-1.debian.tar.xz' libusb-1.0_1.0.21-1.debian.tar.xz 12076 SHA256:d9f6391d796a338e13d82a6a2ac54bcf3fddf1edadd90a17ee555d5c3feb10a8
```

Other potentially useful URLs:

- https://sources.debian.net/src/libusb-1.0/2:1.0.21-1/ (for browsing the source)
- https://sources.debian.net/src/libusb-1.0/2:1.0.21-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libusb-1.0/2:1.0.21-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libva=1.7.3-2`

Binary Packages:

- `libva-drm1:amd64=1.7.3-2`
- `libva-x11-1:amd64=1.7.3-2`
- `libva1:amd64=1.7.3-2`

Licenses: (parsed from: `/usr/share/doc/libva-drm1/copyright`, `/usr/share/doc/libva-x11-1/copyright`, `/usr/share/doc/libva1/copyright`)

- `BSD-3-clause`
- `Expat`
- `Expat-advertising`
- `GPL-2`
- `GPL-2+`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libva=1.7.3-2
'http://deb.debian.org/debian/pool/main/libv/libva/libva_1.7.3-2.dsc' libva_1.7.3-2.dsc 2651 SHA256:b7f56b06c253073ad01e6a653a96366f50ab237b01d4a32112ba371e156205a6
'http://deb.debian.org/debian/pool/main/libv/libva/libva_1.7.3.orig.tar.bz2' libva_1.7.3.orig.tar.bz2 824490 SHA256:22bc139498065a7950d966dbdb000cad04905cbd3dc8f3541f80d36c4670b9d9
'http://deb.debian.org/debian/pool/main/libv/libva/libva_1.7.3-2.debian.tar.xz' libva_1.7.3-2.debian.tar.xz 12492 SHA256:fe0de3fc0d2843c75d0f8156ab985c6f278d96a954d52f42acb8eab2e748fb50
```

Other potentially useful URLs:

- https://sources.debian.net/src/libva/1.7.3-2/ (for browsing the source)
- https://sources.debian.net/src/libva/1.7.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libva/1.7.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvdpau=1.1.1-6`

Binary Packages:

- `libvdpau1:amd64=1.1.1-6`

Licenses: (parsed from: `/usr/share/doc/libvdpau1/copyright`)

- `Expat`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libvdpau=1.1.1-6
'http://deb.debian.org/debian/pool/main/libv/libvdpau/libvdpau_1.1.1-6.dsc' libvdpau_1.1.1-6.dsc 2355 SHA256:e24dc340defaca6dccab92f863df4055bdfd6817e35ec84e03d737341beb278d
'http://deb.debian.org/debian/pool/main/libv/libvdpau/libvdpau_1.1.1.orig.tar.bz2' libvdpau_1.1.1.orig.tar.bz2 429576 SHA256:857a01932609225b9a3a5bf222b85e39b55c08787d0ad427dbd9ec033d58d736
'http://deb.debian.org/debian/pool/main/libv/libvdpau/libvdpau_1.1.1-6.debian.tar.xz' libvdpau_1.1.1-6.debian.tar.xz 15568 SHA256:712c7635040e5f577aeefa50690e78c5a9819fb5d5f2f798fbf6bcd704e938ce
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvdpau/1.1.1-6/ (for browsing the source)
- https://sources.debian.net/src/libvdpau/1.1.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvdpau/1.1.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvisio=0.1.5-4`

Binary Packages:

- `libvisio-0.1-1:amd64=0.1.5-4+b1`

Licenses: (parsed from: `/usr/share/doc/libvisio-0.1-1/copyright`)

- `MIT | GPL-2`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libvisio=0.1.5-4
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.5-4.dsc' libvisio_0.1.5-4.dsc 2177 SHA256:396f166514b274db96ffcf4a1e55833e3cd9433850e27b565d744f0180e030ac
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.5.orig.tar.bz2' libvisio_0.1.5.orig.tar.bz2 602628 SHA256:b83b7991a40b4e7f07d0cac7bb46ddfac84dece705fd18e21bfd119a09be458e
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.5-4.debian.tar.xz' libvisio_0.1.5-4.debian.tar.xz 7860 SHA256:763357f4997f011d5049ff73b871cf34e6f0a164c4d7f1fec5f3983df0c10f61
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvisio/0.1.5-4/ (for browsing the source)
- https://sources.debian.net/src/libvisio/0.1.5-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvisio/0.1.5-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvorbis=1.3.5-4+deb9u2`

Binary Packages:

- `libvorbis0a:amd64=1.3.5-4+deb9u2`
- `libvorbisenc2:amd64=1.3.5-4+deb9u2`
- `libvorbisfile3:amd64=1.3.5-4+deb9u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libvorbis=1.3.5-4+deb9u2
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.5-4+deb9u2.dsc' libvorbis_1.3.5-4+deb9u2.dsc 2566 SHA256:b8480875bda11dd6e676329568b64ff81722426d9178ad28f4f1f267dbd59d96
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.5.orig.tar.gz' libvorbis_1.3.5.orig.tar.gz 1638779 SHA256:6efbcecdd3e5dfbf090341b485da9d176eb250d893e3eb378c428a2db38301ce
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.5-4+deb9u2.debian.tar.xz' libvorbis_1.3.5-4+deb9u2.debian.tar.xz 11532 SHA256:95cabe08962ce58df7e55766be4115802097689700dc8bacfb9f22d495df6955
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvorbis/1.3.5-4+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/libvorbis/1.3.5-4+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvorbis/1.3.5-4+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvpx=1.6.1-3+deb9u2`

Binary Packages:

- `libvpx4:amd64=1.6.1-3+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libvpx4/copyright`)

- `BSD-3-Clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libvpx=1.6.1-3+deb9u2
'http://security.debian.org/debian-security/pool/updates/main/libv/libvpx/libvpx_1.6.1-3+deb9u2.dsc' libvpx_1.6.1-3+deb9u2.dsc 2300 SHA256:eba391dfc6e6d4d1412fd43de406eb0b11d7adfdc3edb9416eeaa35575a37bfd
'http://security.debian.org/debian-security/pool/updates/main/libv/libvpx/libvpx_1.6.1.orig.tar.gz' libvpx_1.6.1.orig.tar.gz 2493087 SHA256:cda8bb6f0e4848c018177d3a576fa83ed96d762554d7010fe4cfb9d70c22e588
'http://security.debian.org/debian-security/pool/updates/main/libv/libvpx/libvpx_1.6.1-3+deb9u2.debian.tar.xz' libvpx_1.6.1-3+deb9u2.debian.tar.xz 13908 SHA256:71ea0477d6cde9600ecd5f79ef903f0139f5f89947f321e3125b0bc5c1aa4408
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvpx/1.6.1-3+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/libvpx/1.6.1-3+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvpx/1.6.1-3+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwebp=0.5.2-1`

Binary Packages:

- `libwebp6:amd64=0.5.2-1`
- `libwebpmux2:amd64=0.5.2-1`

Licenses: (parsed from: `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpmux2/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.5.2-1
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.5.2-1.dsc' libwebp_0.5.2-1.dsc 2065 SHA256:307e845401cbfa71a0b32c213046cca0253a66c4ca71a9bc126ff65ee2bee1c1
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.5.2.orig.tar.gz' libwebp_0.5.2.orig.tar.gz 1221153 SHA256:b75310c810b3eda222c77f6d6c26b061240e3d9060095de44b2c1bae291ecdef
'http://deb.debian.org/debian/pool/main/libw/libwebp/libwebp_0.5.2-1.debian.tar.xz' libwebp_0.5.2-1.debian.tar.xz 5404 SHA256:0b7b36a7212e9bbeba5c61bbf3c78ca08f96e700058fbc9ea6835050e1936448
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwebp/0.5.2-1/ (for browsing the source)
- https://sources.debian.net/src/libwebp/0.5.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwebp/0.5.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwpd=0.10.1-5+deb9u1`

Binary Packages:

- `libwpd-0.10-10:amd64=0.10.1-5+deb9u1`
- `libwpd-tools=0.10.1-5+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libwpd-0.10-10/copyright`, `/usr/share/doc/libwpd-tools/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libwpd=0.10.1-5+deb9u1
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.1-5+deb9u1.dsc' libwpd_0.10.1-5+deb9u1.dsc 2066 SHA256:daa211e797c063f76e2d7692335a81ecddbfd0ef786eddd4e54e112d3ba011d2
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.1.orig.tar.bz2' libwpd_0.10.1.orig.tar.bz2 656856 SHA256:efc20361d6e43f9ff74de5f4d86c2ce9c677693f5da08b0a88d603b7475a508d
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.1-5+deb9u1.debian.tar.xz' libwpd_0.10.1-5+deb9u1.debian.tar.xz 11836 SHA256:3045c8762a0ec2b9855cd86d083d9144283fbeb13f77fd24cff4cdaa9656e2af
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwpd/0.10.1-5+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libwpd/0.10.1-5+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwpd/0.10.1-5+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwpg=0.3.1-3`

Binary Packages:

- `libwpg-0.3-3:amd64=0.3.1-3`

Licenses: (parsed from: `/usr/share/doc/libwpg-0.3-3/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libwpg=0.3.1-3
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.1-3.dsc' libwpg_0.3.1-3.dsc 2010 SHA256:53ee76f68b2e8de3102c1704ff3508f115c41c316009059dced8764a86046957
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.1.orig.tar.bz2' libwpg_0.3.1.orig.tar.bz2 397128 SHA256:29049b95895914e680390717a243b291448e76e0f82fb4d2479adee5330fbb59
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.1-3.debian.tar.xz' libwpg_0.3.1-3.debian.tar.xz 9220 SHA256:fcb1e4890ace78e7c3505bcee564e176a202b82b76990462245b7ffa8eb6ed96
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwpg/0.3.1-3/ (for browsing the source)
- https://sources.debian.net/src/libwpg/0.3.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwpg/0.3.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwps=0.4.5-1`

Binary Packages:

- `libwps-0.4-4:amd64=0.4.5-1`

Licenses: (parsed from: `/usr/share/doc/libwps-0.4-4/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwps=0.4.5-1
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.5-1.dsc' libwps_0.4.5-1.dsc 2231 SHA256:b597715c85da0a949e955c482213fccf22e2fd2fa9c52a09c0709c94e246fcbb
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.5.orig.tar.bz2' libwps_0.4.5.orig.tar.bz2 754271 SHA256:9192ad0c0ad22bfc24ace884286820029c0decc26ad37e0bed0efbd91ff72ea9
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.5-1.debian.tar.xz' libwps_0.4.5-1.debian.tar.xz 8900 SHA256:3a2eac413ff5650b1508ed8fe11b81cd4fadbc1e3e643a07fe03c3d0d04fb99b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwps/0.4.5-1/ (for browsing the source)
- https://sources.debian.net/src/libwps/0.4.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwps/0.4.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.6.4-3+deb9u1`

Binary Packages:

- `libx11-6:amd64=2:1.6.4-3+deb9u1`
- `libx11-data=2:1.6.4-3+deb9u1`
- `libx11-xcb1:amd64=2:1.6.4-3+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.4-3+deb9u1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.4-3+deb9u1.dsc' libx11_1.6.4-3+deb9u1.dsc 2576 SHA256:f58095603558b7db6b5799852c693efb18adcb64b8a85e21433df0f3080101cd
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.4.orig.tar.gz' libx11_1.6.4.orig.tar.gz 3095115 SHA256:5d7fbb9e15c27900ea8963218a59750b674a8d7c94161b66e96fcfbdaa1c6263
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.4-3+deb9u1.diff.gz' libx11_1.6.4-3+deb9u1.diff.gz 42948 SHA256:9f35ff369042893ffc47fa47fea245b355e7a7e44853d8cc4d8a765c32b407f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.6.4-3+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.6.4-3+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.6.4-3+deb9u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxcb=1.12-1`

Binary Packages:

- `libxcb-dri2-0:amd64=1.12-1`
- `libxcb-dri3-0:amd64=1.12-1`
- `libxcb-glx0:amd64=1.12-1`
- `libxcb-present0:amd64=1.12-1`
- `libxcb-render0:amd64=1.12-1`
- `libxcb-shape0:amd64=1.12-1`
- `libxcb-shm0:amd64=1.12-1`
- `libxcb-sync1:amd64=1.12-1`
- `libxcb-xfixes0:amd64=1.12-1`
- `libxcb1:amd64=1.12-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.12-1
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.12-1.dsc' libxcb_1.12-1.dsc 6558 SHA256:d6ed3f5ef255a692c9654d954da4421c535e02f21e56a657383ea9d52389080d
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.12.orig.tar.gz' libxcb_1.12.orig.tar.gz 745984 SHA256:092f147149d8a6410647a848378aaae749304d5b73e028ccb8306aa8a9e26f06
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.12-1.diff.gz' libxcb_1.12-1.diff.gz 25044 SHA256:e2af982573638874bca1f4159139e2bffa0ee51148544b4c3b09bad84622648c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcb/1.12-1/ (for browsing the source)
- https://sources.debian.net/src/libxcb/1.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcb/1.12-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcomposite=1:0.4.4-2`

Binary Packages:

- `libxcomposite1:amd64=1:0.4.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcomposite=1:0.4.4-2
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4-2.dsc' libxcomposite_0.4.4-2.dsc 2178 SHA256:4124027ad4b4598a61c45cbc345988010a2a5ba6e7c80259917f59414be69861
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4.orig.tar.gz' libxcomposite_0.4.4.orig.tar.gz 354584 SHA256:83c04649819c6f52cda1b0ce8bcdcc48ad8618428ad803fb07f20b802f1bdad1
'http://deb.debian.org/debian/pool/main/libx/libxcomposite/libxcomposite_0.4.4-2.diff.gz' libxcomposite_0.4.4-2.diff.gz 15755 SHA256:9689ae3fcc76054fe09909692e71a1a4fe356e84f3adfa2be668e173d0369ebc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcomposite/1:0.4.4-2/ (for browsing the source)
- https://sources.debian.net/src/libxcomposite/1:0.4.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcomposite/1:0.4.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcursor=1:1.1.14-1+deb9u2`

Binary Packages:

- `libxcursor1:amd64=1:1.1.14-1+deb9u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcursor=1:1.1.14-1+deb9u2
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.14-1+deb9u2.dsc' libxcursor_1.1.14-1+deb9u2.dsc 2334 SHA256:c7d9fb3b4aee36b317f62a8a04697931ac2356f9ebf7f8937c7e9ac8a41034ea
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.14.orig.tar.gz' libxcursor_1.1.14.orig.tar.gz 374910 SHA256:be0954faf274969ffa6d95b9606b9c0cfee28c13b6fc014f15606a0c8b05c17b
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.14-1+deb9u2.diff.gz' libxcursor_1.1.14-1+deb9u2.diff.gz 19765 SHA256:5b56f9b5f9327471ddfd8c5f8a349d93faded3b40e9eb1d0ea1b5129e2db84a3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcursor/1:1.1.14-1+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/libxcursor/1:1.1.14-1+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcursor/1:1.1.14-1+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdamage=1:1.1.4-2`

Binary Packages:

- `libxdamage1:amd64=1:1.1.4-2+b3`

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

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

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

### `dpkg` source package: `libxfixes=1:5.0.3-1`

Binary Packages:

- `libxfixes3:amd64=1:5.0.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxfixes=1:5.0.3-1
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.3-1.dsc' libxfixes_5.0.3-1.dsc 2040 SHA256:87c1c491d8ff261b5a723c6c6aa974f315ff6f25f47425285a62065cbf944025
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.3.orig.tar.gz' libxfixes_5.0.3.orig.tar.gz 360412 SHA256:9ab6c13590658501ce4bd965a8a5d32ba4d8b3bb39a5a5bc9901edffc5666570
'http://deb.debian.org/debian/pool/main/libx/libxfixes/libxfixes_5.0.3-1.diff.gz' libxfixes_5.0.3-1.diff.gz 15140 SHA256:95b9688465531c60ff372bf8a2eb5fdd456970cbbb679ba13e54d24af44fb904
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxfixes/1:5.0.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxfixes/1:5.0.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxfixes/1:5.0.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxi=2:1.7.9-1`

Binary Packages:

- `libxi6:amd64=2:1.7.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxi=2:1.7.9-1
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.9-1.dsc' libxi_1.7.9-1.dsc 2202 SHA256:fb19b7e8b9ad6306c3e8a6728f29576f956f07a7980e7b4d727259714d6ca686
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.9.orig.tar.gz' libxi_1.7.9.orig.tar.gz 604214 SHA256:463cc5370191404bc0f8a450fdbf6d9159efbbf274e5e0f427a60191fed9cf4b
'http://deb.debian.org/debian/pool/main/libx/libxi/libxi_1.7.9-1.diff.gz' libxi_1.7.9-1.diff.gz 15892 SHA256:8c9c221faecc97a7ba7ff1a1a14fad580c49b72e270dc3aae40b72b2d7f4dc5e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxi/2:1.7.9-1/ (for browsing the source)
- https://sources.debian.net/src/libxi/2:1.7.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxi/2:1.7.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxinerama=2:1.1.3-1`

Binary Packages:

- `libxinerama1:amd64=2:1.1.3-1+b3`

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

### `dpkg` source package: `libxkbcommon=0.7.1-2~deb9u1`

Binary Packages:

- `libxkbcommon0:amd64=0.7.1-2~deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxkbcommon=0.7.1-2~deb9u1
'http://deb.debian.org/debian/pool/main/libx/libxkbcommon/libxkbcommon_0.7.1-2~deb9u1.dsc' libxkbcommon_0.7.1-2~deb9u1.dsc 2386 SHA256:f53cfc53bfab41e6b94a0c7ba1e94501b05bd759aef4e04fadfee3afa43d816d
'http://deb.debian.org/debian/pool/main/libx/libxkbcommon/libxkbcommon_0.7.1.orig.tar.gz' libxkbcommon_0.7.1.orig.tar.gz 977667 SHA256:db941b54113b24003dadbf671505194d67e513b54006df9350b8697442af0ad9
'http://deb.debian.org/debian/pool/main/libx/libxkbcommon/libxkbcommon_0.7.1-2~deb9u1.diff.gz' libxkbcommon_0.7.1-2~deb9u1.diff.gz 32105 SHA256:7ff7f125d257a5573a7c36b0f8e2e1e39b503ffd6810c5e51378c1efafb6c724
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxkbcommon/0.7.1-2~deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libxkbcommon/0.7.1-2~deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxkbcommon/0.7.1-2~deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxml2=2.9.4+dfsg1-2.2+deb9u2`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-2.2+deb9u2`

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

### `dpkg` source package: `libxrandr=2:1.5.1-1`

Binary Packages:

- `libxrandr2:amd64=2:1.5.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrandr=2:1.5.1-1
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.5.1-1.dsc' libxrandr_1.5.1-1.dsc 2046 SHA256:0d7102ab75fdfe06534e842d5dcac8430614c61a061ab12794e2285712b0b103
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.5.1.orig.tar.gz' libxrandr_1.5.1.orig.tar.gz 388607 SHA256:2baa7fb3eca78fe7e11a09b373ba898b717f7eeba4a4bfd68187e04b4789b0d3
'http://deb.debian.org/debian/pool/main/libx/libxrandr/libxrandr_1.5.1-1.diff.gz' libxrandr_1.5.1-1.diff.gz 16386 SHA256:42262cbc2117ea559a4e16a02c6ea6478554aa2128d9fe1e141da07006612a1d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxrandr/2:1.5.1-1/ (for browsing the source)
- https://sources.debian.net/src/libxrandr/2:1.5.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxrandr/2:1.5.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxshmfence=1.2-1`

Binary Packages:

- `libxshmfence1:amd64=1.2-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxshmfence=1.2-1
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.2-1.dsc' libxshmfence_1.2-1.dsc 2128 SHA256:85a28d2f6211ebbf0a115d0f72d874cce179178958bcb2a77094e3499464b25d
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.2.orig.tar.gz' libxshmfence_1.2.orig.tar.gz 355356 SHA256:58467a0e36fc4ec749dc55f81a4ab3b822c82b6dfb7d36bdb6b28c9fd2a5ccaf
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.2-1.diff.gz' libxshmfence_1.2-1.diff.gz 13284 SHA256:65db7e07c5c5b12d0b1f93cdb0c4e3e448429240044247ea2f64a89c0cce5f8e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxshmfence/1.2-1/ (for browsing the source)
- https://sources.debian.net/src/libxshmfence/1.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxshmfence/1.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxslt=1.1.29-2.1+deb9u1`

Binary Packages:

- `libxslt1.1:amd64=1.1.29-2.1+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.29-2.1+deb9u1
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.29-2.1+deb9u1.dsc' libxslt_1.1.29-2.1+deb9u1.dsc 2563 SHA256:a7b353c973bd0a66c85c2786c608d9059fafa7c4f58613e3ca5a47124f4c4bb6
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.29.orig.tar.gz' libxslt_1.1.29.orig.tar.gz 3428524 SHA256:b5976e3857837e7617b29f2249ebb5eeac34e249208d31f1fbf7a6ba7a4090ce
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.29-2.1+deb9u1.debian.tar.xz' libxslt_1.1.29-2.1+deb9u1.debian.tar.xz 30436 SHA256:1551bfcb01d176f629a4dbc9031617ecc35a8f1825fa470b4e9191115cb0f3dd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxslt/1.1.29-2.1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libxslt/1.1.29-2.1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxslt/1.1.29-2.1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxss=1:1.2.2-1`

Binary Packages:

- `libxss1:amd64=1:1.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxss=1:1.2.2-1
'http://deb.debian.org/debian/pool/main/libx/libxss/libxss_1.2.2-1.dsc' libxss_1.2.2-1.dsc 2042 SHA256:22379490d80d7661c793f0f016a5e12255fdb53a0b2b58b6fe14afa805fcac3f
'http://deb.debian.org/debian/pool/main/libx/libxss/libxss_1.2.2.orig.tar.gz' libxss_1.2.2.orig.tar.gz 348915 SHA256:e12ba814d44f7b58534c0d8521e2d4574f7bf2787da405de4341c3b9f4cc8d96
'http://deb.debian.org/debian/pool/main/libx/libxss/libxss_1.2.2-1.diff.gz' libxss_1.2.2-1.diff.gz 14712 SHA256:fcc9c125f3af01da27f6cee798410a7907a63802f5c6360f972e12b1ff59e6c1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxss/1:1.2.2-1/ (for browsing the source)
- https://sources.debian.net/src/libxss/1:1.2.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxss/1:1.2.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxtst=2:1.2.3-1`

Binary Packages:

- `libxtst6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxtst=2:1.2.3-1
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.3-1.dsc' libxtst_1.2.3-1.dsc 2243 SHA256:979f05e505ea319c3f75955e10345338f77a512f5a6a0a887d6f4633d6bd4633
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.3.orig.tar.gz' libxtst_1.2.3.orig.tar.gz 400197 SHA256:a0c83acce02d4923018c744662cb28eb0dbbc33b4adc027726879ccf68fbc2c2
'http://deb.debian.org/debian/pool/main/libx/libxtst/libxtst_1.2.3-1.diff.gz' libxtst_1.2.3-1.diff.gz 10177 SHA256:c4739fc7ccda7caaffcf36f934b7c33463390e71d567c7d62f635db1946b74ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxtst/2:1.2.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxtst/2:1.2.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxtst/2:1.2.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxv=2:1.0.11-1`

Binary Packages:

- `libxv1:amd64=2:1.0.11-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxv=2:1.0.11-1
'http://deb.debian.org/debian/pool/main/libx/libxv/libxv_1.0.11-1.dsc' libxv_1.0.11-1.dsc 1959 SHA256:7753e8d4496ec0d3f32417b03cfc8b344e2dff486e46f630158a6a52e4bd8542
'http://deb.debian.org/debian/pool/main/libx/libxv/libxv_1.0.11.orig.tar.gz' libxv_1.0.11.orig.tar.gz 387057 SHA256:c4112532889b210e21cf05f46f0f2f8354ff7e1b58061e12d7a76c95c0d47bb1
'http://deb.debian.org/debian/pool/main/libx/libxv/libxv_1.0.11-1.diff.gz' libxv_1.0.11-1.diff.gz 8235 SHA256:529ed2bcbccc9340c9c7987e8c5ed933a0fa41d6e4e67ef71ce3925ac83d93b6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxv/2:1.0.11-1/ (for browsing the source)
- https://sources.debian.net/src/libxv/2:1.0.11-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxv/2:1.0.11-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxxf86vm=1:1.1.4-1`

Binary Packages:

- `libxxf86vm1:amd64=1:1.1.4-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxxf86vm=1:1.1.4-1
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.dsc' libxxf86vm_1.1.4-1.dsc 2078 SHA256:5a3aded030a415b0d6c201d2b9d3af36f241dc981f10052fd4c2b56d59597838
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4.orig.tar.gz' libxxf86vm_1.1.4.orig.tar.gz 363146 SHA256:5108553c378a25688dcb57dca383664c36e293d60b1505815f67980ba9318a99
'http://deb.debian.org/debian/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.diff.gz' libxxf86vm_1.1.4-1.diff.gz 8040 SHA256:e0f11739d28c7a4475820ebda26e6f29e6cfa80b99a3513c075471132c81725b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxxf86vm/1:1.1.4-1/ (for browsing the source)
- https://sources.debian.net/src/libxxf86vm/1:1.1.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxxf86vm/1:1.1.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lp-solve=5.5.0.15-4`

Binary Packages:

- `lp-solve=5.5.0.15-4+b1`

Licenses: (parsed from: `/usr/share/doc/lp-solve/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris lp-solve=5.5.0.15-4
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.15-4.dsc' lp-solve_5.5.0.15-4.dsc 2236 SHA256:e8df23b10cf0a730d2d6d1d4c366aec78f9c5f0ff7d75eaa2b123d873d41ce6b
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.15.orig-doc.tar.gz' lp-solve_5.5.0.15.orig-doc.tar.gz 1484929 SHA256:a9dcfa62148a283a6e11c0bb9524f4d5a4a4ecf06511e32cbd2faec04f791e17
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.15.orig.tar.gz' lp-solve_5.5.0.15.orig.tar.gz 802881 SHA256:ea1243e8aa2f0d52172dc0a90d1c2a8d2a4f696a39fc9cf07321810363d18985
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.0.15-4.debian.tar.xz' lp-solve_5.5.0.15-4.debian.tar.xz 9628 SHA256:f68b43e394b2e9795ddf7cfba41bc4f9a36a9e2f8e8efe798e86c6544baaf509
```

Other potentially useful URLs:

- https://sources.debian.net/src/lp-solve/5.5.0.15-4/ (for browsing the source)
- https://sources.debian.net/src/lp-solve/5.5.0.15-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lp-solve/5.5.0.15-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `lvm2=2.02.168-2`

Binary Packages:

- `dmsetup=2:1.02.137-2`
- `libdevmapper1.02.1:amd64=2:1.02.137-2`

Licenses: (parsed from: `/usr/share/doc/dmsetup/copyright`, `/usr/share/doc/libdevmapper1.02.1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris lvm2=2.02.168-2
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.168-2.dsc' lvm2_2.02.168-2.dsc 2736 SHA256:a06f0cb7e11db0186e9895eca62f8a8219da68b69081e9abed54801e30e597bb
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.168.orig.tar.xz' lvm2_2.02.168.orig.tar.xz 1562080 SHA256:ca257318fecfc66fb36b5ea02d90e075afb340557fcf5a343ba6071f84aeed8c
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.02.168-2.debian.tar.xz' lvm2_2.02.168-2.debian.tar.xz 32516 SHA256:1a6673093d4ef5eef4555c109b934cf2f89c1288f926dc4a4b949f1705feed8f
```

Other potentially useful URLs:

- https://sources.debian.net/src/lvm2/2.02.168-2/ (for browsing the source)
- https://sources.debian.net/src/lvm2/2.02.168-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lvm2/2.02.168-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mercurial=4.0-1+deb9u1`

Binary Packages:

- `mercurial=4.0-1+deb9u1`
- `mercurial-common=4.0-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=4.0-1+deb9u1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_4.0-1+deb9u1.dsc' mercurial_4.0-1+deb9u1.dsc 2427 SHA256:ba44c9b1c5426154dd3bf44ad16b2973e4da475b8dd5d97ce9ebcd3ec472e174
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_4.0.orig.tar.gz' mercurial_4.0.orig.tar.gz 4850316 SHA256:24be080745230840f214d93e9f9fb4e25510f9abbbec2e56fab18543fedc43a7
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_4.0-1+deb9u1.debian.tar.xz' mercurial_4.0-1+deb9u1.debian.tar.xz 101944 SHA256:83c6dee02fa4df95235a2f03baea99731a37e9d8d166362db6152a2990e6ad96
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/4.0-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/mercurial/4.0-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/4.0-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mesa=13.0.6-1`

Binary Packages:

- `libegl1-mesa:amd64=13.0.6-1+b2`
- `libgbm1:amd64=13.0.6-1+b2`
- `libgl1-mesa-glx:amd64=13.0.6-1+b2`
- `libglapi-mesa:amd64=13.0.6-1+b2`
- `libwayland-egl1-mesa:amd64=13.0.6-1+b2`

Licenses: (parsed from: `/usr/share/doc/libegl1-mesa/copyright`, `/usr/share/doc/libgbm1/copyright`, `/usr/share/doc/libgl1-mesa-glx/copyright`, `/usr/share/doc/libglapi-mesa/copyright`, `/usr/share/doc/libwayland-egl1-mesa/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris mesa=13.0.6-1
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_13.0.6-1.dsc' mesa_13.0.6-1.dsc 4571 SHA256:563d23edf784ca6ae8369e1b4d791a7952bf4e9c38c44e3f20376fcbeff1eec8
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_13.0.6.orig.tar.gz' mesa_13.0.6.orig.tar.gz 15481392 SHA256:1076590f29103f022a2cd87e6dff6ae77072013745603d06b0410c373ab2bb1a
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_13.0.6-1.diff.gz' mesa_13.0.6-1.diff.gz 86452 SHA256:02a85877d37cd36f713d6170e33cef72b00dccafff708262f8eeb4d5c3b47883
```

Other potentially useful URLs:

- https://sources.debian.net/src/mesa/13.0.6-1/ (for browsing the source)
- https://sources.debian.net/src/mesa/13.0.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mesa/13.0.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mhash=0.9.9.9-7`

Binary Packages:

- `libmhash2:amd64=0.9.9.9-7`

Licenses: (parsed from: `/usr/share/doc/libmhash2/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris mhash=0.9.9.9-7
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9-7.dsc' mhash_0.9.9.9-7.dsc 1947 SHA256:cb4349ff77c8ad7ecb0b5d02083d0a0f2d60f7e8dd6ce4735cbafc7b4dc63461
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9.orig.tar.gz' mhash_0.9.9.9.orig.tar.gz 577533 SHA256:73991e9e54bb392484a510943d4c5d395462181cc4abe53f863edec13c335403
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9-7.debian.tar.xz' mhash_0.9.9.9-7.debian.tar.xz 11120 SHA256:229076933ac07420e16f7ab76e820aba79158cd7c5f3204fd1adac4f048bbe5a
```

Other potentially useful URLs:

- https://sources.debian.net/src/mhash/0.9.9.9-7/ (for browsing the source)
- https://sources.debian.net/src/mhash/0.9.9.9-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mhash/0.9.9.9-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mime-support=3.60`

Binary Packages:

- `mime-support=3.60`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.60
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.60.dsc' mime-support_3.60.dsc 1605 SHA256:1c3c61f6943b130ee6518facac394b733661975955b84af640b78fa354d7595d
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.60.tar.gz' mime-support_3.60.tar.gz 36840 SHA256:f31d81f68dc007f56567cc14fb3b2effbd42d1dd087e414508e14e33d1a6a3a4
```

Other potentially useful URLs:

- https://sources.debian.net/src/mime-support/3.60/ (for browsing the source)
- https://sources.debian.net/src/mime-support/3.60/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mime-support/3.60/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpdecimal=2.4.2-1`

Binary Packages:

- `libmpdec2:amd64=2.4.2-1`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-1
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.2-1.dsc' mpdecimal_2.4.2-1.dsc 1893 SHA256:5bc782829357ebc9f0c12084642319e5ac89784a119433f8bfba7a11008d7c13
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.2-1.debian.tar.xz' mpdecimal_2.4.2-1.debian.tar.xz 5172 SHA256:b95fb775fd04a7ad34fa5bd2c222b49ee2dfd7f0e15295dbd3f7fb86a9b0194b
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpdecimal/2.4.2-1/ (for browsing the source)
- https://sources.debian.net/src/mpdecimal/2.4.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpdecimal/2.4.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpg123=1.23.8-1`

Binary Packages:

- `libmpg123-0:amd64=1.23.8-1+b1`

Licenses: (parsed from: `/usr/share/doc/libmpg123-0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpg123=1.23.8-1
'http://deb.debian.org/debian/pool/main/m/mpg123/mpg123_1.23.8-1.dsc' mpg123_1.23.8-1.dsc 2280 SHA256:3842e9fe8e3f16a123953c407e69e1302d7699175858528ca3d6f6fcc340e02f
'http://deb.debian.org/debian/pool/main/m/mpg123/mpg123_1.23.8.orig.tar.bz2' mpg123_1.23.8.orig.tar.bz2 893728 SHA256:de2303c8ecb65593e39815c0a2f2f2d91f708c43b85a55fdd1934c82e677cf8e
'http://deb.debian.org/debian/pool/main/m/mpg123/mpg123_1.23.8-1.debian.tar.xz' mpg123_1.23.8-1.debian.tar.xz 23296 SHA256:94eadde46dc8235be91397877660f5927bbe17913d7346b7fdb4ae00fb87612f
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpg123/1.23.8-1/ (for browsing the source)
- https://sources.debian.net/src/mpg123/1.23.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpg123/1.23.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mythes=2:1.2.4-3`

Binary Packages:

- `libmythes-1.2-0:amd64=2:1.2.4-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris mythes=2:1.2.4-3
'http://deb.debian.org/debian/pool/main/m/mythes/mythes_1.2.4-3.dsc' mythes_1.2.4-3.dsc 1846 SHA256:d308af92445c1ed8cbadd3d57df0a3aa4ac1063d158d5337fe682b259e8d0c47
'http://deb.debian.org/debian/pool/main/m/mythes/mythes_1.2.4.orig.tar.gz' mythes_1.2.4.orig.tar.gz 4910303 SHA256:1e81f395d8c851c3e4e75b568e20fa2fa549354e75ab397f9de4b0e0790a305f
'http://deb.debian.org/debian/pool/main/m/mythes/mythes_1.2.4-3.debian.tar.xz' mythes_1.2.4-3.debian.tar.xz 5060 SHA256:4515e2ef57f2d35de4034dc5ffbf0964a27dd6cb6189b16b50cc8fa0d6914cbe
```

Other potentially useful URLs:

- https://sources.debian.net/src/mythes/2:1.2.4-3/ (for browsing the source)
- https://sources.debian.net/src/mythes/2:1.2.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mythes/2:1.2.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.0+20161126-1+deb9u2`

Binary Packages:

- `libncurses5:amd64=6.0+20161126-1+deb9u2`
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

### `dpkg` source package: `neon27=0.30.2-2`

Binary Packages:

- `libneon27-gnutls:amd64=0.30.2-2`

Licenses: (parsed from: `/usr/share/doc/libneon27-gnutls/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris neon27=0.30.2-2
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.2-2.dsc' neon27_0.30.2-2.dsc 2161 SHA256:4fbd7df7bad817622e83eb974e932ae83c83d8265c8ad689de963d438d3f7584
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.2.orig.tar.gz' neon27_0.30.2.orig.tar.gz 932779 SHA256:db0bd8cdec329b48f53a6f00199c92d5ba40b0f015b153718d1b15d3d967fbca
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.2-2.debian.tar.xz' neon27_0.30.2-2.debian.tar.xz 10512 SHA256:5f828eebc843ac38070631aa064f3dc1837104fb57040951dbf80bd7bd6e5190
```

Other potentially useful URLs:

- https://sources.debian.net/src/neon27/0.30.2-2/ (for browsing the source)
- https://sources.debian.net/src/neon27/0.30.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/neon27/0.30.2-2/ (for access to the source package after it no longer exists in the archive)

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

Licenses: (parsed from: `/usr/share/doc/libhogweed4/copyright`, `/usr/share/doc/libnettle6/copyright`)

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
'http://security.debian.org/debian-security/pool/updates/main/n/nghttp2/nghttp2_1.18.1-1+deb9u1.dsc' nghttp2_1.18.1-1+deb9u1.dsc 2657 SHA256:fc99fa8d124d322f7cd872c3088a268ea86f42e71229fc98d8a90869950d0a14
'http://security.debian.org/debian-security/pool/updates/main/n/nghttp2/nghttp2_1.18.1.orig.tar.bz2' nghttp2_1.18.1.orig.tar.bz2 1780766 SHA256:5d8bb930eb90c552ec836c7b1862406b69cafcda5520bf266c8f5d914d9b447c
'http://security.debian.org/debian-security/pool/updates/main/n/nghttp2/nghttp2_1.18.1-1+deb9u1.debian.tar.xz' nghttp2_1.18.1-1+deb9u1.debian.tar.xz 12300 SHA256:94cf473ee6a78181ebdddc18676df356fb788540cf426b7eca944573f2808733
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.18.1-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.18.1-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.18.1-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `npth=1.3-1`

Binary Packages:

- `libnpth0:amd64=1.3-1`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.3-1
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.3-1.dsc' npth_1.3-1.dsc 1949 SHA256:63e2598a3aebe21ef7969a601906a719e923673e04a4d157b6dde605566079be
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.3.orig.tar.bz2' npth_1.3.orig.tar.bz2 295998 SHA256:bca81940436aed0734eb8d0ff8b179e04cc8c087f5625204419f5f45d736a82a
'http://deb.debian.org/debian/pool/main/n/npth/npth_1.3-1.debian.tar.xz' npth_1.3-1.debian.tar.xz 10324 SHA256:4910e19597aea46841eaffc6df58ecf91d5d059130ecb1442fee9f5f963b229c
```

Other potentially useful URLs:

- https://sources.debian.net/src/npth/1.3-1/ (for browsing the source)
- https://sources.debian.net/src/npth/1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/npth/1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nspr=2:4.12-6`

Binary Packages:

- `libnspr4:amd64=2:4.12-6`

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

### `dpkg` source package: `numactl=2.0.11-2.1`

Binary Packages:

- `libnuma1:amd64=2.0.11-2.1`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.11-2.1
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.11-2.1.dsc' numactl_2.0.11-2.1.dsc 1613 SHA256:3462c9e9a53e1cdbec095092859fdd2448e629a687b6dac511f83708cecbbfe3
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.11.orig.tar.gz' numactl_2.0.11.orig.tar.gz 408175 SHA256:450c091235f891ee874a8651b179c30f57a1391ca5c4673354740ba65e527861
'http://deb.debian.org/debian/pool/main/n/numactl/numactl_2.0.11-2.1.debian.tar.xz' numactl_2.0.11-2.1.debian.tar.xz 6760 SHA256:1dc86f99e7b2d8d652a2af34b14d66b7a3637316403789a3c10f09b490cf89d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/numactl/2.0.11-2.1/ (for browsing the source)
- https://sources.debian.net/src/numactl/2.0.11-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/numactl/2.0.11-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openal-soft=1:1.17.2-4`

Binary Packages:

- `libopenal-data=1:1.17.2-4`
- `libopenal1:amd64=1:1.17.2-4+b2`

Licenses: (parsed from: `/usr/share/doc/libopenal-data/copyright`, `/usr/share/doc/libopenal1/copyright`)

- `Apache`
- `BSD-3-clause-cmake`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris openal-soft=1:1.17.2-4
'http://deb.debian.org/debian/pool/main/o/openal-soft/openal-soft_1.17.2-4.dsc' openal-soft_1.17.2-4.dsc 2569 SHA256:1f53ca73c13ac7e578958f0c3f6ee720bcc954d9fe6cd80cce039907e68df179
'http://deb.debian.org/debian/pool/main/o/openal-soft/openal-soft_1.17.2.orig.tar.bz2' openal-soft_1.17.2.orig.tar.bz2 486934 SHA256:a341f8542f1f0b8c65241a17da13d073f18ec06658e1a1606a8ecc8bbc2b3314
'http://deb.debian.org/debian/pool/main/o/openal-soft/openal-soft_1.17.2-4.debian.tar.xz' openal-soft_1.17.2-4.debian.tar.xz 12716 SHA256:aaa87e1f08cc701f1ddf03d6648854c136ea19f7245fe3615273b5ee926cbbea
```

Other potentially useful URLs:

- https://sources.debian.net/src/openal-soft/1:1.17.2-4/ (for browsing the source)
- https://sources.debian.net/src/openal-soft/1:1.17.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openal-soft/1:1.17.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `opencv=2.4.9.1+dfsg1-2`

Binary Packages:

- `libopencv-core2.4v5:amd64=2.4.9.1+dfsg1-2`
- `libopencv-imgproc2.4v5:amd64=2.4.9.1+dfsg1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris opencv=2.4.9.1+dfsg1-2
'http://deb.debian.org/debian/pool/main/o/opencv/opencv_2.4.9.1+dfsg1-2.dsc' opencv_2.4.9.1+dfsg1-2.dsc 5992 SHA256:4e414ba11af4ee69fd081384ecb4fc8bd23aed6d758a2f366a7c0a09d7cb3e2c
'http://deb.debian.org/debian/pool/main/o/opencv/opencv_2.4.9.1+dfsg1.orig.tar.xz' opencv_2.4.9.1+dfsg1.orig.tar.xz 54171652 SHA256:bad5380d935277b3553f2146b9cd49a1ba3e402b4845fb54fd80787ff057b5c7
'http://deb.debian.org/debian/pool/main/o/opencv/opencv_2.4.9.1+dfsg1-2.debian.tar.xz' opencv_2.4.9.1+dfsg1-2.debian.tar.xz 33276 SHA256:fdd6ca715d30d4cdd6d693f92b7b4877d1781a2a0024ad0410e55eaaa93d0cf8
```

Other potentially useful URLs:

- https://sources.debian.net/src/opencv/2.4.9.1+dfsg1-2/ (for browsing the source)
- https://sources.debian.net/src/opencv/2.4.9.1+dfsg1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/opencv/2.4.9.1+dfsg1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openjpeg2=2.1.2-1.1+deb9u3`

Binary Packages:

- `libopenjp2-7:amd64=2.1.2-1.1+deb9u3`

Licenses: (parsed from: `/usr/share/doc/libopenjp2-7/copyright`)

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
$ apt-get source -qq --print-uris openjpeg2=2.1.2-1.1+deb9u3
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.1.2-1.1+deb9u3.dsc' openjpeg2_2.1.2-1.1+deb9u3.dsc 2797 SHA256:dcb5cf6adee12ab0cc23d9a08731df6ee87406a98f623233348580e9f0373f78
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.1.2.orig.tar.gz' openjpeg2_2.1.2.orig.tar.gz 1987071 SHA256:4ce77b6ef538ef090d9bde1d5eeff8b3069ab56c4906f083475517c2c023dfa7
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.1.2-1.1+deb9u3.debian.tar.xz' openjpeg2_2.1.2-1.1+deb9u3.debian.tar.xz 25464 SHA256:c168bec05ef60b78e1d219760d6faf67e58f9055cbde770005bd12123c3b0002
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjpeg2/2.1.2-1.1+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/openjpeg2/2.1.2-1.1+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjpeg2/2.1.2-1.1+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.44+dfsg-5+deb9u3`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.44+dfsg-5+deb9u3`
- `libldap-common=2.4.44+dfsg-5+deb9u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.44+dfsg-5+deb9u3
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.44+dfsg-5+deb9u3.dsc' openldap_2.4.44+dfsg-5+deb9u3.dsc 3009 SHA256:feff6977d4674bbbbe3c34c9d292edcfe6d895d10aa165910dbc96819a327abb
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.44+dfsg.orig.tar.gz' openldap_2.4.44+dfsg.orig.tar.gz 4826590 SHA256:d5187c229bec163c5d97845846e1b87917755f85b04f444c08836384f4bd7ffe
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.44+dfsg-5+deb9u3.debian.tar.xz' openldap_2.4.44+dfsg-5+deb9u3.debian.tar.xz 168576 SHA256:926e2b00418901d9b52d314a6f6319f84c9dd04e12d085830ffc37bf3329c402
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.44+dfsg-5+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.44+dfsg-5+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.44+dfsg-5+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:7.4p1-10+deb9u7`

Binary Packages:

- `openssh-client=1:7.4p1-10+deb9u7`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-3-clause`
- `Beer-ware`
- `CORE-SDI-BSD-style`
- `Expat-with-advertising-restriction`
- `GPL-2 with OpenSSH-linking exception`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:7.4p1-10+deb9u7
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.4p1-10+deb9u7.dsc' openssh_7.4p1-10+deb9u7.dsc 2924 SHA256:8446f0cc09ef50c650188e674e0cefe77fcc853e874357b1c68e620dfee9dbf4
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.4p1.orig.tar.gz' openssh_7.4p1.orig.tar.gz 1511780 SHA256:1b1fc4a14e2024293181924ed24872e6f2e06293f3e8926a376b8aec481f19d1
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.4p1-10+deb9u7.debian.tar.xz' openssh_7.4p1-10+deb9u7.debian.tar.xz 171104 SHA256:3620c8d683ffa5e16361caed3339ea1c3064c6d456d6ff718e138e33786cc06d
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:7.4p1-10+deb9u7/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:7.4p1-10+deb9u7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:7.4p1-10+deb9u7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl1.0=1.0.2u-1~deb9u1`

Binary Packages:

- `libssl1.0.2:amd64=1.0.2u-1~deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl1.0=1.0.2u-1~deb9u1
'http://security.debian.org/debian-security/pool/updates/main/o/openssl1.0/openssl1.0_1.0.2u-1~deb9u1.dsc' openssl1.0_1.0.2u-1~deb9u1.dsc 2383 SHA256:35e2627956512ce933f91e66ecb4a276200d8d1ab67ee599fc1a8dd7ae0a183a
'http://security.debian.org/debian-security/pool/updates/main/o/openssl1.0/openssl1.0_1.0.2u.orig.tar.gz' openssl1.0_1.0.2u.orig.tar.gz 5355412 SHA256:ecd0c6ffb493dd06707d38b14bb4d8c2288bb7033735606569d8f90f89669d16
'http://security.debian.org/debian-security/pool/updates/main/o/openssl1.0/openssl1.0_1.0.2u.orig.tar.gz.asc' openssl1.0_1.0.2u.orig.tar.gz.asc 488 SHA256:84d7a8b23df5567e80e3732f69c5428ee533a2bc7c3c2264dd8390a7af2a8620
'http://security.debian.org/debian-security/pool/updates/main/o/openssl1.0/openssl1.0_1.0.2u-1~deb9u1.debian.tar.xz' openssl1.0_1.0.2u-1~deb9u1.debian.tar.xz 94808 SHA256:2b3beb8c675e7ede236e7f54ebad5df277c995722c9a85ca6e0033896119db7c
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl1.0/1.0.2u-1~deb9u1/ (for browsing the source)
- https://sources.debian.net/src/openssl1.0/1.0.2u-1~deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl1.0/1.0.2u-1~deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.0l-1~deb9u1`

Binary Packages:

- `libssl1.1:amd64=1.1.0l-1~deb9u1`
- `openssl=1.1.0l-1~deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.0l-1~deb9u1
'http://security.debian.org/debian-security/pool/updates/main/o/openssl/openssl_1.1.0l-1~deb9u1.dsc' openssl_1.1.0l-1~deb9u1.dsc 2437 SHA256:9ae8fb3e89110ad3c75ba6a52b8f40cc5419b56f31c5c8b6f6aca0949cd90ea7
'http://security.debian.org/debian-security/pool/updates/main/o/openssl/openssl_1.1.0l.orig.tar.gz' openssl_1.1.0l.orig.tar.gz 5294857 SHA256:74a2f756c64fd7386a29184dc0344f4831192d61dc2481a93a4c5dd727f41148
'http://security.debian.org/debian-security/pool/updates/main/o/openssl/openssl_1.1.0l.orig.tar.gz.asc' openssl_1.1.0l.orig.tar.gz.asc 488 SHA256:afc83de9f9f1ef5f79ab8a31bbdeb26f9ac9a07cfdab7628a773267d31f85e42
'http://security.debian.org/debian-security/pool/updates/main/o/openssl/openssl_1.1.0l-1~deb9u1.debian.tar.xz' openssl_1.1.0l-1~deb9u1.debian.tar.xz 72100 SHA256:78290d8a50219fe9c1c5676084a5567b23aff12f701bcd975e4c0d32264d5116
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.0l-1~deb9u1/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.0l-1~deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.0l-1~deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `opus=1.2~alpha2-1`

Binary Packages:

- `libopus0:amd64=1.2~alpha2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris opus=1.2~alpha2-1
'http://deb.debian.org/debian/pool/main/o/opus/opus_1.2~alpha2-1.dsc' opus_1.2~alpha2-1.dsc 1967 SHA256:1b281c14f23ff5336f2edfc07181ae9a6d358a72162598589fec609df83d9de6
'http://deb.debian.org/debian/pool/main/o/opus/opus_1.2~alpha2.orig.tar.gz' opus_1.2~alpha2.orig.tar.gz 1021012 SHA256:148d38cd0a19e0dde7f7e5491c19953025ff4e7e172e7b21fcf7ba3ff84fa06e
'http://deb.debian.org/debian/pool/main/o/opus/opus_1.2~alpha2-1.diff.gz' opus_1.2~alpha2-1.diff.gz 7445 SHA256:0bc67d52b0d1de2836390e267240c4bd998c5985e34a71d03ba3f57d7668a219
```

Other potentially useful URLs:

- https://sources.debian.net/src/opus/1.2~alpha2-1/ (for browsing the source)
- https://sources.debian.net/src/opus/1.2~alpha2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/opus/1.2~alpha2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `orc=1:0.4.26-2`

Binary Packages:

- `liborc-0.4-0:amd64=1:0.4.26-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris orc=1:0.4.26-2
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.26-2.dsc' orc_0.4.26-2.dsc 2475 SHA256:567e6ea1cda4be1d29cba0bafac9a7d1e414b1f301e6855c959c3e16d43442bd
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.26.orig.tar.xz' orc_0.4.26.orig.tar.xz 465768 SHA256:7d52fa80ef84988359c3434e1eea302d077a08987abdde6905678ebcad4fa649
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.26-2.debian.tar.xz' orc_0.4.26-2.debian.tar.xz 5232 SHA256:fc3b26eb39dde0cbf3d47ceade7ddf22ce613645f5d5879361c02165a9c18206
```

Other potentially useful URLs:

- https://sources.debian.net/src/orc/1:0.4.26-2/ (for browsing the source)
- https://sources.debian.net/src/orc/1:0.4.26-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/orc/1:0.4.26-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.3-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.3-2`
- `p11-kit=0.23.3-2`
- `p11-kit-modules:amd64=0.23.3-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`, `/usr/share/doc/p11-kit/copyright`, `/usr/share/doc/p11-kit-modules/copyright`)

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

### `dpkg` source package: `pango1.0=1.40.5-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.40.5-1`
- `libpangocairo-1.0-0:amd64=1.40.5-1`
- `libpangoft2-1.0-0:amd64=1.40.5-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.40.5-1
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.40.5-1.dsc' pango1.0_1.40.5-1.dsc 3268 SHA256:21b6ba0332f7e690b167eb37ea4eb9c64a95e95b2130a57903112c4d244eb42d
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.40.5.orig.tar.xz' pango1.0_1.40.5.orig.tar.xz 1065152 SHA256:24748140456c42360b07b2c77a1a2e1216d07c056632079557cd4e815b9d01c9
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.40.5-1.debian.tar.xz' pango1.0_1.40.5-1.debian.tar.xz 27304 SHA256:6ec6be5f87ce79ba23e5843e8e271f85ccce9f035b71d373d96a1a2e882cc876
```

Other potentially useful URLs:

- https://sources.debian.net/src/pango1.0/1.40.5-1/ (for browsing the source)
- https://sources.debian.net/src/pango1.0/1.40.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pango1.0/1.40.5-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.24.1-3+deb9u5.dsc' perl_5.24.1-3+deb9u5.dsc 2393 SHA256:d30a446b21afb8f3c0da9bc117244646ef34a05c440a18bcd5c114ee87f8293f
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.24.1.orig.tar.xz' perl_5.24.1.orig.tar.xz 11569284 SHA256:03a77bac4505c270f1890ece75afc7d4b555090b41aa41ea478747e23b2afb3f
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.24.1-3+deb9u5.debian.tar.xz' perl_5.24.1-3+deb9u5.debian.tar.xz 185316 SHA256:fbb78d029b5a9a94e32feba2e360d3628a8a6de90066f90ff22e78d4918aab69
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.24.1-3+deb9u5/ (for browsing the source)
- https://sources.debian.net/src/perl/5.24.1-3+deb9u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.24.1-3+deb9u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.0.0-2`

Binary Packages:

- `pinentry-curses=1.0.0-2`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.0.0-2
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.0.0-2.dsc' pinentry_1.0.0-2.dsc 2591 SHA256:01349d75a92435037a4f4ad252a42cabe7bef774cb8ac6e8c6e24a4107f06e13
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.0.0.orig.tar.bz2' pinentry_1.0.0.orig.tar.bz2 436930 SHA256:1672c2edc1feb036075b187c0773787b2afd0544f55025c645a71b4c2f79275a
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.0.0-2.debian.tar.xz' pinentry_1.0.0-2.debian.tar.xz 16672 SHA256:85e0b03d74a64a08b51f6ffac58a1a07a42499615aa993f367675ef12d0b47fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.0.0-2/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.0.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.0.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pixman=0.34.0-1`

Binary Packages:

- `libpixman-1-0:amd64=0.34.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.34.0-1
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.34.0-1.dsc' pixman_0.34.0-1.dsc 2103 SHA256:157e17c323d461a07f48e570a87228098770fd4388324b2dfcf360bf59ac1e11
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.34.0.orig.tar.gz' pixman_0.34.0.orig.tar.gz 878784 SHA256:21b6b249b51c6800dc9553b65106e1e37d0e25df942c90531d4c3997aa20a88e
'http://deb.debian.org/debian/pool/main/p/pixman/pixman_0.34.0-1.diff.gz' pixman_0.34.0-1.diff.gz 315394 SHA256:a230def25913d56f9f13e4dbb1014214f84e85fe502c943d560f4335cfc1c5cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/pixman/0.34.0-1/ (for browsing the source)
- https://sources.debian.net/src/pixman/0.34.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pixman/0.34.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `poppler-data=0.4.7-8`

Binary Packages:

- `poppler-data=0.4.7-8`

Licenses: (parsed from: `/usr/share/doc/poppler-data/copyright`)

- `BSD-3-cluase`
- `GPL-2`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris poppler-data=0.4.7-8
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.7-8.dsc' poppler-data_0.4.7-8.dsc 2002 SHA256:3660fc4d5a0755cc504d74f4139316c37cc280430fffb7d25eb9a827a6c0534d
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.7.orig-ai0.tar.gz' poppler-data_0.4.7.orig-ai0.tar.gz 3515 SHA256:755a3a7cec6019b7cb6a7ac89828820e90d5105e66ebc2a7aacecacfb3ed4f1d
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.7.orig.tar.gz' poppler-data_0.4.7.orig.tar.gz 4182339 SHA256:e752b0d88a7aba54574152143e7bf76436a7ef51977c55d6bd9a48dccde3a7de
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.7-8.debian.tar.xz' poppler-data_0.4.7-8.debian.tar.xz 9032 SHA256:e38af64cb05bd17b927eb8ba1b35bfb35e2e01dbad323f052e816762bccae134
```

Other potentially useful URLs:

- https://sources.debian.net/src/poppler-data/0.4.7-8/ (for browsing the source)
- https://sources.debian.net/src/poppler-data/0.4.7-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/poppler-data/0.4.7-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `poppler=0.48.0-2+deb9u2`

Binary Packages:

- `libpoppler64:amd64=0.48.0-2+deb9u2`
- `poppler-utils=0.48.0-2+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libpoppler64/copyright`, `/usr/share/doc/poppler-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris poppler=0.48.0-2+deb9u2
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_0.48.0-2+deb9u2.dsc' poppler_0.48.0-2+deb9u2.dsc 3408 SHA256:658eab614c16d776952faf31b3a442f6e2bc28802a8f523fe4e958f6b5976efe
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_0.48.0.orig.tar.xz' poppler_0.48.0.orig.tar.xz 1684164 SHA256:85a003968074c85d8e13bf320ec47cef647b496b56dcff4c790b34e5482fef93
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_0.48.0-2+deb9u2.debian.tar.xz' poppler_0.48.0-2+deb9u2.debian.tar.xz 40808 SHA256:5842d61f5bda84dac0e624ec0aef684b2beab70491e1e0c1c6b8cfd70485997c
```

Other potentially useful URLs:

- https://sources.debian.net/src/poppler/0.48.0-2+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/poppler/0.48.0-2+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/poppler/0.48.0-2+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.12-3+deb9u1`

Binary Packages:

- `libprocps6:amd64=2:3.3.12-3+deb9u1`
- `procps=2:3.3.12-3+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libprocps6/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.12-3+deb9u1
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.12-3+deb9u1.dsc' procps_3.3.12-3+deb9u1.dsc 2333 SHA256:0a9977b3577de224b4db2c957d8825faca13e131bd79daace4a9f3b4cbdeb067
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.12.orig.tar.xz' procps_3.3.12.orig.tar.xz 840540 SHA256:042fcc93e1850aee4c193c51c03f369293fb64fe47e37b38852be6693d12a3af
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.12-3+deb9u1.debian.tar.xz' procps_3.3.12-3+deb9u1.debian.tar.xz 33320 SHA256:2645283a93fe698eb93a560ee0fd8897ecc7a8997bb65e2e1537f91dc788e3e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.12-3+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.12-3+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.12-3+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `psmisc=22.21-2.1`

Binary Packages:

- `psmisc=22.21-2.1+b2`

Licenses: (parsed from: `/usr/share/doc/psmisc/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris psmisc=22.21-2.1
'http://deb.debian.org/debian/pool/main/p/psmisc/psmisc_22.21-2.1.dsc' psmisc_22.21-2.1.dsc 1348 SHA256:3e1e9615bbaa521b8ef054b26faded392179f1919b62dec901cf820efab65404
'http://deb.debian.org/debian/pool/main/p/psmisc/psmisc_22.21.orig.tar.gz' psmisc_22.21.orig.tar.gz 457702 SHA256:97323cad619210845b696d7d722c383852b2acb5c49b5b0852c4f29c77a8145a
'http://deb.debian.org/debian/pool/main/p/psmisc/psmisc_22.21-2.1.debian.tar.xz' psmisc_22.21-2.1.debian.tar.xz 6824 SHA256:b4d5fd3e3c4f402c265476cf1b7ef1bf360c810ea11e74d333fade6f44b9d761
```

Other potentially useful URLs:

- https://sources.debian.net/src/psmisc/22.21-2.1/ (for browsing the source)
- https://sources.debian.net/src/psmisc/22.21-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/psmisc/22.21-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pulseaudio=10.0-1+deb9u1`

Binary Packages:

- `libpulse0:amd64=10.0-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libpulse0/copyright`)

- `AGPL-3+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris pulseaudio=10.0-1+deb9u1
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_10.0-1+deb9u1.dsc' pulseaudio_10.0-1+deb9u1.dsc 3822 SHA256:d14a46f11e0908b8bfd0dafd167db84a75beabf56ae723c0db6d59bedfff7005
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_10.0.orig.tar.xz' pulseaudio_10.0.orig.tar.xz 1608040 SHA256:a3186824de9f0d2095ded5d0d0db0405dc73133983c2fbb37291547e37462f57
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_10.0-1+deb9u1.debian.tar.xz' pulseaudio_10.0-1+deb9u1.debian.tar.xz 41516 SHA256:7fd5a9de718e264c9de828a03594edcdf3ec59dcf470c7abe46097448b5315a8
```

Other potentially useful URLs:

- https://sources.debian.net/src/pulseaudio/10.0-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/pulseaudio/10.0-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pulseaudio/10.0-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pwgen=2.07-1.1`

Binary Packages:

- `pwgen=2.07-1.1+b1`

Licenses: (parsed from: `/usr/share/doc/pwgen/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris pwgen=2.07-1.1
'http://deb.debian.org/debian/pool/main/p/pwgen/pwgen_2.07-1.1.dsc' pwgen_2.07-1.1.dsc 1684 SHA256:ddcc8975a1c77be9861a54899289b4a0529aa340a59d08d03884ef1c9eb7aed5
'http://deb.debian.org/debian/pool/main/p/pwgen/pwgen_2.07.orig.tar.gz' pwgen_2.07.orig.tar.gz 53513 SHA256:eb74593f58296c21c71cd07933e070492e9222b79cedf81d1a02ce09c0e11556
'http://deb.debian.org/debian/pool/main/p/pwgen/pwgen_2.07-1.1.debian.tar.xz' pwgen_2.07-1.1.debian.tar.xz 5980 SHA256:49c4d5b11bd7d3a2517e2cfa0f2a4c3cfd5b005c96ff134daa7862acd8aec890
```

Other potentially useful URLs:

- https://sources.debian.net/src/pwgen/2.07-1.1/ (for browsing the source)
- https://sources.debian.net/src/pwgen/2.07-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pwgen/2.07-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python-defaults=2.7.13-2`

Binary Packages:

- `libpython-stdlib:amd64=2.7.13-2`
- `python=2.7.13-2`
- `python-minimal=2.7.13-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.13-2
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.13-2.dsc' python-defaults_2.7.13-2.dsc 2677 SHA256:80d5452cde16052caa5b9c3880ed067c3d4f2e60485a56947531a6650f6e7d94
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.13-2.tar.gz' python-defaults_2.7.13-2.tar.gz 273915 SHA256:aa376f54a9b2ca59b6f051ce0b4320d95ef60f114f90d98a90e510c3968b416a
```

Other potentially useful URLs:

- https://sources.debian.net/src/python-defaults/2.7.13-2/ (for browsing the source)
- https://sources.debian.net/src/python-defaults/2.7.13-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python-defaults/2.7.13-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python2.7=2.7.13-2+deb9u3`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.13-2+deb9u3`
- `libpython2.7-stdlib:amd64=2.7.13-2+deb9u3`
- `python2.7=2.7.13-2+deb9u3`
- `python2.7-minimal=2.7.13-2+deb9u3`

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
$ apt-get source -qq --print-uris python2.7=2.7.13-2+deb9u3
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.13-2+deb9u3.dsc' python2.7_2.7.13-2+deb9u3.dsc 3370 SHA256:07f864cef82aaf3741af4c89aa5bcc595c56c283c3ff61630c36171ce5aac9f3
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.13.orig.tar.gz' python2.7_2.7.13.orig.tar.gz 17076672 SHA256:a4f05a0720ce0fd92626f0278b6b433eee9a6173ddf2bced7957dfb599a5ece1
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.13-2+deb9u3.diff.gz' python2.7_2.7.13-2+deb9u3.diff.gz 284882 SHA256:4e7d5d372cb78eadc0fafa461a579a658ee245fcc1142234561406b45193c087
```

Other potentially useful URLs:

- https://sources.debian.net/src/python2.7/2.7.13-2+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/python2.7/2.7.13-2+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python2.7/2.7.13-2+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.5.3-1`

Binary Packages:

- `libpython3-stdlib:amd64=3.5.3-1`
- `python3=3.5.3-1`
- `python3-minimal=3.5.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.5.3-1
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.5.3-1.dsc' python3-defaults_3.5.3-1.dsc 2776 SHA256:2bec1dd8a5836d5a19fbbd48d7c49aec40642669036297a34bbfd8b0b2d61439
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.5.3-1.tar.gz' python3-defaults_3.5.3-1.tar.gz 1007580 SHA256:aa58a9fceb9975f71be344e594393cf3384dd6b55d9541abf0bee7c5dce8ec15
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3-defaults/3.5.3-1/ (for browsing the source)
- https://sources.debian.net/src/python3-defaults/3.5.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3-defaults/3.5.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3.5=3.5.3-1+deb9u1`

Binary Packages:

- `libpython3.5:amd64=3.5.3-1+deb9u1`
- `libpython3.5-minimal:amd64=3.5.3-1+deb9u1`
- `libpython3.5-stdlib:amd64=3.5.3-1+deb9u1`
- `python3.5=3.5.3-1+deb9u1`
- `python3.5-minimal=3.5.3-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libpython3.5/copyright`, `/usr/share/doc/libpython3.5-minimal/copyright`, `/usr/share/doc/libpython3.5-stdlib/copyright`, `/usr/share/doc/python3.5/copyright`, `/usr/share/doc/python3.5-minimal/copyright`)

- `* Permission to use this software in any way is granted without`
- `Apache`
- `Apache-2`
- `Apache-2.0`
- `By obtaining, using, and/or copying this software and/or its`
- `Expat`
- `GPL-2`
- `ISC`
- `LGPL-2.1+`
- `PSF-2`
- `Permission  is  hereby granted,  free  of charge,  to  any person`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Permission to use, copy, modify,`
- `Python`
- `Redistribution`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `binary forms, with`
- `distribute this software`
- `distribute this software and`
- `distribute this software for any`
- `implied`
- `its`
- `see above, some license as Python`
- `use in source`
- `without`

Source:

```console
$ apt-get source -qq --print-uris python3.5=3.5.3-1+deb9u1
'http://deb.debian.org/debian/pool/main/p/python3.5/python3.5_3.5.3-1+deb9u1.dsc' python3.5_3.5.3-1+deb9u1.dsc 3370 SHA256:ab783e665c7943425b4e14d0473806c5a8d4ceabde25958a77b49fb5fd47f8c6
'http://deb.debian.org/debian/pool/main/p/python3.5/python3.5_3.5.3.orig.tar.xz' python3.5_3.5.3.orig.tar.xz 15213396 SHA256:eefe2ad6575855423ab630f5b51a8ef6e5556f774584c06beab4926f930ddbb0
'http://deb.debian.org/debian/pool/main/p/python3.5/python3.5_3.5.3-1+deb9u1.debian.tar.xz' python3.5_3.5.3-1+deb9u1.debian.tar.xz 221400 SHA256:04f498e2a049fd95e5f152ff5a2242d1fe99084fb44eba4df0a6758512d731a4
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.5/3.5.3-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/python3.5/3.5.3-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.5/3.5.3-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `raptor2=2.0.14-1`

Binary Packages:

- `libraptor2-0:amd64=2.0.14-1+b1`

Licenses: (parsed from: `/usr/share/doc/libraptor2-0/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris raptor2=2.0.14-1
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14-1.dsc' raptor2_2.0.14-1.dsc 1455 SHA256:9cee0bfac55f8b7fe7d72e3780de235f4dd5309ca89e5afaed302dfed0e1221a
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14.orig.tar.gz' raptor2_2.0.14.orig.tar.gz 1877454 SHA256:cb447b7c684cbe60f1266d622691fd20fdcf7b91f4a470c6de5fc8e8961df1b2
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14-1.debian.tar.xz' raptor2_2.0.14-1.debian.tar.xz 7624 SHA256:2b13e72202c99570f225f378318cdceca38ee130e7a24e46881e7672ea2b8758
```

Other potentially useful URLs:

- https://sources.debian.net/src/raptor2/2.0.14-1/ (for browsing the source)
- https://sources.debian.net/src/raptor2/2.0.14-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/raptor2/2.0.14-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rasqal=0.9.32-1`

Binary Packages:

- `librasqal3:amd64=0.9.32-1+b1`

Licenses: (parsed from: `/usr/share/doc/librasqal3/copyright`)

- `Apache-2.0`
- `Apache-2.0+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris rasqal=0.9.32-1
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.32-1.dsc' rasqal_0.9.32-1.dsc 1360 SHA256:fd0ecaa94c86647ee855def087955b01f0bfe2933c8471c83d2094d7b60f84ce
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.32.orig.tar.gz' rasqal_0.9.32.orig.tar.gz 1544623 SHA256:eeba03218e3b7dfa033934d523a1a64671a9a0f64eadc38a01e4b43367be2e8f
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.32-1.debian.tar.xz' rasqal_0.9.32-1.debian.tar.xz 5888 SHA256:02c3a4303f0a5afb84de6a06303aac1684ed900eb49a5f517222734b3d0caea6
```

Other potentially useful URLs:

- https://sources.debian.net/src/rasqal/0.9.32-1/ (for browsing the source)
- https://sources.debian.net/src/rasqal/0.9.32-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rasqal/0.9.32-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `redland=1.0.17-1.1`

Binary Packages:

- `librdf0:amd64=1.0.17-1.1`

Licenses: (parsed from: `/usr/share/doc/librdf0/copyright`)

- `Apache-2.0`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris redland=1.0.17-1.1
'http://deb.debian.org/debian/pool/main/r/redland/redland_1.0.17-1.1.dsc' redland_1.0.17-1.1.dsc 2378 SHA256:da5aaa6ca35a38f5d59a42b4c54f43101de74feaffbee69b0619ddb2ff38e944
'http://deb.debian.org/debian/pool/main/r/redland/redland_1.0.17.orig.tar.gz' redland_1.0.17.orig.tar.gz 1621566 SHA256:de1847f7b59021c16bdc72abb4d8e2d9187cd6124d69156f3326dd34ee043681
'http://deb.debian.org/debian/pool/main/r/redland/redland_1.0.17-1.1.debian.tar.xz' redland_1.0.17-1.1.debian.tar.xz 8284 SHA256:3bf4791aa5aa82dd0e32d76c9fd8539652769b8fb60cd9a04831afab78eb4747
```

Other potentially useful URLs:

- https://sources.debian.net/src/redland/1.0.17-1.1/ (for browsing the source)
- https://sources.debian.net/src/redland/1.0.17-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/redland/1.0.17-1.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `rubberband=1.8.1-7`

Binary Packages:

- `librubberband2:amd64=1.8.1-7`

Licenses: (parsed from: `/usr/share/doc/librubberband2/copyright`)

- `GPL-2`
- `GPL-2+`
- `other-1`
- `other-bsd-3-clause-kissft`
- `other-bsd-3-clause-speex`
- `other-bsd-4-clause-1`
- `other-bsd-4-clause-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris rubberband=1.8.1-7
'http://deb.debian.org/debian/pool/main/r/rubberband/rubberband_1.8.1-7.dsc' rubberband_1.8.1-7.dsc 2396 SHA256:38f8fd134baffbe1dfdc9a72fc5bd914facc8e733b4e9342ab5d6d4d7b61c129
'http://deb.debian.org/debian/pool/main/r/rubberband/rubberband_1.8.1.orig.tar.bz2' rubberband_1.8.1.orig.tar.bz2 177501 SHA256:ff0c63b0b5ce41f937a8a3bc560f27918c5fe0b90c6bc1cb70829b86ada82b75
'http://deb.debian.org/debian/pool/main/r/rubberband/rubberband_1.8.1-7.debian.tar.xz' rubberband_1.8.1-7.debian.tar.xz 9204 SHA256:5b396c169ed2b0d9bae40de2be1d0ed04a6bc4cc0fb170031ec38b9be2df7041
```

Other potentially useful URLs:

- https://sources.debian.net/src/rubberband/1.8.1-7/ (for browsing the source)
- https://sources.debian.net/src/rubberband/1.8.1-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rubberband/1.8.1-7/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `serf=1.3.9-3+deb9u1`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-3+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-3+deb9u1/


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

### `dpkg` source package: `shared-mime-info=1.8-1+deb9u1`

Binary Packages:

- `shared-mime-info=1.8-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.8-1+deb9u1
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.8-1+deb9u1.dsc' shared-mime-info_1.8-1+deb9u1.dsc 2266 SHA256:36646ba27a24b8a312a49d41b58831c4352c2723fd4f14f9acf6762f3c1e3a19
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.8.orig.tar.xz' shared-mime-info_1.8.orig.tar.xz 589444 SHA256:2af55ef1a0319805b74ab40d331a3962c905477d76c086f49e34dc96363589e9
'http://deb.debian.org/debian/pool/main/s/shared-mime-info/shared-mime-info_1.8-1+deb9u1.debian.tar.xz' shared-mime-info_1.8-1+deb9u1.debian.tar.xz 10384 SHA256:60496e642e6dea89268e1cadaff1cda885351d75d32332fa1cf2d7f7110def20
```

Other potentially useful URLs:

- https://sources.debian.net/src/shared-mime-info/1.8-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/shared-mime-info/1.8-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shared-mime-info/1.8-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shine=3.1.0-5`

Binary Packages:

- `libshine3:amd64=3.1.0-5`

Licenses: (parsed from: `/usr/share/doc/libshine3/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris shine=3.1.0-5
'http://deb.debian.org/debian/pool/main/s/shine/shine_3.1.0-5.dsc' shine_3.1.0-5.dsc 2033 SHA256:b92f2b27e0a0e64f6025e18d0d9908c0c88df3c798770dfd0ea169fe701efe55
'http://deb.debian.org/debian/pool/main/s/shine/shine_3.1.0.orig.tar.gz' shine_3.1.0.orig.tar.gz 1275236 SHA256:6c5310bda766b116ed2415d639a27e5e11040e068b4b2db6bd733333e620cb4f
'http://deb.debian.org/debian/pool/main/s/shine/shine_3.1.0-5.debian.tar.xz' shine_3.1.0-5.debian.tar.xz 3520 SHA256:87f9bcafcb40551889dd73da54ecdb2865fd5e3391efef6982061b970b5f9e0f
```

Other potentially useful URLs:

- https://sources.debian.net/src/shine/3.1.0-5/ (for browsing the source)
- https://sources.debian.net/src/shine/3.1.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shine/3.1.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `six=1.10.0-3`

Binary Packages:

- `python-six=1.10.0-3`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.10.0-3
'http://deb.debian.org/debian/pool/main/s/six/six_1.10.0-3.dsc' six_1.10.0-3.dsc 2158 SHA256:71f2d5ff8b999c471cc2e92712befe482351a5ae226321e0e795bc683c8729cb
'http://deb.debian.org/debian/pool/main/s/six/six_1.10.0.orig.tar.gz' six_1.10.0.orig.tar.gz 29630 SHA256:105f8d68616f8248e24bf0e9372ef04d3cc10104f1980f54d57b2ce73a5ad56a
'http://deb.debian.org/debian/pool/main/s/six/six_1.10.0-3.debian.tar.xz' six_1.10.0-3.debian.tar.xz 3668 SHA256:860cc57244ea4e69eb4ee3ad1b823472c20d868c1cc25745b236ba6c9e1f3563
```

Other potentially useful URLs:

- https://sources.debian.net/src/six/1.10.0-3/ (for browsing the source)
- https://sources.debian.net/src/six/1.10.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/six/1.10.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `slang2=2.3.1-5`

Binary Packages:

- `libslang2:amd64=2.3.1-5`

Licenses: (parsed from: `/usr/share/doc/libslang2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris slang2=2.3.1-5
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.1-5.dsc' slang2_2.3.1-5.dsc 2312 SHA256:32cb921b59687559485d15f2c8ef84cde98af2dad663c3397a89c26d77b44af0
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.1.orig.tar.xz' slang2_2.3.1.orig.tar.xz 1287100 SHA256:3bcc81bbbfbe1f458162f67caa7fa8ad46af57f804bd64283ea8aff382d881b6
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.1-5.debian.tar.xz' slang2_2.3.1-5.debian.tar.xz 22160 SHA256:3c4efbda9f8d3df955f0c743fbaa1063651f3f48a084c49f19983aa470306af8
```

Other potentially useful URLs:

- https://sources.debian.net/src/slang2/2.3.1-5/ (for browsing the source)
- https://sources.debian.net/src/slang2/2.3.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/slang2/2.3.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `snappy=1.1.3-3`

Binary Packages:

- `libsnappy1v5:amd64=1.1.3-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris snappy=1.1.3-3
'http://deb.debian.org/debian/pool/main/s/snappy/snappy_1.1.3-3.dsc' snappy_1.1.3-3.dsc 1803 SHA256:05dceab1ed94b6bc1da1f39468028b31d16607504dd31bb792ff9a08e9b7b8d6
'http://deb.debian.org/debian/pool/main/s/snappy/snappy_1.1.3.orig.tar.gz' snappy_1.1.3.orig.tar.gz 1509026 SHA256:2f1e82adf0868c9e26a5a7a3115111b6da7e432ddbac268a7ca2fae2a247eef3
'http://deb.debian.org/debian/pool/main/s/snappy/snappy_1.1.3-3.debian.tar.xz' snappy_1.1.3-3.debian.tar.xz 4360 SHA256:1fce7fccdfaf714065a6ee4ad60943f7f30d004059fd98d5a4dcc464ad998623
```

Other potentially useful URLs:

- https://sources.debian.net/src/snappy/1.1.3-3/ (for browsing the source)
- https://sources.debian.net/src/snappy/1.1.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/snappy/1.1.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sndio=1.1.0-3`

Binary Packages:

- `libsndio6.1:amd64=1.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libsndio6.1/copyright`)

- `ISC`
- `ISC-packaging`

Source:

```console
$ apt-get source -qq --print-uris sndio=1.1.0-3
'http://deb.debian.org/debian/pool/main/s/sndio/sndio_1.1.0-3.dsc' sndio_1.1.0-3.dsc 1861 SHA256:31f5b892d023550d3b4657ee74982a6053102db4869c8c8c23d3c7a8aaf2752b
'http://deb.debian.org/debian/pool/main/s/sndio/sndio_1.1.0.orig.tar.gz' sndio_1.1.0.orig.tar.gz 121018 SHA256:fcd7f845ff70f38c2898d737450b8aa3e1bb0afb9d147e8429ef22c0b2c2db57
'http://deb.debian.org/debian/pool/main/s/sndio/sndio_1.1.0-3.debian.tar.xz' sndio_1.1.0-3.debian.tar.xz 5196 SHA256:c0e5e04946b01d04f131223a9c9ee6e204ee325b50419e2160eed19a4d49d8aa
```

Other potentially useful URLs:

- https://sources.debian.net/src/sndio/1.1.0-3/ (for browsing the source)
- https://sources.debian.net/src/sndio/1.1.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sndio/1.1.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `speex=1.2~rc1.2-1`

Binary Packages:

- `libspeex1:amd64=1.2~rc1.2-1+b2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris speex=1.2~rc1.2-1
'http://deb.debian.org/debian/pool/main/s/speex/speex_1.2~rc1.2-1.dsc' speex_1.2~rc1.2-1.dsc 1540 SHA256:faf1fa4e640bf3ba153ebe58f8f40824437ef303b276e04ef15b3841199dce43
'http://deb.debian.org/debian/pool/main/s/speex/speex_1.2~rc1.2.orig.tar.gz' speex_1.2~rc1.2.orig.tar.gz 1069339 SHA256:8320fb86a024dfe1b6a78a7d57bc2388e5f8cb7f2fa10c946db2704e1e5d2805
'http://deb.debian.org/debian/pool/main/s/speex/speex_1.2~rc1.2-1.diff.gz' speex_1.2~rc1.2-1.diff.gz 9750 SHA256:6c549549a9a8d1b24f12ddbfa706f1e078ad5d9fed9a9fe584f9d08b47458930
```

Other potentially useful URLs:

- https://sources.debian.net/src/speex/1.2~rc1.2-1/ (for browsing the source)
- https://sources.debian.net/src/speex/1.2~rc1.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/speex/1.2~rc1.2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `subversion=1.9.5-1+deb9u5`

Binary Packages:

- `libsvn1:amd64=1.9.5-1+deb9u5`
- `subversion=1.9.5-1+deb9u5`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris subversion=1.9.5-1+deb9u5
'http://security.debian.org/debian-security/pool/updates/main/s/subversion/subversion_1.9.5-1+deb9u5.dsc' subversion_1.9.5-1+deb9u5.dsc 2947 SHA256:8f2758d5a5b1f8611612c0ce7af6de09b3c125c7dafba772c0a8a09acb916c35
'http://security.debian.org/debian-security/pool/updates/main/s/subversion/subversion_1.9.5.orig.tar.gz' subversion_1.9.5.orig.tar.gz 10615674 SHA256:280ba586c5d51d7b976b65d22d5e8e42f3908ed1c968d71120dcf534ce857a83
'http://security.debian.org/debian-security/pool/updates/main/s/subversion/subversion_1.9.5-1+deb9u5.diff.gz' subversion_1.9.5-1+deb9u5.diff.gz 2548586 SHA256:3cc8c1e90d4367825b23ddce27b7c3a80a60e1e1bf99cd70bb995255eef1ace1
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.9.5-1+deb9u5/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.9.5-1+deb9u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.9.5-1+deb9u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `suitesparse=1:4.5.4-1`

Binary Packages:

- `libcolamd2:amd64=1:4.5.4-1`
- `libsuitesparseconfig4:amd64=1:4.5.4-1`

Licenses: (parsed from: `/usr/share/doc/libcolamd2/copyright`, `/usr/share/doc/libsuitesparseconfig4/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `permissive`
- `permissive-2`

Source:

```console
$ apt-get source -qq --print-uris suitesparse=1:4.5.4-1
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_4.5.4-1.dsc' suitesparse_4.5.4-1.dsc 2793 SHA256:540c9b25e3afc8d4d3c5e0764d2467828f78beb4cc7e2c23bf0b74ff29a68c8a
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_4.5.4.orig.tar.gz' suitesparse_4.5.4.orig.tar.gz 30309663 SHA256:698b5c455645bb1ad29a185f0d52025f3bd7cb7261e182c8878b0eb60567a714
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_4.5.4-1.debian.tar.xz' suitesparse_4.5.4-1.debian.tar.xz 17528 SHA256:ffe6743f2dbf43142c6e87ad506778439f79dd847eae022e9bb294123e6076aa
```

Other potentially useful URLs:

- https://sources.debian.net/src/suitesparse/1:4.5.4-1/ (for browsing the source)
- https://sources.debian.net/src/suitesparse/1:4.5.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/suitesparse/1:4.5.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd-shim=10-3`

Binary Packages:

- `systemd-shim=10-3`

Licenses: (parsed from: `/usr/share/doc/systemd-shim/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris systemd-shim=10-3
'http://deb.debian.org/debian/pool/main/s/systemd-shim/systemd-shim_10-3.dsc' systemd-shim_10-3.dsc 1805 SHA256:c9e672cbde072b53853774ece75d3562fb539f80feb7f1aa9ce7936fd8a59c6f
'http://deb.debian.org/debian/pool/main/s/systemd-shim/systemd-shim_10.orig.tar.gz' systemd-shim_10.orig.tar.gz 26669 SHA256:1583c8cd99f8e02ebf29490afcec59a6041e556c895c11a1fb68291879262736
'http://deb.debian.org/debian/pool/main/s/systemd-shim/systemd-shim_10-3.debian.tar.xz' systemd-shim_10-3.debian.tar.xz 8948 SHA256:a74e2cacfae5b6db343472742d5d63dfafd90f77bd0210f9e50331b1b445d6e9
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd-shim/10-3/ (for browsing the source)
- https://sources.debian.net/src/systemd-shim/10-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd-shim/10-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=232-25+deb9u12`

Binary Packages:

- `libpam-systemd:amd64=232-25+deb9u12`
- `libsystemd0:amd64=232-25+deb9u12`
- `libudev1:amd64=232-25+deb9u12`
- `systemd=232-25+deb9u12`

Licenses: (parsed from: `/usr/share/doc/libpam-systemd/copyright`, `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`, `/usr/share/doc/systemd/copyright`)

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

### `dpkg` source package: `tbb=4.3~20150611-2`

Binary Packages:

- `libtbb2:amd64=4.3~20150611-2`

Licenses: (parsed from: `/usr/share/doc/libtbb2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris tbb=4.3~20150611-2
'http://deb.debian.org/debian/pool/main/t/tbb/tbb_4.3~20150611-2.dsc' tbb_4.3~20150611-2.dsc 2003 SHA256:7fee10d93d59790e0c3b62ddd65200c31b14461bfd2ed2a124811c84290bfa86
'http://deb.debian.org/debian/pool/main/t/tbb/tbb_4.3~20150611.orig.tar.xz' tbb_4.3~20150611.orig.tar.xz 1745460 SHA256:1de251c3743345889c246b4b081a2f8dd27dbed01b567f5ce42fb2231983a75b
'http://deb.debian.org/debian/pool/main/t/tbb/tbb_4.3~20150611-2.debian.tar.xz' tbb_4.3~20150611-2.debian.tar.xz 10780 SHA256:354756a271a981b963d4821855ee9011e8f89375ed14f8ba734168cf1770f6d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/tbb/4.3~20150611-2/ (for browsing the source)
- https://sources.debian.net/src/tbb/4.3~20150611-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tbb/4.3~20150611-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tcp-wrappers=7.6.q-26`

Binary Packages:

- `libwrap0:amd64=7.6.q-26`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcp-wrappers=7.6.q-26
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-26.dsc' tcp-wrappers_7.6.q-26.dsc 1746 SHA256:eba34e1c727c60e2ca8beda71b2a256d2981ebf044627fd912d9d5ce03b05406
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q.orig.tar.gz' tcp-wrappers_7.6.q.orig.tar.gz 99438 SHA256:9543d7adedf78a6de0b221ccbbd1952e08b5138717f4ade814039bb489a4315d
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-26.debian.tar.xz' tcp-wrappers_7.6.q-26.debian.tar.xz 36116 SHA256:48a27f7a94607308c2c23227403309de25acabd0b5f3f75278677f4e53848db5
```

Other potentially useful URLs:

- https://sources.debian.net/src/tcp-wrappers/7.6.q-26/ (for browsing the source)
- https://sources.debian.net/src/tcp-wrappers/7.6.q-26/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tcp-wrappers/7.6.q-26/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.0.8-2+deb9u4`

Binary Packages:

- `libtiff5:amd64=4.0.8-2+deb9u4`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.8-2+deb9u4
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.0.8-2+deb9u4.dsc' tiff_4.0.8-2+deb9u4.dsc 2185 SHA256:7f2a8ae92ea3ea871eb9baca399e589d256163e9689a64ac41ac64253c84b0b7
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.0.8.orig.tar.gz' tiff_4.0.8.orig.tar.gz 2065574 SHA256:59d7a5a8ccd92059913f246877db95a2918e6c04fb9d43fd74e5c3390dac2910
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.0.8-2+deb9u4.debian.tar.xz' tiff_4.0.8-2+deb9u4.debian.tar.xz 32508 SHA256:2096e012af91b8503e656212409c438ad2105fd42c22e8f811fe5ef25810342d
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.0.8-2+deb9u4/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.0.8-2+deb9u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.0.8-2+deb9u4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `twolame=0.3.13-2`

Binary Packages:

- `libtwolame0:amd64=0.3.13-2`

Licenses: (parsed from: `/usr/share/doc/libtwolame0/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris twolame=0.3.13-2
'http://deb.debian.org/debian/pool/main/t/twolame/twolame_0.3.13-2.dsc' twolame_0.3.13-2.dsc 1909 SHA256:628f2a4bb9ccf44f8b3f2d21697d09d90e23d56d8f126c21e37a058301188beb
'http://deb.debian.org/debian/pool/main/t/twolame/twolame_0.3.13.orig.tar.gz' twolame_0.3.13.orig.tar.gz 660415 SHA256:98f332f48951f47f23f70fd0379463aff7d7fb26f07e1e24e42ddef22cc6112a
'http://deb.debian.org/debian/pool/main/t/twolame/twolame_0.3.13-2.debian.tar.xz' twolame_0.3.13-2.debian.tar.xz 4096 SHA256:6c3a47d6f1e6cf4094d8ac4a70c1f44262df2de1ee5bace26d050cad3204a753
```

Other potentially useful URLs:

- https://sources.debian.net/src/twolame/0.3.13-2/ (for browsing the source)
- https://sources.debian.net/src/twolame/0.3.13-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/twolame/0.3.13-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2019c-0+deb9u1`

Binary Packages:

- `tzdata=2019c-0+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2019c-0+deb9u1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c-0+deb9u1.dsc' tzdata_2019c-0+deb9u1.dsc 2270 SHA256:5e6c0a29f32b80acf5e2a6bc739a45f19f1a47a729e5bbcb9e90bc8cbfeaad34
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c.orig.tar.gz' tzdata_2019c.orig.tar.gz 392087 SHA256:79c7806dab09072308da0e3d22c37d3b245015a591891ea147d3b133b60ffc7c
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c.orig.tar.gz.asc' tzdata_2019c.orig.tar.gz.asc 833 SHA256:cd31deaeee229d45e4f4b973441189e7619ef81679359e9c8b47b2a87aaf6a07
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c-0+deb9u1.debian.tar.xz' tzdata_2019c-0+deb9u1.debian.tar.xz 101948 SHA256:96a84b44365eadc4007b4e6d7928061e4f014d0c3de0ff1b711ccda8057a405f
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2019c-0+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2019c-0+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2019c-0+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ucf=3.0036`

Binary Packages:

- `ucf=3.0036`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0036
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0036.dsc' ucf_3.0036.dsc 1343 SHA256:e67a8a3012ac357c7759dabd93d258422b1003bad8c3f17f25fc2a289eeda3bb
'http://deb.debian.org/debian/pool/main/u/ucf/ucf_3.0036.tar.xz' ucf_3.0036.tar.xz 65020 SHA256:34aa44416106f1205376918386b2896edf21dd42b633133b5f8fedecae17fca8
```

Other potentially useful URLs:

- https://sources.debian.net/src/ucf/3.0036/ (for browsing the source)
- https://sources.debian.net/src/ucf/3.0036/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ucf/3.0036/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ufraw=0.22-1.1`

Binary Packages:

- `ufraw=0.22-1.1`
- `ufraw-batch=0.22-1.1`

Licenses: (parsed from: `/usr/share/doc/ufraw/copyright`, `/usr/share/doc/ufraw-batch/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ufraw=0.22-1.1
'http://deb.debian.org/debian/pool/main/u/ufraw/ufraw_0.22-1.1.dsc' ufraw_0.22-1.1.dsc 1972 SHA256:e76403c2fa62b9a1b99f47782bf44d307543cc74a067523345652b1738defe45
'http://deb.debian.org/debian/pool/main/u/ufraw/ufraw_0.22.orig.tar.gz' ufraw_0.22.orig.tar.gz 1103554 SHA256:f7abd28ce587db2a74b4c54149bd8a2523a7ddc09bedf4f923246ff0ae09a25e
'http://deb.debian.org/debian/pool/main/u/ufraw/ufraw_0.22-1.1.debian.tar.xz' ufraw_0.22-1.1.debian.tar.xz 7724 SHA256:9790b8f5d65c5d68bf6ab4d60d5306ad64f92205d2eba88a9f177b90bfaad30e
```

Other potentially useful URLs:

- https://sources.debian.net/src/ufraw/0.22-1.1/ (for browsing the source)
- https://sources.debian.net/src/ufraw/0.22-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ufraw/0.22-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unzip=6.0-21+deb9u2`

Binary Packages:

- `unzip=6.0-21+deb9u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-21+deb9u2
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-21+deb9u2.dsc' unzip_6.0-21+deb9u2.dsc 1372 SHA256:9894c31ba2999c72e81593ba0ecb6ee621c2992071427fc790981df6d9f56605
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-21+deb9u2.debian.tar.xz' unzip_6.0-21+deb9u2.debian.tar.xz 22984 SHA256:8caf2e849fc90bdb22e9c338c64800c98c7179345cbce47d65c8dda4efc8942b
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-21+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-21+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-21+deb9u2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `wavpack=5.0.0-2+deb9u2`

Binary Packages:

- `libwavpack1:amd64=5.0.0-2+deb9u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris wavpack=5.0.0-2+deb9u2
'http://deb.debian.org/debian/pool/main/w/wavpack/wavpack_5.0.0-2+deb9u2.dsc' wavpack_5.0.0-2+deb9u2.dsc 2154 SHA256:14f110f0d6ef0ac18475a16106e49a53f009423eab3472cd30021d30f824c4fc
'http://deb.debian.org/debian/pool/main/w/wavpack/wavpack_5.0.0.orig.tar.bz2' wavpack_5.0.0.orig.tar.bz2 807953 SHA256:918d7e32a19598df543b17fff840b10a0880f87296f9e32af454d256b6a64049
'http://deb.debian.org/debian/pool/main/w/wavpack/wavpack_5.0.0-2+deb9u2.debian.tar.xz' wavpack_5.0.0-2+deb9u2.debian.tar.xz 8856 SHA256:e4aff1c196aa664bbd1c251be1fc09081e5b66ef929eb3e3fffb2100f65356e4
```

Other potentially useful URLs:

- https://sources.debian.net/src/wavpack/5.0.0-2+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/wavpack/5.0.0-2+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wavpack/5.0.0-2+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wayland=1.12.0-1+deb9u1`

Binary Packages:

- `libwayland-client0:amd64=1.12.0-1+deb9u1`
- `libwayland-cursor0:amd64=1.12.0-1+deb9u1`
- `libwayland-server0:amd64=1.12.0-1+deb9u1`

Licenses: (parsed from: `/usr/share/doc/libwayland-client0/copyright`, `/usr/share/doc/libwayland-cursor0/copyright`, `/usr/share/doc/libwayland-server0/copyright`)

- `X11`

Source:

```console
$ apt-get source -qq --print-uris wayland=1.12.0-1+deb9u1
'http://deb.debian.org/debian/pool/main/w/wayland/wayland_1.12.0-1+deb9u1.dsc' wayland_1.12.0-1+deb9u1.dsc 2423 SHA256:564e0dde0f58781a2745c3bc930fcae5edc487405271012363bc0ab9a9354831
'http://deb.debian.org/debian/pool/main/w/wayland/wayland_1.12.0.orig.tar.gz' wayland_1.12.0.orig.tar.gz 575381 SHA256:428537c2887b608cabde189a6450fcade8877e03b063a72c84431b5753a34aef
'http://deb.debian.org/debian/pool/main/w/wayland/wayland_1.12.0-1+deb9u1.diff.gz' wayland_1.12.0-1+deb9u1.diff.gz 11267 SHA256:263506a1fbb4a789ca87ee2c1bac81177c63f3b752010d8f7662e73e188f17e8
```

Other potentially useful URLs:

- https://sources.debian.net/src/wayland/1.12.0-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/wayland/1.12.0-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wayland/1.12.0-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.18-5+deb9u3`

Binary Packages:

- `wget=1.18-5+deb9u3`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.18-5+deb9u3
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.18-5+deb9u3.dsc' wget_1.18-5+deb9u3.dsc 2085 SHA256:0ffd4ef70f0e0c919fd60aa0135ca4b920ebaa9793935dd3a615103f7d209525
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.18.orig.tar.gz' wget_1.18.orig.tar.gz 3865525 SHA256:a00a65fab84cc46e24c53ce88c45604668a7a479276e037dc2f558e34717fb2d
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.18-5+deb9u3.debian.tar.xz' wget_1.18-5+deb9u3.debian.tar.xz 23672 SHA256:da643e00461f2a4451256ec2547a3c2d9d3c9819f3657e459d6cbdaa6c5390ad
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.18-5+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/wget/1.18-5+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.18-5+deb9u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x264=2:0.148.2748+git97eaef2-1`

Binary Packages:

- `libx264-148:amd64=2:0.148.2748+git97eaef2-1`
- `x264=2:0.148.2748+git97eaef2-1`

Licenses: (parsed from: `/usr/share/doc/libx264-148/copyright`, `/usr/share/doc/x264/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with other exception`
- `ISC`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris x264=2:0.148.2748+git97eaef2-1
'http://deb.debian.org/debian/pool/main/x/x264/x264_0.148.2748+git97eaef2-1.dsc' x264_0.148.2748+git97eaef2-1.dsc 2474 SHA256:c4139592e10fcc8796c910157e54b0276d59fd0489610b6a01fba29d542585e7
'http://deb.debian.org/debian/pool/main/x/x264/x264_0.148.2748+git97eaef2.orig.tar.gz' x264_0.148.2748+git97eaef2.orig.tar.gz 894829 SHA256:9121b8701d317f71bcea0ff021bd19e33337e78958c145f57f234d1b047106ee
'http://deb.debian.org/debian/pool/main/x/x264/x264_0.148.2748+git97eaef2-1.debian.tar.xz' x264_0.148.2748+git97eaef2-1.debian.tar.xz 23408 SHA256:24815462857b0426422106bec9af1d4d5e62e975f87e6d399c4f2897a64ea1ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/x264/2:0.148.2748+git97eaef2-1/ (for browsing the source)
- https://sources.debian.net/src/x264/2:0.148.2748+git97eaef2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x264/2:0.148.2748+git97eaef2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x265=2.1-2`

Binary Packages:

- `libx265-95:amd64=2.1-2+b2`

Licenses: (parsed from: `/usr/share/doc/libx265-95/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=2.1-2
'http://deb.debian.org/debian/pool/main/x/x265/x265_2.1-2.dsc' x265_2.1-2.dsc 2218 SHA256:8a9f5c1c3f1dae2a873c44114779b8c0cb8da11e2063b2ff4abf046acdd18842
'http://deb.debian.org/debian/pool/main/x/x265/x265_2.1.orig.tar.gz' x265_2.1.orig.tar.gz 1037400 SHA256:b3bc83754e91ed5655c8cba5a2ed48e6b9ab39699c9ed6554c670211d5870f9c
'http://deb.debian.org/debian/pool/main/x/x265/x265_2.1-2.debian.tar.xz' x265_2.1-2.debian.tar.xz 10664 SHA256:d2c44eacb09ae6fd4b2c11d5f7f07fb76f732454a9b550fc38543d9c812d6c9b
```

Other potentially useful URLs:

- https://sources.debian.net/src/x265/2.1-2/ (for browsing the source)
- https://sources.debian.net/src/x265/2.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x265/2.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xkeyboard-config=2.19-1+deb9u1`

Binary Packages:

- `xkb-data=2.19-1+deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xkeyboard-config=2.19-1+deb9u1
'http://deb.debian.org/debian/pool/main/x/xkeyboard-config/xkeyboard-config_2.19-1+deb9u1.dsc' xkeyboard-config_2.19-1+deb9u1.dsc 2137 SHA256:f093f0118c5c368b069fa64b1f0b0b86392311992c913dc70adf47ddd2e6813b
'http://deb.debian.org/debian/pool/main/x/xkeyboard-config/xkeyboard-config_2.19.orig.tar.gz' xkeyboard-config_2.19.orig.tar.gz 1524485 SHA256:f278c3ef6939122e727dab48e06f08916b09e5cfe1837fbfe6b0f69af96a8048
'http://deb.debian.org/debian/pool/main/x/xkeyboard-config/xkeyboard-config_2.19-1+deb9u1.diff.gz' xkeyboard-config_2.19-1+deb9u1.diff.gz 43605 SHA256:60945abb377bbe7e1b4c45a85325ddb6ae5ce25ede9dc7d0d02c961a4435c304
```

Other potentially useful URLs:

- https://sources.debian.net/src/xkeyboard-config/2.19-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/xkeyboard-config/2.19-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xkeyboard-config/2.19-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorg=1:7.7+19`

Binary Packages:

- `x11-common=1:7.7+19`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+19.dsc' xorg_7.7+19.dsc 2016 SHA256:fc4a577eee67f3604c56701e21b28dccd3858da0f110b708ca3359e2718e3d46
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+19.tar.gz' xorg_7.7+19.tar.gz 288723 SHA256:5de6df9e19009450b94f4f5307049bc2c7dc1114222f6f2f6fc60d737a33a537
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg/1:7.7+19/ (for browsing the source)
- https://sources.debian.net/src/xorg/1:7.7+19/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg/1:7.7+19/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xvidcore=2:1.3.4-1`

Binary Packages:

- `libxvidcore4:amd64=2:1.3.4-1+b2`

Licenses: (parsed from: `/usr/share/doc/libxvidcore4/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xvidcore=2:1.3.4-1
'http://deb.debian.org/debian/pool/main/x/xvidcore/xvidcore_1.3.4-1.dsc' xvidcore_1.3.4-1.dsc 2125 SHA256:8443f4a4c4b3608ea72e15e1c8613f62f83ea6d0b271483dec74f4cec06d0819
'http://deb.debian.org/debian/pool/main/x/xvidcore/xvidcore_1.3.4.orig.tar.gz' xvidcore_1.3.4.orig.tar.gz 818067 SHA256:4e9fd62728885855bc5007fe1be58df42e5e274497591fec37249e1052ae316f
'http://deb.debian.org/debian/pool/main/x/xvidcore/xvidcore_1.3.4-1.debian.tar.xz' xvidcore_1.3.4-1.debian.tar.xz 6056 SHA256:7371066d81e0819c586aeab2f1188c6e57da64dc70d9e582e885c5ccb8f7f5aa
```

Other potentially useful URLs:

- https://sources.debian.net/src/xvidcore/2:1.3.4-1/ (for browsing the source)
- https://sources.debian.net/src/xvidcore/2:1.3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xvidcore/2:1.3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.2-1.2`

Binary Packages:

- `liblzma5:amd64=5.2.2-1.2+b1`
- `xz-utils=5.2.2-1.2+b1`

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

### `dpkg` source package: `yajl=2.1.0-2`

Binary Packages:

- `libyajl2:amd64=2.1.0-2+b3`

Licenses: (parsed from: `/usr/share/doc/libyajl2/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris yajl=2.1.0-2
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0-2.dsc' yajl_2.1.0-2.dsc 1983 SHA256:bb0952d3d1c246cb6ffd920cd14c65e6d2e034c31dda792deca2d80b25841fd0
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0.orig.tar.gz' yajl_2.1.0.orig.tar.gz 83997 SHA256:3fb73364a5a30efe615046d07e6db9d09fd2b41c763c5f7d3bfb121cd5c5ac5a
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0-2.debian.tar.xz' yajl_2.1.0-2.debian.tar.xz 5480 SHA256:e68e0f76f7fc174a1eab3bc05e5549184669458dc78526a7b06aef2d9036a95f
```

Other potentially useful URLs:

- https://sources.debian.net/src/yajl/2.1.0-2/ (for browsing the source)
- https://sources.debian.net/src/yajl/2.1.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/yajl/2.1.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zeromq3=4.2.1-4+deb9u2`

Binary Packages:

- `libzmq5:amd64=4.2.1-4+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libzmq5/copyright`)

- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-3`
- `LGPL-3.0+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris zeromq3=4.2.1-4+deb9u2
'http://deb.debian.org/debian/pool/main/z/zeromq3/zeromq3_4.2.1-4+deb9u2.dsc' zeromq3_4.2.1-4+deb9u2.dsc 2054 SHA256:5df73f71fe112c6447ee9a26627a2bb94bdaac960c2dc0473141abb5d218b3a5
'http://deb.debian.org/debian/pool/main/z/zeromq3/zeromq3_4.2.1.orig.tar.gz' zeromq3_4.2.1.orig.tar.gz 586163 SHA256:f68bc45b51297577522aa83d8f05727dba54e567a177330c82918454b656f74f
'http://deb.debian.org/debian/pool/main/z/zeromq3/zeromq3_4.2.1-4+deb9u2.debian.tar.xz' zeromq3_4.2.1-4+deb9u2.debian.tar.xz 22836 SHA256:f62f53f804da3d88d6c2972782ed48764fbb1726305178b301f1a033364ad159
```

Other potentially useful URLs:

- https://sources.debian.net/src/zeromq3/4.2.1-4+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/zeromq3/4.2.1-4+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zeromq3/4.2.1-4+deb9u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.8.dfsg-5`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-5`

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

### `dpkg` source package: `zvbi=0.2.35-13`

Binary Packages:

- `libzvbi-common=0.2.35-13`
- `libzvbi0:amd64=0.2.35-13`

Licenses: (parsed from: `/usr/share/doc/libzvbi-common/copyright`, `/usr/share/doc/libzvbi0/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris zvbi=0.2.35-13
'http://deb.debian.org/debian/pool/main/z/zvbi/zvbi_0.2.35-13.dsc' zvbi_0.2.35-13.dsc 2109 SHA256:8ac47d2f6354995b0302f780ae4447388e1929d72d3bf9ab893a5e87deba4399
'http://deb.debian.org/debian/pool/main/z/zvbi/zvbi_0.2.35.orig.tar.bz2' zvbi_0.2.35.orig.tar.bz2 1047761 SHA256:fc883c34111a487c4a783f91b1b2bb5610d8d8e58dcba80c7ab31e67e4765318
'http://deb.debian.org/debian/pool/main/z/zvbi/zvbi_0.2.35-13.debian.tar.xz' zvbi_0.2.35-13.debian.tar.xz 15184 SHA256:9199d10d014a76498dc6ef08424b13863c689775e877e3d425d8437b85895886
```

Other potentially useful URLs:

- https://sources.debian.net/src/zvbi/0.2.35-13/ (for browsing the source)
- https://sources.debian.net/src/zvbi/0.2.35-13/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zvbi/0.2.35-13/ (for access to the source package after it no longer exists in the archive)
