# `buildpack-deps:kinetic-scm`

## Docker Metadata

- Image ID: `sha256:8e11b5950fdf2f45c7b523dc7503177e85f5420fdb3548fcecdef4602ba2d115`
- Created: `2022-06-07T02:20:43.531362704Z`
- Virtual Size: ~ 218.84 Mb  
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

### `dpkg` source package: `brotli=1.0.9-2build6`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2build6`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.11+git20210903+057cd650a4ed-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-3build1.dsc' dash_0.5.11+git20210903+057cd650a4ed-3build1.dsc 1834 SHA512:380a677ef7fcd2060f7806e4e552891393adb43bfba82498d143cd2ed4fa0cc7681e573a27bcb0991025a8323f6eb8b113aa1519cf455645556fad968cd26232
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed.orig.tar.xz' dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz 133320 SHA512:eced6bc60ca6ba4394a2ee65d8c6b88eca729c43e47053fc01dec5500ebe002a12f536c128c3fd821a2eb61b97e92c8a0be6d4532926479ce4b7d986be109cb7
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-3build1.debian.tar.xz' dash_0.5.11+git20210903+057cd650a4ed-3build1.debian.tar.xz 42744 SHA512:7dd5b1bcaf76d8de19ad1647862e1140de59822c25d9ab1b42423f16de1e4c606ea393adac12f16a2ce9498d8f9553b8787fc31e5f93feefe36ab84b83402e1e
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.9`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.9`

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


### `dpkg` source package: `e2fsprogs=1.46.5-2ubuntu1`

Binary Packages:

- `e2fsprogs=1.46.5-2ubuntu1`
- `libcom-err2:amd64=1.46.5-2ubuntu1`
- `libext2fs2:amd64=1.46.5-2ubuntu1`
- `libss2:amd64=1.46.5-2ubuntu1`
- `logsave=1.46.5-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `expat=2.4.8-1`

Binary Packages:

- `libexpat1:amd64=2.4.8-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.4.8-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.8-1.dsc' expat_2.4.8-1.dsc 1981 SHA512:78c3bc4c124233d38a690e6dc9e4db0df055fd0e75c75829537b5f62354c08e5a67f14ac6da99d8e070f615f64fa602f3f8062dad14aecc12262ad21d959690a
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.8.orig.tar.gz' expat_2.4.8.orig.tar.gz 8316762 SHA512:452982888e993937dc37968f27eed080d8fb8c8d98935051b195e11051de8fe31217a4d40ae3e7df53fe3265b897823a2a7793af794fd066e0ead4535b5cbc99
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.8-1.debian.tar.xz' expat_2.4.8-1.debian.tar.xz 12556 SHA512:29e304ea46382a34d543a4b079968d493b927ea3272e97e45dffbc5885e39b999bede568628e58e5fc8e973d9c0382d17b114f26d506806577a9497789d850ed
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

### `dpkg` source package: `gcc-12=12.1.0-2ubuntu1`

Binary Packages:

- `gcc-12-base:amd64=12.1.0-2ubuntu1`
- `libgcc-s1:amd64=12.1.0-2ubuntu1`
- `libstdc++6:amd64=12.1.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

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

### `dpkg` source package: `gdbm=1.23-1`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-1`
- `libgdbm6:amd64=1.23-1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

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

### `dpkg` source package: `glibc=2.35-0ubuntu3`

Binary Packages:

- `libc-bin=2.35-0ubuntu3`
- `libc6:amd64=2.35-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

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

- `libgmp10:amd64=2:6.2.1+dfsg-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

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

- `libgssapi-krb5-2:amd64=1.19.2-2`
- `libk5crypto3:amd64=1.19.2-2`
- `libkrb5-3:amd64=1.19.2-2`
- `libkrb5support0:amd64=1.19.2-2`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.19.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2-2.dsc' krb5_1.19.2-2.dsc 3170 SHA512:1b24e80f4b4d9d2635f4a9d45fb9dc6058cd004d0d7bb613a0ce38d4bb4e657e4d1bedeea13f4250d0aca09a039e436313392a2852dc5f2483d2c014388e7f1c
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz' krb5_1.19.2.orig.tar.gz 8741053 SHA512:b90d6ed0e1e8a87eb5cb2c36d88b823a6a6caabf85e5d419adb8a930f7eea09a5f8491464e7e454cca7ba88be09d19415962fe0036ad2e31fc584f9fc0bbd470
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz.asc' krb5_1.19.2.orig.tar.gz.asc 833 SHA512:87c4d096dbb6821401125b8f8a315ce1aac029744ba9670a4f8a2a680e6dd5798e1c6d5d2b68b17fd9a4b3b9c6ff111cd1dcac42f934d48fb20381b3765e0f64
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2-2.debian.tar.xz' krb5_1.19.2-2.debian.tar.xz 106876 SHA512:01d3de8b16728625ddd7860e82d1f98e19fe5c82957ebe816f85e5b0b4405353ce579149b61229a692bf7b8daa1e574599bcf45bb3e1cb6ce89642e2d228c883
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

### `dpkg` source package: `libffi=3.4.2-4`

Binary Packages:

- `libffi8:amd64=3.4.2-4`

Licenses: (parsed from: `/usr/share/doc/libffi8/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

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


### `dpkg` source package: `libsepol=3.3-1build1`

Binary Packages:

- `libsepol2:amd64=3.3-1build1`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `libtirpc=1.3.2-2build1`

Binary Packages:

- `libtirpc-common=1.3.2-2build1`
- `libtirpc3:amd64=1.3.2-2build1`

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
$ apt-get source -qq --print-uris libtirpc=1.3.2-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2build1.dsc' libtirpc_1.3.2-2build1.dsc 2218 SHA512:66c3164c69601f450b2105b7ac755354b0ab7afb1dbc8625b3b8cfee324dfe74662f494bbd1f70fb3c708d1e159a7de02d90fa7f322af7168bbaa98b28cb441d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2.orig.tar.bz2' libtirpc_1.3.2.orig.tar.bz2 513151 SHA512:8664d5c4f842ee5acf83b9c1cadb7871f17b8157a7c4500e2236dcfb3a25768cab39f7c5123758dcd7381e30eb028ddfa26a28f458283f2dcea3426c9878c255
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2build1.debian.tar.xz' libtirpc_1.3.2-2build1.debian.tar.xz 11124 SHA512:5a8e662fe01745b0e608d51de0567d71d3ccbdee6f437730192662615cb4df8a853aead7ee358c4a57cc64b768ff5f5517d45a07b7169aa643a869fb31d453c9
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

### `dpkg` source package: `libxcrypt=1:4.4.27-1`

Binary Packages:

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

### `dpkg` source package: `libzstd=1.5.2+dfsg-1`

Binary Packages:

- `libzstd1:amd64=1.5.2+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

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

### `dpkg` source package: `ncurses=6.3+20220423-2`

Binary Packages:

- `libncurses6:amd64=6.3+20220423-2`
- `libncursesw6:amd64=6.3+20220423-2`
- `libtinfo6:amd64=6.3+20220423-2`
- `ncurses-base=6.3+20220423-2`
- `ncurses-bin=6.3+20220423-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

- `libssl3:amd64=3.0.3-5ubuntu2`
- `openssl=3.0.3-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

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

### `dpkg` source package: `pcre2=10.40-1`

Binary Packages:

- `libpcre2-8-0:amd64=10.40-1`

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

- `libpcre3:amd64=2:8.39-14`

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

- `libreadline8:amd64=8.1.2-1.2`
- `readline-common=8.1.2-1.2`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1.2-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.2.dsc' readline_8.1.2-1.2.dsc 2638 SHA512:b6649e86ad55274944091a5cb5392e73c0c932628f752fd551f1ef65aa3ca0f49d235c81cfa21f87ae1515a8fbbd5c879e6f3440516f8b9da9ab772d287f3deb
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2.orig.tar.gz' readline_8.1.2.orig.tar.gz 2993073 SHA512:b512275c8aa8b3b3178366c6d681f867676fc1c881e375134a88e9c860a448535e04ca43df727817fd0048261e48203e88bd1c086e86572022d1d65fb0350e4d
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.2.debian.tar.xz' readline_8.1.2-1.2.debian.tar.xz 29600 SHA512:f71c739ee97c610a87bdca8ba71e86e62ac92b4c5658199a651c5f498bd2ace43ebff299a20d52c642937e3db78b636b924c64ec7f8219e374b92ec87b5efb58
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

### `dpkg` source package: `sqlite3=3.38.5-1`

Binary Packages:

- `libsqlite3-0:amd64=3.38.5-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

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
- `libblkid1:amd64=2.38-4ubuntu1`
- `libmount1:amd64=2.38-4ubuntu1`
- `libsmartcols1:amd64=2.38-4ubuntu1`
- `libuuid1:amd64=2.38-4ubuntu1`
- `mount=2.38-4ubuntu1`
- `util-linux=2.38-4ubuntu1`
- `util-linux-extra=2.38-4ubuntu1`

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

- `liblzma5:amd64=5.2.5-2.1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.dsc' xz-utils_5.2.5-2.1.dsc 2402 SHA512:2ca63eb555673c2bdd1ee56862420fb7f794fd65924d9a74eb8399f594f91eb0c1943618ffe81bbdb62b7102a23622fabb9f03ef9911b3f0f0d3d90e48dfb066
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA512:59266068a51cb616eb31b67cd8f07ffeb2288d1391c61665ae2ec6814465afac80fec69248f6a2f2db45b44475af001296a99af6a32287226a9c41419173ccbb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.1.debian.tar.xz' xz-utils_5.2.5-2.1.debian.tar.xz 34916 SHA512:e9593ce4cff247ff419ba8d749d2b58f61726e413b11030e137c3fb76f6bf4a23f41c6b65406d2590e3111ea2eec5be14422e3b96aa25edfa95df9b2376f3041
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu9`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu9`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu9
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu9.dsc' zlib_1.2.11.dfsg-2ubuntu9.dsc 2945 SHA512:26d5a0dc49615cce718e898f384f5f4d4ca2d37e76bb68b4e4feadf64b197a42ce0a85c1e96baa3d8d5c2c8d0a115ba109bf31d735eca49897bf3b9d3b3bad04
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu9.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu9.debian.tar.xz 58360 SHA512:e81d458faa4a79d02620a6a07c25c2838dedb7baa11155523184642d561269b8c9677ba96b571b31be429606b9572469871a99ee48f54d95c729efffb6af8563
```
