# `buildpack-deps:hirsute-scm`

## Docker Metadata

- Image ID: `sha256:c983d3a310d65ab153dba1206730b59c8ce20983d995877c3107dd4a00166fde`
- Created: `2021-01-21T07:53:20.230135333Z`
- Virtual Size: ~ 234.17 Mb  
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
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6build1.dsc' attr_2.4.48-6build1.dsc 2482 SHA512:099ac327a747ddb50fc8ff279ed2215e1bb00fb9b5fdac61e951f33a3a8e515b737e6658f630033c5ed35c013dfebf24b7bb351c49b1d710b9d7a24514df5786
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA512:75f870a0e6e19b8975f3fdceee786fbaff3eadaa9ab9af01996ffa8e50fe5b2bba6e4c22c44a6722d11b55feb9e89895d0151d6811c1d2b475ef4ed145f0c923
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA512:39e5879d4879003ba5e1fcb727f91f7661cede12692ae128110328a6c1c5a1e2f79a1329ee4d065f3cc3e0d3d18423f5b5a5b170b5cb49c6888de90d31dcaf9c
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6build1.debian.tar.xz' attr_2.4.48-6build1.debian.tar.xz 27332 SHA512:eed6bb2b3869a23ab89c0349bb1bd1b7c51fb2f225291d49d08c19aa501af81e2fa650b46a5369bb87011413236eacc91b1f468d33630d6af5e3cf12adc68084
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


### `dpkg` source package: `base-files=11ubuntu16`

Binary Packages:

- `base-files=11ubuntu16`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `brotli=1.0.9-2build2`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2build2`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

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

- `libbz2-1.0:amd64=1.0.8-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

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


### `dpkg` source package: `cdebconf=0.256ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.256ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

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

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6ubuntu3`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `dpkg=1.20.5ubuntu3`

Binary Packages:

- `dpkg=1.20.5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `e2fsprogs=1.45.6-1ubuntu1`

Binary Packages:

- `e2fsprogs=1.45.6-1ubuntu1`
- `libcom-err2:amd64=1.45.6-1ubuntu1`
- `libext2fs2:amd64=1.45.6-1ubuntu1`
- `libss2:amd64=1.45.6-1ubuntu1`
- `logsave=1.45.6-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `expat=2.2.10-1`

Binary Packages:

- `libexpat1:amd64=2.2.10-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/expat/2.2.10-1/


### `dpkg` source package: `findutils=4.7.0-1ubuntu2`

Binary Packages:

- `findutils=4.7.0-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gcc-10=10.2.1-6ubuntu1`

Binary Packages:

- `gcc-10-base:amd64=10.2.1-6ubuntu1`
- `libgcc-s1:amd64=10.2.1-6ubuntu1`
- `libstdc++6:amd64=10.2.1-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19-2.dsc' gdbm_1.19-2.dsc 2603 SHA512:ca70a14f93b56b42eb87a820e04b8402075b1048cce0e39a1fd337cc3551dba9803db931ef8a0b50e3f9e5cb6d553df8bdf12f8908fc27c49de2670c0c3812d9
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19.orig.tar.gz' gdbm_1.19.orig.tar.gz 967861 SHA512:118c5b8cdf74898bfb7c2100302fedf80096be017bf08e80a44486563cad5d93b93567622f2e7c7aceb72f30460504bd0b4ddfccf34df994ed65166e12ecd495
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19.orig.tar.gz.asc' gdbm_1.19.orig.tar.gz.asc 181 SHA512:db24d7438a22a8c7974d7aa889f72e1abf402fa56dcbefa19b3cc6ffe08c73f9a251b898de548eaec50759102ebe3df486ebb785e90d571f7c8f10715e3c15d0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.19-2.debian.tar.xz' gdbm_1.19-2.debian.tar.xz 16228 SHA512:36f7bb8e249c5b03840d7ad859cbb4cb6d71f9485cfafbaef219aef78954d17e5e1056289c13c2c1ede67a04f53e7532f02187faa6c8c2b4cb0402a6ee541a79
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


### `dpkg` source package: `glibc=2.32-0ubuntu6`

Binary Packages:

- `libc-bin=2.32-0ubuntu6`
- `libc6:amd64=2.32-0ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gmp=2:6.2.0+dfsg-6ubuntu1`

Binary Packages:

- `libgmp10:amd64=2:6.2.0+dfsg-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

- `libgssapi-krb5-2:amd64=1.17-10ubuntu1`
- `libk5crypto3:amd64=1.17-10ubuntu1`
- `libkrb5-3:amd64=1.17-10ubuntu1`
- `libkrb5support0:amd64=1.17-10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libbsd/0.10.0-1/


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

### `dpkg` source package: `libffi=3.4~20200819gead65ca871-0ubuntu3`

Binary Packages:

- `libffi8ubuntu1:amd64=3.4~20200819gead65ca871-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libffi8ubuntu1/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `libnsl=1.3.0-0ubuntu3`

Binary Packages:

- `libnsl2:amd64=1.3.0-0ubuntu3`

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

### `dpkg` source package: `libpsl=0.21.0-1.1ubuntu1`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libsemanage=3.1-1build2`

Binary Packages:

- `libsemanage-common=3.1-1build2`
- `libsemanage1:amd64=3.1-1build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libsepol=3.1-1`

Binary Packages:

- `libsepol1:amd64=3.1-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libsepol/3.1-1/


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

### `dpkg` source package: `libtirpc=1.3.1-1`

Binary Packages:

- `libtirpc-common=1.3.1-1`
- `libtirpc3:amd64=1.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libtirpc-common/copyright`, `/usr/share/doc/libtirpc3/copyright`)

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

### `dpkg` source package: `libxcrypt=1:4.4.17-1ubuntu1`

Binary Packages:

- `libcrypt1:amd64=1:4.4.17-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libzstd=1.4.8+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.4.8+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libzstd/1.4.8+dfsg-1/


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

### `dpkg` source package: `ncurses=6.2+20201114-2`

Binary Packages:

- `libncurses6:amd64=6.2+20201114-2`
- `libncursesw6:amd64=6.2+20201114-2`
- `libtinfo6:amd64=6.2+20201114-2`
- `ncurses-base=6.2+20201114-2`
- `ncurses-bin=6.2+20201114-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/openssh/1:8.4p1-3/


### `dpkg` source package: `openssl=1.1.1f-1ubuntu5`

Binary Packages:

- `libssl1.1:amd64=1.1.1f-1ubuntu5`
- `openssl=1.1.1f-1ubuntu5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `pcre2=10.35-2ubuntu1`

Binary Packages:

- `libpcre2-8-0:amd64=10.35-2ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pcre3=2:8.39-13`

Binary Packages:

- `libpcre3:amd64=2:8.39-13`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pcre3/2:8.39-13/


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

- `libreadline8:amd64=8.1-1`
- `readline-common=8.1-1`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-1.dsc' readline_8.1-1.dsc 2418 SHA512:aeb4b2a55e583565f64c2185e684c0e7cfcb0256831fc509f18f0d98a7b48d6fc5c1b76f41e2bdeab285f10731c2423c39c5fcc679ce111c2a4d359177394fe7
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.orig.tar.gz' readline_8.1.orig.tar.gz 2993288 SHA512:27790d0461da3093a7fee6e89a51dcab5dc61928ec42e9228ab36493b17220641d5e481ea3d8fee5ee0044c70bf960f55c7d3f1a704cf6b9c42e5c269b797e00
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-1.debian.tar.xz' readline_8.1-1.debian.tar.xz 29220 SHA512:e199bbcbdb999235b388daf537d2b6cce0a2a7ed29eab9f76ddee9ceedc16ba7d63c082b1eeb9769f432f86d2d6fd55d99a7227cbf393f3b5581f5d6f164f556
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

### `dpkg` source package: `sqlite3=3.34.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.34.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
- `libblkid1:amd64=2.36.1-1ubuntu2`
- `libmount1:amd64=2.36.1-1ubuntu2`
- `libsmartcols1:amd64=2.36.1-1ubuntu2`
- `libuuid1:amd64=2.36.1-1ubuntu2`
- `mount=2.36.1-1ubuntu2`
- `util-linux=2.36.1-1ubuntu2`

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


### `dpkg` source package: `wget=1.21-1ubuntu1`

Binary Packages:

- `wget=1.21-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

- `liblzma5:amd64=5.2.4-1ubuntu1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu4`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu4`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

