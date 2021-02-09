# `buildpack-deps:hirsute-curl`

## Docker Metadata

- Image ID: `sha256:e7324159953107a66098448c6643b8f41cb22afc8ae8d21b612b19bfcf483ad0`
- Created: `2021-01-21T07:52:45.422562514Z`
- Virtual Size: ~ 103.38 Mb  
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

### `dpkg` source package: `apt=2.1.18`

Binary Packages:

- `apt=2.1.18`
- `libapt-pkg6.0:amd64=2.1.18`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.1.18
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.1.18.dsc' apt_2.1.18.dsc 2784 SHA512:5b61b2c916b34aa4a0c5b9ae42475c973d6fee2271e2b61c388ae56662847c19e57bbede8b770e0107642fe0365ce5c35662d46d71091e8f709cb6ab3a7a0756
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.1.18.tar.xz' apt_2.1.18.tar.xz 2192808 SHA512:4e2db10fdb84e92152ad0e47429ff84a5dc126e018dc57f51e4662946d28771d79e6dbbe7680249cdcb6d18a378d73266fb9be58b6dd3844af0b56ce33c5bfd1
```

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

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.5-3ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-3ubuntu3.dsc' audit_2.8.5-3ubuntu3.dsc 2854 SHA512:d3264720dd890f7900b13d3346792f522856038369eaa9d3d10ec68d9105a13a14bdd2c3aafeb29cec31f174c058cba04e0474e430567325770425086d43d18b
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5.orig.tar.gz' audit_2.8.5.orig.tar.gz 1140694 SHA512:7d416aaa21c1a167f8e911ca82aecbaba804424f3243f505066c43ecc4a62a34feb2c27555e99d3268608404793dccca0f828c63670e3aa816016fb493f8174a
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-3ubuntu3.debian.tar.xz' audit_2.8.5-3ubuntu3.debian.tar.xz 19984 SHA512:695c0dcab50d9675471eb7dc4d7b9d0dfd43f9b3a165144fad87203dea63c49ced94b4dbe1c43fc8f1f6063da338b8a25f277f70d07fd51d7e675634c228d575
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

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.48
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.48.dsc' base-passwd_3.5.48.dsc 1757 SHA512:cf4eeec8ee970f47c35d851cd1813622c64a9cc3852f6d1134d2415f0c2f16b295a8fecfe7ad7b021a1f01449512b2cd0140cb42897e8c6968f4589a68fb01e6
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.48.tar.xz' base-passwd_3.5.48.tar.xz 53080 SHA512:9a7c39e7e196e2a78de0ebde926326eac96cbe676d8f5791416241c23c01b85cc9870a1dd96da0f37bdfdf1b32e4458eb3cbd2898091e9dd5ca3f082578e2d95
```

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

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20200601
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20200601.dsc' ca-certificates_20200601.dsc 1582 SHA512:ebb9a92fe43ee91e24a1fc57276cabf2b34317af0ddb7fdab2d69d2ad96b442bbf9fe8b7feb8fbcbeda6e84d25635f6d58c37e4ce489d4b4951bc1d3887c0224
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20200601.tar.xz' ca-certificates_20200601.tar.xz 245668 SHA512:7bfd3122430be0a46bd10dcb0e0664561d1e0b2656b9f37677d89f71a1dcb0e668c25ffe08412888125fa9a53ee8245a4b3fc1004c419a159766665b1241113c
```

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
- `libcurl4:amd64=7.72.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl4/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.6-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.dsc' e2fsprogs_1.45.6-1ubuntu1.dsc 3328 SHA512:3c1fc4edd9823e43796442423ea114a9e1f5dcc07559b0c9ee1cdb417d8e043aabdfd7272a21dc2669a8b4886244c73b4248289b3d239205296a62c3d91cc46b
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz' e2fsprogs_1.45.6.orig.tar.gz 7938544 SHA512:432483cb0e32f96169014ca7ef4e053e5d64c6b934ea6f48a86cfd9e01187802ea6a5b13db62e14f4fa3745254c3587a115d560059c1d4995a41273f14f91f8c
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz.asc' e2fsprogs_1.45.6.orig.tar.gz.asc 488 SHA512:afdfebae62948899125802515a01302edd4d9ce8519c83714af133d33f17a9ce2aebbf686ee5f850a2d34a700f362df5c52ac4ea6a49fb71b6fb207a29ed7602
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz' e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz 81276 SHA512:86002f00c0a4968ca15083a98c14c5791d177451b7f1e6270d63698ba1a3a2cfa6547560afe6b60eafe6f52c1908e40488848d8568db263d5a596f3b3e00378f
```

### `dpkg` source package: `findutils=4.7.0-1ubuntu2`

Binary Packages:

- `findutils=4.7.0-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.7.0-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu2.dsc' findutils_4.7.0-1ubuntu2.dsc 2409 SHA512:41cd927580386a080a7ef3728f284abd579935b5d87c8eb1ed6cbef1df19a03ee3a3644bb5a1240a72d31105d3c432c949eaab8d26e02ed0426cf5fb166e545a
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz' findutils_4.7.0.orig.tar.xz 1895048 SHA512:650a24507f8f4ebff83ad28dd27daa4785b4038dcaadc4fe00823b976e848527074cce3f9ec34065b7f037436d2aa6e9ec099bc05d7472c29864ac2c69de7f2e
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz.asc' findutils_4.7.0.orig.tar.xz.asc 488 SHA512:a4868a6f36d7224f05a19096a9ef2e1eedfdc77beb5d4098b0c94634cf9a757d47e2ccdf3451f48c45667a1fa3f30e209a022bf287cad6b3109b37cccea0cb72
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu2.debian.tar.xz' findutils_4.7.0-1ubuntu2.debian.tar.xz 28212 SHA512:9f6eb5bb161ec7b224ce0d6edecc19a425779fc539627e9c053a46e53d3b232336adb5a75a56a5e60b2e4507be87d335c802d49e63f63d8727fd20b8c8025665
```

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


### `dpkg` source package: `glibc=2.32-0ubuntu6`

Binary Packages:

- `libc-bin=2.32-0ubuntu6`
- `libc6:amd64=2.32-0ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.32-0ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.32-0ubuntu6.dsc' glibc_2.32-0ubuntu6.dsc 8950 SHA512:d145765fcc0cc1108b777fffc1344c134c444dcf128689dd35cf77df7a16c87120670348d14c36224d8a530ae64d504bd744812c45c4f62ec17778b93a0fe37d
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.32.orig.tar.xz' glibc_2.32.orig.tar.xz 16744512 SHA512:8460c155b7003e04f18dabece4ed9ad77445fa2288a7dc08e80a8fc4c418828af29e0649951bd71a54ea2ad2d4da7570aafd9bdfe4a37e9951b772b442afe50b
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.32-0ubuntu6.debian.tar.xz' glibc_2.32-0ubuntu6.debian.tar.xz 872612 SHA512:ec2e3b72e99356c738276e7a403b7fcc1e879bd4fb739953e39cd3e76db63bafcd16cb3449f2b046c57e07ce84c96ccd8e45e135661d8cf966c08801564bde9a
```

### `dpkg` source package: `gmp=2:6.2.0+dfsg-6ubuntu1`

Binary Packages:

- `libgmp10:amd64=2:6.2.0+dfsg-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.0+dfsg-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6ubuntu1.dsc' gmp_6.2.0+dfsg-6ubuntu1.dsc 2230 SHA512:3c81d30c5ffde286ca315db3226e22887d4828b3534355fd8900d855d650679a58732de176c7569b98cf59b65b77644e09e06b9909289a07bb8d1330b6e8db9a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg.orig.tar.xz' gmp_6.2.0+dfsg.orig.tar.xz 1842912 SHA512:6ed6df69ced53b13e3e2d64d94f8a34c3257abd4c0967f16d48b064956e260a3d8fb424c84d47dca6d1308bd16b347af3740fce68ebd2d45f1d7f752422c2496
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6ubuntu1.debian.tar.xz' gmp_6.2.0+dfsg-6ubuntu1.debian.tar.xz 54484 SHA512:0c1e932f495d69f886d4b2118ee4eb10587a0164a36c0c0f4c5302ec3aa9960ad9c1a68afab6ef220c2a4bfaa1dea7522410a224b69c253ce497ac6d6198475a
```

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

Source:

```console
$ apt-get source -qq --print-uris libassuan=2.5.3-7.1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.dsc' libassuan_2.5.3-7.1.dsc 2627 SHA512:c6d456a6aa7c4588117c84f17b9e97bb84707fe043b97dd5bb0739b35cfce7aae8713db9753fb07c028cc8581056ae8b8599ae652c13ef96c715413fffb5b885
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA512:e7ccb651ea75b07b2e687d48d86d0ab83cba8e2af7f30da2aec794808e13e6ec93f21d607db50d3431f1c23cb3a07a2793b71170e69fa2f5a82cffb81961f617
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA512:df57f8e575164b0e030d88c57bafe83249add41a551597a7527680cfa351244ae99da295231911e9ac9d8e609383ff0150e852a0383f3d7c68f04036c37c4019
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.debian.tar.xz' libassuan_2.5.3-7.1.debian.tar.xz 13952 SHA512:f13525a7fda448bf878adf858c06ab9bec8df7d9e2d58a7f16bb6808d6459a988a4212e69526b1bb2990af19cfeffc1f30844606f5e3f398d6533b5342a07d5e
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

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.44-1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1.dsc' libcap2_2.44-1.dsc 2179 SHA512:ca21c07ef21e169de98a324a71e2384107e38e1511b6e22e64bdbc141145ec73d3ba1d469d7afdac12dcdad3fd05c63b879205daed6df1f7a03c9e264aed561c
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44.orig.tar.xz' libcap2_2.44.orig.tar.xz 125568 SHA512:1bb323ca362923bd6bd0e2e4639cf8726975165a620a243b31e797056439eb7efb2bfbc8e5521636783a86c7415b2037b1638c98747b79183ca7d3d42a04ff20
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1.debian.tar.xz' libcap2_2.44-1.debian.tar.xz 21116 SHA512:9404455fc1a9306036eb3c748fffdecb0f5c8e92a3692d42ef8b8dbdc259405c50bd24a6c3b963d955f9ea6a7989a38058d8f9abe265b671450f54842063daff
```

### `dpkg` source package: `libffi=3.4~20200819gead65ca871-0ubuntu3`

Binary Packages:

- `libffi8ubuntu1:amd64=3.4~20200819gead65ca871-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libffi8ubuntu1/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4~20200819gead65ca871-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu3.dsc' libffi_3.4~20200819gead65ca871-0ubuntu3.dsc 2179 SHA512:3daf83b86b96208b825523ccdbb3900fe00d189b87811b57d661a3ab43e3b9e5b631ccb7fd2723a2df655b56c643fa0e2733c35f08c2732756eb59852bc85e00
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871.orig.tar.gz' libffi_3.4~20200819gead65ca871.orig.tar.gz 527371 SHA512:c349b1630db80c042f3c11efe58d4eb849e87f2cca0cc1748c99d32cc34ce4c1262825dc070c8a84263e0adcd8a7af3bd33c705ba28b6cc16974552b12bf0c65
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu3.debian.tar.xz' libffi_3.4~20200819gead65ca871-0ubuntu3.debian.tar.xz 7856 SHA512:5496d2d4147aa2ca5e579c149206d2cb1db39f14f7d351b4224496b3289b68f83a8715366bcad933fa798815e8aef416270c77576aaca2a921a7ae5c4b8abb3e
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

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.38-2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2.dsc' libgpg-error_1.38-2.dsc 2220 SHA512:3806e8a764b6cb8cab4b86d7af19afb680c438b05e0357521137cf950edc1bcb75c368f3a0864b639ff9ed1528febcb604fa7818827fd29d180ba65bc39e44c3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2' libgpg-error_1.38.orig.tar.bz2 957637 SHA512:b936a4738c2cee111d855b1ba3ec433da8c77799a87d1f71275f974f871ebfa593c9db06ea53f0490b6cd6b94bef34f6052a587a4d13d839ec0128500c2dd9de
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2.asc' libgpg-error_1.38.orig.tar.bz2.asc 488 SHA512:0f167c6d87f8028c294db2822c2e092f156504893c0bdd8bf883d00dcdd838fed4af5fd3726ab88d41f4e12e8b131cec45dcc610aeb25291ea870d3b9cb621f6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2.debian.tar.xz' libgpg-error_1.38-2.debian.tar.xz 19544 SHA512:319731a51f785d6a0b250dfa9c7ee3951692c051d1d161d2cef31dd20f25662af47edbdf71a85bc5ecbcf423846dc43df85e0af5a8d2734ddae0927e72626128
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

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.1ubuntu1.dsc' libpsl_0.21.0-1.1ubuntu1.dsc 1986 SHA512:c9f9e473f2e96a141b79e3adfc3b0828423cdd281ed19757b3226be91655568dc31466bedd9cf8752555bcb485d226aba9c662dd05070d8ee24082115923909a
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA512:b7466edb9763f94a65330dbb3c19586f9c7b01e20ddedb38ca2fd4c9ee5764a4f9b3291dc4b76659b45425d954f15973345f917b2cd2de72ea731e8c41f2a265
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.1ubuntu1.debian.tar.xz' libpsl_0.21.0-1.1ubuntu1.debian.tar.xz 12892 SHA512:4e9a51728285a2292a1e1e45786d099a13536e8b6d28493101fbc7e0d28dc95de70c3dba35d976cdcb1d129fb9a52a07c91e16b47b2e1309d45a4d360dae575c
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu6`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu6.dsc' libseccomp_2.4.3-1ubuntu6.dsc 2564 SHA512:f271dc13939c977a48f69710c84856f595516968e8f6ee40a85aed21b30b9e81c2d35ce3014089e856c4493aaabf95e1cf32cb813f0a5d5255a30e1ede337b73
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA512:7b7af2e98493243ffe1934fefff5723b24ae9b9bdc4bf039343ee8456c15acb0ea34e81ec292a41143848272aeca794ef92ad38fc3f42c77465170cb540479ef
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu6.debian.tar.xz' libseccomp_2.4.3-1ubuntu6.debian.tar.xz 36448 SHA512:7b2ccc657b51c5547e9c6094996e0f1803258e9876330521746a2e1718fcf2a871894c83b9a8b37aa5814fdaea9dc9a37361f9b131c120c4cac0b7e034bb2d6b
```

### `dpkg` source package: `libselinux=3.1-2build2`

Binary Packages:

- `libselinux1:amd64=3.1-2build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.dsc' libsepol_3.1-1.dsc 1776 SHA512:74a0dd6f3db6578261b78114f46030cd0486b05d0482421bacb5a74a30cbdc98932691c60293d96e5fd258839136d8e0988eb0371cbd6e685b6bce38e0a95bc7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA512:4b5f4e82853ff3e9b4fac2dbdea5c2fc3bb7b508af912217ac4b75da6540fbcd77aa314ab95cd9dfa94fbc4a885000656a663c1a152f65b4cf6970ea0b6034ab
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.debian.tar.xz' libsepol_3.1-1.debian.tar.xz 14584 SHA512:e7c48cde2e2d8748f4df3b6b02c66ffb97ee21c2b749b2d7c9154ac4d4c73fd09a383972ac39edcb6f04faf2631c1dba3512b6622b612e1aec54bc58608df5db
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

Source:

```console
$ apt-get source -qq --print-uris libtirpc=1.3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.1-1.dsc' libtirpc_1.3.1-1.dsc 2111 SHA512:68980155c1303e49dcc383a50bfc9ecab5ebf9a6d0f104f8e7185b59fdbafb8174f4063052c74b0c96a4e3082d71c890d6e5ff06876cbc9f19687bf75f0ad5a0
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.1.orig.tar.bz2' libtirpc_1.3.1.orig.tar.bz2 513399 SHA512:131f746800ac7280cc3900597018fc8dbc8da50c14e29dbaccf36a6d110eded117351108c6b069eaac90d77cfec17014b08e9afddcf153fda2d780ba64260cbc
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.1-1.debian.tar.xz' libtirpc_1.3.1-1.debian.tar.xz 10788 SHA512:d31c143dd18d601ad3b34e2ae63ba8ba2c3b30e69cf83a1e969d13701f9f8085a95a302ae0c496af9791712c7b0cf403209e69e005916c47d0aecf5912d9fa9f
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

### `dpkg` source package: `libxcrypt=1:4.4.17-1ubuntu1`

Binary Packages:

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

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.3-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-0ubuntu1.dsc' lz4_1.9.3-0ubuntu1.dsc 2063 SHA512:e917ff5cd900ae41f8cafb12311c18c9e9bb995581f734100e4eff54b0d6d9d94cdc24c24d30042e18bc28224b3bf96be535446da7afdace8e72e3aae4b31f49
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3.orig.tar.gz' lz4_1.9.3.orig.tar.gz 320958 SHA512:c246b0bda881ee9399fa1be490fa39f43b291bb1d9db72dba8a85db1a50aad416a97e9b300eee3d2a4203c2bd88bda2762e81bc229c3aa409ad217eb306a454c
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-0ubuntu1.debian.tar.xz' lz4_1.9.3-0ubuntu1.debian.tar.xz 12736 SHA512:cdf2da740f844dcb9ffaa91997d7299cc9ca4cfef801c36789b35540f44dd18598aab7f0097b930ebf53d75298a00f6634808bc139d9109cd9102693dd21c78d
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

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2+20201114-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114-2.dsc' ncurses_6.2+20201114-2.dsc 4106 SHA512:9669f4921c9c42b983f0a786ad69829ba6b1bcc43804709a6e55c136dfc7d977e8d1da38ed5d4bf6e23290486a105148eea41a4274c978f64715e0424e30c456
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114.orig.tar.gz' ncurses_6.2+20201114.orig.tar.gz 3539796 SHA512:d163bc8f08f6b2406f8f562fecd9035e0e6f2db8b539cbcaeb4a80b15027b518026526eac1b2681da82b8d03dd1c924a85de1294e6ace2a5dbc03126512a3e2c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114.orig.tar.gz.asc' ncurses_6.2+20201114.orig.tar.gz.asc 265 SHA512:210035a4ec94cdb650ac4cf7990791dc482ea941b410dcf635525fa3282df28464a1b8c0e5a4721868ccbe2609bae2db3632ecd166d239ef84471c536ce81f9c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114-2.debian.tar.xz' ncurses_6.2+20201114-2.debian.tar.xz 51812 SHA512:22a41b42ca7adf57664affe702fa71e40ed26b72da7bb3a1b9a4777f1b708fc80793bd552a802c1be02da42ba0ca8ebb12be462e27b779bbaaab46de190bd3a8
```

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

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.42.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.42.0-1.dsc' nghttp2_1.42.0-1.dsc 2548 SHA512:4c8ef93c4f0e938ece2a09b5edd6e8a15ce55602ed37046b9a5f43636a9b2432e51f6d1c82d242b5d5009665d8c09436b4477cb7691f9ea29109c2b784915a54
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.42.0.orig.tar.bz2' nghttp2_1.42.0.orig.tar.bz2 4523037 SHA512:920ff7642e4994c83c56acedf82d9026d1e256e5f2613ea228a1876ab6b85e910f3aa16b422bbb52f93f47847deb254585909e5201f30246e363869a91a6a7e4
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.42.0-1.debian.tar.xz' nghttp2_1.42.0-1.debian.tar.xz 16352 SHA512:70c30cfe0906dc516001e57b13edd3ae1702a942e0ec742d937a716ad3d576754bb75a50fd067866d6406fb495446b95179673921e6bd7cd6dd8a46d9d7fb583
```

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


### `dpkg` source package: `openssl=1.1.1f-1ubuntu5`

Binary Packages:

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

### `dpkg` source package: `pcre2=10.35-2ubuntu1`

Binary Packages:

- `libpcre2-8-0:amd64=10.35-2ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.35-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.35-2ubuntu1.dsc' pcre2_10.35-2ubuntu1.dsc 2199 SHA512:3f4f1ff57adfa7d4394bdf95b48689f38fb6176f9b4ee8d402045bcca80c8bd158cd8b6b7f504238f18e348340e5295f6584fc758ce05f84e23934d0f2f0bb42
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.35.orig.tar.gz' pcre2_10.35.orig.tar.gz 2299082 SHA512:f9386de9211919da68ad0882dbfb72b344306280b3c4515f496cff4e3ff5c11e29fb71539a357a43a71ef668a742a54cc327a1dc3a00c767fbd0264933beecee
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.35-2ubuntu1.diff.gz' pcre2_10.35-2ubuntu1.diff.gz 6824 SHA512:804c0e95e52d92f8960d7224a2aa5393a749cfbef39d5a0466f1f208854661d1f1c7d17e0b6ec7a61f7288a93f7f3629ec2afceb97cf26262413b40f85cd6aeb
```

### `dpkg` source package: `pcre3=2:8.39-13`

Binary Packages:

- `libpcre3:amd64=2:8.39-13`

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
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.0-6.dsc' perl_5.32.0-6.dsc 2997 SHA512:f3ba6e772589db7af38c7eb50c88d93494191c03854d0e838961035f79d3ab08d595e7d24aed4f16d1962fd8a7f0269af0a68f2e68aacb6662f1ae2a741ff384
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.0.orig-regen-configure.tar.gz' perl_5.32.0.orig-regen-configure.tar.gz 833536 SHA512:e9e224f39cfca20957048ba0b64412c298d896b78ec5b4ac6e638a2600fe9cbc52467a54e2db98ad36ec393500c2a728cc216feafc55b429cf81f476cba97069
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.0.orig.tar.xz' perl_5.32.0.orig.tar.xz 12717336 SHA512:1540247415893bbd94dfeede7b4fba6052688dc0bf27ced817f448246fcdc6e9a6486abc34577dec5b00bf02ed607b2d24ccd4977c3b3c51e8e6edfc0b81c760
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.0-6.debian.tar.xz' perl_5.32.0-6.debian.tar.xz 164248 SHA512:ecff08e71574c9dfa6838442d729811ca72f8e606bfd73847619052a9ebe7e9788a69d460ef7d357031b6cdba325b66699ecad10c7dbc555f464425e37b4dbc7
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

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.34.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.34.0-1.dsc' sqlite3_3.34.0-1.dsc 2410 SHA512:889eada39d276cdeb7baa52ef194320ec80ffa8a1fd4b68ddd8d8c720e4bfbf0d2975e60048bd763607dc833e4d35fdb97c6ee13c1ddc8a5ae08c31a9bb9e245
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.34.0.orig-www.tar.xz' sqlite3_3.34.0.orig-www.tar.xz 5539580 SHA512:1a77b68150204c911fea20e342142c6aa0d2407085a5355ca0069d4fbf9cfdd35ef75c29658ab64f48dc5214ec5ad2fb73cdc7306d62ab2371dfbe4fec3d4551
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.34.0.orig.tar.xz' sqlite3_3.34.0.orig.tar.xz 7340388 SHA512:ca08bf0db197e4e1c5a1f7d5f93a843b2c2c3e6c141fd6f56a09d3c5940f9b1c1ded942be437a93bc9080851138b466edc8a6a2edee144626049f441fac81586
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.34.0-1.debian.tar.xz' sqlite3_3.34.0-1.debian.tar.xz 21456 SHA512:cee0cc17a8091c7e25386245025e94f69da383e35a6550cb26cc8916daf8742948776f726d9aa7ac808faf8b7351d1f468189d3ee6c34516334ed7fa94fffb94
```

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

Source:

```console
$ apt-get source -qq --print-uris systemd=247.1-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_247.1-4ubuntu1.dsc' systemd_247.1-4ubuntu1.dsc 5341 SHA512:58c4ab65a6910ba3630688512cac025c9864054fa2d9ff6fb15978b8aed614f27ee9218942e89a747f2a15d7381075ca3b60c3c5a1e0f94975d1bed2fb67b0cc
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_247.1.orig.tar.gz' systemd_247.1.orig.tar.gz 9889494 SHA512:2a737afcee4409c2be073d8cb650c3465a25c101b3c3072ea6e6a0614d06e3ed7ae55c84f9ae60555915ad1480b3a13aa72fef4b9210139afe6b0d7a7629385a
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_247.1-4ubuntu1.debian.tar.xz' systemd_247.1-4ubuntu1.debian.tar.xz 192828 SHA512:468225c9219ae7e814200cbe8d616b22a8d0d36bc9b3ee3169f06a7dd3f325929b2be91f4b47ce75debbe5871e73c6253ffad39b47d4e9ab3fe20981b8dd4fa8
```

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

Source:

```console
$ apt-get source -qq --print-uris tar=1.32+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.32+dfsg-1.dsc' tar_1.32+dfsg-1.dsc 2015 SHA512:f14fd11f940bf1a14e9c1d23408d75195e9ce52dace1ace1a20ab0c73742ccb3a8d7b329e8f457a6fecb7405e9ead50623809ea90307fb7a036da14d6310eef0
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.32+dfsg.orig.tar.xz' tar_1.32+dfsg.orig.tar.xz 1910772 SHA512:a2bd8eb0afbb08fdf7a5df8ce7c915dd2871bc2cecb3e3f7f175ebfd5f2182c52a28ea7b78ff2a64d247085e41a1b22e79e004b30a9e85dd23bf0908c46712de
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.32+dfsg-1.debian.tar.xz' tar_1.32+dfsg-1.debian.tar.xz 19460 SHA512:601411c7752e60e5e6d8a76ae94c20cd590d1d7c88e140b4cd0943616d42ed0976d0e1b46a8a9f395fece5b6ac31f9892639fc022a23e193a6ca7345d61de4bb
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

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2020.06.17.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.dsc' ubuntu-keyring_2020.06.17.1.dsc 1863 SHA512:84bb35395c9b1c42171b4418434638e2aaef6e389bc2f6388c1a32b0f747524784d4e69b1a5f18ed095de045b97df8ed486bffbd3a3fbfedbdb360209a2420d4
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.tar.gz' ubuntu-keyring_2020.06.17.1.tar.gz 36420 SHA512:33009928eeeadbe1627b77f7db1aba32cf1e59d2fd6767bcd0d441d3521cb2b07c5bf06be86e8426c96b9661786a958b2e978f12d8f0941d1ac79289d977eeaf
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

Source:

```console
$ apt-get source -qq --print-uris xz-utils=5.2.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.dsc' xz-utils_5.2.4-1ubuntu1.dsc 2629 SHA512:09c0668c76bd1653460ae2207f2666785d6ec7bae424d168e2f5dc2c98d2c34b7f983963be27c39ac05df0ad76ccfe088b55a64a09319f26b785544d5c8ffb66
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA512:00db7dd31a61541b1ce6946e0f21106f418dd1ac3f27cdb8682979cbc3bd777cd6dd1f04f9ba257a0a7e24041e15ca40d0dd5c130380dce62280af67a0beb97f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA512:dbfce0556bc85545ce3566a01c25e4876f560409fc2d48f2dc382b10fbd2538c61d8f2c3667d86fc7313aec86c05e53926015000320f19615e97875adae42450
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.debian.tar.xz' xz-utils_5.2.4-1ubuntu1.debian.tar.xz 135512 SHA512:9ec339da084b6aedd5d9dfafe879f7b90ae6dc473458dd8eda234e087f3aa80480b7b0792b54588d57e1b41a2c42f28ef87b8e6a8cd4bb51d43e2517f701724f
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu4`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu4`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu4.dsc' zlib_1.2.11.dfsg-2ubuntu4.dsc 2945 SHA512:afe11a895b3c5355d897543fb74716c2c78c2c273a51f75f53b10a49c678217d31ef7ed6b66a3d3423263dd918379d356bd47da139a3468adcdf2ecb18195a5a
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu4.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu4.debian.tar.xz 50768 SHA512:bd064f5baa8feec0fedb0406169a1a9ba0ba6bd0a581efbaa7c43e88707a429b26dfe3b7eacaa5f6657c3ab29320896473ba6418374583bc2602e3dd9de839af
```
