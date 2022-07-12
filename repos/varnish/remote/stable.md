## `varnish:stable`

```console
$ docker pull varnish@sha256:8b7b459535e7e48b163b0e7d894851aa0d83d49575c22dbc760a5fc738fce7ba
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
$ docker pull varnish@sha256:24b9f4596c2078cd946361b949547a3b1194fe63c0403dd926a8550f8d7a8a05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100591128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10fd84989ad5a039ad95ecea3693a06e6d728f53203de94337d9219d4019c69d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:33:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 07 Jun 2022 18:16:00 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 07 Jun 2022 18:16:00 GMT
WORKDIR /etc/varnish
# Tue, 07 Jun 2022 18:16:01 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:16:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 07 Jun 2022 18:16:01 GMT
EXPOSE 80 8443
# Tue, 07 Jun 2022 18:16:01 GMT
CMD []
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e137a86f459dd0da9bc05dac6ea4cde4f11d381066ae6f46ab9c5fa1bb9326`  
		Last Modified: Tue, 07 Jun 2022 18:16:39 GMT  
		Size: 69.2 MB (69211151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f66b13b24616b785528160791fa39a340094baf1334aa52f6599b13da75b037`  
		Last Modified: Tue, 07 Jun 2022 18:16:29 GMT  
		Size: 701.0 B  
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
$ docker pull varnish@sha256:367d9ae81cbbd4268a768824631a734778f6f6e549ecad76b943ce219075459e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81009219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604a7fd6b29893e306f96d0837e985ad149c2d505144b14150de780f40381f8c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:95dc6dcd4ebd15b42beaf935d91adafb0ea44a443bb44597bc1ff236e831ce18 in / 
# Sat, 28 May 2022 00:43:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:51:45 GMT
ENV VARNISH_SIZE=100M
# Sat, 28 May 2022 16:02:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 28 May 2022 16:03:06 GMT
WORKDIR /etc/varnish
# Sat, 28 May 2022 16:03:06 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 28 May 2022 16:03:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 28 May 2022 16:03:07 GMT
EXPOSE 80 8443
# Sat, 28 May 2022 16:03:08 GMT
CMD []
```

-	Layers:
	-	`sha256:f7bb6d2d11c3060ba2e66ba762e2aa10a0d1d361cfa6a806bcf26a64cc3a79aa`  
		Last Modified: Sat, 28 May 2022 00:49:46 GMT  
		Size: 29.7 MB (29655258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d783ad59af179204e319770b35e27415aa700a28a3307a418b4e168bf97c40`  
		Last Modified: Sat, 28 May 2022 16:04:50 GMT  
		Size: 51.4 MB (51353261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14035e5c15b3f586e231b74547fc1b82b0895f559884d9b1157d488881ca762`  
		Last Modified: Sat, 28 May 2022 16:04:43 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
