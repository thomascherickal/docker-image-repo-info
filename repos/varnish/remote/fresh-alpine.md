## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:be6e04ca4bf1559966ab8a5624c8d65ac4d88854f2e8c2bc5992baa9e767de28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:fresh-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:76322eef28985ba43144e7681a691b10d0fb6d65ca6276ee2aa9fe1503728fac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61971006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba2cd2d3038a9106bcb02208154cc5baf5e4244fe147edaf5e87e1ecbe6d71b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:48:52 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 11:48:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 11:48:53 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 11:48:53 GMT
ENV VARNISH_SIZE=100M
# Tue, 29 Mar 2022 11:50:29 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Tue, 29 Mar 2022 11:50:30 GMT
WORKDIR /etc/varnish
# Tue, 29 Mar 2022 11:50:30 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Tue, 29 Mar 2022 11:50:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 29 Mar 2022 11:50:30 GMT
USER varnish
# Tue, 29 Mar 2022 11:50:30 GMT
EXPOSE 80 8443
# Tue, 29 Mar 2022 11:50:30 GMT
CMD []
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ecdbed9207316489cc108f638bbbd586717bf5c312bec86eb2806b5c430ef4`  
		Last Modified: Tue, 29 Mar 2022 11:57:20 GMT  
		Size: 59.2 MB (59156014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b2e8a1615c6c3fe377f7e38a02e6fe7336e7935f3f62e8feff8036e1fef010`  
		Last Modified: Tue, 29 Mar 2022 11:57:11 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:258e483055d732875c4e80f2496752ba7bf96b551c14a260078323055798d6c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47681592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f902231317ec2f4fc2e9fcbbe13dbfc8f5df233282599579bb51a933652019`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 04:55:17 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 30 Mar 2022 04:55:17 GMT
ARG VARNISH_VERSION=7.1.0
# Wed, 30 Mar 2022 04:55:18 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Wed, 30 Mar 2022 04:55:18 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 30 Mar 2022 04:55:19 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 30 Mar 2022 04:55:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 30 Mar 2022 04:55:19 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Wed, 30 Mar 2022 04:55:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Wed, 30 Mar 2022 04:55:20 GMT
ENV VARNISH_SIZE=100M
# Wed, 30 Mar 2022 04:57:43 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" install;     make -j"$(nproc)" check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 30 Mar 2022 04:57:44 GMT
WORKDIR /etc/varnish
# Wed, 30 Mar 2022 04:57:44 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 30 Mar 2022 04:57:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 30 Mar 2022 04:57:45 GMT
USER varnish
# Wed, 30 Mar 2022 04:57:45 GMT
EXPOSE 80 8443
# Wed, 30 Mar 2022 04:57:46 GMT
CMD []
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32178ceca453e13d81eeff6d402cf27f51122d75f4f7a97b68b2aa9b3f9a8ff7`  
		Last Modified: Wed, 30 Mar 2022 05:09:05 GMT  
		Size: 45.3 MB (45256809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b79c662c4dc07258a372d4e6761abbab07b462703bc6a5b26c466971fb252f`  
		Last Modified: Wed, 30 Mar 2022 05:08:40 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:58cbdde15d49de4a3b402b2fe820ec4d216edefe6e969c990159adde9bbc8c8b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51098682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4989798a731407027a62e9a41f0855279d2354494c1c11252b56c7d8a599ab85`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:46 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:12:32 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:12:32 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:12:34 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:12:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:12:35 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:12:36 GMT
CMD []
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add42a09981f9b64e2b6df10282b0ad8f29f4af959845ba7eb7c95600d99e3b`  
		Last Modified: Thu, 17 Mar 2022 21:19:41 GMT  
		Size: 48.4 MB (48382315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f14629a9a8f57f9d018ae785cecd4382a7917633bae00050f0d52e71add30b0`  
		Last Modified: Thu, 17 Mar 2022 21:19:33 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:d0549983211a082fa2d02ae13f4bcca81fdf22c5a6fab8090cba75609c749380
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.4 MB (100448722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880734c6405cf1e397cc5a52b1d287c72787704c1f920172c1413aeab89e215d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:49:32 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Tue, 29 Mar 2022 10:49:33 GMT
ARG VARNISH_VERSION=7.1.0
# Tue, 29 Mar 2022 10:49:34 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Tue, 29 Mar 2022 10:49:35 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Tue, 29 Mar 2022 10:49:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Tue, 29 Mar 2022 10:49:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Tue, 29 Mar 2022 10:49:38 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Tue, 29 Mar 2022 10:49:39 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Tue, 29 Mar 2022 10:49:40 GMT
ENV VARNISH_SIZE=100M
# Wed, 30 Mar 2022 18:12:55 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" VERBOSE=1 install;     make -j"$(nproc)" VERBOSE=1 check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     sed -i '14 a AC_CHECK_HEADERS([stdatomic.h])' configure.ac;     git clone https://github.com/varnishcache/varnish-cache.git;     cd varnish-cache;     git checkout d48636d23bb277ca8650a6174c872d74080f2859;     cp include/vmb.h ../src/vmb.h;     cd /work/vmod-dynamic;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" VERBOSE=1 install;     make -j"$(nproc)" VERBOSE=1 check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 30 Mar 2022 18:12:56 GMT
WORKDIR /etc/varnish
# Wed, 30 Mar 2022 18:12:57 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 30 Mar 2022 18:12:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 30 Mar 2022 18:12:58 GMT
USER varnish
# Wed, 30 Mar 2022 18:12:59 GMT
EXPOSE 80 8443
# Wed, 30 Mar 2022 18:13:00 GMT
CMD []
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772a591518e56f64627b88720f43754b4c6badbee1e66a9241ff0c2578d232ce`  
		Last Modified: Wed, 30 Mar 2022 18:17:22 GMT  
		Size: 97.6 MB (97629316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f87aa9a385193fe112cec9d06c38ff4db516948e07973eb062686c9070badb6`  
		Last Modified: Wed, 30 Mar 2022 18:17:13 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:2b5a806ea2ade1ea0d76aa0ad7d8ef7c61ae2955e2e9549d7d1972a84eb9e668
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48202141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:529c13f3efcc65dfb1b3ac5697e031c0fefd156f6649062d5289cd9690594762`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:18:43 GMT
ADD file:bf9c99d8209e0bed9fd3b62cbe691ebf3829d5a35e63e2b066f1f842577a6d24 in / 
# Thu, 17 Mar 2022 18:18:48 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 12:09:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 12:10:26 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Fri, 18 Mar 2022 12:10:30 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 12:10:31 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:10:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 12:10:36 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 12:10:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8b7e8363a93630a772b70e3cf72231f43c62addae0ee8e507c61d43e3781c4e7`  
		Last Modified: Thu, 17 Mar 2022 18:20:01 GMT  
		Size: 2.8 MB (2817281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e94cc2aebd9efa44a159f8edfec552af073cbcaf430e29039e344a7af24312`  
		Last Modified: Fri, 18 Mar 2022 12:16:51 GMT  
		Size: 45.4 MB (45384380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26079fd90524de774229d65b85187547d85ba3f7e836d042a8b615469573bcac`  
		Last Modified: Fri, 18 Mar 2022 12:16:43 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:1373aa8f7d593720c308e24e7b549ea1ff90572ebbfcf2490e3b3e1b929e1f18
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.6 MB (88555183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9558fa096c01efbf3a85e42270414355350cc75f303a34731c91a1c12e54d3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Wed, 30 Mar 2022 00:51:10 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Wed, 30 Mar 2022 00:51:10 GMT
ARG VARNISH_VERSION=7.1.0
# Wed, 30 Mar 2022 00:51:10 GMT
ARG DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73
# Wed, 30 Mar 2022 00:51:10 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Wed, 30 Mar 2022 00:51:10 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Wed, 30 Mar 2022 00:51:10 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Wed, 30 Mar 2022 00:51:10 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Wed, 30 Mar 2022 00:51:10 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Wed, 30 Mar 2022 00:51:10 GMT
ENV VARNISH_SIZE=100M
# Wed, 30 Mar 2022 21:00:08 GMT
# ARGS: DIST_SHA512=ad9ce0cdc759976fcb7044914d28863edd197167f583fab2d1bc57f4e5b86c224b7c948faf1f7364a2a16bde9c415375d011462bdc43026c5f7a60e65bd21f73 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;          mkdir -p /work/varnish-modules;     cd /work/varnish-modules;     curl -fLo src.tar.gz https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz;     echo "$VARNISH_MODULES_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" VERBOSE=1 install;     make -j"$(nproc)" VERBOSE=1 check;         mkdir /work/vmod-dynamic;     cd /work/vmod-dynamic;     curl -fLo src.tar.gz https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz;     echo "$VMOD_DYNAMIC_SHA512SUM  src.tar.gz" | sha512sum -c -;     tar xavf src.tar.gz --strip 1;     sed -i '14 a AC_CHECK_HEADERS([stdatomic.h])' configure.ac;     git clone https://github.com/varnishcache/varnish-cache.git;     cd varnish-cache;     git checkout d48636d23bb277ca8650a6174c872d74080f2859;     cp include/vmb.h ../src/vmb.h;     cd /work/vmod-dynamic;     ./autogen.sh;     ./configure --libdir=/usr/lib;     make -j"$(nproc)" VERBOSE=1 install;     make -j"$(nproc)" VERBOSE=1 check;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 30 Mar 2022 21:00:11 GMT
WORKDIR /etc/varnish
# Wed, 30 Mar 2022 21:00:11 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 30 Mar 2022 21:00:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 30 Mar 2022 21:00:11 GMT
USER varnish
# Wed, 30 Mar 2022 21:00:11 GMT
EXPOSE 80 8443
# Wed, 30 Mar 2022 21:00:11 GMT
CMD []
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79050f712b7ad3912b907796002aaa15b7e6a37617f79ddc4b6036de665bbc6`  
		Last Modified: Wed, 30 Mar 2022 21:01:46 GMT  
		Size: 86.0 MB (85954265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251dc011711c00be01b39b29dfa6c5d6032c9706934c684c443ec34eee444a91`  
		Last Modified: Wed, 30 Mar 2022 21:01:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
