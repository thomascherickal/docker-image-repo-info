# `buildpack-deps:mantic-scm`

## Docker Metadata

- Image ID: `sha256:82309d805ca626013980144be9e47ab97fba4af8543f5d772705a8d5a0c7ceac`
- Created: `2023-07-04T03:48:01.846731202Z`
- Virtual Size: ~ 240.21 Mb  
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

### `dpkg` source package: `adduser=3.134ubuntu1`

Binary Packages:

- `adduser=3.134ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.134ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.134ubuntu1.dsc' adduser_3.134ubuntu1.dsc 1862 SHA512:038a00d26bef9df837434d2dc081ffa56fbbba9967a5d4e0880de9f3489013c831116ffae7742f44cbb91d0e9b59074abbe4fe1becfe5bc53d72d4fa8c0162d7
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.134ubuntu1.tar.xz' adduser_3.134ubuntu1.tar.xz 275048 SHA512:035b867ba85c371208d30e940bc2d5bdd539864b87805a60e46b3b5a8107cfa5dd2d196150e70d5024f18816c511fffe20f4b0e86f8b8cc34a2fdff86a90f86e
```

### `dpkg` source package: `apr-util=1.6.3-1ubuntu1`

Binary Packages:

- `libaprutil1:amd64=1.6.3-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.3-1ubuntu1.dsc' apr-util_1.6.3-1ubuntu1.dsc 2904 SHA512:3db7e6c9beab7833a9a913011f84a8b59c617202a4941d3054fe649da609bbd19c20f216dc5eaa9fc0455be0369c52f4537957371f892008da7ba0cb78dc1055
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.3.orig.tar.bz2' apr-util_1.6.3.orig.tar.bz2 432692 SHA512:8050a481eeda7532ef3751dbd8a5aa6c48354d52904a856ef9709484f4b0cc2e022661c49ddf55ec58253db22708ee0607dfa7705d9270e8fee117ae4f06a0fe
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.3.orig.tar.bz2.asc' apr-util_1.6.3.orig.tar.bz2.asc 833 SHA512:6c483e823fb032b161b6bcf77f9a43945aee9afbe40050ebf042865434bc533d21168af20d4cdff597b60b782d8ac9322409a5c2a64bf921b22f5add2451d79d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.3-1ubuntu1.debian.tar.xz' apr-util_1.6.3-1ubuntu1.debian.tar.xz 341848 SHA512:624f0a037dbb045574f357573ac314c214225157b94cad1c72b71a0bc687e166a1ecf2077ec15af6ada6f4a8eebfb2632a47ad24314522e57f3ddcec1618c032
```

### `dpkg` source package: `apr=1.7.2-3`

Binary Packages:

- `libapr1:amd64=1.7.2-3`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2-3.dsc' apr_1.7.2-3.dsc 2262 SHA512:011ea43f83fb42bb4a45e2b93b7c4bc7caf4db68c0b7760a50d731bc432646650316f6fc689dc221c818e70bd87a1e75e92e31bbc79b9b8f050b73ee1fa47f77
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2.orig.tar.bz2' apr_1.7.2.orig.tar.bz2 890218 SHA512:0a3a27ccc97bbe4865c1bc0b803012e3da6d5b1f17d4fb0da6f5f58eec01f6d2ae1f25e52896ea5f9c5ac04c5fddcfd1ac606b301c322cf40d5c4d4ce0a1b76e
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2.orig.tar.bz2.asc' apr_1.7.2.orig.tar.bz2.asc 833 SHA512:77da1e516b30032419b36da8453f56c6149ad18631772613adb095b6eccb7606dc51589d33d422572d3fcefe8f6129bfbb06d0ab7fde5848d873856f4ed93940
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2-3.debian.tar.xz' apr_1.7.2-3.debian.tar.xz 54404 SHA512:b3e02e907a52e96723381bc5b68ba1d7c3762d60cb58c25252c1ec0bc1678c26bb48c753554f39ac47ff8a768ef47182a190da561d46cabe3feb40a9fff011a5
```

### `dpkg` source package: `apt=2.7.1`

Binary Packages:

- `apt=2.7.1`
- `libapt-pkg6.0:amd64=2.7.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.7.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.7.1.dsc' apt_2.7.1.dsc 2933 SHA512:6fe05c4302ee250d4fdfe30d23ac9e82537b6e219cf72383e9ea5ec3d77208e24af0b03e633e358363370b2d1e53b0376d77d5e9f6577f73fcbc05adacfd966c
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.7.1.tar.xz' apt_2.7.1.tar.xz 2334088 SHA512:d1af8afac11204e43ded2d108554ba57dc96441f908e9ad5f58d6a708acac391997ee12cd3d36bc06069578bd333aa417ee378b1e83a4dbc6383f8114dd179ad
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

### `dpkg` source package: `audit=1:3.0.9-1`

Binary Packages:

- `libaudit-common=1:3.0.9-1`
- `libaudit1:amd64=1:3.0.9-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.9-1.dsc' audit_3.0.9-1.dsc 2402 SHA512:ab978ec49d49c040ffd9202c017b86b0d9d84013e9da82a3d557b03eb22d57832d94b5dfbe42288d45eda36c06244a45efc2431232f407565f84c5b15a296dca
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.9.orig.tar.gz' audit_3.0.9.orig.tar.gz 1210655 SHA512:5219eb0b41746eca3406008a97731c0083e7be50ec88563a39537de22cb69fe88490f5fe5a11535930f360b11a62538e2ff6cbe39e059cd760038363954ef4d6
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.9-1.debian.tar.xz' audit_3.0.9-1.debian.tar.xz 18784 SHA512:4369817e498acc2f59efac80e646e0b0ebc84bc03bbf17ecc1c41f2a5a611dad413f86441c2f375002364a30ac55f8b248e370cbedf0e8c22d71d4195763841c
```

### `dpkg` source package: `base-files=13ubuntu1`

Binary Packages:

- `base-files=13ubuntu1`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=13ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_13ubuntu1.dsc' base-files_13ubuntu1.dsc 1613 SHA512:64c1efe75319a5cbf1baa91c0fd085772df3bc74dd1d3f3c73cf98c6a06d2775c8aa192c2df0f73496aaeaec8e11a1c353ac0c6cc2a422ee1fed8db14e88cd0f
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_13ubuntu1.tar.xz' base-files_13ubuntu1.tar.xz 93176 SHA512:617ecd27787efcfd8d26bbf3afa42822cab7e9bcbe062c8c97029bf2531c67eeb6bfc0e7c8c23a6e6177327a49d6c9d8d92fad755d1721f66794c82dbaeb4985
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

### `dpkg` source package: `cdebconf=0.267ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.267ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libdebconfclient0/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.267ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.267ubuntu1.dsc' cdebconf_0.267ubuntu1.dsc 2898 SHA512:4b65ba0ddac9efb1c816566b61ce536e7906ddce22a9bd577bc67c73bd8613739e999474aaa5e09b2fb429e6f6c813e193306d6e5daf4dc5427ed7639594f41a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.267ubuntu1.tar.xz' cdebconf_0.267ubuntu1.tar.xz 284400 SHA512:c69be9679c689ef12cd1b385c26e044e251900a60a911a6e9bdddf3eda8ee743e30fc9b9f352fc55cee96683c6f41daf3671768b8aaaaec3a29f513b4a912c6b
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

### `dpkg` source package: `curl=7.88.1-10ubuntu1`

Binary Packages:

- `curl=7.88.1-10ubuntu1`
- `libcurl3-gnutls:amd64=7.88.1-10ubuntu1`
- `libcurl4:amd64=7.88.1-10ubuntu1`

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

Source:

```console
$ apt-get source -qq --print-uris curl=7.88.1-10ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1-10ubuntu1.dsc' curl_7.88.1-10ubuntu1.dsc 3278 SHA512:f4f4f8744ff4b1d19f46d8d538f8439a0bedf9613c2ff02be970f6c8f8c815e6a6106c8b8e81e31408329af2f645b46095bf2a0e8d1ef1eea9c0fb6c28ed8ea5
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1.orig.tar.gz' curl_7.88.1.orig.tar.gz 4343562 SHA512:67701d458548712bbfaa55f2ebefbf87cdbba01b7b1200f608b1c3af67e8dd8e243fa89f256446d217d658a5a1242331d8b0168ab600351e74ee0e2511e79dae
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1.orig.tar.gz.asc' curl_7.88.1.orig.tar.gz.asc 488 SHA512:90029e6304d7ece487594d9192101084e3b0419c9e4296a76b9d32f44d2fb98753ddc6b0b50c2ffc16ab3b04222af607ca4c813d2c01bf1fd1b670d4d7e39404
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1-10ubuntu1.debian.tar.xz' curl_7.88.1-10ubuntu1.debian.tar.xz 56096 SHA512:841abcd5b86ddb6d2e2150e2b0012ac2a76f19a03d0117c45f50815c9d30610858edb293a62518f6b92cd4ef56f42200c4e40cbcb4d46cf647e2f2fe54ce8f40
```

### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg1-1`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg1-1`
- `libsasl2-modules-db:amd64=2.1.28+dfsg1-1`

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
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg1-1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1-1.dsc' cyrus-sasl2_2.1.28+dfsg1-1.dsc 3327 SHA512:f326808288a537ad99079a4f9fb589160d3ba209298950a40d78f51654533104cb4c81c08f53ce341c40a7786d52c4657d5c3ff96eb13718f362e01b26e944bc
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg1.orig.tar.xz 794540 SHA512:e94075d09b38a50138b782323de286deb7b15008064f07df4fa682e94367e829d9bfafef48d5478f730fef8fde536bcc6d54cab0452b76473a3c620b3dc18fa2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg1-1.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg1-1.debian.tar.xz 98608 SHA512:bbb8684417e1f56650af1bbcebf443cbabfb7e5aa5efa78e0309b5f93c41a377e48faf4310d9168d72e1773bf13350ebeb3c6c19905a66fc7467cc791f4c07a2
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debianutils/5.7-0.4/


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

### `dpkg` source package: `dpkg=1.21.22ubuntu1`

Binary Packages:

- `dpkg=1.21.22ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.22ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.22ubuntu1.dsc' dpkg_1.21.22ubuntu1.dsc 3089 SHA512:8f33d351093b3de7922208f429976a86400e6486ccdc626c22dd0d8b786abcd35f89c3f9c524e848e87cf6fac5368152f6e6273d0e0f893169d297001d5a9bfe
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.22ubuntu1.tar.xz' dpkg_1.21.22ubuntu1.tar.xz 5269268 SHA512:0f005b5a9a49337fd2dcdd307e587e840930cbf09cf24a59c6f5652cac4ad8bed961e060269890156ad99759c8192c3e492f5d1fa144e34ed7fff1fe7c1212b7
```

### `dpkg` source package: `e2fsprogs=1.47.0-1ubuntu1`

Binary Packages:

- `e2fsprogs=1.47.0-1ubuntu1`
- `libcom-err2:amd64=1.47.0-1ubuntu1`
- `libext2fs2:amd64=1.47.0-1ubuntu1`
- `libss2:amd64=1.47.0-1ubuntu1`
- `logsave=1.47.0-1ubuntu1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `expat=2.5.0-2`

Binary Packages:

- `libexpat1:amd64=2.5.0-2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.5.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0-2.dsc' expat_2.5.0-2.dsc 1964 SHA512:a71f12ab67b948e890dd1d7e00339acb22cef4f834bc2cd26cbfc04eb5e0d65d56a22e41d384394862104e2e8da0309f4029b059a7adcfdc2d0b0d1acc64ca28
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0.orig.tar.gz' expat_2.5.0.orig.tar.gz 8320988 SHA512:779f0d0f3f2d8b33db0fd044864ab5ab1a40f20501f792fe90ad0d18de536c4765c3749f120e21fec11a0e6c89af1dc576d1fe261c871ca44a594f7b61fd1d9e
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0-2.debian.tar.xz' expat_2.5.0-2.debian.tar.xz 12804 SHA512:3603f3f3f3e4f0bc2c7a29a25aa7c9681ff4a93d48b7e5fabb0d58f8e048c3d7eb0487140f813bd925c4cb2b956a3bd2f68d8c3d75f79066624d83445739cb57
```

### `dpkg` source package: `findutils=4.9.0-4ubuntu1`

Binary Packages:

- `findutils=4.9.0-4ubuntu1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gcc-13=13.1.0-6ubuntu1`

Binary Packages:

- `gcc-13-base:amd64=13.1.0-6ubuntu1`
- `libgcc-s1:amd64=13.1.0-6ubuntu1`
- `libstdc++6:amd64=13.1.0-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23-3.dsc' gdbm_1.23-3.dsc 2583 SHA512:847e5955f668b7ed9e68ff9dd83f68582f53de50190d7fdade5a3ac0fdb9d2f76bf0e17aa5e873e29c2ac9f8b6e611980e80fc2084fd25cca8364ed4c23e0496
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz' gdbm_1.23.orig.tar.gz 1115854 SHA512:918080cb0225b221c11eb7339634a95e00c526072395f7a3d46ccf42ef020dea7c4c5bec34aff2c4f16033e1fff6583252b7e978f68b8d7f8736b0e025838e10
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz.asc' gdbm_1.23.orig.tar.gz.asc 181 SHA512:6653751c04584f10aa3325bd1cb5b9f7970a786dd2a99602ea620c11a86a9ba5c342aa52627bd06c03da822e9e1600dc034d9a8f42856a287fd67f6b9f161c71
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23-3.debian.tar.xz' gdbm_1.23-3.debian.tar.xz 18552 SHA512:bf4f6cc7fba1a2d1eb8aecbb373fdcbd6244040964def34c5559c2643ec02b2acb25f0ff7107336553b3e2abf9ceaf73453e1990988efd951f63c47e67ae4ac6
```

### `dpkg` source package: `git=1:2.40.1-1ubuntu1`

Binary Packages:

- `git=1:2.40.1-1ubuntu1`
- `git-man=1:2.40.1-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.40.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.40.1-1ubuntu1.dsc' git_2.40.1-1ubuntu1.dsc 2956 SHA512:8c085686790fa7b97b02888083fdaaec376b8a48795531436e7986c913c2949bc98c1e564a09a7e23961bf401b7aabafbe854e4cd9b7ef4dc5d8b05498cdc780
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.40.1.orig.tar.xz' git_2.40.1.orig.tar.xz 7185260 SHA512:9ab41c64c6e666c314683bc4925535e037d43f947b8d327ff7d0379ac12899f4effcc2fe4e47b1ce652ad7140aa4f01f3b99f9cc0cf854cfeface1a5d3e1893e
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.40.1-1ubuntu1.debian.tar.xz' git_2.40.1-1ubuntu1.debian.tar.xz 748944 SHA512:52938786bea5817afeed2fcd6f45f35f5567936823de1254670c1379d094f6514b16a5cd02ec67c1e68bad89ceb6b52030533aa063b9c966af32f18fa1409196
```

### `dpkg` source package: `glibc=2.37-0ubuntu2`

Binary Packages:

- `libc-bin=2.37-0ubuntu2`
- `libc6:amd64=2.37-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.37-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37-0ubuntu2.dsc' glibc_2.37-0ubuntu2.dsc 8718 SHA512:d2b2b2a66a80d703c44a7f312c06fe8d79f70ec60eb5a25ebae33c5f31ceafe52b23334d97d6a7350db3b566f3b69dc49bce8c76843df6e7e22fc84328151b91
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37.orig.tar.xz' glibc_2.37.orig.tar.xz 18674604 SHA512:4fc5932f206bb1b8b54828a28af1a681616b838bbab60c81c82155f3629cbfe1301d271af65511ed917f4c6949a025429221fe6035753282f15346919f15b90c
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37.orig.tar.xz.asc' glibc_2.37.orig.tar.xz.asc 833 SHA512:9849ba6aa9bff59499f67aceb69693c0331e7811fc74dea766a8e08f648ff09972449a540c3ea69bd70401464dd331f56ba29dbd00b6eeb27e9ceb42699089d8
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37-0ubuntu2.debian.tar.xz' glibc_2.37-0ubuntu2.debian.tar.xz 891980 SHA512:865a99eaef3cb3102eeb7cc990aeb59ec9857ef9e97f066f35433f6edcbf179b4d6424578d61717e66ffeb628bfb5d9bf6ac2e7ec9449b1cbbf3efc6085a2263
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

### `dpkg` source package: `gnutls28=3.7.9-2ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.9-2ubuntu1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.9-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.9-2ubuntu1.dsc' gnutls28_3.7.9-2ubuntu1.dsc 3530 SHA512:2d2d0fd27f5ae7627e02f615123e36e9e0fcc4161c622ef7d03e87aad9059bc03d243efa5ab1564bd4e06a236e94ef408d30e1ccbeff72dd25c64b4d812ec89b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.9.orig.tar.xz' gnutls28_3.7.9.orig.tar.xz 6377212 SHA512:56ccbab5f214f9e3cf10a43dd90dedc1e10a38d08b8359a4305dc05c59ddb4a1d3680b282077b6446605c31675a4261cd0579c2c0d976e0b2ced02e6dba224c1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.9.orig.tar.xz.asc' gnutls28_3.7.9.orig.tar.xz.asc 996 SHA512:448407f7696595964a59e848bb4924c005297a1aea1bbdba107a55d643981cae39eb6d44f2adf957390b78314a5d82a9a84d45cccfe95f0d716b0b66548de5dc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.9-2ubuntu1.debian.tar.xz' gnutls28_3.7.9-2ubuntu1.debian.tar.xz 88268 SHA512:28c99f2265479b32e842afd188ea15ae99594bd1e974561cfd4df0acd4c9481fad577946ebcda7b8d15563675ea60dd927d2ace179a7a4d329f04f23b216b95c
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

### `dpkg` source package: `krb5=1.20.1-2`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.20.1-2`
- `libk5crypto3:amd64=1.20.1-2`
- `libkrb5-3:amd64=1.20.1-2`
- `libkrb5support0:amd64=1.20.1-2`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-2.dsc' krb5_1.20.1-2.dsc 3168 SHA512:1379101f70b0a27e758ef6a6d5911a5615847c06197fd910bf13d8ddd90fa8764154372d61149b90dac0a4e63682ca73a97cb57a00eba6f9eb7edaf3f992786b
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz' krb5_1.20.1.orig.tar.gz 8661660 SHA512:6f57479f13f107cd84f30de5c758eb6b9fc59171329c13e5da6073b806755f8d163eb7bd84767ea861ad6458ea0c9eeb00ee044d3bcad01ef136e9888564b6a2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz.asc' krb5_1.20.1.orig.tar.gz.asc 833 SHA512:1d3312bd67581e07adfdadf2c5fe394179631d8add8bd075efefe982a0de22369004e60a14422d426382c8c591e4181b9897088afe9d4e86f0b5a97e5954c67a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-2.debian.tar.xz' krb5_1.20.1-2.debian.tar.xz 99520 SHA512:cc7084e95d0d3cba411f3873c8d9c3200500c624ed3cd34536c39a2668b82a9774ff31961c5a48d485075cb504e534695b6f27d4eda104cf04a2fc58aca19bec
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

### `dpkg` source package: `libbsd=0.11.7-4`

Binary Packages:

- `libbsd0:amd64=0.11.7-4`

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
- `Beerware`
- `Expat`
- `ISC`
- `ISC-Original`
- `libutil-David-Nugent`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.11.7-4
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.7-4.dsc' libbsd_0.11.7-4.dsc 2350 SHA512:9fc370950b1421a0ec801f1075fcf2d03d604f77a8f562c0e8647e0b68f821f9b6d0317b565f4db700fd1555aecdd6a3d66087b55e9a1944ffaea81de032a648
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz' libbsd_0.11.7.orig.tar.xz 418508 SHA512:51fda4724f41dd8a4628afd58c21236a7588d9045e337e06eeabf83805a9aaaa53705441ca901ad11f1c65f18e881523bdc97721a7d3d6a5cced27f2450d09a2
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz.asc' libbsd_0.11.7.orig.tar.xz.asc 833 SHA512:bdcce69ee261039900896c5be48659f1b6b809f3a6e8a5220aac30a6687926ac29e478a3ea737727d077d6575ee11b86eed896932568fdd261a9aaeb46d695b6
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.7-4.debian.tar.xz' libbsd_0.11.7-4.debian.tar.xz 21596 SHA512:24875c5a3b360ff1e2b0bb974e3b99f5bbd3b64a96f7948f94f2afc8c762d5e589fdfae2e81dc021bbc5cab6dbb63586c9cab9676067e4bd6afa5cd6b3612204
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

### `dpkg` source package: `libcbor=0.8.0-2ubuntu1`

Binary Packages:

- `libcbor0.8:amd64=0.8.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libcbor0.8/copyright`)

- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.8.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.8.0-2ubuntu1.dsc' libcbor_0.8.0-2ubuntu1.dsc 2196 SHA512:3dae3506bfaeee3e945c6a500be3f9f7a0de7f10f2924304dc933cc98c7b0f8be5618c14690f92d2c0d64e3c6f29eb5e8ba09185d82452a0d071e2355daff917
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.8.0.orig.tar.gz' libcbor_0.8.0.orig.tar.gz 267044 SHA512:694d2d3a78d80072f96e0afb73590ca1f3572e41d2117330ef4313ed06271743b048d3ba3259c6ffe9a802d5e441379d0e54787d1d42fed08dc81ac4f06c6dbc
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.8.0-2ubuntu1.debian.tar.xz' libcbor_0.8.0-2ubuntu1.debian.tar.xz 5472 SHA512:6c60981075bf118fd7a5df52cbc0d53be00abcc0257b97c3527409d37d400019787ed285d488938061ece9ac0423a936dc190c389ad7ae41a78bc573e6ceab4d
```

### `dpkg` source package: `libedit=3.1-20221030-2`

Binary Packages:

- `libedit2:amd64=3.1-20221030-2`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20221030-2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20221030-2.dsc' libedit_3.1-20221030-2.dsc 2281 SHA512:e3db9cccd742891543df891407449d207b14b392c1c1cc821c63fe3da51c9ecffe5954687e6ad088e6141f0b198be6716456c7370c7b5a49b7223654cf8669ae
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20221030.orig.tar.gz' libedit_3.1-20221030.orig.tar.gz 533261 SHA512:41eb46feaffa909e8790b9a9e304d5246e82ab366721196126a923d68b4d4964d0a433fe238f9d5e0a00aefb5c8cb66132150792929a793785ad091d91016f97
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20221030-2.debian.tar.xz' libedit_3.1-20221030-2.debian.tar.xz 16488 SHA512:ee07a5eda1c62e469a3d3680028c4d21892a7fc76c5259378a9218ae043120faa78df537d61cf1ee35dbbda3f94b093dae1d8143d8f5249ff9d5948faf82fb22
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-2.dsc' liberror-perl_0.17029-2.dsc 2085 SHA512:9b469f24ebdd65c5aacfa41b7099cb1fec5214d98e6e0d793d55a56bc0f0edae8f2ad3c0e09f44558249ff5456f05704c213d7e84661e0e4d774e644d3fd405a
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA512:266ba1feff897c1d162e69a83e595cb40da9a6e1d8b10cc5531626eff392c6da94be03ba722c74827fc2ea0d9d1c1e62e824d9021e098b700db65dd0b3acbd0a
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-2.debian.tar.xz' liberror-perl_0.17029-2.debian.tar.xz 4608 SHA512:beb596444319797a60470e98c14e8e736fd5be9c307ba5482fe96bf77c1382603b1f2a58d68406ecbf2bc5469cab4654645f5469cf059336fef24605b235cb61
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

### `dpkg` source package: `libfido2=1.13.0-1`

Binary Packages:

- `libfido2-1:amd64=1.13.0-1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.13.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.13.0-1.dsc' libfido2_1.13.0-1.dsc 2588 SHA512:403c7d2e80b175811bc40924e1c36175ea68ce166223596001e822ae7c3cd6364d0f1f01b3a1f08bdf486a99b5c5c91957baf58da8dc35ebaa8c05b024b64f8a
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.13.0.orig.tar.gz' libfido2_1.13.0.orig.tar.gz 652777 SHA512:90f8452cee4c9cc72241478e697c5c692ccff5ab27752f2f296c3623ee297d1f80a85a359b4d0656c67790084c116aac921894e762eb52d3a79056e5014c03e7
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.13.0.orig.tar.gz.asc' libfido2_1.13.0.orig.tar.gz.asc 228 SHA512:20e2c4ff34d3f4f605d7e73717f8e379e4124e675e9d3c9223e6053a2c80e0e615776f69efa0bc5cb15ed68ea3c5c9e2ec5567c9c183284fe005a071b31a8456
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.13.0-1.debian.tar.xz' libfido2_1.13.0-1.debian.tar.xz 52864 SHA512:589525b352e3c18387d27905f99efdc034746abb8d8f22a8579885baadcbd841a543284daa422526da2646f64a2c670dba3c70e3fcf08c30327c74a37fdae0cd
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

### `dpkg` source package: `libnsl=1.3.0-2build2`

Binary Packages:

- `libnsl2:amd64=1.3.0-2build2`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build2.dsc' libnsl_1.3.0-2build2.dsc 2087 SHA512:f13d28f34b0e71b04b5a0313b1cc79cdbe7d5e7f910d649af63b42824654e3cf01c02caa0e68309cb03350a17506e034800af1b1e3ab9af99fb64121c119215c
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA512:a5a6c3ccb2d1e724c8c1f65e55dcd09383eb1ae019c55f4c09441eadf23ffbc2196cfad259805b0ac40ddf3a10af0da453e4d739d67d46829c64d0995dab4e55
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build2.debian.tar.xz' libnsl_1.3.0-2build2.debian.tar.xz 4868 SHA512:367904106ba925eaa667cc273b37afd052ba795b7ed004cdb501c13dd26b469df971ac10acec2bf57d91fa4839f356c7dcbcd4969914891152588365844ced9a
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

### `dpkg` source package: `libselinux=3.4-1build4`

Binary Packages:

- `libselinux1:amd64=3.4-1build4`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.4-1build4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4-1build4.dsc' libselinux_3.4-1build4.dsc 2879 SHA512:d3fdfc5e7b5787313ec4eeeb399306cd965df5fffa84474ac4967c51fee002cf0bfab5696c8bea7bd88af678946275641ce995d9a8501d8df252b9555ad20e32
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz' libselinux_3.4.orig.tar.gz 210061 SHA512:7ffa6d2159d2333d836bde3f75dfc78a278283b66ae1e441c178371adb6f463aa6f2d62439079e2068d1135c39dd2b367b001d917c0bdc6871a73630919ef81e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz.asc' libselinux_3.4.orig.tar.gz.asc 833 SHA512:de1e0431cbf8526c4de77e1ebe9fa40111ea4a0e71d6b0e9ec6c975b61f4090ec5df4386af362bbd5cc8faffb24c21febc13356fe081df642bbfa52010a00ba0
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.4-1build4.debian.tar.xz' libselinux_3.4-1build4.debian.tar.xz 29604 SHA512:5f8f6b8b28878366a9fcee512036eab390363c887c1bc371e249b7f6dd043025f77280131bf94d2da9b72c65d974cc061571fc376c57ee253c55ff54b17a1003
```

### `dpkg` source package: `libsemanage=3.4-1build4`

Binary Packages:

- `libsemanage-common=3.4-1build4`
- `libsemanage2:amd64=3.4-1build4`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.4-1build4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.4-1build4.dsc' libsemanage_3.4-1build4.dsc 2915 SHA512:d4c905f87e9efc69f9259a59c6a0682d3e188ea2629f5a6f6e45b0479810425fa193e87a3656added2659e4490e33563c004c5170b8331f043a5f46ee1998b51
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz' libsemanage_3.4.orig.tar.gz 185177 SHA512:831dc789545bb9a0b009bdb4f7fe52f6197ad8325946640f886a960d08e40b8a69eccd5a70cce51466bb5cb7f742feb78d19a9ec63383fbd03aa451508677e73
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz.asc' libsemanage_3.4.orig.tar.gz.asc 833 SHA512:42da56fe008c7b18ea8834f6ae0535e78fb5f94a826a2beef6c8fbde480fd5d0f87a7969e98ded3281f7b76b594e71c466c7630a85536d07a6550d163390fc49
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.4-1build4.debian.tar.xz' libsemanage_3.4-1build4.debian.tar.xz 23428 SHA512:d0669897095913f19816c101320e8c73b0fa165e4b63688a962a6a7c88b34f07737b6895e0ac7419387bcc461a7c274f3aca4273f212763941b17381af11db08
```

### `dpkg` source package: `libsepol=3.4-2.1`

Binary Packages:

- `libsepol2:amd64=3.4-2.1`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.4-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4-2.1.dsc' libsepol_3.4-2.1.dsc 2334 SHA512:d63d2358601cdad17c3e87bd4327be8c5026a8793e6b12ec255166d0a70beeb3301d5df11a6a75d45b8549ac6825a99de87c9b96eda92747dc69c3b17b5f593f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz' libsepol_3.4.orig.tar.gz 490628 SHA512:5e47e6ac626f2bfc10a9f2f24c2e66c4d7f291ca778ebd81c7d565326e036e821d3eb92e5d7540517b1c715466232a7d7da895ab48811d037ad92d423ed934b6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz.asc' libsepol_3.4.orig.tar.gz.asc 833 SHA512:df3631f5f5b27e5893cfb14080089bd5a662d909257045c4b0cfe95e2abbb86d108f954248acd73121a65d9ab5fce771836e1aba4d3003c327ae9eecffefe791
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.4-2.1.debian.tar.xz' libsepol_3.4-2.1.debian.tar.xz 22040 SHA512:15bbbd0dc7bcf04f3f9a6a5ef0503d9c6180c94553579ed1532cdb172328c26d713992a90617dafa557100425572d055867da6691108549b59c58a9dfc6cbae8
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libtasn1-6/4.19.0-2/


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
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.dsc' libtirpc_1.3.3+ds-1.dsc 2129 SHA512:08672fa78293f89a5bc5ffcc5d191fe885b84e4bd0eae5829bd391621a2188f3a36e4e6bb5aa9c4b6a4bfb443687471eec82352d627ac32c448354fd168988ad
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds.orig.tar.gz' libtirpc_1.3.3+ds.orig.tar.gz 699030 SHA512:b32bef18da9763c04cb0d372472fea91ee88ec850d6cb3d8b398c67e47d93862a2f873f2e0a38dc5379d7d3887ac127dc4b43bddfc55403375a4cc839142a562
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.debian.tar.xz' libtirpc_1.3.3+ds-1.debian.tar.xz 11232 SHA512:fa7f5fd84993342230283de1dcd01db8f4aa61c1b100291b0ca09269c9d036d9f3c823986f8f6f0f492a2b24cc4522397e83c0f4e610b844845886e88c74e24e
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

### `dpkg` source package: `libxcrypt=1:4.4.35-1`

Binary Packages:

- `libcrypt1:amd64=1:4.4.35-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.35-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.35-1.dsc' libxcrypt_4.4.35-1.dsc 1591 SHA512:59efeac61b1b9b9ee71dca981b88ed623df0e6ff6c70acd4a0542ac78741da5bc4f40f1ec9feb47375b51a8e54c9abab2305f87b59f717eabceab35d71473c8a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.35.orig.tar.xz' libxcrypt_4.4.35.orig.tar.xz 393948 SHA512:bd58be6448057152b1bf5a7e8adbbecced16b4390ec4f6e2f845e048a305202f32519922f6f214acb85f3faa4b8a0b43938b2b63d63bf25165239b3a3cc8c632
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.35-1.debian.tar.xz' libxcrypt_4.4.35-1.debian.tar.xz 8204 SHA512:dcc5c072a716986541c774430aa38c3f8ba31ead00a45792f92c2bab24001cd42773bb861d9722bf53df57a0981ae4a5cfec4290b1c43a68f1db9c0552a59b6c
```

### `dpkg` source package: `libzstd=1.5.4+dfsg2-5`

Binary Packages:

- `libzstd1:amd64=1.5.4+dfsg2-5`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libzstd/1.5.4+dfsg2-5/


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

### `dpkg` source package: `mawk=1.3.4.20230525-1`

Binary Packages:

- `mawk=1.3.4.20230525-1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `GPL-2.0-only`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20230525-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20230525-1.dsc' mawk_1.3.4.20230525-1.dsc 1918 SHA512:395e31e96a38e80130fcd38d0d165d9a86d57ef3989d8a77fcbf944c160816ea1a2351df718b7c6ad7f09ecc612c07c3cc9603b70466db6367b51f85c4202ba8
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20230525.orig.tar.gz' mawk_1.3.4.20230525.orig.tar.gz 403222 SHA512:704c1a94569e8e953af7b00ea81efa20df03483f57e4183935e73df62309874644f2250a307b136af34ce3df62d90170d8afe7b3a86eeacb31cf5845056126cb
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20230525-1.debian.tar.xz' mawk_1.3.4.20230525-1.debian.tar.xz 14288 SHA512:bf68b5b7aec6c1a9257cf4071b6541f799f2f68c1bd6967e146fced2cc579a6c939014dc39a12bc71d70f84df109101e0e790b32f760d3eb894b37c991753f24
```

### `dpkg` source package: `media-types=10.0.0`

Binary Packages:

- `media-types=10.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=10.0.0
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_10.0.0.dsc' media-types_10.0.0.dsc 1624 SHA512:c7de78d6604f2ea1cd1abeed0f7396f9972af4ea9332fb5f281c1c4b5f4af9df9f6f67a6ab36679095e7f64451e2d36fe82f45690babce13fc61066d55e541ca
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_10.0.0.tar.xz' media-types_10.0.0.tar.xz 57912 SHA512:c8c74ea620b71c6608d2d56f1cd9bc07baa7a2646d81ce4032572613d6e44119747adedc15243dfe2444b1b0fc0caa1b03499252a9c36c2514def4783e3de8d5
```

### `dpkg` source package: `mercurial=6.3.2-1`

Binary Packages:

- `mercurial=6.3.2-1`
- `mercurial-common=6.3.2-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=6.3.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.3.2-1.dsc' mercurial_6.3.2-1.dsc 2848 SHA512:ec64fdcb51a719debce8dac1d0c932cc2061c0ad73112f3c54d2566ccb86a9c771d7cd6c05902454e9c09307e768cc7c5b6f4854308abc9c67255e41274626d6
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.3.2.orig.tar.gz' mercurial_6.3.2.orig.tar.gz 8092710 SHA512:5ca7e448bf336c2a2d4db174c4f486f66f41eef33db14f152abb09b8d82416124d251784cb5898499580083ca104113d0763e27baa9b77feb90ba2fd96d40be5
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.3.2.orig.tar.gz.asc' mercurial_6.3.2.orig.tar.gz.asc 659 SHA512:7a05f805afc256878187afc9679c03e9cdefc4d3adb47420684010f35045c507e4bd0bf78960121e28d51b9525b37fc661045e9c9dbed77a15d0aa2f656aaa72
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.3.2-1.debian.tar.xz' mercurial_6.3.2-1.debian.tar.xz 90164 SHA512:99e49af80ad0d22a6d7b09d468dc881af27c18e7732391243d2cb3a994178ac4a3adf9cd59b6cf5b5d8a9ea587ef065940502c10f1c4f461d08f05b09e6ca466
```

### `dpkg` source package: `ncurses=6.4-4`

Binary Packages:

- `libncursesw6:amd64=6.4-4`
- `libtinfo6:amd64=6.4-4`
- `ncurses-base=6.4-4`
- `ncurses-bin=6.4-4`

Licenses: (parsed from: `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ncurses/6.4-4/


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

### `dpkg` source package: `nghttp2=1.54.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.54.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `all-permissive`

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.54.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.54.0-1.dsc' nghttp2_1.54.0-1.dsc 2534 SHA512:376a1cc0eb61c2a3d2ce773fbb95da6a15125d0fd2f573c96de7a1173ad9832c3f274f39c26a30692acbe993d86020a3177e28d79dcff9afd97a0ac5a2553693
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.54.0.orig.tar.gz' nghttp2_1.54.0.orig.tar.gz 1069605 SHA512:0ec50178068276cde624c47a634beda0b96ef1529970fddb20cf7a9b4b30d792827ffe16f16f5b7e210d0b7913be5d25e6c6704f6f7fb9a1b5a85f63aeaba6bc
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.54.0-1.debian.tar.xz' nghttp2_1.54.0-1.debian.tar.xz 11684 SHA512:b857d34974b1887fc470754afb166d977e7cbaf2e6bbddd6379738a13cb9958f113917ee7011f6a346ff2871acf2e395f6f32e59bcf656e72d6eb0393c87e878
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

### `dpkg` source package: `openldap=2.6.4+dfsg-1~exp1ubuntu1`

Binary Packages:

- `libldap2:amd64=2.6.4+dfsg-1~exp1ubuntu1`

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
$ apt-get source -qq --print-uris openldap=2.6.4+dfsg-1~exp1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.4%2bdfsg-1%7eexp1ubuntu1.dsc' openldap_2.6.4+dfsg-1~exp1ubuntu1.dsc 3470 SHA512:1559fd9adaf85e1eab3d7f413beb47165ed6353a52322157256aad4ff0cab4a924ef034c0909c346d38a0f03f7e4edfc9b40239f55fa4301acce651e156b5938
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.4%2bdfsg.orig.tar.xz' openldap_2.6.4+dfsg.orig.tar.xz 3744892 SHA512:e0c000b4fabe64ff5cbd07eae11a62e048bf53c1a649356616c19c3a08ec37e2d6639663ede57e388b633168aee704c9d64470d17fa32f64988c68a73a82d2ab
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.4%2bdfsg-1%7eexp1ubuntu1.debian.tar.xz' openldap_2.6.4+dfsg-1~exp1ubuntu1.debian.tar.xz 179552 SHA512:5c4b2651c41a8ece042a6704a44cc3fe4f1f6e9752bb7baea8488377c4bb9b8e7e0a32c9fb0be32af98e0924c363e0569d14262984b8c374cd02e2776bf627e5
```

### `dpkg` source package: `openssh=1:9.2p1-2ubuntu3`

Binary Packages:

- `openssh-client=1:9.2p1-2ubuntu3`

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
$ apt-get source -qq --print-uris openssh=1:9.2p1-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.2p1-2ubuntu3.dsc' openssh_9.2p1-2ubuntu3.dsc 3313 SHA512:2ec80a9f6c7c30d7c62e2c9cea240d5d5c3bd7606101599fa8e4ac5e95346efb684f65095112bae043b4c1e1a9065cb34ed10ab7c7ddbabf21fe7ffc75488c07
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.2p1.orig.tar.gz' openssh_9.2p1.orig.tar.gz 1852380 SHA512:c4b79ef3a05b96bfc477ffb31f734635bffd5be213ab58e043111c3232dbe999ff24665fa1069518237cffa5126ded0dda8984e1b8f098f4f09b8c1dae20e604
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.2p1.orig.tar.gz.asc' openssh_9.2p1.orig.tar.gz.asc 833 SHA512:2a56f8946ed00fcd5a92935e090523d40b5c3747e25661d575b799b1825bf5e47a95eed5e7ed968fe042349c2c7d94d6b0e6bf2d9145b5c6ff5df2ca538d56e5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.2p1-2ubuntu3.debian.tar.xz' openssh_9.2p1-2ubuntu3.debian.tar.xz 187764 SHA512:b35256b7bf867667bc416cfb6f1c76f0eb947bd263f3d91eba1d3794a658653b123ac95a9113cba7c62dc498eec92050ad4e391f2419c5373bdcfd35654bd27e
```

### `dpkg` source package: `openssl=3.0.9-1ubuntu1`

Binary Packages:

- `libssl3:amd64=3.0.9-1ubuntu1`
- `openssl=3.0.9-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.9-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.9-1ubuntu1.dsc' openssl_3.0.9-1ubuntu1.dsc 2718 SHA512:6082a7124673136a4128a446a3ce4bec54a0415700f3624e016cf2b81e069a895ff53befe26e2635671b177187e23e76bd679a8758f9add9b9aa47780317c24c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.9.orig.tar.gz' openssl_3.0.9.orig.tar.gz 15181285 SHA512:86c99146b37236419b110db77dd3ac3992e6bed78c258f0cc3434ca233460b4e17c0ac81d7058547fe9cb72a9fd80ee56d4b4916bb731dbe2bbcf1c3d46bf31a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.9.orig.tar.gz.asc' openssl_3.0.9.orig.tar.gz.asc 833 SHA512:9949de6b57d5aa21da1d4b68a29eb37e302403c983bd7d2d8769b320aac4268a9f9091c5fb182862a4f89a9099660939fe609df87c66991b75f7695faf357caf
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.9-1ubuntu1.debian.tar.xz' openssl_3.0.9-1ubuntu1.debian.tar.xz 106836 SHA512:03ee2e5ebc713524123485c514ef1cca409bd118ef00c191fcd122b52265af184e1b98b7210c6f0ee66ed0dde84f5daa09d179b36996150a8db466ef7b155261
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

### `dpkg` source package: `perl=5.36.0-7ubuntu1`

Binary Packages:

- `libperl5.36:amd64=5.36.0-7ubuntu1`
- `perl=5.36.0-7ubuntu1`
- `perl-base=5.36.0-7ubuntu1`
- `perl-modules-5.36=5.36.0-7ubuntu1`

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
$ apt-get source -qq --print-uris perl=5.36.0-7ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-7ubuntu1.dsc' perl_5.36.0-7ubuntu1.dsc 2968 SHA512:74c9b60640c71820ef6654e6a4439220dddc4ce1c4fcf04e470395e189d1ea66a47cbfc5ff2a9dcb9cd288b629b5afa4cc0cbf0f2f3eb2950ef175d39535647c
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig-regen-configure.tar.xz' perl_5.36.0.orig-regen-configure.tar.xz 417784 SHA512:4d16685f569a5b1dea79d607b6d62718111c32efaf5547bb9e1528bd755acf0c8fc74a1cc1f4d68fcb10aef9da7d8fea17a5cc10dabce6efa4721ab45ab03a65
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig.tar.xz' perl_5.36.0.orig.tar.xz 13051500 SHA512:6dd6ac2a77566c173c5ab9c238cf555f2c3e592e89abb5600bc23ce1cbd0c349e0233f6417cbbf1f6d0aefc6a734ba491285af0d3dc68a605b658b65c89f1dab
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-7ubuntu1.debian.tar.xz' perl_5.36.0-7ubuntu1.debian.tar.xz 169744 SHA512:7859f20b2d168d3fb77f8aec0223548f6616c1954f443296fb711680063d188a3534374541e93dafc4212583453edb8d4668420839156a582f16a8dc3dc33c16
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

### `dpkg` source package: `procps=2:4.0.3-1ubuntu1`

Binary Packages:

- `libproc2-0:amd64=2:4.0.3-1ubuntu1`
- `procps=2:4.0.3-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libproc2-0/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:4.0.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_4.0.3-1ubuntu1.dsc' procps_4.0.3-1ubuntu1.dsc 2215 SHA512:92d9fa524b872bb2ebb5b23a8b449a8b09168a31cb34d27ecad328cbad72afde0d8d3e93c6f97df1056ce686f24b73fb0e2bc8eaa5572c4adb2f15ea64dbc9be
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_4.0.3.orig.tar.xz' procps_4.0.3.orig.tar.xz 1294992 SHA512:be9dc5ac4a50fc1b8256af44ac2c5b50f74ef5e48c5c3dcac2779d508988daf3b60989d22db8fc8b699c2f2f338ad367e91b9c01ab46ac9fa0d5c5bbec6f16af
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_4.0.3-1ubuntu1.debian.tar.xz' procps_4.0.3-1ubuntu1.debian.tar.xz 33148 SHA512:efd9dd3ff8ef41c620f7ea4615b3d1d0539dfff7c18f82fc13f21cc74901c8c5b0e35a49344b5bd9f9014ac1ac4dbab889d6b406d801fe7a3b5e1d5aa64999ef
```

### `dpkg` source package: `python3-defaults=3.11.4-1`

Binary Packages:

- `libpython3-stdlib:amd64=3.11.4-1`
- `python3=3.11.4-1`
- `python3-minimal=3.11.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.11.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.11.4-1.dsc' python3-defaults_3.11.4-1.dsc 2961 SHA512:fd27fbd7fc978ea15c263e5a1311560eb13420272903fbf9c5cf4dc0be009871e45518969ca02008d4acf544df2fa3f02a857bd2361288edd3e2bb01d333dc57
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.11.4-1.tar.gz' python3-defaults_3.11.4-1.tar.gz 146142 SHA512:d0cc77aa8ca2e4b74248d7dd072ef4bfadd73235aca0d86478abc276279ae5238aa812ce020f766ac3616da97501a8c3e36519738edfe2459a0ebdb1610b8538
```

### `dpkg` source package: `python3.11=3.11.4-1`

Binary Packages:

- `libpython3.11-minimal:amd64=3.11.4-1`
- `libpython3.11-stdlib:amd64=3.11.4-1`
- `python3.11=3.11.4-1`
- `python3.11-minimal=3.11.4-1`

Licenses: (parsed from: `/usr/share/doc/libpython3.11-minimal/copyright`, `/usr/share/doc/libpython3.11-stdlib/copyright`, `/usr/share/doc/python3.11/copyright`, `/usr/share/doc/python3.11-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.11=3.11.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.11/python3.11_3.11.4-1.dsc' python3.11_3.11.4-1.dsc 3636 SHA512:bad6b7c9dde81054de539371a7c767053f7158ab0a60cb84c0675fc05d9a44410489f18a7cab7ca0d30f343c0f186fbfd20ae1b3edf5a9a306bddae8e95ad37f
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.11/python3.11_3.11.4.orig.tar.xz' python3.11_3.11.4.orig.tar.xz 19954828 SHA512:7eb14fecbf60824d10c22a9057584c3a142c2866f4af6caa2525c10c8bcb24e6e7afb32a44a0e118df0a2b2543d578c3b422ffd4a5fa317dfe6ea371cc7ee1ee
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.11/python3.11_3.11.4-1.debian.tar.xz' python3.11_3.11.4-1.debian.tar.xz 213228 SHA512:e85e44a4f222f574edc10902c840cb1d51824866de6a01ce159fc5e2dac7d536ae3d504ba1513646a70eacfe6a5b1fdd2efc19b4b665ad0a099edaa7f6a5c24c
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

### `dpkg` source package: `rust-sequoia-sq=0.27.0-2`

Binary Packages:

- `sq=0.27.0-2`

Licenses: (parsed from: `/usr/share/doc/sq/copyright`)

- `GPL-2`
- `GPL-2.0-or-later`

Source:

```console
$ apt-get source -qq --print-uris rust-sequoia-sq=0.27.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/r/rust-sequoia-sq/rust-sequoia-sq_0.27.0-2.dsc' rust-sequoia-sq_0.27.0-2.dsc 3088 SHA512:f4fda21e5762ea50b8711ad9d4eee47fa5cdafa658e31a492d149594a767548a4ae5ab5f182be116adc10f49d1f5449d89fae52aba9fb5331de43c94d732d625
'http://archive.ubuntu.com/ubuntu/pool/universe/r/rust-sequoia-sq/rust-sequoia-sq_0.27.0.orig.tar.gz' rust-sequoia-sq_0.27.0.orig.tar.gz 196791 SHA512:af86f5f4d868b970bfe9d027415fb7eda4a03963603bab2987f82b7a31decaec87b64578e9d6d6ce7bbffcb4563824aca715f58b28aaf92925ed2584dcb2f5ba
'http://archive.ubuntu.com/ubuntu/pool/universe/r/rust-sequoia-sq/rust-sequoia-sq_0.27.0-2.debian.tar.xz' rust-sequoia-sq_0.27.0-2.debian.tar.xz 5916 SHA512:5d8826cce1590d95f6620f7eb1c65301e59b8d73774f84fa19928f256f745fa2b609c9785e9b7eb23078863167104f2d03f84060e600f69df5df745928ba7231
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

### `dpkg` source package: `serf=1.3.10-1`

Binary Packages:

- `libserf-1-1:amd64=1.3.10-1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.10-1/


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

### `dpkg` source package: `sqlite3=3.40.1-2`

Binary Packages:

- `libsqlite3-0:amd64=3.40.1-2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.40.1-2/


### `dpkg` source package: `subversion=1.14.2-4build2`

Binary Packages:

- `libsvn1:amd64=1.14.2-4build2`
- `subversion=1.14.2-4build2`

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
$ apt-get source -qq --print-uris subversion=1.14.2-4build2
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.2-4build2.dsc' subversion_1.14.2-4build2.dsc 3794 SHA512:0c084fb20294ec402830537c4d6ee351ae0bae362a8380d1d4aeaf128859528eb83cb9fc543240a53222c35d4fbdb27426a0d1fe90256cb7d9f09ad36e9b7908
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.2.orig.tar.gz' subversion_1.14.2.orig.tar.gz 11626792 SHA512:053d9d38f675f5ddd6ad9c6bd061482f5e9ec9f0cb8ea6db76a91e0646af26dfdab2a882d09395df4e073d704be909160c230251957f86a452d32408da6d7468
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.2.orig.tar.gz.asc' subversion_1.14.2.orig.tar.gz.asc 3215 SHA512:e0bdc9fff6ec6a645005da9031e96c7ad5cc97b9fbac21b91be6efe91adc72d85bd4ad630b5ca28e9cf619b95ea6f6421033e2d4669473faf9ec0406fd2ed6b6
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.2-4build2.debian.tar.xz' subversion_1.14.2-4build2.debian.tar.xz 337324 SHA512:53c2d0312401cfb1a1704799b607a819c8f1a1c8a177d352e138118a7bbcd0545d84580898dcdbb64395a8482e49d9ca8604af1c1839f0029166453c7c74e790
```

### `dpkg` source package: `systemd=252.5-2ubuntu3`

Binary Packages:

- `libsystemd0:amd64=252.5-2ubuntu3`
- `libudev1:amd64=252.5-2ubuntu3`

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
$ apt-get source -qq --print-uris systemd=252.5-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_252.5-2ubuntu3.dsc' systemd_252.5-2ubuntu3.dsc 6750 SHA512:8b95149167ae826674dc151231fe4e2a06374552e96778f5629e2888378c29fb9e973e6ca88988b7ea19001a0ee5ae6f248967dd2741db860e2aa4cd79d73db7
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_252.5.orig.tar.gz' systemd_252.5.orig.tar.gz 11762414 SHA512:f3359e0496b673033d6c8da5c117890e0dc26c9db51003b28f629ac751d9bae117be32d9f54c377eb2d5a7c2d36ac0dbdc2116498698e993550fbdd9aae535b9
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_252.5-2ubuntu3.debian.tar.xz' systemd_252.5-2ubuntu3.debian.tar.xz 230516 SHA512:0e2e33dc91f091ad9881c51585bfb49980580160d892a89162f58b5bf0aa52390cb6f2c04805be8075a99a5cc876c477d4a081c931a4ad6aaff508a41c945602
```

### `dpkg` source package: `sysvinit=3.06-4ubuntu1`

Binary Packages:

- `sysvinit-utils=3.06-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.06-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.06-4ubuntu1.dsc' sysvinit_3.06-4ubuntu1.dsc 2466 SHA512:5d6f20233ff423790a8d64b4290dd5b7804ade6902898166ff006241622a4dc6e94cf396ae8e94c5b7ee9cfea35c565216d7c55a83ed2f73b385374102b4ba08
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.06.orig.tar.gz' sysvinit_3.06.orig.tar.gz 466092 SHA512:9f1111ea05cbb405e3fe2423ee2d281832f3d15a69e39c5c6896e1ee7c0d56369046d39d7a2203f66db05304836dd33f1664652726cadf8a29cb0eea27ce822f
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.06-4ubuntu1.debian.tar.xz' sysvinit_3.06-4ubuntu1.debian.tar.xz 135992 SHA512:7c4d7d742ad5febe27bcf946d0afaef2dd8a0d0711f7f463f4161f87a6b9e7e493815cb92056d22118113275641afdcf39cd42fc5408a0c9ee814502f9f00b52
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

### `dpkg` source package: `tzdata=2023c-4exp1ubuntu1`

Binary Packages:

- `tzdata=2023c-4exp1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `ucf=3.0043+nmu1`

Binary Packages:

- `ucf=3.0043+nmu1`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0043+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043%2bnmu1.dsc' ucf_3.0043+nmu1.dsc 1567 SHA512:608423c255fa2c1072bcaa9c71addd0f393f008ebd321ef4939ed4d714aa43bea4c90979fa5817c19e3d7355415cc70aa8c80ff79760b4286411cfbd58242d77
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043%2bnmu1.tar.xz' ucf_3.0043+nmu1.tar.xz 70916 SHA512:8949f197f6aec35ef7ff8c076ed9f863ef369c65de1a17947445c7182623393633e0094e882d50eadbb0435bf03b9a5cb5d11b6e3bd40e33d5d7b15425583b38
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

### `dpkg` source package: `utf8proc=2.8.0-1`

Binary Packages:

- `libutf8proc2:amd64=2.8.0-1`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.8.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.8.0-1.dsc' utf8proc_2.8.0-1.dsc 2187 SHA512:2d63ce20fa889f6825fcc43a7ea97f4564e1a08299208cf23c630ff55b773174a03e593cbd3ffa81e7ca3fb66e4bab2772588e24f5db024ae7c06eb51621b2c0
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.8.0.orig.tar.gz' utf8proc_2.8.0.orig.tar.gz 190310 SHA512:4b9853fc95db38bee1d7435bef219907e25b249e0c2ec26f7096b8506ab2a139a8d4b71f7133b7550bff59d8f997fe01c2957d362cad18d890ad82bcf158aa06
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.8.0-1.debian.tar.xz' utf8proc_2.8.0-1.debian.tar.xz 5720 SHA512:5cc254a57269479d844d484071fad0b3c4b0a13e5f144656a1c303af667837bee88379d78a8f353c793271d254dc0369c01c557782729753e749d916e8a37669
```

### `dpkg` source package: `util-linux=2.38.1-5ubuntu2`

Binary Packages:

- `bsdutils=1:2.38.1-5ubuntu2`
- `libblkid1:amd64=2.38.1-5ubuntu2`
- `libmount1:amd64=2.38.1-5ubuntu2`
- `libsmartcols1:amd64=2.38.1-5ubuntu2`
- `libuuid1:amd64=2.38.1-5ubuntu2`
- `mount=2.38.1-5ubuntu2`
- `util-linux=2.38.1-5ubuntu2`
- `util-linux-extra=2.38.1-5ubuntu2`

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
$ apt-get source -qq --print-uris util-linux=2.38.1-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38.1-5ubuntu2.dsc' util-linux_2.38.1-5ubuntu2.dsc 4632 SHA512:9df06f35022bedfde4fb8244d76e365565ccb5e5fdb41f393a37b279d6440417ece4745a30d3eaca413bb92041b24a4ec4904875be711803474f7ceae57cb3b3
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38.1.orig.tar.xz' util-linux_2.38.1.orig.tar.xz 7495904 SHA512:07f11147f67dfc6c8bc766dfc83266054e6ede776feada0566b447d13276b6882ee85c6fe53e8d94a17c03332106fc0549deca3cf5f2e92dda554e9bc0551957
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38.1-5ubuntu2.debian.tar.xz' util-linux_2.38.1-5ubuntu2.debian.tar.xz 118828 SHA512:7f9ebca69800999a22cb107168ce18c816d70562cccbc725109f90b6b381bd4c6f69afde2d4fe5019beec4fbfaeeaab2613307c850806ff49ed033540ef90567
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
