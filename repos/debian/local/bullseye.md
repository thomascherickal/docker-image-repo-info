# `debian:bullseye`

## Docker Metadata

- Image ID: `sha256:0622e50112735fc1fdf59a03f4bcd9e86888120fdafd993757854876c667c3ba`
- Created: `2020-08-04T15:42:00.53637541Z`
- Virtual Size: ~ 117.78 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-8`

Binary Packages:

- `libacl1:amd64=2.2.53-8`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-8
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-8.dsc' acl_2.2.53-8.dsc 2464 SHA256:63623506d567cc90c9491aba7e40d480034a21f2d38b0c626f610ef637753a2c
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-8.debian.tar.xz' acl_2.2.53-8.debian.tar.xz 25300 SHA256:f8cfc2ce609f0fa19450cc4cb87aa98c48486231e80f04680b76072c05972e23
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.53-8/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.53-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.53-8/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `apt=2.1.7`

Binary Packages:

- `apt=2.1.7`
- `libapt-pkg6.0:amd64=2.1.7`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.1.7/


### `dpkg` source package: `attr=1:2.4.48-5`

Binary Packages:

- `libattr1:amd64=1:2.4.48-5`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.48-5
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-5.dsc' attr_2.4.48-5.dsc 2433 SHA256:0b20a285b758083e2e202ffdd2930cef1bf84fee498791fc3e26b69a3bced01d
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.4.48-5.debian.tar.xz' attr_2.4.48-5.debian.tar.xz 25560 SHA256:02238253d324250dabdc0434f7de045d85df93458995a465ac434f2a3978a312
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.4.48-5/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.4.48-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.4.48-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:2.8.5-3`

Binary Packages:

- `libaudit-common=1:2.8.5-3`
- `libaudit1:amd64=1:2.8.5-3+b1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.5-3
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.5-3.dsc' audit_2.8.5-3.dsc 2401 SHA256:24f6c0b71797265bd163f53237d8ec359761d92f3840b3315d4dcebf6505121e
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.5.orig.tar.gz' audit_2.8.5.orig.tar.gz 1140694 SHA256:0e5d4103646e00f8d1981e1cd2faea7a2ae28e854c31a803e907a383c5e2ecb7
'http://deb.debian.org/debian/pool/main/a/audit/audit_2.8.5-3.debian.tar.xz' audit_2.8.5-3.debian.tar.xz 17164 SHA256:425eca791602be6865c1198a70ed7bf3775a1a4ef0851645826c09cc9d6df314
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:2.8.5-3/ (for browsing the source)
- https://sources.debian.net/src/audit/1:2.8.5-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:2.8.5-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=11`

Binary Packages:

- `base-files=11`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_11.dsc' base-files_11.dsc 1063 SHA256:8c3da5c6c17db756e8369ccdef4c706ed3e71d5480ca50fec3fe451073e3d94d
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_11.tar.xz' base-files_11.tar.xz 65368 SHA256:cf610763b6fc4e7f6c066fd6bed1d580f6b0fd9e1f91c26a18900117a3d5622e
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/11/ (for browsing the source)
- https://sources.debian.net/src/base-files/11/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/11/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.5.47`

Binary Packages:

- `base-passwd=3.5.47`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.47
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.47.dsc' base-passwd_3.5.47.dsc 1757 SHA256:5a77a4cce51d1eb72e9d96d4083c641435c05888922c7bd3fa6b4395bf9afad3
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.47.tar.xz' base-passwd_3.5.47.tar.xz 53024 SHA256:9810ae0216e96bf9fc7ca6163d47ef8ec7d1677f533451af5911d8202a490a23
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.47/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.47/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.47/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.0-6`

Binary Packages:

- `bash=5.0-6`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/bash/5.0-6/


### `dpkg` source package: `bzip2=1.0.8-4`

Binary Packages:

- `libbz2-1.0:amd64=1.0.8-4`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

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

### `dpkg` source package: `cdebconf=0.253`

Binary Packages:

- `libdebconfclient0:amd64=0.253`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.253
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.253.dsc' cdebconf_0.253.dsc 2750 SHA256:c66fc6fa7bc175f211b597e31326fa20fd5780a936193d40c6777e7bb88b93da
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.253.tar.xz' cdebconf_0.253.tar.xz 275576 SHA256:a9546e1078b7260dc2154750b1354d1b14a02375445642a4e4e083451d0580a7
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.253/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.253/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.253/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=8.30-3`

Binary Packages:

- `coreutils=8.30-3+b1`

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

### `dpkg` source package: `dash=0.5.10.2-7`

Binary Packages:

- `dash=0.5.10.2-7`

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
$ apt-get source -qq --print-uris dash=0.5.10.2-7
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2-7.dsc' dash_0.5.10.2-7.dsc 1762 SHA256:477515a7d980127657c9760f1a53b0175b79455acfd9d92284a6c563971523ea
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA256:3c663919dc5c66ec991da14c7cf7e0be8ad00f3db73986a987c118862b5f6071
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.10.2-7.debian.tar.xz' dash_0.5.10.2-7.debian.tar.xz 45336 SHA256:ba76b70008e95a88f1f2860bc74bea9fd6732df179dbb126706d51cfede713c1
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.10.2-7/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.10.2-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.10.2-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6.dsc' db5.3_5.3.28+dfsg1-0.6.dsc 3138 SHA256:0cd8010ff17180156bc2d91518ca15c4e32bdee7638a1289cdc5c0a803f50279
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6.debian.tar.xz 29196 SHA256:8e7264cfd368d04133a818cdbd3191b874c534f4ad7f83cfdbb3cccf12b5f052
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.6/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.74`

Binary Packages:

- `debconf=1.5.74`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.74
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.74.dsc' debconf_1.5.74.dsc 2082 SHA256:7576b8798165e30aaea23bad812eec729dd091a1ca59063328e7f68223b79af1
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.74.tar.xz' debconf_1.5.74.tar.xz 571108 SHA256:11b3fa02ddafe813c301aa150fef4d510d77afa64cbfe09c7e614995147c48e0
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.74/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.74/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.74/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `debianutils=4.9.1`

Binary Packages:

- `debianutils=4.9.1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.9.1
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.9.1.dsc' debianutils_4.9.1.dsc 1592 SHA256:d30866ea0352263fa7756010e8743ade350024b2fd491bc5befcbaa9a97626b7
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_4.9.1.tar.xz' debianutils_4.9.1.tar.xz 157516 SHA256:af826685d9c56abfa873e84cd392539cd363cb0ba04a09d21187377e1b764091
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/4.9.1/ (for browsing the source)
- https://sources.debian.net/src/debianutils/4.9.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/4.9.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `dpkg=1.20.5`

Binary Packages:

- `dpkg=1.20.5`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.20.5
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.20.5.dsc' dpkg_1.20.5.dsc 2109 SHA256:6c69b24038227fc1715e7a7ddf1f0a0b62f6ec8aeaab4992ddc4215ede341d3a
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.20.5.tar.xz' dpkg_1.20.5.tar.xz 4715684 SHA256:f2f23f3197957d89e54b87cf8fc42ab00e1b74f3a32090efe9acd08443f3e0dd
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.20.5/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.20.5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.20.5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.45.6-1`

Binary Packages:

- `e2fsprogs=1.45.6-1`
- `libcom-err2:amd64=1.45.6-1`
- `libext2fs2:amd64=1.45.6-1`
- `libss2:amd64=1.45.6-1`
- `logsave=1.45.6-1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.6-1
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1.dsc' e2fsprogs_1.45.6-1.dsc 2955 SHA256:22fe3cb0e2a32fba560d2da31866e82efefc3d08daf9497423cac617608c3d0d
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz' e2fsprogs_1.45.6.orig.tar.gz 7938544 SHA256:5f64ac50a2b60b8e67c5b382bb137dec39344017103caffc3a61554424f2d693
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz.asc' e2fsprogs_1.45.6.orig.tar.gz.asc 488 SHA256:831c29bd04c5b21faf2aa2d5fa3b409148973e3ef0d15f67315a5c429180d945
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1.debian.tar.xz' e2fsprogs_1.45.6-1.debian.tar.xz 80452 SHA256:839b31654b2d72706c61ec49a47a8e33b7df41c6c7a427977bcc5afa9a6ffc3e
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.45.6-1/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.45.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.45.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `elfutils=0.180-1`

Binary Packages:

- `libelf1:amd64=0.180-1+b1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.180-1
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.180-1.dsc' elfutils_0.180-1.dsc 2810 SHA256:21325074457d6d02da421a81a00c676da4bced72c5f3abaae77c05a636b517e9
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.180.orig.tar.bz2' elfutils_0.180.orig.tar.bz2 9079640 SHA256:b827b6e35c59d188ba97d7cf148fa8dc6f5c68eb6c5981888dfdbb758c0b569d
'http://deb.debian.org/debian/pool/main/e/elfutils/elfutils_0.180-1.debian.tar.xz' elfutils_0.180-1.debian.tar.xz 33016 SHA256:2049e6fff637816cf7bbf93a9d2e67514f71758c354c61c8b032e9bc13119d0b
```

Other potentially useful URLs:

- https://sources.debian.net/src/elfutils/0.180-1/ (for browsing the source)
- https://sources.debian.net/src/elfutils/0.180-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/elfutils/0.180-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.7.0-1`

Binary Packages:

- `findutils=4.7.0-1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.7.0-1
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0-1.dsc' findutils_4.7.0-1.dsc 2302 SHA256:867867005890a464599024bbc9d3bbc82493e255ca812a906112b9a5eda15169
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz' findutils_4.7.0.orig.tar.xz 1895048 SHA256:c5fefbdf9858f7e4feb86f036e1247a54c79fc2d8e4b7064d5aaa1f47dfa789a
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz.asc' findutils_4.7.0.orig.tar.xz.asc 488 SHA256:2f620e6d941e241fac52344a89149ab1ffeefb0fb9e42174e17a508d59a31d0f
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0-1.debian.tar.xz' findutils_4.7.0-1.debian.tar.xz 27536 SHA256:3503f8ff7b1020c140055fbe06f107c73cd827f50761cf9a3c5296f6890bf0af
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.7.0-1/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.7.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.7.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-10=10.1.0-6`

Binary Packages:

- `gcc-10-base:amd64=10.1.0-6`
- `libgcc-s1:amd64=10.1.0-6`
- `libstdc++6:amd64=10.1.0-6`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.1.0-6
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.1.0-6.dsc' gcc-10_10.1.0-6.dsc 27608 SHA256:ad0d0e98f78c408e6430bcefc2763cf9a9f39f2a9fb9540172befcc441288f50
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.1.0.orig.tar.gz' gcc-10_10.1.0.orig.tar.gz 92670668 SHA256:cdf22173652ee0a51f4789a8c64aa2c7aeeaf67eddeb49d0221c0da368bc9432
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.1.0-6.debian.tar.xz' gcc-10_10.1.0-6.debian.tar.xz 2490624 SHA256:dd898392d33537be532eecf64537753a0659d167a87991d5407a193d90a69d59
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-10/10.1.0-6/ (for browsing the source)
- https://sources.debian.net/src/gcc-10/10.1.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-10/10.1.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-9=9.3.0-15`

Binary Packages:

- `gcc-9-base:amd64=9.3.0-15`

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
$ apt-get source -qq --print-uris gcc-9=9.3.0-15
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0-15.dsc' gcc-9_9.3.0-15.dsc 21922 SHA256:83dd853938bcb9d131210c8f8eddcb4c9c9a3a0704b063da17cd099b32d88d30
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0.orig.tar.gz' gcc-9_9.3.0.orig.tar.gz 88686943 SHA256:824044ffa96eb337bb1c1d4cf6a82691d0290d6f42e1d13362eea855458de060
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0-15.debian.tar.xz' gcc-9_9.3.0-15.debian.tar.xz 735456 SHA256:6561b0b5c3578b7ef031e7c2b4af8178f479f2122df99e20540ea192871ba7ca
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-9/9.3.0-15/ (for browsing the source)
- https://sources.debian.net/src/gcc-9/9.3.0-15/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-9/9.3.0-15/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.31-2`

Binary Packages:

- `libc-bin=2.31-2`
- `libc6:amd64=2.31-2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.31-2
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31-2.dsc' glibc_2.31-2.dsc 8195 SHA256:1e68e21c7c03f539fe4f7b6cd6b04edc124dcbdd4c64a742a0e8defc6c446e03
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31.orig.tar.xz' glibc_2.31.orig.tar.xz 17254692 SHA256:3dc7704b6166839c37d7047626fd199f3d4c09aca0d90e48c51c31c967dce34e
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31-2.debian.tar.xz' glibc_2.31-2.debian.tar.xz 832956 SHA256:2f09126faa95ae00641c8848a4602cf108849d980ce88d9d129adab596ea835d
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.31-2/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.31-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.31-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.0+dfsg-6`

Binary Packages:

- `libgmp10:amd64=2:6.2.0+dfsg-6`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.0+dfsg-6
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.0+dfsg-6.dsc' gmp_6.2.0+dfsg-6.dsc 2144 SHA256:8ca73e96ab6d3d05d21a76b357fdc36959be9c5c863186fd30ee17981c4f2c93
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.0+dfsg.orig.tar.xz' gmp_6.2.0+dfsg.orig.tar.xz 1842912 SHA256:5d7610449498a79aa62d4b9a8f6baaef91b8716726e1009e02b879962dff32ab
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.0+dfsg-6.debian.tar.xz' gmp_6.2.0+dfsg-6.debian.tar.xz 21220 SHA256:bb447179d6bd323e2a37035a8ebab58722f1e5c74abb1043b8b9ad038ce4f9fe
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.0+dfsg-6/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.0+dfsg-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.0+dfsg-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.20-1`

Binary Packages:

- `gpgv=2.2.20-1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.20-1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.20-1.dsc' gnupg2_2.2.20-1.dsc 3241 SHA256:3b6735d9566e0963b47d37df4a58c675510a2f3f5aaa28ce23c4e88e2a370b73
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2' gnupg2_2.2.20.orig.tar.bz2 6786913 SHA256:04a7c9d48b74c399168ee8270e548588ddbe52218c337703d7f06373d326ca30
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2.asc' gnupg2_2.2.20.orig.tar.bz2.asc 1357 SHA256:be34b9959fa4c9baa7269b1c7c695808d6b999ba47f28c614312dd3d8d47ca79
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.20-1.debian.tar.xz' gnupg2_2.2.20-1.debian.tar.xz 61912 SHA256:462e7ed52973485c0687ac122f766a96ce6ea83c03af21e534b535532fda25cd
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.20-1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.20-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.20-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.6.14-2`

Binary Packages:

- `libgnutls30:amd64=3.6.14-2+b1`

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
$ apt-get source -qq --print-uris gnutls28=3.6.14-2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.14-2.dsc' gnutls28_3.6.14-2.dsc 3479 SHA256:c45f3443e574c1ba34b65e3c1165adb9a0a911af57cb1e333f976d8206841b4d
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.14.orig.tar.xz' gnutls28_3.6.14.orig.tar.xz 6069088 SHA256:5630751adec7025b8ef955af4d141d00d252a985769f51b4059e5affa3d39d63
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.14.orig.tar.xz.asc' gnutls28_3.6.14.orig.tar.xz.asc 854 SHA256:a3e05b531b68a4aca8fdc5dce83e7091b5aa859d76de7e8ba9992047272f04dd
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.6.14-2.debian.tar.xz' gnutls28_3.6.14-2.debian.tar.xz 65404 SHA256:dc8574598e599fb83fba2b3163c03d7e9976ddc7e2609c3916f28f09f118d9d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.6.14-2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.6.14-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.6.14-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.4-1`

Binary Packages:

- `grep=3.4-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.4-1
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4-1.dsc' grep_3.4-1.dsc 1674 SHA256:785f527cede9631f075bdd6c7f35e65e6b82897d009682766cf35839a393277d
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4.orig.tar.xz' grep_3.4.orig.tar.xz 1555820 SHA256:58e6751c41a7c25bfc6e9363a41786cff3ba5709cf11d5ad903cf7cce31cc3fb
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4.orig.tar.xz.asc' grep_3.4.orig.tar.xz.asc 833 SHA256:4c1871ff6b79c5e5ce0a192272c171d06ec20762b4b258688b1ca2e47d94b23e
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.4-1.debian.tar.xz' grep_3.4-1.debian.tar.xz 104364 SHA256:582d181804ce72fcfc4c6a9f13ea1dd73ad04c2723b5da346b69ee5cd24a7d08
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.4-1/ (for browsing the source)
- https://sources.debian.net/src/grep/3.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gzip=1.10-2`

Binary Packages:

- `gzip=1.10-2`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-2
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.10-2.dsc' gzip_1.10-2.dsc 2199 SHA256:b51c898723bfbea9abc217578fd739841d92711e8e96e8392d69151a9147475e
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA256:c91f74430bf7bc20402e1f657d0b252cb80aa66ba333a25704512af346633c68
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.10.orig.tar.gz.asc' gzip_1.10.orig.tar.gz.asc 833 SHA256:b5e4942cca901ca37772d3ea060c4af6a1908719cec5327fbe033f9d30933f1b
'http://deb.debian.org/debian/pool/main/g/gzip/gzip_1.10-2.debian.tar.xz' gzip_1.10-2.debian.tar.xz 18560 SHA256:283cb0b05bce5f554f3b663ae5fe1f31e7933140adffc5fdf4193ac466e37469
```

Other potentially useful URLs:

- https://sources.debian.net/src/gzip/1.10-2/ (for browsing the source)
- https://sources.debian.net/src/gzip/1.10-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gzip/1.10-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `init-system-helpers=1.58`

Binary Packages:

- `init-system-helpers=1.58`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.58
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.58.dsc' init-system-helpers_1.58.dsc 1896 SHA256:d754ec5e07416c63ead4c8c029d24027c563ff5f83762f2ac5246f716d405784
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.58.tar.xz' init-system-helpers_1.58.tar.xz 40668 SHA256:99f82ffca33b121f7aa31a06b6227f4684d986ff342a27b07433711de883609d
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.58/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.58/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.58/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iproute2=5.7.0-1`

Binary Packages:

- `iproute2=5.7.0-1`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/iproute2/5.7.0-1/


### `dpkg` source package: `iptables=1.8.5-2`

Binary Packages:

- `libxtables12:amd64=1.8.5-2`

Licenses: (parsed from: `/usr/share/doc/libxtables12/copyright`)

- `Artistic`
- `GPL-2`
- `GPL-2+`
- `custom`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/iptables/1.8.5-2/


### `dpkg` source package: `iputils=3:20190709-3`

Binary Packages:

- `iputils-ping=3:20190709-3`

Licenses: (parsed from: `/usr/share/doc/iputils-ping/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/iputils/3:20190709-3/


### `dpkg` source package: `libbsd=0.10.0-1`

Binary Packages:

- `libbsd0:amd64=0.10.0-1`

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
$ apt-get source -qq --print-uris libbsd=0.10.0-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0-1.dsc' libbsd_0.10.0-1.dsc 2197 SHA256:7c05e2c73658f64cbd4e1762b716cc7c4c1d68391191e82c7d266a351430edd6
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz' libbsd_0.10.0.orig.tar.xz 393576 SHA256:34b8adc726883d0e85b3118fa13605e179a62b31ba51f676136ecb2d0bc1a887
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz.asc' libbsd_0.10.0.orig.tar.xz.asc 833 SHA256:4362f6d811ffc06659ac5cf777d8d01157bedfc28720b41fb485afb0a5acc0c7
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.10.0-1.debian.tar.xz' libbsd_0.10.0-1.debian.tar.xz 16660 SHA256:4cf37d6d5b72702b31b07384612e07173e94e081feef71fec206f86ab38f2411
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.10.0-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.10.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.10.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.7.9-2.2`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.2`

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

### `dpkg` source package: `libcap2=1:2.36-1`

Binary Packages:

- `libcap2:amd64=1:2.36-1`
- `libcap2-bin=1:2.36-1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.36-1
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.36-1.dsc' libcap2_2.36-1.dsc 2179 SHA256:c47d8683fb567d8a57c259073ace2e482e8740e91ed082ea27e04b98410ca450
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.36.orig.tar.xz' libcap2_2.36.orig.tar.xz 112612 SHA256:5048c849bdbbe24d2ca59463142cb279abec5edf3ab6731ab35a596bcf538a49
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.36-1.debian.tar.xz' libcap2_2.36-1.debian.tar.xz 22268 SHA256:efdde4cf107e6ed0e511f33fac4e22542145ff999fef2a12e7a7a8fde4c3effd
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.36-1/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.36-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.36-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.3-4`

Binary Packages:

- `libffi7:amd64=3.3-4`

Licenses: (parsed from: `/usr/share/doc/libffi7/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.3-4
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-4.dsc' libffi_3.3-4.dsc 1932 SHA256:4190ad8e7ae9167a0c67c5926bc3705acb191745cca93ef845dbc06fc097f380
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3.orig.tar.gz' libffi_3.3.orig.tar.gz 1305466 SHA256:72fba7922703ddfa7a028d513ac15a85c8d54c8d67f55fa5a4802885dc652056
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-4.debian.tar.xz' libffi_3.3-4.debian.tar.xz 9016 SHA256:0e8a6d9d87202d04d7646178479c3d365a845f9723da26625d533a169b378100
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.3-4/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.8.6-2`

Binary Packages:

- `libgcrypt20:amd64=1.8.6-2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.6-2
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.6-2.dsc' libgcrypt20_1.8.6-2.dsc 2800 SHA256:740b315567c33846fc69f6663da32cdb00773c463bf9723b1884990642d4c493
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.6.orig.tar.bz2' libgcrypt20_1.8.6.orig.tar.bz2 2997781 SHA256:0cba2700617b99fc33864a0c16b1fa7fdf9781d9ed3509f5d767178e5fd7b975
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.6.orig.tar.bz2.asc' libgcrypt20_1.8.6.orig.tar.bz2.asc 488 SHA256:cd78d977dfa7e485562d802f7624b552be429750f32c066403536c6f05e53cff
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.6-2.debian.tar.xz' libgcrypt20_1.8.6-2.debian.tar.xz 29496 SHA256:effb1e3b70ef3c9805fdc8b445bbcda4b85f4945966a80f4cae32893bc4b4a93
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.8.6-2/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.8.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.8.6-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libidn2=2.3.0-1`

Binary Packages:

- `libidn2-0:amd64=2.3.0-1`

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
$ apt-get source -qq --print-uris libidn2=2.3.0-1
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0-1.dsc' libidn2_2.3.0-1.dsc 2411 SHA256:f4f61425610ae4b4c4d3c74431825fb4b4892d4d07e954d7acdf163595d33f14
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0.orig.tar.gz' libidn2_2.3.0.orig.tar.gz 2164993 SHA256:e1cb1db3d2e249a6a3eb6f0946777c2e892d5c5dc7bd91c74394fc3a01cab8b5
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0-1.debian.tar.xz' libidn2_2.3.0-1.debian.tar.xz 10588 SHA256:a515029f13d12a48a6bc07dadc4cef6592db0a7257f48633795ae7128c23116c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.3.0-1/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.3.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.3.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libmnl=1.0.4-3`

Binary Packages:

- `libmnl0:amd64=1.0.4-3`

Licenses: (parsed from: `/usr/share/doc/libmnl0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libmnl=1.0.4-3
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4-3.dsc' libmnl_1.0.4-3.dsc 2071 SHA256:9dc308ffade8cc0cb7a7ee8925e25f338121f642a9a9caef535effd893d4830a
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4.orig.tar.bz2' libmnl_1.0.4.orig.tar.bz2 301270 SHA256:171f89699f286a5854b72b91d06e8f8e3683064c5901fb09d954a9ab6f551f81
'http://deb.debian.org/debian/pool/main/libm/libmnl/libmnl_1.0.4-3.debian.tar.xz' libmnl_1.0.4-3.debian.tar.xz 7780 SHA256:7f5a5c246ee6d6d65efd01db289886c0ea986546f112e70c3006b50d0e6fabc1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmnl/1.0.4-3/ (for browsing the source)
- https://sources.debian.net/src/libmnl/1.0.4-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmnl/1.0.4-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.4.3-1`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1+b1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.4.3-1.dsc' libseccomp_2.4.3-1.dsc 2416 SHA256:753a11c3aaed55ee2f96cc428582bee5f9e67684d3928337f44db066bf345f5b
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA256:cf15d1421997fac45b936515af61d209c4fd788af11005d212b3d0fd71e7991d
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.4.3-1.debian.tar.xz' libseccomp_2.4.3-1.debian.tar.xz 13400 SHA256:dadccb6c01ddaebad2f694527db8bda948ccd4c9dab9a895adc211ac3a57c49b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.4.3-1/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.4.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.4.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.1-2`

Binary Packages:

- `libselinux1:amd64=3.1-2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.1-2
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.1-2.dsc' libselinux_3.1-2.dsc 2310 SHA256:9d9a31ac3e11dcaa1bbdaa28c3bdc7dc44a94b0b3d6b380e5c5e69f6f57c5901
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.1.orig.tar.gz' libselinux_3.1.orig.tar.gz 204703 SHA256:ea5dcbb4d859e3f999c26a13c630da2f16dff9462e3cc8cb7b458ac157d112e7
'http://deb.debian.org/debian/pool/main/libs/libselinux/libselinux_3.1-2.debian.tar.xz' libselinux_3.1-2.debian.tar.xz 23788 SHA256:336c6df026daf947f37c74d3e3efdfc6b235491d402096f050ce2c9d8bbad415
```

Other potentially useful URLs:

- https://sources.debian.net/src/libselinux/3.1-2/ (for browsing the source)
- https://sources.debian.net/src/libselinux/3.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libselinux/3.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libsemanage=3.1-1`

Binary Packages:

- `libsemanage-common=3.1-1`
- `libsemanage1:amd64=3.1-1`

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

### `dpkg` source package: `libxcrypt=1:4.4.16-1`

Binary Packages:

- `libcrypt1:amd64=1:4.4.16-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxcrypt/1:4.4.16-1/


### `dpkg` source package: `libzstd=1.4.5+dfsg-3`

Binary Packages:

- `libzstd1:amd64=1.4.5+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libzstd/1.4.5+dfsg-3/


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

### `dpkg` source package: `lz4=1.9.2-2`

Binary Packages:

- `liblz4-1:amd64=1.9.2-2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.2-2
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.2-2.dsc' lz4_1.9.2-2.dsc 1956 SHA256:103fa80edbf501cf6e6d9ee0ed3d75d6111cd06026b00aaccaa11fe5555b71a6
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.2.orig.tar.gz' lz4_1.9.2.orig.tar.gz 305796 SHA256:658ba6191fa44c92280d4aa2c271b0f4fbc0e34d249578dd05e50e76d0e5efcc
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.2-2.debian.tar.xz' lz4_1.9.2-2.debian.tar.xz 12712 SHA256:8970a0afc2f1633bbc8b7f55fa36ba711fb4d0c1811e591ad8f52d1d1968592c
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.9.2-2/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.9.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.9.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ncurses=6.2-1`

Binary Packages:

- `libtinfo6:amd64=6.2-1`
- `ncurses-base=6.2-1`
- `ncurses-bin=6.2-1`

Licenses: (parsed from: `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2-1.dsc' ncurses_6.2-1.dsc 4016 SHA256:fc81f03ae9d74b98a6ff6fe5e9a8339bbd71f19aa21f2b041ce5fbecc71cb472
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz' ncurses_6.2.orig.tar.gz 3425862 SHA256:30306e0c76e0f9f1f0de987cf1c82a5c21e1ce6568b9227f7da5b71cbea86c9d
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz.asc' ncurses_6.2.orig.tar.gz.asc 265 SHA256:8733e48fa7dafa61f3df67783402c3b2555fccccff44e912b436a7111b9c8781
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2-1.debian.tar.xz' ncurses_6.2-1.debian.tar.xz 51276 SHA256:b5c4958529954ec70226cf73d5a848e2d159a2c2115faf57258009e28b2e110d
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.2-1/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `nettle=3.6-2`

Binary Packages:

- `libhogweed6:amd64=3.6-2`
- `libnettle8:amd64=3.6-2`

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
$ apt-get source -qq --print-uris nettle=3.6-2
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.6-2.dsc' nettle_3.6-2.dsc 2254 SHA256:3d7c14776e74d14103f49455b1ae3c373bbb374af6f215071deecd436495b43a
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.6.orig.tar.gz' nettle_3.6.orig.tar.gz 2288173 SHA256:d24c0d0f2abffbc8f4f34dcf114b0f131ec3774895f3555922fe2f40f3d5e3f1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.6.orig.tar.gz.asc' nettle_3.6.orig.tar.gz.asc 573 SHA256:f0ee81d3120bb85ce2adee753568f68361d33b3fe363b6a15462b06bb9518ad1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.6-2.debian.tar.xz' nettle_3.6-2.debian.tar.xz 21136 SHA256:55c5e4471fbb92378c198a765135a7dcb327b84344a3ef2fa95340af1053313f
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.6-2/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.6-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `p11-kit=0.23.20-1`

Binary Packages:

- `libp11-kit0:amd64=0.23.20-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/p11-kit/0.23.20-1/


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

### `dpkg` source package: `pcre2=10.34-7`

Binary Packages:

- `libpcre2-8-0:amd64=10.34-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.34-7
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.34-7.dsc' pcre2_10.34-7.dsc 2286 SHA256:c3e2bfd8fabf594238b3f17074dc8ac483aaf80a9f12dbfe927b80a74558732e
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.34.orig.tar.gz' pcre2_10.34.orig.tar.gz 2271533 SHA256:da6aba7ba2509e918e41f4f744a59fa41a2425c59a298a232e7fe85691e00379
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.34-7.diff.gz' pcre2_10.34-7.diff.gz 7068 SHA256:7d44ac1b171ef7f7051213a3a8505b28f3809ed3e2fb348567a29fdf5f2b5fdf
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.34-7/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.34-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.34-7/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `perl=5.30.3-4`

Binary Packages:

- `perl-base=5.30.3-4`

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
$ apt-get source -qq --print-uris perl=5.30.3-4
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.3-4.dsc' perl_5.30.3-4.dsc 2983 SHA256:05c8d356f72848b6e26b57949b5fb7dcc6340719df292f83d02ff05fb84cdd98
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.3.orig-regen-configure.tar.gz' perl_5.30.3.orig-regen-configure.tar.gz 870970 SHA256:99174174fbfc550f801076ab8a1a5831c92f75c1b81e553150351f14a111dcf8
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.3.orig.tar.xz' perl_5.30.3.orig.tar.xz 12375128 SHA256:6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.30.3-4.debian.tar.xz' perl_5.30.3-4.debian.tar.xz 171184 SHA256:a71ed73cab42cadb8cb9efe430ac075e644fea527f3689b64e4e0fe8b9648ffd
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.30.3-4/ (for browsing the source)
- https://sources.debian.net/src/perl/5.30.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.30.3-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `systemd=245.7-1`

Binary Packages:

- `libsystemd0:amd64=245.7-1`
- `libudev1:amd64=245.7-1`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2 with Linux-syscall-note exception`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/systemd/245.7-1/


### `dpkg` source package: `sysvinit=2.96-3`

Binary Packages:

- `sysvinit-utils=2.96-3`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sysvinit/2.96-3/


### `dpkg` source package: `tar=1.30+dfsg-7`

Binary Packages:

- `tar=1.30+dfsg-7`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.30+dfsg-7
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg-7.dsc' tar_1.30+dfsg-7.dsc 1981 SHA256:5117afe47b5aab94c592d52c11c74dba146a11a7cdc22dbe067a4b5a5e895729
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA256:c02f3747ffe02017878303dde8b78e79cd220364c5e8048cf92320232e38912d
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.30+dfsg-7.debian.tar.xz' tar_1.30+dfsg-7.debian.tar.xz 22168 SHA256:12763df7f214458a56edc4a4b27adb2cb2041d597d74212ba34736f02bb68cd3
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.30+dfsg-7/ (for browsing the source)
- https://sources.debian.net/src/tar/1.30+dfsg-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.30+dfsg-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2020a-1`

Binary Packages:

- `tzdata=2020a-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2020a-1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a-1.dsc' tzdata_2020a-1.dsc 2237 SHA256:c1a0bba8797ca5eb91dcda49bcb08a3102020dd1a8557f4d7f74a8343e563975
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz' tzdata_2020a.orig.tar.gz 397245 SHA256:547161eca24d344e0b5f96aff6a76b454da295dc14ed4ca50c2355043fb899a2
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz.asc' tzdata_2020a.orig.tar.gz.asc 833 SHA256:a92f085fe1e7f8bc0f0a0bc4432f27e6cf2d69e64d4a90958bd023eb0ccf45f9
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020a-1.debian.tar.xz' tzdata_2020a-1.debian.tar.xz 105224 SHA256:d84a9a0d0581a2331b7a26f35b1dfc646f9f6bb3dc36f18327151d322206c549
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2020a-1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2020a-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2020a-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.36-1`

Binary Packages:

- `bsdutils=1:2.36-1`
- `libblkid1:amd64=2.36-1`
- `libmount1:amd64=2.36-1`
- `libsmartcols1:amd64=2.36-1`
- `libuuid1:amd64=2.36-1`
- `mount=2.36-1`
- `util-linux=2.36-1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/util-linux/2.36-1/


### `dpkg` source package: `xz-utils=5.2.4-1`

Binary Packages:

- `liblzma5:amd64=5.2.4-1+b1`

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
