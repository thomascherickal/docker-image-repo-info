## `varnish:old`

```console
$ docker pull varnish@sha256:28b9207d49c4e302fc86546b7d45ea4d9e6b5422cc77cb49f51be275d864b039
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
$ docker pull varnish@sha256:dfb97568859cbd5e3b745a67668df23a1ceca18eb292218d9871d52954805d99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106849839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e192e3d65e5429e6f2a7f23281c3cf04d43217560b3c01e47dd8654ab470e545`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:39:16 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:39:16 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:39:16 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:39:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:39:17 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:39:17 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:41:53 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:41:54 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:41:54 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:41:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:41:54 GMT
USER varnish
# Wed, 12 Apr 2023 07:41:54 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:41:54 GMT
CMD []
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c968e0ee4a730130252480debde7124ca86d34f741bf51571a5a29a5ba34693c`  
		Last Modified: Wed, 12 Apr 2023 07:45:05 GMT  
		Size: 75.4 MB (75431120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25daa5e6ca914814a8155ca526ce4bb0b71741603e1898c2e87ec69bd20c5ab0`  
		Last Modified: Wed, 12 Apr 2023 07:44:55 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c244a05033959bcfd06dad6e9bb4c15405ca97412a35d196aa7288a8d0b98865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83190520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f4f1a4a71ea168baeb1694ae369389fda214c037ea35ff0165991f0abe556d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 09:52:54 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 09:52:54 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 09:52:54 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 09:52:55 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 09:52:55 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 09:52:55 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 09:55:29 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 09:55:29 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 09:55:29 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 09:55:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 09:55:29 GMT
USER varnish
# Wed, 12 Apr 2023 09:55:29 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 09:55:29 GMT
CMD []
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c3bf9e9ab14cb00f2a7b32fd61f0dc7f58385c6b36746b7a28d8db143af093`  
		Last Modified: Wed, 12 Apr 2023 09:58:19 GMT  
		Size: 56.6 MB (56610256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3f12a5b2f13f28364d239561b484e09aab0533fa4291c2ec7c6fb72ae6dbe3`  
		Last Modified: Wed, 12 Apr 2023 09:58:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c7c5b44d1b649b8e18f2fa02e3ac6cfbe1219629ee51fb0c297f2ad9d340835c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100869468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064d1446bbe323f8a5118936bc056bec5669a4efea357a44b0250aefebce979f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:48:37 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:48:38 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:48:38 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:48:38 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:48:38 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:50:57 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:50:57 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:50:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:50:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:50:58 GMT
USER varnish
# Wed, 12 Apr 2023 04:50:58 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:50:58 GMT
CMD []
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd387399b52bcda6a293afa412dc3c7ffe5106e36f6820bbfe7b36cfe9c84ce6`  
		Last Modified: Wed, 12 Apr 2023 04:53:31 GMT  
		Size: 70.8 MB (70805151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717900fa7e49b8851eb8e3cc5cb7174be8ba02fa5fae4efc1d5889369dc19982`  
		Last Modified: Wed, 12 Apr 2023 04:53:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:132d16358cb9c81ea691480e6340bafa5db22839213c2608eb00bb1c2e318778
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108229812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:701dd3cc6e511fd1e6a0ccb05404b60373851c1f0318dd8035b6526b81707c28`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:18:22 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 04:18:22 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 04:18:22 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 04:18:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 04:18:23 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 04:18:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 04:21:46 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 04:21:46 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 04:21:47 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 04:21:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 04:21:47 GMT
USER varnish
# Wed, 12 Apr 2023 04:21:47 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 04:21:47 GMT
CMD []
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a639361d9918a14ff82f7bba72feea5809b05f1c6a1c6da01ac194a148379e2`  
		Last Modified: Wed, 12 Apr 2023 04:25:29 GMT  
		Size: 75.8 MB (75830396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95964f0144157e5774aa830935fc68f7bf5b0a1834e27bc6272d49816484fda`  
		Last Modified: Wed, 12 Apr 2023 04:25:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:2ddbd11558d86d08b3f82a25da574d70734fed468550edb4d6b957cf2fc4ff55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106112382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fcc671da9acaf8ae312a5ba85fd3d77e7e1b88a900054ac23433f6dad4b7cde`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:55:40 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 00:55:40 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 00:55:41 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 00:55:41 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 00:55:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 00:55:43 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 00:55:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 00:55:44 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 00:55:45 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 01:06:37 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 01:06:41 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 01:06:41 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 01:06:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 01:06:43 GMT
USER varnish
# Wed, 12 Apr 2023 01:06:43 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 01:06:45 GMT
CMD []
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4a89d7f741d3117b0ee6c2f7194da63a2eb7e31a212514121c21a0f9a2d56d`  
		Last Modified: Wed, 12 Apr 2023 01:18:03 GMT  
		Size: 70.8 MB (70819898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3fec9bc4ead77e694d7ee941f4809ba1dc75a4379c2e14982a287a907f61d2`  
		Last Modified: Wed, 12 Apr 2023 01:17:46 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:8e03fc4febcb1085c13e0d907ca56a70bd0a5015b6001b7575deddb067700889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87145481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5308c0a1d01c5120da7ddc51e7161062bf73b4fe635935570d47dce15b4888`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 07:47:32 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_VERSION=7.2.1
# Wed, 12 Apr 2023 07:47:32 GMT
ARG DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Wed, 12 Apr 2023 07:47:32 GMT
ARG VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47
# Wed, 12 Apr 2023 07:47:33 GMT
ARG VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a
# Wed, 12 Apr 2023 07:47:33 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 12 Apr 2023 07:47:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 12 Apr 2023 07:50:04 GMT
# ARGS: DIST_SHA512=7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.1 VMOD_DYNAMIC_COMMIT=5c702fa6c3a88882a2678f75161692762e7d6c47 VMOD_DYNAMIC_SHA512SUM=3503ae09bae731213d5a6823af9fb758bcbcaf06678a2a0efc0b35d9f1b18ab46e02f02b75db8a4858bb2b623e76ea253e65ef2ae3ab076558b52b414996d33a VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout ffc59a345217b599fd49f7f0442b5f653fbe6fc2;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.2.1.tgz -o $tmpdir/orig.tgz;     echo "7b9b837a8bafdf5798e81bc38163457b3bca16d933a9492800cdd2cde35c9b524a10b7e5ec931217e11d72f32feb05157a7eecfd9cf2c5856e717b634e51d089  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 12 Apr 2023 07:50:08 GMT
WORKDIR /etc/varnish
# Wed, 12 Apr 2023 07:50:08 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 12 Apr 2023 07:50:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 12 Apr 2023 07:50:08 GMT
USER varnish
# Wed, 12 Apr 2023 07:50:08 GMT
EXPOSE 80 8443
# Wed, 12 Apr 2023 07:50:08 GMT
CMD []
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6c0378159be2b47ba02173837a0605e110437dd56ebde55c1b33b16e3a64c1`  
		Last Modified: Wed, 12 Apr 2023 07:53:06 GMT  
		Size: 57.5 MB (57491834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b0aa3c751db4a00420dc9624ea76c92014f9ff8e7975d01d47e5bf3743531c`  
		Last Modified: Wed, 12 Apr 2023 07:52:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
