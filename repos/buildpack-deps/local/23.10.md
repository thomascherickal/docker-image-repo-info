# `buildpack-deps:mantic`

## Docker Metadata

- Image ID: `sha256:bfef5d2082eaa961e2d3cefef8e67a7d13c9269c329297040dd1ca2d2360b92f`
- Created: `2023-12-02T04:26:15.051172148Z`
- Virtual Size: ~ 789.39 Mb  
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

### `dpkg` source package: `binutils=2.41-5ubuntu1`

Binary Packages:

- `binutils=2.41-5ubuntu1`
- `binutils-common:amd64=2.41-5ubuntu1`
- `binutils-x86-64-linux-gnu=2.41-5ubuntu1`
- `libbinutils:amd64=2.41-5ubuntu1`
- `libctf-nobfd0:amd64=2.41-5ubuntu1`
- `libctf0:amd64=2.41-5ubuntu1`
- `libgprofng0:amd64=2.41-5ubuntu1`
- `libsframe1:amd64=2.41-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`, `/usr/share/doc/libgprofng0/copyright`, `/usr/share/doc/libsframe1/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.41-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.41-5ubuntu1.dsc' binutils_2.41-5ubuntu1.dsc 9687 SHA512:cd0fc39618048e85364666297e7b89ec44985f6532cd76bd91769ae8ab182ce068edde293655c72392b5affa4313227fcc518695b831012143498f53c725be0c
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.41.orig.tar.xz' binutils_2.41.orig.tar.xz 26765692 SHA512:5df45d0bd6ddabdce4f35878c041e46a92deef01e7dea5facc97fd65cc06b59abc6fba0eb454b68e571c7e14038dc823fe7f2263843e6e627b7444eaf0fe9374
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.41-5ubuntu1.debian.tar.xz' binutils_2.41-5ubuntu1.debian.tar.xz 197056 SHA512:b1edb1fea3e46bd8e2e955ecee9347c9860ecacab37ac84c69a6758f1b6c52a25b2f7dc12a53840c1efddece8171a44a3159132582e17f97cbde3acd1aa3dedc
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

### `dpkg` source package: `cairo=1.18.0-1`

Binary Packages:

- `libcairo-gobject2:amd64=1.18.0-1`
- `libcairo-script-interpreter2:amd64=1.18.0-1`
- `libcairo2:amd64=1.18.0-1`
- `libcairo2-dev:amd64=1.18.0-1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.18.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.18.0-1.dsc' cairo_1.18.0-1.dsc 2772 SHA512:93d53a43e9fc5979ebfac817aa5cf36b884f65b04d666cfc39a5514095de677d98292f594e3cc5d46df074a9bf2c36f61bed391b807f02d126c1bbc7608037a0
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.18.0.orig.tar.xz' cairo_1.18.0.orig.tar.xz 33761148 SHA512:6366c7d5e3fd3e12df2edc43aa4ed4c3a517de2ef0b1b3b30dfa8b69a7cae1dd55765801228cec308d2e9792037d0704ae49d95b7b12c06f20df092fa0534e1c
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.18.0-1.debian.tar.xz' cairo_1.18.0-1.debian.tar.xz 29720 SHA512:da10f9f9282d9467bf6097f9102265c0d219ee51912ed4d8f788b76b4f0d96c987ac735253d54df913f79ee1ab184805fc59783a5966bdc6f024d5ac8b360a11
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
- `libcurl3-gnutls:amd64=8.2.1-1ubuntu3.1`
- `libcurl4:amd64=8.2.1-1ubuntu3.1`
- `libcurl4-openssl-dev:amd64=8.2.1-1ubuntu3.1`

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
- `OLDAP-2.8`
- `X11`
- `curl`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `dav1d=1.2.1-2`

Binary Packages:

- `libdav1d6:amd64=1.2.1-2`

Licenses: (parsed from: `/usr/share/doc/libdav1d6/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dav1d=1.2.1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.2.1-2.dsc' dav1d_1.2.1-2.dsc 2287 SHA512:387d5151ceb8018bf9002df7f560caafcaca43a6d5740f31f97ef47a36fc5d5595077d635d2951faac0241c3151df37c65a708a5990e57b65c1b4cccac0c4087
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.2.1.orig.tar.xz' dav1d_1.2.1.orig.tar.xz 873008 SHA512:f172eebc0a5f6c51d31fc9e9758c2dd0de51d8a5d0e00c93a5f2b1b16b7b4a37b365f9c56dea95d400e66b63af5fa4c63d9e720719ac38852777fc8c6066e4a7
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.2.1.orig.tar.xz.asc' dav1d_1.2.1.orig.tar.xz.asc 195 SHA512:52289cc6ea15be13bbcf04349c4f2a7c2dae60a52c5a9ec3557aea78b929c5fdfc09a3228b9980f8f024b6d8203fd9ef5e0b1080a6c20c3d1c7a30d19f803973
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_1.2.1-2.debian.tar.xz' dav1d_1.2.1-2.debian.tar.xz 8156 SHA512:4e8ae8ce9d417e1f253766f45259bd64370884d3d178e75419c8d417180c0e14d1ca2f2f662638f8b246dbc62b4cad4ad44229a9550cfc8c367b25e500747c7e
```

### `dpkg` source package: `db-defaults=1:5.3.21ubuntu1`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21ubuntu1.dsc' db-defaults_5.3.21ubuntu1.dsc 1580 SHA512:df7ecb38474c44f16e41b6bf0fa637268ae6cacb315f6c4cd3d620c7007ff4c178257460b125c4d7360dbfd599d1d6f13d242a80e638f0a72f3df0affcd04738
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21ubuntu1.tar.xz' db-defaults_5.3.21ubuntu1.tar.xz 2528 SHA512:4b7e2ddcdedb904861fe89e27c1acdce70f9a224e0f48ff6a34adeea9d6312b602e7dbf03da56d32d4fc02ac6ec66714988cea27000bc190ee438f76bfbfd8ee
```

### `dpkg` source package: `db5.3=5.3.28+dfsg2-2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg2-2`
- `libdb5.3-dev=5.3.28+dfsg2-2`

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

### `dpkg` source package: `dpkg=1.22.0ubuntu1`

Binary Packages:

- `dpkg=1.22.0ubuntu1`
- `dpkg-dev=1.22.0ubuntu1`
- `libdpkg-perl=1.22.0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

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

- `comerr-dev:amd64=2.1-1.47.0-2ubuntu1`
- `e2fsprogs=1.47.0-2ubuntu1`
- `libcom-err2:amd64=1.47.0-2ubuntu1`
- `libext2fs2:amd64=1.47.0-2ubuntu1`
- `libss2:amd64=1.47.0-2ubuntu1`
- `logsave=1.47.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

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

### `dpkg` source package: `elfutils=0.189-4`

Binary Packages:

- `libelf1:amd64=0.189-4`

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
$ apt-get source -qq --print-uris elfutils=0.189-4
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.189-4.dsc' elfutils_0.189-4.dsc 3248 SHA512:b03c9333a26f7eb734048d32f00ac6165059b70e3ebc431aedb825ed5d67f0799793e1f8f4fcc15fc68906eba92b400f4a9c9830cbd311f97ad38d10420eef66
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.189.orig.tar.bz2' elfutils_0.189.orig.tar.bz2 9143169 SHA512:93a877e34db93e5498581d0ab2d702b08c0d87e4cafd9cec9d6636dfa85a168095c305c11583a5b0fb79374dd93bc8d0e9ce6016e6c172764bcea12861605b71
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.189-4.debian.tar.xz' elfutils_0.189-4.debian.tar.xz 43208 SHA512:81406396d3707e5c5b4665d5dd1fc18356fafcf1d26e46ebb752eecd7274e062dc6c93e44dd2becff1fe8151c533f90ac3d5457295bb023283d24ffc825c10d3
```

### `dpkg` source package: `expat=2.5.0-2`

Binary Packages:

- `libexpat1:amd64=2.5.0-2`
- `libexpat1-dev:amd64=2.5.0-2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.5.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0-2.dsc' expat_2.5.0-2.dsc 1964 SHA512:a71f12ab67b948e890dd1d7e00339acb22cef4f834bc2cd26cbfc04eb5e0d65d56a22e41d384394862104e2e8da0309f4029b059a7adcfdc2d0b0d1acc64ca28
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0.orig.tar.gz' expat_2.5.0.orig.tar.gz 8320988 SHA512:779f0d0f3f2d8b33db0fd044864ab5ab1a40f20501f792fe90ad0d18de536c4765c3749f120e21fec11a0e6c89af1dc576d1fe261c871ca44a594f7b61fd1d9e
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.5.0-2.debian.tar.xz' expat_2.5.0-2.debian.tar.xz 12804 SHA512:3603f3f3f3e4f0bc2c7a29a25aa7c9681ff4a93d48b7e5fabb0d58f8e048c3d7eb0487140f813bd925c4cb2b956a3bd2f68d8c3d75f79066624d83445739cb57
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

### `dpkg` source package: `fontconfig=2.14.2-4ubuntu1`

Binary Packages:

- `fontconfig=2.14.2-4ubuntu1`
- `fontconfig-config=2.14.2-4ubuntu1`
- `libfontconfig-dev:amd64=2.14.2-4ubuntu1`
- `libfontconfig1:amd64=2.14.2-4ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.14.2-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.14.2-4ubuntu1.dsc' fontconfig_2.14.2-4ubuntu1.dsc 2430 SHA512:c727a4b4fbb1707fd993b9de35ab46c28ea1ebcb5a27cd78747cfbd5b19aadefd5a5e03c0b6cb1a0edf7b78a3a7d5f1d57a3303f8ab3f50255109d9eab7a218c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.14.2.orig.tar.xz' fontconfig_2.14.2.orig.tar.xz 1440844 SHA512:23483e0ae6aa7589fd37f9949a4cf951c5bff981739dbb446881e4cea86a208c0ab31e2358666eac724af1dc6a689a42733a7ce91cd3e76d8d91eacedb318085
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.14.2-4ubuntu1.debian.tar.xz' fontconfig_2.14.2-4ubuntu1.debian.tar.xz 29108 SHA512:920f2b352d3a6871e044e31062d3a3928b43e53c1a8f518135927d09f371c139f21ce29178a04a1f3aea73a0de2743f23bbb81c44fe953a5d52d05d564ea2541
```

### `dpkg` source package: `fonts-noto=20201225-2`

Binary Packages:

- `fonts-noto-core=20201225-2`
- `fonts-noto-mono=20201225-2`

Licenses: (parsed from: `/usr/share/doc/fonts-noto-core/copyright`, `/usr/share/doc/fonts-noto-mono/copyright`)

- `GPL-3`
- `GPL-3+`
- `OFL-1.1`

Source:

```console
$ apt-get source -qq --print-uris fonts-noto=20201225-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-noto/fonts-noto_20201225-2.dsc' fonts-noto_20201225-2.dsc 2377 SHA512:36234e61f8c356b83a89609872c184592084e4c56edbadad3181068f7f21464b8542d1bca9b9a4083762310b0970904a5a0e1c43b30876ec2807f5c663b29913
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-noto/fonts-noto_20201225.orig.tar.gz' fonts-noto_20201225.orig.tar.gz 903613276 SHA512:240ae214729388e7000a4e12a1fc81b0b562ca6f3fcb4fcdef66a27c1b193825fbf2d0fd4cc8fbae4cd17f57e21fd1589150cb02b7b618d670742692b748f9ff
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-noto/fonts-noto_20201225-2.debian.tar.xz' fonts-noto_20201225-2.debian.tar.xz 110764 SHA512:409610ac8c3ff677578a11f18da8fee6141aee74cad264bcbed65cd3f4c389704eafcac57f2913058f5d62f523ebd39b968b6f17b6a2aae4875953817ec378c3
```

### `dpkg` source package: `freetype=2.13.1+dfsg-1`

Binary Packages:

- `libfreetype-dev:amd64=2.13.1+dfsg-1`
- `libfreetype6:amd64=2.13.1+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`)

- `BSD-3-Clause`
- `BSL-1.0`
- `Expat`
- `FSFAP`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT-Modern-Variant`
- `MIT-SMC`
- `OpenGroup-MIT`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.13.1+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.13.1%2bdfsg-1.dsc' freetype_2.13.1+dfsg-1.dsc 3686 SHA512:4895ec7f089fc7996f111ed2ec41f9604887ce2cab5009635528478f4a3c27852e7810a851983315176f30bcf146769a1345300cf34bebb399068bb03e2f185c
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.13.1%2bdfsg.orig-ft2demos.tar.xz' freetype_2.13.1+dfsg.orig-ft2demos.tar.xz 339736 SHA512:c03205266a420c589eec2a95ca082ab1c5606215a477500fe1a2f31c2f30c327a61e1fececec4ca3268f1a8b92a0bc8310bacf26f276ec09062fa5c5b0878511
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.13.1%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.13.1+dfsg.orig-ft2demos.tar.xz.asc 833 SHA512:ad8460a919e1c6d42c16f17a5c6b8129c1b251ecb1221d3414e1365e5e616371499c0668e6fda5564f0035dfb484261db4ea88fdcaebca42135056fdc0a1d3d5
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.13.1%2bdfsg.orig-ft2docs.tar.xz' freetype_2.13.1+dfsg.orig-ft2docs.tar.xz 2173864 SHA512:e18f0851c52689628fb7fa520c6165895650412bfe1ebab8417bf5738d5cc7d1877e78e4afbede0996938f33554f53a0ea7b837fe81497a12b10daae5b8829ed
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.13.1%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.13.1+dfsg.orig-ft2docs.tar.xz.asc 833 SHA512:3250509e01b51bb3f0db62c943f35f83a8a3ff87cffa4b0b77e6836c192ac2711b1dcef04d0496799e466a1e3a631aa8d524513a8dcd4771728ddd2d15e43463
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.13.1%2bdfsg.orig.tar.xz' freetype_2.13.1+dfsg.orig.tar.xz 2224144 SHA512:d858b6eb1b1a6374e3cd9db89849750d100c74781bbc32f7483346febbf2118c3abca8d9f83fb2575c8609f8a7dc9379d7c64f7c928b3da6f72ff6fa57a83520
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.13.1%2bdfsg-1.debian.tar.xz' freetype_2.13.1+dfsg-1.debian.tar.xz 44484 SHA512:92b8cd686ce5f7058283fe320f9ed5c42ad2721562cb966d7308296fc126251b618dbf5c39d5250858fda82eead3e068f2fa426df2fbfba3d71aa25a4fd5cae3
```

### `dpkg` source package: `fribidi=1.0.13-3`

Binary Packages:

- `libfribidi0:amd64=1.0.13-3`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.13-3
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.13-3.dsc' fribidi_1.0.13-3.dsc 2007 SHA512:801485436ef071306696f6c3db7dcad61d1e39c1cf4bb213aebe2ca13541dfa03f0751337c5b9ff3ec3719bfd5736e00c53a211f8c619541beb95f2fd2d3e5bc
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.13.orig.tar.xz' fribidi_1.0.13.orig.tar.xz 1170100 SHA512:09357d842ff9e05b918f826e28e4a25ad996e17f73242ee9ce53fae9f37ec6c639f9cae4271577f6e0269f34265afc893858225c4a94610f0a6ee7580fb1fe07
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.13-3.debian.tar.xz' fribidi_1.0.13-3.debian.tar.xz 8848 SHA512:fa9aa25785d36b7a08fe06314ea66b7bd8913df456fbdd2fe4be7e44910be1efe023de413bbe35e56383b2f9b35e71eae6d73b2ff7a168e32ed036e9f3877d8c
```

### `dpkg` source package: `gcc-13=13.2.0-4ubuntu3`

Binary Packages:

- `cpp-13=13.2.0-4ubuntu3`
- `g++-13=13.2.0-4ubuntu3`
- `gcc-13=13.2.0-4ubuntu3`
- `gcc-13-base:amd64=13.2.0-4ubuntu3`
- `libasan8:amd64=13.2.0-4ubuntu3`
- `libatomic1:amd64=13.2.0-4ubuntu3`
- `libcc1-0:amd64=13.2.0-4ubuntu3`
- `libgcc-13-dev:amd64=13.2.0-4ubuntu3`
- `libgcc-s1:amd64=13.2.0-4ubuntu3`
- `libgomp1:amd64=13.2.0-4ubuntu3`
- `libhwasan0:amd64=13.2.0-4ubuntu3`
- `libitm1:amd64=13.2.0-4ubuntu3`
- `liblsan0:amd64=13.2.0-4ubuntu3`
- `libquadmath0:amd64=13.2.0-4ubuntu3`
- `libstdc++-13-dev:amd64=13.2.0-4ubuntu3`
- `libstdc++6:amd64=13.2.0-4ubuntu3`
- `libtsan2:amd64=13.2.0-4ubuntu3`
- `libubsan1:amd64=13.2.0-4ubuntu3`

Licenses: (parsed from: `/usr/share/doc/cpp-13/copyright`, `/usr/share/doc/g++-13/copyright`, `/usr/share/doc/gcc-13/copyright`, `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libasan8/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-13-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libhwasan0/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-13-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan2/copyright`, `/usr/share/doc/libubsan1/copyright`)

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

### `dpkg` source package: `gcc-defaults=1.208ubuntu1`

Binary Packages:

- `cpp=4:13.2.0-1ubuntu1`
- `g++=4:13.2.0-1ubuntu1`
- `gcc=4:13.2.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.208ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.208ubuntu1.dsc' gcc-defaults_1.208ubuntu1.dsc 15382 SHA512:d2f6528fe006b7458b442e436d22ab694cff71aeaf11280b08dbcd49b4bd6bfc53992cbe139ebe6cb0b136d82a8ac591b43a1850ba26fb60769226d58682d244
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.208ubuntu1.tar.xz' gcc-defaults_1.208ubuntu1.tar.xz 48484 SHA512:05508b543921888f991d677f3670ea1a53e71b749cc9c9faa8e637738cead2faa1c48b9f7201b1a07a1b1d302fb47f058cbb135d360204514918730806f684b8
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

### `dpkg` source package: `glib2.0=2.78.0-2`

Binary Packages:

- `libglib2.0-0:amd64=2.78.0-2`
- `libglib2.0-bin=2.78.0-2`
- `libglib2.0-data=2.78.0-2`
- `libglib2.0-dev:amd64=2.78.0-2`
- `libglib2.0-dev-bin=2.78.0-2`

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
$ apt-get source -qq --print-uris glib2.0=2.78.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.78.0-2.dsc' glib2.0_2.78.0-2.dsc 3684 SHA512:f37193e9763f96fa2cc3c7a754445d1adfdf216be63407ccd0a36f280745bd666eefeb10f557c712faa8ca7f94e0c5be0b3189201160deac54d61dc8773c6cfe
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.78.0.orig-unicode-data.tar.xz' glib2.0_2.78.0.orig-unicode-data.tar.xz 266184 SHA512:c818eae7b8df69b69abc2c59870eaad7488e3266afb5055b851fcbdd9dd96d9808787881631a8d840487acb3b40c18691b6c58d3df4735fa6eab41a5aa1295ff
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.78.0.orig.tar.xz' glib2.0_2.78.0.orig.tar.xz 5327096 SHA512:3d06890002f4b13f831c83fbb70cfce529f9750e30888619e4d6277116be15d106379a03143412cf4b2a289c0cbdbbc299ecf17284fbffc06c791ecf7556c765
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.78.0-2.debian.tar.xz' glib2.0_2.78.0-2.debian.tar.xz 202588 SHA512:36155efbd8cc7513267d901f0e5df56d9b22d20a0f91c37041de05b61b8391aca989ca7eabf5ec26fabb096856fbdeb41f25b6543d84cf8dbb3912fd31e39e69
```

### `dpkg` source package: `glibc=2.38-1ubuntu6`

Binary Packages:

- `libc-bin=2.38-1ubuntu6`
- `libc-dev-bin=2.38-1ubuntu6`
- `libc6:amd64=2.38-1ubuntu6`
- `libc6-dev:amd64=2.38-1ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

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

- `libgmp-dev:amd64=2:6.3.0+dfsg-2ubuntu4`
- `libgmp10:amd64=2:6.3.0+dfsg-2ubuntu4`
- `libgmpxx4ldbl:amd64=2:6.3.0+dfsg-2ubuntu4`

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

### `dpkg` source package: `gobject-introspection=1.78.1-1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.78.1-1`
- `gir1.2-glib-2.0:amd64=1.78.1-1`
- `libgirepository-1.0-1:amd64=1.78.1-1`

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
$ apt-get source -qq --print-uris gobject-introspection=1.78.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.78.1-1.dsc' gobject-introspection_1.78.1-1.dsc 3392 SHA512:76d2bad3abdd68016f64a9a081d806ad2277a9d9b593932f3425f5cfd9c445f883ddb3bbcbfa2c7b3769b7d0a409c05f35eaedace107af8ae588ed769a9c7d59
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.78.1.orig-glib.tar.xz' gobject-introspection_1.78.1.orig-glib.tar.xz 5327096 SHA512:3d06890002f4b13f831c83fbb70cfce529f9750e30888619e4d6277116be15d106379a03143412cf4b2a289c0cbdbbc299ecf17284fbffc06c791ecf7556c765
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.78.1.orig.tar.xz' gobject-introspection_1.78.1.orig.tar.xz 1060296 SHA512:a3081882995a762645b04faa71082dbd523bee845519007e48b13235aad8a4cd4c74f0d042a6c17710125f945bd970e4b76e95a559274e294d595e04725a4e97
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.78.1-1.debian.tar.xz' gobject-introspection_1.78.1-1.debian.tar.xz 40408 SHA512:456fe7b535748901bea4ead978b81cb01029f2d47222f52a6514fa63097f6d222e709d45bcaece762638bb64fe0188dc33d595cc2b712ecd81e00ba58b85a559
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

### `dpkg` source package: `harfbuzz=8.0.1-1`

Binary Packages:

- `libharfbuzz0b:amd64=8.0.1-1`

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
$ apt-get source -qq --print-uris harfbuzz=8.0.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_8.0.1-1.dsc' harfbuzz_8.0.1-1.dsc 2542 SHA512:6065ae973b29c596e3a7fb3d1e4a6e7371cb31ec887040203813156180f8a29f5d9696e26eaf21020db7dd7f47bbd582bf765179c3fa9a3df86edd2a0f248305
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_8.0.1.orig.tar.xz' harfbuzz_8.0.1.orig.tar.xz 18792332 SHA512:e1292f059b07a5aa2f3fbf345b893209cac895c461b4abf30b8b76bcd03c79dd09f911450293403070e1a0bb08496a7f37693ba5a62a9d423dd6ba55e744444d
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_8.0.1-1.debian.tar.xz' harfbuzz_8.0.1-1.debian.tar.xz 19644 SHA512:e7430bacc4eb9cb275e8aabf3f7115662143886f996ae39214390da9e403b067c4c3fe3205dddfc4c895f46d30ba31b44f67f216eaf36429d1fbe72e7b03134b
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

### `dpkg` source package: `icu=72.1-3ubuntu3`

Binary Packages:

- `icu-devtools=72.1-3ubuntu3`
- `libicu-dev:amd64=72.1-3ubuntu3`
- `libicu72:amd64=72.1-3ubuntu3`

Licenses: (parsed from: `/usr/share/doc/icu-devtools/copyright`, `/usr/share/doc/libicu-dev/copyright`, `/usr/share/doc/libicu72/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu=72.1-3ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1-3ubuntu3.dsc' icu_72.1-3ubuntu3.dsc 2359 SHA512:4345ac6b4fe35e4d9e23100002fa255cc5b569c61f968d047c10bdb6e66eb4bed6d15043af6c80dce613517bea2c9d203b0ded729c47c2dc073fd9eae83d082d
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1.orig.tar.gz' icu_72.1.orig.tar.gz 26303933 SHA512:848c341b37c0ff077e34a95d92c6200d5aaddd0ee5e06134101a74e04deb08256a5e817c8aefab020986abe810b7827dd7b2169a60dacd250c298870518dcae8
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1.orig.tar.gz.asc' icu_72.1.orig.tar.gz.asc 659 SHA512:8b5e841a3baa317a13cadf7deb3582a80cfab8e5bdae6bd04612ee7be3006d9acf07b015de01a94990fa350109a3c11e547482e4cb4ca986161cc701a8cd427b
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_72.1-3ubuntu3.debian.tar.xz' icu_72.1-3ubuntu3.debian.tar.xz 64708 SHA512:31d09726ba3d81aaf7beb8537982187080b2c61587ba922bdceb4c80499e415f9eaf86d2418e7fc4956c7369a7970e58d53cf3694c042639b441d8cb88aa66c8
```

### `dpkg` source package: `imagemagick=8:6.9.11.60+dfsg-1.6ubuntu1`

Binary Packages:

- `imagemagick=8:6.9.11.60+dfsg-1.6ubuntu1`
- `imagemagick-6-common=8:6.9.11.60+dfsg-1.6ubuntu1`
- `imagemagick-6.q16=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickcore-6-arch-config:amd64=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickcore-6-headers=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickcore-6.q16-6:amd64=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickcore-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickcore-dev=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickwand-6-headers=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickwand-6.q16-6:amd64=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickwand-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.6ubuntu1`
- `libmagickwand-dev=8:6.9.11.60+dfsg-1.6ubuntu1`

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.11.60+dfsg-1.6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1.6ubuntu1.dsc' imagemagick_6.9.11.60+dfsg-1.6ubuntu1.dsc 5181 SHA512:ae83028055840700dd8f6ff93e1d15a2ea325353800884fde1318c3b9c73a2c165191739b306bd9776fa8dd59f82f5c77845817e9c15bb6261fda998c8795be8
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg.orig.tar.xz' imagemagick_6.9.11.60+dfsg.orig.tar.xz 9395144 SHA512:345a23eda96516fc7a213bd4a322bca4c8b690efe40ff7b498a448f8cedd7f0d600fae2cb6fff45bc995779a90d8c04b58288273eee97833ddebb4f9f2a3d14c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1.6ubuntu1.debian.tar.xz' imagemagick_6.9.11.60+dfsg-1.6ubuntu1.debian.tar.xz 259460 SHA512:b14064854623591a848cb6ab57b550e9d864d2971497ec48d5c7a9e23d9ae4eae6ab297ea30b00175e947fc1ffc46463ae683423bba83728ce078f13a5502afa
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

### `dpkg` source package: `isl=0.26-3`

Binary Packages:

- `libisl23:amd64=0.26-3`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.26-3
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.26-3.dsc' isl_0.26-3.dsc 1832 SHA512:83773ff0dc5e4f909530a9fee6c2ebed113bf1493f335ed44aaddb530dae55cfad31ad6f1b4c5426eecb7304d5ec159bab60edff4557ca5ef82f3bf1ca6e36e3
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.26.orig.tar.xz' isl_0.26.orig.tar.xz 2035560 SHA512:9b5ec16d14e48f9ac9bf9cd379d3022959cfc617ade9e0d4caf2862299564fecba09d67dbdf1a4071f2f743a4fd0fabd0b0c3d15f5cddfe7226cdd5d6c2a0c66
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.26-3.debian.tar.xz' isl_0.26-3.debian.tar.xz 24700 SHA512:23944f19bbc74fb546c6a0183c74605a038241eec1be2494f5ed2e3734c99d2484cbc4eac1168bd115a01651ab5a07138d1f4e75876c0f1836dd98f389a05616
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

### `dpkg` source package: `jbigkit=2.1-6.1ubuntu1`

Binary Packages:

- `libjbig-dev:amd64=2.1-6.1ubuntu1`
- `libjbig0:amd64=2.1-6.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-6.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-6.1ubuntu1.dsc' jbigkit_2.1-6.1ubuntu1.dsc 2207 SHA512:0559e2551f3ca1106e89a7f2482a17c50ebe886b8d699f1387b6ca032408cdd7976f78871a2da6e16a310035ba1e709f75f0399f1305c098aebed84883e3a816
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA512:c4127480470ef90db1ef3bd2caa444df10b50ed8df0bc9997db7612cb48b49278baf44965028f1807a21028eb965d677e015466306b44683c4ec75a23e1922cf
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-6.1ubuntu1.debian.tar.xz' jbigkit_2.1-6.1ubuntu1.debian.tar.xz 11092 SHA512:74ea1ca6d2e5b4e624382c60ef08dcfc91a2babb0433747dd464283459989d5441f77df2878462d7ff15b6cd98dac530b0483bef0be08062e175bc24c8e4374a
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

- `krb5-multidev:amd64=1.20.1-3ubuntu1`
- `libgssapi-krb5-2:amd64=1.20.1-3ubuntu1`
- `libgssrpc4:amd64=1.20.1-3ubuntu1`
- `libk5crypto3:amd64=1.20.1-3ubuntu1`
- `libkadm5clnt-mit12:amd64=1.20.1-3ubuntu1`
- `libkadm5srv-mit12:amd64=1.20.1-3ubuntu1`
- `libkdb5-10:amd64=1.20.1-3ubuntu1`
- `libkrb5-3:amd64=1.20.1-3ubuntu1`
- `libkrb5-dev:amd64=1.20.1-3ubuntu1`
- `libkrb5support0:amd64=1.20.1-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit12/copyright`, `/usr/share/doc/libkadm5srv-mit12/copyright`, `/usr/share/doc/libkdb5-10/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20.1-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-3ubuntu1.dsc' krb5_1.20.1-3ubuntu1.dsc 3920 SHA512:c9dfc58de924bef20e55cd82232a776e555c6c3f251929c169511d10c62844f4a8fe7f44cc73c39faaa095bdea567c1fcfd6a3ace63bb49b626676650c65553a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz' krb5_1.20.1.orig.tar.gz 8661660 SHA512:6f57479f13f107cd84f30de5c758eb6b9fc59171329c13e5da6073b806755f8d163eb7bd84767ea861ad6458ea0c9eeb00ee044d3bcad01ef136e9888564b6a2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz.asc' krb5_1.20.1.orig.tar.gz.asc 833 SHA512:1d3312bd67581e07adfdadf2c5fe394179631d8add8bd075efefe982a0de22369004e60a14422d426382c8c591e4181b9897088afe9d4e86f0b5a97e5954c67a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.20.1-3ubuntu1.debian.tar.xz' krb5_1.20.1-3ubuntu1.debian.tar.xz 100536 SHA512:39ca9dfafb381bd346d5d63a1915b94b85a57d3e6f4803c4ac34d5ab9541c0f18153508bb99791330848a0208454b006c09db3599ff33b2b6bb6e02f61d26062
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

### `dpkg` source package: `libde265=1.0.12-2`

Binary Packages:

- `libde265-0:amd64=1.0.12-2`

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
$ apt-get source -qq --print-uris libde265=1.0.12-2
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.12-2.dsc' libde265_1.0.12-2.dsc 2066 SHA512:00f86ab68faadc79f9fb0cdc12b82482b9cb92b263dc792f82f228630b38840ad7b208ae4808872817faad2ee97fa0139706d29482be9b4c24c5a6020273821e
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.12.orig.tar.gz' libde265_1.0.12.orig.tar.gz 846345 SHA512:2cd105f3ce15a075da758f5429670b78ec162217017d1057eb828d7bc45414d35f2a8ab3b2cd5f247320c361740f4ab92d2ce5a6d943feeb33dc28c273e1ed64
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.12-2.debian.tar.xz' libde265_1.0.12-2.debian.tar.xz 136316 SHA512:dc46a5adc0b547ce37dc10172837732e86e60b657c7af351cff6388c09804882ccb214c42a2fd6aa32717e636aabc1b4feef04234c5c3c7df8af35cbbac3330e
```

### `dpkg` source package: `libdeflate=1.18-1`

Binary Packages:

- `libdeflate-dev:amd64=1.18-1`
- `libdeflate0:amd64=1.18-1`

Licenses: (parsed from: `/usr/share/doc/libdeflate-dev/copyright`, `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.18-1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.18-1.dsc' libdeflate_1.18-1.dsc 2196 SHA512:824d28b3bafc78541768956048eeca66e5b35717508295ca18700b52a7293c4f2e3e0acea82de204e0261963ca2d88236706268397bec3b30978ab21a31aa7a0
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.18.orig.tar.gz' libdeflate_1.18.orig.tar.gz 184924 SHA512:8a60fa5850f323389370f931579f85a094a35b3db334f2a2afa61bee39ecebc797e93c6fe5deb4178e19d83a1427533975dba6c05ce0b1db88b43c9268d09124
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.18-1.debian.tar.xz' libdeflate_1.18-1.debian.tar.xz 4756 SHA512:aa72680eec89c930c824029cfba0195365df3d8df142be76d90180af081d068860fc3a1f5d8fe0e3696c5b317d6c41ccc7fe2b891af0c7c75eb4c79b55c15093
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

### `dpkg` source package: `libevent=2.1.12-stable-9`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.12-stable-9`
- `libevent-core-2.1-7:amd64=2.1.12-stable-9`
- `libevent-dev=2.1.12-stable-9`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-9`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-9`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-9`

Licenses: (parsed from: `/usr/share/doc/libevent-2.1-7/copyright`, `/usr/share/doc/libevent-core-2.1-7/copyright`, `/usr/share/doc/libevent-dev/copyright`, `/usr/share/doc/libevent-extra-2.1-7/copyright`, `/usr/share/doc/libevent-openssl-2.1-7/copyright`, `/usr/share/doc/libevent-pthreads-2.1-7/copyright`)

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
$ apt-get source -qq --print-uris libevent=2.1.12-stable-9
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-9.dsc' libevent_2.1.12-stable-9.dsc 2377 SHA512:d46ed308d53e99334d6d9fceef5f7e0a77b10b298ae7c256f766cb28c955ca6c3c1f79b0db4260fb5978f169d9e5bda0ac26da3a25a383b67d64d177accee822
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA512:88d8944cd75cbe78bc4e56a6741ca67c017a3686d5349100f1c74f8a68ac0b6410ce64dff160be4a4ba0696ee29540dfed59aaf3c9a02f0c164b00307fcfe84f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-9.debian.tar.xz' libevent_2.1.12-stable-9.debian.tar.xz 17676 SHA512:f569372bb7766833da6045d54bbeae58c21363bfb39b257536ea6271044e98e36c437b937f972f4054cf519858073bb2ae0f32c868e8ed68fc61e0ed290f620e
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

### `dpkg` source package: `libheif=1.16.2-2ubuntu1`

Binary Packages:

- `libheif-plugin-dav1d:amd64=1.16.2-2ubuntu1`
- `libheif-plugin-libde265:amd64=1.16.2-2ubuntu1`
- `libheif1:amd64=1.16.2-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libheif-plugin-dav1d/copyright`, `/usr/share/doc/libheif-plugin-libde265/copyright`, `/usr/share/doc/libheif1/copyright`)

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
$ apt-get source -qq --print-uris libheif=1.16.2-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.16.2-2ubuntu1.dsc' libheif_1.16.2-2ubuntu1.dsc 3008 SHA512:0a4681ffba267618d5fdd46195af353ff2813cbe9591c09267794dbdf1872a446933458ee87a19e88be5b07a81fd4c41c620b17d9e4d60d5f31af492a0be4cba
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.16.2.orig.tar.gz' libheif_1.16.2.orig.tar.gz 1339068 SHA512:a9c377d66bd85f8a3809d9b8c7b26b8d06eef511b14b86ade9db1cd934f0cef8339eeb8290d605fad3e0f5a1e4f104439356c62f893559f8ada957ea21625313
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.16.2-2ubuntu1.debian.tar.xz' libheif_1.16.2-2ubuntu1.debian.tar.xz 8792 SHA512:a6ff960e93841b3f4769fd4fe9b91ccfc2e56a234a88777b9580138691562c9bbbd970289f0d7b7620469a4b4e8d20832c059b7fdb8ad280ce4669f072c15a48
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

### `dpkg` source package: `libpng1.6=1.6.40-1`

Binary Packages:

- `libpng-dev:amd64=1.6.40-1`
- `libpng16-16:amd64=1.6.40-1`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.40-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.40-1.dsc' libpng1.6_1.6.40-1.dsc 2241 SHA512:c0876953715827bf70a28f78ebb6e5ee5834b1a5b2da9179f3876d8cd280c1c84326b7c3366a94a5f5c191a6caff784ecda379b5effba958a4c1d24ca8ca1e62
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.40.orig.tar.gz' libpng1.6_1.6.40.orig.tar.gz 1520834 SHA512:5f36a145c7d41f1c417d5f4e03be0155dae3499d72e67170acaad92c1af418c0bb6bc508e9b4b27ef4206bf0074cbf74978bade3bff28bc291867b8f8c2a38cf
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.40-1.debian.tar.xz' libpng1.6_1.6.40-1.debian.tar.xz 31092 SHA512:0bdc1b6be62b824a5af6a3e5bd9cba89207cab9899732cab8bf882ebf83b3137c8724dd6ed1b2d6fc1125959f964c6f2a34c1a803b82ee5127c0f777182fc9d7
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

### `dpkg` source package: `librsvg=2.54.7+dfsg-2`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.54.7+dfsg-2`
- `librsvg2-2:amd64=2.54.7+dfsg-2`
- `librsvg2-common:amd64=2.54.7+dfsg-2`
- `librsvg2-dev:amd64=2.54.7+dfsg-2`

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
$ apt-get source -qq --print-uris librsvg=2.54.7+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.54.7%2bdfsg-2.dsc' librsvg_2.54.7+dfsg-2.dsc 2960 SHA512:c09212d07343db08c0bcb3b12ded10156b3368b40748d5a6cb46d1b45ea1caa713ade27e6b1cb25a137172feb5d183bbce223b2fa0f069234128c8573b739046
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.54.7%2bdfsg.orig.tar.xz' librsvg_2.54.7+dfsg.orig.tar.xz 14342756 SHA512:e891cd9e2fc93f9f19b91ca99b0c6fe310227620a37ec93a78a69004a0466f47a3d9c8e7f4733e3b49e7f7c788c10adac58958394cd7004593d27df9ea67f4e4
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.54.7%2bdfsg-2.debian.tar.xz' librsvg_2.54.7+dfsg-2.debian.tar.xz 35544 SHA512:af5c96a6ff0c3f13d311e9378c17797d2afd8a5125f31930d339835db3d6ba89d37b554503ad915ce5b4d51d1923ad566572fb6158932ab3ec0cf9b8242de2ee
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
- `libselinux1-dev:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

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

- `libsepol-dev:amd64=3.5-1`
- `libsepol2:amd64=3.5-1`

Licenses: (parsed from: `/usr/share/doc/libsepol-dev/copyright`, `/usr/share/doc/libsepol2/copyright`)

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

### `dpkg` source package: `libtool=2.4.7-7`

Binary Packages:

- `libltdl-dev:amd64=2.4.7-7`
- `libltdl7:amd64=2.4.7-7`
- `libtool=2.4.7-7`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.7-7
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7-7.dsc' libtool_2.4.7-7.dsc 2257 SHA512:ea8556ba972137c14a410c2744253cd594acd7511aeb98d4d48aa22fde5bad8c27a1bf23fa21f2bc6b4c45acdaa8003ce36b0b082eda9ecf066690579ab09f46
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7.orig.tar.xz' libtool_2.4.7.orig.tar.xz 1026028 SHA512:424f4549aa713917859dc31e62153934c67b8b9d5718452f0e50bb8f6ef48ae6274cc4d4ddd905b15858d19c60daf8c194471e6ed0c8f76e7d55e7ef932a8d3a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7-7.debian.tar.xz' libtool_2.4.7-7.debian.tar.xz 40916 SHA512:f6ce4090de656b0ec1d264443bfdcdf4bcc03db92d539d05be80b8b026614d0dd2f0766276fa5be6de428cb7d51d374ced693900edaf3aa4d0354ed5c253c360
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

### `dpkg` source package: `libwebp=1.2.4-0.3`

Binary Packages:

- `libwebp-dev:amd64=1.2.4-0.3`
- `libwebp7:amd64=1.2.4-0.3`
- `libwebpdemux2:amd64=1.2.4-0.3`
- `libwebpmux3:amd64=1.2.4-0.3`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp7/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=1.2.4-0.3
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4-0.3.dsc' libwebp_1.2.4-0.3.dsc 2379 SHA512:eecbaab33e59e437e95646e47deb86a9da0702dfb34ec8fb7f4e01d65c59e476f2e540b788f100e4952b6d39e3f6fab3abefd66d8625ac829180f32faf41db72
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4.orig.tar.gz' libwebp_1.2.4.orig.tar.gz 4141376 SHA512:01f21e2c3057f5878b33664d0070832d78420de3cb2fe4379b07ae6a27bb569fd1c27a920fe324beccb96ae7bfa8c05fdd9e7b0aeba6de06ab4d8b084bb38803
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4.orig.tar.gz.asc' libwebp_1.2.4.orig.tar.gz.asc 833 SHA512:a9a27c81550a3376f9d6e56f3914ee2ad11c3200fb555a5fcb14d7fcf8d8f32a80d8fa5c9a27908a02059a4e2eeb21b1bceaa2061a7c0e809481e47592ec2fa6
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.4-0.3.debian.tar.xz' libwebp_1.2.4-0.3.debian.tar.xz 12004 SHA512:3fcda9b916067fef35f8d5365271ba475557664e5da593e4e67a5dcb23266cca30922133066b81883758ec6cfde29d5b60b498c210edaf6aa00158ff3d49cc3a
```

### `dpkg` source package: `libwmf=0.2.13-1`

Binary Packages:

- `libwmf-0.2-7:amd64=0.2.13-1`
- `libwmf-dev=0.2.13-1`
- `libwmflite-0.2-7:amd64=0.2.13-1`

Licenses: (parsed from: `/usr/share/doc/libwmf-0.2-7/copyright`, `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmflite-0.2-7/copyright`)

- `AGPL-3 with Font exception`
- `GD`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.13-1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.13-1.dsc' libwmf_0.2.13-1.dsc 2502 SHA512:a1c933cb1d2d3d34ce035638aab94aca25d636b16b1edbce044d596899a2b9c436183b16a3ca7ce12dde1b4e7cc1bb889339fbab4f569b0cf462254c8b1f0295
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.13.orig.tar.gz' libwmf_0.2.13.orig.tar.gz 3044235 SHA512:f45a936c9bc98fc1a5f2b0808b497119e4dcd3c132615fdddb7583e5719c7d1d7f85c16ebf313cad453e5b7ae3508bf6b80c4ed2b42322b7dec295d8f4eb86ce
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.13-1.debian.tar.xz' libwmf_0.2.13-1.debian.tar.xz 25712 SHA512:4d68bc37be135e03981980823e3bf3e23ee0358e7f609c0417be37dff0c760eaad7218e2a33dc0a836b25f1161202b05158c9885f6731812efb99e32dd59533c
```

### `dpkg` source package: `libx11=2:1.8.6-1ubuntu1`

Binary Packages:

- `libx11-6:amd64=2:1.8.6-1ubuntu1`
- `libx11-data=2:1.8.6-1ubuntu1`
- `libx11-dev:amd64=2:1.8.6-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.8.6-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.6-1ubuntu1.dsc' libx11_1.8.6-1ubuntu1.dsc 2587 SHA512:798234b1e47069996851787d956bdb6816e1e6acc4ce38a81da21473d3e71fc42ad927b7ff9363a441b2d18187b89935cd78c9fc7cdb29f42254a513cbb43806
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.6.orig.tar.gz' libx11_1.8.6.orig.tar.gz 3193457 SHA512:76ba1e30bd60c6988be7836db9795058541e0c64fb3d628713b78716e058fa2d2cd0a08549af21ada793c3dad7409b89ff7da8af3d1f0f4d5eb78801037977ff
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.6.orig.tar.gz.asc' libx11_1.8.6.orig.tar.gz.asc 801 SHA512:9659724070bbaefcfbcb113ea8e29c605deaa263e1e4e4f9a96136187e3e2118b02c5193054710e443171a56c98aa283604ed1b064f80ba587f3554972385206
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.8.6-1ubuntu1.diff.gz' libx11_1.8.6-1ubuntu1.diff.gz 77714 SHA512:27cfaf27adb7eab1a9d97a1871a23f0bcb01c19a5c0976a108bbedaac4f96bc5de059d497679dc1ebd04ec1cb85b3802d09668e0507cca7f01c7b228455bc462
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

### `dpkg` source package: `libxcrypt=1:4.4.36-2`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.36-2`
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

### `dpkg` source package: `libxml2=2.9.14+dfsg-1.3`

Binary Packages:

- `libxml2:amd64=2.9.14+dfsg-1.3`
- `libxml2-dev:amd64=2.9.14+dfsg-1.3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.14+dfsg-1.3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.3.dsc' libxml2_2.9.14+dfsg-1.3.dsc 3078 SHA512:b80c6bd40047809b56fec1c0c56eb7be20b4c9c173818521bc33853ca471bed585b9412de1f0692731a200e4f13819cc1d1b7aa48a43abfc610ea67c7de43089
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg.orig.tar.xz' libxml2_2.9.14+dfsg.orig.tar.xz 2351200 SHA512:1eacc9ac2cd8d38b8466659b3b9d84b94eb765c8f869d6cca0da131060bbc35c2b31c6148d59690547871a20cea339eac8fbe953b4fe37cf0900862f3fd9621b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.3.debian.tar.xz' libxml2_2.9.14+dfsg-1.3.debian.tar.xz 35076 SHA512:3bec56641f1afd1ef801c64499b90dfcacaa67343f8c8221496cdc5bff89b44033b129ea9e661f234c205b4a3e0a82f5be1c8044242a241bd2827c6d135d7f04
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

### `dpkg` source package: `libxt=1:1.2.1-1.1`

Binary Packages:

- `libxt-dev:amd64=1:1.2.1-1.1`
- `libxt6:amd64=1:1.2.1-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.1-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1-1.1.dsc' libxt_1.2.1-1.1.dsc 2170 SHA512:b7d307ff8b4b80e2075b2d4d292543eb52206a2e9e6e38395c193e12ca7fec4262e11025472bacdd9c2de500b37283747a125760093b013c6993fd597bbe9749
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz' libxt_1.2.1.orig.tar.gz 1024473 SHA512:73c2fd8a6590ab5ee93cf646e4f41fb71d424961ecbf9bc13c68abdf539c63ab0c59a4d3b22195ba21859523f4cf0e937648424532794a1350a5891061096503
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz.asc' libxt_1.2.1.orig.tar.gz.asc 358 SHA512:135e01b8a79beac9530087dee1a5458c359b4f1ae8346e2502f72f4fc24be400477fda90944315c585e3416e80cb74d1a140d5dfec81e854a4996199a8b221dc
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.1-1.1.diff.gz' libxt_1.2.1-1.1.diff.gz 45585 SHA512:a88bd795883c88dc1c71a23b3a321e985f079819129e9a7e6fe37e95ca0f9b9650b18a9897bf7d0f894fc821f014dc74335296b58190ddfd69ffc74c291d6baa
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

### `dpkg` source package: `libzstd=1.5.5+dfsg2-1ubuntu2`

Binary Packages:

- `libzstd-dev:amd64=1.5.5+dfsg2-1ubuntu2`
- `libzstd1:amd64=1.5.5+dfsg2-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libzstd-dev/copyright`, `/usr/share/doc/libzstd1/copyright`)

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

### `dpkg` source package: `linux=6.5.0-13.13`

Binary Packages:

- `linux-libc-dev:amd64=6.5.0-13.13`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lto-disabled-list=43`

Binary Packages:

- `lto-disabled-list=43`

Licenses: (parsed from: `/usr/share/doc/lto-disabled-list/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lto-disabled-list=43
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_43.dsc' lto-disabled-list_43.dsc 1435 SHA512:9dc15b5e2eeeb1e2d6aba43a48f0d06d1b0df82c2fb899833460434c1d1ef824f3c0594c7d3e3335a5ef3457f9764c8e898cfbade509e12223fef212b95e3b0d
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_43.tar.xz' lto-disabled-list_43.tar.xz 13328 SHA512:9a80807ebe8dc8b326b63a00b23c9f17a585390a4824934a1055f24e528cfb68dd4f5135cc96299fa8a01075c8f1748dff8436e34cc89f3bad126ab1cf39b537
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

### `dpkg` source package: `media-types=10.1.0`

Binary Packages:

- `media-types=10.1.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=10.1.0
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_10.1.0.dsc' media-types_10.1.0.dsc 1624 SHA512:78ee4c91efa0eea0314213b1df7cc659f3b47556a648e07c4044f1ae7ae08ccd6c4d479e6425297ac79c38a2a607a157ed781c66751235cecee1eb1ed8edf6b5
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_10.1.0.tar.xz' media-types_10.1.0.tar.xz 59052 SHA512:db92986166c6eedd44d839617c75a1f60704af6d87f92a5c9bb5f207a8e4e27f67b86e340745f6f41e793908d48eb609575678495194a21d368db2fc102b35c9
```

### `dpkg` source package: `mercurial=6.4.4-2`

Binary Packages:

- `mercurial=6.4.4-2`
- `mercurial-common=6.4.4-2`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=6.4.4-2
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.4.4-2.dsc' mercurial_6.4.4-2.dsc 2377 SHA512:7ec3768cd9fb155bd0ddd9309db291164d27b8875f0c265011a9deaa7788fae349e18a51031900e03da12e5dc54bd28b6f5672293c4e8130adf9dd1f4198a4cd
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.4.4.orig.tar.gz' mercurial_6.4.4.orig.tar.gz 8182450 SHA512:6b97eaa10d2367dc583160170e74535e2c863ccc02e3d5527467769ce0b2db78a5496a48bad0f812a1bff5a9afec7751eea88edcefb06d052b9632a16da08c0f
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.4.4-2.debian.tar.xz' mercurial_6.4.4-2.debian.tar.xz 70120 SHA512:836f09bcacb935bac0d962882de399c35ddd2459cae5b282be9a661c12938d1a5e2d7a01794c32112c91e571741c789e6d446713ef45e396219a21cfbcb571c3
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

### `dpkg` source package: `mpfr4=4.2.1-1`

Binary Packages:

- `libmpfr6:amd64=4.2.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.2.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.2.1-1.dsc' mpfr4_4.2.1-1.dsc 1959 SHA512:ddb3f2fe908d50f06f2f36103c09eaeeca0e1d9b3660a45d6b284175523973c6adf2e9846e61f594306d590dcc46f518284b15debb43b818a8ff38f42d902e41
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.2.1.orig.tar.xz' mpfr4_4.2.1.orig.tar.xz 1493608 SHA512:bc68c0d755d5446403644833ecbb07e37360beca45f474297b5d5c40926df1efc3e2067eecffdf253f946288bcca39ca89b0613f545d46a9e767d1d4cf358475
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.2.1-1.debian.tar.xz' mpfr4_4.2.1-1.debian.tar.xz 12556 SHA512:b10465385039b7d17f81dd960d0adc3e92cf6a254a1949b1e88ca2a10da626f1333fd3bf3c37d903b87ffc5458260ac765cccbfc65bb4647953cfb85975fa333
```

### `dpkg` source package: `mysql-8.0=8.0.35-0ubuntu0.23.10.1`

Binary Packages:

- `libmysqlclient-dev=8.0.35-0ubuntu0.23.10.1`
- `libmysqlclient21:amd64=8.0.35-0ubuntu0.23.10.1`

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
$ apt-get source -qq --print-uris mysql-8.0=8.0.35-0ubuntu0.23.10.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.35-0ubuntu0.23.10.1.dsc' mysql-8.0_8.0.35-0ubuntu0.23.10.1.dsc 3568 SHA512:a4267afb691790976fcf7f26d4b6177fee1153ff7dec97ce01579eb9ec3063033513a16da06a4c42efd4315e1522b94a607e64d48cdea56d87ed96aca4b59fc8
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.35.orig.tar.gz' mysql-8.0_8.0.35.orig.tar.gz 438111810 SHA512:2936f7a84aa5f96633b239d1dba3613462d88f3a2ea493a7d05aa9a9b590e9e36a30857f44fcdb11360242375d6106e80cd1b32e0c6cb14502c1518ad1a720b2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.35-0ubuntu0.23.10.1.debian.tar.xz' mysql-8.0_8.0.35-0ubuntu0.23.10.1.debian.tar.xz 147480 SHA512:17428e3dbef274da31f9403744321ae4014d2fe7c6377df8c7b1d6f2dfa4b6cc56c671b5a7dd025c69959585b22df2829499220b209e956504426d2b07ed1324
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

### `dpkg` source package: `ncurses=6.4+20230625-2`

Binary Packages:

- `libncurses-dev:amd64=6.4+20230625-2`
- `libncurses6:amd64=6.4+20230625-2`
- `libncursesw6:amd64=6.4+20230625-2`
- `libtinfo6:amd64=6.4+20230625-2`
- `ncurses-base=6.4+20230625-2`
- `ncurses-bin=6.4+20230625-2`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

### `dpkg` source package: `openexr=3.1.5-5.1`

Binary Packages:

- `libopenexr-3-1-30:amd64=3.1.5-5.1`
- `libopenexr-dev=3.1.5-5.1`

Licenses: (parsed from: `/usr/share/doc/libopenexr-3-1-30/copyright`, `/usr/share/doc/libopenexr-dev/copyright`)

- `BSD-3-clause`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=3.1.5-5.1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5-5.1.dsc' openexr_3.1.5-5.1.dsc 2489 SHA512:f8008331e6a9530219bf71306bc1c8f0da83b4a7c0dd684f77c20e842d0faa5317f1b798cb0023012d7fda88a7a13e6d616f0306f72349da08d4e47fd8da1614
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5.orig.tar.gz' openexr_3.1.5.orig.tar.gz 20327926 SHA512:01ef16eacd2dde83c67b81522bae87f47ba272a41ce7d4e35d865dbdcaa03093e7ac504b95d2c1b3a19535f2364a4f937b0e0570c74243bb1c6e021fce7b620c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5.orig.tar.gz.asc' openexr_3.1.5.orig.tar.gz.asc 287 SHA512:9b3978e44b531429aba42b9cc4969a470898d9d74652e3809edb0273ba9b127c471aec6570b5d352be738f59810091c0df2c70d39c16d2c32833d173b270f72c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_3.1.5-5.1.debian.tar.xz' openexr_3.1.5-5.1.debian.tar.xz 18828 SHA512:37d5507a3a3ed456ae189283923a3d9417cb321d5f7f1ffa94b86fffcd5f53ff3a1b9641906e0c970a59e9d6d14f7a8fd714726ce2e891dd14243967c287c67e
```

### `dpkg` source package: `openjpeg2=2.5.0-2`

Binary Packages:

- `libopenjp2-7:amd64=2.5.0-2`
- `libopenjp2-7-dev:amd64=2.5.0-2`

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
$ apt-get source -qq --print-uris openjpeg2=2.5.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.5.0-2.dsc' openjpeg2_2.5.0-2.dsc 2673 SHA512:ad2f14733d6142ccf6a410ebd6498326d33cde910211c39994f15e7c6fb4e5c3c9e2953bb6120178e0c52ab036f073d2dda6c2be0141a1e32c4c230b239b43a2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.5.0.orig.tar.xz' openjpeg2_2.5.0.orig.tar.xz 1221108 SHA512:a266297d60ff93e14dbee890b01a76870bda69f082dbe8932fc444ccd260c27aaaac8b22e3c00ca71930b2555a1cad6cf6ed0d5d882d9d13f472cc494cab8234
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.5.0-2.debian.tar.xz' openjpeg2_2.5.0-2.debian.tar.xz 17388 SHA512:4cc7c0fd4237efdc79c209ad548e30477fc587ef9206a4e10d7b879309cb087c3ec0b6ee7a6350002405f303546ed54835f34d63a5681a8302f394ca0f985181
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

### `dpkg` source package: `openssh=1:9.3p1-1ubuntu3`

Binary Packages:

- `openssh-client=1:9.3p1-1ubuntu3`

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
$ apt-get source -qq --print-uris openssh=1:9.3p1-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.3p1-1ubuntu3.dsc' openssh_9.3p1-1ubuntu3.dsc 3069 SHA512:8c7da1a7940064740d0ece1b9db82b984aad8868faebb64dd5447ae1b7aeecb89b77f97979d4b283ecda5f796fe3640f3ff074bdf359e1b579657ca610fdb626
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.3p1.orig.tar.gz' openssh_9.3p1.orig.tar.gz 1856839 SHA512:087ff6fe5f6caab4c6c3001d906399e02beffad7277280f11187420c2939fd4befdcb14643862a657ce4cad2f115b82a0a1a2c99df6ee54dcd76b53647637c19
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.3p1-1ubuntu3.debian.tar.xz' openssh_9.3p1-1ubuntu3.debian.tar.xz 192432 SHA512:527f3ebc538593006f8827743b8fe9582703b6bb7ac55644d0c6282a9e14df4887aae71db7574838876238a5e3349aad5280502922aecb4204df1c14c335cf4c
```

### `dpkg` source package: `openssl=3.0.10-1ubuntu2.1`

Binary Packages:

- `libssl-dev:amd64=3.0.10-1ubuntu2.1`
- `libssl3:amd64=3.0.10-1ubuntu2.1`
- `openssl=3.0.10-1ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libssl-dev/copyright`, `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

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

### `dpkg` source package: `pango1.0=1.51.0+ds-2`

Binary Packages:

- `libpango-1.0-0:amd64=1.51.0+ds-2`
- `libpangocairo-1.0-0:amd64=1.51.0+ds-2`
- `libpangoft2-1.0-0:amd64=1.51.0+ds-2`

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
$ apt-get source -qq --print-uris pango1.0=1.51.0+ds-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.51.0%2bds-2.dsc' pango1.0_1.51.0+ds-2.dsc 3584 SHA512:c16d19787d009adccb08656b4bd980789f3cb772c75ac5c4463317bcae1b00bfb448f1269e37eb000290340b8b3dae61a683b4d3646522796a950b660870f182
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.51.0%2bds.orig.tar.xz' pango1.0_1.51.0+ds.orig.tar.xz 1731104 SHA512:2ed4ec6baf4e21da1f19d4ef43b1e3b1753229022f8e8ae6ac4ef910ab664defba8fd99391255d37f5b0f5b71ec3aee7f1ba15f5a449c04dfb07902fd700a635
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.51.0%2bds-2.debian.tar.xz' pango1.0_1.51.0+ds-2.debian.tar.xz 41192 SHA512:3b0a5c5ac1e17ff83678a06f11e7bb781d21c22e4956e76a5ce16064e57eeaa6f2d43bc3833662add7ea7e62165c174e5fad8cbe78cdc60a23d3b53c3bb07c2f
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

### `dpkg` source package: `pcre2=10.42-4`

Binary Packages:

- `libpcre2-16-0:amd64=10.42-4`
- `libpcre2-32-0:amd64=10.42-4`
- `libpcre2-8-0:amd64=10.42-4`
- `libpcre2-dev:amd64=10.42-4`
- `libpcre2-posix3:amd64=10.42-4`

Licenses: (parsed from: `/usr/share/doc/libpcre2-16-0/copyright`, `/usr/share/doc/libpcre2-32-0/copyright`, `/usr/share/doc/libpcre2-8-0/copyright`, `/usr/share/doc/libpcre2-dev/copyright`, `/usr/share/doc/libpcre2-posix3/copyright`)

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

- `libperl5.36:amd64=5.36.0-9ubuntu1.1`
- `perl=5.36.0-9ubuntu1.1`
- `perl-base=5.36.0-9ubuntu1.1`
- `perl-modules-5.36=5.36.0-9ubuntu1.1`

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

### `dpkg` source package: `pkgconf=1.8.1-2`

Binary Packages:

- `libpkgconf3:amd64=1.8.1-2`
- `pkg-config:amd64=1.8.1-2`
- `pkgconf:amd64=1.8.1-2`
- `pkgconf-bin=1.8.1-2`

Licenses: (parsed from: `/usr/share/doc/libpkgconf3/copyright`, `/usr/share/doc/pkg-config/copyright`, `/usr/share/doc/pkgconf/copyright`, `/usr/share/doc/pkgconf-bin/copyright`)

- `BSD-2`
- `BSD-4`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pkgconf=1.8.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkgconf/pkgconf_1.8.1-2.dsc' pkgconf_1.8.1-2.dsc 1638 SHA512:9c27cecac22ac56a68fb423384b920b64f8f9adc29015cd6dcc43baa43d39ff77bc7261f64034ab949ddb4edfe9410d363fb64629b10dd9184b8bce7a78db42e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkgconf/pkgconf_1.8.1.orig.tar.xz' pkgconf_1.8.1.orig.tar.xz 302372 SHA512:7a7d5204c1c9bfb6578bda56f299d1fa0300e69a133a65730b10ad77aefbf26fceb74ae77cecda326b3ed5db5736f27fcce94764b3a56d40f4bb99fecdc80bba
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkgconf/pkgconf_1.8.1-2.debian.tar.xz' pkgconf_1.8.1-2.debian.tar.xz 15556 SHA512:b1f41553a2dbec8b25d46e6bb7aa55b948030a8557d9ad0435c1922ce7fb033fec80026653440ce03a04a99785edf6118eb7c62a5b92b460eade2f205b8a77da
```

### `dpkg` source package: `postgresql-15=15.4-1ubuntu1`

Binary Packages:

- `libpq-dev=15.4-1ubuntu1`
- `libpq5:amd64=15.4-1ubuntu1`

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
$ apt-get source -qq --print-uris postgresql-15=15.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-15/postgresql-15_15.4-1ubuntu1.dsc' postgresql-15_15.4-1ubuntu1.dsc 4116 SHA512:edcdcfa82d936d7810651aac981386e49eb13a4965c8b4d3743ea3763c48c08c1454408b4914ad56f208181607a1b6eeb80f01983f0ec079cf5bf6574297428d
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-15/postgresql-15_15.4.orig.tar.gz' postgresql-15_15.4.orig.tar.gz 29978353 SHA512:e99099f5d973ecc87758ea485823f6e6de87e15e8b63d5b04a9dca2bf0ec10116bbb456b94da308befa192c2999864557b61f0c9c05462b2354b0cdd71e70fb8
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-15/postgresql-15_15.4-1ubuntu1.debian.tar.xz' postgresql-15_15.4-1ubuntu1.debian.tar.xz 25308 SHA512:8ba4e1d2584eaafb88450501cfa57a13fb54563500abdb3ee89053fd4b8e157f25f5d64bde84426de86acbe5637e3c61c839c13caf55ecce662bb8cb60508cdc
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

### `dpkg` source package: `python3-defaults=3.11.4-5`

Binary Packages:

- `libpython3-stdlib:amd64=3.11.4-5`
- `python3=3.11.4-5`
- `python3-minimal=3.11.4-5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.11.4-5
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.11.4-5.dsc' python3-defaults_3.11.4-5.dsc 3001 SHA512:d39f4d0c80dc998ec124eea3ec2c9cbc317ffdeb9d08cb98802400b889c540f48e21761c0da460c392402dac7fc481884568006b3d443226102e3b7cccec2f83
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.11.4-5.tar.gz' python3-defaults_3.11.4-5.tar.gz 146763 SHA512:493fe4be0396bd5a4dc23da544756450ad8f4ee0502345f2f0e7be43642a560d5e6144d3c693fa223f010d466481329cdda6347c733c890adb8ff18fb7e9122c
```

### `dpkg` source package: `python3-stdlib-extensions=3.11.5-1`

Binary Packages:

- `python3-distutils=3.11.5-1`
- `python3-lib2to3=3.11.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.11.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.11.5-1.dsc' python3-stdlib-extensions_3.11.5-1.dsc 2563 SHA512:b050010409ad04d8fe42d25ba72cf2dd9a8a35b339aa930dcd2a3f9c72d2de32a59a6b1be0de562ce8becd759d6af051676fcee9144c8f530e81ceb683116a15
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.11.5.orig.tar.xz' python3-stdlib-extensions_3.11.5.orig.tar.xz 1784144 SHA512:1a5c65bd1675d301d08101dc4a26b8775f76db91f049bb2168ab2e3d2d9e8952d11b6301537bdec082f3333d51058b032ce7a3e8dddf97655b0f5d5e12bc09bd
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.11.5-1.debian.tar.xz' python3-stdlib-extensions_3.11.5-1.debian.tar.xz 29120 SHA512:c6be4697ce59e507c5583387d6c55a745b3475cc71c8533f85003096a2f454b342a9fed65261950caa2875c45f3af56741ea432415b10d426be5e1825a7b4220
```

### `dpkg` source package: `python3.11=3.11.6-3`

Binary Packages:

- `libpython3.11-minimal:amd64=3.11.6-3`
- `libpython3.11-stdlib:amd64=3.11.6-3`
- `python3.11=3.11.6-3`
- `python3.11-minimal=3.11.6-3`

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
$ apt-get source -qq --print-uris python3.11=3.11.6-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.11/python3.11_3.11.6-3.dsc' python3.11_3.11.6-3.dsc 3655 SHA512:15109521f97428aeb6ab63d28b52d38096b96ea2c2bb4580dee68c3657dbae702a3e510b442088ae935dfa75e477c2e362cb4c44c2542fd6288f5fab803e4ce1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.11/python3.11_3.11.6.orig.tar.xz' python3.11_3.11.6.orig.tar.xz 20067204 SHA512:94b1038f6f53de0c44f99f72ed0f2e0791fd9d2a325ae00ba145b2b2c332c27b300b3ea3473017518089478f15e01867b1bb203c16610039cce36f8366de341a
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.11/python3.11_3.11.6-3.debian.tar.xz' python3.11_3.11.6-3.debian.tar.xz 213928 SHA512:859c5e0fc4c1fb1dbf77a4608d0987aa018d91c2ae4960639fbfc4f51edae4817b93d8370e77a0ff24a2a37b6752b5e971887bc0bbd56685b1d206130d188662
```

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

### `dpkg` source package: `sqlite3=3.42.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.42.0-1`
- `libsqlite3-dev:amd64=3.42.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

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

### `dpkg` source package: `tiff=4.5.1+git230720-1ubuntu1`

Binary Packages:

- `libtiff-dev:amd64=4.5.1+git230720-1ubuntu1`
- `libtiff6:amd64=4.5.1+git230720-1ubuntu1`
- `libtiffxx6:amd64=4.5.1+git230720-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff6/copyright`, `/usr/share/doc/libtiffxx6/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.5.1+git230720-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.5.1%2bgit230720-1ubuntu1.dsc' tiff_4.5.1+git230720-1ubuntu1.dsc 2435 SHA512:aca1de8629dccc36817aa4ec5707a4367455e2e5603062cac36b3e7ec12fbe9cf3c8589be6979f0b99af3d7cfc841f522345a682693dcaefee04cc765a7e01dc
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.5.1%2bgit230720.orig.tar.xz' tiff_4.5.1+git230720.orig.tar.xz 1781896 SHA512:6bf9653f5c65d17c2944b20d14a5d5ab3b89d461bc6eb935a54aa8df99ce7221aeb2172f06b44affd06d81aeaab5698b90b07fde883167d0abf51debaaa6f71b
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.5.1%2bgit230720-1ubuntu1.debian.tar.xz' tiff_4.5.1+git230720-1ubuntu1.debian.tar.xz 22224 SHA512:525d5f4812c51e614bbd453d8b2f013873c3cb3dbc9f3c5ec4291b0c50fd6a393acded5938f7be430c9613aafa46b8825537b77265821995d5a41f6aa5d4210b
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

### `dpkg` source package: `unzip=6.0-28ubuntu1`

Binary Packages:

- `unzip=6.0-28ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-28ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-28ubuntu1.dsc' unzip_6.0-28ubuntu1.dsc 1836 SHA512:d3e4624dcb937521ba0abf8696c7641877d752738e90ae62f62534220ad7d95c88885ed9619ada67b0b00c39c6de2deb703dceb2ec085ab1c090a1f0779296a4
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA512:0694e403ebc57b37218e00ec1a406cae5cc9c5b52b6798e0d4590840b6cdbf9ddc0d9471f67af783e960f8fa2e620394d51384257dca23d06bcd90224a80ce5d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-28ubuntu1.debian.tar.xz' unzip_6.0-28ubuntu1.debian.tar.xz 28440 SHA512:1a73f1dfc8cdc0e904618461327959d27342e75cf613a8129bb664e3704b3afe1de942960a676e4eff4a6bbfbef3f6b77c94b46f79b6a035413461a11a854146
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

### `dpkg` source package: `util-linux=2.39.1-4ubuntu2`

Binary Packages:

- `bsdutils=1:2.39.1-4ubuntu2`
- `libblkid-dev:amd64=2.39.1-4ubuntu2`
- `libblkid1:amd64=2.39.1-4ubuntu2`
- `libmount-dev:amd64=2.39.1-4ubuntu2`
- `libmount1:amd64=2.39.1-4ubuntu2`
- `libsmartcols1:amd64=2.39.1-4ubuntu2`
- `libuuid1:amd64=2.39.1-4ubuntu2`
- `mount=2.39.1-4ubuntu2`
- `util-linux=2.39.1-4ubuntu2`
- `uuid-dev:amd64=2.39.1-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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

### `dpkg` source package: `xorgproto=2023.2-1`

Binary Packages:

- `x11proto-core-dev=2023.2-1`
- `x11proto-dev=2023.2-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2023.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2023.2-1.dsc' xorgproto_2023.2-1.dsc 3336 SHA512:d6459c917da1e6cc44e5661744780998f1cd3663dafb70621d304b6bc5113a6bd1d16f13a2b13739b065ea8fbf535096a3d1f0a5e9d145d823a86610baa247a4
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2023.2.orig.tar.gz' xorgproto_2023.2.orig.tar.gz 1150326 SHA512:9f03dcf7b2e7363523cdae6618f7c7db0041335aad505e0322571c391f2ef294957012a755b70e1dd24c3c0178e0423a36554032f552786d724eb9be31891436
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2023.2.orig.tar.gz.asc' xorgproto_2023.2.orig.tar.gz.asc 195 SHA512:bf84acc1adc37a2fe17193dec431a628980707200d8dd571c85f009bd5218d5470b3ac76d31756d10551dc75dfcfc791ec262c933837d0b8554181c2b99893b5
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2023.2-1.diff.gz' xorgproto_2023.2-1.diff.gz 25092 SHA512:ce40310bb67106bfe53052506d277c94e5a16a0c82a20e43944cdf57de1c724bc88af72aff3cd946f4d1f8527bc898f2d43ed9caa4d02a9dbf0647b6e3f3c798
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

### `dpkg` source package: `xz-utils=5.4.1-0.2`

Binary Packages:

- `liblzma-dev:amd64=5.4.1-0.2`
- `liblzma5:amd64=5.4.1-0.2`
- `xz-utils=5.4.1-0.2`

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
$ apt-get source -qq --print-uris xz-utils=5.4.1-0.2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.dsc' xz-utils_5.4.1-0.2.dsc 2621 SHA512:0c07970eedd5b1f67f8750f99dd7f86a1aef12cb1f1b3691fab1b1311d55de76ad597ac55c4e845adee3cdf8d8ba96ceeaed810b6688419934c20e3bafb8bb15
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz' xz-utils_5.4.1.orig.tar.xz 1485272 SHA512:f890ee5207799fbc7bb9ae031f444d39d82275b0e1b8cc7f01fdb9270050e38849bd1269db2a2f12fe87b5e23e03f9e809a5c3456d066c0a56e6f98d728553ea
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz.asc' xz-utils_5.4.1.orig.tar.xz.asc 833 SHA512:0802a4ae8f8fe700288b0fb1a4c9f59f71b26fcaea88cd368d36dcfd96a1deb2380a7b9af66b84d2f4faf68ff114d9b4b4e48b5b8362c37a8e528f13a4233cf3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.debian.tar.xz' xz-utils_5.4.1-0.2.debian.tar.xz 87432 SHA512:0d83bec7f80471ef4b3c5845cc2502807bb41f111970149244de1927618ed758d4e6da455f72eaa9d76acb41d4be685b968b1a8e5883f204277fde75fbc5d79b
```

### `dpkg` source package: `zlib=1:1.2.13.dfsg-1ubuntu5`

Binary Packages:

- `zlib1g:amd64=1:1.2.13.dfsg-1ubuntu5`
- `zlib1g-dev:amd64=1:1.2.13.dfsg-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.13.dfsg-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu5.dsc' zlib_1.2.13.dfsg-1ubuntu5.dsc 2968 SHA512:f464da1d48704d87d498db0b2f5e00eaa7e2b58cad27b5493fb6ab96d9ee9555522197d3b948a140bbd7f72ef29e89515c6c17297dd4a2688fb02e7145a9c855
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg.orig.tar.bz2' zlib_1.2.13.dfsg.orig.tar.bz2 1239825 SHA512:266ea72465ad1f0b63e42f8275c650615829929f2ff19064144c5bb942acd31cd8581ce45781c438fce949c6d9f3fa385efa59f754761441107ca1144fb56802
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.13.dfsg-1ubuntu5.debian.tar.xz' zlib_1.2.13.dfsg-1ubuntu5.debian.tar.xz 57068 SHA512:2fba202da1d40363e844c0baba3b8af3878087eb7b2b31ab4ba5f26616b1dc9f135483036cc42fbf53a1c359a19370c491d49f01058c91180485229ac3b36343
```
