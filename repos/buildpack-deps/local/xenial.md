# `buildpack-deps:xenial`

## Docker Metadata

- Image ID: `sha256:ccceb225aac979daaa0386670bc20ce27808a0635bba4787823f728fb04c490e`
- Created: `2020-07-24T15:08:04.760885187Z`
- Virtual Size: ~ 648.56 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/bin/bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.52-3`

Binary Packages:

- `libacl1:amd64=2.2.52-3`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.52-3
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3.dsc' acl_2.2.52-3.dsc 2025 SHA256:82e344b9ab176559a85630b74ee5a68d678d7f24b6fe8139f2fd9fcf38a48095
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52.orig.tar.bz2' acl_2.2.52.orig.tar.bz2 312128 SHA256:59d05b38af76baf2eddccbf08c7968a17451cc785ffecc657fcb46ce32b2631d
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.52-3.debian.tar.xz' acl_2.2.52-3.debian.tar.xz 8740 SHA256:fc3f1178d18288993fc4ce4853b7f9dcdf0bd1fd26e4f69349a4e4e5916d1fa8
```

### `dpkg` source package: `adduser=3.113+nmu3ubuntu4`

Binary Packages:

- `adduser=3.113+nmu3ubuntu4`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.113+nmu3ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.113+nmu3ubuntu4.dsc' adduser_3.113+nmu3ubuntu4.dsc 1856 SHA256:323f327b25e1fbeba38278eae5813be6238a7c5959e7c10af041999408440247
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.113+nmu3ubuntu4.tar.gz' adduser_3.113+nmu3ubuntu4.tar.gz 367980 SHA256:6e4d44c8388b9ba85fc175fa4a48ed43bf6500913c2c631fda0e4419ae63c65a
```

### `dpkg` source package: `apparmor=2.10.95-0ubuntu2.11`

Binary Packages:

- `libapparmor1:amd64=2.10.95-0ubuntu2.11`

Licenses: (parsed from: `/usr/share/doc/libapparmor1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris apparmor=2.10.95-0ubuntu2.11
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.10.95-0ubuntu2.11.dsc' apparmor_2.10.95-0ubuntu2.11.dsc 3256 SHA256:611d2f29819a258e80ddf377be07f1aaa0e10bb81e73efea2cd22a8e6a4b4432
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.10.95.orig.tar.gz' apparmor_2.10.95.orig.tar.gz 4502268 SHA256:3f659a599718f4a5e2a33140916715f574a5cb3634a6b9ed6d29f7b0617e4d1a
'http://archive.ubuntu.com/ubuntu/pool/main/a/apparmor/apparmor_2.10.95-0ubuntu2.11.debian.tar.xz' apparmor_2.10.95-0ubuntu2.11.debian.tar.xz 98980 SHA256:ba13706bc1d8b872cf08e748129b6d892e961440aad0b2329e610a3ba865eb7b
```

### `dpkg` source package: `apr-util=1.5.4-1build1`

Binary Packages:

- `libaprutil1:amd64=1.5.4-1build1`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.5.4-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.5.4-1build1.dsc' apr-util_1.5.4-1build1.dsc 2642 SHA256:f464c7a9fb9293c117e80d9669450ca61191ad456cf40dd74777caf06e5f18db
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.5.4.orig.tar.bz2' apr-util_1.5.4.orig.tar.bz2 694427 SHA256:a6cf327189ca0df2fb9d5633d7326c460fe2b61684745fd7963e79a6dd0dc82e
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.5.4-1build1.debian.tar.xz' apr-util_1.5.4-1build1.debian.tar.xz 16564 SHA256:562bd9b543a16edf8218deda292c606aabe5265a369cf7b2559f13c1cc300e3c
```

### `dpkg` source package: `apr=1.5.2-3`

Binary Packages:

- `libapr1:amd64=1.5.2-3`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.5.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.5.2-3.dsc' apr_1.5.2-3.dsc 2090 SHA256:2344484f62544881344defbb1076ca6cce51f930f1a5abd359e65eafb0e169cb
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.5.2.orig.tar.bz2' apr_1.5.2.orig.tar.bz2 826885 SHA256:7d03ed29c22a7152be45b8e50431063736df9e1daa1ddf93f6a547ba7a28f67a
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.5.2-3.debian.tar.xz' apr_1.5.2-3.debian.tar.xz 18572 SHA256:442ffb9a7225cf405fe7a2b4a4624543fcb93e6f14cccf22acd57916cfa8348d
```

### `dpkg` source package: `apt=1.2.32ubuntu0.1`

Binary Packages:

- `apt=1.2.32ubuntu0.1`
- `libapt-pkg5.0:amd64=1.2.32ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.2.32ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.2.32ubuntu0.1.dsc' apt_1.2.32ubuntu0.1.dsc 2218 SHA256:e73a0ac2ae73ee0417d135f8d5e5a0b0906aa9ace64fd0a4d4a0cfc483a7269f
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.2.32ubuntu0.1.tar.xz' apt_1.2.32ubuntu0.1.tar.xz 2095712 SHA256:3374c23e40ec7a8d7efbb740b353065760b3527c12bfad0a6daa4072436b8afc
```

### `dpkg` source package: `atk1.0=2.18.0-1`

Binary Packages:

- `libatk1.0-0:amd64=2.18.0-1`
- `libatk1.0-data=2.18.0-1`

Licenses: (parsed from: `/usr/share/doc/libatk1.0-0/copyright`, `/usr/share/doc/libatk1.0-data/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris atk1.0=2.18.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.18.0-1.dsc' atk1.0_2.18.0-1.dsc 2738 SHA256:3d58e1e9e653705df8a092ed6942e2e518b1e539196e467fc60f20721ccaa84c
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.18.0.orig.tar.xz' atk1.0_2.18.0.orig.tar.xz 687932 SHA256:ce6c48d77bf951083029d5a396dd552d836fff3c1715d3a7022e917e46d0c92b
'http://archive.ubuntu.com/ubuntu/pool/main/a/atk1.0/atk1.0_2.18.0-1.debian.tar.xz' atk1.0_2.18.0-1.debian.tar.xz 10520 SHA256:84ebc674126d71a27994b856274d05c801782ab4cbd3b78351c987525243ed1d
```

### `dpkg` source package: `attr=1:2.4.47-2`

Binary Packages:

- `libattr1:amd64=1:2.4.47-2`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.47-2
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2.dsc' attr_2.4.47-2.dsc 2027 SHA256:ee842d6d62d473acf02b494c432cf33128fa46455a09d3172c77c252449fa1a6
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47.orig.tar.bz2' attr_2.4.47.orig.tar.bz2 281877 SHA256:6c1208035757f5ce9b516402dd45b8299a53ae4d69ad2c352116f9cb8d7bc274
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.47-2.debian.tar.xz' attr_2.4.47-2.debian.tar.xz 8096 SHA256:f65909562def601b1556393f5656032c058dc574ba622414ad3eb80c7b05a42a
```

### `dpkg` source package: `audit=1:2.4.5-1ubuntu2.1`

Binary Packages:

- `libaudit-common=1:2.4.5-1ubuntu2.1`
- `libaudit1:amd64=1:2.4.5-1ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.4.5-1ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.4.5-1ubuntu2.1.dsc' audit_2.4.5-1ubuntu2.1.dsc 2753 SHA256:a4f05c33bdfde5cddada8c933c3ec34c9a532bcc558f965e41c27c851ce0a607
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.4.5.orig.tar.gz' audit_2.4.5.orig.tar.gz 1030113 SHA256:e73cdd3fc779b122523acaabcda3e27ce70eec22ad4eb526898be9be5b2838e0
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.4.5-1ubuntu2.1.debian.tar.xz' audit_2.4.5-1ubuntu2.1.debian.tar.xz 19292 SHA256:285eef1a789f47c9ad6a30dc8427822b624146715a8f603d011bdc117529d5b2
```

### `dpkg` source package: `autoconf=2.69-9`

Binary Packages:

- `autoconf=2.69-9`

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
$ apt-get source -qq --print-uris autoconf=2.69-9
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-9.dsc' autoconf_2.69-9.dsc 1944 SHA256:a279ec1b96760dcd9725a62b47ec80ac7c69add08cf189aa52b1b2268fc275cd
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-9.debian.tar.xz' autoconf_2.69-9.debian.tar.xz 22728 SHA256:9498087074be2dab0cb7b37e9dbeac0bf5cd26019a3c25694fc61039f0bda064
```

### `dpkg` source package: `automake-1.15=1:1.15-4ubuntu1`

Binary Packages:

- `automake=1:1.15-4ubuntu1`

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
$ apt-get source -qq --print-uris automake-1.15=1:1.15-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.15/automake-1.15_1.15-4ubuntu1.dsc' automake-1.15_1.15-4ubuntu1.dsc 2352 SHA256:446e0e71de6b75022defe822df11ef461de3d5090c255130788c77fab1f7e04a
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.15/automake-1.15_1.15.orig.tar.xz' automake-1.15_1.15.orig.tar.xz 1496708 SHA256:9908c75aabd49d13661d6dcb1bc382252d22cc77bf733a2d55e87f2aa2db8636
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.15/automake-1.15_1.15-4ubuntu1.debian.tar.xz' automake-1.15_1.15-4ubuntu1.debian.tar.xz 12868 SHA256:1fb41424b5827296281addf047c9619eac99c5342b57e7412014176981443f28
```

### `dpkg` source package: `autotools-dev=20150820.1`

Binary Packages:

- `autotools-dev=20150820.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20150820.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20150820.1.dsc' autotools-dev_20150820.1.dsc 1641 SHA256:7f5e21caa39e5e40fc4d1560b288a3b785810daead1593567a491221716a5136
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20150820.1.tar.xz' autotools-dev_20150820.1.tar.xz 61792 SHA256:fa40ff0ad94a8790357324f22a64bd8673383d5d56687dbebd3df5afe046c81f
```

### `dpkg` source package: `avahi=0.6.32~rc+dfsg-1ubuntu2.3`

Binary Packages:

- `libavahi-client3:amd64=0.6.32~rc+dfsg-1ubuntu2.3`
- `libavahi-common-data:amd64=0.6.32~rc+dfsg-1ubuntu2.3`
- `libavahi-common3:amd64=0.6.32~rc+dfsg-1ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/libavahi-client3/copyright`, `/usr/share/doc/libavahi-common-data/copyright`, `/usr/share/doc/libavahi-common3/copyright`)

- `GPL`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris avahi=0.6.32~rc+dfsg-1ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.6.32~rc+dfsg-1ubuntu2.3.dsc' avahi_0.6.32~rc+dfsg-1ubuntu2.3.dsc 4414 SHA256:6f8eeca33df49a63a874c78cc0a2e637272259c02c8a8274f7d9ea95b651e5f5
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.6.32~rc+dfsg.orig.tar.gz' avahi_0.6.32~rc+dfsg.orig.tar.gz 665175 SHA256:84f609611323613c8635146d1a93be0914f1f7a8027d1d5e71cbbab156741dac
'http://archive.ubuntu.com/ubuntu/pool/main/a/avahi/avahi_0.6.32~rc+dfsg-1ubuntu2.3.debian.tar.xz' avahi_0.6.32~rc+dfsg-1ubuntu2.3.debian.tar.xz 34628 SHA256:4bb9ea6de721e4383dd2a4e6b489bf68b11a1516b432481cdb714ea0058919a5
```

### `dpkg` source package: `base-files=9.4ubuntu4.11`

Binary Packages:

- `base-files=9.4ubuntu4.11`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `base-passwd=3.5.39`

Binary Packages:

- `base-passwd=3.5.39`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.39
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.39.dsc' base-passwd_3.5.39.dsc 1720 SHA256:cfb464663fd23f5b64b7fdeb8860a754b28ee77b346bf2a362c36ceccb7a65ea
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.39.tar.xz' base-passwd_3.5.39.tar.xz 51560 SHA256:d827ce2d7b9b4b572527b2071f0e1354840a14c3a43a5081bcb31de400112803
```

### `dpkg` source package: `bash=4.3-14ubuntu1.4`

Binary Packages:

- `bash=4.3-14ubuntu1.4`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=4.3-14ubuntu1.4
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.3-14ubuntu1.4.dsc' bash_4.3-14ubuntu1.4.dsc 2346 SHA256:4eb674be50b59fcd6702176894b5c1c5898eecfb8f324401a0ae96d3cc13908f
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.3.orig.tar.gz' bash_4.3.orig.tar.gz 7516231 SHA256:b2fe79ddf9e7abdb4695e3070afa866d2a94a58d1cc9d731585330c753815491
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_4.3-14ubuntu1.4.debian.tar.xz' bash_4.3-14ubuntu1.4.debian.tar.xz 94248 SHA256:14cb48781639f7b06b73e9c1650b9848e9ffe7aa38b4f3ea1fcdb1af693e0bdb
```

### `dpkg` source package: `binutils=2.26.1-1ubuntu1~16.04.8`

Binary Packages:

- `binutils=2.26.1-1ubuntu1~16.04.8`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.26.1-1ubuntu1~16.04.8
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.26.1-1ubuntu1~16.04.8.dsc' binutils_2.26.1-1ubuntu1~16.04.8.dsc 4078 SHA256:60e2b2896c9b40414cd179a9f1d6d5d4d9849774848e3e9a0e14b04c989c6871
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.26.1.orig.tar.gz' binutils_2.26.1.orig.tar.gz 34868933 SHA256:dd9c3e37c266e4fefba68e444e2a00538b3c902dd31bf4912d90dca6d830a2a1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.26.1-1ubuntu1~16.04.8.diff.gz' binutils_2.26.1-1ubuntu1~16.04.8.diff.gz 235088 SHA256:93ab2695f3e686949f1b41a22465274aa8694c100db34f161d92a04a18664b63
```

### `dpkg` source package: `bzip2=1.0.6-8ubuntu0.2`

Binary Packages:

- `bzip2=1.0.6-8ubuntu0.2`
- `libbz2-1.0:amd64=1.0.6-8ubuntu0.2`
- `libbz2-dev:amd64=1.0.6-8ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8ubuntu0.2.dsc' bzip2_1.0.6-8ubuntu0.2.dsc 2173 SHA256:0afaa6cd738938e3e66814722960785a37b5e96ea68f27a99eb5fb52dfd763e8
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8ubuntu0.2.debian.tar.bz2' bzip2_1.0.6-8ubuntu0.2.debian.tar.bz2 61599 SHA256:df33ff2757f888545ecb2b0a53ade6cc697aa664ebd70e664674cdd3c2dd26df
```

### `dpkg` source package: `bzr=2.7.0-2ubuntu3.1`

Binary Packages:

- `bzr=2.7.0-2ubuntu3.1`
- `python-bzrlib=2.7.0-2ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/bzr/copyright`, `/usr/share/doc/python-bzrlib/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris bzr=2.7.0-2ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0-2ubuntu3.1.dsc' bzr_2.7.0-2ubuntu3.1.dsc 2669 SHA256:f0edd85fd866a668052d147f08d0a3b6cc31b872e56d8e8f999ac29a228e7877
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0.orig.tar.gz' bzr_2.7.0.orig.tar.gz 10944322 SHA256:5204369dc80e5738d7f4f5db5920e010cc5cb89097cf165462685ab70d9ab00b
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzr/bzr_2.7.0-2ubuntu3.1.debian.tar.xz' bzr_2.7.0-2ubuntu3.1.debian.tar.xz 42660 SHA256:7336e2ffc7f1f3a36d76c781f96076df4f81d140904163bb57f64f2a802f965b
```

### `dpkg` source package: `ca-certificates=20190110~16.04.1`

Binary Packages:

- `ca-certificates=20190110~16.04.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~16.04.1.dsc' ca-certificates_20190110~16.04.1.dsc 1969 SHA256:d71f5af4b47dd58e6a6221edbb2ca2102e7b24bb662eb41f6247131f36ddb26e
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110~16.04.1.tar.xz' ca-certificates_20190110~16.04.1.tar.xz 243584 SHA256:021db3fbd372f1caf1cdeccd117f9f271297603490b4381405422da481f40dcc
```

### `dpkg` source package: `cairo=1.14.6-1`

Binary Packages:

- `libcairo-gobject2:amd64=1.14.6-1`
- `libcairo-script-interpreter2:amd64=1.14.6-1`
- `libcairo2:amd64=1.14.6-1`
- `libcairo2-dev=1.14.6-1`

Licenses: (parsed from: `/usr/share/doc/libcairo-gobject2/copyright`, `/usr/share/doc/libcairo-script-interpreter2/copyright`, `/usr/share/doc/libcairo2/copyright`, `/usr/share/doc/libcairo2-dev/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.14.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.14.6-1.dsc' cairo_1.14.6-1.dsc 2865 SHA256:1e3f66a22c364646c05a127bc1fcfecd04476a994e30b2e251c03f9ff09d55ce
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.14.6.orig.tar.xz' cairo_1.14.6.orig.tar.xz 36040596 SHA256:613cb38447b76a93ff7235e17acd55a78b52ea84a9df128c3f2257f8eaa7b252
'http://archive.ubuntu.com/ubuntu/pool/main/c/cairo/cairo_1.14.6-1.debian.tar.xz' cairo_1.14.6-1.debian.tar.xz 27704 SHA256:83dbaa90cf79127db9c87edf3a4d38c193abc2d346555ab70bb619e899da5070
```

### `dpkg` source package: `cdebconf=0.198ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.198ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.198ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.198ubuntu1.dsc' cdebconf_0.198ubuntu1.dsc 2825 SHA256:d595d3afcad97026a763909a3efe66e296b02e432827d66a49c6f7088023a21e
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.198ubuntu1.tar.xz' cdebconf_0.198ubuntu1.tar.xz 269256 SHA256:2f3490411599195bd31fb1a29770694888c8295f9bf5012bfb4fa22ebd3990f1
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

### `dpkg` source package: `coreutils=8.25-2ubuntu3~16.04`

Binary Packages:

- `coreutils=8.25-2ubuntu3~16.04`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.25-2ubuntu3~16.04
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.25-2ubuntu3~16.04.dsc' coreutils_8.25-2ubuntu3~16.04.dsc 2095 SHA256:90f76af8f3b01d49dfdb1b2e03e7cfebf855567d378a57092286a7df0aa199a4
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.25.orig.tar.xz' coreutils_8.25.orig.tar.xz 5725008 SHA256:31e67c057a5b32a582f26408c789e11c2e8d676593324849dcf5779296cdce87
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.25-2ubuntu3~16.04.debian.tar.xz' coreutils_8.25-2ubuntu3~16.04.debian.tar.xz 28336 SHA256:f6fd913f2b0b08df9109308dfd1202b06060e130b8e6bf94daad32e86a3937cf
```

### `dpkg` source package: `cryptsetup=2:1.6.6-5ubuntu2.1`

Binary Packages:

- `libcryptsetup4:amd64=2:1.6.6-5ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libcryptsetup4/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cryptsetup=2:1.6.6-5ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cryptsetup/cryptsetup_1.6.6-5ubuntu2.1.dsc' cryptsetup_1.6.6-5ubuntu2.1.dsc 2650 SHA256:138cdb723928fcef0b15e427e2ee56511587751c7d63defe902f4e6daaff5e2e
'http://archive.ubuntu.com/ubuntu/pool/main/c/cryptsetup/cryptsetup_1.6.6.orig.tar.xz' cryptsetup_1.6.6.orig.tar.xz 1145940 SHA256:2d2ce28e4e1137dd599d87884b62ef6dbf14fd7848b2a2bf7d61cf125fbd8e6f
'http://archive.ubuntu.com/ubuntu/pool/main/c/cryptsetup/cryptsetup_1.6.6-5ubuntu2.1.debian.tar.xz' cryptsetup_1.6.6-5ubuntu2.1.debian.tar.xz 91808 SHA256:0979ff24a2c4ecc5471a017b286cd7a4ccc497e72854b02aadc21465dcce96e4
```

### `dpkg` source package: `cups=2.1.3-4ubuntu0.11`

Binary Packages:

- `libcups2:amd64=2.1.3-4ubuntu0.11`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.1.3-4ubuntu0.11
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3-4ubuntu0.11.dsc' cups_2.1.3-4ubuntu0.11.dsc 3755 SHA256:fb5a6bd7cea89db24de1d46afe4f38988cc9e74c047179b22c0fad074980430b
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3.orig.tar.bz2' cups_2.1.3.orig.tar.bz2 8832400 SHA256:36a70d43584aea2617da914b9331e23341c3501a8254c4d2eae9c11ec01fd4d3
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3-4ubuntu0.11.debian.tar.xz' cups_2.1.3-4ubuntu0.11.debian.tar.xz 356476 SHA256:57935d44ebbdf60d8b9cdb3ca1607a28ba74f3f439d9e31e413154a0cc42c97e
```

### `dpkg` source package: `curl=7.47.0-1ubuntu2.15`

Binary Packages:

- `curl=7.47.0-1ubuntu2.15`
- `libcurl3:amd64=7.47.0-1ubuntu2.15`
- `libcurl3-gnutls:amd64=7.47.0-1ubuntu2.15`
- `libcurl4-openssl-dev:amd64=7.47.0-1ubuntu2.15`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4-openssl-dev/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.47.0-1ubuntu2.15
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.47.0-1ubuntu2.15.dsc' curl_7.47.0-1ubuntu2.15.dsc 2733 SHA256:f69c59d02657dccb7fd3e5d25119ea89c84e7c8b6c9fad08bd0a5fbeb6ca07f0
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.47.0.orig.tar.gz' curl_7.47.0.orig.tar.gz 4563163 SHA256:df01bd42af361978d9de7de8529718bcafe01897a544a7650139a1954c55bdfe
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.47.0-1ubuntu2.15.debian.tar.xz' curl_7.47.0-1ubuntu2.15.debian.tar.xz 56200 SHA256:973830da76df0141298d9e4f76eff6df691af1c9354cb8ea3c2bc15157a63d14
```

### `dpkg` source package: `cyrus-sasl2=2.1.26.dfsg1-14ubuntu0.2`

Binary Packages:

- `libsasl2-2:amd64=2.1.26.dfsg1-14ubuntu0.2`
- `libsasl2-modules-db:amd64=2.1.26.dfsg1-14ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.26.dfsg1-14ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.dsc' cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.dsc 3416 SHA256:9214dcfd7ecfad26fcaa18cee72cc8ae8a49e9b6d789965c9fa2084ee527c8ba
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz' cyrus-sasl2_2.1.26.dfsg1.orig.tar.gz 1494337 SHA256:172c39555012f479543ce7305949db75df708771fe8f8b34248027f09e53bb85
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.debian.tar.xz' cyrus-sasl2_2.1.26.dfsg1-14ubuntu0.2.debian.tar.xz 95360 SHA256:14ced70b89687fd018df67edf9a0ab7b65fd2617a583f4b573c3a070100e1681
```

### `dpkg` source package: `dash=0.5.8-2.1ubuntu2`

Binary Packages:

- `dash=0.5.8-2.1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.8-2.1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.1ubuntu2.dsc' dash_0.5.8-2.1ubuntu2.dsc 1882 SHA256:16cb7f56041a9daa198728715318a5d88c19da01eb3ffccbc71f67304b077564
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8.orig.tar.gz' dash_0.5.8.orig.tar.gz 223028 SHA256:c6db3a237747b02d20382a761397563d813b306c020ae28ce25a1c3915fac60f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.8-2.1ubuntu2.diff.gz' dash_0.5.8-2.1ubuntu2.diff.gz 73054 SHA256:3c200a0b9c88b2e421bce9c717bf2ace7a9378c271a9b60463913e312424565a
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

### `dpkg` source package: `db5.3=5.3.28-11ubuntu0.2`

Binary Packages:

- `libdb5.3:amd64=5.3.28-11ubuntu0.2`
- `libdb5.3-dev=5.3.28-11ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-11ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-11ubuntu0.2.dsc' db5.3_5.3.28-11ubuntu0.2.dsc 3182 SHA256:cfb1c1fcd31bbbabe8b9fbea0fb0755091c1d5f4f745626342a46eea1448b066
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-11ubuntu0.2.debian.tar.xz' db5.3_5.3.28-11ubuntu0.2.debian.tar.xz 29312 SHA256:01f2cd8d0eda0f2b48b1aef7cb3babe94ecd14b1955de437b61e04f7b72bdd0c
```

### `dpkg` source package: `dbus=1.10.6-1ubuntu3.6`

Binary Packages:

- `libdbus-1-3:amd64=1.10.6-1ubuntu3.6`

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
$ apt-get source -qq --print-uris dbus=1.10.6-1ubuntu3.6
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6-1ubuntu3.6.dsc' dbus_1.10.6-1ubuntu3.6.dsc 3090 SHA256:40376cff2bd1f388c376a8c4cced48cf501d158b4a90334e2197ff7cc5249457
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6.orig.tar.gz' dbus_1.10.6.orig.tar.gz 1952608 SHA256:b5fefa08a77edd76cd64d872db949eebc02cf6f3f8be82e4bbc641742af5d35f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6-1ubuntu3.6.debian.tar.xz' dbus_1.10.6-1ubuntu3.6.debian.tar.xz 66784 SHA256:93d3eeed9d8d511cd3be493b052b2bf7c3a8a55dcb9ed115c5bf5c0f362562bd
```

### `dpkg` source package: `debconf=1.5.58ubuntu2`

Binary Packages:

- `debconf=1.5.58ubuntu2`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.58ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.58ubuntu2.dsc' debconf_1.5.58ubuntu2.dsc 2076 SHA256:dee4cd1507a5dd5e9614d05bbeae471ac1ce9c1dff3638dd4f2ab2b5d17b5b18
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.58ubuntu2.tar.gz' debconf_1.5.58ubuntu2.tar.gz 1007295 SHA256:222c50e853057713375bd9c05e32da4d616bb7a7d5aae5fa0b2b20bf7be2321e
```

### `dpkg` source package: `debianutils=4.7`

Binary Packages:

- `debianutils=4.7`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.7
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.7.dsc' debianutils_4.7.dsc 1703 SHA256:8dd1d66186f56bfe11bce5151b50c6909787d690bf90cc90212ea6deec186460
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.7.tar.xz' debianutils_4.7.tar.xz 156276 SHA256:a269cacd40f52f2fa5d5636357714a49e8538459c16d77772efaa23711fe53d9
```

### `dpkg` source package: `diffutils=1:3.3-3`

Binary Packages:

- `diffutils=1:3.3-3`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.3-3
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.3-3.dsc' diffutils_3.3-3.dsc 1438 SHA256:2ac1b096ab1f6f0c628d6952fe65336d0c792a3d4814fb73a81a3f1f518eff91
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.3.orig.tar.xz' diffutils_3.3.orig.tar.xz 1197832 SHA256:a25e89a8ab65fded1731e4186be1bb25cda967834b6df973599cdcd5abdfc19c
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.3-3.debian.tar.xz' diffutils_3.3-3.debian.tar.xz 18356 SHA256:a0d1946979196f793a8ca55b21ab7891227de08f15bac2578ed84f4911e8b755
```

### `dpkg` source package: `djvulibre=3.5.27.1-5ubuntu0.1`

Binary Packages:

- `libdjvulibre-dev:amd64=3.5.27.1-5ubuntu0.1`
- `libdjvulibre-text=3.5.27.1-5ubuntu0.1`
- `libdjvulibre21:amd64=3.5.27.1-5ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-dev/copyright`, `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris djvulibre=3.5.27.1-5ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-5ubuntu0.1.dsc' djvulibre_3.5.27.1-5ubuntu0.1.dsc 2586 SHA256:3650e888f71dbb3929bd663cd192f900e430db70894d75970555788229d0dd4e
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1.orig.tar.gz' djvulibre_3.5.27.1.orig.tar.gz 3231662 SHA256:77f07de3f1039aa19eba2eb3170d9ce9a0918ba7b704a59cfaf08f42fcc52144
'http://archive.ubuntu.com/ubuntu/pool/main/d/djvulibre/djvulibre_3.5.27.1-5ubuntu0.1.debian.tar.xz' djvulibre_3.5.27.1-5ubuntu0.1.debian.tar.xz 23060 SHA256:681551c3d72edf03c25b0be79bca38c220b4e97bbea718025506a807df63a5ac
```

### `dpkg` source package: `dpkg=1.18.4ubuntu1.6`

Binary Packages:

- `dpkg=1.18.4ubuntu1.6`
- `dpkg-dev=1.18.4ubuntu1.6`
- `libdpkg-perl=1.18.4ubuntu1.6`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.18.4ubuntu1.6
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.18.4ubuntu1.6.dsc' dpkg_1.18.4ubuntu1.6.dsc 2211 SHA256:77e2c2cd8f204e8ed805e771a3002af4b8781bd7dc3c288cd63885f6a0983c04
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.18.4ubuntu1.6.tar.xz' dpkg_1.18.4ubuntu1.6.tar.xz 4297512 SHA256:9e1e85e9a4d015b1b446d9da5cbec225830a6a1807a93ab32e559c06761187a5
```

### `dpkg` source package: `e2fsprogs=1.42.13-1ubuntu1.2`

Binary Packages:

- `comerr-dev=2.1-1.42.13-1ubuntu1.2`
- `e2fslibs:amd64=1.42.13-1ubuntu1.2`
- `e2fsprogs=1.42.13-1ubuntu1.2`
- `libcomerr2:amd64=1.42.13-1ubuntu1.2`
- `libss2:amd64=1.42.13-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/comerr-dev/copyright`, `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.42.13-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.42.13-1ubuntu1.2.dsc' e2fsprogs_1.42.13-1ubuntu1.2.dsc 2606 SHA256:22d89ad571441c943253fd2105236a034ff902b224a8ded651efd8aa148630b7
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.42.13.orig.tar.gz' e2fsprogs_1.42.13.orig.tar.gz 6511931 SHA256:59993ff3a44f82e504561e0ebf95e8c8fa9f9f5746eb6a7182239605d2a4e2d4
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.42.13-1ubuntu1.2.debian.tar.xz' e2fsprogs_1.42.13-1ubuntu1.2.debian.tar.xz 72228 SHA256:a5fb8efee48f188172d74d2084257ebe47dee11c46110a1b1990db65d64760fe
```

### `dpkg` source package: `elfutils=0.165-3ubuntu1.2`

Binary Packages:

- `libelf1:amd64=0.165-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libelf1/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris elfutils=0.165-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.165-3ubuntu1.2.dsc' elfutils_0.165-3ubuntu1.2.dsc 2393 SHA256:4219dab089e2857bb391e6e844d45fb40f841daf0e5aaf352f41893b991a4431
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.165.orig.tar.bz2' elfutils_0.165.orig.tar.bz2 6481128 SHA256:a7fc9277192caaa5f30b47e8c0518dbcfd8c4a19c6493a63d511d804290ce972
'http://archive.ubuntu.com/ubuntu/pool/main/e/elfutils/elfutils_0.165-3ubuntu1.2.debian.tar.xz' elfutils_0.165-3ubuntu1.2.debian.tar.xz 52004 SHA256:906e73b2e35b173731270d3bdd486a738670f9854740c352a49e5d72af03a08a
```

### `dpkg` source package: `expat=2.1.0-7ubuntu0.16.04.5`

Binary Packages:

- `libexpat1:amd64=2.1.0-7ubuntu0.16.04.5`
- `libexpat1-dev:amd64=2.1.0-7ubuntu0.16.04.5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.1.0-7ubuntu0.16.04.5
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0-7ubuntu0.16.04.5.dsc' expat_2.1.0-7ubuntu0.16.04.5.dsc 2387 SHA256:39c54dc2f9fa64fe3d1b2d216e0446de8dc37d2656a5597a8b344070ce2310e2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0.orig.tar.gz' expat_2.1.0.orig.tar.gz 562616 SHA256:823705472f816df21c8f6aa026dd162b280806838bb55b3432b0fb1fcca7eb86
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0-7ubuntu0.16.04.5.debian.tar.xz' expat_2.1.0-7ubuntu0.16.04.5.debian.tar.xz 23116 SHA256:f422e05965440e42c030904fc6605c39cb5477c114ac7b172427ce96d63e97e0
```

### `dpkg` source package: `explorercanvas=0.r3-4`

Binary Packages:

- `libjs-excanvas=0.r3-4`

Licenses: (parsed from: `/usr/share/doc/libjs-excanvas/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris explorercanvas=0.r3-4
'http://archive.ubuntu.com/ubuntu/pool/universe/e/explorercanvas/explorercanvas_0.r3-4.dsc' explorercanvas_0.r3-4.dsc 2000 SHA256:d168011ed1f110f82b5039a6b070167f1f262d2a35d7fa25a6b5462f73761637
'http://archive.ubuntu.com/ubuntu/pool/universe/e/explorercanvas/explorercanvas_0.r3.orig.tar.gz' explorercanvas_0.r3.orig.tar.gz 50748 SHA256:687af8084781b8eb3451fc55c88f6dfddc2b84428d197daf2c4c33fd5c55fed8
'http://archive.ubuntu.com/ubuntu/pool/universe/e/explorercanvas/explorercanvas_0.r3-4.debian.tar.xz' explorercanvas_0.r3-4.debian.tar.xz 2040 SHA256:afcaa3e229d9b423988fc30439aeee1599c9dac8ad94430309404f9cf9f0c11f
```

### `dpkg` source package: `fftw3=3.3.4-2ubuntu1`

Binary Packages:

- `libfftw3-double3:amd64=3.3.4-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libfftw3-double3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris fftw3=3.3.4-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.4-2ubuntu1.dsc' fftw3_3.3.4-2ubuntu1.dsc 2826 SHA256:ec8f6ad388190517b0816228bde513b9cf3f439b4bf2743976e4e2e827b2f037
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.4.orig.tar.gz' fftw3_3.3.4.orig.tar.gz 3940427 SHA256:8f0cde90929bc05587c3368d2f15cd0530a60b8a9912a8e2979a72dbe5af0982
'http://archive.ubuntu.com/ubuntu/pool/main/f/fftw3/fftw3_3.3.4-2ubuntu1.debian.tar.xz' fftw3_3.3.4-2ubuntu1.debian.tar.xz 12664 SHA256:c40d58a6d0f8bf17ecc272222c433972a313c069440bb83caf4d740b592a765c
```

### `dpkg` source package: `file=1:5.25-2ubuntu1.4`

Binary Packages:

- `file=1:5.25-2ubuntu1.4`
- `libmagic1:amd64=1:5.25-2ubuntu1.4`

Licenses: (parsed from: `/usr/share/doc/file/copyright`, `/usr/share/doc/libmagic1/copyright`)

- `BSD-2-Clause-alike`
- `BSD-2-Clause-netbsd`
- `BSD-2-Clause-regents`
- `MIT-Old-Style-with-legal-disclaimer-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris file=1:5.25-2ubuntu1.4
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.25-2ubuntu1.4.dsc' file_5.25-2ubuntu1.4.dsc 2252 SHA256:93852fd7fdd101bc1ce03d5036f7e1ffd0e4e5c9b381ff6dfd459796bc4bcdfa
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.25.orig.tar.xz' file_5.25.orig.tar.xz 537916 SHA256:8062cae8be640ff8583b8714e394dc73c3127d23f8fe9097f1433cdb36bff31c
'http://archive.ubuntu.com/ubuntu/pool/main/f/file/file_5.25-2ubuntu1.4.debian.tar.xz' file_5.25-2ubuntu1.4.debian.tar.xz 35264 SHA256:fc098703f4ad633e9ae084b49445418e6f04dcf45ebd1c3b542f51e690814330
```

### `dpkg` source package: `findutils=4.6.0+git+20160126-2`

Binary Packages:

- `findutils=4.6.0+git+20160126-2`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.6.0+git+20160126-2
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20160126-2.dsc' findutils_4.6.0+git+20160126-2.dsc 2163 SHA256:b4b644696cb66bdf72c59b25efe61800ae20fadfcc8e633cde240e4a956567a7
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20160126.orig.tar.xz' findutils_4.6.0+git+20160126.orig.tar.xz 1710188 SHA256:3d25cef1e0d5e098e323b06f66aea9f02f993a0cf6f13a437d712a8a722cd67e
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.6.0+git+20160126-2.debian.tar.xz' findutils_4.6.0+git+20160126-2.debian.tar.xz 25080 SHA256:58bf1e7a07fbac6a68693b099ec6fc9a6166e0b1b60cebe6bac3b90287a8dc3f
```

### `dpkg` source package: `fontconfig=2.11.94-0ubuntu1.1`

Binary Packages:

- `fontconfig=2.11.94-0ubuntu1.1`
- `fontconfig-config=2.11.94-0ubuntu1.1`
- `libfontconfig1:amd64=2.11.94-0ubuntu1.1`
- `libfontconfig1-dev:amd64=2.11.94-0ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.11.94-0ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.11.94-0ubuntu1.1.dsc' fontconfig_2.11.94-0ubuntu1.1.dsc 2287 SHA256:8d710d0aa61c6e9205e90ae78c0d7c726df35a24032dfd315065999238b7a05e
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.11.94.orig.tar.bz2' fontconfig_2.11.94.orig.tar.bz2 1567540 SHA256:d763c024df434146f3352448bc1f4554f390c8a48340cef7aa9cc44716a159df
'http://archive.ubuntu.com/ubuntu/pool/main/f/fontconfig/fontconfig_2.11.94-0ubuntu1.1.debian.tar.xz' fontconfig_2.11.94-0ubuntu1.1.debian.tar.xz 27932 SHA256:791c24b08a0698489c6acb84fdd23e5a79bb7d574691026906324adf4282d6ee
```

### `dpkg` source package: `fonts-dejavu=2.35-1`

Binary Packages:

- `fonts-dejavu-core=2.35-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`)

- `GPL-2`
- `GPL-2+`
- `bitstream-vera`

Source:

```console
$ apt-get source -qq --print-uris fonts-dejavu=2.35-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.35-1.dsc' fonts-dejavu_2.35-1.dsc 2583 SHA256:b02163fb4033175371a6cb6e39e193d438d910ab907eed5d14b47a3a5e57b392
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.35.orig.tar.bz2' fonts-dejavu_2.35.orig.tar.bz2 11493699 SHA256:646f5f52fbba7c6c82580a22cedb487f31ecf28aa28c71da5c38e04c2989abf5
'http://archive.ubuntu.com/ubuntu/pool/main/f/fonts-dejavu/fonts-dejavu_2.35-1.debian.tar.xz' fonts-dejavu_2.35-1.debian.tar.xz 10276 SHA256:5922af28fff7db4c5845c17623fe882028742f90db658f4183c21648e0cafd3d
```

### `dpkg` source package: `freetype=2.6.1-0.1ubuntu2.4`

Binary Packages:

- `libfreetype6:amd64=2.6.1-0.1ubuntu2.4`
- `libfreetype6-dev:amd64=2.6.1-0.1ubuntu2.4`

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
$ apt-get source -qq --print-uris freetype=2.6.1-0.1ubuntu2.4
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.6.1-0.1ubuntu2.4.dsc' freetype_2.6.1-0.1ubuntu2.4.dsc 2236 SHA256:6ce5d66f62309247b8248bd45fd1317b2f20b3de620217956b477f67d9e5b6b8
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.6.1.orig.tar.gz' freetype_2.6.1.orig.tar.gz 2411537 SHA256:ffaef13dc5ccc265e97519115a51a103e88b9d9d3223289bc1a98c0c2094d5b3
'http://archive.ubuntu.com/ubuntu/pool/main/f/freetype/freetype_2.6.1-0.1ubuntu2.4.diff.gz' freetype_2.6.1-0.1ubuntu2.4.diff.gz 45130 SHA256:cd72bfe2cdafbee867edbaefd16b38a16bd8fc8b1cca11546f216fdb9e6d8cfe
```

### `dpkg` source package: `gcc-5=5.4.0-6ubuntu1~16.04.12`

Binary Packages:

- `cpp-5=5.4.0-6ubuntu1~16.04.12`
- `g++-5=5.4.0-6ubuntu1~16.04.12`
- `gcc-5=5.4.0-6ubuntu1~16.04.12`
- `gcc-5-base:amd64=5.4.0-6ubuntu1~16.04.12`
- `libasan2:amd64=5.4.0-6ubuntu1~16.04.12`
- `libatomic1:amd64=5.4.0-6ubuntu1~16.04.12`
- `libcc1-0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libcilkrts5:amd64=5.4.0-6ubuntu1~16.04.12`
- `libgcc-5-dev:amd64=5.4.0-6ubuntu1~16.04.12`
- `libgomp1:amd64=5.4.0-6ubuntu1~16.04.12`
- `libitm1:amd64=5.4.0-6ubuntu1~16.04.12`
- `liblsan0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libmpx0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libquadmath0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libstdc++-5-dev:amd64=5.4.0-6ubuntu1~16.04.12`
- `libstdc++6:amd64=5.4.0-6ubuntu1~16.04.12`
- `libtsan0:amd64=5.4.0-6ubuntu1~16.04.12`
- `libubsan0:amd64=5.4.0-6ubuntu1~16.04.12`

Licenses: (parsed from: `/usr/share/doc/cpp-5/copyright`, `/usr/share/doc/g++-5/copyright`, `/usr/share/doc/gcc-5/copyright`, `/usr/share/doc/gcc-5-base/copyright`, `/usr/share/doc/libasan2/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-5-dev/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libmpx0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-5-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gcc-5=5.4.0-6ubuntu1~16.04.12
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-5/gcc-5_5.4.0-6ubuntu1~16.04.12.dsc' gcc-5_5.4.0-6ubuntu1~16.04.12.dsc 28298 SHA256:4f6afb05c2f291aff65695bbf9f561106789f48b89d34d80ded9797c2acb4499
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-5/gcc-5_5.4.0.orig.tar.gz' gcc-5_5.4.0.orig.tar.gz 73530162 SHA256:00f73e8382aa8653aa501ce2263597c2c4429912bfa18102f47cc362f00ed88d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-5/gcc-5_5.4.0-6ubuntu1~16.04.12.diff.gz' gcc-5_5.4.0-6ubuntu1~16.04.12.diff.gz 1486130 SHA256:d0c772f3f39df2dedaf74b8e5ded301ae77a6f9d1fca4072690d812bd3b0bb69
```

### `dpkg` source package: `gcc-defaults=1.150ubuntu1`

Binary Packages:

- `cpp=4:5.3.1-1ubuntu1`
- `g++=4:5.3.1-1ubuntu1`
- `gcc=4:5.3.1-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.150ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.150ubuntu1.dsc' gcc-defaults_1.150ubuntu1.dsc 12634 SHA256:5f538e1bb59109b47d820cdd056993d462f24468c67f6a1a005db389dffa8ee2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.150ubuntu1.tar.gz' gcc-defaults_1.150ubuntu1.tar.gz 73857 SHA256:cadaf435151fb1b901b0351d20a9981fe33d94fbb1ab14bd9960095b673ce6ed
```

### `dpkg` source package: `gccgo-6=6.0.1-0ubuntu1`

Binary Packages:

- `gcc-6-base:amd64=6.0.1-0ubuntu1`
- `libgcc1:amd64=1:6.0.1-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-6-base/copyright`, `/usr/share/doc/libgcc1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris gccgo-6=6.0.1-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gccgo-6/gccgo-6_6.0.1-0ubuntu1.dsc' gccgo-6_6.0.1-0ubuntu1.dsc 11285 SHA256:4c02817baac83492323ebe7800d44de609eca147518682307a3bad2bd5134129
'http://archive.ubuntu.com/ubuntu/pool/main/g/gccgo-6/gccgo-6_6.0.1.orig.tar.gz' gccgo-6_6.0.1.orig.tar.gz 76335555 SHA256:daff7478ce52d00572683547c810bf50652a9057c33e3ce703c9f0baae28f4c3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gccgo-6/gccgo-6_6.0.1-0ubuntu1.diff.gz' gccgo-6_6.0.1-0ubuntu1.diff.gz 633954 SHA256:839eea6c2d23670f09b642864ff61e3097b47391cb508a5997538750ff8678f6
```

### `dpkg` source package: `gdbm=1.8.3-13.1`

Binary Packages:

- `libgdbm-dev=1.8.3-13.1`
- `libgdbm3:amd64=1.8.3-13.1`

Licenses: (parsed from: `/usr/share/doc/libgdbm-dev/copyright`, `/usr/share/doc/libgdbm3/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.8.3-13.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.8.3-13.1.dsc' gdbm_1.8.3-13.1.dsc 1830 SHA256:b1d8bef30edc491315c337930cbe2b61f44f55035adfc26ae945bab5ca57d5c9
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.8.3.orig.tar.bz2' gdbm_1.8.3.orig.tar.bz2 172796 SHA256:1d5995b6e9e6be4ff62c8126d019f184a083dd8e6f75f6c74b9fe023b5b9440e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.8.3-13.1.debian.tar.xz' gdbm_1.8.3-13.1.debian.tar.xz 14748 SHA256:251401e1f5210226f384e936b1b7ea1df40119a918d9f3dbf48b2e51d4df8983
```

### `dpkg` source package: `gdk-pixbuf=2.32.2-1ubuntu1.6`

Binary Packages:

- `gir1.2-gdkpixbuf-2.0:amd64=2.32.2-1ubuntu1.6`
- `libgdk-pixbuf2.0-0:amd64=2.32.2-1ubuntu1.6`
- `libgdk-pixbuf2.0-common=2.32.2-1ubuntu1.6`
- `libgdk-pixbuf2.0-dev=2.32.2-1ubuntu1.6`

Licenses: (parsed from: `/usr/share/doc/gir1.2-gdkpixbuf-2.0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-dev/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.32.2-1ubuntu1.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2-1ubuntu1.6.dsc' gdk-pixbuf_2.32.2-1ubuntu1.6.dsc 2912 SHA256:ada3327bb6913d7056cd8de4360d3cbc359ca04e526337d406e4cef3ab640965
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2.orig.tar.xz' gdk-pixbuf_2.32.2.orig.tar.xz 2429268 SHA256:d3ab06fc123b13effed4c27c77cebdfad2173ff20628d82c397b7660ae926145
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2-1ubuntu1.6.debian.tar.xz' gdk-pixbuf_2.32.2-1ubuntu1.6.debian.tar.xz 19956 SHA256:89b307e6007e8acec4038bdc994c81d36f3371d3ea5ccc2877d697cb0a6c445b
```

### `dpkg` source package: `git=1:2.7.4-0ubuntu1.9`

Binary Packages:

- `git=1:2.7.4-0ubuntu1.9`
- `git-man=1:2.7.4-0ubuntu1.9`

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
$ apt-get source -qq --print-uris git=1:2.7.4-0ubuntu1.9
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.7.4-0ubuntu1.9.dsc' git_2.7.4-0ubuntu1.9.dsc 2897 SHA256:a7c83276d876be29656f08a3e1f6ef153c21f6556b31bb0abb9cbb15c0fd0b03
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.7.4.orig.tar.xz' git_2.7.4.orig.tar.xz 3909636 SHA256:dee574defbe05ec7356a0842ddbda51315926f2fa7e39c2539f2c3dcc52e457b
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.7.4-0ubuntu1.9.debian.tar.xz' git_2.7.4-0ubuntu1.9.debian.tar.xz 572052 SHA256:2ab39ce8a9d1d94a549be4d086e6b59ae2c4201bc022dd1368a38eebe98cdf24
```

### `dpkg` source package: `glib2.0=2.48.2-0ubuntu4.6`

Binary Packages:

- `libglib2.0-0:amd64=2.48.2-0ubuntu4.6`
- `libglib2.0-bin=2.48.2-0ubuntu4.6`
- `libglib2.0-data=2.48.2-0ubuntu4.6`
- `libglib2.0-dev=2.48.2-0ubuntu4.6`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-bin/copyright`, `/usr/share/doc/libglib2.0-data/copyright`, `/usr/share/doc/libglib2.0-dev/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.48.2-0ubuntu4.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2-0ubuntu4.6.dsc' glib2.0_2.48.2-0ubuntu4.6.dsc 2865 SHA256:a60904a518cd721a2d69730c568bccc2664d90486eecbfaca96afc2ab0ad0051
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2.orig.tar.xz' glib2.0_2.48.2.orig.tar.xz 6408644 SHA256:f25e751589cb1a58826eac24fbd4186cda4518af772806b666a3f91f66e6d3f4
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2-0ubuntu4.6.debian.tar.xz' glib2.0_2.48.2-0ubuntu4.6.debian.tar.xz 77696 SHA256:1ee4dc4c0d01e438beca989c6b49f2a73150db2c861ab3b751c833806b8bf48c
```

### `dpkg` source package: `glibc=2.23-0ubuntu11.2`

Binary Packages:

- `libc-bin=2.23-0ubuntu11.2`
- `libc-dev-bin=2.23-0ubuntu11.2`
- `libc6:amd64=2.23-0ubuntu11.2`
- `libc6-dev:amd64=2.23-0ubuntu11.2`
- `multiarch-support=2.23-0ubuntu11.2`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.23-0ubuntu11.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23-0ubuntu11.2.dsc' glibc_2.23-0ubuntu11.2.dsc 8547 SHA256:bf8f1067f5524046070f3cac025888651a99447cc789a0e5b9eafa97a3571f9c
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23.orig.tar.xz' glibc_2.23.orig.tar.xz 13849968 SHA256:bf6c528eeebefcacc295270068b79330c1fb2b22458ff66285b4175d23442c96
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23-0ubuntu11.2.debian.tar.xz' glibc_2.23-0ubuntu11.2.debian.tar.xz 1357888 SHA256:04ebe665c81c24481057a4facd6c07e9c43319f6a2dc98fce18ecd247d1af96d
```

### `dpkg` source package: `gmp=2:6.1.0+dfsg-2`

Binary Packages:

- `libgmp-dev:amd64=2:6.1.0+dfsg-2`
- `libgmp10:amd64=2:6.1.0+dfsg-2`
- `libgmpxx4ldbl:amd64=2:6.1.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp-dev/copyright`, `/usr/share/doc/libgmp10/copyright`, `/usr/share/doc/libgmpxx4ldbl/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.1.0+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.0+dfsg-2.dsc' gmp_6.1.0+dfsg-2.dsc 2161 SHA256:a790b4fea2792f968014a3ef41ea749dcc6687bcb33aa5bea59400ccd101337e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.0+dfsg.orig.tar.xz' gmp_6.1.0+dfsg.orig.tar.xz 1786120 SHA256:78a74cfd933bbdf7e93909a6069e53e8aba8389e9b3880300c926da7a7d55632
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.1.0+dfsg-2.debian.tar.xz' gmp_6.1.0+dfsg-2.debian.tar.xz 20576 SHA256:c933e3cb45cd4101cc0604b5bc0fb96d6067b3614e730dbf26588985720ba581
```

### `dpkg` source package: `gnupg=1.4.20-1ubuntu3.3`

Binary Packages:

- `gnupg=1.4.20-1ubuntu3.3`
- `gpgv=1.4.20-1ubuntu3.3`

Licenses: (parsed from: `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gpgv/copyright`)

- `GPL-3`
- `GPL-3+ with OpenSSL exception`
- `RFC-Reference`

Source:

```console
$ apt-get source -qq --print-uris gnupg=1.4.20-1ubuntu3.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg/gnupg_1.4.20-1ubuntu3.3.dsc' gnupg_1.4.20-1ubuntu3.3.dsc 2166 SHA256:5703bb24fd96c217a2d95bbab61d887a511cfcf8fb2e1dc06b801316c98ee33f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg/gnupg_1.4.20.orig.tar.gz' gnupg_1.4.20.orig.tar.gz 5156447 SHA256:dc1f1a6028488303a4efb01aadda480b9cd0f49f65aef94c432628fdd127e586
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg/gnupg_1.4.20-1ubuntu3.3.debian.tar.xz' gnupg_1.4.20-1ubuntu3.3.debian.tar.xz 42452 SHA256:b12190aba71ef462a9ba164f2c5713474f0451c3dd6f1fdabb5f8ecfe4ee2938
```

### `dpkg` source package: `gnutls28=3.4.10-4ubuntu1.8`

Binary Packages:

- `libgnutls30:amd64=3.4.10-4ubuntu1.8`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `CC0 license`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `GPLv3+`
- `LGPL`
- `LGPL-3`
- `LGPL2.1`
- `The main library is licensed under GNU Lesser`
- `nonstandard, see below`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.4.10-4ubuntu1.8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.4.10-4ubuntu1.8.dsc' gnutls28_3.4.10-4ubuntu1.8.dsc 2439 SHA256:b65dc2e562dc61f1aa7baf41ba564b71826d1e2af7f54249c9f7e2917692cde5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.4.10.orig.tar.xz' gnutls28_3.4.10.orig.tar.xz 6645892 SHA256:6a32c2b4acbd33ff7eefcbd1357009da04c94c60146ef61320b6c076b1bdf59f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.4.10-4ubuntu1.8.debian.tar.xz' gnutls28_3.4.10-4ubuntu1.8.debian.tar.xz 113000 SHA256:41efab50985952713e5eb46472653a44889ac33de6985e43d6082c45e0a6d55c
```

### `dpkg` source package: `gobject-introspection=1.46.0-3ubuntu1`

Binary Packages:

- `gir1.2-freedesktop:amd64=1.46.0-3ubuntu1`
- `gir1.2-glib-2.0:amd64=1.46.0-3ubuntu1`
- `libgirepository-1.0-1:amd64=1.46.0-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gir1.2-freedesktop/copyright`, `/usr/share/doc/gir1.2-glib-2.0/copyright`, `/usr/share/doc/libgirepository-1.0-1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris gobject-introspection=1.46.0-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.46.0-3ubuntu1.dsc' gobject-introspection_1.46.0-3ubuntu1.dsc 3004 SHA256:a1e53758fae32e7d6ad2ef323264ac591694d39e661ad1636fb926ddb8f19813
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.46.0.orig.tar.xz' gobject-introspection_1.46.0.orig.tar.xz 1359436 SHA256:6658bd3c2b8813eb3e2511ee153238d09ace9d309e4574af27443d87423e4233
'http://archive.ubuntu.com/ubuntu/pool/main/g/gobject-introspection/gobject-introspection_1.46.0-3ubuntu1.debian.tar.xz' gobject-introspection_1.46.0-3ubuntu1.debian.tar.xz 19584 SHA256:9c8c898f33d1629ec267700010a34715a7f4f854af983a9d3f038dbc55b68792
```

### `dpkg` source package: `graphite2=1.3.10-0ubuntu0.16.04.1`

Binary Packages:

- `libgraphite2-3:amd64=1.3.10-0ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libgraphite2-3/copyright`)

- `Artistic`
- `GPL`
- `GPL-1+`
- `GPL1+ | Artistic`
- `LGPL | other`
- `LGPL-2`
- `LGPL-2+`
- `MPL-1.1 | GPL-2 | LGPL-2.1`
- `other`

Source:

```console
$ apt-get source -qq --print-uris graphite2=1.3.10-0ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.10-0ubuntu0.16.04.1.dsc' graphite2_1.3.10-0ubuntu0.16.04.1.dsc 2238 SHA256:a1bb1b86e8f56a790b9e1336f0c75a10f76d9a0f12c0bd0fc24c8a5709a6c4b1
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.10.orig.tar.gz' graphite2_1.3.10.orig.tar.gz 3889647 SHA256:90fde3b2f9ea95d68ffb19278d07d9b8a7efa5ba0e413bebcea802ce05cda1ae
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphite2/graphite2_1.3.10-0ubuntu0.16.04.1.debian.tar.xz' graphite2_1.3.10-0ubuntu0.16.04.1.debian.tar.xz 10016 SHA256:05b62d5770153e989fa452e6097fd201c538a97fdbbbc7a2034d89717f57e448
```

### `dpkg` source package: `graphviz=2.38.0-12ubuntu2.1`

Binary Packages:

- `libcdt5=2.38.0-12ubuntu2.1`
- `libcgraph6=2.38.0-12ubuntu2.1`
- `libgraphviz-dev=2.38.0-12ubuntu2.1`
- `libgvc6=2.38.0-12ubuntu2.1`
- `libgvc6-plugins-gtk=2.38.0-12ubuntu2.1`
- `libgvpr2=2.38.0-12ubuntu2.1`
- `libpathplan4=2.38.0-12ubuntu2.1`
- `libxdot4=2.38.0-12ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libcdt5/copyright`, `/usr/share/doc/libcgraph6/copyright`, `/usr/share/doc/libgraphviz-dev/copyright`, `/usr/share/doc/libgvc6/copyright`, `/usr/share/doc/libgvc6-plugins-gtk/copyright`, `/usr/share/doc/libgvpr2/copyright`, `/usr/share/doc/libpathplan4/copyright`, `/usr/share/doc/libxdot4/copyright`)

- `GPL-2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris graphviz=2.38.0-12ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphviz/graphviz_2.38.0-12ubuntu2.1.dsc' graphviz_2.38.0-12ubuntu2.1.dsc 3301 SHA256:5ba3bff345f80201306631e06a284d348a509ac0ed4ef8118ab7706936f2f169
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphviz/graphviz_2.38.0.orig.tar.gz' graphviz_2.38.0.orig.tar.gz 25848858 SHA256:81aa238d9d4a010afa73a9d2a704fc3221c731e1e06577c2ab3496bdef67859e
'http://archive.ubuntu.com/ubuntu/pool/main/g/graphviz/graphviz_2.38.0-12ubuntu2.1.debian.tar.xz' graphviz_2.38.0-12ubuntu2.1.debian.tar.xz 43652 SHA256:5e0396dad5766cbd3ebaf62412ed41b2605faf0866402f696909e385acdd1cfb
```

### `dpkg` source package: `grep=2.25-1~16.04.1`

Binary Packages:

- `grep=2.25-1~16.04.1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=2.25-1~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_2.25-1~16.04.1.dsc' grep_2.25-1~16.04.1.dsc 1971 SHA256:a41abfce1c101fd14d435cafbf15c2ecec5dbb01c157a52a2d24a6baae387048
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_2.25.orig.tar.xz' grep_2.25.orig.tar.xz 1327856 SHA256:e21e83bac50450e0d0d61a42c154ee0dceaacdbf4f604ef6e79071cb8e596830
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_2.25-1~16.04.1.debian.tar.bz2' grep_2.25-1~16.04.1.debian.tar.bz2 108236 SHA256:10a95f4bdee1d2beb05ab1727e114d1f0737f5a917e88b973200a38146a2e085
```

### `dpkg` source package: `gtk+2.0=2.24.30-1ubuntu1.16.04.2`

Binary Packages:

- `libgtk2.0-0:amd64=2.24.30-1ubuntu1.16.04.2`
- `libgtk2.0-common=2.24.30-1ubuntu1.16.04.2`

Licenses: (parsed from: `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

- `LGPL-2`
- `other`

Source:

```console
$ apt-get source -qq --print-uris gtk+2.0=2.24.30-1ubuntu1.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.30-1ubuntu1.16.04.2.dsc' gtk+2.0_2.24.30-1ubuntu1.16.04.2.dsc 3981 SHA256:84256a4ecd7b29bfc080ec5cbbdf6527f6610d06b34cf3cae2265846915a5ef6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.30.orig.tar.xz' gtk+2.0_2.24.30.orig.tar.xz 12800276 SHA256:0d15cec3b6d55c60eac205b1f3ba81a1ed4eadd9d0f8e7c508bc7065d0c4ca50
'http://archive.ubuntu.com/ubuntu/pool/main/g/gtk+2.0/gtk+2.0_2.24.30-1ubuntu1.16.04.2.debian.tar.xz' gtk+2.0_2.24.30-1ubuntu1.16.04.2.debian.tar.xz 107272 SHA256:7481a47cc636f102d5db761e2cae0f3d82a5b644b255faedbc8f2bd25ef4fe62
```

### `dpkg` source package: `gzip=1.6-4ubuntu1`

Binary Packages:

- `gzip=1.6-4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.6-4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-4ubuntu1.dsc' gzip_1.6-4ubuntu1.dsc 1907 SHA256:77c1d15c52947d50656365597802c586249d26a4f56c8075f5d94b4634d11465
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6.orig.tar.gz' gzip_1.6.orig.tar.gz 1074924 SHA256:97eb83b763d9e5ad35f351fe5517e6b71521d7aac7acf3e3cacdb6b1496d8f7e
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.6-4ubuntu1.debian.tar.xz' gzip_1.6-4ubuntu1.debian.tar.xz 14932 SHA256:9a3e558c87a78bf65f9b9c48d718b3ef0bb69e0cf07617f44e37f41ba5f7b006
```

### `dpkg` source package: `harfbuzz=1.0.1-1ubuntu0.1`

Binary Packages:

- `libharfbuzz0b:amd64=1.0.1-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=1.0.1-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.0.1-1ubuntu0.1.dsc' harfbuzz_1.0.1-1ubuntu0.1.dsc 2820 SHA256:87239e2ef7544ba3d73ea2912d6243a3204e879b20ffd1b97af5f6ab592cb242
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.0.1.orig.tar.bz2' harfbuzz_1.0.1.orig.tar.bz2 1211877 SHA256:32a1a7ad584a2f2cfba5c1d234d046c0521e86e7a21d403e15e89aa509ef0ea8
'http://archive.ubuntu.com/ubuntu/pool/main/h/harfbuzz/harfbuzz_1.0.1-1ubuntu0.1.debian.tar.xz' harfbuzz_1.0.1-1ubuntu0.1.debian.tar.xz 8952 SHA256:5b8b03fa2a6ed98e0e90b2d279e6d477c8d692b8ed772e35cab1f4cb51a20d10
```

### `dpkg` source package: `heimdal=1.7~git20150920+dfsg-4ubuntu1.16.04.1`

Binary Packages:

- `libasn1-8-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libgssapi3-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libhcrypto4-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libheimbase1-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libheimntlm0-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libhx509-5-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libkrb5-26-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libroken18-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`
- `libwind0-heimdal:amd64=1.7~git20150920+dfsg-4ubuntu1.16.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris heimdal=1.7~git20150920+dfsg-4ubuntu1.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.dsc' heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.dsc 3766 SHA256:068e9500ada30813dac1721e71ec4ad4129142b960b7fe19487db1892865c82e
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_1.7~git20150920+dfsg.orig.tar.gz' heimdal_1.7~git20150920+dfsg.orig.tar.gz 8979556 SHA256:fb3cb14b1d8cd25e5b8f73ab5d6de434b91cdebef2dd3d8efc96a403d0750d50
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.debian.tar.xz' heimdal_1.7~git20150920+dfsg-4ubuntu1.16.04.1.debian.tar.xz 65512 SHA256:f30b75cde57b7848f70e923d705fdd1eaa805c840c4fe37585af332fc1583099
```

### `dpkg` source package: `hicolor-icon-theme=0.15-0ubuntu1.1`

Binary Packages:

- `hicolor-icon-theme=0.15-0ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/hicolor-icon-theme/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris hicolor-icon-theme=0.15-0ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.15-0ubuntu1.1.dsc' hicolor-icon-theme_0.15-0ubuntu1.1.dsc 2084 SHA256:b2f4740a56d5911937dde4c840c416577393eae349683882f7470fc52e2e9b2b
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.15.orig.tar.xz' hicolor-icon-theme_0.15.orig.tar.xz 51056 SHA256:9cc45ac3318c31212ea2d8cb99e64020732393ee7630fa6c1810af5f987033cc
'http://archive.ubuntu.com/ubuntu/pool/main/h/hicolor-icon-theme/hicolor-icon-theme_0.15-0ubuntu1.1.debian.tar.xz' hicolor-icon-theme_0.15-0ubuntu1.1.debian.tar.xz 3356 SHA256:b9ffb5a9fd267257e072d065e8be2aed82aeff5cb7631cd413cf5a82632727fc
```

### `dpkg` source package: `hostname=3.16ubuntu2`

Binary Packages:

- `hostname=3.16ubuntu2`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.16ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.16ubuntu2.dsc' hostname_3.16ubuntu2.dsc 1573 SHA256:dcffca698d9f428a83b744d638ef2069252395d9b5d1a3098578f01b0cb347a5
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.16ubuntu2.tar.gz' hostname_3.16ubuntu2.tar.gz 14378 SHA256:e0a38fa03b66abd428e119e5af2cccb78a0462cdb58e2e540e66d964e2719195
```

### `dpkg` source package: `icu=55.1-7ubuntu0.5`

Binary Packages:

- `icu-devtools=55.1-7ubuntu0.5`
- `libicu-dev:amd64=55.1-7ubuntu0.5`
- `libicu55:amd64=55.1-7ubuntu0.5`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=55.1-7ubuntu0.5
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1-7ubuntu0.5.dsc' icu_55.1-7ubuntu0.5.dsc 2162 SHA256:caf3f1a7de6e0f4c75128d7f3aec0e1e1e532739220ab0626ca3a256243584b0
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1.orig.tar.gz' icu_55.1.orig.tar.gz 25600847 SHA256:e16b22cbefdd354bec114541f7849a12f8fc2015320ca5282ee4fd787571457b
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1-7ubuntu0.5.debian.tar.xz' icu_55.1-7ubuntu0.5.debian.tar.xz 32320 SHA256:9bcc091972d7de4cd6589578b91a090c0f8f1b05d1344f10923ac2c339188c7f
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

### `dpkg` source package: `imagemagick=8:6.8.9.9-7ubuntu5.15`

Binary Packages:

- `imagemagick=8:6.8.9.9-7ubuntu5.15`
- `imagemagick-6.q16=8:6.8.9.9-7ubuntu5.15`
- `imagemagick-common=8:6.8.9.9-7ubuntu5.15`
- `libmagickcore-6-arch-config:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickcore-6-headers=8:6.8.9.9-7ubuntu5.15`
- `libmagickcore-6.q16-2:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickcore-6.q16-2-extra:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickcore-6.q16-dev:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickcore-dev=8:6.8.9.9-7ubuntu5.15`
- `libmagickwand-6-headers=8:6.8.9.9-7ubuntu5.15`
- `libmagickwand-6.q16-2:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickwand-6.q16-dev:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickwand-dev=8:6.8.9.9-7ubuntu5.15`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/imagemagick-common/copyright`, `/usr/share/doc/libmagickcore-6-arch-config/copyright`, `/usr/share/doc/libmagickcore-6-headers/copyright`, `/usr/share/doc/libmagickcore-6.q16-2/copyright`, `/usr/share/doc/libmagickcore-6.q16-2-extra/copyright`, `/usr/share/doc/libmagickcore-6.q16-dev/copyright`, `/usr/share/doc/libmagickcore-dev/copyright`, `/usr/share/doc/libmagickwand-6-headers/copyright`, `/usr/share/doc/libmagickwand-6.q16-2/copyright`, `/usr/share/doc/libmagickwand-6.q16-dev/copyright`, `/usr/share/doc/libmagickwand-dev/copyright`)

- `Artistic`
- `GPL-1`
- `ImageMagick`
- `ImageMagickLicensePartEZXML`
- `ImageMagickLicensePartFIG`
- `ImageMagickLicensePartGsview`
- `ImageMagickLicensePartOpenSSH`
- `ImageMagickPartGraphicsMagick`
- `ImageMagickPartlibjpeg`
- `ImageMagickPartlibsquish`
- `Magick++`
- `Perllikelicence`
- `TatcherUlrichPublicDomain`

Source:

```console
$ apt-get source -qq --print-uris imagemagick=8:6.8.9.9-7ubuntu5.15
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.8.9.9-7ubuntu5.15.dsc' imagemagick_6.8.9.9-7ubuntu5.15.dsc 4337 SHA256:46263aa987b6f93e2214cda73c49e2a46a20ff407cb807eb379dcc402056cf2c
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.8.9.9.orig.tar.xz' imagemagick_6.8.9.9.orig.tar.xz 7891624 SHA256:a4cccc70179ff2c67550e063cdcb2e62907338ef3e68b45bb1c41931e515b3eb
'http://archive.ubuntu.com/ubuntu/pool/main/i/imagemagick/imagemagick_6.8.9.9-7ubuntu5.15.debian.tar.xz' imagemagick_6.8.9.9-7ubuntu5.15.debian.tar.xz 318708 SHA256:51dde4d550d998d8f771421b512ccde3c4cc2d368aaeb6d318da15f7e7d14295
```

### `dpkg` source package: `init-system-helpers=1.29ubuntu4`

Binary Packages:

- `init=1.29ubuntu4`
- `init-system-helpers=1.29ubuntu4`

Licenses: (parsed from: `/usr/share/doc/init/copyright`, `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.29ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.29ubuntu4.dsc' init-system-helpers_1.29ubuntu4.dsc 2047 SHA256:10991f100d3d1dd450652826e382cda3037243d1268acef903e9fed977840486
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.29ubuntu4.tar.xz' init-system-helpers_1.29ubuntu4.tar.xz 58648 SHA256:f0ae7b86351157ed635a97751ea82894d0352d716dfb232c2dd4bb557f30f21f
```

### `dpkg` source package: `insserv=1.14.0-5ubuntu3`

Binary Packages:

- `insserv=1.14.0-5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/insserv/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris insserv=1.14.0-5ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/i/insserv/insserv_1.14.0-5ubuntu3.dsc' insserv_1.14.0-5ubuntu3.dsc 2033 SHA256:30a8e6edc9c105803dfc98d733ba0ed8f0aaf81c4aa4f5ba132241b9a1fcb3a2
'http://archive.ubuntu.com/ubuntu/pool/main/i/insserv/insserv_1.14.0.orig.tar.gz' insserv_1.14.0.orig.tar.gz 53851 SHA256:da74dcf5225a00aa8aef4d5afc6a20e009b2ed9af328dabd55fef1cb3a32140e
'http://archive.ubuntu.com/ubuntu/pool/main/i/insserv/insserv_1.14.0-5ubuntu3.debian.tar.xz' insserv_1.14.0-5ubuntu3.debian.tar.xz 48124 SHA256:a4d0d0703fa398819ab7b4cad573f334feee80aac5520202457519e737b4648a
```

### `dpkg` source package: `isl=0.16.1-1`

Binary Packages:

- `libisl15:amd64=0.16.1-1`

Licenses: (parsed from: `/usr/share/doc/libisl15/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.16.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.16.1-1.dsc' isl_0.16.1-1.dsc 1857 SHA256:d6428f2a18db18cdfbff3be72b33dbc4b1838d5efea97ae5715c24115250be91
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.16.1.orig.tar.gz' isl_0.16.1.orig.tar.gz 1889136 SHA256:fb34703bd694622aef92164bad983c15ec04274edbe19e614d9ecda54b85603d
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.16.1-1.debian.tar.xz' isl_0.16.1-1.debian.tar.xz 21152 SHA256:d1ee2fd3a5b7289ba7f66fe443f57f5b6f4297a3a9164d840fafc9c37d3ec632
```

### `dpkg` source package: `jasper=1.900.1-debian1-2.4ubuntu1.2`

Binary Packages:

- `libjasper-dev=1.900.1-debian1-2.4ubuntu1.2`
- `libjasper1:amd64=1.900.1-debian1-2.4ubuntu1.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `jbigkit=2.1-3.1`

Binary Packages:

- `libjbig-dev:amd64=2.1-3.1`
- `libjbig0:amd64=2.1-3.1`

Licenses: (parsed from: `/usr/share/doc/libjbig-dev/copyright`, `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1.dsc' jbigkit_2.1-3.1.dsc 1299 SHA256:62c8812d508958c5d35f2b1579dc3052fb5bd8d2e77d023fad064c4b48c8c3f8
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1.debian.tar.xz' jbigkit_2.1-3.1.debian.tar.xz 7600 SHA256:ebc3c52deaf37d52baea54d648a713640dc262926abda7bf05cd08e7db5dd1ee
```

### `dpkg` source package: `jquery=1.11.3+dfsg-4`

Binary Packages:

- `libjs-jquery=1.11.3+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libjs-jquery/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris jquery=1.11.3+dfsg-4
'http://archive.ubuntu.com/ubuntu/pool/main/j/jquery/jquery_1.11.3+dfsg-4.dsc' jquery_1.11.3+dfsg-4.dsc 2068 SHA256:480550fa1f1753e1ddfab71b46a16bc2bc75f2b045bbb8d77e52fac0cca43861
'http://archive.ubuntu.com/ubuntu/pool/main/j/jquery/jquery_1.11.3+dfsg.orig.tar.gz' jquery_1.11.3+dfsg.orig.tar.gz 525555 SHA256:7f0f998d792f5d030a9e7e8c3d0648d81852a8098a8758817837f070aec770ab
'http://archive.ubuntu.com/ubuntu/pool/main/j/jquery/jquery_1.11.3+dfsg-4.debian.tar.xz' jquery_1.11.3+dfsg-4.debian.tar.xz 7232 SHA256:c632f57fd361b19ee8d693f955fc1e562111f37622d129bac2570d78514f0473
```

### `dpkg` source package: `keyutils=1.5.9-8ubuntu1`

Binary Packages:

- `libkeyutils1:amd64=1.5.9-8ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.5.9-8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-8ubuntu1.dsc' keyutils_1.5.9-8ubuntu1.dsc 1548 SHA256:dd06e9b6a773ed745cd74dbce13d585469aa508f2afbc6fa51a58939b295ce07
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9.orig.tar.bz2' keyutils_1.5.9.orig.tar.bz2 74683 SHA256:4da2c5552c688b65ab14d4fd40fbdf720c8b396d8ece643e040cf6e707e083ae
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.5.9-8ubuntu1.debian.tar.xz' keyutils_1.5.9-8ubuntu1.debian.tar.xz 16716 SHA256:36f69846dfeb1e7abdd39dace57a43f9637e426cf4c5252dd9990af36488249b
```

### `dpkg` source package: `kmod=22-1ubuntu5.2`

Binary Packages:

- `libkmod2:amd64=22-1ubuntu5.2`

Licenses: (parsed from: `/usr/share/doc/libkmod2/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris kmod=22-1ubuntu5.2
'http://archive.ubuntu.com/ubuntu/pool/main/k/kmod/kmod_22-1ubuntu5.2.dsc' kmod_22-1ubuntu5.2.dsc 2165 SHA256:b7e21eda8b57d7bba700afcc9c0cf0f2ea5e3a484e87b6b91b521cd2409b3964
'http://archive.ubuntu.com/ubuntu/pool/main/k/kmod/kmod_22.orig.tar.xz' kmod_22.orig.tar.xz 160576 SHA256:158cbbca15c570eb2f4ce29a64cae785cb377a200cf62d6f70ca52e3d33325f3
'http://archive.ubuntu.com/ubuntu/pool/main/k/kmod/kmod_22-1ubuntu5.2.debian.tar.xz' kmod_22-1ubuntu5.2.debian.tar.xz 14524 SHA256:f8dd1134e6cff72a458e66d2e86ef413be07a29cc66c87d02544bb5c2037bfb7
```

### `dpkg` source package: `krb5=1.13.2+dfsg-5ubuntu2.1`

Binary Packages:

- `krb5-multidev=1.13.2+dfsg-5ubuntu2.1`
- `libgssapi-krb5-2:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libgssrpc4:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libk5crypto3:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkadm5clnt-mit9:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkadm5srv-mit9:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkdb5-8:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkrb5-3:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkrb5-dev=1.13.2+dfsg-5ubuntu2.1`
- `libkrb5support0:amd64=1.13.2+dfsg-5ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/krb5-multidev/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libgssrpc4/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkadm5clnt-mit9/copyright`, `/usr/share/doc/libkadm5srv-mit9/copyright`, `/usr/share/doc/libkdb5-8/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5-dev/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.13.2+dfsg-5ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg-5ubuntu2.1.dsc' krb5_1.13.2+dfsg-5ubuntu2.1.dsc 3520 SHA256:d32e3a18bd00e7446c67d28c4c70bb96ec80da9b0e9215d4d8531100e1f91952
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg.orig.tar.gz' krb5_1.13.2+dfsg.orig.tar.gz 11884064 SHA256:a7af3953e4ab52b17f80bdfc2fc7471b66b512b128520796e2b993554543873a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg-5ubuntu2.1.debian.tar.xz' krb5_1.13.2+dfsg-5ubuntu2.1.debian.tar.xz 113600 SHA256:2536a14f7a186c9076d8fb8053be04842300ab000046b4d53c8fa8c9959f1efd
```

### `dpkg` source package: `lcms2=2.6-3ubuntu2.1`

Binary Packages:

- `liblcms2-2:amd64=2.6-3ubuntu2.1`
- `liblcms2-dev:amd64=2.6-3ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`, `/usr/share/doc/liblcms2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris lcms2=2.6-3ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.6-3ubuntu2.1.dsc' lcms2_2.6-3ubuntu2.1.dsc 2203 SHA256:2f6dbceb336dbba9a95c87df41175cfa44d045c82edc731fd7406936c0a97bd0
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.6.orig.tar.gz' lcms2_2.6.orig.tar.gz 4583389 SHA256:5172528839647c54c3da211837225e221be93e4733f5b5e9f57668f7107e14b1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lcms2/lcms2_2.6-3ubuntu2.1.debian.tar.xz' lcms2_2.6-3ubuntu2.1.debian.tar.xz 2417988 SHA256:74d3f20d1e8937bee6db0a5496a7a7e434ed2c6af6850483f70f9a3ef8515a2b
```

### `dpkg` source package: `libbsd=0.8.2-1ubuntu0.1`

Binary Packages:

- `libbsd0:amd64=0.8.2-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
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
$ apt-get source -qq --print-uris libbsd=0.8.2-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2-1ubuntu0.1.dsc' libbsd_0.8.2-1ubuntu0.1.dsc 2083 SHA256:6013acffdab3de3fe2422c2fc14fe0eb1d99dd8c36ea6fba5e739de192334cdb
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2.orig.tar.xz' libbsd_0.8.2.orig.tar.xz 344292 SHA256:b2f644cae94a6e2fe109449c20ad79a0f6ee4faec2205b07eefa0020565e250a
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2-1ubuntu0.1.debian.tar.xz' libbsd_0.8.2-1ubuntu0.1.debian.tar.xz 15652 SHA256:6477748f804e4fba6f2c050da5a47e6c93553f5da16d2e4a7af06c89829b107e
```

### `dpkg` source package: `libcap2=1:2.24-12`

Binary Packages:

- `libcap2:amd64=1:2.24-12`
- `libcap2-bin=1:2.24-12`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`, `/usr/share/doc/libcap2-bin/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.24-12
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.24-12.dsc' libcap2_2.24-12.dsc 2211 SHA256:4db68746bd1fe7df6d29ae15c3605e4e1d0e44723580c05166144735c773ae14
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.24.orig.tar.xz' libcap2_2.24.orig.tar.xz 63264 SHA256:51cd1c568a2baf1e687573bd6117a94b07f33b46a05acaa50ee208792a830b79
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap2/libcap2_2.24-12.debian.tar.xz' libcap2_2.24-12.debian.tar.xz 18704 SHA256:34be2e791ec96095cc0b405e532874e8c79aeb2125981ebc6896a0ad0b999cf2
```

### `dpkg` source package: `libcroco=0.6.11-1`

Binary Packages:

- `libcroco3:amd64=0.6.11-1`

Licenses: (parsed from: `/usr/share/doc/libcroco3/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcroco=0.6.11-1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.11-1.dsc' libcroco_0.6.11-1.dsc 2256 SHA256:5b614275709f3aeb92b4f4049f792b43035c304b300637d97b8205b9d3da39a6
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.11.orig.tar.xz' libcroco_0.6.11.orig.tar.xz 477312 SHA256:132b528a948586b0dfa05d7e9e059901bca5a3be675b6071a90a90b81ae5a056
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcroco/libcroco_0.6.11-1.debian.tar.xz' libcroco_0.6.11-1.debian.tar.xz 6624 SHA256:55bc5a89e557c2615e1d3c46697c9ef564328f356a1f312523bd7aea966911a3
```

### `dpkg` source package: `libdatrie=0.2.10-2`

Binary Packages:

- `libdatrie1:amd64=0.2.10-2`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.10-2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-2.dsc' libdatrie_0.2.10-2.dsc 2216 SHA256:28028afb148bbe42e31a32c9c28ebc19bd0448694fe136e9180bd162345f95c2
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10.orig.tar.xz' libdatrie_0.2.10.orig.tar.xz 294380 SHA256:180eff7b0309ca19a02d5864e744185d715f021398a096fec6cf960f8ebfaa2b
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdatrie/libdatrie_0.2.10-2.debian.tar.xz' libdatrie_0.2.10-2.debian.tar.xz 7132 SHA256:9f4b854767fa683853c74f5fb7b477694b9d7b3279315dd56fd6c51aa9a43ff0
```

### `dpkg` source package: `libedit=3.1-20150325-1ubuntu2`

Binary Packages:

- `libedit2:amd64=3.1-20150325-1ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20150325-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20150325-1ubuntu2.dsc' libedit_3.1-20150325-1ubuntu2.dsc 2342 SHA256:58a27a139b3b1e216a9b9d95fc8f0a0e0bccb244b016b382e6957d0e5a8cdb04
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20150325.orig.tar.gz' libedit_3.1-20150325.orig.tar.gz 502792 SHA256:c88a5e4af83c5f40dda8455886ac98923a9c33125699742603a88a0253fcc8c5
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20150325-1ubuntu2.debian.tar.bz2' libedit_3.1-20150325-1ubuntu2.debian.tar.bz2 10946 SHA256:97d03ee621a5ec98b2683052b57c151462ec690a8e94e7d52bae76c79975f8b3
```

### `dpkg` source package: `liberror-perl=0.17-1.2`

Binary Packages:

- `liberror-perl=0.17-1.2`

Licenses: (parsed from: `/usr/share/doc/liberror-perl/copyright`)

- `Artistic`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris liberror-perl=0.17-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17-1.2.dsc' liberror-perl_0.17-1.2.dsc 1825 SHA256:d024e770bb970061e338798934a1862b5dd51ca99f04f6cdab1c5a58b30b4eba
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17.orig.tar.gz' liberror-perl_0.17.orig.tar.gz 17266 SHA256:2e8157981a77e87d37d26d8b6b3183560dddc541b491b0b32fcda010730b257c
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17-1.2.diff.gz' liberror-perl_0.17-1.2.diff.gz 3645 SHA256:26664db91daa76fdf78be37196df02067b2283deae1b4ac766923d7ef08c3fb8
```

### `dpkg` source package: `libevent=2.0.21-stable-2ubuntu0.16.04.1`

Binary Packages:

- `libevent-2.0-5:amd64=2.0.21-stable-2ubuntu0.16.04.1`
- `libevent-core-2.0-5:amd64=2.0.21-stable-2ubuntu0.16.04.1`
- `libevent-dev=2.0.21-stable-2ubuntu0.16.04.1`
- `libevent-extra-2.0-5:amd64=2.0.21-stable-2ubuntu0.16.04.1`
- `libevent-openssl-2.0-5:amd64=2.0.21-stable-2ubuntu0.16.04.1`
- `libevent-pthreads-2.0-5:amd64=2.0.21-stable-2ubuntu0.16.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libevent=2.0.21-stable-2ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.0.21-stable-2ubuntu0.16.04.1.dsc' libevent_2.0.21-stable-2ubuntu0.16.04.1.dsc 2531 SHA256:94da0c60ca7cc3985992ea43610e00f3e416b96b508965ff3f6a44d8a2cbf6d2
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.0.21-stable.orig.tar.gz' libevent_2.0.21-stable.orig.tar.gz 850772 SHA256:22a530a8a5ba1cb9c080cba033206b17dacd21437762155c6d30ee6469f574f5
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.0.21-stable-2ubuntu0.16.04.1.debian.tar.xz' libevent_2.0.21-stable-2ubuntu0.16.04.1.debian.tar.xz 14084 SHA256:4f90ca8f0762b7981c16c966391447c2dcda0295b4e2939213c74cb403baf3ec
```

### `dpkg` source package: `libexif=0.6.21-2ubuntu0.5`

Binary Packages:

- `libexif-dev=0.6.21-2ubuntu0.5`
- `libexif12:amd64=0.6.21-2ubuntu0.5`

Licenses: (parsed from: `/usr/share/doc/libexif-dev/copyright`, `/usr/share/doc/libexif12/copyright`)

- `BSD-2-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libexif=0.6.21-2ubuntu0.5
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21-2ubuntu0.5.dsc' libexif_0.6.21-2ubuntu0.5.dsc 2185 SHA256:26984f3d41b4205394283b42094d8b9262d629466a1d7a7da170c483b609f54b
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21.orig.tar.gz' libexif_0.6.21.orig.tar.gz 2081615 SHA256:edb7eb13664cf950a6edd132b75e99afe61c5effe2f16494e6d27bc404b287bf
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libexif/libexif_0.6.21-2ubuntu0.5.debian.tar.xz' libexif_0.6.21-2ubuntu0.5.debian.tar.xz 16932 SHA256:bba1ddc751bdad47c0a3412849f1793a04f037d1462582b4af5a37c11e8a69f3
```

### `dpkg` source package: `libffi=3.2.1-4`

Binary Packages:

- `libffi-dev:amd64=3.2.1-4`
- `libffi6:amd64=3.2.1-4`

Licenses: (parsed from: `/usr/share/doc/libffi-dev/copyright`, `/usr/share/doc/libffi6/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.2.1-4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-4.dsc' libffi_3.2.1-4.dsc 1914 SHA256:e2bdb4202f1c8be9d3cec5bf459a4a1619f494241938d982d6029e15a8b1da9e
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1.orig.tar.gz' libffi_3.2.1.orig.tar.gz 940837 SHA256:d06ebb8e1d9a22d19e38d63fdb83954253f39bedc5d46232a05645685722ca37
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.2.1-4.debian.tar.xz' libffi_3.2.1-4.debian.tar.xz 8932 SHA256:4d7d5f9172e8a8d3e412ed47e14755e27a0657054a7786b578eb6327b0d08b2d
```

### `dpkg` source package: `libgcrypt20=1.6.5-2ubuntu0.6`

Binary Packages:

- `libgcrypt20:amd64=1.6.5-2ubuntu0.6`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.6.5-2ubuntu0.6
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.6.5-2ubuntu0.6.dsc' libgcrypt20_1.6.5-2ubuntu0.6.dsc 2653 SHA256:9a49e72112a7a42d54960a8f170117970d5751ecad0ccdb186dfea360fdd3fe4
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.6.5.orig.tar.bz2' libgcrypt20_1.6.5.orig.tar.bz2 2549601 SHA256:f49ebc5842d455ae7019def33eb5a014a0f07a2a8353dc3aa50a76fd1dafa924
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.6.5-2ubuntu0.6.debian.tar.xz' libgcrypt20_1.6.5-2ubuntu0.6.debian.tar.xz 38412 SHA256:1024930d785a1d5a4345821e923cde1fe20bdfd1aa3a46689374e9822472df9d
```

### `dpkg` source package: `libgd2=2.1.1-4ubuntu0.16.04.12`

Binary Packages:

- `libgd3:amd64=2.1.1-4ubuntu0.16.04.12`

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
$ apt-get source -qq --print-uris libgd2=2.1.1-4ubuntu0.16.04.12
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgd2/libgd2_2.1.1-4ubuntu0.16.04.12.dsc' libgd2_2.1.1-4ubuntu0.16.04.12.dsc 2178 SHA256:5947479fb8f24bf86e945f5cb22178b62764c4020cdef704cac3cd9f7926a7ed
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgd2/libgd2_2.1.1.orig.tar.gz' libgd2_2.1.1.orig.tar.gz 2033791 SHA256:a68c69d2fe3eaab9db63b1c4d391dd549c26d3b47bfba484d5ed2d433c55d4d8
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgd2/libgd2_2.1.1-4ubuntu0.16.04.12.debian.tar.xz' libgd2_2.1.1-4ubuntu0.16.04.12.debian.tar.xz 62544 SHA256:c806b49a86a5477b8591c496b4aa3f820bb16a3b3cea9dea24ec351b25cc5fdd
```

### `dpkg` source package: `libgpg-error=1.21-2ubuntu1`

Binary Packages:

- `libgpg-error0:amd64=1.21-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `GPL-2.1+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.21-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.21-2ubuntu1.dsc' libgpg-error_1.21-2ubuntu1.dsc 2306 SHA256:591fc35e29c7314e9dcbea0ed929afc563dd5e0a6be18d65d2480762353bd71f
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.21.orig.tar.bz2' libgpg-error_1.21.orig.tar.bz2 763186 SHA256:b7dbdb3cad63a740e9f0c632a1da32d4afdb694ec86c8625c98ea0691713b84d
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.21-2ubuntu1.debian.tar.xz' libgpg-error_1.21-2ubuntu1.debian.tar.xz 11988 SHA256:b67f4686d39ec678e860b28d05e07567ec6d43025c18b82c1e9a5dda07a00ed9
```

### `dpkg` source package: `libice=2:1.0.9-1`

Binary Packages:

- `libice-dev:amd64=2:1.0.9-1`
- `libice6:amd64=2:1.0.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-1.dsc' libice_1.0.9-1.dsc 2140 SHA256:f90a79944f147b5db208677d92381fd0886c201616172bac0b28ef0e85912ebd
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9.orig.tar.gz' libice_1.0.9.orig.tar.gz 455871 SHA256:7812a824a66dd654c830d21982749b3b563d9c2dfe0b88b203cefc14a891edc0
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libice/libice_1.0.9-1.diff.gz' libice_1.0.9-1.diff.gz 6260 SHA256:85d68a69d5e6b25b352eb98c6c33fa7a324da8dd913d7e84a049852fb87287e7
```

### `dpkg` source package: `libidn=1.32-3ubuntu1.2`

Binary Packages:

- `libidn11:amd64=1.32-3ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libidn11/copyright`)

- `GAP`
- `GFDL-1.3`
- `GFDL-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libidn=1.32-3ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.32-3ubuntu1.2.dsc' libidn_1.32-3ubuntu1.2.dsc 2303 SHA256:7e8ac6585e9ab5e0fce89ff91ff1972709da56551814973b84ef36e6c84072e4
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.32.orig.tar.gz' libidn_1.32.orig.tar.gz 3483155 SHA256:ba5d5afee2beff703a34ee094668da5c6ea5afa38784cebba8924105e185c4f5
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn/libidn_1.32-3ubuntu1.2.debian.tar.xz' libidn_1.32-3ubuntu1.2.debian.tar.xz 84724 SHA256:f898167a432eeb656fe372b0565af7ab26f8eeaf269cfd768d34fa97fcaa3a4c
```

### `dpkg` source package: `libjpeg-turbo=1.4.2-0ubuntu3.4`

Binary Packages:

- `libjpeg-turbo8:amd64=1.4.2-0ubuntu3.4`
- `libjpeg-turbo8-dev:amd64=1.4.2-0ubuntu3.4`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`, `/usr/share/doc/libjpeg-turbo8-dev/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1.4.2-0ubuntu3.4
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2-0ubuntu3.4.dsc' libjpeg-turbo_1.4.2-0ubuntu3.4.dsc 2302 SHA256:0080b735775bfdc8927856da35ec52dc870d787b0d6864ad1875aa2a1c15d69d
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2.orig.tar.gz' libjpeg-turbo_1.4.2.orig.tar.gz 1569306 SHA256:521bb5d3043e7ac063ce3026d9a59cc2ab2e9636c655a2515af5f4706122233e
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2-0ubuntu3.4.debian.tar.xz' libjpeg-turbo_1.4.2-0ubuntu3.4.debian.tar.xz 30156 SHA256:f3e6a20cb3accb33cfdfed128ebc09e21416952472601a759bc4fd37bba482d7
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

### `dpkg` source package: `liblqr=0.4.2-2`

Binary Packages:

- `liblqr-1-0:amd64=0.4.2-2`
- `liblqr-1-0-dev=0.4.2-2`

Licenses: (parsed from: `/usr/share/doc/liblqr-1-0/copyright`, `/usr/share/doc/liblqr-1-0-dev/copyright`)

- `GPL-3`
- `GPLv3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris liblqr=0.4.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.dsc' liblqr_0.4.2-2.dsc 2024 SHA256:7e203605ebe40cde3e467db4298d7ee3f83f3d3082b05f8984868cdef1606245
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2.orig.tar.gz' liblqr_0.4.2.orig.tar.gz 439884 SHA256:d4c22373432cca749e4326cd41fce365e6ff857c0bfd7a5302b8eb34b69f0336
'http://archive.ubuntu.com/ubuntu/pool/main/libl/liblqr/liblqr_0.4.2-2.debian.tar.xz' liblqr_0.4.2-2.debian.tar.xz 5860 SHA256:2c886ee88f65eade9e1cd10965bf572a3cc178d6119b9342c8469b6b41d2bb62
```

### `dpkg` source package: `libmaxminddb=1.0.4-2.1`

Binary Packages:

- `libmaxminddb-dev:amd64=1.0.4-2.1`
- `libmaxminddb0:amd64=1.0.4-2.1`

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
$ apt-get source -qq --print-uris libmaxminddb=1.0.4-2.1
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.0.4-2.1.dsc' libmaxminddb_1.0.4-2.1.dsc 1918 SHA256:8deb3af3f4b76c6814a014360ce3e10d230ca95f312e4db70b09d3f0320d9973
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.0.4.orig.tar.gz' libmaxminddb_1.0.4.orig.tar.gz 119936 SHA256:e43949128235065e00047941408d911b2d6a3847b7f2c2598b5d81fdce0a11c2
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmaxminddb/libmaxminddb_1.0.4-2.1.debian.tar.xz' libmaxminddb_1.0.4-2.1.debian.tar.xz 4480 SHA256:99efb570462042fbff2719420afdfaf3a521515d0e304052131d815672f310f7
```

### `dpkg` source package: `libpng=1.2.54-1ubuntu1.1`

Binary Packages:

- `libpng12-0:amd64=1.2.54-1ubuntu1.1`
- `libpng12-dev:amd64=1.2.54-1ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libpng12-0/copyright`, `/usr/share/doc/libpng12-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libpng=1.2.54-1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng/libpng_1.2.54-1ubuntu1.1.dsc' libpng_1.2.54-1ubuntu1.1.dsc 2121 SHA256:f38f2e0fdbdcbf20a569e02f9b3365638e88d084ae677ae164966f4f063c2c08
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng/libpng_1.2.54.orig.tar.xz' libpng_1.2.54.orig.tar.xz 571448 SHA256:cf85516482780f2bc2c5b5073902f12b1519019d47bf473326c2018bdff1d272
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpng/libpng_1.2.54-1ubuntu1.1.debian.tar.xz' libpng_1.2.54-1ubuntu1.1.debian.tar.xz 18820 SHA256:2c3fa2d8bb8df50a89680fecc288b95e9f1c4bf809797f7e85e90c22031a1a2e
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

### `dpkg` source package: `librsvg=2.40.13-3`

Binary Packages:

- `gir1.2-rsvg-2.0:amd64=2.40.13-3`
- `librsvg2-2:amd64=2.40.13-3`
- `librsvg2-common:amd64=2.40.13-3`
- `librsvg2-dev:amd64=2.40.13-3`

Licenses: (parsed from: `/usr/share/doc/gir1.2-rsvg-2.0/copyright`, `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`, `/usr/share/doc/librsvg2-dev/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris librsvg=2.40.13-3
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.13-3.dsc' librsvg_2.40.13-3.dsc 2753 SHA256:af4272681ef53d16c75d6f70ba40de82cae258b3c1bffbf9ea5707393165bac5
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.13.orig.tar.xz' librsvg_2.40.13.orig.tar.xz 552900 SHA256:4d6ea93ec05f5dabe7262d711d246a0a99b2311e215360dd3dcabd6afe3b9804
'http://archive.ubuntu.com/ubuntu/pool/main/libr/librsvg/librsvg_2.40.13-3.debian.tar.xz' librsvg_2.40.13-3.debian.tar.xz 17120 SHA256:3897c82eed5d2857a62cdf442f599c94e3c2bd89f16d26bd4c43c3d8b3c271eb
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3.16.04.2`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3.16.04.2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2`
- `LGPL-2.0+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `libselinux=2.4-3build2`

Binary Packages:

- `libselinux1:amd64=2.4-3build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=2.4-3build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.4-3build2.dsc' libselinux_2.4-3build2.dsc 2491 SHA256:c14dbd5eff5dfd66c41b9ed3d09e1186975b233c8a2a59720ccb8b318c85883c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.4.orig.tar.gz' libselinux_2.4.orig.tar.gz 165931 SHA256:46043091f4c5ba4f43e8d3715f30d665a2d571c9126c1f03945c9ea4ed380f7b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_2.4-3build2.debian.tar.xz' libselinux_2.4-3build2.debian.tar.xz 23216 SHA256:96f1c0526970460e6b5f64ea4d2f7ecabe06e80e23e83e4feccecb955e1ca956
```

### `dpkg` source package: `libsemanage=2.3-1build3`

Binary Packages:

- `libsemanage-common=2.3-1build3`
- `libsemanage1:amd64=2.3-1build3`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=2.3-1build3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.3-1build3.dsc' libsemanage_2.3-1build3.dsc 2497 SHA256:920f1f389316617711778cbe83eb36f62d59a2ebb3b1488f75c41014c0bc684c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.3.orig.tar.gz' libsemanage_2.3.orig.tar.gz 138231 SHA256:03e09e35e611c286e446bef92b6023ef2623815996f5a53394bb02e49a312e4b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_2.3-1build3.debian.tar.xz' libsemanage_2.3-1build3.debian.tar.xz 15056 SHA256:d4f90c66ba911f72c5195da957cdcacd91a583e64ad06c01bf5b692387ee3d33
```

### `dpkg` source package: `libsepol=2.4-2`

Binary Packages:

- `libsepol1:amd64=2.4-2`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=2.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.4-2.dsc' libsepol_2.4-2.dsc 1768 SHA256:fca86fc62f736baf96ac2061327553b74b1b34f7ace89d982baa5374c24e2841
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.4.orig.tar.gz' libsepol_2.4.orig.tar.gz 570822 SHA256:299015d59932404c6b69d365fdecffe5c0e2f9c44e08b47286a4bfc02ee49659
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_2.4-2.debian.tar.xz' libsepol_2.4-2.debian.tar.xz 13188 SHA256:85e50e42c49dee9b21b5dda5fb754ce6d10482a4641e9f088da103b9178c2c1d
```

### `dpkg` source package: `libsigsegv=2.10-4`

Binary Packages:

- `libsigsegv2:amd64=2.10-4`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.10-4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.10-4.dsc' libsigsegv_2.10-4.dsc 2166 SHA256:54837482677ed4d42203c80bb10ba0308431a00cb8ccca3256cce8a3bdfa8d8e
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.10.orig.tar.gz' libsigsegv_2.10.orig.tar.gz 402279 SHA256:8460a4a3dd4954c3d96d7a4f5dd5bc4d9b76f5754196aa245287553b26d2199a
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.10-4.debian.tar.xz' libsigsegv_2.10-4.debian.tar.xz 9532 SHA256:abc74f39b89e7dc5ee46cf4e9cf9e6b9dcc00122ffe87e49036647c5e9a10d36
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

### `dpkg` source package: `libtasn1-6=4.7-3ubuntu0.16.04.3`

Binary Packages:

- `libtasn1-6:amd64=4.7-3ubuntu0.16.04.3`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.7-3ubuntu0.16.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.7-3ubuntu0.16.04.3.dsc' libtasn1-6_4.7-3ubuntu0.16.04.3.dsc 2495 SHA256:53a43e4795381eca289ba755fc806822373f31f2bbc6f12ae7f6d32c2e7c710a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.7.orig.tar.gz' libtasn1-6_4.7.orig.tar.gz 1851611 SHA256:a40780dc93fc6d819170240e8ece25352058a85fd1d2347ce0f143667d8f11c9
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.7-3ubuntu0.16.04.3.debian.tar.xz' libtasn1-6_4.7-3ubuntu0.16.04.3.debian.tar.xz 60468 SHA256:aeed7264d288f57c858fb247f94920c1157a840c03fd27c7eaa3d6a6e36a66d7
```

### `dpkg` source package: `libthai=0.1.24-2`

Binary Packages:

- `libthai-data=0.1.24-2`
- `libthai0:amd64=0.1.24-2`

Licenses: (parsed from: `/usr/share/doc/libthai-data/copyright`, `/usr/share/doc/libthai0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libthai=0.1.24-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.24-2.dsc' libthai_0.1.24-2.dsc 2341 SHA256:4e760ef914d56d7a83fbbbf2ff25446e7669335e5404d2accf89445b81874c9c
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.24.orig.tar.xz' libthai_0.1.24.orig.tar.xz 394672 SHA256:a2dd95f79084a27ac077cc206e66e30ee193b70738676ed39792acc9a1c2af0d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libthai/libthai_0.1.24-2.debian.tar.xz' libthai_0.1.24-2.debian.tar.xz 10780 SHA256:94ff719ca7679150ceab23ee45c3eeeb7c13196fbc206310e150bd32574eeebd
```

### `dpkg` source package: `libtool=2.4.6-0.1`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-0.1`
- `libltdl7:amd64=2.4.6-0.1`
- `libtool=2.4.6-0.1`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`, `/usr/share/doc/libtool/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-0.1.dsc' libtool_2.4.6-0.1.dsc 2080 SHA256:c0ec24bc1e892564840061e64cf288e018484d733208d97815f3b12f043088b6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-0.1.debian.tar.xz' libtool_2.4.6-0.1.debian.tar.xz 19332 SHA256:1b9d3e0f9d177d259206cdda69d6cec8dd04df14cbb064b71869936ca5f2722f
```

### `dpkg` source package: `libusb=2:0.1.12-28`

Binary Packages:

- `libusb-0.1-4:amd64=2:0.1.12-28`

Licenses: (parsed from: `/usr/share/doc/libusb-0.1-4/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libusb=2:0.1.12-28
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb/libusb_0.1.12-28.dsc' libusb_0.1.12-28.dsc 2012 SHA256:be0a89935a8764dc64d40a28959397e6582261eef2152c4ce90a13490471dc5f
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb/libusb_0.1.12.orig.tar.gz' libusb_0.1.12.orig.tar.gz 389343 SHA256:37f6f7d9de74196eb5fc0bbe0aea9b5c939de7f500acba3af6fd643f3b538b44
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb/libusb_0.1.12-28.debian.tar.xz' libusb_0.1.12-28.debian.tar.xz 21524 SHA256:eaf2314902b0bb9de3e1fa8c9abfcecea7b78c9824048016beaca34f7cc4351b
```

### `dpkg` source package: `libvpx=1.5.0-2ubuntu1.1`

Binary Packages:

- `libvpx3:amd64=1.5.0-2ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libvpx3/copyright`)

- `Artistic`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libvpx=1.5.0-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvpx/libvpx_1.5.0-2ubuntu1.1.dsc' libvpx_1.5.0-2ubuntu1.1.dsc 2127 SHA256:4bdbcd90cd8d09cf96f1ecf2295526510d24ab3bbd5915a12e7500f0ac437179
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvpx/libvpx_1.5.0.orig.tar.bz2' libvpx_1.5.0.orig.tar.bz2 1906571 SHA256:306d67908625675f8e188d37a81fbfafdf5068b09d9aa52702b6fbe601c76797
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvpx/libvpx_1.5.0-2ubuntu1.1.debian.tar.xz' libvpx_1.5.0-2ubuntu1.1.debian.tar.xz 17492 SHA256:b7a61dfb8e9c26a93c9ab55eca39dc98111e0c5c3470e25343bcb5cff0087e80
```

### `dpkg` source package: `libwebp=0.4.4-1`

Binary Packages:

- `libwebp-dev:amd64=0.4.4-1`
- `libwebp5:amd64=0.4.4-1`
- `libwebpdemux1:amd64=0.4.4-1`
- `libwebpmux1:amd64=0.4.4-1`

Licenses: (parsed from: `/usr/share/doc/libwebp-dev/copyright`, `/usr/share/doc/libwebp5/copyright`, `/usr/share/doc/libwebpdemux1/copyright`, `/usr/share/doc/libwebpmux1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=0.4.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.4.4-1.dsc' libwebp_0.4.4-1.dsc 2077 SHA256:278509d0b7ec8507d8f23ec520b9eabd719727a1454d032c62d41641487a175b
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.4.4.orig.tar.gz' libwebp_0.4.4.orig.tar.gz 992491 SHA256:c65d34edb57338e331ba4d622227a2b3179444cfca17d02c34f1ead63f603e86
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwebp/libwebp_0.4.4-1.debian.tar.xz' libwebp_0.4.4-1.debian.tar.xz 6800 SHA256:edc5175cf73d87dfba9e1b7f35d54fd361a9866ab1682e6ca60229b501f17df5
```

### `dpkg` source package: `libwmf=0.2.8.4-10.5ubuntu1`

Binary Packages:

- `libwmf-dev=0.2.8.4-10.5ubuntu1`
- `libwmf0.2-7:amd64=0.2.8.4-10.5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libwmf-dev/copyright`, `/usr/share/doc/libwmf0.2-7/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris libwmf=0.2.8.4-10.5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-10.5ubuntu1.dsc' libwmf_0.2.8.4-10.5ubuntu1.dsc 2232 SHA256:45ea2302830d57b4a0a8c59dc25765572e232cc60d65e9229f1185f2f3c4001d
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4.orig.tar.gz' libwmf_0.2.8.4.orig.tar.gz 2169375 SHA256:5b345c69220545d003ad52bfd035d5d6f4f075e65204114a9e875e84895a7cf8
'http://archive.ubuntu.com/ubuntu/pool/main/libw/libwmf/libwmf_0.2.8.4-10.5ubuntu1.debian.tar.xz' libwmf_0.2.8.4-10.5ubuntu1.debian.tar.xz 11696 SHA256:e448f84c36c2921403cf47e19090ad17be71877c3ec62cdf4b4c8a3e8869d5ee
```

### `dpkg` source package: `libx11=2:1.6.3-1ubuntu2.1`

Binary Packages:

- `libx11-6:amd64=2:1.6.3-1ubuntu2.1`
- `libx11-data=2:1.6.3-1ubuntu2.1`
- `libx11-dev:amd64=2:1.6.3-1ubuntu2.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.3-1ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.3-1ubuntu2.1.dsc' libx11_1.6.3-1ubuntu2.1.dsc 2603 SHA256:efb03b486de6587de9572f57f42948125a8ea5ad47f6e872f2b9c17a150de103
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.3.orig.tar.gz' libx11_1.6.3.orig.tar.gz 3105928 SHA256:0b03b9d22f4c9e59b4ba498f294e297f013cae27050dfa0f3496640200db5376
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.3-1ubuntu2.1.diff.gz' libx11_1.6.3-1ubuntu2.1.diff.gz 44832 SHA256:205f80b6f3110c068f3bbf18b177102399b67634ef5c436a71d1f90b58ac753f
```

### `dpkg` source package: `libxau=1:1.0.8-1`

Binary Packages:

- `libxau-dev:amd64=1:1.0.8-1`
- `libxau6:amd64=1:1.0.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.8-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1.dsc' libxau_1.0.8-1.dsc 2040 SHA256:3ddb5f2c7a49ef7507b8d1e63e891238db877b4d1bb1c5486a3e3242c8523602
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8.orig.tar.gz' libxau_1.0.8.orig.tar.gz 362044 SHA256:c343b4ef66d66a6b3e0e27aa46b37ad5cab0f11a5c565eafb4a1c7590bc71d7b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.8-1.diff.gz' libxau_1.0.8-1.diff.gz 15287 SHA256:b493479d6a52a0e753dd357ad8a4bc5c4296015f3f7b96cf546f7c5c5843cbb0
```

### `dpkg` source package: `libxcb=1.11.1-1ubuntu1`

Binary Packages:

- `libxcb-render0:amd64=1.11.1-1ubuntu1`
- `libxcb-render0-dev:amd64=1.11.1-1ubuntu1`
- `libxcb-shm0:amd64=1.11.1-1ubuntu1`
- `libxcb-shm0-dev:amd64=1.11.1-1ubuntu1`
- `libxcb1:amd64=1.11.1-1ubuntu1`
- `libxcb1-dev:amd64=1.11.1-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.11.1-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.11.1-1ubuntu1.dsc' libxcb_1.11.1-1ubuntu1.dsc 6434 SHA256:d059cea4a732eb2600d829d023af89956b46d85399d90be122a887a6baf59a26
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.11.1.orig.tar.gz' libxcb_1.11.1.orig.tar.gz 633057 SHA256:660312d5e64d0a5800262488042c1707a0261fa01a759bad265b1b75dd4844dd
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.11.1-1ubuntu1.diff.gz' libxcb_1.11.1-1ubuntu1.diff.gz 25030 SHA256:017d57e8d555e9f003b1d1ef394b81eddecf9029b6b7e582400dd51e17d63401
```

### `dpkg` source package: `libxcomposite=1:0.4.4-1`

Binary Packages:

- `libxcomposite1:amd64=1:0.4.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcomposite=1:0.4.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.dsc' libxcomposite_0.4.4-1.dsc 2170 SHA256:b304040285ca2d6e2667bfec45097814bdd017380c629a5972993407c656469a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4.orig.tar.gz' libxcomposite_0.4.4.orig.tar.gz 354584 SHA256:83c04649819c6f52cda1b0ce8bcdcc48ad8618428ad803fb07f20b802f1bdad1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcomposite/libxcomposite_0.4.4-1.diff.gz' libxcomposite_0.4.4-1.diff.gz 15633 SHA256:09fe6dd7d98d935e7307d57f926912d477b929f06c159962840d3a398f376988
```

### `dpkg` source package: `libxcursor=1:1.1.14-1ubuntu0.16.04.2`

Binary Packages:

- `libxcursor1:amd64=1:1.1.14-1ubuntu0.16.04.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcursor=1:1.1.14-1ubuntu0.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.14-1ubuntu0.16.04.2.dsc' libxcursor_1.1.14-1ubuntu0.16.04.2.dsc 2429 SHA256:90b7527e0b0d352b5f0f21a55ff8bdceb6e3d26071cc6b8253e7409ff2d91d3a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.14.orig.tar.gz' libxcursor_1.1.14.orig.tar.gz 374910 SHA256:be0954faf274969ffa6d95b9606b9c0cfee28c13b6fc014f15606a0c8b05c17b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcursor/libxcursor_1.1.14-1ubuntu0.16.04.2.diff.gz' libxcursor_1.1.14-1ubuntu0.16.04.2.diff.gz 19882 SHA256:7d3f0f5d8c168f2580f511f4da5d4458e332c9c8a4423364a27b8b07d6b49ee1
```

### `dpkg` source package: `libxdamage=1:1.1.4-2`

Binary Packages:

- `libxdamage1:amd64=1:1.1.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdamage=1:1.1.4-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4-2.dsc' libxdamage_1.1.4-2.dsc 2127 SHA256:43cbefb5c69f51d89a11cf84718fe0c42058fc9b6ec7c0076e7c37b9e829feb5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4.orig.tar.gz' libxdamage_1.1.4.orig.tar.gz 339060 SHA256:4bb3e9d917f5f593df2277d452926ee6ad96de7b7cd1017cbcf4579fe5d3442b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdamage/libxdamage_1.1.4-2.diff.gz' libxdamage_1.1.4-2.diff.gz 14930 SHA256:d238c1a266c30cd124ede7e6c86635bfaa108fa552c4a82919101cebf22670e9
```

### `dpkg` source package: `libxdmcp=1:1.1.2-1.1`

Binary Packages:

- `libxdmcp-dev:amd64=1:1.1.2-1.1`
- `libxdmcp6:amd64=1:1.1.2-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.2-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-1.1.dsc' libxdmcp_1.1.2-1.1.dsc 2098 SHA256:605175ee859f00ace43a4c35dc2d7c60971c0e1f21769b508b5bce2303979436
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2.orig.tar.gz' libxdmcp_1.1.2.orig.tar.gz 404115 SHA256:6f7c7e491a23035a26284d247779174dedc67e34e93cc3548b648ffdb6fc57c0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.2-1.1.diff.gz' libxdmcp_1.1.2-1.1.diff.gz 17944 SHA256:d764e8d251d06c9e5a50783cee393c621b7288bc3369d158b6a1d2e4372f3c9e
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

### `dpkg` source package: `libxfixes=1:5.0.1-2`

Binary Packages:

- `libxfixes3:amd64=1:5.0.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxfixes=1:5.0.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.1-2.dsc' libxfixes_5.0.1-2.dsc 2160 SHA256:1569c87546b8d59ee7f60b395b10ea1a6f9d52418aed9d7cf2d633b14a1f1f25
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.1.orig.tar.gz' libxfixes_5.0.1.orig.tar.gz 352057 SHA256:81b692856c0e7ab2778a34a32aa6b3f455b9b58cf388f009cba872ed933ae9c0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxfixes/libxfixes_5.0.1-2.diff.gz' libxfixes_5.0.1-2.diff.gz 6564 SHA256:df62260744ac03e8354b004685d439c32588e826c9dc570b6109070447601ce0
```

### `dpkg` source package: `libxi=2:1.7.6-1`

Binary Packages:

- `libxi6:amd64=2:1.7.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxi=2:1.7.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.6-1.dsc' libxi_1.7.6-1.dsc 2269 SHA256:b0d205346b418dbfbdd36dadc164e6050bcfa5cd691f190c9aa0ac91d2a0e5e8
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.6.orig.tar.gz' libxi_1.7.6.orig.tar.gz 601628 SHA256:4e88fa7decd287e58140ea72238f8d54e4791de302938c83695fc0c9ac102b7e
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxi/libxi_1.7.6-1.diff.gz' libxi_1.7.6-1.diff.gz 10149 SHA256:ae61f11cd06263d7a4caf25835fdd8ba4e8ad319781acb1e0cd177eab82ce8a7
```

### `dpkg` source package: `libxinerama=2:1.1.3-1`

Binary Packages:

- `libxinerama1:amd64=2:1.1.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxinerama=2:1.1.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3-1.dsc' libxinerama_1.1.3-1.dsc 2198 SHA256:4cf9a3558bd7ce1b4f55a581175c05e4b4a172364458a21ff4b657b714688fbb
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3.orig.tar.gz' libxinerama_1.1.3.orig.tar.gz 350141 SHA256:0ba243222ae5aba4c6a3d7a394c32c8b69220a6872dbb00b7abae8753aca9a44
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxinerama/libxinerama_1.1.3-1.diff.gz' libxinerama_1.1.3-1.diff.gz 15738 SHA256:2b1487e3511ddabfec666a62f6e5e8ac4f97536b0d53c51f7bf4cbe07508a130
```

### `dpkg` source package: `libxml2=2.9.3+dfsg1-1ubuntu0.7`

Binary Packages:

- `libxml2:amd64=2.9.3+dfsg1-1ubuntu0.7`
- `libxml2-dev:amd64=2.9.3+dfsg1-1ubuntu0.7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.3+dfsg1-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1-1ubuntu0.7.dsc' libxml2_2.9.3+dfsg1-1ubuntu0.7.dsc 2756 SHA256:316bf37291791a4dfd649aae1a1f42215014bea0046980b8d0a793724e83a707
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1.orig.tar.xz' libxml2_2.9.3+dfsg1.orig.tar.xz 2475440 SHA256:d6b7686fa12c70dd9ce7c7d97c84471b5afed1c176538df8c670754d8c206079
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1-1ubuntu0.7.debian.tar.xz' libxml2_2.9.3+dfsg1-1ubuntu0.7.debian.tar.xz 57976 SHA256:67f1a2c05d95d6e7d2e2906c32e55d625d708e19c2bf13af074a4f7abd485487
```

### `dpkg` source package: `libxpm=1:3.5.11-1ubuntu0.16.04.1`

Binary Packages:

- `libxpm4:amd64=1:3.5.11-1ubuntu0.16.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxpm=1:3.5.11-1ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.11-1ubuntu0.16.04.1.dsc' libxpm_3.5.11-1ubuntu0.16.04.1.dsc 2251 SHA256:4782bb9304c52ae6cec76fcff72117a5c51b735327b338e26fb7402b3c6c2bde
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.11.orig.tar.gz' libxpm_3.5.11.orig.tar.gz 527020 SHA256:53ddf924441b7ed2de994d4934358c13d9abf4828b1b16e1255ade5032b31df7
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxpm/libxpm_3.5.11-1ubuntu0.16.04.1.diff.gz' libxpm_3.5.11-1ubuntu0.16.04.1.diff.gz 16815 SHA256:71ee198fe5c394998adebf1f5b89f356729820c400d96382ce4aa4798cb5cb4e
```

### `dpkg` source package: `libxrandr=2:1.5.0-1`

Binary Packages:

- `libxrandr2:amd64=2:1.5.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrandr=2:1.5.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.0-1.dsc' libxrandr_1.5.0-1.dsc 2125 SHA256:e1fe17d69676e15108ff6c6c3eedc2c3c72fef8a9dd9bde1ac9f4f4467efdfd1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.0.orig.tar.gz' libxrandr_1.5.0.orig.tar.gz 382147 SHA256:1b594a149e6b124aab7149446f2fd886461e2935eca8dca43fe83a70cf8ec451
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrandr/libxrandr_1.5.0-1.diff.gz' libxrandr_1.5.0-1.diff.gz 13507 SHA256:f04e5dccdee7db84d534aa4423b927710fbffe513c0ec632f92129a70323334e
```

### `dpkg` source package: `libxrender=1:0.9.9-0ubuntu1`

Binary Packages:

- `libxrender-dev:amd64=1:0.9.9-0ubuntu1`
- `libxrender1:amd64=1:0.9.9-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.9-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.9-0ubuntu1.dsc' libxrender_0.9.9-0ubuntu1.dsc 1562 SHA256:3b9304baa99c34df694a673aeffc1e44d7564f1e0efa71ac542435afcfd0f334
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.9.orig.tar.gz' libxrender_0.9.9.orig.tar.gz 371568 SHA256:beeac64ff8d225f775019eb7c688782dee9f4cc7b412a65538f8dde7be4e90fe
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxrender/libxrender_0.9.9-0ubuntu1.diff.gz' libxrender_0.9.9-0ubuntu1.diff.gz 18873 SHA256:b02577c21b37a46cd0b554ab25ad4bfd49545e02774b4ab2b80c2deae93abd91
```

### `dpkg` source package: `libxslt=1.1.28-2.1ubuntu0.3`

Binary Packages:

- `libxslt1-dev:amd64=1.1.28-2.1ubuntu0.3`
- `libxslt1.1:amd64=1.1.28-2.1ubuntu0.3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxslt=1.1.28-2.1ubuntu0.3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.28-2.1ubuntu0.3.dsc' libxslt_1.1.28-2.1ubuntu0.3.dsc 2482 SHA256:430bdf4c9147f094d327d0778d7288ae4097af224343263f5b19f14919f0e071
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.28.orig.tar.gz' libxslt_1.1.28.orig.tar.gz 3435907 SHA256:5fc7151a57b89c03d7b825df5a0fae0a8d5f05674c0e7cf2937ecec4d54a028c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxslt/libxslt_1.1.28-2.1ubuntu0.3.debian.tar.xz' libxslt_1.1.28-2.1ubuntu0.3.debian.tar.xz 42428 SHA256:d51924988291e776f2d31e532d060dbf47464f494602757f0d23e8baad6e7a29
```

### `dpkg` source package: `libxt=1:1.1.5-0ubuntu1`

Binary Packages:

- `libxt-dev:amd64=1:1.1.5-0ubuntu1`
- `libxt6:amd64=1:1.1.5-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.1.5-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5-0ubuntu1.dsc' libxt_1.1.5-0ubuntu1.dsc 1535 SHA256:26ea43fe0b9ed6612a2303b5fb0f84642ba9540a4a1bd18ccd84f17d17ac7e30
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5.orig.tar.gz' libxt_1.1.5.orig.tar.gz 962169 SHA256:b59bee38a9935565fa49dc1bfe84cb30173e2e07e1dcdf801430d4b54eb0caa3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxt/libxt_1.1.5-0ubuntu1.diff.gz' libxt_1.1.5-0ubuntu1.diff.gz 11392 SHA256:e4945799551b88b8a8e62487384adc04a4c9cc7e1af8fa156d55582f6315874a
```

### `dpkg` source package: `libyaml=0.1.6-3`

Binary Packages:

- `libyaml-0-2:amd64=0.1.6-3`
- `libyaml-dev:amd64=0.1.6-3`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`, `/usr/share/doc/libyaml-dev/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.1.6-3
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.6-3.dsc' libyaml_0.1.6-3.dsc 1893 SHA256:ed5bc299d3bcc0b038206f8780639d4682e65f521dff571b9336e2f8626d0011
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.6.orig.tar.gz' libyaml_0.1.6.orig.tar.gz 503012 SHA256:7da6971b4bd08a986dd2a61353bc422362bd0edcc67d7ebaac68c95f74182749
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.1.6-3.debian.tar.xz' libyaml_0.1.6-3.debian.tar.xz 4268 SHA256:fd567e6918903833e5c4f1f87254c550eca07c2bba1ccbe6031da33243cf4297
```

### `dpkg` source package: `linux=4.4.0-186.216`

Binary Packages:

- `linux-libc-dev:amd64=4.4.0-186.216`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`
- `redpine-signals`

Source:

```console
$ apt-get source -qq --print-uris linux=4.4.0-186.216
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_4.4.0-186.216.dsc' linux_4.4.0-186.216.dsc 11909 SHA256:be89e56f62386e9c7461b2ddab85e5f456214d9198012bc1ab814a3638aae8c5
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_4.4.0.orig.tar.gz' linux_4.4.0.orig.tar.gz 132860730 SHA256:730e75919b5d30a9bc934ccb300eaedfdf44994ca9ee1d07a46901c46c221357
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_4.4.0-186.216.diff.gz' linux_4.4.0-186.216.diff.gz 16629023 SHA256:d9355d89b9c9ddabd89d0ff6fa09d59894f31c48122fdb8f17ac08b6839d13b3
```

### `dpkg` source package: `lsb=9.20160110ubuntu0.2`

Binary Packages:

- `lsb-base=9.20160110ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=9.20160110ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20160110ubuntu0.2.dsc' lsb_9.20160110ubuntu0.2.dsc 2160 SHA256:673883614cba3ffc8efef9103ee80164e4744abf3aac80abd7535f9d027886c5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_9.20160110ubuntu0.2.tar.xz' lsb_9.20160110ubuntu0.2.tar.xz 57832 SHA256:deb95383b904e6014bfa1efca7700b0a9a6596f2b9afbcdd52de8b75d64e2d3a
```

### `dpkg` source package: `lvm2=2.02.133-1ubuntu10`

Binary Packages:

- `libdevmapper1.02.1:amd64=2:1.02.110-1ubuntu10`

Licenses: (parsed from: `/usr/share/doc/libdevmapper1.02.1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris lvm2=2.02.133-1ubuntu10
'http://archive.ubuntu.com/ubuntu/pool/main/l/lvm2/lvm2_2.02.133-1ubuntu10.dsc' lvm2_2.02.133-1ubuntu10.dsc 3151 SHA256:49b49c886da1f5b5d078875a025ee5f37d049e77c3abe49568b3b6fd7babb5de
'http://archive.ubuntu.com/ubuntu/pool/main/l/lvm2/lvm2_2.02.133.orig.tar.xz' lvm2_2.02.133.orig.tar.xz 1356636 SHA256:79c6fc85f28b6af1870d7e3b06d8339270746a5028f47a5b412f4394156ed846
'http://archive.ubuntu.com/ubuntu/pool/main/l/lvm2/lvm2_2.02.133-1ubuntu10.debian.tar.xz' lvm2_2.02.133-1ubuntu10.debian.tar.xz 42320 SHA256:54f13369a8576c98472dcc9121e3ac4fd69f3af02d2aa4a7aeb0224e87176d1e
```

### `dpkg` source package: `lz4=0.0~r131-2ubuntu2`

Binary Packages:

- `liblz4-1:amd64=0.0~r131-2ubuntu2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=0.0~r131-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu2.dsc' lz4_0.0~r131-2ubuntu2.dsc 2007 SHA256:123f23834f83a4dca6d74a611cc0294491bd339d2e0be04d65783d6debbccc02
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131.orig.tar.gz' lz4_0.0~r131.orig.tar.gz 133784 SHA256:9d4d00614d6b9dec3114b33d1224b6262b99ace24434c53487a0c8fd0b18cfed
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_0.0~r131-2ubuntu2.debian.tar.xz' lz4_0.0~r131-2ubuntu2.debian.tar.xz 5224 SHA256:c0afb4a440b1e7b803e2d9dcf616be539c1d16baebc681cdf837000e4c5077b7
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

### `dpkg` source package: `m4=1.4.17-5`

Binary Packages:

- `m4=1.4.17-5`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.17-5
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.17-5.dsc' m4_1.4.17-5.dsc 1411 SHA256:4fb85651ee1e951f17304042e83253d7ca75a2f962be9796b10aad5ac96f5524
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.17.orig.tar.xz' m4_1.4.17.orig.tar.xz 1149088 SHA256:f0543c3beb51fa6b3337d8025331591e0e18d8ec2886ed391f1aade43477d508
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.17-5.debian.tar.xz' m4_1.4.17-5.debian.tar.xz 12544 SHA256:74045004fae4025bc850c2d53e4d95ed7374b9c22c846c3d3596e39986697049
```

### `dpkg` source package: `make-dfsg=4.1-6`

Binary Packages:

- `make=4.1-6`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.1-6
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-6.dsc' make-dfsg_4.1-6.dsc 1840 SHA256:c28066ebe2002e4791ac3a4e808d8a5f0bed75eff8e0462449a08ab767153361
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1.orig.tar.gz' make-dfsg_4.1.orig.tar.gz 1350231 SHA256:b3ed04fb6718289e4a430afbe2df6ecba9177aad9f6d09aaf38e5409262ca8a3
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.1-6.diff.gz' make-dfsg_4.1-6.diff.gz 42552 SHA256:b647e6961a9707ea009de85fb65f8156143deab139be1636a200abdffe5e91c3
```

### `dpkg` source package: `makedev=2.3.1-93ubuntu2~ubuntu16.04.1`

Binary Packages:

- `makedev=2.3.1-93ubuntu2~ubuntu16.04.1`

Licenses: (parsed from: `/usr/share/doc/makedev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris makedev=2.3.1-93ubuntu2~ubuntu16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/makedev/makedev_2.3.1-93ubuntu2~ubuntu16.04.1.dsc' makedev_2.3.1-93ubuntu2~ubuntu16.04.1.dsc 1855 SHA256:eb4f5db89cafe3d55b12f3c59041c6b0691936a0a69433e69f47fc55e09811a1
'http://archive.ubuntu.com/ubuntu/pool/main/m/makedev/makedev_2.3.1.orig.tar.gz' makedev_2.3.1.orig.tar.gz 9924 SHA256:8599712f2b2b3778eea344f59e1512cea284e802560317fac436585885a41dfa
'http://archive.ubuntu.com/ubuntu/pool/main/m/makedev/makedev_2.3.1-93ubuntu2~ubuntu16.04.1.diff.gz' makedev_2.3.1-93ubuntu2~ubuntu16.04.1.diff.gz 50340 SHA256:caf4da6a9b3903b03536c93a54aea44bf3cf74af7444e79038de12eecc73841b
```

### `dpkg` source package: `mawk=1.3.3-17ubuntu2`

Binary Packages:

- `mawk=1.3.3-17ubuntu2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.3-17ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu2.dsc' mawk_1.3.3-17ubuntu2.dsc 1843 SHA256:d9058945d45b0e9ee5dd1c9c2e16d8f28b96d5c2e777f743594096fa2a5e277b
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3.orig.tar.gz' mawk_1.3.3.orig.tar.gz 209942 SHA256:32649c46063d4ef0777a12ae6e9a26bcc920833d54e1abca7edb8d37481e7485
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.3-17ubuntu2.diff.gz' mawk_1.3.3-17ubuntu2.diff.gz 63882 SHA256:670103046767474be29e80f2143dc67e3d0b958972f5942c3df94883f978eded
```

### `dpkg` source package: `mercurial=3.7.3-1ubuntu1.2`

Binary Packages:

- `mercurial=3.7.3-1ubuntu1.2`
- `mercurial-common=3.7.3-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=3.7.3-1ubuntu1.2
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_3.7.3-1ubuntu1.2.dsc' mercurial_3.7.3-1ubuntu1.2.dsc 2387 SHA256:e7630314efbc0a71b73cc69f23a8d4a842605823d30eb0daf4cc37483cd7cff7
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_3.7.3.orig.tar.gz' mercurial_3.7.3.orig.tar.gz 4636732 SHA256:c099c42d74e2d520b61dd372cd996b0fa7605c06617834fd7b13c79b9a9a5b30
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_3.7.3-1ubuntu1.2.debian.tar.xz' mercurial_3.7.3-1ubuntu1.2.debian.tar.xz 65164 SHA256:a9e06adde535207d4b633ba209621fb030a2ee06b0173d3eec4233b561783b4b
```

### `dpkg` source package: `mime-support=3.59ubuntu1`

Binary Packages:

- `mime-support=3.59ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.59ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.59ubuntu1.dsc' mime-support_3.59ubuntu1.dsc 1711 SHA256:37703b2273222f23dd8ad048f898a381412df0a76473047e0b7757a8043ff354
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.59ubuntu1.tar.gz' mime-support_3.59ubuntu1.tar.gz 37508 SHA256:55ee4350da8425fb65e7c9b60518e20de09c5a72d08148e644fcefe7abf9c83d
```

### `dpkg` source package: `mpclib3=1.0.3-1`

Binary Packages:

- `libmpc3:amd64=1.0.3-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.0.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.0.3-1.dsc' mpclib3_1.0.3-1.dsc 1940 SHA256:4b424e1c6063d48fd0d045b5afe37004346dae267ced0994fa8e11ff41cada45
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.0.3.orig.tar.gz' mpclib3_1.0.3.orig.tar.gz 669925 SHA256:617decc6ea09889fb08ede330917a00b16809b8db88c29c31bfbb49cbf88ecc3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.0.3-1.diff.gz' mpclib3_1.0.3-1.diff.gz 3684 SHA256:5a3fe9a7eddb4428d42e95f5919cce517f17411acdb2a73013a8f1a2bb246565
```

### `dpkg` source package: `mpfr4=3.1.4-1`

Binary Packages:

- `libmpfr4:amd64=3.1.4-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr4/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=3.1.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_3.1.4-1.dsc' mpfr4_3.1.4-1.dsc 1965 SHA256:98c867cd9e2d82fd9f1bae851a3ec8e76aa35d9e54d9e0d75a2fcd97f08992a9
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_3.1.4.orig.tar.xz' mpfr4_3.1.4.orig.tar.xz 1122152 SHA256:761413b16d749c53e2bfd2b1dfaa3b027b0e793e404b90b5fbaeef60af6517f5
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_3.1.4-1.debian.tar.xz' mpfr4_3.1.4-1.debian.tar.xz 9656 SHA256:e0562521ac0ef9fc2039ef1305962ee1ad529ae2210e197cee0080b1facc4d60
```

### `dpkg` source package: `mysql-5.7=5.7.30-0ubuntu0.16.04.1`

Binary Packages:

- `libmysqlclient-dev=5.7.30-0ubuntu0.16.04.1`
- `libmysqlclient20:amd64=5.7.30-0ubuntu0.16.04.1`
- `mysql-common=5.7.30-0ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libmysqlclient-dev/copyright`, `/usr/share/doc/libmysqlclient20/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-like`
- `Boost`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL`
- `LGPL-2`
- `SWsoft`
- `public-domain`
- `zlib/libpng`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ncurses=6.0+20160213-1ubuntu1`

Binary Packages:

- `libncurses5:amd64=6.0+20160213-1ubuntu1`
- `libncurses5-dev:amd64=6.0+20160213-1ubuntu1`
- `libncursesw5:amd64=6.0+20160213-1ubuntu1`
- `libncursesw5-dev:amd64=6.0+20160213-1ubuntu1`
- `libtinfo-dev:amd64=6.0+20160213-1ubuntu1`
- `libtinfo5:amd64=6.0+20160213-1ubuntu1`
- `ncurses-base=6.0+20160213-1ubuntu1`
- `ncurses-bin=6.0+20160213-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.0+20160213-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.0+20160213-1ubuntu1.dsc' ncurses_6.0+20160213-1ubuntu1.dsc 4379 SHA256:16628fbe5a690f6f8d147a54d0ba6900a0afeaa51d318475781ce3f14df1ca79
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.0+20160213.orig.tar.gz' ncurses_6.0+20160213.orig.tar.gz 3153008 SHA256:20269c2dd62a311b9a3fb9f25638d35a057a5ece5f8d6caf4e70a3da6f01082c
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.0+20160213-1ubuntu1.debian.tar.xz' ncurses_6.0+20160213-1ubuntu1.debian.tar.xz 54496 SHA256:9551738e1bdc425d12897cc459ce5ce40b5e12530b144b731c0a7b3e077c07c7
```

### `dpkg` source package: `netbase=5.3`

Binary Packages:

- `netbase=5.3`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=5.3
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.3.dsc' netbase_5.3.dsc 1308 SHA256:fcb9c97fe55277f775fd5a39933ca0189b9a983c6cf1abc8184fc29b8e1d77cb
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_5.3.tar.xz' netbase_5.3.tar.xz 31292 SHA256:81f6c69795044d62b8ad959cf9daf049d0545fd466c52860ad3f933b1e97b88b
```

### `dpkg` source package: `nettle=3.2-1ubuntu0.16.04.1`

Binary Packages:

- `libhogweed4:amd64=3.2-1ubuntu0.16.04.1`
- `libnettle6:amd64=3.2-1ubuntu0.16.04.1`

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
$ apt-get source -qq --print-uris nettle=3.2-1ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.2-1ubuntu0.16.04.1.dsc' nettle_3.2-1ubuntu0.16.04.1.dsc 2200 SHA256:15cbaa7c21e695c264ee3ec33be7ead629816f34cd0e2ea910300d9f6f084835
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.2.orig.tar.gz' nettle_3.2.orig.tar.gz 1879604 SHA256:ea4283def236413edab5a4cf9cf32adf540c8df1b9b67641cfc2302fca849d97
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.2-1ubuntu0.16.04.1.debian.tar.xz' nettle_3.2-1ubuntu0.16.04.1.debian.tar.xz 21340 SHA256:49e9715ec8f211831efeaa90122fb16126e39d2cf0739fecd572621b5e55a097
```

### `dpkg` source package: `openexr=2.2.0-10ubuntu2.3`

Binary Packages:

- `libopenexr-dev=2.2.0-10ubuntu2.3`
- `libopenexr22:amd64=2.2.0-10ubuntu2.3`

Licenses: (parsed from: `/usr/share/doc/libopenexr-dev/copyright`, `/usr/share/doc/libopenexr22/copyright`)

- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.2.0-10ubuntu2.3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-10ubuntu2.3.dsc' openexr_2.2.0-10ubuntu2.3.dsc 2395 SHA256:751a0d8a271cd923e76020b46e16500cdd116291509b3fefa0108a4cb6b3d711
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0.orig.tar.gz' openexr_2.2.0.orig.tar.gz 14489661 SHA256:36a012f6c43213f840ce29a8b182700f6cf6b214bea0d5735594136b44914231
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-10ubuntu2.3.debian.tar.xz' openexr_2.2.0-10ubuntu2.3.debian.tar.xz 44996 SHA256:3ad0a21dc7ede66f6acf664ea57f7ba3dce00e4a2139a43cca1876b4c2fd417b
```

### `dpkg` source package: `openldap=2.4.42+dfsg-2ubuntu3.9`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.42+dfsg-2ubuntu3.9`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.42+dfsg-2ubuntu3.9
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.42+dfsg-2ubuntu3.9.dsc' openldap_2.4.42+dfsg-2ubuntu3.9.dsc 3054 SHA256:cbf8d203c54a73edc7611e81864900ac8f8c27b5944b44fc94d5130993918ade
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.42+dfsg.orig.tar.gz' openldap_2.4.42+dfsg.orig.tar.gz 4813173 SHA256:5f56e4e3584f7a4b4c8437a2c985b2f519836946be77ef1aa43a5d20c02ea97b
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.42+dfsg-2ubuntu3.9.debian.tar.xz' openldap_2.4.42+dfsg-2ubuntu3.9.debian.tar.xz 181648 SHA256:d533a0257b2e86abdafc89e386d27585ac91eaf1ca7da33abb982185c704a3d6
```

### `dpkg` source package: `openssh=1:7.2p2-4ubuntu2.10`

Binary Packages:

- `openssh-client=1:7.2p2-4ubuntu2.10`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:7.2p2-4ubuntu2.10
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_7.2p2-4ubuntu2.10.dsc' openssh_7.2p2-4ubuntu2.10.dsc 2974 SHA256:bbdd31c1ea9ced8cd3350cd943e3600dd911e52315e747904d3dbb405a5ab6c2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_7.2p2.orig.tar.gz' openssh_7.2p2.orig.tar.gz 1499808 SHA256:a72781d1a043876a224ff1b0032daa4094d87565a68528759c1c2cab5482548c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_7.2p2-4ubuntu2.10.debian.tar.xz' openssh_7.2p2-4ubuntu2.10.debian.tar.xz 178928 SHA256:c789931ee9c0abfcecd4c275d472cc46583cb06f986a4df330a550fb226e89db
```

### `dpkg` source package: `openssl=1.0.2g-1ubuntu4.16`

Binary Packages:

- `libssl-dev:amd64=1.0.2g-1ubuntu4.16`
- `libssl1.0.0:amd64=1.0.2g-1ubuntu4.16`
- `openssl=1.0.2g-1ubuntu4.16`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.0.2g-1ubuntu4.16
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g-1ubuntu4.16.dsc' openssl_1.0.2g-1ubuntu4.16.dsc 2453 SHA256:3a8e643acae8c4e627ed97b05e51c2eaf873680170792db4e5dce4df58b40642
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g.orig.tar.gz' openssl_1.0.2g.orig.tar.gz 5266102 SHA256:b784b1b3907ce39abf4098702dade6365522a253ad1552e267a9a0e89594aa33
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g-1ubuntu4.16.debian.tar.xz' openssl_1.0.2g-1ubuntu4.16.debian.tar.xz 136592 SHA256:d306228914752dd61e390d4d00ce8f6bbf3d3702ecfa116b255eebfb8d52dd33
```

### `dpkg` source package: `p11-kit=0.23.2-5~ubuntu16.04.1`

Binary Packages:

- `libp11-kit0:amd64=0.23.2-5~ubuntu16.04.1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.2-5~ubuntu16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.2-5~ubuntu16.04.1.dsc' p11-kit_0.23.2-5~ubuntu16.04.1.dsc 2326 SHA256:02e852c8a77600d3856587beeaa390a71210545f49ce027adb10b29ec14c6d54
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.2.orig.tar.gz' p11-kit_0.23.2.orig.tar.gz 1022733 SHA256:ba726ea8303c97467a33fca50ee79b7b35212964be808ecf9b145e9042fdfaf0
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.2-5~ubuntu16.04.1.debian.tar.xz' p11-kit_0.23.2-5~ubuntu16.04.1.debian.tar.xz 15208 SHA256:8d916c95e619ba3bf98aaaaf92c6115e09c4222925be1a43e6882c77d5e5a166
```

### `dpkg` source package: `pam=1.1.8-3.2ubuntu2.1`

Binary Packages:

- `libpam-modules:amd64=1.1.8-3.2ubuntu2.1`
- `libpam-modules-bin=1.1.8-3.2ubuntu2.1`
- `libpam-runtime=1.1.8-3.2ubuntu2.1`
- `libpam0g:amd64=1.1.8-3.2ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.1.8-3.2ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.1.8-3.2ubuntu2.1.dsc' pam_1.1.8-3.2ubuntu2.1.dsc 2249 SHA256:2fd155508c2786bb48f0e1ebe604d268f61303035c203c7a90d5f5b97e742cdc
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.1.8.orig.tar.gz' pam_1.1.8.orig.tar.gz 1892765 SHA256:4183409a450708a976eca5af561dbf4f0490141a08e86e4a1e649c7c1b094876
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.1.8-3.2ubuntu2.1.diff.gz' pam_1.1.8-3.2ubuntu2.1.diff.gz 198992 SHA256:1e1bd29430a9734bd8e5415952c1bfc16dedc94b5d3bbc678d728daa096edb29
```

### `dpkg` source package: `pango1.0=1.38.1-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.38.1-1`
- `libpangocairo-1.0-0:amd64=1.38.1-1`
- `libpangoft2-1.0-0:amd64=1.38.1-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `LGPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.38.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.38.1-1.dsc' pango1.0_1.38.1-1.dsc 3171 SHA256:786e84e8a00ab1b062f05356dbd371b771ef3fe3cf09144ba1de6b0668929e24
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.38.1.orig.tar.xz' pango1.0_1.38.1.orig.tar.xz 1047372 SHA256:1320569f6c6d75d6b66172b2d28e59c56ee864ee9df202b76799c4506a214eb7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pango1.0/pango1.0_1.38.1-1.debian.tar.xz' pango1.0_1.38.1-1.debian.tar.xz 29216 SHA256:673a39fb35b469af653a819a65e778563fc4be3fa8265e7321006f9be06df143
```

### `dpkg` source package: `patch=2.7.5-1ubuntu0.16.04.2`

Binary Packages:

- `patch=2.7.5-1ubuntu0.16.04.2`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.5-1ubuntu0.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.5-1ubuntu0.16.04.2.dsc' patch_2.7.5-1ubuntu0.16.04.2.dsc 1950 SHA256:f80df1b7bff022afff6309230c6fc50c4eb5d32666ff3632f4b5bfa5b74f8805
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.5.orig.tar.xz' patch_2.7.5.orig.tar.xz 727704 SHA256:fd95153655d6b95567e623843a0e77b81612d502ecf78a489a4aed7867caa299
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.5-1ubuntu0.16.04.2.debian.tar.xz' patch_2.7.5-1ubuntu0.16.04.2.debian.tar.xz 12588 SHA256:4274779969c41d90db394717edde6e783e504c750e71ce61ec9077ad299e5bcf
```

### `dpkg` source package: `pcre3=2:8.38-3.1`

Binary Packages:

- `libpcre16-3:amd64=2:8.38-3.1`
- `libpcre3:amd64=2:8.38-3.1`
- `libpcre3-dev:amd64=2:8.38-3.1`
- `libpcre32-3:amd64=2:8.38-3.1`
- `libpcrecpp0v5:amd64=2:8.38-3.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.38-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38-3.1.dsc' pcre3_8.38-3.1.dsc 2074 SHA256:6a46bc62c33198fe38257f0dddecb4c534825f8f066bf88f2a45ad935b879885
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38.orig.tar.gz' pcre3_8.38.orig.tar.gz 2053336 SHA256:9883e419c336c63b0cb5202b09537c140966d585e4d0da66147dc513da13e629
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38-3.1.debian.tar.gz' pcre3_8.38-3.1.debian.tar.gz 32289 SHA256:9ee1b838c1de50cb5f6641016d0dd21b06f1038b9b7c3b1098e0a89b9c24b39f
```

### `dpkg` source package: `perl=5.22.1-9ubuntu0.6`

Binary Packages:

- `libperl5.22:amd64=5.22.1-9ubuntu0.6`
- `perl=5.22.1-9ubuntu0.6`
- `perl-base=5.22.1-9ubuntu0.6`
- `perl-modules-5.22=5.22.1-9ubuntu0.6`

Licenses: (parsed from: `/usr/share/doc/libperl5.22/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.22/copyright`)

- `Artistic`
- `Artistic,`
- `Artistic-2`
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
- `S2P`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.22.1-9ubuntu0.6
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.22.1-9ubuntu0.6.dsc' perl_5.22.1-9ubuntu0.6.dsc 2480 SHA256:5e45c28174bac9738045c0be2b13f82db99aa1148796c5cdfa4ee151a57ed9ed
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.22.1.orig.tar.xz' perl_5.22.1.orig.tar.xz 11223940 SHA256:9e87317d693ce828095204be0d09af8d60b8785533fadea1a82b6f0e071e5c79
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.22.1-9ubuntu0.6.debian.tar.xz' perl_5.22.1-9ubuntu0.6.debian.tar.xz 161972 SHA256:8ada4467517b405493c876ba78121ff4ec25eed15cfbbc65682da461050a1f6b
```

### `dpkg` source package: `pixman=0.33.6-1`

Binary Packages:

- `libpixman-1-0:amd64=0.33.6-1`
- `libpixman-1-dev=0.33.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.33.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6-1.dsc' pixman_0.33.6-1.dsc 2085 SHA256:08e94c263c3cde1c841458512705fa6a52a78c8f48e31f0bf3a2ae8a518eb51e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6.orig.tar.gz' pixman_0.33.6.orig.tar.gz 878996 SHA256:4e1e72c0ed31d10944f304976e87e6c87b441c853713eeecf115e22c23d4b17d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6-1.diff.gz' pixman_0.33.6-1.diff.gz 315093 SHA256:f382e753698aa95fae9019128a4b463935695b4c906785397f3eaa04e05a06d5
```

### `dpkg` source package: `pkg-config=0.29.1-0ubuntu1`

Binary Packages:

- `pkg-config=0.29.1-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.1-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu1.dsc' pkg-config_0.29.1-0ubuntu1.dsc 1842 SHA256:0ade40d184e9684f9e22e622022f1b798123cc63cd37d669f664f47dddc5e072
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1.orig.tar.gz' pkg-config_0.29.1.orig.tar.gz 2013454 SHA256:beb43c9e064555469bd4390dcfd8030b1536e0aa103f08d7abf7ae8cac0cb001
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu1.diff.gz' pkg-config_0.29.1-0ubuntu1.diff.gz 12597 SHA256:1c44aeeec1896a69f21861e9b9e18bb783258d57f4bd678b173b3890f1a209bf
```

### `dpkg` source package: `postgresql-9.5=9.5.21-0ubuntu0.16.04.1`

Binary Packages:

- `libpq-dev=9.5.21-0ubuntu0.16.04.1`
- `libpq5:amd64=9.5.21-0ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libpq-dev/copyright`, `/usr/share/doc/libpq5/copyright`)

- `Custom-Unicode`
- `Custom-pg_dump`
- `Custom-regex`
- `PostgreSQL`
- `Tcl`
- `almost exclusively BSD`

Source:

```console
$ apt-get source -qq --print-uris postgresql-9.5=9.5.21-0ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-9.5/postgresql-9.5_9.5.21-0ubuntu0.16.04.1.dsc' postgresql-9.5_9.5.21-0ubuntu0.16.04.1.dsc 3777 SHA256:ed8e0aec9a736b4f9f01f57fe8d1cc8e99c48bca7c421fb1ca7ea8faf298926f
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-9.5/postgresql-9.5_9.5.21.orig.tar.bz2' postgresql-9.5_9.5.21.orig.tar.bz2 17640928 SHA256:7eb56e4fa877243c2df78adc5a0ef02f851060c282682b4bb97b854100fb732c
'http://archive.ubuntu.com/ubuntu/pool/main/p/postgresql-9.5/postgresql-9.5_9.5.21-0ubuntu0.16.04.1.debian.tar.xz' postgresql-9.5_9.5.21-0ubuntu0.16.04.1.debian.tar.xz 27344 SHA256:46f5fb5b38b475805ee114de8c8feac211df6645263b9d39de6fb04b2304b6c5
```

### `dpkg` source package: `procps=2:3.3.10-4ubuntu2.5`

Binary Packages:

- `libprocps4:amd64=2:3.3.10-4ubuntu2.5`
- `procps=2:3.3.10-4ubuntu2.5`

Licenses: (parsed from: `/usr/share/doc/libprocps4/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.10-4ubuntu2.5
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10-4ubuntu2.5.dsc' procps_3.3.10-4ubuntu2.5.dsc 2227 SHA256:bf17eb5a055ff767dcc10ce3696f2e7622da96bbe8ac3c9d2d5aa92697a23282
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10.orig.tar.xz' procps_3.3.10.orig.tar.xz 814816 SHA256:40a3d2b0489e057d85564f4f304083b24fc699b39ea828610183fb9f0a6ebe97
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10-4ubuntu2.5.debian.tar.xz' procps_3.3.10-4ubuntu2.5.debian.tar.xz 44704 SHA256:e0f01bc3e2569fbe3780f0c5943d916e8f9c0a74bd065b3f328383bf8ff10a40
```

### `dpkg` source package: `python-defaults=2.7.12-1~16.04`

Binary Packages:

- `libpython-stdlib:amd64=2.7.12-1~16.04`
- `python=2.7.12-1~16.04`
- `python-minimal=2.7.12-1~16.04`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.12-1~16.04
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.12-1~16.04.dsc' python-defaults_2.7.12-1~16.04.dsc 2659 SHA256:e8a6f2510d07b565a6be42b8e8e05e2f3d30581883934efeb75904026207c5fc
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-defaults/python-defaults_2.7.12-1~16.04.tar.gz' python-defaults_2.7.12-1~16.04.tar.gz 280070 SHA256:843d90debb74aedf336532f90d181e109a7d685275177e069a1df02faa42d732
```

### `dpkg` source package: `python2.7=2.7.12-1ubuntu0~16.04.12`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.12-1ubuntu0~16.04.12`
- `libpython2.7-stdlib:amd64=2.7.12-1ubuntu0~16.04.12`
- `python2.7=2.7.12-1ubuntu0~16.04.12`
- `python2.7-minimal=2.7.12-1ubuntu0~16.04.12`

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
$ apt-get source -qq --print-uris python2.7=2.7.12-1ubuntu0~16.04.12
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.12-1ubuntu0~16.04.12.dsc' python2.7_2.7.12-1ubuntu0~16.04.12.dsc 3391 SHA256:4f689a676d8901fd4b9d42465d81bc1ae0d2daff59faf80e96b8b3678a05daa0
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.12.orig.tar.gz' python2.7_2.7.12.orig.tar.gz 16935960 SHA256:3cb522d17463dfa69a155ab18cffa399b358c966c0363d6c8b5b3bf1384da4b6
'http://archive.ubuntu.com/ubuntu/pool/main/p/python2.7/python2.7_2.7.12-1ubuntu0~16.04.12.diff.gz' python2.7_2.7.12-1ubuntu0~16.04.12.diff.gz 309624 SHA256:1449a1d51f938581bba6442dfa4075fbb809de24d4be6cdb7f9c213e88a86339
```

### `dpkg` source package: `readline6=6.3-8ubuntu2`

Binary Packages:

- `libreadline-dev:amd64=6.3-8ubuntu2`
- `libreadline6:amd64=6.3-8ubuntu2`
- `libreadline6-dev:amd64=6.3-8ubuntu2`
- `readline-common=6.3-8ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline6/copyright`, `/usr/share/doc/libreadline6-dev/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline6=6.3-8ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline6/readline6_6.3-8ubuntu2.dsc' readline6_6.3-8ubuntu2.dsc 2566 SHA256:3c7e3168dd1510f040325c1ab1e28c7fbde34d1a899005a98a894a9f27bd98f6
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline6/readline6_6.3.orig.tar.gz' readline6_6.3.orig.tar.gz 2468560 SHA256:56ba6071b9462f980c5a72ab0023893b65ba6debb4eeb475d7a563dc65cafd43
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline6/readline6_6.3-8ubuntu2.debian.tar.xz' readline6_6.3-8ubuntu2.debian.tar.xz 31232 SHA256:32d4f30dc92d79d722b04c2b678883245d2eccff2ed4f8591faebca7e6d81948
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d-1ubuntu0.1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.dsc' rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.dsc 2408 SHA256:0b82d42fecf5e830ec00f6d3191d582908e1e4feed57c031d9ab02b4b0d4f2db
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.orig.tar.gz 149016 SHA256:f8eb8d0c8ed085c90666ba0e8fbe0e960e0cf0c2a58604fda3ed85a28f2ef5f6
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d-1ubuntu0.1.debian.tar.xz 9000 SHA256:9178a6648106397566589db2c7a6f8da9cd0273ee955df7f4030f02a63013cf9
```

### `dpkg` source package: `sed=4.2.2-7`

Binary Packages:

- `sed=4.2.2-7`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris sed=4.2.2-7
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.2.2-7.dsc' sed_4.2.2-7.dsc 1974 SHA256:42f5764a279ac3f9b31d9e922024b519b950b35e82830e552839cd41fbb8e0b0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.2.2.orig.tar.bz2' sed_4.2.2.orig.tar.bz2 1059414 SHA256:f048d1838da284c8bc9753e4506b85a1e0cc1ea8999d36f6995bcb9460cddbd7
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.2.2-7.debian.tar.xz' sed_4.2.2-7.debian.tar.xz 85048 SHA256:416b70f601b40246c1daf7261f117ea9ff01564f574bd34871573fc5c9f74db7
```

### `dpkg` source package: `sensible-utils=0.0.9ubuntu0.16.04.1`

Binary Packages:

- `sensible-utils=0.0.9ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.9ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.9ubuntu0.16.04.1.dsc' sensible-utils_0.0.9ubuntu0.16.04.1.dsc 1514 SHA256:7ba1a4fac5ca66adc0ea77634931e1843730ce76897964b58cc8d3ec67e74e0c
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.9ubuntu0.16.04.1.tar.xz' sensible-utils_0.0.9ubuntu0.16.04.1.tar.xz 54048 SHA256:3790882bdc1a54691ed28084b161bc0a01fc8f9adf49e6f7497d72b54fb07ee3
```

### `dpkg` source package: `serf=1.3.8-1`

Binary Packages:

- `libserf-1-1:amd64=1.3.8-1`

Licenses: (parsed from: `/usr/share/doc/libserf-1-1/copyright`)

- `Apache-2.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/serf/1.3.8-1/


### `dpkg` source package: `shadow=1:4.2-3.1ubuntu5.4`

Binary Packages:

- `login=1:4.2-3.1ubuntu5.4`
- `passwd=1:4.2-3.1ubuntu5.4`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.2-3.1ubuntu5.4
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.2-3.1ubuntu5.4.dsc' shadow_4.2-3.1ubuntu5.4.dsc 2513 SHA256:964bf283d4a1ec090c4e4044133789485ca608206cf87dda678c3350eda3590d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.2.orig.tar.xz' shadow_4.2.orig.tar.xz 1088696 SHA256:c5bd72c4ecb438b99289e4630b22ea0626987a378d084910dbe59eceaa34be1d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.2-3.1ubuntu5.4.debian.tar.xz' shadow_4.2-3.1ubuntu5.4.debian.tar.xz 506364 SHA256:50ccd266ff5bdc8577fe090b04c9be675340bf59b44fa843cd20174055540a15
```

### `dpkg` source package: `shared-mime-info=1.5-2ubuntu0.2`

Binary Packages:

- `shared-mime-info=1.5-2ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/shared-mime-info/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris shared-mime-info=1.5-2ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.5-2ubuntu0.2.dsc' shared-mime-info_1.5-2ubuntu0.2.dsc 2289 SHA256:ca9e4459755bc42b5d54938bb20b5c1cac9144e590f690583169ac349bfcd669
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.5.orig.tar.xz' shared-mime-info_1.5.orig.tar.xz 559040 SHA256:d6412840eb265bf36e61fd7b6fc6bea21b0f58cb22bed16f2ccccdd54bea4180
'http://archive.ubuntu.com/ubuntu/pool/main/s/shared-mime-info/shared-mime-info_1.5-2ubuntu0.2.debian.tar.xz' shared-mime-info_1.5-2ubuntu0.2.debian.tar.xz 10548 SHA256:7687ced629abcb5e53fb5686403393c99a89dec08a8a8070b9818242b0bf4b92
```

### `dpkg` source package: `six=1.10.0-3`

Binary Packages:

- `python-six=1.10.0-3`

Licenses: (parsed from: `/usr/share/doc/python-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.10.0-3
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.10.0-3.dsc' six_1.10.0-3.dsc 2158 SHA256:71f2d5ff8b999c471cc2e92712befe482351a5ae226321e0e795bc683c8729cb
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.10.0.orig.tar.gz' six_1.10.0.orig.tar.gz 29630 SHA256:105f8d68616f8248e24bf0e9372ef04d3cc10104f1980f54d57b2ce73a5ad56a
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.10.0-3.debian.tar.xz' six_1.10.0-3.debian.tar.xz 3668 SHA256:860cc57244ea4e69eb4ee3ad1b823472c20d868c1cc25745b236ba6c9e1f3563
```

### `dpkg` source package: `sqlite3=3.11.0-1ubuntu1.5`

Binary Packages:

- `libsqlite3-0:amd64=3.11.0-1ubuntu1.5`
- `libsqlite3-dev:amd64=3.11.0-1ubuntu1.5`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.11.0-1ubuntu1.5
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0-1ubuntu1.5.dsc' sqlite3_3.11.0-1ubuntu1.5.dsc 2625 SHA256:296116f2ab465baecbd2bff99f4a994549737a45302cc6e5184616a07d227003
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0.orig-www.tar.xz' sqlite3_3.11.0.orig-www.tar.xz 3135012 SHA256:99843a91a1da29cf07269df49b37b0cd8a75035a88aacdb1186f94a9a217bab3
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0.orig.tar.xz' sqlite3_3.11.0.orig.tar.xz 5122440 SHA256:79fb8800b8744337d5317270899a5a40612bb76f81517e131bf496c26b044490
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0-1ubuntu1.5.debian.tar.xz' sqlite3_3.11.0-1ubuntu1.5.debian.tar.xz 45984 SHA256:05dbaed6db014ac494c7d0322d572196e4538d73cef7579e9d033e704cf086f8
```

### `dpkg` source package: `subversion=1.9.3-2ubuntu1.3`

Binary Packages:

- `libsvn1:amd64=1.9.3-2ubuntu1.3`
- `subversion=1.9.3-2ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libsvn1/copyright`, `/usr/share/doc/subversion/copyright`)

- `Apache-2.0`
- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris subversion=1.9.3-2ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/s/subversion/subversion_1.9.3-2ubuntu1.3.dsc' subversion_1.9.3-2ubuntu1.3.dsc 3287 SHA256:e6803d4fec28d482f552cdc00ceac22faca3364688cee0c903f293609915fad4
'http://archive.ubuntu.com/ubuntu/pool/main/s/subversion/subversion_1.9.3.orig.tar.gz' subversion_1.9.3.orig.tar.gz 10600934 SHA256:74cd21d2f8a2a54e4dbd2389fe1605a19dbda8ba88ffc4bb0edc9a66e143cc93
'http://archive.ubuntu.com/ubuntu/pool/main/s/subversion/subversion_1.9.3-2ubuntu1.3.diff.gz' subversion_1.9.3-2ubuntu1.3.diff.gz 2434888 SHA256:26c82d098c0f513d838bdbba3159a6ab20fca0f0e1797496f1428d73f1b0cdbb
```

### `dpkg` source package: `systemd=229-4ubuntu21.28`

Binary Packages:

- `libsystemd0:amd64=229-4ubuntu21.28`
- `libudev1:amd64=229-4ubuntu21.28`
- `systemd=229-4ubuntu21.28`
- `systemd-sysv=229-4ubuntu21.28`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`, `/usr/share/doc/systemd/copyright`, `/usr/share/doc/systemd-sysv/copyright`)

- `CC0`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=229-4ubuntu21.28
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229-4ubuntu21.28.dsc' systemd_229-4ubuntu21.28.dsc 4643 SHA256:d1dba84ee92a4d5fc5a8a7b2568afebc7db1c7d113f23042c7ee19b1c222de6c
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229.orig.tar.gz' systemd_229.orig.tar.gz 4319173 SHA256:b51b0a48d1beb388d95bd6a98d62be05490335d4bb388aefecdcb576e91e0741
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229-4ubuntu21.28.debian.tar.xz' systemd_229-4ubuntu21.28.debian.tar.xz 312524 SHA256:8be42f694303095740a7c8381a0914b4573c7a8c18b97a844ebd3c0954e31eb5
```

### `dpkg` source package: `sysvinit=2.88dsf-59.3ubuntu2`

Binary Packages:

- `initscripts=2.88dsf-59.3ubuntu2`
- `sysv-rc=2.88dsf-59.3ubuntu2`
- `sysvinit-utils=2.88dsf-59.3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/initscripts/copyright`, `/usr/share/doc/sysv-rc/copyright`, `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.88dsf-59.3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.3ubuntu2.dsc' sysvinit_2.88dsf-59.3ubuntu2.dsc 2284 SHA256:a64f0c2c11c14c8bf57fee7c583ae38ea710ec3288c3d840daeeec5a2eab1676
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf.orig.tar.gz' sysvinit_2.88dsf.orig.tar.gz 125330 SHA256:b016f937958d2809a020d407e1287bdc09abf1d44efaa96530e2ea57f544f4e8
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.88dsf-59.3ubuntu2.debian.tar.xz' sysvinit_2.88dsf-59.3ubuntu2.debian.tar.xz 134864 SHA256:d4cf7aa3d6c1f8727cbd699395053d541844a9ff02ea5e6a1119eb90604586b8
```

### `dpkg` source package: `tar=1.28-2.1ubuntu0.1`

Binary Packages:

- `tar=1.28-2.1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.28-2.1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.28-2.1ubuntu0.1.dsc' tar_1.28-2.1ubuntu0.1.dsc 2025 SHA256:b4ed109da748b893bfb036dd81251156181573659b35e506e5c8bc8c7c155fd4
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.28.orig.tar.xz' tar_1.28.orig.tar.xz 1756440 SHA256:6da98f52fc469754dbde475c861581036ff2c83a1ef4f7250292935139f587d9
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.28-2.1ubuntu0.1.debian.tar.xz' tar_1.28-2.1ubuntu0.1.debian.tar.xz 36868 SHA256:1933bd564d70d3d0cf085291969af36b2461265270be25f3819cc033f72c1ac6
```

### `dpkg` source package: `tiff=4.0.6-1ubuntu0.7`

Binary Packages:

- `libtiff5:amd64=4.0.6-1ubuntu0.7`
- `libtiff5-dev:amd64=4.0.6-1ubuntu0.7`
- `libtiffxx5:amd64=4.0.6-1ubuntu0.7`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`, `/usr/share/doc/libtiff5-dev/copyright`, `/usr/share/doc/libtiffxx5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.6-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6-1ubuntu0.7.dsc' tiff_4.0.6-1ubuntu0.7.dsc 2399 SHA256:93e01b61c5e12478dd640d88b820ba68bbfa7fcf5aad1a0c6e14360b5491e3b8
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6.orig.tar.gz' tiff_4.0.6.orig.tar.gz 2192991 SHA256:4d57a50907b510e3049a4bba0d7888930fdfc16ce49f1bf693e5b6247370d68c
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6-1ubuntu0.7.debian.tar.xz' tiff_4.0.6-1ubuntu0.7.debian.tar.xz 63940 SHA256:469b5e0dbc6de4395ce1085583099533c15690fd5135b0475dda50c4c149388c
```

### `dpkg` source package: `ubuntu-keyring=2012.05.19.1`

Binary Packages:

- `ubuntu-keyring=2012.05.19.1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2012.05.19.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2012.05.19.1.dsc' ubuntu-keyring_2012.05.19.1.dsc 1505 SHA256:cd665a3c2a14d1029ecdc50612ed2c4853d94b2ded033577ea01923753463d1d
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2012.05.19.1.tar.gz' ubuntu-keyring_2012.05.19.1.tar.gz 21072 SHA256:9945fb0b2838fdda323ad8a186a04d304bc1ac8f8fb2a96b8d2c84a4ef517429
```

### `dpkg` source package: `ucf=3.0036`

Binary Packages:

- `ucf=3.0036`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0036
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0036.dsc' ucf_3.0036.dsc 1343 SHA256:e67a8a3012ac357c7759dabd93d258422b1003bad8c3f17f25fc2a289eeda3bb
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0036.tar.xz' ucf_3.0036.tar.xz 65020 SHA256:34aa44416106f1205376918386b2896edf21dd42b633133b5f8fedecae17fca8
```

### `dpkg` source package: `unzip=6.0-20ubuntu1`

Binary Packages:

- `unzip=6.0-20ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-20ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-20ubuntu1.dsc' unzip_6.0-20ubuntu1.dsc 1782 SHA256:b3a01c0cf67b19ae87c621f1362474283841a88e4388335dbe29dd331efb6814
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://archive.ubuntu.com/ubuntu/pool/main/u/unzip/unzip_6.0-20ubuntu1.debian.tar.xz' unzip_6.0-20ubuntu1.debian.tar.xz 19896 SHA256:0ddf122ef15b739e3ea06db4b9e80f40759dce23a2c886678881453a43bd0842
```

### `dpkg` source package: `ustr=1.0.4-5`

Binary Packages:

- `libustr-1.0-1:amd64=1.0.4-5`

Licenses: (parsed from: `/usr/share/doc/libustr-1.0-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris ustr=1.0.4-5
'http://archive.ubuntu.com/ubuntu/pool/main/u/ustr/ustr_1.0.4-5.dsc' ustr_1.0.4-5.dsc 2016 SHA256:3c06f54e4c05e76bf7c4d7192bbf3a7b259372c7448a4245e8317115808cf7c9
'http://archive.ubuntu.com/ubuntu/pool/main/u/ustr/ustr_1.0.4.orig.tar.gz' ustr_1.0.4.orig.tar.gz 301345 SHA256:4d293b6b9d9fe51d58441f4b09b1f0005fcad8256ae8048587789bf5dbefb62e
'http://archive.ubuntu.com/ubuntu/pool/main/u/ustr/ustr_1.0.4-5.debian.tar.xz' ustr_1.0.4-5.debian.tar.xz 24948 SHA256:a21e78acf82dcccef2893932ef7b85852419bfd9b18382e63c34e7710c1d7762
```

### `dpkg` source package: `util-linux=2.27.1-6ubuntu3.10`

Binary Packages:

- `bsdutils=1:2.27.1-6ubuntu3.10`
- `libblkid1:amd64=2.27.1-6ubuntu3.10`
- `libfdisk1:amd64=2.27.1-6ubuntu3.10`
- `libmount1:amd64=2.27.1-6ubuntu3.10`
- `libsmartcols1:amd64=2.27.1-6ubuntu3.10`
- `libuuid1:amd64=2.27.1-6ubuntu3.10`
- `mount=2.27.1-6ubuntu3.10`
- `util-linux=2.27.1-6ubuntu3.10`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`)

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
$ apt-get source -qq --print-uris util-linux=2.27.1-6ubuntu3.10
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1-6ubuntu3.10.dsc' util-linux_2.27.1-6ubuntu3.10.dsc 3960 SHA256:ba6324f1adbcb27671e9a51410c19dbfd60cab3aab7e6835b49f44986ea6fa89
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1.orig.tar.xz' util-linux_2.27.1.orig.tar.xz 3964512 SHA256:0a818fcdede99aec43ffe6ca5b5388bff80d162f2f7bd4541dca94fecb87a290
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1-6ubuntu3.10.debian.tar.xz' util-linux_2.27.1-6ubuntu3.10.debian.tar.xz 89428 SHA256:ca634fb3adc4742729638eacc16d66591447ccf4566e44f0572eec99c3d05983
```

### `dpkg` source package: `wget=1.17.1-1ubuntu1.5`

Binary Packages:

- `wget=1.17.1-1ubuntu1.5`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.17.1-1ubuntu1.5
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.17.1-1ubuntu1.5.dsc' wget_1.17.1-1ubuntu1.5.dsc 1935 SHA256:f099484626617379373d8dc84e7fc6f32b5128d544af26840be29668d948e5b3
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.17.1.orig.tar.gz' wget_1.17.1.orig.tar.gz 3801442 SHA256:029fbb93bdc1c0c5a7507b6076a6ec2f8d34204a85aa87e5b2f61a9405b290f5
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.17.1-1ubuntu1.5.debian.tar.xz' wget_1.17.1-1ubuntu1.5.debian.tar.xz 29484 SHA256:76f25fc0d1f935576e479501a529f4a173a2d896fbbff7920e38f4b0da86069a
```

### `dpkg` source package: `x11proto-core=7.0.31-1~ubuntu16.04.2`

Binary Packages:

- `x11proto-core-dev=7.0.31-1~ubuntu16.04.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-core=7.0.31-1~ubuntu16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-core/x11proto-core_7.0.31-1~ubuntu16.04.2.dsc' x11proto-core_7.0.31-1~ubuntu16.04.2.dsc 2097 SHA256:b7684cf8bf9107c9a48153020bd4388782468bfd64c5f0711cb2cc5328c4e325
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-core/x11proto-core_7.0.31.orig.tar.gz' x11proto-core_7.0.31.orig.tar.gz 367979 SHA256:6d755eaae27b45c5cc75529a12855fed5de5969b367ed05003944cf901ed43c7
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-core/x11proto-core_7.0.31-1~ubuntu16.04.2.diff.gz' x11proto-core_7.0.31-1~ubuntu16.04.2.diff.gz 30062 SHA256:85a4cbb575954e7bfb405c856bf1efb1358af5a14b0b687b86888dac8aa4d3a5
```

### `dpkg` source package: `x11proto-input=2.3.1-1`

Binary Packages:

- `x11proto-input-dev=2.3.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-input=2.3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-input/x11proto-input_2.3.1-1.dsc' x11proto-input_2.3.1-1.dsc 1937 SHA256:c43dcce256561df0c239d24a5d9653cf651bfc949dc1a98bb450b1f23dda0b21
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-input/x11proto-input_2.3.1.orig.tar.gz' x11proto-input_2.3.1.orig.tar.gz 236302 SHA256:23f65ac55c36ea8c378e30b4a4fd85317c95923134e3fe46569741b94c8ed4ca
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-input/x11proto-input_2.3.1-1.diff.gz' x11proto-input_2.3.1-1.diff.gz 5603 SHA256:c92b1b97ce557f3564bd5252f921c1bc510df00ef1a81323078181754b4a31ab
```

### `dpkg` source package: `x11proto-kb=1.0.7-0ubuntu1`

Binary Packages:

- `x11proto-kb-dev=1.0.7-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-kb=1.0.7-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-kb/x11proto-kb_1.0.7-0ubuntu1.dsc' x11proto-kb_1.0.7-0ubuntu1.dsc 1343 SHA256:8923c65eb2193e49be47f32311eb03ad818545a55059672da26ed1f8127b4ba2
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-kb/x11proto-kb_1.0.7.orig.tar.gz' x11proto-kb_1.0.7.orig.tar.gz 325858 SHA256:828cb275b91268b1a3ea950d5c0c5eb076c678fdf005d517411f89cc8c3bb416
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-kb/x11proto-kb_1.0.7-0ubuntu1.diff.gz' x11proto-kb_1.0.7-0ubuntu1.diff.gz 14128 SHA256:2782403bed56d6e19aee719fa1aee1136abe152b008a0bab93732b313fed490a
```

### `dpkg` source package: `x11proto-render=2:0.11.1-2`

Binary Packages:

- `x11proto-render-dev=2:0.11.1-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-render=2:0.11.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-render/x11proto-render_0.11.1-2.dsc' x11proto-render_0.11.1-2.dsc 1979 SHA256:5cebbcce7928bd468b0eb447d9da403e5228af1691549a529a9012d2f7d18948
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-render/x11proto-render_0.11.1.orig.tar.gz' x11proto-render_0.11.1.orig.tar.gz 124436 SHA256:a0a4be3cad9381ae28279ba5582e679491fc2bec9aab8a65993108bf8dbce5fe
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-render/x11proto-render_0.11.1-2.diff.gz' x11proto-render_0.11.1-2.diff.gz 14527 SHA256:614b7adf6f08bdf25bc7fb565f048e2f94e290c3bd056fa2485e093eb887c54f
```

### `dpkg` source package: `x11proto-xext=7.3.0-1`

Binary Packages:

- `x11proto-xext-dev=7.3.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris x11proto-xext=7.3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-xext/x11proto-xext_7.3.0-1.dsc' x11proto-xext_7.3.0-1.dsc 1997 SHA256:4b806c7f17f7dd466901111ce0862117541098025470601c251499d76affe9fc
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-xext/x11proto-xext_7.3.0.orig.tar.gz' x11proto-xext_7.3.0.orig.tar.gz 290814 SHA256:1b1bcdf91221e78c6c33738667a57bd9aaa63d5953174ad8ed9929296741c9f5
'http://archive.ubuntu.com/ubuntu/pool/main/x/x11proto-xext/x11proto-xext_7.3.0-1.diff.gz' x11proto-xext_7.3.0-1.diff.gz 16644 SHA256:68eec9363c7f8bcfbbaba68d6661284eb78fffccbddb293b95a6c85647cfcf6c
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

### `dpkg` source package: `xorg=1:7.7+13ubuntu3.1`

Binary Packages:

- `x11-common=1:7.7+13ubuntu3.1`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+13ubuntu3.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+13ubuntu3.1.dsc' xorg_7.7+13ubuntu3.1.dsc 2112 SHA256:5c0130212f42b56c6049fcbf9a03b9559ee4931c7d7b4741627189b3a5e01e21
'http://archive.ubuntu.com/ubuntu/pool/main/x/xorg/xorg_7.7+13ubuntu3.1.tar.gz' xorg_7.7+13ubuntu3.1.tar.gz 289897 SHA256:bd672adfec604657e3ac825649ad4f4ef727a8839612abc4fce760d57801778b
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

### `dpkg` source package: `xz-utils=5.1.1alpha+20120614-2ubuntu2`

Binary Packages:

- `liblzma-dev:amd64=5.1.1alpha+20120614-2ubuntu2`
- `liblzma5:amd64=5.1.1alpha+20120614-2ubuntu2`
- `xz-utils=5.1.1alpha+20120614-2ubuntu2`

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
$ apt-get source -qq --print-uris xz-utils=5.1.1alpha+20120614-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2ubuntu2.dsc' xz-utils_5.1.1alpha+20120614-2ubuntu2.dsc 2409 SHA256:0a8cb3d928d1327f70b998b713c10afd9cd064056f5973d48075cd3d0f7872ca
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614.orig.tar.gz' xz-utils_5.1.1alpha+20120614.orig.tar.gz 556454 SHA256:b168e63400db449a6e7b3a06e668f557ca27e3d70accbd29d2b5a98e15c00fee
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2ubuntu2.debian.tar.gz' xz-utils_5.1.1alpha+20120614-2ubuntu2.debian.tar.gz 156001 SHA256:e7743d4a96276ccffc4e171812e402a1f503f87df3b668ef0e58db6629146a18
```

### `dpkg` source package: `zlib=1:1.2.8.dfsg-2ubuntu4.3`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-2ubuntu4.3`
- `zlib1g-dev:amd64=1:1.2.8.dfsg-2ubuntu4.3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.8.dfsg-2ubuntu4.3
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.8.dfsg-2ubuntu4.3.dsc' zlib_1.2.8.dfsg-2ubuntu4.3.dsc 2535 SHA256:d0e23d3bf4b5062bbb929e4e78639ded99129dbfeca9fb735c5d2390b1f9c398
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.8.dfsg.orig.tar.gz' zlib_1.2.8.dfsg.orig.tar.gz 361943 SHA256:2caecc2c3f1ef8b87b8f72b128a03e61c307e8c14f5ec9b422ef7914ba75cf9f
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.8.dfsg-2ubuntu4.3.debian.tar.xz' zlib_1.2.8.dfsg-2ubuntu4.3.debian.tar.xz 19128 SHA256:25a6dda8dd5fad7c5927e43b815056335e27e7a1a552b5d8e5a4d5b4f9a9ce8f
```
