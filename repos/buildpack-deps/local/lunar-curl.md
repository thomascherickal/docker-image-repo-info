# `buildpack-deps:lunar-curl`

## Docker Metadata

- Image ID: `sha256:7e37d1b86e663a732896bf3d39af7f0224e89bee8471e9c1bba9e4e100eaf04a`
- Created: `2023-03-02T03:37:57.125837231Z`
- Virtual Size: ~ 95.48 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
- Labels:
  - `org.opencontainers.image.ref.name=ubuntu`
  - `org.opencontainers.image.version=23.04`

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
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1-3.dsc' acl_2.3.1-3.dsc 2508 SHA512:4162efc9071c57eeced2c4faa9b13c8f46dac98d7876db14c7bc37ec526c02f2a2aced5b828f594bfa101d37a594573e865b856a96538a524df66b715082e15c
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1.orig.tar.xz' acl_2.3.1.orig.tar.xz 355676 SHA512:7d02f05d17305f8587ab485395b00c7fdb8e44c1906d0d04b70a43a3020803e8b2b8c707abb6147f794867dfa87bd51769c2d3e11a3db55ecbd2006a6e6231dc
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1.orig.tar.xz.asc' acl_2.3.1.orig.tar.xz.asc 833 SHA512:be046f3bf1ac7e21d2a07bf6ea87c1fedeed2f9d370d8bf3de1aa0c448de5484b1523697415849b6b7ca23e48e3df5353f6aebe850eb20fc2044d2681c71f298
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1-3.debian.tar.xz' acl_2.3.1-3.debian.tar.xz 30968 SHA512:a29af03f79bf6cd50852c9538013458b8bdb579c2059df1682120ced75bf8023b32a4f4c2fff8466364d1c97ad4113f84fdfbdc1c991b3f5a7fee2b1db2692d0
```

### `dpkg` source package: `adduser=3.129ubuntu1`

Binary Packages:

- `adduser=3.129ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.129ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.129ubuntu1.dsc' adduser_3.129ubuntu1.dsc 1794 SHA512:f61cb4ccb94bdcb1c36eeb455af9ec6b0aed3772668e16b7316291a432036702098f6652e66d1337a563870c8786bb5636ef7e900b4a369fc58c7c80f86e6ec9
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.129ubuntu1.tar.xz' adduser_3.129ubuntu1.tar.xz 236628 SHA512:04ff19eb83e37b293744e16c1fa7af988906e387c56ca6c2dcc23c7d0270c7483ca5437631b7a946d463b89dc3f9754e74aa80bd0e7a3bef933ed13aaedcc6f6
```

### `dpkg` source package: `apt=2.5.5`

Binary Packages:

- `apt=2.5.5`
- `libapt-pkg6.0:amd64=2.5.5`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.5.5/


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
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1-4.dsc' attr_2.5.1-4.dsc 2477 SHA512:acb8f17654b972fa6a9ac4701b863cff73313af8f86feaf1cf1f276a1484f02cef6fe9b6a39c4223bd1773163d223f611dbf1807dc655b3b557595130ab39290
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA512:9e5555260189bb6ef2440c76700ebb813ff70582eb63d446823874977307d13dfa3a347dfae619f8866943dfa4b24ccf67dadd7e3ea2637239fdb219be5d2932
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA512:be4f3629ef66bd400bcdeaf8b6b1564dc729472a514d59fb4909a30f3269711dedea16002283e9aabbf83c374e0a3d70bc00f1136da0fed66a8184acdfd7e78f
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1-4.debian.tar.xz' attr_2.5.1-4.debian.tar.xz 32152 SHA512:933e59fb9dd43bf3b250dbc36276a52484271e893a96efa85648148ef84f5059b79152dad341fe6dbf5ab9dd71290e8aa6e7ceb4923ccecfe42046c096d29efe
```

### `dpkg` source package: `audit=1:3.0.7-1.1`

Binary Packages:

- `libaudit-common=1:3.0.7-1.1`
- `libaudit1:amd64=1:3.0.7-1.1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/audit/1:3.0.7-1.1/


### `dpkg` source package: `base-files=12.3ubuntu1`

Binary Packages:

- `base-files=12.3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=12.3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_12.3ubuntu1.dsc' base-files_12.3ubuntu1.dsc 1253 SHA512:1337275ab0357ea5a42082ac2cce9ce7a9b521a4d2763ec98d9875351cf189b59ba78cbda607bd620839cab1a12a2fdbdb5087f0d946377ba8cb7cd19ae2d573
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_12.3ubuntu1.tar.xz' base-files_12.3ubuntu1.tar.xz 92740 SHA512:fff32fd198950ea232c1efe5e3aebb86880c49f3f93175d4245ec512dd40563a7b2720da82941872f3bb4777a360652e3e02411bb97ed338f4a5e0247618af62
```

### `dpkg` source package: `base-passwd=3.6.1`

Binary Packages:

- `base-passwd=3.6.1`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.6.1
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.6.1.dsc' base-passwd_3.6.1.dsc 1740 SHA512:b631fac3bb17d25bca3a04d74a542dcb7a97f29bd98da38dabd4c38ebfeb9638466876e20e60ea9b86f8168cc50f5ae2153a9a59d635114ff10bc9425a7a998e
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.6.1.tar.xz' base-passwd_3.6.1.tar.xz 56072 SHA512:f26df2acbd103c60dd2003bc72ce043c05f66009464245d2740e4389374687e7c67114ee2120dab79546a29f9b5bd29fd8321f758fc7db32165125c4286593a8
```

### `dpkg` source package: `bash=5.2.15-2ubuntu1`

Binary Packages:

- `bash=5.2.15-2ubuntu1`

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
$ apt-get source -qq --print-uris bash=5.2.15-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.2.15-2ubuntu1.dsc' bash_5.2.15-2ubuntu1.dsc 2450 SHA512:2c4deb119d02436a930af8b6965823de57c636bedcfc9482e399fea4793f604542c8fc70d2aff522f589fd5f1f5f84b37b397d269897e913257201de03e42a82
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.2.15.orig.tar.gz' bash_5.2.15.orig.tar.gz 9997221 SHA512:8322b26b8fd185a8c366970ce346075b4df76676d6e0f78c33d8bcac8c04a8e87bcf7cf74f5e259d90a750aa146b8baec69d1d2c2c12d26ea93472847c8dcd1f
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.2.15-2ubuntu1.debian.tar.xz' bash_5.2.15-2ubuntu1.debian.tar.xz 103652 SHA512:b02e631ab2500c0633138e6c7fe682db4d138b9904d86c495e9d17ccff78ed5a88471d4e0288b7fabd98abc2398e1029b8f4a23f4d7550474c720addaf041bb2
```

### `dpkg` source package: `brotli=1.0.9-2build7`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2build7`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2build7
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build7.dsc' brotli_1.0.9-2build7.dsc 2285 SHA512:ae62b6933300cd10c65559f6d94e03a4fa6404168042a52481cfbc87715f05258a5c3b1cec00e1dd33c5111fa3d46d43dd3ea53667e71559ae88a9eae81e56f6
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build7.debian.tar.xz' brotli_1.0.9-2build7.debian.tar.xz 5836 SHA512:03247406da55d9742fcf3aed6a4ba6837887483b9e737b9fc7b8554e5103dd09cd0f48dd7832aabaa50ab06a2a7076856d6a95dc6debd3c4bb8d9557ae35d1b5
```

### `dpkg` source package: `bzip2=1.0.8-5build1`

Binary Packages:

- `libbz2-1.0:amd64=1.0.8-5build1`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-5build1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-5build1.dsc' bzip2_1.0.8-5build1.dsc 1860 SHA512:dfb9cd3a99f8c80a27e088b6ba7f06f50bc2bdbc61f574ed8f77d0fa58ff07fa1c34a060351fd4b601537181143dd934caadd7a00eb97aea5933febb7b61743d
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA512:083f5e675d73f3233c7930ebe20425a533feedeaaa9d8cc86831312a6581cefbe6ed0d08d2fa89be81082f2a5abdabca8b3c080bf97218a1bd59dc118a30b9f3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-5build1.debian.tar.bz2' bzip2_1.0.8-5build1.debian.tar.bz2 26870 SHA512:e030c257c3458d780fd0ffc6f328efd69d0e875e81acd7441a7c6651194ebded61017c96aad7c99061f93d50dfc33056abe98c9a599abc900f49d51c4a1eed6f
```

### `dpkg` source package: `ca-certificates=20211016ubuntu1`

Binary Packages:

- `ca-certificates=20211016ubuntu1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20211016ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20211016ubuntu1.dsc' ca-certificates_20211016ubuntu1.dsc 1846 SHA512:2cb0046a5407819dc4e6a7017e60a4c1c12898824cbae55a0638710e0829fcf6401202b7758e10d73e268fa6618c2feb9f37d6d29dacafa5acd993fd7c1494b6
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20211016ubuntu1.tar.xz' ca-certificates_20211016ubuntu1.tar.xz 239852 SHA512:3097abc8c4e60cb52990940ad0974d95e3a63d49d43563d73aaf7d0b57f822a0584b23cb0a94674de2505adb3985e7dc79553984b7f96507803d4acdbba96578
```

### `dpkg` source package: `cdebconf=0.264ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.264ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.264ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.264ubuntu1.dsc' cdebconf_0.264ubuntu1.dsc 2898 SHA512:f34fac21b8ef101bf2e2503aa55964be0050c1fb0d689034a1b3d9df5181acacd497e44c3f2e83898b461f6fa44043cf99d757412fbf7761c8e946182acc3331
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.264ubuntu1.tar.xz' cdebconf_0.264ubuntu1.tar.xz 282992 SHA512:5a6683e2e5f42747558a4f333ff50ac6acec3b7e4dae48aafdd48a721ccfc2fc4c1666038df9879a494df4ab08c3095f813f94d71864cba9a174c7c674f89c3f
```

### `dpkg` source package: `coreutils=9.1-1ubuntu2`

Binary Packages:

- `coreutils=9.1-1ubuntu2`

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
$ apt-get source -qq --print-uris coreutils=9.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_9.1-1ubuntu2.dsc' coreutils_9.1-1ubuntu2.dsc 2010 SHA512:342d3531f615940dea8fb45d15dad65903f785fa6393b4c55a5c53e2fa80d2a51d3ee2878a92e5145dd4be50b827d9c42932218f836f905f20008fe1b3635e06
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_9.1.orig.tar.xz' coreutils_9.1.orig.tar.xz 5712104 SHA512:a6ee2c549140b189e8c1b35e119d4289ec27244ec0ed9da0ac55202f365a7e33778b1dc7c4e64d1669599ff81a8297fe4f5adbcc8a3a2f75c919a43cd4b9bdfa
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_9.1-1ubuntu2.debian.tar.xz' coreutils_9.1-1ubuntu2.debian.tar.xz 38492 SHA512:54c46926e87c50345823d4d8dcf977bd172cc81be821991e5bdd698056ca919293074e23d59502727e0e93a08ff780bb9b53ac997e57894926ae08b079afb736
```

### `dpkg` source package: `curl=7.87.0-1ubuntu1`

Binary Packages:

- `curl=7.87.0-1ubuntu1`
- `libcurl4:amd64=7.87.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl4/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris curl=7.87.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.87.0-1ubuntu1.dsc' curl_7.87.0-1ubuntu1.dsc 3107 SHA512:59f98f1adb587cce5bb46a88f7f479687720d845c2328ed760791868ed68da87f773d54a7ec0adc08666deed1d75a3dda23babe842d5d0fb42d49f6a91fd0649
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.87.0.orig.tar.gz' curl_7.87.0.orig.tar.gz 4291127 SHA512:939be5a7d82f7ed4e96173639aa50f5e6748b387d3f458f3845c584ad24d15d77b8cd64f4f2dc11bcc207b097d125d1dc713a9769964e3d4766182a217e9898d
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.87.0.orig.tar.gz.asc' curl_7.87.0.orig.tar.gz.asc 488 SHA512:de7405f14bf4e2573a3070fba9ead65bef3e5bbe3911175aa7d5152c84ee28137d5c07f4827d51c63fc9057a8106cf8f169ecc6e9f5d1a8a9b092d26d744f3f9
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.87.0-1ubuntu1.debian.tar.xz' curl_7.87.0-1ubuntu1.debian.tar.xz 39424 SHA512:a6d239ae89ad4768777dfb7653029d2b866cafdfaf3a8fcd19c34e5e97793b7c1fdf6979b4f6a0a96bd28df4de2049d75c796c09fe8f437320121a2a8d8f2303
```

### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg-10`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg-10`
- `libsasl2-modules-db:amd64=2.1.28+dfsg-10`

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

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg-10
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-10.dsc' cyrus-sasl2_2.1.28+dfsg-10.dsc 3324 SHA512:3a29dc8eeb056b889b2894c126efa6da5ce21e39e2ef64d6e8411caae36f50940815fce2e09bc6d31df20d8c3c738ee048ecdd6f6f48d93105875186209442e1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg.orig.tar.xz 797472 SHA512:70cccbac70e71828f1345beba5c78c14332e425b75c84a66393cf62ecf6848741c5912697fc0197516f1d4c41ec8c9644506a6241588b8f6bf5bba79edd8b15a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-10.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg-10.debian.tar.xz 97056 SHA512:b3da3c50696e60e5ee97811423ceb0d54fec0f3c8da02b21c47ee96dd476790adc948b42ae0df3ced4373371913b09eb975fe830197710ebb71918822e0f8d92
```

### `dpkg` source package: `dash=0.5.12-2ubuntu1`

Binary Packages:

- `dash=0.5.12-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.12-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.12-2ubuntu1.dsc' dash_0.5.12-2ubuntu1.dsc 2116 SHA512:dc5d7fcb5214df2cde5a0decc4f4ca69c688aefc4873a5b61e1943dcdd5527dda09376a118cd52ec21a4250a3e53bf067bbb3b51099d685b3f0663df07729a1e
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.12.orig.tar.gz' dash_0.5.12.orig.tar.gz 246054 SHA512:13bd262be0089260cbd13530a9cf34690c0abeb2f1920eb5e61be7951b716f9f335b86279d425dbfae56cbd49231a8fdffdff70601a5177da3d543be6fc5eb17
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.12-2ubuntu1.debian.tar.xz' dash_0.5.12-2ubuntu1.debian.tar.xz 38724 SHA512:14f001c8b0d2f9018551fc1899c7f0602ae2e2bfa52d1bb276e09ecb70450c917e550db27fe80cf0041976c96a24c368e6c5711ceae245486346442def3e6bed
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-1.dsc' db5.3_5.3.28+dfsg2-1.dsc 2887 SHA512:066dba82587633d175cc4547a76ea4977655456d829fa75a626949723a63b03ec9acfe84a6f4d0ca07638cc2f0a8f67af227c8cbe287850846f59cd42eeaddb9
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2.orig.tar.xz' db5.3_5.3.28+dfsg2.orig.tar.xz 21287688 SHA512:f9c9d042702ef3fcfdd4b4859583048f3396b161009dc24b6d3a2c53533d58214239fc80e2c42db17e9f092df44d531502737f3b368b956bff49ef057b6b51ef
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-1.debian.tar.xz' db5.3_5.3.28+dfsg2-1.debian.tar.xz 34660 SHA512:48d5d4572db4dd48539b7753a3e6abc9578616ca3c73a66fd9dc058a6efefdc653dbe0658bc1f45e4b7a11bf69d9d626529d3cb65fe67d23b6584a3804da1f9d
```

### `dpkg` source package: `debconf=1.5.82`

Binary Packages:

- `debconf=1.5.82`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.82
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.82.dsc' debconf_1.5.82.dsc 2035 SHA512:bca5b8290d54709a706faaef77f16fb98fc074e7aacc8a40d650f4a76c1d843b8a2534cadbfe9f6170e6d4892b82d76f2fb16e474fb82bcc5e616024fae68be6
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.82.tar.xz' debconf_1.5.82.tar.xz 571540 SHA512:5a9b26d90cf02e6f5b267e6e6416e91ac31115b124b05b4edd2dd785eea92a6d9c060f591dad6645784ff956a07555cb1bf11a35f4712d5bc308c4b6726da88a
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.7-0.4.dsc' debianutils_5.7-0.4.dsc 1737 SHA512:91f750cac588110e2790b886a5408152411fa0a1df78f6e6544fedc19200a5efc7e9da417ee152b077ddb5a87c68bd8130314f628879acb30724fe240fc4293e
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.7.orig.tar.gz' debianutils_5.7.orig.tar.gz 257231 SHA512:79acd8885abca93842d696167171a359011c49a40f38deeb25bc94d62905f95afa3a7b2540d3bd4b0ffd363c5c48a439a1a68139a29d6c033980b019cea75d92
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.7-0.4.debian.tar.xz' debianutils_5.7-0.4.debian.tar.xz 22412 SHA512:dff3affac8165446b05a911fcc54c4d0db0491f0bdba3f0e1464f2f6bc3020f607a4df324edbc59b72a02df5cd3351804763bb7a2b20785f0453fd30c0fec25f
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8-4.dsc' diffutils_3.8-4.dsc 1705 SHA512:b666ab8c76ddda9262d84f00e17b5139bae88d612233332e75f51f18975177460e6891cb3b28e20d8a9311df9aaa927a280cf4a7855d566e9569154e1237ae7e
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz' diffutils_3.8.orig.tar.xz 1585120 SHA512:279441270987e70d5ecfaf84b6285a4866929c43ec877e50f154a788858d548a8a316f2fc26ad62f7348c8d289cb29a09d06dfadce1806e3d8b4ea88c8b1aa7c
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz.asc' diffutils_3.8.orig.tar.xz.asc 833 SHA512:0464ac89209411993800666b45ff90243d22fbda53bf1d71c6870d565b39cc8d9c54c141b9d297a181ce74ad8fb5313953f416bced179ff7728a52a3e9a4f5a5
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8-4.debian.tar.xz' diffutils_3.8-4.debian.tar.xz 14428 SHA512:874a41a50f6db1b91a358445513a22a24871be830a10a9d192ac2957fa91a4c3e2265472fcf08f867b21a1c125b192ca559cc77c5ad51e35275a635d58ae1c8a
```

### `dpkg` source package: `dpkg=1.21.19ubuntu3`

Binary Packages:

- `dpkg=1.21.19ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `e2fsprogs=1.46.6~rc1-1ubuntu1`

Binary Packages:

- `e2fsprogs=1.46.6~rc1-1ubuntu1`
- `libcom-err2:amd64=1.46.6~rc1-1ubuntu1`
- `libext2fs2:amd64=1.46.6~rc1-1ubuntu1`
- `libss2:amd64=1.46.6~rc1-1ubuntu1`
- `logsave=1.46.6~rc1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.6~rc1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1-1ubuntu1.dsc' e2fsprogs_1.46.6~rc1-1ubuntu1.dsc 2957 SHA512:053deb1cadfbb95b9894216ec1a1fb90d32cba597dfd3da9e2b3895b032fa4c1ed2eaa3434158db46775a40a0296d60e9f1383905331827221df50807a9475bf
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1.orig.tar.gz' e2fsprogs_1.46.6~rc1.orig.tar.gz 9615342 SHA512:2b6afe2f8b5c83fd061bf72fe507bdc22206b1a781d3baecca693a6744f203715e8e6dd6e7864dfa853c85e72f4e94a813ff362ea8e43c0443025ab644550648
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1-1ubuntu1.debian.tar.xz' e2fsprogs_1.46.6~rc1-1ubuntu1.debian.tar.xz 85224 SHA512:d9ee270014468c1a00b7ada6715e3b3479b6d2f3bd3c6b044aad670304cfad4ab1bf275bc359642ca0c4d2c4d46ced52ba7740b3711ea974a75e11240d908dbd
```

### `dpkg` source package: `findutils=4.9.0-3ubuntu1`

Binary Packages:

- `findutils=4.9.0-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.9.0-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0-3ubuntu1.dsc' findutils_4.9.0-3ubuntu1.dsc 2066 SHA512:0967a16fb4f83f749314e0e61ecdd112b2ba2e6c8bc2da1650e85cb45f4e4f489cf03e80bb96248fb0d3fe5fe91167cf84840d68e5f6b5fb977a284e5199029c
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA512:ba4844f4403de0148ad14b46a3dbefd5a721f6257c864bf41a6789b11705408524751c627420b15a52af95564d8e5b52f0978474f640a62ab86a41d20cf14be9
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA512:b8e0b5471242912a20b9e468fa27b7f27339af5f7be8918173105262dee0152183bf4cf516844d348b206a694e028490d5d3b190f3aed8c698ba5444941f8dfc
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0-3ubuntu1.debian.tar.xz' findutils_4.9.0-3ubuntu1.debian.tar.xz 28484 SHA512:2aeef5a8931606e3aec4f6e4f28c560d564b6bf43f2c459b189514a96fba4837104ba04ed1fdef75d101b5055f5692df47615369317e10f36f2d03e28b09dd24
```

### `dpkg` source package: `gcc-13=13-20230215-1ubuntu2`

Binary Packages:

- `gcc-13-base:amd64=13-20230215-1ubuntu2`
- `libgcc-s1:amd64=13-20230215-1ubuntu2`
- `libstdc++6:amd64=13-20230215-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-13=13-20230215-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13-20230215-1ubuntu2.dsc' gcc-13_13-20230215-1ubuntu2.dsc 27878 SHA512:40420c326666257a75fe583a73e0d1693e9b196ebf1a98b0d33d168fac9a110e544f4ac754197ae19f62fc7af7b3edf285aa4d9e5ffcee2121c8c5c7b62f7035
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13-20230215.orig.tar.gz' gcc-13_13-20230215.orig.tar.gz 87845313 SHA512:5009465ba6b292c8915d8dab8f9c3a9e139e43f0389d187d477a9e2410e761e39697f5723a6a8105882d498ea53ab28407d309f6b30ca0971db29e020ae8bcad
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13-20230215-1ubuntu2.debian.tar.xz' gcc-13_13-20230215-1ubuntu2.debian.tar.xz 530440 SHA512:b4fec4f9b6177e06d9803944206907feac165a4b18be3012e70c5bd5ae6040c9ca171f75180a95dffabe94a11892d4b68a9668a68cabafe5d35acab329f64ffe
```

### `dpkg` source package: `glibc=2.36-0ubuntu4`

Binary Packages:

- `libc-bin=2.36-0ubuntu4`
- `libc6:amd64=2.36-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.36-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.36-0ubuntu4.dsc' glibc_2.36-0ubuntu4.dsc 8718 SHA512:c731c14abae40b97be15d00a53ba478862e32dbd21e3a859220d4d08e56e300236c9dc12f7646d14bfd70a3b83fe720e5198defab0fac7f860b4b13c10f08874
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.36.orig.tar.xz' glibc_2.36.orig.tar.xz 18610836 SHA512:9ea0bbda32f83a85b7da0c34f169607fb8a102f0a11a914e6bf531be47d1bef4f5307128286cffa1e2dc5879f0e6ccaef527dd353486883fa332a0b44bde8b3e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.36.orig.tar.xz.asc' glibc_2.36.orig.tar.xz.asc 833 SHA512:b6999ebc4067e08950207e9c67f5172c6d43144e6680677bf3d93093c2270cb4c6e75f9ad37a60e7fec243141fd64b4348782c5794fcf03be363adf0b4543d53
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.36-0ubuntu4.debian.tar.xz' glibc_2.36-0ubuntu4.debian.tar.xz 931048 SHA512:6a70647fceb9f8db048865685f0101b45a87291bbd0b10780ed45a0e9c8ff353edd31ade36976e05cf7e95d479e24d08b7d0eb972330bc9d806be461d58baa66
```

### `dpkg` source package: `gmp=2:6.2.1+dfsg1-1.1ubuntu1`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg1-1.1ubuntu1`

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
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg1-1.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.1ubuntu1.dsc' gmp_6.2.1+dfsg1-1.1ubuntu1.dsc 2345 SHA512:24359c1bbfc542ed29b17994362a473a716a90c43f9edb631473fae5d8fd6260726872b70c216dcd2185436f8273a044968d381df1dfa3fa2d4f8bffcc44fadb
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg1.orig.tar.xz' gmp_6.2.1+dfsg1.orig.tar.xz 1787428 SHA512:705b8de10ed61e00d3124a6ba4de7075dde1addc32282cc410513de136f0b5c3c769adc37bfd629c1f7208ab6ba0332f2dbe236208e2cf06b2528ea64ddc31af
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.1ubuntu1.debian.tar.xz' gmp_6.2.1+dfsg1-1.1ubuntu1.debian.tar.xz 39516 SHA512:67d948ba1f1da4c1d220ea948088633ab329ee6aab2a8c7e02af24f5eec1f3fd5377a7a486e09e9f53f45bb8639e7f11ae23479a36cf61c91799ea00cda26706
```

### `dpkg` source package: `gnupg2=2.2.40-1ubuntu2`

Binary Packages:

- `dirmngr=2.2.40-1ubuntu2`
- `gnupg=2.2.40-1ubuntu2`
- `gnupg-l10n=2.2.40-1ubuntu2`
- `gnupg-utils=2.2.40-1ubuntu2`
- `gpg=2.2.40-1ubuntu2`
- `gpg-agent=2.2.40-1ubuntu2`
- `gpg-wks-client=2.2.40-1ubuntu2`
- `gpg-wks-server=2.2.40-1ubuntu2`
- `gpgconf=2.2.40-1ubuntu2`
- `gpgsm=2.2.40-1ubuntu2`
- `gpgv=2.2.40-1ubuntu2`

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
$ apt-get source -qq --print-uris gnupg2=2.2.40-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40-1ubuntu2.dsc' gnupg2_2.2.40-1ubuntu2.dsc 3949 SHA512:5024ecb689bd1761b0a339f5a7b84abf09d74d19919eff7e2963c03f778736428c0e9b90a814bbeb1ab76be9f5ea781b3b8b8b2325ead1f7abce371a8fe2080f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2' gnupg2_2.2.40.orig.tar.bz2 7301631 SHA512:4c2f5fbf37ba6fbad0045aad23129186963010c673ea0b81801adc4f98efe14d6c7228e22815b6b26307c1fe5bb51cd088aa6a0f06a9325d3c021849ef81c594
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2.asc' gnupg2_2.2.40.orig.tar.bz2.asc 228 SHA512:50e8abae322430bf4d3230d0291ca519663a1397fe0d0b8df29076808504b5fea2b984952d6dc51ecc239c12af8ecd5d93b88dd1c6bc0babf0b48a5a840b8ada
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40-1ubuntu2.debian.tar.xz' gnupg2_2.2.40-1ubuntu2.debian.tar.xz 65128 SHA512:052a619ac71b39e2ed5e8f5390b6fcdbacf3c98247a71a2026980c9640e0f0b717b2053e93c3f57590323f35973110a53fa50d31ec963c840d14dd4de7e87307
```

### `dpkg` source package: `gnutls28=3.7.8-5ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.8-5ubuntu1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.8-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.8-5ubuntu1.dsc' gnutls28_3.7.8-5ubuntu1.dsc 3496 SHA512:8a493bae4b585f683db6df3c43ca0f6c5b3a5a3d6db0767a807d76130f5ed6894c271af53c39989c2dfff1816cd6420ec1fd9b74679c20d1b71a10ace6f9ca35
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.8.orig.tar.xz' gnutls28_3.7.8.orig.tar.xz 6029220 SHA512:4199bcf7c9e3aab2f52266aadceefc563dfe2d938d0ea1f3ec3be95d66f4a8c8e5494d3a800c03dd02ad386dec1738bd63e1fe0d8b394a2ccfc7d6c6a0cc9359
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.8.orig.tar.xz.asc' gnutls28_3.7.8.orig.tar.xz.asc 1760 SHA512:f6aa8c7e263e7413d469d5bf045ece612337e6d5cfdd0618191a27aa0d01050a03ffef9c8b92e3bae3d1f0355102797c9d96b1e83b3f02bcc9582d64651bc2da
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.8-5ubuntu1.debian.tar.xz' gnutls28_3.7.8-5ubuntu1.debian.tar.xz 89872 SHA512:a0d67b507173da8ad127dc19d584f81229857fd24c7928f1008b1025343f4a9aeceff5ef9dd4eb0eb07e4ae78683f6f1828f16260575fe3b3990c54652109b3d
```

### `dpkg` source package: `grep=3.8-5`

Binary Packages:

- `grep=3.8-5`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.8-5
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.8-5.dsc' grep_3.8-5.dsc 1608 SHA512:612ae21b8e6e9ce8075b6f3c5b5684aac3778269f532f7f0d1f2c9f378e323184533e297710bbe0a91883b268c68a83fc37f0192abc62172ac78c894b979b2d0
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.8.orig.tar.xz' grep_3.8.orig.tar.xz 1709536 SHA512:2014519a80c6dcd799837e1bd7d9d5ebe8729ec54b0dc76981dac4755a9a8a9f200470cdcc911e2825bed8162e61da39e3dd60289f7393b48bf67314077d0c79
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.8.orig.tar.xz.asc' grep_3.8.orig.tar.xz.asc 833 SHA512:8266b58485f225c2189814e3898c72e59d251b729e0c302d31f57abdb7ac2e6e28dde2c5c8095673b6f007b2a3ebc26db1dca910a7771aba80dad4b3c6761ee4
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.8-5.debian.tar.xz' grep_3.8-5.debian.tar.xz 21048 SHA512:1fcc73636f525c5843dd3d17e8b26bf35fdf3299efbb6c23625f0340058e793fb47318f41f80a76a328242add2a5d9797b67393b1fcb2053afa134ab23d4d74d
```

### `dpkg` source package: `gzip=1.12-1ubuntu1`

Binary Packages:

- `gzip=1.12-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.12-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.12-1ubuntu1.dsc' gzip_1.12-1ubuntu1.dsc 2303 SHA512:8b6f5ada04f3dbcb891f9af31a28cf1a161392f98f78724088752981a3453474b32ad2f7312c683bd65fba6b6fe14b26bbacbe462a3204acfe614f7c0f217ff5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.12.orig.tar.xz' gzip_1.12.orig.tar.xz 825548 SHA512:116326fe991828227de150336a0c016f4fe932dfbb728a16b4a84965256d9929574a4f5cfaf3cf6bb4154972ef0d110f26ab472c93e62ec9a5fd7a5d65abea24
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.12.orig.tar.xz.asc' gzip_1.12.orig.tar.xz.asc 833 SHA512:1f4702797f7c5f1873c2f9c2f6210ba23824455d17ee82f50f0bf24240ed5bdf0090cf85338ccf76ba82422f8b4ad3a329d8bbf1350cb094d7bd61aa45550397
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.12-1ubuntu1.debian.tar.xz' gzip_1.12-1ubuntu1.debian.tar.xz 19796 SHA512:247ee91f2d67935a809248c8134789a57e13db3534e7d7c5e0ab543a4b1024cc39c29b3fb2fc5805b42f87004187601e642c45fd1f51baa80b21441786e64da7
```

### `dpkg` source package: `hostname=3.23+nmu1ubuntu1`

Binary Packages:

- `hostname=3.23+nmu1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23+nmu1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23%2bnmu1ubuntu1.dsc' hostname_3.23+nmu1ubuntu1.dsc 1567 SHA512:95f3a3ae2197f342fbac41664b2aca64bac415a9b7675364f256512207fadfd2476786e186781c05724fcf0b1d37cbfa1560c6f363e27495e5d35efea92483c4
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23%2bnmu1ubuntu1.tar.xz' hostname_3.23+nmu1ubuntu1.tar.xz 13124 SHA512:c14a9a7e39812ba6be3a3ed62f1e95815437e78b8edfa4a0daa7fc5939a22b522df51eed30ef96940082cae95a9a53f1988e9740d9b423b728dfa5995f92937d
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.65.2.dsc' init-system-helpers_1.65.2.dsc 2195 SHA512:146e1c34d482c36a528ec7f4c3dab6398d4e23af8aeb5a993b565fe88fb76aba38b647a075fae9d6ffa1848392fb995eda76f1971c3ff28436461e6aefafe6fe
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.65.2.tar.xz' init-system-helpers_1.65.2.tar.xz 44400 SHA512:b65d8c4848188a16a3dc52f5c2535566b472898aad5b455fcd2c4600884257e41f081cb5876630536af14f5bd9d92d379493882a7d53a7dee3a2b3007b12f85d
```

### `dpkg` source package: `keyutils=1.6.3-2`

Binary Packages:

- `libkeyutils1:amd64=1.6.3-2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.3-2
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.3-2.dsc' keyutils_1.6.3-2.dsc 2079 SHA512:25176970cfeccf59c7c798042029ff78150ad2f8a1a6871aabd34c8d8bf9cb7c7ef2b1cfe78cbd7b61207a21512de703bee26d580b2a2bc62acc4722ba6e186c
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.3.orig.tar.gz' keyutils_1.6.3.orig.tar.gz 137022 SHA512:f65965b8566037078b8eeffa66c6fdbe121c8c2bea7fa5bce04cf7ba5ccc50d5b48e51f4a67ca91e4d5d9a12469e7e3eb3036c920ab25e3feba6e93b4c149cf9
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.3-2.debian.tar.xz' keyutils_1.6.3-2.debian.tar.xz 13196 SHA512:cda54c621a40334005373a1dc90f93f3e1f6b5c5e0cbbd6299312526e77cc05e4e2eed4473e7e7f06847b5b47a7f2aee377362540ee48c9f38a5f5cf37931132
```

### `dpkg` source package: `krb5=1.20.1-1build1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.20.1-1build1`
- `libk5crypto3:amd64=1.20.1-1build1`
- `libkrb5-3:amd64=1.20.1-1build1`
- `libkrb5support0:amd64=1.20.1-1build1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20.1-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-1build1.dsc' krb5_1.20.1-1build1.dsc 3913 SHA512:0591c14d26d615d33ab75a3e2c5ac066ce141279eff023100a999aadd0adf4adf80212777bcc7f0409b43854303c1f6d9fc7398294bb6c62bdfc2893ba4f78b5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz' krb5_1.20.1.orig.tar.gz 8661660 SHA512:6f57479f13f107cd84f30de5c758eb6b9fc59171329c13e5da6073b806755f8d163eb7bd84767ea861ad6458ea0c9eeb00ee044d3bcad01ef136e9888564b6a2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz.asc' krb5_1.20.1.orig.tar.gz.asc 833 SHA512:1d3312bd67581e07adfdadf2c5fe394179631d8add8bd075efefe982a0de22369004e60a14422d426382c8c591e4181b9897088afe9d4e86f0b5a97e5954c67a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-1build1.debian.tar.xz' krb5_1.20.1-1build1.debian.tar.xz 99504 SHA512:f0fa16ef6c12296bf612f99f0b8f833cd9def044e6e4b62238fba31e5c5a34113a31273b0ad8784c2cbbdef746d5fac83d58ea007bec729af92226dfcbaa9d57
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5-5.dsc' libassuan_2.5.5-5.dsc 1997 SHA512:a9adc6bb30d71df875e9250ba43fb11cedc25f626d8478887e5c513c15fa85b649d8b19f4bd718852bc407d2e511563439a6bfbfd692499ed94d71a3610ff01a
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2' libassuan_2.5.5.orig.tar.bz2 572263 SHA512:70117f77aa43bbbe0ed28da5ef23834c026780a74076a92ec775e30f851badb423e9a2cb9e8d142c94e4f6f8a794988c1b788fd4bd2271e562071adf0ab16403
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2.asc' libassuan_2.5.5.orig.tar.bz2.asc 228 SHA512:343336ea5dffa113cd934167f548faf4e85d31bf64a46541ee6828b4d0995a8cc9d0668995812d9c4d3ab73347d5b1bbfff0d6ed586fbf4bbc57ac42e828e8d5
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5-5.debian.tar.xz' libassuan_2.5.5-5.debian.tar.xz 14256 SHA512:e52d0e524f7a8a97f128fd4ea91d6755c842a58044cf541b55bbdff1326c31671f446094e8517826f992b00da41a6a5e3432a8eb1f46b76abae3b2d1894255dc
```

### `dpkg` source package: `libcap-ng=0.8.3-1build1`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1build1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libcap2=1:2.66-3ubuntu2`

Binary Packages:

- `libcap2:amd64=1:2.66-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.66-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.66-3ubuntu2.dsc' libcap2_2.66-3ubuntu2.dsc 2311 SHA512:e3f662805aeba4846e21fe980a60fe237f12a5ce35f6d6e0639d090643367f2c77b016508cef1a843cd31d3564c0352ada74ab4045174b23bc4aeea8375135b7
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.66.orig.tar.xz' libcap2_2.66.orig.tar.xz 181592 SHA512:ac005b622f6e065f30ce282a5c87240e7b9da75366ee537aa4835bc501b44bc242c10a4ba4dc070e2415fc7f635d1c3c4e45fbeeaf962cf7973dda82bf6377f0
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.66-3ubuntu2.debian.tar.xz' libcap2_2.66-3ubuntu2.debian.tar.xz 20612 SHA512:2af5d8c5cc20d192d95646728eb0ffc383c980f63f5e8565046b3ff53351c7d7e07a25dd89e3795d2d41f5a271cc97f2e9d778aa880e4a1c15c00f16137eb735
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.4-1.dsc' libffi_3.4.4-1.dsc 1951 SHA512:cfcf127389ffec7a5a32061cc39c39af23c1d78b113e72598c2e1a76d4f0e5b9d621eda2f59c20beac243f87eb11d459a158bb9e7d3ec37e17b70dc8a298db42
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.4.orig.tar.gz' libffi_3.4.4.orig.tar.gz 1362394 SHA512:88680aeb0fa0dc0319e5cd2ba45b4b5a340bc9b4bcf20b1e0613b39cd898f177a3863aa94034d8e23a7f6f44d858a53dcd36d1bb8dee13b751ef814224061889
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.4-1.debian.tar.xz' libffi_3.4.4-1.debian.tar.xz 10380 SHA512:6fdf678230a0ce9a6e70eefe20429705a497cb8e710a89a33695381274110bc6c022c80250668d2786e0264b743ae0b6db88550f45aec0485c606c56ce80dad9
```

### `dpkg` source package: `libgcrypt20=1.10.1-3ubuntu1`

Binary Packages:

- `libgcrypt20:amd64=1.10.1-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.1-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-3ubuntu1.dsc' libgcrypt20_1.10.1-3ubuntu1.dsc 2897 SHA512:b5e69531652bb05971db3e0d1704d3b8621ca1539d99ba03ac47fcea0c9a7ac98dc4e0c3e352888641906cefac04ae6619cafbade8a9074d1464f0b0eec7fa88
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2' libgcrypt20_1.10.1.orig.tar.bz2 3778457 SHA512:e5ca7966624fff16c3013795836a2c4377f0193dbb4ac5ad2b79654b1fa8992e17d83816569a402212dc8367a7980d4141f5d6ac282bae6b9f02186365b61f13
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2.asc' libgcrypt20_1.10.1.orig.tar.bz2.asc 228 SHA512:dc74b1029ce1909466eeb9cbdbf77b3e3fd2093ef40ea81bd1b9860eb11d1994087a9b575b6c94ed22f64d0f7e8d2999e30c7ea60fd90a2ecf99ddb60cd156c6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-3ubuntu1.debian.tar.xz' libgcrypt20_1.10.1-3ubuntu1.debian.tar.xz 41952 SHA512:927cf224f23d313fd68c0d9d2300e426dccdc5311a08df7e2c588b847adefec09f984061cd666805930269bbbdda37cd6c79a34d76b16b5211ca8e5a9acbc269
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.46-1.dsc' libgpg-error_1.46-1.dsc 2273 SHA512:84eccc5384bcf780ab23867740b9f18993b0c64d8881230dbaeb7837ff33dcde7bba7510068e3ec1e8080a0e159ed60b4f8e52d23177d0a27dc0ccae6a1e43fe
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.46.orig.tar.bz2' libgpg-error_1.46.orig.tar.bz2 1014291 SHA512:b06223bb2b0f67d3db5d0d9ab116361a0eda175d4667352b5c0941408d37f2b0ba8e507297e480ccebb88cbba9d0a133820b896914b07d264fb3edaac7b8c99d
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.46.orig.tar.bz2.asc' libgpg-error_1.46.orig.tar.bz2.asc 228 SHA512:89f5561f8539cd1c39c6e5d5e51cfc27d1d8525dbafb27efed5ffc9c8e19533b2aa5b83df1357e9f85b182ead46dbd3e4d1bee707554fcab7238f36f2ae1a1f9
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.46-1.debian.tar.xz' libgpg-error_1.46-1.debian.tar.xz 18532 SHA512:20865fad9fb3781df9719874a67ee66a341eb1fa3bc1cd90630ba9103a38d33a9ce2b12d395bbc42e59840b0e800491ab60e8564418b8dcbd955236d8a8bb1e0
```

### `dpkg` source package: `libidn2=2.3.3-1build1`

Binary Packages:

- `libidn2-0:amd64=2.3.3-1build1`

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
$ apt-get source -qq --print-uris libidn2=2.3.3-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.3-1build1.dsc' libidn2_2.3.3-1build1.dsc 2663 SHA512:cd07a7bf26d7fcbd6fc559154cdd0ee4eceb1b16a9b4fb0ff67f28f2df477ccfa63c43f639c3838cd4da1c86b2b1fb5bc6b68ed06f93c9d5eb9b6f17f79bb648
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz' libidn2_2.3.3.orig.tar.gz 2116946 SHA512:2dd0201b5224b3eb6a5667e53c9a2beb6e6aefefab23060a70f143bb5d447029e8f4200e4e0460a4fab51767f0bdfc9583a0cc757652bee58f5593106dd18274
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz.asc' libidn2_2.3.3.orig.tar.gz.asc 228 SHA512:bad901350e21ff39f0385685c13b3f366cd77dad59c736547773f9555531bc56022982c3fb6fffd5b82624bdd3ea8bd1806e531f80a06c77e4e46b08f18f08a9
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.3-1build1.debian.tar.xz' libidn2_2.3.3-1build1.debian.tar.xz 16092 SHA512:a7e7c19d48b676b7b083c6f55a3cc9880dec316e4f28166255839d0824e2b67ff753509c627eb89a84e514d3661bd4d23800bb6cea0c902d7bbb958e3e9083ba
```

### `dpkg` source package: `libksba=1.6.3-2`

Binary Packages:

- `libksba8:amd64=1.6.3-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.3-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.3-2.dsc' libksba_1.6.3-2.dsc 2482 SHA512:30b9393ab75dd1d704eabf31077cf0cf938af1211ea42dba06eca3abc54da0bcadfd7d6b18e175f35bb371d279e1fa821122219b3158df91c15cee2a0afa77e8
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.3.orig.tar.bz2' libksba_1.6.3.orig.tar.bz2 668287 SHA512:188f6d27b4904c10cd54ba949c1132dd6c167f53dd1b77eae39c5b8e3ac8b15e87b2a54cdfddac95ac4ed41ee83c3d4e1b17d95126f245b6c204fade6739a2ce
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.3.orig.tar.bz2.asc' libksba_1.6.3.orig.tar.bz2.asc 228 SHA512:fb9e49b4ce0bb14b0009b52f687c01ae57e6465b298555702536ae7a76b0807d05a6033dfc2058d5cdd9313401d55afcc98f60cee4440af03d1aa14e063c2c27
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.3-2.debian.tar.xz' libksba_1.6.3-2.debian.tar.xz 14636 SHA512:6d31b7fb155a0f2e243f4ad4482f6cc36d0d87cea9bdfb4c0d641b974c3dde020973012e86226a3ca94def5f18e1d63daab16b8e9b359a1ceca7016d33f4e1ee
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4-2.dsc' libmd_1.0.4-2.dsc 2264 SHA512:d06f3e257f79d1a49af24ab198487ebbbc695ef593eb40c951888f1fdaec80e50df2d4ae590442b742506f314f29677c54b3f2c28ea439e8e5ac3a77de4d10b3
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz' libmd_1.0.4.orig.tar.xz 264472 SHA512:731553ecc5e0e1eb228cced8fccd531fe31fb5c7627ca30013d287e1aeb8222959cf7498fbb7414bbabb967b25d4e8b0edd54fc47f6ccf55fc91087db0725ce3
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz.asc' libmd_1.0.4.orig.tar.xz.asc 833 SHA512:ec4b60a721da1f315fad73daa8ee620f44a53f17a30506c4d63b154b3abde19bb248b2ce6b83b989589e2a9184ebbe1b870e83181e18a4147d75617579d10504
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4-2.debian.tar.xz' libmd_1.0.4-2.debian.tar.xz 10204 SHA512:b1fb9128c407f1ae6f154508f8c45e28aa1d8886740dcb7a5c4fda0135cc6e534b93f864dd5746c7be3a03bd7109eac0faf7c388937da8d15c0fad76604e441c
```

### `dpkg` source package: `libpsl=0.21.2-1`

Binary Packages:

- `libpsl5:amd64=0.21.2-1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`
- `gnulib`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.2-1.dsc' libpsl_0.21.2-1.dsc 1622 SHA512:2bb260d1a03628b819a4b6be2e0c7c0ee51b599a5fd3535c0bb0622831f59d4a491be064708767bf8c395cec598ddc8b01a41c58fab1fd33354c13906224f707
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.2.orig.tar.xz' libpsl_0.21.2.orig.tar.xz 1870352 SHA512:5308feee863b84705246ce303c093e0c9fecd948ab382fd7480e9ea1ca5f72de42fc2c8f70472a97603580a3fd1eb2b552b093d79756e9fe93effba9f25b6aa4
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.2-1.debian.tar.xz' libpsl_0.21.2-1.debian.tar.xz 11940 SHA512:114ab8452d153bcad4e5702d6ef4172e8f5c43d69d3126bc06678135a54ae20bbe3e6c1e83cd2fc9cd8ae3b0add929a04b13cc6841c213687be259a07b558ed5
```

### `dpkg` source package: `libseccomp=2.5.4-1ubuntu2`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.4-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4-1ubuntu2.dsc' libseccomp_2.5.4-1ubuntu2.dsc 2799 SHA512:4fca61fc6e892446a4926f920a9f428aa34536346ccb4f2a7866b321893eeff5b8c009937e6270675329e1fde515630346ff4fa60ed8a10d2a1f0d3bf918636f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz' libseccomp_2.5.4.orig.tar.gz 637228 SHA512:92650bd7d1d48b383f402a536b97a017fd0f6ad1234daf4b938d01c92e8d134a01d2f2dd45fd9e2d025d7556bd1386ec360402145a87f20580c85949d62cea0e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz.asc' libseccomp_2.5.4.orig.tar.gz.asc 833 SHA512:10ce632da2762e3b5acb468194b2424d80bab786cc5923a8ee0b0684290282ef2f0a17192680afb36626c82e73a3ba64e73f248ed63cd3e55c3cf8cee4e1e447
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4-1ubuntu2.debian.tar.xz' libseccomp_2.5.4-1ubuntu2.debian.tar.xz 23632 SHA512:81a06032af40f3638dc603941f586bab9c66d866f6632478c49f7e82ac07702db76981439bceea81f1129a9ba324db05e30845ba74ebe1fcb08de179aa702b22
```

### `dpkg` source package: `libselinux=3.4-1build3`

Binary Packages:

- `libselinux1:amd64=3.4-1build3`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.4-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4-1build3.dsc' libselinux_3.4-1build3.dsc 2908 SHA512:c5d3bda0e675bc167c785dfabc4b9d676c84fa643e8874eccf635249df60fcc293bc859343b20c387c1a70123099d75904a1781a5aa5a648cf11407328b9061b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz' libselinux_3.4.orig.tar.gz 210061 SHA512:7ffa6d2159d2333d836bde3f75dfc78a278283b66ae1e441c178371adb6f463aa6f2d62439079e2068d1135c39dd2b367b001d917c0bdc6871a73630919ef81e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz.asc' libselinux_3.4.orig.tar.gz.asc 833 SHA512:de1e0431cbf8526c4de77e1ebe9fa40111ea4a0e71d6b0e9ec6c975b61f4090ec5df4386af362bbd5cc8faffb24c21febc13356fe081df642bbfa52010a00ba0
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4-1build3.debian.tar.xz' libselinux_3.4-1build3.debian.tar.xz 29572 SHA512:f32f0ce97c712e4a68966383d190cc519d0d1c11d98e45f8c33760dd67e7443bac3c9b9ed6f90156dfd27e24e9078767ca83ebee5db326c24cad763d8c68849d
```

### `dpkg` source package: `libsemanage=3.4-1build3`

Binary Packages:

- `libsemanage-common=3.4-1build3`
- `libsemanage2:amd64=3.4-1build3`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libsepol=3.4-2`

Binary Packages:

- `libsepol2:amd64=3.4-2`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4-2.dsc' libsepol_3.4-2.dsc 2005 SHA512:dfac0d64c2e2a2f68643a65091aeabc6175387e935a9fcf33834d29e52e0d5a6cb747462f656c82eb368915c71c7f6f38010eb3868ba9e2214de0f4eb3c867f8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz' libsepol_3.4.orig.tar.gz 490628 SHA512:5e47e6ac626f2bfc10a9f2f24c2e66c4d7f291ca778ebd81c7d565326e036e821d3eb92e5d7540517b1c715466232a7d7da895ab48811d037ad92d423ed934b6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz.asc' libsepol_3.4.orig.tar.gz.asc 833 SHA512:df3631f5f5b27e5893cfb14080089bd5a662d909257045c4b0cfe95e2abbb86d108f954248acd73121a65d9ab5fce771836e1aba4d3003c327ae9eecffefe791
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4-2.debian.tar.xz' libsepol_3.4-2.debian.tar.xz 21516 SHA512:571122e4656dce9a761db4f05777d51e7da95bb344fe74e62871bed744d4b30c7b80920106728b1039a47694f567181f6f3bba5e4782f97ce119e0975f7ed62f
```

### `dpkg` source package: `libssh=0.10.4-2`

Binary Packages:

- `libssh-4:amd64=0.10.4-2`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.10.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.4-2.dsc' libssh_0.10.4-2.dsc 2742 SHA512:33ec87fd8a2465a283b640bb05b4ba17a9ac0d8ab8c873de1b6f7f32e9efd07aedaf5af3a3be304bac3881ecb9a88621b90b27b594dcf33ad7f76b5f08745164
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.4.orig.tar.xz' libssh_0.10.4.orig.tar.xz 554920 SHA512:01ee52d480201d9886c15e81137c185334b404d1c8e8b743ddf58e95fe8619c8c013616a49807bd1111fde72fa177cd35f3c22b66cbf5d720b5abfacdf7601ed
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.4.orig.tar.xz.asc' libssh_0.10.4.orig.tar.xz.asc 833 SHA512:8200215d6471851dac8cd8efd07400b9bc4403cf5406a9fdb28a68ef8fe85c227f92a26071fb32d9396b91661568333b5ceb9b23665d22e761b981dd880bbbc8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.4-2.debian.tar.xz' libssh_0.10.4-2.debian.tar.xz 27800 SHA512:1f74b898e821200d621f700ecd71445bf4356f6ad61cd07c75089c308eba4849f91519543deb7087c17e19b4b0645a35ca9e43634a7ef0694df6960b4c64d199
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-2.dsc' libtasn1-6_4.19.0-2.dsc 2662 SHA512:86405d615a659eba8e60b01f293b442564b2438c00c81241c5683bd52165e10398d9d1016051abcfdef4e4fb7f7cebb703b82d950bf68e9906ae9893dfdb2624
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz' libtasn1-6_4.19.0.orig.tar.gz 1786576 SHA512:287f5eddfb5e21762d9f14d11997e56b953b980b2b03a97ed4cd6d37909bda1ed7d2cdff9da5d270a21d863ab7e54be6b85c05f1075ac5d8f0198997cf335ef4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz.asc' libtasn1-6_4.19.0.orig.tar.gz.asc 228 SHA512:e0417625f8df22c6421914bf2d4f19d7f27260c24c04f50e59669681f326debe06ddef9dc5a2e20fda50feb30bbbf3f41597e64961257304ec2c407aa76d107e
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-2.debian.tar.xz' libtasn1-6_4.19.0-2.debian.tar.xz 22012 SHA512:970b94efd8f52de08852d6c16b43c180ce498c2e929188f5b908bf6fb3cd6078dede768551d9329e33d6af201e6d3c2036128affa9c78ecc0045c13db886fa88
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.0-2.dsc' libunistring_1.0-2.dsc 2181 SHA512:40ad936d753f207f93223dab8e99b14d733e7b4f8234b7aa111789b4fb974116aa1339ede4accf3751ad44e379f1ecadf903e1c006b31e4a72bba65173f01c21
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz' libunistring_1.0.orig.tar.xz 2367800 SHA512:70d5ad82722844dbeacdfcb4d7593358e4a00a9222a98537add4b7f0bf4a2bb503dfb3cd627e52e2a5ca1d3da9e5daf38a6bd521197f92002e11e715fb1662d1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz.asc' libunistring_1.0.orig.tar.xz.asc 833 SHA512:7e32f69fac79fc418ea0aac5eca8c09fd5acbbe781d00504cd24145e2da45ba5696f20c00d16647cee8a65de2397f71bd86522e619566e7413faae4e5d739cac
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.0-2.debian.tar.xz' libunistring_1.0-2.debian.tar.xz 14520 SHA512:cae7a131985dd7d47248acd7fdd4d3332b804bb9d06c2e05c94507c4549a5c0d56a88c4657e09410cf98beedde104796b7a3e51d62290cc6465717cb0b20753d
```

### `dpkg` source package: `libxcrypt=1:4.4.33-2`

Binary Packages:

- `libcrypt1:amd64=1:4.4.33-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.33-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.33-2.dsc' libxcrypt_4.4.33-2.dsc 1591 SHA512:fc2bed4c87de4d8f6ce2b7b39cb208c59d40b4deea4c3e0ea913178ba72675a00b0034d30a64dbad443710c101663ebb4490f516c5bdc24148764db5ffae50ba
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.33.orig.tar.xz' libxcrypt_4.4.33.orig.tar.xz 393372 SHA512:67a0a2ce0301976513873a15acfb0d3c36c934bf62c5172a6268f48ce54cba40bbd05a1881a96cfe57c0f69c4816f0fff5a344afd99147b5f6b3fde16006d59e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.33-2.debian.tar.xz' libxcrypt_4.4.33-2.debian.tar.xz 8196 SHA512:f4718e5c8ab773cc18d7627a3cfacfdd783e3d1dbe3f41f4c2d4ce6776cdaf0e3e3125f668e30b1f6684abdae510949ac1f227fab34878ae1e7c39ec96202a5a
```

### `dpkg` source package: `libzstd=1.5.2+dfsg2-3`

Binary Packages:

- `libzstd1:amd64=1.5.2+dfsg2-3`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.2+dfsg2-3
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg2-3.dsc' libzstd_1.5.2+dfsg2-3.dsc 2454 SHA512:8782bcc326da99d585106640cea59fe66a702f895e8e6978e8df7ba93e028086ea12e9afe920c1b7f9c2de621fd3d6bbdc7b2cc90d069c04a7d7915a020c0f49
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg2.orig.tar.xz' libzstd_1.5.2+dfsg2.orig.tar.xz 1447608 SHA512:f41580b7fd64b5265f2e4dbe4161108091397f7f9b416e8f412b22de1c8687d41f094f58e77f5c4daa9c7842841c5729da1381173e8ad722a5531f6c01008fdf
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg2.orig.tar.xz.asc' libzstd_1.5.2+dfsg2.orig.tar.xz.asc 833 SHA512:ec83cbdd8d1f21f2c64b4a8ac51b47582eef2ab9a189a9c32fd496e31f5a73dac21f8ffe38dcfec3e67beeed3634bb5979c1a0009eeaac05aaa4e4168991ed5b
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg2-3.debian.tar.xz' libzstd_1.5.2+dfsg2-3.debian.tar.xz 12944 SHA512:cc874345995a2309735ebde048653bd880deaf9fa6cb18bf5838afdab6d00e7f2344ab07a9b4048902574879e730ff07a3abce5cfd66d8b1750d65bab129d46b
```

### `dpkg` source package: `lsb=11.5`

Binary Packages:

- `lsb-base=11.5`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.5.dsc' lsb_11.5.dsc 1614 SHA512:1335711764722a7e00911ad0ee62a2e01a8b7567632ea30815cc046209ca44d631fa586fbc7dc9c5ae5af90b6728f6f4e9048eec46f75a5f7d006a424b652120
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.5.tar.xz' lsb_11.5.tar.xz 38756 SHA512:87f7d1753de13a08cfc292ccc33dd94ffb0a0d7d9a634952a60da56c198791d76a5b6b2d4c59d7ae8bd5c35bfdb372a1d6e1466d80a9f12c24a876589d042d54
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.4-1.dsc' lz4_1.9.4-1.dsc 1951 SHA512:556aac9a8300772dc4016c09c5783ad38da73c2abe06a2074ed31ae2429972f81e49e883e11c1d9f25c63a8c8ea95cf7f738a1e9ebc2280a015615eb2c84ee10
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.4.orig.tar.gz' lz4_1.9.4.orig.tar.gz 354063 SHA512:043a9acb2417624019d73db140d83b80f1d7c43a6fd5be839193d68df8fd0b3f610d7ed4d628c2a9184f7cde9a0fd1ba9d075d8251298e3eb4b3a77f52736684
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.4-1.debian.tar.xz' lz4_1.9.4-1.debian.tar.xz 8128 SHA512:e89e2577dea9d76f6cac8c154c3fc6f77f501b5896ba949561e8a6a1e4982ad8de83d2deab8ca53dccab9856294dc2397d359cb0f4279b4f70b152c482043d88
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.dsc' mawk_1.3.4.20200120-3.1.dsc 1776 SHA512:1eb52b1393f45a35e63cbd065c2c125ae42cf4e58fc18b44350fc4311198d4d976b38a3d5ccba0e87ca5c5a69c2085970d3ebd9762543baaed3f994aee533fc2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA512:14d9a6642ce931bf6457d248fc2d6da4f0ea7541976ca282ea708b26df048f86fdf92c27f72d497501ccd43a244d1d1a606f1a2f266a7558306fea35dcc3041b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.debian.tar.xz' mawk_1.3.4.20200120-3.1.debian.tar.xz 14080 SHA512:e4c067f337c7d5302c275198d04f0211023626db4e72ab6f8e5642fe0936f97cb583f5c6d8911c424e9a79b438fb57b6320b8aa68cf384db2bf44a7e512a0388
```

### `dpkg` source package: `ncurses=6.4-2`

Binary Packages:

- `libncurses6:amd64=6.4-2`
- `libncursesw6:amd64=6.4-2`
- `libtinfo6:amd64=6.4-2`
- `ncurses-base=6.4-2`
- `ncurses-bin=6.4-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4-2.dsc' ncurses_6.4-2.dsc 4110 SHA512:a18f206ab2a7852483f2c0a7cc8859e30092fe83817ce059be16cdf7f1f75b2dcbf8b2e17a0fadd653c71c869e0496f957de86babe30d0307cc2f127e5728f56
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4.orig.tar.gz' ncurses_6.4.orig.tar.gz 3612591 SHA512:1c2efff87a82a57e57b0c60023c87bae93f6718114c8f9dc010d4c21119a2f7576d0225dab5f0a227c2cfc6fb6bdbd62728e407f35fce5bf351bb50cf9e0fd34
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4.orig.tar.gz.asc' ncurses_6.4.orig.tar.gz.asc 729 SHA512:8ee8b4b1ff3f804085a4f09aa8be1cf93d8633f7a6c7bcb079556c0a3fb2f4be8886c18c22dbc4f01fa03f88dc682ebce27459f9110909f72133f3685df2eb41
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4-2.debian.tar.xz' ncurses_6.4-2.debian.tar.xz 55492 SHA512:01a446828996dcd19a6a69b06d9bc9fbbc9110ea3487197897dc4f5bfc21cf2a5e9c1b16308b8689bce468804b43c85809687f86e140c3dbbfa8057dbb4523d1
```

### `dpkg` source package: `netbase=6.4`

Binary Packages:

- `netbase=6.4`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.4
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.4.dsc' netbase_6.4.dsc 898 SHA512:243ea79c8566581ff6137d0525195c0c9ceea2234cf74eb28aef5f6791ba35003e91bc063ce508c7be3038c05cf081db1d8f717d193f78554b7aa4a215d7c9ef
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.4.tar.xz' netbase_6.4.tar.xz 32712 SHA512:cbc588e5fbef5e3e2c8a2dc49214237e8340bf3fae66973237d1714f67c039d4b8d6886581d92b45a004fa23ff016ad8c82cb15b6f752d1ffa23e3284fe0b80a
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.8.1-2.dsc' nettle_3.8.1-2.dsc 2274 SHA512:441e46fd50c9626864ea1cb848230ea032cd06a5242ff496e9e5cd22ab44ad28016412d12ccd113baf114672e026334ef11a472116ef41bb9509917df091f080
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.8.1.orig.tar.gz' nettle_3.8.1.orig.tar.gz 2406251 SHA512:a405da3438d185d96917b03b00abb9ab43e04f58f770f657f716c25d64bb258ee170a71328e74736caa7121f50c0c89d3cc840c1201d2a92cfaf1357d24bdc6a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.8.1.orig.tar.gz.asc' nettle_3.8.1.orig.tar.gz.asc 573 SHA512:5856cfe4f0e907734af2ad699f0c26ad46e1a80828fd587ac1122b6493ad8527f832c2042ad936e139128a79a2f2478f5888d3a6ad92185984472f788f5e865a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.8.1-2.debian.tar.xz' nettle_3.8.1-2.debian.tar.xz 23396 SHA512:54d32e6ccb8da1ea1ea66bbbeef4e3c6a878e8e067ffe29156c8727c256f2fa3134115d818961460c87f6ad226e6c70a4de7d67e54a14b965ff67abe0c604036
```

### `dpkg` source package: `nghttp2=1.51.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.51.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `all-permissive`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/nghttp2/1.51.0-1/


### `dpkg` source package: `npth=1.6-3build2`

Binary Packages:

- `libnpth0:amd64=1.6-3build2`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-3build2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-3build2.dsc' npth_1.6-3build2.dsc 2063 SHA512:19ea7bd0ffc2b0aff06c52298c9a25c2f30619239bea09b571feb4a3d162f461a4529136e351da42b16ab3eaef5add24234f644e822e859ccb32de5bfd658ec0
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA512:2ed1012e14a9d10665420b9a23628be7e206fd9348111ec751349b93557ee69f1176bcf7e6b195b35b1c44a5e0e81ee33b713f03d79a33d1ecd9037035afeda2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-3build2.debian.tar.xz' npth_1.6-3build2.debian.tar.xz 10904 SHA512:426ab3ab9e27b3701d67cde0a4c4040aa9ccac22a0266321824487fe80a118ccd6860b6fa0fb5ca3c46dfa3c20053889fbb51a2e74618065b3aff059a0216c4c
```

### `dpkg` source package: `openldap=2.6.3+dfsg-1~exp1ubuntu1`

Binary Packages:

- `libldap2:amd64=2.6.3+dfsg-1~exp1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libldap2/copyright`)

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
$ apt-get source -qq --print-uris openldap=2.6.3+dfsg-1~exp1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.3%2bdfsg-1%7eexp1ubuntu1.dsc' openldap_2.6.3+dfsg-1~exp1ubuntu1.dsc 3461 SHA512:bc00aa6ae1d7f8536dd5e30438d5f12d3ed382c1ea0c6f0a56f0ecdd6870cfe1a3b69f1b6d9aa1275d257986c527eef75a18594d05b6278a4f7d43d04ee3a704
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.3%2bdfsg.orig.tar.xz' openldap_2.6.3+dfsg.orig.tar.xz 3741144 SHA512:951b935aa6a3f9dd1c2b7a4a289b6244d605a2a3de248051c8078b8afd5bfaab5943d5c6adddf9e85eb6813db3ddff18478f2c85625df4095ec037bdc579bdc7
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.3%2bdfsg-1%7eexp1ubuntu1.debian.tar.xz' openldap_2.6.3+dfsg-1~exp1ubuntu1.debian.tar.xz 178740 SHA512:0aff107f8e324195f4c00b367a9c1f29c9bdf71812a59693007532ef457cf924215ee025b911ec9ab1d65c0cf0ccde7c288df507925a5dd54fbcbf6f774dc555
```

### `dpkg` source package: `openssl=3.0.7-1ubuntu1`

Binary Packages:

- `libssl3:amd64=3.0.7-1ubuntu1`
- `openssl=3.0.7-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.7-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.7-1ubuntu1.dsc' openssl_3.0.7-1ubuntu1.dsc 2544 SHA512:0e6b8f734de2f2920cabc0d11f3642bb00673089a60030dde81dcabd9515a3d647437b4c3fdefabb20c5bc3ad8d384f097a042a49be2dcb66df7db6523bb7f2b
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.7.orig.tar.gz' openssl_3.0.7.orig.tar.gz 15107575 SHA512:6c2bcd1cd4b499e074e006150dda906980df505679d8e9d988ae93aa61ee6f8c23c0fa369e2edc1e1a743d7bec133044af11d5ed57633b631ae479feb59e3424
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.7.orig.tar.gz.asc' openssl_3.0.7.orig.tar.gz.asc 858 SHA512:9093a8a5a990f5f37bd95e7ca55f2371e59242be408ea7d9403bcfc9c8873c022237e13c0ec81881a20607ea46927887a895a82b6f50c6f423b4c54f9ef0cde1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.7-1ubuntu1.debian.tar.xz' openssl_3.0.7-1ubuntu1.debian.tar.xz 106024 SHA512:8d74039c54f222796c5643ea43cc1caf869b592eb1c3c62190a6e7825dc857b38ef580f1a00a81b14d1e250b4303e9779817e3704eef5788fef7a75d5d642cd2
```

### `dpkg` source package: `p11-kit=0.24.1-2ubuntu1`

Binary Packages:

- `libp11-kit0:amd64=0.24.1-2ubuntu1`

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
$ apt-get source -qq --print-uris p11-kit=0.24.1-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1-2ubuntu1.dsc' p11-kit_0.24.1-2ubuntu1.dsc 2434 SHA512:7ab6cf1fa7900437807c28187bd84ff58626f3db75a3766ef549805485733ed18852f5eac931eb10e50eb1d39265985ce559946638ffc5f8b2fd7e818b021770
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz' p11-kit_0.24.1.orig.tar.xz 838304 SHA512:8cf170c714bb9e0cf3df93e8ec55b8e3c55cabf2c6a27f177ac6de8b8028985df2ca0216d3215d6828dc2ae3095c4e1a4febe8cb26b88ec321defc66bb011e81
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz.asc' p11-kit_0.24.1.orig.tar.xz.asc 833 SHA512:c9cb909a9443cc554c32d7816add59a1b1225186517a0bc8dc267a638a93de070a6ce57c0bafaf1a2b0a03acbdb0a3c1fdd88a615f402ade13e41d20463a7803
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1-2ubuntu1.debian.tar.xz' p11-kit_0.24.1-2ubuntu1.debian.tar.xz 31416 SHA512:d357e3a2cfade291436d796cb843fda3637c1e906db9c1acb8e2a0b518dc88aadbc17e9708baee01400a9659432dd557a4868b096b3de1b26e9c9837bb16a20c
```

### `dpkg` source package: `pam=1.5.2-5ubuntu1`

Binary Packages:

- `libpam-modules:amd64=1.5.2-5ubuntu1`
- `libpam-modules-bin=1.5.2-5ubuntu1`
- `libpam-runtime=1.5.2-5ubuntu1`
- `libpam0g:amd64=1.5.2-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.5.2-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2-5ubuntu1.dsc' pam_1.5.2-5ubuntu1.dsc 2664 SHA512:cf95c7594647f4ba30ab4b761b620a6ad2550fed36a127bf7ac4a922f0d5c9b403d3465d56e727ddef67ce4ee7fd5e1fb1508ab2f601920b50b06e5e705e23f2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA512:fa16350c132d3e5fb82b60d991768fb596582639841b8ece645c684705467305ccf1302a0147ec222ab78c01b2c9114c5496dc1ca565d2b56bf315f29a815144
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2-5ubuntu1.debian.tar.xz' pam_1.5.2-5ubuntu1.debian.tar.xz 166668 SHA512:d1cde467271414b1eee7bc030838cd508482de7643a37729989cdb1b551353b2fa912c8536ddb51790e1f5de4bfa359a5af004b533128024f621ede07939628d
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.42-1.dsc' pcre2_10.42-1.dsc 2302 SHA512:885d8d2a345d3c4a1ac95f0b5aed856392d35a4823ea3404536f17f8a7077bbaee943554d9ce40ba565b5262e577ed0649cd4f0b8add8873bed7211cc36b0454
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.42.orig.tar.gz' pcre2_10.42.orig.tar.gz 2397194 SHA512:a3db6c5c620775838819be616652e73ce00f5ef5c1f49f559ff3efb51a119d02f01254c5901c1f7d0c47c0ddfcf4313e38d6ca32c35381b8f87f36896d10e6f7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.42-1.diff.gz' pcre2_10.42-1.diff.gz 7895 SHA512:381b28be73dbaceba13d6bc3498ae10155d6c614add038a306481ad86a9033586e3873822cdfadd037b155bb9ae9c2fa6bcfd66001dad653fb09b238caa11eb2
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-7.dsc' perl_5.36.0-7.dsc 2886 SHA512:2a84ec712340a3f125aa3853ae3c0a0933138de1fe226b520b7c9ea7ed2b70a7e10fe94a265699a212b3f943cf61302cf05c756d92eb7671d6cc21e490ea2b78
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig-regen-configure.tar.xz' perl_5.36.0.orig-regen-configure.tar.xz 417784 SHA512:4d16685f569a5b1dea79d607b6d62718111c32efaf5547bb9e1528bd755acf0c8fc74a1cc1f4d68fcb10aef9da7d8fea17a5cc10dabce6efa4721ab45ab03a65
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig.tar.xz' perl_5.36.0.orig.tar.xz 13051500 SHA512:6dd6ac2a77566c173c5ab9c238cf555f2c3e592e89abb5600bc23ce1cbd0c349e0233f6417cbbf1f6d0aefc6a734ba491285af0d3dc68a605b658b65c89f1dab
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-7.debian.tar.xz' perl_5.36.0-7.debian.tar.xz 169288 SHA512:366489ee981c62a22f19883f67dfe2f0b972a0a0e276c4a40a02df31661171260ad9fdaa180089f0f51ade46b8bf6c02c560691c58426baea5885ec550c435c5
```

### `dpkg` source package: `pinentry=1.2.1-1ubuntu1`

Binary Packages:

- `pinentry-curses=1.2.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.2.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.1-1ubuntu1.dsc' pinentry_1.2.1-1ubuntu1.dsc 2999 SHA512:2e895300429edd2b707fded47ee07d66bf7d439417deae2a78720cf833152bf71f9357cc93632358c1d59963f1513ccaaa2c3904c4de51991d65b60cb19bcf2f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.1.orig.tar.bz2' pinentry_1.2.1.orig.tar.bz2 547698 SHA512:a665315628f4dcf07e16a22db3f3be15d7e7e93b3deec0546c7275b71b0e3bd65535a08af5e12d6339fd6595132df86529401d9d12bd17c428a3466e8dfafab6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.1.orig.tar.bz2.asc' pinentry_1.2.1.orig.tar.bz2.asc 390 SHA512:60b63b7fe2d6793840be55635f9a704cd42eda69ccaea2453d47b5f7a5198d313b8f23555972584f7f087fd5d0fc2a379bfc5f7512f325b018cc5c3e2e54a47e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.1-1ubuntu1.debian.tar.xz' pinentry_1.2.1-1ubuntu1.debian.tar.xz 18828 SHA512:94a82f96b7cf520c8335fea8a7be1beb8baf9e68e5939e3436837eca87ed0346bd295e406f6d546c74f0592332c6913e6c6b709c7dbe014bda769d556ce71238
```

### `dpkg` source package: `procps=2:3.3.17-7ubuntu1`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-7ubuntu1`
- `procps=2:3.3.17-7ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-7ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-7ubuntu1.dsc' procps_3.3.17-7ubuntu1.dsc 2237 SHA512:756be0329040247eadaf884e61164172eb618dee97bed81242b100a53dd219d8b471067c9a7109ac96214256ed1f5f7832883cfd632e1d209bbb730bf6f4ea0a
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA512:59e9a5013430fd9da508c4655d58375dc32e025bb502bb28fb9a92a48e4f2838b3355e92b4648f7384b2050064d17079bf4595d889822ebb5030006bc154a1a7
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-7ubuntu1.debian.tar.xz' procps_3.3.17-7ubuntu1.debian.tar.xz 34528 SHA512:77435e34138738e58394c7eab10716d5ad59b4eb92c045114dd0ef374b3e987ceada7e65272e4ead85e6adeaa9980dc81ee5dd6c937a6be1c241c339d35475c1
```

### `dpkg` source package: `readline=8.2-1.3`

Binary Packages:

- `libreadline8:amd64=8.2-1.3`
- `readline-common=8.2-1.3`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ISC-no-attribution`

Source:

```console
$ apt-get source -qq --print-uris readline=8.2-1.3
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.2-1.3.dsc' readline_8.2-1.3.dsc 2553 SHA512:ae771c7d5d13e41c6b033ca1862ad2b7d78c1ea365f592a3703d1659b47c9b3ec068c5261dab470cec73b2d065d1f75e04fbd79d6800e65c114ac4267244a919
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.2.orig.tar.gz' readline_8.2.orig.tar.gz 3043952 SHA512:0a451d459146bfdeecc9cdd94bda6a6416d3e93abd80885a40b334312f16eb890f8618a27ca26868cebbddf1224983e631b1cbc002c1a4d1cd0d65fba9fea49a
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.2-1.3.debian.tar.xz' readline_8.2-1.3.debian.tar.xz 30016 SHA512:17d127126bcabeac5215266752c21a9f154f5c252319fa23885c4e5cd2d43372f830f9bc730a21d45e5ce6c4b1a3f3f649144febf2203f5c617b2e507b807a2b
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2build4`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2build4`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2build4
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2build4.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build4.dsc 2431 SHA512:7536b21c9c8be02e06171db49bf0b653e4b7738e6c01f74b0b7433c2986c731eafd1743f87836e7250a744d0e34dc700685bbe7128956a274e9a9832d32c891e
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA512:bdfcbab73179d614a295a7b136ea4c9d0ce4620883b493f298362784d245608cd6ad4b0ad30f94ed73a086b4555399521ae9e95b6375fce75e455ae68c055e7b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2build4.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build4.debian.tar.xz 8376 SHA512:b01ac33a7251e3c0fad21897d31710766136027b656cb29903cf8f695893648631037a96fa18aa40eae7ad363394344aad4f2fae152622618b88f22133c03578
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.9-1.dsc' sed_4.9-1.dsc 2077 SHA512:5c7b4495f8e2e7f93f81d8bd01fc49905b35226d537c87c1ab87b8374a9afd446d7c3ffcc97d007d1b304cc5928b421c1bea3823b77aaa37dda05d08101bd645
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.9.orig.tar.xz' sed_4.9.orig.tar.xz 1397092 SHA512:36157a4b4a2430cf421b7bd07f1675d680d9f1616be96cf6ad6ee74a9ec0fe695f8d0b1e1f0b008bbb33cc7fcde5e1c456359bbbc63f8aebdd4fedc3982cf6dc
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.9.orig.tar.xz.asc' sed_4.9.orig.tar.xz.asc 833 SHA512:ceb235850184b99017783486e182ade9db38313d20b2b34d23f54d8affe180f7a191139b993e8ec7718ca33eff732f547ca4b3b59aaf865feaae611dfeae5c46
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.9-1.debian.tar.xz' sed_4.9-1.debian.tar.xz 62616 SHA512:5f10389226e093abdf014187dd1e097522938051594158265b0f294cea36b45043081f89a40ec8a91f7fb9a9b907699ca02752cbeac2a5b156f0f702e97881c8
```

### `dpkg` source package: `sensible-utils=0.0.17+nmu1`

Binary Packages:

- `sensible-utils=0.0.17+nmu1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.17+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.17%2bnmu1.dsc' sensible-utils_0.0.17+nmu1.dsc 1728 SHA512:d9c48bb639287be8fe7ae97e824189dcdadc1517b41e9f3dcffa122030f094a0b1ec765adeac20057b186d47e8817d92ce7dedaebb2a44e2fb71d5df7adb9788
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.17%2bnmu1.tar.xz' sensible-utils_0.0.17+nmu1.tar.xz 66476 SHA512:3c4e7dc2fec360d8a3a7ff1574fc826f7f04e5ef3d186a13155ba7fecba09d599a82cda037fc406c758d773746e04fadd427dc1b3cc5efe3598fffc2c923b287
```

### `dpkg` source package: `shadow=1:4.13+dfsg1-1ubuntu1`

Binary Packages:

- `login=1:4.13+dfsg1-1ubuntu1`
- `passwd=1:4.13+dfsg1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.13+dfsg1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.13%2bdfsg1-1ubuntu1.dsc' shadow_4.13+dfsg1-1ubuntu1.dsc 2509 SHA512:77dda236b8198dfd3516b2b74d782b859aacc007f097f8f9c5ead574fd23984baa10b36cf1c32d8e0187dee05a970ec8a20b0d8f447d1c0e437c6006520ad8e9
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.13%2bdfsg1.orig.tar.xz' shadow_4.13+dfsg1.orig.tar.xz 1811752 SHA512:27106ca26d6e4c9e5833cf79811b10f656ade547bbc18b87faf79bbe0581a9e1467cbb6c354320e2d5233d17208d77742ebf197d32b6d2f08439e37e368ded1d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.13%2bdfsg1-1ubuntu1.debian.tar.xz' shadow_4.13+dfsg1-1ubuntu1.debian.tar.xz 91380 SHA512:9c8909ca0d9552d1094598fee5b96dcdf9f3b5a8265920466cadde63151996ade671760b40ccb99fcca43c90a28d35b66ad0d2dbf03782bf5daf7815fd406664
```

### `dpkg` source package: `sqlite3=3.40.1-1`

Binary Packages:

- `libsqlite3-0:amd64=3.40.1-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.40.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.40.1-1.dsc' sqlite3_3.40.1-1.dsc 2487 SHA512:72864c682b6661d1bb21795a21ec075528a7862bfc69ad9fd4b65c5def7e4f53f59c2b1880f203eb2b06b11ab8b5d92fe4053c281b3ba4059693ba8b7358b6a4
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.40.1.orig-www.tar.xz' sqlite3_3.40.1.orig-www.tar.xz 5865720 SHA512:2815637c8aa553351303e44c8348d510dc9a5f7c4fca973e000b491e8607525f8a6d5a842c0cb708d510bcb2a3e491b2384d6b13693a1e4b63fab54029017093
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.40.1.orig.tar.xz' sqlite3_3.40.1.orig.tar.xz 8019048 SHA512:83f88923aa2922d9067c7f322bc020a8aed9b1002e236281dc2be5cc895bb2cffaae2f2d37585369ccfaa0107640541552c14d36f8923e762366a97b4ce67df6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.40.1-1.debian.tar.xz' sqlite3_3.40.1-1.debian.tar.xz 29804 SHA512:3dc61ed9d1c68d62a9f8dcfbef984f322be6a5f7679a9bab469c0b5a7be91d8235a01df5945e12a6e1e80626b35e897f4d4fcafe684f0e17d984ef1a220b4ec6
```

### `dpkg` source package: `systemd=252.4-1ubuntu1`

Binary Packages:

- `libsystemd0:amd64=252.4-1ubuntu1`
- `libudev1:amd64=252.4-1ubuntu1`

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
$ apt-get source -qq --print-uris systemd=252.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_252.4-1ubuntu1.dsc' systemd_252.4-1ubuntu1.dsc 6601 SHA512:73583721109976bc851456ecbe461d7a501e089a97c407cf4077388c52245deb2ff0fe74b641fadb5719c56c8b7c1cfe10f13148500409416112c91a95c6bc4a
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_252.4.orig.tar.gz' systemd_252.4.orig.tar.gz 11753300 SHA512:d4e99a67c59091dae78f654433a6c5e114ae66256b72d9d43292c43a986ee6a58e2d06f12866cbd7ec821b61580ec003af1725f60fd4b038b4a981b3ca839ee2
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_252.4-1ubuntu1.debian.tar.xz' systemd_252.4-1ubuntu1.debian.tar.xz 227284 SHA512:fb9cbea6acee6f4e0ce29612cae6866b6089c0b034b0c3ea14244bf2d6329a9276acd37183abf383b8b3b01ca3f1482b84a15d00339a355db824fde1cc526a00
```

### `dpkg` source package: `sysvinit=3.05-7ubuntu2`

Binary Packages:

- `sysvinit-utils=3.05-7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.05-7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.05-7ubuntu2.dsc' sysvinit_3.05-7ubuntu2.dsc 2466 SHA512:417a2e7412d0f35c290fde8a163eb91dcabafb3ec1c34e094053bb05453271288f4b82fa92c707b8c75a6b0b9b7b952571ff55b3e1d85e7e5a22fbd0fe4d9e62
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.05.orig.tar.gz' sysvinit_3.05.orig.tar.gz 435554 SHA512:7939a959e60108ac0ebe9504c3cf472a7c24711063da0d01d9dbdbe8e4db018d9b4d7313a4552ac5032af61db71f18f30608e362ca8563003bfe2d9edb66cfba
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.05-7ubuntu2.debian.tar.xz' sysvinit_3.05-7ubuntu2.debian.tar.xz 135292 SHA512:9456dd0fb150403c94e0b5f25c2664b5a705aa813fdbc1efa564e24a5f9d958009faf4e17140cff81e240a7b9e164883ac359684222ff05d19e34af363fc6b78
```

### `dpkg` source package: `tar=1.34+dfsg-1.1`

Binary Packages:

- `tar=1.34+dfsg-1.1`

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
$ apt-get source -qq --print-uris tar=1.34+dfsg-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1.1.dsc' tar_1.34+dfsg-1.1.dsc 1998 SHA512:ce74c0853397e8d1b047612d5208299ce7e2a635285686245d93f43d3bf2ed980df3c000769ff3c00b946e321273efe57d9a1e8f8ca012e23b1a256a837a1c8d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA512:ec5553c53c4a5f523f872a8095f699c17bf41400fbe2f0f8b45291ccbaf9ac51dea8445c81bd95697f8853c95dcad3250071d23dbbcab857a428ee92e647bde9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1.1.debian.tar.xz' tar_1.34+dfsg-1.1.debian.tar.xz 20148 SHA512:9b473bd6e3d84fc066e28006dcc33a9542f96ea2469f87987e60a8d1c7d7d190478c597fb76630f799d925b570645469bfda71067e2918d1108ece804b88fb41
```

### `dpkg` source package: `tzdata=2022g-2ubuntu1`

Binary Packages:

- `tzdata=2022g-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2022g-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022g-2ubuntu1.dsc' tzdata_2022g-2ubuntu1.dsc 2414 SHA512:a0e0af4ea7c8a54ad76b0cbadc4b5624131208fa3e41fb6276dee3513c8fffa7f082dda0ed2d1fe42f809bf89f6242dcd6aee6e9c871d1545fe90db07f5a7fd2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022g.orig.tar.gz' tzdata_2022g.orig.tar.gz 439731 SHA512:7f79394295e00e3a24ebdbf9af3bc454a65f432a93b517e7e96c7f9db9949f6f5fdae9892a9d3789ff44ae0eb1bfe4744d36976b4624659af951d26414f94e65
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022g.orig.tar.gz.asc' tzdata_2022g.orig.tar.gz.asc 833 SHA512:3474a05373ec4397e17133c54708e1f9efd1f1c5e7ee6945f0972809ceda2214cc4962238773818d04ab4f29dcdf0b3e87247ab19795d06a62b8769dd85cf76b
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022g-2ubuntu1.debian.tar.xz' tzdata_2022g-2ubuntu1.debian.tar.xz 172944 SHA512:c62d34dc4af68ace8af465035743a539f4076e251baa4d22fcdacde9bb2a553848dfec02301844e020bf354cfc286d45b7c2e4cdc2cea37b44294b4a17b67051
```

### `dpkg` source package: `ubuntu-keyring=2021.03.26`

Binary Packages:

- `ubuntu-keyring=2021.03.26`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2021.03.26
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2021.03.26.dsc' ubuntu-keyring_2021.03.26.dsc 1855 SHA512:7502f4f4d9a288fab9fb84b6ae5f8500cb3f14c68ed586b489dee95f12087b232bcecd9369e98258bb710afda50e5672dfbc6422b1436e896fb529dec8832252
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2021.03.26.tar.gz' ubuntu-keyring_2021.03.26.tar.gz 34529 SHA512:04a76e2bfa88fb428face9e01976ff98a3a26fe2b555340c14200fc6099ee3b474a6733486cedfe933933c0a6826ee3550660499d7b26bda8a27a620b1d6a35f
```

### `dpkg` source package: `usrmerge=33ubuntu1`

Binary Packages:

- `usrmerge=33ubuntu1`

Licenses: (parsed from: `/usr/share/doc/usrmerge/copyright`)

- `GPL v2`
- `GPL-2`
- `later (please see /usr/share/common-licenses/GPL-2)`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=33ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_33ubuntu1.dsc' usrmerge_33ubuntu1.dsc 1717 SHA512:7eec869b81491eaaff56afb185402b5a5f5c91eab3c88fff4ca28dcbe33f4878bd638c9118f470cf7e57bbef4612637e84018268ec6227eeb3999c097e50c1bc
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_33ubuntu1.tar.xz' usrmerge_33ubuntu1.tar.xz 14900 SHA512:89d750915d80888614eb536e57edffcf38ac599c3c435ece144e2ae7048d52c32d7f9082b7acb826c0189946f90151a3009460f5faac97a5383051d74db419a5
```

### `dpkg` source package: `util-linux=2.38.1-4ubuntu1`

Binary Packages:

- `bsdutils=1:2.38.1-4ubuntu1`
- `libblkid1:amd64=2.38.1-4ubuntu1`
- `libmount1:amd64=2.38.1-4ubuntu1`
- `libsmartcols1:amd64=2.38.1-4ubuntu1`
- `libuuid1:amd64=2.38.1-4ubuntu1`
- `mount=2.38.1-4ubuntu1`
- `util-linux=2.38.1-4ubuntu1`
- `util-linux-extra=2.38.1-4ubuntu1`

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
$ apt-get source -qq --print-uris util-linux=2.38.1-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38.1-4ubuntu1.dsc' util-linux_2.38.1-4ubuntu1.dsc 4632 SHA512:30666c73e0f03eba2dbb3f7d6a2cecda628743ca5066df079ec1ba08480c1462789b1c8f3d577a66dd0f15d2e9648c295bfc2fd99602a82da26d1d7d8f5b6eeb
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38.1.orig.tar.xz' util-linux_2.38.1.orig.tar.xz 7495904 SHA512:07f11147f67dfc6c8bc766dfc83266054e6ede776feada0566b447d13276b6882ee85c6fe53e8d94a17c03332106fc0549deca3cf5f2e92dda554e9bc0551957
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38.1-4ubuntu1.debian.tar.xz' util-linux_2.38.1-4ubuntu1.debian.tar.xz 117468 SHA512:32819d2d07bf2b84ebe3a3e5b32cb36b6b48e742f775ce909c192c4efb0b4208b2bc2559343cc4e0414d667e0268f0838e5010abbdb9c178d98fa284745c56d7
```

### `dpkg` source package: `wget=1.21.3-1ubuntu1`

Binary Packages:

- `wget=1.21.3-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.3-1ubuntu1.dsc' wget_1.21.3-1ubuntu1.dsc 2243 SHA512:a93ad7308ba283204d2b28edefd6a65851f1c576274f356504538a49bb414c25020a92ac30ceda00546ec6d2b45508e09bd1aadf3a34925eb2b93bf9610c1ce3
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.3.orig.tar.gz' wget_1.21.3.orig.tar.gz 5079864 SHA512:29889ecbf590dff0f39183d9e0621741d731a554d990e5c995a4644725dca62e8e19601d40db0ef7d62ebf54e5457c7409965e4832b6e60e4ccbc9c8caa30718
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.3.orig.tar.gz.asc' wget_1.21.3.orig.tar.gz.asc 854 SHA512:b9f41496e0083545bc703c97b0758500f337527647cdc422152d7855d05351e3a62685269238c78300eafdbfaed8afecaeb988901a3d8a6b002e9fb3d70efe4f
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.3-1ubuntu1.debian.tar.xz' wget_1.21.3-1ubuntu1.debian.tar.xz 63772 SHA512:da66b025bc1ad2114daa4c47992e575f78d62fc18b1ef95b0669fcb0260e520a8b46e3916538b3ec873351574cf9b136669c1dd026ae04f4d3d60021121eff3c
```

### `dpkg` source package: `xxhash=0.8.1-1`

Binary Packages:

- `libxxhash0:amd64=0.8.1-1`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.1-1.dsc' xxhash_0.8.1-1.dsc 1966 SHA512:645799311fdf21568b23134cdf586a54bb32b58639adb8ebc1f5ad26fdfdc485506c87d763133163fde705b2f904d6f01f50e4d13ebec2b476d38e66ded2bf22
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.1.orig.tar.gz' xxhash_0.8.1.orig.tar.gz 171552 SHA512:12feedd6a1859ef55e27218dbd6dcceccbb5a4da34cd80240d2f7d44cd246c7afdeb59830c2d5b90189bb5159293532208bf5bb622250102e12d6e1bad14a193
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.1-1.debian.tar.xz' xxhash_0.8.1-1.debian.tar.xz 4572 SHA512:e59d4fc6f736d3af6f7be3ec64fc1ee4382e917a942e4000159652082e2f73f52ae0f72adb98505ac9bd8894a89800e21c0913ba4b511959f07a2bc84c341920
```

### `dpkg` source package: `xz-utils=5.4.1-0.0`

Binary Packages:

- `liblzma5:amd64=5.4.1-0.0`

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
$ apt-get source -qq --print-uris xz-utils=5.4.1-0.0
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1-0.0.dsc' xz-utils_5.4.1-0.0.dsc 2517 SHA512:829e0b0b2bdecca23163d3e2927f17e37b420244ce2863a279add6d2fbef57089bb8c692ebf9237dd627d281ac47f12e8c81538141d26e710fc4919596af0457
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz' xz-utils_5.4.1.orig.tar.xz 1485272 SHA512:f890ee5207799fbc7bb9ae031f444d39d82275b0e1b8cc7f01fdb9270050e38849bd1269db2a2f12fe87b5e23e03f9e809a5c3456d066c0a56e6f98d728553ea
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz.asc' xz-utils_5.4.1.orig.tar.xz.asc 833 SHA512:0802a4ae8f8fe700288b0fb1a4c9f59f71b26fcaea88cd368d36dcfd96a1deb2380a7b9af66b84d2f4faf68ff114d9b4b4e48b5b8362c37a8e528f13a4233cf3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1-0.0.debian.tar.xz' xz-utils_5.4.1-0.0.debian.tar.xz 24076 SHA512:21fd054fcc0e1bce8835d4e19618038a6d795f6cdf5a82aa9b6f3a26852e459eac806d1ca6c4430b726cf4bc22a99921da38b02db166b0e90e17f390e41d00d0
```

### `dpkg` source package: `zlib=1:1.2.13.dfsg-1ubuntu4`

Binary Packages:

- `zlib1g:amd64=1:1.2.13.dfsg-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.13.dfsg-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu4.dsc' zlib_1.2.13.dfsg-1ubuntu4.dsc 2972 SHA512:0ef70f7a1ee27e9d414001d67497f14014e188b90a4615fb2a955c96f7997bc36d6a5931c63e733d5ebefa87bbfdcdd6810a1278c210a39a7c1fc43df6ca4edc
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg.orig.tar.bz2' zlib_1.2.13.dfsg.orig.tar.bz2 1239825 SHA512:266ea72465ad1f0b63e42f8275c650615829929f2ff19064144c5bb942acd31cd8581ce45781c438fce949c6d9f3fa385efa59f754761441107ca1144fb56802
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu4.debian.tar.xz' zlib_1.2.13.dfsg-1ubuntu4.debian.tar.xz 57960 SHA512:312357388a757db8f3588f637a3d016f28fbff89fed2bb882a4972f5f838e39129fcb01d77cbd0ba9ec3e65fbc993e9f0c4e11acb298894dc6350fb9b1e2d7ca
```
