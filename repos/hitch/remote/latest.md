## `hitch:latest`

```console
$ docker pull hitch@sha256:9e3e2303ef3700c8fa7cbe27ee88db523791efb4c4ddcfa25137386a1b92cac6
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
$ docker pull hitch@sha256:29772d91ef9e9adda675924bc35839255290265f73e7b698ae5f0b6aa2fa6faa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33037195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dd6789b0cca2e56d2a5f21561b469cc731732629130b716b1901af77dc056f1`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:03:06 GMT
ARG SRCVER=1.7.3
# Thu, 23 Mar 2023 09:03:06 GMT
ARG PKGVER=1
# Thu, 23 Mar 2023 09:03:06 GMT
ARG DISTVER=bullseye
# Thu, 23 Mar 2023 09:03:06 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Thu, 23 Mar 2023 09:03:06 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Thu, 23 Mar 2023 09:04:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Thu, 23 Mar 2023 09:04:46 GMT
WORKDIR /etc/hitch
# Thu, 23 Mar 2023 09:04:46 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Thu, 23 Mar 2023 09:04:47 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Thu, 23 Mar 2023 09:04:47 GMT
EXPOSE 443
# Thu, 23 Mar 2023 09:04:47 GMT
CMD []
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8422672b718df163d48d8770bc2fc26e636e674e3bc568b31fc519d059fe7523`  
		Last Modified: Thu, 23 Mar 2023 09:06:59 GMT  
		Size: 1.6 MB (1625373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0097a13b7672ceb33ed3dafa8f2387483ad38996c0ebc046ce6321d956889cd0`  
		Last Modified: Thu, 23 Mar 2023 09:06:59 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm variant v7

```console
$ docker pull hitch@sha256:202c905a2c884ee1f03545aea5e71fffffd7782cb6a0c4246a3a861dd81efda3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28122472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab0665c0bf275d66c5498c4a86e9b6eab7a5b6c04fbe7523d3b9793d24639ff`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:55:31 GMT
ARG SRCVER=1.7.3
# Thu, 23 Mar 2023 13:55:31 GMT
ARG PKGVER=1
# Thu, 23 Mar 2023 13:55:31 GMT
ARG DISTVER=bullseye
# Thu, 23 Mar 2023 13:55:31 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Thu, 23 Mar 2023 13:55:32 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Thu, 23 Mar 2023 13:57:33 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Thu, 23 Mar 2023 13:57:33 GMT
WORKDIR /etc/hitch
# Thu, 23 Mar 2023 13:57:33 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:57:33 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Thu, 23 Mar 2023 13:57:33 GMT
EXPOSE 443
# Thu, 23 Mar 2023 13:57:33 GMT
CMD []
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a010b4473fa92487c63b03017552465230eab9a10424eac1acc3e40d82199c67`  
		Last Modified: Thu, 23 Mar 2023 13:59:22 GMT  
		Size: 1.5 MB (1544726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0c464d155387d2d85ed6403923cd56399199115628ea48013d13ec7807b79f`  
		Last Modified: Thu, 23 Mar 2023 13:59:22 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:d6b59173cb3c959d01c5d1d3c5a302d1cafc1a482d2271f3137cf24f57703ac3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31669776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc611773b1329502cb956be1743edacd7672c0f23e68bac9d8a57e778a6f7c2e`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:03:19 GMT
ARG SRCVER=1.7.3
# Thu, 23 Mar 2023 09:03:20 GMT
ARG PKGVER=1
# Thu, 23 Mar 2023 09:03:20 GMT
ARG DISTVER=bullseye
# Thu, 23 Mar 2023 09:03:20 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Thu, 23 Mar 2023 09:03:20 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Thu, 23 Mar 2023 09:05:15 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Thu, 23 Mar 2023 09:05:15 GMT
WORKDIR /etc/hitch
# Thu, 23 Mar 2023 09:05:15 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Thu, 23 Mar 2023 09:05:15 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Thu, 23 Mar 2023 09:05:16 GMT
EXPOSE 443
# Thu, 23 Mar 2023 09:05:16 GMT
CMD []
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622376863cef1f9da68edfcfdffdb9a6a37e5114603f8bb7bedfbbe4fa8e0811`  
		Last Modified: Thu, 23 Mar 2023 09:07:11 GMT  
		Size: 1.6 MB (1606660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fceec7e8461add66360ad23de7c4c1166a2431beb19d7ed45dba01aca0070343`  
		Last Modified: Thu, 23 Mar 2023 09:07:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; 386

```console
$ docker pull hitch@sha256:5ba24bbab7cabe7d33a59f74c809c5bf259e02cecd9a4fca5d600ce2af059c47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34027330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f96d00fc3a7321d2bc2b8b66be316e6437bf823f7d144324ebcf7debc192376`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:33:22 GMT
ARG SRCVER=1.7.3
# Thu, 23 Mar 2023 13:33:22 GMT
ARG PKGVER=1
# Thu, 23 Mar 2023 13:33:22 GMT
ARG DISTVER=bullseye
# Thu, 23 Mar 2023 13:33:23 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Thu, 23 Mar 2023 13:33:23 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Thu, 23 Mar 2023 13:35:43 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Thu, 23 Mar 2023 13:35:43 GMT
WORKDIR /etc/hitch
# Thu, 23 Mar 2023 13:35:43 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Thu, 23 Mar 2023 13:35:43 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Thu, 23 Mar 2023 13:35:43 GMT
EXPOSE 443
# Thu, 23 Mar 2023 13:35:43 GMT
CMD []
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc4931c4990dbe152d19fb2123fa103183b676dd82355d6fb3458af88885edd`  
		Last Modified: Thu, 23 Mar 2023 13:38:00 GMT  
		Size: 1.6 MB (1630637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7908a50943fce32558af8b87267097713e9e5b3f19ef4ed31dbeb56dd0d3a376`  
		Last Modified: Thu, 23 Mar 2023 13:37:59 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; ppc64le

```console
$ docker pull hitch@sha256:c4bfbfe92edb8b472d4e3bee9948b68deda643ca80dd2fbbf5084546218130e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36975427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:222dcf52aedc0519c9e35a435d024f9bc41eb9b840c6edc9d1b39bd3bc42f14d`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:14:54 GMT
ARG SRCVER=1.7.3
# Wed, 01 Mar 2023 07:14:55 GMT
ARG PKGVER=1
# Wed, 01 Mar 2023 07:14:56 GMT
ARG DISTVER=bullseye
# Wed, 01 Mar 2023 07:14:57 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 01 Mar 2023 07:14:57 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Wed, 01 Mar 2023 07:22:46 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 01 Mar 2023 07:22:49 GMT
WORKDIR /etc/hitch
# Wed, 01 Mar 2023 07:22:49 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:22:50 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 01 Mar 2023 07:22:51 GMT
EXPOSE 443
# Wed, 01 Mar 2023 07:22:52 GMT
CMD []
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5e2e36befa4e6c2cd1e6a05e005e2ad1654902712260765409e7b442a8c9d9`  
		Last Modified: Wed, 01 Mar 2023 07:30:49 GMT  
		Size: 1.7 MB (1686908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf887eb6fdc393f5e32dcf73cfc0f50d1dc31a6b36f3cfdccf856706b8c3d296`  
		Last Modified: Wed, 01 Mar 2023 07:30:48 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; s390x

```console
$ docker pull hitch@sha256:5d83b684351e043b05170e7194208f83a4a3abeafb5cce4d6672dc8c96c2a0ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31269045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff87c3374d43f2559c779e248c7350d72c699bcf5f997af1f155ebbff8c01771`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:30:48 GMT
ARG SRCVER=1.7.3
# Thu, 23 Mar 2023 07:30:48 GMT
ARG PKGVER=1
# Thu, 23 Mar 2023 07:30:48 GMT
ARG DISTVER=bullseye
# Thu, 23 Mar 2023 07:30:48 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Thu, 23 Mar 2023 07:30:48 GMT
ARG SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd
# Thu, 23 Mar 2023 07:32:33 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=88de82e639e7f9b7873bb7226fcbcbc4cd5779c75a5bd21fca8e1ca927a2a3ae9eb455d73d1f42d4dc45546118c718d1b58396836ed9c8acac281d487c9fe8fd SRCVER=1.7.3
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Thu, 23 Mar 2023 07:32:33 GMT
WORKDIR /etc/hitch
# Thu, 23 Mar 2023 07:32:33 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Thu, 23 Mar 2023 07:32:34 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Thu, 23 Mar 2023 07:32:34 GMT
EXPOSE 443
# Thu, 23 Mar 2023 07:32:34 GMT
CMD []
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48c46cc60a24c339d4acca7b380b4c4e8f785720cffe89e5523c5e4cb08528d`  
		Last Modified: Thu, 23 Mar 2023 07:34:48 GMT  
		Size: 1.6 MB (1621810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddd4be5d821c570301c90a696ce075f45d1a06f81d051b3e8608dfd88aa2f76`  
		Last Modified: Thu, 23 Mar 2023 07:34:48 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
