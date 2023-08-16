<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `hitch`

-	[`hitch:1`](#hitch1)
-	[`hitch:1.7`](#hitch17)
-	[`hitch:1.7.2`](#hitch172)
-	[`hitch:1.7.2-1`](#hitch172-1)
-	[`hitch:1.7.3`](#hitch173)
-	[`hitch:1.7.3-1`](#hitch173-1)
-	[`hitch:latest`](#hitchlatest)

## `hitch:1`

```console
$ docker pull hitch@sha256:5dc2200eda652b4445e48262d187006f2fc164d5847319a1a1e222ac9908a23a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hitch:1` - linux; amd64

```console
$ docker pull hitch@sha256:dd86d288fc7247d23bea302eba8d8922f69f69541b99a327f1c2fa8b08301926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33043480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c3c41df73ba661e191a9e420d638961a7c2b6115db4979eab1f8842499f8e7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SRCVER=1.7.3
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGVER=1
# Fri, 28 Jul 2023 03:55:49 GMT
ARG DISTVER=bullseye
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Fri, 28 Jul 2023 03:57:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 28 Jul 2023 03:57:42 GMT
WORKDIR /etc/hitch
# Fri, 28 Jul 2023 03:57:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:57:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Fri, 28 Jul 2023 03:57:43 GMT
EXPOSE 443
# Fri, 28 Jul 2023 03:57:43 GMT
CMD []
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce4d5916070e20a4e55ab081a2f2e40dd3c6506bb53150fb0f6eaf4d255d82`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 1.6 MB (1625461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdc0b4ba0ecebe0776dde4024ee63f953b17cc68a10ebdd312b82a3fd0127fa`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:366b0a87b08677e14a24328b00c1e13d4be89242ddfa84a32696753883641c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28123964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c7aaa1f03bb4efd47023bd435f6c72bec04cb0ae887cb2e8f2d0522ab42ff3`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:34:15 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 07:34:15 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 07:34:16 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 07:34:16 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 07:34:16 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 07:36:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 07:36:29 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 07:36:29 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:36:29 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 07:36:29 GMT
EXPOSE 443
# Wed, 16 Aug 2023 07:36:29 GMT
CMD []
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63299eb73eaf82f2fe926374f1fb4ec255bf190ce110728f6be4575b2e95ffdd`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 1.5 MB (1544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deb4c79b2b9ae842542be5478cade5af3aa28a41be0bf9fc13207661a0d4321`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:689a2683a75f0e3ee97ee7044e42e4fb2dbb7834d6d48f3b896ed4015b7afc73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b36eb7dbf395b0b9dea8496f4fc1312d8819a4102cea678f728db447b9710a`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:10:31 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:10:31 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:10:31 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:10:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:10:32 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:12:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:12:28 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:12:28 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:12:28 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:12:28 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:12:29 GMT
CMD []
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10576dab04f55e719604aeb6ec990863e14fce60cd45ead4d4d2c1bf00b1f8c5`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 1.6 MB (1606793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ee2e032932235bf0fcef63010e523739abc0d743f07813f7f1b15b8633885`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; 386

```console
$ docker pull hitch@sha256:e91c8145e5a7dc5ab7350ecf9b4e16fba1be78cff05897b59b76998ea379bcc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34028517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad5eda2cc0e6bd3957a6becdc500d65f42108755e29712dd7396bb5e138739`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 03:31:26 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 03:34:03 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 03:34:03 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 03:34:03 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:34:03 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 03:34:03 GMT
EXPOSE 443
# Wed, 16 Aug 2023 03:34:03 GMT
CMD []
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08cd8bc2e244a5ca5d75161c4b61834034c4c19641a078d6ca2331987a3a5e`  
		Last Modified: Wed, 16 Aug 2023 03:36:35 GMT  
		Size: 1.6 MB (1630900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451771b9145a8ff1fefbd41b4e243676516ce9736190b765738247abe1d63941`  
		Last Modified: Wed, 16 Aug 2023 03:36:34 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; ppc64le

```console
$ docker pull hitch@sha256:170e62ded87a85f2bfb42acc0e03ab497a04075d00e3397b24105e5744808a9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36979600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13028e41c2ee40d673afa93ae5eaa59f481f41e53ef4089a8543073989e0398`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:33:08 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 04:33:09 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 04:33:10 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 04:33:11 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 04:33:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 04:49:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 04:49:47 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 04:49:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 04:49:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 04:49:48 GMT
EXPOSE 443
# Wed, 16 Aug 2023 04:49:48 GMT
CMD []
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748feeacec9e19e61cf794ad6678c0afa4e219f074fad8b6ec944b793d849669`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 1.7 MB (1688117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e623fea85eb8927b4e51cc68eddc1e0aac4720b7265f235800d3178f1e7f90`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; s390x

```console
$ docker pull hitch@sha256:aae9b16f5a0d350b182f1b49c38419f79e387d6a60991eb25fdaf70dad593ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31275688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96aeac18bbc6090d0b08bcd9bcff4b255931e7267e112e43f8dc4724520cdacb`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:22:21 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:22:21 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:22:22 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:24:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:24:43 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:24:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:24:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:24:43 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:24:43 GMT
CMD []
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a322aa47cfadd0e9cc7a3abd8c7f8fa1f6e3427de7e4c0f50c52acf53581b787`  
		Last Modified: Wed, 16 Aug 2023 01:27:33 GMT  
		Size: 1.6 MB (1622292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f4927bc6be443f72e0510f319233f2bbca6da6728e0cd25d64cb96f1188a09`  
		Last Modified: Wed, 16 Aug 2023 01:27:32 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7`

```console
$ docker pull hitch@sha256:5dc2200eda652b4445e48262d187006f2fc164d5847319a1a1e222ac9908a23a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hitch:1.7` - linux; amd64

```console
$ docker pull hitch@sha256:dd86d288fc7247d23bea302eba8d8922f69f69541b99a327f1c2fa8b08301926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33043480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c3c41df73ba661e191a9e420d638961a7c2b6115db4979eab1f8842499f8e7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SRCVER=1.7.3
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGVER=1
# Fri, 28 Jul 2023 03:55:49 GMT
ARG DISTVER=bullseye
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Fri, 28 Jul 2023 03:57:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 28 Jul 2023 03:57:42 GMT
WORKDIR /etc/hitch
# Fri, 28 Jul 2023 03:57:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:57:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Fri, 28 Jul 2023 03:57:43 GMT
EXPOSE 443
# Fri, 28 Jul 2023 03:57:43 GMT
CMD []
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce4d5916070e20a4e55ab081a2f2e40dd3c6506bb53150fb0f6eaf4d255d82`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 1.6 MB (1625461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdc0b4ba0ecebe0776dde4024ee63f953b17cc68a10ebdd312b82a3fd0127fa`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; arm variant v7

```console
$ docker pull hitch@sha256:366b0a87b08677e14a24328b00c1e13d4be89242ddfa84a32696753883641c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28123964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c7aaa1f03bb4efd47023bd435f6c72bec04cb0ae887cb2e8f2d0522ab42ff3`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:34:15 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 07:34:15 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 07:34:16 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 07:34:16 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 07:34:16 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 07:36:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 07:36:29 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 07:36:29 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:36:29 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 07:36:29 GMT
EXPOSE 443
# Wed, 16 Aug 2023 07:36:29 GMT
CMD []
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63299eb73eaf82f2fe926374f1fb4ec255bf190ce110728f6be4575b2e95ffdd`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 1.5 MB (1544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deb4c79b2b9ae842542be5478cade5af3aa28a41be0bf9fc13207661a0d4321`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:689a2683a75f0e3ee97ee7044e42e4fb2dbb7834d6d48f3b896ed4015b7afc73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b36eb7dbf395b0b9dea8496f4fc1312d8819a4102cea678f728db447b9710a`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:10:31 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:10:31 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:10:31 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:10:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:10:32 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:12:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:12:28 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:12:28 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:12:28 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:12:28 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:12:29 GMT
CMD []
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10576dab04f55e719604aeb6ec990863e14fce60cd45ead4d4d2c1bf00b1f8c5`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 1.6 MB (1606793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ee2e032932235bf0fcef63010e523739abc0d743f07813f7f1b15b8633885`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; 386

```console
$ docker pull hitch@sha256:e91c8145e5a7dc5ab7350ecf9b4e16fba1be78cff05897b59b76998ea379bcc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34028517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad5eda2cc0e6bd3957a6becdc500d65f42108755e29712dd7396bb5e138739`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 03:31:26 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 03:34:03 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 03:34:03 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 03:34:03 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:34:03 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 03:34:03 GMT
EXPOSE 443
# Wed, 16 Aug 2023 03:34:03 GMT
CMD []
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08cd8bc2e244a5ca5d75161c4b61834034c4c19641a078d6ca2331987a3a5e`  
		Last Modified: Wed, 16 Aug 2023 03:36:35 GMT  
		Size: 1.6 MB (1630900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451771b9145a8ff1fefbd41b4e243676516ce9736190b765738247abe1d63941`  
		Last Modified: Wed, 16 Aug 2023 03:36:34 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; ppc64le

```console
$ docker pull hitch@sha256:170e62ded87a85f2bfb42acc0e03ab497a04075d00e3397b24105e5744808a9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36979600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13028e41c2ee40d673afa93ae5eaa59f481f41e53ef4089a8543073989e0398`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:33:08 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 04:33:09 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 04:33:10 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 04:33:11 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 04:33:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 04:49:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 04:49:47 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 04:49:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 04:49:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 04:49:48 GMT
EXPOSE 443
# Wed, 16 Aug 2023 04:49:48 GMT
CMD []
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748feeacec9e19e61cf794ad6678c0afa4e219f074fad8b6ec944b793d849669`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 1.7 MB (1688117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e623fea85eb8927b4e51cc68eddc1e0aac4720b7265f235800d3178f1e7f90`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; s390x

```console
$ docker pull hitch@sha256:aae9b16f5a0d350b182f1b49c38419f79e387d6a60991eb25fdaf70dad593ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31275688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96aeac18bbc6090d0b08bcd9bcff4b255931e7267e112e43f8dc4724520cdacb`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:22:21 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:22:21 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:22:22 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:24:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:24:43 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:24:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:24:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:24:43 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:24:43 GMT
CMD []
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a322aa47cfadd0e9cc7a3abd8c7f8fa1f6e3427de7e4c0f50c52acf53581b787`  
		Last Modified: Wed, 16 Aug 2023 01:27:33 GMT  
		Size: 1.6 MB (1622292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f4927bc6be443f72e0510f319233f2bbca6da6728e0cd25d64cb96f1188a09`  
		Last Modified: Wed, 16 Aug 2023 01:27:32 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.2`

```console
$ docker pull hitch@sha256:1a0b77225d9f495a5839762a1c16327ea43ec6640a1f25f81a1bbb5cb435d60c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hitch:1.7.2` - linux; amd64

```console
$ docker pull hitch@sha256:39080aa6cd3487b5a6165940029c66aa4384c4f647cdb8ac52725baef7d5077b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33042942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da3ce046f798e333df6e32c8a8b78a52d9c31c5749667b1ab62aba5a1e569a26`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:57:57 GMT
ARG SRCVER=1.7.2
# Fri, 28 Jul 2023 03:57:57 GMT
ARG PKGVER=1
# Fri, 28 Jul 2023 03:57:57 GMT
ARG DISTVER=bullseye
# Fri, 28 Jul 2023 03:57:57 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Fri, 28 Jul 2023 03:57:58 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Fri, 28 Jul 2023 03:59:33 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 28 Jul 2023 03:59:33 GMT
WORKDIR /etc/hitch
# Fri, 28 Jul 2023 03:59:33 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:59:33 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Fri, 28 Jul 2023 03:59:33 GMT
EXPOSE 443
# Fri, 28 Jul 2023 03:59:33 GMT
CMD []
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e242e66efe50520b3ae0f61abc8502f973fed8a35275e571091d5433ac5437`  
		Last Modified: Fri, 28 Jul 2023 03:59:58 GMT  
		Size: 1.6 MB (1624923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32c337a3b2a61e8c47420e175201d25cff281b5e2c7982e6f7e8c522ddefc7`  
		Last Modified: Fri, 28 Jul 2023 03:59:58 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; arm variant v7

```console
$ docker pull hitch@sha256:7e49d92a0cd0a5e52b4a12e11d37a64f649d858077d231ad1f44fdae3d80968e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ada556e1bc0e6c1105e40b6e1a50b0faf50a45cd94ba566ad9aaacb47c3ead`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:36:37 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 07:36:37 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 07:36:38 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 07:36:38 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 07:36:38 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 07:38:11 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 07:38:11 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 07:38:11 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:38:11 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 07:38:11 GMT
EXPOSE 443
# Wed, 16 Aug 2023 07:38:11 GMT
CMD []
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3670f43fa8489d9b49443d079cf6652dd553832d661ec1677971d11d009b8364`  
		Last Modified: Wed, 16 Aug 2023 07:38:36 GMT  
		Size: 1.5 MB (1543856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6c87670ebc3fc729539eefa720cff085f1462ddad9de7ec1f0ff5866e18f3a`  
		Last Modified: Wed, 16 Aug 2023 07:38:36 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:552c335d4c6c882ecb1405047b099d5d2f5f341ed26b3e3c2063b6527c7099aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31669323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23a9581121e9084c30d768181209d0665086ec41b2c67aa273988bc4d2fdbf1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:12:39 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 01:12:39 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:12:39 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:12:39 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:12:39 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 01:14:08 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:14:08 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:14:08 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:14:08 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:14:08 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:14:08 GMT
CMD []
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d12b031b8acf99a376b64ec40a8dcf2aeda1aacc590331d69d7f4c8a890553`  
		Last Modified: Wed, 16 Aug 2023 01:14:38 GMT  
		Size: 1.6 MB (1606092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baa216d10f08a5ffc7cfd11345942e0238d5820838d5e507f6356adb09e52eb`  
		Last Modified: Wed, 16 Aug 2023 01:14:38 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; 386

```console
$ docker pull hitch@sha256:61d019ddb0ce321b28cf5f60222bb694d377e00efba56ebe47ba1a71ae0bad01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7497ee52b30035085f2dd6f0ac4a8443cca3bc085ed12ef22e2147c4851d767b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:34:19 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 03:34:19 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 03:34:19 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 03:34:19 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 03:34:19 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 03:36:14 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 03:36:14 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 03:36:14 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:36:14 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 03:36:14 GMT
EXPOSE 443
# Wed, 16 Aug 2023 03:36:14 GMT
CMD []
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326ce57826daefad7eeab9f8765d391e9663d7cc03a01005f1ba111fc4330b1d`  
		Last Modified: Wed, 16 Aug 2023 03:36:49 GMT  
		Size: 1.6 MB (1629626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083548839e310d0805c5aca713287d06f8fd26cee5abd3e9f665c6f33563c511`  
		Last Modified: Wed, 16 Aug 2023 03:36:49 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; ppc64le

```console
$ docker pull hitch@sha256:bf403a93c033d98498b5e1cc54e24bfa3e8e6edc1a4717dd4c21919bb9ae4d75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4694e68e94195652eaa0f3aa36688095ef5b40dd2c7a704765c06aadf3cafb4`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:50:05 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 04:50:05 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 04:50:05 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 04:50:06 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 04:50:06 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 04:57:04 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 04:57:05 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 04:57:05 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 04:57:06 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 04:57:06 GMT
EXPOSE 443
# Wed, 16 Aug 2023 04:57:06 GMT
CMD []
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62b731c8d342a441a08b75646c5a4e9f711d2ecc9ef80f49aff6edceafb4e10`  
		Last Modified: Wed, 16 Aug 2023 04:57:52 GMT  
		Size: 1.7 MB (1686083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea59ee51864948a05d7c0517586c67e4d0dd3b5dac08ab7e85376934c2db6e19`  
		Last Modified: Wed, 16 Aug 2023 04:57:51 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; s390x

```console
$ docker pull hitch@sha256:c050c478dcc64680dd3339f17c9c8d474bec04048fde4e2cae5e08d1ba9f5dd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31275196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83ac54e32e79659a4538566ce027155cb47f95877f04d8ce0e2e9d35edcd43cf`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:25:00 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 01:25:00 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:25:00 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:25:01 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:25:01 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 01:27:10 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:27:10 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:27:10 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:27:11 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:27:11 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:27:11 GMT
CMD []
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc12bc467919534224c5685181477d5466c3e1f8a63b912daa485bfe407c225`  
		Last Modified: Wed, 16 Aug 2023 01:27:42 GMT  
		Size: 1.6 MB (1621801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104e1f5321a2c29e118c786da868e82b9f6f94a8b33a22b50d2389aef13689f3`  
		Last Modified: Wed, 16 Aug 2023 01:27:41 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.2-1`

```console
$ docker pull hitch@sha256:1a0b77225d9f495a5839762a1c16327ea43ec6640a1f25f81a1bbb5cb435d60c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hitch:1.7.2-1` - linux; amd64

```console
$ docker pull hitch@sha256:39080aa6cd3487b5a6165940029c66aa4384c4f647cdb8ac52725baef7d5077b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33042942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da3ce046f798e333df6e32c8a8b78a52d9c31c5749667b1ab62aba5a1e569a26`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:57:57 GMT
ARG SRCVER=1.7.2
# Fri, 28 Jul 2023 03:57:57 GMT
ARG PKGVER=1
# Fri, 28 Jul 2023 03:57:57 GMT
ARG DISTVER=bullseye
# Fri, 28 Jul 2023 03:57:57 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Fri, 28 Jul 2023 03:57:58 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Fri, 28 Jul 2023 03:59:33 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 28 Jul 2023 03:59:33 GMT
WORKDIR /etc/hitch
# Fri, 28 Jul 2023 03:59:33 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:59:33 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Fri, 28 Jul 2023 03:59:33 GMT
EXPOSE 443
# Fri, 28 Jul 2023 03:59:33 GMT
CMD []
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e242e66efe50520b3ae0f61abc8502f973fed8a35275e571091d5433ac5437`  
		Last Modified: Fri, 28 Jul 2023 03:59:58 GMT  
		Size: 1.6 MB (1624923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa32c337a3b2a61e8c47420e175201d25cff281b5e2c7982e6f7e8c522ddefc7`  
		Last Modified: Fri, 28 Jul 2023 03:59:58 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:7e49d92a0cd0a5e52b4a12e11d37a64f649d858077d231ad1f44fdae3d80968e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ada556e1bc0e6c1105e40b6e1a50b0faf50a45cd94ba566ad9aaacb47c3ead`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:36:37 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 07:36:37 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 07:36:38 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 07:36:38 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 07:36:38 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 07:38:11 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 07:38:11 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 07:38:11 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:38:11 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 07:38:11 GMT
EXPOSE 443
# Wed, 16 Aug 2023 07:38:11 GMT
CMD []
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3670f43fa8489d9b49443d079cf6652dd553832d661ec1677971d11d009b8364`  
		Last Modified: Wed, 16 Aug 2023 07:38:36 GMT  
		Size: 1.5 MB (1543856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6c87670ebc3fc729539eefa720cff085f1462ddad9de7ec1f0ff5866e18f3a`  
		Last Modified: Wed, 16 Aug 2023 07:38:36 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:552c335d4c6c882ecb1405047b099d5d2f5f341ed26b3e3c2063b6527c7099aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31669323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23a9581121e9084c30d768181209d0665086ec41b2c67aa273988bc4d2fdbf1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:12:39 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 01:12:39 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:12:39 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:12:39 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:12:39 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 01:14:08 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:14:08 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:14:08 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:14:08 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:14:08 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:14:08 GMT
CMD []
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d12b031b8acf99a376b64ec40a8dcf2aeda1aacc590331d69d7f4c8a890553`  
		Last Modified: Wed, 16 Aug 2023 01:14:38 GMT  
		Size: 1.6 MB (1606092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baa216d10f08a5ffc7cfd11345942e0238d5820838d5e507f6356adb09e52eb`  
		Last Modified: Wed, 16 Aug 2023 01:14:38 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; 386

```console
$ docker pull hitch@sha256:61d019ddb0ce321b28cf5f60222bb694d377e00efba56ebe47ba1a71ae0bad01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7497ee52b30035085f2dd6f0ac4a8443cca3bc085ed12ef22e2147c4851d767b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:34:19 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 03:34:19 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 03:34:19 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 03:34:19 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 03:34:19 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 03:36:14 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 03:36:14 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 03:36:14 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:36:14 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 03:36:14 GMT
EXPOSE 443
# Wed, 16 Aug 2023 03:36:14 GMT
CMD []
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326ce57826daefad7eeab9f8765d391e9663d7cc03a01005f1ba111fc4330b1d`  
		Last Modified: Wed, 16 Aug 2023 03:36:49 GMT  
		Size: 1.6 MB (1629626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083548839e310d0805c5aca713287d06f8fd26cee5abd3e9f665c6f33563c511`  
		Last Modified: Wed, 16 Aug 2023 03:36:49 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; ppc64le

```console
$ docker pull hitch@sha256:bf403a93c033d98498b5e1cc54e24bfa3e8e6edc1a4717dd4c21919bb9ae4d75
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4694e68e94195652eaa0f3aa36688095ef5b40dd2c7a704765c06aadf3cafb4`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:50:05 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 04:50:05 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 04:50:05 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 04:50:06 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 04:50:06 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 04:57:04 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 04:57:05 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 04:57:05 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 04:57:06 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 04:57:06 GMT
EXPOSE 443
# Wed, 16 Aug 2023 04:57:06 GMT
CMD []
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62b731c8d342a441a08b75646c5a4e9f711d2ecc9ef80f49aff6edceafb4e10`  
		Last Modified: Wed, 16 Aug 2023 04:57:52 GMT  
		Size: 1.7 MB (1686083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea59ee51864948a05d7c0517586c67e4d0dd3b5dac08ab7e85376934c2db6e19`  
		Last Modified: Wed, 16 Aug 2023 04:57:51 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; s390x

```console
$ docker pull hitch@sha256:c050c478dcc64680dd3339f17c9c8d474bec04048fde4e2cae5e08d1ba9f5dd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31275196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83ac54e32e79659a4538566ce027155cb47f95877f04d8ce0e2e9d35edcd43cf`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:25:00 GMT
ARG SRCVER=1.7.2
# Wed, 16 Aug 2023 01:25:00 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:25:00 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:25:01 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:25:01 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 16 Aug 2023 01:27:10 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:27:10 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:27:10 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:27:11 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:27:11 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:27:11 GMT
CMD []
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc12bc467919534224c5685181477d5466c3e1f8a63b912daa485bfe407c225`  
		Last Modified: Wed, 16 Aug 2023 01:27:42 GMT  
		Size: 1.6 MB (1621801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104e1f5321a2c29e118c786da868e82b9f6f94a8b33a22b50d2389aef13689f3`  
		Last Modified: Wed, 16 Aug 2023 01:27:41 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.3`

```console
$ docker pull hitch@sha256:5dc2200eda652b4445e48262d187006f2fc164d5847319a1a1e222ac9908a23a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hitch:1.7.3` - linux; amd64

```console
$ docker pull hitch@sha256:dd86d288fc7247d23bea302eba8d8922f69f69541b99a327f1c2fa8b08301926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33043480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c3c41df73ba661e191a9e420d638961a7c2b6115db4979eab1f8842499f8e7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SRCVER=1.7.3
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGVER=1
# Fri, 28 Jul 2023 03:55:49 GMT
ARG DISTVER=bullseye
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Fri, 28 Jul 2023 03:57:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 28 Jul 2023 03:57:42 GMT
WORKDIR /etc/hitch
# Fri, 28 Jul 2023 03:57:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:57:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Fri, 28 Jul 2023 03:57:43 GMT
EXPOSE 443
# Fri, 28 Jul 2023 03:57:43 GMT
CMD []
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce4d5916070e20a4e55ab081a2f2e40dd3c6506bb53150fb0f6eaf4d255d82`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 1.6 MB (1625461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdc0b4ba0ecebe0776dde4024ee63f953b17cc68a10ebdd312b82a3fd0127fa`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; arm variant v7

```console
$ docker pull hitch@sha256:366b0a87b08677e14a24328b00c1e13d4be89242ddfa84a32696753883641c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28123964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c7aaa1f03bb4efd47023bd435f6c72bec04cb0ae887cb2e8f2d0522ab42ff3`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:34:15 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 07:34:15 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 07:34:16 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 07:34:16 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 07:34:16 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 07:36:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 07:36:29 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 07:36:29 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:36:29 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 07:36:29 GMT
EXPOSE 443
# Wed, 16 Aug 2023 07:36:29 GMT
CMD []
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63299eb73eaf82f2fe926374f1fb4ec255bf190ce110728f6be4575b2e95ffdd`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 1.5 MB (1544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deb4c79b2b9ae842542be5478cade5af3aa28a41be0bf9fc13207661a0d4321`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:689a2683a75f0e3ee97ee7044e42e4fb2dbb7834d6d48f3b896ed4015b7afc73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b36eb7dbf395b0b9dea8496f4fc1312d8819a4102cea678f728db447b9710a`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:10:31 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:10:31 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:10:31 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:10:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:10:32 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:12:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:12:28 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:12:28 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:12:28 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:12:28 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:12:29 GMT
CMD []
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10576dab04f55e719604aeb6ec990863e14fce60cd45ead4d4d2c1bf00b1f8c5`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 1.6 MB (1606793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ee2e032932235bf0fcef63010e523739abc0d743f07813f7f1b15b8633885`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; 386

```console
$ docker pull hitch@sha256:e91c8145e5a7dc5ab7350ecf9b4e16fba1be78cff05897b59b76998ea379bcc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34028517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad5eda2cc0e6bd3957a6becdc500d65f42108755e29712dd7396bb5e138739`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 03:31:26 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 03:34:03 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 03:34:03 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 03:34:03 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:34:03 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 03:34:03 GMT
EXPOSE 443
# Wed, 16 Aug 2023 03:34:03 GMT
CMD []
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08cd8bc2e244a5ca5d75161c4b61834034c4c19641a078d6ca2331987a3a5e`  
		Last Modified: Wed, 16 Aug 2023 03:36:35 GMT  
		Size: 1.6 MB (1630900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451771b9145a8ff1fefbd41b4e243676516ce9736190b765738247abe1d63941`  
		Last Modified: Wed, 16 Aug 2023 03:36:34 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; ppc64le

```console
$ docker pull hitch@sha256:170e62ded87a85f2bfb42acc0e03ab497a04075d00e3397b24105e5744808a9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36979600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13028e41c2ee40d673afa93ae5eaa59f481f41e53ef4089a8543073989e0398`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:33:08 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 04:33:09 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 04:33:10 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 04:33:11 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 04:33:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 04:49:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 04:49:47 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 04:49:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 04:49:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 04:49:48 GMT
EXPOSE 443
# Wed, 16 Aug 2023 04:49:48 GMT
CMD []
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748feeacec9e19e61cf794ad6678c0afa4e219f074fad8b6ec944b793d849669`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 1.7 MB (1688117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e623fea85eb8927b4e51cc68eddc1e0aac4720b7265f235800d3178f1e7f90`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; s390x

```console
$ docker pull hitch@sha256:aae9b16f5a0d350b182f1b49c38419f79e387d6a60991eb25fdaf70dad593ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31275688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96aeac18bbc6090d0b08bcd9bcff4b255931e7267e112e43f8dc4724520cdacb`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:22:21 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:22:21 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:22:22 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:24:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:24:43 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:24:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:24:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:24:43 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:24:43 GMT
CMD []
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a322aa47cfadd0e9cc7a3abd8c7f8fa1f6e3427de7e4c0f50c52acf53581b787`  
		Last Modified: Wed, 16 Aug 2023 01:27:33 GMT  
		Size: 1.6 MB (1622292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f4927bc6be443f72e0510f319233f2bbca6da6728e0cd25d64cb96f1188a09`  
		Last Modified: Wed, 16 Aug 2023 01:27:32 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.3-1`

```console
$ docker pull hitch@sha256:5dc2200eda652b4445e48262d187006f2fc164d5847319a1a1e222ac9908a23a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hitch:1.7.3-1` - linux; amd64

```console
$ docker pull hitch@sha256:dd86d288fc7247d23bea302eba8d8922f69f69541b99a327f1c2fa8b08301926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33043480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c3c41df73ba661e191a9e420d638961a7c2b6115db4979eab1f8842499f8e7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SRCVER=1.7.3
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGVER=1
# Fri, 28 Jul 2023 03:55:49 GMT
ARG DISTVER=bullseye
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Fri, 28 Jul 2023 03:57:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 28 Jul 2023 03:57:42 GMT
WORKDIR /etc/hitch
# Fri, 28 Jul 2023 03:57:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:57:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Fri, 28 Jul 2023 03:57:43 GMT
EXPOSE 443
# Fri, 28 Jul 2023 03:57:43 GMT
CMD []
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce4d5916070e20a4e55ab081a2f2e40dd3c6506bb53150fb0f6eaf4d255d82`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 1.6 MB (1625461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdc0b4ba0ecebe0776dde4024ee63f953b17cc68a10ebdd312b82a3fd0127fa`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:366b0a87b08677e14a24328b00c1e13d4be89242ddfa84a32696753883641c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28123964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c7aaa1f03bb4efd47023bd435f6c72bec04cb0ae887cb2e8f2d0522ab42ff3`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:34:15 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 07:34:15 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 07:34:16 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 07:34:16 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 07:34:16 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 07:36:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 07:36:29 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 07:36:29 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:36:29 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 07:36:29 GMT
EXPOSE 443
# Wed, 16 Aug 2023 07:36:29 GMT
CMD []
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63299eb73eaf82f2fe926374f1fb4ec255bf190ce110728f6be4575b2e95ffdd`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 1.5 MB (1544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deb4c79b2b9ae842542be5478cade5af3aa28a41be0bf9fc13207661a0d4321`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:689a2683a75f0e3ee97ee7044e42e4fb2dbb7834d6d48f3b896ed4015b7afc73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b36eb7dbf395b0b9dea8496f4fc1312d8819a4102cea678f728db447b9710a`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:10:31 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:10:31 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:10:31 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:10:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:10:32 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:12:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:12:28 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:12:28 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:12:28 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:12:28 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:12:29 GMT
CMD []
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10576dab04f55e719604aeb6ec990863e14fce60cd45ead4d4d2c1bf00b1f8c5`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 1.6 MB (1606793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ee2e032932235bf0fcef63010e523739abc0d743f07813f7f1b15b8633885`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; 386

```console
$ docker pull hitch@sha256:e91c8145e5a7dc5ab7350ecf9b4e16fba1be78cff05897b59b76998ea379bcc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34028517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad5eda2cc0e6bd3957a6becdc500d65f42108755e29712dd7396bb5e138739`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 03:31:26 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 03:34:03 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 03:34:03 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 03:34:03 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:34:03 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 03:34:03 GMT
EXPOSE 443
# Wed, 16 Aug 2023 03:34:03 GMT
CMD []
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08cd8bc2e244a5ca5d75161c4b61834034c4c19641a078d6ca2331987a3a5e`  
		Last Modified: Wed, 16 Aug 2023 03:36:35 GMT  
		Size: 1.6 MB (1630900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451771b9145a8ff1fefbd41b4e243676516ce9736190b765738247abe1d63941`  
		Last Modified: Wed, 16 Aug 2023 03:36:34 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; ppc64le

```console
$ docker pull hitch@sha256:170e62ded87a85f2bfb42acc0e03ab497a04075d00e3397b24105e5744808a9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36979600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13028e41c2ee40d673afa93ae5eaa59f481f41e53ef4089a8543073989e0398`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:33:08 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 04:33:09 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 04:33:10 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 04:33:11 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 04:33:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 04:49:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 04:49:47 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 04:49:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 04:49:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 04:49:48 GMT
EXPOSE 443
# Wed, 16 Aug 2023 04:49:48 GMT
CMD []
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748feeacec9e19e61cf794ad6678c0afa4e219f074fad8b6ec944b793d849669`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 1.7 MB (1688117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e623fea85eb8927b4e51cc68eddc1e0aac4720b7265f235800d3178f1e7f90`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; s390x

```console
$ docker pull hitch@sha256:aae9b16f5a0d350b182f1b49c38419f79e387d6a60991eb25fdaf70dad593ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31275688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96aeac18bbc6090d0b08bcd9bcff4b255931e7267e112e43f8dc4724520cdacb`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:22:21 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:22:21 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:22:22 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:24:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:24:43 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:24:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:24:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:24:43 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:24:43 GMT
CMD []
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a322aa47cfadd0e9cc7a3abd8c7f8fa1f6e3427de7e4c0f50c52acf53581b787`  
		Last Modified: Wed, 16 Aug 2023 01:27:33 GMT  
		Size: 1.6 MB (1622292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f4927bc6be443f72e0510f319233f2bbca6da6728e0cd25d64cb96f1188a09`  
		Last Modified: Wed, 16 Aug 2023 01:27:32 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:latest`

```console
$ docker pull hitch@sha256:5dc2200eda652b4445e48262d187006f2fc164d5847319a1a1e222ac9908a23a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `hitch:latest` - linux; amd64

```console
$ docker pull hitch@sha256:dd86d288fc7247d23bea302eba8d8922f69f69541b99a327f1c2fa8b08301926
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33043480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c3c41df73ba661e191a9e420d638961a7c2b6115db4979eab1f8842499f8e7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SRCVER=1.7.3
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGVER=1
# Fri, 28 Jul 2023 03:55:49 GMT
ARG DISTVER=bullseye
# Fri, 28 Jul 2023 03:55:49 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Fri, 28 Jul 2023 03:55:49 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Fri, 28 Jul 2023 03:57:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Fri, 28 Jul 2023 03:57:42 GMT
WORKDIR /etc/hitch
# Fri, 28 Jul 2023 03:57:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:57:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Fri, 28 Jul 2023 03:57:43 GMT
EXPOSE 443
# Fri, 28 Jul 2023 03:57:43 GMT
CMD []
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce4d5916070e20a4e55ab081a2f2e40dd3c6506bb53150fb0f6eaf4d255d82`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 1.6 MB (1625461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdc0b4ba0ecebe0776dde4024ee63f953b17cc68a10ebdd312b82a3fd0127fa`  
		Last Modified: Fri, 28 Jul 2023 03:59:44 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm variant v7

```console
$ docker pull hitch@sha256:366b0a87b08677e14a24328b00c1e13d4be89242ddfa84a32696753883641c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28123964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75c7aaa1f03bb4efd47023bd435f6c72bec04cb0ae887cb2e8f2d0522ab42ff3`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 00:17:33 GMT
ADD file:d9383f6a4370dbf4af8e05edac181465a410899022cf1788f9001a976b9beecd in / 
# Wed, 16 Aug 2023 00:17:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 07:34:15 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 07:34:15 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 07:34:16 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 07:34:16 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 07:34:16 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 07:36:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 07:36:29 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 07:36:29 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 07:36:29 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 07:36:29 GMT
EXPOSE 443
# Wed, 16 Aug 2023 07:36:29 GMT
CMD []
```

-	Layers:
	-	`sha256:66971a88ba9c0b0ac6503475f1bc4981010269bdba2638318b63c625ee44cd79`  
		Last Modified: Wed, 16 Aug 2023 00:22:09 GMT  
		Size: 26.6 MB (26578637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63299eb73eaf82f2fe926374f1fb4ec255bf190ce110728f6be4575b2e95ffdd`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 1.5 MB (1544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deb4c79b2b9ae842542be5478cade5af3aa28a41be0bf9fc13207661a0d4321`  
		Last Modified: Wed, 16 Aug 2023 07:38:23 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:689a2683a75f0e3ee97ee7044e42e4fb2dbb7834d6d48f3b896ed4015b7afc73
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b36eb7dbf395b0b9dea8496f4fc1312d8819a4102cea678f728db447b9710a`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:10:31 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:10:31 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:10:31 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:10:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:10:32 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:12:28 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:12:28 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:12:28 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:12:28 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:12:28 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:12:29 GMT
CMD []
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10576dab04f55e719604aeb6ec990863e14fce60cd45ead4d4d2c1bf00b1f8c5`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 1.6 MB (1606793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ee2e032932235bf0fcef63010e523739abc0d743f07813f7f1b15b8633885`  
		Last Modified: Wed, 16 Aug 2023 01:14:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; 386

```console
$ docker pull hitch@sha256:e91c8145e5a7dc5ab7350ecf9b4e16fba1be78cff05897b59b76998ea379bcc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34028517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad5eda2cc0e6bd3957a6becdc500d65f42108755e29712dd7396bb5e138739`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 03:31:26 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 03:31:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 03:31:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 03:34:03 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 03:34:03 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 03:34:03 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:34:03 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 03:34:03 GMT
EXPOSE 443
# Wed, 16 Aug 2023 03:34:03 GMT
CMD []
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08cd8bc2e244a5ca5d75161c4b61834034c4c19641a078d6ca2331987a3a5e`  
		Last Modified: Wed, 16 Aug 2023 03:36:35 GMT  
		Size: 1.6 MB (1630900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451771b9145a8ff1fefbd41b4e243676516ce9736190b765738247abe1d63941`  
		Last Modified: Wed, 16 Aug 2023 03:36:34 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; ppc64le

```console
$ docker pull hitch@sha256:170e62ded87a85f2bfb42acc0e03ab497a04075d00e3397b24105e5744808a9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36979600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13028e41c2ee40d673afa93ae5eaa59f481f41e53ef4089a8543073989e0398`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:33:08 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 04:33:09 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 04:33:10 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 04:33:11 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 04:33:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 04:49:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 04:49:47 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 04:49:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 04:49:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 04:49:48 GMT
EXPOSE 443
# Wed, 16 Aug 2023 04:49:48 GMT
CMD []
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748feeacec9e19e61cf794ad6678c0afa4e219f074fad8b6ec944b793d849669`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 1.7 MB (1688117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e623fea85eb8927b4e51cc68eddc1e0aac4720b7265f235800d3178f1e7f90`  
		Last Modified: Wed, 16 Aug 2023 04:57:27 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; s390x

```console
$ docker pull hitch@sha256:aae9b16f5a0d350b182f1b49c38419f79e387d6a60991eb25fdaf70dad593ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31275688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96aeac18bbc6090d0b08bcd9bcff4b255931e7267e112e43f8dc4724520cdacb`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:22:21 GMT
ARG SRCVER=1.7.3
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGVER=1
# Wed, 16 Aug 2023 01:22:21 GMT
ARG DISTVER=bullseye
# Wed, 16 Aug 2023 01:22:21 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 16 Aug 2023 01:22:22 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 16 Aug 2023 01:24:42 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 16 Aug 2023 01:24:43 GMT
WORKDIR /etc/hitch
# Wed, 16 Aug 2023 01:24:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 16 Aug 2023 01:24:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 16 Aug 2023 01:24:43 GMT
EXPOSE 443
# Wed, 16 Aug 2023 01:24:43 GMT
CMD []
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a322aa47cfadd0e9cc7a3abd8c7f8fa1f6e3427de7e4c0f50c52acf53581b787`  
		Last Modified: Wed, 16 Aug 2023 01:27:33 GMT  
		Size: 1.6 MB (1622292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f4927bc6be443f72e0510f319233f2bbca6da6728e0cd25d64cb96f1188a09`  
		Last Modified: Wed, 16 Aug 2023 01:27:32 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
