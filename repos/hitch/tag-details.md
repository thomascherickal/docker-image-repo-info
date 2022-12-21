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
$ docker pull hitch@sha256:43fc4c3dbde99c44adab03493e539370662692af1c71b34500a8b70ce9414df9
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
$ docker pull hitch@sha256:f14d110cb4d7e8e459b78070f702c8bf4462ee33ccae0f4b1566289e7e6ff283
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33022705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea953b1a3bf2478c7e52c1d861292f5c24eca774e3783ae06114172371525de`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:21:10 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:23:30 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:23:30 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:23:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:23:31 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:23:31 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:23:31 GMT
CMD []
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741ed73a429d5b9f41afe5f1258939496be0dc25f0cb456bd16c6a5aee8ecd96`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 1.6 MB (1625345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd019e7737ccc2cba8baaa86d4c00f56f703f0443530a21b077c4ea320b4ddf`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:f88104317429478f144d7c4d8a4125c2eb9693222ea1dbfa05e01a6764d0d5af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e5e699541101d0b8e18bde690a5f89ebd7007e5e3b5ec4222392093792968b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:07:27 GMT
ARG SRCVER=1.7.3
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:07:28 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:07:28 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 06 Dec 2022 12:10:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:10:16 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:10:17 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:10:17 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:10:17 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:10:18 GMT
CMD []
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9ad4ff3fd12955e07cf3d2160368482e741271732f982704b87a0ea115dd42`  
		Last Modified: Tue, 06 Dec 2022 12:13:49 GMT  
		Size: 1.5 MB (1545947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243e2c64e1cf68da5310f5806acde4ec598c66c8c8854df458c970dc869f4bf`  
		Last Modified: Tue, 06 Dec 2022 12:13:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:f139ae56a7d672b4a9c1621a97a60c30614f3d96c9805ab7bf7927bf30518275
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31651618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c6da4958193421111758d7d1f5eeba6b5a969d2d42339c07c9b5642991fd19`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:45:13 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:45:13 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:45:13 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:45:14 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:45:14 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:47:04 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:47:04 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:47:04 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:47:04 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:47:04 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:47:04 GMT
CMD []
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7dff703463282f8c492df6a820ac7e727f0ff9cb2b2146b708e246b6d9939c`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 1.6 MB (1606430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32591fd624e2bcde4b8cc40a6b74d5e19b96c1fc7be2844cb4fd7e4741d7b524`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; 386

```console
$ docker pull hitch@sha256:2d8e8d8e6f3d339230f8dcf6e5a0da68fc0e85e32982e3480a2d39a0d3aaf97c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34005009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f7106c1a59290f2dbd49620d14e7d409b730952cd1e9e25e6b3ff631677783`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:48:26 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 07:48:26 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 07:48:27 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 07:48:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 07:48:29 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 07:50:17 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 07:50:17 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 07:50:19 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:50:19 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 07:50:20 GMT
EXPOSE 443
# Wed, 21 Dec 2022 07:50:21 GMT
CMD []
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea67b56ca5e7d21b769d4fad68a0004766c47d7fcec2ddeff21afe2ab17bfeb`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 1.6 MB (1628847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498f8b88828e0e994c293e82b8139e15886b159c7a9b0cd8847b00cd0de63963`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; ppc64le

```console
$ docker pull hitch@sha256:5135243319b7b25ca1350d27d6d8e8319a9f468319176d4bcce1007bc3083dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36954806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347a684cd4562e425e4fa55e68fbe1b1aed4637667ee19503dd2a1f308762ea7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:42:12 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 01:42:12 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 01:42:12 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 01:42:13 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 01:42:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 01:46:26 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 01:46:27 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 01:46:27 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:46:27 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 01:46:27 GMT
EXPOSE 443
# Wed, 21 Dec 2022 01:46:28 GMT
CMD []
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb578c09a36e4f105c35b83055a1dbb428e9036863a578c8d8927cb883a87f76`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 1.7 MB (1685642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665bae59559a5b9e78f8831d461acdc631268c647c17d2b6f63de8ede764bd0e`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; s390x

```console
$ docker pull hitch@sha256:ebadc9598c5ff65956c44018c2a216c149d2aadb4603ea2c89aea854987d1040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31253477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a7b35a924c94b0ded6d07c9397b21707c955f5eed408f9e00e5b15f84840f1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:32:37 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 02:32:37 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 02:32:38 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 02:32:39 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 02:32:39 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 02:38:37 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 02:38:38 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 02:38:39 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:38:40 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 02:38:40 GMT
EXPOSE 443
# Wed, 21 Dec 2022 02:38:41 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6117cce0c9da63fc1c0ca948f7cc507feb02975c0d9c21bdc829b3aae2a16f`  
		Last Modified: Wed, 21 Dec 2022 02:45:15 GMT  
		Size: 1.6 MB (1623301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba5dd1533ee81be227ff1a276786f6c99e9e6801c4e144ab5272d6864308b7e`  
		Last Modified: Wed, 21 Dec 2022 02:45:14 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7`

```console
$ docker pull hitch@sha256:43fc4c3dbde99c44adab03493e539370662692af1c71b34500a8b70ce9414df9
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
$ docker pull hitch@sha256:f14d110cb4d7e8e459b78070f702c8bf4462ee33ccae0f4b1566289e7e6ff283
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33022705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea953b1a3bf2478c7e52c1d861292f5c24eca774e3783ae06114172371525de`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:21:10 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:23:30 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:23:30 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:23:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:23:31 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:23:31 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:23:31 GMT
CMD []
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741ed73a429d5b9f41afe5f1258939496be0dc25f0cb456bd16c6a5aee8ecd96`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 1.6 MB (1625345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd019e7737ccc2cba8baaa86d4c00f56f703f0443530a21b077c4ea320b4ddf`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; arm variant v7

```console
$ docker pull hitch@sha256:f88104317429478f144d7c4d8a4125c2eb9693222ea1dbfa05e01a6764d0d5af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e5e699541101d0b8e18bde690a5f89ebd7007e5e3b5ec4222392093792968b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:07:27 GMT
ARG SRCVER=1.7.3
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:07:28 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:07:28 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 06 Dec 2022 12:10:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:10:16 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:10:17 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:10:17 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:10:17 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:10:18 GMT
CMD []
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9ad4ff3fd12955e07cf3d2160368482e741271732f982704b87a0ea115dd42`  
		Last Modified: Tue, 06 Dec 2022 12:13:49 GMT  
		Size: 1.5 MB (1545947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243e2c64e1cf68da5310f5806acde4ec598c66c8c8854df458c970dc869f4bf`  
		Last Modified: Tue, 06 Dec 2022 12:13:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:f139ae56a7d672b4a9c1621a97a60c30614f3d96c9805ab7bf7927bf30518275
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31651618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c6da4958193421111758d7d1f5eeba6b5a969d2d42339c07c9b5642991fd19`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:45:13 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:45:13 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:45:13 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:45:14 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:45:14 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:47:04 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:47:04 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:47:04 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:47:04 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:47:04 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:47:04 GMT
CMD []
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7dff703463282f8c492df6a820ac7e727f0ff9cb2b2146b708e246b6d9939c`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 1.6 MB (1606430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32591fd624e2bcde4b8cc40a6b74d5e19b96c1fc7be2844cb4fd7e4741d7b524`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; 386

```console
$ docker pull hitch@sha256:2d8e8d8e6f3d339230f8dcf6e5a0da68fc0e85e32982e3480a2d39a0d3aaf97c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34005009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f7106c1a59290f2dbd49620d14e7d409b730952cd1e9e25e6b3ff631677783`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:48:26 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 07:48:26 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 07:48:27 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 07:48:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 07:48:29 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 07:50:17 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 07:50:17 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 07:50:19 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:50:19 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 07:50:20 GMT
EXPOSE 443
# Wed, 21 Dec 2022 07:50:21 GMT
CMD []
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea67b56ca5e7d21b769d4fad68a0004766c47d7fcec2ddeff21afe2ab17bfeb`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 1.6 MB (1628847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498f8b88828e0e994c293e82b8139e15886b159c7a9b0cd8847b00cd0de63963`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; ppc64le

```console
$ docker pull hitch@sha256:5135243319b7b25ca1350d27d6d8e8319a9f468319176d4bcce1007bc3083dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36954806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347a684cd4562e425e4fa55e68fbe1b1aed4637667ee19503dd2a1f308762ea7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:42:12 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 01:42:12 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 01:42:12 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 01:42:13 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 01:42:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 01:46:26 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 01:46:27 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 01:46:27 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:46:27 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 01:46:27 GMT
EXPOSE 443
# Wed, 21 Dec 2022 01:46:28 GMT
CMD []
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb578c09a36e4f105c35b83055a1dbb428e9036863a578c8d8927cb883a87f76`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 1.7 MB (1685642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665bae59559a5b9e78f8831d461acdc631268c647c17d2b6f63de8ede764bd0e`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; s390x

```console
$ docker pull hitch@sha256:ebadc9598c5ff65956c44018c2a216c149d2aadb4603ea2c89aea854987d1040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31253477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a7b35a924c94b0ded6d07c9397b21707c955f5eed408f9e00e5b15f84840f1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:32:37 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 02:32:37 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 02:32:38 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 02:32:39 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 02:32:39 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 02:38:37 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 02:38:38 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 02:38:39 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:38:40 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 02:38:40 GMT
EXPOSE 443
# Wed, 21 Dec 2022 02:38:41 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6117cce0c9da63fc1c0ca948f7cc507feb02975c0d9c21bdc829b3aae2a16f`  
		Last Modified: Wed, 21 Dec 2022 02:45:15 GMT  
		Size: 1.6 MB (1623301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba5dd1533ee81be227ff1a276786f6c99e9e6801c4e144ab5272d6864308b7e`  
		Last Modified: Wed, 21 Dec 2022 02:45:14 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.2`

```console
$ docker pull hitch@sha256:3b906b83e7b69693c5d204fc7ab0ba5efffe2fa16cc96a8f4e511409e29cba35
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
$ docker pull hitch@sha256:55bfc0952e2e06fcbdea5407839860a1db8ec72cbf4087dc10da738019f66759
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33022077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560e2e44e8335d84aa3c0728ac60684ab1cbe7c65736869aad415007ea7e11f0`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:23:48 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 03:23:48 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:23:48 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:23:48 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:23:48 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 03:25:36 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:25:36 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:25:36 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:25:36 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:25:36 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:25:36 GMT
CMD []
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29fd80c95187e5c923ca65660af29867268f7fc4d635d70f4ee768913070b2`  
		Last Modified: Wed, 21 Dec 2022 03:26:06 GMT  
		Size: 1.6 MB (1624718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0358a84b53426694ffa1c595f6ce75152307b373036f536c65b505b4a8e62533`  
		Last Modified: Wed, 21 Dec 2022 03:26:06 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; arm variant v7

```console
$ docker pull hitch@sha256:9c38a44b86e64b908bf38167204893b5de050e766a8e979690444910697cb6f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28121938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c350336c657baf352c2423fb1ec36e31f6c3e573e120b8c3eb3384e3f6cce55`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:10:28 GMT
ARG SRCVER=1.7.2
# Tue, 06 Dec 2022 12:10:28 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:10:28 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:10:29 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:10:29 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 06 Dec 2022 12:13:13 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:13:13 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:13:14 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:13:14 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:13:14 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:13:15 GMT
CMD []
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a98e79134a51b7b28ae221881414f945c3c0c5fa6063682cef352f866b18b7`  
		Last Modified: Tue, 06 Dec 2022 12:14:09 GMT  
		Size: 1.5 MB (1545173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad226e1f99e6ee073633159a50b108d5bcd7d6414b005e00e0ef46c621bb736b`  
		Last Modified: Tue, 06 Dec 2022 12:14:09 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:7f6403e3ef4dee934c8034db1b968b96066edc79d6cad003f8ab3ea9d78cb9b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31650876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ccc71ef6934c050bc08695d7e2ab90265ce79f2183bf222c5f5530d3445d1e6`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:47:06 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 03:47:06 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:47:06 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:47:06 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:47:06 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 03:48:30 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:48:30 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:48:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:48:30 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:48:30 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:48:30 GMT
CMD []
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68785441280ea70a10ed8e5c753741dc8004cfbf482b87f4e15bfb692fa7d54a`  
		Last Modified: Wed, 21 Dec 2022 03:49:09 GMT  
		Size: 1.6 MB (1605687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d9c0e9e797d576f4fd8183ce94b6b1f46689444c275be868c36b44b9ccac5f`  
		Last Modified: Wed, 21 Dec 2022 03:49:09 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; 386

```console
$ docker pull hitch@sha256:42b8fa3fdbce9fdc1a212814ad14aed0c28a1f071a1040f6454b07eb7ead8b99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34022607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f81ed977b70403d20c2125640c78bc52442378d8c55f9282107fee89c9231061`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:44:29 GMT
ARG SRCVER=1.7.2
# Tue, 06 Dec 2022 12:44:30 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:44:31 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:44:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:44:33 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 06 Dec 2022 12:46:12 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:46:12 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:46:14 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:46:14 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:46:15 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:46:16 GMT
CMD []
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034482fb0930c61fec2ff0f44314c6e55a1eb78df5339f11e1f4fd678dc6c615`  
		Last Modified: Tue, 06 Dec 2022 12:47:01 GMT  
		Size: 1.6 MB (1629145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e20adfe4ad13dc3b20d4df713b3f3b3a3d7f2613c2cb3f992b93d885095e8`  
		Last Modified: Tue, 06 Dec 2022 12:47:01 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; ppc64le

```console
$ docker pull hitch@sha256:ac57773140079f8f6cf9be0ca7dafa83d5af67f78d5324a5a0688aaf9e7cd9c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36953877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03ec7a94561fb34158abc4b0937745343111d4d3a09fec3520659986f628dce5`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:46:37 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 01:46:38 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 01:46:38 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 01:46:38 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 01:46:39 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 01:50:29 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 01:50:29 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 01:50:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:50:30 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 01:50:30 GMT
EXPOSE 443
# Wed, 21 Dec 2022 01:50:30 GMT
CMD []
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae365c5aa289f2da4bb0fe1dc09c94647e3b78aca71e2e5bd10c63175fc02ed1`  
		Last Modified: Wed, 21 Dec 2022 01:51:27 GMT  
		Size: 1.7 MB (1684710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe215e86f3c57628f83f74432f37458cdad62e18645c544415b3fc644cdacefd`  
		Last Modified: Wed, 21 Dec 2022 01:51:26 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; s390x

```console
$ docker pull hitch@sha256:134ce64c9732ff7e86c6acf56d515a1cb75078da070a6b1d3b2b0450fb1425cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31252852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:728fc2480c27a827890a770a7f380de35f071ef3affc39e9bb19f3e38e4e9be3`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:38:54 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 02:38:54 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 02:38:55 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 02:38:56 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 02:38:56 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 02:44:41 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 02:44:42 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 02:44:42 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:44:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 02:44:43 GMT
EXPOSE 443
# Wed, 21 Dec 2022 02:44:44 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c17941c8746377f0b1b64c19a9a66190e40ad9601dfdbc1bea0c28b56e4ca`  
		Last Modified: Wed, 21 Dec 2022 02:45:28 GMT  
		Size: 1.6 MB (1622674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58e7586df7a5f91e1d3da0c8e7a39d9f65a54ec741a36ce2e98c466bb446a6`  
		Last Modified: Wed, 21 Dec 2022 02:45:28 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.2-1`

```console
$ docker pull hitch@sha256:3b906b83e7b69693c5d204fc7ab0ba5efffe2fa16cc96a8f4e511409e29cba35
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
$ docker pull hitch@sha256:55bfc0952e2e06fcbdea5407839860a1db8ec72cbf4087dc10da738019f66759
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33022077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:560e2e44e8335d84aa3c0728ac60684ab1cbe7c65736869aad415007ea7e11f0`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:23:48 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 03:23:48 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:23:48 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:23:48 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:23:48 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 03:25:36 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:25:36 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:25:36 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:25:36 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:25:36 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:25:36 GMT
CMD []
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29fd80c95187e5c923ca65660af29867268f7fc4d635d70f4ee768913070b2`  
		Last Modified: Wed, 21 Dec 2022 03:26:06 GMT  
		Size: 1.6 MB (1624718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0358a84b53426694ffa1c595f6ce75152307b373036f536c65b505b4a8e62533`  
		Last Modified: Wed, 21 Dec 2022 03:26:06 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:9c38a44b86e64b908bf38167204893b5de050e766a8e979690444910697cb6f4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28121938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c350336c657baf352c2423fb1ec36e31f6c3e573e120b8c3eb3384e3f6cce55`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:10:28 GMT
ARG SRCVER=1.7.2
# Tue, 06 Dec 2022 12:10:28 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:10:28 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:10:29 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:10:29 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 06 Dec 2022 12:13:13 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:13:13 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:13:14 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:13:14 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:13:14 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:13:15 GMT
CMD []
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a98e79134a51b7b28ae221881414f945c3c0c5fa6063682cef352f866b18b7`  
		Last Modified: Tue, 06 Dec 2022 12:14:09 GMT  
		Size: 1.5 MB (1545173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad226e1f99e6ee073633159a50b108d5bcd7d6414b005e00e0ef46c621bb736b`  
		Last Modified: Tue, 06 Dec 2022 12:14:09 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:7f6403e3ef4dee934c8034db1b968b96066edc79d6cad003f8ab3ea9d78cb9b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31650876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ccc71ef6934c050bc08695d7e2ab90265ce79f2183bf222c5f5530d3445d1e6`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:47:06 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 03:47:06 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:47:06 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:47:06 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:47:06 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 03:48:30 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:48:30 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:48:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:48:30 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:48:30 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:48:30 GMT
CMD []
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68785441280ea70a10ed8e5c753741dc8004cfbf482b87f4e15bfb692fa7d54a`  
		Last Modified: Wed, 21 Dec 2022 03:49:09 GMT  
		Size: 1.6 MB (1605687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d9c0e9e797d576f4fd8183ce94b6b1f46689444c275be868c36b44b9ccac5f`  
		Last Modified: Wed, 21 Dec 2022 03:49:09 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; 386

```console
$ docker pull hitch@sha256:42b8fa3fdbce9fdc1a212814ad14aed0c28a1f071a1040f6454b07eb7ead8b99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34022607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f81ed977b70403d20c2125640c78bc52442378d8c55f9282107fee89c9231061`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:44:29 GMT
ARG SRCVER=1.7.2
# Tue, 06 Dec 2022 12:44:30 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:44:31 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:44:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:44:33 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 06 Dec 2022 12:46:12 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:46:12 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:46:14 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:46:14 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:46:15 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:46:16 GMT
CMD []
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034482fb0930c61fec2ff0f44314c6e55a1eb78df5339f11e1f4fd678dc6c615`  
		Last Modified: Tue, 06 Dec 2022 12:47:01 GMT  
		Size: 1.6 MB (1629145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2e20adfe4ad13dc3b20d4df713b3f3b3a3d7f2613c2cb3f992b93d885095e8`  
		Last Modified: Tue, 06 Dec 2022 12:47:01 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; ppc64le

```console
$ docker pull hitch@sha256:ac57773140079f8f6cf9be0ca7dafa83d5af67f78d5324a5a0688aaf9e7cd9c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36953877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03ec7a94561fb34158abc4b0937745343111d4d3a09fec3520659986f628dce5`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:46:37 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 01:46:38 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 01:46:38 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 01:46:38 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 01:46:39 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 01:50:29 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 01:50:29 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 01:50:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:50:30 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 01:50:30 GMT
EXPOSE 443
# Wed, 21 Dec 2022 01:50:30 GMT
CMD []
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae365c5aa289f2da4bb0fe1dc09c94647e3b78aca71e2e5bd10c63175fc02ed1`  
		Last Modified: Wed, 21 Dec 2022 01:51:27 GMT  
		Size: 1.7 MB (1684710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe215e86f3c57628f83f74432f37458cdad62e18645c544415b3fc644cdacefd`  
		Last Modified: Wed, 21 Dec 2022 01:51:26 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; s390x

```console
$ docker pull hitch@sha256:134ce64c9732ff7e86c6acf56d515a1cb75078da070a6b1d3b2b0450fb1425cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31252852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:728fc2480c27a827890a770a7f380de35f071ef3affc39e9bb19f3e38e4e9be3`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:38:54 GMT
ARG SRCVER=1.7.2
# Wed, 21 Dec 2022 02:38:54 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 02:38:55 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 02:38:56 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 02:38:56 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 21 Dec 2022 02:44:41 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 02:44:42 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 02:44:42 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:44:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 02:44:43 GMT
EXPOSE 443
# Wed, 21 Dec 2022 02:44:44 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c17941c8746377f0b1b64c19a9a66190e40ad9601dfdbc1bea0c28b56e4ca`  
		Last Modified: Wed, 21 Dec 2022 02:45:28 GMT  
		Size: 1.6 MB (1622674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd58e7586df7a5f91e1d3da0c8e7a39d9f65a54ec741a36ce2e98c466bb446a6`  
		Last Modified: Wed, 21 Dec 2022 02:45:28 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.3`

```console
$ docker pull hitch@sha256:43fc4c3dbde99c44adab03493e539370662692af1c71b34500a8b70ce9414df9
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
$ docker pull hitch@sha256:f14d110cb4d7e8e459b78070f702c8bf4462ee33ccae0f4b1566289e7e6ff283
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33022705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea953b1a3bf2478c7e52c1d861292f5c24eca774e3783ae06114172371525de`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:21:10 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:23:30 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:23:30 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:23:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:23:31 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:23:31 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:23:31 GMT
CMD []
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741ed73a429d5b9f41afe5f1258939496be0dc25f0cb456bd16c6a5aee8ecd96`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 1.6 MB (1625345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd019e7737ccc2cba8baaa86d4c00f56f703f0443530a21b077c4ea320b4ddf`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; arm variant v7

```console
$ docker pull hitch@sha256:f88104317429478f144d7c4d8a4125c2eb9693222ea1dbfa05e01a6764d0d5af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e5e699541101d0b8e18bde690a5f89ebd7007e5e3b5ec4222392093792968b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:07:27 GMT
ARG SRCVER=1.7.3
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:07:28 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:07:28 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 06 Dec 2022 12:10:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:10:16 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:10:17 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:10:17 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:10:17 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:10:18 GMT
CMD []
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9ad4ff3fd12955e07cf3d2160368482e741271732f982704b87a0ea115dd42`  
		Last Modified: Tue, 06 Dec 2022 12:13:49 GMT  
		Size: 1.5 MB (1545947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243e2c64e1cf68da5310f5806acde4ec598c66c8c8854df458c970dc869f4bf`  
		Last Modified: Tue, 06 Dec 2022 12:13:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:f139ae56a7d672b4a9c1621a97a60c30614f3d96c9805ab7bf7927bf30518275
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31651618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c6da4958193421111758d7d1f5eeba6b5a969d2d42339c07c9b5642991fd19`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:45:13 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:45:13 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:45:13 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:45:14 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:45:14 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:47:04 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:47:04 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:47:04 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:47:04 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:47:04 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:47:04 GMT
CMD []
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7dff703463282f8c492df6a820ac7e727f0ff9cb2b2146b708e246b6d9939c`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 1.6 MB (1606430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32591fd624e2bcde4b8cc40a6b74d5e19b96c1fc7be2844cb4fd7e4741d7b524`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; 386

```console
$ docker pull hitch@sha256:2d8e8d8e6f3d339230f8dcf6e5a0da68fc0e85e32982e3480a2d39a0d3aaf97c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34005009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f7106c1a59290f2dbd49620d14e7d409b730952cd1e9e25e6b3ff631677783`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:48:26 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 07:48:26 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 07:48:27 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 07:48:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 07:48:29 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 07:50:17 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 07:50:17 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 07:50:19 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:50:19 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 07:50:20 GMT
EXPOSE 443
# Wed, 21 Dec 2022 07:50:21 GMT
CMD []
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea67b56ca5e7d21b769d4fad68a0004766c47d7fcec2ddeff21afe2ab17bfeb`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 1.6 MB (1628847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498f8b88828e0e994c293e82b8139e15886b159c7a9b0cd8847b00cd0de63963`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; ppc64le

```console
$ docker pull hitch@sha256:5135243319b7b25ca1350d27d6d8e8319a9f468319176d4bcce1007bc3083dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36954806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347a684cd4562e425e4fa55e68fbe1b1aed4637667ee19503dd2a1f308762ea7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:42:12 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 01:42:12 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 01:42:12 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 01:42:13 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 01:42:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 01:46:26 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 01:46:27 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 01:46:27 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:46:27 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 01:46:27 GMT
EXPOSE 443
# Wed, 21 Dec 2022 01:46:28 GMT
CMD []
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb578c09a36e4f105c35b83055a1dbb428e9036863a578c8d8927cb883a87f76`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 1.7 MB (1685642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665bae59559a5b9e78f8831d461acdc631268c647c17d2b6f63de8ede764bd0e`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; s390x

```console
$ docker pull hitch@sha256:ebadc9598c5ff65956c44018c2a216c149d2aadb4603ea2c89aea854987d1040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31253477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a7b35a924c94b0ded6d07c9397b21707c955f5eed408f9e00e5b15f84840f1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:32:37 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 02:32:37 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 02:32:38 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 02:32:39 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 02:32:39 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 02:38:37 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 02:38:38 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 02:38:39 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:38:40 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 02:38:40 GMT
EXPOSE 443
# Wed, 21 Dec 2022 02:38:41 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6117cce0c9da63fc1c0ca948f7cc507feb02975c0d9c21bdc829b3aae2a16f`  
		Last Modified: Wed, 21 Dec 2022 02:45:15 GMT  
		Size: 1.6 MB (1623301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba5dd1533ee81be227ff1a276786f6c99e9e6801c4e144ab5272d6864308b7e`  
		Last Modified: Wed, 21 Dec 2022 02:45:14 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.3-1`

```console
$ docker pull hitch@sha256:43fc4c3dbde99c44adab03493e539370662692af1c71b34500a8b70ce9414df9
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
$ docker pull hitch@sha256:f14d110cb4d7e8e459b78070f702c8bf4462ee33ccae0f4b1566289e7e6ff283
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33022705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea953b1a3bf2478c7e52c1d861292f5c24eca774e3783ae06114172371525de`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:21:10 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:23:30 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:23:30 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:23:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:23:31 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:23:31 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:23:31 GMT
CMD []
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741ed73a429d5b9f41afe5f1258939496be0dc25f0cb456bd16c6a5aee8ecd96`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 1.6 MB (1625345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd019e7737ccc2cba8baaa86d4c00f56f703f0443530a21b077c4ea320b4ddf`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:f88104317429478f144d7c4d8a4125c2eb9693222ea1dbfa05e01a6764d0d5af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e5e699541101d0b8e18bde690a5f89ebd7007e5e3b5ec4222392093792968b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:07:27 GMT
ARG SRCVER=1.7.3
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:07:28 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:07:28 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 06 Dec 2022 12:10:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:10:16 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:10:17 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:10:17 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:10:17 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:10:18 GMT
CMD []
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9ad4ff3fd12955e07cf3d2160368482e741271732f982704b87a0ea115dd42`  
		Last Modified: Tue, 06 Dec 2022 12:13:49 GMT  
		Size: 1.5 MB (1545947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243e2c64e1cf68da5310f5806acde4ec598c66c8c8854df458c970dc869f4bf`  
		Last Modified: Tue, 06 Dec 2022 12:13:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:f139ae56a7d672b4a9c1621a97a60c30614f3d96c9805ab7bf7927bf30518275
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31651618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c6da4958193421111758d7d1f5eeba6b5a969d2d42339c07c9b5642991fd19`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:45:13 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:45:13 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:45:13 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:45:14 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:45:14 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:47:04 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:47:04 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:47:04 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:47:04 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:47:04 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:47:04 GMT
CMD []
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7dff703463282f8c492df6a820ac7e727f0ff9cb2b2146b708e246b6d9939c`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 1.6 MB (1606430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32591fd624e2bcde4b8cc40a6b74d5e19b96c1fc7be2844cb4fd7e4741d7b524`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; 386

```console
$ docker pull hitch@sha256:2d8e8d8e6f3d339230f8dcf6e5a0da68fc0e85e32982e3480a2d39a0d3aaf97c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34005009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f7106c1a59290f2dbd49620d14e7d409b730952cd1e9e25e6b3ff631677783`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:48:26 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 07:48:26 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 07:48:27 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 07:48:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 07:48:29 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 07:50:17 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 07:50:17 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 07:50:19 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:50:19 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 07:50:20 GMT
EXPOSE 443
# Wed, 21 Dec 2022 07:50:21 GMT
CMD []
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea67b56ca5e7d21b769d4fad68a0004766c47d7fcec2ddeff21afe2ab17bfeb`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 1.6 MB (1628847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498f8b88828e0e994c293e82b8139e15886b159c7a9b0cd8847b00cd0de63963`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; ppc64le

```console
$ docker pull hitch@sha256:5135243319b7b25ca1350d27d6d8e8319a9f468319176d4bcce1007bc3083dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36954806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347a684cd4562e425e4fa55e68fbe1b1aed4637667ee19503dd2a1f308762ea7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:42:12 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 01:42:12 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 01:42:12 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 01:42:13 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 01:42:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 01:46:26 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 01:46:27 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 01:46:27 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:46:27 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 01:46:27 GMT
EXPOSE 443
# Wed, 21 Dec 2022 01:46:28 GMT
CMD []
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb578c09a36e4f105c35b83055a1dbb428e9036863a578c8d8927cb883a87f76`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 1.7 MB (1685642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665bae59559a5b9e78f8831d461acdc631268c647c17d2b6f63de8ede764bd0e`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; s390x

```console
$ docker pull hitch@sha256:ebadc9598c5ff65956c44018c2a216c149d2aadb4603ea2c89aea854987d1040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31253477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a7b35a924c94b0ded6d07c9397b21707c955f5eed408f9e00e5b15f84840f1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:32:37 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 02:32:37 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 02:32:38 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 02:32:39 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 02:32:39 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 02:38:37 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 02:38:38 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 02:38:39 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:38:40 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 02:38:40 GMT
EXPOSE 443
# Wed, 21 Dec 2022 02:38:41 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6117cce0c9da63fc1c0ca948f7cc507feb02975c0d9c21bdc829b3aae2a16f`  
		Last Modified: Wed, 21 Dec 2022 02:45:15 GMT  
		Size: 1.6 MB (1623301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba5dd1533ee81be227ff1a276786f6c99e9e6801c4e144ab5272d6864308b7e`  
		Last Modified: Wed, 21 Dec 2022 02:45:14 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:latest`

```console
$ docker pull hitch@sha256:43fc4c3dbde99c44adab03493e539370662692af1c71b34500a8b70ce9414df9
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
$ docker pull hitch@sha256:f14d110cb4d7e8e459b78070f702c8bf4462ee33ccae0f4b1566289e7e6ff283
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33022705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bea953b1a3bf2478c7e52c1d861292f5c24eca774e3783ae06114172371525de`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:21:10 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:21:10 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:21:10 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:23:30 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:23:30 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:23:30 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:23:31 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:23:31 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:23:31 GMT
CMD []
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741ed73a429d5b9f41afe5f1258939496be0dc25f0cb456bd16c6a5aee8ecd96`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 1.6 MB (1625345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd019e7737ccc2cba8baaa86d4c00f56f703f0443530a21b077c4ea320b4ddf`  
		Last Modified: Wed, 21 Dec 2022 03:25:52 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm variant v7

```console
$ docker pull hitch@sha256:f88104317429478f144d7c4d8a4125c2eb9693222ea1dbfa05e01a6764d0d5af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e5e699541101d0b8e18bde690a5f89ebd7007e5e3b5ec4222392093792968b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:07:27 GMT
ARG SRCVER=1.7.3
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGVER=1
# Tue, 06 Dec 2022 12:07:28 GMT
ARG DISTVER=bullseye
# Tue, 06 Dec 2022 12:07:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 06 Dec 2022 12:07:28 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 06 Dec 2022 12:10:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 06 Dec 2022 12:10:16 GMT
WORKDIR /etc/hitch
# Tue, 06 Dec 2022 12:10:17 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 06 Dec 2022 12:10:17 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 06 Dec 2022 12:10:17 GMT
EXPOSE 443
# Tue, 06 Dec 2022 12:10:18 GMT
CMD []
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9ad4ff3fd12955e07cf3d2160368482e741271732f982704b87a0ea115dd42`  
		Last Modified: Tue, 06 Dec 2022 12:13:49 GMT  
		Size: 1.5 MB (1545947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b243e2c64e1cf68da5310f5806acde4ec598c66c8c8854df458c970dc869f4bf`  
		Last Modified: Tue, 06 Dec 2022 12:13:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:f139ae56a7d672b4a9c1621a97a60c30614f3d96c9805ab7bf7927bf30518275
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31651618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c6da4958193421111758d7d1f5eeba6b5a969d2d42339c07c9b5642991fd19`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 03:45:13 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 03:45:13 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 03:45:13 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 03:45:14 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 03:45:14 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 03:47:04 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 03:47:04 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 03:47:04 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 03:47:04 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 03:47:04 GMT
EXPOSE 443
# Wed, 21 Dec 2022 03:47:04 GMT
CMD []
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7dff703463282f8c492df6a820ac7e727f0ff9cb2b2146b708e246b6d9939c`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 1.6 MB (1606430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32591fd624e2bcde4b8cc40a6b74d5e19b96c1fc7be2844cb4fd7e4741d7b524`  
		Last Modified: Wed, 21 Dec 2022 03:48:55 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; 386

```console
$ docker pull hitch@sha256:2d8e8d8e6f3d339230f8dcf6e5a0da68fc0e85e32982e3480a2d39a0d3aaf97c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34005009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f7106c1a59290f2dbd49620d14e7d409b730952cd1e9e25e6b3ff631677783`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 07:48:26 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 07:48:26 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 07:48:27 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 07:48:28 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 07:48:29 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 07:50:17 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 07:50:17 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 07:50:19 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 07:50:19 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 07:50:20 GMT
EXPOSE 443
# Wed, 21 Dec 2022 07:50:21 GMT
CMD []
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea67b56ca5e7d21b769d4fad68a0004766c47d7fcec2ddeff21afe2ab17bfeb`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 1.6 MB (1628847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498f8b88828e0e994c293e82b8139e15886b159c7a9b0cd8847b00cd0de63963`  
		Last Modified: Wed, 21 Dec 2022 07:51:29 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; ppc64le

```console
$ docker pull hitch@sha256:5135243319b7b25ca1350d27d6d8e8319a9f468319176d4bcce1007bc3083dda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36954806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:347a684cd4562e425e4fa55e68fbe1b1aed4637667ee19503dd2a1f308762ea7`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:17:41 GMT
ADD file:5ab731e5c1e145738476449b6b0748f44822bb2cd6c53ae5bbf6ae6bfec83383 in / 
# Wed, 21 Dec 2022 01:17:43 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 01:42:12 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 01:42:12 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 01:42:12 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 01:42:13 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 01:42:13 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 01:46:26 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 01:46:27 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 01:46:27 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 01:46:27 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 01:46:27 GMT
EXPOSE 443
# Wed, 21 Dec 2022 01:46:28 GMT
CMD []
```

-	Layers:
	-	`sha256:ba010cdd67bb149ba042a834d84020887fc3f8ca9d8e51b31f3104286cafb9ba`  
		Last Modified: Wed, 21 Dec 2022 01:23:22 GMT  
		Size: 35.3 MB (35268748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb578c09a36e4f105c35b83055a1dbb428e9036863a578c8d8927cb883a87f76`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 1.7 MB (1685642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665bae59559a5b9e78f8831d461acdc631268c647c17d2b6f63de8ede764bd0e`  
		Last Modified: Wed, 21 Dec 2022 01:51:06 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; s390x

```console
$ docker pull hitch@sha256:ebadc9598c5ff65956c44018c2a216c149d2aadb4603ea2c89aea854987d1040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31253477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a7b35a924c94b0ded6d07c9397b21707c955f5eed408f9e00e5b15f84840f1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:32:37 GMT
ARG SRCVER=1.7.3
# Wed, 21 Dec 2022 02:32:37 GMT
ARG PKGVER=1
# Wed, 21 Dec 2022 02:32:38 GMT
ARG DISTVER=bullseye
# Wed, 21 Dec 2022 02:32:39 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 21 Dec 2022 02:32:39 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 21 Dec 2022 02:38:37 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 21 Dec 2022 02:38:38 GMT
WORKDIR /etc/hitch
# Wed, 21 Dec 2022 02:38:39 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 21 Dec 2022 02:38:40 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 21 Dec 2022 02:38:40 GMT
EXPOSE 443
# Wed, 21 Dec 2022 02:38:41 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6117cce0c9da63fc1c0ca948f7cc507feb02975c0d9c21bdc829b3aae2a16f`  
		Last Modified: Wed, 21 Dec 2022 02:45:15 GMT  
		Size: 1.6 MB (1623301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba5dd1533ee81be227ff1a276786f6c99e9e6801c4e144ab5272d6864308b7e`  
		Last Modified: Wed, 21 Dec 2022 02:45:14 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
