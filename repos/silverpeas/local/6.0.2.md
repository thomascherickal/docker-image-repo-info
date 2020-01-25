# `silverpeas:6.0.2`

## Docker Metadata

- Image ID: `sha256:79b6eaa9a7c3c1d29b7369524a5ce9e88aeffb164d2598b61334da448708c594`
- Created: `2020-01-16T03:01:05.583062417Z`
- Virtual Size: ~ 1.54 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["/opt/run.sh"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `TERM=xterm`
  - `LANG=en_US.UTF-8`
  - `LANGUAGE=en_US.UTF-8`
  - `LC_ALL=en_US.UTF-8`
  - `JAVA_HOME=/docker-java-home`
  - `SILVERPEAS_HOME=/opt/silverpeas`
  - `JBOSS_HOME=/opt/wildfly`
  - `SILVERPEAS_VERSION=6.0.2`
  - `WILDFLY_VERSION=10.1.0`
- Labels:
  - `build=1`
  - `description=Image to install and to run Silverpeas 6`
  - `name=Silverpeas 6`
  - `vendor=Silverpeas`
  - `version=6.0.2`

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

### `dpkg` source package: `alsa-lib=1.1.0-0ubuntu1`

Binary Packages:

- `libasound2:amd64=1.1.0-0ubuntu1`
- `libasound2-data=1.1.0-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libasound2/copyright`, `/usr/share/doc/libasound2-data/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris alsa-lib=1.1.0-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/alsa-lib/alsa-lib_1.1.0-0ubuntu1.dsc' alsa-lib_1.1.0-0ubuntu1.dsc 1894 SHA256:17f7b1432cd6b2b1f5573658d42744fe7adeafd5aad482c9ee0be30869ef27f7
'http://archive.ubuntu.com/ubuntu/pool/main/a/alsa-lib/alsa-lib_1.1.0.orig.tar.bz2' alsa-lib_1.1.0.orig.tar.bz2 929874 SHA256:dfde65d11e82b68f82e562ab6228c1fb7c78854345d3c57e2c68a9dd3dae1f15
'http://archive.ubuntu.com/ubuntu/pool/main/a/alsa-lib/alsa-lib_1.1.0-0ubuntu1.debian.tar.xz' alsa-lib_1.1.0-0ubuntu1.debian.tar.xz 53828 SHA256:216445e0a62424c36080e4ef7eca6ad5c4bfe12f1258e52c1d98e53d212efac3
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

### `dpkg` source package: `apt=1.2.32`

Binary Packages:

- `apt=1.2.32`
- `libapt-pkg5.0:amd64=1.2.32`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg5.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=1.2.32
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.2.32.dsc' apt_1.2.32.dsc 2432 SHA256:9202ffff0487cfbf57f3adb052d81e591cf0fd6ba44dfcc56b7500e91c2d4688
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_1.2.32.tar.xz' apt_1.2.32.tar.xz 2084344 SHA256:0c7044bd3eafed199d32e72af476f8c6305962918348aa3593d6d5aa301f7431
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

Source:

```console
$ apt-get source -qq --print-uris base-files=9.4ubuntu4.11
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_9.4ubuntu4.11.dsc' base-files_9.4ubuntu4.11.dsc 1575 SHA256:916072c008683dbd6468e04ad140eab668d9e511c888836f4280d0434b8ed065
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_9.4ubuntu4.11.tar.xz' base-files_9.4ubuntu4.11.tar.xz 65368 SHA256:0e65fae9f9d964c2d0539b79f2fa10591f9ca96a9e415828dc58560dfd97b92a
```

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

### `dpkg` source package: `bzip2=1.0.6-8ubuntu0.2`

Binary Packages:

- `libbz2-1.0:amd64=1.0.6-8ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libbz2-1.0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.6-8ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8ubuntu0.2.dsc' bzip2_1.0.6-8ubuntu0.2.dsc 2173 SHA256:0afaa6cd738938e3e66814722960785a37b5e96ea68f27a99eb5fb52dfd763e8
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6.orig.tar.bz2' bzip2_1.0.6.orig.tar.bz2 708737 SHA256:d70a9ccd8bdf47e302d96c69fecd54925f45d9c7b966bb4ef5f56b770960afa7
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.6-8ubuntu0.2.debian.tar.bz2' bzip2_1.0.6-8ubuntu0.2.debian.tar.bz2 61599 SHA256:df33ff2757f888545ecb2b0a53ade6cc697aa664ebd70e664674cdd3c2dd26df
```

### `dpkg` source package: `ca-certificates-java=20160321ubuntu1`

Binary Packages:

- `ca-certificates-java=20160321ubuntu1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates-java/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates-java=20160321ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates-java/ca-certificates-java_20160321ubuntu1.dsc' ca-certificates-java_20160321ubuntu1.dsc 1855 SHA256:268a8579b394587144c42c3e06e0ed6fc9cb4877c7545577e389fdb639517b95
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates-java/ca-certificates-java_20160321ubuntu1.tar.xz' ca-certificates-java_20160321ubuntu1.tar.xz 15928 SHA256:1b7e1207135713d81844fe9c13e282262a1d0472901b823516d71452d63ce752
```

### `dpkg` source package: `ca-certificates=20170717~16.04.2`

Binary Packages:

- `ca-certificates=20170717~16.04.2`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20170717~16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20170717~16.04.2.dsc' ca-certificates_20170717~16.04.2.dsc 1969 SHA256:0b6e1f7a5d2ae31e0c6729df25bfd008286ebcdd53cfd5d3b395b9e80be3d3f1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20170717~16.04.2.tar.xz' ca-certificates_20170717~16.04.2.tar.xz 293084 SHA256:57f7083062f4318a4d1cb6a020df5ef0b245aa0755b9e6468aa44500e5798567
```

### `dpkg` source package: `cairo=1.14.6-1`

Binary Packages:

- `libcairo2:amd64=1.14.6-1`

Licenses: (parsed from: `/usr/share/doc/libcairo2/copyright`)

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

### `dpkg` source package: `crystalhd=1:0.0~git20110715.fdd2f19-11build1`

Binary Packages:

- `libcrystalhd3:amd64=1:0.0~git20110715.fdd2f19-11build1`

Licenses: (parsed from: `/usr/share/doc/libcrystalhd3/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris crystalhd=1:0.0~git20110715.fdd2f19-11build1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-11build1.dsc' crystalhd_0.0~git20110715.fdd2f19-11build1.dsc 1726 SHA256:27c571228db5639c2c97c787e73ca65f37d3ecd856c664b5edbb559755af57fa
'http://archive.ubuntu.com/ubuntu/pool/universe/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz' crystalhd_0.0~git20110715.fdd2f19.orig.tar.gz 1186072 SHA256:a1c22908b85085dcc4591bc033fe054be63eab59b7d35f0a9ab3fcb2600722b7
'http://archive.ubuntu.com/ubuntu/pool/universe/c/crystalhd/crystalhd_0.0~git20110715.fdd2f19-11build1.debian.tar.xz' crystalhd_0.0~git20110715.fdd2f19-11build1.debian.tar.xz 15240 SHA256:646168058a9a41b20a392fe20f7a2a88caaa1a42fc3e002635c33f0cf129ed0f
```

### `dpkg` source package: `cups-filters=1.8.3-2ubuntu3.5`

Binary Packages:

- `libcupsfilters1:amd64=1.8.3-2ubuntu3.5`

Licenses: (parsed from: `/usr/share/doc/libcupsfilters1/copyright`)

- `BSD-4-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris cups-filters=1.8.3-2ubuntu3.5
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups-filters/cups-filters_1.8.3-2ubuntu3.5.dsc' cups-filters_1.8.3-2ubuntu3.5.dsc 3029 SHA256:0f3a9bc4cfa1409d46ca2e62d86629b8a9c3a99bc6b8620cfb06c879c687fc2f
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups-filters/cups-filters_1.8.3.orig.tar.xz' cups-filters_1.8.3.orig.tar.xz 1373028 SHA256:e1e786f1fbcd3a203d87ebb4106a0ba8d579953cbe22056d12d4ee8143f5341a
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups-filters/cups-filters_1.8.3-2ubuntu3.5.debian.tar.xz' cups-filters_1.8.3-2ubuntu3.5.debian.tar.xz 71656 SHA256:7b85746df6e7caf21cf344ffe3afeb3171b5d199dbf90811c8ed86e17564f64d
```

### `dpkg` source package: `cups=2.1.3-4ubuntu0.10`

Binary Packages:

- `libcups2:amd64=2.1.3-4ubuntu0.10`
- `libcupsimage2:amd64=2.1.3-4ubuntu0.10`

Licenses: (parsed from: `/usr/share/doc/libcups2/copyright`, `/usr/share/doc/libcupsimage2/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2.0 with AOSDL exception`
- `LGPL-2`
- `LGPL-2.0 with AOSDL exception`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris cups=2.1.3-4ubuntu0.10
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3-4ubuntu0.10.dsc' cups_2.1.3-4ubuntu0.10.dsc 3447 SHA256:300c90232b7ca024674df4b48ac3a981ff3ce5efab5a778037bb31c1de34e6b9
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3.orig.tar.bz2' cups_2.1.3.orig.tar.bz2 8832400 SHA256:36a70d43584aea2617da914b9331e23341c3501a8254c4d2eae9c11ec01fd4d3
'http://archive.ubuntu.com/ubuntu/pool/main/c/cups/cups_2.1.3-4ubuntu0.10.debian.tar.xz' cups_2.1.3-4ubuntu0.10.debian.tar.xz 357260 SHA256:4b66b60cf4be4e279268f1361f803fda3b8ae2510b58256a0f0032cfc48ebf7d
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

### `dpkg` source package: `db5.3=5.3.28-11ubuntu0.2`

Binary Packages:

- `libdb5.3:amd64=5.3.28-11ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28-11ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-11ubuntu0.2.dsc' db5.3_5.3.28-11ubuntu0.2.dsc 3182 SHA256:cfb1c1fcd31bbbabe8b9fbea0fb0755091c1d5f4f745626342a46eea1448b066
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28.orig.tar.xz' db5.3_5.3.28.orig.tar.xz 24154920 SHA256:e1f85c8b6ebd0ed3ca72fa0ae97b65006f6d0bd0cd6f4ac24bed103cb5497bf5
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28-11ubuntu0.2.debian.tar.xz' db5.3_5.3.28-11ubuntu0.2.debian.tar.xz 29312 SHA256:01f2cd8d0eda0f2b48b1aef7cb3babe94ecd14b1955de437b61e04f7b72bdd0c
```

### `dpkg` source package: `dbus=1.10.6-1ubuntu3.5`

Binary Packages:

- `dbus=1.10.6-1ubuntu3.5`
- `libdbus-1-3:amd64=1.10.6-1ubuntu3.5`

Licenses: (parsed from: `/usr/share/doc/dbus/copyright`, `/usr/share/doc/libdbus-1-3/copyright`)

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
$ apt-get source -qq --print-uris dbus=1.10.6-1ubuntu3.5
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6-1ubuntu3.5.dsc' dbus_1.10.6-1ubuntu3.5.dsc 3164 SHA256:781a42ed620bca22c3c34a2277354292392188fb23d5efacd9cfa1fd0583386c
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6.orig.tar.gz' dbus_1.10.6.orig.tar.gz 1952608 SHA256:b5fefa08a77edd76cd64d872db949eebc02cf6f3f8be82e4bbc641742af5d35f
'http://archive.ubuntu.com/ubuntu/pool/main/d/dbus/dbus_1.10.6-1ubuntu3.5.debian.tar.xz' dbus_1.10.6-1ubuntu3.5.debian.tar.xz 65116 SHA256:2ce01c691a1df555cd27889e8016b7bdd55b17bf398f9796e8e45c0eee36d605
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

- `libdjvulibre-text=3.5.27.1-5ubuntu0.1`
- `libdjvulibre21:amd64=3.5.27.1-5ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libdjvulibre-text/copyright`, `/usr/share/doc/libdjvulibre21/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

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

### `dpkg` source package: `e2fsprogs=1.42.13-1ubuntu1.1`

Binary Packages:

- `e2fslibs:amd64=1.42.13-1ubuntu1.1`
- `e2fsprogs=1.42.13-1ubuntu1.1`
- `libcomerr2:amd64=1.42.13-1ubuntu1.1`
- `libss2:amd64=1.42.13-1ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/e2fslibs/copyright`, `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcomerr2/copyright`, `/usr/share/doc/libss2/copyright`)

- `GPL-2`
- `LGPL-2`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris expat=2.1.0-7ubuntu0.16.04.5
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0-7ubuntu0.16.04.5.dsc' expat_2.1.0-7ubuntu0.16.04.5.dsc 2387 SHA256:39c54dc2f9fa64fe3d1b2d216e0446de8dc37d2656a5597a8b344070ce2310e2
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0.orig.tar.gz' expat_2.1.0.orig.tar.gz 562616 SHA256:823705472f816df21c8f6aa026dd162b280806838bb55b3432b0fb1fcca7eb86
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.1.0-7ubuntu0.16.04.5.debian.tar.xz' expat_2.1.0-7ubuntu0.16.04.5.debian.tar.xz 23116 SHA256:f422e05965440e42c030904fc6605c39cb5477c114ac7b172427ce96d63e97e0
```

### `dpkg` source package: `ffmpeg=7:2.8.15-0ubuntu0.16.04.1`

Binary Packages:

- `ffmpeg=7:2.8.15-0ubuntu0.16.04.1`
- `libavcodec-ffmpeg56:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libavdevice-ffmpeg56:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libavfilter-ffmpeg5:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libavformat-ffmpeg56:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libavresample-ffmpeg2:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libavutil-ffmpeg54:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libpostproc-ffmpeg53:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libswresample-ffmpeg1:amd64=7:2.8.15-0ubuntu0.16.04.1`
- `libswscale-ffmpeg3:amd64=7:2.8.15-0ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/ffmpeg/copyright`, `/usr/share/doc/libavcodec-ffmpeg56/copyright`, `/usr/share/doc/libavdevice-ffmpeg56/copyright`, `/usr/share/doc/libavfilter-ffmpeg5/copyright`, `/usr/share/doc/libavformat-ffmpeg56/copyright`, `/usr/share/doc/libavresample-ffmpeg2/copyright`, `/usr/share/doc/libavutil-ffmpeg54/copyright`, `/usr/share/doc/libpostproc-ffmpeg53/copyright`, `/usr/share/doc/libswresample-ffmpeg1/copyright`, `/usr/share/doc/libswscale-ffmpeg3/copyright`)

- `BSD-1-Clause`
- `BSD-3-Clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Avisynth exception`
- `GPL-3`
- `GPL-3+`
- `IJG`
- `ISC`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Sundry`
- `Zlib`
- `man-page`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris ffmpeg=7:2.8.15-0ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/universe/f/ffmpeg/ffmpeg_2.8.15-0ubuntu0.16.04.1.dsc' ffmpeg_2.8.15-0ubuntu0.16.04.1.dsc 4893 SHA256:31fd066a28260e4cf6be48f941362ba5b9037ae3d65a78a655c1d60ea1c2dabf
'http://archive.ubuntu.com/ubuntu/pool/universe/f/ffmpeg/ffmpeg_2.8.15.orig.tar.xz' ffmpeg_2.8.15.orig.tar.xz 7228272 SHA256:7b5c0e60fb889fd52ce17a4ab653a2916ad13cbe5b31125876cbf5eaec5ebd18
'http://archive.ubuntu.com/ubuntu/pool/universe/f/ffmpeg/ffmpeg_2.8.15-0ubuntu0.16.04.1.debian.tar.xz' ffmpeg_2.8.15-0ubuntu0.16.04.1.debian.tar.xz 44272 SHA256:64c1f1a71d301321fe2b101b81423b05e552f6bd683743354b9159bd73f1ce5b
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

### `dpkg` source package: `flac=1.3.1-4`

Binary Packages:

- `libflac8:amd64=1.3.1-4`

Licenses: (parsed from: `/usr/share/doc/libflac8/copyright`)

- `BSD-3-clause`
- `GFDL-1.1+`
- `GFDL-1.2`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Public-domain`

Source:

```console
$ apt-get source -qq --print-uris flac=1.3.1-4
'http://archive.ubuntu.com/ubuntu/pool/main/f/flac/flac_1.3.1-4.dsc' flac_1.3.1-4.dsc 2261 SHA256:271adf092634f74eb21d13f0cd02cee14e8c3415b7a23287821a27bb9b1f88b1
'http://archive.ubuntu.com/ubuntu/pool/main/f/flac/flac_1.3.1.orig.tar.xz' flac_1.3.1.orig.tar.xz 941848 SHA256:4773c0099dba767d963fd92143263be338c48702172e8754b9bc5103efe1c56c
'http://archive.ubuntu.com/ubuntu/pool/main/f/flac/flac_1.3.1-4.debian.tar.xz' flac_1.3.1-4.debian.tar.xz 17604 SHA256:68f5e3954876ef78ca60ea126a9e3b9525c2720e1ccf4a88389341e340094d1f
```

### `dpkg` source package: `flite=2.0.0-release-1`

Binary Packages:

- `libflite1:amd64=2.0.0-release-1`

Licenses: (parsed from: `/usr/share/doc/libflite1/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris flite=2.0.0-release-1
'http://archive.ubuntu.com/ubuntu/pool/universe/f/flite/flite_2.0.0-release-1.dsc' flite_2.0.0-release-1.dsc 2243 SHA256:00ffa92806775857ed2cc151f584d212aff7ff4dd9c3342ce74539f00db73731
'http://archive.ubuntu.com/ubuntu/pool/universe/f/flite/flite_2.0.0-release.orig.tar.bz2' flite_2.0.0-release.orig.tar.bz2 14761376 SHA256:678c3860fd539402b5d1699b921239072af6acb4e72dc4720494112807cae411
'http://archive.ubuntu.com/ubuntu/pool/universe/f/flite/flite_2.0.0-release-1.debian.tar.xz' flite_2.0.0-release-1.debian.tar.xz 30220 SHA256:70a9a88aa9d6fd6b0836b22bf5c7ee456e8c5f62a62f8edf60ca557ff10933c5
```

### `dpkg` source package: `fontconfig=2.11.94-0ubuntu1.1`

Binary Packages:

- `fontconfig=2.11.94-0ubuntu1.1`
- `fontconfig-config=2.11.94-0ubuntu1.1`
- `libfontconfig1:amd64=2.11.94-0ubuntu1.1`

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
- `fonts-dejavu-extra=2.35-1`

Licenses: (parsed from: `/usr/share/doc/fonts-dejavu-core/copyright`, `/usr/share/doc/fonts-dejavu-extra/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/libfreetype6/copyright`)

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

### `dpkg` source package: `fribidi=0.19.7-1`

Binary Packages:

- `libfribidi0:amd64=0.19.7-1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=0.19.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_0.19.7-1.dsc' fribidi_0.19.7-1.dsc 1875 SHA256:28787312e2725fa24fc6fd5b7dcdbd77228d9f0767b5bea3f0741cec75c4169b
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_0.19.7.orig.tar.bz2' fribidi_0.19.7.orig.tar.bz2 648299 SHA256:08222a6212bbc2276a2d55c3bf370109ae4a35b689acbc66571ad2a670595a8e
'http://archive.ubuntu.com/ubuntu/pool/main/f/fribidi/fribidi_0.19.7-1.debian.tar.xz' fribidi_0.19.7-1.debian.tar.xz 7428 SHA256:05bba0f9eae7836c033ffd5674491bdac703ef69640dbd3eb029307d7420462e
```

### `dpkg` source package: `game-music-emu=0.6.0-3ubuntu0.16.04.1`

Binary Packages:

- `libgme0:amd64=0.6.0-3ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libgme0/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris game-music-emu=0.6.0-3ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/universe/g/game-music-emu/game-music-emu_0.6.0-3ubuntu0.16.04.1.dsc' game-music-emu_0.6.0-3ubuntu0.16.04.1.dsc 1979 SHA256:60b0d55f1a9252a86e6350e8c99741282ded1aa50d850f40ef08784cab69f08f
'http://archive.ubuntu.com/ubuntu/pool/universe/g/game-music-emu/game-music-emu_0.6.0.orig.tar.bz2' game-music-emu_0.6.0.orig.tar.bz2 170202 SHA256:506e81d0c61e1a26d503fbf5351503e0b31f9fbb374cb1f09979758b46a24987
'http://archive.ubuntu.com/ubuntu/pool/universe/g/game-music-emu/game-music-emu_0.6.0-3ubuntu0.16.04.1.debian.tar.xz' game-music-emu_0.6.0-3ubuntu0.16.04.1.debian.tar.xz 5592 SHA256:a4d7a4f5d9df23098abc4c1fe82696ed8f93d893c50bb8fc14a4de84e705810d
```

### `dpkg` source package: `gcc-5=5.4.0-6ubuntu1~16.04.12`

Binary Packages:

- `gcc-5-base:amd64=5.4.0-6ubuntu1~16.04.12`
- `libgomp1:amd64=5.4.0-6ubuntu1~16.04.12`
- `libstdc++6:amd64=5.4.0-6ubuntu1~16.04.12`

Licenses: (parsed from: `/usr/share/doc/gcc-5-base/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

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

### `dpkg` source package: `gdk-pixbuf=2.32.2-1ubuntu1.6`

Binary Packages:

- `libgdk-pixbuf2.0-0:amd64=2.32.2-1ubuntu1.6`
- `libgdk-pixbuf2.0-common=2.32.2-1ubuntu1.6`

Licenses: (parsed from: `/usr/share/doc/libgdk-pixbuf2.0-0/copyright`, `/usr/share/doc/libgdk-pixbuf2.0-common/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris gdk-pixbuf=2.32.2-1ubuntu1.6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2-1ubuntu1.6.dsc' gdk-pixbuf_2.32.2-1ubuntu1.6.dsc 2912 SHA256:ada3327bb6913d7056cd8de4360d3cbc359ca04e526337d406e4cef3ab640965
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2.orig.tar.xz' gdk-pixbuf_2.32.2.orig.tar.xz 2429268 SHA256:d3ab06fc123b13effed4c27c77cebdfad2173ff20628d82c397b7660ae926145
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdk-pixbuf/gdk-pixbuf_2.32.2-1ubuntu1.6.debian.tar.xz' gdk-pixbuf_2.32.2-1ubuntu1.6.debian.tar.xz 19956 SHA256:89b307e6007e8acec4038bdc994c81d36f3371d3ea5ccc2877d697cb0a6c445b
```

### `dpkg` source package: `ghostscript=9.26~dfsg+0-0ubuntu0.16.04.12`

Binary Packages:

- `ghostscript=9.26~dfsg+0-0ubuntu0.16.04.12`
- `libgs9:amd64=9.26~dfsg+0-0ubuntu0.16.04.12`
- `libgs9-common=9.26~dfsg+0-0ubuntu0.16.04.12`

Licenses: (parsed from: `/usr/share/doc/ghostscript/copyright`, `/usr/share/doc/libgs9/copyright`, `/usr/share/doc/libgs9-common/copyright`)

- `AGPL-3`
- `AGPL-3+`
- `AGPL-3+ with font exception`
- `Apache-2.0`
- `BSD-2-Clause`
- `BSD-3-Clause`
- `BSD-3-Clause~Adobe`
- `Expat`
- `Expat~Ghostgum`
- `Expat~SunSoft`
- `Expat~SunSoft with SunSoft exception`
- `FTL`
- `GAP~configure`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `LGPL-2.1`
- `NTP~Lucent`
- `NTP~Open`
- `NTP~WSU`
- `ZLIB`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris ghostscript=9.26~dfsg+0-0ubuntu0.16.04.12
'http://archive.ubuntu.com/ubuntu/pool/main/g/ghostscript/ghostscript_9.26~dfsg+0-0ubuntu0.16.04.12.dsc' ghostscript_9.26~dfsg+0-0ubuntu0.16.04.12.dsc 2930 SHA256:ddf8d72b36c9656432c0908b8f3be7aabc72f44151ecd2a85079ccce928bed75
'http://archive.ubuntu.com/ubuntu/pool/main/g/ghostscript/ghostscript_9.26~dfsg+0.orig.tar.xz' ghostscript_9.26~dfsg+0.orig.tar.xz 27040868 SHA256:f13dd2be0499ae47f508d66be4f7a61056674c2ee6ff53d954e84bc634986bd7
'http://archive.ubuntu.com/ubuntu/pool/main/g/ghostscript/ghostscript_9.26~dfsg+0-0ubuntu0.16.04.12.debian.tar.xz' ghostscript_9.26~dfsg+0-0ubuntu0.16.04.12.debian.tar.xz 148768 SHA256:ba69fab2e0c40472a6e680908cd5c3df4b0e729c30e85a4092b26701ea8f914c
```

### `dpkg` source package: `giflib=5.1.4-0.3~16.04.1`

Binary Packages:

- `libgif7:amd64=5.1.4-0.3~16.04.1`

Licenses: (parsed from: `/usr/share/doc/libgif7/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris giflib=5.1.4-0.3~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/giflib/giflib_5.1.4-0.3~16.04.1.dsc' giflib_5.1.4-0.3~16.04.1.dsc 2084 SHA256:d631249bbc42a60620d43a2758ebdd3f3b32039d1b1e5db3839e6b83d924eae4
'http://archive.ubuntu.com/ubuntu/pool/main/g/giflib/giflib_5.1.4.orig.tar.bz2' giflib_5.1.4.orig.tar.bz2 639703 SHA256:df27ec3ff24671f80b29e6ab1c4971059c14ac3db95406884fc26574631ba8d5
'http://archive.ubuntu.com/ubuntu/pool/main/g/giflib/giflib_5.1.4-0.3~16.04.1.debian.tar.xz' giflib_5.1.4-0.3~16.04.1.debian.tar.xz 13776 SHA256:ac5c0c006a616baefa10e06dbc6c896f192746e8b46df7392071337c78fffc3f
```

### `dpkg` source package: `glib2.0=2.48.2-0ubuntu4.4`

Binary Packages:

- `libglib2.0-0:amd64=2.48.2-0ubuntu4.4`
- `libglib2.0-data=2.48.2-0ubuntu4.4`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`, `/usr/share/doc/libglib2.0-data/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.48.2-0ubuntu4.4
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2-0ubuntu4.4.dsc' glib2.0_2.48.2-0ubuntu4.4.dsc 3157 SHA256:634120712a9b8c88e44cc5fdb0088a7006f667f7d74859aca494057e01c95a13
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2.orig.tar.xz' glib2.0_2.48.2.orig.tar.xz 6408644 SHA256:f25e751589cb1a58826eac24fbd4186cda4518af772806b666a3f91f66e6d3f4
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.48.2-0ubuntu4.4.debian.tar.xz' glib2.0_2.48.2-0ubuntu4.4.debian.tar.xz 73724 SHA256:0b1544430db9b73d49dfb25e77d6223cc1afe2f296b5db31ad493ea47877183e
```

### `dpkg` source package: `glibc=2.23-0ubuntu11`

Binary Packages:

- `libc-bin=2.23-0ubuntu11`
- `libc6:amd64=2.23-0ubuntu11`
- `locales=2.23-0ubuntu11`
- `multiarch-support=2.23-0ubuntu11`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/locales/copyright`, `/usr/share/doc/multiarch-support/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.23-0ubuntu11
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23-0ubuntu11.dsc' glibc_2.23-0ubuntu11.dsc 8568 SHA256:2c45454af949b7c8d211c09925e4cd5282b40c14048b67dbfec6b394bb6e9828
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23.orig.tar.xz' glibc_2.23.orig.tar.xz 13849968 SHA256:bf6c528eeebefcacc295270068b79330c1fb2b22458ff66285b4175d23442c96
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.23-0ubuntu11.debian.tar.xz' glibc_2.23-0ubuntu11.debian.tar.xz 1246096 SHA256:fcaea11240f3eb24c28420f0bb7a48409da99939be6e1a5ed1479ed4ad1273db
```

### `dpkg` source package: `gmp=2:6.1.0+dfsg-2`

Binary Packages:

- `libgmp10:amd64=2:6.1.0+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

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

### `dpkg` source package: `gnutls28=3.4.10-4ubuntu1.6`

Binary Packages:

- `libgnutls30:amd64=3.4.10-4ubuntu1.6`

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

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


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

### `dpkg` source package: `gsfonts=1:8.11+urwcyr1.0.7~pre44-4.2ubuntu1`

Binary Packages:

- `gsfonts=1:8.11+urwcyr1.0.7~pre44-4.2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gsfonts/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gsfonts=1:8.11+urwcyr1.0.7~pre44-4.2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsfonts/gsfonts_8.11+urwcyr1.0.7~pre44-4.2ubuntu1.dsc' gsfonts_8.11+urwcyr1.0.7~pre44-4.2ubuntu1.dsc 1334 SHA256:9e8008d3e1ee4aee68bfdfa08e9eb1d0c804ece7f3bf5d1d81c3739dec6064fa
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsfonts/gsfonts_8.11+urwcyr1.0.7~pre44.orig.tar.gz' gsfonts_8.11+urwcyr1.0.7~pre44.orig.tar.gz 3390551 SHA256:9f2a598998bf05e023546ac981aa2a857aa1635d2e0e3020a3c3004ad564dc00
'http://archive.ubuntu.com/ubuntu/pool/main/g/gsfonts/gsfonts_8.11+urwcyr1.0.7~pre44-4.2ubuntu1.diff.gz' gsfonts_8.11+urwcyr1.0.7~pre44-4.2ubuntu1.diff.gz 6877 SHA256:205ad64e8ad77f14a1c3724c65db06dde6c78e8610b750839b6c71b0e8c64076
```

### `dpkg` source package: `gtk+2.0=2.24.30-1ubuntu1.16.04.2`

Binary Packages:

- `libgtk2.0-0:amd64=2.24.30-1ubuntu1.16.04.2`
- `libgtk2.0-bin=2.24.30-1ubuntu1.16.04.2`
- `libgtk2.0-common=2.24.30-1ubuntu1.16.04.2`

Licenses: (parsed from: `/usr/share/doc/libgtk2.0-0/copyright`, `/usr/share/doc/libgtk2.0-bin/copyright`, `/usr/share/doc/libgtk2.0-common/copyright`)

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

### `dpkg` source package: `icu=55.1-7ubuntu0.4`

Binary Packages:

- `libicu55:amd64=55.1-7ubuntu0.4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=55.1-7ubuntu0.4
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1-7ubuntu0.4.dsc' icu_55.1-7ubuntu0.4.dsc 2130 SHA256:2acd6485f45d74747a3b47278e129be2d827d97d2a91a8d32d099a65deac7a18
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1.orig.tar.gz' icu_55.1.orig.tar.gz 25600847 SHA256:e16b22cbefdd354bec114541f7849a12f8fc2015320ca5282ee4fd787571457b
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_55.1-7ubuntu0.4.debian.tar.xz' icu_55.1-7ubuntu0.4.debian.tar.xz 31856 SHA256:dbdafcb148992e087b8495855421f515c90a7c40d3286b5d861a5afa9fcc562e
```

### `dpkg` source package: `ijs=0.35-12`

Binary Packages:

- `libijs-0.35:amd64=0.35-12`

Licenses: (parsed from: `/usr/share/doc/libijs-0.35/copyright`)

- `Expat`
- `Expat~X`
- `Expat~X with X exception`
- `GAP`
- `GAP~Makefile.in`
- `GAP~configure`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`

Source:

```console
$ apt-get source -qq --print-uris ijs=0.35-12
'http://archive.ubuntu.com/ubuntu/pool/main/i/ijs/ijs_0.35-12.dsc' ijs_0.35-12.dsc 1912 SHA256:e61103c05c58a623430262e7f7678899e23dd320b9ad0a931b6e8de143706a96
'http://archive.ubuntu.com/ubuntu/pool/main/i/ijs/ijs_0.35.orig.tar.gz' ijs_0.35.orig.tar.gz 344262 SHA256:901fffb73e42dae343a8285a31d9c4e82dc3856d36be30adbdb564bdd27161d6
'http://archive.ubuntu.com/ubuntu/pool/main/i/ijs/ijs_0.35-12.debian.tar.xz' ijs_0.35-12.debian.tar.xz 7812 SHA256:1007ae4f8dbabab90b2d2acf234031260bba26a05c2f31be822e63e27907e8ac
```

### `dpkg` source package: `ilmbase=2.2.0-11ubuntu2`

Binary Packages:

- `libilmbase12:amd64=2.2.0-11ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libilmbase12/copyright`)

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
- `libmagickcore-6.q16-2:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickcore-6.q16-2-extra:amd64=8:6.8.9.9-7ubuntu5.15`
- `libmagickwand-6.q16-2:amd64=8:6.8.9.9-7ubuntu5.15`

Licenses: (parsed from: `/usr/share/doc/imagemagick/copyright`, `/usr/share/doc/imagemagick-6.q16/copyright`, `/usr/share/doc/imagemagick-common/copyright`, `/usr/share/doc/libmagickcore-6.q16-2/copyright`, `/usr/share/doc/libmagickcore-6.q16-2-extra/copyright`, `/usr/share/doc/libmagickwand-6.q16-2/copyright`)

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

### `dpkg` source package: `intel-vaapi-driver=1.7.0-1`

Binary Packages:

- `i965-va-driver:amd64=1.7.0-1`

Licenses: (parsed from: `/usr/share/doc/i965-va-driver/copyright`)

- `Apache-2.0`
- `EPL-1.0`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris intel-vaapi-driver=1.7.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/i/intel-vaapi-driver/intel-vaapi-driver_1.7.0-1.dsc' intel-vaapi-driver_1.7.0-1.dsc 2434 SHA256:78bfa858e3266fb81062f9d8ec5e9662877bffd9adcb1864f25aea824558367f
'http://archive.ubuntu.com/ubuntu/pool/universe/i/intel-vaapi-driver/intel-vaapi-driver_1.7.0.orig.tar.bz2' intel-vaapi-driver_1.7.0.orig.tar.bz2 1114349 SHA256:9d19d6c789a9a4fbce23c4f0eaf993ba776b512bec4c87982ab17ac841435c0c
'http://archive.ubuntu.com/ubuntu/pool/universe/i/intel-vaapi-driver/intel-vaapi-driver_1.7.0-1.debian.tar.xz' intel-vaapi-driver_1.7.0-1.debian.tar.xz 10192 SHA256:0c2903043dcfb455d77549d99bd3fbff73084f257f39c84e52e6fddbf60df640
```

### `dpkg` source package: `jackd2=1.9.10+20150825git1ed50c92~dfsg-1ubuntu1`

Binary Packages:

- `libjack-jackd2-0:amd64=1.9.10+20150825git1ed50c92~dfsg-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libjack-jackd2-0/copyright`)

- `BSD-3-clause`
- `Expat`
- `Expat~modrequest`
- `GPL-2`
- `GPL-2+`
- `GPL-2~either`
- `GPL-2~jack-audio-connection-kit`
- `GPL-2~jackd2`
- `GPL-2~or`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `None`
- `public-domain~Kroon`

Source:

```console
$ apt-get source -qq --print-uris jackd2=1.9.10+20150825git1ed50c92~dfsg-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jackd2/jackd2_1.9.10+20150825git1ed50c92~dfsg-1ubuntu1.dsc' jackd2_1.9.10+20150825git1ed50c92~dfsg-1ubuntu1.dsc 2757 SHA256:cd1ec18ef1122f57e1a4b1c009d3256c27879f697332e19976de4f97f2772169
'http://archive.ubuntu.com/ubuntu/pool/main/j/jackd2/jackd2_1.9.10+20150825git1ed50c92~dfsg.orig.tar.gz' jackd2_1.9.10+20150825git1ed50c92~dfsg.orig.tar.gz 1323432 SHA256:7127ecc608775de8f47ea4f88f1ad75b17eb660745236e2cad3e14d8b98fe791
'http://archive.ubuntu.com/ubuntu/pool/main/j/jackd2/jackd2_1.9.10+20150825git1ed50c92~dfsg-1ubuntu1.debian.tar.xz' jackd2_1.9.10+20150825git1ed50c92~dfsg-1ubuntu1.debian.tar.xz 39608 SHA256:fa6cbe2bdd3ab174134e283c25bd4d8d094bb4952df6640cd38ab133205059c3
```

### `dpkg` source package: `java-common=0.56ubuntu2`

Binary Packages:

- `java-common=0.56ubuntu2`

Licenses: (parsed from: `/usr/share/doc/java-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris java-common=0.56ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/j/java-common/java-common_0.56ubuntu2.dsc' java-common_0.56ubuntu2.dsc 2153 SHA256:349237f0b15050c63a1538d235b5d49245b215f7be64d9071de09d02c0f19b1a
'http://archive.ubuntu.com/ubuntu/pool/main/j/java-common/java-common_0.56ubuntu2.tar.xz' java-common_0.56ubuntu2.tar.xz 12964 SHA256:4d408728bf10a660c82225bb372888f133f74cdcc86060a725fde6f735c85e6f
```

### `dpkg` source package: `jbig2dec=0.12+20150918-1ubuntu0.1`

Binary Packages:

- `libjbig2dec0=0.12+20150918-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libjbig2dec0/copyright`)

- `AGPL-3`
- `AGPL-3+`
- `BSD-2-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `pubic-domain`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris jbig2dec=0.12+20150918-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbig2dec/jbig2dec_0.12+20150918-1ubuntu0.1.dsc' jbig2dec_0.12+20150918-1ubuntu0.1.dsc 2285 SHA256:01d2d1347032873608acf0c368049dd6eda5f7767ee79a3d37db9ae8c0376d42
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbig2dec/jbig2dec_0.12+20150918.orig.tar.gz' jbig2dec_0.12+20150918.orig.tar.gz 122563 SHA256:b40605876d15b400886c1597d3e78f9cd32c33548b3230ed0c44303bc9a345fa
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbig2dec/jbig2dec_0.12+20150918-1ubuntu0.1.debian.tar.xz' jbig2dec_0.12+20150918-1ubuntu0.1.debian.tar.xz 26380 SHA256:2f354037ea63c0c895fa0fac233d53201c61346431067137a5159da7c4ab6c66
```

### `dpkg` source package: `jbigkit=2.1-3.1`

Binary Packages:

- `libjbig0:amd64=2.1-3.1`

Licenses: (parsed from: `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1.dsc' jbigkit_2.1-3.1.dsc 1299 SHA256:62c8812d508958c5d35f2b1579dc3052fb5bd8d2e77d023fad064c4b48c8c3f8
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://archive.ubuntu.com/ubuntu/pool/main/j/jbigkit/jbigkit_2.1-3.1.debian.tar.xz' jbigkit_2.1-3.1.debian.tar.xz 7600 SHA256:ebc3c52deaf37d52baea54d648a713640dc262926abda7bf05cd08e7db5dd1ee
```

### `dpkg` source package: `json-c=0.11-4ubuntu2`

Binary Packages:

- `libjson-c2:amd64=0.11-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libjson-c2/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris json-c=0.11-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-c/json-c_0.11-4ubuntu2.dsc' json-c_0.11-4ubuntu2.dsc 1639 SHA256:2e2a6fd9a8d87e6efd5a0fe3ed2a20ed41b6d8ad4881d5449fc0897b6af12975
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-c/json-c_0.11.orig.tar.gz' json-c_0.11.orig.tar.gz 557263 SHA256:28dfc65145dc0d4df1dfe7701ac173c4e5f9347176c8983edbfac9149494448c
'http://archive.ubuntu.com/ubuntu/pool/main/j/json-c/json-c_0.11-4ubuntu2.debian.tar.xz' json-c_0.11-4ubuntu2.debian.tar.xz 273884 SHA256:96cce11fbf46e57c5b2674922344738c6f2ea1fa0af6e91b3576eb9f1dbd51d0
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

- `krb5-locales=1.13.2+dfsg-5ubuntu2.1`
- `libgssapi-krb5-2:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libk5crypto3:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkrb5-3:amd64=1.13.2+dfsg-5ubuntu2.1`
- `libkrb5support0:amd64=1.13.2+dfsg-5ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/krb5-locales/copyright`, `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.13.2+dfsg-5ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg-5ubuntu2.1.dsc' krb5_1.13.2+dfsg-5ubuntu2.1.dsc 3520 SHA256:d32e3a18bd00e7446c67d28c4c70bb96ec80da9b0e9215d4d8531100e1f91952
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg.orig.tar.gz' krb5_1.13.2+dfsg.orig.tar.gz 11884064 SHA256:a7af3953e4ab52b17f80bdfc2fc7471b66b512b128520796e2b993554543873a
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.13.2+dfsg-5ubuntu2.1.debian.tar.xz' krb5_1.13.2+dfsg-5ubuntu2.1.debian.tar.xz 113600 SHA256:2536a14f7a186c9076d8fb8053be04842300ab000046b4d53c8fa8c9959f1efd
```

### `dpkg` source package: `lame=3.99.5+repack1-9build1`

Binary Packages:

- `libmp3lame0:amd64=3.99.5+repack1-9build1`

Licenses: (parsed from: `/usr/share/doc/libmp3lame0/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-1+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris lame=3.99.5+repack1-9build1
'http://archive.ubuntu.com/ubuntu/pool/universe/l/lame/lame_3.99.5+repack1-9build1.dsc' lame_3.99.5+repack1-9build1.dsc 2298 SHA256:dba1adcbb3e8566da670e47ca491c4b353374f21fb2bbeb856be79ac14e16c59
'http://archive.ubuntu.com/ubuntu/pool/universe/l/lame/lame_3.99.5+repack1.orig.tar.gz' lame_3.99.5+repack1.orig.tar.gz 1464016 SHA256:01c1a34dc5ced11a487f04514cb948d38f6f559daebc85ae23c1c8a6c8280c95
'http://archive.ubuntu.com/ubuntu/pool/universe/l/lame/lame_3.99.5+repack1-9build1.debian.tar.xz' lame_3.99.5+repack1-9build1.debian.tar.xz 15520 SHA256:026f152ff188b9e7a5f4bb426c82a0cb8aff8f2503a870e16bcd6286df687934
```

### `dpkg` source package: `lcms2=2.6-3ubuntu2.1`

Binary Packages:

- `liblcms2-2:amd64=2.6-3ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/liblcms2-2/copyright`)

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

### `dpkg` source package: `libaacs=0.8.1-1`

Binary Packages:

- `libaacs0:amd64=0.8.1-1`

Licenses: (parsed from: `/usr/share/doc/libaacs0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libaacs=0.8.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libaacs/libaacs_0.8.1-1.dsc' libaacs_0.8.1-1.dsc 2143 SHA256:c2dfc2c3503c3339787017f74f16d23f703e55236b144644c37ffa69ce65fe5d
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libaacs/libaacs_0.8.1.orig.tar.bz2' libaacs_0.8.1.orig.tar.bz2 315231 SHA256:95c344a02c47c9753c50a5386fdfb8313f9e4e95949a5c523a452f0bcb01bbe8
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libaacs/libaacs_0.8.1-1.debian.tar.xz' libaacs_0.8.1-1.debian.tar.xz 3948 SHA256:7dd42062fc067de35c878b624e5c0cf225b01f39f69d1fa12a1434da5f129d79
```

### `dpkg` source package: `libass=0.13.1-1`

Binary Packages:

- `libass5:amd64=0.13.1-1`

Licenses: (parsed from: `/usr/share/doc/libass5/copyright`)

- `GPL-2`
- `GPL-2+`
- `ISC`
- `other-1`

Source:

```console
$ apt-get source -qq --print-uris libass=0.13.1-1
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libass/libass_0.13.1-1.dsc' libass_0.13.1-1.dsc 2120 SHA256:7dc13d4871aad1102a50755ae990d201f260d7a28dcc96cef12ee182ff4a2a81
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libass/libass_0.13.1.orig.tar.xz' libass_0.13.1.orig.tar.xz 318840 SHA256:4aa36b1876a61cab46fc9284fee84224b9e2840fe7b3e63d96a8d32574343fe7
'http://archive.ubuntu.com/ubuntu/pool/universe/liba/libass/libass_0.13.1-1.debian.tar.xz' libass_0.13.1-1.debian.tar.xz 5276 SHA256:b72d531075d630e120038c8f4a77a8342fbe9523915860b434102c495d47d166
```

### `dpkg` source package: `libasyncns=0.8-5build1`

Binary Packages:

- `libasyncns0:amd64=0.8-5build1`

Licenses: (parsed from: `/usr/share/doc/libasyncns0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libasyncns=0.8-5build1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libasyncns/libasyncns_0.8-5build1.dsc' libasyncns_0.8-5build1.dsc 1290 SHA256:719caa7a1a54a6af4d7aefa3f78e19005ef0df14c9b0dc9247dad0daed427bf5
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libasyncns/libasyncns_0.8.orig.tar.gz' libasyncns_0.8.orig.tar.gz 341591 SHA256:4f1a66e746cbe54ff3c2fbada5843df4fbbbe7481d80be003e8d11161935ab74
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libasyncns/libasyncns_0.8-5build1.debian.tar.xz' libasyncns_0.8-5build1.debian.tar.xz 4244 SHA256:4be991be063b22c91bfbe047433124db81c0ec28af6e310dc6d4e6b35dfbf7b2
```

### `dpkg` source package: `libavc1394=0.5.4-4`

Binary Packages:

- `libavc1394-0:amd64=0.5.4-4`

Licenses: (parsed from: `/usr/share/doc/libavc1394-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libavc1394=0.5.4-4
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libavc1394/libavc1394_0.5.4-4.dsc' libavc1394_0.5.4-4.dsc 2153 SHA256:e0fcaa8cfbf5b681575b8e56cdae9235baa6d8d0f5832ac08c7c8438276f0d7b
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libavc1394/libavc1394_0.5.4.orig.tar.gz' libavc1394_0.5.4.orig.tar.gz 341679 SHA256:7cb1ff09506ae911ca9860bef4af08c2403f3e131f6c913a2cbd6ddca4215b53
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libavc1394/libavc1394_0.5.4-4.debian.tar.xz' libavc1394_0.5.4-4.debian.tar.xz 6504 SHA256:2fd8771875db51024e01ac35b47ac873ce555a6bc8d2919346269cc1c450a472
```

### `dpkg` source package: `libbdplus=0.1.2-1`

Binary Packages:

- `libbdplus0:amd64=0.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libbdplus0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libbdplus=0.1.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbdplus/libbdplus_0.1.2-1.dsc' libbdplus_0.1.2-1.dsc 2207 SHA256:45b6b69a5ea10b6aa73bf5cee8b52f2df98828bf85f026df80bdb2f394fc2ce9
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbdplus/libbdplus_0.1.2.orig.tar.bz2' libbdplus_0.1.2.orig.tar.bz2 319828 SHA256:a631cae3cd34bf054db040b64edbfc8430936e762eb433b1789358ac3d3dc80a
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbdplus/libbdplus_0.1.2-1.debian.tar.xz' libbdplus_0.1.2-1.debian.tar.xz 2684 SHA256:4cc27445a7666a1992996cb842ce993177a3b152bb718083abdd60b4f9f5ba90
```

### `dpkg` source package: `libbluray=1:0.9.2-2`

Binary Packages:

- `libbluray1:amd64=1:0.9.2-2`

Licenses: (parsed from: `/usr/share/doc/libbluray1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MPL-1.0`

Source:

```console
$ apt-get source -qq --print-uris libbluray=1:0.9.2-2
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbluray/libbluray_0.9.2-2.dsc' libbluray_0.9.2-2.dsc 2601 SHA256:7d54d30fc9a7f39c4682d6577a9be5d2b489241713318e9445b059103c27695c
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbluray/libbluray_0.9.2.orig.tar.bz2' libbluray_0.9.2.orig.tar.bz2 704357 SHA256:efc994f42d2bce6af2ce69d05ba89dbbd88bcec7aca065de094fb3a7880ce7ea
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbluray/libbluray_0.9.2-2.debian.tar.xz' libbluray_0.9.2-2.debian.tar.xz 17172 SHA256:00d4d6631bf8a480c4e5ec4cfb286f4d1baa12daadcc50291e4deb325b7f66c0
```

### `dpkg` source package: `libbs2b=3.1.0+dfsg-2.2`

Binary Packages:

- `libbs2b0:amd64=3.1.0+dfsg-2.2`

Licenses: (parsed from: `/usr/share/doc/libbs2b0/copyright`)

- `FSF-unlimited`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `MIT`
- `MIT+FSF-public`

Source:

```console
$ apt-get source -qq --print-uris libbs2b=3.1.0+dfsg-2.2
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbs2b/libbs2b_3.1.0+dfsg-2.2.dsc' libbs2b_3.1.0+dfsg-2.2.dsc 1939 SHA256:a5fa01cf653b4161bb8595509be5ee91d1f47b8a9ff2b8c98b7fdd60b290e643
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbs2b/libbs2b_3.1.0+dfsg.orig.tar.gz' libbs2b_3.1.0+dfsg.orig.tar.gz 330675 SHA256:c23faf614f787342c1a1a40f83064f2e5a49391733c029dc31d09fba759cee0a
'http://archive.ubuntu.com/ubuntu/pool/universe/libb/libbs2b/libbs2b_3.1.0+dfsg-2.2.debian.tar.xz' libbs2b_3.1.0+dfsg-2.2.debian.tar.xz 4632 SHA256:37d7d8da3d0ab030ca49944e98c83b4ae8a4463d3a70c301af79da20e05b0440
```

### `dpkg` source package: `libbsd=0.8.2-1`

Binary Packages:

- `libbsd0:amd64=0.8.2-1`

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
$ apt-get source -qq --print-uris libbsd=0.8.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2-1.dsc' libbsd_0.8.2-1.dsc 1970 SHA256:c620fbc461ea4f78bb2283ed55e36d1d819354ee08980b28577795f512c2948f
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2.orig.tar.xz' libbsd_0.8.2.orig.tar.xz 344292 SHA256:b2f644cae94a6e2fe109449c20ad79a0f6ee4faec2205b07eefa0020565e250a
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.8.2-1.debian.tar.xz' libbsd_0.8.2-1.debian.tar.xz 14788 SHA256:03e03c6230dc0243aff0535e89f8e1969f2977b247c1ec57a9783cb1094a0906
```

### `dpkg` source package: `libcaca=0.99.beta19-2ubuntu0.16.04.1`

Binary Packages:

- `libcaca0:amd64=0.99.beta19-2ubuntu0.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libcaca0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libcaca=0.99.beta19-2ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcaca/libcaca_0.99.beta19-2ubuntu0.16.04.1.dsc' libcaca_0.99.beta19-2ubuntu0.16.04.1.dsc 2291 SHA256:68cc1cf69e1cb9c21055846c7b854e86e63909f685d7a3528e87d1c217d12f66
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcaca/libcaca_0.99.beta19.orig.tar.gz' libcaca_0.99.beta19.orig.tar.gz 1203495 SHA256:128b467c4ed03264c187405172a4e83049342cc8cc2f655f53a2d0ee9d3772f4
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcaca/libcaca_0.99.beta19-2ubuntu0.16.04.1.debian.tar.xz' libcaca_0.99.beta19-2ubuntu0.16.04.1.debian.tar.xz 12656 SHA256:e814cfe607cd2d97f757db76f4590196b3d351a4f80f174b05a8d3d090750bf5
```

### `dpkg` source package: `libcap-ng=0.7.7-1`

Binary Packages:

- `libcap-ng0:amd64=0.7.7-1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-1.dsc' libcap-ng_0.7.7-1.dsc 1720 SHA256:65bdf23e2d133255e83ef27c14a544c87afe2cf9123685fcf75c5c045805eccc
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7.orig.tar.gz' libcap-ng_0.7.7.orig.tar.gz 420178 SHA256:615549ce39b333f6b78baee0c0b4ef18bc726c6bf1cca123dfd89dd963f6d06b
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.7-1.debian.tar.xz' libcap-ng_0.7.7-1.debian.tar.xz 5040 SHA256:bb9e4801b17e9616cc187b001302894b1d1cf5035ca4040d9888420534c278ad
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

### `dpkg` source package: `libcdio=0.83-4.2ubuntu1`

Binary Packages:

- `libcdio-cdda1:amd64=0.83-4.2ubuntu1`
- `libcdio-paranoia1:amd64=0.83-4.2ubuntu1`
- `libcdio13:amd64=0.83-4.2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libcdio-cdda1/copyright`, `/usr/share/doc/libcdio-paranoia1/copyright`, `/usr/share/doc/libcdio13/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libcdio=0.83-4.2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio/libcdio_0.83-4.2ubuntu1.dsc' libcdio_0.83-4.2ubuntu1.dsc 2448 SHA256:17fb091e174d30e37eea5161ad9549a9304a918482f3fb3fb1e5f241135c36b8
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio/libcdio_0.83.orig.tar.gz' libcdio_0.83.orig.tar.gz 2323747 SHA256:235017e3eccb86424f9c108f2c5d5fca62630bda8c9dcf23b425ba9c5e2482c0
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcdio/libcdio_0.83-4.2ubuntu1.debian.tar.xz' libcdio_0.83-4.2ubuntu1.debian.tar.xz 11576 SHA256:43ea64f58e72dae0d77b436ecbac108038d220d552667ae5774701db62842bf2
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

### `dpkg` source package: `libdc1394-22=2.2.4-1`

Binary Packages:

- `libdc1394-22:amd64=2.2.4-1`

Licenses: (parsed from: `/usr/share/doc/libdc1394-22/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libdc1394-22=2.2.4-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libdc1394-22/libdc1394-22_2.2.4-1.dsc' libdc1394-22_2.2.4-1.dsc 2227 SHA256:573f73d6a8f42db3416cd84750c356631f5e5608146749201fcb51562fc18d4c
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libdc1394-22/libdc1394-22_2.2.4.orig.tar.gz' libdc1394-22_2.2.4.orig.tar.gz 609612 SHA256:a93689a353c241884a98727128f315ecf9965db70dca710b08af10e5fa0d2e6f
'http://archive.ubuntu.com/ubuntu/pool/universe/libd/libdc1394-22/libdc1394-22_2.2.4-1.debian.tar.xz' libdc1394-22_2.2.4-1.debian.tar.xz 8196 SHA256:7421eee4b233bc71f2c9b0c7b015bec7785ec048a1e6e462ed84853740f9a15e
```

### `dpkg` source package: `libdrm=2.4.91-2~16.04.1`

Binary Packages:

- `libdrm-amdgpu1:amd64=2.4.91-2~16.04.1`
- `libdrm-common=2.4.91-2~16.04.1`
- `libdrm-intel1:amd64=2.4.91-2~16.04.1`
- `libdrm-nouveau2:amd64=2.4.91-2~16.04.1`
- `libdrm-radeon1:amd64=2.4.91-2~16.04.1`
- `libdrm2:amd64=2.4.91-2~16.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libdrm=2.4.91-2~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91-2~16.04.1.dsc' libdrm_2.4.91-2~16.04.1.dsc 3293 SHA256:8891ccf20876073151eec7e69d8e6e6508ba1ec39d77d5d86bec7b04d5eff07e
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91.orig.tar.gz' libdrm_2.4.91.orig.tar.gz 1088866 SHA256:c8ea3343d5bfc356550f0b5632403359d050fa09cf05d61e96e73adba0c407a9
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91.orig.tar.gz.asc' libdrm_2.4.91.orig.tar.gz.asc 879 SHA256:ff4e25c667a98e1cba56836df542819bad3dab1aeb38ed1b6ed44c34895b2cca
'http://archive.ubuntu.com/ubuntu/pool/main/libd/libdrm/libdrm_2.4.91-2~16.04.1.diff.gz' libdrm_2.4.91-2~16.04.1.diff.gz 49908 SHA256:3bbb93e25a919e5305b2a0cee43d00bdbcd5f762eefbadf84616a423daea958b
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

### `dpkg` source package: `libffi=3.2.1-4`

Binary Packages:

- `libffi6:amd64=3.2.1-4`

Licenses: (parsed from: `/usr/share/doc/libffi6/copyright`)

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

### `dpkg` source package: `libgsm=1.0.13-4`

Binary Packages:

- `libgsm1:amd64=1.0.13-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libgsm=1.0.13-4
'http://archive.ubuntu.com/ubuntu/pool/universe/libg/libgsm/libgsm_1.0.13-4.dsc' libgsm_1.0.13-4.dsc 1140 SHA256:807be0900ebfc0d96ffa86fed633c389f465da6db7ee57adc275b479be3ccff0
'http://archive.ubuntu.com/ubuntu/pool/universe/libg/libgsm/libgsm_1.0.13.orig.tar.gz' libgsm_1.0.13.orig.tar.gz 65318 SHA256:52c518244d428c2e56c543b98c9135f4a76ff780c32455580b793f60a0a092ad
'http://archive.ubuntu.com/ubuntu/pool/universe/libg/libgsm/libgsm_1.0.13-4.debian.tar.gz' libgsm_1.0.13-4.debian.tar.gz 10333 SHA256:10baf466030802440a0de1b5a11e46292a82525f922bf9e0a182f509e0bc8514
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

### `dpkg` source package: `libiec61883=1.2.0-0.2`

Binary Packages:

- `libiec61883-0:amd64=1.2.0-0.2`

Licenses: (parsed from: `/usr/share/doc/libiec61883-0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libiec61883=1.2.0-0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libiec61883/libiec61883_1.2.0-0.2.dsc' libiec61883_1.2.0-0.2.dsc 1888 SHA256:0cca201c7d5e77ada0bbbf50c6da3ed1718406e3ef0b7a9994588f18ab0eeb71
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libiec61883/libiec61883_1.2.0.orig.tar.gz' libiec61883_1.2.0.orig.tar.gz 339064 SHA256:7c7879c6b9add3148baea697dfbfdcefffbc8ac74e8e6bcf46125ec1d21b373a
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libiec61883/libiec61883_1.2.0-0.2.diff.gz' libiec61883_1.2.0-0.2.diff.gz 6711 SHA256:84c54267c7fec62d2dbf9123057eba1ea9cffc0d29968cd747feb22020ddf71d
```

### `dpkg` source package: `libjpeg-turbo=1.4.2-0ubuntu3.3`

Binary Packages:

- `libjpeg-turbo8:amd64=1.4.2-0ubuntu3.3`

Licenses: (parsed from: `/usr/share/doc/libjpeg-turbo8/copyright`)

- `JPEG`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1.4.2-0ubuntu3.3
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2-0ubuntu3.3.dsc' libjpeg-turbo_1.4.2-0ubuntu3.3.dsc 2286 SHA256:9db340b995c90aa65172783bc80fc7af4a2ac0103ade1001797abca558f02dd7
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2.orig.tar.gz' libjpeg-turbo_1.4.2.orig.tar.gz 1569306 SHA256:521bb5d3043e7ac063ce3026d9a59cc2ab2e9636c655a2515af5f4706122233e
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjpeg-turbo/libjpeg-turbo_1.4.2-0ubuntu3.3.debian.tar.xz' libjpeg-turbo_1.4.2-0ubuntu3.3.debian.tar.xz 29632 SHA256:59e308a4ead3c152ecf512f6e31aaaca3e6be9067dae157113d2a8ce209cf06c
```

### `dpkg` source package: `libjpeg8-empty=8c-2ubuntu8`

Binary Packages:

- `libjpeg8:amd64=8c-2ubuntu8`

Licenses: (parsed from: `/usr/share/doc/libjpeg8/copyright`)

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

Licenses: (parsed from: `/usr/share/doc/liblqr-1-0/copyright`)

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

### `dpkg` source package: `libmodplug=1:0.8.8.5-2`

Binary Packages:

- `libmodplug1:amd64=1:0.8.8.5-2`

Licenses: (parsed from: `/usr/share/doc/libmodplug1/copyright`)

- `Public Domain`

Source:

```console
$ apt-get source -qq --print-uris libmodplug=1:0.8.8.5-2
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmodplug/libmodplug_0.8.8.5-2.dsc' libmodplug_0.8.8.5-2.dsc 2024 SHA256:f598b7c733b979612265f515b994710ab375b5fe708294d99a1e7c3ba1e98510
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmodplug/libmodplug_0.8.8.5.orig.tar.gz' libmodplug_0.8.8.5.orig.tar.gz 546751 SHA256:77462d12ee99476c8645cb5511363e3906b88b33a6b54362b4dbc0f39aa2daad
'http://archive.ubuntu.com/ubuntu/pool/universe/libm/libmodplug/libmodplug_0.8.8.5-2.debian.tar.xz' libmodplug_0.8.8.5-2.debian.tar.xz 11400 SHA256:929178a75202336f43b7ed70b7a32345523ef33abd1d2958e436668d9ddc28df
```

### `dpkg` source package: `libogg=1.3.2-1`

Binary Packages:

- `libogg0:amd64=1.3.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libogg=1.3.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libogg/libogg_1.3.2-1.dsc' libogg_1.3.2-1.dsc 1230 SHA256:dacc2059f8f92d1f6b18805432f2f40ac45fb9d52a1a61f14dc8c7c6a1aecb58
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libogg/libogg_1.3.2.orig.tar.gz' libogg_1.3.2.orig.tar.gz 557232 SHA256:bf253517df60ef1e6f5ae328bac7477595465de30638818948574e05f502dfa3
'http://archive.ubuntu.com/ubuntu/pool/main/libo/libogg/libogg_1.3.2-1.diff.gz' libogg_1.3.2-1.diff.gz 6824 SHA256:9bee2f473a5ed92f1c744105447f15fe38feea8935e740a9eea2d840fa2d15c7
```

### `dpkg` source package: `libpaper=1.1.24+nmu4ubuntu1`

Binary Packages:

- `libpaper-utils=1.1.24+nmu4ubuntu1`
- `libpaper1:amd64=1.1.24+nmu4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpaper-utils/copyright`, `/usr/share/doc/libpaper1/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpaper=1.1.24+nmu4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpaper/libpaper_1.1.24+nmu4ubuntu1.dsc' libpaper_1.1.24+nmu4ubuntu1.dsc 1085 SHA256:2fe39029a382438eebc25df6382535e321b96169d04b5c1146a1e8c13329f5d2
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpaper/libpaper_1.1.24+nmu4ubuntu1.tar.gz' libpaper_1.1.24+nmu4ubuntu1.tar.gz 369936 SHA256:b377e454ebc50712fc4820dd4d0d94b7a7205c9410507dc5f3f89326d38bfc16
```

### `dpkg` source package: `libpciaccess=0.13.4-1`

Binary Packages:

- `libpciaccess0:amd64=0.13.4-1`

Licenses: (parsed from: `/usr/share/doc/libpciaccess0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpciaccess=0.13.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.13.4-1.dsc' libpciaccess_0.13.4-1.dsc 2060 SHA256:c7413e1b3804ae83667d0144eabb5bcba046a16c12f20f94d861edb71a9f67e8
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.13.4.orig.tar.gz' libpciaccess_0.13.4.orig.tar.gz 440390 SHA256:74d92bda448e6fdb64fee4e0091255f48d625d07146a121653022ed3a0ca1f2f
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.13.4-1.diff.gz' libpciaccess_0.13.4-1.diff.gz 24145 SHA256:72e06952d417e15ee23766815f8f10555c2504189f9420a3b6df0be25e972650
```

### `dpkg` source package: `libpng=1.2.54-1ubuntu1.1`

Binary Packages:

- `libpng12-0:amd64=1.2.54-1ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libpng12-0/copyright`)

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

### `dpkg` source package: `libraw1394=2.1.1-2`

Binary Packages:

- `libraw1394-11:amd64=2.1.1-2`

Licenses: (parsed from: `/usr/share/doc/libraw1394-11/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libraw1394=2.1.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libraw1394/libraw1394_2.1.1-2.dsc' libraw1394_2.1.1-2.dsc 2080 SHA256:5909a47ecdae0ac0281eeda1487ce88ca7a04ac43af00bee0b622230959a0f22
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libraw1394/libraw1394_2.1.1.orig.tar.gz' libraw1394_2.1.1.orig.tar.gz 451309 SHA256:a960ac55fb81d56de055ab91b1e124c0ccbb657e059142d2d8fc644e4af8ca74
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libraw1394/libraw1394_2.1.1-2.debian.tar.xz' libraw1394_2.1.1-2.debian.tar.xz 8752 SHA256:b043b7a3cd17ca4122c63cb8c129ec06890106074aa4a54f939bc32c7e6ed05e
```

### `dpkg` source package: `libreoffice=1:5.1.6~rc2-0ubuntu1~xenial10`

Binary Packages:

- `uno-libs3=5.1.6~rc2-0ubuntu1~xenial10`
- `ure=5.1.6~rc2-0ubuntu1~xenial10`

Licenses: (parsed from: `/usr/share/doc/uno-libs3/copyright`, `/usr/share/doc/ure/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `BSD-4-clause`
- `CDDL-1.0`
- `CDDL-1.0 | GPPL-2`
- `GPL`
- `GPL-2`
- `GPL-2 | LGPL-2.1 | MPL-1.1`
- `GPL-2+`
- `LGPL`
- `LGPL | Apache-2.0`
- `LGPL-2`
- `LGPL-2 | Apache-2.0`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-3`
- `LGPL2+`
- `MIT`
- `MIT/X`
- `MPL 1.1 | LGPL-2+ | GPL-2+`
- `MPL-1.1`
- `MPL-1.1 | GPL-2 | LGPL-2`
- `MPL-1.1 | GPL-3+ | LGPL-3+`
- `MPL-1.1 | LGPL-2.1`
- `MPL-2.0`
- `PSF-2`
- `W3C`
- `Zlib`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libreoffice=1:5.1.6~rc2-0ubuntu1~xenial10
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_5.1.6~rc2-0ubuntu1~xenial10.dsc' libreoffice_5.1.6~rc2-0ubuntu1~xenial10.dsc 15032 SHA256:f1e5b995ac622b6e57ca0640dff6347618afa741351d650ac7652194453743f0
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_5.1.6~rc2.orig-src.tar.xz' libreoffice_5.1.6~rc2.orig-src.tar.xz 167395528 SHA256:97365b7193311f32a1e38de537d21c3b50dc35901dddad1a0ab968dbcc09b29e
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_5.1.6~rc2.orig-translations.tar.xz' libreoffice_5.1.6~rc2.orig-translations.tar.xz 134618348 SHA256:1ac60c5060d9f1073169a239efca8c85d8e0355623897dc795bb4de43fa4bc29
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_5.1.6~rc2.orig.tar.xz' libreoffice_5.1.6~rc2.orig.tar.xz 155867604 SHA256:729dcf538e6b825911ba5d24d822e90f76fab0ed5821f81ae60d5800eb0f848d
'http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice/libreoffice_5.1.6~rc2-0ubuntu1~xenial10.debian.tar.xz' libreoffice_5.1.6~rc2-0ubuntu1~xenial10.debian.tar.xz 2115668 SHA256:0870b4419171848a2f09933ce31fcf4b16b424d216814579ba7bf1e6c74daa36
```

### `dpkg` source package: `librsvg=2.40.13-3`

Binary Packages:

- `librsvg2-2:amd64=2.40.13-3`
- `librsvg2-common:amd64=2.40.13-3`

Licenses: (parsed from: `/usr/share/doc/librsvg2-2/copyright`, `/usr/share/doc/librsvg2-common/copyright`)

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

### `dpkg` source package: `libsamplerate=0.1.8-8`

Binary Packages:

- `libsamplerate0:amd64=0.1.8-8`

Licenses: (parsed from: `/usr/share/doc/libsamplerate0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libsamplerate=0.1.8-8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsamplerate/libsamplerate_0.1.8-8.dsc' libsamplerate_0.1.8-8.dsc 1940 SHA256:f13b419b19e18d7023b577382f7d2e65a6554b30793fde197338c7982c515660
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsamplerate/libsamplerate_0.1.8.orig.tar.gz' libsamplerate_0.1.8.orig.tar.gz 4303330 SHA256:93b54bdf46d5e6d2354b7034395fe329c222a966790de34520702bb9642f1c06
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsamplerate/libsamplerate_0.1.8-8.debian.tar.xz' libsamplerate_0.1.8-8.debian.tar.xz 5836 SHA256:d41c73e86687265491780fe507178513b320325108b026bb9d8f6672287c2225
```

### `dpkg` source package: `libsdl1.2=1.2.15+dfsg1-3ubuntu0.1`

Binary Packages:

- `libsdl1.2debian:amd64=1.2.15+dfsg1-3ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libsdl1.2debian/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsdl1.2=1.2.15+dfsg1-3ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsdl1.2/libsdl1.2_1.2.15+dfsg1-3ubuntu0.1.dsc' libsdl1.2_1.2.15+dfsg1-3ubuntu0.1.dsc 2488 SHA256:0b111bc5c5b5cece666b887ce08237c9ab486e2f850d2185cda2c06f4ed819af
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsdl1.2/libsdl1.2_1.2.15+dfsg1.orig.tar.xz' libsdl1.2_1.2.15+dfsg1.orig.tar.xz 2584144 SHA256:5a34fcefedc99099413aedae1219ca1b846f68c92526c61a65f9e520e7bc9552
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsdl1.2/libsdl1.2_1.2.15+dfsg1-3ubuntu0.1.debian.tar.xz' libsdl1.2_1.2.15+dfsg1-3ubuntu0.1.debian.tar.xz 36824 SHA256:2a8f74ee11d4a027a9c59a519f380b6b97828c2f1182d094fde98fa774ca4243
```

### `dpkg` source package: `libseccomp=2.4.1-0ubuntu0.16.04.2`

Binary Packages:

- `libseccomp2:amd64=2.4.1-0ubuntu0.16.04.2`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2`
- `LGPL-2.0+`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.1-0ubuntu0.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.1-0ubuntu0.16.04.2.dsc' libseccomp_2.4.1-0ubuntu0.16.04.2.dsc 2244 SHA256:a02bade5eb7ba5130822d827805101e24f6f090288b7ba800c1141ee94d4a7fe
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.1.orig.tar.gz' libseccomp_2.4.1.orig.tar.gz 606860 SHA256:1ca3735249af66a1b2f762fe6e710fcc294ad7185f1cc961e5bd83f9988006e8
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.1-0ubuntu0.16.04.2.debian.tar.xz' libseccomp_2.4.1-0ubuntu0.16.04.2.debian.tar.xz 10044 SHA256:ed11a719479bf2a57a079d8b293f7f58e2a311243f04fe808b251e491dd4c2fd
```

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

### `dpkg` source package: `libsndfile=1.0.25-10ubuntu0.16.04.2`

Binary Packages:

- `libsndfile1:amd64=1.0.25-10ubuntu0.16.04.2`

Licenses: (parsed from: `/usr/share/doc/libsndfile1/copyright`)

- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libsndfile=1.0.25-10ubuntu0.16.04.2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsndfile/libsndfile_1.0.25-10ubuntu0.16.04.2.dsc' libsndfile_1.0.25-10ubuntu0.16.04.2.dsc 2260 SHA256:309c8c40503c64aacd048e1b1ea346eabe9316ba09fed618f12cf7bd4f3708c9
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsndfile/libsndfile_1.0.25.orig.tar.gz' libsndfile_1.0.25.orig.tar.gz 1060692 SHA256:59016dbd326abe7e2366ded5c344c853829bebfd1702ef26a07ef662d6aa4882
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsndfile/libsndfile_1.0.25-10ubuntu0.16.04.2.debian.tar.xz' libsndfile_1.0.25-10ubuntu0.16.04.2.debian.tar.xz 20616 SHA256:5eae86a05a6498f37795b00f129b6a315e06cd8ab6d0d76a7928eeb18772b2ab
```

### `dpkg` source package: `libsodium=1.0.8-5`

Binary Packages:

- `libsodium18:amd64=1.0.8-5`

Licenses: (parsed from: `/usr/share/doc/libsodium18/copyright`)

- `BSD-2-clause`
- `CC0`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libsodium=1.0.8-5
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsodium/libsodium_1.0.8-5.dsc' libsodium_1.0.8-5.dsc 2022 SHA256:56e870b76ceea5517928be8af6c02c225fbc229ade25ece02aecebf34e2baf8b
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsodium/libsodium_1.0.8.orig.tar.gz' libsodium_1.0.8.orig.tar.gz 1412473 SHA256:61493bdbb13d29b2d0bf5113199e141b986f97f414e86e510f59cfb4e42c85f1
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsodium/libsodium_1.0.8-5.debian.tar.xz' libsodium_1.0.8-5.debian.tar.xz 5844 SHA256:0d55a56baaf2f141c87bb297fcf6d1d078c4d7bde67553774734cf29248e09eb
```

### `dpkg` source package: `libsoxr=0.1.2-1`

Binary Packages:

- `libsoxr0:amd64=0.1.2-1`

Licenses: (parsed from: `/usr/share/doc/libsoxr0/copyright`)

- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Spherepack`
- `permissive1`
- `permissive2`

Source:

```console
$ apt-get source -qq --print-uris libsoxr=0.1.2-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsoxr/libsoxr_0.1.2-1.dsc' libsoxr_0.1.2-1.dsc 2106 SHA256:dc9cdb6f3f88d79abaed570c450fe1ba6f3eba163fd83e5572c817b52c7a0762
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsoxr/libsoxr_0.1.2.orig.tar.xz' libsoxr_0.1.2.orig.tar.xz 83760 SHA256:54e6f434f1c491388cd92f0e3c47f1ade082cc24327bdc43762f7d1eefe0c275
'http://archive.ubuntu.com/ubuntu/pool/universe/libs/libsoxr/libsoxr_0.1.2-1.debian.tar.xz' libsoxr_0.1.2-1.debian.tar.xz 4096 SHA256:46f983cbef66856659fc496de6f112f978abeafd2468c816081c6b30bfffb713
```

### `dpkg` source package: `libssh=0.6.3-4.3ubuntu0.5`

Binary Packages:

- `libssh-gcrypt-4:amd64=0.6.3-4.3ubuntu0.5`

Licenses: (parsed from: `/usr/share/doc/libssh-gcrypt-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.6.3-4.3ubuntu0.5
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.6.3-4.3ubuntu0.5.dsc' libssh_0.6.3-4.3ubuntu0.5.dsc 2429 SHA256:fabe7624254eb4c8ad11f8c0c3e249c6a402755856c4321a3b8c6b20eae1b327
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.6.3.orig.tar.xz' libssh_0.6.3.orig.tar.xz 279492 SHA256:2bb5d7c595059f990a8915c190169257328ffa828ced0c05b09bbe186092cacb
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.6.3-4.3ubuntu0.5.debian.tar.xz' libssh_0.6.3-4.3ubuntu0.5.debian.tar.xz 35892 SHA256:f7e646567b1cccb5030a1d2291b746c9c9b13d899f1581fca57677e5e3e01178
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

### `dpkg` source package: `libtheora=1.1.1+dfsg.1-8`

Binary Packages:

- `libtheora0:amd64=1.1.1+dfsg.1-8`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libtheora=1.1.1+dfsg.1-8
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-8.dsc' libtheora_1.1.1+dfsg.1-8.dsc 2520 SHA256:3b5365363e8abcf789d0ee848a24288dddba595953a1f8152c0319392d7e3b97
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1.orig.tar.gz' libtheora_1.1.1+dfsg.1.orig.tar.gz 2100495 SHA256:c59b0f07a7314dfe2ade15c41bc9f637f8a450fc6b340af61b81760629f28f90
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtheora/libtheora_1.1.1+dfsg.1-8.debian.tar.xz' libtheora_1.1.1+dfsg.1-8.debian.tar.xz 9208 SHA256:c4746f3502fe3489c95895e9ac4572bfc1d8b151349e50395abfd2000f15908c
```

### `dpkg` source package: `libtool=2.4.6-0.1`

Binary Packages:

- `libltdl7:amd64=2.4.6-0.1`

Licenses: (parsed from: `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-0.1
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-0.1.dsc' libtool_2.4.6-0.1.dsc 2080 SHA256:c0ec24bc1e892564840061e64cf288e018484d733208d97815f3b12f043088b6
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-0.1.debian.tar.xz' libtool_2.4.6-0.1.debian.tar.xz 19332 SHA256:1b9d3e0f9d177d259206cdda69d6cec8dd04df14cbb064b71869936ca5f2722f
```

### `dpkg` source package: `libusb-1.0=2:1.0.20-1`

Binary Packages:

- `libusb-1.0-0:amd64=2:1.0.20-1`

Licenses: (parsed from: `/usr/share/doc/libusb-1.0-0/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libusb-1.0=2:1.0.20-1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb-1.0/libusb-1.0_1.0.20-1.dsc' libusb-1.0_1.0.20-1.dsc 2096 SHA256:2d9dab764f330c6343d1ba97a0d77ad6e47d338061e845b0256d02d3fc014154
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb-1.0/libusb-1.0_1.0.20.orig.tar.bz2' libusb-1.0_1.0.20.orig.tar.bz2 795247 SHA256:cb057190ba0a961768224e4dc6883104c6f945b2bf2ef90d7da39e7c1834f7ff
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libusb-1.0/libusb-1.0_1.0.20-1.debian.tar.xz' libusb-1.0_1.0.20-1.debian.tar.xz 10132 SHA256:79181f1b8487cef862c31d5ba378dcc05efed76d5a55a7ae4961b788dcf3a2d4
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

### `dpkg` source package: `libva=1.7.0-1ubuntu0.1`

Binary Packages:

- `libva1:amd64=1.7.0-1ubuntu0.1`
- `va-driver-all:amd64=1.7.0-1ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libva1/copyright`, `/usr/share/doc/va-driver-all/copyright`)

- `BSD-3-clause`
- `Expat`
- `Expat-advertising`
- `GPL-2`
- `GPL-2+`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libva=1.7.0-1ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/universe/libv/libva/libva_1.7.0-1ubuntu0.1.dsc' libva_1.7.0-1ubuntu0.1.dsc 2720 SHA256:eb873c37df426241183d94ae92615b3b0a14b4a69c7516c0e947429b075d3cc6
'http://archive.ubuntu.com/ubuntu/pool/universe/libv/libva/libva_1.7.0.orig.tar.bz2' libva_1.7.0.orig.tar.bz2 788519 SHA256:a689bccbcc81a66b458e448377f108c057d3eee44a2e21a23c92c549dc8bc95f
'http://archive.ubuntu.com/ubuntu/pool/universe/libv/libva/libva_1.7.0-1ubuntu0.1.debian.tar.xz' libva_1.7.0-1ubuntu0.1.debian.tar.xz 11764 SHA256:9e0d737a1a3d93654ebfcda9f715f601fa7b91b068e16787c41ed66803e8770e
```

### `dpkg` source package: `libvdpau=1.1.1-3ubuntu1`

Binary Packages:

- `libvdpau1:amd64=1.1.1-3ubuntu1`
- `vdpau-driver-all:amd64=1.1.1-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libvdpau1/copyright`, `/usr/share/doc/vdpau-driver-all/copyright`)

- `Expat`
- `other`

Source:

```console
$ apt-get source -qq --print-uris libvdpau=1.1.1-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvdpau/libvdpau_1.1.1-3ubuntu1.dsc' libvdpau_1.1.1-3ubuntu1.dsc 2429 SHA256:a11d3d368f3686ef488019090abd50bffc180560128778b40ec9a477975743d4
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvdpau/libvdpau_1.1.1.orig.tar.bz2' libvdpau_1.1.1.orig.tar.bz2 429576 SHA256:857a01932609225b9a3a5bf222b85e39b55c08787d0ad427dbd9ec033d58d736
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvdpau/libvdpau_1.1.1-3ubuntu1.debian.tar.xz' libvdpau_1.1.1-3ubuntu1.debian.tar.xz 15708 SHA256:720d7706e6f63dfe360d203c724210588d6ecfc77f2adce95b5d64273311a494
```

### `dpkg` source package: `libvorbis=1.3.5-3ubuntu0.2`

Binary Packages:

- `libvorbis0a:amd64=1.3.5-3ubuntu0.2`
- `libvorbisenc2:amd64=1.3.5-3ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libvorbis=1.3.5-3ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvorbis/libvorbis_1.3.5-3ubuntu0.2.dsc' libvorbis_1.3.5-3ubuntu0.2.dsc 2377 SHA256:e1d72e8615ad7e702fdd48bd9298d464fd11982ab5832bb63626c7e84b9ff331
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvorbis/libvorbis_1.3.5.orig.tar.gz' libvorbis_1.3.5.orig.tar.gz 1638779 SHA256:6efbcecdd3e5dfbf090341b485da9d176eb250d893e3eb378c428a2db38301ce
'http://archive.ubuntu.com/ubuntu/pool/main/libv/libvorbis/libvorbis_1.3.5-3ubuntu0.2.debian.tar.xz' libvorbis_1.3.5-3ubuntu0.2.debian.tar.xz 12340 SHA256:7b5a461437a2666ec6c3efb06153a415339d89aca4adba19fd0ca235f6a7afc6
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

- `libwebp5:amd64=0.4.4-1`

Licenses: (parsed from: `/usr/share/doc/libwebp5/copyright`)

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

- `libwmf0.2-7:amd64=0.2.8.4-10.5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libwmf0.2-7/copyright`)

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
- `libx11-doc=2:1.6.3-1ubuntu2.1`
- `libx11-xcb1:amd64=2:1.6.3-1ubuntu2.1`

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

- `libxcb-dri2-0:amd64=1.11.1-1ubuntu1`
- `libxcb-dri3-0:amd64=1.11.1-1ubuntu1`
- `libxcb-glx0:amd64=1.11.1-1ubuntu1`
- `libxcb-present0:amd64=1.11.1-1ubuntu1`
- `libxcb-render0:amd64=1.11.1-1ubuntu1`
- `libxcb-shape0:amd64=1.11.1-1ubuntu1`
- `libxcb-shm0:amd64=1.11.1-1ubuntu1`
- `libxcb-sync1:amd64=1.11.1-1ubuntu1`
- `libxcb-xfixes0:amd64=1.11.1-1ubuntu1`
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

### `dpkg` source package: `libxml2=2.9.3+dfsg1-1ubuntu0.6`

Binary Packages:

- `libxml2:amd64=2.9.3+dfsg1-1ubuntu0.6`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.3+dfsg1-1ubuntu0.6
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1-1ubuntu0.6.dsc' libxml2_2.9.3+dfsg1-1ubuntu0.6.dsc 2756 SHA256:84190804790d1e8f6c072e26814d0ab951b50c0e69183b11d193e798d44ce01c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1.orig.tar.xz' libxml2_2.9.3+dfsg1.orig.tar.xz 2475440 SHA256:d6b7686fa12c70dd9ce7c7d97c84471b5afed1c176538df8c670754d8c206079
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.3+dfsg1-1ubuntu0.6.debian.tar.xz' libxml2_2.9.3+dfsg1-1ubuntu0.6.debian.tar.xz 57344 SHA256:a11cde44339fc40403f81eb2383a9118b0c714027299adde1d56e15d808718bd
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

### `dpkg` source package: `libxshmfence=1.2-1`

Binary Packages:

- `libxshmfence1:amd64=1.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxshmfence=1.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.2-1.dsc' libxshmfence_1.2-1.dsc 2128 SHA256:85a28d2f6211ebbf0a115d0f72d874cce179178958bcb2a77094e3499464b25d
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.2.orig.tar.gz' libxshmfence_1.2.orig.tar.gz 355356 SHA256:58467a0e36fc4ec749dc55f81a4ab3b822c82b6dfb7d36bdb6b28c9fd2a5ccaf
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxshmfence/libxshmfence_1.2-1.diff.gz' libxshmfence_1.2-1.diff.gz 13284 SHA256:65db7e07c5c5b12d0b1f93cdb0c4e3e448429240044247ea2f64a89c0cce5f8e
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

### `dpkg` source package: `libxtst=2:1.2.2-1`

Binary Packages:

- `libxtst6:amd64=2:1.2.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxtst=2:1.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxtst/libxtst_1.2.2-1.dsc' libxtst_1.2.2-1.dsc 2303 SHA256:92507fe81ab453ee4e9de52e3b638e33429f74f175ea496c310bffb8434e4b4d
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxtst/libxtst_1.2.2.orig.tar.gz' libxtst_1.2.2.orig.tar.gz 392569 SHA256:221838960c7b9058cd6795c1c3ee8e25bae1c68106be314bc3036a4f26be0e6c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxtst/libxtst_1.2.2-1.diff.gz' libxtst_1.2.2-1.diff.gz 16977 SHA256:3f1ae4cee26b1d93d037610bb7397f324eb293a0520e2be5f5bd822c115cd639
```

### `dpkg` source package: `libxv=2:1.0.10-1`

Binary Packages:

- `libxv1:amd64=2:1.0.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxv=2:1.0.10-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxv/libxv_1.0.10-1.dsc' libxv_1.0.10-1.dsc 1977 SHA256:488cadaa5f248215bf6c617ccd0b00381cc78f4f02aee4d758e2e041e24b6c4a
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxv/libxv_1.0.10.orig.tar.gz' libxv_1.0.10.orig.tar.gz 386940 SHA256:89a664928b625558268de81c633e300948b3752b0593453d7815f8775bab5293
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxv/libxv_1.0.10-1.diff.gz' libxv_1.0.10-1.diff.gz 15227 SHA256:a2ab595bcd2394cd224852d0e679fdec911d7947e33ca6c6a800e93bbf9bd446
```

### `dpkg` source package: `libxxf86vm=1:1.1.4-1`

Binary Packages:

- `libxxf86vm1:amd64=1:1.1.4-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxxf86vm=1:1.1.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.dsc' libxxf86vm_1.1.4-1.dsc 2078 SHA256:5a3aded030a415b0d6c201d2b9d3af36f241dc981f10052fd4c2b56d59597838
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4.orig.tar.gz' libxxf86vm_1.1.4.orig.tar.gz 363146 SHA256:5108553c378a25688dcb57dca383664c36e293d60b1505815f67980ba9318a99
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxxf86vm/libxxf86vm_1.1.4-1.diff.gz' libxxf86vm_1.1.4-1.diff.gz 8040 SHA256:e0f11739d28c7a4475820ebda26e6f29e6cfa80b99a3513c075471132c81725b
```

### `dpkg` source package: `llvm-toolchain-6.0=1:6.0-1ubuntu2~16.04.1`

Binary Packages:

- `libllvm6.0:amd64=1:6.0-1ubuntu2~16.04.1`

Licenses: (parsed from: `/usr/share/doc/libllvm6.0/copyright`)

- `ARM`
- `Apple`
- `BSD-3-Clause`
- `BSD-3-clause`
- `Expat`
- `LLVM`
- `MIT`
- `NCSA`
- `Polly`
- `Python`
- `U-OF-I-BSD-LIKE`
- `public-domain`
- `solar-public-domain`

Source:

```console
$ apt-get source -qq --print-uris llvm-toolchain-6.0=1:6.0-1ubuntu2~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.dsc' llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.dsc 6967 SHA256:b62f6b396290a6c82417d9e1104a24066d95b543e7d40aa2337efc84710a2d85
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-clang-tools-extra.tar.bz2' llvm-toolchain-6.0_6.0.orig-clang-tools-extra.tar.bz2 808825 SHA256:f5c96f38067cf0c8d81395452d0386e4715d83bd5588e49832798f6ed4b2d8fa
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-clang.tar.bz2' llvm-toolchain-6.0_6.0.orig-clang.tar.bz2 13228782 SHA256:d6d155313658edc8f901b1f01e353605de1c6a9a1efe6c87b2c111d23febad43
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-compiler-rt.tar.bz2' llvm-toolchain-6.0_6.0.orig-compiler-rt.tar.bz2 2145520 SHA256:7253f34ae3faee95f32ee6b4a674b87911338f49f5e14f24afb2fa693f53b09c
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-lld.tar.bz2' llvm-toolchain-6.0_6.0.orig-lld.tar.bz2 853733 SHA256:cd67e62c2bfc5cef9fad2b0b1044c072956bc0ab1692616d5dd9b4034782ab1e
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-lldb.tar.bz2' llvm-toolchain-6.0_6.0.orig-lldb.tar.bz2 11238461 SHA256:4519601ff08e43e83dc42dbdd8de134e59e33f78466fd88f1fdfd79798f5bdef
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig-polly.tar.bz2' llvm-toolchain-6.0_6.0.orig-polly.tar.bz2 3253870 SHA256:a256c73b80c5bc311e8dc9471ded02a48c59583a3302f62f3296d223e108b6c6
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0.orig.tar.bz2' llvm-toolchain-6.0_6.0.orig.tar.bz2 29853313 SHA256:6e3439558692bbfd0bcaf4c4d1290e0c97bd710dab42860e0585303bbf67797a
'http://archive.ubuntu.com/ubuntu/pool/main/l/llvm-toolchain-6.0/llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.debian.tar.xz' llvm-toolchain-6.0_6.0-1ubuntu2~16.04.1.debian.tar.xz 70280 SHA256:8d02b5b988e4a5feeb00f374b1a324c5636ebe382f2b6c303afb84895b2f2f48
```

### `dpkg` source package: `lm-sensors=1:3.4.0-2`

Binary Packages:

- `libsensors4:amd64=1:3.4.0-2`

Licenses: (parsed from: `/usr/share/doc/libsensors4/copyright`)

- `GPL`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lm-sensors=1:3.4.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0-2.dsc' lm-sensors_3.4.0-2.dsc 1964 SHA256:bd3cecc8bbef17a0213d1ec38bdaca3a1cafae93cab116d17b5d7eec9a62d60f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0.orig.tar.bz2' lm-sensors_3.4.0.orig.tar.bz2 175802 SHA256:e0579016081a262dd23eafe1d22b41ebde78921e73a1dcef71e05e424340061f
'http://archive.ubuntu.com/ubuntu/pool/main/l/lm-sensors/lm-sensors_3.4.0-2.debian.tar.xz' lm-sensors_3.4.0-2.debian.tar.xz 28484 SHA256:efdb87b87c37be8a1eb478d78046838c3ab0178ffad23dce3f159fbf89e24d9c
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

### `dpkg` source package: `mesa=18.0.5-0ubuntu0~16.04.1`

Binary Packages:

- `libgl1-mesa-dri:amd64=18.0.5-0ubuntu0~16.04.1`
- `libgl1-mesa-glx:amd64=18.0.5-0ubuntu0~16.04.1`
- `libglapi-mesa:amd64=18.0.5-0ubuntu0~16.04.1`
- `mesa-va-drivers:amd64=18.0.5-0ubuntu0~16.04.1`
- `mesa-vdpau-drivers:amd64=18.0.5-0ubuntu0~16.04.1`

Licenses: (parsed from: `/usr/share/doc/libgl1-mesa-dri/copyright`, `/usr/share/doc/libgl1-mesa-glx/copyright`, `/usr/share/doc/libglapi-mesa/copyright`, `/usr/share/doc/mesa-va-drivers/copyright`, `/usr/share/doc/mesa-vdpau-drivers/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris mesa=18.0.5-0ubuntu0~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5-0ubuntu0~16.04.1.dsc' mesa_18.0.5-0ubuntu0~16.04.1.dsc 5261 SHA256:aa9e97113d9328c311541b1a673947c3a847d096a7e1e294216b31aff7165521
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5.orig.tar.gz' mesa_18.0.5.orig.tar.gz 19123780 SHA256:ea3e00329cea899b1e32db812fd2f426832be37e4baa2e2fd9288a3480f30531
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5.orig.tar.gz.asc' mesa_18.0.5.orig.tar.gz.asc 879 SHA256:a651bd04a5290244cb15c2504be35adfbc02ffa6d2fa1621cf88dccd3fa70b52
'http://archive.ubuntu.com/ubuntu/pool/main/m/mesa/mesa_18.0.5-0ubuntu0~16.04.1.diff.gz' mesa_18.0.5-0ubuntu0~16.04.1.diff.gz 144399 SHA256:2baac4569c59de2c6a0081cef1a16c28d66f6a583a8b1d6dde0295a942e3f4fc
```

### `dpkg` source package: `ncurses=6.0+20160213-1ubuntu1`

Binary Packages:

- `libncurses5:amd64=6.0+20160213-1ubuntu1`
- `libncursesw5:amd64=6.0+20160213-1ubuntu1`
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

### `dpkg` source package: `net-tools=1.60-26ubuntu1`

Binary Packages:

- `net-tools=1.60-26ubuntu1`

Licenses: (parsed from: `/usr/share/doc/net-tools/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris net-tools=1.60-26ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/n/net-tools/net-tools_1.60-26ubuntu1.dsc' net-tools_1.60-26ubuntu1.dsc 1903 SHA256:0a2b2ae7502ead9a2759c0edf551274c79ec8a29934c25a22e90c01662a05ade
'http://archive.ubuntu.com/ubuntu/pool/main/n/net-tools/net-tools_1.60.orig.tar.gz' net-tools_1.60.orig.tar.gz 265441 SHA256:ec67967cf7b1a3a3828a84762fbc013ac50ee5dc9aa3095d5c591f302c2de0f5
'http://archive.ubuntu.com/ubuntu/pool/main/n/net-tools/net-tools_1.60-26ubuntu1.diff.gz' net-tools_1.60-26ubuntu1.diff.gz 228352 SHA256:e08e8a6d028be1b02a0d75456a6edd42fc5659ab697bce199b5767c4ab666b06
```

### `dpkg` source package: `netpbm-free=2:10.0-15.3`

Binary Packages:

- `libnetpbm10=2:10.0-15.3`
- `netpbm=2:10.0-15.3`

Licenses: (parsed from: `/usr/share/doc/libnetpbm10/copyright`, `/usr/share/doc/netpbm/copyright`)

- `BSD`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris netpbm-free=2:10.0-15.3
'http://archive.ubuntu.com/ubuntu/pool/main/n/netpbm-free/netpbm-free_10.0-15.3.dsc' netpbm-free_10.0-15.3.dsc 2160 SHA256:8f833d8c186784b98dd632b401fedf7ee71323fb8eff0d837dff1bb9b9f26e57
'http://archive.ubuntu.com/ubuntu/pool/main/n/netpbm-free/netpbm-free_10.0.orig.tar.gz' netpbm-free_10.0.orig.tar.gz 1926538 SHA256:ea3a653f3e5a32e09cea903c5861138f6a597670dff79e2b54e902f140cff2f3
'http://archive.ubuntu.com/ubuntu/pool/main/n/netpbm-free/netpbm-free_10.0-15.3.diff.gz' netpbm-free_10.0-15.3.diff.gz 72028 SHA256:42f9f2f98951f830bc738605fa4c698538c15aed1a0229162bdcf2c6cdf87915
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

### `dpkg` source package: `nspr=2:4.13.1-0ubuntu0.16.04.1`

Binary Packages:

- `libnspr4:amd64=2:4.13.1-0ubuntu0.16.04.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nspr=2:4.13.1-0ubuntu0.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nspr/nspr_4.13.1-0ubuntu0.16.04.1.dsc' nspr_4.13.1-0ubuntu0.16.04.1.dsc 2258 SHA256:02c9e96f0c75b088f70dd1ca22494b649d5dc0b74767966874cedfd27f9e3cd5
'http://archive.ubuntu.com/ubuntu/pool/main/n/nspr/nspr_4.13.1.orig.tar.gz' nspr_4.13.1.orig.tar.gz 1136646 SHA256:5e4c1751339a76e7c772c0c04747488d7f8c98980b434dc846977e43117833ab
'http://archive.ubuntu.com/ubuntu/pool/main/n/nspr/nspr_4.13.1-0ubuntu0.16.04.1.debian.tar.xz' nspr_4.13.1-0ubuntu0.16.04.1.debian.tar.xz 18308 SHA256:047734933b7369657df94947858aa40ad38b46cdd7ba7ead6c6e1656739aac13
```

### `dpkg` source package: `nss=2:3.28.4-0ubuntu0.16.04.10`

Binary Packages:

- `libnss3:amd64=2:3.28.4-0ubuntu0.16.04.10`
- `libnss3-nssdb=2:3.28.4-0ubuntu0.16.04.10`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris nss=2:3.28.4-0ubuntu0.16.04.10
'http://archive.ubuntu.com/ubuntu/pool/main/n/nss/nss_3.28.4-0ubuntu0.16.04.10.dsc' nss_3.28.4-0ubuntu0.16.04.10.dsc 2432 SHA256:9c93d25bad349d3def5fdaa01588070d507f13c76cbd4dde866886b6197ef926
'http://archive.ubuntu.com/ubuntu/pool/main/n/nss/nss_3.28.4.orig.tar.gz' nss_3.28.4.orig.tar.gz 7453282 SHA256:d5d4761778b8d4c378b2174c9e13e7abd20a6961f557d4fcc029af723ffd7189
'http://archive.ubuntu.com/ubuntu/pool/main/n/nss/nss_3.28.4-0ubuntu0.16.04.10.debian.tar.xz' nss_3.28.4-0ubuntu0.16.04.10.debian.tar.xz 45120 SHA256:6c0163e359d5be3e8189dccaafaaf4c4f3107d7c45a4064e73b01ee9f8b60298
```

### `dpkg` source package: `numactl=2.0.11-1ubuntu1.1`

Binary Packages:

- `libnuma1:amd64=2.0.11-1ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.11-1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-1ubuntu1.1.dsc' numactl_2.0.11-1ubuntu1.1.dsc 2215 SHA256:23e5dcb50051fdc25d2fa6fb4e2c64bebf38dbdcde446b18e13673eada21cde4
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11.orig.tar.gz' numactl_2.0.11.orig.tar.gz 408175 SHA256:450c091235f891ee874a8651b179c30f57a1391ca5c4673354740ba65e527861
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.11-1ubuntu1.1.diff.gz' numactl_2.0.11-1ubuntu1.1.diff.gz 7106 SHA256:555a31c7676e117867a8ab2a0218f4c5581d8059547425c9b54e28edc5401a23
```

### `dpkg` source package: `openal-soft=1:1.16.0-3`

Binary Packages:

- `libopenal-data=1:1.16.0-3`
- `libopenal1:amd64=1:1.16.0-3`

Licenses: (parsed from: `/usr/share/doc/libopenal-data/copyright`, `/usr/share/doc/libopenal1/copyright`)

- `Apache`
- `BSD-3-clause-cmake`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2+`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris openal-soft=1:1.16.0-3
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openal-soft/openal-soft_1.16.0-3.dsc' openal-soft_1.16.0-3.dsc 2387 SHA256:8493d2316a3fc15d94e07fe195b3278e2d9ff6567a02266276a0b4f75a789259
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openal-soft/openal-soft_1.16.0.orig.tar.bz2' openal-soft_1.16.0.orig.tar.bz2 393280 SHA256:2f3dcd313fe26391284fbf8596863723f99c65d6c6846dccb48e79cadaf40d5f
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openal-soft/openal-soft_1.16.0-3.debian.tar.xz' openal-soft_1.16.0-3.debian.tar.xz 12520 SHA256:3351735b5ac97b464c79cca06a94a5045746e60afd7a59a75abe0403cf8a0aae
```

### `dpkg` source package: `opencv=2.4.9.1+dfsg-1.5ubuntu1.1`

Binary Packages:

- `libopencv-core2.4v5:amd64=2.4.9.1+dfsg-1.5ubuntu1.1`
- `libopencv-imgproc2.4v5:amd64=2.4.9.1+dfsg-1.5ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris opencv=2.4.9.1+dfsg-1.5ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/opencv/opencv_2.4.9.1+dfsg-1.5ubuntu1.1.dsc' opencv_2.4.9.1+dfsg-1.5ubuntu1.1.dsc 6107 SHA256:e517f6af2a31a02c81e972cb28b321acfe48b101cbb9bca6681e9dccbadce784
'http://archive.ubuntu.com/ubuntu/pool/universe/o/opencv/opencv_2.4.9.1+dfsg.orig.tar.xz' opencv_2.4.9.1+dfsg.orig.tar.xz 55863896 SHA256:aade3b475cc1a9c53076dbcfa0da5aa452733bfeec6bc54dae4d9c4e229594ea
'http://archive.ubuntu.com/ubuntu/pool/universe/o/opencv/opencv_2.4.9.1+dfsg-1.5ubuntu1.1.debian.tar.xz' opencv_2.4.9.1+dfsg-1.5ubuntu1.1.debian.tar.xz 42700 SHA256:19cdda618be7aec8bc0fce5802bc0728666e611068ebc812499e6bc2c3bd1353
```

### `dpkg` source package: `openexr=2.2.0-10ubuntu2.1`

Binary Packages:

- `libopenexr22:amd64=2.2.0-10ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libopenexr22/copyright`)

- `openexr`

Source:

```console
$ apt-get source -qq --print-uris openexr=2.2.0-10ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-10ubuntu2.1.dsc' openexr_2.2.0-10ubuntu2.1.dsc 2395 SHA256:8f2e3f8c3e124f9a726ffcfbb7699630040491dfb6fb6cd5582d3c5f21dc717a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0.orig.tar.gz' openexr_2.2.0.orig.tar.gz 14489661 SHA256:36a012f6c43213f840ce29a8b182700f6cf6b214bea0d5735594136b44914231
'http://archive.ubuntu.com/ubuntu/pool/main/o/openexr/openexr_2.2.0-10ubuntu2.1.debian.tar.xz' openexr_2.2.0-10ubuntu2.1.debian.tar.xz 36820 SHA256:c7ca79ae2f3862af7780478eee19f23a78259a76125c43cd987ebbd6294e973e
```

### `dpkg` source package: `openjdk-8=8u232-b09-0ubuntu1~16.04.1`

Binary Packages:

- `openjdk-8-jdk:amd64=8u232-b09-0ubuntu1~16.04.1`
- `openjdk-8-jdk-headless:amd64=8u232-b09-0ubuntu1~16.04.1`
- `openjdk-8-jre:amd64=8u232-b09-0ubuntu1~16.04.1`
- `openjdk-8-jre-headless:amd64=8u232-b09-0ubuntu1~16.04.1`

Licenses: (parsed from: `/usr/share/doc/openjdk-8-jdk/copyright`, `/usr/share/doc/openjdk-8-jdk-headless/copyright`, `/usr/share/doc/openjdk-8-jre/copyright`, `/usr/share/doc/openjdk-8-jre-headless/copyright`)

- `Apache-2.0`
- `GPL-2`
- `LGPL-2`
- `LGPL-2-1`

Source:

```console
$ apt-get source -qq --print-uris openjdk-8=8u232-b09-0ubuntu1~16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjdk-8/openjdk-8_8u232-b09-0ubuntu1~16.04.1.dsc' openjdk-8_8u232-b09-0ubuntu1~16.04.1.dsc 4884 SHA256:5d83f92441a8a24653d749eb908cb4fbc38b46ee86d306411dbb28ac551378ae
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjdk-8/openjdk-8_8u232-b09.orig.tar.xz' openjdk-8_8u232-b09.orig.tar.xz 71302544 SHA256:5ad0e67de7f3cda5080e66a6bb402d0e844757141ecbc684676abe1eb0f2599e
'http://archive.ubuntu.com/ubuntu/pool/main/o/openjdk-8/openjdk-8_8u232-b09-0ubuntu1~16.04.1.debian.tar.xz' openjdk-8_8u232-b09-0ubuntu1~16.04.1.debian.tar.xz 242860 SHA256:c59e3e6aef8f88682ae650eb603594a254d1eb7c849f12743fa2d174692d8fb0
```

### `dpkg` source package: `openjpeg=1:1.5.2-3.1`

Binary Packages:

- `libopenjpeg5:amd64=1:1.5.2-3.1`

Licenses: (parsed from: `/usr/share/doc/libopenjpeg5/copyright`)

- `BSD-2`
- `BSD-3`
- `Expat`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris openjpeg=1:1.5.2-3.1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openjpeg/openjpeg_1.5.2-3.1.dsc' openjpeg_1.5.2-3.1.dsc 2723 SHA256:1773f1326e2953b27b3eaf7cf74e37b245fda8369d3dc661acab8d93c523a51a
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openjpeg/openjpeg_1.5.2.orig.tar.gz' openjpeg_1.5.2.orig.tar.gz 615450 SHA256:aef498a293b4e75fa1ca8e367c3f32ed08e028d3557b069bf8584d0c1346026d
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openjpeg/openjpeg_1.5.2-3.1.debian.tar.xz' openjpeg_1.5.2-3.1.debian.tar.xz 18660 SHA256:c45f580c9dbdeffe9bc0e1f4f5c69b7a661568771339424690c81e138b973285
```

### `dpkg` source package: `openssl=1.0.2g-1ubuntu4.15`

Binary Packages:

- `libssl1.0.0:amd64=1.0.2g-1ubuntu4.15`
- `openssl=1.0.2g-1ubuntu4.15`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.0.2g-1ubuntu4.15
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g-1ubuntu4.15.dsc' openssl_1.0.2g-1ubuntu4.15.dsc 2453 SHA256:ff8e7bcf4868194e772058bad83030503b5f5a6e29b37e3c4edc04458baa32ba
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g.orig.tar.gz' openssl_1.0.2g.orig.tar.gz 5266102 SHA256:b784b1b3907ce39abf4098702dade6365522a253ad1552e267a9a0e89594aa33
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.0.2g-1ubuntu4.15.debian.tar.xz' openssl_1.0.2g-1ubuntu4.15.debian.tar.xz 130548 SHA256:b83195e7974b691b35be072451b153b29f520c6ffc025e7a4f2d4d8851235b8c
```

### `dpkg` source package: `opus=1.1.2-1ubuntu1`

Binary Packages:

- `libopus0:amd64=1.1.2-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris opus=1.1.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/opus/opus_1.1.2-1ubuntu1.dsc' opus_1.1.2-1ubuntu1.dsc 1983 SHA256:8f8ccf72939b5c7923df4a189ca1d7a0dcf0cd5151e70b5623029c095c54849e
'http://archive.ubuntu.com/ubuntu/pool/main/o/opus/opus_1.1.2.orig.tar.gz' opus_1.1.2.orig.tar.gz 1012168 SHA256:7aaa84f06ec89cbf19d08c1dd1ceac965a11b28b3ff504cc52893f9be78eb5d1
'http://archive.ubuntu.com/ubuntu/pool/main/o/opus/opus_1.1.2-1ubuntu1.debian.tar.xz' opus_1.1.2-1ubuntu1.debian.tar.xz 5920 SHA256:d31fc55216fbda1a05ea6d59f43b71988a5b748c3d292f0297dc97e5585c9535
```

### `dpkg` source package: `orc=1:0.4.25-1`

Binary Packages:

- `liborc-0.4-0:amd64=1:0.4.25-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris orc=1:0.4.25-1
'http://archive.ubuntu.com/ubuntu/pool/main/o/orc/orc_0.4.25-1.dsc' orc_0.4.25-1.dsc 2394 SHA256:31c1f6430cb90b30e7f0b7c89195482c1daea388835faa92056c50accc72ec65
'http://archive.ubuntu.com/ubuntu/pool/main/o/orc/orc_0.4.25.orig.tar.xz' orc_0.4.25.orig.tar.xz 467184 SHA256:c1b1d54a58f26d483f0b3881538984789fe5d5460ab8fab74a1cacbd3d1c53d1
'http://archive.ubuntu.com/ubuntu/pool/main/o/orc/orc_0.4.25-1.debian.tar.xz' orc_0.4.25-1.debian.tar.xz 5044 SHA256:470827b05344905ca68af316e9835fbbd86d368aa7ee12c090a2ade91099b1cb
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

### `dpkg` source package: `pcre3=2:8.38-3.1`

Binary Packages:

- `libpcre3:amd64=2:8.38-3.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.38-3.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38-3.1.dsc' pcre3_8.38-3.1.dsc 2074 SHA256:6a46bc62c33198fe38257f0dddecb4c534825f8f066bf88f2a45ad935b879885
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38.orig.tar.gz' pcre3_8.38.orig.tar.gz 2053336 SHA256:9883e419c336c63b0cb5202b09537c140966d585e4d0da66147dc513da13e629
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.38-3.1.debian.tar.gz' pcre3_8.38-3.1.debian.tar.gz 32289 SHA256:9ee1b838c1de50cb5f6641016d0dd21b06f1038b9b7c3b1098e0a89b9c24b39f
```

### `dpkg` source package: `pcsc-lite=1.8.14-1ubuntu1.16.04.1`

Binary Packages:

- `libpcsclite1:amd64=1.8.14-1ubuntu1.16.04.1`

Licenses: (parsed from: `/usr/share/doc/libpcsclite1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris pcsc-lite=1.8.14-1ubuntu1.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcsc-lite/pcsc-lite_1.8.14-1ubuntu1.16.04.1.dsc' pcsc-lite_1.8.14-1ubuntu1.16.04.1.dsc 2320 SHA256:9018fd262c9fdc19dca2094978aeaa9916ee84b99819d6e301674123974b12b6
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcsc-lite/pcsc-lite_1.8.14.orig.tar.bz2' pcsc-lite_1.8.14.orig.tar.bz2 689197 SHA256:b91f97806042315a41f005e69529cb968621f73f2ddfbd1380111a175b02334e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcsc-lite/pcsc-lite_1.8.14-1ubuntu1.16.04.1.debian.tar.xz' pcsc-lite_1.8.14-1ubuntu1.16.04.1.debian.tar.xz 16128 SHA256:cf9ca73d9624a31ee0af9b6b7ca2a248716e9a1dc1e24f0dcf1f1708e1b89250
```

### `dpkg` source package: `perl=5.22.1-9ubuntu0.6`

Binary Packages:

- `perl-base=5.22.1-9ubuntu0.6`

Licenses: (parsed from: `/usr/share/doc/perl-base/copyright`)

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

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.33.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6-1.dsc' pixman_0.33.6-1.dsc 2085 SHA256:08e94c263c3cde1c841458512705fa6a52a78c8f48e31f0bf3a2ae8a518eb51e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6.orig.tar.gz' pixman_0.33.6.orig.tar.gz 878996 SHA256:4e1e72c0ed31d10944f304976e87e6c87b441c853713eeecf115e22c23d4b17d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pixman/pixman_0.33.6-1.diff.gz' pixman_0.33.6-1.diff.gz 315093 SHA256:f382e753698aa95fae9019128a4b463935695b4c906785397f3eaa04e05a06d5
```

### `dpkg` source package: `poppler-data=0.4.7-7`

Binary Packages:

- `poppler-data=0.4.7-7`

Licenses: (parsed from: `/usr/share/doc/poppler-data/copyright`)

- `BSD-3-cluase`
- `GPL-2`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris poppler-data=0.4.7-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.7-7.dsc' poppler-data_0.4.7-7.dsc 2001 SHA256:8e472a3a4fe898a25e783a79dc01095f3ba35c769ea172443706a697fe09ff6f
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.7.orig-ai0.tar.gz' poppler-data_0.4.7.orig-ai0.tar.gz 3515 SHA256:755a3a7cec6019b7cb6a7ac89828820e90d5105e66ebc2a7aacecacfb3ed4f1d
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.7.orig.tar.gz' poppler-data_0.4.7.orig.tar.gz 4182339 SHA256:e752b0d88a7aba54574152143e7bf76436a7ef51977c55d6bd9a48dccde3a7de
'http://archive.ubuntu.com/ubuntu/pool/main/p/poppler-data/poppler-data_0.4.7-7.debian.tar.xz' poppler-data_0.4.7-7.debian.tar.xz 9004 SHA256:98add8235ea1d8cf58b3828a5f19fd47016cbd72f137b7448076ecaded568274
```

### `dpkg` source package: `procps=2:3.3.10-4ubuntu2.4`

Binary Packages:

- `libprocps4:amd64=2:3.3.10-4ubuntu2.4`
- `procps=2:3.3.10-4ubuntu2.4`

Licenses: (parsed from: `/usr/share/doc/libprocps4/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.10-4ubuntu2.4
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10-4ubuntu2.4.dsc' procps_3.3.10-4ubuntu2.4.dsc 2243 SHA256:f7f14b0b818e21ad1f1f4be7fdedbd375b9c19b7f3ecf92a94f3bc4a1a625f5f
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10.orig.tar.xz' procps_3.3.10.orig.tar.xz 814816 SHA256:40a3d2b0489e057d85564f4f304083b24fc699b39ea828610183fb9f0a6ebe97
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.10-4ubuntu2.4.debian.tar.xz' procps_3.3.10-4ubuntu2.4.debian.tar.xz 44376 SHA256:99854cab3c75853ec70cdda95d09fc22ee431c828e16dcdb9a0feaf65a3f74d1
```

### `dpkg` source package: `pulseaudio=1:8.0-0ubuntu3.10`

Binary Packages:

- `libpulse0:amd64=1:8.0-0ubuntu3.10`

Licenses: (parsed from: `/usr/share/doc/libpulse0/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris pulseaudio=1:8.0-0ubuntu3.10
'http://archive.ubuntu.com/ubuntu/pool/main/p/pulseaudio/pulseaudio_8.0-0ubuntu3.10.dsc' pulseaudio_8.0-0ubuntu3.10.dsc 3636 SHA256:e6a14bd9e178bfcbca1e0ab3e60094565527735d099d2ef7a8f2bddb3a42f4b5
'http://archive.ubuntu.com/ubuntu/pool/main/p/pulseaudio/pulseaudio_8.0.orig.tar.xz' pulseaudio_8.0.orig.tar.xz 1517656 SHA256:690eefe28633466cfd1ab9d85ebfa9376f6b622deec6bfee5091ac9737cd1989
'http://archive.ubuntu.com/ubuntu/pool/main/p/pulseaudio/pulseaudio_8.0-0ubuntu3.10.debian.tar.xz' pulseaudio_8.0-0ubuntu3.10.debian.tar.xz 151208 SHA256:eedb80db434a98bca95c04f38d22844cbd61c5bac3f0a136bbb72af0e8fa8b68
```

### `dpkg` source package: `readline6=6.3-8ubuntu2`

Binary Packages:

- `libreadline6:amd64=6.3-8ubuntu2`
- `readline-common=6.3-8ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libreadline6/copyright`, `/usr/share/doc/readline-common/copyright`)

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

### `dpkg` source package: `s2tc=0~git20131104-1.1`

Binary Packages:

- `libtxc-dxtn-s2tc0:amd64=0~git20131104-1.1`

Licenses: (parsed from: `/usr/share/doc/libtxc-dxtn-s2tc0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris s2tc=0~git20131104-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/s2tc/s2tc_0~git20131104-1.1.dsc' s2tc_0~git20131104-1.1.dsc 2087 SHA256:ef6452f69326ce1eb552b7721fa9e30f443eaba0102772cbf3f79d1c80a2f1ef
'http://archive.ubuntu.com/ubuntu/pool/main/s/s2tc/s2tc_0~git20131104.orig.tar.gz' s2tc_0~git20131104.orig.tar.gz 1395382 SHA256:ebaf5f37f094c824438e4fc518bf80524d332e128db704148fd6f52806b1ceda
'http://archive.ubuntu.com/ubuntu/pool/main/s/s2tc/s2tc_0~git20131104-1.1.debian.tar.gz' s2tc_0~git20131104-1.1.debian.tar.gz 4273 SHA256:b42a114823014f0e3f2c1769f5701f400dd2be3ce0bd0a1dc52421fc0e4c9b55
```

### `dpkg` source package: `schroedinger=1.0.11-2.1build1`

Binary Packages:

- `libschroedinger-1.0-0:amd64=1.0.11-2.1build1`

Licenses: (parsed from: `/usr/share/doc/libschroedinger-1.0-0/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris schroedinger=1.0.11-2.1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/schroedinger/schroedinger_1.0.11-2.1build1.dsc' schroedinger_1.0.11-2.1build1.dsc 1653 SHA256:426cd30212a67a8088d8998c54cc67bb2ac0740256a57960bc14fadc3d97a8d7
'http://archive.ubuntu.com/ubuntu/pool/universe/s/schroedinger/schroedinger_1.0.11.orig.tar.gz' schroedinger_1.0.11.orig.tar.gz 1019247 SHA256:1e572a0735b92aca5746c4528f9bebd35aa0ccf8619b22fa2756137a8cc9f912
'http://archive.ubuntu.com/ubuntu/pool/universe/s/schroedinger/schroedinger_1.0.11-2.1build1.debian.tar.xz' schroedinger_1.0.11-2.1build1.debian.tar.xz 16252 SHA256:ade22a54ba77a9f8796487ef70f929abc5d7e4b527cba7c30f4765b5f7096a22
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

### `dpkg` source package: `sgml-base=1.26+nmu4ubuntu1`

Binary Packages:

- `sgml-base=1.26+nmu4ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sgml-base/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris sgml-base=1.26+nmu4ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.26+nmu4ubuntu1.dsc' sgml-base_1.26+nmu4ubuntu1.dsc 957 SHA256:0b11ab50b2c014793e6593f489f0a4dde796d351cab7520d9fa0629476982f00
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.26+nmu4ubuntu1.tar.gz' sgml-base_1.26+nmu4ubuntu1.tar.gz 12912 SHA256:93d99ea554da5fea0c8abe424042ba8237c86faebaa02976fb92db3d198a47b4
```

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

### `dpkg` source package: `shine=3.1.0-4`

Binary Packages:

- `libshine3:amd64=3.1.0-4`

Licenses: (parsed from: `/usr/share/doc/libshine3/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris shine=3.1.0-4
'http://archive.ubuntu.com/ubuntu/pool/universe/s/shine/shine_3.1.0-4.dsc' shine_3.1.0-4.dsc 2042 SHA256:7cad74f28cb19f376657dcbca40fd348a139b787b8cd8f6037fb76bae17f33c3
'http://archive.ubuntu.com/ubuntu/pool/universe/s/shine/shine_3.1.0.orig.tar.gz' shine_3.1.0.orig.tar.gz 1275236 SHA256:6c5310bda766b116ed2415d639a27e5e11040e068b4b2db6bd733333e620cb4f
'http://archive.ubuntu.com/ubuntu/pool/universe/s/shine/shine_3.1.0-4.debian.tar.xz' shine_3.1.0-4.debian.tar.xz 3472 SHA256:5fc56f00d6653fc9d33b6adf802ea20324ccec762f9c4e581e1ddffee0fdb1a4
```

### `dpkg` source package: `slang2=2.3.0-2ubuntu1.1`

Binary Packages:

- `libslang2:amd64=2.3.0-2ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/libslang2/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris slang2=2.3.0-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/slang2/slang2_2.3.0-2ubuntu1.1.dsc' slang2_2.3.0-2ubuntu1.1.dsc 2445 SHA256:4ad16e8d76bf7e345778ba121ca5174d72736d69c288f370ceaaac8cef557a83
'http://archive.ubuntu.com/ubuntu/pool/main/s/slang2/slang2_2.3.0.orig.tar.xz' slang2_2.3.0.orig.tar.xz 1250392 SHA256:cdd5b9582959b3afdae403ee6f4be9de8efc7e205e4a7de18c1a847ea5ef0472
'http://archive.ubuntu.com/ubuntu/pool/main/s/slang2/slang2_2.3.0-2ubuntu1.1.debian.tar.xz' slang2_2.3.0-2ubuntu1.1.debian.tar.xz 22868 SHA256:7f4edf5f0f656ef8386436c647f0c1a866fb14691970cda0e0d4e2875258bdc7
```

### `dpkg` source package: `snappy=1.1.3-2`

Binary Packages:

- `libsnappy1v5:amd64=1.1.3-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/snappy/1.1.3-2/


### `dpkg` source package: `speex=1.2~rc1.2-1ubuntu1`

Binary Packages:

- `libspeex1:amd64=1.2~rc1.2-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris speex=1.2~rc1.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/speex/speex_1.2~rc1.2-1ubuntu1.dsc' speex_1.2~rc1.2-1ubuntu1.dsc 2317 SHA256:09af27fb2d683424c30994a202ac2ddf6cc4b027ab4043097dee93e30296fbb7
'http://archive.ubuntu.com/ubuntu/pool/main/s/speex/speex_1.2~rc1.2.orig.tar.gz' speex_1.2~rc1.2.orig.tar.gz 1069339 SHA256:8320fb86a024dfe1b6a78a7d57bc2388e5f8cb7f2fa10c946db2704e1e5d2805
'http://archive.ubuntu.com/ubuntu/pool/main/s/speex/speex_1.2~rc1.2-1ubuntu1.diff.gz' speex_1.2~rc1.2-1ubuntu1.diff.gz 10290 SHA256:8058ab2ea9dc3c19d7fcdeab2c5e8838ba6b73ed2c7d3467407dcb51b049e05d
```

### `dpkg` source package: `sqlite3=3.11.0-1ubuntu1.3`

Binary Packages:

- `libsqlite3-0:amd64=3.11.0-1ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.11.0-1ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0-1ubuntu1.3.dsc' sqlite3_3.11.0-1ubuntu1.3.dsc 2609 SHA256:e01bda25539cd0ed16a8c03be7a7a0894bdc9201220feedea163aa56a9bf97e6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0.orig-www.tar.xz' sqlite3_3.11.0.orig-www.tar.xz 3135012 SHA256:99843a91a1da29cf07269df49b37b0cd8a75035a88aacdb1186f94a9a217bab3
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0.orig.tar.xz' sqlite3_3.11.0.orig.tar.xz 5122440 SHA256:79fb8800b8744337d5317270899a5a40612bb76f81517e131bf496c26b044490
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.11.0-1ubuntu1.3.debian.tar.xz' sqlite3_3.11.0-1ubuntu1.3.debian.tar.xz 38916 SHA256:27519465c095855423a0959c287f32e7d25bbaea1ef1bcc49a6d7f9187dd83e6
```

### `dpkg` source package: `systemd=229-4ubuntu21.23`

Binary Packages:

- `libsystemd0:amd64=229-4ubuntu21.23`
- `libudev1:amd64=229-4ubuntu21.23`
- `systemd=229-4ubuntu21.23`
- `systemd-sysv=229-4ubuntu21.23`

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
$ apt-get source -qq --print-uris systemd=229-4ubuntu21.23
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229-4ubuntu21.23.dsc' systemd_229-4ubuntu21.23.dsc 4610 SHA256:b39984f374bb4f913eb53aacc22135458325d1345d22b9ce941d09d250289c71
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229.orig.tar.gz' systemd_229.orig.tar.gz 4319173 SHA256:b51b0a48d1beb388d95bd6a98d62be05490335d4bb388aefecdcb576e91e0741
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_229-4ubuntu21.23.debian.tar.xz' systemd_229-4ubuntu21.23.debian.tar.xz 302036 SHA256:632fc97934fef2aad6665c3cf54abc973664847bd0bd97fba955398c96a2453e
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

### `dpkg` source package: `tbb=4.4~20151115-0ubuntu3`

Binary Packages:

- `libtbb2:amd64=4.4~20151115-0ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libtbb2/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris tbb=4.4~20151115-0ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tbb/tbb_4.4~20151115-0ubuntu3.dsc' tbb_4.4~20151115-0ubuntu3.dsc 2101 SHA256:f99cdc350c1c6e15576d03db78b3a8742bf6f4ef4c0c8d1e968c44f7f8f90e7d
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tbb/tbb_4.4~20151115.orig.tar.gz' tbb_4.4~20151115.orig.tar.gz 3029951 SHA256:3dd5c4fc85c18f49307d3cde4ce937bda230679f7fe2906112e5c8dee4cc77bb
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tbb/tbb_4.4~20151115-0ubuntu3.debian.tar.xz' tbb_4.4~20151115-0ubuntu3.debian.tar.xz 10056 SHA256:3882117671a997c930ad422e443ebe684b77c46c382a16333fb00d4e16ea83d4
```

### `dpkg` source package: `tcp-wrappers=7.6.q-25`

Binary Packages:

- `libwrap0:amd64=7.6.q-25`
- `tcpd=7.6.q-25`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcp-wrappers=7.6.q-25
'http://archive.ubuntu.com/ubuntu/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-25.dsc' tcp-wrappers_7.6.q-25.dsc 1132 SHA256:77e162fcb2fcbe34448cf445f10e746d417a61ec0d79f46fd8ac5883ffc720c7
'http://archive.ubuntu.com/ubuntu/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q.orig.tar.gz' tcp-wrappers_7.6.q.orig.tar.gz 99438 SHA256:9543d7adedf78a6de0b221ccbbd1952e08b5138717f4ade814039bb489a4315d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tcp-wrappers/tcp-wrappers_7.6.q-25.debian.tar.xz' tcp-wrappers_7.6.q-25.debian.tar.xz 35504 SHA256:fb7bb73c586a0c00c76c730ab93ffd73c300e8c4fd83df76222e305a2466c7bb
```

### `dpkg` source package: `tiff=4.0.6-1ubuntu0.7`

Binary Packages:

- `libtiff5:amd64=4.0.6-1ubuntu0.7`

Licenses: (parsed from: `/usr/share/doc/libtiff5/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.0.6-1ubuntu0.7
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6-1ubuntu0.7.dsc' tiff_4.0.6-1ubuntu0.7.dsc 2399 SHA256:93e01b61c5e12478dd640d88b820ba68bbfa7fcf5aad1a0c6e14360b5491e3b8
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6.orig.tar.gz' tiff_4.0.6.orig.tar.gz 2192991 SHA256:4d57a50907b510e3049a4bba0d7888930fdfc16ce49f1bf693e5b6247370d68c
'http://archive.ubuntu.com/ubuntu/pool/main/t/tiff/tiff_4.0.6-1ubuntu0.7.debian.tar.xz' tiff_4.0.6-1ubuntu0.7.debian.tar.xz 63940 SHA256:469b5e0dbc6de4395ce1085583099533c15690fd5135b0475dda50c4c149388c
```

### `dpkg` source package: `twolame=0.3.13-1.2`

Binary Packages:

- `libtwolame0:amd64=0.3.13-1.2`

Licenses: (parsed from: `/usr/share/doc/libtwolame0/copyright`)

- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris twolame=0.3.13-1.2
'http://archive.ubuntu.com/ubuntu/pool/universe/t/twolame/twolame_0.3.13-1.2.dsc' twolame_0.3.13-1.2.dsc 1942 SHA256:39c3844a32217631ea90dfee409d43f48b0152466c0d657976b5a5d3a792c35d
'http://archive.ubuntu.com/ubuntu/pool/universe/t/twolame/twolame_0.3.13.orig.tar.gz' twolame_0.3.13.orig.tar.gz 660415 SHA256:98f332f48951f47f23f70fd0379463aff7d7fb26f07e1e24e42ddef22cc6112a
'http://archive.ubuntu.com/ubuntu/pool/universe/t/twolame/twolame_0.3.13-1.2.diff.gz' twolame_0.3.13-1.2.diff.gz 4432 SHA256:a98313a8238c99f6a3b1fd280f2be62cd0fdfe1c2fffcb8bd7d2544141927470
```

### `dpkg` source package: `ubuntu-keyring=2012.05.19`

Binary Packages:

- `ubuntu-keyring=2012.05.19`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2012.05.19
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2012.05.19.dsc' ubuntu-keyring_2012.05.19.dsc 1542 SHA256:a98138a8ef99905330f7f1340d04f8a9104c8706243e4c694b46db7d11c89d16
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2012.05.19.tar.gz' ubuntu-keyring_2012.05.19.tar.gz 18495 SHA256:8b3bb00770c7b1e5c0abb215ecf8c383cb3b709292a52aeb1022b5556e768b69
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

### `dpkg` source package: `util-linux=2.27.1-6ubuntu3.9`

Binary Packages:

- `bsdutils=1:2.27.1-6ubuntu3.9`
- `libblkid1:amd64=2.27.1-6ubuntu3.9`
- `libfdisk1:amd64=2.27.1-6ubuntu3.9`
- `libmount1:amd64=2.27.1-6ubuntu3.9`
- `libsmartcols1:amd64=2.27.1-6ubuntu3.9`
- `libuuid1:amd64=2.27.1-6ubuntu3.9`
- `mount=2.27.1-6ubuntu3.9`
- `util-linux=2.27.1-6ubuntu3.9`

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
$ apt-get source -qq --print-uris util-linux=2.27.1-6ubuntu3.9
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1-6ubuntu3.9.dsc' util-linux_2.27.1-6ubuntu3.9.dsc 3586 SHA256:184c6e918aab02046b1f8769e488013a4da2c59d9108123447ead31ee9270d72
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1.orig.tar.xz' util-linux_2.27.1.orig.tar.xz 3964512 SHA256:0a818fcdede99aec43ffe6ca5b5388bff80d162f2f7bd4541dca94fecb87a290
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.27.1-6ubuntu3.9.debian.tar.xz' util-linux_2.27.1-6ubuntu3.9.debian.tar.xz 88260 SHA256:6d82ba9a363e1c5aa96b8ee964808d5678bb1749547bc173a701e70082e223bd
```

### `dpkg` source package: `wavpack=4.75.2-2ubuntu0.2`

Binary Packages:

- `libwavpack1:amd64=4.75.2-2ubuntu0.2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris wavpack=4.75.2-2ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/w/wavpack/wavpack_4.75.2-2ubuntu0.2.dsc' wavpack_4.75.2-2ubuntu0.2.dsc 2230 SHA256:4f9feec761d8821e8dfe0960ed243a517617d70d805fad1099a6292937e1aa08
'http://archive.ubuntu.com/ubuntu/pool/main/w/wavpack/wavpack_4.75.2.orig.tar.bz2' wavpack_4.75.2.orig.tar.bz2 439798 SHA256:7d31b34166c33c3109b45c6e4579b472fd05e3ee8ec6d728352961c5cdd1d6b0
'http://archive.ubuntu.com/ubuntu/pool/main/w/wavpack/wavpack_4.75.2-2ubuntu0.2.debian.tar.xz' wavpack_4.75.2-2ubuntu0.2.debian.tar.xz 6932 SHA256:78c0d6d7dd4bb8c158c18b67c9ed4ab5bd779f662db00a4b6bfb9cd7d5b558dd
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

### `dpkg` source package: `x264=2:0.148.2643+git5c65704-1`

Binary Packages:

- `libx264-148:amd64=2:0.148.2643+git5c65704-1`

Licenses: (parsed from: `/usr/share/doc/libx264-148/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with other exception`
- `ISC`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris x264=2:0.148.2643+git5c65704-1
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x264/x264_0.148.2643+git5c65704-1.dsc' x264_0.148.2643+git5c65704-1.dsc 2431 SHA256:e5356f684c004c090443b51b642be73e27047dab584bdd74e8ccb5851bbb171b
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x264/x264_0.148.2643+git5c65704.orig.tar.gz' x264_0.148.2643+git5c65704.orig.tar.gz 884605 SHA256:a2dfed165837bf901652a8f13f06ff2e2bba72fb729dee0faaafb791efa4f319
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x264/x264_0.148.2643+git5c65704-1.debian.tar.xz' x264_0.148.2643+git5c65704-1.debian.tar.xz 22548 SHA256:9d1ee42fc46701d3613bb4eb12162e20e390d6719183bb93754c06d53a6a022b
```

### `dpkg` source package: `x265=1.9-3`

Binary Packages:

- `libx265-79:amd64=1.9-3`

Licenses: (parsed from: `/usr/share/doc/libx265-79/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris x265=1.9-3
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_1.9-3.dsc' x265_1.9-3.dsc 2188 SHA256:2c92827504e3b7486d46dd7ec559495dc1664457914a1c756f16b8d0d7b9c070
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_1.9.orig.tar.gz' x265_1.9.orig.tar.gz 956101 SHA256:3e4654133ed957a98708fdb4cb9a154d9e80922b84e26e43fc462a101c5b15c8
'http://archive.ubuntu.com/ubuntu/pool/universe/x/x265/x265_1.9-3.debian.tar.xz' x265_1.9-3.debian.tar.xz 9744 SHA256:a1c184c22f212222581dcd3174ad91564696f9ca601e2b4dfa0b4dd0461815e3
```

### `dpkg` source package: `xdg-user-dirs=0.15-2ubuntu6.16.04.1`

Binary Packages:

- `xdg-user-dirs=0.15-2ubuntu6.16.04.1`

Licenses: (parsed from: `/usr/share/doc/xdg-user-dirs/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xdg-user-dirs=0.15-2ubuntu6.16.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.15-2ubuntu6.16.04.1.dsc' xdg-user-dirs_0.15-2ubuntu6.16.04.1.dsc 2285 SHA256:a106cbc2b9b24cbd39f5163899b024dd7554aa48782c2b5c634f8fc74be4f874
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.15.orig.tar.gz' xdg-user-dirs_0.15.orig.tar.gz 243747 SHA256:20b4a751f41d0554bce3e0ce5e8d934be98cc62d48f0b90a894c3e1916552786
'http://archive.ubuntu.com/ubuntu/pool/main/x/xdg-user-dirs/xdg-user-dirs_0.15-2ubuntu6.16.04.1.debian.tar.xz' xdg-user-dirs_0.15-2ubuntu6.16.04.1.debian.tar.xz 28440 SHA256:8d5c9a79d6ad03f7e14fce382f88dcdd087395ccd0653fbd657e37291be2f8da
```

### `dpkg` source package: `xml-core=0.13+nmu2`

Binary Packages:

- `xml-core=0.13+nmu2`

Licenses: (parsed from: `/usr/share/doc/xml-core/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xml-core=0.13+nmu2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.13+nmu2.dsc' xml-core_0.13+nmu2.dsc 1738 SHA256:edf913f3aee9865480143bdd91f5f6a0838ca61ddc8674ea316e48a22d65fecb
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.13+nmu2.tar.gz' xml-core_0.13+nmu2.tar.gz 23436 SHA256:cd3f5402265a9ab0e7e4a6efafdc5eb9cb02d33c3e75d1ff1ecb0ac0899e242b
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

### `dpkg` source package: `xvidcore=2:1.3.4-1`

Binary Packages:

- `libxvidcore4:amd64=2:1.3.4-1`

Licenses: (parsed from: `/usr/share/doc/libxvidcore4/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xvidcore=2:1.3.4-1
'http://archive.ubuntu.com/ubuntu/pool/universe/x/xvidcore/xvidcore_1.3.4-1.dsc' xvidcore_1.3.4-1.dsc 2125 SHA256:8443f4a4c4b3608ea72e15e1c8613f62f83ea6d0b271483dec74f4cec06d0819
'http://archive.ubuntu.com/ubuntu/pool/universe/x/xvidcore/xvidcore_1.3.4.orig.tar.gz' xvidcore_1.3.4.orig.tar.gz 818067 SHA256:4e9fd62728885855bc5007fe1be58df42e5e274497591fec37249e1052ae316f
'http://archive.ubuntu.com/ubuntu/pool/universe/x/xvidcore/xvidcore_1.3.4-1.debian.tar.xz' xvidcore_1.3.4-1.debian.tar.xz 6056 SHA256:7371066d81e0819c586aeab2f1188c6e57da64dc70d9e582e885c5ccb8f7f5aa
```

### `dpkg` source package: `xz-utils=5.1.1alpha+20120614-2ubuntu2`

Binary Packages:

- `liblzma5:amd64=5.1.1alpha+20120614-2ubuntu2`

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
$ apt-get source -qq --print-uris xz-utils=5.1.1alpha+20120614-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2ubuntu2.dsc' xz-utils_5.1.1alpha+20120614-2ubuntu2.dsc 2409 SHA256:0a8cb3d928d1327f70b998b713c10afd9cd064056f5973d48075cd3d0f7872ca
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614.orig.tar.gz' xz-utils_5.1.1alpha+20120614.orig.tar.gz 556454 SHA256:b168e63400db449a6e7b3a06e668f557ca27e3d70accbd29d2b5a98e15c00fee
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.1.1alpha+20120614-2ubuntu2.debian.tar.gz' xz-utils_5.1.1alpha+20120614-2ubuntu2.debian.tar.gz 156001 SHA256:e7743d4a96276ccffc4e171812e402a1f503f87df3b668ef0e58db6629146a18
```

### `dpkg` source package: `zeromq3=4.1.4-7ubuntu0.1`

Binary Packages:

- `libzmq5:amd64=4.1.4-7ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/libzmq5/copyright`)

- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-3`
- `LGPL-3.0+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris zeromq3=4.1.4-7ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zeromq3/zeromq3_4.1.4-7ubuntu0.1.dsc' zeromq3_4.1.4-7ubuntu0.1.dsc 2127 SHA256:d0ce166f7976b7b29bc84182c38caf82d0fdf1004b9c6cfca029dc2875111fc6
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zeromq3/zeromq3_4.1.4.orig.tar.gz' zeromq3_4.1.4.orig.tar.gz 1400012 SHA256:e99f44fde25c2e4cb84ce440f87ca7d3fe3271c2b8cfbc67d55e4de25e6fe378
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zeromq3/zeromq3_4.1.4-7ubuntu0.1.debian.tar.xz' zeromq3_4.1.4-7ubuntu0.1.debian.tar.xz 15184 SHA256:b4bbb4553c441a20051feb0f4da08efaaa9043f37f303104d11b4ea1e6b07105
```

### `dpkg` source package: `zip=3.0-11`

Binary Packages:

- `zip=3.0-11`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zip=3.0-11
'http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0-11.dsc' zip_3.0-11.dsc 1306 SHA256:9f7df6a4276dfc79cfc8c49212d702965cef18e3f5433fba70b72577946e7604
'http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0.orig.tar.gz' zip_3.0.orig.tar.gz 1118845 SHA256:f0e8bb1f9b7eb0b01285495a2699df3a4b766784c1765a8f1aeedf63c0806369
'http://archive.ubuntu.com/ubuntu/pool/main/z/zip/zip_3.0-11.debian.tar.xz' zip_3.0-11.debian.tar.xz 8260 SHA256:c5c0714a88592f9e02146bfe4a8d26cd9bd97e8d33b1efc8b37784997caa40ed
```

### `dpkg` source package: `zlib=1:1.2.8.dfsg-2ubuntu4.1`

Binary Packages:

- `zlib1g:amd64=1:1.2.8.dfsg-2ubuntu4.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `zvbi=0.2.35-10`

Binary Packages:

- `libzvbi-common=0.2.35-10`
- `libzvbi0:amd64=0.2.35-10`

Licenses: (parsed from: `/usr/share/doc/libzvbi-common/copyright`, `/usr/share/doc/libzvbi0/copyright`)

- `BSD-2-Clause`
- `BSD-3-Clause`
- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris zvbi=0.2.35-10
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zvbi/zvbi_0.2.35-10.dsc' zvbi_0.2.35-10.dsc 2095 SHA256:729f1e3ff9cbfde94a85f2edb5121257731f6f8deb307c8a7eccf56e74a18753
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zvbi/zvbi_0.2.35.orig.tar.bz2' zvbi_0.2.35.orig.tar.bz2 1047761 SHA256:fc883c34111a487c4a783f91b1b2bb5610d8d8e58dcba80c7ab31e67e4765318
'http://archive.ubuntu.com/ubuntu/pool/universe/z/zvbi/zvbi_0.2.35-10.debian.tar.xz' zvbi_0.2.35-10.debian.tar.xz 14364 SHA256:8ceb1fa8a19403b5b7eeadd65379140b697e0b474ca80a013f43f5a2c8d49fa2
```
