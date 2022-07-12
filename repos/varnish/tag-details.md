<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.10`](#varnish6010)
-	[`varnish:7.0`](#varnish70)
-	[`varnish:7.0-alpine`](#varnish70-alpine)
-	[`varnish:7.0.2`](#varnish702)
-	[`varnish:7.0.2-alpine`](#varnish702-alpine)
-	[`varnish:7.1`](#varnish71)
-	[`varnish:7.1-alpine`](#varnish71-alpine)
-	[`varnish:7.1.0`](#varnish710)
-	[`varnish:7.1.0-alpine`](#varnish710-alpine)
-	[`varnish:alpine`](#varnishalpine)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:fresh-alpine`](#varnishfresh-alpine)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:old`](#varnishold)
-	[`varnish:old-alpine`](#varnishold-alpine)
-	[`varnish:stable`](#varnishstable)

## `varnish:6.0`

```console
$ docker pull varnish@sha256:75cde1f365c01d4f67a4acb2fc4c0f6847b81567649f30c13987f455f59b6e13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:a6aec0b505ab121e0a3a6ed41af86dbea176d84b06114a9125ebc3adf4d4fd9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100578628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592008399710472f47e4e41199f0fa992d820b25e4714cb3dbc7e299f9d03a2c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:08:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 15:09:00 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:09:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:09:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:09:00 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:09:00 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89be986846906e3bd77fcb69c2287e9b2967e13e6db6789e5baf1d506be18d0d`  
		Last Modified: Tue, 12 Jul 2022 15:10:32 GMT  
		Size: 69.2 MB (69211316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a428efaa1b7e1631a51a487cd7d5d5cc05b0e39a4ffa98c2aec733eaf642f2d`  
		Last Modified: Tue, 12 Jul 2022 15:10:22 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:2c4b41efa4196611ae6cb4b6eddcf84bdc0e1a43a03b4c76aac3eedca9b087fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77226111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d94aa4723ac8b23869f306e96838344ed1f5a2cd74755ebfeda8cb2b50e4e28b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:49:30 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 14:01:27 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 24 Jun 2022 14:01:28 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 14:01:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 24 Jun 2022 14:01:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 14:01:29 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 14:01:30 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a9c851df1c2951d6a3d73f1c5810a184f118b264badec4600fcf771ce8931f`  
		Last Modified: Fri, 24 Jun 2022 14:05:06 GMT  
		Size: 50.6 MB (50649305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e281c64d9d1456fd161381c1684f89e9b344f5d89c5828842b284f7d6a7424`  
		Last Modified: Fri, 24 Jun 2022 14:04:37 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:3344e5dbea7c39c0e78316c060bc7cdaf6914c5c484446a18801ad7ea97245e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94702840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664add611afb8aa9218e165904e2c908a1e45e7884530a8f0e3dca4579266009`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:18:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:23:35 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 14:23:36 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:23:38 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:23:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:23:39 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:23:40 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d8825494e5a3d0e5dc7419b15ef72845e7cd473e057dab29425c350e56f8b6`  
		Last Modified: Tue, 12 Jul 2022 14:25:36 GMT  
		Size: 64.6 MB (64647915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71275849326318c97b15f88b97e005a2f8436f713efc326d5ee465ce462a0bfc`  
		Last Modified: Tue, 12 Jul 2022 14:25:27 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:854e3a098f80fdeba4d4cc76090415b08fe9784ac0c51df85bf79af763af0300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102058379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b66188412d2b0af5c64a7ff374272c2c50a99d47354c94fab8596c55197ab2a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:15:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 10:18:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 10:18:48 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 10:18:50 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:18:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 10:18:51 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 10:18:52 GMT
CMD []
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275617bc24aba724d9e033099ad564c3d9848c6b195104cd4d16bd7373466bd1`  
		Last Modified: Tue, 12 Jul 2022 10:20:26 GMT  
		Size: 69.7 MB (69683727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7943edd0a7e181bd2b8627956de13a2ad69628c8b0c11640a5dfb9c260a9bd1`  
		Last Modified: Tue, 12 Jul 2022 10:20:14 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:6b84cbc1a9c28cf8991d7ec366d46fdbd99b146e3425936b6c4c79385742ff0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99796088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52f7bf64fe65b1bab46892519f2b7f0c892d3ec6613dd2de3f41884d756d9ef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:38:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 07:14:13 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 07:14:18 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 07:14:20 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 07 Jun 2022 07:14:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 07:14:24 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 07:14:26 GMT
CMD []
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbfae2215345643446eec0955f5aa2abf2566a51f5bab1280983b19f267d73`  
		Last Modified: Tue, 07 Jun 2022 07:15:58 GMT  
		Size: 64.5 MB (64508688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019e20eb144f16f23de1ecf38bc429a7f5e2081e77131ebd79e4ef88fdd1f94`  
		Last Modified: Tue, 07 Jun 2022 07:15:46 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:d143ac4588cc1f8f8facfce939eb38ad073081e6f10b158d965369d48ac45cce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80994227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76348292b58d165facf504362ea67a0bdfce1dbfdc009bd51c195e4eff713ae`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:13:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:26:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 19:26:45 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:26:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:26:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:26:46 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:26:47 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5713f0c860e92ea10da6e18fa83f8aad21a2056b3d968ad5b0f975587d0c3614`  
		Last Modified: Tue, 12 Jul 2022 19:28:56 GMT  
		Size: 51.4 MB (51353315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8723d90b7e824ceee06e46c8072d1585b761be55f9a8a12393845318b9e5fc57`  
		Last Modified: Tue, 12 Jul 2022 19:28:49 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.10`

```console
$ docker pull varnish@sha256:75cde1f365c01d4f67a4acb2fc4c0f6847b81567649f30c13987f455f59b6e13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.0.10` - linux; amd64

```console
$ docker pull varnish@sha256:a6aec0b505ab121e0a3a6ed41af86dbea176d84b06114a9125ebc3adf4d4fd9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100578628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592008399710472f47e4e41199f0fa992d820b25e4714cb3dbc7e299f9d03a2c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:08:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 15:09:00 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:09:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:09:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:09:00 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:09:00 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89be986846906e3bd77fcb69c2287e9b2967e13e6db6789e5baf1d506be18d0d`  
		Last Modified: Tue, 12 Jul 2022 15:10:32 GMT  
		Size: 69.2 MB (69211316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a428efaa1b7e1631a51a487cd7d5d5cc05b0e39a4ffa98c2aec733eaf642f2d`  
		Last Modified: Tue, 12 Jul 2022 15:10:22 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; arm variant v7

```console
$ docker pull varnish@sha256:2c4b41efa4196611ae6cb4b6eddcf84bdc0e1a43a03b4c76aac3eedca9b087fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77226111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d94aa4723ac8b23869f306e96838344ed1f5a2cd74755ebfeda8cb2b50e4e28b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:49:30 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 14:01:27 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 24 Jun 2022 14:01:28 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 14:01:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 24 Jun 2022 14:01:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 14:01:29 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 14:01:30 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a9c851df1c2951d6a3d73f1c5810a184f118b264badec4600fcf771ce8931f`  
		Last Modified: Fri, 24 Jun 2022 14:05:06 GMT  
		Size: 50.6 MB (50649305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e281c64d9d1456fd161381c1684f89e9b344f5d89c5828842b284f7d6a7424`  
		Last Modified: Fri, 24 Jun 2022 14:04:37 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:3344e5dbea7c39c0e78316c060bc7cdaf6914c5c484446a18801ad7ea97245e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94702840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664add611afb8aa9218e165904e2c908a1e45e7884530a8f0e3dca4579266009`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:18:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:23:35 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 14:23:36 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:23:38 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:23:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:23:39 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:23:40 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d8825494e5a3d0e5dc7419b15ef72845e7cd473e057dab29425c350e56f8b6`  
		Last Modified: Tue, 12 Jul 2022 14:25:36 GMT  
		Size: 64.6 MB (64647915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71275849326318c97b15f88b97e005a2f8436f713efc326d5ee465ce462a0bfc`  
		Last Modified: Tue, 12 Jul 2022 14:25:27 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; 386

```console
$ docker pull varnish@sha256:854e3a098f80fdeba4d4cc76090415b08fe9784ac0c51df85bf79af763af0300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102058379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b66188412d2b0af5c64a7ff374272c2c50a99d47354c94fab8596c55197ab2a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:15:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 10:18:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 10:18:48 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 10:18:50 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:18:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 10:18:51 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 10:18:52 GMT
CMD []
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275617bc24aba724d9e033099ad564c3d9848c6b195104cd4d16bd7373466bd1`  
		Last Modified: Tue, 12 Jul 2022 10:20:26 GMT  
		Size: 69.7 MB (69683727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7943edd0a7e181bd2b8627956de13a2ad69628c8b0c11640a5dfb9c260a9bd1`  
		Last Modified: Tue, 12 Jul 2022 10:20:14 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; ppc64le

```console
$ docker pull varnish@sha256:6b84cbc1a9c28cf8991d7ec366d46fdbd99b146e3425936b6c4c79385742ff0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99796088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52f7bf64fe65b1bab46892519f2b7f0c892d3ec6613dd2de3f41884d756d9ef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:38:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 07:14:13 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 07:14:18 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 07:14:20 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 07 Jun 2022 07:14:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 07:14:24 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 07:14:26 GMT
CMD []
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbfae2215345643446eec0955f5aa2abf2566a51f5bab1280983b19f267d73`  
		Last Modified: Tue, 07 Jun 2022 07:15:58 GMT  
		Size: 64.5 MB (64508688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019e20eb144f16f23de1ecf38bc429a7f5e2081e77131ebd79e4ef88fdd1f94`  
		Last Modified: Tue, 07 Jun 2022 07:15:46 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; s390x

```console
$ docker pull varnish@sha256:d143ac4588cc1f8f8facfce939eb38ad073081e6f10b158d965369d48ac45cce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80994227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76348292b58d165facf504362ea67a0bdfce1dbfdc009bd51c195e4eff713ae`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:13:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:26:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 19:26:45 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:26:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:26:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:26:46 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:26:47 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5713f0c860e92ea10da6e18fa83f8aad21a2056b3d968ad5b0f975587d0c3614`  
		Last Modified: Tue, 12 Jul 2022 19:28:56 GMT  
		Size: 51.4 MB (51353315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8723d90b7e824ceee06e46c8072d1585b761be55f9a8a12393845318b9e5fc57`  
		Last Modified: Tue, 12 Jul 2022 19:28:49 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0`

```console
$ docker pull varnish@sha256:31f5e697661e5c97a7867e92755cefb5067f5177958c35fe38ca0e4be8fd3dec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0` - linux; amd64

```console
$ docker pull varnish@sha256:80ca9c3ffd61c95e2e3bd468c5906e862e51052636ad1105793018e8d74e9e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101190038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1d0d3f5afe71b234b6dce0b66cfade308ae48e137821cf3cdcdba874199813`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:06:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 15:06:39 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:06:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:06:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:06:40 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:06:40 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de66ed810206b73e0c9dab04edcb5ee5e063727b6d2d4288dcacf0b689f442`  
		Last Modified: Tue, 12 Jul 2022 15:10:08 GMT  
		Size: 69.8 MB (69822955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e847f66816c3e7530bb53d396f9f98bfe1dcb263d37ca0a260ceebccaa19563d`  
		Last Modified: Tue, 12 Jul 2022 15:09:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ef8ee948db46e978034b3e527028c92fb71d2ada0c428b60fd0dd6b5607220c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77822750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2c92def99b9454e428b38b30569a93a8227b85b3f9b4728202cf1dcd9fe007`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:49:30 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 13:55:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 24 Jun 2022 13:55:16 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 13:55:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 13:55:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 13:55:17 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 13:55:17 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87d17e6a126e6e5cda5556cd2a907d0ea8de0abc5a0db774bd93da779ed14e5`  
		Last Modified: Fri, 24 Jun 2022 14:04:17 GMT  
		Size: 51.2 MB (51246170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1253653c109b75569f3681144b8051d73b43acba27dbfc05aa2efb3cb6d0c6`  
		Last Modified: Fri, 24 Jun 2022 14:03:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:6498c5ad6d682b0076a0cbec21fef553b379504c201a87f0f7b5f14f80e9c60c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95301932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e738a742894266ad16f79ecd4b9a3474041d4f12dbfb804dff57c7a5d2db21`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:18:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:21:07 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 14:21:07 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:21:09 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:21:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:21:10 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:21:11 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e13c66f23d97c682dfc6fca33c4ba85b04f2b9b22f0a9d4a32679def5baa25b`  
		Last Modified: Tue, 12 Jul 2022 14:25:10 GMT  
		Size: 65.2 MB (65247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e12339074edaf212e4dc9334de848255f4ef5e943ff9e7833cc7e9b636d52b4`  
		Last Modified: Tue, 12 Jul 2022 14:25:01 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; 386

```console
$ docker pull varnish@sha256:ec9290335f55e308e7023f5d8f4972eebc2b1ee671069d8820851417cc0f17df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102585121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b122adf5e34794ee172b03b3fab482bc31219a96195e1e8c300c8ae4cb9d064c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:15:19 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 00:17:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 00:17:34 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 00:17:36 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:17:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 00:17:37 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 00:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf3f822dbf481370990594e81803141573a456e04899ad82fe6c4022627ebb`  
		Last Modified: Tue, 07 Jun 2022 00:21:08 GMT  
		Size: 70.2 MB (70194327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7dae54c84b4938c9aaa05092d4faf306897f47702a337f22ca87439181cc5`  
		Last Modified: Tue, 07 Jun 2022 00:20:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:2e3c1ac9eacb11fab6237bcd3eff4d406e0b300e5c3144e3934ddf939b4e277c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100378186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b130ac9ed26512fd8cddaf8489ddf70922771377f7b1d009ba5e2de0dd5d960`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:38:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 06:55:41 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 06:55:47 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 06:55:48 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:55:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 06:55:55 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 06:56:00 GMT
CMD []
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c63706549952669ea4fc52e3a012cb12b690358fdde6057b825e1f21313259d`  
		Last Modified: Tue, 07 Jun 2022 07:15:28 GMT  
		Size: 65.1 MB (65091015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe199e856d7bedadb8a4da892a5d774b9146e8358d8909a62fadd06dbce3022b`  
		Last Modified: Tue, 07 Jun 2022 07:15:16 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; s390x

```console
$ docker pull varnish@sha256:4b16cb3b466bbe809c4833e2631cd4a9ddf572227e11c2fb3ce158a52465a752
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81623472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426be98166563a81501f737bf7edd9103507a566117a5395e75a6d54d80ada03`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:13:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:19:47 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 19:19:57 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:19:57 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:19:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:19:59 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:20:00 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f44713e40e8cd034f4c8f4dd815e5302835db628ffb0d6f606de6a30b3e909c`  
		Last Modified: Tue, 12 Jul 2022 19:28:33 GMT  
		Size: 52.0 MB (51982789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a43b712b028475ec29bca3a805cc61d86ec779b321fcd68dcdf093c4f9cfc1e`  
		Last Modified: Tue, 12 Jul 2022 19:28:25 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0-alpine`

```console
$ docker pull varnish@sha256:a96966b666c3eb795b5a5ffe4b7f1911e009156774d5551a355de6ba17dd6ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:1f798a786c909e75214591ae7bb11711b606d19904771e17cac071e3fc945f23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58347562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f303a05efad59d4625679d65998e25ac6af2a5a1e8e761d6165038faf0af7a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:46:19 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 09:47:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 09:47:16 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 09:47:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:47:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 09:47:16 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 09:47:16 GMT
CMD []
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd49c5f702ffa093526e350e19af19adacee36ebd21a4d2b8215729aebd24701`  
		Last Modified: Tue, 05 Apr 2022 09:48:23 GMT  
		Size: 55.5 MB (55528711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b11f3cacc52df447f6e49ab5dcad0b25a3e95d3aa5ca786c8a00b94bcea4d97`  
		Last Modified: Tue, 05 Apr 2022 09:48:15 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:d0ef8137631136de68aa9ca8b5a1c202753588e4823091fc74c7381800475e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44158672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b498faee8096b05f4ad1e1a034d79076f1405006bbb01cdc1b62443d19faf0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:12:30 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 19:13:58 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 19:13:59 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 19:13:59 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 19:14:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 19:14:00 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 19:14:00 GMT
CMD []
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a122a3f3e3f4f262ecd7c937fb5b761d7c7025f6b85195b6f6e59efccc3e22`  
		Last Modified: Tue, 05 Apr 2022 19:17:11 GMT  
		Size: 41.7 MB (41730222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e23c5ffb616fb8979712f573ce76a21ff2948ffe3c222f25abeda1b044fb82`  
		Last Modified: Tue, 05 Apr 2022 19:16:49 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:287bbe458761ddf7b90152156bcfcf1680e8229b94e87c6be21fcdcff4105325
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51100328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb806b4ff6eae8a70eec669d64a63205e9fa899f74021c50544a8a3fe8492216`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:24:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 07:25:05 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 07:25:05 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 07:25:07 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 07:25:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 07:25:08 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 07:25:09 GMT
CMD []
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c097d0722cedf772b294574bd3df3ea7bc3fd2a7f0d584bdda75906ab4a4f76`  
		Last Modified: Tue, 05 Apr 2022 07:26:39 GMT  
		Size: 48.4 MB (48382460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2d05467662609f11c35127449028bdba318e2920842c0c49a157d72fd14d4`  
		Last Modified: Tue, 05 Apr 2022 07:26:32 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:8d9a98e8ebe8c794faad1ca62b64b1d0f5d50b4bdc61593272165af938c90e58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58550969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b86a5912210274cdd2be334341ab5c8a5cc8b98b8cacbf00d0bc3b61391b34`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:44:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 06:45:29 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 06:45:29 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 06:45:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:45:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 06:45:32 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 06:45:33 GMT
CMD []
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781285b91779b0524f4a4b362a85bf7ad3c11049ec60271bc351d3ea22722f55`  
		Last Modified: Tue, 05 Apr 2022 06:47:18 GMT  
		Size: 55.7 MB (55729277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ede4c98a857e7e2e4374c87b05da88e9cfa36a1b9d2261f338a8e4cc091689`  
		Last Modified: Tue, 05 Apr 2022 06:47:09 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:99fc715aa51f45f415d42e16933cfd6640741633a9df875d1be9c41bb5eea1e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48200204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afb3e6b26fed2aaed2bdf33c3edb6718410d71cdda8521c1e6a42a745e020d3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:52:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 10:53:50 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 10:53:55 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 10:53:56 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:53:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 10:54:00 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 10:54:02 GMT
CMD []
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7876f582583c6ce1dd934300234645dd5b97252662a8c87fdfbf82c860328d90`  
		Last Modified: Tue, 05 Apr 2022 10:55:44 GMT  
		Size: 45.4 MB (45385557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bba04077c5c30296939df9ed09482547b8947d5decf08a738273fa064ca121a`  
		Last Modified: Tue, 05 Apr 2022 10:55:36 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:d23bba4fca1b0dd78c6f32996dd386b94a4944ac5ea047d049913f9f2c51e200
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113021b450dcbd4035fcfba58dd928217e0d39bff640b6d895c83e8eb2592df4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:12:32 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 06:13:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 06:13:13 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 06:13:13 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:13:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 06:13:13 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 06:13:13 GMT
CMD []
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df61fc68478458a071e8edf49185d9b224067a6e66831cdde802e5d2b66b097`  
		Last Modified: Tue, 05 Apr 2022 06:14:33 GMT  
		Size: 44.1 MB (44067532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829d58f668fddd7b5ed61e0d6c27f5b3abd19844eeb8ad111b395b944d064904`  
		Last Modified: Tue, 05 Apr 2022 06:14:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0.2`

```console
$ docker pull varnish@sha256:31f5e697661e5c97a7867e92755cefb5067f5177958c35fe38ca0e4be8fd3dec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0.2` - linux; amd64

```console
$ docker pull varnish@sha256:80ca9c3ffd61c95e2e3bd468c5906e862e51052636ad1105793018e8d74e9e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101190038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1d0d3f5afe71b234b6dce0b66cfade308ae48e137821cf3cdcdba874199813`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:06:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 15:06:39 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:06:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:06:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:06:40 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:06:40 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de66ed810206b73e0c9dab04edcb5ee5e063727b6d2d4288dcacf0b689f442`  
		Last Modified: Tue, 12 Jul 2022 15:10:08 GMT  
		Size: 69.8 MB (69822955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e847f66816c3e7530bb53d396f9f98bfe1dcb263d37ca0a260ceebccaa19563d`  
		Last Modified: Tue, 12 Jul 2022 15:09:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ef8ee948db46e978034b3e527028c92fb71d2ada0c428b60fd0dd6b5607220c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77822750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2c92def99b9454e428b38b30569a93a8227b85b3f9b4728202cf1dcd9fe007`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:49:30 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 13:55:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 24 Jun 2022 13:55:16 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 13:55:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 13:55:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 13:55:17 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 13:55:17 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87d17e6a126e6e5cda5556cd2a907d0ea8de0abc5a0db774bd93da779ed14e5`  
		Last Modified: Fri, 24 Jun 2022 14:04:17 GMT  
		Size: 51.2 MB (51246170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1253653c109b75569f3681144b8051d73b43acba27dbfc05aa2efb3cb6d0c6`  
		Last Modified: Fri, 24 Jun 2022 14:03:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:6498c5ad6d682b0076a0cbec21fef553b379504c201a87f0f7b5f14f80e9c60c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95301932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e738a742894266ad16f79ecd4b9a3474041d4f12dbfb804dff57c7a5d2db21`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:18:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:21:07 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 14:21:07 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:21:09 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:21:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:21:10 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:21:11 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e13c66f23d97c682dfc6fca33c4ba85b04f2b9b22f0a9d4a32679def5baa25b`  
		Last Modified: Tue, 12 Jul 2022 14:25:10 GMT  
		Size: 65.2 MB (65247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e12339074edaf212e4dc9334de848255f4ef5e943ff9e7833cc7e9b636d52b4`  
		Last Modified: Tue, 12 Jul 2022 14:25:01 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; 386

```console
$ docker pull varnish@sha256:ec9290335f55e308e7023f5d8f4972eebc2b1ee671069d8820851417cc0f17df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102585121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b122adf5e34794ee172b03b3fab482bc31219a96195e1e8c300c8ae4cb9d064c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:15:19 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 00:17:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 00:17:34 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 00:17:36 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:17:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 00:17:37 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 00:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf3f822dbf481370990594e81803141573a456e04899ad82fe6c4022627ebb`  
		Last Modified: Tue, 07 Jun 2022 00:21:08 GMT  
		Size: 70.2 MB (70194327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7dae54c84b4938c9aaa05092d4faf306897f47702a337f22ca87439181cc5`  
		Last Modified: Tue, 07 Jun 2022 00:20:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; ppc64le

```console
$ docker pull varnish@sha256:2e3c1ac9eacb11fab6237bcd3eff4d406e0b300e5c3144e3934ddf939b4e277c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100378186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b130ac9ed26512fd8cddaf8489ddf70922771377f7b1d009ba5e2de0dd5d960`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:38:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 06:55:41 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 06:55:47 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 06:55:48 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:55:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 06:55:55 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 06:56:00 GMT
CMD []
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c63706549952669ea4fc52e3a012cb12b690358fdde6057b825e1f21313259d`  
		Last Modified: Tue, 07 Jun 2022 07:15:28 GMT  
		Size: 65.1 MB (65091015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe199e856d7bedadb8a4da892a5d774b9146e8358d8909a62fadd06dbce3022b`  
		Last Modified: Tue, 07 Jun 2022 07:15:16 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; s390x

```console
$ docker pull varnish@sha256:4b16cb3b466bbe809c4833e2631cd4a9ddf572227e11c2fb3ce158a52465a752
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81623472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426be98166563a81501f737bf7edd9103507a566117a5395e75a6d54d80ada03`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:13:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:19:47 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 19:19:57 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:19:57 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:19:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:19:59 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:20:00 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f44713e40e8cd034f4c8f4dd815e5302835db628ffb0d6f606de6a30b3e909c`  
		Last Modified: Tue, 12 Jul 2022 19:28:33 GMT  
		Size: 52.0 MB (51982789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a43b712b028475ec29bca3a805cc61d86ec779b321fcd68dcdf093c4f9cfc1e`  
		Last Modified: Tue, 12 Jul 2022 19:28:25 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0.2-alpine`

```console
$ docker pull varnish@sha256:a96966b666c3eb795b5a5ffe4b7f1911e009156774d5551a355de6ba17dd6ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.0.2-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:1f798a786c909e75214591ae7bb11711b606d19904771e17cac071e3fc945f23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58347562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f303a05efad59d4625679d65998e25ac6af2a5a1e8e761d6165038faf0af7a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:46:19 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 09:47:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 09:47:16 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 09:47:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:47:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 09:47:16 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 09:47:16 GMT
CMD []
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd49c5f702ffa093526e350e19af19adacee36ebd21a4d2b8215729aebd24701`  
		Last Modified: Tue, 05 Apr 2022 09:48:23 GMT  
		Size: 55.5 MB (55528711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b11f3cacc52df447f6e49ab5dcad0b25a3e95d3aa5ca786c8a00b94bcea4d97`  
		Last Modified: Tue, 05 Apr 2022 09:48:15 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:d0ef8137631136de68aa9ca8b5a1c202753588e4823091fc74c7381800475e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44158672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b498faee8096b05f4ad1e1a034d79076f1405006bbb01cdc1b62443d19faf0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:12:30 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 19:13:58 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 19:13:59 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 19:13:59 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 19:14:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 19:14:00 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 19:14:00 GMT
CMD []
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a122a3f3e3f4f262ecd7c937fb5b761d7c7025f6b85195b6f6e59efccc3e22`  
		Last Modified: Tue, 05 Apr 2022 19:17:11 GMT  
		Size: 41.7 MB (41730222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e23c5ffb616fb8979712f573ce76a21ff2948ffe3c222f25abeda1b044fb82`  
		Last Modified: Tue, 05 Apr 2022 19:16:49 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:287bbe458761ddf7b90152156bcfcf1680e8229b94e87c6be21fcdcff4105325
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51100328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb806b4ff6eae8a70eec669d64a63205e9fa899f74021c50544a8a3fe8492216`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:24:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 07:25:05 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 07:25:05 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 07:25:07 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 07:25:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 07:25:08 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 07:25:09 GMT
CMD []
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c097d0722cedf772b294574bd3df3ea7bc3fd2a7f0d584bdda75906ab4a4f76`  
		Last Modified: Tue, 05 Apr 2022 07:26:39 GMT  
		Size: 48.4 MB (48382460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2d05467662609f11c35127449028bdba318e2920842c0c49a157d72fd14d4`  
		Last Modified: Tue, 05 Apr 2022 07:26:32 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; 386

```console
$ docker pull varnish@sha256:8d9a98e8ebe8c794faad1ca62b64b1d0f5d50b4bdc61593272165af938c90e58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58550969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b86a5912210274cdd2be334341ab5c8a5cc8b98b8cacbf00d0bc3b61391b34`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:44:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 06:45:29 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 06:45:29 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 06:45:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:45:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 06:45:32 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 06:45:33 GMT
CMD []
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781285b91779b0524f4a4b362a85bf7ad3c11049ec60271bc351d3ea22722f55`  
		Last Modified: Tue, 05 Apr 2022 06:47:18 GMT  
		Size: 55.7 MB (55729277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ede4c98a857e7e2e4374c87b05da88e9cfa36a1b9d2261f338a8e4cc091689`  
		Last Modified: Tue, 05 Apr 2022 06:47:09 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:99fc715aa51f45f415d42e16933cfd6640741633a9df875d1be9c41bb5eea1e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48200204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afb3e6b26fed2aaed2bdf33c3edb6718410d71cdda8521c1e6a42a745e020d3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:52:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 10:53:50 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 10:53:55 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 10:53:56 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:53:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 10:54:00 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 10:54:02 GMT
CMD []
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7876f582583c6ce1dd934300234645dd5b97252662a8c87fdfbf82c860328d90`  
		Last Modified: Tue, 05 Apr 2022 10:55:44 GMT  
		Size: 45.4 MB (45385557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bba04077c5c30296939df9ed09482547b8947d5decf08a738273fa064ca121a`  
		Last Modified: Tue, 05 Apr 2022 10:55:36 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:d23bba4fca1b0dd78c6f32996dd386b94a4944ac5ea047d049913f9f2c51e200
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113021b450dcbd4035fcfba58dd928217e0d39bff640b6d895c83e8eb2592df4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:12:32 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 06:13:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 06:13:13 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 06:13:13 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:13:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 06:13:13 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 06:13:13 GMT
CMD []
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df61fc68478458a071e8edf49185d9b224067a6e66831cdde802e5d2b66b097`  
		Last Modified: Tue, 05 Apr 2022 06:14:33 GMT  
		Size: 44.1 MB (44067532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829d58f668fddd7b5ed61e0d6c27f5b3abd19844eeb8ad111b395b944d064904`  
		Last Modified: Tue, 05 Apr 2022 06:14:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1`

```console
$ docker pull varnish@sha256:0dac8cd2294800958f85dfa015b61c12a032fb936c8e3fb92c3ad84c524fa262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1` - linux; amd64

```console
$ docker pull varnish@sha256:dd353c4858b5d068b7999fece56dbdf99fb99a85121250ede66c38167cdefb20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105351648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5268f906b30a2228c6a6388bd4e44f63850541c06257235a9fced4f0e063ec1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:01:15 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 15:01:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 15:01:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:04:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 15:04:16 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:04:17 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:04:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:04:17 GMT
USER varnish
# Tue, 12 Jul 2022 15:04:17 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:04:17 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961c99130da012333143f927891961c27ef1116f0090d8bf533fd840c0b9c74`  
		Last Modified: Tue, 12 Jul 2022 15:09:42 GMT  
		Size: 74.0 MB (73984565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b13cb4c26815a73af08a7ddc35a353fa0f5cb726ac8793d92d2e1d268e853`  
		Last Modified: Tue, 12 Jul 2022 15:09:31 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:13ee5653f822aed1718ef1cf487e4e25f0e2e399e08c021c59a04020bc559a68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81967205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62f1c8d52f6a1feed9a6c2cfd4638a0b148af3dedf3477d5b9db1cf1bd6040c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:41:54 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 13:41:55 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 13:41:55 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 13:41:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 13:41:58 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 13:41:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 13:49:02 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 13:49:03 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 13:49:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 13:49:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 13:49:04 GMT
USER varnish
# Fri, 24 Jun 2022 13:49:05 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 13:49:05 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafa03e57ec05360bf1ec882cbcd696b29942c47bbc4075891dbda3a6055ae9`  
		Last Modified: Fri, 24 Jun 2022 14:03:23 GMT  
		Size: 55.4 MB (55390624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dba669521b3b8d73bdf6969d2650d63159714b743cca40914d359d29a4e6dd2`  
		Last Modified: Fri, 24 Jun 2022 14:02:53 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:18a0523836e220ffb590bc76e8425a0e990ab942917bbd414c699e6fc897d447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99457561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9748f8eed1f5fe15de9eb3eab3e839ec48174edc8e318492b65e73acc05c008`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:15:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 14:15:28 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 14:15:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 14:15:30 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 14:15:31 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 14:15:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 14:15:33 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 14:15:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 14:15:35 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 14:15:36 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 14:15:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:18:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 14:18:30 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:18:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:18:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:18:33 GMT
USER varnish
# Tue, 12 Jul 2022 14:18:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:18:35 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1772ed21321e42f4a7653248dbcb45757b708f882b1f730d1d1edf80c69cb304`  
		Last Modified: Tue, 12 Jul 2022 14:24:41 GMT  
		Size: 69.4 MB (69402860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713cb83db0566be9810b152d08899074408929cc378d72ab71e6e940f95d14e6`  
		Last Modified: Tue, 12 Jul 2022 14:24:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; 386

```console
$ docker pull varnish@sha256:789b73487c4c3c2758a95df1769312f0c0161c6f29267b05268dd74d75483786
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106710623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76032fc1a132fb41031505a50c33160c7b2f45994572b72ace759fb897fbe7e1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:12:40 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 10:12:41 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 10:12:42 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 10:12:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 10:12:44 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 10:12:45 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 10:12:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 10:12:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 10:12:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 10:12:49 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 10:12:50 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 10:15:37 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 10:15:37 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 10:15:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:15:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 10:15:40 GMT
USER varnish
# Tue, 12 Jul 2022 10:15:41 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 10:15:42 GMT
CMD []
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18191750ecd3a1593c9604678a9dec2a16833252b74152865ff36a28a27a6222`  
		Last Modified: Tue, 12 Jul 2022 10:19:52 GMT  
		Size: 74.3 MB (74336200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3225164b08fe2beb56664a2953cb5691cacf11ff9f2cf81e2b85b1e4e0e5ca1`  
		Last Modified: Tue, 12 Jul 2022 10:19:41 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:173b2c7cb38627e42689f13efdf92ca1bc1d020321376c4af6ba13d485aa62bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104551258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d16850a5f77422730f61d747d46e86efa0eb6caea92c0a9764de9640adccd1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:24:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 03:24:06 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 03:24:09 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 03:24:12 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 03:24:14 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 03:24:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 03:24:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 03:24:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 03:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 03:24:47 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 03:24:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 03:56:06 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 03:56:13 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 03:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:56:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 03:56:21 GMT
USER varnish
# Fri, 24 Jun 2022 03:56:23 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 03:56:26 GMT
CMD []
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fdb1ad92808fd81a71e3af63882ad100769b32bcc0716f66d9bf9e0151440`  
		Last Modified: Fri, 24 Jun 2022 03:59:34 GMT  
		Size: 69.3 MB (69263959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0bb90a9b290228ab1938c4e50eec94c34c8f55cc20c2a5e7a597813f28a13`  
		Last Modified: Fri, 24 Jun 2022 03:59:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; s390x

```console
$ docker pull varnish@sha256:30d950ea8c839993bdbb480d94dc13dcfe0c373b11311b4c52e0f72d71c2ec95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85780988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd57ebebc1fdf2b03941e22a350ef6f1df7d70e137d94738955242147ff25d15`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:06:21 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 19:06:22 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 19:06:23 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 19:06:23 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 19:06:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 19:06:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 19:06:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 19:06:27 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 19:06:28 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:13:24 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 19:13:32 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:13:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:13:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:13:34 GMT
USER varnish
# Tue, 12 Jul 2022 19:13:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:13:35 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06561947f6199b7f782a535d09351d41e6435f8bb103b2eab4390f031f333343`  
		Last Modified: Tue, 12 Jul 2022 19:28:04 GMT  
		Size: 56.1 MB (56140308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62677499f8b6b5b494ce7853458111556bc115a949c95098401362f8ef4a7255`  
		Last Modified: Tue, 12 Jul 2022 19:27:56 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1-alpine`

```console
$ docker pull varnish@sha256:9343884f6ab3ad4ad61644d7567b8becef3dd2344e9b22e572a8f1128f757a4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:81397424691b539bc850f20254af04c34cae93a5ec485c3d8339eb9b138dd2f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59100484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c410d76e4ae50504580f78c53148ba1e62fb8d27e1e4a1a2f98d3cde5a289e0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:44:24 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 22:10:26 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 22:11:41 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 22:11:41 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 22:11:41 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 22:11:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 22:11:41 GMT
USER varnish
# Thu, 21 Apr 2022 22:11:41 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 22:11:42 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab0de482a12061e292d208c300acfef4b7903ad36dc4fb177fc61b76f6d7e1a`  
		Last Modified: Thu, 21 Apr 2022 22:13:00 GMT  
		Size: 56.3 MB (56285443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fdb9a66b68029729002c46951f2c45aa31e27860321211a5aac411173bdc8f`  
		Last Modified: Thu, 21 Apr 2022 22:12:52 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:d0a19c4c194556f862a2019c23115bef09d27470e8c93a477ef67996fdfb8cf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44859131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e119e145cf9077541d90985f02df7b5ec99a761ddb73c41e93cdd09238106cf3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:09:14 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 19:09:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 21:38:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 21:41:18 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 21:41:19 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 21:41:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 21:41:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 21:41:20 GMT
USER varnish
# Fri, 22 Apr 2022 21:41:21 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 21:41:21 GMT
CMD []
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79967e8d87646f19a1a9b9742f95266b7c04f20de140ac6cdc8e06ddefc7c3f6`  
		Last Modified: Fri, 22 Apr 2022 21:50:16 GMT  
		Size: 42.4 MB (42434328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb6a24e91ed133ff7d032cd6bdff4025615b86c24190904178eb3bf6f57a2a4`  
		Last Modified: Fri, 22 Apr 2022 21:49:54 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4baf57565dc415a17a031897b6ba12546044b510b9260fe92806a0ce17d22b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca13aff345b38cd131a7f99e198b99d739d007f09d7977dabc789bdbc1f4480`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:22:16 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 07:22:17 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 07:22:18 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 07:22:19 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 07:22:20 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 07:22:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:43:49 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:43:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:43:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:43:52 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:43:53 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:45:14 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:45:14 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:45:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:45:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:45:17 GMT
USER varnish
# Thu, 21 Apr 2022 20:45:18 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:45:19 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53648c9db1a4f4013c5d44e9fd4577e839980908f0dca7a76d3c8efad06d048`  
		Last Modified: Thu, 21 Apr 2022 20:47:24 GMT  
		Size: 49.1 MB (49113769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0a30b3f6f66f585ac84b9bf017f0e7975a34fd479b9701a245f950742ad5b`  
		Last Modified: Thu, 21 Apr 2022 20:47:17 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:de6628a1837145901ad6a52437bd103285f7830c8aa27203eea30f716f01dbe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59292895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09ff39c7c861e7ca0f001f5e542ba94c66a520216bf35e15659ec0c23ba09b8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:42:43 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:42:44 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:42:45 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:42:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:42:47 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:42:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:42:09 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:42:10 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:42:11 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:43:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:43:30 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:43:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:43:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:43:33 GMT
USER varnish
# Thu, 21 Apr 2022 20:43:34 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:43:35 GMT
CMD []
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34115bd677f7c2afb67705f651ff60b689e7a3a69b0cd15a60e3d836a0162e18`  
		Last Modified: Thu, 21 Apr 2022 20:45:21 GMT  
		Size: 56.5 MB (56473443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e121fe38cf19136053915fbb7f2d88e8c3702004736c435aa530245164896`  
		Last Modified: Thu, 21 Apr 2022 20:45:07 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:cf82764a27a365286573acdc67c5995b11030a4fc3184f8124b1645f761b3b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48896574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f3ce1cef6fa74ddc30bc42b6967d168c0174d0c06953c3955dbf10e6da9e8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:48:31 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 10:48:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 10:48:35 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 10:48:37 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 10:48:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 10:48:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 07:13:28 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 07:13:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 07:13:32 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 07:13:35 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 07:13:38 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 07:15:35 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 07:15:41 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 07:15:45 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 07:15:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 07:15:53 GMT
USER varnish
# Fri, 22 Apr 2022 07:15:55 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 07:15:58 GMT
CMD []
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87322051143de85e675a2374befd084c589471c31ae811a63f81690eb82180`  
		Last Modified: Fri, 22 Apr 2022 07:17:52 GMT  
		Size: 46.1 MB (46084905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c270534ccc583852361368fa7e4845ad3b6b16be4280d08c8edb428e390cf`  
		Last Modified: Fri, 22 Apr 2022 07:17:44 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:10414a54f8108d64836a2c9c6c865e5f9ebe6123647c3ee57867ced916313f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47350962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac56919f84b42f704fd7cfaaffe0a712aff857fbe24d7a894d9d4156d8c8b6a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:10:53 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:44:53 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:44:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:44:54 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:46:21 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:46:22 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:46:23 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:46:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:46:23 GMT
USER varnish
# Thu, 21 Apr 2022 20:46:23 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:46:23 GMT
CMD []
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a48f1c01887a27a97e883fdd3fad9fb57c191e26cc389b076ad6ce3abe007`  
		Last Modified: Thu, 21 Apr 2022 20:48:28 GMT  
		Size: 44.8 MB (44750107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c99d1795f78de1f9b33331b3ee9178f8fa9622b60f90d85b5292655323e272`  
		Last Modified: Thu, 21 Apr 2022 20:48:23 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.0`

```console
$ docker pull varnish@sha256:0dac8cd2294800958f85dfa015b61c12a032fb936c8e3fb92c3ad84c524fa262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1.0` - linux; amd64

```console
$ docker pull varnish@sha256:dd353c4858b5d068b7999fece56dbdf99fb99a85121250ede66c38167cdefb20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105351648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5268f906b30a2228c6a6388bd4e44f63850541c06257235a9fced4f0e063ec1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:01:15 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 15:01:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 15:01:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:04:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 15:04:16 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:04:17 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:04:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:04:17 GMT
USER varnish
# Tue, 12 Jul 2022 15:04:17 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:04:17 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961c99130da012333143f927891961c27ef1116f0090d8bf533fd840c0b9c74`  
		Last Modified: Tue, 12 Jul 2022 15:09:42 GMT  
		Size: 74.0 MB (73984565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b13cb4c26815a73af08a7ddc35a353fa0f5cb726ac8793d92d2e1d268e853`  
		Last Modified: Tue, 12 Jul 2022 15:09:31 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:13ee5653f822aed1718ef1cf487e4e25f0e2e399e08c021c59a04020bc559a68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81967205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62f1c8d52f6a1feed9a6c2cfd4638a0b148af3dedf3477d5b9db1cf1bd6040c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:41:54 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 13:41:55 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 13:41:55 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 13:41:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 13:41:58 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 13:41:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 13:49:02 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 13:49:03 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 13:49:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 13:49:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 13:49:04 GMT
USER varnish
# Fri, 24 Jun 2022 13:49:05 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 13:49:05 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafa03e57ec05360bf1ec882cbcd696b29942c47bbc4075891dbda3a6055ae9`  
		Last Modified: Fri, 24 Jun 2022 14:03:23 GMT  
		Size: 55.4 MB (55390624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dba669521b3b8d73bdf6969d2650d63159714b743cca40914d359d29a4e6dd2`  
		Last Modified: Fri, 24 Jun 2022 14:02:53 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:18a0523836e220ffb590bc76e8425a0e990ab942917bbd414c699e6fc897d447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99457561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9748f8eed1f5fe15de9eb3eab3e839ec48174edc8e318492b65e73acc05c008`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:15:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 14:15:28 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 14:15:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 14:15:30 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 14:15:31 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 14:15:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 14:15:33 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 14:15:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 14:15:35 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 14:15:36 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 14:15:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:18:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 14:18:30 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:18:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:18:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:18:33 GMT
USER varnish
# Tue, 12 Jul 2022 14:18:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:18:35 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1772ed21321e42f4a7653248dbcb45757b708f882b1f730d1d1edf80c69cb304`  
		Last Modified: Tue, 12 Jul 2022 14:24:41 GMT  
		Size: 69.4 MB (69402860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713cb83db0566be9810b152d08899074408929cc378d72ab71e6e940f95d14e6`  
		Last Modified: Tue, 12 Jul 2022 14:24:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0` - linux; 386

```console
$ docker pull varnish@sha256:789b73487c4c3c2758a95df1769312f0c0161c6f29267b05268dd74d75483786
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106710623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76032fc1a132fb41031505a50c33160c7b2f45994572b72ace759fb897fbe7e1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:12:40 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 10:12:41 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 10:12:42 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 10:12:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 10:12:44 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 10:12:45 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 10:12:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 10:12:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 10:12:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 10:12:49 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 10:12:50 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 10:15:37 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 10:15:37 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 10:15:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:15:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 10:15:40 GMT
USER varnish
# Tue, 12 Jul 2022 10:15:41 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 10:15:42 GMT
CMD []
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18191750ecd3a1593c9604678a9dec2a16833252b74152865ff36a28a27a6222`  
		Last Modified: Tue, 12 Jul 2022 10:19:52 GMT  
		Size: 74.3 MB (74336200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3225164b08fe2beb56664a2953cb5691cacf11ff9f2cf81e2b85b1e4e0e5ca1`  
		Last Modified: Tue, 12 Jul 2022 10:19:41 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:173b2c7cb38627e42689f13efdf92ca1bc1d020321376c4af6ba13d485aa62bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104551258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d16850a5f77422730f61d747d46e86efa0eb6caea92c0a9764de9640adccd1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:24:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 03:24:06 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 03:24:09 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 03:24:12 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 03:24:14 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 03:24:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 03:24:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 03:24:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 03:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 03:24:47 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 03:24:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 03:56:06 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 03:56:13 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 03:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:56:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 03:56:21 GMT
USER varnish
# Fri, 24 Jun 2022 03:56:23 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 03:56:26 GMT
CMD []
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fdb1ad92808fd81a71e3af63882ad100769b32bcc0716f66d9bf9e0151440`  
		Last Modified: Fri, 24 Jun 2022 03:59:34 GMT  
		Size: 69.3 MB (69263959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0bb90a9b290228ab1938c4e50eec94c34c8f55cc20c2a5e7a597813f28a13`  
		Last Modified: Fri, 24 Jun 2022 03:59:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0` - linux; s390x

```console
$ docker pull varnish@sha256:30d950ea8c839993bdbb480d94dc13dcfe0c373b11311b4c52e0f72d71c2ec95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85780988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd57ebebc1fdf2b03941e22a350ef6f1df7d70e137d94738955242147ff25d15`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:06:21 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 19:06:22 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 19:06:23 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 19:06:23 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 19:06:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 19:06:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 19:06:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 19:06:27 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 19:06:28 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:13:24 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 19:13:32 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:13:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:13:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:13:34 GMT
USER varnish
# Tue, 12 Jul 2022 19:13:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:13:35 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06561947f6199b7f782a535d09351d41e6435f8bb103b2eab4390f031f333343`  
		Last Modified: Tue, 12 Jul 2022 19:28:04 GMT  
		Size: 56.1 MB (56140308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62677499f8b6b5b494ce7853458111556bc115a949c95098401362f8ef4a7255`  
		Last Modified: Tue, 12 Jul 2022 19:27:56 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.0-alpine`

```console
$ docker pull varnish@sha256:9343884f6ab3ad4ad61644d7567b8becef3dd2344e9b22e572a8f1128f757a4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1.0-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:81397424691b539bc850f20254af04c34cae93a5ec485c3d8339eb9b138dd2f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59100484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c410d76e4ae50504580f78c53148ba1e62fb8d27e1e4a1a2f98d3cde5a289e0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:44:24 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 22:10:26 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 22:11:41 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 22:11:41 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 22:11:41 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 22:11:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 22:11:41 GMT
USER varnish
# Thu, 21 Apr 2022 22:11:41 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 22:11:42 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab0de482a12061e292d208c300acfef4b7903ad36dc4fb177fc61b76f6d7e1a`  
		Last Modified: Thu, 21 Apr 2022 22:13:00 GMT  
		Size: 56.3 MB (56285443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fdb9a66b68029729002c46951f2c45aa31e27860321211a5aac411173bdc8f`  
		Last Modified: Thu, 21 Apr 2022 22:12:52 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:d0a19c4c194556f862a2019c23115bef09d27470e8c93a477ef67996fdfb8cf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44859131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e119e145cf9077541d90985f02df7b5ec99a761ddb73c41e93cdd09238106cf3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:09:14 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 19:09:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 21:38:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 21:41:18 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 21:41:19 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 21:41:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 21:41:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 21:41:20 GMT
USER varnish
# Fri, 22 Apr 2022 21:41:21 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 21:41:21 GMT
CMD []
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79967e8d87646f19a1a9b9742f95266b7c04f20de140ac6cdc8e06ddefc7c3f6`  
		Last Modified: Fri, 22 Apr 2022 21:50:16 GMT  
		Size: 42.4 MB (42434328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb6a24e91ed133ff7d032cd6bdff4025615b86c24190904178eb3bf6f57a2a4`  
		Last Modified: Fri, 22 Apr 2022 21:49:54 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4baf57565dc415a17a031897b6ba12546044b510b9260fe92806a0ce17d22b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca13aff345b38cd131a7f99e198b99d739d007f09d7977dabc789bdbc1f4480`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:22:16 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 07:22:17 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 07:22:18 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 07:22:19 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 07:22:20 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 07:22:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:43:49 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:43:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:43:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:43:52 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:43:53 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:45:14 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:45:14 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:45:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:45:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:45:17 GMT
USER varnish
# Thu, 21 Apr 2022 20:45:18 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:45:19 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53648c9db1a4f4013c5d44e9fd4577e839980908f0dca7a76d3c8efad06d048`  
		Last Modified: Thu, 21 Apr 2022 20:47:24 GMT  
		Size: 49.1 MB (49113769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0a30b3f6f66f585ac84b9bf017f0e7975a34fd479b9701a245f950742ad5b`  
		Last Modified: Thu, 21 Apr 2022 20:47:17 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:de6628a1837145901ad6a52437bd103285f7830c8aa27203eea30f716f01dbe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59292895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09ff39c7c861e7ca0f001f5e542ba94c66a520216bf35e15659ec0c23ba09b8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:42:43 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:42:44 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:42:45 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:42:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:42:47 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:42:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:42:09 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:42:10 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:42:11 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:43:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:43:30 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:43:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:43:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:43:33 GMT
USER varnish
# Thu, 21 Apr 2022 20:43:34 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:43:35 GMT
CMD []
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34115bd677f7c2afb67705f651ff60b689e7a3a69b0cd15a60e3d836a0162e18`  
		Last Modified: Thu, 21 Apr 2022 20:45:21 GMT  
		Size: 56.5 MB (56473443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e121fe38cf19136053915fbb7f2d88e8c3702004736c435aa530245164896`  
		Last Modified: Thu, 21 Apr 2022 20:45:07 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:cf82764a27a365286573acdc67c5995b11030a4fc3184f8124b1645f761b3b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48896574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f3ce1cef6fa74ddc30bc42b6967d168c0174d0c06953c3955dbf10e6da9e8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:48:31 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 10:48:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 10:48:35 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 10:48:37 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 10:48:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 10:48:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 07:13:28 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 07:13:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 07:13:32 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 07:13:35 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 07:13:38 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 07:15:35 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 07:15:41 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 07:15:45 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 07:15:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 07:15:53 GMT
USER varnish
# Fri, 22 Apr 2022 07:15:55 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 07:15:58 GMT
CMD []
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87322051143de85e675a2374befd084c589471c31ae811a63f81690eb82180`  
		Last Modified: Fri, 22 Apr 2022 07:17:52 GMT  
		Size: 46.1 MB (46084905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c270534ccc583852361368fa7e4845ad3b6b16be4280d08c8edb428e390cf`  
		Last Modified: Fri, 22 Apr 2022 07:17:44 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:10414a54f8108d64836a2c9c6c865e5f9ebe6123647c3ee57867ced916313f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47350962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac56919f84b42f704fd7cfaaffe0a712aff857fbe24d7a894d9d4156d8c8b6a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:10:53 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:44:53 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:44:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:44:54 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:46:21 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:46:22 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:46:23 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:46:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:46:23 GMT
USER varnish
# Thu, 21 Apr 2022 20:46:23 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:46:23 GMT
CMD []
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a48f1c01887a27a97e883fdd3fad9fb57c191e26cc389b076ad6ce3abe007`  
		Last Modified: Thu, 21 Apr 2022 20:48:28 GMT  
		Size: 44.8 MB (44750107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c99d1795f78de1f9b33331b3ee9178f8fa9622b60f90d85b5292655323e272`  
		Last Modified: Thu, 21 Apr 2022 20:48:23 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:9343884f6ab3ad4ad61644d7567b8becef3dd2344e9b22e572a8f1128f757a4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:alpine` - linux; amd64

```console
$ docker pull varnish@sha256:81397424691b539bc850f20254af04c34cae93a5ec485c3d8339eb9b138dd2f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59100484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c410d76e4ae50504580f78c53148ba1e62fb8d27e1e4a1a2f98d3cde5a289e0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:44:24 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 22:10:26 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 22:11:41 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 22:11:41 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 22:11:41 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 22:11:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 22:11:41 GMT
USER varnish
# Thu, 21 Apr 2022 22:11:41 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 22:11:42 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab0de482a12061e292d208c300acfef4b7903ad36dc4fb177fc61b76f6d7e1a`  
		Last Modified: Thu, 21 Apr 2022 22:13:00 GMT  
		Size: 56.3 MB (56285443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fdb9a66b68029729002c46951f2c45aa31e27860321211a5aac411173bdc8f`  
		Last Modified: Thu, 21 Apr 2022 22:12:52 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:d0a19c4c194556f862a2019c23115bef09d27470e8c93a477ef67996fdfb8cf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44859131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e119e145cf9077541d90985f02df7b5ec99a761ddb73c41e93cdd09238106cf3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:09:14 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 19:09:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 21:38:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 21:41:18 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 21:41:19 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 21:41:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 21:41:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 21:41:20 GMT
USER varnish
# Fri, 22 Apr 2022 21:41:21 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 21:41:21 GMT
CMD []
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79967e8d87646f19a1a9b9742f95266b7c04f20de140ac6cdc8e06ddefc7c3f6`  
		Last Modified: Fri, 22 Apr 2022 21:50:16 GMT  
		Size: 42.4 MB (42434328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb6a24e91ed133ff7d032cd6bdff4025615b86c24190904178eb3bf6f57a2a4`  
		Last Modified: Fri, 22 Apr 2022 21:49:54 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4baf57565dc415a17a031897b6ba12546044b510b9260fe92806a0ce17d22b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca13aff345b38cd131a7f99e198b99d739d007f09d7977dabc789bdbc1f4480`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:22:16 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 07:22:17 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 07:22:18 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 07:22:19 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 07:22:20 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 07:22:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:43:49 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:43:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:43:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:43:52 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:43:53 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:45:14 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:45:14 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:45:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:45:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:45:17 GMT
USER varnish
# Thu, 21 Apr 2022 20:45:18 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:45:19 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53648c9db1a4f4013c5d44e9fd4577e839980908f0dca7a76d3c8efad06d048`  
		Last Modified: Thu, 21 Apr 2022 20:47:24 GMT  
		Size: 49.1 MB (49113769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0a30b3f6f66f585ac84b9bf017f0e7975a34fd479b9701a245f950742ad5b`  
		Last Modified: Thu, 21 Apr 2022 20:47:17 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:de6628a1837145901ad6a52437bd103285f7830c8aa27203eea30f716f01dbe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59292895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09ff39c7c861e7ca0f001f5e542ba94c66a520216bf35e15659ec0c23ba09b8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:42:43 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:42:44 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:42:45 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:42:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:42:47 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:42:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:42:09 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:42:10 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:42:11 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:43:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:43:30 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:43:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:43:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:43:33 GMT
USER varnish
# Thu, 21 Apr 2022 20:43:34 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:43:35 GMT
CMD []
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34115bd677f7c2afb67705f651ff60b689e7a3a69b0cd15a60e3d836a0162e18`  
		Last Modified: Thu, 21 Apr 2022 20:45:21 GMT  
		Size: 56.5 MB (56473443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e121fe38cf19136053915fbb7f2d88e8c3702004736c435aa530245164896`  
		Last Modified: Thu, 21 Apr 2022 20:45:07 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:cf82764a27a365286573acdc67c5995b11030a4fc3184f8124b1645f761b3b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48896574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f3ce1cef6fa74ddc30bc42b6967d168c0174d0c06953c3955dbf10e6da9e8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:48:31 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 10:48:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 10:48:35 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 10:48:37 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 10:48:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 10:48:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 07:13:28 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 07:13:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 07:13:32 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 07:13:35 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 07:13:38 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 07:15:35 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 07:15:41 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 07:15:45 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 07:15:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 07:15:53 GMT
USER varnish
# Fri, 22 Apr 2022 07:15:55 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 07:15:58 GMT
CMD []
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87322051143de85e675a2374befd084c589471c31ae811a63f81690eb82180`  
		Last Modified: Fri, 22 Apr 2022 07:17:52 GMT  
		Size: 46.1 MB (46084905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c270534ccc583852361368fa7e4845ad3b6b16be4280d08c8edb428e390cf`  
		Last Modified: Fri, 22 Apr 2022 07:17:44 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:10414a54f8108d64836a2c9c6c865e5f9ebe6123647c3ee57867ced916313f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47350962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac56919f84b42f704fd7cfaaffe0a712aff857fbe24d7a894d9d4156d8c8b6a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:10:53 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:44:53 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:44:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:44:54 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:46:21 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:46:22 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:46:23 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:46:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:46:23 GMT
USER varnish
# Thu, 21 Apr 2022 20:46:23 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:46:23 GMT
CMD []
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a48f1c01887a27a97e883fdd3fad9fb57c191e26cc389b076ad6ce3abe007`  
		Last Modified: Thu, 21 Apr 2022 20:48:28 GMT  
		Size: 44.8 MB (44750107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c99d1795f78de1f9b33331b3ee9178f8fa9622b60f90d85b5292655323e272`  
		Last Modified: Thu, 21 Apr 2022 20:48:23 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:0dac8cd2294800958f85dfa015b61c12a032fb936c8e3fb92c3ad84c524fa262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:dd353c4858b5d068b7999fece56dbdf99fb99a85121250ede66c38167cdefb20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105351648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5268f906b30a2228c6a6388bd4e44f63850541c06257235a9fced4f0e063ec1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:01:15 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 15:01:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 15:01:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:04:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 15:04:16 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:04:17 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:04:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:04:17 GMT
USER varnish
# Tue, 12 Jul 2022 15:04:17 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:04:17 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961c99130da012333143f927891961c27ef1116f0090d8bf533fd840c0b9c74`  
		Last Modified: Tue, 12 Jul 2022 15:09:42 GMT  
		Size: 74.0 MB (73984565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b13cb4c26815a73af08a7ddc35a353fa0f5cb726ac8793d92d2e1d268e853`  
		Last Modified: Tue, 12 Jul 2022 15:09:31 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:13ee5653f822aed1718ef1cf487e4e25f0e2e399e08c021c59a04020bc559a68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81967205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62f1c8d52f6a1feed9a6c2cfd4638a0b148af3dedf3477d5b9db1cf1bd6040c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:41:54 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 13:41:55 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 13:41:55 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 13:41:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 13:41:58 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 13:41:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 13:49:02 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 13:49:03 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 13:49:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 13:49:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 13:49:04 GMT
USER varnish
# Fri, 24 Jun 2022 13:49:05 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 13:49:05 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafa03e57ec05360bf1ec882cbcd696b29942c47bbc4075891dbda3a6055ae9`  
		Last Modified: Fri, 24 Jun 2022 14:03:23 GMT  
		Size: 55.4 MB (55390624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dba669521b3b8d73bdf6969d2650d63159714b743cca40914d359d29a4e6dd2`  
		Last Modified: Fri, 24 Jun 2022 14:02:53 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:18a0523836e220ffb590bc76e8425a0e990ab942917bbd414c699e6fc897d447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99457561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9748f8eed1f5fe15de9eb3eab3e839ec48174edc8e318492b65e73acc05c008`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:15:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 14:15:28 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 14:15:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 14:15:30 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 14:15:31 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 14:15:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 14:15:33 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 14:15:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 14:15:35 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 14:15:36 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 14:15:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:18:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 14:18:30 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:18:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:18:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:18:33 GMT
USER varnish
# Tue, 12 Jul 2022 14:18:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:18:35 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1772ed21321e42f4a7653248dbcb45757b708f882b1f730d1d1edf80c69cb304`  
		Last Modified: Tue, 12 Jul 2022 14:24:41 GMT  
		Size: 69.4 MB (69402860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713cb83db0566be9810b152d08899074408929cc378d72ab71e6e940f95d14e6`  
		Last Modified: Tue, 12 Jul 2022 14:24:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:789b73487c4c3c2758a95df1769312f0c0161c6f29267b05268dd74d75483786
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106710623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76032fc1a132fb41031505a50c33160c7b2f45994572b72ace759fb897fbe7e1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:12:40 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 10:12:41 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 10:12:42 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 10:12:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 10:12:44 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 10:12:45 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 10:12:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 10:12:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 10:12:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 10:12:49 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 10:12:50 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 10:15:37 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 10:15:37 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 10:15:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:15:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 10:15:40 GMT
USER varnish
# Tue, 12 Jul 2022 10:15:41 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 10:15:42 GMT
CMD []
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18191750ecd3a1593c9604678a9dec2a16833252b74152865ff36a28a27a6222`  
		Last Modified: Tue, 12 Jul 2022 10:19:52 GMT  
		Size: 74.3 MB (74336200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3225164b08fe2beb56664a2953cb5691cacf11ff9f2cf81e2b85b1e4e0e5ca1`  
		Last Modified: Tue, 12 Jul 2022 10:19:41 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:173b2c7cb38627e42689f13efdf92ca1bc1d020321376c4af6ba13d485aa62bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104551258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d16850a5f77422730f61d747d46e86efa0eb6caea92c0a9764de9640adccd1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:24:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 03:24:06 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 03:24:09 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 03:24:12 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 03:24:14 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 03:24:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 03:24:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 03:24:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 03:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 03:24:47 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 03:24:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 03:56:06 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 03:56:13 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 03:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:56:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 03:56:21 GMT
USER varnish
# Fri, 24 Jun 2022 03:56:23 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 03:56:26 GMT
CMD []
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fdb1ad92808fd81a71e3af63882ad100769b32bcc0716f66d9bf9e0151440`  
		Last Modified: Fri, 24 Jun 2022 03:59:34 GMT  
		Size: 69.3 MB (69263959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0bb90a9b290228ab1938c4e50eec94c34c8f55cc20c2a5e7a597813f28a13`  
		Last Modified: Fri, 24 Jun 2022 03:59:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:30d950ea8c839993bdbb480d94dc13dcfe0c373b11311b4c52e0f72d71c2ec95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85780988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd57ebebc1fdf2b03941e22a350ef6f1df7d70e137d94738955242147ff25d15`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:06:21 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 19:06:22 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 19:06:23 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 19:06:23 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 19:06:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 19:06:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 19:06:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 19:06:27 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 19:06:28 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:13:24 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 19:13:32 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:13:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:13:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:13:34 GMT
USER varnish
# Tue, 12 Jul 2022 19:13:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:13:35 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06561947f6199b7f782a535d09351d41e6435f8bb103b2eab4390f031f333343`  
		Last Modified: Tue, 12 Jul 2022 19:28:04 GMT  
		Size: 56.1 MB (56140308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62677499f8b6b5b494ce7853458111556bc115a949c95098401362f8ef4a7255`  
		Last Modified: Tue, 12 Jul 2022 19:27:56 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:9343884f6ab3ad4ad61644d7567b8becef3dd2344e9b22e572a8f1128f757a4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:fresh-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:81397424691b539bc850f20254af04c34cae93a5ec485c3d8339eb9b138dd2f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59100484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c410d76e4ae50504580f78c53148ba1e62fb8d27e1e4a1a2f98d3cde5a289e0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:44:24 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 09:44:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 22:10:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 22:10:26 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 22:10:26 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 22:11:41 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 22:11:41 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 22:11:41 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 22:11:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 22:11:41 GMT
USER varnish
# Thu, 21 Apr 2022 22:11:41 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 22:11:42 GMT
CMD []
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab0de482a12061e292d208c300acfef4b7903ad36dc4fb177fc61b76f6d7e1a`  
		Last Modified: Thu, 21 Apr 2022 22:13:00 GMT  
		Size: 56.3 MB (56285443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fdb9a66b68029729002c46951f2c45aa31e27860321211a5aac411173bdc8f`  
		Last Modified: Thu, 21 Apr 2022 22:12:52 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:d0a19c4c194556f862a2019c23115bef09d27470e8c93a477ef67996fdfb8cf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44859131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e119e145cf9077541d90985f02df7b5ec99a761ddb73c41e93cdd09238106cf3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:09:14 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 19:09:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 19:09:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 19:09:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 21:38:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 21:38:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 21:38:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 21:41:18 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 21:41:19 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 21:41:19 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 21:41:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 21:41:20 GMT
USER varnish
# Fri, 22 Apr 2022 21:41:21 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 21:41:21 GMT
CMD []
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79967e8d87646f19a1a9b9742f95266b7c04f20de140ac6cdc8e06ddefc7c3f6`  
		Last Modified: Fri, 22 Apr 2022 21:50:16 GMT  
		Size: 42.4 MB (42434328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb6a24e91ed133ff7d032cd6bdff4025615b86c24190904178eb3bf6f57a2a4`  
		Last Modified: Fri, 22 Apr 2022 21:49:54 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:4baf57565dc415a17a031897b6ba12546044b510b9260fe92806a0ce17d22b57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51830728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca13aff345b38cd131a7f99e198b99d739d007f09d7977dabc789bdbc1f4480`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:22:16 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 07:22:17 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 07:22:18 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 07:22:19 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 07:22:20 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 07:22:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:43:49 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:43:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:43:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:43:52 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:43:53 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:45:14 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:45:14 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:45:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:45:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:45:17 GMT
USER varnish
# Thu, 21 Apr 2022 20:45:18 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:45:19 GMT
CMD []
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53648c9db1a4f4013c5d44e9fd4577e839980908f0dca7a76d3c8efad06d048`  
		Last Modified: Thu, 21 Apr 2022 20:47:24 GMT  
		Size: 49.1 MB (49113769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0a30b3f6f66f585ac84b9bf017f0e7975a34fd479b9701a245f950742ad5b`  
		Last Modified: Thu, 21 Apr 2022 20:47:17 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:de6628a1837145901ad6a52437bd103285f7830c8aa27203eea30f716f01dbe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59292895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09ff39c7c861e7ca0f001f5e542ba94c66a520216bf35e15659ec0c23ba09b8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:42:43 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:42:44 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:42:45 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:42:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:42:47 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:42:48 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:42:08 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:42:09 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:42:10 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:42:11 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:43:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:43:30 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:43:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:43:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:43:33 GMT
USER varnish
# Thu, 21 Apr 2022 20:43:34 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:43:35 GMT
CMD []
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34115bd677f7c2afb67705f651ff60b689e7a3a69b0cd15a60e3d836a0162e18`  
		Last Modified: Thu, 21 Apr 2022 20:45:21 GMT  
		Size: 56.5 MB (56473443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35e121fe38cf19136053915fbb7f2d88e8c3702004736c435aa530245164896`  
		Last Modified: Thu, 21 Apr 2022 20:45:07 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:cf82764a27a365286573acdc67c5995b11030a4fc3184f8124b1645f761b3b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48896574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f3ce1cef6fa74ddc30bc42b6967d168c0174d0c06953c3955dbf10e6da9e8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:48:31 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 10:48:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 10:48:35 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 10:48:37 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 10:48:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 10:48:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 22 Apr 2022 07:13:28 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 22 Apr 2022 07:13:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 22 Apr 2022 07:13:32 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 22 Apr 2022 07:13:35 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 22 Apr 2022 07:13:38 GMT
ENV VARNISH_SIZE=100M
# Fri, 22 Apr 2022 07:15:35 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 22 Apr 2022 07:15:41 GMT
WORKDIR /etc/varnish
# Fri, 22 Apr 2022 07:15:45 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 22 Apr 2022 07:15:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 22 Apr 2022 07:15:53 GMT
USER varnish
# Fri, 22 Apr 2022 07:15:55 GMT
EXPOSE 80 8443
# Fri, 22 Apr 2022 07:15:58 GMT
CMD []
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e87322051143de85e675a2374befd084c589471c31ae811a63f81690eb82180`  
		Last Modified: Fri, 22 Apr 2022 07:17:52 GMT  
		Size: 46.1 MB (46084905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79c270534ccc583852361368fa7e4845ad3b6b16be4280d08c8edb428e390cf`  
		Last Modified: Fri, 22 Apr 2022 07:17:44 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:10414a54f8108d64836a2c9c6c865e5f9ebe6123647c3ee57867ced916313f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47350962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac56919f84b42f704fd7cfaaffe0a712aff857fbe24d7a894d9d4156d8c8b6a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:10:53 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 05 Apr 2022 06:10:53 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 21 Apr 2022 20:44:53 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 21 Apr 2022 20:44:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 21 Apr 2022 20:44:54 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 21 Apr 2022 20:44:54 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Apr 2022 20:46:21 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Apr 2022 20:46:22 GMT
WORKDIR /etc/varnish
# Thu, 21 Apr 2022 20:46:23 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 21 Apr 2022 20:46:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Apr 2022 20:46:23 GMT
USER varnish
# Thu, 21 Apr 2022 20:46:23 GMT
EXPOSE 80 8443
# Thu, 21 Apr 2022 20:46:23 GMT
CMD []
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8a48f1c01887a27a97e883fdd3fad9fb57c191e26cc389b076ad6ce3abe007`  
		Last Modified: Thu, 21 Apr 2022 20:48:28 GMT  
		Size: 44.8 MB (44750107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c99d1795f78de1f9b33331b3ee9178f8fa9622b60f90d85b5292655323e272`  
		Last Modified: Thu, 21 Apr 2022 20:48:23 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:0dac8cd2294800958f85dfa015b61c12a032fb936c8e3fb92c3ad84c524fa262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:dd353c4858b5d068b7999fece56dbdf99fb99a85121250ede66c38167cdefb20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105351648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5268f906b30a2228c6a6388bd4e44f63850541c06257235a9fced4f0e063ec1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:01:15 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 15:01:15 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 15:01:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 15:01:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 15:01:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:04:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 15:04:16 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:04:17 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:04:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:04:17 GMT
USER varnish
# Tue, 12 Jul 2022 15:04:17 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:04:17 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b961c99130da012333143f927891961c27ef1116f0090d8bf533fd840c0b9c74`  
		Last Modified: Tue, 12 Jul 2022 15:09:42 GMT  
		Size: 74.0 MB (73984565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658b13cb4c26815a73af08a7ddc35a353fa0f5cb726ac8793d92d2e1d268e853`  
		Last Modified: Tue, 12 Jul 2022 15:09:31 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:13ee5653f822aed1718ef1cf487e4e25f0e2e399e08c021c59a04020bc559a68
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81967205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c62f1c8d52f6a1feed9a6c2cfd4638a0b148af3dedf3477d5b9db1cf1bd6040c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:41:54 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 13:41:55 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 13:41:55 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 13:41:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 13:41:57 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 13:41:58 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 13:41:58 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 13:41:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 13:49:02 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 13:49:03 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 13:49:03 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 13:49:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 13:49:04 GMT
USER varnish
# Fri, 24 Jun 2022 13:49:05 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 13:49:05 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dafa03e57ec05360bf1ec882cbcd696b29942c47bbc4075891dbda3a6055ae9`  
		Last Modified: Fri, 24 Jun 2022 14:03:23 GMT  
		Size: 55.4 MB (55390624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dba669521b3b8d73bdf6969d2650d63159714b743cca40914d359d29a4e6dd2`  
		Last Modified: Fri, 24 Jun 2022 14:02:53 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:18a0523836e220ffb590bc76e8425a0e990ab942917bbd414c699e6fc897d447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99457561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9748f8eed1f5fe15de9eb3eab3e839ec48174edc8e318492b65e73acc05c008`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:15:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 14:15:28 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 14:15:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 14:15:30 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 14:15:31 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 14:15:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 14:15:33 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 14:15:34 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 14:15:35 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 14:15:36 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 14:15:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:18:30 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 14:18:30 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:18:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:18:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:18:33 GMT
USER varnish
# Tue, 12 Jul 2022 14:18:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:18:35 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1772ed21321e42f4a7653248dbcb45757b708f882b1f730d1d1edf80c69cb304`  
		Last Modified: Tue, 12 Jul 2022 14:24:41 GMT  
		Size: 69.4 MB (69402860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713cb83db0566be9810b152d08899074408929cc378d72ab71e6e940f95d14e6`  
		Last Modified: Tue, 12 Jul 2022 14:24:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:789b73487c4c3c2758a95df1769312f0c0161c6f29267b05268dd74d75483786
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106710623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76032fc1a132fb41031505a50c33160c7b2f45994572b72ace759fb897fbe7e1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:12:40 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 10:12:41 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 10:12:42 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 10:12:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 10:12:44 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 10:12:45 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 10:12:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 10:12:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 10:12:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 10:12:49 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 10:12:50 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 10:15:37 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 10:15:37 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 10:15:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:15:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 10:15:40 GMT
USER varnish
# Tue, 12 Jul 2022 10:15:41 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 10:15:42 GMT
CMD []
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18191750ecd3a1593c9604678a9dec2a16833252b74152865ff36a28a27a6222`  
		Last Modified: Tue, 12 Jul 2022 10:19:52 GMT  
		Size: 74.3 MB (74336200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3225164b08fe2beb56664a2953cb5691cacf11ff9f2cf81e2b85b1e4e0e5ca1`  
		Last Modified: Tue, 12 Jul 2022 10:19:41 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:173b2c7cb38627e42689f13efdf92ca1bc1d020321376c4af6ba13d485aa62bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104551258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d16850a5f77422730f61d747d46e86efa0eb6caea92c0a9764de9640adccd1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 03:24:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Fri, 24 Jun 2022 03:24:06 GMT
ARG VARNISH_VERSION=7.1.0
# Fri, 24 Jun 2022 03:24:09 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Fri, 24 Jun 2022 03:24:12 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Fri, 24 Jun 2022 03:24:14 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Fri, 24 Jun 2022 03:24:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 24 Jun 2022 03:24:26 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Fri, 24 Jun 2022 03:24:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Fri, 24 Jun 2022 03:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 24 Jun 2022 03:24:47 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 24 Jun 2022 03:24:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 03:56:06 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 24 Jun 2022 03:56:13 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 03:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 03:56:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 03:56:21 GMT
USER varnish
# Fri, 24 Jun 2022 03:56:23 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 03:56:26 GMT
CMD []
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71fdb1ad92808fd81a71e3af63882ad100769b32bcc0716f66d9bf9e0151440`  
		Last Modified: Fri, 24 Jun 2022 03:59:34 GMT  
		Size: 69.3 MB (69263959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c0bb90a9b290228ab1938c4e50eec94c34c8f55cc20c2a5e7a597813f28a13`  
		Last Modified: Fri, 24 Jun 2022 03:59:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:30d950ea8c839993bdbb480d94dc13dcfe0c373b11311b4c52e0f72d71c2ec95
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85780988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd57ebebc1fdf2b03941e22a350ef6f1df7d70e137d94738955242147ff25d15`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:06:21 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 12 Jul 2022 19:06:22 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 12 Jul 2022 19:06:23 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 12 Jul 2022 19:06:23 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 12 Jul 2022 19:06:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 12 Jul 2022 19:06:25 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 12 Jul 2022 19:06:26 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 12 Jul 2022 19:06:27 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 12 Jul 2022 19:06:27 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 12 Jul 2022 19:06:28 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:13:24 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 12 Jul 2022 19:13:32 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:13:32 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:13:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:13:34 GMT
USER varnish
# Tue, 12 Jul 2022 19:13:34 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:13:35 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06561947f6199b7f782a535d09351d41e6435f8bb103b2eab4390f031f333343`  
		Last Modified: Tue, 12 Jul 2022 19:28:04 GMT  
		Size: 56.1 MB (56140308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62677499f8b6b5b494ce7853458111556bc115a949c95098401362f8ef4a7255`  
		Last Modified: Tue, 12 Jul 2022 19:27:56 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:31f5e697661e5c97a7867e92755cefb5067f5177958c35fe38ca0e4be8fd3dec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:old` - linux; amd64

```console
$ docker pull varnish@sha256:80ca9c3ffd61c95e2e3bd468c5906e862e51052636ad1105793018e8d74e9e69
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101190038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a1d0d3f5afe71b234b6dce0b66cfade308ae48e137821cf3cdcdba874199813`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:06:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 15:06:39 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:06:39 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:06:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:06:40 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:06:40 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02de66ed810206b73e0c9dab04edcb5ee5e063727b6d2d4288dcacf0b689f442`  
		Last Modified: Tue, 12 Jul 2022 15:10:08 GMT  
		Size: 69.8 MB (69822955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e847f66816c3e7530bb53d396f9f98bfe1dcb263d37ca0a260ceebccaa19563d`  
		Last Modified: Tue, 12 Jul 2022 15:09:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ef8ee948db46e978034b3e527028c92fb71d2ada0c428b60fd0dd6b5607220c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77822750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2c92def99b9454e428b38b30569a93a8227b85b3f9b4728202cf1dcd9fe007`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:49:30 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 13:55:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 24 Jun 2022 13:55:16 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 13:55:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 24 Jun 2022 13:55:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 13:55:17 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 13:55:17 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87d17e6a126e6e5cda5556cd2a907d0ea8de0abc5a0db774bd93da779ed14e5`  
		Last Modified: Fri, 24 Jun 2022 14:04:17 GMT  
		Size: 51.2 MB (51246170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1253653c109b75569f3681144b8051d73b43acba27dbfc05aa2efb3cb6d0c6`  
		Last Modified: Fri, 24 Jun 2022 14:03:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:6498c5ad6d682b0076a0cbec21fef553b379504c201a87f0f7b5f14f80e9c60c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95301932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e738a742894266ad16f79ecd4b9a3474041d4f12dbfb804dff57c7a5d2db21`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:18:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:21:07 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 14:21:07 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:21:09 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:21:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:21:10 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:21:11 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e13c66f23d97c682dfc6fca33c4ba85b04f2b9b22f0a9d4a32679def5baa25b`  
		Last Modified: Tue, 12 Jul 2022 14:25:10 GMT  
		Size: 65.2 MB (65247234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e12339074edaf212e4dc9334de848255f4ef5e943ff9e7833cc7e9b636d52b4`  
		Last Modified: Tue, 12 Jul 2022 14:25:01 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:ec9290335f55e308e7023f5d8f4972eebc2b1ee671069d8820851417cc0f17df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102585121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b122adf5e34794ee172b03b3fab482bc31219a96195e1e8c300c8ae4cb9d064c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:15:19 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 00:17:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 00:17:34 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 00:17:36 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 07 Jun 2022 00:17:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 00:17:37 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 00:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf3f822dbf481370990594e81803141573a456e04899ad82fe6c4022627ebb`  
		Last Modified: Tue, 07 Jun 2022 00:21:08 GMT  
		Size: 70.2 MB (70194327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7dae54c84b4938c9aaa05092d4faf306897f47702a337f22ca87439181cc5`  
		Last Modified: Tue, 07 Jun 2022 00:20:57 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:2e3c1ac9eacb11fab6237bcd3eff4d406e0b300e5c3144e3934ddf939b4e277c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100378186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b130ac9ed26512fd8cddaf8489ddf70922771377f7b1d009ba5e2de0dd5d960`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:38:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 06:55:41 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 06:55:47 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 06:55:48 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 07 Jun 2022 06:55:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 06:55:55 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 06:56:00 GMT
CMD []
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c63706549952669ea4fc52e3a012cb12b690358fdde6057b825e1f21313259d`  
		Last Modified: Tue, 07 Jun 2022 07:15:28 GMT  
		Size: 65.1 MB (65091015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe199e856d7bedadb8a4da892a5d774b9146e8358d8909a62fadd06dbce3022b`  
		Last Modified: Tue, 07 Jun 2022 07:15:16 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:4b16cb3b466bbe809c4833e2631cd4a9ddf572227e11c2fb3ce158a52465a752
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81623472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:426be98166563a81501f737bf7edd9103507a566117a5395e75a6d54d80ada03`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:13:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:19:47 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 19:19:57 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:19:57 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:19:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:19:59 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:20:00 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f44713e40e8cd034f4c8f4dd815e5302835db628ffb0d6f606de6a30b3e909c`  
		Last Modified: Tue, 12 Jul 2022 19:28:33 GMT  
		Size: 52.0 MB (51982789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a43b712b028475ec29bca3a805cc61d86ec779b321fcd68dcdf093c4f9cfc1e`  
		Last Modified: Tue, 12 Jul 2022 19:28:25 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:a96966b666c3eb795b5a5ffe4b7f1911e009156774d5551a355de6ba17dd6ca5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:old-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:1f798a786c909e75214591ae7bb11711b606d19904771e17cac071e3fc945f23
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58347562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40f303a05efad59d4625679d65998e25ac6af2a5a1e8e761d6165038faf0af7a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:46:19 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 09:47:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 09:47:16 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 09:47:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:47:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 09:47:16 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 09:47:16 GMT
CMD []
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd49c5f702ffa093526e350e19af19adacee36ebd21a4d2b8215729aebd24701`  
		Last Modified: Tue, 05 Apr 2022 09:48:23 GMT  
		Size: 55.5 MB (55528711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b11f3cacc52df447f6e49ab5dcad0b25a3e95d3aa5ca786c8a00b94bcea4d97`  
		Last Modified: Tue, 05 Apr 2022 09:48:15 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:d0ef8137631136de68aa9ca8b5a1c202753588e4823091fc74c7381800475e92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44158672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b498faee8096b05f4ad1e1a034d79076f1405006bbb01cdc1b62443d19faf0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:12:30 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 19:13:58 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 19:13:59 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 19:13:59 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 19:14:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 19:14:00 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 19:14:00 GMT
CMD []
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a122a3f3e3f4f262ecd7c937fb5b761d7c7025f6b85195b6f6e59efccc3e22`  
		Last Modified: Tue, 05 Apr 2022 19:17:11 GMT  
		Size: 41.7 MB (41730222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e23c5ffb616fb8979712f573ce76a21ff2948ffe3c222f25abeda1b044fb82`  
		Last Modified: Tue, 05 Apr 2022 19:16:49 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:287bbe458761ddf7b90152156bcfcf1680e8229b94e87c6be21fcdcff4105325
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51100328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb806b4ff6eae8a70eec669d64a63205e9fa899f74021c50544a8a3fe8492216`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:24:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 07:25:05 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 07:25:05 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 07:25:07 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 07:25:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 07:25:08 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 07:25:09 GMT
CMD []
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c097d0722cedf772b294574bd3df3ea7bc3fd2a7f0d584bdda75906ab4a4f76`  
		Last Modified: Tue, 05 Apr 2022 07:26:39 GMT  
		Size: 48.4 MB (48382460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda2d05467662609f11c35127449028bdba318e2920842c0c49a157d72fd14d4`  
		Last Modified: Tue, 05 Apr 2022 07:26:32 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:8d9a98e8ebe8c794faad1ca62b64b1d0f5d50b4bdc61593272165af938c90e58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58550969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8b86a5912210274cdd2be334341ab5c8a5cc8b98b8cacbf00d0bc3b61391b34`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:44:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 06:45:29 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 06:45:29 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 06:45:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:45:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 06:45:32 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 06:45:33 GMT
CMD []
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781285b91779b0524f4a4b362a85bf7ad3c11049ec60271bc351d3ea22722f55`  
		Last Modified: Tue, 05 Apr 2022 06:47:18 GMT  
		Size: 55.7 MB (55729277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ede4c98a857e7e2e4374c87b05da88e9cfa36a1b9d2261f338a8e4cc091689`  
		Last Modified: Tue, 05 Apr 2022 06:47:09 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:99fc715aa51f45f415d42e16933cfd6640741633a9df875d1be9c41bb5eea1e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48200204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afb3e6b26fed2aaed2bdf33c3edb6718410d71cdda8521c1e6a42a745e020d3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:52:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 10:53:50 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 10:53:55 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 10:53:56 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:53:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 10:54:00 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 10:54:02 GMT
CMD []
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7876f582583c6ce1dd934300234645dd5b97252662a8c87fdfbf82c860328d90`  
		Last Modified: Tue, 05 Apr 2022 10:55:44 GMT  
		Size: 45.4 MB (45385557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bba04077c5c30296939df9ed09482547b8947d5decf08a738273fa064ca121a`  
		Last Modified: Tue, 05 Apr 2022 10:55:36 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:d23bba4fca1b0dd78c6f32996dd386b94a4944ac5ea047d049913f9f2c51e200
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:113021b450dcbd4035fcfba58dd928217e0d39bff640b6d895c83e8eb2592df4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:12:32 GMT
ENV VARNISH_SIZE=100M
# Tue, 05 Apr 2022 06:13:11 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 05 Apr 2022 06:13:13 GMT
WORKDIR /etc/varnish
# Tue, 05 Apr 2022 06:13:13 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:13:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 05 Apr 2022 06:13:13 GMT
EXPOSE 80 8443
# Tue, 05 Apr 2022 06:13:13 GMT
CMD []
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df61fc68478458a071e8edf49185d9b224067a6e66831cdde802e5d2b66b097`  
		Last Modified: Tue, 05 Apr 2022 06:14:33 GMT  
		Size: 44.1 MB (44067532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829d58f668fddd7b5ed61e0d6c27f5b3abd19844eeb8ad111b395b944d064904`  
		Last Modified: Tue, 05 Apr 2022 06:14:27 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:75cde1f365c01d4f67a4acb2fc4c0f6847b81567649f30c13987f455f59b6e13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:a6aec0b505ab121e0a3a6ed41af86dbea176d84b06114a9125ebc3adf4d4fd9b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100578628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592008399710472f47e4e41199f0fa992d820b25e4714cb3dbc7e299f9d03a2c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 15:08:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 15:09:00 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 15:09:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 15:09:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 15:09:00 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 15:09:00 GMT
CMD []
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89be986846906e3bd77fcb69c2287e9b2967e13e6db6789e5baf1d506be18d0d`  
		Last Modified: Tue, 12 Jul 2022 15:10:32 GMT  
		Size: 69.2 MB (69211316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a428efaa1b7e1631a51a487cd7d5d5cc05b0e39a4ffa98c2aec733eaf642f2d`  
		Last Modified: Tue, 12 Jul 2022 15:10:22 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:2c4b41efa4196611ae6cb4b6eddcf84bdc0e1a43a03b4c76aac3eedca9b087fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77226111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d94aa4723ac8b23869f306e96838344ed1f5a2cd74755ebfeda8cb2b50e4e28b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 13:49:30 GMT
ENV VARNISH_SIZE=100M
# Fri, 24 Jun 2022 14:01:27 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 24 Jun 2022 14:01:28 GMT
WORKDIR /etc/varnish
# Fri, 24 Jun 2022 14:01:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 24 Jun 2022 14:01:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 24 Jun 2022 14:01:29 GMT
EXPOSE 80 8443
# Fri, 24 Jun 2022 14:01:30 GMT
CMD []
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a9c851df1c2951d6a3d73f1c5810a184f118b264badec4600fcf771ce8931f`  
		Last Modified: Fri, 24 Jun 2022 14:05:06 GMT  
		Size: 50.6 MB (50649305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e281c64d9d1456fd161381c1684f89e9b344f5d89c5828842b284f7d6a7424`  
		Last Modified: Fri, 24 Jun 2022 14:04:37 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:3344e5dbea7c39c0e78316c060bc7cdaf6914c5c484446a18801ad7ea97245e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94702840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664add611afb8aa9218e165904e2c908a1e45e7884530a8f0e3dca4579266009`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:18:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 14:23:35 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 14:23:36 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 14:23:38 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:23:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 14:23:39 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 14:23:40 GMT
CMD []
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d8825494e5a3d0e5dc7419b15ef72845e7cd473e057dab29425c350e56f8b6`  
		Last Modified: Tue, 12 Jul 2022 14:25:36 GMT  
		Size: 64.6 MB (64647915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71275849326318c97b15f88b97e005a2f8436f713efc326d5ee465ce462a0bfc`  
		Last Modified: Tue, 12 Jul 2022 14:25:27 GMT  
		Size: 699.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:854e3a098f80fdeba4d4cc76090415b08fe9784ac0c51df85bf79af763af0300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102058379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b66188412d2b0af5c64a7ff374272c2c50a99d47354c94fab8596c55197ab2a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:15:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 10:18:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 10:18:48 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 10:18:50 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:18:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 10:18:51 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 10:18:52 GMT
CMD []
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275617bc24aba724d9e033099ad564c3d9848c6b195104cd4d16bd7373466bd1`  
		Last Modified: Tue, 12 Jul 2022 10:20:26 GMT  
		Size: 69.7 MB (69683727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7943edd0a7e181bd2b8627956de13a2ad69628c8b0c11640a5dfb9c260a9bd1`  
		Last Modified: Tue, 12 Jul 2022 10:20:14 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:6b84cbc1a9c28cf8991d7ec366d46fdbd99b146e3425936b6c4c79385742ff0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99796088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52f7bf64fe65b1bab46892519f2b7f0c892d3ec6613dd2de3f41884d756d9ef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:38:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 07:14:13 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 07:14:18 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 07:14:20 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 07 Jun 2022 07:14:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 07:14:24 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 07:14:26 GMT
CMD []
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fbfae2215345643446eec0955f5aa2abf2566a51f5bab1280983b19f267d73`  
		Last Modified: Tue, 07 Jun 2022 07:15:58 GMT  
		Size: 64.5 MB (64508688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d019e20eb144f16f23de1ecf38bc429a7f5e2081e77131ebd79e4ef88fdd1f94`  
		Last Modified: Tue, 07 Jun 2022 07:15:46 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:d143ac4588cc1f8f8facfce939eb38ad073081e6f10b158d965369d48ac45cce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80994227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76348292b58d165facf504362ea67a0bdfce1dbfdc009bd51c195e4eff713ae`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 19:13:57 GMT
ENV VARNISH_SIZE=100M
# Tue, 12 Jul 2022 19:26:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 12 Jul 2022 19:26:45 GMT
WORKDIR /etc/varnish
# Tue, 12 Jul 2022 19:26:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:26:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 12 Jul 2022 19:26:46 GMT
EXPOSE 80 8443
# Tue, 12 Jul 2022 19:26:47 GMT
CMD []
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5713f0c860e92ea10da6e18fa83f8aad21a2056b3d968ad5b0f975587d0c3614`  
		Last Modified: Tue, 12 Jul 2022 19:28:56 GMT  
		Size: 51.4 MB (51353315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8723d90b7e824ceee06e46c8072d1585b761be55f9a8a12393845318b9e5fc57`  
		Last Modified: Tue, 12 Jul 2022 19:28:49 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
