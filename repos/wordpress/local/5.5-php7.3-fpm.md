# `wordpress:5.5.1-php7.3-fpm`

## Docker Metadata

- Image ID: `sha256:1b041c1f340b64ad1d490e4cfe2ef1b5a1a75c929e6be77ea02d85cca1ba4df9`
- Created: `2020-10-12T17:50:13.635102138Z`
- Virtual Size: ~ 530.14 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D`
  - `PHP_VERSION=7.3.23`
  - `PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc`
  - `PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034`
  - `PHP_MD5=`
  - `WORDPRESS_VERSION=5.5.1`
  - `WORDPRESS_SHA1=d3316a4ffff2a12cf92fde8bfdd1ff8691e41931`

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

### `dpkg` source package: `apt=1.8.2.1`

Binary Packages:

- `apt=1.8.2.1`
- `libapt-pkg5.0:amd64=1.8.2.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.8.2.1
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.8.2.1.dsc' apt_1.8.2.1.dsc 2774 SHA256:8e6af99e5eab948853dcffde8bf8b2cc9acdd53fcdadf3505a3c0234b69eabb1
'http://deb.debian.org/debian/pool/main/a/apt/apt_1.8.2.1.tar.xz' apt_1.8.2.1.tar.xz 2189236 SHA256:6d447f2e9437ec24e78350b63bb0592bee1f050811d51990b0c783183b0983f8
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/1.8.2.1/ (for browsing the source)
- https://sources.debian.net/src/apt/1.8.2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/1.8.2.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `autoconf=2.69-11`

Binary Packages:

- `autoconf=2.69-11`

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
$ apt-get source -qq --print-uris autoconf=2.69-11
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-11.dsc' autoconf_2.69-11.dsc 1948 SHA256:249d25370d4f4d1d0cf7b37bfd178bb6fa87011566dd82230991f64814a39dde
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://deb.debian.org/debian/pool/main/a/autoconf/autoconf_2.69-11.debian.tar.xz' autoconf_2.69-11.debian.tar.xz 23540 SHA256:885b3947fdead5b737f6437b80a90a41c5d611791573c5d0cfef50a59c943c1b
```

Other potentially useful URLs:

- https://sources.debian.net/src/autoconf/2.69-11/ (for browsing the source)
- https://sources.debian.net/src/autoconf/2.69-11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/autoconf/2.69-11/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `base-files=10.3+deb10u5`

Binary Packages:

- `base-files=10.3+deb10u5`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-files/10.3+deb10u5/


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

### `dpkg` source package: `binutils=2.31.1-16`

Binary Packages:

- `binutils=2.31.1-16`
- `binutils-common:amd64=2.31.1-16`
- `binutils-x86-64-linux-gnu=2.31.1-16`
- `libbinutils:amd64=2.31.1-16`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.31.1-16
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.31.1-16.dsc' binutils_2.31.1-16.dsc 11421 SHA256:ec76c13684d922a3619d7ec982db191714927bde6de6a3ff89e95d1ce7a61f33
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.31.1.orig.tar.xz' binutils_2.31.1.orig.tar.xz 21649228 SHA256:e398a2d579faa0f2b5a988add5f7481af8e21a21f63b6ea5702e6f517960c5eb
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.31.1-16.debian.tar.xz' binutils_2.31.1-16.debian.tar.xz 127464 SHA256:15fc82a7c682da6bcbf56caf57da8f059655369cbfeb58b8312040e53e4fa11d
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.31.1-16/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.31.1-16/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.31.1-16/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ca-certificates=20200601~deb10u1`

Binary Packages:

- `ca-certificates=20200601~deb10u1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20200601~deb10u1
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20200601~deb10u1.dsc' ca-certificates_20200601~deb10u1.dsc 1837 SHA256:41120aa922b9520b73b88ef3fef18b807c7e5b6dd98c9dec51a3841dabe7fcb8
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20200601~deb10u1.tar.xz' ca-certificates_20200601~deb10u1.tar.xz 245828 SHA256:5911c0471fd83141285c56c414be7f6e7176f28dc8d14a3c55f06303b79a92aa
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20200601~deb10u1/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20200601~deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20200601~deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `cups=2.2.10-6+deb10u3`

Binary Packages:

- `libcups2:amd64=2.2.10-6+deb10u3`
- `libcupsimage2:amd64=2.2.10-6+deb10u3`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`, `/usr/share/doc/libcupsimage2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.2.10-6+deb10u3
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10-6+deb10u3.dsc' cups_2.2.10-6+deb10u3.dsc 3472 SHA256:abd15985e6eb1be56761a11f94ac3754fcf9f2e068a82ec5c23967808e1c933d
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10.orig.tar.gz' cups_2.2.10.orig.tar.gz 10403568 SHA256:77c8b2b3bb7fe8b5fbfffc307f2c817b2d7ec67b657f261a1dd1c61ab81205bb
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10.orig.tar.gz.asc' cups_2.2.10.orig.tar.gz.asc 864 SHA256:be235dd0cc526e5bde2a67f0dc2888be5d8dc40d1dfa44ab1a322d83f606e82d
'http://deb.debian.org/debian/pool/main/c/cups/cups_2.2.10-6+deb10u3.debian.tar.xz' cups_2.2.10-6+deb10u3.debian.tar.xz 360856 SHA256:73ce4319b9008bb96e196b00ca9bc114a4dd66371d84ed2f63e82a67afb66007
```

Other potentially useful URLs:

- https://sources.debian.net/src/cups/2.2.10-6+deb10u3/ (for browsing the source)
- https://sources.debian.net/src/cups/2.2.10-6+deb10u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cups/2.2.10-6+deb10u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `curl=7.64.0-4+deb10u1`

Binary Packages:

- `curl=7.64.0-4+deb10u1`
- `libcurl4:amd64=7.64.0-4+deb10u1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.64.0-4+deb10u1
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.64.0-4+deb10u1.dsc' curl_7.64.0-4+deb10u1.dsc 2719 SHA256:bdbc61f9785516009ae74bb3775e21bed7ab8fdd7bfef4a1a4f471d5218adf3e
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.64.0.orig.tar.gz' curl_7.64.0.orig.tar.gz 4032645 SHA256:cb90d2eb74d4e358c1ed1489f8e3af96b50ea4374ad71f143fa4595e998d81b5
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.64.0-4+deb10u1.debian.tar.xz' curl_7.64.0-4+deb10u1.debian.tar.xz 34156 SHA256:911407ad8d73d0592db7f1a015656089563bb7dab279ec33bff855adf56bcf1b
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

### `dpkg` source package: `dbus=1.12.20-0+deb10u1`

Binary Packages:

- `libdbus-1-3:amd64=1.12.20-0+deb10u1`

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
$ apt-get source -qq --print-uris dbus=1.12.20-0+deb10u1
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20-0+deb10u1.dsc' dbus_1.12.20-0+deb10u1.dsc 3928 SHA256:38fc131a229914bdf8d3945992e53a3a7abab048c6d28c49014389fdbdc642fd
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20.orig.tar.gz' dbus_1.12.20.orig.tar.gz 2095511 SHA256:f77620140ecb4cdc67f37fb444f8a6bea70b5b6461f12f1cbe2cec60fa7de5fe
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20.orig.tar.gz.asc' dbus_1.12.20.orig.tar.gz.asc 833 SHA256:a5f4d51c9c95a6cf7270abb6548894d91d51eebc0e9f996d0951c8ee925894e7
'http://deb.debian.org/debian/pool/main/d/dbus/dbus_1.12.20-0+deb10u1.debian.tar.xz' dbus_1.12.20-0+deb10u1.debian.tar.xz 63300 SHA256:52dafb74ae52ab16159635db7762bdd41c584e292d3e93f84872b47df6004f49
```

Other potentially useful URLs:

- https://sources.debian.net/src/dbus/1.12.20-0+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/dbus/1.12.20-0+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dbus/1.12.20-0+deb10u1/ (for access to the source package after it no longer exists in the archive)

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
- `dpkg-dev=1.19.7`
- `libdpkg-perl=1.19.7`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

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

### `dpkg` source package: `file=1:5.35-4+deb10u1`

Binary Packages:

- `file=1:5.35-4+deb10u1`
- `libmagic-mgc=1:5.35-4+deb10u1`
- `libmagic1:amd64=1:5.35-4+deb10u1`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.35-4+deb10u1
'http://deb.debian.org/debian/pool/main/f/file/file_5.35-4+deb10u1.dsc' file_5.35-4+deb10u1.dsc 1984 SHA256:d1e2d532fc2cf5cfd947b98152916b28c7a6f2c0d6b5da460dea4bc34ca01607
'http://deb.debian.org/debian/pool/main/f/file/file_5.35.orig.tar.xz' file_5.35.orig.tar.xz 643268 SHA256:60b5b8bc762d35452c7995f3db7e8a5e2004d736b8763f086585a5b1af57a632
'http://deb.debian.org/debian/pool/main/f/file/file_5.35-4+deb10u1.debian.tar.xz' file_5.35-4+deb10u1.debian.tar.xz 56264 SHA256:7bbb38f82e1d461d923ca9a3bd9691ebca1920d04d2d78199b098c40474e9dcb
```

Other potentially useful URLs:

- https://sources.debian.net/src/file/1:5.35-4+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/file/1:5.35-4+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/file/1:5.35-4+deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `fontconfig=2.13.1-2`

Binary Packages:

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

### `dpkg` source package: `gcc-8=8.3.0-6`

Binary Packages:

- `cpp-8=8.3.0-6`
- `g++-8=8.3.0-6`
- `gcc-8=8.3.0-6`
- `gcc-8-base:amd64=8.3.0-6`
- `libasan5:amd64=8.3.0-6`
- `libatomic1:amd64=8.3.0-6`
- `libcc1-0:amd64=8.3.0-6`
- `libgcc-8-dev:amd64=8.3.0-6`
- `libgcc1:amd64=1:8.3.0-6`
- `libgomp1:amd64=8.3.0-6`
- `libitm1:amd64=8.3.0-6`
- `liblsan0:amd64=8.3.0-6`
- `libmpx2:amd64=8.3.0-6`
- `libquadmath0:amd64=8.3.0-6`
- `libstdc++-8-dev:amd64=8.3.0-6`
- `libstdc++6:amd64=8.3.0-6`
- `libtsan0:amd64=8.3.0-6`
- `libubsan1:amd64=8.3.0-6`

Licenses: (parsed from: `/usr/share/doc/cpp-8/copyright`, `/usr/share/doc/g++-8/copyright`, `/usr/share/doc/gcc-8/copyright`, `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/libasan5/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-8-dev/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libmpx2/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-8-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

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

### `dpkg` source package: `gcc-defaults=1.181`

Binary Packages:

- `cpp=4:8.3.0-1`
- `g++=4:8.3.0-1`
- `gcc=4:8.3.0-1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.181
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.181.dsc' gcc-defaults_1.181.dsc 15508 SHA256:d89d80502009816bac8e77c423c3f7d4e6fb4b684f036fae785dacf4454ddc75
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.181.tar.gz' gcc-defaults_1.181.tar.gz 72227 SHA256:39c34b070fc29223ba42ae6d53653a8f02fdbc0e9d6ca3245de9b19d2c6e9d07
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-defaults/1.181/ (for browsing the source)
- https://sources.debian.net/src/gcc-defaults/1.181/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-defaults/1.181/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ghostscript=9.27~dfsg-2+deb10u4`

Binary Packages:

- `ghostscript=9.27~dfsg-2+deb10u4`
- `libgs9:amd64=9.27~dfsg-2+deb10u4`
- `libgs9-common=9.27~dfsg-2+deb10u4`

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
$ apt-get source -qq --print-uris ghostscript=9.27~dfsg-2+deb10u4
'http://deb.debian.org/debian/pool/main/g/ghostscript/ghostscript_9.27~dfsg-2+deb10u4.dsc' ghostscript_9.27~dfsg-2+deb10u4.dsc 2795 SHA256:b787519674b83e21473218d5889b8e84f6b590483a7b43e3dcac4698ef2d2660
'http://deb.debian.org/debian/pool/main/g/ghostscript/ghostscript_9.27~dfsg.orig.tar.xz' ghostscript_9.27~dfsg.orig.tar.xz 17723588 SHA256:b90d2117e93c63d774a5ab0a4d6a19c5dcbfd877462ee39a405262948e23ff9b
'http://deb.debian.org/debian/pool/main/g/ghostscript/ghostscript_9.27~dfsg-2+deb10u4.debian.tar.xz' ghostscript_9.27~dfsg-2+deb10u4.debian.tar.xz 124824 SHA256:f9c6d314ade320d6c69dddea99426c90136f90651b4d4bc673f45287f5146e70
```

Other potentially useful URLs:

- https://sources.debian.net/src/ghostscript/9.27~dfsg-2+deb10u4/ (for browsing the source)
- https://sources.debian.net/src/ghostscript/9.27~dfsg-2+deb10u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ghostscript/9.27~dfsg-2+deb10u4/ (for access to the source package after it no longer exists in the archive)

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
- `libc-dev-bin=2.28-10`
- `libc6:amd64=2.28-10`
- `libc6-dev:amd64=2.28-10`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

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

- `gpgv=2.2.12-1+deb10u1`

Licenses: (parsed from: `/usr/share/doc/gpgv/copyright`)

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

### `dpkg` source package: `gnutls28=3.6.7-4+deb10u5`

Binary Packages:

- `libgnutls30:amd64=3.6.7-4+deb10u5`

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
$ apt-get source -qq --print-uris gnutls28=3.6.7-4+deb10u5
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7-4+deb10u5.dsc' gnutls28_3.6.7-4+deb10u5.dsc 3354 SHA256:d91aef3a450b7dceef817264996a3c11b72dd7fb8e892897b63d7e52bd078e4a
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7.orig.tar.xz' gnutls28_3.6.7.orig.tar.xz 8153728 SHA256:5b3409ad5aaf239808730d1ee12fdcd148c0be00262c7edf157af655a8a188e2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7.orig.tar.xz.asc' gnutls28_3.6.7.orig.tar.xz.asc 534 SHA256:a14d0a7b9295b65ae797a70f8e765024a2e363dca03d008bfce0aec2b3f292b0
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.7-4+deb10u5.debian.tar.xz' gnutls28_3.6.7-4+deb10u5.debian.tar.xz 89484 SHA256:d719d468f59aef1c480dda91ffee6d0c728e8635a0808f199d999d04f128b70a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.6.7-4+deb10u5/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.6.7-4+deb10u5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.6.7-4+deb10u5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `icu=63.1-6+deb10u1`

Binary Packages:

- `libicu63:amd64=63.1-6+deb10u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=63.1-6+deb10u1
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.1-6+deb10u1.dsc' icu_63.1-6+deb10u1.dsc 1997 SHA256:c33329e44a83af47cdfd6ca2639611d960b163a5cce39e71945b0ed4b6971ec9
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.1.orig.tar.xz' icu_63.1.orig.tar.xz 13638120 SHA256:347d0e6c39c3538b812c10c6c83815d4a089d578380387ae7d94c5b820948e82
'http://deb.debian.org/debian/pool/main/i/icu/icu_63.1-6+deb10u1.debian.tar.xz' icu_63.1-6+deb10u1.debian.tar.xz 25004 SHA256:d65fde3a61d0ba935b493b46fd42addeb24e0398b8d778124cb489770ec50a6d
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/63.1-6+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/icu/63.1-6+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/63.1-6+deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1+deb10u1`

Binary Packages:

- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1+deb10u1`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1+deb10u1`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1+deb10u1`

Licenses: (parsed from: `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/libmagickcore-6.q16-6/copyright`, `/usr/share/doc/libmagickwand-6.q16-6/copyright`)

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.10.23+dfsg-2.1+deb10u1
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1+deb10u1.dsc' imagemagick_6.9.10.23+dfsg-2.1+deb10u1.dsc 5162 SHA256:7981932a55bdef29fe5815fcad267933603c5aa7530ba4f3e42fafc3abfff394
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg.orig.tar.xz' imagemagick_6.9.10.23+dfsg.orig.tar.xz 9081188 SHA256:44249112b624f2cc315573fa96685e547da27ebb321432259290c407023c531e
'http://deb.debian.org/debian/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1+deb10u1.debian.tar.xz' imagemagick_6.9.10.23+dfsg-2.1+deb10u1.debian.tar.xz 237856 SHA256:a713bde913942f58fa7a6f004c12ce6fe94342a0befc47ef27d948f3007d45a2
```

Other potentially useful URLs:

- https://sources.debian.net/src/imagemagick/8:6.9.10.23+dfsg-2.1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/imagemagick/8:6.9.10.23+dfsg-2.1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/imagemagick/8:6.9.10.23+dfsg-2.1+deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `isl=0.20-2`

Binary Packages:

- `libisl19:amd64=0.20-2`

Licenses: (parsed from: `/usr/share/doc/libisl19/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.20-2
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.20-2.dsc' isl_0.20-2.dsc 1842 SHA256:466b881ac0207f9430ae21069e644f17a6e4428544f9802284727381e5d26089
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.20.orig.tar.xz' isl_0.20.orig.tar.xz 1539064 SHA256:a5596a9fb8a5b365cb612e4b9628735d6e67e9178fae134a816ae195017e77aa
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.20-2.debian.tar.xz' isl_0.20-2.debian.tar.xz 23512 SHA256:ea2b467fea2395ca08f236f520fcc37e50a1c91cad471a9ee89443bfae8f50af
```

Other potentially useful URLs:

- https://sources.debian.net/src/isl/0.20-2/ (for browsing the source)
- https://sources.debian.net/src/isl/0.20-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/isl/0.20-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libsigsegv=2.12-2`

Binary Packages:

- `libsigsegv2:amd64=2.12-2`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.12-2
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12-2.dsc' libsigsegv_2.12-2.dsc 2363 SHA256:b081b244de2f427345838f379405d8438c29db1fa746a4e270167ae7cb10c079
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz' libsigsegv_2.12.orig.tar.gz 451408 SHA256:3ae1af359eebaa4ffc5896a1aee3568c052c99879316a1ab57f8fe1789c390b6
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz.asc' libsigsegv_2.12.orig.tar.gz.asc 2442 SHA256:1861a9a182bbb7a24a18f7e43fe0fa3eb6f6fd53780b30e01990677112694dfc
'http://deb.debian.org/debian/pool/main/libs/libsigsegv/libsigsegv_2.12-2.debian.tar.xz' libsigsegv_2.12-2.debian.tar.xz 8340 SHA256:73940fb346f7afd90c93a341164cd175349e0507de8b1c05b0834b598c372260
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsigsegv/2.12-2/ (for browsing the source)
- https://sources.debian.net/src/libsigsegv/2.12-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsigsegv/2.12-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libx11=2:1.6.7-1+deb10u1`

Binary Packages:

- `libx11-6:amd64=2:1.6.7-1+deb10u1`
- `libx11-data=2:1.6.7-1+deb10u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.7-1+deb10u1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7-1+deb10u1.dsc' libx11_1.6.7-1+deb10u1.dsc 2651 SHA256:32165ead57fed813168f87bd43d5dd387c2a27bba4c77bd8e8075cee90f90fce
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7.orig.tar.gz' libx11_1.6.7.orig.tar.gz 2972354 SHA256:f62ab88c2a87b55e1dc338726a55bb6ed8048084fe6a3294a7ae324ca45159d1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7.orig.tar.gz.asc' libx11_1.6.7.orig.tar.gz.asc 404 SHA256:01a06afbe0574a30721d98f1c80b668ebc46410a9e8b2eb81e69b4bd8667c386
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.6.7-1+deb10u1.diff.gz' libx11_1.6.7-1+deb10u1.diff.gz 52461 SHA256:ea3a943ea781136b3d5320010039e42039b0e58d5aeeca2d2b7a0593f9ce04ef
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.6.7-1+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.6.7-1+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.6.7-1+deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libzip=1.5.1-4`

Binary Packages:

- `libzip4:amd64=1.5.1-4`

Licenses: (parsed from: `/usr/share/doc/libzip4/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libzip=1.5.1-4
'http://deb.debian.org/debian/pool/main/libz/libzip/libzip_1.5.1-4.dsc' libzip_1.5.1-4.dsc 2216 SHA256:833e56bddbc7ef960af36bf0ded714af1a4f50a39aea2df6d8a65ba9ad67bc8f
'http://deb.debian.org/debian/pool/main/libz/libzip/libzip_1.5.1.orig.tar.xz' libzip_1.5.1.orig.tar.xz 717908 SHA256:04ea35b6956c7b3453f1ed3f3fe40e3ddae1f43931089124579e8384e79ed372
'http://deb.debian.org/debian/pool/main/libz/libzip/libzip_1.5.1-4.debian.tar.xz' libzip_1.5.1-4.debian.tar.xz 7980 SHA256:9ecaa728e3c5db11ba80c3047bd79557f3d318be9c6adc069c8aefecfee13cf3
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzip/1.5.1-4/ (for browsing the source)
- https://sources.debian.net/src/libzip/1.5.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzip/1.5.1-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `linux=4.19.132-1`

Binary Packages:

- `linux-libc-dev:amd64=4.19.132-1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `CRYPTOGAMS`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `Unicode-data`
- `X11`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=4.19.132-1
'http://deb.debian.org/debian/pool/main/l/linux/linux_4.19.132-1.dsc' linux_4.19.132-1.dsc 191615 SHA256:3431e9f27ad196e3cd3b0908b5ac5008ed2522118c4f51fd8f8a8c1240819e28
'http://deb.debian.org/debian/pool/main/l/linux/linux_4.19.132.orig.tar.xz' linux_4.19.132.orig.tar.xz 107498852 SHA256:3e9e811d44d190dcd8af04e86ad4c00032a5b74cafece51cfd12581648e4e1db
'http://deb.debian.org/debian/pool/main/l/linux/linux_4.19.132-1.debian.tar.xz' linux_4.19.132-1.debian.tar.xz 3308396 SHA256:c592597164270d5cfbf7efa12a04d8246ba26e2d9228bb8ae030ef88b147fe40
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/4.19.132-1/ (for browsing the source)
- https://sources.debian.net/src/linux/4.19.132-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/4.19.132-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `m4=1.4.18-2`

Binary Packages:

- `m4=1.4.18-2`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-2
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-2.dsc' m4_1.4.18-2.dsc 1426 SHA256:93dda06744f90619c4666515c9b5bc51aa584519c16cafd1e74aaa3733628c1b
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://deb.debian.org/debian/pool/main/m/m4/m4_1.4.18-2.debian.tar.xz' m4_1.4.18-2.debian.tar.xz 17032 SHA256:73718bae96a2f63f0ed38c614ea081074914698207e73450da571461af1c58ec
```

Other potentially useful URLs:

- https://sources.debian.net/src/m4/1.4.18-2/ (for browsing the source)
- https://sources.debian.net/src/m4/1.4.18-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/m4/1.4.18-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `make-dfsg=4.2.1-1.2`

Binary Packages:

- `make=4.2.1-1.2`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.2.1-1.2
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.dsc' make-dfsg_4.2.1-1.2.dsc 2019 SHA256:0c8a2da5d51e03bf43e2929322d5a8406f08e5ee2d81a71ed6e5a8734f1b05cb
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.2.1.orig.tar.gz' make-dfsg_4.2.1.orig.tar.gz 1485018 SHA256:480405e8995796ea47cc54b281b7855280f0d815d296a1af1993eeeb72074e39
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.diff.gz' make-dfsg_4.2.1-1.2.diff.gz 53108 SHA256:80e0b96cee381391a5d3322317075e23d8474c92c5fa4fecd334bc2e0920887b
```

Other potentially useful URLs:

- https://sources.debian.net/src/make-dfsg/4.2.1-1.2/ (for browsing the source)
- https://sources.debian.net/src/make-dfsg/4.2.1-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/make-dfsg/4.2.1-1.2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mpclib3=1.1.0-1`

Binary Packages:

- `libmpc3:amd64=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.1.0-1
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.1.0-1.dsc' mpclib3_1.1.0-1.dsc 1990 SHA256:bb57824015b735bf72399a53f8c6a241e6a8bd402753b0fdcdaa5b99d0aef790
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.1.0.orig.tar.gz' mpclib3_1.1.0.orig.tar.gz 701263 SHA256:6985c538143c1208dcb1ac42cedad6ff52e267b47e5f970183a3e75125b43c2e
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.1.0-1.diff.gz' mpclib3_1.1.0-1.diff.gz 3794 SHA256:84b10a4ae958b3015e136b75be5fee22961255d19be655f7d0adae8d4f3bc977
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpclib3/1.1.0-1/ (for browsing the source)
- https://sources.debian.net/src/mpclib3/1.1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpclib3/1.1.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpfr4=4.0.2-1`

Binary Packages:

- `libmpfr6:amd64=4.0.2-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.0.2-1
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.0.2-1.dsc' mpfr4_4.0.2-1.dsc 1972 SHA256:9021ec2462ed0e73ea1379266740473abf5f826be819226497729f6c6b02e672
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.0.2.orig.tar.xz' mpfr4_4.0.2.orig.tar.xz 1441996 SHA256:1d3be708604eae0e42d578ba93b390c2a145f17743a744d8f3f8c2ad5855a38a
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.0.2-1.debian.tar.xz' mpfr4_4.0.2-1.debian.tar.xz 10544 SHA256:99c4d35654f33340f0efdec67142a34753157b20334cadad9018f5eab29738da
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpfr4/4.0.2-1/ (for browsing the source)
- https://sources.debian.net/src/mpfr4/4.0.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpfr4/4.0.2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `openldap=2.4.47+dfsg-3+deb10u2`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.47+dfsg-3+deb10u2`
- `libldap-common=2.4.47+dfsg-3+deb10u2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.47+dfsg-3+deb10u2
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.47+dfsg-3+deb10u2.dsc' openldap_2.4.47+dfsg-3+deb10u2.dsc 3022 SHA256:e909c6be4bfd1bacf644959bc18ebeebaa13606879f11a7876d044cd688a6f62
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.47+dfsg.orig.tar.gz' openldap_2.4.47+dfsg.orig.tar.gz 4872293 SHA256:8f1ac7a4be7dd8ef158361efbfe16509756d3d9b396f5f378c3cf5c727807651
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.47+dfsg-3+deb10u2.debian.tar.xz' openldap_2.4.47+dfsg-3+deb10u2.debian.tar.xz 168684 SHA256:0f6f81f18a2407bd1a6c6003659d8b33145f31033b6f7fd026607554f0bdfcb0
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.47+dfsg-3+deb10u2/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.47+dfsg-3+deb10u2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.47+dfsg-3+deb10u2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.1d-0+deb10u3`

Binary Packages:

- `libssl1.1:amd64=1.1.1d-0+deb10u3`
- `openssl=1.1.1d-0+deb10u3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1d-0+deb10u3
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d-0+deb10u3.dsc' openssl_1.1.1d-0+deb10u3.dsc 2472 SHA256:7dc19c6d2bf8ee424b3a39d49edd975e2a8b87655eb0a6a81431efde57a44b14
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d.orig.tar.gz' openssl_1.1.1d.orig.tar.gz 8845861 SHA256:1e3a91bc1f9dfce01af26026f856e064eab4c8ee0a8f457b5ae30b40b8b711f2
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d.orig.tar.gz.asc' openssl_1.1.1d.orig.tar.gz.asc 488 SHA256:f3fd3299a79421fffd51d35f62636b8e987dab1d3033d93a19d7685868e15395
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1d-0+deb10u3.debian.tar.xz' openssl_1.1.1d-0+deb10u3.debian.tar.xz 86692 SHA256:59db3dc3bf8e8abee0dc6dd6c62b644e57ac7a0e3ab98ace563885a4f3b205cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.1d-0+deb10u3/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.1d-0+deb10u3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.1d-0+deb10u3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.15-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.15-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

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

### `dpkg` source package: `patch=2.7.6-3+deb10u1`

Binary Packages:

- `patch=2.7.6-3+deb10u1`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-3+deb10u1
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-3+deb10u1.dsc' patch_2.7.6-3+deb10u1.dsc 1731 SHA256:dae4e0d25106b2d14d981309395371397091892359b44a919eb08dd841bee13f
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-3+deb10u1.debian.tar.xz' patch_2.7.6-3+deb10u1.debian.tar.xz 13164 SHA256:58d4e84bd4ce850152e1d1911546ac0aad9764992570c360cff8f9cf03eb37bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/patch/2.7.6-3+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/patch/2.7.6-3+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/patch/2.7.6-3+deb10u1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `perl=5.28.1-6+deb10u1`

Binary Packages:

- `libperl5.28:amd64=5.28.1-6+deb10u1`
- `perl=5.28.1-6+deb10u1`
- `perl-base=5.28.1-6+deb10u1`
- `perl-modules-5.28=5.28.1-6+deb10u1`

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
$ apt-get source -qq --print-uris perl=5.28.1-6+deb10u1
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1-6+deb10u1.dsc' perl_5.28.1-6+deb10u1.dsc 2863 SHA256:a680d97001398640c249fc6bae6124fe59eb465b044f03fb4148b22152895785
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1.orig-regen-configure.tar.xz' perl_5.28.1.orig-regen-configure.tar.xz 411944 SHA256:5873b81af4514d3910ab1a8267b15ff8c0e2100dbae4edfd10b65ef72cd31ef8
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1.orig.tar.xz' perl_5.28.1.orig.tar.xz 12372080 SHA256:fea7162d4cca940a387f0587b93f6737d884bf74d8a9d7cfd978bc12cd0b202d
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.28.1-6+deb10u1.debian.tar.xz' perl_5.28.1-6+deb10u1.debian.tar.xz 185004 SHA256:e531c2d8c85b28b34c2122175a8e8f6cfe56b8a0708972fc4beae9876549d815
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.28.1-6+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/perl/5.28.1-6+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.28.1-6+deb10u1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pkg-config=0.29-6`

Binary Packages:

- `pkg-config=0.29-6`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29-6
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29-6.dsc' pkg-config_0.29-6.dsc 1757 SHA256:a5f1a8f976f3d8ad579341ba73514eb3af9dbc6bad8d2b5828699ac24196624f
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.orig.tar.gz' pkg-config_0.29.orig.tar.gz 1973875 SHA256:c8507705d2a10c67f385d66ca2aae31e81770cc0734b4191eb8c489e864a006b
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29-6.diff.gz' pkg-config_0.29-6.diff.gz 8145 SHA256:c06146d878fb7faa4ac3edb5e45188b184cc650a752384d5c1053f41edf590bc
```

Other potentially useful URLs:

- https://sources.debian.net/src/pkg-config/0.29-6/ (for browsing the source)
- https://sources.debian.net/src/pkg-config/0.29-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pkg-config/0.29-6/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `re2c=1.1.1-1`

Binary Packages:

- `re2c=1.1.1-1`

Licenses: (parsed from: `/usr/share/doc/re2c/copyright`)

- `PHP-3.01`
- `Zend-2.00`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris re2c=1.1.1-1
'http://deb.debian.org/debian/pool/main/r/re2c/re2c_1.1.1-1.dsc' re2c_1.1.1-1.dsc 1833 SHA256:dce993d2ca99b5ab360e9833a068ad615df6930a3424b4337bb888d426e85eae
'http://deb.debian.org/debian/pool/main/r/re2c/re2c_1.1.1.orig.tar.gz' re2c_1.1.1.orig.tar.gz 5907416 SHA256:856597337ea00b24ce91f549f79e6eece1b92ba5f8b63292cad66c14ac7451cf
'http://deb.debian.org/debian/pool/main/r/re2c/re2c_1.1.1-1.debian.tar.xz' re2c_1.1.1-1.debian.tar.xz 9032 SHA256:2f9e3637df4d4fc517ac274fbb3404aa891c3e61d111ffb40bcb9e103e5e9aec
```

Other potentially useful URLs:

- https://sources.debian.net/src/re2c/1.1.1-1/ (for browsing the source)
- https://sources.debian.net/src/re2c/1.1.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/re2c/1.1.1-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `systemd=241-7~deb10u4`

Binary Packages:

- `libsystemd0:amd64=241-7~deb10u4`
- `libudev1:amd64=241-7~deb10u4`

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
$ apt-get source -qq --print-uris systemd=241-7~deb10u4
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_241-7~deb10u4.dsc' systemd_241-7~deb10u4.dsc 4946 SHA256:52707608012c7b13d19ebbbfff704311e33f884f0f843811874e266dcf2faf71
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_241.orig.tar.gz' systemd_241.orig.tar.gz 7640538 SHA256:b2561a8e1d10a2c248253f0dda31a85dd6d69f2b54177de55e02cd1d2778316e
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_241-7~deb10u4.debian.tar.xz' systemd_241-7~deb10u4.debian.tar.xz 178136 SHA256:ff8ed4b3d9c30e14659278f17ea4cfc63c4b1af199a98a861abc670dfdd991cb
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/241-7~deb10u4/ (for browsing the source)
- https://sources.debian.net/src/systemd/241-7~deb10u4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/241-7~deb10u4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `tzdata=2020a-0+deb10u1`

Binary Packages:

- `tzdata=2020a-0+deb10u1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2020a-0+deb10u1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a-0+deb10u1.dsc' tzdata_2020a-0+deb10u1.dsc 2264 SHA256:24c86ca3f4755af8bd1ce2cd985382a490476f20006806fe5ec5c0f6b2a417c9
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz' tzdata_2020a.orig.tar.gz 397245 SHA256:547161eca24d344e0b5f96aff6a76b454da295dc14ed4ca50c2355043fb899a2
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz.asc' tzdata_2020a.orig.tar.gz.asc 833 SHA256:a92f085fe1e7f8bc0f0a0bc4432f27e6cf2d69e64d4a90958bd023eb0ccf45f9
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a-0+deb10u1.debian.tar.xz' tzdata_2020a-0+deb10u1.debian.tar.xz 104936 SHA256:df174cf4f4414006677b626f15b51a04762a2a0ef0171ce2f0c6856710a16d53
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2020a-0+deb10u1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2020a-0+deb10u1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2020a-0+deb10u1/ (for access to the source package after it no longer exists in the archive)

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
