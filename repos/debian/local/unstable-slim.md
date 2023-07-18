# `debian:unstable-slim`

## Docker Metadata

- Image ID: `sha256:595acc5a06a66d7c0a8162185b9579bfa9aa22e8ec60837ad57a224bbac5c040`
- Created: `2023-07-04T01:23:38.353283391Z`
- Virtual Size: ~ 74.39 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.3.1-3`

Binary Packages:

- `libacl1:amd64=2.3.1-3`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.3.1-3
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-3.dsc' acl_2.3.1-3.dsc 2508 SHA256:7820eee88cce7244e0b8eb25cc4f51bdf10aff7a6c1a497f3d18c36bdce712cc
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz' acl_2.3.1.orig.tar.xz 355676 SHA256:c0234042e17f11306c23c038b08e5e070edb7be44bef6697fb8734dcff1c66b1
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz.asc' acl_2.3.1.orig.tar.xz.asc 833 SHA256:54fb8fcd6ae6901f2257e18d503e5e18ad956babf8d80d2ea29f280fc7264662
'http://deb.debian.org/debian/pool/main/a/acl/acl_2.3.1-3.debian.tar.xz' acl_2.3.1-3.debian.tar.xz 30968 SHA256:2eb052bba784a4b873e951b1f91af2abef62e4bf4b83c93f9821eea26f66c8e2
```

Other potentially useful URLs:

- https://sources.debian.net/src/acl/2.3.1-3/ (for browsing the source)
- https://sources.debian.net/src/acl/2.3.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/acl/2.3.1-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `adduser=3.137`

Binary Packages:

- `adduser=3.137`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.137
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.137.dsc' adduser_3.137.dsc 1671 SHA256:e4be6fbfa9db7ca7054a1c31dd2f1503340187b547112c960f2482ce3642f837
'http://deb.debian.org/debian/pool/main/a/adduser/adduser_3.137.tar.xz' adduser_3.137.tar.xz 279192 SHA256:229a61803664c2850f7d8d93e6650cd0b340ea3bbd1b954271719679ea3b0dd0
```

Other potentially useful URLs:

- https://sources.debian.net/src/adduser/3.137/ (for browsing the source)
- https://sources.debian.net/src/adduser/3.137/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/adduser/3.137/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=2.6.1`

Binary Packages:

- `apt=2.6.1`
- `libapt-pkg6.0:amd64=2.6.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.6.1/


### `dpkg` source package: `attr=1:2.5.1-4`

Binary Packages:

- `libattr1:amd64=1:2.5.1-4`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.5.1-4
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-4.dsc' attr_2.5.1-4.dsc 2477 SHA256:0e1486bff1649602cb5cbb6224dbb641436dc8cd28d5c336ad85d650e07d23dd
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA256:db448a626f9313a1a970d636767316a8da32aede70518b8050fa0de7947adc32
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA256:67bc632e754efbadba846d0b40138b3fc3e306c3b909a9ba868c6dba1e2689d0
'http://deb.debian.org/debian/pool/main/a/attr/attr_2.5.1-4.debian.tar.xz' attr_2.5.1-4.debian.tar.xz 32152 SHA256:aea02a3c980a82804a5a333bf02e9e2737a8c5808671625595511290863d6791
```

Other potentially useful URLs:

- https://sources.debian.net/src/attr/1:2.5.1-4/ (for browsing the source)
- https://sources.debian.net/src/attr/1:2.5.1-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/attr/1:2.5.1-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `audit=1:3.0.9-1`

Binary Packages:

- `libaudit-common=1:3.0.9-1`
- `libaudit1:amd64=1:3.0.9-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/audit/1:3.0.9-1/


### `dpkg` source package: `base-files=13`

Binary Packages:

- `base-files=13`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=13
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_13.dsc' base-files_13.dsc 1093 SHA256:9a355f5c19670ce338c4febb196c427cc5f67940953478b515d555fba9fbdddc
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_13.tar.xz' base-files_13.tar.xz 66064 SHA256:439153bdf296481135cb0b801fe46765dc83f8b9914a0275d6a162339de12f56
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/13/ (for browsing the source)
- https://sources.debian.net/src/base-files/13/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/13/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-passwd=3.6.1`

Binary Packages:

- `base-passwd=3.6.1`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.6.1
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.6.1.dsc' base-passwd_3.6.1.dsc 1740 SHA256:b4e5fcdba73369657b241743033e8e7a65c26da43285503c652fa1436ce75d1f
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.6.1.tar.xz' base-passwd_3.6.1.tar.xz 56072 SHA256:6ff369be59d586ba63c0c5fcb00f75f9953fe49db88bc6c6428f2c92866f79af
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.6.1/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.6.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.6.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.2.15-2`

Binary Packages:

- `bash=5.2.15-2+b2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `BSD-4-clause-UC`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `Latex2e`
- `MIT-like`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris bash=5.2.15-2
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.2.15-2.dsc' bash_5.2.15-2.dsc 2317 SHA256:f51753e946af43eb58549c81e03b35a47af9fe6c6364179ccd4ef862b7c3b2d3
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.2.15.orig.tar.gz' bash_5.2.15.orig.tar.gz 9997221 SHA256:7a315bc0e9d90713159e4390ec1096a41e4f33cd8cc3d1a749a8e5ad56600f51
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.2.15-2.debian.tar.xz' bash_5.2.15-2.debian.tar.xz 97380 SHA256:998f8ea5b754a734ae7d8306e149c43d713ddfcf49623a036004b729237dbcca
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/5.2.15-2/ (for browsing the source)
- https://sources.debian.net/src/bash/5.2.15-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/5.2.15-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `libbz2-1.0:amd64=1.0.8-5+b1`

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

### `dpkg` source package: `cdebconf=0.270`

Binary Packages:

- `libdebconfclient0:amd64=0.270`

Licenses: (parsed from: `/usr/share/doc/libdebconfclient0/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.270
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.270.dsc' cdebconf_0.270.dsc 2703 SHA256:d7f396abbbfb2d38fc15589358d05618c9918f4f10facfe1ac259efef91e8a5f
'http://deb.debian.org/debian/pool/main/c/cdebconf/cdebconf_0.270.tar.xz' cdebconf_0.270.tar.xz 284336 SHA256:c27ef57f7dc8a2e7e9651cd0e964f543677bb314a1cf9bc1019736818e342638
```

Other potentially useful URLs:

- https://sources.debian.net/src/cdebconf/0.270/ (for browsing the source)
- https://sources.debian.net/src/cdebconf/0.270/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cdebconf/0.270/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `coreutils=9.1-1`

Binary Packages:

- `coreutils=9.1-1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `BSD-4-clause-UC`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris coreutils=9.1-1
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_9.1-1.dsc' coreutils_9.1-1.dsc 1848 SHA256:2f2fca0a07a1a3f38e3ebeb4cbd97e97e675e77bed84f3e9d0b7e5da4cde75fc
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_9.1.orig.tar.xz' coreutils_9.1.orig.tar.xz 5712104 SHA256:61a1f410d78ba7e7f37a5a4f50e6d1320aca33375484a3255eddf17a38580423
'http://deb.debian.org/debian/pool/main/c/coreutils/coreutils_9.1-1.debian.tar.xz' coreutils_9.1-1.debian.tar.xz 30624 SHA256:45d4ae88d933a7d713ef038943e818a2488e759b6196a409788744cbc6df1832
```

Other potentially useful URLs:

- https://sources.debian.net/src/coreutils/9.1-1/ (for browsing the source)
- https://sources.debian.net/src/coreutils/9.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/coreutils/9.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.12-6`

Binary Packages:

- `dash=0.5.12-6`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.12-6
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.12-6.dsc' dash_0.5.12-6.dsc 1520 SHA256:dfca9cb9a537d09c190baa9fb15848ecaa55f301843779f26260b1429cd72746
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.12.orig.tar.gz' dash_0.5.12.orig.tar.gz 246054 SHA256:6a474ac46e8b0b32916c4c60df694c82058d3297d8b385b74508030ca4a8f28a
'http://deb.debian.org/debian/pool/main/d/dash/dash_0.5.12-6.debian.tar.xz' dash_0.5.12-6.debian.tar.xz 39116 SHA256:155173292d95943d2c737c0f7f4733bb6b39244522f810ee4a64f7be0f4865ab
```

Other potentially useful URLs:

- https://sources.debian.net/src/dash/0.5.12-6/ (for browsing the source)
- https://sources.debian.net/src/dash/0.5.12-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dash/0.5.12-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `db5.3=5.3.28+dfsg2-1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg2-1`

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
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg2-1
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-1.dsc' db5.3_5.3.28+dfsg2-1.dsc 2887 SHA256:fe84d3cd7cde381f1c5a18f223377cf84ea7627ced8063ef33ef8fd93f6e09f4
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2.orig.tar.xz' db5.3_5.3.28+dfsg2.orig.tar.xz 21287688 SHA256:ad41b507415dec8316e828b2230242af2251d2c86eefa3c7aa9ef47c5239ef33
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-1.debian.tar.xz' db5.3_5.3.28+dfsg2-1.debian.tar.xz 34660 SHA256:52cb792fe53138c79a0328ffd1d771e3112791f546fd00e0dcd4b0e3efc5d916
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg2-1/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.82`

Binary Packages:

- `debconf=1.5.82`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.82
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.82.dsc' debconf_1.5.82.dsc 2035 SHA256:ed6e8cc6e073344a25ab932602b3b814f25cfa1a7bfd69e464f9bad65f250dea
'http://deb.debian.org/debian/pool/main/d/debconf/debconf_1.5.82.tar.xz' debconf_1.5.82.tar.xz 571540 SHA256:2d0550c4e2fb98d12055b245907978b28ee2d2b07b62e46be7523384d2ce985e
```

Other potentially useful URLs:

- https://sources.debian.net/src/debconf/1.5.82/ (for browsing the source)
- https://sources.debian.net/src/debconf/1.5.82/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debconf/1.5.82/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debian-archive-keyring=2023.3`

Binary Packages:

- `debian-archive-keyring=2023.3`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2023.3
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2023.3.dsc' debian-archive-keyring_2023.3.dsc 1261 SHA256:31c1ef4aaa73e1b4b3a85a88993a7f5180d9f697a8784f58471d9d39047409f9
'http://deb.debian.org/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2023.3.tar.xz' debian-archive-keyring_2023.3.tar.xz 177472 SHA256:0b9af95add8f2f7834d90f95ce6fde065319148c9363f140077b03684a71eea8
```

Other potentially useful URLs:

- https://sources.debian.net/src/debian-archive-keyring/2023.3/ (for browsing the source)
- https://sources.debian.net/src/debian-archive-keyring/2023.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debian-archive-keyring/2023.3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debianutils=5.7-0.4`

Binary Packages:

- `debianutils=5.7-0.4`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`
- `GPL-2+`
- `SMAIL-GPL`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debianutils/5.7-0.4/


### `dpkg` source package: `diffutils=1:3.8-4`

Binary Packages:

- `diffutils=1:3.8-4`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `FSFAP`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with autoconf exception`
- `GPL-3+ with texinfo exception`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3.0+`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.8-4
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8-4.dsc' diffutils_3.8-4.dsc 1705 SHA256:783af1a151c2a0f42a8a427693cc4bb16037c0d17282d28672d906f2eab424b8
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz' diffutils_3.8.orig.tar.xz 1585120 SHA256:a6bdd7d1b31266d11c4f4de6c1b748d4607ab0231af5188fc2533d0ae2438fec
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz.asc' diffutils_3.8.orig.tar.xz.asc 833 SHA256:500f423d0ffa8d28966d916ed5fc6b79fb160a20ed5cb74eeb1c94a30c340311
'http://deb.debian.org/debian/pool/main/d/diffutils/diffutils_3.8-4.debian.tar.xz' diffutils_3.8-4.debian.tar.xz 14428 SHA256:36abe3a3174c32c3646ca6bad212169a322409086c4a98f967bb9ad58f11c8d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/diffutils/1:3.8-4/ (for browsing the source)
- https://sources.debian.net/src/diffutils/1:3.8-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/diffutils/1:3.8-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dpkg=1.21.22`

Binary Packages:

- `dpkg=1.21.22`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.22
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.22.dsc' dpkg_1.21.22.dsc 3061 SHA256:fd3433a8e8f6cb2435b954ea5f5a200f8bdd04ce158568750d567ca23f47d144
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.21.22.tar.xz' dpkg_1.21.22.tar.xz 5419900 SHA256:5a1d15481bba79d7a4899fd55b4b6b18a987ca8d56ee8c43e9cab63b8a0a3545
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.21.22/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.21.22/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.21.22/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.47.0-2`

Binary Packages:

- `e2fsprogs=1.47.0-2`
- `libcom-err2:amd64=1.47.0-2`
- `libext2fs2:amd64=1.47.0-2`
- `libss2:amd64=1.47.0-2`
- `logsave=1.47.0-2`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `Apache-2`
- `Apache-2.0`
- `BSD-3-Clause`
- `GPL`
- `GPL-2`
- `GPL-2+ with Texinfo exception`
- `ISC`
- `Kazlib`
- `LGPL-2`
- `Latex2e`
- `MIT-US-export`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.47.0-2
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0-2.dsc' e2fsprogs_1.47.0-2.dsc 2846 SHA256:35b4de254e021f721362b767994598e249fea02e38ac446197cd9c22be1130fd
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0.orig.tar.gz' e2fsprogs_1.47.0.orig.tar.gz 9637717 SHA256:6667afde56eef0c6af26684974400e4d2288ea49e9441bf5e6229195d51a3578
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0.orig.tar.gz.asc' e2fsprogs_1.47.0.orig.tar.gz.asc 488 SHA256:704928204a52ddaa0ac8ef549c1bfba3c38e66c361d3853c8a4c38e6082b90f1
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.47.0-2.debian.tar.xz' e2fsprogs_1.47.0-2.debian.tar.xz 87328 SHA256:3a756e08d300666039e34577293d11d70c7a1da7850fad478580a81af6348277
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.47.0-2/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.47.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.47.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `findutils=4.9.0-5`

Binary Packages:

- `findutils=4.9.0-5`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `BSD-3-clause`
- `BSD-3-clause and/or GPL-3+`
- `FSFAP`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL with automake exception`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf-data exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Autoconf-data exception`
- `GPL-3+ with Bison-2.2 exception`
- `ISC`
- `ISC and/or LGPL-2.1+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.9.0-5
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-5.dsc' findutils_4.9.0-5.dsc 2272 SHA256:7d723c60c50b8b624250ad7d6fbb1ca404756a7b69209753e57c8403e06a07a5
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA256:a2bfb8c09d436770edc59f50fa483e785b161a3b7b9d547573cb08065fd462fe
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA256:924c3719d066eda1b3e47175f8b83e90e9a23f0a639ebe7445621917b283c385
'http://deb.debian.org/debian/pool/main/f/findutils/findutils_4.9.0-5.debian.tar.xz' findutils_4.9.0-5.debian.tar.xz 32744 SHA256:456831869d49d8906a98beb2bcbb61e5911d9c44082c4b716615bc23f26c4f20
```

Other potentially useful URLs:

- https://sources.debian.net/src/findutils/4.9.0-5/ (for browsing the source)
- https://sources.debian.net/src/findutils/4.9.0-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/findutils/4.9.0-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-13=13.1.0-7`

Binary Packages:

- `gcc-13-base:amd64=13.1.0-7`
- `libgcc-s1:amd64=13.1.0-7`
- `libstdc++6:amd64=13.1.0-7`

Licenses: (parsed from: `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-13=13.1.0-7
'http://deb.debian.org/debian/pool/main/g/gcc-13/gcc-13_13.1.0-7.dsc' gcc-13_13.1.0-7.dsc 27472 SHA256:88933c1861e2194614f6cd01ed6b833268ad2a49f39379361f9e53b85f0fb8e8
'http://deb.debian.org/debian/pool/main/g/gcc-13/gcc-13_13.1.0.orig.tar.gz' gcc-13_13.1.0.orig.tar.gz 89274824 SHA256:885e4a54319e74321cca4c412aad11a2be0df81d816a3c1856e1430a03b6f4b0
'http://deb.debian.org/debian/pool/main/g/gcc-13/gcc-13_13.1.0-7.debian.tar.xz' gcc-13_13.1.0-7.debian.tar.xz 1315992 SHA256:f02f9d40f90dfdf77f8a72f62317faf98db8c60118d1a51bde5d020231202cbf
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-13/13.1.0-7/ (for browsing the source)
- https://sources.debian.net/src/gcc-13/13.1.0-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-13/13.1.0-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.37-3`

Binary Packages:

- `libc-bin=2.37-3`
- `libc6:amd64=2.37-3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.37-3
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.37-3.dsc' glibc_2.37-3.dsc 9685 SHA256:0ebe98c39a1c01a9e65ea2b652c8ec7e3074a4de54999cf195a6e4aa7065b136
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.37.orig.tar.xz' glibc_2.37.orig.tar.xz 19503016 SHA256:d05f010158c16cef110fa1ab560c31477249ee2105360101858a5146aa6fe7d0
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.37-3.debian.tar.xz' glibc_2.37-3.debian.tar.xz 787472 SHA256:6bb235311f2e5f80562fce95a8a3fbe517b83498c6db9a6dba709f83790e29e4
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.37-3/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.37-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.37-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gmp=2:6.2.1+dfsg1-1.1`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg1-1.1`

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
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg1-1.1
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.1.dsc' gmp_6.2.1+dfsg1-1.1.dsc 2238 SHA256:2831ed4f83bc3304c2403474b335652ab2dc507cd517de44414d9142171748f0
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1.orig.tar.xz' gmp_6.2.1+dfsg1.orig.tar.xz 1787428 SHA256:471b9e463e04362a0124f215afc5f0a4b99caedeeb62634c61bbc12988efa64c
'http://deb.debian.org/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.1.debian.tar.xz' gmp_6.2.1+dfsg1-1.1.debian.tar.xz 19444 SHA256:4e3e324d72fe688e409c716d33b35aa8657f6016cc1aabd5d9c7ec137412e5ef
```

Other potentially useful URLs:

- https://sources.debian.net/src/gmp/2:6.2.1+dfsg1-1.1/ (for browsing the source)
- https://sources.debian.net/src/gmp/2:6.2.1+dfsg1-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gmp/2:6.2.1+dfsg1-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnupg2=2.2.40-1.1`

Binary Packages:

- `gpgv=2.2.40-1.1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.40-1.1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.1.dsc' gnupg2_2.2.40-1.1.dsc 3832 SHA256:89bdffd4176066d37fb5d250a1e5512c428529d10f13413a12893f86a757697f
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2' gnupg2_2.2.40.orig.tar.bz2 7301631 SHA256:1164b29a75e8ab93ea15033300149e1872a7ef6bdda3d7c78229a735f8204c28
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2.asc' gnupg2_2.2.40.orig.tar.bz2.asc 228 SHA256:3907dc165299cd53c0b4aec862323c3bce6037c411600ec87dc5eed7a55eba4a
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.1.debian.tar.xz' gnupg2_2.2.40-1.1.debian.tar.xz 62368 SHA256:356b7c86afdbaab286c5b92816cd1e1f4616cb67d22407c616618ef4d1680a9b
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.40-1.1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.40-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.40-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.9-2`

Binary Packages:

- `libgnutls30:amd64=3.7.9-2`

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
$ apt-get source -qq --print-uris gnutls28=3.7.9-2
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.9-2.dsc' gnutls28_3.7.9-2.dsc 3386 SHA256:65a8fe5a079115b9f2381d3071cbe4f5f00c2dc2a8ef04aab47523ae66f636e4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.9.orig.tar.xz' gnutls28_3.7.9.orig.tar.xz 6377212 SHA256:aaa03416cdbd54eb155187b359e3ec3ed52ec73df4df35a0edd49429ff64d844
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.9.orig.tar.xz.asc' gnutls28_3.7.9.orig.tar.xz.asc 996 SHA256:da4a96b14edd3cd44971a36ba1e976af1057e57a2d6c21b0cc7025c983ee84cc
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.9-2.debian.tar.xz' gnutls28_3.7.9-2.debian.tar.xz 85892 SHA256:1f5f0a73e1f0b25e481785398f7e213237810841ee3860475acbbcc9b0dd16bf
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.9-2/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.9-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.9-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.8-5`

Binary Packages:

- `grep=3.8-5`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/grep/3.8-5/


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

### `dpkg` source package: `hostname=3.23+nmu1`

Binary Packages:

- `hostname=3.23+nmu1`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23+nmu1
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.23%2bnmu1.dsc' hostname_3.23+nmu1.dsc 1281 SHA256:56f2189eaeee638e86d29a05356e7001632e33b2132a41a4634a9ff839264ea6
'http://deb.debian.org/debian/pool/main/h/hostname/hostname_3.23%2bnmu1.tar.xz' hostname_3.23+nmu1.tar.xz 12876 SHA256:f3fb39f30b00ba7dba2cec013195d7e1bb215f241153208ccd52da3eedfe7a7d
```

Other potentially useful URLs:

- https://sources.debian.net/src/hostname/3.23+nmu1/ (for browsing the source)
- https://sources.debian.net/src/hostname/3.23+nmu1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/hostname/3.23+nmu1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `init-system-helpers=1.65.2`

Binary Packages:

- `init-system-helpers=1.65.2`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.65.2
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.65.2.dsc' init-system-helpers_1.65.2.dsc 2195 SHA256:3889593844b232df78f3f886aed6d8351fe0539cee8d15a721d4b682c6a83538
'http://deb.debian.org/debian/pool/main/i/init-system-helpers/init-system-helpers_1.65.2.tar.xz' init-system-helpers_1.65.2.tar.xz 44400 SHA256:888bd5642f31396fd2b1a6f9c8f56ba5f6651fb599dae2b9eecf239902162cae
```

Other potentially useful URLs:

- https://sources.debian.net/src/init-system-helpers/1.65.2/ (for browsing the source)
- https://sources.debian.net/src/init-system-helpers/1.65.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/init-system-helpers/1.65.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.8.3-1`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1+b3`

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

### `dpkg` source package: `libcap2=1:2.66-4`

Binary Packages:

- `libcap2:amd64=1:2.66-4`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.66-4
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.66-4.dsc' libcap2_2.66-4.dsc 2204 SHA256:ab4aaa349c824acaebfb63bec2d2bc10e7cee10ec6725ac6f21f1fe12aa9d8fb
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.66.orig.tar.xz' libcap2_2.66.orig.tar.xz 181592 SHA256:15c40ededb3003d70a283fe587a36b7d19c8b3b554e33f86129c059a4bb466b2
'http://deb.debian.org/debian/pool/main/libc/libcap2/libcap2_2.66-4.debian.tar.xz' libcap2_2.66-4.debian.tar.xz 21468 SHA256:5379eec3a05e40c2485ebe451506883c1f2f99d552c6ded29607080fd278dd7c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcap2/1:2.66-4/ (for browsing the source)
- https://sources.debian.net/src/libcap2/1:2.66-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcap2/1:2.66-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libffi=3.4.4-1`

Binary Packages:

- `libffi8:amd64=3.4.4-1`

Licenses: (parsed from: `/usr/share/doc/libffi8/copyright`)

- `Expat`
- `GPL`
- `GPL-2+`
- `GPL-3+`
- `LGPL-2.1+`
- `MPL-1.1`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.4-1
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.4-1.dsc' libffi_3.4.4-1.dsc 1951 SHA256:21c9ef156b6766535cb014e0765142c8104ffbcd73f003ecfa80cfb314baa4f0
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.4.orig.tar.gz' libffi_3.4.4.orig.tar.gz 1362394 SHA256:d66c56ad259a82cf2a9dfc408b32bf5da52371500b84745f7fb8b645712df676
'http://deb.debian.org/debian/pool/main/libf/libffi/libffi_3.4.4-1.debian.tar.xz' libffi_3.4.4-1.debian.tar.xz 10380 SHA256:161b210bfd2ada0b15b0d2a2a98ffc779cd4a68661a7fdf46f61732493db0895
```

Other potentially useful URLs:

- https://sources.debian.net/src/libffi/3.4.4-1/ (for browsing the source)
- https://sources.debian.net/src/libffi/3.4.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libffi/3.4.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgcrypt20=1.10.2-2`

Binary Packages:

- `libgcrypt20:amd64=1.10.2-2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.2-2
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2-2.dsc' libgcrypt20_1.10.2-2.dsc 2806 SHA256:98f0e92e279815de7d194ad4613e09ce273a9f885b0623fb96a7c2dd054fb55c
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2.orig.tar.bz2' libgcrypt20_1.10.2.orig.tar.bz2 3795164 SHA256:3b9c02a004b68c256add99701de00b383accccf37177e0d6c58289664cce0c03
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2.orig.tar.bz2.asc' libgcrypt20_1.10.2.orig.tar.bz2.asc 228 SHA256:3b5b729d3969b3e828acc483709a686678cecaf20e8559eb525da905c7aa2bcb
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2-2.debian.tar.xz' libgcrypt20_1.10.2-2.debian.tar.xz 35928 SHA256:af27c09663eec29c4c517db892a8b74096fadde77ac4986496bac8e390dd8f6c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.10.2-2/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.10.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.10.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libgpg-error=1.46-1`

Binary Packages:

- `libgpg-error0:amd64=1.46-1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.46-1
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.46-1.dsc' libgpg-error_1.46-1.dsc 2273 SHA256:f1fe4ca2f252f797c2819b0eae1e284e2f0b2c7ac8ec16209054ae45878aaafe
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.46.orig.tar.bz2' libgpg-error_1.46.orig.tar.bz2 1014291 SHA256:b7e11a64246bbe5ef37748de43b245abd72cfcd53c9ae5e7fc5ca59f1c81268d
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.46.orig.tar.bz2.asc' libgpg-error_1.46.orig.tar.bz2.asc 228 SHA256:e0eb40e705068858ee43b6462b204aacf5a554fe4a17cfe63ea99e9612f72e9d
'http://deb.debian.org/debian/pool/main/libg/libgpg-error/libgpg-error_1.46-1.debian.tar.xz' libgpg-error_1.46-1.debian.tar.xz 18532 SHA256:2f80416e16dead749fb6a31a0a3703ae9e562bd32fc4d72184636a1501cd86ef
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgpg-error/1.46-1/ (for browsing the source)
- https://sources.debian.net/src/libgpg-error/1.46-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgpg-error/1.46-1/ (for access to the source package after it no longer exists in the archive)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libidn2/2.3.3-1/


### `dpkg` source package: `libmd=1.1.0-1`

Binary Packages:

- `libmd0:amd64=1.1.0-1`

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
$ apt-get source -qq --print-uris libmd=1.1.0-1
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0-1.dsc' libmd_1.1.0-1.dsc 2283 SHA256:abb74aa06e06dbb88f4c1a7764e1d93c753bdcb60e7151a1897fe247750f5ef1
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0.orig.tar.xz' libmd_1.1.0.orig.tar.xz 271228 SHA256:1bd6aa42275313af3141c7cf2e5b964e8b1fd488025caf2f971f43b00776b332
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0.orig.tar.xz.asc' libmd_1.1.0.orig.tar.xz.asc 833 SHA256:402fd3024e43ab975733d09e661804a58ca58697194e4b15216b1217cfe1dadb
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.1.0-1.debian.tar.xz' libmd_1.1.0-1.debian.tar.xz 8156 SHA256:4e9403dcdd277ae81bb83bc7f4ba9fe5fd6640b74118d8349904f029510596dc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmd/1.1.0-1/ (for browsing the source)
- https://sources.debian.net/src/libmd/1.1.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmd/1.1.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libseccomp=2.5.4-1`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1+b3`

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

- `libselinux1:amd64=3.4-1+b6`

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
- `libsemanage2:amd64=3.4-1+b5`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libsemanage/3.4-1/


### `dpkg` source package: `libsepol=3.4-2.1`

Binary Packages:

- `libsepol2:amd64=3.4-2.1`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libsepol/3.4-2.1/


### `dpkg` source package: `libtasn1-6=4.19.0-3`

Binary Packages:

- `libtasn1-6:amd64=4.19.0-3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.19.0-3
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-3.dsc' libtasn1-6_4.19.0-3.dsc 2662 SHA256:7fd9618be5b99035c7387d969b73365a57b1f6f01ec4abe0af332829af718190
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz' libtasn1-6_4.19.0.orig.tar.gz 1786576 SHA256:1613f0ac1cf484d6ec0ce3b8c06d56263cc7242f1c23b30d82d23de345a63f7a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz.asc' libtasn1-6_4.19.0.orig.tar.gz.asc 228 SHA256:8410c0c004f3509c218a98b276b3308b9c46f48068e8b1a6d9ebfd61ea9f357a
'http://deb.debian.org/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-3.debian.tar.xz' libtasn1-6_4.19.0-3.debian.tar.xz 22084 SHA256:acb32dc03d8c2aeb10e0fb1c2a0247efdab0a6dc5e8f8a4d3cdcfe5ad26bb0df
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtasn1-6/4.19.0-3/ (for browsing the source)
- https://sources.debian.net/src/libtasn1-6/4.19.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtasn1-6/4.19.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libunistring=1.0-2`

Binary Packages:

- `libunistring2:amd64=1.0-2`

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
$ apt-get source -qq --print-uris libunistring=1.0-2
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.0-2.dsc' libunistring_1.0-2.dsc 2181 SHA256:9b9a9d9d4cd1c2118df8cf5ca0dfb787d89afcd99400d7cd01b4c4e9b0bc1ae5
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz' libunistring_1.0.orig.tar.xz 2367800 SHA256:5bab55b49f75d77ed26b257997e919b693f29fd4a1bc22e0e6e024c246c72741
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz.asc' libunistring_1.0.orig.tar.xz.asc 833 SHA256:c1c2ae60eb971593da92e65384a5f1b181717e7b9654854f139f350c6cbe235d
'http://deb.debian.org/debian/pool/main/libu/libunistring/libunistring_1.0-2.debian.tar.xz' libunistring_1.0-2.debian.tar.xz 14520 SHA256:e550d94935cd06eafb0defd7b5d7c914c7bb80a8e818a49efcf7675206572450
```

Other potentially useful URLs:

- https://sources.debian.net/src/libunistring/1.0-2/ (for browsing the source)
- https://sources.debian.net/src/libunistring/1.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libunistring/1.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libxcrypt=1:4.4.35-1`

Binary Packages:

- `libcrypt1:amd64=1:4.4.35-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.35-1
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.35-1.dsc' libxcrypt_4.4.35-1.dsc 1591 SHA256:f984567dc7761aa528f15491aa97c66dfb8b91be9746499936982387498b79bd
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.35.orig.tar.xz' libxcrypt_4.4.35.orig.tar.xz 393948 SHA256:520aa182205c5744630a224e169db5ffce6f439942d3d3866f139260f52876a2
'http://deb.debian.org/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.35-1.debian.tar.xz' libxcrypt_4.4.35-1.debian.tar.xz 8204 SHA256:d4cc6726f30fcc58e301ad7b6ca1353d1b346f3a76a88210ea73bf223cb385d7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxcrypt/1:4.4.35-1/ (for browsing the source)
- https://sources.debian.net/src/libxcrypt/1:4.4.35-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxcrypt/1:4.4.35-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.5.5+dfsg2-1`

Binary Packages:

- `libzstd1:amd64=1.5.5+dfsg2-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.5+dfsg2-1
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-1.dsc' libzstd_1.5.5+dfsg2-1.dsc 2324 SHA256:503b2677c4d316fd409731949de064369d27a3addb858c2ca962ef65f91ed546
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2.orig.tar.xz' libzstd_1.5.5+dfsg2.orig.tar.xz 1784164 SHA256:d7cf3c10d416fd999cb8fcf7685d9268ba7bec8eb78121fc2d0d916fa393d22b
'http://deb.debian.org/debian/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-1.debian.tar.xz' libzstd_1.5.5+dfsg2-1.debian.tar.xz 21144 SHA256:1c5070fa2228e1ae1cca4798e2388a58bb4160c14714d518baa9ef595e80f864
```

Other potentially useful URLs:

- https://sources.debian.net/src/libzstd/1.5.5+dfsg2-1/ (for browsing the source)
- https://sources.debian.net/src/libzstd/1.5.5+dfsg2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libzstd/1.5.5+dfsg2-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mawk=1.3.4.20230525-1`

Binary Packages:

- `mawk=1.3.4.20230525-1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `GPL-2.0-only`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20230525-1
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20230525-1.dsc' mawk_1.3.4.20230525-1.dsc 1918 SHA256:e6fd0a6d20e18d5a99b76bb9246794a47878f130efa28b8ee52edc89ea810020
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20230525.orig.tar.gz' mawk_1.3.4.20230525.orig.tar.gz 403222 SHA256:5639d14bb9124373b3d7f957d2b925ad8ad9656d46212c3f23dbca810cc9269f
'http://deb.debian.org/debian/pool/main/m/mawk/mawk_1.3.4.20230525-1.debian.tar.xz' mawk_1.3.4.20230525-1.debian.tar.xz 14288 SHA256:5d0b292f99d20e72fb03f47e37e30ee46283302b0bea1bebef90c30819699837
```

Other potentially useful URLs:

- https://sources.debian.net/src/mawk/1.3.4.20230525-1/ (for browsing the source)
- https://sources.debian.net/src/mawk/1.3.4.20230525-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mawk/1.3.4.20230525-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.4+20230625-1`

Binary Packages:

- `libtinfo6:amd64=6.4+20230625-1`
- `ncurses-base=6.4+20230625-1`
- `ncurses-bin=6.4+20230625-1`

Licenses: (parsed from: `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.4+20230625-1
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.4%2b20230625-1.dsc' ncurses_6.4+20230625-1.dsc 3807 SHA256:7f5cfc1271d60b30ebc46df49654f099b4f5492cea5159115c6cfdc245972d25
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.4%2b20230625.orig.tar.gz' ncurses_6.4+20230625.orig.tar.gz 3649551 SHA256:54d25c0215c1b7f6f17d64c7f8f229fb34af007d663c0fcd54d9557a1cacc3ee
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.4%2b20230625.orig.tar.gz.asc' ncurses_6.4+20230625.orig.tar.gz.asc 729 SHA256:d20a0166bdf9f8eccc6df015a49fd60a168f00f8430431810fc49963b44c0965
'http://deb.debian.org/debian/pool/main/n/ncurses/ncurses_6.4%2b20230625-1.debian.tar.xz' ncurses_6.4+20230625-1.debian.tar.xz 50328 SHA256:c068f9d6e751ebbfeb5cee05a010580fd539c0251da4a703cc1d14427b284798
```

Other potentially useful URLs:

- https://sources.debian.net/src/ncurses/6.4+20230625-1/ (for browsing the source)
- https://sources.debian.net/src/ncurses/6.4+20230625-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ncurses/6.4+20230625-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `p11-kit=0.24.1-2`

Binary Packages:

- `libp11-kit0:amd64=0.24.1-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `LGPL-2.1`
- `LGPL-2.1+`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/p11-kit/0.24.1-2/


### `dpkg` source package: `pam=1.5.2-6`

Binary Packages:

- `libpam-modules:amd64=1.5.2-6`
- `libpam-modules-bin=1.5.2-6`
- `libpam-runtime=1.5.2-6`
- `libpam0g:amd64=1.5.2-6`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `BSD-3-clause`
- `BSD-tcp_wrappers`
- `Beerware`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+ with Bison exception`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pam=1.5.2-6
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-6.dsc' pam_1.5.2-6.dsc 1998 SHA256:2dbff29f5fc189c95b863ffd690795a7313515619ddadc470eab8a50b7555903
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA256:e4ec7131a91da44512574268f493c6d8ca105c87091691b8e9b56ca685d4f94d
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-6.debian.tar.xz' pam_1.5.2-6.debian.tar.xz 122320 SHA256:97adad0df930ba5ed52b88bef6d494a1b303ca2eb5be9e347479a23e4d9254fc
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.5.2-6/ (for browsing the source)
- https://sources.debian.net/src/pam/1.5.2-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.5.2-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.42-1`

Binary Packages:

- `libpcre2-8-0:amd64=10.42-1`

Licenses: (parsed from: `/usr/share/doc/libpcre2-8-0/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-3-clause-Cambridge with BINARY LIBRARY-LIKE PACKAGES exception`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pcre2=10.42-1
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.42-1.dsc' pcre2_10.42-1.dsc 2302 SHA256:726dafe7a8d07332d4df61edf23f384ddb158b2b263846273d1103b6b9a7c176
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.42.orig.tar.gz' pcre2_10.42.orig.tar.gz 2397194 SHA256:c33b418e3b936ee3153de2c61cc638e7e4fe3156022a5c77d0711bcbb9d64f1f
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.42-1.diff.gz' pcre2_10.42-1.diff.gz 7895 SHA256:8267c3acacb04e8a077235f676187393e295443fc16ff46ddbe5f6476879c8cb
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.42-1/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.42-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.42-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.36.0-7`

Binary Packages:

- `perl-base=5.36.0-7`

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
$ apt-get source -qq --print-uris perl=5.36.0-7
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0-7.dsc' perl_5.36.0-7.dsc 2886 SHA256:d9992947bb5c254e1bf96c56f12ac0bc962a2ff1e700834f871fb412526b4a8b
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0.orig-regen-configure.tar.xz' perl_5.36.0.orig-regen-configure.tar.xz 417784 SHA256:10ac353bc5a933403afe60ed1817e7a456f99bdbcaf80c1cdb0eb3a08ea56d4e
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0.orig.tar.xz' perl_5.36.0.orig.tar.xz 13051500 SHA256:0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0-7.debian.tar.xz' perl_5.36.0-7.debian.tar.xz 169288 SHA256:c8a46245b7102d60539cc4c550977f35cbb8409643abc0d00c7a8b78d0271bea
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.36.0-7/ (for browsing the source)
- https://sources.debian.net/src/perl/5.36.0-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.36.0-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sed=4.9-1`

Binary Packages:

- `sed=4.9-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `BSD-4-clause-UC`
- `BSL-1`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `X11`
- `pcre`

Source:

```console
$ apt-get source -qq --print-uris sed=4.9-1
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9-1.dsc' sed_4.9-1.dsc 2077 SHA256:f0670e00c1ad51321e5b741a737e977cdb3b0eef47964b2269535f7820df576a
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9.orig.tar.xz' sed_4.9.orig.tar.xz 1397092 SHA256:6e226b732e1cd739464ad6862bd1a1aba42d7982922da7a53519631d24975181
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9.orig.tar.xz.asc' sed_4.9.orig.tar.xz.asc 833 SHA256:9ea64f215b308ae0a80cd958daaac23bb13491d69a472a0195974d107890a8c6
'http://deb.debian.org/debian/pool/main/s/sed/sed_4.9-1.debian.tar.xz' sed_4.9-1.debian.tar.xz 62616 SHA256:24cdd6a3b40909ec374bd87df62364904bbe18fc12ba66111e9f9f617ff7f679
```

Other potentially useful URLs:

- https://sources.debian.net/src/sed/4.9-1/ (for browsing the source)
- https://sources.debian.net/src/sed/4.9-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sed/4.9-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `shadow=1:4.13+dfsg1-1`

Binary Packages:

- `login=1:4.13+dfsg1-1+b1`
- `passwd=1:4.13+dfsg1-1+b1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.13+dfsg1-1
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1-1.dsc' shadow_4.13+dfsg1-1.dsc 2402 SHA256:e27b0676e87d4ae75a57cba55433517e8aa30d45817c691c63045d5e6195c667
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1.orig.tar.xz' shadow_4.13+dfsg1.orig.tar.xz 1811752 SHA256:a8bb3a2aceff1cbe39d0f50687dcc1d7e7be0516a9d954d8e2eedb93f5906207
'http://deb.debian.org/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1-1.debian.tar.xz' shadow_4.13+dfsg1-1.debian.tar.xz 78988 SHA256:cbd43c96ebad42bfb1656b5e691cc165f52d1dd6b1ee89202c2a09e59d663b1c
```

Other potentially useful URLs:

- https://sources.debian.net/src/shadow/1:4.13+dfsg1-1/ (for browsing the source)
- https://sources.debian.net/src/shadow/1:4.13+dfsg1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/shadow/1:4.13+dfsg1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=253.5-1`

Binary Packages:

- `libsystemd0:amd64=253.5-1`
- `libudev1:amd64=253.5-1`

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

- http://snapshot.debian.org/package/systemd/253.5-1/


### `dpkg` source package: `sysvinit=3.07-1`

Binary Packages:

- `sysvinit-utils=3.07-1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.07-1
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.07-1.dsc' sysvinit_3.07-1.dsc 2359 SHA256:a65764c7ce0d78529300bcc195c7816b33b52a4347f84102c4a4d39c8a912183
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.07.orig.tar.gz' sysvinit_3.07.orig.tar.gz 513168 SHA256:79ac3d1b3b52cee328a59f4f5357104eafde6f146c2ee10a929096d7177c83df
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.07-1.debian.tar.xz' sysvinit_3.07-1.debian.tar.xz 134388 SHA256:a2fbffb5f18fe4179b17fef1f6bc1ba7615f3747c221c08d3996b8906f5a5115
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/3.07-1/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/3.07-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/3.07-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.34+dfsg-1.2`

Binary Packages:

- `tar=1.34+dfsg-1.2`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1.2
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg-1.2.dsc' tar_1.34+dfsg-1.2.dsc 1768 SHA256:4e7999f6d8a7fef2d09aa5b915877357a80c68ab0a339ee802b304d0e99e7517
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA256:7d57029540cb928394defb3b377b3531237c947e795b51aa8acac0c5ba0e4844
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34%2bdfsg-1.2.debian.tar.xz' tar_1.34+dfsg-1.2.debian.tar.xz 20336 SHA256:6e32291771f375a7e08cc4cabad1a658327d3dd7a4ff1b557a338ffe0675a25c
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.34+dfsg-1.2/ (for browsing the source)
- https://sources.debian.net/src/tar/1.34+dfsg-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.34+dfsg-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2023c-6`

Binary Packages:

- `tzdata=2023c-6`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tzdata/2023c-6/


### `dpkg` source package: `usrmerge=35`

Binary Packages:

- `usr-is-merged=35`

Licenses: (parsed from: `/usr/share/doc/usr-is-merged/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=35
'http://deb.debian.org/debian/pool/main/u/usrmerge/usrmerge_35.dsc' usrmerge_35.dsc 981 SHA256:f8f7fa03aa912a65f54584b1cbaed193575521ab7ffa16c93c9920c41726c9fd
'http://deb.debian.org/debian/pool/main/u/usrmerge/usrmerge_35.tar.xz' usrmerge_35.tar.xz 14416 SHA256:ec52fa22f174204f24ebb45caf579275f5a2b2404be5d4b3fe29ad60ad566829
```

Other potentially useful URLs:

- https://sources.debian.net/src/usrmerge/35/ (for browsing the source)
- https://sources.debian.net/src/usrmerge/35/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/usrmerge/35/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `util-linux=2.38.1-5`

Binary Packages:

- `bsdutils=1:2.38.1-5+b1`
- `libblkid1:amd64=2.38.1-5+b1`
- `libmount1:amd64=2.38.1-5+b1`
- `libsmartcols1:amd64=2.38.1-5+b1`
- `libuuid1:amd64=2.38.1-5+b1`
- `mount=2.38.1-5+b1`
- `util-linux=2.38.1-5+b1`
- `util-linux-extra=2.38.1-5+b1`

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
$ apt-get source -qq --print-uris util-linux=2.38.1-5
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1-5.dsc' util-linux_2.38.1-5.dsc 4547 SHA256:23b6c80b27468a9b7821ff7059b6a0bbb23fa9b2305856ffb78a993726491c08
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1.orig.tar.xz' util-linux_2.38.1.orig.tar.xz 7495904 SHA256:60492a19b44e6cf9a3ddff68325b333b8b52b6c59ce3ebd6a0ecaa4c5117e84f
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.38.1-5.debian.tar.xz' util-linux_2.38.1-5.debian.tar.xz 113832 SHA256:b7bd8e9105f199eccb7aac571f24a33f4738cdfc365a7e4b980ccb542b4d8c7a
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.38.1-5/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.38.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.38.1-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xz-utils=5.4.1-0.2`

Binary Packages:

- `liblzma5:amd64=5.4.1-0.2`

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
$ apt-get source -qq --print-uris xz-utils=5.4.1-0.2
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.dsc' xz-utils_5.4.1-0.2.dsc 2621 SHA256:faaef4551ecc9547f308ca65cdafe6d2fa43b06f11944001490079303c87bf40
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz' xz-utils_5.4.1.orig.tar.xz 1485272 SHA256:5d9827aa1875b21c288f78864bb26d2650b436ea8d2cad364e4921eb6266a5a5
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz.asc' xz-utils_5.4.1.orig.tar.xz.asc 833 SHA256:4b0c7707114996092a5f75a98333de2102db83a27218e4903b8fb7c24a8d0233
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.debian.tar.xz' xz-utils_5.4.1-0.2.debian.tar.xz 87432 SHA256:67eeab55ab3e4b35722d4ec255e0f735b3c61aab0437ab3c8274f5aa77c9c407
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.4.1-0.2/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.4.1-0.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.4.1-0.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.13.dfsg-1`

Binary Packages:

- `zlib1g:amd64=1:1.2.13.dfsg-1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.13.dfsg-1
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.13.dfsg-1.dsc' zlib_1.2.13.dfsg-1.dsc 2399 SHA256:3fa1e6b2fc525062aa88207dda52fed8e045373c809d362fe8a2bfbf7cf515a8
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.13.dfsg.orig.tar.bz2' zlib_1.2.13.dfsg.orig.tar.bz2 1239825 SHA256:71feb7947e3c00ef125f83b79a4e529bde31171e5babe48b391f06758d1ab0a1
'http://deb.debian.org/debian/pool/main/z/zlib/zlib_1.2.13.dfsg-1.debian.tar.xz' zlib_1.2.13.dfsg-1.debian.tar.xz 15700 SHA256:f66cf3d4f2d7defcd4d1fd1fb0a11ee39f1e01b42ec7d059c9dc5c1695133c44
```

Other potentially useful URLs:

- https://sources.debian.net/src/zlib/1:1.2.13.dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/zlib/1:1.2.13.dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zlib/1:1.2.13.dfsg-1/ (for access to the source package after it no longer exists in the archive)
