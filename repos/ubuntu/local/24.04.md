# `ubuntu:24.04`

## Docker Metadata

- Image ID: `sha256:bfaf276bdd215773746bde9489a88d063b98584b8a650272c037da7be94941a6`
- Created: `2023-11-27T11:09:36.303855098Z`
- Virtual Size: ~ 71.06 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
- Labels:
  - `org.opencontainers.image.ref.name=ubuntu`
  - `org.opencontainers.image.version=24.04`

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

### `dpkg` source package: `apt=2.7.6`

Binary Packages:

- `apt=2.7.6`
- `libapt-pkg6.0:amd64=2.7.6`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.7.6
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.7.6.dsc' apt_2.7.6.dsc 2945 SHA512:00fe033fbeaa2f7e7133da0f92ea90c0a32ceb44c1c2a2d8d4dc18b4bf51081084c938525c83b00a1ae2c7dd110e271185ce6c0e52f0a0dfa05c828a7e55737d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.7.6.tar.xz' apt_2.7.6.tar.xz 2345736 SHA512:6d3efd270a6f7d5b2f020f7b5d68a6ecdd2e048c0c0545ab954651f89938ca74bf2f5488a6d769fb8268a5381368f384a28ffaaff235a15a9a4d289124e8a772
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

### `dpkg` source package: `audit=1:3.1.1-1build1`

Binary Packages:

- `libaudit-common=1:3.1.1-1build1`
- `libaudit1:amd64=1:3.1.1-1build1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.1.1-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.1.1-1build1.dsc' audit_3.1.1-1build1.dsc 2747 SHA512:80519794839b68fef897e3b1ec17d3ae476a918f361ff26cd032e4922783df32505f42d0f7b4b7aa64b754e6dbcb30d07b8a34f34b72cb8228b6b547a5ad9ae7
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.1.1.orig.tar.gz' audit_3.1.1.orig.tar.gz 1218111 SHA512:4917970cc4c7f786c464a6d101bf66d55d55ac4716cf415ff97177f08176a6301e946716d28cf5b16054538469b3140b97db99d55a28686a9a807eea60c070f3
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.1.1-1build1.debian.tar.xz' audit_3.1.1-1build1.debian.tar.xz 19044 SHA512:8ed01c9ff2ae563b9b35c6b8d1d83d3995e80a5a3204d33aeaa81c89a678e06c2f0aed56c45f3fde50c576caab03f23a298f742c8818d850a5825a3d8fa79a82
```

### `dpkg` source package: `base-files=13ubuntu5`

Binary Packages:

- `base-files=13ubuntu5`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=13ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_13ubuntu5.dsc' base-files_13ubuntu5.dsc 1613 SHA512:9bde22ef3d1c4a45983d87122fb4691af37224b4ddf20b7f72903abe7f97d556f1e53b3f9f5b0f9cdd2857c23a7c66679565b0595b25519dfa72155b0f18ca6f
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_13ubuntu5.tar.xz' base-files_13ubuntu5.tar.xz 93148 SHA512:ba27dd6efe2b7103923f275041db616d63020d4b23af12356a7bf690f5ba61b019b1296bfbd29a8c485b5ce4cb71e332d519cdb5ae81687691fd99fdb942638e
```

### `dpkg` source package: `base-passwd=3.6.2`

Binary Packages:

- `base-passwd=3.6.2`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.6.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.6.2.dsc' base-passwd_3.6.2.dsc 1762 SHA512:66578b5db0687e74a0daff500db52e2e5fbb3fc5e8bee023ebe99a289915e3f1ce94a1ad313e955fd3d6702dca35c7e54b301b2580393eb4f1e0c716641a25c9
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.6.2.tar.xz' base-passwd_3.6.2.tar.xz 58264 SHA512:f2ff9463ecae4d85345ae9c75f377eeb2baea12ca25082c69440d320f96a4b71bd3d261c06cfc687ad8a2ae072c42924c42ad59dcda08e0ee247186e4c581a96
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

### `dpkg` source package: `db5.3=5.3.28+dfsg2-4`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg2-4`

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
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg2-4
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-4.dsc' db5.3_5.3.28+dfsg2-4.dsc 2190 SHA512:f1055d77f4238356a0124c99d3f91765479ce40b7ebe769fc2f114dcd0e067f27d511e47d2211f01bc21de910eec087fee44ec731e8a317e9579539fb950ae1b
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2.orig.tar.xz' db5.3_5.3.28+dfsg2.orig.tar.xz 21287688 SHA512:f9c9d042702ef3fcfdd4b4859583048f3396b161009dc24b6d3a2c53533d58214239fc80e2c42db17e9f092df44d531502737f3b368b956bff49ef057b6b51ef
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-4.debian.tar.xz' db5.3_5.3.28+dfsg2-4.debian.tar.xz 33624 SHA512:ba77be9eadb07a8a9e8e5ad3e51540e70e0a9e15bb0376e9c535d2488b091d75f8984b23ff786b43767005652529a7214a5b37de4649bb5e691d8c49be2c4733
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

### `dpkg` source package: `debianutils=5.14`

Binary Packages:

- `debianutils=5.14`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`
- `GPL-2+`
- `SMAIL-GPL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.14
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.14.dsc' debianutils_5.14.dsc 1631 SHA512:a90531d0200bc05f82f62f081bc146ff856debf9d34b5dac8eae61bb6bd9aa57ea0dfa29b87f40b671e1c13da5a50bb3774efd8fa826e5b34b4e73a130f68a17
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.14.tar.xz' debianutils_5.14.tar.xz 79676 SHA512:4a152fec6c363c0ca26339bf8bf3f39ec3c10227bbfe5d2f5974c24a6207fdb6c34644ecfdf0c773d4c778b1a95f91a15697b12b5c0cd9a6d0d8f369373b956f
```

### `dpkg` source package: `diffutils=1:3.10-1`

Binary Packages:

- `diffutils=1:3.10-1`

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
$ apt-get source -qq --print-uris diffutils=1:3.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.10-1.dsc' diffutils_3.10-1.dsc 1715 SHA512:754b0ecc805723f61c8fa5dcfa1b667937bfb2b88d4a0385b071fc4b194a83b09f31d358429684908a39b10c0e0edf56743177a3bd5dcdd9b75fe1c368974dab
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.10.orig.tar.xz' diffutils_3.10.orig.tar.xz 1624240 SHA512:219d2c815a120690c6589846271e43aee5c96c61a7ee4abbef97dfcdb3d6416652ed494b417de0ab6688c4322540d48be63b5e617beb6d20530b5d55d723ccbb
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.10.orig.tar.xz.asc' diffutils_3.10.orig.tar.xz.asc 833 SHA512:91aa1fcfca224454e292540ea7813f4a0eb348f06a4374017326d524949775359fc833de597cc201c97f357eb6c675800828a6e3332572376f3554f1f2e1aca1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.10-1.debian.tar.xz' diffutils_3.10-1.debian.tar.xz 13952 SHA512:7fdb469643b31fc6e0a76a02ae900eef05d18c7895bdc2ff2db261500e4dca6cc3a08ef892e5126cc61e53124baaf32b88486f35424c17c86dd2ab3596255cb4
```

### `dpkg` source package: `dpkg=1.22.1ubuntu3`

Binary Packages:

- `dpkg=1.22.1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.22.1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.22.1ubuntu3.dsc' dpkg_1.22.1ubuntu3.dsc 3173 SHA512:0426fa1447d14b41c27d1f6f5596f864bbb21717bbfdfb4ca7be47c9effac364d871662f823cf1cdafbeb0484ec702bc69a200ded22dd4fcec3e34bf86d81dfc
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.22.1ubuntu3.tar.xz' dpkg_1.22.1ubuntu3.tar.xz 5610124 SHA512:0e7b4a92979da4ee442f4774e6b64c76949179159d92263b57ccc9131c829f7b4f17556c5a90f9504bed6e971008f56658b9c76b1002043a943c581cf41be86b
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

### `dpkg` source package: `gcc-13=13.2.0-7ubuntu1`

Binary Packages:

- `gcc-13-base:amd64=13.2.0-7ubuntu1`
- `libgcc-s1:amd64=13.2.0-7ubuntu1`
- `libstdc++6:amd64=13.2.0-7ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-13-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-13=13.2.0-7ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13.2.0-7ubuntu1.dsc' gcc-13_13.2.0-7ubuntu1.dsc 27663 SHA512:ddf26af0c0a3943c45100f0a534c636220cddb165fa29fcacd5d9c2bc8819ac571c5b4aa583519b985df9a3823a29aa1cadfcddcfe008df74d19b203036bd62b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13.2.0.orig.tar.gz' gcc-13_13.2.0.orig.tar.gz 92596024 SHA512:cf149aff3cbee36bf23987e91016fa3f93dbcba8c88319876e6aa3cacd1dacea27d06ea7c4da6394a56d7d9d4f14ac928ead7d25502f0cc6db558f7f5cd99dff
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-13/gcc-13_13.2.0-7ubuntu1.debian.tar.xz' gcc-13_13.2.0-7ubuntu1.debian.tar.xz 1717676 SHA512:5c207961eae0558fca350c65513714c64217029fc23ce9346ec23d60030aa66933f0e60362901abb360a570ab4bb5367d51dff02e3f92f0144c2c63f69aad52b
```

### `dpkg` source package: `glibc=2.38-3ubuntu1`

Binary Packages:

- `libc-bin=2.38-3ubuntu1`
- `libc6:amd64=2.38-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.38-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38-3ubuntu1.dsc' glibc_2.38-3ubuntu1.dsc 9310 SHA512:de01b8db04324f5d375a9ebd6247b3c0b126eac983edc6ff9e03b294bdeeb297630e4b7894e6b04ff81844d17d0342eeb22e662c5a97373f00c2508ee9ab5dc3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38.orig.tar.xz' glibc_2.38.orig.tar.xz 18913712 SHA512:a6dd5e42dcd63d58e2820c783522c8c895890b6e8c8e6c83b025553de0cc77cdf227e7044e431ead98c89c68a9ce4dd63509b47e647775fb2075f011849c1900
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38.orig.tar.xz.asc' glibc_2.38.orig.tar.xz.asc 833 SHA512:32248467450f4530f8e84c03ea78d8293946e1b1def853eff9fb2cb51106e66cc3b024a254f3c2fabd2634f8192bd14e7df00c317f4230860d702c4d9ec7a01e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.38-3ubuntu1.debian.tar.xz' glibc_2.38-3ubuntu1.debian.tar.xz 456828 SHA512:cad380328036402b74bf614a8970daec9be7a90bca5fa21552db56cecdd25122f5720eda8f2dc13dae4c583477458d485beceacbced9df4e46d7de44e36b7100
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

- `gpgv=2.2.40-1.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gpgv/copyright`)

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

### `dpkg` source package: `gnutls28=3.8.1-4ubuntu6`

Binary Packages:

- `libgnutls30:amd64=3.8.1-4ubuntu6`

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
$ apt-get source -qq --print-uris gnutls28=3.8.1-4ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1-4ubuntu6.dsc' gnutls28_3.8.1-4ubuntu6.dsc 3338 SHA512:33717f1a9de0cd2848c761efa18e4fdebeb2a26cd2dd795fe8dafcc4db62b282bcbecd515a1d8b8d0e18f6c5d5c611f863c7569b3dd5488681367d7c4840d341
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1.orig.tar.xz' gnutls28_3.8.1.orig.tar.xz 6447056 SHA512:22e78db86b835843df897d14ad633d8a553c0f9b1389daa0c2f864869c6b9ca889028d434f9552237dc4f1b37c978fbe0cce166e3768e5d4e8850ff69a6fc872
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1.orig.tar.xz.asc' gnutls28_3.8.1.orig.tar.xz.asc 996 SHA512:ad42a077718a91b82959ee7ed8282b69e73825c70c5c60eb4a1f87aab055dee2ac74a03f489d5f11c2094ec6ac01ea44c0daffb61cb4daae714dcaf5ea89ecd0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.8.1-4ubuntu6.debian.tar.xz' gnutls28_3.8.1-4ubuntu6.debian.tar.xz 73692 SHA512:64067f9c5a548cb44bc34c2a564531142bd27ce490773d5c9f4161cb4aebd9d290e5cb9a2e1df3ebd12e6b01bc53ec842ffe066447be7461860f49ba4aa178b0
```

### `dpkg` source package: `grep=3.11-3`

Binary Packages:

- `grep=3.11-3`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.11-3
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11-3.dsc' grep_3.11-3.dsc 1618 SHA512:c2ad81ddf8dfe01527552cc3d9bec4f88261b085c4d4d1edb1f4890a52b2b8515098fe781cf587f436a2bf6b902c40d018c1349cbbee37dd6404181b1d1ca620
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11.orig.tar.xz' grep_3.11.orig.tar.xz 1703776 SHA512:f254a1905a08c8173e12fbdd4fd8baed9a200217fba9d7641f0d78e4e002c1f2a621152d67027d9b25f0bb2430898f5233dc70909d8464fd13d7dd9298e65c42
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11.orig.tar.xz.asc' grep_3.11.orig.tar.xz.asc 833 SHA512:487aba063373ca0594c519991f19b2a6a33b3da0d74735c890f3828fd0880e7e6f64495d2c8f9efa5da53d1eb2d446609bab2399a4b89dcb4510a632e31ffb54
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.11-3.debian.tar.xz' grep_3.11-3.debian.tar.xz 20592 SHA512:13d6976429c6ee7cc32d94fc50cdfa0370b3544cd3d51cff2704fdd69f3d09443de3f8d95730e2972a6c514ee00e850b068e2bfabd85b8e6da7509114429184b
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

### `dpkg` source package: `libcap-ng=0.8.3-1build3`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1build3`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.8.3-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1build3.dsc' libcap-ng_0.8.3-1build3.dsc 2231 SHA512:608f026849eac5fca3abfa0e565edd32fc42a859e3cb026ec111b16136a9a67ad7dfc3da77f100a02b50f73cb341672e870c7706a5802d7c31891e82e30d3deb
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.8.3.orig.tar.gz' libcap-ng_0.8.3.orig.tar.gz 455383 SHA512:0ef9bc7bc6b7b59991f43b79aa6cde3e8d2c22c4b9ced2af8deae501e01d51e893033d109cb8aa0fdcba190140110993089245346334d7b114d18f1bb1b55b97
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1build3.debian.tar.xz' libcap-ng_0.8.3-1build3.debian.tar.xz 10620 SHA512:82abc8ce15c95f720c3f81cf297d9ba91e4a829ade6d99029d93636e5a0f36af9487a7ade7a9dbd474433b6d282ecfbc3c6cf313d2e56f44dbd0a5d10f4c5893
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

### `dpkg` source package: `libgpg-error=1.47-3`

Binary Packages:

- `libgpg-error0:amd64=1.47-3`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.47-3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47-3.dsc' libgpg-error_1.47-3.dsc 2896 SHA512:5484d9ac9145f15e05f56db9c4108b298af263f2b08635e66dc1d6c01edb77c052422d40add556e7503f1884160e129e81ea8621d4a083160bb87d9122edbde4
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47.orig.tar.bz2' libgpg-error_1.47.orig.tar.bz2 1020862 SHA512:bbb4b15dae75856ee5b1253568674b56ad155524ae29a075cb5b0a7e74c4af685131775c3ea2226fff2f84ef80855e77aa661645d002b490a795c7ae57b66a30
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47.orig.tar.bz2.asc' libgpg-error_1.47.orig.tar.bz2.asc 228 SHA512:babf3a17429aa7ad5d952099ea8d21bb5c9ba1bc74ea46f3027e0293449c32365208a05e141fa0bf033491320679b0b212f49919452f3dc63cce5d7f355d7195
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.47-3.debian.tar.xz' libgpg-error_1.47-3.debian.tar.xz 18572 SHA512:9e2bc3ac536bae0d5f0987f42716bed58e9c213339c6131336b2ddb9a4ed8c250fed18b7bdc130ee954a71b3e98d37ea77895ea00a4614222f02b2b93371b4fb
```

### `dpkg` source package: `libidn2=2.3.4-1build1`

Binary Packages:

- `libidn2-0:amd64=2.3.4-1build1`

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
$ apt-get source -qq --print-uris libidn2=2.3.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4-1build1.dsc' libidn2_2.3.4-1build1.dsc 2544 SHA512:0f74769d4eb24386f8410e5fdbe95c6bd40e26aab34174a4c34311e835fcd6043dcf17c0b7d918cefd212922c78ae08d7b5bfe506e02f545906b6eec54472af8
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4.orig.tar.gz' libidn2_2.3.4.orig.tar.gz 2083823 SHA512:a6e90ccef56cfd0b37e3333ab3594bb3cec7ca42a138ca8c4f4ce142da208fa792f6c78ca00c01001c2bc02831abcbaf1cf9bcc346a5290fd7b30708f5a462f3
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4.orig.tar.gz.asc' libidn2_2.3.4.orig.tar.gz.asc 228 SHA512:d2a575723326ae256a60e3edf7766af65434f716e11f963bb7ac29b6b2ff2872b41684a1bd1c6f3a3921e8a083512eff1faf2b0fc02513095c2bcf3563312fe0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.4-1build1.debian.tar.xz' libidn2_2.3.4-1build1.debian.tar.xz 16088 SHA512:ee67682f1696987dd41ab4ff25681a86d189826ee4a5dc0673b457a7d0200c48c409db0c374fecc7c17965193ae2adb0ab96ae80cbabde5aae4125cc3f6a6634
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

### `dpkg` source package: `libselinux=3.5-1build2`

Binary Packages:

- `libselinux1:amd64=3.5-1build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.5-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5-1build2.dsc' libselinux_3.5-1build2.dsc 3007 SHA512:ac8e7137344bcf46bbb062ef0f07860c74481e6b4d635be1be40bafc7e0e84554a5e30f85b87f03bf90751ff2753fa3a2e5e4320ab64919df39bb27499c559da
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5.orig.tar.gz' libselinux_3.5.orig.tar.gz 211453 SHA512:4e13261a5821018a5f3cdce676f180bb62e5bc225981ca8a498ece0d1c88d9ba8eaa0ce4099dd0849309a8a7c5a9a0953df841a9922f2c284e5a109e5d937ba7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5.orig.tar.gz.asc' libselinux_3.5.orig.tar.gz.asc 981 SHA512:ba486d29c92801a02f75213ef5bcc4a0c4a87afe9dfa797aa9bb495ded40f21e37b22d6ea114c0e480d669b090d1116e8b9cac9fa9ea29678d3647bc58d8bb29
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.5-1build2.debian.tar.xz' libselinux_3.5-1build2.debian.tar.xz 35960 SHA512:87fe257d83f8de42662016790a0fccdfe984344b2d2c0a78895295d33e1b667e4270c5d2402609e95fdac30e596715032b4754d78b661a19842ea03690ac053f
```

### `dpkg` source package: `libsemanage=3.5-1build1`

Binary Packages:

- `libsemanage-common=3.5-1build1`
- `libsemanage2:amd64=3.5-1build1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.5-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5-1build1.dsc' libsemanage_3.5-1build1.dsc 3014 SHA512:aa134e2bd2dfa58d11966d7df7ca94738f2095d077dbf329c4c2fda2a0969cf923f64e9e81c8e1f25833bcb5fcf5f3ab8de6930332c9071398edb116d87f8d23
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5.orig.tar.gz' libsemanage_3.5.orig.tar.gz 185060 SHA512:959fbd0d6bc6849da6caa13dc41c3f8818cbbd29f04b5d2ac7246c4b395b4f370f113a04cc9cfcb52be2afebfa636013ac4ad4011384c58c7ce066a45cae2751
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5.orig.tar.gz.asc' libsemanage_3.5.orig.tar.gz.asc 981 SHA512:c0a5ddb69c32ddefa26b3d1ec676bcc373e959dd8b4a7fcf6e1f74a3ca8e9af22af851ca66d3c43a704215ff79d27244e33d23038ef2f52ccc321aeb5f0c2790
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.5-1build1.debian.tar.xz' libsemanage_3.5-1build1.debian.tar.xz 30032 SHA512:338ad06136b29a955ec5492d10fa620dd8745371112ba4376d757d38ba07c08c07901ceade44d7324306d409cc14715cb6fca67292f0e02baee07322a999c721
```

### `dpkg` source package: `libsepol=3.5-2`

Binary Packages:

- `libsepol2:amd64=3.5-2`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5-2.dsc' libsepol_3.5-2.dsc 2005 SHA512:b76be86626690e04932a2824aed67eb8194d710ccaf00bf59defe92a09ce88d12b267dc189188be736f0442b0bce4952ee58db7a3542b3adc14c21231305bb10
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5.orig.tar.gz' libsepol_3.5.orig.tar.gz 497522 SHA512:66f45a9f4951589855961955db686b006b4c0cddead6ac49ad238a0e4a34775905bd10fb8cf0c0ff2ab64f9b7d8366b97fcd5b19c382dec39971a2835cc765c8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5.orig.tar.gz.asc' libsepol_3.5.orig.tar.gz.asc 981 SHA512:5aa46c3a7a5d7fa0d4376766b9444cdea1b14f3ec61725950a24fcb5ba2caae271a415c613807d06e4d9b04b40cda1525c12c442eed8a7e60fb5e5beacdaba3b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.5-2.debian.tar.xz' libsepol_3.5-2.debian.tar.xz 27596 SHA512:87ab5579d0e742fd52509cab880c5e1362830ab6c6581a8ffbd39c7e21b0997b3a4d76357b7bbad7d736ea78b7028f431d10e46a35f7f93fbb8ca6f088ac37ee
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

### `dpkg` source package: `libunistring=1.1-2`

Binary Packages:

- `libunistring5:amd64=1.1-2`

Licenses: (parsed from: `/usr/share/doc/libunistring5/copyright`)

- `FreeSoftware`
- `GFDL-1.2`
- `GFDL-NIV-1.2+`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with distribution exception`
- `GPL-2+ with distribution exception, Expat`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris libunistring=1.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.1-2.dsc' libunistring_1.1-2.dsc 2031 SHA512:89a88cb017f67e0539028c9a99a7530bd407d3776c2535d792ed9f38c007bff056fa9702ee280e38cb4ab26218b899f1d03de3e7150fef29e38b82e8d0e80336
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.1.orig.tar.xz' libunistring_1.1.orig.tar.xz 2397676 SHA512:01a4267bbd301ea5c389b17ee918ae5b7d645da8b2c6c6f0f004ff2dead9f8e50cda2c6047358890a5fceadc8820ffc5154879193b9bb8970f3fb1fea1f411d6
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.1.orig.tar.xz.asc' libunistring_1.1.orig.tar.xz.asc 833 SHA512:f94912a52df8d7863de271315c8b5a7e1e0ab7aabb66273fcdb81c48aa0b23360b80fdb1df9f768aede47dd5a92a280868db41147139dfabecbc82511715db4d
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.1-2.debian.tar.xz' libunistring_1.1-2.debian.tar.xz 14008 SHA512:2ce7e2e2b2fc08f3f6a848ddad65e6b7f17735c4dde7d1af491c289ccc58c3d904702a9468bce5b45c1420fda1895941bd2c04a5aa65f615946f2ceb72637e6f
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

### `dpkg` source package: `libzstd=1.5.5+dfsg2-2`

Binary Packages:

- `libzstd1:amd64=1.5.5+dfsg2-2`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.5+dfsg2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-2.dsc' libzstd_1.5.5+dfsg2-2.dsc 2375 SHA512:b4a49142abf47c7901e3859e9af1a2fa35350ddf03594eed4a0c5f8e656f684b93bc2acdf239fd7af6a6702e5c0671fd732e4b5abc3944fe4f7411237bd6eda4
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2.orig.tar.xz' libzstd_1.5.5+dfsg2.orig.tar.xz 1784164 SHA512:0b24cf71636b36ae17f617f0a4a2e1253ba6a7bfcd8b6f4717cc59310e92d23bde0945f885fa80622d84961b85fa6ba74e3436ab1badc687e8a13ac428a71b8d
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.5%2bdfsg2-2.debian.tar.xz' libzstd_1.5.5+dfsg2-2.debian.tar.xz 21068 SHA512:97f1075658c370cc2b5b80b5e0fd437981740e4718736c1fea5229c237e15854ed701791d5e36e9e5c5435c54a9593af4ffb55b7238128c04bbfca0c0dbf2da3
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

### `dpkg` source package: `mawk=1.3.4.20231102-1`

Binary Packages:

- `mawk=1.3.4.20231102-1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `GPL-2.0-only`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20231102-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20231102-1.dsc' mawk_1.3.4.20231102-1.dsc 2180 SHA512:0c3a8a85de06c9c353940341cd7a091de151952d49cec157623ae9fc78d01230aa53f63f45efef6a7bcd7f7c12f1779795fd59302ad26dc4af9a1faf4c993708
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20231102.orig.tar.gz' mawk_1.3.4.20231102.orig.tar.gz 413107 SHA512:53173a49ad2a63d096755964d0585517180a8555034cee519e2e6cc0c5392408b61960813eec101dd8ded298b6bc86128cd3469c1acb03141c264f24e52446b2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20231102.orig.tar.gz.asc' mawk_1.3.4.20231102.orig.tar.gz.asc 729 SHA512:5933f1cadea90b8349136b0b31f45b04b3e182b61de7ad62fb2142973e64fd8ffc7d3ee17bebd3b9b209d08d3732b2e807fe5554899fe8d4130e1a0d12dc9de8
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20231102-1.debian.tar.xz' mawk_1.3.4.20231102-1.debian.tar.xz 15532 SHA512:5add92ae49ef4c232e31ffbaf237c0739c102f3aa54d9993a6d7d44524ba523df509dda8b368e408f712275c704abacada815fc5e72994cbbf7d8848de398d65
```

### `dpkg` source package: `ncurses=6.4+20231121-1build1`

Binary Packages:

- `libncursesw6:amd64=6.4+20231121-1build1`
- `libtinfo6:amd64=6.4+20231121-1build1`
- `ncurses-base=6.4+20231121-1build1`
- `ncurses-bin=6.4+20231121-1build1`

Licenses: (parsed from: `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.4+20231121-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20231121-1build1.dsc' ncurses_6.4+20231121-1build1.dsc 3831 SHA512:ae293e66bc081cfccca18433d58ebfa8b98cc51420a10e5b7cca366aa9963df12c7c7845d381ad8ff7e590f1852234e6c7225f6669a1989dfc94edbfadd4be13
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20231121.orig.tar.gz' ncurses_6.4+20231121.orig.tar.gz 3671700 SHA512:3c9a4e5b481b542536420306777da7faf8c5151b60236d30dbe23c5716d9ba6a7e271d7720d4fab894add039a760aa9586b98560e8a57cbf36faaf428768c481
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20231121.orig.tar.gz.asc' ncurses_6.4+20231121.orig.tar.gz.asc 729 SHA512:e7f0ae75b2d5e845ef813307a5a6f45c73c540dc1c165054417c3b7aceefdc2802bb863aa196e0f3a709836fa0f20b2598fb74640cef622c1398a779342fe6f3
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.4%2b20231121-1build1.debian.tar.xz' ncurses_6.4+20231121-1build1.debian.tar.xz 48808 SHA512:e5bf12c8ae748930eed60a625b5f99c548e959b499cbe09dae5164ebd90701f3c1c1501fbd562559e9838ee7b9a96691c384ea7546a6023e1be8d6b933e64b62
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

### `dpkg` source package: `pam=1.5.2-9.1ubuntu1`

Binary Packages:

- `libpam-modules:amd64=1.5.2-9.1ubuntu1`
- `libpam-modules-bin=1.5.2-9.1ubuntu1`
- `libpam-runtime=1.5.2-9.1ubuntu1`
- `libpam0g:amd64=1.5.2-9.1ubuntu1`

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
$ apt-get source -qq --print-uris pam=1.5.2-9.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2-9.1ubuntu1.dsc' pam_1.5.2-9.1ubuntu1.dsc 2741 SHA512:d4b7216f82b103713935acee9438bc25da29f3b21619d933e719016aded88a31971271bfdf8d798148a9b6f0768c262b8eb47a454aa17ec6c662530c056b9f95
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA512:fa16350c132d3e5fb82b60d991768fb596582639841b8ece645c684705467305ccf1302a0147ec222ab78c01b2c9114c5496dc1ca565d2b56bf315f29a815144
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.5.2-9.1ubuntu1.debian.tar.xz' pam_1.5.2-9.1ubuntu1.debian.tar.xz 176544 SHA512:91ce7e7d2c575f9e8db5fd7c6903809d4cbec3c276136c7d32622753b22d87f94ed70d34379b671a016003a36ec4a3aa02c18c2578af31c100d3a3380bf11ee7
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

### `dpkg` source package: `perl=5.36.0-9ubuntu1`

Binary Packages:

- `perl-base=5.36.0-9ubuntu1`

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
$ apt-get source -qq --print-uris perl=5.36.0-9ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-9ubuntu1.dsc' perl_5.36.0-9ubuntu1.dsc 3026 SHA512:d4ddd92d2291be5f8ed08833a7baedcf7d3af81d3053700dd621c6107c37022c32ebfe10b2e09b444f387bce75cd35042c2428ac617c77b45feb46c3140c39f5
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig-regen-configure.tar.xz' perl_5.36.0.orig-regen-configure.tar.xz 417784 SHA512:4d16685f569a5b1dea79d607b6d62718111c32efaf5547bb9e1528bd755acf0c8fc74a1cc1f4d68fcb10aef9da7d8fea17a5cc10dabce6efa4721ab45ab03a65
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0.orig.tar.xz' perl_5.36.0.orig.tar.xz 13051500 SHA512:6dd6ac2a77566c173c5ab9c238cf555f2c3e592e89abb5600bc23ce1cbd0c349e0233f6417cbbf1f6d0aefc6a734ba491285af0d3dc68a605b658b65c89f1dab
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.36.0-9ubuntu1.debian.tar.xz' perl_5.36.0-9ubuntu1.debian.tar.xz 170808 SHA512:e2ea25d29a46e5cb5ee15bd43f0310ffd652c684f705603a34d8821d48f21956cd14dc46067dbffd7ec6228520ed36b1ec731989e696796b28d19e573a83cfa2
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `systemd=253.5-1ubuntu7`

Binary Packages:

- `libsystemd0:amd64=253.5-1ubuntu7`
- `libudev1:amd64=253.5-1ubuntu7`

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
$ apt-get source -qq --print-uris systemd=253.5-1ubuntu7
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_253.5-1ubuntu7.dsc' systemd_253.5-1ubuntu7.dsc 6902 SHA512:d54dd5f36a6b7b71a67c758bddaafcf3025988484c3d3fcc5ba6abdcb2e030bb960507af89275d33c96abc9a8951eed5daf6f7910baeeaf30c4ea76cf6bcfd28
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_253.5.orig.tar.gz' systemd_253.5.orig.tar.gz 12015672 SHA512:39709b485cd9287e26ac8e973fa1692b280bec3b96e1da6667e4a4f2ac2228aa072b22802720a254698d32c82f5306d7feb32229e4b6d54cc0e2b1e2caa4cc2e
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_253.5-1ubuntu7.debian.tar.xz' systemd_253.5-1ubuntu7.debian.tar.xz 220320 SHA512:6fab6e06ee154f9ae84bef0f6c5775be759dee368a695f1b7e23d865c72cbf524499610fe0678f97ab943bd7c78143d5f06aa5fa8e1aafb8089aeb0f78854da6
```

### `dpkg` source package: `sysvinit=3.08-3ubuntu1`

Binary Packages:

- `sysvinit-utils=3.08-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.08-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.08-3ubuntu1.dsc' sysvinit_3.08-3ubuntu1.dsc 2495 SHA512:d204847d567b6b367005b9aa6746e7993ad811ac7fec85cc2a15d80ad06d1c01b37d2b518c0d21c2a2598b3a317fe537a86cb7546b7564cb6b37a9337b99d5aa
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.08.orig.tar.gz' sysvinit_3.08.orig.tar.gz 513674 SHA512:63ed7ebd50944adce1a35af7798d0e2d6248f36a606f63bb7a567424555ec33e83c33b897528c801b4b4ac61b24d2a3555c9a690031c50a94e7ead83f37f8e96
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.08-3ubuntu1.debian.tar.xz' sysvinit_3.08-3ubuntu1.debian.tar.xz 139156 SHA512:46c99bc70a9e9d4f5d3edcd16966ee046be3f26b34d47f7cb101b3e15ca50c1dd0fc3877c33ecc6bdd948d74a91cfc387c40ecdb019e966370f42233a965bca3
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

### `dpkg` source package: `util-linux=2.39.2-6ubuntu1`

Binary Packages:

- `bsdutils=1:2.39.2-6ubuntu1`
- `libblkid1:amd64=2.39.2-6ubuntu1`
- `libmount1:amd64=2.39.2-6ubuntu1`
- `libsmartcols1:amd64=2.39.2-6ubuntu1`
- `libuuid1:amd64=2.39.2-6ubuntu1`
- `mount=2.39.2-6ubuntu1`
- `util-linux=2.39.2-6ubuntu1`

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
$ apt-get source -qq --print-uris util-linux=2.39.2-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.39.2-6ubuntu1.dsc' util-linux_2.39.2-6ubuntu1.dsc 4711 SHA512:a0fb49b3257ae4564fbb29f39c5b1152f0d327ccd7325125f70e1c73e8716ce6fe3985fca260b950baacfb49d6a70250f5ca33468c3b04dc75445abca4d64f73
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.39.2.orig.tar.xz' util-linux_2.39.2.orig.tar.xz 8362220 SHA512:cebecdd62749d0aeea2c4faf7ad1606426eff03ef3b15cd9c2df1126f216a4ed546d8fc3218c649fa95944eb87a98bb6a7cdd0bea31057c481c5cf608ffc19a3
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.39.2-6ubuntu1.debian.tar.xz' util-linux_2.39.2-6ubuntu1.debian.tar.xz 105504 SHA512:cb91c7b60ebd4359ba554f4099ecc42fea4a30d3427123b1d76156f455ccd641da4baf457f09535400569f590da9d83378541214da1b93be8154865f89efb906
```

### `dpkg` source package: `xxhash=0.8.2-2`

Binary Packages:

- `libxxhash0:amd64=0.8.2-2`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.2-2.dsc' xxhash_0.8.2-2.dsc 1969 SHA512:7922828f526e6ab7b421a3e3a7a45090fd64b5712e43df49597ed4dad0aa28c973c4b428d06cb9905b881f2c428caeac4d7d5538bf68c69c72662435fe64e5de
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.2.orig.tar.gz' xxhash_0.8.2.orig.tar.gz 1141188 SHA512:3e3eef21432fe88bc4dd9940ccad0308fdea3537b06fa5ac0e74c1bde53413dff29c8b3fc617a8a42b9ce88fcf213311d338a31b1ce73b3729342c9e68f06c78
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.2-2.debian.tar.xz' xxhash_0.8.2-2.debian.tar.xz 4920 SHA512:a88c7e6e538504d31e737feb21fd8af2d57537756bd2ecc5f5396349f3ed20ff87287602e5bcce04f67564a00b192de6b4a70b61c87d641a31248604bf1982b0
```

### `dpkg` source package: `xz-utils=5.4.5-0.1`

Binary Packages:

- `liblzma5:amd64=5.4.5-0.1`

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
$ apt-get source -qq --print-uris xz-utils=5.4.5-0.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.5-0.1.dsc' xz-utils_5.4.5-0.1.dsc 2451 SHA512:0b9ced6c1342de46678b59930c817f803f18562d0651b568e80b9801b702e51fdebeb9b20cc8d1b1e68e4faccdf45e927181be5be7175f0e8d266074b7e63419
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.5.orig.tar.xz' xz-utils_5.4.5.orig.tar.xz 1680520 SHA512:5cbc3b5bb35a9f5773ad657788fe77013471e3b621c5a8149deb7389d48535926e5bed103456fcfe5ecb044b236b1055b03938a6cc877cfc749372b899fc79e5
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.5.orig.tar.xz.asc' xz-utils_5.4.5.orig.tar.xz.asc 833 SHA512:7390e991d6eccc8bb2fd3d319fcde92df0abcdc163bd0210a1d5f6c7a80268f36ead88ce1ae1d6935084f608b515ed1cd87c30085fcc2ee9222fc78c4a37ddbb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.4.5-0.1.debian.tar.xz' xz-utils_5.4.5-0.1.debian.tar.xz 26744 SHA512:0a5c8357ad809126e5585812d58416da135311cadb81c8d5a8a06f6c188298d041a334650247c2f0d67766107b9947038e50fd7c2bcab13d0edc72e24921021f
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
