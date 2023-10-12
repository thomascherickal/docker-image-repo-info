## `varnish:fresh`

```console
$ docker pull varnish@sha256:65558bcd9d1b82306a711269f8061246e7913666701bac39164c2a79d290368a
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
$ docker pull varnish@sha256:e03566ef6752192c478b1aa7bba603dc26f1ee563934c03f28e9c6a7a5396d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134737591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:266771d9cf5c42149096e6813c1b152608a114703951e87c69ce3220c862ab70`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 21:27:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 21:27:13 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 21:27:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 21:27:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 21:27:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 21:27:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 21:30:00 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 21:30:01 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 21:30:01 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:30:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 21:30:01 GMT
USER varnish
# Wed, 11 Oct 2023 21:30:01 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 21:30:01 GMT
CMD []
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73d3b02baeacb05096f1d533167545798575b4b39a4f516a201ad8a3c0fd9e0`  
		Last Modified: Wed, 11 Oct 2023 21:35:14 GMT  
		Size: 105.6 MB (105587228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c88afe6700045cede25a79c7cae3b4fd9c2630ea13c3445c62ee292dc732123`  
		Last Modified: Wed, 11 Oct 2023 21:34:59 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:1feecff1374e6c3d603761b67362c81d8a15190b4fce34911d6257281a848cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105036990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cb20c34e8cd2ad07e5e4d7fb9e378a81db336a803bd894fda058508b99013f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:22 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 11 Oct 2023 18:09:22 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 11 Oct 2023 18:09:22 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 11 Oct 2023 18:09:22 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Wed, 11 Oct 2023 18:09:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 11 Oct 2023 18:12:11 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 11 Oct 2023 18:12:12 GMT
WORKDIR /etc/varnish
# Wed, 11 Oct 2023 18:12:12 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 11 Oct 2023 18:12:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 11 Oct 2023 18:12:12 GMT
USER varnish
# Wed, 11 Oct 2023 18:12:12 GMT
EXPOSE 80 8443
# Wed, 11 Oct 2023 18:12:12 GMT
CMD []
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3d75364756f4e459e71b5941b35371acb082f8bb2f09c42230d48ff70cfa56`  
		Last Modified: Wed, 11 Oct 2023 18:17:46 GMT  
		Size: 80.3 MB (80287576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd120edc727486131696ee7b8fb97154d80d4812e8c1865198e8b909d2e8e457`  
		Last Modified: Wed, 11 Oct 2023 18:17:34 GMT  
		Size: 489.0 B  
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
$ docker pull varnish@sha256:b0b281bd04e70c06c4d95562ddc165603c7fcb63797a5307ea577d0854a46ba0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131877976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8763c9a49d7d742b60afd31d81ea0e3816bba8e58111f0d3bfc26b36fc3c66f5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:38:19 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 08:38:19 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 08:38:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 08:38:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 08:38:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 08:42:04 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 08:42:05 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 08:42:05 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 08:42:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 08:42:06 GMT
USER varnish
# Thu, 12 Oct 2023 08:42:06 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 08:42:06 GMT
CMD []
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d7224a6538ed66733bc96ac79177a58d0039e0e68594173cc295e2ea9b504`  
		Last Modified: Thu, 12 Oct 2023 08:48:35 GMT  
		Size: 101.7 MB (101713366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621ed1744001a5b482de115c1a397507d44f792c45cdd41dce56ecb1fca9cbe3`  
		Last Modified: Thu, 12 Oct 2023 08:48:15 GMT  
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
$ docker pull varnish@sha256:c16359d33b507ad0702a5be497bc4d3bf1dc9550a6b72a01fbfef0d10a15d9e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112330094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8caa54cdeafd2ed33943de55ef8effd990147fcb9b0311032a90892878efb1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 11 Oct 2023 17:50:28 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Wed, 11 Oct 2023 17:50:30 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:48:18 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 12 Oct 2023 00:48:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 12 Oct 2023 00:48:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 12 Oct 2023 00:48:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 12 Oct 2023 00:48:19 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Thu, 12 Oct 2023 00:48:19 GMT
ENV VARNISH_SIZE=100M
# Thu, 12 Oct 2023 01:06:58 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.1.tgz -o $tmpdir/orig.tgz;     echo "d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 12 Oct 2023 01:07:08 GMT
WORKDIR /etc/varnish
# Thu, 12 Oct 2023 01:07:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 12 Oct 2023 01:07:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 12 Oct 2023 01:07:08 GMT
USER varnish
# Thu, 12 Oct 2023 01:07:09 GMT
EXPOSE 80 8443
# Thu, 12 Oct 2023 01:07:09 GMT
CMD []
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1ecabb8eb208085a0cd1ccad185b3741ef91253ac090a644273393b03d5ba9`  
		Last Modified: Thu, 12 Oct 2023 01:15:40 GMT  
		Size: 84.8 MB (84816753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8069a9787fb8bc5a96e8c2c9afaa0c689c46501adc3724923dd883a96e1fd7`  
		Last Modified: Thu, 12 Oct 2023 01:15:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
