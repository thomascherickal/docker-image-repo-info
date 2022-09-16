<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.10`](#varnish6010)
-	[`varnish:7.1`](#varnish71)
-	[`varnish:7.1-alpine`](#varnish71-alpine)
-	[`varnish:7.1.1`](#varnish711)
-	[`varnish:7.1.1-alpine`](#varnish711-alpine)
-	[`varnish:7.2`](#varnish72)
-	[`varnish:7.2-alpine`](#varnish72-alpine)
-	[`varnish:7.2.0`](#varnish720)
-	[`varnish:7.2.0-alpine`](#varnish720-alpine)
-	[`varnish:alpine`](#varnishalpine)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:fresh-alpine`](#varnishfresh-alpine)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:old`](#varnishold)
-	[`varnish:old-alpine`](#varnishold-alpine)
-	[`varnish:stable`](#varnishstable)

## `varnish:6.0`

```console
$ docker pull varnish@sha256:f3e5ecdf63e9b1aac54ba5c9a17d378b7f0879a81168510c3075913fe0c0ac6b
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
$ docker pull varnish@sha256:7376c7bd35daf6fefbb13be6b0d09053c9179134e3d67eebb288c7470c9bde63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100644811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bd8d717b7c4c5985bb57a51e08edc1983492be02706815bae6715fe5305389`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:35:23 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:39:53 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 13:39:53 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:39:53 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:39:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:39:54 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:39:54 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e60ef9ff523c960036ce4579422db4cb54a38db820f736cdfaf8197fa8dc97`  
		Last Modified: Tue, 13 Sep 2022 13:41:24 GMT  
		Size: 69.2 MB (69239988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5cccebb4545f0fb8c8850fb2fd4c089330f5e5ceb54fbad8167522f9a50c75`  
		Last Modified: Tue, 13 Sep 2022 13:41:15 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:8456945bbf5035d0da5e568b83f6901b311e6ce4737d2b7525ef2e81b1ee46f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77214448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23e0e371fff20134e85dd69951d6d8fc47e117a6608975b5a3683c84c99f8206`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 09:17:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 14 Sep 2022 09:21:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 14 Sep 2022 09:21:59 GMT
WORKDIR /etc/varnish
# Wed, 14 Sep 2022 09:21:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 14 Sep 2022 09:21:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 14 Sep 2022 09:21:59 GMT
EXPOSE 80 8443
# Wed, 14 Sep 2022 09:21:59 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a97f0435f33c0b679f380d2e64c74751ca813df0058528016a5a6d6829a86f`  
		Last Modified: Wed, 14 Sep 2022 09:23:49 GMT  
		Size: 50.6 MB (50646687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fb9a273b672257943130cedb60e07d2394eae521ce1f123fffe6ab808ab8ef`  
		Last Modified: Wed, 14 Sep 2022 09:23:42 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e60be39c540957ef5d022a0b8e226a03a1dfce649c589f0139d9566276760c0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94700859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050c6d2c69dae42ac73a197ecd1e63e4c8d87d2b483ca08568d3bf85c4098671`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:51:08 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:55:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 13:55:45 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:55:47 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:55:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:55:48 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:55:49 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c06c206db57123dd985a252975427fb03e52722219cdba578d4350af7f9542`  
		Last Modified: Tue, 13 Sep 2022 13:57:44 GMT  
		Size: 64.6 MB (64645917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64363984b04e8cb866ab0fd7879b69b5f6704aef21c195ebe081d9b88a4a630d`  
		Last Modified: Tue, 13 Sep 2022 13:57:35 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:ee7530f27c0331063c0d85a1c4b569f2188ef865be698f40b7a4d1d4fddb604e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102162087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849660f699b843c7cb096d3e5a0fa4167ca5dd73465d32041c23342096082294`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:50:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 10 Aug 2022 00:10:58 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 10 Aug 2022 00:10:58 GMT
WORKDIR /etc/varnish
# Wed, 10 Aug 2022 00:11:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:11:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 10 Aug 2022 00:11:01 GMT
EXPOSE 80 8443
# Wed, 10 Aug 2022 00:11:02 GMT
CMD []
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551416d7a3fd6bd33021d63c1f1ed875e5c6bf8ac312001f2020f3c684b2d265`  
		Last Modified: Wed, 10 Aug 2022 00:13:19 GMT  
		Size: 69.8 MB (69787331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d53139023415366a342b716b2904d2191cf1e010e870137a180112974b28bf`  
		Last Modified: Wed, 10 Aug 2022 00:13:06 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:f4ef9cecfa3f21f34166c4313bd546c57254308e823f672003c02712391a40a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99780540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d95da7841ca570b682453a77e8c115254de7502ba0842fd135c0b1b5064abfa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:55:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 11:04:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 11:04:55 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 11:04:56 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:04:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 11:04:56 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 11:04:57 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b395186dad8fe056941c287ed6f5a2274254764f1c640e616faa8b81ded16`  
		Last Modified: Tue, 13 Sep 2022 11:07:23 GMT  
		Size: 64.5 MB (64502448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e80220ec6b0a4060a85ce7f7a790fe52300bc047d962ecfc2c8a2fd57c7b4ec`  
		Last Modified: Tue, 13 Sep 2022 11:07:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:98885dfc5266cea2aaf3f0345de157182204e4489499c4202c63ee559f9b057a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80987355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:091248160e935dbb7c24d2a163688640176e0890c25589e93f886b7c4332473c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:56:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 06:59:25 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 06:59:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 06:59:27 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:59:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 06:59:27 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 06:59:28 GMT
CMD []
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf394baf5aa4f42027ab215a1b68569c9e328288832fdda5565d5229ab4495a4`  
		Last Modified: Tue, 13 Sep 2022 07:00:44 GMT  
		Size: 51.4 MB (51351573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633eb3e1a06ce29f4a4ba0ff4c8c423280d1250331682f18d851d981246d166`  
		Last Modified: Tue, 13 Sep 2022 07:00:37 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.10`

```console
$ docker pull varnish@sha256:f3e5ecdf63e9b1aac54ba5c9a17d378b7f0879a81168510c3075913fe0c0ac6b
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
$ docker pull varnish@sha256:7376c7bd35daf6fefbb13be6b0d09053c9179134e3d67eebb288c7470c9bde63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100644811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bd8d717b7c4c5985bb57a51e08edc1983492be02706815bae6715fe5305389`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:35:23 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:39:53 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 13:39:53 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:39:53 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:39:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:39:54 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:39:54 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e60ef9ff523c960036ce4579422db4cb54a38db820f736cdfaf8197fa8dc97`  
		Last Modified: Tue, 13 Sep 2022 13:41:24 GMT  
		Size: 69.2 MB (69239988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5cccebb4545f0fb8c8850fb2fd4c089330f5e5ceb54fbad8167522f9a50c75`  
		Last Modified: Tue, 13 Sep 2022 13:41:15 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; arm variant v7

```console
$ docker pull varnish@sha256:8456945bbf5035d0da5e568b83f6901b311e6ce4737d2b7525ef2e81b1ee46f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77214448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23e0e371fff20134e85dd69951d6d8fc47e117a6608975b5a3683c84c99f8206`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 09:17:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 14 Sep 2022 09:21:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 14 Sep 2022 09:21:59 GMT
WORKDIR /etc/varnish
# Wed, 14 Sep 2022 09:21:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 14 Sep 2022 09:21:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 14 Sep 2022 09:21:59 GMT
EXPOSE 80 8443
# Wed, 14 Sep 2022 09:21:59 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a97f0435f33c0b679f380d2e64c74751ca813df0058528016a5a6d6829a86f`  
		Last Modified: Wed, 14 Sep 2022 09:23:49 GMT  
		Size: 50.6 MB (50646687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fb9a273b672257943130cedb60e07d2394eae521ce1f123fffe6ab808ab8ef`  
		Last Modified: Wed, 14 Sep 2022 09:23:42 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e60be39c540957ef5d022a0b8e226a03a1dfce649c589f0139d9566276760c0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94700859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050c6d2c69dae42ac73a197ecd1e63e4c8d87d2b483ca08568d3bf85c4098671`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:51:08 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:55:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 13:55:45 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:55:47 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:55:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:55:48 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:55:49 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c06c206db57123dd985a252975427fb03e52722219cdba578d4350af7f9542`  
		Last Modified: Tue, 13 Sep 2022 13:57:44 GMT  
		Size: 64.6 MB (64645917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64363984b04e8cb866ab0fd7879b69b5f6704aef21c195ebe081d9b88a4a630d`  
		Last Modified: Tue, 13 Sep 2022 13:57:35 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; 386

```console
$ docker pull varnish@sha256:ee7530f27c0331063c0d85a1c4b569f2188ef865be698f40b7a4d1d4fddb604e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102162087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849660f699b843c7cb096d3e5a0fa4167ca5dd73465d32041c23342096082294`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:50:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 10 Aug 2022 00:10:58 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 10 Aug 2022 00:10:58 GMT
WORKDIR /etc/varnish
# Wed, 10 Aug 2022 00:11:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:11:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 10 Aug 2022 00:11:01 GMT
EXPOSE 80 8443
# Wed, 10 Aug 2022 00:11:02 GMT
CMD []
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551416d7a3fd6bd33021d63c1f1ed875e5c6bf8ac312001f2020f3c684b2d265`  
		Last Modified: Wed, 10 Aug 2022 00:13:19 GMT  
		Size: 69.8 MB (69787331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d53139023415366a342b716b2904d2191cf1e010e870137a180112974b28bf`  
		Last Modified: Wed, 10 Aug 2022 00:13:06 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; ppc64le

```console
$ docker pull varnish@sha256:f4ef9cecfa3f21f34166c4313bd546c57254308e823f672003c02712391a40a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99780540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d95da7841ca570b682453a77e8c115254de7502ba0842fd135c0b1b5064abfa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:55:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 11:04:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 11:04:55 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 11:04:56 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:04:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 11:04:56 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 11:04:57 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b395186dad8fe056941c287ed6f5a2274254764f1c640e616faa8b81ded16`  
		Last Modified: Tue, 13 Sep 2022 11:07:23 GMT  
		Size: 64.5 MB (64502448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e80220ec6b0a4060a85ce7f7a790fe52300bc047d962ecfc2c8a2fd57c7b4ec`  
		Last Modified: Tue, 13 Sep 2022 11:07:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; s390x

```console
$ docker pull varnish@sha256:98885dfc5266cea2aaf3f0345de157182204e4489499c4202c63ee559f9b057a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80987355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:091248160e935dbb7c24d2a163688640176e0890c25589e93f886b7c4332473c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:56:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 06:59:25 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 06:59:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 06:59:27 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:59:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 06:59:27 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 06:59:28 GMT
CMD []
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf394baf5aa4f42027ab215a1b68569c9e328288832fdda5565d5229ab4495a4`  
		Last Modified: Tue, 13 Sep 2022 07:00:44 GMT  
		Size: 51.4 MB (51351573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633eb3e1a06ce29f4a4ba0ff4c8c423280d1250331682f18d851d981246d166`  
		Last Modified: Tue, 13 Sep 2022 07:00:37 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1`

```console
$ docker pull varnish@sha256:93a531ff670336cdf3f59576e2a78ea6047c6bb64d64d69770733d7d718a637b
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
$ docker pull varnish@sha256:0e8f27d3cfb5a2d68e04074e15d1e8bc7ac9dab331055219cd6cd732cbddd021
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106514619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324a8892e787c7c40773fdcaff3a2ae5fd21e9f0bb1c445b1be3e3b7792ab148`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:31:58 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:31:58 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:31:59 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:31:59 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:31:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:31:59 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:31:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:27:28 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:27:28 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:27:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:27:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:27:29 GMT
USER varnish
# Fri, 16 Sep 2022 00:27:29 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:27:29 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bc5fa37c18f8ef5e3cfacc07d2984665abb9543381738b2c53cb9322d40ce1`  
		Last Modified: Fri, 16 Sep 2022 00:28:54 GMT  
		Size: 75.1 MB (75110005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6325df2deb75046ab9f2ed04575d407626eab372b24c26f424907b04995e33e5`  
		Last Modified: Fri, 16 Sep 2022 00:28:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:392642824dbf95562e4be5f32ad959eae47c71195cc4a4f592549b86dfd9ce8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82882221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3df25f03198101a3267cba96f0a1b62785bbed5be1fb8e74c4971b66b1dd85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 09:12:45 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_VERSION=7.1.1
# Wed, 14 Sep 2022 09:12:45 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 14 Sep 2022 09:12:46 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 14 Sep 2022 09:12:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 14 Sep 2022 09:12:46 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Wed, 14 Sep 2022 09:12:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:07:33 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:07:34 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:07:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:07:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:07:34 GMT
USER varnish
# Fri, 16 Sep 2022 01:07:34 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:07:34 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837ab6cca90169544033a72edbbc42950c0ac37d369014a8b865475c25929d7d`  
		Last Modified: Fri, 16 Sep 2022 01:09:28 GMT  
		Size: 56.3 MB (56314670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbc457d33c646badce8896611b19df90fb5cc01d79b798d6efbf1b12cfc84ea`  
		Last Modified: Fri, 16 Sep 2022 01:09:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:51ebe92fa5740ff0d791d15cd441a8b32d6eeff785f0089ac4f077921ab6217e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100529442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1558f14eaa2d5575200e445de6b40e630fabe003647d522f2c1ff6f35471da`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:47:36 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:47:37 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:47:38 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:47:39 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:47:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:47:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:47:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:47:45 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:47:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:59:13 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:59:14 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:59:15 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:59:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:59:16 GMT
USER varnish
# Fri, 16 Sep 2022 00:59:17 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:59:18 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c970cc9dde8076da5c6f21786dd260fec5eeff61c971177d7eda600f72d0bd75`  
		Last Modified: Fri, 16 Sep 2022 01:00:17 GMT  
		Size: 70.5 MB (70474710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99af8e91aa17958255f36cc3c0bb2a23122da60b990136cb11e1c7159e1dbd42`  
		Last Modified: Fri, 16 Sep 2022 01:00:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; 386

```console
$ docker pull varnish@sha256:ca00e9197a158235394e55ac80e116054690d973b61024ab5288c5f00d97f920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107894486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d157e840659f240aa4691e7f7f1fc9c43a8b7e0719341d00f6ff535342f3d100`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:39:38 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:39:39 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:39:40 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:39:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:39:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:39:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:39:44 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:39:45 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:39:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:39:47 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:39:48 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:46:33 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:46:34 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:46:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:46:36 GMT
USER varnish
# Fri, 16 Sep 2022 00:46:37 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:46:38 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf4fd1bf9eb0d00791f595ede4056ac426b9cb5e92a83b8540a7d57d51a915`  
		Last Modified: Fri, 16 Sep 2022 00:49:02 GMT  
		Size: 75.5 MB (75510208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f49a2344808e983420284ba4af102676307b3e4e57205cee8cefcd0f196b73`  
		Last Modified: Fri, 16 Sep 2022 00:48:52 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:387cd6794baf021e9362961e2384acbdb25e98fe9a1a394bb6ca859c3c0d3c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104492792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884a34f4825b0e2e99e750df9c6eb4d44c28ff0a026a3d8932d446f01665b1f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:48:48 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 10:48:48 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 10:48:48 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 10:48:50 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 10:54:43 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 10:54:46 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 10:54:46 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:54:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 10:54:47 GMT
USER varnish
# Tue, 13 Sep 2022 10:54:47 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 10:54:48 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e8423909e32907c374b40534ee89da2efcdb5bb4761bad98dbc593e3aa29e`  
		Last Modified: Tue, 13 Sep 2022 11:06:10 GMT  
		Size: 69.2 MB (69214925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeee3ea66d867696a8db281c80b7caa089b11024d1e616add57c163aebb4ad8`  
		Last Modified: Tue, 13 Sep 2022 11:05:53 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; s390x

```console
$ docker pull varnish@sha256:94533056a29ed197fe0a3b8d7e3267730a8b9550a81604729665a744362ec716
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85727466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:024c8b5a25f9e560b63b1bb14f3a0c93d14354a7ac3b3a849c93566bab34ccd3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:53:42 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 06:53:42 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 06:53:42 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 06:53:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 06:53:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 06:53:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 06:56:13 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 06:56:15 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 06:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:56:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 06:56:16 GMT
USER varnish
# Tue, 13 Sep 2022 06:56:16 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 06:56:16 GMT
CMD []
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04976f863b25f9dbf72873d6cdbccf813a5d2db0ca7818d68284fc6d588ed2ac`  
		Last Modified: Tue, 13 Sep 2022 07:00:20 GMT  
		Size: 56.1 MB (56091911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dcdef6310d5d684296de769c6877cf4dbf99739f5b1af7dfe9555972fef90a`  
		Last Modified: Tue, 13 Sep 2022 07:00:13 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1-alpine`

```console
$ docker pull varnish@sha256:81257c6d7d2a44b04b667945fdadbaf89cd18b55d0353128396a035e5a77c410
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
$ docker pull varnish@sha256:e06e93886caf501e38c01e0cf44514d3366110552961fe17a7d17ff3efff3ca8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59071089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4cdf3802e46ef3f57ec91755bcfd5bb19b6336c84e8097bcfeabb37b807dd5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:27:09 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:31 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:31 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:31 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:32 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:25:47 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:25:48 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:27:36 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:27:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:27:37 GMT
USER varnish
# Fri, 16 Sep 2022 00:27:37 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:27:37 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07f5c00a3fca42168beb309a1da4497d81192fcd78cb270293088a816212694`  
		Last Modified: Thu, 11 Aug 2022 18:29:57 GMT  
		Size: 56.2 MB (56247081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73638df192f2f0445e49db4333e9a9f39e26938968e3c796a81c87fae3df9015`  
		Last Modified: Fri, 16 Sep 2022 00:29:11 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c6b22c4963a1cec7a22ba1a943823cf54e5a5c1b2b9ac286fed3a0029174cb96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44838985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c6a6655fc442310bfb54f8b59a9ccfb5405c8a0bb74e1020d1aa128f99cb1d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 04:07:16 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:01:20 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:01:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:01:21 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:01:21 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:03:23 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:03:24 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:07:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:07:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:07:40 GMT
USER varnish
# Fri, 16 Sep 2022 01:07:40 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:07:40 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6526057e940a58d88649203706292e565d300408dfb557a419d381f3ffd9b83`  
		Last Modified: Thu, 11 Aug 2022 18:08:20 GMT  
		Size: 42.4 MB (42403394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690ee8cc9fd56bce463253ce04df4f0a2516e0d70b4a66686ccc509d6b7eeeb2`  
		Last Modified: Fri, 16 Sep 2022 01:09:43 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:b5f5c38564b8c68d2c89cb0c5cf07cf929d7c6c29623985a41e66df8fa1d7ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51804113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:318da3f2dbda7664008e779ce42a20556100d6c8e8acea62c90fac68535d7bc5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:16:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:51:52 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:51:53 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:51:54 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:51:55 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:51:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:51:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:51:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:51:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:52:00 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:52:01 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:53:20 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:53:20 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:59:30 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:59:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:59:31 GMT
USER varnish
# Fri, 16 Sep 2022 00:59:32 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:59:33 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66637d73d151e7b8d3fe367559b7457ef1203d2aebfd50c2e70fd5bf1e99c081`  
		Last Modified: Thu, 11 Aug 2022 17:58:22 GMT  
		Size: 49.1 MB (49085174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac15dc4fc673a317837b93832817c5e204d3aff8a6f781c1aeed2c550eb0203a`  
		Last Modified: Fri, 16 Sep 2022 01:00:31 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:fc0aba45a3efd75271ef52fe059638e8a931fc594087a18c4653715ea78a8dde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59260455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7289c0f508c7f43337e64f4f82329aa9deab92bfb820139adff8bf251bf79bd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:03:37 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:42:11 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:42:12 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:42:13 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:42:14 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:42:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:42:16 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:42:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:42:18 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:42:19 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:42:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:43:37 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:43:37 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:46:48 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:46:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:46:49 GMT
USER varnish
# Fri, 16 Sep 2022 00:46:50 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:46:51 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48542280e8f5e646fe63a44668949d53d57e9c3f41a0308717d0f58f2c9038e3`  
		Last Modified: Thu, 11 Aug 2022 17:48:38 GMT  
		Size: 56.4 MB (56431439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6279ed53a3e61eb8ad01dc9fa88f7e0be37a3bf70d2ddaa540a2d49788d3b0a`  
		Last Modified: Fri, 16 Sep 2022 00:49:15 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:afb06d7114e815bd133ac5b96241965064541f406cb5707f6c41157d02dbf40b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48872166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3709d135f1017d354137d2bc10fa3c292b86320cf2e4f192d99555c5ecc09fa3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:13:06 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:41 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:44 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:26:34 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:26:37 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:28:32 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:28:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:28:33 GMT
USER varnish
# Fri, 16 Sep 2022 00:28:33 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:28:33 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a15064fbadc2b9bce565fe7971fba76bf7ae75f6d59ef2522607a17e18fb60`  
		Last Modified: Thu, 11 Aug 2022 18:35:48 GMT  
		Size: 46.1 MB (46058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1af803614fcc096ee8ba2285a9d578ffed5f1eaded260624ac7a413e1e337e`  
		Last Modified: Fri, 16 Sep 2022 00:28:59 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:ecf905f62dca3c6c7db7de8bcdf43c42e4ae1c5dc635c19b818bc3ac1bbfd565
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47321925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faddc4fd662ea6dbedb36db17ab477108f0cc14c51de05c9973344b01fbe4e2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:54:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:46:35 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:46:35 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:46:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:48:19 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:48:25 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:51:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:51:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:51:06 GMT
USER varnish
# Fri, 16 Sep 2022 00:51:06 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:51:06 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694fec8cf4b1f4958bdd7c4941f751e5c9df3eb875c8003dccefe1dd9cfce4e2`  
		Last Modified: Thu, 11 Aug 2022 17:56:53 GMT  
		Size: 44.7 MB (44715342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aef5c8565b8c4c641ab0b36f868644a4a2132bc4da1ccc7f8ab18efd4f4596`  
		Last Modified: Fri, 16 Sep 2022 00:51:36 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.1`

```console
$ docker pull varnish@sha256:93a531ff670336cdf3f59576e2a78ea6047c6bb64d64d69770733d7d718a637b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1.1` - linux; amd64

```console
$ docker pull varnish@sha256:0e8f27d3cfb5a2d68e04074e15d1e8bc7ac9dab331055219cd6cd732cbddd021
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106514619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324a8892e787c7c40773fdcaff3a2ae5fd21e9f0bb1c445b1be3e3b7792ab148`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:31:58 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:31:58 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:31:59 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:31:59 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:31:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:31:59 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:31:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:27:28 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:27:28 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:27:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:27:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:27:29 GMT
USER varnish
# Fri, 16 Sep 2022 00:27:29 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:27:29 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bc5fa37c18f8ef5e3cfacc07d2984665abb9543381738b2c53cb9322d40ce1`  
		Last Modified: Fri, 16 Sep 2022 00:28:54 GMT  
		Size: 75.1 MB (75110005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6325df2deb75046ab9f2ed04575d407626eab372b24c26f424907b04995e33e5`  
		Last Modified: Fri, 16 Sep 2022 00:28:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:392642824dbf95562e4be5f32ad959eae47c71195cc4a4f592549b86dfd9ce8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82882221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3df25f03198101a3267cba96f0a1b62785bbed5be1fb8e74c4971b66b1dd85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 09:12:45 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_VERSION=7.1.1
# Wed, 14 Sep 2022 09:12:45 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 14 Sep 2022 09:12:46 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 14 Sep 2022 09:12:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 14 Sep 2022 09:12:46 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Wed, 14 Sep 2022 09:12:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:07:33 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:07:34 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:07:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:07:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:07:34 GMT
USER varnish
# Fri, 16 Sep 2022 01:07:34 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:07:34 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837ab6cca90169544033a72edbbc42950c0ac37d369014a8b865475c25929d7d`  
		Last Modified: Fri, 16 Sep 2022 01:09:28 GMT  
		Size: 56.3 MB (56314670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbc457d33c646badce8896611b19df90fb5cc01d79b798d6efbf1b12cfc84ea`  
		Last Modified: Fri, 16 Sep 2022 01:09:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:51ebe92fa5740ff0d791d15cd441a8b32d6eeff785f0089ac4f077921ab6217e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100529442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1558f14eaa2d5575200e445de6b40e630fabe003647d522f2c1ff6f35471da`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:47:36 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:47:37 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:47:38 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:47:39 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:47:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:47:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:47:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:47:45 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:47:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:59:13 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:59:14 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:59:15 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:59:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:59:16 GMT
USER varnish
# Fri, 16 Sep 2022 00:59:17 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:59:18 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c970cc9dde8076da5c6f21786dd260fec5eeff61c971177d7eda600f72d0bd75`  
		Last Modified: Fri, 16 Sep 2022 01:00:17 GMT  
		Size: 70.5 MB (70474710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99af8e91aa17958255f36cc3c0bb2a23122da60b990136cb11e1c7159e1dbd42`  
		Last Modified: Fri, 16 Sep 2022 01:00:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1` - linux; 386

```console
$ docker pull varnish@sha256:ca00e9197a158235394e55ac80e116054690d973b61024ab5288c5f00d97f920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107894486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d157e840659f240aa4691e7f7f1fc9c43a8b7e0719341d00f6ff535342f3d100`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:39:38 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:39:39 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:39:40 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:39:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:39:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:39:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:39:44 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:39:45 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:39:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:39:47 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:39:48 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:46:33 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:46:34 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:46:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:46:36 GMT
USER varnish
# Fri, 16 Sep 2022 00:46:37 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:46:38 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf4fd1bf9eb0d00791f595ede4056ac426b9cb5e92a83b8540a7d57d51a915`  
		Last Modified: Fri, 16 Sep 2022 00:49:02 GMT  
		Size: 75.5 MB (75510208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f49a2344808e983420284ba4af102676307b3e4e57205cee8cefcd0f196b73`  
		Last Modified: Fri, 16 Sep 2022 00:48:52 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:387cd6794baf021e9362961e2384acbdb25e98fe9a1a394bb6ca859c3c0d3c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104492792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884a34f4825b0e2e99e750df9c6eb4d44c28ff0a026a3d8932d446f01665b1f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:48:48 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 10:48:48 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 10:48:48 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 10:48:50 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 10:54:43 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 10:54:46 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 10:54:46 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:54:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 10:54:47 GMT
USER varnish
# Tue, 13 Sep 2022 10:54:47 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 10:54:48 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e8423909e32907c374b40534ee89da2efcdb5bb4761bad98dbc593e3aa29e`  
		Last Modified: Tue, 13 Sep 2022 11:06:10 GMT  
		Size: 69.2 MB (69214925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeee3ea66d867696a8db281c80b7caa089b11024d1e616add57c163aebb4ad8`  
		Last Modified: Tue, 13 Sep 2022 11:05:53 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1` - linux; s390x

```console
$ docker pull varnish@sha256:94533056a29ed197fe0a3b8d7e3267730a8b9550a81604729665a744362ec716
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85727466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:024c8b5a25f9e560b63b1bb14f3a0c93d14354a7ac3b3a849c93566bab34ccd3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:53:42 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 06:53:42 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 06:53:42 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 06:53:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 06:53:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 06:53:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 06:56:13 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 06:56:15 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 06:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:56:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 06:56:16 GMT
USER varnish
# Tue, 13 Sep 2022 06:56:16 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 06:56:16 GMT
CMD []
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04976f863b25f9dbf72873d6cdbccf813a5d2db0ca7818d68284fc6d588ed2ac`  
		Last Modified: Tue, 13 Sep 2022 07:00:20 GMT  
		Size: 56.1 MB (56091911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dcdef6310d5d684296de769c6877cf4dbf99739f5b1af7dfe9555972fef90a`  
		Last Modified: Tue, 13 Sep 2022 07:00:13 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.1-alpine`

```console
$ docker pull varnish@sha256:81257c6d7d2a44b04b667945fdadbaf89cd18b55d0353128396a035e5a77c410
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.1.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:e06e93886caf501e38c01e0cf44514d3366110552961fe17a7d17ff3efff3ca8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59071089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4cdf3802e46ef3f57ec91755bcfd5bb19b6336c84e8097bcfeabb37b807dd5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:27:09 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:31 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:31 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:31 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:32 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:25:47 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:25:48 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:27:36 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:27:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:27:37 GMT
USER varnish
# Fri, 16 Sep 2022 00:27:37 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:27:37 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07f5c00a3fca42168beb309a1da4497d81192fcd78cb270293088a816212694`  
		Last Modified: Thu, 11 Aug 2022 18:29:57 GMT  
		Size: 56.2 MB (56247081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73638df192f2f0445e49db4333e9a9f39e26938968e3c796a81c87fae3df9015`  
		Last Modified: Fri, 16 Sep 2022 00:29:11 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c6b22c4963a1cec7a22ba1a943823cf54e5a5c1b2b9ac286fed3a0029174cb96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44838985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c6a6655fc442310bfb54f8b59a9ccfb5405c8a0bb74e1020d1aa128f99cb1d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 04:07:16 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:01:20 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:01:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:01:21 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:01:21 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:03:23 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:03:24 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:07:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:07:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:07:40 GMT
USER varnish
# Fri, 16 Sep 2022 01:07:40 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:07:40 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6526057e940a58d88649203706292e565d300408dfb557a419d381f3ffd9b83`  
		Last Modified: Thu, 11 Aug 2022 18:08:20 GMT  
		Size: 42.4 MB (42403394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690ee8cc9fd56bce463253ce04df4f0a2516e0d70b4a66686ccc509d6b7eeeb2`  
		Last Modified: Fri, 16 Sep 2022 01:09:43 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:b5f5c38564b8c68d2c89cb0c5cf07cf929d7c6c29623985a41e66df8fa1d7ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51804113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:318da3f2dbda7664008e779ce42a20556100d6c8e8acea62c90fac68535d7bc5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:16:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:51:52 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:51:53 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:51:54 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:51:55 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:51:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:51:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:51:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:51:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:52:00 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:52:01 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:53:20 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:53:20 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:59:30 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:59:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:59:31 GMT
USER varnish
# Fri, 16 Sep 2022 00:59:32 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:59:33 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66637d73d151e7b8d3fe367559b7457ef1203d2aebfd50c2e70fd5bf1e99c081`  
		Last Modified: Thu, 11 Aug 2022 17:58:22 GMT  
		Size: 49.1 MB (49085174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac15dc4fc673a317837b93832817c5e204d3aff8a6f781c1aeed2c550eb0203a`  
		Last Modified: Fri, 16 Sep 2022 01:00:31 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:fc0aba45a3efd75271ef52fe059638e8a931fc594087a18c4653715ea78a8dde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59260455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7289c0f508c7f43337e64f4f82329aa9deab92bfb820139adff8bf251bf79bd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:03:37 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:42:11 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:42:12 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:42:13 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:42:14 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:42:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:42:16 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:42:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:42:18 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:42:19 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:42:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:43:37 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:43:37 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:46:48 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:46:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:46:49 GMT
USER varnish
# Fri, 16 Sep 2022 00:46:50 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:46:51 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48542280e8f5e646fe63a44668949d53d57e9c3f41a0308717d0f58f2c9038e3`  
		Last Modified: Thu, 11 Aug 2022 17:48:38 GMT  
		Size: 56.4 MB (56431439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6279ed53a3e61eb8ad01dc9fa88f7e0be37a3bf70d2ddaa540a2d49788d3b0a`  
		Last Modified: Fri, 16 Sep 2022 00:49:15 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:afb06d7114e815bd133ac5b96241965064541f406cb5707f6c41157d02dbf40b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48872166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3709d135f1017d354137d2bc10fa3c292b86320cf2e4f192d99555c5ecc09fa3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:13:06 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:41 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:44 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:26:34 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:26:37 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:28:32 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:28:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:28:33 GMT
USER varnish
# Fri, 16 Sep 2022 00:28:33 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:28:33 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a15064fbadc2b9bce565fe7971fba76bf7ae75f6d59ef2522607a17e18fb60`  
		Last Modified: Thu, 11 Aug 2022 18:35:48 GMT  
		Size: 46.1 MB (46058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1af803614fcc096ee8ba2285a9d578ffed5f1eaded260624ac7a413e1e337e`  
		Last Modified: Fri, 16 Sep 2022 00:28:59 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:ecf905f62dca3c6c7db7de8bcdf43c42e4ae1c5dc635c19b818bc3ac1bbfd565
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47321925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faddc4fd662ea6dbedb36db17ab477108f0cc14c51de05c9973344b01fbe4e2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:54:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:46:35 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:46:35 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:46:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:48:19 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:48:25 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:51:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:51:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:51:06 GMT
USER varnish
# Fri, 16 Sep 2022 00:51:06 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:51:06 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694fec8cf4b1f4958bdd7c4941f751e5c9df3eb875c8003dccefe1dd9cfce4e2`  
		Last Modified: Thu, 11 Aug 2022 17:56:53 GMT  
		Size: 44.7 MB (44715342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aef5c8565b8c4c641ab0b36f868644a4a2132bc4da1ccc7f8ab18efd4f4596`  
		Last Modified: Fri, 16 Sep 2022 00:51:36 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2`

```console
$ docker pull varnish@sha256:07de59281e8de107d79384da13b4a22ea479258b3f7a96dac4e29d362aaa252b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `varnish:7.2` - linux; amd64

```console
$ docker pull varnish@sha256:ac25649870433f81f22ca973603dc1d0f5dd1148db92da31dcafc786a5c2205c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106839342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:502365b7eda42038a7b4881a333bb3d4267f40c65c49f770a1e7aff905c8ffa6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:20:12 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:20:13 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:23:05 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:23:06 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:23:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:23:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:23:06 GMT
USER varnish
# Fri, 16 Sep 2022 00:23:06 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:23:07 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42006373584e39a01bde292642b6b6756a735be8928a22bbad358065b05eadd`  
		Last Modified: Fri, 16 Sep 2022 00:28:09 GMT  
		Size: 75.4 MB (75434730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428dd53b0e8d1693d05f12c459a8adfc1fcc36f64374ee9dc5e39c5e81ea43b`  
		Last Modified: Fri, 16 Sep 2022 00:27:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; arm variant v7

```console
$ docker pull varnish@sha256:49dbcfe00cee33208e0e5f85e567fc4e84b91ab99c9b26cdc4afa7b45ecb387f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83180209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42cd64097f5fdb743cc48289e95967c0685ef4bd18e7355f4f920f717651788`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:58:10 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:58:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:01:43 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:01:43 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:01:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:01:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:01:44 GMT
USER varnish
# Fri, 16 Sep 2022 01:01:44 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:01:44 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a6cd0e18662964d280804dd01554de8bb9b971a029c354b7efe6cb49e95598`  
		Last Modified: Fri, 16 Sep 2022 01:08:38 GMT  
		Size: 56.6 MB (56612656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7b32473cf4d3042ee50dff41ffb77f52e5a3aba63dc3900fce85ef5eeee469`  
		Last Modified: Fri, 16 Sep 2022 01:08:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2` - linux; 386

```console
$ docker pull varnish@sha256:d94a5806dde228730c1a5010c198565b4aceb2aa79403d2603214adb23b8a4a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108210824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5926f9317e97cf459f5aa8532ea5877dbd3c84faf1e52ec9e89e62910428707`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:38:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:38:57 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:38:58 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:38:59 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:39:00 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:39:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:39:02 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:39:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:39:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:39:05 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:39:06 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:41:55 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:41:55 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:41:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:41:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:41:58 GMT
USER varnish
# Fri, 16 Sep 2022 00:41:59 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:42:00 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa1b00fb0e7dcf76da750e7eeac34b1b57900cb36f2c0b445c9e9908f81d89`  
		Last Modified: Fri, 16 Sep 2022 00:48:09 GMT  
		Size: 75.8 MB (75826543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdca77082062b163027c1b0218cad42bc34d330971868e3281e1cd38a5acd8f`  
		Last Modified: Fri, 16 Sep 2022 00:48:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2-alpine`

```console
$ docker pull varnish@sha256:7fe87650e04b01829e591d422e6786326477629638de619b3dee2530f4c2f1e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `varnish:7.2-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:ef17c17fdcea34d65990bb50e656a81b3becca39155145b1dab0ee56a61a10a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fac30dc1fd6914f554db55eccfbd5a4f705f454135bfc9631e77ece17cb7597`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:23:20 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:23:20 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:23:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:24:35 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:24:36 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:24:36 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:24:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:24:36 GMT
USER varnish
# Fri, 16 Sep 2022 00:24:36 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:24:36 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1909f664b2216d22acfb48beb89bcafb752a1686070b08b6335248f35de7d7d2`  
		Last Modified: Fri, 16 Sep 2022 00:28:31 GMT  
		Size: 56.6 MB (56573383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b37653782d6d27108bd803806ff900bf67f525f5708cbe366cfae4118707c9`  
		Last Modified: Fri, 16 Sep 2022 00:28:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:411ee92c511224a69f1b8410129148528e6cdb54f3ca2d7bf6f8d6d7e56d8f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a2caf60a24c546c8a9968c3bb600c822afc216ecd4a2f2612872fe6106272f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 01:01:50 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 01:01:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:03:57 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:03:57 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:03:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:03:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:03:57 GMT
USER varnish
# Fri, 16 Sep 2022 01:03:57 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:03:57 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7320892a7243b5fbbe7f135b1f5b6ca479e9247dd1c2323348040dc69b8cd99`  
		Last Modified: Fri, 16 Sep 2022 01:09:02 GMT  
		Size: 42.7 MB (42712648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9166e5ac4946000e07e74ef1ac6d26bfb6d0c25eda3dc65e0b80ac8b1e5a51`  
		Last Modified: Fri, 16 Sep 2022 01:08:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2-alpine` - linux; 386

```console
$ docker pull varnish@sha256:4c5d53f6eac73b1b835a422b6c3967b9049208ced971d31b73246d4d14ceeb4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59567119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4f5f548b25d23a022a00d354529b3d7f29645afa7c259cfa4db5ed378f1adf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:42:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:42:09 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:42:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:42:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:42:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:42:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:42:14 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:42:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:42:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:42:17 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:42:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:43:38 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:43:39 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:43:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:43:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:43:41 GMT
USER varnish
# Fri, 16 Sep 2022 00:43:42 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:43:43 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3037481039cd1db3531c7508c96b2301a31a19c9cd2b4e746e5f6a1e17ca9f`  
		Last Modified: Fri, 16 Sep 2022 00:48:36 GMT  
		Size: 56.7 MB (56738103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72f8e94ab3ee1b398b1eb1fc512705e474651279d495668e74b0962a10a78c3`  
		Last Modified: Fri, 16 Sep 2022 00:48:29 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2.0`

```console
$ docker pull varnish@sha256:07de59281e8de107d79384da13b4a22ea479258b3f7a96dac4e29d362aaa252b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `varnish:7.2.0` - linux; amd64

```console
$ docker pull varnish@sha256:ac25649870433f81f22ca973603dc1d0f5dd1148db92da31dcafc786a5c2205c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106839342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:502365b7eda42038a7b4881a333bb3d4267f40c65c49f770a1e7aff905c8ffa6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:20:12 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:20:13 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:23:05 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:23:06 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:23:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:23:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:23:06 GMT
USER varnish
# Fri, 16 Sep 2022 00:23:06 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:23:07 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42006373584e39a01bde292642b6b6756a735be8928a22bbad358065b05eadd`  
		Last Modified: Fri, 16 Sep 2022 00:28:09 GMT  
		Size: 75.4 MB (75434730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428dd53b0e8d1693d05f12c459a8adfc1fcc36f64374ee9dc5e39c5e81ea43b`  
		Last Modified: Fri, 16 Sep 2022 00:27:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:49dbcfe00cee33208e0e5f85e567fc4e84b91ab99c9b26cdc4afa7b45ecb387f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83180209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42cd64097f5fdb743cc48289e95967c0685ef4bd18e7355f4f920f717651788`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:58:10 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:58:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:01:43 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:01:43 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:01:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:01:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:01:44 GMT
USER varnish
# Fri, 16 Sep 2022 01:01:44 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:01:44 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a6cd0e18662964d280804dd01554de8bb9b971a029c354b7efe6cb49e95598`  
		Last Modified: Fri, 16 Sep 2022 01:08:38 GMT  
		Size: 56.6 MB (56612656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7b32473cf4d3042ee50dff41ffb77f52e5a3aba63dc3900fce85ef5eeee469`  
		Last Modified: Fri, 16 Sep 2022 01:08:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.0` - linux; 386

```console
$ docker pull varnish@sha256:d94a5806dde228730c1a5010c198565b4aceb2aa79403d2603214adb23b8a4a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108210824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5926f9317e97cf459f5aa8532ea5877dbd3c84faf1e52ec9e89e62910428707`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:38:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:38:57 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:38:58 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:38:59 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:39:00 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:39:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:39:02 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:39:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:39:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:39:05 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:39:06 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:41:55 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:41:55 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:41:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:41:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:41:58 GMT
USER varnish
# Fri, 16 Sep 2022 00:41:59 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:42:00 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa1b00fb0e7dcf76da750e7eeac34b1b57900cb36f2c0b445c9e9908f81d89`  
		Last Modified: Fri, 16 Sep 2022 00:48:09 GMT  
		Size: 75.8 MB (75826543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdca77082062b163027c1b0218cad42bc34d330971868e3281e1cd38a5acd8f`  
		Last Modified: Fri, 16 Sep 2022 00:48:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.2.0-alpine`

```console
$ docker pull varnish@sha256:7fe87650e04b01829e591d422e6786326477629638de619b3dee2530f4c2f1e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `varnish:7.2.0-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:ef17c17fdcea34d65990bb50e656a81b3becca39155145b1dab0ee56a61a10a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fac30dc1fd6914f554db55eccfbd5a4f705f454135bfc9631e77ece17cb7597`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:23:20 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:23:20 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:23:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:24:35 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:24:36 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:24:36 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:24:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:24:36 GMT
USER varnish
# Fri, 16 Sep 2022 00:24:36 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:24:36 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1909f664b2216d22acfb48beb89bcafb752a1686070b08b6335248f35de7d7d2`  
		Last Modified: Fri, 16 Sep 2022 00:28:31 GMT  
		Size: 56.6 MB (56573383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b37653782d6d27108bd803806ff900bf67f525f5708cbe366cfae4118707c9`  
		Last Modified: Fri, 16 Sep 2022 00:28:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:411ee92c511224a69f1b8410129148528e6cdb54f3ca2d7bf6f8d6d7e56d8f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a2caf60a24c546c8a9968c3bb600c822afc216ecd4a2f2612872fe6106272f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 01:01:50 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 01:01:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:03:57 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:03:57 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:03:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:03:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:03:57 GMT
USER varnish
# Fri, 16 Sep 2022 01:03:57 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:03:57 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7320892a7243b5fbbe7f135b1f5b6ca479e9247dd1c2323348040dc69b8cd99`  
		Last Modified: Fri, 16 Sep 2022 01:09:02 GMT  
		Size: 42.7 MB (42712648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9166e5ac4946000e07e74ef1ac6d26bfb6d0c25eda3dc65e0b80ac8b1e5a51`  
		Last Modified: Fri, 16 Sep 2022 01:08:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.2.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:4c5d53f6eac73b1b835a422b6c3967b9049208ced971d31b73246d4d14ceeb4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59567119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4f5f548b25d23a022a00d354529b3d7f29645afa7c259cfa4db5ed378f1adf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:42:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:42:09 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:42:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:42:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:42:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:42:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:42:14 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:42:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:42:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:42:17 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:42:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:43:38 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:43:39 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:43:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:43:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:43:41 GMT
USER varnish
# Fri, 16 Sep 2022 00:43:42 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:43:43 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3037481039cd1db3531c7508c96b2301a31a19c9cd2b4e746e5f6a1e17ca9f`  
		Last Modified: Fri, 16 Sep 2022 00:48:36 GMT  
		Size: 56.7 MB (56738103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72f8e94ab3ee1b398b1eb1fc512705e474651279d495668e74b0962a10a78c3`  
		Last Modified: Fri, 16 Sep 2022 00:48:29 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:82485cc5dd483b170dd080407ceca060bf1b7250fabc00d99479025af32aa3cc
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
$ docker pull varnish@sha256:ef17c17fdcea34d65990bb50e656a81b3becca39155145b1dab0ee56a61a10a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fac30dc1fd6914f554db55eccfbd5a4f705f454135bfc9631e77ece17cb7597`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:23:20 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:23:20 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:23:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:24:35 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:24:36 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:24:36 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:24:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:24:36 GMT
USER varnish
# Fri, 16 Sep 2022 00:24:36 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:24:36 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1909f664b2216d22acfb48beb89bcafb752a1686070b08b6335248f35de7d7d2`  
		Last Modified: Fri, 16 Sep 2022 00:28:31 GMT  
		Size: 56.6 MB (56573383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b37653782d6d27108bd803806ff900bf67f525f5708cbe366cfae4118707c9`  
		Last Modified: Fri, 16 Sep 2022 00:28:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:411ee92c511224a69f1b8410129148528e6cdb54f3ca2d7bf6f8d6d7e56d8f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a2caf60a24c546c8a9968c3bb600c822afc216ecd4a2f2612872fe6106272f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 01:01:50 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 01:01:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:03:57 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:03:57 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:03:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:03:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:03:57 GMT
USER varnish
# Fri, 16 Sep 2022 01:03:57 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:03:57 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7320892a7243b5fbbe7f135b1f5b6ca479e9247dd1c2323348040dc69b8cd99`  
		Last Modified: Fri, 16 Sep 2022 01:09:02 GMT  
		Size: 42.7 MB (42712648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9166e5ac4946000e07e74ef1ac6d26bfb6d0c25eda3dc65e0b80ac8b1e5a51`  
		Last Modified: Fri, 16 Sep 2022 01:08:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:717487768ed81ea94dcd6748da9228cb8fe1b81073556069cb80a5a73295860a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51804094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee536e43e5fad78caf269808dfee93cd9e76b376e813eb5964549278149e59b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:16:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:51:52 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:51:53 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:51:54 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:51:55 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:51:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:51:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:51:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:51:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:52:00 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:52:01 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:53:20 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:53:20 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:53:22 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:53:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:53:23 GMT
USER varnish
# Thu, 11 Aug 2022 17:53:24 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:53:25 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66637d73d151e7b8d3fe367559b7457ef1203d2aebfd50c2e70fd5bf1e99c081`  
		Last Modified: Thu, 11 Aug 2022 17:58:22 GMT  
		Size: 49.1 MB (49085174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b2c3b885888b477b35c280e036923c88b655803b494242a5f224b80f8ceed`  
		Last Modified: Thu, 11 Aug 2022 17:58:15 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:4c5d53f6eac73b1b835a422b6c3967b9049208ced971d31b73246d4d14ceeb4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59567119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4f5f548b25d23a022a00d354529b3d7f29645afa7c259cfa4db5ed378f1adf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:42:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:42:09 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:42:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:42:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:42:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:42:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:42:14 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:42:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:42:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:42:17 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:42:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:43:38 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:43:39 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:43:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:43:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:43:41 GMT
USER varnish
# Fri, 16 Sep 2022 00:43:42 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:43:43 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3037481039cd1db3531c7508c96b2301a31a19c9cd2b4e746e5f6a1e17ca9f`  
		Last Modified: Fri, 16 Sep 2022 00:48:36 GMT  
		Size: 56.7 MB (56738103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72f8e94ab3ee1b398b1eb1fc512705e474651279d495668e74b0962a10a78c3`  
		Last Modified: Fri, 16 Sep 2022 00:48:29 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:30297707c2dea193bfd2f5f51f569d60a07ab77e2c3bbd04fa2d3cd1e5a9ba1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48872146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198c71b8b6d1f902598d81b5071bfdb145e03dbd456cc6450dbff7b15d3e124a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:13:06 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:41 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:44 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:26:34 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:26:37 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 18:26:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 18:26:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 18:26:38 GMT
USER varnish
# Thu, 11 Aug 2022 18:26:39 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 18:26:39 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a15064fbadc2b9bce565fe7971fba76bf7ae75f6d59ef2522607a17e18fb60`  
		Last Modified: Thu, 11 Aug 2022 18:35:48 GMT  
		Size: 46.1 MB (46058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ce3575e5c3e8299b4379e48b60fd9a86b324975077480e6b6099c2d229a0c7`  
		Last Modified: Thu, 11 Aug 2022 18:35:36 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:ef0bc428fc8797be18df6dbab001bd40862f568a9b2c21fdb3649b31e4caf168
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47321908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:469bd0d9c7f85d2ba2e3eec193b415418ebc882b89f18eb37d1fde4b613c0f78`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:54:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:46:35 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:46:35 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:46:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:48:19 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:48:25 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:48:25 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:48:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:48:26 GMT
USER varnish
# Thu, 11 Aug 2022 17:48:26 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:48:27 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694fec8cf4b1f4958bdd7c4941f751e5c9df3eb875c8003dccefe1dd9cfce4e2`  
		Last Modified: Thu, 11 Aug 2022 17:56:53 GMT  
		Size: 44.7 MB (44715342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e69ac324df99a42204cf390757a838e28f80ceb7564f1e690948bcba9a7e14c`  
		Last Modified: Thu, 11 Aug 2022 17:56:48 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:c8503c744ea22f1a22c3af63fb181a79519ca6856bcd0288c76e9c2d6b1f0180
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
$ docker pull varnish@sha256:ac25649870433f81f22ca973603dc1d0f5dd1148db92da31dcafc786a5c2205c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106839342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:502365b7eda42038a7b4881a333bb3d4267f40c65c49f770a1e7aff905c8ffa6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:20:12 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:20:13 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:23:05 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:23:06 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:23:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:23:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:23:06 GMT
USER varnish
# Fri, 16 Sep 2022 00:23:06 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:23:07 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42006373584e39a01bde292642b6b6756a735be8928a22bbad358065b05eadd`  
		Last Modified: Fri, 16 Sep 2022 00:28:09 GMT  
		Size: 75.4 MB (75434730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428dd53b0e8d1693d05f12c459a8adfc1fcc36f64374ee9dc5e39c5e81ea43b`  
		Last Modified: Fri, 16 Sep 2022 00:27:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:49dbcfe00cee33208e0e5f85e567fc4e84b91ab99c9b26cdc4afa7b45ecb387f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83180209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42cd64097f5fdb743cc48289e95967c0685ef4bd18e7355f4f920f717651788`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:58:10 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:58:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:01:43 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:01:43 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:01:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:01:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:01:44 GMT
USER varnish
# Fri, 16 Sep 2022 01:01:44 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:01:44 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a6cd0e18662964d280804dd01554de8bb9b971a029c354b7efe6cb49e95598`  
		Last Modified: Fri, 16 Sep 2022 01:08:38 GMT  
		Size: 56.6 MB (56612656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7b32473cf4d3042ee50dff41ffb77f52e5a3aba63dc3900fce85ef5eeee469`  
		Last Modified: Fri, 16 Sep 2022 01:08:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:07bbbdb43cac6d60fa13d7f99a2960dfc7e29fea102984539e603067c51f15e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99412516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2938bfd77b00a8f5dc79537b75c6f9302fc1008081483716398c168b536e5fcc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:47:36 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:47:37 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:47:38 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:47:39 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:47:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:47:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:47:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:47:45 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:47:46 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:50:44 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 13:50:45 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:50:46 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:50:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:50:47 GMT
USER varnish
# Tue, 13 Sep 2022 13:50:48 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:50:49 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc53de5761eead687d57c6833225c1b27e8f0fbafb9bde67ecfb7cd0ca0034c`  
		Last Modified: Tue, 13 Sep 2022 13:56:50 GMT  
		Size: 69.4 MB (69357802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371c28164205f4cb5ff1c3f63c3e8091ab05bde41b7cb9333d92eb92d73b7b10`  
		Last Modified: Tue, 13 Sep 2022 13:56:41 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:d94a5806dde228730c1a5010c198565b4aceb2aa79403d2603214adb23b8a4a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108210824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5926f9317e97cf459f5aa8532ea5877dbd3c84faf1e52ec9e89e62910428707`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:38:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:38:57 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:38:58 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:38:59 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:39:00 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:39:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:39:02 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:39:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:39:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:39:05 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:39:06 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:41:55 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:41:55 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:41:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:41:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:41:58 GMT
USER varnish
# Fri, 16 Sep 2022 00:41:59 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:42:00 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa1b00fb0e7dcf76da750e7eeac34b1b57900cb36f2c0b445c9e9908f81d89`  
		Last Modified: Fri, 16 Sep 2022 00:48:09 GMT  
		Size: 75.8 MB (75826543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdca77082062b163027c1b0218cad42bc34d330971868e3281e1cd38a5acd8f`  
		Last Modified: Fri, 16 Sep 2022 00:48:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:387cd6794baf021e9362961e2384acbdb25e98fe9a1a394bb6ca859c3c0d3c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104492792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884a34f4825b0e2e99e750df9c6eb4d44c28ff0a026a3d8932d446f01665b1f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:48:48 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 10:48:48 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 10:48:48 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 10:48:50 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 10:54:43 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 10:54:46 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 10:54:46 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:54:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 10:54:47 GMT
USER varnish
# Tue, 13 Sep 2022 10:54:47 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 10:54:48 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e8423909e32907c374b40534ee89da2efcdb5bb4761bad98dbc593e3aa29e`  
		Last Modified: Tue, 13 Sep 2022 11:06:10 GMT  
		Size: 69.2 MB (69214925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeee3ea66d867696a8db281c80b7caa089b11024d1e616add57c163aebb4ad8`  
		Last Modified: Tue, 13 Sep 2022 11:05:53 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:94533056a29ed197fe0a3b8d7e3267730a8b9550a81604729665a744362ec716
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85727466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:024c8b5a25f9e560b63b1bb14f3a0c93d14354a7ac3b3a849c93566bab34ccd3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:53:42 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 06:53:42 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 06:53:42 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 06:53:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 06:53:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 06:53:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 06:56:13 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 06:56:15 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 06:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:56:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 06:56:16 GMT
USER varnish
# Tue, 13 Sep 2022 06:56:16 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 06:56:16 GMT
CMD []
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04976f863b25f9dbf72873d6cdbccf813a5d2db0ca7818d68284fc6d588ed2ac`  
		Last Modified: Tue, 13 Sep 2022 07:00:20 GMT  
		Size: 56.1 MB (56091911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dcdef6310d5d684296de769c6877cf4dbf99739f5b1af7dfe9555972fef90a`  
		Last Modified: Tue, 13 Sep 2022 07:00:13 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:82485cc5dd483b170dd080407ceca060bf1b7250fabc00d99479025af32aa3cc
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
$ docker pull varnish@sha256:ef17c17fdcea34d65990bb50e656a81b3becca39155145b1dab0ee56a61a10a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fac30dc1fd6914f554db55eccfbd5a4f705f454135bfc9631e77ece17cb7597`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:23:20 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:23:20 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:23:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:23:21 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:24:35 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:24:36 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:24:36 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:24:36 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:24:36 GMT
USER varnish
# Fri, 16 Sep 2022 00:24:36 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:24:36 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1909f664b2216d22acfb48beb89bcafb752a1686070b08b6335248f35de7d7d2`  
		Last Modified: Fri, 16 Sep 2022 00:28:31 GMT  
		Size: 56.6 MB (56573383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b37653782d6d27108bd803806ff900bf67f525f5708cbe366cfae4118707c9`  
		Last Modified: Fri, 16 Sep 2022 00:28:23 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:411ee92c511224a69f1b8410129148528e6cdb54f3ca2d7bf6f8d6d7e56d8f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a2caf60a24c546c8a9968c3bb600c822afc216ecd4a2f2612872fe6106272f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 01:01:50 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 01:01:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 01:01:51 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:03:57 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:03:57 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:03:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:03:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:03:57 GMT
USER varnish
# Fri, 16 Sep 2022 01:03:57 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:03:57 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7320892a7243b5fbbe7f135b1f5b6ca479e9247dd1c2323348040dc69b8cd99`  
		Last Modified: Fri, 16 Sep 2022 01:09:02 GMT  
		Size: 42.7 MB (42712648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9166e5ac4946000e07e74ef1ac6d26bfb6d0c25eda3dc65e0b80ac8b1e5a51`  
		Last Modified: Fri, 16 Sep 2022 01:08:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:717487768ed81ea94dcd6748da9228cb8fe1b81073556069cb80a5a73295860a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51804094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee536e43e5fad78caf269808dfee93cd9e76b376e813eb5964549278149e59b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:16:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:51:52 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:51:53 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:51:54 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:51:55 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:51:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:51:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:51:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:51:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:52:00 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:52:01 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:53:20 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:53:20 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:53:22 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:53:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:53:23 GMT
USER varnish
# Thu, 11 Aug 2022 17:53:24 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:53:25 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66637d73d151e7b8d3fe367559b7457ef1203d2aebfd50c2e70fd5bf1e99c081`  
		Last Modified: Thu, 11 Aug 2022 17:58:22 GMT  
		Size: 49.1 MB (49085174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b2c3b885888b477b35c280e036923c88b655803b494242a5f224b80f8ceed`  
		Last Modified: Thu, 11 Aug 2022 17:58:15 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:4c5d53f6eac73b1b835a422b6c3967b9049208ced971d31b73246d4d14ceeb4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59567119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4f5f548b25d23a022a00d354529b3d7f29645afa7c259cfa4db5ed378f1adf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:42:08 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:42:09 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:42:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:42:11 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:42:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:42:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:42:14 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:42:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:42:16 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:42:17 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Fri, 16 Sep 2022 00:42:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:43:38 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:43:39 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:43:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:43:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:43:41 GMT
USER varnish
# Fri, 16 Sep 2022 00:43:42 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:43:43 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3037481039cd1db3531c7508c96b2301a31a19c9cd2b4e746e5f6a1e17ca9f`  
		Last Modified: Fri, 16 Sep 2022 00:48:36 GMT  
		Size: 56.7 MB (56738103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72f8e94ab3ee1b398b1eb1fc512705e474651279d495668e74b0962a10a78c3`  
		Last Modified: Fri, 16 Sep 2022 00:48:29 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:30297707c2dea193bfd2f5f51f569d60a07ab77e2c3bbd04fa2d3cd1e5a9ba1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48872146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198c71b8b6d1f902598d81b5071bfdb145e03dbd456cc6450dbff7b15d3e124a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:13:06 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:41 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:44 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:26:34 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:26:37 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 18:26:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 18:26:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 18:26:38 GMT
USER varnish
# Thu, 11 Aug 2022 18:26:39 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 18:26:39 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a15064fbadc2b9bce565fe7971fba76bf7ae75f6d59ef2522607a17e18fb60`  
		Last Modified: Thu, 11 Aug 2022 18:35:48 GMT  
		Size: 46.1 MB (46058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ce3575e5c3e8299b4379e48b60fd9a86b324975077480e6b6099c2d229a0c7`  
		Last Modified: Thu, 11 Aug 2022 18:35:36 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:ef0bc428fc8797be18df6dbab001bd40862f568a9b2c21fdb3649b31e4caf168
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47321908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:469bd0d9c7f85d2ba2e3eec193b415418ebc882b89f18eb37d1fde4b613c0f78`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:54:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:46:35 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:46:35 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:46:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:48:19 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:48:25 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:48:25 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:48:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:48:26 GMT
USER varnish
# Thu, 11 Aug 2022 17:48:26 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:48:27 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694fec8cf4b1f4958bdd7c4941f751e5c9df3eb875c8003dccefe1dd9cfce4e2`  
		Last Modified: Thu, 11 Aug 2022 17:56:53 GMT  
		Size: 44.7 MB (44715342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e69ac324df99a42204cf390757a838e28f80ceb7564f1e690948bcba9a7e14c`  
		Last Modified: Thu, 11 Aug 2022 17:56:48 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:c8503c744ea22f1a22c3af63fb181a79519ca6856bcd0288c76e9c2d6b1f0180
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
$ docker pull varnish@sha256:ac25649870433f81f22ca973603dc1d0f5dd1148db92da31dcafc786a5c2205c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106839342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:502365b7eda42038a7b4881a333bb3d4267f40c65c49f770a1e7aff905c8ffa6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:20:12 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:20:12 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:20:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:20:13 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:20:13 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:23:05 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:23:06 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:23:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:23:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:23:06 GMT
USER varnish
# Fri, 16 Sep 2022 00:23:06 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:23:07 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42006373584e39a01bde292642b6b6756a735be8928a22bbad358065b05eadd`  
		Last Modified: Fri, 16 Sep 2022 00:28:09 GMT  
		Size: 75.4 MB (75434730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428dd53b0e8d1693d05f12c459a8adfc1fcc36f64374ee9dc5e39c5e81ea43b`  
		Last Modified: Fri, 16 Sep 2022 00:27:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:49dbcfe00cee33208e0e5f85e567fc4e84b91ab99c9b26cdc4afa7b45ecb387f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83180209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42cd64097f5fdb743cc48289e95967c0685ef4bd18e7355f4f920f717651788`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:58:10 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:58:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:58:10 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:58:11 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:01:43 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:01:43 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:01:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:01:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:01:44 GMT
USER varnish
# Fri, 16 Sep 2022 01:01:44 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:01:44 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a6cd0e18662964d280804dd01554de8bb9b971a029c354b7efe6cb49e95598`  
		Last Modified: Fri, 16 Sep 2022 01:08:38 GMT  
		Size: 56.6 MB (56612656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7b32473cf4d3042ee50dff41ffb77f52e5a3aba63dc3900fce85ef5eeee469`  
		Last Modified: Fri, 16 Sep 2022 01:08:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:07bbbdb43cac6d60fa13d7f99a2960dfc7e29fea102984539e603067c51f15e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99412516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2938bfd77b00a8f5dc79537b75c6f9302fc1008081483716398c168b536e5fcc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:47:36 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:47:37 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:47:38 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:47:39 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:47:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:47:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:47:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:47:45 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:47:46 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:50:44 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 13:50:45 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:50:46 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:50:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:50:47 GMT
USER varnish
# Tue, 13 Sep 2022 13:50:48 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:50:49 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc53de5761eead687d57c6833225c1b27e8f0fbafb9bde67ecfb7cd0ca0034c`  
		Last Modified: Tue, 13 Sep 2022 13:56:50 GMT  
		Size: 69.4 MB (69357802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371c28164205f4cb5ff1c3f63c3e8091ab05bde41b7cb9333d92eb92d73b7b10`  
		Last Modified: Tue, 13 Sep 2022 13:56:41 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:d94a5806dde228730c1a5010c198565b4aceb2aa79403d2603214adb23b8a4a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108210824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5926f9317e97cf459f5aa8532ea5877dbd3c84faf1e52ec9e89e62910428707`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Fri, 16 Sep 2022 00:38:56 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:38:57 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:38:58 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:38:59 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:39:00 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:39:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:39:02 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:39:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:39:04 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 16 Sep 2022 00:39:05 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Fri, 16 Sep 2022 00:39:06 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:41:55 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.0.tgz -o $tmpdir/orig.tgz;     echo "d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:41:55 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:41:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:41:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:41:58 GMT
USER varnish
# Fri, 16 Sep 2022 00:41:59 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:42:00 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa1b00fb0e7dcf76da750e7eeac34b1b57900cb36f2c0b445c9e9908f81d89`  
		Last Modified: Fri, 16 Sep 2022 00:48:09 GMT  
		Size: 75.8 MB (75826543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdca77082062b163027c1b0218cad42bc34d330971868e3281e1cd38a5acd8f`  
		Last Modified: Fri, 16 Sep 2022 00:48:00 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:387cd6794baf021e9362961e2384acbdb25e98fe9a1a394bb6ca859c3c0d3c29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104492792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884a34f4825b0e2e99e750df9c6eb4d44c28ff0a026a3d8932d446f01665b1f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:48:48 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 10:48:48 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 10:48:48 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 10:48:49 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 10:48:50 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 10:48:50 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 10:48:51 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 10:54:43 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 10:54:46 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 10:54:46 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:54:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 10:54:47 GMT
USER varnish
# Tue, 13 Sep 2022 10:54:47 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 10:54:48 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4e8423909e32907c374b40534ee89da2efcdb5bb4761bad98dbc593e3aa29e`  
		Last Modified: Tue, 13 Sep 2022 11:06:10 GMT  
		Size: 69.2 MB (69214925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeee3ea66d867696a8db281c80b7caa089b11024d1e616add57c163aebb4ad8`  
		Last Modified: Tue, 13 Sep 2022 11:05:53 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:94533056a29ed197fe0a3b8d7e3267730a8b9550a81604729665a744362ec716
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85727466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:024c8b5a25f9e560b63b1bb14f3a0c93d14354a7ac3b3a849c93566bab34ccd3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:53:42 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 06:53:42 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 06:53:42 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 06:53:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 06:53:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 06:53:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 06:53:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 06:56:13 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 13 Sep 2022 06:56:15 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 06:56:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:56:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 06:56:16 GMT
USER varnish
# Tue, 13 Sep 2022 06:56:16 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 06:56:16 GMT
CMD []
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04976f863b25f9dbf72873d6cdbccf813a5d2db0ca7818d68284fc6d588ed2ac`  
		Last Modified: Tue, 13 Sep 2022 07:00:20 GMT  
		Size: 56.1 MB (56091911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dcdef6310d5d684296de769c6877cf4dbf99739f5b1af7dfe9555972fef90a`  
		Last Modified: Tue, 13 Sep 2022 07:00:13 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:93f1ee491f22f31466be60d790b68170e44404858cd40be201f5eb8d8f748f12
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
$ docker pull varnish@sha256:0e8f27d3cfb5a2d68e04074e15d1e8bc7ac9dab331055219cd6cd732cbddd021
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106514619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:324a8892e787c7c40773fdcaff3a2ae5fd21e9f0bb1c445b1be3e3b7792ab148`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:31:58 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:31:58 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:31:58 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:31:59 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:31:59 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:31:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:31:59 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:31:59 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:27:28 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:27:28 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:27:28 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:27:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:27:29 GMT
USER varnish
# Fri, 16 Sep 2022 00:27:29 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:27:29 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bc5fa37c18f8ef5e3cfacc07d2984665abb9543381738b2c53cb9322d40ce1`  
		Last Modified: Fri, 16 Sep 2022 00:28:54 GMT  
		Size: 75.1 MB (75110005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6325df2deb75046ab9f2ed04575d407626eab372b24c26f424907b04995e33e5`  
		Last Modified: Fri, 16 Sep 2022 00:28:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:392642824dbf95562e4be5f32ad959eae47c71195cc4a4f592549b86dfd9ce8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82882221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3df25f03198101a3267cba96f0a1b62785bbed5be1fb8e74c4971b66b1dd85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 09:12:45 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_VERSION=7.1.1
# Wed, 14 Sep 2022 09:12:45 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 14 Sep 2022 09:12:45 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 14 Sep 2022 09:12:46 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 14 Sep 2022 09:12:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 14 Sep 2022 09:12:46 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Wed, 14 Sep 2022 09:12:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 01:07:33 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 01:07:34 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:07:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:07:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:07:34 GMT
USER varnish
# Fri, 16 Sep 2022 01:07:34 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:07:34 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837ab6cca90169544033a72edbbc42950c0ac37d369014a8b865475c25929d7d`  
		Last Modified: Fri, 16 Sep 2022 01:09:28 GMT  
		Size: 56.3 MB (56314670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbc457d33c646badce8896611b19df90fb5cc01d79b798d6efbf1b12cfc84ea`  
		Last Modified: Fri, 16 Sep 2022 01:09:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:51ebe92fa5740ff0d791d15cd441a8b32d6eeff785f0089ac4f077921ab6217e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100529442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1558f14eaa2d5575200e445de6b40e630fabe003647d522f2c1ff6f35471da`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:47:36 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:47:37 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:47:38 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:47:39 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:47:40 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:47:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:47:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:47:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:47:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:47:45 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:47:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:59:13 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:59:14 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:59:15 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:59:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:59:16 GMT
USER varnish
# Fri, 16 Sep 2022 00:59:17 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:59:18 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c970cc9dde8076da5c6f21786dd260fec5eeff61c971177d7eda600f72d0bd75`  
		Last Modified: Fri, 16 Sep 2022 01:00:17 GMT  
		Size: 70.5 MB (70474710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99af8e91aa17958255f36cc3c0bb2a23122da60b990136cb11e1c7159e1dbd42`  
		Last Modified: Fri, 16 Sep 2022 01:00:07 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:ca00e9197a158235394e55ac80e116054690d973b61024ab5288c5f00d97f920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107894486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d157e840659f240aa4691e7f7f1fc9c43a8b7e0719341d00f6ff535342f3d100`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:39:38 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 13 Sep 2022 13:39:39 GMT
ARG VARNISH_VERSION=7.1.1
# Tue, 13 Sep 2022 13:39:40 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Tue, 13 Sep 2022 13:39:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 13 Sep 2022 13:39:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 13 Sep 2022 13:39:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 13 Sep 2022 13:39:44 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Tue, 13 Sep 2022 13:39:45 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Tue, 13 Sep 2022 13:39:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Tue, 13 Sep 2022 13:39:47 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Tue, 13 Sep 2022 13:39:48 GMT
ENV VARNISH_SIZE=100M
# Fri, 16 Sep 2022 00:46:33 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Fri, 16 Sep 2022 00:46:34 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:46:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:46:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:46:36 GMT
USER varnish
# Fri, 16 Sep 2022 00:46:37 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:46:38 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf4fd1bf9eb0d00791f595ede4056ac426b9cb5e92a83b8540a7d57d51a915`  
		Last Modified: Fri, 16 Sep 2022 00:49:02 GMT  
		Size: 75.5 MB (75510208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f49a2344808e983420284ba4af102676307b3e4e57205cee8cefcd0f196b73`  
		Last Modified: Fri, 16 Sep 2022 00:48:52 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:d0a2b760121557cb94b520f2a934acdbad4c06fdb547edde643ba842f6023e74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100365171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1828c15f932f1e6e858475569866ec4c6d0b27da2be84fd68d8ae3b9b81a227d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:55:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 10:59:43 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.3.tgz -o $tmpdir/orig.tgz;     echo "515d5a60120228de381af5f78cd0b712ee77430c59c8760a1a027c5f5759c8f20f3ab79f4d3785f9f4ca3b1b62b0abb59d9e0b29010a879b6f93fa65e6b6f84d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.3|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 10:59:46 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 10:59:46 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 13 Sep 2022 10:59:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 10:59:47 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 10:59:47 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12b83bb4233042369930cd653c1e6831ee9fe778318d40589fe67dbe43432be`  
		Last Modified: Tue, 13 Sep 2022 11:06:49 GMT  
		Size: 65.1 MB (65087305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f1af3d216ad5340c9c62569fb8db93d72a556ae738b63700a3f21b33dbd665`  
		Last Modified: Tue, 13 Sep 2022 11:06:32 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:a7115290cb378d89994c87a110df2c64a3dba89196adefb2d40fe942fe0b51d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81710873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ee846e84940b0300ce72d5c41d6d4a38c4f2b765453c0e546d1f6331a38f3de`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 11:40:25 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:53:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.3.tgz -o $tmpdir/orig.tgz;     echo "515d5a60120228de381af5f78cd0b712ee77430c59c8760a1a027c5f5759c8f20f3ab79f4d3785f9f4ca3b1b62b0abb59d9e0b29010a879b6f93fa65e6b6f84d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.3|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 11 Aug 2022 17:53:26 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:53:26 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:53:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:53:27 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:53:27 GMT
CMD []
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6ab6eea21e17409b7654bac2f0fc6f26fd8104133e80bcb4bcbcc4e5b8196a`  
		Last Modified: Thu, 11 Aug 2022 17:57:13 GMT  
		Size: 52.1 MB (52070139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83de5e690835b31244ed1023a677c99da6e1a951724e8c0dc8c4aba24c29b16`  
		Last Modified: Thu, 11 Aug 2022 17:57:07 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:81257c6d7d2a44b04b667945fdadbaf89cd18b55d0353128396a035e5a77c410
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
$ docker pull varnish@sha256:e06e93886caf501e38c01e0cf44514d3366110552961fe17a7d17ff3efff3ca8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59071089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4cdf3802e46ef3f57ec91755bcfd5bb19b6336c84e8097bcfeabb37b807dd5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:27:09 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:31 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:31 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:31 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:31 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:32 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:25:47 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:25:48 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:27:36 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:27:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:27:37 GMT
USER varnish
# Fri, 16 Sep 2022 00:27:37 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:27:37 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07f5c00a3fca42168beb309a1da4497d81192fcd78cb270293088a816212694`  
		Last Modified: Thu, 11 Aug 2022 18:29:57 GMT  
		Size: 56.2 MB (56247081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73638df192f2f0445e49db4333e9a9f39e26938968e3c796a81c87fae3df9015`  
		Last Modified: Fri, 16 Sep 2022 00:29:11 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c6b22c4963a1cec7a22ba1a943823cf54e5a5c1b2b9ac286fed3a0029174cb96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44838985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19c6a6655fc442310bfb54f8b59a9ccfb5405c8a0bb74e1020d1aa128f99cb1d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 04:07:16 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:01:20 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:01:20 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:01:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:01:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:01:21 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:01:21 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:03:23 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:03:24 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 01:07:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 01:07:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 01:07:40 GMT
USER varnish
# Fri, 16 Sep 2022 01:07:40 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 01:07:40 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6526057e940a58d88649203706292e565d300408dfb557a419d381f3ffd9b83`  
		Last Modified: Thu, 11 Aug 2022 18:08:20 GMT  
		Size: 42.4 MB (42403394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690ee8cc9fd56bce463253ce04df4f0a2516e0d70b4a66686ccc509d6b7eeeb2`  
		Last Modified: Fri, 16 Sep 2022 01:09:43 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:b5f5c38564b8c68d2c89cb0c5cf07cf929d7c6c29623985a41e66df8fa1d7ccf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51804113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:318da3f2dbda7664008e779ce42a20556100d6c8e8acea62c90fac68535d7bc5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:16:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:51:52 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:51:53 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:51:54 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:51:55 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:51:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:51:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:51:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:51:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:52:00 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:52:01 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:53:20 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:53:20 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:59:30 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:59:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:59:31 GMT
USER varnish
# Fri, 16 Sep 2022 00:59:32 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:59:33 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66637d73d151e7b8d3fe367559b7457ef1203d2aebfd50c2e70fd5bf1e99c081`  
		Last Modified: Thu, 11 Aug 2022 17:58:22 GMT  
		Size: 49.1 MB (49085174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac15dc4fc673a317837b93832817c5e204d3aff8a6f781c1aeed2c550eb0203a`  
		Last Modified: Fri, 16 Sep 2022 01:00:31 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:fc0aba45a3efd75271ef52fe059638e8a931fc594087a18c4653715ea78a8dde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.3 MB (59260455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7289c0f508c7f43337e64f4f82329aa9deab92bfb820139adff8bf251bf79bd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:03:37 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:42:11 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:42:12 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:42:13 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:42:14 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:42:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:42:16 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:42:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:42:18 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:42:19 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:42:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:43:37 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:43:37 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:46:48 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:46:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:46:49 GMT
USER varnish
# Fri, 16 Sep 2022 00:46:50 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:46:51 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48542280e8f5e646fe63a44668949d53d57e9c3f41a0308717d0f58f2c9038e3`  
		Last Modified: Thu, 11 Aug 2022 17:48:38 GMT  
		Size: 56.4 MB (56431439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6279ed53a3e61eb8ad01dc9fa88f7e0be37a3bf70d2ddaa540a2d49788d3b0a`  
		Last Modified: Fri, 16 Sep 2022 00:49:15 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:afb06d7114e815bd133ac5b96241965064541f406cb5707f6c41157d02dbf40b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48872166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3709d135f1017d354137d2bc10fa3c292b86320cf2e4f192d99555c5ecc09fa3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:13:06 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:41 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:44 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:26:34 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:26:37 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:28:32 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:28:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:28:33 GMT
USER varnish
# Fri, 16 Sep 2022 00:28:33 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:28:33 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a15064fbadc2b9bce565fe7971fba76bf7ae75f6d59ef2522607a17e18fb60`  
		Last Modified: Thu, 11 Aug 2022 18:35:48 GMT  
		Size: 46.1 MB (46058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1af803614fcc096ee8ba2285a9d578ffed5f1eaded260624ac7a413e1e337e`  
		Last Modified: Fri, 16 Sep 2022 00:28:59 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:ecf905f62dca3c6c7db7de8bcdf43c42e4ae1c5dc635c19b818bc3ac1bbfd565
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47321925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8faddc4fd662ea6dbedb36db17ab477108f0cc14c51de05c9973344b01fbe4e2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:54:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:46:35 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:46:35 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:46:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:48:19 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:48:25 GMT
WORKDIR /etc/varnish
# Fri, 16 Sep 2022 00:51:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 16 Sep 2022 00:51:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 16 Sep 2022 00:51:06 GMT
USER varnish
# Fri, 16 Sep 2022 00:51:06 GMT
EXPOSE 80 8443
# Fri, 16 Sep 2022 00:51:06 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694fec8cf4b1f4958bdd7c4941f751e5c9df3eb875c8003dccefe1dd9cfce4e2`  
		Last Modified: Thu, 11 Aug 2022 17:56:53 GMT  
		Size: 44.7 MB (44715342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aef5c8565b8c4c641ab0b36f868644a4a2132bc4da1ccc7f8ab18efd4f4596`  
		Last Modified: Fri, 16 Sep 2022 00:51:36 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:f3e5ecdf63e9b1aac54ba5c9a17d378b7f0879a81168510c3075913fe0c0ac6b
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
$ docker pull varnish@sha256:7376c7bd35daf6fefbb13be6b0d09053c9179134e3d67eebb288c7470c9bde63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100644811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bd8d717b7c4c5985bb57a51e08edc1983492be02706815bae6715fe5305389`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:35:23 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:39:53 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 13:39:53 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:39:53 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:39:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:39:54 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:39:54 GMT
CMD []
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e60ef9ff523c960036ce4579422db4cb54a38db820f736cdfaf8197fa8dc97`  
		Last Modified: Tue, 13 Sep 2022 13:41:24 GMT  
		Size: 69.2 MB (69239988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5cccebb4545f0fb8c8850fb2fd4c089330f5e5ceb54fbad8167522f9a50c75`  
		Last Modified: Tue, 13 Sep 2022 13:41:15 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:8456945bbf5035d0da5e568b83f6901b311e6ce4737d2b7525ef2e81b1ee46f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77214448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23e0e371fff20134e85dd69951d6d8fc47e117a6608975b5a3683c84c99f8206`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 09:17:15 GMT
ENV VARNISH_SIZE=100M
# Wed, 14 Sep 2022 09:21:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 14 Sep 2022 09:21:59 GMT
WORKDIR /etc/varnish
# Wed, 14 Sep 2022 09:21:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 14 Sep 2022 09:21:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 14 Sep 2022 09:21:59 GMT
EXPOSE 80 8443
# Wed, 14 Sep 2022 09:21:59 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a97f0435f33c0b679f380d2e64c74751ca813df0058528016a5a6d6829a86f`  
		Last Modified: Wed, 14 Sep 2022 09:23:49 GMT  
		Size: 50.6 MB (50646687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fb9a273b672257943130cedb60e07d2394eae521ce1f123fffe6ab808ab8ef`  
		Last Modified: Wed, 14 Sep 2022 09:23:42 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e60be39c540957ef5d022a0b8e226a03a1dfce649c589f0139d9566276760c0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94700859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:050c6d2c69dae42ac73a197ecd1e63e4c8d87d2b483ca08568d3bf85c4098671`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:51:08 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 13:55:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 13:55:45 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 13:55:47 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 13:55:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 13:55:48 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 13:55:49 GMT
CMD []
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c06c206db57123dd985a252975427fb03e52722219cdba578d4350af7f9542`  
		Last Modified: Tue, 13 Sep 2022 13:57:44 GMT  
		Size: 64.6 MB (64645917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64363984b04e8cb866ab0fd7879b69b5f6704aef21c195ebe081d9b88a4a630d`  
		Last Modified: Tue, 13 Sep 2022 13:57:35 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:ee7530f27c0331063c0d85a1c4b569f2188ef865be698f40b7a4d1d4fddb604e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.2 MB (102162087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:849660f699b843c7cb096d3e5a0fa4167ca5dd73465d32041c23342096082294`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:50:05 GMT
ENV VARNISH_SIZE=100M
# Wed, 10 Aug 2022 00:10:58 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 10 Aug 2022 00:10:58 GMT
WORKDIR /etc/varnish
# Wed, 10 Aug 2022 00:11:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:11:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 10 Aug 2022 00:11:01 GMT
EXPOSE 80 8443
# Wed, 10 Aug 2022 00:11:02 GMT
CMD []
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551416d7a3fd6bd33021d63c1f1ed875e5c6bf8ac312001f2020f3c684b2d265`  
		Last Modified: Wed, 10 Aug 2022 00:13:19 GMT  
		Size: 69.8 MB (69787331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d53139023415366a342b716b2904d2191cf1e010e870137a180112974b28bf`  
		Last Modified: Wed, 10 Aug 2022 00:13:06 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:f4ef9cecfa3f21f34166c4313bd546c57254308e823f672003c02712391a40a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99780540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d95da7841ca570b682453a77e8c115254de7502ba0842fd135c0b1b5064abfa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:55:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 11:04:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 11:04:55 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 11:04:56 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:04:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 11:04:56 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 11:04:57 GMT
CMD []
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6b395186dad8fe056941c287ed6f5a2274254764f1c640e616faa8b81ded16`  
		Last Modified: Tue, 13 Sep 2022 11:07:23 GMT  
		Size: 64.5 MB (64502448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e80220ec6b0a4060a85ce7f7a790fe52300bc047d962ecfc2c8a2fd57c7b4ec`  
		Last Modified: Tue, 13 Sep 2022 11:07:06 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:98885dfc5266cea2aaf3f0345de157182204e4489499c4202c63ee559f9b057a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (80987355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:091248160e935dbb7c24d2a163688640176e0890c25589e93f886b7c4332473c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:56:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 13 Sep 2022 06:59:25 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 13 Sep 2022 06:59:27 GMT
WORKDIR /etc/varnish
# Tue, 13 Sep 2022 06:59:27 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:59:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 13 Sep 2022 06:59:27 GMT
EXPOSE 80 8443
# Tue, 13 Sep 2022 06:59:28 GMT
CMD []
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf394baf5aa4f42027ab215a1b68569c9e328288832fdda5565d5229ab4495a4`  
		Last Modified: Tue, 13 Sep 2022 07:00:44 GMT  
		Size: 51.4 MB (51351573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6633eb3e1a06ce29f4a4ba0ff4c8c423280d1250331682f18d851d981246d166`  
		Last Modified: Tue, 13 Sep 2022 07:00:37 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
