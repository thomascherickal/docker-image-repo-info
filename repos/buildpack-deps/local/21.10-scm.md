# `buildpack-deps:impish-scm`

## Docker Metadata

- Image ID: `sha256:948855c3898acffc9373d4d4a43be0300cc8eb82948ba6447f467fc4b9f4572b`
- Created: `2021-06-25T21:49:53.058668423Z`
- Virtual Size: ~ 221.04 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-10ubuntu1`

Binary Packages:

- `libacl1:amd64=2.2.53-10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-10ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-10ubuntu1.dsc' acl_2.2.53-10ubuntu1.dsc 2521 SHA512:f82999d73f8f1bf0b1bce498f8c3e37fd28569989070c2897e25a9a5cb8cfa13ea4ff30313020062eb0a903c74f40b30201eee5b57d139bd49aef4d672227b3a
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA512:176b7957fe0e7618e0b7bf2ac5071f7fa29417df718cce977661a576fa184e4af9d303b591c9d556b6ba8923e799457343afa401f5a9f7ecd9022185a4e06716
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA512:a76dcc4f9952bb809aed3c8e0d26e9ae1aa8098ec8492c4d95a23ab74ec92d6896f1eb6307a555098277aa1191cc01d75a2f6a35dd8e8ccb46d3155404bc6f22
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-10ubuntu1.debian.tar.xz' acl_2.2.53-10ubuntu1.debian.tar.xz 25644 SHA512:fc59c4f46886643ac24cb76e642158e3d4180a64ca5424208ae749cd43b36add764a4dc616480b38a5f4ebecbe4beeba86c1938602dd0c453179436cfd10472c
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

### `dpkg` source package: `apr-util=1.6.1-5ubuntu1`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu1.dsc' apr-util_1.6.1-5ubuntu1.dsc 2644 SHA512:82969ab0267ea55a687b097f1b48b5161b54fd453e409cd6f67d8a2ffee66dd7edc7eb0c3b4c7fa3264c666b6cc4c116ec74a891157e721bbe520acafaf0939c
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA512:40eff8a37c0634f7fdddd6ca5e596b38de15fd10767a34c30bbe49c632816e8f3e1e230678034f578dd5816a94f246fb5dfdf48d644829af13bf28de3225205d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu1.debian.tar.xz' apr-util_1.6.1-5ubuntu1.debian.tar.xz 342724 SHA512:d31ced761628d2b2535daeea88537f4818f1bb242f3842a955255c74925c453607eb8895fad31e0d7f3cf5c2054ac5ecc4c51296a9da3bada3a98ea01ead46df
```

### `dpkg` source package: `apr=1.7.0-6`

Binary Packages:

- `libapr1:amd64=1.7.0-6`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-6
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-6.dsc' apr_1.7.0-6.dsc 2250 SHA512:32b84f507be86d63a1f71531060058777ec630d07fbc587e3e5d2cb8f08b2db4793e2e4e0463ada9f2845ff4c208f8328df9fece5b61fa02afeacce7c926cca8
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA512:3dc42d5caf17aab16f5c154080f020d5aed761e22db4c5f6506917f6bfd2bf8becfb40af919042bd4ce1077d5de74aa666f5edfba7f275efba78e8893c115148
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA512:19b2b128c7c4cb40db06149c75325013a716c783e28e366c1bacf289fdb5d305e5779d8dc55a63729250ad3338cd4c726e133c788fe53ab3519f1bc8d4da6f90
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-6.debian.tar.xz' apr_1.7.0-6.debian.tar.xz 214280 SHA512:9ab10688afdf5e32911b1feb35f8caaa58a8533bc1dabdebf6d6a1a9439bd59fd07504c81a0edc9d08e0e8b54af2e3713a8adae08fa2a0f6ba2f4c616d6d3a8e
```

### `dpkg` source package: `apt=2.3.5`

Binary Packages:

- `apt=2.3.5`
- `libapt-pkg6.0:amd64=2.3.5`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.3.5/


### `dpkg` source package: `attr=1:2.4.48-6build1`

Binary Packages:

- `libattr1:amd64=1:2.4.48-6build1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.48-6build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6build1.dsc' attr_2.4.48-6build1.dsc 2482 SHA512:099ac327a747ddb50fc8ff279ed2215e1bb00fb9b5fdac61e951f33a3a8e515b737e6658f630033c5ed35c013dfebf24b7bb351c49b1d710b9d7a24514df5786
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA512:75f870a0e6e19b8975f3fdceee786fbaff3eadaa9ab9af01996ffa8e50fe5b2bba6e4c22c44a6722d11b55feb9e89895d0151d6811c1d2b475ef4ed145f0c923
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA512:39e5879d4879003ba5e1fcb727f91f7661cede12692ae128110328a6c1c5a1e2f79a1329ee4d065f3cc3e0d3d18423f5b5a5b170b5cb49c6888de90d31dcaf9c
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-6build1.debian.tar.xz' attr_2.4.48-6build1.debian.tar.xz 27332 SHA512:eed6bb2b3869a23ab89c0349bb1bd1b7c51fb2f225291d49d08c19aa501af81e2fa650b46a5369bb87011413236eacc91b1f468d33630d6af5e3cf12adc68084
```

### `dpkg` source package: `audit=1:3.0-2ubuntu1`

Binary Packages:

- `libaudit-common=1:3.0-2ubuntu1`
- `libaudit1:amd64=1:3.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0-2ubuntu1.dsc' audit_3.0-2ubuntu1.dsc 2811 SHA512:ec7cdd23daf0653cb61830c22a21bc48625ff4bb977fcc06ff8d3c3b1763006501aa83734e9579c2ff08b9c316aba7907eb0823dc770289cd41c53638f074fcf
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.orig.tar.gz' audit_3.0.orig.tar.gz 1109442 SHA512:b82ec73c85a8ebb5108b526673d6fe08cbe0b51376788f3ea6ed5747c4612158462893e719496dffbd723f833f84383a2d1d55fd78a3ed985ecfd19545060c88
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0-2ubuntu1.debian.tar.xz' audit_3.0-2ubuntu1.debian.tar.xz 21228 SHA512:e9b798e0be2e8cbc4e935f210e0b3902c2d08a12887f4a0dbcb9b02bd481b4294c1fa6287eb3411c8b11b18142b2fd0e9675c0bcbf3cf9e4c6977ebd46d5be5e
```

### `dpkg` source package: `base-files=11.1ubuntu3`

Binary Packages:

- `base-files=11.1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11.1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11.1ubuntu3.dsc' base-files_11.1ubuntu3.dsc 1598 SHA512:ba748f56e4eff7ae50b48be52298da3fc8b98608a47573623bed82384cff3d8469d767ca3d5a401bc898bcde6ddc7587d5927ba80634141d7f69e4065dc57f7d
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11.1ubuntu3.tar.xz' base-files_11.1ubuntu3.tar.xz 81536 SHA512:503d09daa68d0426236b9a201227c1e56085d847a356c676e6f35ee5451195aa954263fe6fa414c30de8b23f87a7da1e49ff041ff7543a151037d8ac940b864b
```

### `dpkg` source package: `base-passwd=3.5.50`

Binary Packages:

- `base-passwd=3.5.50`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.50
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.50.dsc' base-passwd_3.5.50.dsc 1757 SHA512:e681a55510895fa8fda1ec8f489b7b85e5cf989684ed88eeb52d1e0e2eca5aa25619ec12905319c2c6db2b9155dcf3d4efe090fc0483c312d923482b0e238199
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.50.tar.xz' base-passwd_3.5.50.tar.xz 53836 SHA512:ad6d270d84d693739881ace50bd8166a827e8f5beeb70b78f3ecce610e1e85a79b96b95f7dcd8fb56bd8393b51a0587c66e7aee80145a9ba4827eb2ee528f1aa
```

### `dpkg` source package: `bash=5.1-3ubuntu1`

Binary Packages:

- `bash=5.1-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.1-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-3ubuntu1.dsc' bash_5.1-3ubuntu1.dsc 2426 SHA512:b999404130f3fa2eeec91f4d2cf0f4b4c06748c30506af6f4f01a8e336156b6bc27de5535cba6c0d98164f50786c2ac89770c8bc925c8a09ca707bdd861ff129
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1.orig.tar.xz' bash_5.1.orig.tar.xz 5802740 SHA512:95d3acc542231cb893e1347c7d9dd66687f68cd347a0e9e126fde2d14e68c5b5530d1a5866eafa781e88aa013fcf72b4ad56d2e484c2ac7a69bd90bb149a9b86
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.1-3ubuntu1.debian.tar.xz' bash_5.1-3ubuntu1.debian.tar.xz 98316 SHA512:f85071421d1d09c57bea4bf05329fb2c625337d68d768a88b3aea3a716543e7e68f8e89480d18f7a0f29364fea1de97b46e178cb8d006f97d7fe0227aa8ae411
```

### `dpkg` source package: `brotli=1.0.9-2build2`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2build2`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build2.dsc' brotli_1.0.9-2build2.dsc 2310 SHA512:89c6d31a94ad22663e962582df7545c421141ace6dd70a68e7b9d4de35368a850bb5fd33c6df4bac157fa2fa77b9ad9da81fc2219a643846293c0eed85c5cfee
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build2.debian.tar.xz' brotli_1.0.9-2build2.debian.tar.xz 5652 SHA512:0e2cef83495d666e0dd2aaee5017f4a534bbe115d3274ea01dd5b722b429dca8485c3011583e6fac3f9da378f14d3f409d5c2265b47f01db8028401946222e5b
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

### `dpkg` source package: `ca-certificates=20210119build1`

Binary Packages:

- `ca-certificates=20210119build1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20210119build1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20210119build1.dsc' ca-certificates_20210119build1.dsc 1766 SHA512:f1c899115c920aa773d60434058b5dab1a15ade1cca41e0ff49bf57b6c2d2b7096d654fa3a44b7177c343ba08c722d634d6239cf552ee02edba4a1a8cf9208b6
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20210119build1.tar.xz' ca-certificates_20210119build1.tar.xz 232812 SHA512:019ad4500019668a61854f08b4880464b11150c51b792278af8978a4c2e9e5913e9922790c52a19254c99bfe21f4a02a36cab6804584627601c94f2428e7939b
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

### `dpkg` source package: `curl=7.74.0-1.2ubuntu2`

Binary Packages:

- `curl=7.74.0-1.2ubuntu2`
- `libcurl3-gnutls:amd64=7.74.0-1.2ubuntu2`
- `libcurl4:amd64=7.74.0-1.2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.74.0-1.2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.74.0-1.2ubuntu2.dsc' curl_7.74.0-1.2ubuntu2.dsc 2771 SHA512:c2b4ec483942c0bf82bbef2e6c9d9433d9c672cc5c64c1f9c34978bb94d47890095ec4049996d1077c36d30263ed0057ef28c6c88d67d1b545b8f8b9472963c5
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.74.0.orig.tar.gz' curl_7.74.0.orig.tar.gz 4043409 SHA512:4b61a23463315dce5529aa5f1dc7d21d7876347912c68855c9cfcb01e06492af1510975fafb213c67ac7b9764287767da69043a79376a4be366aa23ace09f163
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.74.0-1.2ubuntu2.debian.tar.xz' curl_7.74.0-1.2ubuntu2.debian.tar.xz 38776 SHA512:f74521ca06564a8b9994f2a875845b49ea324411e2fb6e57d4278a0f9acd49a98882075681669190c33cc4d9b2faa46657be7173d91f983041df0b70e8b89b9c
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2.1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.1.dsc' cyrus-sasl2_2.1.27+dfsg-2.1.dsc 3433 SHA512:cb391becb2f584e00faed4bea9c2de4c21493e839d41822f3ed2181b4ddb8966b65e7909fb6b412a978fe3b851b3f41ecd2155af3bb4556a19ea1c6e48797fe6
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA512:a795e4362f85a50e223c5456d03526832eb29fdbc9e17a767045f8542638e3f987d382b79b072bcd694bd1a12cbb818cff6c326063ca2bbe05453c1acf7fb8ad
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.1.debian.tar.xz 101356 SHA512:ea34d0b770c8b59f42e93157071e51f97afdb6dc177eb633360fcdf1d24103dc5107d6fbf7a38e905f17120c33c9d0d59e21c0a8b2fddbbb17621fd6dc502f6e
```

### `dpkg` source package: `dash=0.5.11+git20210120+802ebd4-1`

Binary Packages:

- `dash=0.5.11+git20210120+802ebd4-1`

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
$ apt-get source -qq --print-uris dash=0.5.11+git20210120+802ebd4-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20210120+802ebd4-1.dsc' dash_0.5.11+git20210120+802ebd4-1.dsc 1646 SHA512:0e1e02dac87bbb55cc69e7ebdc632ebc82d0b12e91478ad6e56c65205b74a778ea2d2671f6f085396a410ad8afbac33c18d980ebe94c7df50f2254840901679c
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20210120+802ebd4.orig.tar.xz' dash_0.5.11+git20210120+802ebd4.orig.tar.xz 133332 SHA512:076a59f6b0eb4c01ab6f51382fe242079b51b41ee2354140659861b9cb1b19b5a84752509ee4510f834b5e8ba5ccae5cc28f470e5ddea97cef811a02bd9274e7
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20210120+802ebd4-1.debian.tar.xz' dash_0.5.11+git20210120+802ebd4-1.debian.tar.xz 42504 SHA512:08f51e0e6b68d3a922be6ed67f782bcb43c3adeca8f9a4a22c6a06ac93de2a3efa80874ba6feb86be250310464fe168afb048065b534b58ada222d0dc72a57f3
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8ubuntu1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8ubuntu1.dsc' db5.3_5.3.28+dfsg1-0.8ubuntu1.dsc 3220 SHA512:f7df482fb21791cdf06e966c7c812fa6b9270c3ad86dfe4ff0a08b514c46491cbafeb114aa106f3e66e9839422481f56112c9dff9e764f3cbff032a45547a83c
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA512:50cb87bc3f24065839ee2932e82af032b236b290ebe89983076f503c6c62c5f36ff93d7847a3f68b2b19f35088fbab5d3ac6a34553d07e8148e68e9a3f079a12
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8ubuntu1.debian.tar.xz' db5.3_5.3.28+dfsg1-0.8ubuntu1.debian.tar.xz 31912 SHA512:83e8592b218688627248d7a41f4432834f1ba7f76605d71bcc550bf63886789fad2ff31bd9a8734afe353a267cc91129933628d160bacb6451e72fde253c787d
```

### `dpkg` source package: `debconf=1.5.76`

Binary Packages:

- `debconf=1.5.76`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debconf/1.5.76/


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

### `dpkg` source package: `diffutils=1:3.7-5ubuntu1`

Binary Packages:

- `diffutils=1:3.7-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.7-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-5ubuntu1.dsc' diffutils_3.7-5ubuntu1.dsc 2203 SHA512:e033e0f3dee1ef38c9fbec818045f888496c2908f3ce64f248d54bd15af4d4a6459d13e003ccdcdc558c352ae610b5dc3db2a7af50c5752a3dc1a3c5aa69ed0d
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz' diffutils_3.7.orig.tar.xz 1448828 SHA512:7b12cf8aea1b9844773748f72272d9c6a38adae9c3c3a8c62048f91fb56c60b76035fa5f51665dceaf2cfbf1d1f4a3efdcc24bf47a5a16ff4350543314b12c9c
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz.asc' diffutils_3.7.orig.tar.xz.asc 833 SHA512:3e7e6ae735f930d8249fb0cb6913937fb03783f0fb3de44473e22b134d2452a7d9a2f733ef63b91548976482d85d25af2a2d07e06ca22195b3d816e51e4e0ab6
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-5ubuntu1.debian.tar.xz' diffutils_3.7-5ubuntu1.debian.tar.xz 89736 SHA512:7fc0502d8eca59ac2905c1dd56411efd00f29c33941a299bdcb3d96f5b743b8a11575305686dc06287b522b755c2f2a105186c9580524815a016bbdb39381f1b
```

### `dpkg` source package: `dpkg=1.20.9ubuntu1`

Binary Packages:

- `dpkg=1.20.9ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `e2fsprogs=1.46.2-1ubuntu2`

Binary Packages:

- `e2fsprogs=1.46.2-1ubuntu2`
- `libcom-err2:amd64=1.46.2-1ubuntu2`
- `libext2fs2:amd64=1.46.2-1ubuntu2`
- `libss2:amd64=1.46.2-1ubuntu2`
- `logsave=1.46.2-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.2-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.2-1ubuntu2.dsc' e2fsprogs_1.46.2-1ubuntu2.dsc 3203 SHA512:2d926007d383fbb9430d144f5263a68d559b819dd0580453481cf10ed05e7700bf9426ec5ccef171ef6d5b06a63f583fbe028f462a40056d64fdd1196448ab6c
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.2.orig.tar.gz' e2fsprogs_1.46.2.orig.tar.gz 9496954 SHA512:cdf03e0e5190073dbd9c0d0cd0fea66cc8ed462a789b018b39c45c0dcbbe268992851603035e8e9afb9c3d8cedd1d3550ec27d179b2dca3db629ddc148db4d76
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.2.orig.tar.gz.asc' e2fsprogs_1.46.2.orig.tar.gz.asc 488 SHA512:9d0355c2070a5906ee129a6eca1707bb0a93361c3cec09c6ee63982bcace9a6336381a55dce862fc43b0ebf9e490afab0c0b4e1d56daebcb06b44f55ff915ed2
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.2-1ubuntu2.debian.tar.xz' e2fsprogs_1.46.2-1ubuntu2.debian.tar.xz 85832 SHA512:8be2f38e44e698f10d40645dd150251ff55acfb8761b4c68531794dd2a5f1dde721ff1dc1dada9a568ce7a6a9291a01074543c0bca4905784d8a516e6625b49d
```

### `dpkg` source package: `expat=2.3.0-1`

Binary Packages:

- `libexpat1:amd64=2.3.0-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.3.0-1.dsc' expat_2.3.0-1.dsc 1981 SHA512:a33b683b5df6cd9c4de5295dde86a75921d2611431ffbc6ea6132002bb5e235df3de4eeeac0d9baec44771e800a3b5628de60e41d2603f8c526039a7d1997f06
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.3.0.orig.tar.gz' expat_2.3.0.orig.tar.gz 8283476 SHA512:728ceb1d912fabc7662d4201828dc29c7fdaff124a1d6dc81434b1951eb530b17f1bbb1aec22c1520543cff3844f4751f29d3c59b696dd8a56598abdc25e1d08
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.3.0-1.debian.tar.xz' expat_2.3.0-1.debian.tar.xz 11024 SHA512:332b66d19ae430456d0f508d970794766368f3f7759a8ea608e50ca14bed43f80df9b9a9621a2a389c6a52497c7c369e66b5eb167c6ba9bdeec3ecc94f8f5d94
```

### `dpkg` source package: `findutils=4.8.0-1ubuntu1`

Binary Packages:

- `findutils=4.8.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.8.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0-1ubuntu1.dsc' findutils_4.8.0-1ubuntu1.dsc 2409 SHA512:0386a8d5ca33514092937709d1c0748af8504d84f157edacfb73f627117eb5416755635634b041041956e795e3adeb79b71618aab0116ac60c92f3b283bd4383
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz' findutils_4.8.0.orig.tar.xz 1983096 SHA512:eaa2da304dbeb2cd659b9210ac37da1bde4cd665c12a818eca98541c5ed5cba1050641fc0c39c0a446a5a7a87a8d654df0e0e6b0cee21752ea485188c9f1071e
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0.orig.tar.xz.asc' findutils_4.8.0.orig.tar.xz.asc 488 SHA512:e6ea8bd9a58ac4f787a9cc7dad9f75fab9e0623e7cda463bef60651c9319574ac7c8ba06f7d33cbead0ecb8788db71eb39f50550deb066d6d6baa625b0374a45
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.8.0-1ubuntu1.debian.tar.xz' findutils_4.8.0-1ubuntu1.debian.tar.xz 27588 SHA512:5a30569ce48d1bdb5215c765b15d5cca96f026db2841c883e2275a9429d21be909d1ed7da8a104de5db6b9555b8acd8d82d64e85cb17d76090fa3409240a20f0
```

### `dpkg` source package: `gcc-11=11.1.0-2ubuntu1`

Binary Packages:

- `gcc-11-base:amd64=11.1.0-2ubuntu1`
- `libgcc-s1:amd64=11.1.0-2ubuntu1`
- `libstdc++6:amd64=11.1.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `git=1:2.31.1-1ubuntu1`

Binary Packages:

- `git=1:2.31.1-1ubuntu1`
- `git-man=1:2.31.1-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.31.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.31.1-1ubuntu1.dsc' git_2.31.1-1ubuntu1.dsc 2986 SHA512:5cf3d828215d8c339294128335c549b3f4cd977bd65b274abb4341c97bb07140bacadf62f7f7bd2b19983fbc68dfc1775204a3cb8842edaa73462f92ca88deb2
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.31.1.orig.tar.xz' git_2.31.1.orig.tar.xz 6413368 SHA512:9aa334a3e8519700ff5d112153ec42677722980094caa9d22aa91afdb65166bd9a98fa445c0d327c428ebfa73bf4832e9b3836109a1d9319feafe3191cfd170e
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.31.1-1ubuntu1.debian.tar.xz' git_2.31.1-1ubuntu1.debian.tar.xz 678776 SHA512:c1235d7c143951479ab9160ef26aa088eed6362e109cbf0b6f35942ce15d2f7a62027eef3c78535a8e59a1fbb5307898d69efad6328d3ae4268949531eba6773
```

### `dpkg` source package: `glibc=2.33-0ubuntu7`

Binary Packages:

- `libc-bin=2.33-0ubuntu7`
- `libc6:amd64=2.33-0ubuntu7`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.33-0ubuntu7
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.33-0ubuntu7.dsc' glibc_2.33-0ubuntu7.dsc 8982 SHA512:4c197b97a9998afb4747e2b6fe97c0711965a66e56a8b5c8e1737759c8450204526841d88b23aded6ff6c6edfae82ac134b39e9b9e8a7da39a0bb36ba8ac943e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.33.orig.tar.xz' glibc_2.33.orig.tar.xz 17031280 SHA512:4cb5777b68b22b746cc51669e0e9282b43c83f6944e42656e6db7195ebb68f2f9260f130fdeb4e3cfc64efae4f58d96c43d388f52be1eb024ca448084684abdb
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.33.orig.tar.xz.asc' glibc_2.33.orig.tar.xz.asc 833 SHA512:a1cf64161aa5b97f04c89ff3f94a8de9b01f1115ca36905416c5018b212dfde85fa8751026d0743fbefb554880bae19fe551bbde4c8fe1d50e69db3cf5c014c1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.33-0ubuntu7.debian.tar.xz' glibc_2.33-0ubuntu7.debian.tar.xz 893396 SHA512:3317a4431db081ab61a383c30eec089c29069ac47fc25cf8ec571bad923cca7540e0f9bcd20bbd645e75280c26a97b3d3755338c223e1aca109ba7e3624b8abc
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1+dfsg-1ubuntu2.dsc' gmp_6.2.1+dfsg-1ubuntu2.dsc 2256 SHA512:2fd6a3a95e4bfc997d01a5af7e1b19d737538960e73d78c75c53e233afd3967a50335abde6024848a60d07c5fae53b27d7bcf8a0c8acddac144e403cbd5d08d6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1+dfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA512:801948b7dcf592959ea387a86bee34dfb4e02c5e93815a785fc46174899ba22129853a3e34109a6df86048a144765c5f39e65fddfcecba879cc60da62f32fea0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1+dfsg-1ubuntu2.debian.tar.xz' gmp_6.2.1+dfsg-1ubuntu2.debian.tar.xz 43744 SHA512:32ee0629d2769fe687dbd3731e546f115bd1d4f644dcbc9392b0addc58982758126c08c51ab6a7c46f047d6f4a0a42632f216704ecf0d5f0a6670f0a6c8bd8b2
```

### `dpkg` source package: `gnupg2=2.2.20-1ubuntu3`

Binary Packages:

- `dirmngr=2.2.20-1ubuntu3`
- `gnupg=2.2.20-1ubuntu3`
- `gnupg-l10n=2.2.20-1ubuntu3`
- `gnupg-utils=2.2.20-1ubuntu3`
- `gpg=2.2.20-1ubuntu3`
- `gpg-agent=2.2.20-1ubuntu3`
- `gpg-wks-client=2.2.20-1ubuntu3`
- `gpg-wks-server=2.2.20-1ubuntu3`
- `gpgconf=2.2.20-1ubuntu3`
- `gpgsm=2.2.20-1ubuntu3`
- `gpgv=2.2.20-1ubuntu3`

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
$ apt-get source -qq --print-uris gnupg2=2.2.20-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu3.dsc' gnupg2_2.2.20-1ubuntu3.dsc 3959 SHA512:8466131be3765e7445f60c8ad4d684c9e87e97872974608096581127a920e95c2619cc3169d24aa8363563c777630a65aa36cbf1f46deb0006eac829ecb881e0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2' gnupg2_2.2.20.orig.tar.bz2 6786913 SHA512:3e69f102366ec3415f439ab81aae2458182fa1a18dfb86565b1d9dc638f3fc4c179a5947f0042b7c5a813345676285a662793664a1803ea9ad8328f0548e0edc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2.asc' gnupg2_2.2.20.orig.tar.bz2.asc 1357 SHA512:0972788af253f84959ab3142e3d4bf025b7e7077377574e69851ae3d37cbf296211fdf50cd77fe47f844bc3383489ff88cf35186d2f72cb0adc84cdfe77bfd26
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu3.debian.tar.xz' gnupg2_2.2.20-1ubuntu3.debian.tar.xz 64860 SHA512:5e01aa7c5b9b5c37e99743547be2c167fb1d75071ae47dd9f43b7767821adcb47a8671f25144bf921673854ef8c6762a15f9db7a3f247e12267170b7f0d6785b
```

### `dpkg` source package: `gnutls28=3.7.1-4ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.1-4ubuntu1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.1-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1-4ubuntu1.dsc' gnutls28_3.7.1-4ubuntu1.dsc 3594 SHA512:07be127e313c190cadc93f99346fa0d754427a4de2827fbb4f5975f3d26ea7582cf7248ce85d63a4bc6731cbfe7a92781776574e84402129d14b0be6d87e52aa
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1.orig.tar.xz' gnutls28_3.7.1.orig.tar.xz 6038388 SHA512:0fe801f03676c3bd970387f94578c8be7ba6030904989e7d21dffdc726209bab44c8096fbcb6d51fed2de239537bd00df2338ee9c8d984a1c386826b91062a95
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1.orig.tar.xz.asc' gnutls28_3.7.1.orig.tar.xz.asc 854 SHA512:72101722be460c3092ff602dbf7246e81172a8aa2f7a9eba73a76536d00798cf58ab8a6d90b79cdb29f4c5f65ca0129d2f4e22e46dd66f4cee9e4a559b72d546
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.1-4ubuntu1.debian.tar.xz' gnutls28_3.7.1-4ubuntu1.debian.tar.xz 83592 SHA512:e1ef74d81d726e82e52f1cffab12d1773597ef6bd04ca29a96377277ae82fdeed7aa0af4d617d71ce7c74ff89c8090f1cc9d6e5e6dad70bd1a6beb99a796d5b0
```

### `dpkg` source package: `grep=3.6-1`

Binary Packages:

- `grep=3.6-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6-1.dsc' grep_3.6-1.dsc 1644 SHA512:df414b678efc2cc78b275594bad61ce2e657ff7b52af57eddb22795c11043f70f1b699e63b4e2c48f8be15a44cdc026f19dc793b4d2ee85c62e0421caadf1b08
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6.orig.tar.xz' grep_3.6.orig.tar.xz 1589412 SHA512:8934544a19ded61344d83ff2cab501e86f17f8ae338892e0c36c2d2d8e63c76817840a0071ef5e3fcbca9115eba8a1aae0e4c46b024e75cd9a2e3bd05f933d90
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6.orig.tar.xz.asc' grep_3.6.orig.tar.xz.asc 833 SHA512:0cdf0078d10fda8aecc434f35148fa18378dd160002d745fb960fe506aedfcdab379ba5aeff9e692becd05b7717033401bd7d92b1aabe151b47561682669a3cd
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.6-1.debian.tar.xz' grep_3.6-1.debian.tar.xz 17748 SHA512:cf35da621f88880c03c41d1f174fd1a091630552f264340a86801c2603ebe189671ed1120466a53710cb94659d0b1b2124bd4f00d33c11dd0e7a5d3d905cf46c
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

### `dpkg` source package: `heimdal=7.7.0+dfsg-2`

Binary Packages:

- `libasn1-8-heimdal:amd64=7.7.0+dfsg-2`
- `libgssapi3-heimdal:amd64=7.7.0+dfsg-2`
- `libhcrypto4-heimdal:amd64=7.7.0+dfsg-2`
- `libheimbase1-heimdal:amd64=7.7.0+dfsg-2`
- `libheimntlm0-heimdal:amd64=7.7.0+dfsg-2`
- `libhx509-5-heimdal:amd64=7.7.0+dfsg-2`
- `libkrb5-26-heimdal:amd64=7.7.0+dfsg-2`
- `libroken18-heimdal:amd64=7.7.0+dfsg-2`
- `libwind0-heimdal:amd64=7.7.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libasn1-8-heimdal/copyright`, `/usr/share/doc/libgssapi3-heimdal/copyright`, `/usr/share/doc/libhcrypto4-heimdal/copyright`, `/usr/share/doc/libheimbase1-heimdal/copyright`, `/usr/share/doc/libheimntlm0-heimdal/copyright`, `/usr/share/doc/libhx509-5-heimdal/copyright`, `/usr/share/doc/libkrb5-26-heimdal/copyright`, `/usr/share/doc/libroken18-heimdal/copyright`, `/usr/share/doc/libwind0-heimdal/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `custom`
- `none`

Source:

```console
$ apt-get source -qq --print-uris heimdal=7.7.0+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.dsc' heimdal_7.7.0+dfsg-2.dsc 3580 SHA512:09d067d3a6060bffc5484417e2329f0534344c7f0b839195dfd126abcf8c2e626cca5d88ba941ae20c2e0ca81bfd8b99ff19b3d5a8fc7e99a1f465a3b5b3c457
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg.orig.tar.xz' heimdal_7.7.0+dfsg.orig.tar.xz 5945252 SHA512:14141f3fff264c9516f736bcc51c998df69cfaa7108d2387921299efd7e82d79b918dee4029905dc221c204d3340ffc17da9472baf80029372d7c13de328ec0a
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.debian.tar.xz' heimdal_7.7.0+dfsg-2.debian.tar.xz 128660 SHA512:a5435ead813f75b0bc7b071dbf4030378f0a8217acd2837d94d0527c0dc456509cd0eef945f7a5c397f7bd2b893400f9813837c404b5b7b0b84fc7540fe40e3e
```

### `dpkg` source package: `hostname=3.23`

Binary Packages:

- `hostname=3.23`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.dsc' hostname_3.23.dsc 1402 SHA512:d520afa2db493464f3b63edc680307f6734c7cf1ec516a42f8de60c3d2d99e3a2e3c18ee5c190cd36f4c3271584b24fe8a4cc7a610b8feaa31c02315f3da512d
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.tar.gz' hostname_3.23.tar.gz 13672 SHA512:aff70bc381ea58944e01f0cabfc674a273b18b0935a87737e16964c08c24382177cc3495368f88a877e293b7fbda76684979cc227eca93e4b033b9c3a975af01
```

### `dpkg` source package: `init-system-helpers=1.60`

Binary Packages:

- `init-system-helpers=1.60`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.60
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.60.dsc' init-system-helpers_1.60.dsc 1902 SHA512:e262b8777e157be7abc9cf95daef12f1f2176e14516630cfd5443528c360082e308a0b002ec67dded0071ea8182b29f65134d20c18f2c97c9c2f274c3f2c5cf6
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.60.tar.xz' init-system-helpers_1.60.tar.xz 40584 SHA512:3739613fa8afa1fa6032f47f8cec67c526171987a7d1eae31d479db9cc1e49ae3cd397a858130c17680d62becb9c6499bd1da1268e9ed25b044337ab69f0dd88
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

### `dpkg` source package: `krb5=1.18.3-5`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.18.3-5`
- `libk5crypto3:amd64=1.18.3-5`
- `libkrb5-3:amd64=1.18.3-5`
- `libkrb5support0:amd64=1.18.3-5`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.18.3-5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3-5.dsc' krb5_1.18.3-5.dsc 3177 SHA512:50c69087c3bc8e8d767412e792844c76214107134095d74b2cf5db421940377ce524dd6bdffa52d99ba01ad6a4612874fba4726c4078ac8533457e15efd8fc39
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz' krb5_1.18.3.orig.tar.gz 8715312 SHA512:cf0bf6cf8f622fa085954e6da998d952cf64dc7ccc319972ed81ea0542089cabf2d0e8243df84da01ad6f40584768ca2f02d108630c6741fa7b3d7d98c887c01
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3.orig.tar.gz.asc' krb5_1.18.3.orig.tar.gz.asc 833 SHA512:7c5a83e13d00910d895d545ed63310ebec48c90c29846dd54e48048f710360e8306778729b636baa091a4e9048998ff6d4dfe37f88dd6292540d55678c961a30
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.18.3-5.debian.tar.xz' krb5_1.18.3-5.debian.tar.xz 103684 SHA512:377f89bb89afb980e480e42563e41e78c195e7f468fa2fdd19ba5951e58091b6e7afae3e3aaf56bcf5cbbcd023db8d874df10264f7d41613bbc8f34e0eef7d3c
```

### `dpkg` source package: `libassuan=2.5.4-1ubuntu1`

Binary Packages:

- `libassuan0:amd64=2.5.4-1ubuntu1`

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
$ apt-get source -qq --print-uris libassuan=2.5.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.4-1ubuntu1.dsc' libassuan_2.5.4-1ubuntu1.dsc 2757 SHA512:97aaa39e12d4eb54762bfa3521780cb9b18037ba86162e353793125c5fbca6677773f10ee61e294e86d423ba8818c5aa2f03e41c8f2c78a655d674e4c2cc6f10
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.4.orig.tar.bz2' libassuan_2.5.4.orig.tar.bz2 574039 SHA512:764993d5311c24f0c0f970016e903e1a16783a2050c42072dbc1bc4f350f119e53b0be17ed6df25a0086bc9f8c25ee4f3134330577968480997263f95e05594f
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.4.orig.tar.bz2.asc' libassuan_2.5.4.orig.tar.bz2.asc 228 SHA512:e97f873670ad52439355dbc0184c74a8341299000ad7170767c06da0b222c9ef47cd645b1ac48747a2a98e1ab3e4c64964bc3aa960423e9d269154d5926b4262
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.4-1ubuntu1.debian.tar.xz' libassuan_2.5.4-1ubuntu1.debian.tar.xz 14380 SHA512:5015863b2b5754471f9ca31388457d4e2138498f30b89fe7feeaa9a7afa0b799dd14eb578a7833131bf40d30e35b6cab75f7835d7cc70c33a1056b6e7307c339
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

### `dpkg` source package: `libedit=3.1-20191231-2`

Binary Packages:

- `libedit2:amd64=3.1-20191231-2`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-2.dsc' libedit_3.1-20191231-2.dsc 2208 SHA512:213ea6f60df04e9a383d808f23dc805d119f583143deab5b80d07c06622d747f83913500ebbbaa21c6587a602adfef073cf95a918c2fff64cfc11a596e3c1653
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA512:1df2eced98e8db1bb0af940678c154d87e3b11dd21e65a903682367f5feace5112f9a543b8e0cb04bbfeaaf73729f808db2d9c302637fc063e81c0a37777ac2c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-2.debian.tar.xz' libedit_3.1-20191231-2.debian.tar.xz 14576 SHA512:f692bc1540d04468bc26da89844ede38f2323984a94d8c894c222f69663ab04c07241c9e9d0d9bd1a93d0a52bceaeeb7ec11525adf76d945266a1e7adcd89fb2
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

### `dpkg` source package: `libffi=3.4~20200819gead65ca871-0ubuntu5`

Binary Packages:

- `libffi8ubuntu1:amd64=3.4~20200819gead65ca871-0ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libffi8ubuntu1/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4~20200819gead65ca871-0ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu5.dsc' libffi_3.4~20200819gead65ca871-0ubuntu5.dsc 2220 SHA512:b1e16e20dfbaa91706a3b24356456bc8d9e5c862796b56f66f5395e0b4056307eccb01fbeabec5a1d5e89ae948b332d91282c38e504ce18981e1334be2fadc09
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871.orig.tar.gz' libffi_3.4~20200819gead65ca871.orig.tar.gz 527371 SHA512:c349b1630db80c042f3c11efe58d4eb849e87f2cca0cc1748c99d32cc34ce4c1262825dc070c8a84263e0adcd8a7af3bd33c705ba28b6cc16974552b12bf0c65
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu5.debian.tar.xz' libffi_3.4~20200819gead65ca871-0ubuntu5.debian.tar.xz 7980 SHA512:cf453efd9b01dd63f237c023530597188471423e266fcf7716ece957abdfd11ed9244c5913db78965f5bca1e63c51eafcbd3299195058bee0214fb7d210faf74
```

### `dpkg` source package: `libfido2=1.6.0-2`

Binary Packages:

- `libfido2-1:amd64=1.6.0-2`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.6.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0-2.dsc' libfido2_1.6.0-2.dsc 2565 SHA512:37bb1caa75b306ae625779cb39315b75b3aed32d131103b78706188a7c062762ad9bec7dc1ddcf510e463900f4311165e5b50a284cdf6bb51d1a9d1bac1d2f4a
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz' libfido2_1.6.0.orig.tar.gz 413904 SHA512:c473732a2f7ef54156097d315e44457d89056446ab3112a7c7a6fd99d5c2c8ae0ca2451ff9cd45be6c32de1ab335d6dfdb2b0c56b40cae9eb41391d18d83be4a
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0.orig.tar.gz.asc' libfido2_1.6.0.orig.tar.gz.asc 488 SHA512:ea6b2191bbbce3b1e905a6835cc05f38571f65d3590984e1591a1b630bafa29c646a4c813cc5761cf3013b41da1246a70037eaa7aeefe3daf7740a468cc99d4f
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.6.0-2.debian.tar.xz' libfido2_1.6.0-2.debian.tar.xz 72700 SHA512:c890d377b53a2ef686d40aa07af0e2ead25ad217dd5692bbcf29f246b6672eb4aed53afc6bbbdf1b3a4c0e2ad6f778a7bdb43ff72eb708c7c404feedf2ff0e54
```

### `dpkg` source package: `libgcrypt20=1.8.7-5ubuntu1`

Binary Packages:

- `libgcrypt20:amd64=1.8.7-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.7-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-5ubuntu1.dsc' libgcrypt20_1.8.7-5ubuntu1.dsc 2562 SHA512:fc4161f417f974a3a88b3f9f3b1ea0095550a08af0b4d809426d97cd9057c20d06380b7f60edab0ed20438ea318b26f6a2a6fed97c666fb968781afd4d2388aa
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2' libgcrypt20_1.8.7.orig.tar.bz2 2985660 SHA512:6309d17624d8029848990d225d5924886c951cef691266c8e010fbbb7f678972cee70cbb91d370ad0bcdc8c8761402a090c2c853c9427ec79293624a59da5060
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7.orig.tar.bz2.asc' libgcrypt20_1.8.7.orig.tar.bz2.asc 228 SHA512:4ba6875dfddbc9bece0c4d25d1c3b0e6183045288ca876b84c24d487ee72f751ecda6eaec71e70ba00fd2434c77127283af1a957ac9e6f40352ef67add672c72
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.7-5ubuntu1.debian.tar.xz' libgcrypt20_1.8.7-5ubuntu1.debian.tar.xz 39848 SHA512:35ec4913d4988d9897da3ac3d45a727836ad90a5bf4d742925f46086d576faab410573371a11f496801e78c537c302111d89c86f8d022d4462b0d0741f86298a
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

### `dpkg` source package: `libnsl=1.3.0-2`

Binary Packages:

- `libnsl2:amd64=1.3.0-2`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2.dsc' libnsl_1.3.0-2.dsc 1955 SHA512:cc9705030314323a099c712f7a3cbc014841ddf109f151025d36d5074303f863a2fee36911afc8e828aa6af5fbbe6e194fa65e89715328d734cd69d68bdedb40
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA512:a5a6c3ccb2d1e724c8c1f65e55dcd09383eb1ae019c55f4c09441eadf23ffbc2196cfad259805b0ac40ddf3a10af0da453e4d739d67d46829c64d0995dab4e55
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-2.debian.tar.xz' libnsl_1.3.0-2.debian.tar.xz 4692 SHA512:d25562e49ae091a6e0102710f73b6d73ed21ed519bf75f66582c8d2e39148d6dd394cbe040303dcbe5cec53bde56c70eca7e9a2b4be7a6c1bffcd5b48e2e11ea
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

### `dpkg` source package: `libselinux=3.1-3build1`

Binary Packages:

- `libselinux1:amd64=3.1-3build1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.1-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-3build1.dsc' libselinux_3.1-3build1.dsc 2670 SHA512:b320f55bab2f4e0b52e7c411631c32afd291923f61f49fd54fbf2b937be54c98660d41d50a3061b416598b2ab775f6ffcca0e9f4cd57786b8875799fe25013ce
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1.orig.tar.gz' libselinux_3.1.orig.tar.gz 204703 SHA512:57730cddd2d4751556d9e1f207c0f85119c81848f0620c16239e997150989e3f9a586a8c23861fd51ed89f7e084ad441190a58a288258a49a95f7beef7dbbb13
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-3build1.debian.tar.xz' libselinux_3.1-3build1.debian.tar.xz 24252 SHA512:8a2499e99bd257882928aabd6c72df5efdb984bb54f2446c7f791beb9bfcf8150aeaf3415d864ad4ccd53892f6f48306784780e4b6d169fca2814ed30765bba3
```

### `dpkg` source package: `libsemanage=3.1-1ubuntu1`

Binary Packages:

- `libsemanage-common=3.1-1ubuntu1`
- `libsemanage1:amd64=3.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1ubuntu1.dsc' libsemanage_3.1-1ubuntu1.dsc 2713 SHA512:a8cfc21d226499eebe9af1f23257c19410f3a3b18fef2984519fea9173132d6e6bd64910fa314c9e24fa3bffc5509a948b3d47501e1922e7fde3d64b0e8a0cb7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1.orig.tar.gz' libsemanage_3.1.orig.tar.gz 179601 SHA512:8609ca7d13b5c603677740f2b14558fea3922624af182d20d618237ba11fcf2559fab82fc68d1efa6ff118f064d426f005138521652c761de92cd66150102197
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1ubuntu1.debian.tar.xz' libsemanage_3.1-1ubuntu1.debian.tar.xz 17816 SHA512:241f3b835d6daa840abb2209aa7feb596df69f8b31b2f9e82d1ac2bed9277390def85d2c254ce37a35a6bd9b5a783ddf45e7de6761bb9d760e00576373dd5c8b
```

### `dpkg` source package: `libsepol=3.1-1ubuntu1`

Binary Packages:

- `libsepol1:amd64=3.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1ubuntu1.dsc' libsepol_3.1-1ubuntu1.dsc 2150 SHA512:28e91fdce97c8aa37730bafd2188a8795c985b7c3a04d75e218b3082f9ae4b4ebc23d39d98a422f3dabcc0ea79b5f4a847d12ae5e15a178400d21266c4bf8d30
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA512:4b5f4e82853ff3e9b4fac2dbdea5c2fc3bb7b508af912217ac4b75da6540fbcd77aa314ab95cd9dfa94fbc4a885000656a663c1a152f65b4cf6970ea0b6034ab
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1ubuntu1.debian.tar.xz' libsepol_3.1-1ubuntu1.debian.tar.xz 14760 SHA512:4120fa3c54a6b991d1b34d6f79dd8a97febb8467f8864f563b3e44e9a5813f9cf7fe249b5ee04f082cd3746ff422a6c673e20f2a26c3e890b06f0f63ecb434a5
```

### `dpkg` source package: `libssh=0.9.5-1`

Binary Packages:

- `libssh-4:amd64=0.9.5-1`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5-1.dsc' libssh_0.9.5-1.dsc 2364 SHA512:8b0f2c4fa628db7866ff4b433a94e7ec6c3e03cb961a4d3b7b3d4fadb9c84a9459c2c7fce2b37878b47fbcfb1e3f303589963f324fb8a56cb32a8c0ebe8a35d6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5.orig.tar.xz' libssh_0.9.5.orig.tar.xz 502876 SHA512:64e692a0bfa7f73585ea7b7b8b1d4c9a7f9be59565bfd4de32ca8cd9db121f87e7ad51f5c80269fbd99545af34dcf1894374ed8a6d6c1ac5f8601c026572ac18
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5.orig.tar.xz.asc' libssh_0.9.5.orig.tar.xz.asc 833 SHA512:f0b76cdccf26144b9cc9ad3f7e1605b50473fc5c686d0d9a2419b13382440776c09428d717253a918f7347b90e4a562fd88d8ea85a6e54f06b149826295b4f8e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.5-1.debian.tar.xz' libssh_0.9.5-1.debian.tar.xz 27056 SHA512:3c77003311004858f9972ec7ec5c7b4aa379c174083fc946c2671868b480bb8cc87e9bebde50a02165f78dca5e3f283fc93874ae523c42b0e15ad166e9ca4b05
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

### `dpkg` source package: `libtirpc=1.3.1-1build1`

Binary Packages:

- `libtirpc-common=1.3.1-1build1`
- `libtirpc3:amd64=1.3.1-1build1`

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
$ apt-get source -qq --print-uris libtirpc=1.3.1-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.1-1build1.dsc' libtirpc_1.3.1-1build1.dsc 2135 SHA512:9cc8da4769d548e7008d60a0fd79bb5793522d7dd22bd2a547c0f8187ab128fc62dab88e53738f7a1db376ab4487073fed73c506bea9bf31df17499d29462181
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.1.orig.tar.bz2' libtirpc_1.3.1.orig.tar.bz2 513399 SHA512:131f746800ac7280cc3900597018fc8dbc8da50c14e29dbaccf36a6d110eded117351108c6b069eaac90d77cfec17014b08e9afddcf153fda2d780ba64260cbc
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.3.1-1build1.debian.tar.xz' libtirpc_1.3.1-1build1.debian.tar.xz 10848 SHA512:e4e346b9df6d75f2ef8c7d40c82e54ee151b96d4fa5af40d7fd59ff05523c8981311b56c2ef963f4eff5eba89724fe712da1313042bbc2eabc7ac51e9bb26fcc
```

### `dpkg` source package: `libunistring=0.9.10-4`

Binary Packages:

- `libunistring2:amd64=0.9.10-4`

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
$ apt-get source -qq --print-uris libunistring=0.9.10-4
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.dsc' libunistring_0.9.10-4.dsc 2212 SHA512:498003f18665d5b50c34a5bcaa6d13dae65673d99671e5256e3500aeeae35710dad7e08c1f3ab20adb37ba10ca9b36a6916068cc3425261e734b5ecc25e78bf8
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA512:01dcab6e05ea4c33572bf96cc0558bcffbfc0e62fc86410cef06c1597a0073d5750525fe2dee4fdb39c9bd704557fcbab864f9645958108a2e07950bc539fe54
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA512:94d4316df1407850f34e84064275ae512d1ee1cd519420e2342a3f36c17d1ff7fa4019fea64507a04034ffc356c0c9add94a5abf756dd5995913583f68cfe0bd
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.debian.tar.xz' libunistring_0.9.10-4.debian.tar.xz 40936 SHA512:b687df5ffae03ad5de8c2ee42b566946c2164574a78801a55ca1a4ee61d602007de002f5c996b7b408bf8793706061b6339657b50db305811e543e24de87516e
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
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-2.1.dsc' libzstd_1.4.8+dfsg-2.1.dsc 2274 SHA512:80d08192a1cfbd07b93072a99f898111ae7009105e4e378b1ed7aa722df3123753729b545cd7b3608d17be17a4be1d1231658222531c9f31db6210892644a3a6
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA512:07fabe431367eea4badae7b1e46ac73e0b33aad5b67361bc7b67d5f9aef249c51db5b560f1cf59233255cc49db341a8d8440fed87745026fca7a7c5c14448cd8
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-2.1.debian.tar.xz' libzstd_1.4.8+dfsg-2.1.debian.tar.xz 12224 SHA512:c43ebcd786bf0bf011ba37136ff03f6996b1569508a98aea55c004e48466080f0b799fba71469391898d55253a435c80b1a0a75c7f5229980dc973cf09f98814
```

### `dpkg` source package: `lsb=11.1.0ubuntu2`

Binary Packages:

- `lsb-base=11.1.0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.dsc' lsb_11.1.0ubuntu2.dsc 2230 SHA512:d4545cee6b6ee4b54cd13ed7f8ab874a44579ce0783bb813a9dc48f0ca132b2bf11aba2fd179ff7d82ad867f663e1521b224da0de5fb3f66b634542d56addc55
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.tar.xz' lsb_11.1.0ubuntu2.tar.xz 46024 SHA512:b4a2c35ef8a21e3e6e1978687f54f485f0a3c8ee09082f8ae0d7a3dc0f65381062e1df962190164c3539f3f86c073961eb9f3c37b2aa4d3d8d6907a99ce04161
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

### `dpkg` source package: `mpdecimal=2.5.1-2`

Binary Packages:

- `libmpdec3:amd64=2.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libmpdec3/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.5.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1-2.dsc' mpdecimal_2.5.1-2.dsc 1919 SHA512:5bb42ab4c1f4279b5dd01b88960460839d19c544d86e8ac77db6209f0d2902035f4cc5392c3c88d2fbb3cdb867f70a30151c8a8f1ca34af83f22743f9c652b86
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1.orig.tar.gz' mpdecimal_2.5.1.orig.tar.gz 2584021 SHA512:710cb5cb71dbcf3e170ca15869c148df0547b848400c6b6dd70c67d9961dbe1190af8fb4d1623bfb0ca2afe44f369a42e311ab5225ed89d4031cb49a3bd70f30
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.5.1-2.debian.tar.xz' mpdecimal_2.5.1-2.debian.tar.xz 6696 SHA512:15a1a5ea119353aefbf2e3d250f678c1af2e97b0f3542997e0a71149aa546dfc8512d45ac349e9b89ddcf161a99ff8b1e0bb7180e2bc2da07d08b9a335c54787
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
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114-2build1.dsc' ncurses_6.2+20201114-2build1.dsc 4155 SHA512:329c5e300e7c17925750a0bc7ece0582ec23cf8323ed74134e1cb7b235deb596b7f8cb8b01a80b21bb32e6d11aeb6e00e2fb9ffbe9ea0186b1139a417ce452fa
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114.orig.tar.gz' ncurses_6.2+20201114.orig.tar.gz 3539796 SHA512:d163bc8f08f6b2406f8f562fecd9035e0e6f2db8b539cbcaeb4a80b15027b518026526eac1b2681da82b8d03dd1c924a85de1294e6ace2a5dbc03126512a3e2c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114.orig.tar.gz.asc' ncurses_6.2+20201114.orig.tar.gz.asc 265 SHA512:210035a4ec94cdb650ac4cf7990791dc482ea941b410dcf635525fa3282df28464a1b8c0e5a4721868ccbe2609bae2db3632ecd166d239ef84471c536ce81f9c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2+20201114-2build1.debian.tar.xz' ncurses_6.2+20201114-2build1.debian.tar.xz 51936 SHA512:ba116c897b83cc0acfdc9ef0065067363d862a67e77d8f26533859ec8bd20c5d5b3ae76b573a52456dc084f206b58033f0dfc8484c3bd14da49d9c38112ab1f1
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

### `dpkg` source package: `nettle=3.7.2-3`

Binary Packages:

- `libhogweed6:amd64=3.7.2-3`
- `libnettle8:amd64=3.7.2-3`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/nettle/3.7.2-3/


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

### `dpkg` source package: `openldap=2.4.57+dfsg-2ubuntu1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.57+dfsg-2ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.57+dfsg-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.57+dfsg-2ubuntu1.dsc' openldap_2.4.57+dfsg-2ubuntu1.dsc 3155 SHA512:358417cc1cf0184b9274da2b5a98265bd2b5f251ab18b70b0187de9617fd627133ea709521d7606331845532b3ad35f53c8264693b47da2706b614fa7a2b75e1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.57+dfsg.orig.tar.gz' openldap_2.4.57+dfsg.orig.tar.gz 5054318 SHA512:8d26e217a1847c362418900a79e63cbdb408b6709d22945d79655bf1828dbe1ccaafcf5b7629f5ff50e3b5f246277b35df2f979dd53b1922fe00bb60deb9d9d1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.57+dfsg-2ubuntu1.debian.tar.xz' openldap_2.4.57+dfsg-2ubuntu1.debian.tar.xz 182804 SHA512:c91c2961f5bf88b94a49803adca066d3b3f3b600c737f462dfdbc691260953508c6869f52feb6cf95a9d094283f5e03b9cb50adea321ad5a9c0bc2ca836a883d
```

### `dpkg` source package: `openssh=1:8.4p1-5ubuntu1`

Binary Packages:

- `openssh-client=1:8.4p1-5ubuntu1`

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
$ apt-get source -qq --print-uris openssh=1:8.4p1-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1-5ubuntu1.dsc' openssh_8.4p1-5ubuntu1.dsc 3370 SHA512:849944bbbbb5d11a7893468bfcdd54ea201f8b759afba8a2dbdd5999e2d1668b6f3c79b620b5bfdcd493fb7d742bd909d1bc8613317e6504550b7a294c3cecdf
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1.orig.tar.gz' openssh_8.4p1.orig.tar.gz 1742201 SHA512:d65275b082c46c5efe7cf3264fa6794d6e99a36d4a54b50554fc56979d6c0837381587fd5399195e1db680d2a5ad1ef0b99a180eac2b4de5637906cb7a89e9ce
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1.orig.tar.gz.asc' openssh_8.4p1.orig.tar.gz.asc 683 SHA512:3d9a026db27729a5a56785db3824230ccf2a3beca4bb48ef465e44d869b944dbc5d443152a1b1be21bc9c213c465d3d7ca1f876a387d0a6b9682a0cfec3e6e32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.4p1-5ubuntu1.debian.tar.xz' openssh_8.4p1-5ubuntu1.debian.tar.xz 180032 SHA512:faec209ecd6598baa573b27bb5b5096fb82e748541033c0afc6bd47efe58887c0a54afa83e9cec0f6f89d825963e796b447a48744389194b569c92e5e7113015
```

### `dpkg` source package: `openssl=1.1.1j-1ubuntu4`

Binary Packages:

- `libssl1.1:amd64=1.1.1j-1ubuntu4`
- `openssl=1.1.1j-1ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1j-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1j-1ubuntu4.dsc' openssl_1.1.1j-1ubuntu4.dsc 2737 SHA512:f641ee7d7e53808b59f0271bf3f6ad4d8c34c9ae675c173d94b9941f4756593f52b0f7d3cd4aa2500651c975aecd305a840739b208931615b35bfd9ac5533516
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1j.orig.tar.gz' openssl_1.1.1j.orig.tar.gz 9823161 SHA512:51e44995663b5258b0018bdc1e2b0e7e8e0cce111138ca1f80514456af920fce4e409a411ce117c0f3eb9190ac3e47c53a43f39b06acd35b7494e2bec4a607d5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1j.orig.tar.gz.asc' openssl_1.1.1j.orig.tar.gz.asc 488 SHA512:0a387ddd5dea88e5d62b4bd05320993ed6750c0d88d6712dd97c76c9f2bd3d9235a2b8e90a36bfc0834101d3e49e79523b3eb4ed9913bddc6e470de242bfffee
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1j-1ubuntu4.debian.tar.xz' openssl_1.1.1j-1ubuntu4.debian.tar.xz 149188 SHA512:7ac27bcfb676da35c10c489f83f8e932a9070cde5f3c3824eb962dfabd676e5ddeb18f1670c5b8b973f831758f188a8bd65ab17c32f85232945c3654e808f8ca
```

### `dpkg` source package: `p11-kit=0.23.22-1`

Binary Packages:

- `libp11-kit0:amd64=0.23.22-1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.22-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22-1.dsc' p11-kit_0.23.22-1.dsc 2417 SHA512:09d764f710260a71041b5714397af68b0aaf20bd419b9aac7997709d80ac3bddf4fe2c132ca9510bb662986b4e3576627628237cd9c95ed7d1ff1ffcca04cee7
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz' p11-kit_0.23.22.orig.tar.xz 830016 SHA512:098819e6ca4ad9cc2a0bc2e478aea67354d051a4f03e6c7d75d13d2469b6dc7654f26b15530052f6ed51acb35531c2539e0f971b31e29e6673e857c903afb080
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22.orig.tar.xz.asc' p11-kit_0.23.22.orig.tar.xz.asc 854 SHA512:1ebb730b9c29908773de12aca89df2434576b8d9ec5da6d33db772b1e1aa4b0e8aa86ddc3e0de1abcd98a7012b5a25e3097e3a2dda2401cc37f79fd76b4f9467
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.22-1.debian.tar.xz' p11-kit_0.23.22-1.debian.tar.xz 22256 SHA512:5d10918372cf7b6ae5ee6aa03e653b2ba55e61a691c9e9e7d8673a2e4a632941ccda38e213691ca5b05ce422d1af71ced902cf9c7b8d3be7e45662e96e6dce69
```

### `dpkg` source package: `pam=1.3.1-5ubuntu7`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu7`
- `libpam-modules-bin=1.3.1-5ubuntu7`
- `libpam-runtime=1.3.1-5ubuntu7`
- `libpam0g:amd64=1.3.1-5ubuntu7`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu7.dsc' pam_1.3.1-5ubuntu7.dsc 2699 SHA512:e43aba98b79337d266668ba6d3da81a0352abf9716d7f35b8cd8e0f291f8ac5d6759d9c2c7d497671160502c4d2ff686c52ae9425f9f981d3710e9d05fb81267
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA512:6bc8e2a5b64686f0a23846221c5228c88418ba485b17c53b3a12f91262b5bb73566d6b6a5daa1f63bbae54310aee918b987e44a72ce809b4e7c668f0fadfe08e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu7.debian.tar.xz' pam_1.3.1-5ubuntu7.debian.tar.xz 172872 SHA512:3037c8862d5f47cc815c5afdc2da729f815522f5966321a50cd2ab50c6974f071a30f1680209a9c7447edd40d8047a90c1919b90ebfc77b9444fc521982431d9
```

### `dpkg` source package: `pcre2=10.36-2ubuntu5`

Binary Packages:

- `libpcre2-8-0:amd64=10.36-2ubuntu5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.36-2ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.36-2ubuntu5.dsc' pcre2_10.36-2ubuntu5.dsc 2278 SHA512:3c8e8b4c2eff8dc95f33b2566e293cd2ae12d2b80383691dbb8642d854d8f462f29ecfa8eed2877a2ed3df3c61c9080bb0c1c7e206ee285aacb1a995f772290d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.36.orig.tar.gz' pcre2_10.36.orig.tar.gz 2290719 SHA512:a776cda406aea4a30f5072b24fc41bafd580d92e6d7c782b3c5468570f58fb085184ff707d90d8e83662f578c4327178f5ff4236222d0b3ca07244ef70528aa8
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.36-2ubuntu5.diff.gz' pcre2_10.36-2ubuntu5.diff.gz 7183 SHA512:ae6dfd6ed5ef3ad7f16c8f782fe7cc1f0f12a989eb273b600d73c6bec908b9b2949ad68a3324a2a9ee1c35f5a1f2ac26812eb57f1cb383f72ceabdfb3a64055a
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

### `dpkg` source package: `perl=5.32.1-3ubuntu2`

Binary Packages:

- `libperl5.32:amd64=5.32.1-3ubuntu2`
- `perl=5.32.1-3ubuntu2`
- `perl-base=5.32.1-3ubuntu2`
- `perl-modules-5.32=5.32.1-3ubuntu2`

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
$ apt-get source -qq --print-uris perl=5.32.1-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1-3ubuntu2.dsc' perl_5.32.1-3ubuntu2.dsc 2914 SHA512:d5b80321782e6f10a70f3a8b2a0b2c7cf54e29d13e29073cc3ced076edeca8052ea5ec28e04ede6b5df80da81b514da861e1d7abd987bf931906d344ac105203
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1.orig-regen-configure.tar.gz' perl_5.32.1.orig-regen-configure.tar.gz 871331 SHA512:c80782d17ea13cbe5592166cd8d1fcc80229eb2df39f89415ae9bf0dd2f9d3f05d554b0089fdd4d968a4ae53037cad18097289ee7ff19020eddd94db1de00fbb
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1.orig.tar.xz' perl_5.32.1.orig.tar.xz 12610988 SHA512:3443c75aea91f0fe3712fee576239f1946d2301b8f7390b690e2f5d070fe71af8f9fa7769e42086c2d33d5f84370f80368fa9350b4f10cc0ac3e6c1f6209d8f9
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.32.1-3ubuntu2.debian.tar.xz' perl_5.32.1-3ubuntu2.debian.tar.xz 165164 SHA512:d6dd1dff0bb68638ba6cdbbfd6f396b985d5ccf2b63ac0d343632874bae86742f27c5c1822e39559d0ec62dc5cd5dc40ae7849b17b92abd9888a1b5bcc182842
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

### `dpkg` source package: `procps=2:3.3.17-5ubuntu2`

Binary Packages:

- `libprocps8:amd64=2:3.3.17-5ubuntu2`
- `procps=2:3.3.17-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.17-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-5ubuntu2.dsc' procps_3.3.17-5ubuntu2.dsc 2237 SHA512:a55f7783a4f8ef668b3aae12908cce276f36101d3aab72f6e887441b31797adcca1fcae2340a32e105a98af184e4298acd8303ffc738895870866cccc9c7e40f
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17.orig.tar.xz' procps_3.3.17.orig.tar.xz 1008428 SHA512:59e9a5013430fd9da508c4655d58375dc32e025bb502bb28fb9a92a48e4f2838b3355e92b4648f7384b2050064d17079bf4595d889822ebb5030006bc154a1a7
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.17-5ubuntu2.debian.tar.xz' procps_3.3.17-5ubuntu2.debian.tar.xz 33552 SHA512:3941ac7bb94ad5676ec81271b1f3407d8d1671fc32687be3cb135413f4475427cdb979f14f5de7d00740a62bdd79b030418e0cb31152416b1729a7bb84e32425
```

### `dpkg` source package: `python3-defaults=3.9.4-1`

Binary Packages:

- `libpython3-stdlib:amd64=3.9.4-1`
- `python3=3.9.4-1`
- `python3-minimal=3.9.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.9.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.4-1.dsc' python3-defaults_3.9.4-1.dsc 2879 SHA512:ba4961aeb3c481ad29771d0a6a37c984a41fac691daa62e52e0331e593b277816e3d560f5075beb6bd61f3608a3544573f816f1a8fdf0501d0d0e58b4eeeece0
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.4-1.tar.gz' python3-defaults_3.9.4-1.tar.gz 140963 SHA512:7a0357ce46a2e0f96d8545f457a69dd10dccb80dd7c569dd4074a3a2a834d1ddf7a0ce21f91d9dc55a942affcb40283ce96cdec80c1be12e669a270f559b52ca
```

### `dpkg` source package: `python3.9=3.9.5-3`

Binary Packages:

- `libpython3.9-minimal:amd64=3.9.5-3`
- `libpython3.9-stdlib:amd64=3.9.5-3`
- `python3.9=3.9.5-3`
- `python3.9-minimal=3.9.5-3`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3.9/3.9.5-3/


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

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2build2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2build2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build2.dsc 2402 SHA512:bd16f8a7269549b4f15e46017012a2d99ed22378dcca6b9b664ff137d18c946b3f0b03f8a961c928196ddc473f1012a968bd91c3d4df6837da97fa0634f85c12
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA512:bdfcbab73179d614a295a7b136ea4c9d0ce4620883b493f298362784d245608cd6ad4b0ad30f94ed73a086b4555399521ae9e95b6375fce75e455ae68c055e7b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build2.debian.tar.xz 8276 SHA512:9fb15d0d48319162214f9e417a183559f9b09c22ea89546c81ae2add40c802bb48ff54ea32162b209c99bf8dae939f4eb7af9498aff831f697f5f095160b95ba
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


### `dpkg` source package: `shadow=1:4.8.1-1ubuntu8`

Binary Packages:

- `login=1:4.8.1-1ubuntu8`
- `passwd=1:4.8.1-1ubuntu8`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu8.dsc' shadow_4.8.1-1ubuntu8.dsc 2345 SHA512:ba6658eab0eae7ed21ffd04f0e63f761ab45a682b18992cd83776dac5dc617f6d301a3829fdc5726d7b815883a8f8a455a8a2820f984f7aea3c2201573e9f2cb
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA512:780a983483d847ed3c91c82064a0fa902b6f4185225978241bc3bc03fcc3aa143975b46aee43151c6ba43efcfdb1819516b76ba7ad3d1d3c34fcc38ea42e917b
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu8.debian.tar.xz' shadow_4.8.1-1ubuntu8.debian.tar.xz 86200 SHA512:01824fe4238614df35b199e1b3f3851719a71f2c76a77cc90883a3cca0b56082309e2aee8825603d01651d06442a4ef30de83139629cef585285b59182eaa97a
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

### `dpkg` source package: `systemd=248.3-1ubuntu1`

Binary Packages:

- `libsystemd0:amd64=248.3-1ubuntu1`
- `libudev1:amd64=248.3-1ubuntu1`

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
$ apt-get source -qq --print-uris systemd=248.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_248.3-1ubuntu1.dsc' systemd_248.3-1ubuntu1.dsc 5366 SHA512:7c1a30831ee3023a13303af5be2e1c91ec8be696fb57baf9c541129de80b09a3c0cc25191c528ad43933a7eee0c61725c2cb99ddcd2a43da7573b7467530a446
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_248.3.orig.tar.gz' systemd_248.3.orig.tar.gz 10320940 SHA512:8e7ff0d5e63cc933e4dc23f7e0bef9707fde90396605eb8822d34de90d7abe8fd37e5739e33b657868218aa7281147cc944c096c007324c3e6fb54d833a83485
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_248.3-1ubuntu1.debian.tar.xz' systemd_248.3-1ubuntu1.debian.tar.xz 198572 SHA512:9404ea5a700630d4da370c1c4c29201f64d7cf0516691777afd14908db86ba2f300fdf5074af17bcb106f06ffc38045802c09cfafcd764b0f5e77e4bf9540a01
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
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34+dfsg-1build1.dsc' tar_1.34+dfsg-1build1.dsc 2093 SHA512:3251c52ed6f0e3dc2b89f61a6f0dbf28c04170c5c18ebee5a2b035e02ba876b89bf45d60c6eda6f26f86211465e9aafc6b715592077d6f9120ed8cbcafd70cbb
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34+dfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA512:ec5553c53c4a5f523f872a8095f699c17bf41400fbe2f0f8b45291ccbaf9ac51dea8445c81bd95697f8853c95dcad3250071d23dbbcab857a428ee92e647bde9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34+dfsg-1build1.debian.tar.xz' tar_1.34+dfsg-1build1.debian.tar.xz 19296 SHA512:50378351a260ca81aa2e68994bd37fbfbd35e3b8c9d8c07cfe2b8424edb0da64c40283cca625af95a8a4abe4483bf5c205727fc35dda13773d2ddaead4f9fb24
```

### `dpkg` source package: `tzdata=2021a-1ubuntu1`

Binary Packages:

- `tzdata=2021a-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2021a-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021a-1ubuntu1.dsc' tzdata_2021a-1ubuntu1.dsc 2358 SHA512:d0de8ec0c949a976b6d657f1e2e4045296737b28a1e49de0bad6acd0af4027c7e10676b968ffc3d6ef0c8b62e2a5a6676cd95cbdcbfca2730ecac30e0837bfe4
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021a.orig.tar.gz' tzdata_2021a.orig.tar.gz 411892 SHA512:7cdd762ec90ce12a30fa36b1d66d1ea82d9fa21e514e2b9c7fcbe2541514ee0fadf30843ff352c65512fb270857b51d1517b45e1232b89c6f954ba9ff1833bb3
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021a.orig.tar.gz.asc' tzdata_2021a.orig.tar.gz.asc 833 SHA512:41532174622222fc5e8d733c4af2decfcd0ab3f56db946763d1731ae96873e31abcb31f9a7a442428c78ea21612318b05c99bcf4b9bf37d59f11d1dc914814e6
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021a-1ubuntu1.debian.tar.xz' tzdata_2021a-1ubuntu1.debian.tar.xz 165180 SHA512:1e73ceed23d16f8a54a8ddcc0cb72eb675f585bfb0aecffdf03ae74ee95bff50da28bbcf9cbb40a42072d41937ebfa3b35b4ff4daf689e09ef3eecb55818b924
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

### `dpkg` source package: `usrmerge=25ubuntu1`

Binary Packages:

- `usrmerge=25ubuntu1`

Licenses: (parsed from: `/usr/share/doc/usrmerge/copyright`)

- `GPL v2`
- `GPL-2`
- `later (please see /usr/share/common-licenses/GPL-2)`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=25ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_25ubuntu1.dsc' usrmerge_25ubuntu1.dsc 1614 SHA512:c2d86a38a0876f291c2c7c7fe563c019739032d2303ce6a1b17d2388e7f366168c33b83b0db93e493bd4ad265e941d081f3cb45aa4a1d455ea4a607b9b70d706
'http://archive.ubuntu.com/ubuntu/pool/main/u/usrmerge/usrmerge_25ubuntu1.tar.xz' usrmerge_25ubuntu1.tar.xz 12620 SHA512:7baaf4b45dacf3204186c961216930f49682d1b53246bd99116d4c2efff3c47ff14e21d4d6aa4730aeb1496884427dcfb4ef099d5ab24c03dd94485e754a93e5
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

### `dpkg` source package: `util-linux=2.36.1-7ubuntu2`

Binary Packages:

- `bsdutils=1:2.36.1-7ubuntu2`
- `libblkid1:amd64=2.36.1-7ubuntu2`
- `libmount1:amd64=2.36.1-7ubuntu2`
- `libsmartcols1:amd64=2.36.1-7ubuntu2`
- `libuuid1:amd64=2.36.1-7ubuntu2`
- `mount=2.36.1-7ubuntu2`
- `util-linux=2.36.1-7ubuntu2`

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
$ apt-get source -qq --print-uris util-linux=2.36.1-7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1-7ubuntu2.dsc' util-linux_2.36.1-7ubuntu2.dsc 4496 SHA512:67550fa43b1e87bcfc2d6e840e312259c2e79996bbc533d377338b5491c7517c2c6c8c5ec3ec33bf330f03f213e798df82351977148499132ecddd55b069304b
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1.orig.tar.xz' util-linux_2.36.1.orig.tar.xz 5231880 SHA512:9dfd01ae4c16fa35015dafd222d555988b72e4d1d2fbadd140791b9ef78f84fa8254d4d08dc67cabf41e873338867f19e786b989d708ccfe5161c4f7679bba7a
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.1-7ubuntu2.debian.tar.xz' util-linux_2.36.1-7ubuntu2.debian.tar.xz 102024 SHA512:45378c3291b306980b9715e57826035cebb0637807fe62831a842d063fe8faa9f02ca7a1bbfc36d5981a116a249059eb548dfb424d8cb8027da6fc3d7a574079
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

### `dpkg` source package: `xxhash=0.8.0-2`

Binary Packages:

- `libxxhash0:amd64=0.8.0-2`

Licenses: (parsed from: `/usr/share/doc/libxxhash0/copyright`)

- `BSD-2-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris xxhash=0.8.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0-2.dsc' xxhash_0.8.0-2.dsc 1601 SHA512:8ced1e4a71c06c4de87469316d28d1ea905f52bb3debb4152d2b42f0eda355dbac43576d7d5eb4e31d8e9a032e83ba4b5893db9aed04e5abffe8437e1d2f1b7c
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0.orig.tar.gz' xxhash_0.8.0.orig.tar.gz 145909 SHA512:c3973b3c98bad44e1d8687ab4f9461aecd1c071bb3d320537a4c50fb7301edd13e990bab48cc6e5ca30536a814c8fa8cac24ceb1803a7e8eca30ef73d449373e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xxhash/xxhash_0.8.0-2.debian.tar.xz' xxhash_0.8.0-2.debian.tar.xz 4160 SHA512:7ca8e3e87bb87bd58e03161ecfbe682f3950068bc4aec0a7e300c307b35bdafc6d76a54edf4887a584c426d455d0c557d9d4df98d85c7cdf734d67e5f5aca4f3
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

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu6`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu6`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu6.dsc' zlib_1.2.11.dfsg-2ubuntu6.dsc 2970 SHA512:8c366400152e7c9e508a5f3f9160bb2dcf6666fbc5ea76901875aa3d2a8fafc8f7dbc5c177efb6923ee736ae83094c67754cd4009653ee608e911a53d806c0e6
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu6.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu6.debian.tar.xz 51084 SHA512:6b217f69106cf737db367ac2814549b488d49d0809ed2d886808fd79ae237b74140b9e9ce7f7cb849468394d2dbf67585bd54321e49f444eef735fef782cc6b8
```
