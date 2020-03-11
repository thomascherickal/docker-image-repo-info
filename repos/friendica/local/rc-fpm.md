# `friendica:2020.03-rc-fpm`

## Docker Metadata

- Image ID: `sha256:d60de0487a641c78a27527f991636dad36e8f5c30f672bae5894e5f6bf096e18`
- Created: `2020-03-10T23:29:37.45427036Z`
- Virtual Size: ~ 427.81 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/entrypoint-dev.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie`
  - `GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D`
  - `PHP_VERSION=7.3.15`
  - `PHP_URL=https://www.php.net/get/php-7.3.15.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://www.php.net/get/php-7.3.15.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=de7ae7cf3d1dbb2824975b26b32991dac2b732886ec22075b8c53b261b018166`
  - `PHP_MD5=`
  - `TINI_VERSION=v0.18.0`
  - `FRIENDICA_VERSION=2020.03-rc`
  - `FRIENDICA_ADDONS=2020.03-rc`

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

### `dpkg` source package: `autoconf=2.69-10`

Binary Packages:

- `autoconf=2.69-10`

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
$ apt-get source -qq --print-uris autoconf=2.69-10
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-10.dsc' autoconf_2.69-10.dsc 1948 SHA256:0e8c77d8a268f0a797ea53c7396620fac549272259a50a6fe0c5b5941f1ac95f
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-10.debian.tar.xz' autoconf_2.69-10.debian.tar.xz 23048 SHA256:f294c3ba40fd942b4119175401bf57191f08429916a8b9bf3d04f53567c96d35
```

Other potentially useful URLs:

- https://sources.debian.net/src/autoconf/2.69-10/ (for browsing the source)
- https://sources.debian.net/src/autoconf/2.69-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autoconf/2.69-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=9.9+deb9u12`

Binary Packages:

- `base-files=9.9+deb9u12`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=9.9+deb9u12
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_9.9+deb9u12.dsc' base-files_9.9+deb9u12.dsc 1099 SHA256:838bfc2cef4cfcda5f0d44274b2f0f92658a6ad13db21d3df562bbb7e6cb0ccc
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_9.9+deb9u12.tar.xz' base-files_9.9+deb9u12.tar.xz 63200 SHA256:0f06aee1432ee2d0d3133ba7c72d4b9b5a7a869d37ac006d438e258037da098e
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/9.9+deb9u12/ (for browsing the source)
- https://sources.debian.net/src/base-files/9.9+deb9u12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/9.9+deb9u12/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `curl=7.52.1-5+deb9u10`

Binary Packages:

- `curl=7.52.1-5+deb9u10`
- `libcurl3:amd64=7.52.1-5+deb9u10`
- `libcurl3-gnutls:amd64=7.52.1-5+deb9u10`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.52.1-5+deb9u10
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.52.1-5+deb9u10.dsc' curl_7.52.1-5+deb9u10.dsc 2822 SHA256:313cd1eeb23ee0cb069040ab48d3d4fba08811d14b1581647b0e0bf303747160
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.52.1.orig.tar.gz' curl_7.52.1.orig.tar.gz 3504621 SHA256:a8984e8b20880b621f61a62d95ff3c0763a3152093a9f9ce4287cfd614add6ae
'http://security.debian.org/debian-security/pool/updates/main/c/curl/curl_7.52.1-5+deb9u10.debian.tar.xz' curl_7.52.1-5+deb9u10.debian.tar.xz 43360 SHA256:014f6df474eb55469883314060bef68c04334862ff8d543c04bec6f5fae4542c
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.52.1-5+deb9u10/ (for browsing the source)
- https://sources.debian.net/src/curl/7.52.1-5+deb9u10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.52.1-5+deb9u10/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.dsc' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.dsc 3381 SHA256:a331441098ece65be5bf13d871b486115af68daf06a0145adf6cda8ef71d73e4
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz 1143888 SHA256:69f34971f768e7ee6a6b647ec2d16a5a72a854ecd4602b019d5f79ba61063fdc
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.debian.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3+deb9u1.debian.tar.xz 94992 SHA256:be1ba4b3bfcc4740354342686deac73ca2e46c4871219599229efe8cfe98df6f
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27~101-g0780600+dfsg-3+deb9u1/ (for access to the source package after it no longer exists in the archive)

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
- `dpkg-dev=1.18.25`
- `libdpkg-perl=1.18.25`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

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

### `dpkg` source package: `file=1:5.30-1+deb9u3`

Binary Packages:

- `file=1:5.30-1+deb9u3`
- `libmagic-mgc=1:5.30-1+deb9u3`
- `libmagic1:amd64=1:5.30-1+deb9u3`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.30-1+deb9u3
'http://deb.debian.org/debian/pool/main/f/file/file_5.30-1+deb9u3.dsc' file_5.30-1+deb9u3.dsc 2166 SHA256:ef90aa103f3ed04e3c8b199533a2197405599a38bc8091fb8170b20d6d7a18c2
'http://deb.debian.org/debian/pool/main/f/file/file_5.30.orig.tar.xz' file_5.30.orig.tar.xz 578628 SHA256:813feaa00da67897b652aa2f0bdeba46f1a265223071a3ea0591476b4e1b0291
'http://deb.debian.org/debian/pool/main/f/file/file_5.30-1+deb9u3.debian.tar.xz' file_5.30-1+deb9u3.debian.tar.xz 40224 SHA256:03fa6392b9681915e386d93baa729ebbde3fa1d204a34368eb1877302ebbf4d7
```

Other potentially useful URLs:

- https://sources.debian.net/src/file/1:5.30-1+deb9u3/ (for browsing the source)
- https://sources.debian.net/src/file/1:5.30-1+deb9u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/file/1:5.30-1+deb9u3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `fontconfig=2.11.0-6.7`

Binary Packages:

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

### `dpkg` source package: `freetype=2.6.3-3.2+deb9u1`

Binary Packages:

- `libfreetype6:amd64=2.6.3-3.2+deb9u1`

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
$ apt-get source -qq --print-uris freetype=2.6.3-3.2+deb9u1
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.6.3-3.2+deb9u1.dsc' freetype_2.6.3-3.2+deb9u1.dsc 2165 SHA256:3722fb56c793ba2a93e46bb3156c81430247a3be84841b07290af1d2c5df9bfa
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.6.3.orig.tar.gz' freetype_2.6.3.orig.tar.gz 7313547 SHA256:814a22aad85e8ca2cb4acfc2e9dc59caa6eded4f6619590f7bd0a721e4b076a3
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.6.3-3.2+deb9u1.diff.gz' freetype_2.6.3-3.2+deb9u1.diff.gz 40763 SHA256:26822de2fe918a287779817dea689660bee1bfcf69ba43977b9b32b16a56bba3
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.6.3-3.2+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.6.3-3.2+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.6.3-3.2+deb9u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-6=6.3.0-18+deb9u1`

Binary Packages:

- `cpp-6=6.3.0-18+deb9u1`
- `g++-6=6.3.0-18+deb9u1`
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

Licenses: (parsed from: `/usr/share/doc/cpp-6/copyright`, `/usr/share/doc/g++-6/copyright`, `/usr/share/doc/gcc-6/copyright`, `/usr/share/doc/gcc-6-base/copyright`, `/usr/share/doc/libasan3/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-6-dev/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libmpx2/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-6-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan0/copyright`)

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
- `g++=4:6.3.0-4`
- `gcc=4:6.3.0-4`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

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
'http://deb.debian.org/debian/pool/main/g/git/git_2.11.0-3+deb9u5.dsc' git_2.11.0-3+deb9u5.dsc 2944 SHA256:0a0eeebee1b417f964ab45a0cec7c2a0835639960da68b86db618776bae6521f
'http://deb.debian.org/debian/pool/main/g/git/git_2.11.0.orig.tar.xz' git_2.11.0.orig.tar.xz 4197984 SHA256:7e7e8d69d494892373b87007674be5820a4bc1ef596a0117d03ea3169119fd0b
'http://deb.debian.org/debian/pool/main/g/git/git_2.11.0-3+deb9u5.debian.tar.xz' git_2.11.0-3+deb9u5.debian.tar.xz 572380 SHA256:ccf9c4a9c59ddc34df84b72e8bf8226328359abbf91205c397fabbb7c8168d8d
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.11.0-3+deb9u5/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.11.0-3+deb9u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.11.0-3+deb9u5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glib2.0=2.50.3-2+deb9u2`

Binary Packages:

- `libglib2.0-0:amd64=2.50.3-2+deb9u2`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.50.3-2+deb9u2
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.50.3-2+deb9u2.dsc' glib2.0_2.50.3-2+deb9u2.dsc 3278 SHA256:04b8ae6238d36052ef753615f8278b69df8b91922c15776409a1a60e3eec3b00
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.50.3.orig.tar.xz' glib2.0_2.50.3.orig.tar.xz 7589284 SHA256:82ee94bf4c01459b6b00cb9db0545c2237921e3060c0b74cff13fbc020cfd999
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.50.3-2+deb9u2.debian.tar.xz' glib2.0_2.50.3-2+deb9u2.debian.tar.xz 77776 SHA256:f6d26084bf06135d85188f881790d9e0c5e706d24735af68cafa5d96f3da7fd4
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.50.3-2+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.50.3-2+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.50.3-2+deb9u2/ (for access to the source package after it no longer exists in the archive)

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

- `libgnutls-openssl27:amd64=3.5.8-5+deb9u4`
- `libgnutls30:amd64=3.5.8-5+deb9u4`

Licenses: (parsed from: `/usr/share/doc/libgnutls-openssl27/copyright`, `/usr/share/doc/libgnutls30/copyright`)

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

### `dpkg` source package: `imagemagick=8:6.9.7.4+dfsg-11+deb9u7`

Binary Packages:

- `imagemagick-6-common=8:6.9.7.4+dfsg-11+deb9u7`
- `libmagickcore-6.q16-3:amd64=8:6.9.7.4+dfsg-11+deb9u7`
- `libmagickwand-6.q16-3:amd64=8:6.9.7.4+dfsg-11+deb9u7`

Licenses: (parsed from: `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/libmagickcore-6.q16-3/copyright`, `/usr/share/doc/libmagickwand-6.q16-3/copyright`)

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

### `dpkg` source package: `libidn=1.33-1+deb9u1`

Binary Packages:

- `libidn11:amd64=1.33-1+deb9u1`

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
$ apt-get source -qq --print-uris libidn=1.33-1+deb9u1
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33-1+deb9u1.dsc' libidn_1.33-1+deb9u1.dsc 1640 SHA256:39ba49fd4df8faa36b581ff20cc09406d1ecd54e505503f17f0994e899c097d2
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33.orig.tar.gz' libidn_1.33.orig.tar.gz 3501056 SHA256:44a7aab635bb721ceef6beecc4d49dfd19478325e1b47f3196f7d2acc4930e19
'http://deb.debian.org/debian/pool/main/libi/libidn/libidn_1.33-1+deb9u1.debian.tar.xz' libidn_1.33-1+deb9u1.debian.tar.xz 63132 SHA256:b1c50fd09aa7c3a54f4715ff7c673731a1fabcd3118053be15f65918e9481bb9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn/1.33-1+deb9u1/ (for browsing the source)
- https://sources.debian.net/src/libidn/1.33-1+deb9u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn/1.33-1+deb9u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libmemcached=1.0.18-4.1`

Binary Packages:

- `libmemcached11:amd64=1.0.18-4.1`
- `libmemcachedutil2:amd64=1.0.18-4.1`

Licenses: (parsed from: `/usr/share/doc/libmemcached11/copyright`, `/usr/share/doc/libmemcachedutil2/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-Sun`
- `BSD-3-clause-TangentOrg`
- `Bob-Jenkins`
- `Paul-Hsieh`
- `RSA-Data-Security`

Source:

```console
$ apt-get source -qq --print-uris libmemcached=1.0.18-4.1
'http://deb.debian.org/debian/pool/main/libm/libmemcached/libmemcached_1.0.18-4.1.dsc' libmemcached_1.0.18-4.1.dsc 2361 SHA256:46d0a33ebc984f2d6fccb8618262f303038bba51a0a0b017325c91b084d2de24
'http://deb.debian.org/debian/pool/main/libm/libmemcached/libmemcached_1.0.18.orig.tar.gz' libmemcached_1.0.18.orig.tar.gz 1039649 SHA256:e22c0bb032fde08f53de9ffbc5a128233041d9f33b5de022c0978a2149885f82
'http://deb.debian.org/debian/pool/main/libm/libmemcached/libmemcached_1.0.18-4.1.debian.tar.xz' libmemcached_1.0.18-4.1.debian.tar.xz 12212 SHA256:1b969428b177da00c22219df6bc908594b7d5d9bb5b9857173411d3cbf892e93
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmemcached/1.0.18-4.1/ (for browsing the source)
- https://sources.debian.net/src/libmemcached/1.0.18-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmemcached/1.0.18-4.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libsigsegv=2.10-5`

Binary Packages:

- `libsigsegv2:amd64=2.10-5`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.10-5
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.10-5.dsc' libsigsegv_2.10-5.dsc 2176 SHA256:92d54f05c061e7a3fb58e6a697b249014c6bf3e9d9364fce8d31e39c9e978d94
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.10.orig.tar.gz' libsigsegv_2.10.orig.tar.gz 402279 SHA256:8460a4a3dd4954c3d96d7a4f5dd5bc4d9b76f5754196aa245287553b26d2199a
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.10-5.debian.tar.xz' libsigsegv_2.10-5.debian.tar.xz 10196 SHA256:91c32dce30bee0e8a27f6a546338253662551b29ec4b15583217b9408e057ece
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsigsegv/2.10-5/ (for browsing the source)
- https://sources.debian.net/src/libsigsegv/2.10-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsigsegv/2.10-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libx11=2:1.6.4-3+deb9u1`

Binary Packages:

- `libx11-6:amd64=2:1.6.4-3+deb9u1`
- `libx11-data=2:1.6.4-3+deb9u1`

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

### `dpkg` source package: `libzip=1.1.2-1.1`

Binary Packages:

- `libzip4:amd64=1.1.2-1.1+b1`

Licenses: (parsed from: `/usr/share/doc/libzip4/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libzip=1.1.2-1.1
'http://deb.debian.org/debian/pool/main/libz/libzip/libzip_1.1.2-1.1.dsc' libzip_1.1.2-1.1.dsc 2162 SHA256:f973d6fb8838bb220a7ae297e19bf822b256509dc0bf53ab7374183ea7cbc651
'http://deb.debian.org/debian/pool/main/libz/libzip/libzip_1.1.2.orig.tar.gz' libzip_1.1.2.orig.tar.gz 671193 SHA256:59ac7c09b0aa9aa7e21849c236d0a66a97aa6d442d78335c2fdfe0ee16366221
'http://deb.debian.org/debian/pool/main/libz/libzip/libzip_1.1.2-1.1.debian.tar.xz' libzip_1.1.2-1.1.debian.tar.xz 4940 SHA256:49e5589eb16f16cc6a8011e1613d5e1a41e39ae7ca8bb576c11d181e745532bb
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzip/1.1.2-1.1/ (for browsing the source)
- https://sources.debian.net/src/libzip/1.1.2-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzip/1.1.2-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `linux=4.9.210-1`

Binary Packages:

- `linux-libc-dev:amd64=4.9.210-1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `CRYPTOGAMS`
- `GPL-2`
- `LGPL-2.1`
- `Unicode-data`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=4.9.210-1
'http://deb.debian.org/debian/pool/main/l/linux/linux_4.9.210-1.dsc' linux_4.9.210-1.dsc 125025 SHA256:f16e4a27ca2f36fc78746b706a0df5c28860c18a7e6bf53d7392f115edb5868d
'http://deb.debian.org/debian/pool/main/l/linux/linux_4.9.210.orig.tar.xz' linux_4.9.210.orig.tar.xz 94867552 SHA256:4e3d283a6fdc8f6bdf74df8a79d0367c6d3f6033da25a23119b153a7e22ace57
'http://deb.debian.org/debian/pool/main/l/linux/linux_4.9.210-1.debian.tar.xz' linux_4.9.210-1.debian.tar.xz 1277320 SHA256:930d4102fb0ecf86af74186b0081aabd3855d1fd525441e0b7bb30095c4aec2f
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/4.9.210-1/ (for browsing the source)
- https://sources.debian.net/src/linux/4.9.210-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/4.9.210-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `m4=1.4.18-1`

Binary Packages:

- `m4=1.4.18-1`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-1
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-1.dsc' m4_1.4.18-1.dsc 1426 SHA256:83a6c5e4b94aa47634b7c988fa485155c01120c17682865e6f032de9adf1090c
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-1.debian.tar.xz' m4_1.4.18-1.debian.tar.xz 15784 SHA256:55de78acb0272fd6e2637ab933114e64eefa58ba1e97b063629453ae1e163fff
```

Other potentially useful URLs:

- https://sources.debian.net/src/m4/1.4.18-1/ (for browsing the source)
- https://sources.debian.net/src/m4/1.4.18-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/m4/1.4.18-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `make-dfsg=4.1-9.1`

Binary Packages:

- `make=4.1-9.1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.1-9.1
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.1-9.1.dsc' make-dfsg_4.1-9.1.dsc 2037 SHA256:3527e91633b0d2830a52f3b85229b2f8bdec5e1e5b77bbff95b20317757ab3a3
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.1.orig.tar.gz' make-dfsg_4.1.orig.tar.gz 1350231 SHA256:b3ed04fb6718289e4a430afbe2df6ecba9177aad9f6d09aaf38e5409262ca8a3
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.1-9.1.diff.gz' make-dfsg_4.1-9.1.diff.gz 45452 SHA256:ec9d39ed253808378aeb91bb2c34bbd177637ed197682e093c3aadfb97b338a3
```

Other potentially useful URLs:

- https://sources.debian.net/src/make-dfsg/4.1-9.1/ (for browsing the source)
- https://sources.debian.net/src/make-dfsg/4.1-9.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/make-dfsg/4.1-9.1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.18.1-1+deb9u1.dsc' nghttp2_1.18.1-1+deb9u1.dsc 2657 SHA256:fc99fa8d124d322f7cd872c3088a268ea86f42e71229fc98d8a90869950d0a14
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.18.1.orig.tar.bz2' nghttp2_1.18.1.orig.tar.bz2 1780766 SHA256:5d8bb930eb90c552ec836c7b1862406b69cafcda5520bf266c8f5d914d9b447c
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.18.1-1+deb9u1.debian.tar.xz' nghttp2_1.18.1-1+deb9u1.debian.tar.xz 12300 SHA256:94cf473ee6a78181ebdddc18676df356fb788540cf426b7eca944573f2808733
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

### `dpkg` source package: `openjpeg2=2.1.2-1.1+deb9u4`

Binary Packages:

- `libopenjp2-7:amd64=2.1.2-1.1+deb9u4`

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
$ apt-get source -qq --print-uris openjpeg2=2.1.2-1.1+deb9u4
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.1.2-1.1+deb9u4.dsc' openjpeg2_2.1.2-1.1+deb9u4.dsc 2623 SHA256:f3830f5cb00a22cc544d762bdc864e65e9393d040142ddd79b5d3d6169802968
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.1.2.orig.tar.gz' openjpeg2_2.1.2.orig.tar.gz 1987071 SHA256:4ce77b6ef538ef090d9bde1d5eeff8b3069ab56c4906f083475517c2c023dfa7
'http://deb.debian.org/debian/pool/main/o/openjpeg2/openjpeg2_2.1.2-1.1+deb9u4.debian.tar.xz' openjpeg2_2.1.2-1.1+deb9u4.debian.tar.xz 26744 SHA256:18fd3d6617216bab817581a05e80317579eccef3f43c5f26da6f0fcf4db23d0a
```

Other potentially useful URLs:

- https://sources.debian.net/src/openjpeg2/2.1.2-1.1+deb9u4/ (for browsing the source)
- https://sources.debian.net/src/openjpeg2/2.1.2-1.1+deb9u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openjpeg2/2.1.2-1.1+deb9u4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `openssl1.0=1.0.2u-1~deb9u1`

Binary Packages:

- `libssl1.0.2:amd64=1.0.2u-1~deb9u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl1.0=1.0.2u-1~deb9u1
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2u-1~deb9u1.dsc' openssl1.0_1.0.2u-1~deb9u1.dsc 2383 SHA256:35e2627956512ce933f91e66ecb4a276200d8d1ab67ee599fc1a8dd7ae0a183a
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2u.orig.tar.gz' openssl1.0_1.0.2u.orig.tar.gz 5355412 SHA256:ecd0c6ffb493dd06707d38b14bb4d8c2288bb7033735606569d8f90f89669d16
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2u.orig.tar.gz.asc' openssl1.0_1.0.2u.orig.tar.gz.asc 488 SHA256:84d7a8b23df5567e80e3732f69c5428ee533a2bc7c3c2264dd8390a7af2a8620
'http://deb.debian.org/debian/pool/main/o/openssl1.0/openssl1.0_1.0.2u-1~deb9u1.debian.tar.xz' openssl1.0_1.0.2u-1~deb9u1.debian.tar.xz 94808 SHA256:2b3beb8c675e7ede236e7f54ebad5df277c995722c9a85ca6e0033896119db7c
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

- `libp11-kit0:amd64=0.23.3-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

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

### `dpkg` source package: `patch=2.7.5-1+deb9u2`

Binary Packages:

- `patch=2.7.5-1+deb9u2`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.5-1+deb9u2
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.5-1+deb9u2.dsc' patch_2.7.5-1+deb9u2.dsc 1840 SHA256:3e6b3452b6a658b5762b198a94f1ac5af6bb687f90e5749a7f5af12364ffa269
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.5.orig.tar.xz' patch_2.7.5.orig.tar.xz 727704 SHA256:fd95153655d6b95567e623843a0e77b81612d502ecf78a489a4aed7867caa299
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.5-1+deb9u2.debian.tar.xz' patch_2.7.5-1+deb9u2.debian.tar.xz 13036 SHA256:c094ca6eabeb6c7fe3ea964bd242a2f018c5e2ce5b82cc4e977b37e214109c6e
```

Other potentially useful URLs:

- https://sources.debian.net/src/patch/2.7.5-1+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/patch/2.7.5-1+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/patch/2.7.5-1+deb9u2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `perl=5.24.1-3+deb9u6`

Binary Packages:

- `libperl5.24:amd64=5.24.1-3+deb9u6`
- `perl=5.24.1-3+deb9u6`
- `perl-base=5.24.1-3+deb9u6`
- `perl-modules-5.24=5.24.1-3+deb9u6`

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
$ apt-get source -qq --print-uris perl=5.24.1-3+deb9u6
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.24.1-3+deb9u6.dsc' perl_5.24.1-3+deb9u6.dsc 2397 SHA256:5c61985fb955a4b756f7d5502977f6f28178f477a21e4b0a42f265fbda76d412
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.24.1.orig.tar.xz' perl_5.24.1.orig.tar.xz 11569284 SHA256:03a77bac4505c270f1890ece75afc7d4b555090b41aa41ea478747e23b2afb3f
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.24.1-3+deb9u6.debian.tar.xz' perl_5.24.1-3+deb9u6.debian.tar.xz 186028 SHA256:55452dc45712a3a80dd16f796278bf1748582f28e9754131aea282a4719aebbd
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.24.1-3+deb9u6/ (for browsing the source)
- https://sources.debian.net/src/perl/5.24.1-3+deb9u6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.24.1-3+deb9u6/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `popt=1.16-10`

Binary Packages:

- `libpopt0:amd64=1.16-10+b2`

Licenses: (parsed from: `/usr/share/doc/libpopt0/copyright`)

- `GPL-2`
- `GPL-2+`
- `X-Consortium`

Source:

```console
$ apt-get source -qq --print-uris popt=1.16-10
'http://deb.debian.org/debian/pool/main/p/popt/popt_1.16-10.dsc' popt_1.16-10.dsc 1800 SHA256:874c8f002ef0f8d0c704cf136af58079983e7dc2646bf4322f6fe9261ddfe4a7
'http://deb.debian.org/debian/pool/main/p/popt/popt_1.16.orig.tar.gz' popt_1.16.orig.tar.gz 702769 SHA256:e728ed296fe9f069a0e005003c3d6b2dde3d9cad453422a10d6558616d304cc8
'http://deb.debian.org/debian/pool/main/p/popt/popt_1.16-10.debian.tar.xz' popt_1.16-10.debian.tar.xz 14136 SHA256:8300cbb47148f59fc6edc2f8ebe227a319b080ed26d17db846d1e346f0614899
```

Other potentially useful URLs:

- https://sources.debian.net/src/popt/1.16-10/ (for browsing the source)
- https://sources.debian.net/src/popt/1.16-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/popt/1.16-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `re2c=0.16-2`

Binary Packages:

- `re2c=0.16-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris re2c=0.16-2
'http://deb.debian.org/debian/pool/main/r/re2c/re2c_0.16-2.dsc' re2c_0.16-2.dsc 1409 SHA256:3bffc53b5d992e5fc8da101d3059339e0ea4a67eae876e105c85d7939ce81581
'http://deb.debian.org/debian/pool/main/r/re2c/re2c_0.16.orig.tar.gz' re2c_0.16.orig.tar.gz 4892417 SHA256:48c12564297641cceb5ff05aead57f28118db6277f31e2262437feba89069e84
'http://deb.debian.org/debian/pool/main/r/re2c/re2c_0.16-2.debian.tar.xz' re2c_0.16-2.debian.tar.xz 5060 SHA256:da2356059e82a247af002c72424709543cd6ea18c04f3dc3ac553b8cc56822e4
```

Other potentially useful URLs:

- https://sources.debian.net/src/re2c/0.16-2/ (for browsing the source)
- https://sources.debian.net/src/re2c/0.16-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/re2c/0.16-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `rsync=3.1.2-1+deb9u2`

Binary Packages:

- `rsync=3.1.2-1+deb9u2`

Licenses: (parsed from: `/usr/share/doc/rsync/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris rsync=3.1.2-1+deb9u2
'http://deb.debian.org/debian/pool/main/r/rsync/rsync_3.1.2-1+deb9u2.dsc' rsync_3.1.2-1+deb9u2.dsc 1717 SHA256:7ff035929408e160639c0d27c56ea910e561b5858da724ba1e88104855d8b065
'http://deb.debian.org/debian/pool/main/r/rsync/rsync_3.1.2.orig.tar.gz' rsync_3.1.2.orig.tar.gz 892724 SHA256:ecfa62a7fa3c4c18b9eccd8c16eaddee4bd308a76ea50b5c02a5840f09c0a1c2
'http://deb.debian.org/debian/pool/main/r/rsync/rsync_3.1.2-1+deb9u2.debian.tar.xz' rsync_3.1.2-1+deb9u2.debian.tar.xz 31156 SHA256:9c9b13658cf79ba0171337574365837f0b40696f0e615f794dbfecc2c562fc84
```

Other potentially useful URLs:

- https://sources.debian.net/src/rsync/3.1.2-1+deb9u2/ (for browsing the source)
- https://sources.debian.net/src/rsync/3.1.2-1+deb9u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rsync/3.1.2-1+deb9u2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ssmtp=2.64-8`

Binary Packages:

- `ssmtp=2.64-8+b2`

Licenses: (parsed from: `/usr/share/doc/ssmtp/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ssmtp=2.64-8
'http://deb.debian.org/debian/pool/main/s/ssmtp/ssmtp_2.64-8.dsc' ssmtp_2.64-8.dsc 1819 SHA256:0b115e9b555a267d35d1fc81b7a245f0a1104085ead361b862b913836d961238
'http://deb.debian.org/debian/pool/main/s/ssmtp/ssmtp_2.64.orig.tar.bz2' ssmtp_2.64.orig.tar.bz2 52501 SHA256:22c37dc90c871e8e052b2cab0ad219d010fa938608cd66b21c8f3c759046fa36
'http://deb.debian.org/debian/pool/main/s/ssmtp/ssmtp_2.64-8.debian.tar.bz2' ssmtp_2.64-8.debian.tar.bz2 37916 SHA256:2ed9caf0a14d4d5a44837a4a76cd5c9a52e527e2eb7a300eb328d90cc97917f0
```

Other potentially useful URLs:

- https://sources.debian.net/src/ssmtp/2.64-8/ (for browsing the source)
- https://sources.debian.net/src/ssmtp/2.64-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ssmtp/2.64-8/ (for access to the source package after it no longer exists in the archive)

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
