# `buildpack-deps:sid-scm`

## Docker Metadata

- Image ID: `sha256:32fbcb734afc617780a7497dd1659b3fc41e11fe61877d879529757d70531066`
- Created: `2022-11-15T10:28:04.475671448Z`
- Virtual Size: ~ 322.55 Mb  
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

### `dpkg` source package: `apr-util=1.6.1-5`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5+b2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-5
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1-5.dsc' apr-util_1.6.1-5.dsc 2754 SHA256:dab17dcb495ae31448ceb506448a5b1a6155ae9771073950227c47e09241b9d6
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2.asc' apr-util_1.6.1.orig.tar.bz2.asc 801 SHA256:47837b605290c0d7659b73734e4a9d5e6c0c24c13185cd4d91837afe63c07ca4
'http://deb.debian.org/debian/pool/main/a/apr-util/apr-util_1.6.1-5.debian.tar.xz' apr-util_1.6.1-5.debian.tar.xz 342000 SHA256:9489fa1228c0e7362f4a4d099c015b7552b928b7d73c9d79b6d4c16b52edce3b
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr-util/1.6.1-5/ (for browsing the source)
- https://sources.debian.net/src/apr-util/1.6.1-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr-util/1.6.1-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apr=1.7.0-8`

Binary Packages:

- `libapr1:amd64=1.7.0-8`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-8
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0-8.dsc' apr_1.7.0-8.dsc 2272 SHA256:f13890ccea0e69493c1d2172bf5b733e4b989931c44d150eb496bf88db55a528
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA256:e2e148f0b2e99b8e5c6caa09f6d4fb4dd3e83f744aa72a952f94f5a14436f7ea
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA256:5a6c4e721ed82116d7877254ae11c076014040af2ff816ea15ec81e77a4a7d43
'http://deb.debian.org/debian/pool/main/a/apr/apr_1.7.0-8.debian.tar.xz' apr_1.7.0-8.debian.tar.xz 215848 SHA256:a412ee67df3c7159d67e698293be83a3edc33ee086a35a385420de1a81a11b08
```

Other potentially useful URLs:

- https://sources.debian.net/src/apr/1.7.0-8/ (for browsing the source)
- https://sources.debian.net/src/apr/1.7.0-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apr/1.7.0-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `apt=2.5.4`

Binary Packages:

- `apt=2.5.4`
- `libapt-pkg6.0:amd64=2.5.4`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.5.4
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.5.4.dsc' apt_2.5.4.dsc 2933 SHA256:db0927bccb81a1fea73760bdb917d64261f8a482f99c74af09515a5e009b5fd2
'http://deb.debian.org/debian/pool/main/a/apt/apt_2.5.4.tar.xz' apt_2.5.4.tar.xz 2322832 SHA256:7c50f63fa8f8b28cde7b45055df168937d382f28b0045d5133829b70636ef872
```

Other potentially useful URLs:

- https://sources.debian.net/src/apt/2.5.4/ (for browsing the source)
- https://sources.debian.net/src/apt/2.5.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/apt/2.5.4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `audit=1:3.0.7-1.1`

Binary Packages:

- `libaudit-common=1:3.0.7-1.1`
- `libaudit1:amd64=1:3.0.7-1.1+b2`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0.7-1.1
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.7-1.1.dsc' audit_3.0.7-1.1.dsc 2500 SHA256:5b15ad446bf4904a985b9fd549341967b9b6c908a5096f4ebd02c0ad83ad00b7
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.7.orig.tar.gz' audit_3.0.7.orig.tar.gz 1180226 SHA256:8b4c78632a9301a1c7f859b0e38fc0b9c260b8214d6b7c771bf28b3d73a62597
'http://deb.debian.org/debian/pool/main/a/audit/audit_3.0.7-1.1.debian.tar.xz' audit_3.0.7-1.1.debian.tar.xz 18668 SHA256:f78863e469f8768b403a1d406e56a720aeb168788cd3b3f4d771a12280d1c70e
```

Other potentially useful URLs:

- https://sources.debian.net/src/audit/1:3.0.7-1.1/ (for browsing the source)
- https://sources.debian.net/src/audit/1:3.0.7-1.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/audit/1:3.0.7-1.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `base-files=12.3`

Binary Packages:

- `base-files=12.3`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=12.3
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_12.3.dsc' base-files_12.3.dsc 1078 SHA256:0a96a31ba0e17e966dd980c8c44b2d8cf397d448a79fcd6c254a6e4f83dc40e7
'http://deb.debian.org/debian/pool/main/b/base-files/base-files_12.3.tar.xz' base-files_12.3.tar.xz 65824 SHA256:3f48878de686a4e2f7aa2353168f056605d7a94100e52bd37a8a26ec17689bef
```

Other potentially useful URLs:

- https://sources.debian.net/src/base-files/12.3/ (for browsing the source)
- https://sources.debian.net/src/base-files/12.3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/base-files/12.3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `bash=5.2-2`

Binary Packages:

- `bash=5.2-2+b1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.2-2
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.2-2.dsc' bash_5.2-2.dsc 2296 SHA256:29d400729f7eef31fb181ffc3cf1d1099b3432f70da46dd702ae5872a5990efa
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.2.orig.tar.xz' bash_5.2.orig.tar.xz 5886100 SHA256:f358a087da1f0c754f814172d8cd0b012ea68086d7aadd4eabff92074aa575d8
'http://deb.debian.org/debian/pool/main/b/bash/bash_5.2-2.debian.tar.xz' bash_5.2-2.debian.tar.xz 86508 SHA256:c4ea6d58fc2c50a6d34ea06522983eab47fc41345a34373c37f67eb3d89c853f
```

Other potentially useful URLs:

- https://sources.debian.net/src/bash/5.2-2/ (for browsing the source)
- https://sources.debian.net/src/bash/5.2-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/bash/5.2-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2+b5`

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

### `dpkg` source package: `ca-certificates=20211016`

Binary Packages:

- `ca-certificates=20211016`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20211016
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20211016.dsc' ca-certificates_20211016.dsc 1890 SHA256:3d665bb54fa36529dc62fab8cf02a9d54c3a8530b17d9f3f93d170a97727b98c
'http://deb.debian.org/debian/pool/main/c/ca-certificates/ca-certificates_20211016.tar.xz' ca-certificates_20211016.tar.xz 239608 SHA256:2ae9b6dc5f40c25d6d7fe55e07b54f12a8967d1955d3b7b2f42ee46266eeef88
```

Other potentially useful URLs:

- https://sources.debian.net/src/ca-certificates/20211016/ (for browsing the source)
- https://sources.debian.net/src/ca-certificates/20211016/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/ca-certificates/20211016/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `curl=7.86.0-1`

Binary Packages:

- `curl=7.86.0-1`
- `libcurl3-gnutls:amd64=7.86.0-1`
- `libcurl4:amd64=7.86.0-1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `BSD-4-Clause-UC`
- `FSFULLR`
- `GPL-2`
- `GPL-2+ with Autoconf-data exception`
- `GPL-2+ with Libtool exception`
- `GPL-3+ with Autoconf-data exception`
- `ISC`
- `X11`
- `curl`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/curl/7.86.0-1/


### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg-9`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg-9`
- `libsasl2-modules-db:amd64=2.1.28+dfsg-9`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cyrus-sasl2/2.1.28+dfsg-9/


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debconf/1.5.79/


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

### `dpkg` source package: `debianutils=5.7-0.4`

Binary Packages:

- `debianutils=5.7-0.4`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`
- `GPL-2+`
- `SMAIL-GPL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.7-0.4
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.4.dsc' debianutils_5.7-0.4.dsc 1737 SHA256:1cd234cc6449122c5bb8213e7b2919162002ae4234a5c51b2b8e54e82837a047
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7.orig.tar.gz' debianutils_5.7.orig.tar.gz 257231 SHA256:27ec9e0e7e44dc8ab611aa576330471bacb07e4491ffecf0d3aa6909c92f9022
'http://deb.debian.org/debian/pool/main/d/debianutils/debianutils_5.7-0.4.debian.tar.xz' debianutils_5.7-0.4.debian.tar.xz 22412 SHA256:e47eb4fc4cd16fedc8fd741c42acb3af1de19ba42143016adafe61c282ad6771
```

Other potentially useful URLs:

- https://sources.debian.net/src/debianutils/5.7-0.4/ (for browsing the source)
- https://sources.debian.net/src/debianutils/5.7-0.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/debianutils/5.7-0.4/ (for access to the source package after it no longer exists in the archive)

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

- `dpkg=1.21.9+b1`

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

### `dpkg` source package: `e2fsprogs=1.46.6~rc1-1`

Binary Packages:

- `e2fsprogs=1.46.6~rc1-1+b1`
- `libcom-err2:amd64=1.46.6~rc1-1+b1`
- `libext2fs2:amd64=1.46.6~rc1-1+b1`
- `libss2:amd64=1.46.6~rc1-1+b1`
- `logsave=1.46.6~rc1-1+b1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.6~rc1-1
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1-1.dsc' e2fsprogs_1.46.6~rc1-1.dsc 2785 SHA256:794e88c34ec8ee6c51c01474248de036aece8aeef0f0b626d7b83003deba640c
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1.orig.tar.gz' e2fsprogs_1.46.6~rc1.orig.tar.gz 9615342 SHA256:a21354e3f0e94d2874ebe1b5587aa536438aca10b516aa00bd6a808e86c5adeb
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1.orig.tar.gz.asc' e2fsprogs_1.46.6~rc1.orig.tar.gz.asc 13016974 SHA256:26ffb2f1c2d7440375791863bc579347060ddf2b6c1339cf469d5edb492d4604
'http://deb.debian.org/debian/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1-1.debian.tar.xz' e2fsprogs_1.46.6~rc1-1.debian.tar.xz 83724 SHA256:300b9985a1c367071637e2416af4088f07edbcea7ef1c2293273a1b73ab0dd4b
```

Other potentially useful URLs:

- https://sources.debian.net/src/e2fsprogs/1.46.6~rc1-1/ (for browsing the source)
- https://sources.debian.net/src/e2fsprogs/1.46.6~rc1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/e2fsprogs/1.46.6~rc1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `expat=2.5.0-1`

Binary Packages:

- `libexpat1:amd64=2.5.0-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.5.0-1
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.5.0-1.dsc' expat_2.5.0-1.dsc 1981 SHA256:e7c69b69d720ae1e2971f5edc7fffe274f0047cc61e541cd2013afcc1ba80b81
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.5.0.orig.tar.gz' expat_2.5.0.orig.tar.gz 8320988 SHA256:ab00ee05c7067fd10a35c5d2a4922ebba746ddd50ff83b79c828da17bbdf1757
'http://deb.debian.org/debian/pool/main/e/expat/expat_2.5.0-1.debian.tar.xz' expat_2.5.0-1.debian.tar.xz 12680 SHA256:232c69ecdf58850b28b5e22374eae4db024d6558f2fbbd57b9af48ab31ce97ed
```

Other potentially useful URLs:

- https://sources.debian.net/src/expat/2.5.0-1/ (for browsing the source)
- https://sources.debian.net/src/expat/2.5.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/expat/2.5.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gcc-12=12.2.0-9`

Binary Packages:

- `gcc-12-base:amd64=12.2.0-9`
- `libgcc-s1:amd64=12.2.0-9`
- `libstdc++6:amd64=12.2.0-9`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12.2.0-9
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.2.0-9.dsc' gcc-12_12.2.0-9.dsc 27501 SHA256:63279c981d508ab170e62409398ca662818b00f498011671f3d1f2d69f09983c
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.2.0.orig.tar.gz' gcc-12_12.2.0.orig.tar.gz 87090343 SHA256:b8298be16aeeb96a889c6afed0a8e2241b47452e89cc81fe65ea849d5c740fcb
'http://deb.debian.org/debian/pool/main/g/gcc-12/gcc-12_12.2.0-9.debian.tar.xz' gcc-12_12.2.0-9.debian.tar.xz 1610684 SHA256:f0d55cb27b02d531047400eefa2ed898fbb8ce55a6b7cc4213e6b398bf3607e1
```

Other potentially useful URLs:

- https://sources.debian.net/src/gcc-12/12.2.0-9/ (for browsing the source)
- https://sources.debian.net/src/gcc-12/12.2.0-9/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gcc-12/12.2.0-9/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gdbm=1.23-3`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-3`
- `libgdbm6:amd64=1.23-3`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.23-3
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23-3.dsc' gdbm_1.23-3.dsc 2583 SHA256:3e4a52655a1b65c51d33e032913edda3423dcae8cc282c16a455a0afd2d2738d
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz' gdbm_1.23.orig.tar.gz 1115854 SHA256:74b1081d21fff13ae4bd7c16e5d6e504a4c26f7cde1dca0d963a484174bbcacd
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz.asc' gdbm_1.23.orig.tar.gz.asc 181 SHA256:64ebb68cc68e8915d62cb20ea40323c00b56051f844589ee0a52169fff34cecb
'http://deb.debian.org/debian/pool/main/g/gdbm/gdbm_1.23-3.debian.tar.xz' gdbm_1.23-3.debian.tar.xz 18552 SHA256:a0ff17befcbd7c4b361cfe0d821a7a71334102a9c423537bd57f60f18f6802ea
```

Other potentially useful URLs:

- https://sources.debian.net/src/gdbm/1.23-3/ (for browsing the source)
- https://sources.debian.net/src/gdbm/1.23-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gdbm/1.23-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `git=1:2.38.1-1`

Binary Packages:

- `git=1:2.38.1-1`
- `git-man=1:2.38.1-1`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-3-clause`
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
- `Zlib`
- `dlmalloc`
- `mingw-runtime`

Source:

```console
$ apt-get source -qq --print-uris git=1:2.38.1-1
'http://deb.debian.org/debian/pool/main/g/git/git_2.38.1-1.dsc' git_2.38.1-1.dsc 2825 SHA256:500be7ab00360288196aaf434efcc15e733e90dfb02157483e48196a8d56fe89
'http://deb.debian.org/debian/pool/main/g/git/git_2.38.1.orig.tar.xz' git_2.38.1.orig.tar.xz 7088208 SHA256:97ddf8ea58a2b9e0fbc2508e245028ca75911bd38d1551616b148c1aa5740ad9
'http://deb.debian.org/debian/pool/main/g/git/git_2.38.1-1.debian.tar.xz' git_2.38.1-1.debian.tar.xz 733140 SHA256:b2aec5827639f2f939774f457414a6b46f1fce1f014f76a1a48f12a980c3baca
```

Other potentially useful URLs:

- https://sources.debian.net/src/git/1:2.38.1-1/ (for browsing the source)
- https://sources.debian.net/src/git/1:2.38.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/git/1:2.38.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `glibc=2.36-5`

Binary Packages:

- `libc-bin=2.36-5`
- `libc6:amd64=2.36-5`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.36-5
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.36-5.dsc' glibc_2.36-5.dsc 9689 SHA256:7d6a6b90ff19c66f2704a8d2a9a21f2e2c1e0e67517b67fa9d0f5f862bbb69d3
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.36.orig.tar.xz' glibc_2.36.orig.tar.xz 19363988 SHA256:a543c02070d46ccaf866957efd13f10c924daa74c86a90a0254db09a92a708ee
'http://deb.debian.org/debian/pool/main/g/glibc/glibc_2.36-5.debian.tar.xz' glibc_2.36-5.debian.tar.xz 820064 SHA256:11ab403a5dd75750f1670671704a30571af73ad59f5ab3e3bfd86ca189cc80ec
```

Other potentially useful URLs:

- https://sources.debian.net/src/glibc/2.36-5/ (for browsing the source)
- https://sources.debian.net/src/glibc/2.36-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/glibc/2.36-5/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `gnupg2=2.2.40-1`

Binary Packages:

- `dirmngr=2.2.40-1`
- `gnupg=2.2.40-1`
- `gnupg-l10n=2.2.40-1`
- `gnupg-utils=2.2.40-1`
- `gpg=2.2.40-1`
- `gpg-agent=2.2.40-1`
- `gpg-wks-client=2.2.40-1`
- `gpg-wks-server=2.2.40-1`
- `gpgconf=2.2.40-1`
- `gpgsm=2.2.40-1`
- `gpgv=2.2.40-1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.40-1
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.dsc' gnupg2_2.2.40-1.dsc 3219 SHA256:2e07176a2a1c7f98ac9713d2b99b1c77f310d67b67a2f51faea1ed676b858bc5
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2' gnupg2_2.2.40.orig.tar.bz2 7301631 SHA256:1164b29a75e8ab93ea15033300149e1872a7ef6bdda3d7c78229a735f8204c28
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2.asc' gnupg2_2.2.40.orig.tar.bz2.asc 228 SHA256:3907dc165299cd53c0b4aec862323c3bce6037c411600ec87dc5eed7a55eba4a
'http://deb.debian.org/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.debian.tar.xz' gnupg2_2.2.40-1.debian.tar.xz 62220 SHA256:b398070b061dcf035da6e97576512ab7a0e13a48ab0364850be67a439e519706
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnupg2/2.2.40-1/ (for browsing the source)
- https://sources.debian.net/src/gnupg2/2.2.40-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnupg2/2.2.40-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `gnutls28=3.7.8-4`

Binary Packages:

- `libgnutls30:amd64=3.7.8-4`

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
$ apt-get source -qq --print-uris gnutls28=3.7.8-4
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.8-4.dsc' gnutls28_3.7.8-4.dsc 3445 SHA256:aa807a59f8c7a6d9d7b034eb8e9665f4b232fc496ca89bb1b9fec39c8cf192d5
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.8.orig.tar.xz' gnutls28_3.7.8.orig.tar.xz 6029220 SHA256:c58ad39af0670efe6a8aee5e3a8b2331a1200418b64b7c51977fb396d4617114
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.8.orig.tar.xz.asc' gnutls28_3.7.8.orig.tar.xz.asc 1760 SHA256:796ac6a01ed73a96b6737c4ea2928ea99715ce922fd49fe6e81de2fc36dc5945
'http://deb.debian.org/debian/pool/main/g/gnutls28/gnutls28_3.7.8-4.debian.tar.xz' gnutls28_3.7.8-4.debian.tar.xz 85632 SHA256:9b731ee77d3525885178096d44113e466f8033b35dd9df1540a8e7f5a488d5ad
```

Other potentially useful URLs:

- https://sources.debian.net/src/gnutls28/3.7.8-4/ (for browsing the source)
- https://sources.debian.net/src/gnutls28/3.7.8-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/gnutls28/3.7.8-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `grep=3.8-3`

Binary Packages:

- `grep=3.8-3`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.8-3
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.8-3.dsc' grep_3.8-3.dsc 1608 SHA256:b5b25e30ece7da06ea4ef856f362b77a6e47ece57e7b1b1b0abcf2f5b1312222
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.8.orig.tar.xz' grep_3.8.orig.tar.xz 1709536 SHA256:498d7cc1b4fb081904d87343febb73475cf771e424fb7e6141aff66013abc382
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.8.orig.tar.xz.asc' grep_3.8.orig.tar.xz.asc 833 SHA256:347aec924499df3fa41a0d782f3cd3e4a51a15de98b44eaab04084cd34060cd0
'http://deb.debian.org/debian/pool/main/g/grep/grep_3.8-3.debian.tar.xz' grep_3.8-3.debian.tar.xz 20332 SHA256:72d615732ccef5721b4c4e7cdf62daa46399d092ae7d324ff89958fb6cac8512
```

Other potentially useful URLs:

- https://sources.debian.net/src/grep/3.8-3/ (for browsing the source)
- https://sources.debian.net/src/grep/3.8-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/grep/3.8-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `keyutils=1.6.3-1`

Binary Packages:

- `libkeyutils1:amd64=1.6.3-1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.3-1
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3-1.dsc' keyutils_1.6.3-1.dsc 2055 SHA256:2c0e828b11a4483b5d1c949384f77d49412559c9f6a7193a1321476830f742be
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3.orig.tar.gz' keyutils_1.6.3.orig.tar.gz 137022 SHA256:a61d5706136ae4c05bd48f86186bcfdbd88dd8bd5107e3e195c924cfc1b39bb4
'http://deb.debian.org/debian/pool/main/k/keyutils/keyutils_1.6.3-1.debian.tar.xz' keyutils_1.6.3-1.debian.tar.xz 13136 SHA256:e11ef757e2db97c8c5cd381cc29f3e5e125aa485f8446dc62777ba5a16678a63
```

Other potentially useful URLs:

- https://sources.debian.net/src/keyutils/1.6.3-1/ (for browsing the source)
- https://sources.debian.net/src/keyutils/1.6.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/keyutils/1.6.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `krb5=1.20-1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.20-1+b1`
- `libk5crypto3:amd64=1.20-1+b1`
- `libkrb5-3:amd64=1.20-1+b1`
- `libkrb5support0:amd64=1.20-1+b1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/krb5/1.20-1/


### `dpkg` source package: `libassuan=2.5.5-5`

Binary Packages:

- `libassuan0:amd64=2.5.5-5`

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
$ apt-get source -qq --print-uris libassuan=2.5.5-5
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-5.dsc' libassuan_2.5.5-5.dsc 1997 SHA256:60be1d43dd5a7c4bce7a97f58513915990c8c615ea02c68b8cd5cf1e33b84a0c
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2' libassuan_2.5.5.orig.tar.bz2 572263 SHA256:8e8c2fcc982f9ca67dcbb1d95e2dc746b1739a4668bc20b3a3c5be632edb34e4
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2.asc' libassuan_2.5.5.orig.tar.bz2.asc 228 SHA256:8bb0d1d818ac91fa27a8ebed2975dac12eac9a6e075dfba225cc488ac9b4133f
'http://deb.debian.org/debian/pool/main/liba/libassuan/libassuan_2.5.5-5.debian.tar.xz' libassuan_2.5.5-5.debian.tar.xz 14256 SHA256:9d46fe972ba45692e28a2618e457a7f9141afc122281a862bcb4aa16716c97d7
```

Other potentially useful URLs:

- https://sources.debian.net/src/libassuan/2.5.5-5/ (for browsing the source)
- https://sources.debian.net/src/libassuan/2.5.5-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libassuan/2.5.5-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.11.7-1`

Binary Packages:

- `libbsd0:amd64=0.11.7-1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
- `BSD-3-clause-Regents`
- `BSD-3-clause-author`
- `BSD-4-clause-Niels-Provos`
- `BSD-5-clause-Peter-Wemm`
- `Beerware`
- `Expat`
- `ISC`
- `ISC-Original`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.11.7-1
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7-1.dsc' libbsd_0.11.7-1.dsc 2308 SHA256:f8627014f4ef55b2b79a4a26aacfa01a0c4fef899922a4c40b6f2dc5f8a7019c
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz' libbsd_0.11.7.orig.tar.xz 418508 SHA256:9baa186059ebbf25c06308e9f991fda31f7183c0f24931826d83aa6abd8a0261
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz.asc' libbsd_0.11.7.orig.tar.xz.asc 833 SHA256:b470d3fa5ad6948de7a85891e652970828f26eb7057028d57b94fa8644af934a
'http://deb.debian.org/debian/pool/main/libb/libbsd/libbsd_0.11.7-1.debian.tar.xz' libbsd_0.11.7-1.debian.tar.xz 18012 SHA256:8f852a5846f34df63ac56a2e520c2cc9bcd9eb7ecb6f67ecec78438a4c1f6d47
```

Other potentially useful URLs:

- https://sources.debian.net/src/libbsd/0.11.7-1/ (for browsing the source)
- https://sources.debian.net/src/libbsd/0.11.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libbsd/0.11.7-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libcap-ng=0.8.3-1`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1+b2`

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

### `dpkg` source package: `libcbor=0.8.0-2`

Binary Packages:

- `libcbor0.8:amd64=0.8.0-2+b1`

Licenses: (parsed from: `/usr/share/doc/libcbor0.8/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.8.0-2
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0-2.dsc' libcbor_0.8.0-2.dsc 2114 SHA256:ea9cbadf7d9cd9a3f7dcf7467f3e71dd7aab6d06cad15d01b2f0c19a0ad749a7
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0.orig.tar.gz' libcbor_0.8.0.orig.tar.gz 267044 SHA256:618097166ea4a54499646998ccaa949a5816e6a665cf1d6df383690895217c8b
'http://deb.debian.org/debian/pool/main/libc/libcbor/libcbor_0.8.0-2.debian.tar.xz' libcbor_0.8.0-2.debian.tar.xz 4024 SHA256:48df3ff85250d1e6274a19d9bcc18b5b582a368667120b7bd21d798ca6feccb0
```

Other potentially useful URLs:

- https://sources.debian.net/src/libcbor/0.8.0-2/ (for browsing the source)
- https://sources.debian.net/src/libcbor/0.8.0-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libcbor/0.8.0-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libedit=3.1-20221030-1`

Binary Packages:

- `libedit2:amd64=3.1-20221030-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libedit/3.1-20221030-1/


### `dpkg` source package: `liberror-perl=0.17029-2`

Binary Packages:

- `liberror-perl=0.17029-2`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17029-2
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029-2.dsc' liberror-perl_0.17029-2.dsc 2085 SHA256:48c6ca66e03144a8bec4f32b2419f34d70e8a00500b01ea3bb6a5cab0c03e164
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA256:1a23f7913032aed6d4b68321373a3899ca66590f4727391a091ec19c95bf7adc
'http://deb.debian.org/debian/pool/main/libe/liberror-perl/liberror-perl_0.17029-2.debian.tar.xz' liberror-perl_0.17029-2.debian.tar.xz 4608 SHA256:60deb5d5cbc4b478f8db4cfa0ac6c512e85eea5fcd7fc7285c26a9942d3b8b67
```

Other potentially useful URLs:

- https://sources.debian.net/src/liberror-perl/0.17029-2/ (for browsing the source)
- https://sources.debian.net/src/liberror-perl/0.17029-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/liberror-perl/0.17029-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libfido2=1.12.0-1`

Binary Packages:

- `libfido2-1:amd64=1.12.0-1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libfido2/1.12.0-1/


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

### `dpkg` source package: `libksba=1.6.2-3`

Binary Packages:

- `libksba8:amd64=1.6.2-3`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libksba/1.6.2-3/


### `dpkg` source package: `libmd=1.0.4-2`

Binary Packages:

- `libmd0:amd64=1.0.4-2`

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
$ apt-get source -qq --print-uris libmd=1.0.4-2
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4-2.dsc' libmd_1.0.4-2.dsc 2264 SHA256:5e060cb277f31e67b91033e05ece00832ca8056decba873b1698a5680414a177
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz' libmd_1.0.4.orig.tar.xz 264472 SHA256:f51c921042e34beddeded4b75557656559cf5b1f2448033b4c1eec11c07e530f
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz.asc' libmd_1.0.4.orig.tar.xz.asc 833 SHA256:32deebe1cfab127ee69a3e8c8caf439e459b7cdcdd7535fe021cb485adc14057
'http://deb.debian.org/debian/pool/main/libm/libmd/libmd_1.0.4-2.debian.tar.xz' libmd_1.0.4-2.debian.tar.xz 10204 SHA256:a27a2221b1a81e192455e2e93da2e313b21e489f6ac2bcf84b0b813dc3fe261b
```

Other potentially useful URLs:

- https://sources.debian.net/src/libmd/1.0.4-2/ (for browsing the source)
- https://sources.debian.net/src/libmd/1.0.4-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libmd/1.0.4-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libnsl=1.3.0-2`

Binary Packages:

- `libnsl2:amd64=1.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libnsl2/copyright`)

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

### `dpkg` source package: `libseccomp=2.5.4-1`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1+b2`

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

- `libselinux1:amd64=3.4-1+b3`

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
- `libsemanage2:amd64=3.4-1+b3`

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

### `dpkg` source package: `libssh2=1.10.0-3`

Binary Packages:

- `libssh2-1:amd64=1.10.0-3+b1`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.10.0-3
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0-3.dsc' libssh2_1.10.0-3.dsc 2283 SHA256:a0fe68f402a2f44dd6bd2219457fb8677b2149a83e7b009e93ff0635de940766
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz' libssh2_1.10.0.orig.tar.gz 965044 SHA256:2d64e90f3ded394b91d3a2e774ca203a4179f69aebee03003e5a6fa621e41d51
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz.asc' libssh2_1.10.0.orig.tar.gz.asc 488 SHA256:75702eaf490fa8c1e69b889c5c6366c2c3f3b089bc715f9f9be081c88f115f81
'http://deb.debian.org/debian/pool/main/libs/libssh2/libssh2_1.10.0-3.debian.tar.xz' libssh2_1.10.0-3.debian.tar.xz 8416 SHA256:c0bea31fe565273656349484d1000b557e489ee322834b40c4d7d33317a56940
```

Other potentially useful URLs:

- https://sources.debian.net/src/libssh2/1.10.0-3/ (for browsing the source)
- https://sources.debian.net/src/libssh2/1.10.0-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libssh2/1.10.0-3/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libtirpc=1.3.3+ds-1`

Binary Packages:

- `libtirpc-common=1.3.3+ds-1`
- `libtirpc3:amd64=1.3.3+ds-1`

Licenses: (parsed from: `/usr/share/doc/libtirpc-common/copyright`, `/usr/share/doc/libtirpc3/copyright`)

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
$ apt-get source -qq --print-uris libtirpc=1.3.3+ds-1
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.dsc' libtirpc_1.3.3+ds-1.dsc 2129 SHA256:c05c5d76027d4162d5a29d73eef90076559bde0fa5133b2e0045d82155e1b2af
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds.orig.tar.gz' libtirpc_1.3.3+ds.orig.tar.gz 699030 SHA256:facd98473c3a16fe6564c6458ef96ebb84d144345d1171f034fa019424bba027
'http://deb.debian.org/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.debian.tar.xz' libtirpc_1.3.3+ds-1.debian.tar.xz 11232 SHA256:fd1865c49e905951a641082981c1dab7f018caea1a5e23af1791728a3320800e
```

Other potentially useful URLs:

- https://sources.debian.net/src/libtirpc/1.3.3+ds-1/ (for browsing the source)
- https://sources.debian.net/src/libtirpc/1.3.3+ds-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/libtirpc/1.3.3+ds-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `libxcrypt=1:4.4.30-1`

Binary Packages:

- `libcrypt1:amd64=1:4.4.30-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxcrypt/1:4.4.30-1/


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

### `dpkg` source package: `media-types=8.0.0`

Binary Packages:

- `media-types=8.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=8.0.0
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_8.0.0.dsc' media-types_8.0.0.dsc 1620 SHA256:e80b1ac65060ce4a6d12184ca9ee564f38073b736e4ddd473be081931b50ffed
'http://deb.debian.org/debian/pool/main/m/media-types/media-types_8.0.0.tar.xz' media-types_8.0.0.tar.xz 56364 SHA256:85f9b3ccbb6bc8dc0fff47105726ca1877ac2011cc7e8244ab276d5583f4890e
```

Other potentially useful URLs:

- https://sources.debian.net/src/media-types/8.0.0/ (for browsing the source)
- https://sources.debian.net/src/media-types/8.0.0/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/media-types/8.0.0/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mercurial=6.2.3-1`

Binary Packages:

- `mercurial=6.2.3-1+b1`
- `mercurial-common=6.2.3-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=6.2.3-1
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.2.3-1.dsc' mercurial_6.2.3-1.dsc 2799 SHA256:99e81e44614075c6cab7b20225df50a8c33480e61af640f3d72c63802db70129
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.2.3.orig.tar.gz' mercurial_6.2.3.orig.tar.gz 8058864 SHA256:98d1ae002f68adf53d65c5947fe8b7a379f98cf05d9b8ea1f4077d2ca5dce9db
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.2.3.orig.tar.gz.asc' mercurial_6.2.3.orig.tar.gz.asc 659 SHA256:ce18248bfb508479f8117df172951a64c8098e9768af4db90adf951ff329f74b
'http://deb.debian.org/debian/pool/main/m/mercurial/mercurial_6.2.3-1.debian.tar.xz' mercurial_6.2.3-1.debian.tar.xz 69956 SHA256:459b0dec435d3af41aad8918a07fa9eadff56ee385d08f7460584445f237402a
```

Other potentially useful URLs:

- https://sources.debian.net/src/mercurial/6.2.3-1/ (for browsing the source)
- https://sources.debian.net/src/mercurial/6.2.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mercurial/6.2.3-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpdecimal=2.5.1-2`

Binary Packages:

- `libmpdec3:amd64=2.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libmpdec3/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.5.1-2
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1-2.dsc' mpdecimal_2.5.1-2.dsc 1919 SHA256:293054eddc70e50d3a482d1fec446a7f10202b9c6f7ceaf92600f60b429f8919
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1.orig.tar.gz' mpdecimal_2.5.1.orig.tar.gz 2584021 SHA256:9f9cd4c041f99b5c49ffb7b59d9f12d95b683d88585608aa56a6307667b2b21f
'http://deb.debian.org/debian/pool/main/m/mpdecimal/mpdecimal_2.5.1-2.debian.tar.xz' mpdecimal_2.5.1-2.debian.tar.xz 6696 SHA256:5ff6a2502605579d140614e7c023c14d363f520253cc2ef8e844651807237321
```

Other potentially useful URLs:

- https://sources.debian.net/src/mpdecimal/2.5.1-2/ (for browsing the source)
- https://sources.debian.net/src/mpdecimal/2.5.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mpdecimal/2.5.1-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ncurses=6.3+20220423-2`

Binary Packages:

- `libncurses6:amd64=6.3+20220423-2`
- `libncursesw6:amd64=6.3+20220423-2`
- `libtinfo6:amd64=6.3+20220423-2`
- `ncurses-base=6.3+20220423-2`
- `ncurses-bin=6.3+20220423-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

### `dpkg` source package: `netbase=6.4`

Binary Packages:

- `netbase=6.4`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.4
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.4.dsc' netbase_6.4.dsc 898 SHA256:dc26cfcaa49fd874cc27c65216b2f8b6d3ad62845b78da4bdf0aea55592af756
'http://deb.debian.org/debian/pool/main/n/netbase/netbase_6.4.tar.xz' netbase_6.4.tar.xz 32712 SHA256:fa6621826ff1150e581bd90bc3c8a4ecafe5df90404f207db6dcdf2c75f26ad7
```

Other potentially useful URLs:

- https://sources.debian.net/src/netbase/6.4/ (for browsing the source)
- https://sources.debian.net/src/netbase/6.4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/netbase/6.4/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `nghttp2=1.50.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.50.0-1+b1`

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
$ apt-get source -qq --print-uris nghttp2=1.50.0-1
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.50.0-1.dsc' nghttp2_1.50.0-1.dsc 2508 SHA256:60ee2845ebb87ea663191a22d16fa4bc191ddb7a826c94e56f39023e717ebacc
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.50.0.orig.tar.gz' nghttp2_1.50.0.orig.tar.gz 3885952 SHA256:6de469efc8e9d47059327a6736aebe0a7d73f57e5e37ab4c4f838fb1eebd7889
'http://deb.debian.org/debian/pool/main/n/nghttp2/nghttp2_1.50.0-1.debian.tar.xz' nghttp2_1.50.0-1.debian.tar.xz 12912 SHA256:4db3911036ea625172b517d590a31386fd950b1a9c4b561e252d915582af8318
```

Other potentially useful URLs:

- https://sources.debian.net/src/nghttp2/1.50.0-1/ (for browsing the source)
- https://sources.debian.net/src/nghttp2/1.50.0-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/nghttp2/1.50.0-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `openldap=2.5.13+dfsg-2`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.13+dfsg-2+b1`

Licenses: (parsed from: `/usr/share/doc/libldap-2.5-0/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-California`
- `BSD-3-clause-variant`
- `BSD-4-clause-California`
- `Beerware`
- `Expat`
- `Expat-ISC`
- `Expat-UNM`
- `F5`
- `FSF-unlimited`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `GPL-2+ with Libtool exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Autoconf exception`
- `GPL-3+ with Libtool exception`
- `JCG`
- `MIT-XC`
- `NeoSoft-permissive`
- `OpenLDAP-2.8`
- `UMich`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.13+dfsg-2
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg-2.dsc' openldap_2.5.13+dfsg-2.dsc 3224 SHA256:304eb2f104e2c1986f18c14c4f3d0ddba6049aa4440f8401c903303c6943ef24
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg.orig.tar.xz' openldap_2.5.13+dfsg.orig.tar.xz 3727704 SHA256:1d95c400a3eae6730246614ef16883de3dbd1b14b01a1ebe3a9aa1ccad2c13ec
'http://deb.debian.org/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg-2.debian.tar.xz' openldap_2.5.13+dfsg-2.debian.tar.xz 164476 SHA256:ca255fdc5ef77c3c9660af701331f19a0fe7dffbd625c5302746d2ace75a9656
```

Other potentially useful URLs:

- https://sources.debian.net/src/openldap/2.5.13+dfsg-2/ (for browsing the source)
- https://sources.debian.net/src/openldap/2.5.13+dfsg-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openldap/2.5.13+dfsg-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssh=1:9.1p1-1`

Binary Packages:

- `openssh-client=1:9.1p1-1`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:9.1p1-1
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.1p1-1.dsc' openssh_9.1p1-1.dsc 3311 SHA256:66cecc01833154ecc84909a16b947e66b800935b58d33c11c45fe84a3026e8af
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.1p1.orig.tar.gz' openssh_9.1p1.orig.tar.gz 1838747 SHA256:19f85009c7e3e23787f0236fbb1578392ab4d4bf9f8ec5fe6bc1cd7e8bfdd288
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.1p1.orig.tar.gz.asc' openssh_9.1p1.orig.tar.gz.asc 833 SHA256:abac4673e0862604ab1f69a4597d191940c0cf58679dc5fc81fbdbd8b28ca267
'http://deb.debian.org/debian/pool/main/o/openssh/openssh_9.1p1-1.debian.tar.xz' openssh_9.1p1-1.debian.tar.xz 179584 SHA256:a6ffc0939c91d636ef4fe6514295de63ac57280a1c2fd207e9914c5618648d0d
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssh/1:9.1p1-1/ (for browsing the source)
- https://sources.debian.net/src/openssh/1:9.1p1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssh/1:9.1p1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `openssl=3.0.7-1`

Binary Packages:

- `libssl3:amd64=3.0.7-1`
- `openssl=3.0.7-1`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.7-1
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.7-1.dsc' openssl_3.0.7-1.dsc 2601 SHA256:96e332e50ec17be6f623ef2c77c6146f2dd8418e4b1fe918db0b27798c0e9087
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.7.orig.tar.gz' openssl_3.0.7.orig.tar.gz 15107575 SHA256:83049d042a260e696f62406ac5c08bf706fd84383f945cf21bd61e9ed95c396e
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.7.orig.tar.gz.asc' openssl_3.0.7.orig.tar.gz.asc 858 SHA256:18be1d820b25ed5c7d8efe4fdba0b947925273ca114bbd78faecbd99a52df203
'http://deb.debian.org/debian/pool/main/o/openssl/openssl_3.0.7-1.debian.tar.xz' openssl_3.0.7-1.debian.tar.xz 74992 SHA256:a43f0c9aa8756629d8d34c3e9f41f5bed85672c7a4b6110d3f65a5edf5d3b89b
```

Other potentially useful URLs:

- https://sources.debian.net/src/openssl/3.0.7-1/ (for browsing the source)
- https://sources.debian.net/src/openssl/3.0.7-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/openssl/3.0.7-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `pam=1.5.2-5`

Binary Packages:

- `libpam-modules:amd64=1.5.2-5`
- `libpam-modules-bin=1.5.2-5`
- `libpam-runtime=1.5.2-5`
- `libpam0g:amd64=1.5.2-5`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.5.2-5
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-5.dsc' pam_1.5.2-5.dsc 2559 SHA256:84f46408901fdc41394db0a7feecffafb889fd5420a4d0b158af8b92970e2f37
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA256:e4ec7131a91da44512574268f493c6d8ca105c87091691b8e9b56ca685d4f94d
'http://deb.debian.org/debian/pool/main/p/pam/pam_1.5.2-5.debian.tar.xz' pam_1.5.2-5.debian.tar.xz 120208 SHA256:bcb0bc38f2589669eb92feec0581235f06b9d278393326ec509963484853a46c
```

Other potentially useful URLs:

- https://sources.debian.net/src/pam/1.5.2-5/ (for browsing the source)
- https://sources.debian.net/src/pam/1.5.2-5/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pam/1.5.2-5/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pcre2=10.40-2`

Binary Packages:

- `libpcre2-8-0:amd64=10.40-2`

Licenses: (parsed from: `/usr/share/doc/libpcre2-8-0/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-3-clause-Cambridge with BINARY LIBRARY-LIKE PACKAGES exception`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pcre2=10.40-2
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40-2.dsc' pcre2_10.40-2.dsc 2286 SHA256:0e8c4be76baaa3d0e6917d28d8d58756bea4d7d792ef81950b8ce2e132213526
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40.orig.tar.gz' pcre2_10.40.orig.tar.gz 2359622 SHA256:ded42661cab30ada2e72ebff9e725e745b4b16ce831993635136f2ef86177724
'http://deb.debian.org/debian/pool/main/p/pcre2/pcre2_10.40-2.diff.gz' pcre2_10.40-2.diff.gz 7862 SHA256:1a465883118d186a27ac6c2c7adb118bf54bf4e7fe161c587cdd86df1c323f21
```

Other potentially useful URLs:

- https://sources.debian.net/src/pcre2/10.40-2/ (for browsing the source)
- https://sources.debian.net/src/pcre2/10.40-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pcre2/10.40-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `perl=5.36.0-4`

Binary Packages:

- `libperl5.36:amd64=5.36.0-4`
- `perl=5.36.0-4`
- `perl-base=5.36.0-4`
- `perl-modules-5.36=5.36.0-4`

Licenses: (parsed from: `/usr/share/doc/libperl5.36/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.36/copyright`)

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
$ apt-get source -qq --print-uris perl=5.36.0-4
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0-4.dsc' perl_5.36.0-4.dsc 2886 SHA256:0197ec2878f75924f4f998831452e5f1f0dc690f001ffda47dc863661a7cb098
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0.orig-regen-configure.tar.xz' perl_5.36.0.orig-regen-configure.tar.xz 417784 SHA256:10ac353bc5a933403afe60ed1817e7a456f99bdbcaf80c1cdb0eb3a08ea56d4e
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0.orig.tar.xz' perl_5.36.0.orig.tar.xz 13051500 SHA256:0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0
'http://deb.debian.org/debian/pool/main/p/perl/perl_5.36.0-4.debian.tar.xz' perl_5.36.0-4.debian.tar.xz 167276 SHA256:2a21ee22a950c598cb83f436ef92d6f59c0651a1b8ac0beaa495e2fb8343624a
```

Other potentially useful URLs:

- https://sources.debian.net/src/perl/5.36.0-4/ (for browsing the source)
- https://sources.debian.net/src/perl/5.36.0-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/perl/5.36.0-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `pinentry=1.2.1-1`

Binary Packages:

- `pinentry-curses=1.2.1-1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.2.1-1
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1-1.dsc' pinentry_1.2.1-1.dsc 2242 SHA256:cb45060817fa5563d76591d99f0a7596aa069101710545852ec34a70a387597e
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1.orig.tar.bz2' pinentry_1.2.1.orig.tar.bz2 547698 SHA256:457a185e5a85238fb945a955dc6352ab962dc8b48720b62fc9fa48c7540a4067
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1.orig.tar.bz2.asc' pinentry_1.2.1.orig.tar.bz2.asc 390 SHA256:9f7d9c7509e4ff4161a043893d76183bd975230fcad671b643c90f78e500ba95
'http://deb.debian.org/debian/pool/main/p/pinentry/pinentry_1.2.1-1.debian.tar.xz' pinentry_1.2.1-1.debian.tar.xz 18568 SHA256:ae1bd8af99fe91bd3877b6fd3d606facbfb1be02d0227da7cc81f54f7fe2f708
```

Other potentially useful URLs:

- https://sources.debian.net/src/pinentry/1.2.1-1/ (for browsing the source)
- https://sources.debian.net/src/pinentry/1.2.1-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/pinentry/1.2.1-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `procps=2:3.3.17-7.1`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-7.1`
- `procps=2:3.3.17-7.1`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-7.1
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-7.1.dsc' procps_3.3.17-7.1.dsc 2144 SHA256:789aba0b71ce3985ac7c9fb2f80a7a66afc5924590dba241e0b345c64136511e
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA256:4518b3e7aafd34ec07d0063d250fd474999b20b200218c3ae56f5d2113f141b4
'http://deb.debian.org/debian/pool/main/p/procps/procps_3.3.17-7.1.debian.tar.xz' procps_3.3.17-7.1.debian.tar.xz 29244 SHA256:7c2cd3d0f83b74adc202e463fbc55591538a1f2e1cc775ebaa7f5bf7be48949e
```

Other potentially useful URLs:

- https://sources.debian.net/src/procps/2:3.3.17-7.1/ (for browsing the source)
- https://sources.debian.net/src/procps/2:3.3.17-7.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/procps/2:3.3.17-7.1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `python3-defaults=3.10.6-2`

Binary Packages:

- `libpython3-stdlib:amd64=3.10.6-2`
- `python3=3.10.6-2`
- `python3-minimal=3.10.6-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-defaults/3.10.6-2/


### `dpkg` source package: `python3.10=3.10.8-3`

Binary Packages:

- `libpython3.10-minimal:amd64=3.10.8-3`
- `libpython3.10-stdlib:amd64=3.10.8-3`
- `python3.10=3.10.8-3`
- `python3.10-minimal=3.10.8-3`

Licenses: (parsed from: `/usr/share/doc/libpython3.10-minimal/copyright`, `/usr/share/doc/libpython3.10-stdlib/copyright`, `/usr/share/doc/python3.10/copyright`, `/usr/share/doc/python3.10-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.10=3.10.8-3
'http://deb.debian.org/debian/pool/main/p/python3.10/python3.10_3.10.8-3.dsc' python3.10_3.10.8-3.dsc 3662 SHA256:c8299b1b682e515ca6424afa733d5ace13ddb8fa3613d4cace7636240a546b34
'http://deb.debian.org/debian/pool/main/p/python3.10/python3.10_3.10.8.orig.tar.xz' python3.10_3.10.8.orig.tar.xz 19619508 SHA256:6a30ecde59c47048013eb5a658c9b5dec277203d2793667f578df7671f7f03f3
'http://deb.debian.org/debian/pool/main/p/python3.10/python3.10_3.10.8-3.debian.tar.xz' python3.10_3.10.8-3.debian.tar.xz 219448 SHA256:0975ad5385c5014ed26927363a9cade2291539aeb3c1078da025bbd5b11b3c98
```

Other potentially useful URLs:

- https://sources.debian.net/src/python3.10/3.10.8-3/ (for browsing the source)
- https://sources.debian.net/src/python3.10/3.10.8-3/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/python3.10/3.10.8-3/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `readline=8.2-1.1`

Binary Packages:

- `libreadline8:amd64=8.2-1.1`
- `readline-common=8.2-1.1`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/readline/8.2-1.1/


### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2+b2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc 2299 SHA256:a296819cd2ab5880b67ad963ef0867cb10e462f4403e52565aa863eb05bb1370
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://deb.debian.org/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz 8096 SHA256:26d47de07d16285e4ca55b0828cbbf1ba35e671f9b3500a87e301fe755d26882
```

Other potentially useful URLs:

- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for browsing the source)
- https://sources.debian.net/src/rtmpdump/2.4+20151223.gitfa8646d.1-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/rtmpdump/2.4+20151223.gitfa8646d.1-2/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `sensible-utils=0.0.17`

Binary Packages:

- `sensible-utils=0.0.17`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.17
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.17.dsc' sensible-utils_0.0.17.dsc 1733 SHA256:e4754f4763f77d57fdb29093ec78eb0a84bac4e3aa94e4c251f0d00f11a4b231
'http://deb.debian.org/debian/pool/main/s/sensible-utils/sensible-utils_0.0.17.tar.xz' sensible-utils_0.0.17.tar.xz 66648 SHA256:5edf1f6043eeb88957ffe0b0e8793fbbdf40c8ff83f5bf9b36c9421c2d977626
```

Other potentially useful URLs:

- https://sources.debian.net/src/sensible-utils/0.0.17/ (for browsing the source)
- https://sources.debian.net/src/sensible-utils/0.0.17/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sensible-utils/0.0.17/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `serf=1.3.9-11`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-11`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-11/


### `dpkg` source package: `shadow=1:4.13+dfsg1-1`

Binary Packages:

- `login=1:4.13+dfsg1-1`
- `passwd=1:4.13+dfsg1-1`

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

### `dpkg` source package: `sqlite3=3.39.4-1`

Binary Packages:

- `libsqlite3-0:amd64=3.39.4-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.39.4-1/


### `dpkg` source package: `subversion=1.14.2-4`

Binary Packages:

- `libsvn1:amd64=1.14.2-4`
- `subversion=1.14.2-4`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `AFL-3`
- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BoostAcMacros`
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
$ apt-get source -qq --print-uris subversion=1.14.2-4
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2-4.dsc' subversion_1.14.2-4.dsc 4046 SHA256:8a4b9684043e17d0bb4c1892be7869493563613ef7e2dfe4bb3ffac059ff1b87
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2.orig.tar.gz' subversion_1.14.2.orig.tar.gz 11626792 SHA256:fd826afad03db7a580722839927dc664f3e93398fe88b66905732c8530971353
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2.orig.tar.gz.asc' subversion_1.14.2.orig.tar.gz.asc 3215 SHA256:da6a0a5ff56f671ad2d1eae708f8d1cc1abf0485b029a163ff8272cba5475861
'http://deb.debian.org/debian/pool/main/s/subversion/subversion_1.14.2-4.debian.tar.xz' subversion_1.14.2-4.debian.tar.xz 337148 SHA256:b9da3d33171f9e153a2c9d2080996a2fda6cf3b30659f9bbff0c00d279f6f2e6
```

Other potentially useful URLs:

- https://sources.debian.net/src/subversion/1.14.2-4/ (for browsing the source)
- https://sources.debian.net/src/subversion/1.14.2-4/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/subversion/1.14.2-4/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `systemd=252.1-1`

Binary Packages:

- `libsystemd0:amd64=252.1-1`
- `libudev1:amd64=252.1-1`

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

- http://snapshot.debian.org/package/systemd/252.1-1/


### `dpkg` source package: `sysvinit=3.05-7`

Binary Packages:

- `sysvinit-utils=3.05-7`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.05-7
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.05-7.dsc' sysvinit_3.05-7.dsc 2359 SHA256:b2da3c9acf9247111c39f1fddc8698c4636ff8f2d38910026c73af1fc9fc89a0
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.05.orig.tar.gz' sysvinit_3.05.orig.tar.gz 435554 SHA256:1e15471afdd550e88c121e5030707d9f00ca66b29fa91eacdaae072bde53f6bc
'http://deb.debian.org/debian/pool/main/s/sysvinit/sysvinit_3.05-7.debian.tar.xz' sysvinit_3.05-7.debian.tar.xz 134388 SHA256:9fbadadc858b042a70bb483866d5b5d2b51dcf73097853c4c42fa13c30ab2acb
```

Other potentially useful URLs:

- https://sources.debian.net/src/sysvinit/3.05-7/ (for browsing the source)
- https://sources.debian.net/src/sysvinit/3.05-7/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/sysvinit/3.05-7/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `tzdata=2022f-1`

Binary Packages:

- `tzdata=2022f-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tzdata=2022f-1
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022f-1.dsc' tzdata_2022f-1.dsc 2205 SHA256:ba9398a31794bf68a9ab08edc1560b6fc41644db67381fa1044cc7bec71eaeb7
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022f.orig.tar.gz' tzdata_2022f.orig.tar.gz 436352 SHA256:9990d71f675d212567b931fe8aae1cab7027f89fefb8a79d808a6933a67af000
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022f.orig.tar.gz.asc' tzdata_2022f.orig.tar.gz.asc 833 SHA256:2788b16875bbb5f8ccd1343352ed9bcf7cb98393ea6ecb49f48bb938ffc88854
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2022f-1.debian.tar.xz' tzdata_2022f-1.debian.tar.xz 112140 SHA256:e0780bbc953d605a30da7627ac3fd3bd738ef23aa5cad08d346367f2ef372b33
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2022f-1/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2022f-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2022f-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `usrmerge=33`

Binary Packages:

- `usr-is-merged=33`

Licenses: (parsed from: `/usr/share/doc/usr-is-merged/copyright`)

- `GPL v2`
- `GPL-2`
- `later (please see /usr/share/common-licenses/GPL-2)`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=33
'http://deb.debian.org/debian/pool/main/u/usrmerge/usrmerge_33.dsc' usrmerge_33.dsc 981 SHA256:2bb5db7017ba0703691b6d4da14329d80e2d6eb8ae51a9fcd783f0ee8a369ab2
'http://deb.debian.org/debian/pool/main/u/usrmerge/usrmerge_33.tar.xz' usrmerge_33.tar.xz 14084 SHA256:55e1f5b8ba2e10e418f6c70de627ee9554c5caf730f657ba062b060a916b3b7d
```

Other potentially useful URLs:

- https://sources.debian.net/src/usrmerge/33/ (for browsing the source)
- https://sources.debian.net/src/usrmerge/33/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/usrmerge/33/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `utf8proc=2.7.0-4`

Binary Packages:

- `libutf8proc2:amd64=2.7.0-4`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/utf8proc/2.7.0-4/


### `dpkg` source package: `util-linux=2.38.1-1.1`

Binary Packages:

- `bsdutils=1:2.38.1-1.1+b1`
- `libblkid1:amd64=2.38.1-1.1+b1`
- `libmount1:amd64=2.38.1-1.1+b1`
- `libsmartcols1:amd64=2.38.1-1.1+b1`
- `libuuid1:amd64=2.38.1-1.1+b1`
- `mount=2.38.1-1.1+b1`
- `util-linux=2.38.1-1.1+b1`
- `util-linux-extra=2.38.1-1.1+b1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/util-linux/2.38.1-1.1/


### `dpkg` source package: `wget=1.21.3-1`

Binary Packages:

- `wget=1.21.3-1+b2`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21.3-1
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3-1.dsc' wget_1.21.3-1.dsc 2167 SHA256:e294772dac85a4d59fa64269515aa4a93664789f1f4612cfe309785384fd1f55
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3.orig.tar.gz' wget_1.21.3.orig.tar.gz 5079864 SHA256:5726bb8bc5ca0f6dc7110f6416e4bb7019e2d2ff5bf93d1ca2ffcc6656f220e5
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3.orig.tar.gz.asc' wget_1.21.3.orig.tar.gz.asc 854 SHA256:a4d96f04bc5a034310eae177df9adc79ef7a6f0fad7bf7669bf0ac318fa22ccd
'http://deb.debian.org/debian/pool/main/w/wget/wget_1.21.3-1.debian.tar.xz' wget_1.21.3-1.debian.tar.xz 60660 SHA256:30901c12ded6e455d55fe73c40245b51d2fd53e20e30713a10e066fdfadb9d20
```

Other potentially useful URLs:

- https://sources.debian.net/src/wget/1.21.3-1/ (for browsing the source)
- https://sources.debian.net/src/wget/1.21.3-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/wget/1.21.3-1/ (for access to the source package after it no longer exists in the archive)

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

### `dpkg` source package: `xz-utils=5.2.7-0.1`

Binary Packages:

- `liblzma5:amd64=5.2.7-0.1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.7-0.1
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.7-0.1.dsc' xz-utils_5.2.7-0.1.dsc 2247 SHA256:9324b210c29b9a9e0ae510e98d160d3c22e043bceafc16df0321a910f5769457
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.7.orig.tar.xz' xz-utils_5.2.7.orig.tar.xz 1282620 SHA256:8712e9acb0b6b49a97d443458a3067dc5c08a025e02dc5f773176c51dd7cfc69
'http://deb.debian.org/debian/pool/main/x/xz-utils/xz-utils_5.2.7-0.1.debian.tar.xz' xz-utils_5.2.7-0.1.debian.tar.xz 31540 SHA256:9cf41fbe4f0048b8553ad7b4085f90ee671b24da77b4f630b4a149fcc43f613e
```

Other potentially useful URLs:

- https://sources.debian.net/src/xz-utils/5.2.7-0.1/ (for browsing the source)
- https://sources.debian.net/src/xz-utils/5.2.7-0.1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/xz-utils/5.2.7-0.1/ (for access to the source package after it no longer exists in the archive)

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
