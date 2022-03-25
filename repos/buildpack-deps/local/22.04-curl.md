# `buildpack-deps:jammy-curl`

## Docker Metadata

- Image ID: `sha256:62980bdfe9568899ff86700e0c5c94890e6165de7e24bd36d4480cb24c1bb795`
- Created: `2022-03-18T06:56:01.572949514Z`
- Virtual Size: ~ 96.10 Mb  
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

### `dpkg` source package: `apt=2.4.1`

Binary Packages:

- `apt=2.4.1`
- `libapt-pkg6.0:amd64=2.4.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.4.1/


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

### `dpkg` source package: `audit=1:3.0.7-1`

Binary Packages:

- `libaudit-common=1:3.0.7-1`
- `libaudit1:amd64=1:3.0.7-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/audit/1:3.0.7-1/


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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `curl=7.81.0-1`

Binary Packages:

- `curl=7.81.0-1`
- `libcurl4:amd64=7.81.0-1`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl4/copyright`)

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

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg2-3ubuntu1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg2-3ubuntu1`
- `libsasl2-modules-db:amd64=2.1.27+dfsg2-3ubuntu1`

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
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg2-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg2-3ubuntu1.dsc' cyrus-sasl2_2.1.27+dfsg2-3ubuntu1.dsc 3517 SHA512:51d1d14563cfd73d104551d3bd24ffcf0576aa0101eb98ebc570adf6f0c9f164fa74bc0d59cab406b47555d707ec494a41bc6eb5955f4605d97360b6c1ab32b7
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg2.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg2.orig.tar.xz 829892 SHA512:13337dfcc57ea8fec471ee0f2a0f6b58fb92907ad0899a4a8afaba957c5da302924e71c9fc4a61bbc913a4ee2ea74b05772cb26ed58d5724a312bb20a8b6a4cb
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27%2bdfsg2-3ubuntu1.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg2-3ubuntu1.debian.tar.xz 93396 SHA512:55b7a94c940238954aa82c35e52be26bff9c5cdb217a2f949146a0f3b6f1d366b15e1caea957aa12f18ca3954d1416d8aabb2fbc95803a2a11c0f3aa2cc211a5
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
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-3.dsc' dash_0.5.11+git20210903+057cd650a4ed-3.dsc 1686 SHA512:896f69b46297284f7f01f3d12833cefd80b1bbb540a0388273dcb48d7db9790e1c1591ce656c048455278bdf37c2bfe3a03068885ed19089332a0ccb5763600e
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed.orig.tar.xz' dash_0.5.11+git20210903+057cd650a4ed.orig.tar.xz 133320 SHA512:eced6bc60ca6ba4394a2ee65d8c6b88eca729c43e47053fc01dec5500ebe002a12f536c128c3fd821a2eb61b97e92c8a0be6d4532926479ce4b7d986be109cb7
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.11%2bgit20210903%2b057cd650a4ed-3.debian.tar.xz' dash_0.5.11+git20210903+057cd650a4ed-3.debian.tar.xz 42656 SHA512:1668d3d85ec32e9933b8b5b71d44be0fcb772a7b6d485cac1aff09868a1099b5a01bcb6ee17685ad08268e54a92e70affd461039b1e3268bd2abb557caf45feb
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8ubuntu2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.8ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.8ubuntu2.dsc' db5.3_5.3.28+dfsg1-0.8ubuntu2.dsc 3245 SHA512:41b929ded6b945733dadc66fb4438b9ac87fc674163a5eadee584fa43df8115bde9e35c7ae0432dfe92b562ab0d69ef09688a485a514819b69223ef2fddbf019
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA512:50cb87bc3f24065839ee2932e82af032b236b290ebe89983076f503c6c62c5f36ff93d7847a3f68b2b19f35088fbab5d3ac6a34553d07e8148e68e9a3f079a12
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg1-0.8ubuntu2.debian.tar.xz' db5.3_5.3.28+dfsg1-0.8ubuntu2.debian.tar.xz 31952 SHA512:03f093df95a539fc367a657543998e9efe2dfede8fb1e4289421698cbc16b393f30f428b66001fa456b7b15b6b57e9c1dc5953328abe88ba5535c07a50bba7a6
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

### `dpkg` source package: `gcc-11=11.2.0-18ubuntu1`

Binary Packages:

- `gcc-11-base:amd64=11.2.0-18ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-11-base/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.2.0-18ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-18ubuntu1.dsc' gcc-11_11.2.0-18ubuntu1.dsc 22819 SHA512:ab4e7f87b8dba772cc809308b22f5a72157a00f8518f88826c1551c67b044d8fd9c5c70c3f61510c55e79d4ee2ced609c854b0336aeca1ff66ae70d04b1688a6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0.orig.tar.gz' gcc-11_11.2.0.orig.tar.gz 87861992 SHA512:64e4634769a62faa0adbfe99e5e590dd9efc1facac20a7dd71ab9f1d675e7df80678cbdc75c966e08ccf91dbc1e1a681d8e3227d0026ffcb5f46bdc96acaace8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-18ubuntu1.debian.tar.xz' gcc-11_11.2.0-18ubuntu1.debian.tar.xz 2067484 SHA512:d4f5d936572a4987a93862f943348eb77b954f7c8b36733753cc516937181cdd7aa1d20f25770adf89f256719b0a376c9b60c33c5a15f7a48c6b24bead5f1bec
```

### `dpkg` source package: `gcc-12=12-20220313-1ubuntu1`

Binary Packages:

- `gcc-12-base:amd64=12-20220313-1ubuntu1`
- `libgcc-s1:amd64=12-20220313-1ubuntu1`
- `libstdc++6:amd64=12-20220313-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12-20220313-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12-20220313-1ubuntu1.dsc' gcc-12_12-20220313-1ubuntu1.dsc 27778 SHA512:7a08334f4ab6d59603b3f23b74f27ffd7f284f2e64038ecb5f02aeb898f60b4535cd32f0b743dd3c3dd89d8436b137ff0b3f815e483a16a8d82aa60e2d3ca55e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12-20220313.orig.tar.gz' gcc-12_12-20220313.orig.tar.gz 97165820 SHA512:faa88f6aade8400a9a2c99f8a8a0e18bff6f1e910fc53d20b39dd52d66ebcdd9f835d54b655b5d2d31d1e6c2c028d6d248e608ab4fa5bca8de78d72841ee6447
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12-20220313-1ubuntu1.debian.tar.xz' gcc-12_12-20220313-1ubuntu1.debian.tar.xz 561904 SHA512:f6c6660dd3086d66fcd78fc21bb0e9f19fdd958ac8a11d7657863edd46401174d8d519c0d2bc2738bc35ecc456a13b6e7c436e8447ba29bd86225cbdef7b6c32
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

### `dpkg` source package: `init-system-helpers=1.62`

Binary Packages:

- `init-system-helpers=1.62`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.62
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.62.dsc' init-system-helpers_1.62.dsc 1993 SHA512:f706cf5841877ccabe6f5a8e62d44ce5b312c09776d7fb7fd841f39c2d841b3f7f19bcb63cf94073f853165ae44def8f171a0abce658d05c76a48bf1e91697eb
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.62.tar.xz' init-system-helpers_1.62.tar.xz 42144 SHA512:d90f12e642d086bd0d560ece87d119079c164b90ddbb77b2f804979540095b655715febbc2a5b0d50d7f94434d1ff7c0f4044d5d5411916fbca8300f3f88da7f
```

### `dpkg` source package: `keyutils=1.6.1-2ubuntu3`

Binary Packages:

- `libkeyutils1:amd64=1.6.1-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.1-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu3.dsc' keyutils_1.6.1-2ubuntu3.dsc 2203 SHA512:7e9c3266bf707b3553758ab89f815542edca6d7ed0ca069986bee3dda75b534f5b275b786e246232b3234c6ccbaf4c67ff60f68bba73b0a3e2ec1bbfa00b295e
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1.orig.tar.bz2' keyutils_1.6.1.orig.tar.bz2 97232 SHA512:ea6e20b2594234c7f51581eef2b8fd19c109fa9eacaaef8dfbb4f237bd1d6fdf071ec23b4ff334cb22a46461d09d17cf499987fd1f00e66f27506888876961e1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu3.debian.tar.xz' keyutils_1.6.1-2ubuntu3.debian.tar.xz 18936 SHA512:16f390f0fc3154a77c8ca3666d44881a6ca2f0d11cfe0398cd82b57b6f552af85c156de358d0b87e39f301331897d72de058050e3cb53720a76b5b5ebf07aa3d
```

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

### `dpkg` source package: `libcap-ng=0.7.9-2.2build3`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.2build3`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.2build3
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2build3.dsc' libcap-ng_0.7.9-2.2build3.dsc 2105 SHA512:50d7c66eea7dbadcd2314f3eb5ae9f4464e9a2a82a36004efd841bc092f6c4787dd9856aa14bef85035ae9db115b3a9aee78436b790a373e935d98f7fd761cd5
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA512:095edabaf76a943aab0645b843b14e20b1733ba1d47a8e34d82f6586ca9a1512ba2677d232b13dd3900b913837401bb58bf74481970e967ba19041959dc43259
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2build3.debian.tar.xz' libcap-ng_0.7.9-2.2build3.debian.tar.xz 6432 SHA512:9ce3f52dc0c89739f0117ba7c1b8fdfcdb51ceb7cea7c00aa55522ba733efdb7a37a7f21a9bfd106e453a8477a759af0aaf4688e4b18c3c9cc659657aeb2c0bb
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

### `dpkg` source package: `libseccomp=2.5.3-2ubuntu1`

Binary Packages:

- `libseccomp2:amd64=2.5.3-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libselinux=3.3-1build1`

Binary Packages:

- `libselinux1:amd64=3.3-1build1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.3-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.3-1build1.dsc' libselinux_3.3-1build1.dsc 2673 SHA512:fc40ad2eb1ec90980550e15e43ebb44e3e2343b1d5fde714e091fd2deebd7b09f877becd4fd853802fc7fb6d1b8eea076bfb4f23f5e9804f4b46b9f8082416ce
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.3.orig.tar.gz' libselinux_3.3.orig.tar.gz 206826 SHA512:9a89c05ea4b17453168a985ece93ba6d6c4127916e657c46d4135eb59a1f6408faa0802cc2e49187defbde5247d659037beee089877affbab3eab6af3433696c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.3-1build1.debian.tar.xz' libselinux_3.3-1build1.debian.tar.xz 24012 SHA512:722029b9683879effa2a8783b96beadc2c6132622031c0e5330e7431d50b979e181f79f664d40a5f5cd25c5d1f35fc396e6d792d2f4b4183dca6089de8e2a7ef
```

### `dpkg` source package: `libsemanage=3.3-1build1`

Binary Packages:

- `libsemanage-common=3.3-1build1`
- `libsemanage2:amd64=3.3-1build1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-3.dsc' libzstd_1.4.8+dfsg-3.dsc 2291 SHA512:54e17fdc2882d49265739bb844f21e7e07e50873d0aba149ba6e6d11f15dd03040c63652f57164bd00e21cec9922f14074f48628cf158f30a667a63c3004b117
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA512:07fabe431367eea4badae7b1e46ac73e0b33aad5b67361bc7b67d5f9aef249c51db5b560f1cf59233255cc49db341a8d8440fed87745026fca7a7c5c14448cd8
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8%2bdfsg-3.debian.tar.xz' libzstd_1.4.8+dfsg-3.debian.tar.xz 12184 SHA512:b006d4c1ef6c687331dfb4d585227262a51f6578a4faa2cea9224fdfbdfcc61dd0f1e4fdbf453617ebb2c3dc68ec09bfebf27e3631b6fd0aa20e87c44bffbaef
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

### `dpkg` source package: `openldap=2.5.11+dfsg-1~exp1ubuntu3`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.11+dfsg-1~exp1ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.11+dfsg-1~exp1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11%2bdfsg-1%7eexp1ubuntu3.dsc' openldap_2.5.11+dfsg-1~exp1ubuntu3.dsc 3298 SHA512:728ad98af8644cb3a41e762343935acc3897191b58a5ab2f6861d46f23d98340defe434c65aa67b5f97c461f6bfadd9ff2041cc4e6f4702b882cd03fab11f482
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11%2bdfsg.orig.tar.gz' openldap_2.5.11+dfsg.orig.tar.gz 5609424 SHA512:a728d66c8a6bfa34d8e80eab86c2612685cab1358008cc10f9d9862a03aff46a5a19cd6487732131222efae6b86c27d5446fd829e89a4cadeb79161fd9ed437c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11%2bdfsg-1%7eexp1ubuntu3.debian.tar.xz' openldap_2.5.11+dfsg-1~exp1ubuntu3.debian.tar.xz 170932 SHA512:2dc8db44e01d3a1a884faa70c7c461d77319f890dd022f52861c87ec8dc007e7d772bdcac6296d9d25687aa53adcdb7f86d64dc86518227d0afefa709fe68bdf
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

### `dpkg` source package: `pam=1.4.0-11ubuntu1`

Binary Packages:

- `libpam-modules:amd64=1.4.0-11ubuntu1`
- `libpam-modules-bin=1.4.0-11ubuntu1`
- `libpam-runtime=1.4.0-11ubuntu1`
- `libpam0g:amd64=1.4.0-11ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.4.0-11ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0-11ubuntu1.dsc' pam_1.4.0-11ubuntu1.dsc 2757 SHA512:6c6dfb6fa539fc608ab06035703fb7f79328d312dbf294c41e2e6d1445fe3e6532ebbe46d70ef0ed9c2a6eecdf626398dde5dd6a3240d640650ae8e60544c4ca
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0.orig.tar.xz' pam_1.4.0.orig.tar.xz 988908 SHA512:26eda95c45598a500bc142da4d1abf93d03b3bbb0f2390fa87c72dcbffa208dbfa115c0b411095c31ee9955e36422ccf3e2df3bd486818fafffef8c4310798c4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.4.0-11ubuntu1.debian.tar.xz' pam_1.4.0-11ubuntu1.debian.tar.xz 167484 SHA512:bdfcc4f5479f1a6400968dab1347b5b630288ad718ce1b39d206924236f76c4b0ed93c49caa021122d0c718d7d3b2d637e1cedc07e81b10f175a3b11c2a18728
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

### `dpkg` source package: `perl=5.34.0-3ubuntu1`

Binary Packages:

- `perl-base=5.34.0-3ubuntu1`

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
$ apt-get source -qq --print-uris perl=5.34.0-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0-3ubuntu1.dsc' perl_5.34.0-3ubuntu1.dsc 2993 SHA512:6f65ee700ac9a4d45ff9c676d1ae6dac1d75cfd4d071e4c88cd00a0579dcdbc68f194121a610f4d8f460d5d086d118dc0ec2d1b016d56c945ce262702dec2c6c
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0.orig-regen-configure.tar.xz' perl_5.34.0.orig-regen-configure.tar.xz 415412 SHA512:2581152e0747105314c4fa4167f1f97d286436b996341b9b75e4099ba18f15eb0d2b42888622fbe9b5499d3fe304bc8aa9ad207a945f590135beccfb68ea28b0
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0.orig.tar.xz' perl_5.34.0.orig.tar.xz 12881416 SHA512:691b4b31eacec357191fba777612b4e3eae59e946a22998a50766697c0d61db1d42a9b3bc1e41abf0d1ca1893e4a7c06d7bf3290480cf03d7f79befd7a8a3267
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.34.0-3ubuntu1.debian.tar.xz' perl_5.34.0-3ubuntu1.debian.tar.xz 167356 SHA512:670be9084642fbce2ac074c684ec857a57f5ce3a87bfa20e93a4504876abb38821bc31a39deca01eda767ad4a09bd97709990e8704fe4225f9401916c151313a
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
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2build3.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build3.dsc 2427 SHA512:d88c3302e6f5fcaece5673963c9d0b1f9295c7240d1d227444de9108a87a0ac4f90b1cd6af790b6497ee82457db9502f02299ab8585dfcaf1c9196065b412cd6
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA512:bdfcbab73179d614a295a7b136ea4c9d0ce4620883b493f298362784d245608cd6ad4b0ad30f94ed73a086b4555399521ae9e95b6375fce75e455ae68c055e7b
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2build3.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build3.debian.tar.xz 8324 SHA512:96c84a3c9d660a87e063e1140b51422250844fa959a00be7a9142a3fbed033f46845d9ba05cb8f083194d7cef9d6b6f49cfa9d05c2ef99c9561c802e92c15149
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

### `dpkg` source package: `shadow=1:4.8.1-2ubuntu1`

Binary Packages:

- `login=1:4.8.1-2ubuntu1`
- `passwd=1:4.8.1-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `systemd=249.10-0ubuntu2`

Binary Packages:

- `libsystemd0:amd64=249.10-0ubuntu2`
- `libudev1:amd64=249.10-0ubuntu2`

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

### `dpkg` source package: `tar=1.34+dfsg-1build2`

Binary Packages:

- `tar=1.34+dfsg-1build2`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.34+dfsg-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1build2.dsc' tar_1.34+dfsg-1build2.dsc 2118 SHA512:14708ca603715baa504d88249195d0459f50003d8a26e7c8eddc4c700cd97712e3de1bb17fc0e1cbbf012de4f995825c5c87d7a013465ce30265b928a00a7320
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg.orig.tar.xz' tar_1.34+dfsg.orig.tar.xz 1981736 SHA512:ec5553c53c4a5f523f872a8095f699c17bf41400fbe2f0f8b45291ccbaf9ac51dea8445c81bd95697f8853c95dcad3250071d23dbbcab857a428ee92e647bde9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.34%2bdfsg-1build2.debian.tar.xz' tar_1.34+dfsg-1build2.debian.tar.xz 19356 SHA512:e96be222eb54237203ab689f981e97c3c83dd0b9851ce70b9194527928eb7a2efa011e82521bd4ad9c326c8d04caa3d0efda065fd35281ae3351d804ecad7c17
```

### `dpkg` source package: `tzdata=2021e-1ubuntu1`

Binary Packages:

- `tzdata=2021e-1ubuntu1`

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

### `dpkg` source package: `util-linux=2.37.2-4ubuntu3`

Binary Packages:

- `bsdutils=1:2.37.2-4ubuntu3`
- `libblkid1:amd64=2.37.2-4ubuntu3`
- `libmount1:amd64=2.37.2-4ubuntu3`
- `libsmartcols1:amd64=2.37.2-4ubuntu3`
- `libuuid1:amd64=2.37.2-4ubuntu3`
- `mount=2.37.2-4ubuntu3`
- `util-linux=2.37.2-4ubuntu3`

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
$ apt-get source -qq --print-uris util-linux=2.37.2-4ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2-4ubuntu3.dsc' util-linux_2.37.2-4ubuntu3.dsc 4542 SHA512:e4e9cabeb25329e66c77b24ba8b8892b2e0bbc6f00edd98859fd8186070d8ff21ee0da2d45ab8a9087e10c7a21737e0221465d8cc086d7b6e545d0fc1cb10691
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2.orig.tar.xz' util-linux_2.37.2.orig.tar.xz 5621624 SHA512:38f0fe820445e3bfa79550e6581c230f98c7661566ccc4daa51c7208a5f972c61b4e57dfc86bed074fdbc7c40bc79f856be8f6a05a8860c1c0cecc4208e8b81d
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2-4ubuntu3.debian.tar.xz' util-linux_2.37.2-4ubuntu3.debian.tar.xz 107608 SHA512:829cf9a4e12fc6ee7ac8e79c1847ac38f6d20fe7f2edd08773ed685ab95d6e92c3b87d7bf5169dab9406da3d95f0367ca519fa14ef6a6633e62dfd0625c8e888
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
