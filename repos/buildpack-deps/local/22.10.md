# `buildpack-deps:kinetic`

## Docker Metadata

- Image ID: `sha256:db54a842dfeadd0fafb843607483607f5a218d73c908a50a0428dc86fd5216c3`
- Created: `2022-06-07T02:22:20.633881881Z`
- Virtual Size: ~ 718.01 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.3.1-1`

Binary Packages:

- `libacl1:amd64=2.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1-1.dsc' acl_2.3.1-1.dsc 2486 SHA512:8eb7f71030d7c4d355886390f12ffd7f66605bb2082a9a9de2eea0918aefe7b7cf1c26a3f8872681f5b3074df1cf07c4d01ae564bcba5b400b048b0e34b233c2
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1.orig.tar.xz' acl_2.3.1.orig.tar.xz 355676 SHA512:7d02f05d17305f8587ab485395b00c7fdb8e44c1906d0d04b70a43a3020803e8b2b8c707abb6147f794867dfa87bd51769c2d3e11a3db55ecbd2006a6e6231dc
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1.orig.tar.xz.asc' acl_2.3.1.orig.tar.xz.asc 833 SHA512:be046f3bf1ac7e21d2a07bf6ea87c1fedeed2f9d370d8bf3de1aa0c448de5484b1523697415849b6b7ca23e48e3df5353f6aebe850eb20fc2044d2681c71f298
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.3.1-1.debian.tar.xz' acl_2.3.1-1.debian.tar.xz 27732 SHA512:2fdfcd8daa1919e850cd3ed634b4141d65bbf7847eaf0a7899b6e8ae52fe2fa15de3378f6487a9224d00eb530cf5b285cc3b6272af66fcdcf1f29f2838648083
```

### `dpkg` source package: `adduser=3.121ubuntu1`

Binary Packages:

- `adduser=3.121ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.121ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.121ubuntu1.dsc' adduser_3.121ubuntu1.dsc 1804 SHA512:5d884c2b792bb2197c4d9855f06a1c778a346d8473f77f836fab34ff3adeb9197c7221bca622a92bb5f20fdadb53abb6538b6da2ed4f80d7f83ac84e55cf4464
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.121ubuntu1.tar.xz' adduser_3.121ubuntu1.tar.xz 228260 SHA512:0d47de2e87f6e4327831eb875b5db322d197e50c207f2b574297cd0e782ced11dfffd2f6c1cc42d1d49efecfd491bbc26a26cb99a62cacb1a34a201c5ceab4c7
```

### `dpkg` source package: `aom=3.3.0-2`

Binary Packages:

- `libaom3:amd64=3.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libaom3/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `ISC`
- `public-domain-md5`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/aom/3.3.0-2/


### `dpkg` source package: `apr-util=1.6.1-5ubuntu4`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-5ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu4.dsc' apr-util_1.6.1-5ubuntu4.dsc 2266 SHA512:ed049fbfc6316f2c014c0933851de8fa3d671d62ef9e68f153ba39d9e0bcbd9a627fee9902773fca85c6bb35b264ddc247f50aacd3f1773175be09cfd0d1a585
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA512:40eff8a37c0634f7fdddd6ca5e596b38de15fd10767a34c30bbe49c632816e8f3e1e230678034f578dd5816a94f246fb5dfdf48d644829af13bf28de3225205d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu4.debian.tar.xz' apr-util_1.6.1-5ubuntu4.debian.tar.xz 342880 SHA512:01795e95ce4b5003c3622925151caea9bdf0104d33f1d4ef4279429bfdf4a381749e6019658bdc9037fabde0aab6c9f6b437e81303b89364f0f5385f34ad4070
```

### `dpkg` source package: `apr=1.7.0-8build1`

Binary Packages:

- `libapr1:amd64=1.7.0-8build1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-8build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-8build1.dsc' apr_1.7.0-8build1.dsc 1951 SHA512:c9da10b8d05e62a7e5e25832408e97f2c512592bc9ea4f6d55e7edcb28ca3c7a9446492eef0c3c26ee67b31d99307b70e6bc4c655454fa983f5da263fd8a73c0
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA512:3dc42d5caf17aab16f5c154080f020d5aed761e22db4c5f6506917f6bfd2bf8becfb40af919042bd4ce1077d5de74aa666f5edfba7f275efba78e8893c115148
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA512:19b2b128c7c4cb40db06149c75325013a716c783e28e366c1bacf289fdb5d305e5779d8dc55a63729250ad3338cd4c726e133c788fe53ab3519f1bc8d4da6f90
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-8build1.debian.tar.xz' apr_1.7.0-8build1.debian.tar.xz 215944 SHA512:c11d784190391ea47706d34c7d324804ca9e8402bbb11cc9fecbb38827f0454a6ef8a8f8003f5e0b597fbc2e38da663e6bbeef371aa6a1685bb3c6f401030b6c
```

### `dpkg` source package: `apt=2.5.0`

Binary Packages:

- `apt=2.5.0`
- `libapt-pkg6.0:amd64=2.5.0`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.5.0
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.5.0.dsc' apt_2.5.0.dsc 2933 SHA512:9195e965411d9c5d037f9b4417815cd4d33159484c2cf907076c3f3eec071903b8f9d3aa30a254aecfae74142a2392b8482ccd6d421cbf1c4aa5e805c2db859d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.5.0.tar.xz' apt_2.5.0.tar.xz 2218792 SHA512:9631e1435cb2ec124872e112d59e748fc48077c56906d797a36bfeeaf53b8e923f3c9d48da02ec6a030f7d0004828a3a9fe493e1a1aec6a93319a9e3f50c334e
```

### `dpkg` source package: `attr=1:2.5.1-1build1`

Binary Packages:

- `libattr1:amd64=1:2.5.1-1build1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.5.1-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1-1build1.dsc' attr_2.5.1-1build1.dsc 2134 SHA512:4beeec510cf7976a3b2c0de3b90974ef03886b3a98ccb2b74f6278ed988727af3a0fa432d86aefd3bdb4bc50e29b3351f11fd892512407203f3e61636290ae15
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA512:9e5555260189bb6ef2440c76700ebb813ff70582eb63d446823874977307d13dfa3a347dfae619f8866943dfa4b24ccf67dadd7e3ea2637239fdb219be5d2932
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA512:be4f3629ef66bd400bcdeaf8b6b1564dc729472a514d59fb4909a30f3269711dedea16002283e9aabbf83c374e0a3d70bc00f1136da0fed66a8184acdfd7e78f
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1-1build1.debian.tar.xz' attr_2.5.1-1build1.debian.tar.xz 28032 SHA512:c9d0869a3bb9f8019e6764fee3a78d8b1b9a3cdb37968aac19a9a7e7bbeeaadcbad86d5363ce3b0e26b5a178a4d446e4097d095e17b7a6d7f3e595d07176675c
```

### `dpkg` source package: `audit=1:3.0.7-1build1`

Binary Packages:

- `libaudit-common=1:3.0.7-1build1`
- `libaudit1:amd64=1:3.0.7-1build1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0.7-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.7-1build1.dsc' audit_3.0.7-1build1.dsc 2771 SHA512:beb14e23239ab9c87dd4a57821d7d557a14a3e67f66306110ef87cd77cd2c07426f3bc8413d757618f886c5059e9bf624347753170708e0ad39b90f96fd51053
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.7.orig.tar.gz' audit_3.0.7.orig.tar.gz 1180226 SHA512:b5662b32082fc2ac54e247aa0db5442d76afa30134ebba1d624a17004e9ccf6856bb75344af4ce9d9a0a66c03e1c6f18b7d45658d7df13ea71af0c8362e08d70
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.7-1build1.debian.tar.xz' audit_3.0.7-1build1.debian.tar.xz 17772 SHA512:cdf346fc7dc04e42b44a9089fb7c01e68ea54ccd20d3eef8100d0cd8eed8ebd0764d8fd6ceab133faa0bfeee18e3cfe7625d230600b0e34ed0c19a7b739ec783
```

### `dpkg` source package: `autoconf=2.71-2`

Binary Packages:

- `autoconf=2.71-2`

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
$ apt-get source -qq --print-uris autoconf=2.71-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.71-2.dsc' autoconf_2.71-2.dsc 1988 SHA512:c5757e1208aa8749f0b37953b7440847691759c66f9c313f3541bdfb837a17d02341254bf8cb6db43a01005c8aa9a247101283598c5ce4014a47daf9e61d2b0a
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.71.orig.tar.gz' autoconf_2.71.orig.tar.gz 2003781 SHA512:2bc5331f9807da8754b2ee623a30299cc0d103d6f98068a4c22263aab67ff148b7ad3a1646bd274e604bc08a8ef0ac2601e6422e641ad0cfab2222d60a58c5a8
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.71-2.debian.tar.xz' autoconf_2.71-2.debian.tar.xz 23588 SHA512:578c6ccf29c3e46f4bd109a7fb17d55ae7e0fa1db1082e91da00b320bcd7699872cb1db1ea5c8d9034f20c13d00010e1dceea6013f46fe67bf5d406a8485914a
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

### `dpkg` source package: `base-files=12ubuntu5`

Binary Packages:

- `base-files=12ubuntu5`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `base-passwd=3.5.52build1`

Binary Packages:

- `base-passwd=3.5.52build1`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.52build1
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.52build1.dsc' base-passwd_3.5.52build1.dsc 1320 SHA512:2071171adf14d276664526662fab08d34a45a259ebcdbee7ae57bb004d3d12793e629006a37b649f16c0f04856e9f7bb79fb92fe304525167f48e73dec0cc4fd
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.52build1.tar.xz' base-passwd_3.5.52build1.tar.xz 54252 SHA512:699ffe50f4a7fbdea2c0b25d3b2452d538598870cf39b84668d9b7efa20ec41284c331513e89c966e7248732b1ec1abdfdb871e31f8e9efa026c691e89236ffe
```

### `dpkg` source package: `bash=5.1-6ubuntu1`

Binary Packages:

- `bash=5.1-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-6ubuntu1.dsc' bash_5.1-6ubuntu1.dsc 2426 SHA512:9c808b5b8a281e01c5a4a503eca84fca8b21a2153dc4e7abbedda21346ae4005c806ffe7afd689b7ff66af8d431b9b4bebf2f1324745c01ed5f3ee219a515a88
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA512:95d3acc542231cb893e1347c7d9dd66687f68cd347a0e9e126fde2d14e68c5b5530d1a5866eafa781e88aa013fcf72b4ad56d2e484c2ac7a69bd90bb149a9b86
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-6ubuntu1.debian.tar.xz' bash_5.1-6ubuntu1.debian.tar.xz 99652 SHA512:da77655882d0977656b75c750589307c54c7d5dd28b1cfc357d4a474ebf26399a91cfa19c4ba381e0a59a8f115f8381d432e82f2e659cb9bcbebf3fa0cd77bc1
```

### `dpkg` source package: `binutils=2.38-4ubuntu1`

Binary Packages:

- `binutils=2.38-4ubuntu1`
- `binutils-common:amd64=2.38-4ubuntu1`
- `binutils-x86-64-linux-gnu=2.38-4ubuntu1`
- `libbinutils:amd64=2.38-4ubuntu1`
- `libctf-nobfd0:amd64=2.38-4ubuntu1`
- `libctf0:amd64=2.38-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.38-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.38-4ubuntu1.dsc' binutils_2.38-4ubuntu1.dsc 8799 SHA512:29b9c64c93449f6c0824fb67076cdfd1f59dd20677311d55665e496d0b9943301d799282007502e3c2d07bd516911263dc578b07d0a704e438c75f48a58b6493
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.38.orig.tar.xz' binutils_2.38.orig.tar.xz 23651408 SHA512:8bf0b0d193c9c010e0518ee2b2e5a830898af206510992483b427477ed178396cd210235e85fd7bd99a96fc6d5eedbeccbd48317a10f752b7336ada8b2bb826d
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.38-4ubuntu1.debian.tar.xz' binutils_2.38-4ubuntu1.debian.tar.xz 282692 SHA512:eb921a69a55f9a45830b2b1ca8a600066bff29adf8850d481fe853ac7a1fb61febacd6ce092790aad5d1033b2ace766951d88776cd81889cf57b437fe824cd46
```

### `dpkg` source package: `brotli=1.0.9-2build6`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2build6`
- `libbrotli1:amd64=1.0.9-2build6`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2build6
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build6.dsc' brotli_1.0.9-2build6.dsc 1940 SHA512:9294702945cdaadad51f8690e7454d06b3281f94429123a4353cfdcce9eac598e9ad827f97f74798a7e958147aafec059022214b3bb7fe1db6337bebec2774b4
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build6.debian.tar.xz' brotli_1.0.9-2build6.debian.tar.xz 5812 SHA512:a50a2e8ce37aa228c3074f657d5591cd509f6b34e78b3b16b044072886c184623994a6420e5c0759a2bab1df26ba69462692c7d2c59bdc72f9683b7df884771c
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

### `dpkg` source package: `ca-certificates=20211016`

Binary Packages:

- `ca-certificates=20211016`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20211016
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20211016.dsc' ca-certificates_20211016.dsc 1890 SHA512:fab268d15ac882b5a39939a04edd613761b284781bf2fecadce13ce38815e5b1afa6fc4001c2076a355e9257f52b942ac0e38e943f587536f79e1876c3f670c9
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20211016.tar.xz' ca-certificates_20211016.tar.xz 239608 SHA512:bedf072c8aa1b05b249ea272f5cecfe16bdcd762c02c712323f12ac7a278e8814453f5f3caad86a2581e451788b292ed3a76a6a81620926459bb890133cffde1
```

### `dpkg` source package: `cairo=1.16.0-5ubuntu2`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-5ubuntu2`
- `libcairo-script-interpreter2:amd64=1.16.0-5ubuntu2`
- `libcairo2:amd64=1.16.0-5ubuntu2`
- `libcairo2-dev:amd64=1.16.0-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-5ubuntu2.dsc' cairo_1.16.0-5ubuntu2.dsc 2880 SHA512:e9415592136e7f42794f20d8c74fed895347a95d3ffd89621440c1e12212f65083926613e87fc6ad6df8f669058dc20ad12b2e1bdee2d7a7f85ec0b7c0dd4e26
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA512:9eb27c4cf01c0b8b56f2e15e651f6d4e52c99d0005875546405b64f1132aed12fbf84727273f493d84056a13105e065009d89e94a8bfaf2be2649e232b82377f
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-5ubuntu2.debian.tar.xz' cairo_1.16.0-5ubuntu2.debian.tar.xz 33368 SHA512:d51b6655b5ea60420bb80252fbcfe2e31cbef6242043457195eab60716b84dc9ae68eb4de95214b10a5ec6d5675891067a4940b58c2249602f0f355b9d31d8d4
```

### `dpkg` source package: `cdebconf=0.261ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.261ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.261ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.261ubuntu1.dsc' cdebconf_0.261ubuntu1.dsc 2941 SHA512:18554e0d66831166d01e199612aa1cd43ed56e00995d62329f2c951143860bc413870acf71f4d0e72e228ce70e6a09c97d87750e5ada1a48beaf4b39d675084c
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.261ubuntu1.tar.xz' cdebconf_0.261ubuntu1.tar.xz 297016 SHA512:6c2c8e2dccdb923ae6dc6a6b3873e6a56f6bdc4a6298c0576f60cb8d5c63bd06c4b9dac4ada4abd0d672a4e54509ad558fc9d1424a8029568d8d86cb54926390
```

### `dpkg` source package: `coreutils=8.32-4.1ubuntu1`

Binary Packages:

- `coreutils=8.32-4.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.32-4.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-4.1ubuntu1.dsc' coreutils_8.32-4.1ubuntu1.dsc 2291 SHA512:891c9ffe7dbdc3603bddd3bd4f89c26f9c348c19a59c36ba4fb4659090bcac02bf72e349c71b64b94fa3f398681956738d67c3c7cc2cc8090eec1287b01b6959
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz' coreutils_8.32.orig.tar.xz 5547836 SHA512:1c8f3584efd61b4b02e7ac5db8e103b63cfb2063432caaf1e64cb2dcc56d8c657d1133bbf10bd41468d6a1f31142e6caa81d16ae68fa3e6e84075c253613a145
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz.asc' coreutils_8.32.orig.tar.xz.asc 833 SHA512:9c73b35c9e8f7c2b8eff317afcb5aa3234c5f41c80d1882f3c2342906f3fdc876ae45d1256dd1b8fd3cb58c50925f3c13f93de5018626634fdca3c72c14a9acb
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-4.1ubuntu1.debian.tar.xz' coreutils_8.32-4.1ubuntu1.debian.tar.xz 41096 SHA512:74adfa2f2a85af8d7024ad6d13942e915217dcb10e29caa9c314e0a15da6ec019e7aa52ac5351c35ccea1bace7a05c6dc7569b7b0487c8fcd46b3ba42d66d89d
```

### `dpkg` source package: `curl=7.83.1-1ubuntu1`

Binary Packages:

- `curl=7.83.1-1ubuntu1`
- `libcurl3-gnutls:amd64=7.83.1-1ubuntu1`
- `libcurl4:amd64=7.83.1-1ubuntu1`
- `libcurl4-openssl-dev:amd64=7.83.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg-6ubuntu1`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg-6ubuntu1`
- `libsasl2-modules-db:amd64=2.1.28+dfsg-6ubuntu1`

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
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-6ubuntu1.dsc' cyrus-sasl2_2.1.28+dfsg-6ubuntu1.dsc 3570 SHA512:a152639cba35898c8d905bbcbbce9b0556edd10f9e8b523c4a3d7995396e0a678cb332b591244062bb19f7688bee317e8fde50f930cf90018e20e6bc37d4d663
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg.orig.tar.xz 797472 SHA512:70cccbac70e71828f1345beba5c78c14332e425b75c84a66393cf62ecf6848741c5912697fc0197516f1d4c41ec8c9644506a6241588b8f6bf5bba79edd8b15a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-6ubuntu1.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg-6ubuntu1.debian.tar.xz 94360 SHA512:3d3f925f18cd1ee64ff70779767d7c74a2eb768125636cb23b4e6e20744f2e725828df39c33fda8780643e6f2608375f4ebb5cb1668a0f555b328eb35184f4e6
```

### `dpkg` source package: `dash=0.5.11+git20210903+057cd650a4ed-3build1`

Binary Packages:

- `dash=0.5.11+git20210903+057cd650a4ed-3build1`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `Expat`
- `FSFUL`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.9`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.9`
- `libdb5.3-dev=5.3.28+dfsg1-0.9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.9
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.9.dsc' db5.3_5.3.28+dfsg1-0.9.dsc 2628 SHA512:73bb2d91ad3dc1a642e1d7bc238478d1531513e3950ca4694ce4971faf5b0ec62cd0fa9ac529c94632d9cc225a3f72b4bf2c4ffe052b0212b719a559551ab53f
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA512:50cb87bc3f24065839ee2932e82af032b236b290ebe89983076f503c6c62c5f36ff93d7847a3f68b2b19f35088fbab5d3ac6a34553d07e8148e68e9a3f079a12
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.9.debian.tar.xz' db5.3_5.3.28+dfsg1-0.9.debian.tar.xz 31576 SHA512:1a2baf51c47d5450769454c98e1b60934c7cf624a0b58cdf073835a35a628cf4bea4f002232f06a55c372cc9ba902cfcb42841754299f313b7cacebb02c4a19f
```

### `dpkg` source package: `debconf=1.5.79ubuntu1`

Binary Packages:

- `debconf=1.5.79ubuntu1`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.79ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.79ubuntu1.dsc' debconf_1.5.79ubuntu1.dsc 2077 SHA512:0aac451b347a5f6758ab2e468c25ea8061840519412210861a13ced479d5e6bb2a3abd469cb0cf68d80f1f9c4debba28501141055eb2eb1ac1701f800cdd83ba
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.79ubuntu1.tar.xz' debconf_1.5.79ubuntu1.tar.xz 570660 SHA512:1bf6de4d1cec7475f64d9bdaa47ef6dcb3d1181bcb3b97076ec60213534aa344ca49d552fdcb5c6fde4d42c364b8242bb4880de0a787493868383e6db36f9e5f
```

### `dpkg` source package: `debianutils=5.7-0.2`

Binary Packages:

- `debianutils=5.7-0.2`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.7-0.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.7-0.2.dsc' debianutils_5.7-0.2.dsc 1542 SHA512:ef393fe10de8d84dedc38e60ca4760c93b02ecdcf6b1930d30f2e230dfbc002a5113459f430ac850df90285f534553db4e6ee6c533c9b25b8eb99594d533ce58
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.7.orig.tar.gz' debianutils_5.7.orig.tar.gz 257231 SHA512:79acd8885abca93842d696167171a359011c49a40f38deeb25bc94d62905f95afa3a7b2540d3bd4b0ffd363c5c48a439a1a68139a29d6c033980b019cea75d92
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.7-0.2.debian.tar.xz' debianutils_5.7-0.2.debian.tar.xz 21664 SHA512:9984de24acd5a8cb9dfad84ba5d26689a808a0a9a23f231c099f30a3dbe1ade2e3eaec758b0f4e358d0f79d0b2d97ad164df78f58b776afcf76085ddf47a4172
```

### `dpkg` source package: `diffutils=1:3.8-0ubuntu2`

Binary Packages:

- `diffutils=1:3.8-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.8-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8-0ubuntu2.dsc' diffutils_3.8-0ubuntu2.dsc 1821 SHA512:645b14680e3669261eb372ce523d8258ee65b010b4e290650f8a0a4c922a26f80ee381e3711b2bf01249d64e248c184f8898abc6e0e50cb9f64cbd647ab1f684
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz' diffutils_3.8.orig.tar.xz 1585120 SHA512:279441270987e70d5ecfaf84b6285a4866929c43ec877e50f154a788858d548a8a316f2fc26ad62f7348c8d289cb29a09d06dfadce1806e3d8b4ea88c8b1aa7c
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz.asc' diffutils_3.8.orig.tar.xz.asc 833 SHA512:0464ac89209411993800666b45ff90243d22fbda53bf1d71c6870d565b39cc8d9c54c141b9d297a181ce74ad8fb5313953f416bced179ff7728a52a3e9a4f5a5
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8-0ubuntu2.debian.tar.xz' diffutils_3.8-0ubuntu2.debian.tar.xz 11692 SHA512:fab99ca407c3b1bbc427ebf14595d540e6ad2957e9b43065005efd9d5b423e6a4d6d460cccd05faf5786193a5bf1cf46721743e580161d5004167eca15fc405b
```

### `dpkg` source package: `djvulibre=3.5.28-2build2`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.28-2build2`
- `libdjvulibre-text=3.5.28-2build2`
- `libdjvulibre21:amd64=3.5.28-2build2`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.28-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-2build2.dsc' djvulibre_3.5.28-2build2.dsc 2046 SHA512:9f4f35666510ca672084a023227435af0b9adb08bddef262eda079d8b3d69718a218a2ae442068ef2c02a81da0bc783075ea833df23a499b1e7f5f8835f9491e
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28.orig.tar.xz' djvulibre_3.5.28.orig.tar.xz 2959024 SHA512:4fdbecd2b7b583ee4211c9cda6638a3a831c883e2552b3c8ad09f69e8734831addc14f590faab8c58d7f9f017b527abccc384f6066e674e341cf43c96db49cb7
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-2build2.debian.tar.xz' djvulibre_3.5.28-2build2.debian.tar.xz 17552 SHA512:f66fd65d191043f0976a376668ec9ac60764491ec841577b4dd3bc868da1d293474a2fced48d87f86b6b0225a7e7322196803bd0a198993b838c823e50eee7e8
```

### `dpkg` source package: `dpkg=1.21.7ubuntu3`

Binary Packages:

- `dpkg=1.21.7ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `dpkg=1.21.8ubuntu1`

Binary Packages:

- `dpkg-dev=1.21.8ubuntu1`
- `libdpkg-perl=1.21.8ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.8ubuntu1.dsc' dpkg_1.21.8ubuntu1.dsc 2167 SHA512:a80c3206878dad12eb9b313e60cba6d013f2ee8447ff45ece9958a40294362bdf00b295f4caeca86e9a853c31efb63704c5aa99f5225570ebdb2f2d8156b3242
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.8ubuntu1.tar.xz' dpkg_1.21.8ubuntu1.tar.xz 5092172 SHA512:41986538261be4a7c85407a3fe2f42119cf98345b6a2443272e53d01dea694420adbe0a8da0d62aaedc9f4efe4708b942a2f736f1bfde30e7e082983eaa73310
```

### `dpkg` source package: `e2fsprogs=1.46.5-2ubuntu1`

Binary Packages:

- `comerr-dev:amd64=2.1-1.46.5-2ubuntu1`
- `e2fsprogs=1.46.5-2ubuntu1`
- `libcom-err2:amd64=1.46.5-2ubuntu1`
- `libext2fs2:amd64=1.46.5-2ubuntu1`
- `libss2:amd64=1.46.5-2ubuntu1`
- `logsave=1.46.5-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `elfutils=0.187-1`

Binary Packages:

- `libelf1:amd64=0.187-1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.187-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.187-1.dsc' elfutils_0.187-1.dsc 3218 SHA512:334bf178060b8d32b27519bfc8169d467c93d34eddbbbd519fb0e21b9b7717f122a539c284600179be2fd8ad91f24dc3cdbd0619b5a98353170ae142d00b9f95
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.187.orig.tar.bz2' elfutils_0.187.orig.tar.bz2 9240221 SHA512:a9b9e32b503b8b50a62d4e4001097ed2721d3475232a6380e6b9853bd1647aec016440c0ca7ceb950daf1144f8db9814ab43cf33cc0ebef7fc91e9e775c9e874
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.187-1.debian.tar.xz' elfutils_0.187-1.debian.tar.xz 37944 SHA512:bb5205ef1df968bdfbeb9bd6ccbd7c72e9a5a48b728cc8ec8ebe1bd15a403a5f4a5d9f2b6ee49828ae704c519ffdd936da767fc9e450add854581f08e7254a71
```

### `dpkg` source package: `expat=2.4.8-1`

Binary Packages:

- `libexpat1:amd64=2.4.8-1`
- `libexpat1-dev:amd64=2.4.8-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.4.8-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.8-1.dsc' expat_2.4.8-1.dsc 1981 SHA512:78c3bc4c124233d38a690e6dc9e4db0df055fd0e75c75829537b5f62354c08e5a67f14ac6da99d8e070f615f64fa602f3f8062dad14aecc12262ad21d959690a
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.8.orig.tar.gz' expat_2.4.8.orig.tar.gz 8316762 SHA512:452982888e993937dc37968f27eed080d8fb8c8d98935051b195e11051de8fe31217a4d40ae3e7df53fe3265b897823a2a7793af794fd066e0ead4535b5cbc99
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.8-1.debian.tar.xz' expat_2.4.8-1.debian.tar.xz 12556 SHA512:29e304ea46382a34d543a4b079968d493b927ea3272e97e45dffbc5885e39b999bede568628e58e5fc8e973d9c0382d17b114f26d506806577a9497789d850ed
```

### `dpkg` source package: `fftw3=3.3.8-2ubuntu8`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2ubuntu8`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu8.dsc' fftw3_3.3.8-2ubuntu8.dsc 2673 SHA512:f0e7a1991fe120a3048d22a02f90adf7d934ad95a82ecc36360fa760a5125cf58d3e2dc6167dc847723af6f61720f95019895fcb8f8d0fc6902e39017aed944c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA512:ab918b742a7c7dcb56390a0a0014f517a6dff9a2e4b4591060deeb2c652bf3c6868aa74559a422a276b853289b4b701bdcbd3d4d8c08943acf29167a7be81a38
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu8.debian.tar.xz' fftw3_3.3.8-2ubuntu8.debian.tar.xz 14356 SHA512:99280a373b3c5a19d472e8bd23495759aa905aec12c3c01b3f3399fd1a300b4a0cb847369efad9690ec85bf8e9206428f9bf707edc0c665485362aa6cfaf1722
```

### `dpkg` source package: `file=1:5.41-4`

Binary Packages:

- `file=1:5.41-4`
- `libmagic-mgc=1:5.41-4`
- `libmagic1:amd64=1:5.41-4`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.41-4
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41-4.dsc' file_5.41-4.dsc 2240 SHA512:ea167ca43bb61dda225ace97dd80a9c18e7fa1026f147f629d686f977fdfc0271cd0a91de166b1e960e9d2a79afdfab815fac9ae0d36c46162d440c7bcf4f8cf
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41.orig.tar.gz' file_5.41.orig.tar.gz 1064097 SHA512:bbf2d8e39450b31d0ba8d76d202790fea953775657f942f06e6dc9091798d4a395f7205e542388e4a25b6a4506d07f36c5c4da37cfce0734133e9203a3b00654
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41.orig.tar.gz.asc' file_5.41.orig.tar.gz.asc 169 SHA512:ce9c2b1ccb5900cd2e16f0a77b2e727cd472436355b846784d36b97c7239430eceb6101a2364f2dabeb6723bec38e8fa69ed09bfd859839b76701363fe88b590
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41-4.debian.tar.xz' file_5.41-4.debian.tar.xz 34300 SHA512:cf716c1d73fa8f93538e5bbc9a89f623b6eae2665b775817c761b75fd56a66bb92f45a1b662daa96e4ab79451f47f564f1bb12061d7205b0644466e190093092
```

### `dpkg` source package: `findutils=4.8.0-1ubuntu3`

Binary Packages:

- `findutils=4.8.0-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.8.0-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0-1ubuntu3.dsc' findutils_4.8.0-1ubuntu3.dsc 2064 SHA512:3f0f5195138342ce515ff83f5e653457d78158c8b871ef04002adb4cc69cab6023c71f7d1032db7032d25806c22a8ad33dbf3007018d382968863521a33af2cd
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz' findutils_4.8.0.orig.tar.xz 1983096 SHA512:eaa2da304dbeb2cd659b9210ac37da1bde4cd665c12a818eca98541c5ed5cba1050641fc0c39c0a446a5a7a87a8d654df0e0e6b0cee21752ea485188c9f1071e
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz.asc' findutils_4.8.0.orig.tar.xz.asc 488 SHA512:e6ea8bd9a58ac4f787a9cc7dad9f75fab9e0623e7cda463bef60651c9319574ac7c8ba06f7d33cbead0ecb8788db71eb39f50550deb066d6d6baa625b0374a45
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0-1ubuntu3.debian.tar.xz' findutils_4.8.0-1ubuntu3.debian.tar.xz 27716 SHA512:f0ce8b61f4e0beabad3178424c804468dc4c57f37794887954df28c36227ce77f00383903274a1995a104f9def44270070b9e033eb46d52f5aaaedb1f5883587
```

### `dpkg` source package: `fontconfig=2.13.1-4.4ubuntu1`

Binary Packages:

- `fontconfig=2.13.1-4.4ubuntu1`
- `fontconfig-config=2.13.1-4.4ubuntu1`
- `libfontconfig-dev:amd64=2.13.1-4.4ubuntu1`
- `libfontconfig1:amd64=2.13.1-4.4ubuntu1`
- `libfontconfig1-dev:amd64=2.13.1-4.4ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-4.4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-4.4ubuntu1.dsc' fontconfig_2.13.1-4.4ubuntu1.dsc 2449 SHA512:dcfd5e5e0036b362b90dab6467384de285499e5478291d77e4e9bb6d28831bcbbdf1497514e4f649454d6acb51ea52ac6da378e86bbf00313d04c565b3051768
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA512:f97f2a9db294fd72d416a7d76dd7db5934ade2cf76903764b09e7decc33e0e2eed1a1d35c5f1c7fd9ea39e2c7653b9e65365f0c6205e047e95e38ba5000dd100
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-4.4ubuntu1.debian.tar.xz' fontconfig_2.13.1-4.4ubuntu1.debian.tar.xz 29124 SHA512:8075b5d4ddb11b79ff05bb5292294784c6e0a4a36e92faac89d2b84585ed741ae4a482e7c03aa499aad161918627e635ef272022a6bbc3be4b9b17dc283bb685
```

### `dpkg` source package: `fonts-dejavu=2.37-2build1`

Binary Packages:

- `fonts-dejavu-core=2.37-2build1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2build1.dsc' fonts-dejavu_2.37-2build1.dsc 2411 SHA512:7821679b0f3cabaa4929b11a1a02fff21c05cef965efc399bf8a89b8549b1ac20cdd173c2cb31c397a345683b197623b97998b412c8458a135141ccd733b50d9
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA512:e61fc8c675ef76edb49dd9a8caee62087280929bb8144b52aca2f8def30025c56246589ad8a6a806b9574e6876eedd16d57c70a6ce9c86817a2dfe39d8a2bb2b
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2build1.debian.tar.xz' fonts-dejavu_2.37-2build1.debian.tar.xz 11468 SHA512:b3c0cb3c81b3e4e9d76eefab010f447be973fa9e310960d2e3a1a2e845f4388e0508f8d18d519c7374c68c96c2e05a75f29ccf24135f6250a82181a77d8e9741
```

### `dpkg` source package: `freetype=2.12.1+dfsg-2`

Binary Packages:

- `libfreetype-dev:amd64=2.12.1+dfsg-2`
- `libfreetype6:amd64=2.12.1+dfsg-2`
- `libfreetype6-dev:amd64=2.12.1+dfsg-2`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/freetype/2.12.1+dfsg-2/


### `dpkg` source package: `fribidi=1.0.8-2ubuntu3.1`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2ubuntu3.1.dsc' fribidi_1.0.8-2ubuntu3.1.dsc 2442 SHA512:977cb7df4e1877f0f6d5f58620cfacbb1e25090c2bfd70c71576ada3c9f11f260ed11fb0fd64a5f5bf8cfc8c419a865e0e9b9084f224deb9dfadf1b2e3bd17e9
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA512:d66b1524b26d227fd6a628f438efb875c023ae3be708acaaad11f1f62d0902de0a5f57124458291ef2b0fcd89356c52ab8ae5559b0b5a93fa435b92f1d098ba2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2ubuntu3.1.debian.tar.xz' fribidi_1.0.8-2ubuntu3.1.debian.tar.xz 10888 SHA512:16e448db2038b60b3a086117774e734b1d3ed08ae09cfa1b591f5a95c6372778705ba8940dd464537d5a6e932528c1c1e01376670992580529090f20142d171a
```

### `dpkg` source package: `gcc-11=11.3.0-3ubuntu1`

Binary Packages:

- `cpp-11=11.3.0-3ubuntu1`
- `g++-11=11.3.0-3ubuntu1`
- `gcc-11=11.3.0-3ubuntu1`
- `gcc-11-base:amd64=11.3.0-3ubuntu1`
- `libasan6:amd64=11.3.0-3ubuntu1`
- `libgcc-11-dev:amd64=11.3.0-3ubuntu1`
- `libstdc++-11-dev:amd64=11.3.0-3ubuntu1`
- `libtsan0:amd64=11.3.0-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp-11/copyright`, `/usr/share/doc/g++-11/copyright`, `/usr/share/doc/gcc-11/copyright`, `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libgcc-11-dev/copyright`, `/usr/share/doc/libstdc++-11-dev/copyright`, `/usr/share/doc/libtsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.3.0-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.3.0-3ubuntu1.dsc' gcc-11_11.3.0-3ubuntu1.dsc 22812 SHA512:2b50ca612a54f664d3ea7a78ab9d73936e25e9f111a24a4e2822380bf44d6958de0f55f4d5eff8d250a4bfe15e34aab64bb28c64056e7481fa8985232177fce1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.3.0.orig.tar.gz' gcc-11_11.3.0.orig.tar.gz 88114483 SHA512:ab276f0a908187b3c1ad89e169f16822a6cf6bd245465510b94b7649eb1698e79e7be9d89c817ffbaefce373d3015be07512bf19960e74f9ebfdd8505ff547e2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.3.0-3ubuntu1.debian.tar.xz' gcc-11_11.3.0-3ubuntu1.debian.tar.xz 592132 SHA512:1b8d44174f23e3e1216f210f9ae92b4e688a0b1a124a92906ac4b3160cecbae63376c169f817b804c405bd9d5a6ae6b95fc98ec72483b134a5a1a05dc498d886
```

### `dpkg` source package: `gcc-12=12.1.0-2ubuntu1`

Binary Packages:

- `gcc-12-base:amd64=12.1.0-2ubuntu1`
- `libatomic1:amd64=12.1.0-2ubuntu1`
- `libcc1-0:amd64=12.1.0-2ubuntu1`
- `libgcc-s1:amd64=12.1.0-2ubuntu1`
- `libgomp1:amd64=12.1.0-2ubuntu1`
- `libitm1:amd64=12.1.0-2ubuntu1`
- `liblsan0:amd64=12.1.0-2ubuntu1`
- `libquadmath0:amd64=12.1.0-2ubuntu1`
- `libstdc++6:amd64=12.1.0-2ubuntu1`
- `libubsan1:amd64=12.1.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12.1.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12.1.0-2ubuntu1.dsc' gcc-12_12.1.0-2ubuntu1.dsc 27746 SHA512:2e86d82a816f394dc267fd03e2e51939cf4d7111458983eac035450a3578abb40b610d2c791396eddc2441af353c8c481bfbbfbe364832b015d84dc8600811b7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12.1.0.orig.tar.gz' gcc-12_12.1.0.orig.tar.gz 89394971 SHA512:9132ef095fcc5d683c71b9dc1b77b3af0f4f09b4b00d0e1f6ae1a46d5a4f7faf9e1112967722b6e3fcf72b6692326d036b1d370103b5362a7e19cd430b1ad18d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12.1.0-2ubuntu1.debian.tar.xz' gcc-12_12.1.0-2ubuntu1.debian.tar.xz 1661116 SHA512:042b8fb73ca91a531ca3046b844f0d8a4a53e8d07f1129290317151b12dbb5b9fa02975dd9bc01ef886ea8fa5dbe192f19ac8a587e0d761a573362899fe66a91
```

### `dpkg` source package: `gcc-defaults=1.193ubuntu1`

Binary Packages:

- `cpp=4:11.2.0-1ubuntu1`
- `g++=4:11.2.0-1ubuntu1`
- `gcc=4:11.2.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.193ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.193ubuntu1.dsc' gcc-defaults_1.193ubuntu1.dsc 14438 SHA512:ac90c126ec51cce73c134d24517c1dfe378d214ad6ee5c3edc119fec33c52485dd880994b29e7b787b2eea1cf761564b721044c903bea7deae2edc9031d3d8ed
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.193ubuntu1.tar.xz' gcc-defaults_1.193ubuntu1.tar.xz 48128 SHA512:62cf8f5b9aa4b2200cb037d18556c532178e9698f8502b53dd5a71bc9dfdab7314bda56d5384974fa4f9c23c16567c26ee966b5c3562d819507579932fb983a3
```

### `dpkg` source package: `gdbm=1.23-1`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-1`
- `libgdbm-dev:amd64=1.23-1`
- `libgdbm6:amd64=1.23-1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.23-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23-1.dsc' gdbm_1.23-1.dsc 2583 SHA512:f931348ff659e5f9485fe92734b02c426b6428e41e2abc180b131183e8ca437c5287a7f88854f788e5111efbed114b5eda2b66c24318b39e88661ddbbb39ce15
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz' gdbm_1.23.orig.tar.gz 1115854 SHA512:918080cb0225b221c11eb7339634a95e00c526072395f7a3d46ccf42ef020dea7c4c5bec34aff2c4f16033e1fff6583252b7e978f68b8d7f8736b0e025838e10
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz.asc' gdbm_1.23.orig.tar.gz.asc 181 SHA512:6653751c04584f10aa3325bd1cb5b9f7970a786dd2a99602ea620c11a86a9ba5c342aa52627bd06c03da822e9e1600dc034d9a8f42856a287fd67f6b9f161c71
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.23-1.debian.tar.xz' gdbm_1.23-1.debian.tar.xz 18484 SHA512:e7ca0a608da94e5b5bc5949e27b794c87e032202eb09359ad55f6c1a7a6e895f01126781a4e0fbfdb8fef3de7c4a312b9d5a653aaf55ce8c5afbceb945945253
```

### `dpkg` source package: `gdk-pixbuf=2.42.8+dfsg-1`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.42.8+dfsg-1`
- `libgdk-pixbuf-2.0-0:amd64=2.42.8+dfsg-1`
- `libgdk-pixbuf-2.0-dev:amd64=2.42.8+dfsg-1`
- `libgdk-pixbuf2.0-bin=2.42.8+dfsg-1`
- `libgdk-pixbuf2.0-common=2.42.8+dfsg-1`

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
$ apt-get source -qq --print-uris gdk-pixbuf=2.42.8+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.8%2bdfsg-1.dsc' gdk-pixbuf_2.42.8+dfsg-1.dsc 3123 SHA512:77ed414aa8bc3f6ed7c33d690a4d3f22fbf947e149bdb70694d420492fde7e67193fb688dc04efd7f48ff31ea067dde3c9c6cfcaa210216d6315756248b7bcbd
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.8%2bdfsg.orig.tar.xz' gdk-pixbuf_2.42.8+dfsg.orig.tar.xz 6439548 SHA512:d77093ac4bd5c8f9a5267e67958dd99db009e16f94c44be95a547cd291b6d03fcc35c4a02327dd9f4341af1ae2ecdaa6a1bec02dcf1116ec5a440d22b3f68924
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.8%2bdfsg-1.debian.tar.xz' gdk-pixbuf_2.42.8+dfsg-1.debian.tar.xz 19908 SHA512:d56c7ca401540b58d083292e43011910faa0fd7d92d0b3db1e844713784b32ec9746f6383db22e7bf64149f343cd057d113483d6205fcd521fc8b8bcf948550f
```

### `dpkg` source package: `git=1:2.36.1-1ubuntu1`

Binary Packages:

- `git=1:2.36.1-1ubuntu1`
- `git-man=1:2.36.1-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.36.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.36.1-1ubuntu1.dsc' git_2.36.1-1ubuntu1.dsc 2919 SHA512:01acdda0784efc83fafed21c1e036b8cc8eaf2704c9bd2bbfecc8d7767dcdd281f86aadffc9461bc49e33d5449fb0e19ab616235b8c46e2613be9a4d3a2eb661
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.36.1.orig.tar.xz' git_2.36.1.orig.tar.xz 7004044 SHA512:459432bd0c1d5a87c828a6fbf6d3473f14bf6b95783b3f27ea4f3af1ba9fd0e712a96a41276a16c6ebeb7ac3583a5f445eedd0a9e19fe160c2c8e309ec58818e
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.36.1-1ubuntu1.debian.tar.xz' git_2.36.1-1ubuntu1.debian.tar.xz 720200 SHA512:d79fef67c017584da847f0b20d7a3cf8a4a9112ada465a4bf38e6963ccb27a6459fc13c161c520d1e153e31acee3e549d30ef77515e189697fd20ba9598a3c27
```

### `dpkg` source package: `glib2.0=2.72.1-1`

Binary Packages:

- `libglib2.0-0:amd64=2.72.1-1`
- `libglib2.0-bin=2.72.1-1`
- `libglib2.0-data=2.72.1-1`
- `libglib2.0-dev:amd64=2.72.1-1`
- `libglib2.0-dev-bin=2.72.1-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/glib2.0/2.72.1-1/


### `dpkg` source package: `glibc=2.35-0ubuntu3`

Binary Packages:

- `libc-bin=2.35-0ubuntu3`
- `libc-dev-bin=2.35-0ubuntu3`
- `libc6:amd64=2.35-0ubuntu3`
- `libc6-dev:amd64=2.35-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.35-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35-0ubuntu3.dsc' glibc_2.35-0ubuntu3.dsc 8876 SHA512:80c5bf5c0b79c7b065a6766ac0ca27e0bda2ad7f2e413b663ef3d7f3979f0cd55334a8573b4724bb977d18a928536d8757c5c044f5988af18958ae76d2ec4d47
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35.orig.tar.xz' glibc_2.35.orig.tar.xz 18165952 SHA512:e7336ce27561be5d7c217832a1136fb327e057bd8d3f92925b35c97e3e9f9e486948b5a1e03e5e4090772ef06437a074d10b82e68f17f1ad8f22077ee39e1b66
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35.orig.tar.xz.asc' glibc_2.35.orig.tar.xz.asc 833 SHA512:2a1c152511dac05f9b4e48f7e7a6b59dbf2d8b71fea54f128173113357be26e86216e13c9865f617049e6858396a221a5abc704f65a786b22453945fd80265e9
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35-0ubuntu3.debian.tar.xz' glibc_2.35-0ubuntu3.debian.tar.xz 885776 SHA512:348cb29f6a9e68093dbfbf5f23b4db3f6e25f25bf9d2252b07dc199ed6882da07d0f223fa340439f29aa1eec0d418857e5c17bf1a2a3b361c9c8ef4524492ec3
```

### `dpkg` source package: `gmp=2:6.2.1+dfsg-3ubuntu1`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.1+dfsg-3ubuntu1`
- `libgmp10:amd64=2:6.2.1+dfsg-3ubuntu1`
- `libgmpxx4ldbl:amd64=2:6.2.1+dfsg-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg-3ubuntu1.dsc' gmp_6.2.1+dfsg-3ubuntu1.dsc 2355 SHA512:b41211a64cba1afee1ea7924d38581b26b36f0495ad42be6d25b7175d5fa1e000378a5d36dd80087b0e7d4495620edb1e7e1b32d6c1085a8cdf0a4cb460a0558
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA512:801948b7dcf592959ea387a86bee34dfb4e02c5e93815a785fc46174899ba22129853a3e34109a6df86048a144765c5f39e65fddfcecba879cc60da62f32fea0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg-3ubuntu1.debian.tar.xz' gmp_6.2.1+dfsg-3ubuntu1.debian.tar.xz 40996 SHA512:d7e0a1165a42b11a26a0f9232193db41ce2e7b1f5ea50d258e156fc9d80f9a74b6739491ec73cc1e909a3d09e029f90c3be1460c993690c5081ef8c6a169a4c3
```

### `dpkg` source package: `gnupg2=2.2.27-3ubuntu2`

Binary Packages:

- `dirmngr=2.2.27-3ubuntu2`
- `gnupg=2.2.27-3ubuntu2`
- `gnupg-l10n=2.2.27-3ubuntu2`
- `gnupg-utils=2.2.27-3ubuntu2`
- `gpg=2.2.27-3ubuntu2`
- `gpg-agent=2.2.27-3ubuntu2`
- `gpg-wks-client=2.2.27-3ubuntu2`
- `gpg-wks-server=2.2.27-3ubuntu2`
- `gpgconf=2.2.27-3ubuntu2`
- `gpgsm=2.2.27-3ubuntu2`
- `gpgv=2.2.27-3ubuntu2`

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
$ apt-get source -qq --print-uris gnupg2=2.2.27-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.27-3ubuntu2.dsc' gnupg2_2.2.27-3ubuntu2.dsc 3373 SHA512:fbe7a583145d47a71228fa102a687f46f0506a03fc7a77ff3a73dd7c850f3e1d53cafb164ea0299bc82f93cb95774b95c1d71b4e6bdeaabde19caba87ab46175
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2' gnupg2_2.2.27.orig.tar.bz2 7191555 SHA512:cf336962116c9c08ac80b1299654b94948033ef51d6d5e7f54c2f07bbf7d92c7b0bddb606ceee2cdd837063f519b8d59af5a82816b840a0fc47d90c07b0e95ab
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.27-3ubuntu2.debian.tar.xz' gnupg2_2.2.27-3ubuntu2.debian.tar.xz 66056 SHA512:84dcd0406f9ee7d890c18736dfe674aa3719ccda93288fdbcc36de9969f7fcca4bd3e54a347a37b85d0537fbbd8e5f9218da9a2a01c9bab3de64408cf7743491
```

### `dpkg` source package: `gnutls28=3.7.4-2ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.4-2ubuntu1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gobject-introspection=1.72.0-1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.72.0-1`
- `gir1.2-glib-2.0:amd64=1.72.0-1`
- `libgirepository-1.0-1:amd64=1.72.0-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.72.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.72.0-1.dsc' gobject-introspection_1.72.0-1.dsc 3197 SHA512:5ab663d2ffbd50e238c970808f8893c5d9de42b47d9b56c46e424135f85e6bbb43aab7a1e3a8737bea71e38c946cea469c482f148e96c236a6a784bcf76626a7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.72.0.orig.tar.xz' gobject-introspection_1.72.0.orig.tar.xz 1040936 SHA512:b8fba2bd12e93776c55228acf3487bef36ee40b1abdc7f681b827780ac94a8bfa1f59b0c30d60fa5a1fea2f610de78b9e52029f411128067808f17eb6374cdc5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.72.0-1.debian.tar.xz' gobject-introspection_1.72.0-1.debian.tar.xz 25752 SHA512:ea95a4876d73e31b87ebd869b7a1a12029f6c7205448b46b6452a0731338a1b5fe5adc724675dad8e57bca94e4b04a9a497b0a4ebe49dc9686ed1ab02c4a33ec
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

### `dpkg` source package: `grep=3.7-1build1`

Binary Packages:

- `grep=3.7-1build1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.7-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7-1build1.dsc' grep_3.7-1build1.dsc 1900 SHA512:3345c289bc163924615d3bc9ac3138e35870715d38223ef9d38a90ab17160fc415f8c0c9a5da1939143e2701e46fc854b27b45c280c4af686db2208f2becbe4f
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7.orig.tar.xz' grep_3.7.orig.tar.xz 1641196 SHA512:e9e45dcd40af8367f819f2b93c5e1b4e98a251a9aa251841fa67a875380fae52cfa27c68c6dbdd6a4dde1b1017ee0f6b9833ef6dd6e419d32d71b6df5e972b82
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7.orig.tar.xz.asc' grep_3.7.orig.tar.xz.asc 833 SHA512:9db28883b696fbbb0fad32f4ecd168954dc475d5f0a8f2b4f960ff615ef7dd8348a7caaee85a96287824472a29485ff921af121c582083ca5ad5c30960f99cf4
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7-1build1.debian.tar.xz' grep_3.7-1build1.debian.tar.xz 18184 SHA512:cbefc3635a0b0acc33d8a052d3ca7d583adbd1bcfc384559076b5e4f5508b4a8301b0dd54a029aecbab925a6f916c99a2d5bebe0a6936fe5ffeb5a07a0d9a917
```

### `dpkg` source package: `gzip=1.10-4ubuntu4`

Binary Packages:

- `gzip=1.10-4ubuntu4`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-4ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-4ubuntu4.dsc' gzip_1.10-4ubuntu4.dsc 2269 SHA512:65ca7a283eb955a928afbb3586234a77a06d7468af69f273a203ebddcb629cbb77f1a3e3b80573bd7968dc1ecb9cc3cd9b95c0948a6b941be06fccf27aa2203c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA512:7939043e74554ced0c1c05d354ab4eb36cd6dce89ad79d02ccdc5ed6b7ee390759689b2d47c07227b9b44a62851afe7c76c4cae9f92527d999f3f1b4df1cccff
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz.asc' gzip_1.10.orig.tar.gz.asc 833 SHA512:74727fb3a8b64f81b4dd2d941fa750a789c482d7ae604d0ecfbe5ec623780efc7c5f0e51d65e7b99c2f097c5cd6585cc3a0f1b31abb03306156e0d410d9f0186
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-4ubuntu4.debian.tar.xz' gzip_1.10-4ubuntu4.debian.tar.xz 39072 SHA512:faac8029bc9632865b0a8f2ddd42cce4cb63cb56df2aae6720fa37d28286775cab81c3193800e2350fbefb1a4ecea061f7943efb1385f5821fd0a47cd54efd8d
```

### `dpkg` source package: `harfbuzz=2.7.4-1ubuntu4`

Binary Packages:

- `libharfbuzz0b:amd64=2.7.4-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.7.4-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu4.dsc' harfbuzz_2.7.4-1ubuntu4.dsc 2847 SHA512:0394ecfdc858b0d556256fa5e3074f98d6922bd8fa62c8bdd228950b38a06161608fdfb2cdccace147ef9e724a3adeb540490412eee9bb6ca03d82bd80baaad7
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4.orig.tar.xz' harfbuzz_2.7.4.orig.tar.xz 9532468 SHA512:d2af6a768c397c664f654cf36140e7b5696b3b983f637454604570c348247f7ffea135048d9b02cf6593cbde728567e31bf82a39df5ff38d680c78dff24d4cf0
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu4.debian.tar.xz' harfbuzz_2.7.4-1ubuntu4.debian.tar.xz 11104 SHA512:0cc4d6b6753adf93cf0a3aaec1794bfa20d270b945ef8ca2d948239c9273959d7940f4a1dd7f68c56e8ba982e97e3f673a7d0cd229c82d91cc5fece6272dfd51
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

### `dpkg` source package: `hostname=3.23ubuntu2`

Binary Packages:

- `hostname=3.23ubuntu2`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23ubuntu2.dsc' hostname_3.23ubuntu2.dsc 1085 SHA512:5e7f690bb67fcbc7521df55b69ce899ff005d24fb511c017d60ff5e4c9d9fc51271422bb81fc4998d90149cb814d2a209dc61db4d5073f72a37fb22af59827a0
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23ubuntu2.tar.gz' hostname_3.23ubuntu2.tar.gz 13854 SHA512:28b80ea23cbde63af91912aef2773ce83d7f4d1c2c82beb59a86c0e6b11e276019c610a0a60e69947af2b9bc5f86e4f8f6d13c1cb1a9ce35f1e5cfb03e0dd582
```

### `dpkg` source package: `icu=71.1-3`

Binary Packages:

- `icu-devtools=71.1-3`
- `libicu-dev:amd64=71.1-3`
- `libicu71:amd64=71.1-3`

Licenses: (parsed from: `/usr/share/doc/icu-devtools/copyright`, `/usr/share/doc/libicu-dev/copyright`, `/usr/share/doc/libicu71/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu=71.1-3
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_71.1-3.dsc' icu_71.1-3.dsc 2252 SHA512:d63dca8caba4a0bcc3314953c83c164361b11752266c353ca180803be2dd577f003519fdcf97d788296e5370bea1d666152307f5536dc9ce5a844935bfe5f93e
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_71.1.orig.tar.gz' icu_71.1.orig.tar.gz 25701340 SHA512:1fd2a20aef48369d1f06e2bb74584877b8ad0eb529320b976264ec2db87420bae242715795f372dbc513ea80047bc49077a064e78205cd5e8b33d746fd2a2912
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_71.1.orig.tar.gz.asc' icu_71.1.orig.tar.gz.asc 659 SHA512:3371e14f3959defa7fb8d3eb0308084646ed553169b7a845bff89f9a8c1054ef5bee45c26c1834a84cab38fa87710f1585e6c5787be1fe2df356eb5c2ba20aae
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_71.1-3.debian.tar.xz' icu_71.1-3.debian.tar.xz 65264 SHA512:1afb812ba0d8a57d1985700da1ee49f0b2d8b453a835b00cd24bc5be7212670265d9a70d8daa7f55cb1324822390ab2afe5170fe5af03d03aa27970013e0a7d7
```

### `dpkg` source package: `ilmbase=2.5.7-2`

Binary Packages:

- `libilmbase-dev:amd64=2.5.7-2`
- `libilmbase25:amd64=2.5.7-2`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase25/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.5.7-2
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.7-2.dsc' ilmbase_2.5.7-2.dsc 2483 SHA512:a08b5b06901988324e43fb0f518b3b6586fdee726454c85bb9ae3627f2795127a8a8195959543ad50ce31b928af8b1b8054c2750d3777ccbfa0877d26df46909
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.7.orig.tar.gz' ilmbase_2.5.7.orig.tar.gz 27539574 SHA512:e44edfa2dcfff2fe372ed2ba07b39a472e549025978de178eff26be641767d22d1a3b543fb7672d9b7b2e9f4c308667f785829ed6d9032a2b42f2ffa0163de40
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.7.orig.tar.gz.asc' ilmbase_2.5.7.orig.tar.gz.asc 27539574 SHA512:e44edfa2dcfff2fe372ed2ba07b39a472e549025978de178eff26be641767d22d1a3b543fb7672d9b7b2e9f4c308667f785829ed6d9032a2b42f2ffa0163de40
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.7-2.debian.tar.xz' ilmbase_2.5.7-2.debian.tar.xz 14484 SHA512:b418500f82cd9e87ad97a76d22b0ce62c8da5ce90b186f436148da346912e47498a5888acaf942aa16f22a51cec9bd21d6088d111efa5953c8d14dbcf0cc716f
```

### `dpkg` source package: `imagemagick=8:6.9.11.60+dfsg-1.3build2`

Binary Packages:

- `imagemagick=8:6.9.11.60+dfsg-1.3build2`
- `imagemagick-6-common=8:6.9.11.60+dfsg-1.3build2`
- `imagemagick-6.q16=8:6.9.11.60+dfsg-1.3build2`
- `libmagickcore-6-arch-config:amd64=8:6.9.11.60+dfsg-1.3build2`
- `libmagickcore-6-headers=8:6.9.11.60+dfsg-1.3build2`
- `libmagickcore-6.q16-6:amd64=8:6.9.11.60+dfsg-1.3build2`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.11.60+dfsg-1.3build2`
- `libmagickcore-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.3build2`
- `libmagickcore-dev=8:6.9.11.60+dfsg-1.3build2`
- `libmagickwand-6-headers=8:6.9.11.60+dfsg-1.3build2`
- `libmagickwand-6.q16-6:amd64=8:6.9.11.60+dfsg-1.3build2`
- `libmagickwand-6.q16-dev:amd64=8:6.9.11.60+dfsg-1.3build2`
- `libmagickwand-dev=8:6.9.11.60+dfsg-1.3build2`

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.11.60+dfsg-1.3build2
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1.3build2.dsc' imagemagick_6.9.11.60+dfsg-1.3build2.dsc 5123 SHA512:dc9890ab381fc9880955935a6dd593f3b77fb1e6373b21f13947d78713409405056a727637e57106316e1054905b9922f3f816e6990ecfa9a624aa98ab154cbf
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg.orig.tar.xz' imagemagick_6.9.11.60+dfsg.orig.tar.xz 9395144 SHA512:345a23eda96516fc7a213bd4a322bca4c8b690efe40ff7b498a448f8cedd7f0d600fae2cb6fff45bc995779a90d8c04b58288273eee97833ddebb4f9f2a3d14c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1.3build2.debian.tar.xz' imagemagick_6.9.11.60+dfsg-1.3build2.debian.tar.xz 247016 SHA512:11fe03b53dba2906642c2258e183c4ef90d86e1c4bdd78ad9eb7bd39bc5ed86b7609bc098f35f19777323fe0b950c80f6f5c724972edb600c4c9b5bf152971cc
```

### `dpkg` source package: `init-system-helpers=1.63`

Binary Packages:

- `init-system-helpers=1.63`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.63
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.63.dsc' init-system-helpers_1.63.dsc 1968 SHA512:e07f44691e0d73532aa8708f1a2f42448812da711f60aef403c53e839bda380b6219f83008df0060ff17262398c03dd5ccb0de74b1ee01ce253ecdcfc40a06fc
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.63.tar.xz' init-system-helpers_1.63.tar.xz 43204 SHA512:75accd229a1a2ae50e1b51cd43e36dd7cb2a5712e1aab8992da00fe3061a7d27cbe1396a68bb62771902afaf6f3467fc7888d66df3285946d4cea216c5fef3e1
```

### `dpkg` source package: `isl=0.24-2build1`

Binary Packages:

- `libisl23:amd64=0.24-2build1`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.24-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24-2build1.dsc' isl_0.24-2build1.dsc 1939 SHA512:508aaf010116caea8b9c61bb9c40a3979ed73cd09369b07747b43bed169988c415771c13395e46213f4c95f363f46e055e864723a3fb775fe9d2b5bb5bf45404
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24.orig.tar.xz' isl_0.24.orig.tar.xz 1930956 SHA512:ff6bdcff839e1cd473f2a0c1e4dd4a3612ec6fee4544ccbc62b530a7248db2cf93b4b99bf493a86ddf2aba00e768927265d5d411f92061ea85fd7929073428e8
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24-2build1.debian.tar.xz' isl_0.24-2build1.debian.tar.xz 26628 SHA512:8aafdd03adbe32b3eb6cb9468b676c20c02377c3b45947619258cfc1c682f4e9689945f9dbc6b42fd4c1289c563e7a7bba0af4f0a58b2c7ab94c7fdb3c6c9f5f
```

### `dpkg` source package: `jbigkit=2.1-3.1build3`

Binary Packages:

- `libjbig-dev:amd64=2.1-3.1build3`
- `libjbig0:amd64=2.1-3.1build3`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1build3
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build3.dsc' jbigkit_2.1-3.1build3.dsc 2085 SHA512:e99514c3ef04160b037174e10add2fdbb7239568e2b628ef1065e6b06216df706024b2884d534974f816325f0951df950a51068780f04818d2f3b205d0080df5
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA512:c4127480470ef90db1ef3bd2caa444df10b50ed8df0bc9997db7612cb48b49278baf44965028f1807a21028eb965d677e015466306b44683c4ec75a23e1922cf
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build3.debian.tar.xz' jbigkit_2.1-3.1build3.debian.tar.xz 7788 SHA512:e828dece638f0f702cc917d48d357bf358e4c21cd7839c814ffd4c7382ed98facb0a58e75d949275b67bbce3484b4887144b0c740444a3ed2ddab5db4c56ed5f
```

### `dpkg` source package: `keyutils=1.6.1-2ubuntu3`

Binary Packages:

- `libkeyutils1:amd64=1.6.1-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `krb5=1.19.2-2`

Binary Packages:

- `krb5-multidev:amd64=1.19.2-2`
- `libgssapi-krb5-2:amd64=1.19.2-2`
- `libgssrpc4:amd64=1.19.2-2`
- `libk5crypto3:amd64=1.19.2-2`
- `libkadm5clnt-mit12:amd64=1.19.2-2`
- `libkadm5srv-mit12:amd64=1.19.2-2`
- `libkdb5-10:amd64=1.19.2-2`
- `libkrb5-3:amd64=1.19.2-2`
- `libkrb5-dev:amd64=1.19.2-2`
- `libkrb5support0:amd64=1.19.2-2`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit12/copyright`, `/usr/share/doc/libkadm5srv-mit12/copyright`, `/usr/share/doc/libkdb5-10/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.19.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2-2.dsc' krb5_1.19.2-2.dsc 3170 SHA512:1b24e80f4b4d9d2635f4a9d45fb9dc6058cd004d0d7bb613a0ce38d4bb4e657e4d1bedeea13f4250d0aca09a039e436313392a2852dc5f2483d2c014388e7f1c
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz' krb5_1.19.2.orig.tar.gz 8741053 SHA512:b90d6ed0e1e8a87eb5cb2c36d88b823a6a6caabf85e5d419adb8a930f7eea09a5f8491464e7e454cca7ba88be09d19415962fe0036ad2e31fc584f9fc0bbd470
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz.asc' krb5_1.19.2.orig.tar.gz.asc 833 SHA512:87c4d096dbb6821401125b8f8a315ce1aac029744ba9670a4f8a2a680e6dd5798e1c6d5d2b68b17fd9a4b3b9c6ff111cd1dcac42f934d48fb20381b3765e0f64
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2-2.debian.tar.xz' krb5_1.19.2-2.debian.tar.xz 106876 SHA512:01d3de8b16728625ddd7860e82d1f98e19fe5c82957ebe816f85e5b0b4405353ce579149b61229a692bf7b8daa1e574599bcf45bb3e1cb6ce89642e2d228c883
```

### `dpkg` source package: `lcms2=2.12~rc1-2build2`

Binary Packages:

- `liblcms2-2:amd64=2.12~rc1-2build2`
- `liblcms2-dev:amd64=2.12~rc1-2build2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3 (GPL-3 for the fast_float plugin only)`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.12~rc1-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12%7erc1-2build2.dsc' lcms2_2.12~rc1-2build2.dsc 2120 SHA512:589b8926590d9158a85ad4641920e1f9700fb864b13ec0f2e44292bd0530cc639ecbcbe216405b7a528ecc512902a79456b30985b5c5a278a5c4692f8fc4bc9f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12%7erc1.orig.tar.gz' lcms2_2.12~rc1.orig.tar.gz 7417767 SHA512:1d27e6f91911053b79f2a46c6c16943e25fce2f0501bb7d97f49507522a8a0f911d60f20726fc31727fee5242c6d452c86cdc28735f8f88c3aa9676fd35fdec6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12%7erc1-2build2.debian.tar.xz' lcms2_2.12~rc1-2build2.debian.tar.xz 10616 SHA512:250e0245e300fff7be06a43a30621bff920cbb606e51197177d3d43acc1b50ad0db8988f7c05b6b4365073bf0c952d93dcb79364228698fcd8fbc6b093d4f843
```

### `dpkg` source package: `libassuan=2.5.5-3`

Binary Packages:

- `libassuan0:amd64=2.5.5-3`

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
$ apt-get source -qq --print-uris libassuan=2.5.5-3
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5-3.dsc' libassuan_2.5.5-3.dsc 1997 SHA512:4b936672d6fd1a12e8d7b6c326f690c4d702df61ba9127ccb840e1eb5abb9387f8a7ac0bbe6fa6352c18a73d0cf1ca20a17fabaa5769db9ca83aa2c31b4eea62
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2' libassuan_2.5.5.orig.tar.bz2 572263 SHA512:70117f77aa43bbbe0ed28da5ef23834c026780a74076a92ec775e30f851badb423e9a2cb9e8d142c94e4f6f8a794988c1b788fd4bd2271e562071adf0ab16403
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2.asc' libassuan_2.5.5.orig.tar.bz2.asc 228 SHA512:343336ea5dffa113cd934167f548faf4e85d31bf64a46541ee6828b4d0995a8cc9d0668995812d9c4d3ab73347d5b1bbfff0d6ed586fbf4bbc57ac42e828e8d5
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5-3.debian.tar.xz' libassuan_2.5.5-3.debian.tar.xz 13940 SHA512:f40b55e1dda3ac1da2c5f348a25e6d21803050a355a3890bd2fdac7a2a10e467b7b3c44621d2a2078bad8f930ce5e93190ac4d93e9f423616ba9fcfbdf208872
```

### `dpkg` source package: `libbsd=0.11.6-1`

Binary Packages:

- `libbsd0:amd64=0.11.6-1`

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

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.11.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.6-1.dsc' libbsd_0.11.6-1.dsc 2308 SHA512:9b9b9799f4be63642063e7a7e032a26ec382fe4d25d8577630562f304e2586bfa86b61e4ade539a21d756b667397e83bda839aa3145c8ede94cd7bd374626514
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.6.orig.tar.xz' libbsd_0.11.6.orig.tar.xz 416600 SHA512:9dbbfb84340fc69f59667241701d81d176439ce168f123344805898a269f7bd0e98abf8c7fc12d9bf539d1effb19424d93b647cc9120f693327e736d339e6075
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.6.orig.tar.xz.asc' libbsd_0.11.6.orig.tar.xz.asc 833 SHA512:29d77e53d251c641b00924c9c42b69b66eeb160ef0534e84a4ad1afd9009f87bda82f1b91d271efe37c676295add3fab01ce55aa6cd96aa0c5f34f9837b870cd
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.6-1.debian.tar.xz' libbsd_0.11.6-1.debian.tar.xz 17676 SHA512:ac746879ae6b34ea4abd4ae7eb06dff600b3ee41367f58fd6c54bc2b21fb67c3999549191b432d8c8f7dc18bc49c4c82a2564fba7da143f1db247deea9382d3a
```

### `dpkg` source package: `libcap-ng=0.7.9-2.2build3`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.2build3`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libcap2=1:2.44-1build3`

Binary Packages:

- `libcap2:amd64=1:2.44-1build3`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.44-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1build3.dsc' libcap2_2.44-1build3.dsc 2311 SHA512:30fa503d6bffa093ceafc07a26f48b88da855c2957bc0bce99f83461dbf7e656b0460d58752eb60a3699c1c250e6135bb086461af5e3734f1802adbbd5d39be2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44.orig.tar.xz' libcap2_2.44.orig.tar.xz 125568 SHA512:1bb323ca362923bd6bd0e2e4639cf8726975165a620a243b31e797056439eb7efb2bfbc8e5521636783a86c7415b2037b1638c98747b79183ca7d3d42a04ff20
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1build3.debian.tar.xz' libcap2_2.44-1build3.debian.tar.xz 21312 SHA512:b1c5c20092fe0cb13318f84e585ea9095dd552332a23c8d3162ca1013f02f3b16f7c5a94d407ef88aee62aadfa1f50e67959a3f5206653a801af878f8d89ce24
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

### `dpkg` source package: `libde265=1.0.8-1`

Binary Packages:

- `libde265-0:amd64=1.0.8-1`

Licenses: (parsed from: `/usr/share/doc/libde265-0/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `other-1`
- `public-domain-1`
- `public-domain-2`

Source:

```console
$ apt-get source -qq --print-uris libde265=1.0.8-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.8-1.dsc' libde265_1.0.8-1.dsc 2216 SHA512:75e5ac4bb507cce9a95585e2b1916b65a1995b9389ec81615ed5c86d3cd0ce28a4cdc83a9055b6412dd1db559065ee2e1530ca238f6994b4559b8e91e7e4f338
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.8.orig.tar.gz' libde265_1.0.8.orig.tar.gz 837878 SHA512:bcb33493cbc337d29047c6765189aaba523b20c138aa4fd5c264b3c6aea64cd174cbe14ca2d88c76319e0a8bd5d2e6269f300f056876d2962217eea7934172da
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libde265/libde265_1.0.8-1.debian.tar.xz' libde265_1.0.8-1.debian.tar.xz 8184 SHA512:717f3a2912412222bab2572245dba20b37ac186c19a348bf8b140a9221b8d55fcb6a34a0550a508332f60330b959d73319628a1c26ee4de9fe99f6d1303c116a
```

### `dpkg` source package: `libdeflate=1.10-2`

Binary Packages:

- `libdeflate-dev:amd64=1.10-2`
- `libdeflate0:amd64=1.10-2`

Licenses: (parsed from: `/usr/share/doc/libdeflate-dev/copyright`, `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libdeflate/1.10-2/


### `dpkg` source package: `libedit=3.1-20210910-1build1`

Binary Packages:

- `libedit2:amd64=3.1-20210910-1build1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20210910-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20210910-1build1.dsc' libedit_3.1-20210910-1build1.dsc 2340 SHA512:67cfd7c36cfb575a49a919968710841a19a9f523c6138c3f8bc56de3e546a90adad72f25c1bb4753d83a6d09634c873b3c636613f6d223041f00c7d18ecb7790
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20210910.orig.tar.gz' libedit_3.1-20210910.orig.tar.gz 524722 SHA512:b7361c277f971ebe87e0e539e5e1fb01a4ca1bbab61e199eb97774d8b60dddeb9e35796faf9cc68eb86d1890e8aac11db13b44b57ccc8302d559741fbe9d979e
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20210910-1build1.debian.tar.xz' libedit_3.1-20210910-1build1.debian.tar.xz 15200 SHA512:23ca0f62bf73e9fd1537c599b689807834db6b657c8f0dc448947db49fa3fe0de498ad96ea3d24515f0875fb3f50c4839f1bba25bf9bc48fe23de5fc780f3542
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

### `dpkg` source package: `libevent=2.1.12-stable-5`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.12-stable-5`
- `libevent-core-2.1-7:amd64=2.1.12-stable-5`
- `libevent-dev=2.1.12-stable-5`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-5`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-5`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-5`

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
$ apt-get source -qq --print-uris libevent=2.1.12-stable-5
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-5.dsc' libevent_2.1.12-stable-5.dsc 2356 SHA512:f9ede7afde3917fe195812ca7ad1cd9d60cc7fc6119fa30ff1a9a4cb4aa8d376cc69e5422d827a2d40c8930fb4cdc0cc44f6fd56f4a363a234b85e990344ad31
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA512:88d8944cd75cbe78bc4e56a6741ca67c017a3686d5349100f1c74f8a68ac0b6410ce64dff160be4a4ba0696ee29540dfed59aaf3c9a02f0c164b00307fcfe84f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-5.debian.tar.xz' libevent_2.1.12-stable-5.debian.tar.xz 17032 SHA512:a7fb99b224228a61cbae03f3d0832c1f543150797e6a2910fcdf0846b24cd986837ac11e468b5ffa3814919d293f15a47ca828cb4a7bdc5841e7d3a3f48a9d8b
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

### `dpkg` source package: `libffi=3.4.2-4`

Binary Packages:

- `libffi-dev:amd64=3.4.2-4`
- `libffi8:amd64=3.4.2-4`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi8/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.2-4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.2-4.dsc' libffi_3.4.2-4.dsc 1948 SHA512:a3a3ada71f82d244f8cb54f1cac30ae6be7c4305696700fb6ffb96783f4f9f788c943bc8ba0d7474c9fd31f04453875e1da341240707711e4eff10cd8023e8d1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.2.orig.tar.gz' libffi_3.4.2.orig.tar.gz 1351355 SHA512:31bad35251bf5c0adb998c88ff065085ca6105cf22071b9bd4b5d5d69db4fadf16cadeec9baca944c4bb97b619b035bb8279de8794b922531fddeb0779eb7fb1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.2-4.debian.tar.xz' libffi_3.4.2-4.debian.tar.xz 8164 SHA512:eecf83971847b78aae0c2cfe3b546a858c93462b7d1d2473c96f5b43de47e1d5fc4663b524e4c5792630d7a6d1796e8bdf83f55addc669d0ce3810643924a07f
```

### `dpkg` source package: `libfido2=1.11.0-1`

Binary Packages:

- `libfido2-1:amd64=1.11.0-1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.11.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.11.0-1.dsc' libfido2_1.11.0-1.dsc 2588 SHA512:41d605b05a493a84e452f98e13243f724724ffcba8fd6201e3d4fe49268e5c7b540bc58ffbff3044259b195e27d83d3a81ee71c464608df631cd9b7020760ade
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.11.0.orig.tar.gz' libfido2_1.11.0.orig.tar.gz 624148 SHA512:d9644453d67b84ec8385dfb63796adb3eae2d7f7cb47fbb1bcf9ca7f5cce400623738cc3317d629c2f0af630424cb2788217f8c7f20d1b52b7369c729052d572
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.11.0.orig.tar.gz.asc' libfido2_1.11.0.orig.tar.gz.asc 833 SHA512:281df602dc7372d13b84d421edd52ff8103d90a90f1f9113634f26d9b523d9be393a1452fd3bac71f89c0a7f6213c900cfd347f7295c629fd0ecb36813379de4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.11.0-1.debian.tar.xz' libfido2_1.11.0-1.debian.tar.xz 52472 SHA512:5b06185a268d225dcc344bcc3d637f7fded284126d2824120152a187d5bf997d3565390a4c6db0e1d771c6a84ce7f8e62a1e0d2478438212638fd6f67daf5ff0
```

### `dpkg` source package: `libgcrypt20=1.10.1-2ubuntu1`

Binary Packages:

- `libgcrypt20:amd64=1.10.1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.1-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-2ubuntu1.dsc' libgcrypt20_1.10.1-2ubuntu1.dsc 2918 SHA512:b46e2708b07161785fd419625e8de467f60eddd686e06530f4db2d7dc263702eb2ebbbc53d04e9c147e080981ece86de9a6ff697e334b8a433d6eab8c2af838a
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2' libgcrypt20_1.10.1.orig.tar.bz2 3778457 SHA512:e5ca7966624fff16c3013795836a2c4377f0193dbb4ac5ad2b79654b1fa8992e17d83816569a402212dc8367a7980d4141f5d6ac282bae6b9f02186365b61f13
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2.asc' libgcrypt20_1.10.1.orig.tar.bz2.asc 228 SHA512:dc74b1029ce1909466eeb9cbdbf77b3e3fd2093ef40ea81bd1b9860eb11d1994087a9b575b6c94ed22f64d0f7e8d2999e30c7ea60fd90a2ecf99ddb60cd156c6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-2ubuntu1.debian.tar.xz' libgcrypt20_1.10.1-2ubuntu1.debian.tar.xz 38144 SHA512:46e9f51cbfdca1a23eb88e290465db57e01b443e3ee13b1b5c2d5ea4afb6fda91419a8ae911db8aef344083ca8bd01ceb0853c082f697c787158a5493e862bcd
```

### `dpkg` source package: `libgpg-error=1.43-3`

Binary Packages:

- `libgpg-error0:amd64=1.43-3`

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

- http://snapshot.debian.org/package/libgpg-error/1.43-3/


### `dpkg` source package: `libheif=1.12.0-2build3`

Binary Packages:

- `libheif1:amd64=1.12.0-2build3`

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
$ apt-get source -qq --print-uris libheif=1.12.0-2build3
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.12.0-2build3.dsc' libheif_1.12.0-2build3.dsc 2386 SHA512:63c1db149dc1c477a181771ec4572e9683961e3d2f78743384a1bae64a0b5a10f1eda65839e7c8556f10b0cb1aaf44d672f4f2ac33f83e81faa4800ec294084e
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.12.0.orig.tar.gz' libheif_1.12.0.orig.tar.gz 1684355 SHA512:9e6f74dd52841a33b6021a1581ab28c56123d927caa7972acd284444e90888bbdae983b6d847d20eac7651dacea2193d27eb8df45928cb0774229ef8eea23294
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.12.0-2build3.debian.tar.xz' libheif_1.12.0-2build3.debian.tar.xz 7196 SHA512:572063dad4f77a1002d64dcf5b96edf62d3dbfe88f98df5ff726217e72408dac5d3f8960fca7b29d44ddcaa98641e252064f4ff16223ed543cab1f10cdcd25ca
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

### `dpkg` source package: `libidn2=2.3.2-2build1`

Binary Packages:

- `libidn2-0:amd64=2.3.2-2build1`

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
$ apt-get source -qq --print-uris libidn2=2.3.2-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2-2build1.dsc' libidn2_2.3.2-2build1.dsc 2655 SHA512:bc84158420d526a0f9bca79ca2a8291c55588e2773ded66d7c4b86ad33b370f9d8723cfc3a2b278660de7060687fff5448912e802d7fb63a8ff7876b38440f32
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2.orig.tar.gz' libidn2_2.3.2.orig.tar.gz 2169556 SHA512:958dbf49a47a84c7627ac182f4cc8ea452696cec3f0d1ff102a6c48e89893e772b2aa81f75da8223dfc6326515cca3ae085268fbf997828de9330c3a351152f1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2.orig.tar.gz.asc' libidn2_2.3.2.orig.tar.gz.asc 488 SHA512:0559b51b37c7937f3e1f8bf9de9b193f137f16b79d6673f85691a4f4a12ec132568e913848a70136f8522118817f7ecaa8432d353a5eff6b99a7be8719421fe0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2-2build1.debian.tar.xz' libidn2_2.3.2-2build1.debian.tar.xz 15972 SHA512:d5af028cc405d326c31e67e577ef16d9b8b81e433171220fda2c2a6f8fc982a63b6d1d85c6595f5ce01a5005768d935aeeaa5de8a552990f4e070bc541e78570
```

### `dpkg` source package: `libjpeg-turbo=2.1.2-0ubuntu1`

Binary Packages:

- `libjpeg-turbo8:amd64=2.1.2-0ubuntu1`
- `libjpeg-turbo8-dev:amd64=2.1.2-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.1.2-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2-0ubuntu1.dsc' libjpeg-turbo_2.1.2-0ubuntu1.dsc 1690 SHA512:401a75e62575352db079bd268f00f94c8ea1e8e6c38bda852628729e6dfd3135804e3c9ee5b18b1254fed827e6073b0078553bcbc2c1df30d628bbb717a5ed47
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2.orig.tar.gz' libjpeg-turbo_2.1.2.orig.tar.gz 2257645 SHA512:172c3d8bdad62c32c4560754422fb36f0e80c8316e44d08708f0cba8ee9fd0830f5295d380de34d0f90ec07df6ab4dbe2f0c8451bc60553371c022c9077447c2
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2-0ubuntu1.debian.tar.xz' libjpeg-turbo_2.1.2-0ubuntu1.debian.tar.xz 17240 SHA512:5cfc1e73012f3251e385f0288dece2e3862977fb3975c61c344afc464a2fd329c3fa027fc07edc40097afaad052bdf6f0dad55c665c20ccdde9f2231ec191410
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu10`

Binary Packages:

- `libjpeg-dev:amd64=8c-2ubuntu10`
- `libjpeg8:amd64=8c-2ubuntu10`
- `libjpeg8-dev:amd64=8c-2ubuntu10`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg8/copyright`, `/usr/share/doc/libjpeg8-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg8-empty=8c-2ubuntu10
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu10.dsc' libjpeg8-empty_8c-2ubuntu10.dsc 1655 SHA512:1085be8a159c716c4ca89e6bfb2b1a5ce7b66ad8bc8f4cf3796c2c4ac3dad5169ac5be045f2a9ce103858b42585b1ce52d6dc6986995d073785170d45fe4d29d
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu10.tar.gz' libjpeg8-empty_8c-2ubuntu10.tar.gz 1912 SHA512:1c21044013df62225f861ec6f88b2a43e0f6254522ed379ad081b92f4f89b64686d4e68d70e8384289cd8222df2288400c2d0e8b8ccae87dd079164bdc3f3cf3
```

### `dpkg` source package: `libksba=1.6.0-2build1`

Binary Packages:

- `libksba8:amd64=1.6.0-2build1`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0-2build1.dsc' libksba_1.6.0-2build1.dsc 2602 SHA512:832761d70684def527dacae7f2403972eea3e9133a74c7daa96bf8497693b29a2ddb8d6cd54893604106cecae56637eddbf272e4b7e5778fef4bdd92046f838c
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2' libksba_1.6.0.orig.tar.bz2 662120 SHA512:a7c76d41dfd8ec6383ac2de3c53848cd9f066b538f6f3cd43175e3c8095df51b96d0a24a573481c0c4856b09b7c224e2b562d88f5c0801e7acfb582ea2739c2b
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2.asc' libksba_1.6.0.orig.tar.bz2.asc 228 SHA512:fc381ea66eefdb431a5248fa3ac0751d7343d7f99cc7ebf7621b0763e6e31a80b45c5e17b09bbc7c1c1154e6a0152af1f13798f64959ac63f50b789ec046d7a3
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0-2build1.debian.tar.xz' libksba_1.6.0-2build1.debian.tar.xz 14612 SHA512:95b789302a6a3408e8f3751845a8ed09ad5a09313e8106b9aba24c565219ce2012899068faaa6606b134e64a3244286ef4f035bf36e95d0010c7701edf8aa64e
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

### `dpkg` source package: `libmaxminddb=1.5.2-1build2`

Binary Packages:

- `libmaxminddb-dev:amd64=1.5.2-1build2`
- `libmaxminddb0:amd64=1.5.2-1build2`

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
$ apt-get source -qq --print-uris libmaxminddb=1.5.2-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1build2.dsc' libmaxminddb_1.5.2-1build2.dsc 2454 SHA512:7e7166e405d886d2f8f4a29c0e4c4920d86d1cce2e453cc97e8185a67a7baeadf51a77c313a0bb896342ecb9b77c80733e3ca1641c8bdf0a8f234d49addb69fd
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2.orig.tar.gz' libmaxminddb_1.5.2.orig.tar.gz 249507 SHA512:2f053028e28dc4f1d94039e52193ab71f8dc278f1fafa14bca1af0251d239351acadb5d540e63c250232d0fd1b8f2dd45289f0eae5c55d9b4430acbabbcd11a9
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1build2.debian.tar.xz' libmaxminddb_1.5.2-1build2.debian.tar.xz 12488 SHA512:1017b70ee85f22eed14258a4d594d77e5bf6fbe5dcb0a23e635f0dcb26d09eb173dd777063f695f9610350dab91b8717ae4d701c3b1eb282358d6450394a0889
```

### `dpkg` source package: `libmd=1.0.4-1build1`

Binary Packages:

- `libmd0:amd64=1.0.4-1build1`

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
$ apt-get source -qq --print-uris libmd=1.0.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4-1build1.dsc' libmd_1.0.4-1build1.dsc 2380 SHA512:778b562e6b3860fe6a6d5ddf4d7cce381126be77d151ac7c2a619d57737080f2adc07ff8e01fcafd98b3ace157fc72ab77a572362b56e79e5abb79a99fdacd6c
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz' libmd_1.0.4.orig.tar.xz 264472 SHA512:731553ecc5e0e1eb228cced8fccd531fe31fb5c7627ca30013d287e1aeb8222959cf7498fbb7414bbabb967b25d4e8b0edd54fc47f6ccf55fc91087db0725ce3
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz.asc' libmd_1.0.4.orig.tar.xz.asc 833 SHA512:ec4b60a721da1f315fad73daa8ee620f44a53f17a30506c4d63b154b3abde19bb248b2ce6b83b989589e2a9184ebbe1b870e83181e18a4147d75617579d10504
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4-1build1.debian.tar.xz' libmd_1.0.4-1build1.debian.tar.xz 10264 SHA512:0e287498326a5aa3bc95cb0c576df7d0bb289bfb9db3a1f812d0e202c61af9dc78ecfa4b6b26c2dee3c5ccbefad877919f44ec849b3300f0f30878080eb5cb13
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

### `dpkg` source package: `libpng1.6=1.6.37-5`

Binary Packages:

- `libpng-dev:amd64=1.6.37-5`
- `libpng16-16:amd64=1.6.37-5`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.37-5
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-5.dsc' libpng1.6_1.6.37-5.dsc 2225 SHA512:457d0953cb125e07953e14fe4686613c9a8ab1c91360b05cf95ae9dfb93a50be79dab337a4e10e72f79b041d8dd40ac22e4a6865321cb9a7d8060ef5415753bf
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA512:ccb3705c23b2724e86d072e2ac8cfc380f41fadfd6977a248d588a8ad57b6abe0e4155e525243011f245e98d9b7afbe2e8cc7fd4ff7d82fcefb40c0f48f88918
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-5.debian.tar.xz' libpng1.6_1.6.37-5.debian.tar.xz 32744 SHA512:51565a6b1dc08c2edd9e1c6fab6cd2060f0e6c249a0a7e712f58b4d8d3ec753222bd42ae50d5054a2cc849aad511a6a791ab975406833f29d0c53123c81c62fa
```

### `dpkg` source package: `libpsl=0.21.0-1.2build2`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.2build2`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1.2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.2build2.dsc' libpsl_0.21.0-1.2build2.dsc 2348 SHA512:28ff7399af2290fd447f781b1f799ba5cb8c0cb794833c40d8f16cc81b0abd4f77bd9dc990c7925e8be8832555f07cc6ede80f971b68ac5fc6e644d601e582b6
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA512:b7466edb9763f94a65330dbb3c19586f9c7b01e20ddedb38ca2fd4c9ee5764a4f9b3291dc4b76659b45425d954f15973345f917b2cd2de72ea731e8c41f2a265
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.2build2.debian.tar.xz' libpsl_0.21.0-1.2build2.debian.tar.xz 12896 SHA512:9d8c7130bee8c521e4f1ab1e13edfe2ed2fec538bda9133662d4120e8f5303595e6f27f466f30b07e61b94e138dd2787e17af91b8cc29275b5b4d2e098133eee
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

### `dpkg` source package: `librsvg=2.52.5+dfsg-3`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.52.5+dfsg-3`
- `librsvg2-2:amd64=2.52.5+dfsg-3`
- `librsvg2-common:amd64=2.52.5+dfsg-3`
- `librsvg2-dev:amd64=2.52.5+dfsg-3`

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
$ apt-get source -qq --print-uris librsvg=2.52.5+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.52.5%2bdfsg-3.dsc' librsvg_2.52.5+dfsg-3.dsc 2972 SHA512:c4c32b9b8a82ccd35bf667dbb1ab69c39bfc0ad98bff820c291f1f19bd477d73895550dfec48b3d19013f76b4a740366e70ae499cbf8bdd4f6869cce7f4f889d
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.52.5%2bdfsg.orig.tar.xz' librsvg_2.52.5+dfsg.orig.tar.xz 20813024 SHA512:641dcd149ce0d5117947e3fcb04efd41591812953ec4b12ba350ce9950ed4bcb26726a78df9d317e6bd557e6fd463867476205b5e6720a9a15bd1bcfcb6f7ffe
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.52.5%2bdfsg-3.debian.tar.xz' librsvg_2.52.5+dfsg-3.debian.tar.xz 33800 SHA512:15923a453df7730a666722fe64eee6aeb282013d6e66c69418c7b6b931a6acb4a906620e9aab8f8fc8dabb855664511cd3b19f5fac7733e47803d5e974fa22d4
```

### `dpkg` source package: `libseccomp=2.5.4-1ubuntu1`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4-1ubuntu1.dsc' libseccomp_2.5.4-1ubuntu1.dsc 2491 SHA512:ebe53fcc3d488652a85ac3ef5cd2842785b7c79a707791df5c116bbb564f4f4d36ea2310a15c94939ec76cc8c16fcf69d85fb3bebf25a63103ac2d19b7646566
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz' libseccomp_2.5.4.orig.tar.gz 637228 SHA512:92650bd7d1d48b383f402a536b97a017fd0f6ad1234daf4b938d01c92e8d134a01d2f2dd45fd9e2d025d7556bd1386ec360402145a87f20580c85949d62cea0e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz.asc' libseccomp_2.5.4.orig.tar.gz.asc 833 SHA512:10ce632da2762e3b5acb468194b2424d80bab786cc5923a8ee0b0684290282ef2f0a17192680afb36626c82e73a3ba64e73f248ed63cd3e55c3cf8cee4e1e447
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.4-1ubuntu1.debian.tar.xz' libseccomp_2.5.4-1ubuntu1.debian.tar.xz 23624 SHA512:fde9ad923675c4f39fcb28a5ec2fda28e23e747303595757a3f262b875e2a2f2f4d639a8d9317538e0da770e2d405bdc70fd188249330987e5e3d95c14d74db8
```

### `dpkg` source package: `libselinux=3.3-1build2`

Binary Packages:

- `libselinux1:amd64=3.3-1build2`
- `libselinux1-dev:amd64=3.3-1build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libsemanage=3.3-1build2`

Binary Packages:

- `libsemanage-common=3.3-1build2`
- `libsemanage2:amd64=3.3-1build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libsepol=3.4-1`

Binary Packages:

- `libsepol-dev:amd64=3.4-1`
- `libsepol2:amd64=3.4-1`

Licenses: (parsed from: `/usr/share/doc/libsepol-dev/copyright`, `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libsepol/3.4-1/


### `dpkg` source package: `libsigsegv=2.13-1ubuntu3`

Binary Packages:

- `libsigsegv2:amd64=2.13-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.13-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13-1ubuntu3.dsc' libsigsegv_2.13-1ubuntu3.dsc 2474 SHA512:74d424b26794088d5227b7539d3b7f0764a3dc23099f2a7ad0c3a274baf5cbda54f0a46400fe0132cf1b05523f8eb4fdd723691e447d549a9599fdc17a4fc6b9
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13.orig.tar.gz' libsigsegv_2.13.orig.tar.gz 460736 SHA512:9c0cf01ee2a39f77f2e42eb06a2aa60644e10fe2cd39089de58f6206baf7fe7d61fe0ec6bf187276fcfccf61585154ce904fe374b474b7ba9fa050a61a2f3918
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13.orig.tar.gz.asc' libsigsegv_2.13.orig.tar.gz.asc 819 SHA512:92d8c651557a7cd0ba0a9e0f45f75f5ee7508041e014c8438aa0d84065b5a343867346acbf007fd0d8b3a120e6bde993935f66d1cbd62583bc763ecdde359640
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13-1ubuntu3.debian.tar.xz' libsigsegv_2.13-1ubuntu3.debian.tar.xz 8960 SHA512:fe9c70156c8ed3568b8e1e349afb33eb18b9802a1dbe470bd67079cf053f3883ef24582c316477680983a65aff071a2e32c8996848995fc21fc74a43b567fb6d
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

### `dpkg` source package: `libssh=0.9.6-2build1`

Binary Packages:

- `libssh-4:amd64=0.9.6-2build1`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.6-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6-2build1.dsc' libssh_0.9.6-2build1.dsc 2877 SHA512:63ea8a98ea6c1e9ca3f00fdf592cc5a7bf64d98abb167a0555bbda1ad0a185925ec8ee87f9f0ee846aff05defa1ce4b8edf4e8ae1d22ca8fd1b7c96c16d9d2cd
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6.orig.tar.xz' libssh_0.9.6.orig.tar.xz 1053056 SHA512:4040ec4af937e95be2e41313ef6d4db60b46b8d4dea10c09402398127c1d1ca8843392d207088aeee3c7ef631c6ae7b66861327dcebf78ed3af0723777619fd1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6.orig.tar.xz.asc' libssh_0.9.6.orig.tar.xz.asc 833 SHA512:1b6223efe9e4ce864cd8d97d517f9f0d38c1cd502b5874fdc6a58731038c2830a72ce753f02fc062d9d4d5922107ec9a2e62fe24a704bb5dec0dcfecdb569fe6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6-2build1.debian.tar.xz' libssh_0.9.6-2build1.debian.tar.xz 27568 SHA512:5e4553884339d4457b3487cd82376262e85b14c58f488e40208db9c4e4690cf797e6f77f997f565379597aad491ad2eb631f5d19b454da54a2d8666b85aecc88
```

### `dpkg` source package: `libtasn1-6=4.18.0-4build1`

Binary Packages:

- `libtasn1-6:amd64=4.18.0-4build1`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.18.0-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0-4build1.dsc' libtasn1-6_4.18.0-4build1.dsc 2794 SHA512:cb0f727f9935cdb7784451234c676f0e3544789cc01dd6786006d4662807937722437de6450f4bd24b698b621b7dfa7eaf28d607402ecbb8167315791739d570
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0.orig.tar.gz' libtasn1-6_4.18.0.orig.tar.gz 1724441 SHA512:4f2f4afc7561fda7a1f1c6c525c3c3b08228a1a4aa8c3d3d5e02e993d8f83ccee1dd0f1b201cec0fbfc97043d4b1d7a95ffd34d65422a38b85b931ac7a015831
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0.orig.tar.gz.asc' libtasn1-6_4.18.0.orig.tar.gz.asc 228 SHA512:8ef3918a3130f695d2d5b26dd945084b931005eff8914c50a0ac9795d4cc6ec9e9645e2941ff4235cba3b4b2987ab1c7da65225e24ce16aaab844352ecdafbf6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0-4build1.debian.tar.xz' libtasn1-6_4.18.0-4build1.debian.tar.xz 22112 SHA512:4c363cfa12bd27c22a32ced69ca560ed6d3af2404158dcb0c1be472c6af411931f5d807f77b9966a1fb6bc9089d3d354fc85c3144d8beaabe36036694898a82e
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

### `dpkg` source package: `libtirpc=1.3.2-2build1`

Binary Packages:

- `libtirpc-common=1.3.2-2build1`
- `libtirpc-dev:amd64=1.3.2-2build1`
- `libtirpc3:amd64=1.3.2-2build1`

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
$ apt-get source -qq --print-uris libtirpc=1.3.2-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2build1.dsc' libtirpc_1.3.2-2build1.dsc 2218 SHA512:66c3164c69601f450b2105b7ac755354b0ab7afb1dbc8625b3b8cfee324dfe74662f494bbd1f70fb3c708d1e159a7de02d90fa7f322af7168bbaa98b28cb441d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2.orig.tar.bz2' libtirpc_1.3.2.orig.tar.bz2 513151 SHA512:8664d5c4f842ee5acf83b9c1cadb7871f17b8157a7c4500e2236dcfb3a25768cab39f7c5123758dcd7381e30eb028ddfa26a28f458283f2dcea3426c9878c255
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2build1.debian.tar.xz' libtirpc_1.3.2-2build1.debian.tar.xz 11124 SHA512:5a8e662fe01745b0e608d51de0567d71d3ccbdee6f437730192662615cb4df8a853aead7ee358c4a57cc64b768ff5f5517d45a07b7169aa643a869fb31d453c9
```

### `dpkg` source package: `libtool=2.4.7-4`

Binary Packages:

- `libltdl-dev:amd64=2.4.7-4`
- `libltdl7:amd64=2.4.7-4`
- `libtool=2.4.7-4`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.7-4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7-4.dsc' libtool_2.4.7-4.dsc 2257 SHA512:a194fb4666f17a0351b4535a586bd05414112a8ed7c5f4ed620619465de552456c0966ed830c7edfd361c7ff9beb65476decd78b7c8e20df1aa32d892e1c595a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7.orig.tar.xz' libtool_2.4.7.orig.tar.xz 1026028 SHA512:424f4549aa713917859dc31e62153934c67b8b9d5718452f0e50bb8f6ef48ae6274cc4d4ddd905b15858d19c60daf8c194471e6ed0c8f76e7d55e7ef932a8d3a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.7-4.debian.tar.xz' libtool_2.4.7-4.debian.tar.xz 40100 SHA512:b99f963072c3c3b7f57566c89f02fe483d77227691d1c07716a6261e1324dc0c33fedebf4c1ef5b2ce844ba356b62466d305eead1f9093e606e9ce57441cdbb9
```

### `dpkg` source package: `libunistring=1.0-1`

Binary Packages:

- `libunistring2:amd64=1.0-1`

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
$ apt-get source -qq --print-uris libunistring=1.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.0-1.dsc' libunistring_1.0-1.dsc 1928 SHA512:630d20ef6dd19be991147131d38acae2db15d1df34403264a15a373fcd4b661efffc1ae3916c52448f05cafb93bf1266527efa6630a02def88b86495d688a0c3
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz' libunistring_1.0.orig.tar.xz 2367800 SHA512:70d5ad82722844dbeacdfcb4d7593358e4a00a9222a98537add4b7f0bf4a2bb503dfb3cd627e52e2a5ca1d3da9e5daf38a6bd521197f92002e11e715fb1662d1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_1.0-1.debian.tar.xz' libunistring_1.0-1.debian.tar.xz 42004 SHA512:f9208e7ab38cc742bb46dc1a871ddb03847b99b6169e20e8d8660dd9cdf22bffb27f9b329dcbd025ad9b26aee5a2aab01337f36d8ab3020d2e752f9c2d4368ce
```

### `dpkg` source package: `libwebp=1.2.2-2`

Binary Packages:

- `libwebp-dev:amd64=1.2.2-2`
- `libwebp7:amd64=1.2.2-2`
- `libwebpdemux2:amd64=1.2.2-2`
- `libwebpmux3:amd64=1.2.2-2`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp7/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=1.2.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.2-2.dsc' libwebp_1.2.2-2.dsc 2065 SHA512:4c11b5d638fdc522b854e6ea387690fea5141cff9abdafc53588013b043969ef52c6e1a98db14cbae71510bed6b7113c1bfb9c216a280a4b1ef84f6c3463dd7b
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.2.orig.tar.gz' libwebp_1.2.2.orig.tar.gz 4117468 SHA512:0dd0a721352b513a218d55383bcd0cc45b786df8089f70f87257b5dcc0c4e2f1798e20f1ca98b8fe51710abb667f9c4c14f20f980a11c484c8832f0dc66e3bff
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.2-2.debian.tar.xz' libwebp_1.2.2-2.debian.tar.xz 5688 SHA512:1180ddc2ab7e019a3e662f57167ded93ee05412eb450a1aa2c188ef0116e478707440424869960c5cb3d092bae34dc51f12c6f1f70c5988abe1feca409161e32
```

### `dpkg` source package: `libwmf=0.2.12-5ubuntu2`

Binary Packages:

- `libwmf-0.2-7:amd64=0.2.12-5ubuntu2`
- `libwmf-dev=0.2.12-5ubuntu2`
- `libwmflite-0.2-7:amd64=0.2.12-5ubuntu2`

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
$ apt-get source -qq --print-uris libwmf=0.2.12-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.12-5ubuntu2.dsc' libwmf_0.2.12-5ubuntu2.dsc 2632 SHA512:f8ee424067a5f9de3c6e55050899086f9fe48a64283c0ef2306e99720a7fe57f7f063800e595fe45491586dfde452726756cfdd085c7e002c931407495feeac7
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.12.orig.tar.gz' libwmf_0.2.12.orig.tar.gz 3043572 SHA512:9280851e560becc91546906b911e0c59a1abd690e10680f6d94a335d66aeaec5eb12ccf2214ee7af2a15729a7b5f8b906022822399b4e2bc12c75a2d75748cab
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.12-5ubuntu2.debian.tar.xz' libwmf_0.2.12-5ubuntu2.debian.tar.xz 26204 SHA512:6e52187d938d52b09fbb79c0ce4b5788be7243eef7cfbbe62b6e7c1076a5096a2e0ef8a7cf5aa14033685f207d9ad8f50f6249fbf839179c0179a471269040d5
```

### `dpkg` source package: `libx11=2:1.7.5-1`

Binary Packages:

- `libx11-6:amd64=2:1.7.5-1`
- `libx11-data=2:1.7.5-1`
- `libx11-dev:amd64=2:1.7.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.7.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.5-1.dsc' libx11_1.7.5-1.dsc 2539 SHA512:f126b0bec60f9d5dd002cde0d555ab316674bc6b411358498bf67ea4201be660f4e278c4e42ccdee1c4b9a2503fd64207cb948bf428b1cf56bbc25c62584e9b2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.5.orig.tar.gz' libx11_1.7.5.orig.tar.gz 3170022 SHA512:90474f5f95c3498a02100aeeb6b5ad7ae9076bc40a70cdd828bd881adac0bf278002186142f2760e5504cf82120f4869798831e0e2332ecbc6903e8f7c9114ab
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.5.orig.tar.gz.asc' libx11_1.7.5.orig.tar.gz.asc 358 SHA512:75139b9f7b2f19aed3d3a66ea8b883480db2fa56d713bb0160ea8a0faba208da4c241768f9f2703f723f13906438eda3117f489d7d5d17fbe1cbb75b13c9935d
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.5-1.diff.gz' libx11_1.7.5-1.diff.gz 94094 SHA512:529f346d7f2ebb03988a10bf30516506a648b542d52fb9338e1f7d31cc4e939cffb651ddbd08ddcbf2911b26046864c02b8583914b2413ac244209ecb97313bb
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

### `dpkg` source package: `libxcb=1.14-3ubuntu3`

Binary Packages:

- `libxcb-render0:amd64=1.14-3ubuntu3`
- `libxcb-render0-dev:amd64=1.14-3ubuntu3`
- `libxcb-shm0:amd64=1.14-3ubuntu3`
- `libxcb-shm0-dev:amd64=1.14-3ubuntu3`
- `libxcb1:amd64=1.14-3ubuntu3`
- `libxcb1-dev:amd64=1.14-3ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-3ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-3ubuntu3.dsc' libxcb_1.14-3ubuntu3.dsc 5480 SHA512:cc563eae53e92b3f5cf700f0a61ee036fe0df9a109453dd4cd6a8107dac4a7f6d85e28810011ef74ca69ca36853a8d20e877480b94344ad5262f8fd6da299d5c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA512:6114d8c233b42b56604787a0475e924143aa13f1d382e6029b2150a4360c12ce78073409f754fbb1e5d9f99fc26900c0a4c59e9cfbd4c3d0a3af0c1306e62da1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-3ubuntu3.diff.gz' libxcb_1.14-3ubuntu3.diff.gz 27588 SHA512:228c6da2cf94e02b249ccb04f2668f45b2ab117a4c6670ac6f7ab449582e459df4fc7e1ce5ae5cd945acea6fd00b935ed6394c800ee3d92ce9a0fb6913460f86
```

### `dpkg` source package: `libxcrypt=1:4.4.27-1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.27-1`
- `libcrypt1:amd64=1:4.4.27-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.27-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.27-1.dsc' libxcrypt_4.4.27-1.dsc 1525 SHA512:1335a2ab3f7b519022af13c18dca9ea1c2de3007c07f120d53fbb7eb834ac7e0ece120681c1ee1dd92771469104dccedef3a7e85ec51fc1ca64b52c9447558c0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.27.orig.tar.xz' libxcrypt_4.4.27.orig.tar.xz 391772 SHA512:9d194066ab7eefd3e568b2478d58aa378da8571abf4c37ddcde2c01114a4aa69f0edfb4e3d13d951feac5955336f9b02046d9b1fd1b9fbfbc556aad31cf64d7e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.27-1.debian.tar.xz' libxcrypt_4.4.27-1.debian.tar.xz 7764 SHA512:02e38ba06f3555dd930fc7ed44602dc816ce48f4c29fdc085249948596d5e7e96600cb81c8c9fb2e1dc33574d5136d08feeff3eb1dd3522aa8e5cdc9037c1ae0
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

### `dpkg` source package: `libxml2=2.9.14+dfsg-1`

Binary Packages:

- `libxml2:amd64=2.9.14+dfsg-1`
- `libxml2-dev:amd64=2.9.14+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.14+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.dsc' libxml2_2.9.14+dfsg-1.dsc 2915 SHA512:a01b4f95cceb05f2adb82070ee58aa9d6c09d6b47940efa73b14bcd5a3fc94456a617765b85d9bd75ec8933eca1fcd287d899ddcbc3234129882679101fb6562
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg.orig.tar.xz' libxml2_2.9.14+dfsg.orig.tar.xz 2351200 SHA512:1eacc9ac2cd8d38b8466659b3b9d84b94eb765c8f869d6cca0da131060bbc35c2b31c6148d59690547871a20cea339eac8fbe953b4fe37cf0900862f3fd9621b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.14%2bdfsg-1.debian.tar.xz' libxml2_2.9.14+dfsg-1.debian.tar.xz 28664 SHA512:ec39991892cc7d3d7e76734e05ff16b29f5dcf1783fdfd4eaea56da86fb7b142c616b0fd0f0fe4101dc5767a2c7af12d441097c01069427b1630bf782db4c7fd
```

### `dpkg` source package: `libxrender=1:0.9.10-1build4`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1build4`
- `libxrender1:amd64=1:0.9.10-1build4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libxslt=1.1.34-4build2`

Binary Packages:

- `libxslt1-dev:amd64=1.1.34-4build2`
- `libxslt1.1:amd64=1.1.34-4build2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.34-4build2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4build2.dsc' libxslt_1.1.34-4build2.dsc 2507 SHA512:07b04ca61c5c55f0cb3bbd912a8c855ab58b81197da6b6fffcda315ab4cb7a079927e6efbc38f558fb3f764a8db1ef917e4b9a5d51f0decd5ceb439cf706e179
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA512:1516a11ad608b04740674060d2c5d733b88889de5e413b9a4e8bf8d1a90d712149df6d2b1345b615f529d7c7d3fa6dae12e544da828b39c7d415e54c0ee0776b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA512:9b155d4571daede99cdbf2813a85fb04812737b5e23d3f7c9840225b38f3dbf171623a21645daaee190e7ff9ba38bde932922e96a2a2312c203ffa9917c3baea
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4build2.debian.tar.xz' libxslt_1.1.34-4build2.debian.tar.xz 21636 SHA512:21d861ccb397b17f9a1cc33da287877b998cd6eedd90553bfb4120d893a99907c145b4a29a2f06c30a74f40e3cd4b3e49d31c94fb291018fbe84ce9096ef7ac0
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

### `dpkg` source package: `libyaml=0.2.2-1build2`

Binary Packages:

- `libyaml-0-2:amd64=0.2.2-1build2`
- `libyaml-dev:amd64=0.2.2-1build2`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.2-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1build2.dsc' libyaml_0.2.2-1build2.dsc 2139 SHA512:41b3ce50b076da1118a639496dcda225ed8d7534079f61a470d6d6f80b34c7f0df8e1850024e78a73b25e695c4b10049ce50b09acaca6a2c8145adbf3f41cdad
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2.orig.tar.gz' libyaml_0.2.2.orig.tar.gz 602509 SHA512:0728c89ba43af3cdec22bccaf18c9ad7b07e13cdebed9d8919e2c62cf90bb5e23d2c746fd250320b2827dfcd9f1ce442d3bf8a3fe18b61f9a8d1d7770561e610
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1build2.debian.tar.xz' libyaml_0.2.2-1build2.debian.tar.xz 4284 SHA512:50eb5194764d06438ef0f1a4690a400f1d61ab311a1e72e1c004e1ad15f85de02822012936d7a3f5fc741a325fad490135f3bc14ccf6948e44faa75cabf2d70f
```

### `dpkg` source package: `libzstd=1.5.2+dfsg-1`

Binary Packages:

- `libzstd-dev:amd64=1.5.2+dfsg-1`
- `libzstd1:amd64=1.5.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd-dev/copyright`, `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.2+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg-1.dsc' libzstd_1.5.2+dfsg-1.dsc 2173 SHA512:7651f212659f76627d419741d31070ce15c996a54ded712260b3806c1973a0a46afbd2386c8a8d8b8565481d3659702a8a05a5b1e09a0e28dd9779fbd75f650c
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg.orig.tar.xz' libzstd_1.5.2+dfsg.orig.tar.xz 1404564 SHA512:8e26e9f65d4c649a2a0b75968e491bcad152dd27bca9c9db62a8a11343c6eb361ebe82dec8375efb9a38ecce2417afe628199aeeca1d78c754d4cd1e6fc20542
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.5.2%2bdfsg-1.debian.tar.xz' libzstd_1.5.2+dfsg-1.debian.tar.xz 11820 SHA512:052c0f849654f47d3503a966f23c8c89db29e7f99dea3f400c082e4c2c9dad83ad4986ecad6f4400d90127ed120c006569221cd5ee5438152fb0d3bfca92fa50
```

### `dpkg` source package: `linux=5.15.0-27.28`

Binary Packages:

- `linux-libc-dev:amd64=5.15.0-27.28`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris linux=5.15.0-27.28
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0-27.28.dsc' linux_5.15.0-27.28.dsc 7228 SHA512:aac822f21ca50f5df9be71f6a463956d04555294ac158c89bc1b70c41a73172eb79b86d8a9c7e3c0212c621d2e37576d55f86bc6df1beb1239f500a220f527b6
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0.orig.tar.gz' linux_5.15.0.orig.tar.gz 194969557 SHA512:ae9a32132d5988441c189157703b0f8fa4e232d8d24f7104f944c06827db740beafae55eb37a51eb99b4ac513927cd372321fa1e84afff4d450b786e44414861
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0-27.28.diff.gz' linux_5.15.0-27.28.diff.gz 5796913 SHA512:edb6ec3f2847403964bc7221b4d00a399885d34849343424a9922e4f7048e9946d806031a54d739622d5aa9a64365519442f272751ee0e99fef89c2a56a9c4d3
```

### `dpkg` source package: `lsb=11.1.0ubuntu4`

Binary Packages:

- `lsb-base=11.1.0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu4.dsc' lsb_11.1.0ubuntu4.dsc 2222 SHA512:2b5375ca5938f497f9211d9b85eaf60858c2d59c80ec40a3a04bec6ef47e6685661589f22514f8b2e4a325038feb0375d99e1f905aa93b4a13c3d474e3b86677
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu4.tar.xz' lsb_11.1.0ubuntu4.tar.xz 46152 SHA512:03469c3b85facd88fb4c24b85eb42d6aeab171aa6e5860147ad947e2bbc2f2fe5f78ebd4a457f6af194d33173dccec4f672d1b9d460c070765377d9456bc73da
```

### `dpkg` source package: `lto-disabled-list=26`

Binary Packages:

- `lto-disabled-list=26`

Licenses: (parsed from: `/usr/share/doc/lto-disabled-list/copyright`)

- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lz4=1.9.3-2build2`

Binary Packages:

- `liblz4-1:amd64=1.9.3-2build2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.3-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-2build2.dsc' lz4_1.9.3-2build2.dsc 2091 SHA512:a8f802737139536f8a9c0a3483635ff4dd8a3eba2e0d9d0d27f4f91c17592d1797929d491183dc25de4100a7aa924edefa8ca45eed4968c0e1b7e817f1ae9e1c
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3.orig.tar.gz' lz4_1.9.3.orig.tar.gz 320958 SHA512:c246b0bda881ee9399fa1be490fa39f43b291bb1d9db72dba8a85db1a50aad416a97e9b300eee3d2a4203c2bd88bda2762e81bc229c3aa409ad217eb306a454c
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-2build2.debian.tar.xz' lz4_1.9.3-2build2.debian.tar.xz 14088 SHA512:9f61516a672186299a96aee5b7a71d9cb1ad3db2697fa10b802fef14a63587bb3459281f7300726711a116893c10858914f558aece1d224876e287020a23dde6
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

### `dpkg` source package: `m4=1.4.18-5ubuntu2`

Binary Packages:

- `m4=1.4.18-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-5ubuntu2.dsc' m4_1.4.18-5ubuntu2.dsc 2118 SHA512:093a2b00a5e89a5d48c522766c309970baa194a7abba9f3e65211fc6bfda03b0871c76cc8c96ca371a43f67c40a9cbfb7b9d36765d3e67c07e2288ae1cf39c1b
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA512:06f583efc3855cd8477d8347544f4ae5153a3e50aea74d21968afa7214784ea3ddfc02d0a2b11324120d76a19f2e804d20de11a456b5da929eb6ae469519b174
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA512:effc857a19f1496d6dde2887c0314b37d4b142a435e77614936c730878c798491ad93b28860dddd2601f99a43fa41923729b961004faafc6f798f7bc1842f980
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-5ubuntu2.debian.tar.xz' m4_1.4.18-5ubuntu2.debian.tar.xz 19140 SHA512:38f002fb05a8f016bbde5f2a124747714362a36be51429dad4c0e63d28afd2be66de0870d1d70bae668403606e2b1623f534a801d02fed6593152bd2a7b55a29
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

### `dpkg` source package: `mawk=1.3.4.20200120-3`

Binary Packages:

- `mawk=1.3.4.20200120-3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/mawk/1.3.4.20200120-3/


### `dpkg` source package: `media-types=8.0.0`

Binary Packages:

- `media-types=8.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=8.0.0
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_8.0.0.dsc' media-types_8.0.0.dsc 1620 SHA512:f1f15bb477c452c714689b0f0d4a6ef739c82212ee6b3a4ac6546311cd2305c12b9f38508bc226884029f251ec5a7a0317d0851af8cdeb4375a9575930db76ee
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_8.0.0.tar.xz' media-types_8.0.0.tar.xz 56364 SHA512:fe1b42c1bccf790ae1815e6e6459e8357ed26df9deaa5c57afb85299939d76287da7d8e0b6b51707f82831c6c33322d363ac2a5117e79b42c3f813331bcee506
```

### `dpkg` source package: `mercurial=6.1.2-1`

Binary Packages:

- `mercurial=6.1.2-1`
- `mercurial-common=6.1.2-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/mercurial/6.1.2-1/


### `dpkg` source package: `mpclib3=1.2.1-2build1`

Binary Packages:

- `libmpc3:amd64=1.2.1-2build1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.1-2build1.dsc' mpclib3_1.2.1-2build1.dsc 1984 SHA512:5aa91f39d40bebc1f9ae03506c17687b75ea88d8129baf3a47b6d3d4fe3aba7b1aec499e219b7357747069ea40b8f593b33165c62687a4cb2fcc5e8a21428ffc
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.1.orig.tar.gz' mpclib3_1.2.1.orig.tar.gz 838731 SHA512:3279f813ab37f47fdcc800e4ac5f306417d07f539593ca715876e43e04896e1d5bceccfb288ef2908a3f24b760747d0dbd0392a24b9b341bc3e12082e5c836ee
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.1-2build1.debian.tar.xz' mpclib3_1.2.1-2build1.debian.tar.xz 4576 SHA512:0317f40da1ee5a7ad5733760226ec6ba4cddf7c4fae32b91e771f40bdb1b8a116854cb1cde85566072ef0199d7fbf046ff20fd67ef2ddb655038cb2e19e58662
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

### `dpkg` source package: `mpfr4=4.1.0-3build3`

Binary Packages:

- `libmpfr6:amd64=4.1.0-3build3`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.1.0-3build3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3build3.dsc' mpfr4_4.1.0-3build3.dsc 2066 SHA512:60ea156f6c4a56320ecfb2fefb226b5083363710eacbdec48f36f77bd5265c91548ef28ba775a88c7e927314e5dd757de851001bc7697f863195510047eaf0a3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA512:1bd1c349741a6529dfa53af4f0da8d49254b164ece8a46928cdb13a99460285622d57fe6f68cef19c6727b3f9daa25ddb3d7d65c201c8f387e421c7f7bee6273
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3build3.debian.tar.xz' mpfr4_4.1.0-3build3.debian.tar.xz 12580 SHA512:1126a59104a9556f7ebd622b050b52899bd92442673e6ecbb04e80bc873107b4b61a356373d14b1fff5681090b177e0d3a9a4f212b0f38c347d01ac408222bd0
```

### `dpkg` source package: `mysql-8.0=8.0.28-0ubuntu4`

Binary Packages:

- `libmysqlclient-dev=8.0.28-0ubuntu4`
- `libmysqlclient21:amd64=8.0.28-0ubuntu4`

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


### `dpkg` source package: `mysql-defaults=1.0.8`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.8`
- `mysql-common=5.8+1.0.8`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.8
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.8.dsc' mysql-defaults_1.0.8.dsc 2277 SHA512:da75c1bcea5a463417f6e0c72a708ee63629877e9d92f492dbf9cd9036628d16aee4d1afaf3713274f5e407e21c0e98e6c7212a46da21d3367a544977dcc264c
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.8.tar.xz' mysql-defaults_1.0.8.tar.xz 7316 SHA512:d61adb7640531b51d4f983dec3cd7a5cb6a36a6717ff771681478a2985e3ad27465d3fa567e348eccce0005489aa2973e7fa356549b22a882739f37d82169e9e
```

### `dpkg` source package: `ncurses=6.3+20220423-2`

Binary Packages:

- `libncurses-dev:amd64=6.3+20220423-2`
- `libncurses5-dev:amd64=6.3+20220423-2`
- `libncurses6:amd64=6.3+20220423-2`
- `libncursesw5-dev:amd64=6.3+20220423-2`
- `libncursesw6:amd64=6.3+20220423-2`
- `libtinfo6:amd64=6.3+20220423-2`
- `ncurses-base=6.3+20220423-2`
- `ncurses-bin=6.3+20220423-2`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.3+20220423-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3%2b20220423-2.dsc' ncurses_6.3+20220423-2.dsc 4200 SHA512:6a7194bec8331f7e5396cc58390c6523388a08b6cfc7488dc357112163b2f55d0de7d5060d2591a33b2b074c1fd8b7acb111157c68b9f10a9ed6e21b9551c228
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3%2b20220423.orig.tar.gz' ncurses_6.3+20220423.orig.tar.gz 3611993 SHA512:350a2f36ffea4f98a346217356e2730b6ef115eecd35144b8ef741a119932ab717febb2bd16acc596364084758bd9ecc8223ffcd91e59c9e0700445cfb700284
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3%2b20220423.orig.tar.gz.asc' ncurses_6.3+20220423.orig.tar.gz.asc 729 SHA512:b933258b43863cd1a68dd0ba40d7340dbd2676586aae1409f7dcc33e86f3b0e0e6d1544430632976d96b8ec7a5b3e630c0a81cea3f7f7471eba14ac7194dac3f
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3%2b20220423-2.debian.tar.xz' ncurses_6.3+20220423-2.debian.tar.xz 54600 SHA512:575373307127325f015df4d654037c8294d8ae07c5cd2acb8f145e35d2dfded53cc3c38776a76a4fc3783ddeff8f6f2134eefc0d7d52da456a42871094eea356
```

### `dpkg` source package: `netbase=6.3`

Binary Packages:

- `netbase=6.3`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.3
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.3.dsc' netbase_6.3.dsc 875 SHA512:e21e2c228f5963f34636c646d92280c6307527c1796f3da89a5ec9d26d4a10c08730d68f337f43ebbcd6cc22c4f8fd804673336fbcc9fd41eb1d4f0e687b2a7d
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.3.tar.xz' netbase_6.3.tar.xz 31968 SHA512:3ba7f8b28a9b6ffd89bef62a3c2629cf6ad6b0522319ae7eae46d579aac6f86079930da3b3dd55c76ae48cf6c842f8f162b24324e2f8427e3664fd0db69ed138
```

### `dpkg` source package: `nettle=3.7.3-1build2`

Binary Packages:

- `libhogweed6:amd64=3.7.3-1build2`
- `libnettle8:amd64=3.7.3-1build2`

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
$ apt-get source -qq --print-uris nettle=3.7.3-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3-1build2.dsc' nettle_3.7.3-1build2.dsc 2165 SHA512:3f774011dd48205720ac7e6aa9a44b5afa64c24fce825d6583b58c02f3c8f500ecafa265d18d5deb1ab65d6e938dd76a7917f1d5c3dab0aea28148d531fa26cd
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3.orig.tar.gz' nettle_3.7.3.orig.tar.gz 2383985 SHA512:9901eba305421adff6d551ac7f478dff3f68a339d444c776724ab0b977fe6be792b1d2950c8705acbe76bd924fd6d898a65eded546777884be3b436d0e052437
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3-1build2.debian.tar.xz' nettle_3.7.3-1build2.debian.tar.xz 22100 SHA512:c1935d35e9f04798273053ab92c7405ec225a5d72ba6c2869b0f2bf54b459ac428e113bc149796e91834a8b56082f8bbfbb906a6cd6787142b8932bd1dd83cec
```

### `dpkg` source package: `nghttp2=1.43.0-1build3`

Binary Packages:

- `libnghttp2-14:amd64=1.43.0-1build3`

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

### `dpkg` source package: `numactl=2.0.14-3ubuntu2`

Binary Packages:

- `libnuma1:amd64=2.0.14-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.14-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14-3ubuntu2.dsc' numactl_2.0.14-3ubuntu2.dsc 2110 SHA512:ea29c0e0746cf1b04c3295a2be4809aad18115a7dd0326f8e1bd73465bf0d1031f5853b18e755c4a5de0592e5cb18e50e76ebfbb1f4a92c9bcf13dae28165d28
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14.orig.tar.gz' numactl_2.0.14.orig.tar.gz 107583 SHA512:adaf405f092fd9653f26d00f8c80cb83852c56ebd5d00e714e20d505008e74aa7105b0fb7aa55a605deac0d1491ceff57de931037d33e7944fca105bc6510ed4
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14-3ubuntu2.debian.tar.xz' numactl_2.0.14-3ubuntu2.debian.tar.xz 7588 SHA512:f3e34577c93c315047be275596d59e0481f177e090cd0c7ca8ef6ac3a79eab1ee988003afd49053a0cc6a86bf3f4b0ea387f53da279f9dcbc0d9ed7ca3815fd1
```

### `dpkg` source package: `openexr=2.5.7-1`

Binary Packages:

- `libopenexr-dev=2.5.7-1`
- `libopenexr25:amd64=2.5.7-1`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr25/copyright`)

- `BSD-3-clause`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.5.7-1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.7-1.dsc' openexr_2.5.7-1.dsc 2683 SHA512:ad9ec0d201f62b15cf396bf9fe56f15bf4f993f19cff116ed9d2078909c9fb179a9eb37081710901daf34d016ecb39f802e4dead092c51c0f488f34a3c09fb01
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.7.orig.tar.gz' openexr_2.5.7.orig.tar.gz 27539574 SHA512:e44edfa2dcfff2fe372ed2ba07b39a472e549025978de178eff26be641767d22d1a3b543fb7672d9b7b2e9f4c308667f785829ed6d9032a2b42f2ffa0163de40
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.7.orig.tar.gz.asc' openexr_2.5.7.orig.tar.gz.asc 287 SHA512:9b3978e44b531429aba42b9cc4969a470898d9d74652e3809edb0273ba9b127c471aec6570b5d352be738f59810091c0df2c70d39c16d2c32833d173b270f72c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.7-1.debian.tar.xz' openexr_2.5.7-1.debian.tar.xz 22096 SHA512:eefee3067bc874cd21ecb138ccdf2a0f0bd77faa01626b537e002ce6d2d906b48221e78a8bd33d60874c603b54a1aaf1e987b4e4d3b82df5a67ab9e881c1f5dc
```

### `dpkg` source package: `openjpeg2=2.4.0-6`

Binary Packages:

- `libopenjp2-7:amd64=2.4.0-6`
- `libopenjp2-7-dev:amd64=2.4.0-6`

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
$ apt-get source -qq --print-uris openjpeg2=2.4.0-6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.4.0-6.dsc' openjpeg2_2.4.0-6.dsc 2822 SHA512:d3057b995fa94759b0e4f294dfbd26e745c56c32f8dcd22c7f457e3cf1f7b14590c7ac6be2edc078e7a61281512fbaebb3366bd346773d015f874925ecabaa32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.4.0.orig.tar.xz' openjpeg2_2.4.0.orig.tar.xz 1396964 SHA512:717ead13e0805d52138bedef1a77d51b676c5a2b882ca7f2206b665b3ba5ea2b435fd81c09780e6c1f14400a49c82fcd1eb2cbea1e1d207b541e98797ecd684f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.4.0-6.debian.tar.xz' openjpeg2_2.4.0-6.debian.tar.xz 21124 SHA512:cdd8a1d29388d02c37612183fef2ff679133630871323894f46e7f4a56480118e1e03573b2eea2179ce0f92d6aca6a15ee8e9f382e036d7ff0cb0f1744f2df3e
```

### `dpkg` source package: `openldap=2.5.11+dfsg-1~exp1ubuntu3`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.11+dfsg-1~exp1ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openssh=1:9.0p1-1`

Binary Packages:

- `openssh-client=1:9.0p1-1`

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
$ apt-get source -qq --print-uris openssh=1:9.0p1-1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1-1.dsc' openssh_9.0p1-1.dsc 3347 SHA512:d430c5a45ed3b6cdb7f9a11bdbaa029936b0fcf80e06cb2e096f5106c7a0717b5436dbec66b093ab4c49bf6ae180013cd31a8f31fbaa7aab4e7b7993506d2418
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1.orig.tar.gz' openssh_9.0p1.orig.tar.gz 1822183 SHA512:613ae95317e734868c6a60d9cc5af47a889baa3124bbdd2b31bb51dd6b57b136f4cfcb5604cca78a03bd500baab9b9b45eaf77e038b1ed776c86dce0437449a9
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1.orig.tar.gz.asc' openssh_9.0p1.orig.tar.gz.asc 833 SHA512:7b1445764058435d2fa8a9c7553643983650d4232036c088e46e44beeb538d32cba88f775b1be9da5f21a01d6caea59b3dc4714507781e9cb946546fa54f169f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_9.0p1-1.debian.tar.xz' openssh_9.0p1-1.debian.tar.xz 176128 SHA512:4279b6c24ad4c0e7951bf7a5cb3f848c4bb19b9ca02972e334a11096797e1e76302bc144c0936b64915827391b1c28a20b3a2fced4d8e8cb4a82f4396cfff418
```

### `dpkg` source package: `openssl=3.0.3-5ubuntu2`

Binary Packages:

- `libssl-dev:amd64=3.0.3-5ubuntu2`
- `libssl3:amd64=3.0.3-5ubuntu2`
- `openssl=3.0.3-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libssl-dev/copyright`, `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `p11-kit=0.24.1-1`

Binary Packages:

- `libp11-kit0:amd64=0.24.1-1`

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
$ apt-get source -qq --print-uris p11-kit=0.24.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1-1.dsc' p11-kit_0.24.1-1.dsc 2501 SHA512:77274b15c2114fbc2a93c9f1b293a3e5e95f82db447eb0955db57ef400d3964f31d9aaf73333892bc0773ffb9fc1ea69273f357ad9186bbc42047e91ee598820
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz' p11-kit_0.24.1.orig.tar.xz 838304 SHA512:8cf170c714bb9e0cf3df93e8ec55b8e3c55cabf2c6a27f177ac6de8b8028985df2ca0216d3215d6828dc2ae3095c4e1a4febe8cb26b88ec321defc66bb011e81
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz.asc' p11-kit_0.24.1.orig.tar.xz.asc 833 SHA512:c9cb909a9443cc554c32d7816add59a1b1225186517a0bc8dc267a638a93de070a6ce57c0bafaf1a2b0a03acbdb0a3c1fdd88a615f402ade13e41d20463a7803
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.1-1.debian.tar.xz' p11-kit_0.24.1-1.debian.tar.xz 23200 SHA512:62abd2fc10f6416388157c7a3ed733adfdd5b954713e3149f9f34f1b1daa7d3a4796e928afbefc0a2e649eed0eb7273429aa0f2f1e3a43cef984f26e66db49a3
```

### `dpkg` source package: `pam=1.4.0-13ubuntu1`

Binary Packages:

- `libpam-modules:amd64=1.4.0-13ubuntu1`
- `libpam-modules-bin=1.4.0-13ubuntu1`
- `libpam-runtime=1.4.0-13ubuntu1`
- `libpam0g:amd64=1.4.0-13ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.4.0-13ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0-13ubuntu1.dsc' pam_1.4.0-13ubuntu1.dsc 2757 SHA512:bf0320aeef4520bd53642298ee0e121ac683423e12af50565251c135eb70d6c7e0f73dad816a6f6fc8652b9e98c9def866c8f3951103bfa25f5d0bf73d8c070e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0.orig.tar.xz' pam_1.4.0.orig.tar.xz 988908 SHA512:26eda95c45598a500bc142da4d1abf93d03b3bbb0f2390fa87c72dcbffa208dbfa115c0b411095c31ee9955e36422ccf3e2df3bd486818fafffef8c4310798c4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0-13ubuntu1.debian.tar.xz' pam_1.4.0-13ubuntu1.debian.tar.xz 167572 SHA512:4ccea35fa18cc1eed8aefabc2cffceeba313bbe4a8d1b5fcf2a462e603ec911b520e6badbb96fc30b99ef616d747e630e94e12c9a7c2d9c791d8b46ceb8aecbc
```

### `dpkg` source package: `pango1.0=1.50.7+ds-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.50.7+ds-1`
- `libpangocairo-1.0-0:amd64=1.50.7+ds-1`
- `libpangoft2-1.0-0:amd64=1.50.7+ds-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Apache-2`
- `Apache-2.0`
- `Bitstream-Vera`
- `CC-BY-SA-3.0`
- `CC-BY-SA-3.0,`
- `CC0-1.0`
- `CC0-1.0,`
- `Chromium-BSD-style`
- `Example`
- `Expat`
- `GPL-2+`
- `GPL-2+,`
- `GPL-2.0`
- `GPL-3.0`
- `GPL-3.0+`
- `GPL-3.0+,`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2+,`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.1`
- `OFL-1.1`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.50.7+ds-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.7%2bds-1.dsc' pango1.0_1.50.7+ds-1.dsc 3857 SHA512:1af587bbd736d47088d5e43d140b6f7cef74981d37a4f8feb997646124fb0dbcc77eacc682557e8ea51f24c63fc44216b273664e2688f31c42f7cba8c2590fc2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.7%2bds.orig.tar.xz' pango1.0_1.50.7+ds.orig.tar.xz 2673928 SHA512:fc73810b09a967d1280cdd364a0e4c19a71312a1e3e1d7cfc994a72dce7a8daf2085e048ab10d52e3c255d10db3b2f2ec8a4177ed36fd668fc4bd9dc9c828674
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.7%2bds-1.debian.tar.xz' pango1.0_1.50.7+ds-1.debian.tar.xz 50324 SHA512:0007e4059a0c2c2ed6f0740cf96dbcbf07b2574c6de5d72b5cc32d2f3ee372b26c51bb7f44adf83913d7d11aedf77f841fc0160222840c857e9469b0a315f556
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

### `dpkg` source package: `pcre2=10.40-1`

Binary Packages:

- `libpcre2-16-0:amd64=10.40-1`
- `libpcre2-32-0:amd64=10.40-1`
- `libpcre2-8-0:amd64=10.40-1`
- `libpcre2-dev:amd64=10.40-1`
- `libpcre2-posix3:amd64=10.40-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.40-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.40-1.dsc' pcre2_10.40-1.dsc 2286 SHA512:133e74f3f677d50d6db959839d52946db4493da680feedfd3610289e7ffba80529ef9b18c4346292805e64b6e204bdf8cf04e58627c14738984844709e3f36ce
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.40.orig.tar.gz' pcre2_10.40.orig.tar.gz 2359622 SHA512:679c6f540571850adec880934812e4f26f08ad858c776f10d1ed68ed3c0d4f91f6e1b53d781b53340af43a22c521e585cfc908f3659013c630a320e4fb246dc2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.40-1.diff.gz' pcre2_10.40-1.diff.gz 7134 SHA512:fe2beb58f778ff1bf43c74de129266d2ab4b7a50dea7e7217e8b6edf83451672f99bf50ccb55245acce3bfa2731d2aacb7f03cd623844d3ae7210d97ddfd92e2
```

### `dpkg` source package: `pcre3=2:8.39-14`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-14`
- `libpcre3:amd64=2:8.39-14`
- `libpcre3-dev:amd64=2:8.39-14`
- `libpcre32-3:amd64=2:8.39-14`
- `libpcrecpp0v5:amd64=2:8.39-14`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-14
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-14.dsc' pcre3_8.39-14.dsc 2226 SHA512:7d70d8acc6cfa87516f23570b9a20f080d8af660f6fa9237aa0b01cf1888217ddf9f9102ad95888126ea0d1b5c7bd3162fc5210d797c190a831e1e360156e356
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA512:8b0f14ae5947c4b2d74876a795b04e532fd71c2479a64dbe0ed817e7c7894ea3cae533413de8c17322d305cb7f4e275d72b43e4e828eaca77dc4bcaf04529cf6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-14.debian.tar.gz' pcre3_8.39-14.debian.tar.gz 27185 SHA512:e0678498cbfc9cbebdadf8591fdf58ff6a297510bb06d1f378d3c3ffb3882b9a5eca2a624ebd98e8bf175c38453141f4519612f4111eb491718daaf22b2b9202
```

### `dpkg` source package: `perl=5.34.0-3ubuntu1`

Binary Packages:

- `libperl5.34:amd64=5.34.0-3ubuntu1`
- `perl=5.34.0-3ubuntu1`
- `perl-base=5.34.0-3ubuntu1`
- `perl-modules-5.34=5.34.0-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libperl5.34/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.34/copyright`)

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
$ apt-get source -qq --print-uris perl=5.34.0-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0-3ubuntu1.dsc' perl_5.34.0-3ubuntu1.dsc 2993 SHA512:6f65ee700ac9a4d45ff9c676d1ae6dac1d75cfd4d071e4c88cd00a0579dcdbc68f194121a610f4d8f460d5d086d118dc0ec2d1b016d56c945ce262702dec2c6c
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0.orig-regen-configure.tar.xz' perl_5.34.0.orig-regen-configure.tar.xz 415412 SHA512:2581152e0747105314c4fa4167f1f97d286436b996341b9b75e4099ba18f15eb0d2b42888622fbe9b5499d3fe304bc8aa9ad207a945f590135beccfb68ea28b0
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0.orig.tar.xz' perl_5.34.0.orig.tar.xz 12881416 SHA512:691b4b31eacec357191fba777612b4e3eae59e946a22998a50766697c0d61db1d42a9b3bc1e41abf0d1ca1893e4a7c06d7bf3290480cf03d7f79befd7a8a3267
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0-3ubuntu1.debian.tar.xz' perl_5.34.0-3ubuntu1.debian.tar.xz 167356 SHA512:670be9084642fbce2ac074c684ec857a57f5ce3a87bfa20e93a4504876abb38821bc31a39deca01eda767ad4a09bd97709990e8704fe4225f9401916c151313a
```

### `dpkg` source package: `pinentry=1.2.0-1ubuntu1`

Binary Packages:

- `pinentry-curses=1.2.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.2.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.0-1ubuntu1.dsc' pinentry_1.2.0-1ubuntu1.dsc 2999 SHA512:0808c1cff863c9d5429665b5595217a2363c3e2487447c283e285bc995af5e065545671726b84e37de2443fe3c689b0ee0683228ab5df6f52a657eee32b54c82
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.0.orig.tar.bz2' pinentry_1.2.0.orig.tar.bz2 498390 SHA512:19cea79aa3982d1f0d75220c8e24ca38d6c49475c6f4c5aa7101151b4690db23ed316096a4a411136e716ba4eb471f48f9b09556e5c9837533c2356b9b384b63
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.0.orig.tar.bz2.asc' pinentry_1.2.0.orig.tar.bz2.asc 228 SHA512:2548e62a7d18688c763a044e07d2e3ec52b9f57054ebd869e781aae4c64b50d36032f45931914e5e3c6645ca12c3ed8dcc285ce58f52c9770bb20ad8f895ef24
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.2.0-1ubuntu1.debian.tar.xz' pinentry_1.2.0-1ubuntu1.debian.tar.xz 18936 SHA512:2d77b795e564bf86286216a6bd6c454a540c77c932a7ee676063ad1ab0e9faf4f5506b965b01204b6535497ddbf3adc00cf0bf88410a923f551a9bc1818e7f39
```

### `dpkg` source package: `pixman=0.40.0-1build4`

Binary Packages:

- `libpixman-1-0:amd64=0.40.0-1build4`
- `libpixman-1-dev:amd64=0.40.0-1build4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.40.0-1build4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0-1build4.dsc' pixman_0.40.0-1build4.dsc 2153 SHA512:b7893cacd1f4ab6b1012e4493fea0f5c95361cedd9ac1b4125b0660789724f3bfac0f3d2c17461390b77573bb41eb6fdc5370bde74b0a08669707820b415d75f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0.orig.tar.gz' pixman_0.40.0.orig.tar.gz 913976 SHA512:063776e132f5d59a6d3f94497da41d6fc1c7dca0d269149c78247f0e0d7f520a25208d908cf5e421d1564889a91da44267b12d61c0bd7934cd54261729a7de5f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0-1build4.diff.gz' pixman_0.40.0-1build4.diff.gz 327140 SHA512:1e27c3ca21d9e31640dfefe5576fa3d191890e47b0369c101d724aa95dd68bd9fc97d56b4b8ed700b68cc895a196e2ab3ceb5f77ed8c2e00655cfd20281edd92
```

### `dpkg` source package: `pkg-config=0.29.2-1ubuntu3`

Binary Packages:

- `pkg-config=0.29.2-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.2-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu3.dsc' pkg-config_0.29.2-1ubuntu3.dsc 1910 SHA512:ebeb396389e63ec008928941d0b9b71c55e04c96dccfa799fcbc1eaf0f14003a71c96dd8a54c6e8dca9aa0072c329c1af76d1fed385e11e6c380649c2bf968a3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2.orig.tar.gz' pkg-config_0.29.2.orig.tar.gz 2016830 SHA512:4861ec6428fead416f5cbbbb0bbad10b9152967e481d4b0ff2eb396a9f297f552984c9bb72f6864a37dcd8fca1d9ccceda3ef18d8f121938dbe4fdf2b870fe75
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu3.diff.gz' pkg-config_0.29.2-1ubuntu3.diff.gz 10134 SHA512:881ecd107c06f14b6e42a1c3e85a1233f9c92b0666dc5ad1a5fac21d4a64423dcff40c67bdff88311babde5465be82bd5eea8d863bce088468fdff828d8b98ab
```

### `dpkg` source package: `postgresql-14=14.3-1`

Binary Packages:

- `libpq-dev=14.3-1`
- `libpq5:amd64=14.3-1`

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

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/postgresql-14/14.3-1/


### `dpkg` source package: `procps=2:3.3.17-6ubuntu2`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-6ubuntu2`
- `procps=2:3.3.17-6ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-6ubuntu2.dsc' procps_3.3.17-6ubuntu2.dsc 2237 SHA512:0692d993d91644b7e2f4414cad81282c43dd5144e2f650d3e680a4ba62bb3545860c23f8ad3c99d05bf2ceea31e3f8772a4b0b9f79ea56c76fd1f49f3982ba61
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA512:59e9a5013430fd9da508c4655d58375dc32e025bb502bb28fb9a92a48e4f2838b3355e92b4648f7384b2050064d17079bf4595d889822ebb5030006bc154a1a7
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-6ubuntu2.debian.tar.xz' procps_3.3.17-6ubuntu2.debian.tar.xz 34228 SHA512:68ba4678fde89a5f7fce8b04e5ea0b24f9addc7c15b949b01f908cb9a179d68eb8313fc108a99f260d3cb5dff9fd5c9d33f678d3d8bfdd0cba02bcdd9b0bd3c5
```

### `dpkg` source package: `python3-defaults=3.10.4-0ubuntu2`

Binary Packages:

- `libpython3-stdlib:amd64=3.10.4-0ubuntu2`
- `python3=3.10.4-0ubuntu2`
- `python3-minimal=3.10.4-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.10.4-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.10.4-0ubuntu2.dsc' python3-defaults_3.10.4-0ubuntu2.dsc 3051 SHA512:7439bf4c899f2911807954de0828214124205a37db8d21549a6835011ef6e2926bb8695bf104b541e5ef6ae78a9261121063c14012c00af39896d72665fa18e1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.10.4-0ubuntu2.tar.gz' python3-defaults_3.10.4-0ubuntu2.tar.gz 145230 SHA512:e7d652225cbd08c8cdf367948c479cc2315883032d34c68ce5b688908ba535345d18e66bd124a4eba3828d37ce4c6efd6b8764f0bbc6518740e70bc5e3eef521
```

### `dpkg` source package: `python3-stdlib-extensions=3.10.4-0ubuntu2`

Binary Packages:

- `python3-distutils=3.10.4-0ubuntu2`
- `python3-lib2to3=3.10.4-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.10.4-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.10.4-0ubuntu2.dsc' python3-stdlib-extensions_3.10.4-0ubuntu2.dsc 2525 SHA512:a9b4967c4fff1621da6e0f09d9b2d35a9ff240f46a327caacb373401f92caf3714d19333be3fc4765044e0613b1907f64acd4390d474391333ba0a06ca26f7ef
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.10.4.orig.tar.xz' python3-stdlib-extensions_3.10.4.orig.tar.xz 1113688 SHA512:44ab4d6d883f62a2ebfe6585509caef63d74daea5970487231646c5adf9622e3f979c552867520bb08a7254520d23c6593602a6136ecce32eeaa5e941bd142a3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.10.4-0ubuntu2.debian.tar.xz' python3-stdlib-extensions_3.10.4-0ubuntu2.debian.tar.xz 25376 SHA512:21fae5e2ebc18455df8d9ac2e1c7ffd6cf8ae45f1fc9e1a41e99a1878225398b0f8df13d74f70eafb7868860f0ced905f772ad58ca853592e005072ef84f95a3
```

### `dpkg` source package: `python3.10=3.10.4-4`

Binary Packages:

- `libpython3.10-minimal:amd64=3.10.4-4`
- `libpython3.10-stdlib:amd64=3.10.4-4`
- `python3.10=3.10.4-4`
- `python3.10-minimal=3.10.4-4`

Licenses: (parsed from: `/usr/share/doc/libpython3.10-minimal/copyright`, `/usr/share/doc/libpython3.10-stdlib/copyright`, `/usr/share/doc/python3.10/copyright`, `/usr/share/doc/python3.10-minimal/copyright`)

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

- http://snapshot.debian.org/package/python3.10/3.10.4-4/


### `dpkg` source package: `readline=8.1.2-1.2`

Binary Packages:

- `libreadline-dev:amd64=8.1.2-1.2`
- `libreadline8:amd64=8.1.2-1.2`
- `readline-common=8.1.2-1.2`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1.2-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.2.dsc' readline_8.1.2-1.2.dsc 2638 SHA512:b6649e86ad55274944091a5cb5392e73c0c932628f752fd551f1ef65aa3ca0f49d235c81cfa21f87ae1515a8fbbd5c879e6f3440516f8b9da9ab772d287f3deb
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2.orig.tar.gz' readline_8.1.2.orig.tar.gz 2993073 SHA512:b512275c8aa8b3b3178366c6d681f867676fc1c881e375134a88e9c860a448535e04ca43df727817fd0048261e48203e88bd1c086e86572022d1d65fb0350e4d
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.2.debian.tar.xz' readline_8.1.2-1.2.debian.tar.xz 29600 SHA512:f71c739ee97c610a87bdca8ba71e86e62ac92b4c5658199a651c5f498bd2ace43ebff299a20d52c642937e3db78b636b924c64ec7f8219e374b92ec87b5efb58
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

### `dpkg` source package: `sed=4.8-1ubuntu2`

Binary Packages:

- `sed=4.8-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.8-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8-1ubuntu2.dsc' sed_4.8-1ubuntu2.dsc 2217 SHA512:310ccdf0bac73d16c8898fd600acbeceb534a1be53c795fc6f6059eccb431b45ef9ebcde147c150f9fd5e0d33161269f53e191bb26a095b45339a28b1c3381b2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8.orig.tar.xz' sed_4.8.orig.tar.xz 1348048 SHA512:7de25d9bc2981c63321c2223f3fbcab61d7b0df4fcf7d4394b72400b91993e1288d8bf53948ed5fffcf5a98c75265726a68ad4fb98e1d571bf768603a108c1c8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8.orig.tar.xz.asc' sed_4.8.orig.tar.xz.asc 833 SHA512:9b886bdbd18ee2d60608cee3fd2b4193a1b6c3309d887ee05828c14b89b7b515dbf042a9e0ebdd13e6ccfa42e3cd217a408c796d68c4ebedaaa64f795000f095
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8-1ubuntu2.debian.tar.xz' sed_4.8-1ubuntu2.debian.tar.xz 60936 SHA512:c4f0c5b3f75acbcb213e78f5696129e83bc721031be3c756150e84b7aa7e725ac0d5afacbe18e91d39bc2b7892986d92e1e21db89601ccf2bccb8ac088482180
```

### `dpkg` source package: `sensible-utils=0.0.17`

Binary Packages:

- `sensible-utils=0.0.17`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.17
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.17.dsc' sensible-utils_0.0.17.dsc 1733 SHA512:33e94cbe40fbcb083564b4e4f5947f7c4dc0da0724245d19290667cf8a56eb60ba5b94c0c85e8eee2ae7c988a25a094e7edff3159bbe4339dcf9136a6336f2f7
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.17.tar.xz' sensible-utils_0.0.17.tar.xz 66648 SHA512:fb7803cacc4222f232f64850e5559aca0b56ad98b6fd31f36c89740d72f7a235e7f2934ebce1d788882bff7196d59a2ed6cc3584f31e1c1c9e3593cedca2382b
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


### `dpkg` source package: `shadow=1:4.11.1+dfsg1-2ubuntu1`

Binary Packages:

- `login=1:4.11.1+dfsg1-2ubuntu1`
- `passwd=1:4.11.1+dfsg1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.11.1+dfsg1-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.11.1%2bdfsg1-2ubuntu1.dsc' shadow_4.11.1+dfsg1-2ubuntu1.dsc 2523 SHA512:63b73e3d999b8a09c66432d2f08c143b3c735389af1b7b784a1a22f6b401a8e0f2944144a1dce2f2a71f2bc8466fc3362e72a67ac26b2cdf20978928208fc89d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.11.1%2bdfsg1.orig.tar.xz' shadow_4.11.1+dfsg1.orig.tar.xz 1704716 SHA512:d3f03e41f395ae608e93f7216193fe607d28d9ef85acff46c1f0c828bc630884d847f2f020e497140eb03e22447090eae603ef7affa7c376b6f6b08318fde9f3
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.11.1%2bdfsg1-2ubuntu1.debian.tar.xz' shadow_4.11.1+dfsg1-2ubuntu1.debian.tar.xz 90004 SHA512:0fa2b5365fabd22b27a1df15b39cb8a36fd72fc0ac54dc851fa7f1b3d053ef68a339f6fd568bbf7d4a16e8ebde40b5ce4b3b59e9c88e911b289a79c7375bf17c
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

### `dpkg` source package: `sqlite3=3.38.5-1`

Binary Packages:

- `libsqlite3-0:amd64=3.38.5-1`
- `libsqlite3-dev:amd64=3.38.5-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.38.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.38.5-1.dsc' sqlite3_3.38.5-1.dsc 2487 SHA512:66fdd8c56a5715160599f40038a81311092882a04c38e7bc56d48cd3c0597242d022fa7be2247401bd719c8561afe14c33935be1ad0f33720f43a90bbe2337af
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.38.5.orig-www.tar.xz' sqlite3_3.38.5.orig-www.tar.xz 5739536 SHA512:9790ff45220f7f5e9c4cb1a590f9d4e42a4a06ec2fde656a154668d670d725442d9f5cd169eed54b85f1d0b52ff7fb76236d93c2c7aa4196d3d659462c0121f8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.38.5.orig.tar.xz' sqlite3_3.38.5.orig.tar.xz 7670860 SHA512:e15e2f9a3fc612f90e0bb71ff3664eb5aa78539856906267bfc0119dbe8302bb9764545a925e938a63f690e48c9c2b90102be2b91587cc1308fcc31ad9f2ba20
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.38.5-1.debian.tar.xz' sqlite3_3.38.5-1.debian.tar.xz 28960 SHA512:c5f54f4b8abec5fce7d945b9240ebacf6024c5537ea9c41db26764d2acc08e4a09f32f185a5835cad96c54b445520f04ae52e4bbb134e5138f75acb4f86069bb
```

### `dpkg` source package: `subversion=1.14.2-1`

Binary Packages:

- `libsvn1:amd64=1.14.2-1`
- `subversion=1.14.2-1`

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

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/subversion/1.14.2-1/


### `dpkg` source package: `systemd=249.11-0ubuntu3.1`

Binary Packages:

- `libsystemd0:amd64=249.11-0ubuntu3.1`
- `libudev1:amd64=249.11-0ubuntu3.1`

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


### `dpkg` source package: `sysvinit=3.01-1ubuntu1`

Binary Packages:

- `sysvinit-utils=3.01-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=3.01-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.01-1ubuntu1.dsc' sysvinit_3.01-1ubuntu1.dsc 2138 SHA512:650c939b7af5189cddf6509dd2b6a995c7b389ab4ee33bdad267d8c2b5b5506716b03e512563ed3e3265b32d2d1a9119ee0193f3dc82354896029ae124d2a276
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.01.orig.tar.xz' sysvinit_3.01.orig.tar.xz 126400 SHA512:d3b197fcfccfbc2ad95fe208fb37ed1fcc8173a7a0254528c0d8c6800b054d96e20b48274c55137f19305c105700c35974d454b4bbf5e51fbbf5c082d562167b
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_3.01-1ubuntu1.debian.tar.xz' sysvinit_3.01-1ubuntu1.debian.tar.xz 131304 SHA512:4c835855b58742480284b17959d54b8ac734466fc87321ddf021b61bb3e38b58aab6d07a7f27f09c0b109b4e442c0dce4d797feccce2884f5b401e13abf73554
```

### `dpkg` source package: `tar=1.34+dfsg-1build3`

Binary Packages:

- `tar=1.34+dfsg-1build3`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1build3.dsc' tar_1.34+dfsg-1build3.dsc 2122 SHA512:b09665298f4768ea7451ca9811f6b320fc0e70c314ab7b1e78afc0c470dc4be27153a17b39f629584b7f9489493dfe91575be3cc5d2f808e12c4bc4e645bee6e
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA512:ec5553c53c4a5f523f872a8095f699c17bf41400fbe2f0f8b45291ccbaf9ac51dea8445c81bd95697f8853c95dcad3250071d23dbbcab857a428ee92e647bde9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1build3.debian.tar.xz' tar_1.34+dfsg-1build3.debian.tar.xz 19416 SHA512:3fbe7b908963df828585139f884762b698c14a2fc37618dcf3adb90819b160c8ea7aaa2e9dc9470abf40bd5100710dd1292f666cb77865ef3c558729dd313521
```

### `dpkg` source package: `tiff=4.4.0~rc1-1`

Binary Packages:

- `libtiff-dev:amd64=4.4.0~rc1-1`
- `libtiff5:amd64=4.4.0~rc1-1`
- `libtiffxx5:amd64=4.4.0~rc1-1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.4.0~rc1-1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.4.0%7erc1-1.dsc' tiff_4.4.0~rc1-1.dsc 2213 SHA512:f8f2ad84e4ce68f9d6853cc24366d5a84e89b96848d1e78847b3abda697fd61e69fc47b4ff897ebcd5e5efb0f632193ab8bd3bafdea4a08327cdff3864b12d77
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.4.0%7erc1.orig.tar.bz2' tiff_4.4.0~rc1.orig.tar.bz2 2072932 SHA512:cfeac51bfefaab27600131872d460760beaf2e3c8b7308750880f92c7236fbaedf289a53b85a694b108500cbb1a3984944c64c8f23fa318a6dd7802fc6744d04
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.4.0%7erc1-1.debian.tar.xz' tiff_4.4.0~rc1-1.debian.tar.xz 20896 SHA512:9fd60cede295672f0ee6822818ed651b3a6757fe0ca6688ff5d761a7776f7a4be1655c32acf52d7f50ba81aaa4d98910b435c342a672b97940be675b83a9b26c
```

### `dpkg` source package: `tzdata=2022a-0ubuntu1`

Binary Packages:

- `tzdata=2022a-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2022a-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022a-0ubuntu1.dsc' tzdata_2022a-0ubuntu1.dsc 2085 SHA512:189d384e3910116562965784605c7f45636ad54cb18f1d46bb9a43daf7a9dedafd52f05795de9e02cce7e414ec12a5a75d9f9f7772ce29917a14d1230b692a16
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022a.orig.tar.gz' tzdata_2022a.orig.tar.gz 425833 SHA512:542e4559beac8fd8c4af7d08d816fd12cfe7ffcb6f20bba4ff1c20eba717749ef96e5cf599b2fe03b5b8469c0467f8cb1c893008160da281055a123dd9e810d9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022a-0ubuntu1.debian.tar.xz' tzdata_2022a-0ubuntu1.debian.tar.xz 172576 SHA512:9d373a6a8d55530338b091fb0bd8ec543513d3d85df9fb2672aaa120416c130b558282fef7da9917433c0b46d29dee66b48b51635cda04b7982f4227c9be535e
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

### `dpkg` source package: `unzip=6.0-26ubuntu3`

Binary Packages:

- `unzip=6.0-26ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-26ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-26ubuntu3.dsc' unzip_6.0-26ubuntu3.dsc 1832 SHA512:e79ab0cebdcf3b7e070fc66bc337adbfd3304a692a7438b179e1439fe3794acd63449273081490eb730e339b44cdd81a591fa62daa22b6e59f403bfd8b9ef0b6
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA512:0694e403ebc57b37218e00ec1a406cae5cc9c5b52b6798e0d4590840b6cdbf9ddc0d9471f67af783e960f8fa2e620394d51384257dca23d06bcd90224a80ce5d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-26ubuntu3.debian.tar.xz' unzip_6.0-26ubuntu3.debian.tar.xz 27076 SHA512:096b05833305d3efc8d775c046241c0dc307ade2adba9aa80f8e9c7c19f41b0ade69a0729776d8e60689251612586854bbbcfb0ace84b8e5ef67148889154965
```

### `dpkg` source package: `usrmerge=25ubuntu2`

Binary Packages:

- `usrmerge=25ubuntu2`

Licenses: (parsed from: `/usr/share/doc/usrmerge/copyright`)

- `GPL v2`
- `GPL-2`
- `later (please see /usr/share/common-licenses/GPL-2)`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=25ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_25ubuntu2.dsc' usrmerge_25ubuntu2.dsc 1614 SHA512:2f0ea8dbed8277d1fef2f2c70c0075ce509579161fe2dc3a161919d3015c67caff01aa14ba3df7fa7d6b45ce63dbad48389c418781334d83e308ee16988fa9bc
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_25ubuntu2.tar.xz' usrmerge_25ubuntu2.tar.xz 12812 SHA512:dac8ccc7e2b75c424990713869f80d62d22e1cd86cb35c1784c7e76a12096b8c3f3000cefb406456f6f5c459d14858e710d426ee11714d1a5e342e04186f8353
```

### `dpkg` source package: `utf8proc=2.7.0-3`

Binary Packages:

- `libutf8proc2:amd64=2.7.0-3`

Licenses: (parsed from: `/usr/share/doc/libutf8proc2/copyright`)

- `Expat`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris utf8proc=2.7.0-3
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.7.0-3.dsc' utf8proc_2.7.0-3.dsc 2162 SHA512:715ebac4f4159744be21331ffed20228b00e81807b208489194c16be4654d10cb6350950e203e435568d8facb006c021e18893d145f4a19189ee54b9720a6049
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.7.0.orig.tar.gz' utf8proc_2.7.0.orig.tar.gz 187906 SHA512:29f7883de13302d609e8755872ed43174e70076e9681b4ac3f9b03e50295c45d9972c193bc81f94ad7e11e2d33a46cad5a30a80873173e6e1ae242101ebb3bed
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.7.0-3.debian.tar.xz' utf8proc_2.7.0-3.debian.tar.xz 5608 SHA512:b0c8e5c7d348d7fa66c55872c88c8698aab33734cea340ed851a10da55f786b1ccd27098f075a72eb3711435de119873b2938a031e0de38d7b2710d024d1dc7f
```

### `dpkg` source package: `util-linux=2.38-4ubuntu1`

Binary Packages:

- `bsdutils=1:2.38-4ubuntu1`
- `libblkid-dev:amd64=2.38-4ubuntu1`
- `libblkid1:amd64=2.38-4ubuntu1`
- `libmount-dev:amd64=2.38-4ubuntu1`
- `libmount1:amd64=2.38-4ubuntu1`
- `libsmartcols1:amd64=2.38-4ubuntu1`
- `libuuid1:amd64=2.38-4ubuntu1`
- `mount=2.38-4ubuntu1`
- `util-linux=2.38-4ubuntu1`
- `util-linux-extra=2.38-4ubuntu1`
- `uuid-dev:amd64=2.38-4ubuntu1`

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
$ apt-get source -qq --print-uris util-linux=2.38-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38-4ubuntu1.dsc' util-linux_2.38-4ubuntu1.dsc 4608 SHA512:0e8cec89e38428defa8545e4c56a6cb7033ab3a5460ec4c0fe43f9855a3459f07b99586cf23f6bc7e445014f21bbf53dec424b94325a21b8a55e76aa7f2778c3
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38.orig.tar.xz' util-linux_2.38.orig.tar.xz 7349140 SHA512:d0f7888f457592067938e216695871ce6475a45d83a092cc3fd72b8cf8fca145ca5f3a99122f1744ef60b4f773055cf4e178dc6c59cd30837172aee0b5597e8c
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.38-4ubuntu1.debian.tar.xz' util-linux_2.38-4ubuntu1.debian.tar.xz 100876 SHA512:d07568f442cfc467107637b555b0f785c5b18543554d3cbd991b92ed9bc729447c9ac36adc295ee018c68fb64944e40393ede0b11bfa991b7e4f573a5def49a5
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

- `x11proto-dev=2022.1-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-dev/copyright`)

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

### `dpkg` source package: `xz-utils=5.2.5-2.1`

Binary Packages:

- `liblzma-dev:amd64=5.2.5-2.1`
- `liblzma5:amd64=5.2.5-2.1`
- `xz-utils=5.2.5-2.1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.dsc' xz-utils_5.2.5-2.1.dsc 2402 SHA512:2ca63eb555673c2bdd1ee56862420fb7f794fd65924d9a74eb8399f594f91eb0c1943618ffe81bbdb62b7102a23622fabb9f03ef9911b3f0f0d3d90e48dfb066
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA512:59266068a51cb616eb31b67cd8f07ffeb2288d1391c61665ae2ec6814465afac80fec69248f6a2f2db45b44475af001296a99af6a32287226a9c41419173ccbb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.debian.tar.xz' xz-utils_5.2.5-2.1.debian.tar.xz 34916 SHA512:e9593ce4cff247ff419ba8d749d2b58f61726e413b11030e137c3fb76f6bf4a23f41c6b65406d2590e3111ea2eec5be14422e3b96aa25edfa95df9b2376f3041
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu9`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu9`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2ubuntu9`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu9
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu9.dsc' zlib_1.2.11.dfsg-2ubuntu9.dsc 2945 SHA512:26d5a0dc49615cce718e898f384f5f4d4ca2d37e76bb68b4e4feadf64b197a42ce0a85c1e96baa3d8d5c2c8d0a115ba109bf31d735eca49897bf3b9d3b3bad04
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu9.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu9.debian.tar.xz 58360 SHA512:e81d458faa4a79d02620a6a07c25c2838dedb7baa11155523184642d561269b8c9677ba96b571b31be429606b9572469871a99ee48f54d95c729efffb6af8563
```
