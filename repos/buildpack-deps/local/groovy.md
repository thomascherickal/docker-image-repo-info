# `buildpack-deps:groovy`

## Docker Metadata

- Image ID: `sha256:268406b604889e3d02865d4fe81c03c400558f3adc09ba73ba44723740f865ed`
- Created: `2020-08-19T22:30:05.044529727Z`
- Virtual Size: ~ 714.34 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
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
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-8.dsc' acl_2.2.53-8.dsc 2464 SHA256:63623506d567cc90c9491aba7e40d480034a21f2d38b0c626f610ef637753a2c
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-8.debian.tar.xz' acl_2.2.53-8.debian.tar.xz 25300 SHA256:f8cfc2ce609f0fa19450cc4cb87aa98c48486231e80f04680b76072c05972e23
```

### `dpkg` source package: `adduser=3.118ubuntu2`

Binary Packages:

- `adduser=3.118ubuntu2`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.118ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.dsc' adduser_3.118ubuntu2.dsc 1131 SHA256:785f99d8c75c972cd42d3fab3afa07f97299bb1d70013fe5d295f045224774bb
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.tar.xz' adduser_3.118ubuntu2.tar.xz 222364 SHA256:9429124c39c381b541005da6f0ae29831bd6533dd65c923e06ca2a7c310db382
```

### `dpkg` source package: `apr-util=1.6.1-4ubuntu2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.dsc' apr-util_1.6.1-4ubuntu2.dsc 2686 SHA256:bf8be458f58a6b1576d35bc78647bb0e990fc0d0c47ee7b51a5e2ecf3d378aac
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.debian.tar.xz' apr-util_1.6.1-4ubuntu2.debian.tar.xz 213052 SHA256:2293c33f2e8d354aae7285e6037820d32305dcf4843093123c0683946ae35967
```

### `dpkg` source package: `apr=1.6.5-1ubuntu1`

Binary Packages:

- `libapr1:amd64=1.6.5-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.5-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.dsc' apr_1.6.5-1ubuntu1.dsc 2390 SHA256:9e9d5b1be5c9d17c4720d43096064da70a4cba1593f10c272328e16f8ed4c656
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2' apr_1.6.5.orig.tar.bz2 855393 SHA256:a67ca9fcf9c4ff59bce7f428a323c8b5e18667fdea7b0ebad47d194371b0a105
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2.asc' apr_1.6.5.orig.tar.bz2.asc 801 SHA256:9beff0bb06f4cbbb006176af93258d946d33b7fb54aac13a4c90cfba1cfd0c88
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.debian.tar.xz' apr_1.6.5-1ubuntu1.debian.tar.xz 213596 SHA256:faca1bccb281c7d91bf0846ee908dd0be53b4482c0a1850e03397307682717d1
```

### `dpkg` source package: `apt=2.1.10`

Binary Packages:

- `apt=2.1.10`
- `libapt-pkg6.0:amd64=2.1.10`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.1.10
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.1.10.dsc' apt_2.1.10.dsc 2760 SHA256:2368cefda44f61bb73970781be04ae7947290606d929f1682fb3cfa6ddb6ec0a
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.1.10.tar.xz' apt_2.1.10.tar.xz 2179772 SHA256:aa678d0fcd614a7707e77f3219097401141f5426cd1095c4aa50043920a2c04b
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.dsc' attr_2.4.48-5.dsc 2433 SHA256:0b20a285b758083e2e202ffdd2930cef1bf84fee498791fc3e26b69a3bced01d
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.debian.tar.xz' attr_2.4.48-5.debian.tar.xz 25560 SHA256:02238253d324250dabdc0434f7de045d85df93458995a465ac434f2a3978a312
```

### `dpkg` source package: `audit=1:2.8.5-2ubuntu6`

Binary Packages:

- `libaudit-common=1:2.8.5-2ubuntu6`
- `libaudit1:amd64=1:2.8.5-2ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `autoconf=2.69-11.1`

Binary Packages:

- `autoconf=2.69-11.1`

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
$ apt-get source -qq --print-uris autoconf=2.69-11.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.1.dsc' autoconf_2.69-11.1.dsc 1735 SHA256:06ab6e617ed8d07eecbc29a1669cd748b7ce11ab457c186e7e8794fe02b231ba
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.1.debian.tar.xz' autoconf_2.69-11.1.debian.tar.xz 23488 SHA256:ff76de2fc2956773dc6f47301b66822ea3074a2e556dc2e761cb411342d2228b
```

### `dpkg` source package: `automake-1.16=1:1.16.2-3ubuntu2`

Binary Packages:

- `automake=1:1.16.2-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/automake/copyright`)

- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris automake-1.16=1:1.16.2-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2-3ubuntu2.dsc' automake-1.16_1.16.2-3ubuntu2.dsc 1929 SHA256:c07f0ac1f2912803c28086aff355964335184e8e3dacd4592d5883a878693f4c
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2.orig.tar.xz' automake-1.16_1.16.2.orig.tar.xz 1545912 SHA256:ccc459de3d710e066ab9e12d2f119bd164a08c9341ca24ba22c9adaa179eedd0
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2.orig.tar.xz.asc' automake-1.16_1.16.2.orig.tar.xz.asc 833 SHA256:dbfc268276c94c95177f8e697d2688c944807c1284833a3e5354b78cd73ad8ab
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2-3ubuntu2.debian.tar.xz' automake-1.16_1.16.2-3ubuntu2.debian.tar.xz 13316 SHA256:ba3a4e824df618f280b30cae5e3a47fde95c9c4186c917fbefddb4f552292317
```

### `dpkg` source package: `autotools-dev=20180224.1`

Binary Packages:

- `autotools-dev=20180224.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.dsc' autotools-dev_20180224.1.dsc 1643 SHA256:795f558377bf6c90280c293b2711afc094cd1bf6ae486a395e1361ffd242cd2f
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.tar.xz' autotools-dev_20180224.1.tar.xz 68256 SHA256:355a4d8461dfedebd2c5194603197712a10f71e20de73a35ab6e90b7acf3e837
```

### `dpkg` source package: `base-files=11ubuntu10`

Binary Packages:

- `base-files=11ubuntu10`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `base-passwd=3.5.47`

Binary Packages:

- `base-passwd=3.5.47`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.47
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.dsc' base-passwd_3.5.47.dsc 1757 SHA256:5a77a4cce51d1eb72e9d96d4083c641435c05888922c7bd3fa6b4395bf9afad3
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.tar.xz' base-passwd_3.5.47.tar.xz 53024 SHA256:9810ae0216e96bf9fc7ca6163d47ef8ec7d1677f533451af5911d8202a490a23
```

### `dpkg` source package: `bash=5.0-6ubuntu2`

Binary Packages:

- `bash=5.0-6ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.0-6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu2.dsc' bash_5.0-6ubuntu2.dsc 2435 SHA256:711f1c8c971f993d91a1bde5b45dfe35309369792f9cfaa8be66cbe4e73f7a43
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA256:893858ba233d65bda38039e99dd96a4102b2f6a2d5e6c1c546e0794a60beed97
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu2.debian.tar.xz' bash_5.0-6ubuntu2.debian.tar.xz 74404 SHA256:bd139386937f508dbce82ac58f11e3aa1db25fe795223b3810d2d1005306a335
```

### `dpkg` source package: `binutils=2.35-2ubuntu1`

Binary Packages:

- `binutils=2.35-2ubuntu1`
- `binutils-common:amd64=2.35-2ubuntu1`
- `binutils-x86-64-linux-gnu=2.35-2ubuntu1`
- `libbinutils:amd64=2.35-2ubuntu1`
- `libctf-nobfd0:amd64=2.35-2ubuntu1`
- `libctf0:amd64=2.35-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.35-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.35-2ubuntu1.dsc' binutils_2.35-2ubuntu1.dsc 8767 SHA256:ff9d309e2cbabe891fd1c046de8af554ed3e5aacff71c1f7f7563fb505eced63
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.35.orig.tar.xz' binutils_2.35.orig.tar.xz 22042160 SHA256:1b11659fb49e20e18db460d44485f09442c8c56d5df165de9461eb09c8302f85
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.35-2ubuntu1.debian.tar.xz' binutils_2.35-2ubuntu1.debian.tar.xz 340240 SHA256:37007bb3df41b37c3bb55e379e7755d286f6f202674e6376f5c5181fabc8f794
```

### `dpkg` source package: `breezy=3.1.0-4`

Binary Packages:

- `brz=3.1.0-4`
- `python3-breezy=3.1.0-4`

Licenses: (parsed from: `/usr/share/doc/brz/copyright`, `/usr/share/doc/python3-breezy/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris breezy=3.1.0-4
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.1.0-4.dsc' breezy_3.1.0-4.dsc 2691 SHA256:61f352680600df2bcb96161969a2c043dd989e874213ff9f542c380da08f6022
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.1.0.orig.tar.gz' breezy_3.1.0.orig.tar.gz 9389366 SHA256:1eff207403f48898fa3b3ffa7a4275197c6c58fec105ef267caf1f5fd5a6c7be
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.1.0-4.debian.tar.xz' breezy_3.1.0-4.debian.tar.xz 55524 SHA256:e6c216d4fa8cb1f743dd75e328d02dc660a3cf10377b7481a48fc3489b4a2877
```

### `dpkg` source package: `brotli=1.0.7-7`

Binary Packages:

- `libbrotli-dev:amd64=1.0.7-7`
- `libbrotli1:amd64=1.0.7-7`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.7-7
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-7.dsc' brotli_1.0.7-7.dsc 2292 SHA256:454727e54cd7ca9d7d9360349bc9e42de390746ea51223d3a78861e5dbf93d37
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7.orig.tar.gz' brotli_1.0.7.orig.tar.gz 23827908 SHA256:4c61bfb0faca87219ea587326c467b95acb25555b53d1a421ffa3c8a9296ee2c
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-7.debian.tar.xz' brotli_1.0.7-7.debian.tar.xz 4700 SHA256:deea2090ec04b0c51b0e9867beb34c7d8f515027ad85ca1c45050957120b3392
```

### `dpkg` source package: `bzip2=1.0.8-4ubuntu2`

Binary Packages:

- `bzip2=1.0.8-4ubuntu2`
- `libbz2-1.0:amd64=1.0.8-4ubuntu2`
- `libbz2-dev:amd64=1.0.8-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu2.dsc' bzip2_1.0.8-4ubuntu2.dsc 2212 SHA256:bdb616a38932a65884c5f875939fda91ed3dc16c72ebe2c7f1c9c14a87e17943
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu2.debian.tar.bz2' bzip2_1.0.8-4ubuntu2.debian.tar.bz2 26561 SHA256:382004e27751494c67fb3ac7596b1521b690e40de087f1537bfef4ecfa2d7cb3
```

### `dpkg` source package: `bzr=2.7.0+bzr6622+brz`

Binary Packages:

- `bzr=2.7.0+bzr6622+brz`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.7.0+bzr6622+brz
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622+brz.dsc' bzr_2.7.0+bzr6622+brz.dsc 1866 SHA256:2c1d9f13818b32fbc5dc41d395b91101e2d1b451eae358ffdf83421521dbe670
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622+brz.tar.xz' bzr_2.7.0+bzr6622+brz.tar.xz 18052 SHA256:d847a018e4869b59e9bfc04b0ff3705dcbb5479a8b6796c2dd68e60be3753a42
```

### `dpkg` source package: `ca-certificates=20200601`

Binary Packages:

- `ca-certificates=20200601`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20200601
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20200601.dsc' ca-certificates_20200601.dsc 1582 SHA256:4c18f8be89824bc7e4c51895e513b0d8b748ea84e8190571aa4126ad9dcdd1fe
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20200601.tar.xz' ca-certificates_20200601.tar.xz 245668 SHA256:43766d5a436519503dfd65ab83488ae33ab4d4ca3d0993797b58c92eb9ed4e63
```

### `dpkg` source package: `cairo=1.16.0-4ubuntu1`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-4ubuntu1`
- `libcairo-script-interpreter2:amd64=1.16.0-4ubuntu1`
- `libcairo2:amd64=1.16.0-4ubuntu1`
- `libcairo2-dev:amd64=1.16.0-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-4ubuntu1.dsc' cairo_1.16.0-4ubuntu1.dsc 2950 SHA256:f53596e412c2e1799d5e7e1c414d7db2cade33ba85fd912d39f60525b5a2e23b
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA256:5e7b29b3f113ef870d1e3ecf8adf21f923396401604bda16d44be45e66052331
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-4ubuntu1.debian.tar.xz' cairo_1.16.0-4ubuntu1.debian.tar.xz 30416 SHA256:3725774f0a3f244a8b910e5a5e46bc731ee87372c6effb6c5af2d0db65c64426
```

### `dpkg` source package: `cdebconf=0.252ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.252ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.252ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.252ubuntu1.dsc' cdebconf_0.252ubuntu1.dsc 2865 SHA256:4e851f7f8f6201fdbfe4257ef0b7302fa36b7a89e5b0f209905b92473adce261
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.252ubuntu1.tar.xz' cdebconf_0.252ubuntu1.tar.xz 276852 SHA256:852f565190ad2cc902f041d6eaf587ea8a100f1facebb004b13b0043a2590e7a
```

### `dpkg` source package: `configobj=5.0.6-4`

Binary Packages:

- `python3-configobj=5.0.6-4`

Licenses: (parsed from: `/usr/share/doc/python3-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-4
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-4.dsc' configobj_5.0.6-4.dsc 2246 SHA256:74df72d8fdb3c20e4bc5ab996bf1f8c6297811643989110cc27a019e7beb0429
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA256:2e140354efcca6f558ff9ee941b435ae09a617bc071797bef62c8d6ed2033d5e
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-4.debian.tar.xz' configobj_5.0.6-4.debian.tar.xz 6916 SHA256:dd20992aeef0eb1fb8ab6f0007e265ece33cfc20a6ca18b380eb255674195f01
```

### `dpkg` source package: `coreutils=8.32-3ubuntu1`

Binary Packages:

- `coreutils=8.32-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.32-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-3ubuntu1.dsc' coreutils_8.32-3ubuntu1.dsc 2011 SHA256:c22e6929fd112dfab109d7fbcc0225ba4955b758f6e56a54cea31b4438b71c6f
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz' coreutils_8.32.orig.tar.xz 5547836 SHA256:4458d8de7849df44ccab15e16b1548b285224dbba5f08fac070c1c0e0bcc4cfa
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-3ubuntu1.debian.tar.xz' coreutils_8.32-3ubuntu1.debian.tar.xz 40716 SHA256:c7b6a8b93cbe1d6c45aa6879f5c2aefa8ff2fa5f1087d5ea38b6c51a4612550d
```

### `dpkg` source package: `curl=7.68.0-1ubuntu4`

Binary Packages:

- `curl=7.68.0-1ubuntu4`
- `libcurl3-gnutls:amd64=7.68.0-1ubuntu4`
- `libcurl4:amd64=7.68.0-1ubuntu4`
- `libcurl4-openssl-dev:amd64=7.68.0-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.68.0-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu4.dsc' curl_7.68.0-1ubuntu4.dsc 2725 SHA256:af0de15a54041c751a39e0b0c38e6db199377255cfb0f8138cb70ef8138ba913
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0.orig.tar.gz' curl_7.68.0.orig.tar.gz 4096350 SHA256:1dd7604e418b0b9a9077f62f763f6684c1b092a7bc17e3f354b8ad5c964d7358
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu4.debian.tar.xz' curl_7.68.0-1ubuntu4.debian.tar.xz 33456 SHA256:2749db42eeb45152a9bf6ec48e7e2689f9a288615592aa92d8e13af0eb70e195
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.dsc' cyrus-sasl2_2.1.27+dfsg-2.dsc 3393 SHA256:e7e09491a1c2589c9947164db091d0f9b21b7d122f128841b6eac1adfc51b6c2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz 99956 SHA256:ee894aeee645e842e39b434d5130e1bd15ea24b84c8eeeea3f5077511a87341a
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-7.dsc' dash_0.5.10.2-7.dsc 1762 SHA256:477515a7d980127657c9760f1a53b0175b79455acfd9d92284a6c563971523ea
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA256:3c663919dc5c66ec991da14c7cf7e0be8ad00f3db73986a987c118862b5f6071
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-7.debian.tar.xz' dash_0.5.10.2-7.debian.tar.xz 45336 SHA256:ba76b70008e95a88f1f2860bc74bea9fd6732df179dbb126706d51cfede713c1
```

### `dpkg` source package: `db-defaults=1:5.3.21~exp1ubuntu2`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21~exp1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21~exp1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.dsc' db-defaults_5.3.21~exp1ubuntu2.dsc 2044 SHA256:1960179af0244d410f368653e32d594c8e9331e2046422d05c33edc7f0d248b6
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.tar.xz' db-defaults_5.3.21~exp1ubuntu2.tar.xz 3032 SHA256:03c2bba2824a4f5042960a4712630e35d2cbf885a22d24f2b27b2ca28ad6f46a
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6ubuntu2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6ubuntu2`
- `libdb5.3-dev=5.3.28+dfsg1-0.6ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu2.dsc' db5.3_5.3.28+dfsg1-0.6ubuntu2.dsc 3245 SHA256:d879f4921a2f573132031d9371f0eb020005bdce48d6e12b436bf3515dda8663
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu2.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6ubuntu2.debian.tar.xz 30172 SHA256:e606e7827f077efc92afc6f0d43c921fab4577d619eab06fab23182aefab7506
```

### `dpkg` source package: `debconf=1.5.74`

Binary Packages:

- `debconf=1.5.74`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.74
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.dsc' debconf_1.5.74.dsc 2082 SHA256:7576b8798165e30aaea23bad812eec729dd091a1ca59063328e7f68223b79af1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.tar.xz' debconf_1.5.74.tar.xz 571108 SHA256:11b3fa02ddafe813c301aa150fef4d510d77afa64cbfe09c7e614995147c48e0
```

### `dpkg` source package: `debianutils=4.11`

Binary Packages:

- `debianutils=4.11`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debianutils/4.11/


### `dpkg` source package: `diffutils=1:3.7-3build1`

Binary Packages:

- `diffutils=1:3.7-3build1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.7-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3build1.dsc' diffutils_3.7-3build1.dsc 1901 SHA256:aa6d33da42464b8771136469464af878b2f58ece23eed4b886a9d76599cda7ec
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz' diffutils_3.7.orig.tar.xz 1448828 SHA256:b3a7a6221c3dc916085f0d205abf6b8e1ba443d4dd965118da364a1dc1cb3a26
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3build1.debian.tar.xz' diffutils_3.7-3build1.debian.tar.xz 11252 SHA256:a63b2b4ff5560715724a810eae4104ea59417914be92942c5cf31e4ea8dbc04a
```

### `dpkg` source package: `djvulibre=3.5.27.1-15`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.27.1-15`
- `libdjvulibre-text=3.5.27.1-15`
- `libdjvulibre21:amd64=3.5.27.1-15`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-15
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-15.dsc' djvulibre_3.5.27.1-15.dsc 2406 SHA256:19ca8e31fdebdd50d42623a05d8936bd1402669487b083419f000eceb54eef3a
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA256:77f07de3f1039aa19eba2eb3170d9ce9a0918ba7b704a59cfaf08f42fcc52144
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-15.debian.tar.xz' djvulibre_3.5.27.1-15.debian.tar.xz 80508 SHA256:bc2a4c3df8a412292f5d5096306b3a40a12cb0e5be773efd0a874aef7be477bb
```

### `dpkg` source package: `dpkg=1.20.5ubuntu1`

Binary Packages:

- `dpkg=1.20.5ubuntu1`
- `dpkg-dev=1.20.5ubuntu1`
- `libdpkg-perl=1.20.5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.20.5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.20.5ubuntu1.dsc' dpkg_1.20.5ubuntu1.dsc 2260 SHA256:32cc43155846b03a037b407bbb94d68d9643bb8f793a55a78fb40797d40de84f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.20.5ubuntu1.tar.xz' dpkg_1.20.5ubuntu1.tar.xz 4743268 SHA256:472dcb374e01b2428d6f4bfed6df4b26a4ca9f2c8355df23cf69876f59b59b17
```

### `dpkg` source package: `dulwich=0.19.15-1build1`

Binary Packages:

- `python3-dulwich=0.19.15-1build1`

Licenses: (parsed from: `/usr/share/doc/python3-dulwich/copyright`)

- `Apache-2`
- `Apache-2.0`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dulwich=0.19.15-1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15-1build1.dsc' dulwich_0.19.15-1build1.dsc 2410 SHA256:5a742485cfbf473aeefab144351af69662ab867ab016e5c3541aad6efddfa00c
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15.orig.tar.gz' dulwich_0.19.15.orig.tar.gz 369491 SHA256:805a9b1932dc28b91f359f529c2e46b7623aec3ab719c96d3f2fc63d0d8d8411
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15-1build1.debian.tar.xz' dulwich_0.19.15-1build1.debian.tar.xz 631088 SHA256:6fddcf432f17d8512cafbc8f7bac2e94f54bd7843a820af64e0fe010413e8a5f
```

### `dpkg` source package: `e2fsprogs=1.45.6-1ubuntu1`

Binary Packages:

- `comerr-dev:amd64=2.1-1.45.6-1ubuntu1`
- `e2fsprogs=1.45.6-1ubuntu1`
- `libcom-err2:amd64=1.45.6-1ubuntu1`
- `libext2fs2:amd64=1.45.6-1ubuntu1`
- `libss2:amd64=1.45.6-1ubuntu1`
- `logsave=1.45.6-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.6-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.dsc' e2fsprogs_1.45.6-1ubuntu1.dsc 3328 SHA256:1a4832b1d2bd4a17121bd89fa51ba192e17ad7153da9d16a475fad5b3fa2bf66
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz' e2fsprogs_1.45.6.orig.tar.gz 7938544 SHA256:5f64ac50a2b60b8e67c5b382bb137dec39344017103caffc3a61554424f2d693
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz.asc' e2fsprogs_1.45.6.orig.tar.gz.asc 488 SHA256:831c29bd04c5b21faf2aa2d5fa3b409148973e3ef0d15f67315a5c429180d945
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz' e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz 81276 SHA256:dacb658bcf1b0f7728ddc7f956494d6d414b70e97d45b22c91df24fec01248cc
```

### `dpkg` source package: `elfutils=0.180-1`

Binary Packages:

- `libelf1:amd64=0.180-1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.180-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.180-1.dsc' elfutils_0.180-1.dsc 2810 SHA256:21325074457d6d02da421a81a00c676da4bced72c5f3abaae77c05a636b517e9
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.180.orig.tar.bz2' elfutils_0.180.orig.tar.bz2 9079640 SHA256:b827b6e35c59d188ba97d7cf148fa8dc6f5c68eb6c5981888dfdbb758c0b569d
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.180-1.debian.tar.xz' elfutils_0.180-1.debian.tar.xz 33016 SHA256:2049e6fff637816cf7bbf93a9d2e67514f71758c354c61c8b032e9bc13119d0b
```

### `dpkg` source package: `expat=2.2.9-1build1`

Binary Packages:

- `libexpat1:amd64=2.2.9-1build1`
- `libexpat1-dev:amd64=2.2.9-1build1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.9-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.dsc' expat_2.2.9-1build1.dsc 1998 SHA256:9f2d2e3bf2aec22907e3bf818fac7acc5f1e917821907bdea016f69a5cfe4da0
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9.orig.tar.gz' expat_2.2.9.orig.tar.gz 8273174 SHA256:c341ac8c79e021cc3392a6d76e138e62d1dd287592cb455148540331756a2208
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.debian.tar.xz' expat_2.2.9-1build1.debian.tar.xz 10780 SHA256:400872937adfb41255914391a172237cfe317e57f129562ff2ec66773b2b5bbf
```

### `dpkg` source package: `fftw3=3.3.8-2ubuntu6`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu6.dsc' fftw3_3.3.8-2ubuntu6.dsc 3010 SHA256:412fa277f765c7751b61fa096ef2525704432788321a21a0aba8b000375b4ad6
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA256:6113262f6e92c5bd474f2875fa1b01054c4ad5040f6b0da7c03c98821d9ae303
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu6.debian.tar.xz' fftw3_3.3.8-2ubuntu6.debian.tar.xz 14208 SHA256:a3e961688653dd276b74afe38552767205c512c0c90a741d629e84f3f1030f36
```

### `dpkg` source package: `file=1:5.38-5`

Binary Packages:

- `file=1:5.38-5`
- `libmagic-mgc=1:5.38-5`
- `libmagic1:amd64=1:5.38-5`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.38-5
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38-5.dsc' file_5.38-5.dsc 2237 SHA256:277850accb24add1151e2d24896d7db989a80be007dd8d244ba1ef4dff821043
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38.orig.tar.gz' file_5.38.orig.tar.gz 932528 SHA256:593c2ffc2ab349c5aea0f55fedfe4d681737b6b62376a9b3ad1e77b2cc19fa34
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38.orig.tar.gz.asc' file_5.38.orig.tar.gz.asc 169 SHA256:b9c78e39970abda091ec8752401f5241349cef4709a2e1267a378f7ab25115d8
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38-5.debian.tar.xz' file_5.38-5.debian.tar.xz 35120 SHA256:6f6d89ee23af5a81a989d53c25c5f5d8403ace5f9755453c72e75a49d3693cdb
```

### `dpkg` source package: `findutils=4.7.0-1ubuntu1`

Binary Packages:

- `findutils=4.7.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.7.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu1.dsc' findutils_4.7.0-1ubuntu1.dsc 2446 SHA256:3d157948919082e66cb74e0f927efa3dd240d9fa9814973874d0fa77f3023ead
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz' findutils_4.7.0.orig.tar.xz 1895048 SHA256:c5fefbdf9858f7e4feb86f036e1247a54c79fc2d8e4b7064d5aaa1f47dfa789a
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz.asc' findutils_4.7.0.orig.tar.xz.asc 488 SHA256:2f620e6d941e241fac52344a89149ab1ffeefb0fb9e42174e17a508d59a31d0f
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu1.debian.tar.xz' findutils_4.7.0-1ubuntu1.debian.tar.xz 27700 SHA256:dfb2329fd141384c2d76409c2e99f164cc25954115529245d80d5d41e3167731
```

### `dpkg` source package: `fontconfig=2.13.1-2ubuntu3`

Binary Packages:

- `fontconfig=2.13.1-2ubuntu3`
- `fontconfig-config=2.13.1-2ubuntu3`
- `libfontconfig1:amd64=2.13.1-2ubuntu3`
- `libfontconfig1-dev:amd64=2.13.1-2ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-2ubuntu3.dsc' fontconfig_2.13.1-2ubuntu3.dsc 1959 SHA256:a9eebf6e6e88aa64d33fb3852c97718c212579f9714afd67cb6a9b8b116dd7aa
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA256:f655dd2a986d7aa97e052261b36aa67b0a64989496361eca8d604e6414006741
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-2ubuntu3.debian.tar.xz' fontconfig_2.13.1-2ubuntu3.debian.tar.xz 26344 SHA256:342671f6a1e6d392958a6eec27541c6bdffc6498b469dcc46eca66c9d23a863a
```

### `dpkg` source package: `fonts-dejavu=2.37-2`

Binary Packages:

- `fonts-dejavu-core=2.37-2`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.dsc' fonts-dejavu_2.37-2.dsc 2387 SHA256:13948768dbf1a9aa3ae9fe592a4c6c904b1dd075acb689a49b85e0ae73b1756c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.debian.tar.xz' fonts-dejavu_2.37-2.debian.tar.xz 11408 SHA256:428cf37685df891574d2dcb32aa9366e4e95985fda7d87069903313bb03470ab
```

### `dpkg` source package: `freetype=2.10.2+dfsg-3`

Binary Packages:

- `libfreetype-dev:amd64=2.10.2+dfsg-3`
- `libfreetype6:amd64=2.10.2+dfsg-3`
- `libfreetype6-dev:amd64=2.10.2+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

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
$ apt-get source -qq --print-uris freetype=2.10.2+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg-3.dsc' freetype_2.10.2+dfsg-3.dsc 3680 SHA256:d91c8e350849462dc7fa93bf551c714653dfcbdb82ed7a45f1ecd414475c301b
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2demos.tar.xz' freetype_2.10.2+dfsg.orig-ft2demos.tar.xz 230672 SHA256:3dce65d1ba53d48659688549175765ee163d645b73db7055a3c43a7c882d6daa
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2demos.tar.xz.asc' freetype_2.10.2+dfsg.orig-ft2demos.tar.xz.asc 195 SHA256:0a11f56569a589c9f52a3e60e491aeed566d040f51435082891d6551d6d66338
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2docs.tar.xz' freetype_2.10.2+dfsg.orig-ft2docs.tar.xz 2078712 SHA256:22b9584040a2e3c4387b5998cb9b4340183888eef15c2ac0fd9115cad837cf91
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2docs.tar.xz.asc' freetype_2.10.2+dfsg.orig-ft2docs.tar.xz.asc 195 SHA256:4be0f469d29086486df1ace563b9536e1be34d603e311f89a38b3fef99a9f115
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig.tar.xz' freetype_2.10.2+dfsg.orig.tar.xz 2246904 SHA256:c1f32cbb42a1519ae7d69046d84d359f44bfdea15c800c4f0b60a36c78b46d70
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg-3.debian.tar.xz' freetype_2.10.2+dfsg-3.debian.tar.xz 116212 SHA256:7adcb9c757025deaa295f776787c8dc529d9ddfe30791862d476b73170782013
```

### `dpkg` source package: `fribidi=1.0.8-2`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.dsc' fribidi_1.0.8-2.dsc 1987 SHA256:f1b396620cda57e93799725abad47089902429295f7b3555bc3d5b3f00a79340
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA256:94c7b68d86ad2a9613b4dcffe7bbeb03523d63b5b37918bdf2e4ef34195c1e6c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.debian.tar.xz' fribidi_1.0.8-2.debian.tar.xz 8980 SHA256:898fc0b48625ce31e29d2f9501f17b9991b16b03816db6467faaedb85d22f00b
```

### `dpkg` source package: `gcc-10=10.2.0-5ubuntu2`

Binary Packages:

- `cpp-10=10.2.0-5ubuntu2`
- `g++-10=10.2.0-5ubuntu2`
- `gcc-10=10.2.0-5ubuntu2`
- `gcc-10-base:amd64=10.2.0-5ubuntu2`
- `libasan6:amd64=10.2.0-5ubuntu2`
- `libatomic1:amd64=10.2.0-5ubuntu2`
- `libcc1-0:amd64=10.2.0-5ubuntu2`
- `libgcc-10-dev:amd64=10.2.0-5ubuntu2`
- `libgcc-s1:amd64=10.2.0-5ubuntu2`
- `libgomp1:amd64=10.2.0-5ubuntu2`
- `libitm1:amd64=10.2.0-5ubuntu2`
- `liblsan0:amd64=10.2.0-5ubuntu2`
- `libquadmath0:amd64=10.2.0-5ubuntu2`
- `libstdc++-10-dev:amd64=10.2.0-5ubuntu2`
- `libstdc++6:amd64=10.2.0-5ubuntu2`
- `libtsan0:amd64=10.2.0-5ubuntu2`
- `libubsan1:amd64=10.2.0-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/cpp-10/copyright`, `/usr/share/doc/g++-10/copyright`, `/usr/share/doc/gcc-10/copyright`, `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-10-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-10-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.2.0-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10.2.0-5ubuntu2.dsc' gcc-10_10.2.0-5ubuntu2.dsc 30426 SHA256:c0497cd654a993b6e4ead66239235c71cf6ff27534ad1b9026591d119e110472
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10.2.0.orig.tar.gz' gcc-10_10.2.0.orig.tar.gz 94773960 SHA256:8c932c6527c2d53eebea682092591b701a79901d9f308697f2cf8d443578ac40
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10.2.0-5ubuntu2.debian.tar.xz' gcc-10_10.2.0-5ubuntu2.debian.tar.xz 2024860 SHA256:fd9026959db5bb113dded9a8e96b5bcfd34590eb66b1d1b6846b526af2815986
```

### `dpkg` source package: `gcc-defaults=1.188ubuntu1`

Binary Packages:

- `cpp=4:10.1.0-1ubuntu1`
- `g++=4:10.1.0-1ubuntu1`
- `gcc=4:10.1.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.188ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.188ubuntu1.dsc' gcc-defaults_1.188ubuntu1.dsc 16619 SHA256:abf26d53219fbdc60fb91bcdfdf3300b1a59525a4d0bd35803c83b9d4c038e4c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.188ubuntu1.tar.xz' gcc-defaults_1.188ubuntu1.tar.xz 48416 SHA256:aba102c94d659916b851ac811c4c00e4edcc98e236ecf57b89fafc0e262e9f38
```

### `dpkg` source package: `gdbm=1.18.1-5`

Binary Packages:

- `libgdbm-compat4:amd64=1.18.1-5`
- `libgdbm-dev:amd64=1.18.1-5`
- `libgdbm6:amd64=1.18.1-5`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gdbm/1.18.1-5/


### `dpkg` source package: `gdk-pixbuf=2.40.0+dfsg-5`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-0:amd64=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-bin=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-common=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-dev:amd64=2.40.0+dfsg-5`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.40.0+dfsg-5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-5.dsc' gdk-pixbuf_2.40.0+dfsg-5.dsc 3069 SHA256:67b878bfda43b1d17b8882916e1f5b05849dc8f37a429b1cdc69f16998ad51e0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg.orig.tar.xz' gdk-pixbuf_2.40.0+dfsg.orig.tar.xz 5626144 SHA256:bdb3820005dc3c02ec8b1e2916a1d060f65f44d30ba48ab88704c3380d5a47b8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-5.debian.tar.xz' gdk-pixbuf_2.40.0+dfsg-5.debian.tar.xz 17932 SHA256:a830ae3b8f64e6c62a169514e2faf26d091c8cfaa244eed15f55f968bc312df3
```

### `dpkg` source package: `git=1:2.27.0-1ubuntu1`

Binary Packages:

- `git=1:2.27.0-1ubuntu1`
- `git-man=1:2.27.0-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.27.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0-1ubuntu1.dsc' git_2.27.0-1ubuntu1.dsc 2991 SHA256:fcd999d6ed543017ec0b9858e35e93900cf30dc13bc09138512dfb776c0eb18b
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0.orig.tar.xz' git_2.27.0.orig.tar.xz 6074636 SHA256:73ca9774d7fa226e1d87c1909401623f96dca6a044e583b9a762e84d7d1a73f9
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0-1ubuntu1.debian.tar.xz' git_2.27.0-1ubuntu1.debian.tar.xz 652712 SHA256:7fd6f399e6c8826874515eadccdd88c21bf1a9951fbc92a4f347f1f3c41be11a
```

### `dpkg` source package: `glib2.0=2.64.4-1`

Binary Packages:

- `libglib2.0-0:amd64=2.64.4-1`
- `libglib2.0-bin=2.64.4-1`
- `libglib2.0-data=2.64.4-1`
- `libglib2.0-dev:amd64=2.64.4-1`
- `libglib2.0-dev-bin=2.64.4-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.64.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.4-1.dsc' glib2.0_2.64.4-1.dsc 3328 SHA256:0cb06c20a4a7da393d7d17cd1fee0ecbe0efd41d3948a52442d003754fecc482
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.4.orig.tar.xz' glib2.0_2.64.4.orig.tar.xz 4779456 SHA256:f7e0b325b272281f0462e0f7fff25a833820cac19911ff677251daf6d87bce50
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.4-1.debian.tar.xz' glib2.0_2.64.4-1.debian.tar.xz 93700 SHA256:40db69d7d2013fb2a04017163dd16525f9c4c3a44d48e400ff8fa00083eaf7c5
```

### `dpkg` source package: `glibc=2.31-0ubuntu10`

Binary Packages:

- `libc-bin=2.31-0ubuntu10`
- `libc-dev-bin=2.31-0ubuntu10`
- `libc6:amd64=2.31-0ubuntu10`
- `libc6-dev:amd64=2.31-0ubuntu10`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.31-0ubuntu10
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu10.dsc' glibc_2.31-0ubuntu10.dsc 9309 SHA256:e96042f2807662ddf9288334ea0a3eddc874e46af25018cc5bbc3d29fd7b6cec
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31.orig.tar.xz' glibc_2.31.orig.tar.xz 17317924 SHA256:2b22c7b04a36747d6c74796a73193a6f8856bfd1efc551b5db96baefa053fe5e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu10.debian.tar.xz' glibc_2.31-0ubuntu10.debian.tar.xz 859544 SHA256:74db110b2e22a9e64200f2c453b288298eadb7d86e098cb35cb96138d3746e50
```

### `dpkg` source package: `gmp=2:6.2.0+dfsg-6ubuntu1`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.0+dfsg-6ubuntu1`
- `libgmp10:amd64=2:6.2.0+dfsg-6ubuntu1`
- `libgmpxx4ldbl:amd64=2:6.2.0+dfsg-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.0+dfsg-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6ubuntu1.dsc' gmp_6.2.0+dfsg-6ubuntu1.dsc 2230 SHA256:a7e3e867ba756fce1c1994b8b12e98b189e1af9b7024663e47de9b8a345ce40b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg.orig.tar.xz' gmp_6.2.0+dfsg.orig.tar.xz 1842912 SHA256:5d7610449498a79aa62d4b9a8f6baaef91b8716726e1009e02b879962dff32ab
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6ubuntu1.debian.tar.xz' gmp_6.2.0+dfsg-6ubuntu1.debian.tar.xz 54484 SHA256:1da24eddd3a6e5ef02dd8c87644f62a291b2ac93f7c66fc86a2e5aa258a64d04
```

### `dpkg` source package: `gnupg2=2.2.20-1ubuntu1`

Binary Packages:

- `dirmngr=2.2.20-1ubuntu1`
- `gnupg=2.2.20-1ubuntu1`
- `gnupg-l10n=2.2.20-1ubuntu1`
- `gnupg-utils=2.2.20-1ubuntu1`
- `gpg=2.2.20-1ubuntu1`
- `gpg-agent=2.2.20-1ubuntu1`
- `gpg-wks-client=2.2.20-1ubuntu1`
- `gpg-wks-server=2.2.20-1ubuntu1`
- `gpgconf=2.2.20-1ubuntu1`
- `gpgsm=2.2.20-1ubuntu1`
- `gpgv=2.2.20-1ubuntu1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.20-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu1.dsc' gnupg2_2.2.20-1ubuntu1.dsc 3971 SHA256:f864b21a847e820057a504fa067f4154ecf47487c8cea08bec1646460d7ea9e7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2' gnupg2_2.2.20.orig.tar.bz2 6786913 SHA256:04a7c9d48b74c399168ee8270e548588ddbe52218c337703d7f06373d326ca30
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2.asc' gnupg2_2.2.20.orig.tar.bz2.asc 1357 SHA256:be34b9959fa4c9baa7269b1c7c695808d6b999ba47f28c614312dd3d8d47ca79
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu1.debian.tar.xz' gnupg2_2.2.20-1ubuntu1.debian.tar.xz 64332 SHA256:2232fdbe9b2a4a55613a6b33d4bc8a8959474fbb675dae137c7e4f192cf941de
```

### `dpkg` source package: `gnutls28=3.6.13-4ubuntu4`

Binary Packages:

- `libgnutls30:amd64=3.6.13-4ubuntu4`

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
$ apt-get source -qq --print-uris gnutls28=3.6.13-4ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13-4ubuntu4.dsc' gnutls28_3.6.13-4ubuntu4.dsc 3586 SHA256:bfe7295eae5f906146bfb962f50d7a02e0998c7de042f70bd4ab8732027693a3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13.orig.tar.xz' gnutls28_3.6.13.orig.tar.xz 5958956 SHA256:32041df447d9f4644570cf573c9f60358e865637d69b7e59d1159b7240b52f38
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13.orig.tar.xz.asc' gnutls28_3.6.13.orig.tar.xz.asc 667 SHA256:79eb677b19a35de2f17d2ea87e863755cd53f0072b9435c8a4b57669360f57d0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13-4ubuntu4.debian.tar.xz' gnutls28_3.6.13-4ubuntu4.debian.tar.xz 71076 SHA256:48d1ef66b94d73a3e8386fba9fe68e3218b10220159c9dd3d1c5f3d5dad4d681
```

### `dpkg` source package: `gobject-introspection=1.64.1-1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.64.1-1`
- `gir1.2-glib-2.0:amd64=1.64.1-1`
- `libgirepository-1.0-1:amd64=1.64.1-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.64.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.64.1-1.dsc' gobject-introspection_1.64.1-1.dsc 3088 SHA256:d5f522e9e605b07b94ae1ddcc3ba744c6726d61718a5f509b7e39a41440d3a0d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.64.1.orig.tar.xz' gobject-introspection_1.64.1.orig.tar.xz 1000280 SHA256:80beae6728c134521926affff9b2e97125749b38d38744dc901f4010ee3e7fa7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.64.1-1.debian.tar.xz' gobject-introspection_1.64.1-1.debian.tar.xz 23348 SHA256:5bcb9e66815cf376b50cfba4c5f275faf21c46c4e27bf06bbc2452c1707bc408
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1.dsc' graphite2_1.3.14-1.dsc 2608 SHA256:3a622b8aa7d693d6d60d3cd29b49a7d9d7873ea6089cb52ce7a223261e605152
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14.orig.tar.gz' graphite2_1.3.14.orig.tar.gz 6629829 SHA256:7a3b342c5681921ce2e0c2496509d30b5b078399d5a7bd2358f95166d57d91df
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1.debian.tar.xz' graphite2_1.3.14-1.debian.tar.xz 12068 SHA256:94d584e6c748fa7e2f851c3bb39cb2cdb437b4f91d1d636f3d842357724cd9bd
```

### `dpkg` source package: `grep=3.4-1`

Binary Packages:

- `grep=3.4-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.dsc' grep_3.4-1.dsc 1674 SHA256:785f527cede9631f075bdd6c7f35e65e6b82897d009682766cf35839a393277d
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz' grep_3.4.orig.tar.xz 1555820 SHA256:58e6751c41a7c25bfc6e9363a41786cff3ba5709cf11d5ad903cf7cce31cc3fb
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz.asc' grep_3.4.orig.tar.xz.asc 833 SHA256:4c1871ff6b79c5e5ce0a192272c171d06ec20762b4b258688b1ca2e47d94b23e
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.debian.tar.xz' grep_3.4-1.debian.tar.xz 104364 SHA256:582d181804ce72fcfc4c6a9f13ea1dd73ad04c2723b5da346b69ee5cd24a7d08
```

### `dpkg` source package: `gzip=1.10-2ubuntu1`

Binary Packages:

- `gzip=1.10-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-2ubuntu1.dsc' gzip_1.10-2ubuntu1.dsc 2074 SHA256:bdac8e876b858094311a611b4e69a179fc67a78158c5f59f53b8269bafb4e568
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA256:c91f74430bf7bc20402e1f657d0b252cb80aa66ba333a25704512af346633c68
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-2ubuntu1.debian.tar.xz' gzip_1.10-2ubuntu1.debian.tar.xz 33288 SHA256:23d03e6a7f9cf9b7daf506eaf922ccddda85dfc2827cf48da72d2086608872ef
```

### `dpkg` source package: `harfbuzz=2.6.4-1ubuntu5`

Binary Packages:

- `libharfbuzz0b:amd64=2.6.4-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.6.4-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4-1ubuntu5.dsc' harfbuzz_2.6.4-1ubuntu5.dsc 2841 SHA256:aab39e97e3c186623b53e0a699d04873637e146bea7465d0bf9d8bd623a94fab
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4.orig.tar.xz' harfbuzz_2.6.4.orig.tar.xz 5967468 SHA256:9413b8d96132d699687ef914ebb8c50440efc87b3f775d25856d7ec347c03c12
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4-1ubuntu5.debian.tar.xz' harfbuzz_2.6.4-1ubuntu5.debian.tar.xz 11388 SHA256:1723f96e60fc93a7fbfab84c20fc8e337d25823dd3e310bed84cb097e0891a08
```

### `dpkg` source package: `heimdal=7.7.0+dfsg-2`

Binary Packages:

- `libasn1-8-heimdal:amd64=7.7.0+dfsg-2`
- `libgssapi3-heimdal:amd64=7.7.0+dfsg-2`
- `libhcrypto4-heimdal:amd64=7.7.0+dfsg-2`
- `libheimbase1-heimdal:amd64=7.7.0+dfsg-2`
- `libheimntlm0-heimdal:amd64=7.7.0+dfsg-2`
- `libhx509-5-heimdal:amd64=7.7.0+dfsg-2`
- `libkrb5-26-heimdal:amd64=7.7.0+dfsg-2`
- `libroken18-heimdal:amd64=7.7.0+dfsg-2`
- `libwind0-heimdal:amd64=7.7.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libasn1-8-heimdal/copyright`, `/usr/share/doc/libgssapi3-heimdal/copyright`, `/usr/share/doc/libhcrypto4-heimdal/copyright`, `/usr/share/doc/libheimbase1-heimdal/copyright`, `/usr/share/doc/libheimntlm0-heimdal/copyright`, `/usr/share/doc/libhx509-5-heimdal/copyright`, `/usr/share/doc/libkrb5-26-heimdal/copyright`, `/usr/share/doc/libroken18-heimdal/copyright`, `/usr/share/doc/libwind0-heimdal/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `custom`
- `none`

Source:

```console
$ apt-get source -qq --print-uris heimdal=7.7.0+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.dsc' heimdal_7.7.0+dfsg-2.dsc 3580 SHA256:cd71bc63686f11909d68bce45a9ea1c7ecb8f08b71eb2d39fc6906c4b7f406fb
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg.orig.tar.xz' heimdal_7.7.0+dfsg.orig.tar.xz 5945252 SHA256:6822c9547188b753b6325047fda9255744e4ebbbe02bb0dade78c261061fefac
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.debian.tar.xz' heimdal_7.7.0+dfsg-2.debian.tar.xz 128660 SHA256:076c9b6d91ce69f760ce8812d5737bdf03fc5b1fd2b1ac401f18fda4bbd31055
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

### `dpkg` source package: `hostname=3.23`

Binary Packages:

- `hostname=3.23`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.dsc' hostname_3.23.dsc 1402 SHA256:0694c083fad82da1fd33204557a30bfc745a689a64030ba360062daafe03ede0
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.tar.gz' hostname_3.23.tar.gz 13672 SHA256:bc6d1954b22849869ff8b2a602e39f08b1702f686d4b58dd7927cdeb5b4876ef
```

### `dpkg` source package: `icu=67.1-3ubuntu1`

Binary Packages:

- `icu-devtools=67.1-3ubuntu1`
- `libicu-dev:amd64=67.1-3ubuntu1`
- `libicu67:amd64=67.1-3ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ilmbase=2.3.0-6build1`

Binary Packages:

- `libilmbase-dev:amd64=2.3.0-6build1`
- `libilmbase24:amd64=2.3.0-6build1`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase24/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.3.0-6build1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0-6build1.dsc' ilmbase_2.3.0-6build1.dsc 2367 SHA256:2164e2cff01f17f030b456c2d0920d09461ae76229507459a73cf7c618d4f7f6
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0.orig.tar.gz' ilmbase_2.3.0.orig.tar.gz 596749 SHA256:0ea21166799bbdd920e7a38a7026236566aafdd6e8638f54c9da1af2219fae82
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0.orig.tar.gz.asc' ilmbase_2.3.0.orig.tar.gz.asc 566 SHA256:c7ee3f4432322d4f7c63dd1b0ca2188a8d1c4a018821c3c12a3d9db746b54bee
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0-6build1.debian.tar.xz' ilmbase_2.3.0-6build1.debian.tar.xz 14252 SHA256:1039258f50fda2e94e4dac23e1e8aa702d8e3e83d0e1f12f13a652eadf2ebbf3
```

### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu12`

Binary Packages:

- `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu12`
- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1ubuntu12`
- `imagemagick-6.q16=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6-arch-config:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6-headers=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-dev=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-6-headers=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-dev=8:6.9.10.23+dfsg-2.1ubuntu12`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/libmagickcore-6-arch-config/copyright`, `/usr/share/doc/libmagickcore-6-headers/copyright`, `/usr/share/doc/libmagickcore-6.q16-6/copyright`, `/usr/share/doc/libmagickcore-6.q16-6-extra/copyright`, `/usr/share/doc/libmagickcore-6.q16-dev/copyright`, `/usr/share/doc/libmagickcore-dev/copyright`, `/usr/share/doc/libmagickwand-6-headers/copyright`, `/usr/share/doc/libmagickwand-6.q16-6/copyright`, `/usr/share/doc/libmagickwand-6.q16-dev/copyright`, `/usr/share/doc/libmagickwand-dev/copyright`)

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.10.23+dfsg-2.1ubuntu12
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1ubuntu12.dsc' imagemagick_6.9.10.23+dfsg-2.1ubuntu12.dsc 5228 SHA256:6a694deff027256309ca2593e42ed91e2fe31958db11614cd221ae08195e518b
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.10.23+dfsg.orig.tar.xz' imagemagick_6.9.10.23+dfsg.orig.tar.xz 9081188 SHA256:44249112b624f2cc315573fa96685e547da27ebb321432259290c407023c531e
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1ubuntu12.debian.tar.xz' imagemagick_6.9.10.23+dfsg-2.1ubuntu12.debian.tar.xz 241284 SHA256:e36e8d2800a4241110616a3be9fea11660afd48feed1d4746388bc9b02df1c36
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.58.dsc' init-system-helpers_1.58.dsc 1896 SHA256:d754ec5e07416c63ead4c8c029d24027c563ff5f83762f2ac5246f716d405784
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.58.tar.xz' init-system-helpers_1.58.tar.xz 40668 SHA256:99f82ffca33b121f7aa31a06b6227f4684d986ff342a27b07433711de883609d
```

### `dpkg` source package: `isl=0.22.1-1`

Binary Packages:

- `libisl22:amd64=0.22.1-1`

Licenses: (parsed from: `/usr/share/doc/libisl22/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.22.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1-1.dsc' isl_0.22.1-1.dsc 1860 SHA256:9e9925317ef448cf679040edb6572a2874d497f758b613d9fc633bdafab197cb
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1.orig.tar.xz' isl_0.22.1.orig.tar.xz 1676948 SHA256:28658ce0f0bdb95b51fd2eb15df24211c53284f6ca2ac5e897acc3169e55b60f
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1-1.debian.tar.xz' isl_0.22.1-1.debian.tar.xz 25252 SHA256:bbeb62cfc95e51c25448e127c29fa8ac8009a6f471861de28f326bab2404a406
```

### `dpkg` source package: `jbigkit=2.1-3.1build1`

Binary Packages:

- `libjbig-dev:amd64=2.1-3.1build1`
- `libjbig0:amd64=2.1-3.1build1`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.dsc' jbigkit_2.1-3.1build1.dsc 2085 SHA256:fc768c7dac53f37f89c8d0a25760a29cd9afffc5cf55821f92d0d7e8f8f26e38
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.debian.tar.xz' jbigkit_2.1-3.1build1.debian.tar.xz 7672 SHA256:d7151df94f409045aa4d27dab88e538398196330d1ce135b60564dbc5db0a5c4
```

### `dpkg` source package: `keyutils=1.6.1-2ubuntu1`

Binary Packages:

- `libkeyutils1:amd64=1.6.1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.1-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu1.dsc' keyutils_1.6.1-2ubuntu1.dsc 2191 SHA256:1ab35f3c660bbb1a67258769461300d7287f9f8a3715b00855ef6191b5cb28ae
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1.orig.tar.bz2' keyutils_1.6.1.orig.tar.bz2 97232 SHA256:c8b15722ae51d95b9ad76cc6d49a4c2cc19b0c60f72f61fb9bf43eea7cbd64ce
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu1.debian.tar.xz' keyutils_1.6.1-2ubuntu1.debian.tar.xz 14364 SHA256:d301104058e36c6ddfa403ad622d7226b7beee6fb7a1866ec0edb5d5339063ca
```

### `dpkg` source package: `krb5=1.17-10`

Binary Packages:

- `krb5-multidev:amd64=1.17-10`
- `libgssapi-krb5-2:amd64=1.17-10`
- `libgssrpc4:amd64=1.17-10`
- `libk5crypto3:amd64=1.17-10`
- `libkadm5clnt-mit11:amd64=1.17-10`
- `libkadm5srv-mit11:amd64=1.17-10`
- `libkdb5-9:amd64=1.17-10`
- `libkrb5-3:amd64=1.17-10`
- `libkrb5-dev:amd64=1.17-10`
- `libkrb5support0:amd64=1.17-10`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit11/copyright`, `/usr/share/doc/libkadm5srv-mit11/copyright`, `/usr/share/doc/libkdb5-9/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-10
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-10.dsc' krb5_1.17-10.dsc 3187 SHA256:1ce061fc29b4c1d12c46c07d7a1fc2a16ed026ed5d7bd3e639483bdc27a2007f
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA256:5a6e2284a53de5702d3dc2be3b9339c963f9b5397d3fbbc53beb249380a781f5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-10.debian.tar.xz' krb5_1.17-10.debian.tar.xz 143852 SHA256:6d3cefcea2e4839cc3c5e518083048b8eae62a4bc707db05c1900c5bddafa7f5
```

### `dpkg` source package: `lcms2=2.9-4`

Binary Packages:

- `liblcms2-2:amd64=2.9-4`
- `liblcms2-dev:amd64=2.9-4`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.9-4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-4.dsc' lcms2_2.9-4.dsc 1956 SHA256:6db871353515693e8813911a8f81668b92e8c09fa9e6752e701fa8b14247775d
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9.orig.tar.gz' lcms2_2.9.orig.tar.gz 10974649 SHA256:48c6fdf98396fa245ed86e622028caf49b96fa22f3e5734f853f806fbc8e7d20
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-4.debian.tar.xz' lcms2_2.9-4.debian.tar.xz 10748 SHA256:3dd811c431bed101269937299d28708dfe91f32070cf9786680bec26f408b65b
```

### `dpkg` source package: `libassuan=2.5.3-7.1`

Binary Packages:

- `libassuan0:amd64=2.5.3-7.1`

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
$ apt-get source -qq --print-uris libassuan=2.5.3-7.1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.dsc' libassuan_2.5.3-7.1.dsc 2627 SHA256:9e4cfaef54fee1b6c1fd32fdfe6fc90b2dde78755517ee0ff56859e69251fb07
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA256:91bcb0403866b4e7c4bc1cc52ed4c364a9b5414b3994f718c70303f7f765e702
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA256:53b16a6619a2690b4f22da645a1d0c14b5664825c87b165ca5bd0de32607888a
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.debian.tar.xz' libassuan_2.5.3-7.1.debian.tar.xz 13952 SHA256:c6783e12dc1fb65681c083274f52cb3286da18dcf8a5b38a6de10143003e0681
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.dsc' libbsd_0.10.0-1.dsc 2197 SHA256:7c05e2c73658f64cbd4e1762b716cc7c4c1d68391191e82c7d266a351430edd6
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz' libbsd_0.10.0.orig.tar.xz 393576 SHA256:34b8adc726883d0e85b3118fa13605e179a62b31ba51f676136ecb2d0bc1a887
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz.asc' libbsd_0.10.0.orig.tar.xz.asc 833 SHA256:4362f6d811ffc06659ac5cf777d8d01157bedfc28720b41fb485afb0a5acc0c7
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.debian.tar.xz' libbsd_0.10.0-1.debian.tar.xz 16660 SHA256:4cf37d6d5b72702b31b07384612e07173e94e081feef71fec206f86ab38f2411
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.dsc' libcap-ng_0.7.9-2.2.dsc 2081 SHA256:d573ce59d83d2c117515e7c57dde1c990e9c5a34e0f53ac09f6b4d3e153e9aae
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.debian.tar.xz' libcap-ng_0.7.9-2.2.debian.tar.xz 6308 SHA256:6d7b5cfcf435fe996e5dc78770a9ab1ab614ced5bee56e3e0ba4e09d8c832a0a
```

### `dpkg` source package: `libcbor=0.6.0-0ubuntu2`

Binary Packages:

- `libcbor0.6:amd64=0.6.0-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libcbor0.6/copyright`)

- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.6.0-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu2.dsc' libcbor_0.6.0-0ubuntu2.dsc 2115 SHA256:b6538faed9b0eaa9831fc636d35009c7f7313536969f2dabd1ae8cb1510705b8
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0.orig.tar.gz' libcbor_0.6.0.orig.tar.gz 262622 SHA256:ad97dfe6462a28956be38c924a5a557acf303d8454ca121e02150a5b87e03ee7
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu2.debian.tar.xz' libcbor_0.6.0-0ubuntu2.debian.tar.xz 5984 SHA256:33d07bee780a0277ffab8958170cf3a5f3f300edcf4b041aa0482ad67b3f1e94
```

### `dpkg` source package: `libdatrie=0.2.12-3`

Binary Packages:

- `libdatrie1:amd64=0.2.12-3`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.12-3
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.12-3.dsc' libdatrie_0.2.12-3.dsc 2260 SHA256:631b3aa1b0cf12bcb04df8a19a8370445801a176edce830e74c01f6a55f778aa
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.12.orig.tar.xz' libdatrie_0.2.12.orig.tar.xz 310236 SHA256:452dcc4d3a96c01f80f7c291b42be11863cd1554ff78b93e110becce6e00b149
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.12-3.debian.tar.xz' libdatrie_0.2.12-3.debian.tar.xz 9188 SHA256:10409d93b3762b8ac8e0851bb2b71f76c2c5b57df8999bf8b9686d951c8b7476
```

### `dpkg` source package: `libedit=3.1-20191231-1`

Binary Packages:

- `libedit2:amd64=3.1-20191231-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.dsc' libedit_3.1-20191231-1.dsc 2129 SHA256:1be31eebf9cf3b38a9e7c3c4d4b37f002e3f89df48f00dec32506cbe9337ae38
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA256:dbb82cb7e116a5f8025d35ef5b4f7d4a3cdd0a3909a146a39112095a2d229071
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.debian.tar.xz' libedit_3.1-20191231-1.debian.tar.xz 14168 SHA256:f815baa1932f9df5d4cdb316a85ebd3cc91441c4d83ba2c8454f342573ed0eab
```

### `dpkg` source package: `liberror-perl=0.17029-1`

Binary Packages:

- `liberror-perl=0.17029-1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17029-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.dsc' liberror-perl_0.17029-1.dsc 2336 SHA256:0590467fe8c5f81bff9336e991462b2a9994b4876f4b732c8b8b31e927987cd7
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA256:1a23f7913032aed6d4b68321373a3899ca66590f4727391a091ec19c95bf7adc
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.debian.tar.xz' liberror-perl_0.17029-1.debian.tar.xz 4552 SHA256:a753b142c4c33ebf9cc98ae5f7a08da13b7c9ca2823ec26e45c96efb9c15c42e
```

### `dpkg` source package: `libevent=2.1.12-stable-1`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.12-stable-1`
- `libevent-core-2.1-7:amd64=2.1.12-stable-1`
- `libevent-dev=2.1.12-stable-1`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-1`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-1`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-1`

Licenses: (parsed from: `/usr/share/doc/libevent-2.1-7/copyright`, `/usr/share/doc/libevent-core-2.1-7/copyright`, `/usr/share/doc/libevent-dev/copyright`, `/usr/share/doc/libevent-extra-2.1-7/copyright`, `/usr/share/doc/libevent-openssl-2.1-7/copyright`, `/usr/share/doc/libevent-pthreads-2.1-7/copyright`)

- `BSD-2-clause`
- `BSD-3-Clause~Kitware`
- `BSD-3-clause`
- `BSL`
- `Expat`
- `FSFUL`
- `FSFULLR`
- `FSFULLR-No-Warranty`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `curl`

Source:

```console
$ apt-get source -qq --print-uris libevent=2.1.12-stable-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1.dsc' libevent_2.1.12-stable-1.dsc 2527 SHA256:e82d9dc2160de05b1827b04894a954079e23ede0d5e2b5a1d9e9b2021e7c4e10
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA256:92e6de1be9ec176428fd2367677e61ceffc2ee1cb119035037a27d346b0403bb
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz.asc' libevent_2.1.12-stable.orig.tar.gz.asc 488 SHA256:3cd3d764777540305813495912cd5f7ea7d16edb456d6c88b331a1aa8974dfc2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1.debian.tar.xz' libevent_2.1.12-stable-1.debian.tar.xz 17764 SHA256:cc608fff85ed5b262dee671fe17444aa6734dbc3be232e0b6ecca41252a62438
```

### `dpkg` source package: `libexif=0.6.22-2`

Binary Packages:

- `libexif-dev:amd64=0.6.22-2`
- `libexif12:amd64=0.6.22-2`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.22-2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-2.dsc' libexif_0.6.22-2.dsc 2079 SHA256:6d8a8c0c987b610959c250c912e4995103de141178a7ddb2030f9e8c6f22baf1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22.orig.tar.gz' libexif_0.6.22.orig.tar.gz 1109525 SHA256:46498934b7b931526fdee8fd8eb77a1dddedd529d5a6dbce88daf4384baecc54
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-2.debian.tar.xz' libexif_0.6.22-2.debian.tar.xz 12016 SHA256:bfb1beff5dcff9aadaef3bbeb5592a1f20d7d66a75161c56bfa53c433655f0b8
```

### `dpkg` source package: `libffi=3.3-4`

Binary Packages:

- `libffi-dev:amd64=3.3-4`
- `libffi7:amd64=3.3-4`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi7/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.3-4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3-4.dsc' libffi_3.3-4.dsc 1932 SHA256:4190ad8e7ae9167a0c67c5926bc3705acb191745cca93ef845dbc06fc097f380
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3.orig.tar.gz' libffi_3.3.orig.tar.gz 1305466 SHA256:72fba7922703ddfa7a028d513ac15a85c8d54c8d67f55fa5a4802885dc652056
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3-4.debian.tar.xz' libffi_3.3-4.debian.tar.xz 9016 SHA256:0e8a6d9d87202d04d7646178479c3d365a845f9723da26625d533a169b378100
```

### `dpkg` source package: `libfido2=1.4.0-2`

Binary Packages:

- `libfido2-1:amd64=1.4.0-2`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0-2.dsc' libfido2_1.4.0-2.dsc 2565 SHA256:139d27a6b1079528282c1a320c94f071d5eb3bd62e25a05ef8bb4eb1a0cc7fcb
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0.orig.tar.gz' libfido2_1.4.0.orig.tar.gz 391439 SHA256:ad921fbe7d4bb70e4a971e564cd01f341daf9b5ed5d69b3cbab94a8a811d2a6c
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0.orig.tar.gz.asc' libfido2_1.4.0.orig.tar.gz.asc 488 SHA256:5d40de81c7e032be2d34ab87a8d4e1a2cc4f1f715449f65054a041249eb83fac
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0-2.debian.tar.xz' libfido2_1.4.0-2.debian.tar.xz 73908 SHA256:75b7e7b87e44237c91735a63d93ffd0267cac27fd674395224b438529ed159b6
```

### `dpkg` source package: `libgcrypt20=1.8.5-5ubuntu2`

Binary Packages:

- `libgcrypt20:amd64=1.8.5-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.5-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu2.dsc' libgcrypt20_1.8.5-5ubuntu2.dsc 2907 SHA256:1b53962dd788843f0ca1c3c6e37874a737ba407d42a43f9a303c98d7d9fa92eb
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2' libgcrypt20_1.8.5.orig.tar.bz2 2991291 SHA256:3b4a2a94cb637eff5bdebbcaf46f4d95c4f25206f459809339cdada0eb577ac3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2.asc' libgcrypt20_1.8.5.orig.tar.bz2.asc 488 SHA256:4b24fda7847cd2b70ab19f4c38004a76bbdac46a1ddccff973ae88ba1296a22d
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu2.debian.tar.xz' libgcrypt20_1.8.5-5ubuntu2.debian.tar.xz 35444 SHA256:a173f29ed6637618340e5f89c4480ddfe90eac2bacdadc43b91a51fc96668982
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2.dsc' libgpg-error_1.38-2.dsc 2220 SHA256:ab0ea76aa3552afa664210a871abc74637acafd89c068edf8dc03521b8e22d64
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2' libgpg-error_1.38.orig.tar.bz2 957637 SHA256:d8988275aa69d7149f931c10442e9e34c0242674249e171592b430ff7b3afd02
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2.asc' libgpg-error_1.38.orig.tar.bz2.asc 488 SHA256:d80eb927d85e19e96d8de17552f8f48b517ae7acac7685404e8027475c5b4330
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2.debian.tar.xz' libgpg-error_1.38-2.debian.tar.xz 19544 SHA256:824bcb278ead676c20f174bd551b1cc44a294137fabe6a1d892667882f3b4ba2
```

### `dpkg` source package: `libice=2:1.0.10-0ubuntu1`

Binary Packages:

- `libice-dev:amd64=2:1.0.10-0ubuntu1`
- `libice6:amd64=2:1.0.10-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.10-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-0ubuntu1.dsc' libice_1.0.10-0ubuntu1.dsc 1629 SHA256:51f58a0e5a5c5ea780baa3a057b61a921001831a4817da8825dbf592afccbdd6
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10.orig.tar.gz' libice_1.0.10.orig.tar.gz 481960 SHA256:1116bc64c772fd127a0d0c0ffa2833479905e3d3d8197740b3abd5f292f22d2d
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-0ubuntu1.diff.gz' libice_1.0.10-0ubuntu1.diff.gz 6470 SHA256:a9187c11c1b372b0f4cb58c2fb21f780e9236fd7011bb32c4188c7b37112e8de
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-1.dsc' libidn2_2.3.0-1.dsc 2411 SHA256:f4f61425610ae4b4c4d3c74431825fb4b4892d4d07e954d7acdf163595d33f14
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0.orig.tar.gz' libidn2_2.3.0.orig.tar.gz 2164993 SHA256:e1cb1db3d2e249a6a3eb6f0946777c2e892d5c5dc7bd91c74394fc3a01cab8b5
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-1.debian.tar.xz' libidn2_2.3.0-1.debian.tar.xz 10588 SHA256:a515029f13d12a48a6bc07dadc4cef6592db0a7257f48633795ae7128c23116c
```

### `dpkg` source package: `libjpeg-turbo=2.0.3-0ubuntu2`

Binary Packages:

- `libjpeg-turbo8:amd64=2.0.3-0ubuntu2`
- `libjpeg-turbo8-dev:amd64=2.0.3-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.0.3-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3-0ubuntu2.dsc' libjpeg-turbo_2.0.3-0ubuntu2.dsc 2305 SHA256:f18be4c82879a4ce202626fafff5dc523ccfd5f504b16e41493b60c33964fa07
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3.orig.tar.gz' libjpeg-turbo_2.0.3.orig.tar.gz 2161279 SHA256:a69598bf079463b34d45ca7268462a18b6507fdaa62bb1dfd212f02041499b5d
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3-0ubuntu2.debian.tar.xz' libjpeg-turbo_2.0.3-0ubuntu2.debian.tar.xz 18208 SHA256:4d49d9411736b319d1fc21c8d23740bd5a30f7ffbe9aff2470d52ce8ba022190
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu8`

Binary Packages:

- `libjpeg-dev:amd64=8c-2ubuntu8`
- `libjpeg8:amd64=8c-2ubuntu8`
- `libjpeg8-dev:amd64=8c-2ubuntu8`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg8/copyright`, `/usr/share/doc/libjpeg8-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg8-empty=8c-2ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.dsc' libjpeg8-empty_8c-2ubuntu8.dsc 1637 SHA256:e7f575dcb3e0d462513b6f928179baa0ff1d145273934b1041b714515096b407
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.tar.gz' libjpeg8-empty_8c-2ubuntu8.tar.gz 1770 SHA256:48a4227e9fc70851a4f304b10624e02875bf6f4e2debfcbe4ba0dd85a3ec05c6
```

### `dpkg` source package: `libksba=1.4.0-2`

Binary Packages:

- `libksba8:amd64=1.4.0-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0-2.dsc' libksba_1.4.0-2.dsc 2470 SHA256:71333f487433f883ccff7211c9206804f23b25dbc38f401391f953333984165c
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0.orig.tar.bz2' libksba_1.4.0.orig.tar.bz2 651319 SHA256:bfe6a8e91ff0f54d8a329514db406667000cb207238eded49b599761bfca41b6
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0.orig.tar.bz2.asc' libksba_1.4.0.orig.tar.bz2.asc 488 SHA256:4f8e92ecd55bf3b7db6cec5f83d4721b75a9fcb43eb9b6bae2ed9a018951ca5e
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0-2.debian.tar.xz' libksba_1.4.0-2.debian.tar.xz 10368 SHA256:8f49625bd327bb08975b65c08297cd9eea8591c1bcda98f5289fa5b4710ce0ad
```

### `dpkg` source package: `liblqr=0.4.2-2.1`

Binary Packages:

- `liblqr-1-0:amd64=0.4.2-2.1`
- `liblqr-1-0-dev:amd64=0.4.2-2.1`

Licenses: (parsed from: `/usr/share/doc/liblqr-1-0/copyright`, `/usr/share/doc/liblqr-1-0-dev/copyright`)

- `GPL-3`
- `GPLv3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris liblqr=0.4.2-2.1
'http://archive.ubuntu.com/ubuntu/pool/universe/libl/liblqr/liblqr_0.4.2-2.1.dsc' liblqr_0.4.2-2.1.dsc 2095 SHA256:c54c34cd2f7470a29366eeacde2ca4859a97d684a406fb81a918b970c01d617c
'http://archive.ubuntu.com/ubuntu/pool/universe/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA256:d4c22373432cca749e4326cd41fce365e6ff857c0bfd7a5302b8eb34b69f0336
'http://archive.ubuntu.com/ubuntu/pool/universe/libl/liblqr/liblqr_0.4.2-2.1.debian.tar.xz' liblqr_0.4.2-2.1.debian.tar.xz 5300 SHA256:284a002f1ecac63ac17b1aafbb230da9ce7bd9efe2d5b94e8cad49b607eb2564
```

### `dpkg` source package: `libmaxminddb=1.4.2-0ubuntu1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.4.2-0ubuntu1`
- `libmaxminddb0:amd64=1.4.2-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libmaxminddb-dev/copyright`, `/usr/share/doc/libmaxminddb0/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `CC-BY-SA`
- `GPL`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmaxminddb=1.4.2-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.4.2-0ubuntu1.dsc' libmaxminddb_1.4.2-0ubuntu1.dsc 2209 SHA256:a7f05c735d041f2f5ed90ac58f2df958acc3b8d77f875969f143662e35373b48
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.4.2.orig.tar.gz' libmaxminddb_1.4.2.orig.tar.gz 600664 SHA256:dd582aa971be23dee960ec33c67fb5fd38affba508e6f00ea75959dbd5aad156
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.4.2-0ubuntu1.debian.tar.xz' libmaxminddb_1.4.2-0ubuntu1.debian.tar.xz 4780 SHA256:3bf624b848feb2746b1e824b4db170a5049d9e38e00e7bf3ddfa2e590a31018c
```

### `dpkg` source package: `libpng1.6=1.6.37-2`

Binary Packages:

- `libpng-dev:amd64=1.6.37-2`
- `libpng16-16:amd64=1.6.37-2`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.37-2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-2.dsc' libpng1.6_1.6.37-2.dsc 2225 SHA256:4567a54b5804e068e61477e9cd78346557b85b72add10ef10f130a5be169662e
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA256:ca74a0dace179a8422187671aee97dd3892b53e168627145271cad5b5ac81307
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-2.debian.tar.xz' libpng1.6_1.6.37-2.debian.tar.xz 31844 SHA256:097cee0f0da4013d0231d37e090204ab3fa592b4fecdaaed3fca8d13affcaae8
```

### `dpkg` source package: `libpsl=0.21.0-1.1`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.1.dsc' libpsl_0.21.0-1.1.dsc 2228 SHA256:88e9ead32ef07fd807dd9b2eac7184baea346bd8b13878c9002b32e6286a4237
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA256:055aa87ec166c7afb985d0816c07ff440e1eb899881a318c51c69a0aeea8e279
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.1.debian.tar.xz' libpsl_0.21.0-1.1.debian.tar.xz 12432 SHA256:aaf2dc28ed4b1b3d754895e3c21b0fb2be1f725fdec1f6d35a856cbe0b32cf46
```

### `dpkg` source package: `libpthread-stubs=0.4-1`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.dsc' libpthread-stubs_0.4-1.dsc 1927 SHA256:8923683ac365475d2cc515e5f16f4adc8bd8e37453e1a2a6bedeb9246922829f
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4.orig.tar.gz' libpthread-stubs_0.4.orig.tar.gz 71252 SHA256:50d5686b79019ccea08bcbd7b02fe5a40634abcfd4146b6e75c6420cc170e9d9
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.diff.gz' libpthread-stubs_0.4-1.diff.gz 2346 SHA256:ec435ba2852ad4b0522010943a5b7d39fc7e088067367879778cf10e57f5cc3f
```

### `dpkg` source package: `librsvg=2.48.7-1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.48.7-1`
- `librsvg2-2:amd64=2.48.7-1`
- `librsvg2-common:amd64=2.48.7-1`
- `librsvg2-dev:amd64=2.48.7-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `Boost-1.0`
- `Expat`
- `LGPL-2`
- `LGPL-2+`
- `MPL-2.0`
- `Sun-permissive`
- `Unlicense`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.48.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.48.7-1.dsc' librsvg_2.48.7-1.dsc 2914 SHA256:5e5ac23273073426db86af94e3bfa958b245c088d41d8b5b610c7044476fce22
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.48.7.orig.tar.xz' librsvg_2.48.7.orig.tar.xz 15097208 SHA256:35de5d93e262fcd85fa4529cee147687d21c6e092f223c293921eaaf57e2fec0
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.48.7-1.debian.tar.xz' librsvg_2.48.7-1.debian.tar.xz 24148 SHA256:8a5b5bcf500dbf361adf2448a926c7ebf75552b49497d78fa5c90cb39ac6ce64
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu4`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu4.dsc' libseccomp_2.4.3-1ubuntu4.dsc 2539 SHA256:172bd74618fb9433840a4728e7f22f0a6a02f215ad768e1a6cb2ef3a48cb3477
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA256:cf15d1421997fac45b936515af61d209c4fd788af11005d212b3d0fd71e7991d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu4.debian.tar.xz' libseccomp_2.4.3-1ubuntu4.debian.tar.xz 36432 SHA256:0ef117ab20adf01f8fe6aa0e3f00a401a5527ce28f85ccd88f5fbea0ccb6654b
```

### `dpkg` source package: `libselinux=3.1-2`

Binary Packages:

- `libselinux1:amd64=3.1-2`
- `libselinux1-dev:amd64=3.1-2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-2.dsc' libselinux_3.1-2.dsc 2310 SHA256:9d9a31ac3e11dcaa1bbdaa28c3bdc7dc44a94b0b3d6b380e5c5e69f6f57c5901
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1.orig.tar.gz' libselinux_3.1.orig.tar.gz 204703 SHA256:ea5dcbb4d859e3f999c26a13c630da2f16dff9462e3cc8cb7b458ac157d112e7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-2.debian.tar.xz' libselinux_3.1-2.debian.tar.xz 23788 SHA256:336c6df026daf947f37c74d3e3efdfc6b235491d402096f050ce2c9d8bbad415
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1.dsc' libsemanage_3.1-1.dsc 2339 SHA256:d49f9c29d0ad9c8b42145e0926919df962b58823e9fc22002bbb00333276170d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1.orig.tar.gz' libsemanage_3.1.orig.tar.gz 179601 SHA256:22d6c75526e40d1781c30bcf29abf97171bdfe6780923f11c8e1c76a75a21ff8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1.debian.tar.xz' libsemanage_3.1-1.debian.tar.xz 17556 SHA256:185b151158faaaf3d8f9ff939f29efd3eb5dbb050d01a87d3fde6cf40e778648
```

### `dpkg` source package: `libsepol=3.1-1`

Binary Packages:

- `libsepol1:amd64=3.1-1`
- `libsepol1-dev:amd64=3.1-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`, `/usr/share/doc/libsepol1-dev/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.dsc' libsepol_3.1-1.dsc 1776 SHA256:37bfb6797af8a96eada6c6ace374292b8a16a6bfb557b1e8ab9fd29e72d5888a
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA256:ae6778d01443fdd38cd30eeee846494e19f4d407b09872580372f4aa4bf8a3cc
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.debian.tar.xz' libsepol_3.1-1.debian.tar.xz 14584 SHA256:9351a0b6207f6a5da2951292d3ec5655feb89df5aabc9010094766d811156166
```

### `dpkg` source package: `libsigsegv=2.12-2build1`

Binary Packages:

- `libsigsegv2:amd64=2.12-2build1`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.12-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2build1.dsc' libsigsegv_2.12-2build1.dsc 2466 SHA256:86e2d1f4899d65340bf8970f1ebd969200c4c2bb30a9e5d5e1449185c69cda14
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz' libsigsegv_2.12.orig.tar.gz 451408 SHA256:3ae1af359eebaa4ffc5896a1aee3568c052c99879316a1ab57f8fe1789c390b6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz.asc' libsigsegv_2.12.orig.tar.gz.asc 2442 SHA256:1861a9a182bbb7a24a18f7e43fe0fa3eb6f6fd53780b30e01990677112694dfc
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2build1.debian.tar.xz' libsigsegv_2.12-2build1.debian.tar.xz 8448 SHA256:77beeebdaf45eb6934c3396d938bba2f3b917c8c1cb640932f4b8623b5caacd4
```

### `dpkg` source package: `libsm=2:1.2.3-1`

Binary Packages:

- `libsm-dev:amd64=2:1.2.3-1`
- `libsm6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1.dsc' libsm_1.2.3-1.dsc 2063 SHA256:5488f8de81d53c32cbb5f062b6a6f262cd067283b8082041392dc60f0d04002c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3.orig.tar.gz' libsm_1.2.3.orig.tar.gz 445362 SHA256:1e92408417cb6c6c477a8a6104291001a40b3bb56a4a60608fdd9cd2c5a0f320
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1.diff.gz' libsm_1.2.3-1.diff.gz 8929 SHA256:7eb99ab50b19f26d1470f89e4b46891f6a697cb1794a58ed0d1376cceaf1b6a9
```

### `dpkg` source package: `libssh=0.9.4-1ubuntu2`

Binary Packages:

- `libssh-4:amd64=0.9.4-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.4-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4-1ubuntu2.dsc' libssh_0.9.4-1ubuntu2.dsc 2771 SHA256:f59d9ac6b3097b1484815002cda2e3d5ee49d8306750e55db56b26f5464e1ccd
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4.orig.tar.xz' libssh_0.9.4.orig.tar.xz 500776 SHA256:150897a569852ac05aac831dc417a7ba8e610c86ca2e0154a99c6ade2486226b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4.orig.tar.xz.asc' libssh_0.9.4.orig.tar.xz.asc 833 SHA256:b637b8e4dae3109ae0b10ddfb35f9d5ce01049409c0b3572ee81292be30bccae
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4-1ubuntu2.debian.tar.xz' libssh_0.9.4-1ubuntu2.debian.tar.xz 28748 SHA256:44e6847ea6217664ff793d799acd4892ebef5f580661eda276d378057304c2ff
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.dsc' libtasn1-6_4.16.0-2.dsc 2586 SHA256:fd4a387c71f95c3eceb1072a3f42c7021d73128027ea41a18d6efc6cbfdd764a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz' libtasn1-6_4.16.0.orig.tar.gz 1812442 SHA256:0e0fb0903839117cb6e3b56e68222771bebf22ad7fc2295a0ed7d576e8d4329d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz.asc' libtasn1-6_4.16.0.orig.tar.gz.asc 488 SHA256:06c201e8c3b43c27465ed79294d4c4ec8dcd3e95e4a6176ecbf273229ee3e2d0
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.debian.tar.xz' libtasn1-6_4.16.0-2.debian.tar.xz 17740 SHA256:c1a89b0bac0fb7c83ebac4eafbca0475c24350ade6ccaef31266424725610624
```

### `dpkg` source package: `libthai=0.1.28-3`

Binary Packages:

- `libthai-data=0.1.28-3`
- `libthai0:amd64=0.1.28-3`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.28-3
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28-3.dsc' libthai_0.1.28-3.dsc 2346 SHA256:a6317b6a8e4ba40cedb10a9a659fc23885bfbe5eb8cf3a8b325a86064b0a542d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28.orig.tar.xz' libthai_0.1.28.orig.tar.xz 413592 SHA256:ffe0a17b4b5aa11b153c15986800eca19f6c93a4025ffa5cf2cab2dcdf1ae911
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28-3.debian.tar.xz' libthai_0.1.28-3.debian.tar.xz 12128 SHA256:bca48abd9d040e844ebcb1f91a6ab4bcdfad66e36c1143f79d60461e933fddf9
```

### `dpkg` source package: `libtool=2.4.6-14`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-14`
- `libltdl7:amd64=2.4.6-14`
- `libtool=2.4.6-14`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-14
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-14.dsc' libtool_2.4.6-14.dsc 2500 SHA256:939797b7ce62f69641d319e5d38e53b1608cee649355046eec74271e9fcfb9df
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-14.debian.tar.xz' libtool_2.4.6-14.debian.tar.xz 50832 SHA256:3ef693ea30def97a19fd94ffb2fa5421d5dc35cf7ad897a7161bd647eb4f2415
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.dsc' libunistring_0.9.10-4.dsc 2212 SHA256:5c7940807b538d4204506349cbd67e5c677afb9f0e46e94455353e3f746a481e
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.debian.tar.xz' libunistring_0.9.10-4.debian.tar.xz 40936 SHA256:6c9554e1a1c6d0a02ca4868a5422d176e57a3131c1a8a21de5503b164997525c
```

### `dpkg` source package: `libwebp=0.6.1-2`

Binary Packages:

- `libwebp-dev:amd64=0.6.1-2`
- `libwebp6:amd64=0.6.1-2`
- `libwebpdemux2:amd64=0.6.1-2`
- `libwebpmux3:amd64=0.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.6.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.dsc' libwebp_0.6.1-2.dsc 2064 SHA256:321ee69e44f0d037d5fec47692251e35ed22c9ad0bbf0a6bf0fae990a52319f4
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA256:a86045e3ec24704bddbaa369ca30980d6bf4f2625f4cdca03715e91f9c08bbb4
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.debian.tar.xz' libwebp_0.6.1-2.debian.tar.xz 9532 SHA256:5af543e277abb97f6b2c72ca0d7ce95de79108d88da383d511ef729683fa7a45
```

### `dpkg` source package: `libwmf=0.2.8.4-17ubuntu1`

Binary Packages:

- `libwmf-dev=0.2.8.4-17ubuntu1`
- `libwmf0.2-7:amd64=0.2.8.4-17ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-17ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu1.dsc' libwmf_0.2.8.4-17ubuntu1.dsc 1642 SHA256:31f409e280954b2388e28305ac1c39b85eb141e7823b6fc5eff89194196c4e2a
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu1.debian.tar.xz' libwmf_0.2.8.4-17ubuntu1.debian.tar.xz 12968 SHA256:3d78073cbb035aa87d780d617f647a3e42f4cf5e9c1ada5899f7d80ac306f318
```

### `dpkg` source package: `libx11=2:1.6.10-3`

Binary Packages:

- `libx11-6:amd64=2:1.6.10-3`
- `libx11-data=2:1.6.10-3`
- `libx11-dev:amd64=2:1.6.10-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.10-3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.10-3.dsc' libx11_1.6.10-3.dsc 2574 SHA256:0c860ba77f7cec4a99349af0da30af796bf27c4da8a58a5eaf778f38bb452ced
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.10.orig.tar.gz' libx11_1.6.10.orig.tar.gz 2995209 SHA256:e4b92bcef5d4274693ce4a2a7c9e97d2614fc2b30b17c8166a301f3c335e0ba2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.10.orig.tar.gz.asc' libx11_1.6.10.orig.tar.gz.asc 833 SHA256:de6d162b76bd8fa714283332ce5e9d63eebc90c0800a856e2368b10268a3a199
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.10-3.diff.gz' libx11_1.6.10-3.diff.gz 50566 SHA256:fa403141efa86b4bd4debf4214c01c8fbbe2b80d207b574142091b45b40a124e
```

### `dpkg` source package: `libxau=1:1.0.9-0ubuntu1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.9-0ubuntu1`
- `libxau6:amd64=1:1.0.9-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-0ubuntu1.dsc' libxau_1.0.9-0ubuntu1.dsc 1563 SHA256:b59509d1f8f6c0e21b8bbd46ac1dffcd7a21a635ff3ce9c0acf68ba60fcb5e11
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA256:1f123d8304b082ad63a9e89376400a3b1d4c29e67e3ea07b3f659cccca690eea
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-0ubuntu1.diff.gz' libxau_1.0.9-0ubuntu1.diff.gz 15142 SHA256:cf7e9d50c3b3b8dde3486ee6fcf9bb96585e2af32924e91c10c8612e48b5dce5
```

### `dpkg` source package: `libxcb=1.14-2`

Binary Packages:

- `libxcb-render0:amd64=1.14-2`
- `libxcb-render0-dev:amd64=1.14-2`
- `libxcb-shm0:amd64=1.14-2`
- `libxcb-shm0-dev:amd64=1.14-2`
- `libxcb1:amd64=1.14-2`
- `libxcb1-dev:amd64=1.14-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.dsc' libxcb_1.14-2.dsc 5344 SHA256:997dfadefa35a243a7160b62d628bb25e45439f61687459d581502905bcf1fb2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA256:2c7fcddd1da34d9b238c9caeda20d3bd7486456fc50b3cc6567185dbd5b0ad02
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.diff.gz' libxcb_1.14-2.diff.gz 25716 SHA256:92d7e0a80c3c7f2a5b5afd0c0702183f1c483338d678d67d8d0e61fd8989ba85
```

### `dpkg` source package: `libxcrypt=1:4.4.16-1ubuntu1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.16-1ubuntu1`
- `libcrypt1:amd64=1:4.4.16-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.16-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16-1ubuntu1.dsc' libxcrypt_4.4.16-1ubuntu1.dsc 2212 SHA256:2e030d707ba0c6aced4334a5338ce9a3e9523aaeb9a3884ae962fbad6a07d7b9
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16.orig.tar.xz' libxcrypt_4.4.16.orig.tar.xz 354788 SHA256:6a675b4ef1adde90b07ebc2f45eb9cd26702fbf87aa625d5aae9f68581d34fa6
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16-1ubuntu1.debian.tar.xz' libxcrypt_4.4.16-1ubuntu1.debian.tar.xz 5840 SHA256:6bfd0591b366230b92550693a786b6fe42716e2b57eda7042fc8ec3d355d0e53
```

### `dpkg` source package: `libxdmcp=1:1.1.3-0ubuntu1`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.3-0ubuntu1`
- `libxdmcp6:amd64=1:1.1.3-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.3-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu1.dsc' libxdmcp_1.1.3-0ubuntu1.dsc 1608 SHA256:3f98e3917b5de252eb517c55743bcc5682b43c9f70ead33231ac4318bbc816e1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3.orig.tar.gz' libxdmcp_1.1.3.orig.tar.gz 429668 SHA256:2ef9653d32e09d1bf1b837d0e0311024979653fe755ad3aaada8db1aa6ea180c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu1.diff.gz' libxdmcp_1.1.3-0ubuntu1.diff.gz 18079 SHA256:3037a57202b724ecd7db70c21a601f58277c02ba89e7e5d999973e5baf6d05ca
```

### `dpkg` source package: `libxext=2:1.3.4-0ubuntu1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.4-0ubuntu1`
- `libxext6:amd64=2:1.3.4-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.dsc' libxext_1.3.4-0ubuntu1.dsc 1727 SHA256:8319de2750f28c78e01267a5593776f10afd3f863d4820abe72dbf855a3a77ae
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA256:8ef0789f282826661ff40a8eef22430378516ac580167da35cc948be9041aac1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.diff.gz' libxext_1.3.4-0ubuntu1.diff.gz 20663 SHA256:87a4d23f1f9ff53f3a6cd7cc35252a1249dc63d274c566ea7e23b23585a86170
```

### `dpkg` source package: `libxml2=2.9.10+dfsg-5build1`

Binary Packages:

- `libxml2:amd64=2.9.10+dfsg-5build1`
- `libxml2-dev:amd64=2.9.10+dfsg-5build1`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.10+dfsg-5build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-5build1.dsc' libxml2_2.9.10+dfsg-5build1.dsc 3085 SHA256:d8ee0258616620b0999e71e1bb82b7a81e9f1388e03192416cb8a39169333fc9
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg.orig.tar.xz' libxml2_2.9.10+dfsg.orig.tar.xz 2503560 SHA256:65ee7a2f5e100c64ddf7beb92297c9b2a30b994a76cd1fab67470cf22db6b7d0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-5build1.debian.tar.xz' libxml2_2.9.10+dfsg-5build1.debian.tar.xz 28856 SHA256:06c9b04fdd5fa7e34f22b769689e2e10a5acbeb0ea46ecbc3bb1a7cc8d5a9cb5
```

### `dpkg` source package: `libxrender=1:0.9.10-1`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1`
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

### `dpkg` source package: `libxslt=1.1.34-4`

Binary Packages:

- `libxslt1-dev:amd64=1.1.34-4`
- `libxslt1.1:amd64=1.1.34-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.34-4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4.dsc' libxslt_1.1.34-4.dsc 2375 SHA256:29447f928b2fd534bd819aaf74005ff286f3786689a2684b9cbc61c1c65c2212
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA256:98b1bd46d6792925ad2dfe9a87452ea2adebf69dcb9919ffd55bf926a7f93f7f
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA256:673d1477552bdd5b0cc665704e77ca70e6be5d2f257e6a5a341c846719d747cf
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4.debian.tar.xz' libxslt_1.1.34-4.debian.tar.xz 21464 SHA256:24d5490d6e33f42391d2ce449dd8fec0830ced115a6af886ee03af985a727dc9
```

### `dpkg` source package: `libxt=1:1.1.5-1`

Binary Packages:

- `libxt-dev:amd64=1:1.1.5-1`
- `libxt6:amd64=1:1.1.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libxt/1:1.1.5-1/


### `dpkg` source package: `libyaml=0.2.2-1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.2-1`
- `libyaml-dev:amd64=0.2.2-1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.dsc' libyaml_0.2.2-1.dsc 1833 SHA256:b4baba985391f52409013a0c9303191e34aaa4c1c9200e4c01c4963df801db09
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2.orig.tar.gz' libyaml_0.2.2.orig.tar.gz 602509 SHA256:689ef3ebdecfa81f3789ccd2481acc81fc0f22f3f5c947eed95c4c0802e356b8
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.debian.tar.xz' libyaml_0.2.2-1.debian.tar.xz 4112 SHA256:186aad3e4bcd95891a8c59249c59f862f5f71601058fda0bf020a9e9e39320fe
```

### `dpkg` source package: `libzstd=1.4.5+dfsg-4`

Binary Packages:

- `libzstd1:amd64=1.4.5+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.5+dfsg-4
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg-4.dsc' libzstd_1.4.5+dfsg-4.dsc 2291 SHA256:c3017a5e41c86375cefa599b2d7ac457e7e87882a4e06e8d2af39b25ed29028d
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg.orig.tar.xz' libzstd_1.4.5+dfsg.orig.tar.xz 1387864 SHA256:ff51192647c8f87f447268e20180fe39fe8eb5d643210b82f90af741d7bdf0d2
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg-4.debian.tar.xz' libzstd_1.4.5+dfsg-4.debian.tar.xz 12724 SHA256:1eac2717d60601c467386cffadddd55221dfa6a94a4781de9ad8a331e5498b52
```

### `dpkg` source package: `linux=5.4.0-42.46`

Binary Packages:

- `linux-libc-dev:amd64=5.4.0-42.46`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lsb=11.1.0ubuntu2`

Binary Packages:

- `lsb-base=11.1.0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.dsc' lsb_11.1.0ubuntu2.dsc 2230 SHA256:983ff4ab1ab2b39af974e4b8f4373ab4028d0ee5a409e7cd40401fa8e6ecabde
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.tar.xz' lsb_11.1.0ubuntu2.tar.xz 46024 SHA256:c6ab63b6702dc633988690aacde8ece3e460f8acd8f1af8e6a67ab2fe0798f41
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.dsc' lz4_1.9.2-2.dsc 1956 SHA256:103fa80edbf501cf6e6d9ee0ed3d75d6111cd06026b00aaccaa11fe5555b71a6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2.orig.tar.gz' lz4_1.9.2.orig.tar.gz 305796 SHA256:658ba6191fa44c92280d4aa2c271b0f4fbc0e34d249578dd05e50e76d0e5efcc
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.debian.tar.xz' lz4_1.9.2-2.debian.tar.xz 12712 SHA256:8970a0afc2f1633bbc8b7f55fa36ba711fb4d0c1811e591ad8f52d1d1968592c
```

### `dpkg` source package: `lzo2=2.10-2`

Binary Packages:

- `liblzo2-2:amd64=2.10-2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.10-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2.dsc' lzo2_2.10-2.dsc 1926 SHA256:65a35d9d2511a88f30d4b10313f807c184d1906062e2421833797dafc2682166
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10.orig.tar.gz' lzo2_2.10.orig.tar.gz 600622 SHA256:c0f892943208266f9b6543b3ae308fab6284c5c90e627931446fb49b4221a072
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2.debian.tar.xz' lzo2_2.10-2.debian.tar.xz 6880 SHA256:095b2bf2012138f6892fcf226a0d1eae5d29406d7afe7129d51d64116e61c472
```

### `dpkg` source package: `m4=1.4.18-4`

Binary Packages:

- `m4=1.4.18-4`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-4
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-4.dsc' m4_1.4.18-4.dsc 1638 SHA256:11925f50e25f93d6b9a72336e7b9fd0de72a813d5d5f3204ecc3996f9ca3bbde
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA256:a2a9fff657e65ff25a8f3734f484dbd3ede8f8290786af71626de367dcd74267
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-4.debian.tar.xz' m4_1.4.18-4.debian.tar.xz 17240 SHA256:6543f074d5a3eed4ee7984f8a147c58e005c88254dfcf5bc3778c60b9ed07efd
```

### `dpkg` source package: `make-dfsg=4.3-4ubuntu1`

Binary Packages:

- `make=4.3-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.3-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu1.dsc' make-dfsg_4.3-4ubuntu1.dsc 2147 SHA256:895bd6fad9c8de0bbb146077c21184e9d353700c28c4160888baca0823837626
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA256:be4c17542578824e745f83bcd2a9ba264206187247cb6a5f5df99b0a9d1f9047
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu1.diff.gz' make-dfsg_4.3-4ubuntu1.diff.gz 51058 SHA256:4fbbd2f4f1722450795b655f48634f4793daa821a5e3b29598c76ccb99be0e63
```

### `dpkg` source package: `mawk=1.3.4.20200120-2`

Binary Packages:

- `mawk=1.3.4.20200120-2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.dsc' mawk_1.3.4.20200120-2.dsc 1915 SHA256:5069c46872ac74f5221250dfb88b31b1f2dbb8a2617c1e013f8f80cc34638c6d
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.debian.tar.xz' mawk_1.3.4.20200120-2.debian.tar.xz 7504 SHA256:b772ed2f016b0286980c46cbc1f1f4ae62887ef2aa3dff6ef10cae638f923f26
```

### `dpkg` source package: `mercurial=5.4.1-2ubuntu1`

Binary Packages:

- `mercurial=5.4.1-2ubuntu1`
- `mercurial-common=5.4.1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `mime-support=3.64ubuntu1`

Binary Packages:

- `mime-support=3.64ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.64ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.dsc' mime-support_3.64ubuntu1.dsc 1729 SHA256:669ba4f3fd7594f1c32731b5636b499f44f21c7667148f6f0d16043708743fdc
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.tar.xz' mime-support_3.64ubuntu1.tar.xz 33980 SHA256:5007d2ebc25935bfca6d4bdac0efdfc089a38c1be49d19f0422559f666e4f2c4
```

### `dpkg` source package: `mpclib3=1.2.0~rc1-1`

Binary Packages:

- `libmpc3:amd64=1.2.0~rc1-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.0~rc1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0~rc1-1.dsc' mpclib3_1.2.0~rc1-1.dsc 1879 SHA256:e01865ce9fd9fc07e60592c6a0314108e6988e51fb28977ac3003f2a61d49f6f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0~rc1.orig.tar.gz' mpclib3_1.2.0~rc1.orig.tar.gz 840338 SHA256:1f606dfa490c30beed05c47f595695c2d4205cc4f5c79cc9bdabd557f00f1b70
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0~rc1-1.diff.gz' mpclib3_1.2.0~rc1-1.diff.gz 4264 SHA256:8615b2944b3c9655073d5622f38236762b44137b48418e27904791794ec4f919
```

### `dpkg` source package: `mpfr4=4.1.0-3`

Binary Packages:

- `libmpfr6:amd64=4.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.1.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3.dsc' mpfr4_4.1.0-3.dsc 1959 SHA256:6d2727cf53e788020f671a2cba644ff5dd4e28a2531e66c3ed32d98ce2b5bf4e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA256:0c98a3f1732ff6ca4ea690552079da9c597872d30e96ec28414ee23c95558a7f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3.debian.tar.xz' mpfr4_4.1.0-3.debian.tar.xz 12372 SHA256:b329dd24cba377ed4160c0819a5ec110e029fb52c93e9a141847d5ed2a2068e8
```

### `dpkg` source package: `mysql-8.0=8.0.21-0ubuntu4`

Binary Packages:

- `libmysqlclient-dev=8.0.21-0ubuntu4`
- `libmysqlclient21:amd64=8.0.21-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libmysqlclient-dev/copyright`, `/usr/share/doc/libmysqlclient21/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-like`
- `Boost-1.0`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL`
- `LGPL-2`
- `public-domain`
- `zlib/libpng`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `mysql-defaults=1.0.5ubuntu2`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.5ubuntu2`
- `mysql-common=5.8+1.0.5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.dsc' mysql-defaults_1.0.5ubuntu2.dsc 2251 SHA256:788762eca77d2718a5ecc8e5fc49f90b32e81639a4a06169789e8f34fc35d379
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.tar.xz' mysql-defaults_1.0.5ubuntu2.tar.xz 7168 SHA256:d1b17de186bf8afba5cfc0041ab3c3646dbbed653e72010e2222bb52396e54c0
```

### `dpkg` source package: `ncurses=6.2-1`

Binary Packages:

- `libncurses-dev:amd64=6.2-1`
- `libncurses5-dev:amd64=6.2-1`
- `libncurses6:amd64=6.2-1`
- `libncursesw5-dev:amd64=6.2-1`
- `libncursesw6:amd64=6.2-1`
- `libtinfo6:amd64=6.2-1`
- `ncurses-base=6.2-1`
- `ncurses-bin=6.2-1`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-1.dsc' ncurses_6.2-1.dsc 4016 SHA256:fc81f03ae9d74b98a6ff6fe5e9a8339bbd71f19aa21f2b041ce5fbecc71cb472
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz' ncurses_6.2.orig.tar.gz 3425862 SHA256:30306e0c76e0f9f1f0de987cf1c82a5c21e1ce6568b9227f7da5b71cbea86c9d
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz.asc' ncurses_6.2.orig.tar.gz.asc 265 SHA256:8733e48fa7dafa61f3df67783402c3b2555fccccff44e912b436a7111b9c8781
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-1.debian.tar.xz' ncurses_6.2-1.debian.tar.xz 51276 SHA256:b5c4958529954ec70226cf73d5a848e2d159a2c2115faf57258009e28b2e110d
```

### `dpkg` source package: `netbase=6.1`

Binary Packages:

- `netbase=6.1`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.dsc' netbase_6.1.dsc 1480 SHA256:d3d24cf00001259d3311c0509b4e23ac150cffea27b546e3a204864f52824556
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.tar.xz' netbase_6.1.tar.xz 31984 SHA256:084d743bd84d4d9380bac4c71c51e57406dce44f5a69289bb823c903e9b035d8
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6-2.dsc' nettle_3.6-2.dsc 2254 SHA256:3d7c14776e74d14103f49455b1ae3c373bbb374af6f215071deecd436495b43a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6.orig.tar.gz' nettle_3.6.orig.tar.gz 2288173 SHA256:d24c0d0f2abffbc8f4f34dcf114b0f131ec3774895f3555922fe2f40f3d5e3f1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6.orig.tar.gz.asc' nettle_3.6.orig.tar.gz.asc 573 SHA256:f0ee81d3120bb85ce2adee753568f68361d33b3fe363b6a15462b06bb9518ad1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6-2.debian.tar.xz' nettle_3.6-2.debian.tar.xz 21136 SHA256:55c5e4471fbb92378c198a765135a7dcb327b84344a3ef2fa95340af1053313f
```

### `dpkg` source package: `nghttp2=1.41.0-2`

Binary Packages:

- `libnghttp2-14:amd64=1.41.0-2`

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
$ apt-get source -qq --print-uris nghttp2=1.41.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0-2.dsc' nghttp2_1.41.0-2.dsc 2548 SHA256:de017fb480273ab1f2a5581fd11773fdfbbb64685fe07a4398a98a02f3d7d76a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0.orig.tar.bz2' nghttp2_1.41.0.orig.tar.bz2 1943304 SHA256:645ca078e7ec276dcfa27175f3af6140c8badc7358ec9d2892b6ab2bcee72240
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0-2.debian.tar.xz' nghttp2_1.41.0-2.debian.tar.xz 13268 SHA256:ac0b8341728592ca0de4a73646c2c5c24b4d46df5e6e726b7816e9de52f1d0b2
```

### `dpkg` source package: `npth=1.6-2`

Binary Packages:

- `libnpth0:amd64=1.6-2`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-2.dsc' npth_1.6-2.dsc 1931 SHA256:7bb227f06b60eabbcc02a4fc4c46eba0aec430dda34b6bc7521c53deb9514a71
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA256:1393abd9adcf0762d34798dc34fdcf4d0d22a8410721e76f1e3afcd1daa4e2d1
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-2.debian.tar.xz' npth_1.6-2.debian.tar.xz 10612 SHA256:e848caf5b5296f7415a7af41f97bd9ec1fcc2b477cb134e4ee4309e15f84323a
```

### `dpkg` source package: `openexr=2.3.0-6ubuntu1`

Binary Packages:

- `libopenexr-dev=2.3.0-6ubuntu1`
- `libopenexr24:amd64=2.3.0-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr24/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.3.0-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0-6ubuntu1.dsc' openexr_2.3.0-6ubuntu1.dsc 2630 SHA256:b472f9871435ce5d4f60d4e2fd22aea47806f5471d9aac6cf21e5f06ea5f846c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0.orig.tar.gz' openexr_2.3.0.orig.tar.gz 18416222 SHA256:1dea3145eb3962025e27edb99c97e8cfc67d6310403bbd643e97c364ebf8ff09
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0.orig.tar.gz.asc' openexr_2.3.0.orig.tar.gz.asc 566 SHA256:809172c26aacae76d2caf92d13015ec829853f1ea9b25512c0307c66005e4dcc
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0-6ubuntu1.debian.tar.xz' openexr_2.3.0-6ubuntu1.debian.tar.xz 33684 SHA256:a8f7210fdaad28b8c97c3c1d32cfa6602682af9737381f52b505310f20e942c7
```

### `dpkg` source package: `openjpeg2=2.3.1-1ubuntu4`

Binary Packages:

- `libopenjp2-7:amd64=2.3.1-1ubuntu4`

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
$ apt-get source -qq --print-uris openjpeg2=2.3.1-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu4.dsc' openjpeg2_2.3.1-1ubuntu4.dsc 2842 SHA256:d1ce35b17b6c40cbea1a2291d94ee29fbd334ff622590e3939b749430a0d6e73
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1.orig.tar.xz' openjpeg2_2.3.1.orig.tar.xz 1381768 SHA256:69d39843a25f1a482e1b568fd042eb34837ffc0d708ab7717edeb52e592ecbeb
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu4.debian.tar.xz' openjpeg2_2.3.1-1ubuntu4.debian.tar.xz 21052 SHA256:b42c551474c33926840df7b8fe73d85fb1c5d2d28dc9c08b0ecb6be22af1edb9
```

### `dpkg` source package: `openldap=2.4.50+dfsg-1ubuntu3`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.50+dfsg-1ubuntu3`
- `libldap-common=2.4.50+dfsg-1ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.50+dfsg-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.50+dfsg-1ubuntu3.dsc' openldap_2.4.50+dfsg-1ubuntu3.dsc 3154 SHA256:7be737e116edc37ba62cae4d1495ff248122696975fd4345d32b481176956ea5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.50+dfsg.orig.tar.gz' openldap_2.4.50+dfsg.orig.tar.gz 4891077 SHA256:77e5be35661d2fb51c4425fc5985c668fa0e53cbc83a6c0962470fd240fd7655
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.50+dfsg-1ubuntu3.debian.tar.xz' openldap_2.4.50+dfsg-1ubuntu3.debian.tar.xz 181168 SHA256:630db2fc804a4fba21098a6245d4a6ab566747224345d265dbf7c5903d0e47df
```

### `dpkg` source package: `openssh=1:8.3p1-1`

Binary Packages:

- `openssh-client=1:8.3p1-1`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Beer-ware`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:8.3p1-1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1-1.dsc' openssh_8.3p1-1.dsc 3342 SHA256:7a0f9f0001d10bf6270b47e1c0c75d82e118234609bb75233ffd08877d0d3186
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1.orig.tar.gz' openssh_8.3p1.orig.tar.gz 1706358 SHA256:f2befbe0472fe7eb75d23340eb17531cb6b3aac24075e2066b41f814e12387b2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1.orig.tar.gz.asc' openssh_8.3p1.orig.tar.gz.asc 683 SHA256:c5a5f84a482c93ee59eccb8f9f76b6c70eed56fd9b059fc72b3184effa8135f5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1-1.debian.tar.xz' openssh_8.3p1-1.debian.tar.xz 176252 SHA256:edeb381f43f9b4399fa34f3fab40d60617f3391774304493f2ee7a8dba214ba9
```

### `dpkg` source package: `openssl=1.1.1f-1ubuntu3`

Binary Packages:

- `libssl-dev:amd64=1.1.1f-1ubuntu3`
- `libssl1.1:amd64=1.1.1f-1ubuntu3`
- `openssl=1.1.1f-1ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1f-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu3.dsc' openssl_1.1.1f-1ubuntu3.dsc 2705 SHA256:3b58d6628e89793a297bc5591901bfe3374a708042d384df6e8ec908e5e3c39c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz' openssl_1.1.1f.orig.tar.gz 9792828 SHA256:186c6bfe6ecfba7a5b48c47f8a1673d0f3b0e5ba2e25602dd23b629975da3f35
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz.asc' openssl_1.1.1f.orig.tar.gz.asc 488 SHA256:e9c68097b05be8873e41bd33a9269378ca58e515fbaa30a512c315b602d41dda
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu3.debian.tar.xz' openssl_1.1.1f-1ubuntu3.debian.tar.xz 145256 SHA256:dd675e883550730e221da191588a0b27a5a76115f754e37672681d198505411a
```

### `dpkg` source package: `p11-kit=0.23.20-1build1`

Binary Packages:

- `libp11-kit0:amd64=0.23.20-1build1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pam=1.3.1-5ubuntu5`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu5`
- `libpam-modules-bin=1.3.1-5ubuntu5`
- `libpam-runtime=1.3.1-5ubuntu5`
- `libpam0g:amd64=1.3.1-5ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pango1.0=1.46.0-2`

Binary Packages:

- `libpango-1.0-0:amd64=1.46.0-2`
- `libpangocairo-1.0-0:amd64=1.46.0-2`
- `libpangoft2-1.0-0:amd64=1.46.0-2`

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
$ apt-get source -qq --print-uris pango1.0=1.46.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.46.0-2.dsc' pango1.0_1.46.0-2.dsc 3581 SHA256:2f66f2050614ba0d51852549bb9790baa5ebd3245987614b9557af75692cee34
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.46.0.orig.tar.xz' pango1.0_1.46.0.orig.tar.xz 532168 SHA256:9a81572ebb946187fbdd69d5ffc57e2f7a1f768cd8d2fd89dbb03fb9002a99b5
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.46.0-2.debian.tar.xz' pango1.0_1.46.0-2.debian.tar.xz 34332 SHA256:3d6acb8c28e148381043a939b30218769db06a768e54e23e1b741070f066631d
```

### `dpkg` source package: `patch=2.7.6-6`

Binary Packages:

- `patch=2.7.6-6`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-6
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-6.dsc' patch_2.7.6-6.dsc 1699 SHA256:ad31c243b982ad8dede14f7b4dfe5bb798bb1dc6d4e28c51a797c3af58477c13
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-6.debian.tar.xz' patch_2.7.6-6.debian.tar.xz 14464 SHA256:75ea94b265763b65005381f1eceeaf3351a70ec5c3243bc161d702776414db02
```

### `dpkg` source package: `patiencediff=0.1.0-2build2`

Binary Packages:

- `python3-patiencediff=0.1.0-2build2`

Licenses: (parsed from: `/usr/share/doc/python3-patiencediff/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris patiencediff=0.1.0-2build2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/patiencediff/patiencediff_0.1.0-2build2.dsc' patiencediff_0.1.0-2build2.dsc 2198 SHA256:f47c883408b3a849d8a867ae17f3bec328ce90ff2102da7cc8c491368cd0d4f4
'http://archive.ubuntu.com/ubuntu/pool/universe/p/patiencediff/patiencediff_0.1.0.orig.tar.gz' patiencediff_0.1.0.orig.tar.gz 19965 SHA256:7cd316f57f7b4086923cc0db80273886416134d82945dddd0aa24f0e95c7d302
'http://archive.ubuntu.com/ubuntu/pool/universe/p/patiencediff/patiencediff_0.1.0-2build2.debian.tar.xz' patiencediff_0.1.0-2build2.debian.tar.xz 42868 SHA256:de6ab7a66aa8f13b6be2a3303b35d89d04a0e516c45c049f14c4d38bab2fc1ee
```

### `dpkg` source package: `pcre2=10.34-7`

Binary Packages:

- `libpcre2-16-0:amd64=10.34-7`
- `libpcre2-32-0:amd64=10.34-7`
- `libpcre2-8-0:amd64=10.34-7`
- `libpcre2-dev:amd64=10.34-7`
- `libpcre2-posix2:amd64=10.34-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.34-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.dsc' pcre2_10.34-7.dsc 2286 SHA256:c3e2bfd8fabf594238b3f17074dc8ac483aaf80a9f12dbfe927b80a74558732e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34.orig.tar.gz' pcre2_10.34.orig.tar.gz 2271533 SHA256:da6aba7ba2509e918e41f4f744a59fa41a2425c59a298a232e7fe85691e00379
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.diff.gz' pcre2_10.34-7.diff.gz 7068 SHA256:7d44ac1b171ef7f7051213a3a8505b28f3809ed3e2fb348567a29fdf5f2b5fdf
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.dsc' pcre3_8.39-13.dsc 2226 SHA256:c3a2eb4f02de5b2e00787ed2a35eb82f04ee4b5e99b8ff279bae3c6453aad93b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.debian.tar.gz' pcre3_8.39-13.debian.tar.gz 27002 SHA256:a2143d7358d69b61955a4f977980050447f8891c0e6737080f2b14b920fbde87
```

### `dpkg` source package: `perl=5.30.3-4`

Binary Packages:

- `libperl5.30:amd64=5.30.3-4`
- `perl=5.30.3-4`
- `perl-base=5.30.3-4`
- `perl-modules-5.30=5.30.3-4`

Licenses: (parsed from: `/usr/share/doc/libperl5.30/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.30/copyright`)

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
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3-4.dsc' perl_5.30.3-4.dsc 2983 SHA256:05c8d356f72848b6e26b57949b5fb7dcc6340719df292f83d02ff05fb84cdd98
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3.orig-regen-configure.tar.gz' perl_5.30.3.orig-regen-configure.tar.gz 870970 SHA256:99174174fbfc550f801076ab8a1a5831c92f75c1b81e553150351f14a111dcf8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3.orig.tar.xz' perl_5.30.3.orig.tar.xz 12375128 SHA256:6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3-4.debian.tar.xz' perl_5.30.3-4.debian.tar.xz 171184 SHA256:a71ed73cab42cadb8cb9efe430ac075e644fea527f3689b64e4e0fe8b9648ffd
```

### `dpkg` source package: `pinentry=1.1.0-4build1`

Binary Packages:

- `pinentry-curses=1.1.0-4build1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.dsc' pinentry_1.1.0-4build1.dsc 2595 SHA256:37fbbefc36e4041a80b0e7b4d9770899a3098a1975531e2b84da6914dbe04557
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.debian.tar.xz' pinentry_1.1.0-4build1.debian.tar.xz 17312 SHA256:ccccd3ee3b589456a5e26883608cf75da6e49a9c0e161191c35ceaf509d64489
```

### `dpkg` source package: `pixman=0.38.4-0ubuntu1`

Binary Packages:

- `libpixman-1-0:amd64=0.38.4-0ubuntu1`
- `libpixman-1-dev:amd64=0.38.4-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.38.4-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.38.4-0ubuntu1.dsc' pixman_0.38.4-0ubuntu1.dsc 1468 SHA256:310e4d2fb12e80dc9f11e7c29332f40f5830b98c06b45e0cd62181feea0d7165
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.38.4.orig.tar.gz' pixman_0.38.4.orig.tar.gz 897926 SHA256:da66d6fd6e40aee70f7bd02e4f8f76fc3f006ec879d346bae6a723025cfbdde7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.38.4-0ubuntu1.diff.gz' pixman_0.38.4-0ubuntu1.diff.gz 322901 SHA256:7a7ed16483d2bc68a18769828450d941b1eb8fd0934a275c09502a0075dcccdc
```

### `dpkg` source package: `pkg-config=0.29.2-1ubuntu1`

Binary Packages:

- `pkg-config=0.29.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu1.dsc' pkg-config_0.29.2-1ubuntu1.dsc 1799 SHA256:f6bf9c29157779233b45c0cb849162842724cfd6b94bf8311f0ee744b4f5cdbe
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2.orig.tar.gz' pkg-config_0.29.2.orig.tar.gz 2016830 SHA256:6fc69c01688c9458a57eb9a1664c9aba372ccda420a02bf4429fe610e7e7d591
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu1.diff.gz' pkg-config_0.29.2-1ubuntu1.diff.gz 9852 SHA256:5e9d84b6dc14d7a66e81dc164ea27304f87ae0f0793c876e9f8192ed7ec89352
```

### `dpkg` source package: `postgresql-12=12.3-1build1`

Binary Packages:

- `libpq-dev=12.3-1build1`
- `libpq5:amd64=12.3-1build1`

Licenses: (parsed from: `/usr/share/doc/libpq-dev/copyright`, `/usr/share/doc/libpq5/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-Clause`
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

Source:

```console
$ apt-get source -qq --print-uris postgresql-12=12.3-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.3-1build1.dsc' postgresql-12_12.3-1build1.dsc 3761 SHA256:9a1c87c273055ee9b2e26eb54a99db1b2ff474cfe7e68a96dda3c3a75f9ed9d5
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.3.orig.tar.bz2' postgresql-12_12.3.orig.tar.bz2 20439892 SHA256:94ed64a6179048190695c86ec707cc25d016056ce10fc9d229267d9a8f1dcf41
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.3-1build1.debian.tar.xz' postgresql-12_12.3-1build1.debian.tar.xz 23128 SHA256:2c8e5b00355ef6073e620781b8c635c4a0d2a19c5ebee7fd5be725e09881c260
```

### `dpkg` source package: `procps=2:3.3.16-5ubuntu1`

Binary Packages:

- `libprocps8:amd64=2:3.3.16-5ubuntu1`
- `procps=2:3.3.16-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.16-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-5ubuntu1.dsc' procps_3.3.16-5ubuntu1.dsc 2271 SHA256:f3ba7b03cb6bacb7ae06646ab34757d4de6f93a046304dbf8ebfe48be51cb16b
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16.orig.tar.xz' procps_3.3.16.orig.tar.xz 621892 SHA256:2919299e579d29be3501a802dfe77e6f23be228149d0396d83d0ffbe8fa7efbf
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-5ubuntu1.debian.tar.xz' procps_3.3.16-5ubuntu1.debian.tar.xz 33768 SHA256:70672be61b079e25f078ad93ae3a63ac318a013649d6b6c391b020ca01516bce
```

### `dpkg` source package: `python-certifi=2020.4.5.1-1`

Binary Packages:

- `python3-certifi=2020.4.5.1-1`

Licenses: (parsed from: `/usr/share/doc/python3-certifi/copyright`)

- `GPL-2`
- `MPL-2`

Source:

```console
$ apt-get source -qq --print-uris python-certifi=2020.4.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1-1.dsc' python-certifi_2020.4.5.1-1.dsc 1634 SHA256:fc08f36819c72391207038f5aeb0ee26e8b09238930cba8fb51ad6d3509e58f1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1.orig.tar.xz' python-certifi_2020.4.5.1.orig.tar.xz 144464 SHA256:99350293fccff4fb1e7c4a60ce09519704dce14fc347c18dc915699eb033a758
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1-1.debian.tar.xz' python-certifi_2020.4.5.1-1.debian.tar.xz 7732 SHA256:3c23ee1a03b3b242df921a55fd360d2deb7ca15d8879c72a4987aec1b99c88ed
```

### `dpkg` source package: `python-fastimport=0.9.8-5build1`

Binary Packages:

- `python3-fastimport=0.9.8-5build1`

Licenses: (parsed from: `/usr/share/doc/python3-fastimport/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris python-fastimport=0.9.8-5build1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8-5build1.dsc' python-fastimport_0.9.8-5build1.dsc 2244 SHA256:2ca7934d75936cc98c4520b19844a02ba23c7325116dd0cd37b55a0265dbbf0f
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8.orig.tar.gz' python-fastimport_0.9.8.orig.tar.gz 39512 SHA256:b2f2e8eb97000256e1aab83d2a0a053fc7b93c3aa4f7e9b971a5703dfc5963b9
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8-5build1.debian.tar.xz' python-fastimport_0.9.8-5build1.debian.tar.xz 13644 SHA256:f83a7b8f5824f22c46aacb7ededbed2d801cbcedf67500c5ac3bc71aa6aa981c
```

### `dpkg` source package: `python-urllib3=1.25.9-1`

Binary Packages:

- `python3-urllib3=1.25.9-1`

Licenses: (parsed from: `/usr/share/doc/python3-urllib3/copyright`)

- `Expat`
- `PSF-2`

Source:

```console
$ apt-get source -qq --print-uris python-urllib3=1.25.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9-1.dsc' python-urllib3_1.25.9-1.dsc 2217 SHA256:156567637b749e5070162a3ff3470d0e98c50c93769c925fbabcd483b0bccc07
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9.orig.tar.gz' python-urllib3_1.25.9.orig.tar.gz 254921 SHA256:3018294ebefce6572a474f0604c2021e33b3fd8006ecd11d62107a5d2a963527
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9-1.debian.tar.xz' python-urllib3_1.25.9-1.debian.tar.xz 11472 SHA256:ddf5629ac197176e0d49aac038eac2090dde93f75b33b09988a3bb46e77de146
```

### `dpkg` source package: `python3-defaults=3.8.2-0ubuntu2`

Binary Packages:

- `libpython3-stdlib:amd64=3.8.2-0ubuntu2`
- `python3=3.8.2-0ubuntu2`
- `python3-minimal=3.8.2-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.8.2-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.8.2-0ubuntu2.dsc' python3-defaults_3.8.2-0ubuntu2.dsc 2879 SHA256:3fa296ea2cd52738ebc44a1b83a8df500bf654356336d9bf057144171fe9ee7d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.8.2-0ubuntu2.tar.gz' python3-defaults_3.8.2-0ubuntu2.tar.gz 138226 SHA256:e4969a54306421ebfd195d0c064935db7c53f9f152d8abaae63da33819235e9a
```

### `dpkg` source package: `python3-stdlib-extensions=3.8.5-1`

Binary Packages:

- `python3-distutils=3.8.5-1`
- `python3-lib2to3=3.8.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.8.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.5-1.dsc' python3-stdlib-extensions_3.8.5-1.dsc 2524 SHA256:7d755665c29938c4f1f39ef133701865abd47118f078a9153d136453277a785d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.5.orig.tar.xz' python3-stdlib-extensions_3.8.5.orig.tar.xz 1074164 SHA256:b8cae96587edc5ec8f7dc2d97ace0e1569c3137e206b9db6e720eef186c3deb9
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.5-1.debian.tar.xz' python3-stdlib-extensions_3.8.5-1.debian.tar.xz 17896 SHA256:c9374aa01e08a4a41cd979300f0f12fc5348672a2425cc11ca3c0bead3c011b0
```

### `dpkg` source package: `python3.8=3.8.5-2`

Binary Packages:

- `libpython3.8-minimal:amd64=3.8.5-2`
- `libpython3.8-stdlib:amd64=3.8.5-2`
- `python3.8=3.8.5-2`
- `python3.8-minimal=3.8.5-2`

Licenses: (parsed from: `/usr/share/doc/libpython3.8-minimal/copyright`, `/usr/share/doc/libpython3.8-stdlib/copyright`, `/usr/share/doc/python3.8/copyright`, `/usr/share/doc/python3.8-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.8=3.8.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.8/python3.8_3.8.5-2.dsc' python3.8_3.8.5-2.dsc 3293 SHA256:bb8727d0c147bd6a48697dc298d956c44f24954f555e7f031f23587038ebfbaf
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.8/python3.8_3.8.5.orig.tar.xz' python3.8_3.8.5.orig.tar.xz 18019640 SHA256:e3003ed57db17e617acb382b0cade29a248c6026b1bd8aad1f976e9af66a83b0
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.8/python3.8_3.8.5-2.debian.tar.xz' python3.8_3.8.5-2.debian.tar.xz 210232 SHA256:e9f388751a6f1722f11028263fbb0e7eddc176c166d46094dd7117a6ff7d9fc4
```

### `dpkg` source package: `readline=8.0-4`

Binary Packages:

- `libreadline-dev:amd64=8.0-4`
- `libreadline8:amd64=8.0-4`
- `readline-common=8.0-4`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.dsc' readline_8.0-4.dsc 2434 SHA256:ac9c7bb7380fe740aef09f54becf482eb81032a33dc11f1a8f00e933c5f168f4
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0.orig.tar.gz' readline_8.0.orig.tar.gz 2975937 SHA256:e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.debian.tar.xz' readline_8.0-4.debian.tar.xz 30408 SHA256:60ed18dab6d6b7fc998a263d917f06d9cce6e1ccd19cd8bf4a9d33c5350cf8d6
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2build2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2build2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build2.dsc 2402 SHA256:4c364d1f8f879ce501bc7a9b3f69ca555e2ab8a9df18ef88f729d800f51ad825
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build2.debian.tar.xz 8276 SHA256:e1f8346afb06a7d29c5c4c276dcccd42b1ebb40d9d30561a4066e1bc7a5620fb
```

### `dpkg` source package: `sed=4.7-1build1`

Binary Packages:

- `sed=4.7-1build1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.7-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1build1.dsc' sed_4.7-1build1.dsc 1958 SHA256:2687e4e462fd4943f856d990115efe8449a4413baf56cf82e6bb199fcee09aa9
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7.orig.tar.xz' sed_4.7.orig.tar.xz 1298316 SHA256:2885768cd0a29ff8d58a6280a270ff161f6a3deb5690b2be6c49f46d4c67bd6a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1build1.debian.tar.xz' sed_4.7-1build1.debian.tar.xz 59956 SHA256:89192d49bc4e58bab6e890f46832bbd78ab1210604af5c3a29003c1987ec5908
```

### `dpkg` source package: `sensible-utils=0.0.12+nmu1`

Binary Packages:

- `sensible-utils=0.0.12+nmu1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sensible-utils/0.0.12+nmu1/


### `dpkg` source package: `serf=1.3.9-8build1`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-8build1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `shadow=1:4.8.1-1ubuntu6`

Binary Packages:

- `login=1:4.8.1-1ubuntu6`
- `passwd=1:4.8.1-1ubuntu6`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu6.dsc' shadow_4.8.1-1ubuntu6.dsc 1705 SHA256:f74fd356e3d237624704a1698da160f28f87d780f1d989ad3f494a924242e7c6
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA256:a3ad4630bdc41372f02a647278a8c3514844295d36eefe68ece6c3a641c1ae62
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu6.debian.tar.xz' shadow_4.8.1-1ubuntu6.debian.tar.xz 85620 SHA256:d45a2d33774f455295be012e9828d99dc6cb7cf1bc76ba12e0cfc55296740b20
```

### `dpkg` source package: `shared-mime-info=1.15-1`

Binary Packages:

- `shared-mime-info=1.15-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.15-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15-1.dsc' shared-mime-info_1.15-1.dsc 2198 SHA256:dca6ea0156110b4a2694dd96a721d34ad4f42b51f3d3a20d0d711b77bde5115d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15.orig.tar.xz' shared-mime-info_1.15.orig.tar.xz 772708 SHA256:f482b027437c99e53b81037a9843fccd549243fd52145d016e9c7174a4f5db90
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15-1.debian.tar.xz' shared-mime-info_1.15-1.debian.tar.xz 9728 SHA256:02c4fa8b2b3073c745287dd0e00c69c9f1ba028c7c6496105e3ecdcc02d9f1dd
```

### `dpkg` source package: `six=1.15.0-1`

Binary Packages:

- `python3-six=1.15.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.15.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0-1.dsc' six_1.15.0-1.dsc 2411 SHA256:7a7899358165af2c5e1d9c939b5f66fadb83ef7bc4a806bded01121088bde00c
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0.orig.tar.gz' six_1.15.0.orig.tar.gz 33917 SHA256:30639c035cdb23534cd4aa2dd52c3bf48f06e5f4a941509c8bafd8ce11080259
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0-1.debian.tar.xz' six_1.15.0-1.debian.tar.xz 4480 SHA256:6ccff1bff18fe0de27bc90c652fa8e5f3822c66020e533a9c40fd45b8cefe760
```

### `dpkg` source package: `sqlite3=3.32.3-1`

Binary Packages:

- `libsqlite3-0:amd64=3.32.3-1`
- `libsqlite3-dev:amd64=3.32.3-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.32.3-1/


### `dpkg` source package: `subversion=1.14.0-1`

Binary Packages:

- `libsvn1:amd64=1.14.0-1`
- `subversion=1.14.0-1`

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
$ apt-get source -qq --print-uris subversion=1.14.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0-1.dsc' subversion_1.14.0-1.dsc 3807 SHA256:efb177ab8d566c8dadd01919cb114264961d84e9f0c7ea24a78234ff1f267ea5
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0.orig.tar.gz' subversion_1.14.0.orig.tar.gz 11519871 SHA256:ef3d1147535e41874c304fb5b9ea32745fbf5d7faecf2ce21d4115b567e937d0
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0.orig.tar.gz.asc' subversion_1.14.0.orig.tar.gz.asc 3917 SHA256:98333df38d29a64500d4ad1693741d3d087485555207289b4e53af309abac71a
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0-1.debian.tar.xz' subversion_1.14.0-1.debian.tar.xz 426604 SHA256:2df3c0e9ad9f8ef33d5d3c2ffc19c89b5d0cb8850c526842baa356ca85ac3e3c
```

### `dpkg` source package: `systemd=245.7-1ubuntu1`

Binary Packages:

- `libsystemd0:amd64=245.7-1ubuntu1`
- `libudev1:amd64=245.7-1ubuntu1`

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


### `dpkg` source package: `sysvinit=2.96-3ubuntu1`

Binary Packages:

- `sysvinit-utils=2.96-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-3ubuntu1.dsc' sysvinit_2.96-3ubuntu1.dsc 2781 SHA256:64bab02372e0400ceeb1937a77f127246ae8c6ce63dbebdf309c483bb35179e0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA256:2a2e26b72aa235a23ab1c8471005f890309ce1196c83fbc9413c57b9ab62b587
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA256:dfc184b95da12c8c888c8ae6b0f26fe8a23b07fbcdd240f6600a8a78b9439fa0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-3ubuntu1.debian.tar.xz' sysvinit_2.96-3ubuntu1.debian.tar.xz 128020 SHA256:ce2ed9502ae88eda25db4896ba1bc881794f026b0b8c47419358b2fbd92d8533
```

### `dpkg` source package: `tar=1.30+dfsg-7`

Binary Packages:

- `tar=1.30+dfsg-7`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.30+dfsg-7
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.dsc' tar_1.30+dfsg-7.dsc 1981 SHA256:5117afe47b5aab94c592d52c11c74dba146a11a7cdc22dbe067a4b5a5e895729
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA256:c02f3747ffe02017878303dde8b78e79cd220364c5e8048cf92320232e38912d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.debian.tar.xz' tar_1.30+dfsg-7.debian.tar.xz 22168 SHA256:12763df7f214458a56edc4a4b27adb2cb2041d597d74212ba34736f02bb68cd3
```

### `dpkg` source package: `tiff=4.1.0+git191117-2build1`

Binary Packages:

- `libtiff-dev:amd64=4.1.0+git191117-2build1`
- `libtiff5:amd64=4.1.0+git191117-2build1`
- `libtiffxx5:amd64=4.1.0+git191117-2build1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.1.0+git191117-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117-2build1.dsc' tiff_4.1.0+git191117-2build1.dsc 2291 SHA256:18dad308fbc18f27de10de1b83d315a31aca20449651c01767993dfcabbb7ba0
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117.orig.tar.xz' tiff_4.1.0+git191117.orig.tar.xz 1533524 SHA256:67e1d045e994adb7144b0cca228d70dd6d520aaf8c75c342064bc0fd601e6e42
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117-2build1.debian.tar.xz' tiff_4.1.0+git191117-2build1.debian.tar.xz 19460 SHA256:4a78c0fbfdc708793d23c7030f2b5ee5ac2752f64efa40ef62864f0fe9d867f5
```

### `dpkg` source package: `ubuntu-keyring=2020.06.17.1`

Binary Packages:

- `ubuntu-keyring=2020.06.17.1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2020.06.17.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.dsc' ubuntu-keyring_2020.06.17.1.dsc 1863 SHA256:9ac7c2d8d5b4132872ef2e5a7ece4f73249e53d2aa36b075697e454e643e7ae6
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.tar.gz' ubuntu-keyring_2020.06.17.1.tar.gz 36420 SHA256:e31ba06e1332002e0649c206f54fa67fee038e27f43b9e59e872f1de14a00774
```

### `dpkg` source package: `ucf=3.0043`

Binary Packages:

- `ucf=3.0043`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0043
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043.dsc' ucf_3.0043.dsc 1423 SHA256:5954508238ff1b8e2c61e1f533268911ba06709e821c02de014fd15d2ead81fd
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043.tar.xz' ucf_3.0043.tar.xz 70560 SHA256:0294cc11a6cf032ea99ca5064f73a4ede5b28bc2d4ad0a12e8493c7520c7a2a4
```

### `dpkg` source package: `unzip=6.0-25ubuntu1`

Binary Packages:

- `unzip=6.0-25ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-25ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-25ubuntu1.dsc' unzip_6.0-25ubuntu1.dsc 1833 SHA256:893fcd9e73c91c4df06716f9620adf1ec701a4846b6269c513785a125e55550c
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-25ubuntu1.debian.tar.xz' unzip_6.0-25ubuntu1.debian.tar.xz 26276 SHA256:6a22b0d23cf8b9e1a74626d7d9af5efe1257e157f20006272dc68693a13f3b45
```

### `dpkg` source package: `utf8proc=2.5.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.5.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.5.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0-1.dsc' utf8proc_2.5.0-1.dsc 2154 SHA256:2137104a3712875650629305fe7d7ef37d4d99328846c18b087b289c0ddbf27c
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0.orig.tar.gz' utf8proc_2.5.0.orig.tar.gz 155485 SHA256:d4e8dfc898cfd062493cb7f42d95d70ccdd3a4cd4d90bec0c71b47cca688f1be
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0-1.debian.tar.xz' utf8proc_2.5.0-1.debian.tar.xz 5240 SHA256:333496cf4e178b5ccf4972fa52523d07a21a0cabf0cb123133c6c71f98e92eff
```

### `dpkg` source package: `util-linux=2.36-2ubuntu1`

Binary Packages:

- `bsdutils=1:2.36-2ubuntu1`
- `libblkid-dev:amd64=2.36-2ubuntu1`
- `libblkid1:amd64=2.36-2ubuntu1`
- `libmount-dev:amd64=2.36-2ubuntu1`
- `libmount1:amd64=2.36-2ubuntu1`
- `libsmartcols1:amd64=2.36-2ubuntu1`
- `libuuid1:amd64=2.36-2ubuntu1`
- `mount=2.36-2ubuntu1`
- `util-linux=2.36-2ubuntu1`
- `uuid-dev:amd64=2.36-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.36-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36-2ubuntu1.dsc' util-linux_2.36-2ubuntu1.dsc 4329 SHA256:a8d8d8abcb5c3a7f0074118e0d96001030cfaf3953c19ce97d0af007c9a42d70
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.orig.tar.xz' util-linux_2.36.orig.tar.xz 5242420 SHA256:9e4b1c67eb13b9b67feb32ae1dc0d50e08ce9e5d82e1cccd0ee771ad2fa9e0b1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36-2ubuntu1.debian.tar.xz' util-linux_2.36-2ubuntu1.debian.tar.xz 98844 SHA256:f6d063af7f4b3bf1214c672696fe0a95fa28530c91f1097ff5f72fc27d50d581
```

### `dpkg` source package: `wget=1.20.3-1ubuntu1`

Binary Packages:

- `wget=1.20.3-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.20.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3-1ubuntu1.dsc' wget_1.20.3-1ubuntu1.dsc 2280 SHA256:e40e00e9f93f1c049cd2b7942c9c9e31504acd56350b31f1ecad6ae220a44dfd
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3.orig.tar.gz' wget_1.20.3.orig.tar.gz 4489249 SHA256:31cccfc6630528db1c8e3a06f6decf2a370060b982841cfab2b8677400a5092e
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3.orig.tar.gz.asc' wget_1.20.3.orig.tar.gz.asc 833 SHA256:7b295c84ab6f90c328a203e234e4b2f5f45cb8d2e29eac43a977073933cd49a2
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3-1ubuntu1.debian.tar.xz' wget_1.20.3-1ubuntu1.debian.tar.xz 63312 SHA256:95ae56081866b9e6dfb2a2d2dc2208ba0cf3c76bb5d7e680cc56b18b3ec66c1e
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

### `dpkg` source package: `xorg=1:7.7+19ubuntu14`

Binary Packages:

- `x11-common=1:7.7+19ubuntu14`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19ubuntu14
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu14.dsc' xorg_7.7+19ubuntu14.dsc 2107 SHA256:d9d6449510066c3b34216cf08f797f00f64df3494567b5478a60d0feb50b9d95
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu14.tar.gz' xorg_7.7+19ubuntu14.tar.gz 299269 SHA256:b8a1c0f7b24ae5565f6f22ccf01cd0c8e46c4f5dad6c14bce4f3495e82138213
```

### `dpkg` source package: `xorgproto=2019.2-1ubuntu1`

Binary Packages:

- `x11proto-core-dev=2019.2-1ubuntu1`
- `x11proto-dev=2019.2-1ubuntu1`
- `x11proto-xext-dev=2019.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`, `/usr/share/doc/x11proto-xext-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2019.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2019.2-1ubuntu1.dsc' xorgproto_2019.2-1ubuntu1.dsc 4096 SHA256:1b0fede1501745c7cfed22b86ea951ba6792ae6eda404fafae9533b01fbb2ee2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2019.2.orig.tar.gz' xorgproto_2019.2.orig.tar.gz 1080686 SHA256:ebfcfce48b66bec25d5dff0e9510e04053ef78e51a8eabeeee4c00e399226d61
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2019.2.orig.tar.gz.asc' xorgproto_2019.2.orig.tar.gz.asc 659 SHA256:75da45caac1d85fe37a5e7f33a087d456cad1dc38f2743b7f7df63d7ca583293
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2019.2-1ubuntu1.diff.gz' xorgproto_2019.2-1ubuntu1.diff.gz 21111 SHA256:9162224ecb85b35b37a51fbb2a1c53fc8262339fd3208ded60e141607aa835e8
```

### `dpkg` source package: `xtrans=1.4.0-1`

Binary Packages:

- `xtrans-dev=1.4.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xtrans=1.4.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.4.0-1.dsc' xtrans_1.4.0-1.dsc 1919 SHA256:dd74ab9199e8f45215b566a9317cac7953bf063ce6893c185eccaf0fb4d84d8f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.4.0.orig.tar.gz' xtrans_1.4.0.orig.tar.gz 225941 SHA256:48ed850ce772fef1b44ca23639b0a57e38884045ed2cbb18ab137ef33ec713f9
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.4.0-1.diff.gz' xtrans_1.4.0-1.diff.gz 9522 SHA256:0dac18165654d79e0796b80fab4c1104998d29e6d0b098af0426a1d72399521e
```

### `dpkg` source package: `xz-utils=5.2.4-1ubuntu1`

Binary Packages:

- `liblzma-dev:amd64=5.2.4-1ubuntu1`
- `liblzma5:amd64=5.2.4-1ubuntu1`
- `xz-utils=5.2.4-1ubuntu1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.dsc' xz-utils_5.2.4-1ubuntu1.dsc 2629 SHA256:ef1afb534aae085f0f1265a0b282be3c839b97f5fd30ed652826aeb81b132724
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA256:9717ae363760dedf573dad241420c5fea86256b65bc21d2cf71b2b12f0544f4b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA256:88290c1deeaf674ae2a4821f4373fe0e4cc2a94199eae6dcc26df1e70cc15303
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.debian.tar.xz' xz-utils_5.2.4-1ubuntu1.debian.tar.xz 135512 SHA256:daaa79e97b131e18381c05ed3b7cb878acd6c6f7341779039d7a2af765f37627
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu1`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu1`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu1.dsc' zlib_1.2.11.dfsg-2ubuntu1.dsc 2970 SHA256:2e56b0d54d841d974c96e6cc4361da7c75b1848cded85412cdb4b4bc7791233a
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu1.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu1.debian.tar.xz 49448 SHA256:11c13ba58bd033dbfd2c7408f4a4eaa02035e007dea79ae20f0db580eaa53c9c
```
