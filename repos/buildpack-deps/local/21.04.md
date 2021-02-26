# `buildpack-deps:hirsute`

## Docker Metadata

- Image ID: `sha256:177543eef8faac30d0ac132bdc7eb3f1ba6040f2e239b5198cbae8369e7e6237`
- Created: `2021-01-21T07:55:07.709644683Z`
- Virtual Size: ~ 695.55 Mb  
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/acl/2.2.53-8/


### `dpkg` source package: `adduser=3.118ubuntu5`

Binary Packages:

- `adduser=3.118ubuntu5`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.118ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu5.dsc' adduser_3.118ubuntu5.dsc 1766 SHA512:8d6e9894549dc9dd53db8480cb18ee9b012bc70ea7b53d72b0ad8ad713a1672d2e94750e1cde44d2b8f9fd7e66b1ea7c2ad20202fc7bcd90e2fba5cee63d5b5d
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu5.tar.xz' adduser_3.118ubuntu5.tar.xz 222904 SHA512:ded568a5a3f5a5ac1acc2098e37160194f8c4622e90c7044d599286a321fe8fd701c8554a4517e4d72a6089b8e3b5592b92d46668032bda81de64cc736bf0a75
```

### `dpkg` source package: `apr-util=1.6.1-5ubuntu1`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu1.dsc' apr-util_1.6.1-5ubuntu1.dsc 2644 SHA512:82969ab0267ea55a687b097f1b48b5161b54fd453e409cd6f67d8a2ffee66dd7edc7eb0c3b4c7fa3264c666b6cc4c116ec74a891157e721bbe520acafaf0939c
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA512:40eff8a37c0634f7fdddd6ca5e596b38de15fd10767a34c30bbe49c632816e8f3e1e230678034f578dd5816a94f246fb5dfdf48d644829af13bf28de3225205d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu1.debian.tar.xz' apr-util_1.6.1-5ubuntu1.debian.tar.xz 342724 SHA512:d31ced761628d2b2535daeea88537f4818f1bb242f3842a955255c74925c453607eb8895fad31e0d7f3cf5c2054ac5ecc4c51296a9da3bada3a98ea01ead46df
```

### `dpkg` source package: `apr=1.7.0-6`

Binary Packages:

- `libapr1:amd64=1.7.0-6`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-6
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-6.dsc' apr_1.7.0-6.dsc 2250 SHA512:32b84f507be86d63a1f71531060058777ec630d07fbc587e3e5d2cb8f08b2db4793e2e4e0463ada9f2845ff4c208f8328df9fece5b61fa02afeacce7c926cca8
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA512:3dc42d5caf17aab16f5c154080f020d5aed761e22db4c5f6506917f6bfd2bf8becfb40af919042bd4ce1077d5de74aa666f5edfba7f275efba78e8893c115148
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA512:19b2b128c7c4cb40db06149c75325013a716c783e28e366c1bacf289fdb5d305e5779d8dc55a63729250ad3338cd4c726e133c788fe53ab3519f1bc8d4da6f90
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-6.debian.tar.xz' apr_1.7.0-6.debian.tar.xz 214280 SHA512:9ab10688afdf5e32911b1feb35f8caaa58a8533bc1dabdebf6d6a1a9439bd59fd07504c81a0edc9d08e0e8b54af2e3713a8adae08fa2a0f6ba2f4c616d6d3a8e
```

### `dpkg` source package: `apt=2.1.18`

Binary Packages:

- `apt=2.1.18`
- `libapt-pkg6.0:amd64=2.1.18`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.1.18/


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
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6.dsc' attr_2.4.48-6.dsc 2433 SHA512:07c45ec6e1c07aae661a31ff7ef81655a3c5e0080be38ce3a6aea116ecba0c5e0fe5154099b8841d7b4e1c9becb81c2d8465191ab121675c0a93efc88dfbc713
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA512:75f870a0e6e19b8975f3fdceee786fbaff3eadaa9ab9af01996ffa8e50fe5b2bba6e4c22c44a6722d11b55feb9e89895d0151d6811c1d2b475ef4ed145f0c923
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA512:39e5879d4879003ba5e1fcb727f91f7661cede12692ae128110328a6c1c5a1e2f79a1329ee4d065f3cc3e0d3d18423f5b5a5b170b5cb49c6888de90d31dcaf9c
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6.debian.tar.xz' attr_2.4.48-6.debian.tar.xz 27260 SHA512:002bc4594aa1691cddd0efa1a68508bda7a52583aad48b474e60cbc9fbcea2fa42f8607d7c86aa75cb424ea7cab191f5d5cb7a988f1c386fa21a07edb98773cc
```

### `dpkg` source package: `audit=1:2.8.5-3ubuntu3`

Binary Packages:

- `libaudit-common=1:2.8.5-3ubuntu3`
- `libaudit1:amd64=1:2.8.5-3ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `autoconf=2.69-14`

Binary Packages:

- `autoconf=2.69-14`

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
$ apt-get source -qq --print-uris autoconf=2.69-14
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-14.dsc' autoconf_2.69-14.dsc 1624 SHA512:e81aef911ddc8fcf41a40c00365e2bf3f2c97634e87375e36e132026e6be80061af3cddd29536e7cedccf19ae6908b07bfe28730eac5b6ee819057134eb005cd
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA512:995d3e5a8eb1eb37e2b7fae53c6ec7a9b4df997286b7d643344818f94636756b1bf5ff5ea9155e755cb9461149a853dfbf2886fc6bd7132e5afa9c168e306e9b
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-14.debian.tar.xz' autoconf_2.69-14.debian.tar.xz 24512 SHA512:4161c185a8c16634db36a857f3ab0b81bd9156b27fe6a6ce893d09d4551d4f7db59c5556050c1e22b98e832b3c4f1b083c6949b7b4ae7993fecc4d8287231685
```

### `dpkg` source package: `automake-1.16=1:1.16.3-2ubuntu1`

Binary Packages:

- `automake=1:1.16.3-2ubuntu1`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.3-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.3-2ubuntu1.dsc' automake-1.16_1.16.3-2ubuntu1.dsc 2596 SHA512:fe939e9cb02813ad9e9444f2f481c0fcc5fb4874458daeae3de79d8eae8adbadfa60f4a13e754cf07e1ea6f738ae004fb6b17ce6f1a651892ebca83928435605
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.3.orig.tar.xz' automake-1.16_1.16.3.orig.tar.xz 1590708 SHA512:7265aeb7f82a8a205761d76e6ade7b7e97831c283349fd80f86e511f4b0b3e17f429d1506fca84c76079f63781e5dbf5ca81455d6bf6cda27d2e5c3d23b0d1aa
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.3.orig.tar.xz.asc' automake-1.16_1.16.3.orig.tar.xz.asc 833 SHA512:dc3d1db453f21f375b1632ec70f3658a2987e0e23bcfc47d3e0fffea7ed886d7a8e0af869fb1e8ac18bbec81959379bf14c5f1bbfd6b1c053179122f4d6fb73a
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.3-2ubuntu1.debian.tar.xz' automake-1.16_1.16.3-2ubuntu1.debian.tar.xz 13216 SHA512:d8b5905eaaae8cfd157eaa925cae7e92c07e4e31c8689dbb8ef837e2f1a1438de46d0f4398201c23107d4af50d6006ed22168bd21eb79f3e046019030267d30f
```

### `dpkg` source package: `autotools-dev=20180224.1+nmu1`

Binary Packages:

- `autotools-dev=20180224.1+nmu1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1+nmu1.dsc' autotools-dev_20180224.1+nmu1.dsc 1663 SHA512:936c08ab3dd1ed42fe3f21ce0973168d80e8739557f15dc4d3a9f98dd70426b20f7ca73619c1621d3751997dc9862cd86c1ca9ff61d18697f2c30dd0158f683b
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1+nmu1.tar.xz' autotools-dev_20180224.1+nmu1.tar.xz 68356 SHA512:4fe5941597e64a6a69f9ce8f5c537d8a4a1cdfad5aa476d4353976476a2f33917b5391c849dd49bbe8ba3571520b79781b14db597e8b5f02eee3c01490032023
```

### `dpkg` source package: `base-files=11ubuntu16`

Binary Packages:

- `base-files=11ubuntu16`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11ubuntu16
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11ubuntu16.dsc' base-files_11ubuntu16.dsc 1697 SHA512:ab78458ed36b750eaecd16f7d5b5ae3adddd7d1dc49fa269ec5137cf2ceaeebf891f2fda78510a4244155d4c94e93f940abad4fe395358926afc03de2ce1b89c
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11ubuntu16.tar.xz' base-files_11ubuntu16.tar.xz 80900 SHA512:f741e6dfe8e44b56a83dcb65a01baa0bcbbf7b3fa91b85d6b24d5f2a9652166b45bbf9de872836f885417901aaf8171965fe4ded9fe56fc84d016e2c05d2ab06
```

### `dpkg` source package: `base-passwd=3.5.48`

Binary Packages:

- `base-passwd=3.5.48`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/base-passwd/3.5.48/


### `dpkg` source package: `bash=5.1-1ubuntu1`

Binary Packages:

- `bash=5.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-1ubuntu1.dsc' bash_5.1-1ubuntu1.dsc 2426 SHA512:40b12984febc7f16c3d9dcaa186e12ee52919971c02b089ae3c7edda98f3522717a827f3fc899fbebca552cadc7f9d069d941a81df4422db3a693abbc2593f1a
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA512:95d3acc542231cb893e1347c7d9dd66687f68cd347a0e9e126fde2d14e68c5b5530d1a5866eafa781e88aa013fcf72b4ad56d2e484c2ac7a69bd90bb149a9b86
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-1ubuntu1.debian.tar.xz' bash_5.1-1ubuntu1.debian.tar.xz 94284 SHA512:e50cc59b66ef4194c1986242e07ccf3b4be92a54c274c49ef77b36fdc38b4b72e5b454468d95e0b9b52b9f04421bc57d746d321ba626e6937b19417ffb809cdd
```

### `dpkg` source package: `binutils=2.35.50.20210106-1ubuntu2`

Binary Packages:

- `binutils=2.35.50.20210106-1ubuntu2`
- `binutils-common:amd64=2.35.50.20210106-1ubuntu2`
- `binutils-x86-64-linux-gnu=2.35.50.20210106-1ubuntu2`
- `libbinutils:amd64=2.35.50.20210106-1ubuntu2`
- `libctf-nobfd0:amd64=2.35.50.20210106-1ubuntu2`
- `libctf0:amd64=2.35.50.20210106-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `brotli=1.0.9-2build2`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2build2`
- `libbrotli1:amd64=1.0.9-2build2`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build2.dsc' brotli_1.0.9-2build2.dsc 2310 SHA512:89c6d31a94ad22663e962582df7545c421141ace6dd70a68e7b9d4de35368a850bb5fd33c6df4bac157fa2fa77b9ad9da81fc2219a643846293c0eed85c5cfee
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build2.debian.tar.xz' brotli_1.0.9-2build2.debian.tar.xz 5652 SHA512:0e2cef83495d666e0dd2aaee5017f4a534bbe115d3274ea01dd5b722b429dca8485c3011583e6fac3f9da378f14d3f409d5c2265b47f01db8028401946222e5b
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
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu2.dsc' bzip2_1.0.8-4ubuntu2.dsc 2212 SHA512:bbb7850c0dca5f3c06ddd057addff1ecad68378fd448f739f8b074e039b03eeceea323ec873bf08864367f7240bddb364735f56ac15a2bc5fb4d83fdd71f83ce
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA512:083f5e675d73f3233c7930ebe20425a533feedeaaa9d8cc86831312a6581cefbe6ed0d08d2fa89be81082f2a5abdabca8b3c080bf97218a1bd59dc118a30b9f3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu2.debian.tar.bz2' bzip2_1.0.8-4ubuntu2.debian.tar.bz2 26561 SHA512:6ac1e2e3e22d989ab49e8f01aab592c35dff9950e2ed4439e9df650d3cd2ed7061796bc1e76c7fe9216e2fef4e1b59991fadb508f7c7bed9178d6dcb26247f8e
```

### `dpkg` source package: `ca-certificates=20200601`

Binary Packages:

- `ca-certificates=20200601`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ca-certificates/20200601/


### `dpkg` source package: `cairo=1.16.0-5`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-5`
- `libcairo-script-interpreter2:amd64=1.16.0-5`
- `libcairo2:amd64=1.16.0-5`
- `libcairo2-dev:amd64=1.16.0-5`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cairo/1.16.0-5/


### `dpkg` source package: `cdebconf=0.256ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.256ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.256ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.256ubuntu1.dsc' cdebconf_0.256ubuntu1.dsc 2865 SHA512:1fca0c6e2a9b4fe03646f05e3ac08b8bf250bdc76c55087d874f51e400719c9f6dc09262f666819b37a9ccd28b6279aa725a60a3595ff009dd80d19b677f4590
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.256ubuntu1.tar.xz' cdebconf_0.256ubuntu1.tar.xz 279604 SHA512:daedcf25351b97bec5c6179f6032c12606e818cc7b15ff76c051222c320011648754596175009bb33da8c083f2f65f5eb228aa77e2246da167e5a440b0eb0972
```

### `dpkg` source package: `coreutils=8.32-4ubuntu2`

Binary Packages:

- `coreutils=8.32-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.32-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-4ubuntu2.dsc' coreutils_8.32-4ubuntu2.dsc 2287 SHA512:bc7eb87f77649ff9d88e1cf0876677a4976b17091266fcbbc6d033e59a41d3156c8f37e6a17edd906e40662595b90267d9d3056b4aad23ac45cbe7448a37210a
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz' coreutils_8.32.orig.tar.xz 5547836 SHA512:1c8f3584efd61b4b02e7ac5db8e103b63cfb2063432caaf1e64cb2dcc56d8c657d1133bbf10bd41468d6a1f31142e6caa81d16ae68fa3e6e84075c253613a145
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz.asc' coreutils_8.32.orig.tar.xz.asc 833 SHA512:9c73b35c9e8f7c2b8eff317afcb5aa3234c5f41c80d1882f3c2342906f3fdc876ae45d1256dd1b8fd3cb58c50925f3c13f93de5018626634fdca3c72c14a9acb
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-4ubuntu2.debian.tar.xz' coreutils_8.32-4ubuntu2.debian.tar.xz 40876 SHA512:261a5c2dbb677dcb69b7ad38a0311613549733b330c9266b90328b0f99ac6127be73d45c981e40bf7ca21dcc3aecc6872df041c118315c75fdccea65dd97fc15
```

### `dpkg` source package: `curl=7.72.0-1ubuntu1`

Binary Packages:

- `curl=7.72.0-1ubuntu1`
- `libcurl3-gnutls:amd64=7.72.0-1ubuntu1`
- `libcurl4:amd64=7.72.0-1ubuntu1`
- `libcurl4-openssl-dev:amd64=7.72.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2ubuntu1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2ubuntu1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2ubuntu1.dsc' cyrus-sasl2_2.1.27+dfsg-2ubuntu1.dsc 3487 SHA512:ad266e681201fd0d6f8f99159b9df2225356e6c8ee91fec373143937cab086f180341f7df6955d1655ecc7344507ebb7dc15ba8dd631ed95bac61d4a9b0ae7cb
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA512:a795e4362f85a50e223c5456d03526832eb29fdbc9e17a767045f8542638e3f987d382b79b072bcd694bd1a12cbb818cff6c326063ca2bbe05453c1acf7fb8ad
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2ubuntu1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2ubuntu1.debian.tar.xz 100212 SHA512:656009b18d4edb7934ba77cd66fa6c2748c203c0ae5f7315bb53b5806093650e5f504d25e5f0188c52723dd7fe7b88f9942c51bb61c70b3a8d02ff040c8a19fb
```

### `dpkg` source package: `dash=0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66-5ubuntu1`

Binary Packages:

- `dash=0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66-5ubuntu1`

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
$ apt-get source -qq --print-uris dash=0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66-5ubuntu1.dsc' dash_0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66-5ubuntu1.dsc 2487 SHA512:fc4dbdd307971e2223450705802bccffd3542a2c12b33be28577071b7d670e775f3502888f9e0b1cefbf2ed6907f69963d4195537156966bb4fcf3a1ef031076
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66.orig.tar.gz' dash_0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66.orig.tar.gz 167776 SHA512:808da76a634bd6bc13990f83ad3da336ae92b0b6ff5029744f9c0cc3d2adfe0b2f1cacac6eccc56ef445fe4c1ae1ee8bd6af035285478c62bb7fe10e3d19220d
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66-5ubuntu1.debian.tar.xz' dash_0.5.11+git20200708+dd9ef66+really0.5.11+git20200708+dd9ef66-5ubuntu1.debian.tar.xz 43288 SHA512:25b0d7627153429daac9767f926ee6f80c54cb7c95d651515e01dc3ddf80c241cec228cef4057c8652f9b1b3dfcfebc5404e716424d9d1ca5634d454e02dfb3a
```

### `dpkg` source package: `db-defaults=1:5.3.21~exp1ubuntu2`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21~exp1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21~exp1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.dsc' db-defaults_5.3.21~exp1ubuntu2.dsc 2044 SHA512:f0bd0c0e9c1b19bd5eae5aeb1c8d17664db82c77428c7e4eeb4f27f8a1ec203cf55530d4ffbaa895b186eb639f89287cb9b2798d8ad9b011006a70471f7733ff
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.tar.xz' db-defaults_5.3.21~exp1ubuntu2.tar.xz 3032 SHA512:da58650b949140e8a5f85bae82af5a040c2558fd41763cef3adc8b2f0201a5f13952e4d25b428fef1d0e1cdda6b463c0cfd3402c4f6b6c2727f171bcaf956c25
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6ubuntu3`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6ubuntu3`
- `libdb5.3-dev=5.3.28+dfsg1-0.6ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu3.dsc' db5.3_5.3.28+dfsg1-0.6ubuntu3.dsc 3234 SHA512:e21d4044cf96550b5ed7a0b7ba8209f5bf9c630bfbd862783399f78963964834e0d9ab9ad42815d6fb8882ac92b57cbac0425b9b09a2606f4f673ae93692b4d8
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA512:50cb87bc3f24065839ee2932e82af032b236b290ebe89983076f503c6c62c5f36ff93d7847a3f68b2b19f35088fbab5d3ac6a34553d07e8148e68e9a3f079a12
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu3.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6ubuntu3.debian.tar.xz 30776 SHA512:0afcbf1a9899abaa38035f4c87f44060f63c9f4098e261987317457ea0ab3582f9afaa671015ba25e90be2620fa3b625b4fb9032aff3bc12aeb6004ca6a64fe6
```

### `dpkg` source package: `debconf=1.5.74`

Binary Packages:

- `debconf=1.5.74`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.74
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.dsc' debconf_1.5.74.dsc 2082 SHA512:b2ca913745ff661261cbe2e7338f7fcb6b5bbdd52aaa981950abd0714506ca9b68d15b63dfce8f2605ae7cf675ce4dd407ac822d8e4a71adea8b33a3a35975ec
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.tar.xz' debconf_1.5.74.tar.xz 571108 SHA512:421577c9fb0dae1c851c6676e7b0b3e59e5800d1ab01a9817e4506ee2f7cb812065e1a64b194b1192023951f1f0cabf0359e4dae4320b9cf0705865085cdc5cd
```

### `dpkg` source package: `debianutils=4.11.2`

Binary Packages:

- `debianutils=4.11.2`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.11.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.11.2.dsc' debianutils_4.11.2.dsc 1644 SHA512:b549fe5ef5553f37e5e5c7c0273cf65170224cf0742a721727656b46c31d5495d817c0d6744485028da547de2e7643c92afb9c74f88bb8b4bd96a94bfcac4f2c
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.11.2.tar.xz' debianutils_4.11.2.tar.xz 158132 SHA512:0bd9098beee78b3c8dae839f0c29e9f142cbb22f2ced473cf7ae47a14d9493ba882c1829eba213780392a87a3223b3689729754c8ded80a091efaef3f6f903fd
```

### `dpkg` source package: `diffutils=1:3.7-3ubuntu1`

Binary Packages:

- `diffutils=1:3.7-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.7-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3ubuntu1.dsc' diffutils_3.7-3ubuntu1.dsc 1905 SHA512:258703c49c3f7413bad052b6cace7b5106b157fc179bbdec8c36a7c182b147171da875f64bfba0fc34b3651cfd2a0c53cfe667b7c3a8de51a0b1e8788eec59b9
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz' diffutils_3.7.orig.tar.xz 1448828 SHA512:7b12cf8aea1b9844773748f72272d9c6a38adae9c3c3a8c62048f91fb56c60b76035fa5f51665dceaf2cfbf1d1f4a3efdcc24bf47a5a16ff4350543314b12c9c
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3ubuntu1.debian.tar.xz' diffutils_3.7-3ubuntu1.debian.tar.xz 11816 SHA512:81e62590049c2441daaddb81aaf5bef4ccac044e4ac25f1e00b5f2e958d1bd9a429aafdebfb58313cdbb170d2ef832161a2782b45c56c522661f2b73c8ff9696
```

### `dpkg` source package: `djvulibre=3.5.28-1`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.28-1`
- `libdjvulibre-text=3.5.28-1`
- `libdjvulibre21:amd64=3.5.28-1`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.28-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-1.dsc' djvulibre_3.5.28-1.dsc 2388 SHA512:3aa31db19fab3309cabeb95b0fd8b09705644dcbc683d310d16f0c59e49b7b9c71890f963add724a7eb61b38eee9a009ce3f1b6b055815b305f5b462cd29e8f4
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28.orig.tar.xz' djvulibre_3.5.28.orig.tar.xz 2959024 SHA512:4fdbecd2b7b583ee4211c9cda6638a3a831c883e2552b3c8ad09f69e8734831addc14f590faab8c58d7f9f017b527abccc384f6066e674e341cf43c96db49cb7
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-1.debian.tar.xz' djvulibre_3.5.28-1.debian.tar.xz 14944 SHA512:7cb97d27112abdc51012cdd015622480d2a651024ea407204295c467666144de5a2a90ed36ab84db49ceb3aaf9b63344db7c68be0f146d18b6be5241449c9313
```

### `dpkg` source package: `dpkg=1.20.5ubuntu3`

Binary Packages:

- `dpkg=1.20.5ubuntu3`
- `dpkg-dev=1.20.5ubuntu3`
- `libdpkg-perl=1.20.5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `elfutils=0.182-3`

Binary Packages:

- `libelf1:amd64=0.182-3`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.182-3
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.182-3.dsc' elfutils_0.182-3.dsc 3031 SHA512:f22a6f4c50732c587b5cb953bb0b41fab03466b00028e50a559258afd54537ad6582863e3a0cab03020a0b7772687a073180338a959efa4b4d15666fbcb529f2
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.182.orig.tar.bz2' elfutils_0.182.orig.tar.bz2 9096742 SHA512:8ab0735bbe11b4383169341bf674ace360038b6ae5239f1d5a991c46260cd4bce545e078735b7de3b8fab132bb5da41f60689ff1b1d7ebccfada117a954a2c81
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.182-3.debian.tar.xz' elfutils_0.182-3.debian.tar.xz 33796 SHA512:445807ff2c5a9a22ee4f8b468ca126c81d813978a8f1a1e58aef64ed8e15937b651bad2d90c1ef6e2b62dab821faa708cb62d075234364f26917adead11cc226
```

### `dpkg` source package: `expat=2.2.10-1`

Binary Packages:

- `libexpat1:amd64=2.2.10-1`
- `libexpat1-dev:amd64=2.2.10-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.10-1.dsc' expat_2.2.10-1.dsc 1962 SHA512:7e8d988db934d374c408f6edf2e2ae14d30e7011b36e5d76c776482ab8d13d99e160e0e67e1b14ed2de1b6609c4f161333f55b9aead2937f99916d3e51a02944
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.10.orig.tar.gz' expat_2.2.10.orig.tar.gz 8276395 SHA512:5f2d00ead20139aae89910cc08246cf15f7562af2a4fe1b37ebe4c1500a71d9f0a655ebc43f10164ac846be3186ff43f2b94287b18d2a3af882cbd0a1de41a36
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.10-1.debian.tar.xz' expat_2.2.10-1.debian.tar.xz 10688 SHA512:233902d4d5df5da236bdbf73a0a942699baf931297dd2a6ed4ef7a251174a605de7be8fecc2ee1dcb96786f2584e277073f5f587352654319f77215c80f7f6d1
```

### `dpkg` source package: `fftw3=3.3.8-2ubuntu6`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu6.dsc' fftw3_3.3.8-2ubuntu6.dsc 3010 SHA512:e67e452520bfed6cc0f75e2b4ef49500258536f6ba97417a012c32d5fc4e0b881d7b264e39705d177126261d2e2b6775616726b966b089ed3147aa87c6e1525c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA512:ab918b742a7c7dcb56390a0a0014f517a6dff9a2e4b4591060deeb2c652bf3c6868aa74559a422a276b853289b4b701bdcbd3d4d8c08943acf29167a7be81a38
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu6.debian.tar.xz' fftw3_3.3.8-2ubuntu6.debian.tar.xz 14208 SHA512:fcb2c5a3e073ad60121c0847ba99584f4bcde05dc3f98f0caf13814b9c0840d68b41b94c8003c312fe3a931dd85dd39667902133e97403fa394d6de63349240c
```

### `dpkg` source package: `file=1:5.39-3`

Binary Packages:

- `file=1:5.39-3`
- `libmagic-mgc=1:5.39-3`
- `libmagic1:amd64=1:5.39-3`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.39-3
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39-3.dsc' file_5.39-3.dsc 2237 SHA512:79399bd3c0c70121d19e737c4323d247085a796ce76205246678abd109a6a28b564d8bd85e2b0e2c40a8b047b12ccfcb31346b5ebbbc91ebd36903684a096fd2
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39.orig.tar.gz' file_5.39.orig.tar.gz 954266 SHA512:9cf1a7b769c56eb6f5b25c66ce85fa1300128396e445b2e53dbbd8951e5da973a7a07c4ef9f7ebd1fe945d47bdaf2cd9ef09bd2be6c217a0bcb907d9449835e6
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39.orig.tar.gz.asc' file_5.39.orig.tar.gz.asc 169 SHA512:0b9654e3576862ff0214e67ad023ccc445a8a4a7f40bccc39ec1b332c9952bdb5ed4c324cc36da36c2dce6cb35f3bbf29069c19c574b8705724c7c7d0c562caf
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39-3.debian.tar.xz' file_5.39-3.debian.tar.xz 34420 SHA512:1a664d162fb5827c24ec8a2f6909bb33803148b5b25f6d372784e501636c39f5758687703878bf83fd45045e59f6a862f9bebadf5633caebc0945fe4e85edeac
```

### `dpkg` source package: `findutils=4.7.0-1ubuntu2`

Binary Packages:

- `findutils=4.7.0-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `fontconfig=2.13.1-4.2ubuntu2`

Binary Packages:

- `fontconfig=2.13.1-4.2ubuntu2`
- `fontconfig-config=2.13.1-4.2ubuntu2`
- `libfontconfig-dev:amd64=2.13.1-4.2ubuntu2`
- `libfontconfig1:amd64=2.13.1-4.2ubuntu2`
- `libfontconfig1-dev:amd64=2.13.1-4.2ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2build1.dsc' fonts-dejavu_2.37-2build1.dsc 2411 SHA512:7821679b0f3cabaa4929b11a1a02fff21c05cef965efc399bf8a89b8549b1ac20cdd173c2cb31c397a345683b197623b97998b412c8458a135141ccd733b50d9
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA512:e61fc8c675ef76edb49dd9a8caee62087280929bb8144b52aca2f8def30025c56246589ad8a6a806b9574e6876eedd16d57c70a6ce9c86817a2dfe39d8a2bb2b
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2build1.debian.tar.xz' fonts-dejavu_2.37-2build1.debian.tar.xz 11468 SHA512:b3c0cb3c81b3e4e9d76eefab010f447be973fa9e310960d2e3a1a2e845f4388e0508f8d18d519c7374c68c96c2e05a75f29ccf24135f6250a82181a77d8e9741
```

### `dpkg` source package: `freetype=2.10.4+dfsg-1`

Binary Packages:

- `libfreetype-dev:amd64=2.10.4+dfsg-1`
- `libfreetype6:amd64=2.10.4+dfsg-1`
- `libfreetype6-dev:amd64=2.10.4+dfsg-1`

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
$ apt-get source -qq --print-uris freetype=2.10.4+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4+dfsg-1.dsc' freetype_2.10.4+dfsg-1.dsc 3693 SHA512:5baa3cf53dfea6426980f414d43dd3bfba467b079d955779300cb64c2f9add33aa7841190329cebc45e9a2de56ad20763c6581c9c2266392e2cff861c5b8b783
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2demos.tar.xz' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz 236712 SHA512:d2afc19e5fabbee5205fcc992f6c19bab03485b7af4f55bb2d2dd0a4a9492a3f593540862ca116b54cf161b240d7966cb31a9793578d164fc418449e339e2fa8
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2demos.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz.asc 195 SHA512:6b297a67afd11d21e705f6bfd82ffefec2a3a424a6a1bc5b24b80f037337f888677d7af3bab5d0be13d779162de8d4ae8f30f7fd978de6f6693567f4899980bf
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2docs.tar.xz' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz 2079084 SHA512:171da6c6a172869e9bec0da67cb1abdb0fdb124870f13b751b4e9b1b5e342fb2af38cb606db1c3dcf18076a077e694b7b8dd055dd7f4ab49afe7e1d61b4f9ba8
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4+dfsg.orig-ft2docs.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz.asc 195 SHA512:c42ed2aea76eee7f4e775e26276fd260249b672c06ae0c73f378bc0ac7425e36683c4f8b4a8875d5f31f08d9f8e3a7ba0b427d9a5308c8aa90718c42edf13c52
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4+dfsg.orig.tar.xz' freetype_2.10.4+dfsg.orig.tar.xz 2259340 SHA512:4d02111df4eb932cb1fd4890e6487a0a6830d98dbf35a6377b0fb2b66af89b06a449e149950271adbbff7411e2949e5a2a4ad6cd376e06287b5892dbe3bce3dc
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4+dfsg-1.debian.tar.xz' freetype_2.10.4+dfsg-1.debian.tar.xz 116636 SHA512:0d69ceff879f5a30b6c416b381293cf72ed481eedfdee63a7cde89d12203749f0e81b9f668a8af8ebeec43cc507f03ae15f93803797380c4b77040df6654d7e4
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
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.dsc' fribidi_1.0.8-2.dsc 1987 SHA512:f2f799a6b3704c158482caf08719ef62ca646b03f21b08405e65a9ffc8619335112198aa0a5108632fb7490243f740657d9d0659e52d4c1cebc8300add54e963
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA512:d66b1524b26d227fd6a628f438efb875c023ae3be708acaaad11f1f62d0902de0a5f57124458291ef2b0fcd89356c52ab8ae5559b0b5a93fa435b92f1d098ba2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.debian.tar.xz' fribidi_1.0.8-2.debian.tar.xz 8980 SHA512:04d10d26c3ccf3a0e2782a780fcbe64f1ab47c85633ffeefb1a9251e29ff20a046509afcb30b32a2ec52a52780d5054aad2ec07517b7b667fb06ab99125f9ea3
```

### `dpkg` source package: `gcc-10=10.2.1-6ubuntu1`

Binary Packages:

- `cpp-10=10.2.1-6ubuntu1`
- `g++-10=10.2.1-6ubuntu1`
- `gcc-10=10.2.1-6ubuntu1`
- `gcc-10-base:amd64=10.2.1-6ubuntu1`
- `libasan6:amd64=10.2.1-6ubuntu1`
- `libatomic1:amd64=10.2.1-6ubuntu1`
- `libcc1-0:amd64=10.2.1-6ubuntu1`
- `libgcc-10-dev:amd64=10.2.1-6ubuntu1`
- `libgcc-s1:amd64=10.2.1-6ubuntu1`
- `libgomp1:amd64=10.2.1-6ubuntu1`
- `libitm1:amd64=10.2.1-6ubuntu1`
- `liblsan0:amd64=10.2.1-6ubuntu1`
- `libquadmath0:amd64=10.2.1-6ubuntu1`
- `libstdc++-10-dev:amd64=10.2.1-6ubuntu1`
- `libstdc++6:amd64=10.2.1-6ubuntu1`
- `libtsan0:amd64=10.2.1-6ubuntu1`
- `libubsan1:amd64=10.2.1-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp-10/copyright`, `/usr/share/doc/g++-10/copyright`, `/usr/share/doc/gcc-10/copyright`, `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-10-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-10-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gcc-defaults=1.189ubuntu1`

Binary Packages:

- `cpp=4:10.2.0-1ubuntu1`
- `g++=4:10.2.0-1ubuntu1`
- `gcc=4:10.2.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.189ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.189ubuntu1.dsc' gcc-defaults_1.189ubuntu1.dsc 16534 SHA512:fa7d4341b4d79d3ec6c943ebf883f18f839389439f7aaa6abece5c11723b4d21396ffc67d88ef8e91bbeeac58c5b7549fc3c0506a74f4474fe4157b37b2daa51
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.189ubuntu1.tar.xz' gcc-defaults_1.189ubuntu1.tar.xz 48464 SHA512:da292a787accdf1bc0f17eb378c1e2efe8a533f3fdd8cac56863638c0b4b93af829e980721c90fdaa8c0e3fb8d4af579c4b5629c984ae87e0f456bc0b1230312
```

### `dpkg` source package: `gdbm=1.19-2`

Binary Packages:

- `libgdbm-compat4:amd64=1.19-2`
- `libgdbm-dev:amd64=1.19-2`
- `libgdbm6:amd64=1.19-2`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.19-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19-2.dsc' gdbm_1.19-2.dsc 2603 SHA512:ca70a14f93b56b42eb87a820e04b8402075b1048cce0e39a1fd337cc3551dba9803db931ef8a0b50e3f9e5cb6d553df8bdf12f8908fc27c49de2670c0c3812d9
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19.orig.tar.gz' gdbm_1.19.orig.tar.gz 967861 SHA512:118c5b8cdf74898bfb7c2100302fedf80096be017bf08e80a44486563cad5d93b93567622f2e7c7aceb72f30460504bd0b4ddfccf34df994ed65166e12ecd495
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19.orig.tar.gz.asc' gdbm_1.19.orig.tar.gz.asc 181 SHA512:db24d7438a22a8c7974d7aa889f72e1abf402fa56dcbefa19b3cc6ffe08c73f9a251b898de548eaec50759102ebe3df486ebb785e90d571f7c8f10715e3c15d0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19-2.debian.tar.xz' gdbm_1.19-2.debian.tar.xz 16228 SHA512:36f7bb8e249c5b03840d7ad859cbb4cb6d71f9485cfafbaef219aef78954d17e5e1056289c13c2c1ede67a04f53e7532f02187faa6c8c2b4cb0402a6ee541a79
```

### `dpkg` source package: `gdk-pixbuf-xlib=2.40.2-2build2`

Binary Packages:

- `libgdk-pixbuf-xlib-2.0-0:amd64=2.40.2-2build2`
- `libgdk-pixbuf-xlib-2.0-dev:amd64=2.40.2-2build2`
- `libgdk-pixbuf2.0-0:amd64=2.40.2-2build2`
- `libgdk-pixbuf2.0-dev:amd64=2.40.2-2build2`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf-xlib-2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf-xlib-2.0-dev/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf-xlib=2.40.2-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf-xlib/gdk-pixbuf-xlib_2.40.2-2build2.dsc' gdk-pixbuf-xlib_2.40.2-2build2.dsc 2540 SHA512:34af6756a3ff11856d32373a54d76a6f9fbca051d5f35a1cc84ca890eb1e8506fa7613942cc39d80b808f29695c6aa343dddd301e66c2bd566e5cab88885d66c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf-xlib/gdk-pixbuf-xlib_2.40.2.orig.tar.xz' gdk-pixbuf-xlib_2.40.2.orig.tar.xz 53588 SHA512:246bcace03f4d7d694c4d08f28c7ad044cab63b5cf264b478ee1fe161499e7607c7ffeff93908f1f3b308e5108d78c4b51a3f90b79189d42a1a653c8edc53e37
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf-xlib/gdk-pixbuf-xlib_2.40.2-2build2.debian.tar.xz' gdk-pixbuf-xlib_2.40.2-2build2.debian.tar.xz 14176 SHA512:fdd5c851f633a45b6bcd0fd3fc42d418f4755562cee8648e2c1b8044ce5b965d5e23a062c53d2714d8537971d6f192b3ac6d3ebc60e772619b59eecbf935155e
```

### `dpkg` source package: `gdk-pixbuf=2.42.2+dfsg-1`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.42.2+dfsg-1`
- `libgdk-pixbuf-2.0-0:amd64=2.42.2+dfsg-1`
- `libgdk-pixbuf-2.0-dev:amd64=2.42.2+dfsg-1`
- `libgdk-pixbuf2.0-bin=2.42.2+dfsg-1`
- `libgdk-pixbuf2.0-common=2.42.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-dev/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.42.2+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.2+dfsg-1.dsc' gdk-pixbuf_2.42.2+dfsg-1.dsc 3276 SHA512:6c8ad04639afecdc1db5e8bdd156b940993c12af06c83f961e882b230dec9fb437b8ca761096e974988293fd030b3bf93fca105312310e438b137ea00e96a0a5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.2+dfsg.orig.tar.xz' gdk-pixbuf_2.42.2+dfsg.orig.tar.xz 6433920 SHA512:b3f12fd1592f5b39b319791196c44cc1a05a05b4515cb30ea1ea7ad65763332203e2054d8fffee35685db603180bbf071a7b44ec72743cac3207f152779ece95
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.2+dfsg-1.debian.tar.xz' gdk-pixbuf_2.42.2+dfsg-1.debian.tar.xz 28940 SHA512:4e80f09cd7936a65fd734251d98c54756e6b1fcd13b6836938922a92e95e17486b9d6dfdd63e77b5a488a6681427e53b94495e86b25d4881ba8d156bef44b338
```

### `dpkg` source package: `git=1:2.29.2-1ubuntu1`

Binary Packages:

- `git=1:2.29.2-1ubuntu1`
- `git-man=1:2.29.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `glib2.0=2.66.4-1`

Binary Packages:

- `libglib2.0-0:amd64=2.66.4-1`
- `libglib2.0-bin=2.66.4-1`
- `libglib2.0-data=2.66.4-1`
- `libglib2.0-dev:amd64=2.66.4-1`
- `libglib2.0-dev-bin=2.66.4-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.66.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.66.4-1.dsc' glib2.0_2.66.4-1.dsc 3383 SHA512:f04d4ce12a3f736f0b62b66e7d44c1a78f99cb20350921afce5ba85509c55e35470875440f13d1af2374268a1d6cf617ed253a4f0048ed9149e22337f7c8b67c
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.66.4.orig.tar.xz' glib2.0_2.66.4.orig.tar.xz 4838124 SHA512:b3bc3e6e5cca793139848940e5c0894f1c7e3bd3a770b213a1ea548ac54a2432aebb140ed54518712fb8af36382b3b13d5f7ffd3d87ff63cba9e2f55434f7260
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.66.4-1.debian.tar.xz' glib2.0_2.66.4-1.debian.tar.xz 97544 SHA512:5e21ce053b1924a029665420db04bc44d9b03069e979ee871ce29a03f45167648524fbde54ca01ebb0d884d25ab1b823dad2bd36e123dd22ef83235745218499
```

### `dpkg` source package: `glibc=2.32-0ubuntu6`

Binary Packages:

- `libc-bin=2.32-0ubuntu6`
- `libc-dev-bin=2.32-0ubuntu6`
- `libc6:amd64=2.32-0ubuntu6`
- `libc6-dev:amd64=2.32-0ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gnupg2=2.2.20-1ubuntu2`

Binary Packages:

- `dirmngr=2.2.20-1ubuntu2`
- `gnupg=2.2.20-1ubuntu2`
- `gnupg-l10n=2.2.20-1ubuntu2`
- `gnupg-utils=2.2.20-1ubuntu2`
- `gpg=2.2.20-1ubuntu2`
- `gpg-agent=2.2.20-1ubuntu2`
- `gpg-wks-client=2.2.20-1ubuntu2`
- `gpg-wks-server=2.2.20-1ubuntu2`
- `gpgconf=2.2.20-1ubuntu2`
- `gpgsm=2.2.20-1ubuntu2`
- `gpgv=2.2.20-1ubuntu2`

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
$ apt-get source -qq --print-uris gnupg2=2.2.20-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu2.dsc' gnupg2_2.2.20-1ubuntu2.dsc 3934 SHA512:6f0195968ac45b7d741908bd4890b65dc61b4305fbb71090191f3123a6b4d77f9b799fa4ce737f21f53254e98622150dc4f5acf0e43add6b68f1cb069a4d142a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2' gnupg2_2.2.20.orig.tar.bz2 6786913 SHA512:3e69f102366ec3415f439ab81aae2458182fa1a18dfb86565b1d9dc638f3fc4c179a5947f0042b7c5a813345676285a662793664a1803ea9ad8328f0548e0edc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2.asc' gnupg2_2.2.20.orig.tar.bz2.asc 1357 SHA512:0972788af253f84959ab3142e3d4bf025b7e7077377574e69851ae3d37cbf296211fdf50cd77fe47f844bc3383489ff88cf35186d2f72cb0adc84cdfe77bfd26
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu2.debian.tar.xz' gnupg2_2.2.20-1ubuntu2.debian.tar.xz 64836 SHA512:54d3cff7a23dfde6790381711d30602c52f4e6e90b416eb4e9b69c5cc5f0e19ed6ddd4fd28bd9536cbbd026942015b74dc6e2beec6af50a1e99c49e53aeee32f
```

### `dpkg` source package: `gnutls28=3.7.0-5ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.0-5ubuntu1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.0-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.0-5ubuntu1.dsc' gnutls28_3.7.0-5ubuntu1.dsc 3612 SHA512:ee0e59591341d7d439ab75fad4eaf41ab2b0c0c69230db0bc92dedf128715ed687c8f2d052bce96f7570fae631603dd9855ad23f2d785e8e7b5e727070a599b7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.0.orig.tar.xz' gnutls28_3.7.0.orig.tar.xz 6129176 SHA512:5cf1025f2d0a0cbf5a83dd7f3b22dafd1769f7c3349096c0272d08573bb5ff87f510e0e69b4bbb47dad1b64476aa5479804b2f4ceb2216cd747bbc53bf42d885
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.0.orig.tar.xz.asc' gnutls28_3.7.0.orig.tar.xz.asc 854 SHA512:081bcac03c4461cca2fe7223fa4191fc2d069516452bfb63541e8eae8ca321c40a60c63bba51521282e2d6d10299251b90aa748a4c9a2e910de9a457e7a4e2e5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.0-5ubuntu1.debian.tar.xz' gnutls28_3.7.0-5ubuntu1.debian.tar.xz 72556 SHA512:df1121128cdd28b078bffa2e29e1f71fa574961d330d5d99d2d23c65fe2a292414a53f968b58ed6847aea3706327b7cee32a37a6d8a62a01649af148c4b23f9e
```

### `dpkg` source package: `gobject-introspection=1.66.1-1build1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.66.1-1build1`
- `gir1.2-glib-2.0:amd64=1.66.1-1build1`
- `libgirepository-1.0-1:amd64=1.66.1-1build1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.66.1-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.66.1-1build1.dsc' gobject-introspection_1.66.1-1build1.dsc 2984 SHA512:ce56d8438971677035d47f17b909412dcc4a9dee67245ee5dc829f7c010b0e3330add8b25db3db4dd8b2f81b934b676a2ab012bc4502ec8ab1fe389482c39a72
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.66.1.orig.tar.xz' gobject-introspection_1.66.1.orig.tar.xz 1012784 SHA512:ea1e20cd94ff8af3572f417f35e96648ffc3e94a91d4e4c81adf99bb0f408ac21ecf40990f9dbd5f2e0f4e83360286ca5db88dbc45bd59289596a324acf7df3d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.66.1-1build1.debian.tar.xz' gobject-introspection_1.66.1-1build1.debian.tar.xz 23720 SHA512:1ac379e974376e1f095f88d9f1980158810fd077d66f2bb49e87bf9981ed18a89aa2aee15835f4945521f4624d6c266aebf5674e0f9803c4030eba2270c19f45
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1.dsc' graphite2_1.3.14-1.dsc 2608 SHA512:a1f4621189784463b7b0cfaa9c2615087746f077db6d90909866c30b14789a4e8847ce00c37345a5ce02177d2eba1a2720688edf516e38f099bafbdf050fb35f
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14.orig.tar.gz' graphite2_1.3.14.orig.tar.gz 6629829 SHA512:49d127964d3f5c9403c7aecbfb5b18f32f25fe4919a81c49e0534e7123fe845423e16b0b8c8baaae21162b1150ab3e0f1c22c344e07d4364b6b8473c40a0822c
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1.debian.tar.xz' graphite2_1.3.14-1.debian.tar.xz 12068 SHA512:4f9fab5bf556fbfe6ad80560d0e8d48bd0c38d5996beb938f8ed7cdad44b230881eb3a32dd9e7352fca2b185005ecdc2d3915727ef4f40047818f2bac1b58342
```

### `dpkg` source package: `grep=3.6-1`

Binary Packages:

- `grep=3.6-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6-1.dsc' grep_3.6-1.dsc 1644 SHA512:df414b678efc2cc78b275594bad61ce2e657ff7b52af57eddb22795c11043f70f1b699e63b4e2c48f8be15a44cdc026f19dc793b4d2ee85c62e0421caadf1b08
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6.orig.tar.xz' grep_3.6.orig.tar.xz 1589412 SHA512:8934544a19ded61344d83ff2cab501e86f17f8ae338892e0c36c2d2d8e63c76817840a0071ef5e3fcbca9115eba8a1aae0e4c46b024e75cd9a2e3bd05f933d90
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6.orig.tar.xz.asc' grep_3.6.orig.tar.xz.asc 833 SHA512:0cdf0078d10fda8aecc434f35148fa18378dd160002d745fb960fe506aedfcdab379ba5aeff9e692becd05b7717033401bd7d92b1aabe151b47561682669a3cd
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6-1.debian.tar.xz' grep_3.6-1.debian.tar.xz 17748 SHA512:cf35da621f88880c03c41d1f174fd1a091630552f264340a86801c2603ebe189671ed1120466a53710cb94659d0b1b2124bd4f00d33c11dd0e7a5d3d905cf46c
```

### `dpkg` source package: `gzip=1.10-2ubuntu2`

Binary Packages:

- `gzip=1.10-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `harfbuzz=2.6.7-1ubuntu1`

Binary Packages:

- `libharfbuzz0b:amd64=2.6.7-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.dsc' heimdal_7.7.0+dfsg-2.dsc 3580 SHA512:09d067d3a6060bffc5484417e2329f0534344c7f0b839195dfd126abcf8c2e626cca5d88ba941ae20c2e0ca81bfd8b99ff19b3d5a8fc7e99a1f465a3b5b3c457
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg.orig.tar.xz' heimdal_7.7.0+dfsg.orig.tar.xz 5945252 SHA512:14141f3fff264c9516f736bcc51c998df69cfaa7108d2387921299efd7e82d79b918dee4029905dc221c204d3340ffc17da9472baf80029372d7c13de328ec0a
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.debian.tar.xz' heimdal_7.7.0+dfsg-2.debian.tar.xz 128660 SHA512:a5435ead813f75b0bc7b071dbf4030378f0a8217acd2837d94d0527c0dc456509cd0eef945f7a5c397f7bd2b893400f9813837c404b5b7b0b84fc7540fe40e3e
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
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.dsc' hicolor-icon-theme_0.17-2.dsc 2053 SHA512:5b8b3088f8d9469076d5d2a3448e1115a910958a4ba4b3bbeae287ae3e91fa3a26b87f544a1f92925230e33f6f20e96df51bc5ec01b2735e07bb3f9be2e06c3c
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17.orig.tar.xz' hicolor-icon-theme_0.17.orig.tar.xz 53016 SHA512:eca8655930aa7e234f42630041c0053fde067b970fad1f81c55fcd4c5046c03edfdf2ede72a3e78fba2908e7da53e9463d3c5ae12ab9f5ef261e29a49f9c7a8d
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.debian.tar.xz' hicolor-icon-theme_0.17-2.debian.tar.xz 3536 SHA512:74b8de58f18f861f0f724419514b787495cf67b39abcfdbdc7be6923e44112b86710c015ea5e4c83301d201b503a1014fca335c6dadc522d7f7edca80f638489
```

### `dpkg` source package: `hostname=3.23`

Binary Packages:

- `hostname=3.23`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.dsc' hostname_3.23.dsc 1402 SHA512:d520afa2db493464f3b63edc680307f6734c7cf1ec516a42f8de60c3d2d99e3a2e3c18ee5c190cd36f4c3271584b24fe8a4cc7a610b8feaa31c02315f3da512d
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.tar.gz' hostname_3.23.tar.gz 13672 SHA512:aff70bc381ea58944e01f0cabfc674a273b18b0935a87737e16964c08c24382177cc3495368f88a877e293b7fbda76684979cc227eca93e4b033b9c3a975af01
```

### `dpkg` source package: `icu=67.1-5`

Binary Packages:

- `icu-devtools=67.1-5`
- `libicu-dev:amd64=67.1-5`
- `libicu67:amd64=67.1-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/icu/67.1-5/


### `dpkg` source package: `ilmbase=2.5.3-2`

Binary Packages:

- `libilmbase-dev:amd64=2.5.3-2`
- `libilmbase25:amd64=2.5.3-2`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase25/copyright`)

- `boost`
- `ilmbase`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ilmbase/2.5.3-2/


### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu15`

Binary Packages:

- `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu15`
- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1ubuntu15`
- `imagemagick-6.q16=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickcore-6-arch-config:amd64=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickcore-6-headers=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickcore-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickcore-dev=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickwand-6-headers=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickwand-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu15`
- `libmagickwand-dev=8:6.9.10.23+dfsg-2.1ubuntu15`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `init-system-helpers=1.59`

Binary Packages:

- `init-system-helpers=1.59`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/init-system-helpers/1.59/


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
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.23-1.dsc' isl_0.23-1.dsc 1832 SHA512:a6bb9d9993fe59e90963a007cf1134a62b1454e244b08259af879ff21764c897edf3ccdcd9e36392df8ae1a1367d6e4bdef7610870ef5e37f12cd8da91694b64
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.23.orig.tar.xz' isl_0.23.orig.tar.xz 1729656 SHA512:da4e7cbd5045d074581d4e1c212acb074a8b2345a96515151b0543cbe2601db6ac2bbd93f9ad6643e98f845b68f438f3882c05b8b90969ae542802a3c78fea20
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.23-1.debian.tar.xz' isl_0.23-1.debian.tar.xz 26044 SHA512:79868f2f377ddf8e68714b3b05b9d4cf5ec8c41f1c951975ed82df8ccca2a05db32f802983ce29f38007bc2b33fa5e99f9a0f7cd4d64af370191a4faa09e67d7
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
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.dsc' jbigkit_2.1-3.1build1.dsc 2085 SHA512:62ac0d564fcbe39c097c4e5e0e43dd5f9676f48c85b58affa016e703d4faa464ec01f47756276e874fb195ee0bb968ea24e39ef3656351b23b8ad38fded08d01
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA512:c4127480470ef90db1ef3bd2caa444df10b50ed8df0bc9997db7612cb48b49278baf44965028f1807a21028eb965d677e015466306b44683c4ec75a23e1922cf
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.debian.tar.xz' jbigkit_2.1-3.1build1.debian.tar.xz 7672 SHA512:3ace798cf76fdebcaa1ce497910f45b5a2553e7cae902a9399f1094020b6e24a213290ca499867e681cb7a5cff00dda9c834846b7b3956f90fde90793b1155fb
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
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu1.dsc' keyutils_1.6.1-2ubuntu1.dsc 2191 SHA512:71191d68882b14f40ed4936158acb9a72c73312ff46917a4b7ece3ac1766a28b1f497043890c79d8e61899a68d4a0616c6ca1de1b649515a43c08cbc0684622b
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1.orig.tar.bz2' keyutils_1.6.1.orig.tar.bz2 97232 SHA512:ea6e20b2594234c7f51581eef2b8fd19c109fa9eacaaef8dfbb4f237bd1d6fdf071ec23b4ff334cb22a46461d09d17cf499987fd1f00e66f27506888876961e1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu1.debian.tar.xz' keyutils_1.6.1-2ubuntu1.debian.tar.xz 14364 SHA512:fcb3cf61cd6c4bb8f8dcb4f6fd19decea14642975c6fe40def1a9b36c9eb8b12bf241dedd7f10b2f7655286aa7833970b157b53f32deb48931b6d6f8f2ba5b50
```

### `dpkg` source package: `krb5=1.17-10ubuntu1`

Binary Packages:

- `krb5-multidev:amd64=1.17-10ubuntu1`
- `libgssapi-krb5-2:amd64=1.17-10ubuntu1`
- `libgssrpc4:amd64=1.17-10ubuntu1`
- `libk5crypto3:amd64=1.17-10ubuntu1`
- `libkadm5clnt-mit11:amd64=1.17-10ubuntu1`
- `libkadm5srv-mit11:amd64=1.17-10ubuntu1`
- `libkdb5-9:amd64=1.17-10ubuntu1`
- `libkrb5-3:amd64=1.17-10ubuntu1`
- `libkrb5-dev:amd64=1.17-10ubuntu1`
- `libkrb5support0:amd64=1.17-10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit11/copyright`, `/usr/share/doc/libkadm5srv-mit11/copyright`, `/usr/share/doc/libkdb5-9/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lcms2=2.12~rc1-2`

Binary Packages:

- `liblcms2-2:amd64=2.12~rc1-2`
- `liblcms2-dev:amd64=2.12~rc1-2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3 (GPL-3 for the fast_float plugin only)`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.12~rc1-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12~rc1-2.dsc' lcms2_2.12~rc1-2.dsc 1988 SHA512:bb8187b25476b3c651cc4196d8bf3e09b5fdd93647aa2d27e06328fd0703da9e40d9f9824f1edab07e3d6cf0077cf71a20e945c77a5a4481ec59532e9dd73cc5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12~rc1.orig.tar.gz' lcms2_2.12~rc1.orig.tar.gz 7417767 SHA512:1d27e6f91911053b79f2a46c6c16943e25fce2f0501bb7d97f49507522a8a0f911d60f20726fc31727fee5242c6d452c86cdc28735f8f88c3aa9676fd35fdec6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12~rc1-2.debian.tar.xz' lcms2_2.12~rc1-2.debian.tar.xz 10420 SHA512:4e99528c61f71335e336ced40cf7d29403f2e107e9fa8411fb0e109af5291560af5a130fbc33b2656892cb7d9ff5754966313c31ea91d48dcccf8b3978c6bf04
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libassuan/2.5.3-7.1/


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
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.dsc' libbsd_0.10.0-1.dsc 2197 SHA512:9dbb2fc11b3740b54edc07762b977cb38ee1b3993b87d02f964b00b04c99f3a65a4ff0c5985a4d5786bc4b8f9b795d89a46eb2d90993ea99cb710ae2c5271a3a
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz' libbsd_0.10.0.orig.tar.xz 393576 SHA512:b75529785b16c93d31401187f8a58258fbebe565dac071c8311775c913af989f62cd29d5ce2651af3ea6221cffd31cf04826577d3e546ab9ca14340f297777b9
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz.asc' libbsd_0.10.0.orig.tar.xz.asc 833 SHA512:e7b438ce96ce6d6d0afa17568700e6317ca9336fd9f5a5a5dba842d4bc4cf0426799fc4872155b881ae32a777784e1acce727a66cd0ab37b0dcf529962782a99
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.debian.tar.xz' libbsd_0.10.0-1.debian.tar.xz 16660 SHA512:66bea622de0a3c92e0bae3408554c4e4a2205669753143d929e563f94ea47c4fe68d8f8559fdb826dc2d04b53848e392fc95ec88f1a3d6aaba995d4e6e1f4c12
```

### `dpkg` source package: `libcap-ng=0.7.9-2.2build1`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.2build1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2build1.dsc' libcap-ng_0.7.9-2.2build1.dsc 2130 SHA512:ef3537c7332dafdd53720048d87caed016d3b130b113ba852d1d6d008923a88136e8427d8a47011f00cd1e4f3fe6bd2ab63bcab2b2a75787f50c5d498979ae29
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA512:095edabaf76a943aab0645b843b14e20b1733ba1d47a8e34d82f6586ca9a1512ba2677d232b13dd3900b913837401bb58bf74481970e967ba19041959dc43259
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2build1.debian.tar.xz' libcap-ng_0.7.9-2.2build1.debian.tar.xz 6352 SHA512:2b1dffd21de5f777a8eca0b553e94daf332b2be9c4934ecc47093c95a80b4082d61cfc432fdee95edb6c584e094adae8427809d2371f545c03b5e750d7d3fbd7
```

### `dpkg` source package: `libcap2=1:2.44-1`

Binary Packages:

- `libcap2:amd64=1:2.44-1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libcap2/1:2.44-1/


### `dpkg` source package: `libcbor=0.6.0-0ubuntu3`

Binary Packages:

- `libcbor0.6:amd64=0.6.0-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libcbor0.6/copyright`)

- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.6.0-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu3.dsc' libcbor_0.6.0-0ubuntu3.dsc 2115 SHA512:c15fc674e9693aab0793f69a8bc43613256c2407b2edbbf90ae444e9ef7e2fc9df294a2a375e47082cd005f3cbac519b39eaa7b6d696f77419f63c620fc8540e
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0.orig.tar.gz' libcbor_0.6.0.orig.tar.gz 262622 SHA512:6adbb32780d428140388295c5d740bd77b0ae7b21e3f73629ba56a3aa4e4ee5dbb715454061b0f6f67f2b19ea8366e0e5c24f4ffb1ba629afcb7a776a15045f7
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu3.debian.tar.xz' libcbor_0.6.0-0ubuntu3.debian.tar.xz 5960 SHA512:cb648286620df2371c86a8a0a3b7775f6bae833b885f61a8d8248793465339c0cf32473e570e41acb99f4ada686586d95e297183f6d1fd2a3583f47b11bd0fcc
```

### `dpkg` source package: `libdatrie=0.2.12-3`

Binary Packages:

- `libdatrie1:amd64=0.2.12-3`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libdatrie/0.2.12-3/


### `dpkg` source package: `libedit=3.1-20191231-2`

Binary Packages:

- `libedit2:amd64=3.1-20191231-2`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-2.dsc' libedit_3.1-20191231-2.dsc 2208 SHA512:213ea6f60df04e9a383d808f23dc805d119f583143deab5b80d07c06622d747f83913500ebbbaa21c6587a602adfef073cf95a918c2fff64cfc11a596e3c1653
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA512:1df2eced98e8db1bb0af940678c154d87e3b11dd21e65a903682367f5feace5112f9a543b8e0cb04bbfeaaf73729f808db2d9c302637fc063e81c0a37777ac2c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-2.debian.tar.xz' libedit_3.1-20191231-2.debian.tar.xz 14576 SHA512:f692bc1540d04468bc26da89844ede38f2323984a94d8c894c222f69663ab04c07241c9e9d0d9bd1a93d0a52bceaeeb7ec11525adf76d945266a1e7adcd89fb2
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
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.dsc' liberror-perl_0.17029-1.dsc 2336 SHA512:b81e1ca9f88227a083cf2b1704d8d6d6c642736ab4a355c33cd2f2a06801bd74f7163242881cdaf6579d8a5847e23ed858475a92df31b9a0763567e82022d87b
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA512:266ba1feff897c1d162e69a83e595cb40da9a6e1d8b10cc5531626eff392c6da94be03ba722c74827fc2ea0d9d1c1e62e824d9021e098b700db65dd0b3acbd0a
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.debian.tar.xz' liberror-perl_0.17029-1.debian.tar.xz 4552 SHA512:1ebfa7250e0a3698e63999117079fe951d8a6286b48884260d5207367b6b8d8ca7e2a4d390d80d28d79aa579b4e61286308536f42b5b45d9f26aa64cdd447a27
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
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1.dsc' libevent_2.1.12-stable-1.dsc 2527 SHA512:0a576f747323d12dc93e4da63dc6230a8be533f5b50d38e6f7e3420c8dba75986fe7cc30e64f212a57d7ddaa5a48b64ed7862d3cff4aafdfc25c82a4485c4642
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA512:88d8944cd75cbe78bc4e56a6741ca67c017a3686d5349100f1c74f8a68ac0b6410ce64dff160be4a4ba0696ee29540dfed59aaf3c9a02f0c164b00307fcfe84f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz.asc' libevent_2.1.12-stable.orig.tar.gz.asc 488 SHA512:841b57a0f6ba645b1871f257b9929093b11b7d6fd03332e6339adceddda233e78f6190faa2339e2b67b26dc2a56ddd7ce622792820b582168b31a2d1d1854f1f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1.debian.tar.xz' libevent_2.1.12-stable-1.debian.tar.xz 17764 SHA512:46f75a362e54dd120367009b8cd8cffb123b81855dd0cb0bd5c76610524abf92a7f439420a55d628d8e5fe0136fb832403cf034e683bb60b0637c83adb403d1d
```

### `dpkg` source package: `libexif=0.6.22-3`

Binary Packages:

- `libexif-dev:amd64=0.6.22-3`
- `libexif12:amd64=0.6.22-3`

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
$ apt-get source -qq --print-uris libexif=0.6.22-3
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-3.dsc' libexif_0.6.22-3.dsc 2079 SHA512:4dc9e9a63366fbbcd9c94c9f67194152895566d346718e4d9e08cbeac677978687a0048a142929cf1efb89243939137d8a7b54b8a7b0102786c86aae4a635218
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22.orig.tar.gz' libexif_0.6.22.orig.tar.gz 1109525 SHA512:6c63abe2734c9e83fb04adb00bdd77f687165007c0efd0279df26c101363b990604050c430c7dd73dfa8735dd2fd196334d321bdb114d4869998f21e7bed5b43
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-3.debian.tar.xz' libexif_0.6.22-3.debian.tar.xz 12468 SHA512:87dfece8707e44e99ffc9d08560e55d6b6f6806ca6f1a07a9646631e46b7508cf637590b02821299a98034afd0ac805b80105752199bff0c39f024945879ab88
```

### `dpkg` source package: `libffi=3.4~20200819gead65ca871-0ubuntu3`

Binary Packages:

- `libffi-dev:amd64=3.4~20200819gead65ca871-0ubuntu3`
- `libffi8ubuntu1:amd64=3.4~20200819gead65ca871-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi8ubuntu1/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4~20200819gead65ca871-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu3.dsc' libffi_3.4~20200819gead65ca871-0ubuntu3.dsc 2179 SHA512:3daf83b86b96208b825523ccdbb3900fe00d189b87811b57d661a3ab43e3b9e5b631ccb7fd2723a2df655b56c643fa0e2733c35f08c2732756eb59852bc85e00
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871.orig.tar.gz' libffi_3.4~20200819gead65ca871.orig.tar.gz 527371 SHA512:c349b1630db80c042f3c11efe58d4eb849e87f2cca0cc1748c99d32cc34ce4c1262825dc070c8a84263e0adcd8a7af3bd33c705ba28b6cc16974552b12bf0c65
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu3.debian.tar.xz' libffi_3.4~20200819gead65ca871-0ubuntu3.debian.tar.xz 7856 SHA512:5496d2d4147aa2ca5e579c149206d2cb1db39f14f7d351b4224496b3289b68f83a8715366bcad933fa798815e8aef416270c77576aaca2a921a7ae5c4b8abb3e
```

### `dpkg` source package: `libfido2=1.6.0-2`

Binary Packages:

- `libfido2-1:amd64=1.6.0-2`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.6.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0-2.dsc' libfido2_1.6.0-2.dsc 2565 SHA512:37bb1caa75b306ae625779cb39315b75b3aed32d131103b78706188a7c062762ad9bec7dc1ddcf510e463900f4311165e5b50a284cdf6bb51d1a9d1bac1d2f4a
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz' libfido2_1.6.0.orig.tar.gz 413904 SHA512:c473732a2f7ef54156097d315e44457d89056446ab3112a7c7a6fd99d5c2c8ae0ca2451ff9cd45be6c32de1ab335d6dfdb2b0c56b40cae9eb41391d18d83be4a
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz.asc' libfido2_1.6.0.orig.tar.gz.asc 488 SHA512:ea6b2191bbbce3b1e905a6835cc05f38571f65d3590984e1591a1b630bafa29c646a4c813cc5761cf3013b41da1246a70037eaa7aeefe3daf7740a468cc99d4f
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0-2.debian.tar.xz' libfido2_1.6.0-2.debian.tar.xz 72700 SHA512:c890d377b53a2ef686d40aa07af0e2ead25ad217dd5692bbcf29f246b6672eb4aed53afc6bbbdf1b3a4c0e2ad6f778a7bdb43ff72eb708c7c404feedf2ff0e54
```

### `dpkg` source package: `libgcrypt20=1.8.7-2ubuntu1`

Binary Packages:

- `libgcrypt20:amd64=1.8.7-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.7-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-2ubuntu1.dsc' libgcrypt20_1.8.7-2ubuntu1.dsc 2562 SHA512:88426b8f8ca1a9d5c994f0c4674b9b573ee0085dade3a746480b8ffe1f10eed8a41921aef32e3d63dc5ebce21eb1f315d2bd5acb1b41f07c573300b9f3b765d6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2' libgcrypt20_1.8.7.orig.tar.bz2 2985660 SHA512:6309d17624d8029848990d225d5924886c951cef691266c8e010fbbb7f678972cee70cbb91d370ad0bcdc8c8761402a090c2c853c9427ec79293624a59da5060
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2.asc' libgcrypt20_1.8.7.orig.tar.bz2.asc 228 SHA512:4ba6875dfddbc9bece0c4d25d1c3b0e6183045288ca876b84c24d487ee72f751ecda6eaec71e70ba00fd2434c77127283af1a957ac9e6f40352ef67add672c72
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-2ubuntu1.debian.tar.xz' libgcrypt20_1.8.7-2ubuntu1.debian.tar.xz 35228 SHA512:5524a6e5be504282ba095cdd4ddf49ef0ddca85f7833c562b97d481849b9ad6d7c8efc06011e17030142041a1f1f5b6dadb0a1b4d251e78769ad75250a7a4f56
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libgpg-error/1.38-2/


### `dpkg` source package: `libice=2:1.0.10-1`

Binary Packages:

- `libice-dev:amd64=2:1.0.10-1`
- `libice6:amd64=2:1.0.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1.dsc' libice_1.0.10-1.dsc 2049 SHA512:61fda8a2a78b9c1845666f20eab37a3fb5b806f11cd4b959ad084b47640e41740fc1876596a00316a3687ccccb70c0903595396962930e0228d0f20ed57b54e0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10.orig.tar.gz' libice_1.0.10.orig.tar.gz 481960 SHA512:2d4757f7325eb01180b5d7433cc350eb9606bd3afe82dabc8aa164feda75ef03a0624d74786e655c536c24a80d0ccb2f1e3ecbb04d3459b23f85455006ca8a91
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1.diff.gz' libice_1.0.10-1.diff.gz 11349 SHA512:e8709dffbedbfa0e07896f0176e57c91da571a7eef143492c0815092d8615756a55c4144460c62d6a06f8cc9c5d8b4975b7e62a4ebd82f3ee89d6cb315d4f187
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-5.dsc' libidn2_2.3.0-5.dsc 2046 SHA512:51847de90ee22664bc7ccfdf5195a12b30fc7869613da3321e455edf5ae2a1bd8016c3aeb42e740ca884d7f51a8d140bbd18e1fc5064278ac5e49b8162031618
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0.orig.tar.gz' libidn2_2.3.0.orig.tar.gz 2164993 SHA512:a2bf6d2249948bce14fbbc802f8af1c9b427fc9bf64203a2f3d7239d8e6061d0a8e7970a23e8e5889110a654a321e0504c7a6d049bb501e7f6a23d42b50b6187
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-5.debian.tar.xz' libidn2_2.3.0-5.debian.tar.xz 11276 SHA512:de212b412088d7a868377f90f45d791646101c5e9d4aadf659c7917c74afb68b1b19ec3193f5997527d69f0b5e5739452852021b8e50a9b880c229f9dbfc13ab
```

### `dpkg` source package: `libjpeg-turbo=2.0.3-0ubuntu2`

Binary Packages:

- `libjpeg-turbo8:amd64=2.0.3-0ubuntu2`
- `libjpeg-turbo8-dev:amd64=2.0.3-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.dsc' libjpeg8-empty_8c-2ubuntu8.dsc 1637 SHA512:294caa2f8c916f07fa653469c239f46304cabd9d0194c7f0b311027bf2b09d45e07d6b5bc7bbdd11920e574040ad2b45f3af092d90009a119916a4a4857e0dd6
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.tar.gz' libjpeg8-empty_8c-2ubuntu8.tar.gz 1770 SHA512:07407b8f295f07df0eff6a4384cba7bc11349a1cacf488422b6a20bcbe5cb0ef9809bf847f3e52304a8f092e3581ac40adb745d9281fd4c83edd79f4c7cc8111
```

### `dpkg` source package: `libksba=1.5.0-3`

Binary Packages:

- `libksba8:amd64=1.5.0-3`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.5.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.0-3.dsc' libksba_1.5.0-3.dsc 2470 SHA512:8e8e54a5de8f765000e2448dbb9782f074edf97f7da65b7f67e3e9634aeccc3bdeab505732396322c5db89f821a9e6390307416c331c5e59306effb8610761d7
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.0.orig.tar.bz2' libksba_1.5.0.orig.tar.bz2 656518 SHA512:84383e8b084bf47ac646a9aacb174e510ffcab4b966b649e4351990eaf7ce78cc9d199e6c4f3a1be697888c857ee86ecef949c06156790c7d8d0bd0fb0142721
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.0.orig.tar.bz2.asc' libksba_1.5.0.orig.tar.bz2.asc 228 SHA512:04f2ebeb83ee672b67542ff1c068f0e61bbea61b3917dd9e7af5fceb85e2e4dec191cf1e487344e50f26893c4b9045ba7f21cc6968b4ef675a2407681b856aaf
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.0-3.debian.tar.xz' libksba_1.5.0-3.debian.tar.xz 14300 SHA512:b14715e441a62f7ffefa437a906344d08c85cda12c74978b1927b0d01fbb10fbac59bbbaaeddb5bbddece546e05974e154c9497ea6f104df143f6f25e324211f
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
'http://archive.ubuntu.com/ubuntu/pool/universe/libl/liblqr/liblqr_0.4.2-2.1.dsc' liblqr_0.4.2-2.1.dsc 2095 SHA512:ef20fa2551ce6399f0ecc42301c2d0292d624f4fd9252fd901d58d67ac7325f128cd5209661fe456dda31e4efbb6b48a80415a1b34f815dd7511eeb24e924d36
'http://archive.ubuntu.com/ubuntu/pool/universe/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA512:acfa5868c41ea145092711e84d6c9eb62cb725b3d7531917b0d91b7d4af2a9912b18a96edc2594a826f09dabe0a0a82936ceea7d1f31301a23d558b1450d2547
'http://archive.ubuntu.com/ubuntu/pool/universe/libl/liblqr/liblqr_0.4.2-2.1.debian.tar.xz' liblqr_0.4.2-2.1.debian.tar.xz 5300 SHA512:ba8ade073057be2c5b065d92c0a119049cb67b382ebbf6c2b8c59b1aec52bd60fd6c313c0a2e8d83f39e9733477b615c7a646c47ca9dbbe3c8469ff86078c027
```

### `dpkg` source package: `libmaxminddb=1.5.0-1ubuntu2`

Binary Packages:

- `libmaxminddb-dev:amd64=1.5.0-1ubuntu2`
- `libmaxminddb0:amd64=1.5.0-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libmaxminddb-dev/copyright`, `/usr/share/doc/libmaxminddb0/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `CC-BY-SA-3.0`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libnsl=1.3.0-0ubuntu3`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-0ubuntu3`
- `libnsl2:amd64=1.3.0-0ubuntu3`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-0ubuntu3.dsc' libnsl_1.3.0-0ubuntu3.dsc 2062 SHA512:b0f64be153bc9cc1afd5c1880fec6eda0c8026e18442565696248d4876c781ac94f04124e748ae359e2b38b2b90fbe5b21b064685c7c5bea48baee06d15d9aa2
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA512:a5a6c3ccb2d1e724c8c1f65e55dcd09383eb1ae019c55f4c09441eadf23ffbc2196cfad259805b0ac40ddf3a10af0da453e4d739d67d46829c64d0995dab4e55
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-0ubuntu3.debian.tar.xz' libnsl_1.3.0-0ubuntu3.debian.tar.xz 4740 SHA512:48723ab4335103b3371f8706e78150cdd35a5d3fcd32800cb27d5152aacf10f65dc148c77f8320f43f53e591d0a1b7266cc03e28d2526d95b0a9025283c777c2
```

### `dpkg` source package: `libnss-nis=3.1-0ubuntu4`

Binary Packages:

- `libnss-nis:amd64=3.1-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libnss-nis/copyright`)

- `BSD-3-Regents-DEC`
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
$ apt-get source -qq --print-uris libnss-nis=3.1-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nis/libnss-nis_3.1-0ubuntu4.dsc' libnss-nis_3.1-0ubuntu4.dsc 2052 SHA512:d8c1e8baaf5f903e94aae3f332987f98ede739635457d739ad7d2c083fa98ca26862a53730828d57b17ac69fde49c28ed7cba0fd26efd5f2049981766fb8f291
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nis/libnss-nis_3.1.orig.tar.xz' libnss-nis_3.1.orig.tar.xz 257440 SHA512:3743730aeaf98011d40c0d242f34967ab382d586bbe8da1eb5b3698070c73ca967bbb6dc9dfac0e4c5074a293e0d3f009bfd44c2a50aeb648d65ffd0d6468715
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nis/libnss-nis_3.1-0ubuntu4.debian.tar.xz' libnss-nis_3.1-0ubuntu4.debian.tar.xz 4644 SHA512:5e2e042fed93d7eeac81d969be5cdf08eed67a45d370db2df24439ade08c495c8f0d4ec80fee677e6ba8d4d908d940933781472c6adf60a202718ff5a0d4b8f2
```

### `dpkg` source package: `libnss-nisplus=1.3-0ubuntu4`

Binary Packages:

- `libnss-nisplus:amd64=1.3-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libnss-nisplus/copyright`)

- `GPL-2`
- `GPL-2+-libtool-exception`
- `GPL-3`
- `GPL-3+-autoconf-exception`
- `LGPL-2.1`
- `LGPL-2.1+`
- `permissive-autoconf-m4`
- `permissive-fsf`

Source:

```console
$ apt-get source -qq --print-uris libnss-nisplus=1.3-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nisplus/libnss-nisplus_1.3-0ubuntu4.dsc' libnss-nisplus_1.3-0ubuntu4.dsc 2086 SHA512:0cab077dde1c0eb3889bb13bcdea282fd5426ecfc52ed0db6f5aad559c1dd7ffee0ccbb9bd8948e0ca9509986497e6227ed7a54aba108baf6e46b655e28fdcb4
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nisplus/libnss-nisplus_1.3.orig.tar.gz' libnss-nisplus_1.3.orig.tar.gz 203693 SHA512:bccfee33c7ab69b2b3db6b6bc35509791ef958f9a776b1b5bbd11c35c53f2a07deb80c64344956fab1d67d69545f3fa730fc8decedd3c75a435f72c805b3e906
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nisplus/libnss-nisplus_1.3-0ubuntu4.debian.tar.xz' libnss-nisplus_1.3-0ubuntu4.debian.tar.xz 6452 SHA512:193ee5902866b75207ea3915477f16ba4f33ae935712ae28f13c32a82342e9ae4d1093aebed132ee04d07a983e50c04c6510e34446c93e11ad0f9a7b737371b1
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3.dsc' libpng1.6_1.6.37-3.dsc 2225 SHA512:25bb2f81e07ea84b5d462a435154c632e33f4ffcbc4b326cdb90e805fb322c55ac10baad1a8599e99c30f526fbaeb68691916a5e5cb21e9b8b401856c956eb5c
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA512:ccb3705c23b2724e86d072e2ac8cfc380f41fadfd6977a248d588a8ad57b6abe0e4155e525243011f245e98d9b7afbe2e8cc7fd4ff7d82fcefb40c0f48f88918
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3.debian.tar.xz' libpng1.6_1.6.37-3.debian.tar.xz 32272 SHA512:572781fe5581cbff3a140922bb611e84d44511256d766b85b4e334a47afc3ffbb7d60f96068945efb7e9e4f3d92b8beb63593dab8752d85182c6ecc26907ef37
```

### `dpkg` source package: `libpsl=0.21.0-1.1ubuntu1`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libpthread-stubs=0.4-1`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.dsc' libpthread-stubs_0.4-1.dsc 1927 SHA512:890812cdb72381fbae09d2273cf80fe751097ed1595b065d1ed1f789a7115ccb559fa96d729785226dfefcab84be0826478541f483f81454922adfc1d91d4278
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4.orig.tar.gz' libpthread-stubs_0.4.orig.tar.gz 71252 SHA512:5293c847f5d0c47a6956dd85b6630866f717e51e1e9c48fa10f70aa1e8268adc778eaf92504989c5df58c0dcde656f036248993b0ea5f79d4303012bfeff3c72
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.diff.gz' libpthread-stubs_0.4-1.diff.gz 2346 SHA512:bd46c806b16fe18162078eda8778319da4ca672877eea3c255747b5f0d12dc23bc43ba27dd2ae2d2d7edabc83c285855d5efe694db709fa896a598c97e1475c7
```

### `dpkg` source package: `librsvg=2.50.2+dfsg-1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.50.2+dfsg-1`
- `librsvg2-2:amd64=2.50.2+dfsg-1`
- `librsvg2-common:amd64=2.50.2+dfsg-1`
- `librsvg2-dev:amd64=2.50.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `0BSD`
- `0BSD,`
- `Apache-2.0`
- `Apache-2.0,`
- `BSD-2-clause`
- `BSD-2-clause,`
- `BSD-3-clause`
- `BSD-3-clause,`
- `Boost-1.0`
- `Boost-1.0,`
- `CC-BY-3.0`
- `Expat`
- `Expat,`
- `LGPL-2`
- `LGPL-2+`
- `MPL-2.0`
- `MPL-2.0,`
- `Sun-permissive`
- `Sun-permissive,`
- `Unlicense`
- `Unlicense,`
- `zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/librsvg/2.50.2+dfsg-1/


### `dpkg` source package: `libseccomp=2.4.3-1ubuntu6`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libselinux=3.1-2build2`

Binary Packages:

- `libselinux1:amd64=3.1-2build2`
- `libselinux1-dev:amd64=3.1-2build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.1-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-2build2.dsc' libselinux_3.1-2build2.dsc 2680 SHA512:a65e54000b657a729b4cc1a232a74b250e9d84ddf791d2e03f83716c3af9dd4edd0f8a4955a8d92c0f32f72bf38924cf0b4e823f6a3852011f09dc8ed00772c0
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1.orig.tar.gz' libselinux_3.1.orig.tar.gz 204703 SHA512:57730cddd2d4751556d9e1f207c0f85119c81848f0620c16239e997150989e3f9a586a8c23861fd51ed89f7e084ad441190a58a288258a49a95f7beef7dbbb13
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-2build2.debian.tar.xz' libselinux_3.1-2build2.debian.tar.xz 23880 SHA512:bafa346a9073c0217d4280c80f76dce69a23bfdaa66c9d61a0ec209e5ed651c0f0f9e20e3669ac751ae86ae157772a5403914bc033b49f00ed72c51fe694c718
```

### `dpkg` source package: `libsemanage=3.1-1build2`

Binary Packages:

- `libsemanage-common=3.1-1build2`
- `libsemanage1:amd64=3.1-1build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.1-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1build2.dsc' libsemanage_3.1-1build2.dsc 2709 SHA512:787fc82be0ae8194391e445ff6d945d97f2e3ce6f00c730cdf0a70aaad01a46fc2dc8b9a48c171e5f804fc60a48500f288b328ae69cd7cc725a3ad95a2866fe7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1.orig.tar.gz' libsemanage_3.1.orig.tar.gz 179601 SHA512:8609ca7d13b5c603677740f2b14558fea3922624af182d20d618237ba11fcf2559fab82fc68d1efa6ff118f064d426f005138521652c761de92cd66150102197
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1build2.debian.tar.xz' libsemanage_3.1-1build2.debian.tar.xz 17656 SHA512:ed65d10f4cb6b3b96f6dcb7e5ead6cdc8ed46ca91c692231843f4cd8414d0ad2fcb962424dbe0f7d38ad4cc0ef27da3b70f42c3f6103548dea487af5c8860b45
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
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.dsc' libsepol_3.1-1.dsc 1776 SHA512:74a0dd6f3db6578261b78114f46030cd0486b05d0482421bacb5a74a30cbdc98932691c60293d96e5fd258839136d8e0988eb0371cbd6e685b6bce38e0a95bc7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA512:4b5f4e82853ff3e9b4fac2dbdea5c2fc3bb7b508af912217ac4b75da6540fbcd77aa314ab95cd9dfa94fbc4a885000656a663c1a152f65b4cf6970ea0b6034ab
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.debian.tar.xz' libsepol_3.1-1.debian.tar.xz 14584 SHA512:e7c48cde2e2d8748f4df3b6b02c66ffb97ee21c2b749b2d7c9154ac4d4c73fd09a383972ac39edcb6f04faf2631c1dba3512b6622b612e1aec54bc58608df5db
```

### `dpkg` source package: `libsigsegv=2.12-3`

Binary Packages:

- `libsigsegv2:amd64=2.12-3`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libsigsegv/2.12-3/


### `dpkg` source package: `libsm=2:1.2.3-1`

Binary Packages:

- `libsm-dev:amd64=2:1.2.3-1`
- `libsm6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1.dsc' libsm_1.2.3-1.dsc 2063 SHA512:3453c5c83ee34a008a1674dfc347d6270a51e5e2b2da90cc0b3e9a2f8b5f6524248541123dcac1cb7a14e35f5546dc3c514ae5bc1f74748b3b9f986a34b88f4b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3.orig.tar.gz' libsm_1.2.3.orig.tar.gz 445362 SHA512:03b77d86b33cdb3df4f9d65131a0025182f3cb0c17b33a90d236e8563b3011d225b9d006186302d07850edafa5b899aec6a086b8d437d357cd69fedd5f22d94b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1.diff.gz' libsm_1.2.3-1.diff.gz 8929 SHA512:5cd42b75eabce2c66baa2f22f808f219ef70635e67405743c62d814dd0c1f1a78f2a09e4a5c08ba0e1574a2f07d2161af455e454077ebfa02ab2eb7e9269a362
```

### `dpkg` source package: `libssh=0.9.5-1`

Binary Packages:

- `libssh-4:amd64=0.9.5-1`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5-1.dsc' libssh_0.9.5-1.dsc 2364 SHA512:8b0f2c4fa628db7866ff4b433a94e7ec6c3e03cb961a4d3b7b3d4fadb9c84a9459c2c7fce2b37878b47fbcfb1e3f303589963f324fb8a56cb32a8c0ebe8a35d6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5.orig.tar.xz' libssh_0.9.5.orig.tar.xz 502876 SHA512:64e692a0bfa7f73585ea7b7b8b1d4c9a7f9be59565bfd4de32ca8cd9db121f87e7ad51f5c80269fbd99545af34dcf1894374ed8a6d6c1ac5f8601c026572ac18
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5.orig.tar.xz.asc' libssh_0.9.5.orig.tar.xz.asc 833 SHA512:f0b76cdccf26144b9cc9ad3f7e1605b50473fc5c686d0d9a2419b13382440776c09428d717253a918f7347b90e4a562fd88d8ea85a6e54f06b149826295b4f8e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5-1.debian.tar.xz' libssh_0.9.5-1.debian.tar.xz 27056 SHA512:3c77003311004858f9972ec7ec5c7b4aa379c174083fc946c2671868b480bb8cc87e9bebde50a02165f78dca5e3f283fc93874ae523c42b0e15ad166e9ca4b05
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
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.dsc' libtasn1-6_4.16.0-2.dsc 2586 SHA512:a35e22dbbf29f7f6fb81800d6f8f43561d7b4676082b3ce4c6cac1c1ff16371771d8675983eb6eadf93a40375160a6d07522d4561f73556010e7471adfd66f18
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz' libtasn1-6_4.16.0.orig.tar.gz 1812442 SHA512:b356249535d5d592f9b59de39d21e26dd0f3f00ea47c9cef292cdd878042ea41ecbb7c8d2f02ac5839f5210092fe92a25acd343260ddf644887b031b167c2e71
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz.asc' libtasn1-6_4.16.0.orig.tar.gz.asc 488 SHA512:53254c2ce61e9bb889fe00b43ef2130ab9f122c44832538e3f7b38cb75ada1656213cf5c8c85321078c6b98d325c46eff41ea64d1971d3183f2ec568a18f7ed2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.debian.tar.xz' libtasn1-6_4.16.0-2.debian.tar.xz 17740 SHA512:4803d8de62ab8a579b4707faa701bf3dd767049788c2dbcf32e2845b69a84b15df5987c4314b8bf5962be6ad1d1b015348d9a0a97a8c8c7a2d62fd32891b008d
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libthai/0.1.28-3/


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libtirpc/1.3.1-1/


### `dpkg` source package: `libtool=2.4.6-15`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-15`
- `libltdl7:amd64=2.4.6-15`
- `libtool=2.4.6-15`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-15
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-15.dsc' libtool_2.4.6-15.dsc 2502 SHA512:7315ff050096ea5a250889f4cc853307e3f8b3fb1ad3fc903979415b67be7621c20ede7f0f9f09c6975d3510a4512924888ad27312d10ea976a6d0f27cc488a5
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA512:a6eef35f3cbccf2c9e2667f44a476ebc80ab888725eb768e91a3a6c33b8c931afc46eb23efaee76c8696d3e4eed74ab1c71157bcb924f38ee912c8a90a6521a4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA512:2f26447a837e3242b8f8f38fbab22d89df0949ee62fd966af3b5bae3aa939ba53bc4621174ee58d1c6722d569d7fe5f90097ddccffed28c3067fe5fa996fcb89
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-15.debian.tar.xz' libtool_2.4.6-15.debian.tar.xz 53924 SHA512:5cffe71b101992e73051a4563c4afab2a32270daaf212b2299eb33fb1a843db3032bac02b35c7ae6a2ff54f044d14a4b7d64026f5fbf0f425a8f3de49bf8a498
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
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.dsc' libunistring_0.9.10-4.dsc 2212 SHA512:498003f18665d5b50c34a5bcaa6d13dae65673d99671e5256e3500aeeae35710dad7e08c1f3ab20adb37ba10ca9b36a6916068cc3425261e734b5ecc25e78bf8
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA512:01dcab6e05ea4c33572bf96cc0558bcffbfc0e62fc86410cef06c1597a0073d5750525fe2dee4fdb39c9bd704557fcbab864f9645958108a2e07950bc539fe54
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA512:94d4316df1407850f34e84064275ae512d1ee1cd519420e2342a3f36c17d1ff7fa4019fea64507a04034ffc356c0c9add94a5abf756dd5995913583f68cfe0bd
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.debian.tar.xz' libunistring_0.9.10-4.debian.tar.xz 40936 SHA512:b687df5ffae03ad5de8c2ee42b566946c2164574a78801a55ca1a4ee61d602007de002f5c996b7b408bf8793706061b6339657b50db305811e543e24de87516e
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
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.dsc' libwebp_0.6.1-2.dsc 2064 SHA512:9f3c66da0131970aecf045d013c68b5fec79bc1fcacdd90f0350edd1137b6b0cc1b148e754ef32d7c935251c80504620b957965423741ad89cb1361e3da6a6f6
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA512:313b345a01c91eb07c2e4d46b93fcda9c50dca9e05e39f757238a679355514a2e9bc9bc220f3d3eb6d6a55148957cb2be14dac330203953337759841af1a32bf
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.debian.tar.xz' libwebp_0.6.1-2.debian.tar.xz 9532 SHA512:c1a18ec35b059f40a1303f3ad2bffc448bc666f54a7d7306ccc7cdc579b6495f121111f600108bbd732f6050b07d43a443b412968482a12b37348c40a22b0963
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
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu1.dsc' libwmf_0.2.8.4-17ubuntu1.dsc 1642 SHA512:574cc44e7e7bb4936ee5b2269e6f83bafcac8ba7ffb37e2f56e9e476d2bf8720ae937adc1676ffa1dea2241766e2a2af7ac4d88b3be5c9a8d452951edafc0c17
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA512:d98df8e76a52245487b13e5ab3d2fbba9d246f97ee04a7344c0e5861bb2d0f990fc6d662dbd849ce621768b06eaebd4270fb34bec4ee004334a98b14ba6044a5
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu1.debian.tar.xz' libwmf_0.2.8.4-17ubuntu1.debian.tar.xz 12968 SHA512:7f5119e8e78973b6739ff6314239a7348e49e2e9cfd71d40c16b6c30e3de82c022252b197094536db1acf950a5216a0be19b44c651af8083515661535c998673
```

### `dpkg` source package: `libx11=2:1.7.0-2`

Binary Packages:

- `libx11-6:amd64=2:1.7.0-2`
- `libx11-data=2:1.7.0-2`
- `libx11-dev:amd64=2:1.7.0-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.7.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.0-2.dsc' libx11_1.7.0-2.dsc 2564 SHA512:088dd632cf8329187542f5c4435285584736adea43af2b81768ebc00ceee3690b46c60d5233e63d1dcb4d4cbe6fd697e06bb116dcd03d0720502a292a1bd907b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.0.orig.tar.gz' libx11_1.7.0.orig.tar.gz 3165477 SHA512:bc7162ae29e1d23deb9b8b0c25ca072511f4b35dec7fe4e8e9a103edea350b0dc1ed46ed0ea1ff674ef6570766acbed5e811c697784068163c37bc8562e3e400
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.0.orig.tar.gz.asc' libx11_1.7.0.orig.tar.gz.asc 833 SHA512:8700023de23b730d17c3dd590cfba2d6ae5f200644442942d58f3e59401826946ddc6002df7cf0c726d848bced27cabf1be8695312731c62c1dd671118da2fa2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.0-2.diff.gz' libx11_1.7.0-2.diff.gz 73844 SHA512:368e3897087819231229d30de5e86b8a6e4da74982c7d62d7e4d5495fcec7cdcfee96af3becaf7c4b44a511221adb23e623011812e14512878c616c719a47346
```

### `dpkg` source package: `libxau=1:1.0.9-0ubuntu1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.9-0ubuntu1`
- `libxau6:amd64=1:1.0.9-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libxcb=1.14-2.1`

Binary Packages:

- `libxcb-render0:amd64=1.14-2.1`
- `libxcb-render0-dev:amd64=1.14-2.1`
- `libxcb-shm0:amd64=1.14-2.1`
- `libxcb-shm0-dev:amd64=1.14-2.1`
- `libxcb1:amd64=1.14-2.1`
- `libxcb1-dev:amd64=1.14-2.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.1.dsc' libxcb_1.14-2.1.dsc 5377 SHA512:0631b4fe9a73e0d14b8ab5fd03a2ed3662f33c9140f2b2203eb9cdb2c611322b833a022bc96a5110844ad85ff1f91a2ade53acda752dc94558cf91db65257071
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA512:6114d8c233b42b56604787a0475e924143aa13f1d382e6029b2150a4360c12ce78073409f754fbb1e5d9f99fc26900c0a4c59e9cfbd4c3d0a3af0c1306e62da1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.1.diff.gz' libxcb_1.14-2.1.diff.gz 26530 SHA512:4747b016863e58732e6dc781f31f8fbd373993edb28543bf17dff609e9ac4c96f3a0b49e275d262d0da944a4350cca7564fdff05b23d3245010f41cb58238323
```

### `dpkg` source package: `libxcrypt=1:4.4.17-1ubuntu1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.17-1ubuntu1`
- `libcrypt1:amd64=1:4.4.17-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.17-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.17-1ubuntu1.dsc' libxcrypt_4.4.17-1ubuntu1.dsc 2212 SHA512:7c62dfc3c97092c40ec25518dcd209e15bfd24065b926899db92c92f1cc73c8dc3eda17857054e94796caef4e7d502bb2eeac3844bc510e7b75d56243eeecd98
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.17.orig.tar.xz' libxcrypt_4.4.17.orig.tar.xz 389052 SHA512:a9b921db249394f7224b39ba4630bc3365f071fd647a5148510225d92801da40aa6dc81a128272cdab5ea84b67e19bda37707e5297a94410655b6e4984374bef
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.17-1ubuntu1.debian.tar.xz' libxcrypt_4.4.17-1ubuntu1.debian.tar.xz 5880 SHA512:1a070319bacd05ce7b576cf3db84ad4236d317e2c0fb074de17376b372ce4e01b9ee6f4282a8becbe02978e1faa4abad64a5958274d4297cbda6a79ed82c0f57
```

### `dpkg` source package: `libxdmcp=1:1.1.3-0ubuntu1`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.3-0ubuntu1`
- `libxdmcp6:amd64=1:1.1.3-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libxext=2:1.3.4-0ubuntu1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.4-0ubuntu1`
- `libxext6:amd64=2:1.3.4-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.dsc' libxext_1.3.4-0ubuntu1.dsc 1727 SHA512:504328765410e07377746da12489f06f58dedf3ed390a83c10e9550cd39515fba9240245885e3d45be3fd412ec629ea4770e28e8f80dfe3db63f40665b373844
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA512:4eebd639fd57cb9b84a1e17e368f82fbf3d9f021eef5ad3fe31dd128500db57862a82c1e0d214d447cb7641b2be3fd7e949ee1196f2a482793c6628fb1e5cd70
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.diff.gz' libxext_1.3.4-0ubuntu1.diff.gz 20663 SHA512:bbfb69ff7175641e6c2f2e0b5ae449d56f4a7822ad9273616514cb632dea70afcff7c461510b528e2fa1c5000fb738a2279c9787fae4d5cfe3a97a3a6f769976
```

### `dpkg` source package: `libxml2=2.9.10+dfsg-6.3build1`

Binary Packages:

- `libxml2:amd64=2.9.10+dfsg-6.3build1`
- `libxml2-dev:amd64=2.9.10+dfsg-6.3build1`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.10+dfsg-6.3build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-6.3build1.dsc' libxml2_2.9.10+dfsg-6.3build1.dsc 2721 SHA512:8741ad74e53b0ce1972b1f97e38d93eaef9c3430d2de462345d2a95bd116bdfa1d8138292fb94635efc428f251cd0d014afd5bcc36f6e3a151d96fc37c4c76e4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg.orig.tar.xz' libxml2_2.9.10+dfsg.orig.tar.xz 2503560 SHA512:605c6c0f8bf2c53208d0a036ff09a4025843f45139b711c90dc83066feda2f285a5578d55d4a58d33eedbe7485a5c1ec5608ba6c6beed1fb55649f87dca0cec3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-6.3build1.debian.tar.xz' libxml2_2.9.10+dfsg-6.3build1.debian.tar.xz 29936 SHA512:6de6c51f4b7351432ad06ef859d24bcfc0daf9919c3819e1e1d9e374a1158d03ac38308f6846fa740db758521862f42cd1485e867985e41c9d4394e198eecca5
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
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.dsc' libxrender_0.9.10-1.dsc 2064 SHA512:3ef4856e738e1cc30ea8872845c88ea8f4918682137299a38c8ec33059c4ebd7ae8ec5ce6c658b9e287587356c696cef5dbae1eaaf9380b1b2448f459eab4c70
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA512:7768e62b500f468460f88f27bc1130170b204b478573d9e4406867e557b5638b7c1e21d88d51f9e774ce2344780a384e3c3be51421275d2ee880f9a978a3a232
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.diff.gz' libxrender_0.9.10-1.diff.gz 15399 SHA512:031cff19410477b6e3ff2e9b195ba46a5047fd2263ea19b7276b9fa347817e90c4ba93aa97ca71eb7318385b40d85994b1b04a3664ab1bc1982be8026853908f
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
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4.dsc' libxslt_1.1.34-4.dsc 2375 SHA512:dabcebd926e3f02a3f617bfe06dfeeaf32b01c902cd80a1c03b772f03f98609eb6dc4729432d0a7289f8aeea02ba31e8d7dcbb046b062a73c085f70ab6bfef09
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA512:1516a11ad608b04740674060d2c5d733b88889de5e413b9a4e8bf8d1a90d712149df6d2b1345b615f529d7c7d3fa6dae12e544da828b39c7d415e54c0ee0776b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA512:9b155d4571daede99cdbf2813a85fb04812737b5e23d3f7c9840225b38f3dbf171623a21645daaee190e7ff9ba38bde932922e96a2a2312c203ffa9917c3baea
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4.debian.tar.xz' libxslt_1.1.34-4.debian.tar.xz 21464 SHA512:dbd4104503a3eee856bf42c0a55e78de3687578498c4ab6dac889e787997a1a2fc9d95a0ea7acee37fa6e31e3f79bd791a176eb2f616fa5a8886008fe87b53ce
```

### `dpkg` source package: `libxt=1:1.2.0-1`

Binary Packages:

- `libxt-dev:amd64=1:1.2.0-1`
- `libxt6:amd64=1:1.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0-1.dsc' libxt_1.2.0-1.dsc 2298 SHA512:68dcfae9bc0ba85aab25d6be62cdd8f5ac1bbcd79428f9def8fa4058befbf4b52b3da85e84f94b0a55ea4c3f37afcaf27344e61f7e1da07df0eae8e7829a1b41
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz' libxt_1.2.0.orig.tar.gz 1016961 SHA512:af8147becd98c956e9324b765151f46352cafa1f962c7d1517b18b5d27aa80d093cc3ceabd92c0f181485540987b7e46b18baf38ffe1eadf3f60ab66c3f66c52
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz.asc' libxt_1.2.0.orig.tar.gz.asc 195 SHA512:a105f63f0fdcdddea75024e869dbe271d4261703616d5d2a3393943bf20b72fc70e9c52382dcc0370d2460737fda6f4bcaac3fa7eb84e2f6e234aa358758a13a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0-1.diff.gz' libxt_1.2.0-1.diff.gz 31129 SHA512:de872120880bf38ea2aa362f4e53e0cc84ed7e147c760183ca0f77797d9e0042070fa2c16613ec23a08bc193ecb9c5a12cedbf87ead5483c6c574b25a9f750dd
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
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.dsc' libyaml_0.2.2-1.dsc 1833 SHA512:376309b84fc5e119aee97cc8cdfbf2bcc83b9f09d3967a78ee8beee47c391d89580df1d492dca8d4d81549958e546e802a42c10bf7d902e00074134ae659c063
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2.orig.tar.gz' libyaml_0.2.2.orig.tar.gz 602509 SHA512:0728c89ba43af3cdec22bccaf18c9ad7b07e13cdebed9d8919e2c62cf90bb5e23d2c746fd250320b2827dfcd9f1ce442d3bf8a3fe18b61f9a8d1d7770561e610
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.debian.tar.xz' libyaml_0.2.2-1.debian.tar.xz 4112 SHA512:39c4a9bbb5bc5602e4672ce1ff74b8e85e90fcb86efd2623face9692a525a91a1bc449a45ac0e241eedce4e677aa9be3ef13784ebac868a14f78e41c3ae6f9cb
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-1.dsc' libzstd_1.4.8+dfsg-1.dsc 2291 SHA512:70338b82c4a63442ad69bb8c240c0783e0ba5c6e6e1dbcdca8e0a99f72b6d89d82bbe19131ccb11ae2d5fbb24af99a7b0212c52462c321b43a9cbdc359a1718a
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA512:07fabe431367eea4badae7b1e46ac73e0b33aad5b67361bc7b67d5f9aef249c51db5b560f1cf59233255cc49db341a8d8440fed87745026fca7a7c5c14448cd8
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-1.debian.tar.xz' libzstd_1.4.8+dfsg-1.debian.tar.xz 13240 SHA512:1137f65e26aaeeaae2e0f708be5dc7b3c9f4e42853128652031918b20d31261dd9f992d9b885193cd38764615b964d5d726f1c9032d5984527ea655324dc559b
```

### `dpkg` source package: `linux=5.8.0-36.40+21.04.1`

Binary Packages:

- `linux-libc-dev:amd64=5.8.0-36.40+21.04.1`

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
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.dsc' lsb_11.1.0ubuntu2.dsc 2230 SHA512:d4545cee6b6ee4b54cd13ed7f8ab874a44579ce0783bb813a9dc48f0ca132b2bf11aba2fd179ff7d82ad867f663e1521b224da0de5fb3f66b634542d56addc55
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.tar.xz' lsb_11.1.0ubuntu2.tar.xz 46024 SHA512:b4a2c35ef8a21e3e6e1978687f54f485f0a3c8ee09082f8ae0d7a3dc0f65381062e1df962190164c3539f3f86c073961eb9f3c37b2aa4d3d8d6907a99ce04161
```

### `dpkg` source package: `lz4=1.9.3-0ubuntu1`

Binary Packages:

- `liblz4-1:amd64=1.9.3-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lzo2=2.10-2`

Binary Packages:

- `liblzo2-2:amd64=2.10-2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/lzo2/2.10-2/


### `dpkg` source package: `m4=1.4.18-5`

Binary Packages:

- `m4=1.4.18-5`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-5
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-5.dsc' m4_1.4.18-5.dsc 1637 SHA512:563a448bdd6101967d2281e0cf44fd542aeb476be9face3da15ef3450703ad3d5890e8d55bd2dbac97c16b700ef10001ba3faced5ffd87505cd074c05cc29178
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA512:06f583efc3855cd8477d8347544f4ae5153a3e50aea74d21968afa7214784ea3ddfc02d0a2b11324120d76a19f2e804d20de11a456b5da929eb6ae469519b174
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA512:effc857a19f1496d6dde2887c0314b37d4b142a435e77614936c730878c798491ad93b28860dddd2601f99a43fa41923729b961004faafc6f798f7bc1842f980
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-5.debian.tar.xz' m4_1.4.18-5.debian.tar.xz 17468 SHA512:3623a57f096cfbf6ec496d893fd805039bfb262c52624c2fc46dbbdbe9cee4c0061798e4915cc6f7ba984b9e74184d759dcf15d730c35073af5937de29c8dce4
```

### `dpkg` source package: `mailcap=3.68ubuntu1`

Binary Packages:

- `mailcap=3.68ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mailcap/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mailcap=3.68ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mailcap/mailcap_3.68ubuntu1.dsc' mailcap_3.68ubuntu1.dsc 1691 SHA512:a7e7485cc056fd09193ae751d7b25ad45d79bb4857e011aedfaa7c4ebf82b636bbe2ae8fc9885361e6e98f98a31478e352af8a64e569f946ad2b5fd960603371
'http://archive.ubuntu.com/ubuntu/pool/main/m/mailcap/mailcap_3.68ubuntu1.tar.xz' mailcap_3.68ubuntu1.tar.xz 27120 SHA512:988ecf261f9b8c62b14d68b3c3702cb515ff009ec0d194cc59dc233d64c12375c961dd09168b6f50aea6a0ba61878240f7b9011403212f69f29cbae31edd765c
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
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu1.dsc' make-dfsg_4.3-4ubuntu1.dsc 2147 SHA512:e1c5e4cc453a78982d26ec21ae66f0a5cda46ea3e2762d8e660065e7d430428b55416e0d6fcd259c9b55030a57f967dc662103bdad794976f9d0991ea1c01778
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA512:bdc150f9d256145923380d6e7058ab9b2b4e43fcb1d75ab2984fa8f859eab6852a68e4ea5f626633e0bec76fbebf1477378e268e8ffdb5cb2a53b29cbc439bc1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu1.diff.gz' make-dfsg_4.3-4ubuntu1.diff.gz 51058 SHA512:c2dd5be8149a60ca4a54146a25c5c4b6599172c052644d7290542b622e503f6fa1b2e5f255cfad82f068b66049778771e472e574b03202323dcbea6e71a1ec99
```

### `dpkg` source package: `mawk=1.3.4.20200120-2`

Binary Packages:

- `mawk=1.3.4.20200120-2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.dsc' mawk_1.3.4.20200120-2.dsc 1915 SHA512:dce7f6b96efa65c5cd2f365a4b8fad23aec8ecda4a31e624094479a7032303e64170c12c89a3f928649a3725f4e54a65af376369dab79ad31b3c4a13973f8754
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA512:14d9a6642ce931bf6457d248fc2d6da4f0ea7541976ca282ea708b26df048f86fdf92c27f72d497501ccd43a244d1d1a606f1a2f266a7558306fea35dcc3041b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.debian.tar.xz' mawk_1.3.4.20200120-2.debian.tar.xz 7504 SHA512:06326bd0c6b31d82f68102ef04ff2af272f84e12ffaa0354ac439c42c7c832f1616f398c2b1109f7052ddaede2a77a6469a2d925117044aaade93979592a7685
```

### `dpkg` source package: `media-types=4.0.0`

Binary Packages:

- `media-types=4.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=4.0.0
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_4.0.0.dsc' media-types_4.0.0.dsc 1620 SHA512:ff19b9eecde75e5558aa945438e12a1d964dec3188205ce1c90973c6d0948218823fc0c158a729a2b1efb3ddbd54264746c2c8d5167b14e008e54427672d0b47
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_4.0.0.tar.xz' media-types_4.0.0.tar.xz 33988 SHA512:6167849bfe24b9ce54221ee6d663d245e7c5db51975b42806797d94680a71dd208906b69ee827d9cea52711d0f676e2492c4d0d818e1d3dac1fa049335ac0f1d
```

### `dpkg` source package: `mercurial=5.5.2-1build1`

Binary Packages:

- `mercurial=5.5.2-1build1`
- `mercurial-common=5.5.2-1build1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `mime-support=3.66`

Binary Packages:

- `mime-support=3.66`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.66
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.66.dsc' mime-support_3.66.dsc 1625 SHA512:f3ed0e0c9274b4dc1dcc7c4f7b6c1e6d350cf1df2507572f326fec51b126012d1c8f54a0a61dd6e0647bc435eaca3d6addda79173b129522f7f1fcbedf2c67bb
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.66.tar.xz' mime-support_3.66.tar.xz 9568 SHA512:d41b074cf38dbe738b74367c456f28309fd3d00b67b2926db96523eba8ccaf534a11399bc5083d5875e439882159054a75e001d060863684611e20a26ed73bb1
```

### `dpkg` source package: `mpclib3=1.2.0-1`

Binary Packages:

- `libmpc3:amd64=1.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0-1.dsc' mpclib3_1.2.0-1.dsc 1851 SHA512:b68a2e0ea822170dcfb7b7b5b538fec1fc1d130a64eb325114ee5e7a6fa129eeed617293a2aefb296273e3d6c56d3bd8bd0a5ab3be4b88be7d2bfa55d07b5daa
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0.orig.tar.gz' mpclib3_1.2.0.orig.tar.gz 840711 SHA512:84fa3338f51d369111456a63ad040256a1beb70699e21e2a932c779aa1c3bd08b201412c1659ecbb58403ea0548faacc35996d94f88f0639549269b7563c61b7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0-1.diff.gz' mpclib3_1.2.0-1.diff.gz 4281 SHA512:eb877cab746ff3d1fa79e431c01cc48f936739d8b69074cfbf881716690cfab78ccb916afb39065b04ffebf03a52cdb47c99ad6716c30fd8136e141e7f2f7768
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
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3.dsc' mpfr4_4.1.0-3.dsc 1959 SHA512:ff99a80c7468e508efab5e4135e6fd54d7a50e55ccb168eda22a788ace44aae8b5bcf4091ed691b603ca96da0fb1af1f3e52411d61806e40d20b5923e5bd0bf4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA512:1bd1c349741a6529dfa53af4f0da8d49254b164ece8a46928cdb13a99460285622d57fe6f68cef19c6727b3f9daa25ddb3d7d65c201c8f387e421c7f7bee6273
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3.debian.tar.xz' mpfr4_4.1.0-3.debian.tar.xz 12372 SHA512:a0472b95ab7d7c8a00d7716039fefbd30142939f2077a930f0dafc056a3a5b9debc65bb9ddbfb88fbfdb6bcf9fb7871631bdb7376ca24d400e11a4c1a371df3e
```

### `dpkg` source package: `mysql-8.0=8.0.22-0ubuntu0.20.10.2`

Binary Packages:

- `libmysqlclient-dev=8.0.22-0ubuntu0.20.10.2`
- `libmysqlclient21:amd64=8.0.22-0ubuntu0.20.10.2`

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
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.dsc' mysql-defaults_1.0.5ubuntu2.dsc 2251 SHA512:452eb9dfdd1adc3a8e6134ae3f6d6a9d684654fd5f39727fef3ad632f046218eeaab492378565e4fa38bab40e1bc9e4765be09d4dcf303cdaf9a091f49338ace
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.tar.xz' mysql-defaults_1.0.5ubuntu2.tar.xz 7168 SHA512:6ed627ae4ac2fba44d674683e4f320ed89d44f2565c19d6e2c11206cab1f6eeab707367edbcc27f4fd54e1ef51e4637abb18d8381f4f27a344af00e1688f8cb0
```

### `dpkg` source package: `ncurses=6.2+20201114-2`

Binary Packages:

- `libncurses-dev:amd64=6.2+20201114-2`
- `libncurses5-dev:amd64=6.2+20201114-2`
- `libncurses6:amd64=6.2+20201114-2`
- `libncursesw5-dev:amd64=6.2+20201114-2`
- `libncursesw6:amd64=6.2+20201114-2`
- `libtinfo6:amd64=6.2+20201114-2`
- `ncurses-base=6.2+20201114-2`
- `ncurses-bin=6.2+20201114-2`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ncurses/6.2+20201114-2/


### `dpkg` source package: `netbase=6.2`

Binary Packages:

- `netbase=6.2`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.2
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.2.dsc' netbase_6.2.dsc 875 SHA512:5641cc2dc13982e72869fe0a0319edc56a53c3c5a9902485993d1c03a73951a8587e88e4712d116d8cfbd3c6cd96e74ce7247ed6d2b49a83c60d5a6369e36456
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.2.tar.xz' netbase_6.2.tar.xz 31908 SHA512:81fdc4e9ca99c61a5441a3a60ca1c0be99abbf036eb8e2edd036acc6efaf8effcf083470af08f3eeaf0f75281325ae34de35fceea6fed6ed7687f06123acec01
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/nettle/3.6-2/


### `dpkg` source package: `nghttp2=1.42.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.42.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `SIL-OFL-1.1`
- `all-permissive`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/nghttp2/1.42.0-1/


### `dpkg` source package: `npth=1.6-3`

Binary Packages:

- `libnpth0:amd64=1.6-3`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-3
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-3.dsc' npth_1.6-3.dsc 1931 SHA512:0ee136515640c735dec41cc6c1cd6dc267c849e45621f8bf8a969a0782e2e2e305fb95d58641f0df62a377cf21a28609b32b9fc1509adb02b328ffeb82b80583
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA512:2ed1012e14a9d10665420b9a23628be7e206fd9348111ec751349b93557ee69f1176bcf7e6b195b35b1c44a5e0e81ee33b713f03d79a33d1ecd9037035afeda2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-3.debian.tar.xz' npth_1.6-3.debian.tar.xz 10712 SHA512:47b3f95586854b2a0667af6bb4f2bb8ff86eef934ad5b4d1b3e2a5255ce8acc0eedd9c8586c07527e223f8e29efa3bc3aeb69c86acdfb36cbb51743903abf8ef
```

### `dpkg` source package: `openexr=2.5.3-2`

Binary Packages:

- `libopenexr-dev=2.5.3-2`
- `libopenexr25:amd64=2.5.3-2`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr25/copyright`)

- `BSD-3-clause`
- `openexr`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openexr/2.5.3-2/


### `dpkg` source package: `openjpeg2=2.3.1-1ubuntu5`

Binary Packages:

- `libopenjp2-7:amd64=2.3.1-1ubuntu5`

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
$ apt-get source -qq --print-uris openjpeg2=2.3.1-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu5.dsc' openjpeg2_2.3.1-1ubuntu5.dsc 2842 SHA512:5181a94bafe9f04a417b8e483458b4aa558fc8501d01269ad411891aeb81c88ebd17a9a7021837a8fca6feb50ba5b932969aa1eb5ce6d442dfc4b2313c91e719
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1.orig.tar.xz' openjpeg2_2.3.1.orig.tar.xz 1381768 SHA512:1346fae5f554102c46ad26e59888c693bf57b3ffaccfb5040b6c177f2ca510dd0915966d6bfd252b4293c0c098290c8e6cd923c265ca288e95e1fb7522b66b32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu5.debian.tar.xz' openjpeg2_2.3.1-1ubuntu5.debian.tar.xz 25156 SHA512:0dec70bb78cf4999a209ecb5b9c208b9b1e5336b59ccf709842efe3da10246b9458e513a03442004616ae0bfe2fcfc54012ee6053a8837dd4b70592a23b85b71
```

### `dpkg` source package: `openldap=2.4.56+dfsg-1ubuntu1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.56+dfsg-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openssh=1:8.4p1-3`

Binary Packages:

- `openssh-client=1:8.4p1-3`

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
$ apt-get source -qq --print-uris openssh=1:8.4p1-3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1-3.dsc' openssh_8.4p1-3.dsc 3353 SHA512:ebb6403ee32af3a350cd7c70dfd50d0361c6b3e076f5f3583aa403a4418ac37e8479b5cb099cf2385d7e8a48c56cfa055a1b7043337131d9e2afaa383d140c13
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1.orig.tar.gz' openssh_8.4p1.orig.tar.gz 1742201 SHA512:d65275b082c46c5efe7cf3264fa6794d6e99a36d4a54b50554fc56979d6c0837381587fd5399195e1db680d2a5ad1ef0b99a180eac2b4de5637906cb7a89e9ce
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1.orig.tar.gz.asc' openssh_8.4p1.orig.tar.gz.asc 683 SHA512:3d9a026db27729a5a56785db3824230ccf2a3beca4bb48ef465e44d869b944dbc5d443152a1b1be21bc9c213c465d3d7ca1f876a387d0a6b9682a0cfec3e6e32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1-3.debian.tar.xz' openssh_8.4p1-3.debian.tar.xz 178784 SHA512:e4844f4918ba7e7ea59d5fe69d5106219b17647dd20f2d09e1b44d08f9bb26d0fd9f7d6c77c5b3cbc02c12167620025512dab60656079492509626b37a43cf44
```

### `dpkg` source package: `openssl=1.1.1f-1ubuntu5`

Binary Packages:

- `libssl-dev:amd64=1.1.1f-1ubuntu5`
- `libssl1.1:amd64=1.1.1f-1ubuntu5`
- `openssl=1.1.1f-1ubuntu5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1f-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu5.dsc' openssl_1.1.1f-1ubuntu5.dsc 2705 SHA512:1117e25e430e01a4103b0e80727eaa883bd395924dbd46f928b0620e9b451d2efad15973eb3edad98a60c765fe7d4c99e3946a4c3c4a4274bb7432108ed30877
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz' openssl_1.1.1f.orig.tar.gz 9792828 SHA512:b00bd9b5ad5298fbceeec6bb19c1ab0c106ca5cfb31178497c58bf7e0e0cf30fcc19c20f84e23af31cc126bf2447d3e4f8461db97bafa7bd78f69561932f000c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz.asc' openssl_1.1.1f.orig.tar.gz.asc 488 SHA512:63b01ffc23b2fec2cfc147d382b486a136e5610e181be94aa333022803a442ded37e8276fefb62b3176b571b94a1d2243c05b86b52ad7784fe0068d1ad948562
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu5.debian.tar.xz' openssl_1.1.1f-1ubuntu5.debian.tar.xz 154368 SHA512:4611f58d07da4263f30d5fe176d6a5035ee102121d06a126f24b281af884428beb7e3b744db1e08585eeb161ed99793fe1cebc030cd2cadd40d06ee1d42ab909
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22-1.dsc' p11-kit_0.23.22-1.dsc 2417 SHA512:09d764f710260a71041b5714397af68b0aaf20bd419b9aac7997709d80ac3bddf4fe2c132ca9510bb662986b4e3576627628237cd9c95ed7d1ff1ffcca04cee7
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz' p11-kit_0.23.22.orig.tar.xz 830016 SHA512:098819e6ca4ad9cc2a0bc2e478aea67354d051a4f03e6c7d75d13d2469b6dc7654f26b15530052f6ed51acb35531c2539e0f971b31e29e6673e857c903afb080
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz.asc' p11-kit_0.23.22.orig.tar.xz.asc 854 SHA512:1ebb730b9c29908773de12aca89df2434576b8d9ec5da6d33db772b1e1aa4b0e8aa86ddc3e0de1abcd98a7012b5a25e3097e3a2dda2401cc37f79fd76b4f9467
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22-1.debian.tar.xz' p11-kit_0.23.22-1.debian.tar.xz 22256 SHA512:5d10918372cf7b6ae5ee6aa03e653b2ba55e61a691c9e9e7d8673a2e4a632941ccda38e213691ca5b05ce422d1af71ced902cf9c7b8d3be7e45662e96e6dce69
```

### `dpkg` source package: `pam=1.3.1-5ubuntu6`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu6`
- `libpam-modules-bin=1.3.1-5ubuntu6`
- `libpam-runtime=1.3.1-5ubuntu6`
- `libpam0g:amd64=1.3.1-5ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu6.dsc' pam_1.3.1-5ubuntu6.dsc 2699 SHA512:436e65b46b14cb02b6d13255143f8a06064a52c3a3fa8dae7a2305f1e7a3017db19389693c0150a9a4aacc40ad3664318178ebdafd081b1057fd083920391a34
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA512:6bc8e2a5b64686f0a23846221c5228c88418ba485b17c53b3a12f91262b5bb73566d6b6a5daa1f63bbae54310aee918b987e44a72ce809b4e7c668f0fadfe08e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu6.debian.tar.xz' pam_1.3.1-5ubuntu6.debian.tar.xz 160300 SHA512:c3e8d10c1d799a8b34d29d584d34813191f7dab1124ae9824d6df5e3eea49fb76b4647b30ecaad69bc06031eb02b0cbc8612673e85944690ea7f88b874ac369c
```

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pango1.0/1.46.2-3/


### `dpkg` source package: `patch=2.7.6-7`

Binary Packages:

- `patch=2.7.6-7`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7.dsc' patch_2.7.6-7.dsc 1706 SHA512:80b70e71b30bb0fffc01cb1abc13cd5474b0c049b201234646f2d9a3117c8c7339264818b1633a522430c8825513a83460aab666a9590eb72a0bdc80048093f6
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA512:fcca87bdb67a88685a8a25597f9e015f5e60197b9a269fa350ae35a7991ed8da553939b4bbc7f7d3cfd863c67142af403b04165633acbce4339056a905e87fbd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7.debian.tar.xz' patch_2.7.6-7.debian.tar.xz 15084 SHA512:8c46cca63c5978edf6e40f163d5039b092d6125cfd620ab20bd7fdb04d4ea5fe6162e914719e4948d1faf7f958be8a77903344bcbb2b392e7078d9c31768a6dc
```

### `dpkg` source package: `pcre2=10.35-2ubuntu1`

Binary Packages:

- `libpcre2-16-0:amd64=10.35-2ubuntu1`
- `libpcre2-32-0:amd64=10.35-2ubuntu1`
- `libpcre2-8-0:amd64=10.35-2ubuntu1`
- `libpcre2-dev:amd64=10.35-2ubuntu1`
- `libpcre2-posix2:amd64=10.35-2ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.dsc' pcre3_8.39-13.dsc 2226 SHA512:5a12d0001341c4bdda5b087ef418d5f4e2ab5d27d3fb117319fce82e86ffe0167e2bf1e8afee1fb71fb479fc697fd1243ead3d89519a628a84ede2f99bf79cd0
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA512:8b0f14ae5947c4b2d74876a795b04e532fd71c2479a64dbe0ed817e7c7894ea3cae533413de8c17322d305cb7f4e275d72b43e4e828eaca77dc4bcaf04529cf6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.debian.tar.gz' pcre3_8.39-13.debian.tar.gz 27002 SHA512:1dda1a982ecf1cf888e4f716101e84d99f427cd46874ab4d4116b0bda0852ef5cb7f57cec0edc7cab24c5095431694787dc052dab771621449f7c9d8c2367b86
```

### `dpkg` source package: `perl=5.32.0-6`

Binary Packages:

- `libperl5.32:amd64=5.32.0-6`
- `perl=5.32.0-6`
- `perl-base=5.32.0-6`
- `perl-modules-5.32=5.32.0-6`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/perl/5.32.0-6/


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
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.dsc' pinentry_1.1.0-4build1.dsc 2595 SHA512:c2aefb05c736ee9cf779e641a0a0a20810fccb8e6e8c88f7d13a08b3e8cfa7f4246d9c70ecc6a907bdda143366b058e866a8f78124ef259ae4dc7963a542f389
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA512:5012672925bcb5f683358c259e55e4b87c67cf063ad52c759308933733025c33f7ce08e5b8019ffc101cbf7ef30499040ef2fd34a7611698e65e1593f80948cd
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.debian.tar.xz' pinentry_1.1.0-4build1.debian.tar.xz 17312 SHA512:6288a034c9c08e4a164c5e2d9c66142638a0da6947031e0199811272e004c107209bb0feb0048ae685176ba3a4d3a98e7520edb16d633721a474810897b8f18d
```

### `dpkg` source package: `pixman=0.40.0-1`

Binary Packages:

- `libpixman-1-0:amd64=0.40.0-1`
- `libpixman-1-dev:amd64=0.40.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pixman/0.40.0-1/


### `dpkg` source package: `pkg-config=0.29.2-1ubuntu1`

Binary Packages:

- `pkg-config=0.29.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu1.dsc' pkg-config_0.29.2-1ubuntu1.dsc 1799 SHA512:1feaf95782519c0248ddca2682c8b628aee8d5bb0a0b7b044899e30981007c824f77a76f96a1304b803136f0dd87a9dd0aef7b067cb79171ddd33c5038377e13
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2.orig.tar.gz' pkg-config_0.29.2.orig.tar.gz 2016830 SHA512:4861ec6428fead416f5cbbbb0bbad10b9152967e481d4b0ff2eb396a9f297f552984c9bb72f6864a37dcd8fca1d9ccceda3ef18d8f121938dbe4fdf2b870fe75
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu1.diff.gz' pkg-config_0.29.2-1ubuntu1.diff.gz 9852 SHA512:f569a50558520fec4450933234d33801a30f80f82d95d31aec5a91823bd55d8962ef4f63cc730923145c372da9c50e44dde836f45ed69c0ad64178c6787ef94d
```

### `dpkg` source package: `postgresql-13=13.1-1build1`

Binary Packages:

- `libpq-dev=13.1-1build1`
- `libpq5:amd64=13.1-1build1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `procps=2:3.3.16-5ubuntu2`

Binary Packages:

- `libprocps8:amd64=2:3.3.16-5ubuntu2`
- `procps=2:3.3.16-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.16-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-5ubuntu2.dsc' procps_3.3.16-5ubuntu2.dsc 2234 SHA512:565d002c6b01a3d50dcac0ba9f1f9428aa6969509a3fd0e977b85fb3bffc4892e05ed5baa8a114ffe8552f5ac11d8aba48a4705d47dc38f0a6fde27ab3f62ea1
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16.orig.tar.xz' procps_3.3.16.orig.tar.xz 621892 SHA512:38db4f72fe40c2f027b23b18bbc8c29cfcdf6bcdb029199fe4bebede153943aa884157f56e792c399f9a4949cc514687500bb99a75a5e7ad7b9e878f52090304
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-5ubuntu2.debian.tar.xz' procps_3.3.16-5ubuntu2.debian.tar.xz 34056 SHA512:b3e95ef3cfd671d9683f2e6ba136f8f0a22a1ab6f7a87e27cfc255b533dc985c0d3fc87f8e180d8bf376390d88dd5bf1aa0316edfdb5ca99f952b0b5c9d63e33
```

### `dpkg` source package: `python3-defaults=3.9.0-3ubuntu1`

Binary Packages:

- `libpython3-stdlib:amd64=3.9.0-3ubuntu1`
- `python3=3.9.0-3ubuntu1`
- `python3-minimal=3.9.0-3ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python3-stdlib-extensions=3.9.0-1`

Binary Packages:

- `python3-distutils=3.9.0-1`
- `python3-lib2to3=3.9.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-stdlib-extensions/3.9.0-1/


### `dpkg` source package: `python3.9=3.9.1-1`

Binary Packages:

- `libpython3.9-minimal:amd64=3.9.1-1`
- `libpython3.9-stdlib:amd64=3.9.1-1`
- `python3.9=3.9.1-1`
- `python3.9-minimal=3.9.1-1`

Licenses: (parsed from: `/usr/share/doc/libpython3.9-minimal/copyright`, `/usr/share/doc/libpython3.9-stdlib/copyright`, `/usr/share/doc/python3.9/copyright`, `/usr/share/doc/python3.9-minimal/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3.9/3.9.1-1/


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
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-1.dsc' readline_8.1-1.dsc 2418 SHA512:aeb4b2a55e583565f64c2185e684c0e7cfcb0256831fc509f18f0d98a7b48d6fc5c1b76f41e2bdeab285f10731c2423c39c5fcc679ce111c2a4d359177394fe7
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.orig.tar.gz' readline_8.1.orig.tar.gz 2993288 SHA512:27790d0461da3093a7fee6e89a51dcab5dc61928ec42e9228ab36493b17220641d5e481ea3d8fee5ee0044c70bf960f55c7d3f1a704cf6b9c42e5c269b797e00
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-1.debian.tar.xz' readline_8.1-1.debian.tar.xz 29220 SHA512:e199bbcbdb999235b388daf537d2b6cce0a2a7ed29eab9f76ddee9ceedc16ba7d63c082b1eeb9769f432f86d2d6fd55d99a7227cbf393f3b5581f5d6f164f556
```

### `dpkg` source package: `rpcsvc-proto=1.4.2-0ubuntu4`

Binary Packages:

- `rpcsvc-proto=1.4.2-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/rpcsvc-proto/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+-autoconf-exception`
- `GPL-3`
- `GPL-3+-autoconf-exception`
- `MIT`
- `permissive-autoconf-m4`
- `permissive-autoconf-m4-no-warranty`
- `permissive-configure`
- `permissive-fsf`
- `permissive-makefile-in`

Source:

```console
$ apt-get source -qq --print-uris rpcsvc-proto=1.4.2-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-0ubuntu4.dsc' rpcsvc-proto_1.4.2-0ubuntu4.dsc 2084 SHA512:9394b59683cb47176e8ff8a90247d48794d6b3e0db1d31e28e117048648f648cc2a858e9b034959eb377edda37dd87efd47065deb3876a5610dacefb9630c33b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2.orig.tar.xz' rpcsvc-proto_1.4.2.orig.tar.xz 171620 SHA512:631fbfc00af94c5d7def0759f27e97dc14d400b4468c906719ae18ecef74815730798c882d1aaa4f90359224e7b829019b786baddc3097905b54f940ca85a714
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-0ubuntu4.debian.tar.xz' rpcsvc-proto_1.4.2-0ubuntu4.debian.tar.xz 4132 SHA512:92efb91238c1b4e62db66a8a4bd48a6a0ce57e82acf9578625166b7b6b94523c247b194c3a8be88c07aa4a0250adb2aedd76c39ada51d43127d42341709989f5
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
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build2.dsc 2402 SHA512:bd16f8a7269549b4f15e46017012a2d99ed22378dcca6b9b664ff137d18c946b3f0b03f8a961c928196ddc473f1012a968bd91c3d4df6837da97fa0634f85c12
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA512:bdfcbab73179d614a295a7b136ea4c9d0ce4620883b493f298362784d245608cd6ad4b0ad30f94ed73a086b4555399521ae9e95b6375fce75e455ae68c055e7b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build2.debian.tar.xz 8276 SHA512:9fb15d0d48319162214f9e417a183559f9b09c22ea89546c81ae2add40c802bb48ff54ea32162b209c99bf8dae939f4eb7af9498aff831f697f5f095160b95ba
```

### `dpkg` source package: `sed=4.7-1ubuntu1`

Binary Packages:

- `sed=4.7-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.7-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1ubuntu1.dsc' sed_4.7-1ubuntu1.dsc 1962 SHA512:179205b845907589f9ad485b632716d2a4214d7331359a7e1cb2d77320f54e64d38bff5886dfe5fac793b5088f020401610c0bf7d94f6d629b2faee09ca3be17
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7.orig.tar.xz' sed_4.7.orig.tar.xz 1298316 SHA512:e0be5db4cdf8226b34aaa9071bc5ae0eafde1c52227cee3512eea7fe2520d6c5cebf15266aa5c4adffbb51bf125c140a15644e28d57759893c12823ea9bbf4fb
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1ubuntu1.debian.tar.xz' sed_4.7-1ubuntu1.debian.tar.xz 60556 SHA512:7dce87f4bd2f26819da09efddfc2caf68d958b254704423e0c77ad58f201a8ddd0f9e48e211e23f675348196e0a81dfd67865fb7f009eebfb76b15ebde0f15cf
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.14.dsc' sensible-utils_0.0.14.dsc 1702 SHA512:f2640c77c7cb63aa94f67ffc47f6e6df6f22eb4598432b2d29f415cbda8b1c57aa439a447cd7a2201ea8002a7fbc1352cd125357962e854a3f4b7d85e8ba0ed0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.14.tar.xz' sensible-utils_0.0.14.tar.xz 64448 SHA512:15ba996f811ab3a9c1f5726f35766d74aafdf925c5c2392b33c6643d6c439796a742f9d0f4625c79de640e6b5e4a6a032b768eb1bc4ac31b448f9767b0ceed44
```

### `dpkg` source package: `serf=1.3.9-10`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-10`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-10/


### `dpkg` source package: `shadow=1:4.8.1-1ubuntu8`

Binary Packages:

- `login=1:4.8.1-1ubuntu8`
- `passwd=1:4.8.1-1ubuntu8`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu8.dsc' shadow_4.8.1-1ubuntu8.dsc 2345 SHA512:ba6658eab0eae7ed21ffd04f0e63f761ab45a682b18992cd83776dac5dc617f6d301a3829fdc5726d7b815883a8f8a455a8a2820f984f7aea3c2201573e9f2cb
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA512:780a983483d847ed3c91c82064a0fa902b6f4185225978241bc3bc03fcc3aa143975b46aee43151c6ba43efcfdb1819516b76ba7ad3d1d3c34fcc38ea42e917b
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu8.debian.tar.xz' shadow_4.8.1-1ubuntu8.debian.tar.xz 86200 SHA512:01824fe4238614df35b199e1b3f3851719a71f2c76a77cc90883a3cca0b56082309e2aee8825603d01651d06442a4ef30de83139629cef585285b59182eaa97a
```

### `dpkg` source package: `shared-mime-info=2.0-1`

Binary Packages:

- `shared-mime-info=2.0-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.0-1.dsc' shared-mime-info_2.0-1.dsc 2223 SHA512:d4a7484c19043cd1326901385bd370b94ccd727736f1772e1b380eefc590820fdf870badd060e5a9f28f9106d4676f6283823a06f3558f07767ae91e85f9561c
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.0.orig.tar.xz' shared-mime-info_2.0.orig.tar.xz 5015272 SHA512:f4a1ea9a408ffcff325e57585dec5862405e9fd6c79e444048039f3061676501c40168cecf8935d002644a702a21f08f0f7c680ef6a65fdf188e0d892f3cc085
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.0-1.debian.tar.xz' shared-mime-info_2.0-1.debian.tar.xz 10612 SHA512:6e5617dd2522d90c4735e1b936668fe55366d3dc113e844c124c3eb30e73ca059331f253a9adf0c2e26bd39544ef7b2672cde50bd21cca23b877e8a64e529b92
```

### `dpkg` source package: `sqlite3=3.34.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.34.0-1`
- `libsqlite3-dev:amd64=3.34.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.34.0-1/


### `dpkg` source package: `subversion=1.14.0-3build2`

Binary Packages:

- `libsvn1:amd64=1.14.0-3build2`
- `subversion=1.14.0-3build2`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `systemd=247.1-4ubuntu1`

Binary Packages:

- `libsystemd0:amd64=247.1-4ubuntu1`
- `libudev1:amd64=247.1-4ubuntu1`

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


### `dpkg` source package: `sysvinit=2.96-5ubuntu1`

Binary Packages:

- `sysvinit-utils=2.96-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-5ubuntu1.dsc' sysvinit_2.96-5ubuntu1.dsc 2716 SHA512:a6c31c46bfb66eac6059133aef2da3439029763095fd6a04cdb4ffc137f3f397e2906121ab3c510ceae28bca2e4453cc40e78c9ee44c3f358068ef3895c68d01
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA512:1388398568ebfe53460796f8ab75a3ead6111612888ea36e8f1c0db4d41ef6f45fc217abb7804519ff1143a78d97c95b24e42c8c22c95a47b9436484bfb6f45d
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA512:2b3798e8fc8531cd1a2b2a523159b7f064bfadd8815b930fb70d5a1380775f1b5bac5627d5cd9d95b03ff3737d8d6b2f357c6bc21ac2e21ee089b67f98b4eb6a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-5ubuntu1.debian.tar.xz' sysvinit_2.96-5ubuntu1.debian.tar.xz 128828 SHA512:8505b783ed88277eac28a62c4d36f6f54dd3f2a10e637a095ac7b6e13428be74af692834b0262ffa3549bf9f4c5fc20086b516f84eff5f99c869c086a9f29761
```

### `dpkg` source package: `tar=1.32+dfsg-1`

Binary Packages:

- `tar=1.32+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tar/1.32+dfsg-1/


### `dpkg` source package: `tiff=4.1.0+git201212-1ubuntu1`

Binary Packages:

- `libtiff-dev:amd64=4.1.0+git201212-1ubuntu1`
- `libtiff5:amd64=4.1.0+git201212-1ubuntu1`
- `libtiffxx5:amd64=4.1.0+git201212-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.1.0+git201212-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git201212-1ubuntu1.dsc' tiff_4.1.0+git201212-1ubuntu1.dsc 2301 SHA512:8959d04ad31b052003a8ae04dce6a048f1843e455886757612a6d791bc3dec450e0e235c3b97f14026b1023e5fd3271f0954a499efad1ab025d7128905c538da
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git201212.orig.tar.xz' tiff_4.1.0+git201212.orig.tar.xz 1723848 SHA512:6fdffc889594981d4e47e52b70e0cf533124ec4a5959b60b9b7f08cd00c42606f836e52061c213795943d4ba412db892133fd7dfe9b837c324bc5e641970d796
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git201212-1ubuntu1.debian.tar.xz' tiff_4.1.0+git201212-1ubuntu1.debian.tar.xz 19616 SHA512:81108341d1321e7ccc424cd02256e231ac21512d936a96c5afb9056a4e09e42169d88ca1b32320f21abba3559c17334b3f383b07e77eda50cbb2d6f28d1dabb3
```

### `dpkg` source package: `tzdata=2020f-1ubuntu2`

Binary Packages:

- `tzdata=2020f-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ubuntu-keyring=2020.06.17.1`

Binary Packages:

- `ubuntu-keyring=2020.06.17.1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ucf=3.0043`

Binary Packages:

- `ucf=3.0043`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0043
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043.dsc' ucf_3.0043.dsc 1423 SHA512:666851d1df82352f8b2be8b8760250cfa1f7635718f0f1598a3d9e9f11a9d687ec4cfb7f6bf950b194d771db039508b6d62c288f53078e2712580bda7b5befa7
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043.tar.xz' ucf_3.0043.tar.xz 70560 SHA512:693209ea06a63279278ac8f63e70fe151880f7c51d54c91ad5e846449f883d5893658d8c6932553d70da4e56ebae3ef67c0eda8593b0768f5979849c79f89f27
```

### `dpkg` source package: `unzip=6.0-25ubuntu1`

Binary Packages:

- `unzip=6.0-25ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `utf8proc=2.5.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.5.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.5.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0-1.dsc' utf8proc_2.5.0-1.dsc 2154 SHA512:db27af4c75e805f6d39b39bce01648229eb63f542899e6779c2779fd49f48a78409237bb9ae358da3002ec239a1e8e265ff5006a7aeaf935b10dbb26b2f3c22e
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0.orig.tar.gz' utf8proc_2.5.0.orig.tar.gz 155485 SHA512:0c553faf4f3841c17c7aa4cce1e917b1585c430ac3f7f240ab98cbe01b9743f2074532e6f71faf3df030f5af00e483a3faf9716a67e6a4b1bb66a3de48308014
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0-1.debian.tar.xz' utf8proc_2.5.0-1.debian.tar.xz 5240 SHA512:0a32ae86570560b98eb174b33ff819cc07ad945466527def0567e729436491aab410b9d239597d5484c0b07d4dae676f2ebc2ffb09a2bd6ef455abb08e6cd94b
```

### `dpkg` source package: `util-linux=2.36.1-1ubuntu2`

Binary Packages:

- `bsdutils=1:2.36.1-1ubuntu2`
- `libblkid-dev:amd64=2.36.1-1ubuntu2`
- `libblkid1:amd64=2.36.1-1ubuntu2`
- `libmount-dev:amd64=2.36.1-1ubuntu2`
- `libmount1:amd64=2.36.1-1ubuntu2`
- `libsmartcols1:amd64=2.36.1-1ubuntu2`
- `libuuid1:amd64=2.36.1-1ubuntu2`
- `mount=2.36.1-1ubuntu2`
- `util-linux=2.36.1-1ubuntu2`
- `uuid-dev:amd64=2.36.1-1ubuntu2`

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
$ apt-get source -qq --print-uris util-linux=2.36.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1-1ubuntu2.dsc' util-linux_2.36.1-1ubuntu2.dsc 4422 SHA512:87b280d39f9def6e0256d5a24b2807ea9b069524160a5d3fed1d324a9d94c9b45b694b302b0e95d70af9679a277ac5c58b26877e39f59de9d1a76bdcfbffe4ca
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1.orig.tar.xz' util-linux_2.36.1.orig.tar.xz 5231880 SHA512:9dfd01ae4c16fa35015dafd222d555988b72e4d1d2fbadd140791b9ef78f84fa8254d4d08dc67cabf41e873338867f19e786b989d708ccfe5161c4f7679bba7a
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1-1ubuntu2.debian.tar.xz' util-linux_2.36.1-1ubuntu2.debian.tar.xz 99248 SHA512:96f0744d877246cdb46bb2a2d3edff37a69c3f7f1163b1f743be181101e8a76b29029a37bb9f7afa1db95a988a90cda0dc902e930fb42a9bdae3299f09ccd1c0
```

### `dpkg` source package: `wget=1.21-1ubuntu1`

Binary Packages:

- `wget=1.21-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21-1ubuntu1.dsc' wget_1.21-1ubuntu1.dsc 2260 SHA512:56322a76fad682f669bfa2caf913d2e887f0d34642157255d630a8274d0a2d72cec832988c89c577f92d7aecbab413853e1e9c09cfb03651e8d97a7a5856df85
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.orig.tar.gz' wget_1.21.orig.tar.gz 4866788 SHA512:13313a98f91ef34ad90103f076285549eb4887d77953e9f192d3b0667642b5ceb9e2e30091f766cbf1d6ed423499c497ed85d826f3f3e92f0711aa06d8303c5a
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.orig.tar.gz.asc' wget_1.21.orig.tar.gz.asc 854 SHA512:1bdaedc164800158625fddbc842c2cbe246d3e3c2f07546ecebacc8c1ea44779aab31a707d792f965669f2403941d4869e59719198563a0f39099145609310d1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21-1ubuntu1.debian.tar.xz' wget_1.21-1ubuntu1.debian.tar.xz 63388 SHA512:6213a76b085d9afee038037af06ec2f18655572763b3b949c837a552fea081d03d4b186c332db1afcea6797e3e5381597a3a2b547bc3cd1d646142e34a950dd4
```

### `dpkg` source package: `xorg-sgml-doctools=1:1.11-1.1`

Binary Packages:

- `xorg-sgml-doctools=1:1.11-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xorg-sgml-doctools=1:1.11-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.1.dsc' xorg-sgml-doctools_1.11-1.1.dsc 1987 SHA512:1682e1a4d4be1bfb1242adfa22b2764a9425b035cbfae9fd58925d4904eb301fe48bf92fc5935e973d7653db001ab221a8eac8cc5e2840d5a2e0cb4f1bb4895c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11.orig.tar.gz' xorg-sgml-doctools_1.11.orig.tar.gz 150367 SHA512:a2386e41a8e2f7deaded61e00eaeab922647c0d0f4e36268c4337dc71d2412b0ec433140d080a0fd118b6112ed0a4f960280f932fe8d4a90ea9dc8bedf1eb75e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.1.diff.gz' xorg-sgml-doctools_1.11-1.1.diff.gz 3296 SHA512:0ea09f6de75cf649fb82705a0470e5ba04edbe59ccfa26132e60120e04036b86e9ff47785fdcee2499fa005cbbdfc9e04ebdca619d0253ea558e2fe5501b9ec4
```

### `dpkg` source package: `xorg=1:7.7+19ubuntu15`

Binary Packages:

- `x11-common=1:7.7+19ubuntu15`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19ubuntu15
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu15.dsc' xorg_7.7+19ubuntu15.dsc 2082 SHA512:4f55afe6f4b5824b98638d61573a8d02c840351f869662ba83015f68bffead3371e5db76612bde6a8502be7fe22eb9a92e77e7d06fe4060fac9765e1a485384b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu15.tar.gz' xorg_7.7+19ubuntu15.tar.gz 299216 SHA512:298af258b64ec0190cec7ddc5f9f02633cdc0d4b67eb414ee3af3bdfcfb840fb2ce010a82643a2a3a28517d383ece3b7e6921035235107b693741018ea5ec678
```

### `dpkg` source package: `xorgproto=2020.1-1`

Binary Packages:

- `x11proto-core-dev=2020.1-1`
- `x11proto-dev=2020.1-1`
- `x11proto-xext-dev=2020.1-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`, `/usr/share/doc/x11proto-xext-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2020.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1-1.dsc' xorgproto_2020.1-1.dsc 3410 SHA512:657d90d91061a1ce0d48ead6d6b5b072219289939a9b84c496eea98dea008b0b665c8bb9c3cd8a6f4d4017a5978cd38257c81844d26d524740ccf7560d668fc5
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1.orig.tar.gz' xorgproto_2020.1.orig.tar.gz 1081369 SHA512:d0bc3aec517fd00fa5fd32a5715760c34810a19154e10fb1f92f2e2fe7f26136f7ba9b76b47fcd37c3c4796663154f4e5abf6a18dd634619b0f718f3e4737ae9
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1.orig.tar.gz.asc' xorgproto_2020.1.orig.tar.gz.asc 659 SHA512:5932a8525ca3032d61b87ef8f69b5ff8997da095eebfcb3400fa5ce6a97413a7161a794b8dfac16475ee56154348ff62c1eba02b2dd191f8e89bf12f2056bfbe
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1-1.diff.gz' xorgproto_2020.1-1.diff.gz 20627 SHA512:7213ab21dda33bb416e74ecd18ed569670b44a064f76ea2f5ccfcd3fcbdccaf232842d376559694cde3b7753cf4b0b1279e423219c4640d4d2d8f941eff14ddb
```

### `dpkg` source package: `xtrans=1.4.0-1`

Binary Packages:

- `xtrans-dev=1.4.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xtrans=1.4.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.4.0-1.dsc' xtrans_1.4.0-1.dsc 1919 SHA512:ac171ce0f00e1741e97a4ddad630ccff69070c0ef60047071b3f940fad08cb468d5ded7b2d4f0f500aeda73f2b703d55a7a4bbe0d5fff88cc3381486a111f580
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.4.0.orig.tar.gz' xtrans_1.4.0.orig.tar.gz 225941 SHA512:21287ccf18fe2ebd458765496b026d175bf47c6e8e5c21d5b9ea17203967efc0cf6928fa2f3385d289a680c7002c3640e4731937029e99933c2a64bb9fab5326
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.4.0-1.diff.gz' xtrans_1.4.0-1.diff.gz 9522 SHA512:d6deaa9579fb61e6ffd296ffe6b083eb9de572001c0a5bc82229ecc3d50bf2ee2f6504b3daa533bd34f3d647d6bd2235728084ec0b59869f6446652b998797f7
```

### `dpkg` source package: `xxhash=0.8.0-2`

Binary Packages:

- `libxxhash0:amd64=0.8.0-2`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0-2.dsc' xxhash_0.8.0-2.dsc 1601 SHA512:8ced1e4a71c06c4de87469316d28d1ea905f52bb3debb4152d2b42f0eda355dbac43576d7d5eb4e31d8e9a032e83ba4b5893db9aed04e5abffe8437e1d2f1b7c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0.orig.tar.gz' xxhash_0.8.0.orig.tar.gz 145909 SHA512:c3973b3c98bad44e1d8687ab4f9461aecd1c071bb3d320537a4c50fb7301edd13e990bab48cc6e5ca30536a814c8fa8cac24ceb1803a7e8eca30ef73d449373e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0-2.debian.tar.xz' xxhash_0.8.0-2.debian.tar.xz 4160 SHA512:7ca8e3e87bb87bd58e03161ecfbe682f3950068bc4aec0a7e300c307b35bdafc6d76a54edf4887a584c426d455d0c557d9d4df98d85c7cdf734d67e5f5aca4f3
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu4`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu4`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2ubuntu4`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu4.dsc' zlib_1.2.11.dfsg-2ubuntu4.dsc 2945 SHA512:afe11a895b3c5355d897543fb74716c2c78c2c273a51f75f53b10a49c678217d31ef7ed6b66a3d3423263dd918379d356bd47da139a3468adcdf2ecb18195a5a
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu4.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu4.debian.tar.xz 50768 SHA512:bd064f5baa8feec0fedb0406169a1a9ba0ba6bd0a581efbaa7c43e88707a429b26dfe3b7eacaa5f6657c3ab29320896473ba6418374583bc2602e3dd9de839af
```
