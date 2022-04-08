# `buildpack-deps:impish-scm`

## Docker Metadata

- Image ID: `sha256:a2f1fd74ccad0cedab23a1a01b44a44b9cd4d14952738747ab6566cc2df35178`
- Created: `2022-04-05T22:48:11.677360135Z`
- Virtual Size: ~ 214.06 Mb  
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

### `dpkg` source package: `brotli=1.0.9-2build3`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2build3`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

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

- `libbz2-1.0:amd64=1.0.8-4ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

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

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8ubuntu1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8ubuntu1`

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

### `dpkg` source package: `dpkg=1.20.9ubuntu2`

Binary Packages:

- `dpkg=1.20.9ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

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

- `e2fsprogs=1.46.3-1ubuntu3`
- `libcom-err2:amd64=1.46.3-1ubuntu3`
- `libext2fs2:amd64=1.46.3-1ubuntu3`
- `libss2:amd64=1.46.3-1ubuntu3`
- `logsave=1.46.3-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

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

### `dpkg` source package: `expat=2.4.1-2ubuntu0.3`

Binary Packages:

- `libexpat1:amd64=2.4.1-2ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.4.1-2ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.1-2ubuntu0.3.dsc' expat_2.4.1-2ubuntu0.3.dsc 2096 SHA512:7f8c7c2d36ea20d941fc30b0f8029239716c95a26317f805ff0d0a8d503a2d61d2b9ba3ca2e1850ed0d1cce045341874d12d68104057cd0074bf5bea5ad85fe5
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.1.orig.tar.gz' expat_2.4.1.orig.tar.gz 8307804 SHA512:1f08861e9b766fdbbc40159404a3fe1a86451d635ef81874fa3492845eda83ac2dc6a0272525891d396b70c9a9254c2f6c907fe4abb2f8a533ccd3f52dae9d5a
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.4.1-2ubuntu0.3.debian.tar.xz' expat_2.4.1-2ubuntu0.3.debian.tar.xz 26116 SHA512:fd58c4788f11c5c670e3ca91784dd0a672905a96bbf3877132b33bcb0fefea8028c600deecd698c4019771ee6a4542605d78e1fd5beda795e5ae835b10210195
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

### `dpkg` source package: `gcc-11=11.2.0-7ubuntu2`

Binary Packages:

- `gcc-11-base:amd64=11.2.0-7ubuntu2`
- `libgcc-s1:amd64=11.2.0-7ubuntu2`
- `libstdc++6:amd64=11.2.0-7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

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

### `dpkg` source package: `gdbm=1.19-2`

Binary Packages:

- `libgdbm-compat4:amd64=1.19-2`
- `libgdbm6:amd64=1.19-2`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

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

### `dpkg` source package: `glibc=2.34-0ubuntu3.2`

Binary Packages:

- `libc-bin=2.34-0ubuntu3.2`
- `libc6:amd64=2.34-0ubuntu3.2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

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

- `libgmp10:amd64=2:6.2.1+dfsg-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

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

- `libgssapi-krb5-2:amd64=1.18.3-6`
- `libk5crypto3:amd64=1.18.3-6`
- `libkrb5-3:amd64=1.18.3-6`
- `libkrb5support0:amd64=1.18.3-6`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.18.3-6
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3-6.dsc' krb5_1.18.3-6.dsc 3636 SHA512:2824f0ed6c98e1bc38322c83ca7733e6d996b677247c43f25abfabcb79405af4a3c9b323db80829bdd56f058ce5122f3792a31688a4dc5d13484f70d3a595101
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz' krb5_1.18.3.orig.tar.gz 8715312 SHA512:cf0bf6cf8f622fa085954e6da998d952cf64dc7ccc319972ed81ea0542089cabf2d0e8243df84da01ad6f40584768ca2f02d108630c6741fa7b3d7d98c887c01
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz.asc' krb5_1.18.3.orig.tar.gz.asc 833 SHA512:7c5a83e13d00910d895d545ed63310ebec48c90c29846dd54e48048f710360e8306778729b636baa091a4e9048998ff6d4dfe37f88dd6292540d55678c961a30
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3-6.debian.tar.xz' krb5_1.18.3-6.debian.tar.xz 105116 SHA512:0a8654cb4bd923e3fbe653e0403f93ea13b23321022db6f7471d4dabb685d651f60c7fc2eb4c5d805177205e444eaa5e9fd246cb822e67f41825ee93bd7327eb
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

### `dpkg` source package: `libffi=3.4.2-1ubuntu5`

Binary Packages:

- `libffi8:amd64=3.4.2-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libffi8/copyright`)

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

- `libnsl2:amd64=1.3.0-2build1`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build1.dsc' libnsl_1.3.0-2build1.dsc 2004 SHA512:3881693bdbc58ac4c926fa31e543e417cc75f0294c5dbcafb2a550f0e207f18fc39f860c6080b5cbb8d0e883669d0c9b0a3b95fbd921cb884ac9c9c684452bd5
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA512:a5a6c3ccb2d1e724c8c1f65e55dcd09383eb1ae019c55f4c09441eadf23ffbc2196cfad259805b0ac40ddf3a10af0da453e4d739d67d46829c64d0995dab4e55
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2build1.debian.tar.xz' libnsl_1.3.0-2build1.debian.tar.xz 4772 SHA512:6d83aff8aa0e32a6e7ccabda6923ec3d13def4b1dc641aa66217d63b3c4b232311720e5e713af8e9bc3ddbe70f7b1fa7d7d159576eceae16045cdbe0bb06c526
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

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1ubuntu2.dsc' libsepol_3.1-1ubuntu2.dsc 2150 SHA512:ef1d2e5c03dfaab2895570e0798894dac489ea0ccd6c05d38b0db1ed418a0b8090c5432cc6a81325c9bc1ae2f3ee97e957a098d9842129d69125c1e0b381d3a4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA512:4b5f4e82853ff3e9b4fac2dbdea5c2fc3bb7b508af912217ac4b75da6540fbcd77aa314ab95cd9dfa94fbc4a885000656a663c1a152f65b4cf6970ea0b6034ab
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1ubuntu2.debian.tar.xz' libsepol_3.1-1ubuntu2.debian.tar.xz 14812 SHA512:b76a2dc19431d19295fb5841ad9ddf92ad42c8a851b23e7df932ad71d5e4a2dc4865d5e0bdd5438f5b88a127b9e3fc79a8134361fdb16d7360bbd1c095b22b5c
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

### `dpkg` source package: `libtirpc=1.3.2-2`

Binary Packages:

- `libtirpc-common=1.3.2-2`
- `libtirpc3:amd64=1.3.2-2`

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
$ apt-get source -qq --print-uris libtirpc=1.3.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2.dsc' libtirpc_1.3.2-2.dsc 2111 SHA512:f7b3f3d948f0aa417f40f41c769780b70dda4bbd7d421da4515a0b69c525809b4a182edd91f64187efe9b7c581ddfc1f5ec4c14a29bb738849181cbb324abcc1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2.orig.tar.bz2' libtirpc_1.3.2.orig.tar.bz2 513151 SHA512:8664d5c4f842ee5acf83b9c1cadb7871f17b8157a7c4500e2236dcfb3a25768cab39f7c5123758dcd7381e30eb028ddfa26a28f458283f2dcea3426c9878c255
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.2-2.debian.tar.xz' libtirpc_1.3.2-2.debian.tar.xz 10996 SHA512:742916905b6fa8b5a41d151cac18a7bb2eaa7571675ed486907ffba71b23871165db9d08578469caa61a33c677adcfb04309211a86aa815a88952fc87e572a78
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

### `dpkg` source package: `libxcrypt=1:4.4.18-4ubuntu1`

Binary Packages:

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

### `dpkg` source package: `libzstd=1.4.8+dfsg-2.1`

Binary Packages:

- `libzstd1:amd64=1.4.8+dfsg-2.1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

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

### `dpkg` source package: `ncurses=6.2+20201114-2build1`

Binary Packages:

- `libncurses6:amd64=6.2+20201114-2build1`
- `libncursesw6:amd64=6.2+20201114-2build1`
- `libtinfo6:amd64=6.2+20201114-2build1`
- `ncurses-base=6.2+20201114-2build1`
- `ncurses-bin=6.2+20201114-2build1`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

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

### `dpkg` source package: `pcre2=10.37-0ubuntu2`

Binary Packages:

- `libpcre2-8-0:amd64=10.37-0ubuntu2`

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

- `libpcre3:amd64=2:8.39-13build3`

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

- `libreadline8:amd64=8.1-2`
- `readline-common=8.1-2`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-2.dsc' readline_8.1-2.dsc 2418 SHA512:032340de3dc9d4cf0c601ef149b640c48619d1096cfafe34e8cfc79eb46ca3617ac0147f327a0dea6cc24dce6ffd89f821217700ea14352fbc7d5b7111857722
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.orig.tar.gz' readline_8.1.orig.tar.gz 2993288 SHA512:27790d0461da3093a7fee6e89a51dcab5dc61928ec42e9228ab36493b17220641d5e481ea3d8fee5ee0044c70bf960f55c7d3f1a704cf6b9c42e5c269b797e00
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1-2.debian.tar.xz' readline_8.1-2.debian.tar.xz 29800 SHA512:d32debb1e3847d34cac592cebcc12208f10243ec766eb4c9a60bf203ba5cda5c449c91682e4ee6983d6c68d4dd458944b328e64d39fa782f34636bfe03bdaaff
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

### `dpkg` source package: `sqlite3=3.35.5-1`

Binary Packages:

- `libsqlite3-0:amd64=3.35.5-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

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

### `dpkg` source package: `tzdata=2022a-0ubuntu0.21.10`

Binary Packages:

- `tzdata=2022a-0ubuntu0.21.10`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2022a-0ubuntu0.21.10
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022a-0ubuntu0.21.10.dsc' tzdata_2022a-0ubuntu0.21.10.dsc 2109 SHA512:791803108bf78de40f37a88abae520d98c5a162e3123a79ce22af8d734501af64844aa0d1113f0880d52a4f5cea7e69d63d33444fcbbb0fad255683ac45322ab
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022a.orig.tar.gz' tzdata_2022a.orig.tar.gz 425833 SHA512:542e4559beac8fd8c4af7d08d816fd12cfe7ffcb6f20bba4ff1c20eba717749ef96e5cf599b2fe03b5b8469c0467f8cb1c893008160da281055a123dd9e810d9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2022a-0ubuntu0.21.10.debian.tar.xz' tzdata_2022a-0ubuntu0.21.10.debian.tar.xz 166404 SHA512:b1244bf30de0ec0bc2fd207e7a0b4170d3e31bcb0e0798a1f55904edae384f786054a70450ace1f43d674e894a8b93e95315c2bc7048507f81042e4bf4ba3594
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
- `libblkid1:amd64=2.36.1-8ubuntu2.2`
- `libmount1:amd64=2.36.1-8ubuntu2.2`
- `libsmartcols1:amd64=2.36.1-8ubuntu2.2`
- `libuuid1:amd64=2.36.1-8ubuntu2.2`
- `mount=2.36.1-8ubuntu2.2`
- `util-linux=2.36.1-8ubuntu2.2`

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

- `liblzma5:amd64=5.2.5-2`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.dsc' xz-utils_5.2.5-2.dsc 2312 SHA512:5ccb4f20c29ad6935d8673f306329af29a29086652cc24c10a73e31b2ee06dcbc9410eb4b944c3ba403cf78de06b7bdd5480b3c1b6bfdd382ae654cb1a759a29
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA512:59266068a51cb616eb31b67cd8f07ffeb2288d1391c61665ae2ec6814465afac80fec69248f6a2f2db45b44475af001296a99af6a32287226a9c41419173ccbb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz.asc' xz-utils_5.2.5.orig.tar.xz.asc 833 SHA512:582864ae306861ede34074ebfd23ab161ad3340ab4a068f727583de2bd2058da70dfe73019f4e70b8267e0e0c62f275da1e23f47d40c0b80038449b0ac335020
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2.debian.tar.xz' xz-utils_5.2.5-2.debian.tar.xz 33532 SHA512:2a645ab7aeccec5141d0ac0475d2f6eb3f9253397ad0fa1227ec8b20e14ae720649884278e9a7f860fbb07c30f3192a88a41ba39459a062461f2c6bd1acc6762
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu7.1`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu7.1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu7.1
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu7.1.dsc' zlib_1.2.11.dfsg-2ubuntu7.1.dsc 2953 SHA512:0258ee599d6da169e67f0bda6318a51e700dd05eac2845df4da06974e819791f4f145d6459b2cf2194d64356bf4bb2f680d8aa6cb208eca95e4cab93d8055e5a
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu7.1.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu7.1.debian.tar.xz 58516 SHA512:86b7cca1125aafcabfd9f2474944576e1333e3682d68a8159b22a3c6de8245e6553d1f57e4556d3eb55551ab2f5a30bcb88876931870d00f29a9b0cd8ca15234
```
