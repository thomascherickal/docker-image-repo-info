# `buildpack-deps:mantic-curl`

## Docker Metadata

- Image ID: `sha256:392c449b2867d49805ee4b096b0a3444aafcb711d7e3543e906c551acfb15076`
- Created: `2023-12-02T04:21:00.853081957Z`
- Virtual Size: ~ 95.25 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
- Labels:
  - `org.opencontainers.image.ref.name=ubuntu`
  - `org.opencontainers.image.version=23.10`

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

### `dpkg` source package: `adduser=3.137ubuntu1`

Binary Packages:

- `adduser=3.137ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.137ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.137ubuntu1.dsc' adduser_3.137ubuntu1.dsc 1862 SHA512:4e32edd8d12689bc8f6fb2b5280b0504bbd19bdd963cebb32a016d87fbeb837cbfb9c4c544b37943adf346d33137c684936591ccbf5c89856a91f2777f00ae49
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.137ubuntu1.tar.xz' adduser_3.137ubuntu1.tar.xz 280408 SHA512:46979160ef2f6b85097958cd11e549ae48efa24e1719155fd90ae7b322c0adac087cac7d0a709cd084ee11557575b05dfde89a9d63bcfd80fb47779c41098d48
```

### `dpkg` source package: `apt=2.7.3`

Binary Packages:

- `apt=2.7.3`
- `libapt-pkg6.0:amd64=2.7.3`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.7.3
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.7.3.dsc' apt_2.7.3.dsc 2945 SHA512:35608187cc9605110148634b01a56a1d06ad259c2a8dc127a630803e2943a70827379be97b28092b7fdf5a2b59103e450efcabdef82da571f434f4b286c2735e
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.7.3.tar.xz' apt_2.7.3.tar.xz 2343000 SHA512:0941bdffa2344edadf5cc6b299188acc05a10bb3ff1f4d10c7ac5c96daafce6a9fc2dc7d40a38617f950e623dec25ed68c7bf51e346cdf5fdf600ef00de5416e
```

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

### `dpkg` source package: `audit=1:3.1.1-1`

Binary Packages:

- `libaudit-common=1:3.1.1-1`
- `libaudit1:amd64=1:3.1.1-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.1.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.1.1-1.dsc' audit_3.1.1-1.dsc 2402 SHA512:860c8ba15c80cc17541ff6245fe1abc63681962476550aff63712f849ebab7ac5e50e2f4c21b4b472716ce15e6bcec656117e0acef2e2b8adc02abda17bf3863
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.1.1.orig.tar.gz' audit_3.1.1.orig.tar.gz 1218111 SHA512:4917970cc4c7f786c464a6d101bf66d55d55ac4716cf415ff97177f08176a6301e946716d28cf5b16054538469b3140b97db99d55a28686a9a807eea60c070f3
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.1.1-1.debian.tar.xz' audit_3.1.1-1.debian.tar.xz 18944 SHA512:ab98846a36aef4a1954b63973b57fa86e69e6012c7813068a0a7f224f30e4850c734e5ce568ed7485861fe4a362587512de4c00614326638d07bd6e3e7363af6
```

### `dpkg` source package: `base-files=13ubuntu2`

Binary Packages:

- `base-files=13ubuntu2`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=13ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_13ubuntu2.dsc' base-files_13ubuntu2.dsc 1650 SHA512:3763d569f2cf77de66e2368626f6e2cfc5ca9aa1647da4a066d8d3cf3de5373d15a67f6f24982a2c4134f72fbfa22986097818cba3d594029dba7ec0955768ad
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_13ubuntu2.tar.xz' base-files_13ubuntu2.tar.xz 93264 SHA512:4a8b7fba2181938411e6b243ae452a13939ee93720987e5532d258481997a23a4096f3dc79d54da148479b212c8363629240dc2f52eb8b31359229e062f932fe
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

### `dpkg` source package: `brotli=1.0.9-2build8`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2build8`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2build8
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build8.dsc' brotli_1.0.9-2build8.dsc 2285 SHA512:dd4dbaec5136b6ec2c96bfb495fd7bb6271cbcd74458792cddd73ad45332fe3dd8e4b7d10c4ea6b5e0c10668dc8cf322e910c8807e2297ed2c589ecc3902c014
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build8.debian.tar.xz' brotli_1.0.9-2build8.debian.tar.xz 5884 SHA512:e09a1e108cbd266194f3c3760f12ee2a0608049882e9773356a457b4ca74029f8849c498fc8fdda3d101de6e1868b0776467c71ef22f2e9e245b4cb4871203cc
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

### `dpkg` source package: `ca-certificates=20230311ubuntu1`

Binary Packages:

- `ca-certificates=20230311ubuntu1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20230311ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20230311ubuntu1.dsc' ca-certificates_20230311ubuntu1.dsc 1846 SHA512:dd9af00eafa728a2d32ac7cc30e781f7983dbf3b56e85a1daa53ba958f364af60ae7dbc3c50ebd435398b127472ac19bf2658f6829ef8c8cc44c02c75f5858e7
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20230311ubuntu1.tar.xz' ca-certificates_20230311ubuntu1.tar.xz 258172 SHA512:15b59854164fccf1a057f4f97cb4b07a09c1bdcbfb8a36e9436ce50c50b447100e604edc35bfbf8a7ce64755fc40897c50f70503b3ba3cfcd0c6e1f3f4e6ba20
```

### `dpkg` source package: `cdebconf=0.270ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.270ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libdebconfclient0/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.270ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.270ubuntu1.dsc' cdebconf_0.270ubuntu1.dsc 2873 SHA512:03876bf61814c0d99bcdb548b27a33ea04b82d6d1431266b7afab72238a2e1410c5dccfa9409f360008f3808a1f930f1d870655c0c7b1bf2c689fc764739cefc
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.270ubuntu1.tar.xz' cdebconf_0.270ubuntu1.tar.xz 285780 SHA512:37ac3c7a352dea023b10dad8202f31e037e8bf8d1fc5050a757107ea4ba5561ae0f74c6254778bf4dc3226f343e2c1873e41412708b845fd65fd23eb7969e6de
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

### `dpkg` source package: `curl=8.2.1-1ubuntu3.1`

Binary Packages:

- `curl=8.2.1-1ubuntu3.1`
- `libcurl4:amd64=8.2.1-1ubuntu3.1`

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
- `OLDAP-2.8`
- `X11`
- `curl`

Source:

```console
$ apt-get source -qq --print-uris curl=8.2.1-1ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_8.2.1-1ubuntu3.1.dsc' curl_8.2.1-1ubuntu3.1.dsc 3094 SHA512:cb16bac3813df485fa48be18080d3d967518031828187405e3c27bedd58ee410d5c3684968d40a58882b6366739cb94ca792ae1395616d0428ec7c6ad11ae96d
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_8.2.1.orig.tar.gz' curl_8.2.1.orig.tar.gz 4394020 SHA512:d0a906f4dff4c485e6dae930d9a7530147f4c0a0cbb46a83cb9be9d7bd6b9c320386c8be5bcdd3749f2d468b0daf39d06e8c581bab1fa792fd26da409a575cbd
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_8.2.1-1ubuntu3.1.debian.tar.xz' curl_8.2.1-1ubuntu3.1.debian.tar.xz 52240 SHA512:ce024386864f482c09ec1390ee5d613efe0438150e2d5ce6a3247911b4e0999eb003cddd57868d2c3ac1040617e4fe695b0f0edefef624d31a59b02453345eab
```

### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg1-3`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg1-3`
- `libsasl2-modules-db:amd64=2.1.28+dfsg1-3`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-2.2-clause`
- `BSD-3-Clause-Attribution`
- `BSD-3-clause`
- `BSD-3-clause-JANET`
- `BSD-3-clause-PADL`
- `BSD-4-clause-UC`
- `FSFULLR`
- `GPL-3`
- `GPL-3+`
- `IBM-as-is`
- `MIT-CMU`
- `MIT-Export`
- `MIT-OpenVision`
- `OpenLDAP`
- `RSA-MD`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg1-3
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1-3.dsc' cyrus-sasl2_2.1.28+dfsg1-3.dsc 3330 SHA512:3ac2330cb2cd35120eb80cb45866595abaf1dd5fbd357236f8b8e63eee3dd81e41235c10725cdca9b2b6785c36aa1412052f7769fa051cfe57b476c1ad63b2fd
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg1.orig.tar.xz 794540 SHA512:e94075d09b38a50138b782323de286deb7b15008064f07df4fa682e94367e829d9bfafef48d5478f730fef8fde536bcc6d54cab0452b76473a3c620b3dc18fa2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1-3.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg1-3.debian.tar.xz 106568 SHA512:4f602a8532af0bd452ed5be4a018ef60a91527621fc3dca52efd86c2b0ee99697a6f9f7453c1a7fbbbfa130bb889da71ef10fb8d9604fdc8a710c50f302a620b
```

### `dpkg` source package: `dash=0.5.12-6ubuntu1`

Binary Packages:

- `dash=0.5.12-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.12-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.12-6ubuntu1.dsc' dash_0.5.12-6ubuntu1.dsc 2087 SHA512:4f7dab651cbcbb65749c58f99e13ebc9e4e035663c35a5954e79a55fb034f82f1755891b24eac6fdbdcd9d4ea41356f365e01e880a07bd36a0fd77e6da9c333d
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.12.orig.tar.gz' dash_0.5.12.orig.tar.gz 246054 SHA512:13bd262be0089260cbd13530a9cf34690c0abeb2f1920eb5e61be7951b716f9f335b86279d425dbfae56cbd49231a8fdffdff70601a5177da3d543be6fc5eb17
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.12-6ubuntu1.debian.tar.xz' dash_0.5.12-6ubuntu1.debian.tar.xz 39428 SHA512:bab3a9c5bbd839e4a8aaa50df73d4a71b1086dcfebd5d19d12811733382e04e48e694c5f87f901481540cd4e9819503ab246d0270dffde37baaa6dff3f65e454
```

### `dpkg` source package: `db5.3=5.3.28+dfsg2-2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg2-2`

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
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg2-2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-2.dsc' db5.3_5.3.28+dfsg2-2.dsc 2183 SHA512:f9e34e976efb957df08c00d6da2f201e4c2179931942ffb8188cdf7eba24724f42907df0f8a3b275a5aa41ba07518b8a336b39a97e7d35c57dc398f52860585c
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2.orig.tar.xz' db5.3_5.3.28+dfsg2.orig.tar.xz 21287688 SHA512:f9c9d042702ef3fcfdd4b4859583048f3396b161009dc24b6d3a2c53533d58214239fc80e2c42db17e9f092df44d531502737f3b368b956bff49ef057b6b51ef
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-2.debian.tar.xz' db5.3_5.3.28+dfsg2-2.debian.tar.xz 33560 SHA512:c710253211e0ce4d7adfd74ba2ebbc9aac3495f0f5506e18af584569ce77eabaf2c7eae0bc91826bee93ec2f1338ed3c0de6a89cc571af795c535e928afeca81
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

### `dpkg` source package: `debianutils=5.8-1`

Binary Packages:

- `debianutils=5.8-1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`
- `GPL-2+`
- `SMAIL-GPL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.8-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.8-1.dsc' debianutils_5.8-1.dsc 1647 SHA512:8e6471fa22098d7cf13750849ebc0ff2f2bdfd50490186d85e7c7e4bef94ca14b5e02f1339db91ce5df5cf926262d7842c4f5da01aa47c5ac9b6199dc72a0b70
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.8.orig.tar.gz' debianutils_5.8.orig.tar.gz 260865 SHA512:7fddff17804ab334ac1ab3fa4b76a3fed8d83dc2dbf8d9ab1e486b5f226ac8363e98336cfa651c7630eef5fffa4551dbf7a5da1ba60f033b279f9aca624d58a2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.8-1.debian.tar.xz' debianutils_5.8-1.debian.tar.xz 22044 SHA512:7b0f1663447b894d69eb56391324604e705e0af3026fc1a3a08edf891e1c16e29c88e2aaae0c8632ecd2e1965b7118b2921117230139e93484154383dcdd0120
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

### `dpkg` source package: `dpkg=1.22.0ubuntu1`

Binary Packages:

- `dpkg=1.22.0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.22.0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.22.0ubuntu1.dsc' dpkg_1.22.0ubuntu1.dsc 3069 SHA512:0fe848d6e8dbf6e95c206a6ca4b03b96af061c5f3f16dfbc8f9808b8f33fa4593d5fb19bec7b2a4aef4a1bc45957108cbb1304497c95fca5526a5d92454bec2f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.22.0ubuntu1.tar.xz' dpkg_1.22.0ubuntu1.tar.xz 5358284 SHA512:a185638cba29a2054ac40fa59b4b86f6842d10dedd6e53ff7d6c715f1953df6544912a44116a39eec8766903ad23ed2c370d79a745bd48495f105bb9a4df58bd
```

### `dpkg` source package: `e2fsprogs=1.47.0-2ubuntu1`

Binary Packages:

- `e2fsprogs=1.47.0-2ubuntu1`
- `libcom-err2:amd64=1.47.0-2ubuntu1`
- `libext2fs2:amd64=1.47.0-2ubuntu1`
- `libss2:amd64=1.47.0-2ubuntu1`
- `logsave=1.47.0-2ubuntu1`

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
$ apt-get source -qq --print-uris e2fsprogs=1.47.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.47.0-2ubuntu1.dsc' e2fsprogs_1.47.0-2ubuntu1.dsc 3211 SHA512:a0139d8d0528a623e8452366b24313d5bf4d1fa4ad493ab349965c9ad2e8eb00af99b5ea5cb597aaa151856f2be90e52df302b0d6e45d8f93d83ec4860c4650a
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.47.0.orig.tar.gz' e2fsprogs_1.47.0.orig.tar.gz 9637717 SHA512:4f03a469d03cb0f0656bd17c64d944606fb25e68002e3e42c278f3775fee6bf776cc2061ae378b5df4f167a5c33444490111fdcbb140e0320445706f9d048dd0
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.47.0.orig.tar.gz.asc' e2fsprogs_1.47.0.orig.tar.gz.asc 488 SHA512:cd3652ec12f694f1c1f5bd4af4964bb32ad832ba8a06a48864d12a998dc514e9a950ebdb475707a3abb8360852a3469794f2327f097328c99233beef575df144
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.47.0-2ubuntu1.debian.tar.xz' e2fsprogs_1.47.0-2ubuntu1.debian.tar.xz 89008 SHA512:3e75641abe50c48202ea2ddb7bb23939201ae1d739298920525590474447c85cf921518cac05b167cbd02470ac19108abe12a25943759b300c11cf552aea7cb0
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0-5.dsc' findutils_4.9.0-5.dsc 2272 SHA512:8f901310a8e3b1957ee3a4ada366a070c0596a7e706dc6b917dde0ecf75737e72b9bfe1d0c2812676b733e077c93929c5899b0bb50e7e966e109b2473e75d698
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA512:ba4844f4403de0148ad14b46a3dbefd5a721f6257c864bf41a6789b11705408524751c627420b15a52af95564d8e5b52f0978474f640a62ab86a41d20cf14be9
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA512:b8e0b5471242912a20b9e468fa27b7f27339af5f7be8918173105262dee0152183bf4cf516844d348b206a694e028490d5d3b190f3aed8c698ba5444941f8dfc
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.9.0-5.debian.tar.xz' findutils_4.9.0-5.debian.tar.xz 32744 SHA512:64b5df8347a4d698787dae61c0adac845b0dc66450736931e04c5ad072756a5e5191c8e4995e4fa5a568caf0f851518eb3c8358991a4e5749c3f2306b5446380
```

### `dpkg` source package: `gcc-13=13.2.0-4ubuntu3`

Binary Packages:

- `gcc-13-base:amd64=13.2.0-4ubuntu3`
- `libgcc-s1:amd64=13.2.0-4ubuntu3`
- `libstdc++6:amd64=13.2.0-4ubuntu3`

Licenses: (parsed from: `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-13=13.2.0-4ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13.2.0-4ubuntu3.dsc' gcc-13_13.2.0-4ubuntu3.dsc 27652 SHA512:161ebdcff6af93dac86b5591e9ff35abfee8b2cad1c881c09e289c7cb6ed22c9a0c71a315061bc2e90eb992367d1e04a620a3eb386c75c6741dbd53efb2bdb15
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13.2.0.orig.tar.gz' gcc-13_13.2.0.orig.tar.gz 92596024 SHA512:cf149aff3cbee36bf23987e91016fa3f93dbcba8c88319876e6aa3cacd1dacea27d06ea7c4da6394a56d7d9d4f14ac928ead7d25502f0cc6db558f7f5cd99dff
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13.2.0-4ubuntu3.debian.tar.xz' gcc-13_13.2.0-4ubuntu3.debian.tar.xz 1581144 SHA512:7ea0e627632deafe26cf219e4288fb9e1a6b9a7df4c8d2177fce9111b021d5d580ceff5cdcaf11adccb3bb4c72d3aac289417b67365ef771b8a2de4b43301dc9
```

### `dpkg` source package: `glibc=2.38-1ubuntu6`

Binary Packages:

- `libc-bin=2.38-1ubuntu6`
- `libc6:amd64=2.38-1ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.38-1ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38-1ubuntu6.dsc' glibc_2.38-1ubuntu6.dsc 9484 SHA512:5f7324036202076e30f63c1390d6e3bda0ef2d7ae8dbdf5a476f9ec6191860d3a218d552286e9503425a5b170cb5dc0789195a6d20f3ed25b1c1dde731255d97
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38.orig.tar.xz' glibc_2.38.orig.tar.xz 18913712 SHA512:a6dd5e42dcd63d58e2820c783522c8c895890b6e8c8e6c83b025553de0cc77cdf227e7044e431ead98c89c68a9ce4dd63509b47e647775fb2075f011849c1900
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38.orig.tar.xz.asc' glibc_2.38.orig.tar.xz.asc 833 SHA512:32248467450f4530f8e84c03ea78d8293946e1b1def853eff9fb2cb51106e66cc3b024a254f3c2fabd2634f8192bd14e7df00c317f4230860d702c4d9ec7a01e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38-1ubuntu6.debian.tar.xz' glibc_2.38-1ubuntu6.debian.tar.xz 458452 SHA512:054379cce460d74dcb35f20fdfac4ca828548bc4981af0e95ef58ceb8126b2cd05a9c2f655ec32d22fa6be51e5767d85af6a14040ff891e80b7ce22cf91986bf
```

### `dpkg` source package: `gmp=2:6.3.0+dfsg-2ubuntu4`

Binary Packages:

- `libgmp10:amd64=2:6.3.0+dfsg-2ubuntu4`

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
$ apt-get source -qq --print-uris gmp=2:6.3.0+dfsg-2ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.3.0%2bdfsg-2ubuntu4.dsc' gmp_6.3.0+dfsg-2ubuntu4.dsc 2362 SHA512:752c712621f802d56b22b8031f1449ac69d8c271eb7d1f69cc2feeb85cf31849ece2ae488969e9502b9538f75343244bcbc622bbbc7a909d57eae2bf48c5e754
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.3.0%2bdfsg.orig.tar.xz' gmp_6.3.0+dfsg.orig.tar.xz 1870556 SHA512:a422b29024464aeb26c69f64be1bc37407d74e0290f44f67fc040fe38b97f3eb7aa6ba8380722ef36cac39816d1c4f24b771159fb86d5979ef0791dcdef708bc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.3.0%2bdfsg-2ubuntu4.debian.tar.xz' gmp_6.3.0+dfsg-2ubuntu4.debian.tar.xz 38680 SHA512:79fc5aaa101f7cf4390dc9378e1c9e871b77822473c9ba19f0c4e305fa0e47f417bd7c7da0fdd5e939363ea9d5e111dfb755e7170b81aca038796220d72a8697
```

### `dpkg` source package: `gnupg2=2.2.40-1.1ubuntu1`

Binary Packages:

- `dirmngr=2.2.40-1.1ubuntu1`
- `gnupg=2.2.40-1.1ubuntu1`
- `gnupg-l10n=2.2.40-1.1ubuntu1`
- `gnupg-utils=2.2.40-1.1ubuntu1`
- `gpg=2.2.40-1.1ubuntu1`
- `gpg-agent=2.2.40-1.1ubuntu1`
- `gpg-wks-client=2.2.40-1.1ubuntu1`
- `gpg-wks-server=2.2.40-1.1ubuntu1`
- `gpgconf=2.2.40-1.1ubuntu1`
- `gpgsm=2.2.40-1.1ubuntu1`
- `gpgv=2.2.40-1.1ubuntu1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.40-1.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40-1.1ubuntu1.dsc' gnupg2_2.2.40-1.1ubuntu1.dsc 3920 SHA512:c2cfd636e9bdfc8fe19d9213597325782fe15bd228d0e7d601f18c37d23c2be81c62337621bb835d2defc85feade8f67c4a7f680902d32c77f112cfa2258c7bb
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2' gnupg2_2.2.40.orig.tar.bz2 7301631 SHA512:4c2f5fbf37ba6fbad0045aad23129186963010c673ea0b81801adc4f98efe14d6c7228e22815b6b26307c1fe5bb51cd088aa6a0f06a9325d3c021849ef81c594
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2.asc' gnupg2_2.2.40.orig.tar.bz2.asc 228 SHA512:50e8abae322430bf4d3230d0291ca519663a1397fe0d0b8df29076808504b5fea2b984952d6dc51ecc239c12af8ecd5d93b88dd1c6bc0babf0b48a5a840b8ada
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.40-1.1ubuntu1.debian.tar.xz' gnupg2_2.2.40-1.1ubuntu1.debian.tar.xz 65264 SHA512:1efaad1ebfcda85888670e613bb4488ff2ad773190a593f4d2ac298e731a5641e84bfc2c0dba4b5fd8f1af455212a388b99f903dfc770a772d45b4ccaafcb2e1
```

### `dpkg` source package: `gnutls28=3.8.1-4ubuntu1.1`

Binary Packages:

- `libgnutls30:amd64=3.8.1-4ubuntu1.1`

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
$ apt-get source -qq --print-uris gnutls28=3.8.1-4ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1-4ubuntu1.1.dsc' gnutls28_3.8.1-4ubuntu1.1.dsc 3346 SHA512:5649921bc85996ab6942677313c0e8d99b6b2864248c8f823897461fbdc00bda85e0d0603dc23ec4b7f52443fed179c1321d24f66226e2d73bb6fcd5ec910193
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1.orig.tar.xz' gnutls28_3.8.1.orig.tar.xz 6447056 SHA512:22e78db86b835843df897d14ad633d8a553c0f9b1389daa0c2f864869c6b9ca889028d434f9552237dc4f1b37c978fbe0cce166e3768e5d4e8850ff69a6fc872
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1.orig.tar.xz.asc' gnutls28_3.8.1.orig.tar.xz.asc 996 SHA512:ad42a077718a91b82959ee7ed8282b69e73825c70c5c60eb4a1f87aab055dee2ac74a03f489d5f11c2094ec6ac01ea44c0daffb61cb4daae714dcaf5ea89ecd0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1-4ubuntu1.1.debian.tar.xz' gnutls28_3.8.1-4ubuntu1.1.debian.tar.xz 73432 SHA512:a298420308677b92f11c58e7ed46e1cd99f4a3ff36e2d649a56a78902a04fa01622184480fcab7832116162008a0678bc450878b981e8076546e2544d53b4cab
```

### `dpkg` source package: `grep=3.11-2`

Binary Packages:

- `grep=3.11-2`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.11-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11-2.dsc' grep_3.11-2.dsc 1618 SHA512:faf7da2c0e441300787bc4ad52188bff8d667079867df26dcd86a54a9e5d6d919938c1fb3b51fd7125f761cfdba91020c2797562687943324cb53566d1629eb2
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11.orig.tar.xz' grep_3.11.orig.tar.xz 1703776 SHA512:f254a1905a08c8173e12fbdd4fd8baed9a200217fba9d7641f0d78e4e002c1f2a621152d67027d9b25f0bb2430898f5233dc70909d8464fd13d7dd9298e65c42
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11.orig.tar.xz.asc' grep_3.11.orig.tar.xz.asc 833 SHA512:487aba063373ca0594c519991f19b2a6a33b3da0d74735c890f3828fd0880e7e6f64495d2c8f9efa5da53d1eb2d446609bab2399a4b89dcb4510a632e31ffb54
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11-2.debian.tar.xz' grep_3.11-2.debian.tar.xz 20388 SHA512:25ebdf45c3268d3520fd650aba4c2e845c7aec7f59740d3fadcef939ae51b4d69fb8788253a648bbf8c3be315369d59a814c18307b6ac1ea4d20458241bd1860
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

### `dpkg` source package: `init-system-helpers=1.65.2ubuntu1`

Binary Packages:

- `init-system-helpers=1.65.2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.65.2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.65.2ubuntu1.dsc' init-system-helpers_1.65.2ubuntu1.dsc 2314 SHA512:37f649551c147cf7072b21d2c458ee7d9ca912ae7bca9980b49a53f4530011e65867e8ad5fedf42b6b393855454016340a7c6fee19b7224d600f52a0154afa15
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.65.2ubuntu1.tar.xz' init-system-helpers_1.65.2ubuntu1.tar.xz 47788 SHA512:ec563fd3e71adf007a442911d1d8ea8b13f3c99229b28ecd1da8df6a895683049287d7f4d42ecf1b5574b6ce3fb124259522b777e76a5c33f18f80a0fad7a251
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

### `dpkg` source package: `krb5=1.20.1-3ubuntu1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.20.1-3ubuntu1`
- `libk5crypto3:amd64=1.20.1-3ubuntu1`
- `libkrb5-3:amd64=1.20.1-3ubuntu1`
- `libkrb5support0:amd64=1.20.1-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20.1-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-3ubuntu1.dsc' krb5_1.20.1-3ubuntu1.dsc 3920 SHA512:c9dfc58de924bef20e55cd82232a776e555c6c3f251929c169511d10c62844f4a8fe7f44cc73c39faaa095bdea567c1fcfd6a3ace63bb49b626676650c65553a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz' krb5_1.20.1.orig.tar.gz 8661660 SHA512:6f57479f13f107cd84f30de5c758eb6b9fc59171329c13e5da6073b806755f8d163eb7bd84767ea861ad6458ea0c9eeb00ee044d3bcad01ef136e9888564b6a2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz.asc' krb5_1.20.1.orig.tar.gz.asc 833 SHA512:1d3312bd67581e07adfdadf2c5fe394179631d8add8bd075efefe982a0de22369004e60a14422d426382c8c591e4181b9897088afe9d4e86f0b5a97e5954c67a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-3ubuntu1.debian.tar.xz' krb5_1.20.1-3ubuntu1.debian.tar.xz 100536 SHA512:39ca9dfafb381bd346d5d63a1915b94b85a57d3e6f4803c4ac34d5ab9541c0f18153508bb99791330848a0208454b006c09db3599ff33b2b6bb6e02f61d26062
```

### `dpkg` source package: `libassuan=2.5.6-1`

Binary Packages:

- `libassuan0:amd64=2.5.6-1`

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
$ apt-get source -qq --print-uris libassuan=2.5.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.6-1.dsc' libassuan_2.5.6-1.dsc 1997 SHA512:0a850d34564d555a25b067f6a60ab49a4e6dd07b5bf9a1cac175fbde3c1cf1499783d2a1c7de1464f2deacddf5b2ee4f94c47140ea0c920f731e961f8c45eccc
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.6.orig.tar.bz2' libassuan_2.5.6.orig.tar.bz2 577012 SHA512:dcca942d222a2c226a7e34ba7988ee0c3c55bd6032166eb472caf2053db89aeeea7a40e93d8c2887c7ee73c5f838e8b0725e8cfb595accc1606646559362f7ee
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.6.orig.tar.bz2.asc' libassuan_2.5.6.orig.tar.bz2.asc 228 SHA512:aaa1222607320c260d7339a95cca6532947782520b07df3198a5a228129e0247b87f6f3b6fea17590147fbc7345ea36bfa8da45116d3d85c6fc2d4a3df0f629b
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.6-1.debian.tar.xz' libassuan_2.5.6-1.debian.tar.xz 14284 SHA512:6cb39b7745e1f4312f48662821ddfc92247574e545c75456e655e938ee72a419749e82251a7bcdbb29c4145e8c2c65e62aaa3f08cca9b3993c2548d4ac68be85
```

### `dpkg` source package: `libcap-ng=0.8.3-1build2`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1build2`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.8.3-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1build2.dsc' libcap-ng_0.8.3-1build2.dsc 2231 SHA512:0c6e48e6ef5e64cdf97cdb7f16a0cb8fd35e9928ac50f5e0d17035a93906914142c08a31f804a2de15364eeb87278c65ae3b2807cd01bd8b7b6c2e034124c021
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.8.3.orig.tar.gz' libcap-ng_0.8.3.orig.tar.gz 455383 SHA512:0ef9bc7bc6b7b59991f43b79aa6cde3e8d2c22c4b9ced2af8deae501e01d51e893033d109cb8aa0fdcba190140110993089245346334d7b114d18f1bb1b55b97
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1build2.debian.tar.xz' libcap-ng_0.8.3-1build2.debian.tar.xz 10604 SHA512:bec471e45d3550a498e62c66ffe76e76fb799c6b1634b873ddcff61e7ecb7da906634c76323485452e0df85faa2ba530ba1608079e84413ab38b3365bda0a053
```

### `dpkg` source package: `libcap2=1:2.66-4ubuntu1`

Binary Packages:

- `libcap2:amd64=1:2.66-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.66-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.66-4ubuntu1.dsc' libcap2_2.66-4ubuntu1.dsc 2336 SHA512:884095371ffcf06c2e1b5f2a5e9e68f369558767e969c22aeec741a5b57e8cc91ee0311876d165839b55211c93a36c1e1121ce9faaf8d48aa13013eebb0179f4
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.66.orig.tar.xz' libcap2_2.66.orig.tar.xz 181592 SHA512:ac005b622f6e065f30ce282a5c87240e7b9da75366ee537aa4835bc501b44bc242c10a4ba4dc070e2415fc7f635d1c3c4e45fbeeaf962cf7973dda82bf6377f0
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.66-4ubuntu1.debian.tar.xz' libcap2_2.66-4ubuntu1.debian.tar.xz 22076 SHA512:1f19fc5203de495bf3edb52249bcd6ea14a30b521f223cf75171b6b521c370bf8a21def958307d1712d6ad187b938d2a684ee400279f100c0836f24c7fab99cf
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

### `dpkg` source package: `libgcrypt20=1.10.2-3ubuntu1`

Binary Packages:

- `libgcrypt20:amd64=1.10.2-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.2-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2-3ubuntu1.dsc' libgcrypt20_1.10.2-3ubuntu1.dsc 2906 SHA512:a77e7d0baa3a658bab8a46e6ced85b82902d7297c5372f973e253664780a49a7c3dd5747d7bf90f8669e947edf81d1dada0c03557836f8e2ee77fd72579b9630
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2.orig.tar.bz2' libgcrypt20_1.10.2.orig.tar.bz2 3795164 SHA512:3a850baddfe8ffe8b3e96dc54af3fbb9e1dab204db1f06b9b90b8fbbfb7fb7276260cd1e61ba4dde5a662a2385385007478834e62e95f785d2e3d32652adb29e
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2.orig.tar.bz2.asc' libgcrypt20_1.10.2.orig.tar.bz2.asc 228 SHA512:151ac009da846f4f97fc5f8d936c90da53a69e0824890b860249add4620480ca00e239b8b886f2e071e81095f120cf67c991ae981ac0fb58d56ea011c26957ab
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.2-3ubuntu1.debian.tar.xz' libgcrypt20_1.10.2-3ubuntu1.debian.tar.xz 37508 SHA512:c34fe218a47bdf4fd22b3819473723cdd3b4e75c046c535f2c24e5c6712a5664846f3a15b6438eab08cd3226da6b3963b495e70a12f2ce3ed0cc4bc018c2ba2f
```

### `dpkg` source package: `libgpg-error=1.47-2`

Binary Packages:

- `libgpg-error0:amd64=1.47-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.47-2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47-2.dsc' libgpg-error_1.47-2.dsc 2896 SHA512:432611469c1a587b637b0c5d2d714267bf502c5a23f356833dba51f35d41dc77f9656d2230288312be480203900a710c4d05680bf43cbfd763e7c8a086fd2652
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47.orig.tar.bz2' libgpg-error_1.47.orig.tar.bz2 1020862 SHA512:bbb4b15dae75856ee5b1253568674b56ad155524ae29a075cb5b0a7e74c4af685131775c3ea2226fff2f84ef80855e77aa661645d002b490a795c7ae57b66a30
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47.orig.tar.bz2.asc' libgpg-error_1.47.orig.tar.bz2.asc 228 SHA512:babf3a17429aa7ad5d952099ea8d21bb5c9ba1bc74ea46f3027e0293449c32365208a05e141fa0bf033491320679b0b212f49919452f3dc63cce5d7f355d7195
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47-2.debian.tar.xz' libgpg-error_1.47-2.debian.tar.xz 18540 SHA512:1675eb79550e249451dde1035cd875146eb29637f707eb49b8828b20b217b0a4df323e7cabc57fb5a32bbe8667d998cc395a11685432f5d8f48e9d698e96b3de
```

### `dpkg` source package: `libidn2=2.3.4-1`

Binary Packages:

- `libidn2-0:amd64=2.3.4-1`

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
$ apt-get source -qq --print-uris libidn2=2.3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4-1.dsc' libidn2_2.3.4-1.dsc 1915 SHA512:6c135e607124a4574c43b857a02ae91b3bab4f9a779b13864982d39b07aa16f14381b569706ce4bbad824806a7de748a1e88592214c0806723da1ee33ee5098d
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4.orig.tar.gz' libidn2_2.3.4.orig.tar.gz 2083823 SHA512:a6e90ccef56cfd0b37e3333ab3594bb3cec7ca42a138ca8c4f4ce142da208fa792f6c78ca00c01001c2bc02831abcbaf1cf9bcc346a5290fd7b30708f5a462f3
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4.orig.tar.gz.asc' libidn2_2.3.4.orig.tar.gz.asc 228 SHA512:d2a575723326ae256a60e3edf7766af65434f716e11f963bb7ac29b6b2ff2872b41684a1bd1c6f3a3921e8a083512eff1faf2b0fc02513095c2bcf3563312fe0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4-1.debian.tar.xz' libidn2_2.3.4-1.debian.tar.xz 16024 SHA512:0a0cffe0896656ccee725ec270b2cd7dad010d2dc1cb53e05fb8f06633567746e752cf86d0c0ab4eccd7535595ed63498340c3b2b3cec3a8a53d3bb7b3b0ac2f
```

### `dpkg` source package: `libksba=1.6.4-2`

Binary Packages:

- `libksba8:amd64=1.6.4-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.4-2.dsc' libksba_1.6.4-2.dsc 2482 SHA512:34051a546f010964a6dfb88731890f495f783f8a1dc54d0295731893f27b8a6170108a49bb00f1a5f3db391ffb29a07bb2d95addcc025376fc076a207e89f430
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.4.orig.tar.bz2' libksba_1.6.4.orig.tar.bz2 668445 SHA512:07bc26584d1901b2975a02012d90084e3c247a7aeab56d7bcc7197ef0210ece0c4ffd5cb468b998ef696deadfcfdc5fa5dc367077863926503e8f7a8d06856a5
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.4.orig.tar.bz2.asc' libksba_1.6.4.orig.tar.bz2.asc 228 SHA512:f7c53c41927a5bdd3ed4e30ca06b61009ff8506cb6eb5d89c6fe60e23bac8a9bf6d74114c9df5c2c283f4adbf930c6ed916a45a91f4f4f6158e7af23df7b30e2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.4-2.debian.tar.xz' libksba_1.6.4-2.debian.tar.xz 14652 SHA512:3631c4c2777d8120cea117c65cc990d6cadf31e9d7daedde80c640de19c839d1495d0ed42d38a1620e04ed93985da5de875b7f37a83271ee2f81564a6eaf8bd8
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.1.0-1.dsc' libmd_1.1.0-1.dsc 2283 SHA512:0838dfa6755a4e0ce750bc31fa7db32e66000ebfae117b92ad7f1b81b89fbfd1e209ad6bf2d5e19df5ef7b5f4d057c39974f4c475626ea69cc93d05d7fd64ceb
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.1.0.orig.tar.xz' libmd_1.1.0.orig.tar.xz 271228 SHA512:5d0da3337038e474fae7377bbc646d17214e72dc848a7aadc157f49333ce7b5ac1456e45d13674bd410ea08477c6115fc4282fed6c8e6a0bf63537a418c0df96
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.1.0.orig.tar.xz.asc' libmd_1.1.0.orig.tar.xz.asc 833 SHA512:b0ff3baa7eedc205ee6f8b844859145fa6922c39e8f62f1e997851a65b2881649b438a37baa5800d140541da6f4dacc9f92a370f945d7461937b8cdedeca1cef
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.1.0-1.debian.tar.xz' libmd_1.1.0-1.debian.tar.xz 8156 SHA512:d5e657388c32afaa86e1ff86f35f354202065534173eadcc7118afefd1a37fc7f9e97a76f121f20ac7be8c6d53b7eeab242f2f52062e6679e4d470b969fcc581
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

### `dpkg` source package: `libseccomp=2.5.4-1ubuntu3`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.4-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4-1ubuntu3.dsc' libseccomp_2.5.4-1ubuntu3.dsc 2799 SHA512:ed969f1feed2e25afc3e67f09523113a265e10dfe5fbec5e93b088549e5953ab974333e567159d434402e1098ef4f6d305587285aa09eb15514ee594ddffda33
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz' libseccomp_2.5.4.orig.tar.gz 637228 SHA512:92650bd7d1d48b383f402a536b97a017fd0f6ad1234daf4b938d01c92e8d134a01d2f2dd45fd9e2d025d7556bd1386ec360402145a87f20580c85949d62cea0e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz.asc' libseccomp_2.5.4.orig.tar.gz.asc 833 SHA512:10ce632da2762e3b5acb468194b2424d80bab786cc5923a8ee0b0684290282ef2f0a17192680afb36626c82e73a3ba64e73f248ed63cd3e55c3cf8cee4e1e447
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4-1ubuntu3.debian.tar.xz' libseccomp_2.5.4-1ubuntu3.debian.tar.xz 23700 SHA512:980b86e14cabebff0833bc63472e58a936c8f221cd0fc8ebd273c3fe81164d6617fd98a271c422e98deb346b358801069011f7488eca512225f0e1356c9a4469
```

### `dpkg` source package: `libselinux=3.5-1`

Binary Packages:

- `libselinux1:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5-1.dsc' libselinux_3.5-1.dsc 2662 SHA512:2de111b672f95c6caafdd32f219e2036c47171ed1855ac42e51bd659a4adc611084a041a902ee3966efa800f8e13858aecfc56f5cb14618fb67663ba37f13318
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5.orig.tar.gz' libselinux_3.5.orig.tar.gz 211453 SHA512:4e13261a5821018a5f3cdce676f180bb62e5bc225981ca8a498ece0d1c88d9ba8eaa0ce4099dd0849309a8a7c5a9a0953df841a9922f2c284e5a109e5d937ba7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5.orig.tar.gz.asc' libselinux_3.5.orig.tar.gz.asc 981 SHA512:ba486d29c92801a02f75213ef5bcc4a0c4a87afe9dfa797aa9bb495ded40f21e37b22d6ea114c0e480d669b090d1116e8b9cac9fa9ea29678d3647bc58d8bb29
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5-1.debian.tar.xz' libselinux_3.5-1.debian.tar.xz 35804 SHA512:4fff1551a292eb30f06397889efeb87bbf227ffc0325498a0dd18d3ed6269adddb57020c648d1271546d391e1a2fa166c921335627a632a3ea5aa72f3b19406e
```

### `dpkg` source package: `libsemanage=3.5-1`

Binary Packages:

- `libsemanage-common=3.5-1`
- `libsemanage2:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5-1.dsc' libsemanage_3.5-1.dsc 2644 SHA512:73917cb27a588859c78e1ed4ff1ea7204480d1a6dc11a11339d5167897b3048eff2df9f65498d16d684587a4f4a5278dfabc0c12f924f248b0adb2acfdfa439f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5.orig.tar.gz' libsemanage_3.5.orig.tar.gz 185060 SHA512:959fbd0d6bc6849da6caa13dc41c3f8818cbbd29f04b5d2ac7246c4b395b4f370f113a04cc9cfcb52be2afebfa636013ac4ad4011384c58c7ce066a45cae2751
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5.orig.tar.gz.asc' libsemanage_3.5.orig.tar.gz.asc 981 SHA512:c0a5ddb69c32ddefa26b3d1ec676bcc373e959dd8b4a7fcf6e1f74a3ca8e9af22af851ca66d3c43a704215ff79d27244e33d23038ef2f52ccc321aeb5f0c2790
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5-1.debian.tar.xz' libsemanage_3.5-1.debian.tar.xz 29956 SHA512:333264bd9dd88af0e87c4aeabf99ca59e2bc6e1bbed10f0372d4fabc72f0fac0ce86e68d68bdbbb0a51bd133c218226e6027b1db3b7e9e718da995bbdec1d0e6
```

### `dpkg` source package: `libsepol=3.5-1`

Binary Packages:

- `libsepol2:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5-1.dsc' libsepol_3.5-1.dsc 2005 SHA512:8378eb7a3514918ba6c355bec5e6c48fc1a34900635cee77d73e942ae3c538228aa41f0c367dc63c30d01832edf2537592563473f379f7de661df1b5cef7d5cd
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5.orig.tar.gz' libsepol_3.5.orig.tar.gz 497522 SHA512:66f45a9f4951589855961955db686b006b4c0cddead6ac49ad238a0e4a34775905bd10fb8cf0c0ff2ab64f9b7d8366b97fcd5b19c382dec39971a2835cc765c8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5.orig.tar.gz.asc' libsepol_3.5.orig.tar.gz.asc 981 SHA512:5aa46c3a7a5d7fa0d4376766b9444cdea1b14f3ec61725950a24fcb5ba2caae271a415c613807d06e4d9b04b40cda1525c12c442eed8a7e60fb5e5beacdaba3b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5-1.debian.tar.xz' libsepol_3.5-1.debian.tar.xz 27500 SHA512:f813e8003269b11851d027759f319ea527b07d202d40a23578a313ca6750b143e41a5a137b7772b329141544001f996c8b801b998e404d58686bc47da4a3064f
```

### `dpkg` source package: `libssh=0.10.5-3ubuntu1`

Binary Packages:

- `libssh-4:amd64=0.10.5-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.10.5-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.5-3ubuntu1.dsc' libssh_0.10.5-3ubuntu1.dsc 2234 SHA512:b6cedd5aefd1d571528285b633df9daf2d471ddea801cdf0ecc50de76d99ef780aec9ee646a45c38e1d6a28320968ade01c6c2656e935f66be897a8a66917a44
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.5.orig.tar.xz' libssh_0.10.5.orig.tar.xz 557776 SHA512:2b758f9df2b5937865d4aee775ffeafafe3ae6739a89dfc470e38c7394e3c3cb5fcf8f842fdae04929890ee7e47bf8f50e3a38e82dfd26a009f3aae009d589e0
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.5.orig.tar.xz.asc' libssh_0.10.5.orig.tar.xz.asc 833 SHA512:aad5e75d0a5b2e93c6de08f2b6953f05dbef47e14a08eb75c57d3f519a8323064454ba5fbc86b3538489f571a5e446ed942f2b1cea2063c8645ef36815dd2511
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.10.5-3ubuntu1.debian.tar.xz' libssh_0.10.5-3ubuntu1.debian.tar.xz 29520 SHA512:385999ddfbe9d73f4c101942253e47d9bbdf154fb72082a9c89094e2478d698f202bb9575f79f48e221f8ffa6ffe24875e1fe051cd1da662e626f6ffde412add
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-3.dsc' libtasn1-6_4.19.0-3.dsc 2662 SHA512:22e3935a2af804263921c947eaa149bcc1bf32f4bb8c704242d5773acdfca8d0f9d8fd8768a5d414b1741e2ead907f1a31e6a33369baf41443a0d26b59112cd3
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz' libtasn1-6_4.19.0.orig.tar.gz 1786576 SHA512:287f5eddfb5e21762d9f14d11997e56b953b980b2b03a97ed4cd6d37909bda1ed7d2cdff9da5d270a21d863ab7e54be6b85c05f1075ac5d8f0198997cf335ef4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz.asc' libtasn1-6_4.19.0.orig.tar.gz.asc 228 SHA512:e0417625f8df22c6421914bf2d4f19d7f27260c24c04f50e59669681f326debe06ddef9dc5a2e20fda50feb30bbbf3f41597e64961257304ec2c407aa76d107e
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-3.debian.tar.xz' libtasn1-6_4.19.0-3.debian.tar.xz 22084 SHA512:abef85645cc23f8434bc6c4cdcb5d2ce01d47f82f3bc689848e027fd1888ddd4396b8cd9ad1abb712024fb2928d97c0dfb231da2eecfc6bdecffd6829c9d4b89
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

### `dpkg` source package: `libxcrypt=1:4.4.36-2`

Binary Packages:

- `libcrypt1:amd64=1:4.4.36-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.36-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.36-2.dsc' libxcrypt_4.4.36-2.dsc 1563 SHA512:dc89e5cf496906c63ac28a7dc7e73566eabec64347e5cec21343b735627a2153216dbd9fb49e4d26c327febbb914cf52fe1065e1cd05cc7408fbb14abe50929a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.36.orig.tar.xz' libxcrypt_4.4.36.orig.tar.xz 392732 SHA512:82839d70fc068a4d4d5e14488ea7599e2430091ace53640d639628330eff52a058ac589b6b5a39bc6c83166e68cbf9b9e2024e0371df1f949336f633f2a1726e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.36-2.debian.tar.xz' libxcrypt_4.4.36-2.debian.tar.xz 8284 SHA512:f6095cadce8d436bd6ebc51514bd8eb401f331d5c29256f8a15d37637ef1c8a7699fbff69a1bb11e10d5a7ed1370c6f3c8ebd975e3ecbf38b2dbf2852f2cca3f
```

### `dpkg` source package: `libzstd=1.5.5+dfsg2-1ubuntu2`

Binary Packages:

- `libzstd1:amd64=1.5.5+dfsg2-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.5+dfsg2-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-1ubuntu2.dsc' libzstd_1.5.5+dfsg2-1ubuntu2.dsc 2352 SHA512:5da90109c61965ef59b100bb1479c243c79c278a4f40bb4fb8dd547bdec153cd7e7f30764e83cd6d34e221425fa6360ffeea19235963a74936605f5e44dc5683
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2.orig.tar.xz' libzstd_1.5.5+dfsg2.orig.tar.xz 1784164 SHA512:0b24cf71636b36ae17f617f0a4a2e1253ba6a7bfcd8b6f4717cc59310e92d23bde0945f885fa80622d84961b85fa6ba74e3436ab1badc687e8a13ac428a71b8d
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-1ubuntu2.debian.tar.xz' libzstd_1.5.5+dfsg2-1ubuntu2.debian.tar.xz 21400 SHA512:ea28ea8fb4eb2ccabb1d959c25dbdbc85b10467f18660c28d97687c3c8383458b70217182c4531da0e5838b91fb743defabf59a643466d12f2034aa373b2150f
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

### `dpkg` source package: `mawk=1.3.4.20230730-1`

Binary Packages:

- `mawk=1.3.4.20230730-1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `GPL-2.0-only`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20230730-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20230730-1.dsc' mawk_1.3.4.20230730-1.dsc 2180 SHA512:a0bd0a9b8d369f08622b3c6ce46917adfa9e4f0f064d969e91ebc862dc484a3026138174ed66caa97a35a5cae65c11682f66f5b4793d31ac839935fd6f9cfdfd
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20230730.orig.tar.gz' mawk_1.3.4.20230730.orig.tar.gz 410248 SHA512:a38dad468db614e36149916656c22b0dcd3e66ce4be73dada355f9c96c3b4c864d81cbd65608cbed315050a36e2a3bd049e28ce41818cd5da260141b4548bf46
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20230730.orig.tar.gz.asc' mawk_1.3.4.20230730.orig.tar.gz.asc 729 SHA512:28b0d46248beb0244a9d584690b70338cb29f6b08c29350522e91d56ce2ab625f9696a637fa23b4b43448883f79c6a007d731367274285ec7fa45547f22b910d
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20230730-1.debian.tar.xz' mawk_1.3.4.20230730-1.debian.tar.xz 15492 SHA512:ee5a6a99a0f676d1601d8d3153c9c4d3d2cf51713937a973f253c210cd47d52c5f5200bd00a7cfa4a44cb22d76c6d9fc5a8f8b28ec0ad50528588d70017fca9c
```

### `dpkg` source package: `ncurses=6.4+20230625-2`

Binary Packages:

- `libncursesw6:amd64=6.4+20230625-2`
- `libtinfo6:amd64=6.4+20230625-2`
- `ncurses-base=6.4+20230625-2`
- `ncurses-bin=6.4+20230625-2`

Licenses: (parsed from: `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.4+20230625-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20230625-2.dsc' ncurses_6.4+20230625-2.dsc 3807 SHA512:2b553a6bfdb99698cab4b3261ab8ba00d8f9204bed0297ceffa8508965386e63d85abed7148c552a2850256f980279bf5b57209afbbd15fde783ef6a32b559d1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20230625.orig.tar.gz' ncurses_6.4+20230625.orig.tar.gz 3649551 SHA512:adb42d67bd82544ee7d9c2e001bef5f8fec7d9e6459e37f4664057a8e88176c9536b5804e847ab8525f78e6ca44841d1d44f84826bce9e443bdb1a4f59ed5bad
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20230625.orig.tar.gz.asc' ncurses_6.4+20230625.orig.tar.gz.asc 729 SHA512:49dce0e1d23288cdb97e786ed145554c4ef421c8944af91805c2359e79ef9aeffd6a386fc4519ef75d1adcf1d55c403204c6b1c30be69a872c5a5c07d1eac98a
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20230625-2.debian.tar.xz' ncurses_6.4+20230625-2.debian.tar.xz 48584 SHA512:5d6cc5875d813bb03f115309e790e7311f983607db16fba9ffc6385d5180253cd1368f7175cd475c0404e98aafde373d9a9f1c26bca1b7ce96b79f3495b2b557
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

### `dpkg` source package: `nettle=3.9.1-2`

Binary Packages:

- `libhogweed6:amd64=3.9.1-2`
- `libnettle8:amd64=3.9.1-2`

Licenses: (parsed from: `/usr/share/doc/libhogweed6/copyright`, `/usr/share/doc/libnettle8/copyright`)

- `Expat`
- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3+ with Autoconf exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-3+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=3.9.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.9.1-2.dsc' nettle_3.9.1-2.dsc 2274 SHA512:4f48a301f663147237b7a74a2ff6ec85fd575650bcbd060ef273a86014d3f2a7048edfb3c6dfc95d73be2d92c7368469cd326e58785910caba21840b1f00f6bc
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.9.1.orig.tar.gz' nettle_3.9.1.orig.tar.gz 2396741 SHA512:5939c4b43cf9ff6c6272245b85f123c81f8f4e37089fa4f39a00a570016d837f6e706a33226e4bbfc531b02a55b2756ff312461225ed88de338a73069e031ced
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.9.1.orig.tar.gz.asc' nettle_3.9.1.orig.tar.gz.asc 573 SHA512:2ca8ab90c2a437c587987492be2a4c71658256020af725b48ee8f25771b7af28a9c1a8e300826dce58c4b691545d450ec44e668187daaa351a63a77eca4cedcb
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.9.1-2.debian.tar.xz' nettle_3.9.1-2.debian.tar.xz 24440 SHA512:5ecbb74a3e05032f4d13cb6f393f6d23b7a2fff4240370f05d973a331c279d6c9cb0fd5ca7d551febf4fd54e30ebb296729284c6327114529c101edcf80ec2cb
```

### `dpkg` source package: `nghttp2=1.55.1-1ubuntu0.1`

Binary Packages:

- `libnghttp2-14:amd64=1.55.1-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `all-permissive`

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.55.1-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.55.1-1ubuntu0.1.dsc' nghttp2_1.55.1-1ubuntu0.1.dsc 2624 SHA512:680aceda2fa5ee0e69f74796058e006cb4eb47cea8cb465fe3d2433c8b896019f90edba061d13d6c6e5bac92d4a85e16e43e927c244b6c9c42054e35fc929202
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.55.1.orig.tar.gz' nghttp2_1.55.1.orig.tar.gz 1071258 SHA512:0ab1a987ec99f7b0652e75a93bebff9a5363f52758be1f6ae8626dcf9f4b2f931dec0a276cdd7b81522c61040e008345ecc5011c17a763b97a48b0f7e2615451
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.55.1-1ubuntu0.1.debian.tar.xz' nghttp2_1.55.1-1ubuntu0.1.debian.tar.xz 17772 SHA512:a0dc51a5c697271befb66d2231cda1775eabb53e9dbe85f24932fed105f29bb45254195d59b243a1d060c0e725e20f4a1680b85ea3948a6c6fd4deaa02d501ef
```

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

### `dpkg` source package: `openldap=2.6.6+dfsg-1~exp1ubuntu1`

Binary Packages:

- `libldap2:amd64=2.6.6+dfsg-1~exp1ubuntu1`

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
$ apt-get source -qq --print-uris openldap=2.6.6+dfsg-1~exp1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.6%2bdfsg-1%7eexp1ubuntu1.dsc' openldap_2.6.6+dfsg-1~exp1ubuntu1.dsc 3470 SHA512:7c1d353d8f310a2e3c19498cc4c45f9d05123fe732f1a82d56296fe899979d622276f3ecd8ef0b4f1cb67b162913a5e9b3c1ed402ff52e06cfe28301f0ff8500
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.6%2bdfsg.orig.tar.xz' openldap_2.6.6+dfsg.orig.tar.xz 3746232 SHA512:50b7b1020926effc305db829b8782bf733aa83cbf94cce41b770af2f00c4136b07a11462a7b62bd7ef273d451e362267cd658549d9bea6b97f201ec1547dd4e4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.6%2bdfsg-1%7eexp1ubuntu1.debian.tar.xz' openldap_2.6.6+dfsg-1~exp1ubuntu1.debian.tar.xz 179316 SHA512:d1f351512ab8c23e2c4daa1a0f69e87824cb04cdfb86e9e9abb5646ca38ef04f798d718ceaf71c574274c23d3847cd1d202e31b0d8e978e59a3a5b294b793dd5
```

### `dpkg` source package: `openssl=3.0.10-1ubuntu2.1`

Binary Packages:

- `libssl3:amd64=3.0.10-1ubuntu2.1`
- `openssl=3.0.10-1ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.10-1ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.10-1ubuntu2.1.dsc' openssl_3.0.10-1ubuntu2.1.dsc 2728 SHA512:1752d632779c2fcb4eb11b1df953df7dcb037507abb8eef22fdfc956179bb7b8074fabde64e044e1e3d867e13fcc37e26bdc34f28d33b9648010d9e8f12b5219
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.10.orig.tar.gz' openssl_3.0.10.orig.tar.gz 15194904 SHA512:fc12f3beed5e2d2f4767aeb772ceb6ba26f6cbfabc247765854108266b27a1223134f0e81735867a9069bc9c07a14b9816e85903cef91bd1b90f781f0b98b61a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.10.orig.tar.gz.asc' openssl_3.0.10.orig.tar.gz.asc 833 SHA512:3d91e763dcb0bb37cf6586b75c5310c824b5ca75e59a206d759081a67bc016add501648a365aa479dc621f33b86e7aac26d1deb528b43a37187d91eb194b2bdc
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.10-1ubuntu2.1.debian.tar.xz' openssl_3.0.10-1ubuntu2.1.debian.tar.xz 146304 SHA512:3f7ff55cd2a71f52c4300843e4b165256e7029a83e9a4d39a94851732793d90dd17460931554eba1174403d19b134c93f1ac319778041e1adfa609526b9c1e8a
```

### `dpkg` source package: `p11-kit=0.25.0-4ubuntu1`

Binary Packages:

- `libp11-kit0:amd64=0.25.0-4ubuntu1`

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
$ apt-get source -qq --print-uris p11-kit=0.25.0-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.25.0-4ubuntu1.dsc' p11-kit_0.25.0-4ubuntu1.dsc 2608 SHA512:8476349970c06d63d1901f18addd135e2f82fb80297ae72ca574db4ce45f3c09ada4edc7e748b8d7969cd753f032c5e840da8716c63ec54e351e649e22429338
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.25.0.orig.tar.xz' p11-kit_0.25.0.orig.tar.xz 958940 SHA512:e6df3cb224f6ff5671bd3c0557503b5f20bbfded1b6ec340b1dafcbd1b1725ea2d41d0e920756716e0fe9cb28270d115fe77b23ec876a15007b22e3f30d015fe
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.25.0.orig.tar.xz.asc' p11-kit_0.25.0.orig.tar.xz.asc 228 SHA512:4ff7f240e9f166f1e28081f0e23d5b0dd699952fc1b7184dc881ec565eff3f4d5622664af3fc3add4cb828570b6ef77ff2036c467589a1e49605fefda3e73748
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.25.0-4ubuntu1.debian.tar.xz' p11-kit_0.25.0-4ubuntu1.debian.tar.xz 25920 SHA512:6325ede913b64e317ddb851ed9f4ae673d8b3ceec300f95f5ad148ac51c49aaba6c506e31320d7ea4744da67ee1bdd817fdaa44a0478c407111a23094b0059d2
```

### `dpkg` source package: `pam=1.5.2-6ubuntu1`

Binary Packages:

- `libpam-modules:amd64=1.5.2-6ubuntu1`
- `libpam-modules-bin=1.5.2-6ubuntu1`
- `libpam-runtime=1.5.2-6ubuntu1`
- `libpam0g:amd64=1.5.2-6ubuntu1`

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
$ apt-get source -qq --print-uris pam=1.5.2-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2-6ubuntu1.dsc' pam_1.5.2-6ubuntu1.dsc 2733 SHA512:b34c61e4c0ec0659a123b9c3baaa69d6fd7cd12b4b005e7bb78fafa3b5ad043be710a085beb848227d124e00bccf13f6ae74ce92c65422fb21ec6a3f379a9a58
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA512:fa16350c132d3e5fb82b60d991768fb596582639841b8ece645c684705467305ccf1302a0147ec222ab78c01b2c9114c5496dc1ca565d2b56bf315f29a815144
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2-6ubuntu1.debian.tar.xz' pam_1.5.2-6ubuntu1.debian.tar.xz 168564 SHA512:902e85fefdd0127e9cc02b6bf6e204c8f504a2428faa6f1854c33f4f7d1505172c7c52b6a2156597fe606b383c951d1c1905dc4f4ef643f7be985c475f2441f9
```

### `dpkg` source package: `pcre2=10.42-4`

Binary Packages:

- `libpcre2-8-0:amd64=10.42-4`

Licenses: (parsed from: `/usr/share/doc/libpcre2-8-0/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-3-clause-Cambridge with BINARY LIBRARY-LIKE PACKAGES exception`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pcre2=10.42-4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.42-4.dsc' pcre2_10.42-4.dsc 2302 SHA512:097275466e22a43e8d62b1ff1e10f87093ced5c9ed3bb5badc3a6d5c675c0757b24dee800a14a2bfd104fda5eebf8b0065d1977651739f8956d85923944ddddc
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.42.orig.tar.gz' pcre2_10.42.orig.tar.gz 2397194 SHA512:a3db6c5c620775838819be616652e73ce00f5ef5c1f49f559ff3efb51a119d02f01254c5901c1f7d0c47c0ddfcf4313e38d6ca32c35381b8f87f36896d10e6f7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.42-4.diff.gz' pcre2_10.42-4.diff.gz 8111 SHA512:d13593a4e46d686238e766b253886eed102d8728a943f2f55d1459311d6e9715be46dd4fc2353d7375100d0200c9c0037521b5072f7ea30826c19af2d48f93e3
```

### `dpkg` source package: `perl=5.36.0-9ubuntu1.1`

Binary Packages:

- `perl-base=5.36.0-9ubuntu1.1`

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
$ apt-get source -qq --print-uris perl=5.36.0-9ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-9ubuntu1.1.dsc' perl_5.36.0-9ubuntu1.1.dsc 3009 SHA512:ffd2fa91526b4cfbca018c25c491dc3a0b5e2ff8bc7518045f9282289808a6e1020d24d7e8d2e2343639a9ead3f180ac94fb45e4bf00627682363b5975828853
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig-regen-configure.tar.xz' perl_5.36.0.orig-regen-configure.tar.xz 417784 SHA512:4d16685f569a5b1dea79d607b6d62718111c32efaf5547bb9e1528bd755acf0c8fc74a1cc1f4d68fcb10aef9da7d8fea17a5cc10dabce6efa4721ab45ab03a65
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig.tar.xz' perl_5.36.0.orig.tar.xz 13051500 SHA512:6dd6ac2a77566c173c5ab9c238cf555f2c3e592e89abb5600bc23ce1cbd0c349e0233f6417cbbf1f6d0aefc6a734ba491285af0d3dc68a605b658b65c89f1dab
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-9ubuntu1.1.debian.tar.xz' perl_5.36.0-9ubuntu1.1.debian.tar.xz 172720 SHA512:9213709c3e6718d3b8c5cb235e1c729e19a44e86622beebcaa553456a73e0373ca7d70d0b68544f2b4398a57245ea051a8e9249f00a9a44545f08d2d4b2b6099
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

### `dpkg` source package: `procps=2:4.0.3-1ubuntu1.23.10.1`

Binary Packages:

- `libproc2-0:amd64=2:4.0.3-1ubuntu1.23.10.1`
- `procps=2:4.0.3-1ubuntu1.23.10.1`

Licenses: (parsed from: `/usr/share/doc/libproc2-0/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:4.0.3-1ubuntu1.23.10.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_4.0.3-1ubuntu1.23.10.1.dsc' procps_4.0.3-1ubuntu1.23.10.1.dsc 2113 SHA512:1273187f092cc2c9abc30f4459d0e7357d71b3d65c3971f2cda370f84183b0ef2783961cca2662b52875250c2702883a65203073abc345019cb4a6bcaeeb2f9d
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_4.0.3.orig.tar.xz' procps_4.0.3.orig.tar.xz 1294992 SHA512:be9dc5ac4a50fc1b8256af44ac2c5b50f74ef5e48c5c3dcac2779d508988daf3b60989d22db8fc8b699c2f2f338ad367e91b9c01ab46ac9fa0d5c5bbec6f16af
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_4.0.3-1ubuntu1.23.10.1.debian.tar.xz' procps_4.0.3-1ubuntu1.23.10.1.debian.tar.xz 34400 SHA512:dc9c3dac33bfaabc2cc36540c96b2ac7501ab9002579d9d934fd4ac9ce4fe1c588dcaabf6e8dcff6aea3a73ad94d1e1ea3a04be4d9b729c4ef6671e978632153
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

### `dpkg` source package: `sensible-utils=0.0.20`

Binary Packages:

- `sensible-utils=0.0.20`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.20
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.20.dsc' sensible-utils_0.0.20.dsc 1737 SHA512:0b0267948347d7aace0c6117228ffa005e5c36e61c9289c409c33d78349fed34956db655541774ec161dc4497d95ccc9d609557f6aaf1d335ced3689ef16a744
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.20.tar.xz' sensible-utils_0.0.20.tar.xz 70608 SHA512:439b783003f9b9361baec01f2888f9638bf7d670b90e7262c50fdff2b724f53f83a776bda385003f61b0bbf37c3213208642e2f1289e93a1ba6b1da2107cb02f
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

### `dpkg` source package: `sqlite3=3.42.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.42.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.42.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.42.0-1.dsc' sqlite3_3.42.0-1.dsc 2486 SHA512:916fedc0a091d2c9e51e65b66d3fd0dccab3666e74a3b219cbae5cbab8c544bcfb5dca7df7186d3b12c7113386cffa2c6f4f3a9d7f70fc43f1013a1201cdf863
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.42.0.orig-www.tar.xz' sqlite3_3.42.0.orig-www.tar.xz 5708628 SHA512:485fcc839414f74a41f4cf795b597fea793016502a9659d989679f3ecccf085909bde655bc605ce8a89029f2ff220e3977dfd35306ccab2c1d23b2e66ed8c6d6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.42.0.orig.tar.xz' sqlite3_3.42.0.orig.tar.xz 8129004 SHA512:a39b8b33761751d90d3b669834bfe10be81bc66bc8c8cfb80fe3d7690c16c74bcda0c9df0be5af855cb5c6b93829de8f22c2307edc01fb61721027ffb118b896
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.42.0-1.debian.tar.xz' sqlite3_3.42.0-1.debian.tar.xz 29996 SHA512:9602cfe54dd78ac1d4005c551215a536e933bb1dcbfc0897bec0fb503d95ddafeb002c991b1a1cd2b642e49e490d1ef311ca97dcb9e3001727353e23b9d69fbc
```

### `dpkg` source package: `systemd=253.5-1ubuntu6.1`

Binary Packages:

- `libsystemd0:amd64=253.5-1ubuntu6.1`
- `libudev1:amd64=253.5-1ubuntu6.1`

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
$ apt-get source -qq --print-uris systemd=253.5-1ubuntu6.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_253.5-1ubuntu6.1.dsc' systemd_253.5-1ubuntu6.1.dsc 6910 SHA512:7aa167b2a6de8bd48b53a4bda661659fd340cf5bb31c7a848442abf3e201c761e478a41342ebaca016c376630fc25e6e88bc541222aaac5793fc3af74638cd91
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_253.5.orig.tar.gz' systemd_253.5.orig.tar.gz 12015672 SHA512:39709b485cd9287e26ac8e973fa1692b280bec3b96e1da6667e4a4f2ac2228aa072b22802720a254698d32c82f5306d7feb32229e4b6d54cc0e2b1e2caa4cc2e
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_253.5-1ubuntu6.1.debian.tar.xz' systemd_253.5-1ubuntu6.1.debian.tar.xz 220212 SHA512:613fa22f71f77d43f1c483b322f2e4601418ae584948e3088386f0edbf14e643730126de1d5b04bf5921c169cbe4a3a5d69c135bb8556b4e1098f97818bf1274
```

### `dpkg` source package: `sysvinit=3.07-1ubuntu1`

Binary Packages:

- `sysvinit-utils=3.07-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.07-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.07-1ubuntu1.dsc' sysvinit_3.07-1ubuntu1.dsc 2466 SHA512:dfc1df22548ae8f82c974092aab9b701323b6d90921a5cfd203ea0109aa11c21490b4c052cd2a4ea9533651b124b9634d4767c7b144b70c4ae8bee473ad2a742
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.07.orig.tar.gz' sysvinit_3.07.orig.tar.gz 513168 SHA512:16e20b9765c6b5e50b2f10fe9e88e00eddb79eb8ebfb632ef98a98796aaaf07a5016f89b1efacdeb36409fd1638d79bce01186d5c7fc907c63d6a9a7195428d9
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.07-1ubuntu1.debian.tar.xz' sysvinit_3.07-1ubuntu1.debian.tar.xz 135556 SHA512:a3a284fa52a67fc81d29d0df0acb64833ae9ab30864aecfcb7f5545e1bf0eb6fcb99f4b76103b2cf98fca12cde421c5c0e66a2559ef7b92db9d39aa641f3d865
```

### `dpkg` source package: `tar=1.34+dfsg-1.2ubuntu1`

Binary Packages:

- `tar=1.34+dfsg-1.2ubuntu1`

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
$ apt-get source -qq --print-uris tar=1.34+dfsg-1.2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1.2ubuntu1.dsc' tar_1.34+dfsg-1.2ubuntu1.dsc 2105 SHA512:113148f046629ee158ab93b9d7e26a4d1dffdcaebf424d35bb6db686dab4a3fd2558098cf425a9c6bd80459f02bd667622589d11dd9147c99a229c74b2aa7e66
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA512:ec5553c53c4a5f523f872a8095f699c17bf41400fbe2f0f8b45291ccbaf9ac51dea8445c81bd95697f8853c95dcad3250071d23dbbcab857a428ee92e647bde9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1.2ubuntu1.debian.tar.xz' tar_1.34+dfsg-1.2ubuntu1.debian.tar.xz 20920 SHA512:83fbef8663b83dfc3eef10b7688cca8b58485acf697c17f1a676f50c4300967dbac2fda5573c4f020a682c7495da2c5e660a6885c50f663ba9549f9e1aed08f2
```

### `dpkg` source package: `tzdata=2023c-9ubuntu1`

Binary Packages:

- `tzdata=2023c-9ubuntu1`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2023c-9ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2023c-9ubuntu1.dsc' tzdata_2023c-9ubuntu1.dsc 2700 SHA512:b6b07c6fe287a0650a156a3f242675f9b9c522b1d08606e4b1f77d5c7f2c7e1730d680239eb43998f77842c238c8485615e3595e59bb795611b7ef5a8c85981a
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2023c.orig.tar.gz' tzdata_2023c.orig.tar.gz 443902 SHA512:608bd286ebcbd0004cfdc1da183273f08aff61f90c8867661154453d77a05d421e4c46ad6d066a1fe2e87d5c82ec0f1c0224667a3b35f3180a3eb7f6ff84cbf5
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2023c.orig.tar.gz.asc' tzdata_2023c.orig.tar.gz.asc 833 SHA512:15da6e01a12a0390f736fe5bacf27595c8f7080a4b27eccfae7f244bc38d5839e7d25622e325f874db17f9e723777e9cfe0f460fbd595b66772f1642dd603b6b
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2023c-9ubuntu1.debian.tar.xz' tzdata_2023c-9ubuntu1.debian.tar.xz 182668 SHA512:3e4d7214d5925ec144dd4a2d371e79e6e6021d4111ed00b87cebc2984c21d62534637d922c37862afaed12dee217c520a87a414e1a7bb5e7652c347662118e1c
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

### `dpkg` source package: `usrmerge=35ubuntu1`

Binary Packages:

- `usrmerge=35ubuntu1`

Licenses: (parsed from: `/usr/share/doc/usrmerge/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=35ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_35ubuntu1.dsc' usrmerge_35ubuntu1.dsc 1717 SHA512:187148b5844858d99506dadb3dc0f18f439df2f01835d1849d07cccfc2819405a0cd722a68ab67e483b4d5fd69e14ce7cf376710ef59edc4ec21610f98dc3c40
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_35ubuntu1.tar.xz' usrmerge_35ubuntu1.tar.xz 15240 SHA512:5116c42163a7b972282ca7af66c268f29197a725fc91020bcd2fcd7ba31f150a705749f3fcf7b02b45d778ffff93e4bc93af0db9491dd28f82e7be9793e9fb0d
```

### `dpkg` source package: `util-linux=2.39.1-4ubuntu2`

Binary Packages:

- `bsdutils=1:2.39.1-4ubuntu2`
- `libblkid1:amd64=2.39.1-4ubuntu2`
- `libmount1:amd64=2.39.1-4ubuntu2`
- `libsmartcols1:amd64=2.39.1-4ubuntu2`
- `libuuid1:amd64=2.39.1-4ubuntu2`
- `mount=2.39.1-4ubuntu2`
- `util-linux=2.39.1-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.39.1-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.39.1-4ubuntu2.dsc' util-linux_2.39.1-4ubuntu2.dsc 4643 SHA512:0e9d2a14c2662687eed1c8aa35fa4b8ce208a33a82fe5c8c6f102cf9caa68d3199680c2fca93dc86d634e0dab9d6a99f83a23baa6a75f122fdc99dfbb5cb10cc
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.39.1.orig.tar.xz' util-linux_2.39.1.orig.tar.xz 8351164 SHA512:8fe2c9014f6161330610f7470b870855cecbd3fab9c187b75d8f22e16573c82516050479be39cfb9f7dd6d7ef1cc298d31d839b194dda5ec4daf0d1197ac71e9
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.39.1-4ubuntu2.debian.tar.xz' util-linux_2.39.1-4ubuntu2.debian.tar.xz 103044 SHA512:72c0480ece71252f940efb6bd6996212f0ccf06ba24e58330b4ad13a13d161ca30e81cfed4cf0575715442da6ba337adbf74eac09abeebb637272a5035be3950
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
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.dsc' xz-utils_5.4.1-0.2.dsc 2621 SHA512:0c07970eedd5b1f67f8750f99dd7f86a1aef12cb1f1b3691fab1b1311d55de76ad597ac55c4e845adee3cdf8d8ba96ceeaed810b6688419934c20e3bafb8bb15
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz' xz-utils_5.4.1.orig.tar.xz 1485272 SHA512:f890ee5207799fbc7bb9ae031f444d39d82275b0e1b8cc7f01fdb9270050e38849bd1269db2a2f12fe87b5e23e03f9e809a5c3456d066c0a56e6f98d728553ea
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz.asc' xz-utils_5.4.1.orig.tar.xz.asc 833 SHA512:0802a4ae8f8fe700288b0fb1a4c9f59f71b26fcaea88cd368d36dcfd96a1deb2380a7b9af66b84d2f4faf68ff114d9b4b4e48b5b8362c37a8e528f13a4233cf3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.debian.tar.xz' xz-utils_5.4.1-0.2.debian.tar.xz 87432 SHA512:0d83bec7f80471ef4b3c5845cc2502807bb41f111970149244de1927618ed758d4e6da455f72eaa9d76acb41d4be685b968b1a8e5883f204277fde75fbc5d79b
```

### `dpkg` source package: `zlib=1:1.2.13.dfsg-1ubuntu5`

Binary Packages:

- `zlib1g:amd64=1:1.2.13.dfsg-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.13.dfsg-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu5.dsc' zlib_1.2.13.dfsg-1ubuntu5.dsc 2968 SHA512:f464da1d48704d87d498db0b2f5e00eaa7e2b58cad27b5493fb6ab96d9ee9555522197d3b948a140bbd7f72ef29e89515c6c17297dd4a2688fb02e7145a9c855
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg.orig.tar.bz2' zlib_1.2.13.dfsg.orig.tar.bz2 1239825 SHA512:266ea72465ad1f0b63e42f8275c650615829929f2ff19064144c5bb942acd31cd8581ce45781c438fce949c6d9f3fa385efa59f754761441107ca1144fb56802
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu5.debian.tar.xz' zlib_1.2.13.dfsg-1ubuntu5.debian.tar.xz 57068 SHA512:2fba202da1d40363e844c0baba3b8af3878087eb7b2b31ab4ba5f26616b1dc9f135483036cc42fbf53a1c359a19370c491d49f01058c91180485229ac3b36343
```
