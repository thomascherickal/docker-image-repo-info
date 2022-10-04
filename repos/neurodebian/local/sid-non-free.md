# `neurodebian:sid-non-free`

## Docker Metadata

- Image ID: `sha256:81848706649fb2dbee852abdf0bb3057a7a91e27e1a07658c87cf4fa3cf53e79`
- Created: `2022-09-13T13:43:36.433425373Z`
- Virtual Size: ~ 140.34 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.3.1-1`

Binary Packages:

- `libacl1:amd64=2.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.3.1-1
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-1.dsc' acl_2.3.1-1.dsc 2486 SHA256:6299780e84c240e79aae9886deaacc1bd8439a2a58f6a23749156f8a4d62572e
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz' acl_2.3.1.orig.tar.xz 355676 SHA256:c0234042e17f11306c23c038b08e5e070edb7be44bef6697fb8734dcff1c66b1
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz.asc' acl_2.3.1.orig.tar.xz.asc 833 SHA256:54fb8fcd6ae6901f2257e18d503e5e18ad956babf8d80d2ea29f280fc7264662
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-1.debian.tar.xz' acl_2.3.1-1.debian.tar.xz 27732 SHA256:900e8993f3a8b95e2c83fc7f530cc15b5cd165b6f517a639239f51cd60d06f2a
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.3.1-1/ (for browsing the source)
- https://sources.debian.net/src/acl/2.3.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.3.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.129`

Binary Packages:

- `adduser=3.129`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.129
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.129.dsc' adduser_3.129.dsc 1671 SHA256:1201331222be92b5e2eecdf41be2319ed0ea8af8746507133491ed0dad7fbabd
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.129.tar.xz' adduser_3.129.tar.xz 230752 SHA256:45a9f9a6c38961466d3539999c9f9b490d5491c777ab88346ea7a9d81ca56cc3
```

Other potentially useful URLs:

- https://sources.debian.net/src/adduser/3.129/ (for browsing the source)
- https://sources.debian.net/src/adduser/3.129/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adduser/3.129/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=2.5.2`

Binary Packages:

- `apt=2.5.2`
- `libapt-pkg6.0:amd64=2.5.2`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.5.2/


### `dpkg` source package: `attr=1:2.5.1-1`

Binary Packages:

- `libattr1:amd64=1:2.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.5.1-1
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-1.dsc' attr_2.5.1-1.dsc 2455 SHA256:c0bd0dcb0309cdcbd286b31bd97b2c93552ebb7f7634964f351098cd9191e132
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA256:db448a626f9313a1a970d636767316a8da32aede70518b8050fa0de7947adc32
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA256:67bc632e754efbadba846d0b40138b3fc3e306c3b909a9ba868c6dba1e2689d0
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-1.debian.tar.xz' attr_2.5.1-1.debian.tar.xz 27948 SHA256:7eb32437dca67cd24667432150dcb07d8c7d0526e1d3284ecef6833b35214cdf
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.5.1-1/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.5.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.5.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:3.0.7-1`

Binary Packages:

- `libaudit-common=1:3.0.7-1`
- `libaudit1:amd64=1:3.0.7-1+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/audit/1:3.0.7-1/


### `dpkg` source package: `base-files=12.2`

Binary Packages:

- `base-files=12.2`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-files/12.2/


### `dpkg` source package: `base-passwd=3.6.0`

Binary Packages:

- `base-passwd=3.6.0`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-passwd/3.6.0/


### `dpkg` source package: `bash=5.2~rc2-2`

Binary Packages:

- `bash=5.2~rc2-2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/bash/5.2~rc2-2/


### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `libbz2-1.0:amd64=1.0.8-5`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-5
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-5.dsc' bzip2_1.0.8-5.dsc 2206 SHA256:ed9c40f4de3f9e064535e15eac1c61a0f606763db98f4579dbc04067b94a8944
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://deb.debian.org/debian/pool/main/b/bzip2/bzip2_1.0.8-5.debian.tar.bz2' bzip2_1.0.8-5.debian.tar.bz2 26787 SHA256:d68c6eba11d70e14319e24ef1451880a03023b2b75364646adb117086db36039
```

Other potentially useful URLs:

- https://sources.debian.net/src/bzip2/1.0.8-5/ (for browsing the source)
- https://sources.debian.net/src/bzip2/1.0.8-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bzip2/1.0.8-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cdebconf=0.264`

Binary Packages:

- `libdebconfclient0:amd64=0.264`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.264
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.264.dsc' cdebconf_0.264.dsc 2707 SHA256:b41d5d2c77a6604978e2df61cfdb92dea858c87560c292b95d77a47d4bd8747c
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.264.tar.xz' cdebconf_0.264.tar.xz 281292 SHA256:e27599ad371674de8f38aa8b53461688591432e0691d02e183915b76d110050a
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.264/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.264/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.264/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.32-4.1`

Binary Packages:

- `coreutils=8.32-4.1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/coreutils/8.32-4.1/


### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg-8`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg-8`
- `libsasl2-modules-db:amd64=2.1.28+dfsg-8`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-2.2-clause`
- `BSD-3-clause`
- `BSD-3-clause-JANET`
- `BSD-3-clause-PADL`
- `BSD-4-clause`
- `BSD-4-clause-KTH`
- `BSD-4-clause-UC`
- `FSFULLR`
- `GPL-3`
- `GPL-3+`
- `IBM-as-is`
- `MIT-CMU`
- `MIT-Export`
- `MIT-OpenVision`
- `OpenLDAP`
- `OpenSSL`
- `RSA-MD`
- `SSLeay`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg-8
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-8.dsc' cyrus-sasl2_2.1.28+dfsg-8.dsc 3313 SHA256:ade8f5bd6c5c7c35e0ca8763be9876d75b2b2d30fa177c33731d17c78bf2af7b
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg.orig.tar.xz 797472 SHA256:a15886d7da5958bd27f35b7c871dd872f6dc5b9917c9b6b15e3de014c7dab3d9
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-8.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg-8.debian.tar.xz 97032 SHA256:fe16b1de437f3d02c073645e58365eb7997cb799faaac8b571b5e8f5e20585fd
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg-8/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.28+dfsg-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.11+git20210903+057cd650a4ed-9`

Binary Packages:

- `dash=0.5.11+git20210903+057cd650a4ed-9`

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
$ apt-get source -qq --print-uris dash=0.5.11+git20210903+057cd650a4ed-9
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-9.dsc' dash_0.5.11+git20210903+057cd650a4ed-9.dsc 1720 SHA256:dacd578e5fb925bda192f380e65ce17d3d06b2fc3dc8aba3b68a9a42646cce04
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed.orig.tar.xz' dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz 133320 SHA256:4fb06697f33f14fcd6b96cd4dfdd5b343c848a4bb69b7c04f1717767e4a117d3
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-9.debian.tar.xz' dash_0.5.11+git20210903+057cd650a4ed-9.debian.tar.xz 35488 SHA256:0314a8fa4bcd794c36b8e1c129587e125322b25db9d9cbb61cc9389a263ab242
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.11+git20210903+057cd650a4ed-9/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.11+git20210903+057cd650a4ed-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.11+git20210903+057cd650a4ed-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.10`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.10`

Licenses: (parsed from: `/usr/share/doc/libdb5.3/copyright`)

- `Artistic`
- `BSD-3-clause`
- `BSD-3-clause-fjord`
- `GPL`
- `GPL-3`
- `MIT-old`
- `Ms-PL`
- `Sleepycat`
- `TCL-like`
- `X11`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.10
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.10.dsc' db5.3_5.3.28+dfsg1-0.10.dsc 2964 SHA256:7bab820246eb763be7d04fcb2893bedb414f9b3cf7a29327e3530adfbca1963e
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.10.debian.tar.xz' db5.3_5.3.28+dfsg1-0.10.debian.tar.xz 34656 SHA256:2d2b3c6b4643e9c94db58f9540332e23a780d63afdc3fcabe66df01a343d6c65
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.10/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.79`

Binary Packages:

- `debconf=1.5.79`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.79
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.79.dsc' debconf_1.5.79.dsc 2082 SHA256:b6a438542c61b8ff8a58cc33dca17859875783945a0e516239369b7d80e3ca7c
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.79.tar.xz' debconf_1.5.79.tar.xz 570588 SHA256:3456338d4bc329b4140c87d91e76068852c3d354348f77aa3cfb98619c069164
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.79/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.79/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.79/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `debianutils=5.7-0.3`

Binary Packages:

- `debianutils=5.7-0.3`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.7-0.3
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.3.dsc' debianutils_5.7-0.3.dsc 1887 SHA256:134707c6467fb895332cf7520dbb2da33fb8b38b7844dec88e64ceb50647512a
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7.orig.tar.gz' debianutils_5.7.orig.tar.gz 257231 SHA256:27ec9e0e7e44dc8ab611aa576330471bacb07e4491ffecf0d3aa6909c92f9022
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.3.debian.tar.xz' debianutils_5.7-0.3.debian.tar.xz 22120 SHA256:c7117659c2913660e2ffa83aa1362c7a2b49a3f1e20fadcf72e64e589540ffe9
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/5.7-0.3/ (for browsing the source)
- https://sources.debian.net/src/debianutils/5.7-0.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/5.7-0.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `diffutils=1:3.8-1`

Binary Packages:

- `diffutils=1:3.8-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.8-1
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8-1.dsc' diffutils_3.8-1.dsc 1705 SHA256:f00b310d95fce4312f44c4940b374fa3c2b5ccfcb53b6daa4e4a98e2bb47b58a
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz' diffutils_3.8.orig.tar.xz 1585120 SHA256:a6bdd7d1b31266d11c4f4de6c1b748d4607ab0231af5188fc2533d0ae2438fec
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz.asc' diffutils_3.8.orig.tar.xz.asc 833 SHA256:500f423d0ffa8d28966d916ed5fc6b79fb160a20ed5cb74eeb1c94a30c340311
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8-1.debian.tar.xz' diffutils_3.8-1.debian.tar.xz 11004 SHA256:120b1eaecd0cb09eb60cddaf616d269684f2f2b796ee6d9ca7aa4e16af517767
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.8-1/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.21.9`

Binary Packages:

- `dpkg=1.21.9`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.9
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.9.dsc' dpkg_1.21.9.dsc 2120 SHA256:065ee6146fecf372c587fd6f2083cda8704f9b3e20d1816f0972307cdee0c0ac
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.9.tar.xz' dpkg_1.21.9.tar.xz 5084044 SHA256:a0aba375625459260cbc89933a12b3188a713c840e3aaefc14bf2d9adee19642
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.21.9/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.21.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.21.9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.46.5-2`

Binary Packages:

- `e2fsprogs=1.46.5-2`
- `libcom-err2:amd64=1.46.5-2`
- `libext2fs2:amd64=1.46.5-2`
- `libss2:amd64=1.46.5-2`
- `logsave=1.46.5-2`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/e2fsprogs/1.46.5-2/


### `dpkg` source package: `findutils=4.9.0-3`

Binary Packages:

- `findutils=4.9.0-3`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.9.0-3
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-3.dsc' findutils_4.9.0-3.dsc 2304 SHA256:509979a2aeae2883c16b4bf6e96b4b8df9173a6c56e936e957ce86f25b2b4125
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA256:a2bfb8c09d436770edc59f50fa483e785b161a3b7b9d547573cb08065fd462fe
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA256:924c3719d066eda1b3e47175f8b83e90e9a23f0a639ebe7445621917b283c385
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-3.debian.tar.xz' findutils_4.9.0-3.debian.tar.xz 27980 SHA256:d10dfc7a728d372b60d5455b190b6ee78bc65de0ee3ca4974e1addd90389c675
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.9.0-3/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.9.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.9.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-12=12.2.0-2`

Binary Packages:

- `gcc-12-base:amd64=12.2.0-2`
- `libgcc-s1:amd64=12.2.0-2`
- `libstdc++6:amd64=12.2.0-2`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12.2.0-2
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.2.0-2.dsc' gcc-12_12.2.0-2.dsc 27405 SHA256:92bcfa21cfb1ef2e4a369c2b9e3aed19d100146d34b6e145e6c5bf92e2d52a0a
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.2.0.orig.tar.gz' gcc-12_12.2.0.orig.tar.gz 87090343 SHA256:b8298be16aeeb96a889c6afed0a8e2241b47452e89cc81fe65ea849d5c740fcb
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.2.0-2.debian.tar.xz' gcc-12_12.2.0-2.debian.tar.xz 1554016 SHA256:9cc8b6b48caed1e81d2df59de5f67371e625922e8b0930ec542da9f5b896f25d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-12/12.2.0-2/ (for browsing the source)
- https://sources.debian.net/src/gcc-12/12.2.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-12/12.2.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.34-8`

Binary Packages:

- `libc-bin=2.34-8`
- `libc6:amd64=2.34-8`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.34-8
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.34-8.dsc' glibc_2.34-8.dsc 9682 SHA256:1c03c57d3ffb285642966900c1a15166b97189ff6f914950a4a0f6535a421a01
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.34.orig.tar.xz' glibc_2.34.orig.tar.xz 17949940 SHA256:cc13047c7d42748108fc18cf1a4de8ca92f9e5c9bfcee09d6fada21d9a479878
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.34-8.debian.tar.xz' glibc_2.34-8.debian.tar.xz 1000880 SHA256:91fde9acd48db895f6face4bbe72ecb56e234dbea79dd0b1e390b4d1e7236321
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.34-8/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.34-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.34-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.1+dfsg1-1`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg1-1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg1-1
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.dsc' gmp_6.2.1+dfsg1-1.dsc 2230 SHA256:7a2ca2112db9f7ddf46c14d56ee3ed5ffbc7f4b4b33f843c6167533cc4334ae8
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1.orig.tar.xz' gmp_6.2.1+dfsg1.orig.tar.xz 1787428 SHA256:471b9e463e04362a0124f215afc5f0a4b99caedeeb62634c61bbc12988efa64c
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.debian.tar.xz' gmp_6.2.1+dfsg1-1.debian.tar.xz 19244 SHA256:35a11ed82eb0b612cb39e6136099880c4693035ea29d79828a050300a8b6dd6b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg1-1/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.39-1`

Binary Packages:

- `dirmngr=2.2.39-1`
- `gnupg=2.2.39-1`
- `gnupg-l10n=2.2.39-1`
- `gnupg-utils=2.2.39-1`
- `gpg=2.2.39-1`
- `gpg-agent=2.2.39-1`
- `gpg-wks-client=2.2.39-1`
- `gpg-wks-server=2.2.39-1`
- `gpgconf=2.2.39-1`
- `gpgsm=2.2.39-1`
- `gpgv=2.2.39-1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.39-1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.39-1.dsc' gnupg2_2.2.39-1.dsc 3219 SHA256:32e8abac2cb73cc7dcbbd9fdd9c94b19ebefb034f5de6d7851627d3c247807a9
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.39.orig.tar.bz2' gnupg2_2.2.39.orig.tar.bz2 7290098 SHA256:ab74db6685f026d7c0a10b527ecddecd608606a1691d15fda5d0a7f7d27e4c2f
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.39.orig.tar.bz2.asc' gnupg2_2.2.39.orig.tar.bz2.asc 390 SHA256:e2ded32666b9cc72bbe7e78248ed3ae9ec827530fe346812e2f99f59e15701b3
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.39-1.debian.tar.xz' gnupg2_2.2.39-1.debian.tar.xz 61380 SHA256:943f823abb65b2912a3384ca5f9e3538d8384b1e48fe04385fa789829bc5413d
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.39-1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.39-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.39-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.7-2`

Binary Packages:

- `libgnutls30:amd64=3.7.7-2`

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
$ apt-get source -qq --print-uris gnutls28=3.7.7-2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7-2.dsc' gnutls28_3.7.7-2.dsc 3442 SHA256:caf3872d06109c778a247fa690c5056105095cb1e182541e251550675af8fd60
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7.orig.tar.xz' gnutls28_3.7.7.orig.tar.xz 6351664 SHA256:be9143d0d58eab64dba9b77114aaafac529b6c0d7e81de6bdf1c9b59027d2106
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7.orig.tar.xz.asc' gnutls28_3.7.7.orig.tar.xz.asc 996 SHA256:2ca7cc33027c6a2316db52869a4b721f73560e0ade2b7bd758228dbbcebc36e0
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.7-2.debian.tar.xz' gnutls28_3.7.7-2.debian.tar.xz 67348 SHA256:54f6f6fc220ad9df6acbb17b6a8d50152eed2150120d4ed2ca89d982c1ccb6ee
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.7-2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.8-1`

Binary Packages:

- `grep=3.8-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/grep/3.8-1/


### `dpkg` source package: `gzip=1.12-1`

Binary Packages:

- `gzip=1.12-1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.12-1
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12-1.dsc' gzip_1.12-1.dsc 2009 SHA256:49a287787a0b4fc816eb576c011c472d1f630ec1778dfa120bd7fce4a844c253
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12.orig.tar.xz' gzip_1.12.orig.tar.xz 825548 SHA256:ce5e03e519f637e1f814011ace35c4f87b33c0bbabeec35baf5fbd3479e91956
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12.orig.tar.xz.asc' gzip_1.12.orig.tar.xz.asc 833 SHA256:3ed9ab54452576e0be0d477c772c9f47baa36415133fef7dd1fcf7b15480ba32
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.12-1.debian.tar.xz' gzip_1.12-1.debian.tar.xz 18736 SHA256:fcf2317e8eeddd66766ec5f3853025b109bd13815ec86ed6563e1af68d17193a
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.12-1/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.12-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `init-system-helpers=1.64`

Binary Packages:

- `init-system-helpers=1.64`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/init-system-helpers/1.64/


### `dpkg` source package: `libassuan=2.5.5-4`

Binary Packages:

- `libassuan0:amd64=2.5.5-4`

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
$ apt-get source -qq --print-uris libassuan=2.5.5-4
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-4.dsc' libassuan_2.5.5-4.dsc 1997 SHA256:c4f06cdb1684b44ca17acb7804ee593e2164db5b6911b0a9ed338f840931630f
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2' libassuan_2.5.5.orig.tar.bz2 572263 SHA256:8e8c2fcc982f9ca67dcbb1d95e2dc746b1739a4668bc20b3a3c5be632edb34e4
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2.asc' libassuan_2.5.5.orig.tar.bz2.asc 228 SHA256:8bb0d1d818ac91fa27a8ebed2975dac12eac9a6e075dfba225cc488ac9b4133f
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-4.debian.tar.xz' libassuan_2.5.5-4.debian.tar.xz 13976 SHA256:d9d46edba0c5bff1aec978fb9a894662fe144b1abe2f2e21bea8c98dae3e508c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.5-4/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.5-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.5-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.8.3-1`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.8.3-1
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1.dsc' libcap-ng_0.8.3-1.dsc 1634 SHA256:1bf38dbc0c30bcbc776d2d5c25e31d89202de0858f9ca9379c993d55103d7ef0
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3.orig.tar.gz' libcap-ng_0.8.3.orig.tar.gz 455383 SHA256:bed6f6848e22bb2f83b5f764b2aef0ed393054e803a8e3a8711cb2a39e6b492d
'http://deb.debian.org/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1.debian.tar.xz' libcap-ng_0.8.3-1.debian.tar.xz 10488 SHA256:710577902c260f50f8cfc9d7e264131f880eab0581d12ceab17ebe48e2ac53c6
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap-ng/0.8.3-1/ (for browsing the source)
- https://sources.debian.net/src/libcap-ng/0.8.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap-ng/0.8.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap2=1:2.44-1`

Binary Packages:

- `libcap2:amd64=1:2.44-1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

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

### `dpkg` source package: `libeatmydata=130-2`

Binary Packages:

- `eatmydata=130-2`
- `libeatmydata1:amd64=130-2`

Licenses: (parsed from: `/usr/share/doc/eatmydata/copyright`, `/usr/share/doc/libeatmydata1/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libeatmydata=130-2
'http://deb.debian.org/debian/pool/main/libe/libeatmydata/libeatmydata_130-2.dsc' libeatmydata_130-2.dsc 2439 SHA256:684157c21533d3bfd15eca6481835180dfec175d6d8d355d108fba605202a0b5
'http://deb.debian.org/debian/pool/main/libe/libeatmydata/libeatmydata_130.orig.tar.gz' libeatmydata_130.orig.tar.gz 375627 SHA256:48731cd7e612ff73fd6339378fbbff38dd3bcf6c243593b0d9773ca0051541c0
'http://deb.debian.org/debian/pool/main/libe/libeatmydata/libeatmydata_130.orig.tar.gz.asc' libeatmydata_130.orig.tar.gz.asc 833 SHA256:9296d99f3f289b353c2134a065a7231aada7cea24d699d196283ce761a62c058
'http://deb.debian.org/debian/pool/main/libe/libeatmydata/libeatmydata_130-2.debian.tar.xz' libeatmydata_130-2.debian.tar.xz 15576 SHA256:bc242a47408c91714f25461d23fb9ad70e53b4252f8ef17ff589f2b16d78e9e9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libeatmydata/130-2/ (for browsing the source)
- https://sources.debian.net/src/libeatmydata/130-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libeatmydata/130-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.4.2-4`

Binary Packages:

- `libffi8:amd64=3.4.2-4`

Licenses: (parsed from: `/usr/share/doc/libffi8/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.2-4
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2-4.dsc' libffi_3.4.2-4.dsc 1948 SHA256:c7c4890a434795e41a77bddbca949fb904b022a70d8446c5a005ec0f9ed4c554
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2.orig.tar.gz' libffi_3.4.2.orig.tar.gz 1351355 SHA256:540fb721619a6aba3bdeef7d940d8e9e0e6d2c193595bc243241b77ff9e93620
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.2-4.debian.tar.xz' libffi_3.4.2-4.debian.tar.xz 8164 SHA256:06d936d00d43e7999d0bce0aa2e0f1550109295b8093de77e6453acb9eacfd19
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.4.2-4/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.4.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.4.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.10.1-2`

Binary Packages:

- `libgcrypt20:amd64=1.10.1-2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.1-2
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-2.dsc' libgcrypt20_1.10.1-2.dsc 2790 SHA256:aa95c53382f51ed57490496df3ccb47d0ce11de1995cef78b87f7875eba416fb
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2' libgcrypt20_1.10.1.orig.tar.bz2 3778457 SHA256:ef14ae546b0084cd84259f61a55e07a38c3b53afc0f546bffcef2f01baffe9de
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2.asc' libgcrypt20_1.10.1.orig.tar.bz2.asc 228 SHA256:9da6ae5e8b1c253607be7e951b568932740c143ee519f6b3392ece8211e84e33
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-2.debian.tar.xz' libgcrypt20_1.10.1-2.debian.tar.xz 36788 SHA256:96875b4209984bfd192ce05a06f72f86f2ac2279b987f6d8e2e07cb0c95e2f68
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.10.1-2/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.10.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.10.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.45-2`

Binary Packages:

- `libgpg-error0:amd64=1.45-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.45-2
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45-2.dsc' libgpg-error_1.45-2.dsc 2273 SHA256:aacc0e1d60caf48ada2f8c73fa35bcb0f5e6368dfd301a624f5ede9419835144
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45.orig.tar.bz2' libgpg-error_1.45.orig.tar.bz2 1015954 SHA256:570f8ee4fb4bff7b7495cff920c275002aea2147e9a1d220c068213267f80a26
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45.orig.tar.bz2.asc' libgpg-error_1.45.orig.tar.bz2.asc 390 SHA256:3a4bfe4d36842a74a9f48a961df517efae812f1d6e097d274f8db5783a828508
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.45-2.debian.tar.xz' libgpg-error_1.45-2.debian.tar.xz 18820 SHA256:677493c9636cdcbbd7124ee460703dcdf990d4a0982819f006701f94f6285c45
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.45-2/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.45-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.45-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libidn2=2.3.3-1`

Binary Packages:

- `libidn2-0:amd64=2.3.3-1+b1`

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
$ apt-get source -qq --print-uris libidn2=2.3.3-1
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3-1.dsc' libidn2_2.3.3-1.dsc 2206 SHA256:13865e96a0fed8dcb82767db65c946b56ed44fc1806d80d407c512ded2a83984
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz' libidn2_2.3.3.orig.tar.gz 2116946 SHA256:f3ac987522c00d33d44b323cae424e2cffcb4c63c6aa6cd1376edacbf1c36eb0
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz.asc' libidn2_2.3.3.orig.tar.gz.asc 228 SHA256:e8f2bdce5def6c239c2cc3220e808b19b14d3f7eb3a0e14851dd5c16fc9ad0ec
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.3-1.debian.tar.xz' libidn2_2.3.3-1.debian.tar.xz 15964 SHA256:b040c12276e1128394c2f84c97f7e45f340867fa9d0d0a0b9d8f043b1977db99
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.3.3-1/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.3.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.3.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libksba=1.6.0-3`

Binary Packages:

- `libksba8:amd64=1.6.0-3`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.0-3
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0-3.dsc' libksba_1.6.0-3.dsc 2472 SHA256:de87d32fced6fe9593815552043eec226aafc7e6a7f6b258c0f1dcf96adb0da5
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2' libksba_1.6.0.orig.tar.bz2 662120 SHA256:dad683e6f2d915d880aa4bed5cea9a115690b8935b78a1bbe01669189307a48b
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2.asc' libksba_1.6.0.orig.tar.bz2.asc 228 SHA256:c695098f67cc837071d899f0e15d993bcf29eaac8f1ca7428ee793d9c62c795c
'http://deb.debian.org/debian/pool/main/libk/libksba/libksba_1.6.0-3.debian.tar.xz' libksba_1.6.0-3.debian.tar.xz 15004 SHA256:17f8f9679d0dcaaa46d9f4974d2090e23d538206c37014177146b6a5201cf414
```

Other potentially useful URLs:

- https://sources.debian.net/src/libksba/1.6.0-3/ (for browsing the source)
- https://sources.debian.net/src/libksba/1.6.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libksba/1.6.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.5.4-1`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.4-1
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-1.dsc' libseccomp_2.5.4-1.dsc 2676 SHA256:2986473126cb5f3e358fed40ec1482816e1068dbdfe938bf9f80c50afcf32b80
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz' libseccomp_2.5.4.orig.tar.gz 637228 SHA256:d82902400405cf0068574ef3dc1fe5f5926207543ba1ae6f8e7a1576351dcbdb
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz.asc' libseccomp_2.5.4.orig.tar.gz.asc 833 SHA256:af37e70eb422e6f983c1f135a3abb342c3b787716520b71bd774e4906003807f
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-1.debian.tar.xz' libseccomp_2.5.4-1.debian.tar.xz 16264 SHA256:fd7abe7b26a08ca514457fd13302d348d59401616ce3f6809ce15f54e6ebe77d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.5.4-1/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.5.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.5.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.4-1`

Binary Packages:

- `libselinux1:amd64=3.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.4-1
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4-1.dsc' libselinux_3.4-1.dsc 2534 SHA256:4035af53388d343f9b5c46ca2867ba32823cf4a2d218ddd590b34ae59c899157
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz' libselinux_3.4.orig.tar.gz 210061 SHA256:77c294a927e6795c2e98f74b5c3adde9c8839690e9255b767c5fca6acff9b779
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz.asc' libselinux_3.4.orig.tar.gz.asc 833 SHA256:5c370bdef7b756697445e6838ba1b2d934f668b244461e36e245f589ec994a24
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.4-1.debian.tar.xz' libselinux_3.4-1.debian.tar.xz 29416 SHA256:046ace4ad0092104bdfb0c6e5187131910216c89b8b81a4bce3c2067615c9196
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/3.4-1/ (for browsing the source)
- https://sources.debian.net/src/libselinux/3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=3.4-1`

Binary Packages:

- `libsemanage-common=3.4-1`
- `libsemanage2:amd64=3.4-1+b1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.4-1
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4-1.dsc' libsemanage_3.4-1.dsc 2570 SHA256:be300e01bbd08706fb6f0ecd349b3585a535d9ff0957265a7c634545ac3515c8
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz' libsemanage_3.4.orig.tar.gz 185177 SHA256:93b423a21600b8e3fb59bb925d4583d1258f45bebf63c29bde304dfd3d52efd6
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz.asc' libsemanage_3.4.orig.tar.gz.asc 833 SHA256:58da87dd662c135b70c065a0b1ca800cd4b075b365f3d71e0ff02d71c7457883
'http://deb.debian.org/debian/pool/main/libs/libsemanage/libsemanage_3.4-1.debian.tar.xz' libsemanage_3.4-1.debian.tar.xz 23248 SHA256:531c5294d5ec881ef4bc4396a9e1f38895558cd88c4fd6d3f6a673a4b2297a5c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsemanage/3.4-1/ (for browsing the source)
- https://sources.debian.net/src/libsemanage/3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsemanage/3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsepol=3.4-2`

Binary Packages:

- `libsepol2:amd64=3.4-2`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.4-2
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4-2.dsc' libsepol_3.4-2.dsc 2005 SHA256:c43db54870c37a4b6441b1980bfd41932e7851244ba1fda0df86c5f17dd67e8a
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz' libsepol_3.4.orig.tar.gz 490628 SHA256:fc277ac5b52d59d2cd81eec8b1cccd450301d8b54d9dd48a993aea0577cf0336
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz.asc' libsepol_3.4.orig.tar.gz.asc 833 SHA256:ed127c08353dbc2c442d47d77e323e79e5bd47791a0a5bd4dfd077868f4346bc
'http://deb.debian.org/debian/pool/main/libs/libsepol/libsepol_3.4-2.debian.tar.xz' libsepol_3.4-2.debian.tar.xz 21516 SHA256:fdf943b513b8d0fc6b74fd6a007ba35c9601909c0b3fd6e7726b4b09b1243502
```

Other potentially useful URLs:

- https://sources.debian.net/src/libsepol/3.4-2/ (for browsing the source)
- https://sources.debian.net/src/libsepol/3.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libsepol/3.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libtasn1-6=4.19.0-2`

Binary Packages:

- `libtasn1-6:amd64=4.19.0-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.19.0-2
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-2.dsc' libtasn1-6_4.19.0-2.dsc 2662 SHA256:cbecbd9b784af6dedde9ca685a4cc13e1ead027ea051150ff8186af57c547109
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz' libtasn1-6_4.19.0.orig.tar.gz 1786576 SHA256:1613f0ac1cf484d6ec0ce3b8c06d56263cc7242f1c23b30d82d23de345a63f7a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz.asc' libtasn1-6_4.19.0.orig.tar.gz.asc 228 SHA256:8410c0c004f3509c218a98b276b3308b9c46f48068e8b1a6d9ebfd61ea9f357a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-2.debian.tar.xz' libtasn1-6_4.19.0-2.debian.tar.xz 22012 SHA256:21fe6b16fb27cca47b51893708964ddfe04ea5227d1608560b4988e6fca74ae9
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.19.0-2/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.19.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.19.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=1.0-1`

Binary Packages:

- `libunistring2:amd64=1.0-1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libunistring/1.0-1/


### `dpkg` source package: `libxcrypt=1:4.4.28-2`

Binary Packages:

- `libcrypt1:amd64=1:4.4.28-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.28-2
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.28-2.dsc' libxcrypt_4.4.28-2.dsc 1613 SHA256:b668e66960c61b6980fbb6f2ea2cd7602e390f363e843798eca85f6cc6200a87
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.28.orig.tar.xz' libxcrypt_4.4.28.orig.tar.xz 391484 SHA256:2bf09c6c3ea139d11134d2598745a0793f4cf17245720880394c00490dbcb4df
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.28-2.debian.tar.xz' libxcrypt_4.4.28-2.debian.tar.xz 8088 SHA256:d5f8c1c1e2cb9ef9e99da9f3c7f28fc4142781337a72c22a67d841a8a8fee4d5
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.28-2/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.28-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.28-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.5.2+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.5.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.2+dfsg-1
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg-1.dsc' libzstd_1.5.2+dfsg-1.dsc 2173 SHA256:135c6d3ef18470e2eb4289b2aca6256eb9abba28478b08d99b0e1b8257af0b69
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg.orig.tar.xz' libzstd_1.5.2+dfsg.orig.tar.xz 1404564 SHA256:b59caaee4a6176bbe67bf5440b56ca8814da9d2ad2d943eb7b3ee8a0a83e4224
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg-1.debian.tar.xz' libzstd_1.5.2+dfsg-1.debian.tar.xz 11820 SHA256:286c2cc82fd3b0d76d172102efa8004325875bb0db1d12b5a52bbfc050f61a28
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.5.2+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.5.2+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.5.2+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lz4=1.9.4-1`

Binary Packages:

- `liblz4-1:amd64=1.9.4-1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.4-1
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.4-1.dsc' lz4_1.9.4-1.dsc 1951 SHA256:e16302bca544d08d106efc216541f4a0403c8f8a5fad5eaac7588223a55af263
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.4.orig.tar.gz' lz4_1.9.4.orig.tar.gz 354063 SHA256:0b0e3aa07c8c063ddf40b082bdf7e37a1562bda40a0ff5272957f3e987e0e54b
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.4-1.debian.tar.xz' lz4_1.9.4-1.debian.tar.xz 8128 SHA256:47ceec5b95f42598f7b9280b03df9659f2ee6852720ec181488e83bd643f0e5f
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.9.4-1/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.9.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.9.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mawk=1.3.4.20200120-3.1`

Binary Packages:

- `mawk=1.3.4.20200120-3.1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-3.1
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.dsc' mawk_1.3.4.20200120-3.1.dsc 1776 SHA256:ed0543e3111f718e918a73033292fe2616760c8791c13efa0da3818ca835cdc1
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.debian.tar.xz' mawk_1.3.4.20200120-3.1.debian.tar.xz 14080 SHA256:7850d7c44aa826635c79a6666b0d457a03524bcb0307697b062dd717d6d9d491
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.4.20200120-3.1/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.4.20200120-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.4.20200120-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.3+20220423-2`

Binary Packages:

- `libncursesw6:amd64=6.3+20220423-2`
- `libtinfo6:amd64=6.3+20220423-2`
- `ncurses-base=6.3+20220423-2`
- `ncurses-bin=6.3+20220423-2`

Licenses: (parsed from: `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.3+20220423-2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423-2.dsc' ncurses_6.3+20220423-2.dsc 4200 SHA256:bdd7ba478c9328689bd47231328efbf87ab970c4c26f5489b40abb4f4fdd79fa
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423.orig.tar.gz' ncurses_6.3+20220423.orig.tar.gz 3611993 SHA256:a6bdfe499ae98ee937fed4729de09ffea08201317a9d16ed5d0142ac8b8b30e1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423.orig.tar.gz.asc' ncurses_6.3+20220423.orig.tar.gz.asc 729 SHA256:6771460069f300048dd7c7a41027cd38250b4f28d5f1dcef9cf8edb9b5ca691c
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.3%2b20220423-2.debian.tar.xz' ncurses_6.3+20220423-2.debian.tar.xz 54600 SHA256:0a211bbd63949d81d6363a0fe2bf95f8592162f1dd34ded7252ec1d3340036c3
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.3+20220423-2/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.3+20220423-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.3+20220423-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.8.1-2`

Binary Packages:

- `libhogweed6:amd64=3.8.1-2`
- `libnettle8:amd64=3.8.1-2`

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
$ apt-get source -qq --print-uris nettle=3.8.1-2
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.8.1-2.dsc' nettle_3.8.1-2.dsc 2274 SHA256:a437e204da67612efb656cab354835f358b44c077c5c0a46d6e8c30b5c0bddff
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.8.1.orig.tar.gz' nettle_3.8.1.orig.tar.gz 2406251 SHA256:364f3e2b77cd7dcde83fd7c45219c834e54b0c75e428b6f894a23d12dd41cbfe
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.8.1.orig.tar.gz.asc' nettle_3.8.1.orig.tar.gz.asc 573 SHA256:71fe31c44728fdc144cbf12f30ca5d483992c17fd23afabe58f89d4201f66ddb
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.8.1-2.debian.tar.xz' nettle_3.8.1-2.debian.tar.xz 23396 SHA256:8f1eae9c6afffe545de294140f33d53352261478268dafee5ef72d840e1b3d7b
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.8.1-2/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.8.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.8.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `neurodebian=0.41.1`

Binary Packages:

- `neurodebian-freeze=0.41.1`

Licenses: (parsed from: `/usr/share/doc/neurodebian-freeze/copyright`)

- `BSD-2`
- `Expat`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris neurodebian=0.41.1
'http://deb.debian.org/debian/pool/main/n/neurodebian/neurodebian_0.41.1.dsc' neurodebian_0.41.1.dsc 2136 SHA256:64a1433f2586ff870969da2372763b529214ccdd8330590ef129c1e62dc24aef
'http://deb.debian.org/debian/pool/main/n/neurodebian/neurodebian_0.41.1.tar.xz' neurodebian_0.41.1.tar.xz 8318672 SHA256:6733a5d425a63b0e4de9ffa96af7b1dd2eeb72dba59b82a8a49eaa1c3e11b156
```

Other potentially useful URLs:

- https://sources.debian.net/src/neurodebian/0.41.1/ (for browsing the source)
- https://sources.debian.net/src/neurodebian/0.41.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/neurodebian/0.41.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `openldap=2.5.12+dfsg-2`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.12+dfsg-2+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openldap/2.5.12+dfsg-2/


### `dpkg` source package: `p11-kit=0.24.1-1`

Binary Packages:

- `libp11-kit0:amd64=0.24.1-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `LGPL-2.1`
- `LGPL-2.1+`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.24.1-1
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1-1.dsc' p11-kit_0.24.1-1.dsc 2501 SHA256:6d4336ed2799503c65dfb0518d623e3af46bac03e0e1a0ea9ce432044261d55b
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz' p11-kit_0.24.1.orig.tar.xz 838304 SHA256:d8be783efd5cd4ae534cee4132338e3f40f182c3205d23b200094ec85faaaef8
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz.asc' p11-kit_0.24.1.orig.tar.xz.asc 833 SHA256:48041a234bac05f70519b0d4727e78a129ea80a51baf92c7d419f80b7cbdf0ab
'http://deb.debian.org/debian/pool/main/p/p11-kit/p11-kit_0.24.1-1.debian.tar.xz' p11-kit_0.24.1-1.debian.tar.xz 23200 SHA256:769674df62c3caeada0e5885a992302cbde63a81a09972bf6b78f8797ebc40bd
```

Other potentially useful URLs:

- https://sources.debian.net/src/p11-kit/0.24.1-1/ (for browsing the source)
- https://sources.debian.net/src/p11-kit/0.24.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/p11-kit/0.24.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pam=1.5.2-2`

Binary Packages:

- `libpam-modules:amd64=1.5.2-2`
- `libpam-modules-bin=1.5.2-2`
- `libpam-runtime=1.5.2-2`
- `libpam0g:amd64=1.5.2-2`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.5.2-2
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-2.dsc' pam_1.5.2-2.dsc 2550 SHA256:dd6762b3a4a83697229680e277bacbe8f8d42a1d3f333bbb03d95f10038f9fdd
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA256:e4ec7131a91da44512574268f493c6d8ca105c87091691b8e9b56ca685d4f94d
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-2.debian.tar.xz' pam_1.5.2-2.debian.tar.xz 120232 SHA256:c8815f19bc93bbc111f1f7cf1ffa7b9ce4e72da02c9101229a740a8f245c6446
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.5.2-2/ (for browsing the source)
- https://sources.debian.net/src/pam/1.5.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.5.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.40-1`

Binary Packages:

- `libpcre2-8-0:amd64=10.40-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.40-1
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40-1.dsc' pcre2_10.40-1.dsc 2286 SHA256:0c880d9bc04175400921d8d6af2c24f1268a9c8678154b607d0df910d97bcbef
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40.orig.tar.gz' pcre2_10.40.orig.tar.gz 2359622 SHA256:ded42661cab30ada2e72ebff9e725e745b4b16ce831993635136f2ef86177724
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40-1.diff.gz' pcre2_10.40-1.diff.gz 7134 SHA256:6fe586fd149e20d18d42a60d2845b29ff5862511b851bfb80dd64d72359dc1c4
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.40-1/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.40-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.40-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.34.0-5`

Binary Packages:

- `perl-base=5.34.0-5`

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
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.34.0-5
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0-5.dsc' perl_5.34.0-5.dsc 2886 SHA256:fa744b5d2786d0dda1bfdb2960e0c2b66a734c4e268ec5de8e378366f680f021
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0.orig-regen-configure.tar.xz' perl_5.34.0.orig-regen-configure.tar.xz 415412 SHA256:b168f566401fdccc13d0616c258854c1e1a461276922babca617097cd9dfd85b
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0.orig.tar.xz' perl_5.34.0.orig.tar.xz 12881416 SHA256:82c2e5e5c71b0e10487a80d79140469ab1f8056349ca8545140a224dbbed7ded
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.34.0-5.debian.tar.xz' perl_5.34.0-5.debian.tar.xz 167484 SHA256:dbbb6c9c5218faef00bf5ee38b1c4e76bb02733742368984517b6e2449708f93
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.34.0-5/ (for browsing the source)
- https://sources.debian.net/src/perl/5.34.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.34.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.2.0-2`

Binary Packages:

- `pinentry-curses=1.2.0-2`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.2.0-2
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0-2.dsc' pinentry_1.2.0-2.dsc 2242 SHA256:43d974d725f0e261449ea1aa340b00e9e53c0e567f12db7da41942ecc07bd755
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0.orig.tar.bz2' pinentry_1.2.0.orig.tar.bz2 498390 SHA256:10072045a3e043d0581f91cd5676fcac7ffee957a16636adedaa4f583a616470
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0.orig.tar.bz2.asc' pinentry_1.2.0.orig.tar.bz2.asc 228 SHA256:d917a96c24e796daba7bab36bacc75d8106ef24d2afc485d13448d3cf8bd8a86
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.0-2.debian.tar.xz' pinentry_1.2.0-2.debian.tar.xz 19160 SHA256:628541197becd30a5da77a79b878d9e9df4954334792db7b4f740bc3109bdc4d
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.2.0-2/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.2.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.2.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.2~rc2-2`

Binary Packages:

- `libreadline8:amd64=8.2~rc2-2`
- `readline-common=8.2~rc2-2`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.2~rc2-2
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.2%7erc2-2.dsc' readline_8.2~rc2-2.dsc 2640 SHA256:2d1d06a769da84502049727fe154f239b0bd2388d87625a8c69e299f1cb79105
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.2%7erc2.orig.tar.gz' readline_8.2~rc2.orig.tar.gz 3041602 SHA256:4512174b322ba65e3e98dc7317b87784bf59176e6e23ec26176bd8f911b8abd4
'http://deb.debian.org/debian/pool/main/r/readline/readline_8.2%7erc2-2.debian.tar.xz' readline_8.2~rc2-2.debian.tar.xz 29112 SHA256:428fa408f552dad43265a536abf32bbc37280f4a1c733b99c17962ae0ef22d3a
```

Other potentially useful URLs:

- https://sources.debian.net/src/readline/8.2~rc2-2/ (for browsing the source)
- https://sources.debian.net/src/readline/8.2~rc2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/readline/8.2~rc2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.8-1`

Binary Packages:

- `sed=4.8-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.8-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8-1.dsc' sed_4.8-1.dsc 2213 SHA256:f3939fedfca116d7e0efdc2a4088432518a2ea52ffb3a52e14626729781dbf24
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8.orig.tar.xz' sed_4.8.orig.tar.xz 1348048 SHA256:f79b0cfea71b37a8eeec8490db6c5f7ae7719c35587f21edb0617f370eeff633
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8.orig.tar.xz.asc' sed_4.8.orig.tar.xz.asc 833 SHA256:dc256e914030bda14ce4135e655ffcc210e185a9f7de12ed0c4c9f352dc23e08
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.8-1.debian.tar.xz' sed_4.8-1.debian.tar.xz 60148 SHA256:a0c09e5dfa8de8544d464d118114dd53c617b11a369e562b6ba8c29899c6c47e
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.8-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.8-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.8-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shadow=1:4.11.1+dfsg1-2`

Binary Packages:

- `login=1:4.11.1+dfsg1-2`
- `passwd=1:4.11.1+dfsg1-2`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.11.1+dfsg1-2
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.11.1%2bdfsg1-2.dsc' shadow_4.11.1+dfsg1-2.dsc 2416 SHA256:55091e85ca7ff9f9a9d6673a18aee56bc9006ce254b8a9e16abc7b745de1cfda
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.11.1%2bdfsg1.orig.tar.xz' shadow_4.11.1+dfsg1.orig.tar.xz 1704716 SHA256:2605c11ff70d9d934147c74bc2d91771497460efbba29198d069e64ff9cd88ab
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.11.1%2bdfsg1-2.debian.tar.xz' shadow_4.11.1+dfsg1-2.debian.tar.xz 77852 SHA256:e0a1521bf22af1d88d6644fdd438f9afbe4a01b1ee0c468477d4938d80a28ecf
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.11.1+dfsg1-2/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.11.1+dfsg1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.11.1+dfsg1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sqlite3=3.39.3-1`

Binary Packages:

- `libsqlite3-0:amd64=3.39.3-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.39.3-1/


### `dpkg` source package: `systemd=251.4-3`

Binary Packages:

- `libsystemd0:amd64=251.4-3`
- `libudev1:amd64=251.4-3`

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
$ apt-get source -qq --print-uris systemd=251.4-3
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_251.4-3.dsc' systemd_251.4-3.dsc 6269 SHA256:0647413413dbf2a993ba4babc470d1b369dddf1aa79d4b6172c13c18a9497993
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_251.4.orig.tar.gz' systemd_251.4.orig.tar.gz 11440203 SHA256:3459239979f52b8c4ace33734d31c2fb69fa13cf81d04b1b982f7d8d4651e015
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_251.4-3.debian.tar.xz' systemd_251.4-3.debian.tar.xz 171732 SHA256:899e76d3c0cbbf5f17c85760e6d42f280b23572d2143cc3dbc136a8ef9530601
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/251.4-3/ (for browsing the source)
- https://sources.debian.net/src/systemd/251.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/251.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=3.05-2`

Binary Packages:

- `sysvinit-utils=3.05-2`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sysvinit/3.05-2/


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

### `dpkg` source package: `tzdata=2022c-1`

Binary Packages:

- `tzdata=2022c-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tzdata/2022c-1/


### `dpkg` source package: `usrmerge=29`

Binary Packages:

- `usr-is-merged=29`

Licenses: (parsed from: `/usr/share/doc/usr-is-merged/copyright`)

- `GPL v2`
- `GPL-2`
- `later (please see /usr/share/common-licenses/GPL-2)`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/usrmerge/29/


### `dpkg` source package: `util-linux=2.38.1-1`

Binary Packages:

- `bsdutils=1:2.38.1-1`
- `libblkid1:amd64=2.38.1-1`
- `libmount1:amd64=2.38.1-1`
- `libsmartcols1:amd64=2.38.1-1`
- `libuuid1:amd64=2.38.1-1`
- `mount=2.38.1-1`
- `util-linux=2.38.1-1`
- `util-linux-extra=2.38.1-1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/util-linux-extra/copyright`)

- `BSD-3-clause`
- `BSD-4-clause`
- `BSLA`
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
$ apt-get source -qq --print-uris util-linux=2.38.1-1
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1-1.dsc' util-linux_2.38.1-1.dsc 4520 SHA256:45d9335fa92e30b7b12a79c45e4d6303c1e5fe6ac83721f3fb88e5e6aabae557
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1.orig.tar.xz' util-linux_2.38.1.orig.tar.xz 7495904 SHA256:60492a19b44e6cf9a3ddff68325b333b8b52b6c59ce3ebd6a0ecaa4c5117e84f
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1-1.debian.tar.xz' util-linux_2.38.1-1.debian.tar.xz 95928 SHA256:c7a87ca093e565fbaed813b7e8b220f5e875437dd418ded2aefef6322f8aa0b8
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.38.1-1/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.38.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.38.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xxhash=0.8.1-1`

Binary Packages:

- `libxxhash0:amd64=0.8.1-1`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.1-1
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.1-1.dsc' xxhash_0.8.1-1.dsc 1966 SHA256:4a961627c06efc8fa3bc4b06ee9dba6cfaf092f2550b88d63e9218a2728721b4
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.1.orig.tar.gz' xxhash_0.8.1.orig.tar.gz 171552 SHA256:3bb6b7d6f30c591dd65aaaff1c8b7a5b94d81687998ca9400082c739a690436c
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.1-1.debian.tar.xz' xxhash_0.8.1-1.debian.tar.xz 4572 SHA256:d40aa223e90b85435082857b64573541ba9a995841717496e8975aed97241550
```

Other potentially useful URLs:

- https://sources.debian.net/src/xxhash/0.8.1-1/ (for browsing the source)
- https://sources.debian.net/src/xxhash/0.8.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xxhash/0.8.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.5-2.1`

Binary Packages:

- `liblzma5:amd64=5.2.5-2.1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2.1
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.dsc' xz-utils_5.2.5-2.1.dsc 2402 SHA256:338b5ec72d0d48a5fbb004926ebac8850eecd9626e38f6b50960ed975513b081
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA256:3e1e518ffc912f86608a8cb35e4bd41ad1aec210df2a47aaa1f95e7f5576ef56
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.debian.tar.xz' xz-utils_5.2.5-2.1.debian.tar.xz 34916 SHA256:24a1950b365b0922c3ef7f1475930bbcc64cdef04929f081b8ad5e2628ef2413
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.5-2.1/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.5-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.5-2.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.11.dfsg-4.1`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-4.1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-4.1
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-4.1.dsc' zlib_1.2.11.dfsg-4.1.dsc 2881 SHA256:aeb102797f718f2f9bcd090b233dcfaa6a43bd0d7e0148a2d880822406c89728
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.11.dfsg-4.1.debian.tar.xz' zlib_1.2.11.dfsg-4.1.debian.tar.xz 24052 SHA256:6136b2cc6483c27eec681f995864f1876c4765e69ad9c9c61d9cd62a86104e4d
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-4.1/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.11.dfsg-4.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.11.dfsg-4.1/ (for access to the source package after it no longer exists in the archive)
