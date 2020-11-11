# `silverpeas:6.1`

## Docker Metadata

- Image ID: `sha256:46fff63198e279a1ca6f61905ae7e8983e62a08eecfd5bc3079da2eae2f5150c`
- Created: `2020-08-20T01:00:34.707890509Z`
- Virtual Size: ~ 2.47 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/opt/run.sh"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `TERM=xterm`
  - `LANG=en_US.UTF-8`
  - `LANGUAGE=en_US.UTF-8`
  - `LC_ALL=en_US.UTF-8`
  - `JAVA_HOME=/docker-java-home`
  - `SILVERPEAS_HOME=/opt/silverpeas`
  - `JBOSS_HOME=/opt/wildfly`
  - `SILVERPEAS_VERSION=6.1`
  - `WILDFLY_VERSION=18.0.1`
- Labels:
  - `build=2`
  - `description=Image to install and to run Silverpeas 6`
  - `name=Silverpeas 6`
  - `vendor=Silverpeas`
  - `version=6.1`

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

### `dpkg` source package: `alsa-lib=1.1.3-5ubuntu0.5`

Binary Packages:

- `libasound2:amd64=1.1.3-5ubuntu0.5`
- `libasound2-data=1.1.3-5ubuntu0.5`

Licenses: (parsed from: `/usr/share/doc/libasound2/copyright`, `/usr/share/doc/libasound2-data/copyright`)

- `LGPL-2.1`
- `LPGL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris alsa-lib=1.1.3-5ubuntu0.5
'http://archive.ubuntu.com/ubuntu/pool/main/a/alsa-lib/alsa-lib_1.1.3-5ubuntu0.5.dsc' alsa-lib_1.1.3-5ubuntu0.5.dsc 2612 SHA512:8caf5dfc34762d844c41c81bb10d248ceda55e21a5d24789d9055a024a4ac76d04ee9e890e4dea048ad48cf4942b736718c1bba3f9f46b14da7aaffa318293b7
'http://archive.ubuntu.com/ubuntu/pool/main/a/alsa-lib/alsa-lib_1.1.3.orig.tar.bz2' alsa-lib_1.1.3.orig.tar.bz2 962001 SHA512:f5dbe2375a8c66af14378314a5238284d4ed63dfc86a750c0c6e8f6cdb6b1ea2d8ef26f870b5d152dc0b77d9b40821cab523f6734902b91583beb08e28c66850
'http://archive.ubuntu.com/ubuntu/pool/main/a/alsa-lib/alsa-lib_1.1.3-5ubuntu0.5.debian.tar.xz' alsa-lib_1.1.3-5ubuntu0.5.debian.tar.xz 142408 SHA512:a3db9f97d838a005057ebdad5889e82bd86a3b5fe5fc28c000feda8ff4a904622580153bb5584a4161ebbd4a4f9a48362a274d25579c657a890be5bd4b90a074
```

### `dpkg` source package: `apache-pom=18-1`

Binary Packages:

- `libapache-pom-java=18-1`

Licenses: (parsed from: `/usr/share/doc/libapache-pom-java/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apache-pom=18-1
'http://archive.ubuntu.com/ubuntu/pool/universe/a/apache-pom/apache-pom_18-1.dsc' apache-pom_18-1.dsc 2045 SHA256:85ae428afdba43d01fe7d7f942322ceb725781fe3e42f2f4915b5e55e165a633
'http://archive.ubuntu.com/ubuntu/pool/universe/a/apache-pom/apache-pom_18.orig.tar.gz' apache-pom_18.orig.tar.gz 8107 SHA256:5a7e2a1ea9767998929722bbd6c2f34f5a2b3c1cbd14e5210c5465c937acbc36
'http://archive.ubuntu.com/ubuntu/pool/universe/a/apache-pom/apache-pom_18-1.debian.tar.xz' apache-pom_18-1.debian.tar.xz 2804 SHA256:93ea901e12006f057982e7b79dcc5cb205c1fbd886350a3115c8d9c2d8fec593
```

### `dpkg` source package: `apparmor=2.12-4ubuntu5.1`

Binary Packages:

- `libapparmor1:amd64=2.12-4ubuntu5.1`

Licenses: (parsed from: `/usr/share/doc/libapparmor1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris apparmor=2.12-4ubuntu5.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.12-4ubuntu5.1.dsc' apparmor_2.12-4ubuntu5.1.dsc 3181 SHA512:954ab5ff4e791c28857d6458aa477aa60fef09a6f5191fad3d890515b6fcd893b44c278cb8055be17f51fbb07417a2bcce559ca0d07b03444b868d51a14c1be9
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.12.orig.tar.gz' apparmor_2.12.orig.tar.gz 7258450 SHA512:d85fd47c66333fe5658ee5e977b32142697f6e36c575550712ee2ace2ad0fbf2aa59c8fd3b82ad8821c0190adf8cc150cf623ea09a84d5b32bde050a03dd6e9a
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.12-4ubuntu5.1.debian.tar.xz' apparmor_2.12-4ubuntu5.1.debian.tar.xz 89084 SHA512:838586458181e4b49d21af2b6becb9b73670c198ec2314a4bd35e60ee72d5baeffcd269d7c13251d62a1554b3f3cac0e74c187a43418096ec7a0f94f6a0bb5da
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
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.dsc' apt_1.6.12ubuntu0.1.dsc 2561 SHA512:39e55dff8d40ad1c1356f00b1eaff27ab6bb803fc6ea0d0669031540cac8b623e36e36a9c9b1eafc9421f828912d3874e57e58a5347f77e28f8d9d623555ea1d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.tar.xz' apt_1.6.12ubuntu0.1.tar.xz 2172208 SHA512:77c3c1c26522f00ecd7549a51f92f50a58d4fc31a0b31d9f78663b79ab043a2c3be22cde9c568f41b19c1f87d03c999d36adc0a6518de8af262e12b5021c4c84
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

- `at-spi2-core=2.28.0-1`
- `libatspi2.0-0:amd64=2.28.0-1`

Licenses: (parsed from: `/usr/share/doc/at-spi2-core/copyright`, `/usr/share/doc/libatspi2.0-0/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.7-3.1ubuntu1.2.dsc' avahi_0.7-3.1ubuntu1.2.dsc 4186 SHA512:d0877f351d2c9c7d908fce9479ebc5255169d4deb8ccdd5de76e1b381bf7fb886b96bd6fa7cfaff0be4abd5b99c328bd13b53c7c61bd36e9a4ec87207f915570
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.7.orig.tar.gz' avahi_0.7.orig.tar.gz 1333400 SHA512:bae5a1e9204aca90b90e7fd223d19e809e3514d03ba5fa2da1e55bf1d72d3d3b98567f357900c36393613dc17dc98e15ff3ebf0f226f2f6b9766e592452a6ce7
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.7-3.1ubuntu1.2.debian.tar.xz' avahi_0.7-3.1ubuntu1.2.debian.tar.xz 35124 SHA512:372e2334c7dfa73f16ea76abddd8b26dbe1b66eeb8ee01970cb8f426cc8d61fe093914825efa93a7d000b84b92727398b5fd5692092a1cd6e9150843612f78d7
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
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.dsc' bash_4.4.18-2ubuntu1.2.dsc 2434 SHA512:9cac142b52cd93d5faa8db4e755c5509d2a98358a84e5522a669d3b2ad0b3bb87c9f9deb35a582d666baefb98c6e91a96d506ddf833d50b856d36768065eef97
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18.orig.tar.xz' bash_4.4.18.orig.tar.xz 5036272 SHA512:a0c0b84133f9dc1dd404a130a6a8ac08c4551d28bf4d0a6a9be40acee5d1465270af595191cad9584f17fe098b846a70dd1f7772f771db79ff5f03e47cfd5791
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.debian.tar.xz' bash_4.4.18-2ubuntu1.2.debian.tar.xz 65236 SHA512:84ef4350f9069601a8bfe9c444400e268b927c286970270c2c635dac8946f5f499658fe822404ae662d922655a5158b019f8a4c3dcec1ffd72b1aa40b85830e4
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

### `dpkg` source package: `bsh=2.0b4-19`

Binary Packages:

- `libbsh-java=2.0b4-19`

Licenses: (parsed from: `/usr/share/doc/libbsh-java/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris bsh=2.0b4-19
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bsh/bsh_2.0b4-19.dsc' bsh_2.0b4-19.dsc 2168 SHA256:704bc2d34e06efd788f6959b00c507eb9e306a24c2c5e6ae7a57ff22046caa39
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bsh/bsh_2.0b4.orig.tar.gz' bsh_2.0b4.orig.tar.gz 826645 SHA256:776a64db4967af4fdfa13e3801eaf4249afbb7ffa1ced13f525fdf44e6e340f7
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bsh/bsh_2.0b4-19.debian.tar.xz' bsh_2.0b4-19.debian.tar.xz 9636 SHA256:d373b7ed5d54d1572378f4b7b361791d06abad6d8233e14abe7ad9b0c9568022
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
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.dsc' bzip2_1.0.6-8.1ubuntu0.2.dsc 2181 SHA512:872defc414a97416d701ce8bb59ddbf44b80ebffe447d67ebba20ed13b3e006c771002c82ad11c0c669004d22ce9368254e44c6be977c21e7d92dab69ec4e33a
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA512:b1108c392a7f45218b86196498657f50333c870db4ab555ce4859a3fe76c17b4a3430b8a075b7f1c86d9ded006bdf17001b73bfcf261e2d2ee7de4998ad604fd
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2' bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2 61477 SHA512:f895cded216bd210eed7356be97630de75f650bb40d3bb0c7a26b0fadf9991188005ab1c5438e4b8f95614e6ff8c2ad5b2a94f0cc048580bcdc387a219ba7495
```

### `dpkg` source package: `ca-certificates-java=20180516ubuntu1~18.04.1`

Binary Packages:

- `ca-certificates-java=20180516ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates-java/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates-java=20180516ubuntu1~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates-java/ca-certificates-java_20180516ubuntu1~18.04.1.dsc' ca-certificates-java_20180516ubuntu1~18.04.1.dsc 1921 SHA512:8cbd4e43f34bade8b3827814c1b8161c1b6925f47f2fd9089f7acff9a38a3e3bcc58a83661768da63b7f3af29cb99466fcde136efe2e11dd7335629982ab3424
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates-java/ca-certificates-java_20180516ubuntu1~18.04.1.tar.xz' ca-certificates-java_20180516ubuntu1~18.04.1.tar.xz 17196 SHA512:8706a054d0eacc89c316744260a95c2a3fb2fc47d05f0cb260763f2b63974c76d196316fbeb206a7440f464afb5145f732457e2f1a2e4073c2dfce4cd86d353a
```

### `dpkg` source package: `ca-certificates=20190110~18.04.1`

Binary Packages:

- `ca-certificates=20190110~18.04.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `cairo=1.15.10-2ubuntu0.1`

Binary Packages:

- `libcairo-gobject2:amd64=1.15.10-2ubuntu0.1`
- `libcairo2:amd64=1.15.10-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.15.10-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10-2ubuntu0.1.dsc' cairo_1.15.10-2ubuntu0.1.dsc 2290 SHA512:4bcf578ca2f1defc527350003aa380896e9357f7a1abb47c50888ae74359333cfc1755a24df5d833f4de6b43c9c6717fe6b5fbaa60c26cfdc8920b7cdf909b0a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10.orig.tar.xz' cairo_1.15.10.orig.tar.xz 41881364 SHA512:d56dbf1675c37b70344c1202ac7b50540a99f51a243a98464b05ffb3bb6f17b240af15dea9e3553a1abd36c95c6cf75a2077932205db5461d8a6a9d8aed33686
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10-2ubuntu0.1.debian.tar.xz' cairo_1.15.10-2ubuntu0.1.debian.tar.xz 31128 SHA512:f4d7333e2f58e2ed50a90a2e5067c79af805d4f10f834ef9b5552636682d67dbe3cab7e8f5860164e3cf2c5d8232a2c7013e30bd6dd8f1dd41c354595607d5f2
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

### `dpkg` source package: `cdparanoia=3.10.2+debian-13`

Binary Packages:

- `libcdparanoia0:amd64=3.10.2+debian-13`

Licenses: (parsed from: `/usr/share/doc/libcdparanoia0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris cdparanoia=3.10.2+debian-13
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdparanoia/cdparanoia_3.10.2+debian-13.dsc' cdparanoia_3.10.2+debian-13.dsc 2195 SHA256:7ddf0ba8b09821d50a4b226c19ad008df8285cbd86d5148e035067092c544551
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdparanoia/cdparanoia_3.10.2+debian.orig.tar.gz' cdparanoia_3.10.2+debian.orig.tar.gz 178436 SHA256:402f8b8b4370dbdc276dfd624f768956d212893542a91ecbaa6b4206b2afef03
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdparanoia/cdparanoia_3.10.2+debian-13.debian.tar.xz' cdparanoia_3.10.2+debian-13.debian.tar.xz 61152 SHA256:cff55e4394f6da0fb226b9d36cf773dbd022d8ac689a01419375d88708da2614
```

### `dpkg` source package: `chromaprint=1.4.3-1`

Binary Packages:

- `libchromaprint1:amd64=1.4.3-1`

Licenses: (parsed from: `/usr/share/doc/libchromaprint1/copyright`)

- `BSD-3-clause`
- `Expat`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris chromaprint=1.4.3-1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/chromaprint/chromaprint_1.4.3-1.dsc' chromaprint_1.4.3-1.dsc 2257 SHA256:ea067cb8fdbdf773d6a3176a12315e658546d08f5aa2ebd713d85105bf370f2f
'http://archive.ubuntu.com/ubuntu/pool/universe/c/chromaprint/chromaprint_1.4.3.orig.tar.gz' chromaprint_1.4.3.orig.tar.gz 613718 SHA256:d4ae6596283aad7a015a5b0445012054c634a4b9329ecb23000cd354b40a283b
'http://archive.ubuntu.com/ubuntu/pool/universe/c/chromaprint/chromaprint_1.4.3-1.debian.tar.xz' chromaprint_1.4.3-1.debian.tar.xz 5648 SHA256:400f44ab9a509675ccc93b7619b90919019b50e049ed573c7085a4475c5c617e
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

### `dpkg` source package: `commons-parent=43-1`

Binary Packages:

- `libcommons-parent-java=43-1`

Licenses: (parsed from: `/usr/share/doc/libcommons-parent-java/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris commons-parent=43-1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/commons-parent/commons-parent_43-1.dsc' commons-parent_43-1.dsc 2231 SHA256:872bdd6878193c4bf1a8117bc3b61615d674e287e1ebcca98e6320950de553b4
'http://archive.ubuntu.com/ubuntu/pool/universe/c/commons-parent/commons-parent_43.orig.tar.xz' commons-parent_43.orig.tar.xz 28364 SHA256:ec67c89ccd15b59dc6b7c295af57bea9975a2482aad150499940587e58fd1986
'http://archive.ubuntu.com/ubuntu/pool/universe/c/commons-parent/commons-parent_43-1.debian.tar.xz' commons-parent_43-1.debian.tar.xz 3404 SHA256:b60aa8fb108431fd15277de8762eeec678733489a7977240c87619eb2fa674ab
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

### `dpkg` source package: `crystalhd=1:0.0~git20110715.fdd2f19-12`

Binary Packages:

- `libcrystalhd3:amd64=1:0.0~git20110715.fdd2f19-12`

Licenses: (parsed from: `/usr/share/doc/libcrystalhd3/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris crystalhd=1:0.0~git20110715.fdd2f19-12
'http://archive.ubuntu.com/ubuntu/pool/universe/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-12.dsc' crystalhd_0.0~git20110715.fdd2f19-12.dsc 2356 SHA256:24d2413fe865d91f54366f906f04ebaa8cb9a2c28b3359a83f3754581474f621
'http://archive.ubuntu.com/ubuntu/pool/universe/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz' crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz 1186072 SHA256:a1c22908b85085dcc4591bc033fe054be63eab59b7d35f0a9ab3fcb2600722b7
'http://archive.ubuntu.com/ubuntu/pool/universe/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-12.debian.tar.xz' crystalhd_0.0~git20110715.fdd2f19-12.debian.tar.xz 15260 SHA256:b634af1ff394c6e44445e29e7e6b27648d35f58e475ed1749eeaf3dc80ca15a1
```

### `dpkg` source package: `cups-filters=1.20.2-0ubuntu3.1`

Binary Packages:

- `libcupsfilters1:amd64=1.20.2-0ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/libcupsfilters1/copyright`)

- `BSD-4-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris cups-filters=1.20.2-0ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups-filters/cups-filters_1.20.2-0ubuntu3.1.dsc' cups-filters_1.20.2-0ubuntu3.1.dsc 3005 SHA512:351f4c1aab362dce2b7d95c458f8223bb4f90644228e146da03aebe91a95a6f4cf94ba97bffc85c84e0f7bc8b0600a1c17c8b7d3582a1edd6b6402af2bb759c7
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups-filters/cups-filters_1.20.2.orig.tar.xz' cups-filters_1.20.2.orig.tar.xz 1468792 SHA512:94cc2a452b8dc1ed5f03b98e0530d7489dd5a369413b0ab0e7b054fcb198e8fee283507de2ef836df8ce9fb7f217794737fa4851baba72e5b79e38ad02ee61ea
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups-filters/cups-filters_1.20.2-0ubuntu3.1.debian.tar.xz' cups-filters_1.20.2-0ubuntu3.1.debian.tar.xz 74396 SHA512:002ae27c7e2eccf71fd8c9e94536ce41b1d4893c270251546ca4a4424b54e4c7e66327f5c04e3052e3086c1cb800faffe531f405db1319bc727b96456c023b23
```

### `dpkg` source package: `cups=2.2.7-1ubuntu2.8`

Binary Packages:

- `libcups2:amd64=2.2.7-1ubuntu2.8`
- `libcupsimage2:amd64=2.2.7-1ubuntu2.8`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`, `/usr/share/doc/libcupsimage2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.2.7-1ubuntu2.8
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7-1ubuntu2.8.dsc' cups_2.2.7-1ubuntu2.8.dsc 3647 SHA512:3060cb80048cdd63aeb4c2432d074f1d962d918779620c752be883f3759b7e8e12d09a2cc21a3d00d0a8fcda48f6a5c6119454a274b5dd87a80a8a76fea833aa
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7.orig.tar.gz' cups_2.2.7.orig.tar.gz 10330296 SHA512:780a6a484f38967ff678456ec7b532aa8445a9562663e4e4f6f7a24aac6ec9e8eae36459ee3c025dff053d59ad1d9ecfb823e8a832bae9d384db3d1a10d8860e
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7.orig.tar.gz.asc' cups_2.2.7.orig.tar.gz.asc 872 SHA512:0fe9291e40afb7090c9262d16ab11dce250ac04763300ba300fb89df30be002eb6f737a6ec396135bb35a90dc45c82cf3a1a34682469baf75abdcbf0389469fd
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.2.7-1ubuntu2.8.debian.tar.xz' cups_2.2.7-1ubuntu2.8.debian.tar.xz 363376 SHA512:1f0d47719abab3054005a4d382f1388e40fac88d340a71fa4b0b7d6e01c4f8bedcc96c72bc0046a545d3c57fb97735c690bc9db4839243523133c9c0a963957b
```

### `dpkg` source package: `curl=7.58.0-2ubuntu3.10`

Binary Packages:

- `libcurl3-gnutls:amd64=7.58.0-2ubuntu3.10`

Licenses: (parsed from: `/usr/share/doc/libcurl3-gnutls/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.58.0-2ubuntu3.10
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.dsc' curl_7.58.0-2ubuntu3.10.dsc 2781 SHA512:6674bade118bb14272b82c6a0d803ebe0de0ae1530e752518e4b409a31c8448694a4551fcdcbec595d5fe0a53712ec6d5076ae0e4b4d705140fa575cdcc6e269
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0.orig.tar.gz' curl_7.58.0.orig.tar.gz 3879728 SHA512:7b12b79107558bb266672d6e128615fe5a8149c37f4ae540197e3298f5d312beb2d78fbb23e3ea84ea7afc41549898a1e5cd38509f0388b11707b48d5efb8ca3
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.debian.tar.xz' curl_7.58.0-2ubuntu3.10.debian.tar.xz 41908 SHA512:6ec45923614cadc69045ff317270e1494687ea75fa4298df9fe0b23b3d22bf14f7ccf05edbd515cd7d8f011bce4e05faedcb6f327a030584b237a3b76752187f
```

### `dpkg` source package: `cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`
- `libsasl2-modules:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`
- `libsasl2-modules-db:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc 3297 SHA512:0c64b0a5cffa46d49ddd4a359c35e1b92d3c446415e8faf29c7a8d689073dc9bbcd0427aff30ee8d70b1712b27dc202ec14c955538d92998ecd6dc96569b2665
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz 1143888 SHA512:cd684133dcea5856301f50e378ff105e88f8008af06bd4e02fb9a62a88ece2ee1901ea2776ef3d941d6a3cfc2a77875c08054326293818db89e5f9995c4cd524
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz 95712 SHA512:c8eb0ff8cf4db3a3d3af2875626d9f39c058ea259c41d9954be18b269fc0fe0809ac2fea63c1ede72873cfa7388f8b76685e77eaaab64695d62739cef6ad6715
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
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.dsc' db5.3_5.3.28-13.1ubuntu1.1.dsc 3068 SHA512:20b2e7cddbf97b5de71d782b6df35c6586686da822ae978e5d60acfb3fecd4b00568b24a5ff33bfe05bc8776a0dc4d4d5dc0cc1b127f4fd0bb2d485f6fb108bd
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA512:080483cac3119569e04c3c22c95e97e5e448c88d87a443933d0ef2c71b506f309428584d6a8fb9c236c616dd82beffa1b30361b4c918756745983fcf54a3f8da
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz' db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz 29444 SHA512:0e30e4884d67561970fcff40f41641cb7bd663cc5310d396ddc002a26b348d12ca46dd2f265cfd479daffbc42530d047a177b943d65d96dfb483cd1c4e918dc4
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

- `dbus=1.12.2-1ubuntu1.2`
- `libdbus-1-3:amd64=1.12.2-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/dbus/copyright`, `/usr/share/doc/libdbus-1-3/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2-1ubuntu1.2.dsc' dbus_1.12.2-1ubuntu1.2.dsc 3561 SHA512:46b9a2332181b0ce5cbe905f9ada7d059c79a3aa139a5dd96ee8c368a6498a39d160687774b3ba01db33e2cb7233b5e29f91aee95219ebc9f57d09ce0b2dc4c7
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2.orig.tar.gz' dbus_1.12.2.orig.tar.gz 2063143 SHA512:523698ae543a4f1d9142898351ed38827882a3ca583ca7934676af48d09219ea562ae77d734cd142e5ca0d5e74f9e8d0fdeb1019592ca3524e2b690c6283f7cd
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.2-1ubuntu1.2.debian.tar.xz' dbus_1.12.2-1ubuntu1.2.debian.tar.xz 67596 SHA512:3c79ea1f37426593edb3340dce51ad07c007a802125c4113f0c0be685eae0dd6cc6f75c00a337013d8a3e494fbf3ed8761ee058986b7613b23ffaa10633708d1
```

### `dpkg` source package: `debconf=1.5.66ubuntu1`

Binary Packages:

- `debconf=1.5.66ubuntu1`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.66ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.dsc' debconf_1.5.66ubuntu1.dsc 2087 SHA512:5320524b5b84afeb7b48a50e25ba80648de989c83f3e8e6c0797e500b4be872cad0e226fe2e7c0bc3e7bed67747006ae855c5f9131e6ffb9a9618800e83d5016
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.tar.xz' debconf_1.5.66ubuntu1.tar.xz 572556 SHA512:6890b7639c884d4e28d43ac4ca27dd6ab845d9c451521d18369d57a487f2fd14966b30878065d749c60279d0f2f1996035e280e5d060b6c7ff8902bc32fac1f9
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

### `dpkg` source package: `dictionaries-common=1.27.2`

Binary Packages:

- `dictionaries-common=1.27.2`

Licenses: (parsed from: `/usr/share/doc/dictionaries-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris dictionaries-common=1.27.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dictionaries-common/dictionaries-common_1.27.2.dsc' dictionaries-common_1.27.2.dsc 1864 SHA256:2a34c911db6925f19544dda0ddbc3461332e0ae9cf07b17514b4cfa24b551ee3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dictionaries-common/dictionaries-common_1.27.2.tar.gz' dictionaries-common_1.27.2.tar.gz 360175 SHA256:11f94c2fbb632d62e82a0982df78ca66ef9319bd0ce1b423996e12c1b6f88d1d
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

### `dpkg` source package: `djvulibre=3.5.27.1-8ubuntu0.2`

Binary Packages:

- `libdjvulibre-text=3.5.27.1-8ubuntu0.2`
- `libdjvulibre21:amd64=3.5.27.1-8ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-8ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-8ubuntu0.2.dsc' djvulibre_3.5.27.1-8ubuntu0.2.dsc 1870 SHA512:096d825b4c69f8f3cb2468d8bb005c192dfa645c543079d648a7af07286aa0ceead2f73c14a967d3be20d3d36d7396e2e6c7a5056666956faaf52862131e9394
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA512:2ed11daa05995db7bf52113e2f75456c3c804988d2c17d0183b24ab379e52a4ef1871189e8bb132fec6cbc9d629b4d67a4d89ef7df7a995044cb25ff3dcc5de8
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-8ubuntu0.2.debian.tar.xz' djvulibre_3.5.27.1-8ubuntu0.2.debian.tar.xz 59648 SHA512:d6724572b94746374af80bd1165ea1630e282a5a9028d2dc9e49cd5b272b5afa26e1ecb8ade27af1a55a86265945dc7754e5f25bc15423b952afd846ddaa015d
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
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.dsc' dpkg_1.19.0.5ubuntu2.3.dsc 2144 SHA512:b788b94a2e602ab43a7fdf734f518ea8f43fd0d6ccc11a5be01d3e18d5917db1224c266a1790336093fc06a976efa390fd99d81e380f3abe291ba4686c131579
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.tar.xz' dpkg_1.19.0.5ubuntu2.3.tar.xz 4571256 SHA512:f9dc03714fee11a8bb62b3d1a556853329ab3b41dd996914cb47f38432e6b46c939433282f9039575811cb0e57508e9fbd2a5259eca7d9134d4760c636c3ec91
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
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.dsc' e2fsprogs_1.44.1-1ubuntu1.3.dsc 3188 SHA512:e5311f88ee8498252027c0c57ea62dc5a924535d93f66da281e9c1a506eee2157d008f01b96c8df5e597720fd57f05877991310b3d0cedef00a8f84645b65409
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz' e2fsprogs_1.44.1.orig.tar.gz 7544908 SHA512:c4b1f9baab70ceac9058286eeb75f57a738f01eaa0d9dd74eaaf9b0fd0709c954a0b3efb75896b9dd67ab2626febadd6635fe04a5c32e0700419d2531024dacf
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz.asc' e2fsprogs_1.44.1.orig.tar.gz.asc 488 SHA512:8e3771c784ac83b368e2258ebbd12869683be88cfad15b019ed5e60b72c21aac713494e987f3f3568e859b585808a41480027dd991163a785a93bdf78584853b
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz' e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz 81152 SHA512:0fa4885fbd73b00efbd865e17898362d6cd8551be169f8f23ea0fa52cf4de8d6c244315ef69631062fbc97c11be19f0decfac775811b47405416e5ae645e0956
```

### `dpkg` source package: `el-api=3.0.0-2~18.04`

Binary Packages:

- `libel-api-java=3.0.0-2~18.04`

Licenses: (parsed from: `/usr/share/doc/libel-api-java/copyright`)

- `Apache-2.0`
- `CDDL-1.1`
- `GPL-2`
- `GPL-2 with Classpath exception`

Source:

```console
$ apt-get source -qq --print-uris el-api=3.0.0-2~18.04
'http://archive.ubuntu.com/ubuntu/pool/universe/e/el-api/el-api_3.0.0-2~18.04.dsc' el-api_3.0.0-2~18.04.dsc 2027 SHA512:fe41ea7df9913996c5b2abd00bf60b3a2ddce794ac7c53e1a32c6ae8c899a44953169e713dceec68bcae8fe34f5b49e5c8c2409e8f5a2812ca3d5bb5eed8dab4
'http://archive.ubuntu.com/ubuntu/pool/universe/e/el-api/el-api_3.0.0.orig.tar.xz' el-api_3.0.0.orig.tar.xz 41460 SHA512:9d3de97e4856a5a580faf761769a7183d0d05354ba149b7599bb401fb796d767eab5b0125eebb926a250f344e7e706888e307964585db3cbad7648408d26fd4c
'http://archive.ubuntu.com/ubuntu/pool/universe/e/el-api/el-api_3.0.0-2~18.04.debian.tar.xz' el-api_3.0.0-2~18.04.debian.tar.xz 8620 SHA512:3701f64c4035680895f92bc67ee3f126d5788b662c2c9bf2f2871ea2e4b3b3f211b93ad3529dd95a33412a0234d19f6bc1b7738995367192e4ea8b7a720d2e98
```

### `dpkg` source package: `elfutils=0.170-0.4ubuntu0.1`

Binary Packages:

- `libelf1:amd64=0.170-0.4ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.170-0.4ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170-0.4ubuntu0.1.dsc' elfutils_0.170-0.4ubuntu0.1.dsc 2422 SHA512:cc08e16e9e1b892911f1f48d465127ec621c5dfe9ad3054d5d52e1f165b6650ae76c6f590af05ba743c414ad738379b6a9467f33776e8d2c03a4f0d7b2097507
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170.orig.tar.bz2' elfutils_0.170.orig.tar.bz2 8358001 SHA512:aca0b5e271138eaf86e36505ffb101181207b151e833e6cd7c18986ac50678542a5ecd2250f8dd6923ca497142f197c8b08fd225e4130b16b6203c24013d6d28
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170-0.4ubuntu0.1.debian.tar.xz' elfutils_0.170-0.4ubuntu0.1.debian.tar.xz 51740 SHA512:a9d615f2dced250403c897ec1e2e2ff2b44523763b88cfad5656d60e864bb42b35384fdfdad372747499732c20e40e2e7d2de06a18c5284ea19f1a1617e2f254
```

### `dpkg` source package: `emacsen-common=2.0.8`

Binary Packages:

- `emacsen-common=2.0.8`

Licenses: (parsed from: `/usr/share/doc/emacsen-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris emacsen-common=2.0.8
'http://archive.ubuntu.com/ubuntu/pool/main/e/emacsen-common/emacsen-common_2.0.8.dsc' emacsen-common_2.0.8.dsc 1423 SHA256:41299bee5a47ee221beb5b9494d388f3036de09172ae89589ebfb8b5d6f2bc14
'http://archive.ubuntu.com/ubuntu/pool/main/e/emacsen-common/emacsen-common_2.0.8.tar.xz' emacsen-common_2.0.8.tar.xz 17612 SHA256:c9247d17ff82284e26e56af55e09b0a0a33409f253b5da1410f634a306cb717b
```

### `dpkg` source package: `expat=2.2.5-3ubuntu0.2`

Binary Packages:

- `libexpat1:amd64=2.2.5-3ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.5-3ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.dsc' expat_2.2.5-3ubuntu0.2.dsc 2198 SHA512:efe01c6d1bb262332995fe1dbe25829fc5b416fa6f566505a70ed9e11ef5a4d7ca0769eab6fb0dce655f0ec4facefcff1e29d93c660c90a115819f489a0d30f8
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5.orig.tar.gz' expat_2.2.5.orig.tar.gz 8273003 SHA512:61ce2a479521412e0c56c352106c4adfb61a6bedb883921aba3ebccc29311ddd192646ac2c51b41572728d4de6ab4cb60a1dbc71515d742a80a8b59d89ca74d6
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.debian.tar.xz' expat_2.2.5-3ubuntu0.2.debian.tar.xz 12024 SHA512:79f104bce4515465616eea834d2d932aba403929799ea97ecfd09e6890307709caa9b2a4dab2e3697a124232c2ff7f31b5c5a06436df06e19ea934834779da68
```

### `dpkg` source package: `ffmpeg=7:3.4.8-0ubuntu0.2`

Binary Packages:

- `ffmpeg=7:3.4.8-0ubuntu0.2`
- `libavcodec57:amd64=7:3.4.8-0ubuntu0.2`
- `libavdevice57:amd64=7:3.4.8-0ubuntu0.2`
- `libavfilter6:amd64=7:3.4.8-0ubuntu0.2`
- `libavformat57:amd64=7:3.4.8-0ubuntu0.2`
- `libavresample3:amd64=7:3.4.8-0ubuntu0.2`
- `libavutil55:amd64=7:3.4.8-0ubuntu0.2`
- `libpostproc54:amd64=7:3.4.8-0ubuntu0.2`
- `libswresample2:amd64=7:3.4.8-0ubuntu0.2`
- `libswscale4:amd64=7:3.4.8-0ubuntu0.2`

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
$ apt-get source -qq --print-uris ffmpeg=7:3.4.8-0ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/universe/f/ffmpeg/ffmpeg_3.4.8-0ubuntu0.2.dsc' ffmpeg_3.4.8-0ubuntu0.2.dsc 4980 SHA512:f8f713748745ffbe253130e769830fb36e96bff41d84f3738d899c718980dd71fab3e537b28e25aada09e6bd8dd7d3b8331e9ab5f6b4f50632149592f5bca0f2
'http://archive.ubuntu.com/ubuntu/pool/universe/f/ffmpeg/ffmpeg_3.4.8.orig.tar.xz' ffmpeg_3.4.8.orig.tar.xz 8508108 SHA512:cafa9affadfd373ef7a089888196b6853b305bed18acbcc735f3f546fa52c8555c3e6bd41055f0bf68925d9285030f6f85048d3365af588093710491a74fe78c
'http://archive.ubuntu.com/ubuntu/pool/universe/f/ffmpeg/ffmpeg_3.4.8-0ubuntu0.2.debian.tar.xz' ffmpeg_3.4.8-0ubuntu0.2.debian.tar.xz 42392 SHA512:0a8b5c76269e6d2b7eb95cfd09d6041a4216f42a4271fe85a74114614912a018b9964bd0e33c6ee918e95af0b27da1ea8d71610f49ec8463307ed3258f8b253d
```

### `dpkg` source package: `fftw3=3.3.7-1`

Binary Packages:

- `libfftw3-double3:amd64=3.3.7-1`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.7-1.dsc' fftw3_3.3.7-1.dsc 2941 SHA256:65568aacf8b55d87392aeb640ca9bcd37b0d9f1fe2312b298c43c18764e8470a
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.7.orig.tar.xz' fftw3_3.3.7.orig.tar.xz 2354860 SHA256:1eb677807ec114a3b1dbbae5d866683b71de2977101cb116063a753365465498
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.7-1.debian.tar.xz' fftw3_3.3.7-1.debian.tar.xz 13628 SHA256:5b3763ecfa0177e7c43bf330038b4b2c4d71a5b8c9c33b3e89ccfa4e59f2011b
```

### `dpkg` source package: `file=1:5.32-2ubuntu0.4`

Binary Packages:

- `file=1:5.32-2ubuntu0.4`
- `libmagic-mgc=1:5.32-2ubuntu0.4`
- `libmagic1:amd64=1:5.32-2ubuntu0.4`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.32-2ubuntu0.4
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.32-2ubuntu0.4.dsc' file_5.32-2ubuntu0.4.dsc 1972 SHA512:5d05305d59b222640d75fbc2acc9aa5d95d890f78ab6b3343bebcced830b5c3302f1f560b1ee5f21b7f5bf7599355680a1a8ee59e8ab017916635c43b6b88e65
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.32.orig.tar.xz' file_5.32.orig.tar.xz 584352 SHA512:86e095de383a9da86f9adaf0d8cff0f99d7b9c02d75fbc49295f6c44575499e360b8878d0a69109a531307b4f4ac3a7f1655ffcf82ed9619be0e09735d0b139d
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.32-2ubuntu0.4.debian.tar.xz' file_5.32-2ubuntu0.4.debian.tar.xz 33868 SHA512:5ec41bcf4418ca2c07ed981d1a728e817505a181e59151a5f7e21303ae753dac83e6d8228f6b673c614de19eca56eb6cfe22e2ad42ce69cbaa450319a02f18b4
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
'http://archive.ubuntu.com/ubuntu/pool/main/f/flac/flac_1.3.2-1.dsc' flac_1.3.2-1.dsc 2268 SHA256:a3fc6aa13a3e871c3e2b2a8adbae76ce9aec25f11329298831c74e8c4ba65293
'http://archive.ubuntu.com/ubuntu/pool/main/f/flac/flac_1.3.2.orig.tar.xz' flac_1.3.2.orig.tar.xz 776192 SHA256:91cfc3ed61dc40f47f050a109b08610667d73477af6ef36dcad31c31a4a8d53f
'http://archive.ubuntu.com/ubuntu/pool/main/f/flac/flac_1.3.2-1.debian.tar.xz' flac_1.3.2-1.debian.tar.xz 16840 SHA256:33580dfc82808cbb87b4afe24e4bf9e9c8941f9cede035235c76046f1908559f
```

### `dpkg` source package: `flite=2.1-release-1`

Binary Packages:

- `libflite1:amd64=2.1-release-1`

Licenses: (parsed from: `/usr/share/doc/libflite1/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris flite=2.1-release-1
'http://archive.ubuntu.com/ubuntu/pool/universe/f/flite/flite_2.1-release-1.dsc' flite_2.1-release-1.dsc 1878 SHA256:dd8b64159eacf5bcdc743f720ab362a475e91f05bc5d1033f8a851d5d94337de
'http://archive.ubuntu.com/ubuntu/pool/universe/f/flite/flite_2.1-release.orig.tar.bz2' flite_2.1-release.orig.tar.bz2 14816327 SHA256:c73c3f6a2ea764977d6eaf0a287722d1e2066b4697088c552e342c790f3d2b85
'http://archive.ubuntu.com/ubuntu/pool/universe/f/flite/flite_2.1-release-1.debian.tar.xz' flite_2.1-release-1.debian.tar.xz 31144 SHA256:5f7e36406db6c8215e0a2b6d13d8cfa3b3a904c8203b6df4fb938791b8ee8066
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

### `dpkg` source package: `fonts-android=1:6.0.1r16-1.1`

Binary Packages:

- `fonts-droid-fallback=1:6.0.1r16-1.1`

Licenses: (parsed from: `/usr/share/doc/fonts-droid-fallback/copyright`)

- `Apache-2`
- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris fonts-android=1:6.0.1r16-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-android/fonts-android_6.0.1r16-1.1.dsc' fonts-android_6.0.1r16-1.1.dsc 2182 SHA256:17cf1a74074c63cd5d0cc03d81d780ecd0fcb1d8d2ab1bdafb0b6dd30c278500
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-android/fonts-android_6.0.1r16.orig.tar.gz' fonts-android_6.0.1r16.orig.tar.gz 6759063 SHA256:7f14d7b3f3ab0c7258aa7edac4ea1071cb2f22c5820c4eb617095de2ef90d4d8
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-android/fonts-android_6.0.1r16-1.1.debian.tar.xz' fonts-android_6.0.1r16-1.1.debian.tar.xz 6880 SHA256:6beeb5dfb083b73753382d2ca46faaa976c39ca6365dd33f08106d077c525b29
```

### `dpkg` source package: `fonts-crosextra-caladea=20130214-2`

Binary Packages:

- `fonts-crosextra-caladea=20130214-2`

Licenses: (parsed from: `/usr/share/doc/fonts-crosextra-caladea/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris fonts-crosextra-caladea=20130214-2
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-crosextra-caladea/fonts-crosextra-caladea_20130214-2.dsc' fonts-crosextra-caladea_20130214-2.dsc 2159 SHA256:199586f82712aa579daa428e049d3f4a747712a34ce9d8ebcf22c27072ce3252
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-crosextra-caladea/fonts-crosextra-caladea_20130214.orig.tar.gz' fonts-crosextra-caladea_20130214.orig.tar.gz 112756 SHA256:c48d1c2fd613c9c06c959c34da7b8388059e2408d2bb19845dc3ed35f76e4d09
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-crosextra-caladea/fonts-crosextra-caladea_20130214-2.debian.tar.xz' fonts-crosextra-caladea_20130214-2.debian.tar.xz 2504 SHA256:df38b095635456c3979c19e81e28c656e56675b138e4b989c25bb08b2e2eac11
```

### `dpkg` source package: `fonts-crosextra-carlito=20130920-1`

Binary Packages:

- `fonts-crosextra-carlito=20130920-1`

Licenses: (parsed from: `/usr/share/doc/fonts-crosextra-carlito/copyright`)

- `GPL-2`
- `GPL-2+`
- `OFL-1.1`

Source:

```console
$ apt-get source -qq --print-uris fonts-crosextra-carlito=20130920-1
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-crosextra-carlito/fonts-crosextra-carlito_20130920-1.dsc' fonts-crosextra-carlito_20130920-1.dsc 2137 SHA256:53be1d931294feafcee69fb3b4dd47b62d80d1cc3d42057e007dc4c681ef9e06
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-crosextra-carlito/fonts-crosextra-carlito_20130920.orig.tar.gz' fonts-crosextra-carlito_20130920.orig.tar.gz 1169488 SHA256:4bd12b6cbc321c1cf16da76e2c585c925ce956a08067ae6f6c64eff6ccfdaf5a
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-crosextra-carlito/fonts-crosextra-carlito_20130920-1.debian.tar.gz' fonts-crosextra-carlito_20130920-1.debian.tar.gz 4426 SHA256:cd2dcd85536b873a7f3e5c034efa55b93ed5e1c2e102951ce067042ac7863b38
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.dsc' fonts-dejavu_2.37-1.dsc 2575 SHA256:f35ff7b2c8dbfda6564c9dedf088ba06cc6d279fdd8e7cccbd1ae08ded1bb71c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.debian.tar.xz' fonts-dejavu_2.37-1.debian.tar.xz 10424 SHA256:5105cdbfc086f4a83ab6871eb39cc904bf02aa52762402b7cacf33d0938122f7
```

### `dpkg` source package: `fonts-liberation2=2.00.1-7~18.04.2`

Binary Packages:

- `fonts-liberation2=2.00.1-7~18.04.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fonts-liberation2=2.00.1-7~18.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-liberation2/fonts-liberation2_2.00.1-7~18.04.2.dsc' fonts-liberation2_2.00.1-7~18.04.2.dsc 2299 SHA512:894faa5d99967314c4b8bf33bf33b9c5f3a0ae8d354c7eb28dd4d5d4eb5316c4fc3e5d07dade1de2eccc98f6aea3e5c21488f171791455059f0557909f72c760
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-liberation2/fonts-liberation2_2.00.1.orig.tar.gz' fonts-liberation2_2.00.1.orig.tar.gz 4842687 SHA512:8cfc1fa8f36e9f1c622879a822614b851b8339673ed6d2736937c483d85764ef12cc0d8a308f6c50e4877c2ab9b83ca2ea748b1458aa02cc840251e400285362
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-liberation2/fonts-liberation2_2.00.1-7~18.04.2.debian.tar.xz' fonts-liberation2_2.00.1-7~18.04.2.debian.tar.xz 84692 SHA512:d465231449c9bd51fe231b787fc12a94c8ad596b7ac80aa4add5192bc02067ada858dad247c48947d6a8b02bebfe7f19cb3cd8cb1dcab8ea2f9660d4ffcc7109
```

### `dpkg` source package: `fonts-liberation=1:1.07.4-7~18.04.1`

Binary Packages:

- `fonts-liberation=1:1.07.4-7~18.04.1`

Licenses: (parsed from: `/usr/share/doc/fonts-liberation/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fonts-liberation=1:1.07.4-7~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-liberation/fonts-liberation_1.07.4-7~18.04.1.dsc' fonts-liberation_1.07.4-7~18.04.1.dsc 1939 SHA512:52a8566f2a500f8ea98994dff887795007a3761715a9cbc4f04d6c47398227916ac29adba366fca8f67b01f9ab367eda2615ccdb6a7340ac679c06e03fb78cf4
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-liberation/fonts-liberation_1.07.4.orig.tar.gz' fonts-liberation_1.07.4.orig.tar.gz 2937949 SHA512:fc5abb4903f79621157d478baed0963600b04997ded1e0b937a9a41aee3b21900430a4c8ac92e09b7bd8b635ac6cd67c9a3c9f3532ff978d235ba965c25a8f68
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-liberation/fonts-liberation_1.07.4-7~18.04.1.debian.tar.xz' fonts-liberation_1.07.4-7~18.04.1.debian.tar.xz 17048 SHA512:e3d85003696bf59b8b1354c7137689c43129c6e90819addc66f7bbd864f517ce6b84c739638fec27a82693c466b825b4a90e3aeb1028de4b98ff664481766a39
```

### `dpkg` source package: `fonts-linuxlibertine=5.3.0-4`

Binary Packages:

- `fonts-linuxlibertine=5.3.0-4`

Licenses: (parsed from: `/usr/share/doc/fonts-linuxlibertine/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Font exception`
- `OFL-1.1`

Source:

```console
$ apt-get source -qq --print-uris fonts-linuxlibertine=5.3.0-4
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-linuxlibertine/fonts-linuxlibertine_5.3.0-4.dsc' fonts-linuxlibertine_5.3.0-4.dsc 2113 SHA256:127569684fe5ab96f2294dedb7425097a410abd31aac3e2e58b54b6fdcc9abab
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-linuxlibertine/fonts-linuxlibertine_5.3.0.orig.tar.xz' fonts-linuxlibertine_5.3.0.orig.tar.xz 3748996 SHA256:9226823829273175c38ab84c4991d61ceaeded7c6ce50a2bab061d14e441a2a7
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-linuxlibertine/fonts-linuxlibertine_5.3.0-4.debian.tar.xz' fonts-linuxlibertine_5.3.0-4.debian.tar.xz 8764 SHA256:d7eb3eac6641411f55578ec8ca02f0da6c76f03dadf3a7cbe1784448ccce2d6f
```

### `dpkg` source package: `fonts-noto=20171026-2`

Binary Packages:

- `fonts-noto-mono=20171026-2`

Licenses: (parsed from: `/usr/share/doc/fonts-noto-mono/copyright`)

- `GPL-3`
- `GPL-3+`
- `SIL-1.1`

Source:

```console
$ apt-get source -qq --print-uris fonts-noto=20171026-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-noto/fonts-noto_20171026-2.dsc' fonts-noto_20171026-2.dsc 2465 SHA256:e488d36fae6c908654b7e570fc57c4f76bc1ccf0506fe6169c960ed3f418d756
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-noto/fonts-noto_20171026.orig.tar.gz' fonts-noto_20171026.orig.tar.gz 261295944 SHA256:61b7380c9c9b67dc5ee3b62c0f90d736c7cccaae8c94dead41a1ae549977ec31
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-noto/fonts-noto_20171026-2.debian.tar.xz' fonts-noto_20171026-2.debian.tar.xz 18112 SHA256:0ae5c878fbdcf6f19c38b159b9db47e2a1bc5cccbd1b76148c2f08cd8bd7f5d5
```

### `dpkg` source package: `fonts-sil-gentium-basic=1.102-1`

Binary Packages:

- `fonts-sil-gentium-basic=1.102-1`

Licenses: (parsed from: `/usr/share/doc/fonts-sil-gentium-basic/copyright`)

- `OFL-1.1`

Source:

```console
$ apt-get source -qq --print-uris fonts-sil-gentium-basic=1.102-1
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-sil-gentium-basic/fonts-sil-gentium-basic_1.102-1.dsc' fonts-sil-gentium-basic_1.102-1.dsc 2160 SHA256:246df276386d08b62316341e820787a45d2e796f150221f3ddc623633c71b304
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-sil-gentium-basic/fonts-sil-gentium-basic_1.102.orig.tar.xz' fonts-sil-gentium-basic_1.102.orig.tar.xz 380396 SHA256:a7c89371d71ee45a7c12072df75c0ef790674e39fdde747b46d6e4cfb2219f7d
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-sil-gentium-basic/fonts-sil-gentium-basic_1.102-1.debian.tar.xz' fonts-sil-gentium-basic_1.102-1.debian.tar.xz 5184 SHA256:ff836606909f0cc9afc06efde1e7657770f13a779e890b06897b2f599eb00d3b
```

### `dpkg` source package: `fonts-sil-gentium=20081126:1.03-2`

Binary Packages:

- `fonts-sil-gentium=20081126:1.03-2`

Licenses: (parsed from: `/usr/share/doc/fonts-sil-gentium/copyright`)

- `OFL-1.1`

Source:

```console
$ apt-get source -qq --print-uris fonts-sil-gentium=20081126:1.03-2
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-sil-gentium/fonts-sil-gentium_1.03-2.dsc' fonts-sil-gentium_1.03-2.dsc 2107 SHA256:d75b0fded4ab6aa63bd7adec8accdcf78e117274d251709f58ed6b2b3b60f301
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-sil-gentium/fonts-sil-gentium_1.03.orig.tar.xz' fonts-sil-gentium_1.03.orig.tar.xz 428764 SHA256:0754edaec5837f899caf9248496438cf5adc5f2795ee36ac19e49f08bdfd751c
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fonts-sil-gentium/fonts-sil-gentium_1.03-2.debian.tar.xz' fonts-sil-gentium_1.03-2.debian.tar.xz 6528 SHA256:e1b49eb3e9c2a210309b7a6177d83e99b851ed1d1cd60ccd5c9af329b880dbf9
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

### `dpkg` source package: `fribidi=0.19.7-2`

Binary Packages:

- `libfribidi0:amd64=0.19.7-2`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=0.19.7-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_0.19.7-2.dsc' fribidi_0.19.7-2.dsc 1879 SHA256:34405e7d2f1c9b7dc68ae764881b3c5213107a5d5e8cb5f0f8794e3aeb2b6f03
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_0.19.7.orig.tar.bz2' fribidi_0.19.7.orig.tar.bz2 648299 SHA256:08222a6212bbc2276a2d55c3bf370109ae4a35b689acbc66571ad2a670595a8e
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_0.19.7-2.debian.tar.xz' fribidi_0.19.7-2.debian.tar.xz 7468 SHA256:501fe8186407da1350b91d7c9670de21eb37016e6d75ace55d8e14c9d8ccb07e
```

### `dpkg` source package: `game-music-emu=0.6.2-1`

Binary Packages:

- `libgme0:amd64=0.6.2-1`

Licenses: (parsed from: `/usr/share/doc/libgme0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris game-music-emu=0.6.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/g/game-music-emu/game-music-emu_0.6.2-1.dsc' game-music-emu_0.6.2-1.dsc 2006 SHA256:8359c17b8c7d7887b3d44a5ac4958e5456afbf816ba29e6713c1e4212dbe63eb
'http://archive.ubuntu.com/ubuntu/pool/universe/g/game-music-emu/game-music-emu_0.6.2.orig.tar.xz' game-music-emu_0.6.2.orig.tar.xz 163052 SHA256:5046cb471d422dbe948b5f5dd4e5552aaef52a0899c4b2688e5a68a556af7342
'http://archive.ubuntu.com/ubuntu/pool/universe/g/game-music-emu/game-music-emu_0.6.2-1.debian.tar.xz' game-music-emu_0.6.2-1.debian.tar.xz 4412 SHA256:8ea69035bd72261ec85e5f0486707d448f7491733ae055040a9995cebb0ea820
```

### `dpkg` source package: `gcc-7=7.5.0-3ubuntu1~18.04`

Binary Packages:

- `cpp-7=7.5.0-3ubuntu1~18.04`
- `gcc-7-base:amd64=7.5.0-3ubuntu1~18.04`

Licenses: (parsed from: `/usr/share/doc/cpp-7/copyright`, `/usr/share/doc/gcc-7-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-7=7.5.0-3ubuntu1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0-3ubuntu1~18.04.dsc' gcc-7_7.5.0-3ubuntu1~18.04.dsc 28071 SHA512:1c06ed6e3fb7d3799aaad1915e318597a90ec87ec513d6710157cdf3ce877e15989ea62b70e9b6d6a06c9e24ded1174d87621d01e025797b50d13347126dc3ec
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0.orig.tar.gz' gcc-7_7.5.0.orig.tar.gz 73877115 SHA512:806470ea2d8f69a8d7eed14e38d50ea58b7cb6b8da1bd91fecf15f2f840d67f321fb9602f2c25d44f13df12f80a4f8e2dbe4450d482ae876e3678f69a93dd2d8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0-3ubuntu1~18.04.diff.gz' gcc-7_7.5.0-3ubuntu1~18.04.diff.gz 574614 SHA512:030ab7a7894d9af4ce280556bbfd90a695d6d9fc0814f768184dc0cccfb243015f35afc85b97b92a2e1fc7054872b5d59f9fddeb65ca057cbbb3ad2a17935e98
```

### `dpkg` source package: `gcc-8=8.4.0-1ubuntu1~18.04`

Binary Packages:

- `gcc-8-base:amd64=8.4.0-1ubuntu1~18.04`
- `libgcc1:amd64=1:8.4.0-1ubuntu1~18.04`
- `libgomp1:amd64=8.4.0-1ubuntu1~18.04`
- `libstdc++6:amd64=8.4.0-1ubuntu1~18.04`

Licenses: (parsed from: `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-8=8.4.0-1ubuntu1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.dsc' gcc-8_8.4.0-1ubuntu1~18.04.dsc 36382 SHA512:064409c787f62bff87a494f2952f5c3f264d5a7c8508c83b863c1a1ad410d25988cfc73afde9908221258f81714164121cc1f02e3699ca2283c6a3aa035d1ddd
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0.orig.tar.gz' gcc-8_8.4.0.orig.tar.gz 85278215 SHA512:ce6ff302ab2e252950bc446bc2b58c198c4b1a75d59122c00845c026a29068f412e0d59cd6ddd8b648838f80589252a1695afc6193fb669082c9a1c4ad14b1dc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.diff.gz' gcc-8_8.4.0-1ubuntu1~18.04.diff.gz 510634 SHA512:7bd97a04eccd35c3483a82b238d8d54c91071c4d1361cb30fb3fbf7b512c84b9d0bc80499373f2da3e17520d112125ebfebae6b93746feede78f9eecc1ccd4ac
```

### `dpkg` source package: `gcc-defaults=1.176ubuntu2.3`

Binary Packages:

- `cpp=4:7.4.0-1ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.176ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.176ubuntu2.3.dsc' gcc-defaults_1.176ubuntu2.3.dsc 15463 SHA512:77af785110200dbe6c83c7dc8f1a1e3665c5c05a8cc0a03254936fd42c7ac725d3530b4075a98aadc071050319bfe534f38901b43ba6dccc38c6f19b6514503f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.176ubuntu2.3.tar.gz' gcc-defaults_1.176ubuntu2.3.tar.gz 208597 SHA512:586932097826c71bf94d0a8506d823ff894aae9c1a1053bc71ad8a4cf5101221b058ded1f1ad019e2111ddee13e7cfe8ce197193d770dd8c80eb40d41126cd17
```

### `dpkg` source package: `gdbm=1.14.1-6`

Binary Packages:

- `libgdbm-compat4:amd64=1.14.1-6`
- `libgdbm5:amd64=1.14.1-6`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm5/copyright`)

- `GFDL-1.3+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.14.1-6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1-6.dsc' gdbm_1.14.1-6.dsc 2293 SHA256:85fc353e81fc54b49d9c13c71f4247836fb1aac2693e98416a6821de8cfe7b41
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1.orig.tar.gz' gdbm_1.14.1.orig.tar.gz 894412 SHA256:cdceff00ffe014495bed3aed71c7910aa88bf29379f795abc0f46d4ee5f8bc5f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1-6.debian.tar.xz' gdbm_1.14.1-6.debian.tar.xz 27492 SHA256:c9da59f11d5e40ecd877f1256c53ea4750b9d614c7885800e42d0f1885996658
```

### `dpkg` source package: `gdk-pixbuf=2.36.11-2`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.36.11-2`
- `libgdk-pixbuf2.0-bin=2.36.11-2`
- `libgdk-pixbuf2.0-common=2.36.11-2`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

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

### `dpkg` source package: `ghostscript=9.26~dfsg+0-0ubuntu0.18.04.12`

Binary Packages:

- `ghostscript=9.26~dfsg+0-0ubuntu0.18.04.12`
- `libgs9:amd64=9.26~dfsg+0-0ubuntu0.18.04.12`
- `libgs9-common=9.26~dfsg+0-0ubuntu0.18.04.12`

Licenses: (parsed from: `/usr/share/doc/ghostscript/copyright`, `/usr/share/doc/libgs9/copyright`, `/usr/share/doc/libgs9-common/copyright`)

- `AGPL-3`
- `AGPL-3+`
- `AGPL-3+ with font exception`
- `Apache-2.0`
- `BSD-2-Clause`
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `giflib=5.1.4-2ubuntu0.1`

Binary Packages:

- `libgif7:amd64=5.1.4-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libgif7/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris giflib=5.1.4-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/giflib/giflib_5.1.4-2ubuntu0.1.dsc' giflib_5.1.4-2ubuntu0.1.dsc 2018 SHA512:d905863f9b7f0e61ab9ec56ddd46a1ac48fb3feb52cd1c0ba3b312b8b4473b60babf9c0b7fdc843463660c4440c99866162c46346d432a99bfc918d1a2a7d3f2
'http://archive.ubuntu.com/ubuntu/pool/main/g/giflib/giflib_5.1.4.orig.tar.bz2' giflib_5.1.4.orig.tar.bz2 639703 SHA512:32b5e342056c210e6478e9cb3b6ceec9594dcfaf34feea1eb4dad633a081ed4465bceee578c19165907cb47cb83912ac359ceea666a8e07dbbb5420f9928f96d
'http://archive.ubuntu.com/ubuntu/pool/main/g/giflib/giflib_5.1.4-2ubuntu0.1.debian.tar.xz' giflib_5.1.4-2ubuntu0.1.debian.tar.xz 8768 SHA512:e1dc47d73443a9d436482b8945e9f35012f6de278976bdee125d7fd4baa54dcd3c5ee3643e9a1052cfa871917ee5047b22610f4336d8643958ba1e849dfe7b9e
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib-networking/glib-networking_2.56.0-1ubuntu0.1.dsc' glib-networking_2.56.0-1ubuntu0.1.dsc 2320 SHA512:122efa3abe0fa2c29dc767ececd7579767007ffcacdbc18d1f16d2d29a2eca1e948eeeb00388f99618af4e3d7284e30c24707b82b2c7f50aedff8981014e3d57
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib-networking/glib-networking_2.56.0.orig.tar.xz' glib-networking_2.56.0.orig.tar.xz 163852 SHA512:7c34817fa08e29c1d75e253a223d7beda0f38feb731d0a4219b10a220b664974f8f51ea693b93c7ebaa77ebd5e629fcaa5a52da5092513613f6b5faf5e9a21db
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib-networking/glib-networking_2.56.0-1ubuntu0.1.debian.tar.xz' glib-networking_2.56.0-1ubuntu0.1.debian.tar.xz 31224 SHA512:da8f8169d2eb29abb568a4005e1d912c621e87ce19ffb3e88ef5aae9975ae2b05252106533a2823322d3550be3a8cf217cb888a1718de7d7556a930b03dfe16f
```

### `dpkg` source package: `glib2.0=2.56.4-0ubuntu0.18.04.6`

Binary Packages:

- `libglib2.0-0:amd64=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-data=2.56.4-0ubuntu0.18.04.6`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-data/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.56.4-0ubuntu0.18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.dsc' glib2.0_2.56.4-0ubuntu0.18.04.6.dsc 3301 SHA512:aaa2f39144ca99225e255627f292d598d3d58ebffcbbcd2d7685a4993f342273d6b301b6b5f26651944d22b41e563e681d5daf23d1a6cf5fb74b39237132ebad
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4.orig.tar.xz' glib2.0_2.56.4.orig.tar.xz 7029768 SHA512:280a46c2af13283a08c15ff0b4f5492659c2884521930600ad45310ed181c44a878ad8f9b36bae68ed6e7d92db6f1630f7bf015148c513dc317d25807f13abb0
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz' glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz 89540 SHA512:ac9961d3070de87950006fc67a455fbb9b48172389b86097ee2038a7cbd89bc1ea9a4149b86c66816f489dac29dbbd4a7a020d3f6ee4b9b112185b3322e197c2
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
'http://security.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.2.dsc' glibc_2.27-3ubuntu1.2.dsc 9364 SHA512:3c04622e913a85fe8d32a65a14114310aad0df92c848ac00ecea6ad99cc3d4ebb5efd40c562cad0684151edc2348bc229a469662c55f19731d82971295f5cea8
'http://security.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27.orig.tar.xz' glibc_2.27.orig.tar.xz 15923832 SHA512:a0580fb52bc4ea8bb6e6734086b0dc66bd661060cdd837965880b989866490063c2420f250fb19b54e3547c58a5a7f8e012699e6513ce413746fd236ddd239e8
'http://security.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.2.debian.tar.xz' glibc_2.27-3ubuntu1.2.debian.tar.xz 1014508 SHA512:0013d939c1c8be3b5a06fb71e710b7912a475c178e8daff27ece31b8cfb3fbab586f09da22a506a28d4af6aadc6ca8953b6acd1272c2a9010f38d400eec24358
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.dsc' gnutls28_3.5.18-1ubuntu1.4.dsc 2780 SHA512:e8a0d6c2b9ba082f3019e6d287d0734dd26b2f5bd624b6a7a80d46c62a146fff2663124ed3f722d9acd694bd7044fc902bccbd7f7cadff4a0b2aa25fdf272bfd
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz' gnutls28_3.5.18.orig.tar.xz 7261980 SHA512:434cf33a4221fe2edce1b531cb53690d14a0991cb2056006021f625fb018987351f8ec917c3a7803e5e64179cf1647a3002ae783736ffca3188d2d294b76df52
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz.asc' gnutls28_3.5.18.orig.tar.xz.asc 534 SHA512:c5716fed2d87b88690194cef3aa6ad6674162c77ea6bd536dcff7c32dafe66304d4d2d8cefecf9ee709cf0fae8dae40e9e71dc2c69fd55abf8a15fb6cee52950
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz' gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz 83784 SHA512:807eb86a8c91caf999fc6ffe98b522d44926792d0252a18f220052455c7e4c1b321c03c6e2be355cc87b19ec34abb6206ea2af5cd147ad7d2a5b4e541c0c2339
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0-1ubuntu2.dsc' gpgme1.0_1.10.0-1ubuntu2.dsc 3046 SHA512:c3271bad11945eb4edbc6775bb5f2b9c4f625faaa0a5caeb6babb8d9b6150c7fccc452a6c84dc5ba1cc7d5ed0ac4a27af08ff02336215eb70ff8193bacb0b461
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0.orig.tar.bz2' gpgme1.0_1.10.0.orig.tar.bz2 1370162 SHA512:8ffa348ef4775ed3209486444d54411e28c9a0ff1d7a4315feb0b2856ccd5d110b219100ea41262ca0016af69a1936d79fee0eadf2599c7c5bbeed05d11f7ab5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0.orig.tar.bz2.asc' gpgme1.0_1.10.0.orig.tar.bz2.asc 534 SHA512:5a2f7b2e1109bbe71719ad3bb2a0e30e0dae220ed0223a98debb6a0eb8c6ca6e6fd42d3ddd714e253754b41b7321e711c58188e25db248d20bb96d99cbf86136
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.10.0-1ubuntu2.debian.tar.xz' gpgme1.0_1.10.0-1ubuntu2.debian.tar.xz 18372 SHA512:9c412f0adbf98b97561c4915dba70ba772c9ab299d25c402dab78645e8ebc5c5db6655ecd215b8303c94db71742bf96585b6dc31b5a6864624b62cb3ed0a397f
```

### `dpkg` source package: `gpm=1.20.7-5`

Binary Packages:

- `libgpm2:amd64=1.20.7-5`

Licenses: (parsed from: `/usr/share/doc/libgpm2/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0+`

Source:

```console
$ apt-get source -qq --print-uris gpm=1.20.7-5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpm/gpm_1.20.7-5.dsc' gpm_1.20.7-5.dsc 1986 SHA256:d5925ddcecd217ece2790c1c81993c6e32d86914865d90cb9bfabbe1bb6595a8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpm/gpm_1.20.7.orig.tar.gz' gpm_1.20.7.orig.tar.gz 855027 SHA256:c7e4661c24e05ae13547176b649bac8e3a0db2575f7dd57559f9e0b509f90f49
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpm/gpm_1.20.7-5.debian.tar.xz' gpm_1.20.7-5.debian.tar.xz 82740 SHA256:4adbf1434c4975cffe8ce7b180a1bf7047d79b0e4f0e1a8bf68297170df6fdf0
```

### `dpkg` source package: `graphene=1.8.0-1`

Binary Packages:

- `libgraphene-1.0-0:amd64=1.8.0-1`

Licenses: (parsed from: `/usr/share/doc/libgraphene-1.0-0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris graphene=1.8.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphene/graphene_1.8.0-1.dsc' graphene_1.8.0-1.dsc 2449 SHA256:eb292b987ae998a1de98f9fad0610adf97bab758aa234357f4d2f11c284433d6
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphene/graphene_1.8.0.orig.tar.gz' graphene_1.8.0.orig.tar.gz 157279 SHA256:410f2e848952cc5830f39b6f6ea7f9b0a487cfe99dad86eec6f22ccbb3ec635b
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphene/graphene_1.8.0-1.debian.tar.xz' graphene_1.8.0-1.debian.tar.xz 4872 SHA256:4b190645a7d78984e32581c0003283dce6d62bab91e72b8c39495b545f0b25f7
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.dsc' grep_3.1-2build1.dsc 2116 SHA512:420de2689ce397d7ae7cfa80bb3f2285445325269f649c387cd265770ba8ea6c0d7a87b5f40d86f88959f807ed77a5dffd6ebf2abdddf05c5c5653df3c6a1232
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1.orig.tar.xz' grep_3.1.orig.tar.xz 1370880 SHA512:05494381c7dd8aad7e2ee4c17450de8d7b969a99dcfe17747db60df3475bf02d5323d091e896e8343e4f3251c29dc7f0b7a9f93c575c9d58ee2a57014c2c9d26
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.debian.tar.bz2' grep_3.1-2build1.debian.tar.bz2 110087 SHA512:ca29a8001c406a2914a9edc1859f2615abc08dc1c8c8a42e48036844ee6249436dba7a43f5e5c078cb44605d620cd0d93904c92178acf73b42cb6faf416be310
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

### `dpkg` source package: `gsfonts=1:8.11+urwcyr1.0.7~pre44-4.4`

Binary Packages:

- `gsfonts=1:8.11+urwcyr1.0.7~pre44-4.4`

Licenses: (parsed from: `/usr/share/doc/gsfonts/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gsfonts=1:8.11+urwcyr1.0.7~pre44-4.4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsfonts/gsfonts_8.11+urwcyr1.0.7~pre44-4.4.dsc' gsfonts_8.11+urwcyr1.0.7~pre44-4.4.dsc 2011 SHA256:c532a13a9ca87a19d5e1470e94bf9fe7b822c0c1745d8f758f993d2ed4b2c329
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsfonts/gsfonts_8.11+urwcyr1.0.7~pre44.orig.tar.gz' gsfonts_8.11+urwcyr1.0.7~pre44.orig.tar.gz 3390551 SHA256:9f2a598998bf05e023546ac981aa2a857aa1635d2e0e3020a3c3004ad564dc00
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsfonts/gsfonts_8.11+urwcyr1.0.7~pre44-4.4.diff.gz' gsfonts_8.11+urwcyr1.0.7~pre44-4.4.diff.gz 6940 SHA256:b3343e4a90dbf5c7bb59df4a335f76d7877e2e6814d3f68f9988343f227db626
```

### `dpkg` source package: `gst-plugins-base1.0=1.14.5-0ubuntu1~18.04.1`

Binary Packages:

- `gstreamer1.0-gl:amd64=1.14.5-0ubuntu1~18.04.1`
- `gstreamer1.0-plugins-base:amd64=1.14.5-0ubuntu1~18.04.1`
- `libgstreamer-gl1.0-0:amd64=1.14.5-0ubuntu1~18.04.1`
- `libgstreamer-plugins-base1.0-0:amd64=1.14.5-0ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/gstreamer1.0-gl/copyright`, `/usr/share/doc/gstreamer1.0-plugins-base/copyright`, `/usr/share/doc/libgstreamer-gl1.0-0/copyright`, `/usr/share/doc/libgstreamer-plugins-base1.0-0/copyright`)

- `BSD (2 clause)`
- `BSD (3 clause)`
- `GPL-2+`
- `LGPL`
- `LGPL-2+`
- `MIT/X11 (BSD like) LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gst-plugins-base1.0=1.14.5-0ubuntu1~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.dsc' gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.dsc 4444 SHA512:d11c52150adf30b38849b53ee3b89bfa2d3ee3e778f2ece4ad0efef7fc7b5d7038879dbf9882d4b4c28e5b642645d5eb05864846d464b65081f0befd6cf7b824
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.5.orig.tar.xz' gst-plugins-base1.0_1.14.5.orig.tar.xz 3717076 SHA512:4e81c44a5ea3b910f96d3e9251ba38a79feacead4f96adb92eab5a650695ca8d5313e3ec1df78fec04376cf3152d2eefd4d39f6c11dadc98a11e55bbf8c8ccdc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-base1.0/gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz' gst-plugins-base1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz 45600 SHA512:39965114cc67b782820a77bc3981c38d6b6d417446feeed534c5744a0f1f1885ccde90745076218314e3232ffc9e39eda31f02f96eb04a88b54c6c9c37a0b028
```

### `dpkg` source package: `gst-plugins-good1.0=1.14.5-0ubuntu1~18.04.1`

Binary Packages:

- `gstreamer1.0-gtk3:amd64=1.14.5-0ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/gstreamer1.0-gtk3/copyright`)

- `BSD`
- `BSD (3 clause)`
- `GPL-2+`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1+`
- `MIT/X11 (BSD like) LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gst-plugins-good1.0=1.14.5-0ubuntu1~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-good1.0/gst-plugins-good1.0_1.14.5-0ubuntu1~18.04.1.dsc' gst-plugins-good1.0_1.14.5-0ubuntu1~18.04.1.dsc 4186 SHA512:c185511af0d57ed46bc4b7a5645d32edda85469508ff2be1470a16bafac7646f793c45ab90bbc9ac9a95ee586cff367c31a3a7e257cc3e2d1fa09e69d42b637d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-good1.0/gst-plugins-good1.0_1.14.5.orig.tar.xz' gst-plugins-good1.0_1.14.5.orig.tar.xz 3800104 SHA512:11bfadaf39b28a0a6a6c87c4ade8513496e8f13873cb0c2ddc8b8241029b8775d4839f2de441bda664bc67c66c4ca1d6839dd7570f7d79c1f485d5a25cc9d236
'http://archive.ubuntu.com/ubuntu/pool/main/g/gst-plugins-good1.0/gst-plugins-good1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz' gst-plugins-good1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz 124880 SHA512:d11c3af40c3c7620b3578a24e2c7adfbeb31c503f2b8e19f7f10ca9c21a48fb0c3c0af4216a308e40a5f8cc67045a84ce2af03169f88872db75b6527d88febd0
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.5-0ubuntu1~18.04.1.dsc' gstreamer1.0_1.14.5-0ubuntu1~18.04.1.dsc 3052 SHA512:7bbbb065d0704d9fb101ff278a869acc2f10cbe5e83705e5bf7e9b1694d57d833fb4f5130e91f402489354eb7b434540a295a4f2df9493c470a5e68822550f05
'http://archive.ubuntu.com/ubuntu/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.5.orig.tar.xz' gstreamer1.0_1.14.5.orig.tar.xz 3268756 SHA512:1a97ae17f8fff041db5e24d712d33c7116e408be1fabc2abd7b652b067b6ebe6c0943845a33a21335a5b4fa0a1ba178873158659f761f1e3aab04a969029c5d8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gstreamer1.0/gstreamer1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz' gstreamer1.0_1.14.5-0ubuntu1~18.04.1.debian.tar.xz 44584 SHA512:166409aa8b89d35ce695aa7c01ce43824680882cc9d16c74d0468d13e6fffdc279400cbcec7e850034053d2d848a60f32ce3c88ddd9c1d85dc7949a9179b94c1
```

### `dpkg` source package: `gtk+2.0=2.24.32-1ubuntu1`

Binary Packages:

- `libgail-common:amd64=2.24.32-1ubuntu1`
- `libgail18:amd64=2.24.32-1ubuntu1`
- `libgtk2.0-0:amd64=2.24.32-1ubuntu1`
- `libgtk2.0-bin=2.24.32-1ubuntu1`
- `libgtk2.0-common=2.24.32-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgail-common/copyright`, `/usr/share/doc/libgail18/copyright`, `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-bin/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

- `LGPL-2`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+2.0=2.24.32-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.32-1ubuntu1.dsc' gtk+2.0_2.24.32-1ubuntu1.dsc 3887 SHA256:a5ffdb0811ce5b1cbb4c4c1920ae38ee03fc7fffe4e7be9e8c0bd8826dce2778
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.32.orig.tar.xz' gtk+2.0_2.24.32.orig.tar.xz 12620860 SHA256:b6c8a93ddda5eabe3bfee1eb39636c9a03d2a56c7b62828b359bf197943c582e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.32-1ubuntu1.debian.tar.xz' gtk+2.0_2.24.32-1ubuntu1.debian.tar.xz 103116 SHA256:da2adb218e807207a574d47ca4797b02e9f821d11b4aa24af0de83ab43f0a09d
```

### `dpkg` source package: `gtk+3.0=3.22.30-1ubuntu4`

Binary Packages:

- `gtk-update-icon-cache=3.22.30-1ubuntu4`
- `libgtk-3-0:amd64=3.22.30-1ubuntu4`
- `libgtk-3-bin=3.22.30-1ubuntu4`
- `libgtk-3-common=3.22.30-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/gtk-update-icon-cache/copyright`, `/usr/share/doc/libgtk-3-0/copyright`, `/usr/share/doc/libgtk-3-bin/copyright`, `/usr/share/doc/libgtk-3-common/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+3.0/gtk+3.0_3.22.30-1ubuntu4.dsc' gtk+3.0_3.22.30-1ubuntu4.dsc 3364 SHA512:10f32b31fd76aee3bf0e3e64c4d23cfd621abaea21bf6e73cd9bdef5c280df88675be1ffa2166af5a532bb726284e4db45ab97f119645c0363eca94e34ff7151
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+3.0/gtk+3.0_3.22.30.orig.tar.xz' gtk+3.0_3.22.30.orig.tar.xz 18946084 SHA512:31440a615cb2f406d0f904e59febb8f876106f27818ddd6951c76ab9bcb421ca480dae2bebfb1c4b1e03b833fc7c42e9feede053d9d71f19a02fe778e3197b38
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+3.0/gtk+3.0_3.22.30-1ubuntu4.debian.tar.xz' gtk+3.0_3.22.30-1ubuntu4.debian.tar.xz 162544 SHA512:8a3de916027748f1e9f013fd955a83ac568187cd7b52d1972bfd0dd753e860d5c2e89f91c294779a6d5f4f15066bed59084f508274493ea1944570fae341bd21
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

### `dpkg` source package: `hsqldb1.8.0=1.8.0.10+dfsg-10~18.04`

Binary Packages:

- `libhsqldb1.8.0-java=1.8.0.10+dfsg-10~18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris hsqldb1.8.0=1.8.0.10+dfsg-10~18.04
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hsqldb1.8.0/hsqldb1.8.0_1.8.0.10+dfsg-10~18.04.dsc' hsqldb1.8.0_1.8.0.10+dfsg-10~18.04.dsc 1970 SHA512:b2f3c2bf501b2b8f1279a8bac77d638b53657be277239a2f50de0e9086272a5a512f6d3075086773228ca0c49a3525ae58e12d4438332cec73b64ddb62e6a6d2
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hsqldb1.8.0/hsqldb1.8.0_1.8.0.10+dfsg.orig.tar.gz' hsqldb1.8.0_1.8.0.10+dfsg.orig.tar.gz 2917677 SHA512:95a059478c71d55cc28e77154e7e0ac3ac4796936f50558b2e9f29f9325f284117be930aa028eac08078a2bcc59a01c9898b23f4e1af4e38879b91021bd052a2
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hsqldb1.8.0/hsqldb1.8.0_1.8.0.10+dfsg-10~18.04.diff.gz' hsqldb1.8.0_1.8.0.10+dfsg-10~18.04.diff.gz 29681 SHA512:c1a58c9294a11106a7bf35ba3b6295fba972a0bcd0f5c200389078d4be19f949bb44c76d9fdaea3848bde3bab120ab5917b447c70dcc11f4d581568667bfa953
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
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.dsc' icu_60.2-3ubuntu3.1.dsc 2149 SHA512:dc8e59c858c31923068bae1982c390bc5175bcc3fd01510d777fb964a795e327ae350db4bb3929c6dfb68ddebb54227fc7f48ab645b880691b82f52e96993193
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2.orig.tar.gz' icu_60.2.orig.tar.gz 23315541 SHA512:ecbd9eea199d261d5f2b262abab6b1f3ee4e993081faca1426046b4ed2eadbb082fca3ebdeff82f6b431eafa7ddbe764fe64f9d96bf96486d1aa51cdc4c3d8b2
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.debian.tar.xz' icu_60.2-3ubuntu3.1.debian.tar.xz 29068 SHA512:cc5504e882078d5acc217d948d5ce31609e41f08dd20ea73cff1e1e775571710971d51f4d010d273c63b8068eb0edbf2657b9454fa0cb9628bcac1484ce7a762
```

### `dpkg` source package: `ijs=0.35-13`

Binary Packages:

- `libijs-0.35:amd64=0.35-13`

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
$ apt-get source -qq --print-uris ijs=0.35-13
'http://archive.ubuntu.com/ubuntu/pool/main/i/ijs/ijs_0.35-13.dsc' ijs_0.35-13.dsc 2031 SHA256:fbba574e7da557739a5628ddb94c9d954c537b418e3cf6488bdd3badc6100859
'http://archive.ubuntu.com/ubuntu/pool/main/i/ijs/ijs_0.35.orig.tar.gz' ijs_0.35.orig.tar.gz 344262 SHA256:901fffb73e42dae343a8285a31d9c4e82dc3856d36be30adbdb564bdd27161d6
'http://archive.ubuntu.com/ubuntu/pool/main/i/ijs/ijs_0.35-13.debian.tar.xz' ijs_0.35-13.debian.tar.xz 8572 SHA256:53465d3c6fdbf0e6e7dce0b32c1c9b37a94173be91d0af40c238b2dc22384ac0
```

### `dpkg` source package: `ilmbase=2.2.0-11ubuntu2`

Binary Packages:

- `libilmbase12:amd64=2.2.0-11ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libilmbase12/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.2.0-11ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.0-11ubuntu2.dsc' ilmbase_2.2.0-11ubuntu2.dsc 2099 SHA256:894cddbe71ecaa8be9d1a348962270882dbe6c339f65e6b702db2fa07d4c9c2d
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.0.orig.tar.gz' ilmbase_2.2.0.orig.tar.gz 525289 SHA256:ecf815b60695555c1fbc73679e84c7c9902f4e8faa6e8000d2f905b8b86cedc7
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.0-11ubuntu2.debian.tar.xz' ilmbase_2.2.0-11ubuntu2.debian.tar.xz 13400 SHA256:400b77a32f7a04d78ff0462f32dc1e4073f5e1225ed070c63fa6a0ec619905c5
```

### `dpkg` source package: `imagemagick=8:6.9.7.4+dfsg-16ubuntu6.8`

Binary Packages:

- `imagemagick=8:6.9.7.4+dfsg-16ubuntu6.8`
- `imagemagick-6-common=8:6.9.7.4+dfsg-16ubuntu6.8`
- `imagemagick-6.q16=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-6.q16-3:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-6.q16-3-extra:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickwand-6.q16-3:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/libmagickcore-6.q16-3/copyright`, `/usr/share/doc/libmagickcore-6.q16-3-extra/copyright`, `/usr/share/doc/libmagickwand-6.q16-3/copyright`)

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.7.4+dfsg-16ubuntu6.8
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg-16ubuntu6.8.dsc' imagemagick_6.9.7.4+dfsg-16ubuntu6.8.dsc 5234 SHA512:08ac01966c6c0537abac4af44a14920e7d60d3299479e5b217d7caa4e991459a5984389ffa216bf44a3f5e2f01aa1e3909aeef0cce72134eb08b25f112bdc8f6
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg.orig.tar.xz' imagemagick_6.9.7.4+dfsg.orig.tar.xz 8929800 SHA512:c1696b80cb95f00c32079110b84df9a125730f336cca5c04caf4aeb4b2f48ba8014dfd808b8a5cef221d5be4da4ffa1472548aa6885c5f756f04db64baf6fbd3
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg-16ubuntu6.8.debian.tar.xz' imagemagick_6.9.7.4+dfsg-16ubuntu6.8.debian.tar.xz 303304 SHA512:ff3558d6e8fe5e965d2f89765b2b33a6b9ef4c43ad560540137df5322e7f66781fb7073116510df3ff45c4a2bbbb9e258968a4a15c5b4823e9bc4bb09db79baa
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

### `dpkg` source package: `intel-vaapi-driver=2.1.0-0ubuntu1`

Binary Packages:

- `i965-va-driver:amd64=2.1.0-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/i965-va-driver/copyright`)

- `Apache-2.0`
- `EPL-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris intel-vaapi-driver=2.1.0-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/intel-vaapi-driver/intel-vaapi-driver_2.1.0-0ubuntu1.dsc' intel-vaapi-driver_2.1.0-0ubuntu1.dsc 2483 SHA256:7cdb07c5b4427faddfa80c029caf85e1f67fa7ca09667a683279b1ca8e98aef9
'http://archive.ubuntu.com/ubuntu/pool/universe/i/intel-vaapi-driver/intel-vaapi-driver_2.1.0.orig.tar.bz2' intel-vaapi-driver_2.1.0.orig.tar.bz2 2889076 SHA256:ecfaf2ccc4b9af7340e002d2ef807d1e33051d4992f1983f5f4d60e516f86bdf
'http://archive.ubuntu.com/ubuntu/pool/universe/i/intel-vaapi-driver/intel-vaapi-driver_2.1.0-0ubuntu1.debian.tar.xz' intel-vaapi-driver_2.1.0-0ubuntu1.debian.tar.xz 10020 SHA256:d072e27cb9134eb76c3162fdc091daf3182049bab19aebce6c6c25f41b50c7d3
```

### `dpkg` source package: `isl=0.19-1`

Binary Packages:

- `libisl19:amd64=0.19-1`

Licenses: (parsed from: `/usr/share/doc/libisl19/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.19-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19-1.dsc' isl_0.19-1.dsc 1833 SHA256:f9786677430e2ea7295c6ad9480e7e710582f84b5b850a5ddfe1f21b3d726b0f
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19.orig.tar.xz' isl_0.19.orig.tar.xz 1515156 SHA256:6d6c1aa00e2a6dfc509fa46d9a9dbe93af0c451e196a670577a148feecf6b8a5
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19-1.debian.tar.xz' isl_0.19-1.debian.tar.xz 22388 SHA256:aa034a5700c63867aae836a1f985fccc50ccacd1abe57a2a016e076fa745feb0
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
'http://archive.ubuntu.com/ubuntu/pool/main/j/jackd2/jackd2_1.9.12~dfsg-2.dsc' jackd2_1.9.12~dfsg-2.dsc 2521 SHA256:7378eb1f223f0b69b8698f4a09e59c7f26632c1f2dec0452a76ea80ca5798d9a
'http://archive.ubuntu.com/ubuntu/pool/main/j/jackd2/jackd2_1.9.12~dfsg.orig.tar.gz' jackd2_1.9.12~dfsg.orig.tar.gz 1147874 SHA256:059741090d548d1888d34c90647e3ac1650bbee84990dceffcb5144b8f8cd539
'http://archive.ubuntu.com/ubuntu/pool/main/j/jackd2/jackd2_1.9.12~dfsg-2.debian.tar.xz' jackd2_1.9.12~dfsg-2.debian.tar.xz 44324 SHA256:59904fbdc98a3404bd5f21af13bd24977d2e5b03600f2bb0a84127a1bc69aeb9
```

### `dpkg` source package: `java-atk-wrapper=0.33.3-20ubuntu0.1`

Binary Packages:

- `libatk-wrapper-java=0.33.3-20ubuntu0.1`
- `libatk-wrapper-java-jni:amd64=0.33.3-20ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libatk-wrapper-java/copyright`, `/usr/share/doc/libatk-wrapper-java-jni/copyright`)

- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris java-atk-wrapper=0.33.3-20ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/j/java-atk-wrapper/java-atk-wrapper_0.33.3-20ubuntu0.1.dsc' java-atk-wrapper_0.33.3-20ubuntu0.1.dsc 2535 SHA256:83444322690a0d20b34b440dc20e38739a99ac999439d181dabf1d5fe859e37a
'http://archive.ubuntu.com/ubuntu/pool/main/j/java-atk-wrapper/java-atk-wrapper_0.33.3.orig.tar.gz' java-atk-wrapper_0.33.3.orig.tar.gz 73989 SHA256:2ad3bbaa4c2c28348c0433f06f7f3a621f7607d7f3cc8b2dab2a5fe23d2a97bc
'http://archive.ubuntu.com/ubuntu/pool/main/j/java-atk-wrapper/java-atk-wrapper_0.33.3-20ubuntu0.1.debian.tar.bz2' java-atk-wrapper_0.33.3-20ubuntu0.1.debian.tar.bz2 21438 SHA256:9b7eae81b6f21e454e63708f3dea0df95ed5d3aaef484925a84f78c093d8d416
```

### `dpkg` source package: `java-common=0.68ubuntu1~18.04.1`

Binary Packages:

- `default-jre=2:1.11-68ubuntu1~18.04.1`
- `default-jre-headless=2:1.11-68ubuntu1~18.04.1`
- `java-common=0.68ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/default-jre/copyright`, `/usr/share/doc/default-jre-headless/copyright`, `/usr/share/doc/java-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris java-common=0.68ubuntu1~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/j/java-common/java-common_0.68ubuntu1~18.04.1.dsc' java-common_0.68ubuntu1~18.04.1.dsc 2132 SHA512:fd566b2999a4cfdd9b7d6969cfaac88bc844d994fc679138b357355c213c5e0e8e76caafdfed8057edc202d328e82c4308df8025fbbf8cb5982838d24725857c
'http://archive.ubuntu.com/ubuntu/pool/main/j/java-common/java-common_0.68ubuntu1~18.04.1.tar.xz' java-common_0.68ubuntu1~18.04.1.tar.xz 13192 SHA512:27dda03798c06681385d568b87aa36ede3177cff2c95d493a297d5d309d770c422d99aac49f2f33327446ad121a6a3728fb51357e1d2ebd32c275bf104a16f63
```

### `dpkg` source package: `jbig2dec=0.13-6`

Binary Packages:

- `libjbig2dec0:amd64=0.13-6`

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
$ apt-get source -qq --print-uris jbig2dec=0.13-6
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbig2dec/jbig2dec_0.13-6.dsc' jbig2dec_0.13-6.dsc 1924 SHA256:559718685028f92875e4b4ecd26dd74dad4ac1a3efc5115f13a943b2e5019e33
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbig2dec/jbig2dec_0.13.orig.tar.gz' jbig2dec_0.13.orig.tar.gz 122387 SHA256:c8b13b78d4bfd85df088943370cf93768e19c6f5dfe74178d7088e54b6db4ffb
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbig2dec/jbig2dec_0.13-6.debian.tar.xz' jbig2dec_0.13-6.debian.tar.xz 30752 SHA256:bdf6e7483039a99ee8c6d28e5f0f8f3deb2ef6737056d50ecb30ce89ae7da472
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
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-glib/json-glib_1.4.2-3ubuntu0.18.04.1.dsc' json-glib_1.4.2-3ubuntu0.18.04.1.dsc 2112 SHA512:811a99183b511bb514818f3ff3237fc74d7a9cdcca85a6f208d2c223b8fe0d3d58ffc8bbc1ed3b46daab0afb3d2babd89b1846e8d593593394b73316293f1f45
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-glib/json-glib_1.4.2.orig.tar.xz' json-glib_1.4.2.orig.tar.xz 148404 SHA512:0e64e7eaf24629008290e04b0e0ec5f78852927841c0f6f9a8e62a92eeacbac36cca40ddd037cf299e3836cc38b3799f41b64b20a8fc37871b5f57c4da335339
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-glib/json-glib_1.4.2-3ubuntu0.18.04.1.debian.tar.xz' json-glib_1.4.2-3ubuntu0.18.04.1.debian.tar.xz 9072 SHA512:73fd58268df202ebe37088e038a6910b754189ae4fe8642511562e2d25794c75ab5261eddbdc5aac99a5ff5fbc435d2a4b83687582f3f951f1ffb5d82d468cad
```

### `dpkg` source package: `jsp-api=2.3.4-2~18.04`

Binary Packages:

- `libjsp-api-java=2.3.4-2~18.04`

Licenses: (parsed from: `/usr/share/doc/libjsp-api-java/copyright`)

- `Apache-2.0`
- `CDDL-1.1`
- `GPL-2`
- `GPL-2 with Classpath exception`

Source:

```console
$ apt-get source -qq --print-uris jsp-api=2.3.4-2~18.04
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jsp-api/jsp-api_2.3.4-2~18.04.dsc' jsp-api_2.3.4-2~18.04.dsc 2089 SHA512:e5ffecd18901aa7c75ab84fe2adb90a6420dce9e5aa9897e425aeacec78bb8b4430d9d09f486ba330f83e9f16f17f7d1b884284e3946837d32e73ede6316a3a1
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jsp-api/jsp-api_2.3.4.orig.tar.xz' jsp-api_2.3.4.orig.tar.xz 85592 SHA512:79f74b0a9fcc7075fa88a70146064348bed118df98e33c0295934471c7efdfbb011a295b56fa391f1031a858c97b89569a24ea33dc7b17daabdc09c88b287912
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jsp-api/jsp-api_2.3.4-2~18.04.debian.tar.xz' jsp-api_2.3.4-2~18.04.debian.tar.xz 8628 SHA512:81be902543b5f25b18c568a82340ee05a946c2110ff6971f947a06500f1dc63d5a8f32c64b03b062ac1afea29fc4b6aca48ab05fb598e2583a7cb8f443b6f877
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

- `krb5-locales=1.16-2ubuntu0.1`
- `libgssapi-krb5-2:amd64=1.16-2ubuntu0.1`
- `libk5crypto3:amd64=1.16-2ubuntu0.1`
- `libkrb5-3:amd64=1.16-2ubuntu0.1`
- `libkrb5support0:amd64=1.16-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/krb5-locales/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.16-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.1.dsc' krb5_1.16-2ubuntu0.1.dsc 3563 SHA512:a73ea88dc4ac0583330fa93a790def3ae57b201b148995f48f301cddd0975dcbfe54ac099e9dacf6dfe089e177819865c652328d49af98c742d683a62a3a4946
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16.orig.tar.gz' krb5_1.16.orig.tar.gz 9474479 SHA512:7e162467b95dad2b6aaa11686d08a00f1cc4eb08247fca8f0e5a8bcaa5f9f7b42cdf00db69c5c6111bdf9eb8063d53cef3bb207ce5d6a287615ca10b710153f9
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.1.debian.tar.xz' krb5_1.16-2ubuntu0.1.debian.tar.xz 99820 SHA512:80836484a0405bc271e21a04c12547a840a360276bfb30ae1fcb648e9ed67232bfad92c60614463acbe61701c58e72b49ffc892bcf00924c4dbdfac88a59f36c
```

### `dpkg` source package: `lame=3.100-2`

Binary Packages:

- `libmp3lame0:amd64=3.100-2`

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
'http://archive.ubuntu.com/ubuntu/pool/main/l/lame/lame_3.100-2.dsc' lame_3.100-2.dsc 2193 SHA256:23ead7cb4e1e0dd7925e67f935d005aa2ae73b508d240420e63d87b99c5a952e
'http://archive.ubuntu.com/ubuntu/pool/main/l/lame/lame_3.100.orig.tar.gz' lame_3.100.orig.tar.gz 1524133 SHA256:ddfe36cab873794038ae2c1210557ad34857a4b6bdc515785d1da9e175b1da1e
'http://archive.ubuntu.com/ubuntu/pool/main/l/lame/lame_3.100-2.debian.tar.xz' lame_3.100-2.debian.tar.xz 12152 SHA256:096925e4c15a9ee4e3f79451111b0ad11ea33a4ab9b74581e6f4775b7f1867e5
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
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-1ubuntu0.1.dsc' lcms2_2.9-1ubuntu0.1.dsc 2084 SHA512:191a120e26ea97428a29c1a8a9f67f6a087315245a40f7240e93e46fb174e953530010e81f35d041615b7b4c53fb9be266890cc007aef8700db0a35e37eb7735
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9.orig.tar.gz' lcms2_2.9.orig.tar.gz 10974649 SHA512:70b1c51fa8d137d5072425e580745ff1fbf49c6e8bb1da0a8adb0647d3b7c095208793cb02de1e8d1a01363b8575fa60c61bedbff99bbec57a44228239cb00e5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-1ubuntu0.1.debian.tar.xz' lcms2_2.9-1ubuntu0.1.debian.tar.xz 10680 SHA512:84285b89b9b3517d07d12aaefed7e1a343dcb5123538c3bd4cb9307fbf3913a54bfc2c9f022c72af28fe781a5db451ae25c1594c8e6133abcf3d6b36b66eedd6
```

### `dpkg` source package: `libaacs=0.9.0-1`

Binary Packages:

- `libaacs0:amd64=0.9.0-1`

Licenses: (parsed from: `/usr/share/doc/libaacs0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libaacs=0.9.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libaacs/libaacs_0.9.0-1.dsc' libaacs_0.9.0-1.dsc 2108 SHA256:d442a930e2fbd7710d3a197cbe27b211146694ce7ff63f9649571ecd6ebbdd74
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libaacs/libaacs_0.9.0.orig.tar.bz2' libaacs_0.9.0.orig.tar.bz2 316323 SHA256:47e0bdc9c9f0f6146ed7b4cc78ed1527a04a537012cf540cf5211e06a248bace
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libaacs/libaacs_0.9.0-1.debian.tar.xz' libaacs_0.9.0-1.debian.tar.xz 4056 SHA256:0e49a59f0366efe54b5aad9ddde2d4e99cecc009af9ef5df0fee8330ba6616bc
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

### `dpkg` source package: `libass=1:0.14.0-1`

Binary Packages:

- `libass9:amd64=1:0.14.0-1`

Licenses: (parsed from: `/usr/share/doc/libass9/copyright`)

- `GPL-2`
- `GPL-2+`
- `ISC`
- `other-1`

Source:

```console
$ apt-get source -qq --print-uris libass=1:0.14.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libass/libass_0.14.0-1.dsc' libass_0.14.0-1.dsc 2129 SHA256:8944e47c22ed168f80a70e347497173b80d498ec6536cf594a5a2b7011219a6d
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libass/libass_0.14.0.orig.tar.xz' libass_0.14.0.orig.tar.xz 356256 SHA256:881f2382af48aead75b7a0e02e65d88c5ebd369fe46bc77d9270a94aa8fd38a2
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libass/libass_0.14.0-1.debian.tar.xz' libass_0.14.0-1.debian.tar.xz 5700 SHA256:3ccc2c3bebe5f1917484f3ac6496801b0b4602dbe41efa22ef1cb372a2fc13ed
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

### `dpkg` source package: `libasyncns=0.8-6`

Binary Packages:

- `libasyncns0:amd64=0.8-6`

Licenses: (parsed from: `/usr/share/doc/libasyncns0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libasyncns=0.8-6
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libasyncns/libasyncns_0.8-6.dsc' libasyncns_0.8-6.dsc 1921 SHA256:d6a3cccafadceda0bd1542c6325c6238ec34a8ff85276d6f2e5914e282c67dc6
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libasyncns/libasyncns_0.8.orig.tar.gz' libasyncns_0.8.orig.tar.gz 341591 SHA256:4f1a66e746cbe54ff3c2fbada5843df4fbbbe7481d80be003e8d11161935ab74
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libasyncns/libasyncns_0.8-6.debian.tar.xz' libasyncns_0.8-6.debian.tar.xz 4564 SHA256:69b23a155b8a3da3bf68b1e440283e117c55e92bd3b4aa308605fe3f1164485e
```

### `dpkg` source package: `libauthen-sasl-perl=2.1600-1`

Binary Packages:

- `libauthen-sasl-perl=2.1600-1`

Licenses: (parsed from: `/usr/share/doc/libauthen-sasl-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libauthen-sasl-perl=2.1600-1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libauthen-sasl-perl/libauthen-sasl-perl_2.1600-1.dsc' libauthen-sasl-perl_2.1600-1.dsc 2313 SHA256:ddb85abf950c2e63d2403876f1dabb5c00c2390dc7e95e3b6124330c25ca02a2
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libauthen-sasl-perl/libauthen-sasl-perl_2.1600.orig.tar.gz' libauthen-sasl-perl_2.1600.orig.tar.gz 45129 SHA256:6614fa7518f094f853741b63c73f3627168c5d3aca89b1d02b1016dc32854e09
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libauthen-sasl-perl/libauthen-sasl-perl_2.1600-1.debian.tar.xz' libauthen-sasl-perl_2.1600-1.debian.tar.xz 3976 SHA256:edc85675ad2b6c97e4b6df5b4305d1f7afcd6b0af6407c3a4dea5ac58f9750e4
```

### `dpkg` source package: `libavc1394=0.5.4-4build1`

Binary Packages:

- `libavc1394-0:amd64=0.5.4-4build1`

Licenses: (parsed from: `/usr/share/doc/libavc1394-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libavc1394=0.5.4-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libavc1394/libavc1394_0.5.4-4build1.dsc' libavc1394_0.5.4-4build1.dsc 2299 SHA256:d0266351a9e045a7ee21ab414e959c97559bbb432980729a8b7fea11c744b168
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libavc1394/libavc1394_0.5.4.orig.tar.gz' libavc1394_0.5.4.orig.tar.gz 341679 SHA256:7cb1ff09506ae911ca9860bef4af08c2403f3e131f6c913a2cbd6ddca4215b53
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libavc1394/libavc1394_0.5.4-4build1.debian.tar.xz' libavc1394_0.5.4-4build1.debian.tar.xz 6644 SHA256:3b9855f03ca3192d029875d937328a8ea193f992a1d23bd140aa5f0d5477e007
```

### `dpkg` source package: `libbdplus=0.1.2-2`

Binary Packages:

- `libbdplus0:amd64=0.1.2-2`

Licenses: (parsed from: `/usr/share/doc/libbdplus0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libbdplus=0.1.2-2
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbdplus/libbdplus_0.1.2-2.dsc' libbdplus_0.1.2-2.dsc 2136 SHA256:67f250a4551033aa058e7f7872cbd9fbac59db1c00d6c8cb1d94f8172145637a
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbdplus/libbdplus_0.1.2.orig.tar.bz2' libbdplus_0.1.2.orig.tar.bz2 319828 SHA256:a631cae3cd34bf054db040b64edbfc8430936e762eb433b1789358ac3d3dc80a
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbdplus/libbdplus_0.1.2-2.debian.tar.xz' libbdplus_0.1.2-2.debian.tar.xz 2664 SHA256:77815244fa814aff849b5fcf9f012b18ae7ca062cbd95d40e748d42190d45e3e
```

### `dpkg` source package: `libbluray=1:1.0.2-3`

Binary Packages:

- `libbluray2:amd64=1:1.0.2-3`

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
$ apt-get source -qq --print-uris libbluray=1:1.0.2-3
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbluray/libbluray_1.0.2-3.dsc' libbluray_1.0.2-3.dsc 2528 SHA256:088ff7c4426cc6107d7afd928d4614b3e21ed718414ed0ef1d73c9a546f6b2e4
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbluray/libbluray_1.0.2.orig.tar.bz2' libbluray_1.0.2.orig.tar.bz2 733058 SHA256:6d9e7c4e416f664c330d9fa5a05ad79a3fb39b95adfc3fd6910cbed503b7aeff
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbluray/libbluray_1.0.2-3.debian.tar.xz' libbluray_1.0.2-3.debian.tar.xz 16812 SHA256:4e6e7320820e70bd7fe3d4d262b42138a8a166d44e29d9d9cf3fb6abcb029ce1
```

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
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbs2b/libbs2b_3.1.0+dfsg-2.2.dsc' libbs2b_3.1.0+dfsg-2.2.dsc 1939 SHA256:a5fa01cf653b4161bb8595509be5ee91d1f47b8a9ff2b8c98b7fdd60b290e643
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbs2b/libbs2b_3.1.0+dfsg.orig.tar.gz' libbs2b_3.1.0+dfsg.orig.tar.gz 330675 SHA256:c23faf614f787342c1a1a40f83064f2e5a49391733c029dc31d09fba759cee0a
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbs2b/libbs2b_3.1.0+dfsg-2.2.debian.tar.xz' libbs2b_3.1.0+dfsg-2.2.debian.tar.xz 4632 SHA256:37d7d8da3d0ab030ca49944e98c83b4ae8a4463d3a70c301af79da20e05b0440
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
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7-1ubuntu0.1.dsc' libbsd_0.8.7-1ubuntu0.1.dsc 2280 SHA512:a843bcd758e78f005d073a8ca8cfc2813b076851c4dccb307bf12d6870c3fc555e45e89e56d4160a630ae31d59e945f4d41170ac0a9ad9e72e021743b080ad7c
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7.orig.tar.xz' libbsd_0.8.7.orig.tar.xz 371772 SHA512:605a14eb5d33c0e45c3bd29e585ebc15832e2ed1efa9356291a0562622168da96db1a20766e9dae8910ea0c1516429f43905edc8d4f2a40a5a341a689d08fcc3
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7.orig.tar.xz.asc' libbsd_0.8.7.orig.tar.xz.asc 833 SHA512:05b65159a7fd4e256fe41df10f3cc389d84ade4e4a5a8786f8b1990951be10b33ec9fbc6cbea16ae0c44a490253511fb2cd6c23422e11e16dbf80bef7f3eb812
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7-1ubuntu0.1.debian.tar.xz' libbsd_0.8.7-1ubuntu0.1.debian.tar.xz 16608 SHA512:ac2c3278effcba412e732a60258c011b1e6bd0ae9ab28e434fb852df35950905293bba9e2d37466dd29b943763e7e186d3145e81c22f3879b5706f2890e62a17
```

### `dpkg` source package: `libcaca=0.99.beta19-2ubuntu0.18.04.1`

Binary Packages:

- `libcaca0:amd64=0.99.beta19-2ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libcaca0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcaca=0.99.beta19-2ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcaca/libcaca_0.99.beta19-2ubuntu0.18.04.1.dsc' libcaca_0.99.beta19-2ubuntu0.18.04.1.dsc 2339 SHA512:fd0f16b3991057b0201680094dc5ae02ea18ee5011245d04b051e067a74ef10fcbfe3d18500e58e7c5c0ca5aacdfad01bc0204654eeba12cb6850b2b762e006f
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcaca/libcaca_0.99.beta19.orig.tar.gz' libcaca_0.99.beta19.orig.tar.gz 1203495 SHA512:780fc7684d40207cc10df3f87d6d8f1d47ddfffa0e76e41a5ce671b82d5c7f090facb054c3d49ca7c4ea1a619625bb9085ce52f837f50792b4a2d776a4c68e15
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcaca/libcaca_0.99.beta19-2ubuntu0.18.04.1.debian.tar.xz' libcaca_0.99.beta19-2ubuntu0.18.04.1.debian.tar.xz 12708 SHA512:334ab2ca47267500a1000a81345036675f19c380d7d299d9a71674daa34652b94c118895088b0e471021d9410c3052611d8d1549b6303013a92127741ee417dc
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
- `libpam-cap:amd64=1:2.25-1.2`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`, `/usr/share/doc/libpam-cap/copyright`)

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

### `dpkg` source package: `libcdio-paranoia=10.2+0.94+2-2build1`

Binary Packages:

- `libcdio-cdda2:amd64=10.2+0.94+2-2build1`
- `libcdio-paranoia2:amd64=10.2+0.94+2-2build1`

Licenses: (parsed from: `/usr/share/doc/libcdio-cdda2/copyright`, `/usr/share/doc/libcdio-paranoia2/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libcdio-paranoia=10.2+0.94+2-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio-paranoia/libcdio-paranoia_10.2+0.94+2-2build1.dsc' libcdio-paranoia_10.2+0.94+2-2build1.dsc 2287 SHA256:dcdec7f773cae87bc54a242fc5ad8b1134973b728a10afb79e27d0c12451b21f
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio-paranoia/libcdio-paranoia_10.2+0.94+2.orig.tar.gz' libcdio-paranoia_10.2+0.94+2.orig.tar.gz 704560 SHA256:d60f82ece97eeb92407a9ee03f3499c8983206672c28ae5e4e22179063c81941
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio-paranoia/libcdio-paranoia_10.2+0.94+2-2build1.debian.tar.xz' libcdio-paranoia_10.2+0.94+2-2build1.debian.tar.xz 8044 SHA256:22d0b91598f80376cb026536380dd594fe8e22c4b3f53cc6551aba50eac59e19
```

### `dpkg` source package: `libcdio=1.0.0-2ubuntu2`

Binary Packages:

- `libcdio17:amd64=1.0.0-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libcdio17/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libcdio=1.0.0-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio/libcdio_1.0.0-2ubuntu2.dsc' libcdio_1.0.0-2ubuntu2.dsc 2298 SHA256:e5ba26fe1f3918897c926535c01189f176a9260f3b1fffff51c4589075acb19e
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio/libcdio_1.0.0.orig.tar.gz' libcdio_1.0.0.orig.tar.gz 2343992 SHA256:fe080bc3cb7a57becdecf2b392bf39c24df0211f5fdfddfe99748fa052a7e231
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio/libcdio_1.0.0-2ubuntu2.debian.tar.xz' libcdio_1.0.0-2ubuntu2.debian.tar.xz 12376 SHA256:b48ec937ddaa6cd188e9578dd39a231150e72bd41037450550b9e7140766e674
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

### `dpkg` source package: `libcommons-logging-java=1.2-2`

Binary Packages:

- `libcommons-logging-java=1.2-2`

Licenses: (parsed from: `/usr/share/doc/libcommons-logging-java/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libcommons-logging-java=1.2-2
'http://archive.ubuntu.com/ubuntu/pool/universe/libc/libcommons-logging-java/libcommons-logging-java_1.2-2.dsc' libcommons-logging-java_1.2-2.dsc 2416 SHA256:98de13c4e77e3cb89291b32d54aecdfbb6e27a6c74698a405da573bf5700b90e
'http://archive.ubuntu.com/ubuntu/pool/universe/libc/libcommons-logging-java/libcommons-logging-java_1.2.orig.tar.xz' libcommons-logging-java_1.2.orig.tar.xz 134940 SHA256:10dda2b5647087c3478083ab8bc5ef4bcb95d4515b4aed79dcc59b524072b3cd
'http://archive.ubuntu.com/ubuntu/pool/universe/libc/libcommons-logging-java/libcommons-logging-java_1.2-2.debian.tar.xz' libcommons-logging-java_1.2-2.debian.tar.xz 7764 SHA256:d76e48eebb08c6cbc3fb3fe8c1d357ae2f18d03b1c04c57d0a65d0349cc552cb
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

### `dpkg` source package: `libdata-dump-perl=1.23-1`

Binary Packages:

- `libdata-dump-perl=1.23-1`

Licenses: (parsed from: `/usr/share/doc/libdata-dump-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libdata-dump-perl=1.23-1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdata-dump-perl/libdata-dump-perl_1.23-1.dsc' libdata-dump-perl_1.23-1.dsc 2261 SHA256:5362c6e5f931eeac87ea8347c77bd08b2fc61919f8a1d3e0f93468dadeca8f53
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdata-dump-perl/libdata-dump-perl_1.23.orig.tar.gz' libdata-dump-perl_1.23.orig.tar.gz 20771 SHA256:af53b05ef1387b4cab4427e6789179283e4f0da8cf036e8db516ddb344512b65
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdata-dump-perl/libdata-dump-perl_1.23-1.debian.tar.xz' libdata-dump-perl_1.23-1.debian.tar.xz 3456 SHA256:8f4a0f41e4ca3c3bfd5b94585910ade663cfc32972e5a52d6bf031a26648a48e
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

### `dpkg` source package: `libdc1394-22=2.2.5-1`

Binary Packages:

- `libdc1394-22:amd64=2.2.5-1`

Licenses: (parsed from: `/usr/share/doc/libdc1394-22/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libdc1394-22=2.2.5-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libdc1394-22/libdc1394-22_2.2.5-1.dsc' libdc1394-22_2.2.5-1.dsc 2244 SHA256:210d37ef0e48144be2c46bb547d563ac1a67fa1ec8c893461100de8c971ad006
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libdc1394-22/libdc1394-22_2.2.5.orig.tar.gz' libdc1394-22_2.2.5.orig.tar.gz 611918 SHA256:350cc8d08aee5ffc4e1f3049e2e1c2bc6660642d424595157da97ab5b1263337
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libdc1394-22/libdc1394-22_2.2.5-1.debian.tar.xz' libdc1394-22_2.2.5-1.debian.tar.xz 8244 SHA256:895eeea4458059ae65a879a7d1c625508b854eb5f3d472192b94bd5ba281e316
```

### `dpkg` source package: `libdrm=2.4.101-2~18.04.1`

Binary Packages:

- `libdrm-amdgpu1:amd64=2.4.101-2~18.04.1`
- `libdrm-common=2.4.101-2~18.04.1`
- `libdrm-intel1:amd64=2.4.101-2~18.04.1`
- `libdrm-nouveau2:amd64=2.4.101-2~18.04.1`
- `libdrm-radeon1:amd64=2.4.101-2~18.04.1`
- `libdrm2:amd64=2.4.101-2~18.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libdrm=2.4.101-2~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.101-2~18.04.1.dsc' libdrm_2.4.101-2~18.04.1.dsc 3297 SHA512:96d96d552b439a04502e8b32a0d27d02cb1f72cdc6245f9c88c4a114bef74a1629fc1c96ff7888e36a88721154a6ce94920e4b1a5d07504379346936d900c702
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.101.orig.tar.xz' libdrm_2.4.101.orig.tar.xz 408856 SHA512:658cfc6f478b674b77b4613e1af9ce8f4fd2ace8a18e75729de254d14b7c1f5d67d4bfdb58744aea74abca0f6521326225f4156bd5cbeeed79ca3e025f657e8c
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.101.orig.tar.xz.asc' libdrm_2.4.101.orig.tar.xz.asc 833 SHA512:7c3897cb19de52e3a3d259e07993bc2e9699751497b4e3abd1b604a2eb8a5ffaa29cae61f92d2415befa34811e9f91189366b354dac9ab1e93c8a90a367860c2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.101-2~18.04.1.debian.tar.xz' libdrm_2.4.101-2~18.04.1.debian.tar.xz 54212 SHA512:96d7085a73abfcda2997c45e833026e98f1eeb586ed546336aca8a19862d7b7b019f8e64bb6185c6d7b6f27f1cdf9d80e8c939298b4526243c27fcd62116d590
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

### `dpkg` source package: `libedit=3.1-20170329-1`

Binary Packages:

- `libedit2:amd64=3.1-20170329-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20170329-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20170329-1.dsc' libedit_3.1-20170329-1.dsc 2269 SHA256:1e657cfcfbbe5c550b844f17cfeb1d8591136fa57300e6cff2b56e5a3e25ad3f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20170329.orig.tar.gz' libedit_3.1-20170329.orig.tar.gz 508504 SHA256:91f2d90fbd2a048ff6dad7131d9a39e690fd8a8fd982a353f1333dd4017dd4be
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20170329-1.debian.tar.bz2' libedit_3.1-20170329-1.debian.tar.bz2 11267 SHA256:7dd7a23b07b082d058b7fb741d3b750b80699472e7c8efd1935a9e7c59a49a39
```

### `dpkg` source package: `libencode-locale-perl=1.05-1`

Binary Packages:

- `libencode-locale-perl=1.05-1`

Licenses: (parsed from: `/usr/share/doc/libencode-locale-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libencode-locale-perl=1.05-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libencode-locale-perl/libencode-locale-perl_1.05-1.dsc' libencode-locale-perl_1.05-1.dsc 2107 SHA256:2a91183e11732070009fa8b01febde8509e00b69585f8eb56a5c8dce61a5df51
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libencode-locale-perl/libencode-locale-perl_1.05.orig.tar.gz' libencode-locale-perl_1.05.orig.tar.gz 8355 SHA256:176fa02771f542a4efb1dbc2a4c928e8f4391bf4078473bd6040d8f11adb0ec1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libencode-locale-perl/libencode-locale-perl_1.05-1.debian.tar.xz' libencode-locale-perl_1.05-1.debian.tar.xz 2528 SHA256:e722122fa3c8cf0d6d5fead77184d791c341c54985f171a3bb9ece3688d94e48
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

### `dpkg` source package: `libfile-basedir-perl=0.07-1`

Binary Packages:

- `libfile-basedir-perl=0.07-1`

Licenses: (parsed from: `/usr/share/doc/libfile-basedir-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libfile-basedir-perl=0.07-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-basedir-perl/libfile-basedir-perl_0.07-1.dsc' libfile-basedir-perl_0.07-1.dsc 2340 SHA256:dee081ff64355ec91f787bba4acce416dbf3eec44f11c9407133a32b47356b95
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-basedir-perl/libfile-basedir-perl_0.07.orig.tar.gz' libfile-basedir-perl_0.07.orig.tar.gz 9888 SHA256:120a57ef78535e13e1465717b4056aff4ce69af1e31c67c65d1177a52169082b
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-basedir-perl/libfile-basedir-perl_0.07-1.debian.tar.xz' libfile-basedir-perl_0.07-1.debian.tar.xz 2688 SHA256:2cbbb99eadc4b6df66cb43bbf20d2a9dc5c5c3c2717e7c5bd13849db07363af9
```

### `dpkg` source package: `libfile-desktopentry-perl=0.22-1`

Binary Packages:

- `libfile-desktopentry-perl=0.22-1`

Licenses: (parsed from: `/usr/share/doc/libfile-desktopentry-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libfile-desktopentry-perl=0.22-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-desktopentry-perl/libfile-desktopentry-perl_0.22-1.dsc' libfile-desktopentry-perl_0.22-1.dsc 2400 SHA256:94d12f074e00b4c024af2a83691b96971a6fea19de5f18f0caf2675f9028031a
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-desktopentry-perl/libfile-desktopentry-perl_0.22.orig.tar.gz' libfile-desktopentry-perl_0.22.orig.tar.gz 18366 SHA256:169c01e3dae2f629767bec1a9f1cdbd6ec6d713d1501e0b2786e4dd1235635b8
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-desktopentry-perl/libfile-desktopentry-perl_0.22-1.debian.tar.xz' libfile-desktopentry-perl_0.22-1.debian.tar.xz 3244 SHA256:43ce8359412c3d1a01580c3f128e2071a33808f8bccd9d0a2ebc499d53bb49f2
```

### `dpkg` source package: `libfile-listing-perl=6.04-1`

Binary Packages:

- `libfile-listing-perl=6.04-1`

Licenses: (parsed from: `/usr/share/doc/libfile-listing-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libfile-listing-perl=6.04-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-listing-perl/libfile-listing-perl_6.04-1.dsc' libfile-listing-perl_6.04-1.dsc 1493 SHA256:b431527f181f34682315d62422ceac52db806bbeabfecae4cd877714d7dca2f4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-listing-perl/libfile-listing-perl_6.04.orig.tar.gz' libfile-listing-perl_6.04.orig.tar.gz 51536 SHA256:1e0050fcd6789a2179ec0db282bf1e90fb92be35d1171588bd9c47d52d959cf5
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-listing-perl/libfile-listing-perl_6.04-1.debian.tar.gz' libfile-listing-perl_6.04-1.debian.tar.gz 1972 SHA256:f14177c3171bd6d09912ecb82e0b3a7e10fa2d17f56d8964750aefa16b5a6b7b
```

### `dpkg` source package: `libfile-mimeinfo-perl=0.28-1`

Binary Packages:

- `libfile-mimeinfo-perl=0.28-1`

Licenses: (parsed from: `/usr/share/doc/libfile-mimeinfo-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libfile-mimeinfo-perl=0.28-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-mimeinfo-perl/libfile-mimeinfo-perl_0.28-1.dsc' libfile-mimeinfo-perl_0.28-1.dsc 2315 SHA256:a70d886f97ba6d92a5c7a6c8711c95f6f0dbb391d67753ead921272a5bc074dc
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-mimeinfo-perl/libfile-mimeinfo-perl_0.28.orig.tar.gz' libfile-mimeinfo-perl_0.28.orig.tar.gz 32561 SHA256:2a245db46f9aef7481d90b4e196a4d42a238e15f049f57fc1339c0b98681ebc6
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfile-mimeinfo-perl/libfile-mimeinfo-perl_0.28-1.debian.tar.xz' libfile-mimeinfo-perl_0.28-1.debian.tar.xz 4568 SHA256:817f68ebbfa7400ebdceefc0386b7e280c30d124bb3e00ca0ad0824aef7762a9
```

### `dpkg` source package: `libfont-afm-perl=1.20-2`

Binary Packages:

- `libfont-afm-perl=1.20-2`

Licenses: (parsed from: `/usr/share/doc/libfont-afm-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libfont-afm-perl=1.20-2
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfont-afm-perl/libfont-afm-perl_1.20-2.dsc' libfont-afm-perl_1.20-2.dsc 2070 SHA256:1b9c82ec407e56149f1d2d61d21d81fcaea0ee0292bd1b57bf8b415943b27735
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfont-afm-perl/libfont-afm-perl_1.20.orig.tar.gz' libfont-afm-perl_1.20.orig.tar.gz 10421 SHA256:32671166da32596a0f6baacd0c1233825a60acaf25805d79c81a3f18d6088bc1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfont-afm-perl/libfont-afm-perl_1.20-2.debian.tar.xz' libfont-afm-perl_1.20-2.debian.tar.xz 2732 SHA256:981bb81a767cb822668840259fd349f19bc71ef0a27f22dfe87590dbc2f2f674
```

### `dpkg` source package: `libfontenc=1:1.1.3-1`

Binary Packages:

- `libfontenc1:amd64=1:1.1.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libfontenc=1:1.1.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfontenc/libfontenc_1.1.3-1.dsc' libfontenc_1.1.3-1.dsc 2160 SHA256:87e0054659d4764f027fd85a9e95699a851ce5b890f228a600c2a36324edc9f4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfontenc/libfontenc_1.1.3.orig.tar.gz' libfontenc_1.1.3.orig.tar.gz 366621 SHA256:6fba26760ca8d5045f2b52ddf641c12cedc19ee30939c6478162b7db8b6220fb
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfontenc/libfontenc_1.1.3-1.diff.gz' libfontenc_1.1.3-1.diff.gz 8398 SHA256:51122d4d86fa210b10198a5d4e4e2e1f56f23906c43d7fb536d4b7cba5caa336
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
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.dsc' libgcrypt20_1.8.1-4ubuntu1.2.dsc 3035 SHA512:2cab68715075be201f98da207fd67354637c5a275fa4585bed5cf234b9aca50b479ed7aa4144d77005e0bc5f9680b16d364f27d57353ef5341a7327de512e705
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2' libgcrypt20_1.8.1.orig.tar.bz2 2967344 SHA512:27c9d2fd9cba5afca71d421c9299d6942463975fae0bd10d4ff42cda2d7ea213e6b73c071a40fcf23ff52a93394cc7505ab332f8a4a3321826460e471eda5b4e
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2.asc' libgcrypt20_1.8.1.orig.tar.bz2.asc 310 SHA512:2e03cade8815ef146ea186efcdef2be5e1a0cfae3b9f8fcd7d7f774503b93ab29dbd2b284c1ad260181419ae0fc23462762e9a5e20193f89af76ca4ea0c1bccf
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz' libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz 33112 SHA512:7f9196009c18514110d69f457b50dc2ff296943e04f91021193f9549f67be399013cede511131ca54dd32bfa662f26569f52a850a09823a641b640b1664ff68b
```

### `dpkg` source package: `libglvnd=1.0.0-2ubuntu2.3`

Binary Packages:

- `libegl1:amd64=1.0.0-2ubuntu2.3`
- `libgl1:amd64=1.0.0-2ubuntu2.3`
- `libglvnd0:amd64=1.0.0-2ubuntu2.3`
- `libglx0:amd64=1.0.0-2ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/libegl1/copyright`, `/usr/share/doc/libgl1/copyright`, `/usr/share/doc/libglvnd0/copyright`, `/usr/share/doc/libglx0/copyright`)

- `BSD-1-clause`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libglvnd=1.0.0-2ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libglvnd/libglvnd_1.0.0-2ubuntu2.3.dsc' libglvnd_1.0.0-2ubuntu2.3.dsc 2435 SHA512:4e8575554e8af5ea69f536531bf7d99678471609945e0500728f192750cb1cd21b08d12bafa81c8c8885c0c5fe15d612ac26416a4df9638974582966c33bfa63
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libglvnd/libglvnd_1.0.0.orig.tar.gz' libglvnd_1.0.0.orig.tar.gz 795552 SHA512:c6040b0a508a6b74d7113f8e375fcaf93ec6f2875504953f30e2882e58e22f954bd4027a7d9ab8ac41abef266039e5834fdaf4ce2a69d5d98acf3bbdd54f04b6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libglvnd/libglvnd_1.0.0-2ubuntu2.3.debian.tar.xz' libglvnd_1.0.0-2ubuntu2.3.debian.tar.xz 21704 SHA512:08fb273e6a3a82700f86348a1bf0f57d78db7565c9da8417fbb8626529c48eb8d259cbaedebae97ba91cbfb4b151200b04f791b556b69af8551a0fab3e4e5898
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

### `dpkg` source package: `libgsm=1.0.13-4build1`

Binary Packages:

- `libgsm1:amd64=1.0.13-4build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libgsm=1.0.13-4build1
'http://archive.ubuntu.com/ubuntu/pool/universe/libg/libgsm/libgsm_1.0.13-4build1.dsc' libgsm_1.0.13-4build1.dsc 1946 SHA256:c840f9b7c515ca615934fd2a203f099d63c179b0a6579e0b6b795988aa83b48c
'http://archive.ubuntu.com/ubuntu/pool/universe/libg/libgsm/libgsm_1.0.13.orig.tar.gz' libgsm_1.0.13.orig.tar.gz 65318 SHA256:52c518244d428c2e56c543b98c9135f4a76ff780c32455580b793f60a0a092ad
'http://archive.ubuntu.com/ubuntu/pool/universe/libg/libgsm/libgsm_1.0.13-4build1.debian.tar.xz' libgsm_1.0.13-4build1.debian.tar.xz 9544 SHA256:d8a2d41e8990d70f742b269bcbe55eb7903a9b71501779e996abc9cc82c84020
```

### `dpkg` source package: `libgudev=232-2`

Binary Packages:

- `libgudev-1.0-0:amd64=1:232-2`

Licenses: (parsed from: `/usr/share/doc/libgudev-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libgudev=232-2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgudev/libgudev_232-2.dsc' libgudev_232-2.dsc 2305 SHA256:32a8bb891c441019d8fd0af123047ada6df1c42d0bc0363d88a6c8459f4ddd74
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgudev/libgudev_232.orig.tar.xz' libgudev_232.orig.tar.xz 270904 SHA256:ee4cb2b9c573cdf354f6ed744f01b111d4b5bed3503ffa956cefff50489c7860
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgudev/libgudev_232-2.debian.tar.xz' libgudev_232-2.debian.tar.xz 4556 SHA256:aa5e8df923bf2c78ba260b9bbb560a41f2d1528b83585379aa9965b4b8c98113
```

### `dpkg` source package: `libhtml-form-perl=6.03-1`

Binary Packages:

- `libhtml-form-perl=6.03-1`

Licenses: (parsed from: `/usr/share/doc/libhtml-form-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhtml-form-perl=6.03-1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-form-perl/libhtml-form-perl_6.03-1.dsc' libhtml-form-perl_6.03-1.dsc 1494 SHA256:07f1aa9f3cf163677b7b82153769da5297bd614226600efd1c9bf34bb2415c5f
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-form-perl/libhtml-form-perl_6.03.orig.tar.gz' libhtml-form-perl_6.03.orig.tar.gz 23522 SHA256:68c01d94f005d5ca9c4d55ad2a1bf3a8d034a5fc6db187d91a4c42f3fdc9fc36
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-form-perl/libhtml-form-perl_6.03-1.debian.tar.gz' libhtml-form-perl_6.03-1.debian.tar.gz 1978 SHA256:995139be65bcab3c4afe79c88cb9200c048c63f6b51cf5b008934ae3b2d416e4
```

### `dpkg` source package: `libhtml-format-perl=2.12-1`

Binary Packages:

- `libhtml-format-perl=2.12-1`

Licenses: (parsed from: `/usr/share/doc/libhtml-format-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhtml-format-perl=2.12-1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-format-perl/libhtml-format-perl_2.12-1.dsc' libhtml-format-perl_2.12-1.dsc 2253 SHA256:85d329b257604bbbde77073ae1e8e6995a58ffa36f2db9819d880daabd03f3c6
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-format-perl/libhtml-format-perl_2.12.orig.tar.gz' libhtml-format-perl_2.12.orig.tar.gz 50248 SHA256:a8f76839e46a22c64b8635b82072799caf77393d2102fba81041db6348c66899
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-format-perl/libhtml-format-perl_2.12-1.debian.tar.xz' libhtml-format-perl_2.12-1.debian.tar.xz 3944 SHA256:42539c9cb4796a7cb1d68151b7573dbc3d591ab60799e236eee3f5889047b931
```

### `dpkg` source package: `libhtml-parser-perl=3.72-3build1`

Binary Packages:

- `libhtml-parser-perl=3.72-3build1`

Licenses: (parsed from: `/usr/share/doc/libhtml-parser-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhtml-parser-perl=3.72-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-parser-perl/libhtml-parser-perl_3.72-3build1.dsc' libhtml-parser-perl_3.72-3build1.dsc 2298 SHA256:f3c42e5495fcfa5e0af2463569f08871242bd5bdd810c1536f397c1349dd704f
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-parser-perl/libhtml-parser-perl_3.72.orig.tar.gz' libhtml-parser-perl_3.72.orig.tar.gz 90680 SHA256:ec28c7e1d9e67c45eca197077f7cdc41ead1bb4c538c7f02a3296a4bb92f608b
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-parser-perl/libhtml-parser-perl_3.72-3build1.debian.tar.xz' libhtml-parser-perl_3.72-3build1.debian.tar.xz 8868 SHA256:a5156eabc46cc8c464252ad8eb52b50591bd0dc29396a041a3119c7bce9cdb54
```

### `dpkg` source package: `libhtml-tagset-perl=3.20-3`

Binary Packages:

- `libhtml-tagset-perl=3.20-3`

Licenses: (parsed from: `/usr/share/doc/libhtml-tagset-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhtml-tagset-perl=3.20-3
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-tagset-perl/libhtml-tagset-perl_3.20-3.dsc' libhtml-tagset-perl_3.20-3.dsc 2169 SHA256:81d806e9f01b7d019a690a774552aaa8c07f64d4a54002f3b96b90d4f41be125
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-tagset-perl/libhtml-tagset-perl_3.20.orig.tar.gz' libhtml-tagset-perl_3.20.orig.tar.gz 8150 SHA256:adb17dac9e36cd011f5243881c9739417fd102fce760f8de4e9be4c7131108e2
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-tagset-perl/libhtml-tagset-perl_3.20-3.debian.tar.xz' libhtml-tagset-perl_3.20-3.debian.tar.xz 3152 SHA256:4c355d09af9573f9b1f226a7a9e4714fec71d9cb5fa1870a15c4ecb504c42e66
```

### `dpkg` source package: `libhtml-tree-perl=5.07-1`

Binary Packages:

- `libhtml-tree-perl=5.07-1`

Licenses: (parsed from: `/usr/share/doc/libhtml-tree-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhtml-tree-perl=5.07-1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-tree-perl/libhtml-tree-perl_5.07-1.dsc' libhtml-tree-perl_5.07-1.dsc 2231 SHA256:1ef539c08a35791ddcaa42a1ee6f002ada8a64a512cf277af31bd2ef281d275f
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-tree-perl/libhtml-tree-perl_5.07.orig.tar.gz' libhtml-tree-perl_5.07.orig.tar.gz 150477 SHA256:f0374db84731c204b86c1d5b90975fef0d30a86bd9def919343e554e31a9dbbf
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhtml-tree-perl/libhtml-tree-perl_5.07-1.debian.tar.xz' libhtml-tree-perl_5.07-1.debian.tar.xz 6128 SHA256:59899510dde1df1cf0ab0ff8c3ad276fbdd49ac3a15eee8ecdecadb8cab323d1
```

### `dpkg` source package: `libhttp-cookies-perl=6.04-1`

Binary Packages:

- `libhttp-cookies-perl=6.04-1`

Licenses: (parsed from: `/usr/share/doc/libhttp-cookies-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhttp-cookies-perl=6.04-1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-cookies-perl/libhttp-cookies-perl_6.04-1.dsc' libhttp-cookies-perl_6.04-1.dsc 2159 SHA256:c793ceb91b725e82ce74b21f638146a35ed7685da17d56ddc3668f506a688499
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-cookies-perl/libhttp-cookies-perl_6.04.orig.tar.gz' libhttp-cookies-perl_6.04.orig.tar.gz 39502 SHA256:0cc7f079079dcad8293fea36875ef58dd1bfd75ce1a6c244cd73ed9523eb13d4
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-cookies-perl/libhttp-cookies-perl_6.04-1.debian.tar.xz' libhttp-cookies-perl_6.04-1.debian.tar.xz 2628 SHA256:a82f4206432fa02bfbd0846255d19d055814633e1b83e425c2e92c89f0f062d9
```

### `dpkg` source package: `libhttp-daemon-perl=6.01-1`

Binary Packages:

- `libhttp-daemon-perl=6.01-1`

Licenses: (parsed from: `/usr/share/doc/libhttp-daemon-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhttp-daemon-perl=6.01-1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-daemon-perl/libhttp-daemon-perl_6.01-1.dsc' libhttp-daemon-perl_6.01-1.dsc 2136 SHA256:2cd8a7bd8edb9872bb45dcecfadaabe9fe0ea15d877d1b7692e32c04a1c7f149
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-daemon-perl/libhttp-daemon-perl_6.01.orig.tar.gz' libhttp-daemon-perl_6.01.orig.tar.gz 18628 SHA256:43fd867742701a3f9fcc7bd59838ab72c6490c0ebaf66901068ec6997514adc2
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-daemon-perl/libhttp-daemon-perl_6.01-1.debian.tar.gz' libhttp-daemon-perl_6.01-1.debian.tar.gz 1944 SHA256:fc19acdf7808a6ba22d7120bdf25488625a3c2a3e797ea2f3110af844a4f3cad
```

### `dpkg` source package: `libhttp-date-perl=6.02-1`

Binary Packages:

- `libhttp-date-perl=6.02-1`

Licenses: (parsed from: `/usr/share/doc/libhttp-date-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhttp-date-perl=6.02-1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-date-perl/libhttp-date-perl_6.02-1.dsc' libhttp-date-perl_6.02-1.dsc 2062 SHA256:01ce4948f18b63647ac1c57d1e849265b355ec3e772fe54a9249682c3f75fcae
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-date-perl/libhttp-date-perl_6.02.orig.tar.gz' libhttp-date-perl_6.02.orig.tar.gz 7319 SHA256:e8b9941da0f9f0c9c01068401a5e81341f0e3707d1c754f8e11f42a7e629e333
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-date-perl/libhttp-date-perl_6.02-1.debian.tar.gz' libhttp-date-perl_6.02-1.debian.tar.gz 1592 SHA256:a5dd0863eda1dd56690d76309edfc97b9cc65a8a734df8ea7344e6ce383a38e1
```

### `dpkg` source package: `libhttp-message-perl=6.14-1`

Binary Packages:

- `libhttp-message-perl=6.14-1`

Licenses: (parsed from: `/usr/share/doc/libhttp-message-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhttp-message-perl=6.14-1
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-message-perl/libhttp-message-perl_6.14-1.dsc' libhttp-message-perl_6.14-1.dsc 2362 SHA256:0f754a023dd86c311d61c82532cf1ae9ab05a79d71506c4663070158e68818fe
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-message-perl/libhttp-message-perl_6.14.orig.tar.gz' libhttp-message-perl_6.14.orig.tar.gz 77663 SHA256:71aab9f10eb4b8ec6e8e3a85fc5acb46ba04db1c93eb99613b184078c5cf2ac9
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-message-perl/libhttp-message-perl_6.14-1.debian.tar.xz' libhttp-message-perl_6.14-1.debian.tar.xz 2904 SHA256:38f3a47b37bff7fbbebbbb7ee0abfc2858e807d8590f0cb6eac20303804cfd0e
```

### `dpkg` source package: `libhttp-negotiate-perl=6.00-2`

Binary Packages:

- `libhttp-negotiate-perl=6.00-2`

Licenses: (parsed from: `/usr/share/doc/libhttp-negotiate-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libhttp-negotiate-perl=6.00-2
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-negotiate-perl/libhttp-negotiate-perl_6.00-2.dsc' libhttp-negotiate-perl_6.00-2.dsc 2051 SHA256:987f88c27f0f81e718d0e5275a57f71d329ee7e86adbf0fd33c1b031ac7453b3
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-negotiate-perl/libhttp-negotiate-perl_6.00.orig.tar.gz' libhttp-negotiate-perl_6.00.orig.tar.gz 8560 SHA256:4e070ea67427ab1843620debc923b820bd41b9018914dfef54bbc7af9257ae82
'http://archive.ubuntu.com/ubuntu/pool/main/libh/libhttp-negotiate-perl/libhttp-negotiate-perl_6.00-2.debian.tar.gz' libhttp-negotiate-perl_6.00-2.debian.tar.gz 1663 SHA256:f376bf7dc122ce088d0938d4e975178e37ec91187684150503667a81dfc19734
```

### `dpkg` source package: `libice=2:1.0.9-2`

Binary Packages:

- `libice-dev:amd64=2:1.0.9-2`
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
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.dsc' libidn2_2.0.4-1.1ubuntu0.2.dsc 2391 SHA512:5c6d826b5994bdeb59f7d71b060643e051ed32ee0c013f638cb80cbb1fb3ad60671b20503bb47fbfabd29005bd3848a95f3bdae7b4ef6ae1d55cabfb4745fc9c
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4.orig.tar.gz' libidn2_2.0.4.orig.tar.gz 2008524 SHA512:1e51bd4b8f8907531576291f1c2a8865d17429b4105418b4c98754eb982cd1cbb3adbeab4ec0c1c561d2dba11d876c7c09e5dc5b315c55a2c24986d7a2a3b4d2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz' libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz 10290460 SHA512:b46d51758767ae8d7cc5e9fe59df28c559baac7677bfbfd6a2e51b84c29211e38a5f85ec27afd9e72ec333ea81d03ae783a03e1d8202a0f6ef52dd7bde47475f
```

### `dpkg` source package: `libidn=1.33-2.1ubuntu1.2`

Binary Packages:

- `libidn11:amd64=1.33-2.1ubuntu1.2`

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
$ apt-get source -qq --print-uris libidn=1.33-2.1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.33-2.1ubuntu1.2.dsc' libidn_1.33-2.1ubuntu1.2.dsc 2208 SHA512:0eda11fd0faf4226a74fc5d63faefc45540be84018348091f4b0729a6e1d9ca1e9876c098a5e7f58302c8909dd7b73f207a88c13108f8fcf9b182c5d338818cc
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.33.orig.tar.gz' libidn_1.33.orig.tar.gz 3501056 SHA512:38dd459eaeda0c9e3cc2d24d967113515a499747550a2a9157f32357def90d71a3a3b52398e96a44a28cd5948dc353b0473c4ff0453a69720191c4cb49cac2c6
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.33-2.1ubuntu1.2.debian.tar.xz' libidn_1.33-2.1ubuntu1.2.debian.tar.xz 65932 SHA512:66ea071e4eee031408822069dd86d400c3eed6ef6bf704a20b26d716c9c46461982af4eee0b21559476fb9b82afde4897410c68df02d7eb0ef56abbcd4d285f3
```

### `dpkg` source package: `libiec61883=1.2.0-2`

Binary Packages:

- `libiec61883-0:amd64=1.2.0-2`

Licenses: (parsed from: `/usr/share/doc/libiec61883-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libiec61883=1.2.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libiec61883/libiec61883_1.2.0-2.dsc' libiec61883_1.2.0-2.dsc 1928 SHA256:1137ced1712a1e805379c97df8e06ca5287fc8f951414d9aa85ed7ef6e4a09ce
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libiec61883/libiec61883_1.2.0.orig.tar.gz' libiec61883_1.2.0.orig.tar.gz 339064 SHA256:7c7879c6b9add3148baea697dfbfdcefffbc8ac74e8e6bcf46125ec1d21b373a
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libiec61883/libiec61883_1.2.0-2.debian.tar.xz' libiec61883_1.2.0-2.debian.tar.xz 14708 SHA256:f913b26d2724871dbf617e5af9e6c15d5e4ab6404648b3fce810d70cf39c104f
```

### `dpkg` source package: `libio-html-perl=1.001-1`

Binary Packages:

- `libio-html-perl=1.001-1`

Licenses: (parsed from: `/usr/share/doc/libio-html-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libio-html-perl=1.001-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libio-html-perl/libio-html-perl_1.001-1.dsc' libio-html-perl_1.001-1.dsc 2143 SHA256:d9065afdd12b5e0c534938f17a846e9fec028457053d4a064f7f95ebb68f2e5c
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libio-html-perl/libio-html-perl_1.001.orig.tar.gz' libio-html-perl_1.001.orig.tar.gz 19375 SHA256:ea78d2d743794adc028bc9589538eb867174b4e165d7d8b5f63486e6b828e7e0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libio-html-perl/libio-html-perl_1.001-1.debian.tar.xz' libio-html-perl_1.001-1.debian.tar.xz 3124 SHA256:89c86132e54f7f967b4f31eb42ff922eb4017c60e45ba2264e42ba620146f844
```

### `dpkg` source package: `libio-socket-ssl-perl=2.060-3~ubuntu18.04.1`

Binary Packages:

- `libio-socket-ssl-perl=2.060-3~ubuntu18.04.1`

Licenses: (parsed from: `/usr/share/doc/libio-socket-ssl-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libio-socket-ssl-perl=2.060-3~ubuntu18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libio-socket-ssl-perl/libio-socket-ssl-perl_2.060-3~ubuntu18.04.1.dsc' libio-socket-ssl-perl_2.060-3~ubuntu18.04.1.dsc 2699 SHA512:c28730480eb774f1a03a087297270c2ef6e1fe84f86311e6a04e48b7cdde28ac49c93cfca91615532f828a65266695ca7ed1a5a61ecb0b2f1d9fb92845d6c8d2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libio-socket-ssl-perl/libio-socket-ssl-perl_2.060.orig.tar.gz' libio-socket-ssl-perl_2.060.orig.tar.gz 233169 SHA512:1a1e29f8a4b912bd3643509356c66b3a567ae41bb0ac9eb30f6ca97eb68bf9507e20c0fb8512f5dfd309accd6cfba61811b8d637f5e991aaa0a250a906fcb95c
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libio-socket-ssl-perl/libio-socket-ssl-perl_2.060-3~ubuntu18.04.1.debian.tar.xz' libio-socket-ssl-perl_2.060-3~ubuntu18.04.1.debian.tar.xz 11800 SHA512:f676b9c0801773b369aa8e7d595bf2dfaa4923f58609159074e7017bae65267e7c734c7f818b84c9331ca09fa6f57aa37d4a0bc2be30f0673e1b74fd2d65f188
```

### `dpkg` source package: `libipc-system-simple-perl=1.25-4`

Binary Packages:

- `libipc-system-simple-perl=1.25-4`

Licenses: (parsed from: `/usr/share/doc/libipc-system-simple-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libipc-system-simple-perl=1.25-4
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libipc-system-simple-perl/libipc-system-simple-perl_1.25-4.dsc' libipc-system-simple-perl_1.25-4.dsc 2427 SHA256:3bc37e9b691df3f72e1fd16014d8e1b0964c9558470717933089d618b760dce7
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libipc-system-simple-perl/libipc-system-simple-perl_1.25.orig.tar.gz' libipc-system-simple-perl_1.25.orig.tar.gz 29744 SHA256:f1b6aa1dfab886e8e4ea825f46a1cbb26038ef3e727fef5d84444aa8035a4d3b
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libipc-system-simple-perl/libipc-system-simple-perl_1.25-4.debian.tar.xz' libipc-system-simple-perl_1.25-4.debian.tar.xz 2968 SHA256:7c341dcbba739c4805f203fd3e9787777f2107eababee1a6dd852875828238b6
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
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.dsc' libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.dsc 2391 SHA512:8cefc52a722cfdb11e157edaf1afcba85a41e2b2767a0d4cb73ed50526a065da01a807bd2eebeceed19d77386a93f7470e41d8f9a5254c4be69570c8700472d5
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2.orig.tar.gz' libjpeg-turbo_1.5.2.orig.tar.gz 1657235 SHA512:c7fe5cc77e38fad33af3f10e6db961c8edf033a86c09541121f49bfa20547179760924e6d3e397f0add7030459ff3babadd3457ab2da4a40a2147dc1574aa444
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.debian.tar.xz' libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.debian.tar.xz 35396 SHA512:62f1fd71a1cee7e2e196ec48ea45b3968af3f97671c0059cb77d59149efacc7846834fd12b21c6cec4d4c0ca4b4ca351386e425d6bcea682a9df060d8c887f39
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
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.1.dsc' liblqr_0.4.2-2.1.dsc 2095 SHA256:c54c34cd2f7470a29366eeacde2ca4859a97d684a406fb81a918b970c01d617c
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA256:d4c22373432cca749e4326cd41fce365e6ff857c0bfd7a5302b8eb34b69f0336
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.1.debian.tar.xz' liblqr_0.4.2-2.1.debian.tar.xz 5300 SHA256:284a002f1ecac63ac17b1aafbb230da9ce7bd9efe2d5b94e8cad49b607eb2564
```

### `dpkg` source package: `liblwp-mediatypes-perl=6.02-1`

Binary Packages:

- `liblwp-mediatypes-perl=6.02-1`

Licenses: (parsed from: `/usr/share/doc/liblwp-mediatypes-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris liblwp-mediatypes-perl=6.02-1
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblwp-mediatypes-perl/liblwp-mediatypes-perl_6.02-1.dsc' liblwp-mediatypes-perl_6.02-1.dsc 2107 SHA256:1e82d5a00a1502a4ca81ce16cc4cc75c7d2cc3db06b5c7f02fec81671fb4ae18
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblwp-mediatypes-perl/liblwp-mediatypes-perl_6.02.orig.tar.gz' liblwp-mediatypes-perl_6.02.orig.tar.gz 18722 SHA256:18790b0cc5f0a51468495c3847b16738f785a2d460403595001e0b932e5db676
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblwp-mediatypes-perl/liblwp-mediatypes-perl_6.02-1.debian.tar.gz' liblwp-mediatypes-perl_6.02-1.debian.tar.gz 1693 SHA256:31353fc0103f52aa7e93589ef19049de3cf282bc54bcd9786fef0bc0f15172bc
```

### `dpkg` source package: `liblwp-protocol-https-perl=6.07-2`

Binary Packages:

- `liblwp-protocol-https-perl=6.07-2`

Licenses: (parsed from: `/usr/share/doc/liblwp-protocol-https-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris liblwp-protocol-https-perl=6.07-2
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblwp-protocol-https-perl/liblwp-protocol-https-perl_6.07-2.dsc' liblwp-protocol-https-perl_6.07-2.dsc 2365 SHA256:4c6526012e024c27d6b8bf4b4315716bf78d62289040ac734910b1cabbbd3dc1
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblwp-protocol-https-perl/liblwp-protocol-https-perl_6.07.orig.tar.gz' liblwp-protocol-https-perl_6.07.orig.tar.gz 9184 SHA256:522cc946cf84a1776304a5737a54b8822ec9e79b264d0ba0722a70473dbfb9e7
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblwp-protocol-https-perl/liblwp-protocol-https-perl_6.07-2.debian.tar.xz' liblwp-protocol-https-perl_6.07-2.debian.tar.xz 4220 SHA256:30a2da4a67b251dea4e48d47099b0deb313d8dce16493d9a4820db2fd0248eac
```

### `dpkg` source package: `libmailtools-perl=2.18-1`

Binary Packages:

- `libmailtools-perl=2.18-1`

Licenses: (parsed from: `/usr/share/doc/libmailtools-perl/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libmailtools-perl=2.18-1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmailtools-perl/libmailtools-perl_2.18-1.dsc' libmailtools-perl_2.18-1.dsc 1848 SHA256:931c87401d4ad1e401590380963fb4beea4d4f076369715c5953ae447f6ed0b1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmailtools-perl/libmailtools-perl_2.18.orig.tar.gz' libmailtools-perl_2.18.orig.tar.gz 55263 SHA256:dfee9e770257371112f20d978e637759e81bc4f19e97b083585c71ecab37b527
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmailtools-perl/libmailtools-perl_2.18-1.debian.tar.xz' libmailtools-perl_2.18-1.debian.tar.xz 6252 SHA256:69689491c1453b28183b97fc24866f7fd3814a7534c7a669e414d912bdb79809
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

### `dpkg` source package: `libmysofa=0.6~dfsg0-2ubuntu0.18.04.1`

Binary Packages:

- `libmysofa0:amd64=0.6~dfsg0-2ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libmysofa0/copyright`)

- `BSD-3-clause`
- `CC-BY-4.0`
- `CC-BY-SA-3.0`
- `cipic`
- `listen-ircam`
- `mit-kemar`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libnet-dbus-perl=1.1.0-4build2`

Binary Packages:

- `libnet-dbus-perl=1.1.0-4build2`

Licenses: (parsed from: `/usr/share/doc/libnet-dbus-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libnet-dbus-perl=1.1.0-4build2
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-dbus-perl/libnet-dbus-perl_1.1.0-4build2.dsc' libnet-dbus-perl_1.1.0-4build2.dsc 2190 SHA256:11188d2b250f46e783d0e0ef2290b465f66b01e8ef5c12b603ce5333c09ea36c
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-dbus-perl/libnet-dbus-perl_1.1.0.orig.tar.gz' libnet-dbus-perl_1.1.0.orig.tar.gz 111128 SHA256:94ef2a6b2a8172699a707cd59883087e26af7c8dd8ae877efbade5956f2753fb
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-dbus-perl/libnet-dbus-perl_1.1.0-4build2.debian.tar.xz' libnet-dbus-perl_1.1.0-4build2.debian.tar.xz 7088 SHA256:8047a0c5bf61ccf8bb7a34af6a71689c79182cf91925fc8817c98598454fa099
```

### `dpkg` source package: `libnet-http-perl=6.17-1`

Binary Packages:

- `libnet-http-perl=6.17-1`

Licenses: (parsed from: `/usr/share/doc/libnet-http-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libnet-http-perl=6.17-1
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-http-perl/libnet-http-perl_6.17-1.dsc' libnet-http-perl_6.17-1.dsc 2295 SHA256:1f66e5b51026bdf3df9fdb61413f7e1006c7c5679c1161b1af72116b9d8272a6
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-http-perl/libnet-http-perl_6.17.orig.tar.gz' libnet-http-perl_6.17.orig.tar.gz 37943 SHA256:1e8624b1618dc6f7f605f5545643ebb9b833930f4d7485d4124aa2f2f26d1611
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-http-perl/libnet-http-perl_6.17-1.debian.tar.xz' libnet-http-perl_6.17-1.debian.tar.xz 3304 SHA256:7c6af613c6ecaa5159e382aa54b5ff48d88e48e7a30190c899348c90664c0857
```

### `dpkg` source package: `libnet-smtp-ssl-perl=1.04-1`

Binary Packages:

- `libnet-smtp-ssl-perl=1.04-1`

Licenses: (parsed from: `/usr/share/doc/libnet-smtp-ssl-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libnet-smtp-ssl-perl=1.04-1
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-smtp-ssl-perl/libnet-smtp-ssl-perl_1.04-1.dsc' libnet-smtp-ssl-perl_1.04-1.dsc 2268 SHA256:9429f4671338f756fc68b344cbf3a92a8624e71af68471c841c284ae32907b70
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-smtp-ssl-perl/libnet-smtp-ssl-perl_1.04.orig.tar.gz' libnet-smtp-ssl-perl_1.04.orig.tar.gz 2457 SHA256:7b29c45add19d3d5084b751f7ba89a8e40479a446ce21cfd9cc741e558332a00
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-smtp-ssl-perl/libnet-smtp-ssl-perl_1.04-1.debian.tar.xz' libnet-smtp-ssl-perl_1.04-1.debian.tar.xz 2696 SHA256:5826b6569145f52a575084a6f8da3601b361e4a2940218149b1591146f9499c6
```

### `dpkg` source package: `libnet-ssleay-perl=1.84-1ubuntu0.2`

Binary Packages:

- `libnet-ssleay-perl=1.84-1ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libnet-ssleay-perl/copyright`)

- `Artistic`
- `Artistic-2.0`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libnet-ssleay-perl=1.84-1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-ssleay-perl/libnet-ssleay-perl_1.84-1ubuntu0.2.dsc' libnet-ssleay-perl_1.84-1ubuntu0.2.dsc 2358 SHA512:2b7e7bf66d7a6ea9b84ae8fa5a60e4bd75887346a4a7ea1daebb7297f13b2b8fcc679b2345734bc3d195300cdb3fb6c71b936f9ecb342bdd7cee73ed96625ebf
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-ssleay-perl/libnet-ssleay-perl_1.84.orig.tar.gz' libnet-ssleay-perl_1.84.orig.tar.gz 418214 SHA512:8bec39297a8e38f59f8b8a53c234ace79eec9088e5924df3a94b47a87f3ba6ae961c8596680bd9a8a3403e74e15c3d69ecfcc95724ce6b305adc881aa01ce075
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnet-ssleay-perl/libnet-ssleay-perl_1.84-1ubuntu0.2.debian.tar.xz' libnet-ssleay-perl_1.84-1ubuntu0.2.debian.tar.xz 18300 SHA512:87b1e720202117edcadf16f2c56d4374829076d398d6c4ffdd7130020bf77c17a9253ac43a688d0b2d6deaac426e62141c97ecb74f5327bcc6b2aa1004c6d762
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

### `dpkg` source package: `libogg=1.3.2-1`

Binary Packages:

- `libogg0:amd64=1.3.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libogg=1.3.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libogg/libogg_1.3.2-1.dsc' libogg_1.3.2-1.dsc 1230 SHA256:dacc2059f8f92d1f6b18805432f2f40ac45fb9d52a1a61f14dc8c7c6a1aecb58
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libogg/libogg_1.3.2.orig.tar.gz' libogg_1.3.2.orig.tar.gz 557232 SHA256:bf253517df60ef1e6f5ae328bac7477595465de30638818948574e05f502dfa3
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libogg/libogg_1.3.2-1.diff.gz' libogg_1.3.2-1.diff.gz 6824 SHA256:9bee2f473a5ed92f1c744105447f15fe38feea8935e740a9eea2d840fa2d15c7
```

### `dpkg` source package: `libopenmpt=0.3.6-1`

Binary Packages:

- `libopenmpt0:amd64=0.3.6-1`

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
$ apt-get source -qq --print-uris libopenmpt=0.3.6-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libo/libopenmpt/libopenmpt_0.3.6-1.dsc' libopenmpt_0.3.6-1.dsc 2589 SHA256:3e9131101540793a44323aef4bc146dccd608ace202245b0032552c098f64da6
'http://archive.ubuntu.com/ubuntu/pool/universe/libo/libopenmpt/libopenmpt_0.3.6.orig.tar.gz' libopenmpt_0.3.6.orig.tar.gz 1409983 SHA256:0a49e4770c9c7778cd6544ad559bff873ec905c4a3ba6521f6bf192b1c0b34d2
'http://archive.ubuntu.com/ubuntu/pool/universe/libo/libopenmpt/libopenmpt_0.3.6-1.debian.tar.xz' libopenmpt_0.3.6-1.debian.tar.xz 12336 SHA256:74d9634433a10c335be3ce612657dc4bc0bf26647e1f521edd0c0e7dde27821c
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

### `dpkg` source package: `libpaper=1.1.24+nmu5ubuntu1`

Binary Packages:

- `libpaper-utils=1.1.24+nmu5ubuntu1`
- `libpaper1:amd64=1.1.24+nmu5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpaper-utils/copyright`, `/usr/share/doc/libpaper1/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpaper=1.1.24+nmu5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpaper/libpaper_1.1.24+nmu5ubuntu1.dsc' libpaper_1.1.24+nmu5ubuntu1.dsc 1740 SHA256:8963b5701a10bb0ba511385cf73c735105eccf8674b4b5284372b8f266b98e63
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpaper/libpaper_1.1.24+nmu5ubuntu1.tar.gz' libpaper_1.1.24+nmu5ubuntu1.tar.gz 49965 SHA256:0d8f4e87ed194ff4d9139482079efe081ef713e894a4f2f2cb7f56d0cb17f4c8
```

### `dpkg` source package: `libpciaccess=0.14-1`

Binary Packages:

- `libpciaccess0:amd64=0.14-1`

Licenses: (parsed from: `/usr/share/doc/libpciaccess0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpciaccess=0.14-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.14-1.dsc' libpciaccess_0.14-1.dsc 2062 SHA256:1cbfd426e4efcc958b6c9fd4889877b533035175370fa0505f361b89e1aeaa4f
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.14.orig.tar.gz' libpciaccess_0.14.orig.tar.gz 461764 SHA256:8d86e64893917be3dfb1c5e837888d1275399c818783474002203d751312b03c
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.14-1.diff.gz' libpciaccess_0.14-1.diff.gz 25039 SHA256:fea9483fbfb202040a8e5eef3ec3b434b3e897f301e735753568db2106e1512d
```

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
'http://archive.ubuntu.com/ubuntu/pool/universe/libp/libpgm/libpgm_5.2.122~dfsg-2.dsc' libpgm_5.2.122~dfsg-2.dsc 1870 SHA256:2d6eb667fd66046c4c35215068cfa562decd8d0838ec864a35796cdad354fc49
'http://archive.ubuntu.com/ubuntu/pool/universe/libp/libpgm/libpgm_5.2.122~dfsg.orig.tar.xz' libpgm_5.2.122~dfsg.orig.tar.xz 550996 SHA256:d6e5ec0918216d4e9b14459f5742f6f8416df965f03ac4d854bd5d111709b507
'http://archive.ubuntu.com/ubuntu/pool/universe/libp/libpgm/libpgm_5.2.122~dfsg-2.debian.tar.xz' libpgm_5.2.122~dfsg-2.debian.tar.xz 6568 SHA256:5f02e1055a199f545d99f4f709330abe5e31c7073a3cb2ed737a4fbb5b7d2857
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
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc' libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc 2362 SHA512:306827271e4b470dacd142c5b7b4c8d97561c5b2fa39ea5fc36f20bc29f6929c868a0e926179835a24569825def8a778872100b54fbbd1f4b03a817730c40238
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34.orig.tar.xz' libpng1.6_1.6.34.orig.tar.xz 997968 SHA512:89407c5abc1623faaa3992fc1e4a62def671d9a7401108dfceee895d5f16fe7030090bea89b34a36d377d8e6a5d40046886991f663ce075d1a2d31bf9eaf3c51
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz' libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz 24572 SHA512:7b13f1e486f15260f90376604e92c4050ffbf9023bcca17e527b9d5cf81fffdce83301893d635049939d12608a12835f9e3cbf4321b24dbd08afc5efe8d1a50d
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

### `dpkg` source package: `libpthread-stubs=0.3-4`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.3-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.3-4
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3-4.dsc' libpthread-stubs_0.3-4.dsc 1925 SHA256:e72310a5492e641076c199561977703947174c6acc3633073d909f6f5ab3c676
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3.orig.tar.gz' libpthread-stubs_0.3.orig.tar.gz 272939 SHA256:3031f466cf0b06de6b3ccbf2019d15c4fcf75229b7d226a711bc1885b3a82cde
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3-4.diff.gz' libpthread-stubs_0.3-4.diff.gz 2413 SHA256:ce3eb8bdc0f1a4347d42c5736d056973fae46908b764a9f2be83e1bd210f2024
```

### `dpkg` source package: `libraw1394=2.1.2-1`

Binary Packages:

- `libraw1394-11:amd64=2.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libraw1394-11/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libraw1394=2.1.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libraw1394/libraw1394_2.1.2-1.dsc' libraw1394_2.1.2-1.dsc 2080 SHA256:d8b7cb13f4a73fa0dae8d61d5b4ded82b3f02d6b3584ac77c671432d250988f4
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libraw1394/libraw1394_2.1.2.orig.tar.gz' libraw1394_2.1.2.orig.tar.gz 458134 SHA256:ddc4e32721cdfe680d964aaede68ac606a20cd17dd2ba70e2d7e0692086ab57c
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libraw1394/libraw1394_2.1.2-1.debian.tar.xz' libraw1394_2.1.2-1.debian.tar.xz 8760 SHA256:5cee0e0049d820a8e4e5d3dbd94fb2c3d7b782ec09134c6c714ed523829dc1c3
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
- `libreoffice-gnome=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-gtk3=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-impress=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-java-common=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-librelogo=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-math=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-nlpsolver=0.9+LibO6.0.7-0ubuntu0.18.04.10`
- `libreoffice-ogltrans=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-report-builder=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-report-builder-bin=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-script-provider-bsh=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-script-provider-js=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-script-provider-python=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-sdbc-hsqldb=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-sdbc-postgresql=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-style-galaxy=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-style-tango=1:6.0.7-0ubuntu0.18.04.10`
- `libreoffice-wiki-publisher=1.2.0+LibO6.0.7-0ubuntu0.18.04.10`
- `libreoffice-writer=1:6.0.7-0ubuntu0.18.04.10`
- `python3-uno=1:6.0.7-0ubuntu0.18.04.10`
- `uno-libs3=6.0.7-0ubuntu0.18.04.10`
- `ure=6.0.7-0ubuntu0.18.04.10`

Licenses: (parsed from: `/usr/share/doc/fonts-opensymbol/copyright`, `/usr/share/doc/libreoffice/copyright`, `/usr/share/doc/libreoffice-avmedia-backend-gstreamer/copyright`, `/usr/share/doc/libreoffice-base/copyright`, `/usr/share/doc/libreoffice-base-core/copyright`, `/usr/share/doc/libreoffice-base-drivers/copyright`, `/usr/share/doc/libreoffice-calc/copyright`, `/usr/share/doc/libreoffice-common/copyright`, `/usr/share/doc/libreoffice-core/copyright`, `/usr/share/doc/libreoffice-draw/copyright`, `/usr/share/doc/libreoffice-gnome/copyright`, `/usr/share/doc/libreoffice-gtk3/copyright`, `/usr/share/doc/libreoffice-impress/copyright`, `/usr/share/doc/libreoffice-java-common/copyright`, `/usr/share/doc/libreoffice-librelogo/copyright`, `/usr/share/doc/libreoffice-math/copyright`, `/usr/share/doc/libreoffice-nlpsolver/copyright`, `/usr/share/doc/libreoffice-ogltrans/copyright`, `/usr/share/doc/libreoffice-report-builder/copyright`, `/usr/share/doc/libreoffice-report-builder-bin/copyright`, `/usr/share/doc/libreoffice-script-provider-bsh/copyright`, `/usr/share/doc/libreoffice-script-provider-js/copyright`, `/usr/share/doc/libreoffice-script-provider-python/copyright`, `/usr/share/doc/libreoffice-sdbc-hsqldb/copyright`, `/usr/share/doc/libreoffice-sdbc-postgresql/copyright`, `/usr/share/doc/libreoffice-style-galaxy/copyright`, `/usr/share/doc/libreoffice-style-tango/copyright`, `/usr/share/doc/libreoffice-wiki-publisher/copyright`, `/usr/share/doc/libreoffice-writer/copyright`, `/usr/share/doc/python3-uno/copyright`, `/usr/share/doc/uno-libs3/copyright`, `/usr/share/doc/ure/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7-0ubuntu0.18.04.10.dsc' libreoffice_6.0.7-0ubuntu0.18.04.10.dsc 18078 SHA512:e610baf3dd140c38eb53712a29673df3376f29a68c70427adeb5f0b3527643fea0769df49919405139fb68cdc7846a6b24918a0ceef1d14335ea8c74539b97d4
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig-helpcontent2.tar.xz' libreoffice_6.0.7.orig-helpcontent2.tar.xz 2423012 SHA512:6d709a57bb09738cc270a380421157ed55bc71275eab47683c8a44d4f18d3655e898e59e90090fff39a18edb2e809265ef1b14f1df570b3c4b24fab4d5e9da9c
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig-tarballs.tar.xz' libreoffice_6.0.7.orig-tarballs.tar.xz 215486780 SHA512:4d1863ce4e4f7ce34d2e33a61814955e310265041ddc7972177069199e3c0ac85f1164ecc999d9c2ccacac3f882aee3b41f47a2451b415174eaf98bd6ddff814
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig-translations.tar.xz' libreoffice_6.0.7.orig-translations.tar.xz 139598364 SHA512:145043c897a7a4aa3a6892ba5f71a9ef5a0a225543e4e5554390c4cd0d7f3c278246954c6312324b190bfdd609aee55c1bd44ddd86bff86f7cd2758596cdfded
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7.orig.tar.xz' libreoffice_6.0.7.orig.tar.xz 183202236 SHA512:0e2e788a59913d35bf63afa56c87612e29a41c7d53c2031fe25ed0126669338b26e82a346cf0c7eac0fe5c285b1cd4d309aaefaee2118d3b5340885bc0ba006c
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_6.0.7-0ubuntu0.18.04.10.debian.tar.xz' libreoffice_6.0.7-0ubuntu0.18.04.10.debian.tar.xz 2178480 SHA512:0589b0a915c113b0646c10a48a874f6649e20a6281854d4e9661192d4d2295c5632782cb641a12f1e9206a396470c8a42aaceaedc5aa09b2478aeb294054143c
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
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20-2ubuntu0.2.dsc' librsvg_2.40.20-2ubuntu0.2.dsc 2846 SHA512:564b5017bd081092a1098d57b3841070efeab66cb1cafb83c5fdf3a33fba7e432e72f6693a4e10ca18eeb9e28f3787d7c05cf0f6fd6cb9b2c2d4e3de758428fc
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20.orig.tar.xz' librsvg_2.40.20.orig.tar.xz 1796376 SHA512:cdd8224deb4c3786e29f48ed02c32ed9dff5cb15aba574a5ef845801ad3669cfcc3eedb9d359c22213dc7a29de24c363248825adad5877c40abf73b3688ff12f
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20-2ubuntu0.2.debian.tar.xz' librsvg_2.40.20-2ubuntu0.2.debian.tar.xz 16768 SHA512:b87308a049c4aeac87b565c48f88fab84feefb3db4c5f03f1619206ab2920993a59222ee4617d51fd04ad874e277cb00c5748539b14cbe7d9f003ccb601a5e83
```

### `dpkg` source package: `libsamplerate=0.1.9-1`

Binary Packages:

- `libsamplerate0:amd64=0.1.9-1`

Licenses: (parsed from: `/usr/share/doc/libsamplerate0/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libsamplerate=0.1.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsamplerate/libsamplerate_0.1.9-1.dsc' libsamplerate_0.1.9-1.dsc 2039 SHA256:4a7460c6b0f1e0387e6106dfc57957ecf803550d60c4658316cfa0f81b720455
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsamplerate/libsamplerate_0.1.9.orig.tar.gz' libsamplerate_0.1.9.orig.tar.gz 4336641 SHA256:0a7eb168e2f21353fb6d84da152e4512126f7dc48ccb0be80578c565413444c1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsamplerate/libsamplerate_0.1.9-1.debian.tar.xz' libsamplerate_0.1.9-1.debian.tar.xz 7424 SHA256:71ed7abb72b70fe3654e48fbbd4c338bd525f2a03dc3bdfed6682540d660720c
```

### `dpkg` source package: `libsdl2=2.0.8+dfsg1-1ubuntu1.18.04.4`

Binary Packages:

- `libsdl2-2.0-0:amd64=2.0.8+dfsg1-1ubuntu1.18.04.4`

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
$ apt-get source -qq --print-uris libsdl2=2.0.8+dfsg1-1ubuntu1.18.04.4
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsdl2/libsdl2_2.0.8+dfsg1-1ubuntu1.18.04.4.dsc' libsdl2_2.0.8+dfsg1-1ubuntu1.18.04.4.dsc 2561 SHA512:a65bff7f5906d434148bc1c96a030d639cf56a7b75e7b1db0c0f9c86d04afdb3bd3d7cd98c244900b59ff984c7bfe822fc672f58afcfd0924feb44ea37b418d1
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsdl2/libsdl2_2.0.8+dfsg1.orig.tar.gz' libsdl2_2.0.8+dfsg1.orig.tar.gz 3269839 SHA512:46dbdc722cef472376b06400ddc8091fc639682a3d8e926bb1e19adc92f694cce5202a462438a7d4106f11b2951edc962ed6b0632aac64bacb714a3849c74ac9
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsdl2/libsdl2_2.0.8+dfsg1-1ubuntu1.18.04.4.debian.tar.xz' libsdl2_2.0.8+dfsg1-1ubuntu1.18.04.4.debian.tar.xz 18712 SHA512:794d8f79d81207070427b96d54ec0169d514a0f46a463c63b48025ceb7ba5b4e3ff7a2a022bbcec1e4c9b67876945c73f99554a0a8f5140c53a8fc058676b415
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
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.dsc' libseccomp_2.4.3-1ubuntu3.18.04.3.dsc 1951 SHA512:5a16b743f8e8e0d13348e731e5a8519a8b4db4f7f933f613d4422b48f62406b8e89d6f7c83f4c12d12b665aea62f6849a09356ed4bc91c8aa949aee1516fc302
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA512:7b7af2e98493243ffe1934fefff5723b24ae9b9bdc4bf039343ee8456c15acb0ea34e81ec292a41143848272aeca794ef92ad38fc3f42c77465170cb540479ef
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz 27652 SHA512:22d929d8ff17b5edd9767e4c5b32e31d0c6a5fa57b39043c8a1738336ef449324516b0ea8441b2dd7d294651a3de010a71f0a8183feb7a5bda84401879a479f9
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

- `libsm-dev:amd64=2:1.2.2-1`
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

### `dpkg` source package: `libsndfile=1.0.28-4ubuntu0.18.04.1`

Binary Packages:

- `libsndfile1:amd64=1.0.28-4ubuntu0.18.04.1`

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
$ apt-get source -qq --print-uris libsndfile=1.0.28-4ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsndfile/libsndfile_1.0.28-4ubuntu0.18.04.1.dsc' libsndfile_1.0.28-4ubuntu0.18.04.1.dsc 2364 SHA512:4d1e6779ae95d3487b7d02983edc6103b00a7ecb04b6030213f89fe93fb611a41553defb8a115034a2284cd5dd9490c8331e5676b5a8583f4cd3f75d87bb69e4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsndfile/libsndfile_1.0.28.orig.tar.gz' libsndfile_1.0.28.orig.tar.gz 1202833 SHA512:890731a6b8173f714155ce05eaf6d991b31632c8ab207fbae860968861a107552df26fcf85602df2e7f65502c7256c1b41735e1122485a3a07ddb580aa83b57f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsndfile/libsndfile_1.0.28-4ubuntu0.18.04.1.debian.tar.xz' libsndfile_1.0.28-4ubuntu0.18.04.1.debian.tar.xz 15692 SHA512:261a1edb24cbcb2e9803a3fcd2b607c4e57555093c854c89aba04aaba119186b47195f6a0eba69eb8c8475d3cbea01e1bcf4e03faa4d9fe1a78071b48a64bf73
```

### `dpkg` source package: `libsodium=1.0.16-2`

Binary Packages:

- `libsodium23:amd64=1.0.16-2`

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
$ apt-get source -qq --print-uris libsodium=1.0.16-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsodium/libsodium_1.0.16-2.dsc' libsodium_1.0.16-2.dsc 1912 SHA256:5638da6c305cc462a8faef697621bb56d9f90aa2dd01d13dcc73112b3b9ce6de
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsodium/libsodium_1.0.16.orig.tar.gz' libsodium_1.0.16.orig.tar.gz 1571140 SHA256:0c14604bbeab2e82a803215d65c3b6e74bb28291aaee6236d65c699ccfe1a98c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsodium/libsodium_1.0.16-2.debian.tar.xz' libsodium_1.0.16-2.debian.tar.xz 7152 SHA256:76868d50f33869161131b19efa03ea8683f7c38146243fbbf9ad1fd678ccd48a
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
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsoup2.4/libsoup2.4_2.62.1-1ubuntu0.4.dsc' libsoup2.4_2.62.1-1ubuntu0.4.dsc 2825 SHA512:5d3187c3cf3457eed163b85fe4eadcbbf9e4c3e38864eaa273cb4bf787431e0850db31d160b889876b395c494ba0ebd2ae8b650cd543c1dec6842d17e48e8c9e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsoup2.4/libsoup2.4_2.62.1.orig.tar.xz' libsoup2.4_2.62.1.orig.tar.xz 1848776 SHA512:0617abdf41ab339496e81da83ff67e507913ed42ab6ce149afc5dedea74d0118dbaac2913d8ff2875b8842546504b6c0a373e2746e5007a5f4e24197f94b30f5
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsoup2.4/libsoup2.4_2.62.1-1ubuntu0.4.debian.tar.xz' libsoup2.4_2.62.1-1ubuntu0.4.debian.tar.xz 22764 SHA512:2c9e860b577a5a82262fd48f4ae0fbf59cbcff4cca4fa09952b431b310f783084d8c9567552e5a62ca9f695115b517ad531a5fe3d2d5d614735dcc9c38b5fac2
```

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
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsoxr/libsoxr_0.1.2-3.dsc' libsoxr_0.1.2-3.dsc 2170 SHA256:7f6133cee147b7c7d819c6de78541ebedd97cc79a2b66451421d8bea8a9a9d5b
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsoxr/libsoxr_0.1.2.orig.tar.xz' libsoxr_0.1.2.orig.tar.xz 83760 SHA256:54e6f434f1c491388cd92f0e3c47f1ade082cc24327bdc43762f7d1eefe0c275
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsoxr/libsoxr_0.1.2-3.debian.tar.xz' libsoxr_0.1.2-3.debian.tar.xz 4840 SHA256:8c49143d8c600ea024da765049dcddc392d033cea0c43ec4fc27e4c9d0e3d94a
```

### `dpkg` source package: `libssh=0.8.0~20170825.94fa1e38-1ubuntu0.7`

Binary Packages:

- `libssh-gcrypt-4:amd64=0.8.0~20170825.94fa1e38-1ubuntu0.7`

Licenses: (parsed from: `/usr/share/doc/libssh-gcrypt-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.8.0~20170825.94fa1e38-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.8.0~20170825.94fa1e38-1ubuntu0.7.dsc' libssh_0.8.0~20170825.94fa1e38-1ubuntu0.7.dsc 2518 SHA512:310a10f3179034b994048805dfbe1c4a026d7b3466b5bc3816d474d42eb7a3972136fe66801885c9fd568db7cf9c8d9515ce6cfca8b9484ae0036c6439fc2673
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.8.0~20170825.94fa1e38.orig.tar.xz' libssh_0.8.0~20170825.94fa1e38.orig.tar.xz 381176 SHA512:849eb8994361d56391471ef810aca16501fa5609f2c5a1b83bfa2f2ad688c4a5956c1d91c03d6bc6b93ec994ab38e10367ffc7d02c2d5a08f78b03859dcb82e5
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.8.0~20170825.94fa1e38-1ubuntu0.7.debian.tar.xz' libssh_0.8.0~20170825.94fa1e38-1ubuntu0.7.debian.tar.xz 36936 SHA512:60b6efb09514716500a953b8ea356b799c45d1defd13ebf719f44036d1298d5c063c9e12f8189c1916a1a2eef0a35fcb79bfa3c40cb13ecc501f2461c7392ab9
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

### `dpkg` source package: `libtext-iconv-perl=1.7-5build6`

Binary Packages:

- `libtext-iconv-perl=1.7-5build6`

Licenses: (parsed from: `/usr/share/doc/libtext-iconv-perl/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libtext-iconv-perl=1.7-5build6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7-5build6.dsc' libtext-iconv-perl_1.7-5build6.dsc 1841 SHA256:4c645ef83b2a73ee542530651728f9ed3fb3bbd607e4bc7b540b1bb0a6e9d1b8
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7.orig.tar.bz2' libtext-iconv-perl_1.7.orig.tar.bz2 9977 SHA256:815c5169b7afc40bc6f681b4c615ff8fb0e073d87422280c8c759a4666567490
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtext-iconv-perl/libtext-iconv-perl_1.7-5build6.debian.tar.bz2' libtext-iconv-perl_1.7-5build6.debian.tar.bz2 3454 SHA256:747ee5f54cb093e79fa67281b8df1152f0790fadd3ab17c56892de4ca456bde6
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

### `dpkg` source package: `libtheora=1.1.1+dfsg.1-14`

Binary Packages:

- `libtheora0:amd64=1.1.1+dfsg.1-14`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libtheora=1.1.1+dfsg.1-14
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-14.dsc' libtheora_1.1.1+dfsg.1-14.dsc 2592 SHA256:20992f97c4ea622cb2336e6795dd5d816eaf29499ed5278d05dd684218c8e91a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1.orig.tar.gz' libtheora_1.1.1+dfsg.1.orig.tar.gz 2100495 SHA256:c59b0f07a7314dfe2ade15c41bc9f637f8a450fc6b340af61b81760629f28f90
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-14.debian.tar.xz' libtheora_1.1.1+dfsg.1-14.debian.tar.xz 10532 SHA256:51d8d8bc6a613c42857a5c37e93b013e9239c2bb24c24873161adeee08319bc5
```

### `dpkg` source package: `libtie-ixhash-perl=1.23-2`

Binary Packages:

- `libtie-ixhash-perl=1.23-2`

Licenses: (parsed from: `/usr/share/doc/libtie-ixhash-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libtie-ixhash-perl=1.23-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtie-ixhash-perl/libtie-ixhash-perl_1.23-2.dsc' libtie-ixhash-perl_1.23-2.dsc 2144 SHA256:01c7243e392562381da974596b60bbcdacb3afb663ef3757593e8f96df45c113
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtie-ixhash-perl/libtie-ixhash-perl_1.23.orig.tar.gz' libtie-ixhash-perl_1.23.orig.tar.gz 9352 SHA256:fabb0b8c97e67c9b34b6cc18ed66f6c5e01c55b257dcf007555e0b027d4caf56
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtie-ixhash-perl/libtie-ixhash-perl_1.23-2.debian.tar.xz' libtie-ixhash-perl_1.23-2.debian.tar.xz 2036 SHA256:2a80c08ef174e7797b1f32feac55169b9579d6401392703c7989de287234720b
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtimedate-perl/libtimedate-perl_2.3000-2.dsc' libtimedate-perl_2.3000-2.dsc 2136 SHA256:0d7961456d3d45cd1c0e6b4a39ed56290d0722d9e44e3b75645f6608c15455f5
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtimedate-perl/libtimedate-perl_2.3000.orig.tar.gz' libtimedate-perl_2.3000.orig.tar.gz 31109 SHA256:75bd254871cb5853a6aa0403ac0be270cdd75c9d1b6639f18ecba63c15298e86
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtimedate-perl/libtimedate-perl_2.3000-2.debian.tar.xz' libtimedate-perl_2.3000-2.debian.tar.xz 4580 SHA256:092bd262925ed3677fabbfd867ffdc6b5b8ead2ffe2fca912cd20651bca2e2cd
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

### `dpkg` source package: `libtry-tiny-perl=0.30-1`

Binary Packages:

- `libtry-tiny-perl=0.30-1`

Licenses: (parsed from: `/usr/share/doc/libtry-tiny-perl/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libtry-tiny-perl=0.30-1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtry-tiny-perl/libtry-tiny-perl_0.30-1.dsc' libtry-tiny-perl_0.30-1.dsc 2364 SHA256:8739ddcb041194c8a22ba8fdbcf84ccc7faeb414819a608062d19ec4dc4aa998
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtry-tiny-perl/libtry-tiny-perl_0.30.orig.tar.gz' libtry-tiny-perl_0.30.orig.tar.gz 34395 SHA256:da5bd0d5c903519bbf10bb9ba0cb7bcac0563882bcfe4503aee3fb143eddef6b
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtry-tiny-perl/libtry-tiny-perl_0.30-1.debian.tar.xz' libtry-tiny-perl_0.30-1.debian.tar.xz 3532 SHA256:ace34ed42919a033206b51570b96b763f76cff1225685c9da275b57cbf29a9a4
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
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.dsc' libunistring_0.9.9-0ubuntu2.dsc 2006 SHA512:c06c7a7a04dbaef582ed90334e740b70704187df303c033a6298592cdb783f1099ea9a62b787df4b5cbd504ad76f5ff112a3508fda5134b749a25c3222ac9eb1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9.orig.tar.xz' libunistring_0.9.9.orig.tar.xz 2042992 SHA512:c5f3619d0b064c0256dc9326b609cb72871c85102cd67cfc46d85f72b67c564924cd76198c6d6ab60fbf7d6f76ddcb9fbe6c8116f779ca7e24570ae84e31fea8
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.debian.tar.xz' libunistring_0.9.9-0ubuntu2.debian.tar.xz 40424 SHA512:e9c6f76208bef66892b584d83e68b60a05a9cf0b67b1ac10532e996a081319d110a92b440713cb9a46fc45404723a5c81420ede10af2ab8e89432c693db4e1ef
```

### `dpkg` source package: `liburi-perl=1.73-1`

Binary Packages:

- `liburi-perl=1.73-1`

Licenses: (parsed from: `/usr/share/doc/liburi-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris liburi-perl=1.73-1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/liburi-perl/liburi-perl_1.73-1.dsc' liburi-perl_1.73-1.dsc 2218 SHA256:01908a11a130576c562b5a5837b2123ee10b2194eec2d1743d01e188776c7194
'http://archive.ubuntu.com/ubuntu/pool/main/libu/liburi-perl/liburi-perl_1.73.orig.tar.gz' liburi-perl_1.73.orig.tar.gz 106930 SHA256:cca7ab4a6f63f3ccaacae0f2e1337e8edf84137e73f18548ec7d659f23efe413
'http://archive.ubuntu.com/ubuntu/pool/main/libu/liburi-perl/liburi-perl_1.73-1.debian.tar.xz' liburi-perl_1.73-1.debian.tar.xz 5580 SHA256:ae27e0921c94956feb57f94b74ef9c116152be1b028b4ed23ddc02d6213cb288
```

### `dpkg` source package: `libusb-1.0=2:1.0.21-2`

Binary Packages:

- `libusb-1.0-0:amd64=2:1.0.21-2`

Licenses: (parsed from: `/usr/share/doc/libusb-1.0-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libusb-1.0=2:1.0.21-2
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb-1.0/libusb-1.0_1.0.21-2.dsc' libusb-1.0_1.0.21-2.dsc 2067 SHA256:fb8a5cd34d3308652845e054ca97fcd29971cb18659cdb08873d874df1ee8795
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb-1.0/libusb-1.0_1.0.21.orig.tar.bz2' libusb-1.0_1.0.21.orig.tar.bz2 607417 SHA256:7dce9cce9a81194b7065ee912bcd55eeffebab694ea403ffb91b67db66b1824b
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb-1.0/libusb-1.0_1.0.21-2.debian.tar.xz' libusb-1.0_1.0.21-2.debian.tar.xz 13712 SHA256:96da0c02309cfc80de84bbec84a3f63b0571fae83ae1a4d99b361505b959e1eb
```

### `dpkg` source package: `libva=2.1.0-3`

Binary Packages:

- `libva-drm2:amd64=2.1.0-3`
- `libva-x11-2:amd64=2.1.0-3`
- `libva2:amd64=2.1.0-3`
- `va-driver-all:amd64=2.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libva-drm2/copyright`, `/usr/share/doc/libva-x11-2/copyright`, `/usr/share/doc/libva2/copyright`, `/usr/share/doc/va-driver-all/copyright`)

- `Expat`
- `Expat-advertising`
- `GPL-2`
- `GPL-2+`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libva=2.1.0-3
'http://archive.ubuntu.com/ubuntu/pool/universe/libv/libva/libva_2.1.0-3.dsc' libva_2.1.0-3.dsc 2457 SHA256:3bbbb71628354d3b8ed54d1b584fced2275da7999e274734907c146639fde54e
'http://archive.ubuntu.com/ubuntu/pool/universe/libv/libva/libva_2.1.0.orig.tar.bz2' libva_2.1.0.orig.tar.bz2 476977 SHA256:f3fa953a11d3210c3a4ee79031abdbe0863d5ce13d9b3f93f315f1eec60a4b0f
'http://archive.ubuntu.com/ubuntu/pool/universe/libv/libva/libva_2.1.0-3.debian.tar.xz' libva_2.1.0-3.debian.tar.xz 10980 SHA256:610fe4209dda50a4cb3aa28f6f6a6d2c046e4165473b16d8d98d686b2f686294
```

### `dpkg` source package: `libvdpau=1.1.1-3ubuntu1`

Binary Packages:

- `libvdpau1:amd64=1.1.1-3ubuntu1`
- `vdpau-driver-all:amd64=1.1.1-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libvdpau1/copyright`, `/usr/share/doc/vdpau-driver-all/copyright`)

- `Expat`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libvdpau=1.1.1-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvdpau/libvdpau_1.1.1-3ubuntu1.dsc' libvdpau_1.1.1-3ubuntu1.dsc 2429 SHA256:a11d3d368f3686ef488019090abd50bffc180560128778b40ec9a477975743d4
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvdpau/libvdpau_1.1.1.orig.tar.bz2' libvdpau_1.1.1.orig.tar.bz2 429576 SHA256:857a01932609225b9a3a5bf222b85e39b55c08787d0ad427dbd9ec033d58d736
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvdpau/libvdpau_1.1.1-3ubuntu1.debian.tar.xz' libvdpau_1.1.1-3ubuntu1.debian.tar.xz 15708 SHA256:720d7706e6f63dfe360d203c724210588d6ecfc77f2adce95b5d64273311a494
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

### `dpkg` source package: `libvisual=0.4.0-11`

Binary Packages:

- `libvisual-0.4-0:amd64=0.4.0-11`

Licenses: (parsed from: `/usr/share/doc/libvisual-0.4-0/copyright`)

- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libvisual=0.4.0-11
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvisual/libvisual_0.4.0-11.dsc' libvisual_0.4.0-11.dsc 1976 SHA256:b805fcc05a57daf8de43a31368f9a7d2dc0ad2032f7f80aa635680b4517c1ad3
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvisual/libvisual_0.4.0.orig.tar.gz' libvisual_0.4.0.orig.tar.gz 583386 SHA256:0b4dfdb87125e129567752089e3c8b54cefed601eef169d2533d8659da8dc1d7
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvisual/libvisual_0.4.0-11.debian.tar.xz' libvisual_0.4.0-11.debian.tar.xz 18640 SHA256:3f70c27df3b4b7cc075a550dfc6f2383ff93ac955d6a20b54705c5af01757bf4
```

### `dpkg` source package: `libvorbis=1.3.5-4.2`

Binary Packages:

- `libvorbis0a:amd64=1.3.5-4.2`
- `libvorbisenc2:amd64=1.3.5-4.2`
- `libvorbisfile3:amd64=1.3.5-4.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libvorbis=1.3.5-4.2
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvorbis/libvorbis_1.3.5-4.2.dsc' libvorbis_1.3.5-4.2.dsc 2546 SHA256:074430404ed9851708fa99c6028c6419c2eae6d57299e623b443d6079f8b3d87
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvorbis/libvorbis_1.3.5.orig.tar.gz' libvorbis_1.3.5.orig.tar.gz 1638779 SHA256:6efbcecdd3e5dfbf090341b485da9d176eb250d893e3eb378c428a2db38301ce
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvorbis/libvorbis_1.3.5-4.2.debian.tar.xz' libvorbis_1.3.5-4.2.debian.tar.xz 12340 SHA256:22d0f18332c7f5fb06b8366e1653d18165284c07152a3af7872b70cde3a7fdfc
```

### `dpkg` source package: `libvpx=1.7.0-3ubuntu0.18.04.1`

Binary Packages:

- `libvpx5:amd64=1.7.0-3ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libvpx5/copyright`)

- `BSD-3-Clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libvpx=1.7.0-3ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvpx/libvpx_1.7.0-3ubuntu0.18.04.1.dsc' libvpx_1.7.0-3ubuntu0.18.04.1.dsc 2400 SHA512:f12e42e8967faeb4d6662ce6eec8db22cba5ea8aec0c3571a9a5c5e01b829174088c91f55718923cfc74bbf814b15a70c68333d693c1c00459d8f2e161e58b3c
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvpx/libvpx_1.7.0.orig.tar.gz' libvpx_1.7.0.orig.tar.gz 2679797 SHA512:8b3b766b550f8d86907628d7ed88035f9a2612aac21542e0fd5ad35b905eb82cbe1be02a1a24afce7a3bcc4766f62611971f72724761996b392136c40a1e7ff0
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvpx/libvpx_1.7.0-3ubuntu0.18.04.1.debian.tar.xz' libvpx_1.7.0-3ubuntu0.18.04.1.debian.tar.xz 15888 SHA512:0042ff84057f205751f326194415abc2272f215ed0c0604f6574a810e7efcfd33046d3dcebe1bc3960147850328eb7aea776e2af793b05c36c01e3ef116c1fa3
```

### `dpkg` source package: `libwebp=0.6.1-2`

Binary Packages:

- `libwebp6:amd64=0.6.1-2`
- `libwebpmux3:amd64=0.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.6.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.dsc' libwebp_0.6.1-2.dsc 2064 SHA256:321ee69e44f0d037d5fec47692251e35ed22c9ad0bbf0a6bf0fae990a52319f4
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA256:a86045e3ec24704bddbaa369ca30980d6bf4f2625f4cdca03715e91f9c08bbb4
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.debian.tar.xz' libwebp_0.6.1-2.debian.tar.xz 9532 SHA256:5af543e277abb97f6b2c72ca0d7ce95de79108d88da383d511ef729683fa7a45
```

### `dpkg` source package: `libwmf=0.2.8.4-12`

Binary Packages:

- `libwmf0.2-7:amd64=0.2.8.4-12`

Licenses: (parsed from: `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-12
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-12.dsc' libwmf_0.2.8.4-12.dsc 2134 SHA256:cc438ea4b9f9b93d06428989e3920f6e9f1fb317e451aeecbd2b3f608dd82826
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-12.debian.tar.xz' libwmf_0.2.8.4-12.debian.tar.xz 11952 SHA256:579cc19e9199e30b1097559f031a9814f4990206487cb4c402defb68f55be1cd
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

### `dpkg` source package: `libwww-perl=6.31-1ubuntu0.1`

Binary Packages:

- `libwww-perl=6.31-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libwww-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libwww-perl=6.31-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwww-perl/libwww-perl_6.31-1ubuntu0.1.dsc' libwww-perl_6.31-1ubuntu0.1.dsc 2572 SHA512:830b256e3d2e89a41a90fd07dc055648cf073a78b4ce8fd6f7aded45d0dc2a5633405801b1e0cdbe755f7ae5d702bfaa38c260719eee2e56022b9a975c7335d8
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwww-perl/libwww-perl_6.31.orig.tar.gz' libwww-perl_6.31.orig.tar.gz 164626 SHA512:10de1cb2eb8bfc09cc663029a0e58c94a33776515f7d01d2e31bdd060d7124625b4d8151b6beb311ce63b02d59e7912113d054d45f7dbb19963ccd1b3595f1ad
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwww-perl/libwww-perl_6.31-1ubuntu0.1.debian.tar.xz' libwww-perl_6.31-1ubuntu0.1.debian.tar.xz 10436 SHA512:52072b72a68799fdc986da35774ba6da731c6778164af4738670f4dc159726d4a1f3adf4b0c6c242b1ff51579e4815af80487866b2ddea4de5d926ffcca29089
```

### `dpkg` source package: `libwww-robotrules-perl=6.01-1`

Binary Packages:

- `libwww-robotrules-perl=6.01-1`

Licenses: (parsed from: `/usr/share/doc/libwww-robotrules-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libwww-robotrules-perl=6.01-1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwww-robotrules-perl/libwww-robotrules-perl_6.01-1.dsc' libwww-robotrules-perl_6.01-1.dsc 2042 SHA256:d0e32e64b4dbff092769586d1a9773a203e00794bc1de2a255ec0702fac752be
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwww-robotrules-perl/libwww-robotrules-perl_6.01.orig.tar.gz' libwww-robotrules-perl_6.01.orig.tar.gz 9047 SHA256:f817e3e982c9d869c7796bcb5737c3422c2272355424acd162d0f3b132bec9d3
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwww-robotrules-perl/libwww-robotrules-perl_6.01-1.debian.tar.gz' libwww-robotrules-perl_6.01-1.debian.tar.gz 1777 SHA256:c45a0b249556578ddbbbe84ac13a2dddc3045cde0c7307427975cd92cd0b5a41
```

### `dpkg` source package: `libx11-protocol-perl=0.56-7`

Binary Packages:

- `libx11-protocol-perl=0.56-7`

Licenses: (parsed from: `/usr/share/doc/libx11-protocol-perl/copyright`)

- `Artistic`
- `Expat`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libx11-protocol-perl=0.56-7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11-protocol-perl/libx11-protocol-perl_0.56-7.dsc' libx11-protocol-perl_0.56-7.dsc 2267 SHA256:49322d7a9aa54245b10c96daebeebd16924edc4459526637b4d809335876b3b3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11-protocol-perl/libx11-protocol-perl_0.56.orig.tar.gz' libx11-protocol-perl_0.56.orig.tar.gz 101227 SHA256:de96dd6c7c1f25f3287aa7af64902bf84acaaa8e0c3bb76aa1676367e04a08b7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11-protocol-perl/libx11-protocol-perl_0.56-7.debian.tar.xz' libx11-protocol-perl_0.56-7.debian.tar.xz 4348 SHA256:07a1bc718bc433d858c8b997300c41dfec7c0a4ba458977761a1e3549a75674f
```

### `dpkg` source package: `libx11=2:1.6.4-3ubuntu0.2`

Binary Packages:

- `libx11-6:amd64=2:1.6.4-3ubuntu0.2`
- `libx11-data=2:1.6.4-3ubuntu0.2`
- `libx11-dev:amd64=2:1.6.4-3ubuntu0.2`
- `libx11-doc=2:1.6.4-3ubuntu0.2`
- `libx11-xcb1:amd64=2:1.6.4-3ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libxau=1:1.0.8-1ubuntu1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.8-1ubuntu1`
- `libxau6:amd64=1:1.0.8-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1ubuntu1.dsc' libxau_1.0.8-1ubuntu1.dsc 2099 SHA512:944a2481ac5927b7dd649afe7f1f88493499a4de019ac9ef6f0c94f305aedf7695de86935f02610069ef84c0bec56db66357472f773fc9807616b2f4e92f296e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA512:3bdd9c1a491f00000dd891577493803bac3f80d0e61acb28eb2bcb50b8923e6d4540ffc4422bc0f6af8a0d20c5a75d53eedbdef177c25332f970542ea440c5d9
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1ubuntu1.diff.gz' libxau_1.0.8-1ubuntu1.diff.gz 15803 SHA512:c22f2fee07349c910f3d461d1718672ee72fd37b9668e869a7d92b984a3b158034615bf64c9480b995156ef96faa66e0107db50f2fa6fcd6f56da7911bdc8dc7
```

### `dpkg` source package: `libxaw=2:1.0.13-1`

Binary Packages:

- `libxaw7:amd64=2:1.0.13-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxaw=2:1.0.13-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxaw/libxaw_1.0.13-1.dsc' libxaw_1.0.13-1.dsc 2196 SHA256:9fdf48f9ff66c0889cda5030997fe919e5320e7988f32e20bb96602daa37e7f7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxaw/libxaw_1.0.13.orig.tar.gz' libxaw_1.0.13.orig.tar.gz 848997 SHA256:7e74ac3e5f67def549722ff0333d6e6276b8becd9d89615cda011e71238ab694
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxaw/libxaw_1.0.13-1.diff.gz' libxaw_1.0.13-1.diff.gz 12643 SHA256:241f21ba0810d9d859a98ab60f100a366bc9e98cd946c736566a8ed1353a1bcc
```

### `dpkg` source package: `libxcb=1.13-2~ubuntu18.04`

Binary Packages:

- `libxcb-dri2-0:amd64=1.13-2~ubuntu18.04`
- `libxcb-dri3-0:amd64=1.13-2~ubuntu18.04`
- `libxcb-glx0:amd64=1.13-2~ubuntu18.04`
- `libxcb-present0:amd64=1.13-2~ubuntu18.04`
- `libxcb-render0:amd64=1.13-2~ubuntu18.04`
- `libxcb-shape0:amd64=1.13-2~ubuntu18.04`
- `libxcb-shm0:amd64=1.13-2~ubuntu18.04`
- `libxcb-sync1:amd64=1.13-2~ubuntu18.04`
- `libxcb-xfixes0:amd64=1.13-2~ubuntu18.04`
- `libxcb1:amd64=1.13-2~ubuntu18.04`
- `libxcb1-dev:amd64=1.13-2~ubuntu18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.13-2~ubuntu18.04
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13-2~ubuntu18.04.dsc' libxcb_1.13-2~ubuntu18.04.dsc 4762 SHA512:034d032bcbbaa311b44eb0c01a7eefbf671644e3a3f8b1f5c001bf80df45120cc85ba25e8453b66a691751eebf2e21ed93af976471efa824b1d83b33a4f3769b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13.orig.tar.gz' libxcb_1.13.orig.tar.gz 632493 SHA512:28e1db6f1981bef25007c98ba28f4c2a4d285af1aadd43ced631d630abab90ade055f125d5e384b6ff1e5ef8e31a745f53a77d61d862a6e3b7a64c52b749bc02
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13-2~ubuntu18.04.diff.gz' libxcb_1.13-2~ubuntu18.04.diff.gz 25267 SHA512:fd19a1c6a8f6ebf362e871e814455b7cc2d63ffa63f0d47cdc035a3d5bc4b4076a4dc487dfead4d40605a4fa330134eeceb0a3acfc760579de2e2380d3b97b01
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

- `libxdmcp-dev:amd64=1:1.1.2-3`
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
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxkbcommon/libxkbcommon_0.8.2-1~ubuntu18.04.1.dsc' libxkbcommon_0.8.2-1~ubuntu18.04.1.dsc 2178 SHA512:7ffcfd8b44df0c4c9e139e26682ce3187b14445f59235b7eea88c93194d86d451444e5d6715251e49565dc0c0987a4d044cbd889ad74547de525da2ff371f955
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxkbcommon/libxkbcommon_0.8.2-1~ubuntu18.04.1.tar.gz' libxkbcommon_0.8.2-1~ubuntu18.04.1.tar.gz 615081 SHA512:df4478194169c2f6abc43965be2ff0ceae06d37cc11b7bcdb26909b7bcf7b7eca6e933ce3921e4a926335aca94865231fb1a310483c7f59bd1eee2347b470180
```

### `dpkg` source package: `libxml-parser-perl=2.44-2build3`

Binary Packages:

- `libxml-parser-perl=2.44-2build3`

Licenses: (parsed from: `/usr/share/doc/libxml-parser-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libxml-parser-perl=2.44-2build3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-parser-perl/libxml-parser-perl_2.44-2build3.dsc' libxml-parser-perl_2.44-2build3.dsc 2126 SHA256:948ec705fedc0a9568a594dddb3d8a290e2e5e0e7f972ea76429ba530f38af1c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-parser-perl/libxml-parser-perl_2.44.orig.tar.gz' libxml-parser-perl_2.44.orig.tar.gz 237377 SHA256:1ae9d07ee9c35326b3d9aad56eae71a6730a73a116b9fe9e8a4758b7cc033216
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-parser-perl/libxml-parser-perl_2.44-2build3.debian.tar.xz' libxml-parser-perl_2.44-2build3.debian.tar.xz 57564 SHA256:65329000c1a7e6e26d72749f25ab44c4cbc097619863f2e1b776ba127b605880
```

### `dpkg` source package: `libxml-twig-perl=1:3.50-1`

Binary Packages:

- `libxml-twig-perl=1:3.50-1`

Licenses: (parsed from: `/usr/share/doc/libxml-twig-perl/copyright`)

- `Artistic`
- `GPL`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libxml-twig-perl=1:3.50-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-twig-perl/libxml-twig-perl_3.50-1.dsc' libxml-twig-perl_3.50-1.dsc 2130 SHA256:a3ff074183a29e1c93d19a674d84a5d80b11c7d11e002c02ab613e12ff9cedb2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-twig-perl/libxml-twig-perl_3.50.orig.tar.gz' libxml-twig-perl_3.50.orig.tar.gz 403387 SHA256:62005aced4e844651d75c2a54c2dcd8df5e32447d0b8e449c40cf6f83f382b80
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-twig-perl/libxml-twig-perl_3.50-1.debian.tar.xz' libxml-twig-perl_3.50-1.debian.tar.xz 6276 SHA256:5de42e4e4c74f601ca8d5462df8be7f72ef257fc1f869f9403fef31e043cc1f4
```

### `dpkg` source package: `libxml-xpathengine-perl=0.14-1`

Binary Packages:

- `libxml-xpathengine-perl=0.14-1`

Licenses: (parsed from: `/usr/share/doc/libxml-xpathengine-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris libxml-xpathengine-perl=0.14-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-xpathengine-perl/libxml-xpathengine-perl_0.14-1.dsc' libxml-xpathengine-perl_0.14-1.dsc 2232 SHA256:f5e132c7f5f1f8bd2616ba48f03bb12826ca3b8a6223c72237a815b207394d47
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-xpathengine-perl/libxml-xpathengine-perl_0.14.orig.tar.gz' libxml-xpathengine-perl_0.14.orig.tar.gz 26118 SHA256:d2fe7bcbbd0beba1444f4a733401e7b8aa5282fad4266d42735dd74582b2e264
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml-xpathengine-perl/libxml-xpathengine-perl_0.14-1.debian.tar.xz' libxml-xpathengine-perl_0.14-1.debian.tar.xz 4680 SHA256:2e66d2548a546d97963344a04a4b8ffedc3a5206f04ca7900eba0ee49760401e
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
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc 3151 SHA512:77290cb3d711257c73e68521ded224dab4d1343a39474b6ebc849cfb90890d549a7ef475b2e3b2f6a8c46f8142b3bd3ed6aff69a13bca174f9310f6f643744a5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA512:c921697db38b530b1a088636cb31226bbe9df8c9e9c83316ce53770f9bd2faeef360d5f526f34e00cd778150c408e8d91b99a67a5f5030a8b279961ff9299ae5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz 39680 SHA512:532f5357a6ec1e2b31634166dd9ba42f6d7337a2daa743b657e2e61d325306b1857503d3e877a28417388746ecf70c4e17e9515c7709d2ccae4e1221bfa87a87
```

### `dpkg` source package: `libxmu=2:1.1.2-2`

Binary Packages:

- `libxmu6:amd64=2:1.1.2-2`
- `libxmuu1:amd64=2:1.1.2-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxmu=2:1.1.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.2-2.dsc' libxmu_1.1.2-2.dsc 2291 SHA256:5e3333a3fe9dbed9d0df596d964b94aa1d45d56a0475a8b66b3f69d60ab29504
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.2.orig.tar.gz' libxmu_1.1.2.orig.tar.gz 469019 SHA256:e5fd4bacef068f9509b8226017205040e38d3fba8d2de55037200e7176c13dba
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.2-2.diff.gz' libxmu_1.1.2-2.diff.gz 6054 SHA256:c01cbd09a15e71c0418d2689a0fd0b946bf4e40d1dbe9f594beb00a4818f0740
```

### `dpkg` source package: `libxpm=1:3.5.12-1`

Binary Packages:

- `libxpm4:amd64=1:3.5.12-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxpm=1:3.5.12-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.12-1.dsc' libxpm_3.5.12-1.dsc 2061 SHA256:1b5d07d820d656030d0f79a15a0652f258c9d2be0cd6064ec37c40853906f7e8
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.12.orig.tar.gz' libxpm_3.5.12.orig.tar.gz 529302 SHA256:2523acc780eac01db5163267b36f5b94374bfb0de26fc0b5a7bee76649fd8501
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.12-1.diff.gz' libxpm_3.5.12-1.diff.gz 9458 SHA256:4103400f8d73d0ec567f87e8aa9824c4a07d068e81da6efe54fb535ec897e326
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

### `dpkg` source package: `libxshmfence=1.3-1`

Binary Packages:

- `libxshmfence1:amd64=1.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxshmfence=1.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.3-1.dsc' libxshmfence_1.3-1.dsc 2096 SHA256:7da3e1195622ab34427bd5d09167b1f44ed1a3e828782fa8e618f1181c56194a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.3.orig.tar.gz' libxshmfence_1.3.orig.tar.gz 378960 SHA256:7eb3d46ad91bab444f121d475b11b39273142d090f7e9ac43e6a87f4ff5f902c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.3-1.diff.gz' libxshmfence_1.3-1.diff.gz 17456 SHA256:85422af90300523b8fb27e697b59418f18bd7cd5c849161fd0be64c91ce94698
```

### `dpkg` source package: `libxslt=1.1.29-5ubuntu0.2`

Binary Packages:

- `libxslt1.1:amd64=1.1.29-5ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.29-5ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.dsc' libxslt_1.1.29-5ubuntu0.2.dsc 2502 SHA512:4998aeb5983f23bbbd6e93f931b0d4c29cf71ccaee8b08edf477184184fce12791389e0d465784b38855b4587efb0833b084fc1be056ce61153b77115da0e40a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29.orig.tar.gz' libxslt_1.1.29.orig.tar.gz 3428524 SHA512:a1ce555a74a9dabe65e8f64bb66e27e77760fd76940d88f2d59f58dd63ca73c8ae59f3fcbd8e76c8f92ff992fb0c09328528c20ea38ccac83e63252106bf5f31
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.debian.tar.xz' libxslt_1.1.29-5ubuntu0.2.debian.tar.xz 36520 SHA512:4edcdbc3b2cf8c35fa7e56f7b535f7685e55a88892494abf7d6720727f8ed142a29ac1db8ada894fccfee7fc75786af56e2cf8c4c5e61c1c1c1a0694846624bb
```

### `dpkg` source package: `libxss=1:1.2.2-1`

Binary Packages:

- `libxss1:amd64=1:1.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxss=1:1.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxss/libxss_1.2.2-1.dsc' libxss_1.2.2-1.dsc 2042 SHA256:22379490d80d7661c793f0f016a5e12255fdb53a0b2b58b6fe14afa805fcac3f
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxss/libxss_1.2.2.orig.tar.gz' libxss_1.2.2.orig.tar.gz 348915 SHA256:e12ba814d44f7b58534c0d8521e2d4574f7bf2787da405de4341c3b9f4cc8d96
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxss/libxss_1.2.2-1.diff.gz' libxss_1.2.2-1.diff.gz 14712 SHA256:fcc9c125f3af01da27f6cee798410a7907a63802f5c6360f972e12b1ff59e6c1
```

### `dpkg` source package: `libxt=1:1.1.5-1`

Binary Packages:

- `libxt-dev:amd64=1:1.1.5-1`
- `libxt6:amd64=1:1.1.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.1.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5-1.dsc' libxt_1.1.5-1.dsc 2109 SHA256:f44ae1393c9fd02c0b3dd03576c7b26e6c7b09de3271a87e018efadeed311639
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5.orig.tar.gz' libxt_1.1.5.orig.tar.gz 962169 SHA256:b59bee38a9935565fa49dc1bfe84cb30173e2e07e1dcdf801430d4b54eb0caa3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5-1.diff.gz' libxt_1.1.5-1.diff.gz 14462 SHA256:822fe813d1ea9213e6fde91cbb607c0b6874341dc19b77b0f6649b8be8472d82
```

### `dpkg` source package: `libxtst=2:1.2.3-1`

Binary Packages:

- `libxtst6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxtst=2:1.2.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxtst/libxtst_1.2.3-1.dsc' libxtst_1.2.3-1.dsc 2243 SHA256:979f05e505ea319c3f75955e10345338f77a512f5a6a0a887d6f4633d6bd4633
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxtst/libxtst_1.2.3.orig.tar.gz' libxtst_1.2.3.orig.tar.gz 400197 SHA256:a0c83acce02d4923018c744662cb28eb0dbbc33b4adc027726879ccf68fbc2c2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxtst/libxtst_1.2.3-1.diff.gz' libxtst_1.2.3-1.diff.gz 10177 SHA256:c4739fc7ccda7caaffcf36f934b7c33463390e71d567c7d62f635db1946b74ed
```

### `dpkg` source package: `libxv=2:1.0.11-1`

Binary Packages:

- `libxv1:amd64=2:1.0.11-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxv=2:1.0.11-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxv/libxv_1.0.11-1.dsc' libxv_1.0.11-1.dsc 1959 SHA256:7753e8d4496ec0d3f32417b03cfc8b344e2dff486e46f630158a6a52e4bd8542
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxv/libxv_1.0.11.orig.tar.gz' libxv_1.0.11.orig.tar.gz 387057 SHA256:c4112532889b210e21cf05f46f0f2f8354ff7e1b58061e12d7a76c95c0d47bb1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxv/libxv_1.0.11-1.diff.gz' libxv_1.0.11-1.diff.gz 8235 SHA256:529ed2bcbccc9340c9c7987e8c5ed933a0fa41d6e4e67ef71ce3925ac83d93b6
```

### `dpkg` source package: `libxxf86dga=2:1.1.4-1`

Binary Packages:

- `libxxf86dga1:amd64=2:1.1.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxxf86dga=2:1.1.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86dga/libxxf86dga_1.1.4-1.dsc' libxxf86dga_1.1.4-1.dsc 2138 SHA256:606798052db5dc7d2061652503295e303318162d38acbf9894fb1fec991d2c34
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86dga/libxxf86dga_1.1.4.orig.tar.gz' libxxf86dga_1.1.4.orig.tar.gz 358963 SHA256:e6361620a15ceba666901ca8423e8be0c6ed0271a7088742009160349173766b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86dga/libxxf86dga_1.1.4-1.diff.gz' libxxf86dga_1.1.4-1.diff.gz 14920 SHA256:82ad91f1b56bdd3875fd1cad2c3a7b0b99cdf3106391df370367579935471fe9
```

### `dpkg` source package: `libxxf86vm=1:1.1.4-1`

Binary Packages:

- `libxxf86vm1:amd64=1:1.1.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxxf86vm=1:1.1.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.dsc' libxxf86vm_1.1.4-1.dsc 2078 SHA256:5a3aded030a415b0d6c201d2b9d3af36f241dc981f10052fd4c2b56d59597838
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4.orig.tar.gz' libxxf86vm_1.1.4.orig.tar.gz 363146 SHA256:5108553c378a25688dcb57dca383664c36e293d60b1505815f67980ba9318a99
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.diff.gz' libxxf86vm_1.1.4-1.diff.gz 8040 SHA256:e0f11739d28c7a4475820ebda26e6f29e6cfa80b99a3513c075471132c81725b
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
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.dsc' libzstd_1.3.3+dfsg-2ubuntu1.1.dsc 2390 SHA512:8b0c42432f98edf887951e95964acd710e284f0a458b9f05be1ca1428c7c4d491547ee791f0f6c3f854dea057800b716799b69eecfc42d011c6898345570e7d1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg.orig.tar.xz' libzstd_1.3.3+dfsg.orig.tar.xz 1333584 SHA512:40f66d34247f549b6861677a520bdce722036c49bc78096981b3b6b4cbb798780c6afccaff18e843016ec7aab55b8bb3ce3ddbfb089efb5d83028058df5e755c
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz' libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz 12808 SHA512:ae7a558e5ad31ac579856d0ca7f941f95ef570b8b6612249f3f932d85310d56ef7cc4deba4d7ff3a14e46fea25e1eb663b8b841ba4442aa4f7bbe3f2961c3993
```

### `dpkg` source package: `llvm-toolchain-10=1:10.0.0-4ubuntu1~18.04.2`

Binary Packages:

- `libllvm10:amd64=1:10.0.0-4ubuntu1~18.04.2`

Licenses: (parsed from: `/usr/share/doc/libllvm10/copyright`)

- `APACHE-2-LLVM-EXCEPTIONS`
- `Apache-2.0`
- `BSD-3-Clause`
- `BSD-3-clause`
- `MIT`
- `Python`
- `solar-public-domain`

Source:

```console
$ apt-get source -qq --print-uris llvm-toolchain-10=1:10.0.0-4ubuntu1~18.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-10/llvm-toolchain-10_10.0.0-4ubuntu1~18.04.2.dsc' llvm-toolchain-10_10.0.0-4ubuntu1~18.04.2.dsc 5754 SHA512:f90ee3293a09e01758c79eb0a91906322ff12f05401022c61325659409f6bbc109a0beefa192aeed64412ab24db3a2e417c6083ff4b37a5f7f9705b92944cb68
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-10/llvm-toolchain-10_10.0.0.orig.tar.xz' llvm-toolchain-10_10.0.0.orig.tar.xz 78321340 SHA512:7d2111510daf52ad085df9876c993b550e252b2a0ed2153fd45de1465fc2a38a798e7b1418dd750e84315ffce39d4439069510483bae44f4878fcc68e4823865
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-10/llvm-toolchain-10_10.0.0-4ubuntu1~18.04.2.debian.tar.xz' llvm-toolchain-10_10.0.0-4ubuntu1~18.04.2.debian.tar.xz 138936 SHA512:6c9b93289e077cf4ec717ff1d022c96f25a62f83cf3ce627eadec26fa155d4bf4c0b811eb9f53d3d0ce77f18acbd54c516f6574c6473406eae32dea770cb75dc
```

### `dpkg` source package: `lm-sensors=1:3.4.0-4`

Binary Packages:

- `libsensors4:amd64=1:3.4.0-4`

Licenses: (parsed from: `/usr/share/doc/libsensors4/copyright`)

- `GPL`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lm-sensors=1:3.4.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0-4.dsc' lm-sensors_3.4.0-4.dsc 1931 SHA256:7561ac7777dd40644ffd227431dac87f7f52e88c4bfc02d72b7ce42d448aeeff
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0.orig.tar.bz2' lm-sensors_3.4.0.orig.tar.bz2 175802 SHA256:e0579016081a262dd23eafe1d22b41ebde78921e73a1dcef71e05e424340061f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0-4.debian.tar.xz' lm-sensors_3.4.0-4.debian.tar.xz 26436 SHA256:f52640bffc525a3b4cb46e66acb2511e38a2bc64ce33a5021771ad86d77aae23
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

### `dpkg` source package: `mesa=20.0.8-0ubuntu1~18.04.1`

Binary Packages:

- `libegl-mesa0:amd64=20.0.8-0ubuntu1~18.04.1`
- `libgbm1:amd64=20.0.8-0ubuntu1~18.04.1`
- `libgl1-mesa-dri:amd64=20.0.8-0ubuntu1~18.04.1`
- `libgl1-mesa-glx:amd64=20.0.8-0ubuntu1~18.04.1`
- `libglapi-mesa:amd64=20.0.8-0ubuntu1~18.04.1`
- `libglx-mesa0:amd64=20.0.8-0ubuntu1~18.04.1`
- `mesa-va-drivers:amd64=20.0.8-0ubuntu1~18.04.1`
- `mesa-vdpau-drivers:amd64=20.0.8-0ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/libegl-mesa0/copyright`, `/usr/share/doc/libgbm1/copyright`, `/usr/share/doc/libgl1-mesa-dri/copyright`, `/usr/share/doc/libgl1-mesa-glx/copyright`, `/usr/share/doc/libglapi-mesa/copyright`, `/usr/share/doc/libglx-mesa0/copyright`, `/usr/share/doc/mesa-va-drivers/copyright`, `/usr/share/doc/mesa-vdpau-drivers/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-google`
- `BSL`
- `GPL`
- `Khronos`
- `MIT`
- `MLAA`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris mesa=20.0.8-0ubuntu1~18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_20.0.8-0ubuntu1~18.04.1.dsc' mesa_20.0.8-0ubuntu1~18.04.1.dsc 5293 SHA512:c2149b9557227aa1c5fdfaddf62b000feb039a42b326e6b390d546713e3e1ec7fd438eb815d309f202124e39b5c4c876ecd3e30f870ab870daa65872c95ec84f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_20.0.8.orig.tar.gz' mesa_20.0.8.orig.tar.gz 19030315 SHA512:d6a0365c8248c704548d74d6035da43a0791f3306176e873f7929ae34ac2254370190c6cd40cf5e8bfc2455dfbc02f40569a9b12c4b18c2048b29e635427cd53
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_20.0.8-0ubuntu1~18.04.1.diff.gz' mesa_20.0.8-0ubuntu1~18.04.1.diff.gz 118306 SHA512:cba9931b5cd76a3e5300e1201d5f99e6f7893ff612f3ce36c9f33973c7bbc041dc4bb3d433f2dfdc9dcfb2ab48ada45a49b432b62b34a75ba030121e3f3cf2d9
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

### `dpkg` source package: `mpclib3=1.1.0-1`

Binary Packages:

- `libmpc3:amd64=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.1.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0-1.dsc' mpclib3_1.1.0-1.dsc 1990 SHA256:bb57824015b735bf72399a53f8c6a241e6a8bd402753b0fdcdaa5b99d0aef790
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0.orig.tar.gz' mpclib3_1.1.0.orig.tar.gz 701263 SHA256:6985c538143c1208dcb1ac42cedad6ff52e267b47e5f970183a3e75125b43c2e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0-1.diff.gz' mpclib3_1.1.0-1.diff.gz 3794 SHA256:84b10a4ae958b3015e136b75be5fee22961255d19be655f7d0adae8d4f3bc977
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

### `dpkg` source package: `mpfr4=4.0.1-1`

Binary Packages:

- `libmpfr6:amd64=4.0.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.0.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1-1.dsc' mpfr4_4.0.1-1.dsc 1972 SHA256:85d8dad92d3f9ace96ac78b2f4ec00eafef228fa53e0344ae4255fc4d3f75626
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1.orig.tar.xz' mpfr4_4.0.1.orig.tar.xz 1412692 SHA256:67874a60826303ee2fb6affc6dc0ddd3e749e9bfcb4c8655e3953d0458a6e16e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1-1.debian.tar.xz' mpfr4_4.0.1-1.debian.tar.xz 10460 SHA256:9e0d582dea7e88958b8bc1f3782ada59b9c7175f01b4e06e8487fc6cbfc5a2d7
```

### `dpkg` source package: `mpg123=1.25.10-1`

Binary Packages:

- `libmpg123-0:amd64=1.25.10-1`

Licenses: (parsed from: `/usr/share/doc/libmpg123-0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpg123=1.25.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpg123/mpg123_1.25.10-1.dsc' mpg123_1.25.10-1.dsc 2523 SHA256:48a7cc9cb104758592d6505204eb86a0109268f33270ce9dcaa4a05d9957b4f8
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpg123/mpg123_1.25.10.orig.tar.bz2' mpg123_1.25.10.orig.tar.bz2 921219 SHA256:6c1337aee2e4bf993299851c70b7db11faec785303cfca3a5c3eb5f329ba7023
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpg123/mpg123_1.25.10.orig.tar.bz2.asc' mpg123_1.25.10.orig.tar.bz2.asc 847 SHA256:4ea1ac82c47b21f3fb353b8f11040abba8529b0e6f4a50a87e18f68b87b71530
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpg123/mpg123_1.25.10-1.debian.tar.xz' mpg123_1.25.10-1.debian.tar.xz 23548 SHA256:32c68939ff1635124cb5b0c1708c8c420475726e8cb8e5822b8fec97d5266bbb
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
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.dsc' ncurses_6.1-1ubuntu1.18.04.dsc 4702 SHA512:e998c05380a2599d3f37572e720ab60854a1c83bacdf921372767e320d4063c2af611d45409201dbc77e6c6b981537eec246f46326bae6a69536ddf974007ab1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz' ncurses_6.1.orig.tar.gz 3365395 SHA512:e308af43f8b7e01e98a55f4f6c4ee4d1c39ce09d95399fa555b3f0cdf5fd0db0f4c4d820b4af78a63f6cf6d8627587114a40af48cfc066134b600520808a77ee
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz.asc' ncurses_6.1.orig.tar.gz.asc 251 SHA512:53659ddf0890683f1d9bf895d7d5b0693d95e102cde4440685a3d0c97230c4930203a9383bd9833ba4639713a12b0afd2b3ebecd9fa5640fb6f2b5fa8e662441
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.debian.tar.xz' ncurses_6.1-1ubuntu1.18.04.debian.tar.xz 57464 SHA512:ec0211e25ecc865296afd54eeae8314718ca2d443936e016dd74dacfaa1f1de79778b1d50fe9377488f07e40fce82ed367348db30889757efd1db4f96630a6fa
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
'http://archive.ubuntu.com/ubuntu/pool/main/n/neon27/neon27_0.30.2-3~ubuntu18.04.1.dsc' neon27_0.30.2-3~ubuntu18.04.1.dsc 2321 SHA512:64a6481fad715a36670089083c1d350adb239159383d8d117af01ae0dfffb7907261c8c92d3eb5b9052a5cbbe63ad4e6af08bfbacb76963b3cdbcad384a0472b
'http://archive.ubuntu.com/ubuntu/pool/main/n/neon27/neon27_0.30.2.orig.tar.gz' neon27_0.30.2.orig.tar.gz 932779 SHA512:634caf87522e0bd2695c6fba39cae2465e403f9fbd8007eb10e4e035c765d24cb8da932c67bfa35c34aa51b90c7bc7037ebebaa1ec43259366d5d07233efc631
'http://archive.ubuntu.com/ubuntu/pool/main/n/neon27/neon27_0.30.2-3~ubuntu18.04.1.debian.tar.xz' neon27_0.30.2-3~ubuntu18.04.1.debian.tar.xz 12664 SHA512:1d24cd9a09d696e2a2cbd4bbbc02ee98b808e2cee4f911b9239e036dae4be4e117ed3f5e84e695ea2562af3befb60269fdc9be6c26a61a033bef26395ae273a2
```

### `dpkg` source package: `net-tools=1.60+git20161116.90da8a0-1ubuntu1`

Binary Packages:

- `net-tools=1.60+git20161116.90da8a0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/net-tools/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris net-tools=1.60+git20161116.90da8a0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/net-tools/net-tools_1.60+git20161116.90da8a0-1ubuntu1.dsc' net-tools_1.60+git20161116.90da8a0-1ubuntu1.dsc 2238 SHA256:3bb1d688e196fd07984fa81c4dd199b7f0eff8ea51278d16aa2f865695f62e82
'http://archive.ubuntu.com/ubuntu/pool/main/n/net-tools/net-tools_1.60+git20161116.90da8a0.orig.tar.gz' net-tools_1.60+git20161116.90da8a0.orig.tar.gz 288190 SHA256:d3c25c4b70541bb2bb54ebb21e2443811cfd1cbbf4c357d0e960e2973bc4192a
'http://archive.ubuntu.com/ubuntu/pool/main/n/net-tools/net-tools_1.60+git20161116.90da8a0-1ubuntu1.debian.tar.xz' net-tools_1.60+git20161116.90da8a0-1ubuntu1.debian.tar.xz 58348 SHA256:10817a37cb0c45cc0002320fb6d901e873c0e341a9f583b6313a54b3e26e6086
```

### `dpkg` source package: `netbase=5.4`

Binary Packages:

- `netbase=5.4`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.4
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.4.dsc' netbase_5.4.dsc 1326 SHA256:ebe29d45e65b661d64636cbce3840997d8079cf338efbfa347b4c73ed2831b7b
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.4.tar.xz' netbase_5.4.tar.xz 31524 SHA256:66ff73d2d162e2d49db43988d8b8cd328cf7fffca042db73397f14c71825e80d
```

### `dpkg` source package: `netpbm-free=2:10.0-15.3build1`

Binary Packages:

- `libnetpbm10=2:10.0-15.3build1`
- `netpbm=2:10.0-15.3build1`

Licenses: (parsed from: `/usr/share/doc/libnetpbm10/copyright`, `/usr/share/doc/netpbm/copyright`)

- `BSD`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris netpbm-free=2:10.0-15.3build1
'http://archive.ubuntu.com/ubuntu/pool/main/n/netpbm-free/netpbm-free_10.0-15.3build1.dsc' netpbm-free_10.0-15.3build1.dsc 2184 SHA256:57100bdb3b2fc0c357d966979ff9b677a0d772ef5db67368076ec0118ebf8981
'http://archive.ubuntu.com/ubuntu/pool/main/n/netpbm-free/netpbm-free_10.0.orig.tar.gz' netpbm-free_10.0.orig.tar.gz 1926538 SHA256:ea3a653f3e5a32e09cea903c5861138f6a597670dff79e2b54e902f140cff2f3
'http://archive.ubuntu.com/ubuntu/pool/main/n/netpbm-free/netpbm-free_10.0-15.3build1.diff.gz' netpbm-free_10.0-15.3build1.diff.gz 72115 SHA256:fb187f41d676e9ec20d1f48c32738726bc13826ce068de47666fd3b3098eef9f
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

### `dpkg` source package: `norm=1.5r6+dfsg1-6`

Binary Packages:

- `libnorm1:amd64=1.5r6+dfsg1-6`

Licenses: (parsed from: `/usr/share/doc/libnorm1/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause-UC`
- `NRL-2-clause`
- `NRL-3-clause`

Source:

```console
$ apt-get source -qq --print-uris norm=1.5r6+dfsg1-6
'http://archive.ubuntu.com/ubuntu/pool/universe/n/norm/norm_1.5r6+dfsg1-6.dsc' norm_1.5r6+dfsg1-6.dsc 1534 SHA256:e8cab4884a245691d9ef6a24254560cc7abc8d3600c00219f10da836648aba24
'http://archive.ubuntu.com/ubuntu/pool/universe/n/norm/norm_1.5r6+dfsg1.orig.tar.gz' norm_1.5r6+dfsg1.orig.tar.gz 2132249 SHA256:bb63051fb03cde826be4548f157bfbd18525829f8f97870bf94a00be8cae6bed
'http://archive.ubuntu.com/ubuntu/pool/universe/n/norm/norm_1.5r6+dfsg1-6.debian.tar.xz' norm_1.5r6+dfsg1-6.debian.tar.xz 6780 SHA256:d80cd4ebacc76e1506c3b9025f4e382ba8878e2a41c563cbc0b31b8c9a586a06
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


### `dpkg` source package: `numactl=2.0.11-2.1ubuntu0.1`

Binary Packages:

- `libnuma1:amd64=2.0.11-2.1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.11-2.1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-2.1ubuntu0.1.dsc' numactl_2.0.11-2.1ubuntu0.1.dsc 1970 SHA512:ef9adf0b792d712b56903cbb9b9bbc7b0ff8b0b42c836fe52595befbf1412251dcefb6fce0db039a5501b41463d1152046ad11477b332590560c44e669da0f2f
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11.orig.tar.gz' numactl_2.0.11.orig.tar.gz 408175 SHA512:1969d7ee0ff3de0d6f1fa42ec089a17cdb3f92cb35d453b8f8b2eec49724c43787ecbd213357013a8f2500a260b0df9844d515815ca3a0376314a0eed050a0d4
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-2.1ubuntu0.1.debian.tar.xz' numactl_2.0.11-2.1ubuntu0.1.debian.tar.xz 9504 SHA512:a389644eac8e9ddaa9c644d9c3fff01f1bd4c5e0f2b4da7593806846fd5d288af44e559a8eb48a720003e62141924f96b654b0a4adda846947ac5e0601892961
```

### `dpkg` source package: `openal-soft=1:1.18.2-2`

Binary Packages:

- `libopenal-data=1:1.18.2-2`
- `libopenal1:amd64=1:1.18.2-2`

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
$ apt-get source -qq --print-uris openal-soft=1:1.18.2-2
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openal-soft/openal-soft_1.18.2-2.dsc' openal-soft_1.18.2-2.dsc 2384 SHA256:6479b896fb3f1cab9df0b0a719d18caec33ffd05714c705c119989b4d109e6c9
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openal-soft/openal-soft_1.18.2.orig.tar.gz' openal-soft_1.18.2.orig.tar.gz 775095 SHA256:a598241d1af2e90c25a1b91da4c9ddc0e7cb6a4b5f1477fc680d139c57cd38cc
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openal-soft/openal-soft_1.18.2-2.debian.tar.xz' openal-soft_1.18.2-2.debian.tar.xz 12568 SHA256:c000c6a95f16e7307748c40c2c34cdf8484887a56d8bafd8071b716976799059
```

### `dpkg` source package: `openexr=2.2.0-11.1ubuntu1.3`

Binary Packages:

- `libopenexr22:amd64=2.2.0-11.1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libopenexr22/copyright`)

- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.2.0-11.1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-11.1ubuntu1.3.dsc' openexr_2.2.0-11.1ubuntu1.3.dsc 2403 SHA512:425d006d15458deddb507e1b167d81effa77c0973696e81de65d480e53cc8a64df8943df132a3162b76ab54655d51855fe695258879640662f7fdf44067c0489
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0.orig.tar.gz' openexr_2.2.0.orig.tar.gz 14489661 SHA512:017abbeeb6b814508180721bc8e8940094965c4c55b135a198c6bcb109a04bf7f72e4aee81ee72cb2185fe818a41d892b383e8d2d59f40c673198948cb79279a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-11.1ubuntu1.3.debian.tar.xz' openexr_2.2.0-11.1ubuntu1.3.debian.tar.xz 30448 SHA512:69e9a7773c24cab8f63191a3fc40d9eaecaae75cf52b30aff9349400601a60c3cc9700c0959c7a710b2c2085b32cd31eca001c73f1e0b181ba5276328a6e6f41
```

### `dpkg` source package: `openjdk-8=8u265-b01-0ubuntu2~18.04`

Binary Packages:

- `openjdk-8-jdk:amd64=8u265-b01-0ubuntu2~18.04`
- `openjdk-8-jdk-headless:amd64=8u265-b01-0ubuntu2~18.04`
- `openjdk-8-jre:amd64=8u265-b01-0ubuntu2~18.04`
- `openjdk-8-jre-headless:amd64=8u265-b01-0ubuntu2~18.04`

Licenses: (parsed from: `/usr/share/doc/openjdk-8-jdk/copyright`, `/usr/share/doc/openjdk-8-jdk-headless/copyright`, `/usr/share/doc/openjdk-8-jre/copyright`, `/usr/share/doc/openjdk-8-jre-headless/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2`
- `LGPL-2-1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openjdk-lts=11.0.8+10-0ubuntu1~18.04.1`

Binary Packages:

- `openjdk-11-jre:amd64=11.0.8+10-0ubuntu1~18.04.1`
- `openjdk-11-jre-headless:amd64=11.0.8+10-0ubuntu1~18.04.1`

Licenses: (parsed from: `/usr/share/doc/openjdk-11-jre/copyright`, `/usr/share/doc/openjdk-11-jre-headless/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2`
- `LGPL-2-1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openjpeg2=2.3.0-2build0.18.04.1`

Binary Packages:

- `libopenjp2-7:amd64=2.3.0-2build0.18.04.1`

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
$ apt-get source -qq --print-uris openjpeg2=2.3.0-2build0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openjpeg2/openjpeg2_2.3.0-2build0.18.04.1.dsc' openjpeg2_2.3.0-2build0.18.04.1.dsc 2788 SHA512:829c842d7bd33b7723ee34318e34850dd0baf25fe6434554dc256c6ac0c138245f39d3a5f48b10ea348ff117e9bd443ad2a29263872efa4b374ec7eb4dc85bd5
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openjpeg2/openjpeg2_2.3.0.orig.tar.gz' openjpeg2_2.3.0.orig.tar.gz 2074456 SHA512:be8095e592ce2104bf368396c84741102fe8d7c0c7b7083509f6cba0d6f2d0b2db6069cbb107bb02426ef364c214c5f26a21c326e375aa0d96b2096345ae5c4e
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openjpeg2/openjpeg2_2.3.0-2build0.18.04.1.debian.tar.xz' openjpeg2_2.3.0-2build0.18.04.1.debian.tar.xz 21152 SHA512:a0c896c10c9677a6fac5ea845db877a3d9bdc163800e80a9ed5331babe1188cd4e9b1d86a270ea288081fb48ac85edffba4324cf42c12b31a08c67a0f08bfd14
```

### `dpkg` source package: `openldap=2.4.45+dfsg-1ubuntu1.6`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.45+dfsg-1ubuntu1.6`
- `libldap-common=2.4.45+dfsg-1ubuntu1.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openssl=1.1.1-1ubuntu2.1~18.04.6`

Binary Packages:

- `libssl1.1:amd64=1.1.1-1ubuntu2.1~18.04.6`
- `openssl=1.1.1-1ubuntu2.1~18.04.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1-1ubuntu2.1~18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.dsc' openssl_1.1.1-1ubuntu2.1~18.04.6.dsc 2754 SHA512:c16af42e0bb9530125f52ec1af1cef1743de3bfa1e82c51bddf43780b0f6298ddd60fbb260d713df56fc97f46614b922bb04a45f7ed94fadca1f00bff6d55cae
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz' openssl_1.1.1.orig.tar.gz 8337920 SHA512:c0284a4fe84bdf765ca5bc5148da4441ffc36392cfecaf9d372af00cf93b6de5681cab1248b6f8246474532155dc205da5ad49549ad7c61c07c917145e7c9c71
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz.asc' openssl_1.1.1.orig.tar.gz.asc 488 SHA512:cc69ad07a2edc17b579018bac4683f7d48deb8cde4a0f53eb777d2546eec9be6d13a610299705f3b87a7e4e8492432260cd7efc89d124c7fe1def309bbee461f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz' openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz 104692 SHA512:c1945f1641cc7edc9fbf6d9a2384d2fd05442f7d1460a3d7085f90b760ff4d5578d4bd33c662effcd1b92459fee6472415672350005a784fc9eaa19b96cd2fd1
```

### `dpkg` source package: `opus=1.1.2-1ubuntu1`

Binary Packages:

- `libopus0:amd64=1.1.2-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris opus=1.1.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/opus/opus_1.1.2-1ubuntu1.dsc' opus_1.1.2-1ubuntu1.dsc 1983 SHA256:8f8ccf72939b5c7923df4a189ca1d7a0dcf0cd5151e70b5623029c095c54849e
'http://archive.ubuntu.com/ubuntu/pool/main/o/opus/opus_1.1.2.orig.tar.gz' opus_1.1.2.orig.tar.gz 1012168 SHA256:7aaa84f06ec89cbf19d08c1dd1ceac965a11b28b3ff504cc52893f9be78eb5d1
'http://archive.ubuntu.com/ubuntu/pool/main/o/opus/opus_1.1.2-1ubuntu1.debian.tar.xz' opus_1.1.2-1ubuntu1.debian.tar.xz 5920 SHA256:d31fc55216fbda1a05ea6d59f43b71988a5b748c3d292f0297dc97e5585c9535
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
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14-1ubuntu0.1.dsc' pango1.0_1.40.14-1ubuntu0.1.dsc 3358 SHA512:03cd5f36dbbd14f63dd36c0fa633ee62d883897e553195c953b67986ede019bdb3a291b7d8d1e69768a83ff89acc3bb9a4a05b00a248b8a13355513811f554ac
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14.orig.tar.xz' pango1.0_1.40.14.orig.tar.xz 858388 SHA512:35ba7bc8be3992f206ccc2cc5aca0b94e2a3832f887fc9c45b0e29fddcb9051ce05a74377de0ca4ff95a87983b15688fa5d379d592faf87aa8eaca25ac18b7ea
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14-1ubuntu0.1.debian.tar.xz' pango1.0_1.40.14-1ubuntu0.1.debian.tar.xz 28460 SHA512:9de609d588388be9436c3cb0cd1913a7b8eda0a5b8e7e1effd6beb4002cf7a60236cd8a52410d1c09501beddbb2d89473da3f7f56d6b2b47886c18f0561b94d4
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

### `dpkg` source package: `pcsc-lite=1.8.23-1`

Binary Packages:

- `libpcsclite1:amd64=1.8.23-1`

Licenses: (parsed from: `/usr/share/doc/libpcsclite1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris pcsc-lite=1.8.23-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcsc-lite/pcsc-lite_1.8.23-1.dsc' pcsc-lite_1.8.23-1.dsc 2220 SHA256:9dd5d036154746e0b00141d716a8ca0b0e98334bbd1fa7704ead168778833936
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcsc-lite/pcsc-lite_1.8.23.orig.tar.bz2' pcsc-lite_1.8.23.orig.tar.bz2 749922 SHA256:5a27262586eff39cfd5c19aadc8891dd71c0818d3d629539bd631b958be689c9
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcsc-lite/pcsc-lite_1.8.23-1.debian.tar.xz' pcsc-lite_1.8.23-1.debian.tar.xz 29904 SHA256:983c9b69b2e2c0f3da6952627270247e24d86c4fec9965aa802ee901e75a403d
```

### `dpkg` source package: `perl-openssl-defaults=3build1`

Binary Packages:

- `perl-openssl-defaults:amd64=3build1`

Licenses: (parsed from: `/usr/share/doc/perl-openssl-defaults/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris perl-openssl-defaults=3build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl-openssl-defaults/perl-openssl-defaults_3build1.dsc' perl-openssl-defaults_3build1.dsc 1486 SHA256:bcbe2940127dfd7fe140ae51965699bc9b1d561f556a12f65670944ee72ba991
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl-openssl-defaults/perl-openssl-defaults_3build1.tar.xz' perl-openssl-defaults_3build1.tar.xz 4364 SHA256:0e72508143f4f42418a757711798d8eb548401c0ef5cb6a65889fbf9d0c98e6c
```

### `dpkg` source package: `perl=5.26.1-6ubuntu0.3`

Binary Packages:

- `libperl5.26:amd64=5.26.1-6ubuntu0.3`
- `perl=5.26.1-6ubuntu0.3`
- `perl-base=5.26.1-6ubuntu0.3`
- `perl-modules-5.26=5.26.1-6ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/libperl5.26/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.26/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `poppler-data=0.4.8-2`

Binary Packages:

- `poppler-data=0.4.8-2`

Licenses: (parsed from: `/usr/share/doc/poppler-data/copyright`)

- `AGPL-3+`
- `BSD-3-cluase`
- `GPL-2`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris poppler-data=0.4.8-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.8-2.dsc' poppler-data_0.4.8-2.dsc 2340 SHA256:3b0804f140be1e25907cd6e2d5acae61c01e0c4d81e40223a513e7a02304b18c
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.8.orig-ai0.tar.gz' poppler-data_0.4.8.orig-ai0.tar.gz 3515 SHA256:755a3a7cec6019b7cb6a7ac89828820e90d5105e66ebc2a7aacecacfb3ed4f1d
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.8.orig-from-ghostscript.tar.xz' poppler-data_0.4.8.orig-from-ghostscript.tar.xz 2320 SHA256:5070e1f3645080c809d80c42ee2e736648fe37bc2a68c3f54d1f9fce01086215
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.8.orig.tar.gz' poppler-data_0.4.8.orig.tar.gz 4209901 SHA256:1096a18161f263cccdc6d8a2eb5548c41ff8fcf9a3609243f1b6296abdf72872
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.8-2.debian.tar.xz' poppler-data_0.4.8-2.debian.tar.xz 19524 SHA256:471ce26ff9082a1562a360b3ba636ce7d0f19b9fb1b353a3d46c9a4f34d6f8ea
```

### `dpkg` source package: `poppler=0.62.0-2ubuntu2.10`

Binary Packages:

- `libpoppler73:amd64=0.62.0-2ubuntu2.10`

Licenses: (parsed from: `/usr/share/doc/libpoppler73/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris poppler=0.62.0-2ubuntu2.10
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler/poppler_0.62.0-2ubuntu2.10.dsc' poppler_0.62.0-2ubuntu2.10.dsc 3358 SHA512:fe82977903e0b3dd5ef0dd027cde0b8762c2b9b5acf4abf1469668d8a28e7e1b196ae688593180ad975c92b91ea95879d9c175af6632436743429e80d4ca431e
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler/poppler_0.62.0.orig.tar.xz' poppler_0.62.0.orig.tar.xz 1423372 SHA512:91f7eae7b05965ae97a34e658bed2a676be8a6e4d34f82148ece6eb58932632dcf9a34d50c66412f93f560ce575abf5c608ed6b1e5184604b96024801886c706
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler/poppler_0.62.0-2ubuntu2.10.debian.tar.xz' poppler_0.62.0-2ubuntu2.10.debian.tar.xz 43808 SHA512:a9e9613f5275ffdcf401e623a867bf3b1f311c60a17018c1fa98f341bca9decb5efaf21d3b31f77068d67e5a5a9b2b1c77849a1cd84a8cb1cdb6586c9e5c052c
```

### `dpkg` source package: `postgresql-10=10.12-0ubuntu0.18.04.1`

Binary Packages:

- `libpq5:amd64=10.12-0ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libpq5/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.dsc' procps_3.3.12-3ubuntu1.2.dsc 1920 SHA512:0ba0450d7411075000e5be9f64c92c73cf9f029fac707a13ad9bba692042a70c6f5535b31793eaca31670be61408e3a49cd861a0078859c57798a991e713459b
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12.orig.tar.xz' procps_3.3.12.orig.tar.xz 840540 SHA512:cb26a6b8419cc41134ccd072e1b38919ffd7126a99055a64726dc1d55149a2278fbf84528a71388196351e5bc72e81b18ce2a4f576a111d3741971327b30e6f8
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.debian.tar.xz' procps_3.3.12-3ubuntu1.2.debian.tar.xz 37736 SHA512:36ef9f540a72538f4a6fb02bfb53bf0b4689077c733b7dc4e301f968e2698667e6ad997f30a0ad21d189a8ee4bef7de2710441a8cc9f1ecb3aff6f67f182d49e
```

### `dpkg` source package: `publicsuffix=20180223.1310-1`

Binary Packages:

- `publicsuffix=20180223.1310-1`

Licenses: (parsed from: `/usr/share/doc/publicsuffix/copyright`)

- `CC0`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris publicsuffix=20180223.1310-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/publicsuffix/publicsuffix_20180223.1310-1.dsc' publicsuffix_20180223.1310-1.dsc 1343 SHA256:9977613565fee592bc705cdd44e9778e5058bcb2decddc42c6142696a29b69c9
'http://archive.ubuntu.com/ubuntu/pool/main/p/publicsuffix/publicsuffix_20180223.1310.orig.tar.gz' publicsuffix_20180223.1310.orig.tar.gz 83988 SHA256:70204865c9b59993c57bfba823ebd9d8f83db01fe914654d415ffc29ecb5667e
'http://archive.ubuntu.com/ubuntu/pool/main/p/publicsuffix/publicsuffix_20180223.1310-1.debian.tar.xz' publicsuffix_20180223.1310-1.debian.tar.xz 15436 SHA256:05182da7fd7cb1f2aa9397e0230a43798dfdb082a69ba203e712080efe1fd2bd
```

### `dpkg` source package: `pulseaudio=1:11.1-1ubuntu7.10`

Binary Packages:

- `libpulse0:amd64=1:11.1-1ubuntu7.10`

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
$ apt-get source -qq --print-uris pulseaudio=1:11.1-1ubuntu7.10
'http://archive.ubuntu.com/ubuntu/pool/main/p/pulseaudio/pulseaudio_11.1-1ubuntu7.10.dsc' pulseaudio_11.1-1ubuntu7.10.dsc 3227 SHA512:d30bf6b0ad8ea6cfc78a390f7cd2774252cdf418ee19399ce445fdb16273c9895fee3f4f9a772691c5d5732141654f8ada9546809bc122feb64da151033fac2d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pulseaudio/pulseaudio_11.1.orig.tar.xz' pulseaudio_11.1.orig.tar.xz 1648924 SHA512:8863d8d7aede0d9a4d158e84e7bece91747c335f9ac98c7b21fafe76b762f8817e1125307aa46e561e540d2c40525e91f51a55ec34ac55d58fd5980199856a7a
'http://archive.ubuntu.com/ubuntu/pool/main/p/pulseaudio/pulseaudio_11.1-1ubuntu7.10.debian.tar.xz' pulseaudio_11.1-1ubuntu7.10.debian.tar.xz 114456 SHA512:d66ecf85d8e1a0aa04e325ff4a29875a141d426abcf63b9afe440adc28e48afa8b29f9f34aa1018ee699a1b6cacb8e55bc3cca0ae69bf6e44f17db06b72d340d
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
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.dsc' python3-defaults_3.6.7-1~18.04.dsc 2896 SHA512:1f6f6bdbc030b0c9bf24a97b2c48052c8a52810e22e021b00719fce7eea8d454c9cc756e3d73ee79be06655b9a35fe8279bf71833a4aa6c605859856e4a31151
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.tar.gz' python3-defaults_3.6.7-1~18.04.tar.gz 137600 SHA512:7020c60ba146deafaf1937883bea03c39efb1068968025756b32e7c7f069c06bfdfb3e1b91dcaa5a1e1c4c01e0177ea91beb4f5fa71f5e60334866ef5b28a2ef
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `rubberband=1.8.1-7ubuntu2`

Binary Packages:

- `librubberband2:amd64=1.8.1-7ubuntu2`

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
$ apt-get source -qq --print-uris rubberband=1.8.1-7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/r/rubberband/rubberband_1.8.1-7ubuntu2.dsc' rubberband_1.8.1-7ubuntu2.dsc 2442 SHA256:43182648c1613281de9c2e64fab0da7bf1c7664169138a1184a1ef89cd2d3c69
'http://archive.ubuntu.com/ubuntu/pool/universe/r/rubberband/rubberband_1.8.1.orig.tar.bz2' rubberband_1.8.1.orig.tar.bz2 177501 SHA256:ff0c63b0b5ce41f937a8a3bc560f27918c5fe0b90c6bc1cb70829b86ada82b75
'http://archive.ubuntu.com/ubuntu/pool/universe/r/rubberband/rubberband_1.8.1-7ubuntu2.debian.tar.xz' rubberband_1.8.1-7ubuntu2.debian.tar.xz 9424 SHA256:2e1af1831dc0223fc5df26d131e633fc5f9ccbb68c705cfa95823db9584df15f
```

### `dpkg` source package: `scowl=2017.08.24-1`

Binary Packages:

- `hunspell-en-us=1:2017.08.24`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris scowl=2017.08.24-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/scowl/scowl_2017.08.24-1.dsc' scowl_2017.08.24-1.dsc 2935 SHA256:4ee4e72580fa948a91b9eecd6969fc8c3b7abcd5a93142cde4a78a5b0b13f2c8
'http://archive.ubuntu.com/ubuntu/pool/main/s/scowl/scowl_2017.08.24.orig.tar.gz' scowl_2017.08.24.orig.tar.gz 2543767 SHA256:ba84da9f5af06dbfded82236372545c06fd8162c3d48d11410bdfcf27ef3b0cd
'http://archive.ubuntu.com/ubuntu/pool/main/s/scowl/scowl_2017.08.24-1.debian.tar.xz' scowl_2017.08.24-1.debian.tar.xz 15976 SHA256:ca4f77b3335db43f214b2e09797553b1b631ee6586a73d259aad45933578f0e8
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

### `dpkg` source package: `servlet-api=4.0.1-2~18.04`

Binary Packages:

- `libservlet-api-java=4.0.1-2~18.04`
- `libservlet3.1-java=1:4.0.1-2~18.04`

Licenses: (parsed from: `/usr/share/doc/libservlet-api-java/copyright`, `/usr/share/doc/libservlet3.1-java/copyright`)

- `Apache-2.0`
- `CDDL-1.1`
- `GPL-2`
- `GPL-2 with Classpath exception`

Source:

```console
$ apt-get source -qq --print-uris servlet-api=4.0.1-2~18.04
'http://archive.ubuntu.com/ubuntu/pool/universe/s/servlet-api/servlet-api_4.0.1-2~18.04.dsc' servlet-api_4.0.1-2~18.04.dsc 2282 SHA512:31dce402fec1007c8db028fd803ee3d65ae139be5508d74db244e2dd5a408a72124777cb2de36f8d4cfc1a392ab1bbba9ebe877eef26e5db0a8210aa24e0cbe4
'http://archive.ubuntu.com/ubuntu/pool/universe/s/servlet-api/servlet-api_4.0.1.orig.tar.xz' servlet-api_4.0.1.orig.tar.xz 94792 SHA512:0696ef8ab2e78918c9d855cc59b12de4e12bd42a7f0295ba1603d8b7d4eb62bd409d6207e419b2af0be27e508f83947ccada99901000a7b1966eb4c7bf8095e8
'http://archive.ubuntu.com/ubuntu/pool/universe/s/servlet-api/servlet-api_4.0.1-2~18.04.debian.tar.xz' servlet-api_4.0.1-2~18.04.debian.tar.xz 10948 SHA512:681479152e1cb0dfc7acda7827e3ea4ed13c91a5238c66a1dd3dd89d0152631d3489fa80c46fc5acada7905867c4972177126cef7a5285c649c3eade60f8e132
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
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.dsc' shadow_4.5-1ubuntu2.dsc 2426 SHA512:69714d4cd1903f091bc2c4759d98ce588cc90e9f2ab49226b46872eb2b2cf4f996f30b8da146a2950e164d24fa265f90e689043152d79d1bc255add5f90d54a3
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA512:4278544efdd6d800a3c46cfcb144f209ace14ebe017ba1c0d05425fac7868062a73afa8522036a2bc0a16f6f1e7c16373a204463221012367ce0e8e9ef4c4a4d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.debian.tar.xz' shadow_4.5-1ubuntu2.debian.tar.xz 471472 SHA512:d4017784bfc5118b86533da52909459adf4e79ffa049d8029437860bfaeac91eabd40e6510f67bba6f8b2d74fde62c24eb8e37a7b4637d14eeb63aecaf2294cc
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

### `dpkg` source package: `shine=3.1.1-1`

Binary Packages:

- `libshine3:amd64=3.1.1-1`

Licenses: (parsed from: `/usr/share/doc/libshine3/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris shine=3.1.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/shine/shine_3.1.1-1.dsc' shine_3.1.1-1.dsc 2030 SHA256:66a5f46a7a0f5e7fe8264f35740009bd2c774d020f85261339a830403ecfc422
'http://archive.ubuntu.com/ubuntu/pool/universe/s/shine/shine_3.1.1.orig.tar.gz' shine_3.1.1.orig.tar.gz 940443 SHA256:565b87867d6f8e6616a236445d194e36f4daa9b4e7af823fcf5010af7610c49e
'http://archive.ubuntu.com/ubuntu/pool/universe/s/shine/shine_3.1.1-1.debian.tar.xz' shine_3.1.1-1.debian.tar.xz 3488 SHA256:0752ce4cb26066d5f0fd42f4a164340c91e061bb603848e870d29e4c345e9ce9
```

### `dpkg` source package: `slang2=2.3.1a-3ubuntu1`

Binary Packages:

- `libslang2:amd64=2.3.1a-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libslang2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris slang2=2.3.1a-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/slang2/slang2_2.3.1a-3ubuntu1.dsc' slang2_2.3.1a-3ubuntu1.dsc 2401 SHA256:68966016c0ddc7de6c3d61727e10c1bc35e6f82885b0fac76bfc57e11ad7717e
'http://archive.ubuntu.com/ubuntu/pool/main/s/slang2/slang2_2.3.1a.orig.tar.xz' slang2_2.3.1a.orig.tar.xz 1292048 SHA256:c37fb0dc27922b182d240e36ae781a839410738af740928288670b2851d987da
'http://archive.ubuntu.com/ubuntu/pool/main/s/slang2/slang2_2.3.1a-3ubuntu1.debian.tar.xz' slang2_2.3.1a-3ubuntu1.debian.tar.xz 24152 SHA256:011bc33f0abf437d7338ddd25e07c078da1c3c8204e4eac2aa539c99ea742c6b
```

### `dpkg` source package: `snappy=1.1.7-1`

Binary Packages:

- `libsnappy1v5:amd64=1.1.7-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris snappy=1.1.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/snappy/snappy_1.1.7-1.dsc' snappy_1.1.7-1.dsc 1785 SHA256:a2b45cc0ddc41baae02f0dd51448afef2d9a2f771253b472f0141aff6b5c640c
'http://archive.ubuntu.com/ubuntu/pool/main/s/snappy/snappy_1.1.7.orig.tar.gz' snappy_1.1.7.orig.tar.gz 1090550 SHA256:3dfa02e873ff51a11ee02b9ca391807f0c8ea0529a4924afa645fbf97163f9d4
'http://archive.ubuntu.com/ubuntu/pool/main/s/snappy/snappy_1.1.7-1.debian.tar.xz' snappy_1.1.7-1.debian.tar.xz 5028 SHA256:b6041cea215dbc3a48c8230be97445fe0ec342bad9eb4f6ddc26ac6cb3fc4e12
```

### `dpkg` source package: `sndio=1.1.0-3`

Binary Packages:

- `libsndio6.1:amd64=1.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libsndio6.1/copyright`)

- `ISC`
- `ISC-packaging`

Source:

```console
$ apt-get source -qq --print-uris sndio=1.1.0-3
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sndio/sndio_1.1.0-3.dsc' sndio_1.1.0-3.dsc 1861 SHA256:31f5b892d023550d3b4657ee74982a6053102db4869c8c8c23d3c7a8aaf2752b
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sndio/sndio_1.1.0.orig.tar.gz' sndio_1.1.0.orig.tar.gz 121018 SHA256:fcd7f845ff70f38c2898d737450b8aa3e1bb0afb9d147e8429ef22c0b2c2db57
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sndio/sndio_1.1.0-3.debian.tar.xz' sndio_1.1.0-3.debian.tar.xz 5196 SHA256:c0e5e04946b01d04f131223a9c9ee6e204ee325b50419e2160eed19a4d49d8aa
```

### `dpkg` source package: `speex=1.2~rc1.2-1ubuntu2`

Binary Packages:

- `libspeex1:amd64=1.2~rc1.2-1ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris speex=1.2~rc1.2-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/speex/speex_1.2~rc1.2-1ubuntu2.dsc' speex_1.2~rc1.2-1ubuntu2.dsc 2360 SHA256:cfd4ef68c8ae7de261b0540b0749109c0831adee854b9262082c5f2e36cea046
'http://archive.ubuntu.com/ubuntu/pool/main/s/speex/speex_1.2~rc1.2.orig.tar.gz' speex_1.2~rc1.2.orig.tar.gz 1069339 SHA256:8320fb86a024dfe1b6a78a7d57bc2388e5f8cb7f2fa10c946db2704e1e5d2805
'http://archive.ubuntu.com/ubuntu/pool/main/s/speex/speex_1.2~rc1.2-1ubuntu2.diff.gz' speex_1.2~rc1.2-1ubuntu2.diff.gz 10372 SHA256:1f8602e771c179ce81444f2b82414683ee69715837e47b9755b114bbdfb64d17
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
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.dsc' sqlite3_3.22.0-1ubuntu0.4.dsc 2512 SHA512:5b0de02a1ee10ef1d38bbd66e5148f044574aba7211cbe003855b8141062955913514501adac6208297f435c02160a39e14dbad934907afd49a506a34ae4ea9a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig-www.tar.xz' sqlite3_3.22.0.orig-www.tar.xz 3564688 SHA512:e469878137ec3d06886fe096c4325451e8c9b73f6841d28fac9bed45e698bdc1222739570abf2ce456e0853b0c6876b1c79ca0896826295f64d27b276541c1f8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig.tar.xz' sqlite3_3.22.0.orig.tar.xz 6019648 SHA512:ce3b05cb9f75a5c7a5e8562b70e72e23c043222fd61995f795cbcc40f3f8efcac2660e57b588a15bfdce28c8eb644745bb73af35f5b98ba956dd77457d661dfa
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz' sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz 47632 SHA512:1b280b6c301b2f3c15ebdfe6085584cef34257edae14c94d7d6e8d06a7b884a96029d354cb3f09df6b6427f671a24cc25ee1ebc178c7168cd0a52bce8c8b5cf0
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
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.42.dsc' systemd_237-3ubuntu10.42.dsc 5182 SHA512:cd9cea067ac21e9d627c3f28acd6f10e5511a9591d5283e9aab4ae01dc4178e332ccf074bc5dfbc0a7adc7a1ca2687d85d769123af34c59ea9b957ccf2dc54c3
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237.orig.tar.gz' systemd_237.orig.tar.gz 6871350 SHA512:15ef4b92815a6dd9a6c51672dbc00fd7cd0f08068ef0cbeaca574f68d330b28bc67ba1946f24f75ef3d9e7b63843a73eea700db54688061dbf5c9f8470394c3b
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.42.debian.tar.xz' systemd_237-3ubuntu10.42.debian.tar.xz 275288 SHA512:d68b1dcd71ab49bd5b672a456923b50203b866dfd9ac79aa7aefe37e8799d2b37245dc850089e2d700ba129e7ca4f791a164321c46c08f97866c3b67d0345df7
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
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.dsc' tar_1.29b-2ubuntu0.1.dsc 1426 SHA512:07cd0e105d5620c2f9b77c1a8b6f1016f2c83a022a38d0fa9e94bc07ffe3f716df609b8c92808e5e3e80db8eaece3b076643debd54c653eda76eb1973a56e9ab
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b.orig.tar.xz' tar_1.29b.orig.tar.xz 1822008 SHA512:6814c906f3bf3d1421d46e63aff7921acffbd2b2a0a7e5c20b472a821eab839d6eab93653d964ae16376b65da223c57a92455f44793522c84c8b1343af20b106
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.debian.tar.xz' tar_1.29b-2ubuntu0.1.debian.tar.xz 31672 SHA512:e4756dd0ad0d765af0c6639695b17cc86f80033a45705cdcb845639bab7d3aed0fac8d86ac28a0aa2e024bdb4dad43376f4a02c915a0921609deeeed74637bd7
```

### `dpkg` source package: `tcp-wrappers=7.6.q-27`

Binary Packages:

- `libwrap0:amd64=7.6.q-27`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcp-wrappers=7.6.q-27
'http://archive.ubuntu.com/ubuntu/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-27.dsc' tcp-wrappers_7.6.q-27.dsc 1748 SHA256:5313bbce685bf4d4bfc1311ecdbf2a42a3acbc1d5d9fbb5c1b2e27e17d89fa9b
'http://archive.ubuntu.com/ubuntu/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q.orig.tar.gz' tcp-wrappers_7.6.q.orig.tar.gz 99438 SHA256:9543d7adedf78a6de0b221ccbbd1952e08b5138717f4ade814039bb489a4315d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-27.debian.tar.xz' tcp-wrappers_7.6.q-27.debian.tar.xz 36060 SHA256:b73487b0faf59dfcc1074b9f11a91556713d9ae210033536f20cfd3c8bc73b36
```

### `dpkg` source package: `tiff=4.0.9-5ubuntu0.3`

Binary Packages:

- `libtiff5:amd64=4.0.9-5ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.9-5ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9-5ubuntu0.3.dsc' tiff_4.0.9-5ubuntu0.3.dsc 2299 SHA512:1577627fb228fbb25ba7e405c4931bc642f0c2f8d4a061bee16fdf572a23d637bf1974911e18cb17461b8fa533fbcc1924d8b099c96116385e2306f853cb2e1a
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9.orig.tar.gz' tiff_4.0.9.orig.tar.gz 2305681 SHA512:04f3d5eefccf9c1a0393659fe27f3dddd31108c401ba0dc587bca152a1c1f6bc844ba41622ff5572da8cc278593eff8c402b44e7af0a0090e91d326c2d79f6cd
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9-5ubuntu0.3.debian.tar.xz' tiff_4.0.9-5ubuntu0.3.debian.tar.xz 32200 SHA512:f4c77de2474074c942891927b360eedbdf1217c2fa2083338e9d24956a6d6a418e9b4935df3288e652170186d67bbcb865f38a3f5f4c7eea65405a6a6cbf3c0c
```

### `dpkg` source package: `twolame=0.3.13-3`

Binary Packages:

- `libtwolame0:amd64=0.3.13-3`

Licenses: (parsed from: `/usr/share/doc/libtwolame0/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris twolame=0.3.13-3
'http://archive.ubuntu.com/ubuntu/pool/main/t/twolame/twolame_0.3.13-3.dsc' twolame_0.3.13-3.dsc 2079 SHA256:f3e7b075f6b7e15f3e9d72ddd4486aeb427974a75f03fd69ec7bc64f0e38999f
'http://archive.ubuntu.com/ubuntu/pool/main/t/twolame/twolame_0.3.13.orig.tar.gz' twolame_0.3.13.orig.tar.gz 660415 SHA256:98f332f48951f47f23f70fd0379463aff7d7fb26f07e1e24e42ddef22cc6112a
'http://archive.ubuntu.com/ubuntu/pool/main/t/twolame/twolame_0.3.13-3.debian.tar.xz' twolame_0.3.13-3.debian.tar.xz 4352 SHA256:5d1806d16825de652a1c956afbd77739a7d7f1494cf8b238f2f85ed4c94d173f
```

### `dpkg` source package: `ubuntu-keyring=2018.09.18.1~18.04.0`

Binary Packages:

- `ubuntu-keyring=2018.09.18.1~18.04.0`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2018.09.18.1~18.04.0
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.dsc' ubuntu-keyring_2018.09.18.1~18.04.0.dsc 1503 SHA512:1aa2656d79d925d42857de9eb79fac8433fc5ec0cc1daaa55af31f1eb4f482646f48e0e37d8d794ffafccbae34698503aa183b27666b18fc00c38e1b41c92f06
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz' ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz 34238 SHA512:7e0b6b9b4f900139c6743037b18591abba0183db94bf6d988b65c2eafe7bd53900f52af0cea14e1a80f4fd54eef39ef7b5dbf66802b53c022e40802a287912b1
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
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-themes/ubuntu-themes_16.10+18.04.20181005-0ubuntu1.dsc' ubuntu-themes_16.10+18.04.20181005-0ubuntu1.dsc 2345 SHA512:5ef48ee86e3b0ba33c1acd58d9965823caeb4e5b363d18ebd16489e0e7b1101f13c26cdf35e9117c4f8a394bf6289819b1a8d5724572446a35bbb486332f6723
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-themes/ubuntu-themes_16.10+18.04.20181005.orig.tar.gz' ubuntu-themes_16.10+18.04.20181005.orig.tar.gz 16239257 SHA512:53e12897ca236e5a085445b05f48f21639b8acc56d5524022a3379619dbf43d19d71e50f73c6025bdec3f009a23f2d2f83921e13eea9c628fcf7ae27d7372146
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-themes/ubuntu-themes_16.10+18.04.20181005-0ubuntu1.diff.gz' ubuntu-themes_16.10+18.04.20181005-0ubuntu1.diff.gz 28561 SHA512:96f4376ceff9785923b8cb074893cbd6662da5478a173fd97c56c3f2dd40d8d31c73a46d2eb7722ef2429206d9f3eed12ec0afbeaefce3b4cfd113a83729ec68
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `vim=2:8.0.1453-1ubuntu1.3`

Binary Packages:

- `vim=2:8.0.1453-1ubuntu1.3`
- `vim-common=2:8.0.1453-1ubuntu1.3`
- `vim-runtime=2:8.0.1453-1ubuntu1.3`
- `xxd=2:8.0.1453-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/vim/copyright`, `/usr/share/doc/vim-common/copyright`, `/usr/share/doc/vim-runtime/copyright`, `/usr/share/doc/xxd/copyright`)

- `Apache`
- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-2-clause`
- `BSD-3-clause`
- `Compaq`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `OPL-1+`
- `SRA`
- `UC`
- `Vim`
- `Vim-Regexp`
- `X11`
- `XPM`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `wavpack=5.1.0-2ubuntu1.4`

Binary Packages:

- `libwavpack1:amd64=5.1.0-2ubuntu1.4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris wavpack=5.1.0-2ubuntu1.4
'http://archive.ubuntu.com/ubuntu/pool/main/w/wavpack/wavpack_5.1.0-2ubuntu1.4.dsc' wavpack_5.1.0-2ubuntu1.4.dsc 2199 SHA512:e26ebe715cabb16da222cac11469e7242b5d14a2e764919e2d25c5ca605dd90a3910ba9079588a20cb7b4a0478aa2f92c0c67e5b18723b15e52c7648cc9de4be
'http://archive.ubuntu.com/ubuntu/pool/main/w/wavpack/wavpack_5.1.0.orig.tar.bz2' wavpack_5.1.0.orig.tar.bz2 824331 SHA512:4c31616ae63c3a875afa20f26ce935f7a8f9921e2892b4b8388eca3ccd83b2d686f43eed8b9ec1dead934a1148401b9dced3b05f509b7942c48d7af31cf80a54
'http://archive.ubuntu.com/ubuntu/pool/main/w/wavpack/wavpack_5.1.0-2ubuntu1.4.debian.tar.xz' wavpack_5.1.0-2ubuntu1.4.debian.tar.xz 11632 SHA512:8f91fbc0fa443143c936707cd53659506131df47cabe4faac1d2f031526ed960d008851fddb90502d77959f32372fdbf0b495f51515e73c8933ceb352cd07ce0
```

### `dpkg` source package: `wayland=1.16.0-1ubuntu1.1~18.04.3`

Binary Packages:

- `libwayland-client0:amd64=1.16.0-1ubuntu1.1~18.04.3`
- `libwayland-cursor0:amd64=1.16.0-1ubuntu1.1~18.04.3`
- `libwayland-egl1:amd64=1.16.0-1ubuntu1.1~18.04.3`
- `libwayland-server0:amd64=1.16.0-1ubuntu1.1~18.04.3`

Licenses: (parsed from: `/usr/share/doc/libwayland-client0/copyright`, `/usr/share/doc/libwayland-cursor0/copyright`, `/usr/share/doc/libwayland-egl1/copyright`, `/usr/share/doc/libwayland-server0/copyright`)

- `X11`

Source:

```console
$ apt-get source -qq --print-uris wayland=1.16.0-1ubuntu1.1~18.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/w/wayland/wayland_1.16.0-1ubuntu1.1~18.04.3.dsc' wayland_1.16.0-1ubuntu1.1~18.04.3.dsc 2468 SHA512:4fde23eeb1fe6967d70994ff9937a86e0b5918144eef3bad448273266d2e95a077208f1a84288148659087ded4841675f71c52a8312fed4bfa8610ac648f0afd
'http://archive.ubuntu.com/ubuntu/pool/main/w/wayland/wayland_1.16.0-1ubuntu1.1~18.04.3.tar.gz' wayland_1.16.0-1ubuntu1.1~18.04.3.tar.gz 325074 SHA512:1e17d84369d58dac99edfb79249639069b69d63cb4716926963f2d637ec3199eed67ee283a84b32a1d2687c7286d0041752e5c6e54a7b9425cecd3253502a99b
```

### `dpkg` source package: `websocket-api=1.1-1~18.04`

Binary Packages:

- `libwebsocket-api-java=1.1-1~18.04`

Licenses: (parsed from: `/usr/share/doc/libwebsocket-api-java/copyright`)

- `Apache-2.0`
- `CDDL-1.1`
- `GPL-2`
- `GPL-2 with Classpath exception`

Source:

```console
$ apt-get source -qq --print-uris websocket-api=1.1-1~18.04
'http://archive.ubuntu.com/ubuntu/pool/universe/w/websocket-api/websocket-api_1.1-1~18.04.dsc' websocket-api_1.1-1~18.04.dsc 2075 SHA512:07577795e8d7763942f83aeaac598b6c410b7f04779d53f5adec64afb5589e4665ce1fbba79546d9ce0c743e2872680ce1224c5718cec0c948eb50558490919d
'http://archive.ubuntu.com/ubuntu/pool/universe/w/websocket-api/websocket-api_1.1.orig.tar.xz' websocket-api_1.1.orig.tar.xz 28884 SHA512:08dd3f4c17f8264296e6bf4ff8faf23e74b84b94d34b07493ce519300afc53678b0265c9eaae2d619a08e2e97befd7ce3b17ed0760c0d028606f60bcaa2e1037
'http://archive.ubuntu.com/ubuntu/pool/universe/w/websocket-api/websocket-api_1.1-1~18.04.debian.tar.xz' websocket-api_1.1-1~18.04.debian.tar.xz 8540 SHA512:a894a97e5b4384ed808ebf89e5d70f82eaa613496a83a03c76b693eae80e7aee140e71aaa11948484ce872b005b8cd06e5ef9da49d8aa33b80847f1760ab2a46
```

### `dpkg` source package: `wget=1.19.4-1ubuntu2.2`

Binary Packages:

- `wget=1.19.4-1ubuntu2.2`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.19.4-1ubuntu2.2
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4-1ubuntu2.2.dsc' wget_1.19.4-1ubuntu2.2.dsc 2226 SHA512:7fbc8eccfcb3e559f4f25c4159b06a9663f87c02ab63a9eebc63a812a6a0d72958329f4c8f60fd3dc0272bb586a13535389e0fe5d5a6a2b42f909f567976dd57
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4.orig.tar.gz' wget_1.19.4.orig.tar.gz 4310657 SHA512:e84b0c40235b160ade69e18f2f139c782eb2387edc97a847c11dbb906c0273daf6d0ef5afe20360ba965c7da8b5e109f5a45e39ea93d20ec945575203235943a
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4.orig.tar.gz.asc' wget_1.19.4.orig.tar.gz.asc 1241 SHA512:63ad8a3184a98dbda966a535964e37c84291a13fe15f7defb6fb3672f7148d66143498354e818eabc1e506ae9a16f7c9b8188fa22c2fed3a02aa9cb6d1de3a38
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4-1ubuntu2.2.debian.tar.xz' wget_1.19.4-1ubuntu2.2.debian.tar.xz 66156 SHA512:c458c630d82aaeffa0f4df6a543aa9b3a312d5b4aad4835d6da37736f165bb1151a9337ad65298c8b50c4a07de40d40303f0fc5953f2086a1909878f97c7b262
```

### `dpkg` source package: `x11-utils=7.7+3build1`

Binary Packages:

- `x11-utils=7.7+3build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11-utils=7.7+3build1
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11-utils/x11-utils_7.7+3build1.dsc' x11-utils_7.7+3build1.dsc 2178 SHA256:45ac9b2a730ad37d141438c5e479424d9246765ef26fddc57d01113c719d2548
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11-utils/x11-utils_7.7+3build1.tar.gz' x11-utils_7.7+3build1.tar.gz 2711232 SHA256:8761fd09a886d6910b68cbf854e1e1baa381286839f3dca9a28628bbe6e826d2
```

### `dpkg` source package: `x11-xserver-utils=7.7+7build1`

Binary Packages:

- `x11-xserver-utils=7.7+7build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11-xserver-utils=7.7+7build1
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11-xserver-utils/x11-xserver-utils_7.7+7build1.dsc' x11-xserver-utils_7.7+7build1.dsc 1956 SHA256:e3893b0248008eb6ffedb3447a1b0dd53e3e8071e7193ffaf54cbaca73ed507a
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11-xserver-utils/x11-xserver-utils_7.7+7build1.tar.gz' x11-xserver-utils_7.7+7build1.tar.gz 2605226 SHA256:d5ce07f9586db6e686c7ddf701de46de9d73d09a9cf44c5c406b543ef05cb8c1
```

### `dpkg` source package: `x264=2:0.152.2854+gite9a5903-2`

Binary Packages:

- `libx264-152:amd64=2:0.152.2854+gite9a5903-2`

Licenses: (parsed from: `/usr/share/doc/libx264-152/copyright`)

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
$ apt-get source -qq --print-uris x264=2:0.152.2854+gite9a5903-2
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x264/x264_0.152.2854+gite9a5903-2.dsc' x264_0.152.2854+gite9a5903-2.dsc 2469 SHA256:df456fc46c606550c87a8cd4fefee72cd6981acccda66c9ec363e7913fd225dd
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x264/x264_0.152.2854+gite9a5903.orig.tar.gz' x264_0.152.2854+gite9a5903.orig.tar.gz 912193 SHA256:8b623844222e23ae1f166a58575967d41e8a4478b43c4b2ff4b75dbcdd1f2d82
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x264/x264_0.152.2854+gite9a5903-2.debian.tar.xz' x264_0.152.2854+gite9a5903-2.debian.tar.xz 23472 SHA256:a26888df268e5222a137fd09cb871e446d1edd8ca4f57e76eef92f1338277a98
```

### `dpkg` source package: `x265=2.6-3`

Binary Packages:

- `libx265-146:amd64=2.6-3`

Licenses: (parsed from: `/usr/share/doc/libx265-146/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=2.6-3
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_2.6-3.dsc' x265_2.6-3.dsc 2253 SHA256:9d23c37afb383646216502fae2ff7e45396c759aea4f3e8b215e21ef14115801
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_2.6.orig.tar.gz' x265_2.6.orig.tar.gz 1271976 SHA256:1bf0036415996af841884802161065b9e6be74f5f6808ac04831363e2549cdbf
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_2.6-3.debian.tar.xz' x265_2.6-3.debian.tar.xz 12856 SHA256:4ac9f0b06d67a95773b150a378d1e126f1bd5d96be3cc452d6266686b7e8b893
```

### `dpkg` source package: `xdg-user-dirs=0.17-1ubuntu1`

Binary Packages:

- `xdg-user-dirs=0.17-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/xdg-user-dirs/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xdg-user-dirs=0.17-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.17-1ubuntu1.dsc' xdg-user-dirs_0.17-1ubuntu1.dsc 2319 SHA256:62400a07ff099ac286502629389843a22b9d71e30179f37b7c05a2bc5ae37d9b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.17.orig.tar.gz' xdg-user-dirs_0.17.orig.tar.gz 257291 SHA256:2a07052823788e8614925c5a19ef5b968d8db734fdee656699ea4f97d132418c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.17-1ubuntu1.debian.tar.xz' xdg-user-dirs_0.17-1ubuntu1.debian.tar.xz 28680 SHA256:1c18dd3208d58ec4be6cbf28c480ebc2f9c349463a2e7765d040172ba6a63c23
```

### `dpkg` source package: `xdg-utils=1.1.2-1ubuntu2.3`

Binary Packages:

- `xdg-utils=1.1.2-1ubuntu2.3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xdg-utils=1.1.2-1ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-utils/xdg-utils_1.1.2-1ubuntu2.3.dsc' xdg-utils_1.1.2-1ubuntu2.3.dsc 2185 SHA512:4c0a10c4bdfc8fdde074c7d7b78b862b06ed6b7b29f547e0d269b74a21fd4b1ecf4676eee0c454447a6a7fba76d6ec035c98f7cc0291be9d2cdfdce0597d1903
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-utils/xdg-utils_1.1.2.orig.tar.gz' xdg-utils_1.1.2.orig.tar.gz 296735 SHA512:1927506065788b5f8bba8b0617a8ee585265342fa40c4b73000d320acd5909036daef94d49495b00982dbb67b7706b2f1ed949cb4cc519dfa534be2c1c8f74db
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-utils/xdg-utils_1.1.2-1ubuntu2.3.debian.tar.xz' xdg-utils_1.1.2-1ubuntu2.3.debian.tar.xz 12276 SHA512:bd20598ed7584b1d1032950245d401cb9dc5e9584a67d77eb5d44099003ecd6138ca4a93c48ceb33b9bc04d8cdabcaae8ca7fb101182a620f0a16ac20b42c639
```

### `dpkg` source package: `xft=2.3.2-1`

Binary Packages:

- `libxft2:amd64=2.3.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xft=2.3.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xft/xft_2.3.2-1.dsc' xft_2.3.2-1.dsc 2115 SHA256:69698a22404fae66b26bcc3cfe959cf0b42a0704ffdb0eec27a109fa0ce99714
'http://archive.ubuntu.com/ubuntu/pool/main/x/xft/xft_2.3.2.orig.tar.gz' xft_2.3.2.orig.tar.gz 402454 SHA256:26cdddcc70b187833cbe9dc54df1864ba4c03a7175b2ca9276de9f05dce74507
'http://archive.ubuntu.com/ubuntu/pool/main/x/xft/xft_2.3.2-1.diff.gz' xft_2.3.2-1.diff.gz 11645 SHA256:e72df82575f6942a326c0bf414650b9be1fd6e8624e3746dc39286d5017b1333
```

### `dpkg` source package: `xkeyboard-config=2.23.1-1ubuntu1.18.04.1`

Binary Packages:

- `xkb-data=2.23.1-1ubuntu1.18.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xkeyboard-config=2.23.1-1ubuntu1.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xkeyboard-config/xkeyboard-config_2.23.1-1ubuntu1.18.04.1.dsc' xkeyboard-config_2.23.1-1ubuntu1.18.04.1.dsc 1645 SHA512:9abc336013fbb13322699f8ade9c0a1a97c5d19c83f2c34c3c497c716fd824a3355e9c8b8ba023557583ff5e75ea90819ad3594bdce1a71612e2af562c0e88b3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xkeyboard-config/xkeyboard-config_2.23.1.orig.tar.gz' xkeyboard-config_2.23.1.orig.tar.gz 1599103 SHA512:2f11039e48b1a0f45d5c3c5e1b7a3c915b1d6050972b11434ec13caafe3948c5bde6f4bba856c4e1fa7408ccd2680d39c5250ab267558b55f2b010528dc73016
'http://archive.ubuntu.com/ubuntu/pool/main/x/xkeyboard-config/xkeyboard-config_2.23.1-1ubuntu1.18.04.1.diff.gz' xkeyboard-config_2.23.1-1ubuntu1.18.04.1.diff.gz 52509 SHA512:639f52ff248d0feb17b02e71ff11d4ea7e9b23d88c9917d4e0441eb2352f70c60575e08f3d51f73bca8b3a2860ce97ccb2d1ee61bdbd8d4e519dfe2a1da92e7b
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

### `dpkg` source package: `xorg-sgml-doctools=1:1.11-1`

Binary Packages:

- `xorg-sgml-doctools=1:1.11-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xorg-sgml-doctools=1:1.11-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.dsc' xorg-sgml-doctools_1.11-1.dsc 1975 SHA256:1f4a12a38420b0ddab35553b9588fdf43ab39577958aed70fca435c9a747141a
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11.orig.tar.gz' xorg-sgml-doctools_1.11.orig.tar.gz 150367 SHA256:986326d7b4dd2ad298f61d8d41fe3929ac6191c6000d6d7e47a8ffc0c34e7426
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.diff.gz' xorg-sgml-doctools_1.11-1.diff.gz 3194 SHA256:18eeb355cb0efff9f47f8ed8e852eee322d9733a427419f4b39f43bc4df630c1
```

### `dpkg` source package: `xorg=1:7.7+19ubuntu7.1`

Binary Packages:

- `x11-common=1:7.7+19ubuntu7.1`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19ubuntu7.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu7.1.dsc' xorg_7.7+19ubuntu7.1.dsc 2103 SHA512:e6c459b18a96cbfda965f13852ff1c75b7e3240f61c4ea941996b99f74ffcf52b6ef539d37ca91903459260354a9368db5cd38d84903647259d8f1ac85a47943
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu7.1.tar.gz' xorg_7.7+19ubuntu7.1.tar.gz 298771 SHA512:6e3ac8b4932fc3ba476ce69fa5e111ed2f57b46e0b9361b01f631d82e635e8741088eedeeafdb0e13cf63cbedacf0a0872ca656ace349ecb6a79402f67522b6a
```

### `dpkg` source package: `xorgproto=2018.4-4`

Binary Packages:

- `x11proto-core-dev=2018.4-4`
- `x11proto-dev=2018.4-4`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2018.4-4
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4-4.dsc' xorgproto_2018.4-4.dsc 4059 SHA256:6279a145ce040d9301a0e2efdf203dd7d2822bc9a90e94de08d545c4b724d8e3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4.orig.tar.gz' xorgproto_2018.4.orig.tar.gz 493597 SHA256:8e48d851efea0e951bcb6cf0d537f84ba3803de95e488bd039fe59fc75ec8f7d
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4.orig.tar.gz.asc' xorgproto_2018.4.orig.tar.gz.asc 241 SHA256:3ab131cf8f497d315043b2c791912c22045da557e6894f1e5db533a0b0baed2f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4-4.diff.gz' xorgproto_2018.4-4.diff.gz 20976 SHA256:a9b27658c7c9e53372679bbb26099abed6cb9215355a99995858164de3fa5048
```

### `dpkg` source package: `xtrans=1.3.5-1`

Binary Packages:

- `xtrans-dev=1.3.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xtrans=1.3.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5-1.dsc' xtrans_1.3.5-1.dsc 1901 SHA256:64750bc2dd993ac93b9e0a8d6109ce72963ab22296479145eb3f392d238c2280
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5.orig.tar.gz' xtrans_1.3.5.orig.tar.gz 227536 SHA256:b7a577c1b6c75030145e53b4793db9c88f9359ac49e7d771d4385d21b3e5945d
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5-1.diff.gz' xtrans_1.3.5-1.diff.gz 16122 SHA256:2acb2c4f5958ef1bbae74ca64007d0465261a4f62bfad6ed22f1f144c0e445e1
```

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
'http://archive.ubuntu.com/ubuntu/pool/universe/x/xvidcore/xvidcore_1.3.5-1.dsc' xvidcore_1.3.5-1.dsc 2131 SHA256:36b1e21f8767346d8698c13ad560961336726c2cb206b7097715d421abdf8192
'http://archive.ubuntu.com/ubuntu/pool/universe/x/xvidcore/xvidcore_1.3.5.orig.tar.bz2' xvidcore_1.3.5.orig.tar.bz2 698846 SHA256:7c20f279f9d8e89042e85465d2bcb1b3130ceb1ecec33d5448c4589d78f010b4
'http://archive.ubuntu.com/ubuntu/pool/universe/x/xvidcore/xvidcore_1.3.5-1.debian.tar.xz' xvidcore_1.3.5-1.debian.tar.xz 6180 SHA256:06166aa04159f8c451d53f1ae70cbf65a65d325b4769f779dc009894ca801e08
```

### `dpkg` source package: `xz-utils=5.2.2-1.3`

Binary Packages:

- `liblzma5:amd64=5.2.2-1.3`
- `xz-utils=5.2.2-1.3`

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

### `dpkg` source package: `zeromq3=4.2.5-1ubuntu0.2`

Binary Packages:

- `libzmq5:amd64=4.2.5-1ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libzmq5/copyright`)

- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-3`
- `LGPL-3.0+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris zeromq3=4.2.5-1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zeromq3/zeromq3_4.2.5-1ubuntu0.2.dsc' zeromq3_4.2.5-1ubuntu0.2.dsc 1973 SHA512:63b6318b3c835b5cab4c8589d9d66f1bd3765ab45565707e777fac19ed0cd671fe13e763358c238bcb5c4b8a694998500d3138e9509e56c61034d1fdb11bb824
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zeromq3/zeromq3_4.2.5.orig.tar.gz' zeromq3_4.2.5.orig.tar.gz 1409447 SHA512:4556cb50d05a6d133015a0ba804d6d951a47479a33fa29561eaeecb93d48b7bb6477365d0986c38b779f500cadaf08522c4a7aa13f5510303bd923f794d37036
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zeromq3/zeromq3_4.2.5-1ubuntu0.2.debian.tar.xz' zeromq3_4.2.5-1ubuntu0.2.debian.tar.xz 22840 SHA512:9618ff385a838b28756488663271a6da228b941b462aea99edec6ab7be7159be62b8777c7ce9dc5894f93bd7f34385eb3040a1abae76be0757ed232e5e29e423
```

### `dpkg` source package: `zip=3.0-11build1`

Binary Packages:

- `zip=3.0-11build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zip=3.0-11build1
'http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0-11build1.dsc' zip_3.0-11build1.dsc 1658 SHA256:47bc14d9970340a3469117770adca913c1c1803547f847366f37562d78979904
'http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0.orig.tar.gz' zip_3.0.orig.tar.gz 1118845 SHA256:f0e8bb1f9b7eb0b01285495a2699df3a4b766784c1765a8f1aeedf63c0806369
'http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0-11build1.debian.tar.xz' zip_3.0-11build1.debian.tar.xz 8308 SHA256:3011af4bcde82439198f97af23220e6ba4837de9aaa68811688bd48a990c7981
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
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zvbi/zvbi_0.2.35-13.dsc' zvbi_0.2.35-13.dsc 2109 SHA256:8ac47d2f6354995b0302f780ae4447388e1929d72d3bf9ab893a5e87deba4399
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zvbi/zvbi_0.2.35.orig.tar.bz2' zvbi_0.2.35.orig.tar.bz2 1047761 SHA256:fc883c34111a487c4a783f91b1b2bb5610d8d8e58dcba80c7ab31e67e4765318
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zvbi/zvbi_0.2.35-13.debian.tar.xz' zvbi_0.2.35-13.debian.tar.xz 15184 SHA256:9199d10d014a76498dc6ef08424b13863c689775e877e3d425d8437b85895886
```
