# `xwiki:12`

## Docker Metadata

- Image ID: `sha256:b4c5deb994febc9cc680b0fafa779f8d3bee9550a7eff9ea394cd0319dc3f15b`
- Created: `2020-09-01T07:34:13.119421807Z`
- Virtual Size: ~ 1.31 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["xwiki"]`
- Environment:
  - `PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=en_US.UTF-8`
  - `LANGUAGE=en_US:en`
  - `LC_ALL=en_US.UTF-8`
  - `JAVA_VERSION=jdk-11.0.8+10`
  - `JAVA_HOME=/opt/java/openjdk`
  - `CATALINA_HOME=/usr/local/tomcat`
  - `TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib`
  - `LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib`
  - `GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23`
  - `TOMCAT_MAJOR=8`
  - `TOMCAT_VERSION=8.5.57`
  - `TOMCAT_SHA512=720de36bb3e40a4c67bdf0137b12ae0fd733aef772d81a4b8dab00f29924ddd17ecb2a7217b9551fc0ca51bd81d1da13ad63b6694c445e5c0e42dfa7f279ede1`
  - `XWIKI_VERSION=12.7`
  - `XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/12.7`
  - `XWIKI_DOWNLOAD_SHA256=2106a0bb64e7ee755b356cd5e661da98d650baf64ff820b221b1751afa0ffb95`
  - `MYSQL_JDBC_VERSION=8.0.20`
  - `MYSQL_JDBC_SHA256=56a42553b516660ae0bcd08f7f4f5f375294afbd62200d6c0c88a8c61c668ede`
  - `MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.20`
  - `MYSQL_JDBC_ARTIFACT=mysql-connector-java-8.0.20.jar`
  - `MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-java-8.0.20.jar`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3build1`

Binary Packages:

- `libacl1:amd64=2.2.52-3build1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3build1.dsc' acl_2.2.52-3build1.dsc 2031 SHA256:864215f3e68d6b169a044bd952e78be9b0b1cf527a2cbf25866cab919e78e64b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3build1.debian.tar.xz' acl_2.2.52-3build1.debian.tar.xz 8788 SHA256:0729d8c850aa26bc9f1b22ce632efb1616a3f97dc5fca1d9edfda45b582b7f37
```

### `dpkg` source package: `adduser=3.116ubuntu1`

Binary Packages:

- `adduser=3.116ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.116ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.116ubuntu1.dsc' adduser_3.116ubuntu1.dsc 1845 SHA256:fc44097093d74fc2e36fc37dceb54cf6bcb70a434240b14fd91beb64849cf2fd
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.116ubuntu1.tar.xz' adduser_3.116ubuntu1.tar.xz 216868 SHA256:f34f1d95e96ecae3b068a3dd666848f82f06cbb26152c56a6b72bd71555a8f18
```

### `dpkg` source package: `adwaita-icon-theme=3.28.0-1ubuntu1`

Binary Packages:

- `adwaita-icon-theme=3.28.0-1ubuntu1`

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
$ apt-get source -qq --print-uris adwaita-icon-theme=3.28.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.28.0-1ubuntu1.dsc' adwaita-icon-theme_3.28.0-1ubuntu1.dsc 2344 SHA256:ae47ec360d09ee62180ff5438f60306c2bf31a9fb6349665054c95fcc6a5c7a1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.28.0.orig.tar.xz' adwaita-icon-theme_3.28.0.orig.tar.xz 19992224 SHA256:7aae8c1dffd6772fd1a21a3d365a0ea28b7c3988bdbbeafbf8742cda68242150
'http://archive.ubuntu.com/ubuntu/pool/main/a/adwaita-icon-theme/adwaita-icon-theme_3.28.0-1ubuntu1.debian.tar.xz' adwaita-icon-theme_3.28.0-1ubuntu1.debian.tar.xz 29528 SHA256:4ed0f37ddd3297bcc595486b9eb326638347c565f57a0327e0e6f170f170a786
```

### `dpkg` source package: `apr=1.6.3-2`

Binary Packages:

- `libapr1:amd64=1.6.3-2`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.3-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3-2.dsc' apr_1.6.3-2.dsc 2305 SHA256:0597703f9ea3bc3b30fcd7e055c67c2113e5c4255df5ff42738ce6a396bf5afc
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3.orig.tar.bz2' apr_1.6.3.orig.tar.bz2 854100 SHA256:131f06d16d7aabd097fa992a33eec2b6af3962f93e6d570a9bd4d85e95993172
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3.orig.tar.bz2.asc' apr_1.6.3.orig.tar.bz2.asc 801 SHA256:33db39162f7ca9acdccaa4f19630a67045542791b262116d3512c8b5d7c3fca1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3-2.debian.tar.xz' apr_1.6.3-2.debian.tar.xz 213068 SHA256:ac515f888f7157586631e3de9792ee01d239f9cbf1e768be31ee6daac61f2597
```

### `dpkg` source package: `apt=1.6.12ubuntu0.1`

Binary Packages:

- `apt=1.6.12ubuntu0.1`
- `libapt-pkg5.0:amd64=1.6.12ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.6.12ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.dsc' apt_1.6.12ubuntu0.1.dsc 2561 SHA256:4f14aab7fb35be3b4de7b9c73074a632f956ea284c460b1d2453bb03af8e04ab
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.tar.xz' apt_1.6.12ubuntu0.1.tar.xz 2172208 SHA256:207daf6cdc6488b65e2b5bffbb721670ee7034507f3d9b460e36fff5668d0360
```

### `dpkg` source package: `at-spi2-atk=2.26.2-1`

Binary Packages:

- `libatk-bridge2.0-0:amd64=2.26.2-1`

Licenses: (parsed from: `/usr/share/doc/libatk-bridge2.0-0/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2`
- `LGPL-2+`
- `Unlimited`

Source:

```console
$ apt-get source -qq --print-uris at-spi2-atk=2.26.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/at-spi2-atk/at-spi2-atk_2.26.2-1.dsc' at-spi2-atk_2.26.2-1.dsc 2468 SHA256:526d85336524da7b738360cb1ce0bec6149bfdbeb74cba6d1449e1d3e2023244
'http://archive.ubuntu.com/ubuntu/pool/main/a/at-spi2-atk/at-spi2-atk_2.26.2.orig.tar.xz' at-spi2-atk_2.26.2.orig.tar.xz 322800 SHA256:61891f0abae1689f6617a963105a3f1dcdab5970c4a36ded9c79a7a544b16a6e
'http://archive.ubuntu.com/ubuntu/pool/main/a/at-spi2-atk/at-spi2-atk_2.26.2-1.debian.tar.xz' at-spi2-atk_2.26.2-1.debian.tar.xz 10020 SHA256:ce0bd67fb48f52cb700fde438d1a9bc7c25eadbd4c07698644f58d5053965ab6
```

### `dpkg` source package: `at-spi2-core=2.28.0-1`

Binary Packages:

- `libatspi2.0-0:amd64=2.28.0-1`

Licenses: (parsed from: `/usr/share/doc/libatspi2.0-0/copyright`)

- `AFL-2.1`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris at-spi2-core=2.28.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/at-spi2-core/at-spi2-core_2.28.0-1.dsc' at-spi2-core_2.28.0-1.dsc 2590 SHA256:4400bcbb8468c1070ee6b8a12d78b66a6882b88252148c63b7e9fdd092b1de27
'http://archive.ubuntu.com/ubuntu/pool/main/a/at-spi2-core/at-spi2-core_2.28.0.orig.tar.xz' at-spi2-core_2.28.0.orig.tar.xz 186676 SHA256:42a2487ab11ce43c288e73b2668ef8b1ab40a0e2b4f94e80fca04ad27b6f1c87
'http://archive.ubuntu.com/ubuntu/pool/main/a/at-spi2-core/at-spi2-core_2.28.0-1.debian.tar.xz' at-spi2-core_2.28.0-1.debian.tar.xz 7788 SHA256:41ede327a3fc89101903ffbde5bef3fe67782bdb0f1b2f62fe069bf6ce0ce861
```

### `dpkg` source package: `atk1.0=2.28.1-1`

Binary Packages:

- `libatk1.0-0:amd64=2.28.1-1`
- `libatk1.0-data=2.28.1-1`

Licenses: (parsed from: `/usr/share/doc/libatk1.0-0/copyright`, `/usr/share/doc/libatk1.0-data/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris atk1.0=2.28.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.28.1-1.dsc' atk1.0_2.28.1-1.dsc 2689 SHA256:b46a41c8d797d5e669a442e5ccddec346b0a2c3db0daa82716382cb8e1d5bdae
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.28.1.orig.tar.xz' atk1.0_2.28.1.orig.tar.xz 712508 SHA256:cd3a1ea6ecc268a2497f0cd018e970860de24a6d42086919d6bf6c8e8d53f4fc
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.28.1-1.debian.tar.xz' atk1.0_2.28.1-1.debian.tar.xz 11332 SHA256:375251cf6a420220a5d9facb9dd0b20cdf7506414802c103fdb662d0a5e1b70d
```

### `dpkg` source package: `attr=1:2.4.47-2build1`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2build1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2build1.dsc' attr_2.4.47-2build1.dsc 2033 SHA256:b78dbf07b789010caabc12c1ab0b2a944072058fe47ac6b5d345209c16f4e1f5
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2build1.debian.tar.xz' attr_2.4.47-2build1.debian.tar.xz 8168 SHA256:6732a8874190a1f792c7f9cb95fadc1dc852baf2e164b0d7b4bcea525f5c0882
```

### `dpkg` source package: `audit=1:2.8.2-1ubuntu1`

Binary Packages:

- `libaudit-common=1:2.8.2-1ubuntu1`
- `libaudit1:amd64=1:2.8.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2-1ubuntu1.dsc' audit_2.8.2-1ubuntu1.dsc 2903 SHA256:454c231dc2268ee4862f87d65720354699be9b807a411556a536bc2b4e581a90
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2.orig.tar.gz' audit_2.8.2.orig.tar.gz 1121970 SHA256:67b59b2b77afee9ed87afa4d80ffc8e6f3a1f4bbedd5f2871f387c952147bcba
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2-1ubuntu1.debian.tar.xz' audit_2.8.2-1ubuntu1.debian.tar.xz 21344 SHA256:2bc93230e3bf01eef5e9a5acff8f904af074e6e39003f1db8941118fbd041ec2
```

### `dpkg` source package: `avahi=0.7-3.1ubuntu1.2`

Binary Packages:

- `libavahi-client3:amd64=0.7-3.1ubuntu1.2`
- `libavahi-common-data:amd64=0.7-3.1ubuntu1.2`
- `libavahi-common3:amd64=0.7-3.1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.7-3.1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.7-3.1ubuntu1.2.dsc' avahi_0.7-3.1ubuntu1.2.dsc 4186 SHA256:7aa3692290fb1fbd04ca07b221b02eb861cfdbeeb35cf17cbdb7c81f6b02ed3c
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.7.orig.tar.gz' avahi_0.7.orig.tar.gz 1333400 SHA256:57a99b5dfe7fdae794e3d1ee7a62973a368e91e414bd0dfa5d84434de5b14804
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.7-3.1ubuntu1.2.debian.tar.xz' avahi_0.7-3.1ubuntu1.2.debian.tar.xz 35124 SHA256:a72a1652e00b4385f99407e4f26eb1656e8eb0026d127e246533438d1ae05407
```

### `dpkg` source package: `base-files=10.1ubuntu2.9`

Binary Packages:

- `base-files=10.1ubuntu2.9`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `base-passwd=3.5.44`

Binary Packages:

- `base-passwd=3.5.44`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.44
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.44.dsc' base-passwd_3.5.44.dsc 1685 SHA256:22a5db1e9bb71fa8a4d682b3f9c01470a61b8041eb6212471181c6808b268c13
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.44.tar.xz' base-passwd_3.5.44.tar.xz 52644 SHA256:f17a0746024572e86e60e4614cf226a81ffe682ceaf1a1fce9dc1a8002683e90
```

### `dpkg` source package: `bash=4.4.18-2ubuntu1.2`

Binary Packages:

- `bash=4.4.18-2ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.4.18-2ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.dsc' bash_4.4.18-2ubuntu1.2.dsc 2434 SHA256:febc739ab69e09853f8f1d4b1db7038937911bee7d715926f1e7ff461b63c82f
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18.orig.tar.xz' bash_4.4.18.orig.tar.xz 5036272 SHA256:704143a7170041ac9f1025455d6d23ff0f353711a3dc557b47d6e6322f24cd02
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.debian.tar.xz' bash_4.4.18-2ubuntu1.2.debian.tar.xz 65236 SHA256:b0191aab30dd0531d7acbeab7c64014a1c9e484f417678a18ad1655a77b7b6f9
```

### `dpkg` source package: `boost1.65.1=1.65.1+dfsg-0ubuntu5`

Binary Packages:

- `libboost-date-time1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-filesystem1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-iostreams1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-locale1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-system1.65.1:amd64=1.65.1+dfsg-0ubuntu5`
- `libboost-thread1.65.1:amd64=1.65.1+dfsg-0ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libboost-date-time1.65.1/copyright`, `/usr/share/doc/libboost-filesystem1.65.1/copyright`, `/usr/share/doc/libboost-iostreams1.65.1/copyright`, `/usr/share/doc/libboost-locale1.65.1/copyright`, `/usr/share/doc/libboost-system1.65.1/copyright`, `/usr/share/doc/libboost-thread1.65.1/copyright`)

- `Boost`
- `bjam`
- `boostbook`

Source:

```console
$ apt-get source -qq --print-uris boost1.65.1=1.65.1+dfsg-0ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.65.1/boost1.65.1_1.65.1+dfsg-0ubuntu5.dsc' boost1.65.1_1.65.1+dfsg-0ubuntu5.dsc 7825 SHA256:e046822facd57a5810416328f6e440f5ae5a4017215d1ea3ca7bec59e090c598
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.65.1/boost1.65.1_1.65.1+dfsg.orig.tar.bz2' boost1.65.1_1.65.1+dfsg.orig.tar.bz2 82120283 SHA256:c7709bf6b416e0609fac4bcc0c0093a890ccbeaeebbeabe45877cffc5d06f43c
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.65.1/boost1.65.1_1.65.1+dfsg-0ubuntu5.debian.tar.xz' boost1.65.1_1.65.1+dfsg-0ubuntu5.debian.tar.xz 105524 SHA256:c238e8a63c232911402cef6f8ea7763bddf572f7062b5353147ee9ed9a79afdb
```

### `dpkg` source package: `bzip2=1.0.6-8.1ubuntu0.2`

Binary Packages:

- `bzip2=1.0.6-8.1ubuntu0.2`
- `libbz2-1.0:amd64=1.0.6-8.1ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8.1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.dsc' bzip2_1.0.6-8.1ubuntu0.2.dsc 2181 SHA256:62f49d3ded30713bbae8a0aaab69bebdc5533afe6e488ceb0aa03bce7c2c5ff3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2' bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2 61477 SHA256:b4fede4240afa43e0e666e5a539da8d9744b2b2917388cfe93574f967e328e6a
```

### `dpkg` source package: `ca-certificates=20190110~18.04.1`

Binary Packages:

- `ca-certificates=20190110~18.04.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~18.04.1.dsc' ca-certificates_20190110~18.04.1.dsc 1830 SHA256:b5bcd791eb1c232b228766301a7513b404a376fe380c8b19bce504fd1f2312c6
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~18.04.1.tar.xz' ca-certificates_20190110~18.04.1.tar.xz 243664 SHA256:ec23bbc58d8e6bc8b6aa8c0a9081965635a54b474cfd99829e51e2aa25ca6550
```

### `dpkg` source package: `cairo=1.15.10-2ubuntu0.1`

Binary Packages:

- `libcairo-gobject2:amd64=1.15.10-2ubuntu0.1`
- `libcairo2:amd64=1.15.10-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.15.10-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10-2ubuntu0.1.dsc' cairo_1.15.10-2ubuntu0.1.dsc 2290 SHA256:f46a6d10e734d78f328bdf5505adec6e8283745a9aff395c506848f5a3346873
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10.orig.tar.xz' cairo_1.15.10.orig.tar.xz 41881364 SHA256:62ca226134cf2f1fd114bea06f8b374eb37f35d8e22487eaa54d5e9428958392
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10-2ubuntu0.1.debian.tar.xz' cairo_1.15.10-2ubuntu0.1.debian.tar.xz 31128 SHA256:5e23a8cf88a4cc11935ef84ef33661611cefafd72281ae20c58016a3788e1b5f
```

### `dpkg` source package: `cdebconf=0.213ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.213ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.213ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.213ubuntu1.dsc' cdebconf_0.213ubuntu1.dsc 2769 SHA256:76cb3f0b1685629220b0e4c3105757b95714f7350df4e7863d5310f1f581fee0
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.213ubuntu1.tar.xz' cdebconf_0.213ubuntu1.tar.xz 272596 SHA256:624feaf9e7e5f407271f99e06e54d5002fcce51345553a626caf7b4a65f0afd1
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/c/clucene-core/clucene-core_2.3.3.4+dfsg-1.dsc' clucene-core_2.3.3.4+dfsg-1.dsc 2019 SHA256:5158409a1b0c6913f82e5e0562ace6f3ff0cab197cf72b86e039b9fb9a73e1ed
'http://archive.ubuntu.com/ubuntu/pool/main/c/clucene-core/clucene-core_2.3.3.4+dfsg.orig.tar.xz' clucene-core_2.3.3.4+dfsg.orig.tar.xz 826688 SHA256:c70b8202c0afca27f9fa2f1a5d09a41bc4cc57a8f68c854379891ea2e24f1490
'http://archive.ubuntu.com/ubuntu/pool/main/c/clucene-core/clucene-core_2.3.3.4+dfsg-1.debian.tar.xz' clucene-core_2.3.3.4+dfsg-1.debian.tar.xz 8736 SHA256:a7d25d096e70105464a911e908fee7e5eb25adf3682ae75b1b514d6a5846b076
```

### `dpkg` source package: `colord=1.3.3-2build1`

Binary Packages:

- `libcolord2:amd64=1.3.3-2build1`

Licenses: (parsed from: `/usr/share/doc/libcolord2/copyright`)

- `CC0`
- `GFDL-NIV`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris colord=1.3.3-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/c/colord/colord_1.3.3-2build1.dsc' colord_1.3.3-2build1.dsc 2966 SHA256:67f8c4ae30f17b3096a6120169de439085f4d8d4186a7be3e2a2de7a0936645e
'http://archive.ubuntu.com/ubuntu/pool/main/c/colord/colord_1.3.3.orig.tar.xz' colord_1.3.3.orig.tar.xz 1240104 SHA256:d1848e797106a036b0d6ebed99a789a6ae07d60f1d9cc59be5b257efe7ec31a4
'http://archive.ubuntu.com/ubuntu/pool/main/c/colord/colord_1.3.3-2build1.debian.tar.xz' colord_1.3.3-2build1.debian.tar.xz 26840 SHA256:19064b1f189c5e0657fd5b0a461351fca19e492b0dea13304c39944b9f5f7687
```

### `dpkg` source package: `coreutils=8.28-1ubuntu1`

Binary Packages:

- `coreutils=8.28-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.28-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28-1ubuntu1.dsc' coreutils_8.28-1ubuntu1.dsc 2302 SHA256:9a7154fd8a458295b686383767f9305095e6ea929a08c8f56cf51640c3fe209f
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz' coreutils_8.28.orig.tar.xz 5252336 SHA256:1117b1a16039ddd84d51a9923948307cfa28c2cea03d1a2438742253df0a0c65
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz.asc' coreutils_8.28.orig.tar.xz.asc 1196 SHA256:505b1a530a55732a9ed659d419ff4973d1b15059078d2060675927058db9607d
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28-1ubuntu1.debian.tar.xz' coreutils_8.28-1ubuntu1.debian.tar.xz 37940 SHA256:71ba2e83edc675a79e1e0556aff326ab2ae812332692e3db29615e8ed1b427f4
```

### `dpkg` source package: `cups=2.2.7-1ubuntu2.8`

Binary Packages:

- `libcups2:amd64=2.2.7-1ubuntu2.8`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.2.7-1ubuntu2.8
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7-1ubuntu2.8.dsc' cups_2.2.7-1ubuntu2.8.dsc 3647 SHA256:da0dd48e993c1882c8c64407d7ddcfd04a471381d03fd2a02e6d14ef98e42d9a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7.orig.tar.gz' cups_2.2.7.orig.tar.gz 10330296 SHA256:3c4b637b737077565ccdfbd5f61785d03f49461ae736fcc2c0ffaf41d2c6ea6a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7.orig.tar.gz.asc' cups_2.2.7.orig.tar.gz.asc 872 SHA256:2b17bef166e1f8a0dece544c0e4f0d847f6d2c8e784298898966352f4e47581a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7-1ubuntu2.8.debian.tar.xz' cups_2.2.7-1ubuntu2.8.debian.tar.xz 363376 SHA256:eb062ea65e733f3c3bbe045c08477929a3cf02e6b6676586f8af72273ad2ddb9
```

### `dpkg` source package: `curl=7.58.0-2ubuntu3.10`

Binary Packages:

- `curl=7.58.0-2ubuntu3.10`
- `libcurl3-gnutls:amd64=7.58.0-2ubuntu3.10`
- `libcurl4:amd64=7.58.0-2ubuntu3.10`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.58.0-2ubuntu3.10
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.dsc' curl_7.58.0-2ubuntu3.10.dsc 2781 SHA256:0f80b3add0f3a8c471d1ae4f0aac8d473a3fcba72e9fba398355f16bfcd4615e
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0.orig.tar.gz' curl_7.58.0.orig.tar.gz 3879728 SHA256:cc245bf9a1a42a45df491501d97d5593392a03f7b4f07b952793518d97666115
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.debian.tar.xz' curl_7.58.0-2ubuntu3.10.debian.tar.xz 41908 SHA256:0aca9be6c8fdb0ab69b109b34d4424c99097c894ba8487fd7e28f83bc27f4850
```

### `dpkg` source package: `cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`
- `libsasl2-modules-db:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc 3297 SHA256:2f101f60d7c7245946f9ba90f29d3585b2ef7cb1593275001acb224feb7231e1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz 1143888 SHA256:69f34971f768e7ee6a6b647ec2d16a5a72a854ecd4602b019d5f79ba61063fdc
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz 95712 SHA256:a44bdbd8cfa996c30e617cd0d2fe292819511cc364f42b8169d334bfa7e28e1b
```

### `dpkg` source package: `d-conf=0.26.0-2ubuntu3`

Binary Packages:

- `dconf-gsettings-backend:amd64=0.26.0-2ubuntu3`
- `dconf-service=0.26.0-2ubuntu3`
- `libdconf1:amd64=0.26.0-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dconf-gsettings-backend/copyright`, `/usr/share/doc/dconf-service/copyright`, `/usr/share/doc/libdconf1/copyright`)

- `GPL-3`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris d-conf=0.26.0-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/d-conf/d-conf_0.26.0-2ubuntu3.dsc' d-conf_0.26.0-2ubuntu3.dsc 2043 SHA256:b7aa2a0d1b73d7a223f749cf5ec489611a4ed68d619984694f1cc7978db5d376
'http://archive.ubuntu.com/ubuntu/pool/main/d/d-conf/d-conf_0.26.0.orig.tar.xz' d-conf_0.26.0.orig.tar.xz 219688 SHA256:8683292eb31a3fae31e561f0a4220d8569b0f6d882e9958b68373f9043d658c9
'http://archive.ubuntu.com/ubuntu/pool/main/d/d-conf/d-conf_0.26.0-2ubuntu3.debian.tar.xz' d-conf_0.26.0-2ubuntu3.debian.tar.xz 9420 SHA256:2cf046f1e83bee9bb3585fb6fa47642126836d04058023f9eab833debdf7b4ce
```

### `dpkg` source package: `dash=0.5.8-2.10`

Binary Packages:

- `dash=0.5.8-2.10`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.8-2.10
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.10.dsc' dash_0.5.8-2.10.dsc 1618 SHA256:1e8fdac0880d57d8ed5eb11f9f1750a67c71a7200180cf3ed5aa3e74dab3e4c5
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8.orig.tar.gz' dash_0.5.8.orig.tar.gz 223028 SHA256:c6db3a237747b02d20382a761397563d813b306c020ae28ce25a1c3915fac60f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.10.debian.tar.xz' dash_0.5.8-2.10.debian.tar.xz 43920 SHA256:0d870b0cf9b3ad40e4d4f1e3d4d9097f4d62151693a48f34cb1d49865fd4abdb
```

### `dpkg` source package: `db5.3=5.3.28-13.1ubuntu1.1`

Binary Packages:

- `libdb5.3:amd64=5.3.28-13.1ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-13.1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.dsc' db5.3_5.3.28-13.1ubuntu1.1.dsc 3068 SHA256:1f438506524139f9cb87d3566a6f593186a6543070046e90e1c14c04740d7a0f
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz' db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz 29444 SHA256:d5b19e81a0d94bb29965b84e03855219b80b3bc782aea47e12ad2ace9995b099
```

### `dpkg` source package: `dbus-glib=0.110-2`

Binary Packages:

- `libdbus-glib-1-2:amd64=0.110-2`

Licenses: (parsed from: `/usr/share/doc/libdbus-glib-1-2/copyright`)

- `AFL-2.1`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dbus-glib=0.110-2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-glib/dbus-glib_0.110-2.dsc' dbus-glib_0.110-2.dsc 2601 SHA256:c9174cc67a04dd43ab5cc0811940836a4f1cf884c1c61b42da8acad1b42452bf
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-glib/dbus-glib_0.110.orig.tar.gz' dbus-glib_0.110.orig.tar.gz 836497 SHA256:7ce4760cf66c69148f6bd6c92feaabb8812dee30846b24cd0f7395c436d7e825
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-glib/dbus-glib_0.110.orig.tar.gz.asc' dbus-glib_0.110.orig.tar.gz.asc 833 SHA256:931761a795405539f0c976e3c8bd07b55f7e7f338037b828dd151096528e4aa4
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-glib/dbus-glib_0.110-2.debian.tar.xz' dbus-glib_0.110-2.debian.tar.xz 31200 SHA256:d5bbfd3eb875f8625b8a096f2e6ad2d95065e14dc2c4893b21fefa66f1c21aec
```

### `dpkg` source package: `dbus=1.12.2-1ubuntu1.2`

Binary Packages:

- `libdbus-1-3:amd64=1.12.2-1ubuntu1.2`

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
$ apt-get source -qq --print-uris dbus=1.12.2-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2-1ubuntu1.2.dsc' dbus_1.12.2-1ubuntu1.2.dsc 3561 SHA256:b32c5ff7b7e6ffb950839e5de9487bb40512b158477e1c47c1502a26752c3628
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2.orig.tar.gz' dbus_1.12.2.orig.tar.gz 2063143 SHA256:272bb5091770b047c8188b926d5e6038fa4fe6745488b2add96b23e2d9a83d88
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2-1ubuntu1.2.debian.tar.xz' dbus_1.12.2-1ubuntu1.2.debian.tar.xz 67596 SHA256:8a61cf6c3a0d8def6dc3e2405640e9eaaf8fb4532d670103f80cad3a48d20da2
```

### `dpkg` source package: `debconf=1.5.66ubuntu1`

Binary Packages:

- `debconf=1.5.66ubuntu1`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.66ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.dsc' debconf_1.5.66ubuntu1.dsc 2087 SHA256:6bc588eaa2e880ac33800384328b95a50542097baaba5e89d363798840bb05a2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.tar.xz' debconf_1.5.66ubuntu1.tar.xz 572556 SHA256:d044d6707a6f44a58022575899c852d256ee5b88f4e136f5394652f263e17a95
```

### `dpkg` source package: `debianutils=4.8.4`

Binary Packages:

- `debianutils=4.8.4`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.4
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.4.dsc' debianutils_4.8.4.dsc 1764 SHA256:8b12921fe6e4f51d295bfd4213706d588a6c9b8bab659b0ee1fe525f37e9fbcc
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.4.tar.xz' debianutils_4.8.4.tar.xz 156344 SHA256:c061ab99aea61f892043b7624b021ab5b193e9c6bbfd474da0fbcdd506be1eb2
```

### `dpkg` source package: `diffutils=1:3.6-1`

Binary Packages:

- `diffutils=1:3.6-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6-1.dsc' diffutils_3.6-1.dsc 1453 SHA256:26fe7690b45748dc92cee6af224192e78db2ac574e16ae0aeb8ed6a472c883cd
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6.orig.tar.xz' diffutils_3.6.orig.tar.xz 1398296 SHA256:d621e8bdd4b573918c8145f7ae61817d1be9deb4c8d2328a65cea8e11d783bd6
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6-1.debian.tar.xz' diffutils_3.6-1.debian.tar.xz 10808 SHA256:f6ab546a134bde18a87ca8e3c98919680e79d81a65a24801ae06ef69b33f24d8
```

### `dpkg` source package: `dpkg=1.19.0.5ubuntu2.3`

Binary Packages:

- `dpkg=1.19.0.5ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.0.5ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.dsc' dpkg_1.19.0.5ubuntu2.3.dsc 2144 SHA256:ac37d92c336bf4360cedce228d94ba4af248da265e5c161f33b06ed929fbe401
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.tar.xz' dpkg_1.19.0.5ubuntu2.3.tar.xz 4571256 SHA256:4945a605113fac66d275937b5de3678398f32ded55352cd773619c30ab1bd9a5
```

### `dpkg` source package: `e2fsprogs=1.44.1-1ubuntu1.3`

Binary Packages:

- `e2fsprogs=1.44.1-1ubuntu1.3`
- `libcom-err2:amd64=1.44.1-1ubuntu1.3`
- `libext2fs2:amd64=1.44.1-1ubuntu1.3`
- `libss2:amd64=1.44.1-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.44.1-1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.dsc' e2fsprogs_1.44.1-1ubuntu1.3.dsc 3188 SHA256:91385415b8464ff34676bb5129d6bd16e5db599b9a01ef82198e5f5517fd6191
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz' e2fsprogs_1.44.1.orig.tar.gz 7544908 SHA256:a5a8068dfe105050d8c63d67515a0ae5fff3f37232f725e0aa72b389eeb6c1e6
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz.asc' e2fsprogs_1.44.1.orig.tar.gz.asc 488 SHA256:6e8eb8df52f5cd577f5eae489108c6fbe2c5381e01f83c325873e034d5a84e46
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz' e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz 81152 SHA256:923cef16c7ce15022672ed0992f9ce9202f9331eead7c88b47bba52106189eac
```

### `dpkg` source package: `expat=2.2.5-3ubuntu0.2`

Binary Packages:

- `libexpat1:amd64=2.2.5-3ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.5-3ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.dsc' expat_2.2.5-3ubuntu0.2.dsc 2198 SHA256:680793c534c3f2ccee1251f6b03c445454250d320e31021a30f8b2fe571e75d5
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5.orig.tar.gz' expat_2.2.5.orig.tar.gz 8273003 SHA256:b3781742738611eaa737543ee94264dd511c52a3ba7e53111f7d705f6bff65a8
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.debian.tar.xz' expat_2.2.5-3ubuntu0.2.debian.tar.xz 12024 SHA256:9d9b040636ebf98fe3e401e6ebacc53073a2d508385bc91bde0fcb6b2aaa5675
```

### `dpkg` source package: `findutils=4.6.0+git+20170828-2`

Binary Packages:

- `findutils=4.6.0+git+20170828-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20170828-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828-2.dsc' findutils_4.6.0+git+20170828-2.dsc 2221 SHA256:6997072de2f1b24457073275f7b8f15ad2f0569389dcb277ebe99dd1846e2ee9
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828.orig.tar.xz' findutils_4.6.0+git+20170828.orig.tar.xz 1865192 SHA256:8d6571ffd5105307bcb1b20c4b7d5c2d0b5152e463b082801268bd3ec9e2bbfd
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828-2.debian.tar.xz' findutils_4.6.0+git+20170828-2.debian.tar.xz 26532 SHA256:5b13792a14edec982fddcf74fe01b4380b909703d76aaba2860da51c6248de73
```

### `dpkg` source package: `fontconfig=2.12.6-0ubuntu2`

Binary Packages:

- `fontconfig=2.12.6-0ubuntu2`
- `fontconfig-config=2.12.6-0ubuntu2`
- `libfontconfig1:amd64=2.12.6-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.12.6-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.12.6-0ubuntu2.dsc' fontconfig_2.12.6-0ubuntu2.dsc 2384 SHA256:e7109f728f73761ad17ff5c5ec066ad940b67b779a78a094b67a7af4cfafadcc
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.12.6.orig.tar.bz2' fontconfig_2.12.6.orig.tar.bz2 1624683 SHA256:cf0c30807d08f6a28ab46c61b8dbd55c97d2f292cf88f3a07d3384687f31f017
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.12.6-0ubuntu2.debian.tar.xz' fontconfig_2.12.6-0ubuntu2.debian.tar.xz 29168 SHA256:75c259e2d6b1944fe76a49f89b806b3ee34fe7a42eb25efd289e38b1b5e16517
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.dsc' fonts-dejavu_2.37-1.dsc 2575 SHA256:f35ff7b2c8dbfda6564c9dedf088ba06cc6d279fdd8e7cccbd1ae08ded1bb71c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.debian.tar.xz' fonts-dejavu_2.37-1.debian.tar.xz 10424 SHA256:5105cdbfc086f4a83ab6871eb39cc904bf02aa52762402b7cacf33d0938122f7
```

### `dpkg` source package: `freetype=2.8.1-2ubuntu2`

Binary Packages:

- `libfreetype6:amd64=2.8.1-2ubuntu2`

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
$ apt-get source -qq --print-uris freetype=2.8.1-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1-2ubuntu2.dsc' freetype_2.8.1-2ubuntu2.dsc 2288 SHA256:f7a1e8715cc35405d814fd97478e37ff22fad2bb639c049e058298c9f5847015
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1.orig.tar.gz' freetype_2.8.1.orig.tar.gz 4242784 SHA256:a7531cb8c2f6b709896f018380ad97e677e243847ff8a098d1b8b5d23e9d74d7
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1-2ubuntu2.diff.gz' freetype_2.8.1-2ubuntu2.diff.gz 44335 SHA256:ec498da97b3c1715b67f8d6ed85e6d9a2eb8b709cabce38519a8ab5ca995b85a
```

### `dpkg` source package: `gcc-8=8.4.0-1ubuntu1~18.04`

Binary Packages:

- `gcc-8-base:amd64=8.4.0-1ubuntu1~18.04`
- `libgcc1:amd64=1:8.4.0-1ubuntu1~18.04`
- `libstdc++6:amd64=8.4.0-1ubuntu1~18.04`

Licenses: (parsed from: `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-8=8.4.0-1ubuntu1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.dsc' gcc-8_8.4.0-1ubuntu1~18.04.dsc 36382 SHA256:bf7f453948fc746550c79b00c0af3940a2ff00c2f1692a376ebb90393963355a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0.orig.tar.gz' gcc-8_8.4.0.orig.tar.gz 85278215 SHA256:eb917ceb079e90afe1e524dee295e2360c63b923c611ae231144385be37dde2a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.diff.gz' gcc-8_8.4.0-1ubuntu1~18.04.diff.gz 510634 SHA256:5dbda7df03e650d72ad7c54ad8d8a48389ee358ebfad18a40bf6d8bb57c8c2ad
```

### `dpkg` source package: `gdk-pixbuf=2.36.11-2`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.36.11-2`
- `libgdk-pixbuf2.0-common=2.36.11-2`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.36.11-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.11-2.dsc' gdk-pixbuf_2.36.11-2.dsc 2886 SHA256:6c6482b64d3b15bf893d6b3dc1864ab49f92ee994736d53ce84a3d052d57e6c4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.11.orig.tar.xz' gdk-pixbuf_2.36.11.orig.tar.xz 5675908 SHA256:ae62ab87250413156ed72ef756347b10208c00e76b222d82d9ed361ed9dde2f3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.11-2.debian.tar.xz' gdk-pixbuf_2.36.11-2.debian.tar.xz 15204 SHA256:064020524e80e3ac713dd6bdf861660df26c61d9aceb75be74df44a9979c0a0c
```

### `dpkg` source package: `glib-networking=2.56.0-1ubuntu0.1`

Binary Packages:

- `glib-networking:amd64=2.56.0-1ubuntu0.1`
- `glib-networking-common=2.56.0-1ubuntu0.1`
- `glib-networking-services=2.56.0-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/glib-networking/copyright`, `/usr/share/doc/glib-networking-common/copyright`, `/usr/share/doc/glib-networking-services/copyright`)

- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris glib-networking=2.56.0-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib-networking/glib-networking_2.56.0-1ubuntu0.1.dsc' glib-networking_2.56.0-1ubuntu0.1.dsc 2320 SHA256:749930ca467491bfe2c9d907c031a34d4492759adaca01cb5a1f3d84a31eb036
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib-networking/glib-networking_2.56.0.orig.tar.xz' glib-networking_2.56.0.orig.tar.xz 163852 SHA256:47fd10bcae2e5039dc5f685e3ea384f48e64a6bee26d755718f534a978477c93
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib-networking/glib-networking_2.56.0-1ubuntu0.1.debian.tar.xz' glib-networking_2.56.0-1ubuntu0.1.debian.tar.xz 31224 SHA256:934c32861afb7162a28b39d1554488a75845eb7366da656e3f864476541e752d
```

### `dpkg` source package: `glib2.0=2.56.4-0ubuntu0.18.04.6`

Binary Packages:

- `libglib2.0-0:amd64=2.56.4-0ubuntu0.18.04.6`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.56.4-0ubuntu0.18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.dsc' glib2.0_2.56.4-0ubuntu0.18.04.6.dsc 3301 SHA256:a4cc68dbc3255f458789213e5eaa1ff1c409d8fc49688c9b136cfa4ef30dafa1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4.orig.tar.xz' glib2.0_2.56.4.orig.tar.xz 7029768 SHA256:27f703d125efb07f8a743666b580df0b4095c59fc8750e8890132c91d437504c
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz' glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz 89540 SHA256:57f17e1760946894ae729e988798ac11339460e8ee71421c6b0a5b6cdde9af36
```

### `dpkg` source package: `glibc=2.27-3ubuntu1.2`

Binary Packages:

- `libc-bin=2.27-3ubuntu1.2`
- `libc6:amd64=2.27-3ubuntu1.2`
- `locales=2.27-3ubuntu1.2`
- `multiarch-support=2.27-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/locales/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.27-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.2.dsc' glibc_2.27-3ubuntu1.2.dsc 9364 SHA256:2ac325cce2251c710dd041f4725925cdbccefba6f6f0f0d95a2a5a09e2050c2e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27.orig.tar.xz' glibc_2.27.orig.tar.xz 15923832 SHA256:0e9826488e3ffedb4d14a426d741b7b1cf15f6973ab30762af9a188ad47633ed
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.2.debian.tar.xz' glibc_2.27-3ubuntu1.2.debian.tar.xz 1014508 SHA256:e488a6293dfb3b8074b9be03655ffd3c98f2d0a5b8bb2a29cf4c526fbf01dcb0
```

### `dpkg` source package: `gmp=2:6.1.2+dfsg-2`

Binary Packages:

- `libgmp10:amd64=2:6.1.2+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-2.dsc' gmp_6.1.2+dfsg-2.dsc 2152 SHA256:d1e7b69c619c2d07b3eaf9f051159cde1884cf9c68109f1dee278bf7a59b632b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-2.debian.tar.xz' gmp_6.1.2+dfsg-2.debian.tar.xz 20744 SHA256:33cf6cc65827c9df744e4e07b216ca2d02eb57327a949f80a7b7dddd0485ee85
```

### `dpkg` source package: `gnupg2=2.2.4-1ubuntu1.2`

Binary Packages:

- `dirmngr=2.2.4-1ubuntu1.2`
- `gnupg=2.2.4-1ubuntu1.2`
- `gnupg-l10n=2.2.4-1ubuntu1.2`
- `gnupg-utils=2.2.4-1ubuntu1.2`
- `gpg=2.2.4-1ubuntu1.2`
- `gpg-agent=2.2.4-1ubuntu1.2`
- `gpg-wks-client=2.2.4-1ubuntu1.2`
- `gpg-wks-server=2.2.4-1ubuntu1.2`
- `gpgconf=2.2.4-1ubuntu1.2`
- `gpgsm=2.2.4-1ubuntu1.2`
- `gpgv=2.2.4-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-l10n/copyright`, `/usr/share/doc/gnupg-utils/copyright`, `/usr/share/doc/gpg/copyright`, `/usr/share/doc/gpg-agent/copyright`, `/usr/share/doc/gpg-wks-client/copyright`, `/usr/share/doc/gpg-wks-server/copyright`, `/usr/share/doc/gpgconf/copyright`, `/usr/share/doc/gpgsm/copyright`, `/usr/share/doc/gpgv/copyright`)

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
$ apt-get source -qq --print-uris gnupg2=2.2.4-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4-1ubuntu1.2.dsc' gnupg2_2.2.4-1ubuntu1.2.dsc 3816 SHA256:3b5821e3a8c95653140d0bbc791098ab6c08d6fc7206857a21b25e291e79f2bc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4.orig.tar.bz2' gnupg2_2.2.4.orig.tar.bz2 6571487 SHA256:401a3e64780fdfa6d7670de0880aa5c9d589b3db7a7098979d7606cec546f2ec
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4.orig.tar.bz2.asc' gnupg2_2.2.4.orig.tar.bz2.asc 952 SHA256:30dd26e12b451e8f6799ba3a81449ed18db3d3e747820b237a39745ab264c899
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4-1ubuntu1.2.debian.tar.bz2' gnupg2_2.2.4-1ubuntu1.2.debian.tar.bz2 82238 SHA256:ad2e70205e5d5f52c092c58e619ee58e5f5bc2b44f44a2c462296fc34a1960de
```

### `dpkg` source package: `gnutls28=3.5.18-1ubuntu1.4`

Binary Packages:

- `libgnutls30:amd64=3.5.18-1ubuntu1.4`

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
$ apt-get source -qq --print-uris gnutls28=3.5.18-1ubuntu1.4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.dsc' gnutls28_3.5.18-1ubuntu1.4.dsc 2780 SHA256:6c58a44e5790eb86989318bf660e2391561c04518d4d8c7b85fb495a4efcd5ae
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz' gnutls28_3.5.18.orig.tar.xz 7261980 SHA256:ae2248d9e78747cf9c469dde81ff8f90b56838b707a0637f3f7d4eee90e80234
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz.asc' gnutls28_3.5.18.orig.tar.xz.asc 534 SHA256:50bb942469be0639bbab925de630fb921aa8cac5f40072cb1c2cf1fb7ae7977b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz' gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz 83784 SHA256:3ff4cbd5e9b6d9d51479fdae70486598ad7c11dae50aa06e98f000290f30cd05
```

### `dpkg` source package: `gpgme1.0=1.10.0-1ubuntu2`

Binary Packages:

- `libgpgme11:amd64=1.10.0-1ubuntu2`
- `libgpgmepp6:amd64=1.10.0-1ubuntu2`

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
$ apt-get source -qq --print-uris gpgme1.0=1.10.0-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0-1ubuntu2.dsc' gpgme1.0_1.10.0-1ubuntu2.dsc 3046 SHA256:fe60f76894d4f8b089e456762978f7fb5e78592cf0fa039b8980edca72c3448b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0.orig.tar.bz2' gpgme1.0_1.10.0.orig.tar.bz2 1370162 SHA256:1a8fed1197c3b99c35f403066bb344a26224d292afc048cfdfc4ccd5690a0693
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0.orig.tar.bz2.asc' gpgme1.0_1.10.0.orig.tar.bz2.asc 534 SHA256:a7058cd592ae81c35fc05bcc6b32019a025ab5ef65a01402ceeb533a104a50b5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0-1ubuntu2.debian.tar.xz' gpgme1.0_1.10.0-1ubuntu2.debian.tar.xz 18372 SHA256:792b744cc5b0a8af5f125641e5bc4a86c3862b7a9cf3ae6ba74ee0f16d3553c1
```

### `dpkg` source package: `graphite2=1.3.11-2`

Binary Packages:

- `libgraphite2-3:amd64=1.3.11-2`

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
$ apt-get source -qq --print-uris graphite2=1.3.11-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11-2.dsc' graphite2_1.3.11-2.dsc 2367 SHA256:3c2f5ed2b6021e9a18456215d5d01354434f14577dbc862f7f53c8ce62200d71
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11.orig.tar.gz' graphite2_1.3.11.orig.tar.gz 4236768 SHA256:945c01d3647b355d68e5541773fc99a7f29ede6a264bcbd735156a7c493459ff
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11-2.debian.tar.xz' graphite2_1.3.11-2.debian.tar.xz 14068 SHA256:c47ef4ae6edfa6ce02483f347e67786b0fce089515087370ccc10f22ad711f90
```

### `dpkg` source package: `grep=3.1-2build1`

Binary Packages:

- `grep=3.1-2build1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.dsc' grep_3.1-2build1.dsc 2116 SHA256:b9dff3a4089e3491a057c76fe2d941bbc669c1f9d934f5929052d32abd952961
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1.orig.tar.xz' grep_3.1.orig.tar.xz 1370880 SHA256:db625c7ab3bb3ee757b3926a5cfa8d9e1c3991ad24707a83dde8a5ef2bf7a07e
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.debian.tar.bz2' grep_3.1-2build1.debian.tar.bz2 110087 SHA256:699bbd6681e4ef27a24b9876b6b2c3b1ce1be1b140676cd051170e5cc05dd876
```

### `dpkg` source package: `gsettings-desktop-schemas=3.28.0-1ubuntu1`

Binary Packages:

- `gsettings-desktop-schemas=3.28.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gsettings-desktop-schemas/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gsettings-desktop-schemas=3.28.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.28.0-1ubuntu1.dsc' gsettings-desktop-schemas_3.28.0-1ubuntu1.dsc 2632 SHA256:c622e78d2a4e984573fc9360359de3aa1251567c823d6b7cea33d810aad67be5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.28.0.orig.tar.xz' gsettings-desktop-schemas_3.28.0.orig.tar.xz 648296 SHA256:4cb4cd7790b77e5542ec75275237613ad22f3a1f2f41903a298cf6cc996a9167
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsettings-desktop-schemas/gsettings-desktop-schemas_3.28.0-1ubuntu1.debian.tar.xz' gsettings-desktop-schemas_3.28.0-1ubuntu1.debian.tar.xz 7644 SHA256:149a50f92971df5794ff431f68ceaea1a9b84dd3a472bfee62957cbee4f2a9d7
```

### `dpkg` source package: `gst-plugins-base1.0=1.14.5-0ubuntu1~18.04.1`

Binary Packages:

- `libgstreamer-plugins-base1.0-0:amd64=1.14.5-0ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer-plugins-base1.0-0/copyright`)

- `BSD (2 clause)`
- `BSD (3 clause)`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`
- `MIT/X11 (BSD like) LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gst-plugins-base1.0=1.14.5-0ubuntu1~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.dsc' gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.dsc 4444 SHA256:ba08578352c3f032120647a591a189fced869eb4123874c74806c8f90f4a49c9
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.5.orig.tar.xz' gst-plugins-base1.0_1.14.5.orig.tar.xz 3717076 SHA256:7bfa9b329ea7f3c654fa1b2d43650bf2646598a5e3cb21f42c516b7e975d638e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz' gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz 45600 SHA256:55b60c10a296977b5c52b2dd333a5a2f505e9f32ead87f73423c7fece0ea1ef7
```

### `dpkg` source package: `gstreamer1.0=1.14.5-0ubuntu1~18.04.1`

Binary Packages:

- `libgstreamer1.0-0:amd64=1.14.5-0ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/libgstreamer1.0-0/copyright`)

- `GPL-2+`
- `GPL-3+`
- `LGPL`
- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gstreamer1.0=1.14.5-0ubuntu1~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.5-0ubuntu1~18.04.1.dsc' gstreamer1.0_1.14.5-0ubuntu1~18.04.1.dsc 3052 SHA256:5a657bab269dde8bf08f0a3df510794ed59211f850a5792f10d1c90d26657462
'http://archive.ubuntu.com/ubuntu/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.5.orig.tar.xz' gstreamer1.0_1.14.5.orig.tar.xz 3268756 SHA256:e40888752883177e97b2d90cd68591f87ccd213dc0178ff721d80a4cdaad34b5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz' gstreamer1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz 44584 SHA256:b181b69ec4f952848efef822105aa4ab6b0acab54ade8d859fa3a3642824075d
```

### `dpkg` source package: `gtk+3.0=3.22.30-1ubuntu4`

Binary Packages:

- `gtk-update-icon-cache=3.22.30-1ubuntu4`
- `libgtk-3-0:amd64=3.22.30-1ubuntu4`
- `libgtk-3-common=3.22.30-1ubuntu4`

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
$ apt-get source -qq --print-uris gtk+3.0=3.22.30-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+3.0/gtk+3.0_3.22.30-1ubuntu4.dsc' gtk+3.0_3.22.30-1ubuntu4.dsc 3364 SHA256:f4b7cbc787b8e65d02186f43ba78935040bbb5381693da8aa8455a9fc1436e9e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+3.0/gtk+3.0_3.22.30.orig.tar.xz' gtk+3.0_3.22.30.orig.tar.xz 18946084 SHA256:a1a4a5c12703d4e1ccda28333b87ff462741dc365131fbc94c218ae81d9a6567
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+3.0/gtk+3.0_3.22.30-1ubuntu4.debian.tar.xz' gtk+3.0_3.22.30-1ubuntu4.debian.tar.xz 162544 SHA256:24bc3d5c670bb77840ee5cc83d39970aee76a3364ff6422b9ebaeac4bc7a6292
```

### `dpkg` source package: `gzip=1.6-5ubuntu1`

Binary Packages:

- `gzip=1.6-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-5ubuntu1.dsc' gzip_1.6-5ubuntu1.dsc 2023 SHA256:439e340fce084b9b30e22a5537712f9b4727a20e77952addeea7633a4e9ef073
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-5ubuntu1.debian.tar.xz' gzip_1.6-5ubuntu1.debian.tar.xz 15516 SHA256:db01e3f2195cf0ebcf43ad38d07a70059b6b5b292706f2412de34928b9146db5
```

### `dpkg` source package: `harfbuzz=1.7.2-1ubuntu1`

Binary Packages:

- `libharfbuzz-icu0:amd64=1.7.2-1ubuntu1`
- `libharfbuzz0b:amd64=1.7.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz-icu0/copyright`, `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=1.7.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2-1ubuntu1.dsc' harfbuzz_1.7.2-1ubuntu1.dsc 2825 SHA256:0222317c07eecbb164a537694dcb01ff4c658a56e577f9667cbb8ec144d287fa
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2.orig.tar.bz2' harfbuzz_1.7.2.orig.tar.bz2 1708416 SHA256:a790585e35c1a87f0dcc23580c84b7cc2324e6f67a2946178d278c2a36c790cb
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2-1ubuntu1.debian.tar.xz' harfbuzz_1.7.2-1ubuntu1.debian.tar.xz 9168 SHA256:f94a2a0990fd0b39fdef14444fa39b0bd1d15f6c79e74b697856ba2cef06b0bf
```

### `dpkg` source package: `heimdal=7.5.0+dfsg-1`

Binary Packages:

- `libasn1-8-heimdal:amd64=7.5.0+dfsg-1`
- `libgssapi3-heimdal:amd64=7.5.0+dfsg-1`
- `libhcrypto4-heimdal:amd64=7.5.0+dfsg-1`
- `libheimbase1-heimdal:amd64=7.5.0+dfsg-1`
- `libheimntlm0-heimdal:amd64=7.5.0+dfsg-1`
- `libhx509-5-heimdal:amd64=7.5.0+dfsg-1`
- `libkrb5-26-heimdal:amd64=7.5.0+dfsg-1`
- `libroken18-heimdal:amd64=7.5.0+dfsg-1`
- `libwind0-heimdal:amd64=7.5.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libasn1-8-heimdal/copyright`, `/usr/share/doc/libgssapi3-heimdal/copyright`, `/usr/share/doc/libhcrypto4-heimdal/copyright`, `/usr/share/doc/libheimbase1-heimdal/copyright`, `/usr/share/doc/libheimntlm0-heimdal/copyright`, `/usr/share/doc/libhx509-5-heimdal/copyright`, `/usr/share/doc/libkrb5-26-heimdal/copyright`, `/usr/share/doc/libroken18-heimdal/copyright`, `/usr/share/doc/libwind0-heimdal/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `custom`
- `none`

Source:

```console
$ apt-get source -qq --print-uris heimdal=7.5.0+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-1.dsc' heimdal_7.5.0+dfsg-1.dsc 3674 SHA256:98ce6bf21ac01400ec10a3620fe3c047da4cf63269f521ba96c59bbcaed822bf
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg.orig.tar.gz' heimdal_7.5.0+dfsg.orig.tar.gz 8955005 SHA256:489119b7a1a900b88163765654dc59cba9a321b078fafc76629e2b85ef140867
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-1.debian.tar.xz' heimdal_7.5.0+dfsg-1.debian.tar.xz 125776 SHA256:7ad6c3f3968989ff06181409e1515a3feaf5a630d27ade7f2f018c9241f8c225
```

### `dpkg` source package: `hicolor-icon-theme=0.17-2`

Binary Packages:

- `hicolor-icon-theme=0.17-2`

Licenses: (parsed from: `/usr/share/doc/hicolor-icon-theme/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris hicolor-icon-theme=0.17-2
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.dsc' hicolor-icon-theme_0.17-2.dsc 2053 SHA256:9df02b466f82cd6fa13930bc197d001ed8ddac1abc7f8dde3db45ed1708336bd
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17.orig.tar.xz' hicolor-icon-theme_0.17.orig.tar.xz 53016 SHA256:317484352271d18cbbcfac3868eab798d67fff1b8402e740baa6ff41d588a9d8
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.debian.tar.xz' hicolor-icon-theme_0.17-2.debian.tar.xz 3536 SHA256:97eec9852a2923b95bd13fc59c30fb1b9063ffd1f8a04748544d4975a84e98f2
```

### `dpkg` source package: `hostname=3.20`

Binary Packages:

- `hostname=3.20`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.20
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.20.dsc' hostname_3.20.dsc 1429 SHA256:1fd7b0b2b61e58aa0e50de4d375072c938cb3cc4b722bc73e085e3a3691d9114
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.20.tar.gz' hostname_3.20.tar.gz 13336 SHA256:e7ed56f8c532573ff34d9bd6e7a10d04fbbb2c7fae187898805868e5fed24ab0
```

### `dpkg` source package: `humanity-icon-theme=0.6.15`

Binary Packages:

- `humanity-icon-theme=0.6.15`

Licenses: (parsed from: `/usr/share/doc/humanity-icon-theme/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris humanity-icon-theme=0.6.15
'http://archive.ubuntu.com/ubuntu/pool/main/h/humanity-icon-theme/humanity-icon-theme_0.6.15.dsc' humanity-icon-theme_0.6.15.dsc 1631 SHA256:cc3387acdf0e27443d7d3ec65dd07ad691421f46134493279a5f92d0a7706d1a
'http://archive.ubuntu.com/ubuntu/pool/main/h/humanity-icon-theme/humanity-icon-theme_0.6.15.tar.xz' humanity-icon-theme_0.6.15.tar.xz 1755216 SHA256:9dbcb425c2ee2a58c70da1eda4c2c88e32e7ede4094fb59772726864c8214aa6
```

### `dpkg` source package: `hunspell=1.6.2-1`

Binary Packages:

- `libhunspell-1.6-0:amd64=1.6.2-1`

Licenses: (parsed from: `/usr/share/doc/libhunspell-1.6-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris hunspell=1.6.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/h/hunspell/hunspell_1.6.2-1.dsc' hunspell_1.6.2-1.dsc 2241 SHA256:2b484c0f869a0cab2521a9b37de3547bd94650fde91eed918b68df62ccb58f16
'http://archive.ubuntu.com/ubuntu/pool/main/h/hunspell/hunspell_1.6.2.orig.tar.gz' hunspell_1.6.2.orig.tar.gz 721165 SHA256:3cd9ceb062fe5814f668e4f22b2fa6e3ba0b339b921739541ce180cac4d6f4c4
'http://archive.ubuntu.com/ubuntu/pool/main/h/hunspell/hunspell_1.6.2-1.debian.tar.xz' hunspell_1.6.2-1.debian.tar.xz 21800 SHA256:bd6afc139891e889436f63a2be665015ca5f98a1a56e85e3c94287223a032cf8
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/h/hyphen/hyphen_2.8.8-5.dsc' hyphen_2.8.8-5.dsc 2097 SHA256:f2d4b3129b865d87babdb4fa1142e9b3dafd7cc9739c1fbf534a09e8a64e936b
'http://archive.ubuntu.com/ubuntu/pool/main/h/hyphen/hyphen_2.8.8.orig.tar.gz' hyphen_2.8.8.orig.tar.gz 638369 SHA256:304636d4eccd81a14b6914d07b84c79ebb815288c76fe027b9ebff6ff24d5705
'http://archive.ubuntu.com/ubuntu/pool/main/h/hyphen/hyphen_2.8.8-5.debian.tar.xz' hyphen_2.8.8-5.debian.tar.xz 12012 SHA256:ab8848f6e7cd71a6f806ab17c51c871f773e4d0ad58bb02b75bdd051c001460e
```

### `dpkg` source package: `icu=60.2-3ubuntu3.1`

Binary Packages:

- `libicu60:amd64=60.2-3ubuntu3.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=60.2-3ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.dsc' icu_60.2-3ubuntu3.1.dsc 2149 SHA256:eb8ac79f5fdbd30cfedbf8e5f2c3997dac813115aab9b583dfeced859889ac57
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2.orig.tar.gz' icu_60.2.orig.tar.gz 23315541 SHA256:a8c2ddbdf2be01c7ddcfded837afe46362e1069ea6093f66816b2d1caa8272ae
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.debian.tar.xz' icu_60.2-3ubuntu3.1.debian.tar.xz 29068 SHA256:b93559560abae724d3466f3d84a362282f97bb6562a82e99da06846f0dc6c09c
```

### `dpkg` source package: `init-system-helpers=1.51`

Binary Packages:

- `init-system-helpers=1.51`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.51
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.51.dsc' init-system-helpers_1.51.dsc 1963 SHA256:82f0e30fef2ad14c65f9c7d8ccafd43549451041fdf661dca28b963a6cef02e4
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.51.tar.xz' init-system-helpers_1.51.tar.xz 37468 SHA256:e18b28efe8df087146d9c1e4e9c25386ee1b7312f518d48a2a38469a6c661be0
```

### `dpkg` source package: `iso-codes=3.79-1`

Binary Packages:

- `iso-codes=3.79-1`

Licenses: (parsed from: `/usr/share/doc/iso-codes/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris iso-codes=3.79-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/iso-codes/iso-codes_3.79-1.dsc' iso-codes_3.79-1.dsc 1977 SHA256:54a35ab10e61cc41f2d2e31c8b49d7374ce734cf49d25e9ef65149dffdd2f5ab
'http://archive.ubuntu.com/ubuntu/pool/main/i/iso-codes/iso-codes_3.79.orig.tar.xz' iso-codes_3.79.orig.tar.xz 3576536 SHA256:cbafd36cd4c588a254c0a5c42e682190c3784ceaf2a098da4c9c4a0cbc842822
'http://archive.ubuntu.com/ubuntu/pool/main/i/iso-codes/iso-codes_3.79-1.debian.tar.xz' iso-codes_3.79-1.debian.tar.xz 23716 SHA256:e2e82661eb94a32d31e6b5a0e07953712955339b15aaa640b5db1a0df0561253
```

### `dpkg` source package: `jbigkit=2.1-3.1build1`

Binary Packages:

- `libjbig0:amd64=2.1-3.1build1`

Licenses: (parsed from: `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.dsc' jbigkit_2.1-3.1build1.dsc 2085 SHA256:fc768c7dac53f37f89c8d0a25760a29cd9afffc5cf55821f92d0d7e8f8f26e38
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.debian.tar.xz' jbigkit_2.1-3.1build1.debian.tar.xz 7672 SHA256:d7151df94f409045aa4d27dab88e538398196330d1ce135b60564dbc5db0a5c4
```

### `dpkg` source package: `json-glib=1.4.2-3ubuntu0.18.04.1`

Binary Packages:

- `libjson-glib-1.0-0:amd64=1.4.2-3ubuntu0.18.04.1`
- `libjson-glib-1.0-common=1.4.2-3ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libjson-glib-1.0-0/copyright`, `/usr/share/doc/libjson-glib-1.0-common/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris json-glib=1.4.2-3ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-glib/json-glib_1.4.2-3ubuntu0.18.04.1.dsc' json-glib_1.4.2-3ubuntu0.18.04.1.dsc 2112 SHA256:8b7e878616e72e7da2a91cbf8bcd5e4573bf6f199ec56eb5d68b70308236e4da
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-glib/json-glib_1.4.2.orig.tar.xz' json-glib_1.4.2.orig.tar.xz 148404 SHA256:ea185056d95f26a549590677cb532a0b2955e58b118b4486d6587ee9ccaf73c1
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-glib/json-glib_1.4.2-3ubuntu0.18.04.1.debian.tar.xz' json-glib_1.4.2-3ubuntu0.18.04.1.debian.tar.xz 9072 SHA256:3f793d1decf6f82ea5b3b0e099bbea5009793d39933ecc1ded1f0b02a30394be
```

### `dpkg` source package: `keyutils=1.5.9-9.2ubuntu2`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-9.2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-9.2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-9.2ubuntu2.dsc' keyutils_1.5.9-9.2ubuntu2.dsc 2237 SHA256:67cb7c4b1dadc2c0ca85286ef8f11f7e71f91b67d47fca58ecd41e1bd83271ad
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-9.2ubuntu2.debian.tar.xz' keyutils_1.5.9-9.2ubuntu2.debian.tar.xz 18492 SHA256:51706bd0d480913584d3fa8fcfe32dcf210742bb75c08e6a2d5f022748654086
```

### `dpkg` source package: `krb5=1.16-2ubuntu0.1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.16-2ubuntu0.1`
- `libk5crypto3:amd64=1.16-2ubuntu0.1`
- `libkrb5-3:amd64=1.16-2ubuntu0.1`
- `libkrb5support0:amd64=1.16-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.16-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.1.dsc' krb5_1.16-2ubuntu0.1.dsc 3563 SHA256:2c955da3464e506961ee80a769bd5139b2df6770ed51947a510f48f451be70c0
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16.orig.tar.gz' krb5_1.16.orig.tar.gz 9474479 SHA256:faeb125f83b0fb4cdb2f99f088140631bb47d975982de0956d18c85842969e08
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.1.debian.tar.xz' krb5_1.16-2ubuntu0.1.debian.tar.xz 99820 SHA256:9e3a973805af340fab23cd28737187567214adb98452d1564ada05652036fc0c
```

### `dpkg` source package: `lcms2=2.9-1ubuntu0.1`

Binary Packages:

- `liblcms2-2:amd64=2.9-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.9-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-1ubuntu0.1.dsc' lcms2_2.9-1ubuntu0.1.dsc 2084 SHA256:aac9c6cc63af8c4587ff51c7b69babe48d8283181818934639a3bd958e4145cb
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9.orig.tar.gz' lcms2_2.9.orig.tar.gz 10974649 SHA256:48c6fdf98396fa245ed86e622028caf49b96fa22f3e5734f853f806fbc8e7d20
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-1ubuntu0.1.debian.tar.xz' lcms2_2.9-1ubuntu0.1.debian.tar.xz 10680 SHA256:b541cee04359249b80f3313522f1ff5d9175e787e0320a510fac7cd4640a5bfc
```

### `dpkg` source package: `libabw=0.1.2-1ubuntu1`

Binary Packages:

- `libabw-0.1-1:amd64=0.1.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libabw-0.1-1/copyright`)

- `GPL-3`
- `LGPL-3`
- `MPL-1.1 | GPL-3 | LGPL-3`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libabw=0.1.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libabw/libabw_0.1.2-1ubuntu1.dsc' libabw_0.1.2-1ubuntu1.dsc 2060 SHA256:ac95d42a37361b66355570a4f522992ab983068722c265812636f48c15490ab5
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libabw/libabw_0.1.2.orig.tar.xz' libabw_0.1.2.orig.tar.xz 318400 SHA256:0b72944d5af81dda0a5c5803ee84cbac4b81441a4d767aa57029adc6744c2485
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libabw/libabw_0.1.2-1ubuntu1.debian.tar.xz' libabw_0.1.2-1ubuntu1.debian.tar.xz 13304 SHA256:b977eeca95b2b492db06a227ec360e994f66c13cfe3b94c5d589d4d0c35d43ff
```

### `dpkg` source package: `libassuan=2.5.1-2`

Binary Packages:

- `libassuan0:amd64=2.5.1-2`

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
$ apt-get source -qq --print-uris libassuan=2.5.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1-2.dsc' libassuan_2.5.1-2.dsc 2215 SHA256:e954a7ef30815e62832ca4a1d2959142e264795e7ec78ba369752353135beb68
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1.orig.tar.bz2' libassuan_2.5.1.orig.tar.bz2 564857 SHA256:47f96c37b4f2aac289f0bc1bacfa8bd8b4b209a488d3d15e2229cb6cc9b26449
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1-2.debian.tar.xz' libassuan_2.5.1-2.debian.tar.xz 15236 SHA256:4a67901dcb0e92cd40e0d5d7148ebe6f929378671df373eb68b48acb560d641f
```

### `dpkg` source package: `libbsd=0.8.7-1ubuntu0.1`

Binary Packages:

- `libbsd0:amd64=0.8.7-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
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
$ apt-get source -qq --print-uris libbsd=0.8.7-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7-1ubuntu0.1.dsc' libbsd_0.8.7-1ubuntu0.1.dsc 2280 SHA256:864507ff2c7bcfc0078d819db67d698240f9a391fa393e3c5caeb86b0fe5a840
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7.orig.tar.xz' libbsd_0.8.7.orig.tar.xz 371772 SHA256:f548f10e5af5a08b1e22889ce84315b1ebe41505b015c9596bad03fd13a12b31
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7.orig.tar.xz.asc' libbsd_0.8.7.orig.tar.xz.asc 833 SHA256:93ae025cc6430971572ce3c52af30a9ea8d8ae760e8759afe41fa955528617b4
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7-1ubuntu0.1.debian.tar.xz' libbsd_0.8.7-1ubuntu0.1.debian.tar.xz 16608 SHA256:7edb06c4abc9398dbce53521e3671f062bfd9154eb7d401e6037dcf7d9977143
```

### `dpkg` source package: `libcap-ng=0.7.7-3.1`

Binary Packages:

- `libcap-ng0:amd64=0.7.7-3.1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.7-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.1.dsc' libcap-ng_0.7.7-3.1.dsc 2266 SHA256:f545d107ed3e6160b16aac09e242d1ccc054bfca76f6d70731a83c031b416f53
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7.orig.tar.gz' libcap-ng_0.7.7.orig.tar.gz 420178 SHA256:615549ce39b333f6b78baee0c0b4ef18bc726c6bf1cca123dfd89dd963f6d06b
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.1.debian.tar.xz' libcap-ng_0.7.7-3.1.debian.tar.xz 5432 SHA256:074bf729c3081af729e7e0fbbe3354ddecc16e045245e7d4f44003b9f1f1adc6
```

### `dpkg` source package: `libcap2=1:2.25-1.2`

Binary Packages:

- `libcap2:amd64=1:2.25-1.2`
- `libcap2-bin=1:2.25-1.2`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.25-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.25-1.2.dsc' libcap2_2.25-1.2.dsc 2230 SHA256:a492c5c61703dcd80e19ff408d8562671fbfe0a03dd93c3570ddf214ac06752b
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.25.orig.tar.xz' libcap2_2.25.orig.tar.xz 63672 SHA256:693c8ac51e983ee678205571ef272439d83afe62dd8e424ea14ad9790bc35162
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.25-1.2.debian.tar.xz' libcap2_2.25-1.2.debian.tar.xz 20912 SHA256:0088bcf76d6cdf1c242431b3b97e91e50120cc2fc2b938dbeb3606dece7d9870
```

### `dpkg` source package: `libcdr=0.1.4-1build1`

Binary Packages:

- `libcdr-0.1-1:amd64=0.1.4-1build1`

Licenses: (parsed from: `/usr/share/doc/libcdr-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libcdr=0.1.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdr/libcdr_0.1.4-1build1.dsc' libcdr_0.1.4-1build1.dsc 2124 SHA256:6f4af8d63346717ddf78a21d913b4fd414ab622fc06bd0b618e3a9f16c0ef997
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdr/libcdr_0.1.4.orig.tar.xz' libcdr_0.1.4.orig.tar.xz 609592 SHA256:e7a7e8b00a3df5798110024d7061fe9d1c3330277d2e4fa9213294f966a4a66d
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdr/libcdr_0.1.4-1build1.debian.tar.xz' libcdr_0.1.4-1build1.debian.tar.xz 7976 SHA256:3ecb148a6c130e25a58d3755025722e00d52aae145782e2823399ef894a69ddd
```

### `dpkg` source package: `libcmis=0.5.1+git20160603-3build2`

Binary Packages:

- `libcmis-0.5-5v5=0.5.1+git20160603-3build2`

Licenses: (parsed from: `/usr/share/doc/libcmis-0.5-5v5/copyright`)

- `GPL`
- `LGPL`
- `MPL | GPL2+ | LGPL2+`

Source:

```console
$ apt-get source -qq --print-uris libcmis=0.5.1+git20160603-3build2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcmis/libcmis_0.5.1+git20160603-3build2.dsc' libcmis_0.5.1+git20160603-3build2.dsc 2314 SHA256:d17945fb64064853399272d23378a17838db6b0cbe3c4a2865bb44c80d2dc085
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcmis/libcmis_0.5.1+git20160603.orig.tar.bz2' libcmis_0.5.1+git20160603.orig.tar.bz2 208196 SHA256:a916526d4379ce720599164e38c904f9571924e7aedcf0654d73387b64d2ce2a
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcmis/libcmis_0.5.1+git20160603-3build2.debian.tar.xz' libcmis_0.5.1+git20160603-3build2.debian.tar.xz 4512 SHA256:aebfc158814ab70ac01672e7707283d3a349070805500642fcf660458a8dc6e6
```

### `dpkg` source package: `libcroco=0.6.12-2`

Binary Packages:

- `libcroco3:amd64=0.6.12-2`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.12-2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.12-2.dsc' libcroco_0.6.12-2.dsc 2204 SHA256:46e81715670968edd1d71cd878a5426ea2b28513bc4975f0b1975185adb69c9e
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.12.orig.tar.xz' libcroco_0.6.12.orig.tar.xz 482028 SHA256:ddc4b5546c9fb4280a5017e2707fbd4839034ed1aba5b7d4372212f34f84f860
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.12-2.debian.tar.xz' libcroco_0.6.12-2.debian.tar.xz 8076 SHA256:038c42873794d314fb40c9d0a78c49b841b9ac8f3a947f3fee5f7928e7d155b0
```

### `dpkg` source package: `libdatrie=0.2.10-7`

Binary Packages:

- `libdatrie1:amd64=0.2.10-7`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.10-7
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-7.dsc' libdatrie_0.2.10-7.dsc 2256 SHA256:63ad3d2782cfcca0d34055a152908ad65c6b2fc84d3079b79cf90ac4924a77fb
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10.orig.tar.xz' libdatrie_0.2.10.orig.tar.xz 294380 SHA256:180eff7b0309ca19a02d5864e744185d715f021398a096fec6cf960f8ebfaa2b
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-7.debian.tar.xz' libdatrie_0.2.10-7.debian.tar.xz 8576 SHA256:0c1496995d89daacad655618e6fff5402cb6935bb5b386c54bf4dcd1cf1b8f85
```

### `dpkg` source package: `libe-book=0.1.3-1`

Binary Packages:

- `libe-book-0.1-1:amd64=0.1.3-1`

Licenses: (parsed from: `/usr/share/doc/libe-book-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libe-book=0.1.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libe-book/libe-book_0.1.3-1.dsc' libe-book_0.1.3-1.dsc 2041 SHA256:d433911367b45f4c5ca5d22cb60c89fb560eecb04bc1bf40b1110c19147b113c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libe-book/libe-book_0.1.3.orig.tar.xz' libe-book_0.1.3.orig.tar.xz 416268 SHA256:7e8d8ff34f27831aca3bc6f9cc532c2f90d2057c778963b884ff3d1e34dfe1f9
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libe-book/libe-book_0.1.3-1.debian.tar.xz' libe-book_0.1.3-1.debian.tar.xz 7184 SHA256:3ddb1cda6b6b116e957620e6b0942f1eb757cde16367218266b73db9ec1de1eb
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libeot/libeot_0.01-5.dsc' libeot_0.01-5.dsc 1949 SHA256:71933404d061aeffe2c0e5da353ef7c5146fd061131b0a8c31257b16b080cab6
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libeot/libeot_0.01.orig.tar.bz2' libeot_0.01.orig.tar.bz2 260288 SHA256:cf5091fa8e7dcdbe667335eb90a2cfdd0a3fe8f8c7c8d1ece44d9d055736a06a
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libeot/libeot_0.01-5.debian.tar.xz' libeot_0.01-5.debian.tar.xz 7492 SHA256:e6f5685fee36d82d31e1d2b2334314098b8bac7b87de59ee89809795f85b87c5
```

### `dpkg` source package: `libepoxy=1.4.3-1`

Binary Packages:

- `libepoxy0:amd64=1.4.3-1`

Licenses: (parsed from: `/usr/share/doc/libepoxy0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libepoxy=1.4.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libepoxy/libepoxy_1.4.3-1.dsc' libepoxy_1.4.3-1.dsc 2107 SHA256:896b02444d12e4be1a1aa9582e5227041d595d355cf7ee431833eff0f4207fd2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libepoxy/libepoxy_1.4.3.orig.tar.xz' libepoxy_1.4.3.orig.tar.xz 821560 SHA256:85f3608223106be2bdf8e45eb25c0593904f6f00f40abe9100993f249923a39b
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libepoxy/libepoxy_1.4.3-1.debian.tar.xz' libepoxy_1.4.3-1.debian.tar.xz 15900 SHA256:a3f21f10bb7c812630c8f88123e692ddc4bebf0aff5f9250d80afc24a8cc28b5
```

### `dpkg` source package: `libepubgen=0.1.0-2ubuntu1`

Binary Packages:

- `libepubgen-0.1-1:amd64=0.1.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libepubgen-0.1-1/copyright`)

- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libepubgen=0.1.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libepubgen/libepubgen_0.1.0-2ubuntu1.dsc' libepubgen_0.1.0-2ubuntu1.dsc 1774 SHA256:0193e4802aa9cc5d7db51aa5dfee6032806a643b2c031f42c1eb880221fecf9c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libepubgen/libepubgen_0.1.0.orig.tar.bz2' libepubgen_0.1.0.orig.tar.bz2 398811 SHA256:730bd1cbeee166334faadbc06c953a67b145c3c4754a3b503482066dae4cd633
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libepubgen/libepubgen_0.1.0-2ubuntu1.debian.tar.xz' libepubgen_0.1.0-2ubuntu1.debian.tar.xz 5596 SHA256:fd4d0b2856977f7f9dc823d4af3baa95378ae43a3275b5c83e325d55f86d55e8
```

### `dpkg` source package: `libetonyek=0.1.7-3`

Binary Packages:

- `libetonyek-0.1-1:amd64=0.1.7-3`

Licenses: (parsed from: `/usr/share/doc/libetonyek-0.1-1/copyright`)

- `MPL 2.0`

Source:

```console
$ apt-get source -qq --print-uris libetonyek=0.1.7-3
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libetonyek/libetonyek_0.1.7-3.dsc' libetonyek_0.1.7-3.dsc 2081 SHA256:3a382d8ac1dfb45292ba67dabe6ca469fd32cea8cff687570802d55249b021f3
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libetonyek/libetonyek_0.1.7.orig.tar.xz' libetonyek_0.1.7.orig.tar.xz 1256232 SHA256:69dbe10d4426d52f09060d489f8eb90dfa1df592e82eb0698d9dbaf38cc734ac
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libetonyek/libetonyek_0.1.7-3.debian.tar.xz' libetonyek_0.1.7-3.debian.tar.xz 9140 SHA256:b07ae6e21613ee218a03e261ca08a73689238c46c3a64f68e72fc0bd080fed80
```

### `dpkg` source package: `libexttextcat=3.4.5-1`

Binary Packages:

- `libexttextcat-2.0-0:amd64=3.4.5-1`
- `libexttextcat-data=3.4.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libexttextcat=3.4.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexttextcat/libexttextcat_3.4.5-1.dsc' libexttextcat_3.4.5-1.dsc 2099 SHA256:9a5f988e773efec298260e0464df6b4d77b01d82d2a989d317c5529f9c3ac586
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexttextcat/libexttextcat_3.4.5.orig.tar.xz' libexttextcat_3.4.5.orig.tar.xz 1041268 SHA256:13fdbc9d4c489a4d0519e51933a1aa21fe3fb9eb7da191b87f7a63e82797dac8
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexttextcat/libexttextcat_3.4.5-1.debian.tar.xz' libexttextcat_3.4.5-1.debian.tar.xz 7224 SHA256:bf214f4c725d236a8e77b4f7199316255de431eb48638b78f5346890fb3c0849
```

### `dpkg` source package: `libffi=3.2.1-8`

Binary Packages:

- `libffi6:amd64=3.2.1-8`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-8
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-8.dsc' libffi_3.2.1-8.dsc 1959 SHA256:a07201eb5374cfab35703a6f4c88a494bb23ece91da5481497bc25404c57eaf4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-8.debian.tar.xz' libffi_3.2.1-8.debian.tar.xz 11660 SHA256:1eb0b13e0c0fc989ed98011d18dcddf8a05af17380fe1258883761a8d16586b4
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfreehand/libfreehand_0.1.2-2.dsc' libfreehand_0.1.2-2.dsc 2039 SHA256:ceba859e4062f5fa88f497d3c7a3927a9e6206c33ca82cfed80aeb2e1dfee5ea
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfreehand/libfreehand_0.1.2.orig.tar.xz' libfreehand_0.1.2.orig.tar.xz 516132 SHA256:0e422d1564a6dbf22a9af598535425271e583514c0f7ba7d9091676420de34ac
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfreehand/libfreehand_0.1.2-2.debian.tar.xz' libfreehand_0.1.2-2.debian.tar.xz 13112 SHA256:aa9a003c2acf5f36bee24469ce48ed52f828c66795309cf9d5c514fe5cedfcd1
```

### `dpkg` source package: `libgcrypt20=1.8.1-4ubuntu1.2`

Binary Packages:

- `libgcrypt20:amd64=1.8.1-4ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.1-4ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.dsc' libgcrypt20_1.8.1-4ubuntu1.2.dsc 3035 SHA256:2033925196ff659631496ea66d2feea91112512ab36fcefbcac84fb98b8523dc
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2' libgcrypt20_1.8.1.orig.tar.bz2 2967344 SHA256:7a2875f8b1ae0301732e878c0cca2c9664ff09ef71408f085c50e332656a78b3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2.asc' libgcrypt20_1.8.1.orig.tar.bz2.asc 310 SHA256:9e08f467824855084594a14c4a0455963dac9a359d543e8c2a91ca3498ad031b
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz' libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz 33112 SHA256:e1b2d8ea9bb06c9370bf76934be994458f596162bfaac27061c9047a2ac45c25
```

### `dpkg` source package: `libgpg-error=1.27-6`

Binary Packages:

- `libgpg-error0:amd64=1.27-6`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.27-6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27-6.dsc' libgpg-error_1.27-6.dsc 2343 SHA256:d4cc2c1691b295f558d5b347df8a8ad2f0260cf57146180bed223b94ffacafbb
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27.orig.tar.bz2' libgpg-error_1.27.orig.tar.bz2 813060 SHA256:4f93aac6fecb7da2b92871bb9ee33032be6a87b174f54abf8ddf0911a22d29d2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27-6.debian.tar.xz' libgpg-error_1.27-6.debian.tar.xz 20556 SHA256:89bc57dc3df449febf037226daf1aee830455c4efa493c0e3bdeab2a48971479
```

### `dpkg` source package: `libice=2:1.0.9-2`

Binary Packages:

- `libice6:amd64=2:1.0.9-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-2.dsc' libice_1.0.9-2.dsc 2130 SHA256:116595cd54be23edad0b55e1cd4bc1929f277fa5c2d00d8f187b0bc5dd39ad6c
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-2.diff.gz' libice_1.0.9-2.diff.gz 6384 SHA256:777f13e08aada3103c32a0b93a26782ca959027bcd98c2c1ddaade8f944fa40a
```

### `dpkg` source package: `libidn2=2.0.4-1.1ubuntu0.2`

Binary Packages:

- `libidn2-0:amd64=2.0.4-1.1ubuntu0.2`

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
$ apt-get source -qq --print-uris libidn2=2.0.4-1.1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.dsc' libidn2_2.0.4-1.1ubuntu0.2.dsc 2391 SHA256:013191e4a413de9928b5f76b2ab7237055d2e51ed1f82c7bd5ddddff6615d7c8
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4.orig.tar.gz' libidn2_2.0.4.orig.tar.gz 2008524 SHA256:644b6b03b285fb0ace02d241d59483d98bc462729d8bb3608d5cad5532f3d2f0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz' libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz 10290460 SHA256:45c587e0bf489b0367a7a1c2eadbd2efcc774c035ef4868c95ea5b0e0f399be2
```

### `dpkg` source package: `libjpeg-turbo=1.5.2-0ubuntu5.18.04.4`

Binary Packages:

- `libjpeg-turbo8:amd64=1.5.2-0ubuntu5.18.04.4`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1.5.2-0ubuntu5.18.04.4
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.dsc' libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.dsc 2391 SHA256:9181849c8b3b48fb97562a3dec0e8bf0a920992927a9fd7e6f50097ef9299bb0
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2.orig.tar.gz' libjpeg-turbo_1.5.2.orig.tar.gz 1657235 SHA256:9098943b270388727ae61de82adec73cf9f0dbb240b3bc8b172595ebf405b528
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.debian.tar.xz' libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.debian.tar.xz 35396 SHA256:8d0685c3a0e185ee75eb9811a16c9894302d8149f5a7da226d6c87ca8b5b224e
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu8`

Binary Packages:

- `libjpeg8:amd64=8c-2ubuntu8`

Licenses: (parsed from: `/usr/share/doc/libjpeg8/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg8-empty=8c-2ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.dsc' libjpeg8-empty_8c-2ubuntu8.dsc 1637 SHA256:e7f575dcb3e0d462513b6f928179baa0ff1d145273934b1041b714515096b407
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.tar.gz' libjpeg8-empty_8c-2ubuntu8.tar.gz 1770 SHA256:48a4227e9fc70851a4f304b10624e02875bf6f4e2debfcbe4ba0dd85a3ec05c6
```

### `dpkg` source package: `libksba=1.3.5-2`

Binary Packages:

- `libksba8:amd64=1.3.5-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.3.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5-2.dsc' libksba_1.3.5-2.dsc 2526 SHA256:4fd08fd129f97ab1df86c220b88b7b2c6e4e04aa90bfd3ae364d18022256bef8
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2' libksba_1.3.5.orig.tar.bz2 620649 SHA256:41444fd7a6ff73a79ad9728f985e71c9ba8cd3e5e53358e70d5f066d35c1a340
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2.asc' libksba_1.3.5.orig.tar.bz2.asc 287 SHA256:a954b03144ee882c838853da24fd7b6868b78df72a18c71079217d968698a76f
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5-2.debian.tar.xz' libksba_1.3.5-2.debian.tar.xz 13852 SHA256:98c985bff973be1aecc702fa15887ff1e5b8de481d1dc3e99423a587754eaabd
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblangtag/liblangtag_0.6.2-1.dsc' liblangtag_0.6.2-1.dsc 2370 SHA256:a0909825917c4ead4be851f4885ddfe501af65cadda1add6b45facd2af4ff6c4
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblangtag/liblangtag_0.6.2.orig.tar.bz2' liblangtag_0.6.2.orig.tar.bz2 766080 SHA256:d6242790324f1432fb0a6fae71b6851f520b2c5a87675497cf8ea14c2924d52e
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblangtag/liblangtag_0.6.2-1.debian.tar.xz' liblangtag_0.6.2-1.debian.tar.xz 6072 SHA256:003688ddf23bdbfcc27816ea7e9714f58930ca26d36d1685f06d28760fbff81a
```

### `dpkg` source package: `libmspub=0.1.4-1`

Binary Packages:

- `libmspub-0.1-1:amd64=0.1.4-1`

Licenses: (parsed from: `/usr/share/doc/libmspub-0.1-1/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libmspub=0.1.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmspub/libmspub_0.1.4-1.dsc' libmspub_0.1.4-1.dsc 2105 SHA256:6fce7406b885d7e37c6a542fa5170a27418853b25db66149d0512b8490a267e1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmspub/libmspub_0.1.4.orig.tar.xz' libmspub_0.1.4.orig.tar.xz 377472 SHA256:ef36c1a1aabb2ba3b0bedaaafe717bf4480be2ba8de6f3894be5fd3702b013ba
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmspub/libmspub_0.1.4-1.debian.tar.xz' libmspub_0.1.4-1.debian.tar.xz 7160 SHA256:04bb3417404f0048ecbb5ad26e360c64d4df1854baf978dae6159f10c0a45d8f
```

### `dpkg` source package: `libmwaw=0.3.13-1`

Binary Packages:

- `libmwaw-0.3-3:amd64=0.3.13-1`

Licenses: (parsed from: `/usr/share/doc/libmwaw-0.3-3/copyright`)

- `BSD`
- `LGPL`
- `MPL2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmwaw=0.3.13-1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmwaw/libmwaw_0.3.13-1.dsc' libmwaw_0.3.13-1.dsc 2072 SHA256:633980c80135f2e9bd332fa9b6dcaddd90e083449778e05d503e4611afe5a484
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmwaw/libmwaw_0.3.13.orig.tar.xz' libmwaw_0.3.13.orig.tar.xz 1258220 SHA256:db55c728448f9c795cd71a0bb6043f6d4744e3e001b955a018a2c634981d5aea
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmwaw/libmwaw_0.3.13-1.debian.tar.xz' libmwaw_0.3.13-1.debian.tar.xz 8152 SHA256:33ef2458a7b53178e68439f184f7cfead60ff216395ac7f5043566ce98d1bb04
```

### `dpkg` source package: `libodfgen=0.1.6-2`

Binary Packages:

- `libodfgen-0.1-1:amd64=0.1.6-2`

Licenses: (parsed from: `/usr/share/doc/libodfgen-0.1-1/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libodfgen=0.1.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libodfgen/libodfgen_0.1.6-2.dsc' libodfgen_0.1.6-2.dsc 1925 SHA256:e63c30d5461b53a11fdc83e3dd585735273e94b80812e5e2627d6e96eaf5e838
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libodfgen/libodfgen_0.1.6.orig.tar.bz2' libodfgen_0.1.6.orig.tar.bz2 446705 SHA256:2c7b21892f84a4c67546f84611eccdad6259875c971e98ddb027da66ea0ac9c2
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libodfgen/libodfgen_0.1.6-2.debian.tar.xz' libodfgen_0.1.6-2.debian.tar.xz 6868 SHA256:97ee71689bd24694abfee2c7b736ebeb45aa2cd215a338edd8183342a9ecea8f
```

### `dpkg` source package: `liborcus=0.13.4-2`

Binary Packages:

- `liborcus-0.13-0:amd64=0.13.4-2`

Licenses: (parsed from: `/usr/share/doc/liborcus-0.13-0/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3+`
- `MIT`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris liborcus=0.13.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libo/liborcus/liborcus_0.13.4-2.dsc' liborcus_0.13.4-2.dsc 2624 SHA256:f2a08d175764c8e7fb68ac269107674b62dcb254899e3e7d5d39a46b4bbcd4f8
'http://archive.ubuntu.com/ubuntu/pool/main/libo/liborcus/liborcus_0.13.4.orig.tar.xz' liborcus_0.13.4.orig.tar.xz 1569904 SHA256:1b3f09c03286f6db015537d030195ec06162aa5ae56da21303ef1436be60ed31
'http://archive.ubuntu.com/ubuntu/pool/main/libo/liborcus/liborcus_0.13.4-2.debian.tar.xz' liborcus_0.13.4-2.debian.tar.xz 11232 SHA256:0f9624dbc5fbe864edd274d35fade3883a6d18fdec2fd9ae4e95065a03c473c4
```

### `dpkg` source package: `libpagemaker=0.0.4-1`

Binary Packages:

- `libpagemaker-0.0-0:amd64=0.0.4-1`

Licenses: (parsed from: `/usr/share/doc/libpagemaker-0.0-0/copyright`)

- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libpagemaker=0.0.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpagemaker/libpagemaker_0.0.4-1.dsc' libpagemaker_0.0.4-1.dsc 2008 SHA256:fc7040296e01d0175dbf4ed2fc4ff75aec1ec8bd07db9b4323680b8501075e63
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpagemaker/libpagemaker_0.0.4.orig.tar.xz' libpagemaker_0.0.4.orig.tar.xz 306496 SHA256:66adacd705a7d19895e08eac46d1e851332adf2e736c566bef1164e7a442519d
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpagemaker/libpagemaker_0.0.4-1.debian.tar.xz' libpagemaker_0.0.4-1.debian.tar.xz 6628 SHA256:02f9cfbf5c9bba7ff914afcb8829c45047eff5a56107598216e761861b82999a
```

### `dpkg` source package: `libpng1.6=1.6.34-1ubuntu0.18.04.2`

Binary Packages:

- `libpng16-16:amd64=1.6.34-1ubuntu0.18.04.2`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.34-1ubuntu0.18.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc' libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc 2362 SHA256:d121cf079c097f868b33f234601baadc6e34d5e96320f427eb3482e28900c321
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34.orig.tar.xz' libpng1.6_1.6.34.orig.tar.xz 997968 SHA256:2f1e960d92ce3b3abd03d06dfec9637dfbd22febf107a536b44f7a47c60659f6
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz' libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz 24572 SHA256:08abc3815a3ce53c46717a3a5c1b2044782c5659639afc9f6f9cb6fdcb386d90
```

### `dpkg` source package: `libproxy=0.4.15-1`

Binary Packages:

- `libproxy1v5:amd64=0.4.15-1`

Licenses: (parsed from: `/usr/share/doc/libproxy1v5/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libproxy=0.4.15-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libproxy/libproxy_0.4.15-1.dsc' libproxy_0.4.15-1.dsc 3280 SHA256:91779897b80fac88f6b7058cad3335078189dac35e90ea1894318b53cfc7f3fa
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libproxy/libproxy_0.4.15.orig.tar.gz' libproxy_0.4.15.orig.tar.gz 93084 SHA256:18f58b0a0043b6881774187427ead158d310127fc46a1c668ad6d207fb28b4e0
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libproxy/libproxy_0.4.15-1.debian.tar.xz' libproxy_0.4.15-1.debian.tar.xz 9908 SHA256:85325735c9b4e6b5bf2f920573ae11ffd56aae1b3cb7e28f173a57186fa3454f
```

### `dpkg` source package: `libpsl=0.19.1-5build1`

Binary Packages:

- `libpsl5:amd64=0.19.1-5build1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.19.1-5build1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1-5build1.dsc' libpsl_0.19.1-5build1.dsc 2229 SHA256:cb9bcc439b8e37ee27bd3e69a8afa6dd2a59c90ba45de4d533df256f61c8a4f5
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1.orig.tar.gz' libpsl_0.19.1.orig.tar.gz 8578385 SHA256:e370181114b8ef9daf2bb6db49b1edb842335839c15a088e7ec0a35e04e9a227
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1-5build1.debian.tar.xz' libpsl_0.19.1-5build1.debian.tar.xz 9860 SHA256:53285bee66ac22a25dd41f7778cc4e94ae3d61929eb6701a8064a38a964e40e2
```

### `dpkg` source package: `libreoffice=1:6.0.7-0ubuntu0.18.04.10`

Binary Packages:

- `fonts-opensymbol=2:102.10+LibO6.0.7-0ubuntu0.18.04.10`
- `libreoffice=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-avmedia-backend-gstreamer=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-base=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-base-core=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-base-drivers=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-calc=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-common=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-core=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-draw=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-impress=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-math=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-report-builder-bin=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-style-galaxy=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-style-tango=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-writer=1:6.0.7-0ubuntu0.18.04.10`
- `python3-uno=1:6.0.7-0ubuntu0.18.04.10`
- `uno-libs3=6.0.7-0ubuntu0.18.04.10`
- `ure=6.0.7-0ubuntu0.18.04.10`

Licenses: (parsed from: `/usr/share/doc/fonts-opensymbol/copyright`, `/usr/share/doc/libreoffice/copyright`, `/usr/share/doc/libreoffice-avmedia-backend-gstreamer/copyright`, `/usr/share/doc/libreoffice-base/copyright`, `/usr/share/doc/libreoffice-base-core/copyright`, `/usr/share/doc/libreoffice-base-drivers/copyright`, `/usr/share/doc/libreoffice-calc/copyright`, `/usr/share/doc/libreoffice-common/copyright`, `/usr/share/doc/libreoffice-core/copyright`, `/usr/share/doc/libreoffice-draw/copyright`, `/usr/share/doc/libreoffice-impress/copyright`, `/usr/share/doc/libreoffice-math/copyright`, `/usr/share/doc/libreoffice-report-builder-bin/copyright`, `/usr/share/doc/libreoffice-style-galaxy/copyright`, `/usr/share/doc/libreoffice-style-tango/copyright`, `/usr/share/doc/libreoffice-writer/copyright`, `/usr/share/doc/python3-uno/copyright`, `/usr/share/doc/uno-libs3/copyright`, `/usr/share/doc/ure/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-3`
- `MIT`
- `MPL-1.1`
- `MPL-2.0`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libreoffice=1:6.0.7-0ubuntu0.18.04.10
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7-0ubuntu0.18.04.10.dsc' libreoffice_6.0.7-0ubuntu0.18.04.10.dsc 18078 SHA256:d74b61f11018aed63dd965480c93ce6aba94a741b19b3866a65a510fb3aa2fb4
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig-helpcontent2.tar.xz' libreoffice_6.0.7.orig-helpcontent2.tar.xz 2423012 SHA256:41c1ef4b0437acd7e8ba36789b45906e99e0487b12198bce0d30ed74c9e0ccaf
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig-tarballs.tar.xz' libreoffice_6.0.7.orig-tarballs.tar.xz 215486780 SHA256:96116dcc195ab1f47fa677bf88f8d233561422dbfe5a0539f7408b56e254c194
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig-translations.tar.xz' libreoffice_6.0.7.orig-translations.tar.xz 139598364 SHA256:24a3ef909cfb0722dec3d6e40924681b41641f175e5df90b3e5507fdceb43186
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig.tar.xz' libreoffice_6.0.7.orig.tar.xz 183202236 SHA256:fc67036b0c00c1685d39acec6c485a4a250b6bb92fc08a88377d39d2f7fd7923
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7-0ubuntu0.18.04.10.debian.tar.xz' libreoffice_6.0.7-0ubuntu0.18.04.10.debian.tar.xz 2178480 SHA256:c3a47dcedfedb834044bcffcb333016c07c497a86ea5884fca8361d215ffd441
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librest/librest_0.8.0-2.dsc' librest_0.8.0-2.dsc 2455 SHA256:5b07238bde6883684aad271a518b0924dd05d36c7581d56a0e57c1ed8b56b6f6
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librest/librest_0.8.0.orig.tar.xz' librest_0.8.0.orig.tar.xz 334024 SHA256:e7b89b200c1417073aef739e8a27ff2ab578056c27796ec74f5886a5e0dff647
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librest/librest_0.8.0-2.debian.tar.xz' librest_0.8.0-2.debian.tar.xz 6536 SHA256:233b15b5c4b36fa6b2ac026305fd5db043e4de22a14f947d304956adba640827
```

### `dpkg` source package: `librevenge=0.0.4-6ubuntu2`

Binary Packages:

- `librevenge-0.0-0:amd64=0.0.4-6ubuntu2`

Licenses: (parsed from: `/usr/share/doc/librevenge-0.0-0/copyright`)

- `LGPL-2.1`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris librevenge=0.0.4-6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librevenge/librevenge_0.0.4-6ubuntu2.dsc' librevenge_0.0.4-6ubuntu2.dsc 2035 SHA256:44c8af7983df4241d857785b4e40b3aa579abae32d94f8ebcea134adc9efd177
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librevenge/librevenge_0.0.4.orig.tar.bz2' librevenge_0.0.4.orig.tar.bz2 529833 SHA256:c51601cd08320b75702812c64aae0653409164da7825fd0f451ac2c5dbe77cbf
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librevenge/librevenge_0.0.4-6ubuntu2.debian.tar.xz' librevenge_0.0.4-6ubuntu2.debian.tar.xz 13712 SHA256:0366405c50e6abc83c2221bbdfc1108584aeeee9e8e0c7a8aea3213683f0d5be
```

### `dpkg` source package: `librsvg=2.40.20-2ubuntu0.2`

Binary Packages:

- `librsvg2-2:amd64=2.40.20-2ubuntu0.2`
- `librsvg2-common:amd64=2.40.20-2ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.40.20-2ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20-2ubuntu0.2.dsc' librsvg_2.40.20-2ubuntu0.2.dsc 2846 SHA256:6790f598b07cb0433bb4243e9afd17cc768168f93e3eab03173fad90747b81ce
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20.orig.tar.xz' librsvg_2.40.20.orig.tar.xz 1796376 SHA256:cff4dd3c3b78bfe99d8fcfad3b8ba1eee3289a0823c0e118d78106be6b84c92b
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20-2ubuntu0.2.debian.tar.xz' librsvg_2.40.20-2ubuntu0.2.debian.tar.xz 16768 SHA256:8eca9882068282bbfa972d33a1e4d96b5e188fda216a0f1a489c231a92d4b178
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3.18.04.3`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3.18.04.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu3.18.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.dsc' libseccomp_2.4.3-1ubuntu3.18.04.3.dsc 1951 SHA256:a21ac1a2c77ed23af125630a6fe63035e35cd8312d5023efdb5c9434c2d3d30e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA256:cf15d1421997fac45b936515af61d209c4fd788af11005d212b3d0fd71e7991d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz 27652 SHA256:9110a31f32f7c63318f75c09493c021e454fa46d7bb0ccca4b0874610c85a71c
```

### `dpkg` source package: `libselinux=2.7-2build2`

Binary Packages:

- `libselinux1:amd64=2.7-2build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.7-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7-2build2.dsc' libselinux_2.7-2build2.dsc 2468 SHA256:86f2d8422230927aa3274773e2b8a9ed15cb539804c378e75515afcd28545c37
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7.orig.tar.gz' libselinux_2.7.orig.tar.gz 187574 SHA256:d0fec0769b3ad60aa7baf9b9a4b7a056827769dc2dadda0dc0eb59b3d1c18c57
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7-2build2.debian.tar.xz' libselinux_2.7-2build2.debian.tar.xz 23176 SHA256:ef7a781c247797b66f4d68907d8dd6fec7188d0a08e2a8541437d5f7f6796105
```

### `dpkg` source package: `libsemanage=2.7-2build2`

Binary Packages:

- `libsemanage-common=2.7-2build2`
- `libsemanage1:amd64=2.7-2build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.7-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7-2build2.dsc' libsemanage_2.7-2build2.dsc 2555 SHA256:4454d11e7228df1e5166907867bbd1be4e6cc8b20c6834dc690fb0dcf19d1c43
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7.orig.tar.gz' libsemanage_2.7.orig.tar.gz 153465 SHA256:07e9477714ce6a4557a1fe924ea4cb06501b62d0fa0e3c0dc32a2cf47cb8d476
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7-2build2.debian.tar.xz' libsemanage_2.7-2build2.debian.tar.xz 17136 SHA256:d6d11ecc5687baa3b07a2a2360a9cbc4b93424a9728aa17b81cd9faf13855c3a
```

### `dpkg` source package: `libsepol=2.7-1`

Binary Packages:

- `libsepol1:amd64=2.7-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7-1.dsc' libsepol_2.7-1.dsc 1814 SHA256:7de809477acd60d256eca160d5fc6986e5e65227706b1cdb23f8139bb49d2782
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7.orig.tar.gz' libsepol_2.7.orig.tar.gz 471147 SHA256:d69d3bd8ec901a3bd5adf2be2fb47fb1a685ed73066ab482e7e505371a48f9e7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7-1.debian.tar.xz' libsepol_2.7-1.debian.tar.xz 13944 SHA256:56b1c2b0e492b2089f23a0d7a95a260377a0e3adefc60e90c0ff6eff6be08450
```

### `dpkg` source package: `libsm=2:1.2.2-1`

Binary Packages:

- `libsm6:amd64=2:1.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2-1.dsc' libsm_1.2.2-1.dsc 2107 SHA256:1347efa550751179c0a3f1042a9f8ae43ee0c22cf0c2283921fa83e52a68433f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2.orig.tar.gz' libsm_1.2.2.orig.tar.gz 415990 SHA256:14bb7c669ce2b8ff712fbdbf48120e3742a77edcd5e025d6b3325ed30cf120f4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2-1.diff.gz' libsm_1.2.2-1.diff.gz 6183 SHA256:9848714292ead15fcc48ab2d337f2cc5fc08910abbdfaf69d3ef1b89d3fdb2d5
```

### `dpkg` source package: `libsoup2.4=2.62.1-1ubuntu0.4`

Binary Packages:

- `libsoup-gnome2.4-1:amd64=2.62.1-1ubuntu0.4`
- `libsoup2.4-1:amd64=2.62.1-1ubuntu0.4`

Licenses: (parsed from: `/usr/share/doc/libsoup-gnome2.4-1/copyright`, `/usr/share/doc/libsoup2.4-1/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libsoup2.4=2.62.1-1ubuntu0.4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsoup2.4/libsoup2.4_2.62.1-1ubuntu0.4.dsc' libsoup2.4_2.62.1-1ubuntu0.4.dsc 2825 SHA256:7988e3bd4be850de335adac80ed04e5ef33e83f19fcd199b3ae5daf53fcb5766
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsoup2.4/libsoup2.4_2.62.1.orig.tar.xz' libsoup2.4_2.62.1.orig.tar.xz 1848776 SHA256:f037ddac2e0f9b1c842a0060fa6119bea1d3b349a2c901283c961247e45883d7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsoup2.4/libsoup2.4_2.62.1-1ubuntu0.4.debian.tar.xz' libsoup2.4_2.62.1-1ubuntu0.4.debian.tar.xz 22764 SHA256:43250ded120ca401d7d9d8a8f31f2a0a482ff2ed59875e51990c5c9596a598de
```

### `dpkg` source package: `libtasn1-6=4.13-2`

Binary Packages:

- `libtasn1-6:amd64=4.13-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.13-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13-2.dsc' libtasn1-6_4.13-2.dsc 2574 SHA256:8f583c0ae8568ccf7fcf66c387963ef949d644cfca56d66512a17cb91c3a44fd
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz' libtasn1-6_4.13.orig.tar.gz 1891703 SHA256:7e528e8c317ddd156230c4e31d082cd13e7ddeb7a54824be82632209550c8cca
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz.asc' libtasn1-6_4.13.orig.tar.gz.asc 774 SHA256:90261376528edf44831d1369847088cc2fb48669860d343961daca42e674b226
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13-2.debian.tar.xz' libtasn1-6_4.13-2.debian.tar.xz 63332 SHA256:f36a43fb898c031b6b1a5f43b35af1aea95ac164bb2b57c7f07d1c098ed9f7eb
```

### `dpkg` source package: `libthai=0.1.27-2`

Binary Packages:

- `libthai-data=0.1.27-2`
- `libthai0:amd64=0.1.27-2`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.27-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.27-2.dsc' libthai_0.1.27-2.dsc 2342 SHA256:781b3c7f53d0d743f2cedb7588c3a640aa33c437e3ebd872e018c9113d010323
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.27.orig.tar.xz' libthai_0.1.27.orig.tar.xz 410360 SHA256:1659fa1b7b1d6562102d7feb8c8c3fd94bb2dc5761ed7dbaae4f300e1c03eff6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.27-2.debian.tar.xz' libthai_0.1.27-2.debian.tar.xz 11660 SHA256:f3c469626104cc97808eab21716bff413b760fb8637976fd27a1b9f0fae64914
```

### `dpkg` source package: `libtool=2.4.6-2`

Binary Packages:

- `libltdl7:amd64=2.4.6-2`

Licenses: (parsed from: `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-2.dsc' libtool_2.4.6-2.dsc 2324 SHA256:caa2b9d5c32e491388d0627e2f808b6cb2f260dd1b0b9fdafc9bff957f05bb29
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-2.debian.tar.xz' libtool_2.4.6-2.debian.tar.xz 36024 SHA256:6227fb1240a90ef06855567e71ee96e4950dd53c4399348f36c1ec39367cd8ea
```

### `dpkg` source package: `libunistring=0.9.9-0ubuntu2`

Binary Packages:

- `libunistring2:amd64=0.9.9-0ubuntu2`

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
$ apt-get source -qq --print-uris libunistring=0.9.9-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.dsc' libunistring_0.9.9-0ubuntu2.dsc 2006 SHA256:b2c297bb30b94a8b4435bb749f0f65564376049fbaf262e9689435217d55a38b
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9.orig.tar.xz' libunistring_0.9.9.orig.tar.xz 2042992 SHA256:a4d993ecfce16cf503ff7579f5da64619cee66226fb3b998dafb706190d9a833
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.debian.tar.xz' libunistring_0.9.9-0ubuntu2.debian.tar.xz 40424 SHA256:cb7a56608d98804e4dc83e1cae6035ef6b89e18f3dcbcd44afb16e32313ed4ba
```

### `dpkg` source package: `libvisio=0.1.6-1build1`

Binary Packages:

- `libvisio-0.1-1:amd64=0.1.6-1build1`

Licenses: (parsed from: `/usr/share/doc/libvisio-0.1-1/copyright`)

- `MIT | GPL-2`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libvisio=0.1.6-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvisio/libvisio_0.1.6-1build1.dsc' libvisio_0.1.6-1build1.dsc 2207 SHA256:a39659222c47a84065403719eb18fd122500e9dec70392192d3bc1fae2ab968b
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvisio/libvisio_0.1.6.orig.tar.bz2' libvisio_0.1.6.orig.tar.bz2 878672 SHA256:c9262ae9797e63a8967e444fb41e4da1861c861eefd121e9e0e4f41eb72b39b9
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvisio/libvisio_0.1.6-1build1.debian.tar.xz' libvisio_0.1.6-1build1.debian.tar.xz 8168 SHA256:3b3033e9ffbed4307b88561a402d1bf4aa5e4df29bbdc8372cec922a36bc5149
```

### `dpkg` source package: `libwpd=0.10.2-2`

Binary Packages:

- `libwpd-0.10-10:amd64=0.10.2-2`

Licenses: (parsed from: `/usr/share/doc/libwpd-0.10-10/copyright`)

- `LGPL`
- `MPL-2.0 | LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libwpd=0.10.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwpd/libwpd_0.10.2-2.dsc' libwpd_0.10.2-2.dsc 2052 SHA256:b6d80190f761320c9ac62a719b965c0858cffece28e4b6b56ff15ed34a06e579
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwpd/libwpd_0.10.2.orig.tar.bz2' libwpd_0.10.2.orig.tar.bz2 674231 SHA256:8859deb6df292c82c7657b7ecbb6f3ef65da252df9d265b755f06bec77add52c
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwpd/libwpd_0.10.2-2.debian.tar.xz' libwpd_0.10.2-2.debian.tar.xz 11456 SHA256:1f553f21f1d0aad96ff8212b88d346cd770a4ec9267f382717b289d7ecae66ce
```

### `dpkg` source package: `libwpg=0.3.1-3`

Binary Packages:

- `libwpg-0.3-3:amd64=0.3.1-3`

Licenses: (parsed from: `/usr/share/doc/libwpg-0.3-3/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libwpg=0.3.1-3
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwpg/libwpg_0.3.1-3.dsc' libwpg_0.3.1-3.dsc 2010 SHA256:53ee76f68b2e8de3102c1704ff3508f115c41c316009059dced8764a86046957
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwpg/libwpg_0.3.1.orig.tar.bz2' libwpg_0.3.1.orig.tar.bz2 397128 SHA256:29049b95895914e680390717a243b291448e76e0f82fb4d2479adee5330fbb59
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwpg/libwpg_0.3.1-3.debian.tar.xz' libwpg_0.3.1-3.debian.tar.xz 9220 SHA256:fcb1e4890ace78e7c3505bcee564e176a202b82b76990462245b7ffa8eb6ed96
```

### `dpkg` source package: `libwps=0.4.8-1`

Binary Packages:

- `libwps-0.4-4:amd64=0.4.8-1`

Licenses: (parsed from: `/usr/share/doc/libwps-0.4-4/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwps=0.4.8-1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwps/libwps_0.4.8-1.dsc' libwps_0.4.8-1.dsc 2203 SHA256:2876f02967c381452ec3dcd0c2f3ddc8ed2666f88bd5f237effe486807333036
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwps/libwps_0.4.8.orig.tar.xz' libwps_0.4.8.orig.tar.xz 648512 SHA256:e478e825ef33f6a434a19ff902c5469c9da7acc866ea0d8ab610a8b2aa94177e
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwps/libwps_0.4.8-1.debian.tar.xz' libwps_0.4.8-1.debian.tar.xz 8948 SHA256:7c34eb504ba933dbea0c41949360d9e613c6a3dab69527cec7fea802de4a8d88
```

### `dpkg` source package: `libx11=2:1.6.4-3ubuntu0.2`

Binary Packages:

- `libx11-6:amd64=2:1.6.4-3ubuntu0.2`
- `libx11-data=2:1.6.4-3ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libxau=1:1.0.8-1ubuntu1`

Binary Packages:

- `libxau6:amd64=1:1.0.8-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1ubuntu1.dsc' libxau_1.0.8-1ubuntu1.dsc 2099 SHA256:23c48bfc9d043cd365a8f305e3b655a271ddd06c40269e7e66453dcc8a2c26be
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA256:c343b4ef66d66a6b3e0e27aa46b37ad5cab0f11a5c565eafb4a1c7590bc71d7b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1ubuntu1.diff.gz' libxau_1.0.8-1ubuntu1.diff.gz 15803 SHA256:c327e2666fb02d5f3dbb18988eb60fcdd335921169a807045e43c881b185b5b9
```

### `dpkg` source package: `libxcb=1.13-2~ubuntu18.04`

Binary Packages:

- `libxcb-render0:amd64=1.13-2~ubuntu18.04`
- `libxcb-shm0:amd64=1.13-2~ubuntu18.04`
- `libxcb1:amd64=1.13-2~ubuntu18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.13-2~ubuntu18.04
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13-2~ubuntu18.04.dsc' libxcb_1.13-2~ubuntu18.04.dsc 4762 SHA256:df45510fc8aaea367e93b5ddb829476982afe39adca00ede5ec07af81bcfe26b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13.orig.tar.gz' libxcb_1.13.orig.tar.gz 632493 SHA256:0bb3cfd46dbd90066bf4d7de3cad73ec1024c7325a4a0cbf5f4a0d4fa91155fb
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13-2~ubuntu18.04.diff.gz' libxcb_1.13-2~ubuntu18.04.diff.gz 25267 SHA256:06fe87d0c4e450a0b976503488c3cd446fd494ef53cfd78d71bb50d74512a5cd
```

### `dpkg` source package: `libxcomposite=1:0.4.4-2`

Binary Packages:

- `libxcomposite1:amd64=1:0.4.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcomposite=1:0.4.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4-2.dsc' libxcomposite_0.4.4-2.dsc 2178 SHA256:4124027ad4b4598a61c45cbc345988010a2a5ba6e7c80259917f59414be69861
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4.orig.tar.gz' libxcomposite_0.4.4.orig.tar.gz 354584 SHA256:83c04649819c6f52cda1b0ce8bcdcc48ad8618428ad803fb07f20b802f1bdad1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4-2.diff.gz' libxcomposite_0.4.4-2.diff.gz 15755 SHA256:9689ae3fcc76054fe09909692e71a1a4fe356e84f3adfa2be668e173d0369ebc
```

### `dpkg` source package: `libxcursor=1:1.1.15-1`

Binary Packages:

- `libxcursor1:amd64=1:1.1.15-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcursor=1:1.1.15-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.15-1.dsc' libxcursor_1.1.15-1.dsc 2288 SHA256:0e204ad2040f088b9a06d28576148970c107f13f3951b95d7536b5bb6fa7e4c4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.15.orig.tar.gz' libxcursor_1.1.15.orig.tar.gz 406960 SHA256:449befea2b11dde58ba3323b2c1ec30550013bd84d80501eb56d0048e62251a1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.15-1.debian.tar.xz' libxcursor_1.1.15-1.debian.tar.xz 8796 SHA256:67728eb5f3ad07f61390793c060b4b6b56806af5b60f0057db04762bc804650f
```

### `dpkg` source package: `libxdamage=1:1.1.4-3`

Binary Packages:

- `libxdamage1:amd64=1:1.1.4-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdamage=1:1.1.4-3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4-3.dsc' libxdamage_1.1.4-3.dsc 2161 SHA256:f1207d4fca942d2cddfe40abc818046e282ceeb0e0b565a44c2908fd03c41368
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4.orig.tar.gz' libxdamage_1.1.4.orig.tar.gz 339060 SHA256:4bb3e9d917f5f593df2277d452926ee6ad96de7b7cd1017cbcf4579fe5d3442b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4-3.debian.tar.xz' libxdamage_1.1.4-3.debian.tar.xz 5904 SHA256:94dcf3997a92f5e1b4681dcbe555af4469607ae7af2d0dc643a7a1be7b94e64a
```

### `dpkg` source package: `libxdmcp=1:1.1.2-3`

Binary Packages:

- `libxdmcp6:amd64=1:1.1.2-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.dsc' libxdmcp_1.1.2-3.dsc 2145 SHA256:f9697dca6a275aeee9a3eee9fb2d55e0f77485481e8b84efc6950fc9b1988460
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2.orig.tar.gz' libxdmcp_1.1.2.orig.tar.gz 404115 SHA256:6f7c7e491a23035a26284d247779174dedc67e34e93cc3548b648ffdb6fc57c0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.diff.gz' libxdmcp_1.1.2-3.diff.gz 18017 SHA256:5844df115c17e5ba40ac116f80373304d821c607e763ef6f40562421f5cc0cf3
```

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

- `libxext6:amd64=2:1.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3-1.dsc' libxext_1.3.3-1.dsc 2221 SHA256:47106df75b8f3db1e43803e8e94a2e966cd23f7daa8cfc393af739a9e33ef955
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3.orig.tar.gz' libxext_1.3.3.orig.tar.gz 468441 SHA256:eb0b88050491fef4716da4b06a4d92b4fc9e76f880d6310b2157df604342cfe5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3-1.diff.gz' libxext_1.3.3-1.diff.gz 20763 SHA256:e294a4884eb68acbd151312cb0c973aad63268b637b15ccf1911864b7197557e
```

### `dpkg` source package: `libxfixes=1:5.0.3-1`

Binary Packages:

- `libxfixes3:amd64=1:5.0.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxfixes=1:5.0.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.3-1.dsc' libxfixes_5.0.3-1.dsc 2040 SHA256:87c1c491d8ff261b5a723c6c6aa974f315ff6f25f47425285a62065cbf944025
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.3.orig.tar.gz' libxfixes_5.0.3.orig.tar.gz 360412 SHA256:9ab6c13590658501ce4bd965a8a5d32ba4d8b3bb39a5a5bc9901edffc5666570
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.3-1.diff.gz' libxfixes_5.0.3-1.diff.gz 15140 SHA256:95b9688465531c60ff372bf8a2eb5fdd456970cbbb679ba13e54d24af44fb904
```

### `dpkg` source package: `libxi=2:1.7.9-1`

Binary Packages:

- `libxi6:amd64=2:1.7.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxi=2:1.7.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.9-1.dsc' libxi_1.7.9-1.dsc 2202 SHA256:fb19b7e8b9ad6306c3e8a6728f29576f956f07a7980e7b4d727259714d6ca686
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.9.orig.tar.gz' libxi_1.7.9.orig.tar.gz 604214 SHA256:463cc5370191404bc0f8a450fdbf6d9159efbbf274e5e0f427a60191fed9cf4b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.9-1.diff.gz' libxi_1.7.9-1.diff.gz 15892 SHA256:8c9c221faecc97a7ba7ff1a1a14fad580c49b72e270dc3aae40b72b2d7f4dc5e
```

### `dpkg` source package: `libxinerama=2:1.1.3-1`

Binary Packages:

- `libxinerama1:amd64=2:1.1.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxinerama=2:1.1.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3-1.dsc' libxinerama_1.1.3-1.dsc 2198 SHA256:4cf9a3558bd7ce1b4f55a581175c05e4b4a172364458a21ff4b657b714688fbb
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3.orig.tar.gz' libxinerama_1.1.3.orig.tar.gz 350141 SHA256:0ba243222ae5aba4c6a3d7a394c32c8b69220a6872dbb00b7abae8753aca9a44
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3-1.diff.gz' libxinerama_1.1.3-1.diff.gz 15738 SHA256:2b1487e3511ddabfec666a62f6e5e8ac4f97536b0d53c51f7bf4cbe07508a130
```

### `dpkg` source package: `libxkbcommon=0.8.2-1~ubuntu18.04.1`

Binary Packages:

- `libxkbcommon0:amd64=0.8.2-1~ubuntu18.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxkbcommon=0.8.2-1~ubuntu18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxkbcommon/libxkbcommon_0.8.2-1~ubuntu18.04.1.dsc' libxkbcommon_0.8.2-1~ubuntu18.04.1.dsc 2178 SHA256:86b561d0df66d061cd968b532f0d8c463ab47953cc18a2a592e87ec63edcafa1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxkbcommon/libxkbcommon_0.8.2-1~ubuntu18.04.1.tar.gz' libxkbcommon_0.8.2-1~ubuntu18.04.1.tar.gz 615081 SHA256:d17cd2366ca48362589fd759eb715982e48570629b6a2c1c70ffd499847de720
```

### `dpkg` source package: `libxml2=2.9.4+dfsg1-6.1ubuntu1.3`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-6.1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.4+dfsg1-6.1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc 3151 SHA256:dd8d75ce7c2e568642ffd8a84ce7d8d6372babc32ee726884a539d5d24698169
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA256:a74ad55e346aa0b2b41903e66d21f8f3d2a736b3f41e32496376861ab484184e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz 39680 SHA256:f746e94d2dd252b2e605f2d2fb265b7e788f6fadd45e76588928e2b889349917
```

### `dpkg` source package: `libxrandr=2:1.5.1-1`

Binary Packages:

- `libxrandr2:amd64=2:1.5.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrandr=2:1.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.1-1.dsc' libxrandr_1.5.1-1.dsc 2046 SHA256:0d7102ab75fdfe06534e842d5dcac8430614c61a061ab12794e2285712b0b103
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.1.orig.tar.gz' libxrandr_1.5.1.orig.tar.gz 388607 SHA256:2baa7fb3eca78fe7e11a09b373ba898b717f7eeba4a4bfd68187e04b4789b0d3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.1-1.diff.gz' libxrandr_1.5.1-1.diff.gz 16386 SHA256:42262cbc2117ea559a4e16a02c6ea6478554aa2128d9fe1e141da07006612a1d
```

### `dpkg` source package: `libxrender=1:0.9.10-1`

Binary Packages:

- `libxrender1:amd64=1:0.9.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.dsc' libxrender_0.9.10-1.dsc 2064 SHA256:95d6471218b44f4e60c48cea60cfb4865bbe861530add23f6c859515bee92dbd
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA256:770527cce42500790433df84ec3521e8bf095dfe5079454a92236494ab296adf
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.diff.gz' libxrender_0.9.10-1.diff.gz 15399 SHA256:ff56a0a00119383adc5f1731e86155ae5c2de069e1d059a9da1d777917430588
```

### `dpkg` source package: `libxslt=1.1.29-5ubuntu0.2`

Binary Packages:

- `libxslt1.1:amd64=1.1.29-5ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.29-5ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.dsc' libxslt_1.1.29-5ubuntu0.2.dsc 2502 SHA256:2b8253a9387cf6dfd96696fa39c1a228249d9463293f33536a5cf5978c96d259
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29.orig.tar.gz' libxslt_1.1.29.orig.tar.gz 3428524 SHA256:b5976e3857837e7617b29f2249ebb5eeac34e249208d31f1fbf7a6ba7a4090ce
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.debian.tar.xz' libxslt_1.1.29-5ubuntu0.2.debian.tar.xz 36520 SHA256:d6fcf48ac5c8a6e8af41c57dba2add6a8d608939370210c9a1d0d888f5088863
```

### `dpkg` source package: `libzstd=1.3.3+dfsg-2ubuntu1.1`

Binary Packages:

- `libzstd1:amd64=1.3.3+dfsg-2ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause-with-patent-grant`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.3.3+dfsg-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.dsc' libzstd_1.3.3+dfsg-2ubuntu1.1.dsc 2390 SHA256:625d37dcb1b8b26dea3e9b38c9a10db4f4dfa275d889f98dd0f62db3d0e2fa31
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg.orig.tar.xz' libzstd_1.3.3+dfsg.orig.tar.xz 1333584 SHA256:e236191547a0ab53cc52c0207ead0d51305dbe9452b5f34d4ea9eb1f51031a93
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz' libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz 12808 SHA256:9c7421170f0a1e6234147a89ba7fa5933c0771177423e962e6faf3fd13dcbb64
```

### `dpkg` source package: `lp-solve=5.5.0.15-4build1`

Binary Packages:

- `lp-solve=5.5.0.15-4build1`

Licenses: (parsed from: `/usr/share/doc/lp-solve/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris lp-solve=5.5.0.15-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lp-solve/lp-solve_5.5.0.15-4build1.dsc' lp-solve_5.5.0.15-4build1.dsc 2242 SHA256:54793e62079b91ae7e47a7a282650ec46740ed9881284efe0e5b39090ac7a267
'http://archive.ubuntu.com/ubuntu/pool/main/l/lp-solve/lp-solve_5.5.0.15.orig-doc.tar.gz' lp-solve_5.5.0.15.orig-doc.tar.gz 1484929 SHA256:a9dcfa62148a283a6e11c0bb9524f4d5a4a4ecf06511e32cbd2faec04f791e17
'http://archive.ubuntu.com/ubuntu/pool/main/l/lp-solve/lp-solve_5.5.0.15.orig.tar.gz' lp-solve_5.5.0.15.orig.tar.gz 802881 SHA256:ea1243e8aa2f0d52172dc0a90d1c2a8d2a4f696a39fc9cf07321810363d18985
'http://archive.ubuntu.com/ubuntu/pool/main/l/lp-solve/lp-solve_5.5.0.15-4build1.debian.tar.xz' lp-solve_5.5.0.15-4build1.debian.tar.xz 9716 SHA256:c8d47e23c925e601669624e6b90f577596f4a5d534b71f31b5093621f6315469
```

### `dpkg` source package: `lsb=9.20170808ubuntu1`

Binary Packages:

- `lsb-base=9.20170808ubuntu1`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20170808ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20170808ubuntu1.dsc' lsb_9.20170808ubuntu1.dsc 2126 SHA256:9b98df7b442472d172612bf6855b4dbc3cd6d5892d8073605dda786fec94af5f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20170808ubuntu1.tar.xz' lsb_9.20170808ubuntu1.tar.xz 45492 SHA256:b26bcb746e0bff05ad3e15dfbeb0ba7ea2a8d031f765a6cfa568c57d14c522c4
```

### `dpkg` source package: `lz4=0.0~r131-2ubuntu3`

Binary Packages:

- `liblz4-1:amd64=0.0~r131-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=0.0~r131-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu3.dsc' lz4_0.0~r131-2ubuntu3.dsc 2129 SHA256:b6f9a71053ff1414f695790833e689dc8bd4c48169b05a8df8de47edba7a7b58
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131.orig.tar.gz' lz4_0.0~r131.orig.tar.gz 133784 SHA256:9d4d00614d6b9dec3114b33d1224b6262b99ace24434c53487a0c8fd0b18cfed
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu3.debian.tar.xz' lz4_0.0~r131-2ubuntu3.debian.tar.xz 5340 SHA256:94834bac922397529ffc185f9c4c7e7a6eb1ef3bc527f3fcd26e36fc9430afa7
```

### `dpkg` source package: `mawk=1.3.3-17ubuntu3`

Binary Packages:

- `mawk=1.3.3-17ubuntu3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu3.dsc' mawk_1.3.3-17ubuntu3.dsc 1970 SHA256:2893a0c18b75c41d480be67d5d4edb7124ed7e9b5ed643d2670aa34481f7a77c
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu3.diff.gz' mawk_1.3.3-17ubuntu3.diff.gz 64052 SHA256:d1be148525885cb1869e35514f55005b5043f3310b08c444625005a3e14c81fc
```

### `dpkg` source package: `mhash=0.9.9.9-7`

Binary Packages:

- `libmhash2:amd64=0.9.9.9-7`

Licenses: (parsed from: `/usr/share/doc/libmhash2/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris mhash=0.9.9.9-7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mhash/mhash_0.9.9.9-7.dsc' mhash_0.9.9.9-7.dsc 1947 SHA256:cb4349ff77c8ad7ecb0b5d02083d0a0f2d60f7e8dd6ce4735cbafc7b4dc63461
'http://archive.ubuntu.com/ubuntu/pool/main/m/mhash/mhash_0.9.9.9.orig.tar.gz' mhash_0.9.9.9.orig.tar.gz 577533 SHA256:73991e9e54bb392484a510943d4c5d395462181cc4abe53f863edec13c335403
'http://archive.ubuntu.com/ubuntu/pool/main/m/mhash/mhash_0.9.9.9-7.debian.tar.xz' mhash_0.9.9.9-7.debian.tar.xz 11120 SHA256:229076933ac07420e16f7ab76e820aba79158cd7c5f3204fd1adac4f048bbe5a
```

### `dpkg` source package: `mime-support=3.60ubuntu1`

Binary Packages:

- `mime-support=3.60ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.60ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.60ubuntu1.dsc' mime-support_3.60ubuntu1.dsc 1712 SHA256:1e58e26d0f87f25ebe6c08007e9d354a24457ab73d40a1eb3b9ab62ea0d366d5
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.60ubuntu1.tar.gz' mime-support_3.60ubuntu1.tar.gz 37743 SHA256:cb1bc122ac2dc7046f6c0c06146ac0897a3c1c02e7e5e53cdd30817db2c62d33
```

### `dpkg` source package: `mpdecimal=2.4.2-1ubuntu1`

Binary Packages:

- `libmpdec2:amd64=2.4.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1ubuntu1.dsc' mpdecimal_2.4.2-1ubuntu1.dsc 2051 SHA256:6a1a2c1b839492e178d601dc6b9de26a3173124b35659ccd21362167a4fabda9
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1ubuntu1.debian.tar.xz' mpdecimal_2.4.2-1ubuntu1.debian.tar.xz 5328 SHA256:091414d364411f1d05b496f877e04d8ad22d52441cb698d739929907e94e0fc7
```

### `dpkg` source package: `mythes=2:1.2.4-3`

Binary Packages:

- `libmythes-1.2-0:amd64=2:1.2.4-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris mythes=2:1.2.4-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mythes/mythes_1.2.4-3.dsc' mythes_1.2.4-3.dsc 1846 SHA256:d308af92445c1ed8cbadd3d57df0a3aa4ac1063d158d5337fe682b259e8d0c47
'http://archive.ubuntu.com/ubuntu/pool/main/m/mythes/mythes_1.2.4.orig.tar.gz' mythes_1.2.4.orig.tar.gz 4910303 SHA256:1e81f395d8c851c3e4e75b568e20fa2fa549354e75ab397f9de4b0e0790a305f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mythes/mythes_1.2.4-3.debian.tar.xz' mythes_1.2.4-3.debian.tar.xz 5060 SHA256:4515e2ef57f2d35de4034dc5ffbf0964a27dd6cb6189b16b50cc8fa0d6914cbe
```

### `dpkg` source package: `ncurses=6.1-1ubuntu1.18.04`

Binary Packages:

- `libncurses5:amd64=6.1-1ubuntu1.18.04`
- `libncursesw5:amd64=6.1-1ubuntu1.18.04`
- `libtinfo5:amd64=6.1-1ubuntu1.18.04`
- `ncurses-base=6.1-1ubuntu1.18.04`
- `ncurses-bin=6.1-1ubuntu1.18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1-1ubuntu1.18.04
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.dsc' ncurses_6.1-1ubuntu1.18.04.dsc 4702 SHA256:9ff732e257304efa8ab3e5dba1ee85f6a360866466261c6a19f1a5d45b62d8f7
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz' ncurses_6.1.orig.tar.gz 3365395 SHA256:aa057eeeb4a14d470101eff4597d5833dcef5965331be3528c08d99cebaa0d17
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz.asc' ncurses_6.1.orig.tar.gz.asc 251 SHA256:47fd6ab5c2b08758f9c372c2bb75f2f0dbcd5cf58ae30b08f791a903da0259a4
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.debian.tar.xz' ncurses_6.1-1ubuntu1.18.04.debian.tar.xz 57464 SHA256:5f6822a052024372aa181f32dbe689ba3efd47920b5ffd3bae3c57c07f913983
```

### `dpkg` source package: `neon27=0.30.2-3~ubuntu18.04.1`

Binary Packages:

- `libneon27-gnutls:amd64=0.30.2-3~ubuntu18.04.1`

Licenses: (parsed from: `/usr/share/doc/libneon27-gnutls/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris neon27=0.30.2-3~ubuntu18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/neon27/neon27_0.30.2-3~ubuntu18.04.1.dsc' neon27_0.30.2-3~ubuntu18.04.1.dsc 2321 SHA256:d329fe7f7b0eb7e390fe0f46d9e5bb6221502cc28bf81b30071abef1b0a7c9b5
'http://archive.ubuntu.com/ubuntu/pool/main/n/neon27/neon27_0.30.2.orig.tar.gz' neon27_0.30.2.orig.tar.gz 932779 SHA256:db0bd8cdec329b48f53a6f00199c92d5ba40b0f015b153718d1b15d3d967fbca
'http://archive.ubuntu.com/ubuntu/pool/main/n/neon27/neon27_0.30.2-3~ubuntu18.04.1.debian.tar.xz' neon27_0.30.2-3~ubuntu18.04.1.debian.tar.xz 12664 SHA256:e91f153bec47832ea80400fb8f89851d7eaf7a08680c50747390c959e25aaf65
```

### `dpkg` source package: `nettle=3.4-1`

Binary Packages:

- `libhogweed4:amd64=3.4-1`
- `libnettle6:amd64=3.4-1`

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
$ apt-get source -qq --print-uris nettle=3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4-1.dsc' nettle_3.4-1.dsc 2238 SHA256:0ceb4600fdedf43916e95fb6b354ebb4038f00f5814433582d0481b510310e86
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.orig.tar.gz' nettle_3.4.orig.tar.gz 1935069 SHA256:ae7a42df026550b85daca8389b6a60ba6313b0567f374392e54918588a411e94
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.orig.tar.gz.asc' nettle_3.4.orig.tar.gz.asc 1238 SHA256:86d7441c7334dd95d16b1ca488fd94ec45ed6406714d4ed9887c7212e337eb2a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4-1.debian.tar.xz' nettle_3.4-1.debian.tar.xz 19884 SHA256:9bfc25562ed36449e75741b0473e0e558bc9ef5c20ca24e7c650fea87d631c03
```

### `dpkg` source package: `nghttp2=1.30.0-1ubuntu1`

Binary Packages:

- `libnghttp2-14:amd64=1.30.0-1ubuntu1`

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
$ apt-get source -qq --print-uris nghttp2=1.30.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0-1ubuntu1.dsc' nghttp2_1.30.0-1ubuntu1.dsc 2674 SHA256:1848fdc28933b7ee23dbebe3c9dcd0ca9182f95a278d627758d5ccfa2e0b44ad
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0.orig.tar.bz2' nghttp2_1.30.0.orig.tar.bz2 1839714 SHA256:f66918dd03773f4847da1d069295c758ce478cbd1fe58298a37d65e1dce056d8
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0-1ubuntu1.debian.tar.xz' nghttp2_1.30.0-1ubuntu1.debian.tar.xz 13244 SHA256:eb99f2c10cd872ce750964fc59734aa70b89ad04179291a23bfbee0e1a2903d3
```

### `dpkg` source package: `npth=1.5-3`

Binary Packages:

- `libnpth0:amd64=1.5-3`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.5-3
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5-3.dsc' npth_1.5-3.dsc 1954 SHA256:98e02623d39451685321ab638e12cd0b85f7829f6b174d03dbb806b8d899ae3f
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5.orig.tar.bz2' npth_1.5.orig.tar.bz2 299308 SHA256:294a690c1f537b92ed829d867bee537e46be93fbd60b16c04630fbbfcd9db3c2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5-3.debian.tar.xz' npth_1.5-3.debian.tar.xz 10480 SHA256:5cbaf91c95c90ab82053110eeec5ac72f5a3cab36829edb0579f1fb759ec5fec
```

### `dpkg` source package: `nspr=2:4.18-1ubuntu1`

Binary Packages:

- `libnspr4:amd64=2:4.18-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.18-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nspr/nspr_4.18-1ubuntu1.dsc' nspr_4.18-1ubuntu1.dsc 2136 SHA256:fd2977c7937d1c2a6a39d21f42bcccc8615b6c126ed6b15f1e6685e9d872fdf9
'http://archive.ubuntu.com/ubuntu/pool/main/n/nspr/nspr_4.18.orig.tar.gz' nspr_4.18.orig.tar.gz 1139663 SHA256:b89657c09bf88707d06ac238b8930d3ae08de68cb3edccfdc2e3dc97f9c8fb34
'http://archive.ubuntu.com/ubuntu/pool/main/n/nspr/nspr_4.18-1ubuntu1.debian.tar.xz' nspr_4.18-1ubuntu1.debian.tar.xz 19520 SHA256:712cd17e174defbae082724ba3278164218cd77f4fa322d5f376c0bec111b70c
```

### `dpkg` source package: `nss=2:3.35-2ubuntu2.11`

Binary Packages:

- `libnss3:amd64=2:3.35-2ubuntu2.11`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openldap=2.4.45+dfsg-1ubuntu1.6`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.45+dfsg-1ubuntu1.6`
- `libldap-common=2.4.45+dfsg-1ubuntu1.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.45+dfsg-1ubuntu1.6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg-1ubuntu1.6.dsc' openldap_2.4.45+dfsg-1ubuntu1.6.dsc 2884 SHA256:7f7b47c9ca3e1e61c7e1955813148f4f127e9c29e96efcb22b797fded2282630
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg.orig.tar.gz' openldap_2.4.45+dfsg.orig.tar.gz 4846458 SHA256:d51c70423aa0554d454fd3d43e7f2e940523b4ef07979305b48c233ae44b2b32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg-1ubuntu1.6.debian.tar.xz' openldap_2.4.45+dfsg-1ubuntu1.6.debian.tar.xz 179188 SHA256:959cf67aceadf0af09caf85615d61161df4b91ef9ff2153ea420ae7eec8b9f2d
```

### `dpkg` source package: `openssl=1.1.1-1ubuntu2.1~18.04.6`

Binary Packages:

- `libssl1.1:amd64=1.1.1-1ubuntu2.1~18.04.6`
- `openssl=1.1.1-1ubuntu2.1~18.04.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1-1ubuntu2.1~18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.dsc' openssl_1.1.1-1ubuntu2.1~18.04.6.dsc 2754 SHA256:e35516df9f2b2798065730bbc87f1b5a6b87ff4716f5ae2d3ed4a2ce32f7029f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz' openssl_1.1.1.orig.tar.gz 8337920 SHA256:2836875a0f89c03d0fdf483941512613a50cfb421d6fd94b9f41d7279d586a3d
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz.asc' openssl_1.1.1.orig.tar.gz.asc 488 SHA256:f3296150114069ea73a72eafbfdcbb295b770e7cbf3266f9590f3d0932498b3e
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz' openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz 104692 SHA256:8251b6f87af26364a341f7beeeef26ed99c7f90819804dba3c1e6bf2f698bb99
```

### `dpkg` source package: `orc=1:0.4.28-1`

Binary Packages:

- `liborc-0.4-0:amd64=1:0.4.28-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris orc=1:0.4.28-1
'http://archive.ubuntu.com/ubuntu/pool/main/o/orc/orc_0.4.28-1.dsc' orc_0.4.28-1.dsc 2415 SHA256:d7d4f24a814a9e1a739cca3be3b80c06bb6f46cfbb071ec0520d4daa58bebfc0
'http://archive.ubuntu.com/ubuntu/pool/main/o/orc/orc_0.4.28.orig.tar.xz' orc_0.4.28.orig.tar.xz 469460 SHA256:bfcd7c6563b05672386c4eedfc4c0d4a0a12b4b4775b74ec6deb88fc2bcd83ce
'http://archive.ubuntu.com/ubuntu/pool/main/o/orc/orc_0.4.28-1.debian.tar.xz' orc_0.4.28-1.debian.tar.xz 6728 SHA256:5835df79d24618b2935363d199aebee1dcf98a9e975ac33804708b7789886447
```

### `dpkg` source package: `p11-kit=0.23.9-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.9-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9-2.dsc' p11-kit_0.23.9-2.dsc 2458 SHA256:e4c271a89abf52a95d23cca02bd6fb6ea5d5611b139ac63b0db728e7d9895449
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9.orig.tar.gz' p11-kit_0.23.9.orig.tar.gz 1091561 SHA256:e1c1649c335107a8d33cf3762eb7f57b2d0681f0c7d8353627293a58d6b4db63
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9.orig.tar.gz.asc' p11-kit_0.23.9.orig.tar.gz.asc 900 SHA256:334562f6a37f96339173a33a90b246466e0b2673e03658b205d75ebbb63bad10
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9-2.debian.tar.xz' p11-kit_0.23.9-2.debian.tar.xz 21704 SHA256:fa6af69f96f6ccdce95d61e39662a38768b05f8872b2b2008d56cc4fff0ed3fd
```

### `dpkg` source package: `pam=1.1.8-3.6ubuntu2.18.04.1`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.6ubuntu2.18.04.1`
- `libpam-modules-bin=1.1.8-3.6ubuntu2.18.04.1`
- `libpam-runtime=1.1.8-3.6ubuntu2.18.04.1`
- `libpam0g:amd64=1.1.8-3.6ubuntu2.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pango1.0=1.40.14-1ubuntu0.1`

Binary Packages:

- `libpango-1.0-0:amd64=1.40.14-1ubuntu0.1`
- `libpangocairo-1.0-0:amd64=1.40.14-1ubuntu0.1`
- `libpangoft2-1.0-0:amd64=1.40.14-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.40.14-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14-1ubuntu0.1.dsc' pango1.0_1.40.14-1ubuntu0.1.dsc 3358 SHA256:4dff30f666f681591f878326115625c9eca431c9237e9affe66452a4d48d757e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14.orig.tar.xz' pango1.0_1.40.14.orig.tar.xz 858388 SHA256:90af1beaa7bf9e4c52db29ec251ec4fd0a8f2cc185d521ad1f88d01b3a6a17e3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14-1ubuntu0.1.debian.tar.xz' pango1.0_1.40.14-1ubuntu0.1.debian.tar.xz 28460 SHA256:f4c031a14629eaea9dd7a5a4209b0652ceb7cabafcd653bd112b67982cf83ba7
```

### `dpkg` source package: `pcre3=2:8.39-9`

Binary Packages:

- `libpcre3:amd64=2:8.39-9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-9
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-9.dsc' pcre3_8.39-9.dsc 2224 SHA256:cfbe37b2022027f62f236d74bb6af90befd2964161d77b2fd459c75ae7c36e36
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-9.debian.tar.gz' pcre3_8.39-9.debian.tar.gz 26333 SHA256:68be90799b722a8d5a075c3d2f48718cb21e2e736e0edf1e7e46a87c51215f55
```

### `dpkg` source package: `perl=5.26.1-6ubuntu0.3`

Binary Packages:

- `perl-base=5.26.1-6ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/perl-base/copyright`)

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
$ apt-get source -qq --print-uris perl=5.26.1-6ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1-6ubuntu0.3.dsc' perl_5.26.1-6ubuntu0.3.dsc 2768 SHA256:76badc610c519409d121d4c9b965614a798f6a681d8427d5a63a898ef3f963e8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1.orig-regen-configure.tar.gz' perl_5.26.1.orig-regen-configure.tar.gz 712883 SHA256:918f054a64b2835bc1c6ed79c1e082e7dcdb76735a95b54ee39c25ea9e245ca4
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1.orig.tar.xz' perl_5.26.1.orig.tar.xz 11922848 SHA256:fe8208133e73e47afc3251c08d2c21c5a60160165a8ab8b669c43a420e4ec680
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1-6ubuntu0.3.debian.tar.xz' perl_5.26.1-6ubuntu0.3.debian.tar.xz 174240 SHA256:9f509fc771c8b46cea480cf464f4ddb83bd33160673607a02431e42a7fba9d61
```

### `dpkg` source package: `pinentry=1.1.0-1`

Binary Packages:

- `pinentry-curses=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-1.dsc' pinentry_1.1.0-1.dsc 2910 SHA256:8cda3442923c0e18f9c3d5a2817a97a54db7447046b9c469e890abd19c680247
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2.asc' pinentry_1.1.0.orig.tar.bz2.asc 534 SHA256:0e3a7633b9fddf9c01c3dcf74aeb94888cc6d5d233f0b8357b0b9c1a1fed9a73
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-1.debian.tar.xz' pinentry_1.1.0-1.debian.tar.xz 15408 SHA256:ddee92638e762f125ac09b86b4f3b31e2d240e8d2dcce940302293bb2ea0873e
```

### `dpkg` source package: `pixman=0.34.0-2`

Binary Packages:

- `libpixman-1-0:amd64=0.34.0-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.34.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.34.0-2.dsc' pixman_0.34.0-2.dsc 2091 SHA256:a2d9b02ea4b0255813197c2266cee166578b083815e255530aec390bbc43d15c
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.34.0.orig.tar.gz' pixman_0.34.0.orig.tar.gz 878784 SHA256:21b6b249b51c6800dc9553b65106e1e37d0e25df942c90531d4c3997aa20a88e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.34.0-2.diff.gz' pixman_0.34.0-2.diff.gz 315460 SHA256:e81ec91d58776d804a2c56cbebb8c80fa3318a45a6a7246005bc96985f7dd805
```

### `dpkg` source package: `poppler=0.62.0-2ubuntu2.10`

Binary Packages:

- `libpoppler73:amd64=0.62.0-2ubuntu2.10`

Licenses: (parsed from: `/usr/share/doc/libpoppler73/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris poppler=0.62.0-2ubuntu2.10
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler/poppler_0.62.0-2ubuntu2.10.dsc' poppler_0.62.0-2ubuntu2.10.dsc 3358 SHA256:0f3e245b972711150f760ddc946c89c2093b52be4d5f52b57c553abe076f585a
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler/poppler_0.62.0.orig.tar.xz' poppler_0.62.0.orig.tar.xz 1423372 SHA256:5b9a73dfd4d6f61d165ada1e4f0abd2d420494bf9d0b1c15d0db3f7b83a729c6
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler/poppler_0.62.0-2ubuntu2.10.debian.tar.xz' poppler_0.62.0-2ubuntu2.10.debian.tar.xz 43808 SHA256:923c2bb540a923c1351561276c59cf8fb50e5821b52eec8942f9c4573541df92
```

### `dpkg` source package: `procps=2:3.3.12-3ubuntu1.2`

Binary Packages:

- `libprocps6:amd64=2:3.3.12-3ubuntu1.2`
- `procps=2:3.3.12-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libprocps6/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.12-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.dsc' procps_3.3.12-3ubuntu1.2.dsc 1920 SHA256:90aeb0430ae305b135a648772fe57255c64cbd6bd8dc900f86d92fd7448ac84c
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12.orig.tar.xz' procps_3.3.12.orig.tar.xz 840540 SHA256:042fcc93e1850aee4c193c51c03f369293fb64fe47e37b38852be6693d12a3af
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.debian.tar.xz' procps_3.3.12-3ubuntu1.2.debian.tar.xz 37736 SHA256:8773c939de7b2cb2b26709452ede19a6e315a83f5fb318e9968f4f4fca16ada4
```

### `dpkg` source package: `python3-defaults=3.6.7-1~18.04`

Binary Packages:

- `libpython3-stdlib:amd64=3.6.7-1~18.04`
- `python3=3.6.7-1~18.04`
- `python3-minimal=3.6.7-1~18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.6.7-1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.dsc' python3-defaults_3.6.7-1~18.04.dsc 2896 SHA256:a4dad3f3681c698e3f1232a4e56934877954e39c21e330f4491ba8e916bb1655
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.tar.gz' python3-defaults_3.6.7-1~18.04.tar.gz 137600 SHA256:df14f4993ac87537415f1abaa69d80790fb01e51033416bc123038f731286ed4
```

### `dpkg` source package: `python3.6=3.6.9-1~18.04ubuntu1.1`

Binary Packages:

- `libpython3.6:amd64=3.6.9-1~18.04ubuntu1.1`
- `libpython3.6-minimal:amd64=3.6.9-1~18.04ubuntu1.1`
- `libpython3.6-stdlib:amd64=3.6.9-1~18.04ubuntu1.1`
- `python3.6=3.6.9-1~18.04ubuntu1.1`
- `python3.6-minimal=3.6.9-1~18.04ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libpython3.6/copyright`, `/usr/share/doc/libpython3.6-minimal/copyright`, `/usr/share/doc/libpython3.6-stdlib/copyright`, `/usr/share/doc/python3.6/copyright`, `/usr/share/doc/python3.6-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.6=3.6.9-1~18.04ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9-1~18.04ubuntu1.1.dsc' python3.6_3.6.9-1~18.04ubuntu1.1.dsc 3470 SHA256:e780132c4fd5341e24b354d7ca37fb3d5d22f4178c1a180c0f530b18c9586e30
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9.orig.tar.xz' python3.6_3.6.9.orig.tar.xz 17212164 SHA256:5e2f5f554e3f8f7f0296f7e73d8600c4e9acbaee6b2555b83206edf5153870da
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9-1~18.04ubuntu1.1.debian.tar.xz' python3.6_3.6.9-1~18.04ubuntu1.1.debian.tar.xz 218936 SHA256:63afea0ff02387fb269d4e96a1732b0ba42740d1f7046f75d5cfcbfd719459e7
```

### `dpkg` source package: `raptor2=2.0.14-1build1`

Binary Packages:

- `libraptor2-0:amd64=2.0.14-1build1`

Licenses: (parsed from: `/usr/share/doc/libraptor2-0/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris raptor2=2.0.14-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/r/raptor2/raptor2_2.0.14-1build1.dsc' raptor2_2.0.14-1build1.dsc 2105 SHA256:0d3d3edda7468fcd04842c90934c962e9e74835906015c44eeef4f4368a843a8
'http://archive.ubuntu.com/ubuntu/pool/main/r/raptor2/raptor2_2.0.14.orig.tar.gz' raptor2_2.0.14.orig.tar.gz 1877454 SHA256:cb447b7c684cbe60f1266d622691fd20fdcf7b91f4a470c6de5fc8e8961df1b2
'http://archive.ubuntu.com/ubuntu/pool/main/r/raptor2/raptor2_2.0.14-1build1.debian.tar.xz' raptor2_2.0.14-1build1.debian.tar.xz 7716 SHA256:1e41da60d17156b90ad9bdc6c15a9102a8436897a05007b4fdbd60f18ac6e5f0
```

### `dpkg` source package: `rasqal=0.9.32-1build1`

Binary Packages:

- `librasqal3:amd64=0.9.32-1build1`

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
$ apt-get source -qq --print-uris rasqal=0.9.32-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rasqal/rasqal_0.9.32-1build1.dsc' rasqal_0.9.32-1build1.dsc 2055 SHA256:3cbd8111b3412ac661d830df3f1c1e0bfb20b9eaf770eba2605b8bfd7b2a93a2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rasqal/rasqal_0.9.32.orig.tar.gz' rasqal_0.9.32.orig.tar.gz 1544623 SHA256:eeba03218e3b7dfa033934d523a1a64671a9a0f64eadc38a01e4b43367be2e8f
'http://archive.ubuntu.com/ubuntu/pool/main/r/rasqal/rasqal_0.9.32-1build1.debian.tar.xz' rasqal_0.9.32-1build1.debian.tar.xz 6000 SHA256:fde534798a43494f5879ba977ba06db3b7767705b247f6dfbe31b93fd2570d88
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0-3.dsc' readline_7.0-3.dsc 2538 SHA256:f27a5dc9053b88641e3effc6c03b7840cbbbd887e8dcaf05d9e336c7bc7c6a53
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0.orig.tar.gz' readline_7.0.orig.tar.gz 2910016 SHA256:750d437185286f40a369e1e4f4764eda932b9459b5ec9a731628393dd3d32334
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0-3.debian.tar.xz' readline_7.0-3.debian.tar.xz 30012 SHA256:bf166310d6ca7716f2bd0e9e06cee2458b0157f7989d028730fc305643560175
```

### `dpkg` source package: `redland=1.0.17-1.1`

Binary Packages:

- `librdf0:amd64=1.0.17-1.1`

Licenses: (parsed from: `/usr/share/doc/librdf0/copyright`)

- `Apache-2.0`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris redland=1.0.17-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/r/redland/redland_1.0.17-1.1.dsc' redland_1.0.17-1.1.dsc 2378 SHA256:da5aaa6ca35a38f5d59a42b4c54f43101de74feaffbee69b0619ddb2ff38e944
'http://archive.ubuntu.com/ubuntu/pool/main/r/redland/redland_1.0.17.orig.tar.gz' redland_1.0.17.orig.tar.gz 1621566 SHA256:de1847f7b59021c16bdc72abb4d8e2d9187cd6124d69156f3326dd34ee043681
'http://archive.ubuntu.com/ubuntu/pool/main/r/redland/redland_1.0.17-1.1.debian.tar.xz' redland_1.0.17-1.1.debian.tar.xz 8284 SHA256:3bf4791aa5aa82dd0e32d76c9fd8539652769b8fb60cd9a04831afab78eb4747
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc 2315 SHA256:e56822b88625bf6a51f06652fc36fa2a1348b4325ac76541800cd078192aa3d2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz 8044 SHA256:675847f5cddb860256cbf2e7d5b85918aa53b59b0fd97a466b39a5c77a399537
```

### `dpkg` source package: `sed=4.4-2`

Binary Packages:

- `sed=4.4-2`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4-2.dsc' sed_4.4-2.dsc 2006 SHA256:0e025a69a04c867048f918778771e2ba79d6ddfd62cb5ce6c3a6e255c005706c
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4.orig.tar.xz' sed_4.4.orig.tar.xz 1181664 SHA256:cbd6ebc5aaf080ed60d0162d7f6aeae58211a1ee9ba9bb25623daa6cd942683b
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4-2.debian.tar.xz' sed_4.4-2.debian.tar.xz 59600 SHA256:9f9b8bec0438ea0d0bd4315548de519543385c8196bcfcc61362f38f4cc6e7ed
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.dsc' sensible-utils_0.0.12.dsc 1732 SHA256:1b62cc5f7561b3f5692a6edaec942e2e97e8368dabff8c865867d428eecb1221
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.tar.xz' sensible-utils_0.0.12.tar.xz 62152 SHA256:99ba2ebf8c57447c69d426b99b84ff9dc817be0bc4988ec6890a14558c529e2e
```

### `dpkg` source package: `shadow=1:4.5-1ubuntu2`

Binary Packages:

- `login=1:4.5-1ubuntu2`
- `passwd=1:4.5-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.5-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.dsc' shadow_4.5-1ubuntu2.dsc 2426 SHA256:34cc68fd24c6376c16311720f20dcb345e5da19adbe39edae249a49e45cee9e1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA256:22b0952dc944b163e2370bb911b11ca275fc80ad024267cf21e496b28c23d500
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.debian.tar.xz' shadow_4.5-1ubuntu2.debian.tar.xz 471472 SHA256:0025e344b478aae6e2d9ad7657b5e1fd0ebd1fda7a55e7fc144840f75b92d358
```

### `dpkg` source package: `shared-mime-info=1.9-2`

Binary Packages:

- `shared-mime-info=1.9-2`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.9-2.dsc' shared-mime-info_1.9-2.dsc 2203 SHA256:0592a6550b9bee8895d4a4fe577a15a28a5a911135765ae74b310abaea5c5b66
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.9.orig.tar.xz' shared-mime-info_1.9.orig.tar.xz 607648 SHA256:5c0133ec4e228e41bdf52f726d271a2d821499c2ab97afd3aa3d6cf43efcdc83
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.9-2.debian.tar.xz' shared-mime-info_1.9-2.debian.tar.xz 9992 SHA256:18cb7e2c0f2a3daa2d55abc87c4619d68f537f268a3bad8510e1fcf0d6b0cd76
```

### `dpkg` source package: `sqlite3=3.22.0-1ubuntu0.4`

Binary Packages:

- `libsqlite3-0:amd64=3.22.0-1ubuntu0.4`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.22.0-1ubuntu0.4
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.dsc' sqlite3_3.22.0-1ubuntu0.4.dsc 2512 SHA256:d3d351ccddcb3fc1f08f0cd7f98e1e28a4f5d310609882933a719864cd386ae9
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig-www.tar.xz' sqlite3_3.22.0.orig-www.tar.xz 3564688 SHA256:a61a14d6f457bb31ca32f4844398140050597fe4403dc0ee19576111f407e231
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig.tar.xz' sqlite3_3.22.0.orig.tar.xz 6019648 SHA256:f973ba63b5a1ea1d72e80c585bfb945e71d3f8b74fbecccdf345a84f8c91e5d1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz' sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz 47632 SHA256:3fddb7f76857daed76685d157320271706c72529aaec2e843a83ea92bc05b689
```

### `dpkg` source package: `suitesparse=1:5.1.2-2`

Binary Packages:

- `libcolamd2:amd64=1:5.1.2-2`
- `libsuitesparseconfig5:amd64=1:5.1.2-2`

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
$ apt-get source -qq --print-uris suitesparse=1:5.1.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/suitesparse/suitesparse_5.1.2-2.dsc' suitesparse_5.1.2-2.dsc 2885 SHA256:f6fd9bb6c11445ca0fe4174a9228817d657a2f6b4ed0bc10ecb3524e68d49694
'http://archive.ubuntu.com/ubuntu/pool/main/s/suitesparse/suitesparse_5.1.2.orig.tar.gz' suitesparse_5.1.2.orig.tar.gz 45063055 SHA256:4ec8d344bd8e95b898132ddffd7ee93bfbb2c1224925d11bab844b08f9b4c3b7
'http://archive.ubuntu.com/ubuntu/pool/main/s/suitesparse/suitesparse_5.1.2-2.debian.tar.xz' suitesparse_5.1.2-2.debian.tar.xz 29056 SHA256:5e64720f4b9854dec9f7f871686b09b3ccafc24e5c698bf6a3c95089c52bc3b0
```

### `dpkg` source package: `systemd=237-3ubuntu10.42`

Binary Packages:

- `libsystemd0:amd64=237-3ubuntu10.42`
- `libudev1:amd64=237-3ubuntu10.42`

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
$ apt-get source -qq --print-uris systemd=237-3ubuntu10.42
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.42.dsc' systemd_237-3ubuntu10.42.dsc 5182 SHA256:38073197625912794aacfe4522006680aae20d1743699fa9b0de71f14536fa74
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237.orig.tar.gz' systemd_237.orig.tar.gz 6871350 SHA256:c83dabbe1c9de6b9db1dafdb7e04140c7d0535705c68842f6c0768653ba4913c
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.42.debian.tar.xz' systemd_237-3ubuntu10.42.debian.tar.xz 275288 SHA256:8f408963e65e7cd4435df53e43c17f39b4a5d3df0cf66fba99f91a8f5956f685
```

### `dpkg` source package: `sysvinit=2.88dsf-59.10ubuntu1`

Binary Packages:

- `sysvinit-utils=2.88dsf-59.10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.10ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10ubuntu1.dsc' sysvinit_2.88dsf-59.10ubuntu1.dsc 2428 SHA256:030f4e8a71381529da3141988344d6e1d0e05ba437e0cdd38d2f3786185bf285
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10ubuntu1.debian.tar.xz' sysvinit_2.88dsf-59.10ubuntu1.debian.tar.xz 132736 SHA256:faee591309aa0065aa43f44a1e840eb01db7f55379af2b45949534bd0317b734
```

### `dpkg` source package: `tar=1.29b-2ubuntu0.1`

Binary Packages:

- `tar=1.29b-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.29b-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.dsc' tar_1.29b-2ubuntu0.1.dsc 1426 SHA256:a926fddb2d770936f8925c84bb665bb7cf6fae020ff7573dd85126a54aa6acb5
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b.orig.tar.xz' tar_1.29b.orig.tar.xz 1822008 SHA256:6a59706ebee384a6cd2fb3ee1dbfbfc20c5c66c7efd7cedb28edc054fca8ba00
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.debian.tar.xz' tar_1.29b-2ubuntu0.1.debian.tar.xz 31672 SHA256:4fbae6a9aaf492dabed71d6a5e07fb1d5bad89d88eaea4c398791cd326fe44d5
```

### `dpkg` source package: `tiff=4.0.9-5ubuntu0.3`

Binary Packages:

- `libtiff5:amd64=4.0.9-5ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.9-5ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9-5ubuntu0.3.dsc' tiff_4.0.9-5ubuntu0.3.dsc 2299 SHA256:4d94bb13865a4fa532439c1302ed53b2abbe75ded475a9f039b02f0adbc3ce65
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9.orig.tar.gz' tiff_4.0.9.orig.tar.gz 2305681 SHA256:6e7bdeec2c310734e734d19aae3a71ebe37a4d842e0e23dbb1b8921c0026cfcd
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9-5ubuntu0.3.debian.tar.xz' tiff_4.0.9-5ubuntu0.3.debian.tar.xz 32200 SHA256:112756eb47b85ec49b13f697319740f682884c1cdcd4623a2b75434892c9d1fd
```

### `dpkg` source package: `tzdata=2020a-0ubuntu0.18.04`

Binary Packages:

- `tzdata=2020a-0ubuntu0.18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2020a-0ubuntu0.18.04
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.18.04.dsc' tzdata_2020a-0ubuntu0.18.04.dsc 2363 SHA256:2cda7350a6124fa6b930e51904ee56034c302101fb7357c08f9c3828c87ffc1a
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz' tzdata_2020a.orig.tar.gz 397245 SHA256:547161eca24d344e0b5f96aff6a76b454da295dc14ed4ca50c2355043fb899a2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz.asc' tzdata_2020a.orig.tar.gz.asc 833 SHA256:a92f085fe1e7f8bc0f0a0bc4432f27e6cf2d69e64d4a90958bd023eb0ccf45f9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.18.04.debian.tar.xz' tzdata_2020a-0ubuntu0.18.04.debian.tar.xz 104992 SHA256:a983c500ec5b85f5b111350edc7b59533557e0c439bad23ccfeb940f93b6b73f
```

### `dpkg` source package: `ubuntu-keyring=2018.09.18.1~18.04.0`

Binary Packages:

- `ubuntu-keyring=2018.09.18.1~18.04.0`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2018.09.18.1~18.04.0
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.dsc' ubuntu-keyring_2018.09.18.1~18.04.0.dsc 1503 SHA256:1c9a599b6b3c98fdc920756c8031678d2556b6267eb55f057d0369cfc64e0263
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz' ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz 34238 SHA256:7095b786c02816bb6933b3a73ed6c9e302542e8fc1edb8346f7ddab49e95b3bd
```

### `dpkg` source package: `ubuntu-themes=16.10+18.04.20181005-0ubuntu1`

Binary Packages:

- `ubuntu-mono=16.10+18.04.20181005-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-mono/copyright`)

- `CC-BY-SA-3.0`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-themes=16.10+18.04.20181005-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-themes/ubuntu-themes_16.10+18.04.20181005-0ubuntu1.dsc' ubuntu-themes_16.10+18.04.20181005-0ubuntu1.dsc 2345 SHA256:7464db211a9c9e0a658e10aa27230904fa83f37215a6bc2f17ad1caa27672e07
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-themes/ubuntu-themes_16.10+18.04.20181005.orig.tar.gz' ubuntu-themes_16.10+18.04.20181005.orig.tar.gz 16239257 SHA256:ac6113a14a321eeb54adbc5fe08181c232eeb8f744e253cbe5fe8dc1106248ae
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-themes/ubuntu-themes_16.10+18.04.20181005-0ubuntu1.diff.gz' ubuntu-themes_16.10+18.04.20181005-0ubuntu1.diff.gz 28561 SHA256:f411edf412edfa1afb682e802575772b0ae92e0e2933c205e95eded5bb525e7c
```

### `dpkg` source package: `ucf=3.0038`

Binary Packages:

- `ucf=3.0038`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0038
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0038.dsc' ucf_3.0038.dsc 1445 SHA256:5fab6d0af664eac92b3404c6bb62d0a3ceb88cd21a1462b9a262d1292c77328f
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0038.tar.xz' ucf_3.0038.tar.xz 65416 SHA256:262ccd52637c869ac851838a176d76e90db8d3f12373e3b62eb89e217f93fe7e
```

### `dpkg` source package: `unzip=6.0-21ubuntu1`

Binary Packages:

- `unzip=6.0-21ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-21ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-21ubuntu1.dsc' unzip_6.0-21ubuntu1.dsc 1800 SHA256:76f9c291eae4039e31fda029426c96a332d3ce905a2306998ff55798d03ea44d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-21ubuntu1.debian.tar.xz' unzip_6.0-21ubuntu1.debian.tar.xz 21080 SHA256:8db974c22a5ef50029eb9a7e5429ff099e1cf7cfd36d3951fa4e00e4fd47843f
```

### `dpkg` source package: `util-linux=2.31.1-0.4ubuntu3.6`

Binary Packages:

- `bsdutils=1:2.31.1-0.4ubuntu3.6`
- `fdisk=2.31.1-0.4ubuntu3.6`
- `libblkid1:amd64=2.31.1-0.4ubuntu3.6`
- `libfdisk1:amd64=2.31.1-0.4ubuntu3.6`
- `libmount1:amd64=2.31.1-0.4ubuntu3.6`
- `libsmartcols1:amd64=2.31.1-0.4ubuntu3.6`
- `libuuid1:amd64=2.31.1-0.4ubuntu3.6`
- `mount=2.31.1-0.4ubuntu3.6`
- `util-linux=2.31.1-0.4ubuntu3.6`

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
$ apt-get source -qq --print-uris util-linux=2.31.1-0.4ubuntu3.6
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.31.1-0.4ubuntu3.6.dsc' util-linux_2.31.1-0.4ubuntu3.6.dsc 4147 SHA256:e1bd0d6290ebeefdeb6b2f4925d04c01b833292efcf59441343254db51f7bbf0
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.31.1.orig.tar.xz' util-linux_2.31.1.orig.tar.xz 4514032 SHA256:cfd5789570e9ff75e079471faeca1511ade1607f650523a6ad25d1e26516ae4e
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.31.1-0.4ubuntu3.6.debian.tar.xz' util-linux_2.31.1-0.4ubuntu3.6.debian.tar.xz 101672 SHA256:b019ef3e51f6dee11811afb6943bacc59fb8fb961785bfc6448a92c4a5c0f8c2
```

### `dpkg` source package: `wayland=1.16.0-1ubuntu1.1~18.04.3`

Binary Packages:

- `libwayland-client0:amd64=1.16.0-1ubuntu1.1~18.04.3`
- `libwayland-cursor0:amd64=1.16.0-1ubuntu1.1~18.04.3`
- `libwayland-egl1:amd64=1.16.0-1ubuntu1.1~18.04.3`

Licenses: (parsed from: `/usr/share/doc/libwayland-client0/copyright`, `/usr/share/doc/libwayland-cursor0/copyright`, `/usr/share/doc/libwayland-egl1/copyright`)

- `X11`

Source:

```console
$ apt-get source -qq --print-uris wayland=1.16.0-1ubuntu1.1~18.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/w/wayland/wayland_1.16.0-1ubuntu1.1~18.04.3.dsc' wayland_1.16.0-1ubuntu1.1~18.04.3.dsc 2468 SHA256:03cdef8cf7b7a37556b9be30ae8c4b73914c1e2c82e68aa11bd7fd69b7e8aad6
'http://archive.ubuntu.com/ubuntu/pool/main/w/wayland/wayland_1.16.0-1ubuntu1.1~18.04.3.tar.gz' wayland_1.16.0-1ubuntu1.1~18.04.3.tar.gz 325074 SHA256:71b3f7d7bb8c3077146d289d60bff4f8b92425e15cd4c257ea762c3d4d5768f6
```

### `dpkg` source package: `xkeyboard-config=2.23.1-1ubuntu1.18.04.1`

Binary Packages:

- `xkb-data=2.23.1-1ubuntu1.18.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xkeyboard-config=2.23.1-1ubuntu1.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xkeyboard-config/xkeyboard-config_2.23.1-1ubuntu1.18.04.1.dsc' xkeyboard-config_2.23.1-1ubuntu1.18.04.1.dsc 1645 SHA256:27cb81e9e2793b8b06559c20cf81c893b40506bd21d7d2ee7eaa9bf383d26247
'http://archive.ubuntu.com/ubuntu/pool/main/x/xkeyboard-config/xkeyboard-config_2.23.1.orig.tar.gz' xkeyboard-config_2.23.1.orig.tar.gz 1599103 SHA256:6567ccf5d134aae19ef110f5c847d5326aed01fc671167a6b8f8c47aeada0b85
'http://archive.ubuntu.com/ubuntu/pool/main/x/xkeyboard-config/xkeyboard-config_2.23.1-1ubuntu1.18.04.1.diff.gz' xkeyboard-config_2.23.1-1ubuntu1.18.04.1.diff.gz 52509 SHA256:3f0d971376a9856ca8014e37919cd759086eb5e0c3338d684b3c23d57968e800
```

### `dpkg` source package: `xmlsec1=1.2.25-1build1`

Binary Packages:

- `libxmlsec1:amd64=1.2.25-1build1`
- `libxmlsec1-nss:amd64=1.2.25-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xmlsec1=1.2.25-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xmlsec1/xmlsec1_1.2.25-1build1.dsc' xmlsec1_1.2.25-1build1.dsc 2131 SHA256:db2d5e8f74e05baa27738322bb1ac69f8bf56c21421d5c4b885f44bc5254c391
'http://archive.ubuntu.com/ubuntu/pool/main/x/xmlsec1/xmlsec1_1.2.25.orig.tar.gz' xmlsec1_1.2.25.orig.tar.gz 1839160 SHA256:967ca83edf25ccb5b48a3c4a09ad3405a63365576503bf34290a42de1b92fcd2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xmlsec1/xmlsec1_1.2.25-1build1.debian.tar.xz' xmlsec1_1.2.25-1build1.debian.tar.xz 7872 SHA256:bc71b96ace34a616298eac2571466b78a9110bc42b73bff7304463ef2966b162
```

### `dpkg` source package: `xorg=1:7.7+19ubuntu7.1`

Binary Packages:

- `x11-common=1:7.7+19ubuntu7.1`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19ubuntu7.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu7.1.dsc' xorg_7.7+19ubuntu7.1.dsc 2103 SHA256:f7d9c7bb4a6093e4c460ad07e639cb2681eb5546cf063d5944da5b4274069d2b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu7.1.tar.gz' xorg_7.7+19ubuntu7.1.tar.gz 298771 SHA256:9dfc6652a267fca006c8c98566c5fc96adca09455d9962ca6c69c30e0c181b39
```

### `dpkg` source package: `xz-utils=5.2.2-1.3`

Binary Packages:

- `liblzma5:amd64=5.2.2-1.3`

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
$ apt-get source -qq --print-uris xz-utils=5.2.2-1.3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.dsc' xz-utils_5.2.2-1.3.dsc 2575 SHA256:3ea4e6a32f6265b152f89ceafe78c8839e5f4bb1cad137b159fe2013817f9342
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz' xz-utils_5.2.2.orig.tar.xz 1016404 SHA256:f341b1906ebcdde291dd619399ae944600edc9193619dd0c0110a5f05bfcc89e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz.asc' xz-utils_5.2.2.orig.tar.xz.asc 543 SHA256:2cc0575556e1331b3f468e6e7dca5969ce86efcc315d62672279b4e68b2e449f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.debian.tar.xz' xz-utils_5.2.2-1.3.debian.tar.xz 108680 SHA256:d76c3acf39d0999c14384695394970e8f98853fd6736ba91972d3e67106bc6f6
```

### `dpkg` source package: `yajl=2.1.0-2build1`

Binary Packages:

- `libyajl2:amd64=2.1.0-2build1`

Licenses: (parsed from: `/usr/share/doc/libyajl2/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris yajl=2.1.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/y/yajl/yajl_2.1.0-2build1.dsc' yajl_2.1.0-2build1.dsc 2129 SHA256:2d84c8f4cf92edcf23774a9cfff9d3b61b49f009f4ab7872e774ced308d3929e
'http://archive.ubuntu.com/ubuntu/pool/main/y/yajl/yajl_2.1.0.orig.tar.gz' yajl_2.1.0.orig.tar.gz 83997 SHA256:3fb73364a5a30efe615046d07e6db9d09fd2b41c763c5f7d3bfb121cd5c5ac5a
'http://archive.ubuntu.com/ubuntu/pool/main/y/yajl/yajl_2.1.0-2build1.debian.tar.xz' yajl_2.1.0-2build1.debian.tar.xz 5592 SHA256:36fbc2b06f8e5cbd5b5868a42634ce64c86bbddecd6b3ae85ed5c2ac36318c81
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-0ubuntu2`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-0ubuntu2.dsc' zlib_1.2.11.dfsg-0ubuntu2.dsc 2676 SHA256:e733161caf3c6864deec55f40f80c0872f7c83bd9c6e9f937472f227ad912281
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.xz' zlib_1.2.11.dfsg.orig.tar.xz 287216 SHA256:881c8a90f488def83488aa91fd68563c023013a4b9b07a040f6da2727d76ad60
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-0ubuntu2.debian.tar.xz' zlib_1.2.11.dfsg-0ubuntu2.debian.tar.xz 18344 SHA256:afad42904f793d13a0b631e082e575d90a7c7c443973d08a00061a9bbb5ca380
```
