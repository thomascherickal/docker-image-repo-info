# `buildpack-deps:focal`

## Docker Metadata

- Image ID: `sha256:9c25d4c50b24ccab9932177b660c2ad31e1d9aaf5588a1d6bc8330903350b2f9`
- Created: `2019-12-19T07:34:57.007745778Z`
- Virtual Size: ~ 701.11 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-5`

Binary Packages:

- `libacl1:amd64=2.2.53-5`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-5
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-5ubuntu1.dsc' acl_2.2.53-5ubuntu1.dsc 2480 SHA256:926f984b2b0a546290247154b73e716eb16c79831c2adea74fc0e4f1e0e4f6a1
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-5ubuntu1.debian.tar.xz' acl_2.2.53-5ubuntu1.debian.tar.xz 22460 SHA256:2d92cc49cab36f19d2ae0c89aa9a27aa94519cc1b6a75f1932a2e482c8036f15
```

### `dpkg` source package: `adduser=3.118ubuntu1`

Binary Packages:

- `adduser=3.118ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.118ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu1.dsc' adduser_3.118ubuntu1.dsc 1808 SHA256:415e093e945d4a37679504f4f54e0fcd903c4f524dd90526440965aea7bba77c
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu1.tar.xz' adduser_3.118ubuntu1.tar.xz 217300 SHA256:16e8d59231d814af0701a24195246f169a26df1b39d59e3cea04db882a31973a
```

### `dpkg` source package: `apr-util=1.6.1-4build1`

Binary Packages:

- `libaprutil1:amd64=1.6.1-4build1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4build1.dsc' apr-util_1.6.1-4build1.dsc 2838 SHA256:eb38c2580ebca1cb794cac38dc0f38fc1b313b6a95740b9bde3fd0f2aecb1bc1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2.asc' apr-util_1.6.1.orig.tar.bz2.asc 801 SHA256:47837b605290c0d7659b73734e4a9d5e6c0c24c13185cd4d91837afe63c07ca4
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4build1.debian.tar.xz' apr-util_1.6.1-4build1.debian.tar.xz 212508 SHA256:62d45d064dabcced9dcf418a5ecaff3de56a082cb8edb064becf89eb2cba05c4
```

### `dpkg` source package: `apr=1.6.5-1`

Binary Packages:

- `libapr1:amd64=1.6.5-1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1.dsc' apr_1.6.5-1.dsc 2296 SHA256:80c471107d7f90ab5de012e4211559f4f6852ca2b7fd6911f06420aa66d27ec0
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2' apr_1.6.5.orig.tar.bz2 855393 SHA256:a67ca9fcf9c4ff59bce7f428a323c8b5e18667fdea7b0ebad47d194371b0a105
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2.asc' apr_1.6.5.orig.tar.bz2.asc 801 SHA256:9beff0bb06f4cbbb006176af93258d946d33b7fb54aac13a4c90cfba1cfd0c88
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1.debian.tar.xz' apr_1.6.5-1.debian.tar.xz 213168 SHA256:cb03a6ad0b8c525c67744e7d3f7c52af446e73bd6d4eeb6fd4622677df60db2b
```

### `dpkg` source package: `apt=1.9.4`

Binary Packages:

- `apt=1.9.4`
- `libapt-pkg5.90:amd64=1.9.4`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.90/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/1.9.4/


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

### `dpkg` source package: `audit=1:2.8.5-2ubuntu3`

Binary Packages:

- `libaudit-common=1:2.8.5-2ubuntu3`
- `libaudit1:amd64=1:2.8.5-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `autoconf=2.69-11ubuntu1`

Binary Packages:

- `autoconf=2.69-11ubuntu1`

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
$ apt-get source -qq --print-uris autoconf=2.69-11ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11ubuntu1.dsc' autoconf_2.69-11ubuntu1.dsc 2100 SHA256:0731cfd07f7453722deac31c9a6059bfa9f8b99d267841f30c9c791d524c0f2f
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11ubuntu1.debian.tar.xz' autoconf_2.69-11ubuntu1.debian.tar.xz 23684 SHA256:945b2c898c9b2a08979a52cee3f9cd2354e2c8a96aa12506cb5270cb87fa83a6
```

### `dpkg` source package: `automake-1.16=1:1.16.1-4ubuntu3`

Binary Packages:

- `automake=1:1.16.1-4ubuntu3`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.1-4ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.1-4ubuntu3.dsc' automake-1.16_1.16.1-4ubuntu3.dsc 2334 SHA256:1705b3f133b71906898771c9657a478473706402d07c10a681ae9ac9a67fef54
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.1.orig.tar.xz' automake-1.16_1.16.1.orig.tar.xz 1534936 SHA256:5d05bb38a23fd3312b10aea93840feec685bdf4a41146e78882848165d3ae921
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.1-4ubuntu3.debian.tar.xz' automake-1.16_1.16.1-4ubuntu3.debian.tar.xz 15060 SHA256:9d7edaf15badc1d071315d59a31a18ba195a3e1cc9a879c63a47a37a621a220f
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

### `dpkg` source package: `base-files=11ubuntu1`

Binary Packages:

- `base-files=11ubuntu1`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `base-passwd=3.5.46`

Binary Packages:

- `base-passwd=3.5.46`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-passwd/3.5.46/


### `dpkg` source package: `bash=5.0-5ubuntu1`

Binary Packages:

- `bash=5.0-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.0-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-5ubuntu1.dsc' bash_5.0-5ubuntu1.dsc 2447 SHA256:f819523a8bf9ea8048c0f6115d213a355e8bfac7caac66b9d4e57552b7b3b473
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA256:893858ba233d65bda38039e99dd96a4102b2f6a2d5e6c1c546e0794a60beed97
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-5ubuntu1.debian.tar.xz' bash_5.0-5ubuntu1.debian.tar.xz 71348 SHA256:83f318783c9a1b5014d3b9c2a0e8fc045fb01d2c675c4aeb1136c31538a15afe
```

### `dpkg` source package: `binutils=2.33.1-6ubuntu1`

Binary Packages:

- `binutils=2.33.1-6ubuntu1`
- `binutils-common:amd64=2.33.1-6ubuntu1`
- `binutils-x86-64-linux-gnu=2.33.1-6ubuntu1`
- `libbinutils:amd64=2.33.1-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `brotli=1.0.7-5`

Binary Packages:

- `libbrotli1:amd64=1.0.7-5`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.7-5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-5.dsc' brotli_1.0.7-5.dsc 2491 SHA256:25ff0a01848020e00ecff028df3ab25a5e651670932cc55cec2c93775d6f63da
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7.orig.tar.gz' brotli_1.0.7.orig.tar.gz 23827908 SHA256:4c61bfb0faca87219ea587326c467b95acb25555b53d1a421ffa3c8a9296ee2c
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-5.debian.tar.xz' brotli_1.0.7-5.debian.tar.xz 4456 SHA256:c1c2475f1acf0b15f75f870120d30c220d9af149cb44d2422f198cf6580648ae
```

### `dpkg` source package: `bzip2=1.0.8-2`

Binary Packages:

- `bzip2=1.0.8-2`
- `libbz2-1.0:amd64=1.0.8-2`
- `libbz2-dev:amd64=1.0.8-2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-2.dsc' bzip2_1.0.8-2.dsc 2180 SHA256:646cdcbb786a89a647cfafb280ef467143c06c445c4bf6fe69ec4a7882943064
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-2.debian.tar.bz2' bzip2_1.0.8-2.debian.tar.bz2 26032 SHA256:237c8619bc9bc16f357b1077064a3e58aa1a230dadb4b9bb3bd8dc8f454afc0b
```

### `dpkg` source package: `bzr=2.7.0+bzr6622-17ubuntu1`

Binary Packages:

- `bzr=2.7.0+bzr6622-17ubuntu1`
- `python-bzrlib=2.7.0+bzr6622-17ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`, `/usr/share/doc/python-bzrlib/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.7.0+bzr6622-17ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622-17ubuntu1.dsc' bzr_2.7.0+bzr6622-17ubuntu1.dsc 2921 SHA256:7829358bac6c2765241a85216334d8aceef4d51ace678bdaa07de8e4b1fa3583
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622.orig.tar.gz' bzr_2.7.0+bzr6622.orig.tar.gz 10948360 SHA256:08bba3e76cba9beb6b686e71253045beeab9db94753ddbcafa0f8ed1cba377ff
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622-17ubuntu1.debian.tar.xz' bzr_2.7.0+bzr6622-17ubuntu1.debian.tar.xz 71040 SHA256:4ea2afef7cbd263a30891480dece7b1368204b00548c39f4478c53c6a67a564e
```

### `dpkg` source package: `ca-certificates=20190110`

Binary Packages:

- `ca-certificates=20190110`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110.dsc' ca-certificates_20190110.dsc 1805 SHA256:bffbfe63a1ad2a07c6094502f05899c65edba93aefe58682f440e000fc65f6f0
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110.tar.xz' ca-certificates_20190110.tar.xz 243472 SHA256:ee4bf0f4c6398005f5b5ca4e0b87b82837ac5c3b0280a1cb3a63c47555c3a675
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

### `dpkg` source package: `cdebconf=0.250ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.250ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.250ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.250ubuntu1.dsc' cdebconf_0.250ubuntu1.dsc 2858 SHA256:bed77f0e55d2fa9212d108c6be741ff2e19e39e77ae9b3c5d3215b36fe9fed1a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.250ubuntu1.tar.xz' cdebconf_0.250ubuntu1.tar.xz 276512 SHA256:00dfbfc507ad5761de0a92580fe7838cce191e667460bfe5cc99cb430fef8626
```

### `dpkg` source package: `configobj=5.0.6-3`

Binary Packages:

- `python-configobj=5.0.6-3`

Licenses: (parsed from: `/usr/share/doc/python-configobj/copyright`)

- `BSD-3-clause`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/configobj/5.0.6-3/


### `dpkg` source package: `coreutils=8.30-3ubuntu2`

Binary Packages:

- `coreutils=8.30-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.30-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.30-3ubuntu2.dsc' coreutils_8.30-3ubuntu2.dsc 2048 SHA256:f36fe0ac14978b240a750b79d2bbd737d6b1939296c3a287899933aa2a1906ea
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.30.orig.tar.xz' coreutils_8.30.orig.tar.xz 5359532 SHA256:e831b3a86091496cdba720411f9748de81507798f6130adeaef872d206e1b057
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.30-3ubuntu2.debian.tar.xz' coreutils_8.30-3ubuntu2.debian.tar.xz 39636 SHA256:98204ef9d94e5c567880cd0245fdb7940eaf7592d6c6830c300ad117628b351f
```

### `dpkg` source package: `curl=7.66.0-1ubuntu1`

Binary Packages:

- `curl=7.66.0-1ubuntu1`
- `libcurl3-gnutls:amd64=7.66.0-1ubuntu1`
- `libcurl4:amd64=7.66.0-1ubuntu1`
- `libcurl4-openssl-dev:amd64=7.66.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.66.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.66.0-1ubuntu1.dsc' curl_7.66.0-1ubuntu1.dsc 2761 SHA256:5beec04120a0ee227345d8bfe5f35ba8b12c42207d20682114e4711ee796c866
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.66.0.orig.tar.gz' curl_7.66.0.orig.tar.gz 4066716 SHA256:d0393da38ac74ffac67313072d7fe75b1fa1010eb5987f63f349b024a36b7ffb
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.66.0-1ubuntu1.debian.tar.xz' curl_7.66.0-1ubuntu1.debian.tar.xz 29980 SHA256:39dbe250a139986dfa09ec46fd05daec746927cae74bfbc59f439f0e9d0874cc
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-1build3`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-1build3`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-1build3`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `dash=0.5.10.2-6`

Binary Packages:

- `dash=0.5.10.2-6`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.10.2-6
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-6.dsc' dash_0.5.10.2-6.dsc 1756 SHA256:d509a23ebdc4f107c911914590c1400e5a24383f35c5d6904e48d2afeff168ac
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA256:3c663919dc5c66ec991da14c7cf7e0be8ad00f3db73986a987c118862b5f6071
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-6.debian.tar.xz' dash_0.5.10.2-6.debian.tar.xz 44232 SHA256:1448fbfc2541be52787da81ce03bb81ad6b1f380cba1b7e747abefdcd44f6c86
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

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6ubuntu1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6ubuntu1`
- `libdb5.3-dev=5.3.28+dfsg1-0.6ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu1.dsc' db5.3_5.3.28+dfsg1-0.6ubuntu1.dsc 3220 SHA256:9374bf67244c85ea18442d804d4055b12493d73692f35e05c54d2f77ce979df1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu1.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6ubuntu1.debian.tar.xz 30108 SHA256:d22388b6e2b7e588b1ee16816878bd67c4edb79efb8ea47daf4edfb79605f26f
```

### `dpkg` source package: `debconf=1.5.73`

Binary Packages:

- `debconf=1.5.73`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.73
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.73.dsc' debconf_1.5.73.dsc 2081 SHA256:cdd4c049414cd167a4a9479d883e205bf5cebb19fc4bb6f132000a56291eb670
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.73.tar.xz' debconf_1.5.73.tar.xz 570780 SHA256:513895b2b77d9fb72542152390e7d4c67fe1e08de75fdad44d54ce1e7d83ecef
```

### `dpkg` source package: `debianutils=4.9`

Binary Packages:

- `debianutils=4.9`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debianutils/4.9/


### `dpkg` source package: `diffutils=1:3.7-3`

Binary Packages:

- `diffutils=1:3.7-3`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.7-3
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3.dsc' diffutils_3.7-3.dsc 1453 SHA256:99dee94cec05454a65a9cb542bea1720dbd4c511d13f9784c9e3741e76a9b9ba
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz' diffutils_3.7.orig.tar.xz 1448828 SHA256:b3a7a6221c3dc916085f0d205abf6b8e1ba443d4dd965118da364a1dc1cb3a26
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3.debian.tar.xz' diffutils_3.7-3.debian.tar.xz 11116 SHA256:a455228f12283b5f3c0165db4ab9b12071adc37fb9dd50dcb5e1b8851c524f1f
```

### `dpkg` source package: `djvulibre=3.5.27.1-14`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.27.1-14`
- `libdjvulibre-text=3.5.27.1-14`
- `libdjvulibre21:amd64=3.5.27.1-14`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-14
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-14.dsc' djvulibre_3.5.27.1-14.dsc 2406 SHA256:ccb6659a2bbf2ac63223f8dc91b2d59f40ff77c2c25dbb7f6b531c4b2d46bc08
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA256:77f07de3f1039aa19eba2eb3170d9ce9a0918ba7b704a59cfaf08f42fcc52144
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-14.debian.tar.xz' djvulibre_3.5.27.1-14.debian.tar.xz 76272 SHA256:72f7680b069de1e51b15098fd6711e15205c62ab388ae5b66afdb29e8cb02300
```

### `dpkg` source package: `dpkg=1.19.7ubuntu2`

Binary Packages:

- `dpkg=1.19.7ubuntu2`
- `dpkg-dev=1.19.7ubuntu2`
- `libdpkg-perl=1.19.7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.7ubuntu2.dsc' dpkg_1.19.7ubuntu2.dsc 2262 SHA256:579516f6ebccc399f7bc1b1ed49c298ecdea0511e4c3ad68f083486bb1abd3cb
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.7ubuntu2.tar.xz' dpkg_1.19.7ubuntu2.tar.xz 4730708 SHA256:972f148f1404b3382002d919c35fabfdfa74161492882a8f8af33e7f534af977
```

### `dpkg` source package: `e2fsprogs=1.45.3-4ubuntu2`

Binary Packages:

- `comerr-dev:amd64=2.1-1.45.3-4ubuntu2`
- `e2fsprogs=1.45.3-4ubuntu2`
- `libcom-err2:amd64=1.45.3-4ubuntu2`
- `libext2fs2:amd64=1.45.3-4ubuntu2`
- `libss2:amd64=1.45.3-4ubuntu2`
- `logsave=1.45.3-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.3-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.3-4ubuntu2.dsc' e2fsprogs_1.45.3-4ubuntu2.dsc 3259 SHA256:0eaed7cc5000be5333685939814db3c2bef191be6dec2846cb2c25d1e2029891
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.3.orig.tar.gz' e2fsprogs_1.45.3.orig.tar.gz 7926121 SHA256:3a5556e0cb746c214e4c581951a3c21ba5c145eb53008277f88f1f98ae75983d
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.3.orig.tar.gz.asc' e2fsprogs_1.45.3.orig.tar.gz.asc 488 SHA256:013c21c98dc63a6a6328490a335a1bc6f3a2410f4f6347312bf6b53734faa759
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.3-4ubuntu2.debian.tar.xz' e2fsprogs_1.45.3-4ubuntu2.debian.tar.xz 188120 SHA256:00324578dc4afaf860c1aab9beddc9c6b12a3b1e143b6df6fd5756fc7a782bcd
```

### `dpkg` source package: `elfutils=0.176-1.1`

Binary Packages:

- `libelf1:amd64=0.176-1.1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.176-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.176-1.1.dsc' elfutils_0.176-1.1.dsc 2584 SHA256:6d9fa4741e921f58a3e291def1f92a87bed888db15e73d6e29d46fc48b5f615a
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.176.orig.tar.bz2' elfutils_0.176.orig.tar.bz2 8646075 SHA256:eb5747c371b0af0f71e86215a5ebb88728533c3a104a43d4231963f308cd1023
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.176.orig.tar.bz2.asc' elfutils_0.176.orig.tar.bz2.asc 455 SHA256:51474b579b25fc799de0777e241c83605427d2903f8d28524ef6af42f75931fd
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.176-1.1.debian.tar.xz' elfutils_0.176-1.1.debian.tar.xz 31644 SHA256:06d7057e744d3a6138cf43d30237e2b327b6bfe3041a9a4b210414429c1267f1
```

### `dpkg` source package: `expat=2.2.9-1`

Binary Packages:

- `libexpat1:amd64=2.2.9-1`
- `libexpat1-dev:amd64=2.2.9-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1.dsc' expat_2.2.9-1.dsc 1949 SHA256:58db7b5ac8431570f47921ff545493334d09070a9afab9aaf8282e3c1dfc66ad
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9.orig.tar.gz' expat_2.2.9.orig.tar.gz 8273174 SHA256:c341ac8c79e021cc3392a6d76e138e62d1dd287592cb455148540331756a2208
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1.debian.tar.xz' expat_2.2.9-1.debian.tar.xz 10740 SHA256:85d13af9777815b77a478044604902d9a04eb05f4f0dbcaedcbe1193670239d4
```

### `dpkg` source package: `fftw3=3.3.8-2ubuntu1`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu1.dsc' fftw3_3.3.8-2ubuntu1.dsc 2240 SHA256:f33b0cba612104281fa3de2cdd38e8cedf8aa52a6e28146d9b162a2df11aff8e
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA256:6113262f6e92c5bd474f2875fa1b01054c4ad5040f6b0da7c03c98821d9ae303
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu1.debian.tar.xz' fftw3_3.3.8-2ubuntu1.debian.tar.xz 14028 SHA256:8bc469ad07cef4ebb1c512feecc061ba58eb851d83f67f732d42bc7db0a4f89b
```

### `dpkg` source package: `file=1:5.37-6`

Binary Packages:

- `file=1:5.37-6`
- `libmagic-mgc=1:5.37-6`
- `libmagic1:amd64=1:5.37-6`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.37-6
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37-6.dsc' file_5.37-6.dsc 2214 SHA256:9e549c158d657c6345f5a33d4c151a7c4a383953c2ea9c74171e10b942dddd69
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37.orig.tar.gz' file_5.37.orig.tar.gz 887682 SHA256:e9c13967f7dd339a3c241b7710ba093560b9a33013491318e88e6b8b57bae07f
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37.orig.tar.gz.asc' file_5.37.orig.tar.gz.asc 169 SHA256:f73642d84908665dad226f247ae223e6bf52da8b2ca20ca88bd4e4966eef6bc7
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37-6.debian.tar.xz' file_5.37-6.debian.tar.xz 37648 SHA256:a20a1af3ece8b33c6da832d1dd04e3ff8b79a7d4833311b335b3f2c6fa09bd5a
```

### `dpkg` source package: `findutils=4.6.0+git+20190209-2ubuntu1`

Binary Packages:

- `findutils=4.6.0+git+20190209-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20190209-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20190209-2ubuntu1.dsc' findutils_4.6.0+git+20190209-2ubuntu1.dsc 2244 SHA256:27c67aa55d3c1adb7793156f06859799e235968fcd710c4dbfd4f3f0e644f811
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20190209.orig.tar.xz' findutils_4.6.0+git+20190209.orig.tar.xz 1893084 SHA256:6832b3f6ddc0e2718795e6732ea40cc5309b948505f55fb9935919d6aaac7e9d
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20190209-2ubuntu1.debian.tar.xz' findutils_4.6.0+git+20190209-2ubuntu1.debian.tar.xz 26800 SHA256:75c9b4c324d8b43cd71081987df83145ad915e6929bfeb992df81b165fba123c
```

### `dpkg` source package: `fontconfig=2.13.1-2ubuntu2`

Binary Packages:

- `fontconfig=2.13.1-2ubuntu2`
- `fontconfig-config=2.13.1-2ubuntu2`
- `libfontconfig1:amd64=2.13.1-2ubuntu2`
- `libfontconfig1-dev:amd64=2.13.1-2ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-2ubuntu2.dsc' fontconfig_2.13.1-2ubuntu2.dsc 1959 SHA256:d467a0a70276839f7b608d8ee64d2379e251676b32ac547ef60298faa9861ba3
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA256:f655dd2a986d7aa97e052261b36aa67b0a64989496361eca8d604e6414006741
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-2ubuntu2.debian.tar.xz' fontconfig_2.13.1-2ubuntu2.debian.tar.xz 26232 SHA256:027f1e464d5e79636c61d1cff0b183188dc037066b84af651ae175f4073d2d5f
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.dsc' fonts-dejavu_2.37-1.dsc 2575 SHA256:f35ff7b2c8dbfda6564c9dedf088ba06cc6d279fdd8e7cccbd1ae08ded1bb71c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.debian.tar.xz' fonts-dejavu_2.37-1.debian.tar.xz 10424 SHA256:5105cdbfc086f4a83ab6871eb39cc904bf02aa52762402b7cacf33d0938122f7
```

### `dpkg` source package: `freetype=2.10.1-2`

Binary Packages:

- `libfreetype-dev:amd64=2.10.1-2`
- `libfreetype6:amd64=2.10.1-2`
- `libfreetype6-dev:amd64=2.10.1-2`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `FSFUL`
- `FSFULLR`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `MPL-1.1`
- `OFL-1.1`
- `OpenGroup-BSD-like`
- `Permissive`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.10.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1-2.dsc' freetype_2.10.1-2.dsc 3749 SHA256:3515097c45d05c7f82f8636a7fa65c12ed70868affbc270fe6788bf61b5d4cd8
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1.orig-ft2demos.tar.gz' freetype_2.10.1.orig-ft2demos.tar.gz 305328 SHA256:5e9e94a2db9d1a945293a1644a502f6664a2173a454d4a55b19695e2e2f4a0bc
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1.orig-ft2demos.tar.gz.asc' freetype_2.10.1.orig-ft2demos.tar.gz.asc 195 SHA256:ccee51c4b4101b89a66ba5f2bdd54d127e93e120086982db57fa33761f310e9e
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1.orig-ft2docs.tar.gz' freetype_2.10.1.orig-ft2docs.tar.gz 2123885 SHA256:a4e4a8e69c7bf833eba7c158254a572fd43131d5e9b8791bd2ecbb03546ce155
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1.orig-ft2docs.tar.gz.asc' freetype_2.10.1.orig-ft2docs.tar.gz.asc 195 SHA256:aaedd84036d9e615fbb5acf71081dd05c9d7333686593432e445ee89655a79c9
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1.orig.tar.gz' freetype_2.10.1.orig.tar.gz 3478158 SHA256:3a60d391fd579440561bf0e7f31af2222bc610ad6ce4d9d7bd2165bca8669110
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1.orig.tar.gz.asc' freetype_2.10.1.orig.tar.gz.asc 195 SHA256:3952cc2651536ef5157601143d1efc453a7fe5ca64eaf765d034c417aabd4210
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.1-2.debian.tar.xz' freetype_2.10.1-2.debian.tar.xz 114884 SHA256:3d1405fe90e17ee290e06f4fd65a16ff38d9f9604aff12c40a0574edb3dbbe62
```

### `dpkg` source package: `fribidi=1.0.7-1.1`

Binary Packages:

- `libfribidi0:amd64=1.0.7-1.1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.7-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.7-1.1.dsc' fribidi_1.0.7-1.1.dsc 2444 SHA256:716cfa7b98103104c2dec36d90427d91185a7dfb96cf7ae0854713a830e5da87
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.7.orig.tar.bz2' fribidi_1.0.7.orig.tar.bz2 2074943 SHA256:5ab5f21e9f2fc57b4b40f8ea8f14dba78a5cc46d9cf94bc5e00a58e6886a935d
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.7-1.1.debian.tar.xz' fribidi_1.0.7-1.1.debian.tar.xz 8908 SHA256:bef9430be691d1790754431c7fe2f0b33235e406fce3956c9a67e1c1268390ef
```

### `dpkg` source package: `gcc-9=9.2.1-21ubuntu1`

Binary Packages:

- `cpp-9=9.2.1-21ubuntu1`
- `g++-9=9.2.1-21ubuntu1`
- `gcc-9=9.2.1-21ubuntu1`
- `gcc-9-base:amd64=9.2.1-21ubuntu1`
- `libasan5:amd64=9.2.1-21ubuntu1`
- `libatomic1:amd64=9.2.1-21ubuntu1`
- `libcc1-0:amd64=9.2.1-21ubuntu1`
- `libgcc-9-dev:amd64=9.2.1-21ubuntu1`
- `libgcc1:amd64=1:9.2.1-21ubuntu1`
- `libgomp1:amd64=9.2.1-21ubuntu1`
- `libitm1:amd64=9.2.1-21ubuntu1`
- `liblsan0:amd64=9.2.1-21ubuntu1`
- `libquadmath0:amd64=9.2.1-21ubuntu1`
- `libstdc++-9-dev:amd64=9.2.1-21ubuntu1`
- `libstdc++6:amd64=9.2.1-21ubuntu1`
- `libtsan0:amd64=9.2.1-21ubuntu1`
- `libubsan1:amd64=9.2.1-21ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp-9/copyright`, `/usr/share/doc/g++-9/copyright`, `/usr/share/doc/gcc-9/copyright`, `/usr/share/doc/gcc-9-base/copyright`, `/usr/share/doc/libasan5/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-9-dev/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-9-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gcc-9=9.2.1-21ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.2.1-21ubuntu1.dsc' gcc-9_9.2.1-21ubuntu1.dsc 29805 SHA256:45105a81c792910ffea693969280dcfccc97b53c9cef41b778f8ad5aacfa6a20
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.2.1.orig.tar.gz' gcc-9_9.2.1.orig.tar.gz 90195906 SHA256:8819e4bbae43592726be676262f81f242bc5b7a50a019012d8ef02d135a1280c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.2.1-21ubuntu1.debian.tar.xz' gcc-9_9.2.1-21ubuntu1.debian.tar.xz 879416 SHA256:f7d6484b82e3f0d10e55e1b131ea67ec4451fdc34d4f9d5d4284d5b5c1872308
```

### `dpkg` source package: `gcc-defaults=1.185.1ubuntu1`

Binary Packages:

- `cpp=4:9.2.1-3.1ubuntu1`
- `g++=4:9.2.1-3.1ubuntu1`
- `gcc=4:9.2.1-3.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.185.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.185.1ubuntu1.dsc' gcc-defaults_1.185.1ubuntu1.dsc 16544 SHA256:236740a44cad4b9f743c5ac74489f20efdee3a8ec32f85f7256c8afe11e77671
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.185.1ubuntu1.tar.gz' gcc-defaults_1.185.1ubuntu1.tar.gz 58720 SHA256:f0a7546463ac7be2487a0b626c6e86e59d13ab46c6297e9c60678bfd98e09308
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

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.18.1-5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.dsc' gdbm_1.18.1-5.dsc 2635 SHA256:4c0c4498378c673c9d2d8dfb5b319a4830d2dd21e65faaaa8e0f09cb7f71606b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz' gdbm_1.18.1.orig.tar.gz 941863 SHA256:86e613527e5dba544e73208f42b78b7c022d4fa5a6d5498bf18c8d6f745b91dc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz.asc' gdbm_1.18.1.orig.tar.gz.asc 412 SHA256:3254738e7689e44ac65e78a766806828b8282e6bb1c0e5bb6156a99e567889a5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.debian.tar.xz' gdbm_1.18.1-5.debian.tar.xz 16348 SHA256:3c1a0e05b40a97ee51ce77c736c72c37738ba31b2720111d3bc99175a2c3a3ed
```

### `dpkg` source package: `gdk-pixbuf=2.40.0+dfsg-1ubuntu1`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.40.0+dfsg-1ubuntu1`
- `libgdk-pixbuf2.0-0:amd64=2.40.0+dfsg-1ubuntu1`
- `libgdk-pixbuf2.0-bin=2.40.0+dfsg-1ubuntu1`
- `libgdk-pixbuf2.0-common=2.40.0+dfsg-1ubuntu1`
- `libgdk-pixbuf2.0-dev:amd64=2.40.0+dfsg-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `git=1:2.24.0-1ubuntu1`

Binary Packages:

- `git=1:2.24.0-1ubuntu1`
- `git-man=1:2.24.0-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.24.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.24.0-1ubuntu1.dsc' git_2.24.0-1ubuntu1.dsc 2969 SHA256:6f451c542d8325236b27c12a258b9c71883b161f5cbfc937c367c0c661b1b9d8
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.24.0.orig.tar.xz' git_2.24.0.orig.tar.xz 5766056 SHA256:9f71d61973626d8b28c4cdf8e2484b4bf13870ed643fed982d68b2cfd754371b
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.24.0-1ubuntu1.debian.tar.xz' git_2.24.0-1ubuntu1.debian.tar.xz 629624 SHA256:76a10c89f966e336a5328553515db590675123256acb7e3cd050068e3829e43f
```

### `dpkg` source package: `glib2.0=2.63.1-2ubuntu1`

Binary Packages:

- `libglib2.0-0:amd64=2.63.1-2ubuntu1`
- `libglib2.0-bin=2.63.1-2ubuntu1`
- `libglib2.0-data=2.63.1-2ubuntu1`
- `libglib2.0-dev:amd64=2.63.1-2ubuntu1`
- `libglib2.0-dev-bin=2.63.1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `glibc=2.30-0ubuntu2`

Binary Packages:

- `libc-bin=2.30-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`)

- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `glibc=2.30-0ubuntu3`

Binary Packages:

- `libc-dev-bin=2.30-0ubuntu3`
- `libc6:amd64=2.30-0ubuntu3`
- `libc6-dev:amd64=2.30-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.30-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.30-0ubuntu3.dsc' glibc_2.30-0ubuntu3.dsc 9228 SHA256:0d63090ad8836a71237cf7ce69e8fe369aeed7d2e20537e5149ba1555d80892e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.30.orig.tar.xz' glibc_2.30.orig.tar.xz 17080288 SHA256:88b5b39b80a4cb4d7b17bded91a2a9e99ff00190377321446f55d00a97611870
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.30-0ubuntu3.debian.tar.xz' glibc_2.30-0ubuntu3.debian.tar.xz 850808 SHA256:fb17aa2731b83b1468dd7e2b0fb0dce06f127b53557eee60011cdf3c561a9a85
```

### `dpkg` source package: `gmp=2:6.1.2+dfsg-4`

Binary Packages:

- `libgmp-dev:amd64=2:6.1.2+dfsg-4`
- `libgmp10:amd64=2:6.1.2+dfsg-4`
- `libgmpxx4ldbl:amd64=2:6.1.2+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-4.dsc' gmp_6.1.2+dfsg-4.dsc 2123 SHA256:5e9c98e1636344bf0c84710ee564ee6032d6a9db26aa5d29857d65b2a979877c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-4.debian.tar.xz' gmp_6.1.2+dfsg-4.debian.tar.xz 21416 SHA256:cb25b080d915d9e5a641920f0471b4deb5368af739c7675d887cf290c2cffbe2
```

### `dpkg` source package: `gnupg2=2.2.17-3ubuntu1`

Binary Packages:

- `dirmngr=2.2.17-3ubuntu1`
- `gnupg=2.2.17-3ubuntu1`
- `gnupg-l10n=2.2.17-3ubuntu1`
- `gnupg-utils=2.2.17-3ubuntu1`
- `gpg=2.2.17-3ubuntu1`
- `gpg-agent=2.2.17-3ubuntu1`
- `gpg-wks-client=2.2.17-3ubuntu1`
- `gpg-wks-server=2.2.17-3ubuntu1`
- `gpgconf=2.2.17-3ubuntu1`
- `gpgsm=2.2.17-3ubuntu1`
- `gpgv=2.2.17-3ubuntu1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.17-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.17-3ubuntu1.dsc' gnupg2_2.2.17-3ubuntu1.dsc 3945 SHA256:2b986fd198f0873279071a9fb074549f5b0a4ba4e44ceebabe546b39d175e49f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.17.orig.tar.bz2' gnupg2_2.2.17.orig.tar.bz2 6717554 SHA256:afa262868e39b651a2db4c071fba90415154243e83a830ca00516f9a807fd514
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.17.orig.tar.bz2.asc' gnupg2_2.2.17.orig.tar.bz2.asc 488 SHA256:b719d78c3b3d91ae6c5569c6ce48b8b71cfd9ac53cc95c681ea196720b9d7000
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.17-3ubuntu1.debian.tar.xz' gnupg2_2.2.17-3ubuntu1.debian.tar.xz 66684 SHA256:a6d07fb9d1c8cecff84d9b68a7dc282b6da685fc1c76ed81a7d1ed661a4b0ba7
```

### `dpkg` source package: `gnutls28=3.6.10-5`

Binary Packages:

- `libgnutls30:amd64=3.6.10-5`

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
- `LGPLv3+_or_GPLv2+`
- `The main library is licensed under GNU Lesser`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gnutls28/3.6.10-5/


### `dpkg` source package: `gobject-introspection=1.62.0-2`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.62.0-2`
- `gir1.2-glib-2.0:amd64=1.62.0-2`
- `libgirepository-1.0-1:amd64=1.62.0-2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.62.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.62.0-2.dsc' gobject-introspection_1.62.0-2.dsc 2898 SHA256:e0e2a55bbcbd084a1280c8ea55632257fea20ab9d620eb51ef75f951117a9a18
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.62.0.orig.tar.xz' gobject-introspection_1.62.0.orig.tar.xz 980732 SHA256:b1ee7ed257fdbc008702bdff0ff3e78a660e7e602efa8f211dc89b9d1e7d90a2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.62.0-2.debian.tar.xz' gobject-introspection_1.62.0-2.debian.tar.xz 21708 SHA256:c0e0c4c04510e906749289404464beac8faddfa1ea2692ac7c39e7d0d97b5f44
```

### `dpkg` source package: `graphite2=1.3.13-11`

Binary Packages:

- `libgraphite2-3:amd64=1.3.13-11`

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
$ apt-get source -qq --print-uris graphite2=1.3.13-11
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.13-11.dsc' graphite2_1.3.13-11.dsc 2587 SHA256:cfd46b34cf1a33e2c54be2815c17573b68fe567362b4fdb4f19f841271302691
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.13.orig.tar.gz' graphite2_1.3.13.orig.tar.gz 6664941 SHA256:2f9f609deeddfe2b193502adc8df3b0396694b799a433c36e85fd1242e654cd9
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.13-11.debian.tar.xz' graphite2_1.3.13-11.debian.tar.xz 12068 SHA256:ecac95e52d550a271ec5c506489c82c1561301c641df3caf0048ea0d572abc11
```

### `dpkg` source package: `grep=3.3-1build1`

Binary Packages:

- `grep=3.3-1build1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.3-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.3-1build1.dsc' grep_3.3-1build1.dsc 2071 SHA256:06d804485087fb2a22da76190b60dc800971dc8e6b6c8f3088fdce41bd8469c3
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.3.orig.tar.xz' grep_3.3.orig.tar.xz 1473056 SHA256:b960541c499619efd6afe1fa795402e4733c8e11ebf9fafccc0bb4bccdc5b514
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.3-1build1.debian.tar.xz' grep_3.3-1build1.debian.tar.xz 104360 SHA256:a08e6e88ada40dc5e0195dfea04f4c8aea9e2b57a3272185fedc85a2ad575d23
```

### `dpkg` source package: `gzip=1.10-0ubuntu3`

Binary Packages:

- `gzip=1.10-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `harfbuzz=2.6.4-1ubuntu1`

Binary Packages:

- `libharfbuzz0b:amd64=2.6.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.6.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4-1ubuntu1.dsc' harfbuzz_2.6.4-1ubuntu1.dsc 2878 SHA256:b827934b81f1115eaffd848ee19e7e9dc5f958d843d7e9b56c11f6334db9ce46
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4.orig.tar.xz' harfbuzz_2.6.4.orig.tar.xz 5967468 SHA256:9413b8d96132d699687ef914ebb8c50440efc87b3f775d25856d7ec347c03c12
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4-1ubuntu1.debian.tar.xz' harfbuzz_2.6.4-1ubuntu1.debian.tar.xz 11152 SHA256:1ab2ebdb4a41858c9a461fb8be6553d3981af3ebd40a29888fb173d40f5f99ce
```

### `dpkg` source package: `heimdal=7.5.0+dfsg-3build1`

Binary Packages:

- `libasn1-8-heimdal:amd64=7.5.0+dfsg-3build1`
- `libgssapi3-heimdal:amd64=7.5.0+dfsg-3build1`
- `libhcrypto4-heimdal:amd64=7.5.0+dfsg-3build1`
- `libheimbase1-heimdal:amd64=7.5.0+dfsg-3build1`
- `libheimntlm0-heimdal:amd64=7.5.0+dfsg-3build1`
- `libhx509-5-heimdal:amd64=7.5.0+dfsg-3build1`
- `libkrb5-26-heimdal:amd64=7.5.0+dfsg-3build1`
- `libroken18-heimdal:amd64=7.5.0+dfsg-3build1`
- `libwind0-heimdal:amd64=7.5.0+dfsg-3build1`

Licenses: (parsed from: `/usr/share/doc/libasn1-8-heimdal/copyright`, `/usr/share/doc/libgssapi3-heimdal/copyright`, `/usr/share/doc/libhcrypto4-heimdal/copyright`, `/usr/share/doc/libheimbase1-heimdal/copyright`, `/usr/share/doc/libheimntlm0-heimdal/copyright`, `/usr/share/doc/libhx509-5-heimdal/copyright`, `/usr/share/doc/libkrb5-26-heimdal/copyright`, `/usr/share/doc/libroken18-heimdal/copyright`, `/usr/share/doc/libwind0-heimdal/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `custom`
- `none`

Source:

```console
$ apt-get source -qq --print-uris heimdal=7.5.0+dfsg-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-3build1.dsc' heimdal_7.5.0+dfsg-3build1.dsc 3628 SHA256:7e971aad47d4518dc4d487c5d9508c3711949509e540d2a84fd8ede16530e67f
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg.orig.tar.gz' heimdal_7.5.0+dfsg.orig.tar.gz 8955005 SHA256:489119b7a1a900b88163765654dc59cba9a321b078fafc76629e2b85ef140867
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-3build1.debian.tar.xz' heimdal_7.5.0+dfsg-3build1.debian.tar.xz 461560 SHA256:f5e7d09ab71cdc18ce2776bc1c047681d6daacdc55cb637cb9520bc11f528324
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

### `dpkg` source package: `icu=63.2-2`

Binary Packages:

- `icu-devtools=63.2-2`
- `libicu-dev:amd64=63.2-2`
- `libicu63:amd64=63.2-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=63.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_63.2-2.dsc' icu_63.2-2.dsc 1965 SHA256:b11e7fb65cce3bf22e7549c8291a5e058171a8eaf9e37ca8c30b45971e4ad97f
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_63.2.orig.tar.xz' icu_63.2.orig.tar.xz 13630108 SHA256:ab79c7bf11eacc0e3368b29ebba5cff67f41860a522f6a3957377353d5bc8d71
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_63.2-2.debian.tar.xz' icu_63.2-2.debian.tar.xz 34300 SHA256:2a9fb8ab29527e985b24dc7b15dd116be0b4a2edd9f106dca77c6f75b9baab7d
```

### `dpkg` source package: `ilmbase=2.3.0-6`

Binary Packages:

- `libilmbase-dev:amd64=2.3.0-6`
- `libilmbase24:amd64=2.3.0-6`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase24/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.3.0-6
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0-6.dsc' ilmbase_2.3.0-6.dsc 2473 SHA256:1651b6968fdca9a273be866b7ab6aa887f6b916ab48f160bae5a79d83f87fe58
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0.orig.tar.gz' ilmbase_2.3.0.orig.tar.gz 596749 SHA256:0ea21166799bbdd920e7a38a7026236566aafdd6e8638f54c9da1af2219fae82
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0.orig.tar.gz.asc' ilmbase_2.3.0.orig.tar.gz.asc 566 SHA256:c7ee3f4432322d4f7c63dd1b0ca2188a8d1c4a018821c3c12a3d9db746b54bee
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.3.0-6.debian.tar.xz' ilmbase_2.3.0-6.debian.tar.xz 14184 SHA256:58c947fd6ff46a5a71564f70fd69f2df19bd139c428c8019c4f8a088c50358f1
```

### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu10`

Binary Packages:

- `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu10`
- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1ubuntu10`
- `imagemagick-6.q16=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickcore-6-arch-config:amd64=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickcore-6-headers=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickcore-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickcore-dev=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickwand-6-headers=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickwand-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu10`
- `libmagickwand-dev=8:6.9.10.23+dfsg-2.1ubuntu10`

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.10.23+dfsg-2.1ubuntu10
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1ubuntu10.dsc' imagemagick_6.9.10.23+dfsg-2.1ubuntu10.dsc 4490 SHA256:7ddfc9cf7a4dc622af0a663d13017f829ec0e57bc899df6d6021ce5e355157a5
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.10.23+dfsg.orig.tar.xz' imagemagick_6.9.10.23+dfsg.orig.tar.xz 9081188 SHA256:44249112b624f2cc315573fa96685e547da27ebb321432259290c407023c531e
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1ubuntu10.debian.tar.xz' imagemagick_6.9.10.23+dfsg-2.1ubuntu10.debian.tar.xz 242628 SHA256:85a4c6f00a82399fc2b0a06b82ba7d974314dfdf1d5a18e1a14ebd152ed9d234
```

### `dpkg` source package: `init-system-helpers=1.57`

Binary Packages:

- `init-system-helpers=1.57`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.57
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.57.dsc' init-system-helpers_1.57.dsc 1896 SHA256:88bb5af040c99f010b6d6947ff5c80ae4863ff787e0eeae91e99dcd15a10dbb8
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.57.tar.xz' init-system-helpers_1.57.tar.xz 40460 SHA256:e9d83fd8756a42666fb5d19a8835813823295846659b4e58f138bb9b54e9f5dd
```

### `dpkg` source package: `isl=0.22-2`

Binary Packages:

- `libisl22:amd64=0.22-2`

Licenses: (parsed from: `/usr/share/doc/libisl22/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.22-2
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22-2.dsc' isl_0.22-2.dsc 1846 SHA256:c203abb2d44658dc3f5cfa2dc9d7bc301f4ac8ec1c8cb791e781c5e675d14f18
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.orig.tar.xz' isl_0.22.orig.tar.xz 1676992 SHA256:6c8bc56c477affecba9c59e2c9f026967ac8bad01b51bdd07916db40a517b9fa
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22-2.debian.tar.xz' isl_0.22-2.debian.tar.xz 25228 SHA256:547c8c8c452a31247be532fcfe65efee98ef9c8351a35662308e6ec385c6a7c9
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

### `dpkg` source package: `keyutils=1.6-6ubuntu1`

Binary Packages:

- `libkeyutils1:amd64=1.6-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6-6ubuntu1.dsc' keyutils_1.6-6ubuntu1.dsc 2148 SHA256:76dfe0a0d9bb0a417d9c20c2f20b0beb9097dccd30c30a41375ef99cf0a710b6
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.orig.tar.bz2' keyutils_1.6.orig.tar.bz2 93973 SHA256:d3aef20cec0005c0fa6b4be40079885567473185b1a57b629b030e67942c7115
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6-6ubuntu1.debian.tar.xz' keyutils_1.6-6ubuntu1.debian.tar.xz 13636 SHA256:a4ae24062e9d20a0e2092e4cb342b664c0211ba7efdfeb7bde5f8d209c9ad1db
```

### `dpkg` source package: `krb5=1.17-6`

Binary Packages:

- `krb5-multidev:amd64=1.17-6`
- `libgssapi-krb5-2:amd64=1.17-6`
- `libgssrpc4:amd64=1.17-6`
- `libk5crypto3:amd64=1.17-6`
- `libkadm5clnt-mit11:amd64=1.17-6`
- `libkadm5srv-mit11:amd64=1.17-6`
- `libkdb5-9:amd64=1.17-6`
- `libkrb5-3:amd64=1.17-6`
- `libkrb5-dev:amd64=1.17-6`
- `libkrb5support0:amd64=1.17-6`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit11/copyright`, `/usr/share/doc/libkadm5srv-mit11/copyright`, `/usr/share/doc/libkdb5-9/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-6
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-6.dsc' krb5_1.17-6.dsc 3173 SHA256:413a7eea29e609ebcb622308da9e2dd98a3a73861f5ee52b121c2f32ee9d2abf
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA256:5a6e2284a53de5702d3dc2be3b9339c963f9b5397d3fbbc53beb249380a781f5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-6.debian.tar.xz' krb5_1.17-6.debian.tar.xz 143328 SHA256:0419148ef3a7908dad511eca3d9127b318ac1b697a67f719e19a1ff380c00086
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

### `dpkg` source package: `libassuan=2.5.3-7ubuntu1`

Binary Packages:

- `libassuan0:amd64=2.5.3-7ubuntu1`

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
$ apt-get source -qq --print-uris libassuan=2.5.3-7ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7ubuntu1.dsc' libassuan_2.5.3-7ubuntu1.dsc 2647 SHA256:b159f5926df8f52f35f8bf16d83f9354eaad63e7c6226b644f3b14d41b97102e
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA256:91bcb0403866b4e7c4bc1cc52ed4c364a9b5414b3994f718c70303f7f765e702
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA256:53b16a6619a2690b4f22da645a1d0c14b5664825c87b165ca5bd0de32607888a
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7ubuntu1.debian.tar.xz' libassuan_2.5.3-7ubuntu1.debian.tar.xz 13872 SHA256:14eb3b76531cbe438fcc8029bb16e9d981a2539c8f299e9eb334ac2cc532184e
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

### `dpkg` source package: `libcap-ng=0.7.9-2.1`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.1.dsc' libcap-ng_0.7.9-2.1.dsc 2109 SHA256:eb2c6bc4c96d0b80a3b36963c94763a1675567c38248a3313492b1e5414427d0
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.1.debian.tar.xz' libcap-ng_0.7.9-2.1.debian.tar.xz 6204 SHA256:529f686a5af51b999ad96ee3166445ffcb9c221af10f36e5c7fd7f3bf61154d5
```

### `dpkg` source package: `libcroco=0.6.13-1`

Binary Packages:

- `libcroco3:amd64=0.6.13-1`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.13-1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.13-1.dsc' libcroco_0.6.13-1.dsc 2216 SHA256:1f9a861643c65b432221f779ad9a6a0a1585724efbb01a10dfe22f69e3fbc18c
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.13.orig.tar.xz' libcroco_0.6.13.orig.tar.xz 487840 SHA256:767ec234ae7aa684695b3a735548224888132e063f92db585759b422570621d4
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.13-1.debian.tar.xz' libcroco_0.6.13-1.debian.tar.xz 7192 SHA256:922d4f962f7608e1ff46700dc26aa6198aa1a5099aaceebe75e9695ce3b8e374
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

### `dpkg` source package: `libedit=3.1-20191025-1`

Binary Packages:

- `libedit2:amd64=3.1-20191025-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libedit/3.1-20191025-1/


### `dpkg` source package: `liberror-perl=0.17028-1`

Binary Packages:

- `liberror-perl=0.17028-1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17028-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17028-1.dsc' liberror-perl_0.17028-1.dsc 2336 SHA256:fd87a6734867c9f7e559324219d91d4dc6234e1730c1b6d689a1710a812bf7d8
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17028.orig.tar.gz' liberror-perl_0.17028.orig.tar.gz 33234 SHA256:3ad85c5e58b31c8903006298424a51bba39f1840e324f5ae612eabc8b935e960
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17028-1.debian.tar.xz' liberror-perl_0.17028-1.debian.tar.xz 4956 SHA256:cc527461cae0692e46dfde26464a4c464be05414cd54a764305271b4e4afc4db
```

### `dpkg` source package: `libevent=2.1.11-stable-1`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.11-stable-1`
- `libevent-core-2.1-7:amd64=2.1.11-stable-1`
- `libevent-dev=2.1.11-stable-1`
- `libevent-extra-2.1-7:amd64=2.1.11-stable-1`
- `libevent-openssl-2.1-7:amd64=2.1.11-stable-1`
- `libevent-pthreads-2.1-7:amd64=2.1.11-stable-1`

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
$ apt-get source -qq --print-uris libevent=2.1.11-stable-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable-1.dsc' libevent_2.1.11-stable-1.dsc 2526 SHA256:b07a15f54f2ab403eed9aa648a1ea9bee05a5a5362570d334a76597e79a1d795
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable.orig.tar.gz' libevent_2.1.11-stable.orig.tar.gz 1082234 SHA256:a65bac6202ea8c5609fd5c7e480e6d25de467ea1917c08290c521752f147283d
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable.orig.tar.gz.asc' libevent_2.1.11-stable.orig.tar.gz.asc 488 SHA256:9add12a6852022f675e4388cb1ac0fdcd68c6c1bc6e5212fae78d3f1c00f2826
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable-1.debian.tar.xz' libevent_2.1.11-stable-1.debian.tar.xz 17264 SHA256:fae364ea17e708a73572dd8b0add7fcded427c9e2b2405679738459c6f02de8d
```

### `dpkg` source package: `libexif=0.6.21-5.1`

Binary Packages:

- `libexif-dev:amd64=0.6.21-5.1`
- `libexif12:amd64=0.6.21-5.1`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.21-5.1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21-5.1.dsc' libexif_0.6.21-5.1.dsc 2272 SHA256:98676c725f48a1602b50499329df85545c997825705980ce5d27ec77effd7310
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21.orig.tar.gz' libexif_0.6.21.orig.tar.gz 2081615 SHA256:edb7eb13664cf950a6edd132b75e99afe61c5effe2f16494e6d27bc404b287bf
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21-5.1.debian.tar.xz' libexif_0.6.21-5.1.debian.tar.xz 13020 SHA256:e026131413e0a951323e8325c9ce175fdb51d7820140c3e79db2a0b25d453c48
```

### `dpkg` source package: `libffi=3.2.1-9`

Binary Packages:

- `libffi-dev:amd64=3.2.1-9`
- `libffi6:amd64=3.2.1-9`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-9
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-9.dsc' libffi_3.2.1-9.dsc 2000 SHA256:28beaed76f2ce4c6a3ce1527eb07534c8ef4bf624a42c803fea045c416f8faa5
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-9.debian.tar.xz' libffi_3.2.1-9.debian.tar.xz 17148 SHA256:26e3cfd358733832da251778bc615a42b908d7779cf8b8d7fc2bdee4660bbbce
```

### `dpkg` source package: `libgcrypt20=1.8.5-3ubuntu1`

Binary Packages:

- `libgcrypt20:amd64=1.8.5-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.5-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-3ubuntu1.dsc' libgcrypt20_1.8.5-3ubuntu1.dsc 2944 SHA256:4c2a1ae5bb86ad57f794dc86cd8809e23eacf0607d950e026558aaea78dc10dd
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2' libgcrypt20_1.8.5.orig.tar.bz2 2991291 SHA256:3b4a2a94cb637eff5bdebbcaf46f4d95c4f25206f459809339cdada0eb577ac3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2.asc' libgcrypt20_1.8.5.orig.tar.bz2.asc 488 SHA256:4b24fda7847cd2b70ab19f4c38004a76bbdac46a1ddccff973ae88ba1296a22d
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-3ubuntu1.debian.tar.xz' libgcrypt20_1.8.5-3ubuntu1.debian.tar.xz 29972 SHA256:db6e34b46dc0b5e1142c4428538d4e07a6d533de33b79001263596c053f33770
```

### `dpkg` source package: `libgpg-error=1.36-7`

Binary Packages:

- `libgpg-error0:amd64=1.36-7`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.36-7
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.36-7.dsc' libgpg-error_1.36-7.dsc 2220 SHA256:08d532f83371e4e2def8ba8c80ab3c830eb2a749a9d40d7a529ee8cf3e058bce
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.36.orig.tar.bz2' libgpg-error_1.36.orig.tar.bz2 920542 SHA256:babd98437208c163175c29453f8681094bcaf92968a15cafb1a276076b33c97c
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.36.orig.tar.bz2.asc' libgpg-error_1.36.orig.tar.bz2.asc 534 SHA256:ef7b12e7a2c348d8e9cb3fb63b4069feeadcfb69074786559064381d179f1df7
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.36-7.debian.tar.xz' libgpg-error_1.36-7.debian.tar.xz 17208 SHA256:2ece6be72b1cea60990d75f7806f8dabb94114c89367b09fe8964cd343f5aebd
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

### `dpkg` source package: `libidn2=2.2.0-2`

Binary Packages:

- `libidn2-0:amd64=2.2.0-2`

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
$ apt-get source -qq --print-uris libidn2=2.2.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.2.0-2.dsc' libidn2_2.2.0-2.dsc 2436 SHA256:a5c5ece3748beaba9ce0a0b29cdab2fe9d861a965a7a96101a49f194acf759d6
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.2.0.orig.tar.gz' libidn2_2.2.0.orig.tar.gz 2110743 SHA256:fc734732b506d878753ec6606982bf7b936e868c25c30ddb0d83f7d7056381fe
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.2.0-2.debian.tar.xz' libidn2_2.2.0-2.debian.tar.xz 11184 SHA256:b38ce002d7eb1abbf2c870ac9570cd06a5087693f359b133defbf44b06f8784d
```

### `dpkg` source package: `libjpeg-turbo=2.0.3-0ubuntu1`

Binary Packages:

- `libjpeg-turbo8:amd64=2.0.3-0ubuntu1`
- `libjpeg-turbo8-dev:amd64=2.0.3-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.0.3-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3-0ubuntu1.dsc' libjpeg-turbo_2.0.3-0ubuntu1.dsc 1651 SHA256:8523ac58f878db995950b0ce7eb2b10c629012a5b4cb2534969c85a14b807913
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3.orig.tar.gz' libjpeg-turbo_2.0.3.orig.tar.gz 2161279 SHA256:a69598bf079463b34d45ca7268462a18b6507fdaa62bb1dfd212f02041499b5d
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3-0ubuntu1.debian.tar.xz' libjpeg-turbo_2.0.3-0ubuntu1.debian.tar.xz 16944 SHA256:72b44a4cff7d6c5cd1543b0d6fe1c0320903b93ceac7113334477bd0af834ab7
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

### `dpkg` source package: `libmaxminddb=1.3.2-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.3.2-1`
- `libmaxminddb0:amd64=1.3.2-1`

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
$ apt-get source -qq --print-uris libmaxminddb=1.3.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.3.2-1.dsc' libmaxminddb_1.3.2-1.dsc 2104 SHA256:c75309a506da7a68fe74b13ab3f8f3024a377859ec9fb77aa2e4c057550c1158
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.3.2.orig.tar.gz' libmaxminddb_1.3.2.orig.tar.gz 248665 SHA256:5fa35b5e7ae3ed11b9c392d6ea38572966c1ceaeab4e2598174911978ea0c027
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.3.2-1.debian.tar.xz' libmaxminddb_1.3.2-1.debian.tar.xz 4868 SHA256:25b816d507995b6fe8d8430f43215f79cc1191e0f931e130e70a7060fa2992ee
```

### `dpkg` source package: `libpng1.6=1.6.37-1`

Binary Packages:

- `libpng-dev:amd64=1.6.37-1`
- `libpng16-16:amd64=1.6.37-1`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.37-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-1.dsc' libpng1.6_1.6.37-1.dsc 2225 SHA256:e2e764f884c1c0b78c25728cdddd8c28e4a30ed9acab261e211ffacc7957156f
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA256:ca74a0dace179a8422187671aee97dd3892b53e168627145271cad5b5ac81307
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-1.debian.tar.xz' libpng1.6_1.6.37-1.debian.tar.xz 31496 SHA256:1be8793d8ef9265dd43f526540a55c5114c427f2a18862d2238a193bdad9b6a1
```

### `dpkg` source package: `libpsl=0.20.2-2`

Binary Packages:

- `libpsl5:amd64=0.20.2-2`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.20.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.20.2-2.dsc' libpsl_0.20.2-2.dsc 1637 SHA256:ae401852522d748f1222b91734bc5bd7c6db0de843dd675adc180f2a1884c94d
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.20.2.orig.tar.gz' libpsl_0.20.2.orig.tar.gz 8590430 SHA256:94d2b5e00e9aa761ae7efbaa67edc00d5298487ed9706eb4789e349012993c31
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.20.2-2.debian.tar.xz' libpsl_0.20.2-2.debian.tar.xz 9920 SHA256:1f008454fdb973964202020fb700d5028e001b7eaa4e77eeab8ebc99b749ea51
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

### `dpkg` source package: `librsvg=2.46.4-1ubuntu1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.46.4-1ubuntu1`
- `librsvg2-2:amd64=2.46.4-1ubuntu1`
- `librsvg2-common:amd64=2.46.4-1ubuntu1`
- `librsvg2-dev:amd64=2.46.4-1ubuntu1`

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
$ apt-get source -qq --print-uris librsvg=2.46.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.46.4-1ubuntu1.dsc' librsvg_2.46.4-1ubuntu1.dsc 2987 SHA256:ca305c9a9493c2a0a83961611f96e5fbd12061220e8806cc2e4011f7928a9f8c
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.46.4.orig.tar.xz' librsvg_2.46.4.orig.tar.xz 12680904 SHA256:b45b9ee3b64c58baaf800bcdff5fcd04d79930dba4c56e46e0d3b0aead40cc29
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.46.4-1ubuntu1.debian.tar.xz' librsvg_2.46.4-1ubuntu1.debian.tar.xz 23020 SHA256:1e04df08802e712539f71aacd3bd68f0d2fcac9b1886f20e577a6f83413dc32c
```

### `dpkg` source package: `libseccomp=2.4.1-0ubuntu0.19.10.3`

Binary Packages:

- `libseccomp2:amd64=2.4.1-0ubuntu0.19.10.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libselinux=3.0-1`

Binary Packages:

- `libselinux1:amd64=3.0-1`
- `libselinux1-dev:amd64=3.0-1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0-1.dsc' libselinux_3.0-1.dsc 2220 SHA256:9f147a02241eb6e3db4b2bcad55cf5fd516702788f6561abbe82e9fd5faed6d7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0.orig.tar.gz' libselinux_3.0.orig.tar.gz 212096 SHA256:2ea2b30f671dae9d6b1391cbe8fb2ce5d36a3ee4fb1cd3c32f0d933c31b82433
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0-1.debian.tar.xz' libselinux_3.0-1.debian.tar.xz 23568 SHA256:765b937149864b2fe265c1e9df7d8f5f8f1d384c1ef351458a996f284a4392ef
```

### `dpkg` source package: `libsemanage=2.9-3build1`

Binary Packages:

- `libsemanage-common=2.9-3build1`
- `libsemanage1:amd64=2.9-3build1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libsepol=3.0-1`

Binary Packages:

- `libsepol1:amd64=3.0-1`
- `libsepol1-dev:amd64=3.0-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`, `/usr/share/doc/libsepol1-dev/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0-1.dsc' libsepol_3.0-1.dsc 1770 SHA256:0073de5844605d380dd56f6630678ad91459496dc768fa9eb4d8cc7f693f5c1a
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0.orig.tar.gz' libsepol_3.0.orig.tar.gz 473864 SHA256:5b7ae1881909f1048b06f7a0c364c5c8a86ec12e0ec76e740fe9595a6033eb79
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0-1.debian.tar.xz' libsepol_3.0-1.debian.tar.xz 14224 SHA256:a16b5bc3c041e016d01794d1a1b9826ed4426862622c05526e93607c325ec328
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2.dsc' libsigsegv_2.12-2.dsc 2363 SHA256:b081b244de2f427345838f379405d8438c29db1fa746a4e270167ae7cb10c079
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz' libsigsegv_2.12.orig.tar.gz 451408 SHA256:3ae1af359eebaa4ffc5896a1aee3568c052c99879316a1ab57f8fe1789c390b6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz.asc' libsigsegv_2.12.orig.tar.gz.asc 2442 SHA256:1861a9a182bbb7a24a18f7e43fe0fa3eb6f6fd53780b30e01990677112694dfc
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2.debian.tar.xz' libsigsegv_2.12-2.debian.tar.xz 8340 SHA256:73940fb346f7afd90c93a341164cd175349e0507de8b1c05b0834b598c372260
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

### `dpkg` source package: `libssh=0.9.0-1ubuntu5`

Binary Packages:

- `libssh-4:amd64=0.9.0-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.0-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.0-1ubuntu5.dsc' libssh_0.9.0-1ubuntu5.dsc 2530 SHA256:f1dfe8beea41c82c3f7aab10fad0074a5b2b503f88ee3a1159c6c96417fbf79b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.0.orig.tar.xz' libssh_0.9.0.orig.tar.xz 487628 SHA256:25303c2995e663cd169fdd902bae88106f48242d7e96311d74f812023482c7a5
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.0-1ubuntu5.debian.tar.xz' libssh_0.9.0-1ubuntu5.debian.tar.xz 37924 SHA256:9f95e62446289df0f47370b5e00e6784fde17c476b6aa439b553494c1adc0210
```

### `dpkg` source package: `libtasn1-6=4.14-3`

Binary Packages:

- `libtasn1-6:amd64=4.14-3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libtasn1-6/4.14-3/


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

### `dpkg` source package: `libtool=2.4.6-11`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-11`
- `libltdl7:amd64=2.4.6-11`
- `libtool=2.4.6-11`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-11
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-11.dsc' libtool_2.4.6-11.dsc 2489 SHA256:ce91f8392456c133e203e68e203b114f43f038760ec116e9e9361fe6f72e407e
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-11.debian.tar.xz' libtool_2.4.6-11.debian.tar.xz 48948 SHA256:2e1ff4e0bf7ef53fc772c61d6a33dd2e6128525621a0e734fa5a3071785e5ec6
```

### `dpkg` source package: `libunistring=0.9.10-2`

Binary Packages:

- `libunistring2:amd64=0.9.10-2`

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
$ apt-get source -qq --print-uris libunistring=0.9.10-2
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-2.dsc' libunistring_0.9.10-2.dsc 2206 SHA256:c6faf64e2d978ec074ebf88264730121dfd03cc1639df94b5dc3eb05b1678532
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-2.debian.tar.xz' libunistring_0.9.10-2.debian.tar.xz 40708 SHA256:5e291a1a15549d12c64575c72868a8c94586715d35062b5efb48fe9a9d09924e
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

### `dpkg` source package: `libwmf=0.2.8.4-15ubuntu1`

Binary Packages:

- `libwmf-dev=0.2.8.4-15ubuntu1`
- `libwmf0.2-7:amd64=0.2.8.4-15ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-15ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-15ubuntu1.dsc' libwmf_0.2.8.4-15ubuntu1.dsc 2329 SHA256:18a53170ac7d0f5f912dbf888e0e33dd476a37b706b248877e30b5afdab86882
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-15ubuntu1.debian.tar.xz' libwmf_0.2.8.4-15ubuntu1.debian.tar.xz 12836 SHA256:a7be255896e272aa648c7d5e0e65d2e1ea53e272a762dcb34d9abddf26efc2c3
```

### `dpkg` source package: `libx11=2:1.6.8-1`

Binary Packages:

- `libx11-6:amd64=2:1.6.8-1`
- `libx11-data=2:1.6.8-1`
- `libx11-dev:amd64=2:1.6.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.8-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.8-1.dsc' libx11_1.6.8-1.dsc 2639 SHA256:4c64049b12059e10fa6986afab53f16a88f8d67ab4ba5778773d840dc1dd1dcc
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.8.orig.tar.gz' libx11_1.6.8.orig.tar.gz 3144482 SHA256:69d1a27cba722dca897198a23fa8d3cad3ec0c715e00205ea4398ec68a4258a5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.8.orig.tar.gz.asc' libx11_1.6.8.orig.tar.gz.asc 358 SHA256:acbbc22289a43defbb0b2fcdc083587492feec31dfef49e9829009986be84f79
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.8-1.diff.gz' libx11_1.6.8-1.diff.gz 56202 SHA256:0f43c4539885873d8bbc6e0387313bc9379ee2054e5c1ab4eab724386e2b1ba3
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

### `dpkg` source package: `libxcb=1.13.1-2`

Binary Packages:

- `libxcb-render0:amd64=1.13.1-2`
- `libxcb-render0-dev:amd64=1.13.1-2`
- `libxcb-shm0:amd64=1.13.1-2`
- `libxcb-shm0-dev:amd64=1.13.1-2`
- `libxcb1:amd64=1.13.1-2`
- `libxcb1-dev:amd64=1.13.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.13.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13.1-2.dsc' libxcb_1.13.1-2.dsc 5375 SHA256:08ee999e42e93af418ab27e772c7e1b464950ea2cbe8cd7ee6759e9a170dd9e8
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13.1.orig.tar.gz' libxcb_1.13.1.orig.tar.gz 636748 SHA256:f09a76971437780a602303170fd51b5f7474051722bc39d566a272d2c4bde1b5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13.1-2.diff.gz' libxcb_1.13.1-2.diff.gz 25487 SHA256:8ee5244ada4bf1e9af0bbd43463877f6185d63942e89e5800613ee4a2627a016
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

### `dpkg` source package: `libxml2=2.9.4+dfsg1-8ubuntu1`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-8ubuntu1`
- `libxml2-dev:amd64=2.9.4+dfsg1-8ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.4+dfsg1-8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-8ubuntu1.dsc' libxml2_2.9.4+dfsg1-8ubuntu1.dsc 2996 SHA256:22a204942242059f4ae6ef5832d796ae276b7d5bbebb42b1810ca5ad4f79f01f
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA256:a74ad55e346aa0b2b41903e66d21f8f3d2a736b3f41e32496376861ab484184e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-8ubuntu1.debian.tar.xz' libxml2_2.9.4+dfsg1-8ubuntu1.debian.tar.xz 39140 SHA256:88f4116978119325759fc8b453a047858c3cc997f59b92ba221251d0ec550d55
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

### `dpkg` source package: `libxslt=1.1.33-0ubuntu1`

Binary Packages:

- `libxslt1-dev:amd64=1.1.33-0ubuntu1`
- `libxslt1.1:amd64=1.1.33-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `libzstd=1.4.4+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.4.4+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.4+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.4+dfsg-1.dsc' libzstd_1.4.4+dfsg-1.dsc 2285 SHA256:9306fb9c71a3449a4b0bdfa67322f519e8c74efdbcee884f63c66fbd0e2c0377
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.4+dfsg.orig.tar.xz' libzstd_1.4.4+dfsg.orig.tar.xz 1357144 SHA256:be9f9bfd3f6816f21e1108869a9acad6efdc4882ed3f7a1f58ec752f67864890
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.4+dfsg-1.debian.tar.xz' libzstd_1.4.4+dfsg-1.debian.tar.xz 16040 SHA256:bb6c7e2206c3c0a2c780ce824efb90f03bc94eeb8497c881f6c8dc28d902d103
```

### `dpkg` source package: `linux=5.3.0-24.26`

Binary Packages:

- `linux-libc-dev:amd64=5.3.0-24.26`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris linux=5.3.0-24.26
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.3.0-24.26.dsc' linux_5.3.0-24.26.dsc 8323 SHA256:9a0f40c9239a8146d0530686c16dfa34c881ad05da3ae886554bb0ed068fdbc7
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.3.0.orig.tar.gz' linux_5.3.0.orig.tar.gz 168029263 SHA256:44edffd835819ac7156f2f4bb7512d25f8cf6eab098b09c9ef0c3c06a01148ef
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.3.0-24.26.diff.gz' linux_5.3.0-24.26.diff.gz 3057437 SHA256:86849df3d725b3977043f4b57c1fbb7284efa4a7dfd40b37406cd60417b668fa
```

### `dpkg` source package: `lsb=11.1.0ubuntu1`

Binary Packages:

- `lsb-base=11.1.0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lz4=1.9.1-2`

Binary Packages:

- `liblz4-1:amd64=1.9.1-2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/lz4/1.9.1-2/


### `dpkg` source package: `lzo2=2.10-0.1`

Binary Packages:

- `liblzo2-2:amd64=2.10-0.1`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.10-0.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-0.1.dsc' lzo2_2.10-0.1.dsc 1869 SHA256:49cdf2efab29d7dd8a907730a37c2c5ca312d9c2150f8e37663838b122856aff
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10.orig.tar.gz' lzo2_2.10.orig.tar.gz 600622 SHA256:c0f892943208266f9b6543b3ae308fab6284c5c90e627931446fb49b4221a072
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-0.1.debian.tar.xz' lzo2_2.10-0.1.debian.tar.xz 6032 SHA256:0d57d800afc09a44180cb323f4c5d77e9a5f29c1ba53a3ebdd5ec225b2d44723
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

### `dpkg` source package: `make-dfsg=4.2.1-1.2`

Binary Packages:

- `make=4.2.1-1.2`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.2.1-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.dsc' make-dfsg_4.2.1-1.2.dsc 2019 SHA256:0c8a2da5d51e03bf43e2929322d5a8406f08e5ee2d81a71ed6e5a8734f1b05cb
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.2.1.orig.tar.gz' make-dfsg_4.2.1.orig.tar.gz 1485018 SHA256:480405e8995796ea47cc54b281b7855280f0d815d296a1af1993eeeb72074e39
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.diff.gz' make-dfsg_4.2.1-1.2.diff.gz 53108 SHA256:80e0b96cee381391a5d3322317075e23d8474c92c5fa4fecd334bc2e0920887b
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

### `dpkg` source package: `mercurial=4.8.2-1ubuntu4`

Binary Packages:

- `mercurial=4.8.2-1ubuntu4`
- `mercurial-common=4.8.2-1ubuntu4`

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

### `dpkg` source package: `mpdecimal=2.4.2-2`

Binary Packages:

- `libmpdec2:amd64=2.4.2-2`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-2.dsc' mpdecimal_2.4.2-2.dsc 1932 SHA256:716e61fc8315a22804adf8403e4d332c1883235b5c3801b6769e6040dc962fe3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-2.debian.tar.xz' mpdecimal_2.4.2-2.debian.tar.xz 5256 SHA256:159113f11169afc675a431840792e1ed8c2d00438bf3e1c5a3eb2c17d9e8da3d
```

### `dpkg` source package: `mpfr4=4.0.2-1`

Binary Packages:

- `libmpfr6:amd64=4.0.2-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.0.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.2-1.dsc' mpfr4_4.0.2-1.dsc 1972 SHA256:9021ec2462ed0e73ea1379266740473abf5f826be819226497729f6c6b02e672
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.2.orig.tar.xz' mpfr4_4.0.2.orig.tar.xz 1441996 SHA256:1d3be708604eae0e42d578ba93b390c2a145f17743a744d8f3f8c2ad5855a38a
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.2-1.debian.tar.xz' mpfr4_4.0.2-1.debian.tar.xz 10544 SHA256:99c4d35654f33340f0efdec67142a34753157b20334cadad9018f5eab29738da
```

### `dpkg` source package: `mysql-8.0=8.0.18-0ubuntu4`

Binary Packages:

- `libmysqlclient-dev=8.0.18-0ubuntu4`
- `libmysqlclient21:amd64=8.0.18-0ubuntu4`

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

Source:

```console
$ apt-get source -qq --print-uris mysql-8.0=8.0.18-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.18-0ubuntu4.dsc' mysql-8.0_8.0.18-0ubuntu4.dsc 3439 SHA256:fa9cb754110ca6acdbbd938cee312c463623d90492e0e00481fbb7f5ce0d5a74
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.18.orig.tar.gz' mysql-8.0_8.0.18.orig.tar.gz 194953221 SHA256:0eccd9d79c04ba0ca661136bb29085e3833d9c48ed022d0b9aba12236994186b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.18-0ubuntu4.debian.tar.xz' mysql-8.0_8.0.18-0ubuntu4.debian.tar.xz 157260 SHA256:f9f104beb5ff91820e5d58853e8352bceaa6215757803ad7d7b3648b96176e02
```

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

### `dpkg` source package: `ncurses=6.1+20191019-1ubuntu1`

Binary Packages:

- `libncurses-dev:amd64=6.1+20191019-1ubuntu1`
- `libncurses5-dev:amd64=6.1+20191019-1ubuntu1`
- `libncurses6:amd64=6.1+20191019-1ubuntu1`
- `libncursesw5-dev:amd64=6.1+20191019-1ubuntu1`
- `libncursesw6:amd64=6.1+20191019-1ubuntu1`
- `libtinfo6:amd64=6.1+20191019-1ubuntu1`
- `ncurses-base=6.1+20191019-1ubuntu1`
- `ncurses-bin=6.1+20191019-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1+20191019-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20191019-1ubuntu1.dsc' ncurses_6.1+20191019-1ubuntu1.dsc 4581 SHA256:847e7864196f3192f379cb56088f0cb1861f1cdf55426b9702d830d28062c919
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20191019.orig.tar.gz' ncurses_6.1+20191019.orig.tar.gz 3463374 SHA256:b42ca297f1823c1b1f2baaf46da5a61f690dc857600c7eb95d02432bd9905d3a
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20191019.orig.tar.gz.asc' ncurses_6.1+20191019.orig.tar.gz.asc 265 SHA256:670ab32ca07bf61d08d62731b1beef62194f684761bb73b2de1143949b0e88b6
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20191019-1ubuntu1.debian.tar.xz' ncurses_6.1+20191019-1ubuntu1.debian.tar.xz 63684 SHA256:6bcbc221c02ea3bb89a4059370fe3f548fb4085f5fed1a42eb3bf115aa382db0
```

### `dpkg` source package: `netbase=5.6`

Binary Packages:

- `netbase=5.6`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.6
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.6.dsc' netbase_5.6.dsc 1306 SHA256:fea82cc64b508a8f5ff3a16dfadce1660468d0a347df5c0ff56a2caaa57668a6
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.6.tar.xz' netbase_5.6.tar.xz 31684 SHA256:5d93a099deb28869b7306e914700fafbd293b55bdb5df05a5aa6effd0af5930c
```

### `dpkg` source package: `nettle=3.5.1+really3.5.1-2`

Binary Packages:

- `libhogweed5:amd64=3.5.1+really3.5.1-2`
- `libnettle7:amd64=3.5.1+really3.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libhogweed5/copyright`, `/usr/share/doc/libnettle7/copyright`)

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
$ apt-get source -qq --print-uris nettle=3.5.1+really3.5.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.dsc' nettle_3.5.1+really3.5.1-2.dsc 2375 SHA256:a64c789e3997a2bba012e0c136de9c11b1bc95cf03069c35d26b00582481eecf
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz' nettle_3.5.1+really3.5.1.orig.tar.gz 1989593 SHA256:75cca1998761b02e16f2db56da52992aef622bf55a3b45ec538bc2eedadc9419
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz.asc' nettle_3.5.1+really3.5.1.orig.tar.gz.asc 573 SHA256:557116e471c7c4556148866b5cec056d6de5f26d080e5930154018be6a9d893e
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.debian.tar.xz' nettle_3.5.1+really3.5.1-2.debian.tar.xz 20044 SHA256:7e816adb06d13913bcd350ca6cb777230b82508ca2d358a4062e5676bf335529
```

### `dpkg` source package: `nghttp2=1.40.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.40.0-1`

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
$ apt-get source -qq --print-uris nghttp2=1.40.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.40.0-1.dsc' nghttp2_1.40.0-1.dsc 2548 SHA256:92de95dcdf9e2a84a7ea1be6a52df510910e376937ec1f75bc75654f04f846ea
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.40.0.orig.tar.bz2' nghttp2_1.40.0.orig.tar.bz2 1937537 SHA256:82758e13727945f2408d0612762e4655180b039f058d5ff40d055fa1497bd94f
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.40.0-1.debian.tar.xz' nghttp2_1.40.0-1.debian.tar.xz 12692 SHA256:7c8589297f5da5f0995aa8bd08bfbe4764da6d841338df61d7b69ab1f5fcfedb
```

### `dpkg` source package: `npth=1.6-1`

Binary Packages:

- `libnpth0:amd64=1.6-1`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-1.dsc' npth_1.6-1.dsc 1925 SHA256:2c327ce494f702482e79ed620445cba303c4449dd0768fecee3ee7d5ade2544a
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA256:1393abd9adcf0762d34798dc34fdcf4d0d22a8410721e76f1e3afcd1daa4e2d1
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-1.debian.tar.xz' npth_1.6-1.debian.tar.xz 10532 SHA256:d312d4a3cf1d082e2f2cf3ea752c41d34f7e120f77a941c6c1680e6093834353
```

### `dpkg` source package: `openexr=2.3.0-6`

Binary Packages:

- `libopenexr-dev=2.3.0-6`
- `libopenexr24:amd64=2.3.0-6`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr24/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.3.0-6
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0-6.dsc' openexr_2.3.0-6.dsc 2678 SHA256:e02a733dff068fbc45286b1f1b99610e4a8234abd2720ba7a6317f483c2369d1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0.orig.tar.gz' openexr_2.3.0.orig.tar.gz 18416222 SHA256:1dea3145eb3962025e27edb99c97e8cfc67d6310403bbd643e97c364ebf8ff09
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0.orig.tar.gz.asc' openexr_2.3.0.orig.tar.gz.asc 566 SHA256:809172c26aacae76d2caf92d13015ec829853f1ea9b25512c0307c66005e4dcc
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.3.0-6.debian.tar.xz' openexr_2.3.0-6.debian.tar.xz 20968 SHA256:38fc6e887d7bb8c0003e353f90cfbbfb61c986e7d0e349182426e64a2f1c48e8
```

### `dpkg` source package: `openldap=2.4.48+dfsg-1ubuntu3`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.48+dfsg-1ubuntu3`
- `libldap-common=2.4.48+dfsg-1ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.48+dfsg-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.48+dfsg-1ubuntu3.dsc' openldap_2.4.48+dfsg-1ubuntu3.dsc 3023 SHA256:f540516ed8698d32fac97b5d9a959361d6c3ab48744131b60682e7233c044fef
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.48+dfsg.orig.tar.gz' openldap_2.4.48+dfsg.orig.tar.gz 4875429 SHA256:8645601c28f094b01baed02a604479b175a45ba010e407212d214313bc6a80ba
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.48+dfsg-1ubuntu3.debian.tar.xz' openldap_2.4.48+dfsg-1ubuntu3.debian.tar.xz 179236 SHA256:74d98ba63e9bd1c33a967eeabec091fb10536306eb04bc6f9511ddb06de88c77
```

### `dpkg` source package: `openssh=1:8.1p1-1`

Binary Packages:

- `openssh-client=1:8.1p1-1`

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
$ apt-get source -qq --print-uris openssh=1:8.1p1-1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.1p1-1.dsc' openssh_8.1p1-1.dsc 3316 SHA256:01e3152f72f1352078308842357f56f5206edcad7c5228ff8c13be83be69349b
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.1p1.orig.tar.gz' openssh_8.1p1.orig.tar.gz 1625894 SHA256:02f5dbef3835d0753556f973cd57b4c19b6b1f6cd24c03445e23ac77ca1b93ff
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.1p1.orig.tar.gz.asc' openssh_8.1p1.orig.tar.gz.asc 683 SHA256:da3f623f0131b55c8199fbbd86be0748d00c6e1e098dfc0ebea664901c9a7ab4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.1p1-1.debian.tar.xz' openssh_8.1p1-1.debian.tar.xz 171604 SHA256:d93a83ebd34b917a307c2876d7a3ad778277f745f38634b961cba65bf07cd10c
```

### `dpkg` source package: `openssl=1.1.1c-1ubuntu4`

Binary Packages:

- `libssl-dev:amd64=1.1.1c-1ubuntu4`
- `libssl1.1:amd64=1.1.1c-1ubuntu4`
- `openssl=1.1.1c-1ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1c-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1c-1ubuntu4.dsc' openssl_1.1.1c-1ubuntu4.dsc 2724 SHA256:aea5f309503b93e512f68a9e5f0c15421df854accf41c2645e36e227ff3d52c7
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1c.orig.tar.gz' openssl_1.1.1c.orig.tar.gz 8864262 SHA256:f6fb3079ad15076154eda9413fed42877d668e7069d9b87396d0804fdb3f4c90
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1c.orig.tar.gz.asc' openssl_1.1.1c.orig.tar.gz.asc 833 SHA256:12663f13a236f0ccb4e74fe2d61b7b2dc1dbdeb83767b21505e61af67d2da6b8
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1c-1ubuntu4.debian.tar.xz' openssl_1.1.1c-1ubuntu4.debian.tar.xz 121932 SHA256:8f6b99871e06689026aa0bbb46739915a19ba2d9efd26969f0ae172ad20f664f
```

### `dpkg` source package: `p11-kit=0.23.18.1-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.18.1-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.18.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.18.1-2.dsc' p11-kit_0.23.18.1-2.dsc 2440 SHA256:608a5664e8a0c379d86e7a5696c1e86b2079e379e4b318103a1b8eb769edac50
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.18.1.orig.tar.gz' p11-kit_0.23.18.1.orig.tar.gz 1305755 SHA256:34c3bd8c0050dd7c4e6228aecf0f168de0a1b34562ddbf74a1c70904c2523c6f
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.18.1.orig.tar.gz.asc' p11-kit_0.23.18.1.orig.tar.gz.asc 854 SHA256:25e209a0eec76740d9906d86df0120505901f99a813e31f2bb1f7607416ec042
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.18.1-2.debian.tar.xz' p11-kit_0.23.18.1-2.debian.tar.xz 21648 SHA256:4f970522a2fdc301879edf8215ef6045423366c0e9b610c6d86b03d2a3e296aa
```

### `dpkg` source package: `pam=1.3.1-5ubuntu1`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu1`
- `libpam-modules-bin=1.3.1-5ubuntu1`
- `libpam-runtime=1.3.1-5ubuntu1`
- `libpam0g:amd64=1.3.1-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pango1.0=1.44.7-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.44.7-1`
- `libpangocairo-1.0-0:amd64=1.44.7-1`
- `libpangoft2-1.0-0:amd64=1.44.7-1`

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
$ apt-get source -qq --print-uris pango1.0=1.44.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.44.7-1.dsc' pango1.0_1.44.7-1.dsc 3322 SHA256:183424385b21ec4f47ecd65eee32272e49690f12fde12ccea00e2f39107ca4cd
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.44.7.orig.tar.xz' pango1.0_1.44.7.orig.tar.xz 521384 SHA256:66a5b6cc13db73efed67b8e933584509f8ddb7b10a8a40c3850ca4a985ea1b1f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.44.7-1.debian.tar.xz' pango1.0_1.44.7-1.debian.tar.xz 31424 SHA256:e57401cc09c03ea13fbb6f8d7414836b18eaf4b9563d147dfd34be32e4e8def1
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

### `dpkg` source package: `pcre3=2:8.39-12`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-12`
- `libpcre3:amd64=2:8.39-12`
- `libpcre3-dev:amd64=2:8.39-12`
- `libpcre32-3:amd64=2:8.39-12`
- `libpcrecpp0v5:amd64=2:8.39-12`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-12
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-12.dsc' pcre3_8.39-12.dsc 2226 SHA256:7660921533f286d211bc129318327041ceb80d3d21e91c1ae7c10f284342c5e0
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-12.debian.tar.gz' pcre3_8.39-12.debian.tar.gz 26509 SHA256:ee193ddee446f0bdb966fca5987ef871da7a528a473304285619988102371c4c
```

### `dpkg` source package: `perl=5.30.0-9`

Binary Packages:

- `libperl5.30:amd64=5.30.0-9`
- `perl=5.30.0-9`
- `perl-base=5.30.0-9`
- `perl-modules-5.30=5.30.0-9`

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
$ apt-get source -qq --print-uris perl=5.30.0-9
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0-9.dsc' perl_5.30.0-9.dsc 2983 SHA256:05eb4e5e304ed6d5d198405fa2f85d0d3decc7342536508d240c3f41e07906b1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0.orig-regen-configure.tar.gz' perl_5.30.0.orig-regen-configure.tar.gz 833235 SHA256:fc55a7309f9e2c404119b005774fc85a8488bad047aee611d17bbe2d608bf4de
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0.orig.tar.xz' perl_5.30.0.orig.tar.xz 12419868 SHA256:ac501cad4af904d33370a9ea39dbb7a8ad4cb19bc7bc8a9c17d8dc3e81ef6306
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0-9.debian.tar.xz' perl_5.30.0-9.debian.tar.xz 161876 SHA256:6140c1b94ba811aad5cab98041f5ccae26a86f619fc738194956ef7fb707b552
```

### `dpkg` source package: `pinentry=1.1.0-3`

Binary Packages:

- `pinentry-curses=1.1.0-3`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-3.dsc' pinentry_1.1.0-3.dsc 2060 SHA256:007e0ef8f0c289d8df814c2ef6fc66c880eb587f4b2ffcab2e229ea324076921
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-3.debian.tar.xz' pinentry_1.1.0-3.debian.tar.xz 17124 SHA256:41315d69b0c0c06f2c1bff846b2d87519a6fa59e8d295d9e6d1a6b7e343b6168
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

### `dpkg` source package: `pkg-config=0.29.1-0ubuntu3`

Binary Packages:

- `pkg-config=0.29.1-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.1-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu3.dsc' pkg-config_0.29.1-0ubuntu3.dsc 1893 SHA256:00b49dc3f2af4760ac41324aa73d358e25ff2d653d36cb471005dacf327e3fd3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1.orig.tar.gz' pkg-config_0.29.1.orig.tar.gz 2013454 SHA256:beb43c9e064555469bd4390dcfd8030b1536e0aa103f08d7abf7ae8cac0cb001
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu3.diff.gz' pkg-config_0.29.1-0ubuntu3.diff.gz 13488 SHA256:60e0ee7ce83c9717265f553b1aa605a5def96fabc53afb9dedc9e6c2e00228bb
```

### `dpkg` source package: `postgresql-12=12.1-1`

Binary Packages:

- `libpq-dev=12.1-1`
- `libpq5:amd64=12.1-1`

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
$ apt-get source -qq --print-uris postgresql-12=12.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.1-1.dsc' postgresql-12_12.1-1.dsc 3591 SHA256:ae23cb3e367e1996341e92e7546f8ab5a70bfb3eb6bd2f82fdefd677131fa006
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.1.orig.tar.bz2' postgresql-12_12.1.orig.tar.bz2 20213711 SHA256:a09bf3abbaf6763980d0f8acbb943b7629a8b20073de18d867aecdb7988483ed
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.1-1.debian.tar.xz' postgresql-12_12.1-1.debian.tar.xz 22520 SHA256:c8506ff2de2561a313e5a0daf84ff6f3be537b7777fb2825dde64435e5e38228
```

### `dpkg` source package: `procps=2:3.3.15-2ubuntu3`

Binary Packages:

- `libprocps7:amd64=2:3.3.15-2ubuntu3`
- `procps=2:3.3.15-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libprocps7/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.15-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.15-2ubuntu3.dsc' procps_3.3.15-2ubuntu3.dsc 1866 SHA256:c2cc91f94f67f271d5d9ce7ec4b0fc7a4701fcd827eefb5030685f0b775a61a2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.15.orig.tar.xz' procps_3.3.15.orig.tar.xz 903372 SHA256:82e8aa55b65eac116eee05f00d2a884a6374760d57100edd429d6e9b4953458d
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.15-2ubuntu3.debian.tar.xz' procps_3.3.15-2ubuntu3.debian.tar.xz 32560 SHA256:5faa3f8adfd573b58cb1919e6f02c65cf01c843c65bb8087c481ac7dbf03146f
```

### `dpkg` source package: `python-defaults=2.7.17-1`

Binary Packages:

- `libpython-stdlib:amd64=2.7.17-1`
- `libpython2-stdlib:amd64=2.7.17-1`
- `python=2.7.17-1`
- `python-minimal=2.7.17-1`
- `python2=2.7.17-1`
- `python2-minimal=2.7.17-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.17-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-defaults/python-defaults_2.7.17-1.dsc' python-defaults_2.7.17-1.dsc 2921 SHA256:282c49fecc189fbfc02564c92d99b8273156e4ca580746ee418a9c1974d155b8
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-defaults/python-defaults_2.7.17-1.tar.gz' python-defaults_2.7.17-1.tar.gz 82679 SHA256:c59e541b82ec5641e8bc6c9ebde927f12738b7de2d2414d84bec9101aa7fe0d0
```

### `dpkg` source package: `python2.7=2.7.17-1`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.17-1`
- `libpython2.7-stdlib:amd64=2.7.17-1`
- `python2.7=2.7.17-1`
- `python2.7-minimal=2.7.17-1`

Licenses: (parsed from: `/usr/share/doc/libpython2.7-minimal/copyright`, `/usr/share/doc/libpython2.7-stdlib/copyright`, `/usr/share/doc/python2.7/copyright`, `/usr/share/doc/python2.7-minimal/copyright`)

- `# Licensed to PSF under a Contributor Agreement`
- `* Permission to use this software in any way is granted without`
- `Apache`
- `Apache-2`
- `Apache-2.0`
- `Expat`
- `GPL-2`
- `ISC`
- `LGPL-2.1+`
- `PSF-2`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Python`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `implied`
- `see above, some license as Python`

Source:

```console
$ apt-get source -qq --print-uris python2.7=2.7.17-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.17-1.dsc' python2.7_2.7.17-1.dsc 3365 SHA256:edf165ecac0f41f5f2ee605dbb66b6e148f7437b1ebe16a6f1444fb8a6a6da22
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.17.orig.tar.gz' python2.7_2.7.17.orig.tar.gz 17535962 SHA256:f22059d09cdf9625e0a7284d24a13062044f5bf59d93a7f3382190dfa94cecde
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.17-1.diff.gz' python2.7_2.7.17-1.diff.gz 286003 SHA256:a71d752753f7aaf0c6bb49bae5dfa2f35db4265742b4709bbd12d816f9cef5c3
```

### `dpkg` source package: `python3-defaults=3.7.5-1ubuntu1`

Binary Packages:

- `libpython3-stdlib:amd64=3.7.5-1ubuntu1`
- `python3=3.7.5-1ubuntu1`
- `python3-minimal=3.7.5-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.7.5-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.7.5-1ubuntu1.dsc' python3-defaults_3.7.5-1ubuntu1.dsc 2904 SHA256:0360fdfae59d37d1e84a535a87ad2b14ecf87c7222a4e12c5efad16971b13ca5
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.7.5-1ubuntu1.tar.gz' python3-defaults_3.7.5-1ubuntu1.tar.gz 137547 SHA256:29c389b72268dbee16ae8527ee9b4d080580c5205416bab70b3c0e5c84beae0d
```

### `dpkg` source package: `python3-stdlib-extensions=3.8.0-1`

Binary Packages:

- `python3-distutils=3.8.0-1`
- `python3-lib2to3=3.8.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.8.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.0-1.dsc' python3-stdlib-extensions_3.8.0-1.dsc 2523 SHA256:3b3c79e49f713337cf3e30f8b67baa9dc4945f42e20f5ea695b9c7c1a486310a
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.0.orig.tar.xz' python3-stdlib-extensions_3.8.0.orig.tar.xz 1058456 SHA256:e4a158e0c1571a831c51cff2e785b9c06340b363756ffe9615593b11f63b2a3f
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.0-1.debian.tar.xz' python3-stdlib-extensions_3.8.0-1.debian.tar.xz 17240 SHA256:a132c69fab4afb8940c1fc10848edcc8382face3516bde7fe238e574cbe0c958
```

### `dpkg` source package: `python3.7=3.7.5-2`

Binary Packages:

- `libpython3.7-minimal:amd64=3.7.5-2`
- `libpython3.7-stdlib:amd64=3.7.5-2`
- `python3.7=3.7.5-2`
- `python3.7-minimal=3.7.5-2`

Licenses: (parsed from: `/usr/share/doc/libpython3.7-minimal/copyright`, `/usr/share/doc/libpython3.7-stdlib/copyright`, `/usr/share/doc/python3.7/copyright`, `/usr/share/doc/python3.7-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.7=3.7.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.7/python3.7_3.7.5-2.dsc' python3.7_3.7.5-2.dsc 3419 SHA256:617f1894c21928ba838322fc62fe24b2e8196de5ffa7a782a9d4d3c7b87edb63
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.7/python3.7_3.7.5.orig.tar.xz' python3.7_3.7.5.orig.tar.xz 17236432 SHA256:e85a76ea9f3d6c485ec1780fca4e500725a4a7bbc63c78ebc44170de9b619d94
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.7/python3.7_3.7.5-2.debian.tar.xz' python3.7_3.7.5-2.debian.tar.xz 210876 SHA256:33446fca4e260b6e846e05d48c07c55c16312dd152eae14eb235a6be7f44ec31
```

### `dpkg` source package: `readline=8.0-3`

Binary Packages:

- `libreadline-dev:amd64=8.0-3`
- `libreadline8:amd64=8.0-3`
- `readline-common=8.0-3`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-3.dsc' readline_8.0-3.dsc 2434 SHA256:c1a879cf7675fa5333a5ec4383e668a5f04b1d4b641f2a9e2150526678d94a0d
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0.orig.tar.gz' readline_8.0.orig.tar.gz 2975937 SHA256:e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-3.debian.tar.xz' readline_8.0-3.debian.tar.xz 29140 SHA256:8262f010dc55b79bbdf885d27252dbb695549c2da065f417af81462b6660e6fb
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2build1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2build1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build1.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build1.dsc 2439 SHA256:fd89213f2d41b00c212a411a945146c6b2e00fce1d1819a9ec380b0d91bd1077
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build1.debian.tar.xz 8216 SHA256:b256cc2aa96c9b99918052c4badfab0339ba95a852eab5ae37aa8b53c259efd2
```

### `dpkg` source package: `sed=4.7-1`

Binary Packages:

- `sed=4.7-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1.dsc' sed_4.7-1.dsc 1880 SHA256:dd0e8daed987929920f7729771f9c7a5b48d094923aaf686efd2ab19db776108
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7.orig.tar.xz' sed_4.7.orig.tar.xz 1298316 SHA256:2885768cd0a29ff8d58a6280a270ff161f6a3deb5690b2be6c49f46d4c67bd6a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1.debian.tar.xz' sed_4.7-1.debian.tar.xz 59824 SHA256:a2ab8d50807fd2242f86d6c6257399e790445ab6f8932f7f487d34361b4fc483
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sensible-utils/0.0.12/


### `dpkg` source package: `serf=1.3.9-7`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-7`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-7/


### `dpkg` source package: `shadow=1:4.5-1.1ubuntu4`

Binary Packages:

- `login=1:4.5-1.1ubuntu4`
- `passwd=1:4.5-1.1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.5-1.1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1.1ubuntu4.dsc' shadow_4.5-1.1ubuntu4.dsc 1761 SHA256:8fff4bad2a5512aebe79427ca3f9e42afbd6ff5efb1080df01ccfd2417697d2e
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA256:22b0952dc944b163e2370bb911b11ca275fc80ad024267cf21e496b28c23d500
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1.1ubuntu4.debian.tar.xz' shadow_4.5-1.1ubuntu4.debian.tar.xz 472436 SHA256:4eaa200a5d65a63bc53761be36ac0f2b972f8758fd47c405714875d14d37d0d4
```

### `dpkg` source package: `shared-mime-info=1.10-1`

Binary Packages:

- `shared-mime-info=1.10-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.10-1.dsc' shared-mime-info_1.10-1.dsc 2197 SHA256:49efdf90a3b97a58fbe8a5b241f721d89d43f03ad52dc8254a4642f12a20d641
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.10.orig.tar.xz' shared-mime-info_1.10.orig.tar.xz 616800 SHA256:c625a83b4838befc8cafcd54e3619946515d9e44d63d61c4adf7f5513ddfbebf
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.10-1.debian.tar.xz' shared-mime-info_1.10-1.debian.tar.xz 10020 SHA256:7b78639aeac9ba261bcccd572739c2cac813541a7ae7799e8e56de0df693295d
```

### `dpkg` source package: `six=1.12.0-2build1`

Binary Packages:

- `python-six=1.12.0-2build1`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.12.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.12.0-2build1.dsc' six_1.12.0-2build1.dsc 2375 SHA256:04473e77c157f7c85a28e6e478293418dce7d21b42d6347898eff49aac902c7e
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.12.0.orig.tar.gz' six_1.12.0.orig.tar.gz 32725 SHA256:d16a0141ec1a18405cd4ce8b4613101da75da0e9a7aec5bdd4fa804d0e0eba73
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.12.0-2build1.debian.tar.xz' six_1.12.0-2build1.debian.tar.xz 4192 SHA256:7e22ff8603fcd41a0f97030b0272ee79a237dcec9cd1e4c91c590c1a583984cc
```

### `dpkg` source package: `sqlite3=3.30.1-1ubuntu1`

Binary Packages:

- `libsqlite3-0:amd64=3.30.1-1ubuntu1`
- `libsqlite3-dev:amd64=3.30.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.30.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.30.1-1ubuntu1.dsc' sqlite3_3.30.1-1ubuntu1.dsc 2505 SHA256:5ecf906bdfc87b81d588396cce7c3572a8caaadd304c8d04936fa0c503de93c6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.30.1.orig-www.tar.xz' sqlite3_3.30.1.orig-www.tar.xz 5700856 SHA256:da1965166e3e9aac2cb1e3b5822945b639b78247599bf4cef361cadbc333d8e9
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.30.1.orig.tar.xz' sqlite3_3.30.1.orig.tar.xz 7044280 SHA256:20792693194546c8ae60906fdcda1cd2796d0b6e585e6e5bcf36146f2db2dd4e
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.30.1-1ubuntu1.debian.tar.xz' sqlite3_3.30.1-1ubuntu1.debian.tar.xz 20616 SHA256:7f76814b9050d39d52194c65853c8d2700928a8fbec8d35b11a175ce1700a09d
```

### `dpkg` source package: `subversion=1.13.0-1`

Binary Packages:

- `libsvn1:amd64=1.13.0-1`
- `subversion=1.13.0-1`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `AFL-3`
- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
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
$ apt-get source -qq --print-uris subversion=1.13.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.13.0-1.dsc' subversion_1.13.0-1.dsc 3642 SHA256:d8f4bc1d90b56e429158bdee1dfa083fcf8713de2a6524d5f91a48dee683bc8f
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.13.0.orig.tar.gz' subversion_1.13.0.orig.tar.gz 11544359 SHA256:daad440c03b8a86fcca804ea82217bb1902cfcae1b7d28c624143c58dcb96931
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.13.0.orig.tar.gz.asc' subversion_1.13.0.orig.tar.gz.asc 2954 SHA256:ed4f87b947b8172fcaa4c741d8ccc7929914b18cf1ccffc32b4f159fdee3070d
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.13.0-1.debian.tar.xz' subversion_1.13.0-1.debian.tar.xz 420392 SHA256:1a25d666bd2f302c4aa2e8c542b9c5b8decd681177d588ef4b6b4471d781e669
```

### `dpkg` source package: `systemd=243-3ubuntu1`

Binary Packages:

- `libsystemd0:amd64=243-3ubuntu1`
- `libudev1:amd64=243-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `sysvinit=2.96-1ubuntu1`

Binary Packages:

- `sysvinit-utils=2.96-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-1ubuntu1.dsc' sysvinit_2.96-1ubuntu1.dsc 2743 SHA256:deed20b4a2a2fc89879aefebd2242dc0e476493eb7ffd46b5952392648ce179d
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA256:2a2e26b72aa235a23ab1c8471005f890309ce1196c83fbc9413c57b9ab62b587
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA256:dfc184b95da12c8c888c8ae6b0f26fe8a23b07fbcdd240f6600a8a78b9439fa0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-1ubuntu1.debian.tar.xz' sysvinit_2.96-1ubuntu1.debian.tar.xz 128256 SHA256:a5b31e908c6189c3ce7c2a1d9802881bf677840f07dcea872aadb9cea1d5d9e6
```

### `dpkg` source package: `tar=1.30+dfsg-6`

Binary Packages:

- `tar=1.30+dfsg-6`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.30+dfsg-6
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-6.dsc' tar_1.30+dfsg-6.dsc 1995 SHA256:1515951c8a2fc9a43e822efd82d9043cdec4bec47ddca9e7f1311c73e6b00d0c
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA256:c02f3747ffe02017878303dde8b78e79cd220364c5e8048cf92320232e38912d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-6.debian.tar.xz' tar_1.30+dfsg-6.debian.tar.xz 22124 SHA256:b7caae6287992536353413e7a9b21301b29c32066bb6f36b7190074af9dd5c50
```

### `dpkg` source package: `tiff=4.1.0+git191117-1`

Binary Packages:

- `libtiff-dev:amd64=4.1.0+git191117-1`
- `libtiff5:amd64=4.1.0+git191117-1`
- `libtiffxx5:amd64=4.1.0+git191117-1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.1.0+git191117-1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117-1.dsc' tiff_4.1.0+git191117-1.dsc 2242 SHA256:719b2652bb6ac2bfe0cb6728cfdb267b320a8dc7c1250940ce567e022876b867
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117.orig.tar.xz' tiff_4.1.0+git191117.orig.tar.xz 1533524 SHA256:67e1d045e994adb7144b0cca228d70dd6d520aaf8c75c342064bc0fd601e6e42
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117-1.debian.tar.xz' tiff_4.1.0+git191117-1.debian.tar.xz 18896 SHA256:15bfa5a520c58b41a67b6ac211feae21159a02acd45965ceb1831a5fd06ebf33
```

### `dpkg` source package: `ubuntu-keyring=2018.09.18.1`

Binary Packages:

- `ubuntu-keyring=2018.09.18.1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2018.09.18.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1.dsc' ubuntu-keyring_2018.09.18.1.dsc 1471 SHA256:326b0cad35b291c233fa09f4ead078c80949080a017442455567207e0e57d4ea
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1.tar.gz' ubuntu-keyring_2018.09.18.1.tar.gz 34263 SHA256:4e8534bd70274b26d835808095b95b7ee5448f5f10234fb6ec39c92c8c155d33
```

### `dpkg` source package: `ucf=3.0038+nmu1`

Binary Packages:

- `ucf=3.0038+nmu1`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0038+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0038+nmu1.dsc' ucf_3.0038+nmu1.dsc 1420 SHA256:89b6f921a30e04a946f62e6996be7c16f2f7c383d20783cd4704b502c6d5b125
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0038+nmu1.tar.xz' ucf_3.0038+nmu1.tar.xz 65860 SHA256:d00bc3dd8d2f91317f52b5352fe129023c72babad55bc0dd4ece7b34183c7436
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

### `dpkg` source package: `utf8proc=2.4.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.4.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.4.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.4.0-1.dsc' utf8proc_2.4.0-1.dsc 2129 SHA256:b214c9cefb3acbd4011c2ce266e3640952e97e69acceca28f4e3226b7087d809
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.4.0.orig.tar.gz' utf8proc_2.4.0.orig.tar.gz 154936 SHA256:b2e5d547c1d94762a6d03a7e05cea46092aab68636460ff8648f1295e2cdfbd7
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.4.0-1.debian.tar.xz' utf8proc_2.4.0-1.debian.tar.xz 4508 SHA256:44ff1481d4156be9d843ac97496220fa495099d726908a982dbec43b056d7d20
```

### `dpkg` source package: `util-linux=2.34-0.1ubuntu2`

Binary Packages:

- `bsdutils=1:2.34-0.1ubuntu2`
- `fdisk=2.34-0.1ubuntu2`
- `libfdisk1:amd64=2.34-0.1ubuntu2`
- `libsmartcols1:amd64=2.34-0.1ubuntu2`
- `mount=2.34-0.1ubuntu2`
- `util-linux=2.34-0.1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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


### `dpkg` source package: `util-linux=2.34-0.1ubuntu4`

Binary Packages:

- `libblkid-dev:amd64=2.34-0.1ubuntu4`
- `libblkid1:amd64=2.34-0.1ubuntu4`
- `libmount-dev:amd64=2.34-0.1ubuntu4`
- `libmount1:amd64=2.34-0.1ubuntu4`
- `libuuid1:amd64=2.34-0.1ubuntu4`
- `uuid-dev:amd64=2.34-0.1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.34-0.1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu4.dsc' util-linux_2.34-0.1ubuntu4.dsc 4063 SHA256:008f382db9570a3412d20ec621bd9c5d4bc499201840d81e73b293c396597696
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34.orig.tar.xz' util-linux_2.34.orig.tar.xz 4974812 SHA256:743f9d0c7252b6db246b659c1e1ce0bd45d8d4508b4dfa427bbb4a3e9b9f62b5
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu4.debian.tar.xz' util-linux_2.34-0.1ubuntu4.debian.tar.xz 86132 SHA256:ea49c33a3636c36f6a0fde35ad2f8f1ac48117c868f0c16454dbdc4625f2f866
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

### `dpkg` source package: `xorg=1:7.7+19ubuntu12`

Binary Packages:

- `x11-common=1:7.7+19ubuntu12`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19ubuntu12
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu12.dsc' xorg_7.7+19ubuntu12.dsc 2082 SHA256:5b8d89f4998c599da4162f57d20e0a7e435bd379f76e5ec9054ad8308bf9605b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu12.tar.gz' xorg_7.7+19ubuntu12.tar.gz 298988 SHA256:60b9cec925987aa4b2e08fb914cc3843de878a6cc2b5a98890f9d5ac51ea0d6d
```

### `dpkg` source package: `xorgproto=2018.4-4`

Binary Packages:

- `x11proto-core-dev=2018.4-4`
- `x11proto-dev=2018.4-4`
- `x11proto-xext-dev=2018.4-4`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`, `/usr/share/doc/x11proto-xext-dev/copyright`)

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

### `dpkg` source package: `xtrans=1.3.5-1build1`

Binary Packages:

- `xtrans-dev=1.3.5-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xtrans=1.3.5-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5-1build1.dsc' xtrans_1.3.5-1build1.dsc 1966 SHA256:0827372b3889b0d9a9f79cc6cc9f453ee2190af57a8e8e995051525791c17223
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5.orig.tar.gz' xtrans_1.3.5.orig.tar.gz 227536 SHA256:b7a577c1b6c75030145e53b4793db9c88f9359ac49e7d771d4385d21b3e5945d
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5-1build1.diff.gz' xtrans_1.3.5-1build1.diff.gz 16003 SHA256:9cde9143cc720fcfbfbd40e5c4c555c3c51e47e5fc59d686bec5ed7ec3f7c097
```

### `dpkg` source package: `xz-utils=5.2.4-1`

Binary Packages:

- `liblzma-dev:amd64=5.2.4-1`
- `liblzma5:amd64=5.2.4-1`
- `xz-utils=5.2.4-1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1.dsc' xz-utils_5.2.4-1.dsc 2518 SHA256:b1572c4efb3c8ebf6f0e044b70e1e0451c919a99d3f80be03b624a54dd7ea593
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA256:9717ae363760dedf573dad241420c5fea86256b65bc21d2cf71b2b12f0544f4b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA256:88290c1deeaf674ae2a4821f4373fe0e4cc2a94199eae6dcc26df1e70cc15303
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1.debian.tar.xz' xz-utils_5.2.4-1.debian.tar.xz 135296 SHA256:d37b558444b76e88a69601df008cf1c0343c58cb7765b7bbb2099b0a19619361
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-1ubuntu3`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-1ubuntu3`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-1ubuntu3.dsc' zlib_1.2.11.dfsg-1ubuntu3.dsc 2814 SHA256:d8394f9e8f23ef65e1a980510b39b235e26c7bee8b963b45995e9154ea4e04de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.xz' zlib_1.2.11.dfsg.orig.tar.xz 287216 SHA256:881c8a90f488def83488aa91fd68563c023013a4b9b07a040f6da2727d76ad60
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-1ubuntu3.debian.tar.xz' zlib_1.2.11.dfsg-1ubuntu3.debian.tar.xz 31904 SHA256:01a43554ada70e4d987105f0e9bc7f73cea72eba4eae1079f91d8b7b2d2912a7
```
