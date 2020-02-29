# `nuxeo:10.10`

## Docker Metadata

- Image ID: `sha256:22aa3207a04be8fa07d647c8e04f404a821e575565c7ebc6200e8d882ba8fd2f`
- Created: `2020-02-27T07:14:32.038989316Z`
- Virtual Size: ~ 1.85 Gb  
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

### `dpkg` source package: `acl=2.2.53-4`

Binary Packages:

- `libacl1:amd64=2.2.53-4`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-4
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-4.dsc' acl_2.2.53-4.dsc 2330 SHA256:532eb4029659db74e6625adc2bd277144f33c92cb0603272d61693b069896a85
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-4.debian.tar.xz' acl_2.2.53-4.debian.tar.xz 18572 SHA256:3e6571adea4886a9549bdc2323d5c55ee8f7dafb6a204513111d5943d2776dd8
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.53-4/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.53-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.53-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `adwaita-icon-theme=3.30.1-1`

Binary Packages:

- `adwaita-icon-theme=3.30.1-1`

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
$ apt-get source -qq --print-uris adwaita-icon-theme=3.30.1-1
'http://deb.debian.org/debian/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.30.1-1.dsc' adwaita-icon-theme_3.30.1-1.dsc 2159 SHA256:f046be9ff1659235fc19b85b318a71bb7a94b6e83497be957e36aa487e4bf220
'http://deb.debian.org/debian/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.30.1.orig.tar.xz' adwaita-icon-theme_3.30.1.orig.tar.xz 19931180 SHA256:6d752a2b1bc668483956d4485c39cad1642d9358e133ff689526e43674a4e1ce
'http://deb.debian.org/debian/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.30.1-1.debian.tar.xz' adwaita-icon-theme_3.30.1-1.debian.tar.xz 27868 SHA256:cf6bb2d4982e2476845411c6537971677473f1edd258f6e4148ae2c9a2fde4ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/adwaita-icon-theme/3.30.1-1/ (for browsing the source)
- https://sources.debian.net/src/adwaita-icon-theme/3.30.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adwaita-icon-theme/3.30.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `alsa-lib=1.1.8-1`

Binary Packages:

- `libasound2:amd64=1.1.8-1`
- `libasound2-data=1.1.8-1`

Licenses: (parsed from: `/usr/share/doc/libasound2/copyright`, `/usr/share/doc/libasound2-data/copyright`)

- `LGPL-2.1`
- `LPGL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris alsa-lib=1.1.8-1
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.1.8-1.dsc' alsa-lib_1.1.8-1.dsc 2485 SHA256:a48dc276a235281d522c3bd8dfc1c264fe3764803b1e079fb76910296cced407
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.1.8.orig.tar.bz2' alsa-lib_1.1.8.orig.tar.bz2 1002562 SHA256:3cdc3a93a6427a26d8efab4ada2152e64dd89140d981f6ffa003e85be707aedf
'http://deb.debian.org/debian/pool/main/a/alsa-lib/alsa-lib_1.1.8-1.debian.tar.xz' alsa-lib_1.1.8-1.debian.tar.xz 34600 SHA256:5d6c027d37b98c5081b98f9dfc0564ba085c51e17474c0227a491e3fcf7331f9
```

Other potentially useful URLs:

- https://sources.debian.net/src/alsa-lib/1.1.8-1/ (for browsing the source)
- https://sources.debian.net/src/alsa-lib/1.1.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/alsa-lib/1.1.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `aom=1.0.0-3`

Binary Packages:

- `libaom0:amd64=1.0.0-3`

Licenses: (parsed from: `/usr/share/doc/libaom0/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `ISC`
- `public-domain-md5`

Source:

```console
$ apt-get source -qq --print-uris aom=1.0.0-3
'http://deb.debian.org/debian/pool/main/a/aom/aom_1.0.0-3.dsc' aom_1.0.0-3.dsc 2290 SHA256:f3cb6863d8287d72e62b8c08fa9aa4df2a53900f0f899ce9dfe833518f53afb8
'http://deb.debian.org/debian/pool/main/a/aom/aom_1.0.0.orig.tar.xz' aom_1.0.0.orig.tar.xz 1896516 SHA256:4319eb3ef38abfabfdb3037cc3a7a47804ed5f58c96576876bbe0ac2a25bbcc6
'http://deb.debian.org/debian/pool/main/a/aom/aom_1.0.0-3.debian.tar.xz' aom_1.0.0-3.debian.tar.xz 21612 SHA256:a9650519798d2fab2c20cbc8fe8f73b7e7f7f03112128771d178a3019c94d15d
```

Other potentially useful URLs:

- https://sources.debian.net/src/aom/1.0.0-3/ (for browsing the source)
- https://sources.debian.net/src/aom/1.0.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/aom/1.0.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apparmor=2.13.2-10`

Binary Packages:

- `libapparmor1:amd64=2.13.2-10`

Licenses: (parsed from: `/usr/share/doc/libapparmor1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris apparmor=2.13.2-10
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.13.2-10.dsc' apparmor_2.13.2-10.dsc 3370 SHA256:743547b3a693f0873f02860a5df8ec909544f9f7f54e97899ee0cb5bec518c60
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.13.2.orig.tar.gz' apparmor_2.13.2.orig.tar.gz 7369240 SHA256:844def9926dfda5c7858428d06e44afc80573f9706458b6e7282edbb40b11a30
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.13.2.orig.tar.gz.asc' apparmor_2.13.2.orig.tar.gz.asc 870 SHA256:5b0fb153a28a29c0d300b390ab62b9a19a3d23634c8c3d08292181d68d8b0e8a
'http://deb.debian.org/debian/pool/main/a/apparmor/apparmor_2.13.2-10.debian.tar.xz' apparmor_2.13.2-10.debian.tar.xz 106724 SHA256:2777537b493f5e3aea89aa41ba9e7664615d3e36be2d87d5ddc63bd9c1f4bc43
```

Other potentially useful URLs:

- https://sources.debian.net/src/apparmor/2.13.2-10/ (for browsing the source)
- https://sources.debian.net/src/apparmor/2.13.2-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apparmor/2.13.2-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr-util=1.6.1-4`

Binary Packages:

- `libaprutil1:amd64=1.6.1-4`

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

### `dpkg` source package: `apt=1.8.2`

Binary Packages:

- `apt=1.8.2`
- `libapt-pkg5.0:amd64=1.8.2`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.8.2
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.8.2.dsc' apt_1.8.2.dsc 2766 SHA256:891cc952f028b79e2eace3db6c19d55dee247ac19d934bbe43c3921104b01c3b
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.8.2.tar.xz' apt_1.8.2.tar.xz 2188344 SHA256:7f9a91c26624bc85733683ee239b0c0d971a593d670855cf7bcf693b08a37734
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/1.8.2/ (for browsing the source)
- https://sources.debian.net/src/apt/1.8.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/1.8.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `argon2=0~20171227-0.2`

Binary Packages:

- `libargon2-1:amd64=0~20171227-0.2`

Licenses: (parsed from: `/usr/share/doc/libargon2-1/copyright`)

- `Apache-2.0`
- `CC0`

Source:

```console
$ apt-get source -qq --print-uris argon2=0~20171227-0.2
'http://deb.debian.org/debian/pool/main/a/argon2/argon2_0~20171227-0.2.dsc' argon2_0~20171227-0.2.dsc 2108 SHA256:357d1e93318d7dd3bee401ee9cd92bd0f3ecaab3990013580a12306efda4ebf7
'http://deb.debian.org/debian/pool/main/a/argon2/argon2_0~20171227.orig.tar.gz' argon2_0~20171227.orig.tar.gz 1503745 SHA256:eaea0172c1f4ee4550d1b6c9ce01aab8d1ab66b4207776aa67991eb5872fdcd8
'http://deb.debian.org/debian/pool/main/a/argon2/argon2_0~20171227-0.2.debian.tar.xz' argon2_0~20171227-0.2.debian.tar.xz 6932 SHA256:49e630c0027ebbe0b53e3e692ce99da750e9bdfeddcebf303e595b4af5a2142f
```

Other potentially useful URLs:

- https://sources.debian.net/src/argon2/0~20171227-0.2/ (for browsing the source)
- https://sources.debian.net/src/argon2/0~20171227-0.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/argon2/0~20171227-0.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `at-spi2-atk=2.30.0-5`

Binary Packages:

- `libatk-bridge2.0-0:amd64=2.30.0-5`

Licenses: (parsed from: `/usr/share/doc/libatk-bridge2.0-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris at-spi2-atk=2.30.0-5
'http://deb.debian.org/debian/pool/main/a/at-spi2-atk/at-spi2-atk_2.30.0-5.dsc' at-spi2-atk_2.30.0-5.dsc 2541 SHA256:0550b9889e02bdad2cb8a688535931c2882e42428cedc1d0ebcaa3bde8033fcd
'http://deb.debian.org/debian/pool/main/a/at-spi2-atk/at-spi2-atk_2.30.0.orig.tar.xz' at-spi2-atk_2.30.0.orig.tar.xz 94824 SHA256:e2e1571004ea7b105c969473ce455a95be4038fb2541471714aeb33a26da8a9a
'http://deb.debian.org/debian/pool/main/a/at-spi2-atk/at-spi2-atk_2.30.0-5.debian.tar.xz' at-spi2-atk_2.30.0-5.debian.tar.xz 9756 SHA256:9e1a14bb5bbcbc07560338bfeab6f62cc8bd0a3682ad94ea27733751e1b7de8e
```

Other potentially useful URLs:

- https://sources.debian.net/src/at-spi2-atk/2.30.0-5/ (for browsing the source)
- https://sources.debian.net/src/at-spi2-atk/2.30.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/at-spi2-atk/2.30.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `at-spi2-core=2.30.0-7`

Binary Packages:

- `libatspi2.0-0:amd64=2.30.0-7`

Licenses: (parsed from: `/usr/share/doc/libatspi2.0-0/copyright`)

- `AFL-2.1`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris at-spi2-core=2.30.0-7
'http://deb.debian.org/debian/pool/main/a/at-spi2-core/at-spi2-core_2.30.0-7.dsc' at-spi2-core_2.30.0-7.dsc 2634 SHA256:c0078bc0bd5b6044bde39300a4b93282055ad19f951dc735f94ce7febb1bccef
'http://deb.debian.org/debian/pool/main/a/at-spi2-core/at-spi2-core_2.30.0.orig.tar.xz' at-spi2-core_2.30.0.orig.tar.xz 188016 SHA256:0175f5393d19da51f4c11462cba4ba6ef3fa042abf1611a70bdfed586b7bfb2b
'http://deb.debian.org/debian/pool/main/a/at-spi2-core/at-spi2-core_2.30.0-7.debian.tar.xz' at-spi2-core_2.30.0-7.debian.tar.xz 10156 SHA256:777a459c3b71d62b2f046bb449ed69ad8822aafb1d859e479bad1e5c25acf4ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/at-spi2-core/2.30.0-7/ (for browsing the source)
- https://sources.debian.net/src/at-spi2-core/2.30.0-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/at-spi2-core/2.30.0-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `atk1.0=2.30.0-2`

Binary Packages:

- `libatk1.0-0:amd64=2.30.0-2`
- `libatk1.0-data=2.30.0-2`

Licenses: (parsed from: `/usr/share/doc/libatk1.0-0/copyright`, `/usr/share/doc/libatk1.0-data/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris atk1.0=2.30.0-2
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.30.0-2.dsc' atk1.0_2.30.0-2.dsc 2689 SHA256:1fc829db40dd6eacba3c6a0b403f23fd26bf2cdd37f1ef88a70667456902a65e
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.30.0.orig.tar.xz' atk1.0_2.30.0.orig.tar.xz 290264 SHA256:dd4d90d4217f2a0c1fee708a555596c2c19d26fef0952e1ead1938ab632c027b
'http://deb.debian.org/debian/pool/main/a/atk1.0/atk1.0_2.30.0-2.debian.tar.xz' atk1.0_2.30.0-2.debian.tar.xz 12008 SHA256:e944e76557b4dd0affe27d92fc0c6c6a37b1fd1a222d2b22326ed5a3af9b1bb1
```

Other potentially useful URLs:

- https://sources.debian.net/src/atk1.0/2.30.0-2/ (for browsing the source)
- https://sources.debian.net/src/atk1.0/2.30.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/atk1.0/2.30.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `attr=1:2.4.48-4`

Binary Packages:

- `libattr1:amd64=1:2.4.48-4`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.48-4
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-4.dsc' attr_2.4.48-4.dsc 2427 SHA256:e53c076f39f1be4186704c94bd32276fa4661a587c360d8da25a5c3abe40cb29
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-4.debian.tar.xz' attr_2.4.48-4.debian.tar.xz 22388 SHA256:a491d226fb3b47aa65997406009893a4cc0628e2ffffe0d411179652dfeb6935
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.4.48-4/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.4.48-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.4.48-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:2.8.4-3`

Binary Packages:

- `libaudit-common=1:2.8.4-3`
- `libaudit1:amd64=1:2.8.4-3`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.4-3
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.4-3.dsc' audit_2.8.4-3.dsc 2483 SHA256:101fd82f4c7af2f8753060b494ac46204b0eee1ffe5d1e113a493b99571af186
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.4.orig.tar.gz' audit_2.8.4.orig.tar.gz 1123889 SHA256:a410694d09fc5708d980a61a5abcb9633a591364f1ecc7e97ad5daef9c898c38
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.4-3.debian.tar.xz' audit_2.8.4-3.debian.tar.xz 16712 SHA256:2b4b16cf58c3a6180d380bd4ad1d30a38fa22826ca3c1233c5298138427e29d0
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:2.8.4-3/ (for browsing the source)
- https://sources.debian.net/src/audit/1:2.8.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:2.8.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `avahi=0.7-4`

Binary Packages:

- `libavahi-client3:amd64=0.7-4+b1`
- `libavahi-common-data:amd64=0.7-4+b1`
- `libavahi-common3:amd64=0.7-4+b1`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.7-4
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.7-4.dsc' avahi_0.7-4.dsc 3888 SHA256:22b467d4f5872b744eb62d7e6b022429672c6fa64488dc0af8bc5a19188732cd
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.7.orig.tar.gz' avahi_0.7.orig.tar.gz 1333400 SHA256:57a99b5dfe7fdae794e3d1ee7a62973a368e91e414bd0dfa5d84434de5b14804
'http://deb.debian.org/debian/pool/main/a/avahi/avahi_0.7-4.debian.tar.xz' avahi_0.7-4.debian.tar.xz 31756 SHA256:46414437ef2cbdb7d9a02f8b49da5e61980dec1c838a6bf62acd0d6e762b838e
```

Other potentially useful URLs:

- https://sources.debian.net/src/avahi/0.7-4/ (for browsing the source)
- https://sources.debian.net/src/avahi/0.7-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/avahi/0.7-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=10.3+deb10u3`

Binary Packages:

- `base-files=10.3+deb10u3`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=10.3+deb10u3
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_10.3+deb10u3.dsc' base-files_10.3+deb10u3.dsc 1103 SHA256:6d8acb1017165c464fbe00e7a6a9b939039578914b6a69ac97be5f02077ec3bf
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_10.3+deb10u3.tar.xz' base-files_10.3+deb10u3.tar.xz 65324 SHA256:eb19b3f1e052665b565ef07c7e50c9dcc33783169f2bfcc71ec826a75ce61008
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/10.3+deb10u3/ (for browsing the source)
- https://sources.debian.net/src/base-files/10.3+deb10u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/10.3+deb10u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.46`

Binary Packages:

- `base-passwd=3.5.46`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.46
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.46.dsc' base-passwd_3.5.46.dsc 1651 SHA256:98b5d79c9f06e05e9f41013f8fee48b08d0ffe398653b6f8bbd93c1ae1f24bd4
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.46.tar.xz' base-passwd_3.5.46.tar.xz 52780 SHA256:da15e380557b5a00cdc14018e3da6cbeaaadc786f2c3cb5b8f1fb4acc150b3da
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.46/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.46/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.46/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.0-4`

Binary Packages:

- `bash=5.0-4`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.0-4
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.0-4.dsc' bash_5.0-4.dsc 2305 SHA256:fe746c72de6e61866a0ed4e21a5b9d154966a8684ec3bdf5bacc70d5351f6282
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA256:893858ba233d65bda38039e99dd96a4102b2f6a2d5e6c1c546e0794a60beed97
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.0-4.debian.tar.xz' bash_5.0-4.debian.tar.xz 91884 SHA256:1e33dff5dd8604fa4205a1746828063cd96a1e635355f3626b54fef155b8c4e5
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/5.0-4/ (for browsing the source)
- https://sources.debian.net/src/bash/5.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/5.0-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `boost1.67=1.67.0-13+deb10u1`

Binary Packages:

- `libboost-atomic1.67.0:amd64=1.67.0-13+deb10u1`
- `libboost-chrono1.67.0:amd64=1.67.0-13+deb10u1`
- `libboost-date-time1.67.0:amd64=1.67.0-13+deb10u1`
- `libboost-filesystem1.67.0:amd64=1.67.0-13+deb10u1`
- `libboost-iostreams1.67.0:amd64=1.67.0-13+deb10u1`
- `libboost-locale1.67.0:amd64=1.67.0-13+deb10u1`
- `libboost-system1.67.0:amd64=1.67.0-13+deb10u1`
- `libboost-thread1.67.0:amd64=1.67.0-13+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libboost-atomic1.67.0/copyright`, `/usr/share/doc/libboost-chrono1.67.0/copyright`, `/usr/share/doc/libboost-date-time1.67.0/copyright`, `/usr/share/doc/libboost-filesystem1.67.0/copyright`, `/usr/share/doc/libboost-iostreams1.67.0/copyright`, `/usr/share/doc/libboost-locale1.67.0/copyright`, `/usr/share/doc/libboost-system1.67.0/copyright`, `/usr/share/doc/libboost-thread1.67.0/copyright`)

- `BSDRegex`
- `BSL-1.0`
- `OldBoost1`
- `OldBoost2`
- `OldBoost3`
- `OldBoost4`
- `PSF`
- `Perforce`
- `SGI`
- `Zlib`
- `boehm_gc`

Source:

```console
$ apt-get source -qq --print-uris boost1.67=1.67.0-13+deb10u1
'http://deb.debian.org/debian/pool/main/b/boost1.67/boost1.67_1.67.0-13+deb10u1.dsc' boost1.67_1.67.0-13+deb10u1.dsc 8402 SHA256:3a7ac414c257170befd3ca714d8f26ae9bc2a6adf10bdbe400800ec723e6c5bb
'http://deb.debian.org/debian/pool/main/b/boost1.67/boost1.67_1.67.0.orig.tar.gz' boost1.67_1.67.0.orig.tar.gz 85291274 SHA256:40c2e1fb225b688453ceeb3348265b4b7f2eee216e14f5158d51b0fef2fe0bb5
'http://deb.debian.org/debian/pool/main/b/boost1.67/boost1.67_1.67.0-13+deb10u1.debian.tar.xz' boost1.67_1.67.0-13+deb10u1.debian.tar.xz 351404 SHA256:48b68b700f8f570c5db7c8ca13dce5c7c986bdc418a7d6ec1175239e11e963b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/boost1.67/1.67.0-13+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/boost1.67/1.67.0-13+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/boost1.67/1.67.0-13+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.6-9.2~deb10u1`

Binary Packages:

- `bzip2=1.0.6-9.2~deb10u1`
- `libbz2-1.0:amd64=1.0.6-9.2~deb10u1`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-9.2~deb10u1
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-9.2~deb10u1.dsc' bzip2_1.0.6-9.2~deb10u1.dsc 2380 SHA256:f518d7c599e1028002a739bd9123fa23767d74e1c5cf1d05f36eb7de9fc25b5c
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.6-9.2~deb10u1.debian.tar.bz2' bzip2_1.0.6-9.2~deb10u1.debian.tar.bz2 27542 SHA256:44900f7371503fe35ea7d3aa5b8ab8c677300be9b0d5277838d0c874be9c8541
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.6-9.2~deb10u1/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.6-9.2~deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.6-9.2~deb10u1/ (for access to the source package after it no longer exists in the archive)

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
- `libcairo2:amd64=1.16.0-4`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo2/copyright`)

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

### `dpkg` source package: `cdebconf=0.249`

Binary Packages:

- `libdebconfclient0:amd64=0.249`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.249
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.249.dsc' cdebconf_0.249.dsc 2783 SHA256:6a0061589add058e5130e9be20ea45056701fd71ac0d26defd9a8c53758486f1
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.249.tar.xz' cdebconf_0.249.tar.xz 275256 SHA256:f7211ab20bfde7a0726cd566fd004b08e7ee358d238e35ea215f4fe0b3883b3e
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.249/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.249/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.249/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `chromaprint=1.4.3-3`

Binary Packages:

- `libchromaprint1:amd64=1.4.3-3`

Licenses: (parsed from: `/usr/share/doc/libchromaprint1/copyright`)

- `BSD-3-clause`
- `Expat`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris chromaprint=1.4.3-3
'http://deb.debian.org/debian/pool/main/c/chromaprint/chromaprint_1.4.3-3.dsc' chromaprint_1.4.3-3.dsc 2242 SHA256:99d4ada350aa0f9bbb3f0dbdbe8e03d687989c3f59ca3a3fd19199e9d06005e4
'http://deb.debian.org/debian/pool/main/c/chromaprint/chromaprint_1.4.3.orig.tar.gz' chromaprint_1.4.3.orig.tar.gz 613718 SHA256:d4ae6596283aad7a015a5b0445012054c634a4b9329ecb23000cd354b40a283b
'http://deb.debian.org/debian/pool/main/c/chromaprint/chromaprint_1.4.3-3.debian.tar.xz' chromaprint_1.4.3-3.debian.tar.xz 6660 SHA256:e1861bc82e1b3fd4641142beedf1543118ebb826263622bd4811c17b78b06377
```

Other potentially useful URLs:

- https://sources.debian.net/src/chromaprint/1.4.3-3/ (for browsing the source)
- https://sources.debian.net/src/chromaprint/1.4.3-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/chromaprint/1.4.3-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `clp=1.16.11+repack1-1`

Binary Packages:

- `coinor-libclp1=1.16.11+repack1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libclp1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris clp=1.16.11+repack1-1
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.16.11+repack1-1.dsc' clp_1.16.11+repack1-1.dsc 2382 SHA256:b195c1d8201b73b729bfcc2c240ab6403f879f3e48da6359d8f26bf5ca5dcc16
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.16.11+repack1.orig.tar.xz' clp_1.16.11+repack1.orig.tar.xz 1201424 SHA256:e9b10caac993e80461c6addb502a4b44721fb161175bf6e3bc792f404c60a923
'http://deb.debian.org/debian/pool/main/c/clp/clp_1.16.11+repack1-1.debian.tar.xz' clp_1.16.11+repack1-1.debian.tar.xz 9720 SHA256:37a77dbda29868632784a588f8c7b91962f322b5d829acd46b077bd503355612
```

Other potentially useful URLs:

- https://sources.debian.net/src/clp/1.16.11+repack1-1/ (for browsing the source)
- https://sources.debian.net/src/clp/1.16.11+repack1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/clp/1.16.11+repack1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `codec2=0.8.1-2`

Binary Packages:

- `libcodec2-0.8.1:amd64=0.8.1-2`

Licenses: (parsed from: `/usr/share/doc/libcodec2-0.8.1/copyright`)

- `COPYING`
- `JMVBSD`
- `KISSFFTBSD`
- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris codec2=0.8.1-2
'http://deb.debian.org/debian/pool/main/c/codec2/codec2_0.8.1-2.dsc' codec2_0.8.1-2.dsc 2054 SHA256:cb911788ed810c6c413155d59490e5dbf5ce4876254e07c04750dc25de10fcee
'http://deb.debian.org/debian/pool/main/c/codec2/codec2_0.8.1.orig.tar.xz' codec2_0.8.1.orig.tar.xz 8868212 SHA256:a07cdaacf59c3f7dbb1c63b769d443af486c434b3bd031fb4edd568ce3e613d6
'http://deb.debian.org/debian/pool/main/c/codec2/codec2_0.8.1-2.debian.tar.xz' codec2_0.8.1-2.debian.tar.xz 51440 SHA256:83978f4a18586921728d5329e84da26d5f8b722b706495a3a27c3597cb8d3d7a
```

Other potentially useful URLs:

- https://sources.debian.net/src/codec2/0.8.1-2/ (for browsing the source)
- https://sources.debian.net/src/codec2/0.8.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/codec2/0.8.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinmp=1.8.3-2`

Binary Packages:

- `coinor-libcoinmp1v5:amd64=1.8.3-2+b11`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinmp1v5/copyright`)

- `CPL-1`
- `EPL-1`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris coinmp=1.8.3-2
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.8.3-2.dsc' coinmp_1.8.3-2.dsc 2011 SHA256:ad3f172d280226e0040a01603df3c54d8d78d354ca615b829bc425fe9bca5816
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.8.3.orig.tar.gz' coinmp_1.8.3.orig.tar.gz 7109200 SHA256:253ea6f55ba6cda18f35ccc8ebe6d6e2e9023df64d02f6536abc8b9ae4206681
'http://deb.debian.org/debian/pool/main/c/coinmp/coinmp_1.8.3-2.debian.tar.xz' coinmp_1.8.3-2.debian.tar.xz 35360 SHA256:1f1348eb44a1204368fd98fd764d702443eacc0ff30dc5f3a14cc4696995d8bd
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinmp/1.8.3-2/ (for browsing the source)
- https://sources.debian.net/src/coinmp/1.8.3-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinmp/1.8.3-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-cbc=2.9.9+repack1-1`

Binary Packages:

- `coinor-libcbc3=2.9.9+repack1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcbc3/copyright`)

- `EPL-1`
- `GPL-3`
- `LUCENT`

Source:

```console
$ apt-get source -qq --print-uris coinor-cbc=2.9.9+repack1-1
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.9.9+repack1-1.dsc' coinor-cbc_2.9.9+repack1-1.dsc 2434 SHA256:570afd7a7ecdfc4a738cb20ff163e14213462ff23373192b8d2ea01fe7944ef7
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.9.9+repack1.orig.tar.xz' coinor-cbc_2.9.9+repack1.orig.tar.xz 891548 SHA256:85bdafbd07624e389d6dd2ee82881ce805597d5f6b13eef2892bbc4518ffeec4
'http://deb.debian.org/debian/pool/main/c/coinor-cbc/coinor-cbc_2.9.9+repack1-1.debian.tar.xz' coinor-cbc_2.9.9+repack1-1.debian.tar.xz 11060 SHA256:fe97021b0bbad31f9222d6015ccd0207317aacfa3a3de139274199747619b3f9
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-cbc/2.9.9+repack1-1/ (for browsing the source)
- https://sources.debian.net/src/coinor-cbc/2.9.9+repack1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-cbc/2.9.9+repack1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-cgl=0.59.10+repack1-1`

Binary Packages:

- `coinor-libcgl1=0.59.10+repack1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcgl1/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-cgl=0.59.10+repack1-1
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.59.10+repack1-1.dsc' coinor-cgl_0.59.10+repack1-1.dsc 2338 SHA256:e2c424b7488131378d35918e3804854aa33f3e657cf196bb6c9ac2a9f09ad129
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.59.10+repack1.orig.tar.xz' coinor-cgl_0.59.10+repack1.orig.tar.xz 548080 SHA256:5d73a6372bf9c7d480a37189e636af1ebc4d2b5090d5fcca93c0f50589dd094d
'http://deb.debian.org/debian/pool/main/c/coinor-cgl/coinor-cgl_0.59.10+repack1-1.debian.tar.xz' coinor-cgl_0.59.10+repack1-1.debian.tar.xz 7612 SHA256:fe87849cc7924b88aa9a40c7e79fef9c62aab26337465240dbe64aaa4aab7119
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-cgl/0.59.10+repack1-1/ (for browsing the source)
- https://sources.debian.net/src/coinor-cgl/0.59.10+repack1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-cgl/0.59.10+repack1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinor-osi=0.107.9+repack1-1`

Binary Packages:

- `coinor-libosi1v5=0.107.9+repack1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libosi1v5/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinor-osi=0.107.9+repack1-1
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.107.9+repack1-1.dsc' coinor-osi_0.107.9+repack1-1.dsc 2274 SHA256:34166ecce1c04c06dd2f6dd0531c8195c1fe9e63428158afb00b42dbc804c43f
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.107.9+repack1.orig.tar.xz' coinor-osi_0.107.9+repack1.orig.tar.xz 451124 SHA256:a32192621fa2eb8b9e19ccc6197d90dd9b9104b69025ec68eaec2a8e51876bab
'http://deb.debian.org/debian/pool/main/c/coinor-osi/coinor-osi_0.107.9+repack1-1.debian.tar.xz' coinor-osi_0.107.9+repack1-1.debian.tar.xz 7856 SHA256:dff858ff54dfcaa60b7ef3e2a855eabb96dd24717474000957bf2fbe1fa5bc78
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinor-osi/0.107.9+repack1-1/ (for browsing the source)
- https://sources.debian.net/src/coinor-osi/0.107.9+repack1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinor-osi/0.107.9+repack1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coinutils=2.10.14+repack1-1`

Binary Packages:

- `coinor-libcoinutils3v5=2.10.14+repack1-1`

Licenses: (parsed from: `/usr/share/doc/coinor-libcoinutils3v5/copyright`)

- `EPL-1`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coinutils=2.10.14+repack1-1
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.10.14+repack1-1.dsc' coinutils_2.10.14+repack1-1.dsc 2297 SHA256:6833a0537cb3f057315c8eef8b923fec88266f0950376547f142209c8eef6577
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.10.14+repack1.orig.tar.xz' coinutils_2.10.14+repack1.orig.tar.xz 817232 SHA256:fd891f6fe8744e8fad889d8121edcc1f3c12b29a2fc454871a62b07e985ddd4c
'http://deb.debian.org/debian/pool/main/c/coinutils/coinutils_2.10.14+repack1-1.debian.tar.xz' coinutils_2.10.14+repack1-1.debian.tar.xz 8444 SHA256:a0f8e0ae4c180943c963baa726a72920d90ce1e3244780c405a2047d5e76c9f0
```

Other potentially useful URLs:

- https://sources.debian.net/src/coinutils/2.10.14+repack1-1/ (for browsing the source)
- https://sources.debian.net/src/coinutils/2.10.14+repack1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coinutils/2.10.14+repack1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `colord=1.4.3-4`

Binary Packages:

- `libcolord2:amd64=1.4.3-4`

Licenses: (parsed from: `/usr/share/doc/libcolord2/copyright`)

- `CC0`
- `GFDL-NIV`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris colord=1.4.3-4
'http://deb.debian.org/debian/pool/main/c/colord/colord_1.4.3-4.dsc' colord_1.4.3-4.dsc 2885 SHA256:699c8a68fc9f62de1af1f81dd6aeeda382505f0ed0bac3b49f1dde0f6bd98214
'http://deb.debian.org/debian/pool/main/c/colord/colord_1.4.3.orig.tar.xz' colord_1.4.3.orig.tar.xz 1858552 SHA256:9a8e669ee1ea31632bee636cc57353f703c2ea9b64cd6e02bbaabe9a1e549df7
'http://deb.debian.org/debian/pool/main/c/colord/colord_1.4.3-4.debian.tar.xz' colord_1.4.3-4.debian.tar.xz 29016 SHA256:706d468cf1e79eac0963822526cec615f80dac963ff814c183f025492a532607
```

Other potentially useful URLs:

- https://sources.debian.net/src/colord/1.4.3-4/ (for browsing the source)
- https://sources.debian.net/src/colord/1.4.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/colord/1.4.3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.30-3`

Binary Packages:

- `coreutils=8.30-3`

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

### `dpkg` source package: `cryptsetup=2:2.1.0-5+deb10u2`

Binary Packages:

- `libcryptsetup12:amd64=2:2.1.0-5+deb10u2`

Licenses: (parsed from: `/usr/share/doc/libcryptsetup12/copyright`)

- `Apache-2.0`
- `CC0`
- `CC0-1.0`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with OpenSSL exception`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-2.1+ with OpenSSL exception`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris cryptsetup=2:2.1.0-5+deb10u2
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_2.1.0-5+deb10u2.dsc' cryptsetup_2.1.0-5+deb10u2.dsc 2842 SHA256:be8654f3862a7271cb313a31a862729697c92e28c4dff94d7b575d98e98d9e1a
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_2.1.0.orig.tar.gz' cryptsetup_2.1.0.orig.tar.gz 10708886 SHA256:e34b6502a8f72a5d76b0dc25349612c83e81d6d7d59a3feda50d66e6859f669e
'http://deb.debian.org/debian/pool/main/c/cryptsetup/cryptsetup_2.1.0-5+deb10u2.debian.tar.xz' cryptsetup_2.1.0-5+deb10u2.debian.tar.xz 112312 SHA256:f775f41955845c849659b83e324514e3b14dbf7a63a7331b9ccbcf3c77252ab0
```

Other potentially useful URLs:

- https://sources.debian.net/src/cryptsetup/2:2.1.0-5+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/cryptsetup/2:2.1.0-5+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cryptsetup/2:2.1.0-5+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `crystalhd=1:0.0~git20110715.fdd2f19-13`

Binary Packages:

- `libcrystalhd3:amd64=1:0.0~git20110715.fdd2f19-13`

Licenses: (parsed from: `/usr/share/doc/libcrystalhd3/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris crystalhd=1:0.0~git20110715.fdd2f19-13
'http://deb.debian.org/debian/pool/main/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-13.dsc' crystalhd_0.0~git20110715.fdd2f19-13.dsc 2363 SHA256:c545c6e51bdd03a34a1f311eb5d52b1316ba9f365cdbba39a1b0fa413ed3df76
'http://deb.debian.org/debian/pool/main/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz' crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz 1186072 SHA256:a1c22908b85085dcc4591bc033fe054be63eab59b7d35f0a9ab3fcb2600722b7
'http://deb.debian.org/debian/pool/main/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-13.debian.tar.xz' crystalhd_0.0~git20110715.fdd2f19-13.debian.tar.xz 15320 SHA256:66308990232a5a91501f5243946a95a03ef36e922f6704c18d4ea380e02ce9bb
```

Other potentially useful URLs:

- https://sources.debian.net/src/crystalhd/1:0.0~git20110715.fdd2f19-13/ (for browsing the source)
- https://sources.debian.net/src/crystalhd/1:0.0~git20110715.fdd2f19-13/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/crystalhd/1:0.0~git20110715.fdd2f19-13/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cups=2.2.10-6+deb10u2`

Binary Packages:

- `libcups2:amd64=2.2.10-6+deb10u2`
- `libcupsimage2:amd64=2.2.10-6+deb10u2`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`, `/usr/share/doc/libcupsimage2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.2.10-6+deb10u2
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10-6+deb10u2.dsc' cups_2.2.10-6+deb10u2.dsc 3472 SHA256:5bee91b9c8c35ad211d67e2dfe250787dd4bb3a2f5c67db1b2b3f3794a0ec331
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10.orig.tar.gz' cups_2.2.10.orig.tar.gz 10403568 SHA256:77c8b2b3bb7fe8b5fbfffc307f2c817b2d7ec67b657f261a1dd1c61ab81205bb
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10.orig.tar.gz.asc' cups_2.2.10.orig.tar.gz.asc 864 SHA256:be235dd0cc526e5bde2a67f0dc2888be5d8dc40d1dfa44ab1a322d83f606e82d
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10-6+deb10u2.debian.tar.xz' cups_2.2.10-6+deb10u2.debian.tar.xz 360016 SHA256:86f8f8acfd8251602e3f629b5561775a05f41ed9b472752e46eec1e2c930bb33
```

Other potentially useful URLs:

- https://sources.debian.net/src/cups/2.2.10-6+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/cups/2.2.10-6+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cups/2.2.10-6+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.64.0-4+deb10u1`

Binary Packages:

- `curl=7.64.0-4+deb10u1`
- `libcurl3-gnutls:amd64=7.64.0-4+deb10u1`
- `libcurl4:amd64=7.64.0-4+deb10u1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.64.0-4+deb10u1
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.64.0-4+deb10u1.dsc' curl_7.64.0-4+deb10u1.dsc 2719 SHA256:bdbc61f9785516009ae74bb3775e21bed7ab8fdd7bfef4a1a4f471d5218adf3e
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.64.0.orig.tar.gz' curl_7.64.0.orig.tar.gz 4032645 SHA256:cb90d2eb74d4e358c1ed1489f8e3af96b50ea4374ad71f143fa4595e998d81b5
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.64.0-4+deb10u1.debian.tar.xz' curl_7.64.0-4+deb10u1.debian.tar.xz 34156 SHA256:911407ad8d73d0592db7f1a015656089563bb7dab279ec33bff855adf56bcf1b
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.64.0-4+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/curl/7.64.0-4+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.64.0-4+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-1+deb10u1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-1+deb10u1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-1+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-1+deb10u1
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-1+deb10u1.dsc' cyrus-sasl2_2.1.27+dfsg-1+deb10u1.dsc 3580 SHA256:4537e3acdf1e009c402110aa47d6f5acef87594b4ad7e13733d3956d85b2d110
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-1+deb10u1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-1+deb10u1.debian.tar.xz 99972 SHA256:df71d3cd6c623702c5daeab440c91899c8d4e7955cf632e6bd07de3a65cb8538
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg-1+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.10.2-5`

Binary Packages:

- `dash=0.5.10.2-5`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.10.2-5
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2-5.dsc' dash_0.5.10.2-5.dsc 1756 SHA256:6255cf35f61df5122637856ad0912986de1c20875177932de1c971b7bbbbd848
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA256:3c663919dc5c66ec991da14c7cf7e0be8ad00f3db73986a987c118862b5f6071
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2-5.debian.tar.xz' dash_0.5.10.2-5.debian.tar.xz 41804 SHA256:fabf27bd78778b151143ed598a6b65019cfce5dd087d9693b848346459951d24
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.10.2-5/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.10.2-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.10.2-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.5`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.5
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.5.dsc' db5.3_5.3.28+dfsg1-0.5.dsc 2804 SHA256:600ef735e47273c7e8de0a9bbbf2d6f31cb1d2851117f94776d7952588c0ecc4
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.5.debian.tar.xz' db5.3_5.3.28+dfsg1-0.5.debian.tar.xz 29128 SHA256:682c1736c1b5f3afbd90cf24e085a0437821ae595dc54aeef8c09ddd1c3d05fe
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.5/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dbus-glib=0.110-4`

Binary Packages:

- `libdbus-glib-1-2:amd64=0.110-4`

Licenses: (parsed from: `/usr/share/doc/libdbus-glib-1-2/copyright`)

- `AFL-2.1`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dbus-glib=0.110-4
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.110-4.dsc' dbus-glib_0.110-4.dsc 2526 SHA256:332cc13e6797afdb97879ab75b8013f6174958d49c791e27d3a86b799d1ce03f
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.110.orig.tar.gz' dbus-glib_0.110.orig.tar.gz 836497 SHA256:7ce4760cf66c69148f6bd6c92feaabb8812dee30846b24cd0f7395c436d7e825
'http://deb.debian.org/debian/pool/main/d/dbus-glib/dbus-glib_0.110-4.debian.tar.xz' dbus-glib_0.110-4.debian.tar.xz 32236 SHA256:51b989f93adc86d050726ead00ac68776bf98297e8fa5134c07deba5872d09c8
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus-glib/0.110-4/ (for browsing the source)
- https://sources.debian.net/src/dbus-glib/0.110-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus-glib/0.110-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dbus=1.12.16-1`

Binary Packages:

- `dbus=1.12.16-1`
- `dbus-user-session=1.12.16-1`
- `libdbus-1-3:amd64=1.12.16-1`

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
$ apt-get source -qq --print-uris dbus=1.12.16-1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.16-1.dsc' dbus_1.12.16-1.dsc 3752 SHA256:86a42029448c3ef881d351db0d298b2d6ecd260110e06b815b520eed63749749
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.16.orig.tar.gz' dbus_1.12.16.orig.tar.gz 2093296 SHA256:54a22d2fa42f2eb2a871f32811c6005b531b9613b1b93a0d269b05e7549fec80
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.16.orig.tar.gz.asc' dbus_1.12.16.orig.tar.gz.asc 833 SHA256:5906e4cb235e8a3a88f5f0566b7775b065dc3e14683c2c379af86b4f428042f9
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.16-1.debian.tar.xz' dbus_1.12.16-1.debian.tar.xz 64052 SHA256:61376d1420c56f81538bc3d5dc3492d9ee08714f69d0cbed804d28fc14421e1f
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus/1.12.16-1/ (for browsing the source)
- https://sources.debian.net/src/dbus/1.12.16-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus/1.12.16-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dconf=0.30.1-2`

Binary Packages:

- `dconf-gsettings-backend:amd64=0.30.1-2`
- `dconf-service=0.30.1-2`
- `libdconf1:amd64=0.30.1-2`

Licenses: (parsed from: `/usr/share/doc/dconf-gsettings-backend/copyright`, `/usr/share/doc/dconf-service/copyright`, `/usr/share/doc/libdconf1/copyright`)

- `GPL-3`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dconf=0.30.1-2
'http://deb.debian.org/debian/pool/main/d/dconf/dconf_0.30.1-2.dsc' dconf_0.30.1-2.dsc 2530 SHA256:c5544652d312f098047b553a734441f7366bdf821ec22a33e2ea84115f5df37c
'http://deb.debian.org/debian/pool/main/d/dconf/dconf_0.30.1.orig.tar.xz' dconf_0.30.1.orig.tar.xz 104376 SHA256:549a3a7cc3881318107dc48a7b02ee8f88c9127acaf2d47f7724f78a8f6d02b7
'http://deb.debian.org/debian/pool/main/d/dconf/dconf_0.30.1-2.debian.tar.xz' dconf_0.30.1-2.debian.tar.xz 9552 SHA256:4658e91e59a50bd6d7360d77d783f6e086eb67c357f74a5c2b61e1e4d423b437
```

Other potentially useful URLs:

- https://sources.debian.net/src/dconf/0.30.1-2/ (for browsing the source)
- https://sources.debian.net/src/dconf/0.30.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dconf/0.30.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.71`

Binary Packages:

- `debconf=1.5.71`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.71
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.71.dsc' debconf_1.5.71.dsc 2047 SHA256:18580a7817060c492048fac9fe0c859b1f5ca07538decfb32b182948a15cab79
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.71.tar.xz' debconf_1.5.71.tar.xz 571272 SHA256:dc23f44775be0d2f52f18eaff4d2d47ef62ae50333df1b737248c8a2635ce433
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.71/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.71/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.71/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `debianutils=4.8.6.1`

Binary Packages:

- `debianutils=4.8.6.1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.6.1
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.6.1.dsc' debianutils_4.8.6.1.dsc 1625 SHA256:fa869200410510cdefc85c89755d21ac054836a18b6916aedeba472e4b0567bb
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.8.6.1.tar.xz' debianutils_4.8.6.1.tar.xz 156604 SHA256:099f1e8a7278b26145a2ba2dda84c4118403bfab38c8d7070a6235a7ffcb55ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.8.6.1/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.8.6.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.8.6.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `desktop-file-utils=0.23-4`

Binary Packages:

- `desktop-file-utils=0.23-4`

Licenses: (parsed from: `/usr/share/doc/desktop-file-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris desktop-file-utils=0.23-4
'http://deb.debian.org/debian/pool/main/d/desktop-file-utils/desktop-file-utils_0.23-4.dsc' desktop-file-utils_0.23-4.dsc 2175 SHA256:44a7cc891021ece9838fcd2a44ad31bb1f04173760edab15c0965c59887ee86c
'http://deb.debian.org/debian/pool/main/d/desktop-file-utils/desktop-file-utils_0.23.orig.tar.xz' desktop-file-utils_0.23.orig.tar.xz 132000 SHA256:6c094031bdec46c9f621708f919084e1cb5294e2c5b1e4c883b3e70cb8903385
'http://deb.debian.org/debian/pool/main/d/desktop-file-utils/desktop-file-utils_0.23-4.debian.tar.xz' desktop-file-utils_0.23-4.debian.tar.xz 5568 SHA256:383b26ad48089a1b798152eb52f7f7cdcce3567ffc75b7c474336e2d381e7a69
```

Other potentially useful URLs:

- https://sources.debian.net/src/desktop-file-utils/0.23-4/ (for browsing the source)
- https://sources.debian.net/src/desktop-file-utils/0.23-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/desktop-file-utils/0.23-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `dpkg=1.19.7`

Binary Packages:

- `dpkg=1.19.7`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

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

### `dpkg` source package: `e2fsprogs=1.44.5-1+deb10u3`

Binary Packages:

- `e2fsprogs=1.44.5-1+deb10u3`
- `libcom-err2:amd64=1.44.5-1+deb10u3`
- `libext2fs2:amd64=1.44.5-1+deb10u3`
- `libss2:amd64=1.44.5-1+deb10u3`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.44.5-1+deb10u3
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.44.5-1+deb10u3.dsc' e2fsprogs_1.44.5-1+deb10u3.dsc 2903 SHA256:acdc31d6fd491f9db97aabc96340559d8492b98e3549df32d8369690e03058dc
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.44.5.orig.tar.gz' e2fsprogs_1.44.5.orig.tar.gz 7619237 SHA256:2e211fae27ef74d5af4a4e40b10b8df7f87c655933bd171aab4889bfc4e6d1cc
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.44.5.orig.tar.gz.asc' e2fsprogs_1.44.5.orig.tar.gz.asc 488 SHA256:c0e3e4e51f46c005890963b005015b784b2f19e291a16a15681b9906528f557e
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.44.5-1+deb10u3.debian.tar.xz' e2fsprogs_1.44.5-1+deb10u3.debian.tar.xz 82412 SHA256:0114857448922a218613f369f665f03f1b1435004c9d79ce5ee1a8a8a6cec53f
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.44.5-1+deb10u3/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.44.5-1+deb10u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.44.5-1+deb10u3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `exiv2=0.25-4`

Binary Packages:

- `libexiv2-14:amd64=0.25-4`

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
$ apt-get source -qq --print-uris exiv2=0.25-4
'http://deb.debian.org/debian/pool/main/e/exiv2/exiv2_0.25-4.dsc' exiv2_0.25-4.dsc 2237 SHA256:144b9d823f69b93737dee5567d4483e1cb24654bf6f2f48fd0e8cd04bf204fe8
'http://deb.debian.org/debian/pool/main/e/exiv2/exiv2_0.25.orig.tar.gz' exiv2_0.25.orig.tar.gz 5434325 SHA256:c80bfc778a15fdb06f71265db2c3d49d8493c382e516cb99b8c9f9cbde36efa4
'http://deb.debian.org/debian/pool/main/e/exiv2/exiv2_0.25-4.debian.tar.xz' exiv2_0.25-4.debian.tar.xz 26800 SHA256:21eb7f23d4e56afbd802c931fbc805ddec488b85be074972d15eaf8b1af0e936
```

Other potentially useful URLs:

- https://sources.debian.net/src/exiv2/0.25-4/ (for browsing the source)
- https://sources.debian.net/src/exiv2/0.25-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/exiv2/0.25-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.6-2+deb10u1`

Binary Packages:

- `libexpat1:amd64=2.2.6-2+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.6-2+deb10u1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.6-2+deb10u1.dsc' expat_2.2.6-2+deb10u1.dsc 2136 SHA256:a32a035c9883b70ddf739eaacaa5c790ec5bf3027ba61eefdbc0cdf634aa4d96
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.6.orig.tar.gz' expat_2.2.6.orig.tar.gz 8275473 SHA256:574499cba22a599393e28d99ecfa1e7fc85be7d6651d543045244d5b561cb7ff
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.6-2+deb10u1.debian.tar.xz' expat_2.2.6-2+deb10u1.debian.tar.xz 12032 SHA256:15e75199a33c4e902788410f37e784c1082906e703c8619c4cfc715a0191e02b
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.6-2+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.6-2+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.6-2+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ffmpeg2theora=0.30-1`

Binary Packages:

- `ffmpeg2theora=0.30-1+b3`

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

### `dpkg` source package: `ffmpeg=7:4.1.4-1~deb10u1`

Binary Packages:

- `ffmpeg=7:4.1.4-1~deb10u1`
- `libavcodec58:amd64=7:4.1.4-1~deb10u1`
- `libavdevice58:amd64=7:4.1.4-1~deb10u1`
- `libavfilter7:amd64=7:4.1.4-1~deb10u1`
- `libavformat58:amd64=7:4.1.4-1~deb10u1`
- `libavresample4:amd64=7:4.1.4-1~deb10u1`
- `libavutil56:amd64=7:4.1.4-1~deb10u1`
- `libpostproc55:amd64=7:4.1.4-1~deb10u1`
- `libswresample3:amd64=7:4.1.4-1~deb10u1`
- `libswscale5:amd64=7:4.1.4-1~deb10u1`

Licenses: (parsed from: `/usr/share/doc/ffmpeg/copyright`, `/usr/share/doc/libavcodec58/copyright`, `/usr/share/doc/libavdevice58/copyright`, `/usr/share/doc/libavfilter7/copyright`, `/usr/share/doc/libavformat58/copyright`, `/usr/share/doc/libavresample4/copyright`, `/usr/share/doc/libavutil56/copyright`, `/usr/share/doc/libpostproc55/copyright`, `/usr/share/doc/libswresample3/copyright`, `/usr/share/doc/libswscale5/copyright`)

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
$ apt-get source -qq --print-uris ffmpeg=7:4.1.4-1~deb10u1
'http://deb.debian.org/debian/pool/main/f/ffmpeg/ffmpeg_4.1.4-1~deb10u1.dsc' ffmpeg_4.1.4-1~deb10u1.dsc 5211 SHA256:55a77c1af767d7809c46dfcfae237fc4876f2de2d4e76bf57733d2c9749dfebb
'http://deb.debian.org/debian/pool/main/f/ffmpeg/ffmpeg_4.1.4.orig.tar.xz' ffmpeg_4.1.4.orig.tar.xz 8896056 SHA256:f1f049a82fcfbf156564e73a3935d7e750891fab2abf302e735104fd4050a7e1
'http://deb.debian.org/debian/pool/main/f/ffmpeg/ffmpeg_4.1.4.orig.tar.xz.asc' ffmpeg_4.1.4.orig.tar.xz.asc 473 SHA256:1ae4a0a9a95b9da8c42268e4e876d344643d38fc1f7f34d49fc478cd97db2bd6
'http://deb.debian.org/debian/pool/main/f/ffmpeg/ffmpeg_4.1.4-1~deb10u1.debian.tar.xz' ffmpeg_4.1.4-1~deb10u1.debian.tar.xz 47556 SHA256:857b91059376c0336ce2ae9c365465e2c0b6eef5c2c70a48ae98a02d88c23aed
```

Other potentially useful URLs:

- https://sources.debian.net/src/ffmpeg/7:4.1.4-1~deb10u1/ (for browsing the source)
- https://sources.debian.net/src/ffmpeg/7:4.1.4-1~deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ffmpeg/7:4.1.4-1~deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ffms2=2.23-4`

Binary Packages:

- `libffms2-4:amd64=2.23-4`

Licenses: (parsed from: `/usr/share/doc/libffms2-4/copyright`)

- `Expat`
- `GPL-2`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris ffms2=2.23-4
'http://deb.debian.org/debian/pool/main/f/ffms2/ffms2_2.23-4.dsc' ffms2_2.23-4.dsc 2258 SHA256:2ba9193b6a9743c6dd7866a5aa3aebc68a28fe973050d7a751693be244cf2b8d
'http://deb.debian.org/debian/pool/main/f/ffms2/ffms2_2.23.orig.tar.gz' ffms2_2.23.orig.tar.gz 488940 SHA256:b09b2aa2b1c6f87f94a0a0dd8284b3c791cbe77f0f3df57af99ddebcd15273ed
'http://deb.debian.org/debian/pool/main/f/ffms2/ffms2_2.23-4.debian.tar.xz' ffms2_2.23-4.debian.tar.xz 10000 SHA256:a37f6fe2941af18882948aa23448e57dd637c3d60bfa4674f67bb5dec069f539
```

Other potentially useful URLs:

- https://sources.debian.net/src/ffms2/2.23-4/ (for browsing the source)
- https://sources.debian.net/src/ffms2/2.23-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ffms2/2.23-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `findutils=4.6.0+git+20190209-2`

Binary Packages:

- `findutils=4.6.0+git+20190209-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20190209-2
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20190209-2.dsc' findutils_4.6.0+git+20190209-2.dsc 2137 SHA256:e09430f44f976ee0e51e3226543247668b4ef88c05d14a84ed2d5a6f1bd07421
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20190209.orig.tar.xz' findutils_4.6.0+git+20190209.orig.tar.xz 1893084 SHA256:6832b3f6ddc0e2718795e6732ea40cc5309b948505f55fb9935919d6aaac7e9d
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.6.0+git+20190209-2.debian.tar.xz' findutils_4.6.0+git+20190209-2.debian.tar.xz 26628 SHA256:d6f4c6fedc27cf5d616c9fbf41a46b8fb8b078f1f21045b484419b145037e849
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.6.0+git+20190209-2/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.6.0+git+20190209-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.6.0+git+20190209-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `flac=1.3.2-3`

Binary Packages:

- `libflac8:amd64=1.3.2-3`

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
$ apt-get source -qq --print-uris flac=1.3.2-3
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.2-3.dsc' flac_1.3.2-3.dsc 2257 SHA256:a0afdc83307af2f0dc49bd13fdd9544c9f22502fe5330fefd58304982cc81df2
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.2.orig.tar.xz' flac_1.3.2.orig.tar.xz 776192 SHA256:91cfc3ed61dc40f47f050a109b08610667d73477af6ef36dcad31c31a4a8d53f
'http://deb.debian.org/debian/pool/main/f/flac/flac_1.3.2-3.debian.tar.xz' flac_1.3.2-3.debian.tar.xz 17984 SHA256:5bd025f01a9638f6c27eabbf94b760d066707e1c82d1e594ca295758a761ec78
```

Other potentially useful URLs:

- https://sources.debian.net/src/flac/1.3.2-3/ (for browsing the source)
- https://sources.debian.net/src/flac/1.3.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/flac/1.3.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `flite=2.1-release-3`

Binary Packages:

- `libflite1:amd64=2.1-release-3`

Licenses: (parsed from: `/usr/share/doc/libflite1/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris flite=2.1-release-3
'http://deb.debian.org/debian/pool/main/f/flite/flite_2.1-release-3.dsc' flite_2.1-release-3.dsc 2246 SHA256:3b5c97f6b3c8ff983d1fa76cb9e31e32179c4acc82a8b104a859f69348200489
'http://deb.debian.org/debian/pool/main/f/flite/flite_2.1-release.orig.tar.bz2' flite_2.1-release.orig.tar.bz2 14816327 SHA256:c73c3f6a2ea764977d6eaf0a287722d1e2066b4697088c552e342c790f3d2b85
'http://deb.debian.org/debian/pool/main/f/flite/flite_2.1-release-3.debian.tar.xz' flite_2.1-release-3.debian.tar.xz 48480 SHA256:c6dc054e21a06453026e3c9a80a20317eed206f5a055a38e853c32e666961f5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/flite/2.1-release-3/ (for browsing the source)
- https://sources.debian.net/src/flite/2.1-release-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/flite/2.1-release-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fontconfig=2.13.1-2`

Binary Packages:

- `fontconfig=2.13.1-2`
- `fontconfig-config=2.13.1-2`
- `libfontconfig1:amd64=2.13.1-2`

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

### `dpkg` source package: `freetype=2.9.1-3+deb10u1`

Binary Packages:

- `libfreetype6:amd64=2.9.1-3+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

- `BSD-3-Clause`
- `Catharon-OSL`
- `FSFUL`
- `FSFULLR`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `OpenGroup-BSD-like`
- `Permissive`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.9.1-3+deb10u1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1-3+deb10u1.dsc' freetype_2.9.1-3+deb10u1.dsc 3690 SHA256:ef4825d67d044be4ea2e86444eae166057f8bd7d5606abf82d5095f47a3a7bd1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1.orig-ft2demos.tar.gz' freetype_2.9.1.orig-ft2demos.tar.gz 294850 SHA256:3d440aad3481285c7455f1593577e375c9d5792c800bbaba68d46fd75130fab9
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1.orig-ft2demos.tar.gz.asc' freetype_2.9.1.orig-ft2demos.tar.gz.asc 359 SHA256:665b8357378dc715fbac964d05cdcc2a2f7fd1e9d7918a27bf50f4d0a17f0d30
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1.orig-ft2docs.tar.gz' freetype_2.9.1.orig-ft2docs.tar.gz 2123920 SHA256:f57c1297f5ad2ad4764f491317fa0f548bd307c4513185d4a0602412e83b1dc9
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1.orig-ft2docs.tar.gz.asc' freetype_2.9.1.orig-ft2docs.tar.gz.asc 359 SHA256:c4c674db43603f719018716970569d1722d0de46fa94757eb7f39266d72cdbd1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1.orig.tar.gz' freetype_2.9.1.orig.tar.gz 2533956 SHA256:ec391504e55498adceb30baceebd147a6e963f636eb617424bcfc47a169898ce
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1.orig.tar.gz.asc' freetype_2.9.1.orig.tar.gz.asc 359 SHA256:2c2c5ae3b3838053b94366639e802b18bc4761003ea15ce73402d276baec424d
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.9.1-3+deb10u1.debian.tar.xz' freetype_2.9.1-3+deb10u1.debian.tar.xz 111972 SHA256:7a2765961a01332f2d402d86a126a9480efb326c995b0db2108c0f825d78cbe2
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.9.1-3+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.9.1-3+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.9.1-3+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fribidi=1.0.5-3.1+deb10u1`

Binary Packages:

- `libfribidi0:amd64=1.0.5-3.1+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.5-3.1+deb10u1
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.5-3.1+deb10u1.dsc' fribidi_1.0.5-3.1+deb10u1.dsc 2476 SHA256:671fc5877218b7b86e1243fc38051f1e0290dd084fec76e23c67be86458be2ab
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.5.orig.tar.bz2' fribidi_1.0.5.orig.tar.bz2 2082617 SHA256:6a64f2a687f5c4f203a46fa659f43dd43d1f8b845df8d723107e8a7e6158e4ce
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.5-3.1+deb10u1.debian.tar.xz' fribidi_1.0.5-3.1+deb10u1.debian.tar.xz 9656 SHA256:6db937390812dcfe3c929999accfd376a310b67af9c4fdb7949f14c1cc62040d
```

Other potentially useful URLs:

- https://sources.debian.net/src/fribidi/1.0.5-3.1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/fribidi/1.0.5-3.1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fribidi/1.0.5-3.1+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `game-music-emu=0.6.2-1`

Binary Packages:

- `libgme0:amd64=0.6.2-1`

Licenses: (parsed from: `/usr/share/doc/libgme0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris game-music-emu=0.6.2-1
'http://deb.debian.org/debian/pool/main/g/game-music-emu/game-music-emu_0.6.2-1.dsc' game-music-emu_0.6.2-1.dsc 2006 SHA256:8359c17b8c7d7887b3d44a5ac4958e5456afbf816ba29e6713c1e4212dbe63eb
'http://deb.debian.org/debian/pool/main/g/game-music-emu/game-music-emu_0.6.2.orig.tar.xz' game-music-emu_0.6.2.orig.tar.xz 163052 SHA256:5046cb471d422dbe948b5f5dd4e5552aaef52a0899c4b2688e5a68a556af7342
'http://deb.debian.org/debian/pool/main/g/game-music-emu/game-music-emu_0.6.2-1.debian.tar.xz' game-music-emu_0.6.2-1.debian.tar.xz 4412 SHA256:8ea69035bd72261ec85e5f0486707d448f7491733ae055040a9995cebb0ea820
```

Other potentially useful URLs:

- https://sources.debian.net/src/game-music-emu/0.6.2-1/ (for browsing the source)
- https://sources.debian.net/src/game-music-emu/0.6.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/game-music-emu/0.6.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-8=8.3.0-6`

Binary Packages:

- `gcc-8-base:amd64=8.3.0-6`
- `libatomic1:amd64=8.3.0-6`
- `libgcc1:amd64=1:8.3.0-6`
- `libgfortran5:amd64=8.3.0-6`
- `libgomp1:amd64=8.3.0-6`
- `libquadmath0:amd64=8.3.0-6`
- `libstdc++6:amd64=8.3.0-6`

Licenses: (parsed from: `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-8=8.3.0-6
'http://deb.debian.org/debian/pool/main/g/gcc-8/gcc-8_8.3.0-6.dsc' gcc-8_8.3.0-6.dsc 32433 SHA256:3b380579af74f1a325a07cc5798f8bff5206f0820fcac5bf64ff2bbd0466867d
'http://deb.debian.org/debian/pool/main/g/gcc-8/gcc-8_8.3.0.orig.tar.gz' gcc-8_8.3.0.orig.tar.gz 87764363 SHA256:ee3fd608f66e5737f20cf71b176cfbf58f7c1d190ad6def33d57610cdae8eac2
'http://deb.debian.org/debian/pool/main/g/gcc-8/gcc-8_8.3.0-6.diff.gz' gcc-8_8.3.0-6.diff.gz 704334 SHA256:211e5e1022e115abbcb9eeb39cf4bf84958c4e8469c0cbe430569947a04c5415
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-8/8.3.0-6/ (for browsing the source)
- https://sources.debian.net/src/gcc-8/8.3.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-8/8.3.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.18.1-4`

Binary Packages:

- `libgdbm-compat4:amd64=1.18.1-4`
- `libgdbm6:amd64=1.18.1-4`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.18.1-4
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1-4.dsc' gdbm_1.18.1-4.dsc 2635 SHA256:14f2a1741041f3ee8ebe1db9985ec12855c856a4c545ace6140b1222030ae64a
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz' gdbm_1.18.1.orig.tar.gz 941863 SHA256:86e613527e5dba544e73208f42b78b7c022d4fa5a6d5498bf18c8d6f745b91dc
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz.asc' gdbm_1.18.1.orig.tar.gz.asc 412 SHA256:3254738e7689e44ac65e78a766806828b8282e6bb1c0e5bb6156a99e567889a5
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.18.1-4.debian.tar.xz' gdbm_1.18.1-4.debian.tar.xz 16460 SHA256:1a7771cf18cacf86b8415cbdeafa4e54dd2dadee59f0c29833aba476726594c5
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.18.1-4/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.18.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.18.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdk-pixbuf=2.38.1+dfsg-1`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.38.1+dfsg-1`
- `libgdk-pixbuf2.0-common=2.38.1+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.38.1+dfsg-1
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.38.1+dfsg-1.dsc' gdk-pixbuf_2.38.1+dfsg-1.dsc 2903 SHA256:6f201d9dcb9b867678fa619bf054ff871105daca0fbc6a2e0639997d2bff91bc
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.38.1+dfsg.orig.tar.xz' gdk-pixbuf_2.38.1+dfsg.orig.tar.xz 5428160 SHA256:9d8666f01bfb31df1168e50d08d5646d18884ed674058b8b216397a85eac922b
'http://deb.debian.org/debian/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.38.1+dfsg-1.debian.tar.xz' gdk-pixbuf_2.38.1+dfsg-1.debian.tar.xz 16792 SHA256:6340efafbdb7b270fe3dd94a0e5c929669f4f0324b9f13a4ef0f2c402253a36f
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdk-pixbuf/2.38.1+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/gdk-pixbuf/2.38.1+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdk-pixbuf/2.38.1+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ghostscript=9.27~dfsg-2+deb10u3`

Binary Packages:

- `ghostscript=9.27~dfsg-2+deb10u3`
- `libgs9:amd64=9.27~dfsg-2+deb10u3`
- `libgs9-common=9.27~dfsg-2+deb10u3`

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
$ apt-get source -qq --print-uris ghostscript=9.27~dfsg-2+deb10u3
'http://deb.debian.org/debian/pool/main/g/ghostscript/ghostscript_9.27~dfsg-2+deb10u3.dsc' ghostscript_9.27~dfsg-2+deb10u3.dsc 2950 SHA256:ef2614644c327c2b263145161ea713c86cf0df67b3617c336eb6bb89a6282184
'http://deb.debian.org/debian/pool/main/g/ghostscript/ghostscript_9.27~dfsg.orig.tar.xz' ghostscript_9.27~dfsg.orig.tar.xz 17723588 SHA256:b90d2117e93c63d774a5ab0a4d6a19c5dcbfd877462ee39a405262948e23ff9b
'http://deb.debian.org/debian/pool/main/g/ghostscript/ghostscript_9.27~dfsg-2+deb10u3.debian.tar.xz' ghostscript_9.27~dfsg-2+deb10u3.debian.tar.xz 113724 SHA256:23865ead29e57764e1aed005cf83ec3fdb68b7492d589dbd0eb9e54e1ea80a4b
```

Other potentially useful URLs:

- https://sources.debian.net/src/ghostscript/9.27~dfsg-2+deb10u3/ (for browsing the source)
- https://sources.debian.net/src/ghostscript/9.27~dfsg-2+deb10u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ghostscript/9.27~dfsg-2+deb10u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.20.1-2+deb10u1`

Binary Packages:

- `git=1:2.20.1-2+deb10u1`
- `git-man=1:2.20.1-2+deb10u1`

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
$ apt-get source -qq --print-uris git=1:2.20.1-2+deb10u1
'http://deb.debian.org/debian/pool/main/g/git/git_2.20.1-2+deb10u1.dsc' git_2.20.1-2+deb10u1.dsc 2923 SHA256:d019a11d3826d5dc1f004cfcfeaad392c22cbd86956bca53271252014b0bd874
'http://deb.debian.org/debian/pool/main/g/git/git_2.20.1.orig.tar.xz' git_2.20.1.orig.tar.xz 5359872 SHA256:9d2e91e2faa2ea61ba0a70201d023b36f54d846314591a002c610ea2ab81c3e9
'http://deb.debian.org/debian/pool/main/g/git/git_2.20.1-2+deb10u1.debian.tar.xz' git_2.20.1-2+deb10u1.debian.tar.xz 632804 SHA256:3fe13b0b41f04e9029d6f3e396a610ddf79271c285cc8b0b7f644b563b6f1368
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.20.1-2+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.20.1-2+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.20.1-2+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib-networking=2.58.0-2`

Binary Packages:

- `glib-networking:amd64=2.58.0-2`
- `glib-networking-common=2.58.0-2`
- `glib-networking-services=2.58.0-2`

Licenses: (parsed from: `/usr/share/doc/glib-networking/copyright`, `/usr/share/doc/glib-networking-common/copyright`, `/usr/share/doc/glib-networking-services/copyright`)

- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris glib-networking=2.58.0-2
'http://deb.debian.org/debian/pool/main/g/glib-networking/glib-networking_2.58.0-2.dsc' glib-networking_2.58.0-2.dsc 2485 SHA256:4065034cbe05ee0b80a7da465159fd9b4a9d9e4e0a366695da5c44bd591f20a2
'http://deb.debian.org/debian/pool/main/g/glib-networking/glib-networking_2.58.0.orig.tar.xz' glib-networking_2.58.0.orig.tar.xz 172632 SHA256:bdfa0255e031b8ee003cc283002536b77ee76450105f1dc6ab066b9bf4330068
'http://deb.debian.org/debian/pool/main/g/glib-networking/glib-networking_2.58.0-2.debian.tar.xz' glib-networking_2.58.0-2.debian.tar.xz 8520 SHA256:27faa08a5d4d0bec7e1d70bd5345dd2ca409f0662ef73a7de8bc8d1fe5b4752e
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib-networking/2.58.0-2/ (for browsing the source)
- https://sources.debian.net/src/glib-networking/2.58.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib-networking/2.58.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.58.3-2+deb10u2`

Binary Packages:

- `libglib2.0-0:amd64=2.58.3-2+deb10u2`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `Apache-2.0`
- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.58.3-2+deb10u2
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.58.3-2+deb10u2.dsc' glib2.0_2.58.3-2+deb10u2.dsc 3466 SHA256:585667486fca2f2a32c04670e1008c5e0ff0cd96024c8618a3e78ee546d85a12
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.58.3.orig.tar.xz' glib2.0_2.58.3.orig.tar.xz 4863648 SHA256:8f43c31767e88a25da72b52a40f3301fefc49a665b56dc10ee7cc9565cbe7481
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.58.3-2+deb10u2.debian.tar.xz' glib2.0_2.58.3-2+deb10u2.debian.tar.xz 93604 SHA256:c4c01644ec784f6b138441d2f8efbfe606d3a3154109d517bf6d8e89e150c57f
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.58.3-2+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.58.3-2+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.58.3-2+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.28-10`

Binary Packages:

- `libc-bin=2.28-10`
- `libc-l10n=2.28-10`
- `libc6:amd64=2.28-10`
- `locales=2.28-10`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-l10n/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/locales/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.28-10
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.28-10.dsc' glibc_2.28-10.dsc 8889 SHA256:9f21ef7002d51a32b46aafb9ca604427cf28c49495ecbf97e44740f53619ce69
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.28.orig.tar.xz' glibc_2.28.orig.tar.xz 17061292 SHA256:53d3c1c7bff0fb25d4c7874bf13435dc44a71fd7dd5ffc9bfdcb513cdfc36854
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.28-10.debian.tar.xz' glibc_2.28-10.debian.tar.xz 885796 SHA256:08ca414d8428a252ea357661631885ff72e47afa0663e3811167cc0897dbb042
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.28-10/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.28-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.28-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.1.2+dfsg-4`

Binary Packages:

- `libgmp10:amd64=2:6.1.2+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-4
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-4.dsc' gmp_6.1.2+dfsg-4.dsc 2123 SHA256:5e9c98e1636344bf0c84710ee564ee6032d6a9db26aa5d29857d65b2a979877c
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.1.2+dfsg-4.debian.tar.xz' gmp_6.1.2+dfsg-4.debian.tar.xz 21416 SHA256:cb25b080d915d9e5a641920f0471b4deb5368af739c7675d887cf290c2cffbe2
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-4/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.1.2+dfsg-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.1.2+dfsg-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.12-1+deb10u1`

Binary Packages:

- `dirmngr=2.2.12-1+deb10u1`
- `gnupg=2.2.12-1+deb10u1`
- `gnupg-l10n=2.2.12-1+deb10u1`
- `gnupg-utils=2.2.12-1+deb10u1`
- `gpg=2.2.12-1+deb10u1`
- `gpg-agent=2.2.12-1+deb10u1`
- `gpg-wks-client=2.2.12-1+deb10u1`
- `gpg-wks-server=2.2.12-1+deb10u1`
- `gpgconf=2.2.12-1+deb10u1`
- `gpgsm=2.2.12-1+deb10u1`
- `gpgv=2.2.12-1+deb10u1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.12-1+deb10u1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.12-1+deb10u1.dsc' gnupg2_2.2.12-1+deb10u1.dsc 3261 SHA256:2e1ca8d194593c151228f6b54da51ccd0b17036a532c7724bfcab17594c886ed
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.12.orig.tar.bz2' gnupg2_2.2.12.orig.tar.bz2 6682303 SHA256:db030f8b4c98640e91300d36d516f1f4f8fe09514a94ea9fc7411ee1a34082cb
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.12.orig.tar.bz2.asc' gnupg2_2.2.12.orig.tar.bz2.asc 3204 SHA256:97c8dc25c4c2fe9a39b2ffd81b65b6f3dc4ad359c9a81ca4bb9b4bdeb6167c60
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.12-1+deb10u1.debian.tar.xz' gnupg2_2.2.12-1+deb10u1.debian.tar.xz 123224 SHA256:f8cd4f8a2b63208fd05ae433dc9cb11d2483a72ef057cfe5fcfe2385b7c63f38
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.12-1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.12-1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.12-1+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.6.7-4+deb10u2`

Binary Packages:

- `libgnutls30:amd64=3.6.7-4+deb10u2`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `Apache-2.0`
- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `GPLv3+`
- `LGPL`
- `LGPL-3`
- `LGPLv3+_or_GPLv2+`
- `The MIT License (MIT)`
- `The main library is licensed under GNU Lesser`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.6.7-4+deb10u2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7-4+deb10u2.dsc' gnutls28_3.6.7-4+deb10u2.dsc 3354 SHA256:e7d5063186b5773fa91de22fa2ff34a13400a012cbd239b51d882971b2d9efca
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7.orig.tar.xz' gnutls28_3.6.7.orig.tar.xz 8153728 SHA256:5b3409ad5aaf239808730d1ee12fdcd148c0be00262c7edf157af655a8a188e2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7.orig.tar.xz.asc' gnutls28_3.6.7.orig.tar.xz.asc 534 SHA256:a14d0a7b9295b65ae797a70f8e765024a2e363dca03d008bfce0aec2b3f292b0
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7-4+deb10u2.debian.tar.xz' gnutls28_3.6.7-4+deb10u2.debian.tar.xz 77516 SHA256:72cd1e02b3b3c39c79f69da00a958d906d0332f15067d5c1b4e40bcd897a0d2e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.6.7-4+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.6.7-4+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.6.7-4+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gpac=0.5.2-426-gc5ad4e4+dfsg5-5`

Binary Packages:

- `libgpac4:amd64=0.5.2-426-gc5ad4e4+dfsg5-5`

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
$ apt-get source -qq --print-uris gpac=0.5.2-426-gc5ad4e4+dfsg5-5
'http://deb.debian.org/debian/pool/main/g/gpac/gpac_0.5.2-426-gc5ad4e4+dfsg5-5.dsc' gpac_0.5.2-426-gc5ad4e4+dfsg5-5.dsc 2707 SHA256:8d2584c04673ff9ca9b235d42bb3ce37caaaf71205d4bc1a5ca549bdaae6ed7a
'http://deb.debian.org/debian/pool/main/g/gpac/gpac_0.5.2-426-gc5ad4e4+dfsg5.orig.tar.xz' gpac_0.5.2-426-gc5ad4e4+dfsg5.orig.tar.xz 3607392 SHA256:964173b9fc2439daa0366951deed08f84235cc554b18e30a62197ba3afd35e00
'http://deb.debian.org/debian/pool/main/g/gpac/gpac_0.5.2-426-gc5ad4e4+dfsg5-5.debian.tar.xz' gpac_0.5.2-426-gc5ad4e4+dfsg5-5.debian.tar.xz 43692 SHA256:a827ba9c1fdc64ef9a04515e306cba8f614eafa2730b83eea3cf6a57cfbfcbd4
```

Other potentially useful URLs:

- https://sources.debian.net/src/gpac/0.5.2-426-gc5ad4e4+dfsg5-5/ (for browsing the source)
- https://sources.debian.net/src/gpac/0.5.2-426-gc5ad4e4+dfsg5-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gpac/0.5.2-426-gc5ad4e4+dfsg5-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gpgme1.0=1.12.0-6`

Binary Packages:

- `libgpgme11:amd64=1.12.0-6`
- `libgpgmepp6:amd64=1.12.0-6`

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
$ apt-get source -qq --print-uris gpgme1.0=1.12.0-6
'http://deb.debian.org/debian/pool/main/g/gpgme1.0/gpgme1.0_1.12.0-6.dsc' gpgme1.0_1.12.0-6.dsc 2634 SHA256:a6abc917763c8e6cbb25eb27712ce73eb5735e4ef5b0e2b1e7f6d75843e11c3a
'http://deb.debian.org/debian/pool/main/g/gpgme1.0/gpgme1.0_1.12.0.orig.tar.bz2' gpgme1.0_1.12.0.orig.tar.bz2 1658803 SHA256:b4dc951c3743a60e2e120a77892e9e864fb936b2e58e7c77e8581f4d050e8cd8
'http://deb.debian.org/debian/pool/main/g/gpgme1.0/gpgme1.0_1.12.0-6.debian.tar.xz' gpgme1.0_1.12.0-6.debian.tar.xz 22052 SHA256:bcdc1a899a63903aae88dbe842bdc29bfdeca7db20ec9d634d71cd31a1e396ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/gpgme1.0/1.12.0-6/ (for browsing the source)
- https://sources.debian.net/src/gpgme1.0/1.12.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gpgme1.0/1.12.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `graphite2=1.3.13-7`

Binary Packages:

- `libgraphite2-3:amd64=1.3.13-7`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-2.1+ `
- `MPL-1.1`
- `custom-sil-open-font-license`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.13-7
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.13-7.dsc' graphite2_1.3.13-7.dsc 2552 SHA256:0c646f75bfaee6b2447fc065dd3db3008c51896bfd3c1ff51919c14a34c6d831
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.13.orig.tar.gz' graphite2_1.3.13.orig.tar.gz 6664941 SHA256:2f9f609deeddfe2b193502adc8df3b0396694b799a433c36e85fd1242e654cd9
'http://deb.debian.org/debian/pool/main/g/graphite2/graphite2_1.3.13-7.debian.tar.xz' graphite2_1.3.13-7.debian.tar.xz 11972 SHA256:6577d43c7b40f8bcf4b18cb86284eec973029a341c1155754649557526304534
```

Other potentially useful URLs:

- https://sources.debian.net/src/graphite2/1.3.13-7/ (for browsing the source)
- https://sources.debian.net/src/graphite2/1.3.13-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/graphite2/1.3.13-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.3-1`

Binary Packages:

- `grep=3.3-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.3-1
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.3-1.dsc' grep_3.3-1.dsc 2038 SHA256:4a019e5634f0a3a15715140fe8639af4cff0f2f7af8cee9b95b0607740ba9b25
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.3.orig.tar.xz' grep_3.3.orig.tar.xz 1473056 SHA256:b960541c499619efd6afe1fa795402e4733c8e11ebf9fafccc0bb4bccdc5b514
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.3-1.debian.tar.xz' grep_3.3-1.debian.tar.xz 104280 SHA256:2cea85fdfe3c70855019c3d9ed9346363137bf3f9931103d9b38514828c8989f
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.3-1/ (for browsing the source)
- https://sources.debian.net/src/grep/3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gsettings-desktop-schemas=3.28.1-1`

Binary Packages:

- `gsettings-desktop-schemas=3.28.1-1`

Licenses: (parsed from: `/usr/share/doc/gsettings-desktop-schemas/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gsettings-desktop-schemas=3.28.1-1
'http://deb.debian.org/debian/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.28.1-1.dsc' gsettings-desktop-schemas_3.28.1-1.dsc 2525 SHA256:107b826809bface0b220cdc931882bf431baa394420ab40cb3e9f4af2941011c
'http://deb.debian.org/debian/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.28.1.orig.tar.xz' gsettings-desktop-schemas_3.28.1.orig.tar.xz 652416 SHA256:f88ea6849ffe897c51cfeca5e45c3890010c82c58be2aee18b01349648e5502f
'http://deb.debian.org/debian/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.28.1-1.debian.tar.xz' gsettings-desktop-schemas_3.28.1-1.debian.tar.xz 4816 SHA256:e3df9a8166d070ece3ba10ecf73bc434be911504a3902112ccbc8be92f814353
```

Other potentially useful URLs:

- https://sources.debian.net/src/gsettings-desktop-schemas/3.28.1-1/ (for browsing the source)
- https://sources.debian.net/src/gsettings-desktop-schemas/3.28.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gsettings-desktop-schemas/3.28.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gst-plugins-base1.0=1.14.4-2`

Binary Packages:

- `libgstreamer-plugins-base1.0-0:amd64=1.14.4-2`

Licenses: (parsed from: `/usr/share/doc/libgstreamer-plugins-base1.0-0/copyright`)

- `BSD (2 clause)`
- `BSD (3 clause)`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`
- `MIT/X11 (BSD like) LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gst-plugins-base1.0=1.14.4-2
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.4-2.dsc' gst-plugins-base1.0_1.14.4-2.dsc 4246 SHA256:7047d8cf6221f0ea01a885152e2fd9625e32b0d7e95c0fd65ae1f9b0dea78097
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.4.orig.tar.xz' gst-plugins-base1.0_1.14.4.orig.tar.xz 3703232 SHA256:ca6139490e48863e7706d870ff4e8ac9f417b56f3b9e4b3ce490c13b09a77461
'http://deb.debian.org/debian/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.4-2.debian.tar.xz' gst-plugins-base1.0_1.14.4-2.debian.tar.xz 45244 SHA256:587dc73d816fc44a6a1fbe8f0279df3be901831ddaf3d16d36852df37011ad19
```

Other potentially useful URLs:

- https://sources.debian.net/src/gst-plugins-base1.0/1.14.4-2/ (for browsing the source)
- https://sources.debian.net/src/gst-plugins-base1.0/1.14.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gst-plugins-base1.0/1.14.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gstreamer1.0=1.14.4-1`

Binary Packages:

- `libgstreamer1.0-0:amd64=1.14.4-1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer1.0-0/copyright`)

- `GPL-2+`
- `GPL-3+`
- `LGPL`
- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gstreamer1.0=1.14.4-1
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.4-1.dsc' gstreamer1.0_1.14.4-1.dsc 3147 SHA256:fd0be5c0c68c8ae26dca906c1c3e662b7303db1487ab1944dc5499dd07c895d3
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.4.orig.tar.xz' gstreamer1.0_1.14.4.orig.tar.xz 3264324 SHA256:f94f6696c5f05a3b3a9183e39c5f5c0b779f75a04c0efa497e7920afa985ffc7
'http://deb.debian.org/debian/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.4-1.debian.tar.xz' gstreamer1.0_1.14.4-1.debian.tar.xz 44476 SHA256:dd34311f959f07cfea7cb7c3fa2c45999ccb0e40fb36118497770425445c7f88
```

Other potentially useful URLs:

- https://sources.debian.net/src/gstreamer1.0/1.14.4-1/ (for browsing the source)
- https://sources.debian.net/src/gstreamer1.0/1.14.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gstreamer1.0/1.14.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gtk+2.0=2.24.32-3`

Binary Packages:

- `libgtk2.0-0:amd64=2.24.32-3`
- `libgtk2.0-common=2.24.32-3`

Licenses: (parsed from: `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

- `LGPL-2`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+2.0=2.24.32-3
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.32-3.dsc' gtk+2.0_2.24.32-3.dsc 3665 SHA256:3b477beb773081846fbfbffd1a33dabf9178496d4f884b94d51fad8bface2a17
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.32.orig.tar.xz' gtk+2.0_2.24.32.orig.tar.xz 12620860 SHA256:b6c8a93ddda5eabe3bfee1eb39636c9a03d2a56c7b62828b359bf197943c582e
'http://deb.debian.org/debian/pool/main/g/gtk+2.0/gtk+2.0_2.24.32-3.debian.tar.xz' gtk+2.0_2.24.32-3.debian.tar.xz 100080 SHA256:ca03b2b1287331d8909a8c0ecc4cd2f6a9d2772ccab4619aa03c353d4eb85333
```

Other potentially useful URLs:

- https://sources.debian.net/src/gtk+2.0/2.24.32-3/ (for browsing the source)
- https://sources.debian.net/src/gtk+2.0/2.24.32-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gtk+2.0/2.24.32-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gtk+3.0=3.24.5-1`

Binary Packages:

- `gtk-update-icon-cache=3.24.5-1`
- `libgtk-3-0:amd64=3.24.5-1`
- `libgtk-3-common=3.24.5-1`

Licenses: (parsed from: `/usr/share/doc/gtk-update-icon-cache/copyright`, `/usr/share/doc/libgtk-3-0/copyright`, `/usr/share/doc/libgtk-3-common/copyright`)

- `Apache-2.0`
- `Expat`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `SWL`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+3.0=3.24.5-1
'http://deb.debian.org/debian/pool/main/g/gtk+3.0/gtk+3.0_3.24.5-1.dsc' gtk+3.0_3.24.5-1.dsc 3770 SHA256:a2371939541fcfc1c0a5c4840905cd77e496680e22485aeb5b869d64da6367f8
'http://deb.debian.org/debian/pool/main/g/gtk+3.0/gtk+3.0_3.24.5.orig.tar.xz' gtk+3.0_3.24.5.orig.tar.xz 21012108 SHA256:0be5fb0d302bc3de26ab58c32990d895831e2b7c7418d0ffea1206d6a3ddb02f
'http://deb.debian.org/debian/pool/main/g/gtk+3.0/gtk+3.0_3.24.5-1.debian.tar.xz' gtk+3.0_3.24.5-1.debian.tar.xz 150544 SHA256:baafc391b16f16b7ced315b414a5e9e23b38a06966292e2b2a356614ac30db5f
```

Other potentially useful URLs:

- https://sources.debian.net/src/gtk+3.0/3.24.5-1/ (for browsing the source)
- https://sources.debian.net/src/gtk+3.0/3.24.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gtk+3.0/3.24.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gtkimageview=1.6.4+dfsg-2`

Binary Packages:

- `libgtkimageview0=1.6.4+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgtkimageview0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris gtkimageview=1.6.4+dfsg-2
'http://deb.debian.org/debian/pool/main/g/gtkimageview/gtkimageview_1.6.4+dfsg-2.dsc' gtkimageview_1.6.4+dfsg-2.dsc 1939 SHA256:af789b0b82e71072619b08841d2e86887e3005fd47549794d48d28a333bcbf31
'http://deb.debian.org/debian/pool/main/g/gtkimageview/gtkimageview_1.6.4+dfsg.orig.tar.gz' gtkimageview_1.6.4+dfsg.orig.tar.gz 1172925 SHA256:9336fe986658862ecf5abbc25a3d6dab12668c72b284d2f88b058d1abf4c5ef6
'http://deb.debian.org/debian/pool/main/g/gtkimageview/gtkimageview_1.6.4+dfsg-2.debian.tar.xz' gtkimageview_1.6.4+dfsg-2.debian.tar.xz 5476 SHA256:bd18fd43ad2531b734ad9863252e6e4a31cfb9ec3163eb5f5e62a491aa2b843e
```

Other potentially useful URLs:

- https://sources.debian.net/src/gtkimageview/1.6.4+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/gtkimageview/1.6.4+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gtkimageview/1.6.4+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.9-3`

Binary Packages:

- `gzip=1.9-3`

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

### `dpkg` source package: `harfbuzz=2.3.1-1`

Binary Packages:

- `libharfbuzz-icu0:amd64=2.3.1-1`
- `libharfbuzz0b:amd64=2.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz-icu0/copyright`, `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.3.1-1
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.3.1-1.dsc' harfbuzz_2.3.1-1.dsc 2298 SHA256:6d70022d4af66c44f7d225c21f656468304abaa3789e5a149dae8772816ba0a6
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.3.1.orig.tar.bz2' harfbuzz_2.3.1.orig.tar.bz2 17942960 SHA256:f205699d5b91374008d6f8e36c59e419ae2d9a7bb8c5d9f34041b9a5abcae468
'http://deb.debian.org/debian/pool/main/h/harfbuzz/harfbuzz_2.3.1-1.debian.tar.xz' harfbuzz_2.3.1-1.debian.tar.xz 9696 SHA256:aa4b07e617c0042c4346ef0fd1e58db4492cb7076583be1f0e9e394571e0d270
```

Other potentially useful URLs:

- https://sources.debian.net/src/harfbuzz/2.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/harfbuzz/2.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/harfbuzz/2.3.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `hostname=3.21`

Binary Packages:

- `hostname=3.21`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.21
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.21.dsc' hostname_3.21.dsc 1398 SHA256:8e61f35d7b3e57833d6110ee22a95af6b12e159bf41a5b659e63b21d01e83121
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.21.tar.gz' hostname_3.21.tar.gz 13467 SHA256:566193a99f97a58f80b1537efe207c798bb88436c31c7dfc6dd4471d888a4a4f
```

Other potentially useful URLs:

- https://sources.debian.net/src/hostname/3.21/ (for browsing the source)
- https://sources.debian.net/src/hostname/3.21/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hostname/3.21/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `hunspell=1.7.0-2`

Binary Packages:

- `libhunspell-1.7-0:amd64=1.7.0-2`

Licenses: (parsed from: `/usr/share/doc/libhunspell-1.7-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris hunspell=1.7.0-2
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.7.0-2.dsc' hunspell_1.7.0-2.dsc 2238 SHA256:0f51c582657cb4c7bc2224a3ed2a90edab723368ceb53b0a0c9d218d7ef2b3f9
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.7.0.orig.tar.gz' hunspell_1.7.0.orig.tar.gz 482156 SHA256:bb27b86eb910a8285407cf3ca33b62643a02798cf2eef468c0a74f6c3ee6bc8a
'http://deb.debian.org/debian/pool/main/h/hunspell/hunspell_1.7.0-2.debian.tar.xz' hunspell_1.7.0-2.debian.tar.xz 21600 SHA256:46b74797ebda002e5dbca8a0d9f0b0ab1a7e56fe08b51d8f1d9c62d186654e44
```

Other potentially useful URLs:

- https://sources.debian.net/src/hunspell/1.7.0-2/ (for browsing the source)
- https://sources.debian.net/src/hunspell/1.7.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hunspell/1.7.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `icu=63.1-6`

Binary Packages:

- `libicu63:amd64=63.1-6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=63.1-6
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.1-6.dsc' icu_63.1-6.dsc 1965 SHA256:dfb3387f8e80c7de6704967694cf74ef7dd407c562b8cc7653156308e924404f
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.1.orig.tar.xz' icu_63.1.orig.tar.xz 13638120 SHA256:347d0e6c39c3538b812c10c6c83815d4a089d578380387ae7d94c5b820948e82
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.1-6.debian.tar.xz' icu_63.1-6.debian.tar.xz 24624 SHA256:c63fc607cb6420136d78f706baf17b7ca68346386e82ca4f30dacc81e1e56681
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/63.1-6/ (for browsing the source)
- https://sources.debian.net/src/icu/63.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/63.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ijs=0.35-14`

Binary Packages:

- `libijs-0.35:amd64=0.35-14`

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
$ apt-get source -qq --print-uris ijs=0.35-14
'http://deb.debian.org/debian/pool/main/i/ijs/ijs_0.35-14.dsc' ijs_0.35-14.dsc 2084 SHA256:20971c4a08fbbda83e132eb640bab003e3cf62b7284d6e2dadb286ad6d790d6a
'http://deb.debian.org/debian/pool/main/i/ijs/ijs_0.35.orig.tar.gz' ijs_0.35.orig.tar.gz 344262 SHA256:901fffb73e42dae343a8285a31d9c4e82dc3856d36be30adbdb564bdd27161d6
'http://deb.debian.org/debian/pool/main/i/ijs/ijs_0.35-14.debian.tar.xz' ijs_0.35-14.debian.tar.xz 8464 SHA256:e7206b52f2bb5979776e3f10927270b3c3949ce7485089835a251648043de5dc
```

Other potentially useful URLs:

- https://sources.debian.net/src/ijs/0.35-14/ (for browsing the source)
- https://sources.debian.net/src/ijs/0.35-14/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ijs/0.35-14/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1`

Binary Packages:

- `imagemagick=8:6.9.10.23+dfsg-2.1`
- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1`
- `imagemagick-6.q16=8:6.9.10.23+dfsg-2.1`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/libmagickcore-6.q16-6/copyright`, `/usr/share/doc/libmagickwand-6.q16-6/copyright`)

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

### `dpkg` source package: `init-system-helpers=1.56+nmu1`

Binary Packages:

- `init-system-helpers=1.56+nmu1`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.56+nmu1
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.56+nmu1.dsc' init-system-helpers_1.56+nmu1.dsc 1945 SHA256:96f7d1c696faf801eb5990223b2782dedaf4092efb9b0dcc13d038b91dbb1a51
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.56+nmu1.tar.xz' init-system-helpers_1.56+nmu1.tar.xz 40488 SHA256:ecb5b9a0dbf0b7e83ef41bfc15bf9d41868642d4d5f817a0962aa1b980a56368
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.56+nmu1/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.56+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.56+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iproute2=4.20.0-2`

Binary Packages:

- `iproute2=4.20.0-2`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris iproute2=4.20.0-2
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_4.20.0-2.dsc' iproute2_4.20.0-2.dsc 1884 SHA256:006d839d17b2871c8e8b655782b59311b2b56ed883760011173bb4df2da1a0fb
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_4.20.0.orig.tar.xz' iproute2_4.20.0.orig.tar.xz 707016 SHA256:c8adaa6a40f888476b23acb283cfa30c0dd55f07b5aa20663ed5ba2ef1f6fda8
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_4.20.0-2.debian.tar.xz' iproute2_4.20.0-2.debian.tar.xz 144416 SHA256:32220902a0bfdae209ffa7aee610cd70d49c759eeada1d9008b84782d1515e00
```

Other potentially useful URLs:

- https://sources.debian.net/src/iproute2/4.20.0-2/ (for browsing the source)
- https://sources.debian.net/src/iproute2/4.20.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iproute2/4.20.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iptables=1.8.2-4`

Binary Packages:

- `libip4tc0:amd64=1.8.2-4`
- `libxtables12:amd64=1.8.2-4`

Licenses: (parsed from: `/usr/share/doc/libip4tc0/copyright`, `/usr/share/doc/libxtables12/copyright`)

- `Artistic-2`
- `GPL-2`
- `GPL-2+`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris iptables=1.8.2-4
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.2-4.dsc' iptables_1.8.2-4.dsc 2699 SHA256:926c91a00c449d7999e5d86e7471ea0591d8fd6633aca3649925aa2fea04273a
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.2.orig.tar.bz2' iptables_1.8.2.orig.tar.bz2 679858 SHA256:a3778b50ed1a3256f9ca975de82c2204e508001fc2471238c8c97f3d1c4c12af
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.2-4.debian.tar.xz' iptables_1.8.2-4.debian.tar.xz 65300 SHA256:e6562e368ed7bff8378c1a31ca0d283f15be3a4c68165786dfaa38cc5e9e9e09
```

Other potentially useful URLs:

- https://sources.debian.net/src/iptables/1.8.2-4/ (for browsing the source)
- https://sources.debian.net/src/iptables/1.8.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iptables/1.8.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iputils=3:20180629-2`

Binary Packages:

- `iputils-ping=3:20180629-2`

Licenses: (parsed from: `/usr/share/doc/iputils-ping/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris iputils=3:20180629-2
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20180629-2.dsc' iputils_20180629-2.dsc 2093 SHA256:c377186ea16ebeb404316f562857e2564e3346b7b0cfd9ef72d88498db6bf3b0
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20180629.orig.tar.bz2' iputils_20180629.orig.tar.bz2 157943 SHA256:1a54fe72d67ac00dae328ddb1952110ee5310ccecbfcb97cbb26d4dedc73fe6d
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20180629-2.debian.tar.xz' iputils_20180629-2.debian.tar.xz 10212 SHA256:bccf6d3819bbcea59ecade34872fb44f30495baa4878cc32b2ec32b973a7ac58
```

Other potentially useful URLs:

- https://sources.debian.net/src/iputils/3:20180629-2/ (for browsing the source)
- https://sources.debian.net/src/iputils/3:20180629-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iputils/3:20180629-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iso-codes=4.2-1`

Binary Packages:

- `iso-codes=4.2-1`

Licenses: (parsed from: `/usr/share/doc/iso-codes/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris iso-codes=4.2-1
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_4.2-1.dsc' iso-codes_4.2-1.dsc 1970 SHA256:d0b4026a19fbf7df0db41bdc095d38765ccb12416e66a754de965e067b425276
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_4.2.orig.tar.xz' iso-codes_4.2.orig.tar.xz 3604904 SHA256:2b7f66c81808ac52e1ed0efe4ce8ae8e43309eedcc411f94f71a3f603cc21f42
'http://deb.debian.org/debian/pool/main/i/iso-codes/iso-codes_4.2-1.debian.tar.xz' iso-codes_4.2-1.debian.tar.xz 23800 SHA256:e6c6caaaa6392e7f9653e4f056e1f24b5875f063c8b3a2509221e36ea2d0a74a
```

Other potentially useful URLs:

- https://sources.debian.net/src/iso-codes/4.2-1/ (for browsing the source)
- https://sources.debian.net/src/iso-codes/4.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iso-codes/4.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jackd2=1.9.12~dfsg-2`

Binary Packages:

- `libjack-jackd2-0:amd64=1.9.12~dfsg-2`

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
$ apt-get source -qq --print-uris jackd2=1.9.12~dfsg-2
'http://deb.debian.org/debian/pool/main/j/jackd2/jackd2_1.9.12~dfsg-2.dsc' jackd2_1.9.12~dfsg-2.dsc 2521 SHA256:7378eb1f223f0b69b8698f4a09e59c7f26632c1f2dec0452a76ea80ca5798d9a
'http://deb.debian.org/debian/pool/main/j/jackd2/jackd2_1.9.12~dfsg.orig.tar.gz' jackd2_1.9.12~dfsg.orig.tar.gz 1147874 SHA256:059741090d548d1888d34c90647e3ac1650bbee84990dceffcb5144b8f8cd539
'http://deb.debian.org/debian/pool/main/j/jackd2/jackd2_1.9.12~dfsg-2.debian.tar.xz' jackd2_1.9.12~dfsg-2.debian.tar.xz 44324 SHA256:59904fbdc98a3404bd5f21af13bd24977d2e5b03600f2bb0a84127a1bc69aeb9
```

Other potentially useful URLs:

- https://sources.debian.net/src/jackd2/1.9.12~dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/jackd2/1.9.12~dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jackd2/1.9.12~dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `jbig2dec=0.16-1`

Binary Packages:

- `libjbig2dec0:amd64=0.16-1`

Licenses: (parsed from: `/usr/share/doc/libjbig2dec0/copyright`)

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
$ apt-get source -qq --print-uris jbig2dec=0.16-1
'http://deb.debian.org/debian/pool/main/j/jbig2dec/jbig2dec_0.16-1.dsc' jbig2dec_0.16-1.dsc 2086 SHA256:66b01f7ce378fa3a6d4bded07e86d37e41b9f914e2e43902fe765f1ad2090af9
'http://deb.debian.org/debian/pool/main/j/jbig2dec/jbig2dec_0.16.orig.tar.gz' jbig2dec_0.16.orig.tar.gz 140155 SHA256:30f706a67604237ffffaece96ae20ee86b2cfebd6277a95f8b0f2ab0f8859850
'http://deb.debian.org/debian/pool/main/j/jbig2dec/jbig2dec_0.16-1.debian.tar.xz' jbig2dec_0.16-1.debian.tar.xz 19620 SHA256:df58d52d65ff4860d1cd9d37eaeed3857f71db5184aa1116a6a910a6bfb53ded
```

Other potentially useful URLs:

- https://sources.debian.net/src/jbig2dec/0.16-1/ (for browsing the source)
- https://sources.debian.net/src/jbig2dec/0.16-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/jbig2dec/0.16-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `json-c=0.12.1+ds-2`

Binary Packages:

- `libjson-c3:amd64=0.12.1+ds-2`

Licenses: (parsed from: `/usr/share/doc/libjson-c3/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris json-c=0.12.1+ds-2
'http://deb.debian.org/debian/pool/main/j/json-c/json-c_0.12.1+ds-2.dsc' json-c_0.12.1+ds-2.dsc 2040 SHA256:933ae6adbb96b30cf98dadbdc03585b5910f9eb147d3dbfa719a8a57f613e884
'http://deb.debian.org/debian/pool/main/j/json-c/json-c_0.12.1+ds.orig.tar.gz' json-c_0.12.1+ds.orig.tar.gz 477598 SHA256:d036d20b63cb17ff02f43b86840f6c8c8da2b99077700c1779b16379cebb788d
'http://deb.debian.org/debian/pool/main/j/json-c/json-c_0.12.1+ds-2.debian.tar.xz' json-c_0.12.1+ds-2.debian.tar.xz 7132 SHA256:54c1434412f6e835f597320b7187a1bdf16f36f22ba2b47a872662fc0854c0c0
```

Other potentially useful URLs:

- https://sources.debian.net/src/json-c/0.12.1+ds-2/ (for browsing the source)
- https://sources.debian.net/src/json-c/0.12.1+ds-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/json-c/0.12.1+ds-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `json-glib=1.4.4-2`

Binary Packages:

- `libjson-glib-1.0-0:amd64=1.4.4-2`
- `libjson-glib-1.0-common=1.4.4-2`

Licenses: (parsed from: `/usr/share/doc/libjson-glib-1.0-0/copyright`, `/usr/share/doc/libjson-glib-1.0-common/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris json-glib=1.4.4-2
'http://deb.debian.org/debian/pool/main/j/json-glib/json-glib_1.4.4-2.dsc' json-glib_1.4.4-2.dsc 2662 SHA256:ea843d6fd7559be1df3b525074777ae7b32351f7cb29d404e287a7c4f9aaa3b3
'http://deb.debian.org/debian/pool/main/j/json-glib/json-glib_1.4.4.orig.tar.xz' json-glib_1.4.4.orig.tar.xz 150440 SHA256:d37052132c7fd2f12bda8f2a4d6829b6de36378772195920cccfdda2e0ef5ad7
'http://deb.debian.org/debian/pool/main/j/json-glib/json-glib_1.4.4-2.debian.tar.xz' json-glib_1.4.4-2.debian.tar.xz 7108 SHA256:9d9531480c9b38a82ac58e5f757045001b68f3d21db58e0df8d6775295292923
```

Other potentially useful URLs:

- https://sources.debian.net/src/json-glib/1.4.4-2/ (for browsing the source)
- https://sources.debian.net/src/json-glib/1.4.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/json-glib/1.4.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `keyutils=1.6-6`

Binary Packages:

- `libkeyutils1:amd64=1.6-6`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6-6
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6-6.dsc' keyutils_1.6-6.dsc 2062 SHA256:1da6a0f50759b4eefe210e351558a854e28d312213d5528792af6938f106f183
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.orig.tar.bz2' keyutils_1.6.orig.tar.bz2 93973 SHA256:d3aef20cec0005c0fa6b4be40079885567473185b1a57b629b030e67942c7115
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6-6.debian.tar.xz' keyutils_1.6-6.debian.tar.xz 12828 SHA256:063876d3733337aad5e632b013bb8fd85bef85b2285ba7d6c8ab5ac7492ca245
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.6-6/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.6-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.6-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `kmod=26-1`

Binary Packages:

- `libkmod2:amd64=26-1`

Licenses: (parsed from: `/usr/share/doc/libkmod2/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris kmod=26-1
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_26-1.dsc' kmod_26-1.dsc 1811 SHA256:6da1eb15c3c5e3dcf670cd717d0c1d779f26d787aadba5f1869a326343aa9d39
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_26.orig.tar.gz' kmod_26.orig.tar.gz 618292 SHA256:f28bc40ead548dce4a8e956fccfc36fd80f2b40884d270b812f1bfbd886e858c
'http://deb.debian.org/debian/pool/main/k/kmod/kmod_26-1.debian.tar.xz' kmod_26-1.debian.tar.xz 8360 SHA256:d009055ab96a856f5d6fcbb73432527e32141fe6f46220206484cce3c3c7cef5
```

Other potentially useful URLs:

- https://sources.debian.net/src/kmod/26-1/ (for browsing the source)
- https://sources.debian.net/src/kmod/26-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/kmod/26-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.17-3`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.17-3`
- `libk5crypto3:amd64=1.17-3`
- `libkrb5-3:amd64=1.17-3`
- `libkrb5support0:amd64=1.17-3`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-3
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.17-3.dsc' krb5_1.17-3.dsc 3302 SHA256:56112c60a10a49126359478893d2f51cee5513e41f6ec7269360c7abe8850f3f
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA256:5a6e2284a53de5702d3dc2be3b9339c963f9b5397d3fbbc53beb249380a781f5
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.17-3.debian.tar.xz' krb5_1.17-3.debian.tar.xz 99396 SHA256:35da9d221e3a29c57c38c9d326d625a5b9199f3d7d64983483bd82f871083c9f
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.17-3/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.17-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.17-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lame=3.100-2`

Binary Packages:

- `libmp3lame0:amd64=3.100-2+b1`

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
$ apt-get source -qq --print-uris lame=3.100-2
'http://deb.debian.org/debian/pool/main/l/lame/lame_3.100-2.dsc' lame_3.100-2.dsc 2193 SHA256:23ead7cb4e1e0dd7925e67f935d005aa2ae73b508d240420e63d87b99c5a952e
'http://deb.debian.org/debian/pool/main/l/lame/lame_3.100.orig.tar.gz' lame_3.100.orig.tar.gz 1524133 SHA256:ddfe36cab873794038ae2c1210557ad34857a4b6bdc515785d1da9e175b1da1e
'http://deb.debian.org/debian/pool/main/l/lame/lame_3.100-2.debian.tar.xz' lame_3.100-2.debian.tar.xz 12152 SHA256:096925e4c15a9ee4e3f79451111b0ad11ea33a4ab9b74581e6f4775b7f1867e5
```

Other potentially useful URLs:

- https://sources.debian.net/src/lame/3.100-2/ (for browsing the source)
- https://sources.debian.net/src/lame/3.100-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lame/3.100-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lapack=3.8.0-2`

Binary Packages:

- `libblas3:amd64=3.8.0-2`
- `liblapack3:amd64=3.8.0-2`

Licenses: (parsed from: `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.8.0-2
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.8.0-2.dsc' lapack_3.8.0-2.dsc 2776 SHA256:8cf38ceb9d86e1c51cbf213da566d1415eb040fa94aceefa5df86b4a6488dc6c
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.8.0.orig.tar.gz' lapack_3.8.0.orig.tar.gz 7426094 SHA256:deb22cc4a6120bff72621155a9917f485f96ef8319ac074a7afbc68aab88bcf6
'http://deb.debian.org/debian/pool/main/l/lapack/lapack_3.8.0-2.debian.tar.xz' lapack_3.8.0-2.debian.tar.xz 21076 SHA256:ac34773cb9f3f8b9659062fc5b6fd68790acc0b93e9bb0cac8a622cf409451c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/lapack/3.8.0-2/ (for browsing the source)
- https://sources.debian.net/src/lapack/3.8.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lapack/3.8.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lcms2=2.9-3`

Binary Packages:

- `liblcms2-2:amd64=2.9-3`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.9-3
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.9-3.dsc' lcms2_2.9-3.dsc 1956 SHA256:2529e211246393053d2f1567f067f9983facf086185b582a56d10ecf04f9ca80
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.9.orig.tar.gz' lcms2_2.9.orig.tar.gz 10974649 SHA256:48c6fdf98396fa245ed86e622028caf49b96fa22f3e5734f853f806fbc8e7d20
'http://deb.debian.org/debian/pool/main/l/lcms2/lcms2_2.9-3.debian.tar.xz' lcms2_2.9-3.debian.tar.xz 10580 SHA256:5916773a94edbfac06c36c95d8c6b7e8dc304cecb91897f84575f51f22663744
```

Other potentially useful URLs:

- https://sources.debian.net/src/lcms2/2.9-3/ (for browsing the source)
- https://sources.debian.net/src/lcms2/2.9-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lcms2/2.9-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lensfun=0.3.2-4`

Binary Packages:

- `liblensfun-data-v1=0.3.2-4`
- `liblensfun1:amd64=0.3.2-4`

Licenses: (parsed from: `/usr/share/doc/liblensfun-data-v1/copyright`, `/usr/share/doc/liblensfun1/copyright`)

- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris lensfun=0.3.2-4
'http://deb.debian.org/debian/pool/main/l/lensfun/lensfun_0.3.2-4.dsc' lensfun_0.3.2-4.dsc 2365 SHA256:b2fb7f14b7e04058baeda8fd1036434fa2ca66fc28714b8c3246fcdc8a075036
'http://deb.debian.org/debian/pool/main/l/lensfun/lensfun_0.3.2.orig.tar.gz' lensfun_0.3.2.orig.tar.gz 784825 SHA256:ae8bcad46614ca47f5bda65b00af4a257a9564a61725df9c74cb260da544d331
'http://deb.debian.org/debian/pool/main/l/lensfun/lensfun_0.3.2-4.debian.tar.xz' lensfun_0.3.2-4.debian.tar.xz 13156 SHA256:b788de19d28f91ff47a6cf2eb6c4f2c326c7389c59aefcad9a4cb2f004d7cea0
```

Other potentially useful URLs:

- https://sources.debian.net/src/lensfun/0.3.2-4/ (for browsing the source)
- https://sources.debian.net/src/lensfun/0.3.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lensfun/0.3.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libabw=0.1.2-1`

Binary Packages:

- `libabw-0.1-1:amd64=0.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libabw-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3 | LGPL-3`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libabw=0.1.2-1
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.2-1.dsc' libabw_0.1.2-1.dsc 1963 SHA256:0cdb89e4377a89c737edc90926e03e3e5f5d69905a0b5c3bfed1e6244c08a7e7
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.2.orig.tar.xz' libabw_0.1.2.orig.tar.xz 318400 SHA256:0b72944d5af81dda0a5c5803ee84cbac4b81441a4d767aa57029adc6744c2485
'http://deb.debian.org/debian/pool/main/liba/libabw/libabw_0.1.2-1.debian.tar.xz' libabw_0.1.2-1.debian.tar.xz 12984 SHA256:11a5263535ca3283857bcfe2911c5d71472909f130b4cb8efd044afa4ba0ab4d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libabw/0.1.2-1/ (for browsing the source)
- https://sources.debian.net/src/libabw/0.1.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libabw/0.1.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libass=1:0.14.0-2`

Binary Packages:

- `libass9:amd64=1:0.14.0-2`

Licenses: (parsed from: `/usr/share/doc/libass9/copyright`)

- `GPL-2`
- `GPL-2+`
- `ISC`
- `other-1`

Source:

```console
$ apt-get source -qq --print-uris libass=1:0.14.0-2
'http://deb.debian.org/debian/pool/main/liba/libass/libass_0.14.0-2.dsc' libass_0.14.0-2.dsc 2093 SHA256:efa8465d4acb8352fdb53b503b90076704b1930286ec1f339aaf5b2045316479
'http://deb.debian.org/debian/pool/main/liba/libass/libass_0.14.0.orig.tar.xz' libass_0.14.0.orig.tar.xz 356256 SHA256:881f2382af48aead75b7a0e02e65d88c5ebd369fe46bc77d9270a94aa8fd38a2
'http://deb.debian.org/debian/pool/main/liba/libass/libass_0.14.0-2.debian.tar.xz' libass_0.14.0-2.debian.tar.xz 5804 SHA256:f585191f54caf8ddf1608458b4146e62472e4f5713416eea7a48ae1c5647abed
```

Other potentially useful URLs:

- https://sources.debian.net/src/libass/1:0.14.0-2/ (for browsing the source)
- https://sources.debian.net/src/libass/1:0.14.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libass/1:0.14.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libassuan=2.5.2-1`

Binary Packages:

- `libassuan0:amd64=2.5.2-1`

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
$ apt-get source -qq --print-uris libassuan=2.5.2-1
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.2-1.dsc' libassuan_2.5.2-1.dsc 1925 SHA256:534810315ca014673a3cc55a63e393ac02c434a4c51d0aff85c7edbcd60fb6e2
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.2.orig.tar.bz2' libassuan_2.5.2.orig.tar.bz2 570676 SHA256:986b1bf277e375f7a960450fbb8ffbd45294d06598916ad4ebf79aee0cb788e7
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.2.orig.tar.bz2.asc' libassuan_2.5.2.orig.tar.bz2.asc 1602 SHA256:b518440a68e4a1177f48c75637d9b4016f1a7c4bc46b820dda120a2d63af77ed
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.2-1.debian.tar.xz' libassuan_2.5.2-1.debian.tar.xz 11168 SHA256:69c1a189a718b289150cd194b9f558d8b2d190e371c6451e26a89b213f4b54f2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.2-1/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libavc1394=0.5.4-5`

Binary Packages:

- `libavc1394-0:amd64=0.5.4-5`

Licenses: (parsed from: `/usr/share/doc/libavc1394-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libavc1394=0.5.4-5
'http://deb.debian.org/debian/pool/main/liba/libavc1394/libavc1394_0.5.4-5.dsc' libavc1394_0.5.4-5.dsc 2122 SHA256:9faa03aa953eecfa46bc4fc98f7c8c2265a1d8cf0b26f04137e196e68b5f2176
'http://deb.debian.org/debian/pool/main/liba/libavc1394/libavc1394_0.5.4.orig.tar.gz' libavc1394_0.5.4.orig.tar.gz 341679 SHA256:7cb1ff09506ae911ca9860bef4af08c2403f3e131f6c913a2cbd6ddca4215b53
'http://deb.debian.org/debian/pool/main/liba/libavc1394/libavc1394_0.5.4-5.debian.tar.xz' libavc1394_0.5.4-5.debian.tar.xz 6600 SHA256:783dde153ec5287c8ca278e0911163ecf4c568f95ac0a9c49307fdd941659ff1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libavc1394/0.5.4-5/ (for browsing the source)
- https://sources.debian.net/src/libavc1394/0.5.4-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libavc1394/0.5.4-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbluray=1:1.1.0-1`

Binary Packages:

- `libbluray2:amd64=1:1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libbluray2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.0`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris libbluray=1:1.1.0-1
'http://deb.debian.org/debian/pool/main/libb/libbluray/libbluray_1.1.0-1.dsc' libbluray_1.1.0-1.dsc 2444 SHA256:03dce6e9249dd297df3f2fdba15ff4d9a3dee4635aec3d9c11e7dedbf7e7ae19
'http://deb.debian.org/debian/pool/main/libb/libbluray/libbluray_1.1.0.orig.tar.bz2' libbluray_1.1.0.orig.tar.bz2 742368 SHA256:e6a600d26ad3453a168dbb144f041134e954b541b44a9a5aa213d1c7d8c3fe83
'http://deb.debian.org/debian/pool/main/libb/libbluray/libbluray_1.1.0-1.debian.tar.xz' libbluray_1.1.0-1.debian.tar.xz 17240 SHA256:8e40078757743d0847fb4a16a63896987d07296182a6e5e3d51879ea7a0621fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbluray/1:1.1.0-1/ (for browsing the source)
- https://sources.debian.net/src/libbluray/1:1.1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbluray/1:1.1.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libbsd=0.9.1-2`

Binary Packages:

- `libbsd0:amd64=0.9.1-2`

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
$ apt-get source -qq --print-uris libbsd=0.9.1-2
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1-2.dsc' libbsd_0.9.1-2.dsc 2181 SHA256:abbba409f21d592c0232eab2641fb3f3181702ce0dce00a5357805d5b2d07d18
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1.orig.tar.xz' libbsd_0.9.1.orig.tar.xz 387180 SHA256:56d835742327d69faccd16955a60b6dcf30684a8da518c4eca0ac713b9e0a7a4
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1.orig.tar.xz.asc' libbsd_0.9.1.orig.tar.xz.asc 833 SHA256:a34a81f40bfef37242943cb1c4c446e75d57f31be3317c887d8a5f2cbfb5577d
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.9.1-2.debian.tar.xz' libbsd_0.9.1-2.debian.tar.xz 16456 SHA256:87c37138ffc1f3dc9fcc1a1a0486d87834c71b6ccce255cda7beb1d8ed5e9a65
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.9.1-2/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.9.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.9.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcaca=0.99.beta19-2.1`

Binary Packages:

- `libcaca0:amd64=0.99.beta19-2.1`

Licenses: (parsed from: `/usr/share/doc/libcaca0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcaca=0.99.beta19-2.1
'http://deb.debian.org/debian/pool/main/libc/libcaca/libcaca_0.99.beta19-2.1.dsc' libcaca_0.99.beta19-2.1.dsc 2224 SHA256:952f7ad2716b6c227597298ffc7d37b0ce199e18b58a5a810019473299e72b99
'http://deb.debian.org/debian/pool/main/libc/libcaca/libcaca_0.99.beta19.orig.tar.gz' libcaca_0.99.beta19.orig.tar.gz 1203495 SHA256:128b467c4ed03264c187405172a4e83049342cc8cc2f655f53a2d0ee9d3772f4
'http://deb.debian.org/debian/pool/main/libc/libcaca/libcaca_0.99.beta19-2.1.debian.tar.xz' libcaca_0.99.beta19-2.1.debian.tar.xz 12624 SHA256:7e2e265972d56c9aeb46686378a25543c6a3d2810cc1649102884dbe9aaf947a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcaca/0.99.beta19-2.1/ (for browsing the source)
- https://sources.debian.net/src/libcaca/0.99.beta19-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcaca/0.99.beta19-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.7.9-2`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.dsc' libcap-ng_0.7.9-2.dsc 1912 SHA256:e787ebb86a7c9fdcfe429c20f2b17528d084917a34b5efc0022619e1e11572a4
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.debian.tar.xz' libcap-ng_0.7.9-2.debian.tar.xz 6220 SHA256:1ce4d5f7ee041b01f254e9d12ae86fef563566871bc457579c70b058b071ae22
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap-ng/0.7.9-2/ (for browsing the source)
- https://sources.debian.net/src/libcap-ng/0.7.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap-ng/0.7.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap2=1:2.25-2`

Binary Packages:

- `libcap2:amd64=1:2.25-2`
- `libcap2-bin=1:2.25-2`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.25-2
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25-2.dsc' libcap2_2.25-2.dsc 2196 SHA256:28adc8b721b5a3151afdddc2081149473ec07f362777e25bfc29b3b96ec432f8
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25.orig.tar.xz' libcap2_2.25.orig.tar.xz 63672 SHA256:693c8ac51e983ee678205571ef272439d83afe62dd8e424ea14ad9790bc35162
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.25-2.debian.tar.xz' libcap2_2.25-2.debian.tar.xz 24876 SHA256:2581cdcaa27cf7e50b8e9f402a8b35ebbf78dd2697fb96bf78f411cd11110a82
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.25-2/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.25-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.25-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcdio-paranoia=10.2+0.94+2-4`

Binary Packages:

- `libcdio-cdda2:amd64=10.2+0.94+2-4`
- `libcdio-paranoia2:amd64=10.2+0.94+2-4`

Licenses: (parsed from: `/usr/share/doc/libcdio-cdda2/copyright`, `/usr/share/doc/libcdio-paranoia2/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libcdio-paranoia=10.2+0.94+2-4
'http://deb.debian.org/debian/pool/main/libc/libcdio-paranoia/libcdio-paranoia_10.2+0.94+2-4.dsc' libcdio-paranoia_10.2+0.94+2-4.dsc 2167 SHA256:65c0b89f6919d6ce6306278d2c32f23bd4ab51a960d14474b624814dbdf9091e
'http://deb.debian.org/debian/pool/main/libc/libcdio-paranoia/libcdio-paranoia_10.2+0.94+2.orig.tar.gz' libcdio-paranoia_10.2+0.94+2.orig.tar.gz 704560 SHA256:d60f82ece97eeb92407a9ee03f3499c8983206672c28ae5e4e22179063c81941
'http://deb.debian.org/debian/pool/main/libc/libcdio-paranoia/libcdio-paranoia_10.2+0.94+2-4.debian.tar.xz' libcdio-paranoia_10.2+0.94+2-4.debian.tar.xz 7948 SHA256:e27d5075f97016ee0aaf0b5c29c0573614c9e4d4db65d217650bab5fe6081934
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcdio-paranoia/10.2+0.94+2-4/ (for browsing the source)
- https://sources.debian.net/src/libcdio-paranoia/10.2+0.94+2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcdio-paranoia/10.2+0.94+2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcdio=2.0.0-2`

Binary Packages:

- `libcdio18:amd64=2.0.0-2`

Licenses: (parsed from: `/usr/share/doc/libcdio18/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libcdio=2.0.0-2
'http://deb.debian.org/debian/pool/main/libc/libcdio/libcdio_2.0.0-2.dsc' libcdio_2.0.0-2.dsc 2179 SHA256:721d1c3da7cbe5aa350676318c5ee7dd39f2f3317f7fb5d0dd60d1c659d72364
'http://deb.debian.org/debian/pool/main/libc/libcdio/libcdio_2.0.0.orig.tar.gz' libcdio_2.0.0.orig.tar.gz 2354813 SHA256:1b481b5da009bea31db875805665974e2fc568e2b2afa516f4036733657cf958
'http://deb.debian.org/debian/pool/main/libc/libcdio/libcdio_2.0.0-2.debian.tar.xz' libcdio_2.0.0-2.debian.tar.xz 10732 SHA256:d49483d113cdc36dd7d556f3fcfaeeef6f77e3381d459eb71d68be5bd08a30f6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcdio/2.0.0-2/ (for browsing the source)
- https://sources.debian.net/src/libcdio/2.0.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcdio/2.0.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcdr=0.1.5-1`

Binary Packages:

- `libcdr-0.1-1:amd64=0.1.5-1`

Licenses: (parsed from: `/usr/share/doc/libcdr-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libcdr=0.1.5-1
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.5-1.dsc' libcdr_0.1.5-1.dsc 2108 SHA256:23817cfcb7db8b42c08112f4e76bc590dcd7bbe3e19983f3a7e2f8ae85098c55
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.5.orig.tar.xz' libcdr_0.1.5.orig.tar.xz 612252 SHA256:6ace5c499a8be34ad871e825442ce388614ae2d8675c4381756a7319429e3a48
'http://deb.debian.org/debian/pool/main/libc/libcdr/libcdr_0.1.5-1.debian.tar.xz' libcdr_0.1.5-1.debian.tar.xz 7924 SHA256:e025ea3b21bba8a987bf8e6dc6ed13c0392280e5fafce3c4feedc3464ae40f05
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcdr/0.1.5-1/ (for browsing the source)
- https://sources.debian.net/src/libcdr/0.1.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcdr/0.1.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcmis=0.5.2-1`

Binary Packages:

- `libcmis-0.5-5v5=0.5.2-1`

Licenses: (parsed from: `/usr/share/doc/libcmis-0.5-5v5/copyright`)

- `GPL`
- `LGPL`
- `MPL | GPL2+ | LGPL2+`

Source:

```console
$ apt-get source -qq --print-uris libcmis=0.5.2-1
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.2-1.dsc' libcmis_0.5.2-1.dsc 2132 SHA256:07ecdb727483ce4e2179db023fea64125ddb7ccf1fa750b6d0ab5bbdef38d231
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.2.orig.tar.gz' libcmis_0.5.2.orig.tar.gz 808619 SHA256:ed6f681a48abbf3c2324564b17a180d21fa9503230e8708825e1ad80daee4f81
'http://deb.debian.org/debian/pool/main/libc/libcmis/libcmis_0.5.2-1.debian.tar.xz' libcmis_0.5.2-1.debian.tar.xz 4340 SHA256:2e1afdda9269b23b76ea2d288b087bb2d77e8d31f8b1b80276510845c1d75ac5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcmis/0.5.2-1/ (for browsing the source)
- https://sources.debian.net/src/libcmis/0.5.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcmis/0.5.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcroco=0.6.12-3`

Binary Packages:

- `libcroco3:amd64=0.6.12-3`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.12-3
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.12-3.dsc' libcroco_0.6.12-3.dsc 2222 SHA256:44d5e01f2b94e84ac9f868acaf6e2f7277e748296c248667d3968855ef388250
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.12.orig.tar.xz' libcroco_0.6.12.orig.tar.xz 482028 SHA256:ddc4b5546c9fb4280a5017e2707fbd4839034ed1aba5b7d4372212f34f84f860
'http://deb.debian.org/debian/pool/main/libc/libcroco/libcroco_0.6.12-3.debian.tar.xz' libcroco_0.6.12-3.debian.tar.xz 8200 SHA256:7380d3d5d2a4a7df8d4c8b7fef6edf3558b35634013ace217003bc5b8ca22d14
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcroco/0.6.12-3/ (for browsing the source)
- https://sources.debian.net/src/libcroco/0.6.12-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcroco/0.6.12-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdatrie=0.2.12-2`

Binary Packages:

- `libdatrie1:amd64=0.2.12-2`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.12-2
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.12-2.dsc' libdatrie_0.2.12-2.dsc 2262 SHA256:f51cade98e90d09e181d19e9fa6f976779cfd912215fb8e0f5f451e06e051f26
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.12.orig.tar.xz' libdatrie_0.2.12.orig.tar.xz 310236 SHA256:452dcc4d3a96c01f80f7c291b42be11863cd1554ff78b93e110becce6e00b149
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.12-2.debian.tar.xz' libdatrie_0.2.12-2.debian.tar.xz 8996 SHA256:78b1bb1549cd9cf998442830132f401b100f8f3581415c7588521d164a814e38
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdatrie/0.2.12-2/ (for browsing the source)
- https://sources.debian.net/src/libdatrie/0.2.12-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdatrie/0.2.12-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libde265=1.0.3-1`

Binary Packages:

- `libde265-0:amd64=1.0.3-1+b1`

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
$ apt-get source -qq --print-uris libde265=1.0.3-1
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.3-1.dsc' libde265_1.0.3-1.dsc 2210 SHA256:cfec77f3186539c6573216220ea506ab5c1702d09f71cb5f15aa6aff1821f19c
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.3.orig.tar.gz' libde265_1.0.3.orig.tar.gz 871127 SHA256:e4206185a7c67d3b797d6537df8dcaa6e5fd5a5f93bd14e65a755c33cd645f7a
'http://deb.debian.org/debian/pool/main/libd/libde265/libde265_1.0.3-1.debian.tar.xz' libde265_1.0.3-1.debian.tar.xz 8004 SHA256:c0613a26f8722a4b1edbfd3a69e3b9c2b048a095e4c6167dedcb4c1312658a6e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libde265/1.0.3-1/ (for browsing the source)
- https://sources.debian.net/src/libde265/1.0.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libde265/1.0.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libdrm=2.4.97-1`

Binary Packages:

- `libdrm-amdgpu1:amd64=2.4.97-1`
- `libdrm-common=2.4.97-1`
- `libdrm-intel1:amd64=2.4.97-1`
- `libdrm-nouveau2:amd64=2.4.97-1`
- `libdrm-radeon1:amd64=2.4.97-1`
- `libdrm2:amd64=2.4.97-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libdrm=2.4.97-1
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.97-1.dsc' libdrm_2.4.97-1.dsc 2985 SHA256:a9517c4dcd6e58485d64cb506134bd8f47d0a9788740e6754feb6c1a8fc83a72
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.97.orig.tar.gz' libdrm_2.4.97.orig.tar.gz 1124510 SHA256:8c6f4d0934f5e005cc61bc05a917463b0c867403de176499256965f6797092f1
'http://deb.debian.org/debian/pool/main/libd/libdrm/libdrm_2.4.97-1.diff.gz' libdrm_2.4.97-1.diff.gz 51561 SHA256:8d92b18a722618ac3d800241a992d6438c82ed9009023f677ed332523cf800bd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdrm/2.4.97-1/ (for browsing the source)
- https://sources.debian.net/src/libdrm/2.4.97-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdrm/2.4.97-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libe-book=0.1.3-1`

Binary Packages:

- `libe-book-0.1-1:amd64=0.1.3-1+b2`

Licenses: (parsed from: `/usr/share/doc/libe-book-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libe-book=0.1.3-1
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.3-1.dsc' libe-book_0.1.3-1.dsc 2041 SHA256:d433911367b45f4c5ca5d22cb60c89fb560eecb04bc1bf40b1110c19147b113c
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.3.orig.tar.xz' libe-book_0.1.3.orig.tar.xz 416268 SHA256:7e8d8ff34f27831aca3bc6f9cc532c2f90d2057c778963b884ff3d1e34dfe1f9
'http://deb.debian.org/debian/pool/main/libe/libe-book/libe-book_0.1.3-1.debian.tar.xz' libe-book_0.1.3-1.debian.tar.xz 7184 SHA256:3ddb1cda6b6b116e957620e6b0942f1eb757cde16367218266b73db9ec1de1eb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libe-book/0.1.3-1/ (for browsing the source)
- https://sources.debian.net/src/libe-book/0.1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libe-book/0.1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20181209-1`

Binary Packages:

- `libedit2:amd64=3.1-20181209-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20181209-1
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20181209-1.dsc' libedit_3.1-20181209-1.dsc 2129 SHA256:147972bfbdd01d2e34f498327be6964b7c836d23eb6a13c1ab2becf756db5217
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20181209.orig.tar.gz' libedit_3.1-20181209.orig.tar.gz 521931 SHA256:2811d70c0b000f2ca91b7cb1a37203134441743c4fcc9c37b0b687f328611064
'http://deb.debian.org/debian/pool/main/libe/libedit/libedit_3.1-20181209-1.debian.tar.xz' libedit_3.1-20181209-1.debian.tar.xz 14044 SHA256:605baee35b231f631d4ca046a8b7de4c34403ddf7c1bf418cec8cd7e027d9f8c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libedit/3.1-20181209-1/ (for browsing the source)
- https://sources.debian.net/src/libedit/3.1-20181209-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libedit/3.1-20181209-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libeot=0.01-5`

Binary Packages:

- `libeot0:amd64=0.01-5`

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

### `dpkg` source package: `libepoxy=1.5.3-0.1`

Binary Packages:

- `libepoxy0:amd64=1.5.3-0.1`

Licenses: (parsed from: `/usr/share/doc/libepoxy0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libepoxy=1.5.3-0.1
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.5.3-0.1.dsc' libepoxy_1.5.3-0.1.dsc 2083 SHA256:48fdcfd0a73f2e770ba147e62ba51a8817198e52ba5f8ae29efc36588f89653f
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.5.3.orig.tar.gz' libepoxy_1.5.3.orig.tar.gz 326768 SHA256:c2f1e2c9c12dcc57dee07cd4ca47de83cf19d0226a225b695066ce58ebb4b117
'http://deb.debian.org/debian/pool/main/libe/libepoxy/libepoxy_1.5.3-0.1.debian.tar.xz' libepoxy_1.5.3-0.1.debian.tar.xz 16692 SHA256:e7b6f1d427b997b1b0d55f04f5ced71e462ad298f8382037e803541a205d3a57
```

Other potentially useful URLs:

- https://sources.debian.net/src/libepoxy/1.5.3-0.1/ (for browsing the source)
- https://sources.debian.net/src/libepoxy/1.5.3-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libepoxy/1.5.3-0.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `liberror-perl=0.17027-2`

Binary Packages:

- `liberror-perl=0.17027-2`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17027-2
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17027-2.dsc' liberror-perl_0.17027-2.dsc 2209 SHA256:e40de8c7a6bb1a49334d0d0b71455c933ee84d9d4d6a2ed877470e4c4ded1973
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17027.orig.tar.gz' liberror-perl_0.17027.orig.tar.gz 33260 SHA256:07b2ac8275dfa04144745a6c1900a596280f862b97d22bab0c5ce02682ebd3be
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17027-2.debian.tar.xz' liberror-perl_0.17027-2.debian.tar.xz 4840 SHA256:64abf6989774c072f725af1569d9a234535a0a2f9959e9c4952eeb30cc435a00
```

Other potentially useful URLs:

- https://sources.debian.net/src/liberror-perl/0.17027-2/ (for browsing the source)
- https://sources.debian.net/src/liberror-perl/0.17027-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liberror-perl/0.17027-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libetonyek=0.1.9-1`

Binary Packages:

- `libetonyek-0.1-1:amd64=0.1.9-1`

Licenses: (parsed from: `/usr/share/doc/libetonyek-0.1-1/copyright`)

- `MPL 2.0`

Source:

```console
$ apt-get source -qq --print-uris libetonyek=0.1.9-1
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.9-1.dsc' libetonyek_0.1.9-1.dsc 2141 SHA256:9e739cc099b150b636d7413079cfed22d1b9e9947eb961e53df75ac223491d35
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.9.orig.tar.xz' libetonyek_0.1.9.orig.tar.xz 1477064 SHA256:e61677e8799ce6e55b25afc11aa5339113f6a49cff031f336e32fa58635b1a4a
'http://deb.debian.org/debian/pool/main/libe/libetonyek/libetonyek_0.1.9-1.debian.tar.xz' libetonyek_0.1.9-1.debian.tar.xz 7948 SHA256:6e0b0d5f3347120e813cc00df6775cc34b3b51f2258ec365a63938c018b0b557
```

Other potentially useful URLs:

- https://sources.debian.net/src/libetonyek/0.1.9-1/ (for browsing the source)
- https://sources.debian.net/src/libetonyek/0.1.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libetonyek/0.1.9-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libffi=3.2.1-9`

Binary Packages:

- `libffi6:amd64=3.2.1-9`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-9
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-9.dsc' libffi_3.2.1-9.dsc 2000 SHA256:28beaed76f2ce4c6a3ce1527eb07534c8ef4bf624a42c803fea045c416f8faa5
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.2.1-9.debian.tar.xz' libffi_3.2.1-9.debian.tar.xz 17148 SHA256:26e3cfd358733832da251778bc615a42b908d7779cf8b8d7fc2bdee4660bbbce
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.2.1-9/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.2.1-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.2.1-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libfreehand=0.1.2-2`

Binary Packages:

- `libfreehand-0.1-1=0.1.2-2`

Licenses: (parsed from: `/usr/share/doc/libfreehand-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libfreehand=0.1.2-2
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.2-2.dsc' libfreehand_0.1.2-2.dsc 2039 SHA256:ceba859e4062f5fa88f497d3c7a3927a9e6206c33ca82cfed80aeb2e1dfee5ea
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.2.orig.tar.xz' libfreehand_0.1.2.orig.tar.xz 516132 SHA256:0e422d1564a6dbf22a9af598535425271e583514c0f7ba7d9091676420de34ac
'http://deb.debian.org/debian/pool/main/libf/libfreehand/libfreehand_0.1.2-2.debian.tar.xz' libfreehand_0.1.2-2.debian.tar.xz 13112 SHA256:aa9a003c2acf5f36bee24469ce48ed52f828c66795309cf9d5c514fe5cedfcd1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libfreehand/0.1.2-2/ (for browsing the source)
- https://sources.debian.net/src/libfreehand/0.1.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libfreehand/0.1.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.8.4-5`

Binary Packages:

- `libgcrypt20:amd64=1.8.4-5`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.4-5
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4-5.dsc' libgcrypt20_1.8.4-5.dsc 2806 SHA256:9450f74a867017adbce0dece0653ced251c742947e5d14721c6021a74b78bf65
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4.orig.tar.bz2' libgcrypt20_1.8.4.orig.tar.bz2 2990108 SHA256:f638143a0672628fde0cad745e9b14deb85dffb175709cacc1f4fe24b93f2227
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4.orig.tar.bz2.asc' libgcrypt20_1.8.4.orig.tar.bz2.asc 534 SHA256:97df94317ad273cffce4e78ad34ad0664819b44496f6528818a4298a691209a3
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4-5.debian.tar.xz' libgcrypt20_1.8.4-5.debian.tar.xz 29372 SHA256:bb65f021c13ef1296e575d176bcf073208067c59e0647fb47e33c01e04d24027
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.8.4-5/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.8.4-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.8.4-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libglu=9.0.0-2.1`

Binary Packages:

- `libglu1-mesa:amd64=9.0.0-2.1+b3`

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

### `dpkg` source package: `libglvnd=1.1.0-1`

Binary Packages:

- `libgl1:amd64=1.1.0-1`
- `libglvnd0:amd64=1.1.0-1`
- `libglx0:amd64=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libgl1/copyright`, `/usr/share/doc/libglvnd0/copyright`, `/usr/share/doc/libglx0/copyright`)

- `BSD-1-clause`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libglvnd=1.1.0-1
'http://deb.debian.org/debian/pool/main/libg/libglvnd/libglvnd_1.1.0-1.dsc' libglvnd_1.1.0-1.dsc 2402 SHA256:372839a6488073aa18ed8d0e9fb3c656d4dddd337ee7238ef4f2a8065b6e290c
'http://deb.debian.org/debian/pool/main/libg/libglvnd/libglvnd_1.1.0.orig.tar.gz' libglvnd_1.1.0.orig.tar.gz 828065 SHA256:49aebc4eccebd6baffc53852a15c9f76433dd57ab593e44ad5ba5f0c20c63259
'http://deb.debian.org/debian/pool/main/libg/libglvnd/libglvnd_1.1.0-1.debian.tar.xz' libglvnd_1.1.0-1.debian.tar.xz 20680 SHA256:b8de9f59b33ba45eff213e8173c4150647334a6b7a5300c2e9c5771552cd723d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libglvnd/1.1.0-1/ (for browsing the source)
- https://sources.debian.net/src/libglvnd/1.1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libglvnd/1.1.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.35-1`

Binary Packages:

- `libgpg-error0:amd64=1.35-1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.35-1
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.35-1.dsc' libgpg-error_1.35-1.dsc 2155 SHA256:1d5e455ea385f522a0cf39510291945d42b95fafc8a1f05537cef3863c1d6c16
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.35.orig.tar.bz2' libgpg-error_1.35.orig.tar.bz2 918408 SHA256:cbd5ee62a8a8c88d48c158fff4fc9ead4132aacd1b4a56eb791f9f997d07e067
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.35.orig.tar.bz2.asc' libgpg-error_1.35.orig.tar.bz2.asc 534 SHA256:f6bfdc64a84245437c443f83faea85407d051d0487550515a4a279573589944d
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.35-1.debian.tar.xz' libgpg-error_1.35-1.debian.tar.xz 16056 SHA256:e600a34c09e6a3e8ec63d6145f4a11b16d92dc0ddeff1ba94cba08a8fecf0b66
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.35-1/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.35-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.35-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgsm=1.0.18-2`

Binary Packages:

- `libgsm1:amd64=1.0.18-2`

Licenses: (parsed from: `/usr/share/doc/libgsm1/copyright`)

- `TU-Berlin-2.0`

Source:

```console
$ apt-get source -qq --print-uris libgsm=1.0.18-2
'http://deb.debian.org/debian/pool/main/libg/libgsm/libgsm_1.0.18-2.dsc' libgsm_1.0.18-2.dsc 1831 SHA256:8b189db3805aaaf49073971af2e1a0dad13fdd0efd6b60c0aae687f78fd76a0a
'http://deb.debian.org/debian/pool/main/libg/libgsm/libgsm_1.0.18.orig.tar.gz' libgsm_1.0.18.orig.tar.gz 64549 SHA256:04f68087c3348bf156b78d59f4d8aff545da7f6e14f33be8f47d33f4efae2a10
'http://deb.debian.org/debian/pool/main/libg/libgsm/libgsm_1.0.18-2.debian.tar.xz' libgsm_1.0.18-2.debian.tar.xz 10276 SHA256:3655a18243e6e3d5706dd069347919c26edd3387d63ecf728fc6ecb242b36b43
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgsm/1.0.18-2/ (for browsing the source)
- https://sources.debian.net/src/libgsm/1.0.18-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgsm/1.0.18-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libheif=1.3.2-2~deb10u1`

Binary Packages:

- `libheif1:amd64=1.3.2-2~deb10u1`

Licenses: (parsed from: `/usr/share/doc/libheif1/copyright`)

- `BSD-3-clause`
- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libheif=1.3.2-2~deb10u1
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.3.2-2~deb10u1.dsc' libheif_1.3.2-2~deb10u1.dsc 2333 SHA256:e81d81ad15d672e3cbc98d289e26219463d509c4a177b8b86591399028a4b5b8
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.3.2.orig.tar.gz' libheif_1.3.2.orig.tar.gz 1328174 SHA256:a9e12a693fc172baa16669f427063edd7bf07964a1cb623ee57cd056c06ee3fc
'http://deb.debian.org/debian/pool/main/libh/libheif/libheif_1.3.2-2~deb10u1.debian.tar.xz' libheif_1.3.2-2~deb10u1.debian.tar.xz 5640 SHA256:7a02c3420388eed126d5fa3c6bea58f78e3d32f499487857213aad5d19482914
```

Other potentially useful URLs:

- https://sources.debian.net/src/libheif/1.3.2-2~deb10u1/ (for browsing the source)
- https://sources.debian.net/src/libheif/1.3.2-2~deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libheif/1.3.2-2~deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libidn2=2.0.5-1+deb10u1`

Binary Packages:

- `libidn2-0:amd64=2.0.5-1+deb10u1`

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
$ apt-get source -qq --print-uris libidn2=2.0.5-1+deb10u1
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.0.5-1+deb10u1.dsc' libidn2_2.0.5-1+deb10u1.dsc 2501 SHA256:6c4eac5dc85983e4cf37ee8deea5e23cfb9e1620f7a94a858726676c8858b498
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.0.5.orig.tar.gz' libidn2_2.0.5.orig.tar.gz 2091929 SHA256:53f69170886f1fa6fa5b332439c7a77a7d22626a82ef17e2c1224858bb4ca2b8
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.0.5-1+deb10u1.debian.tar.xz' libidn2_2.0.5-1+deb10u1.debian.tar.xz 10286540 SHA256:37cfdc06e4e2f03e932af5bb309cbe94f8466f8b347aa34fa7c1e03a425556b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.0.5-1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.0.5-1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.0.5-1+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn=1.33-2.2`

Binary Packages:

- `libidn11:amd64=1.33-2.2`

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
$ apt-get source -qq --print-uris libidn=1.33-2.2
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33-2.2.dsc' libidn_1.33-2.2.dsc 2172 SHA256:e5e1744643291bfbfc3492020aaaac07f7438e1d59d8c8350ed32ed512ccda7e
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33.orig.tar.gz' libidn_1.33.orig.tar.gz 3501056 SHA256:44a7aab635bb721ceef6beecc4d49dfd19478325e1b47f3196f7d2acc4930e19
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33-2.2.debian.tar.xz' libidn_1.33-2.2.debian.tar.xz 65500 SHA256:1bbcfa99312552fb076e0de78939aa20e8d33bdaf6ef430dc340e9f66d5fa245
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn/1.33-2.2/ (for browsing the source)
- https://sources.debian.net/src/libidn/1.33-2.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn/1.33-2.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libiec61883=1.2.0-3`

Binary Packages:

- `libiec61883-0:amd64=1.2.0-3`

Licenses: (parsed from: `/usr/share/doc/libiec61883-0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libiec61883=1.2.0-3
'http://deb.debian.org/debian/pool/main/libi/libiec61883/libiec61883_1.2.0-3.dsc' libiec61883_1.2.0-3.dsc 1984 SHA256:1e6c7729cd431e53c8516ae49b4c0ebc0ee255ebeccc7eb629262c7901da6a5a
'http://deb.debian.org/debian/pool/main/libi/libiec61883/libiec61883_1.2.0.orig.tar.gz' libiec61883_1.2.0.orig.tar.gz 339064 SHA256:7c7879c6b9add3148baea697dfbfdcefffbc8ac74e8e6bcf46125ec1d21b373a
'http://deb.debian.org/debian/pool/main/libi/libiec61883/libiec61883_1.2.0-3.debian.tar.xz' libiec61883_1.2.0-3.debian.tar.xz 12800 SHA256:baf4b8031737c2030a1291e1197adff98215b85d830aecb36153034d758d4c39
```

Other potentially useful URLs:

- https://sources.debian.net/src/libiec61883/1.2.0-3/ (for browsing the source)
- https://sources.debian.net/src/libiec61883/1.2.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libiec61883/1.2.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libimage-exiftool-perl=11.16-1`

Binary Packages:

- `libimage-exiftool-perl=11.16-1`

Licenses: (parsed from: `/usr/share/doc/libimage-exiftool-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libimage-exiftool-perl=11.16-1
'http://deb.debian.org/debian/pool/main/libi/libimage-exiftool-perl/libimage-exiftool-perl_11.16-1.dsc' libimage-exiftool-perl_11.16-1.dsc 2366 SHA256:219230190503eaffe68cc10ec7e7521c0a13de3380719577b6a852eaef785d10
'http://deb.debian.org/debian/pool/main/libi/libimage-exiftool-perl/libimage-exiftool-perl_11.16.orig.tar.gz' libimage-exiftool-perl_11.16.orig.tar.gz 4483254 SHA256:0440342f76099a6773cf9d65d5762be5fd16775f652a562bb127d39a409526c9
'http://deb.debian.org/debian/pool/main/libi/libimage-exiftool-perl/libimage-exiftool-perl_11.16-1.debian.tar.xz' libimage-exiftool-perl_11.16-1.debian.tar.xz 7864 SHA256:7404f441c93d52f8b4f2f3f303efd8c9eb47e41806ebfe0eda5a66534ee5e040
```

Other potentially useful URLs:

- https://sources.debian.net/src/libimage-exiftool-perl/11.16-1/ (for browsing the source)
- https://sources.debian.net/src/libimage-exiftool-perl/11.16-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libimage-exiftool-perl/11.16-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libjpeg-turbo=1:1.5.2-2`

Binary Packages:

- `libjpeg62-turbo:amd64=1:1.5.2-2+b1`

Licenses: (parsed from: `/usr/share/doc/libjpeg62-turbo/copyright`)

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

### `dpkg` source package: `libkate=0.4.1-9`

Binary Packages:

- `libkate1:amd64=0.4.1-9`
- `liboggkate1:amd64=0.4.1-9`

Licenses: (parsed from: `/usr/share/doc/libkate1/copyright`, `/usr/share/doc/liboggkate1/copyright`)

- `BSD-3-Clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libkate=0.4.1-9
'http://deb.debian.org/debian/pool/main/libk/libkate/libkate_0.4.1-9.dsc' libkate_0.4.1-9.dsc 2352 SHA256:1e3814ec7c0968133347ee8f6966dd748f3ff795d2d79437bbbd8ebaae2f0124
'http://deb.debian.org/debian/pool/main/libk/libkate/libkate_0.4.1.orig.tar.gz' libkate_0.4.1.orig.tar.gz 906896 SHA256:c40e81d5866c3d4bf744e76ce0068d8f388f0e25f7e258ce0c8e76d7adc87b68
'http://deb.debian.org/debian/pool/main/libk/libkate/libkate_0.4.1-9.debian.tar.xz' libkate_0.4.1-9.debian.tar.xz 7888 SHA256:a437bfe487ebfa7472b720839df347469b61e55d732761e1f366dda57fcacad7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libkate/0.4.1-9/ (for browsing the source)
- https://sources.debian.net/src/libkate/0.4.1-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libkate/0.4.1-9/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `liblqr=0.4.2-2.1`

Binary Packages:

- `liblqr-1-0:amd64=0.4.2-2.1`

Licenses: (parsed from: `/usr/share/doc/liblqr-1-0/copyright`)

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

### `dpkg` source package: `libmspub=0.1.4-1`

Binary Packages:

- `libmspub-0.1-1:amd64=0.1.4-1+b2`

Licenses: (parsed from: `/usr/share/doc/libmspub-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libmspub=0.1.4-1
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.4-1.dsc' libmspub_0.1.4-1.dsc 2105 SHA256:6fce7406b885d7e37c6a542fa5170a27418853b25db66149d0512b8490a267e1
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.4.orig.tar.xz' libmspub_0.1.4.orig.tar.xz 377472 SHA256:ef36c1a1aabb2ba3b0bedaaafe717bf4480be2ba8de6f3894be5fd3702b013ba
'http://deb.debian.org/debian/pool/main/libm/libmspub/libmspub_0.1.4-1.debian.tar.xz' libmspub_0.1.4-1.debian.tar.xz 7160 SHA256:04bb3417404f0048ecbb5ad26e360c64d4df1854baf978dae6159f10c0a45d8f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmspub/0.1.4-1/ (for browsing the source)
- https://sources.debian.net/src/libmspub/0.1.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmspub/0.1.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmwaw=0.3.14-1`

Binary Packages:

- `libmwaw-0.3-3:amd64=0.3.14-1`

Licenses: (parsed from: `/usr/share/doc/libmwaw-0.3-3/copyright`)

- `BSD`
- `LGPL`
- `MPL2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmwaw=0.3.14-1
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.14-1.dsc' libmwaw_0.3.14-1.dsc 2072 SHA256:53cb596bd6980094cb4a5bb5b8b911a0e33f226274c215b27dbe6e6924d7175d
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.14.orig.tar.xz' libmwaw_0.3.14.orig.tar.xz 1276240 SHA256:aca8bf1ce55ed83adbea82c70d4c8bebe8139f334b3481bf5a6e407f91f33ce9
'http://deb.debian.org/debian/pool/main/libm/libmwaw/libmwaw_0.3.14-1.debian.tar.xz' libmwaw_0.3.14-1.debian.tar.xz 8188 SHA256:8c40ea7f6c0c5eb1d3262b063dc719ec21ee39d96e7f3ccf017021a3f7f3e814
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmwaw/0.3.14-1/ (for browsing the source)
- https://sources.debian.net/src/libmwaw/0.3.14-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmwaw/0.3.14-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmysofa=0.6~dfsg0-3+deb10u1`

Binary Packages:

- `libmysofa0:amd64=0.6~dfsg0-3+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libmysofa0/copyright`)

- `BSD-3-clause`
- `CC-BY-4.0`
- `CC-BY-SA-3.0`
- `cipic`
- `listen-ircam`
- `mit-kemar`

Source:

```console
$ apt-get source -qq --print-uris libmysofa=0.6~dfsg0-3+deb10u1
'http://deb.debian.org/debian/pool/main/libm/libmysofa/libmysofa_0.6~dfsg0-3+deb10u1.dsc' libmysofa_0.6~dfsg0-3+deb10u1.dsc 2194 SHA256:7f3ba82dd576e3c710372959a28e8877aa10a2a9688be0b6d46d991486d22bf2
'http://deb.debian.org/debian/pool/main/libm/libmysofa/libmysofa_0.6~dfsg0.orig.tar.gz' libmysofa_0.6~dfsg0.orig.tar.gz 13540940 SHA256:0da589541f37e5d44b4d84b67e9b8aef84e890659a2b089d476f35937e1912dd
'http://deb.debian.org/debian/pool/main/libm/libmysofa/libmysofa_0.6~dfsg0-3+deb10u1.debian.tar.xz' libmysofa_0.6~dfsg0-3+deb10u1.debian.tar.xz 18020 SHA256:0e25258791152287da6c652c3ea36cebad36fb1ec9b463fe0d9066a99079b3a2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmysofa/0.6~dfsg0-3+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/libmysofa/0.6~dfsg0-3+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmysofa/0.6~dfsg0-3+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libnumbertext=1.0.5-1`

Binary Packages:

- `libnumbertext-1.0-0:amd64=1.0.5-1`
- `libnumbertext-data=1.0.5-1`

Licenses: (parsed from: `/usr/share/doc/libnumbertext-1.0-0/copyright`, `/usr/share/doc/libnumbertext-data/copyright`)

- `BSD-3-clause`
- `CC-BY-SA-3.0`
- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libnumbertext=1.0.5-1
'http://deb.debian.org/debian/pool/main/libn/libnumbertext/libnumbertext_1.0.5-1.dsc' libnumbertext_1.0.5-1.dsc 2410 SHA256:a17570782e60a8432808baae2e17c332b874c7fd3b8f124ed83ed54b6226e07a
'http://deb.debian.org/debian/pool/main/libn/libnumbertext/libnumbertext_1.0.5.orig.tar.gz' libnumbertext_1.0.5.orig.tar.gz 410210 SHA256:508f259325efc25705e27ca1bafe487aa0b8b0f5cc3bf77cb2d53ce7f119c380
'http://deb.debian.org/debian/pool/main/libn/libnumbertext/libnumbertext_1.0.5-1.debian.tar.xz' libnumbertext_1.0.5-1.debian.tar.xz 11328 SHA256:1836b521bd14cf337a6d9a76a49cbd3d6d4e75ba2df8328b359bfb59343958b9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libnumbertext/1.0.5-1/ (for browsing the source)
- https://sources.debian.net/src/libnumbertext/1.0.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libnumbertext/1.0.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libodfgen=0.1.7-1`

Binary Packages:

- `libodfgen-0.1-1:amd64=0.1.7-1`

Licenses: (parsed from: `/usr/share/doc/libodfgen-0.1-1/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libodfgen=0.1.7-1
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.7-1.dsc' libodfgen_0.1.7-1.dsc 1936 SHA256:809fcb4062586f80cf551965c63cf05d9a7b242cd31bd07eb5f094590f994559
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.7.orig.tar.xz' libodfgen_0.1.7.orig.tar.xz 384760 SHA256:323e491f956c8ca2abb12c998e350670930a32317bf9662b0615dd4b3922b831
'http://deb.debian.org/debian/pool/main/libo/libodfgen/libodfgen_0.1.7-1.debian.tar.xz' libodfgen_0.1.7-1.debian.tar.xz 6884 SHA256:6c24a59da564409bd23bb790ea48697522f2d2114d2a90ea313b7c2b8ce727b6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libodfgen/0.1.7-1/ (for browsing the source)
- https://sources.debian.net/src/libodfgen/0.1.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libodfgen/0.1.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libogg=1.3.2-1`

Binary Packages:

- `libogg0:amd64=1.3.2-1+b1`

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

### `dpkg` source package: `libopenmpt=0.4.3-1`

Binary Packages:

- `libopenmpt0:amd64=0.4.3-1`

Licenses: (parsed from: `/usr/share/doc/libopenmpt0/copyright`)

- `BSD-3-clause`
- `GNU-All-Permissive-License`
- `GNU-All-Permissive-License-FSF`
- `GPL-2`
- `GPL-2+ with Autoconf exception`
- `GPL-2+ with LibTool exception`
- `GPL-3`
- `GPL-3+ with AutoConf exception`
- `GPL-3+ with Autoconf Macros exception`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris libopenmpt=0.4.3-1
'http://deb.debian.org/debian/pool/main/libo/libopenmpt/libopenmpt_0.4.3-1.dsc' libopenmpt_0.4.3-1.dsc 2708 SHA256:f4df1873844052732b4903a9b46c4ced2237d13dfc0821a0c68c2cd62978f06c
'http://deb.debian.org/debian/pool/main/libo/libopenmpt/libopenmpt_0.4.3.orig.tar.gz' libopenmpt_0.4.3.orig.tar.gz 1462862 SHA256:d77443a279003921d6f0c4edb30d1e9dda387983f44113a6d58f623c1e6942ae
'http://deb.debian.org/debian/pool/main/libo/libopenmpt/libopenmpt_0.4.3-1.debian.tar.xz' libopenmpt_0.4.3-1.debian.tar.xz 12880 SHA256:63a57ffd4badfe61133e95f2f81b93fb654f20e0f1141847f778261ae52f4e6c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libopenmpt/0.4.3-1/ (for browsing the source)
- https://sources.debian.net/src/libopenmpt/0.4.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libopenmpt/0.4.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `liborcus=0.14.1-6`

Binary Packages:

- `liborcus-0.14-0:amd64=0.14.1-6`

Licenses: (parsed from: `/usr/share/doc/liborcus-0.14-0/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3+`
- `MIT`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris liborcus=0.14.1-6
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.14.1-6.dsc' liborcus_0.14.1-6.dsc 2732 SHA256:5f46ed94069364d03bab057cacf33b553bf79c38316f02134ce4c5a42fd94655
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.14.1.orig.tar.xz' liborcus_0.14.1.orig.tar.xz 1649160 SHA256:1f48a384c02ae1bc2e5f93979cae17c49b5b45b1d2f9dd68cade890dee94ba36
'http://deb.debian.org/debian/pool/main/libo/liborcus/liborcus_0.14.1-6.debian.tar.xz' liborcus_0.14.1-6.debian.tar.xz 12216 SHA256:2b3e308e5094104d207bd97c8dadd2b0892368bd54f3cc7c4ae2854e4c3a7138
```

Other potentially useful URLs:

- https://sources.debian.net/src/liborcus/0.14.1-6/ (for browsing the source)
- https://sources.debian.net/src/liborcus/0.14.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liborcus/0.14.1-6/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libpaper=1.1.28`

Binary Packages:

- `libpaper1:amd64=1.1.28`

Licenses: (parsed from: `/usr/share/doc/libpaper1/copyright`)

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

### `dpkg` source package: `libpciaccess=0.14-1`

Binary Packages:

- `libpciaccess0:amd64=0.14-1`

Licenses: (parsed from: `/usr/share/doc/libpciaccess0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpciaccess=0.14-1
'http://deb.debian.org/debian/pool/main/libp/libpciaccess/libpciaccess_0.14-1.dsc' libpciaccess_0.14-1.dsc 2062 SHA256:1cbfd426e4efcc958b6c9fd4889877b533035175370fa0505f361b89e1aeaa4f
'http://deb.debian.org/debian/pool/main/libp/libpciaccess/libpciaccess_0.14.orig.tar.gz' libpciaccess_0.14.orig.tar.gz 461764 SHA256:8d86e64893917be3dfb1c5e837888d1275399c818783474002203d751312b03c
'http://deb.debian.org/debian/pool/main/libp/libpciaccess/libpciaccess_0.14-1.diff.gz' libpciaccess_0.14-1.diff.gz 25039 SHA256:fea9483fbfb202040a8e5eef3ec3b434b3e897f301e735753568db2106e1512d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpciaccess/0.14-1/ (for browsing the source)
- https://sources.debian.net/src/libpciaccess/0.14-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpciaccess/0.14-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpgm=5.2.122~dfsg-3`

Binary Packages:

- `libpgm-5.2-0:amd64=5.2.122~dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libpgm-5.2-0/copyright`)

- `BSD-3-clause`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libpgm=5.2.122~dfsg-3
'http://deb.debian.org/debian/pool/main/libp/libpgm/libpgm_5.2.122~dfsg-3.dsc' libpgm_5.2.122~dfsg-3.dsc 1821 SHA256:bbe8ae72250fa76cae7e19ecbc22b96c0ff8c37eb059eb1253b792bb9fb1a74b
'http://deb.debian.org/debian/pool/main/libp/libpgm/libpgm_5.2.122~dfsg.orig.tar.xz' libpgm_5.2.122~dfsg.orig.tar.xz 550996 SHA256:d6e5ec0918216d4e9b14459f5742f6f8416df965f03ac4d854bd5d111709b507
'http://deb.debian.org/debian/pool/main/libp/libpgm/libpgm_5.2.122~dfsg-3.debian.tar.xz' libpgm_5.2.122~dfsg-3.debian.tar.xz 6996 SHA256:6ebc892bd2d7ce3ef23beff96d9f24c26e19bf28b467d15b83c8329704782122
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpgm/5.2.122~dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/libpgm/5.2.122~dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpgm/5.2.122~dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libpng1.6=1.6.36-6`

Binary Packages:

- `libpng16-16:amd64=1.6.36-6`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.36-6
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.36-6.dsc' libpng1.6_1.6.36-6.dsc 2219 SHA256:54400844c4631a09ee96f3d3cd1907da7fd4ba053b5d66dc93d9c334d520bc16
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.36.orig.tar.xz' libpng1.6_1.6.36.orig.tar.xz 1012544 SHA256:eceb924c1fa6b79172fdfd008d335f0e59172a86a66481e09d4089df872aa319
'http://deb.debian.org/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.36-6.debian.tar.xz' libpng1.6_1.6.36-6.debian.tar.xz 38376 SHA256:69751c1d45b319237144f536385a6cc05c8d852d83170d7f7f322474e04b94b0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libpng1.6/1.6.36-6/ (for browsing the source)
- https://sources.debian.net/src/libpng1.6/1.6.36-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libpng1.6/1.6.36-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libproxy=0.4.15-5`

Binary Packages:

- `libproxy1v5:amd64=0.4.15-5`

Licenses: (parsed from: `/usr/share/doc/libproxy1v5/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libproxy=0.4.15-5
'http://deb.debian.org/debian/pool/main/libp/libproxy/libproxy_0.4.15-5.dsc' libproxy_0.4.15-5.dsc 3593 SHA256:9036b9d92d4b42e33d247938899b5d74f4b732f44d555ed1aea86c0a97fbb65f
'http://deb.debian.org/debian/pool/main/libp/libproxy/libproxy_0.4.15.orig.tar.gz' libproxy_0.4.15.orig.tar.gz 93084 SHA256:18f58b0a0043b6881774187427ead158d310127fc46a1c668ad6d207fb28b4e0
'http://deb.debian.org/debian/pool/main/libp/libproxy/libproxy_0.4.15-5.debian.tar.xz' libproxy_0.4.15-5.debian.tar.xz 11556 SHA256:d3731410a393fd4bb5aa34e2991d4504866a9b60bf9fb1d95c7515277ade16fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libproxy/0.4.15-5/ (for browsing the source)
- https://sources.debian.net/src/libproxy/0.4.15-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libproxy/0.4.15-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libqxp=0.0.2-1`

Binary Packages:

- `libqxp-0.0-0=0.0.2-1`

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

### `dpkg` source package: `libreoffice=1:6.1.5-3+deb10u5`

Binary Packages:

- `fonts-opensymbol=2:102.10+LibO6.1.5-3+deb10u5`
- `libreoffice=1:6.1.5-3+deb10u5`
- `libreoffice-avmedia-backend-gstreamer=1:6.1.5-3+deb10u5`
- `libreoffice-base=1:6.1.5-3+deb10u5`
- `libreoffice-base-core=1:6.1.5-3+deb10u5`
- `libreoffice-base-drivers=1:6.1.5-3+deb10u5`
- `libreoffice-calc=1:6.1.5-3+deb10u5`
- `libreoffice-common=1:6.1.5-3+deb10u5`
- `libreoffice-core=1:6.1.5-3+deb10u5`
- `libreoffice-draw=1:6.1.5-3+deb10u5`
- `libreoffice-impress=1:6.1.5-3+deb10u5`
- `libreoffice-math=1:6.1.5-3+deb10u5`
- `libreoffice-report-builder-bin=1:6.1.5-3+deb10u5`
- `libreoffice-style-colibre=1:6.1.5-3+deb10u5`
- `libreoffice-style-tango=1:6.1.5-3+deb10u5`
- `libreoffice-writer=1:6.1.5-3+deb10u5`
- `python3-uno=1:6.1.5-3+deb10u5`
- `uno-libs3=6.1.5-3+deb10u5`
- `ure=6.1.5-3+deb10u5`

Licenses: (parsed from: `/usr/share/doc/fonts-opensymbol/copyright`, `/usr/share/doc/libreoffice/copyright`, `/usr/share/doc/libreoffice-avmedia-backend-gstreamer/copyright`, `/usr/share/doc/libreoffice-base/copyright`, `/usr/share/doc/libreoffice-base-core/copyright`, `/usr/share/doc/libreoffice-base-drivers/copyright`, `/usr/share/doc/libreoffice-calc/copyright`, `/usr/share/doc/libreoffice-common/copyright`, `/usr/share/doc/libreoffice-core/copyright`, `/usr/share/doc/libreoffice-draw/copyright`, `/usr/share/doc/libreoffice-impress/copyright`, `/usr/share/doc/libreoffice-math/copyright`, `/usr/share/doc/libreoffice-report-builder-bin/copyright`, `/usr/share/doc/libreoffice-style-colibre/copyright`, `/usr/share/doc/libreoffice-style-tango/copyright`, `/usr/share/doc/libreoffice-writer/copyright`, `/usr/share/doc/python3-uno/copyright`, `/usr/share/doc/uno-libs3/copyright`, `/usr/share/doc/ure/copyright`)

- `Apache-2.0`
- `CC-BY-SA-3.0`
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
- `other`

Source:

```console
$ apt-get source -qq --print-uris libreoffice=1:6.1.5-3+deb10u5
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_6.1.5-3+deb10u5.dsc' libreoffice_6.1.5-3+deb10u5.dsc 27751 SHA256:64fab15443d3aaf3141ab1b24e2901c28f845f3eeca3aad98044570222edfc26
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_6.1.5.orig-helpcontent2.tar.xz' libreoffice_6.1.5.orig-helpcontent2.tar.xz 15185272 SHA256:ea786426ebd47b32a324daf40e9c6534845f1e3ba9d8f7bc92bb5ed84bb5c1f3
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_6.1.5.orig-translations.tar.xz' libreoffice_6.1.5.orig-translations.tar.xz 141848256 SHA256:6e34d397c1527aca9057c3f874e294afa3614cfe3d134dc2075c8b4f58156de6
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_6.1.5.orig.tar.xz' libreoffice_6.1.5.orig.tar.xz 207918636 SHA256:eb49fe8c8d1d18ffc8bcafff59d8c998f7df2e8f8683c55cb509ad3a31c408f2
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_6.1.5.orig.tar.xz.asc' libreoffice_6.1.5.orig.tar.xz.asc 833 SHA256:e5000387f10d5ea3cfd973112a27209afb92439de5da9ac846ce6ce7a483389f
'http://deb.debian.org/debian/pool/main/libr/libreoffice/libreoffice_6.1.5-3+deb10u5.debian.tar.xz' libreoffice_6.1.5-3+deb10u5.debian.tar.xz 9978044 SHA256:e2753fd908b18451f06f85c4f43eb1eefaad9fbe29c72267b85367fca15f5728
```

Other potentially useful URLs:

- https://sources.debian.net/src/libreoffice/1:6.1.5-3+deb10u5/ (for browsing the source)
- https://sources.debian.net/src/libreoffice/1:6.1.5-3+deb10u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libreoffice/1:6.1.5-3+deb10u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `librest=0.8.1-1`

Binary Packages:

- `librest-0.7-0:amd64=0.8.1-1`

Licenses: (parsed from: `/usr/share/doc/librest-0.7-0/copyright`)

- `FSF-INSTALL`
- `FSF-aclocal`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `MIT with XConsortium exception `

Source:

```console
$ apt-get source -qq --print-uris librest=0.8.1-1
'http://deb.debian.org/debian/pool/main/libr/librest/librest_0.8.1-1.dsc' librest_0.8.1-1.dsc 2418 SHA256:0ec122ae048847cc8203b72a7377da475b614ee91c37654163e0622194f122bb
'http://deb.debian.org/debian/pool/main/libr/librest/librest_0.8.1.orig.tar.bz2' librest_0.8.1.orig.tar.bz2 68249 SHA256:9063b9906c3a4684bef6ccaad9462e8409e1025fe37b7c9596fcf2f5f7507904
'http://deb.debian.org/debian/pool/main/libr/librest/librest_0.8.1-1.debian.tar.xz' librest_0.8.1-1.debian.tar.xz 6696 SHA256:9bfb3d85e7904cf8d740932a3bba10b5baf7f2ca371887d9fe0b16af8d34fc32
```

Other potentially useful URLs:

- https://sources.debian.net/src/librest/0.8.1-1/ (for browsing the source)
- https://sources.debian.net/src/librest/0.8.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librest/0.8.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `librsvg=2.44.10-2.1`

Binary Packages:

- `librsvg2-2:amd64=2.44.10-2.1`
- `librsvg2-common:amd64=2.44.10-2.1`

Licenses: (parsed from: `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`)

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
$ apt-get source -qq --print-uris librsvg=2.44.10-2.1
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.44.10-2.1.dsc' librsvg_2.44.10-2.1.dsc 2875 SHA256:b68ca39d7603da41a363a9667184cfe46c1a0f804362829fe953a3f3a2e21e59
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.44.10.orig.tar.xz' librsvg_2.44.10.orig.tar.xz 9874524 SHA256:175bb677837d5ab3596c3287e3d40f9bb60469271fd3055f2e2d1b54aeaa4f5d
'http://deb.debian.org/debian/pool/main/libr/librsvg/librsvg_2.44.10-2.1.debian.tar.xz' librsvg_2.44.10-2.1.debian.tar.xz 23972 SHA256:106c4e4ecdca6a845957830d6e0135ed01dcf5e63cfc57669754bb80cba50d3f
```

Other potentially useful URLs:

- https://sources.debian.net/src/librsvg/2.44.10-2.1/ (for browsing the source)
- https://sources.debian.net/src/librsvg/2.44.10-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/librsvg/2.44.10-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsamplerate=0.1.9-2`

Binary Packages:

- `libsamplerate0:amd64=0.1.9-2`

Licenses: (parsed from: `/usr/share/doc/libsamplerate0/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libsamplerate=0.1.9-2
'http://deb.debian.org/debian/pool/main/libs/libsamplerate/libsamplerate_0.1.9-2.dsc' libsamplerate_0.1.9-2.dsc 2159 SHA256:a424910e1cdcfc8596a086c3256af8b63af450f4d0bc244fab3163cbb8e1707a
'http://deb.debian.org/debian/pool/main/libs/libsamplerate/libsamplerate_0.1.9.orig.tar.gz' libsamplerate_0.1.9.orig.tar.gz 4336641 SHA256:0a7eb168e2f21353fb6d84da152e4512126f7dc48ccb0be80578c565413444c1
'http://deb.debian.org/debian/pool/main/libs/libsamplerate/libsamplerate_0.1.9-2.debian.tar.xz' libsamplerate_0.1.9-2.debian.tar.xz 7496 SHA256:9fb3e5e7724f327272b7228ea267bfbb53be214db35778d85e3a9ce5e618634b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsamplerate/0.1.9-2/ (for browsing the source)
- https://sources.debian.net/src/libsamplerate/0.1.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsamplerate/0.1.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsdl2=2.0.9+dfsg1-1`

Binary Packages:

- `libsdl2-2.0-0:amd64=2.0.9+dfsg1-1`

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
$ apt-get source -qq --print-uris libsdl2=2.0.9+dfsg1-1
'http://deb.debian.org/debian/pool/main/libs/libsdl2/libsdl2_2.0.9+dfsg1-1.dsc' libsdl2_2.0.9+dfsg1-1.dsc 2774 SHA256:65656e3aa44cb9565ac2063320665442b25c921267f113cd55b5d9900b1e9d92
'http://deb.debian.org/debian/pool/main/libs/libsdl2/libsdl2_2.0.9+dfsg1.orig.tar.xz' libsdl2_2.0.9+dfsg1.orig.tar.xz 2277172 SHA256:80a8b03376e96d3d210d642a93fc9bf41902399557025419e52a97c37a9cab7d
'http://deb.debian.org/debian/pool/main/libs/libsdl2/libsdl2_2.0.9+dfsg1-1.debian.tar.xz' libsdl2_2.0.9+dfsg1-1.debian.tar.xz 18260 SHA256:5e49299244f5da653820a178e98a7b7495da21b50d7e7c93c7731e10c123d6d6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsdl2/2.0.9+dfsg1-1/ (for browsing the source)
- https://sources.debian.net/src/libsdl2/2.0.9+dfsg1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsdl2/2.0.9+dfsg1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.3.3-4`

Binary Packages:

- `libseccomp2:amd64=2.3.3-4`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.3.3-4
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.3-4.dsc' libseccomp_2.3.3-4.dsc 2500 SHA256:1443086c253ffacdad635aeb27a37b21958119833782290ae868b897eb9f6ab0
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.3.orig.tar.gz' libseccomp_2.3.3.orig.tar.gz 564546 SHA256:7fc28f4294cc72e61c529bedf97e705c3acf9c479a8f1a3028d4cd2ca9f3b155
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.3.3-4.debian.tar.xz' libseccomp_2.3.3-4.debian.tar.xz 12104 SHA256:deab2e069e145bf31d0a5569ad3adb2b94217623e02a25d4c9fa0d298073769e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.3.3-4/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.3.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.3.3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=2.8-1`

Binary Packages:

- `libselinux1:amd64=2.8-1+b1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.8-1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.8-1.dsc' libselinux_2.8-1.dsc 2347 SHA256:0f08d64f4488312a8e8b7ffb12771cd385560752473a2e585449edc27223c129
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.8.orig.tar.gz' libselinux_2.8.orig.tar.gz 187759 SHA256:31db96ec7643ce10912b3c3f98506a08a9116dcfe151855fd349c3fda96187e1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_2.8-1.debian.tar.xz' libselinux_2.8-1.debian.tar.xz 23052 SHA256:a0b150e870a3da7e1d7b0fec7c1a5ae6988a0985e545c69cfe8fe05363c5bf64
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/2.8-1/ (for browsing the source)
- https://sources.debian.net/src/libselinux/2.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/2.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=2.8-2`

Binary Packages:

- `libsemanage-common=2.8-2`
- `libsemanage1:amd64=2.8-2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.8-2
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.8-2.dsc' libsemanage_2.8-2.dsc 2434 SHA256:f7cbe0594c098808a449804a357159bec4db54389df0319c2b5306b10ec2e707
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.8.orig.tar.gz' libsemanage_2.8.orig.tar.gz 154200 SHA256:1c0de8d2c51e5460926c21e371105c84a39087dfd8f8e9f0cc1d017e4cbea8e2
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_2.8-2.debian.tar.xz' libsemanage_2.8-2.debian.tar.xz 17756 SHA256:02315ffeb2b0a24b7c3bc8fa0c0e1e217e4a7b284bb88f64b0bf613e76d125e2
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/2.8-2/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/2.8-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/2.8-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=2.8-1`

Binary Packages:

- `libsepol1:amd64=2.8-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.8-1
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.8-1.dsc' libsepol_2.8-1.dsc 1792 SHA256:37b0b79ab0f7533c194272809ccb3f3c5ff788536f66254c0d405e2e8b2b270e
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.8.orig.tar.gz' libsepol_2.8.orig.tar.gz 473384 SHA256:3ad6916a8352bef0bad49acc8037a5f5b48c56f94e4cb4e1959ca475fa9d24d6
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_2.8-1.debian.tar.xz' libsepol_2.8-1.debian.tar.xz 14076 SHA256:7b8d0b47396c96830754db2e5b679d294486aeffd93cfd21ac68202031374a00
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/2.8-1/ (for browsing the source)
- https://sources.debian.net/src/libsepol/2.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/2.8-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libsndfile=1.0.28-6`

Binary Packages:

- `libsndfile1:amd64=1.0.28-6`

Licenses: (parsed from: `/usr/share/doc/libsndfile1/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `FSFAP`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `gsm`
- `sun`

Source:

```console
$ apt-get source -qq --print-uris libsndfile=1.0.28-6
'http://deb.debian.org/debian/pool/main/libs/libsndfile/libsndfile_1.0.28-6.dsc' libsndfile_1.0.28-6.dsc 2195 SHA256:91d5bd81cb4e8ebc01e54ec7398f47aa0ff78330640c599c046ad019b240ee45
'http://deb.debian.org/debian/pool/main/libs/libsndfile/libsndfile_1.0.28.orig.tar.gz' libsndfile_1.0.28.orig.tar.gz 1202833 SHA256:1ff33929f042fa333aed1e8923aa628c3ee9e1eb85512686c55092d1e5a9dfa9
'http://deb.debian.org/debian/pool/main/libs/libsndfile/libsndfile_1.0.28-6.debian.tar.xz' libsndfile_1.0.28-6.debian.tar.xz 16332 SHA256:25ae11e5742ef808cf9e74dbfb905323b9aa31941f35847e939380818c98e5cc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsndfile/1.0.28-6/ (for browsing the source)
- https://sources.debian.net/src/libsndfile/1.0.28-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsndfile/1.0.28-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsodium=1.0.17-1`

Binary Packages:

- `libsodium23:amd64=1.0.17-1`

Licenses: (parsed from: `/usr/share/doc/libsodium23/copyright`)

- `BSD-2-clause`
- `CC0`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libsodium=1.0.17-1
'http://deb.debian.org/debian/pool/main/libs/libsodium/libsodium_1.0.17-1.dsc' libsodium_1.0.17-1.dsc 1913 SHA256:e2fb1951476b7b7177e7b2848b6d896a55ddffb11b0e5f82563d24944fc910ac
'http://deb.debian.org/debian/pool/main/libs/libsodium/libsodium_1.0.17.orig.tar.gz' libsodium_1.0.17.orig.tar.gz 1604410 SHA256:602e07029c780e154347fb95495b13ce48709ae705c6cff927ecb0c485b95672
'http://deb.debian.org/debian/pool/main/libs/libsodium/libsodium_1.0.17-1.debian.tar.xz' libsodium_1.0.17-1.debian.tar.xz 7256 SHA256:fdaf9fcb6b5a0801f1344d2350da2882d49273ed9c641e1dd747a66e5b318b6c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsodium/1.0.17-1/ (for browsing the source)
- https://sources.debian.net/src/libsodium/1.0.17-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsodium/1.0.17-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsoup2.4=2.64.2-2`

Binary Packages:

- `libsoup-gnome2.4-1:amd64=2.64.2-2`
- `libsoup2.4-1:amd64=2.64.2-2`

Licenses: (parsed from: `/usr/share/doc/libsoup-gnome2.4-1/copyright`, `/usr/share/doc/libsoup2.4-1/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libsoup2.4=2.64.2-2
'http://deb.debian.org/debian/pool/main/libs/libsoup2.4/libsoup2.4_2.64.2-2.dsc' libsoup2.4_2.64.2-2.dsc 2683 SHA256:753759de74e4a1850e09d046cc8918a7053b9ea7b5e3d47667000e9d8434143b
'http://deb.debian.org/debian/pool/main/libs/libsoup2.4/libsoup2.4_2.64.2.orig.tar.xz' libsoup2.4_2.64.2.orig.tar.xz 1793440 SHA256:75ddc194a5b1d6f25033bb9d355f04bfe5c03e0e1c71ed0774104457b3a786c6
'http://deb.debian.org/debian/pool/main/libs/libsoup2.4/libsoup2.4_2.64.2-2.debian.tar.xz' libsoup2.4_2.64.2-2.debian.tar.xz 17896 SHA256:7c875c91ec49cba83d62ac9a7b800712aaea4470d9126432896c46b1359210a7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsoup2.4/2.64.2-2/ (for browsing the source)
- https://sources.debian.net/src/libsoup2.4/2.64.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsoup2.4/2.64.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsoxr=0.1.2-3`

Binary Packages:

- `libsoxr0:amd64=0.1.2-3`

Licenses: (parsed from: `/usr/share/doc/libsoxr0/copyright`)

- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Spherepack`
- `permissive1`
- `permissive2`

Source:

```console
$ apt-get source -qq --print-uris libsoxr=0.1.2-3
'http://deb.debian.org/debian/pool/main/libs/libsoxr/libsoxr_0.1.2-3.dsc' libsoxr_0.1.2-3.dsc 2170 SHA256:7f6133cee147b7c7d819c6de78541ebedd97cc79a2b66451421d8bea8a9a9d5b
'http://deb.debian.org/debian/pool/main/libs/libsoxr/libsoxr_0.1.2.orig.tar.xz' libsoxr_0.1.2.orig.tar.xz 83760 SHA256:54e6f434f1c491388cd92f0e3c47f1ade082cc24327bdc43762f7d1eefe0c275
'http://deb.debian.org/debian/pool/main/libs/libsoxr/libsoxr_0.1.2-3.debian.tar.xz' libsoxr_0.1.2-3.debian.tar.xz 4840 SHA256:8c49143d8c600ea024da765049dcddc392d033cea0c43ec4fc27e4c9d0e3d94a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsoxr/0.1.2-3/ (for browsing the source)
- https://sources.debian.net/src/libsoxr/0.1.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsoxr/0.1.2-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libssh=0.8.7-1`

Binary Packages:

- `libssh-gcrypt-4:amd64=0.8.7-1`

Licenses: (parsed from: `/usr/share/doc/libssh-gcrypt-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.8.7-1
'http://deb.debian.org/debian/pool/main/libs/libssh/libssh_0.8.7-1.dsc' libssh_0.8.7-1.dsc 2436 SHA256:86eac33fbdb9aa5d1dbcae383198fba93067d7e85c72ff5e99a475b445452bf7
'http://deb.debian.org/debian/pool/main/libs/libssh/libssh_0.8.7.orig.tar.xz' libssh_0.8.7.orig.tar.xz 430104 SHA256:43304ca22f0ba0b654e14b574a39816bc70212fdea5858a6637cc26cade3d592
'http://deb.debian.org/debian/pool/main/libs/libssh/libssh_0.8.7-1.debian.tar.xz' libssh_0.8.7-1.debian.tar.xz 26212 SHA256:9a66708a602bdfb19a41aea677ea1d49f9a722b3d42772985e19238a19e85ea4
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh/0.8.7-1/ (for browsing the source)
- https://sources.debian.net/src/libssh/0.8.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh/0.8.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libstaroffice=0.0.6-1`

Binary Packages:

- `libstaroffice-0.0-0:amd64=0.0.6-1`

Licenses: (parsed from: `/usr/share/doc/libstaroffice-0.0-0/copyright`)

- `BSD`
- `LGPL`
- `MPL2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libstaroffice=0.0.6-1
'http://deb.debian.org/debian/pool/main/libs/libstaroffice/libstaroffice_0.0.6-1.dsc' libstaroffice_0.0.6-1.dsc 2155 SHA256:396a566ea3bcfc475b29a6185647b61d42e56aa53e42010c7100e67f24683953
'http://deb.debian.org/debian/pool/main/libs/libstaroffice/libstaroffice_0.0.6.orig.tar.xz' libstaroffice_0.0.6.orig.tar.xz 706324 SHA256:6b00e1ed8194e6072be4441025d1b888e39365727ed5b23e0e8c92c4009d1ec4
'http://deb.debian.org/debian/pool/main/libs/libstaroffice/libstaroffice_0.0.6-1.debian.tar.xz' libstaroffice_0.0.6-1.debian.tar.xz 8144 SHA256:e4c86e326757ff51622da08052944a2b61998710c5bebefae358706bae277d83
```

Other potentially useful URLs:

- https://sources.debian.net/src/libstaroffice/0.0.6-1/ (for browsing the source)
- https://sources.debian.net/src/libstaroffice/0.0.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libstaroffice/0.0.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.13-3`

Binary Packages:

- `libtasn1-6:amd64=4.13-3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.13-3
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13-3.dsc' libtasn1-6_4.13-3.dsc 2574 SHA256:15a984daba0bc64819a1203cd28a1e869a30e0edde227237e4cdcfbc86131227
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz' libtasn1-6_4.13.orig.tar.gz 1891703 SHA256:7e528e8c317ddd156230c4e31d082cd13e7ddeb7a54824be82632209550c8cca
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz.asc' libtasn1-6_4.13.orig.tar.gz.asc 774 SHA256:90261376528edf44831d1369847088cc2fb48669860d343961daca42e674b226
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.13-3.debian.tar.xz' libtasn1-6_4.13-3.debian.tar.xz 63384 SHA256:1428c31d3d900d8fa1946fc29d9d2839c73c7a4c0ebff7a2571c134aef53c310
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.13-3/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.13-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.13-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libthai=0.1.28-2`

Binary Packages:

- `libthai-data=0.1.28-2`
- `libthai0:amd64=0.1.28-2`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.28-2
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28-2.dsc' libthai_0.1.28-2.dsc 2348 SHA256:93e36d78cb14add1ff913f27957719bf08c8a87b4611ad1eef5961ce2cc45a43
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28.orig.tar.xz' libthai_0.1.28.orig.tar.xz 413592 SHA256:ffe0a17b4b5aa11b153c15986800eca19f6c93a4025ffa5cf2cab2dcdf1ae911
'http://deb.debian.org/debian/pool/main/libt/libthai/libthai_0.1.28-2.debian.tar.xz' libthai_0.1.28-2.debian.tar.xz 11952 SHA256:6cf7601099f2401bf206f988db523f1c06901432ae0ace720541209a93735ccd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libthai/0.1.28-2/ (for browsing the source)
- https://sources.debian.net/src/libthai/0.1.28-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libthai/0.1.28-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtheora=1.1.1+dfsg.1-15`

Binary Packages:

- `libtheora0:amd64=1.1.1+dfsg.1-15`

Licenses: (parsed from: `/usr/share/doc/libtheora0/copyright`)

- `BSD-3-Clause`

Source:

```console
$ apt-get source -qq --print-uris libtheora=1.1.1+dfsg.1-15
'http://deb.debian.org/debian/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-15.dsc' libtheora_1.1.1+dfsg.1-15.dsc 2603 SHA256:8c6c3a7d5befe0e67eb87e19c8b09046bfa185a57c4f0716ec32b4386cfc51a6
'http://deb.debian.org/debian/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1.orig.tar.gz' libtheora_1.1.1+dfsg.1.orig.tar.gz 2100495 SHA256:c59b0f07a7314dfe2ade15c41bc9f637f8a450fc6b340af61b81760629f28f90
'http://deb.debian.org/debian/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-15.debian.tar.xz' libtheora_1.1.1+dfsg.1-15.debian.tar.xz 10736 SHA256:ffd09e84ac612b4f6326d4c43b26349688be34f688e09a6ed3c9160fcb99bead
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtheora/1.1.1+dfsg.1-15/ (for browsing the source)
- https://sources.debian.net/src/libtheora/1.1.1+dfsg.1-15/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtheora/1.1.1+dfsg.1-15/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtool=2.4.6-9`

Binary Packages:

- `libltdl7:amd64=2.4.6-9`

Licenses: (parsed from: `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-9
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-9.dsc' libtool_2.4.6-9.dsc 2479 SHA256:3c5f93896e23939923db04ed4e756b7bd801dc562fab9202b304916cca8de7cf
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://deb.debian.org/debian/pool/main/libt/libtool/libtool_2.4.6-9.debian.tar.xz' libtool_2.4.6-9.debian.tar.xz 48724 SHA256:489885dceeb98fe168e0c1a3955c1d0c0d83e9aaff969188a3fd42116cb61b29
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtool/2.4.6-9/ (for browsing the source)
- https://sources.debian.net/src/libtool/2.4.6-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtool/2.4.6-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=0.9.10-1`

Binary Packages:

- `libunistring2:amd64=0.9.10-1`

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
$ apt-get source -qq --print-uris libunistring=0.9.10-1
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-1.dsc' libunistring_0.9.10-1.dsc 2206 SHA256:2118b96b1125399556bd95b8917cd559c4e9afe8d85861b01435f9635cefcdf2
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_0.9.10-1.debian.tar.xz' libunistring_0.9.10-1.debian.tar.xz 40328 SHA256:dd4d07437e6332003e702aa2f56911a21091ac6f10d0cdc17aaaaa8e29ad63b7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/0.9.10-1/ (for browsing the source)
- https://sources.debian.net/src/libunistring/0.9.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/0.9.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libusb-1.0=2:1.0.22-2`

Binary Packages:

- `libusb-1.0-0:amd64=2:1.0.22-2`

Licenses: (parsed from: `/usr/share/doc/libusb-1.0-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libusb-1.0=2:1.0.22-2
'http://deb.debian.org/debian/pool/main/libu/libusb-1.0/libusb-1.0_1.0.22-2.dsc' libusb-1.0_1.0.22-2.dsc 2138 SHA256:d1235e973e1da4274456807ae6a0d0079e7f7a0c8a82101639870b8e6e020cee
'http://deb.debian.org/debian/pool/main/libu/libusb-1.0/libusb-1.0_1.0.22.orig.tar.bz2' libusb-1.0_1.0.22.orig.tar.bz2 598833 SHA256:75aeb9d59a4fdb800d329a545c2e6799f732362193b465ea198f2aa275518157
'http://deb.debian.org/debian/pool/main/libu/libusb-1.0/libusb-1.0_1.0.22-2.debian.tar.xz' libusb-1.0_1.0.22-2.debian.tar.xz 12532 SHA256:286f20165bfe073ca88c1c258d197e1cf60bbf4d7e96643380f45c2c713ad85f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libusb-1.0/2:1.0.22-2/ (for browsing the source)
- https://sources.debian.net/src/libusb-1.0/2:1.0.22-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libusb-1.0/2:1.0.22-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libva=2.4.0-1`

Binary Packages:

- `libva-drm2:amd64=2.4.0-1`
- `libva-x11-2:amd64=2.4.0-1`
- `libva2:amd64=2.4.0-1`

Licenses: (parsed from: `/usr/share/doc/libva-drm2/copyright`, `/usr/share/doc/libva-x11-2/copyright`, `/usr/share/doc/libva2/copyright`)

- `Expat`
- `Expat-advertising`
- `GPL-2`
- `GPL-2+`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libva=2.4.0-1
'http://deb.debian.org/debian/pool/main/libv/libva/libva_2.4.0-1.dsc' libva_2.4.0-1.dsc 2402 SHA256:da6fb0f680121e2731581e103d19bf5b478d7df4308348383ee890a7ce118750
'http://deb.debian.org/debian/pool/main/libv/libva/libva_2.4.0.orig.tar.gz' libva_2.4.0.orig.tar.gz 223232 SHA256:67f0289944b3c39307ab0f1b7ab33de072f6e674758d2f122b51616c3d7b115b
'http://deb.debian.org/debian/pool/main/libv/libva/libva_2.4.0-1.debian.tar.xz' libva_2.4.0-1.debian.tar.xz 11220 SHA256:feef8a5b95c0936bd1184a73bbec3af7d5b3ed09bde80587cc72478b00ff517e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libva/2.4.0-1/ (for browsing the source)
- https://sources.debian.net/src/libva/2.4.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libva/2.4.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvdpau=1.1.1-10`

Binary Packages:

- `libvdpau1:amd64=1.1.1-10`

Licenses: (parsed from: `/usr/share/doc/libvdpau1/copyright`)

- `Expat`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libvdpau=1.1.1-10
'http://deb.debian.org/debian/pool/main/libv/libvdpau/libvdpau_1.1.1-10.dsc' libvdpau_1.1.1-10.dsc 2379 SHA256:76b2a3a8f72be99b90aa4895d18852aa82e25008cf7a24e0115b0601229996bf
'http://deb.debian.org/debian/pool/main/libv/libvdpau/libvdpau_1.1.1.orig.tar.bz2' libvdpau_1.1.1.orig.tar.bz2 429576 SHA256:857a01932609225b9a3a5bf222b85e39b55c08787d0ad427dbd9ec033d58d736
'http://deb.debian.org/debian/pool/main/libv/libvdpau/libvdpau_1.1.1-10.debian.tar.xz' libvdpau_1.1.1-10.debian.tar.xz 10904 SHA256:50b65aa94f4f9ce4c36232e90455917e29436dfa56a548978cf64716b4185f4a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvdpau/1.1.1-10/ (for browsing the source)
- https://sources.debian.net/src/libvdpau/1.1.1-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvdpau/1.1.1-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvidstab=1.1.0-2`

Binary Packages:

- `libvidstab1.1:amd64=1.1.0-2`

Licenses: (parsed from: `/usr/share/doc/libvidstab1.1/copyright`)

- `GPL-2`
- `GPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris libvidstab=1.1.0-2
'http://deb.debian.org/debian/pool/main/libv/libvidstab/libvidstab_1.1.0-2.dsc' libvidstab_1.1.0-2.dsc 1826 SHA256:fe500228434c80b7dc3798552a3c4023b1d086eeb18ce8d111f460e608972526
'http://deb.debian.org/debian/pool/main/libv/libvidstab/libvidstab_1.1.0.orig.tar.gz' libvidstab_1.1.0.orig.tar.gz 77736 SHA256:14d2a053e56edad4f397be0cb3ef8eb1ec3150404ce99a426c4eb641861dc0bb
'http://deb.debian.org/debian/pool/main/libv/libvidstab/libvidstab_1.1.0-2.debian.tar.xz' libvidstab_1.1.0-2.debian.tar.xz 3876 SHA256:c7a8ff87c37d68666c69f589929de5d25383f4932b6629af674c60e94f7e2ea6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvidstab/1.1.0-2/ (for browsing the source)
- https://sources.debian.net/src/libvidstab/1.1.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvidstab/1.1.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvisio=0.1.6-1`

Binary Packages:

- `libvisio-0.1-1:amd64=0.1.6-1+b2`

Licenses: (parsed from: `/usr/share/doc/libvisio-0.1-1/copyright`)

- `MIT | GPL-2`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libvisio=0.1.6-1
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.6-1.dsc' libvisio_0.1.6-1.dsc 2191 SHA256:8a11494265e7354db988de09969d8c100b5cec4fb7f859c7ef0435efc4a2485c
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.6.orig.tar.bz2' libvisio_0.1.6.orig.tar.bz2 878672 SHA256:c9262ae9797e63a8967e444fb41e4da1861c861eefd121e9e0e4f41eb72b39b9
'http://deb.debian.org/debian/pool/main/libv/libvisio/libvisio_0.1.6-1.debian.tar.xz' libvisio_0.1.6-1.debian.tar.xz 8068 SHA256:3d384600beeaef451494e9bf980453ebb443eaa2e3a5832e5aa8df7405e29a18
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvisio/0.1.6-1/ (for browsing the source)
- https://sources.debian.net/src/libvisio/0.1.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvisio/0.1.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvorbis=1.3.6-2`

Binary Packages:

- `libvorbis0a:amd64=1.3.6-2`
- `libvorbisenc2:amd64=1.3.6-2`
- `libvorbisfile3:amd64=1.3.6-2`

Licenses: (parsed from: `/usr/share/doc/libvorbis0a/copyright`, `/usr/share/doc/libvorbisenc2/copyright`, `/usr/share/doc/libvorbisfile3/copyright`)

- `BSD-3-Clause`
- `RFC-special`

Source:

```console
$ apt-get source -qq --print-uris libvorbis=1.3.6-2
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.6-2.dsc' libvorbis_1.3.6-2.dsc 2310 SHA256:bf04834eef80f0ea2369c6aaa3b399a9356275815b0a87659f208d79fdae1ef4
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.6.orig.tar.gz' libvorbis_1.3.6.orig.tar.gz 1634357 SHA256:6ed40e0241089a42c48604dc00e362beee00036af2d8b3f46338031c9e0351cb
'http://deb.debian.org/debian/pool/main/libv/libvorbis/libvorbis_1.3.6-2.debian.tar.xz' libvorbis_1.3.6-2.debian.tar.xz 12084 SHA256:5ce95b27205c2ce5e39f263da5acaa4063846377aec905ede2f64f933f3cfbf6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvorbis/1.3.6-2/ (for browsing the source)
- https://sources.debian.net/src/libvorbis/1.3.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvorbis/1.3.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libvpx=1.7.0-3+deb10u1`

Binary Packages:

- `libvpx5:amd64=1.7.0-3+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libvpx5/copyright`)

- `BSD-3-Clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libvpx=1.7.0-3+deb10u1
'http://deb.debian.org/debian/pool/main/libv/libvpx/libvpx_1.7.0-3+deb10u1.dsc' libvpx_1.7.0-3+deb10u1.dsc 2293 SHA256:1799371d542b9771b43f6dd373c40bdd31c8633b7fbcf68e8626ee179e29d098
'http://deb.debian.org/debian/pool/main/libv/libvpx/libvpx_1.7.0.orig.tar.gz' libvpx_1.7.0.orig.tar.gz 2679797 SHA256:1fec931eb5c94279ad219a5b6e0202358e94a93a90cfb1603578c326abfc1238
'http://deb.debian.org/debian/pool/main/libv/libvpx/libvpx_1.7.0-3+deb10u1.debian.tar.xz' libvpx_1.7.0-3+deb10u1.debian.tar.xz 13936 SHA256:758471f1ecbdded674c5780cef72f3b7ad354934909cfb39a3c37c618f33bbd6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libvpx/1.7.0-3+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/libvpx/1.7.0-3+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libvpx/1.7.0-3+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libwebp=0.6.1-2`

Binary Packages:

- `libwebp6:amd64=0.6.1-2`
- `libwebpmux3:amd64=0.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

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

### `dpkg` source package: `libwpd=0.10.3-1`

Binary Packages:

- `libwpd-0.10-10:amd64=0.10.3-1`
- `libwpd-tools=0.10.3-1`

Licenses: (parsed from: `/usr/share/doc/libwpd-0.10-10/copyright`, `/usr/share/doc/libwpd-tools/copyright`)

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

### `dpkg` source package: `libwps=0.4.10-1`

Binary Packages:

- `libwps-0.4-4:amd64=0.4.10-1`

Licenses: (parsed from: `/usr/share/doc/libwps-0.4-4/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwps=0.4.10-1
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.10-1.dsc' libwps_0.4.10-1.dsc 2238 SHA256:358ba1060f3ec85d6d567486309ce7f63ebdbb7c8ddf9493f57415f5b27d15de
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.10.orig.tar.xz' libwps_0.4.10.orig.tar.xz 695448 SHA256:1421e034286a9f96d3168a1c54ea570ee7aa008ca07b89de005ad5ce49fb29ca
'http://deb.debian.org/debian/pool/main/libw/libwps/libwps_0.4.10-1.debian.tar.xz' libwps_0.4.10-1.debian.tar.xz 9000 SHA256:ea804298fee7ae7641a44b997e6e0b7f32ce9228e660ff7fb739673201090bac
```

Other potentially useful URLs:

- https://sources.debian.net/src/libwps/0.4.10-1/ (for browsing the source)
- https://sources.debian.net/src/libwps/0.4.10-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libwps/0.4.10-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libx11=2:1.6.7-1`

Binary Packages:

- `libx11-6:amd64=2:1.6.7-1`
- `libx11-data=2:1.6.7-1`
- `libx11-xcb1:amd64=2:1.6.7-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.7-1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7-1.dsc' libx11_1.6.7-1.dsc 2619 SHA256:ca544ccaf4b4bf08b96ca6f3c096d3b189f437cfd5cba8edb72e75cf050f56c6
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7.orig.tar.gz' libx11_1.6.7.orig.tar.gz 2972354 SHA256:f62ab88c2a87b55e1dc338726a55bb6ed8048084fe6a3294a7ae324ca45159d1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7.orig.tar.gz.asc' libx11_1.6.7.orig.tar.gz.asc 404 SHA256:01a06afbe0574a30721d98f1c80b668ebc46410a9e8b2eb81e69b4bd8667c386
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7-1.diff.gz' libx11_1.6.7-1.diff.gz 49222 SHA256:8215096d47c997b9591daa837fcd7d3970b6a9524dca889d2a1316f9f1dc59ad
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.6.7-1/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.6.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.6.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxau=1:1.0.8-1`

Binary Packages:

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

### `dpkg` source package: `libxcb=1.13.1-2`

Binary Packages:

- `libxcb-dri2-0:amd64=1.13.1-2`
- `libxcb-dri3-0:amd64=1.13.1-2`
- `libxcb-glx0:amd64=1.13.1-2`
- `libxcb-present0:amd64=1.13.1-2`
- `libxcb-render0:amd64=1.13.1-2`
- `libxcb-shape0:amd64=1.13.1-2`
- `libxcb-shm0:amd64=1.13.1-2`
- `libxcb-sync1:amd64=1.13.1-2`
- `libxcb-xfixes0:amd64=1.13.1-2`
- `libxcb1:amd64=1.13.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.13.1-2
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.13.1-2.dsc' libxcb_1.13.1-2.dsc 5375 SHA256:08ee999e42e93af418ab27e772c7e1b464950ea2cbe8cd7ee6759e9a170dd9e8
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.13.1.orig.tar.gz' libxcb_1.13.1.orig.tar.gz 636748 SHA256:f09a76971437780a602303170fd51b5f7474051722bc39d566a272d2c4bde1b5
'http://deb.debian.org/debian/pool/main/libx/libxcb/libxcb_1.13.1-2.diff.gz' libxcb_1.13.1-2.diff.gz 25487 SHA256:8ee5244ada4bf1e9af0bbd43463877f6185d63942e89e5800613ee4a2627a016
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcb/1.13.1-2/ (for browsing the source)
- https://sources.debian.net/src/libxcb/1.13.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcb/1.13.1-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxcursor=1:1.1.15-2`

Binary Packages:

- `libxcursor1:amd64=1:1.1.15-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcursor=1:1.1.15-2
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.15-2.dsc' libxcursor_1.1.15-2.dsc 2261 SHA256:b202f32569fe210ca7565c15ba11bee9f3cfbb4f8e45416e40d843dcf507383f
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.15.orig.tar.gz' libxcursor_1.1.15.orig.tar.gz 406960 SHA256:449befea2b11dde58ba3323b2c1ec30550013bd84d80501eb56d0048e62251a1
'http://deb.debian.org/debian/pool/main/libx/libxcursor/libxcursor_1.1.15-2.debian.tar.xz' libxcursor_1.1.15-2.debian.tar.xz 8976 SHA256:7731ffa6e36651fee827cf69c7a70926ecfd29303adeb0ba75a8b9a83cf9247d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcursor/1:1.1.15-2/ (for browsing the source)
- https://sources.debian.net/src/libxcursor/1:1.1.15-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcursor/1:1.1.15-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxdamage=1:1.1.4-3`

Binary Packages:

- `libxdamage1:amd64=1:1.1.4-3+b3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdamage=1:1.1.4-3
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4-3.dsc' libxdamage_1.1.4-3.dsc 2161 SHA256:f1207d4fca942d2cddfe40abc818046e282ceeb0e0b565a44c2908fd03c41368
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4.orig.tar.gz' libxdamage_1.1.4.orig.tar.gz 339060 SHA256:4bb3e9d917f5f593df2277d452926ee6ad96de7b7cd1017cbcf4579fe5d3442b
'http://deb.debian.org/debian/pool/main/libx/libxdamage/libxdamage_1.1.4-3.debian.tar.xz' libxdamage_1.1.4-3.debian.tar.xz 5904 SHA256:94dcf3997a92f5e1b4681dcbe555af4469607ae7af2d0dc643a7a1be7b94e64a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxdamage/1:1.1.4-3/ (for browsing the source)
- https://sources.debian.net/src/libxdamage/1:1.1.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxdamage/1:1.1.4-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxkbcommon=0.8.2-1`

Binary Packages:

- `libxkbcommon0:amd64=0.8.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxkbcommon=0.8.2-1
'http://deb.debian.org/debian/pool/main/libx/libxkbcommon/libxkbcommon_0.8.2-1.dsc' libxkbcommon_0.8.2-1.dsc 2122 SHA256:053c4578baf2e236af87ed450e8621447c1468e8db51461ce960c2b3d78af1bb
'http://deb.debian.org/debian/pool/main/libx/libxkbcommon/libxkbcommon_0.8.2-1.tar.gz' libxkbcommon_0.8.2-1.tar.gz 614828 SHA256:373fb14dcc3913f894b86221d6e6473dadbc52e14c277b4b42d1af7d7fe37a1a
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxkbcommon/0.8.2-1/ (for browsing the source)
- https://sources.debian.net/src/libxkbcommon/0.8.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxkbcommon/0.8.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxml2=2.9.4+dfsg1-7`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-7+b3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.4+dfsg1-7
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-7.dsc' libxml2_2.9.4+dfsg1-7.dsc 2976 SHA256:fc4d4be13a37b03f68862afcaccbac997f6044620cbba747bb836d4bd65bed75
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA256:a74ad55e346aa0b2b41903e66d21f8f3d2a736b3f41e32496376861ab484184e
'http://deb.debian.org/debian/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-7.debian.tar.xz' libxml2_2.9.4+dfsg1-7.debian.tar.xz 36168 SHA256:403a560713d0ff32672dce6090193632c92008977dd68d88f42f8b20fb2f5601
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxml2/2.9.4+dfsg1-7/ (for browsing the source)
- https://sources.debian.net/src/libxml2/2.9.4+dfsg1-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxml2/2.9.4+dfsg1-7/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxshmfence=1.3-1`

Binary Packages:

- `libxshmfence1:amd64=1.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxshmfence=1.3-1
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.3-1.dsc' libxshmfence_1.3-1.dsc 2096 SHA256:7da3e1195622ab34427bd5d09167b1f44ed1a3e828782fa8e618f1181c56194a
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.3.orig.tar.gz' libxshmfence_1.3.orig.tar.gz 378960 SHA256:7eb3d46ad91bab444f121d475b11b39273142d090f7e9ac43e6a87f4ff5f902c
'http://deb.debian.org/debian/pool/main/libx/libxshmfence/libxshmfence_1.3-1.diff.gz' libxshmfence_1.3-1.diff.gz 17456 SHA256:85422af90300523b8fb27e697b59418f18bd7cd5c849161fd0be64c91ce94698
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxshmfence/1.3-1/ (for browsing the source)
- https://sources.debian.net/src/libxshmfence/1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxshmfence/1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxslt=1.1.32-2.2~deb10u1`

Binary Packages:

- `libxslt1.1:amd64=1.1.32-2.2~deb10u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.32-2.2~deb10u1
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.32-2.2~deb10u1.dsc' libxslt_1.1.32-2.2~deb10u1.dsc 2781 SHA256:ae3c135ea738ba088bda7dc76fb63cb68920a1fac0514aa5ff8761182d48b1f3
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.32.orig.tar.gz' libxslt_1.1.32.orig.tar.gz 3440715 SHA256:526ecd0abaf4a7789041622c3950c0e7f2c4c8835471515fd77eec684a355460
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.32.orig.tar.gz.asc' libxslt_1.1.32.orig.tar.gz.asc 455 SHA256:68b374a73747c57a17d62f0ccc1e9714f68a292e700fe4c88e3c2d9dcba71871
'http://deb.debian.org/debian/pool/main/libx/libxslt/libxslt_1.1.32-2.2~deb10u1.debian.tar.xz' libxslt_1.1.32-2.2~deb10u1.debian.tar.xz 34232 SHA256:1ac65664ec024a34da9c4180778073198868fb4ce78fb9bc936564dd61cc57e5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxslt/1.1.32-2.2~deb10u1/ (for browsing the source)
- https://sources.debian.net/src/libxslt/1.1.32-2.2~deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxslt/1.1.32-2.2~deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libzmf=0.0.2-1`

Binary Packages:

- `libzmf-0.0-0:amd64=0.0.2-1+b2`

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

### `dpkg` source package: `libzstd=1.3.8+dfsg-3`

Binary Packages:

- `libzstd1:amd64=1.3.8+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.3.8+dfsg-3
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.3.8+dfsg-3.dsc' libzstd_1.3.8+dfsg-3.dsc 2285 SHA256:d5a46f4c8ecaffac70eb8799a7a221cf8c877d830bb2803364aeb6c825afa6e3
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.3.8+dfsg.orig.tar.xz' libzstd_1.3.8+dfsg.orig.tar.xz 1299276 SHA256:03851f2c26ffbf1d43633df3f98966f3c62e698e91ef4dc90523915bc934e5f7
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.3.8+dfsg-3.debian.tar.xz' libzstd_1.3.8+dfsg-3.debian.tar.xz 10396 SHA256:392a971d6bba30b6cb3e5ff04efb10c45b052e458dfc6631ede9e024341321f9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.3.8+dfsg-3/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.3.8+dfsg-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.3.8+dfsg-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lilv=0.24.2~dfsg0-2`

Binary Packages:

- `liblilv-0-0:amd64=0.24.2~dfsg0-2`

Licenses: (parsed from: `/usr/share/doc/liblilv-0-0/copyright`)

- `BSD-3-clause`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris lilv=0.24.2~dfsg0-2
'http://deb.debian.org/debian/pool/main/l/lilv/lilv_0.24.2~dfsg0-2.dsc' lilv_0.24.2~dfsg0-2.dsc 2237 SHA256:d98573e3f03ef11f107aa1296eb08d4479d7d09dac283176c5c3ad13986aeb5f
'http://deb.debian.org/debian/pool/main/l/lilv/lilv_0.24.2~dfsg0.orig.tar.bz2' lilv_0.24.2~dfsg0.orig.tar.bz2 244405 SHA256:fc041902ed098109da4089360e2b3497a30edea4c09de4ced42cb41faba9ed0c
'http://deb.debian.org/debian/pool/main/l/lilv/lilv_0.24.2~dfsg0-2.debian.tar.xz' lilv_0.24.2~dfsg0-2.debian.tar.xz 7400 SHA256:bc105fb6e1bb0038c9f25f6b806b1c67fda90f2a2c8b17a4d8943294246f58a1
```

Other potentially useful URLs:

- https://sources.debian.net/src/lilv/0.24.2~dfsg0-2/ (for browsing the source)
- https://sources.debian.net/src/lilv/0.24.2~dfsg0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lilv/0.24.2~dfsg0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `llvm-toolchain-7=1:7.0.1-8`

Binary Packages:

- `libllvm7:amd64=1:7.0.1-8`

Licenses: (parsed from: `/usr/share/doc/libllvm7/copyright`)

- `ARM`
- `Apple`
- `BSD-3-Clause`
- `BSD-3-clause`
- `Expat`
- `LLVM`
- `MIT`
- `NCSA`
- `Polly`
- `Python`
- `U-OF-I-BSD-LIKE`
- `public-domain`
- `solar-public-domain`

Source:

```console
$ apt-get source -qq --print-uris llvm-toolchain-7=1:7.0.1-8
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1-8.dsc' llvm-toolchain-7_7.0.1-8.dsc 8253 SHA256:315347f31a2bc02c82185062bde8ad702fc6298d6eaa4bf121db3a984d9c90c4
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-clang-tools-extra.tar.bz2' llvm-toolchain-7_7.0.1.orig-clang-tools-extra.tar.bz2 954392 SHA256:5bd9a587e321536bfe93619d4260f2c6d85973c7d2212b5a29f4e6d0b081b67a
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-clang.tar.bz2' llvm-toolchain-7_7.0.1.orig-clang.tar.bz2 13927137 SHA256:78d974b2200cf18e4d711492b601ffbe104fe43682f2626b931eeb89ad4524b1
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-compiler-rt.tar.bz2' llvm-toolchain-7_7.0.1.orig-compiler-rt.tar.bz2 2364285 SHA256:58c730ee430ebf274946402098c4798e0b8b45ff0d1fa05741236e10b713c06b
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-libcxx.tar.bz2' llvm-toolchain-7_7.0.1.orig-libcxx.tar.bz2 1797541 SHA256:c54637220202040940d280e7970f1feb917fc0c951e1d4f12e7dfb4ad603ecd3
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-libcxxabi.tar.bz2' llvm-toolchain-7_7.0.1.orig-libcxxabi.tar.bz2 543991 SHA256:bac1d1855064f1f934080950bd622fa4cccb01aff98d504cbf48ae9a23d2e97e
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-lld.tar.bz2' llvm-toolchain-7_7.0.1.orig-lld.tar.bz2 996785 SHA256:d51bab2cd2dfe4e19e51f473e511fb10fe845586470bcadf01d33fb739766a40
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-lldb.tar.bz2' llvm-toolchain-7_7.0.1.orig-lldb.tar.bz2 11361330 SHA256:4ad23cd6eaf71960ad6746c469555b781e398763f383d5f6ab7d6a17f27f85f7
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-openmp.tar.bz2' llvm-toolchain-7_7.0.1.orig-openmp.tar.bz2 998026 SHA256:99cf464fcbcbfb8bbc80bde455f7a0171cb945970a4d8028ec055ffdfedb5e10
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig-polly.tar.bz2' llvm-toolchain-7_7.0.1.orig-polly.tar.bz2 3319947 SHA256:3a5f5af8efed79763d2e052e75c11e6e987377201fde54fe6f664c8c9faa6b44
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1.orig.tar.bz2' llvm-toolchain-7_7.0.1.orig.tar.bz2 33380406 SHA256:4a45763b46c2d48ab6db5347afdbba520407e9b16134e71163163a4d2a5e0980
'http://deb.debian.org/debian/pool/main/l/llvm-toolchain-7/llvm-toolchain-7_7.0.1-8.debian.tar.xz' llvm-toolchain-7_7.0.1-8.debian.tar.xz 112440 SHA256:2b728675b1d2f119433fce1d9507efc4f11b6673d38911ae0f4ec7dbd957bb62
```

Other potentially useful URLs:

- https://sources.debian.net/src/llvm-toolchain-7/1:7.0.1-8/ (for browsing the source)
- https://sources.debian.net/src/llvm-toolchain-7/1:7.0.1-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/llvm-toolchain-7/1:7.0.1-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lm-sensors=1:3.5.0-3`

Binary Packages:

- `libsensors-config=1:3.5.0-3`
- `libsensors5:amd64=1:3.5.0-3`

Licenses: (parsed from: `/usr/share/doc/libsensors-config/copyright`, `/usr/share/doc/libsensors5/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris lm-sensors=1:3.5.0-3
'http://deb.debian.org/debian/pool/main/l/lm-sensors/lm-sensors_3.5.0-3.dsc' lm-sensors_3.5.0-3.dsc 1998 SHA256:5f4ff4b1d99df17f0fc422a94915965b9c38222a89cccf5cb1736096516c84b8
'http://deb.debian.org/debian/pool/main/l/lm-sensors/lm-sensors_3.5.0.orig.tar.gz' lm-sensors_3.5.0.orig.tar.gz 267133 SHA256:f671c1d63a4cd8581b3a4a775fd7864a740b15ad046fe92038bcff5c5134d7e0
'http://deb.debian.org/debian/pool/main/l/lm-sensors/lm-sensors_3.5.0-3.debian.tar.xz' lm-sensors_3.5.0-3.debian.tar.xz 26348 SHA256:d09e3f9c5d83499cc7bb924c66061cec58b9f256f67cfb40022fd2f24faab486
```

Other potentially useful URLs:

- https://sources.debian.net/src/lm-sensors/1:3.5.0-3/ (for browsing the source)
- https://sources.debian.net/src/lm-sensors/1:3.5.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lm-sensors/1:3.5.0-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `lsb=10.2019051400`

Binary Packages:

- `lsb-base=10.2019051400`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=10.2019051400
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_10.2019051400.dsc' lsb_10.2019051400.dsc 1695 SHA256:79be4b76a50edb2e2f0fb0f2301d74aa36be7e4ed1aedc2cb92e0ca93a97e194
'http://deb.debian.org/debian/pool/main/l/lsb/lsb_10.2019051400.tar.xz' lsb_10.2019051400.tar.xz 42204 SHA256:e134c5780b70e3aac9d175e70bee4eb187e01bc02bb0d4e8a9b19dc52aabd557
```

Other potentially useful URLs:

- https://sources.debian.net/src/lsb/10.2019051400/ (for browsing the source)
- https://sources.debian.net/src/lsb/10.2019051400/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lsb/10.2019051400/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lvm2=2.03.02-3`

Binary Packages:

- `dmsetup=2:1.02.155-3`
- `libdevmapper1.02.1:amd64=2:1.02.155-3`

Licenses: (parsed from: `/usr/share/doc/dmsetup/copyright`, `/usr/share/doc/libdevmapper1.02.1/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris lvm2=2.03.02-3
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.03.02-3.dsc' lvm2_2.03.02-3.dsc 2660 SHA256:0d04f20d1900444e110527a286b8268308d53128cad2c17d9e2d5a22871d8547
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.03.02.orig.tar.gz' lvm2_2.03.02.orig.tar.gz 2361046 SHA256:550ba750239fd75b7e52c9877565cabffef506bbf6d7f6f17b9700dee56c720f
'http://deb.debian.org/debian/pool/main/l/lvm2/lvm2_2.03.02-3.debian.tar.xz' lvm2_2.03.02-3.debian.tar.xz 32340 SHA256:964096b890ba97231a9652d389fcd1cc258775e9045582e49670781084aceb9a
```

Other potentially useful URLs:

- https://sources.debian.net/src/lvm2/2.03.02-3/ (for browsing the source)
- https://sources.debian.net/src/lvm2/2.03.02-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lvm2/2.03.02-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lz4=1.8.3-1`

Binary Packages:

- `liblz4-1:amd64=1.8.3-1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.8.3-1
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.8.3-1.dsc' lz4_1.8.3-1.dsc 1932 SHA256:fed178383bc99451256cedf0d39731d106f70103125c043e4ef7112a642190b5
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.8.3.orig.tar.gz' lz4_1.8.3.orig.tar.gz 327897 SHA256:33af5936ac06536805f9745e0b6d61da606a1f8b4cc5c04dd3cbaca3b9b4fc43
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.8.3-1.debian.tar.xz' lz4_1.8.3-1.debian.tar.xz 11336 SHA256:e98f02ec04236c616ea003d0a0e50818b2a959436fcd833ba1bcfc14664ab156
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.8.3-1/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.8.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.8.3-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mercurial=4.8.2-1+deb10u1`

Binary Packages:

- `mercurial=4.8.2-1+deb10u1`
- `mercurial-common=4.8.2-1+deb10u1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=4.8.2-1+deb10u1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_4.8.2-1+deb10u1.dsc' mercurial_4.8.2-1+deb10u1.dsc 2709 SHA256:e47f77a1f9555e4648e3331100318853dc81215531a18c41f731d93383038df1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_4.8.2.orig.tar.gz' mercurial_4.8.2.orig.tar.gz 6870985 SHA256:6c202cb9cf05e63b86477ebf84d6475eb10b4022ac2cd3a7481fb36d9c45fdb2
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_4.8.2.orig.tar.gz.asc' mercurial_4.8.2.orig.tar.gz.asc 833 SHA256:ceaf75242740acfd06a96aae53d8a40f3b3f3c4a7119bb53224d0bf6efa65254
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_4.8.2-1+deb10u1.debian.tar.xz' mercurial_4.8.2-1+deb10u1.debian.tar.xz 64940 SHA256:5673d16057e140b74c0939e509a15dc4b67e18ee71cf806e9940896a42c9130c
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/4.8.2-1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/mercurial/4.8.2-1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/4.8.2-1+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mesa=18.3.6-2+deb10u1`

Binary Packages:

- `libgl1-mesa-dri:amd64=18.3.6-2+deb10u1`
- `libglapi-mesa:amd64=18.3.6-2+deb10u1`
- `libglx-mesa0:amd64=18.3.6-2+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libgl1-mesa-dri/copyright`, `/usr/share/doc/libglapi-mesa/copyright`, `/usr/share/doc/libglx-mesa0/copyright`)

- `Apache-2.0`
- `BSD`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSL`
- `GPL`
- `Khronos`
- `MIT`
- `MLAA`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris mesa=18.3.6-2+deb10u1
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_18.3.6-2+deb10u1.dsc' mesa_18.3.6-2+deb10u1.dsc 5172 SHA256:6170d13614b38d58d40c04b17b28920f701cf79f240c2b7dd384599289d7d89e
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_18.3.6.orig.tar.gz' mesa_18.3.6.orig.tar.gz 20348664 SHA256:4619d92afadf7072f7956599a2ccd0934fc45b4ddbc2eb865bdcb50ddf963f87
'http://deb.debian.org/debian/pool/main/m/mesa/mesa_18.3.6-2+deb10u1.diff.gz' mesa_18.3.6-2+deb10u1.diff.gz 105356 SHA256:f0fedac93bb9aca2248c7c676885f967516ccd87c4a3ce5c81918254fa9d273d
```

Other potentially useful URLs:

- https://sources.debian.net/src/mesa/18.3.6-2+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/mesa/18.3.6-2+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mesa/18.3.6-2+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mhash=0.9.9.9-7`

Binary Packages:

- `libmhash2:amd64=0.9.9.9-7+b1`

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

### `dpkg` source package: `mime-support=3.62`

Binary Packages:

- `mime-support=3.62`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.62
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.62.dsc' mime-support_3.62.dsc 1576 SHA256:62195cb653122db4571f97a32aaaa93e558dacf15563b061e8e1f24f6ce1b52b
'http://deb.debian.org/debian/pool/main/m/mime-support/mime-support_3.62.tar.gz' mime-support_3.62.tar.gz 37130 SHA256:54e0a03e0cd63c7c9fe68a18ead0a2143fd3c327604215f989d85484d0409f4a
```

Other potentially useful URLs:

- https://sources.debian.net/src/mime-support/3.62/ (for browsing the source)
- https://sources.debian.net/src/mime-support/3.62/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mime-support/3.62/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpdecimal=2.4.2-2`

Binary Packages:

- `libmpdec2:amd64=2.4.2-2`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-2
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.2-2.dsc' mpdecimal_2.4.2-2.dsc 1932 SHA256:716e61fc8315a22804adf8403e4d332c1883235b5c3801b6769e6040dc962fe3
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.4.2-2.debian.tar.xz' mpdecimal_2.4.2-2.debian.tar.xz 5256 SHA256:159113f11169afc675a431840792e1ed8c2d00438bf3e1c5a3eb2c17d9e8da3d
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpdecimal/2.4.2-2/ (for browsing the source)
- https://sources.debian.net/src/mpdecimal/2.4.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpdecimal/2.4.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpg123=1.25.10-2`

Binary Packages:

- `libmpg123-0:amd64=1.25.10-2`

Licenses: (parsed from: `/usr/share/doc/libmpg123-0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpg123=1.25.10-2
'http://deb.debian.org/debian/pool/main/m/mpg123/mpg123_1.25.10-2.dsc' mpg123_1.25.10-2.dsc 2306 SHA256:5e10443e1a471e89dafa663bbe4e914b5ddd1df51cba1f9044f1625921c576a7
'http://deb.debian.org/debian/pool/main/m/mpg123/mpg123_1.25.10.orig.tar.bz2' mpg123_1.25.10.orig.tar.bz2 921219 SHA256:6c1337aee2e4bf993299851c70b7db11faec785303cfca3a5c3eb5f329ba7023
'http://deb.debian.org/debian/pool/main/m/mpg123/mpg123_1.25.10-2.debian.tar.xz' mpg123_1.25.10-2.debian.tar.xz 23596 SHA256:a55b8c7ffd3b3cf8491dc0398af45125ffb8d3b9f491d096fa8087cae0e3efa3
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpg123/1.25.10-2/ (for browsing the source)
- https://sources.debian.net/src/mpg123/1.25.10-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpg123/1.25.10-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ncurses=6.1+20181013-2+deb10u2`

Binary Packages:

- `libncurses6:amd64=6.1+20181013-2+deb10u2`
- `libncursesw6:amd64=6.1+20181013-2+deb10u2`
- `libtinfo6:amd64=6.1+20181013-2+deb10u2`
- `ncurses-base=6.1+20181013-2+deb10u2`
- `ncurses-bin=6.1+20181013-2+deb10u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1+20181013-2+deb10u2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20181013-2+deb10u2.dsc' ncurses_6.1+20181013-2+deb10u2.dsc 4179 SHA256:8318631ff3298951a93d6dd6c20bd47c9e5fdaaf30578d541bd6404bdd5317ea
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20181013.orig.tar.gz' ncurses_6.1+20181013.orig.tar.gz 3411288 SHA256:aeb1d098ee90b39a763b57b00da19ff5bbb573dea077f98fbd85d59444bb3b59
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20181013.orig.tar.gz.asc' ncurses_6.1+20181013.orig.tar.gz.asc 251 SHA256:865931406e519909a4d0ab87b14d0c6d3ebccb7b3e0dac5c6095f0dfce5e14cf
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.1+20181013-2+deb10u2.debian.tar.xz' ncurses_6.1+20181013-2+deb10u2.debian.tar.xz 61664 SHA256:4574ec11ce2577e76f30f8d40cc2a9ebf94d8208f47247021da88b7b09e77df9
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.1+20181013-2+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.1+20181013-2+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.1+20181013-2+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `neon27=0.30.2-3`

Binary Packages:

- `libneon27-gnutls:amd64=0.30.2-3`

Licenses: (parsed from: `/usr/share/doc/libneon27-gnutls/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris neon27=0.30.2-3
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.2-3.dsc' neon27_0.30.2-3.dsc 2161 SHA256:32774ff23c38851c28be38b80779ebaa698e7822ed34e3db5ef86d5c5c905f4a
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.2.orig.tar.gz' neon27_0.30.2.orig.tar.gz 932779 SHA256:db0bd8cdec329b48f53a6f00199c92d5ba40b0f015b153718d1b15d3d967fbca
'http://deb.debian.org/debian/pool/main/n/neon27/neon27_0.30.2-3.debian.tar.xz' neon27_0.30.2-3.debian.tar.xz 12532 SHA256:e3c46a5858c1167d373df0d7b1e11c2360696873aa423c88ae10dc8d29191aba
```

Other potentially useful URLs:

- https://sources.debian.net/src/neon27/0.30.2-3/ (for browsing the source)
- https://sources.debian.net/src/neon27/0.30.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/neon27/0.30.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `netbase=5.6`

Binary Packages:

- `netbase=5.6`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.6
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.6.dsc' netbase_5.6.dsc 1306 SHA256:fea82cc64b508a8f5ff3a16dfadce1660468d0a347df5c0ff56a2caaa57668a6
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_5.6.tar.xz' netbase_5.6.tar.xz 31684 SHA256:5d93a099deb28869b7306e914700fafbd293b55bdb5df05a5aa6effd0af5930c
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/5.6/ (for browsing the source)
- https://sources.debian.net/src/netbase/5.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/5.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.4.1-1`

Binary Packages:

- `libhogweed4:amd64=3.4.1-1`
- `libnettle6:amd64=3.4.1-1`

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
$ apt-get source -qq --print-uris nettle=3.4.1-1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4.1-1.dsc' nettle_3.4.1-1.dsc 2258 SHA256:829d6f504938a22a704042211fe351f2e27c52d3811f42c508e95421a9c634fb
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4.1.orig.tar.gz' nettle_3.4.1.orig.tar.gz 1947053 SHA256:f941cf1535cd5d1819be5ccae5babef01f6db611f9b5a777bae9c7604b8a92ad
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4.1.orig.tar.gz.asc' nettle_3.4.1.orig.tar.gz.asc 2476 SHA256:07b265366b46bc67950da3f34687235eaa85c45b326e42bb7c9b58830b651d28
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.4.1-1.debian.tar.xz' nettle_3.4.1-1.debian.tar.xz 19988 SHA256:0339933966853cc0c3b2a9721f44116ee31d136d9983d33275d1beb291c11edb
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.4.1-1/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.4.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.4.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nghttp2=1.36.0-2+deb10u1`

Binary Packages:

- `libnghttp2-14:amd64=1.36.0-2+deb10u1`

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
$ apt-get source -qq --print-uris nghttp2=1.36.0-2+deb10u1
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.36.0-2+deb10u1.dsc' nghttp2_1.36.0-2+deb10u1.dsc 2601 SHA256:3712e7cbb20d1b43f8f7a9c5408b79bd80e4c3c0cb2d4ad68062d367b1715fd6
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.36.0.orig.tar.bz2' nghttp2_1.36.0.orig.tar.bz2 1919021 SHA256:16a734d7414062911e23989e243ca76e7722cb3c60273723e3e3ae4c21e71ceb
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.36.0-2+deb10u1.debian.tar.xz' nghttp2_1.36.0-2+deb10u1.debian.tar.xz 13132 SHA256:f4fb4dd2385d158efba2ec3d3ce1b13c24ecb05c75f353f370f7cb0f080c7537
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.36.0-2+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.36.0-2+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.36.0-2+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `norm=1.5.8+dfsg2-1`

Binary Packages:

- `libnorm1:amd64=1.5.8+dfsg2-1`

Licenses: (parsed from: `/usr/share/doc/libnorm1/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause-UC`
- `NRL-2-clause`
- `NRL-3-clause`

Source:

```console
$ apt-get source -qq --print-uris norm=1.5.8+dfsg2-1
'http://deb.debian.org/debian/pool/main/n/norm/norm_1.5.8+dfsg2-1.dsc' norm_1.5.8+dfsg2-1.dsc 1559 SHA256:22fd2c4b8e732c43639f2f817f0c6a24981020a5ecfc76230b6e6005f6891d88
'http://deb.debian.org/debian/pool/main/n/norm/norm_1.5.8+dfsg2.orig.tar.gz' norm_1.5.8+dfsg2.orig.tar.gz 2320548 SHA256:31cde2ef09da189c8ad168cd68c53119ce9e0e56e0de7e37c2e37c81f4c6347d
'http://deb.debian.org/debian/pool/main/n/norm/norm_1.5.8+dfsg2-1.debian.tar.xz' norm_1.5.8+dfsg2-1.debian.tar.xz 6696 SHA256:0d500a111a878d7c5fc3dbc0d9c64d1248a02ffe776dd013b53f7609aee7904a
```

Other potentially useful URLs:

- https://sources.debian.net/src/norm/1.5.8+dfsg2-1/ (for browsing the source)
- https://sources.debian.net/src/norm/1.5.8+dfsg2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/norm/1.5.8+dfsg2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `nspr=2:4.20-1`

Binary Packages:

- `libnspr4:amd64=2:4.20-1`

Licenses: (parsed from: `/usr/share/doc/libnspr4/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.20-1
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.20-1.dsc' nspr_4.20-1.dsc 1988 SHA256:ab98e6f90a634ca5aaafb0e10ae4672da2f5b3b29176831d5b9ced7bd339422e
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.20.orig.tar.gz' nspr_4.20.orig.tar.gz 1140892 SHA256:2c8964913da89ffbaf464d49ce44d79e8804e1794ef9a8c52a7bff7224d1556e
'http://deb.debian.org/debian/pool/main/n/nspr/nspr_4.20-1.debian.tar.xz' nspr_4.20-1.debian.tar.xz 10568 SHA256:5b06cb375a8ca203a52b68dd8dd1e57f91d27fc407f88bf2c013f45291aa99df
```

Other potentially useful URLs:

- https://sources.debian.net/src/nspr/2:4.20-1/ (for browsing the source)
- https://sources.debian.net/src/nspr/2:4.20-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nspr/2:4.20-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nss=2:3.42.1-1+deb10u2`

Binary Packages:

- `libnss3:amd64=2:3.42.1-1+deb10u2`

Licenses: (parsed from: `/usr/share/doc/libnss3/copyright`)

- `BSD-3`
- `MIT`
- `MPL-2.0`
- `Zlib`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nss=2:3.42.1-1+deb10u2
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.42.1-1+deb10u2.dsc' nss_3.42.1-1+deb10u2.dsc 2192 SHA256:250588dbf5f41ad73bd58783173e7e04af5ded0022d7689f602d721c6d63e2aa
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.42.1.orig.tar.gz' nss_3.42.1.orig.tar.gz 23416408 SHA256:087db37d38fd49dfd584dd2a8b5baa7fc88de7c9bd97c0c2d5be4abcafc61fc6
'http://deb.debian.org/debian/pool/main/n/nss/nss_3.42.1-1+deb10u2.debian.tar.xz' nss_3.42.1-1+deb10u2.debian.tar.xz 25984 SHA256:da8c24a005ed9ebba0c9b3a69cfe7cfbd3717931d93b8e77b1ba812e2b8d1b78
```

Other potentially useful URLs:

- https://sources.debian.net/src/nss/2:3.42.1-1+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/nss/2:3.42.1-1+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nss/2:3.42.1-1+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `numactl=2.0.12-1`

Binary Packages:

- `libnuma1:amd64=2.0.12-1`

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

### `dpkg` source package: `openal-soft=1:1.19.1-1`

Binary Packages:

- `libopenal-data=1:1.19.1-1`
- `libopenal1:amd64=1:1.19.1-1`

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
$ apt-get source -qq --print-uris openal-soft=1:1.19.1-1
'http://deb.debian.org/debian/pool/main/o/openal-soft/openal-soft_1.19.1-1.dsc' openal-soft_1.19.1-1.dsc 2524 SHA256:1ba42d3f53a4b394d1c7077b1281dfd4c8d10b1435c889d7033cd90e468468f4
'http://deb.debian.org/debian/pool/main/o/openal-soft/openal-soft_1.19.1.orig.tar.gz' openal-soft_1.19.1.orig.tar.gz 683061 SHA256:9f3536ab2bb7781dbafabc6a61e0b34b17edd16bd6c2eaf2ae71bc63078f98c7
'http://deb.debian.org/debian/pool/main/o/openal-soft/openal-soft_1.19.1-1.debian.tar.xz' openal-soft_1.19.1-1.debian.tar.xz 12768 SHA256:6bb1a5c6dbfdc02e5ff1d0eca00c7f2af43ca1be532424513cea20726ad48646
```

Other potentially useful URLs:

- https://sources.debian.net/src/openal-soft/1:1.19.1-1/ (for browsing the source)
- https://sources.debian.net/src/openal-soft/1:1.19.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openal-soft/1:1.19.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openjpeg2=2.3.0-2+deb10u1`

Binary Packages:

- `libopenjp2-7:amd64=2.3.0-2+deb10u1`

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
$ apt-get source -qq --print-uris openjpeg2=2.3.0-2+deb10u1
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.3.0-2+deb10u1.dsc' openjpeg2_2.3.0-2+deb10u1.dsc 2590 SHA256:a8b1faaf14416687c5cf25bb95662ab4c9e2e552069c226666e685d5fa6cc212
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.3.0.orig.tar.gz' openjpeg2_2.3.0.orig.tar.gz 2074456 SHA256:fd5ca8cf3f195b0a54c56193c5897bb423c00db577afda4033318006769a5833
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.3.0-2+deb10u1.debian.tar.xz' openjpeg2_2.3.0-2+deb10u1.debian.tar.xz 21984 SHA256:9ba5f95157fc8f861ee5bae029ee2956e837e29a701e0212dc7b6bf6c256c707
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjpeg2/2.3.0-2+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/openjpeg2/2.3.0-2+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjpeg2/2.3.0-2+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.47+dfsg-3+deb10u1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.47+dfsg-3+deb10u1`
- `libldap-common=2.4.47+dfsg-3+deb10u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.47+dfsg-3+deb10u1
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.47+dfsg-3+deb10u1.dsc' openldap_2.4.47+dfsg-3+deb10u1.dsc 2888 SHA256:ff503d526d22d0301ff34b0009023d00419e7744a3d7a9048cad07698e94b1bf
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.47+dfsg.orig.tar.gz' openldap_2.4.47+dfsg.orig.tar.gz 4872293 SHA256:8f1ac7a4be7dd8ef158361efbfe16509756d3d9b396f5f378c3cf5c727807651
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.47+dfsg-3+deb10u1.debian.tar.xz' openldap_2.4.47+dfsg-3+deb10u1.debian.tar.xz 167928 SHA256:9dbde8632c9eb32f6282f0b37e9849a5a3a8d69b8bd9571d215230923ec5607d
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.47+dfsg-3+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.47+dfsg-3+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.47+dfsg-3+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:7.9p1-10+deb10u2`

Binary Packages:

- `openssh-client=1:7.9p1-10+deb10u2`

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
$ apt-get source -qq --print-uris openssh=1:7.9p1-10+deb10u2
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.9p1-10+deb10u2.dsc' openssh_7.9p1-10+deb10u2.dsc 3321 SHA256:bb8384534491eb1edba6c12a2d4f289e59abb4ec4795101d9655fae52e426dec
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.9p1.orig.tar.gz' openssh_7.9p1.orig.tar.gz 1565384 SHA256:6b4b3ba2253d84ed3771c8050728d597c91cfce898713beb7b64a305b6f11aad
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.9p1.orig.tar.gz.asc' openssh_7.9p1.orig.tar.gz.asc 683 SHA256:4fd584498595450d68f5514b3d79eb14425a3d6aa9e9021d9e928fdd7b4469eb
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_7.9p1-10+deb10u2.debian.tar.xz' openssh_7.9p1-10+deb10u2.debian.tar.xz 174016 SHA256:2f8d81757e3050aab4ab735692c1b2d521cee54ec3987ef3b08fbaff84abf3c1
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:7.9p1-10+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:7.9p1-10+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:7.9p1-10+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.1d-0+deb10u2`

Binary Packages:

- `libssl1.1:amd64=1.1.1d-0+deb10u2`
- `openssl=1.1.1d-0+deb10u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1d-0+deb10u2
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d-0+deb10u2.dsc' openssl_1.1.1d-0+deb10u2.dsc 2472 SHA256:cfeb4085016d29b14c2e0b1c204fd95a6fe20be3c12b669b8b0d6553eb2108a9
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d.orig.tar.gz' openssl_1.1.1d.orig.tar.gz 8845861 SHA256:1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d.orig.tar.gz.asc' openssl_1.1.1d.orig.tar.gz.asc 488 SHA256:f3fd3299a79421fffd51d35f62636b8e987dab1d3033d93a19d7685868e15395
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d-0+deb10u2.debian.tar.xz' openssl_1.1.1d-0+deb10u2.debian.tar.xz 84848 SHA256:418f08b2182c54bad5f049d8b17433055e146c84c793794ebca3d74231b53389
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.1d-0+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.1d-0+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.1d-0+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `opus=1.3-1`

Binary Packages:

- `libopus0:amd64=1.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris opus=1.3-1
'http://deb.debian.org/debian/pool/main/o/opus/opus_1.3-1.dsc' opus_1.3-1.dsc 1908 SHA256:348b90a6280d171324f061764d91f6b01f4830a5f2bbc9eabf8d8c3426564de0
'http://deb.debian.org/debian/pool/main/o/opus/opus_1.3.orig.tar.gz' opus_1.3.orig.tar.gz 1070384 SHA256:be838dbf1510246a94d063e7bcfe30f5d1c269718a5b77b6e47e21e48e2b5647
'http://deb.debian.org/debian/pool/main/o/opus/opus_1.3-1.diff.gz' opus_1.3-1.diff.gz 8758 SHA256:721379b4485517cd63a613d2d209900faa79bc68d9e6e7b9e310c9bcc7013036
```

Other potentially useful URLs:

- https://sources.debian.net/src/opus/1.3-1/ (for browsing the source)
- https://sources.debian.net/src/opus/1.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/opus/1.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `orc=1:0.4.28-3.1`

Binary Packages:

- `liborc-0.4-0:amd64=1:0.4.28-3.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris orc=1:0.4.28-3.1
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.28-3.1.dsc' orc_0.4.28-3.1.dsc 2233 SHA256:683ee13c0ddb2e38bdb422c0c0e8ca91f70baad4cdc4363861aa2d6b9be66ba5
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.28.orig.tar.xz' orc_0.4.28.orig.tar.xz 469460 SHA256:bfcd7c6563b05672386c4eedfc4c0d4a0a12b4b4775b74ec6deb88fc2bcd83ce
'http://deb.debian.org/debian/pool/main/o/orc/orc_0.4.28-3.1.debian.tar.xz' orc_0.4.28-3.1.debian.tar.xz 6964 SHA256:e8583f484c0732741fda4eeb90030ac147fd9480fc00aafd84480aa3b2d432e5
```

Other potentially useful URLs:

- https://sources.debian.net/src/orc/1:0.4.28-3.1/ (for browsing the source)
- https://sources.debian.net/src/orc/1:0.4.28-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/orc/1:0.4.28-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.15-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.15-2`
- `p11-kit=0.23.15-2`
- `p11-kit-modules:amd64=0.23.15-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`, `/usr/share/doc/p11-kit/copyright`, `/usr/share/doc/p11-kit-modules/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.15-2
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.15-2.dsc' p11-kit_0.23.15-2.dsc 2420 SHA256:c4a856c207f95510c5ba978394cf3c2e3867c1e857e965f89c321515844fe52c
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.15.orig.tar.gz' p11-kit_0.23.15.orig.tar.gz 1276733 SHA256:f7c139a0c77a1f0012619003e542060ba8f94799a0ef463026db390680e4d798
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.15.orig.tar.gz.asc' p11-kit_0.23.15.orig.tar.gz.asc 879 SHA256:e28bd948178e2f91e18fbb4387d7b6532aa44eb92ac4c67a6485bc9cd9c79db8
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.23.15-2.debian.tar.xz' p11-kit_0.23.15-2.debian.tar.xz 22820 SHA256:878675cf4c1e73c2d53960ca9e6e558470acb64aad9ad5b55dc556e90e80bf8e
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.23.15-2/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.23.15-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.23.15-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `pango1.0=1.42.4-7~deb10u1`

Binary Packages:

- `libpango-1.0-0:amd64=1.42.4-7~deb10u1`
- `libpangocairo-1.0-0:amd64=1.42.4-7~deb10u1`
- `libpangoft2-1.0-0:amd64=1.42.4-7~deb10u1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Example`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.42.4-7~deb10u1
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.42.4-7~deb10u1.dsc' pango1.0_1.42.4-7~deb10u1.dsc 3301 SHA256:48cb653f7a82d8127192e71ca644544f94bac7f882565f40f74b5dbe74c3d00e
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.42.4.orig.tar.xz' pango1.0_1.42.4.orig.tar.xz 833876 SHA256:1d2b74cd63e8bd41961f2f8d952355aa0f9be6002b52c8aa7699d9f5da597c9d
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.42.4-7~deb10u1.debian.tar.xz' pango1.0_1.42.4-7~deb10u1.debian.tar.xz 50480 SHA256:ceb9b2f2b01b8ab0f46f73078f04ea57805d8106de4369a13b507cba74034d6e
```

Other potentially useful URLs:

- https://sources.debian.net/src/pango1.0/1.42.4-7~deb10u1/ (for browsing the source)
- https://sources.debian.net/src/pango1.0/1.42.4-7~deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pango1.0/1.42.4-7~deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.32-5`

Binary Packages:

- `libpcre2-8-0:amd64=10.32-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.32-5
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.32-5.dsc' pcre2_10.32-5.dsc 2342 SHA256:df327f59608e018603b138cf5a557fe5febfa5f24281152d68f3a52ba542d504
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.32.orig.tar.gz' pcre2_10.32.orig.tar.gz 2169349 SHA256:9ca9be72e1a04f22be308323caa8c06ebd0c51efe99ee11278186cafbc4fe3af
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.32-5.diff.gz' pcre2_10.32-5.diff.gz 5187 SHA256:bfe23d2661bf5727a10a1c1e49660c35afc0a4ad1c151bdcefb7c5a52e71e685
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.32-5/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.32-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.32-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre3=2:8.39-12`

Binary Packages:

- `libpcre3:amd64=2:8.39-12`

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

### `dpkg` source package: `perl=5.28.1-6`

Binary Packages:

- `libperl5.28:amd64=5.28.1-6`
- `perl=5.28.1-6`
- `perl-base=5.28.1-6`
- `perl-modules-5.28=5.28.1-6`

Licenses: (parsed from: `/usr/share/doc/libperl5.28/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.28/copyright`)

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
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.28.1-6
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1-6.dsc' perl_5.28.1-6.dsc 2835 SHA256:3af8a65b216c6aadf9093d979c25eb48f6f2b3286264a3f1f65ccefcc9fc653c
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1.orig-regen-configure.tar.xz' perl_5.28.1.orig-regen-configure.tar.xz 411944 SHA256:5873b81af4514d3910ab1a8267b15ff8c0e2100dbae4edfd10b65ef72cd31ef8
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1.orig.tar.xz' perl_5.28.1.orig.tar.xz 12372080 SHA256:fea7162d4cca940a387f0587b93f6737d884bf74d8a9d7cfd978bc12cd0b202d
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1-6.debian.tar.xz' perl_5.28.1-6.debian.tar.xz 178708 SHA256:59a3fd93229c9ca1a1f8a4692eb768f16444494e6bf0d454ea27de5f5a1655cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.28.1-6/ (for browsing the source)
- https://sources.debian.net/src/perl/5.28.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.28.1-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.1.0-2`

Binary Packages:

- `pinentry-curses=1.1.0-2`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-2
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-2.dsc' pinentry_1.1.0-2.dsc 2055 SHA256:a3f157d367217eb91581d9fc53f23205794c7572894497a04d4d91eb6d5aff06
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.1.0-2.debian.tar.xz' pinentry_1.1.0-2.debian.tar.xz 16480 SHA256:b09437607c63c620bb581fe14080e897b5fb8210d08611b18b751efead7776da
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.1.0-2/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.1.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.1.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pixman=0.36.0-1`

Binary Packages:

- `libpixman-1-0:amd64=0.36.0-1`

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

### `dpkg` source package: `poppler-data=0.4.9-2`

Binary Packages:

- `poppler-data=0.4.9-2`

Licenses: (parsed from: `/usr/share/doc/poppler-data/copyright`)

- `AGPL-3+`
- `BSD-3-cluase`
- `GPL-2`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris poppler-data=0.4.9-2
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.9-2.dsc' poppler-data_0.4.9-2.dsc 2456 SHA256:da4b19cc39f2b0d767dfd500c04949db7aa2139324c4e0d3278ed86d3edcfde5
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.9.orig-ai0.tar.gz' poppler-data_0.4.9.orig-ai0.tar.gz 3515 SHA256:755a3a7cec6019b7cb6a7ac89828820e90d5105e66ebc2a7aacecacfb3ed4f1d
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.9.orig-from-ghostscript.tar.xz' poppler-data_0.4.9.orig-from-ghostscript.tar.xz 2320 SHA256:5070e1f3645080c809d80c42ee2e736648fe37bc2a68c3f54d1f9fce01086215
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.9.orig.tar.gz' poppler-data_0.4.9.orig.tar.gz 4196919 SHA256:1f9c7e7de9ecd0db6ab287349e31bf815ca108a5a175cf906a90163bdbe32012
'http://deb.debian.org/debian/pool/main/p/poppler-data/poppler-data_0.4.9-2.debian.tar.xz' poppler-data_0.4.9-2.debian.tar.xz 19504 SHA256:300792a153c1bfcf2413807875e333c7ba31a30a71f64d97bca58de307589d70
```

Other potentially useful URLs:

- https://sources.debian.net/src/poppler-data/0.4.9-2/ (for browsing the source)
- https://sources.debian.net/src/poppler-data/0.4.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/poppler-data/0.4.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `poppler=0.71.0-5`

Binary Packages:

- `libpoppler82:amd64=0.71.0-5`
- `poppler-utils=0.71.0-5`

Licenses: (parsed from: `/usr/share/doc/libpoppler82/copyright`, `/usr/share/doc/poppler-utils/copyright`)

- `Apache-2.0`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris poppler=0.71.0-5
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_0.71.0-5.dsc' poppler_0.71.0-5.dsc 3290 SHA256:4d6ade0a08aea864c8f5beb1e621cf04b68237064352b7dc4162a75abb45866e
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_0.71.0.orig.tar.xz' poppler_0.71.0.orig.tar.xz 1480852 SHA256:badbecd2dddf63352fd85ec08a9c2ed122fdadacf2a34fcb4cc227c4d01f2cf9
'http://deb.debian.org/debian/pool/main/p/poppler/poppler_0.71.0-5.debian.tar.xz' poppler_0.71.0-5.debian.tar.xz 39792 SHA256:0e70d8bcd9deb7ff07e998aa5541ea6a95ade8fd1aac9bdbdae02a0585eb6757
```

Other potentially useful URLs:

- https://sources.debian.net/src/poppler/0.71.0-5/ (for browsing the source)
- https://sources.debian.net/src/poppler/0.71.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/poppler/0.71.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.15-2`

Binary Packages:

- `libprocps7:amd64=2:3.3.15-2`
- `procps=2:3.3.15-2`

Licenses: (parsed from: `/usr/share/doc/libprocps7/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.15-2
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.15-2.dsc' procps_3.3.15-2.dsc 2104 SHA256:c7f695ddba2fdf0c3b9de5c38de22713a7046dd9e4a141d59155f4dd62008b32
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.15.orig.tar.xz' procps_3.3.15.orig.tar.xz 903372 SHA256:82e8aa55b65eac116eee05f00d2a884a6374760d57100edd429d6e9b4953458d
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.15-2.debian.tar.xz' procps_3.3.15-2.debian.tar.xz 28060 SHA256:4e90c4129744b726929990239139fde29ab4e438d65d75f5d4c479ead2001aed
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.15-2/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.15-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.15-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pulseaudio=12.2-4+deb10u1`

Binary Packages:

- `libpulse0:amd64=12.2-4+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libpulse0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris pulseaudio=12.2-4+deb10u1
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_12.2-4+deb10u1.dsc' pulseaudio_12.2-4+deb10u1.dsc 3749 SHA256:737ed45fa8bafc03f71bccd2033ba69bafe778f2073109383be62d80ab212c0b
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_12.2.orig.tar.xz' pulseaudio_12.2.orig.tar.xz 1665092 SHA256:809668ffc296043779c984f53461c2b3987a45b7a25eb2f0a1d11d9f23ba4055
'http://deb.debian.org/debian/pool/main/p/pulseaudio/pulseaudio_12.2-4+deb10u1.debian.tar.xz' pulseaudio_12.2-4+deb10u1.debian.tar.xz 35364 SHA256:60ce8abc0f2352123501b8e8eddd30bf31c78d95dcb1e474fc5beecdd139ad87
```

Other potentially useful URLs:

- https://sources.debian.net/src/pulseaudio/12.2-4+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/pulseaudio/12.2-4+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pulseaudio/12.2-4+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pwgen=2.08-1`

Binary Packages:

- `pwgen=2.08-1`

Licenses: (parsed from: `/usr/share/doc/pwgen/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris pwgen=2.08-1
'http://deb.debian.org/debian/pool/main/p/pwgen/pwgen_2.08-1.dsc' pwgen_2.08-1.dsc 1708 SHA256:8ba952876ced56465dff1cdae42b61756b13a66656716a37bebd905857e4fee7
'http://deb.debian.org/debian/pool/main/p/pwgen/pwgen_2.08.orig.tar.gz' pwgen_2.08.orig.tar.gz 54884 SHA256:dab03dd30ad5a58e578c5581241a6e87e184a18eb2c3b2e0fffa8a9cf105c97b
'http://deb.debian.org/debian/pool/main/p/pwgen/pwgen_2.08.orig.tar.gz.asc' pwgen_2.08.orig.tar.gz.asc 488 SHA256:b16dde245d7153f261ebc8de6d5226c4cd7bccd9f880e66697f17903fcad3b6c
'http://deb.debian.org/debian/pool/main/p/pwgen/pwgen_2.08-1.debian.tar.xz' pwgen_2.08-1.debian.tar.xz 5656 SHA256:3d2ebdf3b6692e9daabf30f334127bc1aea82228a5d8bcf2cce15bfd0cd76fdc
```

Other potentially useful URLs:

- https://sources.debian.net/src/pwgen/2.08-1/ (for browsing the source)
- https://sources.debian.net/src/pwgen/2.08-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pwgen/2.08-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python-defaults=2.7.16-1`

Binary Packages:

- `libpython-stdlib:amd64=2.7.16-1`
- `libpython2-stdlib:amd64=2.7.16-1`
- `python=2.7.16-1`
- `python-minimal=2.7.16-1`
- `python2=2.7.16-1`
- `python2-minimal=2.7.16-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.16-1
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.16-1.dsc' python-defaults_2.7.16-1.dsc 2917 SHA256:6482803ce46522db092fcd3d67ed380bdfbe817b77b5ec93b65f5825fe45e544
'http://deb.debian.org/debian/pool/main/p/python-defaults/python-defaults_2.7.16-1.tar.gz' python-defaults_2.7.16-1.tar.gz 82643 SHA256:4623728a4070ba58f15d2885a4ad2f590a94e705c4f18c8f0ff51151ad89fbc1
```

Other potentially useful URLs:

- https://sources.debian.net/src/python-defaults/2.7.16-1/ (for browsing the source)
- https://sources.debian.net/src/python-defaults/2.7.16-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python-defaults/2.7.16-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python2.7=2.7.16-2+deb10u1`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.16-2+deb10u1`
- `libpython2.7-stdlib:amd64=2.7.16-2+deb10u1`
- `python2.7=2.7.16-2+deb10u1`
- `python2.7-minimal=2.7.16-2+deb10u1`

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
$ apt-get source -qq --print-uris python2.7=2.7.16-2+deb10u1
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.16-2+deb10u1.dsc' python2.7_2.7.16-2+deb10u1.dsc 3362 SHA256:c976ba9e854cf611131aacb06f3ddca206b5c799871cb269dbef1ee629be6066
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.16.orig.tar.gz' python2.7_2.7.16.orig.tar.gz 17431748 SHA256:01da813a3600876f03f46db11cc5c408175e99f03af2ba942ef324389a83bad5
'http://deb.debian.org/debian/pool/main/p/python2.7/python2.7_2.7.16-2+deb10u1.diff.gz' python2.7_2.7.16-2+deb10u1.diff.gz 293706 SHA256:37150412430a010c1f0cd816ff1c2b0d90459ecc37c8aa5df5d68f698ececeed
```

Other potentially useful URLs:

- https://sources.debian.net/src/python2.7/2.7.16-2+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/python2.7/2.7.16-2+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python2.7/2.7.16-2+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.7.3-1`

Binary Packages:

- `libpython3-stdlib:amd64=3.7.3-1`
- `python3=3.7.3-1`
- `python3-minimal=3.7.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.7.3-1
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.7.3-1.dsc' python3-defaults_3.7.3-1.dsc 2797 SHA256:00fc9d88fab413659b27886833b4f20c15400cb335de94a3f2dbb01f7adf9058
'http://deb.debian.org/debian/pool/main/p/python3-defaults/python3-defaults_3.7.3-1.tar.gz' python3-defaults_3.7.3-1.tar.gz 137436 SHA256:ed0fe03fc72b766bc4449088ff82764ac7486431efca38de89841a139f3362ad
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3-defaults/3.7.3-1/ (for browsing the source)
- https://sources.debian.net/src/python3-defaults/3.7.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3-defaults/3.7.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3.7=3.7.3-2+deb10u1`

Binary Packages:

- `libpython3.7:amd64=3.7.3-2+deb10u1`
- `libpython3.7-minimal:amd64=3.7.3-2+deb10u1`
- `libpython3.7-stdlib:amd64=3.7.3-2+deb10u1`
- `python3.7=3.7.3-2+deb10u1`
- `python3.7-minimal=3.7.3-2+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libpython3.7/copyright`, `/usr/share/doc/libpython3.7-minimal/copyright`, `/usr/share/doc/libpython3.7-stdlib/copyright`, `/usr/share/doc/python3.7/copyright`, `/usr/share/doc/python3.7-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.7=3.7.3-2+deb10u1
'http://deb.debian.org/debian/pool/main/p/python3.7/python3.7_3.7.3-2+deb10u1.dsc' python3.7_3.7.3-2+deb10u1.dsc 3404 SHA256:0ddf97878c8fa2b619d034b88b94c7900d3c506c5c99b8682adaeb8409aa31a3
'http://deb.debian.org/debian/pool/main/p/python3.7/python3.7_3.7.3.orig.tar.xz' python3.7_3.7.3.orig.tar.xz 17108364 SHA256:da60b54064d4cfcd9c26576f6df2690e62085123826cff2e667e72a91952d318
'http://deb.debian.org/debian/pool/main/p/python3.7/python3.7_3.7.3-2+deb10u1.debian.tar.xz' python3.7_3.7.3-2+deb10u1.debian.tar.xz 216340 SHA256:21d5287cd148d35c0a7db8cd45fe4f3ad70b2c0606e4a1dc40dd56f272201491
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.7/3.7.3-2+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/python3.7/3.7.3-2+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.7/3.7.3-2+deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `readline=7.0-5`

Binary Packages:

- `libreadline7:amd64=7.0-5`
- `readline-common=7.0-5`

Licenses: (parsed from: `/usr/share/doc/libreadline7/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=7.0-5
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0-5.dsc' readline_7.0-5.dsc 2419 SHA256:4a804235e91ced3b957b0772101ca3992f5ad051e6540b8c41a1f98a06e84033
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0.orig.tar.gz' readline_7.0.orig.tar.gz 2910016 SHA256:750d437185286f40a369e1e4f4764eda932b9459b5ec9a731628393dd3d32334
'http://deb.debian.org/debian/pool/main/r/readline/readline_7.0-5.debian.tar.xz' readline_7.0-5.debian.tar.xz 29992 SHA256:5c1cc7396a670ce7e6e4c0bc36e8d3067b7642bea5b30fc3ff22bf8e65d2ee80
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/7.0-5/ (for browsing the source)
- https://sources.debian.net/src/readline/7.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/7.0-5/ (for access to the source package after it no longer exists in the archive)

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

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2`

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

### `dpkg` source package: `sensible-utils=0.0.12`

Binary Packages:

- `sensible-utils=0.0.12`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.12
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.12.dsc' sensible-utils_0.0.12.dsc 1732 SHA256:1b62cc5f7561b3f5692a6edaec942e2e97e8368dabff8c865867d428eecb1221
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.12.tar.xz' sensible-utils_0.0.12.tar.xz 62152 SHA256:99ba2ebf8c57447c69d426b99b84ff9dc817be0bc4988ec6890a14558c529e2e
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.12/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serd=0.28.0~dfsg0-1`

Binary Packages:

- `libserd-0-0:amd64=0.28.0~dfsg0-1`

Licenses: (parsed from: `/usr/share/doc/libserd-0-0/copyright`)

- `BSD-3-clause`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris serd=0.28.0~dfsg0-1
'http://deb.debian.org/debian/pool/main/s/serd/serd_0.28.0~dfsg0-1.dsc' serd_0.28.0~dfsg0-1.dsc 2248 SHA256:15410919fc9ea54cdcd88efa5cb752ea31ea922b158a8e36dd4e1afaff860afa
'http://deb.debian.org/debian/pool/main/s/serd/serd_0.28.0~dfsg0.orig.tar.xz' serd_0.28.0~dfsg0.orig.tar.xz 272256 SHA256:03cd874613653cae53e18f4065216276285ea2e74542f700478afd67a7bc2150
'http://deb.debian.org/debian/pool/main/s/serd/serd_0.28.0~dfsg0-1.debian.tar.xz' serd_0.28.0~dfsg0-1.debian.tar.xz 6424 SHA256:50dc52b2a26f3aee19094e2bf00f75c7f2e0416941d3c8bee13bc68e69d2f248
```

Other potentially useful URLs:

- https://sources.debian.net/src/serd/0.28.0~dfsg0-1/ (for browsing the source)
- https://sources.debian.net/src/serd/0.28.0~dfsg0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/serd/0.28.0~dfsg0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serf=1.3.9-7`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-7+b10`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-7/


### `dpkg` source package: `shadow=1:4.5-1.1`

Binary Packages:

- `login=1:4.5-1.1`
- `passwd=1:4.5-1.1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.5-1.1
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5-1.1.dsc' shadow_4.5-1.1.dsc 2319 SHA256:75993dc19ccc4d5c404831d2dab021a03eaa39216b518d596b639d8f2ea4e98b
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA256:22b0952dc944b163e2370bb911b11ca275fc80ad024267cf21e496b28c23d500
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.5-1.1.debian.tar.xz' shadow_4.5-1.1.debian.tar.xz 462960 SHA256:3bb16bbf5d9a255d7333932ae99815d65c1c8e86127e5016809d4ba55c499538
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.5-1.1/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.5-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.5-1.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `shine=3.1.1-2`

Binary Packages:

- `libshine3:amd64=3.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libshine3/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris shine=3.1.1-2
'http://deb.debian.org/debian/pool/main/s/shine/shine_3.1.1-2.dsc' shine_3.1.1-2.dsc 1999 SHA256:57792862005a2482a7c1ee94544dd30bdeeacbf8b4cad842ad741b65545e8a16
'http://deb.debian.org/debian/pool/main/s/shine/shine_3.1.1.orig.tar.gz' shine_3.1.1.orig.tar.gz 940443 SHA256:565b87867d6f8e6616a236445d194e36f4daa9b4e7af823fcf5010af7610c49e
'http://deb.debian.org/debian/pool/main/s/shine/shine_3.1.1-2.debian.tar.xz' shine_3.1.1-2.debian.tar.xz 3624 SHA256:a9f669c5af27f11c0cca98c736decc49b056ccfe32893f85a6064161f36b1b5b
```

Other potentially useful URLs:

- https://sources.debian.net/src/shine/3.1.1-2/ (for browsing the source)
- https://sources.debian.net/src/shine/3.1.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shine/3.1.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `slang2=2.3.2-2`

Binary Packages:

- `libslang2:amd64=2.3.2-2`

Licenses: (parsed from: `/usr/share/doc/libslang2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris slang2=2.3.2-2
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.2-2.dsc' slang2_2.3.2-2.dsc 2294 SHA256:94612c6c4fa7081643f517efa5967e75b9478a0726caf887278d834256975fd4
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.2.orig.tar.xz' slang2_2.3.2.orig.tar.xz 1309848 SHA256:18c99f4c5ad9710eb0fcd4c82f7c32427f94c9c93a5ba04a88318e521db2cadf
'http://deb.debian.org/debian/pool/main/s/slang2/slang2_2.3.2-2.debian.tar.xz' slang2_2.3.2-2.debian.tar.xz 22060 SHA256:107600914e32f0b840b9bacfb46511828f1bbb0af9ad1440610566e2dc289a15
```

Other potentially useful URLs:

- https://sources.debian.net/src/slang2/2.3.2-2/ (for browsing the source)
- https://sources.debian.net/src/slang2/2.3.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/slang2/2.3.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `snappy=1.1.7-1`

Binary Packages:

- `libsnappy1v5:amd64=1.1.7-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris snappy=1.1.7-1
'http://deb.debian.org/debian/pool/main/s/snappy/snappy_1.1.7-1.dsc' snappy_1.1.7-1.dsc 1785 SHA256:a2b45cc0ddc41baae02f0dd51448afef2d9a2f771253b472f0141aff6b5c640c
'http://deb.debian.org/debian/pool/main/s/snappy/snappy_1.1.7.orig.tar.gz' snappy_1.1.7.orig.tar.gz 1090550 SHA256:3dfa02e873ff51a11ee02b9ca391807f0c8ea0529a4924afa645fbf97163f9d4
'http://deb.debian.org/debian/pool/main/s/snappy/snappy_1.1.7-1.debian.tar.xz' snappy_1.1.7-1.debian.tar.xz 5028 SHA256:b6041cea215dbc3a48c8230be97445fe0ec342bad9eb4f6ddc26ac6cb3fc4e12
```

Other potentially useful URLs:

- https://sources.debian.net/src/snappy/1.1.7-1/ (for browsing the source)
- https://sources.debian.net/src/snappy/1.1.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/snappy/1.1.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sndio=1.5.0-3`

Binary Packages:

- `libsndio7.0:amd64=1.5.0-3`

Licenses: (parsed from: `/usr/share/doc/libsndio7.0/copyright`)

- `ISC`
- `ISC-packaging`

Source:

```console
$ apt-get source -qq --print-uris sndio=1.5.0-3
'http://deb.debian.org/debian/pool/main/s/sndio/sndio_1.5.0-3.dsc' sndio_1.5.0-3.dsc 1942 SHA256:e024ba6ddd4bcc81bf955689a55c454a8a031b729addaed6aa0bb05afc2ad3b1
'http://deb.debian.org/debian/pool/main/s/sndio/sndio_1.5.0.orig.tar.gz' sndio_1.5.0.orig.tar.gz 125661 SHA256:12c70044749ad9cb7eaeb26c936816aa6b314fe4be71ef479d12272e4c5ad253
'http://deb.debian.org/debian/pool/main/s/sndio/sndio_1.5.0-3.debian.tar.xz' sndio_1.5.0-3.debian.tar.xz 5780 SHA256:325417b7a391a106ede0d1f30cbc0e1bbbda56ef2713c7598a1436c1d92c7d03
```

Other potentially useful URLs:

- https://sources.debian.net/src/sndio/1.5.0-3/ (for browsing the source)
- https://sources.debian.net/src/sndio/1.5.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sndio/1.5.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sord=0.16.0~dfsg0-1`

Binary Packages:

- `libsord-0-0:amd64=0.16.0~dfsg0-1+b1`

Licenses: (parsed from: `/usr/share/doc/libsord-0-0/copyright`)

- `BSD-3-clause`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris sord=0.16.0~dfsg0-1
'http://deb.debian.org/debian/pool/main/s/sord/sord_0.16.0~dfsg0-1.dsc' sord_0.16.0~dfsg0-1.dsc 2228 SHA256:e8bfe1c3894a040c0d0da25e55c356ec2fc213a77570eaa43dbd4b938e88090b
'http://deb.debian.org/debian/pool/main/s/sord/sord_0.16.0~dfsg0.orig.tar.xz' sord_0.16.0~dfsg0.orig.tar.xz 206836 SHA256:11f3e5273d3da63e0305943b087083f89335d434acf599d7a1d75fe084bed1ef
'http://deb.debian.org/debian/pool/main/s/sord/sord_0.16.0~dfsg0-1.debian.tar.xz' sord_0.16.0~dfsg0-1.debian.tar.xz 5092 SHA256:017d8ef206b8646cd179f1b3bf0060ab3a5360bd7040c85be24efa4f0339b90c
```

Other potentially useful URLs:

- https://sources.debian.net/src/sord/0.16.0~dfsg0-1/ (for browsing the source)
- https://sources.debian.net/src/sord/0.16.0~dfsg0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sord/0.16.0~dfsg0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `sqlite3=3.27.2-3`

Binary Packages:

- `libsqlite3-0:amd64=3.27.2-3`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.27.2-3
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.27.2-3.dsc' sqlite3_3.27.2-3.dsc 2398 SHA256:4d8c953891d6268911aa273f8cb7c9e0bdd026c7918f6203fd019d3e16cea1cc
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.27.2.orig-www.tar.xz' sqlite3_3.27.2.orig-www.tar.xz 5602752 SHA256:b50bea0e1974b33bcb2cec4c29fcdeecd8f960020ce0310b15fb123938844bee
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.27.2.orig.tar.xz' sqlite3_3.27.2.orig.tar.xz 6844832 SHA256:6cb1606bbc38270739d256b5ab1cf94dccf5b2a3b4cbceb0545aac76f6ef40f2
'http://deb.debian.org/debian/pool/main/s/sqlite3/sqlite3_3.27.2-3.debian.tar.xz' sqlite3_3.27.2-3.debian.tar.xz 30372 SHA256:0a95abfc23baa8d0fa2ec7fc6b96f46e34c37f23ff540bc041eff111e6550af9
```

Other potentially useful URLs:

- https://sources.debian.net/src/sqlite3/3.27.2-3/ (for browsing the source)
- https://sources.debian.net/src/sqlite3/3.27.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sqlite3/3.27.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sratom=0.6.0~dfsg0-1`

Binary Packages:

- `libsratom-0-0:amd64=0.6.0~dfsg0-1`

Licenses: (parsed from: `/usr/share/doc/libsratom-0-0/copyright`)

- `BSD-3-clause`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris sratom=0.6.0~dfsg0-1
'http://deb.debian.org/debian/pool/main/s/sratom/sratom_0.6.0~dfsg0-1.dsc' sratom_0.6.0~dfsg0-1.dsc 2251 SHA256:970caa2b71bccd7fef266da7e6686df5695c01b984b566cfacb791f4a1fb8cde
'http://deb.debian.org/debian/pool/main/s/sratom/sratom_0.6.0~dfsg0.orig.tar.xz' sratom_0.6.0~dfsg0.orig.tar.xz 138872 SHA256:dd9c28ef2ecb8609888b50379e84fa416bf3c7a5615f6f1d1dad511e8c4de54a
'http://deb.debian.org/debian/pool/main/s/sratom/sratom_0.6.0~dfsg0-1.debian.tar.xz' sratom_0.6.0~dfsg0-1.debian.tar.xz 4396 SHA256:3c23328c147834f5703b9ca4dc5e68ca64c223cf8e297a7fa2085f5c5861898c
```

Other potentially useful URLs:

- https://sources.debian.net/src/sratom/0.6.0~dfsg0-1/ (for browsing the source)
- https://sources.debian.net/src/sratom/0.6.0~dfsg0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sratom/0.6.0~dfsg0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `subversion=1.10.4-1+deb10u1`

Binary Packages:

- `libsvn1:amd64=1.10.4-1+deb10u1`
- `subversion=1.10.4-1+deb10u1`

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
$ apt-get source -qq --print-uris subversion=1.10.4-1+deb10u1
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.4-1+deb10u1.dsc' subversion_1.10.4-1+deb10u1.dsc 3428 SHA256:c9956fd5b850924dd123048b39195b3d591f55b9cbdf18d4d2a0f496f7decc72
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.4.orig.tar.gz' subversion_1.10.4.orig.tar.gz 11347907 SHA256:354022a837596eb1b5676639ea8d73aa326fa8b2c610d8e1b39aeb7228921f4e
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.4.orig.tar.gz.asc' subversion_1.10.4.orig.tar.gz.asc 2107 SHA256:bc6173c43ac837f875d9f2921e118c194455796b419769e155496cf084376428
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.10.4-1+deb10u1.debian.tar.xz' subversion_1.10.4-1+deb10u1.debian.tar.xz 438024 SHA256:1bc8900ef1b9d2af84827dab0fd0164e2058381be3bba0db6fd13cbc858c9b1e
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.10.4-1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.10.4-1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.10.4-1+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `suitesparse=1:5.4.0+dfsg-1`

Binary Packages:

- `libcolamd2:amd64=1:5.4.0+dfsg-1`
- `libsuitesparseconfig5:amd64=1:5.4.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libcolamd2/copyright`, `/usr/share/doc/libsuitesparseconfig5/copyright`)

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
$ apt-get source -qq --print-uris suitesparse=1:5.4.0+dfsg-1
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_5.4.0+dfsg-1.dsc' suitesparse_5.4.0+dfsg-1.dsc 3094 SHA256:0c18f97f8a736f0071296ab9c331e66583145ee108e41ab5e3786811beba142f
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_5.4.0+dfsg.orig.tar.xz' suitesparse_5.4.0+dfsg.orig.tar.xz 41794852 SHA256:95bf7956b8ccbb5c9db0071221ef88f39dc0439e8f321d7f95a451e670ce1ace
'http://deb.debian.org/debian/pool/main/s/suitesparse/suitesparse_5.4.0+dfsg-1.debian.tar.xz' suitesparse_5.4.0+dfsg-1.debian.tar.xz 31528 SHA256:eb19a768a88ad0a43b3b079d70af2e126369e49ba9f9155505f4ea6089081dcc
```

Other potentially useful URLs:

- https://sources.debian.net/src/suitesparse/1:5.4.0+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/suitesparse/1:5.4.0+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/suitesparse/1:5.4.0+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=241-7~deb10u3`

Binary Packages:

- `libpam-systemd:amd64=241-7~deb10u3`
- `libsystemd0:amd64=241-7~deb10u3`
- `libudev1:amd64=241-7~deb10u3`
- `systemd=241-7~deb10u3`
- `systemd-sysv=241-7~deb10u3`

Licenses: (parsed from: `/usr/share/doc/libpam-systemd/copyright`, `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`, `/usr/share/doc/systemd/copyright`, `/usr/share/doc/systemd-sysv/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=241-7~deb10u3
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_241-7~deb10u3.dsc' systemd_241-7~deb10u3.dsc 4946 SHA256:04ef215da8e05800c587601eacb011f9596dd7138ac85b43f33efdbf6b799a31
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_241.orig.tar.gz' systemd_241.orig.tar.gz 7640538 SHA256:b2561a8e1d10a2c248253f0dda31a85dd6d69f2b54177de55e02cd1d2778316e
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_241-7~deb10u3.debian.tar.xz' systemd_241-7~deb10u3.debian.tar.xz 169396 SHA256:54d4d0624c776ab2a375f303ed64bfe25ddc8cb47b5bfe6c2a400ba842420363
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/241-7~deb10u3/ (for browsing the source)
- https://sources.debian.net/src/systemd/241-7~deb10u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/241-7~deb10u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=2.93-8`

Binary Packages:

- `sysvinit-utils=2.93-8`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.93-8
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.93-8.dsc' sysvinit_2.93-8.dsc 2657 SHA256:84aa66bfa1c7963c179da26c015468d489b39bde19c85096b4d3e261e5fc043d
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.93.orig.tar.xz' sysvinit_2.93.orig.tar.xz 117580 SHA256:472d460e233d981488509a167125a82925c8c9aba6b5608cb22598fdf326a8ff
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.93.orig.tar.xz.asc' sysvinit_2.93.orig.tar.xz.asc 1076 SHA256:cf2b374a96276a16e3ef07ad2be596420f0d8d77227aad3144d7ab4ea165a4af
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.93-8.debian.tar.xz' sysvinit_2.93-8.debian.tar.xz 127136 SHA256:2db2ae46048acf743445545151cbc0bc5530eca1f2eec51df3175d8ab26edfa6
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.93-8/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.93-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.93-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.30+dfsg-6`

Binary Packages:

- `tar=1.30+dfsg-6`

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

### `dpkg` source package: `tcp-wrappers=7.6.q-28`

Binary Packages:

- `libwrap0:amd64=7.6.q-28`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcp-wrappers=7.6.q-28
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-28.dsc' tcp-wrappers_7.6.q-28.dsc 1726 SHA256:6bfa392a42ce81204a0bea9e6a80460468ce34612c2af4405382fcead3ac4ca6
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q.orig.tar.gz' tcp-wrappers_7.6.q.orig.tar.gz 99438 SHA256:9543d7adedf78a6de0b221ccbbd1952e08b5138717f4ade814039bb489a4315d
'http://deb.debian.org/debian/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-28.debian.tar.xz' tcp-wrappers_7.6.q-28.debian.tar.xz 36104 SHA256:9e878177878b7796ab9e8cb4abb094bf66b3d37e0e1af3cee3e24afde4b1e11f
```

Other potentially useful URLs:

- https://sources.debian.net/src/tcp-wrappers/7.6.q-28/ (for browsing the source)
- https://sources.debian.net/src/tcp-wrappers/7.6.q-28/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tcp-wrappers/7.6.q-28/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.1.0+git191117-2~deb10u1`

Binary Packages:

- `libtiff5:amd64=4.1.0+git191117-2~deb10u1`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.1.0+git191117-2~deb10u1
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.1.0+git191117-2~deb10u1.dsc' tiff_4.1.0+git191117-2~deb10u1.dsc 2274 SHA256:fc63d46d3fbc75c2f03b09b79f9297d701a2b08c968bc8b5826f9e71df5180c8
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.1.0+git191117.orig.tar.xz' tiff_4.1.0+git191117.orig.tar.xz 1533524 SHA256:67e1d045e994adb7144b0cca228d70dd6d520aaf8c75c342064bc0fd601e6e42
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.1.0+git191117-2~deb10u1.debian.tar.xz' tiff_4.1.0+git191117-2~deb10u1.debian.tar.xz 19440 SHA256:e9dcc77d338663f6be84efe32ae5d4ec9b48923c731aa939f37aa909e60d9f10
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.1.0+git191117-2~deb10u1/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.1.0+git191117-2~deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.1.0+git191117-2~deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `twolame=0.3.13-4`

Binary Packages:

- `libtwolame0:amd64=0.3.13-4`

Licenses: (parsed from: `/usr/share/doc/libtwolame0/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris twolame=0.3.13-4
'http://deb.debian.org/debian/pool/main/t/twolame/twolame_0.3.13-4.dsc' twolame_0.3.13-4.dsc 2049 SHA256:554631368c225e14bf19679816521041149459ff75169e650f6d6a74e59f4a1f
'http://deb.debian.org/debian/pool/main/t/twolame/twolame_0.3.13.orig.tar.gz' twolame_0.3.13.orig.tar.gz 660415 SHA256:98f332f48951f47f23f70fd0379463aff7d7fb26f07e1e24e42ddef22cc6112a
'http://deb.debian.org/debian/pool/main/t/twolame/twolame_0.3.13-4.debian.tar.xz' twolame_0.3.13-4.debian.tar.xz 4460 SHA256:2dde6d2565e95dbecec6a0921ded7cd5adf2d6535ba5aed6f7f41d4cbea7b5c4
```

Other potentially useful URLs:

- https://sources.debian.net/src/twolame/0.3.13-4/ (for browsing the source)
- https://sources.debian.net/src/twolame/0.3.13-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/twolame/0.3.13-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2019c-0+deb10u1`

Binary Packages:

- `tzdata=2019c-0+deb10u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2019c-0+deb10u1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c-0+deb10u1.dsc' tzdata_2019c-0+deb10u1.dsc 2264 SHA256:983c27d24d78c52d8f213b1b5800aaa90a171a4f805451b0845752f97c6f924b
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c.orig.tar.gz' tzdata_2019c.orig.tar.gz 392087 SHA256:79c7806dab09072308da0e3d22c37d3b245015a591891ea147d3b133b60ffc7c
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c.orig.tar.gz.asc' tzdata_2019c.orig.tar.gz.asc 833 SHA256:cd31deaeee229d45e4f4b973441189e7619ef81679359e9c8b47b2a87aaf6a07
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2019c-0+deb10u1.debian.tar.xz' tzdata_2019c-0+deb10u1.debian.tar.xz 104932 SHA256:fa8071037767a7dfa054c26621c5079809ee038eddb32a58814faf3541d52d5a
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2019c-0+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2019c-0+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2019c-0+deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ufraw=0.22-4`

Binary Packages:

- `ufraw=0.22-4`
- `ufraw-batch=0.22-4`

Licenses: (parsed from: `/usr/share/doc/ufraw/copyright`, `/usr/share/doc/ufraw-batch/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ufraw=0.22-4
'http://deb.debian.org/debian/pool/main/u/ufraw/ufraw_0.22-4.dsc' ufraw_0.22-4.dsc 1619 SHA256:8ff4fad5b207b7e7220cd20443eb0378052a847e0210fb80844b7df7abff24f5
'http://deb.debian.org/debian/pool/main/u/ufraw/ufraw_0.22.orig.tar.gz' ufraw_0.22.orig.tar.gz 1103554 SHA256:f7abd28ce587db2a74b4c54149bd8a2523a7ddc09bedf4f923246ff0ae09a25e
'http://deb.debian.org/debian/pool/main/u/ufraw/ufraw_0.22-4.debian.tar.xz' ufraw_0.22-4.debian.tar.xz 9048 SHA256:5a06d7d5660df57c2cf7861dd000ebb48dcaa9b7caab4a6c1f5a2a3ac9ad4c5a
```

Other potentially useful URLs:

- https://sources.debian.net/src/ufraw/0.22-4/ (for browsing the source)
- https://sources.debian.net/src/ufraw/0.22-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ufraw/0.22-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `unzip=6.0-23+deb10u1`

Binary Packages:

- `unzip=6.0-23+deb10u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-23+deb10u1
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-23+deb10u1.dsc' unzip_6.0-23+deb10u1.dsc 1376 SHA256:17c827fcb399d9e82bd08a7574838d95b10a335294edad6f604175dc1e7e8859
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://deb.debian.org/debian/pool/main/u/unzip/unzip_6.0-23+deb10u1.debian.tar.xz' unzip_6.0-23+deb10u1.debian.tar.xz 23012 SHA256:f64e87c377aea1139e2d2d6cc0ea8edb089951d28089e1e5de567a6cb715d384
```

Other potentially useful URLs:

- https://sources.debian.net/src/unzip/6.0-23+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/unzip/6.0-23+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/unzip/6.0-23+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `utf8proc=2.3.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.3.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.3.0-1
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.3.0-1.dsc' utf8proc_2.3.0-1.dsc 2097 SHA256:046ea990ad7ebbe39c5a1db14a360cde520ac289a7e50cc33907c0607b9ed5c0
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.3.0.orig.tar.gz' utf8proc_2.3.0.orig.tar.gz 154282 SHA256:c0265a49b59bab95481cab1ae958ba034dedc47ad58676a61f5de1fa9347930e
'http://deb.debian.org/debian/pool/main/u/utf8proc/utf8proc_2.3.0-1.debian.tar.xz' utf8proc_2.3.0-1.debian.tar.xz 49176 SHA256:0b1689423d166cb671812e990bc30682c18e0cea8b97e1d71fb7f8136d81d317
```

Other potentially useful URLs:

- https://sources.debian.net/src/utf8proc/2.3.0-1/ (for browsing the source)
- https://sources.debian.net/src/utf8proc/2.3.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/utf8proc/2.3.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.33.1-0.1`

Binary Packages:

- `bsdutils=1:2.33.1-0.1`
- `fdisk=2.33.1-0.1`
- `libblkid1:amd64=2.33.1-0.1`
- `libfdisk1:amd64=2.33.1-0.1`
- `libmount1:amd64=2.33.1-0.1`
- `libsmartcols1:amd64=2.33.1-0.1`
- `libuuid1:amd64=2.33.1-0.1`
- `mount=2.33.1-0.1`
- `util-linux=2.33.1-0.1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.33.1-0.1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.33.1-0.1.dsc' util-linux_2.33.1-0.1.dsc 3988 SHA256:b5ee1ff0a8de37c3e4d7c0c29b7571b30ba4bea1d37e55e3d1dac3a3cbc50827
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.33.1.orig.tar.xz' util-linux_2.33.1.orig.tar.xz 4650936 SHA256:c14bd9f3b6e1792b90db87696e87ec643f9d63efa0a424f092a5a6b2f2dbef21
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.33.1-0.1.debian.tar.xz' util-linux_2.33.1-0.1.debian.tar.xz 81780 SHA256:07bfeb8298fab559dec2091463cab343785853bcae6c92c0806b7639e105913a
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.33.1-0.1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.33.1-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.33.1-0.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wavpack=5.1.0-6`

Binary Packages:

- `libwavpack1:amd64=5.1.0-6`

Licenses: (parsed from: `/usr/share/doc/libwavpack1/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris wavpack=5.1.0-6
'http://deb.debian.org/debian/pool/main/w/wavpack/wavpack_5.1.0-6.dsc' wavpack_5.1.0-6.dsc 2056 SHA256:aa5c3b5103146353f5202a27d769467230605671f2ce2f82b90a5d4929374b89
'http://deb.debian.org/debian/pool/main/w/wavpack/wavpack_5.1.0.orig.tar.bz2' wavpack_5.1.0.orig.tar.bz2 824331 SHA256:1939627d5358d1da62bc6158d63f7ed12905552f3a799c799ee90296a7612944
'http://deb.debian.org/debian/pool/main/w/wavpack/wavpack_5.1.0-6.debian.tar.xz' wavpack_5.1.0-6.debian.tar.xz 10860 SHA256:2802722260e7e95dcfc25d8d6704f5dea80018797fd583537baec4b7729993b4
```

Other potentially useful URLs:

- https://sources.debian.net/src/wavpack/5.1.0-6/ (for browsing the source)
- https://sources.debian.net/src/wavpack/5.1.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wavpack/5.1.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wayland=1.16.0-1`

Binary Packages:

- `libwayland-client0:amd64=1.16.0-1`
- `libwayland-cursor0:amd64=1.16.0-1`
- `libwayland-egl1:amd64=1.16.0-1`

Licenses: (parsed from: `/usr/share/doc/libwayland-client0/copyright`, `/usr/share/doc/libwayland-cursor0/copyright`, `/usr/share/doc/libwayland-egl1/copyright`)

- `X11`

Source:

```console
$ apt-get source -qq --print-uris wayland=1.16.0-1
'http://deb.debian.org/debian/pool/main/w/wayland/wayland_1.16.0-1.dsc' wayland_1.16.0-1.dsc 2321 SHA256:cbfdadf1b50b40244da6f6deabbbe5b5cb4bb95b247e7d1649f43d3d874ca288
'http://deb.debian.org/debian/pool/main/w/wayland/wayland_1.16.0-1.tar.gz' wayland_1.16.0-1.tar.gz 324833 SHA256:6c3ed6fdf6906aab51e94119b86589d21f497e03d28c8fc3a7a16e286798b55e
```

Other potentially useful URLs:

- https://sources.debian.net/src/wayland/1.16.0-1/ (for browsing the source)
- https://sources.debian.net/src/wayland/1.16.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wayland/1.16.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.20.1-1.1`

Binary Packages:

- `wget=1.20.1-1.1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.20.1-1.1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.20.1-1.1.dsc' wget_1.20.1-1.1.dsc 2092 SHA256:b193fdf37cc33955e366ae1fdb6df5425d13769d9e131c52382ae132ad931261
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.20.1.orig.tar.gz' wget_1.20.1.orig.tar.gz 4392853 SHA256:b783b390cb571c837b392857945f5a1f00ec6b043177cc42abb8ee1b542ee1b3
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.20.1-1.1.debian.tar.xz' wget_1.20.1-1.1.debian.tar.xz 60872 SHA256:7eee4b6b9394a495888d1fc0db951c6b3bd883ca522a11df3433732dc116001e
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.20.1-1.1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.20.1-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.20.1-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x264=2:0.155.2917+git0a84d98-2`

Binary Packages:

- `libx264-155:amd64=2:0.155.2917+git0a84d98-2`
- `x264=2:0.155.2917+git0a84d98-2`

Licenses: (parsed from: `/usr/share/doc/libx264-155/copyright`, `/usr/share/doc/x264/copyright`)

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
$ apt-get source -qq --print-uris x264=2:0.155.2917+git0a84d98-2
'http://deb.debian.org/debian/pool/main/x/x264/x264_0.155.2917+git0a84d98-2.dsc' x264_0.155.2917+git0a84d98-2.dsc 2407 SHA256:b296d3069efcbbf6a7a9c3a6bfd1ec99fa559ece8c5959158859e47e0092a393
'http://deb.debian.org/debian/pool/main/x/x264/x264_0.155.2917+git0a84d98.orig.tar.gz' x264_0.155.2917+git0a84d98.orig.tar.gz 934501 SHA256:814e8d233a7a98a66b4c592bec60c531369bac453d679ba6c006bdcd2677e7e8
'http://deb.debian.org/debian/pool/main/x/x264/x264_0.155.2917+git0a84d98-2.debian.tar.xz' x264_0.155.2917+git0a84d98-2.debian.tar.xz 23260 SHA256:9058a14889abcb6e28e1219ba3b5a78c00125f91877a1ecf3ac7d3aa352b19c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/x264/2:0.155.2917+git0a84d98-2/ (for browsing the source)
- https://sources.debian.net/src/x264/2:0.155.2917+git0a84d98-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x264/2:0.155.2917+git0a84d98-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `x265=2.9-4`

Binary Packages:

- `libx265-165:amd64=2.9-4`

Licenses: (parsed from: `/usr/share/doc/libx265-165/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=2.9-4
'http://deb.debian.org/debian/pool/main/x/x265/x265_2.9-4.dsc' x265_2.9-4.dsc 2223 SHA256:eba4d3027a0c194365f5ffa162095051990888fe99284bf93fe103d52c6afd85
'http://deb.debian.org/debian/pool/main/x/x265/x265_2.9.orig.tar.gz' x265_2.9.orig.tar.gz 1385848 SHA256:ebae687c84a39f54b995417c52a2fdde65a4e2e7ebac5730d251471304b91024
'http://deb.debian.org/debian/pool/main/x/x265/x265_2.9-4.debian.tar.xz' x265_2.9-4.debian.tar.xz 13180 SHA256:f307f040084643e4a0138ab3f5babf648683089530fd5f515d16fdb5f9354aaf
```

Other potentially useful URLs:

- https://sources.debian.net/src/x265/2.9-4/ (for browsing the source)
- https://sources.debian.net/src/x265/2.9-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/x265/2.9-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xkeyboard-config=2.26-2`

Binary Packages:

- `xkb-data=2.26-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xkeyboard-config=2.26-2
'http://deb.debian.org/debian/pool/main/x/xkeyboard-config/xkeyboard-config_2.26-2.dsc' xkeyboard-config_2.26-2.dsc 2111 SHA256:32930b4862b6a51799dd2da66781dea68df4d231c7e6eadaffbf7da2528673e6
'http://deb.debian.org/debian/pool/main/x/xkeyboard-config/xkeyboard-config_2.26.orig.tar.gz' xkeyboard-config_2.26.orig.tar.gz 1626968 SHA256:8d7e2aaa4e9d66843540e6ef3ebadf79d665d954bfa37d8829be428da6e08bbe
'http://deb.debian.org/debian/pool/main/x/xkeyboard-config/xkeyboard-config_2.26-2.diff.gz' xkeyboard-config_2.26-2.diff.gz 65550 SHA256:68261530c86dc1f6373486fc32ff4e7af6b4a447d184a5f1ff8a54ff248efb78
```

Other potentially useful URLs:

- https://sources.debian.net/src/xkeyboard-config/2.26-2/ (for browsing the source)
- https://sources.debian.net/src/xkeyboard-config/2.26-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xkeyboard-config/2.26-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xmlsec1=1.2.27-2`

Binary Packages:

- `libxmlsec1:amd64=1.2.27-2`
- `libxmlsec1-nss:amd64=1.2.27-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xmlsec1=1.2.27-2
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.27-2.dsc' xmlsec1_1.2.27-2.dsc 2591 SHA256:e62d69aba1b996ee6e2ac574e8f0b05fd4dd8b44e47e8cca3ffafacebed64646
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.27.orig.tar.gz' xmlsec1_1.2.27.orig.tar.gz 1999945 SHA256:9094a84149a7ab50325fe4e5ee96de14d5280fde257539abb401b43044c97648
'http://deb.debian.org/debian/pool/main/x/xmlsec1/xmlsec1_1.2.27-2.debian.tar.xz' xmlsec1_1.2.27-2.debian.tar.xz 8728 SHA256:e6c1eeec7bc77a99e1c6e75f6a1919b283e5edf4e0828059fd27c46d55967f74
```

Other potentially useful URLs:

- https://sources.debian.net/src/xmlsec1/1.2.27-2/ (for browsing the source)
- https://sources.debian.net/src/xmlsec1/1.2.27-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xmlsec1/1.2.27-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xvidcore=2:1.3.5-1`

Binary Packages:

- `libxvidcore4:amd64=2:1.3.5-1`

Licenses: (parsed from: `/usr/share/doc/libxvidcore4/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xvidcore=2:1.3.5-1
'http://deb.debian.org/debian/pool/main/x/xvidcore/xvidcore_1.3.5-1.dsc' xvidcore_1.3.5-1.dsc 2131 SHA256:36b1e21f8767346d8698c13ad560961336726c2cb206b7097715d421abdf8192
'http://deb.debian.org/debian/pool/main/x/xvidcore/xvidcore_1.3.5.orig.tar.bz2' xvidcore_1.3.5.orig.tar.bz2 698846 SHA256:7c20f279f9d8e89042e85465d2bcb1b3130ceb1ecec33d5448c4589d78f010b4
'http://deb.debian.org/debian/pool/main/x/xvidcore/xvidcore_1.3.5-1.debian.tar.xz' xvidcore_1.3.5-1.debian.tar.xz 6180 SHA256:06166aa04159f8c451d53f1ae70cbf65a65d325b4769f779dc009894ca801e08
```

Other potentially useful URLs:

- https://sources.debian.net/src/xvidcore/2:1.3.5-1/ (for browsing the source)
- https://sources.debian.net/src/xvidcore/2:1.3.5-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xvidcore/2:1.3.5-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.4-1`

Binary Packages:

- `liblzma5:amd64=5.2.4-1`
- `xz-utils=5.2.4-1`

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

### `dpkg` source package: `zeromq3=4.3.1-4+deb10u1`

Binary Packages:

- `libzmq5:amd64=4.3.1-4+deb10u1`

Licenses: (parsed from: `/usr/share/doc/libzmq5/copyright`)

- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-3`
- `LGPL-3.0+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris zeromq3=4.3.1-4+deb10u1
'http://deb.debian.org/debian/pool/main/z/zeromq3/zeromq3_4.3.1-4+deb10u1.dsc' zeromq3_4.3.1-4+deb10u1.dsc 1887 SHA256:a813ac13021af84b47a33933de63b43a62f1040aac2db7c3f9e6c28453f4e5f2
'http://deb.debian.org/debian/pool/main/z/zeromq3/zeromq3_4.3.1.orig.tar.gz' zeromq3_4.3.1.orig.tar.gz 788963 SHA256:e1dec061725b55d791e0c6952b8c220846c8cd901c09d1283a6e902898205b9d
'http://deb.debian.org/debian/pool/main/z/zeromq3/zeromq3_4.3.1-4+deb10u1.debian.tar.xz' zeromq3_4.3.1-4+deb10u1.debian.tar.xz 15780 SHA256:f42a40b085582634e2b04488f882d84b00e1416a43d01acbce5afd25867ae91e
```

Other potentially useful URLs:

- https://sources.debian.net/src/zeromq3/4.3.1-4+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/zeromq3/4.3.1-4+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zeromq3/4.3.1-4+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.11.dfsg-1`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-1
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-1.dsc' zlib_1.2.11.dfsg-1.dsc 2266 SHA256:bf21ab4d60cb836725162f5072884596e781a2f4974182af1868f546306eb8c8
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-1.debian.tar.xz' zlib_1.2.11.dfsg-1.debian.tar.xz 18956 SHA256:00b95b629fbe9a5181f8ba1ceddedf627aba1ab42e47f5916be8a41deb54098a
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.11.dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zvbi=0.2.35-16`

Binary Packages:

- `libzvbi-common=0.2.35-16`
- `libzvbi0:amd64=0.2.35-16`

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
$ apt-get source -qq --print-uris zvbi=0.2.35-16
'http://deb.debian.org/debian/pool/main/z/zvbi/zvbi_0.2.35-16.dsc' zvbi_0.2.35-16.dsc 2125 SHA256:0df6f41282538105a4815c641b744d818aa54fb798073e84c041fb1437b6ca4a
'http://deb.debian.org/debian/pool/main/z/zvbi/zvbi_0.2.35.orig.tar.bz2' zvbi_0.2.35.orig.tar.bz2 1047761 SHA256:fc883c34111a487c4a783f91b1b2bb5610d8d8e58dcba80c7ab31e67e4765318
'http://deb.debian.org/debian/pool/main/z/zvbi/zvbi_0.2.35-16.debian.tar.xz' zvbi_0.2.35-16.debian.tar.xz 15704 SHA256:077f976b116a772913a58256db01e6c9bf4764701b1f95f069c82d2133bef64d
```

Other potentially useful URLs:

- https://sources.debian.net/src/zvbi/0.2.35-16/ (for browsing the source)
- https://sources.debian.net/src/zvbi/0.2.35-16/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zvbi/0.2.35-16/ (for access to the source package after it no longer exists in the archive)
