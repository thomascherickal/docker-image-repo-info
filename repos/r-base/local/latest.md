# `r-base:4.3.0`

## Docker Metadata

- Image ID: `sha256:74c13832c443d9ef54d22292957d04d5f2cd57d6d48156af054558779c039300`
- Created: `2023-04-21T19:32:35.969253946Z`
- Virtual Size: ~ 855.15 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Command: `["R"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LC_ALL=en_US.UTF-8`
  - `LANG=en_US.UTF-8`
  - `R_BASE_VERSION=4.3.0`
- Labels:
  - `org.opencontainers.image.authors=Dirk Eddelbuettel <edd@debian.org>`
  - `org.opencontainers.image.licenses=GPL-2.0-or-later`
  - `org.opencontainers.image.source=https://github.com/rocker-org/rocker`
  - `org.opencontainers.image.vendor=Rocker Project`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.3.1-3`

Binary Packages:

- `libacl1:amd64=2.3.1-3`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.3.1-3
'http://http.debian.net/debian/pool/main/a/acl/acl_2.3.1-3.dsc' acl_2.3.1-3.dsc 2508 SHA256:7820eee88cce7244e0b8eb25cc4f51bdf10aff7a6c1a497f3d18c36bdce712cc
'http://http.debian.net/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz' acl_2.3.1.orig.tar.xz 355676 SHA256:c0234042e17f11306c23c038b08e5e070edb7be44bef6697fb8734dcff1c66b1
'http://http.debian.net/debian/pool/main/a/acl/acl_2.3.1.orig.tar.xz.asc' acl_2.3.1.orig.tar.xz.asc 833 SHA256:54fb8fcd6ae6901f2257e18d503e5e18ad956babf8d80d2ea29f280fc7264662
'http://http.debian.net/debian/pool/main/a/acl/acl_2.3.1-3.debian.tar.xz' acl_2.3.1-3.debian.tar.xz 30968 SHA256:2eb052bba784a4b873e951b1f91af2abef62e4bf4b83c93f9821eea26f66c8e2
```

### `dpkg` source package: `apt=2.6.0`

Binary Packages:

- `apt=2.6.0`
- `libapt-pkg6.0:amd64=2.6.0`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.6.0
'http://http.debian.net/debian/pool/main/a/apt/apt_2.6.0.dsc' apt_2.6.0.dsc 2933 SHA256:abadebf55073af5acc2c39d069d5d3889e02e3e3955880dcd471ff906ab59077
'http://http.debian.net/debian/pool/main/a/apt/apt_2.6.0.tar.xz' apt_2.6.0.tar.xz 2328252 SHA256:43467d1ca7de6c0955fd991925433e22fa66230870e5f66c4498675d01776c2a
```

### `dpkg` source package: `attr=1:2.5.1-4`

Binary Packages:

- `libattr1:amd64=1:2.5.1-4`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.5.1-4
'http://http.debian.net/debian/pool/main/a/attr/attr_2.5.1-4.dsc' attr_2.5.1-4.dsc 2477 SHA256:0e1486bff1649602cb5cbb6224dbb641436dc8cd28d5c336ad85d650e07d23dd
'http://http.debian.net/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz' attr_2.5.1.orig.tar.xz 318188 SHA256:db448a626f9313a1a970d636767316a8da32aede70518b8050fa0de7947adc32
'http://http.debian.net/debian/pool/main/a/attr/attr_2.5.1.orig.tar.xz.asc' attr_2.5.1.orig.tar.xz.asc 833 SHA256:67bc632e754efbadba846d0b40138b3fc3e306c3b909a9ba868c6dba1e2689d0
'http://http.debian.net/debian/pool/main/a/attr/attr_2.5.1-4.debian.tar.xz' attr_2.5.1-4.debian.tar.xz 32152 SHA256:aea02a3c980a82804a5a333bf02e9e2737a8c5808671625595511290863d6791
```

### `dpkg` source package: `audit=1:3.0.9-1`

Binary Packages:

- `libaudit-common=1:3.0.9-1`
- `libaudit1:amd64=1:3.0.9-1`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:3.0.9-1
'http://http.debian.net/debian/pool/main/a/audit/audit_3.0.9-1.dsc' audit_3.0.9-1.dsc 2402 SHA256:39d4efdc4e15420f4a1df2b8d7efd17864f2d7da6d84f3122a7c53b6c66a2a1d
'http://http.debian.net/debian/pool/main/a/audit/audit_3.0.9.orig.tar.gz' audit_3.0.9.orig.tar.gz 1210655 SHA256:fd9570444df1573a274ca8ba23590082298a083cfc0618138957f590e845bc78
'http://http.debian.net/debian/pool/main/a/audit/audit_3.0.9-1.debian.tar.xz' audit_3.0.9-1.debian.tar.xz 18784 SHA256:b80d2685b79a617098a3389f41356ffd77d8d62d59bee03b189e31dd9b81580e
```

### `dpkg` source package: `base-files=12.4`

Binary Packages:

- `base-files=12.4`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=12.4
'http://http.debian.net/debian/pool/main/b/base-files/base-files_12.4.dsc' base-files_12.4.dsc 1101 SHA256:7aa2991f4996279d574cbfc001caf6693cab13ed5c94786fd85e9eff8bc65ff4
'http://http.debian.net/debian/pool/main/b/base-files/base-files_12.4.tar.xz' base-files_12.4.tar.xz 66024 SHA256:01d677e63939218e4115a1407b8807f1f6975757b19454b593b5857afc941104
```

### `dpkg` source package: `base-passwd=3.6.1`

Binary Packages:

- `base-passwd=3.6.1`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.6.1
'http://http.debian.net/debian/pool/main/b/base-passwd/base-passwd_3.6.1.dsc' base-passwd_3.6.1.dsc 1740 SHA256:b4e5fcdba73369657b241743033e8e7a65c26da43285503c652fa1436ce75d1f
'http://http.debian.net/debian/pool/main/b/base-passwd/base-passwd_3.6.1.tar.xz' base-passwd_3.6.1.tar.xz 56072 SHA256:6ff369be59d586ba63c0c5fcb00f75f9953fe49db88bc6c6428f2c92866f79af
```

### `dpkg` source package: `bash=5.2.15-2`

Binary Packages:

- `bash=5.2.15-2+b1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `BSD-4-clause-UC`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `Latex2e`
- `MIT-like`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris bash=5.2.15-2
'http://http.debian.net/debian/pool/main/b/bash/bash_5.2.15-2.dsc' bash_5.2.15-2.dsc 2317 SHA256:f51753e946af43eb58549c81e03b35a47af9fe6c6364179ccd4ef862b7c3b2d3
'http://http.debian.net/debian/pool/main/b/bash/bash_5.2.15.orig.tar.gz' bash_5.2.15.orig.tar.gz 9997221 SHA256:7a315bc0e9d90713159e4390ec1096a41e4f33cd8cc3d1a749a8e5ad56600f51
'http://http.debian.net/debian/pool/main/b/bash/bash_5.2.15-2.debian.tar.xz' bash_5.2.15-2.debian.tar.xz 97380 SHA256:998f8ea5b754a734ae7d8306e149c43d713ddfcf49623a036004b729237dbcca
```

### `dpkg` source package: `binutils=2.40-2`

Binary Packages:

- `binutils=2.40-2`
- `binutils-common:amd64=2.40-2`
- `binutils-x86-64-linux-gnu=2.40-2`
- `libbinutils:amd64=2.40-2`
- `libctf-nobfd0:amd64=2.40-2`
- `libctf0:amd64=2.40-2`
- `libgprofng0:amd64=2.40-2`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`, `/usr/share/doc/libgprofng0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.40-2
'http://http.debian.net/debian/pool/main/b/binutils/binutils_2.40-2.dsc' binutils_2.40-2.dsc 11692 SHA256:cd75da7829d819189ba6154d408666373b307e222b393223804c4c4a7156f421
'http://http.debian.net/debian/pool/main/b/binutils/binutils_2.40.orig.tar.xz' binutils_2.40.orig.tar.xz 25364048 SHA256:d78c2d2eb24a9be1e02f8854cb1bd435556d7f584fb6bfb6b07e6527d43fc41d
'http://http.debian.net/debian/pool/main/b/binutils/binutils_2.40-2.debian.tar.xz' binutils_2.40-2.debian.tar.xz 102476 SHA256:a71c03e51d7ac2be8d97daa29dc02e578978c8eeddfd51045502fd008cec8adc
```

### `dpkg` source package: `boot=1.3-28.1-1`

Binary Packages:

- `r-cran-boot=1.3-28.1-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-boot/copyright`)

- `'unlimited distribution'`

Source:

```console
$ apt-get source -qq --print-uris boot=1.3-28.1-1
'http://http.debian.net/debian/pool/main/b/boot/boot_1.3-28.1-1.dsc' boot_1.3-28.1-1.dsc 1816 SHA256:2a77d1f260086849c36782a4016179611543bf74f3b6ffdec10f179c9ce834d1
'http://http.debian.net/debian/pool/main/b/boot/boot_1.3-28.1.orig.tar.gz' boot_1.3-28.1.orig.tar.gz 236854 SHA256:d4cde76fcc8ccc7ffa329de69147b66a6a93a10188e89342fd18207b1d02ff53
'http://http.debian.net/debian/pool/main/b/boot/boot_1.3-28.1-1.debian.tar.xz' boot_1.3-28.1-1.debian.tar.xz 5344 SHA256:b8aa9a51db4cd1d8a7e77a17772e2619cc952fbea54aeec37791d1bbc23b6fed
```

### `dpkg` source package: `brotli=1.0.9-2`

Binary Packages:

- `libbrotli1:amd64=1.0.9-2+b6`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.9-2
'http://http.debian.net/debian/pool/main/b/brotli/brotli_1.0.9-2.dsc' brotli_1.0.9-2.dsc 2261 SHA256:8c4c86748ec9770e08b60233d658593650444b04a452dc5b607ed5b5537b683e
'http://http.debian.net/debian/pool/main/b/brotli/brotli_1.0.9.orig.tar.gz' brotli_1.0.9.orig.tar.gz 486984 SHA256:f9e8d81d0405ba66d181529af42a3354f838c939095ff99930da6aa9cdf6fe46
'http://http.debian.net/debian/pool/main/b/brotli/brotli_1.0.9-2.debian.tar.xz' brotli_1.0.9-2.debian.tar.xz 5552 SHA256:ab81b1db852c8d01e0fa5b0b650bb486f32a232b35336828423af50af6fecca0
```

### `dpkg` source package: `build-essential=12.9`

Binary Packages:

- `build-essential=12.9`

Licenses: (parsed from: `/usr/share/doc/build-essential/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris build-essential=12.9
'http://http.debian.net/debian/pool/main/b/build-essential/build-essential_12.9.dsc' build-essential_12.9.dsc 2220 SHA256:1e4ad67c69001a162b2eb3a2019f037e53c8a1e312073ba1a2110d1e21971555
'http://http.debian.net/debian/pool/main/b/build-essential/build-essential_12.9.tar.xz' build-essential_12.9.tar.xz 51532 SHA256:938da370b4ef883687d141723d1b7470ad76bec7a54158d3d6b9b38f9c9eedb2
```

### `dpkg` source package: `bzip2=1.0.8-5`

Binary Packages:

- `bzip2=1.0.8-5+b1`
- `libbz2-1.0:amd64=1.0.8-5+b1`
- `libbz2-dev:amd64=1.0.8-5+b1`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-5
'http://http.debian.net/debian/pool/main/b/bzip2/bzip2_1.0.8-5.dsc' bzip2_1.0.8-5.dsc 2206 SHA256:ed9c40f4de3f9e064535e15eac1c61a0f606763db98f4579dbc04067b94a8944
'http://http.debian.net/debian/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://http.debian.net/debian/pool/main/b/bzip2/bzip2_1.0.8-5.debian.tar.bz2' bzip2_1.0.8-5.debian.tar.bz2 26787 SHA256:d68c6eba11d70e14319e24ef1451880a03023b2b75364646adb117086db36039
```

### `dpkg` source package: `ca-certificates=20230311`

Binary Packages:

- `ca-certificates=20230311`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20230311
'http://http.debian.net/debian/pool/main/c/ca-certificates/ca-certificates_20230311.dsc' ca-certificates_20230311.dsc 1768 SHA256:bf44adb22fce619310b0f8d7bb6952b0a80907de9e3ecb773143769e98478a3b
'http://http.debian.net/debian/pool/main/c/ca-certificates/ca-certificates_20230311.tar.xz' ca-certificates_20230311.tar.xz 257772 SHA256:83de934afa186e279d1ed08ea0d73f5cf43a6fbfb5f00874b6db3711c64576f3
```

### `dpkg` source package: `cairo=1.16.0-7`

Binary Packages:

- `libcairo2:amd64=1.16.0-7`

Licenses: (parsed from: `/usr/share/doc/libcairo2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris cairo=1.16.0-7
'http://http.debian.net/debian/pool/main/c/cairo/cairo_1.16.0-7.dsc' cairo_1.16.0-7.dsc 2823 SHA256:96b21b7b9c9ab4ae689b1191830b53d0b3c38e5664105c36a3c39dee6bcf29a4
'http://http.debian.net/debian/pool/main/c/cairo/cairo_1.16.0.orig.tar.xz' cairo_1.16.0.orig.tar.xz 41997432 SHA256:5e7b29b3f113ef870d1e3ecf8adf21f923396401604bda16d44be45e66052331
'http://http.debian.net/debian/pool/main/c/cairo/cairo_1.16.0-7.debian.tar.xz' cairo_1.16.0-7.debian.tar.xz 33816 SHA256:af666a040fd54df96885907d0e9a74883396218a620ae03d173f1a3fee4980ea
```

### `dpkg` source package: `cdebconf=0.268`

Binary Packages:

- `libdebconfclient0:amd64=0.268`

Licenses: (parsed from: `/usr/share/doc/libdebconfclient0/copyright`)

- `BSD-2-Clause`
- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.268
'http://http.debian.net/debian/pool/main/c/cdebconf/cdebconf_0.268.dsc' cdebconf_0.268.dsc 2703 SHA256:b712610b4230b1c11749f014f3008dfd604193ab6b550990c8605f4814f770f7
'http://http.debian.net/debian/pool/main/c/cdebconf/cdebconf_0.268.tar.xz' cdebconf_0.268.tar.xz 282628 SHA256:a4a9d32bccef73e908b81047cf387630389aecc84711be116ddcc7180915b467
```

### `dpkg` source package: `cluster=2.1.4-1`

Binary Packages:

- `r-cran-cluster=2.1.4-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-cluster/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris cluster=2.1.4-1
'http://http.debian.net/debian/pool/main/c/cluster/cluster_2.1.4-1.dsc' cluster_2.1.4-1.dsc 1831 SHA256:ce277562952708c41387e9d8bb2bfcd401588fb572ff34bde60dbe23a7539b6e
'http://http.debian.net/debian/pool/main/c/cluster/cluster_2.1.4.orig.tar.gz' cluster_2.1.4.orig.tar.gz 352076 SHA256:c6f10ceca29a176ba833f24ebf71fd451629052c2338398ba286df5689d6f5b6
'http://http.debian.net/debian/pool/main/c/cluster/cluster_2.1.4-1.debian.tar.xz' cluster_2.1.4-1.debian.tar.xz 4312 SHA256:66b4c3d4bbf804497bd58849ca22b59457f57e121c1922877cb9de57d3e9bc34
```

### `dpkg` source package: `codetools=0.2-19-1`

Binary Packages:

- `r-cran-codetools=0.2-19-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-codetools/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris codetools=0.2-19-1
'http://http.debian.net/debian/pool/main/c/codetools/codetools_0.2-19-1.dsc' codetools_0.2-19-1.dsc 1859 SHA256:c2254fd82acbc89bab6588b8d902be70baa79ad716ef261f3b04ba6333058940
'http://http.debian.net/debian/pool/main/c/codetools/codetools_0.2-19.orig.tar.gz' codetools_0.2-19.orig.tar.gz 38235 SHA256:c4b7e567c87f33dad85de92f79641e5e5b5deede6d19a9dfa47133d191782dab
'http://http.debian.net/debian/pool/main/c/codetools/codetools_0.2-19-1.debian.tar.xz' codetools_0.2-19-1.debian.tar.xz 2900 SHA256:23fb4526e3d9b4b18388b255d9deed50bf55b277f4abfdc7bc9b4556092090f1
```

### `dpkg` source package: `coreutils=9.1-1`

Binary Packages:

- `coreutils=9.1-1`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `BSD-4-clause-UC`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris coreutils=9.1-1
'http://http.debian.net/debian/pool/main/c/coreutils/coreutils_9.1-1.dsc' coreutils_9.1-1.dsc 1848 SHA256:2f2fca0a07a1a3f38e3ebeb4cbd97e97e675e77bed84f3e9d0b7e5da4cde75fc
'http://http.debian.net/debian/pool/main/c/coreutils/coreutils_9.1.orig.tar.xz' coreutils_9.1.orig.tar.xz 5712104 SHA256:61a1f410d78ba7e7f37a5a4f50e6d1320aca33375484a3255eddf17a38580423
'http://http.debian.net/debian/pool/main/c/coreutils/coreutils_9.1-1.debian.tar.xz' coreutils_9.1-1.debian.tar.xz 30624 SHA256:45d4ae88d933a7d713ef038943e818a2488e759b6196a409788744cbc6df1832
```

### `dpkg` source package: `curl=7.88.1-8`

Binary Packages:

- `libcurl4:amd64=7.88.1-8`

Licenses: (parsed from: `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `BSD-4-Clause-UC`
- `FSFULLR`
- `GPL-2`
- `GPL-2+ with Autoconf-data exception`
- `GPL-2+ with Libtool exception`
- `GPL-3+ with Autoconf-data exception`
- `ISC`
- `X11`
- `curl`

Source:

```console
$ apt-get source -qq --print-uris curl=7.88.1-8
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.88.1-8.dsc' curl_7.88.1-8.dsc 3159 SHA256:37cb3c88cb357058cd971f2db1ef109d3ec4179e59a4825044cd8fdd9b8469fc
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.88.1.orig.tar.gz' curl_7.88.1.orig.tar.gz 4343562 SHA256:cdb38b72e36bc5d33d5b8810f8018ece1baa29a8f215b4495e495ded82bbf3c7
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.88.1.orig.tar.gz.asc' curl_7.88.1.orig.tar.gz.asc 488 SHA256:7a5a55d7123149a1b357f298cf895bd0a601e3a2807005ef6c95f3752803485f
'http://deb.debian.org/debian/pool/main/c/curl/curl_7.88.1-8.debian.tar.xz' curl_7.88.1-8.debian.tar.xz 45700 SHA256:d223a089ebe48d32c04c2e47a6b73a2bbaa7dff13220456cf7eb625d2286f9a9
```

Other potentially useful URLs:

- https://sources.debian.net/src/curl/7.88.1-8/ (for browsing the source)
- https://sources.debian.net/src/curl/7.88.1-8/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/curl/7.88.1-8/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `cyrus-sasl2=2.1.28+dfsg-10`

Binary Packages:

- `libsasl2-2:amd64=2.1.28+dfsg-10`
- `libsasl2-modules-db:amd64=2.1.28+dfsg-10`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-2-clause`
- `BSD-2.2-clause`
- `BSD-3-clause`
- `BSD-3-clause-JANET`
- `BSD-3-clause-PADL`
- `BSD-4-clause`
- `BSD-4-clause-KTH`
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
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.28+dfsg-10
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-10.dsc' cyrus-sasl2_2.1.28+dfsg-10.dsc 3324 SHA256:cb9c913a6f4716456c93ed205dfef84915a37cf2c994160564e8336e86831d7a
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg.orig.tar.xz' cyrus-sasl2_2.1.28+dfsg.orig.tar.xz 797472 SHA256:a15886d7da5958bd27f35b7c871dd872f6dc5b9917c9b6b15e3de014c7dab3d9
'http://deb.debian.org/debian/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.28%2bdfsg-10.debian.tar.xz' cyrus-sasl2_2.1.28+dfsg-10.debian.tar.xz 97056 SHA256:8c94a1c1982a1603d13ef055b0d2511054db4a43cbb1224702f31e5d985136b1
```

Other potentially useful URLs:

- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg-10/ (for browsing the source)
- https://sources.debian.net/src/cyrus-sasl2/2.1.28+dfsg-10/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/cyrus-sasl2/2.1.28+dfsg-10/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `dash=0.5.12-2`

Binary Packages:

- `dash=0.5.12-2`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `BSD-3-Clause`
- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.12-2
'http://http.debian.net/debian/pool/main/d/dash/dash_0.5.12-2.dsc' dash_0.5.12-2.dsc 1520 SHA256:25c0fb805c735fdb7470ce485ce76dae1a7b6c04efdfb0fdac5eab921cbd78a5
'http://http.debian.net/debian/pool/main/d/dash/dash_0.5.12.orig.tar.gz' dash_0.5.12.orig.tar.gz 246054 SHA256:6a474ac46e8b0b32916c4c60df694c82058d3297d8b385b74508030ca4a8f28a
'http://http.debian.net/debian/pool/main/d/dash/dash_0.5.12-2.debian.tar.xz' dash_0.5.12-2.debian.tar.xz 38512 SHA256:bddd9129215eb60f4cc43a0ffdcc42d8f25e0bd09730520d599a2b7bc492e375
```

### `dpkg` source package: `db5.3=5.3.28+dfsg2-1`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg2-1`

Licenses: (parsed from: `/usr/share/doc/libdb5.3/copyright`)

- `Artistic`
- `BSD-3-clause`
- `BSD-3-clause-fjord`
- `GPL`
- `GPL-3`
- `MIT-old`
- `Ms-PL`
- `Sleepycat`
- `TCL-like`
- `X11`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg2-1
'http://http.debian.net/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-1.dsc' db5.3_5.3.28+dfsg2-1.dsc 2887 SHA256:fe84d3cd7cde381f1c5a18f223377cf84ea7627ced8063ef33ef8fd93f6e09f4
'http://http.debian.net/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2.orig.tar.xz' db5.3_5.3.28+dfsg2.orig.tar.xz 21287688 SHA256:ad41b507415dec8316e828b2230242af2251d2c86eefa3c7aa9ef47c5239ef33
'http://http.debian.net/debian/pool/main/d/db5.3/db5.3_5.3.28%2bdfsg2-1.debian.tar.xz' db5.3_5.3.28+dfsg2-1.debian.tar.xz 34660 SHA256:52cb792fe53138c79a0328ffd1d771e3112791f546fd00e0dcd4b0e3efc5d916
```

### `dpkg` source package: `debconf=1.5.82`

Binary Packages:

- `debconf=1.5.82`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.82
'http://http.debian.net/debian/pool/main/d/debconf/debconf_1.5.82.dsc' debconf_1.5.82.dsc 2035 SHA256:ed6e8cc6e073344a25ab932602b3b814f25cfa1a7bfd69e464f9bad65f250dea
'http://http.debian.net/debian/pool/main/d/debconf/debconf_1.5.82.tar.xz' debconf_1.5.82.tar.xz 571540 SHA256:2d0550c4e2fb98d12055b245907978b28ee2d2b07b62e46be7523384d2ce985e
```

### `dpkg` source package: `debian-archive-keyring=2023.2`

Binary Packages:

- `debian-archive-keyring=2023.2`

Licenses: (parsed from: `/usr/share/doc/debian-archive-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debian-archive-keyring=2023.2
'http://http.debian.net/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2023.2.dsc' debian-archive-keyring_2023.2.dsc 1261 SHA256:f7f78271e6b8596a35e49a5711b99790405552b9bfdc1c995c7944a934c3ee28
'http://http.debian.net/debian/pool/main/d/debian-archive-keyring/debian-archive-keyring_2023.2.tar.xz' debian-archive-keyring_2023.2.tar.xz 177448 SHA256:1abe1f16b8d09d795ede6318cb278df31ba8340ba99368e8664a158fbf76ec29
```

### `dpkg` source package: `debianutils=5.7-0.4`

Binary Packages:

- `debianutils=5.7-0.4`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`
- `GPL-2+`
- `SMAIL-GPL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris debianutils=5.7-0.4
'http://http.debian.net/debian/pool/main/d/debianutils/debianutils_5.7-0.4.dsc' debianutils_5.7-0.4.dsc 1737 SHA256:1cd234cc6449122c5bb8213e7b2919162002ae4234a5c51b2b8e54e82837a047
'http://http.debian.net/debian/pool/main/d/debianutils/debianutils_5.7.orig.tar.gz' debianutils_5.7.orig.tar.gz 257231 SHA256:27ec9e0e7e44dc8ab611aa576330471bacb07e4491ffecf0d3aa6909c92f9022
'http://http.debian.net/debian/pool/main/d/debianutils/debianutils_5.7-0.4.debian.tar.xz' debianutils_5.7-0.4.debian.tar.xz 22412 SHA256:e47eb4fc4cd16fedc8fd741c42acb3af1de19ba42143016adafe61c282ad6771
```

### `dpkg` source package: `diffutils=1:3.8-4`

Binary Packages:

- `diffutils=1:3.8-4`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `FSFAP`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with autoconf exception`
- `GPL-3+ with texinfo exception`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3.0+`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.8-4
'http://http.debian.net/debian/pool/main/d/diffutils/diffutils_3.8-4.dsc' diffutils_3.8-4.dsc 1705 SHA256:783af1a151c2a0f42a8a427693cc4bb16037c0d17282d28672d906f2eab424b8
'http://http.debian.net/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz' diffutils_3.8.orig.tar.xz 1585120 SHA256:a6bdd7d1b31266d11c4f4de6c1b748d4607ab0231af5188fc2533d0ae2438fec
'http://http.debian.net/debian/pool/main/d/diffutils/diffutils_3.8.orig.tar.xz.asc' diffutils_3.8.orig.tar.xz.asc 833 SHA256:500f423d0ffa8d28966d916ed5fc6b79fb160a20ed5cb74eeb1c94a30c340311
'http://http.debian.net/debian/pool/main/d/diffutils/diffutils_3.8-4.debian.tar.xz' diffutils_3.8-4.debian.tar.xz 14428 SHA256:36abe3a3174c32c3646ca6bad212169a322409086c4a98f967bb9ad58f11c8d4
```

### `dpkg` source package: `dpkg=1.21.21`

Binary Packages:

- `dpkg=1.21.21`
- `dpkg-dev=1.21.21`
- `libdpkg-perl=1.21.21`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.21.21
'http://http.debian.net/debian/pool/main/d/dpkg/dpkg_1.21.21.dsc' dpkg_1.21.21.dsc 3061 SHA256:9b8e9bd7bef0be5214f5ef8358b21c53e4ddfa949d399563de865b22d8d6b00c
'http://http.debian.net/debian/pool/main/d/dpkg/dpkg_1.21.21.tar.xz' dpkg_1.21.21.tar.xz 5395164 SHA256:985073817aa0512122f1a7e77598a6b0be168d6c71ac56a3383927eb0813e089
```

### `dpkg` source package: `e2fsprogs=1.46.6-1`

Binary Packages:

- `e2fsprogs=1.46.6-1`
- `libcom-err2:amd64=1.46.6-1`
- `libext2fs2:amd64=1.46.6-1`
- `libss2:amd64=1.46.6-1`
- `logsave=1.46.6-1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `Apache-2`
- `Apache-2.0`
- `BSD-3-Clause`
- `GPL`
- `GPL-2`
- `GPL-2+ with Texinfo exception`
- `ISC`
- `Kazlib`
- `LGPL-2`
- `Latex2e`
- `MIT-US-export`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/e2fsprogs/1.46.6-1/


### `dpkg` source package: `ed=1.19-1`

Binary Packages:

- `ed=1.19-1`

Licenses: (parsed from: `/usr/share/doc/ed/copyright`)

- `BSD-2-Clause`
- `FCONF`
- `FDOC`
- `FLOG`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris ed=1.19-1
'http://http.debian.net/debian/pool/main/e/ed/ed_1.19-1.dsc' ed_1.19-1.dsc 1818 SHA256:01c795ded42ae21c3e6d15a20640422e21f4769eb9b2e796aeef6e75342cbf5c
'http://http.debian.net/debian/pool/main/e/ed/ed_1.19.orig.tar.gz' ed_1.19.orig.tar.gz 89119 SHA256:8e5c3e7c84972e73957ff396b8318a21795f86547dd1fe4ec4232a9e6e44ca1d
'http://http.debian.net/debian/pool/main/e/ed/ed_1.19-1.debian.tar.xz' ed_1.19-1.debian.tar.xz 8528 SHA256:cf83ae1ae31ca91f7d5c34a574f26e3ca8f213ee44cd49c49b284b57d910d4d5
```

### `dpkg` source package: `expat=2.5.0-1`

Binary Packages:

- `libexpat1:amd64=2.5.0-1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.5.0-1
'http://http.debian.net/debian/pool/main/e/expat/expat_2.5.0-1.dsc' expat_2.5.0-1.dsc 1981 SHA256:e7c69b69d720ae1e2971f5edc7fffe274f0047cc61e541cd2013afcc1ba80b81
'http://http.debian.net/debian/pool/main/e/expat/expat_2.5.0.orig.tar.gz' expat_2.5.0.orig.tar.gz 8320988 SHA256:ab00ee05c7067fd10a35c5d2a4922ebba746ddd50ff83b79c828da17bbdf1757
'http://http.debian.net/debian/pool/main/e/expat/expat_2.5.0-1.debian.tar.xz' expat_2.5.0-1.debian.tar.xz 12680 SHA256:232c69ecdf58850b28b5e22374eae4db024d6558f2fbbd57b9af48ab31ce97ed
```

### `dpkg` source package: `findutils=4.9.0-4`

Binary Packages:

- `findutils=4.9.0-4`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `BSD-3-clause`
- `BSD-3-clause and/or GPL-3+`
- `FSFAP`
- `FSFULLR`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL with automake exception`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf-data exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Autoconf-data exception`
- `GPL-3+ with Bison-2.2 exception`
- `ISC`
- `ISC and/or LGPL-2.1+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.9.0-4
'http://http.debian.net/debian/pool/main/f/findutils/findutils_4.9.0-4.dsc' findutils_4.9.0-4.dsc 2304 SHA256:3bb39a6a5f96101f9bb28fed234db186fcec198e064478fef3c0fdf2434f0681
'http://http.debian.net/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz' findutils_4.9.0.orig.tar.xz 2046252 SHA256:a2bfb8c09d436770edc59f50fa483e785b161a3b7b9d547573cb08065fd462fe
'http://http.debian.net/debian/pool/main/f/findutils/findutils_4.9.0.orig.tar.xz.asc' findutils_4.9.0.orig.tar.xz.asc 488 SHA256:924c3719d066eda1b3e47175f8b83e90e9a23f0a639ebe7445621917b283c385
'http://http.debian.net/debian/pool/main/f/findutils/findutils_4.9.0-4.debian.tar.xz' findutils_4.9.0-4.debian.tar.xz 33192 SHA256:ae73dc487b02fb00b2135e43f93733d5561fc8ca7f0997075f21247f6742ec54
```

### `dpkg` source package: `fontconfig=2.14.1-4`

Binary Packages:

- `fontconfig=2.14.1-4`
- `fontconfig-config=2.14.1-4`
- `libfontconfig1:amd64=2.14.1-4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris fontconfig=2.14.1-4
'http://http.debian.net/debian/pool/main/f/fontconfig/fontconfig_2.14.1-4.dsc' fontconfig_2.14.1-4.dsc 2693 SHA256:8bb59d9c96ff8ef77df06dc65273fa398bf248f7e2448a8314989ec01ce74a58
'http://http.debian.net/debian/pool/main/f/fontconfig/fontconfig_2.14.1.orig.tar.xz' fontconfig_2.14.1.orig.tar.xz 1447044 SHA256:298e883f6e11d2c5e6d53c8a8394de58d563902cfab934e6be12fb5a5f361ef0
'http://http.debian.net/debian/pool/main/f/fontconfig/fontconfig_2.14.1-4.debian.tar.xz' fontconfig_2.14.1-4.debian.tar.xz 55972 SHA256:9c2421c04c8d26a006166ad39e0be10de5f2e8149f508b6dbd87f1403275f4a5
```

### `dpkg` source package: `foreign=0.8.84-1`

Binary Packages:

- `r-cran-foreign=0.8.84-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-foreign/copyright`)

- `GPL`
- `GPL `

Source:

```console
$ apt-get source -qq --print-uris foreign=0.8.84-1
'http://http.debian.net/debian/pool/main/f/foreign/foreign_0.8.84-1.dsc' foreign_0.8.84-1.dsc 1838 SHA256:478e0828435c14138b855048b19bab4486cfb1bba26ddc209d65bb21e5ca97c9
'http://http.debian.net/debian/pool/main/f/foreign/foreign_0.8.84.orig.tar.gz' foreign_0.8.84.orig.tar.gz 361712 SHA256:17edf302c7568a122dc496a61a4a886ef7c02224a235d945b473611c79c98549
'http://http.debian.net/debian/pool/main/f/foreign/foreign_0.8.84-1.debian.tar.xz' foreign_0.8.84-1.debian.tar.xz 4332 SHA256:ab0493afc06eec6460dd35a3dca7f0a6d05329ab96f21f03420069239783df48
```

### `dpkg` source package: `freetype=2.12.1+dfsg-4`

Binary Packages:

- `libfreetype6:amd64=2.12.1+dfsg-4`

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
$ apt-get source -qq --print-uris freetype=2.12.1+dfsg-4
'http://http.debian.net/debian/pool/main/f/freetype/freetype_2.12.1%2bdfsg-4.dsc' freetype_2.12.1+dfsg-4.dsc 3767 SHA256:364461f41897ae1c37ee9d6a9624a5d8db594df55dd8f87df611ed1053b736b7
'http://http.debian.net/debian/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2demos.tar.xz' freetype_2.12.1+dfsg.orig-ft2demos.tar.xz 263656 SHA256:ce729d97f166a919a6a3037c949af01d5d6e1783614024d72683153f0bc5ef05
'http://http.debian.net/debian/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2demos.tar.xz.asc' freetype_2.12.1+dfsg.orig-ft2demos.tar.xz.asc 833 SHA256:0303e45fe1dc659f14353c276ac0ea1025b30e19ac8138c52d5df79b55726f14
'http://http.debian.net/debian/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2docs.tar.xz' freetype_2.12.1+dfsg.orig-ft2docs.tar.xz 2038632 SHA256:6664a32e4eedaa89f45422c1150e32da46fd301c972cbfd19d2dcc6dd96f07d1
'http://http.debian.net/debian/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig-ft2docs.tar.xz.asc' freetype_2.12.1+dfsg.orig-ft2docs.tar.xz.asc 833 SHA256:e686683830c782c30cdd83278c8d5ed7ab930ae7d548682565b706322f44007f
'http://http.debian.net/debian/pool/main/f/freetype/freetype_2.12.1%2bdfsg.orig.tar.xz' freetype_2.12.1+dfsg.orig.tar.xz 2188492 SHA256:7dedb6b9adf331559daea614a83b8de42a753e685ec8e1c4bdb4529eb880b0d1
'http://http.debian.net/debian/pool/main/f/freetype/freetype_2.12.1%2bdfsg-4.debian.tar.xz' freetype_2.12.1+dfsg-4.debian.tar.xz 43248 SHA256:05ada04cbc7cb18e087d6abffaa748ecc7fa0f6c9537edaffb41c863ec4fb5f5
```

### `dpkg` source package: `fribidi=1.0.8-2.1`

Binary Packages:

- `libfribidi0:amd64=1.0.8-2.1`

Licenses: (parsed from: `/usr/share/doc/libfribidi0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris fribidi=1.0.8-2.1
'http://http.debian.net/debian/pool/main/f/fribidi/fribidi_1.0.8-2.1.dsc' fribidi_1.0.8-2.1.dsc 2457 SHA256:7efd56752103ca3ea6190bbc3ee49b613bc131cd7551fb64c6e9d233d4496553
'http://http.debian.net/debian/pool/main/f/fribidi/fribidi_1.0.8.orig.tar.bz2' fribidi_1.0.8.orig.tar.bz2 2077095 SHA256:94c7b68d86ad2a9613b4dcffe7bbeb03523d63b5b37918bdf2e4ef34195c1e6c
'http://http.debian.net/debian/pool/main/f/fribidi/fribidi_1.0.8-2.1.debian.tar.xz' fribidi_1.0.8-2.1.debian.tar.xz 10348 SHA256:7e80ba37a8ef1ce98c73a888b56a3f1192fbd0f43c46b626026106065bd2993a
```

### `dpkg` source package: `gcc-12=12.2.0-14`

Binary Packages:

- `cpp-12=12.2.0-14`
- `g++-12=12.2.0-14`
- `gcc-12=12.2.0-14`
- `gcc-12-base:amd64=12.2.0-14`
- `gfortran-12=12.2.0-14`
- `libasan8:amd64=12.2.0-14`
- `libatomic1:amd64=12.2.0-14`
- `libcc1-0:amd64=12.2.0-14`
- `libgcc-12-dev:amd64=12.2.0-14`
- `libgcc-s1:amd64=12.2.0-14`
- `libgfortran-12-dev:amd64=12.2.0-14`
- `libgfortran5:amd64=12.2.0-14`
- `libgomp1:amd64=12.2.0-14`
- `libitm1:amd64=12.2.0-14`
- `liblsan0:amd64=12.2.0-14`
- `libquadmath0:amd64=12.2.0-14`
- `libstdc++-12-dev:amd64=12.2.0-14`
- `libstdc++6:amd64=12.2.0-14`
- `libtsan2:amd64=12.2.0-14`
- `libubsan1:amd64=12.2.0-14`

Licenses: (parsed from: `/usr/share/doc/cpp-12/copyright`, `/usr/share/doc/g++-12/copyright`, `/usr/share/doc/gcc-12/copyright`, `/usr/share/doc/gcc-12-base/copyright`, `/usr/share/doc/gfortran-12/copyright`, `/usr/share/doc/libasan8/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-12-dev/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgfortran-12-dev/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++-12-dev/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan2/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-12=12.2.0-14
'http://http.debian.net/debian/pool/main/g/gcc-12/gcc-12_12.2.0-14.dsc' gcc-12_12.2.0-14.dsc 27302 SHA256:b11f8eca97c60a8e55f0cfd4dffdd52560698909fdcde3eacb5241ce1f1f09ad
'http://http.debian.net/debian/pool/main/g/gcc-12/gcc-12_12.2.0.orig.tar.gz' gcc-12_12.2.0.orig.tar.gz 87090343 SHA256:b8298be16aeeb96a889c6afed0a8e2241b47452e89cc81fe65ea849d5c740fcb
'http://http.debian.net/debian/pool/main/g/gcc-12/gcc-12_12.2.0-14.debian.tar.xz' gcc-12_12.2.0-14.debian.tar.xz 1664492 SHA256:e6f33b48753d62be04188a30c69883061a7ad1576c22166e79be2c9e7aa258f2
```

### `dpkg` source package: `gcc-defaults=1.203`

Binary Packages:

- `cpp=4:12.2.0-3`
- `g++=4:12.2.0-3`
- `gcc=4:12.2.0-3`
- `gfortran=4:12.2.0-3`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`, `/usr/share/doc/gfortran/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.203
'http://http.debian.net/debian/pool/main/g/gcc-defaults/gcc-defaults_1.203.dsc' gcc-defaults_1.203.dsc 12592 SHA256:39417c8e6cf5bfa22b1c58f004e9f7630725ace3138a216ba64ec75d83c3fceb
'http://http.debian.net/debian/pool/main/g/gcc-defaults/gcc-defaults_1.203.tar.xz' gcc-defaults_1.203.tar.xz 45208 SHA256:bbf861f5502592b91602392123b482f9fb521948a8994057d152486f78b200b0
```

### `dpkg` source package: `gdbm=1.23-3`

Binary Packages:

- `libgdbm-compat4:amd64=1.23-3`
- `libgdbm6:amd64=1.23-3`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.23-3
'http://http.debian.net/debian/pool/main/g/gdbm/gdbm_1.23-3.dsc' gdbm_1.23-3.dsc 2583 SHA256:3e4a52655a1b65c51d33e032913edda3423dcae8cc282c16a455a0afd2d2738d
'http://http.debian.net/debian/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz' gdbm_1.23.orig.tar.gz 1115854 SHA256:74b1081d21fff13ae4bd7c16e5d6e504a4c26f7cde1dca0d963a484174bbcacd
'http://http.debian.net/debian/pool/main/g/gdbm/gdbm_1.23.orig.tar.gz.asc' gdbm_1.23.orig.tar.gz.asc 181 SHA256:64ebb68cc68e8915d62cb20ea40323c00b56051f844589ee0a52169fff34cecb
'http://http.debian.net/debian/pool/main/g/gdbm/gdbm_1.23-3.debian.tar.xz' gdbm_1.23-3.debian.tar.xz 18552 SHA256:a0ff17befcbd7c4b361cfe0d821a7a71334102a9c423537bd57f60f18f6802ea
```

### `dpkg` source package: `glib2.0=2.74.6-2`

Binary Packages:

- `libglib2.0-0:amd64=2.74.6-2`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `AFL-2.0`
- `Apache-2.0`
- `Apache-2.0 with LLVM exception`
- `BSD-3-clause-pcre`
- `CC-BY-SA-3.0`
- `CC0-1.0`
- `Expat`
- `FSFULLR`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `Iconv-PD`
- `Janik-permissive`
- `Kuchling-PD`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `Mingw-PD`
- `Old-GLib-Tests-permissive`
- `Plumb-PD`
- `Unicode-DFS-2016`
- `bzip2-1.0.6`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.74.6-2
'http://http.debian.net/debian/pool/main/g/glib2.0/glib2.0_2.74.6-2.dsc' glib2.0_2.74.6-2.dsc 3667 SHA256:3643bdb48d558e0cc8090dd29042182309595aa554dc24a319182c60a0c964e2
'http://http.debian.net/debian/pool/main/g/glib2.0/glib2.0_2.74.6.orig-unicode-data.tar.xz' glib2.0_2.74.6.orig-unicode-data.tar.xz 267596 SHA256:dabcaff9298aa111a94e580561d2f29371f3e61b356c925ec5e0792df2b11ff2
'http://http.debian.net/debian/pool/main/g/glib2.0/glib2.0_2.74.6.orig.tar.xz' glib2.0_2.74.6.orig.tar.xz 5217312 SHA256:069cf7e51cd261eb163aaf06c8d1754c6835f31252180aff5814e5afc7757fbc
'http://http.debian.net/debian/pool/main/g/glib2.0/glib2.0_2.74.6-2.debian.tar.xz' glib2.0_2.74.6-2.debian.tar.xz 120348 SHA256:cfd5202bd548def51f5d3c59657eba8f62c88c7339db635445bf0325043c81e6
```

### `dpkg` source package: `glibc=2.36-9`

Binary Packages:

- `libc-bin=2.36-9`
- `libc-dev-bin=2.36-9`
- `libc-l10n=2.36-9`
- `libc6:amd64=2.36-9`
- `libc6-dev:amd64=2.36-9`
- `locales=2.36-9`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc-l10n/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`, `/usr/share/doc/locales/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.36-9
'http://http.debian.net/debian/pool/main/g/glibc/glibc_2.36-9.dsc' glibc_2.36-9.dsc 9729 SHA256:dbb3e0a62b277118f0268171fae750c2d0bf37749bb42289380a1e679758a6dd
'http://http.debian.net/debian/pool/main/g/glibc/glibc_2.36.orig.tar.xz' glibc_2.36.orig.tar.xz 19363988 SHA256:a543c02070d46ccaf866957efd13f10c924daa74c86a90a0254db09a92a708ee
'http://http.debian.net/debian/pool/main/g/glibc/glibc_2.36-9.debian.tar.xz' glibc_2.36-9.debian.tar.xz 836988 SHA256:e87e7df56380102fad8a011b352eefa9d28bf2d241142d451c0e99452f4d61ae
```

### `dpkg` source package: `gmp=2:6.2.1+dfsg1-1.1`

Binary Packages:

- `libgmp10:amd64=2:6.2.1+dfsg1-1.1`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Bison exception`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.1+dfsg1-1.1
'http://http.debian.net/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.1.dsc' gmp_6.2.1+dfsg1-1.1.dsc 2238 SHA256:2831ed4f83bc3304c2403474b335652ab2dc507cd517de44414d9142171748f0
'http://http.debian.net/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1.orig.tar.xz' gmp_6.2.1+dfsg1.orig.tar.xz 1787428 SHA256:471b9e463e04362a0124f215afc5f0a4b99caedeeb62634c61bbc12988efa64c
'http://http.debian.net/debian/pool/main/g/gmp/gmp_6.2.1%2bdfsg1-1.1.debian.tar.xz' gmp_6.2.1+dfsg1-1.1.debian.tar.xz 19444 SHA256:4e3e324d72fe688e409c716d33b35aa8657f6016cc1aabd5d9c7ec137412e5ef
```

### `dpkg` source package: `gnupg2=2.2.40-1.1`

Binary Packages:

- `gpgv=2.2.40-1.1`

Licenses: (parsed from: `/usr/share/doc/gpgv/copyright`)

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
$ apt-get source -qq --print-uris gnupg2=2.2.40-1.1
'http://http.debian.net/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.1.dsc' gnupg2_2.2.40-1.1.dsc 3832 SHA256:89bdffd4176066d37fb5d250a1e5512c428529d10f13413a12893f86a757697f
'http://http.debian.net/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2' gnupg2_2.2.40.orig.tar.bz2 7301631 SHA256:1164b29a75e8ab93ea15033300149e1872a7ef6bdda3d7c78229a735f8204c28
'http://http.debian.net/debian/pool/main/g/gnupg2/gnupg2_2.2.40.orig.tar.bz2.asc' gnupg2_2.2.40.orig.tar.bz2.asc 228 SHA256:3907dc165299cd53c0b4aec862323c3bce6037c411600ec87dc5eed7a55eba4a
'http://http.debian.net/debian/pool/main/g/gnupg2/gnupg2_2.2.40-1.1.debian.tar.xz' gnupg2_2.2.40-1.1.debian.tar.xz 62368 SHA256:356b7c86afdbaab286c5b92816cd1e1f4616cb67d22407c616618ef4d1680a9b
```

### `dpkg` source package: `gnutls28=3.7.9-1`

Binary Packages:

- `libgnutls30:amd64=3.7.9-1`

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
$ apt-get source -qq --print-uris gnutls28=3.7.9-1
'http://http.debian.net/debian/pool/main/g/gnutls28/gnutls28_3.7.9-1.dsc' gnutls28_3.7.9-1.dsc 3386 SHA256:6d8f16e98f74421ff459e81244de340d85f359b9ef8248ed300d84a38ad10c9a
'http://http.debian.net/debian/pool/main/g/gnutls28/gnutls28_3.7.9.orig.tar.xz' gnutls28_3.7.9.orig.tar.xz 6377212 SHA256:aaa03416cdbd54eb155187b359e3ec3ed52ec73df4df35a0edd49429ff64d844
'http://http.debian.net/debian/pool/main/g/gnutls28/gnutls28_3.7.9.orig.tar.xz.asc' gnutls28_3.7.9.orig.tar.xz.asc 996 SHA256:da4a96b14edd3cd44971a36ba1e976af1057e57a2d6c21b0cc7025c983ee84cc
'http://http.debian.net/debian/pool/main/g/gnutls28/gnutls28_3.7.9-1.debian.tar.xz' gnutls28_3.7.9-1.debian.tar.xz 85804 SHA256:cea9b352d2eec06333448773f36b0de2462ea41465fd21785c345cb7c0342b26
```

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
'http://http.debian.net/debian/pool/main/g/graphite2/graphite2_1.3.14-1.dsc' graphite2_1.3.14-1.dsc 2608 SHA256:3a622b8aa7d693d6d60d3cd29b49a7d9d7873ea6089cb52ce7a223261e605152
'http://http.debian.net/debian/pool/main/g/graphite2/graphite2_1.3.14.orig.tar.gz' graphite2_1.3.14.orig.tar.gz 6629829 SHA256:7a3b342c5681921ce2e0c2496509d30b5b078399d5a7bd2358f95166d57d91df
'http://http.debian.net/debian/pool/main/g/graphite2/graphite2_1.3.14-1.debian.tar.xz' graphite2_1.3.14-1.debian.tar.xz 12068 SHA256:94d584e6c748fa7e2f851c3bb39cb2cdb437b4f91d1d636f3d842357724cd9bd
```

### `dpkg` source package: `grep=3.8-5`

Binary Packages:

- `grep=3.8-5`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.8-5
'http://http.debian.net/debian/pool/main/g/grep/grep_3.8-5.dsc' grep_3.8-5.dsc 1608 SHA256:12b8d98e0112683e0439e61d5b3b7cdeafdfc579641c35aa25199bc0431061d0
'http://http.debian.net/debian/pool/main/g/grep/grep_3.8.orig.tar.xz' grep_3.8.orig.tar.xz 1709536 SHA256:498d7cc1b4fb081904d87343febb73475cf771e424fb7e6141aff66013abc382
'http://http.debian.net/debian/pool/main/g/grep/grep_3.8.orig.tar.xz.asc' grep_3.8.orig.tar.xz.asc 833 SHA256:347aec924499df3fa41a0d782f3cd3e4a51a15de98b44eaab04084cd34060cd0
'http://http.debian.net/debian/pool/main/g/grep/grep_3.8-5.debian.tar.xz' grep_3.8-5.debian.tar.xz 21048 SHA256:c49bb8ab9ed98fd1aa76f8af838ac9abd664e65042c0e40f99983c60ba03fba1
```

### `dpkg` source package: `gzip=1.12-1`

Binary Packages:

- `gzip=1.12-1`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `FSF-manpages`
- `GFDL-1.3+-no-invariant`
- `GFDL-3`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.12-1
'http://http.debian.net/debian/pool/main/g/gzip/gzip_1.12-1.dsc' gzip_1.12-1.dsc 2009 SHA256:49a287787a0b4fc816eb576c011c472d1f630ec1778dfa120bd7fce4a844c253
'http://http.debian.net/debian/pool/main/g/gzip/gzip_1.12.orig.tar.xz' gzip_1.12.orig.tar.xz 825548 SHA256:ce5e03e519f637e1f814011ace35c4f87b33c0bbabeec35baf5fbd3479e91956
'http://http.debian.net/debian/pool/main/g/gzip/gzip_1.12.orig.tar.xz.asc' gzip_1.12.orig.tar.xz.asc 833 SHA256:3ed9ab54452576e0be0d477c772c9f47baa36415133fef7dd1fcf7b15480ba32
'http://http.debian.net/debian/pool/main/g/gzip/gzip_1.12-1.debian.tar.xz' gzip_1.12-1.debian.tar.xz 18736 SHA256:fcf2317e8eeddd66766ec5f3853025b109bd13815ec86ed6563e1af68d17193a
```

### `dpkg` source package: `harfbuzz=6.0.0+dfsg-3`

Binary Packages:

- `libharfbuzz0b:amd64=6.0.0+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libharfbuzz0b/copyright`)

- `Apache-2.0`
- `CC0-1.0`
- `Expat`
- `FSFAP`
- `FSFUL`
- `FSFULLR`
- `GPL-2`
- `GPL-2+ with AutoConf exception`
- `GPL-2+ with Font exception`
- `GPL-2+ with LibTool exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with AutoConf exception`
- `ISC`
- `LGPL-2.1`
- `LGPL-2.1+`
- `MIT`
- `Monotype`
- `OFL-1.1`
- `UFL-1.0`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris harfbuzz=6.0.0+dfsg-3
'http://http.debian.net/debian/pool/main/h/harfbuzz/harfbuzz_6.0.0%2bdfsg-3.dsc' harfbuzz_6.0.0+dfsg-3.dsc 2810 SHA256:a03b89402656feb6e9b1439f69b55f3cfbd7b1c70a71e18819f0396d1a6fd607
'http://http.debian.net/debian/pool/main/h/harfbuzz/harfbuzz_6.0.0%2bdfsg.orig.tar.xz' harfbuzz_6.0.0+dfsg.orig.tar.xz 18981700 SHA256:89266cb363e49b6aa999eda04ca25b0d234a69ad9304679631371f4697652368
'http://http.debian.net/debian/pool/main/h/harfbuzz/harfbuzz_6.0.0%2bdfsg-3.debian.tar.xz' harfbuzz_6.0.0+dfsg-3.debian.tar.xz 19084 SHA256:0cabb3f1910d66d84967d65e4eaef9aa5b056e4d279ba46444d3f9c3e25a96ac
```

### `dpkg` source package: `hostname=3.23+nmu1`

Binary Packages:

- `hostname=3.23+nmu1`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23+nmu1
'http://http.debian.net/debian/pool/main/h/hostname/hostname_3.23%2bnmu1.dsc' hostname_3.23+nmu1.dsc 1281 SHA256:56f2189eaeee638e86d29a05356e7001632e33b2132a41a4634a9ff839264ea6
'http://http.debian.net/debian/pool/main/h/hostname/hostname_3.23%2bnmu1.tar.xz' hostname_3.23+nmu1.tar.xz 12876 SHA256:f3fb39f30b00ba7dba2cec013195d7e1bb215f241153208ccd52da3eedfe7a7d
```

### `dpkg` source package: `icu=72.1-3`

Binary Packages:

- `icu-devtools=72.1-3`
- `libicu-dev:amd64=72.1-3`
- `libicu72:amd64=72.1-3`

Licenses: (parsed from: `/usr/share/doc/icu-devtools/copyright`, `/usr/share/doc/libicu-dev/copyright`, `/usr/share/doc/libicu72/copyright`)

- `GPL-3`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris icu=72.1-3
'http://http.debian.net/debian/pool/main/i/icu/icu_72.1-3.dsc' icu_72.1-3.dsc 2252 SHA256:fdb557502398e70fe74502f5c2e5ec436b7c7f267420fba7ceaca7ce501dbf6e
'http://http.debian.net/debian/pool/main/i/icu/icu_72.1.orig.tar.gz' icu_72.1.orig.tar.gz 26303933 SHA256:a2d2d38217092a7ed56635e34467f92f976b370e20182ad325edea6681a71d68
'http://http.debian.net/debian/pool/main/i/icu/icu_72.1.orig.tar.gz.asc' icu_72.1.orig.tar.gz.asc 659 SHA256:87b6ff610d587292cec0444fa8cbbfb12994cb89bade40578f5ba6470de245c7
'http://http.debian.net/debian/pool/main/i/icu/icu_72.1-3.debian.tar.xz' icu_72.1-3.debian.tar.xz 62172 SHA256:e7b9edb525c7c94043577920dc5f1cc63c18e362a07b44d3e3ec39e89f174bb6
```

### `dpkg` source package: `init-system-helpers=1.65.2`

Binary Packages:

- `init-system-helpers=1.65.2`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.65.2
'http://http.debian.net/debian/pool/main/i/init-system-helpers/init-system-helpers_1.65.2.dsc' init-system-helpers_1.65.2.dsc 2195 SHA256:3889593844b232df78f3f886aed6d8351fe0539cee8d15a721d4b682c6a83538
'http://http.debian.net/debian/pool/main/i/init-system-helpers/init-system-helpers_1.65.2.tar.xz' init-system-helpers_1.65.2.tar.xz 44400 SHA256:888bd5642f31396fd2b1a6f9c8f56ba5f6651fb599dae2b9eecf239902162cae
```

### `dpkg` source package: `isl=0.25-1`

Binary Packages:

- `libisl23:amd64=0.25-1`

Licenses: (parsed from: `/usr/share/doc/libisl23/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.25-1
'http://http.debian.net/debian/pool/main/i/isl/isl_0.25-1.dsc' isl_0.25-1.dsc 1832 SHA256:e4f18c3fc65369b5fc8870b2c5f30cb9c3f2ec9f50f8e29156cc06cce2dbe437
'http://http.debian.net/debian/pool/main/i/isl/isl_0.25.orig.tar.xz' isl_0.25.orig.tar.xz 1977048 SHA256:be7b210647ccadf90a2f0b000fca11a4d40546374a850db67adb32fad4b230d9
'http://http.debian.net/debian/pool/main/i/isl/isl_0.25-1.debian.tar.xz' isl_0.25-1.debian.tar.xz 24344 SHA256:22ceb736a06ed290ea06c4f6c81ef8ed944b3738aa496c1961d193edfc847f30
```

### `dpkg` source package: `jansson=2.14-2`

Binary Packages:

- `libjansson4:amd64=2.14-2`

Licenses: (parsed from: `/usr/share/doc/libjansson4/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris jansson=2.14-2
'http://http.debian.net/debian/pool/main/j/jansson/jansson_2.14-2.dsc' jansson_2.14-2.dsc 1980 SHA256:6296ddd9c0a022bd1b70074aefb171cfcdf5694a04ffd32b35fd66097621af87
'http://http.debian.net/debian/pool/main/j/jansson/jansson_2.14.orig.tar.gz' jansson_2.14.orig.tar.gz 141500 SHA256:c739578bf6b764aa0752db9a2fdadcfe921c78f1228c7ec0bb47fa804c55d17b
'http://http.debian.net/debian/pool/main/j/jansson/jansson_2.14-2.debian.tar.xz' jansson_2.14-2.debian.tar.xz 5428 SHA256:e89fe4fd8221f6934ddb50f2e7f8404311928d0e23e49a5599f3d3d14ee8cb88
```

### `dpkg` source package: `jbigkit=2.1-6.1`

Binary Packages:

- `libjbig0:amd64=2.1-6.1`

Licenses: (parsed from: `/usr/share/doc/libjbig0/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris jbigkit=2.1-6.1
'http://http.debian.net/debian/pool/main/j/jbigkit/jbigkit_2.1-6.1.dsc' jbigkit_2.1-6.1.dsc 2089 SHA256:8dea586c47cb4b2436f77fd33ef4a702b9da936d74de8332a72a8ddbe8124e09
'http://http.debian.net/debian/pool/main/j/jbigkit/jbigkit_2.1.orig.tar.gz' jbigkit_2.1.orig.tar.gz 438710 SHA256:de7106b6bfaf495d6865c7dd7ac6ca1381bd12e0d81405ea81e7f2167263d932
'http://http.debian.net/debian/pool/main/j/jbigkit/jbigkit_2.1-6.1.debian.tar.xz' jbigkit_2.1-6.1.debian.tar.xz 9244 SHA256:c9ba99e84d18b1affdc97b26b625721ed06b41a92996d9b426b62c0dbe3868cd
```

### `dpkg` source package: `kernsmooth=2.23-20-1`

Binary Packages:

- `r-cran-kernsmooth=2.23-20-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris kernsmooth=2.23-20-1
'http://http.debian.net/debian/pool/main/k/kernsmooth/kernsmooth_2.23-20-1.dsc' kernsmooth_2.23-20-1.dsc 1891 SHA256:2b09ccd2ac359365bd3cb32aa688b1cabb89beb2e25e21a5768da6604cf11c1d
'http://http.debian.net/debian/pool/main/k/kernsmooth/kernsmooth_2.23-20.orig.tar.gz' kernsmooth_2.23-20.orig.tar.gz 25946 SHA256:20eb75051e2473933d41eedc9945b03c632847fd581e2207d452cf317fa5ec39
'http://http.debian.net/debian/pool/main/k/kernsmooth/kernsmooth_2.23-20-1.debian.tar.xz' kernsmooth_2.23-20-1.debian.tar.xz 3356 SHA256:900201f86061c4ebdbe9f0bfd888574169fb0ed5f254e993a00c80a0b59a8942
```

### `dpkg` source package: `keyutils=1.6.3-2`

Binary Packages:

- `libkeyutils1:amd64=1.6.3-2`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6.3-2
'http://http.debian.net/debian/pool/main/k/keyutils/keyutils_1.6.3-2.dsc' keyutils_1.6.3-2.dsc 2079 SHA256:77e6f0e5018f0f6cfb5a3689d7f185a014b2437d0a097609ffda32bfd3a64f28
'http://http.debian.net/debian/pool/main/k/keyutils/keyutils_1.6.3.orig.tar.gz' keyutils_1.6.3.orig.tar.gz 137022 SHA256:a61d5706136ae4c05bd48f86186bcfdbd88dd8bd5107e3e195c924cfc1b39bb4
'http://http.debian.net/debian/pool/main/k/keyutils/keyutils_1.6.3-2.debian.tar.xz' keyutils_1.6.3-2.debian.tar.xz 13196 SHA256:9b9b40729465d4895860838e82e13d2ee4ffc44a97c9acd1d47a51bd33ade899
```

### `dpkg` source package: `krb5=1.20.1-1`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.20.1-1+b1`
- `libk5crypto3:amd64=1.20.1-1+b1`
- `libkrb5-3:amd64=1.20.1-1+b1`
- `libkrb5support0:amd64=1.20.1-1+b1`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.20.1-1
'http://http.debian.net/debian/pool/main/k/krb5/krb5_1.20.1-1.dsc' krb5_1.20.1-1.dsc 3168 SHA256:dca082e1aac1ae5f7622b524942a305ad7c93e584f3a67db02f48542eb5b415a
'http://http.debian.net/debian/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz' krb5_1.20.1.orig.tar.gz 8661660 SHA256:704aed49b19eb5a7178b34b2873620ec299db08752d6a8574f95d41879ab8851
'http://http.debian.net/debian/pool/main/k/krb5/krb5_1.20.1.orig.tar.gz.asc' krb5_1.20.1.orig.tar.gz.asc 833 SHA256:2afeec5dbc586cc40b7975645e02b4c41c4d719dd02213e828c72d8239d55666
'http://http.debian.net/debian/pool/main/k/krb5/krb5_1.20.1-1.debian.tar.xz' krb5_1.20.1-1.debian.tar.xz 99428 SHA256:19c5f3e66ee1c22f05d86e1ec521e08f885105db4d42403593db6e6db38fad13
```

### `dpkg` source package: `lapack=3.11.0-2`

Binary Packages:

- `libblas-dev:amd64=3.11.0-2`
- `libblas3:amd64=3.11.0-2`
- `liblapack-dev:amd64=3.11.0-2`
- `liblapack3:amd64=3.11.0-2`

Licenses: (parsed from: `/usr/share/doc/libblas-dev/copyright`, `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack-dev/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.11.0-2
'http://http.debian.net/debian/pool/main/l/lapack/lapack_3.11.0-2.dsc' lapack_3.11.0-2.dsc 3307 SHA256:664d828b9015f9d7db00dd53d42ee7ae0b30e90725fa5300fce35a833ecd5ecf
'http://http.debian.net/debian/pool/main/l/lapack/lapack_3.11.0.orig.tar.gz' lapack_3.11.0.orig.tar.gz 7723808 SHA256:4b9ba79bfd4921ca820e83979db76ab3363155709444a787979e81c22285ffa9
'http://http.debian.net/debian/pool/main/l/lapack/lapack_3.11.0-2.debian.tar.xz' lapack_3.11.0-2.debian.tar.xz 32936 SHA256:36825c7cb768267fe7d322145a4160d4e564a21730b16d78a59090102cc35dfd
```

### `dpkg` source package: `lattice=0.20-45-3`

Binary Packages:

- `r-cran-lattice=0.20-45-3`

Licenses: (parsed from: `/usr/share/doc/r-cran-lattice/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris lattice=0.20-45-3
'http://http.debian.net/debian/pool/main/l/lattice/lattice_0.20-45-3.dsc' lattice_0.20-45-3.dsc 1845 SHA256:aa5d7456ac0a384fddb6a67685ec2ea39107d533c6320dc574916a52447602de
'http://http.debian.net/debian/pool/main/l/lattice/lattice_0.20-45.orig.tar.gz' lattice_0.20-45.orig.tar.gz 399470 SHA256:22388d92bdb7d3959da84d7308d9026dd8226ef07580783729e8ad2f7d7507ad
'http://http.debian.net/debian/pool/main/l/lattice/lattice_0.20-45-3.debian.tar.xz' lattice_0.20-45-3.debian.tar.xz 5276 SHA256:a7a6e17033f0b0ef5738388e5a21c4bbaf05ceea29c878bf32dadc27c0461899
```

### `dpkg` source package: `lerc=4.0.0+ds-2`

Binary Packages:

- `liblerc4:amd64=4.0.0+ds-2`

Licenses: (parsed from: `/usr/share/doc/liblerc4/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris lerc=4.0.0+ds-2
'http://http.debian.net/debian/pool/main/l/lerc/lerc_4.0.0%2bds-2.dsc' lerc_4.0.0+ds-2.dsc 2224 SHA256:61c32adc1590f930af4b94b151e6a0a8569ace7d7a4f1961eb049f209b47a417
'http://http.debian.net/debian/pool/main/l/lerc/lerc_4.0.0%2bds.orig.tar.xz' lerc_4.0.0+ds.orig.tar.xz 348140 SHA256:acf855502fd3b950ee78f0b67bc9e9b39316b3526fbf6d8b8b1a9482fb756723
'http://http.debian.net/debian/pool/main/l/lerc/lerc_4.0.0%2bds-2.debian.tar.xz' lerc_4.0.0+ds-2.debian.tar.xz 7780 SHA256:b5676df41934c3c95447a66f766ac8f536cf9fa88063c93b0201e6b4fd25aff6
```

### `dpkg` source package: `less=590-1.2`

Binary Packages:

- `less=590-1.2`

Licenses: (parsed from: `/usr/share/doc/less/copyright`)

- `GPL-3`
- `GPL-3+`
- `Less`
- `Less,`
- `Spencer-86`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris less=590-1.2
'http://deb.debian.org/debian/pool/main/l/less/less_590-1.2.dsc' less_590-1.2.dsc 1944 SHA256:6290f5e8607fb61719d37a50c627fc25d96f8caf19502d7137ade61a1d56a0ef
'http://deb.debian.org/debian/pool/main/l/less/less_590.orig.tar.gz' less_590.orig.tar.gz 352574 SHA256:6aadf54be8bf57d0e2999a3c5d67b1de63808bb90deb8f77b028eafae3a08e10
'http://deb.debian.org/debian/pool/main/l/less/less_590-1.2.debian.tar.xz' less_590-1.2.debian.tar.xz 20456 SHA256:f4873578bec704987a6f22704453e2d8914c39fbc1d908853f074f5530f4aa3e
```

Other potentially useful URLs:

- https://sources.debian.net/src/less/590-1.2/ (for browsing the source)
- https://sources.debian.net/src/less/590-1.2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/less/590-1.2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `libbsd=0.11.7-2`

Binary Packages:

- `libbsd0:amd64=0.11.7-2`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
- `BSD-3-clause-Regents`
- `BSD-3-clause-author`
- `BSD-4-clause-Niels-Provos`
- `Beerware`
- `Expat`
- `ISC`
- `ISC-Original`
- `libutil-David-Nugent`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.11.7-2
'http://http.debian.net/debian/pool/main/libb/libbsd/libbsd_0.11.7-2.dsc' libbsd_0.11.7-2.dsc 2330 SHA256:21c62d65fa3b914d765b733fb0e03d331db830df45f1a5225f95902567f05146
'http://http.debian.net/debian/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz' libbsd_0.11.7.orig.tar.xz 418508 SHA256:9baa186059ebbf25c06308e9f991fda31f7183c0f24931826d83aa6abd8a0261
'http://http.debian.net/debian/pool/main/libb/libbsd/libbsd_0.11.7.orig.tar.xz.asc' libbsd_0.11.7.orig.tar.xz.asc 833 SHA256:b470d3fa5ad6948de7a85891e652970828f26eb7057028d57b94fa8644af934a
'http://http.debian.net/debian/pool/main/libb/libbsd/libbsd_0.11.7-2.debian.tar.xz' libbsd_0.11.7-2.debian.tar.xz 18116 SHA256:e588e52a99415226767362637071764ebfaf454450bda64d53652e7a451d3e67
```

### `dpkg` source package: `libcap-ng=0.8.3-1`

Binary Packages:

- `libcap-ng0:amd64=0.8.3-1+b3`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.8.3-1
'http://http.debian.net/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1.dsc' libcap-ng_0.8.3-1.dsc 1634 SHA256:1bf38dbc0c30bcbc776d2d5c25e31d89202de0858f9ca9379c993d55103d7ef0
'http://http.debian.net/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3.orig.tar.gz' libcap-ng_0.8.3.orig.tar.gz 455383 SHA256:bed6f6848e22bb2f83b5f764b2aef0ed393054e803a8e3a8711cb2a39e6b492d
'http://http.debian.net/debian/pool/main/libc/libcap-ng/libcap-ng_0.8.3-1.debian.tar.xz' libcap-ng_0.8.3-1.debian.tar.xz 10488 SHA256:710577902c260f50f8cfc9d7e264131f880eab0581d12ceab17ebe48e2ac53c6
```

### `dpkg` source package: `libcap2=1:2.66-3`

Binary Packages:

- `libcap2:amd64=1:2.66-3`

Licenses: (parsed from: `/usr/share/doc/libcap2/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libcap2=1:2.66-3
'http://http.debian.net/debian/pool/main/libc/libcap2/libcap2_2.66-3.dsc' libcap2_2.66-3.dsc 2204 SHA256:0fa3650cb450b1d2056cf28b2433683552ddc4f2bceecd834ec050bc65ae762d
'http://http.debian.net/debian/pool/main/libc/libcap2/libcap2_2.66.orig.tar.xz' libcap2_2.66.orig.tar.xz 181592 SHA256:15c40ededb3003d70a283fe587a36b7d19c8b3b554e33f86129c059a4bb466b2
'http://http.debian.net/debian/pool/main/libc/libcap2/libcap2_2.66-3.debian.tar.xz' libcap2_2.66-3.debian.tar.xz 20196 SHA256:d300a825188f7253021c26dbdaec24b4c7bff3e8717286a1af1f3292601d3069
```

### `dpkg` source package: `libdatrie=0.2.13-2`

Binary Packages:

- `libdatrie1:amd64=0.2.13-2+b1`

Licenses: (parsed from: `/usr/share/doc/libdatrie1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris libdatrie=0.2.13-2
'http://http.debian.net/debian/pool/main/libd/libdatrie/libdatrie_0.2.13-2.dsc' libdatrie_0.2.13-2.dsc 2239 SHA256:d359689deccfa654ab844d6e955fff5e826d9a5dc9a74408d1b6a095f78ab0e5
'http://http.debian.net/debian/pool/main/libd/libdatrie/libdatrie_0.2.13.orig.tar.xz' libdatrie_0.2.13.orig.tar.xz 314072 SHA256:12231bb2be2581a7f0fb9904092d24b0ed2a271a16835071ed97bed65267f4be
'http://http.debian.net/debian/pool/main/libd/libdatrie/libdatrie_0.2.13-2.debian.tar.xz' libdatrie_0.2.13-2.debian.tar.xz 9604 SHA256:3f341eb067c5365345e0a416a3c835a8e785c3220aca27c8fb2a01499d0214e9
```

### `dpkg` source package: `libdeflate=1.14-1`

Binary Packages:

- `libdeflate0:amd64=1.14-1`

Licenses: (parsed from: `/usr/share/doc/libdeflate0/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libdeflate=1.14-1
'http://http.debian.net/debian/pool/main/libd/libdeflate/libdeflate_1.14-1.dsc' libdeflate_1.14-1.dsc 2214 SHA256:1f82791c5ac5623ed110e09cc991471deebfe4c419414392d1242e122c6f4c19
'http://http.debian.net/debian/pool/main/libd/libdeflate/libdeflate_1.14.orig.tar.gz' libdeflate_1.14.orig.tar.gz 180182 SHA256:89e7df898c37c3427b0f39aadcf733731321a278771d20fc553f92da8d4808ac
'http://http.debian.net/debian/pool/main/libd/libdeflate/libdeflate_1.14-1.debian.tar.xz' libdeflate_1.14-1.debian.tar.xz 4784 SHA256:4794c379cc4e77eaeb283620bd80a7ce57b858af508f80ba6d5efbc4bcb10434
```

### `dpkg` source package: `libffi=3.4.4-1`

Binary Packages:

- `libffi8:amd64=3.4.4-1`

Licenses: (parsed from: `/usr/share/doc/libffi8/copyright`)

- `Expat`
- `GPL`
- `GPL-2+`
- `GPL-3+`
- `LGPL-2.1+`
- `MPL-1.1`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.4.4-1
'http://http.debian.net/debian/pool/main/libf/libffi/libffi_3.4.4-1.dsc' libffi_3.4.4-1.dsc 1951 SHA256:21c9ef156b6766535cb014e0765142c8104ffbcd73f003ecfa80cfb314baa4f0
'http://http.debian.net/debian/pool/main/libf/libffi/libffi_3.4.4.orig.tar.gz' libffi_3.4.4.orig.tar.gz 1362394 SHA256:d66c56ad259a82cf2a9dfc408b32bf5da52371500b84745f7fb8b645712df676
'http://http.debian.net/debian/pool/main/libf/libffi/libffi_3.4.4-1.debian.tar.xz' libffi_3.4.4-1.debian.tar.xz 10380 SHA256:161b210bfd2ada0b15b0d2a2a98ffc779cd4a68661a7fdf46f61732493db0895
```

### `dpkg` source package: `libgcrypt20=1.10.1-3`

Binary Packages:

- `libgcrypt20:amd64=1.10.1-3`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.10.1-3
'http://http.debian.net/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-3.dsc' libgcrypt20_1.10.1-3.dsc 2790 SHA256:0f1754a411c7b5147ff6c335016f27e3c1743a816053642935ffb75a563a0928
'http://http.debian.net/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2' libgcrypt20_1.10.1.orig.tar.bz2 3778457 SHA256:ef14ae546b0084cd84259f61a55e07a38c3b53afc0f546bffcef2f01baffe9de
'http://http.debian.net/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1.orig.tar.bz2.asc' libgcrypt20_1.10.1.orig.tar.bz2.asc 228 SHA256:9da6ae5e8b1c253607be7e951b568932740c143ee519f6b3392ece8211e84e33
'http://http.debian.net/debian/pool/main/libg/libgcrypt20/libgcrypt20_1.10.1-3.debian.tar.xz' libgcrypt20_1.10.1-3.debian.tar.xz 40560 SHA256:20e11c2ab8ef3878d3e95be6027e6abadbbf49100f313db69acff2548ab6955b
```

### `dpkg` source package: `libgpg-error=1.46-1`

Binary Packages:

- `libgpg-error0:amd64=1.46-1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.46-1
'http://http.debian.net/debian/pool/main/libg/libgpg-error/libgpg-error_1.46-1.dsc' libgpg-error_1.46-1.dsc 2273 SHA256:f1fe4ca2f252f797c2819b0eae1e284e2f0b2c7ac8ec16209054ae45878aaafe
'http://http.debian.net/debian/pool/main/libg/libgpg-error/libgpg-error_1.46.orig.tar.bz2' libgpg-error_1.46.orig.tar.bz2 1014291 SHA256:b7e11a64246bbe5ef37748de43b245abd72cfcd53c9ae5e7fc5ca59f1c81268d
'http://http.debian.net/debian/pool/main/libg/libgpg-error/libgpg-error_1.46.orig.tar.bz2.asc' libgpg-error_1.46.orig.tar.bz2.asc 228 SHA256:e0eb40e705068858ee43b6462b204aacf5a554fe4a17cfe63ea99e9612f72e9d
'http://http.debian.net/debian/pool/main/libg/libgpg-error/libgpg-error_1.46-1.debian.tar.xz' libgpg-error_1.46-1.debian.tar.xz 18532 SHA256:2f80416e16dead749fb6a31a0a3703ae9e562bd32fc4d72184636a1501cd86ef
```

### `dpkg` source package: `libice=2:1.0.10-1`

Binary Packages:

- `libice6:amd64=2:1.0.10-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libice=2:1.0.10-1
'http://http.debian.net/debian/pool/main/libi/libice/libice_1.0.10-1.dsc' libice_1.0.10-1.dsc 2049 SHA256:adb7b4e250db838a476a44b5a941c8f935ac2b20858186f09228cd3e0696034d
'http://http.debian.net/debian/pool/main/libi/libice/libice_1.0.10.orig.tar.gz' libice_1.0.10.orig.tar.gz 481960 SHA256:1116bc64c772fd127a0d0c0ffa2833479905e3d3d8197740b3abd5f292f22d2d
'http://http.debian.net/debian/pool/main/libi/libice/libice_1.0.10-1.diff.gz' libice_1.0.10-1.diff.gz 11349 SHA256:d186b3877416a7e80f1923fe2fc736d576e585a41450bcf4cd5e74f9dd099362
```

### `dpkg` source package: `libidn2=2.3.3-1`

Binary Packages:

- `libidn2-0:amd64=2.3.3-1+b1`

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
$ apt-get source -qq --print-uris libidn2=2.3.3-1
'http://http.debian.net/debian/pool/main/libi/libidn2/libidn2_2.3.3-1.dsc' libidn2_2.3.3-1.dsc 2206 SHA256:13865e96a0fed8dcb82767db65c946b56ed44fc1806d80d407c512ded2a83984
'http://http.debian.net/debian/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz' libidn2_2.3.3.orig.tar.gz 2116946 SHA256:f3ac987522c00d33d44b323cae424e2cffcb4c63c6aa6cd1376edacbf1c36eb0
'http://http.debian.net/debian/pool/main/libi/libidn2/libidn2_2.3.3.orig.tar.gz.asc' libidn2_2.3.3.orig.tar.gz.asc 228 SHA256:e8f2bdce5def6c239c2cc3220e808b19b14d3f7eb3a0e14851dd5c16fc9ad0ec
'http://http.debian.net/debian/pool/main/libi/libidn2/libidn2_2.3.3-1.debian.tar.xz' libidn2_2.3.3-1.debian.tar.xz 15964 SHA256:b040c12276e1128394c2f84c97f7e45f340867fa9d0d0a0b9d8f043b1977db99
```

### `dpkg` source package: `libjpeg-turbo=1:2.1.5-2`

Binary Packages:

- `libjpeg-dev:amd64=1:2.1.5-2`
- `libjpeg62-turbo:amd64=1:2.1.5-2`
- `libjpeg62-turbo-dev:amd64=1:2.1.5-2`

Licenses: (parsed from: `/usr/share/doc/libjpeg-dev/copyright`, `/usr/share/doc/libjpeg62-turbo/copyright`, `/usr/share/doc/libjpeg62-turbo-dev/copyright`)

- `BSD-3-clause`
- `BSD-BY-LC-NE`
- `Expat`
- `NTP`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris libjpeg-turbo=1:2.1.5-2
'http://http.debian.net/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5-2.dsc' libjpeg-turbo_2.1.5-2.dsc 2493 SHA256:d718ead0dfbcbc8523665c02a7f7152e31039ded641d022868722623bb3b486d
'http://http.debian.net/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5.orig.tar.gz' libjpeg-turbo_2.1.5.orig.tar.gz 2264471 SHA256:254f3642b04e309fee775123133c6464181addc150499561020312ec61c1bf7c
'http://http.debian.net/debian/pool/main/libj/libjpeg-turbo/libjpeg-turbo_2.1.5-2.debian.tar.xz' libjpeg-turbo_2.1.5-2.debian.tar.xz 107768 SHA256:cdb2433c2f7101345c1ffa14efb943787c675b86354691a32490845fe4bc9237
```

### `dpkg` source package: `libmd=1.0.4-2`

Binary Packages:

- `libmd0:amd64=1.0.4-2`

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
$ apt-get source -qq --print-uris libmd=1.0.4-2
'http://http.debian.net/debian/pool/main/libm/libmd/libmd_1.0.4-2.dsc' libmd_1.0.4-2.dsc 2264 SHA256:5e060cb277f31e67b91033e05ece00832ca8056decba873b1698a5680414a177
'http://http.debian.net/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz' libmd_1.0.4.orig.tar.xz 264472 SHA256:f51c921042e34beddeded4b75557656559cf5b1f2448033b4c1eec11c07e530f
'http://http.debian.net/debian/pool/main/libm/libmd/libmd_1.0.4.orig.tar.xz.asc' libmd_1.0.4.orig.tar.xz.asc 833 SHA256:32deebe1cfab127ee69a3e8c8caf439e459b7cdcdd7535fe021cb485adc14057
'http://http.debian.net/debian/pool/main/libm/libmd/libmd_1.0.4-2.debian.tar.xz' libmd_1.0.4-2.debian.tar.xz 10204 SHA256:a27a2221b1a81e192455e2e93da2e313b21e489f6ac2bcf84b0b813dc3fe261b
```

### `dpkg` source package: `libnsl=1.3.0-2`

Binary Packages:

- `libnsl-dev:amd64=1.3.0-2`
- `libnsl2:amd64=1.3.0-2`

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
$ apt-get source -qq --print-uris libnsl=1.3.0-2
'http://http.debian.net/debian/pool/main/libn/libnsl/libnsl_1.3.0-2.dsc' libnsl_1.3.0-2.dsc 1955 SHA256:1da570eed6693c774cce51f3c33f989d1aa4bf1dcb8660818d8a834a1a3728ef
'http://http.debian.net/debian/pool/main/libn/libnsl/libnsl_1.3.0.orig.tar.xz' libnsl_1.3.0.orig.tar.xz 321488 SHA256:eac3062957fa302c62eff4aed718a07bacbf9ceb0a058289f12a19bfdda3c8e2
'http://http.debian.net/debian/pool/main/libn/libnsl/libnsl_1.3.0-2.debian.tar.xz' libnsl_1.3.0-2.debian.tar.xz 4692 SHA256:7f8dccc706931b9e206448ffb475487a4a0abaded27cf611d418f4a34415dca7
```

### `dpkg` source package: `libpaper=1.1.29`

Binary Packages:

- `libpaper-utils=1.1.29`
- `libpaper1:amd64=1.1.29`

Licenses: (parsed from: `/usr/share/doc/libpaper-utils/copyright`, `/usr/share/doc/libpaper1/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libpaper=1.1.29
'http://http.debian.net/debian/pool/main/libp/libpaper/libpaper_1.1.29.dsc' libpaper_1.1.29.dsc 1604 SHA256:940adde11d3bd19c3be7e3e16cdd737ca8fa52fac31e002d2530beea3e64cfc9
'http://http.debian.net/debian/pool/main/libp/libpaper/libpaper_1.1.29.tar.gz' libpaper_1.1.29.tar.gz 44942 SHA256:26330e21e9a3124658d515fd850b0cde546ff42d89b2596a5264c5f1677f0547
```

### `dpkg` source package: `libpng1.6=1.6.39-2`

Binary Packages:

- `libpng-dev:amd64=1.6.39-2`
- `libpng16-16:amd64=1.6.39-2`

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
$ apt-get source -qq --print-uris libpng1.6=1.6.39-2
'http://http.debian.net/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.39-2.dsc' libpng1.6_1.6.39-2.dsc 2241 SHA256:c5fcfb43b423028e7f3c00ea398caddec361bf796ff1cbc18dd565b97fb1a3fe
'http://http.debian.net/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.39.orig.tar.gz' libpng1.6_1.6.39.orig.tar.gz 1519415 SHA256:a00e9d2f2f664186e4202db9299397f851aea71b36a35e74910b8820e380d441
'http://http.debian.net/debian/pool/main/libp/libpng1.6/libpng1.6_1.6.39-2.debian.tar.xz' libpng1.6_1.6.39-2.debian.tar.xz 31076 SHA256:c3a73a6143e18c9a62b32d6db80acbc525f03c795bca41079087d89febff0217
```

### `dpkg` source package: `libpsl=0.21.2-1`

Binary Packages:

- `libpsl5:amd64=0.21.2-1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`
- `gnulib`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.2-1
'http://http.debian.net/debian/pool/main/libp/libpsl/libpsl_0.21.2-1.dsc' libpsl_0.21.2-1.dsc 1622 SHA256:1ddb578f5865a447b11078993cef2138107c82f8590ec2516af6f9970a2d4e0f
'http://http.debian.net/debian/pool/main/libp/libpsl/libpsl_0.21.2.orig.tar.xz' libpsl_0.21.2.orig.tar.xz 1870352 SHA256:11e34380f2c81d6e72c710464aae3b680df4ddcc1007826c630fb03c7ca6aa54
'http://http.debian.net/debian/pool/main/libp/libpsl/libpsl_0.21.2-1.debian.tar.xz' libpsl_0.21.2-1.debian.tar.xz 11940 SHA256:78327367c83ce2dc6a8404f479a7589eacb0266f1d4a25619d5f6f00f98ab7b6
```

### `dpkg` source package: `libseccomp=2.5.4-1`

Binary Packages:

- `libseccomp2:amd64=2.5.4-1+b3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.5.4-1
'http://http.debian.net/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-1.dsc' libseccomp_2.5.4-1.dsc 2676 SHA256:2986473126cb5f3e358fed40ec1482816e1068dbdfe938bf9f80c50afcf32b80
'http://http.debian.net/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz' libseccomp_2.5.4.orig.tar.gz 637228 SHA256:d82902400405cf0068574ef3dc1fe5f5926207543ba1ae6f8e7a1576351dcbdb
'http://http.debian.net/debian/pool/main/libs/libseccomp/libseccomp_2.5.4.orig.tar.gz.asc' libseccomp_2.5.4.orig.tar.gz.asc 833 SHA256:af37e70eb422e6f983c1f135a3abb342c3b787716520b71bd774e4906003807f
'http://http.debian.net/debian/pool/main/libs/libseccomp/libseccomp_2.5.4-1.debian.tar.xz' libseccomp_2.5.4-1.debian.tar.xz 16264 SHA256:fd7abe7b26a08ca514457fd13302d348d59401616ce3f6809ce15f54e6ebe77d
```

### `dpkg` source package: `libselinux=3.4-1`

Binary Packages:

- `libselinux1:amd64=3.4-1+b5`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.4-1
'http://http.debian.net/debian/pool/main/libs/libselinux/libselinux_3.4-1.dsc' libselinux_3.4-1.dsc 2534 SHA256:4035af53388d343f9b5c46ca2867ba32823cf4a2d218ddd590b34ae59c899157
'http://http.debian.net/debian/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz' libselinux_3.4.orig.tar.gz 210061 SHA256:77c294a927e6795c2e98f74b5c3adde9c8839690e9255b767c5fca6acff9b779
'http://http.debian.net/debian/pool/main/libs/libselinux/libselinux_3.4.orig.tar.gz.asc' libselinux_3.4.orig.tar.gz.asc 833 SHA256:5c370bdef7b756697445e6838ba1b2d934f668b244461e36e245f589ec994a24
'http://http.debian.net/debian/pool/main/libs/libselinux/libselinux_3.4-1.debian.tar.xz' libselinux_3.4-1.debian.tar.xz 29416 SHA256:046ace4ad0092104bdfb0c6e5187131910216c89b8b81a4bce3c2067615c9196
```

### `dpkg` source package: `libsemanage=3.4-1`

Binary Packages:

- `libsemanage-common=3.4-1`
- `libsemanage2:amd64=3.4-1+b5`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.4-1
'http://http.debian.net/debian/pool/main/libs/libsemanage/libsemanage_3.4-1.dsc' libsemanage_3.4-1.dsc 2570 SHA256:be300e01bbd08706fb6f0ecd349b3585a535d9ff0957265a7c634545ac3515c8
'http://http.debian.net/debian/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz' libsemanage_3.4.orig.tar.gz 185177 SHA256:93b423a21600b8e3fb59bb925d4583d1258f45bebf63c29bde304dfd3d52efd6
'http://http.debian.net/debian/pool/main/libs/libsemanage/libsemanage_3.4.orig.tar.gz.asc' libsemanage_3.4.orig.tar.gz.asc 833 SHA256:58da87dd662c135b70c065a0b1ca800cd4b075b365f3d71e0ff02d71c7457883
'http://http.debian.net/debian/pool/main/libs/libsemanage/libsemanage_3.4-1.debian.tar.xz' libsemanage_3.4-1.debian.tar.xz 23248 SHA256:531c5294d5ec881ef4bc4396a9e1f38895558cd88c4fd6d3f6a673a4b2297a5c
```

### `dpkg` source package: `libsepol=3.4-2`

Binary Packages:

- `libsepol2:amd64=3.4-2`

Licenses: (parsed from: `/usr/share/doc/libsepol2/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.4-2
'http://http.debian.net/debian/pool/main/libs/libsepol/libsepol_3.4-2.dsc' libsepol_3.4-2.dsc 2005 SHA256:c43db54870c37a4b6441b1980bfd41932e7851244ba1fda0df86c5f17dd67e8a
'http://http.debian.net/debian/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz' libsepol_3.4.orig.tar.gz 490628 SHA256:fc277ac5b52d59d2cd81eec8b1cccd450301d8b54d9dd48a993aea0577cf0336
'http://http.debian.net/debian/pool/main/libs/libsepol/libsepol_3.4.orig.tar.gz.asc' libsepol_3.4.orig.tar.gz.asc 833 SHA256:ed127c08353dbc2c442d47d77e323e79e5bd47791a0a5bd4dfd077868f4346bc
'http://http.debian.net/debian/pool/main/libs/libsepol/libsepol_3.4-2.debian.tar.xz' libsepol_3.4-2.debian.tar.xz 21516 SHA256:fdf943b513b8d0fc6b74fd6a007ba35c9601909c0b3fd6e7726b4b09b1243502
```

### `dpkg` source package: `libsm=2:1.2.3-1`

Binary Packages:

- `libsm6:amd64=2:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libsm=2:1.2.3-1
'http://http.debian.net/debian/pool/main/libs/libsm/libsm_1.2.3-1.dsc' libsm_1.2.3-1.dsc 2063 SHA256:5488f8de81d53c32cbb5f062b6a6f262cd067283b8082041392dc60f0d04002c
'http://http.debian.net/debian/pool/main/libs/libsm/libsm_1.2.3.orig.tar.gz' libsm_1.2.3.orig.tar.gz 445362 SHA256:1e92408417cb6c6c477a8a6104291001a40b3bb56a4a60608fdd9cd2c5a0f320
'http://http.debian.net/debian/pool/main/libs/libsm/libsm_1.2.3-1.diff.gz' libsm_1.2.3-1.diff.gz 8929 SHA256:7eb99ab50b19f26d1470f89e4b46891f6a697cb1794a58ed0d1376cceaf1b6a9
```

### `dpkg` source package: `libssh2=1.10.0-3`

Binary Packages:

- `libssh2-1:amd64=1.10.0-3+b1`

Licenses: (parsed from: `/usr/share/doc/libssh2-1/copyright`)

- `BSD3`

Source:

```console
$ apt-get source -qq --print-uris libssh2=1.10.0-3
'http://http.debian.net/debian/pool/main/libs/libssh2/libssh2_1.10.0-3.dsc' libssh2_1.10.0-3.dsc 2283 SHA256:a0fe68f402a2f44dd6bd2219457fb8677b2149a83e7b009e93ff0635de940766
'http://http.debian.net/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz' libssh2_1.10.0.orig.tar.gz 965044 SHA256:2d64e90f3ded394b91d3a2e774ca203a4179f69aebee03003e5a6fa621e41d51
'http://http.debian.net/debian/pool/main/libs/libssh2/libssh2_1.10.0.orig.tar.gz.asc' libssh2_1.10.0.orig.tar.gz.asc 488 SHA256:75702eaf490fa8c1e69b889c5c6366c2c3f3b089bc715f9f9be081c88f115f81
'http://http.debian.net/debian/pool/main/libs/libssh2/libssh2_1.10.0-3.debian.tar.xz' libssh2_1.10.0-3.debian.tar.xz 8416 SHA256:c0bea31fe565273656349484d1000b557e489ee322834b40c4d7d33317a56940
```

### `dpkg` source package: `libtasn1-6=4.19.0-2`

Binary Packages:

- `libtasn1-6:amd64=4.19.0-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.19.0-2
'http://http.debian.net/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-2.dsc' libtasn1-6_4.19.0-2.dsc 2662 SHA256:cbecbd9b784af6dedde9ca685a4cc13e1ead027ea051150ff8186af57c547109
'http://http.debian.net/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz' libtasn1-6_4.19.0.orig.tar.gz 1786576 SHA256:1613f0ac1cf484d6ec0ce3b8c06d56263cc7242f1c23b30d82d23de345a63f7a
'http://http.debian.net/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0.orig.tar.gz.asc' libtasn1-6_4.19.0.orig.tar.gz.asc 228 SHA256:8410c0c004f3509c218a98b276b3308b9c46f48068e8b1a6d9ebfd61ea9f357a
'http://http.debian.net/debian/pool/main/libt/libtasn1-6/libtasn1-6_4.19.0-2.debian.tar.xz' libtasn1-6_4.19.0-2.debian.tar.xz 22012 SHA256:21fe6b16fb27cca47b51893708964ddfe04ea5227d1608560b4988e6fca74ae9
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
'http://http.debian.net/debian/pool/main/libt/libthai/libthai_0.1.29-1.dsc' libthai_0.1.29-1.dsc 2325 SHA256:470b853bcb84ce88c63720da51ee5b0001fd1ebec8f8679a986b155d0be1ff06
'http://http.debian.net/debian/pool/main/libt/libthai/libthai_0.1.29.orig.tar.xz' libthai_0.1.29.orig.tar.xz 417728 SHA256:fc80cc7dcb50e11302b417cebd24f2d30a8b987292e77e003267b9100d0f4bcd
'http://http.debian.net/debian/pool/main/libt/libthai/libthai_0.1.29-1.debian.tar.xz' libthai_0.1.29-1.debian.tar.xz 12564 SHA256:5c86bd1c2af7972e29cead559823c8f85b9dd9363efad0d90ab7ad86e35840ef
```

### `dpkg` source package: `libtirpc=1.3.3+ds-1`

Binary Packages:

- `libtirpc-common=1.3.3+ds-1`
- `libtirpc-dev:amd64=1.3.3+ds-1`
- `libtirpc3:amd64=1.3.3+ds-1`

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
$ apt-get source -qq --print-uris libtirpc=1.3.3+ds-1
'http://http.debian.net/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.dsc' libtirpc_1.3.3+ds-1.dsc 2129 SHA256:c05c5d76027d4162d5a29d73eef90076559bde0fa5133b2e0045d82155e1b2af
'http://http.debian.net/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds.orig.tar.gz' libtirpc_1.3.3+ds.orig.tar.gz 699030 SHA256:facd98473c3a16fe6564c6458ef96ebb84d144345d1171f034fa019424bba027
'http://http.debian.net/debian/pool/main/libt/libtirpc/libtirpc_1.3.3%2bds-1.debian.tar.xz' libtirpc_1.3.3+ds-1.debian.tar.xz 11232 SHA256:fd1865c49e905951a641082981c1dab7f018caea1a5e23af1791728a3320800e
```

### `dpkg` source package: `libunistring=1.0-2`

Binary Packages:

- `libunistring2:amd64=1.0-2`

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
$ apt-get source -qq --print-uris libunistring=1.0-2
'http://http.debian.net/debian/pool/main/libu/libunistring/libunistring_1.0-2.dsc' libunistring_1.0-2.dsc 2181 SHA256:9b9a9d9d4cd1c2118df8cf5ca0dfb787d89afcd99400d7cd01b4c4e9b0bc1ae5
'http://http.debian.net/debian/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz' libunistring_1.0.orig.tar.xz 2367800 SHA256:5bab55b49f75d77ed26b257997e919b693f29fd4a1bc22e0e6e024c246c72741
'http://http.debian.net/debian/pool/main/libu/libunistring/libunistring_1.0.orig.tar.xz.asc' libunistring_1.0.orig.tar.xz.asc 833 SHA256:c1c2ae60eb971593da92e65384a5f1b181717e7b9654854f139f350c6cbe235d
'http://http.debian.net/debian/pool/main/libu/libunistring/libunistring_1.0-2.debian.tar.xz' libunistring_1.0-2.debian.tar.xz 14520 SHA256:e550d94935cd06eafb0defd7b5d7c914c7bb80a8e818a49efcf7675206572450
```

### `dpkg` source package: `libwebp=1.2.4-0.1`

Binary Packages:

- `libwebp7:amd64=1.2.4-0.1`

Licenses: (parsed from: `/usr/share/doc/libwebp7/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris libwebp=1.2.4-0.1
'http://http.debian.net/debian/pool/main/libw/libwebp/libwebp_1.2.4-0.1.dsc' libwebp_1.2.4-0.1.dsc 2401 SHA256:78443a7e59704d1c60e862b6482cff5c50ca5f47adc5d94638cd740d86782353
'http://http.debian.net/debian/pool/main/libw/libwebp/libwebp_1.2.4.orig.tar.gz' libwebp_1.2.4.orig.tar.gz 4141376 SHA256:7bf5a8a28cc69bcfa8cb214f2c3095703c6b73ac5fba4d5480c205331d9494df
'http://http.debian.net/debian/pool/main/libw/libwebp/libwebp_1.2.4.orig.tar.gz.asc' libwebp_1.2.4.orig.tar.gz.asc 833 SHA256:4c546cf7f757a70d8803ab850e69d28e7ce06e66dbee003fd3ede7346543851a
'http://http.debian.net/debian/pool/main/libw/libwebp/libwebp_1.2.4-0.1.debian.tar.xz' libwebp_1.2.4-0.1.debian.tar.xz 7156 SHA256:af583ae1943db329440623ccf1e7aeb11a477cae24a306985c6c0c5e60ce41ae
```

### `dpkg` source package: `libx11=2:1.8.4-2`

Binary Packages:

- `libx11-6:amd64=2:1.8.4-2`
- `libx11-data=2:1.8.4-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.8.4-2
'http://http.debian.net/debian/pool/main/libx/libx11/libx11_1.8.4-2.dsc' libx11_1.8.4-2.dsc 2483 SHA256:efd2c1f9c8dfa14e188a1c4b6354ba5504c859a8dcd0868a867338089a6c5551
'http://http.debian.net/debian/pool/main/libx/libx11/libx11_1.8.4.orig.tar.gz' libx11_1.8.4.orig.tar.gz 3168573 SHA256:efd3a3a43c1f177edc2c205bedb0719b6648203595e54c0b83a32576aeaca7cd
'http://http.debian.net/debian/pool/main/libx/libx11/libx11_1.8.4.orig.tar.gz.asc' libx11_1.8.4.orig.tar.gz.asc 801 SHA256:9d9a6bcdd81a40ed377b2981a4d40a0db1315d095e9ccc35a0ba78e692df8591
'http://http.debian.net/debian/pool/main/libx/libx11/libx11_1.8.4-2.diff.gz' libx11_1.8.4-2.diff.gz 110943 SHA256:eb3816b3256b0a30f5f3ec7a1837ee60e984e8ce10e4ba53f0e4f0693e5c8bf0
```

### `dpkg` source package: `libxau=1:1.0.9-1`

Binary Packages:

- `libxau6:amd64=1:1.0.9-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-1
'http://http.debian.net/debian/pool/main/libx/libxau/libxau_1.0.9-1.dsc' libxau_1.0.9-1.dsc 2183 SHA256:e6e059652cda7e5a49b6c9a70667639f32d629c20320487d16c642a06c1ebf85
'http://http.debian.net/debian/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA256:1f123d8304b082ad63a9e89376400a3b1d4c29e67e3ea07b3f659cccca690eea
'http://http.debian.net/debian/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz.asc' libxau_1.0.9.orig.tar.gz.asc 801 SHA256:af6104aaf3c5ede529e381237dd60f49640ec96593a84502fa493b86582b2f04
'http://http.debian.net/debian/pool/main/libx/libxau/libxau_1.0.9-1.diff.gz' libxau_1.0.9-1.diff.gz 10193 SHA256:7b34899563f172e8f11d061de41b58fe1c32f8683d985e57686677ccb7299a9a
```

### `dpkg` source package: `libxcb=1.15-1`

Binary Packages:

- `libxcb-render0:amd64=1.15-1`
- `libxcb-shm0:amd64=1.15-1`
- `libxcb1:amd64=1.15-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.15-1
'http://http.debian.net/debian/pool/main/libx/libxcb/libxcb_1.15-1.dsc' libxcb_1.15-1.dsc 5344 SHA256:f689569f33e70ca4c95c91b094d0659eb49a958d9ac43186640338f9290e298b
'http://http.debian.net/debian/pool/main/libx/libxcb/libxcb_1.15.orig.tar.gz' libxcb_1.15.orig.tar.gz 650774 SHA256:1cb65df8543a69ec0555ac696123ee386321dfac1964a3da39976c9a05ad724d
'http://http.debian.net/debian/pool/main/libx/libxcb/libxcb_1.15-1.diff.gz' libxcb_1.15-1.diff.gz 26267 SHA256:639c719ed06ffc397b200a209abd1a049e21e9e19431fb14c9ca870de01a6eac
```

### `dpkg` source package: `libxcrypt=1:4.4.33-2`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.33-2`
- `libcrypt1:amd64=1:4.4.33-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.33-2
'http://http.debian.net/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.33-2.dsc' libxcrypt_4.4.33-2.dsc 1591 SHA256:910ae411c9462f07667e46540af3dbb30f46413ddd90f1f176781666042dbb38
'http://http.debian.net/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.33.orig.tar.xz' libxcrypt_4.4.33.orig.tar.xz 393372 SHA256:5e2da5cb5f263e9ac4c4b3f49c75e3b8523889210f45c60bb7e97b229c75a10b
'http://http.debian.net/debian/pool/main/libx/libxcrypt/libxcrypt_4.4.33-2.debian.tar.xz' libxcrypt_4.4.33-2.debian.tar.xz 8196 SHA256:23194c9b0642533fb27fe8c33391d3fa838a55e17e5a88a419ed31548b0721c9
```

### `dpkg` source package: `libxdmcp=1:1.1.2-3`

Binary Packages:

- `libxdmcp6:amd64=1:1.1.2-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.2-3
'http://http.debian.net/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.dsc' libxdmcp_1.1.2-3.dsc 2145 SHA256:f9697dca6a275aeee9a3eee9fb2d55e0f77485481e8b84efc6950fc9b1988460
'http://http.debian.net/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2.orig.tar.gz' libxdmcp_1.1.2.orig.tar.gz 404115 SHA256:6f7c7e491a23035a26284d247779174dedc67e34e93cc3548b648ffdb6fc57c0
'http://http.debian.net/debian/pool/main/libx/libxdmcp/libxdmcp_1.1.2-3.diff.gz' libxdmcp_1.1.2-3.diff.gz 18017 SHA256:5844df115c17e5ba40ac116f80373304d821c607e763ef6f40562421f5cc0cf3
```

### `dpkg` source package: `libxext=2:1.3.4-1`

Binary Packages:

- `libxext6:amd64=2:1.3.4-1+b1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-1
'http://http.debian.net/debian/pool/main/libx/libxext/libxext_1.3.4-1.dsc' libxext_1.3.4-1.dsc 2118 SHA256:25024f57d955739c6b858822bf93ec3c71400b56fc0d666826f440e3661fd7c0
'http://http.debian.net/debian/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA256:8ef0789f282826661ff40a8eef22430378516ac580167da35cc948be9041aac1
'http://http.debian.net/debian/pool/main/libx/libxext/libxext_1.3.4-1.diff.gz' libxext_1.3.4-1.diff.gz 12509 SHA256:b975870d6a7b791ffbe2d57efdf6e20c250c5e76d12e45b04c8655f593bb8337
```

### `dpkg` source package: `libxmu=2:1.1.3-3`

Binary Packages:

- `libxmuu1:amd64=2:1.1.3-3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxmu=2:1.1.3-3
'http://http.debian.net/debian/pool/main/libx/libxmu/libxmu_1.1.3-3.dsc' libxmu_1.1.3-3.dsc 2165 SHA256:d9dfadd0a6be92f88b1151c695e5799f889a39047176f80a91fcba24333cd063
'http://http.debian.net/debian/pool/main/libx/libxmu/libxmu_1.1.3.orig.tar.gz' libxmu_1.1.3.orig.tar.gz 497343 SHA256:5bd9d4ed1ceaac9ea023d86bf1c1632cd3b172dce4a193a72a94e1d9df87a62e
'http://http.debian.net/debian/pool/main/libx/libxmu/libxmu_1.1.3-3.diff.gz' libxmu_1.1.3-3.diff.gz 8085 SHA256:6f599ddd7951a1db5c1899fcd2a7c0289ae4ec9f9a783bc5e5b209b83c7ea12d
```

### `dpkg` source package: `libxrender=1:0.9.10-1.1`

Binary Packages:

- `libxrender1:amd64=1:0.9.10-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxrender=1:0.9.10-1.1
'http://http.debian.net/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.1.dsc' libxrender_0.9.10-1.1.dsc 2072 SHA256:348ab15d05f1d802da485e4c6abdb9d5419691fb7c8ce44ca5b17b2b7f889ce8
'http://http.debian.net/debian/pool/main/libx/libxrender/libxrender_0.9.10.orig.tar.gz' libxrender_0.9.10.orig.tar.gz 373717 SHA256:770527cce42500790433df84ec3521e8bf095dfe5079454a92236494ab296adf
'http://http.debian.net/debian/pool/main/libx/libxrender/libxrender_0.9.10-1.1.diff.gz' libxrender_0.9.10-1.1.diff.gz 15201 SHA256:caf8c84085b3b0d073f738fa12d32d4eca2d8b669cb3c7f1b1cd2ce64b7b10b7
```

### `dpkg` source package: `libxss=1:1.2.3-1`

Binary Packages:

- `libxss1:amd64=1:1.2.3-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxss=1:1.2.3-1
'http://http.debian.net/debian/pool/main/libx/libxss/libxss_1.2.3-1.dsc' libxss_1.2.3-1.dsc 2203 SHA256:783dbcd49a0934d994693af676ee98734dad070ab2434a6afe831c2de0ecca1d
'http://http.debian.net/debian/pool/main/libx/libxss/libxss_1.2.3.orig.tar.gz' libxss_1.2.3.orig.tar.gz 385215 SHA256:4f74e7e412144591d8e0616db27f433cfc9f45aae6669c6c4bb03e6bf9be809a
'http://http.debian.net/debian/pool/main/libx/libxss/libxss_1.2.3.orig.tar.gz.asc' libxss_1.2.3.orig.tar.gz.asc 705 SHA256:4e900524d56c8e7263365267efa91bb3671110c9eb28ccab58f70e2188f0b91b
'http://http.debian.net/debian/pool/main/libx/libxss/libxss_1.2.3-1.diff.gz' libxss_1.2.3-1.diff.gz 7145 SHA256:9d381b48f1377f27c506113e1f9b7d6ee286b856421f7f2b27017f01dccfef04
```

### `dpkg` source package: `libxt=1:1.2.1-1.1`

Binary Packages:

- `libxt6:amd64=1:1.2.1-1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxt=1:1.2.1-1.1
'http://http.debian.net/debian/pool/main/libx/libxt/libxt_1.2.1-1.1.dsc' libxt_1.2.1-1.1.dsc 2170 SHA256:62859ce41aa5914f32715fadb9dc60a54cc1ef3331b2122969ffbe31e5d53be7
'http://http.debian.net/debian/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz' libxt_1.2.1.orig.tar.gz 1024473 SHA256:6da1bfa9dd0ed87430a5ce95b129485086394df308998ebe34d98e378e3dfb33
'http://http.debian.net/debian/pool/main/libx/libxt/libxt_1.2.1.orig.tar.gz.asc' libxt_1.2.1.orig.tar.gz.asc 358 SHA256:da406cc94c25ca6773bb37c2055e2eb5665491f7ca6dfc9ea04f0f30ea3fd098
'http://http.debian.net/debian/pool/main/libx/libxt/libxt_1.2.1-1.1.diff.gz' libxt_1.2.1-1.1.diff.gz 45585 SHA256:ae7993031f3d77fcdbc2540f9d1b6b4a0afafddd747f1de444e4ffe2fa678fca
```

### `dpkg` source package: `libzstd=1.5.4+dfsg2-5`

Binary Packages:

- `libzstd1:amd64=1.5.4+dfsg2-5`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.5.4+dfsg2-5
'http://http.debian.net/debian/pool/main/libz/libzstd/libzstd_1.5.4%2bdfsg2-5.dsc' libzstd_1.5.4+dfsg2-5.dsc 2589 SHA256:8f602f92b575aa8b5e979196fb6ee82d78f233521dc9636526d3ecba1f63c1b1
'http://http.debian.net/debian/pool/main/libz/libzstd/libzstd_1.5.4%2bdfsg2.orig.tar.xz' libzstd_1.5.4+dfsg2.orig.tar.xz 1582660 SHA256:8cf4bbb65e77ec348d052c8d6230eba66d435bddf64c8b5be2fcb16880c19953
'http://http.debian.net/debian/pool/main/libz/libzstd/libzstd_1.5.4%2bdfsg2.orig.tar.xz.asc' libzstd_1.5.4+dfsg2.orig.tar.xz.asc 833 SHA256:be007507630aabfc7d88d5d3c467115935ca22025253491d525e0119bbb23d40
'http://http.debian.net/debian/pool/main/libz/libzstd/libzstd_1.5.4%2bdfsg2-5.debian.tar.xz' libzstd_1.5.4+dfsg2-5.debian.tar.xz 216092 SHA256:82ce911445772861d0838bd4545f93bc50658bc7f3cefdb17a307dfb8ffca5d8
```

### `dpkg` source package: `linux=6.1.20-2`

Binary Packages:

- `linux-libc-dev:amd64=6.1.20-2`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `BSD-2-clause`
- `CRYPTOGAMS`
- `GPL-2`
- `GPL-2+-or-X11`
- `LGPL-2.1`
- `Unicode-data`
- `Xen-interface`

Source:

```console
$ apt-get source -qq --print-uris linux=6.1.20-2
'http://http.debian.net/debian/pool/main/l/linux/linux_6.1.20-2.dsc' linux_6.1.20-2.dsc 276943 SHA256:0770faca88ec9da5711fc0d5abdd150d188c56bf8dd19ae0120aa22f5fe69a3e
'http://http.debian.net/debian/pool/main/l/linux/linux_6.1.20.orig.tar.xz' linux_6.1.20.orig.tar.xz 137291340 SHA256:18dca37b48f4643a62a8bd0adee0888d7b815f75229f90833992b28b6a651427
'http://http.debian.net/debian/pool/main/l/linux/linux_6.1.20-2.debian.tar.xz' linux_6.1.20-2.debian.tar.xz 4585780 SHA256:8fc1b579ed50f458975aa1d65ae3d513e64a8fd207d192ea8767a58e72dd09b6
```

### `dpkg` source package: `littler=0.3.17-1`

Binary Packages:

- `littler=0.3.17-1`
- `r-cran-littler=0.3.17-1`

Licenses: (parsed from: `/usr/share/doc/littler/copyright`, `/usr/share/doc/r-cran-littler/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris littler=0.3.17-1
'http://http.debian.net/debian/pool/main/l/littler/littler_0.3.17-1.dsc' littler_0.3.17-1.dsc 1874 SHA256:498188a08a83118674afc3856d0341714b1aba98f001978a41e076723673f5ce
'http://http.debian.net/debian/pool/main/l/littler/littler_0.3.17.orig.tar.gz' littler_0.3.17.orig.tar.gz 118131 SHA256:4cebe1fe21eb28bea13d1118d611021603e7354b5f77f29854b60002cb2ca554
'http://http.debian.net/debian/pool/main/l/littler/littler_0.3.17-1.debian.tar.xz' littler_0.3.17-1.debian.tar.xz 7000 SHA256:2e23a273ffea5e9d44b7bc08d21c87e3ea8ef311f3494350f273e66c9de459d1
```

### `dpkg` source package: `lz4=1.9.4-1`

Binary Packages:

- `liblz4-1:amd64=1.9.4-1`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.4-1
'http://http.debian.net/debian/pool/main/l/lz4/lz4_1.9.4-1.dsc' lz4_1.9.4-1.dsc 1951 SHA256:e16302bca544d08d106efc216541f4a0403c8f8a5fad5eaac7588223a55af263
'http://http.debian.net/debian/pool/main/l/lz4/lz4_1.9.4.orig.tar.gz' lz4_1.9.4.orig.tar.gz 354063 SHA256:0b0e3aa07c8c063ddf40b082bdf7e37a1562bda40a0ff5272957f3e987e0e54b
'http://http.debian.net/debian/pool/main/l/lz4/lz4_1.9.4-1.debian.tar.xz' lz4_1.9.4-1.debian.tar.xz 8128 SHA256:47ceec5b95f42598f7b9280b03df9659f2ee6852720ec181488e83bd643f0e5f
```

### `dpkg` source package: `make-dfsg=4.3-4.1`

Binary Packages:

- `make=4.3-4.1`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.3-4.1
'http://http.debian.net/debian/pool/main/m/make-dfsg/make-dfsg_4.3-4.1.dsc' make-dfsg_4.3-4.1.dsc 2019 SHA256:d2523d94f4d4198df6801f238d36cf0dea2ab5521f1d19ee76b2e8ee1f1918bb
'http://http.debian.net/debian/pool/main/m/make-dfsg/make-dfsg_4.3.orig.tar.gz' make-dfsg_4.3.orig.tar.gz 1845906 SHA256:be4c17542578824e745f83bcd2a9ba264206187247cb6a5f5df99b0a9d1f9047
'http://http.debian.net/debian/pool/main/m/make-dfsg/make-dfsg_4.3-4.1.diff.gz' make-dfsg_4.3-4.1.diff.gz 50940 SHA256:753c254ecaba425ebe2e0a0fb4d299847701e1c3eeb43df563e39975cae56b4c
```

### `dpkg` source package: `mawk=1.3.4.20200120-3.1`

Binary Packages:

- `mawk=1.3.4.20200120-3.1`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `CC-BY-3.0`
- `GPL-2`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-3.1
'http://http.debian.net/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.dsc' mawk_1.3.4.20200120-3.1.dsc 1776 SHA256:ed0543e3111f718e918a73033292fe2616760c8791c13efa0da3818ca835cdc1
'http://http.debian.net/debian/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://http.debian.net/debian/pool/main/m/mawk/mawk_1.3.4.20200120-3.1.debian.tar.xz' mawk_1.3.4.20200120-3.1.debian.tar.xz 14080 SHA256:7850d7c44aa826635c79a6666b0d457a03524bcb0307697b062dd717d6d9d491
```

### `dpkg` source package: `mgcv=1.8-41-1`

Binary Packages:

- `r-cran-mgcv=1.8-41-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-mgcv/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris mgcv=1.8-41-1
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-41-1.dsc' mgcv_1.8-41-1.dsc 1833 SHA256:636a642de933e2b15c3910cc3dc231bef6243272185f024879eefab0cd5d9a46
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-41.orig.tar.gz' mgcv_1.8-41.orig.tar.gz 1072476 SHA256:2f7a030fe2be75edef6bd96147df46c2262f3cdc44c383d8f82b401df44fe690
'http://deb.debian.org/debian/pool/main/m/mgcv/mgcv_1.8-41-1.debian.tar.xz' mgcv_1.8-41-1.debian.tar.xz 5456 SHA256:04e21c268348d0c834057051b46a7bce8b3ec98aa215c985eaa178f32a92aa16
```

Other potentially useful URLs:

- https://sources.debian.net/src/mgcv/1.8-41-1/ (for browsing the source)
- https://sources.debian.net/src/mgcv/1.8-41-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/mgcv/1.8-41-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `mpclib3=1.3.1-1`

Binary Packages:

- `libmpc3:amd64=1.3.1-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.3.1-1
'http://http.debian.net/debian/pool/main/m/mpclib3/mpclib3_1.3.1-1.dsc' mpclib3_1.3.1-1.dsc 1877 SHA256:b2252a499fd0f8e92ce2cf7d8e68477ffc9dd06127803a91f0a1115822efec75
'http://http.debian.net/debian/pool/main/m/mpclib3/mpclib3_1.3.1.orig.tar.gz' mpclib3_1.3.1.orig.tar.gz 773573 SHA256:ab642492f5cf882b74aa0cb730cd410a81edcdbec895183ce930e706c1c759b8
'http://http.debian.net/debian/pool/main/m/mpclib3/mpclib3_1.3.1-1.debian.tar.xz' mpclib3_1.3.1-1.debian.tar.xz 4656 SHA256:25adb496258adacad69c022d712f96fbc465bcef9fd4751829dc351d9ce6a45d
```

### `dpkg` source package: `mpfr4=4.2.0-1`

Binary Packages:

- `libmpfr6:amd64=4.2.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.2.0-1
'http://http.debian.net/debian/pool/main/m/mpfr4/mpfr4_4.2.0-1.dsc' mpfr4_4.2.0-1.dsc 1959 SHA256:bfd38815d4d79f9ea3f14d94f61a075a0914ecbe4ef9666b7f6597340a60c250
'http://http.debian.net/debian/pool/main/m/mpfr4/mpfr4_4.2.0.orig.tar.xz' mpfr4_4.2.0.orig.tar.xz 1477532 SHA256:06a378df13501248c1b2db5aa977a2c8126ae849a9d9b7be2546fb4a9c26d993
'http://http.debian.net/debian/pool/main/m/mpfr4/mpfr4_4.2.0-1.debian.tar.xz' mpfr4_4.2.0-1.debian.tar.xz 12488 SHA256:05faf305be60659d8db47e1925fa4062be8fb89e5fcd70fb0e5444554b1625a8
```

### `dpkg` source package: `ncurses=6.4-2`

Binary Packages:

- `libncurses-dev:amd64=6.4-2`
- `libncurses5-dev:amd64=6.4-2`
- `libncurses6:amd64=6.4-2`
- `libncursesw6:amd64=6.4-2`
- `libtinfo6:amd64=6.4-2`
- `ncurses-base=6.4-2`
- `ncurses-bin=6.4-2`

Licenses: (parsed from: `/usr/share/doc/libncurses-dev/copyright`, `/usr/share/doc/libncurses5-dev/copyright`, `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.4-2
'http://http.debian.net/debian/pool/main/n/ncurses/ncurses_6.4-2.dsc' ncurses_6.4-2.dsc 4110 SHA256:32af7dee7301dad824671a08a66f0c9327498fcd8295d3830eb07e12272460ce
'http://http.debian.net/debian/pool/main/n/ncurses/ncurses_6.4.orig.tar.gz' ncurses_6.4.orig.tar.gz 3612591 SHA256:6931283d9ac87c5073f30b6290c4c75f21632bb4fc3603ac8100812bed248159
'http://http.debian.net/debian/pool/main/n/ncurses/ncurses_6.4.orig.tar.gz.asc' ncurses_6.4.orig.tar.gz.asc 729 SHA256:f9096c5311eab61908c142e77e58f503f9228e13d351365b3c331ca5ad5a67db
'http://http.debian.net/debian/pool/main/n/ncurses/ncurses_6.4-2.debian.tar.xz' ncurses_6.4-2.debian.tar.xz 55492 SHA256:edce466824e276ec7f86ff8fa926e46e6e7340b96b81cfadfc5fb73ae869d27a
```

### `dpkg` source package: `nettle=3.8.1-2`

Binary Packages:

- `libhogweed6:amd64=3.8.1-2`
- `libnettle8:amd64=3.8.1-2`

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
$ apt-get source -qq --print-uris nettle=3.8.1-2
'http://http.debian.net/debian/pool/main/n/nettle/nettle_3.8.1-2.dsc' nettle_3.8.1-2.dsc 2274 SHA256:a437e204da67612efb656cab354835f358b44c077c5c0a46d6e8c30b5c0bddff
'http://http.debian.net/debian/pool/main/n/nettle/nettle_3.8.1.orig.tar.gz' nettle_3.8.1.orig.tar.gz 2406251 SHA256:364f3e2b77cd7dcde83fd7c45219c834e54b0c75e428b6f894a23d12dd41cbfe
'http://http.debian.net/debian/pool/main/n/nettle/nettle_3.8.1.orig.tar.gz.asc' nettle_3.8.1.orig.tar.gz.asc 573 SHA256:71fe31c44728fdc144cbf12f30ca5d483992c17fd23afabe58f89d4201f66ddb
'http://http.debian.net/debian/pool/main/n/nettle/nettle_3.8.1-2.debian.tar.xz' nettle_3.8.1-2.debian.tar.xz 23396 SHA256:8f1eae9c6afffe545de294140f33d53352261478268dafee5ef72d840e1b3d7b
```

### `dpkg` source package: `nghttp2=1.52.0-1`

Binary Packages:

- `libnghttp2-14:amd64=1.52.0-1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `all-permissive`

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.52.0-1
'http://http.debian.net/debian/pool/main/n/nghttp2/nghttp2_1.52.0-1.dsc' nghttp2_1.52.0-1.dsc 2534 SHA256:bffd8160b6993a63ee53a3506203c7001a237cf9d4a3206f4771380290e45dce
'http://http.debian.net/debian/pool/main/n/nghttp2/nghttp2_1.52.0.orig.tar.gz' nghttp2_1.52.0.orig.tar.gz 1064232 SHA256:6b71561a9950b4a90fa36aa3160763f1437f3730d7a12434e416aa3f4ab145e0
'http://http.debian.net/debian/pool/main/n/nghttp2/nghttp2_1.52.0-1.debian.tar.xz' nghttp2_1.52.0-1.debian.tar.xz 11640 SHA256:3c43efdde81f32595f05e22bc03474cea63d91c89b93c2b6140b6e3338be5189
```

### `dpkg` source package: `nlme=3.1.162-1`

Binary Packages:

- `r-cran-nlme=3.1.162-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-nlme/copyright`)

- `GPL`
- `GPL `

Source:

```console
$ apt-get source -qq --print-uris nlme=3.1.162-1
'http://http.debian.net/debian/pool/main/n/nlme/nlme_3.1.162-1.dsc' nlme_3.1.162-1.dsc 1840 SHA256:049a9ae92e930c9e397f4d69c260f1f4842d37d72a0c2d10d6dccc08841ca35b
'http://http.debian.net/debian/pool/main/n/nlme/nlme_3.1.162.orig.tar.gz' nlme_3.1.162.orig.tar.gz 848546 SHA256:ba6da2575554afa2614c4cba9971f8a9f8a07622d201284cb78899f3d6a2dc67
'http://http.debian.net/debian/pool/main/n/nlme/nlme_3.1.162-1.debian.tar.xz' nlme_3.1.162-1.debian.tar.xz 7312 SHA256:f1c45b43c07e3344cfa08a57e3b3427eaf447ad0ea1b04c903edcf4c5969de8e
```

### `dpkg` source package: `openblas=0.3.21+ds-4`

Binary Packages:

- `libopenblas0-pthread:amd64=0.3.21+ds-4`

Licenses: (parsed from: `/usr/share/doc/libopenblas0-pthread/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-2-clause-texas`
- `BSD-3-clause`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openblas=0.3.21+ds-4
'http://http.debian.net/debian/pool/main/o/openblas/openblas_0.3.21%2bds-4.dsc' openblas_0.3.21+ds-4.dsc 4815 SHA256:2faed37b360c6d2a31e82032f8278d29bbec19d99425de2ce501614dff4e5880
'http://http.debian.net/debian/pool/main/o/openblas/openblas_0.3.21%2bds.orig.tar.xz' openblas_0.3.21+ds.orig.tar.xz 1885884 SHA256:bbec5cca61c8033b2d57aaecde205d709323a0b35a5f193290081dbb3826848a
'http://http.debian.net/debian/pool/main/o/openblas/openblas_0.3.21%2bds-4.debian.tar.xz' openblas_0.3.21+ds-4.debian.tar.xz 24824 SHA256:cb8ded6f29379c6a720ce3e7b62f9884419c7d3ba66e49184a3c09272af2065b
```

### `dpkg` source package: `openldap=2.5.13+dfsg-5`

Binary Packages:

- `libldap-2.5-0:amd64=2.5.13+dfsg-5`

Licenses: (parsed from: `/usr/share/doc/libldap-2.5-0/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-California`
- `BSD-3-clause-variant`
- `BSD-4-clause-California`
- `Beerware`
- `Expat`
- `Expat-ISC`
- `Expat-UNM`
- `F5`
- `FSF-unlimited`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `GPL-2+ with Libtool exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Autoconf exception`
- `GPL-3+ with Libtool exception`
- `JCG`
- `MIT-XC`
- `NeoSoft-permissive`
- `OpenLDAP-2.8`
- `UMich`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openldap=2.5.13+dfsg-5
'http://http.debian.net/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg-5.dsc' openldap_2.5.13+dfsg-5.dsc 3233 SHA256:3192f78a46825039c6c9de6808ae98ab3d1c8846f43d2109ed654fd9c33fe472
'http://http.debian.net/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg.orig.tar.xz' openldap_2.5.13+dfsg.orig.tar.xz 3727704 SHA256:1d95c400a3eae6730246614ef16883de3dbd1b14b01a1ebe3a9aa1ccad2c13ec
'http://http.debian.net/debian/pool/main/o/openldap/openldap_2.5.13%2bdfsg-5.debian.tar.xz' openldap_2.5.13+dfsg-5.debian.tar.xz 164516 SHA256:161e22c1c79e2f7c6013cfc2bbf0265d6bbb78d91a0fcfa9ca866837f2c31d88
```

### `dpkg` source package: `openssl=3.0.8-1`

Binary Packages:

- `libssl3:amd64=3.0.8-1`
- `openssl=3.0.8-1`

Licenses: (parsed from: `/usr/share/doc/libssl3/copyright`, `/usr/share/doc/openssl/copyright`)

- `Apache-2.0`
- `Artistic`
- `GPL-1`
- `GPL-1+`

Source:

```console
$ apt-get source -qq --print-uris openssl=3.0.8-1
'http://http.debian.net/debian/pool/main/o/openssl/openssl_3.0.8-1.dsc' openssl_3.0.8-1.dsc 2633 SHA256:0f8ac1a4ed55e1e1b70e93a781450273c02cf52aacc0eb70b69586a30ed68261
'http://http.debian.net/debian/pool/main/o/openssl/openssl_3.0.8.orig.tar.gz' openssl_3.0.8.orig.tar.gz 15151328 SHA256:6c13d2bf38fdf31eac3ce2a347073673f5d63263398f1f69d0df4a41253e4b3e
'http://http.debian.net/debian/pool/main/o/openssl/openssl_3.0.8.orig.tar.gz.asc' openssl_3.0.8.orig.tar.gz.asc 833 SHA256:565e31cbc436ec4de82c4b526a01caab1cdc9b78d32705f6e0f57666980331ad
'http://http.debian.net/debian/pool/main/o/openssl/openssl_3.0.8-1.debian.tar.xz' openssl_3.0.8-1.debian.tar.xz 75420 SHA256:b7b254f67f0f3443fc4441deec2b9bc6d2d24f9168827dd88ff2bab6f370976c
```

### `dpkg` source package: `p11-kit=0.24.1-2`

Binary Packages:

- `libp11-kit0:amd64=0.24.1-2`

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
$ apt-get source -qq --print-uris p11-kit=0.24.1-2
'http://http.debian.net/debian/pool/main/p/p11-kit/p11-kit_0.24.1-2.dsc' p11-kit_0.24.1-2.dsc 2501 SHA256:b88a483cb9afd5556ea4ac64d5df4543123a53bf0e50d1c01454887220259a89
'http://http.debian.net/debian/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz' p11-kit_0.24.1.orig.tar.xz 838304 SHA256:d8be783efd5cd4ae534cee4132338e3f40f182c3205d23b200094ec85faaaef8
'http://http.debian.net/debian/pool/main/p/p11-kit/p11-kit_0.24.1.orig.tar.xz.asc' p11-kit_0.24.1.orig.tar.xz.asc 833 SHA256:48041a234bac05f70519b0d4727e78a129ea80a51baf92c7d419f80b7cbdf0ab
'http://http.debian.net/debian/pool/main/p/p11-kit/p11-kit_0.24.1-2.debian.tar.xz' p11-kit_0.24.1-2.debian.tar.xz 23332 SHA256:9a14085b12cfd90e76008c2809e6557224243e1daeae4fbd7fad97e4396f730f
```

### `dpkg` source package: `pam=1.5.2-6`

Binary Packages:

- `libpam-modules:amd64=1.5.2-6`
- `libpam-modules-bin=1.5.2-6`
- `libpam-runtime=1.5.2-6`
- `libpam0g:amd64=1.5.2-6`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `BSD-3-clause`
- `BSD-tcp_wrappers`
- `Beerware`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+ with Bison exception`
- `LGPL-2`
- `LGPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pam=1.5.2-6
'http://http.debian.net/debian/pool/main/p/pam/pam_1.5.2-6.dsc' pam_1.5.2-6.dsc 1998 SHA256:2dbff29f5fc189c95b863ffd690795a7313515619ddadc470eab8a50b7555903
'http://http.debian.net/debian/pool/main/p/pam/pam_1.5.2.orig.tar.xz' pam_1.5.2.orig.tar.xz 988784 SHA256:e4ec7131a91da44512574268f493c6d8ca105c87091691b8e9b56ca685d4f94d
'http://http.debian.net/debian/pool/main/p/pam/pam_1.5.2-6.debian.tar.xz' pam_1.5.2-6.debian.tar.xz 122320 SHA256:97adad0df930ba5ed52b88bef6d494a1b303ca2eb5be9e347479a23e4d9254fc
```

### `dpkg` source package: `pango1.0=1.50.12+ds-1`

Binary Packages:

- `libpango-1.0-0:amd64=1.50.12+ds-1`
- `libpangocairo-1.0-0:amd64=1.50.12+ds-1`
- `libpangoft2-1.0-0:amd64=1.50.12+ds-1`

Licenses: (parsed from: `/usr/share/doc/libpango-1.0-0/copyright`, `/usr/share/doc/libpangocairo-1.0-0/copyright`, `/usr/share/doc/libpangoft2-1.0-0/copyright`)

- `Apache-2`
- `Apache-2.0`
- `Bitstream-Vera`
- `CC0-1.0`
- `Chromium-BSD-style`
- `Example`
- `GPL-2+`
- `GPL-2.0`
- `ICU`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `OFL-1.1`
- `TCL`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris pango1.0=1.50.12+ds-1
'http://http.debian.net/debian/pool/main/p/pango1.0/pango1.0_1.50.12%2bds-1.dsc' pango1.0_1.50.12+ds-1.dsc 3544 SHA256:596e06d288dbdcafcf08fb43201055d6f86a9a66911c7aa28112da781353489b
'http://http.debian.net/debian/pool/main/p/pango1.0/pango1.0_1.50.12%2bds.orig.tar.xz' pango1.0_1.50.12+ds.orig.tar.xz 1729376 SHA256:ec19df0570cf87583ebff514968a958c25031a6f47eb39e8eb06530166ffb239
'http://http.debian.net/debian/pool/main/p/pango1.0/pango1.0_1.50.12%2bds-1.debian.tar.xz' pango1.0_1.50.12+ds-1.debian.tar.xz 41088 SHA256:40e68995280ba7ea475ef9049bd9beb224e4552987d124507abdc813d5e903d9
```

### `dpkg` source package: `patch=2.7.6-7`

Binary Packages:

- `patch=2.7.6-7`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-7
'http://http.debian.net/debian/pool/main/p/patch/patch_2.7.6-7.dsc' patch_2.7.6-7.dsc 1706 SHA256:d954fd576d935ac54b7d44d4976eb52d0da84a57f7bad90c6e5bd5e33595030a
'http://http.debian.net/debian/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://http.debian.net/debian/pool/main/p/patch/patch_2.7.6-7.debian.tar.xz' patch_2.7.6-7.debian.tar.xz 15084 SHA256:7725f30b042d8cf63516e480036e93ca2ff0ce5ad3754db4a4e69d33e96a2624
```

### `dpkg` source package: `pcre2=10.42-1`

Binary Packages:

- `libpcre2-16-0:amd64=10.42-1`
- `libpcre2-32-0:amd64=10.42-1`
- `libpcre2-8-0:amd64=10.42-1`
- `libpcre2-dev:amd64=10.42-1`
- `libpcre2-posix3:amd64=10.42-1`

Licenses: (parsed from: `/usr/share/doc/libpcre2-16-0/copyright`, `/usr/share/doc/libpcre2-32-0/copyright`, `/usr/share/doc/libpcre2-8-0/copyright`, `/usr/share/doc/libpcre2-dev/copyright`, `/usr/share/doc/libpcre2-posix3/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-3-clause-Cambridge with BINARY LIBRARY-LIKE PACKAGES exception`
- `X11`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pcre2=10.42-1
'http://http.debian.net/debian/pool/main/p/pcre2/pcre2_10.42-1.dsc' pcre2_10.42-1.dsc 2302 SHA256:726dafe7a8d07332d4df61edf23f384ddb158b2b263846273d1103b6b9a7c176
'http://http.debian.net/debian/pool/main/p/pcre2/pcre2_10.42.orig.tar.gz' pcre2_10.42.orig.tar.gz 2397194 SHA256:c33b418e3b936ee3153de2c61cc638e7e4fe3156022a5c77d0711bcbb9d64f1f
'http://http.debian.net/debian/pool/main/p/pcre2/pcre2_10.42-1.diff.gz' pcre2_10.42-1.diff.gz 7895 SHA256:8267c3acacb04e8a077235f676187393e295443fc16ff46ddbe5f6476879c8cb
```

### `dpkg` source package: `pcre3=2:8.39-15`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-15`
- `libpcre3:amd64=2:8.39-15`
- `libpcre3-dev:amd64=2:8.39-15`
- `libpcre32-3:amd64=2:8.39-15`
- `libpcrecpp0v5:amd64=2:8.39-15`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-15
'http://http.debian.net/debian/pool/main/p/pcre3/pcre3_8.39-15.dsc' pcre3_8.39-15.dsc 2224 SHA256:335f76ecf668b069c9f3a0eb7904df3a271686d769e3e16b5e4f6b52e4254b9d
'http://http.debian.net/debian/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://http.debian.net/debian/pool/main/p/pcre3/pcre3_8.39-15.debian.tar.gz' pcre3_8.39-15.debian.tar.gz 27007 SHA256:e596e7ad1d4e60af4b9655b1582a0ef765aea1e09ce2efa031611d03b1353c67
```

### `dpkg` source package: `perl=5.36.0-7`

Binary Packages:

- `libperl5.36:amd64=5.36.0-7`
- `perl=5.36.0-7`
- `perl-base=5.36.0-7`
- `perl-modules-5.36=5.36.0-7`

Licenses: (parsed from: `/usr/share/doc/libperl5.36/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.36/copyright`)

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
$ apt-get source -qq --print-uris perl=5.36.0-7
'http://http.debian.net/debian/pool/main/p/perl/perl_5.36.0-7.dsc' perl_5.36.0-7.dsc 2886 SHA256:d9992947bb5c254e1bf96c56f12ac0bc962a2ff1e700834f871fb412526b4a8b
'http://http.debian.net/debian/pool/main/p/perl/perl_5.36.0.orig-regen-configure.tar.xz' perl_5.36.0.orig-regen-configure.tar.xz 417784 SHA256:10ac353bc5a933403afe60ed1817e7a456f99bdbcaf80c1cdb0eb3a08ea56d4e
'http://http.debian.net/debian/pool/main/p/perl/perl_5.36.0.orig.tar.xz' perl_5.36.0.orig.tar.xz 13051500 SHA256:0f386dccbee8e26286404b2cca144e1005be65477979beb9b1ba272d4819bcf0
'http://http.debian.net/debian/pool/main/p/perl/perl_5.36.0-7.debian.tar.xz' perl_5.36.0-7.debian.tar.xz 169288 SHA256:c8a46245b7102d60539cc4c550977f35cbb8409643abc0d00c7a8b78d0271bea
```

### `dpkg` source package: `pixman=0.42.2-1`

Binary Packages:

- `libpixman-1-0:amd64=0.42.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pixman=0.42.2-1
'http://http.debian.net/debian/pool/main/p/pixman/pixman_0.42.2-1.dsc' pixman_0.42.2-1.dsc 2021 SHA256:393302f5ba22d1206c456902baa02cdd577cb74fe35ec6659f587cce67b91b3d
'http://http.debian.net/debian/pool/main/p/pixman/pixman_0.42.2.orig.tar.gz' pixman_0.42.2.orig.tar.gz 959669 SHA256:ea1480efada2fd948bc75366f7c349e1c96d3297d09a3fe62626e38e234a625e
'http://http.debian.net/debian/pool/main/p/pixman/pixman_0.42.2-1.diff.gz' pixman_0.42.2-1.diff.gz 319616 SHA256:dd6472676c68260a298e52f45c485d3cc85c4bf25df8af0f68e37acff7bfed8a
```

### `dpkg` source package: `pkgconf=1.8.1-1`

Binary Packages:

- `libpkgconf3:amd64=1.8.1-1`
- `pkg-config:amd64=1.8.1-1`
- `pkgconf:amd64=1.8.1-1`
- `pkgconf-bin=1.8.1-1`

Licenses: (parsed from: `/usr/share/doc/libpkgconf3/copyright`, `/usr/share/doc/pkg-config/copyright`, `/usr/share/doc/pkgconf/copyright`, `/usr/share/doc/pkgconf-bin/copyright`)

- `BSD-2`
- `BSD-4`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pkgconf=1.8.1-1
'http://http.debian.net/debian/pool/main/p/pkgconf/pkgconf_1.8.1-1.dsc' pkgconf_1.8.1-1.dsc 1570 SHA256:cf1f645d7a9522354a334130a55d16be7d62e304070d6675f826844b143dc47e
'http://http.debian.net/debian/pool/main/p/pkgconf/pkgconf_1.8.1.orig.tar.xz' pkgconf_1.8.1.orig.tar.xz 302372 SHA256:644361ada2942be05655d4452eb018791647c31bba429b287f1f68deb2dc6840
'http://http.debian.net/debian/pool/main/p/pkgconf/pkgconf_1.8.1-1.debian.tar.xz' pkgconf_1.8.1-1.debian.tar.xz 15060 SHA256:bd9330105d17bf4b9a9d2aaba4a150b35da21b7ba4b45d4bf7e034fa6e53ba2f
```

### `dpkg` source package: `r-base=4.3.0-1`

Binary Packages:

- `r-base=4.3.0-1`
- `r-base-core=4.3.0-1`
- `r-base-dev=4.3.0-1`
- `r-recommended=4.3.0-1`

Licenses: (parsed from: `/usr/share/doc/r-base/copyright`, `/usr/share/doc/r-base-core/copyright`, `/usr/share/doc/r-base-dev/copyright`, `/usr/share/doc/r-recommended/copyright`)

- `Artistic`
- `GPL-2`
- `GPL-3`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-base=4.3.0-1
'http://http.debian.net/debian/pool/main/r/r-base/r-base_4.3.0-1.dsc' r-base_4.3.0-1.dsc 2939 SHA256:0070ae029bc7da8fff1d0888067e96bc945766d5066492c69ea08bd5a16d1540
'http://http.debian.net/debian/pool/main/r/r-base/r-base_4.3.0.orig.tar.gz' r-base_4.3.0.orig.tar.gz 34821768 SHA256:45dcc48b6cf27d361020f77fde1a39209e997b81402b3663ca1c010056a6a609
'http://http.debian.net/debian/pool/main/r/r-base/r-base_4.3.0-1.debian.tar.xz' r-base_4.3.0-1.debian.tar.xz 99184 SHA256:db504a670f9f7260519cff72ef0bcabfd22189d97f44548a09f0f0424d4a4123
```

### `dpkg` source package: `r-cran-class=7.3-21-1`

Binary Packages:

- `r-cran-class=7.3-21-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-class/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-class=7.3-21-1
'http://http.debian.net/debian/pool/main/r/r-cran-class/r-cran-class_7.3-21-1.dsc' r-cran-class_7.3-21-1.dsc 1873 SHA256:10ae439e889843ad9717de58086cac9930bf2162c491a6d6a281f9bad33fed15
'http://http.debian.net/debian/pool/main/r/r-cran-class/r-cran-class_7.3-21.orig.tar.gz' r-cran-class_7.3-21.orig.tar.gz 20812 SHA256:0c19404aa4d2da61a62495e788b07c8e429c4c5ee64486ea5e6dd347bcaecddf
'http://http.debian.net/debian/pool/main/r/r-cran-class/r-cran-class_7.3-21-1.debian.tar.xz' r-cran-class_7.3-21-1.debian.tar.xz 3240 SHA256:b04341e179c40c56ad93116a1dc4e4386f03792101643ed796d768f4b346f160
```

### `dpkg` source package: `r-cran-docopt=0.7.1-2`

Binary Packages:

- `r-cran-docopt=0.7.1-2`

Licenses: (parsed from: `/usr/share/doc/r-cran-docopt/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris r-cran-docopt=0.7.1-2
'http://http.debian.net/debian/pool/main/r/r-cran-docopt/r-cran-docopt_0.7.1-2.dsc' r-cran-docopt_0.7.1-2.dsc 2087 SHA256:f7713b448b9b14766351e295d3ee0059f3a1c6319ecdf5ef33d5da40bc609d1b
'http://http.debian.net/debian/pool/main/r/r-cran-docopt/r-cran-docopt_0.7.1.orig.tar.gz' r-cran-docopt_0.7.1.orig.tar.gz 29465 SHA256:9f473887e4607e9b21fd4ab02e802858d0ac2ca6dad9e357a9d884a47fe4b0ff
'http://http.debian.net/debian/pool/main/r/r-cran-docopt/r-cran-docopt_0.7.1-2.debian.tar.xz' r-cran-docopt_0.7.1-2.debian.tar.xz 2472 SHA256:3358c9988254f326b3d2a351f3a75fd3c655d56de13e7f822cceaf39fb1f7fca
```

### `dpkg` source package: `r-cran-mass=7.3-58.2-1`

Binary Packages:

- `r-cran-mass=7.3-58.2-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-mass/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-mass=7.3-58.2-1
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-58.2-1.dsc' r-cran-mass_7.3-58.2-1.dsc 1865 SHA256:8a079ed0c489c45e8f58591e30068cb8028dfb8e16a18230fba49eb9a04ca362
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-58.2.orig.tar.gz' r-cran-mass_7.3-58.2.orig.tar.gz 515055 SHA256:b5c09d5368ca432bb21ebb4997433dbefb28e19174851e2d8358bab02add784b
'http://deb.debian.org/debian/pool/main/r/r-cran-mass/r-cran-mass_7.3-58.2-1.debian.tar.xz' r-cran-mass_7.3-58.2-1.debian.tar.xz 6476 SHA256:48e24e06bb4d1c59a86837e9dae76dfe618e6cef5b4e030fd90576dff1397037
```

Other potentially useful URLs:

- https://sources.debian.net/src/r-cran-mass/7.3-58.2-1/ (for browsing the source)
- https://sources.debian.net/src/r-cran-mass/7.3-58.2-1/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/r-cran-mass/7.3-58.2-1/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `r-cran-nnet=7.3-18-1`

Binary Packages:

- `r-cran-nnet=7.3-18-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-nnet/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-nnet=7.3-18-1
'http://http.debian.net/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-18-1.dsc' r-cran-nnet_7.3-18-1.dsc 1848 SHA256:72f8e7ab7bd771fe59dc7a5ab09d0bece9cd3d45e818edb36f72e316c92fc5ed
'http://http.debian.net/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-18.orig.tar.gz' r-cran-nnet_7.3-18.orig.tar.gz 29146 SHA256:d29aebfb5cb00071eecf754d55db5d474a6fda88860df5c9d31ba89aa8d9e3d0
'http://http.debian.net/debian/pool/main/r/r-cran-nnet/r-cran-nnet_7.3-18-1.debian.tar.xz' r-cran-nnet_7.3-18-1.debian.tar.xz 3268 SHA256:030e75928fbdff50c16adf02c0ad967878c7cd77a487f8ebad4f2aa88b202eb8
```

### `dpkg` source package: `r-cran-spatial=7.3-16-1`

Binary Packages:

- `r-cran-spatial=7.3-16-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-spatial/copyright`)

- `GPL-2`
- `GPL-2 | GPL-3`

Source:

```console
$ apt-get source -qq --print-uris r-cran-spatial=7.3-16-1
'http://http.debian.net/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-16-1.dsc' r-cran-spatial_7.3-16-1.dsc 1884 SHA256:c28cbd1546fc782777a0e53807edb0f023ae6dcbd0c7bf603d2d87448c15cfb5
'http://http.debian.net/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-16.orig.tar.gz' r-cran-spatial_7.3-16.orig.tar.gz 44631 SHA256:e46565a64c5ec148a77789867e5103746462a41de294539b230bad2a0e16e406
'http://http.debian.net/debian/pool/main/r/r-cran-spatial/r-cran-spatial_7.3-16-1.debian.tar.xz' r-cran-spatial_7.3-16-1.debian.tar.xz 3204 SHA256:c698569124b560ff42ebb6e3731115197967d78475fbcaec7c937444d6db0f96
```

### `dpkg` source package: `readline=8.2-1.3`

Binary Packages:

- `libreadline-dev:amd64=8.2-1.3`
- `libreadline8:amd64=8.2-1.3`
- `readline-common=8.2-1.3`

Licenses: (parsed from: `/usr/share/doc/libreadline-dev/copyright`, `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ISC-no-attribution`

Source:

```console
$ apt-get source -qq --print-uris readline=8.2-1.3
'http://http.debian.net/debian/pool/main/r/readline/readline_8.2-1.3.dsc' readline_8.2-1.3.dsc 2553 SHA256:05497ea99bef3f14b8d502cbe3f84fe7bbc0bce1c4f139ca32f0fd60dcac977e
'http://http.debian.net/debian/pool/main/r/readline/readline_8.2.orig.tar.gz' readline_8.2.orig.tar.gz 3043952 SHA256:3feb7171f16a84ee82ca18a36d7b9be109a52c04f492a053331d7d1095007c35
'http://http.debian.net/debian/pool/main/r/readline/readline_8.2-1.3.debian.tar.xz' readline_8.2-1.3.debian.tar.xz 30016 SHA256:8cd3c02d6c07b4cf57da607de168a9e347ee05c31857f0f6236fe3df4fc207d9
```

### `dpkg` source package: `rmatrix=1.5-3-1`

Binary Packages:

- `r-cran-matrix=1.5-3-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-matrix/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rmatrix=1.5-3-1
'http://http.debian.net/debian/pool/main/r/rmatrix/rmatrix_1.5-3-1.dsc' rmatrix_1.5-3-1.dsc 1860 SHA256:a5d76f341039c2c96b0680c6f933c511e3ced02daaa40437294c4baac61ef1d1
'http://http.debian.net/debian/pool/main/r/rmatrix/rmatrix_1.5-3.orig.tar.gz' rmatrix_1.5-3.orig.tar.gz 2163568 SHA256:4e720f4edc97b1c09646a445851b1ce955caf6b1de8306a2283328b526fee00d
'http://http.debian.net/debian/pool/main/r/rmatrix/rmatrix_1.5-3-1.debian.tar.xz' rmatrix_1.5-3-1.debian.tar.xz 5760 SHA256:1041176f784dbbb40ac6d7e13a0789c103b6e1fedb3ff981c2e7b6eaa9a1bbeb
```

### `dpkg` source package: `rpart=4.1.19-1`

Binary Packages:

- `r-cran-rpart=4.1.19-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-rpart/copyright`)

- `GPL-2`
- `GPL-2+ | license included below`

Source:

```console
$ apt-get source -qq --print-uris rpart=4.1.19-1
'http://http.debian.net/debian/pool/main/r/rpart/rpart_4.1.19-1.dsc' rpart_4.1.19-1.dsc 1843 SHA256:03c01b26658418329eb1c894902da1fb2a601c1e1d22f7ba110e995bb3cd5216
'http://http.debian.net/debian/pool/main/r/rpart/rpart_4.1.19.orig.tar.gz' rpart_4.1.19.orig.tar.gz 859025 SHA256:fe723ed0b5583fae8b40e6fecc29b357229cb11f2339b02a4e4f812926249565
'http://http.debian.net/debian/pool/main/r/rpart/rpart_4.1.19-1.debian.tar.xz' rpart_4.1.19-1.debian.tar.xz 4388 SHA256:3bea7d8cd1f2652d3d3966f23c61369c391dac8b2ab229700937c028b505c74a
```

### `dpkg` source package: `rpcsvc-proto=1.4.3-1`

Binary Packages:

- `rpcsvc-proto=1.4.3-1`

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
$ apt-get source -qq --print-uris rpcsvc-proto=1.4.3-1
'http://http.debian.net/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.3-1.dsc' rpcsvc-proto_1.4.3-1.dsc 1999 SHA256:7d8e122bd18b02fe0de6d467a0ecdafff74035b3e1ed0da1c0c792d9c015682f
'http://http.debian.net/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.3.orig.tar.xz' rpcsvc-proto_1.4.3.orig.tar.xz 167964 SHA256:69315e94430f4e79c74d43422f4a36e6259e97e67e2677b2c7d7060436bd99b1
'http://http.debian.net/debian/pool/main/r/rpcsvc-proto/rpcsvc-proto_1.4.3-1.debian.tar.xz' rpcsvc-proto_1.4.3-1.debian.tar.xz 4228 SHA256:02034b9dadcf3af5424f72eb65c3842c8d7117b6b78e7a3c798316ceb60843d1
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2+b2`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2
'http://http.debian.net/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2.dsc 2299 SHA256:a296819cd2ab5880b67ad963ef0867cb10e462f4403e52565aa863eb05bb1370
'http://http.debian.net/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://http.debian.net/debian/pool/main/r/rtmpdump/rtmpdump_2.4%2b20151223.gitfa8646d.1-2.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2.debian.tar.xz 8096 SHA256:26d47de07d16285e4ca55b0828cbbf1ba35e671f9b3500a87e301fe755d26882
```

### `dpkg` source package: `sed=4.9-1`

Binary Packages:

- `sed=4.9-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `BSD-4-clause-UC`
- `BSL-1`
- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `X11`
- `pcre`

Source:

```console
$ apt-get source -qq --print-uris sed=4.9-1
'http://http.debian.net/debian/pool/main/s/sed/sed_4.9-1.dsc' sed_4.9-1.dsc 2077 SHA256:f0670e00c1ad51321e5b741a737e977cdb3b0eef47964b2269535f7820df576a
'http://http.debian.net/debian/pool/main/s/sed/sed_4.9.orig.tar.xz' sed_4.9.orig.tar.xz 1397092 SHA256:6e226b732e1cd739464ad6862bd1a1aba42d7982922da7a53519631d24975181
'http://http.debian.net/debian/pool/main/s/sed/sed_4.9.orig.tar.xz.asc' sed_4.9.orig.tar.xz.asc 833 SHA256:9ea64f215b308ae0a80cd958daaac23bb13491d69a472a0195974d107890a8c6
'http://http.debian.net/debian/pool/main/s/sed/sed_4.9-1.debian.tar.xz' sed_4.9-1.debian.tar.xz 62616 SHA256:24cdd6a3b40909ec374bd87df62364904bbe18fc12ba66111e9f9f617ff7f679
```

### `dpkg` source package: `sensible-utils=0.0.17+nmu1`

Binary Packages:

- `sensible-utils=0.0.17+nmu1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.17+nmu1
'http://http.debian.net/debian/pool/main/s/sensible-utils/sensible-utils_0.0.17%2bnmu1.dsc' sensible-utils_0.0.17+nmu1.dsc 1728 SHA256:764436dac8b6796ba49e9dd96e3c9ef8612cacad1953e6cd7525a17b99a9e4a1
'http://http.debian.net/debian/pool/main/s/sensible-utils/sensible-utils_0.0.17%2bnmu1.tar.xz' sensible-utils_0.0.17+nmu1.tar.xz 66476 SHA256:a4ead62e0dc8f965453221dcb09c964abc4f1bedad24f527d33c443a1570cb31
```

### `dpkg` source package: `shadow=1:4.13+dfsg1-1`

Binary Packages:

- `login=1:4.13+dfsg1-1+b1`
- `passwd=1:4.13+dfsg1-1+b1`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `BSD-3-clause`
- `GPL-1`
- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.13+dfsg1-1
'http://http.debian.net/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1-1.dsc' shadow_4.13+dfsg1-1.dsc 2402 SHA256:e27b0676e87d4ae75a57cba55433517e8aa30d45817c691c63045d5e6195c667
'http://http.debian.net/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1.orig.tar.xz' shadow_4.13+dfsg1.orig.tar.xz 1811752 SHA256:a8bb3a2aceff1cbe39d0f50687dcc1d7e7be0516a9d954d8e2eedb93f5906207
'http://http.debian.net/debian/pool/main/s/shadow/shadow_4.13%2bdfsg1-1.debian.tar.xz' shadow_4.13+dfsg1-1.debian.tar.xz 78988 SHA256:cbd43c96ebad42bfb1656b5e691cc165f52d1dd6b1ee89202c2a09e59d663b1c
```

### `dpkg` source package: `survival=3.5-3-1`

Binary Packages:

- `r-cran-survival=3.5-3-1`

Licenses: (parsed from: `/usr/share/doc/r-cran-survival/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris survival=3.5-3-1
'http://http.debian.net/debian/pool/main/s/survival/survival_3.5-3-1.dsc' survival_3.5-3-1.dsc 1861 SHA256:15f6d75cd992eb2b77f7f896390d4072fc8c6e255f95872061048a1aa1b6f057
'http://http.debian.net/debian/pool/main/s/survival/survival_3.5-3.orig.tar.gz' survival_3.5-3.orig.tar.gz 6247942 SHA256:bfa082fd938760fa06f76d70fe2a613c70620e4d2870f14270d8e20f1fbc44c6
'http://http.debian.net/debian/pool/main/s/survival/survival_3.5-3-1.debian.tar.xz' survival_3.5-3-1.debian.tar.xz 6244 SHA256:c8227f3ea3babc73fc7b0dad526c2188dd72574f0110cc3241a0b5e805494573
```

### `dpkg` source package: `systemd=252.6-1`

Binary Packages:

- `libsystemd0:amd64=252.6-1`
- `libudev1:amd64=252.6-1`

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
$ apt-get source -qq --print-uris systemd=252.6-1
'http://http.debian.net/debian/pool/main/s/systemd/systemd_252.6-1.dsc' systemd_252.6-1.dsc 6571 SHA256:16872c4ce37094d38eea11322084d4e852261879d6d605fe6b69bbc219d25b5a
'http://http.debian.net/debian/pool/main/s/systemd/systemd_252.6.orig.tar.gz' systemd_252.6.orig.tar.gz 11823064 SHA256:5f0b391f7e481f9ce0798515f34e85963990d42a27f9f80fc9e7321610b69784
'http://http.debian.net/debian/pool/main/s/systemd/systemd_252.6-1.debian.tar.xz' systemd_252.6-1.debian.tar.xz 170404 SHA256:c5bb237f47188e433e6f7e157a2365f2be539e695619a668172e26bf108090c3
```

### `dpkg` source package: `sysvinit=3.06-2`

Binary Packages:

- `sysvinit-utils=3.06-2`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2.0`
- `GPL-2.0+`
- `GPL-3`
- `GPL-3.0`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sysvinit/3.06-2/


### `dpkg` source package: `tar=1.34+dfsg-1`

Binary Packages:

- `tar=1.34+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/tar/1.34+dfsg-1/


### `dpkg` source package: `tcl8.6=8.6.13+dfsg-2`

Binary Packages:

- `libtcl8.6:amd64=8.6.13+dfsg-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tcl8.6=8.6.13+dfsg-2
'http://http.debian.net/debian/pool/main/t/tcl8.6/tcl8.6_8.6.13%2bdfsg-2.dsc' tcl8.6_8.6.13+dfsg-2.dsc 2120 SHA256:7965fd63c4cb970d0f675f574f6730114c806139e433cb3589a428658fc4d0cd
'http://http.debian.net/debian/pool/main/t/tcl8.6/tcl8.6_8.6.13%2bdfsg.orig.tar.gz' tcl8.6_8.6.13+dfsg.orig.tar.gz 6302749 SHA256:83bce7277e3825df0179567e0d8a431ebb1a126df53ea4a94af89dd4dd0f26d5
'http://http.debian.net/debian/pool/main/t/tcl8.6/tcl8.6_8.6.13%2bdfsg-2.debian.tar.xz' tcl8.6_8.6.13+dfsg-2.debian.tar.xz 14336 SHA256:899c8d800988caa1f5a8b070d3697f29c3d098754416cc2816b94dfa93aef009
```

### `dpkg` source package: `tex-gyre=20180621-6`

Binary Packages:

- `fonts-texgyre=20180621-6`

Licenses: (parsed from: `/usr/share/doc/fonts-texgyre/copyright`)

- `DejaVu-License`
- `GPL-2`
- `GPL-2+`
- `GUST-Font-License`

Source:

```console
$ apt-get source -qq --print-uris tex-gyre=20180621-6
'http://http.debian.net/debian/pool/main/t/tex-gyre/tex-gyre_20180621-6.dsc' tex-gyre_20180621-6.dsc 2241 SHA256:83a26e65fee0ac79f31a44e083e03da2fef7b031c70d0f336796782cc0fed099
'http://http.debian.net/debian/pool/main/t/tex-gyre/tex-gyre_20180621.orig.tar.gz' tex-gyre_20180621.orig.tar.gz 24033627 SHA256:fe6b0f8ca6890d4a369f36c3b45bc30470069701a2f59042178ad5933fc9cdb8
'http://http.debian.net/debian/pool/main/t/tex-gyre/tex-gyre_20180621-6.debian.tar.xz' tex-gyre_20180621-6.debian.tar.xz 11632 SHA256:731e04abb52038a7de626e4679d6b823b2d692be029bb88399951fb69b286f67
```

### `dpkg` source package: `tiff=4.5.0-5`

Binary Packages:

- `libtiff6:amd64=4.5.0-5`

Licenses: (parsed from: `/usr/share/doc/libtiff6/copyright`)

- `Hylafax`

Source:

```console
$ apt-get source -qq --print-uris tiff=4.5.0-5
'http://http.debian.net/debian/pool/main/t/tiff/tiff_4.5.0-5.dsc' tiff_4.5.0-5.dsc 2255 SHA256:cec33019d88624f8ad8a771c8a4cac4b0d07f18e69171c997dab87e7c69c1914
'http://http.debian.net/debian/pool/main/t/tiff/tiff_4.5.0.orig.tar.bz2' tiff_4.5.0.orig.tar.bz2 2050377 SHA256:638f43d7dea33948d5dee7f39572fc0194d9cc3c74195de9dd26a4388a1f880a
'http://http.debian.net/debian/pool/main/t/tiff/tiff_4.5.0-5.debian.tar.xz' tiff_4.5.0-5.debian.tar.xz 26516 SHA256:3fc31dfe0aef671343b84ce23e7baf64789e306838fb176819c18d0754b3811f
```

### `dpkg` source package: `tk8.6=8.6.13-2`

Binary Packages:

- `libtk8.6:amd64=8.6.13-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris tk8.6=8.6.13-2
'http://http.debian.net/debian/pool/main/t/tk8.6/tk8.6_8.6.13-2.dsc' tk8.6_8.6.13-2.dsc 2155 SHA256:12783fea0125ef3e67a1a07b2b24f7e27329214394ca5b543bd38716a91d7a1e
'http://http.debian.net/debian/pool/main/t/tk8.6/tk8.6_8.6.13.orig.tar.gz' tk8.6_8.6.13.orig.tar.gz 4546848 SHA256:2e65fa069a23365440a3c56c556b8673b5e32a283800d8d9b257e3f584ce0675
'http://http.debian.net/debian/pool/main/t/tk8.6/tk8.6_8.6.13-2.debian.tar.xz' tk8.6_8.6.13-2.debian.tar.xz 10740 SHA256:1e57bc189cfa3e73e140aa1853b91e6c9a4da99eccd931de24e0c2cd525f8319
```

### `dpkg` source package: `tzdata=2023c-2`

Binary Packages:

- `tzdata=2023c-2`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2023c-2
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2023c-2.dsc' tzdata_2023c-2.dsc 2332 SHA256:3c4c8d81c7b57dad577bd21fbb7eea93e9ac37b38b33ab52621a1016ec12ccde
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2023c.orig.tar.gz' tzdata_2023c.orig.tar.gz 443902 SHA256:3f510b5d1b4ae9bb38e485aa302a776b317fb3637bdb6404c4adf7b6cadd965c
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2023c.orig.tar.gz.asc' tzdata_2023c.orig.tar.gz.asc 833 SHA256:d5ec7b6ceddc46aa137c0ef85fa5c87445509d7997c067ee0fd2e2a23f833557
'http://deb.debian.org/debian/pool/main/t/tzdata/tzdata_2023c-2.debian.tar.xz' tzdata_2023c-2.debian.tar.xz 117956 SHA256:e886e6b1faf63e27636eacba708b8e5935ec971d5ad6210bf960e9caa9db1b2e
```

Other potentially useful URLs:

- https://sources.debian.net/src/tzdata/2023c-2/ (for browsing the source)
- https://sources.debian.net/src/tzdata/2023c-2/debian/copyright/ (for direct copyright/license information)
- http://snapshot.debian.org/package/tzdata/2023c-2/ (for access to the source package after it no longer exists in the archive)

### `dpkg` source package: `ucf=3.0043+nmu1`

Binary Packages:

- `ucf=3.0043+nmu1`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0043+nmu1
'http://http.debian.net/debian/pool/main/u/ucf/ucf_3.0043%2bnmu1.dsc' ucf_3.0043+nmu1.dsc 1567 SHA256:5ef70fa7a58cd3f162932661453a1e9d21d749b47a1aa84198f7c4cd9eac20ee
'http://http.debian.net/debian/pool/main/u/ucf/ucf_3.0043%2bnmu1.tar.xz' ucf_3.0043+nmu1.tar.xz 70916 SHA256:a07143046236cb082517e346362306cb3fe4d3634cad1add40c905b0e0ecf58c
```

### `dpkg` source package: `unzip=6.0-28`

Binary Packages:

- `unzip=6.0-28`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris unzip=6.0-28
'http://http.debian.net/debian/pool/main/u/unzip/unzip_6.0-28.dsc' unzip_6.0-28.dsc 1359 SHA256:f5b486028b61a145b591fdd96aaeaf89ef6eef164a299f43bd5e6704bdefc8a2
'http://http.debian.net/debian/pool/main/u/unzip/unzip_6.0.orig.tar.gz' unzip_6.0.orig.tar.gz 1376845 SHA256:036d96991646d0449ed0aa952e4fbe21b476ce994abc276e49d30e686708bd37
'http://http.debian.net/debian/pool/main/u/unzip/unzip_6.0-28.debian.tar.xz' unzip_6.0-28.debian.tar.xz 25032 SHA256:e51364116c84739c591728ecc841113a914fa11358fd10ff0d6813524d811bb9
```

### `dpkg` source package: `usrmerge=35`

Binary Packages:

- `usr-is-merged=35`

Licenses: (parsed from: `/usr/share/doc/usr-is-merged/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris usrmerge=35
'http://http.debian.net/debian/pool/main/u/usrmerge/usrmerge_35.dsc' usrmerge_35.dsc 981 SHA256:f8f7fa03aa912a65f54584b1cbaed193575521ab7ffa16c93c9920c41726c9fd
'http://http.debian.net/debian/pool/main/u/usrmerge/usrmerge_35.tar.xz' usrmerge_35.tar.xz 14416 SHA256:ec52fa22f174204f24ebb45caf579275f5a2b2404be5d4b3fe29ad60ad566829
```

### `dpkg` source package: `util-linux=2.38.1-5`

Binary Packages:

- `bsdutils=1:2.38.1-5+b1`
- `libblkid1:amd64=2.38.1-5+b1`
- `libmount1:amd64=2.38.1-5+b1`
- `libsmartcols1:amd64=2.38.1-5+b1`
- `libuuid1:amd64=2.38.1-5+b1`
- `mount=2.38.1-5+b1`
- `util-linux=2.38.1-5+b1`
- `util-linux-extra=2.38.1-5+b1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/util-linux-extra/copyright`)

- `BSD-3-clause`
- `BSD-4-clause`
- `BSLA`
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
$ apt-get source -qq --print-uris util-linux=2.38.1-5
'http://http.debian.net/debian/pool/main/u/util-linux/util-linux_2.38.1-5.dsc' util-linux_2.38.1-5.dsc 4547 SHA256:23b6c80b27468a9b7821ff7059b6a0bbb23fa9b2305856ffb78a993726491c08
'http://http.debian.net/debian/pool/main/u/util-linux/util-linux_2.38.1.orig.tar.xz' util-linux_2.38.1.orig.tar.xz 7495904 SHA256:60492a19b44e6cf9a3ddff68325b333b8b52b6c59ce3ebd6a0ecaa4c5117e84f
'http://http.debian.net/debian/pool/main/u/util-linux/util-linux_2.38.1-5.debian.tar.xz' util-linux_2.38.1-5.debian.tar.xz 113832 SHA256:b7bd8e9105f199eccb7aac571f24a33f4738cdfc365a7e4b980ccb542b4d8c7a
```

### `dpkg` source package: `vim=2:9.0.1378-1`

Binary Packages:

- `vim-common=2:9.0.1378-1`
- `vim-tiny=2:9.0.1378-1`

Licenses: (parsed from: `/usr/share/doc/vim-common/copyright`, `/usr/share/doc/vim-tiny/copyright`)

- `Apache`
- `Apache-2.0`
- `Artistic`
- `Artistic-1`
- `BSD-2-clause`
- `BSD-3-clause`
- `Compaq`
- `EDL-1`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `OPL-1+`
- `UC`
- `Vim`
- `Vim-Regexp`
- `X11`
- `XPM`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris vim=2:9.0.1378-1
'http://http.debian.net/debian/pool/main/v/vim/vim_9.0.1378-1.dsc' vim_9.0.1378-1.dsc 3177 SHA256:22f5912861dfb5beac051494576d01a4ef08b6be6413f122710a9172d91f308c
'http://http.debian.net/debian/pool/main/v/vim/vim_9.0.1378.orig.tar.xz' vim_9.0.1378.orig.tar.xz 11109404 SHA256:6f20c108c0fe5dbcb00a00080b3607feb024a499de2c4d004de9c3bd74516523
'http://http.debian.net/debian/pool/main/v/vim/vim_9.0.1378-1.debian.tar.xz' vim_9.0.1378-1.debian.tar.xz 180200 SHA256:81cd659c6e2a960a068cea189d1242fb7155fdd318ea79de3aca4ce45e41ca8e
```

### `dpkg` source package: `wget=1.21.3-1`

Binary Packages:

- `wget=1.21.3-1+b2`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.21.3-1
'http://http.debian.net/debian/pool/main/w/wget/wget_1.21.3-1.dsc' wget_1.21.3-1.dsc 2167 SHA256:e294772dac85a4d59fa64269515aa4a93664789f1f4612cfe309785384fd1f55
'http://http.debian.net/debian/pool/main/w/wget/wget_1.21.3.orig.tar.gz' wget_1.21.3.orig.tar.gz 5079864 SHA256:5726bb8bc5ca0f6dc7110f6416e4bb7019e2d2ff5bf93d1ca2ffcc6656f220e5
'http://http.debian.net/debian/pool/main/w/wget/wget_1.21.3.orig.tar.gz.asc' wget_1.21.3.orig.tar.gz.asc 854 SHA256:a4d96f04bc5a034310eae177df9adc79ef7a6f0fad7bf7669bf0ac318fa22ccd
'http://http.debian.net/debian/pool/main/w/wget/wget_1.21.3-1.debian.tar.xz' wget_1.21.3-1.debian.tar.xz 60660 SHA256:30901c12ded6e455d55fe73c40245b51d2fd53e20e30713a10e066fdfadb9d20
```

### `dpkg` source package: `xauth=1:1.1.2-1`

Binary Packages:

- `xauth=1:1.1.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xauth=1:1.1.2-1
'http://http.debian.net/debian/pool/main/x/xauth/xauth_1.1.2-1.dsc' xauth_1.1.2-1.dsc 1840 SHA256:5b6f718530b68c385368bae7267e7dd0044882290e7b3e4fbe6d63bb8d65c9f0
'http://http.debian.net/debian/pool/main/x/xauth/xauth_1.1.2.orig.tar.gz' xauth_1.1.2.orig.tar.gz 214621 SHA256:84d27a1023d8da524c134f424b312e53cb96e08871f96868aa20316bfcbbc054
'http://http.debian.net/debian/pool/main/x/xauth/xauth_1.1.2-1.diff.gz' xauth_1.1.2-1.diff.gz 18091 SHA256:6afd6f9a3c9b6320e4b523bbe6e5ff3960d59310c9b0efc8b6496d39144710ed
```

### `dpkg` source package: `xdg-utils=1.1.3-4.1`

Binary Packages:

- `xdg-utils=1.1.3-4.1`

Licenses: (parsed from: `/usr/share/doc/xdg-utils/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris xdg-utils=1.1.3-4.1
'http://http.debian.net/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3-4.1.dsc' xdg-utils_1.1.3-4.1.dsc 1756 SHA256:c54ae65034c4c3e9f2208a44990111d34fc5ed1e689efd3907a2a8e5e965ccac
'http://http.debian.net/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3.orig.tar.gz' xdg-utils_1.1.3.orig.tar.gz 297170 SHA256:d798b08af8a8e2063ddde6c9fa3398ca81484f27dec642c5627ffcaa0d4051d9
'http://http.debian.net/debian/pool/main/x/xdg-utils/xdg-utils_1.1.3-4.1.debian.tar.xz' xdg-utils_1.1.3-4.1.debian.tar.xz 15660 SHA256:0ea0b550719ab75f9a0fe58ed907673c5bcfc2bd87537845534694c502740aed
```

### `dpkg` source package: `xft=2.3.6-1`

Binary Packages:

- `libxft2:amd64=2.3.6-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris xft=2.3.6-1
'http://http.debian.net/debian/pool/main/x/xft/xft_2.3.6-1.dsc' xft_2.3.6-1.dsc 2006 SHA256:252220495bd12fac30d8f1b1994916beaed9c5149138dcc62e230fee17339530
'http://http.debian.net/debian/pool/main/x/xft/xft_2.3.6.orig.tar.gz' xft_2.3.6.orig.tar.gz 447498 SHA256:b7e59f69e0bbabe9438088775f7e5a7c16a572e58b11f9722519385d38192df5
'http://http.debian.net/debian/pool/main/x/xft/xft_2.3.6-1.diff.gz' xft_2.3.6-1.diff.gz 17995 SHA256:9d4c64fc52626134a3f753df88fceaba0cb460bd9b56544f0e42178deca77019
```

### `dpkg` source package: `xorg=1:7.7+23`

Binary Packages:

- `x11-common=1:7.7+23`

Licenses: (parsed from: `/usr/share/doc/x11-common/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris xorg=1:7.7+23
'http://http.debian.net/debian/pool/main/x/xorg/xorg_7.7%2b23.dsc' xorg_7.7+23.dsc 1975 SHA256:b06ef48b56736e0a0a48bcbc1afd2cf6dcd70959c2b52e195456a0392076469c
'http://http.debian.net/debian/pool/main/x/xorg/xorg_7.7%2b23.tar.gz' xorg_7.7+23.tar.gz 287306 SHA256:8458b8798d7d6098cd5259abc447d6c7a371e20e641cac82cf635296a71f468e
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
'http://http.debian.net/debian/pool/main/x/xxhash/xxhash_0.8.1-1.dsc' xxhash_0.8.1-1.dsc 1966 SHA256:4a961627c06efc8fa3bc4b06ee9dba6cfaf092f2550b88d63e9218a2728721b4
'http://http.debian.net/debian/pool/main/x/xxhash/xxhash_0.8.1.orig.tar.gz' xxhash_0.8.1.orig.tar.gz 171552 SHA256:3bb6b7d6f30c591dd65aaaff1c8b7a5b94d81687998ca9400082c739a690436c
'http://http.debian.net/debian/pool/main/x/xxhash/xxhash_0.8.1-1.debian.tar.xz' xxhash_0.8.1-1.debian.tar.xz 4572 SHA256:d40aa223e90b85435082857b64573541ba9a995841717496e8975aed97241550
```

### `dpkg` source package: `xz-utils=5.4.1-0.2`

Binary Packages:

- `liblzma-dev:amd64=5.4.1-0.2`
- `liblzma5:amd64=5.4.1-0.2`
- `xz-utils=5.4.1-0.2`

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
$ apt-get source -qq --print-uris xz-utils=5.4.1-0.2
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.dsc' xz-utils_5.4.1-0.2.dsc 2621 SHA256:faaef4551ecc9547f308ca65cdafe6d2fa43b06f11944001490079303c87bf40
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz' xz-utils_5.4.1.orig.tar.xz 1485272 SHA256:5d9827aa1875b21c288f78864bb26d2650b436ea8d2cad364e4921eb6266a5a5
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.4.1.orig.tar.xz.asc' xz-utils_5.4.1.orig.tar.xz.asc 833 SHA256:4b0c7707114996092a5f75a98333de2102db83a27218e4903b8fb7c24a8d0233
'http://http.debian.net/debian/pool/main/x/xz-utils/xz-utils_5.4.1-0.2.debian.tar.xz' xz-utils_5.4.1-0.2.debian.tar.xz 87432 SHA256:67eeab55ab3e4b35722d4ec255e0f735b3c61aab0437ab3c8274f5aa77c9c407
```

### `dpkg` source package: `zip=3.0-13`

Binary Packages:

- `zip=3.0-13`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris zip=3.0-13
'http://http.debian.net/debian/pool/main/z/zip/zip_3.0-13.dsc' zip_3.0-13.dsc 1336 SHA256:9fad1b5bda0c38a6811494159953a19dc42b9022b29b73ba51f30d2bb48445e6
'http://http.debian.net/debian/pool/main/z/zip/zip_3.0.orig.tar.gz' zip_3.0.orig.tar.gz 1118845 SHA256:f0e8bb1f9b7eb0b01285495a2699df3a4b766784c1765a8f1aeedf63c0806369
'http://http.debian.net/debian/pool/main/z/zip/zip_3.0-13.debian.tar.xz' zip_3.0-13.debian.tar.xz 8688 SHA256:4f5aca2d9f6021d2fd73f2fc16e9a392ab98673a940b44cf78fe38b8cdec1ab9
```

### `dpkg` source package: `zlib=1:1.2.13.dfsg-1`

Binary Packages:

- `zlib1g:amd64=1:1.2.13.dfsg-1`
- `zlib1g-dev:amd64=1:1.2.13.dfsg-1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.13.dfsg-1
'http://http.debian.net/debian/pool/main/z/zlib/zlib_1.2.13.dfsg-1.dsc' zlib_1.2.13.dfsg-1.dsc 2399 SHA256:3fa1e6b2fc525062aa88207dda52fed8e045373c809d362fe8a2bfbf7cf515a8
'http://http.debian.net/debian/pool/main/z/zlib/zlib_1.2.13.dfsg.orig.tar.bz2' zlib_1.2.13.dfsg.orig.tar.bz2 1239825 SHA256:71feb7947e3c00ef125f83b79a4e529bde31171e5babe48b391f06758d1ab0a1
'http://http.debian.net/debian/pool/main/z/zlib/zlib_1.2.13.dfsg-1.debian.tar.xz' zlib_1.2.13.dfsg-1.debian.tar.xz 15700 SHA256:f66cf3d4f2d7defcd4d1fd1fb0a11ee39f1e01b42ec7d059c9dc5c1695133c44
```
