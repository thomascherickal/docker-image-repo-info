# `buildpack-deps:bionic`

## Docker Metadata

- Image ID: `sha256:52e8c53deaf38daf74bde52dc83f9d7da64a2829d888fc8d26427bd2161a90e4`
- Created: `2020-11-26T01:05:55.897109897Z`
- Virtual Size: ~ 618.10 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3build1`

Binary Packages:

- `libacl1:amd64=2.2.52-3build1`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3build1.dsc' acl_2.2.52-3build1.dsc 2031 SHA256:864215f3e68d6b169a044bd952e78be9b0b1cf527a2cbf25866cab919e78e64b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3build1.debian.tar.xz' acl_2.2.52-3build1.debian.tar.xz 8788 SHA256:0729d8c850aa26bc9f1b22ce632efb1616a3f97dc5fca1d9edfda45b582b7f37
```

### `dpkg` source package: `adduser=3.116ubuntu1`

Binary Packages:

- `adduser=3.116ubuntu1`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.116ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.116ubuntu1.dsc' adduser_3.116ubuntu1.dsc 1845 SHA256:fc44097093d74fc2e36fc37dceb54cf6bcb70a434240b14fd91beb64849cf2fd
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.116ubuntu1.tar.xz' adduser_3.116ubuntu1.tar.xz 216868 SHA256:f34f1d95e96ecae3b068a3dd666848f82f06cbb26152c56a6b72bd71555a8f18
```

### `dpkg` source package: `apr-util=1.6.1-2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-2.dsc' apr-util_1.6.1-2.dsc 2851 SHA256:7a3a7d0dccc0d89ad751988163cb57d34b32094893d08c4d0ac79e9bfee6d8f4
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2.asc' apr-util_1.6.1.orig.tar.bz2.asc 801 SHA256:47837b605290c0d7659b73734e4a9d5e6c0c24c13185cd4d91837afe63c07ca4
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-2.debian.tar.xz' apr-util_1.6.1-2.debian.tar.xz 211832 SHA256:e30e919e7e049a8a7056b7184e77d69b82660d71a4bf9654d1c9bfccf2fcde30
```

### `dpkg` source package: `apr=1.6.3-2`

Binary Packages:

- `libapr1:amd64=1.6.3-2`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.3-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3-2.dsc' apr_1.6.3-2.dsc 2305 SHA256:0597703f9ea3bc3b30fcd7e055c67c2113e5c4255df5ff42738ce6a396bf5afc
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3.orig.tar.bz2' apr_1.6.3.orig.tar.bz2 854100 SHA256:131f06d16d7aabd097fa992a33eec2b6af3962f93e6d570a9bd4d85e95993172
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3.orig.tar.bz2.asc' apr_1.6.3.orig.tar.bz2.asc 801 SHA256:33db39162f7ca9acdccaa4f19630a67045542791b262116d3512c8b5d7c3fca1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.3-2.debian.tar.xz' apr_1.6.3-2.debian.tar.xz 213068 SHA256:ac515f888f7157586631e3de9792ee01d239f9cbf1e768be31ee6daac61f2597
```

### `dpkg` source package: `apt=1.6.12ubuntu0.1`

Binary Packages:

- `apt=1.6.12ubuntu0.1`
- `libapt-pkg5.0:amd64=1.6.12ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.6.12ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.dsc' apt_1.6.12ubuntu0.1.dsc 2561 SHA512:39e55dff8d40ad1c1356f00b1eaff27ab6bb803fc6ea0d0669031540cac8b623e36e36a9c9b1eafc9421f828912d3874e57e58a5347f77e28f8d9d623555ea1d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.6.12ubuntu0.1.tar.xz' apt_1.6.12ubuntu0.1.tar.xz 2172208 SHA512:77c3c1c26522f00ecd7549a51f92f50a58d4fc31a0b31d9f78663b79ab043a2c3be22cde9c568f41b19c1f87d03c999d36adc0a6518de8af262e12b5021c4c84
```

### `dpkg` source package: `attr=1:2.4.47-2build1`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2build1`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2build1.dsc' attr_2.4.47-2build1.dsc 2033 SHA256:b78dbf07b789010caabc12c1ab0b2a944072058fe47ac6b5d345209c16f4e1f5
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2build1.debian.tar.xz' attr_2.4.47-2build1.debian.tar.xz 8168 SHA256:6732a8874190a1f792c7f9cb95fadc1dc852baf2e164b0d7b4bcea525f5c0882
```

### `dpkg` source package: `audit=1:2.8.2-1ubuntu1`

Binary Packages:

- `libaudit-common=1:2.8.2-1ubuntu1`
- `libaudit1:amd64=1:2.8.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2-1ubuntu1.dsc' audit_2.8.2-1ubuntu1.dsc 2903 SHA256:454c231dc2268ee4862f87d65720354699be9b807a411556a536bc2b4e581a90
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2.orig.tar.gz' audit_2.8.2.orig.tar.gz 1121970 SHA256:67b59b2b77afee9ed87afa4d80ffc8e6f3a1f4bbedd5f2871f387c952147bcba
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.2-1ubuntu1.debian.tar.xz' audit_2.8.2-1ubuntu1.debian.tar.xz 21344 SHA256:2bc93230e3bf01eef5e9a5acff8f904af074e6e39003f1db8941118fbd041ec2
```

### `dpkg` source package: `autoconf=2.69-11`

Binary Packages:

- `autoconf=2.69-11`

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
$ apt-get source -qq --print-uris autoconf=2.69-11
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.dsc' autoconf_2.69-11.dsc 1948 SHA256:249d25370d4f4d1d0cf7b37bfd178bb6fa87011566dd82230991f64814a39dde
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.debian.tar.xz' autoconf_2.69-11.debian.tar.xz 23540 SHA256:885b3947fdead5b737f6437b80a90a41c5d611791573c5d0cfef50a59c943c1b
```

### `dpkg` source package: `automake-1.15=1:1.15.1-3ubuntu2`

Binary Packages:

- `automake=1:1.15.1-3ubuntu2`

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
$ apt-get source -qq --print-uris automake-1.15=1:1.15.1-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.15/automake-1.15_1.15.1-3ubuntu2.dsc' automake-1.15_1.15.1-3ubuntu2.dsc 2663 SHA256:406f9f2118936675f458d18fcb7aeb707428ba0fffb074c21e8083834a5e95ff
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.15/automake-1.15_1.15.1.orig.tar.xz' automake-1.15_1.15.1.orig.tar.xz 1509496 SHA256:af6ba39142220687c500f79b4aa2f181d9b24e4f8d8ec497cea4ba26c64bedaf
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.15/automake-1.15_1.15.1-3ubuntu2.debian.tar.xz' automake-1.15_1.15.1-3ubuntu2.debian.tar.xz 14580 SHA256:d84981f19bcf179aaeb1a471329c28332aae3fa22062b840bbc700032a556e0b
```

### `dpkg` source package: `autotools-dev=20180224.1`

Binary Packages:

- `autotools-dev=20180224.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.dsc' autotools-dev_20180224.1.dsc 1643 SHA256:795f558377bf6c90280c293b2711afc094cd1bf6ae486a395e1361ffd242cd2f
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.tar.xz' autotools-dev_20180224.1.tar.xz 68256 SHA256:355a4d8461dfedebd2c5194603197712a10f71e20de73a35ab6e90b7acf3e837
```

### `dpkg` source package: `base-files=10.1ubuntu2.10`

Binary Packages:

- `base-files=10.1ubuntu2.10`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=10.1ubuntu2.10
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_10.1ubuntu2.10.dsc' base-files_10.1ubuntu2.10.dsc 1688 SHA512:79cd0404b5885944c52a99dbed1d9ffc33dad914a2c2151c283d981fd3a4a1064bb594a45deda9c36889d0aa5f0b6b5b6a1d7c77c13b9460ac191cd4f0484e87
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_10.1ubuntu2.10.tar.xz' base-files_10.1ubuntu2.10.tar.xz 79780 SHA512:826d4e116644b905c52372f79cdb29aa0f5a360f3dd48843d51aae778c4a8ab4264d24a9c01a3f16230d6b5db209b09d06fa976a0018bb0c3d0c512297183757
```

### `dpkg` source package: `base-passwd=3.5.44`

Binary Packages:

- `base-passwd=3.5.44`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.44
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.44.dsc' base-passwd_3.5.44.dsc 1685 SHA256:22a5db1e9bb71fa8a4d682b3f9c01470a61b8041eb6212471181c6808b268c13
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.44.tar.xz' base-passwd_3.5.44.tar.xz 52644 SHA256:f17a0746024572e86e60e4614cf226a81ffe682ceaf1a1fce9dc1a8002683e90
```

### `dpkg` source package: `bash=4.4.18-2ubuntu1.2`

Binary Packages:

- `bash=4.4.18-2ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.4.18-2ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.dsc' bash_4.4.18-2ubuntu1.2.dsc 2434 SHA512:9cac142b52cd93d5faa8db4e755c5509d2a98358a84e5522a669d3b2ad0b3bb87c9f9deb35a582d666baefb98c6e91a96d506ddf833d50b856d36768065eef97
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18.orig.tar.xz' bash_4.4.18.orig.tar.xz 5036272 SHA512:a0c0b84133f9dc1dd404a130a6a8ac08c4551d28bf4d0a6a9be40acee5d1465270af595191cad9584f17fe098b846a70dd1f7772f771db79ff5f03e47cfd5791
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.4.18-2ubuntu1.2.debian.tar.xz' bash_4.4.18-2ubuntu1.2.debian.tar.xz 65236 SHA512:84ef4350f9069601a8bfe9c444400e268b927c286970270c2c635dac8946f5f499658fe822404ae662d922655a5158b019f8a4c3dcec1ffd72b1aa40b85830e4
```

### `dpkg` source package: `binutils=2.30-21ubuntu1~18.04.4`

Binary Packages:

- `binutils=2.30-21ubuntu1~18.04.4`
- `binutils-common:amd64=2.30-21ubuntu1~18.04.4`
- `binutils-x86-64-linux-gnu=2.30-21ubuntu1~18.04.4`
- `libbinutils:amd64=2.30-21ubuntu1~18.04.4`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.30-21ubuntu1~18.04.4
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.30-21ubuntu1~18.04.4.dsc' binutils_2.30-21ubuntu1~18.04.4.dsc 11670 SHA512:eb6395cdf36bcbebad2e8dc310941d8d07792b2bedf516b402da2f5fceb32dad5997f0d28996281bababb75fa7e47f5d436187f1c8e0bd31a21018951a1bb34b
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.30.orig.tar.xz' binutils_2.30.orig.tar.xz 20286700 SHA512:e747ea20d8d79fcd21b9d9f6695059caa7189d60f19256da398e34b789fea9a133c32b192e9693b5828d27683739b0198431bf8b3e39fb3b04884cf89d9aa839
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.30-21ubuntu1~18.04.4.debian.tar.xz' binutils_2.30-21ubuntu1~18.04.4.debian.tar.xz 622680 SHA512:cb1ec1b01224eac900f4b74e03c858e3813de07a2d415b0c158db43b33c46c05b2be83da565602b244fda3f59b46df556ac7131b292590d140def6635b759ab9
```

### `dpkg` source package: `bzip2=1.0.6-8.1ubuntu0.2`

Binary Packages:

- `bzip2=1.0.6-8.1ubuntu0.2`
- `libbz2-1.0:amd64=1.0.6-8.1ubuntu0.2`
- `libbz2-dev:amd64=1.0.6-8.1ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8.1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.dsc' bzip2_1.0.6-8.1ubuntu0.2.dsc 2181 SHA512:872defc414a97416d701ce8bb59ddbf44b80ebffe447d67ebba20ed13b3e006c771002c82ad11c0c669004d22ce9368254e44c6be977c21e7d92dab69ec4e33a
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA512:b1108c392a7f45218b86196498657f50333c870db4ab555ce4859a3fe76c17b4a3430b8a075b7f1c86d9ded006bdf17001b73bfcf261e2d2ee7de4998ad604fd
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2' bzip2_1.0.6-8.1ubuntu0.2.debian.tar.bz2 61477 SHA512:f895cded216bd210eed7356be97630de75f650bb40d3bb0c7a26b0fadf9991188005ab1c5438e4b8f95614e6ff8c2ad5b2a94f0cc048580bcdc387a219ba7495
```

### `dpkg` source package: `bzr=2.7.0+bzr6622-10`

Binary Packages:

- `bzr=2.7.0+bzr6622-10`
- `python-bzrlib=2.7.0+bzr6622-10`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`, `/usr/share/doc/python-bzrlib/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.7.0+bzr6622-10
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0+bzr6622-10.dsc' bzr_2.7.0+bzr6622-10.dsc 2521 SHA256:658f59aaaa101288369e96ab766f5344e31eaa835fa008ad56df2ed65d11903e
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0+bzr6622.orig.tar.gz' bzr_2.7.0+bzr6622.orig.tar.gz 10948360 SHA256:08bba3e76cba9beb6b686e71253045beeab9db94753ddbcafa0f8ed1cba377ff
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0+bzr6622-10.debian.tar.xz' bzr_2.7.0+bzr6622-10.debian.tar.xz 92572 SHA256:0e35de0eea3cb6910e3dfef330502afd01be60c4cd0b9ca3d5f77e9bb0f406aa
```

### `dpkg` source package: `ca-certificates=20201027ubuntu0.18.04.1`

Binary Packages:

- `ca-certificates=20201027ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20201027ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20201027ubuntu0.18.04.1.dsc' ca-certificates_20201027ubuntu0.18.04.1.dsc 1937 SHA512:874fb0954587d2d76b1f10a6a026f8fc190a254074b55703ec3f1873204d13977265f0e822bdbadf3fe23d59ca9c06e913fdb1c94249a561d3d3ddbf26867a5c
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20201027ubuntu0.18.04.1.tar.xz' ca-certificates_20201027ubuntu0.18.04.1.tar.xz 241956 SHA512:d75463849f08fa4be684ff86147828025abdde813f87b93167c047334db39d66c7f349f48d779a3557d4e58f9de9661a4ba83cba8231c19f29bf6661f14d7ab2
```

### `dpkg` source package: `cairo=1.15.10-2ubuntu0.1`

Binary Packages:

- `libcairo-gobject2:amd64=1.15.10-2ubuntu0.1`
- `libcairo-script-interpreter2:amd64=1.15.10-2ubuntu0.1`
- `libcairo2:amd64=1.15.10-2ubuntu0.1`
- `libcairo2-dev:amd64=1.15.10-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.15.10-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10-2ubuntu0.1.dsc' cairo_1.15.10-2ubuntu0.1.dsc 2290 SHA512:4bcf578ca2f1defc527350003aa380896e9357f7a1abb47c50888ae74359333cfc1755a24df5d833f4de6b43c9c6717fe6b5fbaa60c26cfdc8920b7cdf909b0a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10.orig.tar.xz' cairo_1.15.10.orig.tar.xz 41881364 SHA512:d56dbf1675c37b70344c1202ac7b50540a99f51a243a98464b05ffb3bb6f17b240af15dea9e3553a1abd36c95c6cf75a2077932205db5461d8a6a9d8aed33686
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.15.10-2ubuntu0.1.debian.tar.xz' cairo_1.15.10-2ubuntu0.1.debian.tar.xz 31128 SHA512:f4d7333e2f58e2ed50a90a2e5067c79af805d4f10f834ef9b5552636682d67dbe3cab7e8f5860164e3cf2c5d8232a2c7013e30bd6dd8f1dd41c354595607d5f2
```

### `dpkg` source package: `cdebconf=0.213ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.213ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.213ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.213ubuntu1.dsc' cdebconf_0.213ubuntu1.dsc 2769 SHA256:76cb3f0b1685629220b0e4c3105757b95714f7350df4e7863d5310f1f581fee0
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.213ubuntu1.tar.xz' cdebconf_0.213ubuntu1.tar.xz 272596 SHA256:624feaf9e7e5f407271f99e06e54d5002fcce51345553a626caf7b4a65f0afd1
```

### `dpkg` source package: `configobj=5.0.6-2`

Binary Packages:

- `python-configobj=5.0.6-2`

Licenses: (parsed from: `/usr/share/doc/python-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-2.dsc' configobj_5.0.6-2.dsc 2381 SHA256:9bb8577128460ff33326d3d90b8454376c83f4d41b1da61aeabdbfcbfb5e0087
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA256:2e140354efcca6f558ff9ee941b435ae09a617bc071797bef62c8d6ed2033d5e
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-2.debian.tar.xz' configobj_5.0.6-2.debian.tar.xz 7436 SHA256:dc677cd329b4a3aacebe10c5a169d9d092cc27888c3f3f9203930cacd6a0eab8
```

### `dpkg` source package: `coreutils=8.28-1ubuntu1`

Binary Packages:

- `coreutils=8.28-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.28-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28-1ubuntu1.dsc' coreutils_8.28-1ubuntu1.dsc 2302 SHA256:9a7154fd8a458295b686383767f9305095e6ea929a08c8f56cf51640c3fe209f
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz' coreutils_8.28.orig.tar.xz 5252336 SHA256:1117b1a16039ddd84d51a9923948307cfa28c2cea03d1a2438742253df0a0c65
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28.orig.tar.xz.asc' coreutils_8.28.orig.tar.xz.asc 1196 SHA256:505b1a530a55732a9ed659d419ff4973d1b15059078d2060675927058db9607d
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.28-1ubuntu1.debian.tar.xz' coreutils_8.28-1ubuntu1.debian.tar.xz 37940 SHA256:71ba2e83edc675a79e1e0556aff326ab2ae812332692e3db29615e8ed1b427f4
```

### `dpkg` source package: `curl=7.58.0-2ubuntu3.10`

Binary Packages:

- `curl=7.58.0-2ubuntu3.10`
- `libcurl3-gnutls:amd64=7.58.0-2ubuntu3.10`
- `libcurl4:amd64=7.58.0-2ubuntu3.10`
- `libcurl4-openssl-dev:amd64=7.58.0-2ubuntu3.10`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.58.0-2ubuntu3.10
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.dsc' curl_7.58.0-2ubuntu3.10.dsc 2781 SHA512:6674bade118bb14272b82c6a0d803ebe0de0ae1530e752518e4b409a31c8448694a4551fcdcbec595d5fe0a53712ec6d5076ae0e4b4d705140fa575cdcc6e269
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0.orig.tar.gz' curl_7.58.0.orig.tar.gz 3879728 SHA512:7b12b79107558bb266672d6e128615fe5a8149c37f4ae540197e3298f5d312beb2d78fbb23e3ea84ea7afc41549898a1e5cd38509f0388b11707b48d5efb8ca3
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.58.0-2ubuntu3.10.debian.tar.xz' curl_7.58.0-2ubuntu3.10.debian.tar.xz 41908 SHA512:6ec45923614cadc69045ff317270e1494687ea75fa4298df9fe0b23b3d22bf14f7ccf05edbd515cd7d8f011bce4e05faedcb6f327a030584b237a3b76752187f
```

### `dpkg` source package: `cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Binary Packages:

- `libsasl2-2:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`
- `libsasl2-modules-db:amd64=2.1.27~101-g0780600+dfsg-3ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27~101-g0780600+dfsg-3ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.dsc 3297 SHA512:0c64b0a5cffa46d49ddd4a359c35e1b92d3c446415e8faf29c7a8d689073dc9bbcd0427aff30ee8d70b1712b27dc202ec14c955538d92998ecd6dc96569b2665
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg.orig.tar.xz 1143888 SHA512:cd684133dcea5856301f50e378ff105e88f8008af06bd4e02fb9a62a88ece2ee1901ea2776ef3d941d6a3cfc2a77875c08054326293818db89e5f9995c4cd524
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz' cyrus-sasl2_2.1.27~101-g0780600+dfsg-3ubuntu2.1.debian.tar.xz 95712 SHA512:c8eb0ff8cf4db3a3d3af2875626d9f39c058ea259c41d9954be18b269fc0fe0809ac2fea63c1ede72873cfa7388f8b76685e77eaaab64695d62739cef6ad6715
```

### `dpkg` source package: `dash=0.5.8-2.10`

Binary Packages:

- `dash=0.5.8-2.10`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.8-2.10
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.10.dsc' dash_0.5.8-2.10.dsc 1618 SHA256:1e8fdac0880d57d8ed5eb11f9f1750a67c71a7200180cf3ed5aa3e74dab3e4c5
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8.orig.tar.gz' dash_0.5.8.orig.tar.gz 223028 SHA256:c6db3a237747b02d20382a761397563d813b306c020ae28ce25a1c3915fac60f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.10.debian.tar.xz' dash_0.5.8-2.10.debian.tar.xz 43920 SHA256:0d870b0cf9b3ad40e4d4f1e3d4d9097f4d62151693a48f34cb1d49865fd4abdb
```

### `dpkg` source package: `db-defaults=1:5.3.21~exp1ubuntu2`

Binary Packages:

- `libdb-dev:amd64=1:5.3.21~exp1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libdb-dev/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris db-defaults=1:5.3.21~exp1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.dsc' db-defaults_5.3.21~exp1ubuntu2.dsc 2044 SHA256:1960179af0244d410f368653e32d594c8e9331e2046422d05c33edc7f0d248b6
'http://archive.ubuntu.com/ubuntu/pool/main/d/db-defaults/db-defaults_5.3.21~exp1ubuntu2.tar.xz' db-defaults_5.3.21~exp1ubuntu2.tar.xz 3032 SHA256:03c2bba2824a4f5042960a4712630e35d2cbf885a22d24f2b27b2ca28ad6f46a
```

### `dpkg` source package: `db5.3=5.3.28-13.1ubuntu1.1`

Binary Packages:

- `libdb5.3:amd64=5.3.28-13.1ubuntu1.1`
- `libdb5.3-dev=5.3.28-13.1ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-13.1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.dsc' db5.3_5.3.28-13.1ubuntu1.1.dsc 3068 SHA512:20b2e7cddbf97b5de71d782b6df35c6586686da822ae978e5d60acfb3fecd4b00568b24a5ff33bfe05bc8776a0dc4d4d5dc0cc1b127f4fd0bb2d485f6fb108bd
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA512:080483cac3119569e04c3c22c95e97e5e448c88d87a443933d0ef2c71b506f309428584d6a8fb9c236c616dd82beffa1b30361b4c918756745983fcf54a3f8da
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz' db5.3_5.3.28-13.1ubuntu1.1.debian.tar.xz 29444 SHA512:0e30e4884d67561970fcff40f41641cb7bd663cc5310d396ddc002a26b348d12ca46dd2f265cfd479daffbc42530d047a177b943d65d96dfb483cd1c4e918dc4
```

### `dpkg` source package: `debconf=1.5.66ubuntu1`

Binary Packages:

- `debconf=1.5.66ubuntu1`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.66ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.dsc' debconf_1.5.66ubuntu1.dsc 2087 SHA512:5320524b5b84afeb7b48a50e25ba80648de989c83f3e8e6c0797e500b4be872cad0e226fe2e7c0bc3e7bed67747006ae855c5f9131e6ffb9a9618800e83d5016
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.66ubuntu1.tar.xz' debconf_1.5.66ubuntu1.tar.xz 572556 SHA512:6890b7639c884d4e28d43ac4ca27dd6ab845d9c451521d18369d57a487f2fd14966b30878065d749c60279d0f2f1996035e280e5d060b6c7ff8902bc32fac1f9
```

### `dpkg` source package: `debianutils=4.8.4`

Binary Packages:

- `debianutils=4.8.4`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.8.4
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.4.dsc' debianutils_4.8.4.dsc 1764 SHA256:8b12921fe6e4f51d295bfd4213706d588a6c9b8bab659b0ee1fe525f37e9fbcc
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.8.4.tar.xz' debianutils_4.8.4.tar.xz 156344 SHA256:c061ab99aea61f892043b7624b021ab5b193e9c6bbfd474da0fbcdd506be1eb2
```

### `dpkg` source package: `diffutils=1:3.6-1`

Binary Packages:

- `diffutils=1:3.6-1`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6-1.dsc' diffutils_3.6-1.dsc 1453 SHA256:26fe7690b45748dc92cee6af224192e78db2ac574e16ae0aeb8ed6a472c883cd
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6.orig.tar.xz' diffutils_3.6.orig.tar.xz 1398296 SHA256:d621e8bdd4b573918c8145f7ae61817d1be9deb4c8d2328a65cea8e11d783bd6
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.6-1.debian.tar.xz' diffutils_3.6-1.debian.tar.xz 10808 SHA256:f6ab546a134bde18a87ca8e3c98919680e79d81a65a24801ae06ef69b33f24d8
```

### `dpkg` source package: `djvulibre=3.5.27.1-8ubuntu0.2`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.27.1-8ubuntu0.2`
- `libdjvulibre-text=3.5.27.1-8ubuntu0.2`
- `libdjvulibre21:amd64=3.5.27.1-8ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-8ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-8ubuntu0.2.dsc' djvulibre_3.5.27.1-8ubuntu0.2.dsc 1870 SHA512:096d825b4c69f8f3cb2468d8bb005c192dfa645c543079d648a7af07286aa0ceead2f73c14a967d3be20d3d36d7396e2e6c7a5056666956faaf52862131e9394
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA512:2ed11daa05995db7bf52113e2f75456c3c804988d2c17d0183b24ab379e52a4ef1871189e8bb132fec6cbc9d629b4d67a4d89ef7df7a995044cb25ff3dcc5de8
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-8ubuntu0.2.debian.tar.xz' djvulibre_3.5.27.1-8ubuntu0.2.debian.tar.xz 59648 SHA512:d6724572b94746374af80bd1165ea1630e282a5a9028d2dc9e49cd5b272b5afa26e1ecb8ade27af1a55a86265945dc7754e5f25bc15423b952afd846ddaa015d
```

### `dpkg` source package: `dpkg=1.19.0.5ubuntu2.3`

Binary Packages:

- `dpkg=1.19.0.5ubuntu2.3`
- `dpkg-dev=1.19.0.5ubuntu2.3`
- `libdpkg-perl=1.19.0.5ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.0.5ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.dsc' dpkg_1.19.0.5ubuntu2.3.dsc 2144 SHA512:b788b94a2e602ab43a7fdf734f518ea8f43fd0d6ccc11a5be01d3e18d5917db1224c266a1790336093fc06a976efa390fd99d81e380f3abe291ba4686c131579
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.0.5ubuntu2.3.tar.xz' dpkg_1.19.0.5ubuntu2.3.tar.xz 4571256 SHA512:f9dc03714fee11a8bb62b3d1a556853329ab3b41dd996914cb47f38432e6b46c939433282f9039575811cb0e57508e9fbd2a5259eca7d9134d4760c636c3ec91
```

### `dpkg` source package: `e2fsprogs=1.44.1-1ubuntu1.3`

Binary Packages:

- `comerr-dev:amd64=2.1-1.44.1-1ubuntu1.3`
- `e2fsprogs=1.44.1-1ubuntu1.3`
- `libcom-err2:amd64=1.44.1-1ubuntu1.3`
- `libext2fs2:amd64=1.44.1-1ubuntu1.3`
- `libss2:amd64=1.44.1-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.44.1-1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.dsc' e2fsprogs_1.44.1-1ubuntu1.3.dsc 3188 SHA512:e5311f88ee8498252027c0c57ea62dc5a924535d93f66da281e9c1a506eee2157d008f01b96c8df5e597720fd57f05877991310b3d0cedef00a8f84645b65409
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz' e2fsprogs_1.44.1.orig.tar.gz 7544908 SHA512:c4b1f9baab70ceac9058286eeb75f57a738f01eaa0d9dd74eaaf9b0fd0709c954a0b3efb75896b9dd67ab2626febadd6635fe04a5c32e0700419d2531024dacf
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1.orig.tar.gz.asc' e2fsprogs_1.44.1.orig.tar.gz.asc 488 SHA512:8e3771c784ac83b368e2258ebbd12869683be88cfad15b019ed5e60b72c21aac713494e987f3f3568e859b585808a41480027dd991163a785a93bdf78584853b
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz' e2fsprogs_1.44.1-1ubuntu1.3.debian.tar.xz 81152 SHA512:0fa4885fbd73b00efbd865e17898362d6cd8551be169f8f23ea0fa52cf4de8d6c244315ef69631062fbc97c11be19f0decfac775811b47405416e5ae645e0956
```

### `dpkg` source package: `elfutils=0.170-0.4ubuntu0.1`

Binary Packages:

- `libelf1:amd64=0.170-0.4ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.170-0.4ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170-0.4ubuntu0.1.dsc' elfutils_0.170-0.4ubuntu0.1.dsc 2422 SHA512:cc08e16e9e1b892911f1f48d465127ec621c5dfe9ad3054d5d52e1f165b6650ae76c6f590af05ba743c414ad738379b6a9467f33776e8d2c03a4f0d7b2097507
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170.orig.tar.bz2' elfutils_0.170.orig.tar.bz2 8358001 SHA512:aca0b5e271138eaf86e36505ffb101181207b151e833e6cd7c18986ac50678542a5ecd2250f8dd6923ca497142f197c8b08fd225e4130b16b6203c24013d6d28
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.170-0.4ubuntu0.1.debian.tar.xz' elfutils_0.170-0.4ubuntu0.1.debian.tar.xz 51740 SHA512:a9d615f2dced250403c897ec1e2e2ff2b44523763b88cfad5656d60e864bb42b35384fdfdad372747499732c20e40e2e7d2de06a18c5284ea19f1a1617e2f254
```

### `dpkg` source package: `expat=2.2.5-3ubuntu0.2`

Binary Packages:

- `libexpat1:amd64=2.2.5-3ubuntu0.2`
- `libexpat1-dev:amd64=2.2.5-3ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.5-3ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.dsc' expat_2.2.5-3ubuntu0.2.dsc 2198 SHA512:efe01c6d1bb262332995fe1dbe25829fc5b416fa6f566505a70ed9e11ef5a4d7ca0769eab6fb0dce655f0ec4facefcff1e29d93c660c90a115819f489a0d30f8
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5.orig.tar.gz' expat_2.2.5.orig.tar.gz 8273003 SHA512:61ce2a479521412e0c56c352106c4adfb61a6bedb883921aba3ebccc29311ddd192646ac2c51b41572728d4de6ab4cb60a1dbc71515d742a80a8b59d89ca74d6
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.5-3ubuntu0.2.debian.tar.xz' expat_2.2.5-3ubuntu0.2.debian.tar.xz 12024 SHA512:79f104bce4515465616eea834d2d932aba403929799ea97ecfd09e6890307709caa9b2a4dab2e3697a124232c2ff7f31b5c5a06436df06e19ea934834779da68
```

### `dpkg` source package: `fftw3=3.3.7-1`

Binary Packages:

- `libfftw3-double3:amd64=3.3.7-1`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.7-1.dsc' fftw3_3.3.7-1.dsc 2941 SHA256:65568aacf8b55d87392aeb640ca9bcd37b0d9f1fe2312b298c43c18764e8470a
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.7.orig.tar.xz' fftw3_3.3.7.orig.tar.xz 2354860 SHA256:1eb677807ec114a3b1dbbae5d866683b71de2977101cb116063a753365465498
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.7-1.debian.tar.xz' fftw3_3.3.7-1.debian.tar.xz 13628 SHA256:5b3763ecfa0177e7c43bf330038b4b2c4d71a5b8c9c33b3e89ccfa4e59f2011b
```

### `dpkg` source package: `file=1:5.32-2ubuntu0.4`

Binary Packages:

- `file=1:5.32-2ubuntu0.4`
- `libmagic-mgc=1:5.32-2ubuntu0.4`
- `libmagic1:amd64=1:5.32-2ubuntu0.4`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic-mgc/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.32-2ubuntu0.4
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.32-2ubuntu0.4.dsc' file_5.32-2ubuntu0.4.dsc 1972 SHA512:5d05305d59b222640d75fbc2acc9aa5d95d890f78ab6b3343bebcced830b5c3302f1f560b1ee5f21b7f5bf7599355680a1a8ee59e8ab017916635c43b6b88e65
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.32.orig.tar.xz' file_5.32.orig.tar.xz 584352 SHA512:86e095de383a9da86f9adaf0d8cff0f99d7b9c02d75fbc49295f6c44575499e360b8878d0a69109a531307b4f4ac3a7f1655ffcf82ed9619be0e09735d0b139d
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.32-2ubuntu0.4.debian.tar.xz' file_5.32-2ubuntu0.4.debian.tar.xz 33868 SHA512:5ec41bcf4418ca2c07ed981d1a728e817505a181e59151a5f7e21303ae753dac83e6d8228f6b673c614de19eca56eb6cfe22e2ad42ce69cbaa450319a02f18b4
```

### `dpkg` source package: `findutils=4.6.0+git+20170828-2`

Binary Packages:

- `findutils=4.6.0+git+20170828-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20170828-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828-2.dsc' findutils_4.6.0+git+20170828-2.dsc 2221 SHA256:6997072de2f1b24457073275f7b8f15ad2f0569389dcb277ebe99dd1846e2ee9
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828.orig.tar.xz' findutils_4.6.0+git+20170828.orig.tar.xz 1865192 SHA256:8d6571ffd5105307bcb1b20c4b7d5c2d0b5152e463b082801268bd3ec9e2bbfd
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20170828-2.debian.tar.xz' findutils_4.6.0+git+20170828-2.debian.tar.xz 26532 SHA256:5b13792a14edec982fddcf74fe01b4380b909703d76aaba2860da51c6248de73
```

### `dpkg` source package: `fontconfig=2.12.6-0ubuntu2`

Binary Packages:

- `fontconfig=2.12.6-0ubuntu2`
- `fontconfig-config=2.12.6-0ubuntu2`
- `libfontconfig1:amd64=2.12.6-0ubuntu2`
- `libfontconfig1-dev:amd64=2.12.6-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.12.6-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.12.6-0ubuntu2.dsc' fontconfig_2.12.6-0ubuntu2.dsc 2384 SHA256:e7109f728f73761ad17ff5c5ec066ad940b67b779a78a094b67a7af4cfafadcc
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.12.6.orig.tar.bz2' fontconfig_2.12.6.orig.tar.bz2 1624683 SHA256:cf0c30807d08f6a28ab46c61b8dbd55c97d2f292cf88f3a07d3384687f31f017
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.12.6-0ubuntu2.debian.tar.xz' fontconfig_2.12.6-0ubuntu2.debian.tar.xz 29168 SHA256:75c259e2d6b1944fe76a49f89b806b3ee34fe7a42eb25efd289e38b1b5e16517
```

### `dpkg` source package: `fonts-dejavu=2.37-1`

Binary Packages:

- `fonts-dejavu-core=2.37-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.37-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.dsc' fonts-dejavu_2.37-1.dsc 2575 SHA256:f35ff7b2c8dbfda6564c9dedf088ba06cc6d279fdd8e7cccbd1ae08ded1bb71c
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37.orig.tar.bz2' fonts-dejavu_2.37.orig.tar.bz2 12050109 SHA256:4b21c5203f792343d5e90ab1cb0cf07e99887218abe3d83cd9a98cea9085e799
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.37-1.debian.tar.xz' fonts-dejavu_2.37-1.debian.tar.xz 10424 SHA256:5105cdbfc086f4a83ab6871eb39cc904bf02aa52762402b7cacf33d0938122f7
```

### `dpkg` source package: `freetype=2.8.1-2ubuntu2.1`

Binary Packages:

- `libfreetype6:amd64=2.8.1-2ubuntu2.1`
- `libfreetype6-dev:amd64=2.8.1-2ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`, `/usr/share/doc/libfreetype6-dev/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `Catharon-OSL`
- `FTL`
- `GPL-2`
- `GPL-2+`
- `GZip`
- `OpenGroup-BSD-like`

Source:

```console
$ apt-get source -qq --print-uris freetype=2.8.1-2ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1-2ubuntu2.1.dsc' freetype_2.8.1-2ubuntu2.1.dsc 1951 SHA512:90e7186c8550b7daceb1adfa35059ea8c08672d01a65f800a63edeabc328fb9f74d66e8d330288c7f97c2751862dc23e5c9cb7a62299a1463d8541a7ae2eafab
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1.orig.tar.gz' freetype_2.8.1.orig.tar.gz 4242784 SHA512:60164caefc506c096142a05e4b578f48d65350fca3082527cd421ed5d0b9671c1123c2303b50ea09dc204288d6d4cbb548a761f67bd8260220f2c83b8f144d42
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.8.1-2ubuntu2.1.diff.gz' freetype_2.8.1-2ubuntu2.1.diff.gz 44970 SHA512:f3906b19118934019b61afa47f7be110fa56815cebe3d08fc82990c6eb9228e2ed43f0767bdb38d313a1e04217fe5d543f7efc7539437d197666e80462332525
```

### `dpkg` source package: `gcc-7=7.5.0-3ubuntu1~18.04`

Binary Packages:

- `cpp-7=7.5.0-3ubuntu1~18.04`
- `g++-7=7.5.0-3ubuntu1~18.04`
- `gcc-7=7.5.0-3ubuntu1~18.04`
- `gcc-7-base:amd64=7.5.0-3ubuntu1~18.04`
- `libasan4:amd64=7.5.0-3ubuntu1~18.04`
- `libcilkrts5:amd64=7.5.0-3ubuntu1~18.04`
- `libgcc-7-dev:amd64=7.5.0-3ubuntu1~18.04`
- `libstdc++-7-dev:amd64=7.5.0-3ubuntu1~18.04`
- `libubsan0:amd64=7.5.0-3ubuntu1~18.04`

Licenses: (parsed from: `/usr/share/doc/cpp-7/copyright`, `/usr/share/doc/g++-7/copyright`, `/usr/share/doc/gcc-7/copyright`, `/usr/share/doc/gcc-7-base/copyright`, `/usr/share/doc/libasan4/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-7-dev/copyright`, `/usr/share/doc/libstdc++-7-dev/copyright`, `/usr/share/doc/libubsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-7=7.5.0-3ubuntu1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0-3ubuntu1~18.04.dsc' gcc-7_7.5.0-3ubuntu1~18.04.dsc 28071 SHA512:1c06ed6e3fb7d3799aaad1915e318597a90ec87ec513d6710157cdf3ce877e15989ea62b70e9b6d6a06c9e24ded1174d87621d01e025797b50d13347126dc3ec
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0.orig.tar.gz' gcc-7_7.5.0.orig.tar.gz 73877115 SHA512:806470ea2d8f69a8d7eed14e38d50ea58b7cb6b8da1bd91fecf15f2f840d67f321fb9602f2c25d44f13df12f80a4f8e2dbe4450d482ae876e3678f69a93dd2d8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-7/gcc-7_7.5.0-3ubuntu1~18.04.diff.gz' gcc-7_7.5.0-3ubuntu1~18.04.diff.gz 574614 SHA512:030ab7a7894d9af4ce280556bbfd90a695d6d9fc0814f768184dc0cccfb243015f35afc85b97b92a2e1fc7054872b5d59f9fddeb65ca057cbbb3ad2a17935e98
```

### `dpkg` source package: `gcc-8=8.4.0-1ubuntu1~18.04`

Binary Packages:

- `gcc-8-base:amd64=8.4.0-1ubuntu1~18.04`
- `libatomic1:amd64=8.4.0-1ubuntu1~18.04`
- `libcc1-0:amd64=8.4.0-1ubuntu1~18.04`
- `libgcc1:amd64=1:8.4.0-1ubuntu1~18.04`
- `libgomp1:amd64=8.4.0-1ubuntu1~18.04`
- `libitm1:amd64=8.4.0-1ubuntu1~18.04`
- `liblsan0:amd64=8.4.0-1ubuntu1~18.04`
- `libmpx2:amd64=8.4.0-1ubuntu1~18.04`
- `libquadmath0:amd64=8.4.0-1ubuntu1~18.04`
- `libstdc++6:amd64=8.4.0-1ubuntu1~18.04`
- `libtsan0:amd64=8.4.0-1ubuntu1~18.04`

Licenses: (parsed from: `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc1/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libmpx2/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-8=8.4.0-1ubuntu1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.dsc' gcc-8_8.4.0-1ubuntu1~18.04.dsc 36382 SHA512:064409c787f62bff87a494f2952f5c3f264d5a7c8508c83b863c1a1ad410d25988cfc73afde9908221258f81714164121cc1f02e3699ca2283c6a3aa035d1ddd
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0.orig.tar.gz' gcc-8_8.4.0.orig.tar.gz 85278215 SHA512:ce6ff302ab2e252950bc446bc2b58c198c4b1a75d59122c00845c026a29068f412e0d59cd6ddd8b648838f80589252a1695afc6193fb669082c9a1c4ad14b1dc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-8/gcc-8_8.4.0-1ubuntu1~18.04.diff.gz' gcc-8_8.4.0-1ubuntu1~18.04.diff.gz 510634 SHA512:7bd97a04eccd35c3483a82b238d8d54c91071c4d1361cb30fb3fbf7b512c84b9d0bc80499373f2da3e17520d112125ebfebae6b93746feede78f9eecc1ccd4ac
```

### `dpkg` source package: `gcc-defaults=1.176ubuntu2.3`

Binary Packages:

- `cpp=4:7.4.0-1ubuntu2.3`
- `g++=4:7.4.0-1ubuntu2.3`
- `gcc=4:7.4.0-1ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.176ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.176ubuntu2.3.dsc' gcc-defaults_1.176ubuntu2.3.dsc 15463 SHA512:77af785110200dbe6c83c7dc8f1a1e3665c5c05a8cc0a03254936fd42c7ac725d3530b4075a98aadc071050319bfe534f38901b43ba6dccc38c6f19b6514503f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.176ubuntu2.3.tar.gz' gcc-defaults_1.176ubuntu2.3.tar.gz 208597 SHA512:586932097826c71bf94d0a8506d823ff894aae9c1a1053bc71ad8a4cf5101221b058ded1f1ad019e2111ddee13e7cfe8ce197193d770dd8c80eb40d41126cd17
```

### `dpkg` source package: `gdbm=1.14.1-6`

Binary Packages:

- `libgdbm-compat4:amd64=1.14.1-6`
- `libgdbm-dev:amd64=1.14.1-6`
- `libgdbm5:amd64=1.14.1-6`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm5/copyright`)

- `GFDL-1.3+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.14.1-6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1-6.dsc' gdbm_1.14.1-6.dsc 2293 SHA256:85fc353e81fc54b49d9c13c71f4247836fb1aac2693e98416a6821de8cfe7b41
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1.orig.tar.gz' gdbm_1.14.1.orig.tar.gz 894412 SHA256:cdceff00ffe014495bed3aed71c7910aa88bf29379f795abc0f46d4ee5f8bc5f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.14.1-6.debian.tar.xz' gdbm_1.14.1-6.debian.tar.xz 27492 SHA256:c9da59f11d5e40ecd877f1256c53ea4750b9d614c7885800e42d0f1885996658
```

### `dpkg` source package: `gdk-pixbuf=2.36.11-2`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.36.11-2`
- `libgdk-pixbuf2.0-0:amd64=2.36.11-2`
- `libgdk-pixbuf2.0-common=2.36.11-2`
- `libgdk-pixbuf2.0-dev=2.36.11-2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1-or-LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.36.11-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.11-2.dsc' gdk-pixbuf_2.36.11-2.dsc 2886 SHA256:6c6482b64d3b15bf893d6b3dc1864ab49f92ee994736d53ce84a3d052d57e6c4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.11.orig.tar.xz' gdk-pixbuf_2.36.11.orig.tar.xz 5675908 SHA256:ae62ab87250413156ed72ef756347b10208c00e76b222d82d9ed361ed9dde2f3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.36.11-2.debian.tar.xz' gdk-pixbuf_2.36.11-2.debian.tar.xz 15204 SHA256:064020524e80e3ac713dd6bdf861660df26c61d9aceb75be74df44a9979c0a0c
```

### `dpkg` source package: `git=1:2.17.1-1ubuntu0.7`

Binary Packages:

- `git=1:2.17.1-1ubuntu0.7`
- `git-man=1:2.17.1-1ubuntu0.7`

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
$ apt-get source -qq --print-uris git=1:2.17.1-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.17.1-1ubuntu0.7.dsc' git_2.17.1-1ubuntu0.7.dsc 2959 SHA512:bf9e014f7a07a501bdf4116ccd1d16a5144e0c4ef6d5f71da00a0123506b0da1fa682aec42e17d5e33add47af98966d441e0e7480759705261ed09acd3f13593
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.17.1.orig.tar.xz' git_2.17.1.orig.tar.xz 5015484 SHA512:77c27569d40fbae1842130baa0cdda674a02e384631bd8fb1f2ddf67ce372dd4903b2ce6b4283a4ae506cdedd5daa55baa2afe6a6689528511e24e4beb864960
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.17.1-1ubuntu0.7.debian.tar.xz' git_2.17.1-1ubuntu0.7.debian.tar.xz 614088 SHA512:4d72c074e39f5e06bccbfcdc3f79a2d503df1cfa6bb2db75bac092eefa95155c7bd1cc393076c176be5a18c169bdb22d31fbfa5b5f072b97a21d1ec9473780e5
```

### `dpkg` source package: `glib2.0=2.56.4-0ubuntu0.18.04.6`

Binary Packages:

- `libglib2.0-0:amd64=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-bin=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-data=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-dev:amd64=2.56.4-0ubuntu0.18.04.6`
- `libglib2.0-dev-bin=2.56.4-0ubuntu0.18.04.6`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`, `/usr/share/doc/libglib2.0-dev-bin/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.56.4-0ubuntu0.18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.dsc' glib2.0_2.56.4-0ubuntu0.18.04.6.dsc 3301 SHA512:aaa2f39144ca99225e255627f292d598d3d58ebffcbbcd2d7685a4993f342273d6b301b6b5f26651944d22b41e563e681d5daf23d1a6cf5fb74b39237132ebad
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4.orig.tar.xz' glib2.0_2.56.4.orig.tar.xz 7029768 SHA512:280a46c2af13283a08c15ff0b4f5492659c2884521930600ad45310ed181c44a878ad8f9b36bae68ed6e7d92db6f1630f7bf015148c513dc317d25807f13abb0
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz' glib2.0_2.56.4-0ubuntu0.18.04.6.debian.tar.xz 89540 SHA512:ac9961d3070de87950006fc67a455fbb9b48172389b86097ee2038a7cbd89bc1ea9a4149b86c66816f489dac29dbbd4a7a020d3f6ee4b9b112185b3322e197c2
```

### `dpkg` source package: `glibc=2.27-3ubuntu1.3`

Binary Packages:

- `libc-bin=2.27-3ubuntu1.3`
- `libc-dev-bin=2.27-3ubuntu1.3`
- `libc6:amd64=2.27-3ubuntu1.3`
- `libc6-dev:amd64=2.27-3ubuntu1.3`
- `multiarch-support=2.27-3ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.27-3ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.3.dsc' glibc_2.27-3ubuntu1.3.dsc 9612 SHA512:6ec933fbb36d3a57963f660c9563b022f809fd7a1fbde7a40bb9aff1b1c3e15a4e2afe4c039475a7f40ffd668023b71011ab788f45f5cbf4e0eed48992f34942
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27.orig.tar.xz' glibc_2.27.orig.tar.xz 15923832 SHA512:a0580fb52bc4ea8bb6e6734086b0dc66bd661060cdd837965880b989866490063c2420f250fb19b54e3547c58a5a7f8e012699e6513ce413746fd236ddd239e8
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.27-3ubuntu1.3.debian.tar.xz' glibc_2.27-3ubuntu1.3.debian.tar.xz 1091232 SHA512:af39aa3f6a8d464e294f4cdcd7d5ee068ab34a8b7f6664e6e291da30259c32af686e5d8b374504f2407db6b5b86a90f2219a010061bebe962e2d76857072b384
```

### `dpkg` source package: `gmp=2:6.1.2+dfsg-2`

Binary Packages:

- `libgmp-dev:amd64=2:6.1.2+dfsg-2`
- `libgmp10:amd64=2:6.1.2+dfsg-2`
- `libgmpxx4ldbl:amd64=2:6.1.2+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.2+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-2.dsc' gmp_6.1.2+dfsg-2.dsc 2152 SHA256:d1e7b69c619c2d07b3eaf9f051159cde1884cf9c68109f1dee278bf7a59b632b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg.orig.tar.xz' gmp_6.1.2+dfsg.orig.tar.xz 1804424 SHA256:18016f718f621e7641ddd4e57f8e140391c5183252e5998263ffff59198a65b7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.2+dfsg-2.debian.tar.xz' gmp_6.1.2+dfsg-2.debian.tar.xz 20744 SHA256:33cf6cc65827c9df744e4e07b216ca2d02eb57327a949f80a7b7dddd0485ee85
```

### `dpkg` source package: `gnupg2=2.2.4-1ubuntu1.3`

Binary Packages:

- `dirmngr=2.2.4-1ubuntu1.3`
- `gnupg=2.2.4-1ubuntu1.3`
- `gnupg-l10n=2.2.4-1ubuntu1.3`
- `gnupg-utils=2.2.4-1ubuntu1.3`
- `gpg=2.2.4-1ubuntu1.3`
- `gpg-agent=2.2.4-1ubuntu1.3`
- `gpg-wks-client=2.2.4-1ubuntu1.3`
- `gpg-wks-server=2.2.4-1ubuntu1.3`
- `gpgconf=2.2.4-1ubuntu1.3`
- `gpgsm=2.2.4-1ubuntu1.3`
- `gpgv=2.2.4-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-l10n/copyright`, `/usr/share/doc/gnupg-utils/copyright`, `/usr/share/doc/gpg/copyright`, `/usr/share/doc/gpg-agent/copyright`, `/usr/share/doc/gpg-wks-client/copyright`, `/usr/share/doc/gpg-wks-server/copyright`, `/usr/share/doc/gpgconf/copyright`, `/usr/share/doc/gpgsm/copyright`, `/usr/share/doc/gpgv/copyright`)

- `BSD-3-clause`
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
$ apt-get source -qq --print-uris gnupg2=2.2.4-1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4-1ubuntu1.3.dsc' gnupg2_2.2.4-1ubuntu1.3.dsc 3816 SHA512:3efcaaf8b3c15d75f160447fef982d6ada0b13ef97622a61b7f10d8990dc6dda9d38667e7f80cb8d895a90b00bf118f3b795c36084d68c981f766df76dd1f45e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4.orig.tar.bz2' gnupg2_2.2.4.orig.tar.bz2 6571487 SHA512:3d5c93b7662433103e9549d066a6b1a0c09d595851fab712d2ee844a55157e952a8a2dd5deff70fa8dd6817481f81c3fe5135603bca03206857310d04c1067a8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4.orig.tar.bz2.asc' gnupg2_2.2.4.orig.tar.bz2.asc 952 SHA512:85c60b8ff5f7d307d5b741e446915ea067804ad27b4a4b779fbafc11800b0cfb2a94d956b502164a3781b5ad2807434215a3413b913ce22d656838163dc1dabb
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.4-1ubuntu1.3.debian.tar.bz2' gnupg2_2.2.4-1ubuntu1.3.debian.tar.bz2 85796 SHA512:76e34e17b0df0647a60a7216ebc5d9f7a6ad6d35165514cc7fbffe579668e78ce152449eb460a462e2522d2d3b5c06f9681da9686ba31ffe115917e4818030df
```

### `dpkg` source package: `gnutls28=3.5.18-1ubuntu1.4`

Binary Packages:

- `libgnutls30:amd64=3.5.18-1ubuntu1.4`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The MIT License (MIT)`
- `The main library is licensed under GNU Lesser`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.5.18-1ubuntu1.4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.dsc' gnutls28_3.5.18-1ubuntu1.4.dsc 2780 SHA512:e8a0d6c2b9ba082f3019e6d287d0734dd26b2f5bd624b6a7a80d46c62a146fff2663124ed3f722d9acd694bd7044fc902bccbd7f7cadff4a0b2aa25fdf272bfd
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz' gnutls28_3.5.18.orig.tar.xz 7261980 SHA512:434cf33a4221fe2edce1b531cb53690d14a0991cb2056006021f625fb018987351f8ec917c3a7803e5e64179cf1647a3002ae783736ffca3188d2d294b76df52
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18.orig.tar.xz.asc' gnutls28_3.5.18.orig.tar.xz.asc 534 SHA512:c5716fed2d87b88690194cef3aa6ad6674162c77ea6bd536dcff7c32dafe66304d4d2d8cefecf9ee709cf0fae8dae40e9e71dc2c69fd55abf8a15fb6cee52950
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz' gnutls28_3.5.18-1ubuntu1.4.debian.tar.xz 83784 SHA512:807eb86a8c91caf999fc6ffe98b522d44926792d0252a18f220052455c7e4c1b321c03c6e2be355cc87b19ec34abb6206ea2af5cd147ad7d2a5b4e541c0c2339
```

### `dpkg` source package: `gobject-introspection=1.56.1-1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.56.1-1`
- `gir1.2-glib-2.0:amd64=1.56.1-1`
- `libgirepository-1.0-1:amd64=1.56.1-1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.56.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.56.1-1.dsc' gobject-introspection_1.56.1-1.dsc 2915 SHA256:978c16c9988d7bc6fed4f112012d9027d5add7e783d405057c4757e8d377a5a5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.56.1.orig.tar.xz' gobject-introspection_1.56.1.orig.tar.xz 1397812 SHA256:5b2875ccff99ff7baab63a34b67f8c920def240e178ff50add809e267d9ea24b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.56.1-1.debian.tar.xz' gobject-introspection_1.56.1-1.debian.tar.xz 20460 SHA256:20fb97a39c69106ab3b008b31e0409bc6de47989a888004c24dba64397151d86
```

### `dpkg` source package: `graphite2=1.3.11-2`

Binary Packages:

- `libgraphite2-3:amd64=1.3.11-2`
- `libgraphite2-dev:amd64=1.3.11-2`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`, `/usr/share/doc/libgraphite2-dev/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-2.1+ `
- `MPL-1.1`
- `custom-sil-open-font-license`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.11-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11-2.dsc' graphite2_1.3.11-2.dsc 2367 SHA256:3c2f5ed2b6021e9a18456215d5d01354434f14577dbc862f7f53c8ce62200d71
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11.orig.tar.gz' graphite2_1.3.11.orig.tar.gz 4236768 SHA256:945c01d3647b355d68e5541773fc99a7f29ede6a264bcbd735156a7c493459ff
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.11-2.debian.tar.xz' graphite2_1.3.11-2.debian.tar.xz 14068 SHA256:c47ef4ae6edfa6ce02483f347e67786b0fce089515087370ccc10f22ad711f90
```

### `dpkg` source package: `grep=3.1-2build1`

Binary Packages:

- `grep=3.1-2build1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.dsc' grep_3.1-2build1.dsc 2116 SHA512:420de2689ce397d7ae7cfa80bb3f2285445325269f649c387cd265770ba8ea6c0d7a87b5f40d86f88959f807ed77a5dffd6ebf2abdddf05c5c5653df3c6a1232
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1.orig.tar.xz' grep_3.1.orig.tar.xz 1370880 SHA512:05494381c7dd8aad7e2ee4c17450de8d7b969a99dcfe17747db60df3475bf02d5323d091e896e8343e4f3251c29dc7f0b7a9f93c575c9d58ee2a57014c2c9d26
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.1-2build1.debian.tar.bz2' grep_3.1-2build1.debian.tar.bz2 110087 SHA512:ca29a8001c406a2914a9edc1859f2615abc08dc1c8c8a42e48036844ee6249436dba7a43f5e5c078cb44605d620cd0d93904c92178acf73b42cb6faf416be310
```

### `dpkg` source package: `gzip=1.6-5ubuntu1`

Binary Packages:

- `gzip=1.6-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-5ubuntu1.dsc' gzip_1.6-5ubuntu1.dsc 2023 SHA256:439e340fce084b9b30e22a5537712f9b4727a20e77952addeea7633a4e9ef073
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-5ubuntu1.debian.tar.xz' gzip_1.6-5ubuntu1.debian.tar.xz 15516 SHA256:db01e3f2195cf0ebcf43ad38d07a70059b6b5b292706f2412de34928b9146db5
```

### `dpkg` source package: `harfbuzz=1.7.2-1ubuntu1`

Binary Packages:

- `gir1.2-harfbuzz-0.0:amd64=1.7.2-1ubuntu1`
- `libharfbuzz-dev:amd64=1.7.2-1ubuntu1`
- `libharfbuzz-gobject0:amd64=1.7.2-1ubuntu1`
- `libharfbuzz-icu0:amd64=1.7.2-1ubuntu1`
- `libharfbuzz0b:amd64=1.7.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-harfbuzz-0.0/copyright`, `/usr/share/doc/libharfbuzz-dev/copyright`, `/usr/share/doc/libharfbuzz-gobject0/copyright`, `/usr/share/doc/libharfbuzz-icu0/copyright`, `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=1.7.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2-1ubuntu1.dsc' harfbuzz_1.7.2-1ubuntu1.dsc 2825 SHA256:0222317c07eecbb164a537694dcb01ff4c658a56e577f9667cbb8ec144d287fa
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2.orig.tar.bz2' harfbuzz_1.7.2.orig.tar.bz2 1708416 SHA256:a790585e35c1a87f0dcc23580c84b7cc2324e6f67a2946178d278c2a36c790cb
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.7.2-1ubuntu1.debian.tar.xz' harfbuzz_1.7.2-1ubuntu1.debian.tar.xz 9168 SHA256:f94a2a0990fd0b39fdef14444fa39b0bd1d15f6c79e74b697856ba2cef06b0bf
```

### `dpkg` source package: `heimdal=7.5.0+dfsg-1`

Binary Packages:

- `libasn1-8-heimdal:amd64=7.5.0+dfsg-1`
- `libgssapi3-heimdal:amd64=7.5.0+dfsg-1`
- `libhcrypto4-heimdal:amd64=7.5.0+dfsg-1`
- `libheimbase1-heimdal:amd64=7.5.0+dfsg-1`
- `libheimntlm0-heimdal:amd64=7.5.0+dfsg-1`
- `libhx509-5-heimdal:amd64=7.5.0+dfsg-1`
- `libkrb5-26-heimdal:amd64=7.5.0+dfsg-1`
- `libroken18-heimdal:amd64=7.5.0+dfsg-1`
- `libwind0-heimdal:amd64=7.5.0+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libasn1-8-heimdal/copyright`, `/usr/share/doc/libgssapi3-heimdal/copyright`, `/usr/share/doc/libhcrypto4-heimdal/copyright`, `/usr/share/doc/libheimbase1-heimdal/copyright`, `/usr/share/doc/libheimntlm0-heimdal/copyright`, `/usr/share/doc/libhx509-5-heimdal/copyright`, `/usr/share/doc/libkrb5-26-heimdal/copyright`, `/usr/share/doc/libroken18-heimdal/copyright`, `/usr/share/doc/libwind0-heimdal/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `custom`
- `none`

Source:

```console
$ apt-get source -qq --print-uris heimdal=7.5.0+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-1.dsc' heimdal_7.5.0+dfsg-1.dsc 3674 SHA256:98ce6bf21ac01400ec10a3620fe3c047da4cf63269f521ba96c59bbcaed822bf
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg.orig.tar.gz' heimdal_7.5.0+dfsg.orig.tar.gz 8955005 SHA256:489119b7a1a900b88163765654dc59cba9a321b078fafc76629e2b85ef140867
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.5.0+dfsg-1.debian.tar.xz' heimdal_7.5.0+dfsg-1.debian.tar.xz 125776 SHA256:7ad6c3f3968989ff06181409e1515a3feaf5a630d27ade7f2f018c9241f8c225
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
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.dsc' hicolor-icon-theme_0.17-2.dsc 2053 SHA256:9df02b466f82cd6fa13930bc197d001ed8ddac1abc7f8dde3db45ed1708336bd
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17.orig.tar.xz' hicolor-icon-theme_0.17.orig.tar.xz 53016 SHA256:317484352271d18cbbcfac3868eab798d67fff1b8402e740baa6ff41d588a9d8
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.17-2.debian.tar.xz' hicolor-icon-theme_0.17-2.debian.tar.xz 3536 SHA256:97eec9852a2923b95bd13fc59c30fb1b9063ffd1f8a04748544d4975a84e98f2
```

### `dpkg` source package: `hostname=3.20`

Binary Packages:

- `hostname=3.20`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.20
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.20.dsc' hostname_3.20.dsc 1429 SHA256:1fd7b0b2b61e58aa0e50de4d375072c938cb3cc4b722bc73e085e3a3691d9114
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.20.tar.gz' hostname_3.20.tar.gz 13336 SHA256:e7ed56f8c532573ff34d9bd6e7a10d04fbbb2c7fae187898805868e5fed24ab0
```

### `dpkg` source package: `icu-le-hb=1.0.3+git161113-4`

Binary Packages:

- `libicu-le-hb-dev:amd64=1.0.3+git161113-4`
- `libicu-le-hb0:amd64=1.0.3+git161113-4`

Licenses: (parsed from: `/usr/share/doc/libicu-le-hb-dev/copyright`, `/usr/share/doc/libicu-le-hb0/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu-le-hb=1.0.3+git161113-4
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu-le-hb/icu-le-hb_1.0.3+git161113-4.dsc' icu-le-hb_1.0.3+git161113-4.dsc 1929 SHA256:e486c93a9795a26347607ea19ad2ca97e043b6de3dcbbc8bf70b0826d740ed50
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu-le-hb/icu-le-hb_1.0.3+git161113.orig.tar.xz' icu-le-hb_1.0.3+git161113.orig.tar.xz 31460 SHA256:777cdb6fecedb6400cab85894a8407bb70771e38a0e99b837ccf9e4a55f8578c
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu-le-hb/icu-le-hb_1.0.3+git161113-4.debian.tar.xz' icu-le-hb_1.0.3+git161113-4.debian.tar.xz 3176 SHA256:e140404464ff5c26af2f7f2f974cb4447e833a64f4529e85564ad367fb483ee5
```

### `dpkg` source package: `icu=60.2-3ubuntu3.1`

Binary Packages:

- `icu-devtools=60.2-3ubuntu3.1`
- `libicu-dev=60.2-3ubuntu3.1`
- `libicu60:amd64=60.2-3ubuntu3.1`
- `libiculx60:amd64=60.2-3ubuntu3.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=60.2-3ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.dsc' icu_60.2-3ubuntu3.1.dsc 2149 SHA512:dc8e59c858c31923068bae1982c390bc5175bcc3fd01510d777fb964a795e327ae350db4bb3929c6dfb68ddebb54227fc7f48ab645b880691b82f52e96993193
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2.orig.tar.gz' icu_60.2.orig.tar.gz 23315541 SHA512:ecbd9eea199d261d5f2b262abab6b1f3ee4e993081faca1426046b4ed2eadbb082fca3ebdeff82f6b431eafa7ddbe764fe64f9d96bf96486d1aa51cdc4c3d8b2
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_60.2-3ubuntu3.1.debian.tar.xz' icu_60.2-3ubuntu3.1.debian.tar.xz 29068 SHA512:cc5504e882078d5acc217d948d5ce31609e41f08dd20ea73cff1e1e775571710971d51f4d010d273c63b8068eb0edbf2657b9454fa0cb9628bcac1484ce7a762
```

### `dpkg` source package: `ilmbase=2.2.0-11ubuntu2`

Binary Packages:

- `libilmbase-dev=2.2.0-11ubuntu2`
- `libilmbase12:amd64=2.2.0-11ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libilmbase-dev/copyright`, `/usr/share/doc/libilmbase12/copyright`)

- `boost`
- `ilmbase`

Source:

```console
$ apt-get source -qq --print-uris ilmbase=2.2.0-11ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.0-11ubuntu2.dsc' ilmbase_2.2.0-11ubuntu2.dsc 2099 SHA256:894cddbe71ecaa8be9d1a348962270882dbe6c339f65e6b702db2fa07d4c9c2d
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.0.orig.tar.gz' ilmbase_2.2.0.orig.tar.gz 525289 SHA256:ecf815b60695555c1fbc73679e84c7c9902f4e8faa6e8000d2f905b8b86cedc7
'http://archive.ubuntu.com/ubuntu/pool/main/i/ilmbase/ilmbase_2.2.0-11ubuntu2.debian.tar.xz' ilmbase_2.2.0-11ubuntu2.debian.tar.xz 13400 SHA256:400b77a32f7a04d78ff0462f32dc1e4073f5e1225ed070c63fa6a0ec619905c5
```

### `dpkg` source package: `imagemagick=8:6.9.7.4+dfsg-16ubuntu6.8`

Binary Packages:

- `imagemagick=8:6.9.7.4+dfsg-16ubuntu6.8`
- `imagemagick-6-common=8:6.9.7.4+dfsg-16ubuntu6.8`
- `imagemagick-6.q16=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-6-arch-config:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-6-headers=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-6.q16-3:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-6.q16-3-extra:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-6.q16-dev:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickcore-dev=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickwand-6-headers=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickwand-6.q16-3:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickwand-6.q16-dev:amd64=8:6.9.7.4+dfsg-16ubuntu6.8`
- `libmagickwand-dev=8:6.9.7.4+dfsg-16ubuntu6.8`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6-common/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/libmagickcore-6-arch-config/copyright`, `/usr/share/doc/libmagickcore-6-headers/copyright`, `/usr/share/doc/libmagickcore-6.q16-3/copyright`, `/usr/share/doc/libmagickcore-6.q16-3-extra/copyright`, `/usr/share/doc/libmagickcore-6.q16-dev/copyright`, `/usr/share/doc/libmagickcore-dev/copyright`, `/usr/share/doc/libmagickwand-6-headers/copyright`, `/usr/share/doc/libmagickwand-6.q16-3/copyright`, `/usr/share/doc/libmagickwand-6.q16-dev/copyright`, `/usr/share/doc/libmagickwand-dev/copyright`)

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
- `LGPL-3`
- `LGPL-3+`
- `Magick++`
- `Perllikelicence`
- `TatcherUlrichPublicDomain`

Source:

```console
$ apt-get source -qq --print-uris imagemagick=8:6.9.7.4+dfsg-16ubuntu6.8
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg-16ubuntu6.8.dsc' imagemagick_6.9.7.4+dfsg-16ubuntu6.8.dsc 5234 SHA512:08ac01966c6c0537abac4af44a14920e7d60d3299479e5b217d7caa4e991459a5984389ffa216bf44a3f5e2f01aa1e3909aeef0cce72134eb08b25f112bdc8f6
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg.orig.tar.xz' imagemagick_6.9.7.4+dfsg.orig.tar.xz 8929800 SHA512:c1696b80cb95f00c32079110b84df9a125730f336cca5c04caf4aeb4b2f48ba8014dfd808b8a5cef221d5be4da4ffa1472548aa6885c5f756f04db64baf6fbd3
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.9.7.4+dfsg-16ubuntu6.8.debian.tar.xz' imagemagick_6.9.7.4+dfsg-16ubuntu6.8.debian.tar.xz 303304 SHA512:ff3558d6e8fe5e965d2f89765b2b33a6b9ef4c43ad560540137df5322e7f66781fb7073116510df3ff45c4a2bbbb9e258968a4a15c5b4823e9bc4bb09db79baa
```

### `dpkg` source package: `init-system-helpers=1.51`

Binary Packages:

- `init-system-helpers=1.51`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.51
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.51.dsc' init-system-helpers_1.51.dsc 1963 SHA256:82f0e30fef2ad14c65f9c7d8ccafd43549451041fdf661dca28b963a6cef02e4
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.51.tar.xz' init-system-helpers_1.51.tar.xz 37468 SHA256:e18b28efe8df087146d9c1e4e9c25386ee1b7312f518d48a2a38469a6c661be0
```

### `dpkg` source package: `isl=0.19-1`

Binary Packages:

- `libisl19:amd64=0.19-1`

Licenses: (parsed from: `/usr/share/doc/libisl19/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.19-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19-1.dsc' isl_0.19-1.dsc 1833 SHA256:f9786677430e2ea7295c6ad9480e7e710582f84b5b850a5ddfe1f21b3d726b0f
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19.orig.tar.xz' isl_0.19.orig.tar.xz 1515156 SHA256:6d6c1aa00e2a6dfc509fa46d9a9dbe93af0c451e196a670577a148feecf6b8a5
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.19-1.debian.tar.xz' isl_0.19-1.debian.tar.xz 22388 SHA256:aa034a5700c63867aae836a1f985fccc50ccacd1abe57a2a016e076fa745feb0
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
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.dsc' jbigkit_2.1-3.1build1.dsc 2085 SHA256:fc768c7dac53f37f89c8d0a25760a29cd9afffc5cf55821f92d0d7e8f8f26e38
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1build1.debian.tar.xz' jbigkit_2.1-3.1build1.debian.tar.xz 7672 SHA256:d7151df94f409045aa4d27dab88e538398196330d1ce135b60564dbc5db0a5c4
```

### `dpkg` source package: `keyutils=1.5.9-9.2ubuntu2`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-9.2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-9.2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-9.2ubuntu2.dsc' keyutils_1.5.9-9.2ubuntu2.dsc 2237 SHA256:67cb7c4b1dadc2c0ca85286ef8f11f7e71f91b67d47fca58ecd41e1bd83271ad
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-9.2ubuntu2.debian.tar.xz' keyutils_1.5.9-9.2ubuntu2.debian.tar.xz 18492 SHA256:51706bd0d480913584d3fa8fcfe32dcf210742bb75c08e6a2d5f022748654086
```

### `dpkg` source package: `krb5=1.16-2ubuntu0.2`

Binary Packages:

- `krb5-multidev:amd64=1.16-2ubuntu0.2`
- `libgssapi-krb5-2:amd64=1.16-2ubuntu0.2`
- `libgssrpc4:amd64=1.16-2ubuntu0.2`
- `libk5crypto3:amd64=1.16-2ubuntu0.2`
- `libkadm5clnt-mit11:amd64=1.16-2ubuntu0.2`
- `libkadm5srv-mit11:amd64=1.16-2ubuntu0.2`
- `libkdb5-9:amd64=1.16-2ubuntu0.2`
- `libkrb5-3:amd64=1.16-2ubuntu0.2`
- `libkrb5-dev:amd64=1.16-2ubuntu0.2`
- `libkrb5support0:amd64=1.16-2ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit11/copyright`, `/usr/share/doc/libkadm5srv-mit11/copyright`, `/usr/share/doc/libkdb5-9/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.16-2ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.2.dsc' krb5_1.16-2ubuntu0.2.dsc 3566 SHA512:04d0fe2c659918de633560296f62b19b4f358efc714be7ce90938bdfd1d9b1c13d4de597761ef162077fb5a53b48cfa49583be0057d9c232d26736856a89dcae
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16.orig.tar.gz' krb5_1.16.orig.tar.gz 9474479 SHA512:7e162467b95dad2b6aaa11686d08a00f1cc4eb08247fca8f0e5a8bcaa5f9f7b42cdf00db69c5c6111bdf9eb8063d53cef3bb207ce5d6a287615ca10b710153f9
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.16-2ubuntu0.2.debian.tar.xz' krb5_1.16-2ubuntu0.2.debian.tar.xz 100948 SHA512:77a936bb4cbcefdecc24b9c2d45c4275b40cb363dda386f02347bc4d6668408c405a23bc795722315d4dfd77db49584d6e494235f84dc6b93db0563c749c558b
```

### `dpkg` source package: `lcms2=2.9-1ubuntu0.1`

Binary Packages:

- `liblcms2-2:amd64=2.9-1ubuntu0.1`
- `liblcms2-dev:amd64=2.9-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.9-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-1ubuntu0.1.dsc' lcms2_2.9-1ubuntu0.1.dsc 2084 SHA512:191a120e26ea97428a29c1a8a9f67f6a087315245a40f7240e93e46fb174e953530010e81f35d041615b7b4c53fb9be266890cc007aef8700db0a35e37eb7735
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9.orig.tar.gz' lcms2_2.9.orig.tar.gz 10974649 SHA512:70b1c51fa8d137d5072425e580745ff1fbf49c6e8bb1da0a8adb0647d3b7c095208793cb02de1e8d1a01363b8575fa60c61bedbff99bbec57a44228239cb00e5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.9-1ubuntu0.1.debian.tar.xz' lcms2_2.9-1ubuntu0.1.debian.tar.xz 10680 SHA512:84285b89b9b3517d07d12aaefed7e1a343dcb5123538c3bd4cb9307fbf3913a54bfc2c9f022c72af28fe781a5db451ae25c1594c8e6133abcf3d6b36b66eedd6
```

### `dpkg` source package: `libassuan=2.5.1-2`

Binary Packages:

- `libassuan0:amd64=2.5.1-2`

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
$ apt-get source -qq --print-uris libassuan=2.5.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1-2.dsc' libassuan_2.5.1-2.dsc 2215 SHA256:e954a7ef30815e62832ca4a1d2959142e264795e7ec78ba369752353135beb68
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1.orig.tar.bz2' libassuan_2.5.1.orig.tar.bz2 564857 SHA256:47f96c37b4f2aac289f0bc1bacfa8bd8b4b209a488d3d15e2229cb6cc9b26449
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.1-2.debian.tar.xz' libassuan_2.5.1-2.debian.tar.xz 15236 SHA256:4a67901dcb0e92cd40e0d5d7148ebe6f929378671df373eb68b48acb560d641f
```

### `dpkg` source package: `libbsd=0.8.7-1ubuntu0.1`

Binary Packages:

- `libbsd0:amd64=0.8.7-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
- `BSD-3-clause-Peter-Wemm`
- `BSD-3-clause-Regents`
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
$ apt-get source -qq --print-uris libbsd=0.8.7-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7-1ubuntu0.1.dsc' libbsd_0.8.7-1ubuntu0.1.dsc 2280 SHA512:a843bcd758e78f005d073a8ca8cfc2813b076851c4dccb307bf12d6870c3fc555e45e89e56d4160a630ae31d59e945f4d41170ac0a9ad9e72e021743b080ad7c
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7.orig.tar.xz' libbsd_0.8.7.orig.tar.xz 371772 SHA512:605a14eb5d33c0e45c3bd29e585ebc15832e2ed1efa9356291a0562622168da96db1a20766e9dae8910ea0c1516429f43905edc8d4f2a40a5a341a689d08fcc3
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7.orig.tar.xz.asc' libbsd_0.8.7.orig.tar.xz.asc 833 SHA512:05b65159a7fd4e256fe41df10f3cc389d84ade4e4a5a8786f8b1990951be10b33ec9fbc6cbea16ae0c44a490253511fb2cd6c23422e11e16dbf80bef7f3eb812
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.7-1ubuntu0.1.debian.tar.xz' libbsd_0.8.7-1ubuntu0.1.debian.tar.xz 16608 SHA512:ac2c3278effcba412e732a60258c011b1e6bd0ae9ab28e434fb852df35950905293bba9e2d37466dd29b943763e7e186d3145e81c22f3879b5706f2890e62a17
```

### `dpkg` source package: `libcap-ng=0.7.7-3.1`

Binary Packages:

- `libcap-ng0:amd64=0.7.7-3.1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.7-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.1.dsc' libcap-ng_0.7.7-3.1.dsc 2266 SHA256:f545d107ed3e6160b16aac09e242d1ccc054bfca76f6d70731a83c031b416f53
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7.orig.tar.gz' libcap-ng_0.7.7.orig.tar.gz 420178 SHA256:615549ce39b333f6b78baee0c0b4ef18bc726c6bf1cca123dfd89dd963f6d06b
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-3.1.debian.tar.xz' libcap-ng_0.7.7-3.1.debian.tar.xz 5432 SHA256:074bf729c3081af729e7e0fbbe3354ddecc16e045245e7d4f44003b9f1f1adc6
```

### `dpkg` source package: `libcroco=0.6.12-2`

Binary Packages:

- `libcroco3:amd64=0.6.12-2`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.12-2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.12-2.dsc' libcroco_0.6.12-2.dsc 2204 SHA256:46e81715670968edd1d71cd878a5426ea2b28513bc4975f0b1975185adb69c9e
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.12.orig.tar.xz' libcroco_0.6.12.orig.tar.xz 482028 SHA256:ddc4b5546c9fb4280a5017e2707fbd4839034ed1aba5b7d4372212f34f84f860
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.12-2.debian.tar.xz' libcroco_0.6.12-2.debian.tar.xz 8076 SHA256:038c42873794d314fb40c9d0a78c49b841b9ac8f3a947f3fee5f7928e7d155b0
```

### `dpkg` source package: `libdatrie=0.2.10-7`

Binary Packages:

- `libdatrie1:amd64=0.2.10-7`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.10-7
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-7.dsc' libdatrie_0.2.10-7.dsc 2256 SHA256:63ad3d2782cfcca0d34055a152908ad65c6b2fc84d3079b79cf90ac4924a77fb
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10.orig.tar.xz' libdatrie_0.2.10.orig.tar.xz 294380 SHA256:180eff7b0309ca19a02d5864e744185d715f021398a096fec6cf960f8ebfaa2b
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-7.debian.tar.xz' libdatrie_0.2.10-7.debian.tar.xz 8576 SHA256:0c1496995d89daacad655618e6fff5402cb6935bb5b386c54bf4dcd1cf1b8f85
```

### `dpkg` source package: `libedit=3.1-20170329-1`

Binary Packages:

- `libedit2:amd64=3.1-20170329-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20170329-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20170329-1.dsc' libedit_3.1-20170329-1.dsc 2269 SHA256:1e657cfcfbbe5c550b844f17cfeb1d8591136fa57300e6cff2b56e5a3e25ad3f
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20170329.orig.tar.gz' libedit_3.1-20170329.orig.tar.gz 508504 SHA256:91f2d90fbd2a048ff6dad7131d9a39e690fd8a8fd982a353f1333dd4017dd4be
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20170329-1.debian.tar.bz2' libedit_3.1-20170329-1.debian.tar.bz2 11267 SHA256:7dd7a23b07b082d058b7fb741d3b750b80699472e7c8efd1935a9e7c59a49a39
```

### `dpkg` source package: `liberror-perl=0.17025-1`

Binary Packages:

- `liberror-perl=0.17025-1`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL-1`
- `GPL-1+`
- `MIT/X11`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17025-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17025-1.dsc' liberror-perl_0.17025-1.dsc 2077 SHA256:994800c0123fe452ca1f1019e5bf71755c3200231d84999a31dd19be16ada41b
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17025.orig.tar.gz' liberror-perl_0.17025.orig.tar.gz 32013 SHA256:6c9f474ad3d4fe0cabff6b6be532cb1dd348245986d4a6b600ad921d5cfdefaf
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17025-1.debian.tar.xz' liberror-perl_0.17025-1.debian.tar.xz 4108 SHA256:0288dcf7eeff5cddfaf8c6bdfbe9fc170a1d333bb6d88489ca8158c929a44f76
```

### `dpkg` source package: `libevent=2.1.8-stable-4build1`

Binary Packages:

- `libevent-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-core-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-dev=2.1.8-stable-4build1`
- `libevent-extra-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-openssl-2.1-6:amd64=2.1.8-stable-4build1`
- `libevent-pthreads-2.1-6:amd64=2.1.8-stable-4build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libevent=2.1.8-stable-4build1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.8-stable-4build1.dsc' libevent_2.1.8-stable-4build1.dsc 2110 SHA256:50bb6f58ce43bfb8c0b5123bc9722167f79f71c13dcc053da0d38259a9862c4b
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.8-stable.orig.tar.gz' libevent_2.1.8-stable.orig.tar.gz 1026485 SHA256:965cc5a8bb46ce4199a47e9b2c9e1cae3b137e8356ffdad6d94d3b9069b71dc2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.8-stable-4build1.debian.tar.xz' libevent_2.1.8-stable-4build1.debian.tar.xz 12176 SHA256:bc2aaa2398fd296875ee522fbdc1ed146531cd1db9f49119f71d8cf257c51a97
```

### `dpkg` source package: `libexif=0.6.21-4ubuntu0.6`

Binary Packages:

- `libexif-dev:amd64=0.6.21-4ubuntu0.6`
- `libexif12:amd64=0.6.21-4ubuntu0.6`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.21-4ubuntu0.6
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21-4ubuntu0.6.dsc' libexif_0.6.21-4ubuntu0.6.dsc 2242 SHA512:589d9a72aedbabf34e8f3c9498b3e29cf40c96ab08315eb88e5d3f2e8f34e25bc9150beabf8182e6255f17e20969464ab88110eb4a6789dcf7b1285abf9100b7
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21.orig.tar.gz' libexif_0.6.21.orig.tar.gz 2081615 SHA512:0a1fac9460d1d91fea8d8390e335946439de44c0ec0e1fd9fa7006532c64bececd12cd622e800c8f1176092bba926a7075838944ad6b62fa07d285af6f73e9fe
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21-4ubuntu0.6.debian.tar.xz' libexif_0.6.21-4ubuntu0.6.debian.tar.xz 17900 SHA512:0fe3b58982f68fbd4a63d3c15d0797bb039fac039b5de4da68a394dba69cadb81087fb2f8fbb58d0a88fb1d47a4ea6321fd61f63929742d5472e7f7242c8eb6d
```

### `dpkg` source package: `libffi=3.2.1-8`

Binary Packages:

- `libffi-dev:amd64=3.2.1-8`
- `libffi6:amd64=3.2.1-8`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-8
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-8.dsc' libffi_3.2.1-8.dsc 1959 SHA256:a07201eb5374cfab35703a6f4c88a494bb23ece91da5481497bc25404c57eaf4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-8.debian.tar.xz' libffi_3.2.1-8.debian.tar.xz 11660 SHA256:1eb0b13e0c0fc989ed98011d18dcddf8a05af17380fe1258883761a8d16586b4
```

### `dpkg` source package: `libgcrypt20=1.8.1-4ubuntu1.2`

Binary Packages:

- `libgcrypt20:amd64=1.8.1-4ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.1-4ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.dsc' libgcrypt20_1.8.1-4ubuntu1.2.dsc 3035 SHA512:2cab68715075be201f98da207fd67354637c5a275fa4585bed5cf234b9aca50b479ed7aa4144d77005e0bc5f9680b16d364f27d57353ef5341a7327de512e705
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2' libgcrypt20_1.8.1.orig.tar.bz2 2967344 SHA512:27c9d2fd9cba5afca71d421c9299d6942463975fae0bd10d4ff42cda2d7ea213e6b73c071a40fcf23ff52a93394cc7505ab332f8a4a3321826460e471eda5b4e
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1.orig.tar.bz2.asc' libgcrypt20_1.8.1.orig.tar.bz2.asc 310 SHA512:2e03cade8815ef146ea186efcdef2be5e1a0cfae3b9f8fcd7d7f774503b93ab29dbd2b284c1ad260181419ae0fc23462762e9a5e20193f89af76ca4ea0c1bccf
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz' libgcrypt20_1.8.1-4ubuntu1.2.debian.tar.xz 33112 SHA512:7f9196009c18514110d69f457b50dc2ff296943e04f91021193f9549f67be399013cede511131ca54dd32bfa662f26569f52a850a09823a641b640b1664ff68b
```

### `dpkg` source package: `libgpg-error=1.27-6`

Binary Packages:

- `libgpg-error0:amd64=1.27-6`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.27-6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27-6.dsc' libgpg-error_1.27-6.dsc 2343 SHA256:d4cc2c1691b295f558d5b347df8a8ad2f0260cf57146180bed223b94ffacafbb
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27.orig.tar.bz2' libgpg-error_1.27.orig.tar.bz2 813060 SHA256:4f93aac6fecb7da2b92871bb9ee33032be6a87b174f54abf8ddf0911a22d29d2
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.27-6.debian.tar.xz' libgpg-error_1.27-6.debian.tar.xz 20556 SHA256:89bc57dc3df449febf037226daf1aee830455c4efa493c0e3bdeab2a48971479
```

### `dpkg` source package: `libice=2:1.0.9-2`

Binary Packages:

- `libice-dev:amd64=2:1.0.9-2`
- `libice6:amd64=2:1.0.9-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-2.dsc' libice_1.0.9-2.dsc 2130 SHA256:116595cd54be23edad0b55e1cd4bc1929f277fa5c2d00d8f187b0bc5dd39ad6c
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-2.diff.gz' libice_1.0.9-2.diff.gz 6384 SHA256:777f13e08aada3103c32a0b93a26782ca959027bcd98c2c1ddaade8f944fa40a
```

### `dpkg` source package: `libidn2=2.0.4-1.1ubuntu0.2`

Binary Packages:

- `libidn2-0:amd64=2.0.4-1.1ubuntu0.2`

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
$ apt-get source -qq --print-uris libidn2=2.0.4-1.1ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.dsc' libidn2_2.0.4-1.1ubuntu0.2.dsc 2391 SHA512:5c6d826b5994bdeb59f7d71b060643e051ed32ee0c013f638cb80cbb1fb3ad60671b20503bb47fbfabd29005bd3848a95f3bdae7b4ef6ae1d55cabfb4745fc9c
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4.orig.tar.gz' libidn2_2.0.4.orig.tar.gz 2008524 SHA512:1e51bd4b8f8907531576291f1c2a8865d17429b4105418b4c98754eb982cd1cbb3adbeab4ec0c1c561d2dba11d876c7c09e5dc5b315c55a2c24986d7a2a3b4d2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz' libidn2_2.0.4-1.1ubuntu0.2.debian.tar.xz 10290460 SHA512:b46d51758767ae8d7cc5e9fe59df28c559baac7677bfbfd6a2e51b84c29211e38a5f85ec27afd9e72ec333ea81d03ae783a03e1d8202a0f6ef52dd7bde47475f
```

### `dpkg` source package: `libjpeg-turbo=1.5.2-0ubuntu5.18.04.4`

Binary Packages:

- `libjpeg-turbo8:amd64=1.5.2-0ubuntu5.18.04.4`
- `libjpeg-turbo8-dev:amd64=1.5.2-0ubuntu5.18.04.4`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1.5.2-0ubuntu5.18.04.4
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.dsc' libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.dsc 2391 SHA512:8cefc52a722cfdb11e157edaf1afcba85a41e2b2767a0d4cb73ed50526a065da01a807bd2eebeceed19d77386a93f7470e41d8f9a5254c4be69570c8700472d5
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2.orig.tar.gz' libjpeg-turbo_1.5.2.orig.tar.gz 1657235 SHA512:c7fe5cc77e38fad33af3f10e6db961c8edf033a86c09541121f49bfa20547179760924e6d3e397f0add7030459ff3babadd3457ab2da4a40a2147dc1574aa444
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.debian.tar.xz' libjpeg-turbo_1.5.2-0ubuntu5.18.04.4.debian.tar.xz 35396 SHA512:62f1fd71a1cee7e2e196ec48ea45b3968af3f97671c0059cb77d59149efacc7846834fd12b21c6cec4d4c0ca4b4ca351386e425d6bcea682a9df060d8c887f39
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
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.dsc' libjpeg8-empty_8c-2ubuntu8.dsc 1637 SHA256:e7f575dcb3e0d462513b6f928179baa0ff1d145273934b1041b714515096b407
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg8-empty/libjpeg8-empty_8c-2ubuntu8.tar.gz' libjpeg8-empty_8c-2ubuntu8.tar.gz 1770 SHA256:48a4227e9fc70851a4f304b10624e02875bf6f4e2debfcbe4ba0dd85a3ec05c6
```

### `dpkg` source package: `libksba=1.3.5-2`

Binary Packages:

- `libksba8:amd64=1.3.5-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.3.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5-2.dsc' libksba_1.3.5-2.dsc 2526 SHA256:4fd08fd129f97ab1df86c220b88b7b2c6e4e04aa90bfd3ae364d18022256bef8
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2' libksba_1.3.5.orig.tar.bz2 620649 SHA256:41444fd7a6ff73a79ad9728f985e71c9ba8cd3e5e53358e70d5f066d35c1a340
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2.asc' libksba_1.3.5.orig.tar.bz2.asc 287 SHA256:a954b03144ee882c838853da24fd7b6868b78df72a18c71079217d968698a76f
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5-2.debian.tar.xz' libksba_1.3.5-2.debian.tar.xz 13852 SHA256:98c985bff973be1aecc702fa15887ff1e5b8de481d1dc3e99423a587754eaabd
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
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.1.dsc' liblqr_0.4.2-2.1.dsc 2095 SHA256:c54c34cd2f7470a29366eeacde2ca4859a97d684a406fb81a918b970c01d617c
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA256:d4c22373432cca749e4326cd41fce365e6ff857c0bfd7a5302b8eb34b69f0336
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.1.debian.tar.xz' liblqr_0.4.2-2.1.debian.tar.xz 5300 SHA256:284a002f1ecac63ac17b1aafbb230da9ce7bd9efe2d5b94e8cad49b607eb2564
```

### `dpkg` source package: `libmaxminddb=1.3.1-1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.3.1-1`
- `libmaxminddb0:amd64=1.3.1-1`

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
$ apt-get source -qq --print-uris libmaxminddb=1.3.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.3.1-1.dsc' libmaxminddb_1.3.1-1.dsc 2133 SHA256:3695eba088beaee7249b202b24cf72e839a73a6ec7a7d5c6242eebb28e225298
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.3.1.orig.tar.gz' libmaxminddb_1.3.1.orig.tar.gz 244429 SHA256:6c7f5303322098e3222f1c19bde33c6043514ffe1ce37b50231aa0c04cfffa17
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.3.1-1.debian.tar.xz' libmaxminddb_1.3.1-1.debian.tar.xz 5264 SHA256:0e0d1adb0cd799cee340d9e3ce6529c8f763957037b6d1958dd9ca1f4763d6cf
```

### `dpkg` source package: `libpng1.6=1.6.34-1ubuntu0.18.04.2`

Binary Packages:

- `libpng-dev:amd64=1.6.34-1ubuntu0.18.04.2`
- `libpng16-16:amd64=1.6.34-1ubuntu0.18.04.2`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.34-1ubuntu0.18.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc' libpng1.6_1.6.34-1ubuntu0.18.04.2.dsc 2362 SHA512:306827271e4b470dacd142c5b7b4c8d97561c5b2fa39ea5fc36f20bc29f6929c868a0e926179835a24569825def8a778872100b54fbbd1f4b03a817730c40238
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34.orig.tar.xz' libpng1.6_1.6.34.orig.tar.xz 997968 SHA512:89407c5abc1623faaa3992fc1e4a62def671d9a7401108dfceee895d5f16fe7030090bea89b34a36d377d8e6a5d40046886991f663ce075d1a2d31bf9eaf3c51
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng1.6/libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz' libpng1.6_1.6.34-1ubuntu0.18.04.2.debian.tar.xz 24572 SHA512:7b13f1e486f15260f90376604e92c4050ffbf9023bcca17e527b9d5cf81fffdce83301893d635049939d12608a12835f9e3cbf4321b24dbd08afc5efe8d1a50d
```

### `dpkg` source package: `libpsl=0.19.1-5build1`

Binary Packages:

- `libpsl5:amd64=0.19.1-5build1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.19.1-5build1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1-5build1.dsc' libpsl_0.19.1-5build1.dsc 2229 SHA256:cb9bcc439b8e37ee27bd3e69a8afa6dd2a59c90ba45de4d533df256f61c8a4f5
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1.orig.tar.gz' libpsl_0.19.1.orig.tar.gz 8578385 SHA256:e370181114b8ef9daf2bb6db49b1edb842335839c15a088e7ec0a35e04e9a227
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.19.1-5build1.debian.tar.xz' libpsl_0.19.1-5build1.debian.tar.xz 9860 SHA256:53285bee66ac22a25dd41f7778cc4e94ae3d61929eb6701a8064a38a964e40e2
```

### `dpkg` source package: `libpthread-stubs=0.3-4`

Binary Packages:

- `libpthread-stubs0-dev:amd64=0.3-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libpthread-stubs=0.3-4
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3-4.dsc' libpthread-stubs_0.3-4.dsc 1925 SHA256:e72310a5492e641076c199561977703947174c6acc3633073d909f6f5ab3c676
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3.orig.tar.gz' libpthread-stubs_0.3.orig.tar.gz 272939 SHA256:3031f466cf0b06de6b3ccbf2019d15c4fcf75229b7d226a711bc1885b3a82cde
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpthread-stubs/libpthread-stubs_0.3-4.diff.gz' libpthread-stubs_0.3-4.diff.gz 2413 SHA256:ce3eb8bdc0f1a4347d42c5736d056973fae46908b764a9f2be83e1bd210f2024
```

### `dpkg` source package: `librsvg=2.40.20-2ubuntu0.2`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.40.20-2ubuntu0.2`
- `librsvg2-2:amd64=2.40.20-2ubuntu0.2`
- `librsvg2-common:amd64=2.40.20-2ubuntu0.2`
- `librsvg2-dev:amd64=2.40.20-2ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.40.20-2ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20-2ubuntu0.2.dsc' librsvg_2.40.20-2ubuntu0.2.dsc 2846 SHA512:564b5017bd081092a1098d57b3841070efeab66cb1cafb83c5fdf3a33fba7e432e72f6693a4e10ca18eeb9e28f3787d7c05cf0f6fd6cb9b2c2d4e3de758428fc
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20.orig.tar.xz' librsvg_2.40.20.orig.tar.xz 1796376 SHA512:cdd8224deb4c3786e29f48ed02c32ed9dff5cb15aba574a5ef845801ad3669cfcc3eedb9d359c22213dc7a29de24c363248825adad5877c40abf73b3688ff12f
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.20-2ubuntu0.2.debian.tar.xz' librsvg_2.40.20-2ubuntu0.2.debian.tar.xz 16768 SHA512:b87308a049c4aeac87b565c48f88fab84feefb3db4c5f03f1619206ab2920993a59222ee4617d51fd04ad874e277cb00c5748539b14cbe7d9f003ccb601a5e83
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3.18.04.3`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3.18.04.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu3.18.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.dsc' libseccomp_2.4.3-1ubuntu3.18.04.3.dsc 1951 SHA512:5a16b743f8e8e0d13348e731e5a8519a8b4db4f7f933f613d4422b48f62406b8e89d6f7c83f4c12d12b665aea62f6849a09356ed4bc91c8aa949aee1516fc302
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA512:7b7af2e98493243ffe1934fefff5723b24ae9b9bdc4bf039343ee8456c15acb0ea34e81ec292a41143848272aeca794ef92ad38fc3f42c77465170cb540479ef
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.18.04.3.debian.tar.xz 27652 SHA512:22d929d8ff17b5edd9767e4c5b32e31d0c6a5fa57b39043c8a1738336ef449324516b0ea8441b2dd7d294651a3de010a71f0a8183feb7a5bda84401879a479f9
```

### `dpkg` source package: `libselinux=2.7-2build2`

Binary Packages:

- `libselinux1:amd64=2.7-2build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.7-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7-2build2.dsc' libselinux_2.7-2build2.dsc 2468 SHA256:86f2d8422230927aa3274773e2b8a9ed15cb539804c378e75515afcd28545c37
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7.orig.tar.gz' libselinux_2.7.orig.tar.gz 187574 SHA256:d0fec0769b3ad60aa7baf9b9a4b7a056827769dc2dadda0dc0eb59b3d1c18c57
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.7-2build2.debian.tar.xz' libselinux_2.7-2build2.debian.tar.xz 23176 SHA256:ef7a781c247797b66f4d68907d8dd6fec7188d0a08e2a8541437d5f7f6796105
```

### `dpkg` source package: `libsemanage=2.7-2build2`

Binary Packages:

- `libsemanage-common=2.7-2build2`
- `libsemanage1:amd64=2.7-2build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.7-2build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7-2build2.dsc' libsemanage_2.7-2build2.dsc 2555 SHA256:4454d11e7228df1e5166907867bbd1be4e6cc8b20c6834dc690fb0dcf19d1c43
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7.orig.tar.gz' libsemanage_2.7.orig.tar.gz 153465 SHA256:07e9477714ce6a4557a1fe924ea4cb06501b62d0fa0e3c0dc32a2cf47cb8d476
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.7-2build2.debian.tar.xz' libsemanage_2.7-2build2.debian.tar.xz 17136 SHA256:d6d11ecc5687baa3b07a2a2360a9cbc4b93424a9728aa17b81cd9faf13855c3a
```

### `dpkg` source package: `libsepol=2.7-1`

Binary Packages:

- `libsepol1:amd64=2.7-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7-1.dsc' libsepol_2.7-1.dsc 1814 SHA256:7de809477acd60d256eca160d5fc6986e5e65227706b1cdb23f8139bb49d2782
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7.orig.tar.gz' libsepol_2.7.orig.tar.gz 471147 SHA256:d69d3bd8ec901a3bd5adf2be2fb47fb1a685ed73066ab482e7e505371a48f9e7
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.7-1.debian.tar.xz' libsepol_2.7-1.debian.tar.xz 13944 SHA256:56b1c2b0e492b2089f23a0d7a95a260377a0e3adefc60e90c0ff6eff6be08450
```

### `dpkg` source package: `libsigsegv=2.12-1`

Binary Packages:

- `libsigsegv2:amd64=2.12-1`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.12-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-1.dsc' libsigsegv_2.12-1.dsc 2372 SHA256:f1a17e8431a3c1f5d8f69745dcaea78c4007bf463b19c6497fd9672e9e07e438
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz' libsigsegv_2.12.orig.tar.gz 451408 SHA256:3ae1af359eebaa4ffc5896a1aee3568c052c99879316a1ab57f8fe1789c390b6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz.asc' libsigsegv_2.12.orig.tar.gz.asc 2442 SHA256:1861a9a182bbb7a24a18f7e43fe0fa3eb6f6fd53780b30e01990677112694dfc
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-1.debian.tar.xz' libsigsegv_2.12-1.debian.tar.xz 8548 SHA256:b72c81bfae92575211ceeb2eb4e90453ca4393806efc7f2804df28e7641bc810
```

### `dpkg` source package: `libsm=2:1.2.2-1`

Binary Packages:

- `libsm-dev:amd64=2:1.2.2-1`
- `libsm6:amd64=2:1.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2-1.dsc' libsm_1.2.2-1.dsc 2107 SHA256:1347efa550751179c0a3f1042a9f8ae43ee0c22cf0c2283921fa83e52a68433f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2.orig.tar.gz' libsm_1.2.2.orig.tar.gz 415990 SHA256:14bb7c669ce2b8ff712fbdbf48120e3742a77edcd5e025d6b3325ed30cf120f4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsm/libsm_1.2.2-1.diff.gz' libsm_1.2.2-1.diff.gz 6183 SHA256:9848714292ead15fcc48ab2d337f2cc5fc08910abbdfaf69d3ef1b89d3fdb2d5
```

### `dpkg` source package: `libtasn1-6=4.13-2`

Binary Packages:

- `libtasn1-6:amd64=4.13-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.13-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13-2.dsc' libtasn1-6_4.13-2.dsc 2574 SHA256:8f583c0ae8568ccf7fcf66c387963ef949d644cfca56d66512a17cb91c3a44fd
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz' libtasn1-6_4.13.orig.tar.gz 1891703 SHA256:7e528e8c317ddd156230c4e31d082cd13e7ddeb7a54824be82632209550c8cca
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13.orig.tar.gz.asc' libtasn1-6_4.13.orig.tar.gz.asc 774 SHA256:90261376528edf44831d1369847088cc2fb48669860d343961daca42e674b226
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.13-2.debian.tar.xz' libtasn1-6_4.13-2.debian.tar.xz 63332 SHA256:f36a43fb898c031b6b1a5f43b35af1aea95ac164bb2b57c7f07d1c098ed9f7eb
```

### `dpkg` source package: `libthai=0.1.27-2`

Binary Packages:

- `libthai-data=0.1.27-2`
- `libthai0:amd64=0.1.27-2`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.27-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.27-2.dsc' libthai_0.1.27-2.dsc 2342 SHA256:781b3c7f53d0d743f2cedb7588c3a640aa33c437e3ebd872e018c9113d010323
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.27.orig.tar.xz' libthai_0.1.27.orig.tar.xz 410360 SHA256:1659fa1b7b1d6562102d7feb8c8c3fd94bb2dc5761ed7dbaae4f300e1c03eff6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.27-2.debian.tar.xz' libthai_0.1.27-2.debian.tar.xz 11660 SHA256:f3c469626104cc97808eab21716bff413b760fb8637976fd27a1b9f0fae64914
```

### `dpkg` source package: `libtool=2.4.6-2`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-2`
- `libltdl7:amd64=2.4.6-2`
- `libtool=2.4.6-2`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-2.dsc' libtool_2.4.6-2.dsc 2324 SHA256:caa2b9d5c32e491388d0627e2f808b6cb2f260dd1b0b9fdafc9bff957f05bb29
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-2.debian.tar.xz' libtool_2.4.6-2.debian.tar.xz 36024 SHA256:6227fb1240a90ef06855567e71ee96e4950dd53c4399348f36c1ec39367cd8ea
```

### `dpkg` source package: `libunistring=0.9.9-0ubuntu2`

Binary Packages:

- `libunistring2:amd64=0.9.9-0ubuntu2`

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
$ apt-get source -qq --print-uris libunistring=0.9.9-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.dsc' libunistring_0.9.9-0ubuntu2.dsc 2006 SHA512:c06c7a7a04dbaef582ed90334e740b70704187df303c033a6298592cdb783f1099ea9a62b787df4b5cbd504ad76f5ff112a3508fda5134b749a25c3222ac9eb1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9.orig.tar.xz' libunistring_0.9.9.orig.tar.xz 2042992 SHA512:c5f3619d0b064c0256dc9326b609cb72871c85102cd67cfc46d85f72b67c564924cd76198c6d6ab60fbf7d6f76ddcb9fbe6c8116f779ca7e24570ae84e31fea8
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.9-0ubuntu2.debian.tar.xz' libunistring_0.9.9-0ubuntu2.debian.tar.xz 40424 SHA512:e9c6f76208bef66892b584d83e68b60a05a9cf0b67b1ac10532e996a081319d110a92b440713cb9a46fc45404723a5c81420ede10af2ab8e89432c693db4e1ef
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
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.dsc' libwebp_0.6.1-2.dsc 2064 SHA256:321ee69e44f0d037d5fec47692251e35ed22c9ad0bbf0a6bf0fae990a52319f4
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1.orig.tar.gz' libwebp_0.6.1.orig.tar.gz 3554290 SHA256:a86045e3ec24704bddbaa369ca30980d6bf4f2625f4cdca03715e91f9c08bbb4
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.6.1-2.debian.tar.xz' libwebp_0.6.1-2.debian.tar.xz 9532 SHA256:5af543e277abb97f6b2c72ca0d7ce95de79108d88da383d511ef729683fa7a45
```

### `dpkg` source package: `libwmf=0.2.8.4-12`

Binary Packages:

- `libwmf-dev=0.2.8.4-12`
- `libwmf0.2-7:amd64=0.2.8.4-12`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-12
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-12.dsc' libwmf_0.2.8.4-12.dsc 2134 SHA256:cc438ea4b9f9b93d06428989e3920f6e9f1fb317e451aeecbd2b3f608dd82826
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-12.debian.tar.xz' libwmf_0.2.8.4-12.debian.tar.xz 11952 SHA256:579cc19e9199e30b1097559f031a9814f4990206487cb4c402defb68f55be1cd
```

### `dpkg` source package: `libx11=2:1.6.4-3ubuntu0.3`

Binary Packages:

- `libx11-6:amd64=2:1.6.4-3ubuntu0.3`
- `libx11-data=2:1.6.4-3ubuntu0.3`
- `libx11-dev:amd64=2:1.6.4-3ubuntu0.3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.4-3ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.4-3ubuntu0.3.dsc' libx11_1.6.4-3ubuntu0.3.dsc 2512 SHA512:30b631362563320c87a82d44cc140374b4a45beb02ddddd3856ef96d87f9f331177bc08a1da125f590fe6433ca80bf6ddd3764621c8831beaea31e1b3662d524
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.4.orig.tar.gz' libx11_1.6.4.orig.tar.gz 3095115 SHA512:253597837e9074f962aacf8d9974491b134591b18b61835f5ab14a6488fbcb15b7761b5ce8c43cfbba10db052933a582bab0fe0980e2388189d60e39a46a0107
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.4-3ubuntu0.3.diff.gz' libx11_1.6.4-3ubuntu0.3.diff.gz 49007 SHA512:2ba8f13f173a55da3433946237333c99fc5be9b3e9d9c557eebfc3a620d7a3da71d2c7f89e3c31f17e597d01cb6da978f83727ccebcc76f264fef19cf16bf738
```

### `dpkg` source package: `libxau=1:1.0.8-1ubuntu1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.8-1ubuntu1`
- `libxau6:amd64=1:1.0.8-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1ubuntu1.dsc' libxau_1.0.8-1ubuntu1.dsc 2099 SHA512:944a2481ac5927b7dd649afe7f1f88493499a4de019ac9ef6f0c94f305aedf7695de86935f02610069ef84c0bec56db66357472f773fc9807616b2f4e92f296e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA512:3bdd9c1a491f00000dd891577493803bac3f80d0e61acb28eb2bcb50b8923e6d4540ffc4422bc0f6af8a0d20c5a75d53eedbdef177c25332f970542ea440c5d9
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1ubuntu1.diff.gz' libxau_1.0.8-1ubuntu1.diff.gz 15803 SHA512:c22f2fee07349c910f3d461d1718672ee72fd37b9668e869a7d92b984a3b158034615bf64c9480b995156ef96faa66e0107db50f2fa6fcd6f56da7911bdc8dc7
```

### `dpkg` source package: `libxcb=1.13-2~ubuntu18.04`

Binary Packages:

- `libxcb-render0:amd64=1.13-2~ubuntu18.04`
- `libxcb-render0-dev:amd64=1.13-2~ubuntu18.04`
- `libxcb-shm0:amd64=1.13-2~ubuntu18.04`
- `libxcb-shm0-dev:amd64=1.13-2~ubuntu18.04`
- `libxcb1:amd64=1.13-2~ubuntu18.04`
- `libxcb1-dev:amd64=1.13-2~ubuntu18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.13-2~ubuntu18.04
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13-2~ubuntu18.04.dsc' libxcb_1.13-2~ubuntu18.04.dsc 4762 SHA512:034d032bcbbaa311b44eb0c01a7eefbf671644e3a3f8b1f5c001bf80df45120cc85ba25e8453b66a691751eebf2e21ed93af976471efa824b1d83b33a4f3769b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13.orig.tar.gz' libxcb_1.13.orig.tar.gz 632493 SHA512:28e1db6f1981bef25007c98ba28f4c2a4d285af1aadd43ced631d630abab90ade055f125d5e384b6ff1e5ef8e31a745f53a77d61d862a6e3b7a64c52b749bc02
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.13-2~ubuntu18.04.diff.gz' libxcb_1.13-2~ubuntu18.04.diff.gz 25267 SHA512:fd19a1c6a8f6ebf362e871e814455b7cc2d63ffa63f0d47cdc035a3d5bc4b4076a4dc487dfead4d40605a4fa330134eeceb0a3acfc760579de2e2380d3b97b01
```

### `dpkg` source package: `libxdmcp=1:1.1.2-3`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.2-3`
- `libxdmcp6:amd64=1:1.1.2-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.dsc' libxdmcp_1.1.2-3.dsc 2145 SHA256:f9697dca6a275aeee9a3eee9fb2d55e0f77485481e8b84efc6950fc9b1988460
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2.orig.tar.gz' libxdmcp_1.1.2.orig.tar.gz 404115 SHA256:6f7c7e491a23035a26284d247779174dedc67e34e93cc3548b648ffdb6fc57c0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.diff.gz' libxdmcp_1.1.2-3.diff.gz 18017 SHA256:5844df115c17e5ba40ac116f80373304d821c607e763ef6f40562421f5cc0cf3
```

### `dpkg` source package: `libxext=2:1.3.3-1`

Binary Packages:

- `libxext-dev:amd64=2:1.3.3-1`
- `libxext6:amd64=2:1.3.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3-1.dsc' libxext_1.3.3-1.dsc 2221 SHA256:47106df75b8f3db1e43803e8e94a2e966cd23f7daa8cfc393af739a9e33ef955
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3.orig.tar.gz' libxext_1.3.3.orig.tar.gz 468441 SHA256:eb0b88050491fef4716da4b06a4d92b4fc9e76f880d6310b2157df604342cfe5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.3-1.diff.gz' libxext_1.3.3-1.diff.gz 20763 SHA256:e294a4884eb68acbd151312cb0c973aad63268b637b15ccf1911864b7197557e
```

### `dpkg` source package: `libxml2=2.9.4+dfsg1-6.1ubuntu1.3`

Binary Packages:

- `libxml2:amd64=2.9.4+dfsg1-6.1ubuntu1.3`
- `libxml2-dev:amd64=2.9.4+dfsg1-6.1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`, `/usr/share/doc/libxml2-dev/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.4+dfsg1-6.1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.dsc 3151 SHA512:77290cb3d711257c73e68521ded224dab4d1343a39474b6ebc849cfb90890d549a7ef475b2e3b2f6a8c46f8142b3bd3ed6aff69a13bca174f9310f6f643744a5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1.orig.tar.xz' libxml2_2.9.4+dfsg1.orig.tar.xz 2446412 SHA512:c921697db38b530b1a088636cb31226bbe9df8c9e9c83316ce53770f9bd2faeef360d5f526f34e00cd778150c408e8d91b99a67a5f5030a8b279961ff9299ae5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz' libxml2_2.9.4+dfsg1-6.1ubuntu1.3.debian.tar.xz 39680 SHA512:532f5357a6ec1e2b31634166dd9ba42f6d7337a2daa743b657e2e61d325306b1857503d3e877a28417388746ecf70c4e17e9515c7709d2ccae4e1221bfa87a87
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
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.dsc' libxrender_0.9.10-1.dsc 2064 SHA256:95d6471218b44f4e60c48cea60cfb4865bbe861530add23f6c859515bee92dbd
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA256:770527cce42500790433df84ec3521e8bf095dfe5079454a92236494ab296adf
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.10-1.diff.gz' libxrender_0.9.10-1.diff.gz 15399 SHA256:ff56a0a00119383adc5f1731e86155ae5c2de069e1d059a9da1d777917430588
```

### `dpkg` source package: `libxslt=1.1.29-5ubuntu0.2`

Binary Packages:

- `libxslt1-dev:amd64=1.1.29-5ubuntu0.2`
- `libxslt1.1:amd64=1.1.29-5ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.29-5ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.dsc' libxslt_1.1.29-5ubuntu0.2.dsc 2502 SHA512:4998aeb5983f23bbbd6e93f931b0d4c29cf71ccaee8b08edf477184184fce12791389e0d465784b38855b4587efb0833b084fc1be056ce61153b77115da0e40a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29.orig.tar.gz' libxslt_1.1.29.orig.tar.gz 3428524 SHA512:a1ce555a74a9dabe65e8f64bb66e27e77760fd76940d88f2d59f58dd63ca73c8ae59f3fcbd8e76c8f92ff992fb0c09328528c20ea38ccac83e63252106bf5f31
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.29-5ubuntu0.2.debian.tar.xz' libxslt_1.1.29-5ubuntu0.2.debian.tar.xz 36520 SHA512:4edcdbc3b2cf8c35fa7e56f7b535f7685e55a88892494abf7d6720727f8ed142a29ac1db8ada894fccfee7fc75786af56e2cf8c4c5e61c1c1c1a0694846624bb
```

### `dpkg` source package: `libxt=1:1.1.5-1`

Binary Packages:

- `libxt-dev:amd64=1:1.1.5-1`
- `libxt6:amd64=1:1.1.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.1.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5-1.dsc' libxt_1.1.5-1.dsc 2109 SHA256:f44ae1393c9fd02c0b3dd03576c7b26e6c7b09de3271a87e018efadeed311639
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5.orig.tar.gz' libxt_1.1.5.orig.tar.gz 962169 SHA256:b59bee38a9935565fa49dc1bfe84cb30173e2e07e1dcdf801430d4b54eb0caa3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5-1.diff.gz' libxt_1.1.5-1.diff.gz 14462 SHA256:822fe813d1ea9213e6fde91cbb607c0b6874341dc19b77b0f6649b8be8472d82
```

### `dpkg` source package: `libyaml=0.1.7-2ubuntu3`

Binary Packages:

- `libyaml-0-2:amd64=0.1.7-2ubuntu3`
- `libyaml-dev:amd64=0.1.7-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.1.7-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.7-2ubuntu3.dsc' libyaml_0.1.7-2ubuntu3.dsc 2019 SHA256:122f3c4ddc6b6f069382587fdde2ba9ed4800b303bce92c3d11d4fee1c1c0c5c
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.7.orig.tar.gz' libyaml_0.1.7.orig.tar.gz 527518 SHA256:8088e457264a98ba451a90b8661fcb4f9d6f478f7265d48322a196cec2480729
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.7-2ubuntu3.debian.tar.xz' libyaml_0.1.7-2ubuntu3.debian.tar.xz 4288 SHA256:d1b9caa9e645c2c306417068bcdd85e56e6065d74771c15cc970652e52f8259b
```

### `dpkg` source package: `libzstd=1.3.3+dfsg-2ubuntu1.1`

Binary Packages:

- `libzstd1:amd64=1.3.3+dfsg-2ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause-with-patent-grant`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.3.3+dfsg-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.dsc' libzstd_1.3.3+dfsg-2ubuntu1.1.dsc 2390 SHA512:8b0c42432f98edf887951e95964acd710e284f0a458b9f05be1ca1428c7c4d491547ee791f0f6c3f854dea057800b716799b69eecfc42d011c6898345570e7d1
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg.orig.tar.xz' libzstd_1.3.3+dfsg.orig.tar.xz 1333584 SHA512:40f66d34247f549b6861677a520bdce722036c49bc78096981b3b6b4cbb798780c6afccaff18e843016ec7aab55b8bb3ce3ddbfb089efb5d83028058df5e755c
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz' libzstd_1.3.3+dfsg-2ubuntu1.1.debian.tar.xz 12808 SHA512:ae7a558e5ad31ac579856d0ca7f941f95ef570b8b6612249f3f932d85310d56ef7cc4deba4d7ff3a14e46fea25e1eb663b8b841ba4442aa4f7bbe3f2961c3993
```

### `dpkg` source package: `linux=4.15.0-124.127`

Binary Packages:

- `linux-libc-dev:amd64=4.15.0-124.127`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `lsb=9.20170808ubuntu1`

Binary Packages:

- `lsb-base=9.20170808ubuntu1`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20170808ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20170808ubuntu1.dsc' lsb_9.20170808ubuntu1.dsc 2126 SHA256:9b98df7b442472d172612bf6855b4dbc3cd6d5892d8073605dda786fec94af5f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20170808ubuntu1.tar.xz' lsb_9.20170808ubuntu1.tar.xz 45492 SHA256:b26bcb746e0bff05ad3e15dfbeb0ba7ea2a8d031f765a6cfa568c57d14c522c4
```

### `dpkg` source package: `lz4=0.0~r131-2ubuntu3`

Binary Packages:

- `liblz4-1:amd64=0.0~r131-2ubuntu3`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=0.0~r131-2ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu3.dsc' lz4_0.0~r131-2ubuntu3.dsc 2129 SHA256:b6f9a71053ff1414f695790833e689dc8bd4c48169b05a8df8de47edba7a7b58
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131.orig.tar.gz' lz4_0.0~r131.orig.tar.gz 133784 SHA256:9d4d00614d6b9dec3114b33d1224b6262b99ace24434c53487a0c8fd0b18cfed
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu3.debian.tar.xz' lz4_0.0~r131-2ubuntu3.debian.tar.xz 5340 SHA256:94834bac922397529ffc185f9c4c7e7a6eb1ef3bc527f3fcd26e36fc9430afa7
```

### `dpkg` source package: `lzo2=2.08-1.2`

Binary Packages:

- `liblzo2-2:amd64=2.08-1.2`

Licenses: (parsed from: `/usr/share/doc/liblzo2-2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lzo2=2.08-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.08-1.2.dsc' lzo2_2.08-1.2.dsc 1804 SHA256:09eabe81d6f631a29cc603843b27ab914704726a1400a2219cf83b1da4e72892
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.08.orig.tar.gz' lzo2_2.08.orig.tar.gz 589045 SHA256:ac1b3e4dee46febe9fd28737eb7f5692d3232ef1a01da10444394c3d47536614
'http://archive.ubuntu.com/ubuntu/pool/main/l/lzo2/lzo2_2.08-1.2.debian.tar.xz' lzo2_2.08-1.2.debian.tar.xz 5996 SHA256:5a9aa3a2432f5d4f689b24c64ea3daec7646e736da37721388ae88b670dd99bc
```

### `dpkg` source package: `m4=1.4.18-1`

Binary Packages:

- `m4=1.4.18-1`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-1.dsc' m4_1.4.18-1.dsc 1426 SHA256:83a6c5e4b94aa47634b7c988fa485155c01120c17682865e6f032de9adf1090c
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-1.debian.tar.xz' m4_1.4.18-1.debian.tar.xz 15784 SHA256:55de78acb0272fd6e2637ab933114e64eefa58ba1e97b063629453ae1e163fff
```

### `dpkg` source package: `make-dfsg=4.1-9.1ubuntu1`

Binary Packages:

- `make=4.1-9.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.1-9.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-9.1ubuntu1.dsc' make-dfsg_4.1-9.1ubuntu1.dsc 2079 SHA256:d8ca40c89cb2b808b28264b7097a001f00a517a68d5bc2657b5c5e1bbfd0ce8b
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1.orig.tar.gz' make-dfsg_4.1.orig.tar.gz 1350231 SHA256:b3ed04fb6718289e4a430afbe2df6ecba9177aad9f6d09aaf38e5409262ca8a3
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-9.1ubuntu1.diff.gz' make-dfsg_4.1-9.1ubuntu1.diff.gz 46399 SHA256:6adc229835bd4cf04cefab0767534f9e6934989413002dd5525ec557010af5e8
```

### `dpkg` source package: `mawk=1.3.3-17ubuntu3`

Binary Packages:

- `mawk=1.3.3-17ubuntu3`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu3.dsc' mawk_1.3.3-17ubuntu3.dsc 1970 SHA256:2893a0c18b75c41d480be67d5d4edb7124ed7e9b5ed643d2670aa34481f7a77c
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu3.diff.gz' mawk_1.3.3-17ubuntu3.diff.gz 64052 SHA256:d1be148525885cb1869e35514f55005b5043f3310b08c444625005a3e14c81fc
```

### `dpkg` source package: `mercurial=4.5.3-1ubuntu2.1`

Binary Packages:

- `mercurial=4.5.3-1ubuntu2.1`
- `mercurial-common=4.5.3-1ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=4.5.3-1ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.5.3-1ubuntu2.1.dsc' mercurial_4.5.3-1ubuntu2.1.dsc 2760 SHA512:5340e0fb12f2d205a327ec8ac82d61b08eed8ad37848bcba37b40b5bfc758f37a7463d88d92359073925bab19cb708883510afb6118e541e14fe76a2c84972cc
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.5.3.orig.tar.gz' mercurial_4.5.3.orig.tar.gz 5884837 SHA512:9c23ffefb0a194b5a88ee783186347c21e7d973524ba40119439702953b35b01ad6fbc32ce09ae169f1020963e92312a39321b1da3ffe06db1d44158761abbec
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.5.3.orig.tar.gz.asc' mercurial_4.5.3.orig.tar.gz.asc 833 SHA512:c34d9e3ac1a04cc8b35405828ab4d8a7c98ef775f4af5e8ac3b347b504ca608bcd66f06646aeb554688aa95f14900e1a611675aabf385efd7b322548051c25eb
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_4.5.3-1ubuntu2.1.debian.tar.xz' mercurial_4.5.3-1ubuntu2.1.debian.tar.xz 61912 SHA512:1ffee389075de0f74afc611c7e2d1f65488d4a9da9518c7f51d45c859a18af310c130db7a939bad8deefd1c55591b507a02b75eeeec46738c0e192b6cd8469b1
```

### `dpkg` source package: `mime-support=3.60ubuntu1`

Binary Packages:

- `mime-support=3.60ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.60ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.60ubuntu1.dsc' mime-support_3.60ubuntu1.dsc 1712 SHA256:1e58e26d0f87f25ebe6c08007e9d354a24457ab73d40a1eb3b9ab62ea0d366d5
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.60ubuntu1.tar.gz' mime-support_3.60ubuntu1.tar.gz 37743 SHA256:cb1bc122ac2dc7046f6c0c06146ac0897a3c1c02e7e5e53cdd30817db2c62d33
```

### `dpkg` source package: `mpclib3=1.1.0-1`

Binary Packages:

- `libmpc3:amd64=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.1.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0-1.dsc' mpclib3_1.1.0-1.dsc 1990 SHA256:bb57824015b735bf72399a53f8c6a241e6a8bd402753b0fdcdaa5b99d0aef790
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0.orig.tar.gz' mpclib3_1.1.0.orig.tar.gz 701263 SHA256:6985c538143c1208dcb1ac42cedad6ff52e267b47e5f970183a3e75125b43c2e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0-1.diff.gz' mpclib3_1.1.0-1.diff.gz 3794 SHA256:84b10a4ae958b3015e136b75be5fee22961255d19be655f7d0adae8d4f3bc977
```

### `dpkg` source package: `mpdecimal=2.4.2-1ubuntu1`

Binary Packages:

- `libmpdec2:amd64=2.4.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1ubuntu1.dsc' mpdecimal_2.4.2-1ubuntu1.dsc 2051 SHA256:6a1a2c1b839492e178d601dc6b9de26a3173124b35659ccd21362167a4fabda9
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-1ubuntu1.debian.tar.xz' mpdecimal_2.4.2-1ubuntu1.debian.tar.xz 5328 SHA256:091414d364411f1d05b496f877e04d8ad22d52441cb698d739929907e94e0fc7
```

### `dpkg` source package: `mpfr4=4.0.1-1`

Binary Packages:

- `libmpfr6:amd64=4.0.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.0.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1-1.dsc' mpfr4_4.0.1-1.dsc 1972 SHA256:85d8dad92d3f9ace96ac78b2f4ec00eafef228fa53e0344ae4255fc4d3f75626
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1.orig.tar.xz' mpfr4_4.0.1.orig.tar.xz 1412692 SHA256:67874a60826303ee2fb6affc6dc0ddd3e749e9bfcb4c8655e3953d0458a6e16e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.1-1.debian.tar.xz' mpfr4_4.0.1-1.debian.tar.xz 10460 SHA256:9e0d582dea7e88958b8bc1f3782ada59b9c7175f01b4e06e8487fc6cbfc5a2d7
```

### `dpkg` source package: `mysql-5.7=5.7.32-0ubuntu0.18.04.1`

Binary Packages:

- `libmysqlclient-dev=5.7.32-0ubuntu0.18.04.1`
- `libmysqlclient20:amd64=5.7.32-0ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libmysqlclient-dev/copyright`, `/usr/share/doc/libmysqlclient20/copyright`)

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
- `SWsoft`
- `public-domain`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris mysql-5.7=5.7.32-0ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.32-0ubuntu0.18.04.1.dsc' mysql-5.7_5.7.32-0ubuntu0.18.04.1.dsc 3446 SHA512:82d901205870bc6cc721ca13bdce003c5ec4bce58c7aa0afcdf9c8af0190883e6e88ebe3b78628ef0a94d0f5218cfbe0b66370fbbe6477745ec9b14ce5bb6721
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.32.orig.tar.gz' mysql-5.7_5.7.32.orig.tar.gz 52882168 SHA512:33a617d040efd065ea1c2ad84be537f851480abd5cc8a6879b7f170bc4e6db9432bd03f2a6bc680b71f17839c508cab0e7ef1a3aba032197da1b7943c916c77a
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-5.7/mysql-5.7_5.7.32-0ubuntu0.18.04.1.debian.tar.xz' mysql-5.7_5.7.32-0ubuntu0.18.04.1.debian.tar.xz 156432 SHA512:a2f8b486a1e95cab2e1d912fb1d96d38439aee3b63ee771f1c0770da7f46bcc081fc3f3d1083e4a1f3a15c1ab40174179dc1a47502338f4ae679c0dafc4e7df8
```

### `dpkg` source package: `mysql-defaults=1.0.4`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.4`
- `mysql-common=5.8+1.0.4`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.4.dsc' mysql-defaults_1.0.4.dsc 2213 SHA256:c0cb0ba90874c858c30cfc71ccbd078c1fb1b45fbfdc6414af75811101d6f01f
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.4.tar.xz' mysql-defaults_1.0.4.tar.xz 7084 SHA256:01b92a09aaa08fd589610c0d7cbe55e05dce64db57ff2dfa6f794bcf857e002a
```

### `dpkg` source package: `ncurses=6.1-1ubuntu1.18.04`

Binary Packages:

- `libncurses5:amd64=6.1-1ubuntu1.18.04`
- `libncurses5-dev:amd64=6.1-1ubuntu1.18.04`
- `libncursesw5:amd64=6.1-1ubuntu1.18.04`
- `libncursesw5-dev:amd64=6.1-1ubuntu1.18.04`
- `libtinfo-dev:amd64=6.1-1ubuntu1.18.04`
- `libtinfo5:amd64=6.1-1ubuntu1.18.04`
- `ncurses-base=6.1-1ubuntu1.18.04`
- `ncurses-bin=6.1-1ubuntu1.18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.1-1ubuntu1.18.04
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.dsc' ncurses_6.1-1ubuntu1.18.04.dsc 4702 SHA512:e998c05380a2599d3f37572e720ab60854a1c83bacdf921372767e320d4063c2af611d45409201dbc77e6c6b981537eec246f46326bae6a69536ddf974007ab1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz' ncurses_6.1.orig.tar.gz 3365395 SHA512:e308af43f8b7e01e98a55f4f6c4ee4d1c39ce09d95399fa555b3f0cdf5fd0db0f4c4d820b4af78a63f6cf6d8627587114a40af48cfc066134b600520808a77ee
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1.orig.tar.gz.asc' ncurses_6.1.orig.tar.gz.asc 251 SHA512:53659ddf0890683f1d9bf895d7d5b0693d95e102cde4440685a3d0c97230c4930203a9383bd9833ba4639713a12b0afd2b3ebecd9fa5640fb6f2b5fa8e662441
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.1-1ubuntu1.18.04.debian.tar.xz' ncurses_6.1-1ubuntu1.18.04.debian.tar.xz 57464 SHA512:ec0211e25ecc865296afd54eeae8314718ca2d443936e016dd74dacfaa1f1de79778b1d50fe9377488f07e40fce82ed367348db30889757efd1db4f96630a6fa
```

### `dpkg` source package: `netbase=5.4`

Binary Packages:

- `netbase=5.4`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.4
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.4.dsc' netbase_5.4.dsc 1326 SHA256:ebe29d45e65b661d64636cbce3840997d8079cf338efbfa347b4c73ed2831b7b
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.4.tar.xz' netbase_5.4.tar.xz 31524 SHA256:66ff73d2d162e2d49db43988d8b8cd328cf7fffca042db73397f14c71825e80d
```

### `dpkg` source package: `nettle=3.4-1`

Binary Packages:

- `libhogweed4:amd64=3.4-1`
- `libnettle6:amd64=3.4-1`

Licenses: (parsed from: `/usr/share/doc/libhogweed4/copyright`, `/usr/share/doc/libnettle6/copyright`)

- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1+`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4-1.dsc' nettle_3.4-1.dsc 2238 SHA256:0ceb4600fdedf43916e95fb6b354ebb4038f00f5814433582d0481b510310e86
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.orig.tar.gz' nettle_3.4.orig.tar.gz 1935069 SHA256:ae7a42df026550b85daca8389b6a60ba6313b0567f374392e54918588a411e94
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4.orig.tar.gz.asc' nettle_3.4.orig.tar.gz.asc 1238 SHA256:86d7441c7334dd95d16b1ca488fd94ec45ed6406714d4ed9887c7212e337eb2a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.4-1.debian.tar.xz' nettle_3.4-1.debian.tar.xz 19884 SHA256:9bfc25562ed36449e75741b0473e0e558bc9ef5c20ca24e7c650fea87d631c03
```

### `dpkg` source package: `nghttp2=1.30.0-1ubuntu1`

Binary Packages:

- `libnghttp2-14:amd64=1.30.0-1ubuntu1`

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
$ apt-get source -qq --print-uris nghttp2=1.30.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0-1ubuntu1.dsc' nghttp2_1.30.0-1ubuntu1.dsc 2674 SHA256:1848fdc28933b7ee23dbebe3c9dcd0ca9182f95a278d627758d5ccfa2e0b44ad
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0.orig.tar.bz2' nghttp2_1.30.0.orig.tar.bz2 1839714 SHA256:f66918dd03773f4847da1d069295c758ce478cbd1fe58298a37d65e1dce056d8
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.30.0-1ubuntu1.debian.tar.xz' nghttp2_1.30.0-1ubuntu1.debian.tar.xz 13244 SHA256:eb99f2c10cd872ce750964fc59734aa70b89ad04179291a23bfbee0e1a2903d3
```

### `dpkg` source package: `npth=1.5-3`

Binary Packages:

- `libnpth0:amd64=1.5-3`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.5-3
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5-3.dsc' npth_1.5-3.dsc 1954 SHA256:98e02623d39451685321ab638e12cd0b85f7829f6b174d03dbb806b8d899ae3f
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5.orig.tar.bz2' npth_1.5.orig.tar.bz2 299308 SHA256:294a690c1f537b92ed829d867bee537e46be93fbd60b16c04630fbbfcd9db3c2
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.5-3.debian.tar.xz' npth_1.5-3.debian.tar.xz 10480 SHA256:5cbaf91c95c90ab82053110eeec5ac72f5a3cab36829edb0579f1fb759ec5fec
```

### `dpkg` source package: `openexr=2.2.0-11.1ubuntu1.3`

Binary Packages:

- `libopenexr-dev=2.2.0-11.1ubuntu1.3`
- `libopenexr22:amd64=2.2.0-11.1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr22/copyright`)

- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.2.0-11.1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-11.1ubuntu1.3.dsc' openexr_2.2.0-11.1ubuntu1.3.dsc 2403 SHA512:425d006d15458deddb507e1b167d81effa77c0973696e81de65d480e53cc8a64df8943df132a3162b76ab54655d51855fe695258879640662f7fdf44067c0489
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0.orig.tar.gz' openexr_2.2.0.orig.tar.gz 14489661 SHA512:017abbeeb6b814508180721bc8e8940094965c4c55b135a198c6bcb109a04bf7f72e4aee81ee72cb2185fe818a41d892b383e8d2d59f40c673198948cb79279a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-11.1ubuntu1.3.debian.tar.xz' openexr_2.2.0-11.1ubuntu1.3.debian.tar.xz 30448 SHA512:69e9a7773c24cab8f63191a3fc40d9eaecaae75cf52b30aff9349400601a60c3cc9700c0959c7a710b2c2085b32cd31eca001c73f1e0b181ba5276328a6e6f41
```

### `dpkg` source package: `openldap=2.4.45+dfsg-1ubuntu1.8`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.45+dfsg-1ubuntu1.8`
- `libldap-common=2.4.45+dfsg-1ubuntu1.8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.45+dfsg-1ubuntu1.8
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg-1ubuntu1.8.dsc' openldap_2.4.45+dfsg-1ubuntu1.8.dsc 2884 SHA512:a1c1140cfe42895f9e3b70fb1c6330ba9297a8a3c055367612a56cb1cd2c442cc7455ec6cf063dd90dbc65872b66841aad9d9e4704da7ea2a02e29419426974f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg.orig.tar.gz' openldap_2.4.45+dfsg.orig.tar.gz 4846458 SHA512:fb2089aa6949ecced1d48242b203bc2f744e920ecea41559209f7d3a1cfe626c1d81e8a9234b6997b2379832d62e439ca1f674a8a06635fdaa359fc09d1b414e
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.45+dfsg-1ubuntu1.8.debian.tar.xz' openldap_2.4.45+dfsg-1ubuntu1.8.debian.tar.xz 180120 SHA512:d7b237e15595050f2309cee9cc6082a478e5d685644715fb7b7f739a9ed4a0fdcbdffc36a51b9cd2690cdffc4db6b431563ac66c87c2bed582b074c6f298b56e
```

### `dpkg` source package: `openssh=1:7.6p1-4ubuntu0.3`

Binary Packages:

- `openssh-client=1:7.6p1-4ubuntu0.3`

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
$ apt-get source -qq --print-uris openssh=1:7.6p1-4ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_7.6p1-4ubuntu0.3.dsc' openssh_7.6p1-4ubuntu0.3.dsc 3220 SHA512:0873d1711a591380e389552d9ca09b470c276b4037cf38068e2a8adfaec9b33d897602d040a55a0e71ed3f18f4e04ab036ea8d9f0710be9816f2d60871c0dc26
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_7.6p1.orig.tar.gz' openssh_7.6p1.orig.tar.gz 1489788 SHA512:de17fdcb8239401f76740c8d689a8761802f6df94e68d953f3c70b9f4f8bdb403617c48c1d01cc8c368d88e9d50aee540bf03d5a36687dfb39dfd28d73029d72
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_7.6p1.orig.tar.gz.asc' openssh_7.6p1.orig.tar.gz.asc 683 SHA512:2e98dcafc5933a2b2353b1dddc5182e2091643c6ccdb51d928e433bce7ad37cecb9b45c406975b530e859eb748c3e5c61a6d52b8e1df3d34202fafb77406ef8b
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_7.6p1-4ubuntu0.3.debian.tar.xz' openssh_7.6p1-4ubuntu0.3.debian.tar.xz 167500 SHA512:7f627306cf98fd96511c817528bba2727d88be655633486d8b6821a73e7d5e055ec7088fd155fc4b1f8db48dbe5996f299f3a33d55c2bb9f09e9fa6a3fcba301
```

### `dpkg` source package: `openssl1.0=1.0.2n-1ubuntu5.4`

Binary Packages:

- `libssl1.0.0:amd64=1.0.2n-1ubuntu5.4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl1.0=1.0.2n-1ubuntu5.4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl1.0/openssl1.0_1.0.2n-1ubuntu5.4.dsc' openssl1.0_1.0.2n-1ubuntu5.4.dsc 2713 SHA512:bfb29d59394f5fba4956668e90a7c70ee445475030e86b0c2dd236b6ead43d4afafcbc9783e812d2335a748efac0ae67093cd5df25ba0488097f880456206b5b
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl1.0/openssl1.0_1.0.2n.orig.tar.gz' openssl1.0_1.0.2n.orig.tar.gz 5375802 SHA512:144bf0d6aa27b4af01df0b7b734c39962649e1711554247d42e05e14d8945742b18745aefdba162e2dfc762b941fd7d3b2d5dc6a781ae4ba10a6f5a3cadb0687
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl1.0/openssl1.0_1.0.2n.orig.tar.gz.asc' openssl1.0_1.0.2n.orig.tar.gz.asc 455 SHA512:7a4d82d1abbfdac92f87839321a40348099fa32193e97042c1d5ff0b0ac719104e0e2b079e0669e603c98c7d2313d0e0de4c1aec0c9180eadd1dd241e7f1985a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl1.0/openssl1.0_1.0.2n-1ubuntu5.4.debian.tar.xz' openssl1.0_1.0.2n-1ubuntu5.4.debian.tar.xz 116892 SHA512:512265c5b7e6f8f2faa8ff5efd401eb1b8633166c31bbe13f827ba762058c734601843326c2f2b35ce9c2aef5cde25379475ad30cee2c107e7186dc5d66899b3
```

### `dpkg` source package: `openssl=1.1.1-1ubuntu2.1~18.04.6`

Binary Packages:

- `libssl-dev:amd64=1.1.1-1ubuntu2.1~18.04.6`
- `libssl1.1:amd64=1.1.1-1ubuntu2.1~18.04.6`
- `openssl=1.1.1-1ubuntu2.1~18.04.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1-1ubuntu2.1~18.04.6
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.dsc' openssl_1.1.1-1ubuntu2.1~18.04.6.dsc 2754 SHA512:c16af42e0bb9530125f52ec1af1cef1743de3bfa1e82c51bddf43780b0f6298ddd60fbb260d713df56fc97f46614b922bb04a45f7ed94fadca1f00bff6d55cae
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz' openssl_1.1.1.orig.tar.gz 8337920 SHA512:c0284a4fe84bdf765ca5bc5148da4441ffc36392cfecaf9d372af00cf93b6de5681cab1248b6f8246474532155dc205da5ad49549ad7c61c07c917145e7c9c71
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1.orig.tar.gz.asc' openssl_1.1.1.orig.tar.gz.asc 488 SHA512:cc69ad07a2edc17b579018bac4683f7d48deb8cde4a0f53eb777d2546eec9be6d13a610299705f3b87a7e4e8492432260cd7efc89d124c7fe1def309bbee461f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz' openssl_1.1.1-1ubuntu2.1~18.04.6.debian.tar.xz 104692 SHA512:c1945f1641cc7edc9fbf6d9a2384d2fd05442f7d1460a3d7085f90b760ff4d5578d4bd33c662effcd1b92459fee6472415672350005a784fc9eaa19b96cd2fd1
```

### `dpkg` source package: `p11-kit=0.23.9-2`

Binary Packages:

- `libp11-kit0:amd64=0.23.9-2`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9-2.dsc' p11-kit_0.23.9-2.dsc 2458 SHA256:e4c271a89abf52a95d23cca02bd6fb6ea5d5611b139ac63b0db728e7d9895449
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9.orig.tar.gz' p11-kit_0.23.9.orig.tar.gz 1091561 SHA256:e1c1649c335107a8d33cf3762eb7f57b2d0681f0c7d8353627293a58d6b4db63
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9.orig.tar.gz.asc' p11-kit_0.23.9.orig.tar.gz.asc 900 SHA256:334562f6a37f96339173a33a90b246466e0b2673e03658b205d75ebbb63bad10
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.9-2.debian.tar.xz' p11-kit_0.23.9-2.debian.tar.xz 21704 SHA256:fa6af69f96f6ccdce95d61e39662a38768b05f8872b2b2008d56cc4fff0ed3fd
```

### `dpkg` source package: `pam=1.1.8-3.6ubuntu2.18.04.2`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.6ubuntu2.18.04.2`
- `libpam-modules-bin=1.1.8-3.6ubuntu2.18.04.2`
- `libpam-runtime=1.1.8-3.6ubuntu2.18.04.2`
- `libpam0g:amd64=1.1.8-3.6ubuntu2.18.04.2`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.6ubuntu2.18.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.1.8-3.6ubuntu2.18.04.2.dsc' pam_1.1.8-3.6ubuntu2.18.04.2.dsc 2557 SHA512:244e2c6f339822de9eb5419f86d620d346ad32121b71efb673628835ac3e6c2b0eb62eb552a26a8d6647e3fc182d3e2f949725dc5c5e50329285c5c49ec5e70b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.1.8-3.6ubuntu2.18.04.2.tar.gz' pam_1.1.8-3.6ubuntu2.18.04.2.tar.gz 1991026 SHA512:12f83aabb144253d761bc3b6f96614a122b4bfafc89ec4baa0805ca50df47986e7f7b025aa79e21fcf61c9ab308983064de17ffbcbe39f4333104e6d3b7d5ff6
```

### `dpkg` source package: `pango1.0=1.40.14-1ubuntu0.1`

Binary Packages:

- `libpango-1.0-0:amd64=1.40.14-1ubuntu0.1`
- `libpangocairo-1.0-0:amd64=1.40.14-1ubuntu0.1`
- `libpangoft2-1.0-0:amd64=1.40.14-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.40.14-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14-1ubuntu0.1.dsc' pango1.0_1.40.14-1ubuntu0.1.dsc 3358 SHA512:03cd5f36dbbd14f63dd36c0fa633ee62d883897e553195c953b67986ede019bdb3a291b7d8d1e69768a83ff89acc3bb9a4a05b00a248b8a13355513811f554ac
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14.orig.tar.xz' pango1.0_1.40.14.orig.tar.xz 858388 SHA512:35ba7bc8be3992f206ccc2cc5aca0b94e2a3832f887fc9c45b0e29fddcb9051ce05a74377de0ca4ff95a87983b15688fa5d379d592faf87aa8eaca25ac18b7ea
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.40.14-1ubuntu0.1.debian.tar.xz' pango1.0_1.40.14-1ubuntu0.1.debian.tar.xz 28460 SHA512:9de609d588388be9436c3cb0cd1913a7b8eda0a5b8e7e1effd6beb4002cf7a60236cd8a52410d1c09501beddbb2d89473da3f7f56d6b2b47886c18f0561b94d4
```

### `dpkg` source package: `patch=2.7.6-2ubuntu1.1`

Binary Packages:

- `patch=2.7.6-2ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-2ubuntu1.1.dsc' patch_2.7.6-2ubuntu1.1.dsc 1798 SHA512:80fefde6e5b713944a47a40d9dec24510467249135659f987f2d544c8e83ff4acf3b4e5cbcb8fa87cbf0ae001fa66173f06a8404d2163a66578a3b41ff6a62fa
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA512:fcca87bdb67a88685a8a25597f9e015f5e60197b9a269fa350ae35a7991ed8da553939b4bbc7f7d3cfd863c67142af403b04165633acbce4339056a905e87fbd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-2ubuntu1.1.debian.tar.xz' patch_2.7.6-2ubuntu1.1.debian.tar.xz 12356 SHA512:3ba381149e7e7a7f878a6ff485c42775a8f1c8c0546cdbe9d7f9354bd1700bb884028466a9c660979b1bc0ad1e8ed9f09e50688d33d8979eee14d4bb0a65f332
```

### `dpkg` source package: `pcre3=2:8.39-9`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-9`
- `libpcre3:amd64=2:8.39-9`
- `libpcre3-dev:amd64=2:8.39-9`
- `libpcre32-3:amd64=2:8.39-9`
- `libpcrecpp0v5:amd64=2:8.39-9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-9
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-9.dsc' pcre3_8.39-9.dsc 2224 SHA256:cfbe37b2022027f62f236d74bb6af90befd2964161d77b2fd459c75ae7c36e36
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-9.debian.tar.gz' pcre3_8.39-9.debian.tar.gz 26333 SHA256:68be90799b722a8d5a075c3d2f48718cb21e2e736e0edf1e7e46a87c51215f55
```

### `dpkg` source package: `perl=5.26.1-6ubuntu0.5`

Binary Packages:

- `libperl5.26:amd64=5.26.1-6ubuntu0.5`
- `perl=5.26.1-6ubuntu0.5`
- `perl-base=5.26.1-6ubuntu0.5`
- `perl-modules-5.26=5.26.1-6ubuntu0.5`

Licenses: (parsed from: `/usr/share/doc/libperl5.26/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.26/copyright`)

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
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.26.1-6ubuntu0.5
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1-6ubuntu0.5.dsc' perl_5.26.1-6ubuntu0.5.dsc 2768 SHA512:bc90544acc5f20ce216819c617607e3ee0b9f30e1244ebcc2b52b473bea72dc2f8159d9b5945fffca1ba27ae24aa4567b24b6a2558a004a6b4c0532a9bde5a62
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1.orig-regen-configure.tar.gz' perl_5.26.1.orig-regen-configure.tar.gz 712883 SHA512:3a8ecf16483d87d40bf428e952a3f5c287af8e4f64977133b61188855120d5896b3c5af845a19ad1912f469d9345dddd728708f6171498a7fd0dd0f56b463139
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1.orig.tar.xz' perl_5.26.1.orig.tar.xz 11922848 SHA512:13faa7bcd7ed8c490c37e9032c115af06c9b8152b75f8062409dd72d263d1314480e8a9a883490de1b448b2e6d53b6a87d108e2eceb17de2524d5857c6a7d300
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.26.1-6ubuntu0.5.debian.tar.xz' perl_5.26.1-6ubuntu0.5.debian.tar.xz 179176 SHA512:0d8612be05063b50a59cad031ef6c3572f1a747295df186a24ad646b897f0e0df7ff00bd914480c094d3702f1b249d822d8262202e8d25c5ed96b9403d5e86ed
```

### `dpkg` source package: `pinentry=1.1.0-1`

Binary Packages:

- `pinentry-curses=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-1.dsc' pinentry_1.1.0-1.dsc 2910 SHA256:8cda3442923c0e18f9c3d5a2817a97a54db7447046b9c469e890abd19c680247
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2.asc' pinentry_1.1.0.orig.tar.bz2.asc 534 SHA256:0e3a7633b9fddf9c01c3dcf74aeb94888cc6d5d233f0b8357b0b9c1a1fed9a73
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-1.debian.tar.xz' pinentry_1.1.0-1.debian.tar.xz 15408 SHA256:ddee92638e762f125ac09b86b4f3b31e2d240e8d2dcce940302293bb2ea0873e
```

### `dpkg` source package: `pixman=0.34.0-2`

Binary Packages:

- `libpixman-1-0:amd64=0.34.0-2`
- `libpixman-1-dev:amd64=0.34.0-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.34.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.34.0-2.dsc' pixman_0.34.0-2.dsc 2091 SHA256:a2d9b02ea4b0255813197c2266cee166578b083815e255530aec390bbc43d15c
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.34.0.orig.tar.gz' pixman_0.34.0.orig.tar.gz 878784 SHA256:21b6b249b51c6800dc9553b65106e1e37d0e25df942c90531d4c3997aa20a88e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.34.0-2.diff.gz' pixman_0.34.0-2.diff.gz 315460 SHA256:e81ec91d58776d804a2c56cbebb8c80fa3318a45a6a7246005bc96985f7dd805
```

### `dpkg` source package: `pkg-config=0.29.1-0ubuntu2`

Binary Packages:

- `pkg-config=0.29.1-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.1-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu2.dsc' pkg-config_0.29.1-0ubuntu2.dsc 1824 SHA256:91f07d5a80083fbe86c93d9f107890920f4740df8f3d1e6b162a5d703afc3b89
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1.orig.tar.gz' pkg-config_0.29.1.orig.tar.gz 2013454 SHA256:beb43c9e064555469bd4390dcfd8030b1536e0aa103f08d7abf7ae8cac0cb001
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu2.diff.gz' pkg-config_0.29.1-0ubuntu2.diff.gz 12715 SHA256:8d5645ccad7bdbcaf3bd83b1b18c7f7d0e2a813e9813b5d4603aa646fc5ff5ea
```

### `dpkg` source package: `postgresql-10=10.15-0ubuntu0.18.04.1`

Binary Packages:

- `libpq-dev=10.15-0ubuntu0.18.04.1`
- `libpq5:amd64=10.15-0ubuntu0.18.04.1`

Licenses: (parsed from: `/usr/share/doc/libpq-dev/copyright`, `/usr/share/doc/libpq5/copyright`)

- `Artistic`
- `BSD-2-clause`
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
$ apt-get source -qq --print-uris postgresql-10=10.15-0ubuntu0.18.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-10/postgresql-10_10.15-0ubuntu0.18.04.1.dsc' postgresql-10_10.15-0ubuntu0.18.04.1.dsc 3620 SHA512:38a20a69a07a07adf0d26a58c11fbdae7f5de0d1481f2f2420328355f8d5b1c90e3a032b8a2cb2e2e2a4c8a67b45f761e69bb4b9212fcf7489c8952d5a667dd8
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-10/postgresql-10_10.15.orig.tar.bz2' postgresql-10_10.15.orig.tar.bz2 19089779 SHA512:88fe322a8691692f8c1b8ca7f7a5a035c399c1d2a0e6276b60863f2c0cb8e4857b041d7364641e0738438aee0836688e712b9c176ac454ee98386dfd18754636
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-10/postgresql-10_10.15-0ubuntu0.18.04.1.debian.tar.xz' postgresql-10_10.15-0ubuntu0.18.04.1.debian.tar.xz 35260 SHA512:63a1074e3ec915df7f1cda04c7a2dfd350f80594cd5a5156557dbde352235c779585ce110b8edcebf081c36da1426cca59583d26f2376ff41c08732a4c0447de
```

### `dpkg` source package: `procps=2:3.3.12-3ubuntu1.2`

Binary Packages:

- `libprocps6:amd64=2:3.3.12-3ubuntu1.2`
- `procps=2:3.3.12-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libprocps6/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.12-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.dsc' procps_3.3.12-3ubuntu1.2.dsc 1920 SHA512:0ba0450d7411075000e5be9f64c92c73cf9f029fac707a13ad9bba692042a70c6f5535b31793eaca31670be61408e3a49cd861a0078859c57798a991e713459b
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12.orig.tar.xz' procps_3.3.12.orig.tar.xz 840540 SHA512:cb26a6b8419cc41134ccd072e1b38919ffd7126a99055a64726dc1d55149a2278fbf84528a71388196351e5bc72e81b18ce2a4f576a111d3741971327b30e6f8
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.12-3ubuntu1.2.debian.tar.xz' procps_3.3.12-3ubuntu1.2.debian.tar.xz 37736 SHA512:36ef9f540a72538f4a6fb02bfb53bf0b4689077c733b7dc4e301f968e2698667e6ad997f30a0ad21d189a8ee4bef7de2710441a8cc9f1ecb3aff6f67f182d49e
```

### `dpkg` source package: `python-defaults=2.7.15~rc1-1`

Binary Packages:

- `libpython-stdlib:amd64=2.7.15~rc1-1`
- `python=2.7.15~rc1-1`
- `python-minimal=2.7.15~rc1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.15~rc1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.15~rc1-1.dsc' python-defaults_2.7.15~rc1-1.dsc 2633 SHA256:1089e25a274fb86e8dfbab1b661ecb5ef2b7610e1b6e3fbf8388f875758f7c2c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.15~rc1-1.tar.gz' python-defaults_2.7.15~rc1-1.tar.gz 1958015 SHA256:f3bed2b81091821d2e514c2e17c6846f7e744487fd15f7d3c48fa1c91b9cd49b
```

### `dpkg` source package: `python2.7=2.7.17-1~18.04ubuntu1.2`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.17-1~18.04ubuntu1.2`
- `libpython2.7-stdlib:amd64=2.7.17-1~18.04ubuntu1.2`
- `python2.7=2.7.17-1~18.04ubuntu1.2`
- `python2.7-minimal=2.7.17-1~18.04ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libpython2.7-minimal/copyright`, `/usr/share/doc/libpython2.7-stdlib/copyright`, `/usr/share/doc/python2.7/copyright`, `/usr/share/doc/python2.7-minimal/copyright`)

- `# Licensed to PSF under a Contributor Agreement`
- `* Permission to use this software in any way is granted without`
- `Apache`
- `Apache-2`
- `Apache-2.0`
- `Expat`
- `GPL-2`
- `ISC`
- `LGPL-2.1+`
- `PSF-2`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Python`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `implied`
- `see above, some license as Python`

Source:

```console
$ apt-get source -qq --print-uris python2.7=2.7.17-1~18.04ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.17-1~18.04ubuntu1.2.dsc' python2.7_2.7.17-1~18.04ubuntu1.2.dsc 3483 SHA512:5450e075e251ba89bb299da7468875428b81a9249bb0a72fd845aa517bbae52f876c339f9064861f287e62adb7db70d5c2ad3cdd1ac425a2371372775fc4277f
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.17.orig.tar.gz' python2.7_2.7.17.orig.tar.gz 17535962 SHA512:f526baff7f1a9451244edb04e2aca63336b656aac178f4f64c135390b5b1185990ccff0c48f602914dd1c49c9e075951d372b4f2daac39e336c23ae84ef4ca16
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.17-1~18.04ubuntu1.2.diff.gz' python2.7_2.7.17-1~18.04ubuntu1.2.diff.gz 294617 SHA512:a92eb8fe030174bc0b063d71e58dcb364a0d62bf554afae01da6dc121246442149630c104d2d4f49a0d7a247042ffa176973baf5f6d516f772b986f4dbdaf19e
```

### `dpkg` source package: `python3-defaults=3.6.7-1~18.04`

Binary Packages:

- `libpython3-stdlib:amd64=3.6.7-1~18.04`
- `python3=3.6.7-1~18.04`
- `python3-minimal=3.6.7-1~18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.6.7-1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.dsc' python3-defaults_3.6.7-1~18.04.dsc 2896 SHA512:1f6f6bdbc030b0c9bf24a97b2c48052c8a52810e22e021b00719fce7eea8d454c9cc756e3d73ee79be06655b9a35fe8279bf71833a4aa6c605859856e4a31151
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.6.7-1~18.04.tar.gz' python3-defaults_3.6.7-1~18.04.tar.gz 137600 SHA512:7020c60ba146deafaf1937883bea03c39efb1068968025756b32e7c7f069c06bfdfb3e1b91dcaa5a1e1c4c01e0177ea91beb4f5fa71f5e60334866ef5b28a2ef
```

### `dpkg` source package: `python3-stdlib-extensions=3.6.9-1~18.04`

Binary Packages:

- `python3-distutils=3.6.9-1~18.04`
- `python3-lib2to3=3.6.9-1~18.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.6.9-1~18.04
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.6.9-1~18.04.dsc' python3-stdlib-extensions_3.6.9-1~18.04.dsc 2624 SHA512:e10786f72375b0da8042ac41094c5c2fa9d4649001646da0072e51207042dc0434d5f06616e50a13bfe9610044f0e0bed4cc5b6e9487c38a81024568d52918ce
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.6.9.orig.tar.bz2' python3-stdlib-extensions_3.6.9.orig.tar.bz2 4237908 SHA512:79312db29db5ad407d6710f3f8d1c725f2efd481d875d06dfb7e3d442cafccca19d0601a899b86c4cf0360ba6dcaeca187e856c5a6d50df04abef309122b3dd7
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.6.9-1~18.04.debian.tar.xz' python3-stdlib-extensions_3.6.9-1~18.04.debian.tar.xz 16908 SHA512:7f0e9efb59e4a50b913c13ed0308a3f3fd4c9fc8f029ea6100f40afffc7e6698c781d0910e5443dcde20345a9e5ef4402d4e22f393507169149e58fe14d857a3
```

### `dpkg` source package: `python3.6=3.6.9-1~18.04ubuntu1.3`

Binary Packages:

- `libpython3.6-minimal:amd64=3.6.9-1~18.04ubuntu1.3`
- `libpython3.6-stdlib:amd64=3.6.9-1~18.04ubuntu1.3`
- `python3.6=3.6.9-1~18.04ubuntu1.3`
- `python3.6-minimal=3.6.9-1~18.04ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libpython3.6-minimal/copyright`, `/usr/share/doc/libpython3.6-stdlib/copyright`, `/usr/share/doc/python3.6/copyright`, `/usr/share/doc/python3.6-minimal/copyright`)

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
$ apt-get source -qq --print-uris python3.6=3.6.9-1~18.04ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9-1~18.04ubuntu1.3.dsc' python3.6_3.6.9-1~18.04ubuntu1.3.dsc 3470 SHA512:90c6343deb85a452e9a7b2987db330b37b9fe3f04ee1eaf2b21f8a2303e844736e13735e81a2f0f8feeab2b9aa795fa27a8ec14d84eda070f670afb4c4077990
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9.orig.tar.xz' python3.6_3.6.9.orig.tar.xz 17212164 SHA512:05de9c6f44d96a52bfce10ede4312de892573edaf8bece65926d19973a3a800d65eed7a857af945f69efcfb25efa3788e7a54016b03d80b611eb51c3ea074819
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.6/python3.6_3.6.9-1~18.04ubuntu1.3.debian.tar.xz' python3.6_3.6.9-1~18.04ubuntu1.3.debian.tar.xz 220084 SHA512:6f37facb9aad3fb2f00c587132fd8716cd54329b9f6087c4a2429844edd17e6dbf64d9c763f8b774782610da4ffa9647127b54482cbecd79846c9f7e24c0d17d
```

### `dpkg` source package: `readline=7.0-3`

Binary Packages:

- `libreadline-dev:amd64=7.0-3`
- `libreadline7:amd64=7.0-3`
- `readline-common=7.0-3`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline7/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=7.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0-3.dsc' readline_7.0-3.dsc 2538 SHA256:f27a5dc9053b88641e3effc6c03b7840cbbbd887e8dcaf05d9e336c7bc7c6a53
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0.orig.tar.gz' readline_7.0.orig.tar.gz 2910016 SHA256:750d437185286f40a369e1e4f4764eda932b9459b5ec9a731628393dd3d32334
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_7.0-3.debian.tar.xz' readline_7.0-3.debian.tar.xz 30012 SHA256:bf166310d6ca7716f2bd0e9e06cee2458b0157f7989d028730fc305643560175
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-1.dsc 2315 SHA256:e56822b88625bf6a51f06652fc36fa2a1348b4325ac76541800cd078192aa3d2
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-1.debian.tar.xz 8044 SHA256:675847f5cddb860256cbf2e7d5b85918aa53b59b0fd97a466b39a5c77a399537
```

### `dpkg` source package: `sed=4.4-2`

Binary Packages:

- `sed=4.4-2`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4-2.dsc' sed_4.4-2.dsc 2006 SHA256:0e025a69a04c867048f918778771e2ba79d6ddfd62cb5ce6c3a6e255c005706c
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4.orig.tar.xz' sed_4.4.orig.tar.xz 1181664 SHA256:cbd6ebc5aaf080ed60d0162d7f6aeae58211a1ee9ba9bb25623daa6cd942683b
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.4-2.debian.tar.xz' sed_4.4-2.debian.tar.xz 59600 SHA256:9f9b8bec0438ea0d0bd4315548de519543385c8196bcfcc61362f38f4cc6e7ed
```

### `dpkg` source package: `sensible-utils=0.0.12`

Binary Packages:

- `sensible-utils=0.0.12`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.12
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.dsc' sensible-utils_0.0.12.dsc 1732 SHA256:1b62cc5f7561b3f5692a6edaec942e2e97e8368dabff8c865867d428eecb1221
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12.tar.xz' sensible-utils_0.0.12.tar.xz 62152 SHA256:99ba2ebf8c57447c69d426b99b84ff9dc817be0bc4988ec6890a14558c529e2e
```

### `dpkg` source package: `serf=1.3.9-6`

Binary Packages:

- `libserf-1-1:amd64=1.3.9-6`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache`
- `Apache-2.0`
- `Zlib`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.9-6/


### `dpkg` source package: `shadow=1:4.5-1ubuntu2`

Binary Packages:

- `login=1:4.5-1ubuntu2`
- `passwd=1:4.5-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.5-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.dsc' shadow_4.5-1ubuntu2.dsc 2426 SHA512:69714d4cd1903f091bc2c4759d98ce588cc90e9f2ab49226b46872eb2b2cf4f996f30b8da146a2950e164d24fa265f90e689043152d79d1bc255add5f90d54a3
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5.orig.tar.xz' shadow_4.5.orig.tar.xz 1344524 SHA512:4278544efdd6d800a3c46cfcb144f209ace14ebe017ba1c0d05425fac7868062a73afa8522036a2bc0a16f6f1e7c16373a204463221012367ce0e8e9ef4c4a4d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.5-1ubuntu2.debian.tar.xz' shadow_4.5-1ubuntu2.debian.tar.xz 471472 SHA512:d4017784bfc5118b86533da52909459adf4e79ffa049d8029437860bfaeac91eabd40e6510f67bba6f8b2d74fde62c24eb8e37a7b4637d14eeb63aecaf2294cc
```

### `dpkg` source package: `shared-mime-info=1.9-2`

Binary Packages:

- `shared-mime-info=1.9-2`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.9-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.9-2.dsc' shared-mime-info_1.9-2.dsc 2203 SHA256:0592a6550b9bee8895d4a4fe577a15a28a5a911135765ae74b310abaea5c5b66
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.9.orig.tar.xz' shared-mime-info_1.9.orig.tar.xz 607648 SHA256:5c0133ec4e228e41bdf52f726d271a2d821499c2ab97afd3aa3d6cf43efcdc83
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.9-2.debian.tar.xz' shared-mime-info_1.9-2.debian.tar.xz 9992 SHA256:18cb7e2c0f2a3daa2d55abc87c4619d68f537f268a3bad8510e1fcf0d6b0cd76
```

### `dpkg` source package: `six=1.11.0-2`

Binary Packages:

- `python-six=1.11.0-2`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.11.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.11.0-2.dsc' six_1.11.0-2.dsc 2316 SHA256:c0391b38bc251a3df586bdb163cb250af78aee69bbb27880215a350caaea53f2
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.11.0.orig.tar.gz' six_1.11.0.orig.tar.gz 29860 SHA256:70e8a77beed4562e7f14fe23a786b54f6296e34344c23bc42f07b15018ff98e9
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.11.0-2.debian.tar.xz' six_1.11.0-2.debian.tar.xz 4176 SHA256:bbd91dcb509a1f083bf531062b77dfdf2cbd2badca0fbe5d81957fe852ac4a7a
```

### `dpkg` source package: `sqlite3=3.22.0-1ubuntu0.4`

Binary Packages:

- `libsqlite3-0:amd64=3.22.0-1ubuntu0.4`
- `libsqlite3-dev:amd64=3.22.0-1ubuntu0.4`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.22.0-1ubuntu0.4
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.dsc' sqlite3_3.22.0-1ubuntu0.4.dsc 2512 SHA512:5b0de02a1ee10ef1d38bbd66e5148f044574aba7211cbe003855b8141062955913514501adac6208297f435c02160a39e14dbad934907afd49a506a34ae4ea9a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig-www.tar.xz' sqlite3_3.22.0.orig-www.tar.xz 3564688 SHA512:e469878137ec3d06886fe096c4325451e8c9b73f6841d28fac9bed45e698bdc1222739570abf2ce456e0853b0c6876b1c79ca0896826295f64d27b276541c1f8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0.orig.tar.xz' sqlite3_3.22.0.orig.tar.xz 6019648 SHA512:ce3b05cb9f75a5c7a5e8562b70e72e23c043222fd61995f795cbcc40f3f8efcac2660e57b588a15bfdce28c8eb644745bb73af35f5b98ba956dd77457d661dfa
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz' sqlite3_3.22.0-1ubuntu0.4.debian.tar.xz 47632 SHA512:1b280b6c301b2f3c15ebdfe6085584cef34257edae14c94d7d6e8d06a7b884a96029d354cb3f09df6b6427f671a24cc25ee1ebc178c7168cd0a52bce8c8b5cf0
```

### `dpkg` source package: `subversion=1.9.7-4ubuntu1`

Binary Packages:

- `libsvn1:amd64=1.9.7-4ubuntu1`
- `subversion=1.9.7-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris subversion=1.9.7-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.9.7-4ubuntu1.dsc' subversion_1.9.7-4ubuntu1.dsc 3118 SHA256:13e18929d55c09986a758d3245ff246996d7f75f9d6f7313c394ba4d0a73b5ed
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.9.7.orig.tar.gz' subversion_1.9.7.orig.tar.gz 10643686 SHA256:c72a209c883e20245f14c4e644803f50ae83ae24652e385ff5e82300a0d06c3c
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.9.7-4ubuntu1.debian.tar.xz' subversion_1.9.7-4ubuntu1.debian.tar.xz 2270568 SHA256:67ea7ddc37e697340eaa9f8fea08980ba01b529f3ab6487eeb8726bc9ae77f29
```

### `dpkg` source package: `systemd=237-3ubuntu10.43`

Binary Packages:

- `libsystemd0:amd64=237-3ubuntu10.43`
- `libudev1:amd64=237-3ubuntu10.43`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=237-3ubuntu10.43
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.43.dsc' systemd_237-3ubuntu10.43.dsc 5187 SHA512:a15d7060d674bd8ee019a71f42fa9a79fbd067b726806cc31e5fdc7ab03c414c1d1453aebb673d812f0529b293f529967a5013cbb7fcae8c948d3434aae8bed3
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237.orig.tar.gz' systemd_237.orig.tar.gz 6871350 SHA512:15ef4b92815a6dd9a6c51672dbc00fd7cd0f08068ef0cbeaca574f68d330b28bc67ba1946f24f75ef3d9e7b63843a73eea700db54688061dbf5c9f8470394c3b
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_237-3ubuntu10.43.debian.tar.xz' systemd_237-3ubuntu10.43.debian.tar.xz 277780 SHA512:fb31f967e4427624c8d1df146595166ebef9b56b42d1e03ef4393e171279d2d6b52d0d5bc31c13413585013d4a9d09c3eda9158fb7ba390b0cd480b3b155b18d
```

### `dpkg` source package: `sysvinit=2.88dsf-59.10ubuntu1`

Binary Packages:

- `sysvinit-utils=2.88dsf-59.10ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.10ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10ubuntu1.dsc' sysvinit_2.88dsf-59.10ubuntu1.dsc 2428 SHA256:030f4e8a71381529da3141988344d6e1d0e05ba437e0cdd38d2f3786185bf285
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.10ubuntu1.debian.tar.xz' sysvinit_2.88dsf-59.10ubuntu1.debian.tar.xz 132736 SHA256:faee591309aa0065aa43f44a1e840eb01db7f55379af2b45949534bd0317b734
```

### `dpkg` source package: `tar=1.29b-2ubuntu0.1`

Binary Packages:

- `tar=1.29b-2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.29b-2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.dsc' tar_1.29b-2ubuntu0.1.dsc 1426 SHA512:07cd0e105d5620c2f9b77c1a8b6f1016f2c83a022a38d0fa9e94bc07ffe3f716df609b8c92808e5e3e80db8eaece3b076643debd54c653eda76eb1973a56e9ab
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b.orig.tar.xz' tar_1.29b.orig.tar.xz 1822008 SHA512:6814c906f3bf3d1421d46e63aff7921acffbd2b2a0a7e5c20b472a821eab839d6eab93653d964ae16376b65da223c57a92455f44793522c84c8b1343af20b106
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.29b-2ubuntu0.1.debian.tar.xz' tar_1.29b-2ubuntu0.1.debian.tar.xz 31672 SHA512:e4756dd0ad0d765af0c6639695b17cc86f80033a45705cdcb845639bab7d3aed0fac8d86ac28a0aa2e024bdb4dad43376f4a02c915a0921609deeeed74637bd7
```

### `dpkg` source package: `tiff=4.0.9-5ubuntu0.3`

Binary Packages:

- `libtiff-dev=4.0.9-5ubuntu0.3`
- `libtiff5:amd64=4.0.9-5ubuntu0.3`
- `libtiff5-dev:amd64=4.0.9-5ubuntu0.3`
- `libtiffxx5:amd64=4.0.9-5ubuntu0.3`

Licenses: (parsed from: `/usr/share/doc/libtiff-dev/copyright`, `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiff5-dev/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.9-5ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9-5ubuntu0.3.dsc' tiff_4.0.9-5ubuntu0.3.dsc 2299 SHA512:1577627fb228fbb25ba7e405c4931bc642f0c2f8d4a061bee16fdf572a23d637bf1974911e18cb17461b8fa533fbcc1924d8b099c96116385e2306f853cb2e1a
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9.orig.tar.gz' tiff_4.0.9.orig.tar.gz 2305681 SHA512:04f3d5eefccf9c1a0393659fe27f3dddd31108c401ba0dc587bca152a1c1f6bc844ba41622ff5572da8cc278593eff8c402b44e7af0a0090e91d326c2d79f6cd
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.9-5ubuntu0.3.debian.tar.xz' tiff_4.0.9-5ubuntu0.3.debian.tar.xz 32200 SHA512:f4c77de2474074c942891927b360eedbdf1217c2fa2083338e9d24956a6d6a418e9b4935df3288e652170186d67bbcb865f38a3f5f4c7eea65405a6a6cbf3c0c
```

### `dpkg` source package: `ubuntu-keyring=2018.09.18.1~18.04.0`

Binary Packages:

- `ubuntu-keyring=2018.09.18.1~18.04.0`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2018.09.18.1~18.04.0
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.dsc' ubuntu-keyring_2018.09.18.1~18.04.0.dsc 1503 SHA512:1aa2656d79d925d42857de9eb79fac8433fc5ec0cc1daaa55af31f1eb4f482646f48e0e37d8d794ffafccbae34698503aa183b27666b18fc00c38e1b41c92f06
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz' ubuntu-keyring_2018.09.18.1~18.04.0.tar.gz 34238 SHA512:7e0b6b9b4f900139c6743037b18591abba0183db94bf6d988b65c2eafe7bd53900f52af0cea14e1a80f4fd54eef39ef7b5dbf66802b53c022e40802a287912b1
```

### `dpkg` source package: `ucf=3.0038`

Binary Packages:

- `ucf=3.0038`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0038
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0038.dsc' ucf_3.0038.dsc 1445 SHA256:5fab6d0af664eac92b3404c6bb62d0a3ceb88cd21a1462b9a262d1292c77328f
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0038.tar.xz' ucf_3.0038.tar.xz 65416 SHA256:262ccd52637c869ac851838a176d76e90db8d3f12373e3b62eb89e217f93fe7e
```

### `dpkg` source package: `unzip=6.0-21ubuntu1`

Binary Packages:

- `unzip=6.0-21ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-21ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-21ubuntu1.dsc' unzip_6.0-21ubuntu1.dsc 1800 SHA256:76f9c291eae4039e31fda029426c96a332d3ce905a2306998ff55798d03ea44d
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-21ubuntu1.debian.tar.xz' unzip_6.0-21ubuntu1.debian.tar.xz 21080 SHA256:8db974c22a5ef50029eb9a7e5429ff099e1cf7cfd36d3951fa4e00e4fd47843f
```

### `dpkg` source package: `util-linux=2.31.1-0.4ubuntu3.7`

Binary Packages:

- `bsdutils=1:2.31.1-0.4ubuntu3.7`
- `fdisk=2.31.1-0.4ubuntu3.7`
- `libblkid1:amd64=2.31.1-0.4ubuntu3.7`
- `libfdisk1:amd64=2.31.1-0.4ubuntu3.7`
- `libmount1:amd64=2.31.1-0.4ubuntu3.7`
- `libsmartcols1:amd64=2.31.1-0.4ubuntu3.7`
- `libuuid1:amd64=2.31.1-0.4ubuntu3.7`
- `mount=2.31.1-0.4ubuntu3.7`
- `util-linux=2.31.1-0.4ubuntu3.7`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.31.1-0.4ubuntu3.7
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.31.1-0.4ubuntu3.7.dsc' util-linux_2.31.1-0.4ubuntu3.7.dsc 4122 SHA512:2602472fb8da0cedd750f9df51b3a5ff4a04be4fcc8843d2b9294495d5697c7209111ec2889f980da7051c39ee186ab3d69fdefea08a1531c9686e4ac9427a1e
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.31.1.orig.tar.xz' util-linux_2.31.1.orig.tar.xz 4514032 SHA512:0a3dc7a4c80f180d99ff64452e6e7269688a7d066a212ab15eafb3b9aaedf0b5294345bc1087dc9655f0efc82d4bb7dff9b669b5ee338a5f13aaff7407fe384f
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.31.1-0.4ubuntu3.7.debian.tar.xz' util-linux_2.31.1-0.4ubuntu3.7.debian.tar.xz 102216 SHA512:f94ae8ca8fa4d3a79a2c909807bbee0bc28156abe33e072a47149fab6f820aab462f2869f564c9a30ef20c0ca21f2b777809324c7c426bf58f584ea4efe3596f
```

### `dpkg` source package: `wget=1.19.4-1ubuntu2.2`

Binary Packages:

- `wget=1.19.4-1ubuntu2.2`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.19.4-1ubuntu2.2
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4-1ubuntu2.2.dsc' wget_1.19.4-1ubuntu2.2.dsc 2226 SHA512:7fbc8eccfcb3e559f4f25c4159b06a9663f87c02ab63a9eebc63a812a6a0d72958329f4c8f60fd3dc0272bb586a13535389e0fe5d5a6a2b42f909f567976dd57
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4.orig.tar.gz' wget_1.19.4.orig.tar.gz 4310657 SHA512:e84b0c40235b160ade69e18f2f139c782eb2387edc97a847c11dbb906c0273daf6d0ef5afe20360ba965c7da8b5e109f5a45e39ea93d20ec945575203235943a
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4.orig.tar.gz.asc' wget_1.19.4.orig.tar.gz.asc 1241 SHA512:63ad8a3184a98dbda966a535964e37c84291a13fe15f7defb6fb3672f7148d66143498354e818eabc1e506ae9a16f7c9b8188fa22c2fed3a02aa9cb6d1de3a38
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.19.4-1ubuntu2.2.debian.tar.xz' wget_1.19.4-1ubuntu2.2.debian.tar.xz 66156 SHA512:c458c630d82aaeffa0f4df6a543aa9b3a312d5b4aad4835d6da37736f165bb1151a9337ad65298c8b50c4a07de40d40303f0fc5953f2086a1909878f97c7b262
```

### `dpkg` source package: `xorg-sgml-doctools=1:1.11-1`

Binary Packages:

- `xorg-sgml-doctools=1:1.11-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xorg-sgml-doctools=1:1.11-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.dsc' xorg-sgml-doctools_1.11-1.dsc 1975 SHA256:1f4a12a38420b0ddab35553b9588fdf43ab39577958aed70fca435c9a747141a
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11.orig.tar.gz' xorg-sgml-doctools_1.11.orig.tar.gz 150367 SHA256:986326d7b4dd2ad298f61d8d41fe3929ac6191c6000d6d7e47a8ffc0c34e7426
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg-sgml-doctools/xorg-sgml-doctools_1.11-1.diff.gz' xorg-sgml-doctools_1.11-1.diff.gz 3194 SHA256:18eeb355cb0efff9f47f8ed8e852eee322d9733a427419f4b39f43bc4df630c1
```

### `dpkg` source package: `xorg=1:7.7+19ubuntu7.1`

Binary Packages:

- `x11-common=1:7.7+19ubuntu7.1`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+19ubuntu7.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu7.1.dsc' xorg_7.7+19ubuntu7.1.dsc 2103 SHA512:e6c459b18a96cbfda965f13852ff1c75b7e3240f61c4ea941996b99f74ffcf52b6ef539d37ca91903459260354a9368db5cd38d84903647259d8f1ac85a47943
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+19ubuntu7.1.tar.gz' xorg_7.7+19ubuntu7.1.tar.gz 298771 SHA512:6e3ac8b4932fc3ba476ce69fa5e111ed2f57b46e0b9361b01f631d82e635e8741088eedeeafdb0e13cf63cbedacf0a0872ca656ace349ecb6a79402f67522b6a
```

### `dpkg` source package: `xorgproto=2018.4-4`

Binary Packages:

- `x11proto-core-dev=2018.4-4`
- `x11proto-dev=2018.4-4`
- `x11proto-xext-dev=2018.4-4`

Licenses: (parsed from: `/usr/share/doc/x11proto-core-dev/copyright`, `/usr/share/doc/x11proto-dev/copyright`, `/usr/share/doc/x11proto-xext-dev/copyright`)

- `MIT`
- `SGI`

Source:

```console
$ apt-get source -qq --print-uris xorgproto=2018.4-4
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4-4.dsc' xorgproto_2018.4-4.dsc 4059 SHA256:6279a145ce040d9301a0e2efdf203dd7d2822bc9a90e94de08d545c4b724d8e3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4.orig.tar.gz' xorgproto_2018.4.orig.tar.gz 493597 SHA256:8e48d851efea0e951bcb6cf0d537f84ba3803de95e488bd039fe59fc75ec8f7d
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4.orig.tar.gz.asc' xorgproto_2018.4.orig.tar.gz.asc 241 SHA256:3ab131cf8f497d315043b2c791912c22045da557e6894f1e5db533a0b0baed2f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorgproto/xorgproto_2018.4-4.diff.gz' xorgproto_2018.4-4.diff.gz 20976 SHA256:a9b27658c7c9e53372679bbb26099abed6cb9215355a99995858164de3fa5048
```

### `dpkg` source package: `xtrans=1.3.5-1`

Binary Packages:

- `xtrans-dev=1.3.5-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xtrans=1.3.5-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5-1.dsc' xtrans_1.3.5-1.dsc 1901 SHA256:64750bc2dd993ac93b9e0a8d6109ce72963ab22296479145eb3f392d238c2280
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5.orig.tar.gz' xtrans_1.3.5.orig.tar.gz 227536 SHA256:b7a577c1b6c75030145e53b4793db9c88f9359ac49e7d771d4385d21b3e5945d
'http://archive.ubuntu.com/ubuntu/pool/main/x/xtrans/xtrans_1.3.5-1.diff.gz' xtrans_1.3.5-1.diff.gz 16122 SHA256:2acb2c4f5958ef1bbae74ca64007d0465261a4f62bfad6ed22f1f144c0e445e1
```

### `dpkg` source package: `xz-utils=5.2.2-1.3`

Binary Packages:

- `liblzma-dev:amd64=5.2.2-1.3`
- `liblzma5:amd64=5.2.2-1.3`
- `xz-utils=5.2.2-1.3`

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
$ apt-get source -qq --print-uris xz-utils=5.2.2-1.3
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.dsc' xz-utils_5.2.2-1.3.dsc 2575 SHA256:3ea4e6a32f6265b152f89ceafe78c8839e5f4bb1cad137b159fe2013817f9342
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz' xz-utils_5.2.2.orig.tar.xz 1016404 SHA256:f341b1906ebcdde291dd619399ae944600edc9193619dd0c0110a5f05bfcc89e
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2.orig.tar.xz.asc' xz-utils_5.2.2.orig.tar.xz.asc 543 SHA256:2cc0575556e1331b3f468e6e7dca5969ce86efcc315d62672279b4e68b2e449f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.2-1.3.debian.tar.xz' xz-utils_5.2.2-1.3.debian.tar.xz 108680 SHA256:d76c3acf39d0999c14384695394970e8f98853fd6736ba91972d3e67106bc6f6
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-0ubuntu2`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-0ubuntu2`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-0ubuntu2.dsc' zlib_1.2.11.dfsg-0ubuntu2.dsc 2676 SHA256:e733161caf3c6864deec55f40f80c0872f7c83bd9c6e9f937472f227ad912281
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.xz' zlib_1.2.11.dfsg.orig.tar.xz 287216 SHA256:881c8a90f488def83488aa91fd68563c023013a4b9b07a040f6da2727d76ad60
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-0ubuntu2.debian.tar.xz' zlib_1.2.11.dfsg-0ubuntu2.debian.tar.xz 18344 SHA256:afad42904f793d13a0b631e082e575d90a7c7c443973d08a00061a9bbb5ca380
```
