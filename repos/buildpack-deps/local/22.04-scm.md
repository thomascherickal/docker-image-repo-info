# `buildpack-deps:jammy-scm`

## Docker Metadata

- Image ID: `sha256:e1cbe194e1ec811c6a0bf0b692152d53e09dde661d2a239821d3c41062422b1b`
- Created: `2022-02-02T09:28:23.727191452Z`
- Virtual Size: ~ 217.67 Mb  
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

### `dpkg` source package: `apr-util=1.6.1-5ubuntu3`

Binary Packages:

- `libaprutil1:amd64=1.6.1-5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-5ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu3.dsc' apr-util_1.6.1-5ubuntu3.dsc 2611 SHA512:de7f35d8823d5d905225d3939c569eb2da743148f22593665dca3a2d631f8efb959bee2a11ccb0784435b8d1ab51f7afa613348c1f0b30cadcbdcc749b93c0e8
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA512:40eff8a37c0634f7fdddd6ca5e596b38de15fd10767a34c30bbe49c632816e8f3e1e230678034f578dd5816a94f246fb5dfdf48d644829af13bf28de3225205d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-5ubuntu3.debian.tar.xz' apr-util_1.6.1-5ubuntu3.debian.tar.xz 342760 SHA512:dea487dce39c91bb4ab8042ce60926c28c061fd742fcccf49a067542e5da9aa7204b177202f25d1e39dc43718783201a21a9c470a735e2dedd356bff12f867e3
```

### `dpkg` source package: `apr=1.7.0-8`

Binary Packages:

- `libapr1:amd64=1.7.0-8`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.7.0-8
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-8.dsc' apr_1.7.0-8.dsc 2272 SHA512:1fc756a42bde32c1aeb32060ee9290c4c5dc833f289d82bdefdb24c3aa35a7815c1cc00d21a706e53f5b2f1a12466ad209969aca57bc8a6488747720162cf202
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2' apr_1.7.0.orig.tar.bz2 872238 SHA512:3dc42d5caf17aab16f5c154080f020d5aed761e22db4c5f6506917f6bfd2bf8becfb40af919042bd4ce1077d5de74aa666f5edfba7f275efba78e8893c115148
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0.orig.tar.bz2.asc' apr_1.7.0.orig.tar.bz2.asc 801 SHA512:19b2b128c7c4cb40db06149c75325013a716c783e28e366c1bacf289fdb5d305e5779d8dc55a63729250ad3338cd4c726e133c788fe53ab3519f1bc8d4da6f90
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.7.0-8.debian.tar.xz' apr_1.7.0-8.debian.tar.xz 215848 SHA512:0a1b6bae27f482508cef5ec7b3ba8e576b50e4502635b7a0647c17a01aa6e02059c861b1d80ff42cb26530e158b6d38495ee50142088e5a59192c4e9f072c581
```

### `dpkg` source package: `apt=2.3.14`

Binary Packages:

- `apt=2.3.14`
- `libapt-pkg6.0:amd64=2.3.14`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.3.14/


### `dpkg` source package: `attr=1:2.5.1-1`

Binary Packages:

- `libattr1:amd64=1:2.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1-1.dsc' attr_2.5.1-1.dsc 2455 SHA512:c97d5a67b349de80610f52bdeee12a519ac5ba665ac79b86903c5e985b6d279157db89a8bd25b4d98099cbca6235eec37cda2ed2fad22817aeaa1995d9bdca9c
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA512:9e5555260189bb6ef2440c76700ebb813ff70582eb63d446823874977307d13dfa3a347dfae619f8866943dfa4b24ccf67dadd7e3ea2637239fdb219be5d2932
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA512:be4f3629ef66bd400bcdeaf8b6b1564dc729472a514d59fb4909a30f3269711dedea16002283e9aabbf83c374e0a3d70bc00f1136da0fed66a8184acdfd7e78f
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.5.1-1.debian.tar.xz' attr_2.5.1-1.debian.tar.xz 27948 SHA512:a383525a5b8e36ad1f54e411ed34a2afc283215df3870934d1302ab202189bc6bd30a407f718ed016163891040654ea5efd1f0bdcccccdd85395cd13cbcef0fa
```

### `dpkg` source package: `audit=1:3.0-2ubuntu3`

Binary Packages:

- `libaudit-common=1:3.0-2ubuntu3`
- `libaudit1:amd64=1:3.0-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0-2ubuntu3.dsc' audit_3.0-2ubuntu3.dsc 2850 SHA512:ba3775a2a0111abc6db05c38b876ec9b97d673ad8b796ef85b137f91e0d005cfe0acf75b3650f9b26ddcdc65f6be3fca71d8927e60b7b7c2ef60b66a4ee1cc09
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0.orig.tar.gz' audit_3.0.orig.tar.gz 1109442 SHA512:b82ec73c85a8ebb5108b526673d6fe08cbe0b51376788f3ea6ed5747c4612158462893e719496dffbd723f833f84383a2d1d55fd78a3ed985ecfd19545060c88
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_3.0-2ubuntu3.debian.tar.xz' audit_3.0-2ubuntu3.debian.tar.xz 21332 SHA512:995093406a707a37c6636ff8c5ad57ae8b6c8eb84e3847a886a0713939bda51dfa292c6b4b0f7adbfc85cc93e38db09dc1772528ba0f4b425df197a6ad8dbd12
```

### `dpkg` source package: `base-files=12ubuntu2`

Binary Packages:

- `base-files=12ubuntu2`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=12ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_12ubuntu2.dsc' base-files_12ubuntu2.dsc 1245 SHA512:b9eb4d5b8f80915afe36993ad1fd42b9d4e1a3b8d4a146ed7b0c14dcea3c5d32600d56862b1b8bc28b246bd41181b0380a5189f453483eab6cb5a9ab5cdc8de6
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_12ubuntu2.tar.xz' base-files_12ubuntu2.tar.xz 81800 SHA512:13928febbde4cd667398cee7b654f92d235d73aad28be6fdf015d94dbf1a7b7c9fa0b9ca58df0f19da34c1eea921c0f17e996c06b9f9e3fb9fe0ef1a9186ac5b
```

### `dpkg` source package: `base-passwd=3.5.52`

Binary Packages:

- `base-passwd=3.5.52`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.52
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.52.dsc' base-passwd_3.5.52.dsc 1757 SHA512:90239ac4d9cae59f0a602b2daefa7069fd87d383b313360eb8521feb54df6be0a57f68ea2b56dfc5901b039b88dcd9f79cd84dc803c109b0b082e1776e5498c4
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.52.tar.xz' base-passwd_3.5.52.tar.xz 54336 SHA512:c6f38e5955d45990af0b5d58217c4ff8f24c9c6897809934586871ba2ea550b8aeb5353ef6def53b5155493e3018215e4a6c7deb280d171d1ec4352af21f9a49
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

### `dpkg` source package: `brotli=1.0.9-2build4`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2build4`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2build4
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build4.dsc' brotli_1.0.9-2build4.dsc 2310 SHA512:95f6ef20a83f7ec19bc0671c9ee6a37f14af885b98933f4da96f44577b8e26b7f8b1a527cd8466abeb122af793a9e52d349e38bb90c4f1d7c357b6129d157622
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2build4.debian.tar.xz' brotli_1.0.9-2build4.debian.tar.xz 5712 SHA512:bfe1828044f5f71b21a2bd358c2808078f581143004f6bc2ca70179bd1f38494a9606a89b5e57b7104e7482f1678caf7cfb845faaaded0d03186919d15b3a5d3
```

### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `libbz2-1.0:amd64=1.0.8-5`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-5
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-5.dsc' bzip2_1.0.8-5.dsc 2206 SHA512:036a4d1824befdafa0ab69cbcc68df877948894e6bc2196ced010d535f36f5a7c3eb4cfa1626aa7f9ee7e5ae4d62709cbc272645a6acea67aa06c5c533e093e0
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA512:083f5e675d73f3233c7930ebe20425a533feedeaaa9d8cc86831312a6581cefbe6ed0d08d2fa89be81082f2a5abdabca8b3c080bf97218a1bd59dc118a30b9f3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-5.debian.tar.bz2' bzip2_1.0.8-5.debian.tar.bz2 26787 SHA512:6c39f23a4bfaf18ebe8c9cc2f970974ac429587f7f2ad8d11c53a5a8bdac1d857f23b40e57fe245021ecc30c8abc23a65970b8dd27a4b5a2f226b20bc51f6564
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

### `dpkg` source package: `cdebconf=0.256ubuntu4`

Binary Packages:

- `libdebconfclient0:amd64=0.256ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.256ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.256ubuntu4.dsc' cdebconf_0.256ubuntu4.dsc 2941 SHA512:953fc9f1bfbebfc2517de5ea530d52ebb4b5afedc13deffc887412f84de992b19553094cacbbfc8cd9312d1e1edcc64a1430f08de6889aa6a49502d35b17e264
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.256ubuntu4.tar.xz' cdebconf_0.256ubuntu4.tar.xz 279796 SHA512:f701b7b5b933e3f11d74c985905a7cd8f9fee3b4157f29216238be6784e51e3b9f57d19094a9c7ae78b117d545f8572b71f51207d5da500c1fafbbfde1c75e6a
```

### `dpkg` source package: `coreutils=8.32-4ubuntu3`

Binary Packages:

- `coreutils=8.32-4ubuntu3`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.32-4ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-4ubuntu3.dsc' coreutils_8.32-4ubuntu3.dsc 2283 SHA512:1659ed55a593b20330b3bbccd9a4f1674ae8ccae09e12f2147c13c0870403d0a329d465d41bb4dd7b6a490bf067f983e381c1252ad209c8136f4775c5c6da196
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz' coreutils_8.32.orig.tar.xz 5547836 SHA512:1c8f3584efd61b4b02e7ac5db8e103b63cfb2063432caaf1e64cb2dcc56d8c657d1133bbf10bd41468d6a1f31142e6caa81d16ae68fa3e6e84075c253613a145
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz.asc' coreutils_8.32.orig.tar.xz.asc 833 SHA512:9c73b35c9e8f7c2b8eff317afcb5aa3234c5f41c80d1882f3c2342906f3fdc876ae45d1256dd1b8fd3cb58c50925f3c13f93de5018626634fdca3c72c14a9acb
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-4ubuntu3.debian.tar.xz' coreutils_8.32-4ubuntu3.debian.tar.xz 40904 SHA512:351131f25757c7e9e2323ab362992177fceb8e8cc95af26c1abb13f26ded1d0f7fb3d4af40db7a0ff8698401a5ae41fc401622aee1fad12a6e8cbaaae46ce02a
```

### `dpkg` source package: `curl=7.81.0-1`

Binary Packages:

- `curl=7.81.0-1`
- `libcurl3-gnutls:amd64=7.81.0-1`
- `libcurl4:amd64=7.81.0-1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.81.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.81.0-1.dsc' curl_7.81.0-1.dsc 3024 SHA512:6c1248a33c088ab1ce12e7380e89bf6c08a5f3506aafe0a60c343c844b8884ecb284700b65dd6064ba062615cedc376b30c6c363dadee387a7c6b55fb17f4211
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.81.0.orig.tar.gz' curl_7.81.0.orig.tar.gz 4188040 SHA512:e3084f0fa083f7f93eac923edbfdddb5fd0a372b94673ba9d4427a2b95508898c15ecdf63b99a1c1f6cf3215e27b06cbaa2b7073df038d43b362e586f92495d3
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.81.0.orig.tar.gz.asc' curl_7.81.0.orig.tar.gz.asc 488 SHA512:92bc5ede831551285d67b03abe8400c609ad31c9d33e324ee5c41b92dd5c2a0245a09a396bd76807b3e44bcfef944b1e16ac266264f7b85d27cc1c072a6e82bd
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.81.0-1.debian.tar.xz' curl_7.81.0-1.debian.tar.xz 36364 SHA512:96dfca3ffe41b43500d1650523f590b150307d710b568fe4da79519dec47ce605ed2e4f852fd320947d16f74616f736eca5259380a22feca67bc40f6ae0b2dd9
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg2-3`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg2-3`
- `libsasl2-modules-db:amd64=2.1.27+dfsg2-3`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-2.2-clause`
- `BSD-3-clause`
- `BSD-3-clause-JANET`
- `BSD-3-clause-PADL`
- `BSD-4-clause`
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
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg2-3
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg2-3.dsc' cyrus-sasl2_2.1.27+dfsg2-3.dsc 3260 SHA512:fd9f96afe984bdba91fb3b3dd19ac98bbc4611133ea55c72753be80af08adbccff3d2bb381be2d18d808f541fa0375742e0c9e4ef4b7dcb85c82a2010d662d97
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg2.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg2.orig.tar.xz 829892 SHA512:13337dfcc57ea8fec471ee0f2a0f6b58fb92907ad0899a4a8afaba957c5da302924e71c9fc4a61bbc913a4ee2ea74b05772cb26ed58d5724a312bb20a8b6a4cb
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg2-3.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg2-3.debian.tar.xz 92560 SHA512:75f12a41a92f048ae895729d4f8634c9ea0de27042ea4e264154dbb5c153358f7766f26419d25cc5951be4a89177f67dd8af2bad585de87a3faec2a899394d66
```

### `dpkg` source package: `dash=0.5.11+git20210903+057cd650a4ed-3`

Binary Packages:

- `dash=0.5.11+git20210903+057cd650a4ed-3`

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
$ apt-get source -qq --print-uris dash=0.5.11+git20210903+057cd650a4ed-3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20210903+057cd650a4ed-3.dsc' dash_0.5.11+git20210903+057cd650a4ed-3.dsc 1686 SHA512:896f69b46297284f7f01f3d12833cefd80b1bbb540a0388273dcb48d7db9790e1c1591ce656c048455278bdf37c2bfe3a03068885ed19089332a0ccb5763600e
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz' dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz 133320 SHA512:eced6bc60ca6ba4394a2ee65d8c6b88eca729c43e47053fc01dec5500ebe002a12f536c128c3fd821a2eb61b97e92c8a0be6d4532926479ce4b7d986be109cb7
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11+git20210903+057cd650a4ed-3.debian.tar.xz' dash_0.5.11+git20210903+057cd650a4ed-3.debian.tar.xz 42656 SHA512:1668d3d85ec32e9933b8b5b71d44be0fcb772a7b6d485cac1aff09868a1099b5a01bcb6ee17685ad08268e54a92e70affd461039b1e3268bd2abb557caf45feb
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8ubuntu2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.8ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8ubuntu2.dsc' db5.3_5.3.28+dfsg1-0.8ubuntu2.dsc 3245 SHA512:41b929ded6b945733dadc66fb4438b9ac87fc674163a5eadee584fa43df8115bde9e35c7ae0432dfe92b562ab0d69ef09688a485a514819b69223ef2fddbf019
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA512:50cb87bc3f24065839ee2932e82af032b236b290ebe89983076f503c6c62c5f36ff93d7847a3f68b2b19f35088fbab5d3ac6a34553d07e8148e68e9a3f079a12
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.8ubuntu2.debian.tar.xz' db5.3_5.3.28+dfsg1-0.8ubuntu2.debian.tar.xz 31952 SHA512:03f093df95a539fc367a657543998e9efe2dfede8fb1e4289421698cbc16b393f30f428b66001fa456b7b15b6b57e9c1dc5953328abe88ba5535c07a50bba7a6
```

### `dpkg` source package: `debconf=1.5.79`

Binary Packages:

- `debconf=1.5.79`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.79
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.79.dsc' debconf_1.5.79.dsc 2082 SHA512:e12cd4ba94dbfecb277efb2424a4adf9e11f5685afa9574167e59cc78b9a25a385c297eaed1fb29f72347f716aba0ad1f887cb28434d4f84bd92d2b6dd19e972
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.79.tar.xz' debconf_1.5.79.tar.xz 570588 SHA512:08a19a835422ff81d262e2a7212d42ce636e8fa4b58fb9fb220838f3d497e5c179202fcd3e79afca3b697d074749dbf6a81bfbaea54872f75a818d0cf49ab625
```

### `dpkg` source package: `debianutils=5.5-1ubuntu1`

Binary Packages:

- `debianutils=5.5-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.5-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.5-1ubuntu1.dsc' debianutils_5.5-1ubuntu1.dsc 1998 SHA512:450e2f61d20f60ae8eef267ab6cb33d166d3182d7a72c3c463d07dfbafe48308d78280efbe8b127f3aa1c1cf59c2128a38899dd7223bcb9b588fca5ba8f6828a
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.5.orig.tar.xz' debianutils_5.5.orig.tar.xz 104448 SHA512:230310428ee7c145c74bb666ae729754352295230f38ef4e22f7566970c5186d607cd827a5603a678815bd48d4a1eb2716f55c32494ec75eb665651da6a56e6a
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_5.5-1ubuntu1.debian.tar.xz' debianutils_5.5-1ubuntu1.debian.tar.xz 68584 SHA512:85ff41234f2dfb8efd1ddff4349bcc22f958e23acbd7fa262695b397117d6415f003df000fce8acfb2f15eef9259cca15884b5f0004c4133194c6c2c69d85c36
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

### `dpkg` source package: `dpkg=1.21.1ubuntu1`

Binary Packages:

- `dpkg=1.21.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.1ubuntu1.dsc' dpkg_1.21.1ubuntu1.dsc 2271 SHA512:158a3086236c22856faacb232d108f7e006a22f3d8b52e0c4147dbd6010e3534babfc2cd62fe66a59747a565c1699c092631546003113a2bd9a0e4074201b256
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.21.1ubuntu1.tar.xz' dpkg_1.21.1ubuntu1.tar.xz 5015868 SHA512:fe2443e4a498d9f74e601795b2824cb76c2938aa355dea0b4c5fee4432789271b3ecddf387b87dac938012044d1effe232e07f7afa45079bf849f38118895a58
```

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

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.46.5-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.5-2ubuntu1.dsc' e2fsprogs_1.46.5-2ubuntu1.dsc 3103 SHA512:9fd85f269a28246c9b878ab1b61753f4b42f5f23e7e3d7a560dd5124d67ad9e27fc2d76720d5670f39f47dfae93edf21472203d577a613097241dc9905c11341
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.5.orig.tar.gz' e2fsprogs_1.46.5.orig.tar.gz 9530158 SHA512:1a3496cb6ac575c7a5c523cc4eede39bc77c313a6d1fea2d303fc967792d75d94e42d7821e1a61b7513509320aae4a7170506decf5753ddbd1dda9d304cc392e
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.5.orig.tar.gz.asc' e2fsprogs_1.46.5.orig.tar.gz.asc 488 SHA512:b288fa2418a85750673743cb58faf10537e2c79a5c2ec8b0d59435316f00006424195556ccf78fa023b67b05a29cd85bf9d96c14c166847d71a1d79b189c1d05
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.46.5-2ubuntu1.debian.tar.xz' e2fsprogs_1.46.5-2ubuntu1.debian.tar.xz 85096 SHA512:721aa2ceb80c9eb99eef514bbdf081d0f87dbbad0e0dd58f165d2659ce353918169ae26c96d9be8fe6a2062bb4c0788b3189002bf6f8543c2faab44341ec0cb3
```

### `dpkg` source package: `expat=2.4.3-2`

Binary Packages:

- `libexpat1:amd64=2.4.3-2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/expat/2.4.3-2/


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

### `dpkg` source package: `gcc-11=11.2.0-14ubuntu1`

Binary Packages:

- `gcc-11-base:amd64=11.2.0-14ubuntu1`
- `libgcc-s1:amd64=11.2.0-14ubuntu1`
- `libstdc++6:amd64=11.2.0-14ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gdbm=1.22-1`

Binary Packages:

- `libgdbm-compat4:amd64=1.22-1`
- `libgdbm6:amd64=1.22-1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/gdbm/1.22-1/


### `dpkg` source package: `git=1:2.34.1-1ubuntu1`

Binary Packages:

- `git=1:2.34.1-1ubuntu1`
- `git-man=1:2.34.1-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.34.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.34.1-1ubuntu1.dsc' git_2.34.1-1ubuntu1.dsc 2948 SHA512:e6b8158c48af6dbd9f4befb5e8be832bd259ebda8dc04c4dbea9944a283f145b58080a39d91aeadc4066ddadbf86981c6281453a88a9d5c9029a5b312e9fe213
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.34.1.orig.tar.xz' git_2.34.1.orig.tar.xz 6623760 SHA512:a1a8e9e6f64b1da25508fbd2f783564dcdbe181fb5ff1ebab3bdac6db6094e18acc334479a1abf22ac17ce4f733cc3e10a664db9ab234cd523735a3f027b42db
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.34.1-1ubuntu1.debian.tar.xz' git_2.34.1-1ubuntu1.debian.tar.xz 702840 SHA512:0eb2102c0dbda8f9688c259aa0bb81e887c3c61388b353f8332b1af350947c7902fa35e813c9c2a0114ca383cec6504e2f621c75d4024617143a38ebb69d19ca
```

### `dpkg` source package: `glibc=2.34-0ubuntu3`

Binary Packages:

- `libc-bin=2.34-0ubuntu3`
- `libc6:amd64=2.34-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.34-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34-0ubuntu3.dsc' glibc_2.34-0ubuntu3.dsc 8957 SHA512:c743d6fc4cce79bdbc8d45c86f5ca058d77eeec8c94b743a7c2d9e1344b0b60d9eb7f8c0bb01110603e3d5a8739d918e63f41a8d3dbfe328828f3683d2f0e921
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34.orig.tar.xz' glibc_2.34.orig.tar.xz 17301232 SHA512:15252affd9ef4523a8001db16d497f4fdcb3ddf4cde7fe80e075df0bd3cc6524dc29fbe20229dbf5f97af580556e6b1fac0de321a5fe25322bc3e72f93beb624
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34.orig.tar.xz.asc' glibc_2.34.orig.tar.xz.asc 833 SHA512:5b92e315d81a0a157f15b8ac29acddbf4669b51a72483bba4b1769db78986ec9814b23be3d7ac3779cefb0a38070af7ecb37dc1667e1cb3ede8c34cb1ca5d7f3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.34-0ubuntu3.debian.tar.xz' glibc_2.34-0ubuntu3.debian.tar.xz 883372 SHA512:4ca38eecd987f49ee36b5855528b92632125953b118fd39a9e8bb0b55bd77cedc1f2a17ee33fb60465714ff2f396a247cc27e954a1179805cb66bcdd9bc0ef0f
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1+dfsg-3ubuntu1.dsc' gmp_6.2.1+dfsg-3ubuntu1.dsc 2355 SHA512:b41211a64cba1afee1ea7924d38581b26b36f0495ad42be6d25b7175d5fa1e000378a5d36dd80087b0e7d4495620edb1e7e1b32d6c1085a8cdf0a4cb460a0558
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1+dfsg.orig.tar.xz' gmp_6.2.1+dfsg.orig.tar.xz 1853476 SHA512:801948b7dcf592959ea387a86bee34dfb4e02c5e93815a785fc46174899ba22129853a3e34109a6df86048a144765c5f39e65fddfcecba879cc60da62f32fea0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.1+dfsg-3ubuntu1.debian.tar.xz' gmp_6.2.1+dfsg-3ubuntu1.debian.tar.xz 40996 SHA512:d7e0a1165a42b11a26a0f9232193db41ce2e7b1f5ea50d258e156fc9d80f9a74b6739491ec73cc1e909a3d09e029f90c3be1460c993690c5081ef8c6a169a4c3
```

### `dpkg` source package: `gnupg2=2.2.27-3ubuntu1`

Binary Packages:

- `dirmngr=2.2.27-3ubuntu1`
- `gnupg=2.2.27-3ubuntu1`
- `gnupg-l10n=2.2.27-3ubuntu1`
- `gnupg-utils=2.2.27-3ubuntu1`
- `gpg=2.2.27-3ubuntu1`
- `gpg-agent=2.2.27-3ubuntu1`
- `gpg-wks-client=2.2.27-3ubuntu1`
- `gpg-wks-server=2.2.27-3ubuntu1`
- `gpgconf=2.2.27-3ubuntu1`
- `gpgsm=2.2.27-3ubuntu1`
- `gpgv=2.2.27-3ubuntu1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.27-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.27-3ubuntu1.dsc' gnupg2_2.2.27-3ubuntu1.dsc 3755 SHA512:c129f8e93740857ab4d2f00bf975e9501e9eb25ac13aa2cc88ef2a29bee35b846866c210fdb2bc8c9178657d0ca64d5c683223f2df2136f574b679b591f8713a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.27.orig.tar.bz2' gnupg2_2.2.27.orig.tar.bz2 7191555 SHA512:cf336962116c9c08ac80b1299654b94948033ef51d6d5e7f54c2f07bbf7d92c7b0bddb606ceee2cdd837063f519b8d59af5a82816b840a0fc47d90c07b0e95ab
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.27-3ubuntu1.debian.tar.xz' gnupg2_2.2.27-3ubuntu1.debian.tar.xz 66004 SHA512:fa934301fe7fa4bc80ce4350a2f310efb28fcd895a11fbafdf32e6058429e502519574a64c38f171d4b3f315696def13cb33cfc4b26c7f361f4815139ebae7d6
```

### `dpkg` source package: `gnutls28=3.7.3-4ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.3-4ubuntu1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.3-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.3-4ubuntu1.dsc' gnutls28_3.7.3-4ubuntu1.dsc 3564 SHA512:9fac0e1be78d2494426033728657f97ee93ece30fae655818ad052d17ad10888f01767fd3837ffa4ba9c06fd0bbd3df4325228a40713a84d8657b6423ab1e233
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.3.orig.tar.xz' gnutls28_3.7.3.orig.tar.xz 6119292 SHA512:3ace744affe23e284342658d6d2d2de49dd50065489cbc8be18fc7d38187253e5268ca54027ce5cd517056c249ac039a7481e4548cec04325de37ae85617d077
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.3.orig.tar.xz.asc' gnutls28_3.7.3.orig.tar.xz.asc 833 SHA512:cd0d30298377deddf20a835863b71e3f119588061f659906ad2684004758943179531508b1c77c730e930e2131148095e60ad9be365353cce772472d5f5345df
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.7.3-4ubuntu1.debian.tar.xz' gnutls28_3.7.3-4ubuntu1.debian.tar.xz 68892 SHA512:154bee93d15779dd125332edc1aa7071c641547b1b9e60bdfbf331b000578b09e65feaa3d57b8d451beec3ef3b092a7eb8abf15f92ce22532f4edd5bcdf442e6
```

### `dpkg` source package: `grep=3.7-1`

Binary Packages:

- `grep=3.7-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7-1.dsc' grep_3.7-1.dsc 1644 SHA512:4e2fd6b868944336782d4fe4d4b4edc7eae6f81d25382bb300e6e7868924ac2310c74a3713e63f9cee1d91f6a1670ecb762a9cb46dc9236611321bb44cb7c86b
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7.orig.tar.xz' grep_3.7.orig.tar.xz 1641196 SHA512:e9e45dcd40af8367f819f2b93c5e1b4e98a251a9aa251841fa67a875380fae52cfa27c68c6dbdd6a4dde1b1017ee0f6b9833ef6dd6e419d32d71b6df5e972b82
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7.orig.tar.xz.asc' grep_3.7.orig.tar.xz.asc 833 SHA512:9db28883b696fbbb0fad32f4ecd168954dc475d5f0a8f2b4f960ff615ef7dd8348a7caaee85a96287824472a29485ff921af121c582083ca5ad5c30960f99cf4
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.7-1.debian.tar.xz' grep_3.7-1.debian.tar.xz 18104 SHA512:6aae70cf01e123396913d22a1816a2cc58fcfd21fcad80a3864e744f518417ddc54c70af5644ad3b673f216e6aba31b6b2fe526aff2bbaa5c3ade9eb33169a68
```

### `dpkg` source package: `gzip=1.10-4ubuntu2`

Binary Packages:

- `gzip=1.10-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-4ubuntu2.dsc' gzip_1.10-4ubuntu2.dsc 2294 SHA512:38b7685cc695562beccdf90d7cff0ae5433591eaca824af93802a4cbcd389c10eef42f2ab6227bf1609dcfbc0c0d186f54f3075b1ee3c29a9dcbe3d36ab93995
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA512:7939043e74554ced0c1c05d354ab4eb36cd6dce89ad79d02ccdc5ed6b7ee390759689b2d47c07227b9b44a62851afe7c76c4cae9f92527d999f3f1b4df1cccff
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz.asc' gzip_1.10.orig.tar.gz.asc 833 SHA512:74727fb3a8b64f81b4dd2d941fa750a789c482d7ae604d0ecfbe5ec623780efc7c5f0e51d65e7b99c2f097c5cd6585cc3a0f1b31abb03306156e0d410d9f0186
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-4ubuntu2.debian.tar.xz' gzip_1.10-4ubuntu2.debian.tar.xz 34464 SHA512:94bd778ebaf6c4910e61ca4a803429b954f26da6c485b03a0d8f28b614e72931be0c09256f709fe18b19dd44994adc0de8691b24e620be8750cf7343b1542f72
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

### `dpkg` source package: `init-system-helpers=1.61`

Binary Packages:

- `init-system-helpers=1.61`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.61
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.61.dsc' init-system-helpers_1.61.dsc 1927 SHA512:7f3ddd0f30ceebb439cf62a713dac8b375190aed56c3417ef5a39dc4ee34a02a41e58c1f7f0e7950711a2bb2be1d63a75a886b35c5031c84ac82c70e28ff07a2
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.61.tar.xz' init-system-helpers_1.61.tar.xz 41244 SHA512:ff48f12612ba76d28eb86ea3e1252302271b2ad133017cd23635870f4f67ac4c212055a3b74c18bc6daa74f079a794ddf5fe9c1034a873fdcc2b7c77d7a2e2d0
```

### `dpkg` source package: `keyutils=1.6.1-2ubuntu2`

Binary Packages:

- `libkeyutils1:amd64=1.6.1-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.1-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu2.dsc' keyutils_1.6.1-2ubuntu2.dsc 2187 SHA512:cd3096416b46b2020d64d85ebf245d4ddcb1aab58d510a62b356b7ad80e71768894fced728f7a1b2411dd59d65080eab11f6f8e38403a84d5dcca36c76c9c8ac
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1.orig.tar.bz2' keyutils_1.6.1.orig.tar.bz2 97232 SHA512:ea6e20b2594234c7f51581eef2b8fd19c109fa9eacaaef8dfbb4f237bd1d6fdf071ec23b4ff334cb22a46461d09d17cf499987fd1f00e66f27506888876961e1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu2.debian.tar.xz' keyutils_1.6.1-2ubuntu2.debian.tar.xz 14428 SHA512:52908d27d030311c2b949326b31d42c4ed9f090589133385f87a0b1ac38f406193aa8817306de9be85b42efdb33a5e035c90c7636bed2cf36cf8536a897fee24
```

### `dpkg` source package: `krb5=1.19.2-0ubuntu1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.19.2-0ubuntu1`
- `libk5crypto3:amd64=1.19.2-0ubuntu1`
- `libkrb5-3:amd64=1.19.2-0ubuntu1`
- `libkrb5support0:amd64=1.19.2-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `libbsd=0.11.5-1`

Binary Packages:

- `libbsd0:amd64=0.11.5-1`

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
$ apt-get source -qq --print-uris libbsd=0.11.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.5-1.dsc' libbsd_0.11.5-1.dsc 2292 SHA512:635f85618e9bcf22abbe73a6864b87d34c4e9d75bc619cab4e487d0ccbb52e1c006258cb47c8b892869adb5d645303fbff3eb57618f2dc862120f741cfbe175c
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.5.orig.tar.xz' libbsd_0.11.5.orig.tar.xz 409972 SHA512:c52c19eddd53630aca14f9f6221f7b84aa9cc798b4bb91e867822b161793313aab872ac1c0350d29312a72fee6e2061f3910ff918b724ec171d8c9de5837c841
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.5.orig.tar.xz.asc' libbsd_0.11.5.orig.tar.xz.asc 833 SHA512:24a3fb414a3a354284c76724d65225619820f3f6b597ed8d163ed99f19ec433465f909fe047758f83a7cd6fc8ee2676478420c77cb2f0b8b69ffa7a690c8c17f
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.11.5-1.debian.tar.xz' libbsd_0.11.5-1.debian.tar.xz 17604 SHA512:438911ae479952b00aa81cdf2f12863b82a01bc2abf3acb4bf22223f4c851504a77217087b2e2edabf6cf61187314f1c3061f2794de7a38abd953451e2f0d931
```

### `dpkg` source package: `libcap-ng=0.7.9-2.2build2`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.2build2`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2build2.dsc' libcap-ng_0.7.9-2.2build2.dsc 2130 SHA512:d6bc97f045a84143cc1c806d5c7a5151416a7a6083ee3d093ac3b3db318d327b50c0b8eab15a51e749c79ccb173d17f0f9e7ee8628c5d980ec8fbf9b9eebcd99
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA512:095edabaf76a943aab0645b843b14e20b1733ba1d47a8e34d82f6586ca9a1512ba2677d232b13dd3900b913837401bb58bf74481970e967ba19041959dc43259
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2build2.debian.tar.xz' libcap-ng_0.7.9-2.2build2.debian.tar.xz 6388 SHA512:242db3a87a06cb67197b2b8a5dee0240f82d53ca315f23409d19488ba78b37241c190c12de8e2ff7f71a0a2e3c091c01d2f8ae29cfe7fd6d283df3facfe86466
```

### `dpkg` source package: `libcap2=1:2.44-1build2`

Binary Packages:

- `libcap2:amd64=1:2.44-1build2`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.44-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1build2.dsc' libcap2_2.44-1build2.dsc 2228 SHA512:8892feeec1016a5c0755d9b2d90922f44e2575d72fefe1dcc7364d8bd1df46f73cc26b12a7ac66e921918e848f2756571acebc40e39728fdf95980a18dbaa03f
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44.orig.tar.xz' libcap2_2.44.orig.tar.xz 125568 SHA512:1bb323ca362923bd6bd0e2e4639cf8726975165a620a243b31e797056439eb7efb2bfbc8e5521636783a86c7415b2037b1638c98747b79183ca7d3d42a04ff20
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.44-1build2.debian.tar.xz' libcap2_2.44-1build2.debian.tar.xz 21204 SHA512:34cd8d0c043cabced3b5c4bca35a7ad5a8ecc72d28cbf84dc11a464d4a1a43eb680b430bbff50929547bb895c1cfc356198fd971d70ee0fec6b62eb7d2909fae
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

### `dpkg` source package: `libedit=3.1-20210910-1`

Binary Packages:

- `libedit2:amd64=3.1-20210910-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20210910-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20210910-1.dsc' libedit_3.1-20210910-1.dsc 2208 SHA512:1d8510327cc9f3670e55ede42fb963b3ec19b568772687f6e8f3346525fac81f793a3e6ac39b662893c13c5b769f6a40989c0dc719c84e0f05de820fc1b5b15c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20210910.orig.tar.gz' libedit_3.1-20210910.orig.tar.gz 524722 SHA512:b7361c277f971ebe87e0e539e5e1fb01a4ca1bbab61e199eb97774d8b60dddeb9e35796faf9cc68eb86d1890e8aac11db13b44b57ccc8302d559741fbe9d979e
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20210910-1.debian.tar.xz' libedit_3.1-20210910-1.debian.tar.xz 15080 SHA512:963108537cede59b5590f18ee2ae20838a9d80d8a248e0da4ddc9b01597c50495d6890ce148a6bbac73ab8e8209aa8b262f93c73dd64325482e8ce6b60c3eb76
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

### `dpkg` source package: `libfido2=1.10.0-1`

Binary Packages:

- `libfido2-1:amd64=1.10.0-1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.10.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.10.0-1.dsc' libfido2_1.10.0-1.dsc 2588 SHA512:c01468b2452f024b1c3f9f758dc65cc84f9bd2bd3bec1c07da85c50a60aefbca0fdb4bc35c93ee4c8499c29bc2f3581c470a027ddec30f56b3269bdf31f585fe
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.10.0.orig.tar.gz' libfido2_1.10.0.orig.tar.gz 591372 SHA512:ba03e25d3f42f11cec74dee48c853ae35d03600f24ca06d2b751840408a132290fe22461372ae42ae31419061a63d9908c20a2c0cf3c0c9c8dbc46c34916784f
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.10.0.orig.tar.gz.asc' libfido2_1.10.0.orig.tar.gz.asc 833 SHA512:1bdd9c0c161f40444297b0ffecbcf2117d0eb27e4dd28aacc9a84b05746af4fa8cdda9b1c771250c5c14131162ef71cc14b5d9f070e61e9304d47413ee678da3
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.10.0-1.debian.tar.xz' libfido2_1.10.0-1.debian.tar.xz 52432 SHA512:9b2b3c9a9352d72020048a5c50d492e774c772d888bf6926ad5a09e20f388c7219969a5ca7fd70e6615444bd8de25c91f7b4b4f1fd6096b9014349dffbef55ae
```

### `dpkg` source package: `libgcrypt20=1.9.4-3ubuntu2`

Binary Packages:

- `libgcrypt20:amd64=1.9.4-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.9.4-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4-3ubuntu2.dsc' libgcrypt20_1.9.4-3ubuntu2.dsc 2907 SHA512:cab99aef1d24a38dbb9f7af9d66605db14d6b7e87a84fa2b4daf56a162d9f7260002fec2cbc32a852440bf83764a88ac85a48edfeb949d6dfa0963dc7afa7ab4
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4.orig.tar.bz2' libgcrypt20_1.9.4.orig.tar.bz2 3239704 SHA512:d0e117ac73c94d70e9521ee1e6328691498cc8328f8c4e21338096908f5c04c7b838966eb63d59494565f4e19f506c07dab4f4d922150d75610d9f7b57abbf60
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4.orig.tar.bz2.asc' libgcrypt20_1.9.4.orig.tar.bz2.asc 228 SHA512:5fbc2f52ff8a9f2b254791a0d127b012a3648a03d26e043af2ab63d05f69045492581462ba485ecf005a171ea391175bdc73350aa0e76f8b5f75c64a4d685d49
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.9.4-3ubuntu2.debian.tar.xz' libgcrypt20_1.9.4-3ubuntu2.debian.tar.xz 35104 SHA512:94ff8dc2077eeeb13889abcbbcb02443ae32dd236c4731331e602809cce9ce037a5632d0094fa5968aff2c4963a9d7cf089453d934057642e364520e67a87c77
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

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.43-3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.43-3.dsc' libgpg-error_1.43-3.dsc 2270 SHA512:c0cf8b16d720d89b69b5eb5cf22bf7bb0605892ba110100d3b30370fc93c167bda2f501e53e70a2599024bc40c1e509d06e39f68f3be63312967e4308249f0b8
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.43.orig.tar.bz2' libgpg-error_1.43.orig.tar.bz2 999006 SHA512:36769a62d0b4b219a6d58195bed692e34d3b0313f628b1036055ca34b69332edbe6bcdace9855a60d06e7be5998dc13bf1305d0b2bb211a4d8f701e85040961c
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.43.orig.tar.bz2.asc' libgpg-error_1.43.orig.tar.bz2.asc 238 SHA512:1bd12acc57bb394947dec51b70fe067f717e591484be164cafff3ac47a6bacc101f7ac64fbae350233bc76a0002981fb3fbe53db73dc914db52694b8588cecc1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.43-3.debian.tar.xz' libgpg-error_1.43-3.debian.tar.xz 19264 SHA512:bbd7615b02707405efddd4bb1dee355024bb7089770453a2addf7e722c15c2cfbebc3012c9db848f3f55eb4c66f5b9487877e8d94322d8dc1d2731876b4d8281
```

### `dpkg` source package: `libidn2=2.3.2-2`

Binary Packages:

- `libidn2-0:amd64=2.3.2-2`

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
$ apt-get source -qq --print-uris libidn2=2.3.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2-2.dsc' libidn2_2.3.2-2.dsc 2206 SHA512:fd7d1eb9c5289eca9288bf25349a2544493df991de2d092c15cc16d2e7011a6fa46e6e2557a0ec9d76a2195a81456f0c9ebaa03b2de968f78f57de51ecc92b7f
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2.orig.tar.gz' libidn2_2.3.2.orig.tar.gz 2169556 SHA512:958dbf49a47a84c7627ac182f4cc8ea452696cec3f0d1ff102a6c48e89893e772b2aa81f75da8223dfc6326515cca3ae085268fbf997828de9330c3a351152f1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2.orig.tar.gz.asc' libidn2_2.3.2.orig.tar.gz.asc 488 SHA512:0559b51b37c7937f3e1f8bf9de9b193f137f16b79d6673f85691a4f4a12ec132568e913848a70136f8522118817f7ecaa8432d353a5eff6b99a7be8719421fe0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.2-2.debian.tar.xz' libidn2_2.3.2-2.debian.tar.xz 15840 SHA512:b17f0c85a3bcddbf89a293c0d9dd217abd78b4bbe9a6536cb2daeeb73468d1d6ee9ec5b6383baaf4a4cef045b127176b577ef00d449b47bbe9e8257ed2e83aad
```

### `dpkg` source package: `libksba=1.6.0-2`

Binary Packages:

- `libksba8:amd64=1.6.0-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.6.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0-2.dsc' libksba_1.6.0-2.dsc 2470 SHA512:59ea4eba827de2824e5c9a477f2c61cccbda47baa86089bfc655be811c528b150412fb8ebd6c18fa933286714e75264e513a7b5e70106e67dbc9171d7d8d9252
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2' libksba_1.6.0.orig.tar.bz2 662120 SHA512:a7c76d41dfd8ec6383ac2de3c53848cd9f066b538f6f3cd43175e3c8095df51b96d0a24a573481c0c4856b09b7c224e2b562d88f5c0801e7acfb582ea2739c2b
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0.orig.tar.bz2.asc' libksba_1.6.0.orig.tar.bz2.asc 228 SHA512:fc381ea66eefdb431a5248fa3ac0751d7343d7f99cc7ebf7621b0763e6e31a80b45c5e17b09bbc7c1c1154e6a0152af1f13798f64959ac63f50b789ec046d7a3
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.6.0-2.debian.tar.xz' libksba_1.6.0-2.debian.tar.xz 14524 SHA512:bafd10989a76221cd3f4e39541bad24691a55a670d4f60632571a3645152fd812063c28dc113cc59ef377238d0f8a24fafbd719c891f4f0a48ea02db9a144d98
```

### `dpkg` source package: `libmd=1.0.4-1`

Binary Packages:

- `libmd0:amd64=1.0.4-1`

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
$ apt-get source -qq --print-uris libmd=1.0.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4-1.dsc' libmd_1.0.4-1.dsc 2248 SHA512:a9f55143e0b67a898b6f258b65134c54d5f2ed6aac9bcefa54d1e51c39ab7a3683a43429def2b55304ff9dfbda6c02118b191d3a7cc3fc8c511aebcec6de4111
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz' libmd_1.0.4.orig.tar.xz 264472 SHA512:731553ecc5e0e1eb228cced8fccd531fe31fb5c7627ca30013d287e1aeb8222959cf7498fbb7414bbabb967b25d4e8b0edd54fc47f6ccf55fc91087db0725ce3
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz.asc' libmd_1.0.4.orig.tar.xz.asc 833 SHA512:ec4b60a721da1f315fad73daa8ee620f44a53f17a30506c4d63b154b3abde19bb248b2ce6b83b989589e2a9184ebbe1b870e83181e18a4147d75617579d10504
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmd/libmd_1.0.4-1.debian.tar.xz' libmd_1.0.4-1.debian.tar.xz 10144 SHA512:c9a8a682f86089c3f16e120bcf48fd86edbdc895a3e5650599f29ca0829943d53cd7b886a33ccb9c184159efcdc76003c7c6464d3eaae50598350b69e3e029dc
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

### `dpkg` source package: `libpsl=0.21.0-1.2build1`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.2build1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1.2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.2build1.dsc' libpsl_0.21.0-1.2build1.dsc 2265 SHA512:9b04bd6f8fe7b922577ba6a712c226f2199e9451d5593ff9ccf672949a89a3844dcfd8d7da8d42de308603f33ffe3dda485105e81361f5ab7df646776f37fbff
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA512:b7466edb9763f94a65330dbb3c19586f9c7b01e20ddedb38ca2fd4c9ee5764a4f9b3291dc4b76659b45425d954f15973345f917b2cd2de72ea731e8c41f2a265
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.2build1.debian.tar.xz' libpsl_0.21.0-1.2build1.debian.tar.xz 12804 SHA512:5b118dd83c7ddc787ec1d8f88e899cfdfe4739a05fc31905552a8d0fe78898e4c6d031835d5b93aa23a6e17c82cc9e12e1fc9ac4881cb6c6650a2bde045af013
```

### `dpkg` source package: `libseccomp=2.5.2-2ubuntu2`

Binary Packages:

- `libseccomp2:amd64=2.5.2-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libselinux=3.3-1`

Binary Packages:

- `libselinux1:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.3-1.dsc' libselinux_3.3-1.dsc 2299 SHA512:157c6a1aaabe8e9f3fa11e1237283b5ba6aa6112c25c76e75f8480c4f55829d91dbb1b62f24b9da9f991e87824212795cd16b4207588ea73a58379c0aacf1ea3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.3.orig.tar.gz' libselinux_3.3.orig.tar.gz 206826 SHA512:9a89c05ea4b17453168a985ece93ba6d6c4127916e657c46d4135eb59a1f6408faa0802cc2e49187defbde5247d659037beee089877affbab3eab6af3433696c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.3-1.debian.tar.xz' libselinux_3.3-1.debian.tar.xz 23920 SHA512:4d880d10160d9c4a2757c6a4874b9ed57d6379da6711f9a6a0ff6b5f4aa26a94aecc28030b6b75cd14b7d1ca120df6aeef956dbe4ab39a9d90012dff467f4889
```

### `dpkg` source package: `libsemanage=3.3-1`

Binary Packages:

- `libsemanage-common=3.3-1`
- `libsemanage2:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.3-1.dsc' libsemanage_3.3-1.dsc 2320 SHA512:e183f5bd7b04354f8d2c21bd23f946774f566fff92e20f351e64d78a117388db0f562c193cbf2ceca75cac0072b0d798f6836eb387bffaffb1491b2b8580615e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.3.orig.tar.gz' libsemanage_3.3.orig.tar.gz 178890 SHA512:6026d9773c0886436ad801bc0c8beac888b6fb62034edeb863192dea4b6ef34a88e080758820fe635a20e048ac666beee505a0f946258f18571709cca5228aad
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.3-1.debian.tar.xz' libsemanage_3.3-1.debian.tar.xz 17780 SHA512:e2482e3dd64d94a37285682551735a43d670f3c0ec899b2821e86a414c7f32f94c513000ff39172769b529b69264103136cecaa377060267410e0e4331ce91e7
```

### `dpkg` source package: `libsepol=3.3-1`

Binary Packages:

- `libsepol2:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.3-1.dsc' libsepol_3.3-1.dsc 1764 SHA512:e2b879cacf0610a5e577610e850e08679166aab7c775a735c0d005861beeb98099c731869b592ff3a4cc4b24ad248b40cd2fce458f92ba5c7845f0421feedf0c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.3.orig.tar.gz' libsepol_3.3.orig.tar.gz 482546 SHA512:fb6bb69f8e43a911a1a9cbd791593215386e93cb9292e003f5d8efe6e86e0ce5d0287e95d52fe2fbce518a618beaf9b1135aea0d04eaebcdbd8c6d07ee67b500
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.3-1.debian.tar.xz' libsepol_3.3-1.debian.tar.xz 14956 SHA512:142893edbfcf12499d57f723da8423d35b1927bf9027493b112f0b0f473aec1b995d38b8b9434d385232e80fb5df3a2fa75a101704dc4cab7680ec9746728681
```

### `dpkg` source package: `libssh=0.9.6-2`

Binary Packages:

- `libssh-4:amd64=0.9.6-2`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6-2.dsc' libssh_0.9.6-2.dsc 2745 SHA512:235200b64a297a969562085905dcc6f6b8fc8e962a7d1fc6d43a630ad1cac02b60c51ba9acdb976888ef47c67ceda6ebad536bdf494d414d364fbcccb3463102
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6.orig.tar.xz' libssh_0.9.6.orig.tar.xz 1053056 SHA512:4040ec4af937e95be2e41313ef6d4db60b46b8d4dea10c09402398127c1d1ca8843392d207088aeee3c7ef631c6ae7b66861327dcebf78ed3af0723777619fd1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6.orig.tar.xz.asc' libssh_0.9.6.orig.tar.xz.asc 833 SHA512:1b6223efe9e4ce864cd8d97d517f9f0d38c1cd502b5874fdc6a58731038c2830a72ce753f02fc062d9d4d5922107ec9a2e62fe24a704bb5dec0dcfecdb569fe6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.6-2.debian.tar.xz' libssh_0.9.6-2.debian.tar.xz 27452 SHA512:159b4509a4d3007e78296b1b84e43938d1a792c4737e836f496b61162eadb9fbfe6f4dbbf5a6703e2b4417fd148ba0445ec6875f3e5a64f844dec62b14d9e40e
```

### `dpkg` source package: `libtasn1-6=4.18.0-4`

Binary Packages:

- `libtasn1-6:amd64=4.18.0-4`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.18.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0-4.dsc' libtasn1-6_4.18.0-4.dsc 2662 SHA512:f466fdc94362f4f95d2f7c9f0205aa78fb97a64df3df8df3faf3dc563d0fd8802c83535fdd05e0b8f0bfefa2b8e5577b287d6f240a59074787794a50f1ef5cd2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0.orig.tar.gz' libtasn1-6_4.18.0.orig.tar.gz 1724441 SHA512:4f2f4afc7561fda7a1f1c6c525c3c3b08228a1a4aa8c3d3d5e02e993d8f83ccee1dd0f1b201cec0fbfc97043d4b1d7a95ffd34d65422a38b85b931ac7a015831
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0.orig.tar.gz.asc' libtasn1-6_4.18.0.orig.tar.gz.asc 228 SHA512:8ef3918a3130f695d2d5b26dd945084b931005eff8914c50a0ac9795d4cc6ec9e9645e2941ff4235cba3b4b2987ab1c7da65225e24ce16aaab844352ecdafbf6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.18.0-4.debian.tar.xz' libtasn1-6_4.18.0-4.debian.tar.xz 22020 SHA512:f365dc9391e5bdb76fac97cc0b61236a174c33271f86f79d6549b81dcbd151998dbd559963cae706d199b447348a8017b07b32cfce37bfda49e114915bc4565c
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libunistring/0.9.10-6/


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

### `dpkg` source package: `libzstd=1.4.8+dfsg-3`

Binary Packages:

- `libzstd1:amd64=1.4.8+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.8+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-3.dsc' libzstd_1.4.8+dfsg-3.dsc 2291 SHA512:54e17fdc2882d49265739bb844f21e7e07e50873d0aba149ba6e6d11f15dd03040c63652f57164bd00e21cec9922f14074f48628cf158f30a667a63c3004b117
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA512:07fabe431367eea4badae7b1e46ac73e0b33aad5b67361bc7b67d5f9aef249c51db5b560f1cf59233255cc49db341a8d8440fed87745026fca7a7c5c14448cd8
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-3.debian.tar.xz' libzstd_1.4.8+dfsg-3.debian.tar.xz 12184 SHA512:b006d4c1ef6c687331dfb4d585227262a51f6578a4faa2cea9224fdfbdfcc61dd0f1e4fdbf453617ebb2c3dc68ec09bfebf27e3631b6fd0aa20e87c44bffbaef
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

### `dpkg` source package: `lz4=1.9.3-2build1`

Binary Packages:

- `liblz4-1:amd64=1.9.3-2build1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.3-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-2build1.dsc' lz4_1.9.3-2build1.dsc 2008 SHA512:1d5c1b290972d2289d1685e116a20d3a0ff94733408d092ca43bee3b229515fb9021ef681abd75a7ebc174b432f88f3115dfbd434b345fc37b18d15ca3690024
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3.orig.tar.gz' lz4_1.9.3.orig.tar.gz 320958 SHA512:c246b0bda881ee9399fa1be490fa39f43b291bb1d9db72dba8a85db1a50aad416a97e9b300eee3d2a4203c2bd88bda2762e81bc229c3aa409ad217eb306a454c
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.3-2build1.debian.tar.xz' lz4_1.9.3-2build1.debian.tar.xz 13984 SHA512:0a4e6b457206e0963d4d88b08fc439e545c4df6fbc90f1b84518518b30a5b3d4555a2486a03e02772ed1abd68415e3b61f5e982da2177c7687c8c64745c6965f
```

### `dpkg` source package: `mawk=1.3.4.20200120-3`

Binary Packages:

- `mawk=1.3.4.20200120-3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-3.dsc' mawk_1.3.4.20200120-3.dsc 1915 SHA512:f51dae1f342769e4fc0b8d5faf4e988433a0e74912ba0777fbafdf058900c973087c267756f5c2b74298bfc31a36c8bbc99c6c0edcc850710b646d0d24fa1305
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA512:14d9a6642ce931bf6457d248fc2d6da4f0ea7541976ca282ea708b26df048f86fdf92c27f72d497501ccd43a244d1d1a606f1a2f266a7558306fea35dcc3041b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-3.debian.tar.xz' mawk_1.3.4.20200120-3.debian.tar.xz 7520 SHA512:bc4f5401de313108595ba91b17f44b5c67d7650b5557eef8a6c63c75e2ccee5dfd8900576d7e81f0ab1ac2e570f64fa75f38f56f6d4535437c803029216501af
```

### `dpkg` source package: `media-types=4.0.0`

Binary Packages:

- `media-types=4.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/media-types/4.0.0/


### `dpkg` source package: `mercurial=6.0.1-1`

Binary Packages:

- `mercurial=6.0.1-1`
- `mercurial-common=6.0.1-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=6.0.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.0.1-1.dsc' mercurial_6.0.1-1.dsc 2764 SHA512:7026790dd8d3f2ad0d1b6e400eb02169f45475300e73a2f81fef0bb0183d18fdd95575380572de0c932b5feb39d25d3ea477c6c06e21946dc9e143f91b7b60c5
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.0.1.orig.tar.gz' mercurial_6.0.1.orig.tar.gz 8072365 SHA512:dae18c38e7df001177867ed9cb1c9cea6f25fff6c23fd307c56c89bba0e4641d6cf993aabefe1fcb6ab99bd32732b858411f722bea839690fbc04c0a91c1dc53
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.0.1.orig.tar.gz.asc' mercurial_6.0.1.orig.tar.gz.asc 659 SHA512:8fb5e66e3f1593cd8324a7213b00803f50c9fc4d48a028a614b1a37fbe5d5295a8cc48a2c75cabc70101ea410a61cc4354b50b56db99ba2315e06ddddde513eb
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_6.0.1-1.debian.tar.xz' mercurial_6.0.1-1.debian.tar.xz 68640 SHA512:5d768f4552b29d842dff58713a223042d6a2d16b5c1755c4ff5f6d143c8361aa19afbf96b324deecd1d6c292d0cd03b50a5654ce149b4fc007db9dd47be38511
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

### `dpkg` source package: `ncurses=6.3-2`

Binary Packages:

- `libncurses6:amd64=6.3-2`
- `libncursesw6:amd64=6.3-2`
- `libtinfo6:amd64=6.3-2`
- `ncurses-base=6.3-2`
- `ncurses-bin=6.3-2`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.3-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3-2.dsc' ncurses_6.3-2.dsc 4136 SHA512:fdf52a68c36a4d00d3020ff8cb04a37cc6220a4bede4dc46ae63e30e53700e77765a20565c067d549c96cae18b1ed8afbae7c9a9212c1ff8e300bf9727b9647a
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3.orig.tar.gz' ncurses_6.3.orig.tar.gz 3583550 SHA512:5373f228cba6b7869210384a607a2d7faecfcbfef6dbfcd7c513f4e84fbd8bcad53ac7db2e7e84b95582248c1039dcfc7c4db205a618f7da22a166db482f0105
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3.orig.tar.gz.asc' ncurses_6.3.orig.tar.gz.asc 729 SHA512:5673088e7d6af580e8f1e163687146adb51261cd3c75be9ea61368c7590efc0e5e4bc1c2ae76d717f289ff6609089c5ca1f7e4a572266d7b6c5daba98eabed2e
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.3-2.debian.tar.xz' ncurses_6.3-2.debian.tar.xz 54136 SHA512:5925e71d65dabca8e629fbef96e8d42bff449213aafd4a549ceccddff1332f8ebd4d86f3be5524624c56649f46296d6500dae95926ad41742d45196f0074a248
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

### `dpkg` source package: `nettle=3.7.3-1build1`

Binary Packages:

- `libhogweed6:amd64=3.7.3-1build1`
- `libnettle8:amd64=3.7.3-1build1`

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
$ apt-get source -qq --print-uris nettle=3.7.3-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3-1build1.dsc' nettle_3.7.3-1build1.dsc 2082 SHA512:c9340c9ac3e91901cfa9d713dd3603408b695cf57bb0b05944ba7cb70ea611e74006de93d7ffbb8e0cf6f3bb824fbde6f4dfc3d0e5a47e7be14324b56fe1f8cd
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3.orig.tar.gz' nettle_3.7.3.orig.tar.gz 2383985 SHA512:9901eba305421adff6d551ac7f478dff3f68a339d444c776724ab0b977fe6be792b1d2950c8705acbe76bd924fd6d898a65eded546777884be3b436d0e052437
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.7.3-1build1.debian.tar.xz' nettle_3.7.3-1build1.debian.tar.xz 22024 SHA512:3d6ffff632e9c1c987b5cec4f10c273d8cb8bc4ab7f1b1bd9e05342b814e2f157a39157a340464e95330cca9cd2cc445ca75f35f17d78dbc1d4e367ee68358a1
```

### `dpkg` source package: `nghttp2=1.43.0-1build2`

Binary Packages:

- `libnghttp2-14:amd64=1.43.0-1build2`

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
$ apt-get source -qq --print-uris nghttp2=1.43.0-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.43.0-1build2.dsc' nghttp2_1.43.0-1build2.dsc 2547 SHA512:81b2e366be95cc56c2b0b5abe92f51717384a338ce234ca8960d8c9c2593d82161aa07ec046c21caf3d9e8607eb5ee8e61a28200df1b84245eb041ef812b327e
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.43.0.orig.tar.bz2' nghttp2_1.43.0.orig.tar.bz2 4521786 SHA512:f2e6665ad6c73f0a1a8c7b34ca821a905868d41dafca913e6a054eb5afb534a85ae91618c1a4b098e43f350ca3703fd1ece7848f0a771e8393a3eb0581ceaf59
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.43.0-1build2.debian.tar.xz' nghttp2_1.43.0-1build2.debian.tar.xz 16448 SHA512:55273d0a5373c13ca9e6fa25aeb83d44f4d25188473da875a1a81c3311a185560a95646285a5035633c931431307c46938d0d337b69f0c39d54d00a008066696
```

### `dpkg` source package: `npth=1.6-3build1`

Binary Packages:

- `libnpth0:amd64=1.6-3build1`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-3build1.dsc' npth_1.6-3build1.dsc 1980 SHA512:2662b84476f30f68c54c9698012bbc6e25d0aef067c587e1d214126f7abc7f5e9216d2eca9d06054bb7247e28ee256b78548032359b03d0bf65a3d756e2fb0ab
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA512:2ed1012e14a9d10665420b9a23628be7e206fd9348111ec751349b93557ee69f1176bcf7e6b195b35b1c44a5e0e81ee33b713f03d79a33d1ecd9037035afeda2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-3build1.debian.tar.xz' npth_1.6-3build1.debian.tar.xz 10812 SHA512:211d39db8ef6dd954578a6d3e9708092b92e7bb069010f8d9d85298cc26c14f0119774961571f926e36daacba66db50499bec6e1dfd52abf841608173d507f16
```

### `dpkg` source package: `openldap=2.5.11+dfsg-1~exp1ubuntu1`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.11+dfsg-1~exp1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.11+dfsg-1~exp1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11+dfsg-1~exp1ubuntu1.dsc' openldap_2.5.11+dfsg-1~exp1ubuntu1.dsc 3298 SHA512:a807966ceeb7c66227e12c546c8d34929049e1c2126cd96e317dbc7a7e0f5288b414f759c3b8ac2076d5d23afc2a29bbd916d412f9510f2a286132513a30e19f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11+dfsg.orig.tar.gz' openldap_2.5.11+dfsg.orig.tar.gz 5609424 SHA512:a728d66c8a6bfa34d8e80eab86c2612685cab1358008cc10f9d9862a03aff46a5a19cd6487732131222efae6b86c27d5446fd829e89a4cadeb79161fd9ed437c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11+dfsg-1~exp1ubuntu1.debian.tar.xz' openldap_2.5.11+dfsg-1~exp1ubuntu1.debian.tar.xz 170868 SHA512:d6dddb9d150085d8f7d8609253fa6dcda3e1cb4603d9c9d58ff08f6809ca8bdee48342042f35d5720aa46b52b078c6b29f4b834ec3e058fc1308d77bae0dddaa
```

### `dpkg` source package: `openssh=1:8.7p1-4`

Binary Packages:

- `openssh-client=1:8.7p1-4`

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
$ apt-get source -qq --print-uris openssh=1:8.7p1-4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.7p1-4.dsc' openssh_8.7p1-4.dsc 3347 SHA512:d70c26b64c13d5963eaeeca524f5973f61224ac8ad506bd5b0a04f194e22445d49c5f8e9c89330f95af3ff4193bef92e3e5d248d43a2ae9e582058379706d87c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.7p1.orig.tar.gz' openssh_8.7p1.orig.tar.gz 1814595 SHA512:08c81024d9e1248abfda6cc874886ff5ae916669b93cd6aff640e0614ee8cbcbc3fe87a9ce47136b6443ddbb1168b114367c74e117551905994e1a7e3fa2c0c2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.7p1.orig.tar.gz.asc' openssh_8.7p1.orig.tar.gz.asc 833 SHA512:08b4bda855ca3ef202c271f1c0e3486082b93d1009a794d020e7ba223978bc87bf34b1fbccaae3379a47639bd849935fdaaf63bdb781d0a44625066ccf00fbfc
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.7p1-4.debian.tar.xz' openssh_8.7p1-4.debian.tar.xz 185728 SHA512:a27f5e7c674986940375ed5b6b75f82d28ff3463a771c226261a6c20cf1d9929514c3811410e42582b191b50f961468e721043337c5bfcbc256f9a250365b02d
```

### `dpkg` source package: `openssl=3.0.1-0ubuntu1`

Binary Packages:

- `libssl3:amd64=3.0.1-0ubuntu1`
- `openssl=3.0.1-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.1-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.1-0ubuntu1.dsc' openssl_3.0.1-0ubuntu1.dsc 2075 SHA512:737113c7f9650fa11852328a4353d23509fb267780bbf544cde3186c1bfc9f9ecc619ac92e76311baff1c333933b0b83b05df0bcaa29811d498efef514e5af2c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.1.orig.tar.gz' openssl_3.0.1.orig.tar.gz 15011207 SHA512:4eb29386a6c2c47bebc668e68b61872eed1d136e5620d6f8971393ae7dd8d0f640257278735c76adc0c9569a315fdb929c175a2931d52d3fcc4c527ad6a975ce
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.1.orig.tar.gz.asc' openssl_3.0.1.orig.tar.gz.asc 488 SHA512:085e8734b74e58a7c345cf2170fd476e38fe0a3b6eb1a1c417bd1dab962f96a6e2256c409aa4c650bbb57228aacdc75b8a13b693ebea571932de528d7ce622d6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_3.0.1-0ubuntu1.debian.tar.xz' openssl_3.0.1-0ubuntu1.debian.tar.xz 97800 SHA512:a2ccfdbfb9a96b107af84d037be7e3374b4774be07674d7421d2f7c7c6dddbc47a6d59c65429580fce0072e0ccbe2fb8cc887e9584456aa2659f005b2b87cb3a
```

### `dpkg` source package: `p11-kit=0.24.0-6`

Binary Packages:

- `libp11-kit0:amd64=0.24.0-6`

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
$ apt-get source -qq --print-uris p11-kit=0.24.0-6
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.0-6.dsc' p11-kit_0.24.0-6.dsc 2501 SHA512:01b4e07faeda430197ae67f5eab2d52580657bf5219bd350b97a0b044014c8466977a04996a0b514629cd45deae613f35b363592be03ce31a7d2c54e871575af
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.0.orig.tar.xz' p11-kit_0.24.0.orig.tar.xz 834392 SHA512:48369d6fdae79b8c5a255c821fbdb982f0c649cce07c0d92f0ff0c16322fea8919faa94067cae2efede2da3646c0e69a71a3e399b769dc2327f247bcb113eb3c
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.0.orig.tar.xz.asc' p11-kit_0.24.0.orig.tar.xz.asc 833 SHA512:f802c6f42f437d466b008d0c62aedc2f466bcf5bec93a5fbeec183057d22eacd28184198f624972d9df684a663820e77ebdc8d8c0d14533707691b9d69cb9f69
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.24.0-6.debian.tar.xz' p11-kit_0.24.0-6.debian.tar.xz 23176 SHA512:a96c380b1f860f4aa4e32105cf4538ef28d8754faab323c2f30127935bc5f60beca7333144f0da8aef48129274d6faf6659276b09596e7bd5cd65fd571d4a518
```

### `dpkg` source package: `pam=1.4.0-10ubuntu2`

Binary Packages:

- `libpam-modules:amd64=1.4.0-10ubuntu2`
- `libpam-modules-bin=1.4.0-10ubuntu2`
- `libpam-runtime=1.4.0-10ubuntu2`
- `libpam0g:amd64=1.4.0-10ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.4.0-10ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0-10ubuntu2.dsc' pam_1.4.0-10ubuntu2.dsc 2757 SHA512:8da17d75a47d4de2207cbf054dc5508a1e39f5de7a2e362d435221ebddfb2deb44785c520b72cfb6cc59f4b9a913b7ed377f51ba6f3a357f41c87b40df5d6a23
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0.orig.tar.xz' pam_1.4.0.orig.tar.xz 988908 SHA512:26eda95c45598a500bc142da4d1abf93d03b3bbb0f2390fa87c72dcbffa208dbfa115c0b411095c31ee9955e36422ccf3e2df3bd486818fafffef8c4310798c4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0-10ubuntu2.debian.tar.xz' pam_1.4.0-10ubuntu2.debian.tar.xz 167324 SHA512:0325d0d2be2f1864260393183d19687a7c6b6aeb7956746c17a2051cb027b1074a2a9a9aed0d78cea38ca86251b01b42f3ee3a3f5966ed1e1bb72b1738c1fd9a
```

### `dpkg` source package: `pcre2=10.39-3`

Binary Packages:

- `libpcre2-8-0:amd64=10.39-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.39-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.39-3.dsc' pcre2_10.39-3.dsc 2286 SHA512:dc3cbbb1181979d32ab7fdcb552b181590e39a653470bd2b9dce83a69ebfe395c16d1e26a38900e38b0d61a6693cf873ec1265be5516e2f36fb5a3bd502087df
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.39.orig.tar.gz' pcre2_10.39.orig.tar.gz 2309964 SHA512:fe17ea0191a91d4e4fe88a44a07883db594941376a6e38556e03ff3b594820596fd3e43be2d73b700ca68cd0c44e38c33cc891a57b8ed65e34cd832196bc09b2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.39-3.diff.gz' pcre2_10.39-3.diff.gz 7080 SHA512:f678dd627eea121de1648b64f01b8d2c2c0325430f5765bd818d4813740a513beb591abb71bc979182d9a4245deb72c51e592d1885f2e60d2fca92295a933980
```

### `dpkg` source package: `pcre3=2:8.39-13build4`

Binary Packages:

- `libpcre3:amd64=2:8.39-13build4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-13build4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13build4.dsc' pcre3_8.39-13build4.dsc 2133 SHA512:dcd2f6a80e0e5883cad926ac23b6dd33c12f0cca0308e8cb6572eb1da8f649f1853ef105d8268f6ef37b77a4673eba17e03137d09b654b1a4a862448e12c4e29
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA512:8b0f14ae5947c4b2d74876a795b04e532fd71c2479a64dbe0ed817e7c7894ea3cae533413de8c17322d305cb7f4e275d72b43e4e828eaca77dc4bcaf04529cf6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13build4.debian.tar.gz' pcre3_8.39-13build4.debian.tar.gz 26971 SHA512:e7b20615c11217f200ddb4ee68b247f1959bb4d008f8755b747da9db9085856bb52c629f2889391c0c911d0fa708cfe573c9f3cae4871de2588a3ea0fd68daae
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

### `dpkg` source package: `pinentry=1.1.1-1build1`

Binary Packages:

- `pinentry-curses=1.1.1-1build1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.1-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1-1build1.dsc' pinentry_1.1.1-1build1.dsc 2870 SHA512:c6bf5c0088b02cd2f247a9060d6a7d54608a8f84fa49284c9cef8b40b33c3de21d79d03e4d5715fb9ff0b9378b41162669bae1306ff809d7681051a800e48edc
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1.orig.tar.bz2' pinentry_1.1.1.orig.tar.bz2 515723 SHA512:d6ab5af8ac2f3c9c05e09703e95d8e2676f9b2b7ceb97f6a31d101d0e9da7a1e106a6d3eabe86cab1bb35a4b119a7cba1380ac64bf13c61af0b3c48803116c12
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1.orig.tar.bz2.asc' pinentry_1.1.1.orig.tar.bz2.asc 390 SHA512:2b696e5a59219c6fca719d5f948d508279c483d1d2b2c99221522648fe3098da4a195aca2527fbb5b777fa2905dbda642edb5f6ac4038ed9720a5291ce282cff
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.1-1build1.debian.tar.xz' pinentry_1.1.1-1build1.debian.tar.xz 19952 SHA512:6cb361fd91e7176e78e19fa9214e1ccb3bfc867b102f128e44a7c2579283da7b370822c4504b885e800947658062d54c755a49a5cabd7d00f17c84c0233c3ac1
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

### `dpkg` source package: `python3-defaults=3.9.7-4`

Binary Packages:

- `libpython3-stdlib:amd64=3.9.7-4`
- `python3=3.9.7-4`
- `python3-minimal=3.9.7-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.9.7-4
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.7-4.dsc' python3-defaults_3.9.7-4.dsc 2879 SHA512:f829f2fab4fdf387f38c8d93c62e0e8171c2fdb66ba11590084d8fcc4c1a725a297b58e20d9fcafb594be200c0ab230c440b8ac0101b52aaaeaf6d8ba9ab3726
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.7-4.tar.gz' python3-defaults_3.9.7-4.tar.gz 141201 SHA512:1fc07424053d519fdd3a72ee25a17307a38a929dddb5c37be2636eec1b872a43c517e91c07d7f774c3af51b5155358d5d291626510b47ac9d027255d43bc82e3
```

### `dpkg` source package: `python3.9=3.9.10-1`

Binary Packages:

- `libpython3.9-minimal:amd64=3.9.10-1`
- `libpython3.9-stdlib:amd64=3.9.10-1`
- `python3.9=3.9.10-1`
- `python3.9-minimal=3.9.10-1`

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
$ apt-get source -qq --print-uris python3.9=3.9.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.10-1.dsc' python3.9_3.9.10-1.dsc 3500 SHA512:790fdc0b2ce6320d7ac5d189c626e5218c911b67f072170c19db44316ea64a78fbea157be41612a1c31805839553726a18b4e4859320e656c9bc6e28f1d87563
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.10.orig.tar.xz' python3.9_3.9.10.orig.tar.xz 19154136 SHA512:09cb942f84bf362df88999ffa6faf89b4ad12302e67cda4a11547828ebe410c7c93a3dc96cd66fd9c5c7d9a1abe5b8e259e7ec47c10273b42d212270aca5ecba
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.10-1.debian.tar.xz' python3.9_3.9.10-1.debian.tar.xz 212476 SHA512:2bf55ac841c308ba8a62746f8daa8835642d82315d8cd71291b9426d1cf371c7e5aa259d477537ed6009c616b6aaeb05feddd7dc6f458fa7c7d256cc18938f9b
```

### `dpkg` source package: `readline=8.1.2-1`

Binary Packages:

- `libreadline8:amd64=8.1.2-1`
- `readline-common=8.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.dsc' readline_8.1.2-1.dsc 2432 SHA512:3166229d2ac183a46455c7d8cf17ef1d509ca8651ffa7887f654d87bbe1d00a08f9a9f73f14e652ac067d89e5d1128998f8f09f6a1128c56049338ace65ed773
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2.orig.tar.gz' readline_8.1.2.orig.tar.gz 2993073 SHA512:b512275c8aa8b3b3178366c6d681f867676fc1c881e375134a88e9c860a448535e04ca43df727817fd0048261e48203e88bd1c086e86572022d1d65fb0350e4d
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.debian.tar.xz' readline_8.1.2-1.debian.tar.xz 29292 SHA512:a64621c93975bc42ba171c9298c932f9515025513911e744183092e0ef9873db474c4ec27a21f310f40e7b970ba6300edb057552f7e90fc469897ffa2eb706f0
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
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build3.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build3.dsc 2427 SHA512:d88c3302e6f5fcaece5673963c9d0b1f9295c7240d1d227444de9108a87a0ac4f90b1cd6af790b6497ee82457db9502f02299ab8585dfcaf1c9196065b412cd6
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA512:bdfcbab73179d614a295a7b136ea4c9d0ce4620883b493f298362784d245608cd6ad4b0ad30f94ed73a086b4555399521ae9e95b6375fce75e455ae68c055e7b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build3.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build3.debian.tar.xz 8324 SHA512:96c84a3c9d660a87e063e1140b51422250844fa959a00be7a9142a3fbed033f46845d9ba05cb8f083194d7cef9d6b6f49cfa9d05c2ef99c9561c802e92c15149
```

### `dpkg` source package: `sed=4.8-1ubuntu1`

Binary Packages:

- `sed=4.8-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.8-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8-1ubuntu1.dsc' sed_4.8-1ubuntu1.dsc 2188 SHA512:0a5a384e638c1a0da05bef6c90451a523832d9ad5384b4863eff7a6d614a29a15e7800df7a40701b38a64c15284e7376caf5e744879862ba3fdc7b8033a90404
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8.orig.tar.xz' sed_4.8.orig.tar.xz 1348048 SHA512:7de25d9bc2981c63321c2223f3fbcab61d7b0df4fcf7d4394b72400b91993e1288d8bf53948ed5fffcf5a98c75265726a68ad4fb98e1d571bf768603a108c1c8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8.orig.tar.xz.asc' sed_4.8.orig.tar.xz.asc 833 SHA512:9b886bdbd18ee2d60608cee3fd2b4193a1b6c3309d887ee05828c14b89b7b515dbf042a9e0ebdd13e6ccfa42e3cd217a408c796d68c4ebedaaa64f795000f095
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.8-1ubuntu1.debian.tar.xz' sed_4.8-1ubuntu1.debian.tar.xz 60832 SHA512:abf0939b0a0af8e67f17ac2c28c5dc76b616c64ed98f7fe839836cab3bcd273b40ccb647a5b734e27f058d07c60b5caeafee8e84e9b6087950253a7bae104ba4
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

### `dpkg` source package: `serf=1.3.9-10ubuntu1`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `shadow=1:4.8.1-2ubuntu1`

Binary Packages:

- `login=1:4.8.1-2ubuntu1`
- `passwd=1:4.8.1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-2ubuntu1.dsc' shadow_4.8.1-2ubuntu1.dsc 2381 SHA512:04251885e4b9f51c78d133aeddbcb5097e7e9a5844c842f621cb35b49f6cc5db7dad11b3967663dd34311ae8a3f6b28136d5e6dfe95b8ef4d51e8d40d4819310
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA512:780a983483d847ed3c91c82064a0fa902b6f4185225978241bc3bc03fcc3aa143975b46aee43151c6ba43efcfdb1819516b76ba7ad3d1d3c34fcc38ea42e917b
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-2ubuntu1.debian.tar.xz' shadow_4.8.1-2ubuntu1.debian.tar.xz 86604 SHA512:d0531d7faa0bb494f01b93fd7293c207b091392006300364a523f45eeed6868d891adf89d984873cbe0c9f5d8278a41d8e583bf4a1015504f6e7c2d56e4c2656
```

### `dpkg` source package: `sqlite3=3.37.2-2`

Binary Packages:

- `libsqlite3-0:amd64=3.37.2-2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.37.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.37.2-2.dsc' sqlite3_3.37.2-2.dsc 2487 SHA512:d542b60afedb0556cc0c56622934bbd5d6ac456c00bca4ba38ef47245c7b798b871382c2b48b9a9b8a3aa12133b0d19bcc3a81aeebfb3619dca139493586b61f
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.37.2.orig-www.tar.xz' sqlite3_3.37.2.orig-www.tar.xz 5694016 SHA512:577e34b4ae18a3c73be6d955a2e2321e993f61decefbcca5112170072ea556eca93dcf55f3059fbcd96147124442b368150de7f68c603e84b80cbe0228ae78f8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.37.2.orig.tar.xz' sqlite3_3.37.2.orig.tar.xz 7623768 SHA512:dfa51b0a32ab0597cd00ae7abdb53bb255102f397ff8409f3fdbefaad17bc7d5a25f53db90bed47feb1bf4a9a1a4707bc40440c6c5303f3ef5c49ded61558fed
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.37.2-2.debian.tar.xz' sqlite3_3.37.2-2.debian.tar.xz 28536 SHA512:244fccac20d6c63c4897c04bf490603b0ee54d522aa2040d5ff5e41cc4665c8a32ac95e67fbc9961978b67dcbc64f84999b1502fb1696e138a1944aff113cd2f
```

### `dpkg` source package: `subversion=1.14.1-3build2`

Binary Packages:

- `libsvn1:amd64=1.14.1-3build2`
- `subversion=1.14.1-3build2`

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
$ apt-get source -qq --print-uris subversion=1.14.1-3build2
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1-3build2.dsc' subversion_1.14.1-3build2.dsc 3584 SHA512:e5771cdd29b48b2f63303ebfd1fedf9be94230c1892a7b8bc600fbd61cfe5283d1733a22966b9766241e271663cecf3d037cd117ab258265590a6db46418c398
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1.orig.tar.gz' subversion_1.14.1.orig.tar.gz 11534165 SHA512:6cd780f6669c811264de03b94ea41487111957dfd817498699c91e5dbb975e4b9626de9c436c5722fd6a6fadc4fef35f51905c2c0f5fd4955cf0fadef9cba60e
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1.orig.tar.gz.asc' subversion_1.14.1.orig.tar.gz.asc 1288 SHA512:56f3b3ae63e10c503b741107261da955088749845693b34125f8e61c7850035021684b31944e99ed50628cc4f601081627c1472f83f8196eac3a289038a842f9
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.1-3build2.debian.tar.xz' subversion_1.14.1-3build2.debian.tar.xz 430216 SHA512:4acf01cae3afd109b7c83e475c704e0ebc053c60e1fb236b3b2697a4d388d3cca31d3e1757ca03aaa7650921fdf254e17a943c751cd86eb6713d3ad5aafee3f3
```

### `dpkg` source package: `systemd=249.9-0ubuntu2`

Binary Packages:

- `libsystemd0:amd64=249.9-0ubuntu2`
- `libudev1:amd64=249.9-0ubuntu2`

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
$ apt-get source -qq --print-uris systemd=249.9-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_249.9-0ubuntu2.dsc' systemd_249.9-0ubuntu2.dsc 5674 SHA512:b4131429b45a00aaa3d1eb85e873f80c6369767592e35bd958d5d6b8c76ac705311b9b6c9bf939e639befe9eb4a9db6082080e94896876c48482c9ba45c71103
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_249.9.orig.tar.gz' systemd_249.9.orig.tar.gz 10613893 SHA512:ce57bc6c522082e55649fc1886c4dc818c89607e175df2c92feffe288dbd38757f36b30abeebe153f5be6b664a49d729405040a952473cb2133a2e39cf9cc164
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_249.9-0ubuntu2.debian.tar.xz' systemd_249.9-0ubuntu2.debian.tar.xz 224268 SHA512:188bb45d4ab49c2f3ada94eb82c76ac302228bfab4985b78d89ea0255cae0761bd5daffc708279f8654d7a0e7537bc8b090c59590f740745a8c80b5f485de874
```

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

### `dpkg` source package: `tar=1.34+dfsg-1build2`

Binary Packages:

- `tar=1.34+dfsg-1build2`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34+dfsg-1build2.dsc' tar_1.34+dfsg-1build2.dsc 2118 SHA512:14708ca603715baa504d88249195d0459f50003d8a26e7c8eddc4c700cd97712e3de1bb17fc0e1cbbf012de4f995825c5c87d7a013465ce30265b928a00a7320
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34+dfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA512:ec5553c53c4a5f523f872a8095f699c17bf41400fbe2f0f8b45291ccbaf9ac51dea8445c81bd95697f8853c95dcad3250071d23dbbcab857a428ee92e647bde9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34+dfsg-1build2.debian.tar.xz' tar_1.34+dfsg-1build2.debian.tar.xz 19356 SHA512:e96be222eb54237203ab689f981e97c3c83dd0b9851ce70b9194527928eb7a2efa011e82521bd4ad9c326c8d04caa3d0efda065fd35281ae3351d804ecad7c17
```

### `dpkg` source package: `tzdata=2021e-1ubuntu1`

Binary Packages:

- `tzdata=2021e-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2021e-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021e-1ubuntu1.dsc' tzdata_2021e-1ubuntu1.dsc 2326 SHA512:b7e1560c5fd93e4bc6971009d19f0ccee1713bcf4387bdd46a6015e2edf7e4c6adf498b6b5ff0c509294b7e4ec7efe96e90c9f85f5d28d42f27f53e163bc0467
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021e.orig.tar.gz' tzdata_2021e.orig.tar.gz 422509 SHA512:c1e8d04e049157ed5d4af0868855bbd75517e3d7e1db9c41d5283ff260109de46b6fac6be94828201d093e163d868044ac2a9db2bf0aeab800e264d0c73a9119
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021e.orig.tar.gz.asc' tzdata_2021e.orig.tar.gz.asc 833 SHA512:b0bd68939fbf4cdf4078b8e97d0cd642e8112966e874a18218469ca35ff82c29410347a99e1321d6c9d723547ebc7945173418966e80d14b10f60af8ea7bff52
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2021e-1ubuntu1.debian.tar.xz' tzdata_2021e-1ubuntu1.debian.tar.xz 172984 SHA512:1213d6763668582933ca021d2a881b4a1e0496e8591563f30a276916d2ee0bf805795b7aa7aa24584badd65ddabac84d3a498be6647ef3b17730fb4bdfcd5ac8
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

### `dpkg` source package: `util-linux=2.37.2-4ubuntu1`

Binary Packages:

- `bsdutils=1:2.37.2-4ubuntu1`
- `libblkid1:amd64=2.37.2-4ubuntu1`
- `libmount1:amd64=2.37.2-4ubuntu1`
- `libsmartcols1:amd64=2.37.2-4ubuntu1`
- `libuuid1:amd64=2.37.2-4ubuntu1`
- `mount=2.37.2-4ubuntu1`
- `util-linux=2.37.2-4ubuntu1`

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
$ apt-get source -qq --print-uris util-linux=2.37.2-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2-4ubuntu1.dsc' util-linux_2.37.2-4ubuntu1.dsc 4567 SHA512:2245ab47b726712f741ac209c8c1eaed6ba2496070c618abba228b680fe20799de436aa6d54907e669c356a4eceb839d1623a0e3ab904ca8069c10f359fb366e
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2.orig.tar.xz' util-linux_2.37.2.orig.tar.xz 5621624 SHA512:38f0fe820445e3bfa79550e6581c230f98c7661566ccc4daa51c7208a5f972c61b4e57dfc86bed074fdbc7c40bc79f856be8f6a05a8860c1c0cecc4208e8b81d
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2-4ubuntu1.debian.tar.xz' util-linux_2.37.2-4ubuntu1.debian.tar.xz 102856 SHA512:a8d4de10770d8f529ccfb38626e6fdaeb8619881ecffa4bbe109d118b992471f4246189474152c411de60a5e2914800ab5f545ea45c317ae539009f74257a670
```

### `dpkg` source package: `wget=1.21.2-2ubuntu1`

Binary Packages:

- `wget=1.21.2-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21.2-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.2-2ubuntu1.dsc' wget_1.21.2-2ubuntu1.dsc 2243 SHA512:01295325ac2239ad7eebd86e395b6310bc42d04ef7b7722e9320db6f0a44e806009b4bf452c1006e18eb936696c92ac4ba15b55dedebb6e030620cfd7cbb1b60
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.2.orig.tar.gz' wget_1.21.2.orig.tar.gz 5004576 SHA512:3e35f92604486ca459f26df97d392579f1d83a9254519e8ce249b410bacf70dddf716d6caa3b29fd4865163f60410b2b8ad1ca1f7bb3dbb2456386b7647b988d
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.2.orig.tar.gz.asc' wget_1.21.2.orig.tar.gz.asc 833 SHA512:c5349ed20902d4e4d76e681b9e14370d5c1f07d1ba9e600a82af67ac24fe79051b3beabbe563e6967c429cc344ee1bc46aff57c1ab0eb2db8d70e907df49c953
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.2-2ubuntu1.debian.tar.xz' wget_1.21.2-2ubuntu1.debian.tar.xz 64160 SHA512:2e99d242111afdfbfe409165702e553faed0193836d852465d5e8623d27aa2e6dd6f4c806d4f1b2e3c0f825ecd218ace3329b1e145be193a086af7a1b980528d
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

### `dpkg` source package: `xz-utils=5.2.5-2build1`

Binary Packages:

- `liblzma5:amd64=5.2.5-2build1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2build1.dsc' xz-utils_5.2.5-2build1.dsc 2535 SHA512:290381e339adda8dbe75872360a51097b6107a2715406436ecad9f03c758b53bcfec77437afa6a3306e871ee696b144c992cf988cbf162f83a1b54dbff804bc9
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA512:59266068a51cb616eb31b67cd8f07ffeb2288d1391c61665ae2ec6814465afac80fec69248f6a2f2db45b44475af001296a99af6a32287226a9c41419173ccbb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz.asc' xz-utils_5.2.5.orig.tar.xz.asc 833 SHA512:582864ae306861ede34074ebfd23ab161ad3340ab4a068f727583de2bd2058da70dfe73019f4e70b8267e0e0c62f275da1e23f47d40c0b80038449b0ac335020
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2build1.debian.tar.xz' xz-utils_5.2.5-2build1.debian.tar.xz 33600 SHA512:121bccaca745872de67d3c78fe38cd33f9f6fed9b2b32269fdc6852efcd3b153f21513e1c03f1157db19bca220ece82575c1b2e542d440c6eab01b495fc5b8af
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu7`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu7`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu7
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu7.dsc' zlib_1.2.11.dfsg-2ubuntu7.dsc 2945 SHA512:956709508bde7e163129ae35cf5cdac8752510400b0b6404ce0b96529f107836b81268a58f0693a12b51c02251d48316aec0d8e2f3edeab33c7e6f5e94508137
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA512:92819807c0b8de655021bb2d5d182f9b6b381d3072d8c8dc1df34bbaa25d36bcba140c85f754a43cc466aac65850b7a7366aa0c93e804180e5b255e61d5748de
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu7.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu7.debian.tar.xz 54844 SHA512:c3245d9d6c1325a3d176750e232ff2920264d79ec51501e3a6cc1ec2c87ed30ff5d36489dbf1ff867581a3c253ddc596c07f6575147f84726c831af54e86e834
```
