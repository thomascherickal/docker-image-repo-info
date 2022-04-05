# `xwiki:13-postgres-tomcat`

## Docker Metadata

- Image ID: `sha256:0e28d76ed3681d5a083c870e9f143cf5ffb7149372c68cb6e23cc6a7fa5ed338`
- Created: `2022-04-01T21:34:50.23430721Z`
- Virtual Size: ~ 1.55 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["xwiki"]`
- Environment:
  - `PATH=/usr/local/tomcat/bin:/usr/local/openjdk-11/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `JAVA_HOME=/usr/local/openjdk-11`
  - `LANG=C.UTF-8`
  - `JAVA_VERSION=11.0.14.1`
  - `CATALINA_HOME=/usr/local/tomcat`
  - `TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib`
  - `LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib`
  - `GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243`
  - `TOMCAT_MAJOR=9`
  - `TOMCAT_VERSION=9.0.62`
  - `TOMCAT_SHA512=179af1d50a7d330d0842d3f1cae086bbc1b20e8f6752d66500663f3ac71d80f50113bbd29931e21c8e2eccd982f9f872e193364311316fdd67349130d440c83f`
  - `XWIKI_VERSION=13.10.4`
  - `XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.4`
  - `XWIKI_DOWNLOAD_SHA256=2bf3b7f92b97dfdaa695bd812efe77c0f70f1638667abf94f865c7050e486481`
- Labels:
  - `org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>`
  - `org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki`
  - `org.opencontainers.image.licenses=LGPL-2.1`
  - `org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git`
  - `org.opencontainers.image.url=https://hub.docker.com/_/xwiki`
  - `org.opencontainers.image.vendor=xwiki.org`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-10`

Binary Packages:

- `libacl1:amd64=2.2.53-10`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-10
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-10.dsc' acl_2.2.53-10.dsc 2468 SHA256:09204a89156b17a3603b2ce34b3c7b1a9fd7345086c787962188d95347918c59
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-10.debian.tar.xz' acl_2.2.53-10.debian.tar.xz 25536 SHA256:6b83a626aa383334b64666181642c7c13e44a6fe65486d0aaa34bd8de6d58b20
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.53-10/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.53-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.53-10/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `apr=1.7.0-6+deb11u1`

Binary Packages:

- `libapr1:amd64=1.7.0-6+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-6+deb11u1
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0-6%2bdeb11u1.dsc' apr_1.7.0-6+deb11u1.dsc 2282 SHA256:561d329f77659ea05d7303776b76922c4c13c5647b5f9205a3d6637976f345df
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA256:e2e148f0b2e99b8e5c6caa09f6d4fb4dd3e83f744aa72a952f94f5a14436f7ea
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA256:5a6c4e721ed82116d7877254ae11c076014040af2ff816ea15ec81e77a4a7d43
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0-6%2bdeb11u1.debian.tar.xz' apr_1.7.0-6+deb11u1.debian.tar.xz 214884 SHA256:7352919715fe985ccfee1953a85a051e16cd4af0c739c0f827e508a309ee5e06
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.7.0-6+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/apr/1.7.0-6+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.7.0-6+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=2.2.4`

Binary Packages:

- `apt=2.2.4`
- `libapt-pkg6.0:amd64=2.2.4`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.2.4
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.2.4.dsc' apt_2.2.4.dsc 2780 SHA256:750079533300bc3a4f3e10a9c8dbffaa0781b92e3616a12d7e18ab1378ca4466
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.2.4.tar.xz' apt_2.2.4.tar.xz 2197424 SHA256:6eecd04a4979bd2040b22a14571c15d342c4e1802b2023acb5aa19649b1f64ea
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/2.2.4/ (for browsing the source)
- https://sources.debian.net/src/apt/2.2.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/2.2.4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `attr=1:2.4.48-6`

Binary Packages:

- `libattr1:amd64=1:2.4.48-6`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.48-6
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-6.dsc' attr_2.4.48-6.dsc 2433 SHA256:d55d1ba40517146e9a43f9ed1c5dbd82cfe079cd1fdb852323717a953515cfa4
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-6.debian.tar.xz' attr_2.4.48-6.debian.tar.xz 27260 SHA256:77f7e03cc8dd039abc3e4a7353f816a3b07fbd0b22d7784f635c5edf7d20b6df
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.4.48-6/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.4.48-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.4.48-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:3.0-2`

Binary Packages:

- `libaudit-common=1:3.0-2`
- `libaudit1:amd64=1:3.0-2`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0-2
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0-2.dsc' audit_3.0-2.dsc 2397 SHA256:3cb83cc7649bb854c76f9cb6744b34091e667e433a91a57323938fdf3f353227
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.orig.tar.gz' audit_3.0.orig.tar.gz 1109442 SHA256:bd31826823b912b6fe271d2d979ed879e9fc393cab1e2f7c4e1af258231765b8
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0-2.debian.tar.xz' audit_3.0-2.debian.tar.xz 18640 SHA256:10193fa9823eb66dfb1220fb109b8b8e01f3f720c5a1630e9015d92aa7a8ce3a
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:3.0-2/ (for browsing the source)
- https://sources.debian.net/src/audit/1:3.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:3.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `avahi=0.8-5`

Binary Packages:

- `libavahi-client3:amd64=0.8-5`
- `libavahi-common-data:amd64=0.8-5`
- `libavahi-common3:amd64=0.8-5`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.8-5
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.8-5.dsc' avahi_0.8-5.dsc 3949 SHA256:362e84af42fc07a7f99278c354fffd4f6758c647399f4c3328eca7482eccb6d2
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.8.orig.tar.gz' avahi_0.8.orig.tar.gz 1591458 SHA256:060309d7a333d38d951bc27598c677af1796934dbd98e1024e7ad8de798fedda
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.8-5.debian.tar.xz' avahi_0.8-5.debian.tar.xz 34624 SHA256:5b68749ebd5551808b3bcd9a683026833b34dcea13e51d0e554b610517d0afc2
```

Other potentially useful URLs:

- https://sources.debian.net/src/avahi/0.8-5/ (for browsing the source)
- https://sources.debian.net/src/avahi/0.8-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/avahi/0.8-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=11.1+deb11u3`

Binary Packages:

- `base-files=11.1+deb11u3`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11.1+deb11u3
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_11.1%2bdeb11u3.dsc' base-files_11.1+deb11u3.dsc 1110 SHA256:5127052dfd37b7ecf5db01d5ef6e89b9df38e8589f601081308d5cc867fa529f
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_11.1%2bdeb11u3.tar.xz' base-files_11.1+deb11u3.tar.xz 65548 SHA256:f79b172739a45ee88e72f9832eab393f92968cd315db3c5b275cc070a2a7b8d3
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/11.1+deb11u3/ (for browsing the source)
- https://sources.debian.net/src/base-files/11.1+deb11u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/11.1+deb11u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.51`

Binary Packages:

- `base-passwd=3.5.51`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.51
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.51.dsc' base-passwd_3.5.51.dsc 1757 SHA256:5752e4c2e3b9b4d45502f6aa5ce8dfd0136ea60f1b4fbd4524385e4bbd6a1571
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.51.tar.xz' base-passwd_3.5.51.tar.xz 53980 SHA256:66c75ce1877759148dbdd2704b138c4a02adab89d7d7591b6ab184f8f614efba
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.51/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.51/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.51/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.1-2`

Binary Packages:

- `bash=5.1-2+b3`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-2
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-2.dsc' bash_5.1-2.dsc 2296 SHA256:1129f1397ec8e673bb8fc6acf53b371b9ed4132a7076e59bc0bf0f8e8d134e32
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA256:d5eeee4f953c09826409d572e2e8996a2140d67eb8f382ce1f3a9d23883ad696
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.1-2.debian.tar.xz' bash_5.1-2.debian.tar.xz 90660 SHA256:b41f4a62e613ccffbef6032eee4d671bf82cdb00472c452fcb0c510a1503710c
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/5.1-2/ (for browsing the source)
- https://sources.debian.net/src/bash/5.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/5.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `boost1.74=1.74.0-9`

Binary Packages:

- `libboost-filesystem1.74.0:amd64=1.74.0-9`
- `libboost-iostreams1.74.0:amd64=1.74.0-9`
- `libboost-locale1.74.0:amd64=1.74.0-9`
- `libboost-thread1.74.0:amd64=1.74.0-9`

Licenses: (parsed from: `/usr/share/doc/libboost-filesystem1.74.0/copyright`, `/usr/share/doc/libboost-iostreams1.74.0/copyright`, `/usr/share/doc/libboost-locale1.74.0/copyright`, `/usr/share/doc/libboost-thread1.74.0/copyright`)

- `Apache-2.0`
- `BSD2`
- `BSD3_DEShaw`
- `BSD3_Google`
- `BSL-1.0`
- `Caramel`
- `CrystalClear`
- `HP`
- `Jam`
- `Kempf`
- `MIT`
- `NIST`
- `OldBoost1`
- `OldBoost2`
- `OldBoost3`
- `Python`
- `SGI`
- `Spencer`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris boost1.74=1.74.0-9
'http://deb.debian.org/debian/pool/main/b/boost1.74/boost1.74_1.74.0-9.dsc' boost1.74_1.74.0-9.dsc 9222 SHA256:d3ee109fb93c3fd3eb761e1278a7fbf270c3c51564009728b7355af297fbcd50
'http://deb.debian.org/debian/pool/main/b/boost1.74/boost1.74_1.74.0.orig.tar.xz' boost1.74_1.74.0.orig.tar.xz 60536256 SHA256:2467be4af625b5ae4b3c93fc7af196a09eba39c11a7338cd9e8b356fa44d2f45
'http://deb.debian.org/debian/pool/main/b/boost1.74/boost1.74_1.74.0-9.debian.tar.xz' boost1.74_1.74.0-9.debian.tar.xz 367784 SHA256:10ff1892cd8194f38316a63c2236a44cb7681ba17301cbc0a2fa6f482335c1f9
```

Other potentially useful URLs:

- https://sources.debian.net/src/boost1.74/1.74.0-9/ (for browsing the source)
- https://sources.debian.net/src/boost1.74/1.74.0-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/boost1.74/1.74.0-9/ (for access to the source package after it no longer exists in the archive)

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

- `bzip2=1.0.8-4`
- `libbz2-1.0:amd64=1.0.8-4`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

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

### `dpkg` source package: `clp=1.17.5+repack1-1`

Binary Packages:

- `coinor-libclp1=1.17.5+repack1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libclp1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris clp=1.17.5+repack1-1
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.17.5%2brepack1-1.dsc' clp_1.17.5+repack1-1.dsc 2266 SHA256:9811c6c9fc2552c7216680357cfd123c025ff7b48fe8741a2273273f32c140f7
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.17.5%2brepack1.orig.tar.xz' clp_1.17.5+repack1.orig.tar.xz 1303732 SHA256:eba63e7b33b6a8777d0ad1dd53026f8f78a984731c408ccdcb22ca7a0f771f43
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.17.5%2brepack1-1.debian.tar.xz' clp_1.17.5+repack1-1.debian.tar.xz 10664 SHA256:5afd5b9fc616afda6ebbe86cc89f399707668eec3d7395fb4f6aa448943eddc2
```

Other potentially useful URLs:

- https://sources.debian.net/src/clp/1.17.5+repack1-1/ (for browsing the source)
- https://sources.debian.net/src/clp/1.17.5+repack1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/clp/1.17.5+repack1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `clucene-core=2.3.3.4+dfsg-1`

Binary Packages:

- `libclucene-contribs1v5:amd64=2.3.3.4+dfsg-1+b1`
- `libclucene-core1v5:amd64=2.3.3.4+dfsg-1+b1`

Licenses: (parsed from: `/usr/share/doc/libclucene-contribs1v5/copyright`, `/usr/share/doc/libclucene-core1v5/copyright`)

- `Apache-2.0`
- `LGPL-2.1`
- `Reuters-21578 - Distribution 1.0`

Source:

```console
$ apt-get source -qq --print-uris clucene-core=2.3.3.4+dfsg-1
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4%2bdfsg-1.dsc' clucene-core_2.3.3.4+dfsg-1.dsc 2019 SHA256:5158409a1b0c6913f82e5e0562ace6f3ff0cab197cf72b86e039b9fb9a73e1ed
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4%2bdfsg.orig.tar.xz' clucene-core_2.3.3.4+dfsg.orig.tar.xz 826688 SHA256:c70b8202c0afca27f9fa2f1a5d09a41bc4cc57a8f68c854379891ea2e24f1490
'http://deb.debian.org/debian/pool/main/c/clucene-core/clucene-core_2.3.3.4%2bdfsg-1.debian.tar.xz' clucene-core_2.3.3.4+dfsg-1.debian.tar.xz 8736 SHA256:a7d25d096e70105464a911e908fee7e5eb25adf3682ae75b1b514d6a5846b076
```

Other potentially useful URLs:

- https://sources.debian.net/src/clucene-core/2.3.3.4+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/clucene-core/2.3.3.4+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/clucene-core/2.3.3.4+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinmp=1.8.3-3`

Binary Packages:

- `coinor-libcoinmp1v5:amd64=1.8.3-3`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinmp1v5/copyright`)

- `CPL-1`
- `EPL-1`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris coinmp=1.8.3-3
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.8.3-3.dsc' coinmp_1.8.3-3.dsc 2036 SHA256:d661804e868a94e92c5204e77b2e6f33dc0522e7a103d295f3c77bdff9a81fd4
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.8.3.orig.tar.gz' coinmp_1.8.3.orig.tar.gz 7109200 SHA256:253ea6f55ba6cda18f35ccc8ebe6d6e2e9023df64d02f6536abc8b9ae4206681
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.8.3-3.debian.tar.xz' coinmp_1.8.3-3.debian.tar.xz 35428 SHA256:5fd877d245253d255f5399874f19669e6f536011c482eebadacbd89d2ee10e00
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinmp/1.8.3-3/ (for browsing the source)
- https://sources.debian.net/src/coinmp/1.8.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinmp/1.8.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-cbc=2.10.5+ds1-3`

Binary Packages:

- `coinor-libcbc3:amd64=2.10.5+ds1-3`

Licenses: (parsed from: `/usr/share/doc/coinor-libcbc3/copyright`)

- `EPL-1`
- `GPL-3`
- `LUCENT`

Source:

```console
$ apt-get source -qq --print-uris coinor-cbc=2.10.5+ds1-3
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.10.5%2bds1-3.dsc' coinor-cbc_2.10.5+ds1-3.dsc 2407 SHA256:e3807ab8424786e8934f321c13a103bbbcf69d205badcb42d077ca24ca3acc0a
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.10.5%2bds1.orig.tar.xz' coinor-cbc_2.10.5+ds1.orig.tar.xz 927396 SHA256:1792229ce9469169a6e8580a1446b8bcc960584be9eaaff0db5e024f9cff71e3
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.10.5%2bds1-3.debian.tar.xz' coinor-cbc_2.10.5+ds1-3.debian.tar.xz 12844 SHA256:b77dc38bb3e2f727c31dab7272132ee0d43ebfcaf4f9152820a68303f77db507
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-cbc/2.10.5+ds1-3/ (for browsing the source)
- https://sources.debian.net/src/coinor-cbc/2.10.5+ds1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-cbc/2.10.5+ds1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-cgl=0.60.3+repack1-2`

Binary Packages:

- `coinor-libcgl1=0.60.3+repack1-2`

Licenses: (parsed from: `/usr/share/doc/coinor-libcgl1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-cgl=0.60.3+repack1-2
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.60.3%2brepack1-2.dsc' coinor-cgl_0.60.3+repack1-2.dsc 2268 SHA256:1774b866d56d95a2345830c58aeb8678a27b77b14396754803eaf13fee1c002e
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.60.3%2brepack1.orig.tar.xz' coinor-cgl_0.60.3+repack1.orig.tar.xz 606960 SHA256:756f858691021c9982274ee3510b00b998a0e160f62a2a5813e1324b94418576
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.60.3%2brepack1-2.debian.tar.xz' coinor-cgl_0.60.3+repack1-2.debian.tar.xz 8816 SHA256:2c357372b1b53009b417b744b49a55abbf5c651a9237186273bc089330d2935e
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-cgl/0.60.3+repack1-2/ (for browsing the source)
- https://sources.debian.net/src/coinor-cgl/0.60.3+repack1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-cgl/0.60.3+repack1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-osi=0.108.6+repack1-2`

Binary Packages:

- `coinor-libosi1v5:amd64=0.108.6+repack1-2`

Licenses: (parsed from: `/usr/share/doc/coinor-libosi1v5/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-osi=0.108.6+repack1-2
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.108.6%2brepack1-2.dsc' coinor-osi_0.108.6+repack1-2.dsc 2174 SHA256:21bcc2358baeb202d4d9289e1a31ff50ad4e1447cd7b4b0562d8695458e94319
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.108.6%2brepack1.orig.tar.xz' coinor-osi_0.108.6+repack1.orig.tar.xz 500744 SHA256:5ca3b9e20ecc450dbc1c6b9a43be609f52fd6efee97d488a7136657577499980
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.108.6%2brepack1-2.debian.tar.xz' coinor-osi_0.108.6+repack1-2.debian.tar.xz 8608 SHA256:7f23746d853d87825212a97877687da3568ff50db9630a43cf61b8d846e073b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-osi/0.108.6+repack1-2/ (for browsing the source)
- https://sources.debian.net/src/coinor-osi/0.108.6+repack1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-osi/0.108.6+repack1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinutils=2.11.4+repack1-1`

Binary Packages:

- `coinor-libcoinutils3v5=2.11.4+repack1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinutils3v5/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinutils=2.11.4+repack1-1
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.11.4%2brepack1-1.dsc' coinutils_2.11.4+repack1-1.dsc 2176 SHA256:0883209f8f4871a2b63888b5e3e0d241d1f0052031d7ed4779d252c8c3ea8274
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.11.4%2brepack1.orig.tar.xz' coinutils_2.11.4+repack1.orig.tar.xz 841280 SHA256:a9d2bdcb22a00a571c397ce55c3107730729f7d07fb3e60f1058668c5884c074
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.11.4%2brepack1-1.debian.tar.xz' coinutils_2.11.4+repack1-1.debian.tar.xz 8996 SHA256:ee4fd30f435e7f570d24f0b364076102857e15de24aae7973c52cfbc755a9b35
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinutils/2.11.4+repack1-1/ (for browsing the source)
- https://sources.debian.net/src/coinutils/2.11.4+repack1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinutils/2.11.4+repack1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `cups=2.3.3op2-3+deb11u1`

Binary Packages:

- `libcups2:amd64=2.3.3op2-3+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`)

- `Apache-2.0`
- `Apache-2.0-with-GPL2-LGPL2-Exception`
- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `FSFUL`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.3.3op2-3+deb11u1
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.3.3op2-3%2bdeb11u1.dsc' cups_2.3.3op2-3+deb11u1.dsc 3373 SHA256:0366ca59ff6d2d3c33c861d886e1043527fe19a14e7ab66e292c777155401dba
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.3.3op2.orig.tar.gz' cups_2.3.3op2.orig.tar.gz 7993205 SHA256:deb3575bbe79c0ae963402787f265bfcf8d804a71fc2c94318a74efec86f96df
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.3.3op2.orig.tar.gz.asc' cups_2.3.3op2.orig.tar.gz.asc 833 SHA256:ac9e7e3415d727e9882cf0f65ee38459cbcd602cb49cf392e0a65a172fe3bdaf
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.3.3op2-3%2bdeb11u1.debian.tar.xz' cups_2.3.3op2-3+deb11u1.debian.tar.xz 346456 SHA256:3f1dab94f23a46fd566eafc2a9bdc5d2e8f5cbb49b6385b45d753209e8965e16
```

Other potentially useful URLs:

- https://sources.debian.net/src/cups/2.3.3op2-3+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/cups/2.3.3op2-3+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cups/2.3.3op2-3+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.74.0-1.3+deb11u1`

Binary Packages:

- `curl=7.74.0-1.3+deb11u1`
- `libcurl3-gnutls:amd64=7.74.0-1.3+deb11u1`
- `libcurl4:amd64=7.74.0-1.3+deb11u1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.74.0-1.3+deb11u1
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0-1.3%2bdeb11u1.dsc' curl_7.74.0-1.3+deb11u1.dsc 2699 SHA256:7983845054585d56348bc262cee1f4fff96866fe23ca864db3c9d43e829139fc
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0.orig.tar.gz' curl_7.74.0.orig.tar.gz 4043409 SHA256:e56b3921eeb7a2951959c02db0912b5fcd5fdba5aca071da819e1accf338bbd7
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0-1.3%2bdeb11u1.debian.tar.xz' curl_7.74.0-1.3+deb11u1.debian.tar.xz 37024 SHA256:eac5deff2b2511443ba4995daa8afe8985aaa5f62a24d672e9715fcabe0069b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.74.0-1.3+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/curl/7.74.0-1.3+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.74.0-1.3+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2.1+deb11u1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2.1+deb11u1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2.1+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2.1+deb11u1
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg-2.1%2bdeb11u1.dsc' cyrus-sasl2_2.1.27+dfsg-2.1+deb11u1.dsc 3591 SHA256:4dafa1a5c90f0b3d9d6e9d22e810492edd3b91b9f1d4d9666683d257528445d6
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg-2.1%2bdeb11u1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.1+deb11u1.debian.tar.xz 102488 SHA256:70b7a55776febf987363f5bb58322d6f03186215374a2eb0b6203980924f8680
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2.1+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2.1+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg-2.1+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.11+git20200708+dd9ef66-5`

Binary Packages:

- `dash=0.5.11+git20200708+dd9ef66-5`

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
$ apt-get source -qq --print-uris dash=0.5.11+git20200708+dd9ef66-5
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20200708%2bdd9ef66-5.dsc' dash_0.5.11+git20200708+dd9ef66-5.dsc 1906 SHA256:b0568c34647dc2aa0b8e2656c5e7449d9a1feb4b89d6857f507173b1f9a42ee7
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20200708%2bdd9ef66.orig.tar.gz' dash_0.5.11+git20200708+dd9ef66.orig.tar.gz 167776 SHA256:ab70b1f165bfedadd1282da546f1c917f1b7ccb2c5c2f898310a963e2ab5520c
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20200708%2bdd9ef66-5.debian.tar.xz' dash_0.5.11+git20200708+dd9ef66-5.debian.tar.xz 43120 SHA256:5da6039e043c953ff91a31c767ed703699870682ff356a1642f4798ce04a2926
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.11+git20200708+dd9ef66-5/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.11+git20200708+dd9ef66-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.11+git20200708+dd9ef66-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `dbus=1.12.20-2`

Binary Packages:

- `libdbus-1-3:amd64=1.12.20-2`

Licenses: (parsed from: `/usr/share/doc/libdbus-1-3/copyright`)

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
$ apt-get source -qq --print-uris dbus=1.12.20-2
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20-2.dsc' dbus_1.12.20-2.dsc 3638 SHA256:2131b177514f1a5a830d21d5f757ac5f69f30cea7ed1429e357f7bf5098de3c0
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20.orig.tar.gz' dbus_1.12.20.orig.tar.gz 2095511 SHA256:f77620140ecb4cdc67f37fb444f8a6bea70b5b6461f12f1cbe2cec60fa7de5fe
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20.orig.tar.gz.asc' dbus_1.12.20.orig.tar.gz.asc 833 SHA256:a5f4d51c9c95a6cf7270abb6548894d91d51eebc0e9f996d0951c8ee925894e7
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20-2.debian.tar.xz' dbus_1.12.20-2.debian.tar.xz 58076 SHA256:b421fd81e8b8d400846d1d9646d347c5211ac187fd9973e6254f84a717089dc6
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus/1.12.20-2/ (for browsing the source)
- https://sources.debian.net/src/dbus/1.12.20-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus/1.12.20-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dconf=0.38.0-2`

Binary Packages:

- `libdconf1:amd64=0.38.0-2`

Licenses: (parsed from: `/usr/share/doc/libdconf1/copyright`)

- `GPL-3`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dconf=0.38.0-2
'http://deb.debian.org/debian/pool/main/d/dconf/dconf_0.38.0-2.dsc' dconf_0.38.0-2.dsc 2740 SHA256:808e980567c6fa53920d89263b7496d7473d8d6a7a6346b2288abcabf897bbba
'http://deb.debian.org/debian/pool/main/d/dconf/dconf_0.38.0.orig.tar.xz' dconf_0.38.0.orig.tar.xz 115876 SHA256:45f60f41330d27715cce1315af123f94f1c2cdedb68b6bed3b309866eec44f58
'http://deb.debian.org/debian/pool/main/d/dconf/dconf_0.38.0-2.debian.tar.xz' dconf_0.38.0-2.debian.tar.xz 10584 SHA256:410e31fa71e5cd14289a5b6d72b5ac3a8ae365257c28fd8662b85601ecfe8819
```

Other potentially useful URLs:

- https://sources.debian.net/src/dconf/0.38.0-2/ (for browsing the source)
- https://sources.debian.net/src/dconf/0.38.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dconf/0.38.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `debianutils=4.11.2`

Binary Packages:

- `debianutils=4.11.2`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.11.2
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.11.2.dsc' debianutils_4.11.2.dsc 1644 SHA256:b11164a7aa3ca07ae1d758d15d707928defb64f2c35bf96f2e4fd983ee17b310
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.11.2.tar.xz' debianutils_4.11.2.tar.xz 158132 SHA256:3b680e81709b740387335fac8f8806d71611dcf60874e1a792e862e48a1650de
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.11.2/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.11.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.11.2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `e2fsprogs=1.46.2-2`

Binary Packages:

- `e2fsprogs=1.46.2-2`
- `libcom-err2:amd64=1.46.2-2`
- `libext2fs2:amd64=1.46.2-2`
- `libss2:amd64=1.46.2-2`
- `logsave=1.46.2-2`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.2-2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.2-2.dsc' e2fsprogs_1.46.2-2.dsc 2842 SHA256:5b25910da7b90e40881d2cf63ebb4ae49642a8730f6e2a9c953e365dddccb73c
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.2.orig.tar.gz' e2fsprogs_1.46.2.orig.tar.gz 9496954 SHA256:f79f26b4f65bdc059fca12e1ec6a3040c3ce1a503fb70eb915bee71903815cd5
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.2.orig.tar.gz.asc' e2fsprogs_1.46.2.orig.tar.gz.asc 488 SHA256:948552550f23a9e0223cecb51b5b85258c9d94895a20bce1180fce770628a55f
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.2-2.debian.tar.xz' e2fsprogs_1.46.2-2.debian.tar.xz 92624 SHA256:dc67d61815c524922e7461040d732bd245cf0196f7cc8a91ea7911a87b38f737
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.46.2-2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.46.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.46.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `elfutils=0.183-1`

Binary Packages:

- `libdw1:amd64=0.183-1`
- `libelf1:amd64=0.183-1`

Licenses: (parsed from: `/usr/share/doc/libdw1/copyright`, `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.183-1
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.183-1.dsc' elfutils_0.183-1.dsc 3036 SHA256:540e9b9c5d25d8567cb8e82444baef433fc4add627b4ce09185a9527a33113af
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.183.orig.tar.bz2' elfutils_0.183.orig.tar.bz2 9109254 SHA256:c3637c208d309d58714a51e61e63f1958808fead882e9b607506a29e5474f2c5
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.183-1.debian.tar.xz' elfutils_0.183-1.debian.tar.xz 33396 SHA256:e64d82677a9f12344210f2294f8738ce649fbac0ebec20f2354f39d8bd4698ce
```

Other potentially useful URLs:

- https://sources.debian.net/src/elfutils/0.183-1/ (for browsing the source)
- https://sources.debian.net/src/elfutils/0.183-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/elfutils/0.183-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.10-2+deb11u3`

Binary Packages:

- `libexpat1:amd64=2.2.10-2+deb11u3`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.10-2+deb11u3
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.10-2%2bdeb11u3.dsc' expat_2.2.10-2+deb11u3.dsc 2175 SHA256:bf66d8eca15055af1961c95703204fb71f48c0bfbb9db7b2a7eccce19e444555
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.10.orig.tar.gz' expat_2.2.10.orig.tar.gz 8276395 SHA256:62e280f5fd29a5b70973f623e20a7412c3e3912c2684cb0e462e2c881be129e1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.10-2%2bdeb11u3.debian.tar.xz' expat_2.2.10-2+deb11u3.debian.tar.xz 27188 SHA256:03a961cdbe42a5ebee68e072090821995730502cb3822fb59f0c642688fb9f51
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.10-2+deb11u3/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.10-2+deb11u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.10-2+deb11u3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `fonts-dejavu=2.37-2`

Binary Packages:

- `fonts-dejavu-core=2.37-2`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-2
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.dsc' fonts-dejavu_2.37-2.dsc 2387 SHA256:13948768dbf1a9aa3ae9fe592a4c6c904b1dd075acb689a49b85e0ae73b1756c
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://deb.debian.org/debian/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.debian.tar.xz' fonts-dejavu_2.37-2.debian.tar.xz 11408 SHA256:428cf37685df891574d2dcb32aa9366e4e95985fda7d87069903313bb03470ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/fonts-dejavu/2.37-2/ (for browsing the source)
- https://sources.debian.net/src/fonts-dejavu/2.37-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fonts-dejavu/2.37-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `freetype=2.10.4+dfsg-1`

Binary Packages:

- `libfreetype6:amd64=2.10.4+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `FSFAP`
- `FSFUL`
- `FSFULLR`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `OFL-1.1`
- `OpenGroup-BSD-like`
- `Permissive`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.10.4+dfsg-1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4%2bdfsg-1.dsc' freetype_2.10.4+dfsg-1.dsc 3693 SHA256:e49fd5a3be9816e2c9caf287e945a3257e60b809a50db83fcea2aa8e4ffa2438
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2demos.tar.xz' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz 236712 SHA256:3f873ebe4fb387da3859149459f9be95320ce1fd56b50f8fdb9d2a8492887083
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz.asc 195 SHA256:38d5b9a5aa11ecf8c6d4c983ef48b3ce2288fdf93d44719df2598b9d415c8061
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2docs.tar.xz' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz 2079084 SHA256:cca1c19d1efa911bb685d919b5b0fe1279b0699bf8eb6a3d3bf9f02784758212
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz.asc 195 SHA256:29fca9ff0e1cdc57ad5707b17f629eeaa216eb334f6082f1b05fb0fe35e14ff3
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig.tar.xz' freetype_2.10.4+dfsg.orig.tar.xz 2259340 SHA256:db0c0938b3b75cf314775baa75198098e41583b3aaa4804b454f183ce45120a9
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4%2bdfsg-1.debian.tar.xz' freetype_2.10.4+dfsg-1.debian.tar.xz 116636 SHA256:96276d66eb56247545cd9e60ffae0bd5b5aee0490e4e7171337a6666bc51b125
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.10.4+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.10.4+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.10.4+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-10=10.2.1-6`

Binary Packages:

- `gcc-10-base:amd64=10.2.1-6`
- `libgcc-s1:amd64=10.2.1-6`
- `libgfortran5:amd64=10.2.1-6`
- `libquadmath0:amd64=10.2.1-6`
- `libstdc++6:amd64=10.2.1-6`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.2.1-6
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.2.1-6.dsc' gcc-10_10.2.1-6.dsc 27632 SHA256:24024c1e225ca968f37ce39047ff5f1058219976db9e88a807173c2f07fa6029
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.2.1.orig.tar.xz' gcc-10_10.2.1.orig.tar.xz 84547844 SHA256:ea3c05faa381486e6b859c047dc14977418bf1ccda4567064e016493fd6fffec
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.2.1-6.debian.tar.xz' gcc-10_10.2.1-6.debian.tar.xz 2366560 SHA256:a95d6b9da2be83f9751850b002021281411ff1003d9feb77298b131da47820b3
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-10/10.2.1-6/ (for browsing the source)
- https://sources.debian.net/src/gcc-10/10.2.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-10/10.2.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-9=9.3.0-22`

Binary Packages:

- `gcc-9-base:amd64=9.3.0-22`

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
$ apt-get source -qq --print-uris gcc-9=9.3.0-22
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0-22.dsc' gcc-9_9.3.0-22.dsc 21926 SHA256:14a0ea03cee0eb5450cc630a3bdf47da157062b3e7622ac45f6ae14a321eae96
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0.orig.tar.gz' gcc-9_9.3.0.orig.tar.gz 88686943 SHA256:824044ffa96eb337bb1c1d4cf6a82691d0290d6f42e1d13362eea855458de060
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0-22.debian.tar.xz' gcc-9_9.3.0-22.debian.tar.xz 904252 SHA256:68d55260456847880c71831b69c19cb81e9d1abf09274ab77ab6c081e177d94d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-9/9.3.0-22/ (for browsing the source)
- https://sources.debian.net/src/gcc-9/9.3.0-22/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-9/9.3.0-22/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.19-2`

Binary Packages:

- `libgdbm-compat4:amd64=1.19-2`
- `libgdbm6:amd64=1.19-2`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.19-2
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.19-2.dsc' gdbm_1.19-2.dsc 2603 SHA256:1f05cd17a44cdf05eb97df79147a77a57fba3346b48f00909abe8ad963bf6220
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.19.orig.tar.gz' gdbm_1.19.orig.tar.gz 967861 SHA256:37ed12214122b972e18a0d94995039e57748191939ef74115b1d41d8811364bc
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.19.orig.tar.gz.asc' gdbm_1.19.orig.tar.gz.asc 181 SHA256:8f4e0502073a7a22972f1edc84c70151033257d879402ac85176d3ebc984b2b8
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.19-2.debian.tar.xz' gdbm_1.19-2.debian.tar.xz 16228 SHA256:c49d2faaa340acc8e94277dab0e0bf4ac10d49d9c374d6841883ac868edb5014
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.19-2/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.19-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.19-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.30.2-1`

Binary Packages:

- `git=1:2.30.2-1`
- `git-man=1:2.30.2-1`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
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
$ apt-get source -qq --print-uris git=1:2.30.2-1
'http://deb.debian.org/debian/pool/main/g/git/git_2.30.2-1.dsc' git_2.30.2-1.dsc 2867 SHA256:3afa12a5b18f1bc35c24bc1aef1a6c71327069d9c0e8e8aae4f098f2ff308c3d
'http://deb.debian.org/debian/pool/main/g/git/git_2.30.2.orig.tar.xz' git_2.30.2.orig.tar.xz 6329820 SHA256:41f7d90c71f9476cd387673fcb10ce09ccbed67332436a4cc58d7af32c355faa
'http://deb.debian.org/debian/pool/main/g/git/git_2.30.2-1.debian.tar.xz' git_2.30.2-1.debian.tar.xz 670844 SHA256:53233ac9049ebe0bf406e780afebbff3d1845f4001083657c649b30d6c526093
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.30.2-1/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.30.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.30.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.66.8-1`

Binary Packages:

- `libglib2.0-0:amd64=2.66.8-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.66.8-1
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.66.8-1.dsc' glib2.0_2.66.8-1.dsc 3383 SHA256:2f4335085e6d94e4c3fd6441195014b2eed516fc99b649ea75fe66c38bc5edba
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.66.8.orig.tar.xz' glib2.0_2.66.8.orig.tar.xz 4845548 SHA256:97bc87dd91365589af5cbbfea2574833aea7a1b71840fd365ecd2852c76b9c8b
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.66.8-1.debian.tar.xz' glib2.0_2.66.8-1.debian.tar.xz 99420 SHA256:a1d3c2725a1a680cf4e1ab021d66bbb7f223a6faee315e7f35bee0eb38ae712e
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.66.8-1/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.66.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.66.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.31-13+deb11u3`

Binary Packages:

- `libc-bin=2.31-13+deb11u3`
- `libc6:amd64=2.31-13+deb11u3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.31-13+deb11u3
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31-13%2bdeb11u3.dsc' glibc_2.31-13+deb11u3.dsc 8347 SHA256:1a8c389b5664962dda78e289d6938a2276b8b450d41e3081e7bf82db2fe1e409
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31.orig.tar.xz' glibc_2.31.orig.tar.xz 17254692 SHA256:3dc7704b6166839c37d7047626fd199f3d4c09aca0d90e48c51c31c967dce34e
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31-13%2bdeb11u3.debian.tar.xz' glibc_2.31-13+deb11u3.debian.tar.xz 916044 SHA256:1accd7015160a589e8ad1111011fa9c911a572e673aa5689b99f64ce6740226c
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.31-13+deb11u3/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.31-13+deb11u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.31-13+deb11u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.1+dfsg-1+deb11u1`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg-1+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg-1+deb11u1
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg-1%2bdeb11u1.dsc' gmp_6.2.1+dfsg-1+deb11u1.dsc 2181 SHA256:4c09eb0a1c333fc5e67184a18f050af0f46f7f0fdeb533557bebd89df07c137b
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA256:c6ba08e3f079260ab90ff44ab8801eae134cd62cd78f4aa56317c0e70daa40cb
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg-1%2bdeb11u1.debian.tar.xz' gmp_6.2.1+dfsg-1+deb11u1.debian.tar.xz 21920 SHA256:3cde187d542f5c095c6db8b76ec5252353e0413b492c57eb2e67ed3c43f40172
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-1+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-1+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg-1+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.27-2+deb11u1`

Binary Packages:

- `dirmngr=2.2.27-2+deb11u1`
- `gnupg=2.2.27-2+deb11u1`
- `gnupg-l10n=2.2.27-2+deb11u1`
- `gnupg-utils=2.2.27-2+deb11u1`
- `gpg=2.2.27-2+deb11u1`
- `gpg-agent=2.2.27-2+deb11u1`
- `gpg-wks-client=2.2.27-2+deb11u1`
- `gpg-wks-server=2.2.27-2+deb11u1`
- `gpgconf=2.2.27-2+deb11u1`
- `gpgsm=2.2.27-2+deb11u1`
- `gpgv=2.2.27-2+deb11u1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.27-2+deb11u1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-2%2bdeb11u1.dsc' gnupg2_2.2.27-2+deb11u1.dsc 3322 SHA256:851827956ba7268a14f2043c5af8f00d833f77f238fa4f02410215d36aa6327b
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2' gnupg2_2.2.27.orig.tar.bz2 7191555 SHA256:34e60009014ea16402069136e0a5f63d9b65f90096244975db5cea74b3d02399
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2.asc' gnupg2_2.2.27.orig.tar.bz2.asc 119 SHA256:2b44fd82da223cb629062b9c8840d92698c003be8531fc393c38f97b28cae2a4
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-2%2bdeb11u1.debian.tar.xz' gnupg2_2.2.27-2+deb11u1.debian.tar.xz 63404 SHA256:8b7117b6ea0efebd36e96b9501e03715d0954032234378c4051dfd99ca86e69d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.27-2+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.27-2+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.27-2+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.1-5`

Binary Packages:

- `libgnutls30:amd64=3.7.1-5`

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
$ apt-get source -qq --print-uris gnutls28=3.7.1-5
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.1-5.dsc' gnutls28_3.7.1-5.dsc 3487 SHA256:1cdc0abae8cc1b4a86ff4be7e549a5b6e82297645e7f61962e03294987e2ab9f
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.1.orig.tar.xz' gnutls28_3.7.1.orig.tar.xz 6038388 SHA256:3777d7963eca5e06eb315686163b7b3f5045e2baac5e54e038ace9835e5cac6f
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.1.orig.tar.xz.asc' gnutls28_3.7.1.orig.tar.xz.asc 854 SHA256:13a683b12602c169a7ad7827ab0e3f35c8fa1f98675d0073cf7d54a8cd635582
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.1-5.debian.tar.xz' gnutls28_3.7.1-5.debian.tar.xz 88576 SHA256:ec60906fcf50fb01654cf76557cc3810bfa88b0d0492e4d865097b97dd00558d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.1-5/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gpgme1.0=1.14.0-1`

Binary Packages:

- `libgpgme11:amd64=1.14.0-1+b2`
- `libgpgmepp6:amd64=1.14.0-1+b2`

Licenses: (parsed from: `/usr/share/doc/libgpgme11/copyright`, `/usr/share/doc/libgpgmepp6/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gpgme1.0=1.14.0-1
'http://deb.debian.org/debian/pool/main/g/gpgme1.0/gpgme1.0_1.14.0-1.dsc' gpgme1.0_1.14.0-1.dsc 2282 SHA256:df07545cfe20431f9b89d91703aafca4fd977866b0af3dc35a54b9c85db04f91
'http://deb.debian.org/debian/pool/main/g/gpgme1.0/gpgme1.0_1.14.0.orig.tar.bz2' gpgme1.0_1.14.0.orig.tar.bz2 1678910 SHA256:cef1f710a6b0d28f5b44242713ad373702d1466dcbe512eb4e754d7f35cd4307
'http://deb.debian.org/debian/pool/main/g/gpgme1.0/gpgme1.0_1.14.0.orig.tar.bz2.asc' gpgme1.0_1.14.0.orig.tar.bz2.asc 488 SHA256:296bf9648e5c5040438584f3a667f136acfdd571ec68cc6824e0ff786f2ef270
'http://deb.debian.org/debian/pool/main/g/gpgme1.0/gpgme1.0_1.14.0-1.debian.tar.xz' gpgme1.0_1.14.0-1.debian.tar.xz 19560 SHA256:87c9ed6a1390dbbf38708e79d701d260ba00a73eff3c925a12b98878d844bf4e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gpgme1.0/1.14.0-1/ (for browsing the source)
- https://sources.debian.net/src/gpgme1.0/1.14.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gpgme1.0/1.14.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `grep=3.6-1`

Binary Packages:

- `grep=3.6-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.6-1
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.6-1.dsc' grep_3.6-1.dsc 1644 SHA256:ccf6849a07a2c1fb77d2534a414f402af8cadeeac66a41deda04f3e835b09d3d
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.6.orig.tar.xz' grep_3.6.orig.tar.xz 1589412 SHA256:667e15e8afe189e93f9f21a7cd3a7b3f776202f417330b248c2ad4f997d9373e
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.6.orig.tar.xz.asc' grep_3.6.orig.tar.xz.asc 833 SHA256:02b52c0676e0e97762cee638125a345a5300fdcba691c1a5b0725ee6bd28d4a8
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.6-1.debian.tar.xz' grep_3.6-1.debian.tar.xz 17748 SHA256:67b481210e2db6bb9c45d90f39445a90c83e6d32fc6c8e5b9e89bb40488767c4
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.6-1/ (for browsing the source)
- https://sources.debian.net/src/grep/3.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gst-plugins-base1.0=1.18.4-2`

Binary Packages:

- `libgstreamer-plugins-base1.0-0:amd64=1.18.4-2`

Licenses: (parsed from: `/usr/share/doc/libgstreamer-plugins-base1.0-0/copyright`)

- `BSD (2 clause)`
- `BSD (3 clause)`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`
- `MIT/X11 (BSD like) LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gst-plugins-base1.0=1.18.4-2
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.18.4-2.dsc' gst-plugins-base1.0_1.18.4-2.dsc 3836 SHA256:1ab2568ee25f56ef62cadbe4ef8bcdfbb359103903adff0be3fc1c55f9512e65
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.18.4.orig.tar.xz' gst-plugins-base1.0_1.18.4.orig.tar.xz 3169512 SHA256:29e53229a84d01d722f6f6db13087231cdf6113dd85c25746b9b58c3d68e8323
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.18.4-2.debian.tar.xz' gst-plugins-base1.0_1.18.4-2.debian.tar.xz 42760 SHA256:1b423dfcdf78730bbd7e5a80a0b91701273545c05939b075ea223778b6aab441
```

Other potentially useful URLs:

- https://sources.debian.net/src/gst-plugins-base1.0/1.18.4-2/ (for browsing the source)
- https://sources.debian.net/src/gst-plugins-base1.0/1.18.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gst-plugins-base1.0/1.18.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gstreamer1.0=1.18.4-2.1`

Binary Packages:

- `libgstreamer1.0-0:amd64=1.18.4-2.1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer1.0-0/copyright`)

- `GPL-2+`
- `GPL-3+`
- `LGPL`
- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gstreamer1.0=1.18.4-2.1
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.18.4-2.1.dsc' gstreamer1.0_1.18.4-2.1.dsc 2886 SHA256:a2c3c641e3ce0398321c424f4b8663ce0759963f0c01da1ac9f83a1d2dd1911a
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.18.4.orig.tar.xz' gstreamer1.0_1.18.4.orig.tar.xz 2703948 SHA256:9aeec99b38e310817012aa2d1d76573b787af47f8a725a65b833880a094dfbc5
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.18.4-2.1.debian.tar.xz' gstreamer1.0_1.18.4-2.1.debian.tar.xz 44160 SHA256:823a003e524e9951d9ed9f0ae6f70b2661f9e5e3fd067902d8d4b40ba41e1176
```

Other potentially useful URLs:

- https://sources.debian.net/src/gstreamer1.0/1.18.4-2.1/ (for browsing the source)
- https://sources.debian.net/src/gstreamer1.0/1.18.4-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gstreamer1.0/1.18.4-2.1/ (for access to the source package after it no longer exists in the archive)

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

- `libharfbuzz-icu0:amd64=2.7.4-1`
- `libharfbuzz0b:amd64=2.7.4-1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz-icu0/copyright`, `/usr/share/doc/libharfbuzz0b/copyright`)

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

### `dpkg` source package: `hunspell=1.7.0-3`

Binary Packages:

- `libhunspell-1.7-0:amd64=1.7.0-3`

Licenses: (parsed from: `/usr/share/doc/libhunspell-1.7-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris hunspell=1.7.0-3
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.7.0-3.dsc' hunspell_1.7.0-3.dsc 2232 SHA256:f917955044d866233e0bfa0e01fbff6d605ccb6393c415e818604ba88b88e3df
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.7.0.orig.tar.gz' hunspell_1.7.0.orig.tar.gz 482156 SHA256:bb27b86eb910a8285407cf3ca33b62643a02798cf2eef468c0a74f6c3ee6bc8a
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.7.0-3.debian.tar.xz' hunspell_1.7.0-3.debian.tar.xz 21576 SHA256:1bbcadc4880b8af6543b37f42d05d92be1aa8725935974676d3c3af37b21d762
```

Other potentially useful URLs:

- https://sources.debian.net/src/hunspell/1.7.0-3/ (for browsing the source)
- https://sources.debian.net/src/hunspell/1.7.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hunspell/1.7.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hyphen=2.8.8-7`

Binary Packages:

- `libhyphen0:amd64=2.8.8-7`

Licenses: (parsed from: `/usr/share/doc/libhyphen0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.1+`

Source:

```console
$ apt-get source -qq --print-uris hyphen=2.8.8-7
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8-7.dsc' hyphen_2.8.8-7.dsc 2086 SHA256:f77f10861124cb0a9ac701cac314d037244d1bc362bac113efdf643573120ffe
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8.orig.tar.gz' hyphen_2.8.8.orig.tar.gz 638369 SHA256:304636d4eccd81a14b6914d07b84c79ebb815288c76fe027b9ebff6ff24d5705
'http://deb.debian.org/debian/pool/main/h/hyphen/hyphen_2.8.8-7.debian.tar.xz' hyphen_2.8.8-7.debian.tar.xz 12540 SHA256:085a0168906304c9033154923e269ae70b64881dcbe6e52854afd4bd2be60aec
```

Other potentially useful URLs:

- https://sources.debian.net/src/hyphen/2.8.8-7/ (for browsing the source)
- https://sources.debian.net/src/hyphen/2.8.8-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hyphen/2.8.8-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `icu=67.1-7`

Binary Packages:

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

### `dpkg` source package: `iso-codes=4.6.0-1`

Binary Packages:

- `iso-codes=4.6.0-1`

Licenses: (parsed from: `/usr/share/doc/iso-codes/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris iso-codes=4.6.0-1
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_4.6.0-1.dsc' iso-codes_4.6.0-1.dsc 1950 SHA256:fda03e45a8c1449533d3e4d8eeeec6d3b8364f390bdc81f3ed87997dc014601f
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_4.6.0.orig.tar.xz' iso-codes_4.6.0.orig.tar.xz 3669536 SHA256:41c672c18554e979e6191f950f454cdf1bfb67a6369fffe2997ff68e34845409
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_4.6.0-1.debian.tar.xz' iso-codes_4.6.0-1.debian.tar.xz 24008 SHA256:6ada248d2ab8e1474bf1185a84f671b8189e417412838fb16a1691536ca43c71
```

Other potentially useful URLs:

- https://sources.debian.net/src/iso-codes/4.6.0-1/ (for browsing the source)
- https://sources.debian.net/src/iso-codes/4.6.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iso-codes/4.6.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `krb5=1.18.3-6+deb11u1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.18.3-6+deb11u1`
- `libk5crypto3:amd64=1.18.3-6+deb11u1`
- `libkrb5-3:amd64=1.18.3-6+deb11u1`
- `libkrb5support0:amd64=1.18.3-6+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.18.3-6+deb11u1
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3-6%2bdeb11u1.dsc' krb5_1.18.3-6+deb11u1.dsc 2971 SHA256:db16b93a4beae887fe38dfbb19d1c220501c185bb4416924c4ff531312dba91e
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz' krb5_1.18.3.orig.tar.gz 8715312 SHA256:e61783c292b5efd9afb45c555a80dd267ac67eebabca42185362bee6c4fbd719
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3-6%2bdeb11u1.debian.tar.xz' krb5_1.18.3-6+deb11u1.debian.tar.xz 106192 SHA256:c68ecf8e8f4238f8950a7c409392c9a0661a6ad0d5efd88b6f8b0a39f7e8af21
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.18.3-6+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.18.3-6+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.18.3-6+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lapack=3.9.0-3`

Binary Packages:

- `libblas3:amd64=3.9.0-3`
- `liblapack3:amd64=3.9.0-3`

Licenses: (parsed from: `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.9.0-3
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.9.0-3.dsc' lapack_3.9.0-3.dsc 3407 SHA256:80d01af9003e43f6d6d886361b9d279b57b994139b6f12d01d6b00a40cb063a4
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.9.0.orig.tar.gz' lapack_3.9.0.orig.tar.gz 7534567 SHA256:106087f1bb5f46afdfba7f569d0cbe23dacb9a07cd24733765a0e89dbe1ad573
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.9.0-3.debian.tar.xz' lapack_3.9.0-3.debian.tar.xz 27804 SHA256:386d619026331dbf862b46a012f838bdf4298e88d587b5c4068f0188d5305407
```

Other potentially useful URLs:

- https://sources.debian.net/src/lapack/3.9.0-3/ (for browsing the source)
- https://sources.debian.net/src/lapack/3.9.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lapack/3.9.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.12~rc1-2`

Binary Packages:

- `liblcms2-2:amd64=2.12~rc1-2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3 (GPL-3 for the fast_float plugin only)`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.12~rc1-2
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.12%7erc1-2.dsc' lcms2_2.12~rc1-2.dsc 1988 SHA256:57b0b3cde709d8b7c43b195ba7f628d2d79323ee0db883050f253ee9f9acd48a
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.12%7erc1.orig.tar.gz' lcms2_2.12~rc1.orig.tar.gz 7417767 SHA256:3300ddd8c51d60ebcc206d20d185b1b19939c4cec1576d1f5b95297b0fbdfe19
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.12%7erc1-2.debian.tar.xz' lcms2_2.12~rc1-2.debian.tar.xz 10420 SHA256:dddb5b18a42fc7308e732f00643b29ac9f2638cf246569683cb50f13520c2cca
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.12~rc1-2/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.12~rc1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.12~rc1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libabw=0.1.3-1`

Binary Packages:

- `libabw-0.1-1:amd64=0.1.3-1`

Licenses: (parsed from: `/usr/share/doc/libabw-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3 | LGPL-3`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libabw=0.1.3-1
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.3-1.dsc' libabw_0.1.3-1.dsc 1988 SHA256:2460eeb1ba1d5b1ed07c732a33ea2e3b38b062f56b5bc49ee3eebda2fbf7cf30
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.3.orig.tar.xz' libabw_0.1.3.orig.tar.xz 318808 SHA256:e763a9dc21c3d2667402d66e202e3f8ef4db51b34b79ef41f56cacb86dcd6eed
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.3-1.debian.tar.xz' libabw_0.1.3-1.debian.tar.xz 13004 SHA256:72a6c0fe0b74680a58b9282a0ae6b187e83aaaffa45fe2be1785bb690ded6854
```

Other potentially useful URLs:

- https://sources.debian.net/src/libabw/0.1.3-1/ (for browsing the source)
- https://sources.debian.net/src/libabw/0.1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libabw/0.1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.5.3-7.1`

Binary Packages:

- `libassuan0:amd64=2.5.3-7.1`

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
$ apt-get source -qq --print-uris libassuan=2.5.3-7.1
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3-7.1.dsc' libassuan_2.5.3-7.1.dsc 2627 SHA256:9e4cfaef54fee1b6c1fd32fdfe6fc90b2dde78755517ee0ff56859e69251fb07
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA256:91bcb0403866b4e7c4bc1cc52ed4c364a9b5414b3994f718c70303f7f765e702
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA256:53b16a6619a2690b4f22da645a1d0c14b5664825c87b165ca5bd0de32607888a
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.3-7.1.debian.tar.xz' libassuan_2.5.3-7.1.debian.tar.xz 13952 SHA256:c6783e12dc1fb65681c083274f52cb3286da18dcf8a5b38a6de10143003e0681
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.3-7.1/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.3-7.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.3-7.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.11.3-1`

Binary Packages:

- `libbsd0:amd64=0.11.3-1`

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
$ apt-get source -qq --print-uris libbsd=0.11.3-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3-1.dsc' libbsd_0.11.3-1.dsc 2292 SHA256:714c9cee71ddcea7a91593c56ca9ab297856e4f597743a32cda909544fe04ccb
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3.orig.tar.xz' libbsd_0.11.3.orig.tar.xz 399712 SHA256:ff95cf8184151dacae4247832f8d4ea8800fa127dbd15033ecfe839f285b42a1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3.orig.tar.xz.asc' libbsd_0.11.3.orig.tar.xz.asc 833 SHA256:213f30c9537e2a180ebdad6445402ea879f83c3a85907f7509ae7f7304f7ce1b
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.3-1.debian.tar.xz' libbsd_0.11.3-1.debian.tar.xz 17504 SHA256:b414f384d71ebd8ed67b759526df4c83529946414c71cc3c5e5b98bc9323ad3b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.11.3-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.11.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.11.3-1/ (for access to the source package after it no longer exists in the archive)

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
- `libcap2-bin=1:2.44-1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

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

### `dpkg` source package: `libcbor=0.5.0+dfsg-2`

Binary Packages:

- `libcbor0:amd64=0.5.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libcbor0/copyright`)

- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.5.0+dfsg-2
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.5.0%2bdfsg-2.dsc' libcbor_0.5.0+dfsg-2.dsc 2057 SHA256:c1ad2786b340b65d55761ecc3d090a9d997b3a0e5218ff1d39f5cd19df900d73
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.5.0%2bdfsg.orig.tar.gz' libcbor_0.5.0+dfsg.orig.tar.gz 261201 SHA256:2bd1fb795d121a72fc127ccd0e6ce5f5742d5970d0913759bcdc729c700804fb
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.5.0%2bdfsg-2.debian.tar.xz' libcbor_0.5.0+dfsg-2.debian.tar.xz 3944 SHA256:c06d0890b369183142d09fc6a460d68fdaf32bb22f9885ee1cc203d00adc543d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcbor/0.5.0+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/libcbor/0.5.0+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcbor/0.5.0+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcdr=0.1.6-2`

Binary Packages:

- `libcdr-0.1-1:amd64=0.1.6-2`

Licenses: (parsed from: `/usr/share/doc/libcdr-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libcdr=0.1.6-2
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.6-2.dsc' libcdr_0.1.6-2.dsc 2143 SHA256:cbe7d8b05888dc26f46afce5c281b72c6fca30de6f9f40d8552f37952b2a2df2
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.6.orig.tar.xz' libcdr_0.1.6.orig.tar.xz 612068 SHA256:01cd00b04a030977e544433c2d127c997205332cd9b8e35ec0ee17110da7f861
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.6-2.debian.tar.xz' libcdr_0.1.6-2.debian.tar.xz 8332 SHA256:42bda009a55a652c6f807369cff86711f69dc464bebf0311519ac76dac8c0ce5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcdr/0.1.6-2/ (for browsing the source)
- https://sources.debian.net/src/libcdr/0.1.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcdr/0.1.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcmis=0.5.2-3`

Binary Packages:

- `libcmis-0.5-5v5=0.5.2-3`

Licenses: (parsed from: `/usr/share/doc/libcmis-0.5-5v5/copyright`)

- `GPL`
- `LGPL`
- `MPL | GPL2+ | LGPL2+`

Source:

```console
$ apt-get source -qq --print-uris libcmis=0.5.2-3
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.2-3.dsc' libcmis_0.5.2-3.dsc 2157 SHA256:09c68a765b20dc30308dd20c1a4e317b1d6d01bb6c963fb701bd5daf636c0546
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.2.orig.tar.gz' libcmis_0.5.2.orig.tar.gz 808619 SHA256:ed6f681a48abbf3c2324564b17a180d21fa9503230e8708825e1ad80daee4f81
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.2-3.debian.tar.xz' libcmis_0.5.2-3.debian.tar.xz 4692 SHA256:fa651f06436117c0ac3334a2f9dd72149786707ad9f3bee8e17b0f6a80d68687
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcmis/0.5.2-3/ (for browsing the source)
- https://sources.debian.net/src/libcmis/0.5.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcmis/0.5.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdeflate=1.7-1`

Binary Packages:

- `libdeflate0:amd64=1.7-1`

Licenses: (parsed from: `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.7-1
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.7-1.dsc' libdeflate_1.7-1.dsc 2163 SHA256:9f81571abf95f084dd6ce5c5f2b78ce66e5b1c7e2ec0f86e539f9df572061cd6
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.7.orig.tar.gz' libdeflate_1.7.orig.tar.gz 144143 SHA256:a5e6a0a9ab69f40f0f59332106532ca76918977a974e7004977a9498e3f11350
'http://deb.debian.org/debian/pool/main/libd/libdeflate/libdeflate_1.7-1.debian.tar.xz' libdeflate_1.7-1.debian.tar.xz 4392 SHA256:42a4f9b2307b0349fb2cd51a9585564284f480b03fa06c3f03ca02987ca66fb2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdeflate/1.7-1/ (for browsing the source)
- https://sources.debian.net/src/libdeflate/1.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdeflate/1.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libe-book=0.1.3-2`

Binary Packages:

- `libe-book-0.1-1:amd64=0.1.3-2`

Licenses: (parsed from: `/usr/share/doc/libe-book-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libe-book=0.1.3-2
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.3-2.dsc' libe-book_0.1.3-2.dsc 2076 SHA256:9bfd77a45818bd1db3c3c55b94d794916eedd125a7af9994f1042f276ee08c8f
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.3.orig.tar.xz' libe-book_0.1.3.orig.tar.xz 416268 SHA256:7e8d8ff34f27831aca3bc6f9cc532c2f90d2057c778963b884ff3d1e34dfe1f9
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.3-2.debian.tar.xz' libe-book_0.1.3-2.debian.tar.xz 7552 SHA256:fc6ed56015fec65a29f38291c267ff7fcded6327b69aa4f3b7b24bd7230fc389
```

Other potentially useful URLs:

- https://sources.debian.net/src/libe-book/0.1.3-2/ (for browsing the source)
- https://sources.debian.net/src/libe-book/0.1.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libe-book/0.1.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20191231-2`

Binary Packages:

- `libedit2:amd64=3.1-20191231-2+b1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-2
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20191231-2.dsc' libedit_3.1-20191231-2.dsc 2208 SHA256:422c4cab3b047b62142eef4f77995fd1cd0f424c52ffeae953935e241d3aaa81
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA256:dbb82cb7e116a5f8025d35ef5b4f7d4a3cdd0a3909a146a39112095a2d229071
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20191231-2.debian.tar.xz' libedit_3.1-20191231-2.debian.tar.xz 14576 SHA256:afb4656959bfa61817d0bc1982f2628373e84b251a148edb7da3e3c10645366c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20191231-2/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20191231-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20191231-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libeot=0.01-5`

Binary Packages:

- `libeot0:amd64=0.01-5+b1`

Licenses: (parsed from: `/usr/share/doc/libeot0/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libeot=0.01-5
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01-5.dsc' libeot_0.01-5.dsc 1949 SHA256:71933404d061aeffe2c0e5da353ef7c5146fd061131b0a8c31257b16b080cab6
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01.orig.tar.bz2' libeot_0.01.orig.tar.bz2 260288 SHA256:cf5091fa8e7dcdbe667335eb90a2cfdd0a3fe8f8c7c8d1ece44d9d055736a06a
'http://deb.debian.org/debian/pool/main/libe/libeot/libeot_0.01-5.debian.tar.xz' libeot_0.01-5.debian.tar.xz 7492 SHA256:e6f5685fee36d82d31e1d2b2334314098b8bac7b87de59ee89809795f85b87c5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libeot/0.01-5/ (for browsing the source)
- https://sources.debian.net/src/libeot/0.01-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libeot/0.01-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libepoxy=1.5.5-1`

Binary Packages:

- `libepoxy0:amd64=1.5.5-1`

Licenses: (parsed from: `/usr/share/doc/libepoxy0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libepoxy=1.5.5-1
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.5.5-1.dsc' libepoxy_1.5.5-1.dsc 2100 SHA256:2c8bf4505bb9b4bd3d429327dcc52756551aebb2c4a6b23bb77b9c683a257efb
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.5.5.orig.tar.gz' libepoxy_1.5.5.orig.tar.gz 332057 SHA256:5d80a43a6524a1ebdd0c9c5d5105295546a0794681853c636a0c70f8f9c658ce
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.5.5-1.debian.tar.xz' libepoxy_1.5.5-1.debian.tar.xz 17124 SHA256:4a753fdc6165352384031ac77f61f932f570a7500a20d888d546799e18f7d628
```

Other potentially useful URLs:

- https://sources.debian.net/src/libepoxy/1.5.5-1/ (for browsing the source)
- https://sources.debian.net/src/libepoxy/1.5.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libepoxy/1.5.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libepubgen=0.1.1-1`

Binary Packages:

- `libepubgen-0.1-1:amd64=0.1.1-1`

Licenses: (parsed from: `/usr/share/doc/libepubgen-0.1-1/copyright`)

- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libepubgen=0.1.1-1
'http://deb.debian.org/debian/pool/main/libe/libepubgen/libepubgen_0.1.1-1.dsc' libepubgen_0.1.1-1.dsc 2009 SHA256:64381f21242147deecb0bbabefc51b81d25ba7f581c58dc44882354af7337fde
'http://deb.debian.org/debian/pool/main/libe/libepubgen/libepubgen_0.1.1.orig.tar.xz' libepubgen_0.1.1.orig.tar.xz 324380 SHA256:03e084b994cbeffc8c3dd13303b2cb805f44d8f2c3b79f7690d7e3fc7f6215ad
'http://deb.debian.org/debian/pool/main/libe/libepubgen/libepubgen_0.1.1-1.debian.tar.xz' libepubgen_0.1.1-1.debian.tar.xz 2776 SHA256:12f60367c3cc3567039fe7e8a27e71d10caf4768285653ef92f71a6768473ff9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libepubgen/0.1.1-1/ (for browsing the source)
- https://sources.debian.net/src/libepubgen/0.1.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libepubgen/0.1.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libetonyek=0.1.9-4`

Binary Packages:

- `libetonyek-0.1-1:amd64=0.1.9-4`

Licenses: (parsed from: `/usr/share/doc/libetonyek-0.1-1/copyright`)

- `MPL 2.0`

Source:

```console
$ apt-get source -qq --print-uris libetonyek=0.1.9-4
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.9-4.dsc' libetonyek_0.1.9-4.dsc 2202 SHA256:53ea4461a605ba84ab5300ffc8b92cb2bb5454f7f46569111eba5903772c4aad
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.9.orig.tar.xz' libetonyek_0.1.9.orig.tar.xz 1477064 SHA256:e61677e8799ce6e55b25afc11aa5339113f6a49cff031f336e32fa58635b1a4a
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.9-4.debian.tar.xz' libetonyek_0.1.9-4.debian.tar.xz 43372 SHA256:0928958610b525c060704529602547420cf698e872097c45bfd9ccbf7f927cf1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libetonyek/0.1.9-4/ (for browsing the source)
- https://sources.debian.net/src/libetonyek/0.1.9-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libetonyek/0.1.9-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libexttextcat=3.4.5-1`

Binary Packages:

- `libexttextcat-2.0-0:amd64=3.4.5-1`
- `libexttextcat-data=3.4.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libexttextcat=3.4.5-1
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.5-1.dsc' libexttextcat_3.4.5-1.dsc 2099 SHA256:9a5f988e773efec298260e0464df6b4d77b01d82d2a989d317c5529f9c3ac586
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.5.orig.tar.xz' libexttextcat_3.4.5.orig.tar.xz 1041268 SHA256:13fdbc9d4c489a4d0519e51933a1aa21fe3fb9eb7da191b87f7a63e82797dac8
'http://deb.debian.org/debian/pool/main/libe/libexttextcat/libexttextcat_3.4.5-1.debian.tar.xz' libexttextcat_3.4.5-1.debian.tar.xz 7224 SHA256:bf214f4c725d236a8e77b4f7199316255de431eb48638b78f5346890fb3c0849
```

Other potentially useful URLs:

- https://sources.debian.net/src/libexttextcat/3.4.5-1/ (for browsing the source)
- https://sources.debian.net/src/libexttextcat/3.4.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libexttextcat/3.4.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.3-6`

Binary Packages:

- `libffi7:amd64=3.3-6`

Licenses: (parsed from: `/usr/share/doc/libffi7/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.3-6
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-6.dsc' libffi_3.3-6.dsc 1934 SHA256:cb5dcd6b54e0c8c7db4cd97deef68ac9e2ede49138ca5db194b60338eae8dd65
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3.orig.tar.gz' libffi_3.3.orig.tar.gz 1305466 SHA256:72fba7922703ddfa7a028d513ac15a85c8d54c8d67f55fa5a4802885dc652056
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-6.debian.tar.xz' libffi_3.3-6.debian.tar.xz 9168 SHA256:d15879289f32acf2afbbcc6ccf6e0c1aa306f6f06abb8b0301bfa41bffea9a55
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.3-6/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.3-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.3-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libfido2=1.6.0-2`

Binary Packages:

- `libfido2-1:amd64=1.6.0-2`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.6.0-2
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.6.0-2.dsc' libfido2_1.6.0-2.dsc 2565 SHA256:5706f21aa3179124e0e39aeded7519c6536b241ac58457413f36bdbd67cd6cd1
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz' libfido2_1.6.0.orig.tar.gz 413904 SHA256:6aed47aafd22be49c38f9281fb88ccd08c98678d9b8c39cdc87d1bb3ea2c63e4
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz.asc' libfido2_1.6.0.orig.tar.gz.asc 488 SHA256:3340543e15edc67a38850be6777448db33245b5f9f686903d24563a2c7c0d969
'http://deb.debian.org/debian/pool/main/libf/libfido2/libfido2_1.6.0-2.debian.tar.xz' libfido2_1.6.0-2.debian.tar.xz 72700 SHA256:a08adb41d42e64206c5f70f1f2c1510debb37256fe3b92681a0bdc4a73e6d8d2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfido2/1.6.0-2/ (for browsing the source)
- https://sources.debian.net/src/libfido2/1.6.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfido2/1.6.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libfreehand=0.1.2-3`

Binary Packages:

- `libfreehand-0.1-1=0.1.2-3`

Licenses: (parsed from: `/usr/share/doc/libfreehand-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libfreehand=0.1.2-3
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.2-3.dsc' libfreehand_0.1.2-3.dsc 2064 SHA256:b1894483d24c7551e1b2569bb3203863139c3941004de5565dd66f0de0c40adf
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.2.orig.tar.xz' libfreehand_0.1.2.orig.tar.xz 516132 SHA256:0e422d1564a6dbf22a9af598535425271e583514c0f7ba7d9091676420de34ac
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.2-3.debian.tar.xz' libfreehand_0.1.2-3.debian.tar.xz 13488 SHA256:c54b337919ad5f0e748d1e21710d8cd310becef1ce4be4d04bd406f956435bb6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfreehand/0.1.2-3/ (for browsing the source)
- https://sources.debian.net/src/libfreehand/0.1.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfreehand/0.1.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.8.7-6`

Binary Packages:

- `libgcrypt20:amd64=1.8.7-6`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.7-6
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-6.dsc' libgcrypt20_1.8.7-6.dsc 2800 SHA256:af433c97fde6172bb51d458e66acd33c66052bdf78ad72f7034f0b1851015959
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2' libgcrypt20_1.8.7.orig.tar.bz2 2985660 SHA256:03b70f028299561b7034b8966d7dd77ef16ed139c43440925fe8782561974748
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2.asc' libgcrypt20_1.8.7.orig.tar.bz2.asc 228 SHA256:eed6bb4174433640a02c1dc8851f34f85ec55b43d76a24bec87d7175784ef614
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-6.debian.tar.xz' libgcrypt20_1.8.7-6.debian.tar.xz 37564 SHA256:3fe8290b67416579fc99648ba025b8de732c4cc541b60b5f96f53d42a38916f5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.8.7-6/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.8.7-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.8.7-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.38-2`

Binary Packages:

- `libgpg-error0:amd64=1.38-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.38-2
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.38-2.dsc' libgpg-error_1.38-2.dsc 2220 SHA256:ab0ea76aa3552afa664210a871abc74637acafd89c068edf8dc03521b8e22d64
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2' libgpg-error_1.38.orig.tar.bz2 957637 SHA256:d8988275aa69d7149f931c10442e9e34c0242674249e171592b430ff7b3afd02
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2.asc' libgpg-error_1.38.orig.tar.bz2.asc 488 SHA256:d80eb927d85e19e96d8de17552f8f48b517ae7acac7685404e8027475c5b4330
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.38-2.debian.tar.xz' libgpg-error_1.38-2.debian.tar.xz 19544 SHA256:824bcb278ead676c20f174bd551b1cc44a294137fabe6a1d892667882f3b4ba2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.38-2/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.38-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.38-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libidn2=2.3.0-5`

Binary Packages:

- `libidn2-0:amd64=2.3.0-5`

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
$ apt-get source -qq --print-uris libidn2=2.3.0-5
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0-5.dsc' libidn2_2.3.0-5.dsc 2046 SHA256:f8a787741b2395fe87c2773252e539bcc068fde0a5367316082cbbd2fed2be16
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0.orig.tar.gz' libidn2_2.3.0.orig.tar.gz 2164993 SHA256:e1cb1db3d2e249a6a3eb6f0946777c2e892d5c5dc7bd91c74394fc3a01cab8b5
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0-5.debian.tar.xz' libidn2_2.3.0-5.debian.tar.xz 11276 SHA256:e061b97d035e374bc6a948a514c26ad7d1bda31c8147cc8db02e604c82865a15
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.3.0-5/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.3.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.3.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libjpeg-turbo=1:2.0.6-4`

Binary Packages:

- `libjpeg62-turbo:amd64=1:2.0.6-4`

Licenses: (parsed from: `/usr/share/doc/libjpeg62-turbo/copyright`)

- `BSD-3`
- `BSD-BY-LC-NE`
- `Expat`
- `NTP`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:2.0.6-4
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6-4.dsc' libjpeg-turbo_2.0.6-4.dsc 2580 SHA256:fd357f8d1469236ad1f630c185a8af0f76f68c99cd082360148597a479148866
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6.orig.tar.gz' libjpeg-turbo_2.0.6.orig.tar.gz 2192315 SHA256:d74b92ac33b0e3657123ddcf6728788c90dc84dcb6a52013d758af3c4af481bb
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6.orig.tar.gz.asc' libjpeg-turbo_2.0.6.orig.tar.gz.asc 793 SHA256:ab2d95f62c2f25b39823c2b0ee3d72979786f5c310c19943a74eed8c2abc7b4b
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6-4.debian.tar.xz' libjpeg-turbo_2.0.6-4.debian.tar.xz 100860 SHA256:31765ab6f069c8e1f11c0e43fd984dd903506b8eef8b810c06c3f80c796a144c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:2.0.6-4/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:2.0.6-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:2.0.6-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libksba=1.5.0-3`

Binary Packages:

- `libksba8:amd64=1.5.0-3`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.5.0-3
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.5.0-3.dsc' libksba_1.5.0-3.dsc 2470 SHA256:6fd1995d38bd061c81b21ea28fb1f4127b610e18a7deec9214b2bd335bfa93ef
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.5.0.orig.tar.bz2' libksba_1.5.0.orig.tar.bz2 656518 SHA256:ae4af129216b2d7fdea0b5bf2a788cd458a79c983bb09a43f4d525cc87aba0ba
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.5.0.orig.tar.bz2.asc' libksba_1.5.0.orig.tar.bz2.asc 228 SHA256:41a9020381b8201f15b9d7fc2a1abdb90ab2723152d1af0b77a58b12b4884a0f
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.5.0-3.debian.tar.xz' libksba_1.5.0-3.debian.tar.xz 14300 SHA256:ac66ace2752bba3ce8ddfe4f464800da606dcc58862eea493ce88ed341815df4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libksba/1.5.0-3/ (for browsing the source)
- https://sources.debian.net/src/libksba/1.5.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libksba/1.5.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liblangtag=0.6.3-2`

Binary Packages:

- `liblangtag-common=0.6.3-2`
- `liblangtag1:amd64=0.6.3-2`

Licenses: (parsed from: `/usr/share/doc/liblangtag-common/copyright`, `/usr/share/doc/liblangtag1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL | MPL`

Source:

```console
$ apt-get source -qq --print-uris liblangtag=0.6.3-2
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.6.3-2.dsc' liblangtag_0.6.3-2.dsc 2409 SHA256:72824766b526feecaf988328115057cd976009a48df474237a404ddd97f68373
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.6.3.orig.tar.bz2' liblangtag_0.6.3.orig.tar.bz2 755492 SHA256:1f12a20a02ec3a8d22e54dedb8b683a43c9c160bda1ba337bf1060607ae733bd
'http://deb.debian.org/debian/pool/main/libl/liblangtag/liblangtag_0.6.3-2.debian.tar.xz' liblangtag_0.6.3-2.debian.tar.xz 6412 SHA256:c8214a64f326430266feda56b81cdd9fa073b7709a30b8a1aaac639a3aeb524a
```

Other potentially useful URLs:

- https://sources.debian.net/src/liblangtag/0.6.3-2/ (for browsing the source)
- https://sources.debian.net/src/liblangtag/0.6.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liblangtag/0.6.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmd=1.0.3-3`

Binary Packages:

- `libmd0:amd64=1.0.3-3`

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
$ apt-get source -qq --print-uris libmd=1.0.3-3
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.3-3.dsc' libmd_1.0.3-3.dsc 2248 SHA256:c3be656dc94c906898358e1d27394e1aec1769a0b5e09e8a4e8cace735ce9967
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.3.orig.tar.xz' libmd_1.0.3.orig.tar.xz 258584 SHA256:5a02097f95cc250a3f1001865e4dbba5f1d15554120f95693c0541923c52af4a
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.3.orig.tar.xz.asc' libmd_1.0.3.orig.tar.xz.asc 833 SHA256:690c82c27026093e0367b24de5f786b29f6cedacbae67bad3199190689940d3d
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.3-3.debian.tar.xz' libmd_1.0.3-3.debian.tar.xz 10104 SHA256:90f09c473c5ff61e3d937c656f12470610cc731cf9061490f651293d04f3c385
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmd/1.0.3-3/ (for browsing the source)
- https://sources.debian.net/src/libmd/1.0.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmd/1.0.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmspub=0.1.4-3`

Binary Packages:

- `libmspub-0.1-1:amd64=0.1.4-3+b1`

Licenses: (parsed from: `/usr/share/doc/libmspub-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libmspub=0.1.4-3
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.4-3.dsc' libmspub_0.1.4-3.dsc 2130 SHA256:e39be3895ac53886b5f0a240dcd5f296568d14cc386866f98f3b9104f746dbf8
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.4.orig.tar.xz' libmspub_0.1.4.orig.tar.xz 377472 SHA256:ef36c1a1aabb2ba3b0bedaaafe717bf4480be2ba8de6f3894be5fd3702b013ba
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.4-3.debian.tar.xz' libmspub_0.1.4-3.debian.tar.xz 7452 SHA256:3a8337582681ee7341310b150694d92f2e7239625c000d941850d598ecc7468d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmspub/0.1.4-3/ (for browsing the source)
- https://sources.debian.net/src/libmspub/0.1.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmspub/0.1.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmwaw=0.3.17-1`

Binary Packages:

- `libmwaw-0.3-3:amd64=0.3.17-1`

Licenses: (parsed from: `/usr/share/doc/libmwaw-0.3-3/copyright`)

- `BSD`
- `LGPL`
- `MPL2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmwaw=0.3.17-1
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.17-1.dsc' libmwaw_0.3.17-1.dsc 2100 SHA256:e0fac2c4504ac8e4ab928e1efb0ee4e6639b10a17b29b08d924849d465a16031
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.17.orig.tar.bz2' libmwaw_0.3.17.orig.tar.bz2 1678698 SHA256:8f81cc27b63d508576a43ef7448f78bec2fde7c7349b08273400e4de897f651c
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.17-1.debian.tar.xz' libmwaw_0.3.17-1.debian.tar.xz 8228 SHA256:7688c554e9e86130d014a33f707ac643598265393d1d387d4a4e82c3b68712c2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmwaw/0.3.17-1/ (for browsing the source)
- https://sources.debian.net/src/libmwaw/0.3.17-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmwaw/0.3.17-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libnumbertext=1.0.7-1`

Binary Packages:

- `libnumbertext-1.0-0:amd64=1.0.7-1`
- `libnumbertext-data=1.0.7-1`

Licenses: (parsed from: `/usr/share/doc/libnumbertext-1.0-0/copyright`, `/usr/share/doc/libnumbertext-data/copyright`)

- `BSD-3-clause`
- `CC-BY-SA-3.0`
- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libnumbertext=1.0.7-1
'http://deb.debian.org/debian/pool/main/libn/libnumbertext/libnumbertext_1.0.7-1.dsc' libnumbertext_1.0.7-1.dsc 2455 SHA256:f156de5ed6466c72f185e26b059082f851412fba3831732e5fe0cf66d21ced2a
'http://deb.debian.org/debian/pool/main/libn/libnumbertext/libnumbertext_1.0.7.orig.tar.gz' libnumbertext_1.0.7.orig.tar.gz 423658 SHA256:5ea8359532d7b8d7a1b63ccc7825fb3b4f8c6dcdee75cb80206d9647c50d4a03
'http://deb.debian.org/debian/pool/main/libn/libnumbertext/libnumbertext_1.0.7-1.debian.tar.xz' libnumbertext_1.0.7-1.debian.tar.xz 12288 SHA256:3cf06ba55cd3455d9bc6bc43f56ae8cf207c8ea33218469aecfaa9b269fd7eb0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libnumbertext/1.0.7-1/ (for browsing the source)
- https://sources.debian.net/src/libnumbertext/1.0.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libnumbertext/1.0.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libodfgen=0.1.8-2`

Binary Packages:

- `libodfgen-0.1-1:amd64=0.1.8-2`

Licenses: (parsed from: `/usr/share/doc/libodfgen-0.1-1/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libodfgen=0.1.8-2
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.8-2.dsc' libodfgen_0.1.8-2.dsc 1976 SHA256:f9223da50ed9a408ab6bc9e639c96b649aa81726898b99f27924ee59cbd3349a
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.8.orig.tar.xz' libodfgen_0.1.8.orig.tar.xz 386156 SHA256:55200027fd46623b9bdddd38d275e7452d1b0ff8aeddcad6f9ae6dc25f610625
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.8-2.debian.tar.xz' libodfgen_0.1.8-2.debian.tar.xz 6956 SHA256:c7d7cb9f3a8449ff17d53b08996fe68956e9d7759a62ea5ec466dcf8899289e5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libodfgen/0.1.8-2/ (for browsing the source)
- https://sources.debian.net/src/libodfgen/0.1.8-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libodfgen/0.1.8-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liborcus=0.16.1-3`

Binary Packages:

- `liborcus-0.16-0:amd64=0.16.1-3+b2`
- `liborcus-parser-0.16-0:amd64=0.16.1-3+b2`

Licenses: (parsed from: `/usr/share/doc/liborcus-0.16-0/copyright`, `/usr/share/doc/liborcus-parser-0.16-0/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris liborcus=0.16.1-3
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.16.1-3.dsc' liborcus_0.16.1-3.dsc 2922 SHA256:99eedb5abaf00d3431dd05037cc12c5b0687fe367bebd7c04b7f42584a880467
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.16.1.orig.tar.xz' liborcus_0.16.1.orig.tar.xz 1805436 SHA256:a4b26b320d00bdfc769c3a03ed22bd5ad7e54a93dc6b1d00cd949f8f3519faae
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.16.1-3.debian.tar.xz' liborcus_0.16.1-3.debian.tar.xz 8672 SHA256:3740d34b43784e6710e8b8a32bdd0d5510ef9675b017a1672e4fbc3c898d9c7a
```

Other potentially useful URLs:

- https://sources.debian.net/src/liborcus/0.16.1-3/ (for browsing the source)
- https://sources.debian.net/src/liborcus/0.16.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liborcus/0.16.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpagemaker=0.0.4-1`

Binary Packages:

- `libpagemaker-0.0-0:amd64=0.0.4-1`

Licenses: (parsed from: `/usr/share/doc/libpagemaker-0.0-0/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libpagemaker=0.0.4-1
'http://deb.debian.org/debian/pool/main/libp/libpagemaker/libpagemaker_0.0.4-1.dsc' libpagemaker_0.0.4-1.dsc 2008 SHA256:fc7040296e01d0175dbf4ed2fc4ff75aec1ec8bd07db9b4323680b8501075e63
'http://deb.debian.org/debian/pool/main/libp/libpagemaker/libpagemaker_0.0.4.orig.tar.xz' libpagemaker_0.0.4.orig.tar.xz 306496 SHA256:66adacd705a7d19895e08eac46d1e851332adf2e736c566bef1164e7a442519d
'http://deb.debian.org/debian/pool/main/libp/libpagemaker/libpagemaker_0.0.4-1.debian.tar.xz' libpagemaker_0.0.4-1.debian.tar.xz 6628 SHA256:02f9cfbf5c9bba7ff914afcb8829c45047eff5a56107598216e761861b82999a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpagemaker/0.0.4-1/ (for browsing the source)
- https://sources.debian.net/src/libpagemaker/0.0.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpagemaker/0.0.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpgjava=42.2.15-1`

Binary Packages:

- `libpostgresql-jdbc-java=42.2.15-1`

Licenses: (parsed from: `/usr/share/doc/libpostgresql-jdbc-java/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libpgjava=42.2.15-1
'http://deb.debian.org/debian/pool/main/libp/libpgjava/libpgjava_42.2.15-1.dsc' libpgjava_42.2.15-1.dsc 2560 SHA256:cc4d1d8ef1018db755bbc9e37e78073040693eeb4eb8ecd073af2b723e8764fa
'http://deb.debian.org/debian/pool/main/libp/libpgjava/libpgjava_42.2.15.orig.tar.gz' libpgjava_42.2.15.orig.tar.gz 903018 SHA256:fd34f1d133bf9df29fa853bea44029ba22b00a478984d7233fb6218b66d47a8f
'http://deb.debian.org/debian/pool/main/libp/libpgjava/libpgjava_42.2.15-1.debian.tar.xz' libpgjava_42.2.15-1.debian.tar.xz 9728 SHA256:1534ebffd429fb777ccb9504502a9d364765d05c0b5000705e1d99a26d0a558e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpgjava/42.2.15-1/ (for browsing the source)
- https://sources.debian.net/src/libpgjava/42.2.15-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpgjava/42.2.15-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng1.6=1.6.37-3`

Binary Packages:

- `libpng16-16:amd64=1.6.37-3`

Licenses: (parsed from: `/usr/share/doc/libpng16-16/copyright`)

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

### `dpkg` source package: `libqxp=0.0.2-1`

Binary Packages:

- `libqxp-0.0-0=0.0.2-1+b1`

Licenses: (parsed from: `/usr/share/doc/libqxp-0.0-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libqxp=0.0.2-1
'http://deb.debian.org/debian/pool/main/libq/libqxp/libqxp_0.0.2-1.dsc' libqxp_0.0.2-1.dsc 2064 SHA256:5c1e948a963af671c6014ab4e61c3bf63a3d96a0dd01f53493817386b2debc34
'http://deb.debian.org/debian/pool/main/libq/libqxp/libqxp_0.0.2.orig.tar.xz' libqxp_0.0.2.orig.tar.xz 341760 SHA256:e137b6b110120a52c98edd02ebdc4095ee08d0d5295a94316a981750095a945c
'http://deb.debian.org/debian/pool/main/libq/libqxp/libqxp_0.0.2-1.debian.tar.xz' libqxp_0.0.2-1.debian.tar.xz 2192 SHA256:42d72c086e3273dc1aa84fc3254c26a09657e0170fb002543a7b7744a13b44ad
```

Other potentially useful URLs:

- https://sources.debian.net/src/libqxp/0.0.2-1/ (for browsing the source)
- https://sources.debian.net/src/libqxp/0.0.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libqxp/0.0.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libreoffice=1:7.0.4-4+deb11u1`

Binary Packages:

- `fonts-opensymbol=2:102.11+LibO7.0.4-4+deb11u1`
- `libreoffice=1:7.0.4-4+deb11u1`
- `libreoffice-base=1:7.0.4-4+deb11u1`
- `libreoffice-base-core=1:7.0.4-4+deb11u1`
- `libreoffice-base-drivers=1:7.0.4-4+deb11u1`
- `libreoffice-calc=1:7.0.4-4+deb11u1`
- `libreoffice-common=1:7.0.4-4+deb11u1`
- `libreoffice-core=1:7.0.4-4+deb11u1`
- `libreoffice-draw=1:7.0.4-4+deb11u1`
- `libreoffice-impress=1:7.0.4-4+deb11u1`
- `libreoffice-math=1:7.0.4-4+deb11u1`
- `libreoffice-report-builder-bin=1:7.0.4-4+deb11u1`
- `libreoffice-style-colibre=1:7.0.4-4+deb11u1`
- `libreoffice-writer=1:7.0.4-4+deb11u1`
- `libuno-cppu3=1:7.0.4-4+deb11u1`
- `libuno-cppuhelpergcc3-3=1:7.0.4-4+deb11u1`
- `libuno-purpenvhelpergcc3-3=1:7.0.4-4+deb11u1`
- `libuno-sal3=1:7.0.4-4+deb11u1`
- `libuno-salhelpergcc3-3=1:7.0.4-4+deb11u1`
- `python3-uno=1:7.0.4-4+deb11u1`
- `uno-libs-private=1:7.0.4-4+deb11u1`
- `ure=1:7.0.4-4+deb11u1`

Licenses: (parsed from: `/usr/share/doc/fonts-opensymbol/copyright`, `/usr/share/doc/libreoffice/copyright`, `/usr/share/doc/libreoffice-base/copyright`, `/usr/share/doc/libreoffice-base-core/copyright`, `/usr/share/doc/libreoffice-base-drivers/copyright`, `/usr/share/doc/libreoffice-calc/copyright`, `/usr/share/doc/libreoffice-common/copyright`, `/usr/share/doc/libreoffice-core/copyright`, `/usr/share/doc/libreoffice-draw/copyright`, `/usr/share/doc/libreoffice-impress/copyright`, `/usr/share/doc/libreoffice-math/copyright`, `/usr/share/doc/libreoffice-report-builder-bin/copyright`, `/usr/share/doc/libreoffice-style-colibre/copyright`, `/usr/share/doc/libreoffice-writer/copyright`, `/usr/share/doc/libuno-cppu3/copyright`, `/usr/share/doc/libuno-cppuhelpergcc3-3/copyright`, `/usr/share/doc/libuno-purpenvhelpergcc3-3/copyright`, `/usr/share/doc/libuno-sal3/copyright`, `/usr/share/doc/libuno-salhelpergcc3-3/copyright`, `/usr/share/doc/python3-uno/copyright`, `/usr/share/doc/uno-libs-private/copyright`, `/usr/share/doc/ure/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `CC-BY-SA-3.0 `
- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-3`
- `LGPL-3+`
- `MPL-1.1`
- `MPL-2.0`
- `MPL_2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libreoffice=1:7.0.4-4+deb11u1
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_7.0.4-4%2bdeb11u1.dsc' libreoffice_7.0.4-4+deb11u1.dsc 31345 SHA256:22f3b5af8a498e4993488e024768d0bc268fa113e873bdecd976ea8b836f5028
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_7.0.4.orig-helpcontent2.tar.xz' libreoffice_7.0.4.orig-helpcontent2.tar.xz 110142616 SHA256:8311462f214e27841ba4970bbae518b9a4b2088380877b8dff5e2005587357c1
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_7.0.4.orig-translations.tar.xz' libreoffice_7.0.4.orig-translations.tar.xz 176691588 SHA256:28d7421771af20a310983dec5c64da8103eb6a159e098c6e5f1a1c1e6731e146
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_7.0.4.orig.tar.xz' libreoffice_7.0.4.orig.tar.xz 236477520 SHA256:9fa9d2cc8d02f12b1f302b93056d5c0ff986090a6f309bafa506ba53779f2abd
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_7.0.4.orig.tar.xz.asc' libreoffice_7.0.4.orig.tar.xz.asc 833 SHA256:773a0034f2f4a26e3e285ac605e704df6d90b06722af64b95e42ea4452a34b91
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_7.0.4-4%2bdeb11u1.debian.tar.xz' libreoffice_7.0.4-4+deb11u1.debian.tar.xz 19507204 SHA256:8b406e49643e9cb8343bb22d2a59d18ff6cf8c4f71e9cff42243ca5c64a3fdcd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libreoffice/1:7.0.4-4+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/libreoffice/1:7.0.4-4+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libreoffice/1:7.0.4-4+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `librevenge=0.0.4-6`

Binary Packages:

- `librevenge-0.0-0:amd64=0.0.4-6+b1`

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

### `dpkg` source package: `libseccomp=2.5.1-1+deb11u1`

Binary Packages:

- `libseccomp2:amd64=2.5.1-1+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.1-1+deb11u1
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1-1%2bdeb11u1.dsc' libseccomp_2.5.1-1+deb11u1.dsc 2708 SHA256:6a2a00eb5f45e794a2203805348a3990d46f4ded63f8708d3382994ece729436
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1.orig.tar.gz' libseccomp_2.5.1.orig.tar.gz 638811 SHA256:ee307e383c77aa7995abc5ada544d51c9723ae399768a97667d4cdb3c3a30d55
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1.orig.tar.gz.asc' libseccomp_2.5.1.orig.tar.gz.asc 833 SHA256:14d45c86e5ceed5ac5511c3ebf70a4dca128b7584b314dc8a551c779ea225d2e
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1-1%2bdeb11u1.debian.tar.xz' libseccomp_2.5.1-1+deb11u1.debian.tar.xz 19524 SHA256:a09ef7c0b9b6464f426b78a7b978d8566da53667c1a234234ffd2cc600543200
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.5.1-1+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.5.1-1+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.5.1-1+deb11u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libssh2=1.9.0-2`

Binary Packages:

- `libssh2-1:amd64=1.9.0-2`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.9.0-2
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.9.0-2.dsc' libssh2_1.9.0-2.dsc 2007 SHA256:fbf9500e064cdd307a634772d0d417de910fcba874e3edbb72cce538f0389a11
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.9.0.orig.tar.gz' libssh2_1.9.0.orig.tar.gz 888551 SHA256:d5fb8bd563305fd1074dda90bd053fb2d29fc4bce048d182f96eaa466dfadafd
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.9.0-2.debian.tar.xz' libssh2_1.9.0-2.debian.tar.xz 9116 SHA256:7081ec54751720082d3f95ef73e2b52a46f72a67ab765932576c11aeb54df7d9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.9.0-2/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.9.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.9.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libstaroffice=0.0.7-1`

Binary Packages:

- `libstaroffice-0.0-0:amd64=0.0.7-1`

Licenses: (parsed from: `/usr/share/doc/libstaroffice-0.0-0/copyright`)

- `BSD`
- `LGPL`
- `MPL2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libstaroffice=0.0.7-1
'http://deb.debian.org/debian/pool/main/libs/libstaroffice/libstaroffice_0.0.7-1.dsc' libstaroffice_0.0.7-1.dsc 2183 SHA256:0983b2b5192102d484d5b387f6ac8058f4ffe3f9af97e0ad827c7d9440610e3d
'http://deb.debian.org/debian/pool/main/libs/libstaroffice/libstaroffice_0.0.7.orig.tar.gz' libstaroffice_0.0.7.orig.tar.gz 6573700 SHA256:4599b17fa991bd8c0304fe879afc6672cc2154a7d1137799a014971a225c2d73
'http://deb.debian.org/debian/pool/main/libs/libstaroffice/libstaroffice_0.0.7-1.debian.tar.xz' libstaroffice_0.0.7-1.debian.tar.xz 8156 SHA256:827fb03eb11c1bc07611c4c325437e25b596681ec6ccabc094311bf657d6c5ff
```

Other potentially useful URLs:

- https://sources.debian.net/src/libstaroffice/0.0.7-1/ (for browsing the source)
- https://sources.debian.net/src/libstaroffice/0.0.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libstaroffice/0.0.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.16.0-2`

Binary Packages:

- `libtasn1-6:amd64=4.16.0-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

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

### `dpkg` source package: `libtirpc=1.3.1-1`

Binary Packages:

- `libtirpc-common=1.3.1-1`
- `libtirpc3:amd64=1.3.1-1`

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
$ apt-get source -qq --print-uris libtirpc=1.3.1-1
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.1-1.dsc' libtirpc_1.3.1-1.dsc 2111 SHA256:b143e375f621a5a64858c068692304febe222da8f648b89254507eda3e97c68a
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.1.orig.tar.bz2' libtirpc_1.3.1.orig.tar.bz2 513399 SHA256:245895caf066bec5e3d4375942c8cb4366adad184c29c618d97f724ea309ee17
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.1-1.debian.tar.xz' libtirpc_1.3.1-1.debian.tar.xz 10788 SHA256:5012cff4ebc5db473b4fb29e1661bde4354c25b2e23a05df28d2f03ba0547881
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtirpc/1.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/libtirpc/1.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtirpc/1.3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtool=2.4.6-15`

Binary Packages:

- `libltdl7:amd64=2.4.6-15`

Licenses: (parsed from: `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-15
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-15.dsc' libtool_2.4.6-15.dsc 2502 SHA256:c499bd88103239f5d9743c70fd9e84260b0237e43df47c44980ef4ac9ff5f8e0
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-15.debian.tar.xz' libtool_2.4.6-15.debian.tar.xz 53924 SHA256:3955615804746d1440f2880f5cc0cd19e50dbaffe689afbec45dfcaaf5ee0d35
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtool/2.4.6-15/ (for browsing the source)
- https://sources.debian.net/src/libtool/2.4.6-15/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtool/2.4.6-15/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=0.9.10-4`

Binary Packages:

- `libunistring2:amd64=0.9.10-4`

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
$ apt-get source -qq --print-uris libunistring=0.9.10-4
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-4.dsc' libunistring_0.9.10-4.dsc 2212 SHA256:5c7940807b538d4204506349cbd67e5c677afb9f0e46e94455353e3f746a481e
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-4.debian.tar.xz' libunistring_0.9.10-4.debian.tar.xz 40936 SHA256:6c9554e1a1c6d0a02ca4868a5422d176e57a3131c1a8a21de5503b164997525c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/0.9.10-4/ (for browsing the source)
- https://sources.debian.net/src/libunistring/0.9.10-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/0.9.10-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunwind=1.3.2-2`

Binary Packages:

- `libunwind8:amd64=1.3.2-2`

Licenses: (parsed from: `/usr/share/doc/libunwind8/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libunwind=1.3.2-2
'http://deb.debian.org/debian/pool/main/libu/libunwind/libunwind_1.3.2-2.dsc' libunwind_1.3.2-2.dsc 2793 SHA256:9a84747321445af8539a8ffba61791f8ecad5e058db5bf9b401067dd05c573ba
'http://deb.debian.org/debian/pool/main/libu/libunwind/libunwind_1.3.2.orig.tar.gz' libunwind_1.3.2.orig.tar.gz 854114 SHA256:0a4b5a78d8c0418dfa610245f75fa03ad45d8e5e4cc091915d2dbed34c01178e
'http://deb.debian.org/debian/pool/main/libu/libunwind/libunwind_1.3.2.orig.tar.gz.asc' libunwind_1.3.2.orig.tar.gz.asc 659 SHA256:5c1ffad1980acc92536a35643afba3f0e395b2a953fb898fda3403dae8fbd6ef
'http://deb.debian.org/debian/pool/main/libu/libunwind/libunwind_1.3.2-2.debian.tar.xz' libunwind_1.3.2-2.debian.tar.xz 19952 SHA256:87c03a5b832f59fa4984f4fb8a2bf02aabc6075b1d7002331e6b19008eac7c95
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunwind/1.3.2-2/ (for browsing the source)
- https://sources.debian.net/src/libunwind/1.3.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunwind/1.3.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvisio=0.1.7-1`

Binary Packages:

- `libvisio-0.1-1:amd64=0.1.7-1+b1`

Licenses: (parsed from: `/usr/share/doc/libvisio-0.1-1/copyright`)

- `MIT | GPL-2`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libvisio=0.1.7-1
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.7-1.dsc' libvisio_0.1.7-1.dsc 2213 SHA256:61eaf3865704e12520640233be381b093fac33408ee701d504c93fb1f8b87e48
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.7.orig.tar.xz' libvisio_0.1.7.orig.tar.xz 854296 SHA256:8faf8df870cb27b09a787a1959d6c646faa44d0d8ab151883df408b7166bea4c
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.7-1.debian.tar.xz' libvisio_0.1.7-1.debian.tar.xz 8112 SHA256:1731dd1fa9f9d16da62b20d9f73b13a544c1925ffe2c5f0d0f6d5f238770e615
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvisio/0.1.7-1/ (for browsing the source)
- https://sources.debian.net/src/libvisio/0.1.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvisio/0.1.7-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libwpd=0.10.3-1`

Binary Packages:

- `libwpd-0.10-10:amd64=0.10.3-1`

Licenses: (parsed from: `/usr/share/doc/libwpd-0.10-10/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libwpd=0.10.3-1
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.3-1.dsc' libwpd_0.10.3-1.dsc 2049 SHA256:b20fa136afa403bfcd872710487a2f776ecc2df78572300cc9c07abdab8ca6b8
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.3.orig.tar.xz' libwpd_0.10.3.orig.tar.xz 534712 SHA256:2465b0b662fdc5d4e3bebcdc9a79027713fb629ca2bff04a3c9251fdec42dd09
'http://deb.debian.org/debian/pool/main/libw/libwpd/libwpd_0.10.3-1.debian.tar.xz' libwpd_0.10.3-1.debian.tar.xz 11544 SHA256:ed31d59da916d0a7ddda6a323b2a06efdf6101113310b604076ee22cc00be859
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwpd/0.10.3-1/ (for browsing the source)
- https://sources.debian.net/src/libwpd/0.10.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwpd/0.10.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwpg=0.3.3-1`

Binary Packages:

- `libwpg-0.3-3:amd64=0.3.3-1`

Licenses: (parsed from: `/usr/share/doc/libwpg-0.3-3/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libwpg=0.3.3-1
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.3-1.dsc' libwpg_0.3.3-1.dsc 2021 SHA256:0e63ca0563855fe11c4969982047610bd3693783c4cf664e7eacac0c999afaf4
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.3.orig.tar.xz' libwpg_0.3.3.orig.tar.xz 328664 SHA256:99b3f7f8832385748582ab8130fbb9e5607bd5179bebf9751ac1d51a53099d1c
'http://deb.debian.org/debian/pool/main/libw/libwpg/libwpg_0.3.3-1.debian.tar.xz' libwpg_0.3.3-1.debian.tar.xz 9232 SHA256:c27d4b0cb9a474764af7a2b958cba55c5d5297313598f6c8501024d1651a6509
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwpg/0.3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libwpg/0.3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwpg/0.3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwps=0.4.12-1`

Binary Packages:

- `libwps-0.4-4:amd64=0.4.12-1`

Licenses: (parsed from: `/usr/share/doc/libwps-0.4-4/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwps=0.4.12-1
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.12-1.dsc' libwps_0.4.12-1.dsc 2263 SHA256:7ede52ba028854dfad74d8fbb0dd83d8da8de2d0238c1e1ee83f185259a74089
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.12.orig.tar.xz' libwps_0.4.12.orig.tar.xz 713008 SHA256:e21afb52a06d03b774c5a8c72679687ab64891b91ce0c3bdf2d3e97231534edb
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.12-1.debian.tar.xz' libwps_0.4.12-1.debian.tar.xz 9068 SHA256:3167bae70bd8daa1a42c591415d8697b8b1cd560fa6e1bd63e3acf2f35835c6b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwps/0.4.12-1/ (for browsing the source)
- https://sources.debian.net/src/libwps/0.4.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwps/0.4.12-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.7.2-1`

Binary Packages:

- `libx11-6:amd64=2:1.7.2-1`
- `libx11-data=2:1.7.2-1`
- `libx11-xcb1:amd64=2:1.7.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.7.2-1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2-1.dsc' libx11_1.7.2-1.dsc 2539 SHA256:8db8a34ebf9782d4ef47cb28cfeae0b1bc737864a315a182871eeb29f7de7d90
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz' libx11_1.7.2.orig.tar.gz 3181228 SHA256:2c26ccd08f43a6214de89110554fbe97c71692eeb7e7d4829f3004ae6fafd2c0
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz.asc' libx11_1.7.2.orig.tar.gz.asc 833 SHA256:509d0ed983ff3aed0dbfb070dabfce82b5787e626f2fd0bfb2a5887918fcd967
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.2-1.diff.gz' libx11_1.7.2-1.diff.gz 76026 SHA256:7babff68e071a9e3f7bc6241a1a135e3a19c74314240764722a41b31f1e213c8
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.7.2-1/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.7.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.7.2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxcrypt=1:4.4.18-4`

Binary Packages:

- `libcrypt1:amd64=1:4.4.18-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.18-4
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.18-4.dsc' libxcrypt_4.4.18-4.dsc 1477 SHA256:5c0ca54ddad5343596f6c0916caf30fbb9b8a144252b49dc74f97502f33cdb7a
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.18.orig.tar.xz' libxcrypt_4.4.18.orig.tar.xz 397776 SHA256:4cd2a06e98519d57a5572ee8885b6cc23c70a559d234c161d3f22c487edaa3fa
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.18-4.debian.tar.xz' libxcrypt_4.4.18-4.debian.tar.xz 7560 SHA256:6c99b888c57e1411d870fa81d057e30444aa801ed430aa3126d31996e187dd84
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.18-4/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.18-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.18-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxext=2:1.3.3-1.1`

Binary Packages:

- `libxext6:amd64=2:1.3.3-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.3-1.1
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.1.dsc' libxext_1.3.3-1.1.dsc 2243 SHA256:ae9f97003e38da180294f43a8217991df709955dd7576c5333e2412f264f8697
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3.orig.tar.gz' libxext_1.3.3.orig.tar.gz 468441 SHA256:eb0b88050491fef4716da4b06a4d92b4fc9e76f880d6310b2157df604342cfe5
'http://deb.debian.org/debian/pool/main/libx/libxext/libxext_1.3.3-1.1.diff.gz' libxext_1.3.3-1.1.diff.gz 20628 SHA256:6a8ce08c667c4631c59bc79c716187dc7ed20bb7d0967701ab21313e6dd6c752
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxext/2:1.3.3-1.1/ (for browsing the source)
- https://sources.debian.net/src/libxext/2:1.3.3-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxext/2:1.3.3-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxinerama=2:1.1.4-2`

Binary Packages:

- `libxinerama1:amd64=2:1.1.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxinerama=2:1.1.4-2
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.4-2.dsc' libxinerama_1.1.4-2.dsc 2100 SHA256:02e4c8406fd1eae8abfe356894d95d610e2e612a761688ef5afe5e7c60d162e9
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.4.orig.tar.gz' libxinerama_1.1.4.orig.tar.gz 380740 SHA256:64de45e18cc76b8e703cb09b3c9d28bd16e3d05d5cd99f2d630de2d62c3acc18
'http://deb.debian.org/debian/pool/main/libx/libxinerama/libxinerama_1.1.4-2.diff.gz' libxinerama_1.1.4-2.diff.gz 8732 SHA256:06ce6602862839ded43d914d7dd5e5bcd7d7a1477c775f5f47a6c20b1c9b52b6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxinerama/2:1.1.4-2/ (for browsing the source)
- https://sources.debian.net/src/libxinerama/2:1.1.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxinerama/2:1.1.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxml2=2.9.10+dfsg-6.7+deb11u1`

Binary Packages:

- `libxml2:amd64=2.9.10+dfsg-6.7+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.10+dfsg-6.7+deb11u1
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.10%2bdfsg-6.7%2bdeb11u1.dsc' libxml2_2.9.10+dfsg-6.7+deb11u1.dsc 2859 SHA256:48ff26e6dc163adb7ce30b8c0a6c261568e3806d6deaaf860fd11abb64afea1c
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.10%2bdfsg.orig.tar.xz' libxml2_2.9.10+dfsg.orig.tar.xz 2503560 SHA256:65ee7a2f5e100c64ddf7beb92297c9b2a30b994a76cd1fab67470cf22db6b7d0
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.10%2bdfsg-6.7%2bdeb11u1.debian.tar.xz' libxml2_2.9.10+dfsg-6.7+deb11u1.debian.tar.xz 34092 SHA256:405c16306e60f1ad32ebe884dd294bf1f17cd0f3b89dacf7f52faff53af1c7a0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxml2/2.9.10+dfsg-6.7+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/libxml2/2.9.10+dfsg-6.7+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxml2/2.9.10+dfsg-6.7+deb11u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxslt=1.1.34-4`

Binary Packages:

- `libxslt1.1:amd64=1.1.34-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.34-4
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34-4.dsc' libxslt_1.1.34-4.dsc 2375 SHA256:29447f928b2fd534bd819aaf74005ff286f3786689a2684b9cbc61c1c65c2212
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA256:98b1bd46d6792925ad2dfe9a87452ea2adebf69dcb9919ffd55bf926a7f93f7f
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA256:673d1477552bdd5b0cc665704e77ca70e6be5d2f257e6a5a341c846719d747cf
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.34-4.debian.tar.xz' libxslt_1.1.34-4.debian.tar.xz 21464 SHA256:24d5490d6e33f42391d2ce449dd8fec0830ced115a6af886ee03af985a727dc9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxslt/1.1.34-4/ (for browsing the source)
- https://sources.debian.net/src/libxslt/1.1.34-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxslt/1.1.34-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzmf=0.0.2-1`

Binary Packages:

- `libzmf-0.0-0:amd64=0.0.2-1+b3`

Licenses: (parsed from: `/usr/share/doc/libzmf-0.0-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libzmf=0.0.2-1
'http://deb.debian.org/debian/pool/main/libz/libzmf/libzmf_0.0.2-1.dsc' libzmf_0.0.2-1.dsc 2039 SHA256:90c657f960d6b94f73b3d250b3069f1f45f95f8fd4564fcf222a7b4cccd3a097
'http://deb.debian.org/debian/pool/main/libz/libzmf/libzmf_0.0.2.orig.tar.xz' libzmf_0.0.2.orig.tar.xz 320952 SHA256:27051a30cb057fdb5d5de65a1f165c7153dc76e27fe62251cbb86639eb2caf22
'http://deb.debian.org/debian/pool/main/libz/libzmf/libzmf_0.0.2-1.debian.tar.xz' libzmf_0.0.2-1.debian.tar.xz 7648 SHA256:b729bbffd63703b3a3c3bf24a4a4093e5ddacd6cad4c369e340f932b4406eb27
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzmf/0.0.2-1/ (for browsing the source)
- https://sources.debian.net/src/libzmf/0.0.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzmf/0.0.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.4.8+dfsg-2.1`

Binary Packages:

- `libzstd1:amd64=1.4.8+dfsg-2.1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.8+dfsg-2.1
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-2.1.dsc' libzstd_1.4.8+dfsg-2.1.dsc 2274 SHA256:7c656b8cab7a560710358dddbd949b33b1ffcedd7cbef370132e4018b94e2e74
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA256:1e8ce5c4880a6d5bd8d3186e4186607dd19b64fc98a3877fc13aeefd566d67c5
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-2.1.debian.tar.xz' libzstd_1.4.8+dfsg-2.1.debian.tar.xz 12224 SHA256:cba8544590e59303277e3af2bb260fed32723a1084c9f4928956deca2c80032c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.4.8+dfsg-2.1/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.4.8+dfsg-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.4.8+dfsg-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lp-solve=5.5.2.5-2`

Binary Packages:

- `lp-solve=5.5.2.5-2`

Licenses: (parsed from: `/usr/share/doc/lp-solve/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris lp-solve=5.5.2.5-2
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.2.5-2.dsc' lp-solve_5.5.2.5-2.dsc 2268 SHA256:530ec3fd85695622b252433b96d309c20d6abf2d47926d633b19d56cb26d9613
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.2.5.orig-doc.tar.gz' lp-solve_5.5.2.5.orig-doc.tar.gz 1448749 SHA256:4c6085a7083cca04c18876a1c8838ae2427b97080219fffedde1c3a96bc13561
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.2.5.orig.tar.gz' lp-solve_5.5.2.5.orig.tar.gz 812947 SHA256:201a7c62b8b3360c884ee2a73ed7667e5716fc1e809755053b398c2f5b0cf28a
'http://deb.debian.org/debian/pool/main/l/lp-solve/lp-solve_5.5.2.5-2.debian.tar.xz' lp-solve_5.5.2.5-2.debian.tar.xz 16376 SHA256:0cf488a6f378663933cf661e2ee3c0ae02c220a22d74fe9c627c749058bd1ce4
```

Other potentially useful URLs:

- https://sources.debian.net/src/lp-solve/5.5.2.5-2/ (for browsing the source)
- https://sources.debian.net/src/lp-solve/5.5.2.5-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lp-solve/5.5.2.5-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `media-types=4.0.0`

Binary Packages:

- `media-types=4.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=4.0.0
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_4.0.0.dsc' media-types_4.0.0.dsc 1620 SHA256:422edc1275dcc6bf07ac1b30612f501624cba04cfca2331eb87f1ca3af89e701
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_4.0.0.tar.xz' media-types_4.0.0.tar.xz 33988 SHA256:b5eb14fd6addb8f10c1665ebaa113cd0ebfb47f692cf27d9ac47405b13ce4e31
```

Other potentially useful URLs:

- https://sources.debian.net/src/media-types/4.0.0/ (for browsing the source)
- https://sources.debian.net/src/media-types/4.0.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/media-types/4.0.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mercurial=5.6.1-4`

Binary Packages:

- `mercurial=5.6.1-4`
- `mercurial-common=5.6.1-4`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=5.6.1-4
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.6.1-4.dsc' mercurial_5.6.1-4.dsc 2130 SHA256:d8930b0d0b8a4d1adc2951ef521a6194f07a2a0ef923cdfbf73fe109658a0311
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.6.1.orig.tar.gz' mercurial_5.6.1.orig.tar.gz 7836342 SHA256:e55c254f4904c45226a106780e57f4279aee03368f6ff6a981d5d2a38243ffad
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.6.1.orig.tar.gz.asc' mercurial_5.6.1.orig.tar.gz.asc 833 SHA256:bef5ca673b6fe7ab213e07826c2196dd41710df4739f9a49e57dc3d3d38a6d36
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_5.6.1-4.debian.tar.xz' mercurial_5.6.1-4.debian.tar.xz 64588 SHA256:020e6bd6dcbccdb0ca5455116750120408225979ed186b84c58bb12cdb72d819
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/5.6.1-4/ (for browsing the source)
- https://sources.debian.net/src/mercurial/5.6.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/5.6.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mhash=0.9.9.9-9`

Binary Packages:

- `libmhash2:amd64=0.9.9.9-9`

Licenses: (parsed from: `/usr/share/doc/libmhash2/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris mhash=0.9.9.9-9
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9-9.dsc' mhash_0.9.9.9-9.dsc 1883 SHA256:cee703d37a3195a45cf93d0ab889bfdf64203882a4225e2bb2bb3929c99e2045
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9.orig.tar.gz' mhash_0.9.9.9.orig.tar.gz 577533 SHA256:73991e9e54bb392484a510943d4c5d395462181cc4abe53f863edec13c335403
'http://deb.debian.org/debian/pool/main/m/mhash/mhash_0.9.9.9-9.debian.tar.xz' mhash_0.9.9.9-9.debian.tar.xz 12824 SHA256:778226d68c64f1a57d3a49a28d0767553b4ad33dd8a09ebcfd0ac11531eabc06
```

Other potentially useful URLs:

- https://sources.debian.net/src/mhash/0.9.9.9-9/ (for browsing the source)
- https://sources.debian.net/src/mhash/0.9.9.9-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mhash/0.9.9.9-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpdecimal=2.5.1-1`

Binary Packages:

- `libmpdec3:amd64=2.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpdec3/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.5.1-1
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1-1.dsc' mpdecimal_2.5.1-1.dsc 1919 SHA256:5b4e5bc4d714b76af72bc4eaad2ac7feeb08ac5ee9fa5318f91edebe118ab6f9
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1.orig.tar.gz' mpdecimal_2.5.1.orig.tar.gz 2584021 SHA256:9f9cd4c041f99b5c49ffb7b59d9f12d95b683d88585608aa56a6307667b2b21f
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1-1.debian.tar.xz' mpdecimal_2.5.1-1.debian.tar.xz 6444 SHA256:e46140b8e665aee3058d0b2fb4fa44bde600251c8471de73711fa23ac573ee8a
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpdecimal/2.5.1-1/ (for browsing the source)
- https://sources.debian.net/src/mpdecimal/2.5.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpdecimal/2.5.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mythes=2:1.2.4-3`

Binary Packages:

- `libmythes-1.2-0:amd64=2:1.2.4-3+b1`

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

### `dpkg` source package: `ncurses=6.2+20201114-2`

Binary Packages:

- `libncurses6:amd64=6.2+20201114-2`
- `libncursesw6:amd64=6.2+20201114-2`
- `libtinfo6:amd64=6.2+20201114-2`
- `ncurses-base=6.2+20201114-2`
- `ncurses-bin=6.2+20201114-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2+20201114-2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2%2b20201114-2.dsc' ncurses_6.2+20201114-2.dsc 4106 SHA256:011ec8e3464be0d89d6611ab8fa0a84ac5514c0064e12dec9c52ec7b135408b1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2%2b20201114.orig.tar.gz' ncurses_6.2+20201114.orig.tar.gz 3539796 SHA256:aa3f8cfaff2a2b78f184274ec43d9da910c864e4b4d80fc47b5b48cba9154cd2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2%2b20201114.orig.tar.gz.asc' ncurses_6.2+20201114.orig.tar.gz.asc 265 SHA256:91615d9d5575f9e974e78c6aca55e1885f42d1b2600cebec407be4471bb7a27d
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2%2b20201114-2.debian.tar.xz' ncurses_6.2+20201114-2.debian.tar.xz 51812 SHA256:6ebba60b18cf2aceaa67098bfed1b1aa31c03f1a500f45c65ab098ec0a2401d2
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.2+20201114-2/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.2+20201114-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.2+20201114-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `neon27=0.31.2-1`

Binary Packages:

- `libneon27-gnutls:amd64=0.31.2-1`

Licenses: (parsed from: `/usr/share/doc/libneon27-gnutls/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris neon27=0.31.2-1
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.31.2-1.dsc' neon27_0.31.2-1.dsc 2168 SHA256:36647b0e1d179c3f0bfd084143db90e8020c20ad2d06be810f15dd777deb9ec6
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.31.2.orig.tar.gz' neon27_0.31.2.orig.tar.gz 486957 SHA256:c6513d20c0affca6f4b45e2414a86cce951709cf4448b6b64ccdf3579fda0ce5
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.31.2-1.debian.tar.xz' neon27_0.31.2-1.debian.tar.xz 11572 SHA256:374c9d210f4b6f1ab7c7d80b74ecd9aab88892e0d00330f415abcd5b73498339
```

Other potentially useful URLs:

- https://sources.debian.net/src/neon27/0.31.2-1/ (for browsing the source)
- https://sources.debian.net/src/neon27/0.31.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/neon27/0.31.2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `nspr=2:4.29-1`

Binary Packages:

- `libnspr4:amd64=2:4.29-1`

Licenses: (parsed from: `/usr/share/doc/libnspr4/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.29-1
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.29-1.dsc' nspr_4.29-1.dsc 1988 SHA256:04bb16a39313ea2b6bf364885174f9e3698a697e66f30eed0cab2db92b01ef44
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.29.orig.tar.gz' nspr_4.29.orig.tar.gz 1078192 SHA256:22286bdb8059d74632cc7c2865c139e63953ecfb33bf4362ab58827e86e92582
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.29-1.debian.tar.xz' nspr_4.29-1.debian.tar.xz 10728 SHA256:e0fca57a014d1996d768dfb532e88fdd429e59d5536bc08750df896c1895da5b
```

Other potentially useful URLs:

- https://sources.debian.net/src/nspr/2:4.29-1/ (for browsing the source)
- https://sources.debian.net/src/nspr/2:4.29-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nspr/2:4.29-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nss=2:3.61-1+deb11u2`

Binary Packages:

- `libnss3:amd64=2:3.61-1+deb11u2`

Licenses: (parsed from: `/usr/share/doc/libnss3/copyright`)

- `BSD-3`
- `MIT`
- `MPL-2.0`
- `Zlib`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nss=2:3.61-1+deb11u2
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.61-1%2bdeb11u2.dsc' nss_3.61-1+deb11u2.dsc 2333 SHA256:cc93275d15220876046f6aea3bee8fcf0d68741c91deab2b42e2aed61103a1d9
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.61.orig.tar.gz' nss_3.61.orig.tar.gz 82034245 SHA256:312e2d804b34ccf0fec70b57cf8cd6ac853f8ced60df53e30ebb0a7bcd0e1370
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.61-1%2bdeb11u2.debian.tar.xz' nss_3.61-1+deb11u2.debian.tar.xz 23672 SHA256:0e9ecc2edc8d82937b291709d94ef59d7b40615dc115d6d0dabaa9c4e65e5b48
```

Other potentially useful URLs:

- https://sources.debian.net/src/nss/2:3.61-1+deb11u2/ (for browsing the source)
- https://sources.debian.net/src/nss/2:3.61-1+deb11u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nss/2:3.61-1+deb11u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openjpeg2=2.4.0-3`

Binary Packages:

- `libopenjp2-7:amd64=2.4.0-3`

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
$ apt-get source -qq --print-uris openjpeg2=2.4.0-3
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.4.0-3.dsc' openjpeg2_2.4.0-3.dsc 2768 SHA256:c2de7ec896d9fccad5a9d58761593446a0271564babf218fd4ab200b6fe92a05
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.4.0.orig.tar.xz' openjpeg2_2.4.0.orig.tar.xz 1396964 SHA256:4b89da8abea5ea4e8dd5b214f1633a492554d784b5aebc22cb6495a1e5fe681c
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.4.0-3.debian.tar.xz' openjpeg2_2.4.0-3.debian.tar.xz 19712 SHA256:99b94d26c341babae8b5599ca7f8f0e1bb2021eb282ceff5d3c91086d1a3bcfc
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjpeg2/2.4.0-3/ (for browsing the source)
- https://sources.debian.net/src/openjpeg2/2.4.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjpeg2/2.4.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.57+dfsg-3`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.57+dfsg-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.57+dfsg-3
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.57%2bdfsg-3.dsc' openldap_2.4.57+dfsg-3.dsc 3061 SHA256:e51b6c564567aca61508b0bfc6dd53c39564f5b4284155ac51c436abb6ff7496
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.57%2bdfsg.orig.tar.gz' openldap_2.4.57+dfsg.orig.tar.gz 5054318 SHA256:009cc88733eaf41a21607e073a19bce53d7d6ed90a5c280e80880978c4e91db7
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.57%2bdfsg-3.debian.tar.xz' openldap_2.4.57+dfsg-3.debian.tar.xz 168536 SHA256:68e93e3c0a2167196f730d44fba31c5408930223c6900ca5a4e57e09bd5884c6
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.57+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.57+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.57+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:8.4p1-5`

Binary Packages:

- `openssh-client=1:8.4p1-5`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Beer-ware`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:8.4p1-5
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.4p1-5.dsc' openssh_8.4p1-5.dsc 3353 SHA256:77f230be1493a1037ab9b1555709f597563759115f40b189605da9f1817c0138
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.4p1.orig.tar.gz' openssh_8.4p1.orig.tar.gz 1742201 SHA256:5a01d22e407eb1c05ba8a8f7c654d388a13e9f226e4ed33bd38748dafa1d2b24
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.4p1.orig.tar.gz.asc' openssh_8.4p1.orig.tar.gz.asc 683 SHA256:ccd9dd484651ce4cc926228f6e1b46afaf0c5ab98a866217fa0ef1074370ea2b
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_8.4p1-5.debian.tar.xz' openssh_8.4p1-5.debian.tar.xz 179108 SHA256:9f38375592c9903fd64a1e69f42452ddad7e7c35c561ea7b8befbf45870b1a53
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:8.4p1-5/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:8.4p1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:8.4p1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.1n-0+deb11u1`

Binary Packages:

- `libssl1.1:amd64=1.1.1n-0+deb11u1`
- `openssl=1.1.1n-0+deb11u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1n-0+deb11u1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1n-0%2bdeb11u1.dsc' openssl_1.1.1n-0+deb11u1.dsc 2652 SHA256:2d56a8123aa339fd1213f4f743093aeabcc0ec4f60b9061302ab70b9c4c75300
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1n.orig.tar.gz' openssl_1.1.1n.orig.tar.gz 9850712 SHA256:40dceb51a4f6a5275bde0e6bf20ef4b91bfc32ed57c0552e2e8e15463372b17a
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1n.orig.tar.gz.asc' openssl_1.1.1n.orig.tar.gz.asc 488 SHA256:e0e89e9467102880ee6f2ee8c1413933eb1268969afb97b9bec61e2190a62fd0
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1n-0%2bdeb11u1.debian.tar.xz' openssl_1.1.1n-0+deb11u1.debian.tar.xz 84804 SHA256:027a42087b4c4183ed85124dd03847bcf91f397582cb42a89ea0fb0da13e41b0
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.1n-0+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.1n-0+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.1n-0+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `orc=1:0.4.32-1`

Binary Packages:

- `liborc-0.4-0:amd64=1:0.4.32-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris orc=1:0.4.32-1
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.32-1.dsc' orc_0.4.32-1.dsc 2323 SHA256:87cfe7e2b15c979fc3a0cc021211edbc04f94ca667974bc4feae6de957f4e7bd
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.32.orig.tar.xz' orc_0.4.32.orig.tar.xz 180340 SHA256:a66e3d8f2b7e65178d786a01ef61f2a0a0b4d0b8370de7ce134ba73da4af18f0
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.32-1.debian.tar.xz' orc_0.4.32-1.debian.tar.xz 5644 SHA256:98f2598023364af087d4d6b45ad89ed3caa80ba0589755ee7cc79b22fb7cb440
```

Other potentially useful URLs:

- https://sources.debian.net/src/orc/1:0.4.32-1/ (for browsing the source)
- https://sources.debian.net/src/orc/1:0.4.32-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/orc/1:0.4.32-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.22-1`

Binary Packages:

- `libp11-kit0:amd64=0.23.22-1`
- `p11-kit=0.23.22-1`
- `p11-kit-modules:amd64=0.23.22-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`, `/usr/share/doc/p11-kit/copyright`, `/usr/share/doc/p11-kit-modules/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.22-1
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.22-1.dsc' p11-kit_0.23.22-1.dsc 2417 SHA256:b5f7a7908a7da082fa74c2a35667f4f4dd1324eaf43ff4b4a0ffa7e2763774a6
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz' p11-kit_0.23.22.orig.tar.xz 830016 SHA256:8a8f40153dd5a3f8e7c03e641f8db400133fb2a6a9ab2aee1b6d0cb0495ec6b6
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz.asc' p11-kit_0.23.22.orig.tar.xz.asc 854 SHA256:52d36bd38ed84dcc394b97da18ff4b4e220f0b13c5e7922f5b908312678b0b02
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.22-1.debian.tar.xz' p11-kit_0.23.22-1.debian.tar.xz 22256 SHA256:05a157dbeb054dd14c19c0c4f72c50e57fb69c4cfa4b5d34bc7ecdb5d12e7265
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.23.22-1/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.23.22-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.23.22-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.4.0-9+deb11u1`

Binary Packages:

- `libpam-modules:amd64=1.4.0-9+deb11u1`
- `libpam-modules-bin=1.4.0-9+deb11u1`
- `libpam-runtime=1.4.0-9+deb11u1`
- `libpam0g:amd64=1.4.0-9+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.4.0-9+deb11u1
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-9%2bdeb11u1.dsc' pam_1.4.0-9+deb11u1.dsc 1941 SHA256:190b705cc9daeee1febb84e8ac6f31219065f08ff41c8d38fbbb424b545d5ca4
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0.orig.tar.xz' pam_1.4.0.orig.tar.xz 988908 SHA256:cd6d928c51e64139be3bdb38692c68183a509b83d4f2c221024ccd4bcddfd034
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-9%2bdeb11u1.debian.tar.xz' pam_1.4.0-9+deb11u1.debian.tar.xz 120148 SHA256:bcaaad9423c3ab32c5c4f9e363595a84fe3c535aa9568e42e560028a4e33dfcf
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.4.0-9+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/pam/1.4.0-9+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.4.0-9+deb11u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `perl=5.32.1-4+deb11u2`

Binary Packages:

- `libperl5.32:amd64=5.32.1-4+deb11u2`
- `perl=5.32.1-4+deb11u2`
- `perl-base=5.32.1-4+deb11u2`
- `perl-modules-5.32=5.32.1-4+deb11u2`

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
$ apt-get source -qq --print-uris perl=5.32.1-4+deb11u2
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1-4%2bdeb11u2.dsc' perl_5.32.1-4+deb11u2.dsc 2918 SHA256:3c0c1961d7a5fe835cf7d1a9a97905ff7857db2cd1d113c9fc5250de3aaa4e6b
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1.orig-regen-configure.tar.gz' perl_5.32.1.orig-regen-configure.tar.gz 871331 SHA256:1d179b41283f12ad83f9758430f6ddc49bdf20db5c396aeae7e51ebb4e4afd29
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1.orig.tar.xz' perl_5.32.1.orig.tar.xz 12610988 SHA256:57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1-4%2bdeb11u2.debian.tar.xz' perl_5.32.1-4+deb11u2.debian.tar.xz 165768 SHA256:36b96f84a81c8db85a99e701062457a99efdbcc98b1f1a8912d3919f4b8e0f5a
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.32.1-4+deb11u2/ (for browsing the source)
- https://sources.debian.net/src/perl/5.32.1-4+deb11u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.32.1-4+deb11u2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `poppler=20.09.0-3.1`

Binary Packages:

- `libpoppler102:amd64=20.09.0-3.1`

Licenses: (parsed from: `/usr/share/doc/libpoppler102/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris poppler=20.09.0-3.1
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_20.09.0-3.1.dsc' poppler_20.09.0-3.1.dsc 3248 SHA256:8ddc4e09e6b03065e6705544923cf16a5e026730cc7fc5279fa463d99f1e0384
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_20.09.0.orig.tar.xz' poppler_20.09.0.orig.tar.xz 1642932 SHA256:4ed6eb5ddc4c37f2435c9d78ff9c7c4036455aea3507d1ce8400070aab745363
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_20.09.0-3.1.debian.tar.xz' poppler_20.09.0-3.1.debian.tar.xz 34000 SHA256:adfb3883faf8846cd62c6861964324191fe12dcd4af54a8d872970d020d0f7d0
```

Other potentially useful URLs:

- https://sources.debian.net/src/poppler/20.09.0-3.1/ (for browsing the source)
- https://sources.debian.net/src/poppler/20.09.0-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/poppler/20.09.0-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.17-5`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-5`
- `procps=2:3.3.17-5`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-5
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-5.dsc' procps_3.3.17-5.dsc 2136 SHA256:3b1d9a3d3bc9ec24360ed20721d4235fcd4b4dbb9a86c1eba6c42899a50ecff8
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA256:4518b3e7aafd34ec07d0063d250fd474999b20b200218c3ae56f5d2113f141b4
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-5.debian.tar.xz' procps_3.3.17-5.debian.tar.xz 28608 SHA256:e6b5f9ef22eca9f03f79dc79b4c389249368216df8702a8cc380e10f29eda8c9
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.17-5/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.17-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.17-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.9.2-3`

Binary Packages:

- `libpython3-stdlib:amd64=3.9.2-3`
- `python3=3.9.2-3`
- `python3-minimal=3.9.2-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.9.2-3
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.9.2-3.dsc' python3-defaults_3.9.2-3.dsc 2879 SHA256:625d69b163c4ba751d717ccd4e4202f6c3132a4734f0d083ae11dea465cc7760
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.9.2-3.tar.gz' python3-defaults_3.9.2-3.tar.gz 140929 SHA256:64a82311e46c734a897e408cad11d17e5631ec3ec889ae90948111150e8f18ce
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3-defaults/3.9.2-3/ (for browsing the source)
- https://sources.debian.net/src/python3-defaults/3.9.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3-defaults/3.9.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3.9=3.9.2-1`

Binary Packages:

- `libpython3.9:amd64=3.9.2-1`
- `libpython3.9-minimal:amd64=3.9.2-1`
- `libpython3.9-stdlib:amd64=3.9.2-1`
- `python3.9=3.9.2-1`
- `python3.9-minimal=3.9.2-1`

Licenses: (parsed from: `/usr/share/doc/libpython3.9/copyright`, `/usr/share/doc/libpython3.9-minimal/copyright`, `/usr/share/doc/libpython3.9-stdlib/copyright`, `/usr/share/doc/python3.9/copyright`, `/usr/share/doc/python3.9-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.9=3.9.2-1
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.2-1.dsc' python3.9_3.9.2-1.dsc 3493 SHA256:63bc63b864067e7f993be8bc9bf2a08363fde05895bea86961fc5d781e42b68b
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.2.orig.tar.xz' python3.9_3.9.2.orig.tar.xz 18889164 SHA256:3c2034c54f811448f516668dce09d24008a0716c3a794dd8639b5388cbde247d
'http://deb.debian.org/debian/pool/main/p/python3.9/python3.9_3.9.2-1.debian.tar.xz' python3.9_3.9.2-1.debian.tar.xz 211484 SHA256:b8b9e1710ca5dc5b0f0d9734494024ea11f560e36c34eb9191ccb0605798a490
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.9/3.9.2-1/ (for browsing the source)
- https://sources.debian.net/src/python3.9/3.9.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.9/3.9.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `qr-code-generator=1.6.0-1`

Binary Packages:

- `libqrcodegencpp1:amd64=1.6.0-1`

Licenses: (parsed from: `/usr/share/doc/libqrcodegencpp1/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris qr-code-generator=1.6.0-1
'http://deb.debian.org/debian/pool/main/q/qr-code-generator/qr-code-generator_1.6.0-1.dsc' qr-code-generator_1.6.0-1.dsc 2296 SHA256:ac72563bc976f392334b0b76e10943d271724322b69903a12aacb8dec556ec31
'http://deb.debian.org/debian/pool/main/q/qr-code-generator/qr-code-generator_1.6.0.orig.tar.gz' qr-code-generator_1.6.0.orig.tar.gz 135432 SHA256:8acee5a77325e075b910747ad4b1fdb1491b7e22d0b8f1b5a6ea15ea08ba33a8
'http://deb.debian.org/debian/pool/main/q/qr-code-generator/qr-code-generator_1.6.0-1.debian.tar.xz' qr-code-generator_1.6.0-1.debian.tar.xz 7148 SHA256:52d5645b02dd4a2805476c8fddc730110487be9736aef7b37b56d7433d357e47
```

Other potentially useful URLs:

- https://sources.debian.net/src/qr-code-generator/1.6.0-1/ (for browsing the source)
- https://sources.debian.net/src/qr-code-generator/1.6.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/qr-code-generator/1.6.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `raptor2=2.0.14-1.2`

Binary Packages:

- `libraptor2-0:amd64=2.0.14-1.2`

Licenses: (parsed from: `/usr/share/doc/libraptor2-0/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris raptor2=2.0.14-1.2
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14-1.2.dsc' raptor2_2.0.14-1.2.dsc 2276 SHA256:9f9c7152c72c4721685fd6e066278e6c7adbacf7de4d91a405d8fee2fa96bd30
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14.orig.tar.gz' raptor2_2.0.14.orig.tar.gz 1877454 SHA256:cb447b7c684cbe60f1266d622691fd20fdcf7b91f4a470c6de5fc8e8961df1b2
'http://deb.debian.org/debian/pool/main/r/raptor2/raptor2_2.0.14-1.2.debian.tar.xz' raptor2_2.0.14-1.2.debian.tar.xz 8792 SHA256:887e57183d1938d5c5c301e31da97938698432c51731fbee01b3ffd55ad7ea89
```

Other potentially useful URLs:

- https://sources.debian.net/src/raptor2/2.0.14-1.2/ (for browsing the source)
- https://sources.debian.net/src/raptor2/2.0.14-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/raptor2/2.0.14-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rasqal=0.9.33-0.1`

Binary Packages:

- `librasqal3:amd64=0.9.33-0.1`

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
$ apt-get source -qq --print-uris rasqal=0.9.33-0.1
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.33-0.1.dsc' rasqal_0.9.33-0.1.dsc 2071 SHA256:8eec59c6f2c1d9492e625b8e1b0f76a77eb4bbce04395285dffb062eb778087a
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.33.orig.tar.gz' rasqal_0.9.33.orig.tar.gz 1595647 SHA256:6924c9ac6570bd241a9669f83b467c728a322470bf34f4b2da4f69492ccfd97c
'http://deb.debian.org/debian/pool/main/r/rasqal/rasqal_0.9.33-0.1.debian.tar.xz' rasqal_0.9.33-0.1.debian.tar.xz 5980 SHA256:28916ca977362ff9edf41432faa33c5db25595719d34ede560c15318b970c9b1
```

Other potentially useful URLs:

- https://sources.debian.net/src/rasqal/0.9.33-0.1/ (for browsing the source)
- https://sources.debian.net/src/rasqal/0.9.33-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rasqal/0.9.33-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.1-1`

Binary Packages:

- `libreadline8:amd64=8.1-1`
- `readline-common=8.1-1`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1-1
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1-1.dsc' readline_8.1-1.dsc 2418 SHA256:53356fdf2ee122ab75c7b535d292385311f7dea425ccc42143d2b9a2accfc657
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1.orig.tar.gz' readline_8.1.orig.tar.gz 2993288 SHA256:f8ceb4ee131e3232226a17f51b164afc46cd0b9e6cef344be87c65962cb82b02
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.1-1.debian.tar.xz' readline_8.1-1.debian.tar.xz 29220 SHA256:852267a95aeec23b267c838469fee346e83a29e7a08071178dc87682591cffbf
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/8.1-1/ (for browsing the source)
- https://sources.debian.net/src/readline/8.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/8.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `redland=1.0.17-1.1`

Binary Packages:

- `librdf0:amd64=1.0.17-1.1+b1`

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

### `dpkg` source package: `sensible-utils=0.0.14`

Binary Packages:

- `sensible-utils=0.0.14`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.14
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.14.dsc' sensible-utils_0.0.14.dsc 1702 SHA256:002f637ca92db8bab28048cbab10d6509508508806e2005f4dc6ba3ca505a6d8
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.14.tar.xz' sensible-utils_0.0.14.tar.xz 64448 SHA256:a6ee528bf4122d77acacdb97f20cd0434a12ad3ecd119186a5fcee066844c644
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.14/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.14/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `sqlite3=3.34.1-3`

Binary Packages:

- `libsqlite3-0:amd64=3.34.1-3`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.34.1-3
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.34.1-3.dsc' sqlite3_3.34.1-3.dsc 2410 SHA256:bee4705c6a1332c1ecb299e23b54cfe04b63ea5a163be1d211fa676595686cbf
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.34.1.orig-www.tar.xz' sqlite3_3.34.1.orig-www.tar.xz 5581512 SHA256:c63647f3fb6c4b0620d6587e2a744021401df92c307b55e236a7eb28c5000fa7
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.34.1.orig.tar.xz' sqlite3_3.34.1.orig.tar.xz 7343284 SHA256:082f583440c662cb484ae1c124ffe285b587bbb7837e095e693026e6df50334d
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.34.1-3.debian.tar.xz' sqlite3_3.34.1-3.debian.tar.xz 22828 SHA256:aefed33ed3e388d46cd35ab865b5fffe028b7511c0211f8521eacb8562fec0aa
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.34.1-3/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.34.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.34.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `subversion=1.14.1-3`

Binary Packages:

- `libsvn1:amd64=1.14.1-3`
- `subversion=1.14.1-3`

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

### `dpkg` source package: `suitesparse=1:5.8.1+dfsg-2`

Binary Packages:

- `libcolamd2:amd64=1:5.8.1+dfsg-2`
- `libsuitesparseconfig5:amd64=1:5.8.1+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libcolamd2/copyright`, `/usr/share/doc/libsuitesparseconfig5/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-2-clause-lagraph`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `permissive`
- `permissive-2`

Source:

```console
$ apt-get source -qq --print-uris suitesparse=1:5.8.1+dfsg-2
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_5.8.1%2bdfsg-2.dsc' suitesparse_5.8.1+dfsg-2.dsc 3166 SHA256:403c81218e3fad7249f5d9bf9b406a3fd9ce5cab0d5c6c76a7daf58be5a44290
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_5.8.1%2bdfsg.orig.tar.xz' suitesparse_5.8.1+dfsg.orig.tar.xz 37624256 SHA256:cf45a3d4c935cc2100bd4ba61a6f682a049027dce5d91846541a4933e0267752
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_5.8.1%2bdfsg-2.debian.tar.xz' suitesparse_5.8.1+dfsg-2.debian.tar.xz 53448 SHA256:5e82391a54ea8487e471ea28c81841545c6545b34519cae7b1bf145eec3d559b
```

Other potentially useful URLs:

- https://sources.debian.net/src/suitesparse/1:5.8.1+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/suitesparse/1:5.8.1+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/suitesparse/1:5.8.1+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=247.3-7`

Binary Packages:

- `libsystemd0:amd64=247.3-7`
- `libudev1:amd64=247.3-7`

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
$ apt-get source -qq --print-uris systemd=247.3-7
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.3-7.dsc' systemd_247.3-7.dsc 5167 SHA256:c363c7538890cc8bfec033c44ae798c7ead370a143a8dad76ef0714c4784fce2
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.3.orig.tar.gz' systemd_247.3.orig.tar.gz 9895385 SHA256:2869986e219a8dfc96cc0dffac66e0c13bb70a89e16b85a3948876c146cfa3e0
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.3-7.debian.tar.xz' systemd_247.3-7.debian.tar.xz 183052 SHA256:d80595383166aa08ed28441898880fbc124bf2468526d35fc7c85c2c09f12ca5
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/247.3-7/ (for browsing the source)
- https://sources.debian.net/src/systemd/247.3-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/247.3-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=2.96-7+deb11u1`

Binary Packages:

- `sysvinit-utils=2.96-7+deb11u1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-7+deb11u1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-7%2bdeb11u1.dsc' sysvinit_2.96-7+deb11u1.dsc 2374 SHA256:1ef8a8b224aabecbd27ebef68b389bc3149970ef348877cec3ac7351a04c13a7
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.gz' sysvinit_2.96.orig.tar.gz 147834 SHA256:1275620f767c85bb2d7e5b9542579ae097f3eb542065ff30a70efc95b6e84c64
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-7%2bdeb11u1.debian.tar.xz' sysvinit_2.96-7+deb11u1.debian.tar.xz 129936 SHA256:5ce9a0b9735a66c536c77c65e17d4190338e0c0416ba235c26c9cf12d3cfbeb3
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.96-7+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.96-7+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.96-7+deb11u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `tiff=4.2.0-1+deb11u1`

Binary Packages:

- `libtiff5:amd64=4.2.0-1+deb11u1`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.2.0-1+deb11u1
'http://security.debian.org/debian-security/pool/updates/main/t/tiff/tiff_4.2.0-1%2bdeb11u1.dsc' tiff_4.2.0-1+deb11u1.dsc 2461 SHA256:09c0d66b0f710bab934727529fcc418217588ccd62b7ebcbe1a1057bea6507e4
'http://security.debian.org/debian-security/pool/updates/main/t/tiff/tiff_4.2.0.orig.tar.gz' tiff_4.2.0.orig.tar.gz 2809373 SHA256:eb0484e568ead8fa23b513e9b0041df7e327f4ee2d22db5a533929dfc19633cb
'http://security.debian.org/debian-security/pool/updates/main/t/tiff/tiff_4.2.0.orig.tar.gz.asc' tiff_4.2.0.orig.tar.gz.asc 228 SHA256:119bb62934603ff4d3cd81c739d11904b28812a860773b9b2268cc96a339b14f
'http://security.debian.org/debian-security/pool/updates/main/t/tiff/tiff_4.2.0-1%2bdeb11u1.debian.tar.xz' tiff_4.2.0-1+deb11u1.debian.tar.xz 25188 SHA256:a0b8d4a231d97e0dbefde74fe5788d19429c4bcbfd32102a9d09fd6dc39273a0
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.2.0-1+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.2.0-1+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.2.0-1+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2021a-1+deb11u3`

Binary Packages:

- `tzdata=2021a-1+deb11u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2021a-1+deb11u3
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a-1%2bdeb11u3.dsc' tzdata_2021a-1+deb11u3.dsc 2269 SHA256:446f7e859e69214cb3b9a642eedcf61851e60039cc9a6d0ada01eaee49bf4c1d
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a.orig.tar.gz' tzdata_2021a.orig.tar.gz 411892 SHA256:39e7d2ba08c68cbaefc8de3227aab0dec2521be8042cf56855f7dc3a9fb14e08
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a.orig.tar.gz.asc' tzdata_2021a.orig.tar.gz.asc 833 SHA256:9dc5f54674166f4ffbc2d4485e656227430ab5f39c9006e6ed9986281117f058
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a-1%2bdeb11u3.debian.tar.xz' tzdata_2021a-1+deb11u3.debian.tar.xz 109824 SHA256:ec7e4c4b3d2063b82b7cd25975f4fa94d68109d325fdf921d256b033f9be3d82
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2021a-1+deb11u3/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2021a-1+deb11u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2021a-1+deb11u3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `utf8proc=2.5.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.5.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.5.0-1
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.5.0-1.dsc' utf8proc_2.5.0-1.dsc 2154 SHA256:2137104a3712875650629305fe7d7ef37d4d99328846c18b087b289c0ddbf27c
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.5.0.orig.tar.gz' utf8proc_2.5.0.orig.tar.gz 155485 SHA256:d4e8dfc898cfd062493cb7f42d95d70ccdd3a4cd4d90bec0c71b47cca688f1be
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.5.0-1.debian.tar.xz' utf8proc_2.5.0-1.debian.tar.xz 5240 SHA256:333496cf4e178b5ccf4972fa52523d07a21a0cabf0cb123133c6c71f98e92eff
```

Other potentially useful URLs:

- https://sources.debian.net/src/utf8proc/2.5.0-1/ (for browsing the source)
- https://sources.debian.net/src/utf8proc/2.5.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/utf8proc/2.5.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.36.1-8+deb11u1`

Binary Packages:

- `bsdutils=1:2.36.1-8+deb11u1`
- `libblkid1:amd64=2.36.1-8+deb11u1`
- `libmount1:amd64=2.36.1-8+deb11u1`
- `libsmartcols1:amd64=2.36.1-8+deb11u1`
- `libuuid1:amd64=2.36.1-8+deb11u1`
- `mount=2.36.1-8+deb11u1`
- `util-linux=2.36.1-8+deb11u1`

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
$ apt-get source -qq --print-uris util-linux=2.36.1-8+deb11u1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.36.1-8%2bdeb11u1.dsc' util-linux_2.36.1-8+deb11u1.dsc 4461 SHA256:1f42a8e46c383b6fbfb57ea89dfe5adb5b7e6960bc5e8cdb9589109773be6cac
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.36.1.orig.tar.xz' util-linux_2.36.1.orig.tar.xz 5231880 SHA256:09fac242172cd8ec27f0739d8d192402c69417617091d8c6e974841568f37eed
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.36.1-8%2bdeb11u1.debian.tar.xz' util-linux_2.36.1-8+deb11u1.debian.tar.xz 101448 SHA256:edda1d46e25a40e730c672aac2cd0e44f9eeb0fb64b27be957d6924ed5288a0a
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.36.1-8+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.36.1-8+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.36.1-8+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.21-1+deb11u1`

Binary Packages:

- `wget=1.21-1+deb11u1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21-1+deb11u1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21-1%2bdeb11u1.dsc' wget_1.21-1+deb11u1.dsc 2208 SHA256:b9b3c2b206a602f4954688dc85c2131c35ad12621405e89560e060c122f029d1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.orig.tar.gz' wget_1.21.orig.tar.gz 4866788 SHA256:b3bc1a9bd0c19836c9709c318d41c19c11215a07514f49f89b40b9d50ab49325
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.orig.tar.gz.asc' wget_1.21.orig.tar.gz.asc 854 SHA256:da3a99b8a7bbaf70cc339593a9e0c2942dd673152bc7bfcf8f965ae1c06d50df
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21-1%2bdeb11u1.debian.tar.xz' wget_1.21-1+deb11u1.debian.tar.xz 60944 SHA256:cfb8edda9e0667e2fba60939674c8a4e5a14fca04c91e27ed5699b345144804e
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.21-1+deb11u1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.21-1+deb11u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.21-1+deb11u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xmlsec1=1.2.31-1`

Binary Packages:

- `libxmlsec1:amd64=1.2.31-1`
- `libxmlsec1-nss:amd64=1.2.31-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xmlsec1=1.2.31-1
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.31-1.dsc' xmlsec1_1.2.31-1.dsc 2616 SHA256:2b4a3def4c3b3ced1d494f22d98322ade3496ec252afc5fdcc362d20aa22b459
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.31.orig.tar.gz' xmlsec1_1.2.31.orig.tar.gz 1989144 SHA256:9b10bc52cc31e4f76162e3975e50db26b71ab49c571d810b311ca626be5a0b26
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.31-1.debian.tar.xz' xmlsec1_1.2.31-1.debian.tar.xz 8552 SHA256:0b91fdc50b02a65cd257cec6de25bc5492d8cac84bb7556500aaed1ceeb8b76f
```

Other potentially useful URLs:

- https://sources.debian.net/src/xmlsec1/1.2.31-1/ (for browsing the source)
- https://sources.debian.net/src/xmlsec1/1.2.31-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xmlsec1/1.2.31-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorg=1:7.7+22`

Binary Packages:

- `x11-common=1:7.7+22`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+22
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7%2b22.dsc' xorg_7.7+22.dsc 1975 SHA256:5b273e9b4ece8f4525e73721cc1f14ea0772007035c24b5e35269bcdca45b69a
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7%2b22.tar.gz' xorg_7.7+22.tar.gz 287402 SHA256:4e39d07914480826f02f8ba293dc07e5595a2789c53ee47d92cc5ee992ef2ed5
```

Other potentially useful URLs:

- https://sources.debian.net/src/xorg/1:7.7+22/ (for browsing the source)
- https://sources.debian.net/src/xorg/1:7.7+22/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xorg/1:7.7+22/ (for access to the source package after it no longer exists in the archive)

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
- `xz-utils=5.2.5-2`

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

### `dpkg` source package: `yajl=2.1.0-3`

Binary Packages:

- `libyajl2:amd64=2.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libyajl2/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris yajl=2.1.0-3
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0-3.dsc' yajl_2.1.0-3.dsc 1934 SHA256:bb35b92eda156bf114902e231859f241b67207d7b978878f6a595a995e5cf29d
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0.orig.tar.gz' yajl_2.1.0.orig.tar.gz 83997 SHA256:3fb73364a5a30efe615046d07e6db9d09fd2b41c763c5f7d3bfb121cd5c5ac5a
'http://deb.debian.org/debian/pool/main/y/yajl/yajl_2.1.0-3.debian.tar.xz' yajl_2.1.0-3.debian.tar.xz 5616 SHA256:b8056025a0d41af27127bc0993ffbff2ff3c09285494f4498f8ad769443a7463
```

Other potentially useful URLs:

- https://sources.debian.net/src/yajl/2.1.0-3/ (for browsing the source)
- https://sources.debian.net/src/yajl/2.1.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/yajl/2.1.0-3/ (for access to the source package after it no longer exists in the archive)

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
