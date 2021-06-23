# `tomcat:7.0.109-jdk8-corretto`

## Docker Metadata

- Image ID: `sha256:fe1008d9e77524d6f24d414587a1756051ecadb78fca289f70aa7c4e9a3ffbc4`
- Created: `2021-06-14T23:17:35.096472251Z`
- Virtual Size: ~ 374.60 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["catalina.sh","run"]`
- Environment:
  - `PATH=/usr/local/tomcat/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto`
  - `CATALINA_HOME=/usr/local/tomcat`
  - `TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib`
  - `LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib`
  - `GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 61B832AC2F1C5A90F0F9B00A1C506407564C17A3 713DA88BE50911535FE716F5208B0AB1D63011C7 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23`
  - `TOMCAT_MAJOR=7`
  - `TOMCAT_VERSION=7.0.109`
  - `TOMCAT_SHA512=612e830913bf1401bc9540e2273e465b0ee7ef63750a9969a80f1e9da9edb4888aa621fcc6fa5ba23cff94a40e91eb97e3f969b8064dabd49b2d0ea29e59b57e`

## `rpm` (`.rpm`-based packages)

### `rpm` package: `amazon-linux-extras-2.0.0-1.amzn2.noarch`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ yumdownloader --quiet --source --urls amazon-linux-extras-2.0.0-1.amzn2.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/67094641a11e9082fb8e43987b1940d79544840456eb649b721064011e975f07/amazon-linux-extras-2.0.0-1.amzn2.src.rpm
```

### `rpm` package: `apr-1.6.3-5.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): ASL 2.0 and BSD with advertising and ISC and BSD

Source:

```console
$ yumdownloader --quiet --source --urls apr-1.6.3-5.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/2f9f774e1efb0e9f738575da9f51550dd57b0aea82a71d3e360c489d9ea923eb/apr-1.6.3-5.amzn2.0.2.src.rpm
```

### `rpm` package: `basesystem-10.0-7.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls basesystem-10.0-7.amzn2.0.1.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/303ffc769b33bd06f7d3c5d0a1999079ad5afb6d205448dd607a8b6a5cbc3551/basesystem-10.0-7.amzn2.0.1.src.rpm
```

### `rpm` package: `bash-4.2.46-34.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls bash-4.2.46-34.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/088b4acd2aa66aac9479237b6c06724ef38173941734da6a81fb28add6418143/bash-4.2.46-34.amzn2.src.rpm
```

### `rpm` package: `bzip2-libs-1.0.6-13.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ yumdownloader --quiet --source --urls bzip2-libs-1.0.6-13.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d628e30c748a78ba4d69f98730e6030476aeb63f88e8747aa522c48da8eb75ee/bzip2-1.0.6-13.amzn2.0.2.src.rpm
```

### `rpm` package: `ca-certificates-2020.2.41-70.0.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls ca-certificates-2020.2.41-70.0.amzn2.0.1.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/909bcf385d40e7dc85343ba423088131038e39df4d8d25a8ef6dc67cc9f1ad6d/ca-certificates-2020.2.41-70.0.amzn2.0.1.src.rpm
```

### `rpm` package: `chkconfig-1.7.4-1.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ yumdownloader --quiet --source --urls chkconfig-1.7.4-1.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/227e42c03e4cdcc55a1851cfe633f2a280cb53eea907a581d95422575f584465/chkconfig-1.7.4-1.amzn2.0.2.src.rpm
```

### `rpm` package: `coreutils-8.22-24.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls coreutils-8.22-24.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/7785c3a49bafaa745c01233429d6dab66539416864de241fb29aea434a29dcb2/coreutils-8.22-24.amzn2.src.rpm
```

### `rpm` package: `cpio-2.11-28.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls cpio-2.11-28.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/b567960170c409a145333888e05daa9569564d37bd31df920c75c09ef5b710df/cpio-2.11-28.amzn2.src.rpm
```

### `rpm` package: `curl-7.61.1-12.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls curl-7.61.1-12.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/fb75b5678cc9ceacbece78025cb0cbb9a44b0e924ae8853cdc4777604ebdba0d/curl-7.61.1-12.amzn2.0.2.src.rpm
```

### `rpm` package: `cyrus-sasl-lib-2.1.26-23.amzn2.x86_64`

Licenses (from `rpm --query`): BSD with advertising

Source:

```console
$ yumdownloader --quiet --source --urls cyrus-sasl-lib-2.1.26-23.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d94991ec3297e116fddaa0543c7626d29605fd5ce546f5d94f697e65c595ad66/cyrus-sasl-2.1.26-23.amzn2.src.rpm
```

### `rpm` package: `dejavu-fonts-common-2.33-6.amzn2.noarch`

Licenses (from `rpm --query`): Bitstream Vera and Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls dejavu-fonts-common-2.33-6.amzn2.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/2c78ae75ee92a19e0ecbd2d6f1b1e6c343e2c8357057617fb7a03438fcff9ce0/dejavu-fonts-2.33-6.amzn2.src.rpm
```

### `rpm` package: `dejavu-sans-fonts-2.33-6.amzn2.noarch`

Licenses (from `rpm --query`): Bitstream Vera and Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls dejavu-sans-fonts-2.33-6.amzn2.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/2c78ae75ee92a19e0ecbd2d6f1b1e6c343e2c8357057617fb7a03438fcff9ce0/dejavu-fonts-2.33-6.amzn2.src.rpm
```

### `rpm` package: `diffutils-3.3-5.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls diffutils-3.3-5.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/3b94189bd4a0bbb334c887b5a7306f5cbe927e45ca9a9c1e68e6466570b7a4e1/diffutils-3.3-5.amzn2.src.rpm
```

### `rpm` package: `elfutils-libelf-0.176-2.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv2+ or LGPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls elfutils-libelf-0.176-2.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/7f6cc4b60d3a0fb8499726d64a830d91c97b301955f44418c3f1de3fb6304228/elfutils-0.176-2.amzn2.src.rpm
```

### `rpm` package: `expat-2.1.0-12.amzn2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls expat-2.1.0-12.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/95e5534999eef179a172c04292c0a2f85106b24b23ea78e22eced07a3b53a4e3/expat-2.1.0-12.amzn2.src.rpm
```

### `rpm` package: `file-libs-5.11-36.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ yumdownloader --quiet --source --urls file-libs-5.11-36.amzn2.0.1
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6826885873bb4ef8f4d7479ffbfbceb96807ae298e2f0a9a083022200ca7caab/file-5.11-36.amzn2.0.1.src.rpm
```

### `rpm` package: `filesystem-3.2-25.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls filesystem-3.2-25.amzn2.0.4
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/c1bdb520a838326c15c1c86b0a1314c9e44f7689de956010d7a8e4bfda7d34e4/filesystem-3.2-25.amzn2.0.4.src.rpm
```

### `rpm` package: `findutils-4.5.11-6.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls findutils-4.5.11-6.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/8cb38ddd3353da1ca38e2748e4affeb61a422044bf26c05f93cd0e20d83b125d/findutils-4.5.11-6.amzn2.src.rpm
```

### `rpm` package: `fontconfig-2.13.0-4.3.amzn2.x86_64`

Licenses (from `rpm --query`): MIT and Public Domain and UCD

Source:

```console
$ yumdownloader --quiet --source --urls fontconfig-2.13.0-4.3.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d27fa964cbcbbd78a2cd17349b255f37d6fa44876c0186ffd4b05c63d6aae827/fontconfig-2.13.0-4.3.amzn2.src.rpm
```

### `rpm` package: `fontpackages-filesystem-1.44-8.amzn2.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls fontpackages-filesystem-1.44-8.amzn2.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a7c49b56992c5deec79f1d6b1cadaf4a1210c7f5cefea9dab4b353e83eeb6ab5/fontpackages-1.44-8.amzn2.src.rpm
```

### `rpm` package: `freetype-2.8-14.amzn2.1.x86_64`

Licenses (from `rpm --query`): (FTL or GPLv2+) and BSD and MIT and Public Domain and zlib with acknowledgement

Source:

```console
$ yumdownloader --quiet --source --urls freetype-2.8-14.amzn2.1
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6d823c73999355231a92f651c352ef84fbbe1c4faea18662b755e3bf33be45df/freetype-2.8-14.amzn2.1.src.rpm
```

### `rpm` package: `gawk-4.0.2-4.amzn2.1.2.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPL and LGPLv3+ and LGPL and BSD

Source:

```console
$ yumdownloader --quiet --source --urls gawk-4.0.2-4.amzn2.1.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/20e168961dd7975b2be268b247219eb2e7a1bef49898ad360ffae2833d76ad1c/gawk-4.0.2-4.amzn2.1.2.src.rpm
```

### `rpm` package: `gdbm-1.13-6.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls gdbm-1.13-6.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/e2866f1817e24bcd350768bf85c8bbddde135513ced29ce315df75f311cf77cf/gdbm-1.13-6.amzn2.0.2.src.rpm
```

### `rpm` package: `glib2-2.56.1-7.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls glib2-2.56.1-7.amzn2.0.1
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/8ddbb329b8aa21536459692fbc8a9cdf4b2c88037b274b30b843f81bdecfd007/glib2-2.56.1-7.amzn2.0.1.src.rpm
```

### `rpm` package: `glibc-2.26-45.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls glibc-2.26-45.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a086b0ac2103a7cd644bf9cee459e719640e29df0e1f4f9363d9d40676d3b58/glibc-2.26-45.amzn2.src.rpm
```

### `rpm` package: `glibc-common-2.26-45.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls glibc-common-2.26-45.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a086b0ac2103a7cd644bf9cee459e719640e29df0e1f4f9363d9d40676d3b58/glibc-2.26-45.amzn2.src.rpm
```

### `rpm` package: `glibc-langpack-en-2.26-45.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls glibc-langpack-en-2.26-45.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a086b0ac2103a7cd644bf9cee459e719640e29df0e1f4f9363d9d40676d3b58/glibc-2.26-45.amzn2.src.rpm
```

### `rpm` package: `glibc-minimal-langpack-2.26-45.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls glibc-minimal-langpack-2.26-45.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a086b0ac2103a7cd644bf9cee459e719640e29df0e1f4f9363d9d40676d3b58/glibc-2.26-45.amzn2.src.rpm
```

### `rpm` package: `gmp-6.0.0-15.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv3+ or GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls gmp-6.0.0-15.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/712fffd161eb394310f7fe5f7d41ae2aae07cdcce27ca119bf04c6f056eb2b4d/gmp-6.0.0-15.amzn2.0.2.src.rpm
```

### `rpm` package: `gnupg2-2.0.22-5.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls gnupg2-2.0.22-5.amzn2.0.4
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/cf2f89347d3eba84fb17d1d713b4a18aa7b15bfaace0b19464780208135b493f/gnupg2-2.0.22-5.amzn2.0.4.src.rpm
```

### `rpm` package: `gpg-pubkey-b04f24e3-5de94a19`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`yumdownloader` failed or returned no results)!

### `rpm` package: `gpg-pubkey-c87f5b1a-593863f8`

Licenses (from `rpm --query`): pubkey

**WARNING:** unable to find source (`yumdownloader` failed or returned no results)!

### `rpm` package: `gpgme-1.3.2-5.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls gpgme-1.3.2-5.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/81074517b77553b2abbdc13fb0637c599a4c32f25ff85e6e00a9761fbd961d9f/gpgme-1.3.2-5.amzn2.0.2.src.rpm
```

### `rpm` package: `grep-2.20-3.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls grep-2.20-3.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a1fd83c54bc7f4701e6b979d8f5dcc9950e2b5116cbb1c27057f412bed54390/grep-2.20-3.amzn2.0.2.src.rpm
```

### `rpm` package: `info-5.1-5.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls info-5.1-5.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/968c079ef8a8a2efee76ff59cd99e06dd242b8813960171d0f5c23f4a6eb0bb2/texinfo-5.1-5.amzn2.src.rpm
```

### `rpm` package: `java-1.8.0-amazon-corretto-devel-1.8.0_292.b10-1.x86_64`

Licenses (from `rpm --query`): ASL 1.1 and ASL 2.0 and BSD and BSD with advertising and GPL+ and GPLv2 and GPLv2 with exceptions and IJG and LGPLv2+ and MIT and MPLv2.0 and Public Domain and W3C and zlib.

**WARNING:** unable to find source (`yumdownloader` failed or returned no results)!

### `rpm` package: `keyutils-libs-1.5.8-3.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls keyutils-libs-1.5.8-3.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/1579dc52bd90d64e68d663da4dfa4462afa9df1cfbef30d47b64add0dd12210e/keyutils-1.5.8-3.amzn2.0.2.src.rpm
```

### `rpm` package: `krb5-libs-1.15.1-37.amzn2.2.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls krb5-libs-1.15.1-37.amzn2.2.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a4ae5281a860a9566b9d0533461f0a65858cb1cea7cc82eb94f5b0ca59ef8020/krb5-1.15.1-37.amzn2.2.2.src.rpm
```

### `rpm` package: `libacl-2.2.51-14.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libacl-2.2.51-14.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d21969f8fbccf539fa601961f20352b7c95b4cf593c9fa5dad2ac4896c7ca6c9/acl-2.2.51-14.amzn2.src.rpm
```

### `rpm` package: `libassuan-2.1.0-3.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls libassuan-2.1.0-3.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/27b0138d028a9ba30c43384ce6b2d1314d0ac3a6284c6793655c5589893d47ee/libassuan-2.1.0-3.amzn2.0.2.src.rpm
```

### `rpm` package: `libattr-2.4.46-12.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libattr-2.4.46-12.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/370b7813e0e86fadc241a9fb590451372429f0fe3ab17d62a4378b49089f8158/attr-2.4.46-12.amzn2.0.2.src.rpm
```

### `rpm` package: `libblkid-2.30.2-2.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libblkid-2.30.2-2.amzn2.0.4
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/7967325dfd44cdb0fd0caa45b27d56da920dd3110a5989c3ae52364b44ae7d82/util-linux-2.30.2-2.amzn2.0.4.src.rpm
```

### `rpm` package: `libcap-2.22-9.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libcap-2.22-9.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/eb7b89ef09d8fcfa7e14b00d94d983ab918a56db1b8a0ca89667e8fac94467dd/libcap-2.22-9.amzn2.0.2.src.rpm
```

### `rpm` package: `libcom_err-1.42.9-19.amzn2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls libcom_err-1.42.9-19.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/161cbeb604e5866ce40b2be3280195526a37c6675362961dd307be04366b2678/e2fsprogs-1.42.9-19.amzn2.src.rpm
```

### `rpm` package: `libcrypt-2.26-45.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ and LGPLv2+ with exceptions and GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libcrypt-2.26-45.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a086b0ac2103a7cd644bf9cee459e719640e29df0e1f4f9363d9d40676d3b58/glibc-2.26-45.amzn2.src.rpm
```

### `rpm` package: `libcurl-7.61.1-12.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls libcurl-7.61.1-12.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/fb75b5678cc9ceacbece78025cb0cbb9a44b0e924ae8853cdc4777604ebdba0d/curl-7.61.1-12.amzn2.0.2.src.rpm
```

### `rpm` package: `libdb-5.3.21-24.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): BSD and LGPLv2 and Sleepycat

Source:

```console
$ yumdownloader --quiet --source --urls libdb-5.3.21-24.amzn2.0.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a07a0476eadc4a9948fa0985711becd678027168f34c4c53838da1d6335f9ff/libdb-5.3.21-24.amzn2.0.3.src.rpm
```

### `rpm` package: `libdb-utils-5.3.21-24.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): BSD and LGPLv2 and Sleepycat

Source:

```console
$ yumdownloader --quiet --source --urls libdb-utils-5.3.21-24.amzn2.0.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6a07a0476eadc4a9948fa0985711becd678027168f34c4c53838da1d6335f9ff/libdb-5.3.21-24.amzn2.0.3.src.rpm
```

### `rpm` package: `libffi-3.0.13-18.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT and Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls libffi-3.0.13-18.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6d795273d9b8725efa8069ecb46398043d7100cfd4979b9c31489e35504e31f7/libffi-3.0.13-18.amzn2.0.2.src.rpm
```

### `rpm` package: `libgcc-7.3.1-12.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv3+ with exceptions and GPLv2+ with exceptions and LGPLv2+ and BSD

Source:

```console
$ yumdownloader --quiet --source --urls libgcc-7.3.1-12.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/f32f053ece942d6fcf5b871bd5cf53634d56977f7c5783d2a026a65ba5394cf5/gcc-7.3.1-12.amzn2.src.rpm
```

### `rpm` package: `libgcrypt-1.5.3-14.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libgcrypt-1.5.3-14.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/ddfd604706fbb66bc5d000e6f198469a67859ffd99df4344918ba6d329f79bb0/libgcrypt-1.5.3-14.amzn2.0.2.src.rpm
```

### `rpm` package: `libgpg-error-1.12-3.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libgpg-error-1.12-3.amzn2.0.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/997de9d51396f20df5b00b7f41a4bc110b88c5243225ff5941026174850a6e6e/libgpg-error-1.12-3.amzn2.0.3.src.rpm
```

### `rpm` package: `libidn2-2.3.0-1.amzn2.x86_64`

Licenses (from `rpm --query`): (GPLv2+ or LGPLv3+) and GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls libidn2-2.3.0-1.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/12635dd70a57fde4e0cf0238f4cbe5918a7f305f5f15edb0daaf07f35428fde1/libidn2-2.3.0-1.amzn2.src.rpm
```

### `rpm` package: `libmetalink-0.1.3-13.amzn2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls libmetalink-0.1.3-13.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/af0aec2e615d0ff03b96fd674c80f28b00f2d198951b2e418ec80956b87aa389/libmetalink-0.1.3-13.amzn2.src.rpm
```

### `rpm` package: `libmount-2.30.2-2.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libmount-2.30.2-2.amzn2.0.4
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/7967325dfd44cdb0fd0caa45b27d56da920dd3110a5989c3ae52364b44ae7d82/util-linux-2.30.2-2.amzn2.0.4.src.rpm
```

### `rpm` package: `libnghttp2-1.41.0-1.amzn2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls libnghttp2-1.41.0-1.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/0aeaff758cdbf0d80533935b2e5b3f9a6f8fe5bdb9464008ceee2073e12084bd/nghttp2-1.41.0-1.amzn2.src.rpm
```

### `rpm` package: `libpng-1.5.13-8.amzn2.x86_64`

Licenses (from `rpm --query`): zlib

Source:

```console
$ yumdownloader --quiet --source --urls libpng-1.5.13-8.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/720670090e9da15bd9f60e8f1dc38a55d3663dd2277ed7b27fb7b567a1c39d39/libpng-1.5.13-8.amzn2.src.rpm
```

### `rpm` package: `libselinux-2.5-12.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls libselinux-2.5-12.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/0be2744b0f89765b31cecb119ca520449eb8cf48cd7355824f7ca4e0873deec3/libselinux-2.5-12.amzn2.0.2.src.rpm
```

### `rpm` package: `libsepol-2.5-8.1.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libsepol-2.5-8.1.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/c5597168fd76decdd14b8c307ea2ab87a22f7e2236cf9c2ff4cf438c0e6d4120/libsepol-2.5-8.1.amzn2.0.2.src.rpm
```

### `rpm` package: `libssh2-1.4.3-12.amzn2.2.3.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ yumdownloader --quiet --source --urls libssh2-1.4.3-12.amzn2.2.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/ef9036126023044ebfb64786bbf29621695f9fd357830ccf39bebb19932fdde0/libssh2-1.4.3-12.amzn2.2.3.src.rpm
```

### `rpm` package: `libstdc++-7.3.1-12.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv3+ and GPLv3+ with exceptions and GPLv2+ with exceptions and LGPLv2+ and BSD

Source:

```console
$ yumdownloader --quiet --source --urls libstdc++-7.3.1-12.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/f32f053ece942d6fcf5b871bd5cf53634d56977f7c5783d2a026a65ba5394cf5/gcc-7.3.1-12.amzn2.src.rpm
```

### `rpm` package: `libtasn1-4.10-1.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+ and LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls libtasn1-4.10-1.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/99cc7d9be4ecafa389bcb8c2d1d5456b07874ecd6d24e72a73b73a393041043a/libtasn1-4.10-1.amzn2.0.2.src.rpm
```

### `rpm` package: `libunistring-0.9.3-9.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls libunistring-0.9.3-9.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a679646faec5cf08ced31c6b0eb872e88e1267b76b4d3a43c1e553d4446732dd/libunistring-0.9.3-9.amzn2.0.2.src.rpm
```

### `rpm` package: `libuuid-2.30.2-2.amzn2.0.4.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ yumdownloader --quiet --source --urls libuuid-2.30.2-2.amzn2.0.4
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/7967325dfd44cdb0fd0caa45b27d56da920dd3110a5989c3ae52364b44ae7d82/util-linux-2.30.2-2.amzn2.0.4.src.rpm
```

### `rpm` package: `libverto-0.2.5-4.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls libverto-0.2.5-4.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/23eb8faf40e93c9ecbfeccc868d2e42b65bde82f92e1af0b0e9e17c387f1b049/libverto-0.2.5-4.amzn2.0.2.src.rpm
```

### `rpm` package: `libxml2-2.9.1-6.amzn2.5.1.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls libxml2-2.9.1-6.amzn2.5.1
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/e26858355c4df615ccdc11e136485a1acc716811176784f3985644c0f6d49062/libxml2-2.9.1-6.amzn2.5.1.src.rpm
```

### `rpm` package: `lua-5.1.4-15.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls lua-5.1.4-15.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/4f245b1212afa57d45d2ef83997a92d3346a2aa315de8d54c4f93aceb71c2c97/lua-5.1.4-15.amzn2.0.2.src.rpm
```

### `rpm` package: `ncurses-6.0-8.20170212.amzn2.1.3.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls ncurses-6.0-8.20170212.amzn2.1.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a0ab33ecd508ea556f1874e5baa8cc751466cf7b37d6f42ef15adcdf4fa4ad8e/ncurses-6.0-8.20170212.amzn2.1.3.src.rpm
```

### `rpm` package: `ncurses-base-6.0-8.20170212.amzn2.1.3.noarch`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls ncurses-base-6.0-8.20170212.amzn2.1.3.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a0ab33ecd508ea556f1874e5baa8cc751466cf7b37d6f42ef15adcdf4fa4ad8e/ncurses-6.0-8.20170212.amzn2.1.3.src.rpm
```

### `rpm` package: `ncurses-libs-6.0-8.20170212.amzn2.1.3.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls ncurses-libs-6.0-8.20170212.amzn2.1.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a0ab33ecd508ea556f1874e5baa8cc751466cf7b37d6f42ef15adcdf4fa4ad8e/ncurses-6.0-8.20170212.amzn2.1.3.src.rpm
```

### `rpm` package: `nspr-4.25.0-2.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ yumdownloader --quiet --source --urls nspr-4.25.0-2.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/ee6e13b6baffbdfc9c535381457bd739f0ff43933507ee52375981b9e0ee12fa/nspr-4.25.0-2.amzn2.src.rpm
```

### `rpm` package: `nss-3.53.1-3.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ yumdownloader --quiet --source --urls nss-3.53.1-3.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d7aaefe2f0b7813c966d9014f78af25dc5244cceee6909f79731c4d997edcc28/nss-3.53.1-3.amzn2.src.rpm
```

### `rpm` package: `nss-pem-1.0.3-5.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv1.1

Source:

```console
$ yumdownloader --quiet --source --urls nss-pem-1.0.3-5.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/704279710518c94532cf67062b10877693d651e1b652fb60ed1ce1fa0cb49d7a/nss-pem-1.0.3-5.amzn2.src.rpm
```

### `rpm` package: `nss-softokn-3.53.1-6.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ yumdownloader --quiet --source --urls nss-softokn-3.53.1-6.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/4dbb73c4f123686d4098650c59185d23fb37a5339677c2e0d1dd155fe21397bd/nss-softokn-3.53.1-6.amzn2.src.rpm
```

### `rpm` package: `nss-softokn-freebl-3.53.1-6.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ yumdownloader --quiet --source --urls nss-softokn-freebl-3.53.1-6.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/4dbb73c4f123686d4098650c59185d23fb37a5339677c2e0d1dd155fe21397bd/nss-softokn-3.53.1-6.amzn2.src.rpm
```

### `rpm` package: `nss-sysinit-3.53.1-3.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ yumdownloader --quiet --source --urls nss-sysinit-3.53.1-3.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d7aaefe2f0b7813c966d9014f78af25dc5244cceee6909f79731c4d997edcc28/nss-3.53.1-3.amzn2.src.rpm
```

### `rpm` package: `nss-tools-3.53.1-3.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ yumdownloader --quiet --source --urls nss-tools-3.53.1-3.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d7aaefe2f0b7813c966d9014f78af25dc5244cceee6909f79731c4d997edcc28/nss-3.53.1-3.amzn2.src.rpm
```

### `rpm` package: `nss-util-3.53.1-1.amzn2.x86_64`

Licenses (from `rpm --query`): MPLv2.0

Source:

```console
$ yumdownloader --quiet --source --urls nss-util-3.53.1-1.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/96021989815159d56c7af8b960c653a6087105ef7de288ce60ff2d6c4b7558e4/nss-util-3.53.1-1.amzn2.src.rpm
```

### `rpm` package: `openldap-2.4.44-23.amzn2.x86_64`

Licenses (from `rpm --query`): OpenLDAP

Source:

```console
$ yumdownloader --quiet --source --urls openldap-2.4.44-23.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a237631b273d78f45c22f9a8c079ef8e4b8164710a20639182d8ebf3c1428a57/openldap-2.4.44-23.amzn2.src.rpm
```

### `rpm` package: `openssl-libs-1.0.2k-19.amzn2.0.6.x86_64`

Licenses (from `rpm --query`): OpenSSL

Source:

```console
$ yumdownloader --quiet --source --urls openssl-libs-1.0.2k-19.amzn2.0.6
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/96e65fc5c3448c0d5786e4c6c293c14a4bd168ce9a524eb8439c1b8c721c8ded/openssl-1.0.2k-19.amzn2.0.6.src.rpm
```

### `rpm` package: `p11-kit-0.23.22-1.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ yumdownloader --quiet --source --urls p11-kit-0.23.22-1.amzn2.0.1
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/79c2f1cc336aa17382372c2c5577054870d1d123e5ce606f33bc2443e9c91347/p11-kit-0.23.22-1.amzn2.0.1.src.rpm
```

### `rpm` package: `p11-kit-trust-0.23.22-1.amzn2.0.1.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ yumdownloader --quiet --source --urls p11-kit-trust-0.23.22-1.amzn2.0.1
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/79c2f1cc336aa17382372c2c5577054870d1d123e5ce606f33bc2443e9c91347/p11-kit-0.23.22-1.amzn2.0.1.src.rpm
```

### `rpm` package: `pcre-8.32-17.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): BSD

Source:

```console
$ yumdownloader --quiet --source --urls pcre-8.32-17.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/c2b7d97e78a0b2fc29614992206919068a4f34f088bba431056abcb8802ce872/pcre-8.32-17.amzn2.0.2.src.rpm
```

### `rpm` package: `pinentry-0.8.1-17.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls pinentry-0.8.1-17.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/30819f9f22382344ac3af9a69db748efdb80c7dd77ff73f80d77579fd6409209/pinentry-0.8.1-17.amzn2.0.2.src.rpm
```

### `rpm` package: `popt-1.13-16.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls popt-1.13-16.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/849bd178ea42fbff69e6c5e765042ab80fb56a96bcadc7218926b13765282945/popt-1.13-16.amzn2.0.2.src.rpm
```

### `rpm` package: `pth-2.0.7-23.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls pth-2.0.7-23.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/b168e67224ed78f4c9d2430cad3950ad4e8bb373f8c183347b44f80a4f35e069/pth-2.0.7-23.amzn2.0.2.src.rpm
```

### `rpm` package: `pygpgme-0.3-9.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls pygpgme-0.3-9.amzn2.0.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/59142d6d866bcc463e322e6bc8ee0dd7155379ba96d2b6d142c28d1e63e2fa2d/pygpgme-0.3-9.amzn2.0.3.src.rpm
```

### `rpm` package: `pyliblzma-0.5.3-25.amzn2.x86_64`

Licenses (from `rpm --query`): LGPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls pyliblzma-0.5.3-25.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/860af43ebf61fc4b2c6c02ec914630e76e68197a77f6b7318b92f5059c7673d1/pyliblzma-0.5.3-25.amzn2.src.rpm
```

### `rpm` package: `python-2.7.18-1.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): Python

Source:

```console
$ yumdownloader --quiet --source --urls python-2.7.18-1.amzn2.0.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/b3809098d6402ff740278497416e977808ae933a32ce6aa7142f0b97fd4dd089/python-2.7.18-1.amzn2.0.3.src.rpm
```

### `rpm` package: `python-iniparse-0.4-9.amzn2.noarch`

Licenses (from `rpm --query`): MIT

Source:

```console
$ yumdownloader --quiet --source --urls python-iniparse-0.4-9.amzn2.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/c44ed4bc8040ce8e74624bd74404387f1c5320ee6b6d975a81e358ab7919b11a/python-iniparse-0.4-9.amzn2.src.rpm
```

### `rpm` package: `python-libs-2.7.18-1.amzn2.0.3.x86_64`

Licenses (from `rpm --query`): Python

Source:

```console
$ yumdownloader --quiet --source --urls python-libs-2.7.18-1.amzn2.0.3
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/b3809098d6402ff740278497416e977808ae933a32ce6aa7142f0b97fd4dd089/python-2.7.18-1.amzn2.0.3.src.rpm
```

### `rpm` package: `python-pycurl-7.19.0-19.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+ or MIT

Source:

```console
$ yumdownloader --quiet --source --urls python-pycurl-7.19.0-19.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/c498524c54f789da1b967318c6a41d5f28c5b95f66ba831e6de30e246039cf55/python-pycurl-7.19.0-19.amzn2.0.2.src.rpm
```

### `rpm` package: `python-urlgrabber-3.10-9.amzn2.0.1.noarch`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls python-urlgrabber-3.10-9.amzn2.0.1.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/059ccd33bf7223a26eedc0f289477c6c86fa24807e51a00dfbb3b8589ffd60be/python-urlgrabber-3.10-9.amzn2.0.1.src.rpm
```

### `rpm` package: `python2-rpm-4.11.3-40.amzn2.0.5.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls python2-rpm-4.11.3-40.amzn2.0.5
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d62ad87fc4f99ce5544760ef4bedaac867cd9c61474d4f68079d609d5cc2ce9f/rpm-4.11.3-40.amzn2.0.5.src.rpm
```

### `rpm` package: `pyxattr-0.5.1-5.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls pyxattr-0.5.1-5.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/42d7abe323c155cadf4d22f9c13669b38caddd38a8c6bc8841985e1eec52cb43/pyxattr-0.5.1-5.amzn2.0.2.src.rpm
```

### `rpm` package: `readline-6.2-10.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls readline-6.2-10.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/e2b36f4a9d20e84ecb267c1a1b7ac1695a02175ffc08876957103338c6c358a7/readline-6.2-10.amzn2.0.2.src.rpm
```

### `rpm` package: `rpm-4.11.3-40.amzn2.0.5.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls rpm-4.11.3-40.amzn2.0.5
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d62ad87fc4f99ce5544760ef4bedaac867cd9c61474d4f68079d609d5cc2ce9f/rpm-4.11.3-40.amzn2.0.5.src.rpm
```

### `rpm` package: `rpm-build-libs-4.11.3-40.amzn2.0.5.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+ with exceptions

Source:

```console
$ yumdownloader --quiet --source --urls rpm-build-libs-4.11.3-40.amzn2.0.5
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d62ad87fc4f99ce5544760ef4bedaac867cd9c61474d4f68079d609d5cc2ce9f/rpm-4.11.3-40.amzn2.0.5.src.rpm
```

### `rpm` package: `rpm-libs-4.11.3-40.amzn2.0.5.x86_64`

Licenses (from `rpm --query`): GPLv2+ and LGPLv2+ with exceptions

Source:

```console
$ yumdownloader --quiet --source --urls rpm-libs-4.11.3-40.amzn2.0.5
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/d62ad87fc4f99ce5544760ef4bedaac867cd9c61474d4f68079d609d5cc2ce9f/rpm-4.11.3-40.amzn2.0.5.src.rpm
```

### `rpm` package: `sed-4.2.2-5.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv3+

Source:

```console
$ yumdownloader --quiet --source --urls sed-4.2.2-5.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/6536ece4c46bf2ed9823a7e298728310689e54d535226819a7d7fe4b9eeadafd/sed-4.2.2-5.amzn2.0.2.src.rpm
```

### `rpm` package: `setup-2.8.71-10.amzn2.0.1.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls setup-2.8.71-10.amzn2.0.1.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/a048edcb5e7a6552e092a3fd74a073fdd49e7269dd6f7b982088dc71a32cf631/setup-2.8.71-10.amzn2.0.1.src.rpm
```

### `rpm` package: `shared-mime-info-1.8-4.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls shared-mime-info-1.8-4.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/9e51e9ed398518c869e22c71a6cf809d331622958224ced40e8ebf31bf5e810f/shared-mime-info-1.8-4.amzn2.src.rpm
```

### `rpm` package: `sqlite-3.7.17-8.amzn2.1.1.x86_64`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls sqlite-3.7.17-8.amzn2.1.1
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/42efeeae9dcefd0c1a1b0eaafff80300a15588e03c1b5c3e727c2f8912fa8629/sqlite-3.7.17-8.amzn2.1.1.src.rpm
```

### `rpm` package: `system-release-2-13.amzn2.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ yumdownloader --quiet --source --urls system-release-2-13.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/4b1c6b66180103d5b68ebb82a59533f8c260f28e69c3a2b378c11b6e384a38f7/system-release-2-13.amzn2.src.rpm
```

### `rpm` package: `tzdata-2020d-2.amzn2.noarch`

Licenses (from `rpm --query`): Public Domain

Source:

```console
$ yumdownloader --quiet --source --urls tzdata-2020d-2.amzn2.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/524c36fe7d1d5f7939c6ce1eb3b1491b43537756080d6b201dde99e4c88366ae/tzdata-2020d-2.amzn2.src.rpm
```

### `rpm` package: `vim-minimal-8.1.1602-1.amzn2.x86_64`

Licenses (from `rpm --query`): Vim and MIT

Source:

```console
$ yumdownloader --quiet --source --urls vim-minimal-8.1.1602-1.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/55464c9a250bc6772591d5affdf08c9df42fa63858f445546594fca0383741eb/vim-8.1.1602-1.amzn2.src.rpm
```

### `rpm` package: `xz-libs-5.2.2-1.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): LGPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls xz-libs-5.2.2-1.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/bcb9c095602e8f3c64b34b19a8487a9b3dffb2160c8a01d81303eb8201bf2069/xz-5.2.2-1.amzn2.0.2.src.rpm
```

### `rpm` package: `yum-3.4.3-158.amzn2.0.5.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls yum-3.4.3-158.amzn2.0.5.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/517f5774ad6661a925974736ebcb05d62db8093ce75e3161a90d9b3abb71979c/yum-3.4.3-158.amzn2.0.5.src.rpm
```

### `rpm` package: `yum-metadata-parser-1.1.4-10.amzn2.0.2.x86_64`

Licenses (from `rpm --query`): GPLv2

Source:

```console
$ yumdownloader --quiet --source --urls yum-metadata-parser-1.1.4-10.amzn2.0.2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/b710ba0dd68993f774c5fe5325edfec71935fa2f0dba7cd548692b84f31b7988/yum-metadata-parser-1.1.4-10.amzn2.0.2.src.rpm
```

### `rpm` package: `yum-plugin-ovl-1.1.31-46.amzn2.0.1.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls yum-plugin-ovl-1.1.31-46.amzn2.0.1.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/74e03e38d661b26d57dc3fcbd58a66e736b5e8979ccf0493149d0add45dd0416/yum-utils-1.1.31-46.amzn2.0.1.src.rpm
```

### `rpm` package: `yum-plugin-priorities-1.1.31-46.amzn2.0.1.noarch`

Licenses (from `rpm --query`): GPLv2+

Source:

```console
$ yumdownloader --quiet --source --urls yum-plugin-priorities-1.1.31-46.amzn2.0.1.noarch
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/74e03e38d661b26d57dc3fcbd58a66e736b5e8979ccf0493149d0add45dd0416/yum-utils-1.1.31-46.amzn2.0.1.src.rpm
```

### `rpm` package: `zlib-1.2.7-18.amzn2.x86_64`

Licenses (from `rpm --query`): zlib and Boost

Source:

```console
$ yumdownloader --quiet --source --urls zlib-1.2.7-18.amzn2
Enabling amzn2-core-source repository
https://cdn.amazonlinux.com/2/core/2.0/SRPMS/109d2234715c7ad8be9c8e50553d568f5beeca84dcd058376a9e978c1a2a0eac//../../../../../blobstore/b647167c530b0f50390e7cc0820b6705d26f9a415cf0c5ac90c00379c3854636/zlib-1.2.7-18.amzn2.src.rpm
```
