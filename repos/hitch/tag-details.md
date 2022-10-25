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
$ docker pull hitch@sha256:84dd1333abaa4694fca2f6f5ea4e500012832cbfa39a24917255c766b2352f8e
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
$ docker pull hitch@sha256:36d995e4c365800b5c06add5c708d87d502069fea394c1d621e107804cc611cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33047349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31eaa012aff9da55a8ee56277169c8165d45a24d920c94c24e03018c7a8bb497`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 03:52:47 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 03:55:09 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 03:55:09 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 03:55:09 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:55:09 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 03:55:09 GMT
EXPOSE 443
# Tue, 25 Oct 2022 03:55:09 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb58d7c4ae58e46e9f7f3a133a63fbbeb7fbbbb32e33966f5154e47c3ceec12`  
		Last Modified: Tue, 25 Oct 2022 03:57:30 GMT  
		Size: 1.6 MB (1626893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf6c8e8f72cac1af4a352a706377c56b7874956cf78cc69b2497b88a77e5352`  
		Last Modified: Tue, 25 Oct 2022 03:57:29 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:c3283a6eef4a841b5615979347426737657c6f04db50309a6df4cdbc039790da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28124302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a8c14d30f44235e992dea855eefe79c11acecdf645a81ac79c5cb1f9b834e9`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:44:23 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 04:44:23 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 04:44:23 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 04:44:24 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 04:44:24 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 04:47:47 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 04:47:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 04:47:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:47:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 04:47:47 GMT
EXPOSE 443
# Wed, 05 Oct 2022 04:47:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d6e725ca2d90b23ec09d9769a720c8ea428dc565a0580e00dc0288e7c417ba`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 1.5 MB (1544685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615499f7d1a2e2048c31c156eb0a8969d59364085c1d570ccc14f6a15694b255`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:42b4c7d1f3a61042c2f5b40c68dd79e685c8c761730ee2dbe3dc837fe4d6c689
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fd0a49943c28578194e9fb347286933b0fd6f728a9db912a84e63a56a4dc1b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:49:55 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 02:49:56 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 02:49:57 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 02:49:58 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 02:49:59 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 02:51:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 02:51:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 02:51:49 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 02:51:49 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 02:51:50 GMT
EXPOSE 443
# Wed, 05 Oct 2022 02:51:51 GMT
CMD []
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95364e89f7154274782f6ad794ae91ae0571951aeb714289e5bfe5f5c869a1a`  
		Last Modified: Wed, 05 Oct 2022 02:54:22 GMT  
		Size: 1.6 MB (1605257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9775132c628b975ff7fc4739787103a4e303c8804d5eec385e5d574d277f63`  
		Last Modified: Wed, 05 Oct 2022 02:54:21 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; 386

```console
$ docker pull hitch@sha256:63b2fa866cb3b80aea85010b644c541723bcc1192d7ca41c159e910afa0ccea7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fde1440811f3f87556e6c3a840dafa6dcbd31db3bd7611372e2267b73b49c6b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:05:58 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 07:05:58 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 07:05:59 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 07:06:00 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 07:06:01 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 07:07:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 07:07:46 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 07:07:48 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 07:07:48 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 07:07:49 GMT
EXPOSE 443
# Tue, 25 Oct 2022 07:07:50 GMT
CMD []
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a23a52a14eac897ff94c5663255f63ac00f47e3f92d56ce150927369a540f3`  
		Last Modified: Tue, 25 Oct 2022 07:08:48 GMT  
		Size: 1.6 MB (1630494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743da65dbf1956a87b5553dab51ceb17026da945adc6ea0d618c2786e93a7bd5`  
		Last Modified: Tue, 25 Oct 2022 07:08:47 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; ppc64le

```console
$ docker pull hitch@sha256:aef9636130baad766a8865bc0a547fd3c13f77664af349f6577e46383cc50592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36976726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448f5a3e0ba9222fc71277bdee6606e5ce99bf011717c171edc17484b5941c05`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:29 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:00:30 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:00:30 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:05:00 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:05:01 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:05:01 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:05:02 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:05:02 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:05:03 GMT
CMD []
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c47ce2d6eb834e6aea14721c3590d86bbad7a77c833d00eba6f03cee5705c17`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 1.7 MB (1685725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3acccc09b92b264d693c7278e015a528cbce29e6f53f9fcd8841507b95ae15e`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1` - linux; s390x

```console
$ docker pull hitch@sha256:34847678fc7db4e29cb9d71c7c3bee791a529923d2c2b2af901da500a13aac27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31272868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca021ac184cde0e809a5ea16eb5b2f13621080e0ba4d15a72c13112c525ca525`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:11:26 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:13:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:13:16 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:13:16 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:13:16 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:13:17 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:13:17 GMT
CMD []
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afc180f02764cf61833ae606cadcdecbd185b87ce84699db8ae5b73dfa2b8c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 1.6 MB (1621733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937b0482ead9a2ceea3a620c90fa16d7b0ea3122d256d72945ac78f8c53fb7c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7`

```console
$ docker pull hitch@sha256:84dd1333abaa4694fca2f6f5ea4e500012832cbfa39a24917255c766b2352f8e
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
$ docker pull hitch@sha256:36d995e4c365800b5c06add5c708d87d502069fea394c1d621e107804cc611cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33047349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31eaa012aff9da55a8ee56277169c8165d45a24d920c94c24e03018c7a8bb497`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 03:52:47 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 03:55:09 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 03:55:09 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 03:55:09 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:55:09 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 03:55:09 GMT
EXPOSE 443
# Tue, 25 Oct 2022 03:55:09 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb58d7c4ae58e46e9f7f3a133a63fbbeb7fbbbb32e33966f5154e47c3ceec12`  
		Last Modified: Tue, 25 Oct 2022 03:57:30 GMT  
		Size: 1.6 MB (1626893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf6c8e8f72cac1af4a352a706377c56b7874956cf78cc69b2497b88a77e5352`  
		Last Modified: Tue, 25 Oct 2022 03:57:29 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; arm variant v7

```console
$ docker pull hitch@sha256:c3283a6eef4a841b5615979347426737657c6f04db50309a6df4cdbc039790da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28124302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a8c14d30f44235e992dea855eefe79c11acecdf645a81ac79c5cb1f9b834e9`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:44:23 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 04:44:23 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 04:44:23 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 04:44:24 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 04:44:24 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 04:47:47 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 04:47:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 04:47:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:47:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 04:47:47 GMT
EXPOSE 443
# Wed, 05 Oct 2022 04:47:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d6e725ca2d90b23ec09d9769a720c8ea428dc565a0580e00dc0288e7c417ba`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 1.5 MB (1544685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615499f7d1a2e2048c31c156eb0a8969d59364085c1d570ccc14f6a15694b255`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:42b4c7d1f3a61042c2f5b40c68dd79e685c8c761730ee2dbe3dc837fe4d6c689
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fd0a49943c28578194e9fb347286933b0fd6f728a9db912a84e63a56a4dc1b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:49:55 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 02:49:56 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 02:49:57 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 02:49:58 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 02:49:59 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 02:51:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 02:51:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 02:51:49 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 02:51:49 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 02:51:50 GMT
EXPOSE 443
# Wed, 05 Oct 2022 02:51:51 GMT
CMD []
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95364e89f7154274782f6ad794ae91ae0571951aeb714289e5bfe5f5c869a1a`  
		Last Modified: Wed, 05 Oct 2022 02:54:22 GMT  
		Size: 1.6 MB (1605257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9775132c628b975ff7fc4739787103a4e303c8804d5eec385e5d574d277f63`  
		Last Modified: Wed, 05 Oct 2022 02:54:21 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; 386

```console
$ docker pull hitch@sha256:63b2fa866cb3b80aea85010b644c541723bcc1192d7ca41c159e910afa0ccea7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fde1440811f3f87556e6c3a840dafa6dcbd31db3bd7611372e2267b73b49c6b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:05:58 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 07:05:58 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 07:05:59 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 07:06:00 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 07:06:01 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 07:07:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 07:07:46 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 07:07:48 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 07:07:48 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 07:07:49 GMT
EXPOSE 443
# Tue, 25 Oct 2022 07:07:50 GMT
CMD []
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a23a52a14eac897ff94c5663255f63ac00f47e3f92d56ce150927369a540f3`  
		Last Modified: Tue, 25 Oct 2022 07:08:48 GMT  
		Size: 1.6 MB (1630494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743da65dbf1956a87b5553dab51ceb17026da945adc6ea0d618c2786e93a7bd5`  
		Last Modified: Tue, 25 Oct 2022 07:08:47 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; ppc64le

```console
$ docker pull hitch@sha256:aef9636130baad766a8865bc0a547fd3c13f77664af349f6577e46383cc50592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36976726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448f5a3e0ba9222fc71277bdee6606e5ce99bf011717c171edc17484b5941c05`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:29 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:00:30 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:00:30 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:05:00 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:05:01 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:05:01 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:05:02 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:05:02 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:05:03 GMT
CMD []
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c47ce2d6eb834e6aea14721c3590d86bbad7a77c833d00eba6f03cee5705c17`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 1.7 MB (1685725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3acccc09b92b264d693c7278e015a528cbce29e6f53f9fcd8841507b95ae15e`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7` - linux; s390x

```console
$ docker pull hitch@sha256:34847678fc7db4e29cb9d71c7c3bee791a529923d2c2b2af901da500a13aac27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31272868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca021ac184cde0e809a5ea16eb5b2f13621080e0ba4d15a72c13112c525ca525`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:11:26 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:13:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:13:16 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:13:16 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:13:16 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:13:17 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:13:17 GMT
CMD []
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afc180f02764cf61833ae606cadcdecbd185b87ce84699db8ae5b73dfa2b8c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 1.6 MB (1621733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937b0482ead9a2ceea3a620c90fa16d7b0ea3122d256d72945ac78f8c53fb7c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.2`

```console
$ docker pull hitch@sha256:30855bdab2eba5902c6dce77da75ad54a98f9b8409833aed5f88c047177b39d0
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
$ docker pull hitch@sha256:2f667d7958c58f2ee96cafeaac1d82ca741960282d80fa3e988c1c77beb3d535
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33046227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08f855af8178e5070ed35e221972893da2b6202f1fa533a702c0e191f402dede`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:55:25 GMT
ARG SRCVER=1.7.2
# Tue, 25 Oct 2022 03:55:25 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 03:55:25 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 03:55:25 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 03:55:25 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 25 Oct 2022 03:57:13 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 03:57:13 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 03:57:13 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:57:13 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 03:57:14 GMT
EXPOSE 443
# Tue, 25 Oct 2022 03:57:14 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4503a8a7409de4d531fe522901cff0da45c9c61f5fa806c1fbf8388fd3978e93`  
		Last Modified: Tue, 25 Oct 2022 03:57:45 GMT  
		Size: 1.6 MB (1625773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1d40f25f4a4d92fb51aec663869c43d020de66a8b4e0b8426af694677f49c0`  
		Last Modified: Tue, 25 Oct 2022 03:57:45 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; arm variant v7

```console
$ docker pull hitch@sha256:3ad7de08945fd5166560ce1d89376cd05a78a11a7f0777f0505da1fee1ba4bcc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28111025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46bfbe9cfa1beff3cd0bc6456fed2202583b68d431e334940b7de04c6b00aa1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 11:28:55 GMT
ARG SRCVER=1.7.2
# Tue, 13 Sep 2022 11:28:55 GMT
ARG PKGVER=1
# Tue, 13 Sep 2022 11:28:55 GMT
ARG DISTVER=bullseye
# Tue, 13 Sep 2022 11:28:55 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 13 Sep 2022 11:28:55 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 13 Sep 2022 11:32:15 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 13 Sep 2022 11:32:15 GMT
WORKDIR /etc/hitch
# Tue, 13 Sep 2022 11:32:15 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:32:15 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 13 Sep 2022 11:32:16 GMT
EXPOSE 443
# Tue, 13 Sep 2022 11:32:16 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577650a5f05b1f4222eab725e67338793e555e60f1ca8d1dcad5e364c1a2d41`  
		Last Modified: Tue, 13 Sep 2022 11:32:54 GMT  
		Size: 1.5 MB (1543547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a5bf39dfc76e3e27af3795a3455514058d0ffb0ad4ec6fc439307b45eeb820`  
		Last Modified: Tue, 13 Sep 2022 11:32:54 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:7cea0639c49cd7a901df294a28be03d5c824cc50691b9e4dce792aa17a01b738
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31669174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9afdea8abe6100d28e37a387222f9f03c5327d2704e7d0761baad8c85305c887`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:52:07 GMT
ARG SRCVER=1.7.2
# Wed, 05 Oct 2022 02:52:08 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 02:52:09 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 02:52:10 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 02:52:11 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 05 Oct 2022 02:53:49 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 02:53:50 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 02:53:52 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 02:53:52 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 02:53:53 GMT
EXPOSE 443
# Wed, 05 Oct 2022 02:53:54 GMT
CMD []
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3964222ea193abb35491628128e564f178aa5520e2512fa586b48574566fe37`  
		Last Modified: Wed, 05 Oct 2022 02:54:42 GMT  
		Size: 1.6 MB (1604362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee3258437e265ae0bd68285d62dfcd620f842318d25f25dd7ba6b84cc3f4679`  
		Last Modified: Wed, 05 Oct 2022 02:54:41 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; 386

```console
$ docker pull hitch@sha256:dd6edcc259311a21b2c9873b5810604fa14287460a863ed502d19f06ba543374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34011499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:072fbd64b95bea887d6dd2dfc3aea87e96e5ab467e7b1772e237207d764794ec`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:35:32 GMT
ARG SRCVER=1.7.2
# Tue, 13 Sep 2022 06:35:32 GMT
ARG PKGVER=1
# Tue, 13 Sep 2022 06:35:33 GMT
ARG DISTVER=bullseye
# Tue, 13 Sep 2022 06:35:34 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 13 Sep 2022 06:35:35 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 13 Sep 2022 06:37:21 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 13 Sep 2022 06:37:22 GMT
WORKDIR /etc/hitch
# Tue, 13 Sep 2022 06:37:24 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:37:24 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 13 Sep 2022 06:37:25 GMT
EXPOSE 443
# Tue, 13 Sep 2022 06:37:26 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cced29c1fdf41682e20f38086673848dbbbc5b3a8d7447aaed6ea4f5a6ecce`  
		Last Modified: Tue, 13 Sep 2022 06:37:57 GMT  
		Size: 1.6 MB (1627294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb21f2723f56a8d7bd10678a17e8a61a5165a952b37976a8195da7f36298be12`  
		Last Modified: Tue, 13 Sep 2022 06:37:57 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; ppc64le

```console
$ docker pull hitch@sha256:bcfd89f176752c0e572738410eed11466e68fdf9460b3786223f8241bc92e5b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36975707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c5a3890e780139c3006a2ac055c8d74f81e0caaabc70535d08412a80cc2c538`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:05:10 GMT
ARG SRCVER=1.7.2
# Wed, 05 Oct 2022 01:05:10 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:05:11 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:05:11 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:05:11 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 05 Oct 2022 01:09:10 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:09:11 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:09:11 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:09:12 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:09:12 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:09:12 GMT
CMD []
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d26a31c07f34aaf15f18661930d6b15ff345d0873ec587edfb299800a5c308`  
		Last Modified: Wed, 05 Oct 2022 01:10:03 GMT  
		Size: 1.7 MB (1684706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0681e2c5d2279a2357d361af1b39c96249b3c5662060119642e248d9bc22a7f`  
		Last Modified: Wed, 05 Oct 2022 01:10:01 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2` - linux; s390x

```console
$ docker pull hitch@sha256:28cc6662225888e70a1bf36554a801454a9c5402b789dd781e6b856292d39363
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31272364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13f9b057b3064dca42872469df7fc7222c9500298163d2acdeb9253189211110`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:30 GMT
ARG SRCVER=1.7.2
# Wed, 05 Oct 2022 01:13:30 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:13:30 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:13:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:13:30 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 05 Oct 2022 01:15:43 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:15:43 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:15:44 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:15:44 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:15:44 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:15:44 GMT
CMD []
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76661011c0883c2c13e6e6582480c84b4538414554e3e8a6877b6c73d3429013`  
		Last Modified: Wed, 05 Oct 2022 01:16:24 GMT  
		Size: 1.6 MB (1621229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280374f4ae88955ffdd8f941f24c74d1b46849fb2a034d4b2afdacc0ad34c5fd`  
		Last Modified: Wed, 05 Oct 2022 01:16:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.2-1`

```console
$ docker pull hitch@sha256:30855bdab2eba5902c6dce77da75ad54a98f9b8409833aed5f88c047177b39d0
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
$ docker pull hitch@sha256:2f667d7958c58f2ee96cafeaac1d82ca741960282d80fa3e988c1c77beb3d535
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33046227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08f855af8178e5070ed35e221972893da2b6202f1fa533a702c0e191f402dede`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:55:25 GMT
ARG SRCVER=1.7.2
# Tue, 25 Oct 2022 03:55:25 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 03:55:25 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 03:55:25 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 03:55:25 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 25 Oct 2022 03:57:13 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 03:57:13 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 03:57:13 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:57:13 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 03:57:14 GMT
EXPOSE 443
# Tue, 25 Oct 2022 03:57:14 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4503a8a7409de4d531fe522901cff0da45c9c61f5fa806c1fbf8388fd3978e93`  
		Last Modified: Tue, 25 Oct 2022 03:57:45 GMT  
		Size: 1.6 MB (1625773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1d40f25f4a4d92fb51aec663869c43d020de66a8b4e0b8426af694677f49c0`  
		Last Modified: Tue, 25 Oct 2022 03:57:45 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:3ad7de08945fd5166560ce1d89376cd05a78a11a7f0777f0505da1fee1ba4bcc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28111025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46bfbe9cfa1beff3cd0bc6456fed2202583b68d431e334940b7de04c6b00aa1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 11:28:55 GMT
ARG SRCVER=1.7.2
# Tue, 13 Sep 2022 11:28:55 GMT
ARG PKGVER=1
# Tue, 13 Sep 2022 11:28:55 GMT
ARG DISTVER=bullseye
# Tue, 13 Sep 2022 11:28:55 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 13 Sep 2022 11:28:55 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 13 Sep 2022 11:32:15 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 13 Sep 2022 11:32:15 GMT
WORKDIR /etc/hitch
# Tue, 13 Sep 2022 11:32:15 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:32:15 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 13 Sep 2022 11:32:16 GMT
EXPOSE 443
# Tue, 13 Sep 2022 11:32:16 GMT
CMD []
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577650a5f05b1f4222eab725e67338793e555e60f1ca8d1dcad5e364c1a2d41`  
		Last Modified: Tue, 13 Sep 2022 11:32:54 GMT  
		Size: 1.5 MB (1543547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a5bf39dfc76e3e27af3795a3455514058d0ffb0ad4ec6fc439307b45eeb820`  
		Last Modified: Tue, 13 Sep 2022 11:32:54 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:7cea0639c49cd7a901df294a28be03d5c824cc50691b9e4dce792aa17a01b738
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31669174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9afdea8abe6100d28e37a387222f9f03c5327d2704e7d0761baad8c85305c887`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:52:07 GMT
ARG SRCVER=1.7.2
# Wed, 05 Oct 2022 02:52:08 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 02:52:09 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 02:52:10 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 02:52:11 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 05 Oct 2022 02:53:49 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 02:53:50 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 02:53:52 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 02:53:52 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 02:53:53 GMT
EXPOSE 443
# Wed, 05 Oct 2022 02:53:54 GMT
CMD []
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3964222ea193abb35491628128e564f178aa5520e2512fa586b48574566fe37`  
		Last Modified: Wed, 05 Oct 2022 02:54:42 GMT  
		Size: 1.6 MB (1604362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee3258437e265ae0bd68285d62dfcd620f842318d25f25dd7ba6b84cc3f4679`  
		Last Modified: Wed, 05 Oct 2022 02:54:41 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; 386

```console
$ docker pull hitch@sha256:dd6edcc259311a21b2c9873b5810604fa14287460a863ed502d19f06ba543374
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34011499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:072fbd64b95bea887d6dd2dfc3aea87e96e5ab467e7b1772e237207d764794ec`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:35:32 GMT
ARG SRCVER=1.7.2
# Tue, 13 Sep 2022 06:35:32 GMT
ARG PKGVER=1
# Tue, 13 Sep 2022 06:35:33 GMT
ARG DISTVER=bullseye
# Tue, 13 Sep 2022 06:35:34 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 13 Sep 2022 06:35:35 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 13 Sep 2022 06:37:21 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 13 Sep 2022 06:37:22 GMT
WORKDIR /etc/hitch
# Tue, 13 Sep 2022 06:37:24 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 13 Sep 2022 06:37:24 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 13 Sep 2022 06:37:25 GMT
EXPOSE 443
# Tue, 13 Sep 2022 06:37:26 GMT
CMD []
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cced29c1fdf41682e20f38086673848dbbbc5b3a8d7447aaed6ea4f5a6ecce`  
		Last Modified: Tue, 13 Sep 2022 06:37:57 GMT  
		Size: 1.6 MB (1627294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb21f2723f56a8d7bd10678a17e8a61a5165a952b37976a8195da7f36298be12`  
		Last Modified: Tue, 13 Sep 2022 06:37:57 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; ppc64le

```console
$ docker pull hitch@sha256:bcfd89f176752c0e572738410eed11466e68fdf9460b3786223f8241bc92e5b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36975707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c5a3890e780139c3006a2ac055c8d74f81e0caaabc70535d08412a80cc2c538`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:05:10 GMT
ARG SRCVER=1.7.2
# Wed, 05 Oct 2022 01:05:10 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:05:11 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:05:11 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:05:11 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 05 Oct 2022 01:09:10 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:09:11 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:09:11 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:09:12 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:09:12 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:09:12 GMT
CMD []
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d26a31c07f34aaf15f18661930d6b15ff345d0873ec587edfb299800a5c308`  
		Last Modified: Wed, 05 Oct 2022 01:10:03 GMT  
		Size: 1.7 MB (1684706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0681e2c5d2279a2357d361af1b39c96249b3c5662060119642e248d9bc22a7f`  
		Last Modified: Wed, 05 Oct 2022 01:10:01 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.2-1` - linux; s390x

```console
$ docker pull hitch@sha256:28cc6662225888e70a1bf36554a801454a9c5402b789dd781e6b856292d39363
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31272364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13f9b057b3064dca42872469df7fc7222c9500298163d2acdeb9253189211110`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:30 GMT
ARG SRCVER=1.7.2
# Wed, 05 Oct 2022 01:13:30 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:13:30 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:13:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:13:30 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 05 Oct 2022 01:15:43 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:15:43 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:15:44 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:15:44 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:15:44 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:15:44 GMT
CMD []
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76661011c0883c2c13e6e6582480c84b4538414554e3e8a6877b6c73d3429013`  
		Last Modified: Wed, 05 Oct 2022 01:16:24 GMT  
		Size: 1.6 MB (1621229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280374f4ae88955ffdd8f941f24c74d1b46849fb2a034d4b2afdacc0ad34c5fd`  
		Last Modified: Wed, 05 Oct 2022 01:16:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.3`

```console
$ docker pull hitch@sha256:84dd1333abaa4694fca2f6f5ea4e500012832cbfa39a24917255c766b2352f8e
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
$ docker pull hitch@sha256:36d995e4c365800b5c06add5c708d87d502069fea394c1d621e107804cc611cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33047349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31eaa012aff9da55a8ee56277169c8165d45a24d920c94c24e03018c7a8bb497`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 03:52:47 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 03:55:09 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 03:55:09 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 03:55:09 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:55:09 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 03:55:09 GMT
EXPOSE 443
# Tue, 25 Oct 2022 03:55:09 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb58d7c4ae58e46e9f7f3a133a63fbbeb7fbbbb32e33966f5154e47c3ceec12`  
		Last Modified: Tue, 25 Oct 2022 03:57:30 GMT  
		Size: 1.6 MB (1626893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf6c8e8f72cac1af4a352a706377c56b7874956cf78cc69b2497b88a77e5352`  
		Last Modified: Tue, 25 Oct 2022 03:57:29 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; arm variant v7

```console
$ docker pull hitch@sha256:c3283a6eef4a841b5615979347426737657c6f04db50309a6df4cdbc039790da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28124302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a8c14d30f44235e992dea855eefe79c11acecdf645a81ac79c5cb1f9b834e9`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:44:23 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 04:44:23 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 04:44:23 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 04:44:24 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 04:44:24 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 04:47:47 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 04:47:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 04:47:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:47:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 04:47:47 GMT
EXPOSE 443
# Wed, 05 Oct 2022 04:47:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d6e725ca2d90b23ec09d9769a720c8ea428dc565a0580e00dc0288e7c417ba`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 1.5 MB (1544685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615499f7d1a2e2048c31c156eb0a8969d59364085c1d570ccc14f6a15694b255`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:42b4c7d1f3a61042c2f5b40c68dd79e685c8c761730ee2dbe3dc837fe4d6c689
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fd0a49943c28578194e9fb347286933b0fd6f728a9db912a84e63a56a4dc1b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:49:55 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 02:49:56 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 02:49:57 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 02:49:58 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 02:49:59 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 02:51:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 02:51:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 02:51:49 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 02:51:49 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 02:51:50 GMT
EXPOSE 443
# Wed, 05 Oct 2022 02:51:51 GMT
CMD []
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95364e89f7154274782f6ad794ae91ae0571951aeb714289e5bfe5f5c869a1a`  
		Last Modified: Wed, 05 Oct 2022 02:54:22 GMT  
		Size: 1.6 MB (1605257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9775132c628b975ff7fc4739787103a4e303c8804d5eec385e5d574d277f63`  
		Last Modified: Wed, 05 Oct 2022 02:54:21 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; 386

```console
$ docker pull hitch@sha256:63b2fa866cb3b80aea85010b644c541723bcc1192d7ca41c159e910afa0ccea7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fde1440811f3f87556e6c3a840dafa6dcbd31db3bd7611372e2267b73b49c6b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:05:58 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 07:05:58 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 07:05:59 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 07:06:00 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 07:06:01 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 07:07:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 07:07:46 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 07:07:48 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 07:07:48 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 07:07:49 GMT
EXPOSE 443
# Tue, 25 Oct 2022 07:07:50 GMT
CMD []
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a23a52a14eac897ff94c5663255f63ac00f47e3f92d56ce150927369a540f3`  
		Last Modified: Tue, 25 Oct 2022 07:08:48 GMT  
		Size: 1.6 MB (1630494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743da65dbf1956a87b5553dab51ceb17026da945adc6ea0d618c2786e93a7bd5`  
		Last Modified: Tue, 25 Oct 2022 07:08:47 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; ppc64le

```console
$ docker pull hitch@sha256:aef9636130baad766a8865bc0a547fd3c13f77664af349f6577e46383cc50592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36976726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448f5a3e0ba9222fc71277bdee6606e5ce99bf011717c171edc17484b5941c05`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:29 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:00:30 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:00:30 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:05:00 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:05:01 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:05:01 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:05:02 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:05:02 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:05:03 GMT
CMD []
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c47ce2d6eb834e6aea14721c3590d86bbad7a77c833d00eba6f03cee5705c17`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 1.7 MB (1685725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3acccc09b92b264d693c7278e015a528cbce29e6f53f9fcd8841507b95ae15e`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3` - linux; s390x

```console
$ docker pull hitch@sha256:34847678fc7db4e29cb9d71c7c3bee791a529923d2c2b2af901da500a13aac27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31272868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca021ac184cde0e809a5ea16eb5b2f13621080e0ba4d15a72c13112c525ca525`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:11:26 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:13:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:13:16 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:13:16 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:13:16 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:13:17 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:13:17 GMT
CMD []
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afc180f02764cf61833ae606cadcdecbd185b87ce84699db8ae5b73dfa2b8c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 1.6 MB (1621733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937b0482ead9a2ceea3a620c90fa16d7b0ea3122d256d72945ac78f8c53fb7c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:1.7.3-1`

```console
$ docker pull hitch@sha256:84dd1333abaa4694fca2f6f5ea4e500012832cbfa39a24917255c766b2352f8e
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
$ docker pull hitch@sha256:36d995e4c365800b5c06add5c708d87d502069fea394c1d621e107804cc611cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33047349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31eaa012aff9da55a8ee56277169c8165d45a24d920c94c24e03018c7a8bb497`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 03:52:47 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 03:55:09 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 03:55:09 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 03:55:09 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:55:09 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 03:55:09 GMT
EXPOSE 443
# Tue, 25 Oct 2022 03:55:09 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb58d7c4ae58e46e9f7f3a133a63fbbeb7fbbbb32e33966f5154e47c3ceec12`  
		Last Modified: Tue, 25 Oct 2022 03:57:30 GMT  
		Size: 1.6 MB (1626893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf6c8e8f72cac1af4a352a706377c56b7874956cf78cc69b2497b88a77e5352`  
		Last Modified: Tue, 25 Oct 2022 03:57:29 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; arm variant v7

```console
$ docker pull hitch@sha256:c3283a6eef4a841b5615979347426737657c6f04db50309a6df4cdbc039790da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28124302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a8c14d30f44235e992dea855eefe79c11acecdf645a81ac79c5cb1f9b834e9`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:44:23 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 04:44:23 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 04:44:23 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 04:44:24 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 04:44:24 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 04:47:47 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 04:47:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 04:47:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:47:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 04:47:47 GMT
EXPOSE 443
# Wed, 05 Oct 2022 04:47:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d6e725ca2d90b23ec09d9769a720c8ea428dc565a0580e00dc0288e7c417ba`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 1.5 MB (1544685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615499f7d1a2e2048c31c156eb0a8969d59364085c1d570ccc14f6a15694b255`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:42b4c7d1f3a61042c2f5b40c68dd79e685c8c761730ee2dbe3dc837fe4d6c689
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fd0a49943c28578194e9fb347286933b0fd6f728a9db912a84e63a56a4dc1b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:49:55 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 02:49:56 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 02:49:57 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 02:49:58 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 02:49:59 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 02:51:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 02:51:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 02:51:49 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 02:51:49 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 02:51:50 GMT
EXPOSE 443
# Wed, 05 Oct 2022 02:51:51 GMT
CMD []
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95364e89f7154274782f6ad794ae91ae0571951aeb714289e5bfe5f5c869a1a`  
		Last Modified: Wed, 05 Oct 2022 02:54:22 GMT  
		Size: 1.6 MB (1605257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9775132c628b975ff7fc4739787103a4e303c8804d5eec385e5d574d277f63`  
		Last Modified: Wed, 05 Oct 2022 02:54:21 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; 386

```console
$ docker pull hitch@sha256:63b2fa866cb3b80aea85010b644c541723bcc1192d7ca41c159e910afa0ccea7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fde1440811f3f87556e6c3a840dafa6dcbd31db3bd7611372e2267b73b49c6b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:05:58 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 07:05:58 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 07:05:59 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 07:06:00 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 07:06:01 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 07:07:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 07:07:46 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 07:07:48 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 07:07:48 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 07:07:49 GMT
EXPOSE 443
# Tue, 25 Oct 2022 07:07:50 GMT
CMD []
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a23a52a14eac897ff94c5663255f63ac00f47e3f92d56ce150927369a540f3`  
		Last Modified: Tue, 25 Oct 2022 07:08:48 GMT  
		Size: 1.6 MB (1630494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743da65dbf1956a87b5553dab51ceb17026da945adc6ea0d618c2786e93a7bd5`  
		Last Modified: Tue, 25 Oct 2022 07:08:47 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; ppc64le

```console
$ docker pull hitch@sha256:aef9636130baad766a8865bc0a547fd3c13f77664af349f6577e46383cc50592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36976726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448f5a3e0ba9222fc71277bdee6606e5ce99bf011717c171edc17484b5941c05`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:29 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:00:30 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:00:30 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:05:00 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:05:01 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:05:01 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:05:02 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:05:02 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:05:03 GMT
CMD []
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c47ce2d6eb834e6aea14721c3590d86bbad7a77c833d00eba6f03cee5705c17`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 1.7 MB (1685725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3acccc09b92b264d693c7278e015a528cbce29e6f53f9fcd8841507b95ae15e`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:1.7.3-1` - linux; s390x

```console
$ docker pull hitch@sha256:34847678fc7db4e29cb9d71c7c3bee791a529923d2c2b2af901da500a13aac27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31272868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca021ac184cde0e809a5ea16eb5b2f13621080e0ba4d15a72c13112c525ca525`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:11:26 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:13:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:13:16 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:13:16 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:13:16 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:13:17 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:13:17 GMT
CMD []
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afc180f02764cf61833ae606cadcdecbd185b87ce84699db8ae5b73dfa2b8c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 1.6 MB (1621733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937b0482ead9a2ceea3a620c90fa16d7b0ea3122d256d72945ac78f8c53fb7c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `hitch:latest`

```console
$ docker pull hitch@sha256:84dd1333abaa4694fca2f6f5ea4e500012832cbfa39a24917255c766b2352f8e
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
$ docker pull hitch@sha256:36d995e4c365800b5c06add5c708d87d502069fea394c1d621e107804cc611cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33047349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31eaa012aff9da55a8ee56277169c8165d45a24d920c94c24e03018c7a8bb497`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 03:52:47 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 03:52:47 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 03:52:47 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 03:55:09 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 03:55:09 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 03:55:09 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 03:55:09 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 03:55:09 GMT
EXPOSE 443
# Tue, 25 Oct 2022 03:55:09 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb58d7c4ae58e46e9f7f3a133a63fbbeb7fbbbb32e33966f5154e47c3ceec12`  
		Last Modified: Tue, 25 Oct 2022 03:57:30 GMT  
		Size: 1.6 MB (1626893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf6c8e8f72cac1af4a352a706377c56b7874956cf78cc69b2497b88a77e5352`  
		Last Modified: Tue, 25 Oct 2022 03:57:29 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm variant v7

```console
$ docker pull hitch@sha256:c3283a6eef4a841b5615979347426737657c6f04db50309a6df4cdbc039790da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28124302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a8c14d30f44235e992dea855eefe79c11acecdf645a81ac79c5cb1f9b834e9`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:44:23 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 04:44:23 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 04:44:23 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 04:44:24 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 04:44:24 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 04:47:47 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 04:47:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 04:47:47 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:47:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 04:47:47 GMT
EXPOSE 443
# Wed, 05 Oct 2022 04:47:47 GMT
CMD []
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d6e725ca2d90b23ec09d9769a720c8ea428dc565a0580e00dc0288e7c417ba`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 1.5 MB (1544685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615499f7d1a2e2048c31c156eb0a8969d59364085c1d570ccc14f6a15694b255`  
		Last Modified: Wed, 05 Oct 2022 04:48:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:42b4c7d1f3a61042c2f5b40c68dd79e685c8c761730ee2dbe3dc837fe4d6c689
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31670069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02fd0a49943c28578194e9fb347286933b0fd6f728a9db912a84e63a56a4dc1b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:49:55 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 02:49:56 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 02:49:57 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 02:49:58 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 02:49:59 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 02:51:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 02:51:47 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 02:51:49 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 02:51:49 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 02:51:50 GMT
EXPOSE 443
# Wed, 05 Oct 2022 02:51:51 GMT
CMD []
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95364e89f7154274782f6ad794ae91ae0571951aeb714289e5bfe5f5c869a1a`  
		Last Modified: Wed, 05 Oct 2022 02:54:22 GMT  
		Size: 1.6 MB (1605257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9775132c628b975ff7fc4739787103a4e303c8804d5eec385e5d574d277f63`  
		Last Modified: Wed, 05 Oct 2022 02:54:21 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; 386

```console
$ docker pull hitch@sha256:63b2fa866cb3b80aea85010b644c541723bcc1192d7ca41c159e910afa0ccea7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fde1440811f3f87556e6c3a840dafa6dcbd31db3bd7611372e2267b73b49c6b`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:05:58 GMT
ARG SRCVER=1.7.3
# Tue, 25 Oct 2022 07:05:58 GMT
ARG PKGVER=1
# Tue, 25 Oct 2022 07:05:59 GMT
ARG DISTVER=bullseye
# Tue, 25 Oct 2022 07:06:00 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 25 Oct 2022 07:06:01 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Tue, 25 Oct 2022 07:07:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 25 Oct 2022 07:07:46 GMT
WORKDIR /etc/hitch
# Tue, 25 Oct 2022 07:07:48 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 25 Oct 2022 07:07:48 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 25 Oct 2022 07:07:49 GMT
EXPOSE 443
# Tue, 25 Oct 2022 07:07:50 GMT
CMD []
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a23a52a14eac897ff94c5663255f63ac00f47e3f92d56ce150927369a540f3`  
		Last Modified: Tue, 25 Oct 2022 07:08:48 GMT  
		Size: 1.6 MB (1630494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743da65dbf1956a87b5553dab51ceb17026da945adc6ea0d618c2786e93a7bd5`  
		Last Modified: Tue, 25 Oct 2022 07:08:47 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; ppc64le

```console
$ docker pull hitch@sha256:aef9636130baad766a8865bc0a547fd3c13f77664af349f6577e46383cc50592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36976726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448f5a3e0ba9222fc71277bdee6606e5ce99bf011717c171edc17484b5941c05`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:29 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:00:30 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:00:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:00:30 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:05:00 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:05:01 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:05:01 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:05:02 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:05:02 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:05:03 GMT
CMD []
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c47ce2d6eb834e6aea14721c3590d86bbad7a77c833d00eba6f03cee5705c17`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 1.7 MB (1685725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3acccc09b92b264d693c7278e015a528cbce29e6f53f9fcd8841507b95ae15e`  
		Last Modified: Wed, 05 Oct 2022 01:09:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; s390x

```console
$ docker pull hitch@sha256:34847678fc7db4e29cb9d71c7c3bee791a529923d2c2b2af901da500a13aac27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31272868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca021ac184cde0e809a5ea16eb5b2f13621080e0ba4d15a72c13112c525ca525`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SRCVER=1.7.3
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGVER=1
# Wed, 05 Oct 2022 01:11:26 GMT
ARG DISTVER=bullseye
# Wed, 05 Oct 2022 01:11:26 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 05 Oct 2022 01:11:26 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 05 Oct 2022 01:13:16 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 05 Oct 2022 01:13:16 GMT
WORKDIR /etc/hitch
# Wed, 05 Oct 2022 01:13:16 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:13:16 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 05 Oct 2022 01:13:17 GMT
EXPOSE 443
# Wed, 05 Oct 2022 01:13:17 GMT
CMD []
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afc180f02764cf61833ae606cadcdecbd185b87ce84699db8ae5b73dfa2b8c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 1.6 MB (1621733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4937b0482ead9a2ceea3a620c90fa16d7b0ea3122d256d72945ac78f8c53fb7c`  
		Last Modified: Wed, 05 Oct 2022 01:16:12 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
