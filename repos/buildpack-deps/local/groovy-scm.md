# `buildpack-deps:groovy-scm`

## Docker Metadata

- Image ID: `sha256:f0150255a080b938ca092c70e0c1bf7b88b6c7dd3befeeb004d24f26cd0746b0`
- Created: `2020-07-06T23:21:12.618297745Z`
- Virtual Size: ~ 279.91 Mb  
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
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-8.dsc' acl_2.2.53-8.dsc 2464 SHA256:63623506d567cc90c9491aba7e40d480034a21f2d38b0c626f610ef637753a2c
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-8.debian.tar.xz' acl_2.2.53-8.debian.tar.xz 25300 SHA256:f8cfc2ce609f0fa19450cc4cb87aa98c48486231e80f04680b76072c05972e23
```

### `dpkg` source package: `adduser=3.118ubuntu2`

Binary Packages:

- `adduser=3.118ubuntu2`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.118ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.dsc' adduser_3.118ubuntu2.dsc 1131 SHA256:785f99d8c75c972cd42d3fab3afa07f97299bb1d70013fe5d295f045224774bb
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.tar.xz' adduser_3.118ubuntu2.tar.xz 222364 SHA256:9429124c39c381b541005da6f0ae29831bd6533dd65c923e06ca2a7c310db382
```

### `dpkg` source package: `apr-util=1.6.1-4ubuntu2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.dsc' apr-util_1.6.1-4ubuntu2.dsc 2686 SHA256:bf8be458f58a6b1576d35bc78647bb0e990fc0d0c47ee7b51a5e2ecf3d378aac
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.debian.tar.xz' apr-util_1.6.1-4ubuntu2.debian.tar.xz 213052 SHA256:2293c33f2e8d354aae7285e6037820d32305dcf4843093123c0683946ae35967
```

### `dpkg` source package: `apr=1.6.5-1ubuntu1`

Binary Packages:

- `libapr1:amd64=1.6.5-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.5-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.dsc' apr_1.6.5-1ubuntu1.dsc 2390 SHA256:9e9d5b1be5c9d17c4720d43096064da70a4cba1593f10c272328e16f8ed4c656
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2' apr_1.6.5.orig.tar.bz2 855393 SHA256:a67ca9fcf9c4ff59bce7f428a323c8b5e18667fdea7b0ebad47d194371b0a105
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2.asc' apr_1.6.5.orig.tar.bz2.asc 801 SHA256:9beff0bb06f4cbbb006176af93258d946d33b7fb54aac13a4c90cfba1cfd0c88
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.debian.tar.xz' apr_1.6.5-1ubuntu1.debian.tar.xz 213596 SHA256:faca1bccb281c7d91bf0846ee908dd0be53b4482c0a1850e03397307682717d1
```

### `dpkg` source package: `apt=2.1.6`

Binary Packages:

- `apt=2.1.6`
- `libapt-pkg6.0:amd64=2.1.6`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/apt/2.1.6/


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
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.dsc' attr_2.4.48-5.dsc 2433 SHA256:0b20a285b758083e2e202ffdd2930cef1bf84fee498791fc3e26b69a3bced01d
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.debian.tar.xz' attr_2.4.48-5.debian.tar.xz 25560 SHA256:02238253d324250dabdc0434f7de045d85df93458995a465ac434f2a3978a312
```

### `dpkg` source package: `audit=1:2.8.5-2ubuntu6`

Binary Packages:

- `libaudit-common=1:2.8.5-2ubuntu6`
- `libaudit1:amd64=1:2.8.5-2ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.5-2ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-2ubuntu6.dsc' audit_2.8.5-2ubuntu6.dsc 2764 SHA256:b149fad8217d68a80299c1ef72539ee7d756146d692b7e51eade7341e60ac528
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5.orig.tar.gz' audit_2.8.5.orig.tar.gz 1140694 SHA256:0e5d4103646e00f8d1981e1cd2faea7a2ae28e854c31a803e907a383c5e2ecb7
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-2ubuntu6.debian.tar.xz' audit_2.8.5-2ubuntu6.debian.tar.xz 18712 SHA256:d85ecf206bfe256a86e6d39602cd2744beda264a28e413f31c4da227e6542ea7
```

### `dpkg` source package: `base-files=11ubuntu7`

Binary Packages:

- `base-files=11ubuntu7`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `base-passwd=3.5.47`

Binary Packages:

- `base-passwd=3.5.47`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.47
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.dsc' base-passwd_3.5.47.dsc 1757 SHA256:5a77a4cce51d1eb72e9d96d4083c641435c05888922c7bd3fa6b4395bf9afad3
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.tar.xz' base-passwd_3.5.47.tar.xz 53024 SHA256:9810ae0216e96bf9fc7ca6163d47ef8ec7d1677f533451af5911d8202a490a23
```

### `dpkg` source package: `bash=5.0-6ubuntu2`

Binary Packages:

- `bash=5.0-6ubuntu2`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.0-6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu2.dsc' bash_5.0-6ubuntu2.dsc 2435 SHA256:711f1c8c971f993d91a1bde5b45dfe35309369792f9cfaa8be66cbe4e73f7a43
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA256:893858ba233d65bda38039e99dd96a4102b2f6a2d5e6c1c546e0794a60beed97
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu2.debian.tar.xz' bash_5.0-6ubuntu2.debian.tar.xz 74404 SHA256:bd139386937f508dbce82ac58f11e3aa1db25fe795223b3810d2d1005306a335
```

### `dpkg` source package: `breezy=3.0.2-4ubuntu2`

Binary Packages:

- `brz=3.0.2-4ubuntu2`
- `python3-breezy=3.0.2-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/brz/copyright`, `/usr/share/doc/python3-breezy/copyright`)

- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris breezy=3.0.2-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.0.2-4ubuntu2.dsc' breezy_3.0.2-4ubuntu2.dsc 2793 SHA256:387fbd45cbe97d4d0685cba418d213bf5b4023ab4b10039390c2f11b2f9871f5
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.0.2.orig.tar.gz' breezy_3.0.2.orig.tar.gz 15271219 SHA256:50f16bc7faf299f98fe58573da55b0664078f94b1a0e7f0ce9e1e6a0d47e68e0
'http://archive.ubuntu.com/ubuntu/pool/universe/b/breezy/breezy_3.0.2-4ubuntu2.debian.tar.xz' breezy_3.0.2-4ubuntu2.debian.tar.xz 64032 SHA256:6ad61cb9ba7b452882e2fe19e24e99ba9b4fcbaa087af9ea058e9a5c4a9260c1
```

### `dpkg` source package: `brotli=1.0.7-6.1`

Binary Packages:

- `libbrotli1:amd64=1.0.7-6.1`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.7-6.1
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-6.1.dsc' brotli_1.0.7-6.1.dsc 2300 SHA256:c67ed3b56c0fd15f4b2e407aa775305f35c609349f40a5159e049e132981a946
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7.orig.tar.gz' brotli_1.0.7.orig.tar.gz 23827908 SHA256:4c61bfb0faca87219ea587326c467b95acb25555b53d1a421ffa3c8a9296ee2c
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-6.1.debian.tar.xz' brotli_1.0.7-6.1.debian.tar.xz 4460 SHA256:4a1a47922f8c92d7cd98bfd7ff3597247f808a14c5b792500413e6ba68f4d6d0
```

### `dpkg` source package: `bzip2=1.0.8-3ubuntu1`

Binary Packages:

- `bzip2=1.0.8-3ubuntu1`
- `libbz2-1.0:amd64=1.0.8-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-3ubuntu1.dsc' bzip2_1.0.8-3ubuntu1.dsc 2287 SHA256:8ac30099f0c9e8d1273b03fcb2853cb0da66da34a5007e3e388e9d15521e5900
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-3ubuntu1.debian.tar.bz2' bzip2_1.0.8-3ubuntu1.debian.tar.bz2 26439 SHA256:414f018a27324fcba194c37b2eb503ab8ca5ee7d4177356f05f259a57706b708
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
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622+brz.dsc' bzr_2.7.0+bzr6622+brz.dsc 1866 SHA256:2c1d9f13818b32fbc5dc41d395b91101e2d1b451eae358ffdf83421521dbe670
'http://archive.ubuntu.com/ubuntu/pool/universe/b/bzr/bzr_2.7.0+bzr6622+brz.tar.xz' bzr_2.7.0+bzr6622+brz.tar.xz 18052 SHA256:d847a018e4869b59e9bfc04b0ff3705dcbb5479a8b6796c2dd68e60be3753a42
```

### `dpkg` source package: `ca-certificates=20190110ubuntu2`

Binary Packages:

- `ca-certificates=20190110ubuntu2`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110ubuntu2.dsc' ca-certificates_20190110ubuntu2.dsc 1913 SHA256:a71b08c22dad0ab19f890aac01ac3ecd210cf699c110e0c652e71d26f782597e
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110ubuntu2.tar.xz' ca-certificates_20190110ubuntu2.tar.xz 243628 SHA256:2ce310b6d94775568c38072b824ee9ee647434304994f984961f60231f747f80
```

### `dpkg` source package: `cdebconf=0.252ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.252ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.252ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.252ubuntu1.dsc' cdebconf_0.252ubuntu1.dsc 2865 SHA256:4e851f7f8f6201fdbfe4257ef0b7302fa36b7a89e5b0f209905b92473adce261
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.252ubuntu1.tar.xz' cdebconf_0.252ubuntu1.tar.xz 276852 SHA256:852f565190ad2cc902f041d6eaf587ea8a100f1facebb004b13b0043a2590e7a
```

### `dpkg` source package: `configobj=5.0.6-4`

Binary Packages:

- `python3-configobj=5.0.6-4`

Licenses: (parsed from: `/usr/share/doc/python3-configobj/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris configobj=5.0.6-4
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-4.dsc' configobj_5.0.6-4.dsc 2246 SHA256:74df72d8fdb3c20e4bc5ab996bf1f8c6297811643989110cc27a019e7beb0429
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6.orig.tar.gz' configobj_5.0.6.orig.tar.gz 143664 SHA256:2e140354efcca6f558ff9ee941b435ae09a617bc071797bef62c8d6ed2033d5e
'http://archive.ubuntu.com/ubuntu/pool/main/c/configobj/configobj_5.0.6-4.debian.tar.xz' configobj_5.0.6-4.debian.tar.xz 6916 SHA256:dd20992aeef0eb1fb8ab6f0007e265ece33cfc20a6ca18b380eb255674195f01
```

### `dpkg` source package: `coreutils=8.30-3ubuntu2`

Binary Packages:

- `coreutils=8.30-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `curl=7.68.0-1ubuntu2`

Binary Packages:

- `curl=7.68.0-1ubuntu2`
- `libcurl3-gnutls:amd64=7.68.0-1ubuntu2`
- `libcurl4:amd64=7.68.0-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/curl/copyright`, `/usr/share/doc/libcurl3-gnutls/copyright`, `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.68.0-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu2.dsc' curl_7.68.0-1ubuntu2.dsc 2071 SHA256:d44259b40997d294a0cf3c04afd1a4151069f547851d7ce69dc4ef795cd07b66
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0.orig.tar.gz' curl_7.68.0.orig.tar.gz 4096350 SHA256:1dd7604e418b0b9a9077f62f763f6684c1b092a7bc17e3f354b8ad5c964d7358
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu2.debian.tar.xz' curl_7.68.0-1ubuntu2.debian.tar.xz 31648 SHA256:cc451b58c0ffdba9374826dc6d8a66864e9739646021855d80c2488c8298e527
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.dsc' cyrus-sasl2_2.1.27+dfsg-2.dsc 3393 SHA256:e7e09491a1c2589c9947164db091d0f9b21b7d122f128841b6eac1adfc51b6c2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz 99956 SHA256:ee894aeee645e842e39b434d5130e1bd15ea24b84c8eeeea3f5077511a87341a
```

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
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-7.dsc' dash_0.5.10.2-7.dsc 1762 SHA256:477515a7d980127657c9760f1a53b0175b79455acfd9d92284a6c563971523ea
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA256:3c663919dc5c66ec991da14c7cf7e0be8ad00f3db73986a987c118862b5f6071
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-7.debian.tar.xz' dash_0.5.10.2-7.debian.tar.xz 45336 SHA256:ba76b70008e95a88f1f2860bc74bea9fd6732df179dbb126706d51cfede713c1
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6ubuntu2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu2.dsc' db5.3_5.3.28+dfsg1-0.6ubuntu2.dsc 3245 SHA256:d879f4921a2f573132031d9371f0eb020005bdce48d6e12b436bf3515dda8663
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu2.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6ubuntu2.debian.tar.xz 30172 SHA256:e606e7827f077efc92afc6f0d43c921fab4577d619eab06fab23182aefab7506
```

### `dpkg` source package: `debconf=1.5.74`

Binary Packages:

- `debconf=1.5.74`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.74
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.dsc' debconf_1.5.74.dsc 2082 SHA256:7576b8798165e30aaea23bad812eec729dd091a1ca59063328e7f68223b79af1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.74.tar.xz' debconf_1.5.74.tar.xz 571108 SHA256:11b3fa02ddafe813c301aa150fef4d510d77afa64cbfe09c7e614995147c48e0
```

### `dpkg` source package: `debianutils=4.11`

Binary Packages:

- `debianutils=4.11`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.11
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.11.dsc' debianutils_4.11.dsc 1611 SHA256:cd808c7c4fe7b7e096c912197bcbae95767fb24c7f22b0484d4a3747b1840ad2
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.11.tar.xz' debianutils_4.11.tar.xz 157440 SHA256:bb5ce6290696b0d623377521ed217f484aa98f7346c5f7c48f9ae3e1acfb7151
```

### `dpkg` source package: `diffutils=1:3.7-3`

Binary Packages:

- `diffutils=1:3.7-3`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/diffutils/1:3.7-3/


### `dpkg` source package: `dpkg=1.19.7ubuntu4`

Binary Packages:

- `dpkg=1.19.7ubuntu4`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.7ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.7ubuntu4.dsc' dpkg_1.19.7ubuntu4.dsc 2250 SHA256:6365d7768eb8966b46d35933999ee23f7128ec057c21ca107fdccb0c0ec7b720
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.7ubuntu4.tar.xz' dpkg_1.19.7ubuntu4.tar.xz 4743704 SHA256:1714efd82c143f463f43d1e1a0cffcc009e0cb3001cf725209f74bd642b76a27
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
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15-1build1.dsc' dulwich_0.19.15-1build1.dsc 2410 SHA256:5a742485cfbf473aeefab144351af69662ab867ab016e5c3541aad6efddfa00c
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15.orig.tar.gz' dulwich_0.19.15.orig.tar.gz 369491 SHA256:805a9b1932dc28b91f359f529c2e46b7623aec3ab719c96d3f2fc63d0d8d8411
'http://archive.ubuntu.com/ubuntu/pool/universe/d/dulwich/dulwich_0.19.15-1build1.debian.tar.xz' dulwich_0.19.15-1build1.debian.tar.xz 631088 SHA256:6fddcf432f17d8512cafbc8f7bac2e94f54bd7843a820af64e0fe010413e8a5f
```

### `dpkg` source package: `e2fsprogs=1.45.6-1ubuntu1`

Binary Packages:

- `e2fsprogs=1.45.6-1ubuntu1`
- `libcom-err2:amd64=1.45.6-1ubuntu1`
- `libext2fs2:amd64=1.45.6-1ubuntu1`
- `libss2:amd64=1.45.6-1ubuntu1`
- `logsave=1.45.6-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.6-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.dsc' e2fsprogs_1.45.6-1ubuntu1.dsc 3328 SHA256:1a4832b1d2bd4a17121bd89fa51ba192e17ad7153da9d16a475fad5b3fa2bf66
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz' e2fsprogs_1.45.6.orig.tar.gz 7938544 SHA256:5f64ac50a2b60b8e67c5b382bb137dec39344017103caffc3a61554424f2d693
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6.orig.tar.gz.asc' e2fsprogs_1.45.6.orig.tar.gz.asc 488 SHA256:831c29bd04c5b21faf2aa2d5fa3b409148973e3ef0d15f67315a5c429180d945
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz' e2fsprogs_1.45.6-1ubuntu1.debian.tar.xz 81276 SHA256:dacb658bcf1b0f7728ddc7f956494d6d414b70e97d45b22c91df24fec01248cc
```

### `dpkg` source package: `expat=2.2.9-1build1`

Binary Packages:

- `libexpat1:amd64=2.2.9-1build1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.9-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.dsc' expat_2.2.9-1build1.dsc 1998 SHA256:9f2d2e3bf2aec22907e3bf818fac7acc5f1e917821907bdea016f69a5cfe4da0
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9.orig.tar.gz' expat_2.2.9.orig.tar.gz 8273174 SHA256:c341ac8c79e021cc3392a6d76e138e62d1dd287592cb455148540331756a2208
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.debian.tar.xz' expat_2.2.9-1build1.debian.tar.xz 10780 SHA256:400872937adfb41255914391a172237cfe317e57f129562ff2ec66773b2b5bbf
```

### `dpkg` source package: `findutils=4.7.0-1ubuntu1`

Binary Packages:

- `findutils=4.7.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.7.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu1.dsc' findutils_4.7.0-1ubuntu1.dsc 2446 SHA256:3d157948919082e66cb74e0f927efa3dd240d9fa9814973874d0fa77f3023ead
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz' findutils_4.7.0.orig.tar.xz 1895048 SHA256:c5fefbdf9858f7e4feb86f036e1247a54c79fc2d8e4b7064d5aaa1f47dfa789a
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz.asc' findutils_4.7.0.orig.tar.xz.asc 488 SHA256:2f620e6d941e241fac52344a89149ab1ffeefb0fb9e42174e17a508d59a31d0f
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu1.debian.tar.xz' findutils_4.7.0-1ubuntu1.debian.tar.xz 27700 SHA256:dfb2329fd141384c2d76409c2e99f164cc25954115529245d80d5d41e3167731
```

### `dpkg` source package: `gcc-10=10.1.0-3ubuntu1`

Binary Packages:

- `gcc-10-base:amd64=10.1.0-3ubuntu1`
- `libgcc-s1:amd64=10.1.0-3ubuntu1`
- `libstdc++6:amd64=10.1.0-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libstdc++6/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10.1.0-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10.1.0-3ubuntu1.dsc' gcc-10_10.1.0-3ubuntu1.dsc 30426 SHA256:482d3fc83400e12fa50ed68ef3d2e0881eb8b2fbfcd4dafccf497b34d7f0bad4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10.1.0.orig.tar.gz' gcc-10_10.1.0.orig.tar.gz 94357676 SHA256:639726222b60ce144063e2b166057fccda523064839381025130f7128f7b9b66
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10.1.0-3ubuntu1.debian.tar.xz' gcc-10_10.1.0-3ubuntu1.debian.tar.xz 2269564 SHA256:cae6ce2ba708b00f372f446bf21522c147ce361579a4284e1a0787ada3c97931
```

### `dpkg` source package: `gdbm=1.18.1-5`

Binary Packages:

- `libgdbm-compat4:amd64=1.18.1-5`
- `libgdbm6:amd64=1.18.1-5`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.18.1-5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.dsc' gdbm_1.18.1-5.dsc 2635 SHA256:4c0c4498378c673c9d2d8dfb5b319a4830d2dd21e65faaaa8e0f09cb7f71606b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz' gdbm_1.18.1.orig.tar.gz 941863 SHA256:86e613527e5dba544e73208f42b78b7c022d4fa5a6d5498bf18c8d6f745b91dc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz.asc' gdbm_1.18.1.orig.tar.gz.asc 412 SHA256:3254738e7689e44ac65e78a766806828b8282e6bb1c0e5bb6156a99e567889a5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.debian.tar.xz' gdbm_1.18.1-5.debian.tar.xz 16348 SHA256:3c1a0e05b40a97ee51ce77c736c72c37738ba31b2720111d3bc99175a2c3a3ed
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0-1ubuntu1.dsc' git_2.27.0-1ubuntu1.dsc 2991 SHA256:fcd999d6ed543017ec0b9858e35e93900cf30dc13bc09138512dfb776c0eb18b
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0.orig.tar.xz' git_2.27.0.orig.tar.xz 6074636 SHA256:73ca9774d7fa226e1d87c1909401623f96dca6a044e583b9a762e84d7d1a73f9
'http://archive.ubuntu.com/ubuntu/pool/main/g/git/git_2.27.0-1ubuntu1.debian.tar.xz' git_2.27.0-1ubuntu1.debian.tar.xz 652712 SHA256:7fd6f399e6c8826874515eadccdd88c21bf1a9951fbc92a4f347f1f3c41be11a
```

### `dpkg` source package: `glibc=2.31-0ubuntu10`

Binary Packages:

- `libc-bin=2.31-0ubuntu10`
- `libc6:amd64=2.31-0ubuntu10`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc6/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.31-0ubuntu10
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu10.dsc' glibc_2.31-0ubuntu10.dsc 9309 SHA256:e96042f2807662ddf9288334ea0a3eddc874e46af25018cc5bbc3d29fd7b6cec
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31.orig.tar.xz' glibc_2.31.orig.tar.xz 17317924 SHA256:2b22c7b04a36747d6c74796a73193a6f8856bfd1efc551b5db96baefa053fe5e
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu10.debian.tar.xz' glibc_2.31-0ubuntu10.debian.tar.xz 859544 SHA256:74db110b2e22a9e64200f2c453b288298eadb7d86e098cb35cb96138d3746e50
```

### `dpkg` source package: `gmp=2:6.2.0+dfsg-6`

Binary Packages:

- `libgmp10:amd64=2:6.2.0+dfsg-6`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.0+dfsg-6
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6.dsc' gmp_6.2.0+dfsg-6.dsc 2144 SHA256:8ca73e96ab6d3d05d21a76b357fdc36959be9c5c863186fd30ee17981c4f2c93
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg.orig.tar.xz' gmp_6.2.0+dfsg.orig.tar.xz 1842912 SHA256:5d7610449498a79aa62d4b9a8f6baaef91b8716726e1009e02b879962dff32ab
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-6.debian.tar.xz' gmp_6.2.0+dfsg-6.debian.tar.xz 21220 SHA256:bb447179d6bd323e2a37035a8ebab58722f1e5c74abb1043b8b9ad038ce4f9fe
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu1.dsc' gnupg2_2.2.20-1ubuntu1.dsc 3971 SHA256:f864b21a847e820057a504fa067f4154ecf47487c8cea08bec1646460d7ea9e7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2' gnupg2_2.2.20.orig.tar.bz2 6786913 SHA256:04a7c9d48b74c399168ee8270e548588ddbe52218c337703d7f06373d326ca30
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20.orig.tar.bz2.asc' gnupg2_2.2.20.orig.tar.bz2.asc 1357 SHA256:be34b9959fa4c9baa7269b1c7c695808d6b999ba47f28c614312dd3d8d47ca79
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.20-1ubuntu1.debian.tar.xz' gnupg2_2.2.20-1ubuntu1.debian.tar.xz 64332 SHA256:2232fdbe9b2a4a55613a6b33d4bc8a8959474fbb675dae137c7e4f192cf941de
```

### `dpkg` source package: `gnutls28=3.6.13-4ubuntu2`

Binary Packages:

- `libgnutls30:amd64=3.6.13-4ubuntu2`

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
$ apt-get source -qq --print-uris gnutls28=3.6.13-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13-4ubuntu2.dsc' gnutls28_3.6.13-4ubuntu2.dsc 3586 SHA256:4789b5c40031d5f463dfcbd50776375683c65903cba1bde8b58b385d2c91f32c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13.orig.tar.xz' gnutls28_3.6.13.orig.tar.xz 5958956 SHA256:32041df447d9f4644570cf573c9f60358e865637d69b7e59d1159b7240b52f38
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13.orig.tar.xz.asc' gnutls28_3.6.13.orig.tar.xz.asc 667 SHA256:79eb677b19a35de2f17d2ea87e863755cd53f0072b9435c8a4b57669360f57d0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13-4ubuntu2.debian.tar.xz' gnutls28_3.6.13-4ubuntu2.debian.tar.xz 69656 SHA256:7f7cd3b8b2155527da008a57336d978c316a35ca62aa2019dd27ae27a3a9aa7e
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.dsc' grep_3.4-1.dsc 1674 SHA256:785f527cede9631f075bdd6c7f35e65e6b82897d009682766cf35839a393277d
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz' grep_3.4.orig.tar.xz 1555820 SHA256:58e6751c41a7c25bfc6e9363a41786cff3ba5709cf11d5ad903cf7cce31cc3fb
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz.asc' grep_3.4.orig.tar.xz.asc 833 SHA256:4c1871ff6b79c5e5ce0a192272c171d06ec20762b4b258688b1ca2e47d94b23e
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.debian.tar.xz' grep_3.4-1.debian.tar.xz 104364 SHA256:582d181804ce72fcfc4c6a9f13ea1dd73ad04c2723b5da346b69ee5cd24a7d08
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
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-2ubuntu1.dsc' gzip_1.10-2ubuntu1.dsc 2074 SHA256:bdac8e876b858094311a611b4e69a179fc67a78158c5f59f53b8269bafb4e568
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA256:c91f74430bf7bc20402e1f657d0b252cb80aa66ba333a25704512af346633c68
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-2ubuntu1.debian.tar.xz' gzip_1.10-2ubuntu1.debian.tar.xz 33288 SHA256:23d03e6a7f9cf9b7daf506eaf922ccddda85dfc2827cf48da72d2086608872ef
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
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.dsc' heimdal_7.7.0+dfsg-2.dsc 3580 SHA256:cd71bc63686f11909d68bce45a9ea1c7ecb8f08b71eb2d39fc6906c4b7f406fb
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg.orig.tar.xz' heimdal_7.7.0+dfsg.orig.tar.xz 5945252 SHA256:6822c9547188b753b6325047fda9255744e4ebbbe02bb0dade78c261061fefac
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-2.debian.tar.xz' heimdal_7.7.0+dfsg-2.debian.tar.xz 128660 SHA256:076c9b6d91ce69f760ce8812d5737bdf03fc5b1fd2b1ac401f18fda4bbd31055
```

### `dpkg` source package: `hostname=3.23`

Binary Packages:

- `hostname=3.23`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.dsc' hostname_3.23.dsc 1402 SHA256:0694c083fad82da1fd33204557a30bfc745a689a64030ba360062daafe03ede0
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.tar.gz' hostname_3.23.tar.gz 13672 SHA256:bc6d1954b22849869ff8b2a602e39f08b1702f686d4b58dd7927cdeb5b4876ef
```

### `dpkg` source package: `init-system-helpers=1.57`

Binary Packages:

- `init-system-helpers=1.57`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/init-system-helpers/1.57/


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
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu1.dsc' keyutils_1.6.1-2ubuntu1.dsc 2191 SHA256:1ab35f3c660bbb1a67258769461300d7287f9f8a3715b00855ef6191b5cb28ae
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1.orig.tar.bz2' keyutils_1.6.1.orig.tar.bz2 97232 SHA256:c8b15722ae51d95b9ad76cc6d49a4c2cc19b0c60f72f61fb9bf43eea7cbd64ce
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.1-2ubuntu1.debian.tar.xz' keyutils_1.6.1-2ubuntu1.debian.tar.xz 14364 SHA256:d301104058e36c6ddfa403ad622d7226b7beee6fb7a1866ec0edb5d5339063ca
```

### `dpkg` source package: `krb5=1.17-10`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.17-10`
- `libk5crypto3:amd64=1.17-10`
- `libkrb5-3:amd64=1.17-10`
- `libkrb5support0:amd64=1.17-10`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-10
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-10.dsc' krb5_1.17-10.dsc 3187 SHA256:1ce061fc29b4c1d12c46c07d7a1fc2a16ed026ed5d7bd3e639483bdc27a2007f
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA256:5a6e2284a53de5702d3dc2be3b9339c963f9b5397d3fbbc53beb249380a781f5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-10.debian.tar.xz' krb5_1.17-10.debian.tar.xz 143852 SHA256:6d3cefcea2e4839cc3c5e518083048b8eae62a4bc707db05c1900c5bddafa7f5
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
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.dsc' libassuan_2.5.3-7.1.dsc 2627 SHA256:9e4cfaef54fee1b6c1fd32fdfe6fc90b2dde78755517ee0ff56859e69251fb07
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA256:91bcb0403866b4e7c4bc1cc52ed4c364a9b5414b3994f718c70303f7f765e702
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA256:53b16a6619a2690b4f22da645a1d0c14b5664825c87b165ca5bd0de32607888a
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7.1.debian.tar.xz' libassuan_2.5.3-7.1.debian.tar.xz 13952 SHA256:c6783e12dc1fb65681c083274f52cb3286da18dcf8a5b38a6de10143003e0681
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
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.dsc' libbsd_0.10.0-1.dsc 2197 SHA256:7c05e2c73658f64cbd4e1762b716cc7c4c1d68391191e82c7d266a351430edd6
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz' libbsd_0.10.0.orig.tar.xz 393576 SHA256:34b8adc726883d0e85b3118fa13605e179a62b31ba51f676136ecb2d0bc1a887
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz.asc' libbsd_0.10.0.orig.tar.xz.asc 833 SHA256:4362f6d811ffc06659ac5cf777d8d01157bedfc28720b41fb485afb0a5acc0c7
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.debian.tar.xz' libbsd_0.10.0-1.debian.tar.xz 16660 SHA256:4cf37d6d5b72702b31b07384612e07173e94e081feef71fec206f86ab38f2411
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
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.dsc' libcap-ng_0.7.9-2.2.dsc 2081 SHA256:d573ce59d83d2c117515e7c57dde1c990e9c5a34e0f53ac09f6b4d3e153e9aae
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.2.debian.tar.xz' libcap-ng_0.7.9-2.2.debian.tar.xz 6308 SHA256:6d7b5cfcf435fe996e5dc78770a9ab1ab614ced5bee56e3e0ba4e09d8c832a0a
```

### `dpkg` source package: `libcbor=0.6.0-0ubuntu2`

Binary Packages:

- `libcbor0.6:amd64=0.6.0-0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libcbor0.6/copyright`)

- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.6.0-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu2.dsc' libcbor_0.6.0-0ubuntu2.dsc 2115 SHA256:b6538faed9b0eaa9831fc636d35009c7f7313536969f2dabd1ae8cb1510705b8
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0.orig.tar.gz' libcbor_0.6.0.orig.tar.gz 262622 SHA256:ad97dfe6462a28956be38c924a5a557acf303d8454ca121e02150a5b87e03ee7
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu2.debian.tar.xz' libcbor_0.6.0-0ubuntu2.debian.tar.xz 5984 SHA256:33d07bee780a0277ffab8958170cf3a5f3f300edcf4b041aa0482ad67b3f1e94
```

### `dpkg` source package: `libedit=3.1-20191231-1`

Binary Packages:

- `libedit2:amd64=3.1-20191231-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.dsc' libedit_3.1-20191231-1.dsc 2129 SHA256:1be31eebf9cf3b38a9e7c3c4d4b37f002e3f89df48f00dec32506cbe9337ae38
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA256:dbb82cb7e116a5f8025d35ef5b4f7d4a3cdd0a3909a146a39112095a2d229071
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.debian.tar.xz' libedit_3.1-20191231-1.debian.tar.xz 14168 SHA256:f815baa1932f9df5d4cdb316a85ebd3cc91441c4d83ba2c8454f342573ed0eab
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
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.dsc' liberror-perl_0.17029-1.dsc 2336 SHA256:0590467fe8c5f81bff9336e991462b2a9994b4876f4b732c8b8b31e927987cd7
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029.orig.tar.gz' liberror-perl_0.17029.orig.tar.gz 33304 SHA256:1a23f7913032aed6d4b68321373a3899ca66590f4727391a091ec19c95bf7adc
'http://archive.ubuntu.com/ubuntu/pool/main/libe/liberror-perl/liberror-perl_0.17029-1.debian.tar.xz' liberror-perl_0.17029-1.debian.tar.xz 4552 SHA256:a753b142c4c33ebf9cc98ae5f7a08da13b7c9ca2823ec26e45c96efb9c15c42e
```

### `dpkg` source package: `libffi=3.3-4`

Binary Packages:

- `libffi7:amd64=3.3-4`

Licenses: (parsed from: `/usr/share/doc/libffi7/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.3-4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3-4.dsc' libffi_3.3-4.dsc 1932 SHA256:4190ad8e7ae9167a0c67c5926bc3705acb191745cca93ef845dbc06fc097f380
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3.orig.tar.gz' libffi_3.3.orig.tar.gz 1305466 SHA256:72fba7922703ddfa7a028d513ac15a85c8d54c8d67f55fa5a4802885dc652056
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3-4.debian.tar.xz' libffi_3.3-4.debian.tar.xz 9016 SHA256:0e8a6d9d87202d04d7646178479c3d365a845f9723da26625d533a169b378100
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
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0-2.dsc' libfido2_1.4.0-2.dsc 2565 SHA256:139d27a6b1079528282c1a320c94f071d5eb3bd62e25a05ef8bb4eb1a0cc7fcb
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0.orig.tar.gz' libfido2_1.4.0.orig.tar.gz 391439 SHA256:ad921fbe7d4bb70e4a971e564cd01f341daf9b5ed5d69b3cbab94a8a811d2a6c
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0.orig.tar.gz.asc' libfido2_1.4.0.orig.tar.gz.asc 488 SHA256:5d40de81c7e032be2d34ab87a8d4e1a2cc4f1f715449f65054a041249eb83fac
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.4.0-2.debian.tar.xz' libfido2_1.4.0-2.debian.tar.xz 73908 SHA256:75b7e7b87e44237c91735a63d93ffd0267cac27fd674395224b438529ed159b6
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
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu2.dsc' libgcrypt20_1.8.5-5ubuntu2.dsc 2907 SHA256:1b53962dd788843f0ca1c3c6e37874a737ba407d42a43f9a303c98d7d9fa92eb
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2' libgcrypt20_1.8.5.orig.tar.bz2 2991291 SHA256:3b4a2a94cb637eff5bdebbcaf46f4d95c4f25206f459809339cdada0eb577ac3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2.asc' libgcrypt20_1.8.5.orig.tar.bz2.asc 488 SHA256:4b24fda7847cd2b70ab19f4c38004a76bbdac46a1ddccff973ae88ba1296a22d
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu2.debian.tar.xz' libgcrypt20_1.8.5-5ubuntu2.debian.tar.xz 35444 SHA256:a173f29ed6637618340e5f89c4480ddfe90eac2bacdadc43b91a51fc96668982
```

### `dpkg` source package: `libgpg-error=1.38-1`

Binary Packages:

- `libgpg-error0:amd64=1.38-1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.38-1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-1.dsc' libgpg-error_1.38-1.dsc 2220 SHA256:51c7051e568dd16ece0513931b3f83a72f3d08db27681876ccca0d2c785af36a
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2' libgpg-error_1.38.orig.tar.bz2 957637 SHA256:d8988275aa69d7149f931c10442e9e34c0242674249e171592b430ff7b3afd02
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38.orig.tar.bz2.asc' libgpg-error_1.38.orig.tar.bz2.asc 488 SHA256:d80eb927d85e19e96d8de17552f8f48b517ae7acac7685404e8027475c5b4330
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.38-1.debian.tar.xz' libgpg-error_1.38-1.debian.tar.xz 17484 SHA256:01ce992462db6024439ead982746c837d219c5d8b3ba89ed691db649f372be31
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
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-1.dsc' libidn2_2.3.0-1.dsc 2411 SHA256:f4f61425610ae4b4c4d3c74431825fb4b4892d4d07e954d7acdf163595d33f14
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0.orig.tar.gz' libidn2_2.3.0.orig.tar.gz 2164993 SHA256:e1cb1db3d2e249a6a3eb6f0946777c2e892d5c5dc7bd91c74394fc3a01cab8b5
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.3.0-1.debian.tar.xz' libidn2_2.3.0-1.debian.tar.xz 10588 SHA256:a515029f13d12a48a6bc07dadc4cef6592db0a7257f48633795ae7128c23116c
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
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0-2.dsc' libksba_1.4.0-2.dsc 2470 SHA256:71333f487433f883ccff7211c9206804f23b25dbc38f401391f953333984165c
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0.orig.tar.bz2' libksba_1.4.0.orig.tar.bz2 651319 SHA256:bfe6a8e91ff0f54d8a329514db406667000cb207238eded49b599761bfca41b6
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0.orig.tar.bz2.asc' libksba_1.4.0.orig.tar.bz2.asc 488 SHA256:4f8e92ecd55bf3b7db6cec5f83d4721b75a9fcb43eb9b6bae2ed9a018951ca5e
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.4.0-2.debian.tar.xz' libksba_1.4.0-2.debian.tar.xz 10368 SHA256:8f49625bd327bb08975b65c08297cd9eea8591c1bcda98f5289fa5b4710ce0ad
```

### `dpkg` source package: `libpsl=0.21.0-1.1`

Binary Packages:

- `libpsl5:amd64=0.21.0-1.1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.1.dsc' libpsl_0.21.0-1.1.dsc 2228 SHA256:88e9ead32ef07fd807dd9b2eac7184baea346bd8b13878c9002b32e6286a4237
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA256:055aa87ec166c7afb985d0816c07ff440e1eb899881a318c51c69a0aeea8e279
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1.1.debian.tar.xz' libpsl_0.21.0-1.1.debian.tar.xz 12432 SHA256:aaf2dc28ed4b1b3d754895e3c21b0fb2be1f725fdec1f6d35a856cbe0b32cf46
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.dsc' libseccomp_2.4.3-1ubuntu3.dsc 2231 SHA256:a9a2b326dda99e2cf9e0262165a2c7ccba79a3adeb7e1d6305a692bf7c4b2290
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA256:cf15d1421997fac45b936515af61d209c4fd788af11005d212b3d0fd71e7991d
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.debian.tar.xz 33676 SHA256:f4219a23cb21642cd0a795334c43dad0759d1160c7854d0f0b78a6f49aa27625
```

### `dpkg` source package: `libselinux=3.0-1build2`

Binary Packages:

- `libselinux1:amd64=3.0-1build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.0-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0-1build2.dsc' libselinux_3.0-1build2.dsc 2565 SHA256:9a8d6c354ed06350606c009d899d117e71fda20887792b2c25b38222d0190d93
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0.orig.tar.gz' libselinux_3.0.orig.tar.gz 212096 SHA256:2ea2b30f671dae9d6b1391cbe8fb2ce5d36a3ee4fb1cd3c32f0d933c31b82433
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0-1build2.debian.tar.xz' libselinux_3.0-1build2.debian.tar.xz 23720 SHA256:ed85da0fe5561205c95f0f622562425dc7d8dd61ffd213a7fa914d778fe8da71
```

### `dpkg` source package: `libsemanage=3.0-1build2`

Binary Packages:

- `libsemanage-common=3.0-1build2`
- `libsemanage1:amd64=3.0-1build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.0-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.0-1build2.dsc' libsemanage_3.0-1build2.dsc 2678 SHA256:6231f4b00991657fafef2595eb571b2bcbe437de4ec9dc9929c0e69187db5f33
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.0.orig.tar.gz' libsemanage_3.0.orig.tar.gz 180745 SHA256:a497b0720d54eac427f1f3f618eed417e50ed8f4e47ed0f7a1d391bd416e84cf
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.0-1build2.debian.tar.xz' libsemanage_3.0-1build2.debian.tar.xz 17176 SHA256:38a646f91532c920c8c15a695c3585397ddbf032ecf49c52eb89d53c8eac48fb
```

### `dpkg` source package: `libsepol=3.0-1`

Binary Packages:

- `libsepol1:amd64=3.0-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0-1.dsc' libsepol_3.0-1.dsc 1770 SHA256:0073de5844605d380dd56f6630678ad91459496dc768fa9eb4d8cc7f693f5c1a
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0.orig.tar.gz' libsepol_3.0.orig.tar.gz 473864 SHA256:5b7ae1881909f1048b06f7a0c364c5c8a86ec12e0ec76e740fe9595a6033eb79
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0-1.debian.tar.xz' libsepol_3.0-1.debian.tar.xz 14224 SHA256:a16b5bc3c041e016d01794d1a1b9826ed4426862622c05526e93607c325ec328
```

### `dpkg` source package: `libssh=0.9.4-1ubuntu1`

Binary Packages:

- `libssh-4:amd64=0.9.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4-1ubuntu1.dsc' libssh_0.9.4-1ubuntu1.dsc 2038 SHA256:d0d422d98f84b654e7f686388c7a2d19798c1730dac2c20d5d63799c15c17437
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4.orig.tar.xz' libssh_0.9.4.orig.tar.xz 500776 SHA256:150897a569852ac05aac831dc417a7ba8e610c86ca2e0154a99c6ade2486226b
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4.orig.tar.xz.asc' libssh_0.9.4.orig.tar.xz.asc 833 SHA256:b637b8e4dae3109ae0b10ddfb35f9d5ce01049409c0b3572ee81292be30bccae
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.4-1ubuntu1.debian.tar.xz' libssh_0.9.4-1ubuntu1.debian.tar.xz 27792 SHA256:23b7bd156ccba4b0e68b3b5e9e78fd209bf0c809f7ce766e206764609f169f62
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
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.dsc' libtasn1-6_4.16.0-2.dsc 2586 SHA256:fd4a387c71f95c3eceb1072a3f42c7021d73128027ea41a18d6efc6cbfdd764a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz' libtasn1-6_4.16.0.orig.tar.gz 1812442 SHA256:0e0fb0903839117cb6e3b56e68222771bebf22ad7fc2295a0ed7d576e8d4329d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz.asc' libtasn1-6_4.16.0.orig.tar.gz.asc 488 SHA256:06c201e8c3b43c27465ed79294d4c4ec8dcd3e95e4a6176ecbf273229ee3e2d0
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.debian.tar.xz' libtasn1-6_4.16.0-2.debian.tar.xz 17740 SHA256:c1a89b0bac0fb7c83ebac4eafbca0475c24350ade6ccaef31266424725610624
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
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.dsc' libunistring_0.9.10-4.dsc 2212 SHA256:5c7940807b538d4204506349cbd67e5c677afb9f0e46e94455353e3f746a481e
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-4.debian.tar.xz' libunistring_0.9.10-4.debian.tar.xz 40936 SHA256:6c9554e1a1c6d0a02ca4868a5422d176e57a3131c1a8a21de5503b164997525c
```

### `dpkg` source package: `libxcrypt=1:4.4.16-1ubuntu1`

Binary Packages:

- `libcrypt1:amd64=1:4.4.16-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.16-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16-1ubuntu1.dsc' libxcrypt_4.4.16-1ubuntu1.dsc 2212 SHA256:2e030d707ba0c6aced4334a5338ce9a3e9523aaeb9a3884ae962fbad6a07d7b9
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16.orig.tar.xz' libxcrypt_4.4.16.orig.tar.xz 354788 SHA256:6a675b4ef1adde90b07ebc2f45eb9cd26702fbf87aa625d5aae9f68581d34fa6
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.16-1ubuntu1.debian.tar.xz' libxcrypt_4.4.16-1ubuntu1.debian.tar.xz 5840 SHA256:6bfd0591b366230b92550693a786b6fe42716e2b57eda7042fc8ec3d355d0e53
```

### `dpkg` source package: `libzstd=1.4.5+dfsg-2`

Binary Packages:

- `libzstd1:amd64=1.4.5+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.5+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg-2.dsc' libzstd_1.4.5+dfsg-2.dsc 2291 SHA256:d60b1b16ca0370bc2f6715ad9cd350c224d9045ed71a657a70dc48ff9dc3caa2
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg.orig.tar.xz' libzstd_1.4.5+dfsg.orig.tar.xz 1387864 SHA256:ff51192647c8f87f447268e20180fe39fe8eb5d643210b82f90af741d7bdf0d2
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.5+dfsg-2.debian.tar.xz' libzstd_1.4.5+dfsg-2.debian.tar.xz 12080 SHA256:0e0ff4bf091cc7cdf2df1108739640fb52b779db8681928dabc7a1bd873befb1
```

### `dpkg` source package: `lsb=11.1.0ubuntu2`

Binary Packages:

- `lsb-base=11.1.0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.dsc' lsb_11.1.0ubuntu2.dsc 2230 SHA256:983ff4ab1ab2b39af974e4b8f4373ab4028d0ee5a409e7cd40401fa8e6ecabde
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.tar.xz' lsb_11.1.0ubuntu2.tar.xz 46024 SHA256:c6ab63b6702dc633988690aacde8ece3e460f8acd8f1af8e6a67ab2fe0798f41
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
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.dsc' lz4_1.9.2-2.dsc 1956 SHA256:103fa80edbf501cf6e6d9ee0ed3d75d6111cd06026b00aaccaa11fe5555b71a6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2.orig.tar.gz' lz4_1.9.2.orig.tar.gz 305796 SHA256:658ba6191fa44c92280d4aa2c271b0f4fbc0e34d249578dd05e50e76d0e5efcc
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.debian.tar.xz' lz4_1.9.2-2.debian.tar.xz 12712 SHA256:8970a0afc2f1633bbc8b7f55fa36ba711fb4d0c1811e591ad8f52d1d1968592c
```

### `dpkg` source package: `mawk=1.3.4.20200120-2`

Binary Packages:

- `mawk=1.3.4.20200120-2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.dsc' mawk_1.3.4.20200120-2.dsc 1915 SHA256:5069c46872ac74f5221250dfb88b31b1f2dbb8a2617c1e013f8f80cc34638c6d
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.debian.tar.xz' mawk_1.3.4.20200120-2.debian.tar.xz 7504 SHA256:b772ed2f016b0286980c46cbc1f1f4ae62887ef2aa3dff6ef10cae638f923f26
```

### `dpkg` source package: `mercurial=5.4.1-1ubuntu2`

Binary Packages:

- `mercurial=5.4.1-1ubuntu2`
- `mercurial-common=5.4.1-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/mercurial/copyright`, `/usr/share/doc/mercurial-common/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris mercurial=5.4.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.4.1-1ubuntu2.dsc' mercurial_5.4.1-1ubuntu2.dsc 2830 SHA256:d0fa49d9d5893b97853f80f187f249e8c345c1647d69dccc26125d7af8764b7e
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.4.1.orig.tar.gz' mercurial_5.4.1.orig.tar.gz 7725893 SHA256:c31c026b09e8e1301ff23b5acc8a8563eeecbf7ff3495110b13688f01ba88ac6
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.4.1.orig.tar.gz.asc' mercurial_5.4.1.orig.tar.gz.asc 833 SHA256:85a25b7cda3303d06d109f4858e8981f5f9cfce0e7a1161d24fd2f505adf15b8
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mercurial/mercurial_5.4.1-1ubuntu2.debian.tar.xz' mercurial_5.4.1-1ubuntu2.debian.tar.xz 62900 SHA256:64979e17cfc49e8281bf33295be8bd7e132c5b3303e6f64b44ce008f54824c14
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
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.dsc' mime-support_3.64ubuntu1.dsc 1729 SHA256:669ba4f3fd7594f1c32731b5636b499f44f21c7667148f6f0d16043708743fdc
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.tar.xz' mime-support_3.64ubuntu1.tar.xz 33980 SHA256:5007d2ebc25935bfca6d4bdac0efdfc089a38c1be49d19f0422559f666e4f2c4
```

### `dpkg` source package: `mpdecimal=2.4.2-3`

Binary Packages:

- `libmpdec2:amd64=2.4.2-3`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-3.dsc' mpdecimal_2.4.2-3.dsc 1932 SHA256:4cdd04de9915af3c9d787f4922affc1993d76c25cd0715ffdd2658da37c86753
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-3.debian.tar.xz' mpdecimal_2.4.2-3.debian.tar.xz 6352 SHA256:1baf12776a911bc77f76e16aa7600d4ace21a27817f4a56373093065205a9292
```

### `dpkg` source package: `ncurses=6.2-1`

Binary Packages:

- `libncurses6:amd64=6.2-1`
- `libncursesw6:amd64=6.2-1`
- `libtinfo6:amd64=6.2-1`
- `ncurses-base=6.2-1`
- `ncurses-bin=6.2-1`

Licenses: (parsed from: `/usr/share/doc/libncurses6/copyright`, `/usr/share/doc/libncursesw6/copyright`, `/usr/share/doc/libtinfo6/copyright`, `/usr/share/doc/ncurses-base/copyright`, `/usr/share/doc/ncurses-bin/copyright`)

- `BSD-3-clause`
- `MIT/X11`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-1.dsc' ncurses_6.2-1.dsc 4016 SHA256:fc81f03ae9d74b98a6ff6fe5e9a8339bbd71f19aa21f2b041ce5fbecc71cb472
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz' ncurses_6.2.orig.tar.gz 3425862 SHA256:30306e0c76e0f9f1f0de987cf1c82a5c21e1ce6568b9227f7da5b71cbea86c9d
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz.asc' ncurses_6.2.orig.tar.gz.asc 265 SHA256:8733e48fa7dafa61f3df67783402c3b2555fccccff44e912b436a7111b9c8781
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-1.debian.tar.xz' ncurses_6.2-1.debian.tar.xz 51276 SHA256:b5c4958529954ec70226cf73d5a848e2d159a2c2115faf57258009e28b2e110d
```

### `dpkg` source package: `netbase=6.1`

Binary Packages:

- `netbase=6.1`

Licenses: (parsed from: `/usr/share/doc/netbase/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris netbase=6.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.dsc' netbase_6.1.dsc 1480 SHA256:d3d24cf00001259d3311c0509b4e23ac150cffea27b546e3a204864f52824556
'http://archive.ubuntu.com/ubuntu/pool/main/n/netbase/netbase_6.1.tar.xz' netbase_6.1.tar.xz 31984 SHA256:084d743bd84d4d9380bac4c71c51e57406dce44f5a69289bb823c903e9b035d8
```

### `dpkg` source package: `nettle=3.5.1+really3.5.1-2`

Binary Packages:

- `libhogweed5:amd64=3.5.1+really3.5.1-2`
- `libnettle7:amd64=3.5.1+really3.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libhogweed5/copyright`, `/usr/share/doc/libnettle7/copyright`)

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
$ apt-get source -qq --print-uris nettle=3.5.1+really3.5.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.dsc' nettle_3.5.1+really3.5.1-2.dsc 2375 SHA256:a64c789e3997a2bba012e0c136de9c11b1bc95cf03069c35d26b00582481eecf
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz' nettle_3.5.1+really3.5.1.orig.tar.gz 1989593 SHA256:75cca1998761b02e16f2db56da52992aef622bf55a3b45ec538bc2eedadc9419
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz.asc' nettle_3.5.1+really3.5.1.orig.tar.gz.asc 573 SHA256:557116e471c7c4556148866b5cec056d6de5f26d080e5930154018be6a9d893e
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.debian.tar.xz' nettle_3.5.1+really3.5.1-2.debian.tar.xz 20044 SHA256:7e816adb06d13913bcd350ca6cb777230b82508ca2d358a4062e5676bf335529
```

### `dpkg` source package: `nghttp2=1.41.0-2`

Binary Packages:

- `libnghttp2-14:amd64=1.41.0-2`

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
$ apt-get source -qq --print-uris nghttp2=1.41.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0-2.dsc' nghttp2_1.41.0-2.dsc 2548 SHA256:de017fb480273ab1f2a5581fd11773fdfbbb64685fe07a4398a98a02f3d7d76a
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0.orig.tar.bz2' nghttp2_1.41.0.orig.tar.bz2 1943304 SHA256:645ca078e7ec276dcfa27175f3af6140c8badc7358ec9d2892b6ab2bcee72240
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.41.0-2.debian.tar.xz' nghttp2_1.41.0-2.debian.tar.xz 13268 SHA256:ac0b8341728592ca0de4a73646c2c5c24b4d46df5e6e726b7816e9de52f1d0b2
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
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-2.dsc' npth_1.6-2.dsc 1931 SHA256:7bb227f06b60eabbcc02a4fc4c46eba0aec430dda34b6bc7521c53deb9514a71
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA256:1393abd9adcf0762d34798dc34fdcf4d0d22a8410721e76f1e3afcd1daa4e2d1
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-2.debian.tar.xz' npth_1.6-2.debian.tar.xz 10612 SHA256:e848caf5b5296f7415a7af41f97bd9ec1fcc2b477cb134e4ee4309e15f84323a
```

### `dpkg` source package: `openldap=2.4.50+dfsg-1ubuntu2`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.50+dfsg-1ubuntu2`
- `libldap-common=2.4.50+dfsg-1ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.50+dfsg-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.50+dfsg-1ubuntu2.dsc' openldap_2.4.50+dfsg-1ubuntu2.dsc 3154 SHA256:10bb5181fceadd25b5a3b07e9e2c2ae08368653b91afe820bb74ac59ff0b7da4
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.50+dfsg.orig.tar.gz' openldap_2.4.50+dfsg.orig.tar.gz 4891077 SHA256:77e5be35661d2fb51c4425fc5985c668fa0e53cbc83a6c0962470fd240fd7655
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.50+dfsg-1ubuntu2.debian.tar.xz' openldap_2.4.50+dfsg-1ubuntu2.debian.tar.xz 181116 SHA256:aaba6b10665e9cdc8e2148bd450455cb5fdcb513360a67ceaef6c8c93a94c7e5
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
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1-1.dsc' openssh_8.3p1-1.dsc 3342 SHA256:7a0f9f0001d10bf6270b47e1c0c75d82e118234609bb75233ffd08877d0d3186
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1.orig.tar.gz' openssh_8.3p1.orig.tar.gz 1706358 SHA256:f2befbe0472fe7eb75d23340eb17531cb6b3aac24075e2066b41f814e12387b2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1.orig.tar.gz.asc' openssh_8.3p1.orig.tar.gz.asc 683 SHA256:c5a5f84a482c93ee59eccb8f9f76b6c70eed56fd9b059fc72b3184effa8135f5
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.3p1-1.debian.tar.xz' openssh_8.3p1-1.debian.tar.xz 176252 SHA256:edeb381f43f9b4399fa34f3fab40d60617f3391774304493f2ee7a8dba214ba9
```

### `dpkg` source package: `openssl=1.1.1f-1ubuntu3`

Binary Packages:

- `libssl1.1:amd64=1.1.1f-1ubuntu3`
- `openssl=1.1.1f-1ubuntu3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1f-1ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu3.dsc' openssl_1.1.1f-1ubuntu3.dsc 2705 SHA256:3b58d6628e89793a297bc5591901bfe3374a708042d384df6e8ec908e5e3c39c
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz' openssl_1.1.1f.orig.tar.gz 9792828 SHA256:186c6bfe6ecfba7a5b48c47f8a1673d0f3b0e5ba2e25602dd23b629975da3f35
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz.asc' openssl_1.1.1f.orig.tar.gz.asc 488 SHA256:e9c68097b05be8873e41bd33a9269378ca58e515fbaa30a512c315b602d41dda
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu3.debian.tar.xz' openssl_1.1.1f-1ubuntu3.debian.tar.xz 145256 SHA256:dd675e883550730e221da191588a0b27a5a76115f754e37672681d198505411a
```

### `dpkg` source package: `p11-kit=0.23.20-1build1`

Binary Packages:

- `libp11-kit0:amd64=0.23.20-1build1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.20-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20-1build1.dsc' p11-kit_0.23.20-1build1.dsc 2466 SHA256:25b3e4f00439457152fa958f1b54e0222fbb98585aa174308b6d6534b94445c3
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20.orig.tar.xz' p11-kit_0.23.20.orig.tar.xz 822588 SHA256:14d86024c3dfd6b967d9bc0b4ec7b2973014fe7423481f4d230a1a63b8aa6104
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20.orig.tar.xz.asc' p11-kit_0.23.20.orig.tar.xz.asc 854 SHA256:6429a15c3c071629add6712ed75916df90043d47250edb9235d89ee197f613b8
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20-1build1.debian.tar.xz' p11-kit_0.23.20-1build1.debian.tar.xz 22004 SHA256:c43279d68adc9f710ff438f7084316e1e3ca9918f7c653bf1cb932927c415960
```

### `dpkg` source package: `pam=1.3.1-5ubuntu4`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu4`
- `libpam-modules-bin=1.3.1-5ubuntu4`
- `libpam-runtime=1.3.1-5ubuntu4`
- `libpam0g:amd64=1.3.1-5ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu4.dsc' pam_1.3.1-5ubuntu4.dsc 2699 SHA256:b0d51a23352d570209f00156b796e685cee249dfcc36872154de0138f0b27e4b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA256:eff47a4ecd833fbf18de9686632a70ee8d0794b79aecb217ebd0ce11db4cd0db
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu4.debian.tar.xz' pam_1.3.1-5ubuntu4.debian.tar.xz 159780 SHA256:d5c539ac0bb5d05b62a2e9f936145d1cc8dbf94a91e0268e7ae98f043dbe8b0b
```

### `dpkg` source package: `pcre2=10.34-7`

Binary Packages:

- `libpcre2-8-0:amd64=10.34-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.34-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.dsc' pcre2_10.34-7.dsc 2286 SHA256:c3e2bfd8fabf594238b3f17074dc8ac483aaf80a9f12dbfe927b80a74558732e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34.orig.tar.gz' pcre2_10.34.orig.tar.gz 2271533 SHA256:da6aba7ba2509e918e41f4f744a59fa41a2425c59a298a232e7fe85691e00379
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.diff.gz' pcre2_10.34-7.diff.gz 7068 SHA256:7d44ac1b171ef7f7051213a3a8505b28f3809ed3e2fb348567a29fdf5f2b5fdf
```

### `dpkg` source package: `pcre3=2:8.39-13`

Binary Packages:

- `libpcre3:amd64=2:8.39-13`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-13
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.dsc' pcre3_8.39-13.dsc 2226 SHA256:c3a2eb4f02de5b2e00787ed2a35eb82f04ee4b5e99b8ff279bae3c6453aad93b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-13.debian.tar.gz' pcre3_8.39-13.debian.tar.gz 27002 SHA256:a2143d7358d69b61955a4f977980050447f8891c0e6737080f2b14b920fbde87
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
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3-4.dsc' perl_5.30.3-4.dsc 2983 SHA256:05c8d356f72848b6e26b57949b5fb7dcc6340719df292f83d02ff05fb84cdd98
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3.orig-regen-configure.tar.gz' perl_5.30.3.orig-regen-configure.tar.gz 870970 SHA256:99174174fbfc550f801076ab8a1a5831c92f75c1b81e553150351f14a111dcf8
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3.orig.tar.xz' perl_5.30.3.orig.tar.xz 12375128 SHA256:6967595f2e3f3a94544c35152f9a25e0cb8ea24ae45f4bf1882f2e33f4a400f4
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.3-4.debian.tar.xz' perl_5.30.3-4.debian.tar.xz 171184 SHA256:a71ed73cab42cadb8cb9efe430ac075e644fea527f3689b64e4e0fe8b9648ffd
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
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.dsc' pinentry_1.1.0-4build1.dsc 2595 SHA256:37fbbefc36e4041a80b0e7b4d9770899a3098a1975531e2b84da6914dbe04557
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-4build1.debian.tar.xz' pinentry_1.1.0-4build1.debian.tar.xz 17312 SHA256:ccccd3ee3b589456a5e26883608cf75da6e49a9c0e161191c35ceaf509d64489
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

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.16-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-5ubuntu1.dsc' procps_3.3.16-5ubuntu1.dsc 2271 SHA256:f3ba7b03cb6bacb7ae06646ab34757d4de6f93a046304dbf8ebfe48be51cb16b
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16.orig.tar.xz' procps_3.3.16.orig.tar.xz 621892 SHA256:2919299e579d29be3501a802dfe77e6f23be228149d0396d83d0ffbe8fa7efbf
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-5ubuntu1.debian.tar.xz' procps_3.3.16-5ubuntu1.debian.tar.xz 33768 SHA256:70672be61b079e25f078ad93ae3a63ac318a013649d6b6c391b020ca01516bce
```

### `dpkg` source package: `python-certifi=2020.4.5.1-1`

Binary Packages:

- `python3-certifi=2020.4.5.1-1`

Licenses: (parsed from: `/usr/share/doc/python3-certifi/copyright`)

- `GPL-2`
- `MPL-2`

Source:

```console
$ apt-get source -qq --print-uris python-certifi=2020.4.5.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1-1.dsc' python-certifi_2020.4.5.1-1.dsc 1634 SHA256:fc08f36819c72391207038f5aeb0ee26e8b09238930cba8fb51ad6d3509e58f1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1.orig.tar.xz' python-certifi_2020.4.5.1.orig.tar.xz 144464 SHA256:99350293fccff4fb1e7c4a60ce09519704dce14fc347c18dc915699eb033a758
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-certifi/python-certifi_2020.4.5.1-1.debian.tar.xz' python-certifi_2020.4.5.1-1.debian.tar.xz 7732 SHA256:3c23ee1a03b3b242df921a55fd360d2deb7ca15d8879c72a4987aec1b99c88ed
```

### `dpkg` source package: `python-defaults=2.7.17-2ubuntu4`

Binary Packages:

- `libpython2-stdlib:amd64=2.7.17-2ubuntu4`
- `python2=2.7.17-2ubuntu4`
- `python2-minimal=2.7.17-2ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-defaults=2.7.17-2ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-defaults/python-defaults_2.7.17-2ubuntu4.dsc' python-defaults_2.7.17-2ubuntu4.dsc 2558 SHA256:3b07888350cc8d6f8506b0a42b65e4f83e21b582c2fd6f29b91bca181ba0666e
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-defaults/python-defaults_2.7.17-2ubuntu4.tar.gz' python-defaults_2.7.17-2ubuntu4.tar.gz 82316 SHA256:571c7958e16daab3b3350f061fa3a4c2a30250fc9f8f5ef29a68a012fe83c1af
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
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8-5build1.dsc' python-fastimport_0.9.8-5build1.dsc 2244 SHA256:2ca7934d75936cc98c4520b19844a02ba23c7325116dd0cd37b55a0265dbbf0f
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8.orig.tar.gz' python-fastimport_0.9.8.orig.tar.gz 39512 SHA256:b2f2e8eb97000256e1aab83d2a0a053fc7b93c3aa4f7e9b971a5703dfc5963b9
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-fastimport/python-fastimport_0.9.8-5build1.debian.tar.xz' python-fastimport_0.9.8-5build1.debian.tar.xz 13644 SHA256:f83a7b8f5824f22c46aacb7ededbed2d801cbcedf67500c5ac3bc71aa6aa981c
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
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9-1.dsc' python-urllib3_1.25.9-1.dsc 2217 SHA256:156567637b749e5070162a3ff3470d0e98c50c93769c925fbabcd483b0bccc07
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9.orig.tar.gz' python-urllib3_1.25.9.orig.tar.gz 254921 SHA256:3018294ebefce6572a474f0604c2021e33b3fd8006ecd11d62107a5d2a963527
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-urllib3/python-urllib3_1.25.9-1.debian.tar.xz' python-urllib3_1.25.9-1.debian.tar.xz 11472 SHA256:ddf5629ac197176e0d49aac038eac2090dde93f75b33b09988a3bb46e77de146
```

### `dpkg` source package: `python2.7=2.7.18-1`

Binary Packages:

- `libpython2.7-minimal:amd64=2.7.18-1`
- `libpython2.7-stdlib:amd64=2.7.18-1`
- `python2.7=2.7.18-1`
- `python2.7-minimal=2.7.18-1`

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
$ apt-get source -qq --print-uris python2.7=2.7.18-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.18-1.dsc' python2.7_2.7.18-1.dsc 3290 SHA256:deff818747f652988b5f95edba9432ba5932cf8eedc7a831c090002da04ab361
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.18.orig.tar.gz' python2.7_2.7.18.orig.tar.gz 17539408 SHA256:da3080e3b488f648a3d7a4560ddee895284c3380b11d6de75edb986526b9a814
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python2.7/python2.7_2.7.18-1.diff.gz' python2.7_2.7.18-1.diff.gz 287032 SHA256:b738ffc73397cf2a24faedd4c5c3d1591f7009d5a43f6d09b60e2e69bf74ed69
```

### `dpkg` source package: `python3-defaults=3.8.2-0ubuntu2`

Binary Packages:

- `libpython3-stdlib:amd64=3.8.2-0ubuntu2`
- `python3=3.8.2-0ubuntu2`
- `python3-minimal=3.8.2-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.8.2-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.8.2-0ubuntu2.dsc' python3-defaults_3.8.2-0ubuntu2.dsc 2879 SHA256:3fa296ea2cd52738ebc44a1b83a8df500bf654356336d9bf057144171fe9ee7d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.8.2-0ubuntu2.tar.gz' python3-defaults_3.8.2-0ubuntu2.tar.gz 138226 SHA256:e4969a54306421ebfd195d0c064935db7c53f9f152d8abaae63da33819235e9a
```

### `dpkg` source package: `python3.8=3.8.3-1`

Binary Packages:

- `libpython3.8-minimal:amd64=3.8.3-1`
- `libpython3.8-stdlib:amd64=3.8.3-1`
- `python3.8=3.8.3-1`
- `python3.8-minimal=3.8.3-1`

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

Source:

```console
$ apt-get source -qq --print-uris python3.8=3.8.3-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.8/python3.8_3.8.3-1.dsc' python3.8_3.8.3-1.dsc 3288 SHA256:646806a66cd9299459a21e990069fe31bfd8c3e8fdb66a842ffed66ae023258c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.8/python3.8_3.8.3.orig.tar.xz' python3.8_3.8.3.orig.tar.xz 17912964 SHA256:dfab5ec723c218082fe3d5d7ae17ecbdebffa9a1aea4d64aa3a2ecdd2e795864
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3.8/python3.8_3.8.3-1.debian.tar.xz' python3.8_3.8.3-1.debian.tar.xz 210020 SHA256:d1562489156121a1232bdc5eabba431e57a8e1415f3a09c27751ac0ecef31306
```

### `dpkg` source package: `readline=8.0-4`

Binary Packages:

- `libreadline8:amd64=8.0-4`
- `readline-common=8.0-4`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.dsc' readline_8.0-4.dsc 2434 SHA256:ac9c7bb7380fe740aef09f54becf482eb81032a33dc11f1a8f00e933c5f168f4
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0.orig.tar.gz' readline_8.0.orig.tar.gz 2975937 SHA256:e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.debian.tar.xz' readline_8.0-4.debian.tar.xz 30408 SHA256:60ed18dab6d6b7fc998a263d917f06d9cce6e1ccd19cd8bf4a9d33c5350cf8d6
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2build1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2build1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build1.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build1.dsc 2439 SHA256:fd89213f2d41b00c212a411a945146c6b2e00fce1d1819a9ec380b0d91bd1077
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build1.debian.tar.xz 8216 SHA256:b256cc2aa96c9b99918052c4badfab0339ba95a852eab5ae37aa8b53c259efd2
```

### `dpkg` source package: `sed=4.7-1`

Binary Packages:

- `sed=4.7-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.

The source package *may* still be available for download from:

- http://snapshot.debian.org/package/sed/4.7-1/


### `dpkg` source package: `sensible-utils=0.0.12+nmu1`

Binary Packages:

- `sensible-utils=0.0.12+nmu1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.12+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12+nmu1.dsc' sensible-utils_0.0.12+nmu1.dsc 1753 SHA256:68bcb3e542e29a8a0bf281d9145d0e4cd9def529af2ba0cfe0afee3c5af958bc
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12+nmu1.tar.xz' sensible-utils_0.0.12+nmu1.tar.xz 61988 SHA256:53c6606facf083adbbf0da04e6d774b31ff3f46c7ba36a82d3f182779f4c3f5b
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
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu6.dsc' shadow_4.8.1-1ubuntu6.dsc 1705 SHA256:f74fd356e3d237624704a1698da160f28f87d780f1d989ad3f494a924242e7c6
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA256:a3ad4630bdc41372f02a647278a8c3514844295d36eefe68ece6c3a641c1ae62
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu6.debian.tar.xz' shadow_4.8.1-1ubuntu6.debian.tar.xz 85620 SHA256:d45a2d33774f455295be012e9828d99dc6cb7cf1bc76ba12e0cfc55296740b20
```

### `dpkg` source package: `six=1.15.0-1`

Binary Packages:

- `python3-six=1.15.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.15.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0-1.dsc' six_1.15.0-1.dsc 2411 SHA256:7a7899358165af2c5e1d9c939b5f66fadb83ef7bc4a806bded01121088bde00c
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0.orig.tar.gz' six_1.15.0.orig.tar.gz 33917 SHA256:30639c035cdb23534cd4aa2dd52c3bf48f06e5f4a941509c8bafd8ce11080259
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.15.0-1.debian.tar.xz' six_1.15.0-1.debian.tar.xz 4480 SHA256:6ccff1bff18fe0de27bc90c652fa8e5f3822c66020e533a9c40fd45b8cefe760
```

### `dpkg` source package: `sqlite3=3.31.1-5`

Binary Packages:

- `libsqlite3-0:amd64=3.31.1-5`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.31.1-5
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1-5.dsc' sqlite3_3.31.1-5.dsc 2404 SHA256:6f3de8b7819cb4851dcbb2d96aaf2b5f0c3f38e2b9f2320c83b3dc2c01549b6e
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1.orig-www.tar.xz' sqlite3_3.31.1.orig-www.tar.xz 5764424 SHA256:cab01c285fad4eb08bd1e3659cde5a44e17e024badbe9ed01b2de9c625ed0831
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1.orig.tar.xz' sqlite3_3.31.1.orig.tar.xz 7108036 SHA256:dfa6eda312d391d33b7790b061f533d723dc5c30b60720ddd98c89a6fb29272f
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1-5.debian.tar.xz' sqlite3_3.31.1-5.debian.tar.xz 25936 SHA256:96cc015782946a5d92502ddc3d2208397d209788d599d940d58c717a625b8829
```

### `dpkg` source package: `subversion=1.14.0-1`

Binary Packages:

- `libsvn1:amd64=1.14.0-1`
- `subversion=1.14.0-1`

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
$ apt-get source -qq --print-uris subversion=1.14.0-1
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0-1.dsc' subversion_1.14.0-1.dsc 3807 SHA256:efb177ab8d566c8dadd01919cb114264961d84e9f0c7ea24a78234ff1f267ea5
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0.orig.tar.gz' subversion_1.14.0.orig.tar.gz 11519871 SHA256:ef3d1147535e41874c304fb5b9ea32745fbf5d7faecf2ce21d4115b567e937d0
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0.orig.tar.gz.asc' subversion_1.14.0.orig.tar.gz.asc 3917 SHA256:98333df38d29a64500d4ad1693741d3d087485555207289b4e53af309abac71a
'http://archive.ubuntu.com/ubuntu/pool/universe/s/subversion/subversion_1.14.0-1.debian.tar.xz' subversion_1.14.0-1.debian.tar.xz 426604 SHA256:2df3c0e9ad9f8ef33d5d3c2ffc19c89b5d0cb8850c526842baa356ca85ac3e3c
```

### `dpkg` source package: `systemd=245.6-1ubuntu1`

Binary Packages:

- `libsystemd0:amd64=245.6-1ubuntu1`
- `libudev1:amd64=245.6-1ubuntu1`

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
$ apt-get source -qq --print-uris systemd=245.6-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.6-1ubuntu1.dsc' systemd_245.6-1ubuntu1.dsc 5284 SHA256:456f4c0fffb511b05f9679ee039965e4b7781a326e6bebc373fee4041f60799f
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.6.orig.tar.gz' systemd_245.6.orig.tar.gz 9022866 SHA256:f58424fd2d105503f836ff7d099d762901fb40347de993fce7373d65ff640f5b
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.6-1ubuntu1.debian.tar.xz' systemd_245.6-1ubuntu1.debian.tar.xz 210288 SHA256:f9c854bbde9bec45c6f0d8da0c3044010d49cb7a4dd73cd9e3e35c4b09e68ffb
```

### `dpkg` source package: `sysvinit=2.96-3ubuntu1`

Binary Packages:

- `sysvinit-utils=2.96-3ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-3ubuntu1.dsc' sysvinit_2.96-3ubuntu1.dsc 2781 SHA256:64bab02372e0400ceeb1937a77f127246ae8c6ce63dbebdf309c483bb35179e0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA256:2a2e26b72aa235a23ab1c8471005f890309ce1196c83fbc9413c57b9ab62b587
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA256:dfc184b95da12c8c888c8ae6b0f26fe8a23b07fbcdd240f6600a8a78b9439fa0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-3ubuntu1.debian.tar.xz' sysvinit_2.96-3ubuntu1.debian.tar.xz 128020 SHA256:ce2ed9502ae88eda25db4896ba1bc881794f026b0b8c47419358b2fbd92d8533
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
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.dsc' tar_1.30+dfsg-7.dsc 1981 SHA256:5117afe47b5aab94c592d52c11c74dba146a11a7cdc22dbe067a4b5a5e895729
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA256:c02f3747ffe02017878303dde8b78e79cd220364c5e8048cf92320232e38912d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.debian.tar.xz' tar_1.30+dfsg-7.debian.tar.xz 22168 SHA256:12763df7f214458a56edc4a4b27adb2cb2041d597d74212ba34736f02bb68cd3
```

### `dpkg` source package: `ubuntu-keyring=2020.06.17.1`

Binary Packages:

- `ubuntu-keyring=2020.06.17.1`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2020.06.17.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.dsc' ubuntu-keyring_2020.06.17.1.dsc 1863 SHA256:9ac7c2d8d5b4132872ef2e5a7ece4f73249e53d2aa36b075697e454e643e7ae6
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.06.17.1.tar.gz' ubuntu-keyring_2020.06.17.1.tar.gz 36420 SHA256:e31ba06e1332002e0649c206f54fa67fee038e27f43b9e59e872f1de14a00774
```

### `dpkg` source package: `ucf=3.0043`

Binary Packages:

- `ucf=3.0043`

Licenses: (parsed from: `/usr/share/doc/ucf/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris ucf=3.0043
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043.dsc' ucf_3.0043.dsc 1423 SHA256:5954508238ff1b8e2c61e1f533268911ba06709e821c02de014fd15d2ead81fd
'http://archive.ubuntu.com/ubuntu/pool/main/u/ucf/ucf_3.0043.tar.xz' ucf_3.0043.tar.xz 70560 SHA256:0294cc11a6cf032ea99ca5064f73a4ede5b28bc2d4ad0a12e8493c7520c7a2a4
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
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0-1.dsc' utf8proc_2.5.0-1.dsc 2154 SHA256:2137104a3712875650629305fe7d7ef37d4d99328846c18b087b289c0ddbf27c
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0.orig.tar.gz' utf8proc_2.5.0.orig.tar.gz 155485 SHA256:d4e8dfc898cfd062493cb7f42d95d70ccdd3a4cd4d90bec0c71b47cca688f1be
'http://archive.ubuntu.com/ubuntu/pool/universe/u/utf8proc/utf8proc_2.5.0-1.debian.tar.xz' utf8proc_2.5.0-1.debian.tar.xz 5240 SHA256:333496cf4e178b5ccf4972fa52523d07a21a0cabf0cb123133c6c71f98e92eff
```

### `dpkg` source package: `util-linux=2.35.2-5ubuntu3`

Binary Packages:

- `bsdutils=1:2.35.2-5ubuntu3`
- `libblkid1:amd64=2.35.2-5ubuntu3`
- `libmount1:amd64=2.35.2-5ubuntu3`
- `libsmartcols1:amd64=2.35.2-5ubuntu3`
- `libuuid1:amd64=2.35.2-5ubuntu3`
- `mount=2.35.2-5ubuntu3`
- `util-linux=2.35.2-5ubuntu3`

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


### `dpkg` source package: `wget=1.20.3-1ubuntu1`

Binary Packages:

- `wget=1.20.3-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/wget/copyright`)

- `GFDL-1.2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris wget=1.20.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3-1ubuntu1.dsc' wget_1.20.3-1ubuntu1.dsc 2280 SHA256:e40e00e9f93f1c049cd2b7942c9c9e31504acd56350b31f1ecad6ae220a44dfd
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3.orig.tar.gz' wget_1.20.3.orig.tar.gz 4489249 SHA256:31cccfc6630528db1c8e3a06f6decf2a370060b982841cfab2b8677400a5092e
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3.orig.tar.gz.asc' wget_1.20.3.orig.tar.gz.asc 833 SHA256:7b295c84ab6f90c328a203e234e4b2f5f45cb8d2e29eac43a977073933cd49a2
'http://archive.ubuntu.com/ubuntu/pool/main/w/wget/wget_1.20.3-1ubuntu1.debian.tar.xz' wget_1.20.3-1ubuntu1.debian.tar.xz 63312 SHA256:95ae56081866b9e6dfb2a2d2dc2208ba0cf3c76bb5d7e680cc56b18b3ec66c1e
```

### `dpkg` source package: `xz-utils=5.2.4-1`

Binary Packages:

- `liblzma5:amd64=5.2.4-1`

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
$ apt-get source -qq --print-uris xz-utils=5.2.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1.dsc' xz-utils_5.2.4-1.dsc 2518 SHA256:b1572c4efb3c8ebf6f0e044b70e1e0451c919a99d3f80be03b624a54dd7ea593
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA256:9717ae363760dedf573dad241420c5fea86256b65bc21d2cf71b2b12f0544f4b
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA256:88290c1deeaf674ae2a4821f4373fe0e4cc2a94199eae6dcc26df1e70cc15303
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1.debian.tar.xz' xz-utils_5.2.4-1.debian.tar.xz 135296 SHA256:d37b558444b76e88a69601df008cf1c0343c58cb7765b7bbb2099b0a19619361
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu1`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu1.dsc' zlib_1.2.11.dfsg-2ubuntu1.dsc 2970 SHA256:2e56b0d54d841d974c96e6cc4361da7c75b1848cded85412cdb4b4bc7791233a
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu1.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu1.debian.tar.xz 49448 SHA256:11c13ba58bd033dbfd2c7408f4a4eaa02035e007dea79ae20f0db580eaa53c9c
```
