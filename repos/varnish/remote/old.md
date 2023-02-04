## `varnish:old`

```console
$ docker pull varnish@sha256:080760c9ffa5468ecfecbef5f6cbda395602e67e3267eacfb90e811cf0ccda7c
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
$ docker pull varnish@sha256:60f5f29e9d01b76fe923c40561eba3059e0fc9aeffc377890d7918ac522377f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106522000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab33ae0ff23fb3178295cca2908b582bf4133e2244f1d18d12fcd36deea1e473`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:56:02 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Sat, 04 Feb 2023 13:56:03 GMT
ARG VARNISH_VERSION=7.1.2
# Sat, 04 Feb 2023 13:56:03 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Sat, 04 Feb 2023 13:56:03 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Sat, 04 Feb 2023 13:56:03 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Sat, 04 Feb 2023 13:56:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Sat, 04 Feb 2023 13:56:03 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Sat, 04 Feb 2023 13:56:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Sat, 04 Feb 2023 13:56:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 13:56:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 13:56:03 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 13:58:51 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 13:58:51 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 13:58:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 13:58:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 13:58:52 GMT
USER varnish
# Sat, 04 Feb 2023 13:58:52 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 13:58:52 GMT
CMD []
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cc497122d31e83a1ca41d15ad52969c579f1731d532a7c69ef46fec3654b71`  
		Last Modified: Sat, 04 Feb 2023 14:02:14 GMT  
		Size: 75.1 MB (75124588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364e3b6830d4c69ba22b0878f12873fb4af988625143b267a946421aec271e92`  
		Last Modified: Sat, 04 Feb 2023 14:02:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:af440494a9fa63f6e01ab2de90f7511757acffa9f5a6a3d99091307b05143f7d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.9 MB (82883084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30142de2126bc95650930d00a49e560bf838c6bd56af0c704f1b89dd7277be67`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 09:59:36 GMT
ADD file:c3cb8f4527fa96e99a4741ecb398113f25f53389c173b74f6c2a5e39a6575c60 in / 
# Sat, 04 Feb 2023 09:59:36 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 21:22:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_VERSION=7.1.2
# Sat, 04 Feb 2023 21:22:46 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Sat, 04 Feb 2023 21:22:46 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Sat, 04 Feb 2023 21:22:46 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 21:22:46 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 21:25:38 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 21:25:39 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 21:25:39 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 21:25:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 21:25:39 GMT
USER varnish
# Sat, 04 Feb 2023 21:25:39 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 21:25:39 GMT
CMD []
```

-	Layers:
	-	`sha256:bd25bcdfbaa165120ee21b6567df395fe7d7b38da3cca0bcecee55a190e04aab`  
		Last Modified: Sat, 04 Feb 2023 10:06:24 GMT  
		Size: 26.6 MB (26559474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a86cf7003c8f00c3a87657fb934e5c12a0414057288dcf7f8d1c94edb9d665`  
		Last Modified: Sat, 04 Feb 2023 21:29:54 GMT  
		Size: 56.3 MB (56323117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769df1d3e88475c39dda498ae716e7af2815967f933c5cede97335326f57ccaf`  
		Last Modified: Sat, 04 Feb 2023 21:29:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:2828b8fb4faf9a30d5629419058d4264fc9c3042a45fe2eb3968acad624055ea
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100536202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288a3f73b9ee52cdd3f6070aab6bdab815a4c28db9d0465024fc7b6b0072d466`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:01:29 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Sat, 04 Feb 2023 18:01:29 GMT
ARG VARNISH_VERSION=7.1.2
# Sat, 04 Feb 2023 18:01:29 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Sat, 04 Feb 2023 18:01:30 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Sat, 04 Feb 2023 18:01:30 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Sat, 04 Feb 2023 18:01:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Sat, 04 Feb 2023 18:01:30 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Sat, 04 Feb 2023 18:01:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Sat, 04 Feb 2023 18:01:30 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 18:01:30 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 18:01:30 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 18:03:49 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 18:03:50 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 18:03:50 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:03:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 18:03:50 GMT
USER varnish
# Sat, 04 Feb 2023 18:03:50 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 18:03:50 GMT
CMD []
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850cf6761bb822194024fd93c31661bc9833051a5bfb26eacacbe9712a9c4e9b`  
		Last Modified: Sat, 04 Feb 2023 18:06:37 GMT  
		Size: 70.5 MB (70490918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68def1a374fc8952929bd4cd04102d422fe4a196ccf5d9ee75035c969409b934`  
		Last Modified: Sat, 04 Feb 2023 18:06:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:f3128aed82c92308c61fcd6a5058bf223e447469ad7982ef36a32030d7b17e04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107895639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5411731225cec268dd8f1d1e88d59cc5550f24a90e515520d9432787e1625f73`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 08:02:01 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 21 Dec 2022 08:02:01 GMT
ARG VARNISH_VERSION=7.1.2
# Wed, 21 Dec 2022 08:02:02 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Wed, 21 Dec 2022 08:02:03 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 21 Dec 2022 08:02:04 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 21 Dec 2022 08:02:05 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 21 Dec 2022 08:02:06 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 21 Dec 2022 08:02:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 21 Dec 2022 08:02:08 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 21 Dec 2022 08:02:09 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 21 Dec 2022 08:02:10 GMT
ENV VARNISH_SIZE=100M
# Wed, 21 Dec 2022 08:04:52 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Wed, 21 Dec 2022 08:04:53 GMT
WORKDIR /etc/varnish
# Wed, 21 Dec 2022 08:04:55 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 21 Dec 2022 08:04:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 21 Dec 2022 08:04:56 GMT
USER varnish
# Wed, 21 Dec 2022 08:04:57 GMT
EXPOSE 80 8443
# Wed, 21 Dec 2022 08:04:58 GMT
CMD []
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a6719e637c4ec4aefa2383cce5a5a747ee78c9b1f49fee5a08f8e490115257`  
		Last Modified: Wed, 21 Dec 2022 08:06:25 GMT  
		Size: 75.5 MB (75519403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bdf1c8b0011cf5ddb24bc6c5d352c19d005732cb812082d01d31b8db446a9ee`  
		Last Modified: Wed, 21 Dec 2022 08:06:16 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:6c2ea1b8bf38943460059670a97377efaad9c58cf1f3405616878fd3ef11f678
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105799140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bbaba501a529255ee02e242f4ea81a45082ef2d89caeb9b1d92b4ce1be19e62`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:26:22 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Sat, 04 Feb 2023 17:26:22 GMT
ARG VARNISH_VERSION=7.1.2
# Sat, 04 Feb 2023 17:26:23 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Sat, 04 Feb 2023 17:26:23 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Sat, 04 Feb 2023 17:26:24 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Sat, 04 Feb 2023 17:26:24 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Sat, 04 Feb 2023 17:26:25 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Sat, 04 Feb 2023 17:26:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Sat, 04 Feb 2023 17:26:26 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Sat, 04 Feb 2023 17:26:27 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Sat, 04 Feb 2023 17:26:27 GMT
ENV VARNISH_SIZE=100M
# Sat, 04 Feb 2023 17:33:47 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Sat, 04 Feb 2023 17:33:50 GMT
WORKDIR /etc/varnish
# Sat, 04 Feb 2023 17:33:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:33:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 04 Feb 2023 17:33:51 GMT
USER varnish
# Sat, 04 Feb 2023 17:33:52 GMT
EXPOSE 80 8443
# Sat, 04 Feb 2023 17:33:52 GMT
CMD []
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fdaa1edd98c7a5836570e84c300ca9c5c0ec50e1979aed3bcd47e1a85aad64`  
		Last Modified: Sat, 04 Feb 2023 17:42:13 GMT  
		Size: 70.5 MB (70529852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7659d11ad3b36efb455266d0eb495522babcc17a7a8b174abd0d2df45d585fc`  
		Last Modified: Sat, 04 Feb 2023 17:41:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:e75e34fba93f3f32d106700d4e93c5c9707eb9eb32058da5f1328e8e4ad5d27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86833950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aebf2a458caabeda0bd00d1cba9bbc14c65034713a39b9385e47c504a9ac5036`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 10:26:01 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_VERSION=7.1.2
# Wed, 21 Dec 2022 10:26:02 GMT
ARG DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 21 Dec 2022 10:26:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Wed, 21 Dec 2022 10:26:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Wed, 21 Dec 2022 10:26:03 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Wed, 21 Dec 2022 10:26:03 GMT
ENV VMOD_DEPS=automake curl libtool make pkg-config python3-sphinx
# Wed, 21 Dec 2022 10:26:04 GMT
ENV VARNISH_SIZE=100M
# Tue, 10 Jan 2023 01:41:58 GMT
# ARGS: DIST_SHA512=e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.2 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS libgetdns10;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.2.tgz -o $tmpdir/orig.tgz;     echo "e16a4b75ede25f3812dfc4e95545e39a80022835b9155a4e42118f911e41b691cbedd296db48d307ba4a4d0d01df1149306d752de07cabe459ccbf5bcdd49238  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 10 Jan 2023 01:42:07 GMT
WORKDIR /etc/varnish
# Tue, 10 Jan 2023 01:42:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 10 Jan 2023 01:42:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 10 Jan 2023 01:42:08 GMT
USER varnish
# Tue, 10 Jan 2023 01:42:09 GMT
EXPOSE 80 8443
# Tue, 10 Jan 2023 01:42:09 GMT
CMD []
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d4c9c347e9b7f6ec4e2913f77427f763121ee4c5c1581c98442b5f1196eaa1`  
		Last Modified: Tue, 10 Jan 2023 01:43:26 GMT  
		Size: 57.2 MB (57203697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44b8332de2d27a2172b14f1b3da08d4945e94d884acb16dc735410d206be275`  
		Last Modified: Tue, 10 Jan 2023 01:43:18 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
