## `varnish:latest`

```console
$ docker pull varnish@sha256:ead8e23c66e136f77ed25400326b3f905c83c73be864b3f88c619e5bd451be26
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
$ docker pull varnish@sha256:cf54fc50292fee9f265cc1c57359b8ada5d0a967c598addce38ec26c80f1a492
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.4 MB (105405532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2cf1c716f312cd4a14537f5b761028b5cab1da092ece6371ca2156fb594b2c5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 01:20:04 GMT
ADD file:0eae0dca665c7044bf242cb1fc92cb8ea744f5af2dd376a558c90bc47349aefe in / 
# Tue, 02 Aug 2022 01:20:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:36:01 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:21:22 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:21:23 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:21:23 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:21:23 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:21:23 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:21:23 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:21:23 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:21:23 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:21:23 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Thu, 11 Aug 2022 18:21:23 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:24:23 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:24:24 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 18:24:24 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 18:24:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 18:24:24 GMT
USER varnish
# Thu, 11 Aug 2022 18:24:24 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 18:24:24 GMT
CMD []
```

-	Layers:
	-	`sha256:1efc276f4ff952c055dea726cfc96ec6a4fdb8b62d9eed816bd2b788f2860ad7`  
		Last Modified: Tue, 02 Aug 2022 01:24:13 GMT  
		Size: 31.4 MB (31366757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ff6694216a1c2c343b0daee3379ce5cc49dfebf83c5d20c7b37a18e255863b`  
		Last Modified: Thu, 11 Aug 2022 18:29:35 GMT  
		Size: 74.0 MB (74038302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55970dadf2c559f45d07b27b76a01ba931610aa67339c6dd9b66fc2dc11b20b`  
		Last Modified: Thu, 11 Aug 2022 18:29:25 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:13ce65c5cf7a1c0893115040852a90185fabfb06ea3709b75a52c1775caa7110
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81982133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a27f980b875e490a32c93863c0a98996463667a81e18f9ba099c8fd616498d55`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:58:59 GMT
ADD file:1575b776a15adacebc0875642e97a80807d42dcfc8917e1406d47af7ac244c97 in / 
# Tue, 02 Aug 2022 00:58:59 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 12:09:49 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:57:41 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:57:41 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:57:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:57:41 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:57:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:57:41 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:57:41 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:57:41 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:57:41 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Thu, 11 Aug 2022 17:57:42 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:01:06 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:01:06 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 18:01:06 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 18:01:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 18:01:06 GMT
USER varnish
# Thu, 11 Aug 2022 18:01:06 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 18:01:06 GMT
CMD []
```

-	Layers:
	-	`sha256:1dd75a3a9c893a7dc313f683dd62464b7eab6c6d522ee62c8a17022631830f32`  
		Last Modified: Tue, 02 Aug 2022 01:06:45 GMT  
		Size: 26.6 MB (26560586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8814e7f5201bf113474c4aad9e2f0cd6038545f35ef2f1a4282fc661d88cb2c`  
		Last Modified: Thu, 11 Aug 2022 18:07:57 GMT  
		Size: 55.4 MB (55421074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d04f2a9542eef35fc493beda105f15efb25bd4efb5dad903ee26a21c55cc515`  
		Last Modified: Thu, 11 Aug 2022 18:07:49 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:54bd2b74433e5afda4c255b24978228e11301ddcd6e95e995d09d2dd5c935591
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99501274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60cb80d70d69174ee6c00de66ba6aa1f7746e1b9126925888bf012977c96fddd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:25:36 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:48:39 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:48:39 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:48:40 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:48:41 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:48:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:48:43 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:48:44 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:48:45 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:48:46 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Thu, 11 Aug 2022 17:48:47 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:51:40 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:51:41 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:51:43 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:51:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:51:44 GMT
USER varnish
# Thu, 11 Aug 2022 17:51:45 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:51:46 GMT
CMD []
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3567de70d7dd5161d1872eaca7bbec2d6c26fec59cabf29c5423206713199d88`  
		Last Modified: Thu, 11 Aug 2022 17:57:57 GMT  
		Size: 69.4 MB (69446497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1acd3a87ea41e1cd943ad5ccc0ad930d74b6de9189bcfefebc3627f6ba340c7`  
		Last Modified: Thu, 11 Aug 2022 17:57:48 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:0f860445730367a56c84ed8d31f01395a650c5e399f8243cb272406f249f11fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.8 MB (106763269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87998c911befcf7fcaaef1e1f40a9fd400863fa479d762e521c0b691507bde29`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:39:20 GMT
ADD file:f771e2286465694126158821089d801c7296376be2a56189e6041a15d2fe79f5 in / 
# Tue, 02 Aug 2022 00:39:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:46:33 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:38:59 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:39:00 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:39:01 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:39:02 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:39:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:39:04 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:39:05 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:39:06 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:39:07 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Thu, 11 Aug 2022 17:39:08 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:42:00 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:42:00 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:42:02 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:42:02 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:42:03 GMT
USER varnish
# Thu, 11 Aug 2022 17:42:04 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:42:05 GMT
CMD []
```

-	Layers:
	-	`sha256:90eb7f0ce9f33cf5dcd67d54c2fa606186dbaa5f95b6046f36145097267f9e53`  
		Last Modified: Tue, 02 Aug 2022 00:45:14 GMT  
		Size: 32.4 MB (32374054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a15707c9f10299a4a0e7c621a1ac19446c6a2546d265bf40c355c270b13045`  
		Last Modified: Thu, 11 Aug 2022 17:48:14 GMT  
		Size: 74.4 MB (74388741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06165a4347c0ddc22956f0d8e014d4e45d3c04bed355fa60e790155835d85a9`  
		Last Modified: Thu, 11 Aug 2022 17:48:03 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:0f995563650da9ac00d4daab0368d9947941c17cf9219ca993ef951338a12ac4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104600534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21d71351f046f7e428422ce19ecf6cd435e0c5b8fe787d357233072e9f09e953`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 01:30:56 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:17:15 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:17:15 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:17:15 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:17:16 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:17:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:17:17 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:17:17 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:17:17 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:17:18 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Thu, 11 Aug 2022 18:17:18 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:24:29 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:24:31 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 18:24:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 18:24:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 18:24:32 GMT
USER varnish
# Thu, 11 Aug 2022 18:24:33 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 18:24:33 GMT
CMD []
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ff6de86f40607bb0874124b91436931821a4a48c30c7314ad58563d5c0219c`  
		Last Modified: Thu, 11 Aug 2022 18:35:18 GMT  
		Size: 69.3 MB (69327288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58c81ff29d53db209f958d7ddd92d0e2fc01ea85e0225defec1a45b44634a22`  
		Last Modified: Thu, 11 Aug 2022 18:35:01 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:bd5a9ed4da590f47636064ccb2a860886ec08f1ef5234acbbe001b04622f0ca1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85821040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff0859b34e8443e23c71824006f8492c32e566228a2176a75b40eb260fb16811`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 02 Aug 2022 00:42:27 GMT
ADD file:c2afc8990930846fbe7c99bfdfe9ea562c75feb6e3c9122431f7c9f8b5e51a7f in / 
# Tue, 02 Aug 2022 00:42:29 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 11:37:45 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:42:44 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:42:45 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:42:45 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:42:46 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:42:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:42:47 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:42:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:42:48 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:42:48 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkg-config python3-sphinx
# Thu, 11 Aug 2022 17:42:49 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:46:18 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot sbuild";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y $BASE_PKGS;     cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 3ba24a8eee8cc5c082714034145b907402bbdb83;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.1.1.tgz -o $tmpdir/orig.tgz;     echo "7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:46:24 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:46:24 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:46:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:46:25 GMT
USER varnish
# Thu, 11 Aug 2022 17:46:25 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:46:25 GMT
CMD []
```

-	Layers:
	-	`sha256:026d311d0716db60eba0572ea784c21031f420960510cebcc383dc53949b4db8`  
		Last Modified: Tue, 02 Aug 2022 00:48:01 GMT  
		Size: 29.6 MB (29640259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b216b7c3600c2cf97cda6bd08251e0d3f64ebbfffc35d3d582ab183c40793853`  
		Last Modified: Thu, 11 Aug 2022 17:56:36 GMT  
		Size: 56.2 MB (56180307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d5c8ba66fb73ece0cdb666d6f2a0a6636b77e1ad01cceb090eadd8ebe6adf`  
		Last Modified: Thu, 11 Aug 2022 17:56:29 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
