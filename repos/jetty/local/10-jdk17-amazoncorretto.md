# `jetty:10.0.18-jdk17-amazoncorretto`

## Docker Metadata

- Image ID: `sha256:2b3f46eeacb46d2662851c8966b286bebf516c31ca638887a77b4569b07d89a2`
- Created: `2023-11-21T05:08:13.697216714Z`
- Virtual Size: ~ 494.17 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
- Command: `["java","-jar","/usr/local/jetty/start.jar"]`
- Environment:
  - `PATH=/usr/local/jetty/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto`
  - `JETTY_VERSION=10.0.18`
  - `JETTY_HOME=/usr/local/jetty`
  - `JETTY_BASE=/var/lib/jetty`
  - `TMPDIR=/tmp/jetty`
  - `JETTY_TGZ_URL=https://repo1.maven.org/maven2/org/eclipse/jetty/jetty-home/10.0.18/jetty-home-10.0.18.tar.gz`
  - `JETTY_GPG_KEYS=AED5EE6C45D0FE8D5D1B164F27DED4BF6216DB8F 	2A684B57436A81FA8706B53C61C3351A438A3B7D 	5989BAF76217B843D66BE55B2D0E1FB8FE4B68B4 	B59B67FD7904984367F931800818D9D68FB67BAC 	BFBB21C246D7776836287A48A04E0C74ABB35FEA 	8B096546B1A8F02656B15D3B1677D141BCF3584D 	F254B35617DC255D9344BCFA873A8E86B4372146 	E22488CC94F63E3FC928536C4241C08270D999C3`

## `rpm` (`.rpm`-based packages)

### `rpm` package: `amazon-linux-extras-2.0.3-1.amzn2.noarch`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url amazon-linux-extras-2.0.3-1.amzn2.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/c8391609150db76aac95144697183fcaff68c7b05fb74b19e1b4f42af0bf158a/amazon-linux-extras-2.0.3-1.amzn2.src.rpm
```

### `rpm` package: `audit-libs-2.8.1-3.amzn2.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url audit-libs-2.8.1-3.amzn2.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/6af950cd493703410c3c041e3343bf1618b94f4f5a2e72976d8ab1d31f625871/audit-2.8.1-3.amzn2.1.src.rpm
```

### `rpm` package: `basesystem-10.0-7.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url basesystem-10.0-7.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/303ffc769b33bd06f7d3c5d0a1999079ad5afb6d205448dd607a8b6a5cbc3551/basesystem-10.0-7.amzn2.0.1.src.rpm
```

### `rpm` package: `bash-4.2.46-34.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url bash-4.2.46-34.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/088b4acd2aa66aac9479237b6c06724ef38173941734da6a81fb28add6418143/bash-4.2.46-34.amzn2.src.rpm
```

### `rpm` package: `bzip2-libs-1.0.6-13.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url bzip2-libs-1.0.6-13.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/5eb7c8b4ed1b326f5e640d655f92f498451c8013b223ad5702abb108358ef0dc/bzip2-1.0.6-13.amzn2.0.3.src.rpm
```

### `rpm` package: `ca-certificates-2023.2.62-1.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url ca-certificates-2023.2.62-1.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/76a982dd256319dafe3f5aad3aac01edbd5e1d97168ee2e2e8e966fb21bbab20/ca-certificates-2023.2.62-1.amzn2.0.1.src.rpm
```

### `rpm` package: `chkconfig-1.7.4-1.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url chkconfig-1.7.4-1.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/227e42c03e4cdcc55a1851cfe633f2a280cb53eea907a581d95422575f584465/chkconfig-1.7.4-1.amzn2.0.2.src.rpm
```

### `rpm` package: `coreutils-8.22-24.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url coreutils-8.22-24.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/7785c3a49bafaa745c01233429d6dab66539416864de241fb29aea434a29dcb2/coreutils-8.22-24.amzn2.src.rpm
```

### `rpm` package: `cpio-2.12-11.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url cpio-2.12-11.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/ca1a6751af62fcada1d385ffd948fc81d14914d786602012ecd1f902c558d804/cpio-2.12-11.amzn2.src.rpm
```

### `rpm` package: `curl-8.3.0-1.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): curl

Source:

```console
$ dnf --quiet download --source --url curl-8.3.0-1.amzn2.0.4
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/90a58bc134a570402f9393e9e273243cc9032ed5e104355e06a8342c00df1c9d/curl-8.3.0-1.amzn2.0.4.src.rpm
```

### `rpm` package: `cyrus-sasl-lib-2.1.26-24.amzn2.x86_64`

Licenses (from `rpm --query`): BSD with advertising

Source:

```console
$ dnf --quiet download --source --url cyrus-sasl-lib-2.1.26-24.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/3d9de0f7ecb9ee20cf3eeccde9bd3f335ba6aa86b07f1fb45c6d7fdb7edf854a/cyrus-sasl-2.1.26-24.amzn2.src.rpm
```

### `rpm` package: `dejavu-fonts-common-2.33-6.amzn2.noarch`

Licenses (from `rpm --query`): Bitstream Vera and Public Domain

Source:

```console
$ dnf --quiet download --source --url dejavu-fonts-common-2.33-6.amzn2.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2c78ae75ee92a19e0ecbd2d6f1b1e6c343e2c8357057617fb7a03438fcff9ce0/dejavu-fonts-2.33-6.amzn2.src.rpm
```

### `rpm` package: `dejavu-sans-fonts-2.33-6.amzn2.noarch`

Licenses (from `rpm --query`): Bitstream Vera and Public Domain

Source:

```console
$ dnf --quiet download --source --url dejavu-sans-fonts-2.33-6.amzn2.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2c78ae75ee92a19e0ecbd2d6f1b1e6c343e2c8357057617fb7a03438fcff9ce0/dejavu-fonts-2.33-6.amzn2.src.rpm
```

### `rpm` package: `diffutils-3.3-5.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url diffutils-3.3-5.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/3b94189bd4a0bbb334c887b5a7306f5cbe927e45ca9a9c1e68e6466570b7a4e1/diffutils-3.3-5.amzn2.src.rpm
```

### `rpm` package: `elfutils-libelf-0.176-2.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2+ or LGPLv3+

Source:

```console
$ dnf --quiet download --source --url elfutils-libelf-0.176-2.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/1c91483c986f8c6728684f387c271636212f24068e329c1b81b7502fdeeadddc/elfutils-0.176-2.amzn2.0.2.src.rpm
```

### `rpm` package: `expat-2.1.0-15.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url expat-2.1.0-15.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/f9f984ab3675d0250695e8a67360d02f8a0182b40281dd92bf16e8add1919080/expat-2.1.0-15.amzn2.0.3.src.rpm
```

### `rpm` package: `file-libs-5.11-36.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url file-libs-5.11-36.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/6826885873bb4ef8f4d7479ffbfbceb96807ae298e2f0a9a083022200ca7caab/file-5.11-36.amzn2.0.1.src.rpm
```

### `rpm` package: `filesystem-3.2-25.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url filesystem-3.2-25.amzn2.0.4
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/c1bdb520a838326c15c1c86b0a1314c9e44f7689de956010d7a8e4bfda7d34e4/filesystem-3.2-25.amzn2.0.4.src.rpm
```

### `rpm` package: `findutils-4.5.11-6.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url findutils-4.5.11-6.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/8cb38ddd3353da1ca38e2748e4affeb61a422044bf26c05f93cd0e20d83b125d/findutils-4.5.11-6.amzn2.src.rpm
```

### `rpm` package: `fontconfig-2.13.0-4.3.amzn2.x86_64`

Licenses (from `rpm --query`): MIT and Public Domain and UCD

Source:

```console
$ dnf --quiet download --source --url fontconfig-2.13.0-4.3.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/d27fa964cbcbbd78a2cd17349b255f37d6fa44876c0186ffd4b05c63d6aae827/fontconfig-2.13.0-4.3.amzn2.src.rpm
```

### `rpm` package: `fontpackages-filesystem-1.44-8.amzn2.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url fontpackages-filesystem-1.44-8.amzn2.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/a7c49b56992c5deec79f1d6b1cadaf4a1210c7f5cefea9dab4b353e83eeb6ab5/fontpackages-1.44-8.amzn2.src.rpm
```

### `rpm` package: `freetype-2.8-14.amzn2.1.1.x86_64`

Licenses (from `rpm --query`): (FTL or GPLv2+) and BSD and MIT and Public Domain and zlib with acknowledgement

Source:

```console
$ dnf --quiet download --source --url freetype-2.8-14.amzn2.1.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/49d4e4f35ea19b5e24bb1aabbb6216c9b6c2bc4a317956302a2ad197940109d6/freetype-2.8-14.amzn2.1.1.src.rpm
```

### `rpm` package: `gawk-4.0.2-4.amzn2.1.2.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPL and LGPLv3+ and LGPL and BSD

Source:

```console
$ dnf --quiet download --source --url gawk-4.0.2-4.amzn2.1.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/20e168961dd7975b2be268b247219eb2e7a1bef49898ad360ffae2833d76ad1c/gawk-4.0.2-4.amzn2.1.2.src.rpm
```

### `rpm` package: `gdbm-1.13-6.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url gdbm-1.13-6.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/e2866f1817e24bcd350768bf85c8bbddde135513ced29ce315df75f311cf77cf/gdbm-1.13-6.amzn2.0.2.src.rpm
```

### `rpm` package: `glib2-2.56.1-9.amzn2.0.6.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url glib2-2.56.1-9.amzn2.0.6
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/383633f7414eced43358510e6a9cff461e44af8b8d659366b89c1f8df511a4d0/glib2-2.56.1-9.amzn2.0.6.src.rpm
```

### `rpm` package: `glibc-2.26-63.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ dnf --quiet download --source --url glibc-2.26-63.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/f53018ac2b4485b5fa03d1b20cfc6fabdfe74c05b38d166c31c886140b157094/glibc-2.26-63.amzn2.0.1.src.rpm
```

### `rpm` package: `glibc-common-2.26-63.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ dnf --quiet download --source --url glibc-common-2.26-63.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/f53018ac2b4485b5fa03d1b20cfc6fabdfe74c05b38d166c31c886140b157094/glibc-2.26-63.amzn2.0.1.src.rpm
```

### `rpm` package: `glibc-langpack-en-2.26-63.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ dnf --quiet download --source --url glibc-langpack-en-2.26-63.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/f53018ac2b4485b5fa03d1b20cfc6fabdfe74c05b38d166c31c886140b157094/glibc-2.26-63.amzn2.0.1.src.rpm
```

### `rpm` package: `glibc-minimal-langpack-2.26-63.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ dnf --quiet download --source --url glibc-minimal-langpack-2.26-63.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/f53018ac2b4485b5fa03d1b20cfc6fabdfe74c05b38d166c31c886140b157094/glibc-2.26-63.amzn2.0.1.src.rpm
```

### `rpm` package: `gmp-6.0.0-15.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv3+ or GPLv2+

Source:

```console
$ dnf --quiet download --source --url gmp-6.0.0-15.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/712fffd161eb394310f7fe5f7d41ae2aae07cdcce27ca119bf04c6f056eb2b4d/gmp-6.0.0-15.amzn2.0.2.src.rpm
```

### `rpm` package: `gnupg2-2.0.22-5.amzn2.0.5.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url gnupg2-2.0.22-5.amzn2.0.5
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/189e1bdc950a8e13918173d73835981842c90ee3b3cef07c116152a00b8b8a59/gnupg2-2.0.22-5.amzn2.0.5.src.rpm
```

### `rpm` package: `gpg-pubkey-b04f24e3-5de94a19`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `gpg-pubkey-c87f5b1a-593863f8`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `gpgme-1.3.2-5.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url gpgme-1.3.2-5.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/81074517b77553b2abbdc13fb0637c599a4c32f25ff85e6e00a9761fbd961d9f/gpgme-1.3.2-5.amzn2.0.2.src.rpm
```

### `rpm` package: `grep-2.20-3.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url grep-2.20-3.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/6a1fd83c54bc7f4701e6b979d8f5dcc9950e2b5116cbb1c27057f412bed54390/grep-2.20-3.amzn2.0.2.src.rpm
```

### `rpm` package: `gzip-1.5-10.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GFDL

Source:

```console
$ dnf --quiet download --source --url gzip-1.5-10.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/073c2dbe9b6abb1bfeb13882372463c92385805502ccf659e093c5d4b2c3d62e/gzip-1.5-10.amzn2.0.1.src.rpm
```

### `rpm` package: `info-5.1-5.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url info-5.1-5.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/968c079ef8a8a2efee76ff59cd99e06dd242b8813960171d0f5c23f4a6eb0bb2/texinfo-5.1-5.amzn2.src.rpm
```

### `rpm` package: `java-17-amazon-corretto-devel-17.0.9.8-1.x86_64`

Licenses (from `rpm --query`): ASL 1.1 and ASL 2.0 and BSD and BSD with advertising and GPL+ and GPLv2 and GPLv2 with exceptions and IJG and LGPLv2+ and MIT and MPLv2.0 and Public Domain and W3C and zlib and ISC and FTL and RSA.

**WARNING:** unable to find source (`dnf download` failed or returned no results)!

### `rpm` package: `keyutils-libs-1.5.8-3.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+

Source:

```console
$ dnf --quiet download --source --url keyutils-libs-1.5.8-3.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/1579dc52bd90d64e68d663da4dfa4462afa9df1cfbef30d47b64add0dd12210e/keyutils-1.5.8-3.amzn2.0.2.src.rpm
```

### `rpm` package: `krb5-libs-1.15.1-55.amzn2.2.6.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url krb5-libs-1.15.1-55.amzn2.2.6
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/15723437f24b376f52ea3f75ed5fb759008fa7e44fe468838f9796e0d09bd393/krb5-1.15.1-55.amzn2.2.6.src.rpm
```

### `rpm` package: `libacl-2.2.51-14.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libacl-2.2.51-14.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/d21969f8fbccf539fa601961f20352b7c95b4cf593c9fa5dad2ac4896c7ca6c9/acl-2.2.51-14.amzn2.src.rpm
```

### `rpm` package: `libassuan-2.1.0-3.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and GPLv3+

Source:

```console
$ dnf --quiet download --source --url libassuan-2.1.0-3.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/27b0138d028a9ba30c43384ce6b2d1314d0ac3a6284c6793655c5589893d47ee/libassuan-2.1.0-3.amzn2.0.2.src.rpm
```

### `rpm` package: `libattr-2.4.46-12.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libattr-2.4.46-12.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/370b7813e0e86fadc241a9fb590451372429f0fe3ab17d62a4378b49089f8158/attr-2.4.46-12.amzn2.0.2.src.rpm
```

### `rpm` package: `libblkid-2.30.2-2.amzn2.0.11.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libblkid-2.30.2-2.amzn2.0.11
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/c3d8b01e2190e686623eb8551a13a4a33cc08e086036e951fe5ed1b99c7b2b8e/util-linux-2.30.2-2.amzn2.0.11.src.rpm
```

### `rpm` package: `libcap-2.54-1.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): BSD or GPLv2

Source:

```console
$ dnf --quiet download --source --url libcap-2.54-1.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/ab5e39e42f4b1dd512a49eb9ca2c71cebf3647d3f63d147f5b20e7229596ba54/libcap-2.54-1.amzn2.0.2.src.rpm
```

### `rpm` package: `libcap-ng-0.7.5-4.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libcap-ng-0.7.5-4.amzn2.0.4
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/b9685dfd18da9e00613cda24f60b48a09e3b4695dd6131e5e4ce4de70b90e95c/libcap-ng-0.7.5-4.amzn2.0.4.src.rpm
```

### `rpm` package: `libcom_err-1.42.9-19.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libcom_err-1.42.9-19.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/cdaf4c4c0124e55017cfd1c72a24450c9b0652ba3dab8a3dc9b49c120d634f76/e2fsprogs-1.42.9-19.amzn2.0.1.src.rpm
```

### `rpm` package: `libcrypt-2.26-63.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ dnf --quiet download --source --url libcrypt-2.26-63.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/f53018ac2b4485b5fa03d1b20cfc6fabdfe74c05b38d166c31c886140b157094/glibc-2.26-63.amzn2.0.1.src.rpm
```

### `rpm` package: `libcurl-8.3.0-1.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): curl

Source:

```console
$ dnf --quiet download --source --url libcurl-8.3.0-1.amzn2.0.4
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/90a58bc134a570402f9393e9e273243cc9032ed5e104355e06a8342c00df1c9d/curl-8.3.0-1.amzn2.0.4.src.rpm
```

### `rpm` package: `libdb-5.3.21-24.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): BSD and LGPLv2 and Sleepycat

Source:

```console
$ dnf --quiet download --source --url libdb-5.3.21-24.amzn2.0.4
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/5ab6c29aa2ef7ba0ab2454c9bb280a713bceeb3f2307b219a53ae8bed53b7283/libdb-5.3.21-24.amzn2.0.4.src.rpm
```

### `rpm` package: `libdb-utils-5.3.21-24.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): BSD and LGPLv2 and Sleepycat

Source:

```console
$ dnf --quiet download --source --url libdb-utils-5.3.21-24.amzn2.0.4
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/5ab6c29aa2ef7ba0ab2454c9bb280a713bceeb3f2307b219a53ae8bed53b7283/libdb-5.3.21-24.amzn2.0.4.src.rpm
```

### `rpm` package: `libffi-3.0.13-18.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT and Public Domain

Source:

```console
$ dnf --quiet download --source --url libffi-3.0.13-18.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/6d795273d9b8725efa8069ecb46398043d7100cfd4979b9c31489e35504e31f7/libffi-3.0.13-18.amzn2.0.2.src.rpm
```

### `rpm` package: `libgcc-7.3.1-17.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv3+ with exceptions and GPLv2+ with exceptions and LGPLv2+ and BSD

Source:

```console
$ dnf --quiet download --source --url libgcc-7.3.1-17.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/a2b874b1e83eb065848df3e26205c7e903eb46b4c4f40adf7a6a68a1af38698f/gcc-7.3.1-17.amzn2.src.rpm
```

### `rpm` package: `libgcrypt-1.5.3-14.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libgcrypt-1.5.3-14.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/86f0a2bd76acd4f1460e1e52a2d34502480808da4e76a2a1bf835dba805b5d21/libgcrypt-1.5.3-14.amzn2.0.3.src.rpm
```

### `rpm` package: `libgpg-error-1.12-3.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libgpg-error-1.12-3.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/997de9d51396f20df5b00b7f41a4bc110b88c5243225ff5941026174850a6e6e/libgpg-error-1.12-3.amzn2.0.3.src.rpm
```

### `rpm` package: `libidn2-2.3.0-1.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): (GPLv2+ or LGPLv3+) and GPLv3+

Source:

```console
$ dnf --quiet download --source --url libidn2-2.3.0-1.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/779c0a9f244a8c91e46933aab7ba4a6215a2c33ec8c856de02dbf17d02b6337b/libidn2-2.3.0-1.amzn2.0.3.src.rpm
```

### `rpm` package: `libmetalink-0.1.3-13.amzn2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libmetalink-0.1.3-13.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/af0aec2e615d0ff03b96fd674c80f28b00f2d198951b2e418ec80956b87aa389/libmetalink-0.1.3-13.amzn2.src.rpm
```

### `rpm` package: `libmount-2.30.2-2.amzn2.0.11.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libmount-2.30.2-2.amzn2.0.11
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/c3d8b01e2190e686623eb8551a13a4a33cc08e086036e951fe5ed1b99c7b2b8e/util-linux-2.30.2-2.amzn2.0.11.src.rpm
```

### `rpm` package: `libnghttp2-1.41.0-1.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libnghttp2-1.41.0-1.amzn2.0.4
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2d45495937ec7f02f906dec5791d8efe4e25f87279567a9c0f4e6c50005eff4e/nghttp2-1.41.0-1.amzn2.0.4.src.rpm
```

### `rpm` package: `libpng-1.5.13-8.amzn2.0.5.x86_64`

Licenses (from `rpm --query`): zlib

Source:

```console
$ dnf --quiet download --source --url libpng-1.5.13-8.amzn2.0.5
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/47467e24ba5e44cea7252546421ae9c0efe3287136a6c04be179ff755294ed10/libpng-1.5.13-8.amzn2.0.5.src.rpm
```

### `rpm` package: `libselinux-2.5-12.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url libselinux-2.5-12.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/0be2744b0f89765b31cecb119ca520449eb8cf48cd7355824f7ca4e0873deec3/libselinux-2.5-12.amzn2.0.2.src.rpm
```

### `rpm` package: `libsemanage-2.5-11.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libsemanage-2.5-11.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/eb5fb285756eced1c16757805bfe608a70a745fe4e3c61cd1fc230f2c4786ae8/libsemanage-2.5-11.amzn2.src.rpm
```

### `rpm` package: `libsepol-2.5-10.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libsepol-2.5-10.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2b2a8764b4294026c35f8247282865f2631c8ec45d35349bb2bfc1017a97b958/libsepol-2.5-10.amzn2.0.1.src.rpm
```

### `rpm` package: `libssh2-1.4.3-12.amzn2.2.6.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url libssh2-1.4.3-12.amzn2.2.6
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/d9a9fc99ac24238ed884d06fcfcc22ff7b2403783bf4bc31cc92108135e6899e/libssh2-1.4.3-12.amzn2.2.6.src.rpm
```

### `rpm` package: `libstdc++-7.3.1-17.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv3+ with exceptions and GPLv2+ with exceptions and LGPLv2+ and BSD

Source:

```console
$ dnf --quiet download --source --url libstdc++-7.3.1-17.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/a2b874b1e83eb065848df3e26205c7e903eb46b4c4f40adf7a6a68a1af38698f/gcc-7.3.1-17.amzn2.src.rpm
```

### `rpm` package: `libtasn1-4.10-1.amzn2.0.6.x86_64`

Licenses (from `rpm --query`): GPLv3+ and LGPLv2+

Source:

```console
$ dnf --quiet download --source --url libtasn1-4.10-1.amzn2.0.6
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/8c467da4eca42a4eea65011bf811e97d898b4230c0bdf70ea982d6d5f41c1491/libtasn1-4.10-1.amzn2.0.6.src.rpm
```

### `rpm` package: `libunistring-0.9.3-9.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv3+

Source:

```console
$ dnf --quiet download --source --url libunistring-0.9.3-9.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/a679646faec5cf08ced31c6b0eb872e88e1267b76b4d3a43c1e553d4446732dd/libunistring-0.9.3-9.amzn2.0.2.src.rpm
```

### `rpm` package: `libuuid-2.30.2-2.amzn2.0.11.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url libuuid-2.30.2-2.amzn2.0.11
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/c3d8b01e2190e686623eb8551a13a4a33cc08e086036e951fe5ed1b99c7b2b8e/util-linux-2.30.2-2.amzn2.0.11.src.rpm
```

### `rpm` package: `libverto-0.2.5-4.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libverto-0.2.5-4.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/23eb8faf40e93c9ecbfeccc868d2e42b65bde82f92e1af0b0e9e17c387f1b049/libverto-0.2.5-4.amzn2.0.2.src.rpm
```

### `rpm` package: `libxml2-2.9.1-6.amzn2.5.13.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url libxml2-2.9.1-6.amzn2.5.13
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/66be4d50d3b853dc0d36ac1222f7db448f3bf2e19a27604054c3f82c2ae6b7a8/libxml2-2.9.1-6.amzn2.5.13.src.rpm
```

### `rpm` package: `lua-5.1.4-15.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url lua-5.1.4-15.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/4f245b1212afa57d45d2ef83997a92d3346a2aa315de8d54c4f93aceb71c2c97/lua-5.1.4-15.amzn2.0.2.src.rpm
```

### `rpm` package: `ncurses-6.0-8.20170212.amzn2.1.5.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url ncurses-6.0-8.20170212.amzn2.1.5
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/98b847c530961f8735cf280258cb3e0d448497f1190b269e450aedb4a175dddc/ncurses-6.0-8.20170212.amzn2.1.5.src.rpm
```

### `rpm` package: `ncurses-base-6.0-8.20170212.amzn2.1.5.noarch`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url ncurses-base-6.0-8.20170212.amzn2.1.5.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/98b847c530961f8735cf280258cb3e0d448497f1190b269e450aedb4a175dddc/ncurses-6.0-8.20170212.amzn2.1.5.src.rpm
```

### `rpm` package: `ncurses-libs-6.0-8.20170212.amzn2.1.5.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url ncurses-libs-6.0-8.20170212.amzn2.1.5
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/98b847c530961f8735cf280258cb3e0d448497f1190b269e450aedb4a175dddc/ncurses-6.0-8.20170212.amzn2.1.5.src.rpm
```

### `rpm` package: `nspr-4.35.0-1.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url nspr-4.35.0-1.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/ff6f819d94da64b15bbf33ec914529f7010def8329f177e8534293d072901b92/nspr-4.35.0-1.amzn2.src.rpm
```

### `rpm` package: `nss-3.90.0-2.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url nss-3.90.0-2.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/aef9190716ac4adec707edef19bad72e55b07777b8689982da5d4aee378e4ea8/nss-3.90.0-2.amzn2.0.1.src.rpm
```

### `rpm` package: `nss-pem-1.0.3-5.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv1.1

Source:

```console
$ dnf --quiet download --source --url nss-pem-1.0.3-5.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/704279710518c94532cf67062b10877693d651e1b652fb60ed1ce1fa0cb49d7a/nss-pem-1.0.3-5.amzn2.src.rpm
```

### `rpm` package: `nss-softokn-3.90.0-6.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url nss-softokn-3.90.0-6.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/9d593ebd46d832efe91386332615a459ae77c9761cb1fe13c7c28eb9e9934193/nss-softokn-3.90.0-6.amzn2.src.rpm
```

### `rpm` package: `nss-softokn-freebl-3.90.0-6.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url nss-softokn-freebl-3.90.0-6.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/9d593ebd46d832efe91386332615a459ae77c9761cb1fe13c7c28eb9e9934193/nss-softokn-3.90.0-6.amzn2.src.rpm
```

### `rpm` package: `nss-sysinit-3.90.0-2.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url nss-sysinit-3.90.0-2.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/aef9190716ac4adec707edef19bad72e55b07777b8689982da5d4aee378e4ea8/nss-3.90.0-2.amzn2.0.1.src.rpm
```

### `rpm` package: `nss-tools-3.90.0-2.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url nss-tools-3.90.0-2.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/aef9190716ac4adec707edef19bad72e55b07777b8689982da5d4aee378e4ea8/nss-3.90.0-2.amzn2.0.1.src.rpm
```

### `rpm` package: `nss-util-3.90.0-1.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ dnf --quiet download --source --url nss-util-3.90.0-1.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/68b37d43f23fa6b6234f0fe2d106b09fbd801696d98d7aa10982e0cb621419a8/nss-util-3.90.0-1.amzn2.src.rpm
```

### `rpm` package: `openldap-2.4.44-25.amzn2.0.7.x86_64`

Licenses (from `rpm --query`): OpenLDAP

Source:

```console
$ dnf --quiet download --source --url openldap-2.4.44-25.amzn2.0.7
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/db7da8ae89a175ef6835a375dec2b69b3eaecc676cb58b8dd9c1f8e769fb0fc2/openldap-2.4.44-25.amzn2.0.7.src.rpm
```

### `rpm` package: `openssl-libs-1.0.2k-24.amzn2.0.10.x86_64`

Licenses (from `rpm --query`): OpenSSL

Source:

```console
$ dnf --quiet download --source --url openssl-libs-1.0.2k-24.amzn2.0.10
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/e625902ad4db8d06513f1fd38baca97d55997134ac5c5aa99dbbcae1eb44cd55/openssl-1.0.2k-24.amzn2.0.10.src.rpm
```

### `rpm` package: `p11-kit-0.23.22-1.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url p11-kit-0.23.22-1.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/79c2f1cc336aa17382372c2c5577054870d1d123e5ce606f33bc2443e9c91347/p11-kit-0.23.22-1.amzn2.0.1.src.rpm
```

### `rpm` package: `p11-kit-trust-0.23.22-1.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url p11-kit-trust-0.23.22-1.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/79c2f1cc336aa17382372c2c5577054870d1d123e5ce606f33bc2443e9c91347/p11-kit-0.23.22-1.amzn2.0.1.src.rpm
```

### `rpm` package: `pcre-8.32-17.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ dnf --quiet download --source --url pcre-8.32-17.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/b2470976412c846cbcbb44775d2a4ec2e44564585fd3b25c125432f0befabc30/pcre-8.32-17.amzn2.0.3.src.rpm
```

### `rpm` package: `pinentry-0.8.1-17.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url pinentry-0.8.1-17.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/30819f9f22382344ac3af9a69db748efdb80c7dd77ff73f80d77579fd6409209/pinentry-0.8.1-17.amzn2.0.2.src.rpm
```

### `rpm` package: `popt-1.13-16.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url popt-1.13-16.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/849bd178ea42fbff69e6c5e765042ab80fb56a96bcadc7218926b13765282945/popt-1.13-16.amzn2.0.2.src.rpm
```

### `rpm` package: `pth-2.0.7-23.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url pth-2.0.7-23.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/b168e67224ed78f4c9d2430cad3950ad4e8bb373f8c183347b44f80a4f35e069/pth-2.0.7-23.amzn2.0.2.src.rpm
```

### `rpm` package: `pygpgme-0.3-9.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url pygpgme-0.3-9.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/59142d6d866bcc463e322e6bc8ee0dd7155379ba96d2b6d142c28d1e63e2fa2d/pygpgme-0.3-9.amzn2.0.3.src.rpm
```

### `rpm` package: `pyliblzma-0.5.3-25.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv3+

Source:

```console
$ dnf --quiet download --source --url pyliblzma-0.5.3-25.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/860af43ebf61fc4b2c6c02ec914630e76e68197a77f6b7318b92f5059c7673d1/pyliblzma-0.5.3-25.amzn2.src.rpm
```

### `rpm` package: `python-2.7.18-1.amzn2.0.7.x86_64`

Licenses (from `rpm --query`): Python

Source:

```console
$ dnf --quiet download --source --url python-2.7.18-1.amzn2.0.7
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/4b64d54129a06efcdece1f990ca2caad727f3958690ceead0a962f3e08cd6311/python-2.7.18-1.amzn2.0.7.src.rpm
```

### `rpm` package: `python-iniparse-0.4-9.amzn2.noarch`

Licenses (from `rpm --query`): MIT

Source:

```console
$ dnf --quiet download --source --url python-iniparse-0.4-9.amzn2.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/c44ed4bc8040ce8e74624bd74404387f1c5320ee6b6d975a81e358ab7919b11a/python-iniparse-0.4-9.amzn2.src.rpm
```

### `rpm` package: `python-libs-2.7.18-1.amzn2.0.7.x86_64`

Licenses (from `rpm --query`): Python

Source:

```console
$ dnf --quiet download --source --url python-libs-2.7.18-1.amzn2.0.7
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/4b64d54129a06efcdece1f990ca2caad727f3958690ceead0a962f3e08cd6311/python-2.7.18-1.amzn2.0.7.src.rpm
```

### `rpm` package: `python-pycurl-7.19.0-19.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ or MIT

Source:

```console
$ dnf --quiet download --source --url python-pycurl-7.19.0-19.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/c498524c54f789da1b967318c6a41d5f28c5b95f66ba831e6de30e246039cf55/python-pycurl-7.19.0-19.amzn2.0.2.src.rpm
```

### `rpm` package: `python-urlgrabber-3.10-9.amzn2.0.1.noarch`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url python-urlgrabber-3.10-9.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/059ccd33bf7223a26eedc0f289477c6c86fa24807e51a00dfbb3b8589ffd60be/python-urlgrabber-3.10-9.amzn2.0.1.src.rpm
```

### `rpm` package: `python2-rpm-4.11.3-48.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url python2-rpm-4.11.3-48.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2c0a574de618488ca88beda050a3b5999c5c46d9b4ecd4d72a4d9c1c565be785/rpm-4.11.3-48.amzn2.0.3.src.rpm
```

### `rpm` package: `pyxattr-0.5.1-5.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url pyxattr-0.5.1-5.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/42d7abe323c155cadf4d22f9c13669b38caddd38a8c6bc8841985e1eec52cb43/pyxattr-0.5.1-5.amzn2.0.2.src.rpm
```

### `rpm` package: `readline-6.2-10.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url readline-6.2-10.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/e2b36f4a9d20e84ecb267c1a1b7ac1695a02175ffc08876957103338c6c358a7/readline-6.2-10.amzn2.0.2.src.rpm
```

### `rpm` package: `rpm-4.11.3-48.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url rpm-4.11.3-48.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2c0a574de618488ca88beda050a3b5999c5c46d9b4ecd4d72a4d9c1c565be785/rpm-4.11.3-48.amzn2.0.3.src.rpm
```

### `rpm` package: `rpm-build-libs-4.11.3-48.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+ with exceptions

Source:

```console
$ dnf --quiet download --source --url rpm-build-libs-4.11.3-48.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2c0a574de618488ca88beda050a3b5999c5c46d9b4ecd4d72a4d9c1c565be785/rpm-4.11.3-48.amzn2.0.3.src.rpm
```

### `rpm` package: `rpm-libs-4.11.3-48.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+ with exceptions

Source:

```console
$ dnf --quiet download --source --url rpm-libs-4.11.3-48.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/2c0a574de618488ca88beda050a3b5999c5c46d9b4ecd4d72a4d9c1c565be785/rpm-4.11.3-48.amzn2.0.3.src.rpm
```

### `rpm` package: `sed-4.2.2-5.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url sed-4.2.2-5.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/6536ece4c46bf2ed9823a7e298728310689e54d535226819a7d7fe4b9eeadafd/sed-4.2.2-5.amzn2.0.2.src.rpm
```

### `rpm` package: `setup-2.8.71-10.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url setup-2.8.71-10.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/a048edcb5e7a6552e092a3fd74a073fdd49e7269dd6f7b982088dc71a32cf631/setup-2.8.71-10.amzn2.0.1.src.rpm
```

### `rpm` package: `shadow-utils-4.1.5.1-24.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): BSD and GPLv2+

Source:

```console
$ dnf --quiet download --source --url shadow-utils-4.1.5.1-24.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/574175b4d80e173235170c0519c72c1fd30597f99fb0602742b9ee686d06ea1d/shadow-utils-4.1.5.1-24.amzn2.0.3.src.rpm
```

### `rpm` package: `shared-mime-info-1.8-4.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url shared-mime-info-1.8-4.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/9e51e9ed398518c869e22c71a6cf809d331622958224ced40e8ebf31bf5e810f/shared-mime-info-1.8-4.amzn2.src.rpm
```

### `rpm` package: `sqlite-3.7.17-8.amzn2.1.2.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url sqlite-3.7.17-8.amzn2.1.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/5ada8c006d0e919d9a1fcdc513c897787b875dcd0143ca89aae582983119f1d6/sqlite-3.7.17-8.amzn2.1.2.src.rpm
```

### `rpm` package: `system-release-2-16.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url system-release-2-16.amzn2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/1d86dd37090418630254dc852c55859e9033e342f87091b94c9448bcacdb7b2a/system-release-2-16.amzn2.src.rpm
```

### `rpm` package: `tar-1.26-35.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ dnf --quiet download --source --url tar-1.26-35.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/e42eecd8afc27d6dfe714ad849eb507a01361c479efa0b5a968a0782d3eacbaf/tar-1.26-35.amzn2.0.2.src.rpm
```

### `rpm` package: `tzdata-2023c-1.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ dnf --quiet download --source --url tzdata-2023c-1.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/9de2f80d2d90f2d38b85ef444d83e2bec52930605705a0c628674c6f5ae82d29/tzdata-2023c-1.amzn2.0.1.src.rpm
```

### `rpm` package: `ustr-1.0.4-16.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): MIT or LGPLv2+ or BSD

Source:

```console
$ dnf --quiet download --source --url ustr-1.0.4-16.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/7477de946dfcd9c18a323e3fbf55abf8fe1137be0adb7d0c114c610963e4210e/ustr-1.0.4-16.amzn2.0.3.src.rpm
```

### `rpm` package: `vim-data-9.0.2081-1.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Vim AND LGPL-2.1-or-later AND MIT AND GPL-1.0-only AND (GPL-2.0-only OR Vim) AND Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause AND GPL-2.0-or-later AND GPL-3.0-or-later AND OPUBL-1.0

Source:

```console
$ dnf --quiet download --source --url vim-data-9.0.2081-1.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/511165681822d5d2252b615d86e7e59d48c9962a3de487a034fa06870c279412/vim-9.0.2081-1.amzn2.0.1.src.rpm
```

### `rpm` package: `vim-minimal-9.0.2081-1.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): Vim AND LGPL-2.1-or-later AND MIT AND GPL-1.0-only AND (GPL-2.0-only OR Vim) AND Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause AND GPL-2.0-or-later AND GPL-3.0-or-later AND OPUBL-1.0

Source:

```console
$ dnf --quiet download --source --url vim-minimal-9.0.2081-1.amzn2.0.1
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/511165681822d5d2252b615d86e7e59d48c9962a3de487a034fa06870c279412/vim-9.0.2081-1.amzn2.0.1.src.rpm
```

### `rpm` package: `xz-5.2.2-1.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url xz-5.2.2-1.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/e2158e7ac9785d1ff7288d90ddb7ac041ba54804e86b9a604ea0717444a17a76/xz-5.2.2-1.amzn2.0.3.src.rpm
```

### `rpm` package: `xz-libs-5.2.2-1.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ dnf --quiet download --source --url xz-libs-5.2.2-1.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/e2158e7ac9785d1ff7288d90ddb7ac041ba54804e86b9a604ea0717444a17a76/xz-5.2.2-1.amzn2.0.3.src.rpm
```

### `rpm` package: `yum-3.4.3-158.amzn2.0.7.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url yum-3.4.3-158.amzn2.0.7.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/20b76b7827c4831d4cb21e9901970ecfbc6f9215182ce9a40b6c4e96acf51561/yum-3.4.3-158.amzn2.0.7.src.rpm
```

### `rpm` package: `yum-metadata-parser-1.1.4-10.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ dnf --quiet download --source --url yum-metadata-parser-1.1.4-10.amzn2.0.2
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/b710ba0dd68993f774c5fe5325edfec71935fa2f0dba7cd548692b84f31b7988/yum-metadata-parser-1.1.4-10.amzn2.0.2.src.rpm
```

### `rpm` package: `yum-plugin-ovl-1.1.31-46.amzn2.0.1.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url yum-plugin-ovl-1.1.31-46.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/74e03e38d661b26d57dc3fcbd58a66e736b5e8979ccf0493149d0add45dd0416/yum-utils-1.1.31-46.amzn2.0.1.src.rpm
```

### `rpm` package: `yum-plugin-priorities-1.1.31-46.amzn2.0.1.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ dnf --quiet download --source --url yum-plugin-priorities-1.1.31-46.amzn2.0.1.noarch
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/74e03e38d661b26d57dc3fcbd58a66e736b5e8979ccf0493149d0add45dd0416/yum-utils-1.1.31-46.amzn2.0.1.src.rpm
```

### `rpm` package: `zlib-1.2.7-19.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): zlib and Boost

Source:

```console
$ dnf --quiet download --source --url zlib-1.2.7-19.amzn2.0.3
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/a68b3d6332c817448ba6544419f0372457a0e8a1c102da02a75edd25c0dfa6ee/../../../../../blobstore/a4d3572abd43bc021bfe5c83e87d4394ca6f5fb879109d4cdb152a0e1b10dbc4/zlib-1.2.7-19.amzn2.0.3.src.rpm
```
