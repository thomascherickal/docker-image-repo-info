# `buildpack-deps:eoan`

## Docker Metadata

- Image ID: `sha256:07746d98a6eb614ee458c45c77e2b1562ca9559fb1d95cd017292543b5dc64c4`
- Created: `2020-01-16T03:12:38.652462723Z`
- Virtual Size: ~ 677.05 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

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
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-4.dsc' acl_2.2.53-4.dsc 2330 SHA256:532eb4029659db74e6625adc2bd277144f33c92cb0603272d61693b069896a85
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-4.debian.tar.xz' acl_2.2.53-4.debian.tar.xz 18572 SHA256:3e6571adea4886a9549bdc2323d5c55ee8f7dafb6a204513111d5943d2776dd8
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

Source:

```console
$ apt-get source -qq --print-uris apt=1.9.4
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.9.4.dsc' apt_1.9.4.dsc 2744 SHA256:fef428ea8f433254dc126558c0e708a40d26402778c2cf7429fd8203cbf75728
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.9.4.tar.xz' apt_1.9.4.tar.xz 2170120 SHA256:85ae8d5beb44fa02ed88af32137f4c97e7a68e5d9ba4164eab515988105ba292
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-4.dsc' attr_2.4.48-4.dsc 2427 SHA256:e53c076f39f1be4186704c94bd32276fa4661a587c360d8da25a5c3abe40cb29
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-4.debian.tar.xz' attr_2.4.48-4.debian.tar.xz 22388 SHA256:a491d226fb3b47aa65997406009893a4cc0628e2ffffe0d411179652dfeb6935
```

### `dpkg` source package: `audit=1:2.8.5-2ubuntu1`

Binary Packages:

- `libaudit-common=1:2.8.5-2ubuntu1`
- `libaudit1:amd64=1:2.8.5-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.5-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-2ubuntu1.dsc' audit_2.8.5-2ubuntu1.dsc 2776 SHA256:5a01aad11ee54b369ec5ed23aac5bc9a14175e233a12c08b0d8c4c3143fbdd66
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5.orig.tar.gz' audit_2.8.5.orig.tar.gz 1140694 SHA256:0e5d4103646e00f8d1981e1cd2faea7a2ae28e854c31a803e907a383c5e2ecb7
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-2ubuntu1.debian.tar.xz' audit_2.8.5-2ubuntu1.debian.tar.xz 18500 SHA256:7f2d6ee41fed86f68410d6cce144b62e4a20f6f960128d7945e51d81a12382ba
```

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

### `dpkg` source package: `base-files=10.2ubuntu7.19.10.0`

Binary Packages:

- `base-files=10.2ubuntu7.19.10.0`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=10.2ubuntu7.19.10.0
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_10.2ubuntu7.19.10.0.dsc' base-files_10.2ubuntu7.19.10.0.dsc 1644 SHA256:ae6db5ad352b49788bfe1df9eced5df89e316975e5655312fa29703736563a86
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_10.2ubuntu7.19.10.0.tar.xz' base-files_10.2ubuntu7.19.10.0.tar.xz 78784 SHA256:252d0b65c1984d737b80056ed18f0e5b09ac63cfa2e936d8fe8d973b0f2c6521
```

### `dpkg` source package: `base-passwd=3.5.46`

Binary Packages:

- `base-passwd=3.5.46`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.46
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.46.dsc' base-passwd_3.5.46.dsc 1651 SHA256:98b5d79c9f06e05e9f41013f8fee48b08d0ffe398653b6f8bbd93c1ae1f24bd4
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.46.tar.xz' base-passwd_3.5.46.tar.xz 52780 SHA256:da15e380557b5a00cdc14018e3da6cbeaaadc786f2c3cb5b8f1fb4acc150b3da
```

### `dpkg` source package: `bash=5.0-4ubuntu1`

Binary Packages:

- `bash=5.0-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.0-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-4ubuntu1.dsc' bash_5.0-4ubuntu1.dsc 2447 SHA256:4f398f60ff0d21b0b4a03ee0e8bc95f9bb9b10cdba716d48f6c5c67184fc3976
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA256:893858ba233d65bda38039e99dd96a4102b2f6a2d5e6c1c546e0794a60beed97
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-4ubuntu1.debian.tar.xz' bash_5.0-4ubuntu1.debian.tar.xz 67512 SHA256:25c5b39768e4570b8f66252242e710cc4eb3f682d287f393dc982e40a6d91a75
```

### `dpkg` source package: `binutils=2.33-2ubuntu1.2`

Binary Packages:

- `binutils=2.33-2ubuntu1.2`
- `binutils-common:amd64=2.33-2ubuntu1.2`
- `binutils-x86-64-linux-gnu=2.33-2ubuntu1.2`
- `libbinutils:amd64=2.33-2ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.33-2ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.33-2ubuntu1.2.dsc' binutils_2.33-2ubuntu1.2.dsc 8594 SHA256:1dc2cca424dc944247c3c1e2429a5ae7aabd211d6006e2e79e6dd45f9d1b2731
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.33.orig.tar.xz' binutils_2.33.orig.tar.xz 21023972 SHA256:64f129a116ecb48a26e24565585936768aadf4002e245149d0dd6f62d898f056
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.33-2ubuntu1.2.debian.tar.xz' binutils_2.33-2ubuntu1.2.debian.tar.xz 106248 SHA256:50fd6f529ba1fb650b7bcd1ed1f9d09797cef5107ae81c8778659df4ec9124ab
```

### `dpkg` source package: `bzip2=1.0.6-9.2`

Binary Packages:

- `bzip2=1.0.6-9.2`
- `libbz2-1.0:amd64=1.0.6-9.2`
- `libbz2-dev:amd64=1.0.6-9.2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-9.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-9.2.dsc' bzip2_1.0.6-9.2.dsc 2348 SHA256:3b457bb9dabd0db4aec66727e69fe58aa12ec74c9c7980e8f08995a8428d1b5d
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-9.2.debian.tar.bz2' bzip2_1.0.6-9.2.debian.tar.bz2 27527 SHA256:070d9e3e6bf1e70b55fb60d4a155c9be30656d8cd0a38460b82e298ade6e2919
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

### `dpkg` source package: `cairo=1.16.0-4`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-4`
- `libcairo-script-interpreter2:amd64=1.16.0-4`
- `libcairo2:amd64=1.16.0-4`
- `libcairo2-dev:amd64=1.16.0-4`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-4.dsc' cairo_1.16.0-4.dsc 2806 SHA256:cd511a989ea189a15527f0b745196185df71dd3ab7396228cee0709d8b1c9616
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA256:5e7b29b3f113ef870d1e3ecf8adf21f923396401604bda16d44be45e66052331
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-4.debian.tar.xz' cairo_1.16.0-4.debian.tar.xz 30248 SHA256:e2b4c5aae085857e91de4529c00043997b55bb17ebccd3744bf04ac4ccfd31df
```

### `dpkg` source package: `cdebconf=0.249ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.249ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.249ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.249ubuntu1.dsc' cdebconf_0.249ubuntu1.dsc 2898 SHA256:10f32a31f8712256ec87496ff5262183bf81ad03e3d99fe9176020d273c68676
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.249ubuntu1.tar.xz' cdebconf_0.249ubuntu1.tar.xz 276400 SHA256:1f1ffc34409d244aa85689946a852b66418c844179c0e224a0d6cce1d6b9378a
```

### `dpkg` source package: `configobj=5.0.6-3`

Binary Packages:

- `python-configobj=5.0.6-3`

Licenses: (parsed from: `/usr/share/doc/python-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-3
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-3.dsc' configobj_5.0.6-3.dsc 2123 SHA256:bb0b6f41099734c9930109acd4473e84fcca47fadb14949710e5ff8032786299
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA256:2e140354efcca6f558ff9ee941b435ae09a617bc071797bef62c8d6ed2033d5e
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-3.debian.tar.xz' configobj_5.0.6-3.debian.tar.xz 6848 SHA256:8a278320a37b3953a5b372f12f9a6ef6f35b1680c9c7583062f4ab0b01106efc
```

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

### `dpkg` source package: `curl=7.65.3-1ubuntu3`

Binary Packages:

- `curl=7.65.3-1ubuntu3`
- `libcurl3-gnutls:amd64=7.65.3-1ubuntu3`
- `libcurl4:amd64=7.65.3-1ubuntu3`
- `libcurl4-openssl-dev:amd64=7.65.3-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.65.3-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.65.3-1ubuntu3.dsc' curl_7.65.3-1ubuntu3.dsc 2709 SHA256:cb62f24f9cda19bdcb719e5edcf92f64a6ed2b2fbe706b75585eeeb6fbfa6968
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.65.3.orig.tar.gz' curl_7.65.3.orig.tar.gz 4022334 SHA256:4376ac72b95572fb6c4fbffefb97c7ea0dd083e1974c0e44cd7e49396f454839
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.65.3-1ubuntu3.debian.tar.xz' curl_7.65.3-1ubuntu3.debian.tar.xz 30764 SHA256:4cc76896389aeda3f4a7d27edcc526cd9c944cd42c7d14fd7f95dd21973cf827
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-1build3`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-1build3`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-1build3`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-1build3.dsc' cyrus-sasl2_2.1.27+dfsg-1build3.dsc 3442 SHA256:6e467fd255e0a547c6de92592885e1838e2fbd751aa1c6dc513b5660b0beff99
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-1build3.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-1build3.debian.tar.xz 99772 SHA256:41f456759be1d32dbbc6f56d93460785bda9b534897e3dddc350ebcd5cc9d534
```

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

### `dpkg` source package: `debianutils=4.8.6.3`

Binary Packages:

- `debianutils=4.8.6.3`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.6.3
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.6.3.dsc' debianutils_4.8.6.3.dsc 1600 SHA256:c0b3a7483d606a9f866d64cf22bcc4d7d371b1821e9b9b63acb8f915e068ee0f
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.6.3.tar.xz' debianutils_4.8.6.3.tar.xz 156672 SHA256:2cc7de3afc6df1cf6d00af9938efac7ee8f739228e548e512ddc186b6a7be221
```

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

### `dpkg` source package: `djvulibre=3.5.27.1-13ubuntu0.1`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.27.1-13ubuntu0.1`
- `libdjvulibre-text=3.5.27.1-13ubuntu0.1`
- `libdjvulibre21:amd64=3.5.27.1-13ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-13ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-13ubuntu0.1.dsc' djvulibre_3.5.27.1-13ubuntu0.1.dsc 2500 SHA256:2b2d729869a0062e444b3f93c0338859b2e44d5db3aa6a53f7deb554cd5d25fb
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA256:77f07de3f1039aa19eba2eb3170d9ce9a0918ba7b704a59cfaf08f42fcc52144
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-13ubuntu0.1.debian.tar.xz' djvulibre_3.5.27.1-13ubuntu0.1.debian.tar.xz 76504 SHA256:0138dcb05dca644c7240c3cdab94b5e0aa715a975f1de3f38cd68100e5d9b77e
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

### `dpkg` source package: `expat=2.2.7-2`

Binary Packages:

- `libexpat1:amd64=2.2.7-2`
- `libexpat1-dev:amd64=2.2.7-2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.7-2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.7-2.dsc' expat_2.2.7-2.dsc 1949 SHA256:823f03964b62c0fd3d380e4001bc3aea35051cbcaf52d09ca19d5889b7bba1f8
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.7.orig.tar.gz' expat_2.2.7.orig.tar.gz 8278607 SHA256:4efe89dfd8c2f9b971bf9089efa4cc163ac997a75da92c08be14d80a091474e6
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.7-2.debian.tar.xz' expat_2.2.7-2.debian.tar.xz 12852 SHA256:9f427b1f23a95ded54f347d67dd527cb130b686bc190428dc95ed67a0100bc0a
```

### `dpkg` source package: `fftw3=3.3.8-2`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2.dsc' fftw3_3.3.8-2.dsc 2978 SHA256:b4367efbcc2bbbc44b62a9416a1c37764f5214628632553070c35893df786f68
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA256:6113262f6e92c5bd474f2875fa1b01054c4ad5040f6b0da7c03c98821d9ae303
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2.debian.tar.xz' fftw3_3.3.8-2.debian.tar.xz 13696 SHA256:684dede6b4124f309033d128dc7bdf1eb394984e6e8dd79e1fd5d73b95b12461
```

### `dpkg` source package: `file=1:5.37-5ubuntu0.1`

Binary Packages:

- `file=1:5.37-5ubuntu0.1`
- `libmagic-mgc=1:5.37-5ubuntu0.1`
- `libmagic1:amd64=1:5.37-5ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.37-5ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37-5ubuntu0.1.dsc' file_5.37-5ubuntu0.1.dsc 2329 SHA256:73276b2ea707bf62bae3624037d85dd577dd004e3e6c2c4375eabd496e1b980e
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37.orig.tar.gz' file_5.37.orig.tar.gz 887682 SHA256:e9c13967f7dd339a3c241b7710ba093560b9a33013491318e88e6b8b57bae07f
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37.orig.tar.gz.asc' file_5.37.orig.tar.gz.asc 169 SHA256:f73642d84908665dad226f247ae223e6bf52da8b2ca20ca88bd4e4966eef6bc7
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.37-5ubuntu0.1.debian.tar.xz' file_5.37-5ubuntu0.1.debian.tar.xz 37868 SHA256:bc4c913a5fb53914cb6ed1c15bd89956a1f1fb18e5770a4badd5c249609849d1
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

### `dpkg` source package: `freetype=2.9.1-4`

Binary Packages:

- `libfreetype6:amd64=2.9.1-4`
- `libfreetype6-dev:amd64=2.9.1-4`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

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
$ apt-get source -qq --print-uris freetype=2.9.1-4
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1-4.dsc' freetype_2.9.1-4.dsc 3663 SHA256:3338e9b56ef7e7557c1d00ee439dee089c5b918710ed00dbdc58f7b582946aa4
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1.orig-ft2demos.tar.gz' freetype_2.9.1.orig-ft2demos.tar.gz 294850 SHA256:3d440aad3481285c7455f1593577e375c9d5792c800bbaba68d46fd75130fab9
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1.orig-ft2demos.tar.gz.asc' freetype_2.9.1.orig-ft2demos.tar.gz.asc 359 SHA256:665b8357378dc715fbac964d05cdcc2a2f7fd1e9d7918a27bf50f4d0a17f0d30
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1.orig-ft2docs.tar.gz' freetype_2.9.1.orig-ft2docs.tar.gz 2123920 SHA256:f57c1297f5ad2ad4764f491317fa0f548bd307c4513185d4a0602412e83b1dc9
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1.orig-ft2docs.tar.gz.asc' freetype_2.9.1.orig-ft2docs.tar.gz.asc 359 SHA256:c4c674db43603f719018716970569d1722d0de46fa94757eb7f39266d72cdbd1
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1.orig.tar.gz' freetype_2.9.1.orig.tar.gz 2533956 SHA256:ec391504e55498adceb30baceebd147a6e963f636eb617424bcfc47a169898ce
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1.orig.tar.gz.asc' freetype_2.9.1.orig.tar.gz.asc 359 SHA256:2c2c5ae3b3838053b94366639e802b18bc4761003ea15ce73402d276baec424d
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.9.1-4.debian.tar.xz' freetype_2.9.1-4.debian.tar.xz 111992 SHA256:94311247da835d2b32e5e7a00e5db998e87e79a20948d9c526e44a17efa0e3af
```

### `dpkg` source package: `fribidi=1.0.5-3.1ubuntu0.19.10.1`

Binary Packages:

- `libfribidi0:amd64=1.0.5-3.1ubuntu0.19.10.1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.5-3.1ubuntu0.19.10.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.5-3.1ubuntu0.19.10.1.dsc' fribidi_1.0.5-3.1ubuntu0.19.10.1.dsc 2120 SHA256:c0a47ae5dd21413171519770ae298472c73c2ee0921ce81a1936bf85fdc19f39
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.5.orig.tar.bz2' fribidi_1.0.5.orig.tar.bz2 2082617 SHA256:6a64f2a687f5c4f203a46fa659f43dd43d1f8b845df8d723107e8a7e6158e4ce
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.5-3.1ubuntu0.19.10.1.debian.tar.xz' fribidi_1.0.5-3.1ubuntu0.19.10.1.debian.tar.xz 9756 SHA256:2fe1f6b51f404b0d69a16d7d074904605d0de2630ca7767c38299c4b24faa630
```

### `dpkg` source package: `gcc-9=9.2.1-9ubuntu2`

Binary Packages:

- `cpp-9=9.2.1-9ubuntu2`
- `g++-9=9.2.1-9ubuntu2`
- `gcc-9=9.2.1-9ubuntu2`
- `gcc-9-base:amd64=9.2.1-9ubuntu2`
- `libasan5:amd64=9.2.1-9ubuntu2`
- `libatomic1:amd64=9.2.1-9ubuntu2`
- `libcc1-0:amd64=9.2.1-9ubuntu2`
- `libgcc-9-dev:amd64=9.2.1-9ubuntu2`
- `libgcc1:amd64=1:9.2.1-9ubuntu2`
- `libgomp1:amd64=9.2.1-9ubuntu2`
- `libitm1:amd64=9.2.1-9ubuntu2`
- `liblsan0:amd64=9.2.1-9ubuntu2`
- `libquadmath0:amd64=9.2.1-9ubuntu2`
- `libstdc++-9-dev:amd64=9.2.1-9ubuntu2`
- `libstdc++6:amd64=9.2.1-9ubuntu2`
- `libtsan0:amd64=9.2.1-9ubuntu2`
- `libubsan1:amd64=9.2.1-9ubuntu2`

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
$ apt-get source -qq --print-uris gcc-9=9.2.1-9ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.2.1-9ubuntu2.dsc' gcc-9_9.2.1-9ubuntu2.dsc 37925 SHA256:2d40874d375df0ddf5e7c3750e5a018f31221973b536a3929f38b673ebbf04b8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.2.1.orig.tar.gz' gcc-9_9.2.1.orig.tar.gz 90195906 SHA256:8819e4bbae43592726be676262f81f242bc5b7a50a019012d8ef02d135a1280c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.2.1-9ubuntu2.debian.tar.xz' gcc-9_9.2.1-9ubuntu2.debian.tar.xz 539772 SHA256:2ce47d2e1eff6d67a1c7add883bb52442b92b5cbde2ec78dead5faf866188db6
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

### `dpkg` source package: `gdk-pixbuf=2.40.0+dfsg-1build1`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.40.0+dfsg-1build1`
- `libgdk-pixbuf2.0-0:amd64=2.40.0+dfsg-1build1`
- `libgdk-pixbuf2.0-bin=2.40.0+dfsg-1build1`
- `libgdk-pixbuf2.0-common=2.40.0+dfsg-1build1`
- `libgdk-pixbuf2.0-dev:amd64=2.40.0+dfsg-1build1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.40.0+dfsg-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-1build1.dsc' gdk-pixbuf_2.40.0+dfsg-1build1.dsc 2934 SHA256:9bba08384862bd10b759abf9210df27af64f4edec9ee9ea22e5827880acb364f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg.orig.tar.xz' gdk-pixbuf_2.40.0+dfsg.orig.tar.xz 5626144 SHA256:bdb3820005dc3c02ec8b1e2916a1d060f65f44d30ba48ab88704c3380d5a47b8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-1build1.debian.tar.xz' gdk-pixbuf_2.40.0+dfsg-1build1.debian.tar.xz 17080 SHA256:1116d82dc9eef0481dfdc84c4ec56a8b0884cb14048c8b0c3ecfdd85e0de48c9
```

### `dpkg` source package: `git=1:2.20.1-2ubuntu1.19.10.1`

Binary Packages:

- `git=1:2.20.1-2ubuntu1.19.10.1`
- `git-man=1:2.20.1-2ubuntu1.19.10.1`

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
$ apt-get source -qq --print-uris git=1:2.20.1-2ubuntu1.19.10.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.20.1-2ubuntu1.19.10.1.dsc' git_2.20.1-2ubuntu1.19.10.1.dsc 3001 SHA256:68db22c1636a3592fd61e3f80978449c68673d4a0fd146c09ed626b8a4ce2e92
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.20.1.orig.tar.xz' git_2.20.1.orig.tar.xz 5359872 SHA256:9d2e91e2faa2ea61ba0a70201d023b36f54d846314591a002c610ea2ab81c3e9
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.20.1-2ubuntu1.19.10.1.debian.tar.xz' git_2.20.1-2ubuntu1.19.10.1.debian.tar.xz 630736 SHA256:979a78e254017f5fdc12702f1c73bbca9f9e2f7b47848fb68c0bbf40aa31de32
```

### `dpkg` source package: `glib2.0=2.62.1-1`

Binary Packages:

- `libglib2.0-0:amd64=2.62.1-1`
- `libglib2.0-bin=2.62.1-1`
- `libglib2.0-data=2.62.1-1`
- `libglib2.0-dev:amd64=2.62.1-1`
- `libglib2.0-dev-bin=2.62.1-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.62.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.62.1-1.dsc' glib2.0_2.62.1-1.dsc 3232 SHA256:ca848af046b9f6d01562f7c2555feec2c06bbc063e49677a4c758af165c8badc
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.62.1.orig.tar.xz' glib2.0_2.62.1.orig.tar.xz 4681716 SHA256:3dd9024e1d0872a6da7ac509937ccf997161b11d7d35be337c7e829cbae0f9df
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.62.1-1.debian.tar.xz' glib2.0_2.62.1-1.debian.tar.xz 85312 SHA256:7aa788a4d805f0dc16eea9373811ba9b29bc4928d57575649389a3b83a1db2df
```

### `dpkg` source package: `glibc=2.30-0ubuntu2`

Binary Packages:

- `libc-bin=2.30-0ubuntu2`
- `libc-dev-bin=2.30-0ubuntu2`
- `libc6:amd64=2.30-0ubuntu2`
- `libc6-dev:amd64=2.30-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.30-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.30-0ubuntu2.dsc' glibc_2.30-0ubuntu2.dsc 9228 SHA256:7169347395cebf0d15c665d4f79c255efeadee71415e36bd5664219e7d8e9064
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.30.orig.tar.xz' glibc_2.30.orig.tar.xz 17080288 SHA256:88b5b39b80a4cb4d7b17bded91a2a9e99ff00190377321446f55d00a97611870
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.30-0ubuntu2.debian.tar.xz' glibc_2.30-0ubuntu2.debian.tar.xz 850068 SHA256:035f3384f32b7e39247d5e5ba273ed17036813c63088a1cd5a86eb6208a5fb40
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

### `dpkg` source package: `gnupg2=2.2.12-1ubuntu3`

Binary Packages:

- `dirmngr=2.2.12-1ubuntu3`
- `gnupg=2.2.12-1ubuntu3`
- `gnupg-l10n=2.2.12-1ubuntu3`
- `gnupg-utils=2.2.12-1ubuntu3`
- `gpg=2.2.12-1ubuntu3`
- `gpg-agent=2.2.12-1ubuntu3`
- `gpg-wks-client=2.2.12-1ubuntu3`
- `gpg-wks-server=2.2.12-1ubuntu3`
- `gpgconf=2.2.12-1ubuntu3`
- `gpgsm=2.2.12-1ubuntu3`
- `gpgv=2.2.12-1ubuntu3`

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
$ apt-get source -qq --print-uris gnupg2=2.2.12-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.12-1ubuntu3.dsc' gnupg2_2.2.12-1ubuntu3.dsc 3880 SHA256:6bcf404d549e251def8840a6461b7cbd71bd73d9bdcf9c52db0071974a3edc8f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.12.orig.tar.bz2' gnupg2_2.2.12.orig.tar.bz2 6682303 SHA256:db030f8b4c98640e91300d36d516f1f4f8fe09514a94ea9fc7411ee1a34082cb
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.12.orig.tar.bz2.asc' gnupg2_2.2.12.orig.tar.bz2.asc 3204 SHA256:97c8dc25c4c2fe9a39b2ffd81b65b6f3dc4ad359c9a81ca4bb9b4bdeb6167c60
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.12-1ubuntu3.debian.tar.xz' gnupg2_2.2.12-1ubuntu3.debian.tar.xz 65876 SHA256:d95527c25e4c4eb404b1b29096044235eab56b2f5e29a94d764c2063b31016fe
```

### `dpkg` source package: `gnutls28=3.6.9-5ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.6.9-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
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
$ apt-get source -qq --print-uris gnutls28=3.6.9-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.9-5ubuntu1.dsc' gnutls28_3.6.9-5ubuntu1.dsc 3515 SHA256:3990f1d4d72f1c962a27b7a9db64281e35a2421e7ee718f6e63e789f5a4d5928
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.9.orig.tar.xz' gnutls28_3.6.9.orig.tar.xz 5773928 SHA256:4331fca55817ecdd74450b908a6c29b4f05bb24dd13144c6284aa34d872e1fcb
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.9.orig.tar.xz.asc' gnutls28_3.6.9.orig.tar.xz.asc 488 SHA256:7956ffdddad8495f6933233b6ad04bb6b4e8ff9a2977fc0fd7ae95aa33ae245d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.9-5ubuntu1.debian.tar.xz' gnutls28_3.6.9-5ubuntu1.debian.tar.xz 70032 SHA256:9dc3c47c0837ab414873aa6b9ca2b5bd7cfa95d0af7ecebc3c44abd128944fba
```

### `dpkg` source package: `gobject-introspection=1.62.0-1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.62.0-1`
- `gir1.2-glib-2.0:amd64=1.62.0-1`
- `libgirepository-1.0-1:amd64=1.62.0-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.62.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.62.0-1.dsc' gobject-introspection_1.62.0-1.dsc 2873 SHA256:c4ea6565fca985fc404962661f492170bfaeee39f2b53f2da13ad584fce5856b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.62.0.orig.tar.xz' gobject-introspection_1.62.0.orig.tar.xz 980732 SHA256:b1ee7ed257fdbc008702bdff0ff3e78a660e7e602efa8f211dc89b9d1e7d90a2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.62.0-1.debian.tar.xz' gobject-introspection_1.62.0-1.debian.tar.xz 21684 SHA256:9dc2b21286517e1946a682e5a1db260d65ab005cb66746a7dc953aff69c37e06
```

### `dpkg` source package: `graphite2=1.3.13-8`

Binary Packages:

- `libgraphite2-3:amd64=1.3.13-8`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-2.1+ `
- `MPL-1.1`
- `custom-sil-open-font-license`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.13-8
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.13-8.dsc' graphite2_1.3.13-8.dsc 2574 SHA256:1826ab4dd7fc4054fb1d067a77945540406d3ad63be69779d8105c3a9d580b72
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.13.orig.tar.gz' graphite2_1.3.13.orig.tar.gz 6664941 SHA256:2f9f609deeddfe2b193502adc8df3b0396694b799a433c36e85fd1242e654cd9
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.13-8.debian.tar.xz' graphite2_1.3.13-8.debian.tar.xz 11948 SHA256:954259285b4f3f06f3ac6f8ed17312cb882aa044dd83a6946c53aa8b036b834d
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

### `dpkg` source package: `gzip=1.10-0ubuntu3.1`

Binary Packages:

- `gzip=1.10-0ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-0ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-0ubuntu3.1.dsc' gzip_1.10-0ubuntu3.1.dsc 2142 SHA256:04c4893f91149a98fdf657a83010d942859c519881c82a908e0fc967883c7ef4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA256:c91f74430bf7bc20402e1f657d0b252cb80aa66ba333a25704512af346633c68
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-0ubuntu3.1.debian.tar.xz' gzip_1.10-0ubuntu3.1.debian.tar.xz 26540 SHA256:56a14d90d897b271209c2fbe1478e42bf4e45b89bfd942ef56be76d24f9c7a4c
```

### `dpkg` source package: `harfbuzz=2.6.1-3`

Binary Packages:

- `libharfbuzz0b:amd64=2.6.1-3`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.6.1-3
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.1-3.dsc' harfbuzz_2.6.1-3.dsc 2434 SHA256:7c33bb0db60f69fa88722e5ab72a7f49ed49e1701ec160816a64587cef5da9a2
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.1.orig.tar.xz' harfbuzz_2.6.1.orig.tar.xz 5741372 SHA256:c651fb3faaa338aeb280726837c2384064cdc17ef40539228d88a1260960844f
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.1-3.debian.tar.xz' harfbuzz_2.6.1-3.debian.tar.xz 10724 SHA256:4bf3ab1ab3cc096f4e3d76684ff9a7b14bec7b9c01143f8dfcb3f706e649605a
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

### `dpkg` source package: `hostname=3.22`

Binary Packages:

- `hostname=3.22`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.22
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.22.dsc' hostname_3.22.dsc 1396 SHA256:778995b1edea78bb96c07ca916dd7a681f4d109582551db355738b421801efd4
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.22.tar.gz' hostname_3.22.tar.gz 13565 SHA256:b6d712d9e65687755e77b2451165bfd6ee72b4418300edfc4b718d347be256a4
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

### `dpkg` source package: `ilmbase=2.2.1-2ubuntu1`

Binary Packages:

- `libilmbase-dev=2.2.1-2ubuntu1`
- `libilmbase23:amd64=2.2.1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase23/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.2.1-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.1-2ubuntu1.dsc' ilmbase_2.2.1-2ubuntu1.dsc 2401 SHA256:bd4e4f6d751ce4fbb111e7eec1591c70b4e150e86b7adb3f8a24d96c7897e485
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.1.orig.tar.gz' ilmbase_2.2.1.orig.tar.gz 573073 SHA256:cac206e63be68136ef556c2b555df659f45098c159ce24804e9d5e9e0286609e
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.1.orig.tar.gz.asc' ilmbase_2.2.1.orig.tar.gz.asc 566 SHA256:81f3e8947b240ffcae9178574ca7ebadeffa6071f9d03f7810e624e9d0060df0
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.1-2ubuntu1.debian.tar.xz' ilmbase_2.2.1-2ubuntu1.debian.tar.xz 14108 SHA256:56af498f0567bc49745c224b09065a59777f600b576353a93bdf2fd1e687d36a
```

### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu3.1`

Binary Packages:

- `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `imagemagick-6.q16=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickcore-6-arch-config:amd64=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickcore-6-headers=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickcore-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickcore-dev=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickwand-6-headers=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickwand-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu3.1`
- `libmagickwand-dev=8:6.9.10.23+dfsg-2.1ubuntu3.1`

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.10.23+dfsg-2.1ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1ubuntu3.1.dsc' imagemagick_6.9.10.23+dfsg-2.1ubuntu3.1.dsc 5214 SHA256:80842ea414e8e0d74e37966b8f8982e890a4c421cb0628904ce10b86487c2a7d
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg.orig.tar.xz' imagemagick_6.9.10.23+dfsg.orig.tar.xz 9081188 SHA256:44249112b624f2cc315573fa96685e547da27ebb321432259290c407023c531e
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.10.23+dfsg-2.1ubuntu3.1.debian.tar.xz' imagemagick_6.9.10.23+dfsg-2.1ubuntu3.1.debian.tar.xz 240708 SHA256:a34d4ac482d5c50524f565c262973369a6bba32a5f20fa911e6ff71e413780d2
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

### `dpkg` source package: `isl=0.21-2`

Binary Packages:

- `libisl21:amd64=0.21-2`

Licenses: (parsed from: `/usr/share/doc/libisl21/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.21-2
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.21-2.dsc' isl_0.21-2.dsc 1846 SHA256:561e5a9234ff4f1dcab8f57b703ed8fc4a5aadbf3cc0a31ece57a00b4d65f7d5
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.21.orig.tar.xz' isl_0.21.orig.tar.xz 1621680 SHA256:777058852a3db9500954361e294881214f6ecd4b594c00da5eee974cd6a54960
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.21-2.debian.tar.xz' isl_0.21-2.debian.tar.xz 23724 SHA256:ca40ff6d2a6e80dabf018a6c249d9899866af20c30fb828d7194711d3e9cb9bd
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
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6-6.dsc' keyutils_1.6-6.dsc 2062 SHA256:1da6a0f50759b4eefe210e351558a854e28d312213d5528792af6938f106f183
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.orig.tar.bz2' keyutils_1.6.orig.tar.bz2 93973 SHA256:d3aef20cec0005c0fa6b4be40079885567473185b1a57b629b030e67942c7115
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6-6.debian.tar.xz' keyutils_1.6-6.debian.tar.xz 12828 SHA256:063876d3733337aad5e632b013bb8fd85bef85b2285ba7d6c8ab5ac7492ca245
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
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.dsc' libcap-ng_0.7.9-2.dsc 1912 SHA256:e787ebb86a7c9fdcfe429c20f2b17528d084917a34b5efc0022619e1e11572a4
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.debian.tar.xz' libcap-ng_0.7.9-2.debian.tar.xz 6220 SHA256:1ce4d5f7ee041b01f254e9d12ae86fef563566871bc457579c70b058b071ae22
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

### `dpkg` source package: `libedit=3.1-20190324-1`

Binary Packages:

- `libedit2:amd64=3.1-20190324-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20190324-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20190324-1.dsc' libedit_3.1-20190324-1.dsc 2129 SHA256:c4374f38990a3f5dba5da74a78602cd8e87c3c966c9fc2fb9b31aabc27dcff54
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20190324.orig.tar.gz' libedit_3.1-20190324.orig.tar.gz 521999 SHA256:ac8f0f51c1cf65492e4d1e3ed2be360bda41e54633444666422fbf393bba1bae
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20190324-1.debian.tar.xz' libedit_3.1-20190324-1.debian.tar.xz 14112 SHA256:b65610cc1c1e46144705b3627881ed51ffd91ddee349c47d30674f588d1b84b6
```

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

### `dpkg` source package: `libevent=2.1.8-stable-4build1`

Binary Packages:

- `libevent-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-core-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-dev=2.1.8-stable-4build1`
- `libevent-extra-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-openssl-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-pthreads-2.1-6:amd64=2.1.8-stable-4build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libevent=2.1.8-stable-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.8-stable-4build1.dsc' libevent_2.1.8-stable-4build1.dsc 2110 SHA256:50bb6f58ce43bfb8c0b5123bc9722167f79f71c13dcc053da0d38259a9862c4b
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.8-stable.orig.tar.gz' libevent_2.1.8-stable.orig.tar.gz 1026485 SHA256:965cc5a8bb46ce4199a47e9b2c9e1cae3b137e8356ffdad6d94d3b9069b71dc2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.8-stable-4build1.debian.tar.xz' libevent_2.1.8-stable-4build1.debian.tar.xz 12176 SHA256:bc2aaa2398fd296875ee522fbdc1ed146531cd1db9f49119f71d8cf257c51a97
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

### `dpkg` source package: `libgcrypt20=1.8.4-5ubuntu2.1`

Binary Packages:

- `libgcrypt20:amd64=1.8.4-5ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.4-5ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4-5ubuntu2.1.dsc' libgcrypt20_1.8.4-5ubuntu2.1.dsc 2915 SHA256:ff79b270d5b94a109d7104357848b077bc8067895b82c958c807926705a7aff9
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4.orig.tar.bz2' libgcrypt20_1.8.4.orig.tar.bz2 2990108 SHA256:f638143a0672628fde0cad745e9b14deb85dffb175709cacc1f4fe24b93f2227
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4.orig.tar.bz2.asc' libgcrypt20_1.8.4.orig.tar.bz2.asc 534 SHA256:97df94317ad273cffce4e78ad34ad0664819b44496f6528818a4298a691209a3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.4-5ubuntu2.1.debian.tar.xz' libgcrypt20_1.8.4-5ubuntu2.1.debian.tar.xz 31980 SHA256:23e0e8dab2003f6d9c14536b7c4fb55495a036af78e3f63818744031b0737d98
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
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.1.dsc' liblqr_0.4.2-2.1.dsc 2095 SHA256:c54c34cd2f7470a29366eeacde2ca4859a97d684a406fb81a918b970c01d617c
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA256:d4c22373432cca749e4326cd41fce365e6ff857c0bfd7a5302b8eb34b69f0336
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.1.debian.tar.xz' liblqr_0.4.2-2.1.debian.tar.xz 5300 SHA256:284a002f1ecac63ac17b1aafbb230da9ce7bd9efe2d5b94e8cad49b607eb2564
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

### `dpkg` source package: `librsvg=2.44.14-1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.44.14-1`
- `librsvg2-2:amd64=2.44.14-1`
- `librsvg2-common:amd64=2.44.14-1`
- `librsvg2-dev:amd64=2.44.14-1`

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
$ apt-get source -qq --print-uris librsvg=2.44.14-1
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.44.14-1.dsc' librsvg_2.44.14-1.dsc 2978 SHA256:f596544130f3f390c37e187649bb3122fbf78ef01b08e8220f917794a907fb72
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.44.14.orig.tar.xz' librsvg_2.44.14.orig.tar.xz 9898828 SHA256:d74564349548f91c863ad3c518dd059f63c2bd267be22dcada396efe83d07397
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.44.14-1.debian.tar.xz' librsvg_2.44.14-1.debian.tar.xz 23760 SHA256:3b5225976fb1e73a5f75113243ea3ed7339e525350e90de3c42873b140b814aa
```

### `dpkg` source package: `libseccomp=2.4.1-0ubuntu0.19.10.3`

Binary Packages:

- `libseccomp2:amd64=2.4.1-0ubuntu0.19.10.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.1-0ubuntu0.19.10.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.1-0ubuntu0.19.10.3.dsc' libseccomp_2.4.1-0ubuntu0.19.10.3.dsc 2580 SHA256:c8f4b886479df834b2a49254ed8595d44ab10d4842e35bc02123c5211e40ad7b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.1.orig.tar.gz' libseccomp_2.4.1.orig.tar.gz 606860 SHA256:1ca3735249af66a1b2f762fe6e710fcc294ad7185f1cc961e5bd83f9988006e8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.1-0ubuntu0.19.10.3.debian.tar.xz' libseccomp_2.4.1-0ubuntu0.19.10.3.debian.tar.xz 11164 SHA256:169a96e2234830b418544a450d7b5da8a5c075c95de2a2afc96e5cfc445a6943
```

### `dpkg` source package: `libselinux=2.9-2`

Binary Packages:

- `libselinux1:amd64=2.9-2`
- `libselinux1-dev:amd64=2.9-2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.9-2.dsc' libselinux_2.9-2.dsc 2347 SHA256:633fc2dfd8b6995f5f5f911020cbe098c355c7909a947f4be1fc6b2a75eeeb14
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.9.orig.tar.gz' libselinux_2.9.orig.tar.gz 211546 SHA256:1bccc8873e449587d9a2b2cf253de9b89a8291b9fbc7c59393ca9e5f5f4d2693
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.9-2.debian.tar.xz' libselinux_2.9-2.debian.tar.xz 23508 SHA256:6a41da2835650bad03d8123545470117b8e085537a4759a4c6e5c2df1211cba7
```

### `dpkg` source package: `libsemanage=2.9-3`

Binary Packages:

- `libsemanage-common=2.9-3`
- `libsemanage1:amd64=2.9-3`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.9-3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.9-3.dsc' libsemanage_2.9-3.dsc 2305 SHA256:9aa1a41fd7e7746e15fffa762344e76f4189d53f57a260a8190b4a287955f4cb
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.9.orig.tar.gz' libsemanage_2.9.orig.tar.gz 157690 SHA256:2576349d344492e73b468059767268dec1dabd8c35f3c7222c3ec2448737bc1c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.9-3.debian.tar.xz' libsemanage_2.9-3.debian.tar.xz 17208 SHA256:6d8f01aa874e8222be268d860eacc4f19cbdf6a1785db4fc9f229d6cf6d6401f
```

### `dpkg` source package: `libsepol=2.9-2`

Binary Packages:

- `libsepol1:amd64=2.9-2`
- `libsepol1-dev:amd64=2.9-2`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`, `/usr/share/doc/libsepol1-dev/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.9-2.dsc' libsepol_2.9-2.dsc 1792 SHA256:ce6ccf8445a11176f04116ce0c3a9e0bb1c14e4f7a5993a9e923b43fc8709848
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.9.orig.tar.gz' libsepol_2.9.orig.tar.gz 474861 SHA256:a34b12b038d121e3e459b1cbaca3c9202e983137819c16baf63658390e3f1d5d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.9-2.debian.tar.xz' libsepol_2.9-2.debian.tar.xz 14148 SHA256:ce6b6e7944669009c774826c363568ee32846847d999f081f4a16d36506c9b66
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

### `dpkg` source package: `libssh=0.9.0-1ubuntu1.3`

Binary Packages:

- `libssh-4:amd64=0.9.0-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.0-1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.0-1ubuntu1.3.dsc' libssh_0.9.0-1ubuntu1.3.dsc 2779 SHA256:c325283f9e4904fd6d909d0d28f371624f97fd09697656603003e64c1870dab1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.0.orig.tar.xz' libssh_0.9.0.orig.tar.xz 487628 SHA256:25303c2995e663cd169fdd902bae88106f48242d7e96311d74f812023482c7a5
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.0.orig.tar.xz.asc' libssh_0.9.0.orig.tar.xz.asc 833 SHA256:376c3d17bd252290b911903cae6a0bacae7864194224d5bf6f3a0073baf7b83a
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.0-1ubuntu1.3.debian.tar.xz' libssh_0.9.0-1ubuntu1.3.debian.tar.xz 37756 SHA256:0190581a542e68679606935a383161163c694cc5af1fbdb6f1a29edf6316e6b3
```

### `dpkg` source package: `libtasn1-6=4.14-3`

Binary Packages:

- `libtasn1-6:amd64=4.14-3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.14-3
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.14-3.dsc' libtasn1-6_4.14-3.dsc 2566 SHA256:ca49f23ccd5335d3fa7cb7471495ef2826de3b31b527e0207eb4ed42dfb34c43
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.14.orig.tar.gz' libtasn1-6_4.14.orig.tar.gz 1771184 SHA256:9e604ba5c5c8ea403487695c2e407405820d98540d9de884d6e844f9a9c5ba08
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.14.orig.tar.gz.asc' libtasn1-6_4.14.orig.tar.gz.asc 488 SHA256:9c11501a32c3a7da6fd148f2408619054975e38c31b0d2ca562e99477719dda0
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.14-3.debian.tar.xz' libtasn1-6_4.14-3.debian.tar.xz 18580 SHA256:80fb545c99bf1df5b298f172beb42f3e34220389f4d5306aa7026fb0a6a6eefb
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

### `dpkg` source package: `libwmf=0.2.8.4-15`

Binary Packages:

- `libwmf-dev=0.2.8.4-15`
- `libwmf0.2-7:amd64=0.2.8.4-15`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-15
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-15.dsc' libwmf_0.2.8.4-15.dsc 1955 SHA256:0abfd39f3637d7d41ca2a8e74b922d332f9078c28609ea9bf136be00c6860d2f
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-15.debian.tar.xz' libwmf_0.2.8.4-15.debian.tar.xz 12656 SHA256:4027eb1b7ea8bdd33ec8ec6be48275ded6cba895ccb79272b0f98211b26baeaa
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

### `dpkg` source package: `libxml2=2.9.4+dfsg1-7ubuntu3`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-7ubuntu3`
- `libxml2-dev:amd64=2.9.4+dfsg1-7ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.4+dfsg1-7ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-7ubuntu3.dsc' libxml2_2.9.4+dfsg1-7ubuntu3.dsc 3108 SHA256:1de9892ca18180db2ad5a9b3f6d8d6dddfc87f300c61642a652e824fc22d4fff
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA256:a74ad55e346aa0b2b41903e66d21f8f3d2a736b3f41e32496376861ab484184e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-7ubuntu3.debian.tar.xz' libxml2_2.9.4+dfsg1-7ubuntu3.debian.tar.xz 38980 SHA256:6c410c9992d08f552cda50f9349cd3607b3b5893052e806e7ffff182f8c4229b
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

### `dpkg` source package: `libxslt=1.1.33-0ubuntu1.1`

Binary Packages:

- `libxslt1-dev:amd64=1.1.33-0ubuntu1.1`
- `libxslt1.1:amd64=1.1.33-0ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.33-0ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.33-0ubuntu1.1.dsc' libxslt_1.1.33-0ubuntu1.1.dsc 2438 SHA256:b435fd92a4eff1ef99caf179e8e12f2fe6d2a63bc6d33d1f82e9786d903898d2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.33.orig.tar.gz' libxslt_1.1.33.orig.tar.gz 3444093 SHA256:8e36605144409df979cab43d835002f63988f3dc94d5d3537c12796db90e38c8
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.33-0ubuntu1.1.debian.tar.xz' libxslt_1.1.33-0ubuntu1.1.debian.tar.xz 34172 SHA256:f6cf29959be9db4df09c49e9bab5a87a8517d8d2b18db505613fafed18d3829d
```

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

### `dpkg` source package: `libyaml=0.2.1-1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.1-1`
- `libyaml-dev:amd64=0.2.1-1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.1-1.dsc' libyaml_0.2.1-1.dsc 1811 SHA256:916c8c0b5cdb7fce89fba618fa6b9ff9050d2647806b892dc8154668f8222361
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.1.orig.tar.gz' libyaml_0.2.1.orig.tar.gz 601443 SHA256:3ad5c55ec2cf72770e173d973d4120099ba0dec4d074097a488fa79de08304de
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.1-1.debian.tar.xz' libyaml_0.2.1-1.debian.tar.xz 4108 SHA256:4d6bedd7703ad9f43b9173fbd822f31b20d4c41f374257d6839b004f9742f152
```

### `dpkg` source package: `libzstd=1.4.3+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.4.3+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.3+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.3+dfsg-1.dsc' libzstd_1.4.3+dfsg-1.dsc 2285 SHA256:8b99efda28257570300dc9116340224861ccf3acdf49e223a9f861ba4d3d19ac
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.3+dfsg.orig.tar.xz' libzstd_1.4.3+dfsg.orig.tar.xz 1320940 SHA256:fb24c19891043b13d5225af41306789d65e16f6cd04176ca7410056bf0f13d0f
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.3+dfsg-1.debian.tar.xz' libzstd_1.4.3+dfsg-1.debian.tar.xz 16108 SHA256:3dbb5f5d3e6c4c0f43a5f6d6803327bf9c330efdb0b3da461613971af506796b
```

### `dpkg` source package: `linux=5.3.0-26.28`

Binary Packages:

- `linux-libc-dev:amd64=5.3.0-26.28`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lsb=11.0.1ubuntu1`

Binary Packages:

- `lsb-base=11.0.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.0.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.0.1ubuntu1.dsc' lsb_11.0.1ubuntu1.dsc 2174 SHA256:a772358ed1920895b81e96818007b69bba80513d0fb3ed64b3acfa7327c51309
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.0.1ubuntu1.tar.xz' lsb_11.0.1ubuntu1.tar.xz 46120 SHA256:affa99a0a76ebf4bc29b2afc405d190c8d84a25f130e390c869cae82a3c8e74e
```

### `dpkg` source package: `lz4=1.9.1-1`

Binary Packages:

- `liblz4-1:amd64=1.9.1-1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.1-1.dsc' lz4_1.9.1-1.dsc 1932 SHA256:113023de29767783a26e71558bd45d568f3d4c6555424401cdf4bebaaff75c51
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.1.orig.tar.gz' lz4_1.9.1.orig.tar.gz 285336 SHA256:f8377c89dad5c9f266edc0be9b73595296ecafd5bfa1000de148096c50052dc4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.1-1.debian.tar.xz' lz4_1.9.1-1.debian.tar.xz 11788 SHA256:ad397b6035183926ff40cd70dacac6c6b1acd7d93ec74633d41cd49427771b02
```

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

### `dpkg` source package: `m4=1.4.18-2`

Binary Packages:

- `m4=1.4.18-2`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-2.dsc' m4_1.4.18-2.dsc 1426 SHA256:93dda06744f90619c4666515c9b5bc51aa584519c16cafd1e74aaa3733628c1b
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-2.debian.tar.xz' m4_1.4.18-2.debian.tar.xz 17032 SHA256:73718bae96a2f63f0ed38c614ea081074914698207e73450da571461af1c58ec
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

Source:

```console
$ apt-get source -qq --print-uris mercurial=4.8.2-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.8.2-1ubuntu4.dsc' mercurial_4.8.2-1ubuntu4.dsc 2745 SHA256:9433f69ec5bd1bc98b1b0319b976028b7b4c2ac3bef1d6367ca627d8d1f5d85d
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.8.2.orig.tar.gz' mercurial_4.8.2.orig.tar.gz 6870985 SHA256:6c202cb9cf05e63b86477ebf84d6475eb10b4022ac2cd3a7481fb36d9c45fdb2
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.8.2.orig.tar.gz.asc' mercurial_4.8.2.orig.tar.gz.asc 833 SHA256:ceaf75242740acfd06a96aae53d8a40f3b3f3c4a7119bb53224d0bf6efa65254
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.8.2-1ubuntu4.debian.tar.xz' mercurial_4.8.2-1ubuntu4.debian.tar.xz 66296 SHA256:f55665ce2a6c03eeb3de757826f07aacac41236bb4a457643092e279022dc398
```

### `dpkg` source package: `mime-support=3.63ubuntu1`

Binary Packages:

- `mime-support=3.63ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.63ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.63ubuntu1.dsc' mime-support_3.63ubuntu1.dsc 1720 SHA256:eb8205c6a082e9c48d0fa3ce071143671de07d856a7117e14a352a592aa3edc7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.63ubuntu1.tar.gz' mime-support_3.63ubuntu1.tar.gz 38137 SHA256:6cadcebd8ca2f93522c572b2184e7cf470a87921d310a375e1eb95fe70d690e3
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

### `dpkg` source package: `mysql-8.0=8.0.18-0ubuntu0.19.10.1`

Binary Packages:

- `libmysqlclient-dev=8.0.18-0ubuntu0.19.10.1`
- `libmysqlclient21:amd64=8.0.18-0ubuntu0.19.10.1`

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

### `dpkg` source package: `ncurses=6.1+20190803-1ubuntu1`

Binary Packages:

- `libncurses-dev:amd64=6.1+20190803-1ubuntu1`
- `libncurses5-dev:amd64=6.1+20190803-1ubuntu1`
- `libncurses6:amd64=6.1+20190803-1ubuntu1`
- `libncursesw5-dev:amd64=6.1+20190803-1ubuntu1`
- `libncursesw6:amd64=6.1+20190803-1ubuntu1`
- `libtinfo6:amd64=6.1+20190803-1ubuntu1`
- `ncurses-base=6.1+20190803-1ubuntu1`
- `ncurses-bin=6.1+20190803-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1+20190803-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20190803-1ubuntu1.dsc' ncurses_6.1+20190803-1ubuntu1.dsc 4443 SHA256:159cbeb6bbe2893d8bb3334b4c9dc8733ce4ee408a9ba6c85809900797c8533f
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20190803.orig.tar.gz' ncurses_6.1+20190803.orig.tar.gz 3455081 SHA256:48731a430fd3978102ea18a33f2529c22e0e3870b0fadf0fd76526069a3ed003
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20190803.orig.tar.gz.asc' ncurses_6.1+20190803.orig.tar.gz.asc 265 SHA256:fcec4e09cbdaf0728de8d68d7c5f8a771eb287088374218c5182d6807627c2a2
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1+20190803-1ubuntu1.debian.tar.xz' ncurses_6.1+20190803-1ubuntu1.debian.tar.xz 63220 SHA256:ed88ae3306f8c5dafa660f4002e05c9da76e2894b6413fefb037d51e8c0af1ae
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
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.1-1.dsc' nettle_3.4.1-1.dsc 2258 SHA256:829d6f504938a22a704042211fe351f2e27c52d3811f42c508e95421a9c634fb
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.1.orig.tar.gz' nettle_3.4.1.orig.tar.gz 1947053 SHA256:f941cf1535cd5d1819be5ccae5babef01f6db611f9b5a777bae9c7604b8a92ad
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.1.orig.tar.gz.asc' nettle_3.4.1.orig.tar.gz.asc 2476 SHA256:07b265366b46bc67950da3f34687235eaa85c45b326e42bb7c9b58830b651d28
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.1-1.debian.tar.xz' nettle_3.4.1-1.debian.tar.xz 19988 SHA256:0339933966853cc0c3b2a9721f44116ee31d136d9983d33275d1beb291c11edb
```

### `dpkg` source package: `nghttp2=1.39.2-1`

Binary Packages:

- `libnghttp2-14:amd64=1.39.2-1`

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
$ apt-get source -qq --print-uris nghttp2=1.39.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.39.2-1.dsc' nghttp2_1.39.2-1.dsc 2548 SHA256:2703b5c0cc8d92997f4b250297eeaff4b76aca7267d6d1cca6631a525559d55b
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.39.2.orig.tar.bz2' nghttp2_1.39.2.orig.tar.bz2 2002397 SHA256:92a23e4522328c8565028ee0c7270e74add7990614fd1148f2a79d873bc2a1d0
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.39.2-1.debian.tar.xz' nghttp2_1.39.2-1.debian.tar.xz 12600 SHA256:30493844780721041ab46ee4c951b9841ba8a0df3692340d540f116897a3bcfa
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

### `dpkg` source package: `openexr=2.2.1-4.1ubuntu1`

Binary Packages:

- `libopenexr-dev=2.2.1-4.1ubuntu1`
- `libopenexr23:amd64=2.2.1-4.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr23/copyright`)

- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.2.1-4.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.1-4.1ubuntu1.dsc' openexr_2.2.1-4.1ubuntu1.dsc 2377 SHA256:b85994b01154c6af482ab06c7dba782395c29fc830c68810c39dd95992bb6466
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.1.orig.tar.gz' openexr_2.2.1.orig.tar.gz 18176639 SHA256:8f9a5af6131583404261931d9a5c83de0a425cb4b8b25ddab2b169fbf113aecd
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.1-4.1ubuntu1.debian.tar.xz' openexr_2.2.1-4.1ubuntu1.debian.tar.xz 22508 SHA256:ec4517647154f86430af15e101537d4d06eea71bc6918f0d6f7bf95fddfbce81
```

### `dpkg` source package: `openldap=2.4.48+dfsg-1ubuntu1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.48+dfsg-1ubuntu1`
- `libldap-common=2.4.48+dfsg-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.48+dfsg-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.48+dfsg-1ubuntu1.dsc' openldap_2.4.48+dfsg-1ubuntu1.dsc 2986 SHA256:55f8393e57088acd89438cfa66e19af919edc867c8ee462d4c6132cb597a2916
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.48+dfsg.orig.tar.gz' openldap_2.4.48+dfsg.orig.tar.gz 4875429 SHA256:8645601c28f094b01baed02a604479b175a45ba010e407212d214313bc6a80ba
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.48+dfsg-1ubuntu1.debian.tar.xz' openldap_2.4.48+dfsg-1ubuntu1.debian.tar.xz 179116 SHA256:ead23f7be35e1c9e29842b6cdd05f9109c152a48d05d6d25b338d7489b747604
```

### `dpkg` source package: `openssh=1:8.0p1-6build1`

Binary Packages:

- `openssh-client=1:8.0p1-6build1`

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
$ apt-get source -qq --print-uris openssh=1:8.0p1-6build1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.0p1-6build1.dsc' openssh_8.0p1-6build1.dsc 3262 SHA256:719e2697e4ad96fb123e137e1f4668f33ae46675ff021cbf6db98f3f82a5e178
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.0p1.orig.tar.gz' openssh_8.0p1.orig.tar.gz 1597697 SHA256:bd943879e69498e8031eb6b7f44d08cdc37d59a7ab689aa0b437320c3481fd68
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.0p1.orig.tar.gz.asc' openssh_8.0p1.orig.tar.gz.asc 683 SHA256:1904abaa20c24f0c8fed8d7708ec13f4ddca0b8f0f3a191b183b93f142111538
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.0p1-6build1.debian.tar.xz' openssh_8.0p1-6build1.debian.tar.xz 171480 SHA256:7263a0da2bf0c398ac3769c8ab7d02808b8c139a733580454cd6fdfb9b8391d5
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

### `dpkg` source package: `p11-kit=0.23.17-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.17-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.17-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.17-2.dsc' p11-kit_0.23.17-2.dsc 2420 SHA256:1070305d8d8ab29ee5b530b1f04350439e8a55528a19b952fca3e6cf588a2cef
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.17.orig.tar.gz' p11-kit_0.23.17.orig.tar.gz 1278291 SHA256:5447b25d66c05f86cce5bc8856f7a074be84c186730e32c74069ca03386d7c1e
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.17.orig.tar.gz.asc' p11-kit_0.23.17.orig.tar.gz.asc 854 SHA256:1f52278558aca72aa433bf8430fb6a93b1cd1c345c34d954bffb64453c486f03
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.17-2.debian.tar.xz' p11-kit_0.23.17-2.debian.tar.xz 21676 SHA256:069dde62ee1917be5fb8dca316c00c1c27e1686ef6b1cc30028a68733ab40136
```

### `dpkg` source package: `pam=1.3.1-5ubuntu1.19.10.0`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu1.19.10.0`
- `libpam-modules-bin=1.3.1-5ubuntu1.19.10.0`
- `libpam-runtime=1.3.1-5ubuntu1.19.10.0`
- `libpam0g:amd64=1.3.1-5ubuntu1.19.10.0`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu1.19.10.0
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu1.19.10.0.dsc' pam_1.3.1-5ubuntu1.19.10.0.dsc 2731 SHA256:7e6f0d1b40d6b741adc020d13e629d2972555582c72892a4e7ff0f0db992fca0
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA256:eff47a4ecd833fbf18de9686632a70ee8d0794b79aecb217ebd0ce11db4cd0db
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu1.19.10.0.debian.tar.xz' pam_1.3.1-5ubuntu1.19.10.0.debian.tar.xz 159316 SHA256:7363b23a0088634f1562b16434cdd99074e951a886a3c25c72a3edcc34c2a622
```

### `dpkg` source package: `pango1.0=1.42.4-7`

Binary Packages:

- `libpango-1.0-0:amd64=1.42.4-7`
- `libpangocairo-1.0-0:amd64=1.42.4-7`
- `libpangoft2-1.0-0:amd64=1.42.4-7`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Example`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.42.4-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.42.4-7.dsc' pango1.0_1.42.4-7.dsc 3409 SHA256:93b67c2a98f7578917ff62f4a6ec25070b93ad4fee6d24d40664b7d59ce9ae8a
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.42.4.orig.tar.xz' pango1.0_1.42.4.orig.tar.xz 833876 SHA256:1d2b74cd63e8bd41961f2f8d952355aa0f9be6002b52c8aa7699d9f5da597c9d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.42.4-7.debian.tar.xz' pango1.0_1.42.4-7.debian.tar.xz 50436 SHA256:2249c275e24cb56fcd527eedfbd959d68bac06d85dde1bc41d90a05941db50d5
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

### `dpkg` source package: `pcre2=10.32-5`

Binary Packages:

- `libpcre2-16-0:amd64=10.32-5`
- `libpcre2-32-0:amd64=10.32-5`
- `libpcre2-8-0:amd64=10.32-5`
- `libpcre2-dev:amd64=10.32-5`
- `libpcre2-posix0:amd64=10.32-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.32-5
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.32-5.dsc' pcre2_10.32-5.dsc 2342 SHA256:df327f59608e018603b138cf5a557fe5febfa5f24281152d68f3a52ba542d504
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.32.orig.tar.gz' pcre2_10.32.orig.tar.gz 2169349 SHA256:9ca9be72e1a04f22be308323caa8c06ebd0c51efe99ee11278186cafbc4fe3af
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.32-5.diff.gz' pcre2_10.32-5.diff.gz 5187 SHA256:bfe23d2661bf5727a10a1c1e49660c35afc0a4ad1c151bdcefb7c5a52e71e685
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

### `dpkg` source package: `perl=5.28.1-6build1`

Binary Packages:

- `libperl5.28:amd64=5.28.1-6build1`
- `perl=5.28.1-6build1`
- `perl-base=5.28.1-6build1`
- `perl-modules-5.28=5.28.1-6build1`

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
$ apt-get source -qq --print-uris perl=5.28.1-6build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.28.1-6build1.dsc' perl_5.28.1-6build1.dsc 2859 SHA256:b7b93110a83e897c5374c8bf20a3053d6f5249f4581d8ac2ff6bb699ef8201ce
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.28.1.orig-regen-configure.tar.xz' perl_5.28.1.orig-regen-configure.tar.xz 411944 SHA256:5873b81af4514d3910ab1a8267b15ff8c0e2100dbae4edfd10b65ef72cd31ef8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.28.1.orig.tar.xz' perl_5.28.1.orig.tar.xz 12372080 SHA256:fea7162d4cca940a387f0587b93f6737d884bf74d8a9d7cfd978bc12cd0b202d
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.28.1-6build1.debian.tar.xz' perl_5.28.1-6build1.debian.tar.xz 178696 SHA256:f3fe992ad2851db9dce01a3565514e5a2aae482a3e5f218a24301dc646944211
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

### `dpkg` source package: `postgresql-11=11.5-1`

Binary Packages:

- `libpq-dev=11.5-1`
- `libpq5:amd64=11.5-1`

Licenses: (parsed from: `/usr/share/doc/libpq-dev/copyright`, `/usr/share/doc/libpq5/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-clause`
- `Custom-Unicode`
- `Custom-pg_dump`
- `Custom-regex`
- `GPL-1`
- `PostgreSQL`
- `Snowball`
- `Tcl`
- `blf`
- `double-metaphone`
- `imath`
- `nagaysau-ishii`
- `rijndael`

Source:

```console
$ apt-get source -qq --print-uris postgresql-11=11.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-11/postgresql-11_11.5-1.dsc' postgresql-11_11.5-1.dsc 3716 SHA256:343b95f2950f93a02505eac1a89b0ca7c043b151980b85e088b01e0e7528e476
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-11/postgresql-11_11.5.orig.tar.bz2' postgresql-11_11.5.orig.tar.bz2 19773087 SHA256:7fdf23060bfc715144cbf2696cf05b0fa284ad3eb21f0c378591c6bca99ad180
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-11/postgresql-11_11.5-1.debian.tar.xz' postgresql-11_11.5-1.debian.tar.xz 25384 SHA256:72efa53767d9cc353c75bfad6b63ad1e1af7bda9b960aa6cc4ab5c5708cb51c2
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

### `dpkg` source package: `python2.7=2.7.17-1~19.10`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.17-1~19.10`
- `libpython2.7-stdlib:amd64=2.7.17-1~19.10`
- `python2.7=2.7.17-1~19.10`
- `python2.7-minimal=2.7.17-1~19.10`

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
$ apt-get source -qq --print-uris python2.7=2.7.17-1~19.10
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.17-1~19.10.dsc' python2.7_2.7.17-1~19.10.dsc 3388 SHA256:361c555a9675e56102f19dcedcd214272a0626d4a610284e6b2b51b240f2984f
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.17.orig.tar.gz' python2.7_2.7.17.orig.tar.gz 17535962 SHA256:f22059d09cdf9625e0a7284d24a13062044f5bf59d93a7f3382190dfa94cecde
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.17-1~19.10.diff.gz' python2.7_2.7.17-1~19.10.diff.gz 287075 SHA256:88acb5eb9430877dcb9337ee224eb6c3cf84932d9f0872f7da0f7f1157d59bb0
```

### `dpkg` source package: `python3-defaults=3.7.5-1`

Binary Packages:

- `libpython3-stdlib:amd64=3.7.5-1`
- `python3=3.7.5-1`
- `python3-minimal=3.7.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.7.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.7.5-1.dsc' python3-defaults_3.7.5-1.dsc 2801 SHA256:46429104fb8a1dfde14258010723b3cf843ae1f836e24d7d18abb79491bdf3e0
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.7.5-1.tar.gz' python3-defaults_3.7.5-1.tar.gz 137429 SHA256:7cdf04f1ac1dbbca89c45d9f7922b6b2049f879fad06dbad39278cac478117a2
```

### `dpkg` source package: `python3-stdlib-extensions=3.7.5-1build1`

Binary Packages:

- `python3-distutils=3.7.5-1build1`
- `python3-lib2to3=3.7.5-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.7.5-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.7.5-1build1.dsc' python3-stdlib-extensions_3.7.5-1build1.dsc 2563 SHA256:87242f5fd50eae5b5a31004def3b5f60e7d5421bddd5a1d0528547c6eb4e3cd0
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.7.5.orig.tar.xz' python3-stdlib-extensions_3.7.5.orig.tar.xz 1058456 SHA256:e4a158e0c1571a831c51cff2e785b9c06340b363756ffe9615593b11f63b2a3f
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.7.5-1build1.debian.tar.xz' python3-stdlib-extensions_3.7.5-1build1.debian.tar.xz 17260 SHA256:e3e5da632a94f45ac802c358fbc6130e2ef0035755263d3046f343b6e087e910
```

### `dpkg` source package: `python3.7=3.7.5-2~19.10`

Binary Packages:

- `libpython3.7-minimal:amd64=3.7.5-2~19.10`
- `libpython3.7-stdlib:amd64=3.7.5-2~19.10`
- `python3.7=3.7.5-2~19.10`
- `python3.7-minimal=3.7.5-2~19.10`

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
$ apt-get source -qq --print-uris python3.7=3.7.5-2~19.10
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.7/python3.7_3.7.5-2~19.10.dsc' python3.7_3.7.5-2~19.10.dsc 3443 SHA256:108d01fba4b18b7545216952ab129d326e32b9e0595b935acd1f00c8daeb9ee3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.7/python3.7_3.7.5.orig.tar.xz' python3.7_3.7.5.orig.tar.xz 17236432 SHA256:e85a76ea9f3d6c485ec1780fca4e500725a4a7bbc63c78ebc44170de9b619d94
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.7/python3.7_3.7.5-2~19.10.debian.tar.xz' python3.7_3.7.5-2~19.10.debian.tar.xz 210968 SHA256:5b50a0c7e838073577e67ce4ca8fde136148e2c26832a747f1afb38acd0a6848
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

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc 2299 SHA256:a296819cd2ab5880b67ad963ef0867cb10e462f4403e52565aa863eb05bb1370
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz 8096 SHA256:26d47de07d16285e4ca55b0828cbbf1ba35e671f9b3500a87e301fe755d26882
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

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.12
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.dsc' sensible-utils_0.0.12.dsc 1732 SHA256:1b62cc5f7561b3f5692a6edaec942e2e97e8368dabff8c865867d428eecb1221
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.tar.xz' sensible-utils_0.0.12.tar.xz 62152 SHA256:99ba2ebf8c57447c69d426b99b84ff9dc817be0bc4988ec6890a14558c529e2e
```

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

### `dpkg` source package: `six=1.12.0-2`

Binary Packages:

- `python-six=1.12.0-2`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.12.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.12.0-2.dsc' six_1.12.0-2.dsc 2436 SHA256:42f95777eadbbc20053248000023095321ee46f1144b450dd52add27120b58c8
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.12.0.orig.tar.gz' six_1.12.0.orig.tar.gz 32725 SHA256:d16a0141ec1a18405cd4ce8b4613101da75da0e9a7aec5bdd4fa804d0e0eba73
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.12.0-2.debian.tar.xz' six_1.12.0-2.debian.tar.xz 4108 SHA256:ace3c66ad66f5e8d2898b6ae7a233c19f6b9a37041302f022ecf86c3b3feb1b9
```

### `dpkg` source package: `sqlite3=3.29.0-2ubuntu0.1`

Binary Packages:

- `libsqlite3-0:amd64=3.29.0-2ubuntu0.1`
- `libsqlite3-dev:amd64=3.29.0-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.29.0-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.29.0-2ubuntu0.1.dsc' sqlite3_3.29.0-2ubuntu0.1.dsc 2497 SHA256:301390f6cacf8b9c36573634ce67176510ae846d10053f5a1a304685a98e0a44
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.29.0.orig-www.tar.xz' sqlite3_3.29.0.orig-www.tar.xz 5653816 SHA256:879d852db191f0a9ce0c65cc701e0a1eb6ed232eb112deb64c4288f17ded3a29
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.29.0.orig.tar.xz' sqlite3_3.29.0.orig.tar.xz 7004564 SHA256:b0c904b6b04cd377f949e07561df6068614d1eb66a6abb99157750638f9e69c2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.29.0-2ubuntu0.1.debian.tar.xz' sqlite3_3.29.0-2ubuntu0.1.debian.tar.xz 20912 SHA256:bcbba7668811d7bf8ce078a3c3f577d35df76d916f841830c4e13b639e2984ae
```

### `dpkg` source package: `subversion=1.10.6-1`

Binary Packages:

- `libsvn1:amd64=1.10.6-1`
- `subversion=1.10.6-1`

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
$ apt-get source -qq --print-uris subversion=1.10.6-1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.10.6-1.dsc' subversion_1.10.6-1.dsc 3582 SHA256:5b9cc96ff8ea7d375826b154240f2f05378d93a4f4dac1e21dde6eb52c6b1751
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.10.6.orig.tar.gz' subversion_1.10.6.orig.tar.gz 11352043 SHA256:2ab75c61a62d96defc954b599585b79f627e4e235094a17da94dc55b564727c1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.10.6.orig.tar.gz.asc' subversion_1.10.6.orig.tar.gz.asc 2121 SHA256:f485e3ffbe9b2ab287a813cb765904f41e0a499a9552f00c41a00a3169c4d418
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.10.6-1.debian.tar.xz' subversion_1.10.6-1.debian.tar.xz 435188 SHA256:7b1736185763d66d1495a92b893c64be2bd9ef7794a6e94d2b8794cbedc239ad
```

### `dpkg` source package: `systemd=242-7ubuntu3.2`

Binary Packages:

- `libsystemd0:amd64=242-7ubuntu3.2`
- `libudev1:amd64=242-7ubuntu3.2`

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
$ apt-get source -qq --print-uris systemd=242-7ubuntu3.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_242-7ubuntu3.2.dsc' systemd_242-7ubuntu3.2.dsc 5163 SHA256:473a242f1acf2f8998c40de5b6d80c99d1147b067cf7c20ec4eefe3dfcc09f74
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_242.orig.tar.gz' systemd_242.orig.tar.gz 7831435 SHA256:ec22be9a5dd94c9640e6348ed8391d1499af8ca2c2f01109198a414cff6c6cba
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_242-7ubuntu3.2.debian.tar.xz' systemd_242-7ubuntu3.2.debian.tar.xz 198996 SHA256:40d5c61cf19dae649f88e24ad49017a476cd71356a1277fbf0ee6b133cce7425
```

### `dpkg` source package: `sysvinit=2.95-5ubuntu2`

Binary Packages:

- `sysvinit-utils=2.95-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.95-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.95-5ubuntu2.dsc' sysvinit_2.95-5ubuntu2.dsc 2778 SHA256:a8f9cd28ecb0306b85754e020fba7ce438442bc4ee30450cc3a0fd44f07a8a05
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.95.orig.tar.xz' sysvinit_2.95.orig.tar.xz 124576 SHA256:c9029cb93f36bbbad8e1ce109f75e6f4d26056d271106e8812cda7159b6f86c8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.95.orig.tar.xz.asc' sysvinit_2.95.orig.tar.xz.asc 313 SHA256:a6b780455ed83b25924fa79d3c8a8669f8ce3cbad44d716d48cc937f25611b83
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.95-5ubuntu2.debian.tar.xz' sysvinit_2.95-5ubuntu2.debian.tar.xz 128052 SHA256:a74a8096e48bdbeef3522e78fdd91faebd754811513a173ed192a83b8aa38307
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

### `dpkg` source package: `tiff=4.0.10+git191003-1`

Binary Packages:

- `libtiff-dev:amd64=4.0.10+git191003-1`
- `libtiff5:amd64=4.0.10+git191003-1`
- `libtiffxx5:amd64=4.0.10+git191003-1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.10+git191003-1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.10+git191003-1.dsc' tiff_4.0.10+git191003-1.dsc 2243 SHA256:13fc55bc813ae19ccc26dd64ab01c18f50a77eaa86054a987a18e2d694bd88a5
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.10+git191003.orig.tar.xz' tiff_4.0.10+git191003.orig.tar.xz 1478116 SHA256:24cd81288a9cfd9d031dc44e1c4ee020b5d4e8ecbffcef3f8949e55f20e9dd50
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.10+git191003-1.debian.tar.xz' tiff_4.0.10+git191003-1.debian.tar.xz 18696 SHA256:1557b9d3a0be9331fe53479a42bf8ef5611a7b980eb55bb3bf4ee3bd3f46da42
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
- `libblkid-dev:amd64=2.34-0.1ubuntu2`
- `libblkid1:amd64=2.34-0.1ubuntu2`
- `libfdisk1:amd64=2.34-0.1ubuntu2`
- `libmount-dev:amd64=2.34-0.1ubuntu2`
- `libmount1:amd64=2.34-0.1ubuntu2`
- `libsmartcols1:amd64=2.34-0.1ubuntu2`
- `libuuid1:amd64=2.34-0.1ubuntu2`
- `mount=2.34-0.1ubuntu2`
- `util-linux=2.34-0.1ubuntu2`
- `uuid-dev:amd64=2.34-0.1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.34-0.1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu2.dsc' util-linux_2.34-0.1ubuntu2.dsc 3689 SHA256:5678a818fa2b906957a8b9f34d69b044c83d22936b8f96055421d3bc76180495
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34.orig.tar.xz' util-linux_2.34.orig.tar.xz 4974812 SHA256:743f9d0c7252b6db246b659c1e1ce0bd45d8d4508b4dfa427bbb4a3e9b9f62b5
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu2.debian.tar.xz' util-linux_2.34-0.1ubuntu2.debian.tar.xz 85032 SHA256:ca3b8dd6fab0270f3a68d071aba99e0ab9fdd0f76551aae46c6f788965690d13
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
