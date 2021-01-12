# `debian:bullseye`

## Docker Metadata

- Image ID: `sha256:e3a3b08b9d312e134f5ee90402de401ef0cf0bc2f40e49383352760a4813158b`
- Created: `2021-01-12T00:32:09.567621773Z`
- Virtual Size: ~ 121.24 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-9`

Binary Packages:

- `libacl1:amd64=2.2.53-9`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-9
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-9.dsc' acl_2.2.53-9.dsc 2464 SHA256:c606d828d13e3876cb7d30347b4e281d0f9e7d5fde78e2bb8cd9fd0dd3bf27e9
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.2.53-9.debian.tar.xz' acl_2.2.53-9.debian.tar.xz 25504 SHA256:f0cd5bdb0eaa8c5a7609b02ff76da53588a33247df9c44d9b0905ac79009e8e0
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.2.53-9/ (for browsing the source)
- https://sources.debian.net/src/acl/2.2.53-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.2.53-9/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `apt=2.1.15`

Binary Packages:

- `apt=2.1.15`
- `libapt-pkg6.0:amd64=2.1.15`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.1.15/


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

### `dpkg` source package: `audit=1:3.0-1`

Binary Packages:

- `libaudit-common=1:3.0-1`
- `libaudit1:amd64=1:3.0-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/audit/1:3.0-1/


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

### `dpkg` source package: `base-passwd=3.5.48`

Binary Packages:

- `base-passwd=3.5.48`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.48
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.48.dsc' base-passwd_3.5.48.dsc 1757 SHA256:846789aa0586335f225865ba0c025544adbdb46c1f31596da9755cbf407a316e
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.48.tar.xz' base-passwd_3.5.48.tar.xz 53080 SHA256:bd14fb0f21c3d5ed3cae691bc95d3828572d957cf28f582803fb04f1638fbbbc
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.48/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.48/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.48/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.1-2`

Binary Packages:

- `bash=5.1-2`

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

### `dpkg` source package: `cdebconf=0.256`

Binary Packages:

- `libdebconfclient0:amd64=0.256`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.256
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.256.dsc' cdebconf_0.256.dsc 2750 SHA256:a4a90c0d0116f9892c2d627a34ed13c538742702165e75c10fa62994329ad78d
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.256.tar.xz' cdebconf_0.256.tar.xz 278240 SHA256:c6265de643520976b7deee12912da06956bbe401ec011f3a5aabaf38e376c711
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.256/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.256/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.256/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20200708+dd9ef66-5.dsc' dash_0.5.11+git20200708+dd9ef66-5.dsc 1906 SHA256:b0568c34647dc2aa0b8e2656c5e7449d9a1feb4b89d6857f507173b1f9a42ee7
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20200708+dd9ef66.orig.tar.gz' dash_0.5.11+git20200708+dd9ef66.orig.tar.gz 167776 SHA256:ab70b1f165bfedadd1282da546f1c917f1b7ccb2c5c2f898310a963e2ab5520c
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.11+git20200708+dd9ef66-5.debian.tar.xz' dash_0.5.11+git20200708+dd9ef66-5.debian.tar.xz 43120 SHA256:5da6039e043c953ff91a31c767ed703699870682ff356a1642f4798ce04a2926
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.11+git20200708+dd9ef66-5/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.11+git20200708+dd9ef66-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.11+git20200708+dd9ef66-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `elfutils=0.182-2`

Binary Packages:

- `libelf1:amd64=0.182-2`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/elfutils/0.182-2/


### `dpkg` source package: `findutils=4.7.0+git20201010-2`

Binary Packages:

- `findutils=4.7.0+git20201010-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.7.0+git20201010-2
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0+git20201010-2.dsc' findutils_4.7.0+git20201010-2.dsc 2136 SHA256:9ba9f5e02b662d1d6d404aa21d9e5827dac60e0c1879a82698ba0c8be6cf062e
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0+git20201010.orig.tar.xz' findutils_4.7.0+git20201010.orig.tar.xz 1950076 SHA256:f690859f9615cc8fdf04e6f0675c2d1881e9655dffe065cab5fd7f04d8fe6768
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.7.0+git20201010-2.debian.tar.xz' findutils_4.7.0+git20201010-2.debian.tar.xz 27852 SHA256:4555e249a33b492959d15c1fabe19724b4a49e491a83d46ee248d600c58ed397
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.7.0+git20201010-2/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.7.0+git20201010-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.7.0+git20201010-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-10=10.2.1-3`

Binary Packages:

- `gcc-10-base:amd64=10.2.1-3`
- `libgcc-s1:amd64=10.2.1-3`
- `libstdc++6:amd64=10.2.1-3`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.2.1-3
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.2.1-3.dsc' gcc-10_10.2.1-3.dsc 27635 SHA256:d928ae679faeb64fe3b3898163a2d8cdfa757f770016aaa42d1a1899e3aa4016
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.2.1.orig.tar.gz' gcc-10_10.2.1.orig.tar.gz 97337200 SHA256:a04738b0cfcdef4c9b5a04f587cc53dfb45fabb8c363cda1a91cb667bd9ad553
'http://deb.debian.org/debian/pool/main/g/gcc-10/gcc-10_10.2.1-3.debian.tar.xz' gcc-10_10.2.1-3.debian.tar.xz 2313976 SHA256:aa2c00754f924daaa3f658dc828ed652b307573b278e83f37562b803d68f0ede
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-10/10.2.1-3/ (for browsing the source)
- https://sources.debian.net/src/gcc-10/10.2.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-10/10.2.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-9=9.3.0-19`

Binary Packages:

- `gcc-9-base:amd64=9.3.0-19`

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
$ apt-get source -qq --print-uris gcc-9=9.3.0-19
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0-19.dsc' gcc-9_9.3.0-19.dsc 21922 SHA256:05150c28a603170b6194832ee195f79b66a4dfe8c9153d1d8af5fe5402525fc5
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0.orig.tar.gz' gcc-9_9.3.0.orig.tar.gz 88686943 SHA256:824044ffa96eb337bb1c1d4cf6a82691d0290d6f42e1d13362eea855458de060
'http://deb.debian.org/debian/pool/main/g/gcc-9/gcc-9_9.3.0-19.debian.tar.xz' gcc-9_9.3.0-19.debian.tar.xz 849704 SHA256:b5301a295d6bee7bbab146b310df584bfef792ef744c8df1f12d7a3e4c50b5e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-9/9.3.0-19/ (for browsing the source)
- https://sources.debian.net/src/gcc-9/9.3.0-19/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-9/9.3.0-19/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.31-9`

Binary Packages:

- `libc-bin=2.31-9`
- `libc6:amd64=2.31-9`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.31-9
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31-9.dsc' glibc_2.31-9.dsc 8311 SHA256:5f4848ef9d3b98e3271ec9a8077b50147d37db93575fa73a9de487b095e2973c
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31.orig.tar.xz' glibc_2.31.orig.tar.xz 17254692 SHA256:3dc7704b6166839c37d7047626fd199f3d4c09aca0d90e48c51c31c967dce34e
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.31-9.debian.tar.xz' glibc_2.31-9.debian.tar.xz 902504 SHA256:4d1644f39bfbbb2eec8c3e4aceda7472ee435a7a9bf73dc2967ddde0a2e35230
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.31-9/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.31-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.31-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.1+dfsg-1`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg-1
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg-1.dsc' gmp_6.2.1+dfsg-1.dsc 2145 SHA256:2644a10ca1e7d2ebbfb74d16449e485cd79d985a73ddffd258a138222178cb91
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA256:c6ba08e3f079260ab90ff44ab8801eae134cd62cd78f4aa56317c0e70daa40cb
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1+dfsg-1.debian.tar.xz' gmp_6.2.1+dfsg-1.debian.tar.xz 21248 SHA256:5b9fa90b68ca3323bb7a31b60fbd2b495609e39d7b1f21f0f6f1955ca5916163
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gnutls28=3.7.0-5`

Binary Packages:

- `libgnutls30:amd64=3.7.0-5`

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
$ apt-get source -qq --print-uris gnutls28=3.7.0-5
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0-5.dsc' gnutls28_3.7.0-5.dsc 3480 SHA256:d2b1242f130cfd626dc57b285352f371f56d74df978801077cbe89c9394fc519
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0.orig.tar.xz' gnutls28_3.7.0.orig.tar.xz 6129176 SHA256:49e2a22691d252c9f24a9829b293a8f359095bc5a818351f05f1c0a5188a1df8
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0.orig.tar.xz.asc' gnutls28_3.7.0.orig.tar.xz.asc 854 SHA256:c530ea9141b0164c0842840483365c43f7defa3ceb765894f2ddd9751d8864a4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0-5.debian.tar.xz' gnutls28_3.7.0-5.debian.tar.xz 70816 SHA256:acc933295f34c4ef01589a39afc9da6ae026e773b8c371d8d9b1fcff7cbd2fe6
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.0-5/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.0-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `iproute2=5.10.0-2`

Binary Packages:

- `iproute2=5.10.0-2`

Licenses: (parsed from: `/usr/share/doc/iproute2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris iproute2=5.10.0-2
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_5.10.0-2.dsc' iproute2_5.10.0-2.dsc 1864 SHA256:6fe367fb79acf8041e17f610c8108d63503eb7a9e1148677128691177929935f
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_5.10.0.orig.tar.xz' iproute2_5.10.0.orig.tar.xz 798348 SHA256:1508c9476a5b087d26f094e031a2d4fda184783a630f09596e0a6c1f978cee96
'http://deb.debian.org/debian/pool/main/i/iproute2/iproute2_5.10.0-2.debian.tar.xz' iproute2_5.10.0-2.debian.tar.xz 63864 SHA256:2a5fa082085d1f57afd5487d055e4c5a06a41896594bb2ecaf0cce331cf197b2
```

Other potentially useful URLs:

- https://sources.debian.net/src/iproute2/5.10.0-2/ (for browsing the source)
- https://sources.debian.net/src/iproute2/5.10.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iproute2/5.10.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iptables=1.8.6-1`

Binary Packages:

- `libxtables12:amd64=1.8.6-1`

Licenses: (parsed from: `/usr/share/doc/libxtables12/copyright`)

- `Artistic`
- `GPL-2`
- `GPL-2+`
- `custom`

Source:

```console
$ apt-get source -qq --print-uris iptables=1.8.6-1
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.6-1.dsc' iptables_1.8.6-1.dsc 2719 SHA256:425a5c18b34d76acda4b4ff86ae1f4128f6c20b3e611aea3fe6e0849b94e87e1
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.6.orig.tar.bz2' iptables_1.8.6.orig.tar.bz2 715744 SHA256:a0f4fe0c3eb8faa5bd9c8376d132f340b9558e750c91deb2d5028aa3d0047767
'http://deb.debian.org/debian/pool/main/i/iptables/iptables_1.8.6-1.debian.tar.xz' iptables_1.8.6-1.debian.tar.xz 23704 SHA256:e2fe8f88618a23a3553ad29387a650cc6d5c66d668b557f812a792a643310fa2
```

Other potentially useful URLs:

- https://sources.debian.net/src/iptables/1.8.6-1/ (for browsing the source)
- https://sources.debian.net/src/iptables/1.8.6-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iptables/1.8.6-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `iputils=3:20200821-2`

Binary Packages:

- `iputils-ping=3:20200821-2`

Licenses: (parsed from: `/usr/share/doc/iputils-ping/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris iputils=3:20200821-2
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20200821-2.dsc' iputils_20200821-2.dsc 2169 SHA256:f5dfc4aa59ad125978d1b81bbe59a887b11c63af4ba4940da1042337322c80f5
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20200821.orig.tar.xz' iputils_20200821.orig.tar.xz 438336 SHA256:3e6a9a753ab9f6ae377feb78c995914d98a6c86b3646c8c0a5cae23578b1a8d7
'http://deb.debian.org/debian/pool/main/i/iputils/iputils_20200821-2.debian.tar.xz' iputils_20200821-2.debian.tar.xz 10416 SHA256:d90c20bba5d2d03f196a2ba3d3e65850fe6767de3ab07d321231d5973881d0e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/iputils/3:20200821-2/ (for browsing the source)
- https://sources.debian.net/src/iputils/3:20200821-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/iputils/3:20200821-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbpf=0.3-1`

Binary Packages:

- `libbpf0:amd64=1:0.3-1`

Licenses: (parsed from: `/usr/share/doc/libbpf0/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2 with Linux-syscall-note exception`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libbpf=0.3-1
'http://deb.debian.org/debian/pool/main/libb/libbpf/libbpf_0.3-1.dsc' libbpf_0.3-1.dsc 1846 SHA256:55892a32f115ec35d8c2ae220fab9162794cca8fe50875873d001b3ab90bbbf2
'http://deb.debian.org/debian/pool/main/libb/libbpf/libbpf_0.3.orig.tar.gz' libbpf_0.3.orig.tar.gz 979131 SHA256:c168d84a75b541f753ceb49015d9eb886e3fb5cca87cdd9aabce7e10ad3a1efc
'http://deb.debian.org/debian/pool/main/libb/libbpf/libbpf_0.3-1.debian.tar.xz' libbpf_0.3-1.debian.tar.xz 5368 SHA256:cab4b3358490802be62c16064429fdf2384629f4be23211416432a26b8b69965
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbpf/0.3-1/ (for browsing the source)
- https://sources.debian.net/src/libbpf/0.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbpf/0.3-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libffi=3.3-5`

Binary Packages:

- `libffi7:amd64=3.3-5`

Licenses: (parsed from: `/usr/share/doc/libffi7/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.3-5
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-5.dsc' libffi_3.3-5.dsc 1918 SHA256:761deecc2a4cf6c4b1b751f5e3f3b22d0893772cf7c935f0001a65ed133fa0dd
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3.orig.tar.gz' libffi_3.3.orig.tar.gz 1305466 SHA256:72fba7922703ddfa7a028d513ac15a85c8d54c8d67f55fa5a4802885dc652056
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.3-5.debian.tar.xz' libffi_3.3-5.debian.tar.xz 9056 SHA256:6bf37bfa4b2ee8d05810217347cca2a5ae04dd3efc79aa6478e0215c9f75079f
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.3-5/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.3-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.3-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.8.7-2`

Binary Packages:

- `libgcrypt20:amd64=1.8.7-2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.7-2
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-2.dsc' libgcrypt20_1.8.7-2.dsc 2800 SHA256:002a04bd579933b9788900f924c1ee38b851eefc23496a64d83aa2c898bcba1a
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2' libgcrypt20_1.8.7.orig.tar.bz2 2985660 SHA256:03b70f028299561b7034b8966d7dd77ef16ed139c43440925fe8782561974748
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2.asc' libgcrypt20_1.8.7.orig.tar.bz2.asc 228 SHA256:eed6bb4174433640a02c1dc8851f34f85ec55b43d76a24bec87d7175784ef614
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-2.debian.tar.xz' libgcrypt20_1.8.7-2.debian.tar.xz 31668 SHA256:bbb04d6482684d298a6c7aa19dfbbe8b26ab154491d92afae1d95d5303e1c691
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.8.7-2/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.8.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.8.7-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libidn2=2.3.0-4`

Binary Packages:

- `libidn2-0:amd64=2.3.0-4`

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
$ apt-get source -qq --print-uris libidn2=2.3.0-4
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0-4.dsc' libidn2_2.3.0-4.dsc 2046 SHA256:77e2918866e2e0bda02e61f23d9a03173bccea3c96af557d7d81f7921f80d91b
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0.orig.tar.gz' libidn2_2.3.0.orig.tar.gz 2164993 SHA256:e1cb1db3d2e249a6a3eb6f0946777c2e892d5c5dc7bd91c74394fc3a01cab8b5
'http://deb.debian.org/debian/pool/main/libi/libidn2/libidn2_2.3.0-4.debian.tar.xz' libidn2_2.3.0-4.debian.tar.xz 11476 SHA256:11d256a27af58908cc7ddf7dc4e3987f5752156de43707604762d0095bf1042e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libidn2/2.3.0-4/ (for browsing the source)
- https://sources.debian.net/src/libidn2/2.3.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libidn2/2.3.0-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libseccomp=2.5.1-1`

Binary Packages:

- `libseccomp2:amd64=2.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.1-1
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1-1.dsc' libseccomp_2.5.1-1.dsc 2676 SHA256:dca165a5c3308ce0b2e030afa709892fba27f62fe9bc30c984bafe0d5f8e10ee
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1.orig.tar.gz' libseccomp_2.5.1.orig.tar.gz 638811 SHA256:ee307e383c77aa7995abc5ada544d51c9723ae399768a97667d4cdb3c3a30d55
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1.orig.tar.gz.asc' libseccomp_2.5.1.orig.tar.gz.asc 833 SHA256:14d45c86e5ceed5ac5511c3ebf70a4dca128b7584b314dc8a551c779ea225d2e
'http://deb.debian.org/debian/pool/main/libs/libseccomp/libseccomp_2.5.1-1.debian.tar.xz' libseccomp_2.5.1-1.debian.tar.xz 16088 SHA256:09a67e85111bafdda96efe64b7c0c3135a6875ab2d8936f3650e229ba82a2eb1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libseccomp/2.5.1-1/ (for browsing the source)
- https://sources.debian.net/src/libseccomp/2.5.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libseccomp/2.5.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libselinux=3.1-2`

Binary Packages:

- `libselinux1:amd64=3.1-2+b2`

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

### `dpkg` source package: `libxcrypt=1:4.4.17-1`

Binary Packages:

- `libcrypt1:amd64=1:4.4.17-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.17-1
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.17-1.dsc' libxcrypt_4.4.17-1.dsc 1463 SHA256:404666b7959510140e036344184d1648c51c410c7d65fbc7b6cad871d41bfd77
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.17.orig.tar.xz' libxcrypt_4.4.17.orig.tar.xz 389052 SHA256:b6189c6076ee88df6fe2bd14b1e90a73a5ca3a808052e16c7fcd0bf16448c677
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.17-1.debian.tar.xz' libxcrypt_4.4.17-1.debian.tar.xz 5536 SHA256:dc69cdb7c48521231ff13ebc3d432d3775a41fbbc534bf89a60b526a538eca4d
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.17-1/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.17-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.17-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.4.8+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.4.8+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.8+dfsg-1
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-1.dsc' libzstd_1.4.8+dfsg-1.dsc 2291 SHA256:f2d02ff2c386a2cf77d7d5b942aba42adc4083107bb9fe09a25666bdbfe6e4a7
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8+dfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA256:1e8ce5c4880a6d5bd8d3186e4186607dd19b64fc98a3877fc13aeefd566d67c5
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-1.debian.tar.xz' libzstd_1.4.8+dfsg-1.debian.tar.xz 13240 SHA256:064fe623d03eb5985cf05278d762bc3d6d3e7ac6232cfa7d1642637ae119e06b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.4.8+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.4.8+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.4.8+dfsg-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `lz4=1.9.3-1`

Binary Packages:

- `liblz4-1:amd64=1.9.3-1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.3-1
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.3-1.dsc' lz4_1.9.3-1.dsc 1959 SHA256:587dfa6ede9af7eabea15522aeba5dc99c07e6ebfc22fb0c8b182f238d3d43fb
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.3.orig.tar.gz' lz4_1.9.3.orig.tar.gz 320958 SHA256:030644df4611007ff7dc962d981f390361e6c97a34e5cbc393ddfbe019ffe2c1
'http://deb.debian.org/debian/pool/main/l/lz4/lz4_1.9.3-1.debian.tar.xz' lz4_1.9.3-1.debian.tar.xz 13536 SHA256:6d9a7eaf8b9c695553d92a0e15c99cdd5acddd2b609decebbd046cd935c52265
```

Other potentially useful URLs:

- https://sources.debian.net/src/lz4/1.9.3-1/ (for browsing the source)
- https://sources.debian.net/src/lz4/1.9.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lz4/1.9.3-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `ncurses=6.2+20201114-2`

Binary Packages:

- `libtinfo6:amd64=6.2+20201114-2`
- `ncurses-base=6.2+20201114-2`
- `ncurses-bin=6.2+20201114-2`

Licenses: (parsed from: `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2+20201114-2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20201114-2.dsc' ncurses_6.2+20201114-2.dsc 4106 SHA256:011ec8e3464be0d89d6611ab8fa0a84ac5514c0064e12dec9c52ec7b135408b1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20201114.orig.tar.gz' ncurses_6.2+20201114.orig.tar.gz 3539796 SHA256:aa3f8cfaff2a2b78f184274ec43d9da910c864e4b4d80fc47b5b48cba9154cd2
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20201114.orig.tar.gz.asc' ncurses_6.2+20201114.orig.tar.gz.asc 265 SHA256:91615d9d5575f9e974e78c6aca55e1885f42d1b2600cebec407be4471bb7a27d
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.2+20201114-2.debian.tar.xz' ncurses_6.2+20201114-2.debian.tar.xz 51812 SHA256:6ebba60b18cf2aceaa67098bfed1b1aa31c03f1a500f45c65ab098ec0a2401d2
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.2+20201114-2/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.2+20201114-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.2+20201114-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `p11-kit=0.23.22-1`

Binary Packages:

- `libp11-kit0:amd64=0.23.22-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

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

### `dpkg` source package: `perl=5.32.0-6`

Binary Packages:

- `perl-base=5.32.0-6`

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
$ apt-get source -qq --print-uris perl=5.32.0-6
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.0-6.dsc' perl_5.32.0-6.dsc 2997 SHA256:462ccbf2488da171a1b53c6b00ef6c047466307a7ee1a14b19913d37714a5020
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.0.orig-regen-configure.tar.gz' perl_5.32.0.orig-regen-configure.tar.gz 833536 SHA256:c40fa434ff0d6889f31e5e44d36dc568c77887159b55e7b12e49e979d4c4bd55
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.0.orig.tar.xz' perl_5.32.0.orig.tar.xz 12717336 SHA256:6f436b447cf56d22464f980fac1916e707a040e96d52172984c5d184c09b859b
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.0-6.debian.tar.xz' perl_5.32.0-6.debian.tar.xz 164248 SHA256:8c282ed61faa72b5847f7e963b4d9c8078850f6462931da369dd8d36ea4ad7fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.32.0-6/ (for browsing the source)
- https://sources.debian.net/src/perl/5.32.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.32.0-6/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `systemd=247.2-4`

Binary Packages:

- `libsystemd0:amd64=247.2-4`
- `libudev1:amd64=247.2-4`

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
$ apt-get source -qq --print-uris systemd=247.2-4
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.2-4.dsc' systemd_247.2-4.dsc 5167 SHA256:32d877a6666d05c4410ed5d3ba023acdcc9a7cd153069e8ff4ac8e7127740610
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.2.orig.tar.gz' systemd_247.2.orig.tar.gz 9890845 SHA256:e6100f447f67a49f6e019ff7ee317cf8b67a5c491e54dcf8b02975d4307fa468
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.2-4.debian.tar.xz' systemd_247.2-4.debian.tar.xz 156452 SHA256:f68d6bebc4d02c7c02bf4c3c536799e842a765efa734efed148805d33a9e96e7
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/247.2-4/ (for browsing the source)
- https://sources.debian.net/src/systemd/247.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/247.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=2.96-5`

Binary Packages:

- `sysvinit-utils=2.96-5`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-5
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-5.dsc' sysvinit_2.96-5.dsc 2612 SHA256:8d30544cea96d93b875a41d403500db61b9e0abb7175eb69ac76a19f3b69d6da
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA256:2a2e26b72aa235a23ab1c8471005f890309ce1196c83fbc9413c57b9ab62b587
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA256:dfc184b95da12c8c888c8ae6b0f26fe8a23b07fbcdd240f6600a8a78b9439fa0
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-5.debian.tar.xz' sysvinit_2.96-5.debian.tar.xz 128096 SHA256:956f0b67990f83cdb437e4663729450dfa5b014b1b268ab3739eb034431544b6
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.96-5/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.96-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.96-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.32+dfsg-1`

Binary Packages:

- `tar=1.32+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.32+dfsg-1
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.32+dfsg-1.dsc' tar_1.32+dfsg-1.dsc 2015 SHA256:8154c63983aadb982496a047384688c223bb8ffe50146dd05d4138c66dec75cd
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.32+dfsg.orig.tar.xz' tar_1.32+dfsg.orig.tar.xz 1910772 SHA256:9cb89ab8997d5469b24c7a676f0f0ae5b84d730c3d44d9afeabad63431ec8d27
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.32+dfsg-1.debian.tar.xz' tar_1.32+dfsg-1.debian.tar.xz 19460 SHA256:2d4bfe8c6121762fb99d440ad6ab98ad761e02d933d53bdaa5d932661473868c
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.32+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/tar/1.32+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.32+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2020f-1`

Binary Packages:

- `tzdata=2020f-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2020f-1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020f-1.dsc' tzdata_2020f-1.dsc 2237 SHA256:3c06e34890c1bd0a664639633762e279f95d9783040c8326d24ea6c6b1daa6e2
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020f.orig.tar.gz' tzdata_2020f.orig.tar.gz 411739 SHA256:121131918c3ae6dc5d40f0eb87563a2be920b71a76e2392c09519a5e4a666881
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020f.orig.tar.gz.asc' tzdata_2020f.orig.tar.gz.asc 833 SHA256:5b10a0a0cad012e4cd9683b7d3d69160803b93d2fd66cdb6de5fa35d471df6f2
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2020f-1.debian.tar.xz' tzdata_2020f-1.debian.tar.xz 105144 SHA256:1a45295c1bebd4f1379082a476612915b8550e9c382a08c65def0ea2e5a94bcb
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2020f-1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2020f-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2020f-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.36.1-3`

Binary Packages:

- `bsdutils=1:2.36.1-3`
- `libblkid1:amd64=2.36.1-3`
- `libmount1:amd64=2.36.1-3`
- `libsmartcols1:amd64=2.36.1-3`
- `libuuid1:amd64=2.36.1-3`
- `mount=2.36.1-3`
- `util-linux=2.36.1-3`

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

- http://snapshot.debian.org/package/util-linux/2.36.1-3/


### `dpkg` source package: `xxhash=0.8.0-1`

Binary Packages:

- `libxxhash0:amd64=0.8.0-1`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.0-1
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.0-1.dsc' xxhash_0.8.0-1.dsc 1601 SHA256:1926a58706bf07202366d04e0a062e05cad342c78c83f892da7fa2781fd17220
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.0.orig.tar.gz' xxhash_0.8.0.orig.tar.gz 145909 SHA256:7054c3ebd169c97b64a92d7b994ab63c70dd53a06974f1f630ab782c28db0f4f
'http://deb.debian.org/debian/pool/main/x/xxhash/xxhash_0.8.0-1.debian.tar.xz' xxhash_0.8.0-1.debian.tar.xz 3772 SHA256:2543f82555a56cd044c6c908373dd249b6055d1ca197eba87942249da89dc3fd
```

Other potentially useful URLs:

- https://sources.debian.net/src/xxhash/0.8.0-1/ (for browsing the source)
- https://sources.debian.net/src/xxhash/0.8.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xxhash/0.8.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xz-utils=5.2.5-1.0`

Binary Packages:

- `liblzma5:amd64=5.2.5-1.0`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-1.0
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-1.0.dsc' xz-utils_5.2.5-1.0.dsc 2527 SHA256:21fef59fb4b1ee054f5a29830e7e1416348c3a56cf24efbb422eefebbcbe094d
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA256:3e1e518ffc912f86608a8cb35e4bd41ad1aec210df2a47aaa1f95e7f5576ef56
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz.asc' xz-utils_5.2.5.orig.tar.xz.asc 833 SHA256:6efc0075a58912e640119d2b52ef7d1518b260d8720fadc73df21ab7fc727624
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.5-1.0.debian.tar.xz' xz-utils_5.2.5-1.0.debian.tar.xz 31636 SHA256:163c5236a25cc8432fe6c2785c4c66916ea71e1e966130492bbe34f9a1ee679a
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.5-1.0/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.5-1.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.5-1.0/ (for access to the source package after it no longer exists in the archive)

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
