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
$ docker pull varnish@sha256:5a44aecc0e5464962ac12b89350e9e55310b9c771d0e4f6350f9fbfa419f3a61
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
$ docker pull varnish@sha256:45e8f5cb61f1575d50e71c4d87a3a16bee72bd8b0b721fd61931f6d3f772c624
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100589455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f2e90cfe6d081c7685e12181346aa9bc4761abc6b0005e37f13393f31c35d2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:50:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:56:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 11:56:16 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:56:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:56:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:56:16 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:56:16 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c0a85ce8de15827814d50bef44ecd40727b52f8b539af301efc2e1130d0d62`  
		Last Modified: Tue, 29 Mar 2022 11:58:23 GMT  
		Size: 69.2 MB (69210298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6189ac10d80aa022f66906092de569cf06a0a0a01f4f4680652bc7e0a1554b`  
		Last Modified: Tue, 29 Mar 2022 11:58:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:b6fb3fc16c82830efd88746b43fa1b8a337d759d0a706990c87609aa147e69dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77223459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a859bd351464452fdc554c75da983c30e3d62d33c01903dc2286c9c3c92474`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 00:49:05 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 01:09:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 01:09:19 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 01:09:19 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 19 Mar 2022 01:09:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 01:09:20 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 01:09:20 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2592eb74fa05949f18521eb0a3761a218f0ae6bbbf24414c24eb7aea00d8de`  
		Last Modified: Sat, 19 Mar 2022 01:14:10 GMT  
		Size: 50.6 MB (50647657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4252e8835c37e9eea96433c384a9cb37e5869a4b571c70cf97c734b65f4c19c`  
		Last Modified: Sat, 19 Mar 2022 01:13:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:d8de22cf7a21c15e114dd7e88382f20123b151ee152e56abe2bf4e6480aee8dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94710809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef56843c3c39b90f3ac6f000f594f52daf7f49bee705523c956ad57acc9e9a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:18:14 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:18:14 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:18:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:18:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:18:17 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:18:18 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3880751953be62fe965411a15ecbdf2e85f4efebef71a6e079897558c2753d29`  
		Last Modified: Thu, 17 Mar 2022 21:20:51 GMT  
		Size: 64.6 MB (64647095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdde89bc6b1d6118585a9c5cac45a4fc987141fbc08f3c4078644c51448b4da`  
		Last Modified: Thu, 17 Mar 2022 21:20:42 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:7a50b1ef0665d99ed29fad64e5cd3e251438a9cf8c3ce3ac6aae89b9531339fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102072518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6206c4b5e6f4b904b6c17c78084c5617713d6de7ad56a29367a38e9fead204`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:51:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:54:43 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 10:54:44 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:54:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:54:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:54:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e499b8750dfc91b237cbd05cf5db599a87026159b184c6203db45dc75eb66bb`  
		Last Modified: Tue, 29 Mar 2022 10:57:06 GMT  
		Size: 69.7 MB (69682299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de962e95784405a0f75367ec0018478a65eaa53dbe5bea766522b821b11b2a1`  
		Last Modified: Tue, 29 Mar 2022 10:56:57 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:c9a72dfc12386e44fe7ad975e59c65fce45b1ca024f294bd3dea98b9ceddd669
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99791537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5635176bfe6ab76c08819b6c0528e3c1f98e34c4a34f05e3ffafd24c2147c8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 22:19:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 23:09:47 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 23:09:58 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 23:09:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 23:10:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 23:10:09 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 23:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786b85caa695ccd79074b312f23c2333db1849944a4e50cda8ad9dd2ba189ad7`  
		Last Modified: Tue, 29 Mar 2022 23:12:01 GMT  
		Size: 64.5 MB (64508327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968281ed86a2d66a88dbe9ec822f03eb5dc9d0b37a263350ef4cf0f8209669e5`  
		Last Modified: Tue, 29 Mar 2022 23:11:48 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:ee08f190e640af4d06538bf23bc4cfda592dd4a305c6adb2574e5bb6793c4e5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81008314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f3a5d230390dc835e503032a86bde545f39af63dcf157886611dffad68098f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 08:28:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 18 Mar 2022 08:28:18 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 08:28:18 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:28:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 08:28:18 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 08:28:18 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623f0467e8e8ad977aaa28e04253345975ff412058057cd87e8de8f04cb5c6fb`  
		Last Modified: Fri, 18 Mar 2022 08:29:27 GMT  
		Size: 51.4 MB (51351818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba2c417db4714e31117c693c333279a64fc83741ae7d42ba77dad208b0e333`  
		Last Modified: Fri, 18 Mar 2022 08:29:20 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.10`

```console
$ docker pull varnish@sha256:5a44aecc0e5464962ac12b89350e9e55310b9c771d0e4f6350f9fbfa419f3a61
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
$ docker pull varnish@sha256:45e8f5cb61f1575d50e71c4d87a3a16bee72bd8b0b721fd61931f6d3f772c624
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100589455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f2e90cfe6d081c7685e12181346aa9bc4761abc6b0005e37f13393f31c35d2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:50:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:56:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 11:56:16 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:56:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:56:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:56:16 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:56:16 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c0a85ce8de15827814d50bef44ecd40727b52f8b539af301efc2e1130d0d62`  
		Last Modified: Tue, 29 Mar 2022 11:58:23 GMT  
		Size: 69.2 MB (69210298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6189ac10d80aa022f66906092de569cf06a0a0a01f4f4680652bc7e0a1554b`  
		Last Modified: Tue, 29 Mar 2022 11:58:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; arm variant v7

```console
$ docker pull varnish@sha256:b6fb3fc16c82830efd88746b43fa1b8a337d759d0a706990c87609aa147e69dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77223459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a859bd351464452fdc554c75da983c30e3d62d33c01903dc2286c9c3c92474`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 00:49:05 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 01:09:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 01:09:19 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 01:09:19 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 19 Mar 2022 01:09:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 01:09:20 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 01:09:20 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2592eb74fa05949f18521eb0a3761a218f0ae6bbbf24414c24eb7aea00d8de`  
		Last Modified: Sat, 19 Mar 2022 01:14:10 GMT  
		Size: 50.6 MB (50647657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4252e8835c37e9eea96433c384a9cb37e5869a4b571c70cf97c734b65f4c19c`  
		Last Modified: Sat, 19 Mar 2022 01:13:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:d8de22cf7a21c15e114dd7e88382f20123b151ee152e56abe2bf4e6480aee8dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94710809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef56843c3c39b90f3ac6f000f594f52daf7f49bee705523c956ad57acc9e9a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:18:14 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:18:14 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:18:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:18:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:18:17 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:18:18 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3880751953be62fe965411a15ecbdf2e85f4efebef71a6e079897558c2753d29`  
		Last Modified: Thu, 17 Mar 2022 21:20:51 GMT  
		Size: 64.6 MB (64647095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdde89bc6b1d6118585a9c5cac45a4fc987141fbc08f3c4078644c51448b4da`  
		Last Modified: Thu, 17 Mar 2022 21:20:42 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; 386

```console
$ docker pull varnish@sha256:7a50b1ef0665d99ed29fad64e5cd3e251438a9cf8c3ce3ac6aae89b9531339fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102072518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6206c4b5e6f4b904b6c17c78084c5617713d6de7ad56a29367a38e9fead204`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:51:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:54:43 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 10:54:44 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:54:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:54:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:54:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e499b8750dfc91b237cbd05cf5db599a87026159b184c6203db45dc75eb66bb`  
		Last Modified: Tue, 29 Mar 2022 10:57:06 GMT  
		Size: 69.7 MB (69682299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de962e95784405a0f75367ec0018478a65eaa53dbe5bea766522b821b11b2a1`  
		Last Modified: Tue, 29 Mar 2022 10:56:57 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; ppc64le

```console
$ docker pull varnish@sha256:c9a72dfc12386e44fe7ad975e59c65fce45b1ca024f294bd3dea98b9ceddd669
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99791537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5635176bfe6ab76c08819b6c0528e3c1f98e34c4a34f05e3ffafd24c2147c8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 22:19:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 23:09:47 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 23:09:58 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 23:09:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 23:10:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 23:10:09 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 23:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786b85caa695ccd79074b312f23c2333db1849944a4e50cda8ad9dd2ba189ad7`  
		Last Modified: Tue, 29 Mar 2022 23:12:01 GMT  
		Size: 64.5 MB (64508327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968281ed86a2d66a88dbe9ec822f03eb5dc9d0b37a263350ef4cf0f8209669e5`  
		Last Modified: Tue, 29 Mar 2022 23:11:48 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.10` - linux; s390x

```console
$ docker pull varnish@sha256:ee08f190e640af4d06538bf23bc4cfda592dd4a305c6adb2574e5bb6793c4e5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81008314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f3a5d230390dc835e503032a86bde545f39af63dcf157886611dffad68098f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 08:28:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 18 Mar 2022 08:28:18 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 08:28:18 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:28:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 08:28:18 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 08:28:18 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623f0467e8e8ad977aaa28e04253345975ff412058057cd87e8de8f04cb5c6fb`  
		Last Modified: Fri, 18 Mar 2022 08:29:27 GMT  
		Size: 51.4 MB (51351818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba2c417db4714e31117c693c333279a64fc83741ae7d42ba77dad208b0e333`  
		Last Modified: Fri, 18 Mar 2022 08:29:20 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0`

```console
$ docker pull varnish@sha256:b801c56aa8f1b9c05f0e9598854bc4f1c3e923da7f99db243ce332513b69bacb
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
$ docker pull varnish@sha256:29f2924218aff44e9bb35bdae0388298570660b96f8382c443bd43df4d50babd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101201162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5756310d79a680c43eabc487b183a8675937a68bbd58988c9132513e5039e1c2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:50:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:53:01 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 11:53:01 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:53:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:53:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:53:02 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:53:02 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2379b701bfe804e1a17c8e05d1772fc3448d414dde0f50b92ecffc071b7f83ca`  
		Last Modified: Tue, 29 Mar 2022 11:57:43 GMT  
		Size: 69.8 MB (69822232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd9a6d8e5c3764a8cd503830ab99ccd368c6e61dc580115294d5c8c64d991ac`  
		Last Modified: Tue, 29 Mar 2022 11:57:33 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:01265267daaf73dab805ea8e1d072df88e10d3455c1ef4249c83205c24ee81a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77819244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdadebccc4562ee085f25130fc3d8f0b2d86bcd80077fc6a395a1838eb64899a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 00:49:05 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 00:54:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 00:54:37 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 00:54:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:54:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 00:54:38 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 00:54:39 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b8b4c3f734b93e106b4e61a4205afa0e7a6cc65627b991a1f8e77ba59476ea`  
		Last Modified: Sat, 19 Mar 2022 01:11:23 GMT  
		Size: 51.2 MB (51243674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c16e04df37e213bea4ac70bdccd1c234832e551303fb17d85ebd92615ea77`  
		Last Modified: Sat, 19 Mar 2022 01:10:56 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e11fd6713302ff79a09ee261447a1b4dacb1bea7abe1474d4ea52db7195bef08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95310334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a45f7cc20feef392809f19172a9efdd84a47970d141b6c4d8df0b92fc18a660`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:11:32 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:11:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:11:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:11:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:11:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:11:36 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e76646a3e8cb25a95fe35c3856b56ba670f72edbb2b72b58358cbabe594df27`  
		Last Modified: Thu, 17 Mar 2022 21:19:16 GMT  
		Size: 65.2 MB (65246848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef35eaaad2aec815c48e399ad9ce09b86dc12c358b1323a790d792b76d46348d`  
		Last Modified: Thu, 17 Mar 2022 21:19:07 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; 386

```console
$ docker pull varnish@sha256:ff967bfe96be390ea0879e7b29c7361fedd73e8efbf7a72068cbf9131702cadb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102582223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e0cf70fdebb39628c93827754f6976edcefc3b96655a12232a60251d21db4d8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Wed, 23 Mar 2022 23:18:09 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Mar 2022 23:20:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 23 Mar 2022 23:20:36 GMT
WORKDIR /etc/varnish
# Wed, 23 Mar 2022 23:20:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:20:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Mar 2022 23:20:39 GMT
EXPOSE 80 8443
# Wed, 23 Mar 2022 23:20:40 GMT
CMD []
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d725267fd493890980426e1889729e4a81507bb44362a05004b737d5093c2f9`  
		Last Modified: Wed, 23 Mar 2022 23:23:59 GMT  
		Size: 70.2 MB (70195277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017b6e9a9688efab6bde6047ff595f6fb4024aa5da1f1346f680daa65e999ac3`  
		Last Modified: Wed, 23 Mar 2022 23:23:48 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:92d2040e4b9d47fe2252fe27b4f8c7da5edc357bb67d2bac24e9043bec423491
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100374298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e9c1c26fd2df6b1fa055f912bab34c689b2bc85b9c19da91f8a0b9ecfaf1ef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 22:19:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 22:43:24 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 22:43:33 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 22:43:35 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 22:43:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 22:43:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 22:43:50 GMT
CMD []
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aad0307617b134f64961166b820dfb49de1befa320e3628be5280402348c165`  
		Last Modified: Tue, 29 Mar 2022 23:11:06 GMT  
		Size: 65.1 MB (65091318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e75f3605329c6a6bf283072f61229d3f690224cefd6af5d0ccf89e94b67f57`  
		Last Modified: Tue, 29 Mar 2022 23:10:53 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0` - linux; s390x

```console
$ docker pull varnish@sha256:22773d049bf21435113c9a05a109f98891770cc999b3cc708c689513641a7916
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81637564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577ec19b979bd83046063b8688c1605747e7ebb48d7cf040a59560ef296bf450`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:53:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 16:53:20 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:53:20 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:53:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:53:20 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:53:20 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349128ad87266fd7a0da0dab529a20ac021e77bbdd1a8f3d1fdc03be7aa865e`  
		Last Modified: Thu, 17 Mar 2022 16:58:31 GMT  
		Size: 52.0 MB (51981297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412bd8c88e89608521cfaaf3faa15cad9559032ba83110da4705f045799c2b31`  
		Last Modified: Thu, 17 Mar 2022 16:58:24 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0-alpine`

```console
$ docker pull varnish@sha256:807767a5b98ffdf86d917d2943d3f72deda934dcd143c8f9568a45902565f0e6
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
$ docker pull varnish@sha256:2191c54ac764f739bcb5bd535b2ffe2f77a03ea348f9e449a86e6065f568fed1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58347381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2edb8aefb52c80603cbe6caf16f63744965bda637649626fdc5f87613fe1c94`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:53:08 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:54:00 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 11:54:01 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:54:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:54:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:54:01 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:54:01 GMT
CMD []
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd96baffa4d918ae967a3cb824a9926be27d21ea8033092e88fad6096aab3d90`  
		Last Modified: Tue, 29 Mar 2022 11:58:02 GMT  
		Size: 55.5 MB (55528548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317bd7494de5bf540323dab96bc821f1a8d95b6b6b28d01c19c4014bfb39f449`  
		Last Modified: Tue, 29 Mar 2022 11:57:55 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:5e14ecdb3227237be858388b4135d0608f0c7b08fea25257cc3aff3137a6568a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44161132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599b9e6aade9fb82d8d51fee910162af94f3c747be52960c07590c1f4250dd8c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:54:53 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 00:56:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Sat, 19 Mar 2022 00:56:17 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 00:56:17 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:56:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 00:56:18 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 00:56:19 GMT
CMD []
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c45f754ce055922f022022dc3695a530f1a7d8919841b481f2743bcd892d9e6`  
		Last Modified: Sat, 19 Mar 2022 01:12:03 GMT  
		Size: 41.7 MB (41730196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331d2314ee0bdbd9d4bb35ff5598df03c005783d3922834165d7e966ac73cd49`  
		Last Modified: Sat, 19 Mar 2022 01:11:42 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:58cbdde15d49de4a3b402b2fe820ec4d216edefe6e969c990159adde9bbc8c8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51098682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4989798a731407027a62e9a41f0855279d2354494c1c11252b56c7d8a599ab85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:46 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:12:32 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:12:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:12:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:12:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:12:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:12:36 GMT
CMD []
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add42a09981f9b64e2b6df10282b0ad8f29f4af959845ba7eb7c95600d99e3b`  
		Last Modified: Thu, 17 Mar 2022 21:19:41 GMT  
		Size: 48.4 MB (48382315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f14629a9a8f57f9d018ae785cecd4382a7917633bae00050f0d52e71add30b0`  
		Last Modified: Thu, 17 Mar 2022 21:19:33 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:60414c685abcd8930745f1876a54d346b8ce87b6d4b198a2cd4ac99a1172512f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58550665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994c9849309c56c6010ea9a61153a151d3daee8c10b1311d7dbb8752407072ac`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:40 GMT
ADD file:b779b35f4afe33387545e54afc23f09a30d43ad4817cc92ed6b083099748b3cb in / 
# Tue, 29 Mar 2022 00:38:40 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:51:47 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:52:28 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 10:52:28 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:52:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:52:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:52:31 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:52:32 GMT
CMD []
```

-	Layers:
	-	`sha256:ff47816780f28cb5e3d0a86624e638d039b84373892ba3065b1ff9cd4b55b356`  
		Last Modified: Tue, 29 Mar 2022 00:39:52 GMT  
		Size: 2.8 MB (2821065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00db54e99f7c597efeb1960197b93fbf9b6e18130de32926447dd90979888dfe`  
		Last Modified: Tue, 29 Mar 2022 10:56:44 GMT  
		Size: 55.7 MB (55729122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d79ddd44ede3a000dcd5117c0118771368669585b482b103c75519034880842`  
		Last Modified: Tue, 29 Mar 2022 10:56:33 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:732f0a894a4ec364fe68a58021113b1a60f5fdc54e598748ef4bb35c3ac19a71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48200142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1313822e437c4d86cd4d5310307d265e54fd1eef22d74165b39f34ccb2acd5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:44:07 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 22:45:25 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 22:45:33 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 22:45:36 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 22:45:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 22:45:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 22:45:49 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727eb893ac3399b8b7c06699f6dfaf1e437dee968c90920347b9d41361b5ac8`  
		Last Modified: Tue, 29 Mar 2022 23:11:32 GMT  
		Size: 45.4 MB (45385479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6452f699c0644325040cd86e66a403e4a83bca3fbc3359c7b68161392bf2eeb`  
		Last Modified: Tue, 29 Mar 2022 23:11:24 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cf985c0990043bb7f465d16433157fc9f35863a879852c879282f8f6ceadbf6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d4a9025ada0347e039ceca57eb932d70d2304e39a673106238f7cad93785e8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 14:35:54 GMT
ADD file:cd4f7409c75ce2e40b46bbdeca277e2c4500aab51e1a7b6fa518c60e371f0a33 in / 
# Thu, 17 Mar 2022 14:35:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:53:33 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:54:14 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 16:54:16 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:54:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:54:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:54:16 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:54:16 GMT
CMD []
```

-	Layers:
	-	`sha256:1a9a9eea18bd912112f7ed42a3730393bafbb84387ab6790fe9358d09100f3a3`  
		Last Modified: Thu, 17 Mar 2022 14:36:47 GMT  
		Size: 2.6 MB (2605208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a6ee1055eb033458160e7c62fca15b2fe52be379774cfcc33d172ff3a80b2e`  
		Last Modified: Thu, 17 Mar 2022 16:58:46 GMT  
		Size: 44.1 MB (44067113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aad1c673cb296803b470b8e954f42c06628221d764b809d7de327c780ccbab`  
		Last Modified: Thu, 17 Mar 2022 16:58:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0.2`

```console
$ docker pull varnish@sha256:b801c56aa8f1b9c05f0e9598854bc4f1c3e923da7f99db243ce332513b69bacb
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
$ docker pull varnish@sha256:29f2924218aff44e9bb35bdae0388298570660b96f8382c443bd43df4d50babd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101201162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5756310d79a680c43eabc487b183a8675937a68bbd58988c9132513e5039e1c2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:50:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:53:01 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 11:53:01 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:53:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:53:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:53:02 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:53:02 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2379b701bfe804e1a17c8e05d1772fc3448d414dde0f50b92ecffc071b7f83ca`  
		Last Modified: Tue, 29 Mar 2022 11:57:43 GMT  
		Size: 69.8 MB (69822232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd9a6d8e5c3764a8cd503830ab99ccd368c6e61dc580115294d5c8c64d991ac`  
		Last Modified: Tue, 29 Mar 2022 11:57:33 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; arm variant v7

```console
$ docker pull varnish@sha256:01265267daaf73dab805ea8e1d072df88e10d3455c1ef4249c83205c24ee81a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77819244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdadebccc4562ee085f25130fc3d8f0b2d86bcd80077fc6a395a1838eb64899a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 00:49:05 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 00:54:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 00:54:37 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 00:54:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:54:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 00:54:38 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 00:54:39 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b8b4c3f734b93e106b4e61a4205afa0e7a6cc65627b991a1f8e77ba59476ea`  
		Last Modified: Sat, 19 Mar 2022 01:11:23 GMT  
		Size: 51.2 MB (51243674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c16e04df37e213bea4ac70bdccd1c234832e551303fb17d85ebd92615ea77`  
		Last Modified: Sat, 19 Mar 2022 01:10:56 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e11fd6713302ff79a09ee261447a1b4dacb1bea7abe1474d4ea52db7195bef08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95310334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a45f7cc20feef392809f19172a9efdd84a47970d141b6c4d8df0b92fc18a660`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:11:32 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:11:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:11:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:11:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:11:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:11:36 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e76646a3e8cb25a95fe35c3856b56ba670f72edbb2b72b58358cbabe594df27`  
		Last Modified: Thu, 17 Mar 2022 21:19:16 GMT  
		Size: 65.2 MB (65246848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef35eaaad2aec815c48e399ad9ce09b86dc12c358b1323a790d792b76d46348d`  
		Last Modified: Thu, 17 Mar 2022 21:19:07 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; 386

```console
$ docker pull varnish@sha256:ff967bfe96be390ea0879e7b29c7361fedd73e8efbf7a72068cbf9131702cadb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102582223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e0cf70fdebb39628c93827754f6976edcefc3b96655a12232a60251d21db4d8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Wed, 23 Mar 2022 23:18:09 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Mar 2022 23:20:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 23 Mar 2022 23:20:36 GMT
WORKDIR /etc/varnish
# Wed, 23 Mar 2022 23:20:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:20:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Mar 2022 23:20:39 GMT
EXPOSE 80 8443
# Wed, 23 Mar 2022 23:20:40 GMT
CMD []
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d725267fd493890980426e1889729e4a81507bb44362a05004b737d5093c2f9`  
		Last Modified: Wed, 23 Mar 2022 23:23:59 GMT  
		Size: 70.2 MB (70195277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017b6e9a9688efab6bde6047ff595f6fb4024aa5da1f1346f680daa65e999ac3`  
		Last Modified: Wed, 23 Mar 2022 23:23:48 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; ppc64le

```console
$ docker pull varnish@sha256:92d2040e4b9d47fe2252fe27b4f8c7da5edc357bb67d2bac24e9043bec423491
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100374298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e9c1c26fd2df6b1fa055f912bab34c689b2bc85b9c19da91f8a0b9ecfaf1ef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 22:19:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 22:43:24 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 22:43:33 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 22:43:35 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 22:43:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 22:43:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 22:43:50 GMT
CMD []
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aad0307617b134f64961166b820dfb49de1befa320e3628be5280402348c165`  
		Last Modified: Tue, 29 Mar 2022 23:11:06 GMT  
		Size: 65.1 MB (65091318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e75f3605329c6a6bf283072f61229d3f690224cefd6af5d0ccf89e94b67f57`  
		Last Modified: Tue, 29 Mar 2022 23:10:53 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2` - linux; s390x

```console
$ docker pull varnish@sha256:22773d049bf21435113c9a05a109f98891770cc999b3cc708c689513641a7916
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81637564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577ec19b979bd83046063b8688c1605747e7ebb48d7cf040a59560ef296bf450`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:53:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 16:53:20 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:53:20 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:53:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:53:20 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:53:20 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349128ad87266fd7a0da0dab529a20ac021e77bbdd1a8f3d1fdc03be7aa865e`  
		Last Modified: Thu, 17 Mar 2022 16:58:31 GMT  
		Size: 52.0 MB (51981297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412bd8c88e89608521cfaaf3faa15cad9559032ba83110da4705f045799c2b31`  
		Last Modified: Thu, 17 Mar 2022 16:58:24 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.0.2-alpine`

```console
$ docker pull varnish@sha256:807767a5b98ffdf86d917d2943d3f72deda934dcd143c8f9568a45902565f0e6
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
$ docker pull varnish@sha256:2191c54ac764f739bcb5bd535b2ffe2f77a03ea348f9e449a86e6065f568fed1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58347381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2edb8aefb52c80603cbe6caf16f63744965bda637649626fdc5f87613fe1c94`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:53:08 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:54:00 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 11:54:01 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:54:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:54:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:54:01 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:54:01 GMT
CMD []
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd96baffa4d918ae967a3cb824a9926be27d21ea8033092e88fad6096aab3d90`  
		Last Modified: Tue, 29 Mar 2022 11:58:02 GMT  
		Size: 55.5 MB (55528548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317bd7494de5bf540323dab96bc821f1a8d95b6b6b28d01c19c4014bfb39f449`  
		Last Modified: Tue, 29 Mar 2022 11:57:55 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:5e14ecdb3227237be858388b4135d0608f0c7b08fea25257cc3aff3137a6568a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44161132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599b9e6aade9fb82d8d51fee910162af94f3c747be52960c07590c1f4250dd8c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:54:53 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 00:56:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Sat, 19 Mar 2022 00:56:17 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 00:56:17 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:56:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 00:56:18 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 00:56:19 GMT
CMD []
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c45f754ce055922f022022dc3695a530f1a7d8919841b481f2743bcd892d9e6`  
		Last Modified: Sat, 19 Mar 2022 01:12:03 GMT  
		Size: 41.7 MB (41730196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331d2314ee0bdbd9d4bb35ff5598df03c005783d3922834165d7e966ac73cd49`  
		Last Modified: Sat, 19 Mar 2022 01:11:42 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:58cbdde15d49de4a3b402b2fe820ec4d216edefe6e969c990159adde9bbc8c8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51098682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4989798a731407027a62e9a41f0855279d2354494c1c11252b56c7d8a599ab85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:46 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:12:32 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:12:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:12:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:12:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:12:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:12:36 GMT
CMD []
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add42a09981f9b64e2b6df10282b0ad8f29f4af959845ba7eb7c95600d99e3b`  
		Last Modified: Thu, 17 Mar 2022 21:19:41 GMT  
		Size: 48.4 MB (48382315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f14629a9a8f57f9d018ae785cecd4382a7917633bae00050f0d52e71add30b0`  
		Last Modified: Thu, 17 Mar 2022 21:19:33 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; 386

```console
$ docker pull varnish@sha256:60414c685abcd8930745f1876a54d346b8ce87b6d4b198a2cd4ac99a1172512f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58550665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994c9849309c56c6010ea9a61153a151d3daee8c10b1311d7dbb8752407072ac`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:40 GMT
ADD file:b779b35f4afe33387545e54afc23f09a30d43ad4817cc92ed6b083099748b3cb in / 
# Tue, 29 Mar 2022 00:38:40 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:51:47 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:52:28 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 10:52:28 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:52:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:52:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:52:31 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:52:32 GMT
CMD []
```

-	Layers:
	-	`sha256:ff47816780f28cb5e3d0a86624e638d039b84373892ba3065b1ff9cd4b55b356`  
		Last Modified: Tue, 29 Mar 2022 00:39:52 GMT  
		Size: 2.8 MB (2821065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00db54e99f7c597efeb1960197b93fbf9b6e18130de32926447dd90979888dfe`  
		Last Modified: Tue, 29 Mar 2022 10:56:44 GMT  
		Size: 55.7 MB (55729122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d79ddd44ede3a000dcd5117c0118771368669585b482b103c75519034880842`  
		Last Modified: Tue, 29 Mar 2022 10:56:33 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:732f0a894a4ec364fe68a58021113b1a60f5fdc54e598748ef4bb35c3ac19a71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48200142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1313822e437c4d86cd4d5310307d265e54fd1eef22d74165b39f34ccb2acd5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:44:07 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 22:45:25 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 22:45:33 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 22:45:36 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 22:45:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 22:45:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 22:45:49 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727eb893ac3399b8b7c06699f6dfaf1e437dee968c90920347b9d41361b5ac8`  
		Last Modified: Tue, 29 Mar 2022 23:11:32 GMT  
		Size: 45.4 MB (45385479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6452f699c0644325040cd86e66a403e4a83bca3fbc3359c7b68161392bf2eeb`  
		Last Modified: Tue, 29 Mar 2022 23:11:24 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.0.2-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cf985c0990043bb7f465d16433157fc9f35863a879852c879282f8f6ceadbf6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d4a9025ada0347e039ceca57eb932d70d2304e39a673106238f7cad93785e8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 14:35:54 GMT
ADD file:cd4f7409c75ce2e40b46bbdeca277e2c4500aab51e1a7b6fa518c60e371f0a33 in / 
# Thu, 17 Mar 2022 14:35:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:53:33 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:54:14 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 16:54:16 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:54:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:54:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:54:16 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:54:16 GMT
CMD []
```

-	Layers:
	-	`sha256:1a9a9eea18bd912112f7ed42a3730393bafbb84387ab6790fe9358d09100f3a3`  
		Last Modified: Thu, 17 Mar 2022 14:36:47 GMT  
		Size: 2.6 MB (2605208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a6ee1055eb033458160e7c62fca15b2fe52be379774cfcc33d172ff3a80b2e`  
		Last Modified: Thu, 17 Mar 2022 16:58:46 GMT  
		Size: 44.1 MB (44067113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aad1c673cb296803b470b8e954f42c06628221d764b809d7de327c780ccbab`  
		Last Modified: Thu, 17 Mar 2022 16:58:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1`

```console
$ docker pull varnish@sha256:b64b20bfc23c9079a9bcfdcd8ff35e3f1adad84c12ff803975fa593ea9650e72
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
$ docker pull varnish@sha256:98827c7071e80c9a913460e8bd111beb98a38a5686bed5b27ab75abfd5aff9b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105361658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36290e2df272a3fbea54f584b09e13883f48b3505efaa338daf7ecb459b5f47`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:45:29 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:45:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:45:30 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:48:39 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:48:40 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:48:40 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:48:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:48:40 GMT
USER varnish
# Tue, 29 Mar 2022 11:48:40 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:48:40 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85807fba3e9d469810e3036e28e405a87c12416d33733f1f7f7e94c439eb5d77`  
		Last Modified: Tue, 29 Mar 2022 11:56:57 GMT  
		Size: 74.0 MB (73982727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1ff6d1463583ef69a89d1fda387049246c085e61747414ae9c0f1cfc1500b0`  
		Last Modified: Tue, 29 Mar 2022 11:56:48 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af263778cd417e6838329163c0fdea48ae1c41a9f1b36e1a110fccb6a170740e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81965256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4175d88652526ca864b538bb97343be3405b7bc01af633976da847bdc538a7d4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Mon, 21 Mar 2022 21:58:04 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Mon, 21 Mar 2022 21:58:04 GMT
ARG VARNISH_VERSION=7.1.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Mon, 21 Mar 2022 21:58:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 21 Mar 2022 22:04:47 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Mon, 21 Mar 2022 22:04:48 GMT
WORKDIR /etc/varnish
# Mon, 21 Mar 2022 22:04:49 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 21 Mar 2022 22:04:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 21 Mar 2022 22:04:49 GMT
USER varnish
# Mon, 21 Mar 2022 22:04:50 GMT
EXPOSE 80 8443
# Mon, 21 Mar 2022 22:04:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9704905dc71a74a9217b303959eab3275876295fa10d0cafe5bc65ad810cd74`  
		Last Modified: Mon, 21 Mar 2022 22:10:09 GMT  
		Size: 55.4 MB (55389687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721e0eda39f07d8ea4988139f1ba8cac6ce25be060371b306da413ce290b9e3c`  
		Last Modified: Mon, 21 Mar 2022 22:09:39 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:51aff26cb39a2f14fce2e947c23faa09d25dd0a913916db912b7a499e26fa2ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95302102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e131f007cc132b8f6dd08e780522dd2e60731dbe2e0f823ed11e14f40cac89b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 04:32:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Nov 2021 18:45:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";     chown varnish /var/lib/varnish
# Tue, 23 Nov 2021 18:45:49 GMT
WORKDIR /etc/varnish
# Tue, 23 Nov 2021 18:45:50 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 23 Nov 2021 18:45:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 23 Nov 2021 18:45:51 GMT
USER varnish
# Tue, 23 Nov 2021 18:45:52 GMT
EXPOSE 80 8443
# Tue, 23 Nov 2021 18:45:53 GMT
CMD []
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578fcb2ffb3a65568d2158fff866790a57bef5ff9fe4d0adbc8638903200d063`  
		Last Modified: Tue, 23 Nov 2021 18:53:53 GMT  
		Size: 65.2 MB (65245109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2e44ba19c44d8707ddcfa7453b71f4bbf425fd6598d105594e436984544e0d`  
		Last Modified: Tue, 23 Nov 2021 18:53:43 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; 386

```console
$ docker pull varnish@sha256:0047e76b398be942bf25f1d411c80ebcedbadd61923712176629e7c34820a785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106724618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab3736937a96e1a43f3f1aeb4be45e7ff8de82be5c2f989f560f03a5184285e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:46:05 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:46:06 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:46:07 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:46:08 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:46:09 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:46:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:46:11 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:46:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:46:13 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:49:13 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:49:13 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:49:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:49:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:49:16 GMT
USER varnish
# Tue, 29 Mar 2022 10:49:17 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:49:18 GMT
CMD []
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63eaa854035d66fac0390795c2397fe04d07b7430b12fa078504551b318df85`  
		Last Modified: Tue, 29 Mar 2022 10:55:52 GMT  
		Size: 74.3 MB (74334626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a6fe49077958e9a4953cc4d3af1568e29ac356c695803b640474dfe02b9bc9`  
		Last Modified: Tue, 29 Mar 2022 10:55:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:62015f62c67f63ec23add010e41f2ac9dfd880362c44a690dd974ce17e5e3751
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100359492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4cb11f686ef357f33a8e37968cc67ae542dffe603cf9aff29394368a198052c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 03:28:22 GMT
ADD file:5ed330f0fe1328f694fcaefb961cf4da4d8a4ff03100b21af718b69316168706 in / 
# Wed, 17 Nov 2021 03:28:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 06:04:25 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Nov 2021 19:23:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";     chown varnish /var/lib/varnish
# Tue, 23 Nov 2021 19:23:53 GMT
WORKDIR /etc/varnish
# Tue, 23 Nov 2021 19:23:56 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 23 Nov 2021 19:23:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 23 Nov 2021 19:24:01 GMT
USER varnish
# Tue, 23 Nov 2021 19:24:05 GMT
EXPOSE 80 8443
# Tue, 23 Nov 2021 19:24:08 GMT
CMD []
```

-	Layers:
	-	`sha256:258ff2a13858db8f51b65662e02137c0abcfd2528ca73e92b7a40061d938fb1e`  
		Last Modified: Wed, 17 Nov 2021 03:54:34 GMT  
		Size: 35.3 MB (35271382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d18b72ed51762923dec234a3e6d8a5cab5a3021ae2c28a3554deb133f6e21a`  
		Last Modified: Tue, 23 Nov 2021 20:12:14 GMT  
		Size: 65.1 MB (65087635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af30865388f39d784806088616002d8919fb85e113af44fb1e91c8c5c916821`  
		Last Modified: Tue, 23 Nov 2021 20:12:01 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1` - linux; s390x

```console
$ docker pull varnish@sha256:a3c56f087d0388cf65564d909213dce9beb41bb76957ef33e200e114cfdec496
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81633627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f030b8a4929d9f6b3c7ddec396a27c9882ba5fd55bffb52d02838837b50f773e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:09:56 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Nov 2021 18:47:33 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f http://varnish-cache.org/_downloads/varnish-7.0.1.tgz -o $tmpdir/orig.tgz;     echo "7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.1|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";     chown varnish /var/lib/varnish
# Tue, 23 Nov 2021 18:47:35 GMT
WORKDIR /etc/varnish
# Tue, 23 Nov 2021 18:47:35 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 23 Nov 2021 18:47:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 23 Nov 2021 18:47:35 GMT
USER varnish
# Tue, 23 Nov 2021 18:47:35 GMT
EXPOSE 80 8443
# Tue, 23 Nov 2021 18:47:35 GMT
CMD []
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1856848ea6559ab3eee68b844d86e89b75e816219e79719ab420902c863da945`  
		Last Modified: Tue, 23 Nov 2021 18:54:08 GMT  
		Size: 52.0 MB (51982194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebb5c6d1e9db1bb11962fac5aa107d6b0984baa8dfa3186eea6afedfa98c1fd`  
		Last Modified: Tue, 23 Nov 2021 18:54:01 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1-alpine`

```console
$ docker pull varnish@sha256:4349c705264ad51d6f78de0235ac46b29ec3b531977f59ce0bbff2256e02d6d8
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
$ docker pull varnish@sha256:76322eef28985ba43144e7681a691b10d0fb6d65ca6276ee2aa9fe1503728fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61971006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba2cd2d3038a9106bcb02208154cc5baf5e4244fe147edaf5e87e1ecbe6d71b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:48:52 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:48:53 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:50:29 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:50:30 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:50:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:50:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:50:30 GMT
USER varnish
# Tue, 29 Mar 2022 11:50:30 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:50:30 GMT
CMD []
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ecdbed9207316489cc108f638bbbd586717bf5c312bec86eb2806b5c430ef4`  
		Last Modified: Tue, 29 Mar 2022 11:57:20 GMT  
		Size: 59.2 MB (59156014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b2e8a1615c6c3fe377f7e38a02e6fe7336e7935f3f62e8feff8036e1fef010`  
		Last Modified: Tue, 29 Mar 2022 11:57:11 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e74f4644f1ad25dff087e9814b16d6b8d1c50480b3ceed76a131cf1a943f4b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47681740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62e6c4f384214fbe8421578e1eeee7fdb69ef38584a60873192f4c5d6e421e42`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 04:00:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 24 Mar 2022 04:00:49 GMT
ARG VARNISH_VERSION=7.1.0
# Thu, 24 Mar 2022 04:00:50 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Thu, 24 Mar 2022 04:00:50 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Thu, 24 Mar 2022 04:00:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Thu, 24 Mar 2022 04:00:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 24 Mar 2022 04:03:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 24 Mar 2022 04:03:17 GMT
WORKDIR /etc/varnish
# Thu, 24 Mar 2022 04:03:18 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 24 Mar 2022 04:03:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 24 Mar 2022 04:03:18 GMT
USER varnish
# Thu, 24 Mar 2022 04:03:19 GMT
EXPOSE 80 8443
# Thu, 24 Mar 2022 04:03:19 GMT
CMD []
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b368ff8888cb027e695191ca990ad4381869724318cb4eb7f85079bd5f6e8e`  
		Last Modified: Thu, 24 Mar 2022 04:05:49 GMT  
		Size: 45.3 MB (45254199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97355aaad54f82580feb2e175bb0c769223365500c94f3bf41b427fee5787064`  
		Last Modified: Thu, 24 Mar 2022 04:05:25 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:b3ec9620791fcf441a8f754a3ae153982688a0c358ecbcb541905e2c24d760a2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51095518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26159e0db97873e3a5a8a98aaf7c1cf40c468e6a79b58b9f374c740e400c0b6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 18:02:27 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Nov 2021 18:46:59 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;     chown varnish /var/lib/varnish
# Tue, 23 Nov 2021 18:46:59 GMT
WORKDIR /etc/varnish
# Tue, 23 Nov 2021 18:47:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 23 Nov 2021 18:47:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 23 Nov 2021 18:47:02 GMT
USER varnish
# Tue, 23 Nov 2021 18:47:03 GMT
EXPOSE 80 8443
# Tue, 23 Nov 2021 18:47:04 GMT
CMD []
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1818711e82171f58532be9e36ece4bea66ada8827cf9c5ebd8f1b7ea37e7c7c8`  
		Last Modified: Tue, 23 Nov 2021 18:54:17 GMT  
		Size: 48.4 MB (48377338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e61a4444a0bd5c82c31470ed5b05658aae067d486a26c47ba35ea28ccaa50d9`  
		Last Modified: Tue, 23 Nov 2021 18:54:09 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:054271711d30e2fb58f5d698686fd03242c26c5d1639767847da7ef1862bb698
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62092708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64750edf69039dd7d6f29e880d8fdee78660fe2a78dd9a31bbb6bcd3729e27ab`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:49:32 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:49:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:49:34 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:49:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:49:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:49:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:49:38 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:49:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:49:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:50:58 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:50:58 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:51:00 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:51:01 GMT
USER varnish
# Tue, 29 Mar 2022 10:51:02 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:51:03 GMT
CMD []
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24260c4dad9894e6f1ccdd399dca6e51ef7b734f5326e01d44f42ffd1d30e006`  
		Last Modified: Tue, 29 Mar 2022 10:56:16 GMT  
		Size: 59.3 MB (59273305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69df1ecab60edd6421987701bb3b854822ce60c2224dcf6f9c59906cd1a6f4e`  
		Last Modified: Tue, 29 Mar 2022 10:56:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:82158bd40b9d5e4bc2c78be680082978f6c8d9561bc66d91b61704784025b8f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48217443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d83fcb273a473c14857b2126edaaa4803dd101a1eef640d4404359a744c5dd7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:52:07 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Nov 2021 19:25:37 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;     chown varnish /var/lib/varnish
# Tue, 23 Nov 2021 19:25:40 GMT
WORKDIR /etc/varnish
# Tue, 23 Nov 2021 19:25:43 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 23 Nov 2021 19:25:46 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 23 Nov 2021 19:25:48 GMT
USER varnish
# Tue, 23 Nov 2021 19:25:52 GMT
EXPOSE 80 8443
# Tue, 23 Nov 2021 19:25:54 GMT
CMD []
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e264a0d3f91805f5cc7410cb1d330a98486598c9a7fe23b65d6c779465ec3f0`  
		Last Modified: Tue, 23 Nov 2021 20:12:39 GMT  
		Size: 45.4 MB (45399496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a36b52ccb7fa4f0804b44fffb700d4487814ba5baa1e90c3de9127f0701185`  
		Last Modified: Tue, 23 Nov 2021 20:12:30 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:7332cb5e538e4ce7b2cbea1f5df22d4cfb5f25ae86c3a372ce2cfdad56358fe1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46684103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d336021b72dc6a8230d1ced495f049cc1cd444e4388e7f4c8f030f4a5c082d1a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 22:10:22 GMT
ENV VARNISH_SIZE=100M
# Tue, 23 Nov 2021 18:48:19 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"7541d50b03a113f0a13660d459cc4c2eb45d57fb19380ab56a5413a4e5d702f9c0856585f09aeea6084a239ad8c69017af3805a864540b4697e0eac29f00b408  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;     chown varnish /var/lib/varnish
# Tue, 23 Nov 2021 18:48:20 GMT
WORKDIR /etc/varnish
# Tue, 23 Nov 2021 18:48:20 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 23 Nov 2021 18:48:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 23 Nov 2021 18:48:20 GMT
USER varnish
# Tue, 23 Nov 2021 18:48:21 GMT
EXPOSE 80 8443
# Tue, 23 Nov 2021 18:48:21 GMT
CMD []
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150943b9444243ba5bcc08c008ddc0e099f980cc43f0e4221324bb47e961ea34`  
		Last Modified: Tue, 23 Nov 2021 18:54:25 GMT  
		Size: 44.1 MB (44074346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303a433a4cc94594e14447d74042ee6129d8c5864b4d25d42d1e98ff0372f845`  
		Last Modified: Tue, 23 Nov 2021 18:54:19 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.0`

```console
$ docker pull varnish@sha256:a31e7033540b21b998faf49e2faef6227d73fd56a0be14e3efa122d6f9c707c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `varnish:7.1.0` - linux; amd64

```console
$ docker pull varnish@sha256:98827c7071e80c9a913460e8bd111beb98a38a5686bed5b27ab75abfd5aff9b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105361658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36290e2df272a3fbea54f584b09e13883f48b3505efaa338daf7ecb459b5f47`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:45:29 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:45:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:45:30 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:48:39 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:48:40 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:48:40 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:48:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:48:40 GMT
USER varnish
# Tue, 29 Mar 2022 11:48:40 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:48:40 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85807fba3e9d469810e3036e28e405a87c12416d33733f1f7f7e94c439eb5d77`  
		Last Modified: Tue, 29 Mar 2022 11:56:57 GMT  
		Size: 74.0 MB (73982727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1ff6d1463583ef69a89d1fda387049246c085e61747414ae9c0f1cfc1500b0`  
		Last Modified: Tue, 29 Mar 2022 11:56:48 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af263778cd417e6838329163c0fdea48ae1c41a9f1b36e1a110fccb6a170740e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81965256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4175d88652526ca864b538bb97343be3405b7bc01af633976da847bdc538a7d4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Mon, 21 Mar 2022 21:58:04 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Mon, 21 Mar 2022 21:58:04 GMT
ARG VARNISH_VERSION=7.1.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Mon, 21 Mar 2022 21:58:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 21 Mar 2022 22:04:47 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Mon, 21 Mar 2022 22:04:48 GMT
WORKDIR /etc/varnish
# Mon, 21 Mar 2022 22:04:49 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 21 Mar 2022 22:04:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 21 Mar 2022 22:04:49 GMT
USER varnish
# Mon, 21 Mar 2022 22:04:50 GMT
EXPOSE 80 8443
# Mon, 21 Mar 2022 22:04:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9704905dc71a74a9217b303959eab3275876295fa10d0cafe5bc65ad810cd74`  
		Last Modified: Mon, 21 Mar 2022 22:10:09 GMT  
		Size: 55.4 MB (55389687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721e0eda39f07d8ea4988139f1ba8cac6ce25be060371b306da413ce290b9e3c`  
		Last Modified: Mon, 21 Mar 2022 22:09:39 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0` - linux; 386

```console
$ docker pull varnish@sha256:0047e76b398be942bf25f1d411c80ebcedbadd61923712176629e7c34820a785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106724618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab3736937a96e1a43f3f1aeb4be45e7ff8de82be5c2f989f560f03a5184285e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:46:05 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:46:06 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:46:07 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:46:08 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:46:09 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:46:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:46:11 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:46:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:46:13 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:49:13 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:49:13 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:49:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:49:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:49:16 GMT
USER varnish
# Tue, 29 Mar 2022 10:49:17 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:49:18 GMT
CMD []
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63eaa854035d66fac0390795c2397fe04d07b7430b12fa078504551b318df85`  
		Last Modified: Tue, 29 Mar 2022 10:55:52 GMT  
		Size: 74.3 MB (74334626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a6fe49077958e9a4953cc4d3af1568e29ac356c695803b640474dfe02b9bc9`  
		Last Modified: Tue, 29 Mar 2022 10:55:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.1.0-alpine`

```console
$ docker pull varnish@sha256:70b5d71f81b751c836654308f5f49fb487020345ccd5b20cd0874443e37354ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; 386

### `varnish:7.1.0-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:76322eef28985ba43144e7681a691b10d0fb6d65ca6276ee2aa9fe1503728fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61971006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba2cd2d3038a9106bcb02208154cc5baf5e4244fe147edaf5e87e1ecbe6d71b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:48:52 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:48:53 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:50:29 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:50:30 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:50:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:50:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:50:30 GMT
USER varnish
# Tue, 29 Mar 2022 11:50:30 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:50:30 GMT
CMD []
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ecdbed9207316489cc108f638bbbd586717bf5c312bec86eb2806b5c430ef4`  
		Last Modified: Tue, 29 Mar 2022 11:57:20 GMT  
		Size: 59.2 MB (59156014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b2e8a1615c6c3fe377f7e38a02e6fe7336e7935f3f62e8feff8036e1fef010`  
		Last Modified: Tue, 29 Mar 2022 11:57:11 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e74f4644f1ad25dff087e9814b16d6b8d1c50480b3ceed76a131cf1a943f4b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47681740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62e6c4f384214fbe8421578e1eeee7fdb69ef38584a60873192f4c5d6e421e42`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 04:00:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 24 Mar 2022 04:00:49 GMT
ARG VARNISH_VERSION=7.1.0
# Thu, 24 Mar 2022 04:00:50 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Thu, 24 Mar 2022 04:00:50 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Thu, 24 Mar 2022 04:00:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Thu, 24 Mar 2022 04:00:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 24 Mar 2022 04:03:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 24 Mar 2022 04:03:17 GMT
WORKDIR /etc/varnish
# Thu, 24 Mar 2022 04:03:18 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 24 Mar 2022 04:03:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 24 Mar 2022 04:03:18 GMT
USER varnish
# Thu, 24 Mar 2022 04:03:19 GMT
EXPOSE 80 8443
# Thu, 24 Mar 2022 04:03:19 GMT
CMD []
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b368ff8888cb027e695191ca990ad4381869724318cb4eb7f85079bd5f6e8e`  
		Last Modified: Thu, 24 Mar 2022 04:05:49 GMT  
		Size: 45.3 MB (45254199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97355aaad54f82580feb2e175bb0c769223365500c94f3bf41b427fee5787064`  
		Last Modified: Thu, 24 Mar 2022 04:05:25 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.1.0-alpine` - linux; 386

```console
$ docker pull varnish@sha256:054271711d30e2fb58f5d698686fd03242c26c5d1639767847da7ef1862bb698
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62092708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64750edf69039dd7d6f29e880d8fdee78660fe2a78dd9a31bbb6bcd3729e27ab`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:49:32 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:49:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:49:34 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:49:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:49:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:49:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:49:38 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:49:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:49:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:50:58 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:50:58 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:51:00 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:51:01 GMT
USER varnish
# Tue, 29 Mar 2022 10:51:02 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:51:03 GMT
CMD []
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24260c4dad9894e6f1ccdd399dca6e51ef7b734f5326e01d44f42ffd1d30e006`  
		Last Modified: Tue, 29 Mar 2022 10:56:16 GMT  
		Size: 59.3 MB (59273305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69df1ecab60edd6421987701bb3b854822ce60c2224dcf6f9c59906cd1a6f4e`  
		Last Modified: Tue, 29 Mar 2022 10:56:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:5dfb00bccf2f3f18107e46bcdde74ee38ec8309e700ccc532395dc5fa00d0be8
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
$ docker pull varnish@sha256:76322eef28985ba43144e7681a691b10d0fb6d65ca6276ee2aa9fe1503728fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61971006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba2cd2d3038a9106bcb02208154cc5baf5e4244fe147edaf5e87e1ecbe6d71b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:48:52 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:48:53 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:50:29 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:50:30 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:50:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:50:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:50:30 GMT
USER varnish
# Tue, 29 Mar 2022 11:50:30 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:50:30 GMT
CMD []
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ecdbed9207316489cc108f638bbbd586717bf5c312bec86eb2806b5c430ef4`  
		Last Modified: Tue, 29 Mar 2022 11:57:20 GMT  
		Size: 59.2 MB (59156014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b2e8a1615c6c3fe377f7e38a02e6fe7336e7935f3f62e8feff8036e1fef010`  
		Last Modified: Tue, 29 Mar 2022 11:57:11 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e74f4644f1ad25dff087e9814b16d6b8d1c50480b3ceed76a131cf1a943f4b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47681740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62e6c4f384214fbe8421578e1eeee7fdb69ef38584a60873192f4c5d6e421e42`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 04:00:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 24 Mar 2022 04:00:49 GMT
ARG VARNISH_VERSION=7.1.0
# Thu, 24 Mar 2022 04:00:50 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Thu, 24 Mar 2022 04:00:50 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Thu, 24 Mar 2022 04:00:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Thu, 24 Mar 2022 04:00:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 24 Mar 2022 04:03:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 24 Mar 2022 04:03:17 GMT
WORKDIR /etc/varnish
# Thu, 24 Mar 2022 04:03:18 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 24 Mar 2022 04:03:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 24 Mar 2022 04:03:18 GMT
USER varnish
# Thu, 24 Mar 2022 04:03:19 GMT
EXPOSE 80 8443
# Thu, 24 Mar 2022 04:03:19 GMT
CMD []
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b368ff8888cb027e695191ca990ad4381869724318cb4eb7f85079bd5f6e8e`  
		Last Modified: Thu, 24 Mar 2022 04:05:49 GMT  
		Size: 45.3 MB (45254199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97355aaad54f82580feb2e175bb0c769223365500c94f3bf41b427fee5787064`  
		Last Modified: Thu, 24 Mar 2022 04:05:25 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:58cbdde15d49de4a3b402b2fe820ec4d216edefe6e969c990159adde9bbc8c8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51098682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4989798a731407027a62e9a41f0855279d2354494c1c11252b56c7d8a599ab85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:46 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:12:32 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:12:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:12:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:12:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:12:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:12:36 GMT
CMD []
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add42a09981f9b64e2b6df10282b0ad8f29f4af959845ba7eb7c95600d99e3b`  
		Last Modified: Thu, 17 Mar 2022 21:19:41 GMT  
		Size: 48.4 MB (48382315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f14629a9a8f57f9d018ae785cecd4382a7917633bae00050f0d52e71add30b0`  
		Last Modified: Thu, 17 Mar 2022 21:19:33 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:054271711d30e2fb58f5d698686fd03242c26c5d1639767847da7ef1862bb698
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62092708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64750edf69039dd7d6f29e880d8fdee78660fe2a78dd9a31bbb6bcd3729e27ab`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:49:32 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:49:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:49:34 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:49:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:49:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:49:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:49:38 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:49:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:49:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:50:58 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:50:58 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:51:00 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:51:01 GMT
USER varnish
# Tue, 29 Mar 2022 10:51:02 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:51:03 GMT
CMD []
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24260c4dad9894e6f1ccdd399dca6e51ef7b734f5326e01d44f42ffd1d30e006`  
		Last Modified: Tue, 29 Mar 2022 10:56:16 GMT  
		Size: 59.3 MB (59273305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69df1ecab60edd6421987701bb3b854822ce60c2224dcf6f9c59906cd1a6f4e`  
		Last Modified: Tue, 29 Mar 2022 10:56:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:2b5a806ea2ade1ea0d76aa0ad7d8ef7c61ae2955e2e9549d7d1972a84eb9e668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48202141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c13f3efcc65dfb1b3ac5697e031c0fefd156f6649062d5289cd9690594762`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:18:43 GMT
ADD file:bf9c99d8209e0bed9fd3b62cbe691ebf3829d5a35e63e2b066f1f842577a6d24 in / 
# Thu, 17 Mar 2022 18:18:48 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 12:09:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 12:10:26 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Fri, 18 Mar 2022 12:10:30 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 12:10:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:10:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 12:10:36 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 12:10:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8b7e8363a93630a772b70e3cf72231f43c62addae0ee8e507c61d43e3781c4e7`  
		Last Modified: Thu, 17 Mar 2022 18:20:01 GMT  
		Size: 2.8 MB (2817281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e94cc2aebd9efa44a159f8edfec552af073cbcaf430e29039e344a7af24312`  
		Last Modified: Fri, 18 Mar 2022 12:16:51 GMT  
		Size: 45.4 MB (45384380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26079fd90524de774229d65b85187547d85ba3f7e836d042a8b615469573bcac`  
		Last Modified: Fri, 18 Mar 2022 12:16:43 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cf985c0990043bb7f465d16433157fc9f35863a879852c879282f8f6ceadbf6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d4a9025ada0347e039ceca57eb932d70d2304e39a673106238f7cad93785e8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 14:35:54 GMT
ADD file:cd4f7409c75ce2e40b46bbdeca277e2c4500aab51e1a7b6fa518c60e371f0a33 in / 
# Thu, 17 Mar 2022 14:35:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:53:33 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:54:14 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 16:54:16 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:54:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:54:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:54:16 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:54:16 GMT
CMD []
```

-	Layers:
	-	`sha256:1a9a9eea18bd912112f7ed42a3730393bafbb84387ab6790fe9358d09100f3a3`  
		Last Modified: Thu, 17 Mar 2022 14:36:47 GMT  
		Size: 2.6 MB (2605208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a6ee1055eb033458160e7c62fca15b2fe52be379774cfcc33d172ff3a80b2e`  
		Last Modified: Thu, 17 Mar 2022 16:58:46 GMT  
		Size: 44.1 MB (44067113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aad1c673cb296803b470b8e954f42c06628221d764b809d7de327c780ccbab`  
		Last Modified: Thu, 17 Mar 2022 16:58:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:5355195c2be0c5db054e2fb04ce69280d507b6c442730b663b3a7c601f9bc7e5
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
$ docker pull varnish@sha256:98827c7071e80c9a913460e8bd111beb98a38a5686bed5b27ab75abfd5aff9b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105361658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36290e2df272a3fbea54f584b09e13883f48b3505efaa338daf7ecb459b5f47`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:45:29 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:45:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:45:30 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:48:39 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:48:40 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:48:40 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:48:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:48:40 GMT
USER varnish
# Tue, 29 Mar 2022 11:48:40 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:48:40 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85807fba3e9d469810e3036e28e405a87c12416d33733f1f7f7e94c439eb5d77`  
		Last Modified: Tue, 29 Mar 2022 11:56:57 GMT  
		Size: 74.0 MB (73982727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1ff6d1463583ef69a89d1fda387049246c085e61747414ae9c0f1cfc1500b0`  
		Last Modified: Tue, 29 Mar 2022 11:56:48 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af263778cd417e6838329163c0fdea48ae1c41a9f1b36e1a110fccb6a170740e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81965256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4175d88652526ca864b538bb97343be3405b7bc01af633976da847bdc538a7d4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Mon, 21 Mar 2022 21:58:04 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Mon, 21 Mar 2022 21:58:04 GMT
ARG VARNISH_VERSION=7.1.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Mon, 21 Mar 2022 21:58:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 21 Mar 2022 22:04:47 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Mon, 21 Mar 2022 22:04:48 GMT
WORKDIR /etc/varnish
# Mon, 21 Mar 2022 22:04:49 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 21 Mar 2022 22:04:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 21 Mar 2022 22:04:49 GMT
USER varnish
# Mon, 21 Mar 2022 22:04:50 GMT
EXPOSE 80 8443
# Mon, 21 Mar 2022 22:04:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9704905dc71a74a9217b303959eab3275876295fa10d0cafe5bc65ad810cd74`  
		Last Modified: Mon, 21 Mar 2022 22:10:09 GMT  
		Size: 55.4 MB (55389687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721e0eda39f07d8ea4988139f1ba8cac6ce25be060371b306da413ce290b9e3c`  
		Last Modified: Mon, 21 Mar 2022 22:09:39 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e11fd6713302ff79a09ee261447a1b4dacb1bea7abe1474d4ea52db7195bef08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95310334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a45f7cc20feef392809f19172a9efdd84a47970d141b6c4d8df0b92fc18a660`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:11:32 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:11:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:11:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:11:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:11:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:11:36 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e76646a3e8cb25a95fe35c3856b56ba670f72edbb2b72b58358cbabe594df27`  
		Last Modified: Thu, 17 Mar 2022 21:19:16 GMT  
		Size: 65.2 MB (65246848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef35eaaad2aec815c48e399ad9ce09b86dc12c358b1323a790d792b76d46348d`  
		Last Modified: Thu, 17 Mar 2022 21:19:07 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:0047e76b398be942bf25f1d411c80ebcedbadd61923712176629e7c34820a785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106724618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab3736937a96e1a43f3f1aeb4be45e7ff8de82be5c2f989f560f03a5184285e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:46:05 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:46:06 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:46:07 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:46:08 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:46:09 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:46:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:46:11 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:46:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:46:13 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:49:13 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:49:13 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:49:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:49:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:49:16 GMT
USER varnish
# Tue, 29 Mar 2022 10:49:17 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:49:18 GMT
CMD []
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63eaa854035d66fac0390795c2397fe04d07b7430b12fa078504551b318df85`  
		Last Modified: Tue, 29 Mar 2022 10:55:52 GMT  
		Size: 74.3 MB (74334626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a6fe49077958e9a4953cc4d3af1568e29ac356c695803b640474dfe02b9bc9`  
		Last Modified: Tue, 29 Mar 2022 10:55:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:a0c48bf2f162c843ebb10fc977411a3d8e258f6b89de39e491d47718993cf786
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100370202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:725f4afa7625567f4159d88e2e6dcc062bc668f1cd5c553034e2a6967a4d9e77`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 11:39:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 12:08:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 18 Mar 2022 12:08:52 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 12:08:54 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:08:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 12:09:00 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 12:09:02 GMT
CMD []
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1fa8ae10f00d34c8087576b32b9865d74c25fb40cd32770e9aeda3432e9dd0`  
		Last Modified: Fri, 18 Mar 2022 12:16:20 GMT  
		Size: 65.1 MB (65089969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9700e7649d7cf13acc90336a4b0b948f9723a8be37895e9ac6956b6badc4a330`  
		Last Modified: Fri, 18 Mar 2022 12:16:08 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:22773d049bf21435113c9a05a109f98891770cc999b3cc708c689513641a7916
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81637564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577ec19b979bd83046063b8688c1605747e7ebb48d7cf040a59560ef296bf450`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:53:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 16:53:20 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:53:20 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:53:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:53:20 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:53:20 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349128ad87266fd7a0da0dab529a20ac021e77bbdd1a8f3d1fdc03be7aa865e`  
		Last Modified: Thu, 17 Mar 2022 16:58:31 GMT  
		Size: 52.0 MB (51981297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412bd8c88e89608521cfaaf3faa15cad9559032ba83110da4705f045799c2b31`  
		Last Modified: Thu, 17 Mar 2022 16:58:24 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:5dfb00bccf2f3f18107e46bcdde74ee38ec8309e700ccc532395dc5fa00d0be8
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
$ docker pull varnish@sha256:76322eef28985ba43144e7681a691b10d0fb6d65ca6276ee2aa9fe1503728fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61971006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba2cd2d3038a9106bcb02208154cc5baf5e4244fe147edaf5e87e1ecbe6d71b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:48:52 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:48:53 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:50:29 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:50:30 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:50:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:50:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:50:30 GMT
USER varnish
# Tue, 29 Mar 2022 11:50:30 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:50:30 GMT
CMD []
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ecdbed9207316489cc108f638bbbd586717bf5c312bec86eb2806b5c430ef4`  
		Last Modified: Tue, 29 Mar 2022 11:57:20 GMT  
		Size: 59.2 MB (59156014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b2e8a1615c6c3fe377f7e38a02e6fe7336e7935f3f62e8feff8036e1fef010`  
		Last Modified: Tue, 29 Mar 2022 11:57:11 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:e74f4644f1ad25dff087e9814b16d6b8d1c50480b3ceed76a131cf1a943f4b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47681740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62e6c4f384214fbe8421578e1eeee7fdb69ef38584a60873192f4c5d6e421e42`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 04:00:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 24 Mar 2022 04:00:49 GMT
ARG VARNISH_VERSION=7.1.0
# Thu, 24 Mar 2022 04:00:50 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Thu, 24 Mar 2022 04:00:50 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 24 Mar 2022 04:00:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Thu, 24 Mar 2022 04:00:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Thu, 24 Mar 2022 04:00:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 24 Mar 2022 04:03:16 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 24 Mar 2022 04:03:17 GMT
WORKDIR /etc/varnish
# Thu, 24 Mar 2022 04:03:18 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 24 Mar 2022 04:03:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 24 Mar 2022 04:03:18 GMT
USER varnish
# Thu, 24 Mar 2022 04:03:19 GMT
EXPOSE 80 8443
# Thu, 24 Mar 2022 04:03:19 GMT
CMD []
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b368ff8888cb027e695191ca990ad4381869724318cb4eb7f85079bd5f6e8e`  
		Last Modified: Thu, 24 Mar 2022 04:05:49 GMT  
		Size: 45.3 MB (45254199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97355aaad54f82580feb2e175bb0c769223365500c94f3bf41b427fee5787064`  
		Last Modified: Thu, 24 Mar 2022 04:05:25 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:58cbdde15d49de4a3b402b2fe820ec4d216edefe6e969c990159adde9bbc8c8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51098682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4989798a731407027a62e9a41f0855279d2354494c1c11252b56c7d8a599ab85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:46 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:12:32 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:12:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:12:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:12:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:12:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:12:36 GMT
CMD []
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add42a09981f9b64e2b6df10282b0ad8f29f4af959845ba7eb7c95600d99e3b`  
		Last Modified: Thu, 17 Mar 2022 21:19:41 GMT  
		Size: 48.4 MB (48382315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f14629a9a8f57f9d018ae785cecd4382a7917633bae00050f0d52e71add30b0`  
		Last Modified: Thu, 17 Mar 2022 21:19:33 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:054271711d30e2fb58f5d698686fd03242c26c5d1639767847da7ef1862bb698
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62092708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64750edf69039dd7d6f29e880d8fdee78660fe2a78dd9a31bbb6bcd3729e27ab`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:49:32 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:49:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:49:34 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:49:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:49:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:49:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:49:38 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:49:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:49:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:50:58 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:50:58 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:51:00 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:51:01 GMT
USER varnish
# Tue, 29 Mar 2022 10:51:02 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:51:03 GMT
CMD []
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24260c4dad9894e6f1ccdd399dca6e51ef7b734f5326e01d44f42ffd1d30e006`  
		Last Modified: Tue, 29 Mar 2022 10:56:16 GMT  
		Size: 59.3 MB (59273305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69df1ecab60edd6421987701bb3b854822ce60c2224dcf6f9c59906cd1a6f4e`  
		Last Modified: Tue, 29 Mar 2022 10:56:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:2b5a806ea2ade1ea0d76aa0ad7d8ef7c61ae2955e2e9549d7d1972a84eb9e668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48202141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c13f3efcc65dfb1b3ac5697e031c0fefd156f6649062d5289cd9690594762`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:18:43 GMT
ADD file:bf9c99d8209e0bed9fd3b62cbe691ebf3829d5a35e63e2b066f1f842577a6d24 in / 
# Thu, 17 Mar 2022 18:18:48 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 12:09:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 12:10:26 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Fri, 18 Mar 2022 12:10:30 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 12:10:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:10:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 12:10:36 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 12:10:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8b7e8363a93630a772b70e3cf72231f43c62addae0ee8e507c61d43e3781c4e7`  
		Last Modified: Thu, 17 Mar 2022 18:20:01 GMT  
		Size: 2.8 MB (2817281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e94cc2aebd9efa44a159f8edfec552af073cbcaf430e29039e344a7af24312`  
		Last Modified: Fri, 18 Mar 2022 12:16:51 GMT  
		Size: 45.4 MB (45384380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26079fd90524de774229d65b85187547d85ba3f7e836d042a8b615469573bcac`  
		Last Modified: Fri, 18 Mar 2022 12:16:43 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cf985c0990043bb7f465d16433157fc9f35863a879852c879282f8f6ceadbf6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d4a9025ada0347e039ceca57eb932d70d2304e39a673106238f7cad93785e8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 14:35:54 GMT
ADD file:cd4f7409c75ce2e40b46bbdeca277e2c4500aab51e1a7b6fa518c60e371f0a33 in / 
# Thu, 17 Mar 2022 14:35:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:53:33 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:54:14 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 16:54:16 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:54:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:54:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:54:16 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:54:16 GMT
CMD []
```

-	Layers:
	-	`sha256:1a9a9eea18bd912112f7ed42a3730393bafbb84387ab6790fe9358d09100f3a3`  
		Last Modified: Thu, 17 Mar 2022 14:36:47 GMT  
		Size: 2.6 MB (2605208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a6ee1055eb033458160e7c62fca15b2fe52be379774cfcc33d172ff3a80b2e`  
		Last Modified: Thu, 17 Mar 2022 16:58:46 GMT  
		Size: 44.1 MB (44067113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aad1c673cb296803b470b8e954f42c06628221d764b809d7de327c780ccbab`  
		Last Modified: Thu, 17 Mar 2022 16:58:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:5355195c2be0c5db054e2fb04ce69280d507b6c442730b663b3a7c601f9bc7e5
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
$ docker pull varnish@sha256:98827c7071e80c9a913460e8bd111beb98a38a5686bed5b27ab75abfd5aff9b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105361658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36290e2df272a3fbea54f584b09e13883f48b3505efaa338daf7ecb459b5f47`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:45:29 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:45:29 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:45:29 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:45:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:45:30 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:48:39 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:48:40 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:48:40 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:48:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:48:40 GMT
USER varnish
# Tue, 29 Mar 2022 11:48:40 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:48:40 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85807fba3e9d469810e3036e28e405a87c12416d33733f1f7f7e94c439eb5d77`  
		Last Modified: Tue, 29 Mar 2022 11:56:57 GMT  
		Size: 74.0 MB (73982727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1ff6d1463583ef69a89d1fda387049246c085e61747414ae9c0f1cfc1500b0`  
		Last Modified: Tue, 29 Mar 2022 11:56:48 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af263778cd417e6838329163c0fdea48ae1c41a9f1b36e1a110fccb6a170740e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81965256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4175d88652526ca864b538bb97343be3405b7bc01af633976da847bdc538a7d4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Mon, 21 Mar 2022 21:58:04 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Mon, 21 Mar 2022 21:58:04 GMT
ARG VARNISH_VERSION=7.1.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Mon, 21 Mar 2022 21:58:05 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Mon, 21 Mar 2022 21:58:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Mon, 21 Mar 2022 21:58:07 GMT
ENV VARNISH_SIZE=100M
# Mon, 21 Mar 2022 22:04:47 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Mon, 21 Mar 2022 22:04:48 GMT
WORKDIR /etc/varnish
# Mon, 21 Mar 2022 22:04:49 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Mon, 21 Mar 2022 22:04:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 21 Mar 2022 22:04:49 GMT
USER varnish
# Mon, 21 Mar 2022 22:04:50 GMT
EXPOSE 80 8443
# Mon, 21 Mar 2022 22:04:50 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9704905dc71a74a9217b303959eab3275876295fa10d0cafe5bc65ad810cd74`  
		Last Modified: Mon, 21 Mar 2022 22:10:09 GMT  
		Size: 55.4 MB (55389687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721e0eda39f07d8ea4988139f1ba8cac6ce25be060371b306da413ce290b9e3c`  
		Last Modified: Mon, 21 Mar 2022 22:09:39 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e11fd6713302ff79a09ee261447a1b4dacb1bea7abe1474d4ea52db7195bef08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95310334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a45f7cc20feef392809f19172a9efdd84a47970d141b6c4d8df0b92fc18a660`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:11:32 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:11:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:11:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:11:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:11:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:11:36 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e76646a3e8cb25a95fe35c3856b56ba670f72edbb2b72b58358cbabe594df27`  
		Last Modified: Thu, 17 Mar 2022 21:19:16 GMT  
		Size: 65.2 MB (65246848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef35eaaad2aec815c48e399ad9ce09b86dc12c358b1323a790d792b76d46348d`  
		Last Modified: Thu, 17 Mar 2022 21:19:07 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:0047e76b398be942bf25f1d411c80ebcedbadd61923712176629e7c34820a785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106724618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab3736937a96e1a43f3f1aeb4be45e7ff8de82be5c2f989f560f03a5184285e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:46:05 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:46:06 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:46:07 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:46:08 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:46:09 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:46:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:46:11 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:46:12 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:46:13 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:49:13 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.0.tgz -o $tmpdir/orig.tgz;     echo "ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         mkdir /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 10:49:13 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:49:15 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:49:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:49:16 GMT
USER varnish
# Tue, 29 Mar 2022 10:49:17 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:49:18 GMT
CMD []
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63eaa854035d66fac0390795c2397fe04d07b7430b12fa078504551b318df85`  
		Last Modified: Tue, 29 Mar 2022 10:55:52 GMT  
		Size: 74.3 MB (74334626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a6fe49077958e9a4953cc4d3af1568e29ac356c695803b640474dfe02b9bc9`  
		Last Modified: Tue, 29 Mar 2022 10:55:37 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:a0c48bf2f162c843ebb10fc977411a3d8e258f6b89de39e491d47718993cf786
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100370202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:725f4afa7625567f4159d88e2e6dcc062bc668f1cd5c553034e2a6967a4d9e77`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 11:39:46 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 12:08:45 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 18 Mar 2022 12:08:52 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 12:08:54 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:08:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 12:09:00 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 12:09:02 GMT
CMD []
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1fa8ae10f00d34c8087576b32b9865d74c25fb40cd32770e9aeda3432e9dd0`  
		Last Modified: Fri, 18 Mar 2022 12:16:20 GMT  
		Size: 65.1 MB (65089969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9700e7649d7cf13acc90336a4b0b948f9723a8be37895e9ac6956b6badc4a330`  
		Last Modified: Fri, 18 Mar 2022 12:16:08 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:22773d049bf21435113c9a05a109f98891770cc999b3cc708c689513641a7916
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81637564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577ec19b979bd83046063b8688c1605747e7ebb48d7cf040a59560ef296bf450`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:53:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 16:53:20 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:53:20 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:53:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:53:20 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:53:20 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349128ad87266fd7a0da0dab529a20ac021e77bbdd1a8f3d1fdc03be7aa865e`  
		Last Modified: Thu, 17 Mar 2022 16:58:31 GMT  
		Size: 52.0 MB (51981297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412bd8c88e89608521cfaaf3faa15cad9559032ba83110da4705f045799c2b31`  
		Last Modified: Thu, 17 Mar 2022 16:58:24 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:b801c56aa8f1b9c05f0e9598854bc4f1c3e923da7f99db243ce332513b69bacb
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
$ docker pull varnish@sha256:29f2924218aff44e9bb35bdae0388298570660b96f8382c443bd43df4d50babd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101201162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5756310d79a680c43eabc487b183a8675937a68bbd58988c9132513e5039e1c2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:50:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:53:01 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 11:53:01 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:53:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:53:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:53:02 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:53:02 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2379b701bfe804e1a17c8e05d1772fc3448d414dde0f50b92ecffc071b7f83ca`  
		Last Modified: Tue, 29 Mar 2022 11:57:43 GMT  
		Size: 69.8 MB (69822232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd9a6d8e5c3764a8cd503830ab99ccd368c6e61dc580115294d5c8c64d991ac`  
		Last Modified: Tue, 29 Mar 2022 11:57:33 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:01265267daaf73dab805ea8e1d072df88e10d3455c1ef4249c83205c24ee81a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.8 MB (77819244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdadebccc4562ee085f25130fc3d8f0b2d86bcd80077fc6a395a1838eb64899a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 00:49:05 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 00:54:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 00:54:37 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 00:54:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:54:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 00:54:38 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 00:54:39 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b8b4c3f734b93e106b4e61a4205afa0e7a6cc65627b991a1f8e77ba59476ea`  
		Last Modified: Sat, 19 Mar 2022 01:11:23 GMT  
		Size: 51.2 MB (51243674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c16e04df37e213bea4ac70bdccd1c234832e551303fb17d85ebd92615ea77`  
		Last Modified: Sat, 19 Mar 2022 01:10:56 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:e11fd6713302ff79a09ee261447a1b4dacb1bea7abe1474d4ea52db7195bef08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 MB (95310334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a45f7cc20feef392809f19172a9efdd84a47970d141b6c4d8df0b92fc18a660`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:11:32 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:11:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:11:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:11:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:11:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:11:36 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e76646a3e8cb25a95fe35c3856b56ba670f72edbb2b72b58358cbabe594df27`  
		Last Modified: Thu, 17 Mar 2022 21:19:16 GMT  
		Size: 65.2 MB (65246848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef35eaaad2aec815c48e399ad9ce09b86dc12c358b1323a790d792b76d46348d`  
		Last Modified: Thu, 17 Mar 2022 21:19:07 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:ff967bfe96be390ea0879e7b29c7361fedd73e8efbf7a72068cbf9131702cadb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102582223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e0cf70fdebb39628c93827754f6976edcefc3b96655a12232a60251d21db4d8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 08:15:53 GMT
ADD file:2d6be3846f0e5fabd85bc9409b1e2223cad4c57c76f96e9f81489ba78a72a1f5 in / 
# Thu, 17 Mar 2022 08:15:54 GMT
CMD ["bash"]
# Wed, 23 Mar 2022 23:18:09 GMT
ENV VARNISH_SIZE=100M
# Wed, 23 Mar 2022 23:20:36 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 23 Mar 2022 23:20:36 GMT
WORKDIR /etc/varnish
# Wed, 23 Mar 2022 23:20:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:20:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 23 Mar 2022 23:20:39 GMT
EXPOSE 80 8443
# Wed, 23 Mar 2022 23:20:40 GMT
CMD []
```

-	Layers:
	-	`sha256:176085117cac9b2cf2cf57b3a10c9811dbd2773497fbac3086b5024070447e97`  
		Last Modified: Thu, 17 Mar 2022 08:24:00 GMT  
		Size: 32.4 MB (32386475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d725267fd493890980426e1889729e4a81507bb44362a05004b737d5093c2f9`  
		Last Modified: Wed, 23 Mar 2022 23:23:59 GMT  
		Size: 70.2 MB (70195277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017b6e9a9688efab6bde6047ff595f6fb4024aa5da1f1346f680daa65e999ac3`  
		Last Modified: Wed, 23 Mar 2022 23:23:48 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:92d2040e4b9d47fe2252fe27b4f8c7da5edc357bb67d2bac24e9043bec423491
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100374298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e9c1c26fd2df6b1fa055f912bab34c689b2bc85b9c19da91f8a0b9ecfaf1ef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 22:19:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 22:43:24 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 22:43:33 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 22:43:35 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 22:43:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 22:43:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 22:43:50 GMT
CMD []
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aad0307617b134f64961166b820dfb49de1befa320e3628be5280402348c165`  
		Last Modified: Tue, 29 Mar 2022 23:11:06 GMT  
		Size: 65.1 MB (65091318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e75f3605329c6a6bf283072f61229d3f690224cefd6af5d0ccf89e94b67f57`  
		Last Modified: Tue, 29 Mar 2022 23:10:53 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:22773d049bf21435113c9a05a109f98891770cc999b3cc708c689513641a7916
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.6 MB (81637564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577ec19b979bd83046063b8688c1605747e7ebb48d7cf040a59560ef296bf450`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:53:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.0.2.tgz -o $tmpdir/orig.tgz;     echo "5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|7.0.2|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 16:53:20 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:53:20 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:53:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:53:20 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:53:20 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349128ad87266fd7a0da0dab529a20ac021e77bbdd1a8f3d1fdc03be7aa865e`  
		Last Modified: Thu, 17 Mar 2022 16:58:31 GMT  
		Size: 52.0 MB (51981297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412bd8c88e89608521cfaaf3faa15cad9559032ba83110da4705f045799c2b31`  
		Last Modified: Thu, 17 Mar 2022 16:58:24 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:807767a5b98ffdf86d917d2943d3f72deda934dcd143c8f9568a45902565f0e6
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
$ docker pull varnish@sha256:2191c54ac764f739bcb5bd535b2ffe2f77a03ea348f9e449a86e6065f568fed1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58347381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2edb8aefb52c80603cbe6caf16f63744965bda637649626fdc5f87613fe1c94`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:53:08 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:54:00 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 11:54:01 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:54:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:54:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:54:01 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:54:01 GMT
CMD []
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd96baffa4d918ae967a3cb824a9926be27d21ea8033092e88fad6096aab3d90`  
		Last Modified: Tue, 29 Mar 2022 11:58:02 GMT  
		Size: 55.5 MB (55528548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317bd7494de5bf540323dab96bc821f1a8d95b6b6b28d01c19c4014bfb39f449`  
		Last Modified: Tue, 29 Mar 2022 11:57:55 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:5e14ecdb3227237be858388b4135d0608f0c7b08fea25257cc3aff3137a6568a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44161132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599b9e6aade9fb82d8d51fee910162af94f3c747be52960c07590c1f4250dd8c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:54:53 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 00:56:16 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Sat, 19 Mar 2022 00:56:17 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 00:56:17 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:56:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 00:56:18 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 00:56:19 GMT
CMD []
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c45f754ce055922f022022dc3695a530f1a7d8919841b481f2743bcd892d9e6`  
		Last Modified: Sat, 19 Mar 2022 01:12:03 GMT  
		Size: 41.7 MB (41730196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331d2314ee0bdbd9d4bb35ff5598df03c005783d3922834165d7e966ac73cd49`  
		Last Modified: Sat, 19 Mar 2022 01:11:42 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:58cbdde15d49de4a3b402b2fe820ec4d216edefe6e969c990159adde9bbc8c8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51098682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4989798a731407027a62e9a41f0855279d2354494c1c11252b56c7d8a599ab85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:46 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:12:32 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:12:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:12:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:12:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:12:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:12:36 GMT
CMD []
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add42a09981f9b64e2b6df10282b0ad8f29f4af959845ba7eb7c95600d99e3b`  
		Last Modified: Thu, 17 Mar 2022 21:19:41 GMT  
		Size: 48.4 MB (48382315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f14629a9a8f57f9d018ae785cecd4382a7917633bae00050f0d52e71add30b0`  
		Last Modified: Thu, 17 Mar 2022 21:19:33 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:60414c685abcd8930745f1876a54d346b8ce87b6d4b198a2cd4ac99a1172512f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.6 MB (58550665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994c9849309c56c6010ea9a61153a151d3daee8c10b1311d7dbb8752407072ac`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:40 GMT
ADD file:b779b35f4afe33387545e54afc23f09a30d43ad4817cc92ed6b083099748b3cb in / 
# Tue, 29 Mar 2022 00:38:40 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:51:47 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:52:28 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 10:52:28 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:52:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:52:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:52:31 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:52:32 GMT
CMD []
```

-	Layers:
	-	`sha256:ff47816780f28cb5e3d0a86624e638d039b84373892ba3065b1ff9cd4b55b356`  
		Last Modified: Tue, 29 Mar 2022 00:39:52 GMT  
		Size: 2.8 MB (2821065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00db54e99f7c597efeb1960197b93fbf9b6e18130de32926447dd90979888dfe`  
		Last Modified: Tue, 29 Mar 2022 10:56:44 GMT  
		Size: 55.7 MB (55729122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d79ddd44ede3a000dcd5117c0118771368669585b482b103c75519034880842`  
		Last Modified: Tue, 29 Mar 2022 10:56:33 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:732f0a894a4ec364fe68a58021113b1a60f5fdc54e598748ef4bb35c3ac19a71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48200142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c1313822e437c4d86cd4d5310307d265e54fd1eef22d74165b39f34ccb2acd5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:44:07 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 22:45:25 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Tue, 29 Mar 2022 22:45:33 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 22:45:36 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 22:45:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 22:45:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 22:45:49 GMT
CMD []
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0727eb893ac3399b8b7c06699f6dfaf1e437dee968c90920347b9d41361b5ac8`  
		Last Modified: Tue, 29 Mar 2022 23:11:32 GMT  
		Size: 45.4 MB (45385479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6452f699c0644325040cd86e66a403e4a83bca3fbc3359c7b68161392bf2eeb`  
		Last Modified: Tue, 29 Mar 2022 23:11:24 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:cf985c0990043bb7f465d16433157fc9f35863a879852c879282f8f6ceadbf6e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46672799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93d4a9025ada0347e039ceca57eb932d70d2304e39a673106238f7cad93785e8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 14:35:54 GMT
ADD file:cd4f7409c75ce2e40b46bbdeca277e2c4500aab51e1a7b6fa518c60e371f0a33 in / 
# Thu, 17 Mar 2022 14:35:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:53:33 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:54:14 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 16:54:16 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:54:16 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:54:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:54:16 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:54:16 GMT
CMD []
```

-	Layers:
	-	`sha256:1a9a9eea18bd912112f7ed42a3730393bafbb84387ab6790fe9358d09100f3a3`  
		Last Modified: Thu, 17 Mar 2022 14:36:47 GMT  
		Size: 2.6 MB (2605208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a6ee1055eb033458160e7c62fca15b2fe52be379774cfcc33d172ff3a80b2e`  
		Last Modified: Thu, 17 Mar 2022 16:58:46 GMT  
		Size: 44.1 MB (44067113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24aad1c673cb296803b470b8e954f42c06628221d764b809d7de327c780ccbab`  
		Last Modified: Thu, 17 Mar 2022 16:58:41 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:5a44aecc0e5464962ac12b89350e9e55310b9c771d0e4f6350f9fbfa419f3a61
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
$ docker pull varnish@sha256:45e8f5cb61f1575d50e71c4d87a3a16bee72bd8b0b721fd61931f6d3f772c624
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100589455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f2e90cfe6d081c7685e12181346aa9bc4761abc6b0005e37f13393f31c35d2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 11:50:45 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:56:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 11:56:16 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:56:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:56:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:56:16 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:56:16 GMT
CMD []
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c0a85ce8de15827814d50bef44ecd40727b52f8b539af301efc2e1130d0d62`  
		Last Modified: Tue, 29 Mar 2022 11:58:23 GMT  
		Size: 69.2 MB (69210298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6189ac10d80aa022f66906092de569cf06a0a0a01f4f4680652bc7e0a1554b`  
		Last Modified: Tue, 29 Mar 2022 11:58:14 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:b6fb3fc16c82830efd88746b43fa1b8a337d759d0a706990c87609aa147e69dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77223459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a859bd351464452fdc554c75da983c30e3d62d33c01903dc2286c9c3c92474`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 00:49:05 GMT
ENV VARNISH_SIZE=100M
# Sat, 19 Mar 2022 01:09:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 19 Mar 2022 01:09:19 GMT
WORKDIR /etc/varnish
# Sat, 19 Mar 2022 01:09:19 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 19 Mar 2022 01:09:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 19 Mar 2022 01:09:20 GMT
EXPOSE 80 8443
# Sat, 19 Mar 2022 01:09:20 GMT
CMD []
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2592eb74fa05949f18521eb0a3761a218f0ae6bbbf24414c24eb7aea00d8de`  
		Last Modified: Sat, 19 Mar 2022 01:14:10 GMT  
		Size: 50.6 MB (50647657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4252e8835c37e9eea96433c384a9cb37e5869a4b571c70cf97c734b65f4c19c`  
		Last Modified: Sat, 19 Mar 2022 01:13:42 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:d8de22cf7a21c15e114dd7e88382f20123b151ee152e56abe2bf4e6480aee8dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94710809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef56843c3c39b90f3ac6f000f594f52daf7f49bee705523c956ad57acc9e9a6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 21:09:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:18:14 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Thu, 17 Mar 2022 21:18:14 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:18:16 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:18:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:18:17 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:18:18 GMT
CMD []
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3880751953be62fe965411a15ecbdf2e85f4efebef71a6e079897558c2753d29`  
		Last Modified: Thu, 17 Mar 2022 21:20:51 GMT  
		Size: 64.6 MB (64647095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdde89bc6b1d6118585a9c5cac45a4fc987141fbc08f3c4078644c51448b4da`  
		Last Modified: Thu, 17 Mar 2022 21:20:42 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:7a50b1ef0665d99ed29fad64e5cd3e251438a9cf8c3ce3ac6aae89b9531339fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102072518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6206c4b5e6f4b904b6c17c78084c5617713d6de7ad56a29367a38e9fead204`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:51:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 10:54:43 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 10:54:44 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 10:54:45 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:54:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 10:54:46 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 10:54:47 GMT
CMD []
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e499b8750dfc91b237cbd05cf5db599a87026159b184c6203db45dc75eb66bb`  
		Last Modified: Tue, 29 Mar 2022 10:57:06 GMT  
		Size: 69.7 MB (69682299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de962e95784405a0f75367ec0018478a65eaa53dbe5bea766522b821b11b2a1`  
		Last Modified: Tue, 29 Mar 2022 10:56:57 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:c9a72dfc12386e44fe7ad975e59c65fce45b1ca024f294bd3dea98b9ceddd669
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99791537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5635176bfe6ab76c08819b6c0528e3c1f98e34c4a34f05e3ffafd24c2147c8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 22:19:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 23:09:47 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 29 Mar 2022 23:09:58 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 23:09:59 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 29 Mar 2022 23:10:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 23:10:09 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 23:10:13 GMT
CMD []
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786b85caa695ccd79074b312f23c2333db1849944a4e50cda8ad9dd2ba189ad7`  
		Last Modified: Tue, 29 Mar 2022 23:12:01 GMT  
		Size: 64.5 MB (64508327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968281ed86a2d66a88dbe9ec822f03eb5dc9d0b37a263350ef4cf0f8209669e5`  
		Last Modified: Tue, 29 Mar 2022 23:11:48 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:ee08f190e640af4d06538bf23bc4cfda592dd4a305c6adb2574e5bb6793c4e5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81008314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f3a5d230390dc835e503032a86bde545f39af63dcf157886611dffad68098f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 16:51:29 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 08:28:15 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.10.tgz -o $tmpdir/orig.tgz;     echo "b89ac4465aacde2fde963642727d20d7d33d04f89c0764c43d59fe13e70fe729079fef44da28cc0090fa153ec584a0fe9723fd2ce976e8e9021410a5f73eadd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.10|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Fri, 18 Mar 2022 08:28:18 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 08:28:18 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 18 Mar 2022 08:28:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 08:28:18 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 08:28:18 GMT
CMD []
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623f0467e8e8ad977aaa28e04253345975ff412058057cd87e8de8f04cb5c6fb`  
		Last Modified: Fri, 18 Mar 2022 08:29:27 GMT  
		Size: 51.4 MB (51351818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba2c417db4714e31117c693c333279a64fc83741ae7d42ba77dad208b0e333`  
		Last Modified: Fri, 18 Mar 2022 08:29:20 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
