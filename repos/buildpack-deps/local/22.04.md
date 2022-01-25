# `buildpack-deps:jammy`

## Docker Metadata

- Image ID: `sha256:1c44d01f9225c8fd20dceec804bd5c6a79997cf9a364ca59c29b43042664a9fd`
- Created: `2022-01-19T20:30:05.679107377Z`
- Virtual Size: ~ 720.13 Mb  
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `aom=3.2.0-2`

Binary Packages:

- `libaom3:amd64=3.2.0-2`

Licenses: (parsed from: `/usr/share/doc/libaom3/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `ISC`
- `public-domain-md5`

Source:

```console
$ apt-get source -qq --print-uris aom=3.2.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_3.2.0-2.dsc' aom_3.2.0-2.dsc 2190 SHA512:3b75a20c3f0932f2a7ab0ac062a1a78e58a464cbdd6b0f9469324b615eb89792ca0e636c7aee565224b8128ac3550cc2abee36241bd90f65ea940bc72be610d0
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_3.2.0.orig.tar.gz' aom_3.2.0.orig.tar.gz 4728473 SHA512:7f42ecd235e366cf2469825314a36ecad55ce6edc1609f03f0095cc70ee6427303e7896f7e970ac0df5094f74d7b6a3e3a7315a87bde8dec8f0382ca5b690c40
'http://archive.ubuntu.com/ubuntu/pool/universe/a/aom/aom_3.2.0-2.debian.tar.xz' aom_3.2.0-2.debian.tar.xz 12172 SHA512:929f5d5ec6ea3bad081b935f76b3929ce27943d7709f6759edcc3a3c1f91eced18af5428159fbf13b7c0d50be01644d6ede7431464f533d01c09abb18a6b4522
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

### `dpkg` source package: `apt=2.3.13`

Binary Packages:

- `apt=2.3.13`
- `libapt-pkg6.0:amd64=2.3.13`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.3.13/


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

### `dpkg` source package: `automake-1.16=1:1.16.5-1.1`

Binary Packages:

- `automake=1:1.16.5-1.1`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.5-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.1.dsc' automake-1.16_1.16.5-1.1.dsc 2575 SHA512:406bbca627187857308dbaf051355c68842ff03a66bad17c798e974fa26fa50068f7b05a51116518160085903bcda5d31de26e968ee42f17c33f94479a8a8c8d
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz' automake-1.16_1.16.5.orig.tar.xz 1601740 SHA512:3084ae543aa3fb5a05104ffb2e66cfa9a53080f2343c44809707fd648516869511500dba50dae67ff10f92a1bf3b5a92b2a0fa01cda30adb69b9da03994d9d88
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5.orig.tar.xz.asc' automake-1.16_1.16.5.orig.tar.xz.asc 833 SHA512:032a7c39abb4cabbefa4eb9c15263baec0902e48c0c81364307361a41fd55be282b9640707c789f5ae572e8e60240e34d1b575a671b5710f5d2a5716fafc2d51
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.5-1.1.debian.tar.xz' automake-1.16_1.16.5-1.1.debian.tar.xz 13320 SHA512:313223204596bc805a5f92160cc29f10d93c591368c65a1dbba3e5bc26f68436dab6c33a6486044ad5d11c5ccdbd7ec5131d60888ecb12b8a00e53f84fe84591
```

### `dpkg` source package: `autotools-dev=20180224.1+nmu1`

Binary Packages:

- `autotools-dev=20180224.1+nmu1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1+nmu1.dsc' autotools-dev_20180224.1+nmu1.dsc 1663 SHA512:936c08ab3dd1ed42fe3f21ce0973168d80e8739557f15dc4d3a9f98dd70426b20f7ca73619c1621d3751997dc9862cd86c1ca9ff61d18697f2c30dd0158f683b
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1+nmu1.tar.xz' autotools-dev_20180224.1+nmu1.tar.xz 68356 SHA512:4fe5941597e64a6a69f9ce8f5c537d8a4a1cdfad5aa476d4353976476a2f33917b5391c849dd49bbe8ba3571520b79781b14db597e8b5f02eee3c01490032023
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

### `dpkg` source package: `bash=5.1-5ubuntu1`

Binary Packages:

- `bash=5.1-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `binutils=2.37.50.20220106-2ubuntu1`

Binary Packages:

- `binutils=2.37.50.20220106-2ubuntu1`
- `binutils-common:amd64=2.37.50.20220106-2ubuntu1`
- `binutils-x86-64-linux-gnu=2.37.50.20220106-2ubuntu1`
- `libbinutils:amd64=2.37.50.20220106-2ubuntu1`
- `libctf-nobfd0:amd64=2.37.50.20220106-2ubuntu1`
- `libctf0:amd64=2.37.50.20220106-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.37.50.20220106-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.37.50.20220106-2ubuntu1.dsc' binutils_2.37.50.20220106-2ubuntu1.dsc 8883 SHA512:b076def8ee57eaae93c64505b186894c1cc937e4e9bd745b566467980ddeb370cdb9e73c210c6bde4f5cf8e848acb168bc968f2bd77e12776d9bb63fef6da043
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.37.50.20220106.orig.tar.xz' binutils_2.37.50.20220106.orig.tar.xz 22515028 SHA512:b3b546c6fc1b23622720069a7ec301c06be9feb833404d2dda79ca06d179711c7e667420b87255127c3d91445cb775f58c11035783d1bb02356f92169554bdcc
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.37.50.20220106-2ubuntu1.debian.tar.xz' binutils_2.37.50.20220106-2ubuntu1.debian.tar.xz 191064 SHA512:00760a12496b9b1510c4bf5b7cee5c937f0fced232e2c341703389f4867b2753ccff773e9b84a0146239b82a31c36bc00ea39bd4c1b53fa8eeb3acb0feef1134
```

### `dpkg` source package: `brotli=1.0.9-2build4`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2build4`
- `libbrotli1:amd64=1.0.9-2build4`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

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

- `bzip2=1.0.8-5`
- `libbz2-1.0:amd64=1.0.8-5`
- `libbz2-dev:amd64=1.0.8-5`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

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

### `dpkg` source package: `curl=7.80.0-3`

Binary Packages:

- `curl=7.80.0-3`
- `libcurl3-gnutls:amd64=7.80.0-3`
- `libcurl4:amd64=7.80.0-3`
- `libcurl4-openssl-dev:amd64=7.80.0-3`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/curl/7.80.0-3/


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

### `dpkg` source package: `dav1d=0.9.2-1`

Binary Packages:

- `libdav1d5:amd64=0.9.2-1`

Licenses: (parsed from: `/usr/share/doc/libdav1d5/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dav1d=0.9.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.9.2-1.dsc' dav1d_0.9.2-1.dsc 2332 SHA512:90c914fb2e059d442b921460fe742b2050e27896be0578337becb4a8a6fc3d5c8cbe0bb40c85800b082f35eae73e2f0cd23a80546875320ee884a5f4c4b775b6
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.9.2.orig.tar.xz' dav1d_0.9.2.orig.tar.xz 713352 SHA512:87026f8b14e408ff50fc8f137ec2ede4b14c5f69687e615d2359d0f718ae5cb5176522490786d9ae1f7838182f82615c2674f7c2961b6dcec83f1ee587c3af7c
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.9.2.orig.tar.xz.asc' dav1d_0.9.2.orig.tar.xz.asc 195 SHA512:04c367dcc3f2fb2e44cfa94653c2ca86e9fd9647959bfdd62ceb0007ad968e39550a90cb8fdc4ab9d330e5ef918200f91e186f3c6263ebf8295a8b076738b7d6
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dav1d/dav1d_0.9.2-1.debian.tar.xz' dav1d_0.9.2-1.debian.tar.xz 7896 SHA512:6f3d8793c945f7392ffd29f5728fdd615bb4156a72ec993c1af8f4874ab6f5c28daaff86d99d19ea3d8adc13475c2e12da528cbf8375f5b355559094d50a52a9
```

### `dpkg` source package: `db-defaults=1:5.3.21~exp1ubuntu3`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21~exp1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21~exp1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu3.dsc' db-defaults_5.3.21~exp1ubuntu3.dsc 2083 SHA512:cab50e812702db81faca5596196eb47d45cab53429cc31d39f7c0e63a050f47c13972e22aadebd88b51d58e4e39a7224acaedad2b1a97a216ec201b6ae76c049
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu3.tar.xz' db-defaults_5.3.21~exp1ubuntu3.tar.xz 3088 SHA512:4d4ef4cfa3f47d5d248170d67afd102303f35c4230feb134d30ea1a858c8228971932fb349f4b6ff299af21eae9706513d463ceb3ec0852d005a208895b1fe3a
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.8ubuntu2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.8ubuntu2`
- `libdb5.3-dev=5.3.28+dfsg1-0.8ubuntu2`

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

### `dpkg` source package: `dpkg=1.20.9ubuntu3`

Binary Packages:

- `dpkg=1.20.9ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `dpkg=1.21.1ubuntu1`

Binary Packages:

- `dpkg-dev=1.21.1ubuntu1`
- `libdpkg-perl=1.21.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

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

### `dpkg` source package: `e2fsprogs=1.46.4-1ubuntu1`

Binary Packages:

- `e2fsprogs=1.46.4-1ubuntu1`
- `libext2fs2:amd64=1.46.4-1ubuntu1`
- `libss2:amd64=1.46.4-1ubuntu1`
- `logsave=1.46.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `e2fsprogs=1.46.5-2ubuntu1`

Binary Packages:

- `comerr-dev:amd64=2.1-1.46.5-2ubuntu1`
- `libcom-err2:amd64=1.46.5-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/libcom-err2/copyright`)

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

### `dpkg` source package: `elfutils=0.186-1`

Binary Packages:

- `libelf1:amd64=0.186-1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.186-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.186-1.dsc' elfutils_0.186-1.dsc 3218 SHA512:f362b96791a2ab6ac58272a0594ea02c3bee7f362fc48e4996a3a6369b2722c1ad261372ed9cbecf4a316c4783430d9c3a8908d4396b196ccc0864e5372e2878
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.186.orig.tar.bz2' elfutils_0.186.orig.tar.bz2 9230491 SHA512:c9180b27ec62935f18b9431268d176f6023d1bb938731d2af6e7626ae460af6608a70ba68483aa1ec7e6cb0fa0528b661ca8b68bc4f58ea8e18af527c5950c78
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.186-1.debian.tar.xz' elfutils_0.186-1.debian.tar.xz 37876 SHA512:c99a8d33eb7f81790898a7440d479c5972f06b85cd6b7deb3d9fbe23f7c7a698a8cfec57ce1a240ca5556d010a0924fee78fd9aae2263eb18fea950c5a6b94ac
```

### `dpkg` source package: `expat=2.4.3-1`

Binary Packages:

- `libexpat1:amd64=2.4.3-1`
- `libexpat1-dev:amd64=2.4.3-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/expat/2.4.3-1/


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

### `dpkg` source package: `file=1:5.41-2`

Binary Packages:

- `file=1:5.41-2`
- `libmagic-mgc=1:5.41-2`
- `libmagic1:amd64=1:5.41-2`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.41-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41-2.dsc' file_5.41-2.dsc 2240 SHA512:a709f8312cd305d22154633e2a3ebde03a7d9f673504983dec09f3a0bd4ea2c0ba8e396fb4d994f420cdf5eb182db4ced0255a2d0a034aa438d6c597f5179aba
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41.orig.tar.gz' file_5.41.orig.tar.gz 1064097 SHA512:bbf2d8e39450b31d0ba8d76d202790fea953775657f942f06e6dc9091798d4a395f7205e542388e4a25b6a4506d07f36c5c4da37cfce0734133e9203a3b00654
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41.orig.tar.gz.asc' file_5.41.orig.tar.gz.asc 169 SHA512:ce9c2b1ccb5900cd2e16f0a77b2e727cd472436355b846784d36b97c7239430eceb6101a2364f2dabeb6723bec38e8fa69ed09bfd859839b76701363fe88b590
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.41-2.debian.tar.xz' file_5.41-2.debian.tar.xz 33704 SHA512:20ee42f5310ea17e66309ca23090f4bfea4ac7813f28573ad3c530484971c0b47b7d78ee7afd4477b0a53568cc24f62fc0cd256d12cc32d8270c040f64234f2f
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

### `dpkg` source package: `fontconfig=2.13.1-4.2ubuntu4`

Binary Packages:

- `fontconfig=2.13.1-4.2ubuntu4`
- `fontconfig-config=2.13.1-4.2ubuntu4`
- `libfontconfig-dev:amd64=2.13.1-4.2ubuntu4`
- `libfontconfig1:amd64=2.13.1-4.2ubuntu4`
- `libfontconfig1-dev:amd64=2.13.1-4.2ubuntu4`

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

- `libfreetype-dev:amd64=2.11.1+dfsg-1`
- `libfreetype6:amd64=2.11.1+dfsg-1`
- `libfreetype6-dev:amd64=2.11.1+dfsg-1`

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

Source:

```console
$ apt-get source -qq --print-uris freetype=2.11.1+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1+dfsg-1.dsc' freetype_2.11.1+dfsg-1.dsc 3713 SHA512:42415e8ecbd9da21e0ff075e39eddb123e4654a3f92dced474d2384f66ecebb03ec4842899ab4e933d8ba73e4eddac63b91491954cfe05791d1d49aef534b98a
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1+dfsg.orig-ft2demos.tar.xz' freetype_2.11.1+dfsg.orig-ft2demos.tar.xz 257240 SHA512:93d68daefa8a49b4fc987a7356133299fe2a8e012415ea09ad7616ececcfd978fdf9fc7a2d855f7488f51a497d019acb89ef5774484babae66357b3083a883c5
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1+dfsg.orig-ft2demos.tar.xz.asc' freetype_2.11.1+dfsg.orig-ft2demos.tar.xz.asc 195 SHA512:407ffade07cc62c8838d26670dffc7c26b9baf4984c42b2b2467279dabda855536b403f5a7e9dc64a787163657ca81019fef6d1879973faf180d6230ab17cd05
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1+dfsg.orig-ft2docs.tar.xz' freetype_2.11.1+dfsg.orig-ft2docs.tar.xz 2038348 SHA512:c5e19d98425491682edc58230c48390925cc4b466169f655cf3b8575ba787a70feecdeb7a16224b132dcc32f17b041483d84056cda8e3132d98b531e46a26c36
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1+dfsg.orig-ft2docs.tar.xz.asc' freetype_2.11.1+dfsg.orig-ft2docs.tar.xz.asc 195 SHA512:df946695a1fbaa71009f48a8f0860177984728ec1c73385d1e55c07be027dd6a5e634c9dcbb49c51f8143b0d56a6cbf06393403341fb28cea7a8a2cc9a9c5592
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1+dfsg.orig.tar.xz' freetype_2.11.1+dfsg.orig.tar.xz 1988020 SHA512:6a9a0379679abf127761cabb2da39b8faf2ca4c322075da9b86d93363ac81ce909b9544377a784118ba91ca008baa680b9da474bd2da1bfe928d5a4c9114cb08
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.11.1+dfsg-1.debian.tar.xz' freetype_2.11.1+dfsg-1.debian.tar.xz 40132 SHA512:c0a9b0cd8ebc8fc7e85701ba459ac946954d3a473ab069d7db8cb1dbcc8551a431e4abd36e448db2464f0e409c869683d3a1b7be07d4867540fe5b63673dd2ec
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

### `dpkg` source package: `gcc-11=11.2.0-14ubuntu1`

Binary Packages:

- `cpp-11=11.2.0-14ubuntu1`
- `g++-11=11.2.0-14ubuntu1`
- `gcc-11=11.2.0-14ubuntu1`
- `gcc-11-base:amd64=11.2.0-14ubuntu1`
- `libasan6:amd64=11.2.0-14ubuntu1`
- `libatomic1:amd64=11.2.0-14ubuntu1`
- `libcc1-0:amd64=11.2.0-14ubuntu1`
- `libgcc-11-dev:amd64=11.2.0-14ubuntu1`
- `libgcc-s1:amd64=11.2.0-14ubuntu1`
- `libgomp1:amd64=11.2.0-14ubuntu1`
- `libitm1:amd64=11.2.0-14ubuntu1`
- `liblsan0:amd64=11.2.0-14ubuntu1`
- `libquadmath0:amd64=11.2.0-14ubuntu1`
- `libstdc++-11-dev:amd64=11.2.0-14ubuntu1`
- `libstdc++6:amd64=11.2.0-14ubuntu1`
- `libtsan0:amd64=11.2.0-14ubuntu1`
- `libubsan1:amd64=11.2.0-14ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp-11/copyright`, `/usr/share/doc/g++-11/copyright`, `/usr/share/doc/gcc-11/copyright`, `/usr/share/doc/gcc-11-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-11-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-11-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-11=11.2.0-14ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-14ubuntu1.dsc' gcc-11_11.2.0-14ubuntu1.dsc 27910 SHA512:49c5bce7018ae4bbfa29b4e771f9dc98aaa61a34c49e79201cbf52e57cf6b2787ba0c83d2f6a051050282b51363c0c4399863b7877d729d14171123b519e0824
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0.orig.tar.gz' gcc-11_11.2.0.orig.tar.gz 87861992 SHA512:64e4634769a62faa0adbfe99e5e590dd9efc1facac20a7dd71ab9f1d675e7df80678cbdc75c966e08ccf91dbc1e1a681d8e3227d0026ffcb5f46bdc96acaace8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-11/gcc-11_11.2.0-14ubuntu1.debian.tar.xz' gcc-11_11.2.0-14ubuntu1.debian.tar.xz 2006504 SHA512:2a4e3fa763fce7114ad13dee32b52f40af645aafafed49b21ee695c436c0d06bc54cfce995079e556c9a981f59edb1d555836d51ce91d23cc047b0edbd83e949
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

### `dpkg` source package: `gdbm=1.22-1`

Binary Packages:

- `libgdbm-compat4:amd64=1.22-1`
- `libgdbm-dev:amd64=1.22-1`
- `libgdbm6:amd64=1.22-1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.22-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.22-1.dsc' gdbm_1.22-1.dsc 2583 SHA512:9dd1c9c63efe686e7db27c0912ac1074ab6b546d4e7e53bfce798901ddd25ff4c13511a22b08d5da488462c04b39950c3a96af5196d5f9639cbd4b25eb7de06a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.22.orig.tar.gz' gdbm_1.22.orig.tar.gz 1090100 SHA512:67461fc4f41e825d0134175ff99c913ccb4aa7ea3d0f64f32bdedbc7677b3ecabd2c525ac6b2ee47a9561e002e4224e492b72088d57bb4862a1f8c089521ec51
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.22.orig.tar.gz.asc' gdbm_1.22.orig.tar.gz.asc 181 SHA512:5de3d19d38f438622ae4412c7d26863d6ec6a05ba6cd285a8b5a44ada0c86ccd4781b75fa68d9315bfdab4077bb4e92afbbc9588de867f1fd388c8aaf5a644a5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.22-1.debian.tar.xz' gdbm_1.22-1.debian.tar.xz 18484 SHA512:db60c2a3821c8d160d7c4644d2a3926d81da9d5e285a3d99499f3c3446c4db1632b7186bd7d4abad410e83c033f806895e563b15b0849ed137ae1b093bd0f975
```

### `dpkg` source package: `gdk-pixbuf=2.42.6+dfsg-2ubuntu2`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.42.6+dfsg-2ubuntu2`
- `libgdk-pixbuf-2.0-0:amd64=2.42.6+dfsg-2ubuntu2`
- `libgdk-pixbuf-2.0-dev:amd64=2.42.6+dfsg-2ubuntu2`
- `libgdk-pixbuf2.0-bin=2.42.6+dfsg-2ubuntu2`
- `libgdk-pixbuf2.0-common=2.42.6+dfsg-2ubuntu2`

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
$ apt-get source -qq --print-uris gdk-pixbuf=2.42.6+dfsg-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6+dfsg-2ubuntu2.dsc' gdk-pixbuf_2.42.6+dfsg-2ubuntu2.dsc 3416 SHA512:f56e27e3dc2dd82685be5dfddffbffc9845f94a308822e3966235452beaef958c100bbf7b2a1a377c93aa491ea94239b14d4cee7efeb29ec55698d7bfdeb137a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6+dfsg.orig.tar.xz' gdk-pixbuf_2.42.6+dfsg.orig.tar.xz 6527432 SHA512:e3c9479a4ae2d1ffe45a908ad4b693305ebfa55ef3310a241f65bbc36faa880ff696166e317c9022dca569443a7e1a86e35dfc39f298f00ab5e9c7e0c5471e7b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.42.6+dfsg-2ubuntu2.debian.tar.xz' gdk-pixbuf_2.42.6+dfsg-2ubuntu2.debian.tar.xz 29912 SHA512:587c411dcb7f62e5d599eaf89545df2584bec98d5b6e47f120330201583bb5cbb811dbec42ea7752585ca4679c1112698c1566fd4b6281c52597f961ff3ca73d
```

### `dpkg` source package: `git=1:2.33.1-1ubuntu1`

Binary Packages:

- `git=1:2.33.1-1ubuntu1`
- `git-man=1:2.33.1-1ubuntu1`

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
$ apt-get source -qq --print-uris git=1:2.33.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.33.1-1ubuntu1.dsc' git_2.33.1-1ubuntu1.dsc 2948 SHA512:38aebd38a1f37bd2838560513c742c5c8b99b09b8eda3c62bf6efbc3faec8637856cee08226052f1bcade9735c8b71a14c557acdcd66885f499e490419433f47
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.33.1.orig.tar.xz' git_2.33.1.orig.tar.xz 6558636 SHA512:16d417183232e1057bea754d59cdf4bbacc5f1527d1de6ee04cdd293a2512bfa7208e20f6130816605528b59cb1bc3188c5bddf1a42c1413095ee74e44dd2f91
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.33.1-1ubuntu1.debian.tar.xz' git_2.33.1-1ubuntu1.debian.tar.xz 693760 SHA512:49557194ce12abdfdfc366d702a32db6f11c1695ba0b9ad1d6c92c87684d03fef662aa89e89bcd5793c1d22f5b19ec07ee955ea5986ce7756dd580dff623f327
```

### `dpkg` source package: `glib2.0=2.71.0-2`

Binary Packages:

- `libglib2.0-0:amd64=2.71.0-2`
- `libglib2.0-bin=2.71.0-2`
- `libglib2.0-data=2.71.0-2`
- `libglib2.0-dev:amd64=2.71.0-2`
- `libglib2.0-dev-bin=2.71.0-2`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.71.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.71.0-2.dsc' glib2.0_2.71.0-2.dsc 3545 SHA512:8a84b9fcbe6316ef76b2db36fcc44a455fb0ba27de47df88b301e14708b32a983ac832c6f8cbf1d30e18405f022badf4273d977a80a04360a2749b93e4f5e400
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.71.0.orig.tar.xz' glib2.0_2.71.0.orig.tar.xz 4842844 SHA512:833ac450d046e7293a2cabe3157ca393ca0aeac007163384e1705f1860933ae5f1cd1f7f733fd4732c3eaaaa42a941a1c486432c3768ce15238acb37bc2649d6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.71.0-2.debian.tar.xz' glib2.0_2.71.0-2.debian.tar.xz 102444 SHA512:fa5a925cbc6d4f2e2e923eabdb222da377403510d4e8941ea0880c0b06b32f146114c2e5b83e334213377c09ac151faf92dd8b5a3d5b66e91925fc4608ddf390
```

### `dpkg` source package: `glibc=2.34-0ubuntu3`

Binary Packages:

- `libc-bin=2.34-0ubuntu3`
- `libc-dev-bin=2.34-0ubuntu3`
- `libc6:amd64=2.34-0ubuntu3`
- `libc6-dev:amd64=2.34-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

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

### `dpkg` source package: `gmp=2:6.2.1+dfsg-1ubuntu3`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.1+dfsg-1ubuntu3`
- `libgmp10:amd64=2:6.2.1+dfsg-1ubuntu3`
- `libgmpxx4ldbl:amd64=2:6.2.1+dfsg-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `gnutls28=3.7.2-4ubuntu1`

Binary Packages:

- `libgnutls30:amd64=3.7.2-4ubuntu1`

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


### `dpkg` source package: `gobject-introspection=1.70.0-2ubuntu1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.70.0-2ubuntu1`
- `gir1.2-glib-2.0:amd64=1.70.0-2ubuntu1`
- `libgirepository-1.0-1:amd64=1.70.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.70.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.70.0-2ubuntu1.dsc' gobject-introspection_1.70.0-2ubuntu1.dsc 3099 SHA512:62ddb4182a36b063a1f61f9d24eed88f1ab26aeb857fcd655da03392c4a419d41c7284727ab24a1badfd2850d6652537f8d6a13b17df30bcf727b81ff0011d03
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.70.0.orig.tar.xz' gobject-introspection_1.70.0.orig.tar.xz 1029372 SHA512:216b376ed423f607e36c723dd6b67975dbfb63c253f2d8bd0b3661e3d69f8c8059cf221db8c5260b0262fad1b7d738f3b2e5fbd51fdbc31e40ccb115c209baf0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.70.0-2ubuntu1.debian.tar.xz' gobject-introspection_1.70.0-2ubuntu1.debian.tar.xz 25680 SHA512:1fb1571c64444e01a2aa66720f239a9f3dfdddb331420c472ae5f07fb924f1ca90c7d1c7ffdaa27a4a6383046effc0780f73bed912cf3bb413bf54529ed6adb9
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

### `dpkg` source package: `harfbuzz=2.7.4-1ubuntu2`

Binary Packages:

- `libharfbuzz0b:amd64=2.7.4-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.7.4-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu2.dsc' harfbuzz_2.7.4-1ubuntu2.dsc 2872 SHA512:ce9671743df87b66a3d38dd61bda38fc9af01d48751845627ff1b38d422f89ec73687d23cc0f8ca8b70c98ce82900ecc630e01e250e77dfdba5e7a635391b1da
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4.orig.tar.xz' harfbuzz_2.7.4.orig.tar.xz 9532468 SHA512:d2af6a768c397c664f654cf36140e7b5696b3b983f637454604570c348247f7ffea135048d9b02cf6593cbde728567e31bf82a39df5ff38d680c78dff24d4cf0
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.7.4-1ubuntu2.debian.tar.xz' harfbuzz_2.7.4-1ubuntu2.debian.tar.xz 11056 SHA512:f5f42c2f9aa7a4ac3cf4e8c18fc439dc3b8ca963b7a3e8a22147684f4d4e23266282fd92dad35b62632f30ffb5fc93b0c1654dfc231febeacb57bc3170f2d38e
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

- `libjbig-dev:amd64=2.1-3.1build2`
- `libjbig0:amd64=2.1-3.1build2`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1build2
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build2.dsc' jbigkit_2.1-3.1build2.dsc 2081 SHA512:3a120abc6bb211fbb1f58eba95da2a2f92f2df840a618e771b638fdc70dec0f769cc4bceff584f105764f57b99af2c5e6122df03e7c6447a7127444fe06243ad
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA512:c4127480470ef90db1ef3bd2caa444df10b50ed8df0bc9997db7612cb48b49278baf44965028f1807a21028eb965d677e015466306b44683c4ec75a23e1922cf
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build2.debian.tar.xz' jbigkit_2.1-3.1build2.debian.tar.xz 7728 SHA512:811d534138de41e727cd8e13d3c6ab178b010c7a13696977bb8302d04c2561dd7497df2c3664185dbafbe14661c1403f4aa46a32a92cc0fd3641dfbd92c8b7d9
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

- `krb5-multidev:amd64=1.19.2-0ubuntu1`
- `libgssapi-krb5-2:amd64=1.19.2-0ubuntu1`
- `libgssrpc4:amd64=1.19.2-0ubuntu1`
- `libk5crypto3:amd64=1.19.2-0ubuntu1`
- `libkadm5clnt-mit12:amd64=1.19.2-0ubuntu1`
- `libkadm5srv-mit12:amd64=1.19.2-0ubuntu1`
- `libkdb5-10:amd64=1.19.2-0ubuntu1`
- `libkrb5-3:amd64=1.19.2-0ubuntu1`
- `libkrb5-dev:amd64=1.19.2-0ubuntu1`
- `libkrb5support0:amd64=1.19.2-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit12/copyright`, `/usr/share/doc/libkadm5srv-mit12/copyright`, `/usr/share/doc/libkdb5-10/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.19.2-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2-0ubuntu1.dsc' krb5_1.19.2-0ubuntu1.dsc 3882 SHA512:c9fcd928222dde2b577db11cd66a46e1e24e68f5f919868d79b1c8c16c9146f24224fa40f3f46fd43765dd8119679521bdd4eb020a6449d6b85cec199eb53ce3
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz' krb5_1.19.2.orig.tar.gz 8741053 SHA512:b90d6ed0e1e8a87eb5cb2c36d88b823a6a6caabf85e5d419adb8a930f7eea09a5f8491464e7e454cca7ba88be09d19415962fe0036ad2e31fc584f9fc0bbd470
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2.orig.tar.gz.asc' krb5_1.19.2.orig.tar.gz.asc 833 SHA512:87c4d096dbb6821401125b8f8a315ce1aac029744ba9670a4f8a2a680e6dd5798e1c6d5d2b68b17fd9a4b3b9c6ff111cd1dcac42f934d48fb20381b3765e0f64
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.19.2-0ubuntu1.debian.tar.xz' krb5_1.19.2-0ubuntu1.debian.tar.xz 106812 SHA512:a5cfc781f55ca2b604881bae0fb91183c7a5f8192c644f1533aac442a842c4658e23334c3bfd6bde26514d2620ae0b7e92bb90914e18467f00d97bfad6366b0a
```

### `dpkg` source package: `lcms2=2.12~rc1-2build1`

Binary Packages:

- `liblcms2-2:amd64=2.12~rc1-2build1`
- `liblcms2-dev:amd64=2.12~rc1-2build1`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3 (GPL-3 for the fast_float plugin only)`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.12~rc1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12~rc1-2build1.dsc' lcms2_2.12~rc1-2build1.dsc 2037 SHA512:0744869957aaa9d7ac233273a0f4eeec4e7cf9cd519c7fc2407a8aed1b9d213443ab61db0aa879cccdc7c38bffc055f720b95799198d1a76a81bffb496a48679
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12~rc1.orig.tar.gz' lcms2_2.12~rc1.orig.tar.gz 7417767 SHA512:1d27e6f91911053b79f2a46c6c16943e25fce2f0501bb7d97f49507522a8a0f911d60f20726fc31727fee5242c6d452c86cdc28735f8f88c3aa9676fd35fdec6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.12~rc1-2build1.debian.tar.xz' lcms2_2.12~rc1-2build1.debian.tar.xz 10528 SHA512:cf1a037e24d6e86dda44ac1a72c5b585d09174f091f4f60f27bfe75259ffae5a21977862dbab79b49b57fb9000bdc30bb63b961572c1de6e36564e21944ce96f
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

### `dpkg` source package: `libbsd=0.11.3-1ubuntu3`

Binary Packages:

- `libbsd0:amd64=0.11.3-1ubuntu3`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `libcbor=0.6.0-0ubuntu4`

Binary Packages:

- `libcbor0.6:amd64=0.6.0-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libcbor0.6/copyright`)

- `Apache-2.0`
- `Expat`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libdatrie=0.2.13-1ubuntu3`

Binary Packages:

- `libdatrie1:amd64=0.2.13-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.13-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13-1ubuntu3.dsc' libdatrie_0.2.13-1ubuntu3.dsc 2371 SHA512:655a242cc30f5f7bfd2bad6870a4261b0bc31eb0f55788a70499446b8394a4377a509b374ecd6a7de34edefd4ec7a978febb91436ab932dc6263bc1693920f5b
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13.orig.tar.xz' libdatrie_0.2.13.orig.tar.xz 314072 SHA512:db3c879d825ead5871c12ef3a06bb093cb1708a6e7e20775eaf82356af9dd6ad54c6b5cabbe1773f2494d3dfa2426528fdd49441038b6294b70ccb1a3d90099a
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.13-1ubuntu3.debian.tar.xz' libdatrie_0.2.13-1ubuntu3.debian.tar.xz 9660 SHA512:1a5a6ef7b16ead5aeb3a3fe9846969d0dff85e5da5d0687af655e41319cdd5d949de0fadbff9baf6956201d91e64a1c4f84b34c8c8e9d8402430e181f660a2bf
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

### `dpkg` source package: `libdeflate=1.8-1ubuntu1`

Binary Packages:

- `libdeflate-dev:amd64=1.8-1ubuntu1`
- `libdeflate0:amd64=1.8-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libdeflate-dev/copyright`, `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.8-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.8-1ubuntu1.dsc' libdeflate_1.8-1ubuntu1.dsc 1671 SHA512:fbaface57be297f30c88b421bf09ebde37961b0ba1da1ef0259de30b17e8d64c87b0ccf7466264cc1ee3e94316d81961510ebbf48116a33c3d24d090f64c5ff8
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.8.orig.tar.gz' libdeflate_1.8.orig.tar.gz 145823 SHA512:b40caecdf783487488a5bd8213304175348b9db9bc1efdf6d5222fb912f61698b5e196522195a3640d7ff61ba953a93c0c8f75e07f548ac8b9d9c5dd5a787544
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdeflate/libdeflate_1.8-1ubuntu1.debian.tar.xz' libdeflate_1.8-1ubuntu1.debian.tar.xz 4828 SHA512:a888602a6cf02d4ac587fb2777b9139294dcf807f5e09d6b2ba72eb9d41459e20069b10e7e40c3b9888cf3ce4c925344552e52aea419274c9f646090d7f3ed27
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

### `dpkg` source package: `libevent=2.1.12-stable-1build2`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.12-stable-1build2`
- `libevent-core-2.1-7:amd64=2.1.12-stable-1build2`
- `libevent-dev=2.1.12-stable-1build2`
- `libevent-extra-2.1-7:amd64=2.1.12-stable-1build2`
- `libevent-openssl-2.1-7:amd64=2.1.12-stable-1build2`
- `libevent-pthreads-2.1-7:amd64=2.1.12-stable-1build2`

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
$ apt-get source -qq --print-uris libevent=2.1.12-stable-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1build2.dsc' libevent_2.1.12-stable-1build2.dsc 2551 SHA512:b4f54c54ac769b905b80ac48d1e0cfeb4903edb1349d71f840dfa7316f05dae048fa1c5573147acc198c672c3b515fda124ab2bc6847b18eefbfe883a965bea3
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz' libevent_2.1.12-stable.orig.tar.gz 1100847 SHA512:88d8944cd75cbe78bc4e56a6741ca67c017a3686d5349100f1c74f8a68ac0b6410ce64dff160be4a4ba0696ee29540dfed59aaf3c9a02f0c164b00307fcfe84f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable.orig.tar.gz.asc' libevent_2.1.12-stable.orig.tar.gz.asc 488 SHA512:841b57a0f6ba645b1871f257b9929093b11b7d6fd03332e6339adceddda233e78f6190faa2339e2b67b26dc2a56ddd7ce622792820b582168b31a2d1d1854f1f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.12-stable-1build2.debian.tar.xz' libevent_2.1.12-stable-1build2.debian.tar.xz 17888 SHA512:80d88d23eead6656e1f4f3a5257f923090523611c10212b8ea1d6839608d9a41958f10875bf0fc0482d4068a51f8dac2028be2b849691963db6a2bbfb5e95f0f
```

### `dpkg` source package: `libexif=0.6.24-1`

Binary Packages:

- `libexif-dev:amd64=0.6.24-1`
- `libexif12:amd64=0.6.24-1`

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
$ apt-get source -qq --print-uris libexif=0.6.24-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.24-1.dsc' libexif_0.6.24-1.dsc 2116 SHA512:c2584c01b9091967ca859a6f3a3e066a71f3f11113f4f60e340024e2d91af0d40b74b0e128d7eb2deb9225a92d031ab72b6aae2d3a03458de0511ddf0257e14e
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.24.orig.tar.gz' libexif_0.6.24.orig.tar.gz 1140079 SHA512:0b15a157c1030490bf1c4239487dffda90daad467ac6281db2a1b34a8419fca32b4b5265452e75cbcd2c9dc9a829643231cd3749e88251ed1b596756d1c5a9f4
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.24-1.debian.tar.xz' libexif_0.6.24-1.debian.tar.xz 11720 SHA512:709cefebc50645fb06d683566df9b62d2f0ad098b098eecd4e8c3da332aaf4d638ab7837f07e564a79bc3708cee6dd28d1adaa0b99f3f44dafa6914da5ce5240
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

### `dpkg` source package: `libfido2=1.9.0-1build1`

Binary Packages:

- `libfido2-1:amd64=1.9.0-1build1`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `libgpg-error=1.43-1`

Binary Packages:

- `libgpg-error0:amd64=1.43-1`

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

- http://snapshot.debian.org/package/libgpg-error/1.43-1/


### `dpkg` source package: `libheif=1.12.0-2build1`

Binary Packages:

- `libheif1:amd64=1.12.0-2build1`

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
$ apt-get source -qq --print-uris libheif=1.12.0-2build1
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.12.0-2build1.dsc' libheif_1.12.0-2build1.dsc 2423 SHA512:62cc515cbcea9f009ebcbc65860fb6e7971d42b983fb55c716a764c57a8835706757f125eb57c2b787d9e78b216aad085d946d30f192122ec0775fa9e04e3262
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.12.0.orig.tar.gz' libheif_1.12.0.orig.tar.gz 1684355 SHA512:9e6f74dd52841a33b6021a1581ab28c56123d927caa7972acd284444e90888bbdae983b6d847d20eac7651dacea2193d27eb8df45928cb0774229ef8eea23294
'http://archive.ubuntu.com/ubuntu/pool/universe/libh/libheif/libheif_1.12.0-2build1.debian.tar.xz' libheif_1.12.0-2build1.debian.tar.xz 7120 SHA512:0a12dea34fbbfef0d715635eac72e5fde0e6101a11d926f0aeddcc50878b3b97c74d4efb1b5c231eac7abca1fffc6ec7f7b5a544c622a9f3cd9caebee279ed1c
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

### `dpkg` source package: `libjpeg-turbo=2.1.1-0ubuntu1`

Binary Packages:

- `libjpeg-turbo8:amd64=2.1.1-0ubuntu1`
- `libjpeg-turbo8-dev:amd64=2.1.1-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.1.1-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.1-0ubuntu1.dsc' libjpeg-turbo_2.1.1-0ubuntu1.dsc 1706 SHA512:da512a4f2e7a164cc4d6ce9b33d050b5fed7e24be49716757a5545469c087b1f67d984462c55bf0cc886fa3c0557b849620e517769dd8b6bf8ba3ec16c344b24
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.1.orig.tar.gz' libjpeg-turbo_2.1.1.orig.tar.gz 2256321 SHA512:20a5c61923e32ed9670955107ec26e973bd6b05920f294861a6735be591ffcd5c6649a19f37d6adb5dc94642d487244ce595b3f4be1dc59378378b3087159d1f
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.1-0ubuntu1.debian.tar.xz' libjpeg-turbo_2.1.1-0ubuntu1.debian.tar.xz 17248 SHA512:81db704f39bca8cc4271811d4abb62bfbc302a81a5df188a6dd918caeb7c54a30e72aae4ae8da1274920fe46e3587a644bda5bd32c8ffc38468901a6692435b1
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

### `dpkg` source package: `libmaxminddb=1.5.2-1build1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.5.2-1build1`
- `libmaxminddb0:amd64=1.5.2-1build1`

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
$ apt-get source -qq --print-uris libmaxminddb=1.5.2-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1build1.dsc' libmaxminddb_1.5.2-1build1.dsc 2371 SHA512:3b68ac9abebf8b36d0e5bae1a098957cc945dcc59b32a8f32351b6841a7259a0a2f9c7baf6a630a4b7d4060c73ba0714ef5f9847e18d7a1c4321fefb461cff5a
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2.orig.tar.gz' libmaxminddb_1.5.2.orig.tar.gz 249507 SHA512:2f053028e28dc4f1d94039e52193ab71f8dc278f1fafa14bca1af0251d239351acadb5d540e63c250232d0fd1b8f2dd45289f0eae5c55d9b4430acbabbcd11a9
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.5.2-1build1.debian.tar.xz' libmaxminddb_1.5.2-1build1.debian.tar.xz 12408 SHA512:b64b294ba25c96ae77f22a009e1a512ef3ef2c8f83fc3df7f33b65f92b60573874c66daa13515dd4fd046f05288bebe5eb061c5098cc1c11af42a108cb531096
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

### `dpkg` source package: `librsvg=2.52.5+dfsg-1ubuntu1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.52.5+dfsg-1ubuntu1`
- `librsvg2-2:amd64=2.52.5+dfsg-1ubuntu1`
- `librsvg2-common:amd64=2.52.5+dfsg-1ubuntu1`
- `librsvg2-dev:amd64=2.52.5+dfsg-1ubuntu1`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libseccomp=2.5.2-2ubuntu2`

Binary Packages:

- `libseccomp2:amd64=2.5.2-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.2-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.2-2ubuntu2.dsc' libseccomp_2.5.2-2ubuntu2.dsc 2491 SHA512:fa56e0e961a4e895c1c306286500f997dffa2e63bf2f87d9360e5cf3c0e93a36bce94e850df24cc060958baf327e63e4dffeb989f8376e7d83c8c90004683988
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.2.orig.tar.gz' libseccomp_2.5.2.orig.tar.gz 640305 SHA512:b2a95152cb274d6b35753596fd825406dae20c4a48b2f4076f835f977ecf324de38a3fe02e789dc20b49ecf6b4eb67f03e7733e92d40f5e20f25874307f1c2ac
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.2.orig.tar.gz.asc' libseccomp_2.5.2.orig.tar.gz.asc 833 SHA512:cdd93fc69ff1032641a26e3e8573960e336a95c100bc6f09c9b3e281f3e9e34cf5fb68bccfcacd667e30d7f42a062c58c33cbd4ad7ae573971716b5fa290e0f0
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.5.2-2ubuntu2.debian.tar.xz' libseccomp_2.5.2-2ubuntu2.debian.tar.xz 34556 SHA512:abb5bd3f5971f01849f20f7daa866f37605f30bcc8e71db5a948b2ea15a6845af7fc59f84ed76859c72505b6f72c3a76b0d423d2d12a1884642b20d12bec17d2
```

### `dpkg` source package: `libselinux=3.3-1`

Binary Packages:

- `libselinux1:amd64=3.3-1`
- `libselinux1-dev:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

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

- `libsepol-dev:amd64=3.3-1`
- `libsepol2:amd64=3.3-1`

Licenses: (parsed from: `/usr/share/doc/libsepol-dev/copyright`, `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.3-1.dsc' libsepol_3.3-1.dsc 1764 SHA512:e2b879cacf0610a5e577610e850e08679166aab7c775a735c0d005861beeb98099c731869b592ff3a4cc4b24ad248b40cd2fce458f92ba5c7845f0421feedf0c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.3.orig.tar.gz' libsepol_3.3.orig.tar.gz 482546 SHA512:fb6bb69f8e43a911a1a9cbd791593215386e93cb9292e003f5d8efe6e86e0ce5d0287e95d52fe2fbce518a618beaf9b1135aea0d04eaebcdbd8c6d07ee67b500
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.3-1.debian.tar.xz' libsepol_3.3-1.debian.tar.xz 14956 SHA512:142893edbfcf12499d57f723da8423d35b1927bf9027493b112f0b0f473aec1b995d38b8b9434d385232e80fb5df3a2fa75a101704dc4cab7680ec9746728681
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

- `libltdl-dev:amd64=2.4.6-15build1`
- `libltdl7:amd64=2.4.6-15build1`
- `libtool=2.4.6-15build1`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

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

Source:

```console
$ apt-get source -qq --print-uris libunistring=0.9.10-6
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-6.dsc' libunistring_0.9.10-6.dsc 2212 SHA512:838b5c4e4fad0b372335afe7bead76cd11a911e6278bc9e829c8c92d24a4599f09c751cb02b02e9a14778b30f0ef9d4e6c9611d199eed43ad290fe8e8c962ba5
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA512:01dcab6e05ea4c33572bf96cc0558bcffbfc0e62fc86410cef06c1597a0073d5750525fe2dee4fdb39c9bd704557fcbab864f9645958108a2e07950bc539fe54
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA512:94d4316df1407850f34e84064275ae512d1ee1cd519420e2342a3f36c17d1ff7fa4019fea64507a04034ffc356c0c9add94a5abf756dd5995913583f68cfe0bd
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-6.debian.tar.xz' libunistring_0.9.10-6.debian.tar.xz 41588 SHA512:440a3c65e8b155f11bf823289e1481fb25e4a0b2686de53288fde8695a7947dfa47891445a9ffe3a963b5109fabbfedf76bce48bf5a8441ec70098987c25c6df
```

### `dpkg` source package: `libwebp=0.6.1-2.1build1`

Binary Packages:

- `libwebp-dev:amd64=0.6.1-2.1build1`
- `libwebp6:amd64=0.6.1-2.1build1`
- `libwebpdemux2:amd64=0.6.1-2.1build1`
- `libwebpmux3:amd64=0.6.1-2.1build1`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.6.1-2.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.1build1.dsc' libwebp_0.6.1-2.1build1.dsc 2103 SHA512:c6875479be12214e16c81a40aff092d6338dd0f0c51a9013f12b1fe9232e2a51dd960b0979a56cd9dfc05dd601f29bf0d32a374067af0acc04ea80c53c8d56fb
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA512:313b345a01c91eb07c2e4d46b93fcda9c50dca9e05e39f757238a679355514a2e9bc9bc220f3d3eb6d6a55148957cb2be14dac330203953337759841af1a32bf
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.1build1.debian.tar.xz' libwebp_0.6.1-2.1build1.debian.tar.xz 13688 SHA512:d44bc03718f743d42895f998dc9cd3c152bf13807fed23fa4fa9b82b40aaf55229d83f8c9b0e8652fbbae93622c2b8d4a21ef081ef35f11826417c3ee03bea69
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

### `dpkg` source package: `libx11=2:1.7.2-2`

Binary Packages:

- `libx11-6:amd64=2:1.7.2-2`
- `libx11-data=2:1.7.2-2`
- `libx11-dev:amd64=2:1.7.2-2`

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

- `libxau-dev:amd64=1:1.0.9-1build4`
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

### `dpkg` source package: `libxcb=1.14-3ubuntu2`

Binary Packages:

- `libxcb-render0:amd64=1.14-3ubuntu2`
- `libxcb-render0-dev:amd64=1.14-3ubuntu2`
- `libxcb-shm0:amd64=1.14-3ubuntu2`
- `libxcb-shm0-dev:amd64=1.14-3ubuntu2`
- `libxcb1:amd64=1.14-3ubuntu2`
- `libxcb1-dev:amd64=1.14-3ubuntu2`

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

### `dpkg` source package: `libxext=2:1.3.4-1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.4-1`
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

### `dpkg` source package: `libxml2=2.9.12+dfsg-5`

Binary Packages:

- `libxml2:amd64=2.9.12+dfsg-5`
- `libxml2-dev:amd64=2.9.12+dfsg-5`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.12+dfsg-5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12+dfsg-5.dsc' libxml2_2.9.12+dfsg-5.dsc 2576 SHA512:6204f92961d2202a1d5f02d935d267097bc5bbcb9810ba4ea91f018628ef4c8bdc08a1d707750bfd3e9438e039d333c2e1bccd4d213ffc7b3015f461f3a390d5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12+dfsg.orig.tar.xz' libxml2_2.9.12+dfsg.orig.tar.xz 2535044 SHA512:08ffb640e5669b52b29817887d62ef698799570ee5757612826e00aa5237ebf16b13bf838c350aff0ac1081547458d6d1aa6473f3499db7bf87e1f6d39f76386
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.12+dfsg-5.debian.tar.xz' libxml2_2.9.12+dfsg-5.debian.tar.xz 32960 SHA512:c0676d74178e3f38dff76d052501471ff6899cee16c2b399560de1e63ba5dfeed247ca17ad8803f101a05c8adde395678cba53826b5f8725ee464fb596874cfb
```

### `dpkg` source package: `libxrender=1:0.9.10-1build3`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1build3`
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

- `libxslt1-dev:amd64=1.1.34-4build1`
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

### `dpkg` source package: `libxt=1:1.2.0-1build1`

Binary Packages:

- `libxt-dev:amd64=1:1.2.0-1build1`
- `libxt6:amd64=1:1.2.0-1build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.0-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0-1build1.dsc' libxt_1.2.0-1build1.dsc 2347 SHA512:013853d276cecc65f6fb462c6a38aaab9458d8b133b7f5542a7dc3ccf8cc716d41a7edc5ab96bdfe60c897f5012a05afe896ef3594e35aa7acd58fd952cc3443
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz' libxt_1.2.0.orig.tar.gz 1016961 SHA512:af8147becd98c956e9324b765151f46352cafa1f962c7d1517b18b5d27aa80d093cc3ceabd92c0f181485540987b7e46b18baf38ffe1eadf3f60ab66c3f66c52
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0.orig.tar.gz.asc' libxt_1.2.0.orig.tar.gz.asc 195 SHA512:a105f63f0fdcdddea75024e869dbe271d4261703616d5d2a3393943bf20b72fc70e9c52382dcc0370d2460737fda6f4bcaac3fa7eb84e2f6e234aa358758a13a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.2.0-1build1.diff.gz' libxt_1.2.0-1build1.diff.gz 31231 SHA512:b29ef8edfd5e05c1274760ff34be2a98a9145e8e44906c88bffc50a988851a023ca58b641a1e64ba154e2d264e4a1ac3ad980c7c0245b4fdffc860de86c95b32
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
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-3.dsc' libzstd_1.4.8+dfsg-3.dsc 2291 SHA512:54e17fdc2882d49265739bb844f21e7e07e50873d0aba149ba6e6d11f15dd03040c63652f57164bd00e21cec9922f14074f48628cf158f30a667a63c3004b117
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg.orig.tar.xz' libzstd_1.4.8+dfsg.orig.tar.xz 1331996 SHA512:07fabe431367eea4badae7b1e46ac73e0b33aad5b67361bc7b67d5f9aef249c51db5b560f1cf59233255cc49db341a8d8440fed87745026fca7a7c5c14448cd8
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.8+dfsg-3.debian.tar.xz' libzstd_1.4.8+dfsg-3.debian.tar.xz 12184 SHA512:b006d4c1ef6c687331dfb4d585227262a51f6578a4faa2cea9224fdfbdfcc61dd0f1e4fdbf453617ebb2c3dc68ec09bfebf27e3631b6fd0aa20e87c44bffbaef
```

### `dpkg` source package: `linux=5.15.0-17.17`

Binary Packages:

- `linux-libc-dev:amd64=5.15.0-17.17`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris linux=5.15.0-17.17
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0-17.17.dsc' linux_5.15.0-17.17.dsc 7529 SHA512:71007c9dd30315900489a8a9a3821ef48c7a1443c38105519a60bef02ceec7f2e3d009f3c4db414d5c8c0c08af40e6236fbefc325cc4746562af2dec53a9bbcd
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0.orig.tar.gz' linux_5.15.0.orig.tar.gz 194969557 SHA512:ae9a32132d5988441c189157703b0f8fa4e232d8d24f7104f944c06827db740beafae55eb37a51eb99b4ac513927cd372321fa1e84afff4d450b786e44414861
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.15.0-17.17.diff.gz' linux_5.15.0-17.17.diff.gz 4935512 SHA512:710ce2716201bea6b8a64a4a20a64fe53ef2171c9746fa4e87abf6f7e6602b8c52b709f07ccffe8cdfa983a5c57a6727ef0743055234ace96d2fedae2ee7ebc9
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

### `dpkg` source package: `lto-disabled-list=18`

Binary Packages:

- `lto-disabled-list=18`

Licenses: (parsed from: `/usr/share/doc/lto-disabled-list/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lto-disabled-list=18
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_18.dsc' lto-disabled-list_18.dsc 1435 SHA512:dbc72a3bd4023a5039a6768dc0b71a73525f014d2e75a611bba64c9f13cee4b329a3f3181fba85fc15e9e006e0df8a90637c07eb46f8a5a9dab364ed197defe3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lto-disabled-list/lto-disabled-list_18.tar.xz' lto-disabled-list_18.tar.xz 11984 SHA512:9a01d85400b9141bb431f3d03de8afa2b1604dc0525a796711f1683750f6478676e63a445912f57f8d6e12ee481c3ba83430e07ef41f14bc0e1ac06457edfd0f
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

### `dpkg` source package: `lzo2=2.10-2build2`

Binary Packages:

- `liblzo2-2:amd64=2.10-2build2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.10-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2build2.dsc' lzo2_2.10-2build2.dsc 1975 SHA512:13ecf06e59b26905248b8a02ab5a7cfed6b45026a9d2851bdeae90d47a8a248d4f1361c600ee429ef7ce4988f9104875f501235d3c33d7f8128e43552c596c82
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10.orig.tar.gz' lzo2_2.10.orig.tar.gz 600622 SHA512:a3dae5e4a6b93b1f5bf7435e8ab114a9be57252e9efc5dd444947d7a2d031b0819f34bcaeb35f60b5629a01b1238d738735a64db8f672be9690d3c80094511a4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2build2.debian.tar.xz' lzo2_2.10-2build2.debian.tar.xz 6968 SHA512:3ec0b4fba3e596b6b8fdbd74321230b34833306152dc3222e06227df08eaa8447ea0ba089156a2223389a2ed865f70a19e4cb562dd38d1aa8d73b5d795e7d4d9
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

### `dpkg` source package: `make-dfsg=4.3-4ubuntu2`

Binary Packages:

- `make=4.3-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.3-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu2.dsc' make-dfsg_4.3-4ubuntu2.dsc 2143 SHA512:0cb3fb17d059735b9954247cb7abae3cf96dddff1fe9f14ca2a42dab7cc90c238bd282ee55b90a62cbc5d9255faa69ba365066eede12e15e5607d833ce02e583
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA512:bdc150f9d256145923380d6e7058ab9b2b4e43fcb1d75ab2984fa8f859eab6852a68e4ea5f626633e0bec76fbebf1477378e268e8ffdb5cb2a53b29cbc439bc1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.3-4ubuntu2.diff.gz' make-dfsg_4.3-4ubuntu2.diff.gz 51126 SHA512:b1083caeb4c854c0f2f19637371e26de62db3367c21ad3c24edfd73088ced8eb7a6633d2d22ac8a8a70574be053d6931eacf62fd83456b8a233323d7c1d8a8d4
```

### `dpkg` source package: `mawk=1.3.4.20200120-2build1`

Binary Packages:

- `mawk=1.3.4.20200120-2build1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `mysql-8.0=8.0.27-0ubuntu0.21.10.1`

Binary Packages:

- `libmysqlclient-dev=8.0.27-0ubuntu0.21.10.1`
- `libmysqlclient21:amd64=8.0.27-0ubuntu0.21.10.1`

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
$ apt-get source -qq --print-uris mysql-8.0=8.0.27-0ubuntu0.21.10.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.27-0ubuntu0.21.10.1.dsc' mysql-8.0_8.0.27-0ubuntu0.21.10.1.dsc 3517 SHA512:ec061cdaeed863fafb147b9ac3949140a7f0706e4d031045ac6222568af839946a6c28089bb3a18eea031cb234733af42d838a649017d08dd7fbae4badcb10d4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.27.orig.tar.gz' mysql-8.0_8.0.27.orig.tar.gz 292184025 SHA512:6ef2426c0bee46bdf8e2fa5cb159d5ae19f0bed4f7c9bea9b33e0dd922b568c3c68ca063dcbcd7ea6904aaea31877c10064ea10b4bc63fb40d9f31778e3a7891
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.27-0ubuntu0.21.10.1.debian.tar.xz' mysql-8.0_8.0.27-0ubuntu0.21.10.1.debian.tar.xz 158840 SHA512:57f56d98ef49ab731815e922fe9da8635122855876e48622d47f9aea3e5b3f8463c9d501f43b9ce7b06708a3c2761475546ec1b75151d260a3dd2e34a6168064
```

### `dpkg` source package: `mysql-defaults=1.0.7`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.7`
- `mysql-common=5.8+1.0.7`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.7.dsc' mysql-defaults_1.0.7.dsc 2266 SHA512:9acf6dfbafcac002226c8780a5323110fc11f51f5421a62825ec7eb4cf3ce96da15667fef01f5e4267b23cb78ea19d25ce781c2597cf8f177d1b31cade19e34a
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.7.tar.xz' mysql-defaults_1.0.7.tar.xz 7220 SHA512:497fedc48b4252ed1f0351ce0be20ce195069b1ec0acf52690a05f3785b22c6c2eee2379d77ce7c75c1ce16e96daaf365ded9539a084cac1d810bf0e4c6ce6fb
```

### `dpkg` source package: `ncurses=6.3-1`

Binary Packages:

- `libncurses-dev:amd64=6.3-1`
- `libncurses5-dev:amd64=6.3-1`
- `libncurses6:amd64=6.3-1`
- `libncursesw5-dev:amd64=6.3-1`
- `libncursesw6:amd64=6.3-1`
- `libtinfo6:amd64=6.3-1`
- `ncurses-base=6.3-1`
- `ncurses-bin=6.3-1`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/ncurses/6.3-1/


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

### `dpkg` source package: `numactl=2.0.14-3ubuntu1`

Binary Packages:

- `libnuma1:amd64=2.0.14-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.14-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14-3ubuntu1.dsc' numactl_2.0.14-3ubuntu1.dsc 2081 SHA512:1d2429d28f0a5dacdd15d92a124e9bbb81b376b43574c4068ff3b6387ba83226ebbc4f8ede36b7108dbf2fb42f64c74bd546c9beab1230824efd71fa8ed8ab4c
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14.orig.tar.gz' numactl_2.0.14.orig.tar.gz 107583 SHA512:adaf405f092fd9653f26d00f8c80cb83852c56ebd5d00e714e20d505008e74aa7105b0fb7aa55a605deac0d1491ceff57de931037d33e7944fca105bc6510ed4
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.14-3ubuntu1.debian.tar.xz' numactl_2.0.14-3ubuntu1.debian.tar.xz 7528 SHA512:f0ce271e1dde18e951282773cec74b303d12e05e2dc7c98ab2045431cc6309a5aca7ea48c1f3f809527de70eaf43cddd883dc47c738da8aaf0ee6d23473950dd
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

### `dpkg` source package: `openldap=2.5.6+dfsg-1~exp1ubuntu1`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.6+dfsg-1~exp1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.6+dfsg-1~exp1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.6+dfsg-1~exp1ubuntu1.dsc' openldap_2.5.6+dfsg-1~exp1ubuntu1.dsc 3271 SHA512:716911cf25db3768f630de553c6fcf6a433aa9e936ba21cc32234754373dfafd7428c869035e81149434ce050e07db51d9351b86ec2555ee1d524b2818139424
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.6+dfsg.orig.tar.gz' openldap_2.5.6+dfsg.orig.tar.gz 5570324 SHA512:f2b3c9abe53176360847563e4864eab63434671653d74b07a9ce69ff75771716d0deca58d66291c6e582f576ce6daf4588261105e307b23df0d6cdf3254d33f9
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.5.6+dfsg-1~exp1ubuntu1.debian.tar.xz' openldap_2.5.6+dfsg-1~exp1ubuntu1.debian.tar.xz 170828 SHA512:c5943df92305cf4f0a39c80fc48689c4eb5604399ffa636987f60e7f69788e6acb8752e51acc7a04fd9333a0b117c57849db4c52669d7c62c03f93bcbeaf9817
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

### `dpkg` source package: `openssl=1.1.1l-1ubuntu1`

Binary Packages:

- `libssl1.1:amd64=1.1.1l-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openssl=3.0.1-0ubuntu1`

Binary Packages:

- `libssl-dev:amd64=3.0.1-0ubuntu1`
- `libssl3:amd64=3.0.1-0ubuntu1`
- `openssl=3.0.1-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libssl-dev/copyright`, `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

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

### `dpkg` source package: `pango1.0=1.50.3+ds1-3`

Binary Packages:

- `libpango-1.0-0:amd64=1.50.3+ds1-3`
- `libpangocairo-1.0-0:amd64=1.50.3+ds1-3`
- `libpangoft2-1.0-0:amd64=1.50.3+ds1-3`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pango1.0/1.50.3+ds1-3/


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

- `libpcre2-16-0:amd64=10.39-3`
- `libpcre2-32-0:amd64=10.39-3`
- `libpcre2-8-0:amd64=10.39-3`
- `libpcre2-dev:amd64=10.39-3`
- `libpcre2-posix3:amd64=10.39-3`

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

- `libpcre16-3:amd64=2:8.39-13build4`
- `libpcre3:amd64=2:8.39-13build4`
- `libpcre3-dev:amd64=2:8.39-13build4`
- `libpcre32-3:amd64=2:8.39-13build4`
- `libpcrecpp0v5:amd64=2:8.39-13build4`

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
- `libpixman-1-dev:amd64=0.40.0-1build3`

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

### `dpkg` source package: `postgresql-14=14.1-1ubuntu1`

Binary Packages:

- `libpq-dev=14.1-1ubuntu1`
- `libpq5:amd64=14.1-1ubuntu1`

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
$ apt-get source -qq --print-uris postgresql-14=14.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-14/postgresql-14_14.1-1ubuntu1.dsc' postgresql-14_14.1-1ubuntu1.dsc 3657 SHA512:36fd7d896f45eceacd16c2d6a79cd72a7fb54cccfd01ba752cb4517199a4ea7dc3c1a95dc13d4847f3dd98d1cec9ead3ffef67e39d7cc635294701184978c09f
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-14/postgresql-14_14.1.orig.tar.bz2' postgresql-14_14.1.orig.tar.bz2 21887101 SHA512:4a0bec157d5464bb9e5f5c0eb0efdede55526e03f6f4d660b87d161a47705eb152fa0878960b1581bce42a5ed28a1f457825ea54e8d22e34b5b8eb36473ceefd
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-14/postgresql-14_14.1-1ubuntu1.debian.tar.xz' postgresql-14_14.1-1ubuntu1.debian.tar.xz 26184 SHA512:16951a3dd72910cfce1af42404879f22a2e4a26394896562dba001565aff8b936b6b713b1b4d7106e9652ad11a35920f828c88507290ba0672f4e6bd88e7043b
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

### `dpkg` source package: `python3-stdlib-extensions=3.9.9-3`

Binary Packages:

- `python3-distutils=3.9.9-3`
- `python3-lib2to3=3.9.9-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-stdlib-extensions/3.9.9-3/


### `dpkg` source package: `python3.9=3.9.9-2`

Binary Packages:

- `libpython3.9-minimal:amd64=3.9.9-2`
- `libpython3.9-stdlib:amd64=3.9.9-2`
- `python3.9=3.9.9-2`
- `python3.9-minimal=3.9.9-2`

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

- http://snapshot.debian.org/package/python3.9/3.9.9-2/


### `dpkg` source package: `readline=8.1.2-1`

Binary Packages:

- `libreadline-dev:amd64=8.1.2-1`
- `libreadline8:amd64=8.1.2-1`
- `readline-common=8.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.1.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.dsc' readline_8.1.2-1.dsc 2432 SHA512:3166229d2ac183a46455c7d8cf17ef1d509ca8651ffa7887f654d87bbe1d00a08f9a9f73f14e652ac067d89e5d1128998f8f09f6a1128c56049338ace65ed773
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2.orig.tar.gz' readline_8.1.2.orig.tar.gz 2993073 SHA512:b512275c8aa8b3b3178366c6d681f867676fc1c881e375134a88e9c860a448535e04ca43df727817fd0048261e48203e88bd1c086e86572022d1d65fb0350e4d
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.1.2-1.debian.tar.xz' readline_8.1.2-1.debian.tar.xz 29292 SHA512:a64621c93975bc42ba171c9298c932f9515025513911e744183092e0ef9873db474c4ec27a21f310f40e7b970ba6300edb057552f7e90fc469897ffa2eb706f0
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

### `dpkg` source package: `shared-mime-info=2.1-2`

Binary Packages:

- `shared-mime-info=2.1-2`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=2.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.1-2.dsc' shared-mime-info_2.1-2.dsc 2223 SHA512:292d45d7847f5b6de7583f6c24c5ef019169e1bc6b54e5415d2dc0df203136624b7eb3e20040019608fe392468967c31e15d100f9eaa75e052d342d2aa1465c9
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.1.orig.tar.xz' shared-mime-info_2.1.orig.tar.xz 5202496 SHA512:87e308281e83c4cf889594f7c2e8dcb4d0d0d3910124c3816fdb886ba7d6113b2581711adcb17032b47f9b8d8b7001fab58daa52b7da7c0ef87915e341d6f1b0
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_2.1-2.debian.tar.xz' shared-mime-info_2.1-2.debian.tar.xz 11304 SHA512:833518eb333d0bb03018299db5e21b5e9f38d9c89680f86aab9e03289ef7d056ff74b3bdb5f7fb364f990b61bc8f264f2b4113edf59ecb1ef7c72f83970f1a25
```

### `dpkg` source package: `sqlite3=3.36.0-2`

Binary Packages:

- `libsqlite3-0:amd64=3.36.0-2`
- `libsqlite3-dev:amd64=3.36.0-2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sqlite3/3.36.0-2/


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

### `dpkg` source package: `systemd=249.5-2ubuntu2`

Binary Packages:

- `libsystemd0:amd64=249.5-2ubuntu2`
- `libudev1:amd64=249.5-2ubuntu2`

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


### `dpkg` source package: `sysvinit=2.96-7ubuntu2`

Binary Packages:

- `sysvinit-utils=2.96-7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-7ubuntu2.dsc' sysvinit_2.96-7ubuntu2.dsc 2718 SHA512:6543be6337ed7fdca82f62ec790c8ba7a3936cbe798975a0a38f7d7dad8132e30b3bec6688a3da3e1efb634030996cec48770dfa717178064d2558953d9424de
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA512:1388398568ebfe53460796f8ab75a3ead6111612888ea36e8f1c0db4d41ef6f45fc217abb7804519ff1143a78d97c95b24e42c8c22c95a47b9436484bfb6f45d
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA512:2b3798e8fc8531cd1a2b2a523159b7f064bfadd8815b930fb70d5a1380775f1b5bac5627d5cd9d95b03ff3737d8d6b2f357c6bc21ac2e21ee089b67f98b4eb6a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-7ubuntu2.debian.tar.xz' sysvinit_2.96-7ubuntu2.debian.tar.xz 129696 SHA512:6f81ac49fba5e42d77e80cda39263c5b02537f801ae4c784ac1b4e2c8ff9ec523b2465d5cfcf84e00d36098d71ab4a58fd23c608701ef1aa2d4ba1742809f7be
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

### `dpkg` source package: `tiff=4.3.0-2`

Binary Packages:

- `libtiff-dev:amd64=4.3.0-2`
- `libtiff5:amd64=4.3.0-2`
- `libtiffxx5:amd64=4.3.0-2`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.3.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0-2.dsc' tiff_4.3.0-2.dsc 2429 SHA512:6f4554979fe3a2bf1a871d2de81ea006a05a3bf2bfbaee76481dca501d42e9ea14c97987bafdbff853b6ab1bb6a68560aee2024b1a47c3da05a81c8235b79704
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz' tiff_4.3.0.orig.tar.gz 2808254 SHA512:e04a4a6c542e58a174c1e9516af3908acf1d3d3e1096648c5514f4963f73e7af27387a76b0fbabe43cf867a18874088f963796a7cd6e45deb998692e3e235493
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0.orig.tar.gz.asc' tiff_4.3.0.orig.tar.gz.asc 488 SHA512:115a4c5714b52d0fbea800c494d83c8a96b70b2c9ce84a8df03205d9afc517faa17963f5f9508c013d7d3e2be6675b84b594a771a829406473234c4bd85e469e
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.3.0-2.debian.tar.xz' tiff_4.3.0-2.debian.tar.xz 19596 SHA512:cb1417ca9d9fe35537bd8067e348e196efbadcdd1439f9f365e9a62d330a0e4f1b8e87c3c9dc4644d9da6ef5f62a4a0cca7f0eb99f305e9a7bd137565878d42f
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

### `dpkg` source package: `unzip=6.0-26ubuntu2`

Binary Packages:

- `unzip=6.0-26ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-26ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-26ubuntu2.dsc' unzip_6.0-26ubuntu2.dsc 1828 SHA512:bfb7b96858f95d21c40aa28d8309c00bbfe1f0ca44b66e6151081de64ccf09aa205c6785cb95c5ba0aebce73353ad4b54e3f9f507bcac6abd479def529e409de
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA512:0694e403ebc57b37218e00ec1a406cae5cc9c5b52b6798e0d4590840b6cdbf9ddc0d9471f67af783e960f8fa2e620394d51384257dca23d06bcd90224a80ce5d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-26ubuntu2.debian.tar.xz' unzip_6.0-26ubuntu2.debian.tar.xz 27008 SHA512:218ca546b85b88e0421abe3522db2205dcbd18767fe68e147e060d5e73544e541295cc05bc5ff17b7778c6f50499a265b5425ffc2b024f7bd472bfd6e3207b9d
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
- `libblkid-dev:amd64=2.37.2-4ubuntu1`
- `libblkid1:amd64=2.37.2-4ubuntu1`
- `libmount-dev:amd64=2.37.2-4ubuntu1`
- `libmount1:amd64=2.37.2-4ubuntu1`
- `libsmartcols1:amd64=2.37.2-4ubuntu1`
- `libuuid1:amd64=2.37.2-4ubuntu1`
- `mount=2.37.2-4ubuntu1`
- `util-linux=2.37.2-4ubuntu1`
- `uuid-dev:amd64=2.37.2-4ubuntu1`

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
$ apt-get source -qq --print-uris util-linux=2.37.2-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2-4ubuntu1.dsc' util-linux_2.37.2-4ubuntu1.dsc 4567 SHA512:2245ab47b726712f741ac209c8c1eaed6ba2496070c618abba228b680fe20799de436aa6d54907e669c356a4eceb839d1623a0e3ab904ca8069c10f359fb366e
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2.orig.tar.xz' util-linux_2.37.2.orig.tar.xz 5621624 SHA512:38f0fe820445e3bfa79550e6581c230f98c7661566ccc4daa51c7208a5f972c61b4e57dfc86bed074fdbc7c40bc79f856be8f6a05a8860c1c0cecc4208e8b81d
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.37.2-4ubuntu1.debian.tar.xz' util-linux_2.37.2-4ubuntu1.debian.tar.xz 102856 SHA512:a8d4de10770d8f529ccfb38626e6fdaeb8619881ecffa4bbe109d118b992471f4246189474152c411de60a5e2914800ab5f545ea45c317ae539009f74257a670
```

### `dpkg` source package: `wget=1.21-1ubuntu5`

Binary Packages:

- `wget=1.21-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21-1ubuntu5.dsc' wget_1.21-1ubuntu5.dsc 2223 SHA512:aed99207de9ad2bcef7c9174e88d206290b78e1ad133430167affe27bce59a68c428af504fe999d16e37dc56458a1966ae8ad3fe37fe235430612413eb6ff700
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.orig.tar.gz' wget_1.21.orig.tar.gz 4866788 SHA512:13313a98f91ef34ad90103f076285549eb4887d77953e9f192d3b0667642b5ceb9e2e30091f766cbf1d6ed423499c497ed85d826f3f3e92f0711aa06d8303c5a
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21.orig.tar.gz.asc' wget_1.21.orig.tar.gz.asc 854 SHA512:1bdaedc164800158625fddbc842c2cbe246d3e3c2f07546ecebacc8c1ea44779aab31a707d792f965669f2403941d4869e59719198563a0f39099145609310d1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.21-1ubuntu5.debian.tar.xz' wget_1.21-1ubuntu5.debian.tar.xz 63564 SHA512:995e2a6309fd73d453f237db049c013339cbf0d0ae7dd18f191999f036ec97d0fdf29658666ab761f6c33a421ef99f0498c331a2b5777e41ec42a12821efdb70
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

### `dpkg` source package: `xorg=1:7.7+23ubuntu1`

Binary Packages:

- `x11-common=1:7.7+23ubuntu1`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+23ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+23ubuntu1.dsc' xorg_7.7+23ubuntu1.dsc 2066 SHA512:bb74afaaa991e04df01a48960f6bda0f0106009e39d44420d573debe5a884374721d56c998e9ef2f08352c11e1d73d9412b9ba167caabf2053e96381b9639d01
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+23ubuntu1.tar.gz' xorg_7.7+23ubuntu1.tar.gz 295648 SHA512:be0ad038680ea696369d7c9bf6e42c94c2bd110ab4543b1728f4691087fce9c0817f77e4d00d768d189350b4979bcbfe548af445e076e2b89ff993bc81be1175
```

### `dpkg` source package: `xorgproto=2021.5-1`

Binary Packages:

- `x11proto-dev=2021.5-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2021.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2021.5-1.dsc' xorgproto_2021.5-1.dsc 3157 SHA512:00c2d84a7f77f32ac381813f884624b7ec5938b5663627230c545c723944182d36b1ec875a554b5ab258bec0a87dff12c3d31ce87e8520fce8e9ea67e547d5de
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2021.5.orig.tar.gz' xorgproto_2021.5.orig.tar.gz 1132811 SHA512:9c9ec62f0af68fd0dff24010986326a2b201be2b56b8b94abfe7258bf66b3c4c37088596c43a234aae63b1d781f7797caf408e434c98e8805803bc890b8aacb0
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2021.5-1.diff.gz' xorgproto_2021.5-1.diff.gz 22934 SHA512:c48bd4e4bf3d8525cc4e8bb98c7829f519eec0c03ab0dbad1b95cc08d496bf76a4b98a2f3a6fa5203e4bd07c2a354719fbd52be0b310e646df12e3b2eb1407e6
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `xz-utils=5.2.5-2build1`

Binary Packages:

- `liblzma-dev:amd64=5.2.5-2build1`
- `liblzma5:amd64=5.2.5-2build1`
- `xz-utils=5.2.5-2build1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.5-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2build1.dsc' xz-utils_5.2.5-2build1.dsc 2535 SHA512:290381e339adda8dbe75872360a51097b6107a2715406436ecad9f03c758b53bcfec77437afa6a3306e871ee696b144c992cf988cbf162f83a1b54dbff804bc9
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz' xz-utils_5.2.5.orig.tar.xz 1148824 SHA512:59266068a51cb616eb31b67cd8f07ffeb2288d1391c61665ae2ec6814465afac80fec69248f6a2f2db45b44475af001296a99af6a32287226a9c41419173ccbb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5.orig.tar.xz.asc' xz-utils_5.2.5.orig.tar.xz.asc 833 SHA512:582864ae306861ede34074ebfd23ab161ad3340ab4a068f727583de2bd2058da70dfe73019f4e70b8267e0e0c62f275da1e23f47d40c0b80038449b0ac335020
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.5-2build1.debian.tar.xz' xz-utils_5.2.5-2build1.debian.tar.xz 33600 SHA512:121bccaca745872de67d3c78fe38cd33f9f6fed9b2b32269fdc6852efcd3b153f21513e1c03f1157db19bca220ece82575c1b2e542d440c6eab01b495fc5b8af
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
