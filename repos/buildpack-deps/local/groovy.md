# `buildpack-deps:groovy`

## Docker Metadata

- Image ID: `sha256:28c1b94304c665567e6be849d428c385271d854c8d324c1a35844779e27a280f`
- Created: `2020-09-25T23:33:42.129980326Z`
- Virtual Size: ~ 716.09 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-8`

Binary Packages:

- `libacl1:amd64=2.2.53-8`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-8
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-8.dsc' acl_2.2.53-8.dsc 2464 SHA512:ea1317e5b8877acc7cb445b52be0c2cc56c062a76d50277fffd5bdd32b851670434ab2e36b1b9137c2ef127234ba65304d3752d76c787f33e1559b5f85752477
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA512:176b7957fe0e7618e0b7bf2ac5071f7fa29417df718cce977661a576fa184e4af9d303b591c9d556b6ba8923e799457343afa401f5a9f7ecd9022185a4e06716
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA512:a76dcc4f9952bb809aed3c8e0d26e9ae1aa8098ec8492c4d95a23ab74ec92d6896f1eb6307a555098277aa1191cc01d75a2f6a35dd8e8ccb46d3155404bc6f22
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-8.debian.tar.xz' acl_2.2.53-8.debian.tar.xz 25300 SHA512:903dbaff5838fb37bbe96a813cf2a0b5ecbbcdf67da0699d81c49ece777feb5afb1f16e47e2744476f589534fae4a216fbcac4b20126023d0cb6642220260691
```

### `dpkg` source package: `adduser=3.118ubuntu2`

Binary Packages:

- `adduser=3.118ubuntu2`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.118ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.dsc' adduser_3.118ubuntu2.dsc 1131 SHA512:c6a2226a509c17b2b7ec23fa474a10e3afce3259f8b244cf748ef9d8e88fa500f7e1d84145fd0e7d01d6e2782787430cd46130eb556df69c5c1611aaa26a94c7
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.tar.xz' adduser_3.118ubuntu2.tar.xz 222364 SHA512:6236481388a235723c74575cb987a403ee62536f10dd02262c4cf168174269d7c83a2e444ca2efb33ccf0bf430c1773189364609f295de3e8708f9a7c9d378fa
```

### `dpkg` source package: `apr-util=1.6.1-4ubuntu2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.dsc' apr-util_1.6.1-4ubuntu2.dsc 2686 SHA512:4328cc953496e8bce9170d057c06aeb1e6d1b107a7c1263945a50fa98861da8fa0105594c026e58a7ea881b5d5d4d2bad6e39144e8ba0d6bf29d0c3b3d6be185
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA512:40eff8a37c0634f7fdddd6ca5e596b38de15fd10767a34c30bbe49c632816e8f3e1e230678034f578dd5816a94f246fb5dfdf48d644829af13bf28de3225205d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.debian.tar.xz' apr-util_1.6.1-4ubuntu2.debian.tar.xz 213052 SHA512:3087e6b575ee2d01fb320ebcc200b295c637fba7019b78652a0953bdb19cba184b5c2eea771ca7e4b549ecaf3988a17cb339863235ead0e77ba98a9ff0e4861e
```

### `dpkg` source package: `apr=1.6.5-1ubuntu1`

Binary Packages:

- `libapr1:amd64=1.6.5-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.5-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.dsc' apr_1.6.5-1ubuntu1.dsc 2390 SHA512:9a17bac02906eb32172e67e811f99fc0d68ac01dfb896f6fed49776d9b92736b30013e68ab950315f1b442b7a33b5536e21b8d8fd87dc83428c8dc7792377c5e
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2' apr_1.6.5.orig.tar.bz2 855393 SHA512:d3511e320457b5531f565813e626e7941f6b82864852db6aa03dd298a65dbccdcdc4bd580f5314f8be45d268388edab25efe88cf8340b7d2897a4dbe9d0a41fc
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2.asc' apr_1.6.5.orig.tar.bz2.asc 801 SHA512:9a168a31d38f0703aaf796ab1d55a0439e779e9cd0017dfcafd4217081a150db28799da546b861f7967eb839d4afa563c37906d8c4be48f19b66bc699bc036a7
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.debian.tar.xz' apr_1.6.5-1ubuntu1.debian.tar.xz 213596 SHA512:83e7a6b7b57ccc1e53d1b650b749b245a7c5f5d7e7f00b3a59bc3179f588225746e8fd5cddd15d5e20b44758b42905e67ccd1cebaf789e4f37a855e436ffd979
```

### `dpkg` source package: `apt=2.1.10`

Binary Packages:

- `apt=2.1.10`
- `libapt-pkg6.0:amd64=2.1.10`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.1.10
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.1.10.dsc' apt_2.1.10.dsc 2760 SHA512:fee6ee60ca70c95038ae2884710b4844845006d94a30c69252ae3326f3cc24ef142ecc4a648f707d23d678d4f07d4d3522fa035ed7fb5ae8a0123b19550f4bbd
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.1.10.tar.xz' apt_2.1.10.tar.xz 2179772 SHA512:f620e3373c0c19c237f7c40f15dc86d9f0c31aa0578a0f38d3f2cb65b7e7d16689a048574dc05b8729b0bef501c2e0d0e85e567ebfc47830334da0cd7540c84f
```

### `dpkg` source package: `attr=1:2.4.48-5`

Binary Packages:

- `libattr1:amd64=1:2.4.48-5`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.48-5
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.dsc' attr_2.4.48-5.dsc 2433 SHA512:a4b97acde8c985a74c33c15c9d5b76ca474810b7066f896626ef9b8014b789b71a0769f58ce830f0909a0ff284c0fbc9b85c42b4a3580dd5a878bc69a6d62594
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA512:75f870a0e6e19b8975f3fdceee786fbaff3eadaa9ab9af01996ffa8e50fe5b2bba6e4c22c44a6722d11b55feb9e89895d0151d6811c1d2b475ef4ed145f0c923
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA512:39e5879d4879003ba5e1fcb727f91f7661cede12692ae128110328a6c1c5a1e2f79a1329ee4d065f3cc3e0d3d18423f5b5a5b170b5cb49c6888de90d31dcaf9c
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.debian.tar.xz' attr_2.4.48-5.debian.tar.xz 25560 SHA512:e86a1913d5fdbd6d39a1af776a244a849aa6c7bd20c398b9d9e5512b013c5b47a98e5330b6b182b7811d1e820f46d2a593a2a5486c89fb9584edfda3a21ff49d
```

### `dpkg` source package: `audit=1:2.8.5-3ubuntu1`

Binary Packages:

- `libaudit-common=1:2.8.5-3ubuntu1`
- `libaudit1:amd64=1:2.8.5-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.5-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-3ubuntu1.dsc' audit_2.8.5-3ubuntu1.dsc 2829 SHA512:f692829dbd385cc6f9be47220fba5351f2915bcfb69da5fa06cfadc19084fff1f13d9c62f04f7e58c359a503e3f39d3e962cdf0ff2527c60a97b98291bc78811
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5.orig.tar.gz' audit_2.8.5.orig.tar.gz 1140694 SHA512:7d416aaa21c1a167f8e911ca82aecbaba804424f3243f505066c43ecc4a62a34feb2c27555e99d3268608404793dccca0f828c63670e3aa816016fb493f8174a
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-3ubuntu1.debian.tar.xz' audit_2.8.5-3ubuntu1.debian.tar.xz 19940 SHA512:b579712160f8313078a2a9e961b29d9126168543e6dd40de9ba337579885ea25c78119cedc7a50591408139d8235af6ce10450c3b2bf0ed1365ca951be2cdf54
```

### `dpkg` source package: `autoconf=2.69-11.1`

Binary Packages:

- `autoconf=2.69-11.1`

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
$ apt-get source -qq --print-uris autoconf=2.69-11.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.1.dsc' autoconf_2.69-11.1.dsc 1735 SHA512:b3f3f441f3a23d57b4a664286ce9eda0a9de178bf9dd4a4a40cafcd27578dbad1ffa187044f9b049ac8fcb64644450383945fa9bb47cea1c75ff5d0f29b10941
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA512:995d3e5a8eb1eb37e2b7fae53c6ec7a9b4df997286b7d643344818f94636756b1bf5ff5ea9155e755cb9461149a853dfbf2886fc6bd7132e5afa9c168e306e9b
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.1.debian.tar.xz' autoconf_2.69-11.1.debian.tar.xz 23488 SHA512:2f3f361b60b60bc852c6fc5db81271e76d5139a6eec89196b1643e1e55f9581f17ed92a0f71b8bf9ccbf1a05f1dad2664986604e384ed8f2fdea51a651844e0c
```

### `dpkg` source package: `automake-1.16=1:1.16.2-4ubuntu1`

Binary Packages:

- `automake=1:1.16.2-4ubuntu1`

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
$ apt-get source -qq --print-uris automake-1.16=1:1.16.2-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2-4ubuntu1.dsc' automake-1.16_1.16.2-4ubuntu1.dsc 2583 SHA512:b2c2815901a6efc73acee269f4c25ce38c1e9e06930846a0f7c6b85698bf244bc995d9ffac01b898241109e0b875717f24479c9da7886f0202bd5e0b10158e82
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2.orig.tar.xz' automake-1.16_1.16.2.orig.tar.xz 1545912 SHA512:a4aa0e41ceaa7df5bc303a6004597fb158f4198594017cd2c586fd9f5a29233e081766bf22b7e4ef0d4c8c3d45a8591009427efa319b362922a958ac1ef6e27b
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2.orig.tar.xz.asc' automake-1.16_1.16.2.orig.tar.xz.asc 833 SHA512:a672e13249175d5ebe0c6515b4ef185552b8000ec0df2b2d68012066dd66f4fbac5aebc13360ba4c9b7ca924bdf446d877eb7692afa37c996506781125337a3f
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.2-4ubuntu1.debian.tar.xz' automake-1.16_1.16.2-4ubuntu1.debian.tar.xz 13388 SHA512:e4ed313710d28fc8ad613fcf6042e3e7c910851d6d37c47d87078a792780c08a74bc31a8dee9f7a34b381bfc3544daf54eceb6e9856c8696fc7b4354b4470d8b
```

### `dpkg` source package: `autotools-dev=20180224.1`

Binary Packages:

- `autotools-dev=20180224.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.dsc' autotools-dev_20180224.1.dsc 1643 SHA512:636182e70c202dd9c0c0c5ad94f65047b40b5d763e7bc31a5fe5fb3f8150cc51547a6ded77f680c3558ba074cbfab264345b5683bc50c79b116fda588b3f3298
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.tar.xz' autotools-dev_20180224.1.tar.xz 68256 SHA512:ca96e20be9055d69477bc04e184d6dbe1a18d70f466c086f649a74271bd5d1ce88ecd22236a3dc74488fccf19aa5d584a90e9e58bf10f50fa2e62023ff6e3440
```

### `dpkg` source package: `base-files=11ubuntu13`

Binary Packages:

- `base-files=11ubuntu13`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11ubuntu13
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11ubuntu13.dsc' base-files_11ubuntu13.dsc 1672 SHA512:a4900a6bd90d7c64e7f25dabfea87bc3b9e4eff58c0b172ca3640a48c2a91819be20fa4cf11a1c203f59d6c6e0ccd2a126d34bdffcb15204c69e47a79ab6dfbc
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11ubuntu13.tar.xz' base-files_11ubuntu13.tar.xz 80824 SHA512:bc23e347377f884baca0cc5560b6595f619222cc56267d06accbf289294a63b672b69484e0678987488947ccdbd551c2801e6d8f18a064f063684dd37949b1e5
```

### `dpkg` source package: `base-passwd=3.5.47`

Binary Packages:

- `base-passwd=3.5.47`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.47
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.dsc' base-passwd_3.5.47.dsc 1757 SHA512:f921ad4a5f9c6c88f32104108467fdc287be8b75a823041bbc9a2a4f142fd02e7f99af8e075a4469857708c7d10f2284fea9885f073d6b92625e0a7e1c90b210
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.tar.xz' base-passwd_3.5.47.tar.xz 53024 SHA512:f954adf1a82982e9dd9b19c2420b37b3fcd10827fae19aaa8e7784002eb519597158fbba5ea75aba7e41ffe8d7bf31c73fea923ef7f099d007a9cb631dd159e8
```

### `dpkg` source package: `bash=5.0-6ubuntu2`

Binary Packages:

- `bash=5.0-6ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.0-6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu2.dsc' bash_5.0-6ubuntu2.dsc 2435 SHA512:670230fda5d644a3d67353e8240897ff0d3e4a6f638b0b4f037fcc4c213ca465c09ad59a5be43bdf731a0f97d744058e298362b93f904c0e81688c7615fc3605
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA512:f3a719997a8515bae7e84701afafc9b2cdd23c95d29533adb678000b08eba968450b93d5576c3cffbeccbdcd95b713db830e8efeda689258dcfe6f15f0c5dec4
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu2.debian.tar.xz' bash_5.0-6ubuntu2.debian.tar.xz 74404 SHA512:7713a48d733df407b0cbe4972b9141e742a250866fd37be57fd51c9f5c3e2e957f6a0304e68665d86c3554037b47f5a239f9cecb99405c035e9580621c12391a
```

### `dpkg` source package: `binutils=2.35.1-1ubuntu1`

Binary Packages:

- `binutils=2.35.1-1ubuntu1`
- `binutils-common:amd64=2.35.1-1ubuntu1`
- `binutils-x86-64-linux-gnu=2.35.1-1ubuntu1`
- `libbinutils:amd64=2.35.1-1ubuntu1`
- `libctf-nobfd0:amd64=2.35.1-1ubuntu1`
- `libctf0:amd64=2.35.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.35.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.35.1-1ubuntu1.dsc' binutils_2.35.1-1ubuntu1.dsc 8781 SHA512:d47c1dca5a67a7dcef4fe555370b634526e40000ad9dfefeefb8b416712bd6a632eb7b2c598f2506e54e782e67380bd34adb3166f60c423956b7e964825cca39
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.35.1.orig.tar.xz' binutils_2.35.1.orig.tar.xz 22031720 SHA512:94ff72708403413b70b247f3af4099ebaa882b6659249869f1ed9941a0f1912e313f08357d470f9fd2359e7f5e5b0eb86285e5eaf883fa8187789d6b1bd304eb
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.35.1-1ubuntu1.debian.tar.xz' binutils_2.35.1-1ubuntu1.debian.tar.xz 102184 SHA512:86d58fef0c1e9446d78e3f87add3ad070efb500cc8b5895887c269e8485ee7e3a97c83d9d1b3bfa5d73e263c482b2f00d226b3bb69404810af628b69c6038e90
```

### `dpkg` source package: `breezy=3.1.0-5build1`

Binary Packages:

- `brz=3.1.0-5build1`
- `python3-breezy=3.1.0-5build1`

Licenses: (parsed from: `/usr/share/doc/brz/copyright`, `/usr/share/doc/python3-breezy/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris breezy=3.1.0-5build1
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.1.0-5build1.dsc' breezy_3.1.0-5build1.dsc 2715 SHA512:6c4202b5ec01963a124851c8f227f765a741074692222a340d9a4bec18146873e38cf2c29efe9b4b0a17ba169aecc541e480298d908da6c207e58828748ed8d6
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.1.0.orig.tar.gz' breezy_3.1.0.orig.tar.gz 9389366 SHA512:40ea1ae364940ac8ff83d3f5da2437cc62fbda0ca98b3ae90a38dfad87555c3993b852ce186323454d7ab002ba4fbb3270e70953504e449c445efe147847204d
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.1.0-5build1.debian.tar.xz' breezy_3.1.0-5build1.debian.tar.xz 55636 SHA512:030f36c0cde15510a3daa1d25931b7ff4097e6b5da0799a3a7b0ce0c1c2b28cd2b3b45b3a499cb8b5e9cc7fa84a92e976aea932a80a3f594abf23fe441fdf0a8
```

### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli-dev:amd64=1.0.9-2`
- `libbrotli1:amd64=1.0.9-2`

Licenses: (parsed from: `/usr/share/doc/libbrotli-dev/copyright`, `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2.dsc' brotli_1.0.9-2.dsc 2261 SHA512:294514d99598c4cac58705e22994a0b82f3d78f0892766d13e2942c4e34d18824483fb2cbc0314265b8253a9ac3d8a2e2291d25baad965ed777648cd54a97a6f
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA512:b8e2df955e8796ac1f022eb4ebad29532cb7e3aa6a4b6aee91dbd2c7d637eee84d9a144d3e878895bb5e62800875c2c01c8f737a1261020c54feacf9f676b5f5
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.9-2.debian.tar.xz' brotli_1.0.9-2.debian.tar.xz 5552 SHA512:765a0bb1b1671aa31913e967dd610d3612672b2b6f75b922f92fdfb57dfca51e6c16e426ad8bfcbf40c09ac8ddbb627c07ea0ed32ca1f8b2e610472ab763b27b
```

### `dpkg` source package: `bzip2=1.0.8-4ubuntu2`

Binary Packages:

- `bzip2=1.0.8-4ubuntu2`
- `libbz2-1.0:amd64=1.0.8-4ubuntu2`
- `libbz2-dev:amd64=1.0.8-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu2.dsc' bzip2_1.0.8-4ubuntu2.dsc 2212 SHA512:bbb7850c0dca5f3c06ddd057addff1ecad68378fd448f739f8b074e039b03eeceea323ec873bf08864367f7240bddb364735f56ac15a2bc5fb4d83fdd71f83ce
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA512:083f5e675d73f3233c7930ebe20425a533feedeaaa9d8cc86831312a6581cefbe6ed0d08d2fa89be81082f2a5abdabca8b3c080bf97218a1bd59dc118a30b9f3
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-4ubuntu2.debian.tar.bz2' bzip2_1.0.8-4ubuntu2.debian.tar.bz2 26561 SHA512:6ac1e2e3e22d989ab49e8f01aab592c35dff9950e2ed4439e9df650d3cd2ed7061796bc1e76c7fe9216e2fef4e1b59991fadb508f7c7bed9178d6dcb26247f8e
```

### `dpkg` source package: `bzr=2.7.0+bzr6622+brz`

Binary Packages:

- `bzr=2.7.0+bzr6622+brz`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.7.0+bzr6622+brz
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622+brz.dsc' bzr_2.7.0+bzr6622+brz.dsc 1866 SHA512:27872f2421f71e02f7990f64bfb5cde51aa74cd9a52cd260c9979d87b21d9ce659bb9c7b6c248c07a11b3d7cb2044e59fd7baeb1769cb6c8b574c1cea84b7174
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622+brz.tar.xz' bzr_2.7.0+bzr6622+brz.tar.xz 18052 SHA512:ad06bd50262664f93e9a80356082f0470ae39218f5e7f63add6ab1683b41cf1e72b9706a86f4a151872b6ca2020c69cad8fc2bd546ba7e9d229e78963d55773e
```

### `dpkg` source package: `ca-certificates=20200601`

Binary Packages:

- `ca-certificates=20200601`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20200601
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20200601.dsc' ca-certificates_20200601.dsc 1582 SHA512:ebb9a92fe43ee91e24a1fc57276cabf2b34317af0ddb7fdab2d69d2ad96b442bbf9fe8b7feb8fbcbeda6e84d25635f6d58c37e4ce489d4b4951bc1d3887c0224
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20200601.tar.xz' ca-certificates_20200601.tar.xz 245668 SHA512:7bfd3122430be0a46bd10dcb0e0664561d1e0b2656b9f37677d89f71a1dcb0e668c25ffe08412888125fa9a53ee8245a4b3fc1004c419a159766665b1241113c
```

### `dpkg` source package: `cairo=1.16.0-4ubuntu1`

Binary Packages:

- `libcairo-gobject2:amd64=1.16.0-4ubuntu1`
- `libcairo-script-interpreter2:amd64=1.16.0-4ubuntu1`
- `libcairo2:amd64=1.16.0-4ubuntu1`
- `libcairo2-dev:amd64=1.16.0-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-4ubuntu1.dsc' cairo_1.16.0-4ubuntu1.dsc 2950 SHA512:262536534fc2de2df617ff360ba0daafb74907a694081ca0de7612b176da43a04a09ef9a0ae3c2db2ebd0f3329c1d236d8ba9d13e91ad6095015a88d7b4ef432
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA512:9eb27c4cf01c0b8b56f2e15e651f6d4e52c99d0005875546405b64f1132aed12fbf84727273f493d84056a13105e065009d89e94a8bfaf2be2649e232b82377f
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.16.0-4ubuntu1.debian.tar.xz' cairo_1.16.0-4ubuntu1.debian.tar.xz 30416 SHA512:908c4f86c37e01123d572280b093211e6d4eacfd74fbd8f88be17b18070fc48305fb2bdf9d3da4eca026a439e10228c9a466641e49c32f07285ae2948f6a3620
```

### `dpkg` source package: `cdebconf=0.252ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.252ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.252ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.252ubuntu1.dsc' cdebconf_0.252ubuntu1.dsc 2865 SHA512:e1b1b59db9889a9bdb35e3c8a0c8d7cb0d468631bfcda297063b8dde1fe5d88abc85d49eb3a36f620d7c64bcc3023dec7c3d4b919cf55a981f3702b92252b74e
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.252ubuntu1.tar.xz' cdebconf_0.252ubuntu1.tar.xz 276852 SHA512:8cff9ce56664ca71ab7a29893dfb3fe5f84ea4a8be0dd2c1ff811d7edc07a105f3c1a896825b9b30801512c867feac32ea5de38f689bc134536e526d08fb166b
```

### `dpkg` source package: `configobj=5.0.6-4`

Binary Packages:

- `python3-configobj=5.0.6-4`

Licenses: (parsed from: `/usr/share/doc/python3-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-4
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-4.dsc' configobj_5.0.6-4.dsc 2246 SHA512:6989d5184088a12b153343f48f72096798587461f0932470f329e4912eadb0a6e9405f8fc923d8ddb19158b4c5f39ff3a6f272b8bb22beb299db0f35f3b0ab74
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA512:326eb86e362f281ebf07abcb1cf7616abb270c482eafe842371cda8708245ca5e8262f1644b7164664ecc10e9004ed061c9de18cd233a657d4697dbc3ba3c59d
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-4.debian.tar.xz' configobj_5.0.6-4.debian.tar.xz 6916 SHA512:e13cedfc9c016ead9de97a44890cdc51cfc85662fae4e05b35f5a68b1d9ec420930771eb8b4f7528b09c274b551802389faad642207786382e2d5633cd50f8ed
```

### `dpkg` source package: `coreutils=8.32-3ubuntu1`

Binary Packages:

- `coreutils=8.32-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.32-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-3ubuntu1.dsc' coreutils_8.32-3ubuntu1.dsc 2011 SHA512:5ff5a18941b79093f62c4d257d8e6aa4da6cb6fbbd3659479a768fd5d500e1955f0a6d5fd72efd20b182d1d2eb50ca68d0db530f7156a8078af54878a8218dc3
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32.orig.tar.xz' coreutils_8.32.orig.tar.xz 5547836 SHA512:1c8f3584efd61b4b02e7ac5db8e103b63cfb2063432caaf1e64cb2dcc56d8c657d1133bbf10bd41468d6a1f31142e6caa81d16ae68fa3e6e84075c253613a145
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.32-3ubuntu1.debian.tar.xz' coreutils_8.32-3ubuntu1.debian.tar.xz 40716 SHA512:87a9050739a7712cb9a4b262a58393f88d979f02fef46f448eb052f1a08b35c2903c6d925d3cc8c3b72b6f8c37cff30e71136f23f7f1dd1ebc3709d116904673
```

### `dpkg` source package: `curl=7.68.0-1ubuntu4`

Binary Packages:

- `curl=7.68.0-1ubuntu4`
- `libcurl3-gnutls:amd64=7.68.0-1ubuntu4`
- `libcurl4:amd64=7.68.0-1ubuntu4`
- `libcurl4-openssl-dev:amd64=7.68.0-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.68.0-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu4.dsc' curl_7.68.0-1ubuntu4.dsc 2725 SHA512:fb4f99c4dde9ee397b72d0f6a377c425ec72b003d8c4b85c106764bed2e44f26e70d3b70c3d6c16c13c54fb75aba75ec5c318224e33b7c155a573733745a7587
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0.orig.tar.gz' curl_7.68.0.orig.tar.gz 4096350 SHA512:58b42c08b1cf4cb6e68f8e469d5b5f6298eebe286ba2677ad29e1a7eefd15b8609af54544f4c5a7dadebbd3b23bd77700830f2f60fbea7ae3f2f306e640010b0
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu4.debian.tar.xz' curl_7.68.0-1ubuntu4.debian.tar.xz 33456 SHA512:abeffd1a5a18b66a4fa320dfd461dfbebcfb9d7053bfb3e1d7fb0337920f01030551ee8b8b637dbe76b06b1d41e79af934798d79f69894ca03fc9b98579b7705
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/cyrus-sasl2/2.1.27+dfsg-2/


### `dpkg` source package: `dash=0.5.10.2-7`

Binary Packages:

- `dash=0.5.10.2-7`

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
$ apt-get source -qq --print-uris dash=0.5.10.2-7
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-7.dsc' dash_0.5.10.2-7.dsc 1762 SHA512:30a3d095d14dbe7f5fcd519f985d38d1d8ef2c901bf7395ea8da95b9434691acf3e5fef03e4f69442f3653c171e08a1df5f85a9303da4abb3e8b2693756c5ddf
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA512:0ae29be77794df0ba254967649b9728611a75fbb3acd32ab6634d76399d1ce97c7d12d31da465482a7e4f3207093415c496c39525cace9b78ab3cb9444dd7640
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-7.debian.tar.xz' dash_0.5.10.2-7.debian.tar.xz 45336 SHA512:e9bb5d70c1c954270f2a85c251b627d357d6f878e13913d939bfb3ca9b6a6f54a702863560186b3d4dea8aaa89c38fe334f4551720dc030b96cf3533ea1524b4
```

### `dpkg` source package: `db-defaults=1:5.3.21~exp1ubuntu2`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21~exp1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21~exp1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.dsc' db-defaults_5.3.21~exp1ubuntu2.dsc 2044 SHA512:f0bd0c0e9c1b19bd5eae5aeb1c8d17664db82c77428c7e4eeb4f27f8a1ec203cf55530d4ffbaa895b186eb639f89287cb9b2798d8ad9b011006a70471f7733ff
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.tar.xz' db-defaults_5.3.21~exp1ubuntu2.tar.xz 3032 SHA512:da58650b949140e8a5f85bae82af5a040c2558fd41763cef3adc8b2f0201a5f13952e4d25b428fef1d0e1cdda6b463c0cfd3402c4f6b6c2727f171bcaf956c25
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6ubuntu3`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6ubuntu3`
- `libdb5.3-dev=5.3.28+dfsg1-0.6ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu3.dsc' db5.3_5.3.28+dfsg1-0.6ubuntu3.dsc 3234 SHA512:e21d4044cf96550b5ed7a0b7ba8209f5bf9c630bfbd862783399f78963964834e0d9ab9ad42815d6fb8882ac92b57cbac0425b9b09a2606f4f673ae93692b4d8
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA512:50cb87bc3f24065839ee2932e82af032b236b290ebe89983076f503c6c62c5f36ff93d7847a3f68b2b19f35088fbab5d3ac6a34553d07e8148e68e9a3f079a12
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu3.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6ubuntu3.debian.tar.xz 30776 SHA512:0afcbf1a9899abaa38035f4c87f44060f63c9f4098e261987317457ea0ab3582f9afaa671015ba25e90be2620fa3b625b4fb9032aff3bc12aeb6004ca6a64fe6
```

### `dpkg` source package: `debconf=1.5.74`

Binary Packages:

- `debconf=1.5.74`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.74
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.dsc' debconf_1.5.74.dsc 2082 SHA512:b2ca913745ff661261cbe2e7338f7fcb6b5bbdd52aaa981950abd0714506ca9b68d15b63dfce8f2605ae7cf675ce4dd407ac822d8e4a71adea8b33a3a35975ec
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.tar.xz' debconf_1.5.74.tar.xz 571108 SHA512:421577c9fb0dae1c851c6676e7b0b3e59e5800d1ab01a9817e4506ee2f7cb812065e1a64b194b1192023951f1f0cabf0359e4dae4320b9cf0705865085cdc5cd
```

### `dpkg` source package: `debianutils=4.11.1`

Binary Packages:

- `debianutils=4.11.1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/debianutils/4.11.1/


### `dpkg` source package: `diffutils=1:3.7-3build1`

Binary Packages:

- `diffutils=1:3.7-3build1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `djvulibre=3.5.27.1-15`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.27.1-15`
- `libdjvulibre-text=3.5.27.1-15`
- `libdjvulibre21:amd64=3.5.27.1-15`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-15
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-15.dsc' djvulibre_3.5.27.1-15.dsc 2406 SHA512:e7cb957886f0fcfa6983e510bc8188e99a1a69d7ca84f45072f31ea6d0a8c4cbc243af0af4d19f531588a069f8b57277c181b4611aa71d3280bb9d159cd725e4
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA512:2ed11daa05995db7bf52113e2f75456c3c804988d2c17d0183b24ab379e52a4ef1871189e8bb132fec6cbc9d629b4d67a4d89ef7df7a995044cb25ff3dcc5de8
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-15.debian.tar.xz' djvulibre_3.5.27.1-15.debian.tar.xz 80508 SHA512:c7658ddeadb2e9c9c29c28dfa18a3928961569b971d61379d385e5b93ec3fe47ad8ddae144f6be879b3903b76042c5cc02d313062128a40fcdbdee7fb79ae78c
```

### `dpkg` source package: `dpkg=1.20.5ubuntu2`

Binary Packages:

- `dpkg=1.20.5ubuntu2`
- `dpkg-dev=1.20.5ubuntu2`
- `libdpkg-perl=1.20.5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.20.5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.20.5ubuntu2.dsc' dpkg_1.20.5ubuntu2.dsc 2272 SHA512:c79493ec2016b56b97e2842060f7f9d5e290f43e043ede7c8fc2f2fe672df4a243cae62567f1f7546d385b84c262e0e65d59dc6cfa4074fa6febd136bbd9509d
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.20.5ubuntu2.tar.xz' dpkg_1.20.5ubuntu2.tar.xz 4743632 SHA512:bea83e4ed1ee877b38384e0a4ab3e56bc0d7fe502b7a93537e424a9f751ff678900da284c9612f1476341bdcb43aa95caeaafbb183abdfdbd90aa1e0e738bc94
```

### `dpkg` source package: `dulwich=0.19.15-1build1`

Binary Packages:

- `python3-dulwich=0.19.15-1build1`

Licenses: (parsed from: `/usr/share/doc/python3-dulwich/copyright`)

- `Apache-2`
- `Apache-2.0`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris dulwich=0.19.15-1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15-1build1.dsc' dulwich_0.19.15-1build1.dsc 2410 SHA512:10ce690c478276ea50a2f0b280df36eb2a2fdcf0f2e540e6eafa44684bbab22b20a7971345f3198860c6fe4739b409c93cc65e5220c8ebc1c46de1ad893bbb2c
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15.orig.tar.gz' dulwich_0.19.15.orig.tar.gz 369491 SHA512:ae56cf4748ea5f9d275f2d1456bf9fce77859ad2eeba6b7d8f34283e212404ba385f377f4fb86b88dc40982649ec8cfb12ea407dd25ada7cb2b0e862568ac7da
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15-1build1.debian.tar.xz' dulwich_0.19.15-1build1.debian.tar.xz 631088 SHA512:4e0a64605129195a37fa883956a5e8f2208d97eb1a358af4d367d1ea345ac67325cd350bc35665042586044749879c7ca1792676832456a1667a9a294a41b14a
```

### `dpkg` source package: `e2fsprogs=1.45.6-1ubuntu1`

Binary Packages:

- `comerr-dev:amd64=2.1-1.45.6-1ubuntu1`
- `e2fsprogs=1.45.6-1ubuntu1`
- `libcom-err2:amd64=1.45.6-1ubuntu1`
- `libext2fs2:amd64=1.45.6-1ubuntu1`
- `libss2:amd64=1.45.6-1ubuntu1`
- `logsave=1.45.6-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.6-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.dsc' e2fsprogs_1.45.6-1ubuntu1.dsc 3328 SHA512:3c1fc4edd9823e43796442423ea114a9e1f5dcc07559b0c9ee1cdb417d8e043aabdfd7272a21dc2669a8b4886244c73b4248289b3d239205296a62c3d91cc46b
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz' e2fsprogs_1.45.6.orig.tar.gz 7938544 SHA512:432483cb0e32f96169014ca7ef4e053e5d64c6b934ea6f48a86cfd9e01187802ea6a5b13db62e14f4fa3745254c3587a115d560059c1d4995a41273f14f91f8c
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz.asc' e2fsprogs_1.45.6.orig.tar.gz.asc 488 SHA512:afdfebae62948899125802515a01302edd4d9ce8519c83714af133d33f17a9ce2aebbf686ee5f850a2d34a700f362df5c52ac4ea6a49fb71b6fb207a29ed7602
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz' e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz 81276 SHA512:86002f00c0a4968ca15083a98c14c5791d177451b7f1e6270d63698ba1a3a2cfa6547560afe6b60eafe6f52c1908e40488848d8568db263d5a596f3b3e00378f
```

### `dpkg` source package: `elfutils=0.181-1`

Binary Packages:

- `libelf1:amd64=0.181-1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.181-1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.181-1.dsc' elfutils_0.181-1.dsc 2810 SHA512:96af3ab710035fc9d4c16e822c6ea886742b880144fbf5fe5a704dafaf1b170e7a6354d550afa202639253528ded3f0dc89a404763764ee1438eaf499752c421
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.181.orig.tar.bz2' elfutils_0.181.orig.tar.bz2 9088984 SHA512:d565541d5817f409dc89ebb1ee593366f69c371a1531308eeb67ff934b14a0fab0c9009fd7c23240efbaa1b4e04edac5c425e47d80e3e66ba03dcaf000afea36
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.181-1.debian.tar.xz' elfutils_0.181-1.debian.tar.xz 32432 SHA512:86629a3dc83ec0c3f06f343dbd5e100975be30ab7919aefe4e51d10f258c333e080f3cbb263877b0c0ec7a42e8666bcc36be2abaa64c1b5bd48d6871b2b76310
```

### `dpkg` source package: `expat=2.2.9-1build1`

Binary Packages:

- `libexpat1:amd64=2.2.9-1build1`
- `libexpat1-dev:amd64=2.2.9-1build1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.9-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.dsc' expat_2.2.9-1build1.dsc 1998 SHA512:fdca34746c71607dad289fef256b9c4f6c4a7324154ee048c837147b28d9bedd9eb272dca34ff441c2ac631d30387224404ef69291c0e833ed466d12feb6dcc0
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9.orig.tar.gz' expat_2.2.9.orig.tar.gz 8273174 SHA512:e274fa7f30630450cb3ca681b266d765dbb7f5d00d1275ff9d9b2e2f6e1095893b8af4e3f4172ae6297c7a8a831a0a6becd484fe4bcdca09c37922f630780ef0
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.debian.tar.xz' expat_2.2.9-1build1.debian.tar.xz 10780 SHA512:3d92479e76334d974bc3ba9b879579d6e3380bf5365fda64f8ed19a3d76a6c294526795c49a60743575e9c92e33e184d642c635b0a4d70f56dbcc8ee9488a0e6
```

### `dpkg` source package: `fftw3=3.3.8-2ubuntu6`

Binary Packages:

- `libfftw3-double3:amd64=3.3.8-2ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.8-2ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu6.dsc' fftw3_3.3.8-2ubuntu6.dsc 3010 SHA512:e67e452520bfed6cc0f75e2b4ef49500258536f6ba97417a012c32d5fc4e0b881d7b264e39705d177126261d2e2b6775616726b966b089ed3147aa87c6e1525c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8.orig.tar.gz' fftw3_3.3.8.orig.tar.gz 4110137 SHA512:ab918b742a7c7dcb56390a0a0014f517a6dff9a2e4b4591060deeb2c652bf3c6868aa74559a422a276b853289b4b701bdcbd3d4d8c08943acf29167a7be81a38
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.8-2ubuntu6.debian.tar.xz' fftw3_3.3.8-2ubuntu6.debian.tar.xz 14208 SHA512:fcb2c5a3e073ad60121c0847ba99584f4bcde05dc3f98f0caf13814b9c0840d68b41b94c8003c312fe3a931dd85dd39667902133e97403fa394d6de63349240c
```

### `dpkg` source package: `file=1:5.38-5`

Binary Packages:

- `file=1:5.38-5`
- `libmagic-mgc=1:5.38-5`
- `libmagic1:amd64=1:5.38-5`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.38-5
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38-5.dsc' file_5.38-5.dsc 2237 SHA512:a3a46f2bce95410b4720f9886917ab1e9c3041afe9401d1d0dc18eeb838d2a78db4c62eafe3d06ceab65fc6fb06bc2c2058d17cb9904d467c863a1cd997e0ff7
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38.orig.tar.gz' file_5.38.orig.tar.gz 932528 SHA512:9eeeba69cbc9f0c00a0bdf9eaf60c73a4a709e797068f109d85c1ef2a19c8b0e012ecd73714f03cbb1770dfa717e8a661ad746b644cc030cafbfb1f7aac35a40
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38.orig.tar.gz.asc' file_5.38.orig.tar.gz.asc 169 SHA512:2574d4ff1f5f666b1d058f82d7b14f5069830479f889be25af4a23d5295b2b6900f794743595e475ef7e66730701a70f69de321824671226bc135bfd3a3ecd01
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.38-5.debian.tar.xz' file_5.38-5.debian.tar.xz 35120 SHA512:ebaa4921548a7a972410f0f518f21ee62ddbee5b415858cf56388f1c3c18c19226c33c283450cab2a1d6f9f832ba4757bb6a818616864aae39dec2e1131803b0
```

### `dpkg` source package: `findutils=4.7.0-1ubuntu1`

Binary Packages:

- `findutils=4.7.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `fontconfig=2.13.1-2ubuntu3`

Binary Packages:

- `fontconfig=2.13.1-2ubuntu3`
- `fontconfig-config=2.13.1-2ubuntu3`
- `libfontconfig1:amd64=2.13.1-2ubuntu3`
- `libfontconfig1-dev:amd64=2.13.1-2ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.13.1-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-2ubuntu3.dsc' fontconfig_2.13.1-2ubuntu3.dsc 1959 SHA512:cef815ec239627e55baa676923928f1f4c17098cd6c761581b255f8ca5c63a2256e04008fa02a4de7fa16c566e42ea43e98b6a1aab89b8978331bec2d37f708b
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1.orig.tar.bz2' fontconfig_2.13.1.orig.tar.bz2 1723639 SHA512:f97f2a9db294fd72d416a7d76dd7db5934ade2cf76903764b09e7decc33e0e2eed1a1d35c5f1c7fd9ea39e2c7653b9e65365f0c6205e047e95e38ba5000dd100
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.13.1-2ubuntu3.debian.tar.xz' fontconfig_2.13.1-2ubuntu3.debian.tar.xz 26344 SHA512:6e6b7bdd54e2e74f9247c4d768e49b48eb5fe2fc524e269911e9a226d27b6f54e49dba7196e478a9ace65caceb120dd4ed654a61bdc023ceb0efa4b683b373e8
```

### `dpkg` source package: `fonts-dejavu=2.37-2`

Binary Packages:

- `fonts-dejavu-core=2.37-2`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.dsc' fonts-dejavu_2.37-2.dsc 2387 SHA512:3a5dffb19a3de3788d1c94b01490d60f1a112bfa18b8b804ec36882ad17bd2fa331e36b8e2d97c0cd4074c0d18a2a5805085013a5e97d64e507e085256c8eb40
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA512:e61fc8c675ef76edb49dd9a8caee62087280929bb8144b52aca2f8def30025c56246589ad8a6a806b9574e6876eedd16d57c70a6ce9c86817a2dfe39d8a2bb2b
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-2.debian.tar.xz' fonts-dejavu_2.37-2.debian.tar.xz 11408 SHA512:cc7a355819e5a06c4e802066dec8cdee50512c6d8991d65a3cbcd67a25a081cd212f8722e26aff2e24209fac51c60070448d849fed9a8ca6d52dd1e7240cfcba
```

### `dpkg` source package: `freetype=2.10.2+dfsg-3`

Binary Packages:

- `libfreetype-dev:amd64=2.10.2+dfsg-3`
- `libfreetype6:amd64=2.10.2+dfsg-3`
- `libfreetype6-dev:amd64=2.10.2+dfsg-3`

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
$ apt-get source -qq --print-uris freetype=2.10.2+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg-3.dsc' freetype_2.10.2+dfsg-3.dsc 3680 SHA512:bf8fbeff762f03dcd9214906c3302e75ab4fb9dd43f0143d94b7434a352b8fc09d5b83d1068fc85346469ee014ed000e51add246ad99727bd65ba3b2722cd337
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2demos.tar.xz' freetype_2.10.2+dfsg.orig-ft2demos.tar.xz 230672 SHA512:912e3c3cbcdfd30fd918897d28240e04eb7248d130fc519e7d1613873a11d275d658ff247c6d517ebecf7a09de0d05f3dc10631411226015e1b147cba9a8a438
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2demos.tar.xz.asc' freetype_2.10.2+dfsg.orig-ft2demos.tar.xz.asc 195 SHA512:59945ed85bfb347f8a30967d233b798d5e4d72f2a24758768855066ecfaa3cc8e5d3eb04c27841274aff141636529a73919ebb939562902dc4a66329d9658f8b
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2docs.tar.xz' freetype_2.10.2+dfsg.orig-ft2docs.tar.xz 2078712 SHA512:c54956a56920e651102b75c0efa07212e1d95f3bec219b8364b61d9a71171b11da492170cc861c36f3305f32ad1dee46d0d5a561ccdc6ca36591ae3f619a1d67
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig-ft2docs.tar.xz.asc' freetype_2.10.2+dfsg.orig-ft2docs.tar.xz.asc 195 SHA512:c0b92d323e3eb8dd6d48a528756ffc363ee3ed14d634daddd4bb161752bc093cc6f80cc277d3a585c0f3897d9fc5945615ed9433d726dd174653bfee9e3c5aa8
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg.orig.tar.xz' freetype_2.10.2+dfsg.orig.tar.xz 2246904 SHA512:501457e931a513be57049b430baff251176af4a1fabd85adca12372be60c9b5595f68226e0d8c4b8c5543dd137ddc7fb83858432a2e38c662b870d27b340b6fb
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.10.2+dfsg-3.debian.tar.xz' freetype_2.10.2+dfsg-3.debian.tar.xz 116212 SHA512:83afe1e8f5bab4f730dbc1af6a3966d858acc54fb1110d4ae0996ff1552da619adb79ef18240756ebadb1396162b7aec207b14830ef498928471de895967ef02
```

### `dpkg` source package: `fribidi=1.0.8-2`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.dsc' fribidi_1.0.8-2.dsc 1987 SHA512:f2f799a6b3704c158482caf08719ef62ca646b03f21b08405e65a9ffc8619335112198aa0a5108632fb7490243f740657d9d0659e52d4c1cebc8300add54e963
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA512:d66b1524b26d227fd6a628f438efb875c023ae3be708acaaad11f1f62d0902de0a5f57124458291ef2b0fcd89356c52ab8ae5559b0b5a93fa435b92f1d098ba2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_1.0.8-2.debian.tar.xz' fribidi_1.0.8-2.debian.tar.xz 8980 SHA512:04d10d26c3ccf3a0e2782a780fcbe64f1ab47c85633ffeefb1a9251e29ff20a046509afcb30b32a2ec52a52780d5054aad2ec07517b7b667fb06ab99125f9ea3
```

### `dpkg` source package: `gcc-10=10.2.0-9ubuntu2`

Binary Packages:

- `cpp-10=10.2.0-9ubuntu2`
- `g++-10=10.2.0-9ubuntu2`
- `gcc-10=10.2.0-9ubuntu2`
- `gcc-10-base:amd64=10.2.0-9ubuntu2`
- `libasan6:amd64=10.2.0-9ubuntu2`
- `libatomic1:amd64=10.2.0-9ubuntu2`
- `libcc1-0:amd64=10.2.0-9ubuntu2`
- `libgcc-10-dev:amd64=10.2.0-9ubuntu2`
- `libgcc-s1:amd64=10.2.0-9ubuntu2`
- `libgomp1:amd64=10.2.0-9ubuntu2`
- `libitm1:amd64=10.2.0-9ubuntu2`
- `liblsan0:amd64=10.2.0-9ubuntu2`
- `libquadmath0:amd64=10.2.0-9ubuntu2`
- `libstdc++-10-dev:amd64=10.2.0-9ubuntu2`
- `libstdc++6:amd64=10.2.0-9ubuntu2`
- `libtsan0:amd64=10.2.0-9ubuntu2`
- `libubsan1:amd64=10.2.0-9ubuntu2`

Licenses: (parsed from: `/usr/share/doc/cpp-10/copyright`, `/usr/share/doc/g++-10/copyright`, `/usr/share/doc/gcc-10/copyright`, `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libasan6/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-10-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-10-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `gcc-defaults=1.189ubuntu1`

Binary Packages:

- `cpp=4:10.2.0-1ubuntu1`
- `g++=4:10.2.0-1ubuntu1`
- `gcc=4:10.2.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.189ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.189ubuntu1.dsc' gcc-defaults_1.189ubuntu1.dsc 16534 SHA512:fa7d4341b4d79d3ec6c943ebf883f18f839389439f7aaa6abece5c11723b4d21396ffc67d88ef8e91bbeeac58c5b7549fc3c0506a74f4474fe4157b37b2daa51
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.189ubuntu1.tar.xz' gcc-defaults_1.189ubuntu1.tar.xz 48464 SHA512:da292a787accdf1bc0f17eb378c1e2efe8a533f3fdd8cac56863638c0b4b93af829e980721c90fdaa8c0e3fb8d4af579c4b5629c984ae87e0f456bc0b1230312
```

### `dpkg` source package: `gdbm=1.18.1-5.1`

Binary Packages:

- `libgdbm-compat4:amd64=1.18.1-5.1`
- `libgdbm-dev:amd64=1.18.1-5.1`
- `libgdbm6:amd64=1.18.1-5.1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.18.1-5.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.1.dsc' gdbm_1.18.1-5.1.dsc 2618 SHA512:d842511e1a9e0150af43dd7c64c8b4419e53a500cf68ee37aa24771430bc9a165d7c0f41167634c8fecc29af3652ae2290ee7577d3bd98e703a6f38a4b71eb80
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz' gdbm_1.18.1.orig.tar.gz 941863 SHA512:adf9d6c5bc843ff0d7f88c2a1667d509973b2d63378d0001d7e74cc10aee6ea498a4513cc88ddf78c32ba4db5cb040b2794f4f1b3338c65d9894058850e2f5ef
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz.asc' gdbm_1.18.1.orig.tar.gz.asc 412 SHA512:ea614b78c7a15b59dd13ea62f99f298075ca3f43d8d9ea2079e0b3ef25cf104062c595893df7675471e7317fbf496119616a4376bae345852b9f5fc31b181705
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.1.debian.tar.xz' gdbm_1.18.1-5.1.debian.tar.xz 16812 SHA512:a8e5e70b5962ae6b662d868d8ab2d489a8a187a1f0ab2f46947bc38c2b5cfc1152449359666871ec19bd07a46536a4f49197396a553662de22aa049f4e71d293
```

### `dpkg` source package: `gdk-pixbuf=2.40.0+dfsg-5`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-0:amd64=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-bin=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-common=2.40.0+dfsg-5`
- `libgdk-pixbuf2.0-dev:amd64=2.40.0+dfsg-5`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-bin/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.40.0+dfsg-5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-5.dsc' gdk-pixbuf_2.40.0+dfsg-5.dsc 3069 SHA512:6c0ca789f12fd66d4c00b005798c8794cb03bf862dc626e5adda5df228dab7870b867672bd528b48279a8968d0618becb2aa4f8dae8c1e7884ead172cc4a5de2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg.orig.tar.xz' gdk-pixbuf_2.40.0+dfsg.orig.tar.xz 5626144 SHA512:bb8a9d1837bffdc5f50307dba1a1e6f1ac015e6e670ea6cae6d0bc997afa106ff0d928cb847d76848c480a06e1ad3945274b4913eaa4d9a8074797fc82bb7c1f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.40.0+dfsg-5.debian.tar.xz' gdk-pixbuf_2.40.0+dfsg-5.debian.tar.xz 17932 SHA512:65295cf3a975f0515e07fb366f29071eb05d84a285b7d3ec75155da8fbc8cfb2be389b888d1c5d8766bf57c576bef2b239d4561987520faa687f309cb3762168
```

### `dpkg` source package: `git=1:2.27.0-1ubuntu1`

Binary Packages:

- `git=1:2.27.0-1ubuntu1`
- `git-man=1:2.27.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/git/copyright`, `/usr/share/doc/git-man/copyright`)

- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-2-clause`
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
$ apt-get source -qq --print-uris git=1:2.27.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0-1ubuntu1.dsc' git_2.27.0-1ubuntu1.dsc 2991 SHA512:37156a5667907c88dd713cdf3efd463c74fd96f5a6bf67f3cf102e91f969f9cd682ba51bf610382d28b10af4612d65f34cd78cb4a3b9256ac422eec1b71ea140
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0.orig.tar.xz' git_2.27.0.orig.tar.xz 6074636 SHA512:8ddea44503db7caf1f6080e64555541aa64a7b8761fd6541965ee244d9c4a47befccda1a239f11d86c2ad0ff24923d084f65712f5f2d6cfa178573e3471c6c33
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0-1ubuntu1.debian.tar.xz' git_2.27.0-1ubuntu1.debian.tar.xz 652712 SHA512:392bbd0494e86a2e3a06e57e6ad18d160f7540f0f965882190db43691c58153e01be9090ad44cb54e2a4a6a96e63e21eaa38b26424cb3e9b910a774b8679f7eb
```

### `dpkg` source package: `glib2.0=2.66.0-2`

Binary Packages:

- `libglib2.0-0:amd64=2.66.0-2`
- `libglib2.0-bin=2.66.0-2`
- `libglib2.0-data=2.66.0-2`
- `libglib2.0-dev:amd64=2.66.0-2`
- `libglib2.0-dev-bin=2.66.0-2`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.66.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.66.0-2.dsc' glib2.0_2.66.0-2.dsc 3346 SHA512:574c40762941121d510cf6e4c304a94eee3a52d24c7c2c318c2a915015f3477989cab9291e06641ad6d80280c56635893e837cb7886d1117410f03679a493c3e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.66.0.orig.tar.xz' glib2.0_2.66.0.orig.tar.xz 4839236 SHA512:358e6a840b722139593eb7825c3aa70153eb26036e05d13d3286bcc6d2e962c2b4ddcb0fe5c6728b89bfffbd178101e72c576081ae714326a272a9fc34ed953e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.66.0-2.debian.tar.xz' glib2.0_2.66.0-2.debian.tar.xz 94844 SHA512:e24c2e96d0bb9cfb65b4f59ea585487ad331d826b1e580d44768719be0d6aa463e074218ca2b51a388deea9e4ea59f9dd703a7233ce901982fbfef349d9a84a1
```

### `dpkg` source package: `glibc=2.32-0ubuntu3`

Binary Packages:

- `libc-bin=2.32-0ubuntu3`
- `libc-dev-bin=2.32-0ubuntu3`
- `libc6:amd64=2.32-0ubuntu3`
- `libc6-dev:amd64=2.32-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.32-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.32-0ubuntu3.dsc' glibc_2.32-0ubuntu3.dsc 8912 SHA512:d481acb21fb9c456380186d2683452602ca8e5026ba2b1c6a62303cb8995fa1e61ae838531632ba05d344c2e933491b02360e1ec51dd4352ad6ef90732715b5b
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.32.orig.tar.xz' glibc_2.32.orig.tar.xz 16744512 SHA512:8460c155b7003e04f18dabece4ed9ad77445fa2288a7dc08e80a8fc4c418828af29e0649951bd71a54ea2ad2d4da7570aafd9bdfe4a37e9951b772b442afe50b
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.32-0ubuntu3.debian.tar.xz' glibc_2.32-0ubuntu3.debian.tar.xz 859372 SHA512:81b4d873df87a3b6199d146aa981e6235ec416058df8e02b38e5fed2776ba1adbb0281da80a96c09a4946fad11156a89a91b8502470b43b85335058ab9f3587c
```

### `dpkg` source package: `gmp=2:6.2.0+dfsg-6ubuntu1`

Binary Packages:

- `libgmp-dev:amd64=2:6.2.0+dfsg-6ubuntu1`
- `libgmp10:amd64=2:6.2.0+dfsg-6ubuntu1`
- `libgmpxx4ldbl:amd64=2:6.2.0+dfsg-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.0+dfsg-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6ubuntu1.dsc' gmp_6.2.0+dfsg-6ubuntu1.dsc 2230 SHA512:3c81d30c5ffde286ca315db3226e22887d4828b3534355fd8900d855d650679a58732de176c7569b98cf59b65b77644e09e06b9909289a07bb8d1330b6e8db9a
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg.orig.tar.xz' gmp_6.2.0+dfsg.orig.tar.xz 1842912 SHA512:6ed6df69ced53b13e3e2d64d94f8a34c3257abd4c0967f16d48b064956e260a3d8fb424c84d47dca6d1308bd16b347af3740fce68ebd2d45f1d7f752422c2496
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6ubuntu1.debian.tar.xz' gmp_6.2.0+dfsg-6ubuntu1.debian.tar.xz 54484 SHA512:0c1e932f495d69f886d4b2118ee4eb10587a0164a36c0c0f4c5302ec3aa9960ad9c1a68afab6ef220c2a4bfaa1dea7522410a224b69c253ce497ac6d6198475a
```

### `dpkg` source package: `gnupg2=2.2.20-1ubuntu1`

Binary Packages:

- `dirmngr=2.2.20-1ubuntu1`
- `gnupg=2.2.20-1ubuntu1`
- `gnupg-l10n=2.2.20-1ubuntu1`
- `gnupg-utils=2.2.20-1ubuntu1`
- `gpg=2.2.20-1ubuntu1`
- `gpg-agent=2.2.20-1ubuntu1`
- `gpg-wks-client=2.2.20-1ubuntu1`
- `gpg-wks-server=2.2.20-1ubuntu1`
- `gpgconf=2.2.20-1ubuntu1`
- `gpgsm=2.2.20-1ubuntu1`
- `gpgv=2.2.20-1ubuntu1`

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
$ apt-get source -qq --print-uris gnupg2=2.2.20-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu1.dsc' gnupg2_2.2.20-1ubuntu1.dsc 3971 SHA512:dae355ed676febcae7d2db47e4ae41e635a78cbe3977ea8a98ce79f38664d20677027b86049b005fc1718d1f67a93470ab1a68997ef84d6bb7cdd477702db731
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2' gnupg2_2.2.20.orig.tar.bz2 6786913 SHA512:3e69f102366ec3415f439ab81aae2458182fa1a18dfb86565b1d9dc638f3fc4c179a5947f0042b7c5a813345676285a662793664a1803ea9ad8328f0548e0edc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2.asc' gnupg2_2.2.20.orig.tar.bz2.asc 1357 SHA512:0972788af253f84959ab3142e3d4bf025b7e7077377574e69851ae3d37cbf296211fdf50cd77fe47f844bc3383489ff88cf35186d2f72cb0adc84cdfe77bfd26
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu1.debian.tar.xz' gnupg2_2.2.20-1ubuntu1.debian.tar.xz 64332 SHA512:a4d158b8f7399c31473990cc147698bbd4513de459315b26e6df66e45e9d9291c5ce46322c006a698b90be2ce789b08b3ea03a19ec89266a721118e6819941b9
```

### `dpkg` source package: `gnutls28=3.6.13-4ubuntu5`

Binary Packages:

- `libgnutls30:amd64=3.6.13-4ubuntu5`

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


### `dpkg` source package: `gobject-introspection=1.64.1-1build2`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.64.1-1build2`
- `gir1.2-glib-2.0:amd64=1.64.1-1build2`
- `libgirepository-1.0-1:amd64=1.64.1-1build2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `grep=3.4-1`

Binary Packages:

- `grep=3.4-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.dsc' grep_3.4-1.dsc 1674 SHA512:8ff51683a7155442e3d985b1ba1495bae1c8b2ca357ca010ef533969fd9b105e08ff9a26a691a269473219d004b0c468824190e617f15fa96100c7770ac1aa81
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz' grep_3.4.orig.tar.xz 1555820 SHA512:0f1506bd19971fbdcb47a111277ca63e8ad045456f096980852fd0a61c860f29f4b369bbaaa5cbce4b0a81718e3e3274d9a078b491f2109baa9a02ce600ee206
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz.asc' grep_3.4.orig.tar.xz.asc 833 SHA512:720e9b27af30104746a0cfb9141892944d9ec567f203a2d5a59230296b545ce0634382fd4fbde418d96d8f772440db14d499f841dfa23bb986c246ba68c2ccf7
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.debian.tar.xz' grep_3.4-1.debian.tar.xz 104364 SHA512:4939721cfc9cbec0c6c3fb5cb123da3c2d4040e6fa46e84fe4bc26adbca1bd357f92864ef13c367e90ae6e3875cfe4aee1388fe52e293bd409653350aed4a9a6
```

### `dpkg` source package: `gzip=1.10-2ubuntu1`

Binary Packages:

- `gzip=1.10-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-2ubuntu1.dsc' gzip_1.10-2ubuntu1.dsc 2074 SHA512:e116e7438cf5e77837f867ff60f7211703cc02409a12aa2db8d16842ba76f0b75961ede88abb5ab457ed2b7113e8717c104f94c66c059280654a16823c50fa07
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA512:7939043e74554ced0c1c05d354ab4eb36cd6dce89ad79d02ccdc5ed6b7ee390759689b2d47c07227b9b44a62851afe7c76c4cae9f92527d999f3f1b4df1cccff
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-2ubuntu1.debian.tar.xz' gzip_1.10-2ubuntu1.debian.tar.xz 33288 SHA512:39d000ae7356a28275b475e08e296b07d9efc589fa7379aaab4e70fc599378ba56e8f492ebb26ba618b7dc09bd8eb56b2babe5c5d826db852fdd5cf496cd318a
```

### `dpkg` source package: `harfbuzz=2.6.4-1ubuntu5`

Binary Packages:

- `libharfbuzz0b:amd64=2.6.4-1ubuntu5`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=2.6.4-1ubuntu5
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4-1ubuntu5.dsc' harfbuzz_2.6.4-1ubuntu5.dsc 2841 SHA512:27673ff23656a35f16943a38aaa8a6bcdcc494920dc20ae6c4b5c15ecffe38eaf3a2eb9ff358a897dfb3446c25cfd54dc840fcc30735b5a6a2f605d3f714c572
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4.orig.tar.xz' harfbuzz_2.6.4.orig.tar.xz 5967468 SHA512:d8664bb64fda11ff7646693070637e3827f8b3d1de50e11ecf108ce4d19c878b26b2ba4cff278da6e6cc0cb431e1630d9eaa7c32a9bebb9655a7aa8dabf7114f
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_2.6.4-1ubuntu5.debian.tar.xz' harfbuzz_2.6.4-1ubuntu5.debian.tar.xz 11388 SHA512:42d4417ac2d4e84c7e4a8583bbd5f38e5cea485068c7792583de511edc601f78b073635befec0e6b24956ad43610d81758787a30fa54cd7612477b7baa30c07f
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

### `dpkg` source package: `icu=67.1-4`

Binary Packages:

- `icu-devtools=67.1-4`
- `libicu-dev:amd64=67.1-4`
- `libicu67:amd64=67.1-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=67.1-4
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1-4.dsc' icu_67.1-4.dsc 2219 SHA512:f9b19b2fb67fe6957fb9ee494b5095fd68c944edef42f1e05e12fc975ba62ab69ee0a2d9fa868bdba1161c175f4c6cc2d82e67ef7403d4af43dda58f02f3607b
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1.orig.tar.gz' icu_67.1.orig.tar.gz 24518055 SHA512:4779f1ce1ca7976f6fad6768853ea8c540da54d11509e3b6cfd864a04b5f2db1c3d4b546387f91ad02fb90804525bc37d2543173f0d705d6ca11dc6f2b7640a8
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1.orig.tar.gz.asc' icu_67.1.orig.tar.gz.asc 833 SHA512:3d731cfbb200f150f6fda348a100226ad7a56dea428a46745bcaf5be3ad6a0bf3ef685acfdf759f51a53704d78b4a02ee90ecbf50f2e18d14fcef5050afd8f54
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_67.1-4.debian.tar.xz' icu_67.1-4.debian.tar.xz 29480 SHA512:0b95795c7230c58fa6d0bfc13cb07431375026467d3845004aebb374c0fe5be38aacdd9ecbc2d769afb37924c1eb607a9bcd5f821dfe028b06e4cd6c3802bad7
```

### `dpkg` source package: `ilmbase=2.5.3-2`

Binary Packages:

- `libilmbase-dev:amd64=2.5.3-2`
- `libilmbase25:amd64=2.5.3-2`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase25/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.5.3-2
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.3-2.dsc' ilmbase_2.5.3-2.dsc 2468 SHA512:dbff4d72c16ee73a954c71e87c8df7bcf3bf4965d760855784539cdd7766b7e625845ae7add575b42d971b24e2c0546550d8fa64584b051c50e57b3ca6ea8af0
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.3.orig.tar.gz' ilmbase_2.5.3.orig.tar.gz 27534825 SHA512:6da03193d4fea1e97e35008f59304ab408c521ead8495ba411cde5c172cf953be97999971f57398b813d14f1af1d722539a6b74d5ee54b9e74769ea8258d36ba
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.3.orig.tar.gz.asc' ilmbase_2.5.3.orig.tar.gz.asc 287 SHA512:9b3978e44b531429aba42b9cc4969a470898d9d74652e3809edb0273ba9b127c471aec6570b5d352be738f59810091c0df2c70d39c16d2c32833d173b270f72c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/ilmbase/ilmbase_2.5.3-2.debian.tar.xz' ilmbase_2.5.3-2.debian.tar.xz 14304 SHA512:ca489be262593e20012362ee4fd82cf74f79507ce75d530518d1133cd15c0fa515e3964f12c098259e214bf3f3e4f1eccf3fbd15362bdd2f91aedb83a4341310
```

### `dpkg` source package: `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu12`

Binary Packages:

- `imagemagick=8:6.9.10.23+dfsg-2.1ubuntu12`
- `imagemagick-6-common=8:6.9.10.23+dfsg-2.1ubuntu12`
- `imagemagick-6.q16=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6-arch-config:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6-headers=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6.q16-6-extra:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickcore-dev=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-6-headers=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-6.q16-6:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-6.q16-dev:amd64=8:6.9.10.23+dfsg-2.1ubuntu12`
- `libmagickwand-dev=8:6.9.10.23+dfsg-2.1ubuntu12`

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


### `dpkg` source package: `init-system-helpers=1.58`

Binary Packages:

- `init-system-helpers=1.58`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.58
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.58.dsc' init-system-helpers_1.58.dsc 1896 SHA512:eae4ad120fd7d0e289d70a2092fcc1614f92144022702094a794cb96523325eea572027f1cd5bc9413a1c423db03c91f9eee3b820a9f8c616adc96622082b932
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.58.tar.xz' init-system-helpers_1.58.tar.xz 40668 SHA512:bab1b9f186a5183fc98d9230765b81136a5c861d5c83c93296d99072beb59cdbaa241d4b4e5631e8a2bd6ba61390c21a86ccba4587aeaa9a6b7929146f0ccded
```

### `dpkg` source package: `isl=0.22.1-1`

Binary Packages:

- `libisl22:amd64=0.22.1-1`

Licenses: (parsed from: `/usr/share/doc/libisl22/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.22.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1-1.dsc' isl_0.22.1-1.dsc 1860 SHA512:771b74db4ad154cab26ed03fe289186cb0e206da3ecd94b3959b0055598f26cf3a9cbd93a5064709cd81928b7005c7ee2067f011f70e92ed3660ee09f4e92f28
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1.orig.tar.xz' isl_0.22.1.orig.tar.xz 1676948 SHA512:8dc7b0c14e5bfdca8f2161be51d3c9afcd18bc217bb19b7de01dbba0c6f3fdc2b725fb999f8562c77bf2918d3005c9247f7a58474a6da7697390067944d4d4aa
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1-1.debian.tar.xz' isl_0.22.1-1.debian.tar.xz 25252 SHA512:89d5f46f4ce5f73d9d842106f4ee6ca35286d01abaa1cc656efce8ec9de1180634c8d6a1d2cd81402506507d49d3505921799328fb34be7c16148ee5a0936455
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

### `dpkg` source package: `krb5=1.17-10`

Binary Packages:

- `krb5-multidev:amd64=1.17-10`
- `libgssapi-krb5-2:amd64=1.17-10`
- `libgssrpc4:amd64=1.17-10`
- `libk5crypto3:amd64=1.17-10`
- `libkadm5clnt-mit11:amd64=1.17-10`
- `libkadm5srv-mit11:amd64=1.17-10`
- `libkdb5-9:amd64=1.17-10`
- `libkrb5-3:amd64=1.17-10`
- `libkrb5-dev:amd64=1.17-10`
- `libkrb5support0:amd64=1.17-10`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit11/copyright`, `/usr/share/doc/libkadm5srv-mit11/copyright`, `/usr/share/doc/libkdb5-9/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-10
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-10.dsc' krb5_1.17-10.dsc 3187 SHA512:45e81c598fd41bcd246786bf69bf26ecc335c968c1586cf2de58970c80a053cffbdb41c21263f95969749b4091e97fc9495d46ddbf9584868cca63380d628073
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA512:7462a578b936bd17f155a362dbb5d388e157a80a096549028be6c55400b11361c7f8a28e424fd5674801873651df4e694d536cae66728b7ae5e840e532358c52
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-10.debian.tar.xz' krb5_1.17-10.debian.tar.xz 143852 SHA512:79f7b8f7ca4fb481c1b4f8b229c411e5400c9add8b95c3d22f162f5d1a22f1a947f1d16eda6cdf9e897c129ffca7af35d9553335d9081e7ffa5dd573d040615d
```

### `dpkg` source package: `lcms2=2.9-4`

Binary Packages:

- `liblcms2-2:amd64=2.9-4`
- `liblcms2-dev:amd64=2.9-4`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.9-4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-4.dsc' lcms2_2.9-4.dsc 1956 SHA512:c0ebd8cf4512fb1195ba17cba3cd28773ebef7952b8682dda4285ed98f8bf62321716e2fd345d8a0f2de206ffb3dc858b223c0301222a0ccebf08fd5fafaefa5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9.orig.tar.gz' lcms2_2.9.orig.tar.gz 10974649 SHA512:70b1c51fa8d137d5072425e580745ff1fbf49c6e8bb1da0a8adb0647d3b7c095208793cb02de1e8d1a01363b8575fa60c61bedbff99bbec57a44228239cb00e5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-4.debian.tar.xz' lcms2_2.9-4.debian.tar.xz 10748 SHA512:0f3527accbf235dc642b3b3f082414c7e5ccce043d94b07fe323ec8aa9982e658ade3a35503931d777a43abecad9c055ece193772af6094145c7ac3194cda338
```

### `dpkg` source package: `libassuan=2.5.3-7.1`

Binary Packages:

- `libassuan0:amd64=2.5.3-7.1`

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
$ apt-get source -qq --print-uris libassuan=2.5.3-7.1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.dsc' libassuan_2.5.3-7.1.dsc 2627 SHA512:c6d456a6aa7c4588117c84f17b9e97bb84707fe043b97dd5bb0739b35cfce7aae8713db9753fb07c028cc8581056ae8b8599ae652c13ef96c715413fffb5b885
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA512:e7ccb651ea75b07b2e687d48d86d0ab83cba8e2af7f30da2aec794808e13e6ec93f21d607db50d3431f1c23cb3a07a2793b71170e69fa2f5a82cffb81961f617
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA512:df57f8e575164b0e030d88c57bafe83249add41a551597a7527680cfa351244ae99da295231911e9ac9d8e609383ff0150e852a0383f3d7c68f04036c37c4019
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.debian.tar.xz' libassuan_2.5.3-7.1.debian.tar.xz 13952 SHA512:f13525a7fda448bf878adf858c06ab9bec8df7d9e2d58a7f16bb6808d6459a988a4212e69526b1bb2990af19cfeffc1f30844606f5e3f398d6533b5342a07d5e
```

### `dpkg` source package: `libbsd=0.10.0-1`

Binary Packages:

- `libbsd0:amd64=0.10.0-1`

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
- `public-domain-Colin-Plumb`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.10.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.dsc' libbsd_0.10.0-1.dsc 2197 SHA512:9dbb2fc11b3740b54edc07762b977cb38ee1b3993b87d02f964b00b04c99f3a65a4ff0c5985a4d5786bc4b8f9b795d89a46eb2d90993ea99cb710ae2c5271a3a
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz' libbsd_0.10.0.orig.tar.xz 393576 SHA512:b75529785b16c93d31401187f8a58258fbebe565dac071c8311775c913af989f62cd29d5ce2651af3ea6221cffd31cf04826577d3e546ab9ca14340f297777b9
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz.asc' libbsd_0.10.0.orig.tar.xz.asc 833 SHA512:e7b438ce96ce6d6d0afa17568700e6317ca9336fd9f5a5a5dba842d4bc4cf0426799fc4872155b881ae32a777784e1acce727a66cd0ab37b0dcf529962782a99
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.debian.tar.xz' libbsd_0.10.0-1.debian.tar.xz 16660 SHA512:66bea622de0a3c92e0bae3408554c4e4a2205669753143d929e563f94ea47c4fe68d8f8559fdb826dc2d04b53848e392fc95ec88f1a3d6aaba995d4e6e1f4c12
```

### `dpkg` source package: `libcap-ng=0.7.9-2.2`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.2`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.dsc' libcap-ng_0.7.9-2.2.dsc 2081 SHA512:c94566b5dfb5eacc3510206530691ec5d821bdceb96f286c254b0b1c3a4d2157e784e3bc87d94599101d814b9115947152183c51ef8e9dd098298023a32a0dab
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA512:095edabaf76a943aab0645b843b14e20b1733ba1d47a8e34d82f6586ca9a1512ba2677d232b13dd3900b913837401bb58bf74481970e967ba19041959dc43259
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.debian.tar.xz' libcap-ng_0.7.9-2.2.debian.tar.xz 6308 SHA512:d5599574bb0e449edd7859f23de718b9e52dcc7296bea88807a4369fa3089d93b72a316bf9ed2398e9bac864d25f4ea6aa0772c2ddac1e204f0a1e2d4929ff29
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

### `dpkg` source package: `libdatrie=0.2.12-3`

Binary Packages:

- `libdatrie1:amd64=0.2.12-3`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.12-3
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.12-3.dsc' libdatrie_0.2.12-3.dsc 2260 SHA512:5e913935f1414c721c6d60922c8c0a57937c7d484785def3e1aaf2ccd7307f31c9d7c00555283553129986074f2959c5c5656637ff1447643b184f1eac44230b
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.12.orig.tar.xz' libdatrie_0.2.12.orig.tar.xz 310236 SHA512:7cf17859331d6111679e2c6fe0fa256abb13187b0b1116c8225f066281ab852f847a0d2d0d42b9604faf1d56290909fe3386362e34ed5bd1109516dffa2775a1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.12-3.debian.tar.xz' libdatrie_0.2.12-3.debian.tar.xz 9188 SHA512:62da4c1985cdaf97ca417699ba97652929b3da4d91679d728457af831a265d9bc31f73e350be8bb66367a24a1309eb0cc1ba8227e99defa7eefa8d8cbce16c8a
```

### `dpkg` source package: `libedit=3.1-20191231-1`

Binary Packages:

- `libedit2:amd64=3.1-20191231-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.dsc' libedit_3.1-20191231-1.dsc 2129 SHA512:0c476e8e3c597e6523c2fe81faf338f5a82f01bacdbfc05a174150566e32ebe2567416b77db457d5021f02fe363d5390ce28129696c233b38c6a13b6c787b025
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA512:1df2eced98e8db1bb0af940678c154d87e3b11dd21e65a903682367f5feace5112f9a543b8e0cb04bbfeaaf73729f808db2d9c302637fc063e81c0a37777ac2c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.debian.tar.xz' libedit_3.1-20191231-1.debian.tar.xz 14168 SHA512:f37f055e333c245e5a2b86c418d462b72da26e7349a292b8a89602d59ed77a9df7621fba6de94f6c2b5e25d74b14190fd463706fa49281dcf6ffa5c0e4f21286
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

### `dpkg` source package: `libexif=0.6.22-2`

Binary Packages:

- `libexif-dev:amd64=0.6.22-2`
- `libexif12:amd64=0.6.22-2`

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
$ apt-get source -qq --print-uris libexif=0.6.22-2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-2.dsc' libexif_0.6.22-2.dsc 2079 SHA512:12ba9414d750e970f0ab7dc6460d12c6dddb29d81b4d5081c9b2ac67db3049f12529f63e7af3cd08b79302cc767a729c8c7761fee1c5e2a080c5c7defeb418ac
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22.orig.tar.gz' libexif_0.6.22.orig.tar.gz 1109525 SHA512:6c63abe2734c9e83fb04adb00bdd77f687165007c0efd0279df26c101363b990604050c430c7dd73dfa8735dd2fd196334d321bdb114d4869998f21e7bed5b43
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.22-2.debian.tar.xz' libexif_0.6.22-2.debian.tar.xz 12016 SHA512:44895f661e654a6a103dbf61e5080637b424d8ea0fd60005d1ee971ab9b58ac5fc0e52ded7ec6437b9f8cac4d4b4027ff3fa933540056a8f876c8208120a9da3
```

### `dpkg` source package: `libffi=3.4~20200819gead65ca871-0ubuntu3`

Binary Packages:

- `libffi-dev:amd64=3.4~20200819gead65ca871-0ubuntu3`
- `libffi8ubuntu1:amd64=3.4~20200819gead65ca871-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi8ubuntu1/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4~20200819gead65ca871-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu3.dsc' libffi_3.4~20200819gead65ca871-0ubuntu3.dsc 2179 SHA512:3daf83b86b96208b825523ccdbb3900fe00d189b87811b57d661a3ab43e3b9e5b631ccb7fd2723a2df655b56c643fa0e2733c35f08c2732756eb59852bc85e00
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871.orig.tar.gz' libffi_3.4~20200819gead65ca871.orig.tar.gz 527371 SHA512:c349b1630db80c042f3c11efe58d4eb849e87f2cca0cc1748c99d32cc34ce4c1262825dc070c8a84263e0adcd8a7af3bd33c705ba28b6cc16974552b12bf0c65
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.4~20200819gead65ca871-0ubuntu3.debian.tar.xz' libffi_3.4~20200819gead65ca871-0ubuntu3.debian.tar.xz 7856 SHA512:5496d2d4147aa2ca5e579c149206d2cb1db39f14f7d351b4224496b3289b68f83a8715366bcad933fa798815e8aef416270c77576aaca2a921a7ae5c4b8abb3e
```

### `dpkg` source package: `libfido2=1.4.0-2`

Binary Packages:

- `libfido2-1:amd64=1.4.0-2`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0-2.dsc' libfido2_1.4.0-2.dsc 2565 SHA512:bc1b7885bd85e180513c0bd86930babbe90812b6ecd7ed4e08c8df05b0d1aecb83029f05942e192ed84b274612adca87a85e7073694862b3a816d49fac1d09f5
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0.orig.tar.gz' libfido2_1.4.0.orig.tar.gz 391439 SHA512:5cf2f2d70bdba893fd33bf3ca91940c7eded5ed1728b517ff3fc46cbde58bf64f16da4104138b20dcea1d9a1cec730e532bc4938cdcba4ad86343e51a1c3c513
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0.orig.tar.gz.asc' libfido2_1.4.0.orig.tar.gz.asc 488 SHA512:03c0b0c43550b55605ddfd5fc930e3605499a1c3f9e5a23a929db8ac6b7b59f3b64f821958a506ed945b209e27ca9ba62b3bb6e47dbfcd7c9499d7191244c15c
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0-2.debian.tar.xz' libfido2_1.4.0-2.debian.tar.xz 73908 SHA512:d4ce7a549065fcc810b2ca3323fde5729e2b4916b3b721cd937258a33ea5df804d8f072d598ee3f15dbddd4c78280e200ea26038362963ada16bd5d59b9818d4
```

### `dpkg` source package: `libgcrypt20=1.8.5-5ubuntu2`

Binary Packages:

- `libgcrypt20:amd64=1.8.5-5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.5-5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu2.dsc' libgcrypt20_1.8.5-5ubuntu2.dsc 2907 SHA512:f575ef08da63de917a6326ae86a3dbfffca11a7d729e0e7cfbdf8e3c15154b5ee044ba9825481c616c9049854cf625b38c2b0b602cb0ddb75065fa351be2f338
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2' libgcrypt20_1.8.5.orig.tar.bz2 2991291 SHA512:b55e16e838d1b1208e7673366971ae7c0f9c1c79e042f41c03d14ed74c5e387fa69ea81d5414ffda3d2b4f82ea5467fe13b00115727e257db22808cf351bde89
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2.asc' libgcrypt20_1.8.5.orig.tar.bz2.asc 488 SHA512:3993c5e3f2f1714f40a9ad1a19782362c5b80c070ed8d76feacc503d8719f6775465f478098a092730e02683c665c5c91cf30e7700215aae2322be6230f207d6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu2.debian.tar.xz' libgcrypt20_1.8.5-5ubuntu2.debian.tar.xz 35444 SHA512:c14cc8a713fe2bb47c0920d05e68996b92fd34db781d5d6ae2a82e06dad9ba77d647ca8cc59e2bb1d75e82d2d6874ec82d9ad371175a0a827ab604e20585eb89
```

### `dpkg` source package: `libgpg-error=1.38-2`

Binary Packages:

- `libgpg-error0:amd64=1.38-2`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.38-2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2.dsc' libgpg-error_1.38-2.dsc 2220 SHA512:3806e8a764b6cb8cab4b86d7af19afb680c438b05e0357521137cf950edc1bcb75c368f3a0864b639ff9ed1528febcb604fa7818827fd29d180ba65bc39e44c3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2' libgpg-error_1.38.orig.tar.bz2 957637 SHA512:b936a4738c2cee111d855b1ba3ec433da8c77799a87d1f71275f974f871ebfa593c9db06ea53f0490b6cd6b94bef34f6052a587a4d13d839ec0128500c2dd9de
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2.asc' libgpg-error_1.38.orig.tar.bz2.asc 488 SHA512:0f167c6d87f8028c294db2822c2e092f156504893c0bdd8bf883d00dcdd838fed4af5fd3726ab88d41f4e12e8b131cec45dcc610aeb25291ea870d3b9cb621f6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-2.debian.tar.xz' libgpg-error_1.38-2.debian.tar.xz 19544 SHA512:319731a51f785d6a0b250dfa9c7ee3951692c051d1d161d2cef31dd20f25662af47edbdf71a85bc5ecbcf423846dc43df85e0af5a8d2734ddae0927e72626128
```

### `dpkg` source package: `libice=2:1.0.10-1`

Binary Packages:

- `libice-dev:amd64=2:1.0.10-1`
- `libice6:amd64=2:1.0.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1.dsc' libice_1.0.10-1.dsc 2049 SHA512:61fda8a2a78b9c1845666f20eab37a3fb5b806f11cd4b959ad084b47640e41740fc1876596a00316a3687ccccb70c0903595396962930e0228d0f20ed57b54e0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10.orig.tar.gz' libice_1.0.10.orig.tar.gz 481960 SHA512:2d4757f7325eb01180b5d7433cc350eb9606bd3afe82dabc8aa164feda75ef03a0624d74786e655c536c24a80d0ccb2f1e3ecbb04d3459b23f85455006ca8a91
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.10-1.diff.gz' libice_1.0.10-1.diff.gz 11349 SHA512:e8709dffbedbfa0e07896f0176e57c91da571a7eef143492c0815092d8615756a55c4144460c62d6a06f8cc9c5d8b4975b7e62a4ebd82f3ee89d6cb315d4f187
```

### `dpkg` source package: `libidn2=2.3.0-1`

Binary Packages:

- `libidn2-0:amd64=2.3.0-1`

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
$ apt-get source -qq --print-uris libidn2=2.3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-1.dsc' libidn2_2.3.0-1.dsc 2411 SHA512:44a6116df967e852c43dcfa31de888eb68425494d265d31908ffe44c276ced55a62107976194bae926e01a1648bb17c797d1567006d5f7d1065becb664d65e78
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0.orig.tar.gz' libidn2_2.3.0.orig.tar.gz 2164993 SHA512:a2bf6d2249948bce14fbbc802f8af1c9b427fc9bf64203a2f3d7239d8e6061d0a8e7970a23e8e5889110a654a321e0504c7a6d049bb501e7f6a23d42b50b6187
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-1.debian.tar.xz' libidn2_2.3.0-1.debian.tar.xz 10588 SHA512:288eefd1abc264fe9d4049e53fbc6e8c236ca21ec98f5dc5bd737b7d44305a4e2bdfb03b033d0dcda5d35cc514090b68d1366821802e7767c0473ca3751b0998
```

### `dpkg` source package: `libjpeg-turbo=2.0.3-0ubuntu2`

Binary Packages:

- `libjpeg-turbo8:amd64=2.0.3-0ubuntu2`
- `libjpeg-turbo8-dev:amd64=2.0.3-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=2.0.3-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3-0ubuntu2.dsc' libjpeg-turbo_2.0.3-0ubuntu2.dsc 2305 SHA512:14da12e111cd4a4809d518d72d61d7f00616f009ef56d892a095ccc86353b53378cf28a433f7551ebac9494c347984188da6a0b4b24c8427e786227183c2ba0f
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3.orig.tar.gz' libjpeg-turbo_2.0.3.orig.tar.gz 2161279 SHA512:745cc3d50b43dd84721bc3c341d561ffd7f54eda5bbe2d56cad62f4b51ea76da3b18aba9ca694a9db79379aba7a9971cb146387979e96ca6ece950871276cf2f
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.0.3-0ubuntu2.debian.tar.xz' libjpeg-turbo_2.0.3-0ubuntu2.debian.tar.xz 18208 SHA512:b6f9bad6ef2a049d695fa81e890f0aca163b84ee27a1da1643779e2d27ff4ec04d9a862cfc9476e4176b19bcf9f33e3176aac3785aa9c25628d3dd5d2bdc9d1a
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

### `dpkg` source package: `libksba=1.4.0-2`

Binary Packages:

- `libksba8:amd64=1.4.0-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `FSFUL`
- `GPL-3`
- `LGPL-2.1-or-later`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0-2.dsc' libksba_1.4.0-2.dsc 2470 SHA512:e3f7e640df148deae10a28f9b94f78b84b919393011e4035b71d88e3b3f2586f103371d2c94471898612040b0f6e13e8d4f168e4ff1e7e621ad8fa51fee96223
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0.orig.tar.bz2' libksba_1.4.0.orig.tar.bz2 651319 SHA512:7c1666017ebfa50b5663153dead1e019e0ee342c4f44ee8f644fc749e82dcc983237ef0f557de9de3f7908dc90405d967a4db2e36e04fe0d5a09edf49f8a0c8d
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0.orig.tar.bz2.asc' libksba_1.4.0.orig.tar.bz2.asc 488 SHA512:5968660e0b699d6e5f5bf35e60f4492ee523dbebc11a773b490aa84144cb7cf317d76f1879d418a43f3ce23ba7079c2337a8a0309e1d986bf582ca0fd954dc91
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0-2.debian.tar.xz' libksba_1.4.0-2.debian.tar.xz 10368 SHA512:48d91746400d71b5cc8f0f78caf95f6d855da5dccb4b4b4ea18e537fc739b697cfdc7414256b44505f2ccc9e5b623e9bed8e4fbeb6b84f613c62da584fc718b9
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

### `dpkg` source package: `libmaxminddb=1.4.2-0ubuntu1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.4.2-0ubuntu1`
- `libmaxminddb0:amd64=1.4.2-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libmaxminddb-dev/copyright`, `/usr/share/doc/libmaxminddb0/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `CC-BY-SA`
- `GPL`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libmaxminddb=1.4.2-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.4.2-0ubuntu1.dsc' libmaxminddb_1.4.2-0ubuntu1.dsc 2209 SHA512:6268eaa03845afd7a978f9542c91d85d9145327e3a2001e8574dc689d7e8c6bf94dffae875305d4845dbec1b94e014d11824a0ec3dc1f0efc89019efd8820147
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.4.2.orig.tar.gz' libmaxminddb_1.4.2.orig.tar.gz 600664 SHA512:bc18d2f19a74639888a466483afde1bccfc3a83787011a6f38808b76e5a513c9912ff369ccbf584091d4def657e0574b16b35dc69ab12ae4c439aaaf3669c4c1
'http://archive.ubuntu.com/ubuntu/pool/main/libm/libmaxminddb/libmaxminddb_1.4.2-0ubuntu1.debian.tar.xz' libmaxminddb_1.4.2-0ubuntu1.debian.tar.xz 4780 SHA512:03a7c01c6cfe0fc9df94f1d051f4af7c0666aa008f9049e692e38904a1473408feaed65f49a533f00e19d9e552df9817c8d20f338796aad1f6746c7a99660bdc
```

### `dpkg` source package: `libnsl=1.3.0-0ubuntu3`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-0ubuntu3`
- `libnsl2:amd64=1.3.0-0ubuntu3`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-0ubuntu3.dsc' libnsl_1.3.0-0ubuntu3.dsc 2062 SHA512:b0f64be153bc9cc1afd5c1880fec6eda0c8026e18442565696248d4876c781ac94f04124e748ae359e2b38b2b90fbe5b21b064685c7c5bea48baee06d15d9aa2
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA512:a5a6c3ccb2d1e724c8c1f65e55dcd09383eb1ae019c55f4c09441eadf23ffbc2196cfad259805b0ac40ddf3a10af0da453e4d739d67d46829c64d0995dab4e55
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnsl/libnsl_1.3.0-0ubuntu3.debian.tar.xz' libnsl_1.3.0-0ubuntu3.debian.tar.xz 4740 SHA512:48723ab4335103b3371f8706e78150cdd35a5d3fcd32800cb27d5152aacf10f65dc148c77f8320f43f53e591d0a1b7266cc03e28d2526d95b0a9025283c777c2
```

### `dpkg` source package: `libnss-nis=3.1-0ubuntu4`

Binary Packages:

- `libnss-nis:amd64=3.1-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libnss-nis/copyright`)

- `BSD-3-Regents-DEC`
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
$ apt-get source -qq --print-uris libnss-nis=3.1-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nis/libnss-nis_3.1-0ubuntu4.dsc' libnss-nis_3.1-0ubuntu4.dsc 2052 SHA512:d8c1e8baaf5f903e94aae3f332987f98ede739635457d739ad7d2c083fa98ca26862a53730828d57b17ac69fde49c28ed7cba0fd26efd5f2049981766fb8f291
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nis/libnss-nis_3.1.orig.tar.xz' libnss-nis_3.1.orig.tar.xz 257440 SHA512:3743730aeaf98011d40c0d242f34967ab382d586bbe8da1eb5b3698070c73ca967bbb6dc9dfac0e4c5074a293e0d3f009bfd44c2a50aeb648d65ffd0d6468715
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nis/libnss-nis_3.1-0ubuntu4.debian.tar.xz' libnss-nis_3.1-0ubuntu4.debian.tar.xz 4644 SHA512:5e2e042fed93d7eeac81d969be5cdf08eed67a45d370db2df24439ade08c495c8f0d4ec80fee677e6ba8d4d908d940933781472c6adf60a202718ff5a0d4b8f2
```

### `dpkg` source package: `libnss-nisplus=1.3-0ubuntu4`

Binary Packages:

- `libnss-nisplus:amd64=1.3-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libnss-nisplus/copyright`)

- `GPL-2`
- `GPL-2+-libtool-exception`
- `GPL-3`
- `GPL-3+-autoconf-exception`
- `LGPL-2.1`
- `LGPL-2.1+`
- `permissive-autoconf-m4`
- `permissive-fsf`

Source:

```console
$ apt-get source -qq --print-uris libnss-nisplus=1.3-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nisplus/libnss-nisplus_1.3-0ubuntu4.dsc' libnss-nisplus_1.3-0ubuntu4.dsc 2086 SHA512:0cab077dde1c0eb3889bb13bcdea282fd5426ecfc52ed0db6f5aad559c1dd7ffee0ccbb9bd8948e0ca9509986497e6227ed7a54aba108baf6e46b655e28fdcb4
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nisplus/libnss-nisplus_1.3.orig.tar.gz' libnss-nisplus_1.3.orig.tar.gz 203693 SHA512:bccfee33c7ab69b2b3db6b6bc35509791ef958f9a776b1b5bbd11c35c53f2a07deb80c64344956fab1d67d69545f3fa730fc8decedd3c75a435f72c805b3e906
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnss-nisplus/libnss-nisplus_1.3-0ubuntu4.debian.tar.xz' libnss-nisplus_1.3-0ubuntu4.debian.tar.xz 6452 SHA512:193ee5902866b75207ea3915477f16ba4f33ae935712ae28f13c32a82342e9ae4d1093aebed132ee04d07a983e50c04c6510e34446c93e11ad0f9a7b737371b1
```

### `dpkg` source package: `libpng1.6=1.6.37-3`

Binary Packages:

- `libpng-dev:amd64=1.6.37-3`
- `libpng16-16:amd64=1.6.37-3`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.37-3
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3.dsc' libpng1.6_1.6.37-3.dsc 2225 SHA512:25bb2f81e07ea84b5d462a435154c632e33f4ffcbc4b326cdb90e805fb322c55ac10baad1a8599e99c30f526fbaeb68691916a5e5cb21e9b8b401856c956eb5c
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37.orig.tar.gz' libpng1.6_1.6.37.orig.tar.gz 1508805 SHA512:ccb3705c23b2724e86d072e2ac8cfc380f41fadfd6977a248d588a8ad57b6abe0e4155e525243011f245e98d9b7afbe2e8cc7fd4ff7d82fcefb40c0f48f88918
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.37-3.debian.tar.xz' libpng1.6_1.6.37-3.debian.tar.xz 32272 SHA512:572781fe5581cbff3a140922bb611e84d44511256d766b85b4e334a47afc3ffbb7d60f96068945efb7e9e4f3d92b8beb63593dab8752d85182c6ecc26907ef37
```

### `dpkg` source package: `libpsl=0.21.0-1.1`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libpsl/0.21.0-1.1/


### `dpkg` source package: `libpthread-stubs=0.4-1`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.dsc' libpthread-stubs_0.4-1.dsc 1927 SHA512:890812cdb72381fbae09d2273cf80fe751097ed1595b065d1ed1f789a7115ccb559fa96d729785226dfefcab84be0826478541f483f81454922adfc1d91d4278
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4.orig.tar.gz' libpthread-stubs_0.4.orig.tar.gz 71252 SHA512:5293c847f5d0c47a6956dd85b6630866f717e51e1e9c48fa10f70aa1e8268adc778eaf92504989c5df58c0dcde656f036248993b0ea5f79d4303012bfeff3c72
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.4-1.diff.gz' libpthread-stubs_0.4-1.diff.gz 2346 SHA512:bd46c806b16fe18162078eda8778319da4ca672877eea3c255747b5f0d12dc23bc43ba27dd2ae2d2d7edabc83c285855d5efe694db709fa896a598c97e1475c7
```

### `dpkg` source package: `librsvg=2.49.5+dfsg-1`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.49.5+dfsg-1`
- `librsvg2-2:amd64=2.49.5+dfsg-1`
- `librsvg2-common:amd64=2.49.5+dfsg-1`
- `librsvg2-dev:amd64=2.49.5+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `Apache-2.0`
- `Apache-2.0,`
- `BSD-2-clause`
- `BSD-2-clause,`
- `BSD-3-clause`
- `BSD-3-clause,`
- `Boost-1.0`
- `Boost-1.0,`
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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/librsvg/2.49.5+dfsg-1/


### `dpkg` source package: `libseccomp=2.4.3-1ubuntu4`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu4.dsc' libseccomp_2.4.3-1ubuntu4.dsc 2539 SHA512:5c7230d6636e5effa91bb501c7e5c5ca4a560ca0e1ebb7e578fb9c44b963e500bd05306da41a4f87a436fb09f45e6b04c10e5baef7780084b087466539dc31e9
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA512:7b7af2e98493243ffe1934fefff5723b24ae9b9bdc4bf039343ee8456c15acb0ea34e81ec292a41143848272aeca794ef92ad38fc3f42c77465170cb540479ef
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu4.debian.tar.xz' libseccomp_2.4.3-1ubuntu4.debian.tar.xz 36432 SHA512:7cbf6b35628be7426c1015a71f879ec40fe8f18dfd18ffb1e87140ba8b85af89dee9c0ff1449b3e54784754263aab6d2aacbdfe66fbc3a51fa765b47bd307fac
```

### `dpkg` source package: `libselinux=3.1-2`

Binary Packages:

- `libselinux1:amd64=3.1-2`
- `libselinux1-dev:amd64=3.1-2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`, `/usr/share/doc/libselinux1-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-2.dsc' libselinux_3.1-2.dsc 2310 SHA512:75a7bc7fb4ff0c3e00fbb68e0dd960929622cda132df46c529395963e446c29218a89fd97ba3cb6790961d35ec90436f4150a120493d3c35edf978160d5ef9dc
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1.orig.tar.gz' libselinux_3.1.orig.tar.gz 204703 SHA512:57730cddd2d4751556d9e1f207c0f85119c81848f0620c16239e997150989e3f9a586a8c23861fd51ed89f7e084ad441190a58a288258a49a95f7beef7dbbb13
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.1-2.debian.tar.xz' libselinux_3.1-2.debian.tar.xz 23788 SHA512:8d6e869dd13df6e155529056c1e1f3b30771ffe264c94507f3b655189ab56b04454f9f1470c21ae123e5dcb788ea1730204f5d8388b8f8cfb6af8973f2266a67
```

### `dpkg` source package: `libsemanage=3.1-1`

Binary Packages:

- `libsemanage-common=3.1-1`
- `libsemanage1:amd64=3.1-1`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1.dsc' libsemanage_3.1-1.dsc 2339 SHA512:e2bbd7f9aa15d9601c8730dc6c392a67296cf2f199f116eb62e5806b14882ed258ea7b474071559fd786ceb199349e21d89b39d00814a0fd158cac246171dfd0
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1.orig.tar.gz' libsemanage_3.1.orig.tar.gz 179601 SHA512:8609ca7d13b5c603677740f2b14558fea3922624af182d20d618237ba11fcf2559fab82fc68d1efa6ff118f064d426f005138521652c761de92cd66150102197
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.1-1.debian.tar.xz' libsemanage_3.1-1.debian.tar.xz 17556 SHA512:ffee5fea8f9c85a80089f7788b95e9b7f275187326bca53aa4aa350911a6fcc2cf642eab51700447a8716495718db096bc5efb2ff05f90fe3f66d5a8d0e1554b
```

### `dpkg` source package: `libsepol=3.1-1`

Binary Packages:

- `libsepol1:amd64=3.1-1`
- `libsepol1-dev:amd64=3.1-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`, `/usr/share/doc/libsepol1-dev/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.dsc' libsepol_3.1-1.dsc 1776 SHA512:74a0dd6f3db6578261b78114f46030cd0486b05d0482421bacb5a74a30cbdc98932691c60293d96e5fd258839136d8e0988eb0371cbd6e685b6bce38e0a95bc7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1.orig.tar.gz' libsepol_3.1.orig.tar.gz 473842 SHA512:4b5f4e82853ff3e9b4fac2dbdea5c2fc3bb7b508af912217ac4b75da6540fbcd77aa314ab95cd9dfa94fbc4a885000656a663c1a152f65b4cf6970ea0b6034ab
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.1-1.debian.tar.xz' libsepol_3.1-1.debian.tar.xz 14584 SHA512:e7c48cde2e2d8748f4df3b6b02c66ffb97ee21c2b749b2d7c9154ac4d4c73fd09a383972ac39edcb6f04faf2631c1dba3512b6622b612e1aec54bc58608df5db
```

### `dpkg` source package: `libsigsegv=2.12-2build1`

Binary Packages:

- `libsigsegv2:amd64=2.12-2build1`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.12-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2build1.dsc' libsigsegv_2.12-2build1.dsc 2466 SHA512:8bb7cf3b64c3682f1d9720a7469fe8e1b11c7e9833e4118b4f9ffceaff8ab5b23fafa958eeeeb7391369c329c2d1343f4ac7729c868efd4fa83c86b51e902a2d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz' libsigsegv_2.12.orig.tar.gz 451408 SHA512:27986e8aaf4357ed131032aa7c281a5a28c5759530c62bb76f034aea33959547dcaae805e06347a1f532f0488b72fbbbdac4400f74e8d3f2128511526e8a5913
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz.asc' libsigsegv_2.12.orig.tar.gz.asc 2442 SHA512:d0311e322975a2a1e5fe965dd5ee0bdf4daf10892f056e9c9ec07097f51bd9229d88efd1ab29277776bb79e7e854c834e13b108e81d1fef10701b2e3e416ea57
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2build1.debian.tar.xz' libsigsegv_2.12-2build1.debian.tar.xz 8448 SHA512:afbb6b5dd185b80703e2405b5aa4bca5d061c87127ede14fdb0af9d73354cd4a916595156f03332498f562d70edbe6b0ef4d6ae22d1ef676db126b3ef0bca025
```

### `dpkg` source package: `libsm=2:1.2.3-1`

Binary Packages:

- `libsm-dev:amd64=2:1.2.3-1`
- `libsm6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1.dsc' libsm_1.2.3-1.dsc 2063 SHA512:3453c5c83ee34a008a1674dfc347d6270a51e5e2b2da90cc0b3e9a2f8b5f6524248541123dcac1cb7a14e35f5546dc3c514ae5bc1f74748b3b9f986a34b88f4b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3.orig.tar.gz' libsm_1.2.3.orig.tar.gz 445362 SHA512:03b77d86b33cdb3df4f9d65131a0025182f3cb0c17b33a90d236e8563b3011d225b9d006186302d07850edafa5b899aec6a086b8d437d357cd69fedd5f22d94b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.3-1.diff.gz' libsm_1.2.3-1.diff.gz 8929 SHA512:5cd42b75eabce2c66baa2f22f808f219ef70635e67405743c62d814dd0c1f1a78f2a09e4a5c08ba0e1574a2f07d2161af455e454077ebfa02ab2eb7e9269a362
```

### `dpkg` source package: `libssh=0.9.4-1ubuntu3`

Binary Packages:

- `libssh-4:amd64=0.9.4-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.4-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4-1ubuntu3.dsc' libssh_0.9.4-1ubuntu3.dsc 2131 SHA512:3a0c0e91cba9f1292d4e184eb504384c3ad4adc5cb827dc97e798c27e05296da5f3e0b6b072bdf34b022eb19f6da9d71d322823820f0d1ca9428fc86c99e663f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4.orig.tar.xz' libssh_0.9.4.orig.tar.xz 500776 SHA512:38705c19c293ea5e6d286d22eb17021dbe58d88c1e647b699933aa0db9ca1174d43d1ff76c1a1b17bf2cc1a8297ec02f1a67dd9e969676dd69cf6fbdae9bc8d4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4.orig.tar.xz.asc' libssh_0.9.4.orig.tar.xz.asc 833 SHA512:a64e0bd0cc821206359c0b57b97457306cdab92999083800e089aecffbbd251728537264eac55ca69a70a8345ca71db9e3462fa450bb01919f670738eb8ebd7e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4-1ubuntu3.debian.tar.xz' libssh_0.9.4-1ubuntu3.debian.tar.xz 29208 SHA512:4c4ed598bfc0a7cd05a3a1a5f3ea899ab65c9aac90c73242fc36d6d6c8c118923f4c8c63d43105b69c1a54233a7b09a2ca549573523e15325916daf99ba36270
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

### `dpkg` source package: `libthai=0.1.28-3`

Binary Packages:

- `libthai-data=0.1.28-3`
- `libthai0:amd64=0.1.28-3`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.28-3
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28-3.dsc' libthai_0.1.28-3.dsc 2346 SHA512:fe78b44906cb9bcdfb7bcdfe8adae83f6c74dbe1f829224e9c52c442192a6cf886736476ccb62f2a16816f0ff84d853b63f7f6e323d5e8870a4910920bc9c83a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28.orig.tar.xz' libthai_0.1.28.orig.tar.xz 413592 SHA512:925be8367ae0cba026e602f1f60c813306e9051e22fe722afba496b6e493f8c1f3eb56abb77ca663f53678b14ad793daf3269b32d32720c0d869b906cdf15f4e
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.28-3.debian.tar.xz' libthai_0.1.28-3.debian.tar.xz 12128 SHA512:e8220749c5683355909cc1b026f370d931d3a16ae883abd96770f0f00249b2c163265a4c9745d89b3a624f07ff737d852c1fbcd285098497565900854382db96
```

### `dpkg` source package: `libtirpc=1.2.6-1build1`

Binary Packages:

- `libtirpc-common=1.2.6-1build1`
- `libtirpc-dev:amd64=1.2.6-1build1`
- `libtirpc3:amd64=1.2.6-1build1`

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
$ apt-get source -qq --print-uris libtirpc=1.2.6-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.2.6-1build1.dsc' libtirpc_1.2.6-1build1.dsc 2063 SHA512:9c47d12cf25ace79c6b964454d22c49f2449e612183c81052555509cec983f6c5ef76daf3804da3eef0fffbf41e008f3b254302090736b98d756f085aefffcb8
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.2.6.orig.tar.bz2' libtirpc_1.2.6.orig.tar.bz2 513150 SHA512:bcb6b5c062c1301aa1246ec93ae0a5c1d221b8421126d020863517cb814b43ed038fb6c0c2faf4e68ff133b69abefe4f4d42bfc870671da6c27ca941a30b155a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtirpc/libtirpc_1.2.6-1build1.debian.tar.xz' libtirpc_1.2.6-1build1.debian.tar.xz 10476 SHA512:7209185d654c6c5921f8b687e24f9d299f70b17259532d483494d894d2e568639fc7259a908e799ce0ccfe0d93c4d0f32152d96f5a666bfd8f7b09c21bcc93a3
```

### `dpkg` source package: `libtool=2.4.6-14`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-14`
- `libltdl7:amd64=2.4.6-14`
- `libtool=2.4.6-14`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-14
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-14.dsc' libtool_2.4.6-14.dsc 2500 SHA512:e74e10f28a6e78bb0e058ab74bf4b4ba8e6412b5d65ff0aaa2624cf248e848630d29f8dfc58248eaa7fd63ea73347fbb067ea52c11231a3bd482f6d36b3aaff4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA512:a6eef35f3cbccf2c9e2667f44a476ebc80ab888725eb768e91a3a6c33b8c931afc46eb23efaee76c8696d3e4eed74ab1c71157bcb924f38ee912c8a90a6521a4
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA512:2f26447a837e3242b8f8f38fbab22d89df0949ee62fd966af3b5bae3aa939ba53bc4621174ee58d1c6722d569d7fe5f90097ddccffed28c3067fe5fa996fcb89
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-14.debian.tar.xz' libtool_2.4.6-14.debian.tar.xz 50832 SHA512:1cfb4ae9a854ee19e0246fae1ed0d6cac270ce886d8e0003b12df4a740c7323cfdd11795ffc3187b9e0f4d34f03f18b4922f67109274c7e2993ec0e0863c704f
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

### `dpkg` source package: `libwebp=0.6.1-2`

Binary Packages:

- `libwebp-dev:amd64=0.6.1-2`
- `libwebp6:amd64=0.6.1-2`
- `libwebpdemux2:amd64=0.6.1-2`
- `libwebpmux3:amd64=0.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp6/copyright`, `/usr/share/doc/libwebpdemux2/copyright`, `/usr/share/doc/libwebpmux3/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.6.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.dsc' libwebp_0.6.1-2.dsc 2064 SHA512:9f3c66da0131970aecf045d013c68b5fec79bc1fcacdd90f0350edd1137b6b0cc1b148e754ef32d7c935251c80504620b957965423741ad89cb1361e3da6a6f6
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA512:313b345a01c91eb07c2e4d46b93fcda9c50dca9e05e39f757238a679355514a2e9bc9bc220f3d3eb6d6a55148957cb2be14dac330203953337759841af1a32bf
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.debian.tar.xz' libwebp_0.6.1-2.debian.tar.xz 9532 SHA512:c1a18ec35b059f40a1303f3ad2bffc448bc666f54a7d7306ccc7cdc579b6495f121111f600108bbd732f6050b07d43a443b412968482a12b37348c40a22b0963
```

### `dpkg` source package: `libwmf=0.2.8.4-17ubuntu1`

Binary Packages:

- `libwmf-dev=0.2.8.4-17ubuntu1`
- `libwmf0.2-7:amd64=0.2.8.4-17ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-17ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu1.dsc' libwmf_0.2.8.4-17ubuntu1.dsc 1642 SHA512:574cc44e7e7bb4936ee5b2269e6f83bafcac8ba7ffb37e2f56e9e476d2bf8720ae937adc1676ffa1dea2241766e2a2af7ac4d88b3be5c9a8d452951edafc0c17
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA512:d98df8e76a52245487b13e5ab3d2fbba9d246f97ee04a7344c0e5861bb2d0f990fc6d662dbd849ce621768b06eaebd4270fb34bec4ee004334a98b14ba6044a5
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-17ubuntu1.debian.tar.xz' libwmf_0.2.8.4-17ubuntu1.debian.tar.xz 12968 SHA512:7f5119e8e78973b6739ff6314239a7348e49e2e9cfd71d40c16b6c30e3de82c022252b197094536db1acf950a5216a0be19b44c651af8083515661535c998673
```

### `dpkg` source package: `libx11=2:1.6.10-3`

Binary Packages:

- `libx11-6:amd64=2:1.6.10-3`
- `libx11-data=2:1.6.10-3`
- `libx11-dev:amd64=2:1.6.10-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/libx11/2:1.6.10-3/


### `dpkg` source package: `libxau=1:1.0.9-0ubuntu1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.9-0ubuntu1`
- `libxau6:amd64=1:1.0.9-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-0ubuntu1.dsc' libxau_1.0.9-0ubuntu1.dsc 1563 SHA512:328dde9971c137996e8961332f166a3fd9ab9bdb71eba364fbc31ada0b49ae0e632f5d9524b2309356f095727a91b585fe6fdb5ea7b1aa3d11a82043e71220d2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA512:3b22f34a4e35d17421189df8ce3f858b0914aef0cea0b12689dd8576f14eb811e39d6e32384251573daa7e3daba400deea98e7c0e29b4105138cf82195d7f875
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-0ubuntu1.diff.gz' libxau_1.0.9-0ubuntu1.diff.gz 15142 SHA512:1ae8ca9bd62101b49586df2f538e2cc045f936c293429d5285b154ff84e23959ae98a8e47930b4d344ceff3a16b12cb8414e9387d902c77dd2703646c0da53f1
```

### `dpkg` source package: `libxcb=1.14-2`

Binary Packages:

- `libxcb-render0:amd64=1.14-2`
- `libxcb-render0-dev:amd64=1.14-2`
- `libxcb-shm0:amd64=1.14-2`
- `libxcb-shm0-dev:amd64=1.14-2`
- `libxcb1:amd64=1.14-2`
- `libxcb1-dev:amd64=1.14-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.dsc' libxcb_1.14-2.dsc 5344 SHA512:6b1b271519993b813a0cf664074494f7260a6eb3a8dc820ec5cbd486e2d07df356132f0c05fdcda806b1fbb570e08c1701d40255c3e59c760bbee238832d3680
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA512:6114d8c233b42b56604787a0475e924143aa13f1d382e6029b2150a4360c12ce78073409f754fbb1e5d9f99fc26900c0a4c59e9cfbd4c3d0a3af0c1306e62da1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.diff.gz' libxcb_1.14-2.diff.gz 25716 SHA512:c1b2159b673bb91dbc3c7812ce28dad9cc256296025c2b4db7e75e28b0ab6e7f69ff47154e6ea3e2784ad9b4297f3a0cb3e7adea38c73f16ccb33f577f16ba0d
```

### `dpkg` source package: `libxcrypt=1:4.4.16-1ubuntu1`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.16-1ubuntu1`
- `libcrypt1:amd64=1:4.4.16-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.16-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16-1ubuntu1.dsc' libxcrypt_4.4.16-1ubuntu1.dsc 2212 SHA512:16ae25c5659b49ead1e01ecbcef8bc9315adec4b4a70e954382a8396a7fbdc0ec762996f7e75f57111d19cb982ac0139b1f83677edc88ec97e733d3b27dba946
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16.orig.tar.xz' libxcrypt_4.4.16.orig.tar.xz 354788 SHA512:e1336816e886f79a82882c9525abf48a282fa9cb18361a70812530760ca5e055bcbe5437c25b9e105cde7148325c0ec72572662535fb326fb24bfbd9020b0618
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16-1ubuntu1.debian.tar.xz' libxcrypt_4.4.16-1ubuntu1.debian.tar.xz 5840 SHA512:66b1343877ffa07cedc2e92fb1d33e0b1771b351569b1bb8d48826ce6acbe68ce8fd4ab2e753c5923b3a52769087fa5b81d13642539b3afa21e41c04b420c204
```

### `dpkg` source package: `libxdmcp=1:1.1.3-0ubuntu1`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.3-0ubuntu1`
- `libxdmcp6:amd64=1:1.1.3-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.3-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu1.dsc' libxdmcp_1.1.3-0ubuntu1.dsc 1608 SHA512:e49dc560e1819123a5eea6a71c1c5bb97d726b84ff3f940632dd9b1e0a819e315676f730b8a42033254d7713c80f219f4130a0078d23f826ff29301f646e9524
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3.orig.tar.gz' libxdmcp_1.1.3.orig.tar.gz 429668 SHA512:edd05654ad9ea893e9e08269e25ea050d10eaf9f997a08494e24127d1ba0c896cd5338b4595b155c8cbf576e1d910b76e6ad7820fee62d74644f1f276551e2f2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu1.diff.gz' libxdmcp_1.1.3-0ubuntu1.diff.gz 18079 SHA512:47fc7f07b65ef9a06924eff3e752fbe852d5f4ee40e45eff827fa76da200e7903dfaf2d4b3505f8b3a0dd14196a53ff9f3b182c099f9327c9591ff512305e00d
```

### `dpkg` source package: `libxext=2:1.3.4-0ubuntu1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.4-0ubuntu1`
- `libxext6:amd64=2:1.3.4-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.dsc' libxext_1.3.4-0ubuntu1.dsc 1727 SHA512:504328765410e07377746da12489f06f58dedf3ed390a83c10e9550cd39515fba9240245885e3d45be3fd412ec629ea4770e28e8f80dfe3db63f40665b373844
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA512:4eebd639fd57cb9b84a1e17e368f82fbf3d9f021eef5ad3fe31dd128500db57862a82c1e0d214d447cb7641b2be3fd7e949ee1196f2a482793c6628fb1e5cd70
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.diff.gz' libxext_1.3.4-0ubuntu1.diff.gz 20663 SHA512:bbfb69ff7175641e6c2f2e0b5ae449d56f4a7822ad9273616514cb632dea70afcff7c461510b528e2fa1c5000fb738a2279c9787fae4d5cfe3a97a3a6f769976
```

### `dpkg` source package: `libxml2=2.9.10+dfsg-5build1`

Binary Packages:

- `libxml2:amd64=2.9.10+dfsg-5build1`
- `libxml2-dev:amd64=2.9.10+dfsg-5build1`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.10+dfsg-5build1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-5build1.dsc' libxml2_2.9.10+dfsg-5build1.dsc 3085 SHA512:72194b4d6d9b834eed44e6e0ebf3d6670ceb9b635cb87ce858e5b24fc3e523ec7631a6ce762c469a346c694d0af5a1803ba2cdd40f2bc73b716894ff632600b4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg.orig.tar.xz' libxml2_2.9.10+dfsg.orig.tar.xz 2503560 SHA512:605c6c0f8bf2c53208d0a036ff09a4025843f45139b711c90dc83066feda2f285a5578d55d4a58d33eedbe7485a5c1ec5608ba6c6beed1fb55649f87dca0cec3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-5build1.debian.tar.xz' libxml2_2.9.10+dfsg-5build1.debian.tar.xz 28856 SHA512:455e75dbd365a79a5022be8b18535acfc9b95887319097106162a04e1e8322b3c70714262a32cd8637ceba55b5e20f049e0acf2376b22ef8e9c068e97cdf8490
```

### `dpkg` source package: `libxrender=1:0.9.10-1`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.10-1`
- `libxrender1:amd64=1:0.9.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.dsc' libxrender_0.9.10-1.dsc 2064 SHA512:3ef4856e738e1cc30ea8872845c88ea8f4918682137299a38c8ec33059c4ebd7ae8ec5ce6c658b9e287587356c696cef5dbae1eaaf9380b1b2448f459eab4c70
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA512:7768e62b500f468460f88f27bc1130170b204b478573d9e4406867e557b5638b7c1e21d88d51f9e774ce2344780a384e3c3be51421275d2ee880f9a978a3a232
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.diff.gz' libxrender_0.9.10-1.diff.gz 15399 SHA512:031cff19410477b6e3ff2e9b195ba46a5047fd2263ea19b7276b9fa347817e90c4ba93aa97ca71eb7318385b40d85994b1b04a3664ab1bc1982be8026853908f
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

### `dpkg` source package: `libzstd=1.4.5+dfsg-4`

Binary Packages:

- `libzstd1:amd64=1.4.5+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.5+dfsg-4
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg-4.dsc' libzstd_1.4.5+dfsg-4.dsc 2291 SHA512:2e0515b1b4870dccbb98c53d735467f7b24d106b4e031c5e707eb5b90de37450d441273e1812385de45cb4082cca0bc58586de53bb10167264f7475cdf3b5cb0
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg.orig.tar.xz' libzstd_1.4.5+dfsg.orig.tar.xz 1387864 SHA512:347f4b5ac24a75ffc510dc746b5fa26c5d71609ca5dcd4a9c5d4c43aa6f2df510d2e8d998d550e52e5b6f368277a8bf6fa82801a3581f79b866c6a340d0220a7
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg-4.debian.tar.xz' libzstd_1.4.5+dfsg-4.debian.tar.xz 12724 SHA512:5a9ca0b4d9bd16748365869d8530df01074956458b61c89cf298f1584b80e10ff91147ec903071f513b58f9ccfa2f6114a295233dbb1b31f116ce617e18fd267
```

### `dpkg` source package: `linux=5.8.0-19.20`

Binary Packages:

- `linux-libc-dev:amd64=5.8.0-19.20`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `lz4=1.9.2-2`

Binary Packages:

- `liblz4-1:amd64=1.9.2-2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.dsc' lz4_1.9.2-2.dsc 1956 SHA512:b94ed7d5978d633bfe98f365a51e917f73cc3c88b80ca35890d153f0faa521250d20aa26819aa386a019e1a9942ced9f82f869ef75a1bc1a12556a2a951699b7
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2.orig.tar.gz' lz4_1.9.2.orig.tar.gz 305796 SHA512:ae714c61ec8e33ed91359b63f2896cfa102d66b730dce112b74696ec5850e59d88bd5527173e01e354a70fbe8f036557a47c767ee0766bc5f9c257978116c3c1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.debian.tar.xz' lz4_1.9.2-2.debian.tar.xz 12712 SHA512:820d345e52dfef161e1f04fb395b9ec34196756b0af04919b471018e4e1736d21473009296052c65e7ed7142b9f7a922a47ac41848278a302e0d74eb1ab6dbe9
```

### `dpkg` source package: `lzo2=2.10-2`

Binary Packages:

- `liblzo2-2:amd64=2.10-2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.10-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2.dsc' lzo2_2.10-2.dsc 1926 SHA512:7a4ea3574fe62348da0174354986e29f2d2a6c67ca78dcdc24a92278fe2acf5c3bbd2ae36222ee471508b550aec42742245a4cc4cb9739a887320296d014007a
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10.orig.tar.gz' lzo2_2.10.orig.tar.gz 600622 SHA512:a3dae5e4a6b93b1f5bf7435e8ab114a9be57252e9efc5dd444947d7a2d031b0819f34bcaeb35f60b5629a01b1238d738735a64db8f672be9690d3c80094511a4
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.10-2.debian.tar.xz' lzo2_2.10-2.debian.tar.xz 6880 SHA512:06a16828ad19e447fc7d15cd49b911250ba4e82ce556b5d74d181bb24975bc19337c77d2f3502b4f31cd077fbad7d5df79d1ab73bc7be13ad24101d5101c85ae
```

### `dpkg` source package: `m4=1.4.18-4`

Binary Packages:

- `m4=1.4.18-4`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-4
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-4.dsc' m4_1.4.18-4.dsc 1638 SHA512:f124a8f68e9ae4ba59aaf0917660b55effd0bb5da2de122d2a3f730768317751122da9af2c7ca2e78d67b2be0b4cc348cf6835dcc8813053e7b02bd2d91329ee
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA512:06f583efc3855cd8477d8347544f4ae5153a3e50aea74d21968afa7214784ea3ddfc02d0a2b11324120d76a19f2e804d20de11a456b5da929eb6ae469519b174
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA512:effc857a19f1496d6dde2887c0314b37d4b142a435e77614936c730878c798491ad93b28860dddd2601f99a43fa41923729b961004faafc6f798f7bc1842f980
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-4.debian.tar.xz' m4_1.4.18-4.debian.tar.xz 17240 SHA512:52e5efe68d0b11faa8e82eff602da5708e079b8051fd85762b7dbd882c790f5c748e094b450033b19fcd090081a4d3dc4afce04edde8e2aecd3ae1be924fbbb2
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

### `dpkg` source package: `mercurial=5.5.1-1`

Binary Packages:

- `mercurial=5.5.1-1`
- `mercurial-common=5.5.1-1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=5.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.5.1-1.dsc' mercurial_5.5.1-1.dsc 2776 SHA512:32010896defac89cb375b20553122470fd641458ee63dd4a60f9aacec07968163e9fd3aa6196c6001ef85ad158d9f80a5bc23a3a94886a66c52cdaa35e30ca89
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.5.1.orig.tar.gz' mercurial_5.5.1.orig.tar.gz 7759341 SHA512:9cf02dd637154a5205d81eddf69681bd05405a29592c348c9d9cfa3b57ad3e678f98876fa6899d85d33a502b61f81e320262c7da394efb55fcca1d1219ca7cf5
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.5.1.orig.tar.gz.asc' mercurial_5.5.1.orig.tar.gz.asc 833 SHA512:641d310baf2b49a5c6fe746f4ea5eb347e85198fb3d1f0c408ed0e8ea5d091de9951d45b94b2ea00ec77624046df6bd79c891ef515b7fd7fbc245bfd979b8930
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.5.1-1.debian.tar.xz' mercurial_5.5.1-1.debian.tar.xz 63320 SHA512:d0466c9999be9e92cdf0a2d41add70221343044044dc2725963e87299029e9e87b6a080a610c0c286bbe7f7909d3ac9c1232a8aaa61902dc0c7b920b5a97cc6b
```

### `dpkg` source package: `mime-support=3.64ubuntu1`

Binary Packages:

- `mime-support=3.64ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.64ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.dsc' mime-support_3.64ubuntu1.dsc 1729 SHA512:f73a212b23f52534a823245961933fb20bf6266f69340cdd1dcb9f7671f20eb45486379b23f61625657ce7bb1e3aa4a3bfc27e5f7bc940600c0fabe3793106fa
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.tar.xz' mime-support_3.64ubuntu1.tar.xz 33980 SHA512:9369b3c7600ddda018518ebac9fb80bf87122ac0e39d755c86e66301e2b944240e57bb888472b6fa966b4dae5f8a9be966d161a8aef9a118b3b3de2749687c73
```

### `dpkg` source package: `mpclib3=1.2.0~rc1-1`

Binary Packages:

- `libmpc3:amd64=1.2.0~rc1-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.2.0~rc1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0~rc1-1.dsc' mpclib3_1.2.0~rc1-1.dsc 1879 SHA512:a09be2fa296327045427ad5fa2d16fd525bad0abb23ae7f3d4a8b115567bb980fa83d47365fc1a2bf3d7f71041d20f560334c24dd4446188e54f343828bc17c2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0~rc1.orig.tar.gz' mpclib3_1.2.0~rc1.orig.tar.gz 840338 SHA512:12d97751809832ce789a45eb27acc050ab23303faa9a4b43ec3e4b5ca9663b362ed213c18ee49961b199e2469dca5afefa5e2798f5d7d4f47c347e62a805f5f0
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.2.0~rc1-1.diff.gz' mpclib3_1.2.0~rc1-1.diff.gz 4264 SHA512:9c366f1b08e48503ba907a2a6c75316ce63c2b8446f75eab0d4d9d6b78be202ec8d4824c28a8c92a2bbc62ddb506b73bce7f51c1e6d321aec95209ad72af3363
```

### `dpkg` source package: `mpfr4=4.1.0-3`

Binary Packages:

- `libmpfr6:amd64=4.1.0-3`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.1.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3.dsc' mpfr4_4.1.0-3.dsc 1959 SHA512:ff99a80c7468e508efab5e4135e6fd54d7a50e55ccb168eda22a788ace44aae8b5bcf4091ed691b603ca96da0fb1af1f3e52411d61806e40d20b5923e5bd0bf4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0.orig.tar.xz' mpfr4_4.1.0.orig.tar.xz 1525476 SHA512:1bd1c349741a6529dfa53af4f0da8d49254b164ece8a46928cdb13a99460285622d57fe6f68cef19c6727b3f9daa25ddb3d7d65c201c8f387e421c7f7bee6273
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.1.0-3.debian.tar.xz' mpfr4_4.1.0-3.debian.tar.xz 12372 SHA512:a0472b95ab7d7c8a00d7716039fefbd30142939f2077a930f0dafc056a3a5b9debc65bb9ddbfb88fbfdb6bcf9fb7871631bdb7376ca24d400e11a4c1a371df3e
```

### `dpkg` source package: `mysql-8.0=8.0.21-1`

Binary Packages:

- `libmysqlclient-dev=8.0.21-1`
- `libmysqlclient21:amd64=8.0.21-1`

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
$ apt-get source -qq --print-uris mysql-8.0=8.0.21-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.21-1.dsc' mysql-8.0_8.0.21-1.dsc 3317 SHA512:5578e96ea5f4a0a398e2a311ddff0fe705aa1de69e4dc587d0663d85dc13fe42dfa9945668d2efa4b51408ce9bcdc2c867f5e8d2bd809c1f2264df0211a37f5f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.21.orig.tar.gz' mysql-8.0_8.0.21.orig.tar.gz 278292192 SHA512:18128edd7d9604ea69bd308f372d6663ef3629503969148e3a2117175c4ef625358b31b96e0e1b8d10a87037719e3cb61d5c71eee1e26ab0e0a1731977a2d7c1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.21-1.debian.tar.xz' mysql-8.0_8.0.21-1.debian.tar.xz 179564 SHA512:56b7ea775f52d9aa8ac042bd1964e5c29ad39210ffde52c45f702ab4fa37d2abe341e9a5f9d15b48d4dbad1acf93f6bd5418e7c6a68fdb3a2dd6e353133f3238
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

### `dpkg` source package: `ncurses=6.2-1`

Binary Packages:

- `libncurses-dev:amd64=6.2-1`
- `libncurses5-dev:amd64=6.2-1`
- `libncurses6:amd64=6.2-1`
- `libncursesw5-dev:amd64=6.2-1`
- `libncursesw6:amd64=6.2-1`
- `libtinfo6:amd64=6.2-1`
- `ncurses-base=6.2-1`
- `ncurses-bin=6.2-1`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw5-dev/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-1.dsc' ncurses_6.2-1.dsc 4016 SHA512:50bc5dbefc596e210720463826d9d5cb718cd77ccf481ac347149d62a87f6133cacd7d4e6c474acb4a815a716e406a15997b47f248b341e2be603d0c1ce6fc7f
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz' ncurses_6.2.orig.tar.gz 3425862 SHA512:4c1333dcc30e858e8a9525d4b9aefb60000cfc727bc4a1062bace06ffc4639ad9f6e54f6bdda0e3a0e5ea14de995f96b52b3327d9ec633608792c99a1e8d840d
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz.asc' ncurses_6.2.orig.tar.gz.asc 265 SHA512:b46c74b8f7f85ee9631451b2d903448abc506745a5e08c9592d3a323ebe020a7487372b635e810e2df639d07f87ff26c6c0ccee200bb963495838160d5137dd0
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-1.debian.tar.xz' ncurses_6.2-1.debian.tar.xz 51276 SHA512:7601abc7989ac947645f13096e0c6655e81303c8826ae855b9203e1c1dc33a3930b72f31f56c6751aaa2fb45f87aadd57b26361021c2754d93451158f0e17809
```

### `dpkg` source package: `netbase=6.1`

Binary Packages:

- `netbase=6.1`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.dsc' netbase_6.1.dsc 1480 SHA512:6a650cd9c35be4fb9ea86da7f2228702c4d9b6936381f9707741c8dcb9821e2e0125290335edff163bdbc996fa74f146083f01e184162c9d4133f827f10ce563
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.tar.xz' netbase_6.1.tar.xz 31984 SHA512:9252840573dc9e976434c15504f023e25b0fa25a6b2a133a25a064d5a77be3232007d78fd60bd99e2721f929dbd2035c315e47155b51a97c6070514c3061329e
```

### `dpkg` source package: `nettle=3.6-2`

Binary Packages:

- `libhogweed6:amd64=3.6-2`
- `libnettle8:amd64=3.6-2`

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
$ apt-get source -qq --print-uris nettle=3.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6-2.dsc' nettle_3.6-2.dsc 2254 SHA512:1b5f93a849d74d97c8d211444c50a333f4592c0c54a1348e5adab3b9392c20fbc454c9f4f3f831ee946f83310d10bd649de3b5f8797ba76eed709fd8d699f4b4
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6.orig.tar.gz' nettle_3.6.orig.tar.gz 2288173 SHA512:2471af875e51327af61af8bda53cd9c3adc27b6e32592a4b5b10b3ec60999ebf771ab9c54c747b0bade4b3b5a717e77fdbdb53699dd9e8a9ed4eee07f46aed51
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6.orig.tar.gz.asc' nettle_3.6.orig.tar.gz.asc 573 SHA512:006c821e599d8fb64b3e5b71182909c5e5921b35e5223f749b69a2c5507b41220595c3c2fa46a484ae1254b8eb4f4c7bfccfd808a03ca79e9c1fd7cbb8ed7216
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.6-2.debian.tar.xz' nettle_3.6-2.debian.tar.xz 21136 SHA512:00aa9109859953aa0dd25c5f68661174acff20271d7f5f2991edbb2f997acfffc927c772e298486d6f438d4402d8e79c64fef6864ecad3c464600771e34b8436
```

### `dpkg` source package: `nghttp2=1.41.0-3`

Binary Packages:

- `libnghttp2-14:amd64=1.41.0-3`

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
$ apt-get source -qq --print-uris nghttp2=1.41.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0-3.dsc' nghttp2_1.41.0-3.dsc 2548 SHA512:4726645f750316afedba7b41d10cc461d7f0f337f570832cbd18371ddd378dfd8fbfd4b9cba19de244953d479744fd4437727e031228f55b62dcd98a712e0978
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0.orig.tar.bz2' nghttp2_1.41.0.orig.tar.bz2 1943304 SHA512:61de1bbbe91230ebe9f7a3ef4d3874391f8180d93c8ff1e94a58035e4061d2f9057e5ba2b90f6fe86f6aefc7244795385d176a862019c47a3aad974b60caa143
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0-3.debian.tar.xz' nghttp2_1.41.0-3.debian.tar.xz 13688 SHA512:9fdd1658e13415daa7f4d5ee34fbb58265a75b02fc026b5430761657afe0b03cd4778b6e7e52f60a2eeb09563cdbec52b8047d7ced3cb0110d2cc6e6b6d06a2b
```

### `dpkg` source package: `npth=1.6-2`

Binary Packages:

- `libnpth0:amd64=1.6-2`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-2.dsc' npth_1.6-2.dsc 1931 SHA512:66338b3c6effe08952395aa4f00c8a5b4136cce23043c5e9d828798bee7cb0a57aa282f383eb3d98480ac8addeab3607b76c414b4db05cc62fb98c08c076aef6
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA512:2ed1012e14a9d10665420b9a23628be7e206fd9348111ec751349b93557ee69f1176bcf7e6b195b35b1c44a5e0e81ee33b713f03d79a33d1ecd9037035afeda2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-2.debian.tar.xz' npth_1.6-2.debian.tar.xz 10612 SHA512:b76317daa87dcbfe2f5d294b8b350cb210b780192fe15618172679caaa235f90969814b66fcc43838c2df43a77317bba0dcd29c0aaf72a603dcb1d26fbbf52d1
```

### `dpkg` source package: `openexr=2.3.0-6ubuntu3`

Binary Packages:

- `libopenexr-dev=2.3.0-6ubuntu3`
- `libopenexr24:amd64=2.3.0-6ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr24/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `openexr`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `openjpeg2=2.3.1-1ubuntu4`

Binary Packages:

- `libopenjp2-7:amd64=2.3.1-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libopenjp2-7/copyright`)

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
$ apt-get source -qq --print-uris openjpeg2=2.3.1-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu4.dsc' openjpeg2_2.3.1-1ubuntu4.dsc 2842 SHA512:301f7f7748089ba467fd8abfc4a5cfd3129db9a72f278c7a08f517d604402594309bc286ca9cd134ec61427dd0d06e83dd7434fb4454e9bf6a5c27f7ce77e6c5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1.orig.tar.xz' openjpeg2_2.3.1.orig.tar.xz 1381768 SHA512:1346fae5f554102c46ad26e59888c693bf57b3ffaccfb5040b6c177f2ca510dd0915966d6bfd252b4293c0c098290c8e6cd923c265ca288e95e1fb7522b66b32
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjpeg2/openjpeg2_2.3.1-1ubuntu4.debian.tar.xz' openjpeg2_2.3.1-1ubuntu4.debian.tar.xz 21052 SHA512:474ce3c982b7e54aa65497f4899b8464a18436f2c2177b36e7eaf097cb405a11b99ec871a267744d22e662fc18caa4708eb150970076a2ac0b05f2e2dbe68b57
```

### `dpkg` source package: `openldap=2.4.53+dfsg-1ubuntu1`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.53+dfsg-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.53+dfsg-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.53+dfsg-1ubuntu1.dsc' openldap_2.4.53+dfsg-1ubuntu1.dsc 3154 SHA512:de28fd7c565284166b9ea00a247c49702059a8db02e0af5b085508ca796af5268be3e62fa8214f45eaf85fbb08715e28849c26d6f36af5e65041a8315e4c7772
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.53+dfsg.orig.tar.gz' openldap_2.4.53+dfsg.orig.tar.gz 5013515 SHA512:06cf88fe390cb04592407a0767e5051d4e6a8878f30386a0837710a406b037fde09953185ce395c189d69378114a6330ba54c7097d43322d6a3152d1a5b12de4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.53+dfsg-1ubuntu1.debian.tar.xz' openldap_2.4.53+dfsg-1ubuntu1.debian.tar.xz 181644 SHA512:2e3391eef159ac71cb5e1e0febe6bb6b2353c75fe024895d8e8a1e14763089cd6a3c485d418c34a465aff5cffcb47a5b6d87d4ad1a634a044b18cfd8e6fdb8a6
```

### `dpkg` source package: `openssh=1:8.3p1-1`

Binary Packages:

- `openssh-client=1:8.3p1-1`

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
$ apt-get source -qq --print-uris openssh=1:8.3p1-1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1-1.dsc' openssh_8.3p1-1.dsc 3342 SHA512:98f47b52110af25aff0ea690b1536961d9800cb0f131e7bf9e305d2ca999a85a040588abc83bf1acd11bcf16dcc8c88d77fcc151737833f2df854cf56bc47be4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1.orig.tar.gz' openssh_8.3p1.orig.tar.gz 1706358 SHA512:b5232f7c85bf59ae2ff9d17b030117012e257e3b8c0d5ac60bb139a85b1fbf298b40f2e04203a2e13ca7273053ed668b9dedd54d3a67a7cb8e8e58c0228c5f40
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1.orig.tar.gz.asc' openssh_8.3p1.orig.tar.gz.asc 683 SHA512:569fa12b3671af15bd7cd54fc7b13d1d64f3e96eb28f6dc430082f7bec4595689c633d3d56c23faad45b73e4da666c3ec090de26bf54f49410ba9bb8b5363e75
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1-1.debian.tar.xz' openssh_8.3p1-1.debian.tar.xz 176252 SHA512:2e984027a3d68259d517fe91c056ac0b1016703f55a01dee5a7a20ecf13b9177ef6192521cf4e1aff183cae4b40c1a056f06aec5213f6238cd9a543bb3283e7d
```

### `dpkg` source package: `openssl=1.1.1f-1ubuntu4`

Binary Packages:

- `libssl-dev:amd64=1.1.1f-1ubuntu4`
- `libssl1.1:amd64=1.1.1f-1ubuntu4`
- `openssl=1.1.1f-1ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1f-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu4.dsc' openssl_1.1.1f-1ubuntu4.dsc 2705 SHA512:b0c4209047983a2a629751d1ad7cb3b9d2cfb040ed02eb964775a33a0588c5d9adc4db5a19554dc00c1f5e6496572018cbcc6abf39777cbeb4b3f73fc6becc87
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz' openssl_1.1.1f.orig.tar.gz 9792828 SHA512:b00bd9b5ad5298fbceeec6bb19c1ab0c106ca5cfb31178497c58bf7e0e0cf30fcc19c20f84e23af31cc126bf2447d3e4f8461db97bafa7bd78f69561932f000c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz.asc' openssl_1.1.1f.orig.tar.gz.asc 488 SHA512:63b01ffc23b2fec2cfc147d382b486a136e5610e181be94aa333022803a442ded37e8276fefb62b3176b571b94a1d2243c05b86b52ad7784fe0068d1ad948562
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu4.debian.tar.xz' openssl_1.1.1f-1ubuntu4.debian.tar.xz 149616 SHA512:0afc642ee3c0a36afa45c9f4c5f9288ffd6767bae6089a2a4cc199ea8d05c72590fb75409a2e9203e1a4c5691f8d6760236af0085322a2d8c4344e3e1f4b3ef6
```

### `dpkg` source package: `p11-kit=0.23.21-2build1`

Binary Packages:

- `libp11-kit0:amd64=0.23.21-2build1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.21-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.21-2build1.dsc' p11-kit_0.23.21-2build1.dsc 2557 SHA512:0c19b974d43b28c892262a99c9dce7b625e7caa43cd0d21b43591a6b469435e2c259d130fd6775e7e2a6b425f4ce88e458193d61f2c87c480ed71f572f4285f5
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.21.orig.tar.xz' p11-kit_0.23.21.orig.tar.xz 827064 SHA512:4c796ca2c72a650f105a7a70aa62e55edb12e1c151e91ef92bfeee6c5c68982b36023400b42c4efcb1d351b7848e8618c26607cdb0f77b48ae40e2ecfd713e3e
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.21.orig.tar.xz.asc' p11-kit_0.23.21.orig.tar.xz.asc 854 SHA512:8bf48da323fe9c6161673c49870852d34fede5beb6a624ce73090599d3729633153f03dc06aa77478174b1e4e4840c3fe74cd84219747446e2fa29f2a895cfa5
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.21-2build1.debian.tar.xz' p11-kit_0.23.21-2build1.debian.tar.xz 22788 SHA512:88a6885d6a83c3e7f8ed18148c18603b14ee567b9020e324f9873f4e73ffa75b682ce6138566265abfce134d15fba14200069e21127ff0849fa6bf7392ad3e29
```

### `dpkg` source package: `pam=1.3.1-5ubuntu6`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu6`
- `libpam-modules-bin=1.3.1-5ubuntu6`
- `libpam-runtime=1.3.1-5ubuntu6`
- `libpam0g:amd64=1.3.1-5ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu6.dsc' pam_1.3.1-5ubuntu6.dsc 2699 SHA512:436e65b46b14cb02b6d13255143f8a06064a52c3a3fa8dae7a2305f1e7a3017db19389693c0150a9a4aacc40ad3664318178ebdafd081b1057fd083920391a34
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA512:6bc8e2a5b64686f0a23846221c5228c88418ba485b17c53b3a12f91262b5bb73566d6b6a5daa1f63bbae54310aee918b987e44a72ce809b4e7c668f0fadfe08e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu6.debian.tar.xz' pam_1.3.1-5ubuntu6.debian.tar.xz 160300 SHA512:c3e8d10c1d799a8b34d29d584d34813191f7dab1124ae9824d6df5e3eea49fb76b4647b30ecaad69bc06031eb02b0cbc8612673e85944690ea7f88b874ac369c
```

### `dpkg` source package: `pango1.0=1.46.1-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.46.1-1`
- `libpangocairo-1.0-0:amd64=1.46.1-1`
- `libpangoft2-1.0-0:amd64=1.46.1-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Chromium-BSD-style`
- `Example`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `TCL`
- `Unicode`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/pango1.0/1.46.1-1/


### `dpkg` source package: `patch=2.7.6-6`

Binary Packages:

- `patch=2.7.6-6`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-6
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-6.dsc' patch_2.7.6-6.dsc 1699 SHA512:1635fd11e2f69456140596ced8cc2e23a441f92f59af39cb758e188c4093779dbf00a8f6dcd399b9007fd8ca6253354dc0bfa562a2f1142a82cc92455e006f9e
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA512:fcca87bdb67a88685a8a25597f9e015f5e60197b9a269fa350ae35a7991ed8da553939b4bbc7f7d3cfd863c67142af403b04165633acbce4339056a905e87fbd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-6.debian.tar.xz' patch_2.7.6-6.debian.tar.xz 14464 SHA512:b51c4361d71edde86e188d7511f66dc662afaaa5bc6c76c7bf1a99d0abef3d0de2db586d09b8d55b67cd8a0c3a8029570953e996fc639c1e8f926e24dc36bbb5
```

### `dpkg` source package: `patiencediff=0.1.0-2build2`

Binary Packages:

- `python3-patiencediff=0.1.0-2build2`

Licenses: (parsed from: `/usr/share/doc/python3-patiencediff/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris patiencediff=0.1.0-2build2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/patiencediff/patiencediff_0.1.0-2build2.dsc' patiencediff_0.1.0-2build2.dsc 2198 SHA512:28e3e419f8ee11af20168e8263ed308687c1c97e9b048bc58565853b93df63879925f110e3e6030e9b6fb0719d7fe32363e40d9fa4334d96f49507840a95b0cd
'http://archive.ubuntu.com/ubuntu/pool/universe/p/patiencediff/patiencediff_0.1.0.orig.tar.gz' patiencediff_0.1.0.orig.tar.gz 19965 SHA512:a66dd6dad89b7eb0d34115cb6da47280d8c1dcab2d5bc7ca9d3c08d51bf1644066822200664dd96213258181e9279932c8400839902286ce7217c97a188012f8
'http://archive.ubuntu.com/ubuntu/pool/universe/p/patiencediff/patiencediff_0.1.0-2build2.debian.tar.xz' patiencediff_0.1.0-2build2.debian.tar.xz 42868 SHA512:fe0040459ad4a4a6057203c47acb6ea57451a04cd77d86442672fa26cc7d97c2c96607d95813727f8fcbdebccdd22c5adc8a3d6cf0fa08a0297e7fae5c492341
```

### `dpkg` source package: `pcre2=10.34-7`

Binary Packages:

- `libpcre2-16-0:amd64=10.34-7`
- `libpcre2-32-0:amd64=10.34-7`
- `libpcre2-8-0:amd64=10.34-7`
- `libpcre2-dev:amd64=10.34-7`
- `libpcre2-posix2:amd64=10.34-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.34-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.dsc' pcre2_10.34-7.dsc 2286 SHA512:c9830f64827dceb42b7bdaba73069367d07dfc9a1f978cc85c563a799abaa2a5484730be6c89dbee84a4ea5e769fb7cd9bfcd2b71bcd81cb58da1f9fa1dc9379
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34.orig.tar.gz' pcre2_10.34.orig.tar.gz 2271533 SHA512:820b3805fc7fcf3a80dfd42ff570efc8518fe3c50f3feb720319b95316619e5b8f6601b3c9522606315aecd5558ccfc8a04a89fab9921fdfc3400dc2caf17c22
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.diff.gz' pcre2_10.34-7.diff.gz 7068 SHA512:12d6ef86a0e80928a1da98f9fb00ee8b272232ab74e6aade51d76a007ebca310e1d15a1a5058c40932ae25062655e60aa51e37123944af9f852bbd8c7e7c54e6
```

### `dpkg` source package: `pcre3=2:8.39-13`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-13`
- `libpcre3:amd64=2:8.39-13`
- `libpcre3-dev:amd64=2:8.39-13`
- `libpcre32-3:amd64=2:8.39-13`
- `libpcrecpp0v5:amd64=2:8.39-13`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-13
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.dsc' pcre3_8.39-13.dsc 2226 SHA512:5a12d0001341c4bdda5b087ef418d5f4e2ab5d27d3fb117319fce82e86ffe0167e2bf1e8afee1fb71fb479fc697fd1243ead3d89519a628a84ede2f99bf79cd0
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA512:8b0f14ae5947c4b2d74876a795b04e532fd71c2479a64dbe0ed817e7c7894ea3cae533413de8c17322d305cb7f4e275d72b43e4e828eaca77dc4bcaf04529cf6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.debian.tar.gz' pcre3_8.39-13.debian.tar.gz 27002 SHA512:1dda1a982ecf1cf888e4f716101e84d99f427cd46874ab4d4116b0bda0852ef5cb7f57cec0edc7cab24c5095431694787dc052dab771621449f7c9d8c2367b86
```

### `dpkg` source package: `perl=5.30.3-4`

Binary Packages:

- `libperl5.30:amd64=5.30.3-4`
- `perl=5.30.3-4`
- `perl-base=5.30.3-4`
- `perl-modules-5.30=5.30.3-4`

Licenses: (parsed from: `/usr/share/doc/libperl5.30/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.30/copyright`)

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
$ apt-get source -qq --print-uris perl=5.30.3-4
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3-4.dsc' perl_5.30.3-4.dsc 2983 SHA512:d29a64f19026ed8be20d2c11a82dac5e827c9807b5904bdeabd65e39c523d643ece92821fc3d55033dd5689f4644754cc10e1ee5c1c56d12923c3df1d01fb1e8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3.orig-regen-configure.tar.gz' perl_5.30.3.orig-regen-configure.tar.gz 870970 SHA512:947dee318e03fb1a03d3e6c0754a4aae5677616451c05cf411ab76a9b729589db02a28883bb153a325ba02b38f20a6aec11a65308e2ac101f0d86da9482e0ad8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3.orig.tar.xz' perl_5.30.3.orig.tar.xz 12375128 SHA512:0ea62cf17532ee99217a218c39aa530472857c7a1982494f3a01693683062b4cdebe383a79f7b64452c713337b554ed5e0fd6eda018ea29e83c3538a13c24f3c
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3-4.debian.tar.xz' perl_5.30.3-4.debian.tar.xz 171184 SHA512:3b5b5059300b8ae9c36a6eb79bb0692393ad33c755575ab82937b87e1bc7742983e7f89a1c40c3de8cd369056e46f25c92b41352cf7458ccd25fc9bdee93bf95
```

### `dpkg` source package: `pinentry=1.1.0-4build1`

Binary Packages:

- `pinentry-curses=1.1.0-4build1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.dsc' pinentry_1.1.0-4build1.dsc 2595 SHA512:c2aefb05c736ee9cf779e641a0a0a20810fccb8e6e8c88f7d13a08b3e8cfa7f4246d9c70ecc6a907bdda143366b058e866a8f78124ef259ae4dc7963a542f389
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA512:5012672925bcb5f683358c259e55e4b87c67cf063ad52c759308933733025c33f7ce08e5b8019ffc101cbf7ef30499040ef2fd34a7611698e65e1593f80948cd
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.debian.tar.xz' pinentry_1.1.0-4build1.debian.tar.xz 17312 SHA512:6288a034c9c08e4a164c5e2d9c66142638a0da6947031e0199811272e004c107209bb0feb0048ae685176ba3a4d3a98e7520edb16d633721a474810897b8f18d
```

### `dpkg` source package: `pixman=0.38.4-0ubuntu1`

Binary Packages:

- `libpixman-1-0:amd64=0.38.4-0ubuntu1`
- `libpixman-1-dev:amd64=0.38.4-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.38.4-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.38.4-0ubuntu1.dsc' pixman_0.38.4-0ubuntu1.dsc 1468 SHA512:4538b0c8be6d83d6fea6c1f328ce923ac293872c65a247d2eb4eccfebeef5c12f2ad8569adaa58993cfe263a9c9d814a3adb9c9e1630e28af9b8a218bded050a
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.38.4.orig.tar.gz' pixman_0.38.4.orig.tar.gz 897926 SHA512:b66dc23c0bc7327cb90085cbc14ccf96ad58001a927f23af24e0258ca13f32d4255535862f1efcf00e9e723410aa9f51edf26fb01c8cde49379d1225acf7b5af
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.38.4-0ubuntu1.diff.gz' pixman_0.38.4-0ubuntu1.diff.gz 322901 SHA512:c192983c9eeb70d7f3463cf72c3970631477795a5dbf05e2d66de1203b9f6fdcba90452afa147ff00073c3173c49b3506128d3d0b192e9721acf54a05de22050
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

### `dpkg` source package: `postgresql-12=12.4-1`

Binary Packages:

- `libpq-dev=12.4-1`
- `libpq5:amd64=12.4-1`

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
$ apt-get source -qq --print-uris postgresql-12=12.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.4-1.dsc' postgresql-12_12.4-1.dsc 3627 SHA512:b115e52a8f433b840265dffd311291d9c4c169484d81d786644bf7cfa69e12a8a18f3dcfac71ff83e536ea88d915aab87d67c0a7324e24cf65fbf97b7a1d34e5
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.4.orig.tar.bz2' postgresql-12_12.4.orig.tar.bz2 20669776 SHA512:36daf10878ca153370829178786dd6ee366ab4d4d6dc9c527536740fdb14b688ae4c33f850eb4243a7667d23f87e4bfd1ddee0755447ad4f3996e423e391c2f3
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-12/postgresql-12_12.4-1.debian.tar.xz' postgresql-12_12.4-1.debian.tar.xz 23736 SHA512:e53b2af1b8f904efcc28c6723d9752f97079959fb2306f01d777af02ed105967c4b3c89dfa6069daae37830ce77e2db3271bd3c5b75fb85bda76a9b52e2394c3
```

### `dpkg` source package: `procps=2:3.3.16-5ubuntu1`

Binary Packages:

- `libprocps8:amd64=2:3.3.16-5ubuntu1`
- `procps=2:3.3.16-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python-certifi=2020.4.5.1-1`

Binary Packages:

- `python3-certifi=2020.4.5.1-1`

Licenses: (parsed from: `/usr/share/doc/python3-certifi/copyright`)

- `GPL-2`
- `MPL-2`

Source:

```console
$ apt-get source -qq --print-uris python-certifi=2020.4.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1-1.dsc' python-certifi_2020.4.5.1-1.dsc 1634 SHA512:ce68bf2337c2b2f86140062c572baf17821438cfa3a34787eb00e32b1b9773154fb36c73bd0e9123e5b55b88942ad851ffebbbc21e34551ef04ac0630fd09aa9
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1.orig.tar.xz' python-certifi_2020.4.5.1.orig.tar.xz 144464 SHA512:b6975b1ca8bcc9296997692a28f1f995a3b5257cd8e7d1c85eb25bcdbd07e2fe8ddfabf7f46dc2ba2aaa5c833dc413eb0ef3e067c4688f648b356f9c993c6e81
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1-1.debian.tar.xz' python-certifi_2020.4.5.1-1.debian.tar.xz 7732 SHA512:8466d88da785ab9214bf2e343f81a61807d5969120e8bbf9a1b3fa117954d36c3391b17d97a0e68f5ec9b31f84588cdfe7622ca70d8d2f8afa15da29f9091e28
```

### `dpkg` source package: `python-fastimport=0.9.8-5build1`

Binary Packages:

- `python3-fastimport=0.9.8-5build1`

Licenses: (parsed from: `/usr/share/doc/python3-fastimport/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris python-fastimport=0.9.8-5build1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8-5build1.dsc' python-fastimport_0.9.8-5build1.dsc 2244 SHA512:16cb046c4ee6d463f6859bf148413ad2bd009633dd0de95927b6fdcdb48f0b414cc01533ba1f8b3e125beb452bf3b551adcd5b69c8ad7e9abceb280c285fe04b
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8.orig.tar.gz' python-fastimport_0.9.8.orig.tar.gz 39512 SHA512:5d195b641cf6138fdbc6c75781a4a6d3699e3ada9743bbe4c4264879b2da2f8a2e995e7cc3955a5241e9c7a7f24f8114474a0a30907f86e2e335e2be4669f588
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8-5build1.debian.tar.xz' python-fastimport_0.9.8-5build1.debian.tar.xz 13644 SHA512:7075b69e19972a6ca9414cdd4175441ee5baee14495e9357bbce0853efc55b2c7728240335bb68b3a6d25226c888b5b87db5515ef4ef315a11471bd99ead7eaa
```

### `dpkg` source package: `python-urllib3=1.25.9-1`

Binary Packages:

- `python3-urllib3=1.25.9-1`

Licenses: (parsed from: `/usr/share/doc/python3-urllib3/copyright`)

- `Expat`
- `PSF-2`

Source:

```console
$ apt-get source -qq --print-uris python-urllib3=1.25.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9-1.dsc' python-urllib3_1.25.9-1.dsc 2217 SHA512:a6abb8fb7aa46a35611738fe004874f692ba8b86ba65a9a93c99124bf911425e3229c3ed7458fa4b8b9a232fac384c9d850cdd79c2fdd3e83020fecf735d788d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9.orig.tar.gz' python-urllib3_1.25.9.orig.tar.gz 254921 SHA512:505f1d9137e469a48ee0de417f2be36946cf1d9bbcf1233280be399a6c6d8650b5b3c6cfcf884b04e0156974da703f48843381b9aab377738a2e60f7d2d3799b
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9-1.debian.tar.xz' python-urllib3_1.25.9-1.debian.tar.xz 11472 SHA512:043315b917ef30bbf646fde7bd83f8da955e32c98dc3d370d24a9f73a11dc9aa528c0b7f9df9a2c228e33c2483b06059a81ddd45678312a69f118b1b4a75ff70
```

### `dpkg` source package: `python3-defaults=3.8.2-0ubuntu2`

Binary Packages:

- `libpython3-stdlib:amd64=3.8.2-0ubuntu2`
- `python3=3.8.2-0ubuntu2`
- `python3-minimal=3.8.2-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python3-stdlib-extensions=3.8.5-1`

Binary Packages:

- `python3-distutils=3.8.5-1`
- `python3-lib2to3=3.8.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/python3-stdlib-extensions/3.8.5-1/


### `dpkg` source package: `python3.8=3.8.6~rc1-2`

Binary Packages:

- `libpython3.8-minimal:amd64=3.8.6~rc1-2`
- `libpython3.8-stdlib:amd64=3.8.6~rc1-2`
- `python3.8=3.8.6~rc1-2`
- `python3.8-minimal=3.8.6~rc1-2`

Licenses: (parsed from: `/usr/share/doc/libpython3.8-minimal/copyright`, `/usr/share/doc/libpython3.8-stdlib/copyright`, `/usr/share/doc/python3.8/copyright`, `/usr/share/doc/python3.8-minimal/copyright`)

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

- http://snapshot.debian.org/package/python3.8/3.8.6~rc1-2/


### `dpkg` source package: `readline=8.0-4`

Binary Packages:

- `libreadline-dev:amd64=8.0-4`
- `libreadline8:amd64=8.0-4`
- `readline-common=8.0-4`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.dsc' readline_8.0-4.dsc 2434 SHA512:27ed5ba327ddf5ba20376ffba0e5784abd7fcbe66dc8b794bdabad07b0440352e556dc8fc7a08258e8142a8c94d6b2a950049adb8f64d13d695bec6bf5991465
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0.orig.tar.gz' readline_8.0.orig.tar.gz 2975937 SHA512:41759d27bc3a258fefd7f4ff3277fa6ab9c21abb7b160e1a75aa8eba547bd90b288514e76264bd94fb0172da8a4faa54aab2c07b68a0356918ecf7f1969e866f
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.debian.tar.xz' readline_8.0-4.debian.tar.xz 30408 SHA512:f2a21484b637fff8c440f57406e2b2215ea0e59d2d0e3abadcf22af61118a2ba9241ac866fa2ffbd99fe80878976960d705e99feabced28856b0d3ebf16c6ffc
```

### `dpkg` source package: `rpcsvc-proto=1.4.2-0ubuntu3`

Binary Packages:

- `rpcsvc-proto=1.4.2-0ubuntu3`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `sed=4.7-1build1`

Binary Packages:

- `sed=4.7-1build1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `sensible-utils=0.0.13`

Binary Packages:

- `sensible-utils=0.0.13`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.13
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.13.dsc' sensible-utils_0.0.13.dsc 1688 SHA512:1e0e27d2505cfa185398763723f557af400ab34c565cecf64860ba929f53b23b608aa99e427d9f82463fdeae66e6aabc96dffe31f9d2863b3486cfaf46151012
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.13.tar.xz' sensible-utils_0.0.13.tar.xz 62020 SHA512:365406e73e129b80a0abc7e2d32623df23c2eeeb9bf2d597c3c09bdb990b816734acc06225e53b0c4a9a64c0e7d40d434c9a3abead57fd87e180c5a4be62ab8d
```

### `dpkg` source package: `serf=1.3.9-8build1`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-8build1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `shadow=1:4.8.1-1ubuntu6`

Binary Packages:

- `login=1:4.8.1-1ubuntu6`
- `passwd=1:4.8.1-1ubuntu6`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu6.dsc' shadow_4.8.1-1ubuntu6.dsc 1705 SHA512:e2dc5b1cb37ea5cd930e1f3f6ee5449a33c621835ca3b2c948e2c89ab06790781dc3a57feaf29a41ddd02c1ffc93246fd1b7b0a7c76524c4bbb0ada7750f615d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA512:780a983483d847ed3c91c82064a0fa902b6f4185225978241bc3bc03fcc3aa143975b46aee43151c6ba43efcfdb1819516b76ba7ad3d1d3c34fcc38ea42e917b
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu6.debian.tar.xz' shadow_4.8.1-1ubuntu6.debian.tar.xz 85620 SHA512:a2bd0a0845a860dfbb5fceafa3f7a8cb088960271889e0681e0a15c4bd1c12aacf7388507db96a3320e5303c22e120c1f3c00bf3c9e0ebab41b32528b58a2e22
```

### `dpkg` source package: `shared-mime-info=1.15-1`

Binary Packages:

- `shared-mime-info=1.15-1`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.15-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15-1.dsc' shared-mime-info_1.15-1.dsc 2198 SHA512:7c953cce2037c345330b1147e3cd6595cd4261bb32b1b09022b8d88cd19d7a81a4c24e306806c4bb6277c74ae3c7cbd8add94451722754a1801806024f3f9fca
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15.orig.tar.xz' shared-mime-info_1.15.orig.tar.xz 772708 SHA512:3666aa500dfa6a28bd0524400c47fa16d90ae61f8c80f350fd895972319ec2f511618b8a7fa3cbde621edee46fde19e4506bda62f0bd2d0ede1b08d7bdb9aef2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.15-1.debian.tar.xz' shared-mime-info_1.15-1.debian.tar.xz 9728 SHA512:9134c60839a02c8f3088868d615b62393a44c55aa52ddcfbf8caf53d735c717caba805e1c0582f786761d946291b5698cecefefab384b422b6f1ae578b766b47
```

### `dpkg` source package: `six=1.15.0-1`

Binary Packages:

- `python3-six=1.15.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.15.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0-1.dsc' six_1.15.0-1.dsc 2411 SHA512:a8e92b7f408e6b16bc5d4de35d7452d79dba8d99f62698ad3db9b627aa8c732fa7ce2b654b685056abf0927b977d625f736e4504ea8ad44da7f39623e135cd32
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0.orig.tar.gz' six_1.15.0.orig.tar.gz 33917 SHA512:eb840ac17f433f1fc4af56de75cfbfe0b54e6a737bb23c453bf09a4a13d768d153e46064880dc763f4c5cc2785b78ea6d3d3b4a41fed181cb9064837e3f699a9
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0-1.debian.tar.xz' six_1.15.0-1.debian.tar.xz 4480 SHA512:b728ef6b679d69867e1be38d16b71748a2ce8be61734a44feacebc13cfe4055b64cbd2417036d68ec17e0bb1a94eff4d442c8440cf23660bfa9274d622c49a25
```

### `dpkg` source package: `sqlite3=3.33.0-1`

Binary Packages:

- `libsqlite3-0:amd64=3.33.0-1`
- `libsqlite3-dev:amd64=3.33.0-1`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.33.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.33.0-1.dsc' sqlite3_3.33.0-1.dsc 2410 SHA512:46ed945f090ad7b1aaa23c81631f3462d413da9022097fb5fd1ab77b0acc614779b4443b6e4e67fdd37b786a7acda29ff560f591519565900f307528a822cec2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.33.0.orig-www.tar.xz' sqlite3_3.33.0.orig-www.tar.xz 5890732 SHA512:f525229aaf62f30dda07e5f290deca5b0e259b421f7a2bc5739398fa3def9119dc88c2a79eab3e40e3568f2c0ebdee5e45222a724a26c7900c4cfb6359083c19
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.33.0.orig.tar.xz' sqlite3_3.33.0.orig.tar.xz 7319228 SHA512:f5e7fed2d3bb942d39e154fe213faccc9ad2a9edfd3752ac9e49945f52ee8fd57481d618375f9fa4d60392149a17fbbe1c8a5d54652041e33cd55e1b3267b8bc
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.33.0-1.debian.tar.xz' sqlite3_3.33.0-1.debian.tar.xz 21852 SHA512:4915d46f8d38eea98a3a2e956d8bd8680388daa1ed310c2164dadec411608e0e82b13d8deb7311c820e9d980bada88fe7be5d2e2e74ba111f6ff9426e7deddb3
```

### `dpkg` source package: `subversion=1.14.0-2`

Binary Packages:

- `libsvn1:amd64=1.14.0-2`
- `subversion=1.14.0-2`

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
$ apt-get source -qq --print-uris subversion=1.14.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0-2.dsc' subversion_1.14.0-2.dsc 3807 SHA512:efe732d1de08c51a5cccb9fdce436f2978c556823f81acb70f68ea8c9e0ea72cb6879c6bf42a787498818ce050b5ee45ddbcc696b539e3158ee061ed55b4b663
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0.orig.tar.gz' subversion_1.14.0.orig.tar.gz 11519871 SHA512:758d18bc39d6247fc949c11c786fff39484dd498db1cc172d38b37c28d536e6ba1f956660e98d2e365495b2abd07aa6ee76460c71f32edc6d54d1ccf463f0176
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0.orig.tar.gz.asc' subversion_1.14.0.orig.tar.gz.asc 3917 SHA512:6010a0b41c90a07a3a8d5a0e545bb3bf8675558a52e5aba331d02795b6311f967fb63fde6167936c7d158ec0b4ec53fa99ccf987af8f1270fa5c90a1938a448b
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0-2.debian.tar.xz' subversion_1.14.0-2.debian.tar.xz 427376 SHA512:13d9285f4a49aa1a23caf3ae3742d27e901f2d61fe385833cbdd25d92a7e6fac94bb347b7980d62a33c70745755f83a9f46202780645c4702acca1e2b409aff7
```

### `dpkg` source package: `systemd=246.4-1ubuntu1`

Binary Packages:

- `libsystemd0:amd64=246.4-1ubuntu1`
- `libudev1:amd64=246.4-1ubuntu1`

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


### `dpkg` source package: `sysvinit=2.96-3ubuntu1`

Binary Packages:

- `sysvinit-utils=2.96-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-3ubuntu1.dsc' sysvinit_2.96-3ubuntu1.dsc 2781 SHA512:fb9dc5aadea57e71cce3409fa27f9768b575374fd798577b4e3d17b909a72283a3445181a1e96e7cdef54d0f76bd6bf03b4bb4c30e943411deece183c9a90f9b
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA512:1388398568ebfe53460796f8ab75a3ead6111612888ea36e8f1c0db4d41ef6f45fc217abb7804519ff1143a78d97c95b24e42c8c22c95a47b9436484bfb6f45d
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA512:2b3798e8fc8531cd1a2b2a523159b7f064bfadd8815b930fb70d5a1380775f1b5bac5627d5cd9d95b03ff3737d8d6b2f357c6bc21ac2e21ee089b67f98b4eb6a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-3ubuntu1.debian.tar.xz' sysvinit_2.96-3ubuntu1.debian.tar.xz 128020 SHA512:b02a958fc940dbc1b7e6091b04dc1f65162dcedd1a612254427faa12c162c7e0a0f19169ceafc3c045fd7c693a9e134e6fd95d48422c3299c0d53a2425062c35
```

### `dpkg` source package: `tar=1.30+dfsg-7`

Binary Packages:

- `tar=1.30+dfsg-7`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.30+dfsg-7
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.dsc' tar_1.30+dfsg-7.dsc 1981 SHA512:f4bd8b1605b40b64d340ec6640e0c3d745c6a420238158d07b1ed9110d0adf2ef16a0c55d3dfce28c0ff9e4befa255bda369f6247fb612c44e50dd5dd2e748dc
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA512:f9b3843bd4da03f58d6f88de70ecb36b8ac29312714fd2120ff00f17c99e6d77cc82a8f9de348f4c2bdba9a6cc8e8c6c78039b6c14cdee15d68f2517000c36f2
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.debian.tar.xz' tar_1.30+dfsg-7.debian.tar.xz 22168 SHA512:86bb22465adc886b86a79704ea398bf68bd8365f6b149ac555d9e4d3b7d24231c08c2ab8065661fac45ea2b199e415dbb33e55a4b0e5edf06c361092b6a847e3
```

### `dpkg` source package: `tiff=4.1.0+git191117-2build1`

Binary Packages:

- `libtiff-dev:amd64=4.1.0+git191117-2build1`
- `libtiff5:amd64=4.1.0+git191117-2build1`
- `libtiffxx5:amd64=4.1.0+git191117-2build1`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.1.0+git191117-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117-2build1.dsc' tiff_4.1.0+git191117-2build1.dsc 2291 SHA512:2a57d9910e2c29d8e9fa347f84246669c94cfe67860d0cf110ff1b584492d23fda5bd7f91de5b2aa6c2eb29473afd6f6b1b3f22667ae79ed0e7eff58435f1542
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117.orig.tar.xz' tiff_4.1.0+git191117.orig.tar.xz 1533524 SHA512:25b4bc4522fc2e7f3ca6857b87acd4481d8643566b1120c755020afc8b48949238ee2078bc43dd3ba7407eaa4e36b1b712d7056f101ddaf60f94dab8607870b8
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.1.0+git191117-2build1.debian.tar.xz' tiff_4.1.0+git191117-2build1.debian.tar.xz 19460 SHA512:2c9d80f8b4851beebbd994af3a582aaf84c80ce2e968e023e132670a7c35e0a7af728226f87d91bbae7ee4c0989fba235d14e2ad8e1f6d28e7696f0a0e0a9104
```

### `dpkg` source package: `ubuntu-keyring=2020.06.17.1`

Binary Packages:

- `ubuntu-keyring=2020.06.17.1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2020.06.17.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.dsc' ubuntu-keyring_2020.06.17.1.dsc 1863 SHA512:84bb35395c9b1c42171b4418434638e2aaef6e389bc2f6388c1a32b0f747524784d4e69b1a5f18ed095de045b97df8ed486bffbd3a3fbfedbdb360209a2420d4
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.tar.gz' ubuntu-keyring_2020.06.17.1.tar.gz 36420 SHA512:33009928eeeadbe1627b77f7db1aba32cf1e59d2fd6767bcd0d441d3521cb2b07c5bf06be86e8426c96b9661786a958b2e978f12d8f0941d1ac79289d977eeaf
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

### `dpkg` source package: `unzip=6.0-25ubuntu1`

Binary Packages:

- `unzip=6.0-25ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-25ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-25ubuntu1.dsc' unzip_6.0-25ubuntu1.dsc 1833 SHA512:c224c5ccfb3c26a542fbf153c65978b1146a7525893abbe9af3ab7dd430f842b2a114b65ab58198ab349218df019ed4f0c03d8237a8a8d413b60df8011554cde
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA512:0694e403ebc57b37218e00ec1a406cae5cc9c5b52b6798e0d4590840b6cdbf9ddc0d9471f67af783e960f8fa2e620394d51384257dca23d06bcd90224a80ce5d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-25ubuntu1.debian.tar.xz' unzip_6.0-25ubuntu1.debian.tar.xz 26276 SHA512:c3c9d8d8335bb45760a775cf463e24a326974bbc899266a6419233bd4e44879cdff366f1c4e735199ff27235070556f79b022a5d538c68e5ebe9dee34d94af13
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

### `dpkg` source package: `util-linux=2.36-3ubuntu1`

Binary Packages:

- `bsdutils=1:2.36-3ubuntu1`
- `libblkid-dev:amd64=2.36-3ubuntu1`
- `libblkid1:amd64=2.36-3ubuntu1`
- `libmount-dev:amd64=2.36-3ubuntu1`
- `libmount1:amd64=2.36-3ubuntu1`
- `libsmartcols1:amd64=2.36-3ubuntu1`
- `libuuid1:amd64=2.36-3ubuntu1`
- `mount=2.36-3ubuntu1`
- `util-linux=2.36-3ubuntu1`
- `uuid-dev:amd64=2.36-3ubuntu1`

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
$ apt-get source -qq --print-uris util-linux=2.36-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36-3ubuntu1.dsc' util-linux_2.36-3ubuntu1.dsc 4332 SHA512:56c9a05b0b2a3fae12e5076b85d95e935215533e898f6c26d31efcbb502880334c953d1b098287adcab3e75d7a6411e19cf28a700e647256933b6b0a8ab55df4
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36.orig.tar.xz' util-linux_2.36.orig.tar.xz 5242420 SHA512:cbb4975da8d99a1edd45514171d59ea7b019ce0f77a81e88b447a733f725e91c53540d9dc78bc626dc011dca129b8b150aaf9e64ccf62a4202ae816581acf4fd
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.36-3ubuntu1.debian.tar.xz' util-linux_2.36-3ubuntu1.debian.tar.xz 100176 SHA512:bddbaafbcc0afcb855c3a0b1bd9a5035954374468d5f53c075253948e9e6b98141f2efe2d8e2aa4abf1f273e2c3029a8cd37c35c6ed72c36f8895097f2afe67f
```

### `dpkg` source package: `wget=1.20.3-1ubuntu1`

Binary Packages:

- `wget=1.20.3-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.20.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3-1ubuntu1.dsc' wget_1.20.3-1ubuntu1.dsc 2280 SHA512:aa7e8b81a463b6d5615527abf3b878a3cbf1be4eb4aa7a19185176a0d2ee5b50eb6edc30b84e85d07c5276ecae6245128b9b9177e36ad06803d91574bbbc25d4
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3.orig.tar.gz' wget_1.20.3.orig.tar.gz 4489249 SHA512:e8b82b40e270296228094a78d47f81580bdbdea9e6b93fd61b37dccb39430aeb9bda5397dc53a31c952a61629383c7e2a8c8abf414c8a4dd369af6ecf2717e6c
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3.orig.tar.gz.asc' wget_1.20.3.orig.tar.gz.asc 833 SHA512:40e1bb87dba49e9b8a1e3a6e9ffb95e97933508cd8fef4aac9545b74073800e2945b80bab749e57d4ddc8260a612d784160bec45a6c9c057954d22960c8dd170
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3-1ubuntu1.debian.tar.xz' wget_1.20.3-1ubuntu1.debian.tar.xz 63312 SHA512:98a8ff23cdc35b7d0f35ce90f64fb48ba1cef8c60fa2ccca7d28f2c6e3ac43680ce831cecc6c30b7c69c7f435bc7e9cdcef6960d502e532f6616daf3a629a2eb
```

### `dpkg` source package: `xorg-sgml-doctools=1:1.11-1`

Binary Packages:

- `xorg-sgml-doctools=1:1.11-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xorg-sgml-doctools=1:1.11-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.dsc' xorg-sgml-doctools_1.11-1.dsc 1975 SHA512:3f97156991011d90e9b69b183714290859673b024c2d94bd0a4a22b3e3f0ba66e487d4eca0219a202fd2e303beae46ed1419fed505c85aa20a433837df1a2975
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11.orig.tar.gz' xorg-sgml-doctools_1.11.orig.tar.gz 150367 SHA512:a2386e41a8e2f7deaded61e00eaeab922647c0d0f4e36268c4337dc71d2412b0ec433140d080a0fd118b6112ed0a4f960280f932fe8d4a90ea9dc8bedf1eb75e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.diff.gz' xorg-sgml-doctools_1.11-1.diff.gz 3194 SHA512:8877a9ab1bd95620517d0945632a3b0c7ae8f4d89b61a9895fabb4266fe949a3727e62d301f83b14a61bf06231fa55dd7fe016108d401e7c39cfc34c5c7c9b18
```

### `dpkg` source package: `xorg=1:7.7+19ubuntu14`

Binary Packages:

- `x11-common=1:7.7+19ubuntu14`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `xorgproto=2020.1-1`

Binary Packages:

- `x11proto-core-dev=2020.1-1`
- `x11proto-dev=2020.1-1`
- `x11proto-xext-dev=2020.1-1`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`, `/usr/share/doc/x11proto-xext-dev/copyright`)

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

### `dpkg` source package: `xz-utils=5.2.4-1ubuntu1`

Binary Packages:

- `liblzma-dev:amd64=5.2.4-1ubuntu1`
- `liblzma5:amd64=5.2.4-1ubuntu1`
- `xz-utils=5.2.4-1ubuntu1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.dsc' xz-utils_5.2.4-1ubuntu1.dsc 2629 SHA512:09c0668c76bd1653460ae2207f2666785d6ec7bae424d168e2f5dc2c98d2c34b7f983963be27c39ac05df0ad76ccfe088b55a64a09319f26b785544d5c8ffb66
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA512:00db7dd31a61541b1ce6946e0f21106f418dd1ac3f27cdb8682979cbc3bd777cd6dd1f04f9ba257a0a7e24041e15ca40d0dd5c130380dce62280af67a0beb97f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA512:dbfce0556bc85545ce3566a01c25e4876f560409fc2d48f2dc382b10fbd2538c61d8f2c3667d86fc7313aec86c05e53926015000320f19615e97875adae42450
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.debian.tar.xz' xz-utils_5.2.4-1ubuntu1.debian.tar.xz 135512 SHA512:9ec339da084b6aedd5d9dfafe879f7b90ae6dc473458dd8eda234e087f3aa80480b7b0792b54588d57e1b41a2c42f28ef87b8e6a8cd4bb51d43e2517f701724f
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu2`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu2`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

