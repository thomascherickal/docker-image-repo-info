## `hitch:latest`

```console
$ docker pull hitch@sha256:faae09f3e5516d109be7f0f249ecf5db6ff44a9f29c446224ad1f42258ea8bc6
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
$ docker pull hitch@sha256:ee51d7df7b69de719b92c08621505471d8a3b15aa46fb240f08d3b52c010b102
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32990797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfc6447461562934447f3e2709811df50d7ac35ac38086d54ce5debfe046832f`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:29:46 GMT
ARG SRCVER=1.7.2
# Wed, 26 Jan 2022 08:29:46 GMT
ARG PKGVER=1
# Wed, 26 Jan 2022 08:29:46 GMT
ARG DISTVER=bullseye
# Wed, 26 Jan 2022 08:29:47 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 26 Jan 2022 08:29:47 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 26 Jan 2022 08:32:08 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 26 Jan 2022 08:32:09 GMT
WORKDIR /etc/hitch
# Wed, 26 Jan 2022 08:32:09 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:32:09 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 26 Jan 2022 08:32:10 GMT
EXPOSE 443
# Wed, 26 Jan 2022 08:32:10 GMT
CMD []
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd17d9d8301f421892a07cb2aaff987f63ff75f07eb3ef52e3e8b561c62ee92`  
		Last Modified: Wed, 26 Jan 2022 08:32:34 GMT  
		Size: 1.6 MB (1624124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd4107775047a3e2fc9845b4efa7440b96413cb89cbb6d57261bdabceb26ab`  
		Last Modified: Wed, 26 Jan 2022 08:32:33 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm variant v7

```console
$ docker pull hitch@sha256:3604a90b382539625bbc8c4985afb598e21f8d79e03ea25135b5e05308d1b305
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28108980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0202f1713de46f40a9ab5957f20677b1b72a9fd89628856eb8e79d4b1c7739d`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:17:06 GMT
ARG SRCVER=1.7.2
# Tue, 01 Mar 2022 10:17:06 GMT
ARG PKGVER=1
# Tue, 01 Mar 2022 10:17:07 GMT
ARG DISTVER=bullseye
# Tue, 01 Mar 2022 10:17:07 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 01 Mar 2022 10:17:08 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 01 Mar 2022 10:21:14 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 01 Mar 2022 10:21:14 GMT
WORKDIR /etc/hitch
# Tue, 01 Mar 2022 10:21:15 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 01 Mar 2022 10:21:15 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 01 Mar 2022 10:21:15 GMT
EXPOSE 443
# Tue, 01 Mar 2022 10:21:16 GMT
CMD []
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794a0e9f4aa15740c66f95392e1476ce760bc7b493d47d2234425a65e3b3745d`  
		Last Modified: Tue, 01 Mar 2022 10:21:54 GMT  
		Size: 1.5 MB (1543458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d33b6c19d35b5d79c73b8ba90064d3701a4dfe47076a6f858dfd35a2efe3fc`  
		Last Modified: Tue, 01 Mar 2022 10:21:53 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; arm64 variant v8

```console
$ docker pull hitch@sha256:2ac8edbb3e6994be40da1d0ba375ad55ebdff60e021730246d6e1a47047a573b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31661324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c24da1fca2620488ef2d4732174b582198eca5dcdcf0450dfea1f562f27c8ec`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:27:29 GMT
ARG SRCVER=1.7.2
# Wed, 26 Jan 2022 04:27:30 GMT
ARG PKGVER=1
# Wed, 26 Jan 2022 04:27:31 GMT
ARG DISTVER=bullseye
# Wed, 26 Jan 2022 04:27:32 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 26 Jan 2022 04:27:33 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 26 Jan 2022 04:29:24 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 26 Jan 2022 04:29:25 GMT
WORKDIR /etc/hitch
# Wed, 26 Jan 2022 04:29:27 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:29:27 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 26 Jan 2022 04:29:28 GMT
EXPOSE 443
# Wed, 26 Jan 2022 04:29:29 GMT
CMD []
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cf3035de0cb4738786162b0e07a4176777477ec999819496d363d9c71f6251`  
		Last Modified: Wed, 26 Jan 2022 04:29:55 GMT  
		Size: 1.6 MB (1604132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6dcf282ece70ef16bcc9b938810aea685d11488c38a7671d754742617e6864`  
		Last Modified: Wed, 26 Jan 2022 04:29:54 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; 386

```console
$ docker pull hitch@sha256:5b4c22e7da6f1fa67a5d74c37c4fc1dde7ea0f000d8322051c435eab47660d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34006158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e94905711531b7a59227905b194b529fe072af8b7232eeacb9cde8434553760`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:43:30 GMT
ARG SRCVER=1.7.2
# Tue, 01 Mar 2022 09:43:30 GMT
ARG PKGVER=1
# Tue, 01 Mar 2022 09:43:30 GMT
ARG DISTVER=bullseye
# Tue, 01 Mar 2022 09:43:30 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Tue, 01 Mar 2022 09:43:30 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Tue, 01 Mar 2022 09:46:08 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Tue, 01 Mar 2022 09:46:08 GMT
WORKDIR /etc/hitch
# Tue, 01 Mar 2022 09:46:08 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Tue, 01 Mar 2022 09:46:08 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Tue, 01 Mar 2022 09:46:09 GMT
EXPOSE 443
# Tue, 01 Mar 2022 09:46:09 GMT
CMD []
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d65c60f9ef03feed7b43710d0b7c70ae51f8d4bc6d167c80a5fb304a931d8d`  
		Last Modified: Tue, 01 Mar 2022 09:46:42 GMT  
		Size: 1.6 MB (1628354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911063703f0c894637981125ccfefc5cb54793d894f04cbeb189ece07ada83c2`  
		Last Modified: Tue, 01 Mar 2022 09:46:41 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; ppc64le

```console
$ docker pull hitch@sha256:a170c2ed0b748dd1577b15d01083d7c771105d6214e4f4eaa26a680a1b5c1435
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36959804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bf5656aebd83bbb5e778983b0056f37825a1c5d1010dbdcf0f03fe7fb58b84e`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 05:02:29 GMT
ARG SRCVER=1.7.2
# Wed, 26 Jan 2022 05:02:31 GMT
ARG PKGVER=1
# Wed, 26 Jan 2022 05:02:34 GMT
ARG DISTVER=bullseye
# Wed, 26 Jan 2022 05:02:37 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 26 Jan 2022 05:02:40 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 26 Jan 2022 05:15:21 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 26 Jan 2022 05:15:23 GMT
WORKDIR /etc/hitch
# Wed, 26 Jan 2022 05:15:24 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 26 Jan 2022 05:15:25 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 26 Jan 2022 05:15:28 GMT
EXPOSE 443
# Wed, 26 Jan 2022 05:15:30 GMT
CMD []
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be06e4ac21c7236f81e3068fe1081f5b3d264aed0671701edfa96321f9a12144`  
		Last Modified: Wed, 26 Jan 2022 05:15:55 GMT  
		Size: 1.7 MB (1686356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802cf151013b2498d62e75a7a584bc049f24d2cfe75af481c26ced319b53a208`  
		Last Modified: Wed, 26 Jan 2022 05:15:55 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hitch:latest` - linux; s390x

```console
$ docker pull hitch@sha256:1ee6a1e2a94e7d21525c02f2f673801c1d34a7a4c4a8df50f0ee9a50117ed1f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31268094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:395ddd9120af6c3e3d3df60c87c4b4a6d6ccd3eac860c09d3485ef74d0b5a722`
-	Entrypoint: `["docker-hitch-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 03:08:28 GMT
ARG SRCVER=1.7.2
# Wed, 26 Jan 2022 03:08:29 GMT
ARG PKGVER=1
# Wed, 26 Jan 2022 03:08:29 GMT
ARG DISTVER=bullseye
# Wed, 26 Jan 2022 03:08:29 GMT
ARG PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794
# Wed, 26 Jan 2022 03:08:29 GMT
ARG SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf
# Wed, 26 Jan 2022 03:10:10 GMT
# ARGS: DISTVER=bullseye PKGCOMMIT=f12ab7958bc4885f3f00311cbca5103d9e6ba794 PKGVER=1 SHASUM=7b35b5f4a3b6dab2599643c0bc90880a77ea518a627b31813f45a7ee8c52982ba4ac07228b640a0bcf90ea7d63421b62884a091fed6664732585585e5ec15bcf SRCVER=1.7.2
RUN set -ex;     BASE_PKGS="apt-utils curl dirmngr dpkg-dev debhelper devscripts equivs fakeroot git gnupg pkg-config";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnish/pkg-hitch.git;     cd pkg-hitch;     git checkout ${PKGCOMMIT};     rm -rf .git;     curl -Lf https://hitch-tls.org/source/hitch-${SRCVER}.tar.gz -o $tmpdir/orig.tgz;     echo "${SHASUM}  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i         -e "s/@SRCVER@/${SRCVER}/g"         -e "s/@PKGVER@/${PKGVER:-1}/g"         -e "s/@DISTVER@/$DISTVER/g" debian/changelog;     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/hitch*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y purge --auto-remove hitch-build-deps $BASE_PKGS;     apt-get -y install ../*.deb;     sed -i 's/daemon = on/daemon = off/' /etc/hitch/hitch.conf;     rm -rf /var/lib/apt/lists/* "$tmpdir"
# Wed, 26 Jan 2022 03:10:11 GMT
WORKDIR /etc/hitch
# Wed, 26 Jan 2022 03:10:11 GMT
COPY file:1abf3c94dce5dc9f6617dc8d36a6fe6f4f7236189d4819f16cefb54288e80e0d in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:10:11 GMT
ENTRYPOINT ["docker-hitch-entrypoint"]
# Wed, 26 Jan 2022 03:10:11 GMT
EXPOSE 443
# Wed, 26 Jan 2022 03:10:11 GMT
CMD []
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6029eede8974aa9c95d06c9ec6910c58e0a7512828588c5cf1d05d8a3788b76c`  
		Last Modified: Wed, 26 Jan 2022 03:10:32 GMT  
		Size: 1.6 MB (1620607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7094371c5de9532eb34b6f0b0130bc79e2815103d1fb4df0a93ee7596b3bf0`  
		Last Modified: Wed, 26 Jan 2022 03:10:32 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
