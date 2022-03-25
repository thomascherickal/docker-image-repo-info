# `buildpack-deps:impish`

## Docker Metadata

- Image ID: `sha256:8f4f2dc8d354435cd0cd1ca02df54d39a82b73e7316f0378acb7c272ffa7ff7a`
- Created: `2022-03-18T06:55:00.2392865Z`
- Virtual Size: ~ 1.06 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-10ubuntu2`

Binary Packages:

- `libacl1:amd64=2.2.53-10ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-10ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-10ubuntu2.dsc' acl_2.2.53-10ubuntu2.dsc 2521 SHA512:022f9359028b32768b46366dd85cedd32f724117f0d6b113ff2e653ec7fea868ceb8648cb75c6151a7b6580fa87be2c45c00fa0479f191f776b0cde2fe3ffbbb
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA512:176b7957fe0e7618e0b7bf2ac5071f7fa29417df718cce977661a576fa184e4af9d303b591c9d556b6ba8923e799457343afa401f5a9f7ecd9022185a4e06716
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA512:a76dcc4f9952bb809aed3c8e0d26e9ae1aa8098ec8492c4d95a23ab74ec92d6896f1eb6307a555098277aa1191cc01d75a2f6a35dd8e8ccb46d3155404bc6f22
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-10ubuntu2.debian.tar.xz' acl_2.2.53-10ubuntu2.debian.tar.xz 25688 SHA512:4565388ead3d7f12ff2240f46dc2b2e6f9c2f26ab64fcf5838f9c3e61a12f6d29cc50b0a4bee7f47d9d27fc530d81ce4e1ea45ff8a01c8dff9acea73153e03b3
```

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

### `dpkg` source package: `aom=1.0.0.errata1-3build1`

Binary Packages:

- `libaom0:amd64=1.0.0.errata1-3build1`

Licenses: (parsed from: `/usr/share/doc/libaom0/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `ISC`
- `public-domain-md5`

Source:

```console
$ apt-get source -qq --print-uris aom=1.0.0.errata1-3build1
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_1.0.0.errata1-3build1.dsc' aom_1.0.0.errata1-3build1.dsc 2273 SHA512:79e3c67a1e7769c897e4106def183b0ecb4e493cced66b9f4def35f8fb163dc6b7b6631c13359e647b1884a228d161b4a8dc10b3c7f0baff6f7c51da89dcbd42
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_1.0.0.errata1.orig.tar.xz' aom_1.0.0.errata1.orig.tar.xz 1898808 SHA512:d6b97ce39d0ed37ff3a11293548a454682b56d02afc8ae9669dca57083e2dcec8491f5a3dcb714b8cd03e902c4f6e059a175fcade461ac09a13fc746ba812826
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_1.0.0.errata1-3build1.debian.tar.xz' aom_1.0.0.errata1-3build1.debian.tar.xz 21208 SHA512:a98b6e36795949234764d4d5249bbe407c87ecd6cc87298aa26af1042fc8fae8507be5880f129e91e275982aa9a9fcaab1aff11ee315ccd319bfb5b6642064d4
```

### `dpkg` source package: `apr-util=1.6.1-5ubuntu2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu2.dsc' apr-util_1.6.1-5ubuntu2.dsc 2611 SHA512:f8146362fbedfd185fcbb06a21c5c3f97bd8b6f2efa9ed4cd5bfb011ec1101629ba279bb688b500c19c64bbae741b21e00a154c4dee0bfcd9af8f5510ccbcaa3
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA512:40eff8a37c0634f7fdddd6ca5e596b38de15fd10767a34c30bbe49c632816e8f3e1e230678034f578dd5816a94f246fb5dfdf48d644829af13bf28de3225205d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu2.debian.tar.xz' apr-util_1.6.1-5ubuntu2.debian.tar.xz 342740 SHA512:c338ea4b1cb2b92e4774b19c7967fed27d53158f9a2c0bd7c38b4df1819727f54e4af98739422e339a4e4b3554ee35f7b8aa81a9ca8a9861e8c4b1564b74723e
```

### `dpkg` source package: `apr=1.7.0-6ubuntu1`

Binary Packages:

- `libapr1:amd64=1.7.0-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-6ubuntu1.dsc' apr_1.7.0-6ubuntu1.dsc 2049 SHA512:32299e10b010172de80e64e46d3266e18d695acc9c7072a7e2ab28ede8c61d3a41ac8673930157330b6e747646c01fb6aa8bbbe5736d3772ad5d69d534ec74db
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA512:3dc42d5caf17aab16f5c154080f020d5aed761e22db4c5f6506917f6bfd2bf8becfb40af919042bd4ce1077d5de74aa666f5edfba7f275efba78e8893c115148
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA512:19b2b128c7c4cb40db06149c75325013a716c783e28e366c1bacf289fdb5d305e5779d8dc55a63729250ad3338cd4c726e133c788fe53ab3519f1bc8d4da6f90
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-6ubuntu1.debian.tar.xz' apr_1.7.0-6ubuntu1.debian.tar.xz 214960 SHA512:a520ba33119a238df3bbe79832e76504daa9c05b8ee2745ef55ec0c03733f08624751cfe2b028f48de869410f9bdee70aa1574a0125101d6b3d6cb1f5b0f4186
```

### `dpkg` source package: `apt=2.3.9`

Binary Packages:

- `apt=2.3.9`
- `libapt-pkg6.0:amd64=2.3.9`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.3.9
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.3.9.dsc' apt_2.3.9.dsc 2797 SHA512:7d6469bfc071c06d00137f986b66ad3f8948a126c4178bebee810f3479aa7aa3e756a2118356dfeeef49f9c218dc804b3bc6a1c01e3c950475844f3d8631b36c
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.3.9.tar.xz' apt_2.3.9.tar.xz 2204328 SHA512:1e3d65b8d1572ada5007bc5ca25c635580bfc6c03c94a69ab531cc26214fdb8dc78c3ecff0685537b629b714ec059bbe2d7c77a1fc6a406963a58c77e63d4f00
```

### `dpkg` source package: `attr=1:2.4.48-6build2`

Binary Packages:

- `libattr1:amd64=1:2.4.48-6build2`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.48-6build2
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6build2.dsc' attr_2.4.48-6build2.dsc 2482 SHA512:c967873249e32fc258320b0dc6f710d0eb03ac59e6435730087d1ff15654a3fcd777b95e20f42adc4bb8dfd7c5b0316f2133d62c5ca5b3272948591a611baac5
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA512:75f870a0e6e19b8975f3fdceee786fbaff3eadaa9ab9af01996ffa8e50fe5b2bba6e4c22c44a6722d11b55feb9e89895d0151d6811c1d2b475ef4ed145f0c923
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA512:39e5879d4879003ba5e1fcb727f91f7661cede12692ae128110328a6c1c5a1e2f79a1329ee4d065f3cc3e0d3d18423f5b5a5b170b5cb49c6888de90d31dcaf9c
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6build2.debian.tar.xz' attr_2.4.48-6build2.debian.tar.xz 27364 SHA512:c1027696277f687701dd982857aa7b22d0780a546bbc4be6ccafe16b64602dcb1792948278164ddd6470e0bb54808b60c037dfb062be94f659115245023fff76
```

### `dpkg` source package: `audit=1:3.0-2ubuntu2`

Binary Packages:

- `libaudit-common=1:3.0-2ubuntu2`
- `libaudit1:amd64=1:3.0-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0-2ubuntu2.dsc' audit_3.0-2ubuntu2.dsc 2825 SHA512:ac04ed39274cb557031b3fce6a2fb751db3541e6108c601924e002558cce072359e44e7b7dd02680bbff3fd370c765cf05f569217dd40e36338ca76c79a671bf
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.orig.tar.gz' audit_3.0.orig.tar.gz 1109442 SHA512:b82ec73c85a8ebb5108b526673d6fe08cbe0b51376788f3ea6ed5747c4612158462893e719496dffbd723f833f84383a2d1d55fd78a3ed985ecfd19545060c88
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0-2ubuntu2.debian.tar.xz' audit_3.0-2ubuntu2.debian.tar.xz 21304 SHA512:14482acfd7a99f92bb71321f3d71ee6524895cf206112924c115056c55535c004e84b42e2dddd3bbfca4dad5ae65d0b64ba5fe3d5638147a0636bb2a7c3b76ab
```

### `dpkg` source package: `autoconf=2.69-14`

Binary Packages:

- `autoconf=2.69-14`

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
$ apt-get source -qq --print-uris autoconf=2.69-14
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-14.dsc' autoconf_2.69-14.dsc 1624 SHA512:e81aef911ddc8fcf41a40c00365e2bf3f2c97634e87375e36e132026e6be80061af3cddd29536e7cedccf19ae6908b07bfe28730eac5b6ee819057134eb005cd
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA512:995d3e5a8eb1eb37e2b7fae53c6ec7a9b4df997286b7d643344818f94636756b1bf5ff5ea9155e755cb9461149a853dfbf2886fc6bd7132e5afa9c168e306e9b
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-14.debian.tar.xz' autoconf_2.69-14.debian.tar.xz 24512 SHA512:4161c185a8c16634db36a857f3ab0b81bd9156b27fe6a6ce893d09d4551d4f7db59c5556050c1e22b98e832b3c4f1b083c6949b7b4ae7993fecc4d8287231685
```

### `dpkg` source package: `automake-1.16=1:1.16.4-2`

Binary Packages:

- `automake=1:1.16.4-2`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.4-2.dsc' automake-1.16_1.16.4-2.dsc 2561 SHA512:dddf136c00a360f589a46864bc97c7678e8707172f9e70a58475d50672f8211e03cfd99de0c94ac9b058f97cfbf424e13a01b3c93f281d0f852e55b9b5f81a75
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.4.orig.tar.xz' automake-1.16_1.16.4.orig.tar.xz 1599336 SHA512:5a8883657e73b75bfa1ee59ab04af6bf4d43f390ab62fb7a9e8e2ac66159dfe4947b2ac7bc1028afffe6a09d88f388339500e03f6cdfa1226985be45ec033246
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.4.orig.tar.xz.asc' automake-1.16_1.16.4.orig.tar.xz.asc 833 SHA512:ff96d886ba3613b591186bd14fce51ab1f623a2a970f7c62b4901ec5b55ca4ee3b9491f22a2e05eb29826204c3fd4290d2e746fb878b65f31fb0d91fcbb730d8
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.4-2.debian.tar.xz' automake-1.16_1.16.4-2.debian.tar.xz 13044 SHA512:69b95429e0a563c7d50ad70c5d895d513d98b7671c4bec106f12718ba6a9f4c4977a0f20a25673e3118cfbe64d859f926e8128ac7b9c9a6e601b44d65d1e6bae
```

### `dpkg` source package: `autotools-dev=20180224.1+nmu1`

Binary Packages:

- `autotools-dev=20180224.1+nmu1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1%2bnmu1.dsc' autotools-dev_20180224.1+nmu1.dsc 1663 SHA512:936c08ab3dd1ed42fe3f21ce0973168d80e8739557f15dc4d3a9f98dd70426b20f7ca73619c1621d3751997dc9862cd86c1ca9ff61d18697f2c30dd0158f683b
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1%2bnmu1.tar.xz' autotools-dev_20180224.1+nmu1.tar.xz 68356 SHA512:4fe5941597e64a6a69f9ce8f5c537d8a4a1cdfad5aa476d4353976476a2f33917b5391c849dd49bbe8ba3571520b79781b14db597e8b5f02eee3c01490032023
```

### `dpkg` source package: `base-files=11.1ubuntu5`

Binary Packages:

- `base-files=11.1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11.1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11.1ubuntu5.dsc' base-files_11.1ubuntu5.dsc 1623 SHA512:ff71bbc7727e1ca983680ca9fba9494ec5e0d15af25ef28170ac3e7b457924b63d1fc1ebce15ff3d440f68af64956b807a1a6012e0e82cd580e806913fed0586
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11.1ubuntu5.tar.xz' base-files_11.1ubuntu5.tar.xz 81512 SHA512:dea248508fe1a234ae44c06ba02b83007cd0ec31e96399cc9d4f99cfcb7dc0075ccb85fe6ae3aec512a326ec7976f87d8da0ff1cae30266fb950f46a20c523aa
```

### `dpkg` source package: `base-passwd=3.5.51`

Binary Packages:

- `base-passwd=3.5.51`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.51
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.51.dsc' base-passwd_3.5.51.dsc 1757 SHA512:8d022ae0addef596f99a6314d2447f8cf2e474fa55876a403c8a8758024b081c90150e193bc5ab3811a1e94e73bafd190624b8f52d85edbdcb6dbfd9edd61c89
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.51.tar.xz' base-passwd_3.5.51.tar.xz 53980 SHA512:e00e117f7ad25647a8683b8cdb8930371a8d2d670f810808cdcb509e41737f918bc95198912145f654757bd8198d8d31b06dd6cb974b4a4378ebd1cd7954804d
```

### `dpkg` source package: `bash=5.1-3ubuntu2`

Binary Packages:

- `bash=5.1-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-3ubuntu2.dsc' bash_5.1-3ubuntu2.dsc 2426 SHA512:490e12abbd57e284c6145286366b8db083d65c630ef505a41529dd1058708e687b1e5b8a949f3ae00eb7c3a39c7a1285d5be56b4d5c327a2e1cb740fc9da1f21
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA512:95d3acc542231cb893e1347c7d9dd66687f68cd347a0e9e126fde2d14e68c5b5530d1a5866eafa781e88aa013fcf72b4ad56d2e484c2ac7a69bd90bb149a9b86
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-3ubuntu2.debian.tar.xz' bash_5.1-3ubuntu2.debian.tar.xz 98332 SHA512:4cf0ec822763d85c576bf04a768c3de4a2f3bf70be38f05c2348fa8f5fa336816f1d02a82487683abcd7fdc439140521622adab66caf93c00ff74cf8a9002ac1
```

### `dpkg` source package: `binutils=2.37-7ubuntu1`

Binary Packages:

- `binutils=2.37-7ubuntu1`
- `binutils-common:amd64=2.37-7ubuntu1`
- `binutils-x86-64-linux-gnu=2.37-7ubuntu1`
- `libbinutils:amd64=2.37-7ubuntu1`
- `libctf-nobfd0:amd64=2.37-7ubuntu1`
- `libctf0:amd64=2.37-7ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.37-7ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.37-7ubuntu1.dsc' binutils_2.37-7ubuntu1.dsc 8799 SHA512:60f93fbcae568b2914fcb93d1250331645592d727f7c70152ba37d41f17360dfba13437d463dc8870fdc674e07094e51c02b9ebf55271f54e2b22e903e7672c4
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.37.orig.tar.xz' binutils_2.37.orig.tar.xz 22916924 SHA512:5c11aeef6935860a6819ed3a3c93371f052e52b4bdc5033da36037c1544d013b7f12cb8d561ec954fe7469a68f1b66f1a3cd53d5a3af7293635a90d69edd15e7
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.37-7ubuntu1.debian.tar.xz' binutils_2.37-7ubuntu1.debian.tar.xz 175212 SHA512:d0585808225db9c441bac28d3b02a7fb1a970a5a6420bee0749197927b09312ce0dcf410a64c68cc67a689af5a00457083625ba0c8bf9511c69ef0206c13929a
```

### `dpkg` source package: `brotli=1.0.9-2build3`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2build3`
- `libbrotli1:amd64=1.0.9-2build3`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2build3
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build3.dsc' brotli_1.0.9-2build3.dsc 2306 SHA512:a554cd1eebb6db9d7a1271d87c94bbe166055fa8a601da94dfe05bf0a53d52d716cf4ab2934785e31333ae40f6ebf833f044d7d96de64f66daf11fa10c3d1ea8
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build3.debian.tar.xz' brotli_1.0.9-2build3.debian.tar.xz 5700 SHA512:d02187a44c524ac94931a7f09ba9de39005dfd4c31ee3b43531e39c61d0659cfb8cf10704b1c859e9a7b9294b067864624d054a081b362ba1af2e2d584aeaa56
```

### `dpkg` source package: `bzip2=1.0.8-4ubuntu3`

Binary Packages:

- `bzip2=1.0.8-4ubuntu3`
- `libbz2-1.0:amd64=1.0.8-4ubuntu3`
- `libbz2-dev:amd64=1.0.8-4ubuntu3`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-4ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu3.dsc' bzip2_1.0.8-4ubuntu3.dsc 2250 SHA512:71b081f989b574ba90e5cd212c3be0f0b35220eea956be3184fe4408808f8310b1c740626477ddc8d58387e50c56796513588c3d73fc101d8cdba1ab90adc29b
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA512:083f5e675d73f3233c7930ebe20425a533feedeaaa9d8cc86831312a6581cefbe6ed0d08d2fa89be81082f2a5abdabca8b3c080bf97218a1bd59dc118a30b9f3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu3.debian.tar.bz2' bzip2_1.0.8-4ubuntu3.debian.tar.bz2 26650 SHA512:419ccbcac182571cbe52de7ab7c7567a6e86f9402a1dc04bff277fa84ea2ba401e7810b6854b0854e4f1fc55ccabf210c6f8057e11cb7f6e3bc749e4a069f54d
```

### `dpkg` source package: `ca-certificates=20210119ubuntu1`

Binary Packages:

- `ca-certificates=20210119ubuntu1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20210119ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20210119ubuntu1.dsc' ca-certificates_20210119ubuntu1.dsc 1824 SHA512:84266776546f5e19c28efaecd91f159aaa66c0423fcac2c9c4581c72baa4fd63c616a824049f62b2457fff1cad501e6630228080c751056fb93e21af0f9447eb
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20210119ubuntu1.tar.xz' ca-certificates_20210119ubuntu1.tar.xz 233236 SHA512:1f05f7254a42755b045791403a124e9cd0834fef9892beaad1009cd0c99de972cdcf2327fd3f55f6c69329386789613ee3d6d8a1eba9adbd20f38cd8dd77ebad
```

### `dpkg` source package: `cairo=1.16.0-5ubuntu1`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-5ubuntu1`
- `libcairo-script-interpreter2:amd64=1.16.0-5ubuntu1`
- `libcairo2:amd64=1.16.0-5ubuntu1`
- `libcairo2-dev:amd64=1.16.0-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-5ubuntu1.dsc' cairo_1.16.0-5ubuntu1.dsc 2880 SHA512:fdc928fe8d62d73b10fff53046f6c025a3bc10edf38392ab30963e98243add073516279e7616dc62aacfdab8b19b94079083170c564820828809d27366adf495
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA512:9eb27c4cf01c0b8b56f2e15e651f6d4e52c99d0005875546405b64f1132aed12fbf84727273f493d84056a13105e065009d89e94a8bfaf2be2649e232b82377f
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-5ubuntu1.debian.tar.xz' cairo_1.16.0-5ubuntu1.debian.tar.xz 33316 SHA512:6630d9dcb1bbab0ee109d549eab7dfa9223d654eb2feb54f6e2058260093aa3d2e32c82111342ce2c57600a684aed4183dba52388ca552ab9644ca1e80f2377f
```

### `dpkg` source package: `cdebconf=0.256ubuntu3`

Binary Packages:

- `libdebconfclient0:amd64=0.256ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.256ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.256ubuntu3.dsc' cdebconf_0.256ubuntu3.dsc 2941 SHA512:138d03e1d9a6547f14071294d12d415542c7c0c5dec8d6f335a8a979ef74d63bf700de57f4d54873c98ca349f8554e6321e725f32a21becf7cf1e77bb4bcf493
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.256ubuntu3.tar.xz' cdebconf_0.256ubuntu3.tar.xz 279772 SHA512:2141d62f4bba9556eb734c4eb01207a2e818dca748baacc0afe6afbcb526791f0e3ef68081a13288a3b11e6441824343a32ae7daf0367f8ab68cc41a9fe6a8a2
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

### `dpkg` source package: `curl=7.74.0-1.3ubuntu2`

Binary Packages:

- `curl=7.74.0-1.3ubuntu2`
- `libcurl3-gnutls:amd64=7.74.0-1.3ubuntu2`
- `libcurl4:amd64=7.74.0-1.3ubuntu2`
- `libcurl4-openssl-dev:amd64=7.74.0-1.3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.74.0-1.3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.74.0-1.3ubuntu2.dsc' curl_7.74.0-1.3ubuntu2.dsc 2771 SHA512:8284fc92404648c2af19daaf495dacda5d83558b7d624ecc8a0336e018f9989962c70c4631d4fd96c3a499e5c693049d1a40500e5181bed1298c1e03ce4d6e7a
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.74.0.orig.tar.gz' curl_7.74.0.orig.tar.gz 4043409 SHA512:4b61a23463315dce5529aa5f1dc7d21d7876347912c68855c9cfcb01e06492af1510975fafb213c67ac7b9764287767da69043a79376a4be366aa23ace09f163
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.74.0-1.3ubuntu2.debian.tar.xz' curl_7.74.0-1.3ubuntu2.debian.tar.xz 45780 SHA512:d347fa37ab8bc8c434aefa04b9c387948c8e62f90e6a0ebfaf7b499995dad91ca9313abcd4b5893bd904abad6de10ab7e86554935b34953543c9338d1324c7fe
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2.1ubuntu0.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2.1ubuntu0.1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2.1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2.1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg-2.1ubuntu0.1.dsc' cyrus-sasl2_2.1.27+dfsg-2.1ubuntu0.1.dsc 3519 SHA512:267109283bded2e2a9189c2e6556ab9cfd0f84389e29837a36c4bf52c9d282f7fec9ebcd874fce74e0454a6280471a816bcac2a90d44c72e8ab6018474314984
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA512:a795e4362f85a50e223c5456d03526832eb29fdbc9e17a767045f8542638e3f987d382b79b072bcd694bd1a12cbb818cff6c326063ca2bbe05453c1acf7fb8ad
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg-2.1ubuntu0.1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.1ubuntu0.1.debian.tar.xz 102316 SHA512:ca1727e09c2716f476f924880d2e63049a6a743af1f636c0f4df25e4096b5c6da29aaf347ab708bbbd8d7bf38ef3429a7080f96596f6de264d4fd3e532b24c4f
```

### `dpkg` source package: `dash=0.5.11+git20210120+802ebd4-1build1`

Binary Packages:

- `dash=0.5.11+git20210120+802ebd4-1build1`

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
$ apt-get source -qq --print-uris dash=0.5.11+git20210120+802ebd4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210120%2b802ebd4-1build1.dsc' dash_0.5.11+git20210120+802ebd4-1build1.dsc 2169 SHA512:86635d4e25b8c262a90dae33d271cda84b406ec5b4d949691037e9e792756dbdfc8b37362b3afc57b6bfe242db254422b267929a513bf19614d926217dbb7dfd
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210120%2b802ebd4.orig.tar.xz' dash_0.5.11+git20210120+802ebd4.orig.tar.xz 133332 SHA512:076a59f6b0eb4c01ab6f51382fe242079b51b41ee2354140659861b9cb1b19b5a84752509ee4510f834b5e8ba5ccae5cc28f470e5ddea97cef811a02bd9274e7
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210120%2b802ebd4-1build1.debian.tar.xz' dash_0.5.11+git20210120+802ebd4-1build1.debian.tar.xz 42616 SHA512:9febe90890cae798777a903b23c63428709443d58ea3911bf860a16622f0bcf77f2935ea8261dc50272cb589ea13247f5763ea8f4da04cbe679c4ff2838a38e2
```

### `dpkg` source package: `dav1d=0.7.1-3`

Binary Packages:

- `libdav1d4:amd64=0.7.1-3`

Licenses: (parsed from: `/usr/share/doc/libdav1d4/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dav1d=0.7.1-3
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.7.1-3.dsc' dav1d_0.7.1-3.dsc 2307 SHA512:a40ec07062b374aa9829fba2c83fb1f089bfeee7592e7be15c1f7b954de7b7149475f8bde8fb5eacef2b7a84cc0d4bb7dfb487559413017a86e24c858bfe6fd6
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.7.1.orig.tar.xz' dav1d_0.7.1.orig.tar.xz 549068 SHA512:fe7f4a4a547d1239e62025bb40d2f7f97e9fbdfde1d32f9930497801b703a68050ee2fa79793c1cd0c4723678a0736f32431e1b711f63f5de782fe675e5c82de
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.7.1.orig.tar.xz.asc' dav1d_0.7.1.orig.tar.xz.asc 195 SHA512:eebdf9860ca844fd2a79e1dec615d867d861d6906a6f5627932cb2698e9657413c4eae2abf57826a168b1a29bf97fb4b19ea8c7056e0733ceb256237c85f81c5
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.7.1-3.debian.tar.xz' dav1d_0.7.1-3.debian.tar.xz 7768 SHA512:dda9c891b3d3a2bfd0675e9cdb8c02d4d0fd069f25942beb46eb1c6a43af04dda92b1d66b148c4b558e5b49fe561569076979c60854ab38815853e1d6b511672
```

### `dpkg` source package: `db-defaults=1:5.3.21~exp1ubuntu3`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21~exp1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21~exp1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21%7eexp1ubuntu3.dsc' db-defaults_5.3.21~exp1ubuntu3.dsc 2083 SHA512:cab50e812702db81faca5596196eb47d45cab53429cc31d39f7c0e63a050f47c13972e22aadebd88b51d58e4e39a7224acaedad2b1a97a216ec201b6ae76c049
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21%7eexp1ubuntu3.tar.xz' db-defaults_5.3.21~exp1ubuntu3.tar.xz 3088 SHA512:4d4ef4cfa3f47d5d248170d67afd102303f35c4230feb134d30ea1a858c8228971932fb349f4b6ff299af21eae9706513d463ceb3ec0852d005a208895b1fe3a
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8ubuntu1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8ubuntu1`
- `libdb5.3-dev=5.3.28+dfsg1-0.8ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.8ubuntu1.dsc' db5.3_5.3.28+dfsg1-0.8ubuntu1.dsc 3220 SHA512:f7df482fb21791cdf06e966c7c812fa6b9270c3ad86dfe4ff0a08b514c46491cbafeb114aa106f3e66e9839422481f56112c9dff9e764f3cbff032a45547a83c
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA512:50cb87bc3f24065839ee2932e82af032b236b290ebe89983076f503c6c62c5f36ff93d7847a3f68b2b19f35088fbab5d3ac6a34553d07e8148e68e9a3f079a12
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.8ubuntu1.debian.tar.xz' db5.3_5.3.28+dfsg1-0.8ubuntu1.debian.tar.xz 31912 SHA512:83e8592b218688627248d7a41f4432834f1ba7f76605d71bcc550bf63886789fad2ff31bd9a8734afe353a267cc91129933628d160bacb6451e72fde253c787d
```

### `dpkg` source package: `debconf=1.5.77`

Binary Packages:

- `debconf=1.5.77`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.77
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.77.dsc' debconf_1.5.77.dsc 2082 SHA512:238830b883a94448afee10b208be8554a649eab373590d6959f8a9e807503e8f554e6250c537451ba77b57374d555b45e426014732e26c066b94e506bca86b02
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.77.tar.xz' debconf_1.5.77.tar.xz 571412 SHA512:c3cc799ac325c23798db7c424cc35aa2fb223e4bcc7515af1b298e2df4e878c8b4853836f5facf1617aa26b2d46a29fe3ac3653f9bf4cbe9c7c88e30abec1221
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

### `dpkg` source package: `diffutils=1:3.8-0ubuntu1`

Binary Packages:

- `diffutils=1:3.8-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.8-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8-0ubuntu1.dsc' diffutils_3.8-0ubuntu1.dsc 2166 SHA512:d38d7e696fdf2b90f0cf80daa1b3bf51e55323b0ee3837fa544197536f63a0c11b4297398f5528db980d3c847432ba807e0f1b25a446b4a9401ef6df9adeb4ce
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz' diffutils_3.8.orig.tar.xz 1585120 SHA512:279441270987e70d5ecfaf84b6285a4866929c43ec877e50f154a788858d548a8a316f2fc26ad62f7348c8d289cb29a09d06dfadce1806e3d8b4ea88c8b1aa7c
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz.asc' diffutils_3.8.orig.tar.xz.asc 833 SHA512:0464ac89209411993800666b45ff90243d22fbda53bf1d71c6870d565b39cc8d9c54c141b9d297a181ce74ad8fb5313953f416bced179ff7728a52a3e9a4f5a5
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.8-0ubuntu1.debian.tar.xz' diffutils_3.8-0ubuntu1.debian.tar.xz 11616 SHA512:061d016acfa3101c736279afc17b5f206666efc924dfc3fc13ae4a373059686630b49272a2f58b5275db832d5cb0123db5289066471260f6fd0bcab8db08683c
```

### `dpkg` source package: `djvulibre=3.5.28-2build1`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.28-2build1`
- `libdjvulibre-text=3.5.28-2build1`
- `libdjvulibre21:amd64=3.5.28-2build1`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.28-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-2build1.dsc' djvulibre_3.5.28-2build1.dsc 2416 SHA512:e946d78d4316fd31ac3864709e779be8f6b3292341f064ab9829257b6c98265de230358541c837181bf7f87745e877b174ca9419e269c66f8b2b23b26dc65feb
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28.orig.tar.xz' djvulibre_3.5.28.orig.tar.xz 2959024 SHA512:4fdbecd2b7b583ee4211c9cda6638a3a831c883e2552b3c8ad09f69e8734831addc14f590faab8c58d7f9f017b527abccc384f6066e674e341cf43c96db49cb7
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.28-2build1.debian.tar.xz' djvulibre_3.5.28-2build1.debian.tar.xz 17476 SHA512:2edb2008125e18e041ae37c02fff6d4ffeb343be4ada64ac9bdc3aa0f78bf59a41f74a16ad37ee9313a9ac61d06b68b8054aa86a69475ec2fadbc77b74ff2fe9
```

### `dpkg` source package: `dpkg=1.20.9ubuntu2`

Binary Packages:

- `dpkg=1.20.9ubuntu2`
- `dpkg-dev=1.20.9ubuntu2`
- `libdpkg-perl=1.20.9ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.20.9ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.20.9ubuntu2.dsc' dpkg_1.20.9ubuntu2.dsc 2246 SHA512:b7ab9e1e15d0806748131008e7c19f9d0db3ad74a51cbe064eda2bf16c23dffc4a87884c70c0ae1150b074a016ac50d3719b056103cf7a7eb39ecde994b2805e
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.20.9ubuntu2.tar.xz' dpkg_1.20.9ubuntu2.tar.xz 4983396 SHA512:a4204ad7ba67e1be9af1478bc543ad5597d77a72edfdcdad03fbe7ed8a4a6ceb3e410603bc93ef4cd4a08c5054daccef0b22047c32572c880ff896e3fdfce570
```

### `dpkg` source package: `e2fsprogs=1.46.3-1ubuntu3`

Binary Packages:

- `comerr-dev:amd64=2.1-1.46.3-1ubuntu3`
- `e2fsprogs=1.46.3-1ubuntu3`
- `libcom-err2:amd64=1.46.3-1ubuntu3`
- `libext2fs2:amd64=1.46.3-1ubuntu3`
- `libss2:amd64=1.46.3-1ubuntu3`
- `logsave=1.46.3-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.3-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.3-1ubuntu3.dsc' e2fsprogs_1.46.3-1ubuntu3.dsc 3178 SHA512:afbaeb236d77a4f153488c8905dcfdd984c582c12d6f5b264fd3bec82892d073fe126f68952e646b42ac1821feab5811fabd8fdc84c3cf375cd06df46424c203
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.3.orig.tar.gz' e2fsprogs_1.46.3.orig.tar.gz 9510751 SHA512:6c4a5b7900f68671a05f484a83b0f91f803b1df00fd6e059ef6801d9f30be6499d5d8e21923a9cf21335ac2a4cacd21d107ae4d2c546e8997f10ab22a78b266d
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.3.orig.tar.gz.asc' e2fsprogs_1.46.3.orig.tar.gz.asc 488 SHA512:ff495eba93fa39cb9277a5e55a5b8a1b634c9ff47394673d38cef835ffdc5890ead7918bee1006802063f48759babee397565de24f8a587827858a7e339eed10
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.3-1ubuntu3.debian.tar.xz' e2fsprogs_1.46.3-1ubuntu3.debian.tar.xz 85800 SHA512:c4eafbeb9ef671ecc1d85e1fe714fb78a7205a232062860261b0a5a0d3338cd8ad48f76619e0d93c8520d276cdf418c6cc82d4e99b7c5889d97ff35c3b0ae26c
```

### `dpkg` source package: `elfutils=0.185-1build1`

Binary Packages:

- `libelf1:amd64=0.185-1build1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.185-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.185-1build1.dsc' elfutils_0.185-1build1.dsc 3242 SHA512:cf4f81964d842c67a25c6811ea82a9dc61f29af467bd698e95674bd7f5b32855370433c61949ba5d40c969df707ad968e3a55b8d5306c792bfbe3d0502832d89
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.185.orig.tar.bz2' elfutils_0.185.orig.tar.bz2 9187627 SHA512:34de0de1355b11740e036e0fc64f2fc063587c8eb121b19216ee5548d3f0f268d8fc3995176c47190466b9d881007cfa11a9d01e9a50e38af6119492bf8bb47f
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.185-1build1.debian.tar.xz' elfutils_0.185-1build1.debian.tar.xz 37796 SHA512:9ea3b3e01daf6985faa23e42d442c4b46adea63d02026811e1d1caedf759a052ee4a5d49d18403eaed6a6a707d79c83d776a2e017b7603f2f5b7658369ca338d
```

### `dpkg` source package: `expat=2.4.1-2ubuntu0.3`

Binary Packages:

- `libexpat1:amd64=2.4.1-2ubuntu0.3`
- `libexpat1-dev:amd64=2.4.1-2ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.4.1-2ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.1-2ubuntu0.3.dsc' expat_2.4.1-2ubuntu0.3.dsc 2096 SHA512:7f8c7c2d36ea20d941fc30b0f8029239716c95a26317f805ff0d0a8d503a2d61d2b9ba3ca2e1850ed0d1cce045341874d12d68104057cd0074bf5bea5ad85fe5
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.1.orig.tar.gz' expat_2.4.1.orig.tar.gz 8307804 SHA512:1f08861e9b766fdbbc40159404a3fe1a86451d635ef81874fa3492845eda83ac2dc6a0272525891d396b70c9a9254c2f6c907fe4abb2f8a533ccd3f52dae9d5a
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.1-2ubuntu0.3.debian.tar.xz' expat_2.4.1-2ubuntu0.3.debian.tar.xz 26116 SHA512:fd58c4788f11c5c670e3ca91784dd0a672905a96bbf3877132b33bcb0fefea8028c600deecd698c4019771ee6a4542605d78e1fd5beda795e5ae835b10210195
```

### `dpkg` source package: `fftw3=3.3.8-2ubuntu7`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2ubuntu7`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2ubuntu7
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu7.dsc' fftw3_3.3.8-2ubuntu7.dsc 3039 SHA512:70ce862377db4c24ffb74fbed69f46b0fa0a8fd6cf8dfca0242f815d4bf289e0a2658cf83ca3d123914e5f570c14b39597edbcd324e10871a587655a3f2f4fec
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA512:ab918b742a7c7dcb56390a0a0014f517a6dff9a2e4b4591060deeb2c652bf3c6868aa74559a422a276b853289b4b701bdcbd3d4d8c08943acf29167a7be81a38
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu7.debian.tar.xz' fftw3_3.3.8-2ubuntu7.debian.tar.xz 14284 SHA512:19a14bdf1b17e6f0c6b16b6e1bd8ce6ca711d5d2612802c1360681b0bc3c4f3d8843bc12834c1f35ee29146f0412a12e48b57b6a41bc754f23428d780cc686cc
```

### `dpkg` source package: `file=1:5.39-3`

Binary Packages:

- `file=1:5.39-3`
- `libmagic-mgc=1:5.39-3`
- `libmagic1:amd64=1:5.39-3`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.39-3
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39-3.dsc' file_5.39-3.dsc 2237 SHA512:79399bd3c0c70121d19e737c4323d247085a796ce76205246678abd109a6a28b564d8bd85e2b0e2c40a8b047b12ccfcb31346b5ebbbc91ebd36903684a096fd2
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39.orig.tar.gz' file_5.39.orig.tar.gz 954266 SHA512:9cf1a7b769c56eb6f5b25c66ce85fa1300128396e445b2e53dbbd8951e5da973a7a07c4ef9f7ebd1fe945d47bdaf2cd9ef09bd2be6c217a0bcb907d9449835e6
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39.orig.tar.gz.asc' file_5.39.orig.tar.gz.asc 169 SHA512:0b9654e3576862ff0214e67ad023ccc445a8a4a7f40bccc39ec1b332c9952bdb5ed4c324cc36da36c2dce6cb35f3bbf29069c19c574b8705724c7c7d0c562caf
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.39-3.debian.tar.xz' file_5.39-3.debian.tar.xz 34420 SHA512:1a664d162fb5827c24ec8a2f6909bb33803148b5b25f6d372784e501636c39f5758687703878bf83fd45045e59f6a862f9bebadf5633caebc0945fe4e85edeac
```

### `dpkg` source package: `findutils=4.8.0-1ubuntu2`

Binary Packages:

- `findutils=4.8.0-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.8.0-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0-1ubuntu2.dsc' findutils_4.8.0-1ubuntu2.dsc 2434 SHA512:49da1d80963853764bc5aef9b7bad25b339e145454e2fc798855e627b70aff77d8f041c4f2aa2cac735844e75ad6e7c78c4b731e71fd9d50033a679106931e9b
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz' findutils_4.8.0.orig.tar.xz 1983096 SHA512:eaa2da304dbeb2cd659b9210ac37da1bde4cd665c12a818eca98541c5ed5cba1050641fc0c39c0a446a5a7a87a8d654df0e0e6b0cee21752ea485188c9f1071e
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz.asc' findutils_4.8.0.orig.tar.xz.asc 488 SHA512:e6ea8bd9a58ac4f787a9cc7dad9f75fab9e0623e7cda463bef60651c9319574ac7c8ba06f7d33cbead0ecb8788db71eb39f50550deb066d6d6baa625b0374a45
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0-1ubuntu2.debian.tar.xz' findutils_4.8.0-1ubuntu2.debian.tar.xz 27640 SHA512:db4d1cb055051a784d394d3f3559d31bdec15252b3b6bbb8f851ef5cc25da214002a582389ec9fdb8a7713068919025cf6bbe17c9b60f07940fe93dfd59e4d3e
```

### `dpkg` source package: `fontconfig=2.13.1-4.2ubuntu3`

Binary Packages:

- `fontconfig=2.13.1-4.2ubuntu3`
- `fontconfig-config=2.13.1-4.2ubuntu3`
- `libfontconfig-dev:amd64=2.13.1-4.2ubuntu3`
- `libfontconfig1:amd64=2.13.1-4.2ubuntu3`
- `libfontconfig1-dev:amd64=2.13.1-4.2ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-4.2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-4.2ubuntu3.dsc' fontconfig_2.13.1-4.2ubuntu3.dsc 2819 SHA512:ce75bef0de0ce98bf41ae6161352a2b107ce29cb2ef5a06640e03ddc75d91c9ffccc920fa1bb7bd289f44a3705920da0ac2aa35168ea5d92906f7942c29776a8
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA512:f97f2a9db294fd72d416a7d76dd7db5934ade2cf76903764b09e7decc33e0e2eed1a1d35c5f1c7fd9ea39e2c7653b9e65365f0c6205e047e95e38ba5000dd100
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-4.2ubuntu3.debian.tar.xz' fontconfig_2.13.1-4.2ubuntu3.debian.tar.xz 28012 SHA512:73b0c8fc2fbbf900af0f504749105b25df74226deb56b9022edc38412c4bc5ee59b2075677f7ae8e19affc7b81616e0b54dc5c335d7ce97f9d8f230703d3a319
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

### `dpkg` source package: `freetype=2.10.4+dfsg-1build1`

Binary Packages:

- `libfreetype-dev:amd64=2.10.4+dfsg-1build1`
- `libfreetype6:amd64=2.10.4+dfsg-1build1`
- `libfreetype6-dev:amd64=2.10.4+dfsg-1build1`

Licenses: (parsed from: `/usr/share/doc/libfreetype-dev/copyright`, `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `FSFAP`
- `FSFUL`
- `FSFULLR`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `OFL-1.1`
- `OpenGroup-BSD-like`
- `Permissive`
- `Public-Domain`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.10.4+dfsg-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4%2bdfsg-1build1.dsc' freetype_2.10.4+dfsg-1build1.dsc 3742 SHA512:36e1948dc2ebfd28e885d95b4892c0302928ee67aba3eccf7dc3dcdd5e4a9fade6b0f4924056b2bf778eca37b47c247e76ef41ef99562d3fb71707b98776bad2
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2demos.tar.xz' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz 236712 SHA512:d2afc19e5fabbee5205fcc992f6c19bab03485b7af4f55bb2d2dd0a4a9492a3f593540862ca116b54cf161b240d7966cb31a9793578d164fc418449e339e2fa8
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2demos.tar.xz.asc 195 SHA512:6b297a67afd11d21e705f6bfd82ffefec2a3a424a6a1bc5b24b80f037337f888677d7af3bab5d0be13d779162de8d4ae8f30f7fd978de6f6693567f4899980bf
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2docs.tar.xz' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz 2079084 SHA512:171da6c6a172869e9bec0da67cb1abdb0fdb124870f13b751b4e9b1b5e342fb2af38cb606db1c3dcf18076a077e694b7b8dd055dd7f4ab49afe7e1d61b4f9ba8
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.10.4+dfsg.orig-ft2docs.tar.xz.asc 195 SHA512:c42ed2aea76eee7f4e775e26276fd260249b672c06ae0c73f378bc0ac7425e36683c4f8b4a8875d5f31f08d9f8e3a7ba0b427d9a5308c8aa90718c42edf13c52
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4%2bdfsg.orig.tar.xz' freetype_2.10.4+dfsg.orig.tar.xz 2259340 SHA512:4d02111df4eb932cb1fd4890e6487a0a6830d98dbf35a6377b0fb2b66af89b06a449e149950271adbbff7411e2949e5a2a4ad6cd376e06287b5892dbe3bce3dc
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.4%2bdfsg-1build1.debian.tar.xz' freetype_2.10.4+dfsg-1build1.debian.tar.xz 116708 SHA512:4abd460134647a3114268a72ea04a9c50e78f2245be6822d4faf4fc5ca2e76f94af62acb828fbfdb1fdb0d424575ba4dfbf70bd24c765678901851fd5f8f61e3
```

### `dpkg` source package: `fribidi=1.0.8-2ubuntu2`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2ubuntu2.dsc' fribidi_1.0.8-2ubuntu2.dsc 2419 SHA512:ef9c6ae02bdd4eea004dd889ed162265510bd9596b213d5f414838b0d145f536310e950827e12074e62ef35c6026f0557b58c0f75e41a67dad8a5f30a79ad051
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA512:d66b1524b26d227fd6a628f438efb875c023ae3be708acaaad11f1f62d0902de0a5f57124458291ef2b0fcd89356c52ab8ae5559b0b5a93fa435b92f1d098ba2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2ubuntu2.debian.tar.xz' fribidi_1.0.8-2ubuntu2.debian.tar.xz 9292 SHA512:b7033960e87189e9e20497938acc2040e16a5c14b17f08227632d7a5c7d75fa2ad699a10c53f0339972d57bb5a7116a4b45fa5c73d18ba26d4220ce03be80b93
```

### `dpkg` source package: `gcc-11=11.2.0-7ubuntu2`

Binary Packages:

- `cpp-11=11.2.0-7ubuntu2`
- `g++-11=11.2.0-7ubuntu2`
- `gcc-11=11.2.0-7ubuntu2`
- `gcc-11-base:amd64=11.2.0-7ubuntu2`
- `libasan6:amd64=11.2.0-7ubuntu2`
- `libatomic1:amd64=11.2.0-7ubuntu2`
- `libcc1-0:amd64=11.2.0-7ubuntu2`
- `libgcc-11-dev:amd64=11.2.0-7ubuntu2`
- `libgcc-s1:amd64=11.2.0-7ubuntu2`
- `libgomp1:amd64=11.2.0-7ubuntu2`
- `libitm1:amd64=11.2.0-7ubuntu2`
- `liblsan0:amd64=11.2.0-7ubuntu2`
- `libquadmath0:amd64=11.2.0-7ubuntu2`
- `libstdc++-11-dev:amd64=11.2.0-7ubuntu2`
- `libstdc++6:amd64=11.2.0-7ubuntu2`
- `libtsan0:amd64=11.2.0-7ubuntu2`
- `libubsan1:amd64=11.2.0-7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/cpp-11/copyright`, `/usr/share/doc/g++-11/copyright`, `/usr/share/doc/gcc-11/copyright`, `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-11-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-11-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.2.0-7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-7ubuntu2.dsc' gcc-11_11.2.0-7ubuntu2.dsc 27849 SHA512:30f167f0eed6b506c87d4a6502fd895a4acc72aa1c720fdea764e42b60afb11a7edb8312b5e2854e56abe182871d42b75bde1d4e1034325a99a33f0acf97c126
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0.orig.tar.gz' gcc-11_11.2.0.orig.tar.gz 87861992 SHA512:64e4634769a62faa0adbfe99e5e590dd9efc1facac20a7dd71ab9f1d675e7df80678cbdc75c966e08ccf91dbc1e1a681d8e3227d0026ffcb5f46bdc96acaace8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-7ubuntu2.debian.tar.xz' gcc-11_11.2.0-7ubuntu2.debian.tar.xz 1818060 SHA512:d42e106c0f3238ff443d497796e8c1148c80923e32a42d75c40deec8c5a877cc062c58e62fb2a096bb43d67c694d4954486c371f380474dacbd86373b6fe1403
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

### `dpkg` source package: `gdbm=1.19-2`

Binary Packages:

- `libgdbm-compat4:amd64=1.19-2`
- `libgdbm-dev:amd64=1.19-2`
- `libgdbm6:amd64=1.19-2`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

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

### `dpkg` source package: `gdk-pixbuf=2.42.6+dfsg-1build2`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.42.6+dfsg-1build2`
- `libgdk-pixbuf-2.0-0:amd64=2.42.6+dfsg-1build2`
- `libgdk-pixbuf-2.0-dev:amd64=2.42.6+dfsg-1build2`
- `libgdk-pixbuf2.0-bin=2.42.6+dfsg-1build2`
- `libgdk-pixbuf2.0-common=2.42.6+dfsg-1build2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf-2.0-dev/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `Apache-2.0`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `CC0-1.0,`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3.0`
- `GPL-3.0+`
- `GPL-3.0+,`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.42.6+dfsg-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6%2bdfsg-1build2.dsc' gdk-pixbuf_2.42.6+dfsg-1build2.dsc 3308 SHA512:3b8e4214bab328ad3f3a4fdef346d2c212013aa61e1fc968c6325b3e7b8dc4dbccc6cbd72cc0dd267be10a804343f57f5665fe2f1ed41395aff739b107f81b93
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6%2bdfsg.orig.tar.xz' gdk-pixbuf_2.42.6+dfsg.orig.tar.xz 6527432 SHA512:e3c9479a4ae2d1ffe45a908ad4b693305ebfa55ef3310a241f65bbc36faa880ff696166e317c9022dca569443a7e1a86e35dfc39f298f00ab5e9c7e0c5471e7b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6%2bdfsg-1build2.debian.tar.xz' gdk-pixbuf_2.42.6+dfsg-1build2.debian.tar.xz 29768 SHA512:8f7f586289e05aff8502413171d5e5a1d9746c25c75279b8781cfd932e05010b79c22bb47be71baaa191e8536d65aae0058de45f5ac03f10b13418296cc9c666
```

### `dpkg` source package: `git=1:2.32.0-1ubuntu1`

Binary Packages:

- `git=1:2.32.0-1ubuntu1`
- `git-man=1:2.32.0-1ubuntu1`

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

Source:

```console
$ apt-get source -qq --print-uris git=1:2.32.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.32.0-1ubuntu1.dsc' git_2.32.0-1ubuntu1.dsc 2940 SHA512:c1f75086f13cdd318298961ea6099026f9dd99d382b5ca8eaa5dda4244bb93c5f4667ad7e3b22438548eb917f8c5bc857e0504ccd64bb6457d3ec25324c46d91
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.32.0.orig.tar.xz' git_2.32.0.orig.tar.xz 6551348 SHA512:1ab3e7022ccee411d14a7da5c37d6259ef5c0f85ebed8f49698e25c65cbc7a46f8096919fcb6568360bfe284dd7475b596eee1a167db966096255a405853837c
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.32.0-1ubuntu1.debian.tar.xz' git_2.32.0-1ubuntu1.debian.tar.xz 685712 SHA512:be28129901a3d5f6e26e92c9051acefb42ea3058ae94abf3249f4166d7acb793823a12793958d0d8434cf54086e2b5936e9410ccc655f7f42d019120e50dd3f0
```

### `dpkg` source package: `glib2.0=2.68.4-1ubuntu1`

Binary Packages:

- `libglib2.0-0:amd64=2.68.4-1ubuntu1`
- `libglib2.0-bin=2.68.4-1ubuntu1`
- `libglib2.0-data=2.68.4-1ubuntu1`
- `libglib2.0-dev:amd64=2.68.4-1ubuntu1`
- `libglib2.0-dev-bin=2.68.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.68.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.68.4-1ubuntu1.dsc' glib2.0_2.68.4-1ubuntu1.dsc 3508 SHA512:f379fbea280aee3a8ff2930e9bdb19d061fcc7e560db3d99fc63dbf6798939e84f6a42f9d5d6f430dffe66bd4b84cf9cb3d535d0b11de64a96eaa8f5e8721d80
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.68.4.orig.tar.xz' glib2.0_2.68.4.orig.tar.xz 4945212 SHA512:be17d79b41d17fd2b144184d6e793180667b7d9ba299215ea6d4948b4c05f6d888b4868c48643e25935a34ee2f85ee1d03e53325151b7a61819437cbd3c84b10
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.68.4-1ubuntu1.debian.tar.xz' glib2.0_2.68.4-1ubuntu1.debian.tar.xz 101576 SHA512:3693e8619bc31e9f7a87c9f037c9291988329c27919deac9b95490fcca7acabbb63072c2dd7d63741645624d1d4578c830366aa6efc0c0d5a50de27f8057f40a
```

### `dpkg` source package: `glibc=2.34-0ubuntu3.2`

Binary Packages:

- `libc-bin=2.34-0ubuntu3.2`
- `libc-dev-bin=2.34-0ubuntu3.2`
- `libc6:amd64=2.34-0ubuntu3.2`
- `libc6-dev:amd64=2.34-0ubuntu3.2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.34-0ubuntu3.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34-0ubuntu3.2.dsc' glibc_2.34-0ubuntu3.2.dsc 8965 SHA512:029f0b6c9a5b343b6d1dc73a5089fea35ea3d289ee194709904e332f4daaa3433766d1f5f62bfb65ce1d8766f3d505d12900ef641c3df605726a69755b0e20e0
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34.orig.tar.xz' glibc_2.34.orig.tar.xz 17301232 SHA512:15252affd9ef4523a8001db16d497f4fdcb3ddf4cde7fe80e075df0bd3cc6524dc29fbe20229dbf5f97af580556e6b1fac0de321a5fe25322bc3e72f93beb624
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34.orig.tar.xz.asc' glibc_2.34.orig.tar.xz.asc 833 SHA512:5b92e315d81a0a157f15b8ac29acddbf4669b51a72483bba4b1769db78986ec9814b23be3d7ac3779cefb0a38070af7ecb37dc1667e1cb3ede8c34cb1ca5d7f3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34-0ubuntu3.2.debian.tar.xz' glibc_2.34-0ubuntu3.2.debian.tar.xz 890968 SHA512:644d47301d331e898de1285aaa9bbb28d710ee1653d9a1037d1e75eba3b42917640947e9e5d169e50307220b27f13eea7edbb69f527f64a08b2bc9d472a7915b
```

### `dpkg` source package: `gmp=2:6.2.1+dfsg-1ubuntu2`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.1+dfsg-1ubuntu2`
- `libgmp10:amd64=2:6.2.1+dfsg-1ubuntu2`
- `libgmpxx4ldbl:amd64=2:6.2.1+dfsg-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg-1ubuntu2.dsc' gmp_6.2.1+dfsg-1ubuntu2.dsc 2256 SHA512:2fd6a3a95e4bfc997d01a5af7e1b19d737538960e73d78c75c53e233afd3967a50335abde6024848a60d07c5fae53b27d7bcf8a0c8acddac144e403cbd5d08d6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA512:801948b7dcf592959ea387a86bee34dfb4e02c5e93815a785fc46174899ba22129853a3e34109a6df86048a144765c5f39e65fddfcecba879cc60da62f32fea0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1%2bdfsg-1ubuntu2.debian.tar.xz' gmp_6.2.1+dfsg-1ubuntu2.debian.tar.xz 43744 SHA512:32ee0629d2769fe687dbd3731e546f115bd1d4f644dcbc9392b0addc58982758126c08c51ab6a7c46f047d6f4a0a42632f216704ecf0d5f0a6670f0a6c8bd8b2
```

### `dpkg` source package: `gnupg2=2.2.20-1ubuntu4`

Binary Packages:

- `dirmngr=2.2.20-1ubuntu4`
- `gnupg=2.2.20-1ubuntu4`
- `gnupg-l10n=2.2.20-1ubuntu4`
- `gnupg-utils=2.2.20-1ubuntu4`
- `gpg=2.2.20-1ubuntu4`
- `gpg-agent=2.2.20-1ubuntu4`
- `gpg-wks-client=2.2.20-1ubuntu4`
- `gpg-wks-server=2.2.20-1ubuntu4`
- `gpgconf=2.2.20-1ubuntu4`
- `gpgsm=2.2.20-1ubuntu4`
- `gpgv=2.2.20-1ubuntu4`

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
$ apt-get source -qq --print-uris gnupg2=2.2.20-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu4.dsc' gnupg2_2.2.20-1ubuntu4.dsc 3934 SHA512:f763596c0b9c580f6df6766e5e564ca342328836f5efdd34bea6943a48d15d7f34e102d638bd1968e6d2cc53e8466b072e46e49596d0c93738eae36c50731b6d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2' gnupg2_2.2.20.orig.tar.bz2 6786913 SHA512:3e69f102366ec3415f439ab81aae2458182fa1a18dfb86565b1d9dc638f3fc4c179a5947f0042b7c5a813345676285a662793664a1803ea9ad8328f0548e0edc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2.asc' gnupg2_2.2.20.orig.tar.bz2.asc 1357 SHA512:0972788af253f84959ab3142e3d4bf025b7e7077377574e69851ae3d37cbf296211fdf50cd77fe47f844bc3383489ff88cf35186d2f72cb0adc84cdfe77bfd26
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu4.debian.tar.xz' gnupg2_2.2.20-1ubuntu4.debian.tar.xz 64908 SHA512:5d7d8f7e75d3ae759103dbd104a16fa0125248bd55f68f720d8bf9262328c87d6236b1f262c1036b0375e659dace152a66f3ee191864fdd4d276e2ffe0842e76
```

### `dpkg` source package: `gnutls28=3.7.1-5ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.1-5ubuntu1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.1-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1-5ubuntu1.dsc' gnutls28_3.7.1-5ubuntu1.dsc 3594 SHA512:2debb4b8eb36994b13e9e97fb22c2d5354527438ac1b60acea715e44e0c60c62874af2f3c4fc3a98a83c521e6f6249607b8b1ddcb0a39b094d89517211a7e31d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1.orig.tar.xz' gnutls28_3.7.1.orig.tar.xz 6038388 SHA512:0fe801f03676c3bd970387f94578c8be7ba6030904989e7d21dffdc726209bab44c8096fbcb6d51fed2de239537bd00df2338ee9c8d984a1c386826b91062a95
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1.orig.tar.xz.asc' gnutls28_3.7.1.orig.tar.xz.asc 854 SHA512:72101722be460c3092ff602dbf7246e81172a8aa2f7a9eba73a76536d00798cf58ab8a6d90b79cdb29f4c5f65ca0129d2f4e22e46dd66f4cee9e4a559b72d546
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1-5ubuntu1.debian.tar.xz' gnutls28_3.7.1-5ubuntu1.debian.tar.xz 90612 SHA512:893b3b5d9237825fc1878ef4e4707a0e1cba41795ae0ba2ac126ec96ca0dd269ce7b75f7b944e01b7be00a41d68e5b29f22218295a9ee8429c0fb1f18a74e0b5
```

### `dpkg` source package: `gobject-introspection=1.68.0-1build2`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.68.0-1build2`
- `gir1.2-glib-2.0:amd64=1.68.0-1build2`
- `libgirepository-1.0-1:amd64=1.68.0-1build2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.68.0-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.68.0-1build2.dsc' gobject-introspection_1.68.0-1build2.dsc 3004 SHA512:e813f7e287d7abf4c4c7aeb965fd34848981fb9543a77418aa7291864e89ca30a2352c04495b44db25078b1d0f382e3d1aac89825cc0e484ea424dc7a64aeacf
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.68.0.orig.tar.xz' gobject-introspection_1.68.0.orig.tar.xz 1019732 SHA512:d2e64c119aa500b624a57baa2cebe9126ab100003d98b771f4fb51cf92748635de352997f702f40656f7c665f3dfedfbfa19912cc7a2d039d254555243bbc381
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.68.0-1build2.debian.tar.xz' gobject-introspection_1.68.0-1build2.debian.tar.xz 24372 SHA512:3ef94acc05e0eea01396da2b50ab30f9aecc18f7aa656d024f2b3328232ec38f7f67649a3106d34671ecb477b0cd4e66daff6b2bf47edcff2fed5f5e6f9aaacb
```

### `dpkg` source package: `graphite2=1.3.14-1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.14-1`

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
$ apt-get source -qq --print-uris graphite2=1.3.14-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1.dsc' graphite2_1.3.14-1.dsc 2608 SHA512:a1f4621189784463b7b0cfaa9c2615087746f077db6d90909866c30b14789a4e8847ce00c37345a5ce02177d2eba1a2720688edf516e38f099bafbdf050fb35f
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14.orig.tar.gz' graphite2_1.3.14.orig.tar.gz 6629829 SHA512:49d127964d3f5c9403c7aecbfb5b18f32f25fe4919a81c49e0534e7123fe845423e16b0b8c8baaae21162b1150ab3e0f1c22c344e07d4364b6b8473c40a0822c
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1.debian.tar.xz' graphite2_1.3.14-1.debian.tar.xz 12068 SHA512:4f9fab5bf556fbfe6ad80560d0e8d48bd0c38d5996beb938f8ed7cdad44b230881eb3a32dd9e7352fca2b185005ecdc2d3915727ef4f40047818f2bac1b58342
```

### `dpkg` source package: `grep=3.7-0ubuntu1`

Binary Packages:

- `grep=3.7-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.7-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7-0ubuntu1.dsc' grep_3.7-0ubuntu1.dsc 2353 SHA512:9667558c9b26155437a163738c76b2c96e5156b0ed4ec4089b91fa1ad741c8842a6e0584f522d1472c4e069c5ca9512d6f75497a100d492b29b64011c4e127c5
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7.orig.tar.xz' grep_3.7.orig.tar.xz 1641196 SHA512:e9e45dcd40af8367f819f2b93c5e1b4e98a251a9aa251841fa67a875380fae52cfa27c68c6dbdd6a4dde1b1017ee0f6b9833ef6dd6e419d32d71b6df5e972b82
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7.orig.tar.xz.asc' grep_3.7.orig.tar.xz.asc 833 SHA512:9db28883b696fbbb0fad32f4ecd168954dc475d5f0a8f2b4f960ff615ef7dd8348a7caaee85a96287824472a29485ff921af121c582083ca5ad5c30960f99cf4
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7-0ubuntu1.debian.tar.xz' grep_3.7-0ubuntu1.debian.tar.xz 18028 SHA512:b341746a61cc5569b635d2fd39b91b015efaec2f8bddc14c4a51eb66743bd4b380e15dd7435cedc442bc3313620466e5c9a94fa7ff15d29ae1fa538485d1b789
```

### `dpkg` source package: `gzip=1.10-4ubuntu1`

Binary Packages:

- `gzip=1.10-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-4ubuntu1.dsc' gzip_1.10-4ubuntu1.dsc 2306 SHA512:61952245d44a37b3061df1687576c94093b7f31849be3d6713a23921e1955b57a97b9d347c85824ef6216ad46fff4ff6149cf44371310fec2c2c628564121a16
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA512:7939043e74554ced0c1c05d354ab4eb36cd6dce89ad79d02ccdc5ed6b7ee390759689b2d47c07227b9b44a62851afe7c76c4cae9f92527d999f3f1b4df1cccff
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz.asc' gzip_1.10.orig.tar.gz.asc 833 SHA512:74727fb3a8b64f81b4dd2d941fa750a789c482d7ae604d0ecfbe5ec623780efc7c5f0e51d65e7b99c2f097c5cd6585cc3a0f1b31abb03306156e0d410d9f0186
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-4ubuntu1.debian.tar.xz' gzip_1.10-4ubuntu1.debian.tar.xz 34396 SHA512:2bf92e71162a3e10918471f9fd39cef5a611fd81786f3ba399029af1308fc2928b2ca7f9af4ab974e33e9c1c8e6a401810a3c9bd4411964d28530e1b1a678624
```

### `dpkg` source package: `harfbuzz=2.7.4-1ubuntu1`

Binary Packages:

- `libharfbuzz0b:amd64=2.7.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.7.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu1.dsc' harfbuzz_2.7.4-1ubuntu1.dsc 2872 SHA512:a3fa975a6c42b38593fe49fa0436d889942679adf1c3c7ab1665d3172624186b68075bb16c1e6c06589d6a2f15d5f2ddc3442ccdc940135f4122f92a63673140
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4.orig.tar.xz' harfbuzz_2.7.4.orig.tar.xz 9532468 SHA512:d2af6a768c397c664f654cf36140e7b5696b3b983f637454604570c348247f7ffea135048d9b02cf6593cbde728567e31bf82a39df5ff38d680c78dff24d4cf0
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu1.debian.tar.xz' harfbuzz_2.7.4-1ubuntu1.debian.tar.xz 11004 SHA512:b7df6e12585a38c7ad336eaff47ebec568b608c9e9677631f49956b923fc098d4565cd2703e92b83903f3002a4b55d18c8f3c8da289d3f22878d451557616e9b
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

### `dpkg` source package: `hostname=3.23ubuntu1`

Binary Packages:

- `hostname=3.23ubuntu1`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23ubuntu1.dsc' hostname_3.23ubuntu1.dsc 1455 SHA512:ce06d5d3d7b98e167b871c8c989ca31432107b0139b3f117b330c69dd9d2060414236dc51dee47318a48fd34f77a66d2fc9cc4a8220fd028c0c05bd42f4f37f8
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23ubuntu1.tar.gz' hostname_3.23ubuntu1.tar.gz 13754 SHA512:80eaf46a43c48dfc0b31dbebeddd4be6a00404db3243c6d1e6483de567da88015c26298c004f0d757ab701ad566b950a87cc30f9acb06e82ee20217f5e9b5150
```

### `dpkg` source package: `icu=67.1-7ubuntu1`

Binary Packages:

- `icu-devtools=67.1-7ubuntu1`
- `libicu-dev:amd64=67.1-7ubuntu1`
- `libicu67:amd64=67.1-7ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=67.1-7ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1-7ubuntu1.dsc' icu_67.1-7ubuntu1.dsc 2343 SHA512:e8b738ab57cb67b03c1399aedc008135025b11b4c7100a2f635b0986f4c540ffd9cc512412d1a289b84078c9f75a6e669f9911d04c4ad86be052719a9a0a449c
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1.orig.tar.gz' icu_67.1.orig.tar.gz 24518055 SHA512:4779f1ce1ca7976f6fad6768853ea8c540da54d11509e3b6cfd864a04b5f2db1c3d4b546387f91ad02fb90804525bc37d2543173f0d705d6ca11dc6f2b7640a8
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1.orig.tar.gz.asc' icu_67.1.orig.tar.gz.asc 833 SHA512:3d731cfbb200f150f6fda348a100226ad7a56dea428a46745bcaf5be3ad6a0bf3ef685acfdf759f51a53704d78b4a02ee90ecbf50f2e18d14fcef5050afd8f54
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1-7ubuntu1.debian.tar.xz' icu_67.1-7ubuntu1.debian.tar.xz 30804 SHA512:12429339abc878f8376691eb964a4127bc65357b67f6336f992ecc524cfd392ddf3642398bfc49f791e0f101e79aa4ebe94dd92b6dc6f66eab43f3eee1510da3
```

### `dpkg` source package: `ilmbase=2.5.4-1`

Binary Packages:

- `libilmbase-dev:amd64=2.5.4-1`
- `libilmbase25:amd64=2.5.4-1`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase25/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.5.4-1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.4-1.dsc' ilmbase_2.5.4-1.dsc 2468 SHA512:35bcbd451aca19ff125d4969cbc282abc8b803e1b1770381d6ba1e6834a583dd66926373a04e1583cf488c9dc9712179cb1f5a9b4087385073f21d8bd5b3e906
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.4.orig.tar.gz' ilmbase_2.5.4.orig.tar.gz 27535491 SHA512:f0fe305987981e0c7e5a854367702585e4935ad37b0e8c10dcbc7468ae3a6d34bf963ec9ec75cc3abe4cf00e359644476b643978d0289dca46c9785a25d3f7f1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.4.orig.tar.gz.asc' ilmbase_2.5.4.orig.tar.gz.asc 287 SHA512:9b3978e44b531429aba42b9cc4969a470898d9d74652e3809edb0273ba9b127c471aec6570b5d352be738f59810091c0df2c70d39c16d2c32833d173b270f72c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.4-1.debian.tar.xz' ilmbase_2.5.4-1.debian.tar.xz 14348 SHA512:b0f49228a3cda6c27026311d25bd47740123cb37e7b0816d86edc7303d563c0b393f29605cfedfee416a1a471647dcaf4fc1b7517d003015023bbaa5ff961b7d
```

### `dpkg` source package: `imagemagick=8:6.9.11.60+dfsg-1ubuntu1`

Binary Packages:

- `imagemagick=8:6.9.11.60+dfsg-1ubuntu1`
- `imagemagick-6-common=8:6.9.11.60+dfsg-1ubuntu1`
- `imagemagick-6.q16=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickcore-6-arch-config:amd64=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickcore-6-headers=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickcore-6.q16-6:amd64=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickcore-6.q16-dev:amd64=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickcore-dev=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickwand-6-headers=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickwand-6.q16-6:amd64=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickwand-6.q16-dev:amd64=8:6.9.11.60+dfsg-1ubuntu1`
- `libmagickwand-dev=8:6.9.11.60+dfsg-1ubuntu1`

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
$ apt-get source -qq --print-uris imagemagick=8:6.9.11.60+dfsg-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1ubuntu1.dsc' imagemagick_6.9.11.60+dfsg-1ubuntu1.dsc 5211 SHA512:4ed45fbd769052e7251416f2239da7f61bfc2066ec52732d40b5ff2360b3043d28836446398f3cd3a118bbc4a30946f2b4427c8b1fd56bb146952fcc76284259
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg.orig.tar.xz' imagemagick_6.9.11.60+dfsg.orig.tar.xz 9395144 SHA512:345a23eda96516fc7a213bd4a322bca4c8b690efe40ff7b498a448f8cedd7f0d600fae2cb6fff45bc995779a90d8c04b58288273eee97833ddebb4f9f2a3d14c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/imagemagick/imagemagick_6.9.11.60%2bdfsg-1ubuntu1.debian.tar.xz' imagemagick_6.9.11.60+dfsg-1ubuntu1.debian.tar.xz 265424 SHA512:b4f530361392251d22400de1fdb3c5d4096f697d763c765aa8c1b5d179c0e8860eb2ef36990b095933c8624aa078519851530e622e636519c04663d0d2d2f1f8
```

### `dpkg` source package: `init-system-helpers=1.60build1`

Binary Packages:

- `init-system-helpers=1.60build1`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.60build1
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.60build1.dsc' init-system-helpers_1.60build1.dsc 1951 SHA512:9bb66e5fa1313bcfe99e64f0ee4ea4a993dce7ddce428934fe6f5b708f8b1ce0cfd6dcec99754049219f079b7191ff82ab83d5ae3e4f36e1b47328c9d4a1643a
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.60build1.tar.xz' init-system-helpers_1.60build1.tar.xz 40636 SHA512:d2a5b6d1bb7666386834f257a36173fedf676b52228924423d427dca81d885b35ea81e8d311e833ef72dd0cf8fc9ebd686cbb417ef9f44b9113a07c6f43a5d66
```

### `dpkg` source package: `isl=0.24-1`

Binary Packages:

- `libisl23:amd64=0.24-1`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.24-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24-1.dsc' isl_0.24-1.dsc 1832 SHA512:5059c9077b3a7ddbd65607303c87976e0b002e10d478e07ac37480a4d52c9248829fec905b439748630fa7beae3d98e40477c4493194b7fa4b1fdf6820cbb7a3
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24.orig.tar.xz' isl_0.24.orig.tar.xz 1930956 SHA512:ff6bdcff839e1cd473f2a0c1e4dd4a3612ec6fee4544ccbc62b530a7248db2cf93b4b99bf493a86ddf2aba00e768927265d5d411f92061ea85fd7929073428e8
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24-1.debian.tar.xz' isl_0.24-1.debian.tar.xz 26440 SHA512:3fb98fe904ba58bc7461c53c81dead9cbbd908370a849914a9694678e694c68103103fa3735ff9a6f978536f459e9e89ec4246dd7ded158039399f8fa6207c23
```

### `dpkg` source package: `jbigkit=2.1-3.1build1`

Binary Packages:

- `libjbig-dev:amd64=2.1-3.1build1`
- `libjbig0:amd64=2.1-3.1build1`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.dsc' jbigkit_2.1-3.1build1.dsc 2085 SHA512:62ac0d564fcbe39c097c4e5e0e43dd5f9676f48c85b58affa016e703d4faa464ec01f47756276e874fb195ee0bb968ea24e39ef3656351b23b8ad38fded08d01
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA512:c4127480470ef90db1ef3bd2caa444df10b50ed8df0bc9997db7612cb48b49278baf44965028f1807a21028eb965d677e015466306b44683c4ec75a23e1922cf
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.debian.tar.xz' jbigkit_2.1-3.1build1.debian.tar.xz 7672 SHA512:3ace798cf76fdebcaa1ce497910f45b5a2553e7cae902a9399f1094020b6e24a213290ca499867e681cb7a5cff00dda9c834846b7b3956f90fde90793b1155fb
```

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

### `dpkg` source package: `krb5=1.18.3-6`

Binary Packages:

- `krb5-multidev:amd64=1.18.3-6`
- `libgssapi-krb5-2:amd64=1.18.3-6`
- `libgssrpc4:amd64=1.18.3-6`
- `libk5crypto3:amd64=1.18.3-6`
- `libkadm5clnt-mit12:amd64=1.18.3-6`
- `libkadm5srv-mit12:amd64=1.18.3-6`
- `libkdb5-10:amd64=1.18.3-6`
- `libkrb5-3:amd64=1.18.3-6`
- `libkrb5-dev:amd64=1.18.3-6`
- `libkrb5support0:amd64=1.18.3-6`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit12/copyright`, `/usr/share/doc/libkadm5srv-mit12/copyright`, `/usr/share/doc/libkdb5-10/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.18.3-6
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3-6.dsc' krb5_1.18.3-6.dsc 3636 SHA512:2824f0ed6c98e1bc38322c83ca7733e6d996b677247c43f25abfabcb79405af4a3c9b323db80829bdd56f058ce5122f3792a31688a4dc5d13484f70d3a595101
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz' krb5_1.18.3.orig.tar.gz 8715312 SHA512:cf0bf6cf8f622fa085954e6da998d952cf64dc7ccc319972ed81ea0542089cabf2d0e8243df84da01ad6f40584768ca2f02d108630c6741fa7b3d7d98c887c01
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz.asc' krb5_1.18.3.orig.tar.gz.asc 833 SHA512:7c5a83e13d00910d895d545ed63310ebec48c90c29846dd54e48048f710360e8306778729b636baa091a4e9048998ff6d4dfe37f88dd6292540d55678c961a30
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3-6.debian.tar.xz' krb5_1.18.3-6.debian.tar.xz 105116 SHA512:0a8654cb4bd923e3fbe653e0403f93ea13b23321022db6f7471d4dabb685d651f60c7fc2eb4c5d805177205e444eaa5e9fd246cb822e67f41825ee93bd7327eb
```

### `dpkg` source package: `lcms2=2.12~rc1-2`

Binary Packages:

- `liblcms2-2:amd64=2.12~rc1-2`
- `liblcms2-dev:amd64=2.12~rc1-2`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3 (GPL-3 for the fast_float plugin only)`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.12~rc1-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12%7erc1-2.dsc' lcms2_2.12~rc1-2.dsc 1988 SHA512:bb8187b25476b3c651cc4196d8bf3e09b5fdd93647aa2d27e06328fd0703da9e40d9f9824f1edab07e3d6cf0077cf71a20e945c77a5a4481ec59532e9dd73cc5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12%7erc1.orig.tar.gz' lcms2_2.12~rc1.orig.tar.gz 7417767 SHA512:1d27e6f91911053b79f2a46c6c16943e25fce2f0501bb7d97f49507522a8a0f911d60f20726fc31727fee5242c6d452c86cdc28735f8f88c3aa9676fd35fdec6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12%7erc1-2.debian.tar.xz' lcms2_2.12~rc1-2.debian.tar.xz 10420 SHA512:4e99528c61f71335e336ced40cf7d29403f2e107e9fa8411fb0e109af5291560af5a130fbc33b2656892cb7d9ff5754966313c31ea91d48dcccf8b3978c6bf04
```

### `dpkg` source package: `libassuan=2.5.5-1`

Binary Packages:

- `libassuan0:amd64=2.5.5-1`

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
$ apt-get source -qq --print-uris libassuan=2.5.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5-1.dsc' libassuan_2.5.5-1.dsc 2621 SHA512:7235cb3c0136c38c626af4a478feb5b4eb3d818aedbe548671fc516a8fc985bd7577f23a45ffc0c7ecc3df9c90e36734903a0b5445b0d5e70f12b835096da37d
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2' libassuan_2.5.5.orig.tar.bz2 572263 SHA512:70117f77aa43bbbe0ed28da5ef23834c026780a74076a92ec775e30f851badb423e9a2cb9e8d142c94e4f6f8a794988c1b788fd4bd2271e562071adf0ab16403
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5.orig.tar.bz2.asc' libassuan_2.5.5.orig.tar.bz2.asc 228 SHA512:343336ea5dffa113cd934167f548faf4e85d31bf64a46541ee6828b4d0995a8cc9d0668995812d9c4d3ab73347d5b1bbfff0d6ed586fbf4bbc57ac42e828e8d5
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.5-1.debian.tar.xz' libassuan_2.5.5-1.debian.tar.xz 14312 SHA512:71636b215b5d72f492777c474ba9e6b1c57742d30eeae81391acf23e898c0dfcc6f6910b8c6b381eae07e246b4ba8d866e1630aeb8e3c53f6e6b72dce9afd2b7
```

### `dpkg` source package: `libbsd=0.11.3-1ubuntu2`

Binary Packages:

- `libbsd0:amd64=0.11.3-1ubuntu2`

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
$ apt-get source -qq --print-uris libbsd=0.11.3-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.3-1ubuntu2.dsc' libbsd_0.11.3-1ubuntu2.dsc 2341 SHA512:7931bc1160445b75ccebb22a0ec54ff1bf3b7a181f3814c63f01617a893768e51673ad3ca57e6a1fe4428d7ceaeda4b6e95a0d0ce769b430f193101b871ba4e7
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.3.orig.tar.xz' libbsd_0.11.3.orig.tar.xz 399712 SHA512:a7015ea1ffa3766b1a4690526a25231898ad8275149b31fb6801082450172249997c36165626d101ffce53b59767a46676eebc0806426922fe4e773a0376c1f5
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.3.orig.tar.xz.asc' libbsd_0.11.3.orig.tar.xz.asc 833 SHA512:b8a469f0511619cea8bc653020ba72002952388dd7afbccb168df11322b5b9c3ba5a13929b2bc947b6c7dfcd1418441058767d5663c49386af428ed54bba7133
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.3-1ubuntu2.debian.tar.xz' libbsd_0.11.3-1ubuntu2.debian.tar.xz 19168 SHA512:a2873fbf296631a450ec3672989ba964571c921e39a6376993c52ef7f09156abd0afec462e18492ca295638910185d2baad5e260ff65a30432a61b2b945e8e1f
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

### `dpkg` source package: `libcap2=1:2.44-1build1`

Binary Packages:

- `libcap2:amd64=1:2.44-1build1`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.44-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1build1.dsc' libcap2_2.44-1build1.dsc 2228 SHA512:fc6bffe5c44c7b37a9e630622ebf55f90d99140792a5db7961b97552c1580c0381622a1deb6aeb3a566517b572ba073fc4797a2f964624f9d9042da75c005964
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44.orig.tar.xz' libcap2_2.44.orig.tar.xz 125568 SHA512:1bb323ca362923bd6bd0e2e4639cf8726975165a620a243b31e797056439eb7efb2bfbc8e5521636783a86c7415b2037b1638c98747b79183ca7d3d42a04ff20
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1build1.debian.tar.xz' libcap2_2.44-1build1.debian.tar.xz 21184 SHA512:1838af80c050fc4a9aea15944b86ccea4d4902c377607668beb4eeaa6213f83f07c9df102ae29d968be5e01cd3bfd7f32e2696b438b462f08d88a5faaf15ab2f
```

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

### `dpkg` source package: `libdatrie=0.2.13-1ubuntu2`

Binary Packages:

- `libdatrie1:amd64=0.2.13-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.13-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13-1ubuntu2.dsc' libdatrie_0.2.13-1ubuntu2.dsc 2371 SHA512:4c1b76df547563776f07237cf0d596b0a92494a64991faea12ba69ae10dab2ec5110cf37ac77964ef5a2e493328a0b0ddbd64d9387d85c843e81ea0188ff46b6
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13.orig.tar.xz' libdatrie_0.2.13.orig.tar.xz 314072 SHA512:db3c879d825ead5871c12ef3a06bb093cb1708a6e7e20775eaf82356af9dd6ad54c6b5cabbe1773f2494d3dfa2426528fdd49441038b6294b70ccb1a3d90099a
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13-1ubuntu2.debian.tar.xz' libdatrie_0.2.13-1ubuntu2.debian.tar.xz 9616 SHA512:55c350c179bff5f842ff23503dc5791c4e29d66ba33fe5a26505f019dfa85ae65f788f01092cd97e6120a296b5448ada0e0cbfed854882038a7bf588580a10cb
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

### `dpkg` source package: `libdeflate=1.7-2ubuntu2`

Binary Packages:

- `libdeflate-dev:amd64=1.7-2ubuntu2`
- `libdeflate0:amd64=1.7-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libdeflate-dev/copyright`, `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.7-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.7-2ubuntu2.dsc' libdeflate_1.7-2ubuntu2.dsc 2295 SHA512:aa208ad113a450abf7d3735dad886033115cb669a7c4501fcc5a6ed1e0d27fa2c523fde77fd45f478337bf070b0f5a09e85f27f14c11184472053a41702eed0a
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.7.orig.tar.gz' libdeflate_1.7.orig.tar.gz 144143 SHA512:82b297af2d3128a244e561893cce1d3664de410469ba6745c3f68fc3a1962c62467c427f3857bb679578e0f704cd0eba1a64b13c30505addd310ff9af1883068
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.7-2ubuntu2.debian.tar.xz' libdeflate_1.7-2ubuntu2.debian.tar.xz 4720 SHA512:c6a5db3c6e6e7034a9e5480ce08e375bde9363af24d35cc2f10bd62540389e7461ba51a0fa438bbb95e3e1cbb270aeb39b39747935e7b2d4f15291e7f78d8400
```

### `dpkg` source package: `libedit=3.1-20191231-2build1`

Binary Packages:

- `libedit2:amd64=3.1-20191231-2build1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-2build1.dsc' libedit_3.1-20191231-2build1.dsc 2257 SHA512:ec70c17a4642b392d7f398aaa135c1fdce8b6fb998bfa30ff26dd66362dea9b86b51fa631b3710203ea777afcc6200eb29677ac830b5c1112a2550538c4096e5
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA512:1df2eced98e8db1bb0af940678c154d87e3b11dd21e65a903682367f5feace5112f9a543b8e0cb04bbfeaaf73729f808db2d9c302637fc063e81c0a37777ac2c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-2build1.debian.tar.xz' libedit_3.1-20191231-2build1.debian.tar.xz 14664 SHA512:a93bd922fb88903036ee6aa40e5b50701f4185a8213b32e7897b2469ad5e4adf012b04916597a871dee64641ee6e7408e3e2dc33a4de1866cd35f762da0daa12
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

### `dpkg` source package: `libevent=2.1.12-stable-1`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.12-stable-1`
- `libevent-core-2.1-7:amd64=2.1.12-stable-1`
- `libevent-dev=2.1.12-stable-1`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-1`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-1`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-1`

Licenses: (parsed from: `/usr/share/doc/libevent-2.1-7/copyright`, `/usr/share/doc/libevent-core-2.1-7/copyright`, `/usr/share/doc/libevent-dev/copyright`, `/usr/share/doc/libevent-extra-2.1-7/copyright`, `/usr/share/doc/libevent-openssl-2.1-7/copyright`, `/usr/share/doc/libevent-pthreads-2.1-7/copyright`)

- `BSD-2-clause`
- `BSD-3-Clause~Kitware`
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
$ apt-get source -qq --print-uris libevent=2.1.12-stable-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1.dsc' libevent_2.1.12-stable-1.dsc 2527 SHA512:0a576f747323d12dc93e4da63dc6230a8be533f5b50d38e6f7e3420c8dba75986fe7cc30e64f212a57d7ddaa5a48b64ed7862d3cff4aafdfc25c82a4485c4642
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA512:88d8944cd75cbe78bc4e56a6741ca67c017a3686d5349100f1c74f8a68ac0b6410ce64dff160be4a4ba0696ee29540dfed59aaf3c9a02f0c164b00307fcfe84f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz.asc' libevent_2.1.12-stable.orig.tar.gz.asc 488 SHA512:841b57a0f6ba645b1871f257b9929093b11b7d6fd03332e6339adceddda233e78f6190faa2339e2b67b26dc2a56ddd7ce622792820b582168b31a2d1d1854f1f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1.debian.tar.xz' libevent_2.1.12-stable-1.debian.tar.xz 17764 SHA512:46f75a362e54dd120367009b8cd8cffb123b81855dd0cb0bd5c76610524abf92a7f439420a55d628d8e5fe0136fb832403cf034e683bb60b0637c83adb403d1d
```

### `dpkg` source package: `libexif=0.6.22-3`

Binary Packages:

- `libexif-dev:amd64=0.6.22-3`
- `libexif12:amd64=0.6.22-3`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.22-3
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-3.dsc' libexif_0.6.22-3.dsc 2079 SHA512:4dc9e9a63366fbbcd9c94c9f67194152895566d346718e4d9e08cbeac677978687a0048a142929cf1efb89243939137d8a7b54b8a7b0102786c86aae4a635218
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22.orig.tar.gz' libexif_0.6.22.orig.tar.gz 1109525 SHA512:6c63abe2734c9e83fb04adb00bdd77f687165007c0efd0279df26c101363b990604050c430c7dd73dfa8735dd2fd196334d321bdb114d4869998f21e7bed5b43
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-3.debian.tar.xz' libexif_0.6.22-3.debian.tar.xz 12468 SHA512:87dfece8707e44e99ffc9d08560e55d6b6f6806ca6f1a07a9646631e46b7508cf637590b02821299a98034afd0ac805b80105752199bff0c39f024945879ab88
```

### `dpkg` source package: `libffi=3.4.2-1ubuntu5`

Binary Packages:

- `libffi-dev:amd64=3.4.2-1ubuntu5`
- `libffi8:amd64=3.4.2-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi8/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.2-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.2-1ubuntu5.dsc' libffi_3.4.2-1ubuntu5.dsc 2055 SHA512:e88c7949e957694e7a2df7ec588ade04e9b99606ca84b547a9f4d8c8344173a07979fb254bbed353a6bfa0a807f6652777fe45338354f0c8680dba2fd9454215
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.2.orig.tar.gz' libffi_3.4.2.orig.tar.gz 1351355 SHA512:31bad35251bf5c0adb998c88ff065085ca6105cf22071b9bd4b5d5d69db4fadf16cadeec9baca944c4bb97b619b035bb8279de8794b922531fddeb0779eb7fb1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4.2-1ubuntu5.debian.tar.xz' libffi_3.4.2-1ubuntu5.debian.tar.xz 8240 SHA512:a7a62d46d76ea0dd4689d40ff9c66fcb9d1f628279db664f678670006efc2eda84c40e2ad34bd8b01dc1bc1ec718f6344532e83ed9171bde60c55062ae21a4f8
```

### `dpkg` source package: `libfido2=1.6.0-2build1`

Binary Packages:

- `libfido2-1:amd64=1.6.0-2build1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.6.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0-2build1.dsc' libfido2_1.6.0-2build1.dsc 2501 SHA512:2530455e880da1ffe83f8459fe69511b152246439b989c1f70d02ff21c809f3f500899fd3b9ceaa57800495e75c4263d1ffbb7f83efb435e6bca073b6c88148b
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz' libfido2_1.6.0.orig.tar.gz 413904 SHA512:c473732a2f7ef54156097d315e44457d89056446ab3112a7c7a6fd99d5c2c8ae0ca2451ff9cd45be6c32de1ab335d6dfdb2b0c56b40cae9eb41391d18d83be4a
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz.asc' libfido2_1.6.0.orig.tar.gz.asc 488 SHA512:ea6b2191bbbce3b1e905a6835cc05f38571f65d3590984e1591a1b630bafa29c646a4c813cc5761cf3013b41da1246a70037eaa7aeefe3daf7740a468cc99d4f
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0-2build1.debian.tar.xz' libfido2_1.6.0-2build1.debian.tar.xz 72756 SHA512:5c91b3a03b69cb734beecf6f97910ca3b52cc949a5e78cb8b9cec34087a2227cccad2ad247d569061c0c92e95cf8b34b2810c75a63b8cb97c574df8efdf5ef5b
```

### `dpkg` source package: `libgcrypt20=1.8.7-5ubuntu2`

Binary Packages:

- `libgcrypt20:amd64=1.8.7-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.7-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-5ubuntu2.dsc' libgcrypt20_1.8.7-5ubuntu2.dsc 2907 SHA512:0c8afb13df8b3ba984af2903045bfceb4f4e381020a71b231b556af4dd7ac9c87fced87e13045a2340dc4e63edb86d569f77e5cefc4a8c368ea73bc3ce7206c6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2' libgcrypt20_1.8.7.orig.tar.bz2 2985660 SHA512:6309d17624d8029848990d225d5924886c951cef691266c8e010fbbb7f678972cee70cbb91d370ad0bcdc8c8761402a090c2c853c9427ec79293624a59da5060
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2.asc' libgcrypt20_1.8.7.orig.tar.bz2.asc 228 SHA512:4ba6875dfddbc9bece0c4d25d1c3b0e6183045288ca876b84c24d487ee72f751ecda6eaec71e70ba00fd2434c77127283af1a957ac9e6f40352ef67add672c72
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-5ubuntu2.debian.tar.xz' libgcrypt20_1.8.7-5ubuntu2.debian.tar.xz 41648 SHA512:dc585e49ef0cb0b272d828f8477d67c09a6dde0537ac6f0e513fecf20f20afb30eb28368e4655f62397c52d763aa695db67bdfa8061f3d701ae1cefb39f056ce
```

### `dpkg` source package: `libgpg-error=1.38-2build1`

Binary Packages:

- `libgpg-error0:amd64=1.38-2build1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.38-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2build1.dsc' libgpg-error_1.38-2build1.dsc 2874 SHA512:c00d3774cae0417a5ef5c2a54075c69049ba7eeca1393d9ad096278d93f65722501cb2f375771fb9fd12fef23d8753b2fed83306270011c6ad6bb1a9705058db
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2' libgpg-error_1.38.orig.tar.bz2 957637 SHA512:b936a4738c2cee111d855b1ba3ec433da8c77799a87d1f71275f974f871ebfa593c9db06ea53f0490b6cd6b94bef34f6052a587a4d13d839ec0128500c2dd9de
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2.asc' libgpg-error_1.38.orig.tar.bz2.asc 488 SHA512:0f167c6d87f8028c294db2822c2e092f156504893c0bdd8bf883d00dcdd838fed4af5fd3726ab88d41f4e12e8b131cec45dcc610aeb25291ea870d3b9cb621f6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2build1.debian.tar.xz' libgpg-error_1.38-2build1.debian.tar.xz 19608 SHA512:6f50b80ba8b84ed1d1552c82f7f32e027c7abfe8d3e91c69b19ac66ebbc01f7cf4db6bd6c12ec947372b5261475efce167e5f52393e62c102ec8e7900dcfaac0
```

### `dpkg` source package: `libheif=1.11.0-1`

Binary Packages:

- `libheif1:amd64=1.11.0-1`

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
$ apt-get source -qq --print-uris libheif=1.11.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.11.0-1.dsc' libheif_1.11.0-1.dsc 2283 SHA512:3cd0f679192e45a8bd8106d30de8d18989dd8846f6a65a8b46ceef42d3090776891eb84b0fece0bfbcde03b5b633697f1ce9e51aae5094c2c2ab75f9c6cbe4fe
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.11.0.orig.tar.gz' libheif_1.11.0.orig.tar.gz 1680855 SHA512:1a5d54a09a5dc581a054052bac4299f7c96ca121650e9238312c426d5261247ce6af1840088b8717c5a53d212b7ec17bfaa109b9245abfaebf1603eaeb77b0ed
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.11.0-1.debian.tar.xz' libheif_1.11.0-1.debian.tar.xz 6928 SHA512:0985f72d717988edf1c82c28afeab62b4255a4d999543165a72208d52e72f7bfacac870e2c4e373ae4a349922bd49eba37bd453f5347685823b6cc42146daa5a
```

### `dpkg` source package: `libice=2:1.0.10-1build1`

Binary Packages:

- `libice-dev:amd64=2:1.0.10-1build1`
- `libice6:amd64=2:1.0.10-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.10-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1build1.dsc' libice_1.0.10-1build1.dsc 2098 SHA512:9f6f77ac1232659a77f251ca18d6a9c9aa5bdc17bf7ca3440c7a315bbf8d38a2694f2e17cda3ea51cf6660b3ab6e467dbb5be8a5103fd3155ded9f24ba1b96d7
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10.orig.tar.gz' libice_1.0.10.orig.tar.gz 481960 SHA512:2d4757f7325eb01180b5d7433cc350eb9606bd3afe82dabc8aa164feda75ef03a0624d74786e655c536c24a80d0ccb2f1e3ecbb04d3459b23f85455006ca8a91
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1build1.diff.gz' libice_1.0.10-1build1.diff.gz 11418 SHA512:fce82da0eadd6679a6f1616574f551f7404f1a3bc840877ba633d9f407541a7564fc64e5df8b2754d23019e529dc4029464f55fb7411e40bc548b290316539ba
```

### `dpkg` source package: `libidn2=2.3.1-1`

Binary Packages:

- `libidn2-0:amd64=2.3.1-1`

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
$ apt-get source -qq --print-uris libidn2=2.3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.1-1.dsc' libidn2_2.3.1-1.dsc 2206 SHA512:cfbdac93eae031170ad8b0fcfe63a2e62e6f16dee75a9c2a7594226d722677fcdfa3a8b40322dc6c33436222a1d0d1dea064d9bc6b38aadc29664bbc228fb784
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.1.orig.tar.gz' libidn2_2.3.1.orig.tar.gz 2188338 SHA512:4d77a4a79e08a05e46fc14827f987b9e7645ebf5d0c0869eb96f9902c2f6b73ea69fd6f9f97b80a9f07cce84f7aa299834df91485d4e7c16500d31a4b9865fe4
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.1.orig.tar.gz.asc' libidn2_2.3.1.orig.tar.gz.asc 488 SHA512:2db4bb3a11562634276664fb857306271c6ebc96cf5e90b39b404c3fe47190ec65ce3866cebcfa0c1216d29d7aed8c7907b869e602a722db1cf8f6ab94da9c78
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.1-1.debian.tar.xz' libidn2_2.3.1-1.debian.tar.xz 15620 SHA512:75951d21ba15f060310b66902d2665b612a8bde479c390a30e068faaf34919073d4b11d5b4c266119ecf30547a9eb120807d5663e812467c5bacec9156864ece
```

### `dpkg` source package: `libjpeg-turbo=2.0.6-0ubuntu2`

Binary Packages:

- `libjpeg-turbo8:amd64=2.0.6-0ubuntu2`
- `libjpeg-turbo8-dev:amd64=2.0.6-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.0.6-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6-0ubuntu2.dsc' libjpeg-turbo_2.0.6-0ubuntu2.dsc 2330 SHA512:5ed3fc85ac50719da212ce052728493b8c5d3a4524fa9b2518fb4ac431bf876d47e1e5671a9cdcb7e14981a98ba0a802c361dd8b5fa18bff991cecdffd31038f
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6.orig.tar.gz' libjpeg-turbo_2.0.6.orig.tar.gz 2192315 SHA512:504062778224f2ed2ddb64c988fbf466a14247952aab0cf1d35d281942b6f0874eafd34b45914d2208e087f05ddd896c5ba87a67c944e8bb80323e187413038c
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.6-0ubuntu2.debian.tar.xz' libjpeg-turbo_2.0.6-0ubuntu2.debian.tar.xz 17208 SHA512:1ab93071873603cb89ec3cb9c7430b09db4361a3f39d6965f7b0b25b6ec425fb847124f0d48e604333f0e1de7eb5296e507693321538d5a54161ec2971f5ec10
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu8`

Binary Packages:

- `libjpeg-dev:amd64=8c-2ubuntu8`
- `libjpeg8:amd64=8c-2ubuntu8`
- `libjpeg8-dev:amd64=8c-2ubuntu8`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg8/copyright`, `/usr/share/doc/libjpeg8-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg8-empty=8c-2ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.dsc' libjpeg8-empty_8c-2ubuntu8.dsc 1637 SHA512:294caa2f8c916f07fa653469c239f46304cabd9d0194c7f0b311027bf2b09d45e07d6b5bc7bbdd11920e574040ad2b45f3af092d90009a119916a4a4857e0dd6
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.tar.gz' libjpeg8-empty_8c-2ubuntu8.tar.gz 1770 SHA512:07407b8f295f07df0eff6a4384cba7bc11349a1cacf488422b6a20bcbe5cb0ef9809bf847f3e52304a8f092e3581ac40adb745d9281fd4c83edd79f4c7cc8111
```

### `dpkg` source package: `libksba=1.5.1-1`

Binary Packages:

- `libksba8:amd64=1.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.1-1.dsc' libksba_1.5.1-1.dsc 2470 SHA512:e0f5060fc25de9baba6adf37cc9dfb1daf3f142b821795c37922d5d46d41cf55716573e48e83d991548679f51d19373e6e2b85a38b6ba02b34dbd92b60aab68d
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.1.orig.tar.bz2' libksba_1.5.1.orig.tar.bz2 659280 SHA512:156fe6a36daa7b11ce580366ab36a5fceda253413f0057ace791e4f028fd3158a70a3f6ba1d0c824fafee4420d1076864dbd0911606fb65e14c8b2332b6cc92b
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.1.orig.tar.bz2.asc' libksba_1.5.1.orig.tar.bz2.asc 228 SHA512:cd86001afab025c8d7548143235b49ed29f7877e3b531e2f873ab85fc04817933b8faa68af1b42efecbf3ff1afea4db719d837b1b8dcb38238180fbc2d892ec3
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.5.1-1.debian.tar.xz' libksba_1.5.1-1.debian.tar.xz 13896 SHA512:f1d7c77da4c99fe864d0c2c0e8cce505520f75564fce6fda49c8d2473a41862764f1ec65ab0834a8e3d27f6a7d7945ea508a2890653d0b43d4f35518067665ee
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

### `dpkg` source package: `libmaxminddb=1.5.2-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.5.2-1`
- `libmaxminddb0:amd64=1.5.2-1`

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
$ apt-get source -qq --print-uris libmaxminddb=1.5.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1.dsc' libmaxminddb_1.5.2-1.dsc 2322 SHA512:9d3c797339ea8622069154493ded941a38f54a033130e3b55b7d3a14b94e61d2971615b925d283589cbc3161df3f2d3e308bc0da3ae32b80c4bb7ac66bb10bed
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2.orig.tar.gz' libmaxminddb_1.5.2.orig.tar.gz 249507 SHA512:2f053028e28dc4f1d94039e52193ab71f8dc278f1fafa14bca1af0251d239351acadb5d540e63c250232d0fd1b8f2dd45289f0eae5c55d9b4430acbabbcd11a9
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1.debian.tar.xz' libmaxminddb_1.5.2-1.debian.tar.xz 12328 SHA512:96d13a152582757703f9708364542153e93fdb3a2232b9794b98663fec744bc510516946c8dc669fb797497c2317fcc34da5beab92160b86404e975c05ef35da
```

### `dpkg` source package: `libmd=1.0.3-3build1`

Binary Packages:

- `libmd0:amd64=1.0.3-3build1`

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
$ apt-get source -qq --print-uris libmd=1.0.3-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.3-3build1.dsc' libmd_1.0.3-3build1.dsc 2297 SHA512:d32133c7a6f344161a87d729fa2443dae0d63a0eed1ca4f96fd6a66509e486d40daf12b49b84213e53191489103def287e146cb4a347fef0d649ebd8c6f591aa
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.3.orig.tar.xz' libmd_1.0.3.orig.tar.xz 258584 SHA512:f4b5a86bea7b9fac9f7f173032ee436d1e7141f760c1a114a785d31644edbf6802fe8193cc4cf3b5c66d38963be919c05055780bdf6bf5a47927690490ff5966
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.3.orig.tar.xz.asc' libmd_1.0.3.orig.tar.xz.asc 833 SHA512:e532a4f2d2aa2cff758a52d6bacead2fc98e5d03427882599921c4f1f13a306c1983683d2a381e0dd51429dd74cc65cf5084af93e7d048d20d34b1c6c2af0c13
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.3-3build1.debian.tar.xz' libmd_1.0.3-3build1.debian.tar.xz 10176 SHA512:57df8cd931be8510b90d0f6138b0b74fbf49435c4bc5c5b0317b7ae2e5ca461e14b5719dc7feff95c5d3f51d83e538f325ba14e981263e75eaff9231fa960fbf
```

### `dpkg` source package: `libnsl=1.3.0-2build1`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-2build1`
- `libnsl2:amd64=1.3.0-2build1`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build1.dsc' libnsl_1.3.0-2build1.dsc 2004 SHA512:3881693bdbc58ac4c926fa31e543e417cc75f0294c5dbcafb2a550f0e207f18fc39f860c6080b5cbb8d0e883669d0c9b0a3b95fbd921cb884ac9c9c684452bd5
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA512:a5a6c3ccb2d1e724c8c1f65e55dcd09383eb1ae019c55f4c09441eadf23ffbc2196cfad259805b0ac40ddf3a10af0da453e4d739d67d46829c64d0995dab4e55
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build1.debian.tar.xz' libnsl_1.3.0-2build1.debian.tar.xz 4772 SHA512:6d83aff8aa0e32a6e7ccabda6923ec3d13def4b1dc641aa66217d63b3c4b232311720e5e713af8e9bc3ddbe70f7b1fa7d7d159576eceae16045cdbe0bb06c526
```

### `dpkg` source package: `libpng1.6=1.6.37-3build4`

Binary Packages:

- `libpng-dev:amd64=1.6.37-3build4`
- `libpng16-16:amd64=1.6.37-3build4`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.37-3build4
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3build4.dsc' libpng1.6_1.6.37-3build4.dsc 2274 SHA512:68641c1a373d0f70c8ef99274665fd755467c66207fbfa87704a8acb0898d3cc385fcf6e5f5864fa9891a136aa9d367a43e8e623602f2cd4f41de171b0e24ae9
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA512:ccb3705c23b2724e86d072e2ac8cfc380f41fadfd6977a248d588a8ad57b6abe0e4155e525243011f245e98d9b7afbe2e8cc7fd4ff7d82fcefb40c0f48f88918
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3build4.debian.tar.xz' libpng1.6_1.6.37-3build4.debian.tar.xz 32408 SHA512:bfd478850938b0a5f674fcc6fe87e6d0bea7c5cdedecd7c9280dd45ffd2eb6433def42a3e02d1bc1a6695ffddc5b4ffd857520d67b200ff8dced63e5e151513d
```

### `dpkg` source package: `libpsl=0.21.0-1.2`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.2`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.2.dsc' libpsl_0.21.0-1.2.dsc 2216 SHA512:ddad24eef53ec0c61737b7ad67fdca2b5e80554b886972b753557e4b4a84b6e769ce5044c3d65698af5524fff912f32afe4af7989d9fce5500a74f058e4cbe89
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA512:b7466edb9763f94a65330dbb3c19586f9c7b01e20ddedb38ca2fd4c9ee5764a4f9b3291dc4b76659b45425d954f15973345f917b2cd2de72ea731e8c41f2a265
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.2.debian.tar.xz' libpsl_0.21.0-1.2.debian.tar.xz 12724 SHA512:2e91a28f8575166758a58de4f247988b4355af166316feafc44f47e1b5a516e6e174ba47e1c80093830cf001f21e9b4daf2127e46406d599dda6c2cb714e2284
```

### `dpkg` source package: `libpthread-stubs=0.4-1build1`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.4-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1build1.dsc' libpthread-stubs_0.4-1build1.dsc 1951 SHA512:259263cf3b50b128e0aa0cd7a22f0a8659bb49c432d2a6784050e07cbcd796f0ecf93db2189ab7e506e928e767da508d4d53effee84de34132a4d292d897feb1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4.orig.tar.gz' libpthread-stubs_0.4.orig.tar.gz 71252 SHA512:5293c847f5d0c47a6956dd85b6630866f717e51e1e9c48fa10f70aa1e8268adc778eaf92504989c5df58c0dcde656f036248993b0ea5f79d4303012bfeff3c72
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1build1.diff.gz' libpthread-stubs_0.4-1build1.diff.gz 2440 SHA512:68bc199c3cc945a7ea8924084d82710f065239878811580cdc910ab70ba21f275653191219f21b4d1a9851bc8b2c012b1218a347c45641155fc02451e7b69046
```

### `dpkg` source package: `librsvg=2.50.7+dfsg-1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.50.7+dfsg-1`
- `librsvg2-2:amd64=2.50.7+dfsg-1`
- `librsvg2-common:amd64=2.50.7+dfsg-1`
- `librsvg2-dev:amd64=2.50.7+dfsg-1`

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
- `Expat`
- `Expat,`
- `LGPL-2`
- `LGPL-2+`
- `MPL-2.0`
- `MPL-2.0,`
- `Sun-permissive`
- `Sun-permissive,`
- `Unlicense`
- `Unlicense,`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.50.7+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.50.7%2bdfsg-1.dsc' librsvg_2.50.7+dfsg-1.dsc 3001 SHA512:f900cf1e07bb1145c0f3ac53d29fde07f53698f7e295bf92abeb0a52f5173e7563603f06d8bbf969fff58ae2dce14faa05402225dc10b38eb7ced720c156a456
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.50.7%2bdfsg.orig.tar.xz' librsvg_2.50.7+dfsg.orig.tar.xz 19827956 SHA512:90238b505f3f0ccb0d9d2fe7f44ebeffdafe238c0eaaa22cbf3993629a725a9df35a6f0f84eadd2a6463ca0a5e524fa6f924213bd9231322ea134ac3822bed40
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.50.7%2bdfsg-1.debian.tar.xz' librsvg_2.50.7+dfsg-1.debian.tar.xz 30148 SHA512:c26721aa43cf1ddb8c9039213ef44d70073cf23f91680a0f549476b74871c49b41eac1588ebdebb57e3bef81ce5fba30aa8abd8f98dbeda76c99664388171ee3
```

### `dpkg` source package: `libseccomp=2.5.1-1ubuntu1`

Binary Packages:

- `libseccomp2:amd64=2.5.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.1-1ubuntu1.dsc' libseccomp_2.5.1-1ubuntu1.dsc 2546 SHA512:42d9fa21b16df347f275dbe6e2cce30d09ba92219214e4dbd068d157d89e066e0cf2438d81bbeacc5f8f1df8c2d0295c5a1ce811164e16cdc82c231150fe9c34
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.1.orig.tar.gz' libseccomp_2.5.1.orig.tar.gz 638811 SHA512:2be80a6323f9282dbeae8791724e5778b32e2382b2a3d1b0f77366371ec4072ea28128204f675cce101c091c0420d12c497e1a9ccbb7dc5bcbf61bfd777160af
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.1-1ubuntu1.debian.tar.xz' libseccomp_2.5.1-1ubuntu1.debian.tar.xz 31156 SHA512:b808469d617cd1f7418ff9e69463fa7a26d2b823490857b644211db52a7d66301a69a1737dabfca316ae080e183028828bbaa95779774cdb1c8511e63b4c295e
```

### `dpkg` source package: `libselinux=3.1-3build2`

Binary Packages:

- `libselinux1:amd64=3.1-3build2`
- `libselinux1-dev:amd64=3.1-3build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.1-3build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-3build2.dsc' libselinux_3.1-3build2.dsc 2670 SHA512:bc2e3b8176fc7afb67be9bc12ca6af8d4ddb378b018caf481a55f383c3c4652e1ed86af2e3d0cd62c05d0d82c35885f3b53a3a46c19f6f7635ee7196eef81e7a
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1.orig.tar.gz' libselinux_3.1.orig.tar.gz 204703 SHA512:57730cddd2d4751556d9e1f207c0f85119c81848f0620c16239e997150989e3f9a586a8c23861fd51ed89f7e084ad441190a58a288258a49a95f7beef7dbbb13
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-3build2.debian.tar.xz' libselinux_3.1-3build2.debian.tar.xz 24288 SHA512:14e0deec173d848aa20d80e89a9bfeaa1c4f6498604e0e65169a80315d2955f6a19e60633ad3e7564d79fbbe239b224bad9d4c298fadc06ba7c170ca1b10c4e9
```

### `dpkg` source package: `libsemanage=3.1-1ubuntu2`

Binary Packages:

- `libsemanage-common=3.1-1ubuntu2`
- `libsemanage1:amd64=3.1-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1ubuntu2.dsc' libsemanage_3.1-1ubuntu2.dsc 2713 SHA512:a928d4e92ef8617529bfea452869d250d84b5e944a274a60fc878310fad9371c5a399718d36a8b526707f305eb81a94baef8cd86136db4b313f7e59709c04dad
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1.orig.tar.gz' libsemanage_3.1.orig.tar.gz 179601 SHA512:8609ca7d13b5c603677740f2b14558fea3922624af182d20d618237ba11fcf2559fab82fc68d1efa6ff118f064d426f005138521652c761de92cd66150102197
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1ubuntu2.debian.tar.xz' libsemanage_3.1-1ubuntu2.debian.tar.xz 17876 SHA512:d06cb8c40ada4e854e2283b768217e924b4e2e59b3197418d4361d803e0f6e368ddb671ab5eb04c2f5d1fee1dadeae323044a04242586116f271ff266fa7b9d7
```

### `dpkg` source package: `libsepol=3.1-1ubuntu2`

Binary Packages:

- `libsepol1:amd64=3.1-1ubuntu2`
- `libsepol1-dev:amd64=3.1-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`, `/usr/share/doc/libsepol1-dev/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1ubuntu2.dsc' libsepol_3.1-1ubuntu2.dsc 2150 SHA512:ef1d2e5c03dfaab2895570e0798894dac489ea0ccd6c05d38b0db1ed418a0b8090c5432cc6a81325c9bc1ae2f3ee97e957a098d9842129d69125c1e0b381d3a4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA512:4b5f4e82853ff3e9b4fac2dbdea5c2fc3bb7b508af912217ac4b75da6540fbcd77aa314ab95cd9dfa94fbc4a885000656a663c1a152f65b4cf6970ea0b6034ab
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1ubuntu2.debian.tar.xz' libsepol_3.1-1ubuntu2.debian.tar.xz 14812 SHA512:b76a2dc19431d19295fb5841ad9ddf92ad42c8a851b23e7df932ad71d5e4a2dc4865d5e0bdd5438f5b88a127b9e3fc79a8134361fdb16d7360bbd1c095b22b5c
```

### `dpkg` source package: `libsigsegv=2.13-1ubuntu2`

Binary Packages:

- `libsigsegv2:amd64=2.13-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.13-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13-1ubuntu2.dsc' libsigsegv_2.13-1ubuntu2.dsc 2470 SHA512:884873078166325c21a8f1a0c68b9fdae7b8b1ec7fbd24b3bb312dad63f4509ba77d9652db71b5b585e4d05d49335260d54809fb7907a9b767ba0a7ab2632724
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13.orig.tar.gz' libsigsegv_2.13.orig.tar.gz 460736 SHA512:9c0cf01ee2a39f77f2e42eb06a2aa60644e10fe2cd39089de58f6206baf7fe7d61fe0ec6bf187276fcfccf61585154ce904fe374b474b7ba9fa050a61a2f3918
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13.orig.tar.gz.asc' libsigsegv_2.13.orig.tar.gz.asc 819 SHA512:92d8c651557a7cd0ba0a9e0f45f75f5ee7508041e014c8438aa0d84065b5a343867346acbf007fd0d8b3a120e6bde993935f66d1cbd62583bc763ecdde359640
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.13-1ubuntu2.debian.tar.xz' libsigsegv_2.13-1ubuntu2.debian.tar.xz 8908 SHA512:94461f5f88fde371882523d4025057c5418f1d0c1381788dabd11da05e34585b3d18f4b5229b69a487987a10cc1bf26e470b06d5ee8ebb7d60fa26189d0fa637
```

### `dpkg` source package: `libsm=2:1.2.3-1build1`

Binary Packages:

- `libsm-dev:amd64=2:1.2.3-1build1`
- `libsm6:amd64=2:1.2.3-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.3-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1build1.dsc' libsm_1.2.3-1build1.dsc 2087 SHA512:f9b88c48c1ac519cb1f44a614c4126201d8faae1e3cb36025300f55c4acbc466cf45df5864e4bae423ea9cae01b98781fc395c13658850bcbd2522f53170a787
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3.orig.tar.gz' libsm_1.2.3.orig.tar.gz 445362 SHA512:03b77d86b33cdb3df4f9d65131a0025182f3cb0c17b33a90d236e8563b3011d225b9d006186302d07850edafa5b899aec6a086b8d437d357cd69fedd5f22d94b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1build1.diff.gz' libsm_1.2.3-1build1.diff.gz 9003 SHA512:316dcf9581d82165e7ee7067eedc8c8fa25cd712a62e93355a83e710d1eaa6da365223d153cce016112bce30e2a37ec83683e1eadd852cbf6bfc62de901c2365
```

### `dpkg` source package: `libssh=0.9.6-1`

Binary Packages:

- `libssh-4:amd64=0.9.6-1`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6-1.dsc' libssh_0.9.6-1.dsc 2688 SHA512:c322813309cceca2b14a6f132d2b7bd645d5f114d2b3f7e4664b0e5c231fee97cff3092118c28e90570f3a826f98585b8a9f14990754c55df7bbfd4f69fde872
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6.orig.tar.xz' libssh_0.9.6.orig.tar.xz 1053056 SHA512:4040ec4af937e95be2e41313ef6d4db60b46b8d4dea10c09402398127c1d1ca8843392d207088aeee3c7ef631c6ae7b66861327dcebf78ed3af0723777619fd1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6.orig.tar.xz.asc' libssh_0.9.6.orig.tar.xz.asc 833 SHA512:1b6223efe9e4ce864cd8d97d517f9f0d38c1cd502b5874fdc6a58731038c2830a72ce753f02fc062d9d4d5922107ec9a2e62fe24a704bb5dec0dcfecdb569fe6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6-1.debian.tar.xz' libssh_0.9.6-1.debian.tar.xz 27180 SHA512:8cf2cd67e483f36ceabb7fcbdb8dd4d82a87edec009fcb5dce4d210ebe6a4212b2e48da1ed39a054e5b668b5fd8e5966e288da9a7ffe056136c3aa1d1fe043cf
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

### `dpkg` source package: `libthai=0.1.28-4.1`

Binary Packages:

- `libthai-data=0.1.28-4.1`
- `libthai0:amd64=0.1.28-4.1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.28-4.1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28-4.1.dsc' libthai_0.1.28-4.1.dsc 2333 SHA512:63f3bddc46a2a31eac70c82f671ba5a71eecddfbd2355f5911f38004d81992cbda42736a223cc828712d9c944367ad8ca2616f7ddc0bcbcfba10b50270a7db62
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28.orig.tar.xz' libthai_0.1.28.orig.tar.xz 413592 SHA512:925be8367ae0cba026e602f1f60c813306e9051e22fe722afba496b6e493f8c1f3eb56abb77ca663f53678b14ad793daf3269b32d32720c0d869b906cdf15f4e
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28-4.1.debian.tar.xz' libthai_0.1.28-4.1.debian.tar.xz 12852 SHA512:1d97e33af84fe650ef579cd67f6c012536d298a329fdc0cf15f821c5f9aa78ed64dec5740d203e08f4732f6ed574d1b8a5ed9ee0eb57c35b4454acb5ac03f29e
```

### `dpkg` source package: `libtirpc=1.3.2-2`

Binary Packages:

- `libtirpc-common=1.3.2-2`
- `libtirpc-dev:amd64=1.3.2-2`
- `libtirpc3:amd64=1.3.2-2`

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
$ apt-get source -qq --print-uris libtirpc=1.3.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2.dsc' libtirpc_1.3.2-2.dsc 2111 SHA512:f7b3f3d948f0aa417f40f41c769780b70dda4bbd7d421da4515a0b69c525809b4a182edd91f64187efe9b7c581ddfc1f5ec4c14a29bb738849181cbb324abcc1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2.orig.tar.bz2' libtirpc_1.3.2.orig.tar.bz2 513151 SHA512:8664d5c4f842ee5acf83b9c1cadb7871f17b8157a7c4500e2236dcfb3a25768cab39f7c5123758dcd7381e30eb028ddfa26a28f458283f2dcea3426c9878c255
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2.debian.tar.xz' libtirpc_1.3.2-2.debian.tar.xz 10996 SHA512:742916905b6fa8b5a41d151cac18a7bb2eaa7571675ed486907ffba71b23871165db9d08578469caa61a33c677adcfb04309211a86aa815a88952fc87e572a78
```

### `dpkg` source package: `libtool=2.4.6-15`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-15`
- `libltdl7:amd64=2.4.6-15`
- `libtool=2.4.6-15`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-15
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-15.dsc' libtool_2.4.6-15.dsc 2502 SHA512:7315ff050096ea5a250889f4cc853307e3f8b3fb1ad3fc903979415b67be7621c20ede7f0f9f09c6975d3510a4512924888ad27312d10ea976a6d0f27cc488a5
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA512:a6eef35f3cbccf2c9e2667f44a476ebc80ab888725eb768e91a3a6c33b8c931afc46eb23efaee76c8696d3e4eed74ab1c71157bcb924f38ee912c8a90a6521a4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA512:2f26447a837e3242b8f8f38fbab22d89df0949ee62fd966af3b5bae3aa939ba53bc4621174ee58d1c6722d569d7fe5f90097ddccffed28c3067fe5fa996fcb89
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-15.debian.tar.xz' libtool_2.4.6-15.debian.tar.xz 53924 SHA512:5cffe71b101992e73051a4563c4afab2a32270daaf212b2299eb33fb1a843db3032bac02b35c7ae6a2ff54f044d14a4b7d64026f5fbf0f425a8f3de49bf8a498
```

### `dpkg` source package: `libunistring=0.9.10-6`

Binary Packages:

- `libunistring2:amd64=0.9.10-6`

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
$ apt-get source -qq --print-uris libunistring=0.9.10-6
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-6.dsc' libunistring_0.9.10-6.dsc 2212 SHA512:838b5c4e4fad0b372335afe7bead76cd11a911e6278bc9e829c8c92d24a4599f09c751cb02b02e9a14778b30f0ef9d4e6c9611d199eed43ad290fe8e8c962ba5
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA512:01dcab6e05ea4c33572bf96cc0558bcffbfc0e62fc86410cef06c1597a0073d5750525fe2dee4fdb39c9bd704557fcbab864f9645958108a2e07950bc539fe54
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA512:94d4316df1407850f34e84064275ae512d1ee1cd519420e2342a3f36c17d1ff7fa4019fea64507a04034ffc356c0c9add94a5abf756dd5995913583f68cfe0bd
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-6.debian.tar.xz' libunistring_0.9.10-6.debian.tar.xz 41588 SHA512:440a3c65e8b155f11bf823289e1481fb25e4a0b2686de53288fde8695a7947dfa47891445a9ffe3a963b5109fabbfedf76bce48bf5a8441ec70098987c25c6df
```

### `dpkg` source package: `libwebp=0.6.1-2.1`

Binary Packages:

- `libwebp-dev:amd64=0.6.1-2.1`
- `libwebp6:amd64=0.6.1-2.1`
- `libwebpdemux2:amd64=0.6.1-2.1`
- `libwebpmux3:amd64=0.6.1-2.1`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.6.1-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.1.dsc' libwebp_0.6.1-2.1.dsc 2054 SHA512:23b02e37d5d09228b16b0bc6e748b379b998d41dd216e37887a2650800fc2210ca184cbcb36b9d1a363c94de46e55bb73ffce4a853da230db711fe63a11f8bfe
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA512:313b345a01c91eb07c2e4d46b93fcda9c50dca9e05e39f757238a679355514a2e9bc9bc220f3d3eb6d6a55148957cb2be14dac330203953337759841af1a32bf
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.1.debian.tar.xz' libwebp_0.6.1-2.1.debian.tar.xz 13616 SHA512:5774c80c1607886297b34ac6817a5b205e7e0bf30d104e5137aab2a970440e8a61f6f1ef18735069754eaf816be30f301094a1e25ff23e4160eb3c4a3565fcba
```

### `dpkg` source package: `libwmf=0.2.8.4-17ubuntu2`

Binary Packages:

- `libwmf-dev=0.2.8.4-17ubuntu2`
- `libwmf0.2-7:amd64=0.2.8.4-17ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-17ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu2.dsc' libwmf_0.2.8.4-17ubuntu2.dsc 2321 SHA512:8671c220be95d7007081d808c31584e18bd3d35a70b4bffe4fa5653e2397aa0cf24fe022a7bc802313da4baf22442d6a40562aabf163ca1b59163ce1f373a56c
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA512:d98df8e76a52245487b13e5ab3d2fbba9d246f97ee04a7344c0e5861bb2d0f990fc6d662dbd849ce621768b06eaebd4270fb34bec4ee004334a98b14ba6044a5
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu2.debian.tar.xz' libwmf_0.2.8.4-17ubuntu2.debian.tar.xz 13040 SHA512:d8969877b0f8def128357c2a5bd3ae9d0e1e67eec0fbc0977c44127c1cff220a05f482436a1d5a151482b47afe68b62540001a98b3dd562ab79c09702dccdab4
```

### `dpkg` source package: `libx11=2:1.7.2-1`

Binary Packages:

- `libx11-6:amd64=2:1.7.2-1`
- `libx11-data=2:1.7.2-1`
- `libx11-dev:amd64=2:1.7.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.7.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2-1.dsc' libx11_1.7.2-1.dsc 2539 SHA512:687778e86e3ccf50de675d19840905ba36c09fe156709dc19a5ba1a4ea5bc20b98c35720178e6ed0d31d2ce249d4eb055deab35d5f486566b748db20418064ca
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz' libx11_1.7.2.orig.tar.gz 3181228 SHA512:9828e63a2be4b74afa7ebd91373f293d564ee865e81c3b92020041353443ce858eb8712a19b26b3c6b22b016051336fa8dd7d74a02bdeaffbadcba3012d397fa
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz.asc' libx11_1.7.2.orig.tar.gz.asc 833 SHA512:13e8c484fc45324445c6030d72383154c43aa2d4fe3e4741324bda1bcfbfd0db9f0ea16f649668460bdf7e3d5b7a175e0b0d74b44ee5d90f9e7a57cc86aeb423
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2-1.diff.gz' libx11_1.7.2-1.diff.gz 76026 SHA512:ec35ce29557049461812e878b312507a6bac0f4adb3e07e6551846ab97cea99d1f864f4c9048a87a8a5bc4f22a396ba3c4b2effd43e7ad32d190ad49716acdfa
```

### `dpkg` source package: `libxau=1:1.0.9-1build3`

Binary Packages:

- `libxau-dev:amd64=1:1.0.9-1build3`
- `libxau6:amd64=1:1.0.9-1build3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-1build3.dsc' libxau_1.0.9-1build3.dsc 2311 SHA512:22709f548903a519b425716844b1ebe7924d9ee1b83d98cc37b3928b840fb3f53f8d0665c5be6ace36a1efbbc2247af7556b187ac9256e6293e8247edcd368d7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA512:3b22f34a4e35d17421189df8ce3f858b0914aef0cea0b12689dd8576f14eb811e39d6e32384251573daa7e3daba400deea98e7c0e29b4105138cf82195d7f875
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz.asc' libxau_1.0.9.orig.tar.gz.asc 801 SHA512:e59b2944591499d0c0291a8d80ad8ee2cb13ee00c32b0d26c6af12a2bb96c947d4d15924ef15b377b8d7640b75b50f9b8127ba53c582090b3f73b7bcf9e00b01
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-1build3.diff.gz' libxau_1.0.9-1build3.diff.gz 10372 SHA512:59db920f744352329e216121edf875e17c837d6ed5e18aecc4d2054b64145fedf29fe25954d60b60827cb6869137d91c63290e36b8345d8d0fa21dfa142e1ba6
```

### `dpkg` source package: `libxcb=1.14-3ubuntu1`

Binary Packages:

- `libxcb-render0:amd64=1.14-3ubuntu1`
- `libxcb-render0-dev:amd64=1.14-3ubuntu1`
- `libxcb-shm0:amd64=1.14-3ubuntu1`
- `libxcb-shm0-dev:amd64=1.14-3ubuntu1`
- `libxcb1:amd64=1.14-3ubuntu1`
- `libxcb1-dev:amd64=1.14-3ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-3ubuntu1.dsc' libxcb_1.14-3ubuntu1.dsc 5397 SHA512:b35ec5be1a8f706172a0341c541b05dd7abdbf7b0f591b050c647f79a05336da6e0d1070db6cd54f3b0173c6bdf2e5ff146e52096565d0255e56b1e2c8b558b9
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA512:6114d8c233b42b56604787a0475e924143aa13f1d382e6029b2150a4360c12ce78073409f754fbb1e5d9f99fc26900c0a4c59e9cfbd4c3d0a3af0c1306e62da1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-3ubuntu1.diff.gz' libxcb_1.14-3ubuntu1.diff.gz 26941 SHA512:f2696ec6fad36c01e8b722d9698d9dc3527ae2a9804376276528f7b7ce67860fd82bb73043a3ffa2ade71ce413f88f3152a046076a640469d20c119ebabd21dc
```

### `dpkg` source package: `libxcrypt=1:4.4.18-4ubuntu1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.18-4ubuntu1`
- `libcrypt1:amd64=1:4.4.18-4ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.18-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.18-4ubuntu1.dsc' libxcrypt_4.4.18-4ubuntu1.dsc 2214 SHA512:20dd3471f1fcda650018c8235762d6c0a08730a1ac47d338af34a30bacf82aa17114a86aa92d6933f97f0497988bf6c6bc2d5d66ac23aa9c20f8c52d3b98aef0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.18.orig.tar.xz' libxcrypt_4.4.18.orig.tar.xz 397776 SHA512:e12f82cef6fa1cfdbe9c6df2321dfdca2210edbcfbb4e8ce2a2f7aa2d3d5f5f4e540becf2cf8b05f66d3be5f4c40839ca2cf598559a426e0337399313c34f3ae
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.18-4ubuntu1.debian.tar.xz' libxcrypt_4.4.18-4ubuntu1.debian.tar.xz 9024 SHA512:c7e087653ed4b267047d513037e2d4ef13be99c5d586ba55a4860a6207150f6c29b35ccc7c9bf0bced32d58e9b18ea1e3833652d5b414b3b97dda960bf6e6bc9
```

### `dpkg` source package: `libxdmcp=1:1.1.3-0ubuntu4`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.3-0ubuntu4`
- `libxdmcp6:amd64=1:1.1.3-0ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.3-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu4.dsc' libxdmcp_1.1.3-0ubuntu4.dsc 2248 SHA512:a724e6d1bbd9b9212734e18a02e84feb72e7c82c1608cf6a8cd3d6567ca0330b4946a554112f223a975ea0f2a7944e650a64fd13281800a55e0244465f41c7fc
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3.orig.tar.gz' libxdmcp_1.1.3.orig.tar.gz 429668 SHA512:edd05654ad9ea893e9e08269e25ea050d10eaf9f997a08494e24127d1ba0c896cd5338b4595b155c8cbf576e1d910b76e6ad7820fee62d74644f1f276551e2f2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu4.diff.gz' libxdmcp_1.1.3-0ubuntu4.diff.gz 18183 SHA512:6eaddddbaa9c4ea3c96ffc00a60e2ef21ee0a7aa61b40e6da4c6ab04734c701923749b341dbaa0447f24930a641acb4098b52c370565aa51562ddec5698495cd
```

### `dpkg` source package: `libxext=2:1.3.4-0ubuntu3`

Binary Packages:

- `libxext-dev:amd64=2:1.3.4-0ubuntu3`
- `libxext6:amd64=2:1.3.4-0ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu3.dsc' libxext_1.3.4-0ubuntu3.dsc 2367 SHA512:b767983726441620d00f1eefa04866383797be55e33afc5d0f1156b9b4da16582f4194428905f4c848ad17b90dfc597b5b983c85ac273d0987e377c03c4492ec
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA512:4eebd639fd57cb9b84a1e17e368f82fbf3d9f021eef5ad3fe31dd128500db57862a82c1e0d214d447cb7641b2be3fd7e949ee1196f2a482793c6628fb1e5cd70
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu3.diff.gz' libxext_1.3.4-0ubuntu3.diff.gz 20753 SHA512:1d9be8ee74f341d1e4262831738ce918fda4360a65e8800de4ea8bdf5dc1aa2ff89186b23e8bd9bf5540a5d3d6e1cca4a07672d48c76ef2f2fc211dd4eb58fc4
```

### `dpkg` source package: `libxml2=2.9.12+dfsg-4ubuntu0.1`

Binary Packages:

- `libxml2:amd64=2.9.12+dfsg-4ubuntu0.1`
- `libxml2-dev:amd64=2.9.12+dfsg-4ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.12+dfsg-4ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12%2bdfsg-4ubuntu0.1.dsc' libxml2_2.9.12+dfsg-4ubuntu0.1.dsc 2779 SHA512:6a6cba7bfce0988d493efeb98960596e3e6a57cd5924d5de9dce2589da3059637a77218983aa73f9216ffe6d4416a69663ca37bce28bd757b8ea955a9859006d
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12%2bdfsg.orig.tar.xz' libxml2_2.9.12+dfsg.orig.tar.xz 2535044 SHA512:08ffb640e5669b52b29817887d62ef698799570ee5757612826e00aa5237ebf16b13bf838c350aff0ac1081547458d6d1aa6473f3499db7bf87e1f6d39f76386
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12%2bdfsg-4ubuntu0.1.debian.tar.xz' libxml2_2.9.12+dfsg-4ubuntu0.1.debian.tar.xz 35008 SHA512:c77200919089b0f4cbaaa4770700754012dad6f00f60c66598258c38574f81037bf2a3d7023ea6c2505122c8be5d0a556032c0464991cf654a431c193e0063ef
```

### `dpkg` source package: `libxrender=1:0.9.10-1build2`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1build2`
- `libxrender1:amd64=1:0.9.10-1build2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1build2.dsc' libxrender_0.9.10-1build2.dsc 2113 SHA512:61090059674614e9ae1428840a88be690e7d38cb66464a14c213b82f3b8a462abac03c392479527003fecd7f900ccb4b6ec94936345f559b7376d18ee61bf788
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA512:7768e62b500f468460f88f27bc1130170b204b478573d9e4406867e557b5638b7c1e21d88d51f9e774ce2344780a384e3c3be51421275d2ee880f9a978a3a232
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1build2.diff.gz' libxrender_0.9.10-1build2.diff.gz 15610 SHA512:67d3b43b4f215b70ef4169917c1503b64fe9b6b6daa8941426002aba6c6a9dd4b4fe99ec80d2c0c6369ef3af6ecf43f2c00fd34cff9aa1a00087833c121ac07d
```

### `dpkg` source package: `libxslt=1.1.34-4`

Binary Packages:

- `libxslt1-dev:amd64=1.1.34-4`
- `libxslt1.1:amd64=1.1.34-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.34-4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4.dsc' libxslt_1.1.34-4.dsc 2375 SHA512:dabcebd926e3f02a3f617bfe06dfeeaf32b01c902cd80a1c03b772f03f98609eb6dc4729432d0a7289f8aeea02ba31e8d7dcbb046b062a73c085f70ab6bfef09
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA512:1516a11ad608b04740674060d2c5d733b88889de5e413b9a4e8bf8d1a90d712149df6d2b1345b615f529d7c7d3fa6dae12e544da828b39c7d415e54c0ee0776b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA512:9b155d4571daede99cdbf2813a85fb04812737b5e23d3f7c9840225b38f3dbf171623a21645daaee190e7ff9ba38bde932922e96a2a2312c203ffa9917c3baea
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4.debian.tar.xz' libxslt_1.1.34-4.debian.tar.xz 21464 SHA512:dbd4104503a3eee856bf42c0a55e78de3687578498c4ab6dac889e787997a1a2fc9d95a0ea7acee37fa6e31e3f79bd791a176eb2f616fa5a8886008fe87b53ce
```

### `dpkg` source package: `libxt=1:1.2.0-1`

Binary Packages:

- `libxt-dev:amd64=1:1.2.0-1`
- `libxt6:amd64=1:1.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0-1.dsc' libxt_1.2.0-1.dsc 2298 SHA512:68dcfae9bc0ba85aab25d6be62cdd8f5ac1bbcd79428f9def8fa4058befbf4b52b3da85e84f94b0a55ea4c3f37afcaf27344e61f7e1da07df0eae8e7829a1b41
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz' libxt_1.2.0.orig.tar.gz 1016961 SHA512:af8147becd98c956e9324b765151f46352cafa1f962c7d1517b18b5d27aa80d093cc3ceabd92c0f181485540987b7e46b18baf38ffe1eadf3f60ab66c3f66c52
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz.asc' libxt_1.2.0.orig.tar.gz.asc 195 SHA512:a105f63f0fdcdddea75024e869dbe271d4261703616d5d2a3393943bf20b72fc70e9c52382dcc0370d2460737fda6f4bcaac3fa7eb84e2f6e234aa358758a13a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0-1.diff.gz' libxt_1.2.0-1.diff.gz 31129 SHA512:de872120880bf38ea2aa362f4e53e0cc84ed7e147c760183ca0f77797d9e0042070fa2c16613ec23a08bc193ecb9c5a12cedbf87ead5483c6c574b25a9f750dd
```

### `dpkg` source package: `libyaml=0.2.2-1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.2-1`
- `libyaml-dev:amd64=0.2.2-1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.dsc' libyaml_0.2.2-1.dsc 1833 SHA512:376309b84fc5e119aee97cc8cdfbf2bcc83b9f09d3967a78ee8beee47c391d89580df1d492dca8d4d81549958e546e802a42c10bf7d902e00074134ae659c063
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2.orig.tar.gz' libyaml_0.2.2.orig.tar.gz 602509 SHA512:0728c89ba43af3cdec22bccaf18c9ad7b07e13cdebed9d8919e2c62cf90bb5e23d2c746fd250320b2827dfcd9f1ce442d3bf8a3fe18b61f9a8d1d7770561e610
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.debian.tar.xz' libyaml_0.2.2-1.debian.tar.xz 4112 SHA512:39c4a9bbb5bc5602e4672ce1ff74b8e85e90fcb86efd2623face9692a525a91a1bc449a45ac0e241eedce4e677aa9be3ef13784ebac868a14f78e41c3ae6f9cb
```

### `dpkg` source package: `libzstd=1.4.8+dfsg-2.1`

Binary Packages:

- `libzstd-dev:amd64=1.4.8+dfsg-2.1`
- `libzstd1:amd64=1.4.8+dfsg-2.1`

Licenses: (parsed from: `/usr/share/doc/libzstd-dev/copyright`, `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.8+dfsg-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-2.1.dsc' libzstd_1.4.8+dfsg-2.1.dsc 2274 SHA512:80d08192a1cfbd07b93072a99f898111ae7009105e4e378b1ed7aa722df3123753729b545cd7b3608d17be17a4be1d1231658222531c9f31db6210892644a3a6
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA512:07fabe431367eea4badae7b1e46ac73e0b33aad5b67361bc7b67d5f9aef249c51db5b560f1cf59233255cc49db341a8d8440fed87745026fca7a7c5c14448cd8
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-2.1.debian.tar.xz' libzstd_1.4.8+dfsg-2.1.debian.tar.xz 12224 SHA512:c43ebcd786bf0bf011ba37136ff03f6996b1569508a98aea55c004e48466080f0b799fba71469391898d55253a435c80b1a0a75c7f5229980dc973cf09f98814
```

### `dpkg` source package: `linux=5.13.0-35.40`

Binary Packages:

- `linux-libc-dev:amd64=5.13.0-35.40`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lsb=11.1.0ubuntu3`

Binary Packages:

- `lsb-base=11.1.0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu3.dsc' lsb_11.1.0ubuntu3.dsc 2218 SHA512:af52feb8995d853a0d5d9e1bffe7c86527a64d3adc1345f7800bbaaaaa41a50e5c76199a34c6e56f70b3c01c6d5466f5471ce2f97ddb338160f7ccc0cd851b3c
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu3.tar.xz' lsb_11.1.0ubuntu3.tar.xz 46076 SHA512:21c6b7774aab9fddf79bfa000d4d56ee8bbd7a9e0568e00876ba8adedc6c035530f48ed10ec9838420a6a97e877b6b36148e7e1b7eec9780852da85d22547150
```

### `dpkg` source package: `lto-disabled-list=16`

Binary Packages:

- `lto-disabled-list=16`

Licenses: (parsed from: `/usr/share/doc/lto-disabled-list/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lto-disabled-list=16
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_16.dsc' lto-disabled-list_16.dsc 1435 SHA512:a1a72afe4aea37edef60fce71778f1beb3a793fe5ea67c242ef1c5f28983fb2876f18e73b2920fa88f681c049b8b6d8f0a0a14df3a53a91246d9ff36ecafcfaf
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_16.tar.xz' lto-disabled-list_16.tar.xz 11768 SHA512:e1da16ce138d1dde54759dd25517f357040c348e6e755982f5c55674d61a30b4d72d7a7a28fd15cfb93277facd68527b2bcdc08b1a437c59ea593088d12fe6ea
```

### `dpkg` source package: `lz4=1.9.3-2`

Binary Packages:

- `liblz4-1:amd64=1.9.3-2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.3-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-2.dsc' lz4_1.9.3-2.dsc 1959 SHA512:40a064f4e0fcd412b67142a792408e5bd40af14b726e7b85808421730d7bfdf9551365672b91b7dbc7544ab18590009df5503f17efc23183279622933bbd41d6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3.orig.tar.gz' lz4_1.9.3.orig.tar.gz 320958 SHA512:c246b0bda881ee9399fa1be490fa39f43b291bb1d9db72dba8a85db1a50aad416a97e9b300eee3d2a4203c2bd88bda2762e81bc229c3aa409ad217eb306a454c
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-2.debian.tar.xz' lz4_1.9.3-2.debian.tar.xz 13928 SHA512:89211662acc2db72c568ae36484f59645136412397c6fd6551ad56c5ab511c728518af49a2e927f2b84d90b8fefc2fd03ed0ecaad1f454a8e231a97dae12a0f2
```

### `dpkg` source package: `lzo2=2.10-2build1`

Binary Packages:

- `liblzo2-2:amd64=2.10-2build1`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.10-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2build1.dsc' lzo2_2.10-2build1.dsc 1975 SHA512:fc2f2c996c89c82365c037a50af68bb05561c0b0941b56ce8f12301998ec1f2a8aee43f29655193529dc0c6c87aee1fa883b9c80814765b68d0297df109cc8ae
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10.orig.tar.gz' lzo2_2.10.orig.tar.gz 600622 SHA512:a3dae5e4a6b93b1f5bf7435e8ab114a9be57252e9efc5dd444947d7a2d031b0819f34bcaeb35f60b5629a01b1238d738735a64db8f672be9690d3c80094511a4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2build1.debian.tar.xz' lzo2_2.10-2build1.debian.tar.xz 6940 SHA512:1cc531f0e1c89c7f2eab1e6e411c0d32a2f0c477bc3bd3dbc2d3830dcb43949f786ef972129e223696eda9120a50fca5b9468a76d9661052c4caf763e9827e7f
```

### `dpkg` source package: `m4=1.4.18-5ubuntu1`

Binary Packages:

- `m4=1.4.18-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-5ubuntu1.dsc' m4_1.4.18-5ubuntu1.dsc 2089 SHA512:07ff0a10145cc548d670ac0437acc264a48a9c454fb14ed9b8ec79ed79899c263f5bbc27958f211ddc5f75b74a423f8d98dd2671a37595a3fa46a5fde3d65d74
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA512:06f583efc3855cd8477d8347544f4ae5153a3e50aea74d21968afa7214784ea3ddfc02d0a2b11324120d76a19f2e804d20de11a456b5da929eb6ae469519b174
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA512:effc857a19f1496d6dde2887c0314b37d4b142a435e77614936c730878c798491ad93b28860dddd2601f99a43fa41923729b961004faafc6f798f7bc1842f980
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-5ubuntu1.debian.tar.xz' m4_1.4.18-5ubuntu1.debian.tar.xz 19064 SHA512:f724d0bb80186e5efe0a7bb587c874c352a89f8cdbc4aa12637569a59cb405971bd219e16ce67593fe933667e5e2cc00a84c264834e009a9698053ad7533b616
```

### `dpkg` source package: `make-dfsg=4.3-4ubuntu1`

Binary Packages:

- `make=4.3-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.3-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu1.dsc' make-dfsg_4.3-4ubuntu1.dsc 2147 SHA512:e1c5e4cc453a78982d26ec21ae66f0a5cda46ea3e2762d8e660065e7d430428b55416e0d6fcd259c9b55030a57f967dc662103bdad794976f9d0991ea1c01778
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA512:bdc150f9d256145923380d6e7058ab9b2b4e43fcb1d75ab2984fa8f859eab6852a68e4ea5f626633e0bec76fbebf1477378e268e8ffdb5cb2a53b29cbc439bc1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu1.diff.gz' make-dfsg_4.3-4ubuntu1.diff.gz 51058 SHA512:c2dd5be8149a60ca4a54146a25c5c4b6599172c052644d7290542b622e503f6fa1b2e5f255cfad82f068b66049778771e472e574b03202323dcbea6e71a1ec99
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

### `dpkg` source package: `mercurial=5.6.1-4`

Binary Packages:

- `mercurial=5.6.1-4`
- `mercurial-common=5.6.1-4`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=5.6.1-4
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.6.1-4.dsc' mercurial_5.6.1-4.dsc 2130 SHA512:6cdb352e69a98c23dee5a882fa196319565b95c3802784255d08d519f689854964057d1772ca54ba2ee1ead183815b80fc2b17fc64584047e5c2c1908786234c
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.6.1.orig.tar.gz' mercurial_5.6.1.orig.tar.gz 7836342 SHA512:d84d7d9ae4c738e3cb62b26c4dc7f3943abc1b1a55ccc46a4e3435896f715efb30d4d6ff4df6d02a8bef7bd6ead2d21a44342fb8a2101e8fe04211d21efc13b1
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.6.1.orig.tar.gz.asc' mercurial_5.6.1.orig.tar.gz.asc 833 SHA512:b80e92b97c1455977e9c76bb1709f0299780298d4423ad280bd92362e865e07f0ed4be1718521c1b574a70b36dbc485f71c6d6022ec99dd1114441e2e9aacf1d
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.6.1-4.debian.tar.xz' mercurial_5.6.1-4.debian.tar.xz 64588 SHA512:fbbc1a057f628feb4b745102e69fd6361780f584eb9d250e06d43e5af645d6ee566bf70ad1a94f5020b7c308e16c71a1c1e08c6f5a44fbcb617214aaec759ade
```

### `dpkg` source package: `mpclib3=1.2.0-1build1`

Binary Packages:

- `libmpc3:amd64=1.2.0-1build1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.0-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0-1build1.dsc' mpclib3_1.2.0-1build1.dsc 1875 SHA512:cc3833d855a152aa2a9725bd497108f614d39f30eb9b12f77bd40283f4d2fe44227b71ff3667b0ca27051aea465d42933822130e406847ee949c7e9d259e0699
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0.orig.tar.gz' mpclib3_1.2.0.orig.tar.gz 840711 SHA512:84fa3338f51d369111456a63ad040256a1beb70699e21e2a932c779aa1c3bd08b201412c1659ecbb58403ea0548faacc35996d94f88f0639549269b7563c61b7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0-1build1.diff.gz' mpclib3_1.2.0-1build1.diff.gz 4333 SHA512:a4962989f9b2d29706698d813997feb0bc7a20315fbf2ddc90ac511a52e6115e62dec459d0c9ae096763c82935e589082696af6690e8c2f9b48cb085ca5145d6
```

### `dpkg` source package: `mpdecimal=2.5.1-2build1`

Binary Packages:

- `libmpdec3:amd64=2.5.1-2build1`

Licenses: (parsed from: `/usr/share/doc/libmpdec3/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.5.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1-2build1.dsc' mpdecimal_2.5.1-2build1.dsc 1943 SHA512:22d558af2d71179c14b084cd3a299aff13b555ca42492958623385831fe6d418a6b7c1551c3cbf04e38460b3f562dbecc0e484fb6f2952713ef3d3d7d2b79b55
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1.orig.tar.gz' mpdecimal_2.5.1.orig.tar.gz 2584021 SHA512:710cb5cb71dbcf3e170ca15869c148df0547b848400c6b6dd70c67d9961dbe1190af8fb4d1623bfb0ca2afe44f369a42e311ab5225ed89d4031cb49a3bd70f30
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1-2build1.debian.tar.xz' mpdecimal_2.5.1-2build1.debian.tar.xz 6756 SHA512:2e61ec80853c280eff20d1644c8d275ee48d6563f2dac65ff705befcebcb9848aef7732b34afd007083f31b05ce49cea00de410444ef9ff45b64b105f0eb571c
```

### `dpkg` source package: `mpfr4=4.1.0-3build1`

Binary Packages:

- `libmpfr6:amd64=4.1.0-3build1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.1.0-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3build1.dsc' mpfr4_4.1.0-3build1.dsc 1983 SHA512:f0c886e50ac4b441bdbd7f348c438948fd1c9dba7a69cfab827971369c942f76ada59fe12ec0903fa8eac3426b7dce9ffb02177b7b0e16310fa7131fe1b7f00f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA512:1bd1c349741a6529dfa53af4f0da8d49254b164ece8a46928cdb13a99460285622d57fe6f68cef19c6727b3f9daa25ddb3d7d65c201c8f387e421c7f7bee6273
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3build1.debian.tar.xz' mpfr4_4.1.0-3build1.debian.tar.xz 12424 SHA512:1cb8790b81f42f36db85850da25695ab47673e6fbfcace1e108665274fcd6feb5ad2e66a518f779e49b1d04ff7a179fb3a6a255dee3a194c2478c62064a56114
```

### `dpkg` source package: `mysql-8.0=8.0.28-0ubuntu0.21.10.3`

Binary Packages:

- `libmysqlclient-dev=8.0.28-0ubuntu0.21.10.3`
- `libmysqlclient21:amd64=8.0.28-0ubuntu0.21.10.3`

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
$ apt-get source -qq --print-uris mysql-8.0=8.0.28-0ubuntu0.21.10.3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.28-0ubuntu0.21.10.3.dsc' mysql-8.0_8.0.28-0ubuntu0.21.10.3.dsc 3517 SHA512:4220d832cc692b4337021c78985fe7dcaf42840212132dfb72b1ac7b560a7765847fb6f4c8341e7617e4f25a05b3acb08cb4a3a99a09af7c4839280b5000b988
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.28.orig.tar.gz' mysql-8.0_8.0.28.orig.tar.gz 298044027 SHA512:4473678619a03a6c1349ce7330127f03d2da70b5b598375015abe871a0591171fc206f6e248b20085b46a0f465c52408bcadcb732ff72a737c012364d1e46297
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.28-0ubuntu0.21.10.3.debian.tar.xz' mysql-8.0_8.0.28-0ubuntu0.21.10.3.debian.tar.xz 159012 SHA512:65704eb381b2e71964650202dbc15d2f7a1ddeac6a6f322ebfcc04b6a4b6f89e57efbb9153d19f965de80ee8d653cf2e54049e75591d8df3e1bde4a868d6af3a
```

### `dpkg` source package: `mysql-defaults=1.0.5ubuntu2`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.5ubuntu2`
- `mysql-common=5.8+1.0.5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.dsc' mysql-defaults_1.0.5ubuntu2.dsc 2251 SHA512:452eb9dfdd1adc3a8e6134ae3f6d6a9d684654fd5f39727fef3ad632f046218eeaab492378565e4fa38bab40e1bc9e4765be09d4dcf303cdaf9a091f49338ace
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.tar.xz' mysql-defaults_1.0.5ubuntu2.tar.xz 7168 SHA512:6ed627ae4ac2fba44d674683e4f320ed89d44f2565c19d6e2c11206cab1f6eeab707367edbcc27f4fd54e1ef51e4637abb18d8381f4f27a344af00e1688f8cb0
```

### `dpkg` source package: `ncurses=6.2+20201114-2build1`

Binary Packages:

- `libncurses-dev:amd64=6.2+20201114-2build1`
- `libncurses5-dev:amd64=6.2+20201114-2build1`
- `libncurses6:amd64=6.2+20201114-2build1`
- `libncursesw5-dev:amd64=6.2+20201114-2build1`
- `libncursesw6:amd64=6.2+20201114-2build1`
- `libtinfo6:amd64=6.2+20201114-2build1`
- `ncurses-base=6.2+20201114-2build1`
- `ncurses-bin=6.2+20201114-2build1`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2+20201114-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2%2b20201114-2build1.dsc' ncurses_6.2+20201114-2build1.dsc 4155 SHA512:329c5e300e7c17925750a0bc7ece0582ec23cf8323ed74134e1cb7b235deb596b7f8cb8b01a80b21bb32e6d11aeb6e00e2fb9ffbe9ea0186b1139a417ce452fa
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2%2b20201114.orig.tar.gz' ncurses_6.2+20201114.orig.tar.gz 3539796 SHA512:d163bc8f08f6b2406f8f562fecd9035e0e6f2db8b539cbcaeb4a80b15027b518026526eac1b2681da82b8d03dd1c924a85de1294e6ace2a5dbc03126512a3e2c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2%2b20201114.orig.tar.gz.asc' ncurses_6.2+20201114.orig.tar.gz.asc 265 SHA512:210035a4ec94cdb650ac4cf7990791dc482ea941b410dcf635525fa3282df28464a1b8c0e5a4721868ccbe2609bae2db3632ecd166d239ef84471c536ce81f9c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2%2b20201114-2build1.debian.tar.xz' ncurses_6.2+20201114-2build1.debian.tar.xz 51936 SHA512:ba116c897b83cc0acfdc9ef0065067363d862a67e77d8f26533859ec8bd20c5d5b3ae76b573a52456dc084f206b58033f0dfc8484c3bd14da49d9c38112ab1f1
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

### `dpkg` source package: `nettle=3.7.3-1`

Binary Packages:

- `libhogweed6:amd64=3.7.3-1`
- `libnettle8:amd64=3.7.3-1`

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
$ apt-get source -qq --print-uris nettle=3.7.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3-1.dsc' nettle_3.7.3-1.dsc 2033 SHA512:7fb83ee8ced13fe7b9a0f64dda67801eeb0d277b24780259e9195a7541ee8684eb8abd669c42ce1d64ac2b726274e784a37d5a7d693c6f37bc3d4c54e59e0aed
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3.orig.tar.gz' nettle_3.7.3.orig.tar.gz 2383985 SHA512:9901eba305421adff6d551ac7f478dff3f68a339d444c776724ab0b977fe6be792b1d2950c8705acbe76bd924fd6d898a65eded546777884be3b436d0e052437
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3-1.debian.tar.xz' nettle_3.7.3-1.debian.tar.xz 21956 SHA512:0170992b41041da149b1747bd106f8ef773a4643118e5483296d9e5afbff621d4afe7d087acd2cc320b5a5f418c2a44f67c79cdd32f131be5216434350850707
```

### `dpkg` source package: `nghttp2=1.43.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.43.0-1`

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
$ apt-get source -qq --print-uris nghttp2=1.43.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.43.0-1.dsc' nghttp2_1.43.0-1.dsc 2548 SHA512:80051f361c354998f54748fa6c0623a0066999bd9160edaab29967c4d9639d03eea623a02ef19b743791c12b2a1a5274e31ccf3087ef848dc0e597bd790de477
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.43.0.orig.tar.bz2' nghttp2_1.43.0.orig.tar.bz2 4521786 SHA512:f2e6665ad6c73f0a1a8c7b34ca821a905868d41dafca913e6a054eb5afb534a85ae91618c1a4b098e43f350ca3703fd1ece7848f0a771e8393a3eb0581ceaf59
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.43.0-1.debian.tar.xz' nghttp2_1.43.0-1.debian.tar.xz 16308 SHA512:b7f895054b62531f53b2c21398c849383ca48b976ec5242716ee6f511df67fc3953968c574a4534b3da473a86a217aa92478f752757e25249f7026ec5677c8e4
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

### `dpkg` source package: `numactl=2.0.14-0ubuntu2`

Binary Packages:

- `libnuma1:amd64=2.0.14-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.14-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14-0ubuntu2.dsc' numactl_2.0.14-0ubuntu2.dsc 2165 SHA512:a7a0034fca115a982e8960e688ef22539c4e15d1c85d2bc763d70263c23634aed0e2c4265c75cc516399527e9144de3db736415fb625957d5a1c542947e1ae5b
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14.orig.tar.gz' numactl_2.0.14.orig.tar.gz 107583 SHA512:adaf405f092fd9653f26d00f8c80cb83852c56ebd5d00e714e20d505008e74aa7105b0fb7aa55a605deac0d1491ceff57de931037d33e7944fca105bc6510ed4
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14-0ubuntu2.debian.tar.xz' numactl_2.0.14-0ubuntu2.debian.tar.xz 7216 SHA512:36c3868c4c9a6bc733ec212461240e97713fed853acd4ea7582e17a26d422ffc20537dfbab436987a454a32f3c11a0b5e45c5915f6ee718f04a2ca0dc611bc73
```

### `dpkg` source package: `openexr=2.5.4-2`

Binary Packages:

- `libopenexr-dev=2.5.4-2`
- `libopenexr25:amd64=2.5.4-2`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr25/copyright`)

- `BSD-3-clause`
- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.5.4-2
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.4-2.dsc' openexr_2.5.4-2.dsc 2683 SHA512:6aea81902d984ba0acb455ae9174eac59665e57584fbc32ce9c3ccadda3e8bb5ac0b51afbf66b4fb5d00c4b1f6e720e0d5236b83cb155b770567724191ba3c54
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.4.orig.tar.gz' openexr_2.5.4.orig.tar.gz 27535491 SHA512:f0fe305987981e0c7e5a854367702585e4935ad37b0e8c10dcbc7468ae3a6d34bf963ec9ec75cc3abe4cf00e359644476b643978d0289dca46c9785a25d3f7f1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.4.orig.tar.gz.asc' openexr_2.5.4.orig.tar.gz.asc 287 SHA512:9b3978e44b531429aba42b9cc4969a470898d9d74652e3809edb0273ba9b127c471aec6570b5d352be738f59810091c0df2c70d39c16d2c32833d173b270f72c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openexr/openexr_2.5.4-2.debian.tar.xz' openexr_2.5.4-2.debian.tar.xz 21884 SHA512:42c8d6c7d1b78945cb9bd3cef35f9e74cc3fc2aab75319508845f334f01f8ec296e991e6f08fe1637d150df35d1b8f8196bbe8bd2c71f4c9452d04fb43180738
```

### `dpkg` source package: `openjpeg2=2.3.1-1ubuntu5`

Binary Packages:

- `libopenjp2-7:amd64=2.3.1-1ubuntu5`
- `libopenjp2-7-dev=2.3.1-1ubuntu5`

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
$ apt-get source -qq --print-uris openjpeg2=2.3.1-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu5.dsc' openjpeg2_2.3.1-1ubuntu5.dsc 2842 SHA512:5181a94bafe9f04a417b8e483458b4aa558fc8501d01269ad411891aeb81c88ebd17a9a7021837a8fca6feb50ba5b932969aa1eb5ce6d442dfc4b2313c91e719
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1.orig.tar.xz' openjpeg2_2.3.1.orig.tar.xz 1381768 SHA512:1346fae5f554102c46ad26e59888c693bf57b3ffaccfb5040b6c177f2ca510dd0915966d6bfd252b4293c0c098290c8e6cd923c265ca288e95e1fb7522b66b32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu5.debian.tar.xz' openjpeg2_2.3.1-1ubuntu5.debian.tar.xz 25156 SHA512:0dec70bb78cf4999a209ecb5b9c208b9b1e5336b59ccf709842efe3da10246b9458e513a03442004616ae0bfe2fcfc54012ee6053a8837dd4b70592a23b85b71
```

### `dpkg` source package: `openldap=2.5.6+dfsg-1~exp1ubuntu1`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.6+dfsg-1~exp1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.6+dfsg-1~exp1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.6%2bdfsg-1%7eexp1ubuntu1.dsc' openldap_2.5.6+dfsg-1~exp1ubuntu1.dsc 3271 SHA512:716911cf25db3768f630de553c6fcf6a433aa9e936ba21cc32234754373dfafd7428c869035e81149434ce050e07db51d9351b86ec2555ee1d524b2818139424
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.6%2bdfsg.orig.tar.gz' openldap_2.5.6+dfsg.orig.tar.gz 5570324 SHA512:f2b3c9abe53176360847563e4864eab63434671653d74b07a9ce69ff75771716d0deca58d66291c6e582f576ce6daf4588261105e307b23df0d6cdf3254d33f9
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.6%2bdfsg-1%7eexp1ubuntu1.debian.tar.xz' openldap_2.5.6+dfsg-1~exp1ubuntu1.debian.tar.xz 170828 SHA512:c5943df92305cf4f0a39c80fc48689c4eb5604399ffa636987f60e7f69788e6acb8752e51acc7a04fd9333a0b117c57849db4c52669d7c62c03f93bcbeaf9817
```

### `dpkg` source package: `openssh=1:8.4p1-6ubuntu2.1`

Binary Packages:

- `openssh-client=1:8.4p1-6ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Beer-ware`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:8.4p1-6ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1-6ubuntu2.1.dsc' openssh_8.4p1-6ubuntu2.1.dsc 3138 SHA512:91882d8873bd2ff287a6634f19621f17ed768ce145da230f12c37489cf6a2cb835ba4d1fa512e4a036a73f07f23df4c90d74dac4cff02293fc7b7e145acacdf5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1.orig.tar.gz' openssh_8.4p1.orig.tar.gz 1742201 SHA512:d65275b082c46c5efe7cf3264fa6794d6e99a36d4a54b50554fc56979d6c0837381587fd5399195e1db680d2a5ad1ef0b99a180eac2b4de5637906cb7a89e9ce
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1-6ubuntu2.1.debian.tar.xz' openssh_8.4p1-6ubuntu2.1.debian.tar.xz 181748 SHA512:1ee3683f943dc9844e05c67d0a4da430e0bfa90b666ea2dccdcc79b0cbdaf742c2832436de61f4c40136a2f662971a4f7e5c6dc990c0ecb21b36a0f9a1c4a5f9
```

### `dpkg` source package: `openssl=1.1.1l-1ubuntu1.2`

Binary Packages:

- `libssl-dev:amd64=1.1.1l-1ubuntu1.2`
- `libssl1.1:amd64=1.1.1l-1ubuntu1.2`
- `openssl=1.1.1l-1ubuntu1.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1l-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1l-1ubuntu1.2.dsc' openssl_1.1.1l-1ubuntu1.2.dsc 2745 SHA512:b786c30a74f53219580e86dac2eb0799d2892d832f6ee2e025ed91d96b3b9454b880bf20b4bd3ea76cb5b35c0bff2cc7d87e84e8e50e02ad476dc353aa3bf051
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1l.orig.tar.gz' openssl_1.1.1l.orig.tar.gz 9834044 SHA512:d9611f393e37577cca05004531388d3e0ebbf714894cab9f95f4903909cd4f45c214faab664c0cbc3ad3cca309d500b9e6d0ecbf9a0a0588d1677dc6b047f9e0
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1l.orig.tar.gz.asc' openssl_1.1.1l.orig.tar.gz.asc 488 SHA512:22f58aa49cec9e9678e56817113cccb5e1999b3148b1b3c40cf57c217d29b6bf3c7d8a4ed85b2dc865a1560095350902f7a3c78f6d4bb36ca2968740a8407aaf
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1l-1ubuntu1.2.debian.tar.xz' openssl_1.1.1l-1ubuntu1.2.debian.tar.xz 149008 SHA512:c30e1aa986793fb2693eafb230a43e48fba1ece63ff449fcdd9b09d49172f007c9cf81b015d72181eec6889ccc26e9d8d1fde054a128118bb6b991c9eda93f7f
```

### `dpkg` source package: `p11-kit=0.23.22-1build1`

Binary Packages:

- `libp11-kit0:amd64=0.23.22-1build1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.22-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22-1build1.dsc' p11-kit_0.23.22-1build1.dsc 2466 SHA512:2bf5e3f017bd3c5bc31a1e2f85186e637f66c14832101ceee2964a35019ae5e321696b6ed11fd1108846dba3a032b6f2fce968a9f0b019eb803c990891025284
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz' p11-kit_0.23.22.orig.tar.xz 830016 SHA512:098819e6ca4ad9cc2a0bc2e478aea67354d051a4f03e6c7d75d13d2469b6dc7654f26b15530052f6ed51acb35531c2539e0f971b31e29e6673e857c903afb080
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz.asc' p11-kit_0.23.22.orig.tar.xz.asc 854 SHA512:1ebb730b9c29908773de12aca89df2434576b8d9ec5da6d33db772b1e1aa4b0e8aa86ddc3e0de1abcd98a7012b5a25e3097e3a2dda2401cc37f79fd76b4f9467
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22-1build1.debian.tar.xz' p11-kit_0.23.22-1build1.debian.tar.xz 22356 SHA512:66e291cf87c29305562679391af331217cf93e227a708bdbc4ed0490c2802f0219d30a5ce47c194ed3d6b835e029a118d2cbcdb07cfa3b935b321038750ffc98
```

### `dpkg` source package: `pam=1.3.1-5ubuntu11`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu11`
- `libpam-modules-bin=1.3.1-5ubuntu11`
- `libpam-runtime=1.3.1-5ubuntu11`
- `libpam0g:amd64=1.3.1-5ubuntu11`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu11
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu11.dsc' pam_1.3.1-5ubuntu11.dsc 2757 SHA512:7452fabbb7754fa3abbcc187ecbc20d4fe14105733fa2b092d1331257afde2a05397ec1b5c111a94b100c7106c2d85b17869732da43ed24293db4496b347cf19
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA512:6bc8e2a5b64686f0a23846221c5228c88418ba485b17c53b3a12f91262b5bb73566d6b6a5daa1f63bbae54310aee918b987e44a72ce809b4e7c668f0fadfe08e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu11.debian.tar.xz' pam_1.3.1-5ubuntu11.debian.tar.xz 171476 SHA512:638aa11875b0db3c8a5b9fb639e8b702a50e26746027a86e66c005b383627f58db0f267946d5044556e61ac1ec4b9c4a39f0ca85cbd6f9bc645fff2011f05cdd
```

### `dpkg` source package: `pango1.0=1.48.10+ds1-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.48.10+ds1-1`
- `libpangocairo-1.0-0:amd64=1.48.10+ds1-1`
- `libpangoft2-1.0-0:amd64=1.48.10+ds1-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Apache-2.0`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `CC0-1.0 and, CC-BY-SA-3.0,`
- `Chromium-BSD-style`
- `Example`
- `Expat`
- `GPL-3.0`
- `GPL-3.0+`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.48.10+ds1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.48.10%2bds1-1.dsc' pango1.0_1.48.10+ds1-1.dsc 3765 SHA512:d1f1a0ecb3dd372955c36fe264e10938fb8c90715d44a7f19ff4b53fba7c7f3111a1875c213fa16a00899a60f6e7d92fdc5391d0826f1dd2a6b7647578b925bf
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.48.10%2bds1.orig.tar.xz' pango1.0_1.48.10+ds1.orig.tar.xz 721676 SHA512:e95c715e9ab45e476616df1bebde83672d0afd4c55989faf02bb9ab2a776d5e39db54cf55d7380e754bf549e531d0f19c368eec0aea7f91817acc1930608a8ac
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.48.10%2bds1-1.debian.tar.xz' pango1.0_1.48.10+ds1-1.debian.tar.xz 46588 SHA512:7dbfdc8191789a942800d71498441e20ae9bcf52e97c9246f937459179443f4504bc8128a2a47779dab01990953f81a9723a97abfedd3009c6443d65f2e4931a
```

### `dpkg` source package: `patch=2.7.6-7`

Binary Packages:

- `patch=2.7.6-7`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7.dsc' patch_2.7.6-7.dsc 1706 SHA512:80b70e71b30bb0fffc01cb1abc13cd5474b0c049b201234646f2d9a3117c8c7339264818b1633a522430c8825513a83460aab666a9590eb72a0bdc80048093f6
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA512:fcca87bdb67a88685a8a25597f9e015f5e60197b9a269fa350ae35a7991ed8da553939b4bbc7f7d3cfd863c67142af403b04165633acbce4339056a905e87fbd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7.debian.tar.xz' patch_2.7.6-7.debian.tar.xz 15084 SHA512:8c46cca63c5978edf6e40f163d5039b092d6125cfd620ab20bd7fdb04d4ea5fe6162e914719e4948d1faf7f958be8a77903344bcbb2b392e7078d9c31768a6dc
```

### `dpkg` source package: `pcre2=10.37-0ubuntu2`

Binary Packages:

- `libpcre2-16-0:amd64=10.37-0ubuntu2`
- `libpcre2-32-0:amd64=10.37-0ubuntu2`
- `libpcre2-8-0:amd64=10.37-0ubuntu2`
- `libpcre2-dev:amd64=10.37-0ubuntu2`
- `libpcre2-posix3:amd64=10.37-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.37-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.37-0ubuntu2.dsc' pcre2_10.37-0ubuntu2.dsc 2279 SHA512:ca6a68a4cd2ef3f8873d39378032ac997b479854cfa86681d7d506d0b1e3e2a9231e9197192f8f9692ed691e0840b0ac8d62c920cb880487a9a3b3239941e840
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.37.orig.tar.xz' pcre2_10.37.orig.tar.xz 1330424 SHA512:ee2acc053bedcb375f3b1ca986493dc6c4c4081ec0b7e4a263e507adcf84fba53fa1550c22108a04b73cc1ab7628c4271f972eec16ce9645158bcfd6ef6a1e52
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.37-0ubuntu2.debian.tar.xz' pcre2_10.37-0ubuntu2.debian.tar.xz 7264 SHA512:f08d80db62416ea466e6cef6a26dd6b8b499522bfec9dbd3353c746a865f0bdb0fb0e1b3fc685666790bd447fc202f1898729f5f49a9ef201ed75d9fb6dc5731
```

### `dpkg` source package: `pcre3=2:8.39-13build3`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-13build3`
- `libpcre3:amd64=2:8.39-13build3`
- `libpcre3-dev:amd64=2:8.39-13build3`
- `libpcre32-3:amd64=2:8.39-13build3`
- `libpcrecpp0v5:amd64=2:8.39-13build3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-13build3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13build3.dsc' pcre3_8.39-13build3.dsc 2133 SHA512:bb81a058b965410c21825613fb206687a46dd4186d04ac65b3eb6c0b2bf5230fa1c48a03f30d706f1714c2888855f08783b893c63db0e45c33b32816fbc6ad4f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA512:8b0f14ae5947c4b2d74876a795b04e532fd71c2479a64dbe0ed817e7c7894ea3cae533413de8c17322d305cb7f4e275d72b43e4e828eaca77dc4bcaf04529cf6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13build3.debian.tar.gz' pcre3_8.39-13build3.debian.tar.gz 26940 SHA512:2c35a015446cc3d8ed78ed254a8a212d29f398f5b5a2d643dabcb3c559e4ff3e5e44f922a5746ccd981952adf9fa6a3529ddfe3abc5d862d86380b545641aaab
```

### `dpkg` source package: `perl=5.32.1-3ubuntu3`

Binary Packages:

- `libperl5.32:amd64=5.32.1-3ubuntu3`
- `perl=5.32.1-3ubuntu3`
- `perl-base=5.32.1-3ubuntu3`
- `perl-modules-5.32=5.32.1-3ubuntu3`

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

Source:

```console
$ apt-get source -qq --print-uris perl=5.32.1-3ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1-3ubuntu3.dsc' perl_5.32.1-3ubuntu3.dsc 2968 SHA512:37416298fdb6548e3ce3a37f2d0421efbe5f1e9eab7c5e713ad777ee9da12713dc5fc222df51b39eba43b209fb4f6d9e56a67ea0802168d9d7696f508cfda767
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1.orig-regen-configure.tar.gz' perl_5.32.1.orig-regen-configure.tar.gz 871331 SHA512:c80782d17ea13cbe5592166cd8d1fcc80229eb2df39f89415ae9bf0dd2f9d3f05d554b0089fdd4d968a4ae53037cad18097289ee7ff19020eddd94db1de00fbb
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1.orig.tar.xz' perl_5.32.1.orig.tar.xz 12610988 SHA512:3443c75aea91f0fe3712fee576239f1946d2301b8f7390b690e2f5d070fe71af8f9fa7769e42086c2d33d5f84370f80368fa9350b4f10cc0ac3e6c1f6209d8f9
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1-3ubuntu3.debian.tar.xz' perl_5.32.1-3ubuntu3.debian.tar.xz 165596 SHA512:dc77d178df6336f174c4066141494152df538bebfb0f88795b5aa99b8a5f38cfbc312f546e3db3fdd15dff1bc3f5993f06e8bf80405981f43f2d43a2478e11fb
```

### `dpkg` source package: `pinentry=1.1.1-1`

Binary Packages:

- `pinentry-curses=1.1.1-1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1-1.dsc' pinentry_1.1.1-1.dsc 2216 SHA512:92f127bde177f0d3dfa013666427d087de454bf6607f091f1401858b8cf563f7938ea540a6efb7a410cdebad63e93957ee69e4ab8d970365253839948436a1dc
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1.orig.tar.bz2' pinentry_1.1.1.orig.tar.bz2 515723 SHA512:d6ab5af8ac2f3c9c05e09703e95d8e2676f9b2b7ceb97f6a31d101d0e9da7a1e106a6d3eabe86cab1bb35a4b119a7cba1380ac64bf13c61af0b3c48803116c12
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1.orig.tar.bz2.asc' pinentry_1.1.1.orig.tar.bz2.asc 390 SHA512:2b696e5a59219c6fca719d5f948d508279c483d1d2b2c99221522648fe3098da4a195aca2527fbb5b777fa2905dbda642edb5f6ac4038ed9720a5291ce282cff
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1-1.debian.tar.xz' pinentry_1.1.1-1.debian.tar.xz 19864 SHA512:2cbb0abe10c203ba6f510f8da6a1c278a9eb1e72863fc7d7d471289a3458aec671c1e9f239b504ed8af12493313a6c56d4548944c04b7e26964657debbd3126f
```

### `dpkg` source package: `pixman=0.40.0-1build2`

Binary Packages:

- `libpixman-1-0:amd64=0.40.0-1build2`
- `libpixman-1-dev:amd64=0.40.0-1build2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.40.0-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0-1build2.dsc' pixman_0.40.0-1build2.dsc 2070 SHA512:018b6711fccc285ea7faf9c5292cc8e28f62402c7f5da2c8771b4aa9e1ef8c3540bf1a8242421e171b9d67aceace6ec6765632d26a6aa70e8579387a4dbae2a7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0.orig.tar.gz' pixman_0.40.0.orig.tar.gz 913976 SHA512:063776e132f5d59a6d3f94497da41d6fc1c7dca0d269149c78247f0e0d7f520a25208d908cf5e421d1564889a91da44267b12d61c0bd7934cd54261729a7de5f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0-1build2.diff.gz' pixman_0.40.0-1build2.diff.gz 319521 SHA512:5b6ef4533670d72d74fd057eb1ebc9f0be9ea08613bd5d4b6baa6534b1f66e7f541521963c1b4d23cb368ed8432d422fe3a1f17688988dc670d9a18b6896a3c8
```

### `dpkg` source package: `pkg-config=0.29.2-1ubuntu1`

Binary Packages:

- `pkg-config=0.29.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu1.dsc' pkg-config_0.29.2-1ubuntu1.dsc 1799 SHA512:1feaf95782519c0248ddca2682c8b628aee8d5bb0a0b7b044899e30981007c824f77a76f96a1304b803136f0dd87a9dd0aef7b067cb79171ddd33c5038377e13
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2.orig.tar.gz' pkg-config_0.29.2.orig.tar.gz 2016830 SHA512:4861ec6428fead416f5cbbbb0bbad10b9152967e481d4b0ff2eb396a9f297f552984c9bb72f6864a37dcd8fca1d9ccceda3ef18d8f121938dbe4fdf2b870fe75
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu1.diff.gz' pkg-config_0.29.2-1ubuntu1.diff.gz 9852 SHA512:f569a50558520fec4450933234d33801a30f80f82d95d31aec5a91823bd55d8962ef4f63cc730923145c372da9c50e44dde836f45ed69c0ad64178c6787ef94d
```

### `dpkg` source package: `postgresql-13=13.6-0ubuntu0.21.10.1`

Binary Packages:

- `libpq-dev=13.6-0ubuntu0.21.10.1`
- `libpq5:amd64=13.6-0ubuntu0.21.10.1`

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

Source:

```console
$ apt-get source -qq --print-uris postgresql-13=13.6-0ubuntu0.21.10.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-13/postgresql-13_13.6-0ubuntu0.21.10.1.dsc' postgresql-13_13.6-0ubuntu0.21.10.1.dsc 3791 SHA512:a4b2cc106c09bf3689522b7eae25422c0163754e67dcb7a9f7267dc583405b145a87d64ab199254f516193e3e5af5696756b7f890ca22817a1332f6a890b2cda
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-13/postgresql-13_13.6.orig.tar.gz' postgresql-13_13.6.orig.tar.gz 27878427 SHA512:1db280b0a2079ef0ab7b9e74e7da7865a816358587c8aebcfe10cd6113f502c3fd3a1389ee9d5d0c9e6d4adfb38e872d5987b1bfc2aa15a0a61b4c9abe82d4be
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-13/postgresql-13_13.6-0ubuntu0.21.10.1.debian.tar.xz' postgresql-13_13.6-0ubuntu0.21.10.1.debian.tar.xz 28452 SHA512:3534f3ce5623126d9078bea19cdc136c4e1c66ebbc0e351141623a92d0ec0c223dc01b9b6f575ad06c903f63a2244ebd03dee7f42c7304724612100f37e68568
```

### `dpkg` source package: `procps=2:3.3.17-5ubuntu3`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-5ubuntu3`
- `procps=2:3.3.17-5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-5ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-5ubuntu3.dsc' procps_3.3.17-5ubuntu3.dsc 2270 SHA512:8a73bd21677c6278e29634a78d914fc6a65c95d507ff94845177aa0517e0ade3027110c41acf70829ef72ed2f5faceed4563d98a8f1b065ac612b6b7c59c92c8
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA512:59e9a5013430fd9da508c4655d58375dc32e025bb502bb28fb9a92a48e4f2838b3355e92b4648f7384b2050064d17079bf4595d889822ebb5030006bc154a1a7
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-5ubuntu3.debian.tar.xz' procps_3.3.17-5ubuntu3.debian.tar.xz 33476 SHA512:c014f5bd460b3c618bf614e7e9582046c9051cc94708df7864481e8861ad8176a519b33d6ced8ac3e2df98e45650bb0b6108897aa753ee4eb6ad69817f416fc5
```

### `dpkg` source package: `python3-defaults=3.9.4-1build1`

Binary Packages:

- `libpython3-stdlib:amd64=3.9.4-1build1`
- `python3=3.9.4-1build1`
- `python3-minimal=3.9.4-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.9.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.4-1build1.dsc' python3-defaults_3.9.4-1build1.dsc 2903 SHA512:28d8d18715dfc329986c3fc543944807c168c92aad8708d88c214cccbb65cb414cf968afbcae072e598a0841a8a0e5c2238cb68d02a6f7eb6d84dd3b79216202
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.4-1build1.tar.gz' python3-defaults_3.9.4-1build1.tar.gz 141002 SHA512:dc831ca2b5e6fe6c5648ca187c7ef71fb4c4616124a3926657a76696fb3dfd292a60e02bed332e30a4809b58ca091ed2693d371298af67f772d91ed92e2a5b92
```

### `dpkg` source package: `python3-stdlib-extensions=3.9.7-1`

Binary Packages:

- `python3-distutils=3.9.7-1`
- `python3-lib2to3=3.9.7-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.9.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.9.7-1.dsc' python3-stdlib-extensions_3.9.7-1.dsc 2577 SHA512:3a59145f964ef9880bfced3066bae5b01837ba0ba82be514b90e420ee3a2b8ebbd61da4d80f72d8965c2de1e104cd09daf84e3336a596448a6b23226fe47acc5
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.9.7.orig.tar.xz' python3-stdlib-extensions_3.9.7.orig.tar.xz 1101088 SHA512:633d91f0ecb5e575e571e761496797a597bc4e7ee4a2d053b0d22c89fc12e946fb44df2f99e28927f55ca8f8720801bb228c86358f67e12429aafe28d39c3c97
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.9.7-1.debian.tar.xz' python3-stdlib-extensions_3.9.7-1.debian.tar.xz 24500 SHA512:880e93a3aa15d1e1ce6957b08998e78be7e1aebb117b32b7628a299e46fb289064abbec9ed4eed613d318109acd0a8b87a13943732ba69668d141540905df81e
```

### `dpkg` source package: `python3.9=3.9.7-2build1`

Binary Packages:

- `libpython3.9-minimal:amd64=3.9.7-2build1`
- `libpython3.9-stdlib:amd64=3.9.7-2build1`
- `python3.9=3.9.7-2build1`
- `python3.9-minimal=3.9.7-2build1`

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

Source:

```console
$ apt-get source -qq --print-uris python3.9=3.9.7-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.7-2build1.dsc' python3.9_3.9.7-2build1.dsc 3517 SHA512:49d267daf401bb33993f51781718a1e49b4229948dfc45d0ca0b4084c6edfcb5178fc6f23ca203ef116eb87e5a52cce220952edf3775d509de4bd7ffc56654a3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.7.orig.tar.xz' python3.9_3.9.7.orig.tar.xz 19123232 SHA512:55139776ab58a40f9e1e70613d7071d559ef9e51e32a77791422aac134322c21a49f0348c42813214b69789c589367eae43e16d4ae838a73daf37617e966b735
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.7-2build1.debian.tar.xz' python3.9_3.9.7-2build1.debian.tar.xz 212148 SHA512:47dfb2c388b0305c32eac94d4f24b8b2e1777d06e152c0066e80dc21865e830973a916613908268fdd218564ecac086551a523eb074fa1bf8a4a6e4dddae8186
```

### `dpkg` source package: `readline=8.1-2`

Binary Packages:

- `libreadline-dev:amd64=8.1-2`
- `libreadline8:amd64=8.1-2`
- `readline-common=8.1-2`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-2.dsc' readline_8.1-2.dsc 2418 SHA512:032340de3dc9d4cf0c601ef149b640c48619d1096cfafe34e8cfc79eb46ca3617ac0147f327a0dea6cc24dce6ffd89f821217700ea14352fbc7d5b7111857722
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.orig.tar.gz' readline_8.1.orig.tar.gz 2993288 SHA512:27790d0461da3093a7fee6e89a51dcab5dc61928ec42e9228ab36493b17220641d5e481ea3d8fee5ee0044c70bf960f55c7d3f1a704cf6b9c42e5c269b797e00
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-2.debian.tar.xz' readline_8.1-2.debian.tar.xz 29800 SHA512:d32debb1e3847d34cac592cebcc12208f10243ec766eb4c9a60bf203ba5cda5c449c91682e4ee6983d6c68d4dd458944b328e64d39fa782f34636bfe03bdaaff
```

### `dpkg` source package: `rpcsvc-proto=1.4.2-0ubuntu5`

Binary Packages:

- `rpcsvc-proto=1.4.2-0ubuntu5`

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
$ apt-get source -qq --print-uris rpcsvc-proto=1.4.2-0ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-0ubuntu5.dsc' rpcsvc-proto_1.4.2-0ubuntu5.dsc 2109 SHA512:7c9568bb56c7a4a27fbad9c0104dc8776d1e5fc9668a44316822d6305a672676df4c9d064939e9233163e544b46aec188f2aebebc9fed5ce0733b302545b289b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2.orig.tar.xz' rpcsvc-proto_1.4.2.orig.tar.xz 171620 SHA512:631fbfc00af94c5d7def0759f27e97dc14d400b4468c906719ae18ecef74815730798c882d1aaa4f90359224e7b829019b786baddc3097905b54f940ca85a714
'http://archive.ubuntu.com/ubuntu/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.2-0ubuntu5.debian.tar.xz' rpcsvc-proto_1.4.2-0ubuntu5.debian.tar.xz 4208 SHA512:fb38fa8f21c5c17a3055dbf8750db16b02aa77a671a2075f01535fc38f0b30f8d4eb563d6d3200e7d477fc28be1ef2cbbf2e749e8a5b06f23db564f6e94e0bdd
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2build3`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2build3`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2build3
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2build3.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build3.dsc 2427 SHA512:d88c3302e6f5fcaece5673963c9d0b1f9295c7240d1d227444de9108a87a0ac4f90b1cd6af790b6497ee82457db9502f02299ab8585dfcaf1c9196065b412cd6
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA512:bdfcbab73179d614a295a7b136ea4c9d0ce4620883b493f298362784d245608cd6ad4b0ad30f94ed73a086b4555399521ae9e95b6375fce75e455ae68c055e7b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2build3.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build3.debian.tar.xz 8324 SHA512:96c84a3c9d660a87e063e1140b51422250844fa959a00be7a9142a3fbed033f46845d9ba05cb8f083194d7cef9d6b6f49cfa9d05c2ef99c9561c802e92c15149
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


### `dpkg` source package: `shadow=1:4.8.1-1ubuntu9`

Binary Packages:

- `login=1:4.8.1-1ubuntu9`
- `passwd=1:4.8.1-1ubuntu9`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1ubuntu9
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu9.dsc' shadow_4.8.1-1ubuntu9.dsc 2345 SHA512:8d69095b60dc2211e1a98c1a9229fdf57a6e9aa115a378b2440dd7eabf760548e0143685d2f8244290b75e3fe472900d907a263be30e37fa6a7dbb485186ec29
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA512:780a983483d847ed3c91c82064a0fa902b6f4185225978241bc3bc03fcc3aa143975b46aee43151c6ba43efcfdb1819516b76ba7ad3d1d3c34fcc38ea42e917b
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu9.debian.tar.xz' shadow_4.8.1-1ubuntu9.debian.tar.xz 86872 SHA512:89d9d4c33598252e3df47b69e30424edea9743c6033fcf296a6a8ce2b450f9ea67008a3a79a5667a775eedf58320fd25fff83eb9e613e34ac9a88601c2c96930
```

### `dpkg` source package: `shared-mime-info=2.1-1`

Binary Packages:

- `shared-mime-info=2.1-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=2.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.1-1.dsc' shared-mime-info_2.1-1.dsc 2223 SHA512:2baa4bc272270bb312a077a17e9b840a85f5cd6dcee3f17d648283e35bf3194c268801b6001d6ed0ec5ff81f3eea984a99784fdb451dda3740ef74d1aa83bc7a
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.1.orig.tar.xz' shared-mime-info_2.1.orig.tar.xz 5202496 SHA512:87e308281e83c4cf889594f7c2e8dcb4d0d0d3910124c3816fdb886ba7d6113b2581711adcb17032b47f9b8d8b7001fab58daa52b7da7c0ef87915e341d6f1b0
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.1-1.debian.tar.xz' shared-mime-info_2.1-1.debian.tar.xz 10036 SHA512:ac307cb5cf525984faf80e4530671db319e2f35bcdcd83b2bdebfb5a4a9d709ea1a5719980816457ac2bbf3de83273179432342a113ff9deb4454a08668df622
```

### `dpkg` source package: `sqlite3=3.35.5-1`

Binary Packages:

- `libsqlite3-0:amd64=3.35.5-1`
- `libsqlite3-dev:amd64=3.35.5-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.35.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.35.5-1.dsc' sqlite3_3.35.5-1.dsc 2410 SHA512:e45de7358521a0583bac5543ae2cbf22991521ce6d005634d1c06aa533b18e4e1cd17cf63aa58db96a5093c97725632a4efa687b3ebe20a2e446109d4b535bc6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.35.5.orig-www.tar.xz' sqlite3_3.35.5.orig-www.tar.xz 5589276 SHA512:2de026d9d5b2704b4905a6a5e5cfbf72bf633f862d79f545dc696ac37b273712d52b544e5d6c0117ff69efba013f6069822a4422db375273c781ca585450430e
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.35.5.orig.tar.xz' sqlite3_3.35.5.orig.tar.xz 7485512 SHA512:c096be33a001d6eb6760c1c72a74864865d5d190799f17fdcc42e2ad81c61574d11586f5a917792ccd8a218071b5cf14d352ce15e473f0e2e34ef61fa7224661
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.35.5-1.debian.tar.xz' sqlite3_3.35.5-1.debian.tar.xz 21776 SHA512:24de55d890b3d618eea95d496f9c29fefb0ab61eb4c83e3b9ab6367b9766dccc6d38c870b08575f73038a822e694185e78055635fd9899813df2960bbf50ce2e
```

### `dpkg` source package: `subversion=1.14.1-3`

Binary Packages:

- `libsvn1:amd64=1.14.1-3`
- `subversion=1.14.1-3`

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
$ apt-get source -qq --print-uris subversion=1.14.1-3
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1-3.dsc' subversion_1.14.1-3.dsc 3807 SHA512:0e81ee3a1e999c85b7c5c958ddf79a37926838d4ba019c38cb55604b107146900431b36f32ae08fcd2301327d54f080010a5994db4da3755017089509bb858df
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1.orig.tar.gz' subversion_1.14.1.orig.tar.gz 11534165 SHA512:6cd780f6669c811264de03b94ea41487111957dfd817498699c91e5dbb975e4b9626de9c436c5722fd6a6fadc4fef35f51905c2c0f5fd4955cf0fadef9cba60e
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1.orig.tar.gz.asc' subversion_1.14.1.orig.tar.gz.asc 1288 SHA512:56f3b3ae63e10c503b741107261da955088749845693b34125f8e61c7850035021684b31944e99ed50628cc4f601081627c1472f83f8196eac3a289038a842f9
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1-3.debian.tar.xz' subversion_1.14.1-3.debian.tar.xz 430084 SHA512:faf0da8d7291b52b18cb5969f72e74342af1cd98b4d3982cf7cbb7c63842dff627a2368ea2650539cefab1f8a5c2f41e91129feae3697fae0c345defe4ade7a9
```

### `dpkg` source package: `systemd=248.3-1ubuntu8.2`

Binary Packages:

- `libsystemd0:amd64=248.3-1ubuntu8.2`
- `libudev1:amd64=248.3-1ubuntu8.2`

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
$ apt-get source -qq --print-uris systemd=248.3-1ubuntu8.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_248.3-1ubuntu8.2.dsc' systemd_248.3-1ubuntu8.2.dsc 5066 SHA512:c948c9eac6c96b6e4360aac6adae7aaef390cee68eee4e9ec361b08546517930a8f0d4429bd5c6250000a4b37ce677ebea15fe4f5c83c95c628c80b1debb47c3
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_248.3.orig.tar.gz' systemd_248.3.orig.tar.gz 10320940 SHA512:8e7ff0d5e63cc933e4dc23f7e0bef9707fde90396605eb8822d34de90d7abe8fd37e5739e33b657868218aa7281147cc944c096c007324c3e6fb54d833a83485
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_248.3-1ubuntu8.2.debian.tar.xz' systemd_248.3-1ubuntu8.2.debian.tar.xz 219532 SHA512:2cad42212692bd36c433b85bf87db23391d7aec0e88d0d0f6dddd6ccd4015ec23f433b367279dd02bf7e87b65fcfc8fd211b4e353e9f88bb973fda97a169b29c
```

### `dpkg` source package: `sysvinit=2.96-7ubuntu1`

Binary Packages:

- `sysvinit-utils=2.96-7ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-7ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-7ubuntu1.dsc' sysvinit_2.96-7ubuntu1.dsc 2730 SHA512:61638e41c102b87ad0d0453d4aa2356e978b0e54a8b99aebd88725dde602ec848b187d436db6e95b90ae8d2432e9b5ce465e3902f93f74a6283dfeaa8fb77e23
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA512:1388398568ebfe53460796f8ab75a3ead6111612888ea36e8f1c0db4d41ef6f45fc217abb7804519ff1143a78d97c95b24e42c8c22c95a47b9436484bfb6f45d
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA512:2b3798e8fc8531cd1a2b2a523159b7f064bfadd8815b930fb70d5a1380775f1b5bac5627d5cd9d95b03ff3737d8d6b2f357c6bc21ac2e21ee089b67f98b4eb6a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-7ubuntu1.debian.tar.xz' sysvinit_2.96-7ubuntu1.debian.tar.xz 129644 SHA512:033caf3ee6e2b59dbf7c3939622bf804c287d329b7ca056982fae7ee3c8e66b7a9ff0933af2f3425a03edbd5f9328bb0aefaf7331a759f32f8e454866bcc7b0d
```

### `dpkg` source package: `tar=1.34+dfsg-1build1`

Binary Packages:

- `tar=1.34+dfsg-1build1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1build1.dsc' tar_1.34+dfsg-1build1.dsc 2093 SHA512:3251c52ed6f0e3dc2b89f61a6f0dbf28c04170c5c18ebee5a2b035e02ba876b89bf45d60c6eda6f26f86211465e9aafc6b715592077d6f9120ed8cbcafd70cbb
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA512:ec5553c53c4a5f523f872a8095f699c17bf41400fbe2f0f8b45291ccbaf9ac51dea8445c81bd95697f8853c95dcad3250071d23dbbcab857a428ee92e647bde9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1build1.debian.tar.xz' tar_1.34+dfsg-1build1.debian.tar.xz 19296 SHA512:50378351a260ca81aa2e68994bd37fbfbd35e3b8c9d8c07cfe2b8424edb0da64c40283cca625af95a8a4abe4483bf5c205727fc35dda13773d2ddaead4f9fb24
```

### `dpkg` source package: `tiff=4.3.0-1`

Binary Packages:

- `libtiff-dev:amd64=4.3.0-1`
- `libtiff5:amd64=4.3.0-1`
- `libtiffxx5:amd64=4.3.0-1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0-1.dsc' tiff_4.3.0-1.dsc 2429 SHA512:975d082a13c450020e55bbcdb8ff1bf19d51d758186585f0549d99be0084636b4b26a797215714dbf7758d6c38ea550865cc218a6c4165634014f671685093a9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz' tiff_4.3.0.orig.tar.gz 2808254 SHA512:e04a4a6c542e58a174c1e9516af3908acf1d3d3e1096648c5514f4963f73e7af27387a76b0fbabe43cf867a18874088f963796a7cd6e45deb998692e3e235493
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz.asc' tiff_4.3.0.orig.tar.gz.asc 488 SHA512:115a4c5714b52d0fbea800c494d83c8a96b70b2c9ce84a8df03205d9afc517faa17963f5f9508c013d7d3e2be6675b84b594a771a829406473234c4bd85e469e
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0-1.debian.tar.xz' tiff_4.3.0-1.debian.tar.xz 19588 SHA512:847b7f4f9eb50b96484c54e6802aa0168d7470e5a1e94fed234e7038187530dc8f45d54601dd18b0f44329503f63999d4210c2bdce87685f52decd82d9f79c2c
```

### `dpkg` source package: `tzdata=2021e-0ubuntu0.21.10`

Binary Packages:

- `tzdata=2021e-0ubuntu0.21.10`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

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

### `dpkg` source package: `unzip=6.0-26ubuntu1`

Binary Packages:

- `unzip=6.0-26ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-26ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-26ubuntu1.dsc' unzip_6.0-26ubuntu1.dsc 1840 SHA512:29bbd06d1f8b56e2908f29597bddf3da350549aede9eb874fe2e165da59d5c9fc0397984a51f6b06ac31053c07f126a0895ff4a2dce2b3c6724bde509e5dceec
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA512:0694e403ebc57b37218e00ec1a406cae5cc9c5b52b6798e0d4590840b6cdbf9ddc0d9471f67af783e960f8fa2e620394d51384257dca23d06bcd90224a80ce5d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-26ubuntu1.debian.tar.xz' unzip_6.0-26ubuntu1.debian.tar.xz 26944 SHA512:b5cda0f09d51a88bdfdd025d321f343b85966d588ca8821203788651cb9da424d1c1ec7d951c83dcc41529d519f53803ba8bd5a4a6c27f9b4ecd8516e5127064
```

### `dpkg` source package: `usrmerge=25ubuntu1.1`

Binary Packages:

- `usrmerge=25ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/usrmerge/copyright`)

- `GPL v2`
- `GPL-2`
- `later (please see /usr/share/common-licenses/GPL-2)`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=25ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_25ubuntu1.1.dsc' usrmerge_25ubuntu1.1.dsc 1622 SHA512:161e74f0f1489da7bdd94f2caf8391b2b3cdc52f07da5df22745ab51ec86c1cf9cd553997d2bc76ad3b2fb4c1d0058b5aadf5290080ed2d42bdad71318e4ba95
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_25ubuntu1.1.tar.xz' usrmerge_25ubuntu1.1.tar.xz 12820 SHA512:e955c63783536ca5177290b8302a8b21bc3f48d2b66fdcb7090c95e21b8cc8cde22e9885364279b0c0117504c519e07b5aaf8bc8f07dc12b9d6aa708496bb906
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

### `dpkg` source package: `util-linux=2.36.1-8ubuntu2.2`

Binary Packages:

- `bsdutils=1:2.36.1-8ubuntu2.2`
- `libblkid-dev:amd64=2.36.1-8ubuntu2.2`
- `libblkid1:amd64=2.36.1-8ubuntu2.2`
- `libmount-dev:amd64=2.36.1-8ubuntu2.2`
- `libmount1:amd64=2.36.1-8ubuntu2.2`
- `libsmartcols1:amd64=2.36.1-8ubuntu2.2`
- `libuuid1:amd64=2.36.1-8ubuntu2.2`
- `mount=2.36.1-8ubuntu2.2`
- `util-linux=2.36.1-8ubuntu2.2`
- `uuid-dev:amd64=2.36.1-8ubuntu2.2`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid-dev/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount-dev/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.36.1-8ubuntu2.2
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1-8ubuntu2.2.dsc' util-linux_2.36.1-8ubuntu2.2.dsc 4479 SHA512:0133890a12cf4e7419e11f5fe892a47068ffdef08640caca5bbe6a4f20d1ffb4a29f5cac42385daec82d661cdc7cbf197aee51e94de4f0456c2673fcffc66848
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1.orig.tar.xz' util-linux_2.36.1.orig.tar.xz 5231880 SHA512:9dfd01ae4c16fa35015dafd222d555988b72e4d1d2fbadd140791b9ef78f84fa8254d4d08dc67cabf41e873338867f19e786b989d708ccfe5161c4f7679bba7a
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1-8ubuntu2.2.debian.tar.xz' util-linux_2.36.1-8ubuntu2.2.debian.tar.xz 107024 SHA512:cb048520cf6745ab704905d83c36c430d4cf46159859558f30e3673b66787f30be143510375a43784c0bc5a1f539ebd71e2c1043108e9b5acaac53f1adfc56cb
```

### `dpkg` source package: `wget=1.21-1ubuntu3`

Binary Packages:

- `wget=1.21-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21-1ubuntu3.dsc' wget_1.21-1ubuntu3.dsc 1608 SHA512:0ca4783df06b8dd2e35c39ff7e8b0eb750aabdb6135456bbacfd730b78ab1abf93338d615b40ddfc8e99d808b7b463e54365850bdb1a29d4681b763db4ba2bb0
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.orig.tar.gz' wget_1.21.orig.tar.gz 4866788 SHA512:13313a98f91ef34ad90103f076285549eb4887d77953e9f192d3b0667642b5ceb9e2e30091f766cbf1d6ed423499c497ed85d826f3f3e92f0711aa06d8303c5a
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.orig.tar.gz.asc' wget_1.21.orig.tar.gz.asc 854 SHA512:1bdaedc164800158625fddbc842c2cbe246d3e3c2f07546ecebacc8c1ea44779aab31a707d792f965669f2403941d4869e59719198563a0f39099145609310d1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21-1ubuntu3.debian.tar.xz' wget_1.21-1ubuntu3.debian.tar.xz 63472 SHA512:2f6b9607f6c160c412eaee1151ea4245090d4e983bc3b674066adddebf3fdb40248bf01ae2c16676007ef06d0c83b51158c2411382af4f2a334d4e6ca9cfdfb8
```

### `dpkg` source package: `x265=3.4-2`

Binary Packages:

- `libx265-192:amd64=3.4-2`

Licenses: (parsed from: `/usr/share/doc/libx265-192/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=3.4-2
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_3.4-2.dsc' x265_3.4-2.dsc 2229 SHA512:47a9abf37d23c13e18884071d4fe6bcd9c37f69c31d2b3bce2f0c80d027c5480ebed510d1a98de4d2313fa6def07424089ddfd504bbd2d8ad0cfb46946c0b4a3
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_3.4.orig.tar.gz' x265_3.4.orig.tar.gz 1469365 SHA512:576b18711935e7da8433b2170d24ed159eb12ff1a18399360afa1b2132db33b463145c65ed918f667528ee954bbdfb5c69e5480f1c1df801515cefc592f3206e
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_3.4-2.debian.tar.xz' x265_3.4-2.debian.tar.xz 13076 SHA512:bb4b7aa10e9ada765d599f588dc79858359d1d1d8f4b01e31af955cd87e311a4d37b5a82b6cbb563c763048945cddec9607b55d58617606db6fda375217982af
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

### `dpkg` source package: `xorg=1:7.7+22ubuntu2`

Binary Packages:

- `x11-common=1:7.7+22ubuntu2`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+22ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7%2b22ubuntu2.dsc' xorg_7.7+22ubuntu2.dsc 2091 SHA512:0eca3590e290f16995b962c9df7c692761e2702c3bce1e50babedf106ded02ca2e5c1a6f8d8319aab027f1d42a8d762a7f8500a11d7bab6970a5d595f6f1dbae
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7%2b22ubuntu2.tar.gz' xorg_7.7+22ubuntu2.tar.gz 295592 SHA512:07df24783074af43b989f0deebcbb9e95cc2d640432d424e2663242654c7d888eef8c4f36a1025b10c9bf19cbf9d67cb28f0ffc2ab975409172ad998bd0fb739
```

### `dpkg` source package: `xorgproto=2020.1-1`

Binary Packages:

- `x11proto-dev=2020.1-1`
- `x11proto-xext-dev=2020.1-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-dev/copyright`, `/usr/share/doc/x11proto-xext-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2020.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1-1.dsc' xorgproto_2020.1-1.dsc 3410 SHA512:657d90d91061a1ce0d48ead6d6b5b072219289939a9b84c496eea98dea008b0b665c8bb9c3cd8a6f4d4017a5978cd38257c81844d26d524740ccf7560d668fc5
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1.orig.tar.gz' xorgproto_2020.1.orig.tar.gz 1081369 SHA512:d0bc3aec517fd00fa5fd32a5715760c34810a19154e10fb1f92f2e2fe7f26136f7ba9b76b47fcd37c3c4796663154f4e5abf6a18dd634619b0f718f3e4737ae9
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1.orig.tar.gz.asc' xorgproto_2020.1.orig.tar.gz.asc 659 SHA512:5932a8525ca3032d61b87ef8f69b5ff8997da095eebfcb3400fa5ce6a97413a7161a794b8dfac16475ee56154348ff62c1eba02b2dd191f8e89bf12f2056bfbe
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2020.1-1.diff.gz' xorgproto_2020.1-1.diff.gz 20627 SHA512:7213ab21dda33bb416e74ecd18ed569670b44a064f76ea2f5ccfcd3fcbdccaf232842d376559694cde3b7753cf4b0b1279e423219c4640d4d2d8f941eff14ddb
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

### `dpkg` source package: `xxhash=0.8.0-2build1`

Binary Packages:

- `libxxhash0:amd64=0.8.0-2build1`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0-2build1.dsc' xxhash_0.8.0-2build1.dsc 1995 SHA512:6370d766c660d3e932ce8c80c3b648e17122ed8014a1662a9fc763a87aec16f8d820ab9d62138bf61b0c0485089a34071a8159ef2c39bba368e78749878b7e66
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0.orig.tar.gz' xxhash_0.8.0.orig.tar.gz 145909 SHA512:c3973b3c98bad44e1d8687ab4f9461aecd1c071bb3d320537a4c50fb7301edd13e990bab48cc6e5ca30536a814c8fa8cac24ceb1803a7e8eca30ef73d449373e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0-2build1.debian.tar.xz' xxhash_0.8.0-2build1.debian.tar.xz 4244 SHA512:ce631e18514cbc9607b5ec6f6ab5e4ca32452d7766d8f68dfbecfdd5c27597e040662650a4fe1ace750b27676d0a02259b351e4525f77575ec0ee98d074e578c
```

### `dpkg` source package: `xz-utils=5.2.5-2`

Binary Packages:

- `liblzma-dev:amd64=5.2.5-2`
- `liblzma5:amd64=5.2.5-2`
- `xz-utils=5.2.5-2`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.dsc' xz-utils_5.2.5-2.dsc 2312 SHA512:5ccb4f20c29ad6935d8673f306329af29a29086652cc24c10a73e31b2ee06dcbc9410eb4b944c3ba403cf78de06b7bdd5480b3c1b6bfdd382ae654cb1a759a29
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA512:59266068a51cb616eb31b67cd8f07ffeb2288d1391c61665ae2ec6814465afac80fec69248f6a2f2db45b44475af001296a99af6a32287226a9c41419173ccbb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz.asc' xz-utils_5.2.5.orig.tar.xz.asc 833 SHA512:582864ae306861ede34074ebfd23ab161ad3340ab4a068f727583de2bd2058da70dfe73019f4e70b8267e0e0c62f275da1e23f47d40c0b80038449b0ac335020
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.debian.tar.xz' xz-utils_5.2.5-2.debian.tar.xz 33532 SHA512:2a645ab7aeccec5141d0ac0475d2f6eb3f9253397ad0fa1227ec8b20e14ae720649884278e9a7f860fbb07c30f3192a88a41ba39459a062461f2c6bd1acc6762
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu7`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu7`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2ubuntu7`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu7
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu7.dsc' zlib_1.2.11.dfsg-2ubuntu7.dsc 2945 SHA512:956709508bde7e163129ae35cf5cdac8752510400b0b6404ce0b96529f107836b81268a58f0693a12b51c02251d48316aec0d8e2f3edeab33c7e6f5e94508137
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu7.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu7.debian.tar.xz 54844 SHA512:c3245d9d6c1325a3d176750e232ff2920264d79ec51501e3a6cc1ec2c87ed30ff5d36489dbf1ff867581a3c253ddc596c07f6575147f84726c831af54e86e834
```
