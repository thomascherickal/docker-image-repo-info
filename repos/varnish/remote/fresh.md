## `varnish:fresh`

```console
$ docker pull varnish@sha256:95587ca949be166e5800bd26d6a03049b6d24b60bd52637f15b415543f892265
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
$ docker pull varnish@sha256:f7126e89d57e86b6bce04a92f7f19dc31a2a748d3d7ce9de9bb8c97ace8be88b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134702815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e16c250b81d4df0153d5a9919009c75e65c8a17222c67a2d303ea7513080bc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 04:55:40 GMT
ADD file:a1398394375faab8dd9e1e8d584eea96c750fb57ae4ffd2b14624f1cf263561b in / 
# Wed, 20 Sep 2023 04:55:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 16:47:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 10:00:13 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 10:00:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 10:00:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 10:00:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 10:00:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 10:00:13 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 10:00:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 10:00:13 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 10:00:13 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 10:00:13 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 10:03:01 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 10:03:02 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 10:03:02 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 10:03:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 10:03:02 GMT
USER varnish
# Thu, 21 Sep 2023 10:03:02 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 10:03:02 GMT
CMD []
```

-	Layers:
	-	`sha256:a803e7c4b030119420574a882a52b6431e160fceb7620f61b525d49bc2d58886`  
		Last Modified: Wed, 20 Sep 2023 05:00:22 GMT  
		Size: 29.1 MB (29124705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbeceee01016f5ec8f88dc9715bb72027b8220df91509be67422afd43ac848e0`  
		Last Modified: Thu, 21 Sep 2023 10:08:10 GMT  
		Size: 105.6 MB (105577617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e456fb3f0eb6ce3280e418a0c8c5dddf3945e384bf36dec41c1a93c740d39d`  
		Last Modified: Thu, 21 Sep 2023 10:07:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:2da39c82a15f27a7a9de2fd031646f2e7953eab02106f5381bb6e80fd4f4314b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105090520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37d20a8436d032abc7b52151c1a4416779498ff0b91a7f98dea7751e61b23a79`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:56b69c762bd03a9b00a1677740f7209aac08bac69a9e73563e326b9b0efbbfcc in / 
# Wed, 20 Sep 2023 04:57:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:02:48 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 20 Sep 2023 22:02:48 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 20 Sep 2023 22:02:48 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 20 Sep 2023 22:02:48 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 20 Sep 2023 22:02:49 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 20 Sep 2023 22:02:49 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 20 Sep 2023 22:02:49 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 20 Sep 2023 22:02:49 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 20 Sep 2023 22:02:49 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 20 Sep 2023 22:02:50 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 20 Sep 2023 22:02:50 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Sep 2023 22:07:24 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 20 Sep 2023 22:07:27 GMT
WORKDIR /etc/varnish
# Wed, 20 Sep 2023 22:07:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Sep 2023 22:07:28 GMT
USER varnish
# Wed, 20 Sep 2023 22:07:28 GMT
EXPOSE 80 8443
# Wed, 20 Sep 2023 22:07:28 GMT
CMD []
```

-	Layers:
	-	`sha256:e0b5206657a67707f4c57136f811162ce89a951fec109a406df7508d59e644cb`  
		Last Modified: Wed, 20 Sep 2023 05:01:16 GMT  
		Size: 24.8 MB (24805628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795a9d469998b5e1515034ddbc6778be003739d21287c7aa254d1a80225950e2`  
		Last Modified: Wed, 20 Sep 2023 22:17:34 GMT  
		Size: 80.3 MB (80284401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996bc55adc748abe1134e8a7ed3821d673682093e7e24d5f9d4cd446061415e0`  
		Last Modified: Wed, 20 Sep 2023 22:17:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:472bd27e1d4a42daf22c320d58944cf4ea8243a2a3dd9300e1cb7b76264bedda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129197485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6368c63db1f983c26740d4676cf9ae4da73811320dd0f21fabf6191e6e872ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:48:56 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:34:35 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:34:36 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:34:36 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 04:34:36 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:37:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:37:06 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:37:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:37:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:37:06 GMT
USER varnish
# Thu, 21 Sep 2023 04:37:06 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d168552ad41a2f9b1ae51e74b416a1fbf5f899631badf1ecf74bb5962f131c8`  
		Last Modified: Thu, 21 Sep 2023 04:41:26 GMT  
		Size: 100.0 MB (100039772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee0db284127fd79a1e633f9ee036d58c5817770e41d69607d88963d53c073f`  
		Last Modified: Thu, 21 Sep 2023 04:41:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:be746fcff281c5c08112526dbd7ed21d517c500310badbfa306a69a98fd07eff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131844351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b41347c8fa036834c6f786a45f0cf7715a3930add2236e3613e11bcf3ce23d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 00:41:55 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Wed, 20 Sep 2023 00:41:56 GMT
CMD ["bash"]
# Thu, 21 Sep 2023 02:26:12 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 02:26:13 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 02:26:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 02:26:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 02:26:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 02:26:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 02:26:13 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 02:26:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 02:26:13 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 02:26:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 02:26:14 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 02:29:57 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 02:29:59 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 02:29:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 02:29:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 02:30:00 GMT
USER varnish
# Thu, 21 Sep 2023 02:30:00 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 02:30:00 GMT
CMD []
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ca2e829b0ced5dd6f71272f8fb1e36413c9dbeac10c5cf6ff3051e96425b2d`  
		Last Modified: Thu, 21 Sep 2023 02:39:09 GMT  
		Size: 101.7 MB (101701965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a873a3ca6e4e41d4eb36a12f84f15c520a971a265c9bfdb7fe3d8c96c7b3a8c5`  
		Last Modified: Thu, 21 Sep 2023 02:38:46 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:eaf09088e570d715dad0da9638f931eae33ca9cade9fb50fe0a8ee10b2126fd5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137636377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:351079a888550d099a6fbf859adde1dc956a915f96a192f13d11d1e46a4f258f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 07:52:54 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Wed, 20 Sep 2023 07:52:55 GMT
CMD ["bash"]
# Thu, 21 Sep 2023 00:59:38 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 00:59:38 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 00:59:39 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 00:59:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 00:59:40 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 00:59:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 00:59:40 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 00:59:41 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 00:59:42 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 00:59:42 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 00:59:42 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:05:09 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:05:14 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:05:14 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:05:14 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:05:14 GMT
USER varnish
# Thu, 21 Sep 2023 01:05:15 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:05:15 GMT
CMD []
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15f2bfbd6986762d145cea8aab0e68de11fa2dca6e32e8948ee7660602eca7b`  
		Last Modified: Thu, 21 Sep 2023 01:18:30 GMT  
		Size: 104.5 MB (104516425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418b5b4602845154d19c9615cd53f47b9cd6cf591575773e17d4703076b1f5f1`  
		Last Modified: Thu, 21 Sep 2023 01:18:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:5f81cf37a0f9b434d334b4474f6b2a922dc3d69b44c10643d662f414379efb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112304312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2424b30794bc9a254976a88cff8128a0a08379f5469157ba1214a32035f1d308`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 20 Sep 2023 02:54:26 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Wed, 20 Sep 2023 02:54:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:30:23 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:46:39 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:46:39 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:46:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:46:40 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:46:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:46:40 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:46:40 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:46:40 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:46:40 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 21 Sep 2023 01:46:40 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:49:02 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:49:08 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:49:09 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:49:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:49:09 GMT
USER varnish
# Thu, 21 Sep 2023 01:49:09 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:49:09 GMT
CMD []
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f1746bb0fa60e741dc585b6692faff78b1be1b4bdeaccf1ef057b9ff37f514`  
		Last Modified: Thu, 21 Sep 2023 01:54:35 GMT  
		Size: 84.8 MB (84813856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dfde9b1881ef9dd08a3eed2b080f84d5b1f8c6e4fecc2b301c032e8a7d898f`  
		Last Modified: Thu, 21 Sep 2023 01:54:23 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
