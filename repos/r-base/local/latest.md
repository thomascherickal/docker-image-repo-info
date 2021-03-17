# `r-base:4.0.4`

## Docker Metadata

- Image ID: `sha256:640cb54282114b70783269b890bf8daf5c22d436238405265cab644da51eeb99`
- Created: `2021-03-12T12:40:24.482059883Z`
- Virtual Size: ~ 761.21 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["R"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LC_ALL=en_US.UTF-8`
  - `LANG=en_US.UTF-8`
  - `R_BASE_VERSION=4.0.4`
- Labels:
  - `maintainer=Dirk Eddelbuettel <edd@debian.org>`
  - `org.label-schema.license=GPL-2.0`
  - `org.label-schema.vcs-url=https://github.com/rocker-org/r-base`
  - `org.label-schema.vendor=Rocker Project`

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

### `dpkg` source package: `apt=2.2.0`

Binary Packages:

- `apt=2.2.0`
- `libapt-pkg6.0:amd64=2.2.0`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.2.0/


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

### `dpkg` source package: `base-passwd=3.5.49`

Binary Packages:

- `base-passwd=3.5.49`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.49
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.49.dsc' base-passwd_3.5.49.dsc 1757 SHA256:8e8c81bbc7e7163fe9d471c195a191597624b789e7df2cd9358691a4c821b7c2
'http://deb.debian.org/debian/pool/main/b/base-passwd/base-passwd_3.5.49.tar.xz' base-passwd_3.5.49.tar.xz 53152 SHA256:5d0617b70a81f937a8ba91a1c4bf03bff472f84a0f3b841f67d945fecf539801
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-passwd/3.5.49/ (for browsing the source)
- https://sources.debian.net/src/base-passwd/3.5.49/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-passwd/3.5.49/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bash=5.1-2`

Binary Packages:

- `bash=5.1-2+b1`

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

### `dpkg` source package: `binutils=2.35.2-2`

Binary Packages:

- `binutils=2.35.2-2`
- `binutils-common:amd64=2.35.2-2`
- `binutils-x86-64-linux-gnu=2.35.2-2`
- `libbinutils:amd64=2.35.2-2`
- `libctf-nobfd0:amd64=2.35.2-2`
- `libctf0:amd64=2.35.2-2`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.35.2-2
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.35.2-2.dsc' binutils_2.35.2-2.dsc 11303 SHA256:6643177e54ce708b0aa347624018c2b9cf725aca6731142a48a655b12013a9d9
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.35.2.orig.tar.xz' binutils_2.35.2.orig.tar.xz 23514376 SHA256:2643d99d7aba8557319a4b018f6bcae58677fc9bc853d4c2cd2eb571867b75e7
'http://deb.debian.org/debian/pool/main/b/binutils/binutils_2.35.2-2.debian.tar.xz' binutils_2.35.2-2.debian.tar.xz 101124 SHA256:96f56b4d5259be49ce4a2f27057892356f7b0aed499742cb8a07f9f62b10dcb5
```

Other potentially useful URLs:

- https://sources.debian.net/src/binutils/2.35.2-2/ (for browsing the source)
- https://sources.debian.net/src/binutils/2.35.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/binutils/2.35.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `boot=1.3-27-1`

Binary Packages:

- `r-cran-boot=1.3-27-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-boot/copyright`)

- `'unlimited distribution'`

Source:

```console
$ apt-get source -qq --print-uris boot=1.3-27-1
'http://deb.debian.org/debian/pool/main/b/boot/boot_1.3-27-1.dsc' boot_1.3-27-1.dsc 1802 SHA256:4ba059c42eed209da21f6a8499579e94c38fff402b08c93f89312e41c0c6e46f
'http://deb.debian.org/debian/pool/main/b/boot/boot_1.3-27.orig.tar.gz' boot_1.3-27.orig.tar.gz 236799 SHA256:34b2db5b4570377eaaff99d91882ad522c528842def907489b035d22fbb52aed
'http://deb.debian.org/debian/pool/main/b/boot/boot_1.3-27-1.debian.tar.xz' boot_1.3-27-1.debian.tar.xz 5240 SHA256:477313e0342dc76f23ac950a05a33f8de892c2d24b2b1f1e79f21f80cb268021
```

Other potentially useful URLs:

- https://sources.debian.net/src/boot/1.3-27-1/ (for browsing the source)
- https://sources.debian.net/src/boot/1.3-27-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/boot/1.3-27-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `build-essential=12.9`

Binary Packages:

- `build-essential=12.9`

Licenses: (parsed from: `/usr/share/doc/build-essential/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris build-essential=12.9
'http://deb.debian.org/debian/pool/main/b/build-essential/build-essential_12.9.dsc' build-essential_12.9.dsc 2220 SHA256:1e4ad67c69001a162b2eb3a2019f037e53c8a1e312073ba1a2110d1e21971555
'http://deb.debian.org/debian/pool/main/b/build-essential/build-essential_12.9.tar.xz' build-essential_12.9.tar.xz 51532 SHA256:938da370b4ef883687d141723d1b7470ad76bec7a54158d3d6b9b38f9c9eedb2
```

Other potentially useful URLs:

- https://sources.debian.net/src/build-essential/12.9/ (for browsing the source)
- https://sources.debian.net/src/build-essential/12.9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/build-essential/12.9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `bzip2=1.0.8-4`

Binary Packages:

- `bzip2=1.0.8-4`
- `libbz2-1.0:amd64=1.0.8-4`
- `libbz2-dev:amd64=1.0.8-4`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

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

### `dpkg` source package: `cluster=2.1.1-1`

Binary Packages:

- `r-cran-cluster=2.1.1-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-cluster/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cluster=2.1.1-1
'http://deb.debian.org/debian/pool/main/c/cluster/cluster_2.1.1-1.dsc' cluster_2.1.1-1.dsc 1831 SHA256:7170cfee7df016f2c14601f298a747b0ff4db3408085d18aec70b3d2aee6cfff
'http://deb.debian.org/debian/pool/main/c/cluster/cluster_2.1.1.orig.tar.gz' cluster_2.1.1.orig.tar.gz 397306 SHA256:bdb8c709ec9b84922e185f68e1e817a83dfb130b2ef8c4beaee19ce382358063
'http://deb.debian.org/debian/pool/main/c/cluster/cluster_2.1.1-1.debian.tar.xz' cluster_2.1.1-1.debian.tar.xz 4224 SHA256:77e91f19a56e5bee486bfc3c27f919b5c41ada177231332c1d43f0d4abe5e2f9
```

Other potentially useful URLs:

- https://sources.debian.net/src/cluster/2.1.1-1/ (for browsing the source)
- https://sources.debian.net/src/cluster/2.1.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cluster/2.1.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `codetools=0.2-18-1`

Binary Packages:

- `r-cran-codetools=0.2-18-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-codetools/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris codetools=0.2-18-1
'http://deb.debian.org/debian/pool/main/c/codetools/codetools_0.2-18-1.dsc' codetools_0.2-18-1.dsc 1859 SHA256:c5dbbfdad52751ac6af3af2fa3a3dbb3267f136e024289a2102addc41b3e1ecf
'http://deb.debian.org/debian/pool/main/c/codetools/codetools_0.2-18.orig.tar.gz' codetools_0.2-18.orig.tar.gz 38175 SHA256:1a9ea6b9792dbd1688078455929385acc3a5e4bef945c77bec1261fa4a084c28
'http://deb.debian.org/debian/pool/main/c/codetools/codetools_0.2-18-1.debian.tar.xz' codetools_0.2-18-1.debian.tar.xz 2868 SHA256:be07b14194de74900cbcc6a7fb67f52be0be88a103cf4f71682997ebfb576718
```

Other potentially useful URLs:

- https://sources.debian.net/src/codetools/0.2-18-1/ (for browsing the source)
- https://sources.debian.net/src/codetools/0.2-18-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/codetools/0.2-18-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `curl=7.74.0-1.1`

Binary Packages:

- `libcurl4:amd64=7.74.0-1.1`

Licenses: (parsed from: `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.74.0-1.1
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0-1.1.dsc' curl_7.74.0-1.1.dsc 2667 SHA256:38a98f50c870a7be3891ef15c06eb5d8be48dacfbfc2d96765081de07ef4dd36
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0.orig.tar.gz' curl_7.74.0.orig.tar.gz 4043409 SHA256:e56b3921eeb7a2951959c02db0912b5fcd5fdba5aca071da819e1accf338bbd7
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.74.0-1.1.debian.tar.xz' curl_7.74.0-1.1.debian.tar.xz 31456 SHA256:7cbb5cff7442e71598997e83059221df6550276af35899775445218d020f9de6
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.74.0-1.1/ (for browsing the source)
- https://sources.debian.net/src/curl/7.74.0-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.74.0-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2.1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2.1
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.1.dsc' cyrus-sasl2_2.1.27+dfsg-2.1.dsc 3433 SHA256:714b4f59fdf5e3c436b0f10d15535f0048f5164a9a40763f2537fadbd2175da8
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.1.debian.tar.xz 101356 SHA256:0b2cf5e3118a8d99fc39a8133e5508de298b90507fb8c0846d4dae840bf4ec60
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2.1/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.27+dfsg-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg-2.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.8
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8.dsc' db5.3_5.3.28+dfsg1-0.8.dsc 3113 SHA256:5189bebd157e3b51c075804d1affebc87cdbfb782808c621e131660719c24374
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://deb.debian.org/debian/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8.debian.tar.xz' db5.3_5.3.28+dfsg1-0.8.debian.tar.xz 30748 SHA256:073c0c87283bf5e606f3ce6d1814315b40b9685c943601ae3fd81e2da4e612d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.8/ (for browsing the source)
- https://sources.debian.net/src/db5.3/5.3.28+dfsg1-0.8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/db5.3/5.3.28+dfsg1-0.8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `debconf=1.5.74`

Binary Packages:

- `debconf=1.5.74`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debconf/1.5.74/


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

### `dpkg` source package: `dpkg=1.20.7.1`

Binary Packages:

- `dpkg=1.20.7.1`
- `dpkg-dev=1.20.7.1`
- `libdpkg-perl=1.20.7.1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.20.7.1
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.20.7.1.dsc' dpkg_1.20.7.1.dsc 2128 SHA256:7d9c5cf363f7076bc19adc478add8be5d250d750899d8015575a529cb40e4516
'http://deb.debian.org/debian/pool/main/d/dpkg/dpkg_1.20.7.1.tar.xz' dpkg_1.20.7.1.tar.xz 4952736 SHA256:0aad2de687f797ef8ebdabc7bafd16dc1497f1ce23bd9146f9aa73f396a5636f
```

Other potentially useful URLs:

- https://sources.debian.net/src/dpkg/1.20.7.1/ (for browsing the source)
- https://sources.debian.net/src/dpkg/1.20.7.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/dpkg/1.20.7.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `e2fsprogs=1.46.1-1`

Binary Packages:

- `e2fsprogs=1.46.1-1`
- `libcom-err2:amd64=1.46.1-1`
- `libext2fs2:amd64=1.46.1-1`
- `libss2:amd64=1.46.1-1`
- `logsave=1.46.1-1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.1-1
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.1-1.dsc' e2fsprogs_1.46.1-1.dsc 2842 SHA256:bb84dbacf687767e01899c25e1913c48112b4e64a4fc15c0239e21df57997313
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.1.orig.tar.gz' e2fsprogs_1.46.1.orig.tar.gz 9490551 SHA256:49630dc777a808dc67312fa289dca65b9d2dbad80c8267f3b9d437b7167774e4
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.1.orig.tar.gz.asc' e2fsprogs_1.46.1.orig.tar.gz.asc 488 SHA256:f242d6916bc6c135d74f3c6662a62648ee4f18de16bad71152ce8061e131b316
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.1-1.debian.tar.xz' e2fsprogs_1.46.1-1.debian.tar.xz 81932 SHA256:8d64f5db2f96c8abdca8e400c1154ac21a33a157d00d792683ec99889dcc499e
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.46.1-1/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.46.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.46.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ed=1.17-1`

Binary Packages:

- `ed=1.17-1`

Licenses: (parsed from: `/usr/share/doc/ed/copyright`)

- `BSD-2-Clause`
- `FCONF`
- `FDOC`
- `FLOG`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris ed=1.17-1
'http://deb.debian.org/debian/pool/main/e/ed/ed_1.17-1.dsc' ed_1.17-1.dsc 1818 SHA256:05e781f628a47e71e25851dbd252a884b58f70226f0657b4b1b575a52bcc1e8d
'http://deb.debian.org/debian/pool/main/e/ed/ed_1.17.orig.tar.gz' ed_1.17.orig.tar.gz 90863 SHA256:6c84ce06fea002fe76f19bf66c3807edafd898b8ab0f15852e1497d48f44d96d
'http://deb.debian.org/debian/pool/main/e/ed/ed_1.17-1.debian.tar.xz' ed_1.17-1.debian.tar.xz 8464 SHA256:8cc3b3c1bfb139d8ac635d4fefa47f2aa289d007fcd1da553bad97ce26fe7f88
```

Other potentially useful URLs:

- https://sources.debian.net/src/ed/1.17-1/ (for browsing the source)
- https://sources.debian.net/src/ed/1.17-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ed/1.17-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.2.10-2`

Binary Packages:

- `libexpat1:amd64=2.2.10-2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.10-2
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.10-2.dsc' expat_2.2.10-2.dsc 1988 SHA256:f6cf4e5df4429e57f9d67d3a5bbcae5796e6744d392f95c4aeb9db9e056dc63c
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.10.orig.tar.gz' expat_2.2.10.orig.tar.gz 8276395 SHA256:62e280f5fd29a5b70973f623e20a7412c3e3912c2684cb0e462e2c881be129e1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.2.10-2.debian.tar.xz' expat_2.2.10-2.debian.tar.xz 10956 SHA256:1f618e2e5459fb78f7c9879e1964fa3ec03dd071ff4944005b99dc9600c0e4a8
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.2.10-2/ (for browsing the source)
- https://sources.debian.net/src/expat/2.2.10-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.2.10-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `foreign=0.8.81-1`

Binary Packages:

- `r-cran-foreign=0.8.81-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-foreign/copyright`)

- `GPL`
- `GPL `

Source:

```console
$ apt-get source -qq --print-uris foreign=0.8.81-1
'http://deb.debian.org/debian/pool/main/f/foreign/foreign_0.8.81-1.dsc' foreign_0.8.81-1.dsc 1838 SHA256:d7351f6d4fbf4c51191dac820d8ff8eccbe3283ca7114c836a6d904d31f2fba4
'http://deb.debian.org/debian/pool/main/f/foreign/foreign_0.8.81.orig.tar.gz' foreign_0.8.81.orig.tar.gz 363284 SHA256:1ae8f9f18f2a037697fa1a9060417ff255c71764f0145080b2bd23ba8262992c
'http://deb.debian.org/debian/pool/main/f/foreign/foreign_0.8.81-1.debian.tar.xz' foreign_0.8.81-1.debian.tar.xz 4272 SHA256:f178765a6a4476098361d52bd6aef0dc489e2a1e17c2d4876af51f7906636212
```

Other potentially useful URLs:

- https://sources.debian.net/src/foreign/0.8.81-1/ (for browsing the source)
- https://sources.debian.net/src/foreign/0.8.81-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/foreign/0.8.81-1/ (for access to the source package after it no longer exists in the archive)

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
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4+dfsg-1.dsc' freetype_2.10.4+dfsg-1.dsc 3693 SHA256:e49fd5a3be9816e2c9caf287e945a3257e60b809a50db83fcea2aa8e4ffa2438
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2demos.tar.xz' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz 236712 SHA256:3f873ebe4fb387da3859149459f9be95320ce1fd56b50f8fdb9d2a8492887083
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2demos.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz.asc 195 SHA256:38d5b9a5aa11ecf8c6d4c983ef48b3ce2288fdf93d44719df2598b9d415c8061
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2docs.tar.xz' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz 2079084 SHA256:cca1c19d1efa911bb685d919b5b0fe1279b0699bf8eb6a3d3bf9f02784758212
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2docs.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz.asc 195 SHA256:29fca9ff0e1cdc57ad5707b17f629eeaa216eb334f6082f1b05fb0fe35e14ff3
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4+dfsg.orig.tar.xz' freetype_2.10.4+dfsg.orig.tar.xz 2259340 SHA256:db0c0938b3b75cf314775baa75198098e41583b3aaa4804b454f183ce45120a9
'http://deb.debian.org/debian/pool/main/f/freetype/freetype_2.10.4+dfsg-1.debian.tar.xz' freetype_2.10.4+dfsg-1.debian.tar.xz 116636 SHA256:96276d66eb56247545cd9e60ffae0bd5b5aee0490e4e7171337a6666bc51b125
```

Other potentially useful URLs:

- https://sources.debian.net/src/freetype/2.10.4+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/freetype/2.10.4+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/freetype/2.10.4+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `fribidi=1.0.8-2`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.8-2.dsc' fribidi_1.0.8-2.dsc 1987 SHA256:f1b396620cda57e93799725abad47089902429295f7b3555bc3d5b3f00a79340
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA256:94c7b68d86ad2a9613b4dcffe7bbeb03523d63b5b37918bdf2e4ef34195c1e6c
'http://deb.debian.org/debian/pool/main/f/fribidi/fribidi_1.0.8-2.debian.tar.xz' fribidi_1.0.8-2.debian.tar.xz 8980 SHA256:898fc0b48625ce31e29d2f9501f17b9991b16b03816db6467faaedb85d22f00b
```

Other potentially useful URLs:

- https://sources.debian.net/src/fribidi/1.0.8-2/ (for browsing the source)
- https://sources.debian.net/src/fribidi/1.0.8-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/fribidi/1.0.8-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gcc-10=10.2.1-6`

Binary Packages:

- `cpp-10=10.2.1-6`
- `g++-10=10.2.1-6`
- `gcc-10=10.2.1-6`
- `gcc-10-base:amd64=10.2.1-6`
- `gfortran-10=10.2.1-6`
- `libasan6:amd64=10.2.1-6`
- `libatomic1:amd64=10.2.1-6`
- `libcc1-0:amd64=10.2.1-6`
- `libgcc-10-dev:amd64=10.2.1-6`
- `libgcc-s1:amd64=10.2.1-6`
- `libgfortran-10-dev:amd64=10.2.1-6`
- `libgfortran5:amd64=10.2.1-6`
- `libgomp1:amd64=10.2.1-6`
- `libitm1:amd64=10.2.1-6`
- `liblsan0:amd64=10.2.1-6`
- `libquadmath0:amd64=10.2.1-6`
- `libstdc++-10-dev:amd64=10.2.1-6`
- `libstdc++6:amd64=10.2.1-6`
- `libtsan0:amd64=10.2.1-6`
- `libubsan1:amd64=10.2.1-6`

Licenses: (parsed from: `/usr/share/doc/cpp-10/copyright`, `/usr/share/doc/g++-10/copyright`, `/usr/share/doc/gcc-10/copyright`, `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/gfortran-10/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-10-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgfortran-10-dev/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-10-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

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

### `dpkg` source package: `gcc-defaults=1.190`

Binary Packages:

- `cpp=4:10.2.1-1`
- `g++=4:10.2.1-1`
- `gcc=4:10.2.1-1`
- `gfortran=4:10.2.1-1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`, `/usr/share/doc/gfortran/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.190
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.190.dsc' gcc-defaults_1.190.dsc 12072 SHA256:ad953353a3d948dbbf2055aa2d1a2256e6845e7194eddbd939474387b0006a57
'http://deb.debian.org/debian/pool/main/g/gcc-defaults/gcc-defaults_1.190.tar.xz' gcc-defaults_1.190.tar.xz 45284 SHA256:4ce654e9469a9b2fa2d2168da6dd78ac338f7f86b0b68445e46ec2fbc92ece8f
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-defaults/1.190/ (for browsing the source)
- https://sources.debian.net/src/gcc-defaults/1.190/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-defaults/1.190/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `glib2.0=2.66.7-2`

Binary Packages:

- `libglib2.0-0:amd64=2.66.7-2`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.66.7-2
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.66.7-2.dsc' glib2.0_2.66.7-2.dsc 3386 SHA256:549f7f21ece26b3074cbb4560f37719d89c5356464a0f65cc18207b6de096793
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.66.7.orig.tar.xz' glib2.0_2.66.7.orig.tar.xz 4844892 SHA256:09f158769f6f26b31074e15b1ac80ec39b13b53102dfae66cfe826fb2cc65502
'http://deb.debian.org/debian/pool/main/g/glib2.0/glib2.0_2.66.7-2.debian.tar.xz' glib2.0_2.66.7-2.debian.tar.xz 101748 SHA256:c276bc7e31fbe0d3285faac4a4792dab4ab90ef953ba416adc33601c71355c53
```

Other potentially useful URLs:

- https://sources.debian.net/src/glib2.0/2.66.7-2/ (for browsing the source)
- https://sources.debian.net/src/glib2.0/2.66.7-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glib2.0/2.66.7-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.31-9`

Binary Packages:

- `libc-bin=2.31-9`
- `libc-dev-bin=2.31-9`
- `libc-l10n=2.31-9`
- `libc6:amd64=2.31-9`
- `libc6-dev:amd64=2.31-9`
- `locales=2.31-9`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc-l10n/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/locales/copyright`)

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

### `dpkg` source package: `gnupg2=2.2.27-1`

Binary Packages:

- `gpgv=2.2.27-1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.27-1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-1.dsc' gnupg2_2.2.27-1.dsc 3236 SHA256:d43af9a91d0392c2edcccea24dc0dd6e34b4bac65950f3c962c3b916a4cd9774
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2' gnupg2_2.2.27.orig.tar.bz2 7191555 SHA256:34e60009014ea16402069136e0a5f63d9b65f90096244975db5cea74b3d02399
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2.asc' gnupg2_2.2.27.orig.tar.bz2.asc 119 SHA256:2b44fd82da223cb629062b9c8840d92698c003be8531fc393c38f97b28cae2a4
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.27-1.debian.tar.xz' gnupg2_2.2.27-1.debian.tar.xz 62536 SHA256:668b77dc35cde0b65a6c18fab5620fca2c92208d0cc8298822c6eee56342e390
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.27-1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.27-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.27-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.0-7`

Binary Packages:

- `libgnutls30:amd64=3.7.0-7`

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
$ apt-get source -qq --print-uris gnutls28=3.7.0-7
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0-7.dsc' gnutls28_3.7.0-7.dsc 3480 SHA256:67657a677362cdbffcd9c1d138fd9b4011f46dac0be4f4230a4a84f0189e22b7
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0.orig.tar.xz' gnutls28_3.7.0.orig.tar.xz 6129176 SHA256:49e2a22691d252c9f24a9829b293a8f359095bc5a818351f05f1c0a5188a1df8
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0.orig.tar.xz.asc' gnutls28_3.7.0.orig.tar.xz.asc 854 SHA256:c530ea9141b0164c0842840483365c43f7defa3ceb765894f2ddd9751d8864a4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.0-7.debian.tar.xz' gnutls28_3.7.0-7.debian.tar.xz 74408 SHA256:8b4c8b2fd24f0eaf5549386bde5b0127e2e882bb2562949a5d925b37cc92b777
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.0-7/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.0-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.0-7/ (for access to the source package after it no longer exists in the archive)

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

- `libharfbuzz0b:amd64=2.7.4-1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

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

### `dpkg` source package: `icu=67.1-6`

Binary Packages:

- `icu-devtools=67.1-6`
- `libicu-dev:amd64=67.1-6`
- `libicu67:amd64=67.1-6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=67.1-6
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1-6.dsc' icu_67.1-6.dsc 2236 SHA256:873616004303ae242c9881fb777e132f819440ee83409ebd132ca5f606ff6bb7
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1.orig.tar.gz' icu_67.1.orig.tar.gz 24518055 SHA256:94a80cd6f251a53bd2a997f6f1b5ac6653fe791dfab66e1eb0227740fb86d5dc
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1.orig.tar.gz.asc' icu_67.1.orig.tar.gz.asc 833 SHA256:0044119f3df92ff3055dc3609f527fa1290177f6ef1b6650ea136698b245e537
'http://deb.debian.org/debian/pool/main/i/icu/icu_67.1-6.debian.tar.xz' icu_67.1-6.debian.tar.xz 29760 SHA256:9476daddae264b995009524b269555b6efcaaa679d651bb70869655929508d51
```

Other potentially useful URLs:

- https://sources.debian.net/src/icu/67.1-6/ (for browsing the source)
- https://sources.debian.net/src/icu/67.1-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/icu/67.1-6/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `isl=0.23-1`

Binary Packages:

- `libisl23:amd64=0.23-1`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.23-1
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.23-1.dsc' isl_0.23-1.dsc 1832 SHA256:6f5a221a8b33070141ca578078974ab35e963968d777b1d551293fded250ffab
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.23.orig.tar.xz' isl_0.23.orig.tar.xz 1729656 SHA256:5efc53efaef151301f4e7dde3856b66812d8153dede24fab17673f801c8698f2
'http://deb.debian.org/debian/pool/main/i/isl/isl_0.23-1.debian.tar.xz' isl_0.23-1.debian.tar.xz 26044 SHA256:97e9b10aca4b384241335c09b6928cf99f369fb64dfaa46b2a543e72a9d7dbe4
```

Other potentially useful URLs:

- https://sources.debian.net/src/isl/0.23-1/ (for browsing the source)
- https://sources.debian.net/src/isl/0.23-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/isl/0.23-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `kernsmooth=2.23-18-1`

Binary Packages:

- `r-cran-kernsmooth=2.23-18-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris kernsmooth=2.23-18-1
'http://deb.debian.org/debian/pool/main/k/kernsmooth/kernsmooth_2.23-18-1.dsc' kernsmooth_2.23-18-1.dsc 1891 SHA256:ff72c405cd3cf43893a56ccf90c050a77cbbe8c7fb442f2fa58147df477de785
'http://deb.debian.org/debian/pool/main/k/kernsmooth/kernsmooth_2.23-18.orig.tar.gz' kernsmooth_2.23-18.orig.tar.gz 25311 SHA256:8334800c5ad2305539d2731b929ea34f50fa4269ba87277b699fd5be5b03c490
'http://deb.debian.org/debian/pool/main/k/kernsmooth/kernsmooth_2.23-18-1.debian.tar.xz' kernsmooth_2.23-18-1.debian.tar.xz 3316 SHA256:aa60fd936e8d661658395f6b49f463052fef8a94f7b69c73deecbb928457416d
```

Other potentially useful URLs:

- https://sources.debian.net/src/kernsmooth/2.23-18-1/ (for browsing the source)
- https://sources.debian.net/src/kernsmooth/2.23-18-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/kernsmooth/2.23-18-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `krb5=1.18.3-4`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.18.3-4`
- `libk5crypto3:amd64=1.18.3-4`
- `libkrb5-3:amd64=1.18.3-4`
- `libkrb5support0:amd64=1.18.3-4`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.18.3-4
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3-4.dsc' krb5_1.18.3-4.dsc 3437 SHA256:3a400a053bb67ac5e52484a948a768b4d4efb082fa510438dd79b1dc0993ee56
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz' krb5_1.18.3.orig.tar.gz 8715312 SHA256:e61783c292b5efd9afb45c555a80dd267ac67eebabca42185362bee6c4fbd719
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz.asc' krb5_1.18.3.orig.tar.gz.asc 833 SHA256:ded19808ba7320ad0bb3ddfb5202845b2ff36a50613af7832f78dd3cb4437419
'http://deb.debian.org/debian/pool/main/k/krb5/krb5_1.18.3-4.debian.tar.xz' krb5_1.18.3-4.debian.tar.xz 103628 SHA256:69650fce52c8f3b301d9101913b6c9c4d32dee30da8861d8d2e4a07b76163f64
```

Other potentially useful URLs:

- https://sources.debian.net/src/krb5/1.18.3-4/ (for browsing the source)
- https://sources.debian.net/src/krb5/1.18.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/krb5/1.18.3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `lapack=3.9.0-3`

Binary Packages:

- `libblas-dev:amd64=3.9.0-3`
- `libblas3:amd64=3.9.0-3`
- `liblapack-dev:amd64=3.9.0-3`
- `liblapack3:amd64=3.9.0-3`

Licenses: (parsed from: `/usr/share/doc/libblas-dev/copyright`, `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack-dev/copyright`, `/usr/share/doc/liblapack3/copyright`)

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

### `dpkg` source package: `lattice=0.20-41-1`

Binary Packages:

- `r-cran-lattice=0.20-41-1+b1`

Licenses: (parsed from: `/usr/share/doc/r-cran-lattice/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris lattice=0.20-41-1
'http://deb.debian.org/debian/pool/main/l/lattice/lattice_0.20-41-1.dsc' lattice_0.20-41-1.dsc 1839 SHA256:350fd777f491e52711bdc595feb4cb2441d8e6ce5410c8a23f750aba5847aeb1
'http://deb.debian.org/debian/pool/main/l/lattice/lattice_0.20-41.orig.tar.gz' lattice_0.20-41.orig.tar.gz 389631 SHA256:54ca557f0cb33df60eb10b883c2ed2847e061ddd57ed9b5dd7695149609d57b5
'http://deb.debian.org/debian/pool/main/l/lattice/lattice_0.20-41-1.debian.tar.xz' lattice_0.20-41-1.debian.tar.xz 5164 SHA256:8b898302df33c6cb85139e2fcca345cd6ce1ca9b050a78d5c196e1fc60f8a46d
```

Other potentially useful URLs:

- https://sources.debian.net/src/lattice/0.20-41-1/ (for browsing the source)
- https://sources.debian.net/src/lattice/0.20-41-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/lattice/0.20-41-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `less=551-2`

Binary Packages:

- `less=551-2`

Licenses: (parsed from: `/usr/share/doc/less/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris less=551-2
'http://deb.debian.org/debian/pool/main/l/less/less_551-2.dsc' less_551-2.dsc 1631 SHA256:edfbd22cf51a2427e058deee33ea207612be67b81d9ec85093cda9f0ad49647d
'http://deb.debian.org/debian/pool/main/l/less/less_551.orig.tar.gz' less_551.orig.tar.gz 347007 SHA256:ff165275859381a63f19135a8f1f6c5a194d53ec3187f94121ecd8ef0795fe3d
'http://deb.debian.org/debian/pool/main/l/less/less_551-2.debian.tar.xz' less_551-2.debian.tar.xz 18812 SHA256:7e17dfdd154274e67b68a64d799f2115f6fdfa1557f829976a17b3bfde80b889
```

Other potentially useful URLs:

- https://sources.debian.net/src/less/551-2/ (for browsing the source)
- https://sources.debian.net/src/less/551-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/less/551-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libdatrie=0.2.13-1`

Binary Packages:

- `libdatrie1:amd64=0.2.13-1`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.13-1
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.13-1.dsc' libdatrie_0.2.13-1.dsc 2239 SHA256:a775d82ce3131d63c6dddca5df19ea8e72cd8941103239a66ec6902a12350783
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.13.orig.tar.xz' libdatrie_0.2.13.orig.tar.xz 314072 SHA256:12231bb2be2581a7f0fb9904092d24b0ed2a271a16835071ed97bed65267f4be
'http://deb.debian.org/debian/pool/main/libd/libdatrie/libdatrie_0.2.13-1.debian.tar.xz' libdatrie_0.2.13-1.debian.tar.xz 9404 SHA256:b77520311b09756f00bd2c4c1880d16a3ec424ca1454bfcc2da4efaa272df2fc
```

Other potentially useful URLs:

- https://sources.debian.net/src/libdatrie/0.2.13-1/ (for browsing the source)
- https://sources.debian.net/src/libdatrie/0.2.13-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libdatrie/0.2.13-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libgcrypt20=1.8.7-3`

Binary Packages:

- `libgcrypt20:amd64=1.8.7-3`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.7-3
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-3.dsc' libgcrypt20_1.8.7-3.dsc 2800 SHA256:0f02b93b8dd5f2b2d647c38b701f66b40fd2661113fcd472f1768c424af889fa
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2' libgcrypt20_1.8.7.orig.tar.bz2 2985660 SHA256:03b70f028299561b7034b8966d7dd77ef16ed139c43440925fe8782561974748
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2.asc' libgcrypt20_1.8.7.orig.tar.bz2.asc 228 SHA256:eed6bb4174433640a02c1dc8851f34f85ec55b43d76a24bec87d7175784ef614
'http://deb.debian.org/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-3.debian.tar.xz' libgcrypt20_1.8.7-3.debian.tar.xz 35056 SHA256:d3b7e134a69c15dd3d90a22d51c1a3c8c5eb254774777d4d997288dc2c9d8dc1
```

Other potentially useful URLs:

- https://sources.debian.net/src/libgcrypt20/1.8.7-3/ (for browsing the source)
- https://sources.debian.net/src/libgcrypt20/1.8.7-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libgcrypt20/1.8.7-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libjpeg-turbo=1:2.0.6-2`

Binary Packages:

- `libjpeg-dev:amd64=1:2.0.6-2`
- `libjpeg62-turbo:amd64=1:2.0.6-2`
- `libjpeg62-turbo-dev:amd64=1:2.0.6-2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3`
- `BSD-BY-LC-NE`
- `Expat`
- `NTP`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:2.0.6-2
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6-2.dsc' libjpeg-turbo_2.0.6-2.dsc 2577 SHA256:a1522b6d2e9b4897b2a226c00e11b881184d97c1704b11bc5e1eefabba145228
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6.orig.tar.gz' libjpeg-turbo_2.0.6.orig.tar.gz 2192315 SHA256:d74b92ac33b0e3657123ddcf6728788c90dc84dcb6a52013d758af3c4af481bb
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6.orig.tar.gz.asc' libjpeg-turbo_2.0.6.orig.tar.gz.asc 793 SHA256:ab2d95f62c2f25b39823c2b0ee3d72979786f5c310c19943a74eed8c2abc7b4b
'http://deb.debian.org/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6-2.debian.tar.xz' libjpeg-turbo_2.0.6-2.debian.tar.xz 99656 SHA256:fd66fbbee9582d95a2fcbb49c4474aa0ab37b28c3a12a4d72f6a341440af121b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libjpeg-turbo/1:2.0.6-2/ (for browsing the source)
- https://sources.debian.net/src/libjpeg-turbo/1:2.0.6-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libjpeg-turbo/1:2.0.6-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libnsl=1.3.0-2`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-2`
- `libnsl2:amd64=1.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libnsl-dev/copyright`, `/usr/share/doc/libnsl2/copyright`)

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

### `dpkg` source package: `libpaper=1.1.28`

Binary Packages:

- `libpaper-utils=1.1.28+b1`
- `libpaper1:amd64=1.1.28+b1`

Licenses: (parsed from: `/usr/share/doc/libpaper-utils/copyright`, `/usr/share/doc/libpaper1/copyright`)

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

### `dpkg` source package: `libpng1.6=1.6.37-3`

Binary Packages:

- `libpng-dev:amd64=1.6.37-3`
- `libpng16-16:amd64=1.6.37-3`

Licenses: (parsed from: `/usr/share/doc/libpng-dev/copyright`, `/usr/share/doc/libpng16-16/copyright`)

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

### `dpkg` source package: `libthai=0.1.28-4`

Binary Packages:

- `libthai-data=0.1.28-4`
- `libthai0:amd64=0.1.28-4`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.28-4
'http://http.debian.net/debian/pool/main/libt/libthai/libthai_0.1.28-4.dsc' libthai_0.1.28-4.dsc 2325 SHA256:59d0750d49afc6825b21bb58490bd79d474bb68752484060390f675afad3625f
'http://http.debian.net/debian/pool/main/libt/libthai/libthai_0.1.28.orig.tar.xz' libthai_0.1.28.orig.tar.xz 413592 SHA256:ffe0a17b4b5aa11b153c15986800eca19f6c93a4025ffa5cf2cab2dcdf1ae911
'http://http.debian.net/debian/pool/main/libt/libthai/libthai_0.1.28-4.debian.tar.xz' libthai_0.1.28-4.debian.tar.xz 12328 SHA256:ae60d4eb59bf571f198e02f58f0503077866d48a9f7e0a8d5ed5484a23b69cdc
```

### `dpkg` source package: `libtirpc=1.3.1-1`

Binary Packages:

- `libtirpc-common=1.3.1-1`
- `libtirpc-dev:amd64=1.3.1-1`
- `libtirpc3:amd64=1.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libtirpc-common/copyright`, `/usr/share/doc/libtirpc-dev/copyright`, `/usr/share/doc/libtirpc3/copyright`)

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

### `dpkg` source package: `libwebp=0.6.1-2`

Binary Packages:

- `libwebp6:amd64=0.6.1-2+b1`

Licenses: (parsed from: `/usr/share/doc/libwebp6/copyright`)

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

### `dpkg` source package: `libx11=2:1.7.0-2`

Binary Packages:

- `libx11-6:amd64=2:1.7.0-2`
- `libx11-data=2:1.7.0-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.7.0-2
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.0-2.dsc' libx11_1.7.0-2.dsc 2564 SHA256:1540dcbbbdf7e08405d133127ca6f63fe191a3946ae9c5afc95293bc12f784a1
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.0.orig.tar.gz' libx11_1.7.0.orig.tar.gz 3165477 SHA256:c48ec61785ec68fc6a9a6aca0a9578393414fe2562e3cc9cca30234345c7b6ac
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.0.orig.tar.gz.asc' libx11_1.7.0.orig.tar.gz.asc 833 SHA256:f84ea8a3a7c64ea045f8d115e2b0d14d3468e487f85f0084c0809f5c2d234c78
'http://deb.debian.org/debian/pool/main/libx/libx11/libx11_1.7.0-2.diff.gz' libx11_1.7.0-2.diff.gz 73844 SHA256:910d4a1527458ff020f0bab9df55bab44d63db8247543d2b2256c7b258ce439c
```

Other potentially useful URLs:

- https://sources.debian.net/src/libx11/2:1.7.0-2/ (for browsing the source)
- https://sources.debian.net/src/libx11/2:1.7.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libx11/2:1.7.0-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxcrypt=1:4.4.17-1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.17-1`
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

### `dpkg` source package: `libxmu=2:1.1.2-2`

Binary Packages:

- `libxmuu1:amd64=2:1.1.2-2+b3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxmu=2:1.1.2-2
'http://deb.debian.org/debian/pool/main/libx/libxmu/libxmu_1.1.2-2.dsc' libxmu_1.1.2-2.dsc 2291 SHA256:5e3333a3fe9dbed9d0df596d964b94aa1d45d56a0475a8b66b3f69d60ab29504
'http://deb.debian.org/debian/pool/main/libx/libxmu/libxmu_1.1.2.orig.tar.gz' libxmu_1.1.2.orig.tar.gz 469019 SHA256:e5fd4bacef068f9509b8226017205040e38d3fba8d2de55037200e7176c13dba
'http://deb.debian.org/debian/pool/main/libx/libxmu/libxmu_1.1.2-2.diff.gz' libxmu_1.1.2-2.diff.gz 6054 SHA256:c01cbd09a15e71c0418d2689a0fd0b946bf4e40d1dbe9f594beb00a4818f0740
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxmu/2:1.1.2-2/ (for browsing the source)
- https://sources.debian.net/src/libxmu/2:1.1.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxmu/2:1.1.2-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxt=1:1.2.0-1`

Binary Packages:

- `libxt6:amd64=1:1.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.0-1
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0-1.dsc' libxt_1.2.0-1.dsc 2298 SHA256:945650656e7f24f1276a1c100067e7fa728d50d7af93b4fcc149e5a5323df165
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz' libxt_1.2.0.orig.tar.gz 1016961 SHA256:d4bee88898fc5e1dc470e361430c72fbc529b9cdbbb6c0ed3affea3a39f97d8d
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz.asc' libxt_1.2.0.orig.tar.gz.asc 195 SHA256:4c5fe1bceef4aa507d5a95d2636e7ce257ee4f2b5522989ec4a7281cbe860564
'http://deb.debian.org/debian/pool/main/libx/libxt/libxt_1.2.0-1.diff.gz' libxt_1.2.0-1.diff.gz 31129 SHA256:eb723d0651e39c56d1e81fb7519e5093fd7e0177d42fd458d539163512076e52
```

Other potentially useful URLs:

- https://sources.debian.net/src/libxt/1:1.2.0-1/ (for browsing the source)
- https://sources.debian.net/src/libxt/1:1.2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libxt/1:1.2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libzstd=1.4.8+dfsg-2`

Binary Packages:

- `libzstd1:amd64=1.4.8+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libzstd/1.4.8+dfsg-2/


### `dpkg` source package: `linux=5.10.19-1`

Binary Packages:

- `linux-libc-dev:amd64=5.10.19-1`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `BSD-2-clause`
- `CRYPTOGAMS`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `Unicode-data`
- `X11`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=5.10.19-1
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.10.19-1.dsc' linux_5.10.19-1.dsc 195000 SHA256:ff0a1b9d1a4f9f0686f054d2f56b95e0df432ea7da0a2e15d4bd696d2309a427
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.10.19.orig.tar.xz' linux_5.10.19.orig.tar.xz 121470856 SHA256:6926ecf94f1902f3ae6259c078f65baa653335b662418935fc0e6ce7d046f718
'http://deb.debian.org/debian/pool/main/l/linux/linux_5.10.19-1.debian.tar.xz' linux_5.10.19-1.debian.tar.xz 1332548 SHA256:7c76ebc44c06e1c908086ce8168dff463733461fb46f1af5868b81660f99724c
```

Other potentially useful URLs:

- https://sources.debian.net/src/linux/5.10.19-1/ (for browsing the source)
- https://sources.debian.net/src/linux/5.10.19-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/linux/5.10.19-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `littler=0.3.12-1`

Binary Packages:

- `littler=0.3.12-1`
- `r-cran-littler=0.3.12-1`

Licenses: (parsed from: `/usr/share/doc/littler/copyright`, `/usr/share/doc/r-cran-littler/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris littler=0.3.12-1
'http://deb.debian.org/debian/pool/main/l/littler/littler_0.3.12-1.dsc' littler_0.3.12-1.dsc 1874 SHA256:de1dc5b56bbff3a6ee47dcc5126cd434a331bdf906348a25c707db9e653b1cfa
'http://deb.debian.org/debian/pool/main/l/littler/littler_0.3.12.orig.tar.gz' littler_0.3.12.orig.tar.gz 117849 SHA256:513983e5217b171c98af734d6cd525305014796537e87a36b329f2335dbfd7ef
'http://deb.debian.org/debian/pool/main/l/littler/littler_0.3.12-1.debian.tar.xz' littler_0.3.12-1.debian.tar.xz 6892 SHA256:4316fa067f36b24b6410737b3aa82cd20293d6ce27f0efd7a6d6688d9c2da6db
```

Other potentially useful URLs:

- https://sources.debian.net/src/littler/0.3.12-1/ (for browsing the source)
- https://sources.debian.net/src/littler/0.3.12-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/littler/0.3.12-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `make-dfsg=4.3-4`

Binary Packages:

- `make=4.3-4`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.3-4
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.3-4.dsc' make-dfsg_4.3-4.dsc 1657 SHA256:f647a112fa53ecb8707247741cb3aab4a0a6899fb466bdb4bbd44d30604168da
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA256:be4c17542578824e745f83bcd2a9ba264206187247cb6a5f5df99b0a9d1f9047
'http://deb.debian.org/debian/pool/main/m/make-dfsg/make-dfsg_4.3-4.diff.gz' make-dfsg_4.3-4.diff.gz 50880 SHA256:6f4196d2d8fe593e61a58cc885b6ea8ecf9b19d6a4e64bc9a32bb966f7d9a699
```

Other potentially useful URLs:

- https://sources.debian.net/src/make-dfsg/4.3-4/ (for browsing the source)
- https://sources.debian.net/src/make-dfsg/4.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/make-dfsg/4.3-4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `mgcv=1.8-34-1`

Binary Packages:

- `r-cran-mgcv=1.8-34-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-mgcv/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris mgcv=1.8-34-1
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-34-1.dsc' mgcv_1.8-34-1.dsc 1833 SHA256:582792a38891f3f38b3585dbf2cf9b3b3dbacbfc5ceda4a5a15a927e58bd5fbb
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-34.orig.tar.gz' mgcv_1.8-34.orig.tar.gz 1149538 SHA256:15b13af3b7d226d9835ba64551e0477d8323f85b6ebe721ab651f3b17af273de
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-34-1.debian.tar.xz' mgcv_1.8-34-1.debian.tar.xz 5304 SHA256:51f95305d46fced8cba796862b81368cddce79f403e85e00f1ce918bd179fdd2
```

Other potentially useful URLs:

- https://sources.debian.net/src/mgcv/1.8-34-1/ (for browsing the source)
- https://sources.debian.net/src/mgcv/1.8-34-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mgcv/1.8-34-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpclib3=1.2.0-1`

Binary Packages:

- `libmpc3:amd64=1.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.0-1
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.2.0-1.dsc' mpclib3_1.2.0-1.dsc 1851 SHA256:a1d1171fa4602a3b133e7d770f3fc12b417f7813125677be2ced102a41b6abce
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.2.0.orig.tar.gz' mpclib3_1.2.0.orig.tar.gz 840711 SHA256:e90f2d99553a9c19911abdb4305bf8217106a957e3994436428572c8dfe8fda6
'http://deb.debian.org/debian/pool/main/m/mpclib3/mpclib3_1.2.0-1.diff.gz' mpclib3_1.2.0-1.diff.gz 4281 SHA256:9c5e1cd47ac7b5470d3a8649511ff9a8a2f528eed49e99fa4c875ba242c61ec4
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpclib3/1.2.0-1/ (for browsing the source)
- https://sources.debian.net/src/mpclib3/1.2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpclib3/1.2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpfr4=4.1.0-3`

Binary Packages:

- `libmpfr6:amd64=4.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.1.0-3
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.1.0-3.dsc' mpfr4_4.1.0-3.dsc 1959 SHA256:6d2727cf53e788020f671a2cba644ff5dd4e28a2531e66c3ed32d98ce2b5bf4e
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA256:0c98a3f1732ff6ca4ea690552079da9c597872d30e96ec28414ee23c95558a7f
'http://deb.debian.org/debian/pool/main/m/mpfr4/mpfr4_4.1.0-3.debian.tar.xz' mpfr4_4.1.0-3.debian.tar.xz 12372 SHA256:b329dd24cba377ed4160c0819a5ec110e029fb52c93e9a141847d5ed2a2068e8
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpfr4/4.1.0-3/ (for browsing the source)
- https://sources.debian.net/src/mpfr4/4.1.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpfr4/4.1.0-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.2+20201114-2`

Binary Packages:

- `libncurses-dev:amd64=6.2+20201114-2`
- `libncurses5-dev:amd64=6.2+20201114-2`
- `libncurses6:amd64=6.2+20201114-2`
- `libncursesw6:amd64=6.2+20201114-2`
- `libtinfo6:amd64=6.2+20201114-2`
- `ncurses-base=6.2+20201114-2`
- `ncurses-bin=6.2+20201114-2`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

### `dpkg` source package: `nettle=3.7-2.1`

Binary Packages:

- `libhogweed6:amd64=3.7-2.1`
- `libnettle8:amd64=3.7-2.1`

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
$ apt-get source -qq --print-uris nettle=3.7-2.1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.7-2.1.dsc' nettle_3.7-2.1.dsc 2262 SHA256:13661e99da0ef9455e5c7a0716a93c2918349539e2681db232b8ca2b27409c87
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.7.orig.tar.gz' nettle_3.7.orig.tar.gz 2375067 SHA256:f001f64eb444bf13dd91bceccbc20acbc60c4311d6e2b20878452eb9a9cec75a
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.7.orig.tar.gz.asc' nettle_3.7.orig.tar.gz.asc 573 SHA256:1f5ed81582441eb4d953ef8666521ebc349f41f7dde5e11cb0845a2c049941b1
'http://deb.debian.org/debian/pool/main/n/nettle/nettle_3.7-2.1.debian.tar.xz' nettle_3.7-2.1.debian.tar.xz 30880 SHA256:343ab79dbe2907eb276b756ad6a90ba8775cf41b49b5cdffc149e142a9d269fb
```

Other potentially useful URLs:

- https://sources.debian.net/src/nettle/3.7-2.1/ (for browsing the source)
- https://sources.debian.net/src/nettle/3.7-2.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nettle/3.7-2.1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `nlme=3.1.152-1`

Binary Packages:

- `r-cran-nlme=3.1.152-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-nlme/copyright`)

- `GPL`
- `GPL `

Source:

```console
$ apt-get source -qq --print-uris nlme=3.1.152-1
'http://deb.debian.org/debian/pool/main/n/nlme/nlme_3.1.152-1.dsc' nlme_3.1.152-1.dsc 1840 SHA256:40ec4a814f6635fc20e8731a341d383e22f24b10e1e76b8643afc461d2a5e331
'http://deb.debian.org/debian/pool/main/n/nlme/nlme_3.1.152.orig.tar.gz' nlme_3.1.152.orig.tar.gz 805569 SHA256:5b65d1b1f121caf29e60341acf6d85e267fd94ed517748cf42d36359f74e515e
'http://deb.debian.org/debian/pool/main/n/nlme/nlme_3.1.152-1.debian.tar.xz' nlme_3.1.152-1.debian.tar.xz 7160 SHA256:19099d0abc092653c53e4c1c8cfd36f0abe978aaaa5259f9d0e32881a851b8e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/nlme/3.1.152-1/ (for browsing the source)
- https://sources.debian.net/src/nlme/3.1.152-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nlme/3.1.152-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openblas=0.3.13+ds-2`

Binary Packages:

- `libopenblas0-pthread:amd64=0.3.13+ds-2`

Licenses: (parsed from: `/usr/share/doc/libopenblas0-pthread/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-2-clause-texas`
- `BSD-3-clause`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openblas=0.3.13+ds-2
'http://deb.debian.org/debian/pool/main/o/openblas/openblas_0.3.13+ds-2.dsc' openblas_0.3.13+ds-2.dsc 5068 SHA256:54474aba3e2bb0f669fc95dd5860bee43395c7367c34774a4564b26dfbcde73f
'http://deb.debian.org/debian/pool/main/o/openblas/openblas_0.3.13+ds.orig.tar.xz' openblas_0.3.13+ds.orig.tar.xz 1694132 SHA256:4cc8fe4b324c1a051d06b9ebbaf1ac49a434c7ae7a193a72530e7b41b98ad11c
'http://deb.debian.org/debian/pool/main/o/openblas/openblas_0.3.13+ds-2.debian.tar.xz' openblas_0.3.13+ds-2.debian.tar.xz 22972 SHA256:df16d90b12fce62f9e0b90a7fa88c9748d255f4eef8ca21c2225c20437f56427
```

Other potentially useful URLs:

- https://sources.debian.net/src/openblas/0.3.13+ds-2/ (for browsing the source)
- https://sources.debian.net/src/openblas/0.3.13+ds-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openblas/0.3.13+ds-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openldap=2.4.57+dfsg-2`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.57+dfsg-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.57+dfsg-2
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.57+dfsg-2.dsc' openldap_2.4.57+dfsg-2.dsc 3061 SHA256:1fcfd2ce54964068ddf36b64727c99d767e73f7520d6525a286f8e3564821971
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.57+dfsg.orig.tar.gz' openldap_2.4.57+dfsg.orig.tar.gz 5054318 SHA256:009cc88733eaf41a21607e073a19bce53d7d6ed90a5c280e80880978c4e91db7
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.4.57+dfsg-2.debian.tar.xz' openldap_2.4.57+dfsg-2.debian.tar.xz 168496 SHA256:e1ca889e9e7a6ea2eb8adde95119df4a08199c10bd772263989138e85171cc62
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.4.57+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.4.57+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.4.57+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=1.1.1j-1`

Binary Packages:

- `libssl1.1:amd64=1.1.1j-1`
- `openssl=1.1.1j-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1j-1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1j-1.dsc' openssl_1.1.1j-1.dsc 2446 SHA256:6b5054e975a3515acbf6cabf8da4647992156add5091e805a42df13df0d96bbc
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1j.orig.tar.gz' openssl_1.1.1j.orig.tar.gz 9823161 SHA256:aaf2fcb575cdf6491b98ab4829abf78a3dec8402b8b81efc8f23c00d443981bf
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1j.orig.tar.gz.asc' openssl_1.1.1j.orig.tar.gz.asc 488 SHA256:02571ae2fb2de5a1bc613106caabb1c4007b5268312aba221ed873c365fd9c99
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_1.1.1j-1.debian.tar.xz' openssl_1.1.1j-1.debian.tar.xz 84524 SHA256:b3abac4c4bc7e67d961dc86b2d5b59187f47c534402d7bca9286a3ba411d0e3e
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/1.1.1j-1/ (for browsing the source)
- https://sources.debian.net/src/openssl/1.1.1j-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/1.1.1j-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `pam=1.4.0-6`

Binary Packages:

- `libpam-modules:amd64=1.4.0-6`
- `libpam-modules-bin=1.4.0-6`
- `libpam-runtime=1.4.0-6`
- `libpam0g:amd64=1.4.0-6`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.4.0-6
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-6.dsc' pam_1.4.0-6.dsc 2169 SHA256:1147a787ce8b65676ebe0037d66eb21c71436d5c8db41d2d69456e9fea7031a3
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0.orig.tar.xz' pam_1.4.0.orig.tar.xz 988908 SHA256:cd6d928c51e64139be3bdb38692c68183a509b83d4f2c221024ccd4bcddfd034
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.4.0-6.debian.tar.xz' pam_1.4.0-6.debian.tar.xz 115628 SHA256:01555c413669922d03eab697f4a24c81f512f4afb65a0008b9fff4018d4799b5
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.4.0-6/ (for browsing the source)
- https://sources.debian.net/src/pam/1.4.0-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.4.0-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pango1.0=1.46.2-3`

Binary Packages:

- `libpango-1.0-0:amd64=1.46.2-3`
- `libpangocairo-1.0-0:amd64=1.46.2-3`
- `libpangoft2-1.0-0:amd64=1.46.2-3`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Chromium-BSD-style`
- `Example`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.46.2-3
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.46.2-3.dsc' pango1.0_1.46.2-3.dsc 3542 SHA256:bfa040cfe6ac73d4452902b682dead39e6bd057da73b5432912bb50a5336ba8a
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.46.2.orig.tar.xz' pango1.0_1.46.2.orig.tar.xz 535108 SHA256:d89fab5f26767261b493279b65cfb9eb0955cd44c07c5628d36094609fc51841
'http://deb.debian.org/debian/pool/main/p/pango1.0/pango1.0_1.46.2-3.debian.tar.xz' pango1.0_1.46.2-3.debian.tar.xz 38956 SHA256:34e19749e45cba527a0c7f7faf5f118606a6bd85121ef58fe66d87e0e6c9a312
```

Other potentially useful URLs:

- https://sources.debian.net/src/pango1.0/1.46.2-3/ (for browsing the source)
- https://sources.debian.net/src/pango1.0/1.46.2-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pango1.0/1.46.2-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `patch=2.7.6-7`

Binary Packages:

- `patch=2.7.6-7`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-7
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-7.dsc' patch_2.7.6-7.dsc 1706 SHA256:d954fd576d935ac54b7d44d4976eb52d0da84a57f7bad90c6e5bd5e33595030a
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://deb.debian.org/debian/pool/main/p/patch/patch_2.7.6-7.debian.tar.xz' patch_2.7.6-7.debian.tar.xz 15084 SHA256:7725f30b042d8cf63516e480036e93ca2ff0ce5ad3754db4a4e69d33e96a2624
```

Other potentially useful URLs:

- https://sources.debian.net/src/patch/2.7.6-7/ (for browsing the source)
- https://sources.debian.net/src/patch/2.7.6-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/patch/2.7.6-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.36-2`

Binary Packages:

- `libpcre2-16-0:amd64=10.36-2`
- `libpcre2-32-0:amd64=10.36-2`
- `libpcre2-8-0:amd64=10.36-2`
- `libpcre2-dev:amd64=10.36-2`
- `libpcre2-posix2:amd64=10.36-2`

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

- `libpcre16-3:amd64=2:8.39-13`
- `libpcre3:amd64=2:8.39-13`
- `libpcre3-dev:amd64=2:8.39-13`
- `libpcre32-3:amd64=2:8.39-13`
- `libpcrecpp0v5:amd64=2:8.39-13`

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

### `dpkg` source package: `perl=5.32.1-3`

Binary Packages:

- `libperl5.32:amd64=5.32.1-3`
- `perl=5.32.1-3`
- `perl-base=5.32.1-3`
- `perl-modules-5.32=5.32.1-3`

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
$ apt-get source -qq --print-uris perl=5.32.1-3
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1-3.dsc' perl_5.32.1-3.dsc 2886 SHA256:1e4a48b1ad467a853b14f43c44ff7b969d5e590c01cea2d0b2d6374cedaaf50f
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1.orig-regen-configure.tar.gz' perl_5.32.1.orig-regen-configure.tar.gz 871331 SHA256:1d179b41283f12ad83f9758430f6ddc49bdf20db5c396aeae7e51ebb4e4afd29
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1.orig.tar.xz' perl_5.32.1.orig.tar.xz 12610988 SHA256:57cc47c735c8300a8ce2fa0643507b44c4ae59012bfdad0121313db639e02309
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.32.1-3.debian.tar.xz' perl_5.32.1-3.debian.tar.xz 164680 SHA256:1e6f590e5d438f9e5fea962bdb9be7ba1206c32f3c56c88ed19385a7f252fb8d
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.32.1-3/ (for browsing the source)
- https://sources.debian.net/src/perl/5.32.1-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.32.1-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `pkg-config=0.29.2-1`

Binary Packages:

- `pkg-config=0.29.2-1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.2-1
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.2-1.dsc' pkg-config_0.29.2-1.dsc 1771 SHA256:e4feeda94c3882e2aca55eab907900508a2e35111f927a79076154870f8fe373
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.2.orig.tar.gz' pkg-config_0.29.2.orig.tar.gz 2016830 SHA256:6fc69c01688c9458a57eb9a1664c9aba372ccda420a02bf4429fe610e7e7d591
'http://deb.debian.org/debian/pool/main/p/pkg-config/pkg-config_0.29.2-1.diff.gz' pkg-config_0.29.2-1.diff.gz 9202 SHA256:6ecdd3463718e8922b53fca8d2fd37db4ba178f078b5e3ccd38c1a6efffb94ad
```

Other potentially useful URLs:

- https://sources.debian.net/src/pkg-config/0.29.2-1/ (for browsing the source)
- https://sources.debian.net/src/pkg-config/0.29.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pkg-config/0.29.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-base=4.0.4-1`

Binary Packages:

- `r-base=4.0.4-1`
- `r-base-core=4.0.4-1`
- `r-base-dev=4.0.4-1`
- `r-recommended=4.0.4-1`

Licenses: (parsed from: `/usr/share/doc/r-base/copyright`, `/usr/share/doc/r-base-core/copyright`, `/usr/share/doc/r-base-dev/copyright`, `/usr/share/doc/r-recommended/copyright`)

- `Artistic`
- `GPL-2`
- `GPL-3`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-base=4.0.4-1
'http://deb.debian.org/debian/pool/main/r/r-base/r-base_4.0.4-1.dsc' r-base_4.0.4-1.dsc 3019 SHA256:28d1a991b23cd94a10335c8245a21ffc1a82617c7ecbd9e17bc4ffeb54c9fe71
'http://deb.debian.org/debian/pool/main/r/r-base/r-base_4.0.4.orig.tar.gz' r-base_4.0.4.orig.tar.gz 33687611 SHA256:523f27d69744a08c8f0bd5e1e6c3d89a4db29ed983388ba70963a3cd3a4a802e
'http://deb.debian.org/debian/pool/main/r/r-base/r-base_4.0.4-1.debian.tar.xz' r-base_4.0.4-1.debian.tar.xz 97360 SHA256:de97e6ecc4c7141719918fe23425ee52862739a5997d94d5fe93280070412678
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-base/4.0.4-1/ (for browsing the source)
- https://sources.debian.net/src/r-base/4.0.4-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-base/4.0.4-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-class=7.3-18-1`

Binary Packages:

- `r-cran-class=7.3-18-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-class/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-class=7.3-18-1
'http://deb.debian.org/debian/pool/main/r/r-cran-class/r-cran-class_7.3-18-1.dsc' r-cran-class_7.3-18-1.dsc 1873 SHA256:c5721314e49c85613b7017c360d0109f3172db63333507d5b282fc185b9a2944
'http://deb.debian.org/debian/pool/main/r/r-cran-class/r-cran-class_7.3-18.orig.tar.gz' r-cran-class_7.3-18.orig.tar.gz 20780 SHA256:d2ba722e6a898b4b8145f87c132f7d205a2ec54de7f17a9fe7669232e6211391
'http://deb.debian.org/debian/pool/main/r/r-cran-class/r-cran-class_7.3-18-1.debian.tar.xz' r-cran-class_7.3-18-1.debian.tar.xz 3120 SHA256:8f062d0ebf246a3b9f3a17ac02b95ae3a64add252b2a1610cee9b002ea2ebfe1
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-class/7.3-18-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-class/7.3-18-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-class/7.3-18-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-mass=7.3-53.1-1`

Binary Packages:

- `r-cran-mass=7.3-53.1-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-mass/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-mass=7.3-53.1-1
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-53.1-1.dsc' r-cran-mass_7.3-53.1-1.dsc 1865 SHA256:757a78d569a3d7f8a6cc0c7193fd0cf2acec8688b70ebaa23104944bc5786091
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-53.1.orig.tar.gz' r-cran-mass_7.3-53.1.orig.tar.gz 505007 SHA256:e45b1eb97ee32db9a3a211ce42b972094827d93ef2f48bda653c121f08314465
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-53.1-1.debian.tar.xz' r-cran-mass_7.3-53.1-1.debian.tar.xz 6300 SHA256:f45fcb1952d3d5bca99078e1d96568056dbae0c0957f7d7155201dda9ac8ebc5
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-mass/7.3-53.1-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-mass/7.3-53.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-mass/7.3-53.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-nnet=7.3-15-1`

Binary Packages:

- `r-cran-nnet=7.3-15-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-nnet/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-nnet=7.3-15-1
'http://deb.debian.org/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-15-1.dsc' r-cran-nnet_7.3-15-1.dsc 1848 SHA256:ced28d3a199d4793c757b0ed027de494928f968a7aea4904a6c6480043c436ce
'http://deb.debian.org/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-15.orig.tar.gz' r-cran-nnet_7.3-15.orig.tar.gz 29173 SHA256:ace9ed4542e858ccec632062a4c65b8b2ffef367f118a1c97c2917137aed1e19
'http://deb.debian.org/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-15-1.debian.tar.xz' r-cran-nnet_7.3-15-1.debian.tar.xz 3152 SHA256:14a018e1a589d2a4544eb1700208027fc43fb948f18358be2921c33415a97926
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-nnet/7.3-15-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-nnet/7.3-15-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-nnet/7.3-15-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-spatial=7.3-13-1`

Binary Packages:

- `r-cran-spatial=7.3-13-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-spatial/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-spatial=7.3-13-1
'http://deb.debian.org/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-13-1.dsc' r-cran-spatial_7.3-13-1.dsc 1884 SHA256:4e7dd73f203a9ffcdac8655642aae64b31b7c64497f9f6bdcc40ee65107e72fe
'http://deb.debian.org/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-13.orig.tar.gz' r-cran-spatial_7.3-13.orig.tar.gz 44645 SHA256:c47033b41395f7ca91c5a5ad449c7400acf48d7ac4d6fabd582fb4273c523832
'http://deb.debian.org/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-13-1.debian.tar.xz' r-cran-spatial_7.3-13-1.debian.tar.xz 3072 SHA256:63129468fe64f6ed141f7675ffe8ca0a8ee23927bae53b035feb359d09b47432
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-spatial/7.3-13-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-spatial/7.3-13-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-spatial/7.3-13-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.1-1`

Binary Packages:

- `libreadline-dev:amd64=8.1-1`
- `libreadline8:amd64=8.1-1`
- `readline-common=8.1-1`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

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

### `dpkg` source package: `rmatrix=1.3-2-1`

Binary Packages:

- `r-cran-matrix=1.3-2-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-matrix/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rmatrix=1.3-2-1
'http://deb.debian.org/debian/pool/main/r/rmatrix/rmatrix_1.3-2-1.dsc' rmatrix_1.3-2-1.dsc 1860 SHA256:89b8a4dbfce00c3437b9bd01881cf2c6f6cf62b62621fa8a6975d7aa32661864
'http://deb.debian.org/debian/pool/main/r/rmatrix/rmatrix_1.3-2.orig.tar.gz' rmatrix_1.3-2.orig.tar.gz 1974981 SHA256:950ba5d91018e711fd2743b3486a50dc47ae9c271389fce587792f0a9aab9531
'http://deb.debian.org/debian/pool/main/r/rmatrix/rmatrix_1.3-2-1.debian.tar.xz' rmatrix_1.3-2-1.debian.tar.xz 5564 SHA256:171a466dac0d7ee1d56d0ca7cb26bea7dd021ef2b1ce48060a34b8376859c3ca
```

Other potentially useful URLs:

- https://sources.debian.net/src/rmatrix/1.3-2-1/ (for browsing the source)
- https://sources.debian.net/src/rmatrix/1.3-2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rmatrix/1.3-2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rpart=4.1-15-2`

Binary Packages:

- `r-cran-rpart=4.1-15-2+b1`

Licenses: (parsed from: `/usr/share/doc/r-cran-rpart/copyright`)

- `GPL-2`
- `GPL-2 | license included below`

Source:

```console
$ apt-get source -qq --print-uris rpart=4.1-15-2
'http://deb.debian.org/debian/pool/main/r/rpart/rpart_4.1-15-2.dsc' rpart_4.1-15-2.dsc 1840 SHA256:016d8219c9998d8d2fa59c81a40a5ee81e2bff63a8180f256c02548f06820a51
'http://deb.debian.org/debian/pool/main/r/rpart/rpart_4.1-15.orig.tar.gz' rpart_4.1-15.orig.tar.gz 639286 SHA256:2b8ebe0e9e11592debff893f93f5a44a6765abd0bd956b0eb1f70e9394cfae5c
'http://deb.debian.org/debian/pool/main/r/rpart/rpart_4.1-15-2.debian.tar.xz' rpart_4.1-15-2.debian.tar.xz 4336 SHA256:e708011ab48126ea1829d8e6a005cee44edf1b09a4129f71ed2051f6e673e9f8
```

Other potentially useful URLs:

- https://sources.debian.net/src/rpart/4.1-15-2/ (for browsing the source)
- https://sources.debian.net/src/rpart/4.1-15-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rpart/4.1-15-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2+b2`

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

### `dpkg` source package: `survival=3.2-7-1`

Binary Packages:

- `r-cran-survival=3.2-7-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-survival/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris survival=3.2-7-1
'http://deb.debian.org/debian/pool/main/s/survival/survival_3.2-7-1.dsc' survival_3.2-7-1.dsc 1861 SHA256:24db9d6acca440aedd490ec70253fcae6b798ee2ef2362390cee7e8de815c9f1
'http://deb.debian.org/debian/pool/main/s/survival/survival_3.2-7.orig.tar.gz' survival_3.2-7.orig.tar.gz 7657362 SHA256:5356cd73da7ecfda4042e8a8ae00d3531b106f7b39ca31a1843eadf288418a46
'http://deb.debian.org/debian/pool/main/s/survival/survival_3.2-7-1.debian.tar.xz' survival_3.2-7-1.debian.tar.xz 6020 SHA256:1adcbad93930afd120cdeafc6424706d8cedd98a08493ccfd8d118f1b6f87d1f
```

Other potentially useful URLs:

- https://sources.debian.net/src/survival/3.2-7-1/ (for browsing the source)
- https://sources.debian.net/src/survival/3.2-7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/survival/3.2-7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=247.3-1`

Binary Packages:

- `libsystemd0:amd64=247.3-1`
- `libudev1:amd64=247.3-1`

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
$ apt-get source -qq --print-uris systemd=247.3-1
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.3-1.dsc' systemd_247.3-1.dsc 5167 SHA256:6cb274436b236ebfdde4e588da296e918ab590a1dac19847a05743b3cf9cc79f
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.3.orig.tar.gz' systemd_247.3.orig.tar.gz 9895385 SHA256:2869986e219a8dfc96cc0dffac66e0c13bb70a89e16b85a3948876c146cfa3e0
'http://deb.debian.org/debian/pool/main/s/systemd/systemd_247.3-1.debian.tar.xz' systemd_247.3-1.debian.tar.xz 159632 SHA256:171fd135dbb67b70144b24ace49f8cf745f5f65c6b0e562ab4e9b6e21a3aad93
```

Other potentially useful URLs:

- https://sources.debian.net/src/systemd/247.3-1/ (for browsing the source)
- https://sources.debian.net/src/systemd/247.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/systemd/247.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `sysvinit=2.96-6`

Binary Packages:

- `sysvinit-utils=2.96-6`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-6
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-6.dsc' sysvinit_2.96-6.dsc 2601 SHA256:74e62d4b46648432678777dfacbbb752b5bc1e4cab565cbdc93d2e09c6664989
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA256:2a2e26b72aa235a23ab1c8471005f890309ce1196c83fbc9413c57b9ab62b587
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA256:dfc184b95da12c8c888c8ae6b0f26fe8a23b07fbcdd240f6600a8a78b9439fa0
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_2.96-6.debian.tar.xz' sysvinit_2.96-6.debian.tar.xz 128800 SHA256:cd9f9aa8d35b3fa80a9a8fa9c197cf5a11c31367a7675ae97c71828964ec3f11
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/2.96-6/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/2.96-6/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/2.96-6/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tar=1.34+dfsg-1`

Binary Packages:

- `tar=1.34+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34+dfsg-1.dsc' tar_1.34+dfsg-1.dsc 2015 SHA256:12d709cd77e38e5d1753325a9f266b340b5c095a426f438c677b42c031949d89
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34+dfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA256:7d57029540cb928394defb3b377b3531237c947e795b51aa8acac0c5ba0e4844
'http://deb.debian.org/debian/pool/main/t/tar/tar_1.34+dfsg-1.debian.tar.xz' tar_1.34+dfsg-1.debian.tar.xz 19192 SHA256:7228f5cbd36f937dfc1fec042dee8b3e02d92a06afdd44c586c2c8cfb1905538
```

Other potentially useful URLs:

- https://sources.debian.net/src/tar/1.34+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/tar/1.34+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tar/1.34+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tcl8.6=8.6.11+dfsg-1`

Binary Packages:

- `libtcl8.6:amd64=8.6.11+dfsg-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcl8.6=8.6.11+dfsg-1
'http://deb.debian.org/debian/pool/main/t/tcl8.6/tcl8.6_8.6.11+dfsg-1.dsc' tcl8.6_8.6.11+dfsg-1.dsc 2118 SHA256:a1f144a7d92dd13cf78b1001993bc3096f2f5d66072a6c9e7e800a5239491f5b
'http://deb.debian.org/debian/pool/main/t/tcl8.6/tcl8.6_8.6.11+dfsg.orig.tar.gz' tcl8.6_8.6.11+dfsg.orig.tar.gz 6054310 SHA256:10bb25d492f19acb5d00bb24069b0fadd78abad1d5294e5dde141af9fc0693ce
'http://deb.debian.org/debian/pool/main/t/tcl8.6/tcl8.6_8.6.11+dfsg-1.debian.tar.xz' tcl8.6_8.6.11+dfsg-1.debian.tar.xz 14356 SHA256:3cc78ffb13cead08aabe2afc4c86f90599cde37a68dc6f64460e597ea272e959
```

Other potentially useful URLs:

- https://sources.debian.net/src/tcl8.6/8.6.11+dfsg-1/ (for browsing the source)
- https://sources.debian.net/src/tcl8.6/8.6.11+dfsg-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tcl8.6/8.6.11+dfsg-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tex-gyre=20180621-3.1`

Binary Packages:

- `fonts-texgyre=20180621-3.1`

Licenses: (parsed from: `/usr/share/doc/fonts-texgyre/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris tex-gyre=20180621-3.1
'http://deb.debian.org/debian/pool/main/t/tex-gyre/tex-gyre_20180621-3.1.dsc' tex-gyre_20180621-3.1.dsc 2039 SHA256:d34500d573c01e0b608817b902f19c36880b7f833e91b36e20e99a0c4b2b1063
'http://deb.debian.org/debian/pool/main/t/tex-gyre/tex-gyre_20180621.orig.tar.gz' tex-gyre_20180621.orig.tar.gz 24033627 SHA256:fe6b0f8ca6890d4a369f36c3b45bc30470069701a2f59042178ad5933fc9cdb8
'http://deb.debian.org/debian/pool/main/t/tex-gyre/tex-gyre_20180621-3.1.debian.tar.xz' tex-gyre_20180621-3.1.debian.tar.xz 11096 SHA256:52d232bef3d92ad68589904ce906fbe0520c551ebc1ac07a6d1dd4c6694b048a
```

Other potentially useful URLs:

- https://sources.debian.net/src/tex-gyre/20180621-3.1/ (for browsing the source)
- https://sources.debian.net/src/tex-gyre/20180621-3.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tex-gyre/20180621-3.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tiff=4.2.0-1`

Binary Packages:

- `libtiff5:amd64=4.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.2.0-1
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.2.0-1.dsc' tiff_4.2.0-1.dsc 2429 SHA256:53bf09435e02efe3c743d9182ec084553778227af79ac912e42bf660fcf98b25
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.2.0.orig.tar.gz' tiff_4.2.0.orig.tar.gz 2809373 SHA256:eb0484e568ead8fa23b513e9b0041df7e327f4ee2d22db5a533929dfc19633cb
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.2.0.orig.tar.gz.asc' tiff_4.2.0.orig.tar.gz.asc 228 SHA256:119bb62934603ff4d3cd81c739d11904b28812a860773b9b2268cc96a339b14f
'http://deb.debian.org/debian/pool/main/t/tiff/tiff_4.2.0-1.debian.tar.xz' tiff_4.2.0-1.debian.tar.xz 19528 SHA256:8399f266e95aeb9bb4930790868651562ecdad7333cb71983691a105659ab2a1
```

Other potentially useful URLs:

- https://sources.debian.net/src/tiff/4.2.0-1/ (for browsing the source)
- https://sources.debian.net/src/tiff/4.2.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tiff/4.2.0-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tk8.6=8.6.11-2`

Binary Packages:

- `libtk8.6:amd64=8.6.11-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tk8.6=8.6.11-2
'http://deb.debian.org/debian/pool/main/t/tk8.6/tk8.6_8.6.11-2.dsc' tk8.6_8.6.11-2.dsc 2153 SHA256:d5f272e721d806da279ad17f61e09fb7cb10bbc6cc2b0f5352f676837cbed2d4
'http://deb.debian.org/debian/pool/main/t/tk8.6/tk8.6_8.6.11.orig.tar.gz' tk8.6_8.6.11.orig.tar.gz 4496914 SHA256:5228a8187a7f70fa0791ef0f975270f068ba9557f57456f51eb02d9d4ea31282
'http://deb.debian.org/debian/pool/main/t/tk8.6/tk8.6_8.6.11-2.debian.tar.xz' tk8.6_8.6.11-2.debian.tar.xz 10676 SHA256:aac79d6c6ef4118f5262503941174e7f9abb4e22ad3064ce28bdf33eea2f4036
```

Other potentially useful URLs:

- https://sources.debian.net/src/tk8.6/8.6.11-2/ (for browsing the source)
- https://sources.debian.net/src/tk8.6/8.6.11-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tk8.6/8.6.11-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `tzdata=2021a-1`

Binary Packages:

- `tzdata=2021a-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2021a-1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a-1.dsc' tzdata_2021a-1.dsc 2237 SHA256:91419e04006db0b9024ed1d5339cd161df2535b57bad0b13b6eafe77804fe40a
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a.orig.tar.gz' tzdata_2021a.orig.tar.gz 411892 SHA256:39e7d2ba08c68cbaefc8de3227aab0dec2521be8042cf56855f7dc3a9fb14e08
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a.orig.tar.gz.asc' tzdata_2021a.orig.tar.gz.asc 833 SHA256:9dc5f54674166f4ffbc2d4485e656227430ab5f39c9006e6ed9986281117f058
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2021a-1.debian.tar.xz' tzdata_2021a-1.debian.tar.xz 105188 SHA256:8c27130ee8c22415f0839198e3b51f61148aff84c462723f2464c1faee908fcf
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2021a-1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2021a-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2021a-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `util-linux=2.36.1-7`

Binary Packages:

- `bsdutils=1:2.36.1-7`
- `libblkid1:amd64=2.36.1-7`
- `libmount1:amd64=2.36.1-7`
- `libsmartcols1:amd64=2.36.1-7`
- `libuuid1:amd64=2.36.1-7`
- `mount=2.36.1-7`
- `util-linux=2.36.1-7`

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
$ apt-get source -qq --print-uris util-linux=2.36.1-7
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.36.1-7.dsc' util-linux_2.36.1-7.dsc 4271 SHA256:659947b09a7c95769e3ac28fed878f8dc73d9655c7386837f3b4fb31f9c382d5
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.36.1.orig.tar.xz' util-linux_2.36.1.orig.tar.xz 5231880 SHA256:09fac242172cd8ec27f0739d8d192402c69417617091d8c6e974841568f37eed
'http://deb.debian.org/debian/pool/main/u/util-linux/util-linux_2.36.1-7.debian.tar.xz' util-linux_2.36.1-7.debian.tar.xz 98140 SHA256:85def546377248a05e8af87482458ae6a39f081e626d3752c567e87de8dca24e
```

Other potentially useful URLs:

- https://sources.debian.net/src/util-linux/2.36.1-7/ (for browsing the source)
- https://sources.debian.net/src/util-linux/2.36.1-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/util-linux/2.36.1-7/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `vim=2:8.2.2434-3`

Binary Packages:

- `vim-common=2:8.2.2434-3`
- `vim-tiny=2:8.2.2434-3`
- `xxd=2:8.2.2434-3`

Licenses: (parsed from: `/usr/share/doc/vim-common/copyright`, `/usr/share/doc/vim-tiny/copyright`, `/usr/share/doc/xxd/copyright`)

- `Apache`
- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-2-clause`
- `BSD-3-clause`
- `Compaq`
- `EDL-1`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `OPL-1+`
- `SRA`
- `UC`
- `Vim`
- `Vim-Regexp`
- `X11`
- `XPM`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris vim=2:8.2.2434-3
'http://deb.debian.org/debian/pool/main/v/vim/vim_8.2.2434-3.dsc' vim_8.2.2434-3.dsc 3023 SHA256:f9d2b42a24dda4da947a3d0db9400baf45a1004a8766e7f2f8285334c42e59ce
'http://deb.debian.org/debian/pool/main/v/vim/vim_8.2.2434.orig.tar.gz' vim_8.2.2434.orig.tar.gz 15412030 SHA256:dec2f91bb4f877b2bfdf283ccc3d94f99f436a225bd8a9b5e3d422f95c56d702
'http://deb.debian.org/debian/pool/main/v/vim/vim_8.2.2434-3.debian.tar.xz' vim_8.2.2434-3.debian.tar.xz 197368 SHA256:7ef821f110cbb94d9b28a6899a9a34b83a8b5217d5357e76e4af577d5ffcdad6
```

Other potentially useful URLs:

- https://sources.debian.net/src/vim/2:8.2.2434-3/ (for browsing the source)
- https://sources.debian.net/src/vim/2:8.2.2434-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/vim/2:8.2.2434-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `wget=1.21-1`

Binary Packages:

- `wget=1.21-1+b1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21-1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21-1.dsc' wget_1.21-1.dsc 2147 SHA256:0f643c806036d3ed7367b4ac5333c3c6b30071786ae60d548db630c498e2789e
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.orig.tar.gz' wget_1.21.orig.tar.gz 4866788 SHA256:b3bc1a9bd0c19836c9709c318d41c19c11215a07514f49f89b40b9d50ab49325
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.orig.tar.gz.asc' wget_1.21.orig.tar.gz.asc 854 SHA256:da3a99b8a7bbaf70cc339593a9e0c2942dd673152bc7bfcf8f965ae1c06d50df
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21-1.debian.tar.xz' wget_1.21-1.debian.tar.xz 60528 SHA256:efacd406cd2bca442e377d130195a36e72d9723932c2bdc69748d80acc21dbcd
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.21-1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.21-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.21-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xauth=1:1.1-1`

Binary Packages:

- `xauth=1:1.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xauth=1:1.1-1
'http://deb.debian.org/debian/pool/main/x/xauth/xauth_1.1-1.dsc' xauth_1.1-1.dsc 1878 SHA256:59f36197de42b36757aa37b142e187181ea49e7765c5f16a3e00f4576694d49d
'http://deb.debian.org/debian/pool/main/x/xauth/xauth_1.1.orig.tar.gz' xauth_1.1.orig.tar.gz 204146 SHA256:e9fce796c8c5c9368594b9e8bbba237fb54b6615f5fd60e8d0a5b3c52a92c5ef
'http://deb.debian.org/debian/pool/main/x/xauth/xauth_1.1-1.diff.gz' xauth_1.1-1.diff.gz 13752 SHA256:80f52f736ca3d5b5e79ccee802a271e16f4421748ab985709541cb77e965bf24
```

Other potentially useful URLs:

- https://sources.debian.net/src/xauth/1:1.1-1/ (for browsing the source)
- https://sources.debian.net/src/xauth/1:1.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xauth/1:1.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xdg-utils=1.1.3-4`

Binary Packages:

- `xdg-utils=1.1.3-4`

Licenses: (parsed from: `/usr/share/doc/xdg-utils/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris xdg-utils=1.1.3-4
'http://deb.debian.org/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3-4.dsc' xdg-utils_1.1.3-4.dsc 2093 SHA256:e0e32c5c302b74819fe432a21cc4ef0fc7da9d29db9ff8bf934104a8ea715cea
'http://deb.debian.org/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3.orig.tar.gz' xdg-utils_1.1.3.orig.tar.gz 297170 SHA256:d798b08af8a8e2063ddde6c9fa3398ca81484f27dec642c5627ffcaa0d4051d9
'http://deb.debian.org/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3-4.debian.tar.xz' xdg-utils_1.1.3-4.debian.tar.xz 15484 SHA256:7f980ab16b9c7e13726a053b9e5113062ab9669409b45d68f4c8944375fd95d4
```

Other potentially useful URLs:

- https://sources.debian.net/src/xdg-utils/1.1.3-4/ (for browsing the source)
- https://sources.debian.net/src/xdg-utils/1.1.3-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xdg-utils/1.1.3-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xft=2.3.2-2`

Binary Packages:

- `libxft2:amd64=2.3.2-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xft=2.3.2-2
'http://deb.debian.org/debian/pool/main/x/xft/xft_2.3.2-2.dsc' xft_2.3.2-2.dsc 2000 SHA256:56c1f34591cdc307e83abaabb28e22e190cabcf528241e18dfcd5dca9e530f89
'http://deb.debian.org/debian/pool/main/x/xft/xft_2.3.2.orig.tar.gz' xft_2.3.2.orig.tar.gz 402454 SHA256:26cdddcc70b187833cbe9dc54df1864ba4c03a7175b2ca9276de9f05dce74507
'http://deb.debian.org/debian/pool/main/x/xft/xft_2.3.2-2.diff.gz' xft_2.3.2-2.diff.gz 10327 SHA256:e94bd505f05507b5691dca9380c2bd4595ba1fd267c09831ab6e3be4bfd87062
```

Other potentially useful URLs:

- https://sources.debian.net/src/xft/2.3.2-2/ (for browsing the source)
- https://sources.debian.net/src/xft/2.3.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xft/2.3.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `xorg=1:7.7+22`

Binary Packages:

- `x11-common=1:7.7+22`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+22
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+22.dsc' xorg_7.7+22.dsc 1975 SHA256:5b273e9b4ece8f4525e73721cc1f14ea0772007035c24b5e35269bcdca45b69a
'http://deb.debian.org/debian/pool/main/x/xorg/xorg_7.7+22.tar.gz' xorg_7.7+22.tar.gz 287402 SHA256:4e39d07914480826f02f8ba293dc07e5595a2789c53ee47d92cc5ee992ef2ed5
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

- `liblzma-dev:amd64=5.2.5-2`
- `liblzma5:amd64=5.2.5-2`
- `xz-utils=5.2.5-2`

Licenses: (parsed from: `/usr/share/doc/liblzma-dev/copyright`, `/usr/share/doc/liblzma5/copyright`, `/usr/share/doc/xz-utils/copyright`)

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
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.dsc' xz-utils_5.2.5-2.dsc 2312 SHA256:fa2706f0c863bee4715460bc9103c6fb73ad2cbc12d8d6d7d5dced81ab349949
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA256:3e1e518ffc912f86608a8cb35e4bd41ad1aec210df2a47aaa1f95e7f5576ef56
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz.asc' xz-utils_5.2.5.orig.tar.xz.asc 833 SHA256:6efc0075a58912e640119d2b52ef7d1518b260d8720fadc73df21ab7fc727624
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.2.5-2.debian.tar.xz' xz-utils_5.2.5-2.debian.tar.xz 33532 SHA256:7bf06a86c35cc6b21a7731df9e11d241f8d3c16b0fe6ed78d64506d1bc29b06e
```

### `dpkg` source package: `zip=3.0-12`

Binary Packages:

- `zip=3.0-12`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zip=3.0-12
'http://deb.debian.org/debian/pool/main/z/zip/zip_3.0-12.dsc' zip_3.0-12.dsc 1328 SHA256:529b19003979b7eae4a305e05d0d9fda81917e2d55a16a6d65588d69380ab80f
'http://deb.debian.org/debian/pool/main/z/zip/zip_3.0.orig.tar.gz' zip_3.0.orig.tar.gz 1118845 SHA256:f0e8bb1f9b7eb0b01285495a2699df3a4b766784c1765a8f1aeedf63c0806369
'http://deb.debian.org/debian/pool/main/z/zip/zip_3.0-12.debian.tar.xz' zip_3.0-12.debian.tar.xz 8628 SHA256:522174080773f72882bd240ca384e698134f61ad6405ce8f995e1d21c9ba41d8
```

Other potentially useful URLs:

- https://sources.debian.net/src/zip/3.0-12/ (for browsing the source)
- https://sources.debian.net/src/zip/3.0-12/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/zip/3.0-12/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

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
