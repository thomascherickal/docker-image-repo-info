# `ros:rolling-ros-base`

## Docker Metadata

- Image ID: `sha256:a4d86fe3731f9d8e0f01689266fe6c1b9aa5cb0e41577a478a50ef371e63844b`
- Created: `2022-03-01T01:29:09.132972915Z`
- Virtual Size: ~ 811.07 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/ros_entrypoint.sh"]`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `LC_ALL=C.UTF-8`
  - `ROS_DISTRO=rolling`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.3.1-1`

Binary Packages:

- `acl=2.3.1-1`
- `libacl1:amd64=2.3.1-1`
- `libacl1-dev:amd64=2.3.1-1`

Licenses: (parsed from: `/usr/share/doc/acl/copyright`, `/usr/share/doc/libacl1/copyright`, `/usr/share/doc/libacl1-dev/copyright`)

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

### `dpkg` source package: `ann=1.1.2+doc-7build1`

Binary Packages:

- `libann0=1.1.2+doc-7build1`

Licenses: (parsed from: `/usr/share/doc/libann0/copyright`)

- `GPL-3`
- `GPL-3.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris ann=1.1.2+doc-7build1
'http://archive.ubuntu.com/ubuntu/pool/universe/a/ann/ann_1.1.2%2bdoc-7build1.dsc' ann_1.1.2+doc-7build1.dsc 2164 SHA512:e2613d5270ab40f9139f2cfb912c466a485237ad645c0cb7075429886a351a53cc1e4c6dbdddd5ccc8397240fff17d28885675564010d7a4da0e5a9f2e0d8096
'http://archive.ubuntu.com/ubuntu/pool/universe/a/ann/ann_1.1.2%2bdoc.orig.tar.gz' ann_1.1.2+doc.orig.tar.gz 693957 SHA512:fb004a014add109d0b0949443c4c599795363d20ee65386421f898f5276b5df08714a3cd8d371d5a03417e7c3f7f3451335f90df2ca274ce95c658b958a253ae
'http://archive.ubuntu.com/ubuntu/pool/universe/a/ann/ann_1.1.2%2bdoc-7build1.debian.tar.xz' ann_1.1.2+doc-7build1.debian.tar.xz 172220 SHA512:bdea0ce4e76fe53714922c2cd33488818ad20d1f8cb5eb97c064bb9ceac10899aad2d88a0590c977cbdc698854149b715815f054efadb88b0d018be8fbe06aee
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
- `libattr1-dev:amd64=1:2.5.1-1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`, `/usr/share/doc/libattr1-dev/copyright`)

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `binutils=2.38-2ubuntu1`

Binary Packages:

- `binutils=2.38-2ubuntu1`
- `binutils-common:amd64=2.38-2ubuntu1`
- `binutils-x86-64-linux-gnu=2.38-2ubuntu1`
- `libbinutils:amd64=2.38-2ubuntu1`
- `libctf-nobfd0:amd64=2.38-2ubuntu1`
- `libctf0:amd64=2.38-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.38-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.38-2ubuntu1.dsc' binutils_2.38-2ubuntu1.dsc 8799 SHA512:fae8d03cb186c23e8db877391d2bcab8296b4e5b16b2a81351799180164a9ea45dea17df2b15f7c9b246540c81bcc097aa7fafa6b73fe16342ee65c11c8543ce
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.38.orig.tar.xz' binutils_2.38.orig.tar.xz 23651408 SHA512:8bf0b0d193c9c010e0518ee2b2e5a830898af206510992483b427477ed178396cd210235e85fd7bd99a96fc6d5eedbeccbd48317a10f752b7336ada8b2bb826d
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.38-2ubuntu1.debian.tar.xz' binutils_2.38-2ubuntu1.debian.tar.xz 212464 SHA512:29c76c2a3e4adb58e599b862e0c4ff923a97c150d8b1ab8822049536a0d821e6d51463d61b7d579e68483af8b72e0fb731c3c25c7acb0df9c7baee0392f80f31
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

### `dpkg` source package: `build-essential=12.9ubuntu2`

Binary Packages:

- `build-essential=12.9ubuntu2`

Licenses: (parsed from: `/usr/share/doc/build-essential/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris build-essential=12.9ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.9ubuntu2.dsc' build-essential_12.9ubuntu2.dsc 2415 SHA512:8121dda0738ae116c63dc65787d6fce9c07105fe1c68ff4ef255534d1bb5b146e9790eca56076768fbd57828bd87423f6d60f16901ddad3e7966a9313ee36a68
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.9ubuntu2.tar.xz' build-essential_12.9ubuntu2.tar.xz 51504 SHA512:5d99e8b5896e40caee786b4bf0ee9d997d2e9bc08934a193d0ee6e35c750b539c39a20d535b5f4851b7a7f49dddaead2c8a277c824e7b19f7092fb83e2b55832
```

### `dpkg` source package: `bullet=3.06+dfsg-4build2`

Binary Packages:

- `libbullet-dev:amd64=3.06+dfsg-4build2`
- `libbullet3.06:amd64=3.06+dfsg-4build2`

Licenses: (parsed from: `/usr/share/doc/libbullet-dev/copyright`, `/usr/share/doc/libbullet3.06/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSL-1.0`
- `Elsevier-CDROM-License`
- `Expat`
- `GNU-All-Permissive-License`
- `GPL-2`
- `GPL-2+`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris bullet=3.06+dfsg-4build2
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bullet/bullet_3.06%2bdfsg-4build2.dsc' bullet_3.06+dfsg-4build2.dsc 2441 SHA512:530f3b66690f2a1f2864a992615cff7dd3fe4e1198af17afa46c472c688f5c7d5b401c5e6535187b38161d33f592658cf9102adc62224cff483b205157af9792
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bullet/bullet_3.06%2bdfsg.orig.tar.xz' bullet_3.06+dfsg.orig.tar.xz 1565000 SHA512:2e4000a0cf219d8c1a8e15c7eb43f78478d52eeb7566cd920bb43918252e47ce3df79e00d62cfe2085c9b1b9201b2c4fe9b46ff404fa4fa902971df403ca0917
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bullet/bullet_3.06%2bdfsg-4build2.debian.tar.xz' bullet_3.06+dfsg-4build2.debian.tar.xz 13000 SHA512:46ce69dd833d3049d35613c80e2070c0a9604ee9546e34bcfe4cca928658bba95813e9c6e1481d9f93109e7600ad77d0522ba5dc6f07fbd78fb3447ba732bf3f
```

### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `bzip2=1.0.8-5`
- `libbz2-1.0:amd64=1.0.8-5`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

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

### `dpkg` source package: `cairo=1.16.0-5ubuntu2`

Binary Packages:

- `libcairo2:amd64=1.16.0-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libcairo2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-5ubuntu2.dsc' cairo_1.16.0-5ubuntu2.dsc 2880 SHA512:e9415592136e7f42794f20d8c74fed895347a95d3ffd89621440c1e12212f65083926613e87fc6ad6df8f669058dc20ad12b2e1bdee2d7a7f85ec0b7c0dd4e26
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA512:9eb27c4cf01c0b8b56f2e15e651f6d4e52c99d0005875546405b64f1132aed12fbf84727273f493d84056a13105e065009d89e94a8bfaf2be2649e232b82377f
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-5ubuntu2.debian.tar.xz' cairo_1.16.0-5ubuntu2.debian.tar.xz 33368 SHA512:d51b6655b5ea60420bb80252fbcfe2e31cbef6242043457195eab60716b84dc9ae68eb4de95214b10a5ec6d5675891067a4940b58c2249602f0f355b9d31d8d4
```

### `dpkg` source package: `catch2=2.13.8-1`

Binary Packages:

- `catch2=2.13.8-1`

Licenses: (parsed from: `/usr/share/doc/catch2/copyright`)

- `BSD-3`
- `Boost-1.0`

Source:

```console
$ apt-get source -qq --print-uris catch2=2.13.8-1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/catch2/catch2_2.13.8-1.dsc' catch2_2.13.8-1.dsc 1909 SHA512:cf8605069417c2ad6edd423bc78962923246b4945ed24038b11f8ff74cf01d84a856896ed4d96af7d7868ee168befcacf74f4daee7e33ff076a90f916903dfd4
'http://archive.ubuntu.com/ubuntu/pool/universe/c/catch2/catch2_2.13.8.orig.tar.gz' catch2_2.13.8.orig.tar.gz 661681 SHA512:21521738238cd67ebd53a9075ce5888abce10625ded19bfaf52e0ee24ace62e6e0d25f0e991731006c677e9aefd391f67c3a3d3b907a751429a2d559110f70ef
'http://archive.ubuntu.com/ubuntu/pool/universe/c/catch2/catch2_2.13.8-1.debian.tar.xz' catch2_2.13.8-1.debian.tar.xz 4616 SHA512:faa0fab432679f2cbdfabe917d7eef989a0af3dcf37936b1989a851414be868c50106f130c8e49a1cb5dd002a2932b823d762884ac1ecbd17c4160a91d392bb2
```

### `dpkg` source package: `cdebconf=0.256ubuntu4`

Binary Packages:

- `libdebconfclient0:amd64=0.256ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `cmake=3.22.1-1ubuntu1`

Binary Packages:

- `cmake=3.22.1-1ubuntu1`
- `cmake-data=3.22.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cmake/copyright`, `/usr/share/doc/cmake-data/copyright`)

- `Apache-2.0`
- `BSD-0-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-Clause`
- `BSD-4-clause`
- `Expat`
- `GPL-2`
- `GPL-2+with_exception`
- `GPL-3`
- `GPL-3+with_exception`
- `ISC`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris cmake=3.22.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.22.1-1ubuntu1.dsc' cmake_3.22.1-1ubuntu1.dsc 3706 SHA512:ffba326ea6381a60ff08365a572eee2dbdb1bef90b4e4524d5dd1b5e6debb9cdb39b60d06027ffd7d7df3fd5dbbd50cd40392662e27ba33f81b26d7275a8eb00
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.22.1.orig.tar.gz' cmake_3.22.1.orig.tar.gz 9778031 SHA512:b1e900fe573cd1cc76d26386f2298d7722737c9ff67930ee108994972b4561ef69caeb537177c9b95b7f17b755e20e034825d3807ea0d2dd4c391310b03adc11
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.22.1-1ubuntu1.debian.tar.xz' cmake_3.22.1-1ubuntu1.debian.tar.xz 32872 SHA512:73cdf553f4574b62bc004c2ec808efbfb095f106d0412243b7540537b9fd2d9dcff69db21d52462c5bb4f1f0b72967c5dbb2ec7c7d02bf7087a323061bf49829
```

### `dpkg` source package: `console-bridge=1.0.1+dfsg2-3`

Binary Packages:

- `libconsole-bridge-dev:amd64=1.0.1+dfsg2-3`
- `libconsole-bridge1.0:amd64=1.0.1+dfsg2-3`

Licenses: (parsed from: `/usr/share/doc/libconsole-bridge-dev/copyright`, `/usr/share/doc/libconsole-bridge1.0/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris console-bridge=1.0.1+dfsg2-3
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_1.0.1%2bdfsg2-3.dsc' console-bridge_1.0.1+dfsg2-3.dsc 1934 SHA512:1a8a3ec2f852acb95e6bcd15b6a225c444fdec0f3df714c1769632e6815b125e4a987997906ce1040cceb288ac6e92844f88a47698cefbd8f2f0f9136bf13de9
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_1.0.1%2bdfsg2.orig.tar.xz' console-bridge_1.0.1+dfsg2.orig.tar.xz 10352 SHA512:5a6e2feaa843633143418e36d4bffb5b5b1af54d8df0db84b75088f27035e8f7dadaf52aea6c4321cd669e3d9f2f72f42fdb6e3c1ae1092ec4ec08be529beff7
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_1.0.1%2bdfsg2-3.debian.tar.xz' console-bridge_1.0.1+dfsg2-3.debian.tar.xz 4020 SHA512:4ddd2886430091dcb4d50a88aa58dad5317030075ef9de9e8d5368ba8c8f280ce6d6714a5b78a090a1435f9094d82e7e0a151cb3cc130cb6c51d268f6955fe91
```

### `dpkg` source package: `coreutils=8.32-4ubuntu3`

Binary Packages:

- `coreutils=8.32-4ubuntu3`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `cov-core=1.15.0-3build1`

Binary Packages:

- `python3-cov-core=1.15.0-3build1`

Licenses: (parsed from: `/usr/share/doc/python3-cov-core/copyright`)

- `Expat/MIT`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris cov-core=1.15.0-3build1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cov-core/cov-core_1.15.0-3build1.dsc' cov-core_1.15.0-3build1.dsc 2065 SHA512:a5bf1975efce6d7395f4a78957ee1ab9c5c02050ccca747116407ddcecd979e6f2268ab2c4fc0d55e00ba39c23bb549dc41c9152909a8a886e2dac01a5030a6e
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cov-core/cov-core_1.15.0.orig.tar.gz' cov-core_1.15.0.orig.tar.gz 5890 SHA512:1b962a6a7253c1f6530248f3a71058e7709ee5cca274166807f040163c9cc240e9e85e42820063476c1c0f6dfca81d45277738663ed818fe715b30db151ace16
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cov-core/cov-core_1.15.0-3build1.debian.tar.xz' cov-core_1.15.0-3build1.debian.tar.xz 3888 SHA512:9fbd917e72d68b5519949aaff0215be00b6b40e1c1f705214ec0f3575eaef035feca0b71d36b999cd6eb7f4c8798de980b945db3013c2437f5c48dec5d14186d
```

### `dpkg` source package: `cppcheck=2.7-1`

Binary Packages:

- `cppcheck=2.7-1`

Licenses: (parsed from: `/usr/share/doc/cppcheck/copyright`)

- `BSD-2`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris cppcheck=2.7-1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cppcheck/cppcheck_2.7-1.dsc' cppcheck_2.7-1.dsc 2186 SHA512:edb8f968e5cef167a27c9dbd140043f41a0a06cd77b7437a850216b8013c65e952ce3fbba53b44d7f33c1fec80cd8f07e54e0a1fc3e0414a455959e30b255374
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cppcheck/cppcheck_2.7.orig.tar.gz' cppcheck_2.7.orig.tar.gz 3939557 SHA512:62f00957476dbb4de700550bf299fd56c23ee105846d725b78e6b61417f0ecb4283e24528b72d04fea3aed43282968902c12fdb527fdd5e07e6b05764b150e1e
'http://archive.ubuntu.com/ubuntu/pool/universe/c/cppcheck/cppcheck_2.7-1.debian.tar.xz' cppcheck_2.7-1.debian.tar.xz 11868 SHA512:302c38afba279b636be1cdc7ce2a13612fe71a9e56a2e50cf6fa86d6596de17fa0d8132752c98a3e894ea47271f6a92817433c8d432bd6486bd0a77aecbdfa2d
```

### `dpkg` source package: `curl=7.81.0-1`

Binary Packages:

- `libcurl3-gnutls:amd64=7.81.0-1`
- `libcurl4:amd64=7.81.0-1`

Licenses: (parsed from: `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

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

### `dpkg` source package: `dbus-python=1.2.18-3`

Binary Packages:

- `python3-dbus=1.2.18-3`

Licenses: (parsed from: `/usr/share/doc/python3-dbus/copyright`)

- `AFL-2.1`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dbus-python=1.2.18-3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.18-3.dsc' dbus-python_1.2.18-3.dsc 3112 SHA512:8268bb83b03aa4c5a1619907c4ddc8bfbcfdd26621c31ffcb377f4cbd0c58a2ffd86577831e97cc453d13d58f08441979f4341217df6c320fec7ab84e1986c87
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.18.orig.tar.gz' dbus-python_1.2.18.orig.tar.gz 578204 SHA512:72f422c59637392bd78b741b66dff2afadcc706452c3e82fdc14b1dc052a0c5cb8a85e2758d18c5cbdc08004419a0b3c16b67b99688d96307084403e72585900
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.18.orig.tar.gz.asc' dbus-python_1.2.18.orig.tar.gz.asc 833 SHA512:5f8b0c8c1771f4e8ace9168c02f04d0e065cfa8dfdaf7e7d991232e42e0f77bef9d72c565a053ed0cee1ac75b5ab7b929fcdb88d34b21f1489107ea4847ada0a
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus-python/dbus-python_1.2.18-3.debian.tar.xz' dbus-python_1.2.18-3.debian.tar.xz 34184 SHA512:59aea346a9d783194509b503a265351993558f74eeb9246380d0c80fdbecf28c551e27197a300b2da07e71af0a960947ba2c865bfa545b6e76c23c086df1ac1c
```

### `dpkg` source package: `dbus=1.12.20-2ubuntu3`

Binary Packages:

- `libdbus-1-3:amd64=1.12.20-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libdbus-1-3/copyright`)

- `AFL-2.1`
- `AFL-2.1,`
- `BSD-3-clause`
- `BSD-3-clause-generic`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `Tcl-BSDish`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris dbus=1.12.20-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.20-2ubuntu3.dsc' dbus_1.12.20-2ubuntu3.dsc 3393 SHA512:2149bf1df60ad3abb29f9f6be4c48d2c7968b0bf2a216acb59d5218e033ed886fda3c2cd035f5c78e6203da3191d991b11b3f29e87150630aebd9b82db1a2fbc
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.20.orig.tar.gz' dbus_1.12.20.orig.tar.gz 2095511 SHA512:0964683bc6859374cc94e42e1ec0cdb542cca67971c205fcba4352500b6c0891665b0718e7d85eb060c81cb82e3346c313892bc02384da300ddd306c7eef0056
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.12.20-2ubuntu3.debian.tar.xz' dbus_1.12.20-2ubuntu3.debian.tar.xz 62548 SHA512:9242e39cc72e97b6f7835a859bbb8c41fb114cab80acbfcced35d5e9cb1c8d138dc29a59803e41887810039561e9230c844cc35c2cb7056aaeedc678bde26214
```

### `dpkg` source package: `debconf=1.5.79`

Binary Packages:

- `debconf=1.5.79`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debconf/1.5.79/


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

### `dpkg` source package: `dh-elpa=2.0.9ubuntu1`

Binary Packages:

- `dh-elpa-helper=2.0.9ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dh-elpa-helper/copyright`)

- `CC0`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris dh-elpa=2.0.9ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/dh-elpa/dh-elpa_2.0.9ubuntu1.dsc' dh-elpa_2.0.9ubuntu1.dsc 1913 SHA512:f62b9edb5444fe1c2ab76f4a70842501911a34bfd2b32ab5a30fa008e145dabc699b49565fa04b4d933ba18e72743255ad441fcdf8f7f3779650c36a09ce6de3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dh-elpa/dh-elpa_2.0.9ubuntu1.tar.xz' dh-elpa_2.0.9ubuntu1.tar.xz 25752 SHA512:bae62af7dfb289252a90bf5681b9f303020e794632222a92edf592cfc20be06a7dc57eb04c36c37e3dea23481a7f7419007b6d2b36ba89d6e2e435f984dd8f8a
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

### `dpkg` source package: `distlib=0.3.4-1`

Binary Packages:

- `python3-distlib=0.3.4-1`

Licenses: (parsed from: `/usr/share/doc/python3-distlib/copyright`)

- `BSD-3-clause`
- `Python`

Source:

```console
$ apt-get source -qq --print-uris distlib=0.3.4-1
'http://archive.ubuntu.com/ubuntu/pool/universe/d/distlib/distlib_0.3.4-1.dsc' distlib_0.3.4-1.dsc 1809 SHA512:9542ad50dbcf1e5129914e8704d28583f3a03ce20be3303e001ee3c68c61adcdb67733b5e439642aece760c3b58da6e6893dc0d0ff5b81fb4548e06551f7f5b9
'http://archive.ubuntu.com/ubuntu/pool/universe/d/distlib/distlib_0.3.4.orig.tar.xz' distlib_0.3.4.orig.tar.xz 342000 SHA512:dd4576d09e171d25ecf345fc202e9088052a8021025f20dff65fa5a790d66d6d2c8791fc32d2891536d60206fccd5544f3c2e07fec6dec5a99623d4dd0258fa1
'http://archive.ubuntu.com/ubuntu/pool/universe/d/distlib/distlib_0.3.4-1.debian.tar.xz' distlib_0.3.4-1.debian.tar.xz 6296 SHA512:8c6d132d712b26ec79bbbaee349901456e14fc5a921e0da4dc32d98595384ce05ba78cae9450b5289cc35ea60fcd21991a6a98cb3571a7dbd8d79aae57f6f27a
```

### `dpkg` source package: `distro-info-data=0.52`

Binary Packages:

- `distro-info-data=0.52`

Licenses: (parsed from: `/usr/share/doc/distro-info-data/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris distro-info-data=0.52
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.52.dsc' distro-info-data_0.52.dsc 1101 SHA512:6475fb2ece6d8bf61e7f753d9f59724305d60826a571e7a17e59cb9189912009d3d2415aca2ca7ddacda64020d8709b4e16b00dae7e5f842e4ff9d237e780c61
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.52.tar.xz' distro-info-data_0.52.tar.xz 9124 SHA512:807f14e5586ac86f8b097d678053486aa4d06fd220eb1aa01f81972678a81e29e3d466717f09990cf605316095b002a51e645a21a75aa08289a4ae5993707b68
```

### `dpkg` source package: `dpkg=1.21.1ubuntu1`

Binary Packages:

- `dpkg=1.21.1ubuntu1`
- `dpkg-dev=1.21.1ubuntu1`
- `libdpkg-perl=1.21.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

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

### `dpkg` source package: `eigen3=3.4.0-2ubuntu2`

Binary Packages:

- `libeigen3-dev=3.4.0-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libeigen3-dev/copyright`)

- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-2`

Source:

```console
$ apt-get source -qq --print-uris eigen3=3.4.0-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/e/eigen3/eigen3_3.4.0-2ubuntu2.dsc' eigen3_3.4.0-2ubuntu2.dsc 2277 SHA512:3df6c64e7becb79056eb462357bd4b5b60dfb8748ce42b47e8c5904a4569f56785a98fca08ec665598d196b182dd49c34029961bcd7791ba0ddca90fdb900a61
'http://archive.ubuntu.com/ubuntu/pool/universe/e/eigen3/eigen3_3.4.0.orig.tar.bz2' eigen3_3.4.0.orig.tar.bz2 2143091 SHA512:cc488eb111e0e248744d2bc4475b345b5fb82361dff226a5b73a33bd0388de8c219cff8cffcf8f476b672fc0e223f339e8c6a1cfb6293840a4a6abf232438a89
'http://archive.ubuntu.com/ubuntu/pool/universe/e/eigen3/eigen3_3.4.0-2ubuntu2.debian.tar.xz' eigen3_3.4.0-2ubuntu2.debian.tar.xz 19656 SHA512:84150ddd6e36fc49df6631b4112587f5162ae76853119afcf262f1613512d96589bfb0f72815ab772bc41b3a58708384033e5495be17a6be6b78dd88e1772953
```

### `dpkg` source package: `emacsen-common=3.0.4`

Binary Packages:

- `emacsen-common=3.0.4`

Licenses: (parsed from: `/usr/share/doc/emacsen-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris emacsen-common=3.0.4
'http://archive.ubuntu.com/ubuntu/pool/main/e/emacsen-common/emacsen-common_3.0.4.dsc' emacsen-common_3.0.4.dsc 1463 SHA512:1c6ee66d7da5e4ff3efde5f7be797f983ec4fde72ec5c713b2af14fc7cace569bde3a1b62bd12f4ba912ea3d80055816b43e6d19f50ca377a779e3adc468fac9
'http://archive.ubuntu.com/ubuntu/pool/main/e/emacsen-common/emacsen-common_3.0.4.tar.xz' emacsen-common_3.0.4.tar.xz 16292 SHA512:0bc4eb00245c6f5ac6d26558656dbef7ad865c7612b37ad0cb0cca82236b17a4a3c0360f2042cc8700f30c955895ab09d1e79901b74a934f55578255a9989c28
```

### `dpkg` source package: `empy=3.3.4-2`

Binary Packages:

- `python3-empy=3.3.4-2`

Licenses: (parsed from: `/usr/share/doc/python3-empy/copyright`)

- `GPL-2`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris empy=3.3.4-2
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.4-2.dsc' empy_3.3.4-2.dsc 1667 SHA512:826b2b4dae78c717bd9ca41f3c13aeb259eaff690c00ad96f907c1c85084dd7dca7787b94d95955d20654f3b4e41e45411150d6c2d35a5110b5232b0752ee278
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.4.orig.tar.gz' empy_3.3.4.orig.tar.gz 63169 SHA512:1bfe1a93926ecd245ba2fbb77bcc1c9b08515260263eb4ce20701c042f5bb0d8184183c0bcfb9342355aa4baaf4439211ce6dc078818b5d434a5f46e46124f1f
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.4-2.debian.tar.xz' empy_3.3.4-2.debian.tar.xz 10056 SHA512:f154ff0e426211b664a387f8a187aff2c5fd423f65a7e7849982a8aad4e61668e70db6ef7f581fbea0a90950b217e3e3acf265c2b4ca03fa05dd78dd135ef1f6
```

### `dpkg` source package: `expat=2.4.4-1`

Binary Packages:

- `libexpat1:amd64=2.4.4-1`
- `libexpat1-dev:amd64=2.4.4-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/expat/2.4.4-1/


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

### `dpkg` source package: `fmtlib=8.1.1+ds1-2`

Binary Packages:

- `libfmt-dev:amd64=8.1.1+ds1-2`
- `libfmt8:amd64=8.1.1+ds1-2`

Licenses: (parsed from: `/usr/share/doc/libfmt-dev/copyright`, `/usr/share/doc/libfmt8/copyright`)

- `BSD-2-Clause`
- `CC0-1.0`
- `Expat`
- `Expat with embedded exception`
- `Python`

Source:

```console
$ apt-get source -qq --print-uris fmtlib=8.1.1+ds1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fmtlib/fmtlib_8.1.1%2bds1-2.dsc' fmtlib_8.1.1+ds1-2.dsc 1480 SHA512:a7075ed1742ae95133647dde33f17654578858d0deafc6b259adbfaf2a81e0eea069fd4af1212d2327b92f3a5b0cfdca9654e3f0b6ab160ed0dd142cc9e21d16
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fmtlib/fmtlib_8.1.1%2bds1.orig.tar.gz' fmtlib_8.1.1+ds1.orig.tar.gz 306710 SHA512:fa90ba870d22a8b22fd933e41fccf5b760c0095161dbe5d94e28d919a34c788f407d9502a4090f0ea36beea8529308e858c5d0d7edf59eb3166d040eebdcd5bb
'http://archive.ubuntu.com/ubuntu/pool/universe/f/fmtlib/fmtlib_8.1.1%2bds1-2.debian.tar.xz' fmtlib_8.1.1+ds1-2.debian.tar.xz 13240 SHA512:821f21d9d4ea403abfd202d67aa145e6ce578f7929a875b8b865219efde85ab937e46bf1dfde0544ee3467cb36343ed5ce5a0ed938022339d9950a364b65057f
```

### `dpkg` source package: `fontconfig=2.13.1-4.2ubuntu4`

Binary Packages:

- `fontconfig=2.13.1-4.2ubuntu4`
- `fontconfig-config=2.13.1-4.2ubuntu4`
- `libfontconfig1:amd64=2.13.1-4.2ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-4.2ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-4.2ubuntu4.dsc' fontconfig_2.13.1-4.2ubuntu4.dsc 2815 SHA512:f011b22b9b4b0e8967e208fb5b6060f30ec168f1b13669a59064e41a2d566e71bdc93286e1905d2f1d2a63119b5ec1402abaf44dfb4af4a7e37a4d2225ea4b8c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA512:f97f2a9db294fd72d416a7d76dd7db5934ade2cf76903764b09e7decc33e0e2eed1a1d35c5f1c7fd9ea39e2c7653b9e65365f0c6205e047e95e38ba5000dd100
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-4.2ubuntu4.debian.tar.xz' fontconfig_2.13.1-4.2ubuntu4.debian.tar.xz 28048 SHA512:e2fd60cc3ba92801e3e90b736745d1aed25596935c0b3b79e3e1eaa4dd91067e59df24db403949ffa0756dbab9a79de6946630ca64cfaaf960f2c39b9b1ddc5e
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

### `dpkg` source package: `freetype=2.11.1+dfsg-1`

Binary Packages:

- `libfreetype6:amd64=2.11.1+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

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
$ apt-get source -qq --print-uris freetype=2.11.1+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1%2bdfsg-1.dsc' freetype_2.11.1+dfsg-1.dsc 3713 SHA512:42415e8ecbd9da21e0ff075e39eddb123e4654a3f92dced474d2384f66ecebb03ec4842899ab4e933d8ba73e4eddac63b91491954cfe05791d1d49aef534b98a
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2demos.tar.xz' freetype_2.11.1+dfsg.orig-ft2demos.tar.xz 257240 SHA512:93d68daefa8a49b4fc987a7356133299fe2a8e012415ea09ad7616ececcfd978fdf9fc7a2d855f7488f51a497d019acb89ef5774484babae66357b3083a883c5
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.11.1+dfsg.orig-ft2demos.tar.xz.asc 195 SHA512:407ffade07cc62c8838d26670dffc7c26b9baf4984c42b2b2467279dabda855536b403f5a7e9dc64a787163657ca81019fef6d1879973faf180d6230ab17cd05
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2docs.tar.xz' freetype_2.11.1+dfsg.orig-ft2docs.tar.xz 2038348 SHA512:c5e19d98425491682edc58230c48390925cc4b466169f655cf3b8575ba787a70feecdeb7a16224b132dcc32f17b041483d84056cda8e3132d98b531e46a26c36
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.11.1+dfsg.orig-ft2docs.tar.xz.asc 195 SHA512:df946695a1fbaa71009f48a8f0860177984728ec1c73385d1e55c07be027dd6a5e634c9dcbb49c51f8143b0d56a6cbf06393403341fb28cea7a8a2cc9a9c5592
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1%2bdfsg.orig.tar.xz' freetype_2.11.1+dfsg.orig.tar.xz 1988020 SHA512:6a9a0379679abf127761cabb2da39b8faf2ca4c322075da9b86d93363ac81ce909b9544377a784118ba91ca008baa680b9da474bd2da1bfe928d5a4c9114cb08
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1%2bdfsg-1.debian.tar.xz' freetype_2.11.1+dfsg-1.debian.tar.xz 40132 SHA512:c0a9b0cd8ebc8fc7e85701ba459ac946954d3a473ab069d7db8cb1dbcc8551a431e4abd36e448db2464f0e409c869683d3a1b7be07d4867540fe5b63673dd2ec
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

### `dpkg` source package: `gcc-11=11.2.0-16ubuntu1`

Binary Packages:

- `cpp-11=11.2.0-16ubuntu1`
- `g++-11=11.2.0-16ubuntu1`
- `gcc-11=11.2.0-16ubuntu1`
- `gcc-11-base:amd64=11.2.0-16ubuntu1`
- `libasan6:amd64=11.2.0-16ubuntu1`
- `libgcc-11-dev:amd64=11.2.0-16ubuntu1`
- `libstdc++-11-dev:amd64=11.2.0-16ubuntu1`
- `libtsan0:amd64=11.2.0-16ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp-11/copyright`, `/usr/share/doc/g++-11/copyright`, `/usr/share/doc/gcc-11/copyright`, `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libgcc-11-dev/copyright`, `/usr/share/doc/libstdc++-11-dev/copyright`, `/usr/share/doc/libtsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.2.0-16ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-16ubuntu1.dsc' gcc-11_11.2.0-16ubuntu1.dsc 27910 SHA512:f6ffb6571af0cae4be08d2f1d06863bb1e29d3a7c935e13460dc170f65c844222bf0d4cd72b714ab9771d82b58131af161a094b439c62d485ee2dede7267d380
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0.orig.tar.gz' gcc-11_11.2.0.orig.tar.gz 87861992 SHA512:64e4634769a62faa0adbfe99e5e590dd9efc1facac20a7dd71ab9f1d675e7df80678cbdc75c966e08ccf91dbc1e1a681d8e3227d0026ffcb5f46bdc96acaace8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-16ubuntu1.debian.tar.xz' gcc-11_11.2.0-16ubuntu1.debian.tar.xz 2033548 SHA512:e259a01556809730e42ada412a3e0acdb676eae6d934607058a3f0ad310e5eade0f4f7d258f6c5920c96362a12497eb651b4cde03420569b1cc31d2add6d3199
```

### `dpkg` source package: `gcc-12=12-20220222-1ubuntu1`

Binary Packages:

- `gcc-12-base:amd64=12-20220222-1ubuntu1`
- `libatomic1:amd64=12-20220222-1ubuntu1`
- `libcc1-0:amd64=12-20220222-1ubuntu1`
- `libgcc-s1:amd64=12-20220222-1ubuntu1`
- `libgfortran5:amd64=12-20220222-1ubuntu1`
- `libgomp1:amd64=12-20220222-1ubuntu1`
- `libitm1:amd64=12-20220222-1ubuntu1`
- `liblsan0:amd64=12-20220222-1ubuntu1`
- `libquadmath0:amd64=12-20220222-1ubuntu1`
- `libstdc++6:amd64=12-20220222-1ubuntu1`
- `libubsan1:amd64=12-20220222-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12-20220222-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12-20220222-1ubuntu1.dsc' gcc-12_12-20220222-1ubuntu1.dsc 27784 SHA512:8d3fdd7136dad82a5699bf72090d5f0cd518f18c2e0bedba36e0b6a50766c6e5a0aa45905b3bde0dd29079707766dcb3774d69e8826e677f5f923a7a1940bfc8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12-20220222.orig.tar.gz' gcc-12_12-20220222.orig.tar.gz 84486569 SHA512:2255e4d1f3fb53dcf04029f2f5a8880d2d76abe855e522b73074d6d6356f5bfe2f8c897d023f1dc3d26cb22b45c25729e7bd2985f666a30ee2563dc637de0826
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-12/gcc-12_12-20220222-1ubuntu1.debian.tar.xz' gcc-12_12-20220222-1ubuntu1.debian.tar.xz 560852 SHA512:e4d25ceda8ffa775e2593c4f3aa7926efed9546673abe8b74b2a5881936f145e4ced898ed458b19080d8ecd3a93570c21c580efd46435e402bae4b9b4ee5c06c
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

### `dpkg` source package: `glib2.0=2.71.2-1`

Binary Packages:

- `libglib2.0-0:amd64=2.71.2-1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.71.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.71.2-1.dsc' glib2.0_2.71.2-1.dsc 3536 SHA512:ecb970fa25c6176bd31f0d44d7f7badb45e87cca7843f89b0ee05f66047b4298654a82b60f42bc93240ad12fe00513659d1590add71fb454a6e9c902461abfe4
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.71.2.orig.tar.xz' glib2.0_2.71.2.orig.tar.xz 4880616 SHA512:21b7076c21b9a7c4ff937a58e3b1d05a3d351a74dec3d40674d0e3069d05b57e072efad5c3b23332bd6d2098bc2960dd2de5d43757a27346a6bc30a3ffce9cd1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.71.2-1.debian.tar.xz' glib2.0_2.71.2-1.debian.tar.xz 103332 SHA512:204b44574ea5c4ac55d3cf59a5a8ad18f38720f16013e45c7dfdeeb030f83bed843e491793f85eb251d5f7b37873c5e827a3056b508f0bdc0ebafd81996ca881
```

### `dpkg` source package: `glibc=2.35-0ubuntu1`

Binary Packages:

- `libc-bin=2.35-0ubuntu1`
- `libc-dev-bin=2.35-0ubuntu1`
- `libc6:amd64=2.35-0ubuntu1`
- `libc6-dev:amd64=2.35-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GFDL-1.3`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.35-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35-0ubuntu1.dsc' glibc_2.35-0ubuntu1.dsc 8876 SHA512:202cdee3da32c0596eff7b84bbdfac55c706becce0ff0776b6d89924165aa21946b5fcf0c95fa505a9f594c9ea657a5e811782b80b98fef6278aac7a6c3c6e2b
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35.orig.tar.xz' glibc_2.35.orig.tar.xz 18165952 SHA512:e7336ce27561be5d7c217832a1136fb327e057bd8d3f92925b35c97e3e9f9e486948b5a1e03e5e4090772ef06437a074d10b82e68f17f1ad8f22077ee39e1b66
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35.orig.tar.xz.asc' glibc_2.35.orig.tar.xz.asc 833 SHA512:2a1c152511dac05f9b4e48f7e7a6b59dbf2d8b71fea54f128173113357be26e86216e13c9865f617049e6858396a221a5abc704f65a786b22453945fd80265e9
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.35-0ubuntu1.debian.tar.xz' glibc_2.35-0ubuntu1.debian.tar.xz 875676 SHA512:5db5ee8734867629123786c19d9f395bdc735b24c68a17aa2e238d63a7fa99792dc3c771fd283d56d2d396fca3555bbafb46bc8af70f275b6b4631774889bf52
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
- `gnupg2=2.2.27-3ubuntu1`
- `gpg=2.2.27-3ubuntu1`
- `gpg-agent=2.2.27-3ubuntu1`
- `gpg-wks-client=2.2.27-3ubuntu1`
- `gpg-wks-server=2.2.27-3ubuntu1`
- `gpgconf=2.2.27-3ubuntu1`
- `gpgsm=2.2.27-3ubuntu1`
- `gpgv=2.2.27-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-l10n/copyright`, `/usr/share/doc/gnupg-utils/copyright`, `/usr/share/doc/gnupg2/copyright`, `/usr/share/doc/gpg/copyright`, `/usr/share/doc/gpg-agent/copyright`, `/usr/share/doc/gpg-wks-client/copyright`, `/usr/share/doc/gpg-wks-server/copyright`, `/usr/share/doc/gpgconf/copyright`, `/usr/share/doc/gpgsm/copyright`, `/usr/share/doc/gpgv/copyright`)

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

### `dpkg` source package: `googletest=1.11.0-3`

Binary Packages:

- `google-mock:amd64=1.11.0-3`
- `googletest=1.11.0-3`
- `libgtest-dev:amd64=1.11.0-3`

Licenses: (parsed from: `/usr/share/doc/google-mock/copyright`, `/usr/share/doc/googletest/copyright`, `/usr/share/doc/libgtest-dev/copyright`)

- `Apache`
- `BSD-C3`
- `GAP`

Source:

```console
$ apt-get source -qq --print-uris googletest=1.11.0-3
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.11.0-3.dsc' googletest_1.11.0-3.dsc 2212 SHA512:b3c48915e8df612563fbd032104bcddd8a474213351ce2896723617839635a4a570eaf3d0c4441e921db75ffa69037b320afa3230b0e478e01ee5be3fdb85518
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.11.0.orig.tar.gz' googletest_1.11.0.orig.tar.gz 886169 SHA512:8fe2e40add39f90b30e8eb1f6a70142966ba55c26e103eacf75bc4b8306e1065bb23adc16b1f5ae8e67a5359af4a9fdb8f413c84cf5814e9a50a186123c3da54
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.11.0-3.debian.tar.xz' googletest_1.11.0-3.debian.tar.xz 13488 SHA512:60bc6ec4b8b86f2930b44d64b20237d544e64d800e66df66fb44c1b80d89272d131112af2387615762e29ca03d4e0c9dc717fccdc6653cf3cb8a8b878801998b
```

### `dpkg` source package: `graphite2=1.3.14-1build1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.14-1build1`

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
$ apt-get source -qq --print-uris graphite2=1.3.14-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1build1.dsc' graphite2_1.3.14-1build1.dsc 2632 SHA512:c6cbc4a7a0cf1c4e8bb3acbfb7252c2dc87c7a238f9cf0797dda9091d80dcf76a62e15a178636fdd2a39761271cfb63fcb29a5a534d062e1153977a8f28be5df
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14.orig.tar.gz' graphite2_1.3.14.orig.tar.gz 6629829 SHA512:49d127964d3f5c9403c7aecbfb5b18f32f25fe4919a81c49e0534e7123fe845423e16b0b8c8baaae21162b1150ab3e0f1c22c344e07d4364b6b8473c40a0822c
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.14-1build1.debian.tar.xz' graphite2_1.3.14-1build1.debian.tar.xz 12156 SHA512:ffbc74c5a9d4c616722ebcb48b72d0354e88c774b0120492de85adefa346e4a3f81641924dcd7f914e77b9871546f2ba4da1905fd3f38d92007af8f3ce38e137
```

### `dpkg` source package: `graphviz=2.42.2-5build1`

Binary Packages:

- `graphviz=2.42.2-5build1`
- `libcdt5:amd64=2.42.2-5build1`
- `libcgraph6:amd64=2.42.2-5build1`
- `libgvc6=2.42.2-5build1`
- `libgvpr2:amd64=2.42.2-5build1`
- `liblab-gamut1:amd64=2.42.2-5build1`
- `libpathplan4:amd64=2.42.2-5build1`

Licenses: (parsed from: `/usr/share/doc/graphviz/copyright`, `/usr/share/doc/libcdt5/copyright`, `/usr/share/doc/libcgraph6/copyright`, `/usr/share/doc/libgvc6/copyright`, `/usr/share/doc/libgvpr2/copyright`, `/usr/share/doc/liblab-gamut1/copyright`, `/usr/share/doc/libpathplan4/copyright`)

- `EPL-1.0`
- `MIT`
- `X/MIT`
- `zlib-style`

Source:

```console
$ apt-get source -qq --print-uris graphviz=2.42.2-5build1
'http://archive.ubuntu.com/ubuntu/pool/universe/g/graphviz/graphviz_2.42.2-5build1.dsc' graphviz_2.42.2-5build1.dsc 3253 SHA512:b4450035b88d8b14b2561971142d98f0be6bbfe63424287686fe3e152ed65bc80971e803ed99fde55d24cc2b4bcf8b57a4c3f5b09c1c4b12c770dd6c7b45702d
'http://archive.ubuntu.com/ubuntu/pool/universe/g/graphviz/graphviz_2.42.2.orig.tar.bz2' graphviz_2.42.2.orig.tar.bz2 30740923 SHA512:7dab159539179df1febf4396d6bea2c071e0f311745941a07861d54b1db96a52f1328bee08148e099fa06ce5f1c9a9b6272ba60bb6147bf51b55de881a431fb3
'http://archive.ubuntu.com/ubuntu/pool/universe/g/graphviz/graphviz_2.42.2-5build1.debian.tar.xz' graphviz_2.42.2-5build1.debian.tar.xz 39008 SHA512:87c1c62dd84e7db318d128c0694129412cc5698eb23fef3fb63fc01bab24feb3526f2df78e6ac3030d0c93b5f6ce3d3200eb44e94da4040274af367b215a0030
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

### `dpkg` source package: `gts=0.7.6+darcs121130-5`

Binary Packages:

- `libgts-0.7-5:amd64=0.7.6+darcs121130-5`

Licenses: (parsed from: `/usr/share/doc/libgts-0.7-5/copyright`)

- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gts=0.7.6+darcs121130-5
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gts/gts_0.7.6%2bdarcs121130-5.dsc' gts_0.7.6+darcs121130-5.dsc 2109 SHA512:f21c97dde3e495778bc0a2794f5db0fba90796fbe33ba9e71326e39894a14fa6a86822e7ea690165379bbe244586eb03326d4a474e3d9adcbca12d4a4000bb8b
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gts/gts_0.7.6%2bdarcs121130.orig.tar.gz' gts_0.7.6+darcs121130.orig.tar.gz 880569 SHA512:84c38dc345830eea75755d9d55235b6d76786a84c3b9c3b7e057437bf395a9f2687596bbf037afd601b9f31a485d425a371ca5e60680265f10cb414400db4142
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gts/gts_0.7.6%2bdarcs121130-5.debian.tar.xz' gts_0.7.6+darcs121130-5.debian.tar.xz 13344 SHA512:d1c066ff5ee677e976b9e3cbc4f68cba78a61035b562cdc6fd41ea798a069a26bffc1fa1ccd6e015df59b1a28abbe09e8bdb16529835bd7c5af30f81a7ee83a0
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

### `dpkg` source package: `harfbuzz=2.7.4-1ubuntu3`

Binary Packages:

- `libharfbuzz0b:amd64=2.7.4-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.7.4-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu3.dsc' harfbuzz_2.7.4-1ubuntu3.dsc 2872 SHA512:86e4c1ae67c0982119119c71b0ba00deda9d12b769c0549f83f38a9346ffae6d1d103307114974598e4d0fa42e56ccaa2b2b5b91a43dcb81c72ac4db091a295c
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4.orig.tar.xz' harfbuzz_2.7.4.orig.tar.xz 9532468 SHA512:d2af6a768c397c664f654cf36140e7b5696b3b983f637454604570c348247f7ffea135048d9b02cf6593cbde728567e31bf82a39df5ff38d680c78dff24d4cf0
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu3.debian.tar.xz' harfbuzz_2.7.4-1ubuntu3.debian.tar.xz 11068 SHA512:22189a09bf0f435ae26f597ce9809fe12ebb9bcbbcbcd1d5d75d54d1cfdc148ee2b375497368afa72040ce0cd848d3cd0f04b9154e48201de4bb26bd2a9e525e
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

### `dpkg` source package: `icu=70.1-2`

Binary Packages:

- `libicu70:amd64=70.1-2`

Licenses: (parsed from: `/usr/share/doc/libicu70/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu=70.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_70.1-2.dsc' icu_70.1-2.dsc 2252 SHA512:e1bad285bb7f66be62b8b9d595b289095621a88b0c5a2141b7317473ac25ab30a4b83de38ce215d6b7e0e135b2101ed7ab7bcf6d9b3666b4a554095b0ed6d1de
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_70.1.orig.tar.gz' icu_70.1.orig.tar.gz 25449582 SHA512:0b26ae7207155cb65a8fdb25f7b2fa4431e74b12bccbed0884a17feaae3c96833d12451064dd152197fd6ea5fd3adfd95594284a463e66c82e0d860f645880c9
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_70.1.orig.tar.gz.asc' icu_70.1.orig.tar.gz.asc 659 SHA512:17f65641de023b81f18588c5b1be6f88a8d308565343b09241ecfdc6250caeeb785e666d0772b668d5cb0fb243abc88766f02d27b273946e946e8c339cbca942
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_70.1-2.debian.tar.xz' icu_70.1-2.debian.tar.xz 62440 SHA512:ca6771b09b9f232e69b3f6fd6c3445c9b27d86c918a6b52c903a2ebe658b273ea5181fcc3030aaad90450f9d86e620fdd42e710ed81c90c29d889ecfd44c6700
```

### `dpkg` source package: `init-system-helpers=1.61`

Binary Packages:

- `init-system-helpers=1.61`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/init-system-helpers/1.61/


### `dpkg` source package: `isl=0.24-2`

Binary Packages:

- `libisl23:amd64=0.24-2`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.24-2
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24-2.dsc' isl_0.24-2.dsc 1832 SHA512:4600f20562f21f3c9fe8a8e5ee220d4db5eb9cc6f0b679d268e779df254b7333ec0a7072870fadfa4c41631b17dad4e772b6e95d3f368bcbb35fa04b88c51cac
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24.orig.tar.xz' isl_0.24.orig.tar.xz 1930956 SHA512:ff6bdcff839e1cd473f2a0c1e4dd4a3612ec6fee4544ccbc62b530a7248db2cf93b4b99bf493a86ddf2aba00e768927265d5d411f92061ea85fd7929073428e8
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.24-2.debian.tar.xz' isl_0.24-2.debian.tar.xz 26476 SHA512:d5232d4e71e23e33376a342399fb352d64c1ea035f5142fa2ff60e621f3dfba198018092c7f01aaf76fe9b77dc66dcf75c660064ce2e88ee62f6998297fbf122
```

### `dpkg` source package: `jbigkit=2.1-3.1build2`

Binary Packages:

- `libjbig0:amd64=2.1-3.1build2`

Licenses: (parsed from: `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1build2
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build2.dsc' jbigkit_2.1-3.1build2.dsc 2081 SHA512:3a120abc6bb211fbb1f58eba95da2a2f92f2df840a618e771b638fdc70dec0f769cc4bceff584f105764f57b99af2c5e6122df03e7c6447a7127444fe06243ad
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA512:c4127480470ef90db1ef3bd2caa444df10b50ed8df0bc9997db7612cb48b49278baf44965028f1807a21028eb965d677e015466306b44683c4ec75a23e1922cf
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build2.debian.tar.xz' jbigkit_2.1-3.1build2.debian.tar.xz 7728 SHA512:811d534138de41e727cd8e13d3c6ab178b010c7a13696977bb8302d04c2561dd7497df2c3664185dbafbe14661c1403f4aa46a32a92cc0fd3641dfbd92c8b7d9
```

### `dpkg` source package: `jquery-goodies=12-3`

Binary Packages:

- `libjs-jquery-metadata=12-3`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-metadata/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris jquery-goodies=12-3
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-goodies/jquery-goodies_12-3.dsc' jquery-goodies_12-3.dsc 3598 SHA512:615a8766df5d119fabf4d457751e2562e465026c22acd866bfbad35a31fda5faac0f71f486b291dc4b24d8f5e302c8c3dd544536cfb715377130c52c5021aa06
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-goodies/jquery-goodies_12.orig.tar.xz' jquery-goodies_12.orig.tar.xz 1238604 SHA512:a4da2cb231a8e8b9d6fbd75d99fd41c1f029f9a5939f5babeb436c8a6e3dc06d9c1bac353d1739398213e2ebea719c0019fa1a62a41de69335d9198e613995e8
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-goodies/jquery-goodies_12-3.debian.tar.xz' jquery-goodies_12-3.debian.tar.xz 12724 SHA512:9a4be31edc636921c6d5c2be7070a419c121f6f99fbf46458c85902111f2b16d85fcd447ec540e1f6b9ab2719cea0901f4bec1ba11dd5279309063b907883e43
```

### `dpkg` source package: `jquery-tablesorter=1:2.31.3+dfsg1-3`

Binary Packages:

- `libjs-jquery-tablesorter=1:2.31.3+dfsg1-3`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-tablesorter/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-2+`
- `expat`

Source:

```console
$ apt-get source -qq --print-uris jquery-tablesorter=1:2.31.3+dfsg1-3
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-tablesorter/jquery-tablesorter_2.31.3%2bdfsg1-3.dsc' jquery-tablesorter_2.31.3+dfsg1-3.dsc 2216 SHA512:73e765399f33230ca0bd120b4f81e547629f4f27dc985943862588a52e9baed45387766ef96d5ad8ea83c185b20a769a87b6be9e5885b7af2d2b637c91f39d49
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-tablesorter/jquery-tablesorter_2.31.3%2bdfsg1.orig.tar.xz' jquery-tablesorter_2.31.3+dfsg1.orig.tar.xz 582616 SHA512:2b66546aa1ec8ede9df6065ddb329f7e40f7d6e637a79f51bf28de3341e396edb0eee9fddaea9bd59645f7d8da06534ede7de65412a0029e45725fe171cd1b96
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-tablesorter/jquery-tablesorter_2.31.3%2bdfsg1-3.debian.tar.xz' jquery-tablesorter_2.31.3+dfsg1-3.debian.tar.xz 5556 SHA512:8eb41dc847dbacd85800ba52c3c859e227f10a948634c747547304c2dd4ea04051cd21bf5a88c7643b9f1f8087f8da5ac21b436c96638fe1a7ac0609161449d0
```

### `dpkg` source package: `jquery-throttle-debounce=1.1+dfsg.1-2`

Binary Packages:

- `libjs-jquery-throttle-debounce=1.1+dfsg.1-2`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-throttle-debounce/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris jquery-throttle-debounce=1.1+dfsg.1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-throttle-debounce/jquery-throttle-debounce_1.1%2bdfsg.1-2.dsc' jquery-throttle-debounce_1.1+dfsg.1-2.dsc 2093 SHA512:d0808d23d83b79c19bb5fec19618570d55aba9851395040ba18f875802ce60f3f9dc7a0eccde07a8fd6f16b0b829db15175bc221b8b598d539e71fcba143159b
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-throttle-debounce/jquery-throttle-debounce_1.1%2bdfsg.1.orig.tar.gz' jquery-throttle-debounce_1.1+dfsg.1.orig.tar.gz 16990 SHA512:b1c3b812e96c01e74f86ac048125baf954f5aabe15bbd868e90fd9bf69f569e51eb6ef88e2c143bdd64292231069b6be53d338f8c07a5cff3889106fe6eaa565
'http://archive.ubuntu.com/ubuntu/pool/universe/j/jquery-throttle-debounce/jquery-throttle-debounce_1.1%2bdfsg.1-2.debian.tar.xz' jquery-throttle-debounce_1.1+dfsg.1-2.debian.tar.xz 6096 SHA512:e2f06194a327aa5c8fb02047ff694908f03f592fbe22549f9e8a9a57b4fbffb5b18aea58492facbb75c2a7fda792df2939435f827a64b2d1f3011b44c76d8602
```

### `dpkg` source package: `keyutils=1.6.1-2ubuntu2`

Binary Packages:

- `libkeyutils1:amd64=1.6.1-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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


### `dpkg` source package: `lapack=3.10.0-2ubuntu1`

Binary Packages:

- `libblas3:amd64=3.10.0-2ubuntu1`
- `liblapack3:amd64=3.10.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.10.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.10.0-2ubuntu1.dsc' lapack_3.10.0-2ubuntu1.dsc 3474 SHA512:2bdbf698a2ae59dc09b752a20e7b4dfe1c25bd6dc255a36e7fa763d38cb2555eb56a51317867c3a99c09438d038822eeaa933b03b37b836c63fa602a5893b8ae
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.10.0.orig.tar.gz' lapack_3.10.0.orig.tar.gz 7630775 SHA512:56055000c241bab8f318ebd79249ea012c33be0c4c3eca6a78e247f35ad9e8088f46605a0ba52fd5ad3e7898be3b7bc6c50ceb3af327c4986a266b06fe768cbf
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.10.0-2ubuntu1.debian.tar.xz' lapack_3.10.0-2ubuntu1.debian.tar.xz 29040 SHA512:192a9ec75107c5427bd6f2d35e4785034666ba635eb6129f926aaa1663939b625f2800b6acaf686faf69cf21fb8f4201733e5515511e203895300e25675afb78
```

### `dpkg` source package: `libarchive=3.5.2-1ubuntu1`

Binary Packages:

- `libarchive13:amd64=3.5.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libarchive13/copyright`)

- `Apache-2.0`
- `BSD-1-clause-UCB`
- `BSD-124-clause-UCB`
- `BSD-2-clause`
- `BSD-3-clause-UCB`
- `BSD-4-clause-UCB`
- `Expat`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris libarchive=3.5.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.5.2-1ubuntu1.dsc' libarchive_3.5.2-1ubuntu1.dsc 2615 SHA512:7665e45376861ca611a3dc1206b4a541911bb0c2415fabc3df9c3f0775e4430d4cd8e2a2d45ba858c47ddaf80c804dd531a1dc67df24cef39f163105a4846978
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.5.2.orig.tar.xz' libarchive_3.5.2.orig.tar.xz 4905416 SHA512:ac7c47f9ddfe5d4d5db6ca9c1bcba788af95662bf0e54ca5426fe66cd8262896e12acc426eecdf0e0d6681c180bcd37f4c4469619273607e95399c7f49b61c7c
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.5.2.orig.tar.xz.asc' libarchive_3.5.2.orig.tar.xz.asc 833 SHA512:f2e12493106bf613857e83908d742dc287c5ffc451a2c4348749acf9cf8e947157e330cbfa9a031b0121ee6552b9145948fd40a9fdd412a34bdae95883663e88
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.5.2-1ubuntu1.debian.tar.xz' libarchive_3.5.2-1ubuntu1.debian.tar.xz 30964 SHA512:97996d18a4a3f94969b20e54a4b237edbe1d5afd8cf6c3e651f06513ca6d9089fe895de7837f6038bb6230628c17353211b288ea6bbf3044768cbdc23ba83000
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

### `dpkg` source package: `libdeflate=1.10-1ubuntu1`

Binary Packages:

- `libdeflate0:amd64=1.10-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.10-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.10-1ubuntu1.dsc' libdeflate_1.10-1ubuntu1.dsc 2288 SHA512:a73e1eb55ea6e0cb3b13b92a875418c14fcd8388e3dbeb4fa86fd69c185ad4eb335bc51775256d88a484fc87128225bfda02fc866b34700aa742e9c91a7570bd
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.10.orig.tar.gz' libdeflate_1.10.orig.tar.gz 158379 SHA512:2b59cc170c7fb3bb13bd3c6853070ea24fb9e6844dde4d08e43a8a5f8745ecbf844952390ff758070c6fc4f17d9eec8c4d2a729922bf84e2eaa9e74f1424e241
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.10-1ubuntu1.debian.tar.xz' libdeflate_1.10-1ubuntu1.debian.tar.xz 5000 SHA512:b091e61750eedf1d71a02c39a520065ee3213c676d0fa9439d1bb516b06cedb836bc95be71e26ce821fc3336c33083ad80433824580eaaa6ad40467beca44a7b
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

### `dpkg` source package: `libgd2=2.3.0-2ubuntu2`

Binary Packages:

- `libgd3:amd64=2.3.0-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgd3/copyright`)

- `BSD-3-clause`
- `GAP~Makefile.in`
- `GAP~configure`
- `GD`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `HPND`
- `MIT`
- `WEBP`
- `XFIG`

Source:

```console
$ apt-get source -qq --print-uris libgd2=2.3.0-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgd2/libgd2_2.3.0-2ubuntu2.dsc' libgd2_2.3.0-2ubuntu2.dsc 2318 SHA512:96c030bf2491b412fa423cbac1b2f2d3ace638a99c66ea8e7f55cd1c409d1fa5999a7fd02968949eb56fb8b28dc03d61e4464d0de13a5ef7428051b133ccc235
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgd2/libgd2_2.3.0.orig.tar.gz' libgd2_2.3.0.orig.tar.gz 3102749 SHA512:1ffdbe41f24fcdb22f5b195b8f1a22650a3dc30a798c23a7ee1a93acfdb70c2608d97ff908a01246ad44e1cfc13dbd20cc006d7a25b882907489daa1880db30b
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgd2/libgd2_2.3.0-2ubuntu2.debian.tar.xz' libgd2_2.3.0-2ubuntu2.debian.tar.xz 34548 SHA512:992da1a98982cca39cd6df17c963b4f4e169d99a9331c74ad5f02eb80371c909b51d83c7362df96ed41cc2206ff478bd705f2d983de90456c8560601aaa25732
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

### `dpkg` source package: `libice=2:1.0.10-1build1`

Binary Packages:

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

### `dpkg` source package: `libjpeg-turbo=2.1.2-0ubuntu1`

Binary Packages:

- `libjpeg-turbo8:amd64=2.1.2-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.1.2-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2-0ubuntu1.dsc' libjpeg-turbo_2.1.2-0ubuntu1.dsc 1690 SHA512:401a75e62575352db079bd268f00f94c8ea1e8e6c38bda852628729e6dfd3135804e3c9ee5b18b1254fed827e6073b0078553bcbc2c1df30d628bbb717a5ed47
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2.orig.tar.gz' libjpeg-turbo_2.1.2.orig.tar.gz 2257645 SHA512:172c3d8bdad62c32c4560754422fb36f0e80c8316e44d08708f0cba8ee9fd0830f5295d380de34d0f90ec07df6ab4dbe2f0c8451bc60553371c022c9077447c2
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.2-0ubuntu1.debian.tar.xz' libjpeg-turbo_2.1.2-0ubuntu1.debian.tar.xz 17240 SHA512:5cfc1e73012f3251e385f0288dece2e3862977fb3975c61c344afc464a2fd329c3fa027fc07edc40097afaad052bdf6f0dad55c665c20ccdde9f2231ec191410
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu8`

Binary Packages:

- `libjpeg8:amd64=8c-2ubuntu8`

Licenses: (parsed from: `/usr/share/doc/libjpeg8/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg8-empty=8c-2ubuntu8
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.dsc' libjpeg8-empty_8c-2ubuntu8.dsc 1637 SHA512:294caa2f8c916f07fa653469c239f46304cabd9d0194c7f0b311027bf2b09d45e07d6b5bc7bbdd11920e574040ad2b45f3af092d90009a119916a4a4857e0dd6
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.tar.gz' libjpeg8-empty_8c-2ubuntu8.tar.gz 1770 SHA512:07407b8f295f07df0eff6a4384cba7bc11349a1cacf488422b6a20bcbe5cb0ef9809bf847f3e52304a8f092e3581ac40adb745d9281fd4c83edd79f4c7cc8111
```

### `dpkg` source package: `libjs-jquery-hotkeys=0~20130707+git2d51e3a9+dfsg-2ubuntu1`

Binary Packages:

- `libjs-jquery-hotkeys=0~20130707+git2d51e3a9+dfsg-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-hotkeys/copyright`)

- `GPL-2`
- `MIT-or-GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libjs-jquery-hotkeys=0~20130707+git2d51e3a9+dfsg-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-hotkeys/libjs-jquery-hotkeys_0%7e20130707%2bgit2d51e3a9%2bdfsg-2ubuntu1.dsc' libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg-2ubuntu1.dsc 1658 SHA512:befc3d91889f52440ae93f9d5c9bc318970c13cc5cf54b205b83121d599e10bf8fad528b0f86fef9d8c2df73a02cab53925e89598b074a2eb294f6cd32e7dea8
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-hotkeys/libjs-jquery-hotkeys_0%7e20130707%2bgit2d51e3a9%2bdfsg.orig.tar.xz' libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg.orig.tar.xz 8604 SHA512:51a56b1ca9d72c32c04f8adad00c3f8c79c869d24651fe1f29e01666788375c536d59e2f5bc1e739ba50ecaa2a1454d4bc64ca1b2b32a84c60f768f379a811ad
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-hotkeys/libjs-jquery-hotkeys_0%7e20130707%2bgit2d51e3a9%2bdfsg-2ubuntu1.debian.tar.gz' libjs-jquery-hotkeys_0~20130707+git2d51e3a9+dfsg-2ubuntu1.debian.tar.gz 4768 SHA512:cb386d47415e1b1c394e0fbdc90662e2e5de6ba7d017cdc23bf219c1b85f2a0d5bae327fac4e68dd9f94988a2c5231a161b558f49e8b7b758e51f97832732263
```

### `dpkg` source package: `libjs-jquery-isonscreen=1.2.0-1.1`

Binary Packages:

- `libjs-jquery-isonscreen=1.2.0-1.1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery-isonscreen/copyright`)

- `GPL-2`
- `MIT-or-GPL`

Source:

```console
$ apt-get source -qq --print-uris libjs-jquery-isonscreen=1.2.0-1.1
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-isonscreen/libjs-jquery-isonscreen_1.2.0-1.1.dsc' libjs-jquery-isonscreen_1.2.0-1.1.dsc 2110 SHA512:20d5b9e33600d84743a413a7eb6950ea2e5d79fa99bc290fe7ab2bfc2f4d56775566d619647e84246fd7a43e2dc4dc541db4cdf27eae797eae1744302ea97799
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-isonscreen/libjs-jquery-isonscreen_1.2.0.orig.tar.gz' libjs-jquery-isonscreen_1.2.0.orig.tar.gz 727 SHA512:ea375b421f58dc789f7a8481ee6ef1504c3c23946e768e7566eb99a9b9b18d04e1a0ab3f439ea1f845e0f34198bec73d0b8c387ae36545f0c1de5aabf27039c4
'http://archive.ubuntu.com/ubuntu/pool/universe/libj/libjs-jquery-isonscreen/libjs-jquery-isonscreen_1.2.0-1.1.debian.tar.xz' libjs-jquery-isonscreen_1.2.0-1.1.debian.tar.xz 2228 SHA512:383257dc57d5a96d79d846f94bd251605df361d743754c2ff2cc7b004b2f4c69e0e3204d988bf034da8c9e020fb85799c65ecaa08450319d10ba8a661d106c78
```

### `dpkg` source package: `libjsoncpp=1.9.5-3`

Binary Packages:

- `libjsoncpp25:amd64=1.9.5-3`

Licenses: (parsed from: `/usr/share/doc/libjsoncpp25/copyright`)

- `Expat_or_PublicDomain_or_DualExpatPD`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libjsoncpp=1.9.5-3
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.9.5-3.dsc' libjsoncpp_1.9.5-3.dsc 1955 SHA512:5155ccae080c0c52c9cffeef244c5692c265c68d676822eeeac0ef6a316df23cd694b1e380d2b2fa562333b47a39c650daee8de61b5ca501d0a784c97dbdd461
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.9.5.orig.tar.gz' libjsoncpp_1.9.5.orig.tar.gz 216055 SHA512:1d06e044759b1e1a4cc4960189dd7e001a0a4389d7239a6d59295af995a553518e4e0337b4b4b817e70da5d9731a4c98655af90791b6287870b5ff8d73ad8873
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.9.5-3.debian.tar.xz' libjsoncpp_1.9.5-3.debian.tar.xz 7268 SHA512:5a5c8370ad816b654c1341b68399b4730b7afc1a814e79c7fd3a3b04c869aa44d24167bff43a6d1022c16ccc10550f73d7163c02879555548f47f2efd62eb166
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

- `libpng16-16:amd64=1.6.37-3build4`

Licenses: (parsed from: `/usr/share/doc/libpng16-16/copyright`)

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

### `dpkg` source package: `libsm=2:1.2.3-1build1`

Binary Packages:

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

### `dpkg` source package: `libthai=0.1.29-1`

Binary Packages:

- `libthai-data=0.1.29-1`
- `libthai0:amd64=0.1.29-1`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.29-1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.29-1.dsc' libthai_0.1.29-1.dsc 2325 SHA512:1e422a9502736b1716a2087d8f60c966186a29efa7429b16be728a7d3c1b4776436c3da9eccff3351026274ba2baaf0be11dca0272667990a2cb5945bcc1befb
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.29.orig.tar.xz' libthai_0.1.29.orig.tar.xz 417728 SHA512:0ba1261581a1705a2a2546a3071acb3c63892dbf111f0dad415667165a6b9542a5e4549061c67b11ec53de7c9e70fceb3c04d794fd12a22d991a539dbacebda1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.29-1.debian.tar.xz' libthai_0.1.29-1.debian.tar.xz 12564 SHA512:aef4cdb9ddd34db56a36ab3b6510d7d878c5d9b8fb856ba6960ba91e2fe003b63e04a4bcd212c3da988369be54fd46da257b9e5a0543e50c242d027eac452ba9
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

### `dpkg` source package: `libtool=2.4.6-15build1`

Binary Packages:

- `libltdl7:amd64=2.4.6-15build1`

Licenses: (parsed from: `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-15build1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-15build1.dsc' libtool_2.4.6-15build1.dsc 2551 SHA512:e63a3cf3be608d0865163dccc469399fe02970fa33f1481d901b0ef46949f40e357826d8813146c4d41167ca8e8fcecfed2c06cba15dd66729a7d75bf0e8b9c0
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA512:a6eef35f3cbccf2c9e2667f44a476ebc80ab888725eb768e91a3a6c33b8c931afc46eb23efaee76c8696d3e4eed74ab1c71157bcb924f38ee912c8a90a6521a4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA512:2f26447a837e3242b8f8f38fbab22d89df0949ee62fd966af3b5bae3aa939ba53bc4621174ee58d1c6722d569d7fe5f90097ddccffed28c3067fe5fa996fcb89
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-15build1.debian.tar.xz' libtool_2.4.6-15build1.debian.tar.xz 53984 SHA512:a2fd734c11504fb8e1631cff2bd2554cedaa60f93432e8e8b3dd62dddb752fb4632b7dac05e26726fd493ba7307bf2ff6caa49f0ea4d90ffb1f1d9d8549e8f3e
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


### `dpkg` source package: `libuv1=1.43.0-1`

Binary Packages:

- `libuv1:amd64=1.43.0-1`

Licenses: (parsed from: `/usr/share/doc/libuv1/copyright`)

- `Apache-2.0`
- `BSD-1-clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `CC-BY-4.0`
- `Expat`
- `GPL3+ with autoconf exception`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris libuv1=1.43.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.43.0-1.dsc' libuv1_1.43.0-1.dsc 1997 SHA512:d7d3d53b1eb5e5c8a02f40c222bc94741911f9a0d335f659122f4194f6a48fbfb20e4e2a0aa1b098454596a2d3c5a61d9740895ceda1a70dd12066fa6edd6dec
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.43.0.orig.tar.gz' libuv1_1.43.0.orig.tar.gz 1296029 SHA512:5a000b5a57efa03218cb8cc8deac91a8371f472452f48fef7d15c8d03ea0d98a966feba1ad9f2bf00f03635563663562dbd6d0cd2018e4d6c9783e64c2b3cd92
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.43.0-1.debian.tar.xz' libuv1_1.43.0-1.debian.tar.xz 20804 SHA512:fe334cabb50b40af716759bdcf08c414a4f206817a1438e23eb615ee7444dc401fa342e9995c2bb8f153e2a6ed0361de7929dd36a86c499f8ee0bd858f955c10
```

### `dpkg` source package: `libwebp=0.6.1-2.1build1`

Binary Packages:

- `libwebp6:amd64=0.6.1-2.1build1`

Licenses: (parsed from: `/usr/share/doc/libwebp6/copyright`)

- `Apache-2.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libwebp=1.2.1-7`

Binary Packages:

- `libwebp7:amd64=1.2.1-7`

Licenses: (parsed from: `/usr/share/doc/libwebp7/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=1.2.1-7
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.1-7.dsc' libwebp_1.2.1-7.dsc 2065 SHA512:a25afc508417d4c9d6c155091a1fc2a728780d4beee4f431492e31ef03285241442eaa2c84f0558d043056c3936bb634ce5b87cd8dc6dd8f28ab94b6f63726b3
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.1.orig.tar.gz' libwebp_1.2.1.orig.tar.gz 4100806 SHA512:5208ac9532c89ea9fec01122cb307afacdbf5c501ed1c6056e9ffc98e2a3386e637224e0301da88ae3a32aa0c210364e1e4eac79487e465ef9e54eb9b1af80aa
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_1.2.1-7.debian.tar.xz' libwebp_1.2.1-7.debian.tar.xz 4976 SHA512:75ab1f808273488b40e898c17b39e808b58ede9ed0b8e36d5e458059196985b079344beb19f61ace09424fe43340f89cea05c229296ffc866844593a034a6d35
```

### `dpkg` source package: `libx11=2:1.7.2-2`

Binary Packages:

- `libx11-6:amd64=2:1.7.2-2`
- `libx11-data=2:1.7.2-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.7.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2-2.dsc' libx11_1.7.2-2.dsc 2539 SHA512:5f0068ff56cace2c4df810f70eba979dfe13978159830c2b37b3923b95599b8e318eb134a18f887e158a1ecf4d4a5535d75fdda985a519b04ca16866fadd8a1c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz' libx11_1.7.2.orig.tar.gz 3181228 SHA512:9828e63a2be4b74afa7ebd91373f293d564ee865e81c3b92020041353443ce858eb8712a19b26b3c6b22b016051336fa8dd7d74a02bdeaffbadcba3012d397fa
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2.orig.tar.gz.asc' libx11_1.7.2.orig.tar.gz.asc 833 SHA512:13e8c484fc45324445c6030d72383154c43aa2d4fe3e4741324bda1bcfbfd0db9f0ea16f649668460bdf7e3d5b7a175e0b0d74b44ee5d90f9e7a57cc86aeb423
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.7.2-2.diff.gz' libx11_1.7.2-2.diff.gz 78109 SHA512:2ae96182523a1899efe2c978d4a8613d0ff4cf2a775cdfc856d96b7f45b9328d2abd5ebcad52e5f50f633fb9e93f53dda8b7babe1165fa312ba58829db2f4ef2
```

### `dpkg` source package: `libxau=1:1.0.9-1build4`

Binary Packages:

- `libxau6:amd64=1:1.0.9-1build4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-1build4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-1build4.dsc' libxau_1.0.9-1build4.dsc 2311 SHA512:0db0bf09df58e632371630c65bf49ec84d334fb9bb44463e4e4c7accd1546933bc195e49db4d8725e87b09c7ec9247e0e236d47a1920776c230ae9ec6fba178e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA512:3b22f34a4e35d17421189df8ce3f858b0914aef0cea0b12689dd8576f14eb811e39d6e32384251573daa7e3daba400deea98e7c0e29b4105138cf82195d7f875
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz.asc' libxau_1.0.9.orig.tar.gz.asc 801 SHA512:e59b2944591499d0c0291a8d80ad8ee2cb13ee00c32b0d26c6af12a2bb96c947d4d15924ef15b377b8d7640b75b50f9b8127ba53c582090b3f73b7bcf9e00b01
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-1build4.diff.gz' libxau_1.0.9-1build4.diff.gz 10419 SHA512:ff15deb6aa33a4b586bc967c8f55a4f5e517a6799b1bb47ef40e4c6078295ddd6dfab1fcf97ccd97ebab04a7d08a30804d8a7647abd7116b0b626286afedb4b1
```

### `dpkg` source package: `libxaw=2:1.0.13-1.1build1`

Binary Packages:

- `libxaw7:amd64=2:1.0.13-1.1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxaw=2:1.0.13-1.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxaw/libxaw_1.0.13-1.1build1.dsc' libxaw_1.0.13-1.1build1.dsc 2267 SHA512:5863b4b9bf6bad2c7f00d3b66f42e5feedb0feaae4bb1f129e50f45dcdc61c20574f08f4995415751ab6fc606e32051ee509df3e4e5c17f9fcc0a23619d475ca
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxaw/libxaw_1.0.13.orig.tar.gz' libxaw_1.0.13.orig.tar.gz 848997 SHA512:aa4eef77066bc8b14f4db2c6d3de84c44c9987504bc7fc1de75e182d5b2f6a8514e83763f6ece42dfb0ccd6177553e8ea8709dd07bbb24ed0c50a33c4a58ccee
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxaw/libxaw_1.0.13-1.1build1.diff.gz' libxaw_1.0.13-1.1build1.diff.gz 12759 SHA512:1b489e7a4589f0ecbe2f8e193bebf27e491dff61b43b3400ea80d4909e70ef739a05348f9330df0426ca93ea40ab173a774d7db301470458ffae0ff80851d4f9
```

### `dpkg` source package: `libxcb=1.14-3ubuntu2`

Binary Packages:

- `libxcb-render0:amd64=1.14-3ubuntu2`
- `libxcb-shm0:amd64=1.14-3ubuntu2`
- `libxcb1:amd64=1.14-3ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-3ubuntu2.dsc' libxcb_1.14-3ubuntu2.dsc 5397 SHA512:a03c8bde0ea68ae9f9eb079002f83857e847aa17aa7b90a3531e0615fe5f99104a90d1147fdddbe1c8a644c9db28dfbed571707d5edac62e01b3708f87bac038
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA512:6114d8c233b42b56604787a0475e924143aa13f1d382e6029b2150a4360c12ce78073409f754fbb1e5d9f99fc26900c0a4c59e9cfbd4c3d0a3af0c1306e62da1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-3ubuntu2.diff.gz' libxcb_1.14-3ubuntu2.diff.gz 26982 SHA512:5a113c3e26d3af27137365cc14eaf2ebbbc9effeb1fa5cf926b1348ea1add0e8395ba28a4637003731e2df5b8c7f7394f9877bbf3de2eac0292f95a0960ee64a
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

### `dpkg` source package: `libxdmcp=1:1.1.3-0ubuntu4`

Binary Packages:

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

### `dpkg` source package: `libxext=2:1.3.4-1`

Binary Packages:

- `libxext6:amd64=2:1.3.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-1.dsc' libxext_1.3.4-1.dsc 2118 SHA512:ae528e9b8ca21b26fed28d2b035cfa52547248a869301668dadae4e7cfc8b2309d65697464356d6599d2a95742cc48b258a31d80cf468007e3c555e18c83fa3a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA512:4eebd639fd57cb9b84a1e17e368f82fbf3d9f021eef5ad3fe31dd128500db57862a82c1e0d214d447cb7641b2be3fd7e949ee1196f2a482793c6628fb1e5cd70
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-1.diff.gz' libxext_1.3.4-1.diff.gz 12509 SHA512:ed7e756706d0dc48b63185db8ab93ea3329a2b1a3d81cb6a79977d80fec60fccedeb58c91b02eeae61c0f9616c4762fcba804ee1381170c06660cd6cccb52784
```

### `dpkg` source package: `libxml2=2.9.12+dfsg-6`

Binary Packages:

- `libxml2:amd64=2.9.12+dfsg-6`
- `libxml2-utils=2.9.12+dfsg-6`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-utils/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.12+dfsg-6
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12%2bdfsg-6.dsc' libxml2_2.9.12+dfsg-6.dsc 2915 SHA512:6447187968c9c4d29005f9f5bc2e3be37a054e56a962a93906929fa28caf83cd3b16789b8fa4a3d860204a5f1c50c70b2a4d991ecd25880a985be4b1b2c8fdba
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12%2bdfsg.orig.tar.xz' libxml2_2.9.12+dfsg.orig.tar.xz 2535044 SHA512:08ffb640e5669b52b29817887d62ef698799570ee5757612826e00aa5237ebf16b13bf838c350aff0ac1081547458d6d1aa6473f3499db7bf87e1f6d39f76386
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12%2bdfsg-6.debian.tar.xz' libxml2_2.9.12+dfsg-6.debian.tar.xz 34004 SHA512:b2529075322a2ad775a95b82deb5ec553052a39e77101a493367b364fd8715d64b5245e223f39908e377ca7b011f93ad16fd4efb31486acf563ea6e267292aea
```

### `dpkg` source package: `libxmu=2:1.1.3-3`

Binary Packages:

- `libxmu6:amd64=2:1.1.3-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxmu=2:1.1.3-3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.3-3.dsc' libxmu_1.1.3-3.dsc 2165 SHA512:7868975bb24189125a57910121c07bfd40fcb57af86a61665d7480f34339c566f4684e1db849d4d589a0e01bb59925ee8de0089bff4df436502e714c3bcc1dec
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.3.orig.tar.gz' libxmu_1.1.3.orig.tar.gz 497343 SHA512:b92fb2e96519880e9f057ae4149bd1bd95584383c6224891f3d832d98ace9292269815fe51d06a4dfc257f51021c2f7367e2f529a7ebcc3dfc64f037720a1cb8
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxmu/libxmu_1.1.3-3.diff.gz' libxmu_1.1.3-3.diff.gz 8085 SHA512:afefb6de2e65cfd1174b58a25f4598966adc375378d6525b2ddac98dce20276ae9ce03b1eb14b3a3a186e2ce00b7d68133a2578048f2582c5bb7b6be42a16fa6
```

### `dpkg` source package: `libxpm=1:3.5.12-1build1`

Binary Packages:

- `libxpm4:amd64=1:3.5.12-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxpm=1:3.5.12-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.12-1build1.dsc' libxpm_3.5.12-1build1.dsc 2110 SHA512:2fc1e2bb53be19d592b3a4d5006e0ab7dfe290da289c3adda84c0dc4c3e2637f9777fcefeeb5f4da9b5f6751879809cf7f0ac0e4d69fc4e996cfb40e3be38285
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.12.orig.tar.gz' libxpm_3.5.12.orig.tar.gz 529302 SHA512:17169016efc1e139f079290b2369fd62df8617867d97d2f50940521951a50f173118143109f0d7c552de92913cefc5ccaeb52225ccdd9abc89b3b85d9b5669f7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.12-1build1.diff.gz' libxpm_3.5.12-1build1.diff.gz 9526 SHA512:4ee2d28342e188a16e1e5f1f675b94b55320b1f432ab96e219265a0aba265ad89462e0834f808d6a875fa4c2ebc3354f956d0e894374ef6e0c88809c552dbfe3
```

### `dpkg` source package: `libxrender=1:0.9.10-1build3`

Binary Packages:

- `libxrender1:amd64=1:0.9.10-1build3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1build3.dsc' libxrender_0.9.10-1build3.dsc 2113 SHA512:ed2c11b4b3a0f4b33163c71472acafee06a54e9abccd08a315a0a4d226ea83f192347a9d930b2fffbeb32468e79b7f491d8743136c1ea37b667383d663d6c2a3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA512:7768e62b500f468460f88f27bc1130170b204b478573d9e4406867e557b5638b7c1e21d88d51f9e774ce2344780a384e3c3be51421275d2ee880f9a978a3a232
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1build3.diff.gz' libxrender_0.9.10-1build3.diff.gz 15652 SHA512:27bbbe8a4843532ed927899a10d300d3807462a67f36c328028e10a8c9c823f6384d03c9b2f11e04feac04a7b7b6df083886198738eb10f98e10a4788c95d97a
```

### `dpkg` source package: `libxslt=1.1.34-4build1`

Binary Packages:

- `libxslt1.1:amd64=1.1.34-4build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.34-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4build1.dsc' libxslt_1.1.34-4build1.dsc 2424 SHA512:dd8461b5da0baf3dea91d4460bc26ee62d53d1a6408ea42afe75d2d6a4c695de680f1f1f54722fedc9db055d338548c539ea53a22b12ed4928228c998dd0f6e0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz' libxslt_1.1.34.orig.tar.gz 3552258 SHA512:1516a11ad608b04740674060d2c5d733b88889de5e413b9a4e8bf8d1a90d712149df6d2b1345b615f529d7c7d3fa6dae12e544da828b39c7d415e54c0ee0776b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34.orig.tar.gz.asc' libxslt_1.1.34.orig.tar.gz.asc 488 SHA512:9b155d4571daede99cdbf2813a85fb04812737b5e23d3f7c9840225b38f3dbf171623a21645daaee190e7ff9ba38bde932922e96a2a2312c203ffa9917c3baea
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.34-4build1.debian.tar.xz' libxslt_1.1.34-4build1.debian.tar.xz 21536 SHA512:68cdd09cf7e1d03857ae46dc37501abf414bc27ddc7fe0d1c9c6ffc0f31db16eb28e35765bcafe4e29162191971a39c340d4f0dea73292156e04b353a2cbcd2a
```

### `dpkg` source package: `libxt=1:1.2.1-1`

Binary Packages:

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

### `dpkg` source package: `libyaml=0.2.2-1build1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.2-1build1`
- `libyaml-dev:amd64=0.2.2-1build1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.2-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1build1.dsc' libyaml_0.2.2-1build1.dsc 2056 SHA512:ff5cd621e7cc371479e4f084b44b270e0c27755ac65c38f2d9ba21d096961e5a7257a83f2f9dfdac6eca3d2d7c71f323b72a7aab80fe4233d4d248f7e15e8138
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2.orig.tar.gz' libyaml_0.2.2.orig.tar.gz 602509 SHA512:0728c89ba43af3cdec22bccaf18c9ad7b07e13cdebed9d8919e2c62cf90bb5e23d2c746fd250320b2827dfcd9f1ce442d3bf8a3fe18b61f9a8d1d7770561e610
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1build1.debian.tar.xz' libyaml_0.2.2-1build1.debian.tar.xz 4200 SHA512:eab5f420c0b0b575658c0493fb34f257787248f6ee89a9d929a7066b1671dc5e3558fd526e0741bcc282d6b174463a39bb07d40f5b308654724099f26cb9b448
```

### `dpkg` source package: `libzstd=1.4.8+dfsg-3`

Binary Packages:

- `libzstd-dev:amd64=1.4.8+dfsg-3`
- `libzstd1:amd64=1.4.8+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libzstd-dev/copyright`, `/usr/share/doc/libzstd1/copyright`)

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

### `dpkg` source package: `linux=5.15.0-18.18`

Binary Packages:

- `linux-libc-dev:amd64=5.15.0-18.18`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris linux=5.15.0-18.18
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0-18.18.dsc' linux_5.15.0-18.18.dsc 7529 SHA512:82a0d705b6cc7ff641fa15a0c0af4d9749c0a04083b3a7a0eb879e6554a062cf3c7132f4cee5a519d7c76724e2331ea272d9057b0f859c66f8356cf7e020c396
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0.orig.tar.gz' linux_5.15.0.orig.tar.gz 194969557 SHA512:ae9a32132d5988441c189157703b0f8fa4e232d8d24f7104f944c06827db740beafae55eb37a51eb99b4ac513927cd372321fa1e84afff4d450b786e44414861
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0-18.18.diff.gz' linux_5.15.0-18.18.diff.gz 5064265 SHA512:b484854cb39f12b5441d09165e090839d3189e53cdc9e57519e14b5d80c5971d247e6e30a45d80981c503dd4c315508d4a7e0cf067bed86564597579c80b933f
```

### `dpkg` source package: `lsb=11.1.0ubuntu3`

Binary Packages:

- `lsb-base=11.1.0ubuntu3`
- `lsb-release=11.1.0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`, `/usr/share/doc/lsb-release/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu3.dsc' lsb_11.1.0ubuntu3.dsc 2218 SHA512:af52feb8995d853a0d5d9e1bffe7c86527a64d3adc1345f7800bbaaaaa41a50e5c76199a34c6e56f70b3c01c6d5466f5471ce2f97ddb338160f7ccc0cd851b3c
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu3.tar.xz' lsb_11.1.0ubuntu3.tar.xz 46076 SHA512:21c6b7774aab9fddf79bfa000d4d56ee8bbd7a9e0568e00876ba8adedc6c035530f48ed10ec9838420a6a97e877b6b36148e7e1b7eec9780852da85d22547150
```

### `dpkg` source package: `lto-disabled-list=22`

Binary Packages:

- `lto-disabled-list=22`

Licenses: (parsed from: `/usr/share/doc/lto-disabled-list/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lto-disabled-list=22
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_22.dsc' lto-disabled-list_22.dsc 1435 SHA512:69a298e39ab16ddfc0c25417c9c2e5e7e52e0c17d8c08489dc5aeaf110238aa81a7946ebceb35c77408ca868f677e4e2e0a91a52b9bb4080b49c27a7a46d9f68
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_22.tar.xz' lto-disabled-list_22.tar.xz 12332 SHA512:0e2221a84f149f36537017b1d15bfc548f6948b6959ec1e31b40b2093b7a209f44576a410a8b0875bfc9d92fc2f438e1fa7a90d51ba378b5244eee816a6c2805
```

### `dpkg` source package: `lxml=4.8.0-1`

Binary Packages:

- `python3-lxml:amd64=4.8.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-lxml/copyright`)

- `GPL`
- `GPL2`
- `later`

Source:

```console
$ apt-get source -qq --print-uris lxml=4.8.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lxml/lxml_4.8.0-1.dsc' lxml_4.8.0-1.dsc 1935 SHA512:4081d6a086a0eb681273f2e730a9df7a910445e7154c718dd149a8972fcf60ad96676d76e6227e70557be4db32a253f898248454b55e6337d9acc5ec5abf9a0b
'http://archive.ubuntu.com/ubuntu/pool/main/l/lxml/lxml_4.8.0.orig.tar.gz' lxml_4.8.0.orig.tar.gz 3209187 SHA512:f39e1a6194eb00045002ef830da18ad1be6307004f29e5266db4fbaecdb14be9142462a39bd55a2753c5e20a59cc104a09aa40ca18b0382ee421c2e67907a154
'http://archive.ubuntu.com/ubuntu/pool/main/l/lxml/lxml_4.8.0-1.debian.tar.xz' lxml_4.8.0-1.debian.tar.xz 8196 SHA512:9f617d2a282036a2f32132a6b5be3fb50e66023622c3b1e7c10bd048c93c27e620d49861abb00bfa9404cd3c679aca6e078cac31a1c8a798ff7e3e397612285b
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

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-3.dsc' mawk_1.3.4.20200120-3.dsc 1915 SHA512:f51dae1f342769e4fc0b8d5faf4e988433a0e74912ba0777fbafdf058900c973087c267756f5c2b74298bfc31a36c8bbc99c6c0edcc850710b646d0d24fa1305
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA512:14d9a6642ce931bf6457d248fc2d6da4f0ea7541976ca282ea708b26df048f86fdf92c27f72d497501ccd43a244d1d1a606f1a2f266a7558306fea35dcc3041b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-3.debian.tar.xz' mawk_1.3.4.20200120-3.debian.tar.xz 7520 SHA512:bc4f5401de313108595ba91b17f44b5c67d7650b5557eef8a6c63c75e2ccee5dfd8900576d7e81f0ab1ac2e570f64fa75f38f56f6d4535437c803029216501af
```

### `dpkg` source package: `media-types=5.0.0`

Binary Packages:

- `media-types=5.0.0`

Licenses: (parsed from: `/usr/share/doc/media-types/copyright`)

- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris media-types=5.0.0
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_5.0.0.dsc' media-types_5.0.0.dsc 1620 SHA512:9228fb18ad283c0d65ef5a0d2acc5a95531bd13c12efc0984d04747a4a3103c1a70cabb19044131113d34760ebd58630383162aeb8c241f0f13b6da3c383c3be
'http://archive.ubuntu.com/ubuntu/pool/main/m/media-types/media-types_5.0.0.tar.xz' media-types_5.0.0.tar.xz 55096 SHA512:2dee1394ce96a367a14b5d1ea0d902619c105a721e6159cc1c398a1cc410196dc4a51f6494ea05adb9f121b52e56b2c48543131cc64f23002cb2fe6b042e76cf
```

### `dpkg` source package: `more-itertools=8.10.0-2`

Binary Packages:

- `python3-more-itertools=8.10.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-more-itertools/copyright`)

- `MIT-style`

Source:

```console
$ apt-get source -qq --print-uris more-itertools=8.10.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/more-itertools/more-itertools_8.10.0-2.dsc' more-itertools_8.10.0-2.dsc 2092 SHA512:fd06076c1f50b266003b908f7bd2a264ccad75d888f0a1f505ff4ba8c2246c4f18108df2a44c6f0adcc74c444275743583b8009048b59525789edad16a2aa047
'http://archive.ubuntu.com/ubuntu/pool/main/m/more-itertools/more-itertools_8.10.0.orig.tar.gz' more-itertools_8.10.0.orig.tar.gz 102929 SHA512:a666710426a825e5aca10b52439a973e08ac6ec09fb5375426194d1342af055a8b6aee48b4e3fa17c4606d6d9cc3673afdd789dbbaf373258be6a71bd63178f7
'http://archive.ubuntu.com/ubuntu/pool/main/m/more-itertools/more-itertools_8.10.0-2.debian.tar.xz' more-itertools_8.10.0-2.debian.tar.xz 2812 SHA512:eaf36d67901a164947cf86f84a21d296f8f9012948bde9ea70390158d4ecbfe77687c119e1e18612dadd90d2142dbb5959663ace84b103715b4e4ca20ec130f6
```

### `dpkg` source package: `mpclib3=1.2.1-1`

Binary Packages:

- `libmpc3:amd64=1.2.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.1-1.dsc' mpclib3_1.2.1-1.dsc 1851 SHA512:b4f870146a79d8f5a552beb5c087dca3c2a190e20f80409f201037989a40b9e2a20a88e152d49bd1eca6fecd3af42f94d99e023648451feb45caaf42af7eb553
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.1.orig.tar.gz' mpclib3_1.2.1.orig.tar.gz 838731 SHA512:3279f813ab37f47fdcc800e4ac5f306417d07f539593ca715876e43e04896e1d5bceccfb288ef2908a3f24b760747d0dbd0392a24b9b341bc3e12082e5c836ee
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.1-1.diff.gz' mpclib3_1.2.1-1.diff.gz 4264 SHA512:59a27b8956ec776e5f6d3036f9d844fa09a1c1a8dcdeae5dd151e02fb2eb40e1a539b1acddef08a48a7ac78934e6b1c4f7acf675dafc910fda022e821ec8f95f
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

### `dpkg` source package: `mpfr4=4.1.0-3build2`

Binary Packages:

- `libmpfr6:amd64=4.1.0-3build2`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.1.0-3build2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3build2.dsc' mpfr4_4.1.0-3build2.dsc 1983 SHA512:1af1bccffee8e614c103aca656a441412f704872d621aed77c37787d1142ac87df949361a262c57348bebbf69d7cb42e4c5d445810721aae552da4f9f736d6c0
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA512:1bd1c349741a6529dfa53af4f0da8d49254b164ece8a46928cdb13a99460285622d57fe6f68cef19c6727b3f9daa25ddb3d7d65c201c8f387e421c7f7bee6273
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3build2.debian.tar.xz' mpfr4_4.1.0-3build2.debian.tar.xz 12464 SHA512:917ef63174e3d79f80ddfad15cdbdc7a904d8906bb385ad7fba74f9a2d44090635b98b0b36b9550bbe6b3cb1089dfc7253405a5c64544b794f9a653f562bfdd7
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

### `dpkg` source package: `netifaces=0.11.0-1`

Binary Packages:

- `python3-netifaces:amd64=0.11.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-netifaces/copyright`)

- `MIT-style`

Source:

```console
$ apt-get source -qq --print-uris netifaces=0.11.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.11.0-1.dsc' netifaces_0.11.0-1.dsc 2072 SHA512:19d4c9015a79ccdae53f827e45482beaeb92ab0c1b76994aacf727774e60b010d1a5d9b4587bfe7b95f09fad7385e6d2b54769a22d645d8bd28a74f0429faadb
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.11.0.orig.tar.gz' netifaces_0.11.0.orig.tar.gz 30106 SHA512:a53110efb78c89c4d72d002104866253a4c085dd27ff9f41d4cfe3811cc5619e7585ceda4e91e83cdd0645c40c745c61d205708ee9a34427b35f437a48f148e5
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.11.0-1.debian.tar.xz' netifaces_0.11.0-1.debian.tar.xz 3768 SHA512:43046e7ea67662e9d5d54323490c945ab51bb3383ab8352ed4556eca5295107b3644ab4ba08471a562403fff7a9c0c9e7de9c6db9927f7b65c52fc8e61e4ef52
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

### `dpkg` source package: `node-jquery=3.6.0+dfsg+~3.5.13-1`

Binary Packages:

- `libjs-jquery=3.6.0+dfsg+~3.5.13-1`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris node-jquery=3.6.0+dfsg+~3.5.13-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/node-jquery/node-jquery_3.6.0%2bdfsg%2b%7e3.5.13-1.dsc' node-jquery_3.6.0+dfsg+~3.5.13-1.dsc 2699 SHA512:44656f0d8cc8a3bc6ea06bbf8d55bf2a2fc4220ba39e170f4a80af49ee93910a5cc03fb355303c4f537d08bbcad857e5fb6e7946bffc684c2d5d5e63f23d1a70
'http://archive.ubuntu.com/ubuntu/pool/main/n/node-jquery/node-jquery_3.6.0%2bdfsg%2b%7e3.5.13.orig-types-jquery.tar.xz' node-jquery_3.6.0+dfsg+~3.5.13.orig-types-jquery.tar.xz 84372 SHA512:4abd8cc14201ec607cc7af01147944ea18c8b125e01efa34d4ca817ed0232b2eaf6a8edb8a1a511e4d8c447d75bb566dad005391cfdc963b903143906e42388c
'http://archive.ubuntu.com/ubuntu/pool/main/n/node-jquery/node-jquery_3.6.0%2bdfsg%2b%7e3.5.13.orig.tar.xz' node-jquery_3.6.0+dfsg+~3.5.13.orig.tar.xz 296988 SHA512:9ae8e2e726d88915de2e33530e60af4e33a9a48e9bc584fd490d8898af8260c13ba058d28375163fcbd46b96caa3e1f9bca8e4404c5b70166daed3afd440afc7
'http://archive.ubuntu.com/ubuntu/pool/main/n/node-jquery/node-jquery_3.6.0%2bdfsg%2b%7e3.5.13-1.debian.tar.xz' node-jquery_3.6.0+dfsg+~3.5.13-1.debian.tar.xz 6328 SHA512:48c5c5c31f6dbf6e20d3ac0b1c7d7ff2e63a2396d7288806b1c698261e7173219173ec410d34883c63ec17fe48c71872633bb6f9d50cf408a0cbaf3d8a5d54db
```

### `dpkg` source package: `nose2=0.9.2-1`

Binary Packages:

- `python3-nose2=0.9.2-1`

Licenses: (parsed from: `/usr/share/doc/python3-nose2/copyright`)

- `BSD-2-clause`
- `Python`

Source:

```console
$ apt-get source -qq --print-uris nose2=0.9.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose2/nose2_0.9.2-1.dsc' nose2_0.9.2-1.dsc 2240 SHA512:836f97319b8a20abfb157e937066d4d7d8365de962f5484f2093f1e76de9ca7bd6faa513003013c3bc74911dd53e5fd44e9fdc38a40a1cd645a556c0ce15dd8e
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose2/nose2_0.9.2.orig.tar.gz' nose2_0.9.2.orig.tar.gz 154695 SHA512:c1d8231decf4ab1712d7b486efcc4835df3c665d401713ac100186a513c68da4e9e1710f4289802fea1cfdbee1c5e3358c30a0e9d14554f408323efd00a1a293
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose2/nose2_0.9.2-1.debian.tar.xz' nose2_0.9.2-1.debian.tar.xz 8080 SHA512:f8183f995d7438caf496541053b3ede64cbdf979a51016a7e6303c62c86b1b3c145b9e857106cdea4c309a23577ca9a79cfd97c080eb5392e2515f479ae29934
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

### `dpkg` source package: `numpy=1:1.21.5-1`

Binary Packages:

- `python3-numpy=1:1.21.5-1`

Licenses: (parsed from: `/usr/share/doc/python3-numpy/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `MIT`
- `Public-Domain`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris numpy=1:1.21.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numpy/numpy_1.21.5-1.dsc' numpy_1.21.5-1.dsc 2884 SHA512:6c7fc3b09e04f4a28a6e8e5e38f2b3eb8915d2fdafd76b80d20a623888cae632d7e24e6b7f4a251033b9a023c93538eb4f9d446163608171f407d12b7bcb7109
'http://archive.ubuntu.com/ubuntu/pool/main/n/numpy/numpy_1.21.5.orig.tar.xz' numpy_1.21.5.orig.tar.xz 6601692 SHA512:4ed39a24758e12d23b1b2dbd32ac892be6ac7e1528f7cee24c34323962795b377dbb3f95660c2bf4be3cc8c093aafe49ace03ca2b9f72de0f2d2ce6aa784dfd1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numpy/numpy_1.21.5-1.debian.tar.xz' numpy_1.21.5-1.debian.tar.xz 30528 SHA512:2780a1e06814c5e0e67f6b62594c8fda3408f0abeeaf751794e48688bcd8f3f7dddbc42d46ef7e7a75ee0dfa1ab7a2a2c7cea0b1c63b529653d1b5d29fe8e615
```

### `dpkg` source package: `openldap=2.5.11+dfsg-1~exp1ubuntu1`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.11+dfsg-1~exp1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.11+dfsg-1~exp1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11%2bdfsg-1%7eexp1ubuntu1.dsc' openldap_2.5.11+dfsg-1~exp1ubuntu1.dsc 3298 SHA512:a807966ceeb7c66227e12c546c8d34929049e1c2126cd96e317dbc7a7e0f5288b414f759c3b8ac2076d5d23afc2a29bbd916d412f9510f2a286132513a30e19f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11%2bdfsg.orig.tar.gz' openldap_2.5.11+dfsg.orig.tar.gz 5609424 SHA512:a728d66c8a6bfa34d8e80eab86c2612685cab1358008cc10f9d9862a03aff46a5a19cd6487732131222efae6b86c27d5446fd829e89a4cadeb79161fd9ed437c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.11%2bdfsg-1%7eexp1ubuntu1.debian.tar.xz' openldap_2.5.11+dfsg-1~exp1ubuntu1.debian.tar.xz 170868 SHA512:d6dddb9d150085d8f7d8609253fa6dcda3e1cb4603d9c9d58ff08f6809ca8bdee48342042f35d5720aa46b52b078c6b29f4b834ec3e058fc1308d77bae0dddaa
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pango1.0=1.50.4+ds-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.50.4+ds-1`
- `libpangocairo-1.0-0:amd64=1.50.4+ds-1`
- `libpangoft2-1.0-0:amd64=1.50.4+ds-1`

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
$ apt-get source -qq --print-uris pango1.0=1.50.4+ds-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.4%2bds-1.dsc' pango1.0_1.50.4+ds-1.dsc 3780 SHA512:306853bf1dc3b7842e0e53ae8235f9ed340140d0d1467ca7742fb973745bae6e029d7f45a8b4b32419386422b7f9d46316ac109cc573de3373f486f2a51d2cb5
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.4%2bds.orig.tar.xz' pango1.0_1.50.4+ds.orig.tar.xz 2671076 SHA512:ce2d53c94cf601d42ba46631de804c3ae18ef261c5e268a1056d0d88d815ca92a0c571ef566853c778663ae31683326acc974e911da0c5163692539f2d47072e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.50.4%2bds-1.debian.tar.xz' pango1.0_1.50.4+ds-1.debian.tar.xz 50252 SHA512:ba981828102acec1bc48a113b7b86e93be21ef8e81cdae1beb2de528515df70a0f0e5ba101a179f68e634242df228068154ea43f12645141fa852be96baabad2
```

### `dpkg` source package: `patch=2.7.6-7build1`

Binary Packages:

- `patch=2.7.6-7build1`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-7build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7build1.dsc' patch_2.7.6-7build1.dsc 1755 SHA512:5d37e8129c0f89bd7b3af269a98c60e82602f048617bbe6b2be3eee5ec4cf7c00eaa81be4e171f8e6cceff0d2cb4d53c4941bcc6c911669682b1bc1573c7addf
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA512:fcca87bdb67a88685a8a25597f9e015f5e60197b9a269fa350ae35a7991ed8da553939b4bbc7f7d3cfd863c67142af403b04165633acbce4339056a905e87fbd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-7build1.debian.tar.xz' patch_2.7.6-7build1.debian.tar.xz 15152 SHA512:eee477d3956d2708076a60c28aa1c75e835c850f280745e283f4a03f9caa65d1d0956f056ec95e405206ff186602dcc4c5fb8d34d8f3f8bf82d87eb69935c4cb
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

### `dpkg` source package: `pixman=0.40.0-1build3`

Binary Packages:

- `libpixman-1-0:amd64=0.40.0-1build3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.40.0-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0-1build3.dsc' pixman_0.40.0-1build3.dsc 2070 SHA512:ac9a676db82b531dc8aec8d9620a4ca1702e44b08100a729becebbfd66eb652c712bdd367cbc8bb6e6abaf0b801a0e0e78498bb26d0f86e9b165de692cf64243
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0.orig.tar.gz' pixman_0.40.0.orig.tar.gz 913976 SHA512:063776e132f5d59a6d3f94497da41d6fc1c7dca0d269149c78247f0e0d7f520a25208d908cf5e421d1564889a91da44267b12d61c0bd7934cd54261729a7de5f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.40.0-1build3.diff.gz' pixman_0.40.0-1build3.diff.gz 319556 SHA512:863b9aac7163073197ca4301ba26b037c4fee0c8e143b3fae8c229453aee6df0f055c4a7aaebc65f674624ce5d5fca3ceaff00baa0e79677db47f7e0a963b375
```

### `dpkg` source package: `pkg-config=0.29.2-1ubuntu2`

Binary Packages:

- `pkg-config=0.29.2-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.2-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu2.dsc' pkg-config_0.29.2-1ubuntu2.dsc 1824 SHA512:3397d8821327d4dfda0388b2d89c494cd11bbaadf9522d737d36bb3cc63a76904f74a8e4d36a47a901f8e9f3c23217fcf968c3304b59cb4a80d0f62b74ea94f4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2.orig.tar.gz' pkg-config_0.29.2.orig.tar.gz 2016830 SHA512:4861ec6428fead416f5cbbbb0bbad10b9152967e481d4b0ff2eb396a9f297f552984c9bb72f6864a37dcd8fca1d9ccceda3ef18d8f121938dbe4fdf2b870fe75
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.2-1ubuntu2.diff.gz' pkg-config_0.29.2-1ubuntu2.diff.gz 9896 SHA512:ce399a8cb8f4572349931efaa38f7616a5b491813ad47acf3a41dca2412d6ce3be42c208e54731f8b3cb21e8d9219bc838d1e0a07083c35dcd980b99d92ebc0e
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pybind11=2.7.1-2`

Binary Packages:

- `pybind11-dev=2.7.1-2`

Licenses: (parsed from: `/usr/share/doc/pybind11-dev/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `BSD-3-Clause+CLA`

Source:

```console
$ apt-get source -qq --print-uris pybind11=2.7.1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pybind11/pybind11_2.7.1-2.dsc' pybind11_2.7.1-2.dsc 2629 SHA512:7de9e7b0410ce6177a95edee1289c540f7a8cce1e350ee56d2cd56d5514f238ebc26523fc8db846dadefda5d1643ce0b5a5dea541cb4c4c781d709b96c759c16
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pybind11/pybind11_2.7.1.orig.tar.gz' pybind11_2.7.1.orig.tar.gz 668217 SHA512:f09f46622b394d3990ab82aa7ea15a06e298df109cd2df263ba9d6ac7fb248217df7450e1954a9679a8360335d5bbf662926a34c8b7c61b6e4c396bbdfd88305
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pybind11/pybind11_2.7.1-2.debian.tar.xz' pybind11_2.7.1-2.debian.tar.xz 68228 SHA512:1b51115c73bd1f95f426ecf7043e3bef7e09ebcfd2619ed1eeaf85915f83940f8d0242f5c0ad8a658ce2a56768537128815fc8b9a1c5791fd41e284fc1ba0313
```

### `dpkg` source package: `pycodestyle=2.8.0-2`

Binary Packages:

- `python3-pycodestyle=2.8.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-pycodestyle/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris pycodestyle=2.8.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pycodestyle/pycodestyle_2.8.0-2.dsc' pycodestyle_2.8.0-2.dsc 2107 SHA512:a3695577354afe0608d53182cee03d04af0957be6803f655abd6f737bfaf9e84688544f55391ca92596f62838895656e1d4185e4a49066ff2e5252310bb72171
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pycodestyle/pycodestyle_2.8.0.orig.tar.gz' pycodestyle_2.8.0.orig.tar.gz 102299 SHA512:0098be44451bc173507e2b396aaf342ccf7f25a6a1f5d5c1f802079a76a66e6bedf9f358b5e07b27bee66e3b279c72a6b72f63e5984f58ae83b7fc5806880fc1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pycodestyle/pycodestyle_2.8.0-2.debian.tar.xz' pycodestyle_2.8.0-2.debian.tar.xz 4396 SHA512:e4b90d970bb414c648a75b491b4cbd7768484bcaea2226f66cae2fad15409533cb74118e71807c4cb9ca57fcad4328153cb91215ee92e6e14cfff797e03b7e27
```

### `dpkg` source package: `pydocstyle=6.1.1-1`

Binary Packages:

- `pydocstyle=6.1.1-1`
- `python3-pydocstyle=6.1.1-1`

Licenses: (parsed from: `/usr/share/doc/pydocstyle/copyright`, `/usr/share/doc/python3-pydocstyle/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris pydocstyle=6.1.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pydocstyle/pydocstyle_6.1.1-1.dsc' pydocstyle_6.1.1-1.dsc 2218 SHA512:591881af9df84bdfe71c2743ad87b810eb08007f652a518557413afd6ab78c51e31341660093a856a3f297e575197dfc099cc1d33efbd377f7e846b9ec6fc3d1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pydocstyle/pydocstyle_6.1.1.orig.tar.gz' pydocstyle_6.1.1.orig.tar.gz 73982 SHA512:ce4932a6601c80d05a46600f5af7df54798025a5f3dc41ab8cf1bc0d63e7f78b70cccb17dc99ddab25eda9abd639f91468fca1b1ceb4539708350212e481a156
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pydocstyle/pydocstyle_6.1.1-1.debian.tar.xz' pydocstyle_6.1.1-1.debian.tar.xz 4364 SHA512:0b1e373513a34ece07e6a5e9a48c0ce6b6f780af6da4968361ae7f51bf864b7e7f9de955cebb1433e1409cb1025936fcc4ffff160c900558bb1a9ef61a1941fc
```

### `dpkg` source package: `pyflakes=2.4.0-2`

Binary Packages:

- `python3-pyflakes=2.4.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-pyflakes/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris pyflakes=2.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pyflakes/pyflakes_2.4.0-2.dsc' pyflakes_2.4.0-2.dsc 2121 SHA512:8dcf8aafca83b10ad3efbd5b4d057e66057641b5640960ffa3cb632b8954830d297abe7f4587e2a6853de283c5a90412589d0003f219549d01650eee2abffd31
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pyflakes/pyflakes_2.4.0.orig.tar.gz' pyflakes_2.4.0.orig.tar.gz 69101 SHA512:f4c6512eb811511c897623f52c4f88e50275a3292582d7dd34462e90e39fecce939818cb92e750eebdd66eab25b91c23540104fc4530c42621d7cfeb1d33c577
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pyflakes/pyflakes_2.4.0-2.debian.tar.xz' pyflakes_2.4.0-2.debian.tar.xz 7748 SHA512:f692ff23a68f9e5389c1df6ed8f628159fbc7fbdd375c4ed48291271ab524a6c4d6dd2c20e0291fb81fb0cb99f63ab4f5c798cc9c6133b236e97de339e5224c6
```

### `dpkg` source package: `pygments=2.10.0+dfsg-1`

Binary Packages:

- `python3-pygments=2.10.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/python3-pygments/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `ISO-1986`

Source:

```console
$ apt-get source -qq --print-uris pygments=2.10.0+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pygments/pygments_2.10.0%2bdfsg-1.dsc' pygments_2.10.0+dfsg-1.dsc 2245 SHA512:980c6f30784ca468ecf91972aa698846939905caedee335e35b810b735a6421239f771f73ea758a55a99d80098201f45ceb571637f16f76ab09652de22bf4481
'http://archive.ubuntu.com/ubuntu/pool/main/p/pygments/pygments_2.10.0%2bdfsg.orig.tar.xz' pygments_2.10.0+dfsg.orig.tar.xz 1046728 SHA512:33b3415e39f926bf35d1265d8f19bf1355b9e1547241e5ddde081e47d281380bdfa83c25db28da5ea4256fec6ed45a5fa7920758db0f9f0e8c6142ee260f32b9
'http://archive.ubuntu.com/ubuntu/pool/main/p/pygments/pygments_2.10.0%2bdfsg-1.debian.tar.xz' pygments_2.10.0+dfsg-1.debian.tar.xz 8180 SHA512:92f483f739cafe28e5aad3a439d1582fb1471840ad8f026324828f40364d05fb27dcc2d1f862cd2f322d29826a3ec60f49845d4baab5bcb647be4bccd588c791
```

### `dpkg` source package: `pyparsing=2.4.7-1`

Binary Packages:

- `python3-pyparsing=2.4.7-1`

Licenses: (parsed from: `/usr/share/doc/python3-pyparsing/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-3`
- `ellis-and-grant`
- `salvolainen`

Source:

```console
$ apt-get source -qq --print-uris pyparsing=2.4.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.4.7-1.dsc' pyparsing_2.4.7-1.dsc 2340 SHA512:6d06384fcf48257fafbaa9681faee68ba044f117fd86f2ad6c57ef8fa7186066376c5b25fc525f057cdd8fa2830289f77780c9a8f9647164596cd490b3c8014e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.4.7.orig.tar.gz' pyparsing_2.4.7.orig.tar.gz 649718 SHA512:0b9f8f18907f65cb3af1b48ed57989e183f28d71646f2b2f820e772476f596ca15ee1a689f3042f18458206457f4683d10daa6e73dfd3ae82d5e4405882f9dd2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.4.7-1.debian.tar.xz' pyparsing_2.4.7-1.debian.tar.xz 7764 SHA512:185911863111ba7c956fb1e7229046ae1516554bc253f342f070afe82c20cfd4c3e098d233c7b341f6518875e47ddcf76ded2528534a959574beebcdf531b846
```

### `dpkg` source package: `pytest=6.2.5-1ubuntu2`

Binary Packages:

- `python3-pytest=6.2.5-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/python3-pytest/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris pytest=6.2.5-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pytest/pytest_6.2.5-1ubuntu2.dsc' pytest_6.2.5-1ubuntu2.dsc 2936 SHA512:4f30f7c8f53c6d899e802992a9f248c42d4eb250509425ef40b9e2d2cbeeda5a1cc59a03be364befa2d489a2faab31cceb10b4020576d7107579bcba2e3bef5d
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pytest/pytest_6.2.5.orig.tar.xz' pytest_6.2.5.orig.tar.xz 883896 SHA512:2f7dd16cdb0e836fb06fd70b827b9616450e0ce3056b4b6deb3e5b6e1d38b99c03e87981ecb352de452c578a17d895e1df5f52c26c719952003ff3d8e1fa8308
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pytest/pytest_6.2.5-1ubuntu2.debian.tar.xz' pytest_6.2.5-1ubuntu2.debian.tar.xz 11340 SHA512:ca468310e87ca57fddfe9199e54af29f695590e13ed259e2c04c9bc79bab173eec3e0d322962a937a119532f39d697f3a8f39954282ec8775070c0bed4c52685
```

### `dpkg` source package: `python-argcomplete=1.8.1-1.5`

Binary Packages:

- `python3-argcomplete=1.8.1-1.5`

Licenses: (parsed from: `/usr/share/doc/python3-argcomplete/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris python-argcomplete=1.8.1-1.5
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-argcomplete/python-argcomplete_1.8.1-1.5.dsc' python-argcomplete_1.8.1-1.5.dsc 2052 SHA512:c2d58d5afee56c25e44593beb84ffec2cb86d9b4e55bd121e47719b9ef14702c782bdc33bec519f867713ca336efda0949ce66e1cb62d909b50fa6df988b742d
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-argcomplete/python-argcomplete_1.8.1.orig.tar.gz' python-argcomplete_1.8.1.orig.tar.gz 53282 SHA512:836fc44a2252c626606378a410ddad8b21ac8c09d2049cadade7edc01fa13b1b92441b783cc1f356e4bc8bbe7640cd2ca262d4396d9f088ea2c28659124e51e9
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-argcomplete/python-argcomplete_1.8.1-1.5.debian.tar.xz' python-argcomplete_1.8.1-1.5.debian.tar.xz 7272 SHA512:59c1d2a32d3dd4c483e7455ee9dbe67ee9f65aa87a2c09c05582da32610f2d85942dfd9bb8aa0c1e47d8162b0699a1b5e3845d00e93ddf69308a6b8ba9739acb
```

### `dpkg` source package: `python-attrs=21.2.0-1`

Binary Packages:

- `python3-attr=21.2.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-attr/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-attrs=21.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-attrs/python-attrs_21.2.0-1.dsc' python-attrs_21.2.0-1.dsc 2361 SHA512:eec9a65c4e9518cf9b124a70409a3be0c40e5404ffee18b8a99dc541c9ce9e9699cef3f4bf2e6cf803e060aba208d176d1e0207784687382dd9ee50aa4cf324c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-attrs/python-attrs_21.2.0.orig.tar.gz' python-attrs_21.2.0.orig.tar.gz 177524 SHA512:fa6569f3bdcc74a735b31dc67ce5ca3535eab8a5eb30f6b91ebf1149609294c0ef0d0910b8e41205d31c4745354c2262c18db901bae0af82c8b8cefc46f8a0a9
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-attrs/python-attrs_21.2.0-1.debian.tar.xz' python-attrs_21.2.0-1.debian.tar.xz 5328 SHA512:7abb633a1fc485bcf527f30a48be404eb34314ff3fad66ac00ccdae92e46e4524c3fcccc153c7adcbb48a8b9f4784d89629101c9309185bbed788a2af7d6c6a1
```

### `dpkg` source package: `python-cffi=1.15.0-1`

Binary Packages:

- `python3-cffi-backend:amd64=1.15.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-cffi-backend/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-cffi=1.15.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.15.0-1.dsc' python-cffi_1.15.0-1.dsc 1802 SHA512:114683c99bbacffa95bd709951fbe1b7c16dd93752c21c173a25e68318a643c3b4e430446e34fae3eb5fff7a2877be16968c59f3b77f7260e9e088057fadab4a
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.15.0.orig.tar.gz' python-cffi_1.15.0.orig.tar.gz 484058 SHA512:ee83efde6f77f4a0c5889088c4c208ed7b9071fe06dfc16a8d2396de07f78fe859e1e39866760198a9d700f3b7359e8715e8a3e4907feb81d3fc4b8dd0dbaca1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.15.0-1.debian.tar.xz' python-cffi_1.15.0-1.debian.tar.xz 7056 SHA512:9bfffa3b0651b15ed4bedf420476b6d17a6847568f2db1e88cb6fac3cfc5f4e1b0a8270bb7e10e83bdb4fc62d431b5fbd2ceb7d1e7383eb11abf594e68aaee9e
```

### `dpkg` source package: `python-coverage=6.2+dfsg1-2`

Binary Packages:

- `python3-coverage=6.2+dfsg1-2`

Licenses: (parsed from: `/usr/share/doc/python3-coverage/copyright`)

- `Apache-2`
- `Apache-2.0`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris python-coverage=6.2+dfsg1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-coverage/python-coverage_6.2%2bdfsg1-2.dsc' python-coverage_6.2+dfsg1-2.dsc 2286 SHA512:45201623f7f960703d7afadc1197e7abe4db30d35c79a7929a3fb9e290a67a046c2c98fbd3e0f6309018323eb01e5df83972bc1e835a0aaca896a95dac350442
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-coverage/python-coverage_6.2%2bdfsg1.orig.tar.xz' python-coverage_6.2+dfsg1.orig.tar.xz 532932 SHA512:16edb82c919f2bed5346484e30992b849a496f6d7a1d502db66b12288e917392b748ca607b09cbbde558bd4eff804e175a426b079a30083e15ee306de5a11cfb
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-coverage/python-coverage_6.2%2bdfsg1-2.debian.tar.xz' python-coverage_6.2+dfsg1-2.debian.tar.xz 19232 SHA512:fc9e06f5c46376106f2b8fb974c4cd58c5354119464cd0ed6e11096b4d16645d861eb7472160089c9712c5d1ae9b1a4603353a3524e4171c2c163223c15ab9cf
```

### `dpkg` source package: `python-cryptography=3.4.8-1ubuntu1`

Binary Packages:

- `python3-cryptography=3.4.8-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python3-cryptography/copyright`)

- `Apache`
- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-cryptography=3.4.8-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_3.4.8-1ubuntu1.dsc' python-cryptography_3.4.8-1ubuntu1.dsc 3116 SHA512:7d096c28c8567c5b02dd53c4c9fcb9be01332f479ccf6e3f43490b2d0a5ae8afc30e24692f16948049fdb07e93f98e8e7412cdf2bd31510fd1707383d3c8ff36
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_3.4.8.orig.tar.gz' python-cryptography_3.4.8.orig.tar.gz 546907 SHA512:b0d64a573b488af3e453fc1885bbafb65f8a2260e81cf64830f981589afca0bd7be052a5f5b8ed83dd78d9638da37c680f3705cbf2d47d5b28fb5a5454f1cea5
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_3.4.8-1ubuntu1.debian.tar.xz' python-cryptography_3.4.8-1ubuntu1.debian.tar.xz 23260 SHA512:af987a9a6384cf8ac27f3b186dc9dc8a6e570a7db7abae2332959793783aae8608eaf1ebc4c4a994d062ceea4cea34b5a05666c7d780eb06a35a7fddd2c68c0c
```

### `dpkg` source package: `python-dateutil=2.8.1-6`

Binary Packages:

- `python3-dateutil=2.8.1-6`

Licenses: (parsed from: `/usr/share/doc/python3-dateutil/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris python-dateutil=2.8.1-6
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.8.1-6.dsc' python-dateutil_2.8.1-6.dsc 2129 SHA512:defe085f213b14dcb2b1bf568b092cf539fad2690f4ad1895d153c8011a4c8744f25a8710b2eea2aa9de7516f0eda06e2aade979f1c489a5bd936bdf220a0d63
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.8.1.orig.tar.gz' python-dateutil_2.8.1.orig.tar.gz 331745 SHA512:337000216e0f8ce32d6363768444144183ab9268f69082f20858f2b3322b1c449e53b2f2b5dcb3645be22294659ce7838f74ace2fd7a7c4f2adc6cf806a9fa2c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.8.1-6.debian.tar.xz' python-dateutil_2.8.1-6.debian.tar.xz 11508 SHA512:f376c089d6f43f21d4cf602e251ba4537a23fb995d47b200b00158ff4c2396230fc36983e8bde1a2c5af97c1f69e769252467273a6552506832ccfcac80ffb55
```

### `dpkg` source package: `python-distro=1.7.0-1`

Binary Packages:

- `python3-distro=1.7.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-distro/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris python-distro=1.7.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-distro/python-distro_1.7.0-1.dsc' python-distro_1.7.0-1.dsc 1550 SHA512:f6e8f584ac293cdb64eddd7f05588ed2a912afd0f6bd1694268c68075a71e34e277fd649bd704df40b8249b0ad6f73d9ca3a837a3eb5ab73660e2e9b536f1879
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-distro/python-distro_1.7.0.orig.tar.gz' python-distro_1.7.0.orig.tar.gz 52250 SHA512:6d2e2640b5233f9503adec1290d61cfe58a75faba75b42c71c219c73cf32d7a071018543721894d2565219d3d41b616300469bac8d6d4c5a91db89120343d32e
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-distro/python-distro_1.7.0-1.debian.tar.xz' python-distro_1.7.0-1.debian.tar.xz 3372 SHA512:5b3ad1f6d204bf3da55a10eadbb447c5fc54f50b9cfec9dd2d9b54b8c1fc24b201141e09e717ccb084f63441f44aa121f0846535565df2aebea6505164a844a5
```

### `dpkg` source package: `python-docutils=0.17.1+dfsg-2`

Binary Packages:

- `docutils-common=0.17.1+dfsg-2`
- `python3-docutils=0.17.1+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/docutils-common/copyright`, `/usr/share/doc/python3-docutils/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Python-2.1.1`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris python-docutils=0.17.1+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.17.1%2bdfsg-2.dsc' python-docutils_0.17.1+dfsg-2.dsc 2399 SHA512:ed63823b3b46e5c374bbc5044a5760ce53dffeadec65ef8a99fc72030d85ba186744acc7a70cc2cac3ba1159f3826d67e9a8747016f994011c79ac9639b80d1a
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.17.1%2bdfsg.orig.tar.xz' python-docutils_0.17.1+dfsg.orig.tar.xz 1504140 SHA512:90a3af02e6cd11edf07f3fe5dae06042138bf80b54bd88b22b866fa69e0ed6b3babc6bc9ba30bf2452d09fd155720c2c9ceb3e2cfe42e0a1cf10637ba09404ea
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.17.1%2bdfsg-2.debian.tar.xz' python-docutils_0.17.1+dfsg-2.debian.tar.xz 30924 SHA512:eaf37bc33b90bbd34c5e6a54ac0360442e5c3bb356f5b9546aa4bcfc6514740610674eb9d9b470b4c48e330e2d3380047b6979813f5a337974ae0b564d892253
```

### `dpkg` source package: `python-flake8=4.0.1-2`

Binary Packages:

- `python3-flake8=4.0.1-2`

Licenses: (parsed from: `/usr/share/doc/python3-flake8/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-flake8=4.0.1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-flake8/python-flake8_4.0.1-2.dsc' python-flake8_4.0.1-2.dsc 2378 SHA512:416654abcabe42dcc00824f0461c355c122f5a3af0afe7aabd4e32c6d54be623d9582ef10f65c4733127577033b25d9f9dea8cb171899d8360562aabb575c6de
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-flake8/python-flake8_4.0.1.orig.tar.gz' python-flake8_4.0.1.orig.tar.gz 154905 SHA512:0bdbf0218ce893df1c3e61f51cd3f371a5c72bb49ef78fec39548b1684e49b024e91cf4e3dcea60ba1efc08727985ef485814c372461e062ff4f810da99a1796
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-flake8/python-flake8_4.0.1-2.debian.tar.xz' python-flake8_4.0.1-2.debian.tar.xz 8452 SHA512:b6f5e0cf36138d2a74b626d8e1ed852b3f2ed9ff86654cf8a1d9f19cb103124a03ee4c39f5b0c7441c5ad52021baf6281adab61eeed0d0844711bc4c0f8d8f16
```

### `dpkg` source package: `python-importlib-metadata=4.6.4-1`

Binary Packages:

- `python3-importlib-metadata=4.6.4-1`

Licenses: (parsed from: `/usr/share/doc/python3-importlib-metadata/copyright`)

- `Apache-2`
- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris python-importlib-metadata=4.6.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-importlib-metadata/python-importlib-metadata_4.6.4-1.dsc' python-importlib-metadata_4.6.4-1.dsc 1778 SHA512:9e1bb973de96943416f751a15492daf43b47e684088431b4c0b2a1cdc6818c2e84bb5fdffc1104cda15d86fcf7ff4ccbe023b1609a488ec2abaf2e6ebddb6932
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-importlib-metadata/python-importlib-metadata_4.6.4.orig.tar.gz' python-importlib-metadata_4.6.4.orig.tar.gz 39881 SHA512:20aad4adbea8bc417a77cd67a6e22e690e95913ee34822d79e4bb0472f396ece2137ab4cabc455a8154251fe563ed7f56a68bdb7b08a91c8a32f735608cb4a7c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-importlib-metadata/python-importlib-metadata_4.6.4-1.debian.tar.xz' python-importlib-metadata_4.6.4-1.debian.tar.xz 3416 SHA512:39187276acd366bd3654ac41f2394dcf26580b81458e1b9d78b71f93df5c8eedc73c0c2eb21344889a900910b4849e5c8c0ffbf199c2be6d98ad74b3c76b5e92
```

### `dpkg` source package: `python-iniconfig=1.1.1-2`

Binary Packages:

- `python3-iniconfig=1.1.1-2`

Licenses: (parsed from: `/usr/share/doc/python3-iniconfig/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-iniconfig=1.1.1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-iniconfig/python-iniconfig_1.1.1-2.dsc' python-iniconfig_1.1.1-2.dsc 2253 SHA512:68c900ffff6c33973185fa17b45dbd0d0f5f1644d502db3616641fbeb5090e67d48504cfba79e55b2a8dccac7cb3769ad921d8fbfc2a9db4703db986ac9da958
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-iniconfig/python-iniconfig_1.1.1.orig.tar.gz' python-iniconfig_1.1.1.orig.tar.gz 7509 SHA512:3e86490e424adefcc36b498ed0e6c6a6d4c6a2804a95b99163cef456f303b1913e9afe34035039cf0f2e96f7624719dc85e4ab3917ccd59278b22894a00dbf26
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-iniconfig/python-iniconfig_1.1.1-2.debian.tar.xz' python-iniconfig_1.1.1-2.debian.tar.xz 2732 SHA512:8b05095285abb1786e8f348b43334066d76b57761b2e186962750a9d652b4885088027d1d7e5b2eaa6e0a444f19a928d3d5b5aab4eeee809751294e3e549c09c
```

### `dpkg` source package: `python-lark=1.1.1-1`

Binary Packages:

- `python3-lark=1.1.1-1`

Licenses: (parsed from: `/usr/share/doc/python3-lark/copyright`)

- `GPL-2`
- `GPL-2+-with-bootloader-exception`
- `MIT`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris python-lark=1.1.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-lark/python-lark_1.1.1-1.dsc' python-lark_1.1.1-1.dsc 2405 SHA512:08e0c24df1ecd551e089a92d1c838ae6fe3019b8094e70c1990c7771e7b3b633a0d4a2a974f6b4e89d59125d1581b0cb31d162b7a9b87dfb6a9b7e6431fc6538
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-lark/python-lark_1.1.1.orig.tar.gz' python-lark_1.1.1.orig.tar.gz 405270 SHA512:8ce5f1fe97aff09f4f52c90d955b49157fc73e003f5ba0c7c9d9eae6317148fd4d4cd9eb03866e268e33a4d8a5e1dec5e4afe6ad229276ef55094c3938fb2d87
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-lark/python-lark_1.1.1-1.debian.tar.xz' python-lark_1.1.1-1.debian.tar.xz 5516 SHA512:ab73a3945850d2602bdccedda2ba71e394e849ee6f7cdd198dfe1e3450a5224b01fce47b1f30b37819b1c73056da63a152d2ced78bf11d3324743468fab0f219
```

### `dpkg` source package: `python-mccabe=0.6.1-3`

Binary Packages:

- `python3-mccabe=0.6.1-3`

Licenses: (parsed from: `/usr/share/doc/python3-mccabe/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-mccabe=0.6.1-3
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mccabe/python-mccabe_0.6.1-3.dsc' python-mccabe_0.6.1-3.dsc 2110 SHA512:1c41ba971457f851f2657e83ad3f6b332536849924c2a979789513a89a1eef495d2c2d73271a25232d181e9e679377b0fde97a7fa94adb486e1666597242a100
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mccabe/python-mccabe_0.6.1.orig.tar.gz' python-mccabe_0.6.1.orig.tar.gz 8612 SHA512:d8fc251a29790887c14c5932c5172b4cd578cd37ccf14cb96e80f0b97f27023427ea032d14e1e2a99d72627b055eb285f60db69e679ecd79d90a34b0255703d8
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mccabe/python-mccabe_0.6.1-3.debian.tar.xz' python-mccabe_0.6.1-3.debian.tar.xz 2452 SHA512:7b4f629b36caf5567e6d6b649b7f0dae841a5c3132cafd4ceec69709640887579fdc5d51715ef7ed6f0c9bee22948938dc903b237dd31291619ce44a8bd2363b
```

### `dpkg` source package: `python-mock=4.0.3-3`

Binary Packages:

- `python3-mock=4.0.3-3`

Licenses: (parsed from: `/usr/share/doc/python3-mock/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris python-mock=4.0.3-3
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mock/python-mock_4.0.3-3.dsc' python-mock_4.0.3-3.dsc 1920 SHA512:c2ea8ad99d2d5f15d3eb82b2d89b0e3574736d9d7f64a59b3087b3506d0738d7c50107d6ec7f62dff7836f98eeb5d2788431987c292fd4b3af879ce2e735f675
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mock/python-mock_4.0.3.orig.tar.gz' python-mock_4.0.3.orig.tar.gz 80318 SHA512:adfdab253eb3bc1b6cb767c58ffa3a8a5c5f88da0f04ea6680e0d87da59177972d2d99bfe0a770ac2ed4f809ca6a090a9d0f789eea8f4365ef2c54f8e8792e89
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-mock/python-mock_4.0.3-3.debian.tar.xz' python-mock_4.0.3-3.debian.tar.xz 7604 SHA512:85264ced6742588a724da3acd78b933cd3eabd692a125dcd956758cd4c1246ce590372c5264af25be0b45a6d0e7584adee10654f3f7b35849d35c24225e40083
```

### `dpkg` source package: `python-notify2=0.3-4`

Binary Packages:

- `python3-notify2=0.3-4`

Licenses: (parsed from: `/usr/share/doc/python3-notify2/copyright`)

- `BSD-3-Clause`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris python-notify2=0.3-4
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-notify2/python-notify2_0.3-4.dsc' python-notify2_0.3-4.dsc 2151 SHA512:a576cae8cb294f5b6a8a5f2977fec6004f468562818de3e9966173d71cae0e408455c340ef8abb23ef807748f44edbb8a643e681467047cea616d86af705c35c
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-notify2/python-notify2_0.3.orig.tar.gz' python-notify2_0.3.orig.tar.gz 8798 SHA512:3290a5ff291d5500bcf631094fcf10302b234353eb8c26b91e7cd264238443866aadc15224d51eb6608e16b7ffbc9316d4bc551e5ad9de2a48b12a31b195739f
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-notify2/python-notify2_0.3-4.debian.tar.xz' python-notify2_0.3-4.debian.tar.xz 3416 SHA512:4ce63399eb2c5e255e0d7eccb5244e9905bf921ead9b2bd23840466bb276aa496c3a903544047f6c0dfc9490fea4923cce186780fd4722d9aaa9e98071cbf815
```

### `dpkg` source package: `python-packaging=21.3-1`

Binary Packages:

- `python3-packaging=21.3-1`

Licenses: (parsed from: `/usr/share/doc/python3-packaging/copyright`)

- `Apache-2.0`
- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris python-packaging=21.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-packaging/python-packaging_21.3-1.dsc' python-packaging_21.3-1.dsc 2034 SHA512:bca1befa4b8fd264e0ca0837bc92aa28fac3d2bded51cd83c63427c103f2a5c1add07b674be855195ddddc1f5ca83273701c612b76fcf75f620b0d6fee957923
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-packaging/python-packaging_21.3.orig.tar.gz' python-packaging_21.3.orig.tar.gz 84848 SHA512:2e3aa276a4229ac7dc0654d586799473ced9761a83aa4159660d37ae1a2a8f30e987248dd0e260e2834106b589f259a57ce9936eef0dcc3c430a99ac6b663e05
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-packaging/python-packaging_21.3-1.debian.tar.xz' python-packaging_21.3-1.debian.tar.xz 2868 SHA512:ec3a7fc0e3472721757ac4ddd59b1a1593c91a9d3471770a29a0dc842ea72af82f7cfb34c78bdfa4a1e04a5ba55721e062a18d6502efbd666e8719c73776ab14
```

### `dpkg` source package: `python-pbr=5.8.0-0ubuntu1`

Binary Packages:

- `python3-pbr=5.8.0-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python3-pbr/copyright`)

- `Apache-2`
- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris python-pbr=5.8.0-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-pbr/python-pbr_5.8.0-0ubuntu1.dsc' python-pbr_5.8.0-0ubuntu1.dsc 3025 SHA512:58dae240359e918cbc3b831831dc8b94d8071e6c78023cf7f6aa79b6ea1fea91099536624f7095d571c925f82445f2e25f21f000b17046e300e225a522d9ccfe
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-pbr/python-pbr_5.8.0.orig.tar.gz' python-pbr_5.8.0.orig.tar.gz 127170 SHA512:61a8eb63bb76ce8515c4203d60df7c973e02ea61b603d155b611724efb2b15c42416bf8a0285451d3378056d390bbf63d991cec32cc4114ae5cc30ebae0a5a69
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-pbr/python-pbr_5.8.0-0ubuntu1.debian.tar.xz' python-pbr_5.8.0-0ubuntu1.debian.tar.xz 10064 SHA512:95e10efcb165e4159240a4de2e13d4cbab4dce583079775f074ebc0c4665ed093d650a3a4de2c002d7762e9d6bc11b66961acd2c3845902eed5e094faac4b261
```

### `dpkg` source package: `python-pluggy=0.13.0-7.1`

Binary Packages:

- `python3-pluggy=0.13.0-7.1`

Licenses: (parsed from: `/usr/share/doc/python3-pluggy/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-pluggy=0.13.0-7.1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pluggy/python-pluggy_0.13.0-7.1.dsc' python-pluggy_0.13.0-7.1.dsc 1862 SHA512:cfb7467476eb73c4404c38ce3253d2e5d332c768e17cbc38e01bb64e736bf8a72c885b54355a9bc533d17a1d5ce5279c668d855d5c6fe974da951353c2427b36
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pluggy/python-pluggy_0.13.0.orig.tar.gz' python-pluggy_0.13.0.orig.tar.gz 57726 SHA512:82cf7d8aa4a0e09f8ba5048cd7ce038f34ca1453fe0c5a7926a2113e64528d0861955f8544035b4ffd61f0227e3d30d8d4180a05bf80e0de4809546e990bd4c7
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pluggy/python-pluggy_0.13.0-7.1.debian.tar.xz' python-pluggy_0.13.0-7.1.debian.tar.xz 3136 SHA512:650a8b78b1a12c4728bd8f77d2a59e8d3fa153562edd30e3602f1369416ab9778ed1ed6aa5591cf11a0c56c98f9eda29e7eb5b907afefb5c5027549d73a157dd
```

### `dpkg` source package: `python-psutil=5.9.0-1`

Binary Packages:

- `python3-psutil=5.9.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-psutil/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris python-psutil=5.9.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-psutil/python-psutil_5.9.0-1.dsc' python-psutil_5.9.0-1.dsc 2172 SHA512:cb884a0de19a4e811021a9845bf7331a6f478ce96b4cc6f0df03be9ed161a72f25f1468a577fa45b6d3490d5bc500a74e561e1e369b6b65532f69149b8014961
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-psutil/python-psutil_5.9.0.orig.tar.xz' python-psutil_5.9.0.orig.tar.xz 331792 SHA512:2d5ee8fd620175f05b2f3b1e8098d85ef1861c07a4ca59ac24c9cb2892c44b0ce008d3dd914e566435592255437b22cf22bbc60e9e67ca470ddb780e037ce7ac
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-psutil/python-psutil_5.9.0-1.debian.tar.xz' python-psutil_5.9.0-1.debian.tar.xz 6352 SHA512:138e854ed13e4300b2fb075ec509beea5999784e10f56ecc885b8d14c2c686a742dc03d9662aff395c0249ccc7b60170db59c2bb489975ff36d991e76de224f9
```

### `dpkg` source package: `python-py=1.10.0-1`

Binary Packages:

- `python3-py=1.10.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-py/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-py=1.10.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-py/python-py_1.10.0-1.dsc' python-py_1.10.0-1.dsc 2086 SHA512:49fdc9d0fda37e0dff1dc707944d3c9f26d560ec4e8e28e391cd487fb426441258eb566400dd9db976386f6ac885a0425a4b8f1199c6a715c1db8114c0f6355d
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-py/python-py_1.10.0.orig.tar.gz' python-py_1.10.0.orig.tar.gz 206984 SHA512:7a0eb964067bc01fa4f8ffe70b043abfd4619134fbee2935713e28382085d0b8972c319ed665a643b879b18ce662db8a9bd722937af7cf36c233214eea211dd1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-py/python-py_1.10.0-1.debian.tar.xz' python-py_1.10.0-1.debian.tar.xz 12440 SHA512:3c596bd4eff72e2aee33c5fea3f4709186cd0f7ec188a0e974a0d7cc7e3398d70299b93263ca64dcc35806c812e49ef0170272172b48359684d45de15c70ce32
```

### `dpkg` source package: `python-pytest-cov=3.0.0-1`

Binary Packages:

- `python3-pytest-cov=3.0.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-pytest-cov/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris python-pytest-cov=3.0.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pytest-cov/python-pytest-cov_3.0.0-1.dsc' python-pytest-cov_3.0.0-1.dsc 2046 SHA512:a850973343f9131d5518b7dc8b758bf0678f32bb4b810bb8e7443dd9b2264becb379bc574b78985939fb0c30f5aaa86d9df4a6ce333aea0ef7802af1ce133862
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pytest-cov/python-pytest-cov_3.0.0.orig.tar.gz' python-pytest-cov_3.0.0.orig.tar.gz 45384 SHA512:1035090a79f333e3ae13f9a431afea742026b00e6868f1d6c075462d77e88a8f04783a73dc93253de05dc45da74c517c5a87686036369d2ff5ea3867baf8bc35
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-pytest-cov/python-pytest-cov_3.0.0-1.debian.tar.xz' python-pytest-cov_3.0.0-1.debian.tar.xz 2572 SHA512:44d404cb334b915bd6835736a6705de036722cb0c19c6530a667d3fc3d3b476ba40725543faae8246ccdfc5898c57918b032f6efb5dc5fcae442a46d71cd38a5
```

### `dpkg` source package: `python-roman=3.3-1`

Binary Packages:

- `python3-roman=3.3-1`

Licenses: (parsed from: `/usr/share/doc/python3-roman/copyright`)

- `Python-2.1.1`
- `ZPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris python-roman=3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_3.3-1.dsc' python-roman_3.3-1.dsc 2100 SHA512:1d32743ab9a2408caf26a52b37263c7f6d7895f911ed2e8eefbc07cec275430aee3a17ea0dccb55ca39cdccb37fd2a312cec650ca9f5e5fdd4ce6aa8c74ff8f3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_3.3.orig.tar.gz' python-roman_3.3.orig.tar.gz 7174 SHA512:90aab322e4135f221f8278c61ee6ebf2c15f3e35c9eabea19af01c08b95fe01e32faf77da479f80897c7fea6d175dc004b4c72a3cf4105db9e9665c3a30d28ed
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_3.3-1.debian.tar.xz' python-roman_3.3-1.debian.tar.xz 6820 SHA512:346b0233f997b09df68a7cc13d0e00288ce69013eebff26e46ce0435f885ed2083e3ec99a2f2fb4bccc6d4749a8bd8ad1b8e9c75ce008e4e5773ff8722999463
```

### `dpkg` source package: `python-toml=0.10.2-1`

Binary Packages:

- `python3-toml=0.10.2-1`

Licenses: (parsed from: `/usr/share/doc/python3-toml/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-toml=0.10.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-toml/python-toml_0.10.2-1.dsc' python-toml_0.10.2-1.dsc 2052 SHA512:fe84b90ad23375fbef4d5452b9cae81584f13f3e7743267c34093f79a2b9e2e30c43a4875e6d9cd4b44588d9802dde89b1cde661ce171aa389402f7f7e37aea3
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-toml/python-toml_0.10.2.orig.tar.gz' python-toml_0.10.2.orig.tar.gz 23325 SHA512:5c706a3ae336e6b29bdce9752b91c677f7610cbcc1af4169cc24779e248031406cd19ac367725b2aa7903e4b1db71fa59255238c0270b2c146fd5d7e12d9a5da
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-toml/python-toml_0.10.2-1.debian.tar.xz' python-toml_0.10.2-1.debian.tar.xz 2952 SHA512:61ac31ec1ae89325facbdc35e4252095171d30d656709174a0404b19c44481d850140e076a2c9fa8c30ad21c1245b47c26bd59f49a5e7fe2588a5691171df90b
```

### `dpkg` source package: `python-zipp=1.0.0-3`

Binary Packages:

- `python3-zipp=1.0.0-3`

Licenses: (parsed from: `/usr/share/doc/python3-zipp/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-zipp=1.0.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-zipp/python-zipp_1.0.0-3.dsc' python-zipp_1.0.0-3.dsc 2109 SHA512:f2fa7fcb476ba23b65c2dfae30bc57252881da6f1305a9d51428f4a54bc480d63552bdcd29f52655de980b7caa00ad9ba95f3be73a70c54a3d7e1b004db4ae5e
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-zipp/python-zipp_1.0.0.orig.tar.gz' python-zipp_1.0.0.orig.tar.gz 10821 SHA512:dbfadfedd30ca4cb31ac4163f367134d96e57405ef00d5f4c19c0af7a141f78487dec29a0ba94975584fcb462d22c8b536bf29c67b7e298368072e897b0e9d82
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-zipp/python-zipp_1.0.0-3.debian.tar.xz' python-zipp_1.0.0-3.debian.tar.xz 2332 SHA512:851fbfb71c97c508c58cc5cc8ef00542b9b1aab4e15e40e969172171c6f72c4b4fb61187dcbaad7f545604bc94c5fa628bf24763903df1ad1743761d7e8583fa
```

### `dpkg` source package: `python3-catkin-pkg-modules=0.4.24-1`

Binary Packages:

- `python3-catkin-pkg-modules=0.4.24-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-catkin-pkg-modules=0.4.24-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-catkin-pkg-modules/python3-catkin-pkg-modules_0.4.24-1.debian.tar.xz' python3-catkin-pkg-modules_0.4.24-1.debian.tar.xz 2024 SHA512:34839c06efbaceccbfa6fe15e8d62264ca9fd1271f500389df7358b81830e82337f5c526e9935ddd147526dd3da35e8692761d86313f1bdabaca52670a919039
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-catkin-pkg-modules/python3-catkin-pkg-modules_0.4.24-1.dsc' python3-catkin-pkg-modules_0.4.24-1.dsc 1026 SHA512:02c8c18ec94c70bf39670ee4a61a6a8374adc3abcfc93424d4db323da3b14af729e1c83313546a724b78d1629d1a79ec33ada5434575f53e4594004c44d01393
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-catkin-pkg-modules/python3-catkin-pkg-modules_0.4.24.orig.tar.gz' python3-catkin-pkg-modules_0.4.24.orig.tar.gz 61189 SHA512:77336a9221cfccca22782dd111bea6ce34ccd6cfdf288bb523b66b7999023af8a53125f0fe97d8ccf54ff665aac1bca32248136662a0ab4743f893e962c270cd
```

### `dpkg` source package: `python3-catkin-pkg=0.4.24-100`

Binary Packages:

- `python3-catkin-pkg=0.4.24-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-catkin-pkg=0.4.24-100
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-catkin-pkg/python3-catkin-pkg_0.4.24-100.debian.tar.xz' python3-catkin-pkg_0.4.24-100.debian.tar.xz 2012 SHA512:3db57a92e09b3d7406df2299fb3ced667e78ef7b20273da740c453b81075af75173850f31c20b2d550be9fc1b2d047b567f87b0438736c619742f2cb9046f944
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-catkin-pkg/python3-catkin-pkg_0.4.24-100.dsc' python3-catkin-pkg_0.4.24-100.dsc 962 SHA512:48deef0904ca87c021eece7ec5ac1d3cce205b0790140117c42c84c9c0bac9ceb0f95bf3bf0b3642a2f0ff5744ff5d5d632eb675c7c6b7c114197aa35660188d
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-catkin-pkg/python3-catkin-pkg_0.4.24.orig.tar.gz' python3-catkin-pkg_0.4.24.orig.tar.gz 14786 SHA512:f37d1a1285115d125a8ad3cfd67f7f969b6ab7ad0452eefc5d690832a19623e5e9418fa35841139a952b3883ea5406348fae741e09ae3273546212a35489cc59
```

### `dpkg` source package: `python3-colcon-argcomplete=0.3.3-1`

Binary Packages:

- `python3-colcon-argcomplete=0.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-argcomplete=0.3.3-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-argcomplete/python3-colcon-argcomplete_0.3.3-1.debian.tar.xz' python3-colcon-argcomplete_0.3.3-1.debian.tar.xz 1612 SHA512:71ead0b0756a14fa54111a023c1c77ea9040c48e138f1076b630b351b1c59cf2991389b0811776ce979d9ca91887d69883b1208e3ef32c0a2e8518c6c53c7a4b
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-argcomplete/python3-colcon-argcomplete_0.3.3-1.dsc' python3-colcon-argcomplete_0.3.3-1.dsc 969 SHA512:f34a1b95c076c28bf9b45793f87818f21f5054421cbead38e59e1ceae1c37fa15ee21ddf33fb72e400fd731dd8c8918c3f32f34c6a2b83e4eaf05e85870ca038
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-argcomplete/python3-colcon-argcomplete_0.3.3.orig.tar.gz' python3-colcon-argcomplete_0.3.3.orig.tar.gz 7577 SHA512:fea054c099f8d950537ec34186e3ee05d2c514cc4680b958736ec4bf0e4cc4a4122f86a7581d2622dea0bd55fcc5c17b840bbf00c29bcbfb9f7af8a8868cea90
```

### `dpkg` source package: `python3-colcon-bash=0.4.2-1`

Binary Packages:

- `python3-colcon-bash=0.4.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-bash=0.4.2-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-bash/python3-colcon-bash_0.4.2-1.debian.tar.xz' python3-colcon-bash_0.4.2-1.debian.tar.xz 1076 SHA512:7cbe01513c86ad51fec1fc5626d22237c7316fcf4cd4f46028bcc0471184465f575299c4983d4aed3fa1c8ccd7690f8b0380bbddfb2a292e8057c3d820b89809
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-bash/python3-colcon-bash_0.4.2-1.dsc' python3-colcon-bash_0.4.2-1.dsc 906 SHA512:52864f34d65ae34f44921ce5215ced8cfa3886feecfa0e086a323eea8cad24d2436fa38caf3fc4311c0956356fb8f8b1654950cc55daf93a69531e794db2ed56
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-bash/python3-colcon-bash_0.4.2.orig.tar.gz' python3-colcon-bash_0.4.2.orig.tar.gz 5641 SHA512:81e6492d9a73a72751fd40cc0ecdbd23b15563ed7ede0b50ce9695b0fdc68465855396b56917b4089a4fe65ae8c7748737417345b4cda86a3c5ae18096809c07
```

### `dpkg` source package: `python3-colcon-cd=0.1.1-1`

Binary Packages:

- `python3-colcon-cd=0.1.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-cd=0.1.1-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-cd/python3-colcon-cd_0.1.1-1.debian.tar.xz' python3-colcon-cd_0.1.1-1.debian.tar.xz 1076 SHA512:19f3e96910d5fe2707a9b3a88e6bf5672f2f36f0a0e2153738088c42368a1ec3314ec44ea6308fc7b7831a6b104cb205b02a001b27dc649f8382854de5efee22
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-cd/python3-colcon-cd_0.1.1-1.dsc' python3-colcon-cd_0.1.1-1.dsc 888 SHA512:78a294acc17528efe01ac305576c9dda813bfdf88c1b9d58d2f31090d81b92b53942ca4d116ccaa746659b97f123da2c1d6ceace677aa20589e3e332caceed7e
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-cd/python3-colcon-cd_0.1.1.orig.tar.gz' python3-colcon-cd_0.1.1.orig.tar.gz 4215 SHA512:e6a212126570d8f459ffc1b46f796a6ec403e660ed7ed6bf3f965e3160c697888d9248a3f0253e4693c1183b99e861619383670e1c2ceca41962caea90d2c3bf
```

### `dpkg` source package: `python3-colcon-cmake=0.2.26-2`

Binary Packages:

- `python3-colcon-cmake=0.2.26-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-cmake=0.2.26-2
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-cmake/python3-colcon-cmake_0.2.26-2.debian.tar.xz' python3-colcon-cmake_0.2.26-2.debian.tar.xz 1120 SHA512:08d27f880ffcfe001f02dd3489fa25aa5483db1e4b2686bc91a3b6eec67862e4e0b2ce0a1994f327d956cd0a21fbee749185caefdcff3f022dfeaa1cdaa52b5f
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-cmake/python3-colcon-cmake_0.2.26-2.dsc' python3-colcon-cmake_0.2.26-2.dsc 965 SHA512:ac8b8231287b57ca2c88ddf2ab964a5e0c97802619d2b15b1ee3ecbfbe336f1f1c2def00127dcd8dce6fd59b10118bae9ec8d7f278f6f92a187c72bd18cecbd0
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-cmake/python3-colcon-cmake_0.2.26.orig.tar.gz' python3-colcon-cmake_0.2.26.orig.tar.gz 16858 SHA512:71334a2c2dac64b82f48a78a853f7030a4a027161e9a4c2cc3eead4037fb50b2120efe4f4c66226f665157cbc45d979826b63319826d8de285b9d37f0a7d511f
```

### `dpkg` source package: `python3-colcon-common-extensions=0.2.1-1`

Binary Packages:

- `python3-colcon-common-extensions=0.2.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-common-extensions=0.2.1-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-common-extensions/python3-colcon-common-extensions_0.2.1-1.debian.tar.xz' python3-colcon-common-extensions_0.2.1-1.debian.tar.xz 1204 SHA512:b5963a1f450299fa4a2c06caee7a7292e16844261641edf1315e5799f99aad5aa7be10f2b947cb62384f20a0b012107873aedfd6c932607501236c94d96f7bd9
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-common-extensions/python3-colcon-common-extensions_0.2.1-1.dsc' python3-colcon-common-extensions_0.2.1-1.dsc 1023 SHA512:d40498a4519032da4b2c11a2bfe7a79b4aeda3e622c75423546e76a6a89993a6dad62464b936d54fef2806bd3b3cbca23bee0fe66145e9af0d42531f3be5f6d6
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-common-extensions/python3-colcon-common-extensions_0.2.1.orig.tar.gz' python3-colcon-common-extensions_0.2.1.orig.tar.gz 1662 SHA512:df2c17decf64d3d6d5a3f78a53033b422b30cc89e6089da68f740bf78d3a99814e332c98b3a5b9b7ba6a7887f2f9a86567587edcdfa95575817217bdb8d42167
```

### `dpkg` source package: `python3-colcon-core=0.6.1-2`

Binary Packages:

- `python3-colcon-core=0.6.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-core=0.6.1-2
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-core/python3-colcon-core_0.6.1-2.debian.tar.xz' python3-colcon-core_0.6.1-2.debian.tar.xz 1580 SHA512:7af7ad507990ae33ee894fba0efcade2662561af3d1837ac3d1f8924d7721723d983dcbf7d5d4b7120d49d403798b236d4465bee46d00b4cea7fcfa9e959cfdf
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-core/python3-colcon-core_0.6.1-2.dsc' python3-colcon-core_0.6.1-2.dsc 952 SHA512:d15e479b3f1dee4dbc8dceaed1d42f487b91cc46dd368bcdf854fb5cf461ab103b708d2e583627d3198f6fc01ec3a33a18eeee789a6b6fa7e3aabbff1caa270a
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-core/python3-colcon-core_0.6.1.orig.tar.gz' python3-colcon-core_0.6.1.orig.tar.gz 100051 SHA512:9cc90ff44c1c9e3777493ea385d5cd350df2998a1a3a9cd59fb22dd7ec4a9be0749db8e1135961af6938c846d8a86e79bc302375a8e1e67c8e5c59fef7bac75e
```

### `dpkg` source package: `python3-colcon-defaults=0.2.5-1`

Binary Packages:

- `python3-colcon-defaults=0.2.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-defaults=0.2.5-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-defaults/python3-colcon-defaults_0.2.5-1.debian.tar.xz' python3-colcon-defaults_0.2.5-1.debian.tar.xz 1180 SHA512:c79395e205f6b8d39e4cbfc7792c4eddae0fd13f4f55b7f92a052c1613c48fac1eaced696ab996eebfd84ab118d6401ac0b4e5c7936377ca795e33ba3ba66a47
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-defaults/python3-colcon-defaults_0.2.5-1.dsc' python3-colcon-defaults_0.2.5-1.dsc 942 SHA512:00fbb831e6d16b1fa833c330fdf6c47d04930608c7ae92542a42bedb52b1916dd4ae868a914385d89d7725aefad12a7a15a3593ce1bdc79e84b4dff84b3265f7
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-defaults/python3-colcon-defaults_0.2.5.orig.tar.gz' python3-colcon-defaults_0.2.5.orig.tar.gz 5926 SHA512:683a13ac89a065462cefbb3fcc4ed809b23ff374ad8cc8c02853a721497b173d11da8b02674a02a818e9a78e684203861450dd91e73a8d5c7307efcc0133268d
```

### `dpkg` source package: `python3-colcon-devtools=0.2.2-1`

Binary Packages:

- `python3-colcon-devtools=0.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-devtools=0.2.2-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-devtools/python3-colcon-devtools_0.2.2-1.debian.tar.xz' python3-colcon-devtools_0.2.2-1.debian.tar.xz 1072 SHA512:2b0d5d8d57649c07e70ffa72d458bc034be4c3ae88bdb988c862bf7b95bf582d89a8732ca2a32bd8ee6f4b0a646a010e001245dcd1f74c7d385ae553166c4d80
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-devtools/python3-colcon-devtools_0.2.2-1.dsc' python3-colcon-devtools_0.2.2-1.dsc 942 SHA512:8abaeff2a306e0eac3ffe11131388ccf14f9dfda603a12f3e573c1020ef3bafe4fcd7f900f02518379dd3f7790a82a425720a952147e5d0c990bd5b1a7423737
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-devtools/python3-colcon-devtools_0.2.2.orig.tar.gz' python3-colcon-devtools_0.2.2.orig.tar.gz 4834 SHA512:44fb064a0f9bb58ab90e3440e68f11a457c676e000ecc57e51adb8fd0979d86beb4ec8669628c0c4c0fc46f2b28fba71e92a62129bb6907f697e9ff804964499
```

### `dpkg` source package: `python3-colcon-library-path=0.2.1-1`

Binary Packages:

- `python3-colcon-library-path=0.2.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-library-path=0.2.1-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-library-path/python3-colcon-library-path_0.2.1-1.debian.tar.xz' python3-colcon-library-path_0.2.1-1.debian.tar.xz 1000 SHA512:f0e4df16b6139d403f5fad5f581632eb5cd31df8ebc648c705d4da7c9eefdf6a005095e4301322cba03780114baff6d58e49f884cec6ac3ba2959ed4d638b292
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-library-path/python3-colcon-library-path_0.2.1-1.dsc' python3-colcon-library-path_0.2.1-1.dsc 1029 SHA512:3672203f9f0f35df233df0c54ac056fb37744be7ac56eab1d325d6b575b381b4816d07b59c4def12687dcc2e64ff627a4c012df3a9f23f7a031c6ec19f7b297d
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-library-path/python3-colcon-library-path_0.2.1.orig.tar.gz' python3-colcon-library-path_0.2.1.orig.tar.gz 3783 SHA512:60922210d6184263705493bd6764df4c3c7c07da3676217267452a339da35bece4ff308d2bd8db0446f363e53b54ddd068272f47fa99414bdccffef0c5cb36c6
```

### `dpkg` source package: `python3-colcon-metadata=0.2.5-1`

Binary Packages:

- `python3-colcon-metadata=0.2.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-metadata=0.2.5-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-metadata/python3-colcon-metadata_0.2.5-1.debian.tar.xz' python3-colcon-metadata_0.2.5-1.debian.tar.xz 1112 SHA512:ce98b0e24312a8e0ba11c2f01693448c5701a81aba8d6bb2f0a73679ef1ae0e94e5e75637271850c7f5a868f899cde49e9e9e025cc7cd63f057ac069239296a5
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-metadata/python3-colcon-metadata_0.2.5-1.dsc' python3-colcon-metadata_0.2.5-1.dsc 945 SHA512:17b64c85f88192dffc1b33542744a1a7f5fff0b68913cdd8259c4137c6f025c66e70fdaf54ed1356f1177abfd46cd64b108375ef99ef8c36fbd37c9ebb26de24
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-metadata/python3-colcon-metadata_0.2.5.orig.tar.gz' python3-colcon-metadata_0.2.5.orig.tar.gz 10846 SHA512:ba84f2c15a4981dfc0f4dbf10e68186705e8c3704e96182d620ff2f18971e5c145dfbdb1f04f71dacc18b262193c0c308ab39f113282974234e13a4a7dd77ef8
```

### `dpkg` source package: `python3-colcon-mixin=0.2.0-1`

Binary Packages:

- `python3-colcon-mixin=0.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-mixin=0.2.0-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-mixin/python3-colcon-mixin_0.2.0-1.debian.tar.xz' python3-colcon-mixin_0.2.0-1.debian.tar.xz 1120 SHA512:9067121ea29647355d03831b60ff31422963787725cc5d4975fb5b44f3224a236b6a145d63212003b1fd6a90931c0cdd0c44554cfea0908560bc491a4d199551
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-mixin/python3-colcon-mixin_0.2.0-1.dsc' python3-colcon-mixin_0.2.0-1.dsc 918 SHA512:e66b95dc58ad053e044dbb5cfa4b9ae0d573f129b2be43ec3727ba56054a0298cf8861a88349e9fff5bf449df7c193ef04257af5836f03a62782c211504c7171
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-mixin/python3-colcon-mixin_0.2.0.orig.tar.gz' python3-colcon-mixin_0.2.0.orig.tar.gz 12190 SHA512:e1ecbc113652394fd59b658ee4a09ac25681ec2c4ada64273fdf716c978765be76683cdcbde7ef1b957eb1c45f0a801781279c693b5a932e9a9e386b02fa645a
```

### `dpkg` source package: `python3-colcon-notification=0.2.13-1`

Binary Packages:

- `python3-colcon-notification=0.2.13-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-notification=0.2.13-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-notification/python3-colcon-notification_0.2.13-1.debian.tar.xz' python3-colcon-notification_0.2.13-1.debian.tar.xz 1596 SHA512:c2357d364eb5c8481d795e503005160f789a41556c34ad1046d5d7205cb7e6c2faaf09c71f4955a8c299017f73dfeb124eacdba95da72ea4ff62115be10108f6
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-notification/python3-colcon-notification_0.2.13-1.dsc' python3-colcon-notification_0.2.13-1.dsc 988 SHA512:22f3506620a501e67c9131bca8565c3137fe50a4ac0039adbec937ff1f0d9d0e2bca75e03e83e8e32cfa6f491ea62bfbcd66d3b277bfef20a5f4cb3d415f56c5
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-notification/python3-colcon-notification_0.2.13.orig.tar.gz' python3-colcon-notification_0.2.13.orig.tar.gz 54427 SHA512:b406b72b53085888c4a3393e4a3d01245828dca7bbf58679004a0fa0c14cad7cfd661b06360b66ade77dc11bd19c9d0108fc34a27cf03d7884bcbd9479a981fd
```

### `dpkg` source package: `python3-colcon-output=0.2.12-2`

Binary Packages:

- `python3-colcon-output=0.2.12-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-output=0.2.12-2
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-output/python3-colcon-output_0.2.12-2.debian.tar.xz' python3-colcon-output_0.2.12-2.debian.tar.xz 1092 SHA512:c462965e6bad1a6911aac816a9edfe090af6c4f339ca3660ab508da8b57a07837f78b41e656e2218e07f11bfe54e4070a371bd68b827672e067039388ac44995
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-output/python3-colcon-output_0.2.12-2.dsc' python3-colcon-output_0.2.12-2.dsc 971 SHA512:e6d1eb88336be76b66b7bdd9846597bb3c9a08a1d70e7968eaab1a3dea2fd875697cf1f142479c0932497f4a5bdf9fc05ccb7a4fc42603031f4eef529d2f6ef0
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-output/python3-colcon-output_0.2.12.orig.tar.gz' python3-colcon-output_0.2.12.orig.tar.gz 6909 SHA512:58a44c2507cf4406fcf597aa8089cde6164679e42ed0a2cd2e2f222d030a65426e91001ac3d13e306c17d6d634b8a3267ccf09867dc33da7adba8f1c108f6f3b
```

### `dpkg` source package: `python3-colcon-package-information=0.3.3-1`

Binary Packages:

- `python3-colcon-package-information=0.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-package-information=0.3.3-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-package-information/python3-colcon-package-information_0.3.3-1.debian.tar.xz' python3-colcon-package-information_0.3.3-1.debian.tar.xz 1072 SHA512:f15b4a25d26b8dd5bf27a6299d826e7079271b50f7c2530f2dd31d207fa8793d5717bf8da0f8f9aabd9840209d6e60300beb4b1b4c61ae20021c89923a88b0fd
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-package-information/python3-colcon-package-information_0.3.3-1.dsc' python3-colcon-package-information_0.3.3-1.dsc 1041 SHA512:04da1b58e811773dc724568f2cec9174689ea1c0f12c6576f461fa8b5d169ea7b60daf63ead44fa1c49103f33aa753d8aa0c4248dd891985b8e0cca1b4e21622
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-package-information/python3-colcon-package-information_0.3.3.orig.tar.gz' python3-colcon-package-information_0.3.3.orig.tar.gz 9863 SHA512:a98f6ac8cd41fc2d6b4bb6fdbebe7a4dbf12582cf103646ebde2d9b4d68df567fc056bda0c7ac0793c9ea9a206bfff48daabf551afbe73a614123d6d7bc6b803
```

### `dpkg` source package: `python3-colcon-package-selection=0.2.10-2`

Binary Packages:

- `python3-colcon-package-selection=0.2.10-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-package-selection=0.2.10-2
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-package-selection/python3-colcon-package-selection_0.2.10-2.debian.tar.xz' python3-colcon-package-selection_0.2.10-2.debian.tar.xz 1092 SHA512:073377f7d774ae9e91f12486c418d5b51c8d0a86ed41120c0056bd04bb32cbe83229a4d7c369aab5810f82a9fa138e3a1db6553dda995dc46c89f43d767f9c12
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-package-selection/python3-colcon-package-selection_0.2.10-2.dsc' python3-colcon-package-selection_0.2.10-2.dsc 1070 SHA512:66293ad0b13cbbf45e7ebbcddf47f2fcc626b0bc7acb504e03b8628540f2ca082be29d34ff91a88463735661d252bea138cb4bbeedb63e36a1a4369398aab761
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-package-selection/python3-colcon-package-selection_0.2.10.orig.tar.gz' python3-colcon-package-selection_0.2.10.orig.tar.gz 8008 SHA512:8bb9316507d08dbdeee4d725b7948a43b70888d5f8f684b5c2384ba83d5a0605c626940cfc623a5423e8a3f3e8c0cba0c6c6d23b3433e8ba1fc2f7d7b9e6e47f
```

### `dpkg` source package: `python3-colcon-parallel-executor=0.2.4-1`

Binary Packages:

- `python3-colcon-parallel-executor=0.2.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-parallel-executor=0.2.4-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-parallel-executor/python3-colcon-parallel-executor_0.2.4-1.debian.tar.xz' python3-colcon-parallel-executor_0.2.4-1.debian.tar.xz 1068 SHA512:98570b66c1fedf3cb7ad95135d2968b86e5e0f680b7b150423d26ab403082a9c7772e7b33656fe59be947aea877c07e404e222e59ee6487106b6a8e7b7b6c599
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-parallel-executor/python3-colcon-parallel-executor_0.2.4-1.dsc' python3-colcon-parallel-executor_0.2.4-1.dsc 1023 SHA512:499b154e09e32168cf6d67fd0eb8f740e2f59b5852f3a76fcfeb6b72b42a82f4c2698bddfe9f0aa0e5fe3c73695d0f1c5ecc84f15273f830c4146f05f4c74f09
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-parallel-executor/python3-colcon-parallel-executor_0.2.4.orig.tar.gz' python3-colcon-parallel-executor_0.2.4.orig.tar.gz 5647 SHA512:a1e05a52e110485bfbfea6e27270dec5f735e7318c24615db8ca8468569cff26af27188b171c86458bd1e58da578b05828a2a5b614961e43097445a94fb67fed
```

### `dpkg` source package: `python3-colcon-pkg-config=0.1.0-1`

Binary Packages:

- `python3-colcon-pkg-config=0.1.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-pkg-config=0.1.0-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-pkg-config/python3-colcon-pkg-config_0.1.0-1.debian.tar.xz' python3-colcon-pkg-config_0.1.0-1.debian.tar.xz 984 SHA512:98a9ffd7457c80c063489f04a73e69acc4725d936c11b0666b64f1ba71e8ee51ac5d3b2ba2692ca057c84a3d27ebe966f68ab39f8958c6e60bb9fbec5d8e24d6
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-pkg-config/python3-colcon-pkg-config_0.1.0-1.dsc' python3-colcon-pkg-config_0.1.0-1.dsc 1008 SHA512:d42b9ff2a0c59744a6e9dce84b4c9b02ad2982119c8100bad5ec7fd6811ac81e61198ac9d0b7c131a500189b0d2450e45576598930c8af60ad67ad895784f58d
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-pkg-config/python3-colcon-pkg-config_0.1.0.orig.tar.gz' python3-colcon-pkg-config_0.1.0.orig.tar.gz 3408 SHA512:0f6df04ed403172f4a4922b0edb504a67e82d30e24e159dacfc3700dbe59f11862bb5f62a34a359e8a05d368259912a77a9cfd6084093a4c99d65b50b07608e1
```

### `dpkg` source package: `python3-colcon-powershell=0.3.6-1`

Binary Packages:

- `python3-colcon-powershell=0.3.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-powershell=0.3.6-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-powershell/python3-colcon-powershell_0.3.6-1.debian.tar.xz' python3-colcon-powershell_0.3.6-1.debian.tar.xz 1080 SHA512:b83c16cb866b45a823911c874914cc3991b8ee71f53ac7dbf6ef9dc85731e23153fce635ffbc4aa0ac99e9497ac404051421d29883f54471c60c45ce0ac152a6
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-powershell/python3-colcon-powershell_0.3.6-1.dsc' python3-colcon-powershell_0.3.6-1.dsc 960 SHA512:1be2c8b3a7e03af2dd5fab9d5d813a3bce9363b14a8f1604db528f5c47643a2c88c9ab8783ccd5670b8c79d76b083e00fa2bed2cc181209da3e01ed6c37c2b15
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-powershell/python3-colcon-powershell_0.3.6.orig.tar.gz' python3-colcon-powershell_0.3.6.orig.tar.gz 7168 SHA512:577b764a08f75d195ec39d13df86cb3af79d4747c38a7d018d3999b2aee4a0ae5e83ae2a0280dc81f1a9efab938d1f4c38175a582bef028f4f5f61dca9a6c9d4
```

### `dpkg` source package: `python3-colcon-python-setup-py=0.2.7-2`

Binary Packages:

- `python3-colcon-python-setup-py=0.2.7-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-python-setup-py=0.2.7-2
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-python-setup-py/python3-colcon-python-setup-py_0.2.7-2.debian.tar.xz' python3-colcon-python-setup-py_0.2.7-2.debian.tar.xz 1164 SHA512:4f2001b6a50a47e0d17dfb06fe15db4750ef06e971d1a1cd3aeb703890351e16c23966f0389004f8122125dcc12cf0a72aef4d8c9574c7250a1c3d816ffb41b9
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-python-setup-py/python3-colcon-python-setup-py_0.2.7-2.dsc' python3-colcon-python-setup-py_0.2.7-2.dsc 1045 SHA512:6c240213e636fe7505b332c9a036734b1d878cd4f891260d0eb7302878dbfb5484ddbdcf8fa95ad4d026e5621f901cf7abf404591c6bd5a96459d839add6808c
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-python-setup-py/python3-colcon-python-setup-py_0.2.7.orig.tar.gz' python3-colcon-python-setup-py_0.2.7.orig.tar.gz 6579 SHA512:aab3a4c12c5dc2f5d76206597a7f8f73595862c501e545598a9b3380e0af3c2e1d201d1da97a97b7cdf318cbca224fc33adecc46b9107ec686a510288b49c725
```

### `dpkg` source package: `python3-colcon-recursive-crawl=0.2.1-1`

Binary Packages:

- `python3-colcon-recursive-crawl=0.2.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-recursive-crawl=0.2.1-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-recursive-crawl/python3-colcon-recursive-crawl_0.2.1-1.debian.tar.xz' python3-colcon-recursive-crawl_0.2.1-1.debian.tar.xz 1072 SHA512:aad1aafbd5ed8f2aa08bf79513c3c40929bafd4e10bbda2e1936a5a5a7e202b09b0beb81efdced49d80ab7aecba0e0bebf8489276636aef0798c4f7ddb23960d
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-recursive-crawl/python3-colcon-recursive-crawl_0.2.1-1.dsc' python3-colcon-recursive-crawl_0.2.1-1.dsc 1005 SHA512:763ecc90bdca9c57ba2fc15d22851071fdce0b92bb4b3b8c1b9bf5e25144417e86536b42ea04bcc7bccc68389cfd662da461ea1d6201cd138c386bd7fa6215b4
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-recursive-crawl/python3-colcon-recursive-crawl_0.2.1.orig.tar.gz' python3-colcon-recursive-crawl_0.2.1.orig.tar.gz 4100 SHA512:7af4783e49b1b59f961b710dd7dca307d169261d1a4d3d3e8538716905df01776dd8c806053f0d21996fb5f5f4c75a2c6e411a2538a7ccd17bf1eb3391ce7ea5
```

### `dpkg` source package: `python3-colcon-ros=0.3.21-2`

Binary Packages:

- `python3-colcon-ros=0.3.21-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-ros=0.3.21-2
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-ros/python3-colcon-ros_0.3.21-2.debian.tar.xz' python3-colcon-ros_0.3.21-2.debian.tar.xz 1580 SHA512:39d99de8881ae791200bf0d90e5ea56fd9f11c414bbe915264f97fce25ca5ea734fd3fc7fb883d30c6a25dcad744d0dad91129c1dbdd68294157633eea811270
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-ros/python3-colcon-ros_0.3.21-2.dsc' python3-colcon-ros_0.3.21-2.dsc 947 SHA512:8c599112cbcce8cb329d67509cbc771e360efcdf95470b6856649ff4ac0944ea65948d7516b8b64375c0560de72feed74d8b3e3e55a6d9d7457397aa63bb723b
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-ros/python3-colcon-ros_0.3.21.orig.tar.gz' python3-colcon-ros_0.3.21.orig.tar.gz 12800 SHA512:a5fcf9226ed753a100b5f71278758e775e1d62f92409d09fe083eb2ca4bcabf3cdf93ec847033db95493f9998d79d9c6122dbd4cfb72453e1ba6356558975ab2
```

### `dpkg` source package: `python3-colcon-test-result=0.3.8-1`

Binary Packages:

- `python3-colcon-test-result=0.3.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-test-result=0.3.8-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-test-result/python3-colcon-test-result_0.3.8-1.debian.tar.xz' python3-colcon-test-result_0.3.8-1.debian.tar.xz 1076 SHA512:a53a5a1415b08a053b783dd9052b601c316b0e277511c2b5f995baf51cf19011f535811efe8d066b68c57f133e44fc364a2d2bd02d5a3e15dcdad6d5fcd329b6
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-test-result/python3-colcon-test-result_0.3.8-1.dsc' python3-colcon-test-result_0.3.8-1.dsc 969 SHA512:44515222f5c096d7e076bbc9c6911316bd4d09b47402983e9d0b4a34eff440a37565a494930a28146fcd2404b0ee6e26c36c647d8dec9fce464d30acc3e6f86c
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-test-result/python3-colcon-test-result_0.3.8.orig.tar.gz' python3-colcon-test-result_0.3.8.orig.tar.gz 8075 SHA512:c54342d8cdbd71255510510a71bbbd29664469368553d133ecfd7f67cf04ccbc8e07fa25bc62474114450020a40b4271d7048a2382380d641bcf0f8e1445b8d6
```

### `dpkg` source package: `python3-colcon-zsh=0.4.0-1`

Binary Packages:

- `python3-colcon-zsh=0.4.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-colcon-zsh=0.4.0-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-zsh/python3-colcon-zsh_0.4.0-1.debian.tar.xz' python3-colcon-zsh_0.4.0-1.debian.tar.xz 1076 SHA512:3edcc749368472a4b77cb15cf8281286b11ed536254d7b4b40b08da33f703efa49ee997f8def1191e6df45f91d0ed61fdf00f69e7b3ac7d660c6e7c58b8cba1b
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-zsh/python3-colcon-zsh_0.4.0-1.dsc' python3-colcon-zsh_0.4.0-1.dsc 897 SHA512:1895a2b60e11448c282bb48a5cd98a66d1c8f655ffe3d7ad3b7e0b033daa902fbcad0c605b73c00a21d1e3ea0e9bf8cb04ecf25b0d16530e30c46e9d12829485
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-colcon-zsh/python3-colcon-zsh_0.4.0.orig.tar.gz' python3-colcon-zsh_0.4.0.orig.tar.gz 5654 SHA512:dafb711ecd6a8411147d592b064011efd8db4666e8cc8358243841f46cc3aa5427a7a56b1b7e4f71d27b5f88e401f4556d7d26e7af26074d83e68d9dfffae35a
```

### `dpkg` source package: `python3-defaults=3.9.7-4`

Binary Packages:

- `libpython3-dev:amd64=3.9.7-4`
- `libpython3-stdlib:amd64=3.9.7-4`
- `python3=3.9.7-4`
- `python3-dev=3.9.7-4`
- `python3-minimal=3.9.7-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.9.7-4
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.7-4.dsc' python3-defaults_3.9.7-4.dsc 2879 SHA512:f829f2fab4fdf387f38c8d93c62e0e8171c2fdb66ba11590084d8fcc4c1a725a297b58e20d9fcafb594be200c0ab230c440b8ac0101b52aaaeaf6d8ba9ab3726
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.9.7-4.tar.gz' python3-defaults_3.9.7-4.tar.gz 141201 SHA512:1fc07424053d519fdd3a72ee25a17307a38a929dddb5c37be2636eec1b872a43c517e91c07d7f774c3af51b5155358d5d291626510b47ac9d027255d43bc82e3
```

### `dpkg` source package: `python3-rosdep-modules=0.21.0-1`

Binary Packages:

- `python3-rosdep-modules=0.21.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rosdep-modules=0.21.0-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdep-modules/python3-rosdep-modules_0.21.0-1.debian.tar.xz' python3-rosdep-modules_0.21.0-1.debian.tar.xz 2064 SHA512:d7c63e69c11c84478ac8461a37493b47cb8720ddc74f2c9eb13bf64a8ca9db6731dbb03f0cb5a921210313738d4e94354601ce604d17df6b88d9c0a8ef71817f
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdep-modules/python3-rosdep-modules_0.21.0-1.dsc' python3-rosdep-modules_0.21.0-1.dsc 997 SHA512:fbc7deadb772bfa5c482c867e87e6146c3d0db6bdbcf5b50c71fb78eeeb1984ebbf4dfa065af5e82cad0a388ddcbb2581f1ddb26999647f9cd8030f225e0fc7d
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdep-modules/python3-rosdep-modules_0.21.0.orig.tar.gz' python3-rosdep-modules_0.21.0.orig.tar.gz 90044 SHA512:c3ec2896afa1b9617a9c66e7053334e8ce3324e3c41b305f6623fa117728688826e7107ed5b2239b1b55c845b67f1e5c926d543bf866191ec152d3f81d8af98a
```

### `dpkg` source package: `python3-rosdep=0.21.0-1`

Binary Packages:

- `python3-rosdep=0.21.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rosdep=0.21.0-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdep/python3-rosdep_0.21.0-1.debian.tar.xz' python3-rosdep_0.21.0-1.debian.tar.xz 2012 SHA512:fbef44632a55e90671a05f686f0ff8567af9ef99c5608b1807c360f101cfbc8b99e0b059fe564b2275020ed0fd4a2758d8a8af05f32dc670bdd1bcd45680b06d
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdep/python3-rosdep_0.21.0-1.dsc' python3-rosdep_0.21.0-1.dsc 925 SHA512:69fd963abefce0468a7b54c0b96ce6ed6fcde141fbb8703a037c09a7e5802777162662df266152c06e2faadc23c40e8f1dfb264bdeee587c6807c61886eb9caa
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdep/python3-rosdep_0.21.0.orig.tar.gz' python3-rosdep_0.21.0.orig.tar.gz 32255 SHA512:884b89d8de336a7c2d8db0707c97197517cb4fdb57dbeb819ea964bbeaa506ed7af3b04d83ca998de57e7efaf22322f78c30c80fe0ca838bb863631349b3603e
```

### `dpkg` source package: `python3-rosdistro-modules=0.8.3-1`

Binary Packages:

- `python3-rosdistro-modules=0.8.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rosdistro-modules=0.8.3-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdistro-modules/python3-rosdistro-modules_0.8.3-1.debian.tar.xz' python3-rosdistro-modules_0.8.3-1.debian.tar.xz 1988 SHA512:e49a29255db6e09432cef75a251ac970b9b39f0477b1cc7b98bc81cd852b9c925246890fc4efd8e49a971f6116e8ae8f0636c42aef31eea6017aaa0dd817b7a0
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdistro-modules/python3-rosdistro-modules_0.8.3-1.dsc' python3-rosdistro-modules_0.8.3-1.dsc 969 SHA512:db5c2fa5b081101bfae373665da88243f517e548e87e3639edce2e65b6e68d3a3879b60b7db5ef63452dd001517471cf5cf5820fcf8f407efc23775a5c888560
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdistro-modules/python3-rosdistro-modules_0.8.3.orig.tar.gz' python3-rosdistro-modules_0.8.3.orig.tar.gz 44498 SHA512:824b76a2bc35767e49c2d3046c18e0e6f45000d2a27c95020cd72c941fd4331a12193507cd4a641f33f801621a6e3ecff7bf6c22f979d7c293273dc22697bd49
```

### `dpkg` source package: `python3-rosdistro=0.8.3-100`

Binary Packages:

- `python3-rosdistro=0.8.3-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rosdistro=0.8.3-100
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdistro/python3-rosdistro_0.8.3-100.debian.tar.xz' python3-rosdistro_0.8.3-100.debian.tar.xz 1972 SHA512:ded23ea58ca452f4f9fddf7583d1b943ef961496a77c6257214a69fefed7ac1232dc79bb701fb9454dc924c4f4dee8a698e2f813e71519649d573dac9913e3ef
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdistro/python3-rosdistro_0.8.3-100.dsc' python3-rosdistro_0.8.3-100.dsc 909 SHA512:cdb9a09c1659154cde6d4b287f3fd814c3c16fef80142b44ee875c08605e8f47a93a90536bab5004ced6611d110f62a447d9f7ad7c527cdc04021c92339a0cd8
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rosdistro/python3-rosdistro_0.8.3.orig.tar.gz' python3-rosdistro_0.8.3.orig.tar.gz 10568 SHA512:153e0880576d0ac8ccb56cb18a4f08fb1cf14d987fa376e64c0df62f4e067486e5e925dac11d315e13f4e9714a72945d1596be27b6cf43fdb4f2ebe214bf0b64
```

### `dpkg` source package: `python3-rospkg-modules=1.4.0-1`

Binary Packages:

- `python3-rospkg-modules=1.4.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rospkg-modules=1.4.0-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rospkg-modules/python3-rospkg-modules_1.4.0-1.debian.tar.xz' python3-rospkg-modules_1.4.0-1.debian.tar.xz 1168 SHA512:8a17ebdfedf766ae6043759606e19126f8cfec3d93eb28162a316b0a5d64e98d52acdd47d599e1e3625015caacdc4f0f32c51484d783389919e6f8ce6ca5c18b
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rospkg-modules/python3-rospkg-modules_1.4.0-1.dsc' python3-rospkg-modules_1.4.0-1.dsc 973 SHA512:b309e62c393e33076bc010c275da1c51e4fed2c5531d423b9596e54cf478fffb8abeb501d93f48b0f5e98e8f1b036155ee7495f3f03ebb35b7f57deef6fdcfcc
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rospkg-modules/python3-rospkg-modules_1.4.0.orig.tar.gz' python3-rospkg-modules_1.4.0.orig.tar.gz 41508 SHA512:f8e5fd41d03cfb6d675fcd6a2735a7d38dda6a7b94eec140b9c3b31a6db385c86d35ac13cce39539abc6d41f567de454a9c3304f058edcba66ddb816237e69ba
```

### `dpkg` source package: `python3-rospkg=1.4.0-100`

Binary Packages:

- `python3-rospkg=1.4.0-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rospkg=1.4.0-100
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rospkg/python3-rospkg_1.4.0-100.debian.tar.xz' python3-rospkg_1.4.0-100.debian.tar.xz 1116 SHA512:68afea29b9ef8117dea12fbc8784566951db3486781634346d56db58f2499dd90f44b227b4c2b8aed51f7c0def479b149cb8b15c0b584b10998f50e05ffbdc19
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rospkg/python3-rospkg_1.4.0-100.dsc' python3-rospkg_1.4.0-100.dsc 909 SHA512:34d61923077ff52372d23b64ac5a55250610a8a56f47ed67b4f666692d6a82b4e57664a4ec5fa469b8d5b66a41467f7b18182896ad174e4aaff0e918ac5528f7
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-rospkg/python3-rospkg_1.4.0.orig.tar.gz' python3-rospkg_1.4.0.orig.tar.gz 17487 SHA512:428b80a839c1e998f0b3a8601f9ae10339752f26870a6acae9c871e692fd514ccf12b261b9f54bf87b39c6d676c0771a5e2c24291d6ce90227b8874d251e785d
```

### `dpkg` source package: `python3-stdlib-extensions=3.9.10-1`

Binary Packages:

- `python3-distutils=3.9.10-1`
- `python3-lib2to3=3.9.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.9.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.9.10-1.dsc' python3-stdlib-extensions_3.9.10-1.dsc 2571 SHA512:7064d5d7c58247d74b0497c9f3d792e672ad27f27a08de918c9acaebd6189a6a30276390fb86e6ded87b8319c94bd8939f4de2bc75d860b66dd2d0a96e07e04f
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.9.10.orig.tar.xz' python3-stdlib-extensions_3.9.10.orig.tar.xz 1113008 SHA512:6a334816defc3c3e98045d7e8adb1d3f9bf96a14e5151a6174900247aba8cc9ec6b8ce15ec02bf39986584512d1aac2caf36e654c52ffdbbe33125b9c01b24e5
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.9.10-1.debian.tar.xz' python3-stdlib-extensions_3.9.10-1.debian.tar.xz 24812 SHA512:16a36677a36e14b3ab928733df6bd40c4d238dffd4dab15f92e4b2db468d666768927d0a1507dc21c18286461d1eb22ad5d0e7fb606002e1e5a2a09e0a7305de
```

### `dpkg` source package: `python3-vcstool=0.3.0-1`

Binary Packages:

- `python3-vcstool=0.3.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-vcstool=0.3.0-1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-vcstool/python3-vcstool_0.3.0-1.debian.tar.xz' python3-vcstool_0.3.0-1.debian.tar.xz 1088 SHA512:232b57da7b9bea2db8f160af72efe776658bb119781c4a4d44643302f9c73a600c4d677ae14eb93a649c87558182b257679d906f39d823020015d830bf1587b1
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-vcstool/python3-vcstool_0.3.0-1.dsc' python3-vcstool_0.3.0-1.dsc 922 SHA512:21f0b2dd3e28dccee6157b70b9a88b83c7f972f4e108147f30b4e93fbe67d8aea5a1d3eb0227550b8dd61feb002e38e8e76f48da052a87f964a704241cfbbc08
'http://packages.ros.org/ros2/ubuntu/pool/main/p/python3-vcstool/python3-vcstool_0.3.0.orig.tar.gz' python3-vcstool_0.3.0.orig.tar.gz 35587 SHA512:4272b2562448c89a64a2e746c2b0ed682daf7fdc361c18d4d0a8cced525acf3fa919b8c4b12f013e243cdece77aca0de08c88d9b89071e736fe98ce2c3108632
```

### `dpkg` source package: `python3.10=3.10.2-1`

Binary Packages:

- `libpython3.10-minimal:amd64=3.10.2-1`
- `libpython3.10-stdlib:amd64=3.10.2-1`
- `python3.10=3.10.2-1`
- `python3.10-minimal=3.10.2-1`

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

- http://snapshot.debian.org/package/python3.10/3.10.2-1/


### `dpkg` source package: `python3.9=3.9.10-2`

Binary Packages:

- `libpython3.9:amd64=3.9.10-2`
- `libpython3.9-dev:amd64=3.9.10-2`
- `libpython3.9-minimal:amd64=3.9.10-2`
- `libpython3.9-stdlib:amd64=3.9.10-2`
- `python3.9=3.9.10-2`
- `python3.9-dev=3.9.10-2`
- `python3.9-minimal=3.9.10-2`

Licenses: (parsed from: `/usr/share/doc/libpython3.9/copyright`, `/usr/share/doc/libpython3.9-dev/copyright`, `/usr/share/doc/libpython3.9-minimal/copyright`, `/usr/share/doc/libpython3.9-stdlib/copyright`, `/usr/share/doc/python3.9/copyright`, `/usr/share/doc/python3.9-dev/copyright`, `/usr/share/doc/python3.9-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.9=3.9.10-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.10-2.dsc' python3.9_3.9.10-2.dsc 3500 SHA512:6120dae7c3f21469ae25ca23e85fc8ec0374901675e31fa5e5e2f5149ee779a0df003aea97496e0c0d3fec2798517616ca510a4ca7989aa45945b83ce77f33f2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.10.orig.tar.xz' python3.9_3.9.10.orig.tar.xz 19154136 SHA512:09cb942f84bf362df88999ffa6faf89b4ad12302e67cda4a11547828ebe410c7c93a3dc96cd66fd9c5c7d9a1abe5b8e259e7ec47c10273b42d212270aca5ecba
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.9/python3.9_3.9.10-2.debian.tar.xz' python3.9_3.9.10-2.debian.tar.xz 213192 SHA512:d910f0781c73cad710fd7e9adabb7d189368529b4dc4a77fac120ec7a52c98418c22633fc00de7abc472a903008076a648d1a7e6af2105cc51962b87d205b090
```

### `dpkg` source package: `pyyaml=5.4.1-1`

Binary Packages:

- `python3-yaml=5.4.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pyyaml=5.4.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_5.4.1-1.dsc' pyyaml_5.4.1-1.dsc 2085 SHA512:f6e92270b51d829e67c7b0c01273a8203e0f3e6b9bbe1d7e3c2fcc6f1d029565151e44802e48b9cd875430224a1fcbfef8c4c9defd15a304f79d1463321997db
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_5.4.1.orig.tar.gz' pyyaml_5.4.1.orig.tar.gz 175147 SHA512:359c45d843fd839797572efeab121f17b1947647960dfb062f3618f25f71e1a6bc4bab14a1720b6b67f256089d5d48c452ec5419e3130222765c7ca41db11dad
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_5.4.1-1.debian.tar.xz' pyyaml_5.4.1-1.debian.tar.xz 7352 SHA512:2852e419a0acee5615ff9ee7519bfebcd2873f22f44fcb16edc1287accc0438032ce08d03540c15c3d2ec377b87a75b2ed54e3dbe4eb44774c5e4118aca977d6
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

### `dpkg` source package: `rhash=1.4.2-1build1`

Binary Packages:

- `librhash0:amd64=1.4.2-1build1`

Licenses: (parsed from: `/usr/share/doc/librhash0/copyright`)

- `0BSD`

Source:

```console
$ apt-get source -qq --print-uris rhash=1.4.2-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.4.2-1build1.dsc' rhash_1.4.2-1build1.dsc 2324 SHA512:a62b5a56fa4c3d090c554e5fe6d5b9022ea74da312843faf0f3bd277620177ba3f360797dac02eacaa6e14cd031f861851db56d07d51d2e2317ae706892de1ae
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.4.2.orig.tar.gz' rhash_1.4.2.orig.tar.gz 416853 SHA512:41df57e8b3f32c93d8e6f2ac668b32aaa23eb2eaf90a83f109e61e511404a5036ea88bcf2854e19c1ade0f61960e0d9edf01f3d82e1c645fed36579e9d7a6a25
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.4.2.orig.tar.gz.asc' rhash_1.4.2.orig.tar.gz.asc 833 SHA512:a61a0a10a8b5affd69b8e8b9856137eee6ce922ee369e5b5a673edec921201771646412da083679696e7732e4954f9a4205ecfbe1c09b02871de4930b68f0015
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.4.2-1build1.debian.tar.xz' rhash_1.4.2-1build1.debian.tar.xz 9964 SHA512:db4701e1f3b74923bca66a4f8db2519035480d27eb0e464db28ac1fec541ee1af7c9b7e97b63e36855c144bfe05ccb1c4d4e9451f15675c1a0cf436171ccf943
```

### `dpkg` source package: `ros-rolling-action-msgs=1.1.0-2jammy.20220219.164521`

Binary Packages:

- `ros-rolling-action-msgs=1.1.0-2jammy.20220219.164521`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-actionlib-msgs=4.0.0-2jammy.20220219.164646`

Binary Packages:

- `ros-rolling-actionlib-msgs=4.0.0-2jammy.20220219.164646`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-auto=1.3.0-2jammy.20220218.161601`

Binary Packages:

- `ros-rolling-ament-cmake-auto=1.3.0-2jammy.20220218.161601`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-copyright=0.12.0-1jammy.20220218.214222`

Binary Packages:

- `ros-rolling-ament-cmake-copyright=0.12.0-1jammy.20220218.214222`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-core=1.3.0-2jammy.20220218.152613`

Binary Packages:

- `ros-rolling-ament-cmake-core=1.3.0-2jammy.20220218.152613`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-cppcheck=0.12.0-1jammy.20220218.214712`

Binary Packages:

- `ros-rolling-ament-cmake-cppcheck=0.12.0-1jammy.20220218.214712`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-cpplint=0.12.0-1jammy.20220218.214750`

Binary Packages:

- `ros-rolling-ament-cmake-cpplint=0.12.0-1jammy.20220218.214750`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-export-definitions=1.3.0-2jammy.20220218.154359`

Binary Packages:

- `ros-rolling-ament-cmake-export-definitions=1.3.0-2jammy.20220218.154359`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-export-dependencies=1.3.0-2jammy.20220218.155301`

Binary Packages:

- `ros-rolling-ament-cmake-export-dependencies=1.3.0-2jammy.20220218.155301`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-export-include-directories=1.3.0-2jammy.20220218.154544`

Binary Packages:

- `ros-rolling-ament-cmake-export-include-directories=1.3.0-2jammy.20220218.154544`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-export-interfaces=1.3.0-2jammy.20220218.155254`

Binary Packages:

- `ros-rolling-ament-cmake-export-interfaces=1.3.0-2jammy.20220218.155254`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-export-libraries=1.3.0-2jammy.20220218.154146`

Binary Packages:

- `ros-rolling-ament-cmake-export-libraries=1.3.0-2jammy.20220218.154146`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-export-link-flags=1.3.0-2jammy.20220218.154312`

Binary Packages:

- `ros-rolling-ament-cmake-export-link-flags=1.3.0-2jammy.20220218.154312`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-export-targets=1.3.0-2jammy.20220218.155257`

Binary Packages:

- `ros-rolling-ament-cmake-export-targets=1.3.0-2jammy.20220218.155257`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-flake8=0.12.0-1jammy.20220218.214750`

Binary Packages:

- `ros-rolling-ament-cmake-flake8=0.12.0-1jammy.20220218.214750`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-gen-version-h=1.3.0-2jammy.20220218.155546`

Binary Packages:

- `ros-rolling-ament-cmake-gen-version-h=1.3.0-2jammy.20220218.155546`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-gmock=1.3.0-2jammy.20220218.155545`

Binary Packages:

- `ros-rolling-ament-cmake-gmock=1.3.0-2jammy.20220218.155545`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-gtest=1.3.0-2jammy.20220218.155504`

Binary Packages:

- `ros-rolling-ament-cmake-gtest=1.3.0-2jammy.20220218.155504`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-include-directories=1.3.0-2jammy.20220218.153952`

Binary Packages:

- `ros-rolling-ament-cmake-include-directories=1.3.0-2jammy.20220218.153952`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-libraries=1.3.0-2jammy.20220218.154208`

Binary Packages:

- `ros-rolling-ament-cmake-libraries=1.3.0-2jammy.20220218.154208`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-lint-cmake=0.12.0-1jammy.20220218.213912`

Binary Packages:

- `ros-rolling-ament-cmake-lint-cmake=0.12.0-1jammy.20220218.213912`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-pep257=0.12.0-1jammy.20220218.214514`

Binary Packages:

- `ros-rolling-ament-cmake-pep257=0.12.0-1jammy.20220218.214514`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-pytest=1.3.0-2jammy.20220218.155502`

Binary Packages:

- `ros-rolling-ament-cmake-pytest=1.3.0-2jammy.20220218.155502`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-python=1.3.0-2jammy.20220218.154623`

Binary Packages:

- `ros-rolling-ament-cmake-python=1.3.0-2jammy.20220218.154623`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-ros=0.10.0-2jammy.20220218.223719`

Binary Packages:

- `ros-rolling-ament-cmake-ros=0.10.0-2jammy.20220218.223719`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-target-dependencies=1.3.0-2jammy.20220218.155303`

Binary Packages:

- `ros-rolling-ament-cmake-target-dependencies=1.3.0-2jammy.20220218.155303`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-test=1.3.0-2jammy.20220218.155333`

Binary Packages:

- `ros-rolling-ament-cmake-test=1.3.0-2jammy.20220218.155333`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-uncrustify=0.12.0-1jammy.20220218.220458`

Binary Packages:

- `ros-rolling-ament-cmake-uncrustify=0.12.0-1jammy.20220218.220458`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-version=1.3.0-2jammy.20220218.154149`

Binary Packages:

- `ros-rolling-ament-cmake-version=1.3.0-2jammy.20220218.154149`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake-xmllint=0.12.0-1jammy.20220218.214756`

Binary Packages:

- `ros-rolling-ament-cmake-xmllint=0.12.0-1jammy.20220218.214756`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cmake=1.3.0-2jammy.20220218.155909`

Binary Packages:

- `ros-rolling-ament-cmake=1.3.0-2jammy.20220218.155909`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-copyright=0.12.0-1jammy.20220218.213432`

Binary Packages:

- `ros-rolling-ament-copyright=0.12.0-1jammy.20220218.213432`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cppcheck=0.12.0-1jammy.20220218.210127`

Binary Packages:

- `ros-rolling-ament-cppcheck=0.12.0-1jammy.20220218.210127`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-cpplint=0.12.0-1jammy.20220218.213648`

Binary Packages:

- `ros-rolling-ament-cpplint=0.12.0-1jammy.20220218.213648`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-flake8=0.12.0-1jammy.20220218.212013`

Binary Packages:

- `ros-rolling-ament-flake8=0.12.0-1jammy.20220218.212013`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-index-cpp=1.3.0-2jammy.20220218.223740`

Binary Packages:

- `ros-rolling-ament-index-cpp=1.3.0-2jammy.20220218.223740`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-index-python=1.3.0-2jammy.20220218.213942`

Binary Packages:

- `ros-rolling-ament-index-python=1.3.0-2jammy.20220218.213942`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-lint-auto=0.12.0-1jammy.20220218.210255`

Binary Packages:

- `ros-rolling-ament-lint-auto=0.12.0-1jammy.20220218.210255`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-lint-cmake=0.12.0-1jammy.20220218.213647`

Binary Packages:

- `ros-rolling-ament-lint-cmake=0.12.0-1jammy.20220218.213647`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-lint-common=0.12.0-1jammy.20220218.222622`

Binary Packages:

- `ros-rolling-ament-lint-common=0.12.0-1jammy.20220218.222622`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-lint=0.12.0-1jammy.20220218.210210`

Binary Packages:

- `ros-rolling-ament-lint=0.12.0-1jammy.20220218.210210`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-package=0.14.0-2jammy.20220210.172131`

Binary Packages:

- `ros-rolling-ament-package=0.14.0-2jammy.20220210.172131`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-pep257=0.12.0-1jammy.20220218.212854`

Binary Packages:

- `ros-rolling-ament-pep257=0.12.0-1jammy.20220218.212854`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-uncrustify=0.12.0-1jammy.20220218.213908`

Binary Packages:

- `ros-rolling-ament-uncrustify=0.12.0-1jammy.20220218.213908`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ament-xmllint=0.12.0-1jammy.20220218.213649`

Binary Packages:

- `ros-rolling-ament-xmllint=0.12.0-1jammy.20220218.213649`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-builtin-interfaces=1.1.0-2jammy.20220219.162624`

Binary Packages:

- `ros-rolling-builtin-interfaces=1.1.0-2jammy.20220219.162624`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-class-loader=2.2.0-2jammy.20220218.233051`

Binary Packages:

- `ros-rolling-class-loader=2.2.0-2jammy.20220218.233051`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-common-interfaces=4.0.0-2jammy.20220219.171302`

Binary Packages:

- `ros-rolling-common-interfaces=4.0.0-2jammy.20220219.171302`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-composition-interfaces=1.1.0-2jammy.20220219.165024`

Binary Packages:

- `ros-rolling-composition-interfaces=1.1.0-2jammy.20220219.165024`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-console-bridge-vendor=1.3.2-2jammy.20220218.224809`

Binary Packages:

- `ros-rolling-console-bridge-vendor=1.3.2-2jammy.20220218.224809`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-cyclonedds=0.8.2-1jammy.20220218.162406`

Binary Packages:

- `ros-rolling-cyclonedds=0.8.2-1jammy.20220218.162406`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-diagnostic-msgs=4.0.0-2jammy.20220219.165922`

Binary Packages:

- `ros-rolling-diagnostic-msgs=4.0.0-2jammy.20220219.165922`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-domain-coordinator=0.10.0-2jammy.20220218.213650`

Binary Packages:

- `ros-rolling-domain-coordinator=0.10.0-2jammy.20220218.213650`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-eigen3-cmake-module=0.1.1-3jammy.20220218.220624`

Binary Packages:

- `ros-rolling-eigen3-cmake-module=0.1.1-3jammy.20220218.220624`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-fastcdr=1.0.20-3jammy.20220218.155247`

Binary Packages:

- `ros-rolling-fastcdr=1.0.20-3jammy.20220218.155247`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-geometry-msgs=4.0.0-2jammy.20220219.165225`

Binary Packages:

- `ros-rolling-geometry-msgs=4.0.0-2jammy.20220219.165225`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-geometry2=0.21.0-2jammy.20220219.183054`

Binary Packages:

- `ros-rolling-geometry2=0.21.0-2jammy.20220219.183054`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-gmock-vendor=1.10.9004-3jammy.20220218.155411`

Binary Packages:

- `ros-rolling-gmock-vendor=1.10.9004-3jammy.20220218.155411`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-gtest-vendor=1.10.9004-3jammy.20220218.155205`

Binary Packages:

- `ros-rolling-gtest-vendor=1.10.9004-3jammy.20220218.155205`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-iceoryx-binding-c=1.0.2-2jammy.20220218.161425`

Binary Packages:

- `ros-rolling-iceoryx-binding-c=1.0.2-2jammy.20220218.161425`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-iceoryx-posh=1.0.2-2jammy.20220218.155817`

Binary Packages:

- `ros-rolling-iceoryx-posh=1.0.2-2jammy.20220218.155817`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-iceoryx-utils=1.0.2-2jammy.20220218.155328`

Binary Packages:

- `ros-rolling-iceoryx-utils=1.0.2-2jammy.20220218.155328`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-kdl-parser=2.6.1-2jammy.20220219.002558`

Binary Packages:

- `ros-rolling-kdl-parser=2.6.1-2jammy.20220219.002558`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-keyboard-handler=0.0.3-3jammy.20220218.223655`

Binary Packages:

- `ros-rolling-keyboard-handler=0.0.3-3jammy.20220218.223655`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-launch-ros=0.17.0-2jammy.20220219.172726`

Binary Packages:

- `ros-rolling-launch-ros=0.17.0-2jammy.20220219.172726`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-launch-testing-ament-cmake=0.21.0-2jammy.20220218.223702`

Binary Packages:

- `ros-rolling-launch-testing-ament-cmake=0.21.0-2jammy.20220218.223702`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-launch-testing-ros=0.17.0-2jammy.20220219.172941`

Binary Packages:

- `ros-rolling-launch-testing-ros=0.17.0-2jammy.20220219.172941`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-launch-testing=0.21.0-2jammy.20220218.220912`

Binary Packages:

- `ros-rolling-launch-testing=0.21.0-2jammy.20220218.220912`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-launch-xml=0.21.0-2jammy.20220218.215017`

Binary Packages:

- `ros-rolling-launch-xml=0.21.0-2jammy.20220218.215017`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-launch-yaml=0.21.0-2jammy.20220218.215959`

Binary Packages:

- `ros-rolling-launch-yaml=0.21.0-2jammy.20220218.215959`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-launch=0.21.0-2jammy.20220218.214501`

Binary Packages:

- `ros-rolling-launch=0.21.0-2jammy.20220218.214501`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-libstatistics-collector=1.1.0-3jammy.20220219.171505`

Binary Packages:

- `ros-rolling-libstatistics-collector=1.1.0-3jammy.20220219.171505`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-libyaml-vendor=1.2.0-2jammy.20220218.233054`

Binary Packages:

- `ros-rolling-libyaml-vendor=1.2.0-2jammy.20220218.233054`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-lifecycle-msgs=1.1.0-2jammy.20220219.162607`

Binary Packages:

- `ros-rolling-lifecycle-msgs=1.1.0-2jammy.20220219.162607`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-message-filters=4.2.0-2jammy.20220219.180956`

Binary Packages:

- `ros-rolling-message-filters=4.2.0-2jammy.20220219.180956`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-nav-msgs=4.0.0-2jammy.20220219.170033`

Binary Packages:

- `ros-rolling-nav-msgs=4.0.0-2jammy.20220219.170033`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-orocos-kdl=3.3.3-2jammy.20220218.222624`

Binary Packages:

- `ros-rolling-orocos-kdl=3.3.3-2jammy.20220218.222624`

Licenses: (parsed from: `/usr/share/doc/ros-rolling-orocos-kdl/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-osrf-pycommon=1.0.1-2jammy.20220218.155347`

Binary Packages:

- `ros-rolling-osrf-pycommon=1.0.1-2jammy.20220218.155347`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-pluginlib=5.1.0-2jammy.20220218.234001`

Binary Packages:

- `ros-rolling-pluginlib=5.1.0-2jammy.20220218.234001`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-pybind11-vendor=2.3.0-2jammy.20220218.163124`

Binary Packages:

- `ros-rolling-pybind11-vendor=2.3.0-2jammy.20220218.163124`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-python-cmake-module=0.8.1-2jammy.20220218.223426`

Binary Packages:

- `ros-rolling-python-cmake-module=0.8.1-2jammy.20220218.223426`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcl-action=5.0.1-2jammy.20220219.171516`

Binary Packages:

- `ros-rolling-rcl-action=5.0.1-2jammy.20220219.171516`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcl-interfaces=1.1.0-2jammy.20220219.164500`

Binary Packages:

- `ros-rolling-rcl-interfaces=1.1.0-2jammy.20220219.164500`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcl-lifecycle=5.0.1-2jammy.20220219.171504`

Binary Packages:

- `ros-rolling-rcl-lifecycle=5.0.1-2jammy.20220219.171504`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcl-logging-interface=2.2.1-2jammy.20220218.233051`

Binary Packages:

- `ros-rolling-rcl-logging-interface=2.2.1-2jammy.20220218.233051`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcl-logging-spdlog=2.2.1-2jammy.20220218.233921`

Binary Packages:

- `ros-rolling-rcl-logging-spdlog=2.2.1-2jammy.20220218.233921`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcl-yaml-param-parser=5.0.1-2jammy.20220219.143043`

Binary Packages:

- `ros-rolling-rcl-yaml-param-parser=5.0.1-2jammy.20220219.143043`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcl=5.0.1-2jammy.20220219.170638`

Binary Packages:

- `ros-rolling-rcl=5.0.1-2jammy.20220219.170638`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rclcpp-action=15.0.0-2jammy.20220219.180420`

Binary Packages:

- `ros-rolling-rclcpp-action=15.0.0-2jammy.20220219.180420`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rclcpp-components=15.0.0-2jammy.20220219.180416`

Binary Packages:

- `ros-rolling-rclcpp-components=15.0.0-2jammy.20220219.180416`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rclcpp-lifecycle=15.0.0-2jammy.20220219.180456`

Binary Packages:

- `ros-rolling-rclcpp-lifecycle=15.0.0-2jammy.20220219.180456`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rclcpp=15.0.0-2jammy.20220219.172254`

Binary Packages:

- `ros-rolling-rclcpp=15.0.0-2jammy.20220219.172254`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rclpy=3.2.1-2jammy.20220219.172259`

Binary Packages:

- `ros-rolling-rclpy=3.2.1-2jammy.20220219.172259`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcpputils=2.3.2-2jammy.20220218.230658`

Binary Packages:

- `ros-rolling-rcpputils=2.3.2-2jammy.20220218.230658`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rcutils=5.0.1-2jammy.20220218.225333`

Binary Packages:

- `ros-rolling-rcutils=5.0.1-2jammy.20220218.225333`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rmw-cyclonedds-cpp=1.1.2-2jammy.20220219.163404`

Binary Packages:

- `ros-rolling-rmw-cyclonedds-cpp=1.1.2-2jammy.20220219.163404`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rmw-dds-common=1.4.1-2jammy.20220219.162624`

Binary Packages:

- `ros-rolling-rmw-dds-common=1.4.1-2jammy.20220219.162624`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rmw-implementation-cmake=5.1.0-3jammy.20220218.223436`

Binary Packages:

- `ros-rolling-rmw-implementation-cmake=5.1.0-3jammy.20220218.223436`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rmw-implementation=2.7.1-3jammy.20220219.170254`

Binary Packages:

- `ros-rolling-rmw-implementation=2.7.1-3jammy.20220219.170254`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rmw=5.1.0-3jammy.20220219.140811`

Binary Packages:

- `ros-rolling-rmw=5.1.0-3jammy.20220219.140811`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-robot-state-publisher=3.0.0-2jammy.20220219.182429`

Binary Packages:

- `ros-rolling-robot-state-publisher=3.0.0-2jammy.20220219.182429`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros-base=0.9.3-2jammy.20220219.190558`

Binary Packages:

- `ros-rolling-ros-base=0.9.3-2jammy.20220219.190558`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros-core=0.9.3-2jammy.20220219.182937`

Binary Packages:

- `ros-rolling-ros-core=0.9.3-2jammy.20220219.182937`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros-environment=3.2.0-2jammy.20220218.154228`

Binary Packages:

- `ros-rolling-ros-environment=3.2.0-2jammy.20220218.154228`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros-workspace=1.0.2-3jammy.20220218.152856`

Binary Packages:

- `ros-rolling-ros-workspace=1.0.2-3jammy.20220218.152856`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2action=0.17.1-2jammy.20220219.173120`

Binary Packages:

- `ros-rolling-ros2action=0.17.1-2jammy.20220219.173120`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2bag=0.13.0-3jammy.20220219.185928`

Binary Packages:

- `ros-rolling-ros2bag=0.13.0-3jammy.20220219.185928`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2cli-common-extensions=0.1.1-3jammy.20220219.182849`

Binary Packages:

- `ros-rolling-ros2cli-common-extensions=0.1.1-3jammy.20220219.182849`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2cli=0.17.1-2jammy.20220219.172905`

Binary Packages:

- `ros-rolling-ros2cli=0.17.1-2jammy.20220219.172905`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2component=0.17.1-2jammy.20220219.181438`

Binary Packages:

- `ros-rolling-ros2component=0.17.1-2jammy.20220219.181438`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2doctor=0.17.1-2jammy.20220219.173128`

Binary Packages:

- `ros-rolling-ros2doctor=0.17.1-2jammy.20220219.173128`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2interface=0.17.1-2jammy.20220219.173224`

Binary Packages:

- `ros-rolling-ros2interface=0.17.1-2jammy.20220219.173224`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2launch=0.17.0-2jammy.20220219.173719`

Binary Packages:

- `ros-rolling-ros2launch=0.17.0-2jammy.20220219.173719`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2lifecycle=0.17.1-2jammy.20220219.182153`

Binary Packages:

- `ros-rolling-ros2lifecycle=0.17.1-2jammy.20220219.182153`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2multicast=0.17.1-2jammy.20220219.173058`

Binary Packages:

- `ros-rolling-ros2multicast=0.17.1-2jammy.20220219.173058`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2node=0.17.1-2jammy.20220219.173229`

Binary Packages:

- `ros-rolling-ros2node=0.17.1-2jammy.20220219.173229`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2param=0.17.1-2jammy.20220219.173651`

Binary Packages:

- `ros-rolling-ros2param=0.17.1-2jammy.20220219.173651`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2pkg=0.17.1-2jammy.20220219.173323`

Binary Packages:

- `ros-rolling-ros2pkg=0.17.1-2jammy.20220219.173323`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2run=0.17.1-2jammy.20220219.173722`

Binary Packages:

- `ros-rolling-ros2run=0.17.1-2jammy.20220219.173722`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2service=0.17.1-2jammy.20220219.173302`

Binary Packages:

- `ros-rolling-ros2service=0.17.1-2jammy.20220219.173302`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-ros2topic=0.17.1-2jammy.20220219.173135`

Binary Packages:

- `ros-rolling-ros2topic=0.17.1-2jammy.20220219.173135`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-compression-zstd=0.13.0-3jammy.20220219.183636`

Binary Packages:

- `ros-rolling-rosbag2-compression-zstd=0.13.0-3jammy.20220219.183636`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-compression=0.13.0-3jammy.20220219.183231`

Binary Packages:

- `ros-rolling-rosbag2-compression=0.13.0-3jammy.20220219.183231`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-cpp=0.13.0-3jammy.20220219.182330`

Binary Packages:

- `ros-rolling-rosbag2-cpp=0.13.0-3jammy.20220219.182330`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-interfaces=0.13.0-3jammy.20220219.164543`

Binary Packages:

- `ros-rolling-rosbag2-interfaces=0.13.0-3jammy.20220219.164543`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-py=0.13.0-3jammy.20220219.185225`

Binary Packages:

- `ros-rolling-rosbag2-py=0.13.0-3jammy.20220219.185225`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-storage-default-plugins=0.13.0-3jammy.20220219.182002`

Binary Packages:

- `ros-rolling-rosbag2-storage-default-plugins=0.13.0-3jammy.20220219.182002`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-storage=0.13.0-3jammy.20220219.180707`

Binary Packages:

- `ros-rolling-rosbag2-storage=0.13.0-3jammy.20220219.180707`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2-transport=0.13.0-3jammy.20220219.183913`

Binary Packages:

- `ros-rolling-rosbag2-transport=0.13.0-3jammy.20220219.183913`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosbag2=0.13.0-3jammy.20220219.190438`

Binary Packages:

- `ros-rolling-rosbag2=0.13.0-3jammy.20220219.190438`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosgraph-msgs=1.1.0-2jammy.20220219.163324`

Binary Packages:

- `ros-rolling-rosgraph-msgs=1.1.0-2jammy.20220219.163324`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-adapter=3.0.1-2jammy.20220218.223428`

Binary Packages:

- `ros-rolling-rosidl-adapter=3.0.1-2jammy.20220218.223428`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-cli=3.0.1-2jammy.20220218.214229`

Binary Packages:

- `ros-rolling-rosidl-cli=3.0.1-2jammy.20220218.214229`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-cmake=3.0.1-2jammy.20220218.224003`

Binary Packages:

- `ros-rolling-rosidl-cmake=3.0.1-2jammy.20220218.224003`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-default-generators=1.1.1-2jammy.20220219.154817`

Binary Packages:

- `ros-rolling-rosidl-default-generators=1.1.1-2jammy.20220219.154817`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-default-runtime=1.1.1-2jammy.20220219.155251`

Binary Packages:

- `ros-rolling-rosidl-default-runtime=1.1.1-2jammy.20220219.155251`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-generator-c=3.0.1-2jammy.20220218.233148`

Binary Packages:

- `ros-rolling-rosidl-generator-c=3.0.1-2jammy.20220218.233148`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-generator-cpp=3.0.1-2jammy.20220219.000740`

Binary Packages:

- `ros-rolling-rosidl-generator-cpp=3.0.1-2jammy.20220219.000740`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-generator-py=0.14.1-2jammy.20220219.150527`

Binary Packages:

- `ros-rolling-rosidl-generator-py=0.14.1-2jammy.20220219.150527`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-parser=3.0.1-2jammy.20220218.223726`

Binary Packages:

- `ros-rolling-rosidl-parser=3.0.1-2jammy.20220218.223726`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-runtime-c=3.0.1-2jammy.20220218.230908`

Binary Packages:

- `ros-rolling-rosidl-runtime-c=3.0.1-2jammy.20220218.230908`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-runtime-cpp=3.0.1-2jammy.20220218.224813`

Binary Packages:

- `ros-rolling-rosidl-runtime-cpp=3.0.1-2jammy.20220218.224813`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-runtime-py=0.9.1-2jammy.20220219.165922`

Binary Packages:

- `ros-rolling-rosidl-runtime-py=0.9.1-2jammy.20220219.165922`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-typesupport-c=1.4.2-3jammy.20220218.233751`

Binary Packages:

- `ros-rolling-rosidl-typesupport-c=1.4.2-3jammy.20220218.233751`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-typesupport-cpp=1.4.2-3jammy.20220218.234334`

Binary Packages:

- `ros-rolling-rosidl-typesupport-cpp=1.4.2-3jammy.20220218.234334`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-typesupport-interface=3.0.1-2jammy.20220218.223426`

Binary Packages:

- `ros-rolling-rosidl-typesupport-interface=3.0.1-2jammy.20220218.223426`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-typesupport-introspection-c=3.0.1-2jammy.20220218.232254`

Binary Packages:

- `ros-rolling-rosidl-typesupport-introspection-c=3.0.1-2jammy.20220218.232254`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rosidl-typesupport-introspection-cpp=3.0.1-2jammy.20220218.233459`

Binary Packages:

- `ros-rolling-rosidl-typesupport-introspection-cpp=3.0.1-2jammy.20220218.233459`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-rpyutils=0.2.0-2jammy.20220218.214234`

Binary Packages:

- `ros-rolling-rpyutils=0.2.0-2jammy.20220218.214234`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-sensor-msgs=4.0.0-2jammy.20220219.170350`

Binary Packages:

- `ros-rolling-sensor-msgs=4.0.0-2jammy.20220219.170350`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-shape-msgs=4.0.0-2jammy.20220219.170144`

Binary Packages:

- `ros-rolling-shape-msgs=4.0.0-2jammy.20220219.170144`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-shared-queues-vendor=0.13.0-3jammy.20220218.210415`

Binary Packages:

- `ros-rolling-shared-queues-vendor=0.13.0-3jammy.20220218.210415`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-spdlog-vendor=1.3.0-2jammy.20220218.223610`

Binary Packages:

- `ros-rolling-spdlog-vendor=1.3.0-2jammy.20220218.223610`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-sqlite3-vendor=0.13.0-3jammy.20220218.210452`

Binary Packages:

- `ros-rolling-sqlite3-vendor=0.13.0-3jammy.20220218.210452`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-sros2-cmake=0.10.3-2jammy.20220219.173741`

Binary Packages:

- `ros-rolling-sros2-cmake=0.10.3-2jammy.20220219.173741`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-sros2=0.10.3-2jammy.20220219.173513`

Binary Packages:

- `ros-rolling-sros2=0.10.3-2jammy.20220219.173513`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-statistics-msgs=1.1.0-2jammy.20220219.163326`

Binary Packages:

- `ros-rolling-statistics-msgs=1.1.0-2jammy.20220219.163326`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-std-msgs=4.0.0-2jammy.20220219.163322`

Binary Packages:

- `ros-rolling-std-msgs=4.0.0-2jammy.20220219.163322`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-std-srvs=4.0.0-2jammy.20220219.162237`

Binary Packages:

- `ros-rolling-std-srvs=4.0.0-2jammy.20220219.162237`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-stereo-msgs=4.0.0-2jammy.20220219.170905`

Binary Packages:

- `ros-rolling-stereo-msgs=4.0.0-2jammy.20220219.170905`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-bullet=0.21.0-2jammy.20220219.182441`

Binary Packages:

- `ros-rolling-tf2-bullet=0.21.0-2jammy.20220219.182441`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-eigen-kdl=0.21.0-2jammy.20220219.170646`

Binary Packages:

- `ros-rolling-tf2-eigen-kdl=0.21.0-2jammy.20220219.170646`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-eigen=0.21.0-2jammy.20220219.182535`

Binary Packages:

- `ros-rolling-tf2-eigen=0.21.0-2jammy.20220219.182535`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-geometry-msgs=0.21.0-2jammy.20220219.182628`

Binary Packages:

- `ros-rolling-tf2-geometry-msgs=0.21.0-2jammy.20220219.182628`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-kdl=0.21.0-2jammy.20220219.182431`

Binary Packages:

- `ros-rolling-tf2-kdl=0.21.0-2jammy.20220219.182431`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-msgs=0.21.0-2jammy.20220219.165935`

Binary Packages:

- `ros-rolling-tf2-msgs=0.21.0-2jammy.20220219.165935`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-py=0.21.0-2jammy.20220219.173002`

Binary Packages:

- `ros-rolling-tf2-py=0.21.0-2jammy.20220219.173002`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-ros-py=0.21.0-2jammy.20220219.173213`

Binary Packages:

- `ros-rolling-tf2-ros-py=0.21.0-2jammy.20220219.173213`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-ros=0.21.0-2jammy.20220219.181725`

Binary Packages:

- `ros-rolling-tf2-ros=0.21.0-2jammy.20220219.181725`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-sensor-msgs=0.21.0-2jammy.20220219.182845`

Binary Packages:

- `ros-rolling-tf2-sensor-msgs=0.21.0-2jammy.20220219.182845`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2-tools=0.21.0-2jammy.20220219.173413`

Binary Packages:

- `ros-rolling-tf2-tools=0.21.0-2jammy.20220219.173413`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tf2=0.21.0-2jammy.20220219.170243`

Binary Packages:

- `ros-rolling-tf2=0.21.0-2jammy.20220219.170243`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tinyxml-vendor=0.8.2-2jammy.20220218.160646`

Binary Packages:

- `ros-rolling-tinyxml-vendor=0.8.2-2jammy.20220218.160646`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tinyxml2-vendor=0.7.4-2jammy.20220218.163844`

Binary Packages:

- `ros-rolling-tinyxml2-vendor=0.7.4-2jammy.20220218.163844`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-tracetools=4.0.0-2jammy.20220218.224441`

Binary Packages:

- `ros-rolling-tracetools=4.0.0-2jammy.20220218.224441`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-trajectory-msgs=4.0.0-2jammy.20220219.165635`

Binary Packages:

- `ros-rolling-trajectory-msgs=4.0.0-2jammy.20220219.165635`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-uncrustify-vendor=2.0.0-2jammy.20220218.160647`

Binary Packages:

- `ros-rolling-uncrustify-vendor=2.0.0-2jammy.20220218.160647`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-unique-identifier-msgs=2.2.1-2jammy.20220219.162618`

Binary Packages:

- `ros-rolling-unique-identifier-msgs=2.2.1-2jammy.20220219.162618`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-urdf-parser-plugin=2.5.3-2jammy.20220218.223918`

Binary Packages:

- `ros-rolling-urdf-parser-plugin=2.5.3-2jammy.20220218.223918`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-urdf=2.5.3-2jammy.20220219.000917`

Binary Packages:

- `ros-rolling-urdf=2.5.3-2jammy.20220219.000917`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-urdfdom-headers=1.0.5-3jammy.20220218.155403`

Binary Packages:

- `ros-rolling-urdfdom-headers=1.0.5-3jammy.20220218.155403`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-urdfdom=3.0.1-2jammy.20220218.225828`

Binary Packages:

- `ros-rolling-urdfdom=3.0.1-2jammy.20220218.225828`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-visualization-msgs=4.0.0-2jammy.20220219.170908`

Binary Packages:

- `ros-rolling-visualization-msgs=4.0.0-2jammy.20220219.170908`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-yaml-cpp-vendor=8.0.0-2jammy.20220218.160725`

Binary Packages:

- `ros-rolling-yaml-cpp-vendor=8.0.0-2jammy.20220218.160725`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rolling-zstd-vendor=0.13.0-3jammy.20220218.210532`

Binary Packages:

- `ros-rolling-zstd-vendor=0.13.0-3jammy.20220218.210532`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `setuptools=59.6.0-1.2`

Binary Packages:

- `python3-pkg-resources=59.6.0-1.2`
- `python3-setuptools=59.6.0-1.2`

Licenses: (parsed from: `/usr/share/doc/python3-pkg-resources/copyright`, `/usr/share/doc/python3-setuptools/copyright`)

- `Apache-2.0`
- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris setuptools=59.6.0-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/setuptools/setuptools_59.6.0-1.2.dsc' setuptools_59.6.0-1.2.dsc 1561 SHA512:ae90217146c4ef7530bc26242ec92770d0774e04be33276d8d438aae81d8dc944cb9c5919cdaffb7debe312c5a5b2554a21522b16f27e5fb0f7783f8c22c5f31
'http://archive.ubuntu.com/ubuntu/pool/main/s/setuptools/setuptools_59.6.0.orig.tar.gz' setuptools_59.6.0.orig.tar.gz 2281973 SHA512:25472ec7c167e07113c6645880952458969b146766b64224ec8f40dfc2a29b23e47104b63e806292ec81ee4e9dbbdc4663228f39b4412b586cba644f69b52309
'http://archive.ubuntu.com/ubuntu/pool/main/s/setuptools/setuptools_59.6.0-1.2.debian.tar.xz' setuptools_59.6.0-1.2.debian.tar.xz 13572 SHA512:470234d4c24c19ed0d62ad0f69470a4580fbd3a1fdb5f2bc2fb787ec54e64eddc648cd4c660469886eca4a300a7092eeb549954d1da39a0ddc671c399960fdd8
```

### `dpkg` source package: `sgml-base=1.30`

Binary Packages:

- `sgml-base=1.30`

Licenses: (parsed from: `/usr/share/doc/sgml-base/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sgml-base=1.30
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.30.dsc' sgml-base_1.30.dsc 1541 SHA512:6477c8b39b10f41b2059efe28c019fb89c9b2bdd3483a15784affa15bc08fffbd0237fadfab89ea588bee43e9c22ff3898f6c5b15ddb2325478acd2ea3f66bb6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.30.tar.xz' sgml-base_1.30.tar.xz 12536 SHA512:d1453cdad1791f83b29262dd496b23d6b1a468822ae6d28afced7961a56accc5e703123fcef9b6031118623cbb3a71556bc7e56b59322773ba473bc7ba228e9f
```

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

### `dpkg` source package: `six=1.16.0-3`

Binary Packages:

- `python3-six=1.16.0-3`

Licenses: (parsed from: `/usr/share/doc/python3-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.16.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.16.0-3.dsc' six_1.16.0-3.dsc 2358 SHA512:9a70a693229b6bceaa01fbe9c886f68cf3fcf8dd0148caf688e169fa3d0419b44518ec90b1c88c3823716ba1895d2dba28d2b976145480ea526516d6904d3fa1
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.16.0.orig.tar.gz' six_1.16.0.orig.tar.gz 34041 SHA512:076fe31c8f03b0b52ff44346759c7dc8317da0972403b84dfe5898179f55acdba6c78827e0f8a53ff20afe8b76432c6fe0d655a75c24259d9acbaa4d9e8015c0
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.16.0-3.debian.tar.xz' six_1.16.0-3.debian.tar.xz 4964 SHA512:a7f4bf61129722f16c3011852cff0028176893fc3cd8b5e641b6ba0e7f6aaac0858c8b29611a598a786a07d5ee8d8243d6a1c977e6360a1c70a18fbff3090fec
```

### `dpkg` source package: `snowball=2.2.0-1`

Binary Packages:

- `python3-snowballstemmer=2.2.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-snowballstemmer/copyright`)

- `BSD-3-snowball`

Source:

```console
$ apt-get source -qq --print-uris snowball=2.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/snowball/snowball_2.2.0-1.dsc' snowball_2.2.0-1.dsc 1634 SHA512:c42f5df63126939d1de2a40efe0196f3c29fff2289c1c53af00b7ceb74b19af8a49c9a467125be71833edb5d719ad69cb6489cbfa3c7f94c6c091ef1cf9d95f8
'http://archive.ubuntu.com/ubuntu/pool/main/s/snowball/snowball_2.2.0.orig.tar.gz' snowball_2.2.0.orig.tar.gz 223846 SHA512:02c43313de9de2518ea51cfb11f1c29145fc046c7838329bfdefd70b604009ad44b6db8175c25b0db31f03db30a6aec5857aa35775a9c204ec976df9cae62957
'http://archive.ubuntu.com/ubuntu/pool/main/s/snowball/snowball_2.2.0-1.debian.tar.xz' snowball_2.2.0-1.debian.tar.xz 8352 SHA512:080a5003736578092af84eefc158fedf08322229d160e96001f914e1ef18493224684e7fe781de372b50df8e16175628b44e858a20cd283c6fc4e395ffec859a
```

### `dpkg` source package: `spdlog=1:1.9.2+ds-0.2`

Binary Packages:

- `libspdlog-dev:amd64=1:1.9.2+ds-0.2`
- `libspdlog1:amd64=1:1.9.2+ds-0.2`

Licenses: (parsed from: `/usr/share/doc/libspdlog-dev/copyright`, `/usr/share/doc/libspdlog1/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris spdlog=1:1.9.2+ds-0.2
'http://archive.ubuntu.com/ubuntu/pool/universe/s/spdlog/spdlog_1.9.2%2bds-0.2.dsc' spdlog_1.9.2+ds-0.2.dsc 2136 SHA512:a6819ffaa495f5d3fd111d13bdbca25d3e1ccbeab86e30ecffa9535afd66313ce3cb316ca2d5c42fa7757177fc7e3791474a4e9136aee8f40f146578fbf81399
'http://archive.ubuntu.com/ubuntu/pool/universe/s/spdlog/spdlog_1.9.2%2bds.orig.tar.xz' spdlog_1.9.2+ds.orig.tar.xz 163388 SHA512:c4293364a21ed90537667ace2e4c5365f332bb6a6af989c2d82a71c09ed1d41dbb5b43110f9d99d87a3090b58a98058683910cc8c4b5d18753e1af14f23947e2
'http://archive.ubuntu.com/ubuntu/pool/universe/s/spdlog/spdlog_1.9.2%2bds-0.2.debian.tar.xz' spdlog_1.9.2+ds-0.2.debian.tar.xz 6632 SHA512:dcc82ce72334d4adbcaafeb40a6f56889bea7ed2789bfc82cd2f40c2d03c9e489fb4b8e9f89911274115b37bf4e284cc7abedd760f76565f6432830741488182
```

### `dpkg` source package: `sphinx=4.3.2-1`

Binary Packages:

- `libjs-sphinxdoc=4.3.2-1`

Licenses: (parsed from: `/usr/share/doc/libjs-sphinxdoc/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `PSF-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sphinx=4.3.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sphinx/sphinx_4.3.2-1.dsc' sphinx_4.3.2-1.dsc 3502 SHA512:a8b619e88c4d587ca37efe962bbac451ef6d7e3c5724a29eb54dd01dd72281af775c64c7be9943e3ec6b5a35d61a3b51d8eafbbf4b2b29408b637802f8cdc6fd
'http://archive.ubuntu.com/ubuntu/pool/main/s/sphinx/sphinx_4.3.2.orig.tar.gz' sphinx_4.3.2.orig.tar.gz 6657148 SHA512:2045e1964aef54826a2cde30e6c09b7ec35d49a45b7e449c07ee107c41304435eb51e2be307af77bed4ec50534e6e4009501d58187baa1a129134b69cdc56dff
'http://archive.ubuntu.com/ubuntu/pool/main/s/sphinx/sphinx_4.3.2.orig.tar.gz.asc' sphinx_4.3.2.orig.tar.gz.asc 833 SHA512:3d91964c5fa07ca928f40b4c871e9e0ba08c39c47ff81b4d6a3c9fecaae703e1ec2e5d597f5a29d1dcfaca58ac6d9303b6e074de5ac8c834ed8be22d7764bb9f
'http://archive.ubuntu.com/ubuntu/pool/main/s/sphinx/sphinx_4.3.2-1.debian.tar.xz' sphinx_4.3.2-1.debian.tar.xz 40616 SHA512:1822779642dcf9297878082abae43fd751c7a7f34f4135516f3ff4a2d970f1d7222a5006cebd2b2c726990feee4a59badee2aee71e7643b12c6f15c636185f19
```

### `dpkg` source package: `sqlite3=3.37.2-2`

Binary Packages:

- `libsqlite3-0:amd64=3.37.2-2`
- `libsqlite3-dev:amd64=3.37.2-2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

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

### `dpkg` source package: `sudo=1.9.9-1ubuntu2`

Binary Packages:

- `sudo=1.9.9-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/sudo/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `ISC`
- `Zlib`
- `other`

Source:

```console
$ apt-get source -qq --print-uris sudo=1.9.9-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.9.9-1ubuntu2.dsc' sudo_1.9.9-1ubuntu2.dsc 2587 SHA512:5d3f069a7a80c47cd91b8639e469c17482310c667128bd6064b2ebd06d641f0ff07cd339c3d11f6f3f0581d87f4094db6965798cc6855f2514d011bcdf3c2be6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.9.9.orig.tar.gz' sudo_1.9.9.orig.tar.gz 4456969 SHA512:53064240431ae3d9409dc5cb7d72ab55d9ab5f802af4de99fadd987855461b3cca53f261d6256e3b6f35e30c7e162f4dfa3978ef6976415cf5be874fb2026614
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.9.9.orig.tar.gz.asc' sudo_1.9.9.orig.tar.gz.asc 833 SHA512:b73866881351b10e8feca9db238c38330a0d91d53ca33c61c3ed6623e771daf088095332452f99ac2d13126cfc9bab63f0ff1d948b5ae881a194a70c3b0c4e18
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.9.9-1ubuntu2.debian.tar.xz' sudo_1.9.9-1ubuntu2.debian.tar.xz 40476 SHA512:eb5e76691932bb00bdaa691e07273a87422a481b59b2ce97d643a503a99894addaf70c2b8764331b7234f3e8f6ac7966f267886a74145ca8172ba7e25393aec3
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

### `dpkg` source package: `tiff=4.3.0-4`

Binary Packages:

- `libtiff5:amd64=4.3.0-4`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.3.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0-4.dsc' tiff_4.3.0-4.dsc 2417 SHA512:e39150a40a0a6426c35b47accca32ced5c6ce94219eac13ce69e4341f1973c0899c2216131885f856e23e07ce9500877571a81509b9a28cb1125b47606fd0a84
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz' tiff_4.3.0.orig.tar.gz 2808254 SHA512:e04a4a6c542e58a174c1e9516af3908acf1d3d3e1096648c5514f4963f73e7af27387a76b0fbabe43cf867a18874088f963796a7cd6e45deb998692e3e235493
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz.asc' tiff_4.3.0.orig.tar.gz.asc 488 SHA512:115a4c5714b52d0fbea800c494d83c8a96b70b2c9ce84a8df03205d9afc517faa17963f5f9508c013d7d3e2be6675b84b594a771a829406473234c4bd85e469e
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0-4.debian.tar.xz' tiff_4.3.0-4.debian.tar.xz 20808 SHA512:8dfdc7d4a0f08ee618ffd121209ac194b5e7717cca53c0fc9187e09d107cdfa5c41e298348f6b67f457d1bcae09106f800d33a10c3497c2846fd3a572caae718
```

### `dpkg` source package: `tinyxml2=9.0.0+dfsg-3`

Binary Packages:

- `libtinyxml2-9:amd64=9.0.0+dfsg-3`
- `libtinyxml2-dev:amd64=9.0.0+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libtinyxml2-9/copyright`, `/usr/share/doc/libtinyxml2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris tinyxml2=9.0.0+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_9.0.0%2bdfsg-3.dsc' tinyxml2_9.0.0+dfsg-3.dsc 2009 SHA512:788e78a1583d6f50eb574fc5f526355a55e8f6aa669c6abfecad526556532e3223bf4151bf206af6306d5394ee1b3806b4f9f1daa8afc66f881612b71db25360
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_9.0.0%2bdfsg.orig.tar.xz' tinyxml2_9.0.0+dfsg.orig.tar.xz 336516 SHA512:2c11456769fa363d7116d4ce2e3fc2e67643beee5f3814e721b36a613e1bc5050c3b88199ca4b18342622ec493bf1171560ecb21b23d24ed49a1e01a5dd8ff2a
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_9.0.0%2bdfsg-3.debian.tar.xz' tinyxml2_9.0.0+dfsg-3.debian.tar.xz 8408 SHA512:ceff569f2add4c9bc9f87ab37ddf2e19e3ebdb848dacf70475d136e0051f0992636aaabb365e5c0f0aa0cf9fc3a371aff2f7b5ee1a5575298880ffd90db875ea
```

### `dpkg` source package: `tinyxml=2.6.2-6`

Binary Packages:

- `libtinyxml-dev:amd64=2.6.2-6`
- `libtinyxml2.6.2v5:amd64=2.6.2-6`

Licenses: (parsed from: `/usr/share/doc/libtinyxml-dev/copyright`, `/usr/share/doc/libtinyxml2.6.2v5/copyright`)

- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris tinyxml=2.6.2-6
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml/tinyxml_2.6.2-6.dsc' tinyxml_2.6.2-6.dsc 1957 SHA512:d16d8c25cdf3aca6b3f1c1cebb93f9b6840b5f94116afb465797ac2f156c10ceca7032e5b85f4473e0c4355e2cb397cd9f3cc9ad5609f61707a267f931893594
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml/tinyxml_2.6.2.orig.tar.gz' tinyxml_2.6.2.orig.tar.gz 210124 SHA512:133b5db06131a90ad0c2b39b0063f1c8e65e67288a7e5d67e1f7d9ba32af10dc5dfa0462f9723985ee27debe8f09a10a25d4b5a5aaff2ede979b1cebe8e59d56
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml/tinyxml_2.6.2-6.debian.tar.xz' tinyxml_2.6.2-6.debian.tar.xz 5108 SHA512:6ebd1b34e49f027bd0d15ebaea1b081458e875225c0985e52fcf1dedd6853739b09d435ef007d1a23d4c0a003fcd24359b8d0165137dc14b617a2b113d9c249d
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

### `dpkg` source package: `uncrustify=0.72.0+dfsg1-2`

Binary Packages:

- `uncrustify=0.72.0+dfsg1-2`

Licenses: (parsed from: `/usr/share/doc/uncrustify/copyright`)

- `Artistic`
- `GPL`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris uncrustify=0.72.0+dfsg1-2
'http://archive.ubuntu.com/ubuntu/pool/universe/u/uncrustify/uncrustify_0.72.0%2bdfsg1-2.dsc' uncrustify_0.72.0+dfsg1-2.dsc 1594 SHA512:fc18c5a323ecc5f10d9ca5bb60f144d691557a25270e254ef08f68c722e7a4341b7d8ed1d18df1badb3c07c1a8cfc5f87231670a46a6256b9ebd00b688959b3e
'http://archive.ubuntu.com/ubuntu/pool/universe/u/uncrustify/uncrustify_0.72.0%2bdfsg1.orig.tar.xz' uncrustify_0.72.0+dfsg1.orig.tar.xz 866560 SHA512:ce8473747f2cc861dac7a6186861766b4b9061838a54a48925586f1de8f2b9c796494afe6421073758ecb31c939d97ebdb3888600bc395727a80ad941fbdfee2
'http://archive.ubuntu.com/ubuntu/pool/universe/u/uncrustify/uncrustify_0.72.0%2bdfsg1-2.debian.tar.xz' uncrustify_0.72.0+dfsg1-2.debian.tar.xz 6392 SHA512:0c015180757533c66d1d99898650919cdd3076a1361d558b75f9d599e6a8b25c8f2919b48d77240996d5482ea603a7452c3bb6cee828f2d0adc4203b6f7c3657
```

### `dpkg` source package: `underscore=1.13.2~dfsg-2`

Binary Packages:

- `libjs-underscore=1.13.2~dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libjs-underscore/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris underscore=1.13.2~dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/u/underscore/underscore_1.13.2%7edfsg-2.dsc' underscore_1.13.2~dfsg-2.dsc 2200 SHA512:452ea2d91ddbdd394c44fd18b8cab3a82ef4816787fa9a89c9f3059591d8e7c623e3ef983e26fabadf5918705ea99ef4ee6ea1a6b6f8a456590a7cc38ec85764
'http://archive.ubuntu.com/ubuntu/pool/main/u/underscore/underscore_1.13.2%7edfsg.orig.tar.xz' underscore_1.13.2~dfsg.orig.tar.xz 215248 SHA512:f13d496724e2418f177dd44ec119b5124729168aaf92b8a284ff8481a3603540f90b0e33a02d481c65225cff2972a41e671f4feb2be33e92e741caaf84c57295
'http://archive.ubuntu.com/ubuntu/pool/main/u/underscore/underscore_1.13.2%7edfsg-2.debian.tar.xz' underscore_1.13.2~dfsg-2.debian.tar.xz 8988 SHA512:4840dbbd2c73cdc284b7afe2da85dd0b14b5cc64bf7b4eeef18706c7ca6fdddc2feb0912ca5872855df07fc3981ea0720af93bbd5f85723ee1c291304a2d7fab
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `xml-core=0.18+nmu1`

Binary Packages:

- `xml-core=0.18+nmu1`

Licenses: (parsed from: `/usr/share/doc/xml-core/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xml-core=0.18+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.18%2bnmu1.dsc' xml-core_0.18+nmu1.dsc 1632 SHA512:1c3a335850618902a71478ee26136848e7de12f1ec090cca0598d1a2e4810f3fa5b97d65fd058752e904c1073a36785bef3b088ce34623de290e3c80c971b69b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.18%2bnmu1.tar.xz' xml-core_0.18+nmu1.tar.xz 21312 SHA512:568a3e73acb64db8074e88813a6f64c9839a92e9afba6bbb90e5852e2cc6565636e380ba87fec6d29aa6b4eaa896131ef2d404ed3811443a4df1c6bdb3d1545b
```

### `dpkg` source package: `xorg=1:7.7+23ubuntu1`

Binary Packages:

- `x11-common=1:7.7+23ubuntu1`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+23ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7%2b23ubuntu1.dsc' xorg_7.7+23ubuntu1.dsc 2066 SHA512:bb74afaaa991e04df01a48960f6bda0f0106009e39d44420d573debe5a884374721d56c998e9ef2f08352c11e1d73d9412b9ba167caabf2053e96381b9639d01
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7%2b23ubuntu1.tar.gz' xorg_7.7+23ubuntu1.tar.gz 295648 SHA512:be0ad038680ea696369d7c9bf6e42c94c2bd110ab4543b1728f4691087fce9c0817f77e4d00d768d189350b4979bcbfe548af445e076e2b89ff993bc81be1175
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
- `xz-utils=5.2.5-2build1`

Licenses: (parsed from: `/usr/share/doc/liblzma5/copyright`, `/usr/share/doc/xz-utils/copyright`)

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

### `dpkg` source package: `z3=4.8.12-1`

Binary Packages:

- `libz3-4:amd64=4.8.12-1`

Licenses: (parsed from: `/usr/share/doc/libz3-4/copyright`)

- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris z3=4.8.12-1
'http://archive.ubuntu.com/ubuntu/pool/universe/z/z3/z3_4.8.12-1.dsc' z3_4.8.12-1.dsc 2642 SHA512:80334728cedc76e545625685e6e75c460f5380fd633ed17a895511acd8bfc709d732da6e4c0468eef3b46d4c49fe8646c0b8e25e6bdaf4c9653b18efd5a14f25
'http://archive.ubuntu.com/ubuntu/pool/universe/z/z3/z3_4.8.12.orig.tar.gz' z3_4.8.12.orig.tar.gz 4803435 SHA512:0b377923bdaffaca1846aa2abd61003bbecadfcdfc908ed3097d0aac8f32028ac39d93fb4a9c2e2c2bfffbdbee80aa415875f17de6c2ee2ae8e2b7921f788c6e
'http://archive.ubuntu.com/ubuntu/pool/universe/z/z3/z3_4.8.12-1.debian.tar.xz' z3_4.8.12-1.debian.tar.xz 9896 SHA512:ebc23dbfdde0e254566f7d9086bddd1a4b0f9e21ee4274580e1d9e03136bb45d0fea9185035fd6db8976bc3d2194f2a29fa004bce4733fb20ad812f6f09a17cb
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
