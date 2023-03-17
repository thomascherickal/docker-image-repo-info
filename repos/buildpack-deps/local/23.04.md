# `buildpack-deps:lunar`

## Docker Metadata

- Image ID: `sha256:c81d6e1c88be1ef8bc7e4711555c9bc2801e4ae6d1ba36047cc5ccfc957d722a`
- Created: `2023-03-16T05:40:10.361198073Z`
- Virtual Size: ~ 783.99 Mb  
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

### `dpkg` source package: `aom=3.6.0-1`

Binary Packages:

- `libaom3:amd64=3.6.0-1`

Licenses: (parsed from: `/usr/share/doc/libaom3/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `ISC`
- `public-domain-md5`

Source:

```console
$ apt-get source -qq --print-uris aom=3.6.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_3.6.0-1.dsc' aom_3.6.0-1.dsc 2207 SHA512:7af3deb8f6ec9e6e18d1789cb3630ef9c762995673c45620d5d0cb4ea69fc1f8f77cc4659551838bd058e5cf66ef8d7f8e61ed354946cc92edbe499aa1967789
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_3.6.0.orig.tar.gz' aom_3.6.0.orig.tar.gz 5268170 SHA512:2b9984e3c9756aacea04c962cb4ba3e6c71580c0ce2bd629303d7fe5a1fbc3e51696f831781273ee9f33eefa493c2fd7cf47601aa9098884649c337d52f96526
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_3.6.0-1.debian.tar.xz' aom_3.6.0-1.debian.tar.xz 18348 SHA512:a21a36828cdf61d7f8427541e5080bdcaf95b46cfc03eaa609e2eb8c65bcc639e4e84d30a7d5a52370280db4e3cacd415fec30e48354781e467d4b1c4287e1c3
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

### `dpkg` source package: `apr=1.7.2-2`

Binary Packages:

- `libapr1:amd64=1.7.2-2`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2-2.dsc' apr_1.7.2-2.dsc 2262 SHA512:68d6cf0eefe6ef20fea4b1453a5cebfa2ad34d622bb3dcd3dfa761599a8276d70e917ca64d67de4bd9808b70da049cded13f667e646475e50a62258ea0b264db
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2.orig.tar.bz2' apr_1.7.2.orig.tar.bz2 890218 SHA512:0a3a27ccc97bbe4865c1bc0b803012e3da6d5b1f17d4fb0da6f5f58eec01f6d2ae1f25e52896ea5f9c5ac04c5fddcfd1ac606b301c322cf40d5c4d4ce0a1b76e
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2.orig.tar.bz2.asc' apr_1.7.2.orig.tar.bz2.asc 833 SHA512:77da1e516b30032419b36da8453f56c6149ad18631772613adb095b6eccb7606dc51589d33d422572d3fcefe8f6129bfbb06d0ab7fde5848d873856f4ed93940
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.2-2.debian.tar.xz' apr_1.7.2-2.debian.tar.xz 53316 SHA512:abdb0623e45f77bae34a2ffba0cbefb46ad5b283a992e846d1800d22c2d183b3a2433ebb1366aa5eb2dd6356619cf4339da9409fde4ab6ce614a9d13bb71ccf3
```

### `dpkg` source package: `apt=2.6.0`

Binary Packages:

- `apt=2.6.0`
- `libapt-pkg6.0:amd64=2.6.0`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.6.0
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.6.0.dsc' apt_2.6.0.dsc 2933 SHA512:d511ab6fd46ebf49ce2958611e9bfcad0568680555e8973a397671b67e376fada0344118e0d3cb0df6d5d70207db9758169e9b2bf29cbc108a6221037397ddd3
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.6.0.tar.xz' apt_2.6.0.tar.xz 2328252 SHA512:44e35e6773f63bbfee8b5b2c405ffef218226d2af14f45a552eeefca1aea2192052c49a1c4d25a492e7222f243bec9301fcaec2f4cb530e7563791b5a30a749f
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

### `dpkg` source package: `autoconf=2.71-3`

Binary Packages:

- `autoconf=2.71-3`

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
$ apt-get source -qq --print-uris autoconf=2.71-3
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.71-3.dsc' autoconf_2.71-3.dsc 1988 SHA512:77b5211bc883080da398a9b16ea5455b6e1562c4be7459844b58a61bcf57183bf6440547ef3bcc55b4ece3213347aaaa12dbf1603d5528d037cfb956413e29f6
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.71.orig.tar.gz' autoconf_2.71.orig.tar.gz 2003781 SHA512:2bc5331f9807da8754b2ee623a30299cc0d103d6f98068a4c22263aab67ff148b7ad3a1646bd274e604bc08a8ef0ac2601e6422e641ad0cfab2222d60a58c5a8
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.71-3.debian.tar.xz' autoconf_2.71-3.debian.tar.xz 23896 SHA512:12debf9cd25329130b7d9b00b77bbbfb7f3f26cdf6dbe60188203e3a66ed933f693de02c3816856e4157d5843647d7c834c3bd924345a7ac41ad35aac3689f63
```

### `dpkg` source package: `automake-1.16=1:1.16.5-1.3`

Binary Packages:

- `automake=1:1.16.5-1.3`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.5-1.3
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.3.dsc' automake-1.16_1.16.5-1.3.dsc 1973 SHA512:911924e07fb9951025d95d0827f431a63e78d55c95eafa8c61c2248bff6880a5902ac1be2ff4f104308bfe853b7cf4c4cdb860faa1fd7feb0f1a0912f0e4f330
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz' automake-1.16_1.16.5.orig.tar.xz 1601740 SHA512:3084ae543aa3fb5a05104ffb2e66cfa9a53080f2343c44809707fd648516869511500dba50dae67ff10f92a1bf3b5a92b2a0fa01cda30adb69b9da03994d9d88
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz.asc' automake-1.16_1.16.5.orig.tar.xz.asc 833 SHA512:032a7c39abb4cabbefa4eb9c15263baec0902e48c0c81364307361a41fd55be282b9640707c789f5ae572e8e60240e34d1b575a671b5710f5d2a5716fafc2d51
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.3.debian.tar.xz' automake-1.16_1.16.5-1.3.debian.tar.xz 14164 SHA512:ca023f45d90ec57db7819688ae457c162ca4429b360bae8dacd6b8b5087a0da51956fd931f23573d7dd47f26422f702a70b219caa55bf76d395417b97af7d5de
```

### `dpkg` source package: `autotools-dev=20220109.1`

Binary Packages:

- `autotools-dev=20220109.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20220109.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20220109.1.dsc' autotools-dev_20220109.1.dsc 1661 SHA512:aca60be8ed006832005e58bf176f8c7e8abe85986dbcc6d15d8b5c092c89322a132601784ef1f977d7e071c8b033debcef7c3cb5712765be00c2d298d9812d71
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20220109.1.tar.xz' autotools-dev_20220109.1.tar.xz 87340 SHA512:5427cc6897685355018db547ec39fd6bcc0ecbd73ba25869fb841f3503c1753af9a323d963a2b3150ef40ff07486f39377acdec878b2c054c1fa51de9afe01bb
```

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

### `dpkg` source package: `binutils=2.40-2ubuntu3`

Binary Packages:

- `binutils=2.40-2ubuntu3`
- `binutils-common:amd64=2.40-2ubuntu3`
- `binutils-x86-64-linux-gnu=2.40-2ubuntu3`
- `libbinutils:amd64=2.40-2ubuntu3`
- `libctf-nobfd0:amd64=2.40-2ubuntu3`
- `libctf0:amd64=2.40-2ubuntu3`
- `libgprofng0:amd64=2.40-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`, `/usr/share/doc/libgprofng0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.40-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.40-2ubuntu3.dsc' binutils_2.40-2ubuntu3.dsc 9183 SHA512:8b2884c78b387e91edd58a9ddb35cd6b9c2aa473971e24d97e2d203e156406f33411ce8ab2d4de3aac38460d78b008a304aaac3c9a1fc6258a1d45dbb5d59a21
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.40.orig.tar.xz' binutils_2.40.orig.tar.xz 25241484 SHA512:a37e042523bc46494d99d5637c3f3d8f9956d9477b748b3b1f6d7dfbb8d968ed52c932e88a4e946c6f77b8f48f1e1b360ca54c3d298f17193f3b4963472f6925
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.40-2ubuntu3.debian.tar.xz' binutils_2.40-2ubuntu3.debian.tar.xz 337640 SHA512:7ea829635aa9b3ffd3e1749094207767f669a5b29716c335d3676299575296e8c35b0460e85b4034e5c1cd7170623f3195580df330e3259bfc29c274aeddf7dc
```

### `dpkg` source package: `brotli=1.0.9-2build8`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2build8`
- `libbrotli1:amd64=1.0.9-2build8`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

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

- `bzip2=1.0.8-5build1`
- `libbz2-1.0:amd64=1.0.8-5build1`
- `libbz2-dev:amd64=1.0.8-5build1`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `cairo=1.16.0-7`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-7`
- `libcairo-script-interpreter2:amd64=1.16.0-7`
- `libcairo2:amd64=1.16.0-7`
- `libcairo2-dev:amd64=1.16.0-7`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-7
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-7.dsc' cairo_1.16.0-7.dsc 2823 SHA512:f70441caf095f1c012046222af2564ce7e1e57436849323935e5f533c09a83d1c12e963c57db4d007a77e39d7462fdfbcb23a4a2df2d7a631d2607e500804579
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA512:9eb27c4cf01c0b8b56f2e15e651f6d4e52c99d0005875546405b64f1132aed12fbf84727273f493d84056a13105e065009d89e94a8bfaf2be2649e232b82377f
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-7.debian.tar.xz' cairo_1.16.0-7.debian.tar.xz 33816 SHA512:ab54fe20d5bbb7d03685087bb62a55a825d1a1e65572ae657f28e04d5ecbb2f2677d094d65ec4731db0ddb9e74c911a7efbfad3208f0dace3747f47835eb0011
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

### `dpkg` source package: `curl=7.88.1-1ubuntu1`

Binary Packages:

- `curl=7.88.1-1ubuntu1`
- `libcurl3-gnutls:amd64=7.88.1-1ubuntu1`
- `libcurl4:amd64=7.88.1-1ubuntu1`
- `libcurl4-openssl-dev:amd64=7.88.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

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
$ apt-get source -qq --print-uris curl=7.88.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1-1ubuntu1.dsc' curl_7.88.1-1ubuntu1.dsc 3070 SHA512:c75672f7752297bedde5c47d795d3518db43e1b037f2456f40aab2f61fd58394206daf929e512cac113fc963743fc81476d762a86e7cdb679df27e69373156ec
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1.orig.tar.gz' curl_7.88.1.orig.tar.gz 4343562 SHA512:67701d458548712bbfaa55f2ebefbf87cdbba01b7b1200f608b1c3af67e8dd8e243fa89f256446d217d658a5a1242331d8b0168ab600351e74ee0e2511e79dae
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1.orig.tar.gz.asc' curl_7.88.1.orig.tar.gz.asc 488 SHA512:90029e6304d7ece487594d9192101084e3b0419c9e4296a76b9d32f44d2fb98753ddc6b0b50c2ffc16ab3b04222af607ca4c813d2c01bf1fd1b670d4d7e39404
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.88.1-1ubuntu1.debian.tar.xz' curl_7.88.1-1ubuntu1.debian.tar.xz 40028 SHA512:533163b91ad1d1dc117b666f408d024e9d01fa02c8133c6fd2149475b3012e220cbd49fe12f691345974af0cd986322cc03c0d84ece3a9ae6b5efade1f8487c3
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

### `dpkg` source package: `dav1d=1.0.0-2`

Binary Packages:

- `libdav1d6:amd64=1.0.0-2`

Licenses: (parsed from: `/usr/share/doc/libdav1d6/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dav1d=1.0.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.0.0-2.dsc' dav1d_1.0.0-2.dsc 2307 SHA512:efa7b15915e429cdd78f10e867df381f8e080a4cc4d6e97d33b737aac17f682525e64b03ea15fa00c708950710d00b9b55ff5449a0bd7f167fb0c8e5796dd53c
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.0.0.orig.tar.xz' dav1d_1.0.0.orig.tar.xz 810116 SHA512:a3a7e162e45181449cd42af3a4d36669a850a4ee9ab17641dcd63d84406444566e8ebc7caa55b0620ab581039f36d19a90218a40f52ebbe525b37ed9493fb3f3
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.0.0.orig.tar.xz.asc' dav1d_1.0.0.orig.tar.xz.asc 195 SHA512:55976d877714ec96b75d0de7b8a2d1c1427193946d7a744e1fa1d6f0a5d47fb87dc176e47f5c988a1855cd84eddfbec9eddb620dfa139fd563964e472320e3de
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.0.0-2.debian.tar.xz' dav1d_1.0.0-2.debian.tar.xz 7980 SHA512:72c46eeb6440f11852f976173c3e88f358abf7a77b5a9f5357eb5e9b9db88c8a15698560a4762a5b245aa0e5be9691f1c25020338004d02bdb380dae204358a9
```

### `dpkg` source package: `db-defaults=1:5.3.21~exp1ubuntu4`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21~exp1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21~exp1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21%7eexp1ubuntu4.dsc' db-defaults_5.3.21~exp1ubuntu4.dsc 1713 SHA512:e52e7f5604483361083ee1a295e83281936b6b0a88a6e641693d168c2a4a8bc7773ea1f186f354bd3aaf09615255b0f0cbdc07fe2c743f796cf86b5c254d1f7a
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21%7eexp1ubuntu4.tar.xz' db-defaults_5.3.21~exp1ubuntu4.tar.xz 3160 SHA512:85f9bb8c11ead651813fdfa310b9e92f99ff2e23f761d8cd82ec87cfce250b88d50e19093336d2be180789439e6cdba2c0c7ad76ca254bbdc763164c37a2d3be
```

### `dpkg` source package: `db5.3=5.3.28+dfsg2-1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg2-1`
- `libdb5.3-dev=5.3.28+dfsg2-1`

Licenses: (parsed from: `/usr/share/doc/libdb5.3/copyright`, `/usr/share/doc/libdb5.3-dev/copyright`)

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

### `dpkg` source package: `djvulibre=3.5.28-2build3`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.28-2build3`
- `libdjvulibre-text=3.5.28-2build3`
- `libdjvulibre21:amd64=3.5.28-2build3`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.28-2build3
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-2build3.dsc' djvulibre_3.5.28-2build3.dsc 2391 SHA512:b62ce50336f8330e03494bc9fad891e0edf05131ec37c30d9a90676f30efa419289f91cf8addd487219abe350abf3fd470dfb80906ebad3e445db756e2d34752
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28.orig.tar.xz' djvulibre_3.5.28.orig.tar.xz 2959024 SHA512:4fdbecd2b7b583ee4211c9cda6638a3a831c883e2552b3c8ad09f69e8734831addc14f590faab8c58d7f9f017b527abccc384f6066e674e341cf43c96db49cb7
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-2build3.debian.tar.xz' djvulibre_3.5.28-2build3.debian.tar.xz 17612 SHA512:66b190da517dd0d7992a879b821082ee6dd20bd49467d11fe15aee41c5c5d58955f6ded1ca55db3016bfc43a7f4b7fe5370ee773058a8a5c8feba2aa463a7fc0
```

### `dpkg` source package: `dpkg=1.21.21ubuntu1`

Binary Packages:

- `dpkg=1.21.21ubuntu1`
- `dpkg-dev=1.21.21ubuntu1`
- `libdpkg-perl=1.21.21ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.21ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.21ubuntu1.dsc' dpkg_1.21.21ubuntu1.dsc 3089 SHA512:b8d4b7a695092992311387dca420f17b6a4eb88fdfaf029f3f185ef3ac8c0c7572b57238a642a6b32eb7657b1f226de6179b1019ffd746a6a54770a37ad0d2dc
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.21ubuntu1.tar.xz' dpkg_1.21.21ubuntu1.tar.xz 5247484 SHA512:4e03421929041f1e8a9028acda4659c7101a584437230171ea7064b3accf7617ae146bc83c3bfbf8618dee0f090f5adaeab9663cbe30ab5a2f64aab3df3b9bec
```

### `dpkg` source package: `e2fsprogs=1.46.6~rc1-1ubuntu1`

Binary Packages:

- `comerr-dev:amd64=2.1-1.46.6~rc1-1ubuntu1`
- `e2fsprogs=1.46.6~rc1-1ubuntu1`
- `libcom-err2:amd64=1.46.6~rc1-1ubuntu1`
- `libext2fs2:amd64=1.46.6~rc1-1ubuntu1`
- `libss2:amd64=1.46.6~rc1-1ubuntu1`
- `logsave=1.46.6~rc1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.6~rc1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1-1ubuntu1.dsc' e2fsprogs_1.46.6~rc1-1ubuntu1.dsc 2957 SHA512:053deb1cadfbb95b9894216ec1a1fb90d32cba597dfd3da9e2b3895b032fa4c1ed2eaa3434158db46775a40a0296d60e9f1383905331827221df50807a9475bf
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1.orig.tar.gz' e2fsprogs_1.46.6~rc1.orig.tar.gz 9615342 SHA512:2b6afe2f8b5c83fd061bf72fe507bdc22206b1a781d3baecca693a6744f203715e8e6dd6e7864dfa853c85e72f4e94a813ff362ea8e43c0443025ab644550648
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.6%7erc1-1ubuntu1.debian.tar.xz' e2fsprogs_1.46.6~rc1-1ubuntu1.debian.tar.xz 85224 SHA512:d9ee270014468c1a00b7ada6715e3b3479b6d2f3bd3c6b044aad670304cfad4ab1bf275bc359642ca0c4d2c4d46ced52ba7740b3711ea974a75e11240d908dbd
```

### `dpkg` source package: `elfutils=0.188-2.1`

Binary Packages:

- `libelf1:amd64=0.188-2.1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `BSD-2-clause`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.188-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.188-2.1.dsc' elfutils_0.188-2.1.dsc 3451 SHA512:a094088984182d9292de101024a23034d9a79188733b6c919b6051c8aa85c81923c0a30ec6e9c594d012bf6e1d10650fb123b625033a598683d25bc3f4eaf1a8
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.188.orig.tar.bz2' elfutils_0.188.orig.tar.bz2 9112977 SHA512:585551b2d937d19d1becfc2f28935db1dd1a3d25571a62f322b70ac8da98c1a741a55d070327705df6c3e2ee026652e0b9a3c733b050a0b0ec5f2fc75d5b74b5
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.188.orig.tar.bz2.asc' elfutils_0.188.orig.tar.bz2.asc 488 SHA512:daa6e2c164602652542340863c6272628346e5f8acd1c01cca72f065ddfe23c5fcff3d84fa53916e4b888d58778958a0d5e7715033d220f1e36d4d88b5c69aa7
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.188-2.1.debian.tar.xz' elfutils_0.188-2.1.debian.tar.xz 42328 SHA512:e63a4ae7f9246049abf8c75b892e44dafebc4a90efebaf5fa94f8dd8ece4e9a88ce894662d7b2ed046af9068541413d049d7bb3ecde414522bb3edce219a7ba0
```

### `dpkg` source package: `expat=2.5.0-1`

Binary Packages:

- `libexpat1:amd64=2.5.0-1`
- `libexpat1-dev:amd64=2.5.0-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.5.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0-1.dsc' expat_2.5.0-1.dsc 1981 SHA512:feecb87fde8af281f051009ff4544a8c69f1161dad9d449402e309943f2f6e7593f7fce8007123f769af13f69ed0bbfdd99203b9c33658a2a55cd6fad3761bf6
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0.orig.tar.gz' expat_2.5.0.orig.tar.gz 8320988 SHA512:779f0d0f3f2d8b33db0fd044864ab5ab1a40f20501f792fe90ad0d18de536c4765c3749f120e21fec11a0e6c89af1dc576d1fe261c871ca44a594f7b61fd1d9e
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0-1.debian.tar.xz' expat_2.5.0-1.debian.tar.xz 12680 SHA512:f34443bb81bc18d447ce75f9a37332eabd839ac090687ebd308cdd9a906d63177ce2eb3b43757a20d8449bc852730c44e5423707d2e7c380823254551562b493
```

### `dpkg` source package: `fftw3=3.3.10-1ubuntu1`

Binary Packages:

- `libfftw3-double3:amd64=3.3.10-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.10-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.10-1ubuntu1.dsc' fftw3_3.3.10-1ubuntu1.dsc 2853 SHA512:9b6e9b0e6f9777bcc80d92d42eff0482c62ff117e26512eff0cc26e42325f775489dd7d572da0bc73d6bc0af33a23aa5d120f56eba5247f4ef255f5a138d7d40
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.10.orig.tar.gz' fftw3_3.3.10.orig.tar.gz 4262403 SHA512:fa2ea740449fd06c833a82e1fff82bacd554188d500cbedff5a0bc185551799ef9ef9b8b1c227283abdbbdd185424d19df9c0f06ed88d5fe3d9c001d6fab6109
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.10-1ubuntu1.debian.tar.xz' fftw3_3.3.10-1ubuntu1.debian.tar.xz 14776 SHA512:0c1b49c0624bfb0e74af21a60b192d939edf7da3c49f1669a801a8884b77c07f380c2b83ab7ad56a4f6c2e6344bc8e1ab67c867d94cd528dde3404374b363a6e
```

### `dpkg` source package: `file=1:5.44-3`

Binary Packages:

- `file=1:5.44-3`
- `libmagic-mgc=1:5.44-3`
- `libmagic1:amd64=1:5.44-3`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.44-3
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.44-3.dsc' file_5.44-3.dsc 2240 SHA512:2beec2c1e40017456f3afc7c8cc6788fff4b13e707117ef06bea4b6c3142dafe5abc06904cd87f9d7b00ddd1a2eb2fd3f18ed1db6a5e1d1722a9116b08f684c5
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.44.orig.tar.gz' file_5.44.orig.tar.gz 1186437 SHA512:26c3b9c7a6950649d0b2de896bfeca54289febe4cd487c0f91aa6ff1857fa49f9077f8738a17b86100125668a31dae05b586615c564f78da47ac20a1e4a74f63
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.44.orig.tar.gz.asc' file_5.44.orig.tar.gz.asc 201 SHA512:3cbcda31122ba6a28ceb7d60cceb7cf39a70a407dc4945664decc76cd7ad5ec65c73986027f3a894b1a9efa3aa5c8845a3aa643833d283083cf77dbee00001fd
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.44-3.debian.tar.xz' file_5.44-3.debian.tar.xz 38944 SHA512:cceaec62d3f936b7ba12e6ac8fb470d37c7d8c14c2aac1135ccc43de44752fcb10bbd434712fd185cd98786618335f06a47deda0e50dccb3316d617dc8f6f802
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

### `dpkg` source package: `fontconfig=2.14.1-3ubuntu3`

Binary Packages:

- `fontconfig=2.14.1-3ubuntu3`
- `fontconfig-config=2.14.1-3ubuntu3`
- `libfontconfig-dev:amd64=2.14.1-3ubuntu3`
- `libfontconfig1:amd64=2.14.1-3ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.14.1-3ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.14.1-3ubuntu3.dsc' fontconfig_2.14.1-3ubuntu3.dsc 2430 SHA512:00945e6f9196bce47e15de201b03039a5791d219783d56fb2f5e95c6100f83468ff6247d14bfbda8004498d956df9748dd8c1fc0607d94a215b0d62a065effa3
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.14.1.orig.tar.xz' fontconfig_2.14.1.orig.tar.xz 1447044 SHA512:ba42e6f90ec92914895d2157c872c373adfc17be791b92253bcc40e85674a84e43c08ab2b37c3ae85b53b2e7bd2a7847abb479043f303b732c08eeac3ee733db
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.14.1-3ubuntu3.debian.tar.xz' fontconfig_2.14.1-3ubuntu3.debian.tar.xz 28040 SHA512:afc98ffaa97df9af808428452b7c870500d9456a306e0154033cd384b4944f1dcd3326355dee06dcf8ace8f3be1481b8694bd73420d957ac0d63db63da970ce6
```

### `dpkg` source package: `fonts-dejavu=2.37-6`

Binary Packages:

- `fonts-dejavu-core=2.37-6`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-6
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-6.dsc' fonts-dejavu_2.37-6.dsc 2460 SHA512:c079ae8e72fda87e1a6605e7b2ec29c0d160440a74dadf5f9b9f370772d05ce45403df230febb5a77e97fd0d760a0319dd346f23e43cec8e9bd342e0a728dbe5
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA512:e61fc8c675ef76edb49dd9a8caee62087280929bb8144b52aca2f8def30025c56246589ad8a6a806b9574e6876eedd16d57c70a6ce9c86817a2dfe39d8a2bb2b
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-6.debian.tar.xz' fonts-dejavu_2.37-6.debian.tar.xz 12904 SHA512:9efa4065ffd7bcdf6cf7dfb27a8e1d1c3102f28a992de5e6c460f02e2ebed15ae1e90ac486cc5d01f41bf0ebd06186d15fc35a97f7879c99452d80140102a1aa
```

### `dpkg` source package: `freetype=2.12.1+dfsg-4`

Binary Packages:

- `libfreetype-dev:amd64=2.12.1+dfsg-4`
- `libfreetype6:amd64=2.12.1+dfsg-4`
- `libfreetype6-dev:amd64=2.12.1+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

- `BSD-3-Clause`
- `BSL-1.0`
- `FSFAP`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `OpenGroup-BSD-like`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.12.1+dfsg-4
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.12.1%2bdfsg-4.dsc' freetype_2.12.1+dfsg-4.dsc 3767 SHA512:0b7671f82e41de548ad12e813f457183e5eec3b7f8716ed10e3fd278a4a60200053e5ba8a80fff941473ed78151c77de022cb9de11d4f4b63cbcc23b44d0ccae
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2demos.tar.xz' freetype_2.12.1+dfsg.orig-ft2demos.tar.xz 263656 SHA512:cd9356152a64d807c75b797d005ca1dd0bde69cc2fadedec101d125cb54b2aaff1f7afa2f20839caba7db66325df7c11ed4883b7e906110356b28d9900caaae7
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.12.1+dfsg.orig-ft2demos.tar.xz.asc 833 SHA512:7e21a0136aef896f400099c80ce40ae61f226cdd1c807915bf4d856707b79ef0a1ea15a66539a4aeb55d2d1f12ba0706bd2f205d6f7545d8abb0c5c1298e9310
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2docs.tar.xz' freetype_2.12.1+dfsg.orig-ft2docs.tar.xz 2038632 SHA512:276b91b93e375096bc0f9fa76408a6ea9fa89d4d06e9c9179f88d27d41df3f3bc0ce6939ea7a3fd7c93cb694e78fd6bfb154e969188279e2bca82dcc3afd108d
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.12.1+dfsg.orig-ft2docs.tar.xz.asc 833 SHA512:39ccd90fde04074f30029a1a92b09c0d5a1bae7e2fbd965d02591e2cccda80c11588679fb0a9541a6307f120f5c8e386ba50375dc27fbd9e5c5cc3cdee5f2d82
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig.tar.xz' freetype_2.12.1+dfsg.orig.tar.xz 2188492 SHA512:0f7e7522508c716d90e0051d255904039fc548378489bc20531268d738e2deb196b81f521e31552de42fde3c955c22745585f3c5324b6968c7de6b029ce4bc92
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.12.1%2bdfsg-4.debian.tar.xz' freetype_2.12.1+dfsg-4.debian.tar.xz 43248 SHA512:3fdd44f3f2dd99bc7488bce4c1907ada988f3c7900b13af308d1f88316f9b3fc6b640073226879383545e6eccfc960035bb0e80bb6b5a2fe63ece1f33783753e
```

### `dpkg` source package: `fribidi=1.0.8-2.1ubuntu1`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.1ubuntu1.dsc' fribidi_1.0.8-2.1ubuntu1.dsc 2442 SHA512:6f9b694b666d700dd91e7f417d1e1fd2d4b15652cef31f2239400a4dabf76124c0f5281e7820b0d0bbbace82e57bd45870c5fe7da909c9425723f0061941e639
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA512:d66b1524b26d227fd6a628f438efb875c023ae3be708acaaad11f1f62d0902de0a5f57124458291ef2b0fcd89356c52ab8ae5559b0b5a93fa435b92f1d098ba2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.1ubuntu1.debian.tar.xz' fribidi_1.0.8-2.1ubuntu1.debian.tar.xz 11024 SHA512:a447a10dd07964964bfecaaa8fc28038f63c71d9209e5be803b808551114ca83d81828b07391c3cbaba3b7dcb5a01daa68a2710620500407911adc17e1f1f1f9
```

### `dpkg` source package: `gcc-12=12.2.0-16ubuntu1`

Binary Packages:

- `cpp-12=12.2.0-16ubuntu1`
- `g++-12=12.2.0-16ubuntu1`
- `gcc-12=12.2.0-16ubuntu1`
- `gcc-12-base:amd64=12.2.0-16ubuntu1`
- `libgcc-12-dev:amd64=12.2.0-16ubuntu1`
- `libstdc++-12-dev:amd64=12.2.0-16ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp-12/copyright`, `/usr/share/doc/g++-12/copyright`, `/usr/share/doc/gcc-12/copyright`, `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libgcc-12-dev/copyright`, `/usr/share/doc/libstdc++-12-dev/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gcc-13=13-20230305-1ubuntu1`

Binary Packages:

- `gcc-13-base:amd64=13-20230305-1ubuntu1`
- `libasan8:amd64=13-20230305-1ubuntu1`
- `libatomic1:amd64=13-20230305-1ubuntu1`
- `libcc1-0:amd64=13-20230305-1ubuntu1`
- `libgcc-s1:amd64=13-20230305-1ubuntu1`
- `libgomp1:amd64=13-20230305-1ubuntu1`
- `libitm1:amd64=13-20230305-1ubuntu1`
- `liblsan0:amd64=13-20230305-1ubuntu1`
- `libquadmath0:amd64=13-20230305-1ubuntu1`
- `libstdc++6:amd64=13-20230305-1ubuntu1`
- `libtsan2:amd64=13-20230305-1ubuntu1`
- `libubsan1:amd64=13-20230305-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libasan8/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan2/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-13=13-20230305-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13-20230305-1ubuntu1.dsc' gcc-13_13-20230305-1ubuntu1.dsc 27878 SHA512:de9e6fea2ad4f57bad663c06d25f1f08fbca6466267718a3c0992b77b1fda53ad8ccfa1baf26032a162f691cdfe15893b1039f9d8afe3f3ba937e2a461b64fa3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13-20230305.orig.tar.gz' gcc-13_13-20230305.orig.tar.gz 88210451 SHA512:f09d55fe761e1186b280c6891eebfef889dfbaf30b7f1ed0f3cdfcb12dc69b63beff5c346d7d2eb7e36087482bf379123ac95ed0a44d0f56e5f6a99861c5294a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13-20230305-1ubuntu1.debian.tar.xz' gcc-13_13-20230305-1ubuntu1.debian.tar.xz 530640 SHA512:c27c22bdc9a1bbbadfd3226a555dfb84a8d520116898a0263b16b314325d9d777c0e66e76de7819b20c3bd95932b34e42deb88a8e840e271b517cdc1c67dbf58
```

### `dpkg` source package: `gcc-defaults=1.203ubuntu1`

Binary Packages:

- `cpp=4:12.2.0-3ubuntu1`
- `g++=4:12.2.0-3ubuntu1`
- `gcc=4:12.2.0-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.203ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.203ubuntu1.dsc' gcc-defaults_1.203ubuntu1.dsc 14391 SHA512:e6973590d48477a12dbd2d5aa5cf21fc26968e94f5038d1a14dc67e4c2bc6d8cc719e562c5a087b7bc0faee73ad7f45fe4d1efef69f244837ebb86eb22cd974d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.203ubuntu1.tar.xz' gcc-defaults_1.203ubuntu1.tar.xz 48168 SHA512:bd68c42a51231e3fa08b28810e49429279c16d9bf399e47d26abe50a65fccc3cb79ca566534fd1f7af12c6608d9d914144d4840b36d3d04d4cd95d20b87b44fc
```

### `dpkg` source package: `gdbm=1.23-3`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-3`
- `libgdbm-dev:amd64=1.23-3`
- `libgdbm6:amd64=1.23-3`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

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

### `dpkg` source package: `gdk-pixbuf=2.42.10+dfsg-1build1`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.42.10+dfsg-1build1`
- `libgdk-pixbuf-2.0-0:amd64=2.42.10+dfsg-1build1`
- `libgdk-pixbuf-2.0-dev:amd64=2.42.10+dfsg-1build1`
- `libgdk-pixbuf2.0-bin=2.42.10+dfsg-1build1`
- `libgdk-pixbuf2.0-common=2.42.10+dfsg-1build1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-dev/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `CC0-1.0`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.42.10+dfsg-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.10%2bdfsg-1build1.dsc' gdk-pixbuf_2.42.10+dfsg-1build1.dsc 3165 SHA512:7890d45d8b8dbead9b11a40b9824eacee9552fcefbc974ff1ee68cd95b038045605d9c85dc587b4eec8306a4314a85d6ee34e2ea7c68e1c352824201beec9106
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.10%2bdfsg.orig.tar.xz' gdk-pixbuf_2.42.10+dfsg.orig.tar.xz 6439240 SHA512:34f8d7d44d12308c57bd9622efdb7344bad5a89bad7043b40d4d1cab4112ff505ebb9df98d788068ddd2e44cee193e7bcb4f1d56f0432cc859075425652a06fc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.10%2bdfsg-1build1.debian.tar.xz' gdk-pixbuf_2.42.10+dfsg-1build1.debian.tar.xz 21016 SHA512:285257ef6e98fa1347d1389b61573fee10b7e3466a34d7369a9b25cc19040108287c9142ed6205d4d409338110c47fba96dab478f068210472299ddb8e849b0c
```

### `dpkg` source package: `git=1:2.39.2-1ubuntu1`

Binary Packages:

- `git=1:2.39.2-1ubuntu1`
- `git-man=1:2.39.2-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.39.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.39.2-1ubuntu1.dsc' git_2.39.2-1ubuntu1.dsc 2919 SHA512:dda0b8e4c4c7886ec31be660484e0e43faa6456c029e5c4f396bb39014fd0e51d34a3df0f68bd3aab049989ed8abd4956eca9f488feb0a0813ee7bc72cdfa7c0
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.39.2.orig.tar.xz' git_2.39.2.orig.tar.xz 7163224 SHA512:fdca70bee19401c5c7a6d2f3d70bd80b6ba99f6a9f97947de31d4366ee3a78a18d5298abb25727ec8ef67131bca673e48dff2a5a050b6e032884ab04066b20cb
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.39.2-1ubuntu1.debian.tar.xz' git_2.39.2-1ubuntu1.debian.tar.xz 742592 SHA512:007bd077d9d74a5387807951578adb4e28d6ca76604507416a9832edfe5382aa5930bdcaf71f917ab9ce259e3bdbd981ed30288076a37e12caf9aab1c5edf649
```

### `dpkg` source package: `glib2.0=2.75.3-3`

Binary Packages:

- `libglib2.0-0:amd64=2.75.3-3`
- `libglib2.0-bin=2.75.3-3`
- `libglib2.0-data=2.75.3-3`
- `libglib2.0-dev:amd64=2.75.3-3`
- `libglib2.0-dev-bin=2.75.3-3`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `AFL-2.0`
- `Apache-2.0`
- `Apache-2.0 with LLVM exception`
- `BSD-3-clause-pcre`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `Expat`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `Iconv-PD`
- `Janik-permissive`
- `Kuchling-PD`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `Mingw-PD`
- `Old-GLib-Tests-permissive`
- `Plumb-PD`
- `Unicode-DFS-2016`
- `bzip2-1.0.6`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.75.3-3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.75.3-3.dsc' glib2.0_2.75.3-3.dsc 3659 SHA512:57eca80f01a1e899552698747a8d521431ac6eea3cca1699352600778f0fa03e719d4bfff42999c65b70280e68704663127c41068cfac902bee4ad982326652b
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.75.3.orig-unicode-data.tar.xz' glib2.0_2.75.3.orig-unicode-data.tar.xz 266184 SHA512:c818eae7b8df69b69abc2c59870eaad7488e3266afb5055b851fcbdd9dd96d9808787881631a8d840487acb3b40c18691b6c58d3df4735fa6eab41a5aa1295ff
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.75.3.orig.tar.xz' glib2.0_2.75.3.orig.tar.xz 5261616 SHA512:44aa53d0dae69e50c8d5d9adb7c90034c4c2ab5db3c74106c91bfdbdca41bc5523b32b16c33bc65b3c6bf0037bdecb344b80e9708930bde54ac7c618c34ea5a8
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.75.3-3.debian.tar.xz' glib2.0_2.75.3-3.debian.tar.xz 118112 SHA512:4016eb507d99c9d14452d9545f18cf74baef59d21fb0e7449a286fe3939c52a675c3815ef41303465519036d96baf08340b3fed3741dc064ae15e2e9d2cb75ed
```

### `dpkg` source package: `glibc=2.37-0ubuntu1`

Binary Packages:

- `libc-bin=2.37-0ubuntu1`
- `libc-dev-bin=2.37-0ubuntu1`
- `libc6:amd64=2.37-0ubuntu1`
- `libc6-dev:amd64=2.37-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.37-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37-0ubuntu1.dsc' glibc_2.37-0ubuntu1.dsc 8892 SHA512:0bf96ab0ff1f30505459d0c7f3451e661b749bda29b162131cf7f6ca12a534cba4f5959dfd301e10f85bdacae8ead514f87174cb1e79d97b20c6bed15fe1326b
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37.orig.tar.xz' glibc_2.37.orig.tar.xz 18674604 SHA512:4fc5932f206bb1b8b54828a28af1a681616b838bbab60c81c82155f3629cbfe1301d271af65511ed917f4c6949a025429221fe6035753282f15346919f15b90c
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37.orig.tar.xz.asc' glibc_2.37.orig.tar.xz.asc 833 SHA512:9849ba6aa9bff59499f67aceb69693c0331e7811fc74dea766a8e08f648ff09972449a540c3ea69bd70401464dd331f56ba29dbd00b6eeb27e9ceb42699089d8
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.37-0ubuntu1.debian.tar.xz' glibc_2.37-0ubuntu1.debian.tar.xz 880308 SHA512:c97ff7a4c370b916566d52d7e56aae7996ef8ef179847131d2312640a1b05790c6b7817241f077d7b1c851e8e1e7d343957845e5bd38cede1d2cad24f02eac19
```

### `dpkg` source package: `gmp=2:6.2.1+dfsg1-1.1ubuntu1`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.1+dfsg1-1.1ubuntu1`
- `libgmp10:amd64=2:6.2.1+dfsg1-1.1ubuntu1`
- `libgmpxx4ldbl:amd64=2:6.2.1+dfsg1-1.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

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

### `dpkg` source package: `gobject-introspection=1.74.0-3`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.74.0-3`
- `gir1.2-glib-2.0:amd64=1.74.0-3`
- `libgirepository-1.0-1:amd64=1.74.0-3`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `AFL-2.0`
- `Apache-2.0`
- `Apache-2.0 with LLVM exception`
- `BSD-2-clause`
- `BSD-3-clause-pcre`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `Expat`
- `FSFAP`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `Kuchling-PD`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `MPL-1.1`
- `Plumb-PD`
- `Unicode-DFS-2016`
- `bzip2-1.0.6`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.74.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.74.0-3.dsc' gobject-introspection_1.74.0-3.dsc 3473 SHA512:302d338c6c4fba02f92d400b517016c6e847ee565776eb8e4122ca3bea18e544aee7c8a5055a793cbcc8938c285457b4c00c45c8f9cd67300b83023b7ec3bdaf
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.74.0.orig-glib.tar.xz' gobject-introspection_1.74.0.orig-glib.tar.xz 5183072 SHA512:5cdadd2f4568c0c3d45083b4d39699abf651e42e020f7bc880cce3ff33d28943118388d17a0632777e843f48009c1f97d5634fde3cb8c69c7c7f35b278ac8225
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.74.0.orig.tar.xz' gobject-introspection_1.74.0.orig.tar.xz 1044008 SHA512:decff5dda0ec5ec0afda4d6bcd3bdadcbf34289002c0d9c0c77ecf8c5d3f15d196b24d8035041545031006acbdfe76af47c42da061c40e200c87f2c74cd301f0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.74.0-3.debian.tar.xz' gobject-introspection_1.74.0-3.debian.tar.xz 39496 SHA512:c57ef5e43c953dd0ff4379d5b7c7eaf819f41ee0dd47f484288601fb5b08e4ee1f0ae49320892258aa66c75ddca7997e72fdf7e976e93ce454166dacb3a60f66
```

### `dpkg` source package: `graphite2=1.3.14-1build2`

Binary Packages:

- `libgraphite2-3:amd64=1.3.14-1build2`

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
$ apt-get source -qq --print-uris graphite2=1.3.14-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1build2.dsc' graphite2_1.3.14-1build2.dsc 2262 SHA512:c1c167d90602a7f072189d046304af17a2a3e61509405c3623a56231f7c8341091bb2da2c73bfc41c1a3fc60a1f1b585476aec2a932767e3c31a400d37f50966
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14.orig.tar.gz' graphite2_1.3.14.orig.tar.gz 6629829 SHA512:49d127964d3f5c9403c7aecbfb5b18f32f25fe4919a81c49e0534e7123fe845423e16b0b8c8baaae21162b1150ab3e0f1c22c344e07d4364b6b8473c40a0822c
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1build2.debian.tar.xz' graphite2_1.3.14-1build2.debian.tar.xz 12224 SHA512:7c69742dc115a123eaba93092ad67c06e43e8538c04269e05fa06cb12802b9f331f52161c3ff0ddd0520ccad6993c30102f149ac1694552594a3db5f1c07a209
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

### `dpkg` source package: `harfbuzz=6.0.0+dfsg-3build1`

Binary Packages:

- `libharfbuzz0b:amd64=6.0.0+dfsg-3build1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `Apache-2.0`
- `CC0-1.0`
- `Expat`
- `FSFAP`
- `FSFUL`
- `FSFULLR`
- `GPL-2`
- `GPL-2+ with AutoConf exception`
- `GPL-2+ with Font exception`
- `GPL-2+ with LibTool exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with AutoConf exception`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `Monotype`
- `OFL-1.1`
- `UFL-1.0`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=6.0.0+dfsg-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_6.0.0%2bdfsg-3build1.dsc' harfbuzz_6.0.0+dfsg-3build1.dsc 2834 SHA512:246c33cb1491ac186f0d8386094020a777ff3ad5964af357d46376f93b56446c23e688c60aac49ff6bdc8499d8543b68263753c4c470999ffc1162e7086f7c55
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_6.0.0%2bdfsg.orig.tar.xz' harfbuzz_6.0.0+dfsg.orig.tar.xz 18981700 SHA512:cfa54e9ff936610e500bf49934bbb637b02a0414c203933f24086e5e9ad8436aeb1a2747e22fc29b7ee25f9f430f0d5e21c0c3196e108ee2b9ba0ce4b2739cb3
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_6.0.0%2bdfsg-3build1.debian.tar.xz' harfbuzz_6.0.0+dfsg-3build1.debian.tar.xz 19120 SHA512:5c0d32df8035d2e4819d4abc992b06b6f5db2a0c24238f0070df7db050972b2ea9bd984a2cc9e7e93a3a98e14ee88889a9a22472e12bfe47f6f04330b1445ad9
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

### `dpkg` source package: `icu=72.1-3ubuntu1`

Binary Packages:

- `icu-devtools=72.1-3ubuntu1`
- `libicu-dev:amd64=72.1-3ubuntu1`
- `libicu72:amd64=72.1-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/icu-devtools/copyright`, `/usr/share/doc/libicu-dev/copyright`, `/usr/share/doc/libicu72/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu=72.1-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1-3ubuntu1.dsc' icu_72.1-3ubuntu1.dsc 2359 SHA512:4a61d6f9918f90744820812020935f60632b7a615255711df51491d70c8caea67b428fc200c63803ec3899184b7cf789b973f58a6273f678e9b35a8a92173374
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1.orig.tar.gz' icu_72.1.orig.tar.gz 26303933 SHA512:848c341b37c0ff077e34a95d92c6200d5aaddd0ee5e06134101a74e04deb08256a5e817c8aefab020986abe810b7827dd7b2169a60dacd250c298870518dcae8
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1.orig.tar.gz.asc' icu_72.1.orig.tar.gz.asc 659 SHA512:8b5e841a3baa317a13cadf7deb3582a80cfab8e5bdae6bd04612ee7be3006d9acf07b015de01a94990fa350109a3c11e547482e4cb4ca986161cc701a8cd427b
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1-3ubuntu1.debian.tar.xz' icu_72.1-3ubuntu1.debian.tar.xz 62724 SHA512:63ef3360e9a72f0d52faa4f6f264e41df4c66e93187c507473eddac1c9b35a8b7da1451663d2c8c1d12d29d6475b982df8c798435c50955ea94fa46e51a2d4d1
```

### `dpkg` source package: `imagemagick=8:6.9.11.60+dfsg-1.6`

Binary Packages:

- `imagemagick=8:6.9.11.60+dfsg-1.6`
- `imagemagick-6-common=8:6.9.11.60+dfsg-1.6`
- `imagemagick-6.q16=8:6.9.11.60+dfsg-1.6`
- `libmagickcore-6-arch-config:amd64=8:6.9.11.60+dfsg-1.6`
- `libmagickcore-6-headers=8:6.9.11.60+dfsg-1.6`
- `libmagickcore-6.q16-6:amd64=8:6.9.11.60+dfsg-1.6`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.11.60+dfsg-1.6`
- `libmagickcore-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.6`
- `libmagickcore-dev=8:6.9.11.60+dfsg-1.6`
- `libmagickwand-6-headers=8:6.9.11.60+dfsg-1.6`
- `libmagickwand-6.q16-6:amd64=8:6.9.11.60+dfsg-1.6`
- `libmagickwand-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.6`
- `libmagickwand-dev=8:6.9.11.60+dfsg-1.6`

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.11.60+dfsg-1.6
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1.6.dsc' imagemagick_6.9.11.60+dfsg-1.6.dsc 5074 SHA512:f65462ca8faa4b02a3b810a1d68c3573720b305a8df70408a0eda3b62776fa8e4e8025989708f7a750069f6b6d6048d3d1f7183b19f1aafe4b8de6c88bee8451
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg.orig.tar.xz' imagemagick_6.9.11.60+dfsg.orig.tar.xz 9395144 SHA512:345a23eda96516fc7a213bd4a322bca4c8b690efe40ff7b498a448f8cedd7f0d600fae2cb6fff45bc995779a90d8c04b58288273eee97833ddebb4f9f2a3d14c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1.6.debian.tar.xz' imagemagick_6.9.11.60+dfsg-1.6.debian.tar.xz 253928 SHA512:422d67ed8cbfd9b80dc71cc6562926dbd85c5102ed0f669d615ec554a91b31327b2ec9f9554770984e9be6400387c493c9acdf87bc6527a35aa45d13c588eece
```

### `dpkg` source package: `imath=3.1.6-1ubuntu1`

Binary Packages:

- `libimath-3-1-29:amd64=3.1.6-1ubuntu1`
- `libimath-dev:amd64=3.1.6-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libimath-3-1-29/copyright`, `/usr/share/doc/libimath-dev/copyright`)

- `imath`

Source:

```console
$ apt-get source -qq --print-uris imath=3.1.6-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imath/imath_3.1.6-1ubuntu1.dsc' imath_3.1.6-1ubuntu1.dsc 2612 SHA512:2306475ca5b8666af2cb3877b0bed9ac5b114c8489368f37fed2fd17f4a0170e17b7ff6332ea52527eff6fd4901dbb32d869b17e10e40764e8f92222a7b80d9f
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imath/imath_3.1.6.orig.tar.gz' imath_3.1.6.orig.tar.gz 573255 SHA512:c099a291ed7fd7702a7609575f2f3d2ed7f95256c23c2180e2ef1f76ceb07734365f57da5244b1d6cec81ca9859864eb4c9236df02a64aa783af6639a3b59acd
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imath/imath_3.1.6.orig.tar.gz.asc' imath_3.1.6.orig.tar.gz.asc 287 SHA512:9b3978e44b531429aba42b9cc4969a470898d9d74652e3809edb0273ba9b127c471aec6570b5d352be738f59810091c0df2c70d39c16d2c32833d173b270f72c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imath/imath_3.1.6-1ubuntu1.debian.tar.xz' imath_3.1.6-1ubuntu1.debian.tar.xz 9216 SHA512:a6c32b598f6d9bdd175f5f2f74c4979c3d900dd3b9990422abe706f526a3b9baca0a9e4ae7294e1ca3153a02c68538beddc3a73b716e1b2a6700b7dcd89e25e1
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

### `dpkg` source package: `isl=0.25-1`

Binary Packages:

- `libisl23:amd64=0.25-1`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.25-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.25-1.dsc' isl_0.25-1.dsc 1832 SHA512:78192f3e921eb2f8a716c3cb877a4156c14f10d242c3c717d44ba2ff032040a47544359018dcda58c6c5c2dbf87f3ac9864bc79c53d235b6ea2eb0fcf567e73c
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.25.orig.tar.xz' isl_0.25.orig.tar.xz 1977048 SHA512:81ac6b404a71e146bb705efe647ecf3bee19c3254f534cb44228cec13ffc7a33d7d58b980106dbb120ffdc557403d966619e219328edd0a4b3cbc4ac66acb255
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.25-1.debian.tar.xz' isl_0.25-1.debian.tar.xz 24344 SHA512:0d25fb0fd63208a70d2ff55a801f628e7b12566987ea8db0a168b423872d596824dbab608e97ed6010f87d29c9464f422b0ba91cabc7f20b9047e3171c58a6d3
```

### `dpkg` source package: `jansson=2.14-2`

Binary Packages:

- `libjansson4:amd64=2.14-2`

Licenses: (parsed from: `/usr/share/doc/libjansson4/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris jansson=2.14-2
'http://archive.ubuntu.com/ubuntu/pool/main/j/jansson/jansson_2.14-2.dsc' jansson_2.14-2.dsc 1980 SHA512:e1c579cae00db3083448345690769411d1aaf2607ea956fba24542d5427f6e0ed6e2b7159b32d617d708e77b986a61c3c938f2e956e317a253c2ff10be8130f1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jansson/jansson_2.14.orig.tar.gz' jansson_2.14.orig.tar.gz 141500 SHA512:c56e2e8d18819e3f5caa46edd4819694a240aeb3524a6f9d9f4465edf65b183d1870bd5d256cdd378d411a52979121369b951406fdf7bf323db5c30001fa1bc4
'http://archive.ubuntu.com/ubuntu/pool/main/j/jansson/jansson_2.14-2.debian.tar.xz' jansson_2.14-2.debian.tar.xz 5428 SHA512:90520e3b81066b2441b0ac88d49c1bd7f55e1ae7727176cd8f397ed8cce88c6975c9a9bbbcc1f244ae83773e35695643d1dfab4136b19c624871fd7cbe3832bb
```

### `dpkg` source package: `jbigkit=2.1-6ubuntu1`

Binary Packages:

- `libjbig-dev:amd64=2.1-6ubuntu1`
- `libjbig0:amd64=2.1-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-6ubuntu1.dsc' jbigkit_2.1-6ubuntu1.dsc 2162 SHA512:89047747857d8ea307b13809aa78d442df840abc2372a59b3bd090148698698e7d8862394ae3536cf5e8cd7ee055a62a9bc23f23edc8d75592758a4066c4b234
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA512:c4127480470ef90db1ef3bd2caa444df10b50ed8df0bc9997db7612cb48b49278baf44965028f1807a21028eb965d677e015466306b44683c4ec75a23e1922cf
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-6ubuntu1.debian.tar.xz' jbigkit_2.1-6ubuntu1.debian.tar.xz 10964 SHA512:25c01c82d525684ff7e477419676c5da168f8a7b050fbd3795a4a94dc22d1c1ff38076a082fd1bb0b1e048197e6ff82661e0072d7d93745013209a36bbdf2c0e
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

- `krb5-multidev:amd64=1.20.1-1build1`
- `libgssapi-krb5-2:amd64=1.20.1-1build1`
- `libgssrpc4:amd64=1.20.1-1build1`
- `libk5crypto3:amd64=1.20.1-1build1`
- `libkadm5clnt-mit12:amd64=1.20.1-1build1`
- `libkadm5srv-mit12:amd64=1.20.1-1build1`
- `libkdb5-10:amd64=1.20.1-1build1`
- `libkrb5-3:amd64=1.20.1-1build1`
- `libkrb5-dev:amd64=1.20.1-1build1`
- `libkrb5support0:amd64=1.20.1-1build1`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit12/copyright`, `/usr/share/doc/libkadm5srv-mit12/copyright`, `/usr/share/doc/libkdb5-10/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20.1-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-1build1.dsc' krb5_1.20.1-1build1.dsc 3913 SHA512:0591c14d26d615d33ab75a3e2c5ac066ce141279eff023100a999aadd0adf4adf80212777bcc7f0409b43854303c1f6d9fc7398294bb6c62bdfc2893ba4f78b5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz' krb5_1.20.1.orig.tar.gz 8661660 SHA512:6f57479f13f107cd84f30de5c758eb6b9fc59171329c13e5da6073b806755f8d163eb7bd84767ea861ad6458ea0c9eeb00ee044d3bcad01ef136e9888564b6a2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz.asc' krb5_1.20.1.orig.tar.gz.asc 833 SHA512:1d3312bd67581e07adfdadf2c5fe394179631d8add8bd075efefe982a0de22369004e60a14422d426382c8c591e4181b9897088afe9d4e86f0b5a97e5954c67a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-1build1.debian.tar.xz' krb5_1.20.1-1build1.debian.tar.xz 99504 SHA512:f0fa16ef6c12296bf612f99f0b8f833cd9def044e6e4b62238fba31e5c5a34113a31273b0ad8784c2cbbdef746d5fac83d58ea007bec729af92226dfcbaa9d57
```

### `dpkg` source package: `lcms2=2.14-2`

Binary Packages:

- `liblcms2-2:amd64=2.14-2`
- `liblcms2-dev:amd64=2.14-2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `IJG`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.14-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.14-2.dsc' lcms2_2.14-2.dsc 1944 SHA512:0efbd4625439773c89535ad118567c240d8c555e8069712afcf139067cff5186d554824c6f2ed1d955c4b093bae0c4131419761726937e4b09256939944cc911
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.14.orig.tar.gz' lcms2_2.14.orig.tar.gz 7406694 SHA512:92fba0a457ea81590eba0b8d98b7b621da6a83e3857948585e0b524235954954f9ac1670cf6a19b457c0fce22a87899ea4c5810db1ff2acf7c6b6e0dc4b61a1b
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.14-2.debian.tar.xz' lcms2_2.14-2.debian.tar.xz 11728 SHA512:ddadbc46e78a7fbb6d75f13d7921b6710fb28c47cc2a311c7dc79e9a016ef98b81cef1e94d1b4b58af4f396b3dfb320d9f48ec6460a5afd31ead78a6040593b2
```

### `dpkg` source package: `lerc=4.0.0+ds-2ubuntu2`

Binary Packages:

- `liblerc-dev:amd64=4.0.0+ds-2ubuntu2`
- `liblerc4:amd64=4.0.0+ds-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/liblerc-dev/copyright`, `/usr/share/doc/liblerc4/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris lerc=4.0.0+ds-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lerc/lerc_4.0.0%2bds-2ubuntu2.dsc' lerc_4.0.0+ds-2ubuntu2.dsc 1675 SHA512:d055e23e3b39fb7889c73dcd9a13ce2409d00be88e9a85776260c206162569ed85e2e5024d75c3d49ec09f019f5afa9cbd08b6a582150bce321b10182817673e
'http://archive.ubuntu.com/ubuntu/pool/main/l/lerc/lerc_4.0.0%2bds.orig.tar.xz' lerc_4.0.0+ds.orig.tar.xz 348140 SHA512:d5539360fa92f40319466fea73a66d0d03aedff886fb75985bfcaeeb77ef516b9fa24b8d83da09c114bf6090bbd68e64d9ac2649a19315895134fa86023478e1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lerc/lerc_4.0.0%2bds-2ubuntu2.debian.tar.xz' lerc_4.0.0+ds-2ubuntu2.debian.tar.xz 7960 SHA512:34d2a1d2aace8916d208bec39143556fc3098e16d026a4d391a6c16bae8c61a2ec4323f61e9a26bff0470c7c9c33088103c5ee054e81f446629f3e32f9e5a96c
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

### `dpkg` source package: `libdatrie=0.2.13-2`

Binary Packages:

- `libdatrie1:amd64=0.2.13-2`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.13-2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13-2.dsc' libdatrie_0.2.13-2.dsc 2239 SHA512:86ebcb0343ca62b1e832210de6ca74e71786cf7c4c63eb5d1e944dc1bf900c986107c1120e798412fd9780902056fda1403c6124baef044778d479b53aeabb6d
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13.orig.tar.xz' libdatrie_0.2.13.orig.tar.xz 314072 SHA512:db3c879d825ead5871c12ef3a06bb093cb1708a6e7e20775eaf82356af9dd6ad54c6b5cabbe1773f2494d3dfa2426528fdd49441038b6294b70ccb1a3d90099a
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13-2.debian.tar.xz' libdatrie_0.2.13-2.debian.tar.xz 9604 SHA512:032040b6f9da493b7bbc4437eb16dce9dbbf10d0d9381fbc4ec6c636e5cccaf52b14e77739d227b58fc5ba54911c2cea7f679bada7ed93acb048bd996d4ce3d9
```

### `dpkg` source package: `libde265=1.0.11-1`

Binary Packages:

- `libde265-0:amd64=1.0.11-1`

Licenses: (parsed from: `/usr/share/doc/libde265-0/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `other-1`
- `public-domain-1`

Source:

```console
$ apt-get source -qq --print-uris libde265=1.0.11-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.11-1.dsc' libde265_1.0.11-1.dsc 2190 SHA512:6858cd87e0da7cb8300b7afb2e525d0a712c5a54bf5500fc5058c66a625e27e9102d659ffc3e39d6c1895787dd1cb96c03fc5b9e9d8b766cc3106c77bd0a1ebb
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.11.orig.tar.gz' libde265_1.0.11.orig.tar.gz 845996 SHA512:2ce28558c66e20714c07bf3011bc10dccabb770649903616bc32f1c4f18beba559ef7e0e42365ead77d7e813316b8c051039dc393cd351221cbab7248b3fa34c
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.11-1.debian.tar.xz' libde265_1.0.11-1.debian.tar.xz 13820 SHA512:e3dfa5814398567db9f9b28122d2f7e30c711d98f31c226af5d553f23780f3459adb48377cf1e16cc0f93882bb81586c953909c871ca6bcc520b5ffc6ffb4730
```

### `dpkg` source package: `libdeflate=1.15-1`

Binary Packages:

- `libdeflate-dev:amd64=1.15-1`
- `libdeflate0:amd64=1.15-1`

Licenses: (parsed from: `/usr/share/doc/libdeflate-dev/copyright`, `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.15-1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.15-1.dsc' libdeflate_1.15-1.dsc 2221 SHA512:2e78e6e2a62f6b95f6b37a9d995ea708c9dae084e00e4b910141bf3c0eb871f7c8fec26e36ed2c8e293a90eba53eb4b135daa78f0deb615df884b49a2e59b463
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.15.orig.tar.gz' libdeflate_1.15.orig.tar.gz 180818 SHA512:6503844eb113518610294c64fc0b24cbd93f58f654568f6f287c4a6549540c1044ea2123a453166ef78621ee20ef7bb8a3891a398eac1b950fdfef70236121fd
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.15-1.debian.tar.xz' libdeflate_1.15-1.debian.tar.xz 4816 SHA512:bd3801ab80af23d468637abad0b445fc89bf50bdd5220c192fc55e1badb622f62366dd2d0975f0a3207be11cc54a0295cb04d5cdcec4b8d1f5f49961098e871b
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

### `dpkg` source package: `libevent=2.1.12-stable-5ubuntu1`

Binary Packages:

- `libevent-2.1-7a:amd64=2.1.12-stable-5ubuntu1`
- `libevent-core-2.1-7a:amd64=2.1.12-stable-5ubuntu1`
- `libevent-dev=2.1.12-stable-5ubuntu1`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-5ubuntu1`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-5ubuntu1`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libevent-2.1-7a/copyright`, `/usr/share/doc/libevent-core-2.1-7a/copyright`, `/usr/share/doc/libevent-dev/copyright`, `/usr/share/doc/libevent-extra-2.1-7/copyright`, `/usr/share/doc/libevent-openssl-2.1-7/copyright`, `/usr/share/doc/libevent-pthreads-2.1-7/copyright`)

- `BSD-2-clause`
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
$ apt-get source -qq --print-uris libevent=2.1.12-stable-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-5ubuntu1.dsc' libevent_2.1.12-stable-5ubuntu1.dsc 2492 SHA512:2f36aa1ebb97c708395c97da1c23f2e9b191ac4a18d955769fb63aef4b4c53a1b1a9c792ad09e95f93e1e76a7321595ef02f4839b0a9ba634cfba56e4372296c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA512:88d8944cd75cbe78bc4e56a6741ca67c017a3686d5349100f1c74f8a68ac0b6410ce64dff160be4a4ba0696ee29540dfed59aaf3c9a02f0c164b00307fcfe84f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-5ubuntu1.debian.tar.xz' libevent_2.1.12-stable-5ubuntu1.debian.tar.xz 17148 SHA512:312e91309028c036a9a6c3e98a3989beb372960e00e8b4a2223fcf04abd9b432156ae55b24df289baf3c06a7cbd52fa29ee792091ac7493268c05e7be776ec85
```

### `dpkg` source package: `libexif=0.6.24-1build1`

Binary Packages:

- `libexif-dev:amd64=0.6.24-1build1`
- `libexif12:amd64=0.6.24-1build1`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.24-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.24-1build1.dsc' libexif_0.6.24-1build1.dsc 2211 SHA512:a087ff32fa00c47f7d9d47df7ecc53065ead75588a8ea4ffb1eaae25678aae79a713fbd4bc64a16d6667eb7ce86d9fe648409ef8d27fb5d2b3104f222cba9be6
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.24.orig.tar.gz' libexif_0.6.24.orig.tar.gz 1140079 SHA512:0b15a157c1030490bf1c4239487dffda90daad467ac6281db2a1b34a8419fca32b4b5265452e75cbcd2c9dc9a829643231cd3749e88251ed1b596756d1c5a9f4
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.24-1build1.debian.tar.xz' libexif_0.6.24-1build1.debian.tar.xz 11824 SHA512:0ba09c166ed6cc4f55e4ecc12193531cd4ab93a0274906488f5d9dd6f86f39b115e746d430c367b689b508ddc39912f716f003667bdc81ccb963f92dc941ed5f
```

### `dpkg` source package: `libffi=3.4.4-1`

Binary Packages:

- `libffi-dev:amd64=3.4.4-1`
- `libffi8:amd64=3.4.4-1`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi8/copyright`)

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

### `dpkg` source package: `libfido2=1.12.0-2`

Binary Packages:

- `libfido2-1:amd64=1.12.0-2`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.12.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.12.0-2.dsc' libfido2_1.12.0-2.dsc 2588 SHA512:11584b3ff7cdb899cb35791af50f5dbae87fb3932f5a24d00d9b05550415071edb75f3de820bbc5b2802f58e3d35eb1312fada97ff2ebef49d4c7f5b76117651
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.12.0.orig.tar.gz' libfido2_1.12.0.orig.tar.gz 652326 SHA512:ae8c716fe9b2fa52f191c4b3fe61442ba0b7a364a23c6c3a29afdba4f47c5eff89cb1d6c9fcacaefd7d4ebce641d35600527ee33934786c2096ac97f78e9418f
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.12.0.orig.tar.gz.asc' libfido2_1.12.0.orig.tar.gz.asc 228 SHA512:1d603d26fd78534ae0a5cb624ebb8c714bc3d358822f41efdbf3e7ef5056480cc04d649d7a8d821f1109511b1ac5873d5b3307a2c4e666912ca5a8a16df5a011
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.12.0-2.debian.tar.xz' libfido2_1.12.0-2.debian.tar.xz 52808 SHA512:74a1594e9f3a9d3ad05389de3d66f1bcaf0e04ec9164b5807f77cc5caaee74f046941b1c65122fb534133d0b4ca3ea1ab71d0c94df55f0963256b98801874067
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

### `dpkg` source package: `libheif=1.14.2-1`

Binary Packages:

- `libheif1:amd64=1.14.2-1`

Licenses: (parsed from: `/usr/share/doc/libheif1/copyright`)

- `BOOST-1.0`
- `BSD-3-clause`
- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libheif=1.14.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.14.2-1.dsc' libheif_1.14.2-1.dsc 2290 SHA512:2670d9cdf7cc0665c49bbf840c6e885e807f1fe96df469012af149e3ee15b0d9c131e11cb62bfbb7df600f3cde424e7ae878fcc1d1d18e4305eb9ced4dec4ab9
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.14.2.orig.tar.gz' libheif_1.14.2.orig.tar.gz 1739439 SHA512:a7b26bacbf79ee4f8621e59ffc5c96a018166c3246db53b60cf18618a3229510c9f5dda3c7b7c935ebfd4cec70b1d70f326b25a3e5a6c12fbcb4eaeaa0ae72f1
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.14.2-1.debian.tar.xz' libheif_1.14.2-1.debian.tar.xz 7564 SHA512:df4e2f35cd9096c21954151a3e6eee974846c9e90a0bd7c5731f2232a41fb36691496126a1b69af01ded5f205ebc95f1b1aa792d9e9880ecda6f35e9457641c1
```

### `dpkg` source package: `libice=2:1.0.10-1build2`

Binary Packages:

- `libice-dev:amd64=2:1.0.10-1build2`
- `libice6:amd64=2:1.0.10-1build2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.10-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1build2.dsc' libice_1.0.10-1build2.dsc 2181 SHA512:ab928645b15c679673d1adcc53f23b126f4ca90accbef677c15a1bb8bd428e642db5e45ef77b255d9b0351c2501dd01eafb9108875fff7c98f4543432d7e6fbf
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10.orig.tar.gz' libice_1.0.10.orig.tar.gz 481960 SHA512:2d4757f7325eb01180b5d7433cc350eb9606bd3afe82dabc8aa164feda75ef03a0624d74786e655c536c24a80d0ccb2f1e3ecbb04d3459b23f85455006ca8a91
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1build2.diff.gz' libice_1.0.10-1build2.diff.gz 11679 SHA512:dc850d9603ac04ffee3e2de1d2f9786520f6d9829f210649756fac705b6fe2797eda307d45283533342dd425317928fbb5f61d94bfe0fcadbc8f1c0c2cb02d6c
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

### `dpkg` source package: `libjpeg-turbo=2.1.5-2ubuntu1`

Binary Packages:

- `libjpeg-turbo8:amd64=2.1.5-2ubuntu1`
- `libjpeg-turbo8-dev:amd64=2.1.5-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `BSD-3-clause`
- `BSD-BY-LC-NE`
- `Expat`
- `NTP`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.1.5-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5-2ubuntu1.dsc' libjpeg-turbo_2.1.5-2ubuntu1.dsc 2506 SHA512:18ba0e5c7adba980760341bc97da11b0249cf6a098dade631edd3ef1cd5f5c01e30f79b3ce556a30ae32a218968b590984cf2b33942b8565bf222d00a42ae417
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5.orig.tar.gz' libjpeg-turbo_2.1.5.orig.tar.gz 2264471 SHA512:20036303fbe5703a5742dc3778cc5deb2eb98d00a9852e7e80ba73c195bba011ec206c090589c482f1153f74505c3fe06d96af00f6beaa65a7fcf7ffaf626fc2
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5-2ubuntu1.debian.tar.xz' libjpeg-turbo_2.1.5-2ubuntu1.debian.tar.xz 108396 SHA512:8ff55c71badcf8bb200b9ec72a76fa15f4e25d8785011f135d2dc4c082d7a0e5cf59ad0f9f12854bffe27a8667a48fa3f3294f627641e611d9b5f0bdae549446
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu11`

Binary Packages:

- `libjpeg-dev:amd64=8c-2ubuntu11`
- `libjpeg8:amd64=8c-2ubuntu11`
- `libjpeg8-dev:amd64=8c-2ubuntu11`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg8/copyright`, `/usr/share/doc/libjpeg8-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg8-empty=8c-2ubuntu11
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu11.dsc' libjpeg8-empty_8c-2ubuntu11.dsc 1579 SHA512:345994a54ea05e741e0e6d35f0a7fc39f45c3fc34a995e972ae6b2843baf0b2fcc0bf4726aa7bb86249e39f46a7e23a273d2430d0fcb9bb88f03c6e9d3c912aa
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu11.tar.gz' libjpeg8-empty_8c-2ubuntu11.tar.gz 1959 SHA512:eb9cec5b6f3fa5e65950b72c14709d33e638b52a2bd2ac2f2297e0edb9e9e224e6da9bbe355e082026b92d980614e8fe40196e4a3ed7cdd560a65f03b138782b
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

### `dpkg` source package: `libmaxminddb=1.7.1-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.7.1-1`
- `libmaxminddb0:amd64=1.7.1-1`

Licenses: (parsed from: `/usr/share/doc/libmaxminddb-dev/copyright`, `/usr/share/doc/libmaxminddb0/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `CC-BY-SA-3.0`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmaxminddb=1.7.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.7.1-1.dsc' libmaxminddb_1.7.1-1.dsc 2322 SHA512:516e90d23233984d6d9d2d9f13582e9066b560d75c44027a5cf1b3b38b5b2cf5c66f08c097fe6cd6c355d3bb02cbb6fa442a059a1d12ea429f809fb93d954cdc
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.7.1.orig.tar.gz' libmaxminddb_1.7.1.orig.tar.gz 252253 SHA512:df79464ef449dc3a10cb93b6ef73ac40e673a5dec49bdb4c877c8cb46fdbd56fa1594be78869afe9b4db6b65497918febe45e8842874ec42fbe2a6194b46ddd2
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.7.1-1.debian.tar.xz' libmaxminddb_1.7.1-1.debian.tar.xz 12424 SHA512:27fd372bbea0dd43228a7b451c6f406f3a07c17561ccf013bc3cf5501a6375e1387d240cf9eb35afbabeadca9c71ae392642510974e7ba966a72463f7dc6dfe8
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

### `dpkg` source package: `libnsl=1.3.0-2build2`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-2build2`
- `libnsl2:amd64=1.3.0-2build2`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build2.dsc' libnsl_1.3.0-2build2.dsc 2087 SHA512:f13d28f34b0e71b04b5a0313b1cc79cdbe7d5e7f910d649af63b42824654e3cf01c02caa0e68309cb03350a17506e034800af1b1e3ab9af99fb64121c119215c
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA512:a5a6c3ccb2d1e724c8c1f65e55dcd09383eb1ae019c55f4c09441eadf23ffbc2196cfad259805b0ac40ddf3a10af0da453e4d739d67d46829c64d0995dab4e55
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build2.debian.tar.xz' libnsl_1.3.0-2build2.debian.tar.xz 4868 SHA512:367904106ba925eaa667cc273b37afd052ba795b7ed004cdb501c13dd26b469df971ac10acec2bf57d91fa4839f356c7dcbcd4969914891152588365844ced9a
```

### `dpkg` source package: `libpng1.6=1.6.39-2`

Binary Packages:

- `libpng-dev:amd64=1.6.39-2`
- `libpng16-16:amd64=1.6.39-2`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.39-2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.39-2.dsc' libpng1.6_1.6.39-2.dsc 2241 SHA512:63a6b384ea20baec93688dfa682b837ffd98368c1cf018566cf29be080ba2098dd194537973771e0248a8ff6fdaa60eea27f3f071d6a15746dd0b43e0bb8be94
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.39.orig.tar.gz' libpng1.6_1.6.39.orig.tar.gz 1519415 SHA512:d61408cee5850582baa57166547ccab6cc171bc809076e53494ace26157fd7787c3209e3b757fd68c541bfb95afe309745d887fb5cd2005b2024af7355c809a0
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.39-2.debian.tar.xz' libpng1.6_1.6.39-2.debian.tar.xz 31076 SHA512:8e8d4c1c46ccfdf240bc87d9c5bb41710af6c76fa940edab0d19b18d3761ede4027275ff692fd0bfa0013405cd267745a94f2442d92e5e14c4312b2ef2250835
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

### `dpkg` source package: `libpthread-stubs=0.4-1build2`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.4-1build2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.4-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1build2.dsc' libpthread-stubs_0.4-1build2.dsc 2034 SHA512:57efab978e28d3efc132b1c807bce87a563ec444e5ac3f2499a4474da55bc97dbd48d28f3260c5f1d539bbdcbb4afef1bcd23ff3954255d7b5a0e092239c55f6
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4.orig.tar.gz' libpthread-stubs_0.4.orig.tar.gz 71252 SHA512:5293c847f5d0c47a6956dd85b6630866f717e51e1e9c48fa10f70aa1e8268adc778eaf92504989c5df58c0dcde656f036248993b0ea5f79d4303012bfeff3c72
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1build2.diff.gz' libpthread-stubs_0.4-1build2.diff.gz 2546 SHA512:a11200d9b898e9f9dab8a0a6d08567dfbe9177949d28e467bd9ed45a8c48d0ad881bd66d5fc9873d6876e9c78af8cb9454a0aef8ee38e0492c720518a7e90476
```

### `dpkg` source package: `librsvg=2.54.4+dfsg-1ubuntu1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.54.4+dfsg-1ubuntu1`
- `librsvg2-2:amd64=2.54.4+dfsg-1ubuntu1`
- `librsvg2-common:amd64=2.54.4+dfsg-1ubuntu1`
- `librsvg2-dev:amd64=2.54.4+dfsg-1ubuntu1`

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
- `CC-zero-waive-1.0-us`
- `Expat`
- `Expat,`
- `FSFAP`
- `LGPL-2`
- `LGPL-2+`
- `MPL-2.0`
- `MPL-2.0,`
- `OFL-1.1`
- `Sun-permissive`
- `Sun-permissive,`
- `Unlicense`
- `Unlicense,`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.54.4+dfsg-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.54.4%2bdfsg-1ubuntu1.dsc' librsvg_2.54.4+dfsg-1ubuntu1.dsc 2375 SHA512:9c9229cb7eb4a4cdd670862075256f2afe637f945a54496b48aff59f8bac1e0fe0a58c8bc4f76da544130223fdb750ddf17904363d92d34035b71e64fb9dd604
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.54.4%2bdfsg.orig.tar.xz' librsvg_2.54.4+dfsg.orig.tar.xz 20610076 SHA512:8c893ffcb7e6ab0c0c336d14056233924bacf60270a0a0f953c01f2e0e028c8a99aefc7996d0d1006031918781d967bf5db3bf5bf22b91984ae0f002e06a4133
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.54.4%2bdfsg-1ubuntu1.debian.tar.xz' librsvg_2.54.4+dfsg-1ubuntu1.debian.tar.xz 34460 SHA512:cb86e681e2d032d132bd2fb933ce37568562845c6012d4bdb84b60c090023feaaf7951e27a7d2ee8351bdbfc29810509ce8a883e15515c8714578a94adbcf3e7
```

### `dpkg` source package: `libseccomp=2.5.4-1ubuntu2`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libselinux=3.4-1build4`

Binary Packages:

- `libselinux1:amd64=3.4-1build4`
- `libselinux1-dev:amd64=3.4-1build4`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

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

### `dpkg` source package: `libsepol=3.4-2`

Binary Packages:

- `libsepol-dev:amd64=3.4-2`
- `libsepol2:amd64=3.4-2`

Licenses: (parsed from: `/usr/share/doc/libsepol-dev/copyright`, `/usr/share/doc/libsepol2/copyright`)

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

### `dpkg` source package: `libsm=2:1.2.3-1build2`

Binary Packages:

- `libsm-dev:amd64=2:1.2.3-1build2`
- `libsm6:amd64=2:1.2.3-1build2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.3-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1build2.dsc' libsm_1.2.3-1build2.dsc 2170 SHA512:4dc5d9445614801154fb411ae2089c80c55adaea90a9d78a958724d70fc8ea8d36c9a898a478f18a9669f3448d9d9a948c632f2a4869287d1e1f88403e304096
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3.orig.tar.gz' libsm_1.2.3.orig.tar.gz 445362 SHA512:03b77d86b33cdb3df4f9d65131a0025182f3cb0c17b33a90d236e8563b3011d225b9d006186302d07850edafa5b899aec6a086b8d437d357cd69fedd5f22d94b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1build2.diff.gz' libsm_1.2.3-1build2.diff.gz 9062 SHA512:c5ddeb48fe7c846b31382a5da42a2970ae12995afb322c6291977b7ffd2251d4d9e9dc163ecb008902ae8ee3c3a44526115bddc92b402c8f4a9ea0f29f1cb037
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

### `dpkg` source package: `libthai=0.1.29-1build1`

Binary Packages:

- `libthai-data=0.1.29-1build1`
- `libthai0:amd64=0.1.29-1build1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.29-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.29-1build1.dsc' libthai_0.1.29-1build1.dsc 2457 SHA512:d4181f56ccec5cddf5e65a01386d30b51a1e9cea2fd671577fa5cf14435ea3e9b0a6e6668f1f008a0d4180067d4498b163309f5a7a51b2f4ef64ab868439bb0c
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.29.orig.tar.xz' libthai_0.1.29.orig.tar.xz 417728 SHA512:0ba1261581a1705a2a2546a3071acb3c63892dbf111f0dad415667165a6b9542a5e4549061c67b11ec53de7c9e70fceb3c04d794fd12a22d991a539dbacebda1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.29-1build1.debian.tar.xz' libthai_0.1.29-1build1.debian.tar.xz 12676 SHA512:fd2032f66f172ee3e2646099205474c2bbe6a0dd0f0fd685b9e8add66017a160946d5708b4bac4ae9aa5da3062eafdc34c0228c99910b1c013aaee29b9ab9d07
```

### `dpkg` source package: `libtirpc=1.3.3+ds-1`

Binary Packages:

- `libtirpc-common=1.3.3+ds-1`
- `libtirpc-dev:amd64=1.3.3+ds-1`
- `libtirpc3:amd64=1.3.3+ds-1`

Licenses: (parsed from: `/usr/share/doc/libtirpc-common/copyright`, `/usr/share/doc/libtirpc-dev/copyright`, `/usr/share/doc/libtirpc3/copyright`)

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

### `dpkg` source package: `libtool=2.4.7-5`

Binary Packages:

- `libltdl-dev:amd64=2.4.7-5`
- `libltdl7:amd64=2.4.7-5`
- `libtool=2.4.7-5`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.7-5
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7-5.dsc' libtool_2.4.7-5.dsc 2257 SHA512:f231321981d3ccc8fda7656665289c22b078ae46fbcad5283e3134731837599c382dbd436079b542fd810d45f801ebfff2c8515c4fb93c1b718798cfb226b1d7
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7.orig.tar.xz' libtool_2.4.7.orig.tar.xz 1026028 SHA512:424f4549aa713917859dc31e62153934c67b8b9d5718452f0e50bb8f6ef48ae6274cc4d4ddd905b15858d19c60daf8c194471e6ed0c8f76e7d55e7ef932a8d3a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7-5.debian.tar.xz' libtool_2.4.7-5.debian.tar.xz 40136 SHA512:a8f14f297f49987e78ece51c074c338322ff3aa1dbc2b13b491c97e729f99a756e9b8259791f9810dc293b095da5ea80b45823bd0e954004e47e3950cc344660
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

### `dpkg` source package: `libwebp=1.2.4-0.1build1`

Binary Packages:

- `libwebp-dev:amd64=1.2.4-0.1build1`
- `libwebp7:amd64=1.2.4-0.1build1`
- `libwebpdemux2:amd64=1.2.4-0.1build1`
- `libwebpmux3:amd64=1.2.4-0.1build1`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp7/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=1.2.4-0.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4-0.1build1.dsc' libwebp_1.2.4-0.1build1.dsc 2400 SHA512:1a1acba2a4c7893f97026dad51d885a29e7651e79653b0203e13d13c06d7d0601bbe65a514d5a1447d6ed7ca2adba3be0b3d48397dead1656049345cbead1760
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4.orig.tar.gz' libwebp_1.2.4.orig.tar.gz 4141376 SHA512:01f21e2c3057f5878b33664d0070832d78420de3cb2fe4379b07ae6a27bb569fd1c27a920fe324beccb96ae7bfa8c05fdd9e7b0aeba6de06ab4d8b084bb38803
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4.orig.tar.gz.asc' libwebp_1.2.4.orig.tar.gz.asc 833 SHA512:a9a27c81550a3376f9d6e56f3914ee2ad11c3200fb555a5fcb14d7fcf8d8f32a80d8fa5c9a27908a02059a4e2eeb21b1bceaa2061a7c0e809481e47592ec2fa6
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4-0.1build1.debian.tar.xz' libwebp_1.2.4-0.1build1.debian.tar.xz 7220 SHA512:cd021da32fae52d148bb7546df661c994976024957021a6687958e6a79d14588f75bfb29ef3ce7361e5a3a5de4f79d2c412ea123ddd7b0e9a1749df0074c2b82
```

### `dpkg` source package: `libwmf=0.2.12-5ubuntu3`

Binary Packages:

- `libwmf-0.2-7:amd64=0.2.12-5ubuntu3`
- `libwmf-dev=0.2.12-5ubuntu3`
- `libwmflite-0.2-7:amd64=0.2.12-5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libwmf-0.2-7/copyright`, `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmflite-0.2-7/copyright`)

- `AGPL-3`
- `AGPL-3 with Font exception`
- `GD`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.12-5ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.12-5ubuntu3.dsc' libwmf_0.2.12-5ubuntu3.dsc 2632 SHA512:0e35d0cb8a476b45b01c4e26116a3ac41e49231b2beca21cbf96737f4d7c3df4d6460c9223af9bef512bde181d37b570c8b70a0286f78cfd8e2ba51ec8234c08
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.12.orig.tar.gz' libwmf_0.2.12.orig.tar.gz 3043572 SHA512:9280851e560becc91546906b911e0c59a1abd690e10680f6d94a335d66aeaec5eb12ccf2214ee7af2a15729a7b5f8b906022822399b4e2bc12c75a2d75748cab
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.12-5ubuntu3.debian.tar.xz' libwmf_0.2.12-5ubuntu3.debian.tar.xz 26276 SHA512:d7d56bf93cbdeb5398de03e9e39d65aa38c8a92f0fd4c049f154c2db4d7d5635617808bcbf1a5c46793fbd097e2b476574ae5a11dcaa1c874649105ada418905
```

### `dpkg` source package: `libx11=2:1.8.4-2`

Binary Packages:

- `libx11-6:amd64=2:1.8.4-2`
- `libx11-data=2:1.8.4-2`
- `libx11-dev:amd64=2:1.8.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.8.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.4-2.dsc' libx11_1.8.4-2.dsc 2483 SHA512:91627b61789ef627ad27e897478e91044634d0d242c94650ffa62c9b09ec16536884a0e6b1eb0f763890d328aae9e9400683f4c1aebed0953f8b07d01fb3d18a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.4.orig.tar.gz' libx11_1.8.4.orig.tar.gz 3168573 SHA512:b694964c529a3b9b40a67840636a4bdf5641742ad65f1596bd6ea88c51ade1b37cfcdc879f09beac9c5cfe55813128905ebf37bf844b221d4f03a935a5219436
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.4.orig.tar.gz.asc' libx11_1.8.4.orig.tar.gz.asc 801 SHA512:bf9d8ab92ffa841cd1a52845885a008c97ad76356410a29ea787309bafab2e31dce8cc32b58085281d22693e412d3cefcdae6bd901b16f1c636b54ebe5734619
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.4-2.diff.gz' libx11_1.8.4-2.diff.gz 110943 SHA512:4c75e3cc94f951b2dbd4b4bb8c446ed9b571813daf57bc02a48e30066322e89205da9eb65aecb06e2f3e7e9a63183037e8cb2569f8831a992c724cde960b86f8
```

### `dpkg` source package: `libxau=1:1.0.9-1build5`

Binary Packages:

- `libxau-dev:amd64=1:1.0.9-1build5`
- `libxau6:amd64=1:1.0.9-1build5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-1build5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-1build5.dsc' libxau_1.0.9-1build5.dsc 2315 SHA512:b9a9d6888a70e8c7e8161a322a425316ed181d00ad3881caea788aeda9c4346122a70c57d30b91e7692f5c0b468da9d784c228ead5487cfb2474f4fc42b83ada
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA512:3b22f34a4e35d17421189df8ce3f858b0914aef0cea0b12689dd8576f14eb811e39d6e32384251573daa7e3daba400deea98e7c0e29b4105138cf82195d7f875
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz.asc' libxau_1.0.9.orig.tar.gz.asc 801 SHA512:e59b2944591499d0c0291a8d80ad8ee2cb13ee00c32b0d26c6af12a2bb96c947d4d15924ef15b377b8d7640b75b50f9b8127ba53c582090b3f73b7bcf9e00b01
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-1build5.diff.gz' libxau_1.0.9-1build5.diff.gz 10579 SHA512:9485f97bc34a7b348a7bd276001ff5e455a17c8d6b6d6e4382496c38f470f1650f7177103d2b123f25f21ce62899ceb3112909ee92e9a604d302d3c63cb59e8f
```

### `dpkg` source package: `libxcb=1.15-1`

Binary Packages:

- `libxcb-render0:amd64=1.15-1`
- `libxcb-render0-dev:amd64=1.15-1`
- `libxcb-shm0:amd64=1.15-1`
- `libxcb-shm0-dev:amd64=1.15-1`
- `libxcb1:amd64=1.15-1`
- `libxcb1-dev:amd64=1.15-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.15-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.15-1.dsc' libxcb_1.15-1.dsc 5344 SHA512:c86944cd1ec1fe3ae638765551f6061b27c2a83b64a2f3afafe605d4dab5ca7c6752d7ab585bff098dc26b814b435836047c990e7d873d45bbe396fa30ae645e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.15.orig.tar.gz' libxcb_1.15.orig.tar.gz 650774 SHA512:4099899c37fdda62a9a0883863ee9e50b5072e8f396ba6f4594965d9f1743fb6ea991974a99974c6f39bac14ce9aad5669fa633ac1ad2390280d613cc66eb00e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.15-1.diff.gz' libxcb_1.15-1.diff.gz 26267 SHA512:c2a77f0109f7f478623ec4b7f0799175a5cc5cfafdfb036c6fa879bd4d20ce736476534f5e2d2763137dc537a568164287a3b5334346b989b5a91d75beeb79a5
```

### `dpkg` source package: `libxcrypt=1:4.4.33-2`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.33-2`
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

### `dpkg` source package: `libxdmcp=1:1.1.3-0ubuntu5`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.3-0ubuntu5`
- `libxdmcp6:amd64=1:1.1.3-0ubuntu5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.3-0ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu5.dsc' libxdmcp_1.1.3-0ubuntu5.dsc 2252 SHA512:5b6df4dd48380acff08dbe1fe40258d33a2f431e27da076ce54e0a1714dacb1e031aa49e2ace3863dc2131de4df42aa76b423f44f520fd8b2dbb18c4bddcada1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3.orig.tar.gz' libxdmcp_1.1.3.orig.tar.gz 429668 SHA512:edd05654ad9ea893e9e08269e25ea050d10eaf9f997a08494e24127d1ba0c896cd5338b4595b155c8cbf576e1d910b76e6ad7820fee62d74644f1f276551e2f2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu5.diff.gz' libxdmcp_1.1.3-0ubuntu5.diff.gz 18395 SHA512:552a04477a7852b2a68ba268dcd19cee9dd89c2774b6c86ca8f11180f6b179cc7853348653cf3b7d3e89a0079bef91308e8da2dfd34d0f42104f352e47ea07bd
```

### `dpkg` source package: `libxext=2:1.3.4-1build1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.4-1build1`
- `libxext6:amd64=2:1.3.4-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-1build1.dsc' libxext_1.3.4-1build1.dsc 2250 SHA512:d7a857fa82374d6b0f1435f55c697f82f5f17e9492d74eea29e04679eb6a5dd49aeb88abb048e904de207c57d16d5ad487067e6fb45696834ac5c934040d7e90
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA512:4eebd639fd57cb9b84a1e17e368f82fbf3d9f021eef5ad3fe31dd128500db57862a82c1e0d214d447cb7641b2be3fd7e949ee1196f2a482793c6628fb1e5cd70
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-1build1.diff.gz' libxext_1.3.4-1build1.diff.gz 12588 SHA512:bfcebe8e6e277dc1ea81063a4a4663e24b78f2b69439e3b8ed2209168016876f55e8e95c6a1828ab5bf7a1936ec795e14f4391b24ec8801e0102e00e953d46e4
```

### `dpkg` source package: `libxml2=2.9.14+dfsg-1.1build2`

Binary Packages:

- `libxml2:amd64=2.9.14+dfsg-1.1build2`
- `libxml2-dev:amd64=2.9.14+dfsg-1.1build2`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.14+dfsg-1.1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.1build2.dsc' libxml2_2.9.14+dfsg-1.1build2.dsc 2947 SHA512:dd8bb4d89b54c1cc4a8855e56eabf60e3c5c1722a4971f30ada9c82f54b83e7bb38eac1243b0aa5728a6b7c73245b9c4a778cf1826aa43f36a063867b3324acf
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg.orig.tar.xz' libxml2_2.9.14+dfsg.orig.tar.xz 2351200 SHA512:1eacc9ac2cd8d38b8466659b3b9d84b94eb765c8f869d6cca0da131060bbc35c2b31c6148d59690547871a20cea339eac8fbe953b4fe37cf0900862f3fd9621b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.1build2.debian.tar.xz' libxml2_2.9.14+dfsg-1.1build2.debian.tar.xz 32936 SHA512:e0b3cc12461b3b51428341fe51edf0a3a9d70ef2262ea7908418df81d4404c4a17dfa2b3377c8920d1f45b0941932eec17936c68c1cf36f7681044631d07fe47
```

### `dpkg` source package: `libxrender=1:0.9.10-1.1`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1.1`
- `libxrender1:amd64=1:0.9.10-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.1.dsc' libxrender_0.9.10-1.1.dsc 2072 SHA512:0cbb2a8642aad32961e86c36ae69b38b8a78f5894991c4efd54de89864ce3ef1821a6019c365e5e1af23a6c50727fb18045caa2dc261f677b3366ffe05cb0123
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA512:7768e62b500f468460f88f27bc1130170b204b478573d9e4406867e557b5638b7c1e21d88d51f9e774ce2344780a384e3c3be51421275d2ee880f9a978a3a232
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.1.diff.gz' libxrender_0.9.10-1.1.diff.gz 15201 SHA512:079ceac53ac1cfa5ab7ba14356af16e581eb64a1a140861b55301a6ec9ecdd79e26b6719e8aabd90cd819a92517d80f25933f6b83f85eb2e1694bcb7540e9b78
```

### `dpkg` source package: `libxslt=1.1.35-1`

Binary Packages:

- `libxslt1-dev:amd64=1.1.35-1`
- `libxslt1.1:amd64=1.1.35-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.35-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.35-1.dsc' libxslt_1.1.35-1.dsc 2155 SHA512:4bd19486b3a8bc9c4ef5b3a14ce9e3b4440d9c12b667ead50aab450841474fb24d60abc427373e5ffedcbcc4515695896a34c641dfebe52ab74cdd58a7cfe52b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.35.orig.tar.xz' libxslt_1.1.35.orig.tar.xz 1827548 SHA512:9dd4a699235f50ae9b75b25137e387471635b4b2da0a4e4380879cd49f1513470fcfbfd775269b066eac513a1ffa6860c77ec42747168e2348248f09f60c8c96
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.35-1.debian.tar.xz' libxslt_1.1.35-1.debian.tar.xz 21420 SHA512:f3b04999fa4f9e2924406e110fafcebb8de63f6964409f8bf4efd43066e872042a81e0d7ae706819b35b01e99455c537cf9da725b7ae6e78d63f8fee07c60f52
```

### `dpkg` source package: `libxt=1:1.2.1-1`

Binary Packages:

- `libxt-dev:amd64=1:1.2.1-1`
- `libxt6:amd64=1:1.2.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1-1.dsc' libxt_1.2.1-1.dsc 2312 SHA512:6176a90a0e929b22b0b2cc9e34844e904353ecac42fec4498005fb16a1c614051ad7d5dc407489316bdc7a7a7db19800ef43b06bb450961171b86200a2044b9c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz' libxt_1.2.1.orig.tar.gz 1024473 SHA512:73c2fd8a6590ab5ee93cf646e4f41fb71d424961ecbf9bc13c68abdf539c63ab0c59a4d3b22195ba21859523f4cf0e937648424532794a1350a5891061096503
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz.asc' libxt_1.2.1.orig.tar.gz.asc 358 SHA512:135e01b8a79beac9530087dee1a5458c359b4f1ae8346e2502f72f4fc24be400477fda90944315c585e3416e80cb74d1a140d5dfec81e854a4996199a8b221dc
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1-1.diff.gz' libxt_1.2.1-1.diff.gz 45419 SHA512:432a4911d7c6a15f87a093104c1e91df9b122410394ad242d8d5e219fe6c4d65c4ae99b82aafece96dea706f43601dab365557af18c7f332a812012eff0dabf1
```

### `dpkg` source package: `libyaml=0.2.5-1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.5-1`
- `libyaml-dev:amd64=0.2.5-1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.5-1.dsc' libyaml_0.2.5-1.dsc 2071 SHA512:f98d96ba0e2555436999dfb6056a27008df5abd23804c25e9b67d39080f4cd910839a507af5cfcc2c3b1df147ee3035846ba1c1df8aa9abfd4c0ed2acafaab7d
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.5.orig.tar.gz' libyaml_0.2.5.orig.tar.gz 85055 SHA512:a0f01e3fc616b65b18a4aa17692ee8ea1a84dc6387d1cf02ac7ef7ab7f46b9744c2aac0a047ff69d6c2da1d2a2d7b355c877da0db57e34d95cd4f37213ab6e7e
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.5-1.debian.tar.xz' libyaml_0.2.5-1.debian.tar.xz 5324 SHA512:32fb54badad393df364cc3967856fac5dcc9820966c61bf9885a1f359598ab541626bd081957b4c92fb4204050d703c9dd0f09c903c3eb6d385cefe322e88e82
```

### `dpkg` source package: `libzstd=1.5.2+dfsg2-3`

Binary Packages:

- `libzstd-dev:amd64=1.5.2+dfsg2-3`
- `libzstd1:amd64=1.5.2+dfsg2-3`

Licenses: (parsed from: `/usr/share/doc/libzstd-dev/copyright`, `/usr/share/doc/libzstd1/copyright`)

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

### `dpkg` source package: `linux=6.1.0-16.16`

Binary Packages:

- `linux-libc-dev:amd64=6.1.0-16.16`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris linux=6.1.0-16.16
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_6.1.0-16.16.dsc' linux_6.1.0-16.16.dsc 6876 SHA512:7ee9048ffa3021bb984372e12c374ef30817e6596434f68c2003df5f1eac8a3ad1b3f4ab36294f9e41fe98cf15b50387fd9eb173c6d6981f2e55104777f0fc39
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_6.1.0.orig.tar.gz' linux_6.1.0.orig.tar.gz 216385695 SHA512:9d8a57d9071ffe6bd7e43a52d565e455ac00e64d40137d964c66fe47838b178dddc5c278b18d3486f80966a57a8eac720c45291ea822d64996202dccbeccd4b7
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_6.1.0-16.16.diff.gz' linux_6.1.0-16.16.diff.gz 4199184 SHA512:14bd54c964f1cedc38034f2b227d96c0d0411372ae74fad470293c4b8ab5ac303a7ddc9b56d8bd04fb0f2cdd056ee91910bc53d9863b52aadf7936d160fc9c60
```

### `dpkg` source package: `lto-disabled-list=38`

Binary Packages:

- `lto-disabled-list=38`

Licenses: (parsed from: `/usr/share/doc/lto-disabled-list/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lto-disabled-list=38
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_38.dsc' lto-disabled-list_38.dsc 1435 SHA512:4d1fd697a403b8b60e663e7580d5057086ff68fc5aacc774560faf2d3aa5391c14191372e51ef01ed4139c58419da1d63bb293756be5c870dba0692c3ec32afd
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_38.tar.xz' lto-disabled-list_38.tar.xz 13108 SHA512:104bb8a84f037859d4115cf52f29762ea7e3f25c9214b825b4c9e2d2bc9d24bff09628148de0ef76eb0b58d6ef8b110b046acb6804d52455e8bca5bee1ac723b
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

### `dpkg` source package: `lzo2=2.10-2build3`

Binary Packages:

- `liblzo2-2:amd64=2.10-2build3`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.10-2build3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2build3.dsc' lzo2_2.10-2build3.dsc 2058 SHA512:37c777797173360a4f835428066b3d9707e428452e7b6ec8b662828020f712123d0c39f1d534f2c9becc42cb91765bee7d0f1d4b7c61762f2af5cc1cbedd1bb9
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10.orig.tar.gz' lzo2_2.10.orig.tar.gz 600622 SHA512:a3dae5e4a6b93b1f5bf7435e8ab114a9be57252e9efc5dd444947d7a2d031b0819f34bcaeb35f60b5629a01b1238d738735a64db8f672be9690d3c80094511a4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2build3.debian.tar.xz' lzo2_2.10-2build3.debian.tar.xz 7068 SHA512:e25f2f05621bb4d81e85e8a7e0d0c0673f0f5162db09bb6a3b07f766f58e8f50021a2453fa67bfb506bf1653a42f6a33fb786b66597ce138aa075bbb0d69f68a
```

### `dpkg` source package: `m4=1.4.19-3`

Binary Packages:

- `m4=1.4.19-3`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.19-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.19-3.dsc' m4_1.4.19-3.dsc 1637 SHA512:34792bd42cd1c32e7b89468673ce34e3fb913b283f17ff989eeebe2e6b7c76019e322fc908ca9f2d2b8afeaf0d5f13033044f20e74714c0b0369af164aa7578e
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.19.orig.tar.xz' m4_1.4.19.orig.tar.xz 1654908 SHA512:47f595845c89709727bda0b3fc78e3188ef78ec818965b395532e7041cabe9e49677ee4aca3d042930095a7f8df81de3da1026b23b6897be471f6cf13ddd512b
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.19.orig.tar.xz.asc' m4_1.4.19.orig.tar.xz.asc 488 SHA512:d6ac9c6a54c57e9b53fb3e34a60d49df2f46a6e494da0a0c9ae8246b984e68a853b5d8c42677c1a0485c3f36b0bce10a481d3775c0edc1dbdfb27b43545bc31e
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.19-3.debian.tar.xz' m4_1.4.19-3.debian.tar.xz 17184 SHA512:1c5b84935a581f9dad866f0ee832e99503b07c3b56bde945b7cb9f27ccce5b30721428f4457f54df571254426768371c3ebed59d144bdd15f8ecfefe1cdaf796
```

### `dpkg` source package: `make-dfsg=4.3-4.1build1`

Binary Packages:

- `make=4.3-4.1build1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.3-4.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4.1build1.dsc' make-dfsg_4.3-4.1build1.dsc 2072 SHA512:f5580f5dc9e7d4ee3a7bfcd82a42c0615a4828cac1f84db3c720260209cee3334d0a23ea78113cd2b26eaf233d46ec59743d14a8bd05cfd225f111ff739ad57d
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA512:bdc150f9d256145923380d6e7058ab9b2b4e43fcb1d75ab2984fa8f859eab6852a68e4ea5f626633e0bec76fbebf1477378e268e8ffdb5cb2a53b29cbc439bc1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4.1build1.diff.gz' make-dfsg_4.3-4.1build1.diff.gz 50780 SHA512:258dc63a0cea09995adfe4091599664e2ef0d5f81c990f980b0ddf9e02212177c4a23fa8d82e886ecbae33c84816c61530e97fd82c5347ff25a434a3aa6732ae
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

### `dpkg` source package: `mpclib3=1.3.1-1`

Binary Packages:

- `libmpc3:amd64=1.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.3.1-1.dsc' mpclib3_1.3.1-1.dsc 1877 SHA512:242e6c50161e6a9123dd9599629cc11b2ebc3e572186cfcd09f94d72df9e23db7937b825515331ed00e5d0825585c0898b435d9213aa31be5c2648d5e0f54825
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.3.1.orig.tar.gz' mpclib3_1.3.1.orig.tar.gz 773573 SHA512:4bab4ef6076f8c5dfdc99d810b51108ced61ea2942ba0c1c932d624360a5473df20d32b300fc76f2ba4aa2a97e1f275c9fd494a1ba9f07c4cb2ad7ceaeb1ae97
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.3.1-1.debian.tar.xz' mpclib3_1.3.1-1.debian.tar.xz 4656 SHA512:637b992f2eeab690a45397851dd4665d88e026054a6da08404e5fd96fc4d4a583bbf21922e3282e93345a17e091a373492a3a426eb1b2d25d19c8d83d013fdd1
```

### `dpkg` source package: `mpdecimal=2.5.1-2build2`

Binary Packages:

- `libmpdec3:amd64=2.5.1-2build2`

Licenses: (parsed from: `/usr/share/doc/libmpdec3/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.5.1-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1-2build2.dsc' mpdecimal_2.5.1-2build2.dsc 2026 SHA512:2f930154a94b9b4090f18e848ea94d115304827e351abc9141ef8646b9937a0f93eb2517790b661b0569e22bb498497c03972233e1ace6bdd85c9fc6922e7e70
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1.orig.tar.gz' mpdecimal_2.5.1.orig.tar.gz 2584021 SHA512:710cb5cb71dbcf3e170ca15869c148df0547b848400c6b6dd70c67d9961dbe1190af8fb4d1623bfb0ca2afe44f369a42e311ab5225ed89d4031cb49a3bd70f30
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1-2build2.debian.tar.xz' mpdecimal_2.5.1-2build2.debian.tar.xz 6860 SHA512:261ab28a609fbcff2b9561f1b1e484500c5652e48bd0abc4f8c5df73b7e00333b80f1fe416c84800690d13d52d2af72d97503dcd0afa61073ee5610d62a52a02
```

### `dpkg` source package: `mpfr4=4.2.0-1`

Binary Packages:

- `libmpfr6:amd64=4.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.2.0-1.dsc' mpfr4_4.2.0-1.dsc 1959 SHA512:37028f092546cdb981cea24df989508902bed3df8db43ef6e6ef12e95d5da34ab96ea5bed21238949eadb332b0ece995d738a1b39f72beaae5ddf6996b7b986d
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.2.0.orig.tar.xz' mpfr4_4.2.0.orig.tar.xz 1477532 SHA512:58e843125884ca58837ae5159cd4092af09e8f21931a2efd19c15de057c9d1dc0753ae95c592e2ce59a727fbc491af776db8b00a055320413cdcf2033b90505c
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.2.0-1.debian.tar.xz' mpfr4_4.2.0-1.debian.tar.xz 12488 SHA512:6b5acd25cdf8d183e7c9d26af13811dd0cc07cedcda1d6956da45e42ac665beebee510e5428b30d96968e40df1afe94ad55d1eef6e710d0a59ab857655ab0f87
```

### `dpkg` source package: `mysql-8.0=8.0.32-0ubuntu4`

Binary Packages:

- `libmysqlclient-dev=8.0.32-0ubuntu4`
- `libmysqlclient21:amd64=8.0.32-0ubuntu4`

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
$ apt-get source -qq --print-uris mysql-8.0=8.0.32-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.32-0ubuntu4.dsc' mysql-8.0_8.0.32-0ubuntu4.dsc 3536 SHA512:17f6789bd6fd716276eaf249516ba95b344bdf8acfa2ccbe2e7bed10063cd73f4b3ddf87ad3343e8e3afe3b097fce7e8a6db76f3964da56faa05d87caa79b17c
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.32.orig.tar.gz' mysql-8.0_8.0.32.orig.tar.gz 436207624 SHA512:937e0d0350cb583bb4de15b080f08ed92b253a6d7c09f13a028855dae154fc84f0c95fb082b818b2fa6fa792cd2d9db8d7dc7a20a2a0d3d2b6839fbd2c821b44
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.32-0ubuntu4.debian.tar.xz' mysql-8.0_8.0.32-0ubuntu4.debian.tar.xz 421812 SHA512:d123fc90bbb150c7bf48cb6c1d140bef064b227abfff1ee3b276aa38502b8c2cbd967ab5b33fd23304b9befd6c4eac54d9f27ec28938dd13e3175d9c001e8da2
```

### `dpkg` source package: `mysql-defaults=1.1.0`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.1.0`
- `mysql-common=5.8+1.1.0`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.1.0
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.1.0.dsc' mysql-defaults_1.1.0.dsc 2279 SHA512:a1743552a88c65e8258eb5174b488c68d5f58e78a13a7c16491855dfb1d83627041668bfbae6148d917a2fe70cfbd6571a22380522f3077413a9cb20e039e783
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.1.0.tar.xz' mysql-defaults_1.1.0.tar.xz 7396 SHA512:e4fa4e01dbacc0655cea8e6c4d3b79e8edd9a8626977ef47d83fd155d4997bd36ff93377d368d26cea7fd6bd412dd058db5cc063ae3051c9d0ab4f3283e46995
```

### `dpkg` source package: `ncurses=6.4-2`

Binary Packages:

- `libncurses-dev:amd64=6.4-2`
- `libncurses5-dev:amd64=6.4-2`
- `libncurses6:amd64=6.4-2`
- `libncursesw5-dev:amd64=6.4-2`
- `libncursesw6:amd64=6.4-2`
- `libtinfo6:amd64=6.4-2`
- `ncurses-base=6.4-2`
- `ncurses-bin=6.4-2`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

### `dpkg` source package: `nghttp2=1.52.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.52.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `all-permissive`

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.52.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.52.0-1.dsc' nghttp2_1.52.0-1.dsc 2534 SHA512:d9033ae2f9400731d9feb9a4f18b328c9b25499a64702a99c773c4ea69cbe76884713516684ebea2aba975c0ccfdfa5614d41b2bf6c63d8f120133d83b436374
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.52.0.orig.tar.gz' nghttp2_1.52.0.orig.tar.gz 1064232 SHA512:cbd3fbc3e4987ef092d6fe6627eec49a14279f345c555f9b77b791e4ac3b2bd358008e3bb9df86946496b1f6223b30462bb6a4ed4d56703e8e2bf6ce72d5aeac
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.52.0-1.debian.tar.xz' nghttp2_1.52.0-1.debian.tar.xz 11640 SHA512:a79e579fa933d2ed9aa28b59055704a98f3eb0dc95f24ceaad53511e38c6fa48ba29e1a12ee650ac078b8b5d1e380f88bdfa20f66f20d81b81dd91775e26ca53
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

### `dpkg` source package: `numactl=2.0.16-1`

Binary Packages:

- `libnuma1:amd64=2.0.16-1`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.16-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.16-1.dsc' numactl_2.0.16-1.dsc 1980 SHA512:95db6667e50cae559811e6ae8de7793f58251e392dae79a983651094c3e3350ca27f4a90a5cfa90ee07df5bf886bdd4ac31e7c6d5b7f172a01a5eafd1ca966af
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.16.orig.tar.gz' numactl_2.0.16.orig.tar.gz 111144 SHA512:de89bd9f4a9be0e27b21d096aa17a554c209414b5d08b6a2dbd03f8f4830fe4fc5adc88fa8cb08ae1cf75884835dacbde5b6f5d31386244a2582924d2260fcb6
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.16-1.debian.tar.xz' numactl_2.0.16-1.debian.tar.xz 7188 SHA512:1fe8372b070b64dc708a0b89a7c2ec036594610286d625af8b347c4fb5c2c19433e2c8da062de01b54058802d17ec036773b627c8ab3f6428a13d276237059e0
```

### `dpkg` source package: `openexr=3.1.5-4`

Binary Packages:

- `libopenexr-3-1-30:amd64=3.1.5-4`
- `libopenexr-dev=3.1.5-4`

Licenses: (parsed from: `/usr/share/doc/libopenexr-3-1-30/copyright`, `/usr/share/doc/libopenexr-dev/copyright`)

- `BSD-3-clause`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=3.1.5-4
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5-4.dsc' openexr_3.1.5-4.dsc 2506 SHA512:f241f4fecc6f4a03b7de47ddb0d8ebbbb2f4b9a45eda9dcad19fc3bbedbd423f513fe4135c3fd198b19484c0c7269e0ba3b1fd8d72df69cb04ed5bfebc11fca7
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5.orig.tar.gz' openexr_3.1.5.orig.tar.gz 20327926 SHA512:01ef16eacd2dde83c67b81522bae87f47ba272a41ce7d4e35d865dbdcaa03093e7ac504b95d2c1b3a19535f2364a4f937b0e0570c74243bb1c6e021fce7b620c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5.orig.tar.gz.asc' openexr_3.1.5.orig.tar.gz.asc 287 SHA512:9b3978e44b531429aba42b9cc4969a470898d9d74652e3809edb0273ba9b127c471aec6570b5d352be738f59810091c0df2c70d39c16d2c32833d173b270f72c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5-4.debian.tar.xz' openexr_3.1.5-4.debian.tar.xz 18152 SHA512:f6a7a7242a33183262a871ab96a5e4f3137146a83bb9e44bb1e1ee7103b85a8636d797cf7c0e4abe3032a4c59953fdb32360f9772b79561936d98d6f9fb62f59
```

### `dpkg` source package: `openjpeg2=2.5.0-1build1`

Binary Packages:

- `libopenjp2-7:amd64=2.5.0-1build1`
- `libopenjp2-7-dev:amd64=2.5.0-1build1`

Licenses: (parsed from: `/usr/share/doc/libopenjp2-7/copyright`, `/usr/share/doc/libopenjp2-7-dev/copyright`)

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
$ apt-get source -qq --print-uris openjpeg2=2.5.0-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.5.0-1build1.dsc' openjpeg2_2.5.0-1build1.dsc 2697 SHA512:a6fd34c66fd32c32a13dde632eb915cb22822c784b416e3679a313111fe312066f50b706667397f3fcc3f77c666fce05bc9e814067220a375953aee1cf68eea7
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.5.0.orig.tar.xz' openjpeg2_2.5.0.orig.tar.xz 1221108 SHA512:a266297d60ff93e14dbee890b01a76870bda69f082dbe8932fc444ccd260c27aaaac8b22e3c00ca71930b2555a1cad6cf6ed0d5d882d9d13f472cc494cab8234
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.5.0-1build1.debian.tar.xz' openjpeg2_2.5.0-1build1.debian.tar.xz 17412 SHA512:b10d4b1ce14689c35459c7e4899e69e02e1c4cb350fd0a93b1d76603f61b718795bbe878e6d49a6cc60118377721e12a6785dbfff6eac12b4dba259ed7e144e1
```

### `dpkg` source package: `openldap=2.6.3+dfsg-1~exp1ubuntu2`

Binary Packages:

- `libldap2:amd64=2.6.3+dfsg-1~exp1ubuntu2`

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
$ apt-get source -qq --print-uris openldap=2.6.3+dfsg-1~exp1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.3%2bdfsg-1%7eexp1ubuntu2.dsc' openldap_2.6.3+dfsg-1~exp1ubuntu2.dsc 3470 SHA512:f838bd08aaac86b0584ff260b4de496263c28c20f664ff46a2675d507206a6851b64d7f3ffa05615dd1efdfb03462f7b7d17dc616832d301b5b3846fcb0e38aa
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.3%2bdfsg.orig.tar.xz' openldap_2.6.3+dfsg.orig.tar.xz 3741144 SHA512:951b935aa6a3f9dd1c2b7a4a289b6244d605a2a3de248051c8078b8afd5bfaab5943d5c6adddf9e85eb6813db3ddff18478f2c85625df4095ec037bdc579bdc7
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.6.3%2bdfsg-1%7eexp1ubuntu2.debian.tar.xz' openldap_2.6.3+dfsg-1~exp1ubuntu2.debian.tar.xz 179412 SHA512:f305e04594b0153dd68a139736468b1a5eabf94ec39e82a162ce1ff69ec1aa0b7edfce609a6f4cf154a141d7771a85d4b0043aa5e76665281029ee98f74a7f98
```

### `dpkg` source package: `openssh=1:9.0p1-1ubuntu8`

Binary Packages:

- `openssh-client=1:9.0p1-1ubuntu8`

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
$ apt-get source -qq --print-uris openssh=1:9.0p1-1ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1-1ubuntu8.dsc' openssh_9.0p1-1ubuntu8.dsc 3339 SHA512:4db820e83db5064aee6cf9b302bcbd7900c12b7322adfd96b1f681030b62d97084a71ed3cc5b27d10056dead569af6a9fa9200b9db8732b61d1154a973723d58
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1.orig.tar.gz' openssh_9.0p1.orig.tar.gz 1822183 SHA512:613ae95317e734868c6a60d9cc5af47a889baa3124bbdd2b31bb51dd6b57b136f4cfcb5604cca78a03bd500baab9b9b45eaf77e038b1ed776c86dce0437449a9
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1.orig.tar.gz.asc' openssh_9.0p1.orig.tar.gz.asc 833 SHA512:7b1445764058435d2fa8a9c7553643983650d4232036c088e46e44beeb538d32cba88f775b1be9da5f21a01d6caea59b3dc4714507781e9cb946546fa54f169f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1-1ubuntu8.debian.tar.xz' openssh_9.0p1-1ubuntu8.debian.tar.xz 179792 SHA512:5ca349436a7850ed93b98b1740794dd8ce5bd41066e89d78f76b4901860608bbc5fcdec7f0f6101c98b784add2044b3d39fbd2683570a77f259aa966b698c026
```

### `dpkg` source package: `openssl=3.0.7-1ubuntu1`

Binary Packages:

- `libssl-dev:amd64=3.0.7-1ubuntu1`
- `libssl3:amd64=3.0.7-1ubuntu1`
- `openssl=3.0.7-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libssl-dev/copyright`, `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `pango1.0=1.50.12+ds-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.50.12+ds-1`
- `libpangocairo-1.0-0:amd64=1.50.12+ds-1`
- `libpangoft2-1.0-0:amd64=1.50.12+ds-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Apache-2`
- `Apache-2.0`
- `Bitstream-Vera`
- `CC0-1.0`
- `Chromium-BSD-style`
- `Example`
- `GPL-2+`
- `GPL-2.0`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `OFL-1.1`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.50.12+ds-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.12%2bds-1.dsc' pango1.0_1.50.12+ds-1.dsc 3544 SHA512:d5fea8f72b18f153b92bc533897b26442a8ba4faf6ce347237ae3fbda5878cc2b0ee1a605bd3b2c4023c60d8f13df8c0cc98ebfa9e1b692851013e577386b9ef
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.12%2bds.orig.tar.xz' pango1.0_1.50.12+ds.orig.tar.xz 1729376 SHA512:5e5ffefa3c3fcc4351d07f31a005805efeed409fec7fd70d0ac0aefed639b94d5c2b07bd82e036ada2df1f4ed654f65fd8f2762e5d4473ba1a982b6e8bd227cc
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.12%2bds-1.debian.tar.xz' pango1.0_1.50.12+ds-1.debian.tar.xz 41088 SHA512:56e46c0ab5177a2670c21d22839ab1d5f5821e4bce6a692f627950e0ccc98ce9bfe40324783c01484f6f01d4296357b1dd8127f5afe05b4f4dd87b8599b5973f
```

### `dpkg` source package: `patch=2.7.6-7build2`

Binary Packages:

- `patch=2.7.6-7build2`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-7build2
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7build2.dsc' patch_2.7.6-7build2.dsc 1838 SHA512:35ea8fc554a359197cc5ca13dcc3926499563e73e03d8e316d1433d01bc8066e0a138cdab0548d40ec73ee08fe719166c1959793219e798817d69afc94be7665
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA512:fcca87bdb67a88685a8a25597f9e015f5e60197b9a269fa350ae35a7991ed8da553939b4bbc7f7d3cfd863c67142af403b04165633acbce4339056a905e87fbd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7build2.debian.tar.xz' patch_2.7.6-7build2.debian.tar.xz 15248 SHA512:fb482b8f4980bca77a7060aa54cbae01aec9536a72b1e009e9a0cb8f9a35979bf14dcd356b93a2227f18248e81a7e53aac09b7b0d4bd39021681826a9b3ba38f
```

### `dpkg` source package: `pcre2=10.42-1`

Binary Packages:

- `libpcre2-16-0:amd64=10.42-1`
- `libpcre2-32-0:amd64=10.42-1`
- `libpcre2-8-0:amd64=10.42-1`
- `libpcre2-dev:amd64=10.42-1`
- `libpcre2-posix3:amd64=10.42-1`

Licenses: (parsed from: `/usr/share/doc/libpcre2-16-0/copyright`, `/usr/share/doc/libpcre2-32-0/copyright`, `/usr/share/doc/libpcre2-8-0/copyright`, `/usr/share/doc/libpcre2-dev/copyright`, `/usr/share/doc/libpcre2-posix3/copyright`)

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

- `libperl5.36:amd64=5.36.0-7`
- `perl=5.36.0-7`
- `perl-base=5.36.0-7`
- `perl-modules-5.36=5.36.0-7`

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

### `dpkg` source package: `pixman=0.42.2-1`

Binary Packages:

- `libpixman-1-0:amd64=0.42.2-1`
- `libpixman-1-dev:amd64=0.42.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.42.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.42.2-1.dsc' pixman_0.42.2-1.dsc 2021 SHA512:cd8fe22f4c8de60b0966a8100ea3204c321f5223b620a890f5901afdee2030783cd0379e2b4df602c3581120cc2ad28684137e5e34fdc99c795baf32e1cfd959
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.42.2.orig.tar.gz' pixman_0.42.2.orig.tar.gz 959669 SHA512:0a4e327aef89c25f8cb474fbd01de834fd2a1b13fdf7db11ab72072082e45881cd16060673b59d02054b1711ae69c6e2395f6ae9214225ee7153939efcd2fa5d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.42.2-1.diff.gz' pixman_0.42.2-1.diff.gz 319616 SHA512:c475710eace38c80cc59eb1ee6eee9002525fcb30a74e647186601fd1631b09fcafde136fa45618c034be1f75baf2d07f7c78eb92ee4539100fde25f21a834f7
```

### `dpkg` source package: `pkgconf=1.8.1-1ubuntu2`

Binary Packages:

- `libpkgconf3:amd64=1.8.1-1ubuntu2`
- `pkg-config:amd64=1.8.1-1ubuntu2`
- `pkgconf:amd64=1.8.1-1ubuntu2`
- `pkgconf-bin=1.8.1-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libpkgconf3/copyright`, `/usr/share/doc/pkg-config/copyright`, `/usr/share/doc/pkgconf/copyright`, `/usr/share/doc/pkgconf-bin/copyright`)

- `BSD-2`
- `BSD-4`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pkgconf=1.8.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkgconf/pkgconf_1.8.1-1ubuntu2.dsc' pkgconf_1.8.1-1ubuntu2.dsc 2113 SHA512:ef0c195337b5b49d9630d81e888cdde24845dd8c4651cb543a5abd27cda977e75854fa31ad39bd6fbc6ba73fc64a3e46af229b27b48776cb8cbc2c0349a47cb6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkgconf/pkgconf_1.8.1.orig.tar.xz' pkgconf_1.8.1.orig.tar.xz 302372 SHA512:7a7d5204c1c9bfb6578bda56f299d1fa0300e69a133a65730b10ad77aefbf26fceb74ae77cecda326b3ed5db5736f27fcce94764b3a56d40f4bb99fecdc80bba
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkgconf/pkgconf_1.8.1-1ubuntu2.debian.tar.xz' pkgconf_1.8.1-1ubuntu2.debian.tar.xz 15308 SHA512:63dedb498d0a0a6f498a4c7399f489473f4c374d01548637723bf3621fcc261e4bdb58a4453f2d552bc9fb70ce707a11481e57068ca73787589e22b6af0dc07a
```

### `dpkg` source package: `postgresql-15=15.2-1`

Binary Packages:

- `libpq-dev=15.2-1`
- `libpq5:amd64=15.2-1`

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
- `double-metaphone`
- `nagaysau-ishii`

Source:

```console
$ apt-get source -qq --print-uris postgresql-15=15.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-15/postgresql-15_15.2-1.dsc' postgresql-15_15.2-1.dsc 3878 SHA512:4e740fc7eed9e8b238a701b98b905189a2303a604de407e04681c38397634a370679ff751c19de72ccc20830a8d01e7ab69aceb43b35535259a283e063575c05
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-15/postgresql-15_15.2.orig.tar.bz2' postgresql-15_15.2.orig.tar.bz2 22688379 SHA512:115a8a4234791bba4e6dcc4617e9dd77abedcf767894ce9472c59cce9d5d4ef2d4e1746f3a0c7a99de4fc4385fb716652b70dce9f48be45a9db5a682517db7e8
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-15/postgresql-15_15.2-1.debian.tar.xz' postgresql-15_15.2-1.debian.tar.xz 22528 SHA512:eba82f8574be07087fbd9cbebfe4c83240585b104f1fc04ea2e561d380a04e5b216ddc2d244ba73761f3e83c62523b54892863c48cf4734afcf3f0130f0bcb48
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

### `dpkg` source package: `python3-defaults=3.11.1-3`

Binary Packages:

- `libpython3-stdlib:amd64=3.11.1-3`
- `python3=3.11.1-3`
- `python3-minimal=3.11.1-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-defaults/3.11.1-3/


### `dpkg` source package: `python3-stdlib-extensions=3.10.8-1`

Binary Packages:

- `python3-distutils=3.10.8-1`
- `python3-lib2to3=3.10.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-stdlib-extensions/3.10.8-1/


### `dpkg` source package: `python3.11=3.11.1-2`

Binary Packages:

- `libpython3.11-minimal:amd64=3.11.1-2`
- `libpython3.11-stdlib:amd64=3.11.1-2`
- `python3.11=3.11.1-2`
- `python3.11-minimal=3.11.1-2`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3.11/3.11.1-2/


### `dpkg` source package: `readline=8.2-1.3`

Binary Packages:

- `libreadline-dev:amd64=8.2-1.3`
- `libreadline8:amd64=8.2-1.3`
- `readline-common=8.2-1.3`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

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

### `dpkg` source package: `rpcsvc-proto=1.4.2-0ubuntu6`

Binary Packages:

- `rpcsvc-proto=1.4.2-0ubuntu6`

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
$ apt-get source -qq --print-uris rpcsvc-proto=1.4.2-0ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-0ubuntu6.dsc' rpcsvc-proto_1.4.2-0ubuntu6.dsc 2113 SHA512:df8458b423e2d3f8d6da5c6fc19be2ad4ae50d7513e3fa98656b05a734fdc26b2403984ea7da8a0cb5c270f63feae7c258e1f817a3f4a27ffb25107e25f43525
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2.orig.tar.xz' rpcsvc-proto_1.4.2.orig.tar.xz 171620 SHA512:631fbfc00af94c5d7def0759f27e97dc14d400b4468c906719ae18ecef74815730798c882d1aaa4f90359224e7b829019b786baddc3097905b54f940ca85a714
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-0ubuntu6.debian.tar.xz' rpcsvc-proto_1.4.2-0ubuntu6.debian.tar.xz 4268 SHA512:b7ee77b3714b10471fa5be73655f6ce37bd8ca4bfdb07011ac3621723616e69a2323dea9c93ee9ac5d2e9fd0230347224eaa8ae556ec2f2d4b399ec250a5008c
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

### `dpkg` source package: `shared-mime-info=2.2-1`

Binary Packages:

- `shared-mime-info=2.2-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.2-1.dsc' shared-mime-info_2.2-1.dsc 2226 SHA512:fcb8cc0ffe70c71cc1eaded8fa752bcd63c85413a10f65dea9db4d879410fe95107cb3f6945f500d511952ff06994272ba8c583d73618aa71cf6da15ffa4dc23
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.2.orig.tar.bz2' shared-mime-info_2.2.orig.tar.bz2 6428871 SHA512:e32e78435b6bbcdd5abcd1b7708a715d14310f920742e762ce1d4a4f27c1215dbd6493f816d3bf8cf32cf8635a4cee031cf7ea7bad56c4034302273f25da1065
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.2-1.debian.tar.xz' shared-mime-info_2.2-1.debian.tar.xz 10148 SHA512:45f915fdb75cad270f6345e99aaea7f63219096cedda2ae2c395a39c58073a35b6d00033c02e9a16b4ad9c16dd88db232688efa2943958c2911f614c78fb0283
```

### `dpkg` source package: `sqlite3=3.40.1-1`

Binary Packages:

- `libsqlite3-0:amd64=3.40.1-1`
- `libsqlite3-dev:amd64=3.40.1-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

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

### `dpkg` source package: `systemd=252.5-2ubuntu1`

Binary Packages:

- `libsystemd0:amd64=252.5-2ubuntu1`
- `libudev1:amd64=252.5-2ubuntu1`

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


### `dpkg` source package: `sysvinit=3.05-7ubuntu2`

Binary Packages:

- `sysvinit-utils=3.05-7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `tiff=4.5.0-4ubuntu1`

Binary Packages:

- `libtiff-dev:amd64=4.5.0-4ubuntu1`
- `libtiff6:amd64=4.5.0-4ubuntu1`
- `libtiffxx6:amd64=4.5.0-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff6/copyright`, `/usr/share/doc/libtiffxx6/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.5.0-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.5.0-4ubuntu1.dsc' tiff_4.5.0-4ubuntu1.dsc 2368 SHA512:5c8fbe5fdd6d26aed008fc0826b7ceac9576cc57a5a9d0b26ece228f46a3a28a7f0c824b24da182ce307ea4f020a051cedc032486b48a1929b7a3b4adee51230
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.5.0.orig.tar.bz2' tiff_4.5.0.orig.tar.bz2 2050377 SHA512:75da6117546c2a27b6756209435b22ef8a2ca30d84ca30e09ae50a4911bee786c4010dc03636ed6e31c9b3079313efaa7bb383496d12fff3edfb749e5986ad63
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.5.0-4ubuntu1.debian.tar.xz' tiff_4.5.0-4ubuntu1.debian.tar.xz 23000 SHA512:5a0d7e0140a903f163a625e023a4c21e61bc71aa9d1f930bc5f4115a55fccafb4b66b68988297aaf04ffafc3490b93bebf7055e68d9c28a4ad14c3042f9d0b8e
```

### `dpkg` source package: `tzdata=2022g-2ubuntu1`

Binary Packages:

- `tzdata=2022g-2ubuntu1`

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

### `dpkg` source package: `unzip=6.0-27ubuntu1`

Binary Packages:

- `unzip=6.0-27ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-27ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-27ubuntu1.dsc' unzip_6.0-27ubuntu1.dsc 1163 SHA512:7963dfacd662ab3d0bdc7db45435595494e0a7c822a95fc089393b833d49756839fff84db255f26755a6226bffaf899aad13d74000fec0a8836224463df6c319
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA512:0694e403ebc57b37218e00ec1a406cae5cc9c5b52b6798e0d4590840b6cdbf9ddc0d9471f67af783e960f8fa2e620394d51384257dca23d06bcd90224a80ce5d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-27ubuntu1.debian.tar.xz' unzip_6.0-27ubuntu1.debian.tar.xz 28316 SHA512:b9df6697190a6a072c9aaf388bd7eeae1e86d6b8f268d3fcc1e40c5da4423378240bebbb3a05a670cdc1213d251118b6b1dff8788fd57bc55ac1265ccf0f7c11
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

### `dpkg` source package: `util-linux=2.38.1-4ubuntu1`

Binary Packages:

- `bsdutils=1:2.38.1-4ubuntu1`
- `libblkid-dev:amd64=2.38.1-4ubuntu1`
- `libblkid1:amd64=2.38.1-4ubuntu1`
- `libmount-dev:amd64=2.38.1-4ubuntu1`
- `libmount1:amd64=2.38.1-4ubuntu1`
- `libsmartcols1:amd64=2.38.1-4ubuntu1`
- `libuuid1:amd64=2.38.1-4ubuntu1`
- `mount=2.38.1-4ubuntu1`
- `util-linux=2.38.1-4ubuntu1`
- `util-linux-extra=2.38.1-4ubuntu1`
- `uuid-dev:amd64=2.38.1-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/util-linux-extra/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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

### `dpkg` source package: `x265=3.5-2`

Binary Packages:

- `libx265-199:amd64=3.5-2`

Licenses: (parsed from: `/usr/share/doc/libx265-199/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=3.5-2
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_3.5-2.dsc' x265_3.5-2.dsc 2234 SHA512:040a0cc2ffbdc27f45721e3c2dcd233e37e049a639ed399a337e075ce1cd0892fe2d2919e4164e0007bc01de446f05e8515403396f0c4e273f5c0e850fd30c74
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_3.5.orig.tar.gz' x265_3.5.orig.tar.gz 1537044 SHA512:230e683239c3e262096ba96246c6f67229a1625d163f86647a411733bb1cf349685858aee3017bce818bb6992448d0abaa9241615a5b620561ce47ecb164f997
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_3.5-2.debian.tar.xz' x265_3.5-2.debian.tar.xz 13536 SHA512:13da56dd92cec1f2af147049a690135d2361c12819308f87e09ce2a358e32c032eb7afa83bac6da9c4e881cdfbec970c41790b5ab027a9a5c3aee01e33f69fcc
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

### `dpkg` source package: `xorg=1:7.7+23ubuntu2`

Binary Packages:

- `x11-common=1:7.7+23ubuntu2`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+23ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7%2b23ubuntu2.dsc' xorg_7.7+23ubuntu2.dsc 2095 SHA512:f4befc0dd73c66f56856f16c4dc4051f58af50bd8819469df4bb309817952e00f2f4e29776282f85eeaef18a77fdd42cb1cfcb9a69432c4680b216039b37e480
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7%2b23ubuntu2.tar.gz' xorg_7.7+23ubuntu2.tar.gz 301762 SHA512:379e60ab57cc4f9adbf1f59295fca3930bbd638f4100d08c9f1f78bd6ef063e3396385b841e66389771c4ba5825875d738b9aa4b4dc2e3f79d0537415ac0852a
```

### `dpkg` source package: `xorgproto=2022.1-1`

Binary Packages:

- `x11proto-core-dev=2022.1-1`
- `x11proto-dev=2022.1-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2022.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2022.1-1.dsc' xorgproto_2022.1-1.dsc 3410 SHA512:cd5dae5e527d42a2d54eb1adf2028af45462567849937d740fd9e46f9c8f080264c49928d44300ea4d4e77978292b57513c9112054da6da17bd02068f61c5d37
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2022.1.orig.tar.gz' xorgproto_2022.1.orig.tar.gz 1107316 SHA512:e34404eb9f7edfebdecbf38c66491fbca91929c59b5762d3266b2808cdae3f4e65589001d29bf5374effc56173a5467f5a107bf4fe05acae69839b841e83f72c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2022.1.orig.tar.gz.asc' xorgproto_2022.1.orig.tar.gz.asc 195 SHA512:8a975a43434c40af2cdc781aad4dbb8ff2d1730fe6a04b431800d19a81b1fbf53e29503f8226c6579d7335c7250842b4c6eb5e8ee4f1b0f08bb7e87b12b50b3c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2022.1-1.diff.gz' xorgproto_2022.1-1.diff.gz 23288 SHA512:062da8e99882e4b3a6527ec92fb1faace09a7586c30a699af13be1b4f00af076e9d60054e2f61e21425203c5175a51f919dcea81a8e7b0562a8b8eb341b1dc77
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

- `liblzma-dev:amd64=5.4.1-0.0`
- `liblzma5:amd64=5.4.1-0.0`
- `xz-utils=5.4.1-0.0`

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

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/xz-utils/5.4.1-0.0/


### `dpkg` source package: `zlib=1:1.2.13.dfsg-1ubuntu4`

Binary Packages:

- `zlib1g:amd64=1:1.2.13.dfsg-1ubuntu4`
- `zlib1g-dev:amd64=1:1.2.13.dfsg-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.13.dfsg-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu4.dsc' zlib_1.2.13.dfsg-1ubuntu4.dsc 2972 SHA512:0ef70f7a1ee27e9d414001d67497f14014e188b90a4615fb2a955c96f7997bc36d6a5931c63e733d5ebefa87bbfdcdd6810a1278c210a39a7c1fc43df6ca4edc
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg.orig.tar.bz2' zlib_1.2.13.dfsg.orig.tar.bz2 1239825 SHA512:266ea72465ad1f0b63e42f8275c650615829929f2ff19064144c5bb942acd31cd8581ce45781c438fce949c6d9f3fa385efa59f754761441107ca1144fb56802
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu4.debian.tar.xz' zlib_1.2.13.dfsg-1ubuntu4.debian.tar.xz 57960 SHA512:312357388a757db8f3588f637a3d016f28fbff89fed2bb882a4972f5f838e39129fcb01d77cbd0ba9ec3e65fbc993e9f0c4e11acb298894dc6350fb9b1e2d7ca
```
