## `varnish:alpine`

```console
$ docker pull varnish@sha256:dcd3277b2d86f6dd8d3b4c6ff669cd2acf2213face6c246946a71343b4479975
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:alpine` - linux; amd64

```console
$ docker pull varnish@sha256:9686f648ae4a7d9b55bbdc18ab7b9e0a2023d56287a1824f4a04ad8c86a05b3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59492316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418a18ffd20fa7d1a34c6f276773995e5e6ef847bf0ae129f338cbac5863f91e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:25:17 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 18 Sep 2023 19:25:17 GMT
ARG VARNISH_VERSION=7.4.0
# Mon, 18 Sep 2023 19:25:17 GMT
ARG DIST_SHA512=b707348e9e6b7b9a89159a5aaeffaca8a1783623b64c4cc3e719fbb40af8f962610eeb280a5a062af244e231c6e83d290d95e737f56927ffcc5dd0ee1dea5f92
# Mon, 18 Sep 2023 19:25:17 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 18 Sep 2023 19:25:17 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 18 Sep 2023 19:25:17 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 18 Sep 2023 19:25:18 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 18 Sep 2023 19:25:18 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 18 Sep 2023 19:25:18 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 18 Sep 2023 19:25:18 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 18 Sep 2023 19:25:18 GMT
ENV VARNISH_SIZE=100M
# Mon, 18 Sep 2023 19:26:40 GMT
# ARGS: DIST_SHA512=b707348e9e6b7b9a89159a5aaeffaca8a1783623b64c4cc3e719fbb40af8f962610eeb280a5a062af244e231c6e83d290d95e737f56927ffcc5dd0ee1dea5f92 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.0 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 18 Sep 2023 19:26:40 GMT
WORKDIR /etc/varnish
# Mon, 18 Sep 2023 19:26:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 18 Sep 2023 19:26:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 18 Sep 2023 19:26:40 GMT
USER varnish
# Mon, 18 Sep 2023 19:26:40 GMT
EXPOSE 80 8443
# Mon, 18 Sep 2023 19:26:40 GMT
CMD []
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c88ae053c0e1d4bca8233126e418f097c5718ec7811e28b180146413982a8d8`  
		Last Modified: Mon, 18 Sep 2023 19:32:03 GMT  
		Size: 56.7 MB (56665811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110d91a20efaa6db7588d88efad713f7c3d309e833b48bd6e7fbfffa500f151d`  
		Last Modified: Mon, 18 Sep 2023 19:31:56 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:53f9b3af759587518f192eec1f3c70599bcea9f9eda6a87fbf32ba90f3fec2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45251077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9c94e956b808d696f8ad9a59e811e54a348f0230eba580630885aaee1ca603`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:57:37 GMT
ADD file:842dfa6e14e0537b53781830cfb26da9fa7a63229a7a1decc0fe08d8c000b5a9 in / 
# Mon, 07 Aug 2023 19:57:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:16:10 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_VERSION=7.4.1
# Wed, 20 Sep 2023 22:07:41 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Wed, 20 Sep 2023 22:07:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Wed, 20 Sep 2023 22:07:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Wed, 20 Sep 2023 22:07:42 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Wed, 20 Sep 2023 22:07:42 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Wed, 20 Sep 2023 22:07:43 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Sep 2023 22:10:33 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Wed, 20 Sep 2023 22:10:34 GMT
WORKDIR /etc/varnish
# Wed, 20 Sep 2023 22:10:34 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:10:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Sep 2023 22:10:34 GMT
USER varnish
# Wed, 20 Sep 2023 22:10:35 GMT
EXPOSE 80 8443
# Wed, 20 Sep 2023 22:10:35 GMT
CMD []
```

-	Layers:
	-	`sha256:c25753df0ee4b6d3db1dacebcfb1839260ed067556f1f3ff52ddb574cab51045`  
		Last Modified: Mon, 07 Aug 2023 19:58:28 GMT  
		Size: 2.4 MB (2436761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3edaa1bb34a769d2a617d179c3a121ce323795b2d86f371adf2b18198108ff`  
		Last Modified: Wed, 20 Sep 2023 22:17:51 GMT  
		Size: 42.8 MB (42813817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571ba818c66eb7ccee714ee8e27bf848d97144ffa2ee3885ce0d1ba9bc5edf66`  
		Last Modified: Wed, 20 Sep 2023 22:17:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:97de9f09c69852f96f7c296187539c50dea1aea1f5104e0c5c0c300ae8683af8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52224736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03377611cb0f40f9ce132047f83c95c50a27b27b11429d16a7be1312b16fa719`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:52:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 04:37:13 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 04:37:13 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 04:37:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 04:37:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 04:37:14 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 04:38:26 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 04:38:27 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 04:38:27 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 04:38:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 04:38:27 GMT
USER varnish
# Thu, 21 Sep 2023 04:38:27 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 04:38:27 GMT
CMD []
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43115af36871113661de523d5f39c294c446e845b191847bee9039f91080b5e5`  
		Last Modified: Thu, 21 Sep 2023 04:41:44 GMT  
		Size: 49.5 MB (49503372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08a4e7fb6fee04d2a988db665d17b65b17707f7325f9ec73cb624907e43a2`  
		Last Modified: Thu, 21 Sep 2023 04:41:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:5aa6916b378447ac7ce3bce16083f21640ed77f346d9c6b6110232d87f9c8a01
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61137578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e205d190ad66189082289bc366ecf0ec42f35f54efea247d7e628253d2ba02c6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:42:30 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 02:30:06 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 02:30:07 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 02:30:07 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 02:30:07 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 02:32:23 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 02:32:23 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 02:32:24 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 02:32:24 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 02:32:24 GMT
USER varnish
# Thu, 21 Sep 2023 02:32:24 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 02:32:24 GMT
CMD []
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150ec529b4641ae75ebddb680c40d4461ff6cb20cc9de9000d09e55c4cc77ae`  
		Last Modified: Thu, 21 Sep 2023 02:39:33 GMT  
		Size: 58.3 MB (58304764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d857ef55991e2baf89bc4c3c90d9b09873a4a3f98625ef9aff38572db418bdc`  
		Last Modified: Thu, 21 Sep 2023 02:39:22 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:6e774ae86d3ccd908f2effc52757ac4d1253f3a19bc81f2aa0fe7bcff9aa1f1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49267291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d42006d222979c85edb1b343cc64120bcfde800a88fe802c42c9983c8491b645`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 20:16:50 GMT
ADD file:f730d2cd05a420ffd38548ae1611345fc40a7db59dea5ff41328caa60ee42608 in / 
# Mon, 07 Aug 2023 20:16:51 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:23:54 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:05:18 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:05:18 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:05:19 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:05:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:05:20 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:07:35 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:07:37 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:07:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:07:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:07:38 GMT
USER varnish
# Thu, 21 Sep 2023 01:07:38 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:07:38 GMT
CMD []
```

-	Layers:
	-	`sha256:f1ecf55aa97fb0011a1c90ffc58e5cb218908bc85a13afe003aea5a46e045ac8`  
		Last Modified: Mon, 07 Aug 2023 20:18:07 GMT  
		Size: 2.8 MB (2812358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487e7414b13c044e2fe3ed2d0c178b35a7c77da1716fd0f18713c4b30bf0e8e2`  
		Last Modified: Thu, 21 Sep 2023 01:18:59 GMT  
		Size: 46.5 MB (46454433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e361115526684bb9e4ffadc8f804eff285d2ec63f814fb32981a3580974deded`  
		Last Modified: Thu, 21 Sep 2023 01:18:48 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:b098d4b1fdb99444ed73a7bbf08befce53f939ac48d20b65305b2819cbdbbe52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48935923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357502947ec9a8ad3bdb2f0ed4673f3787524c7ebda92b216c258af34a941513`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Mon, 07 Aug 2023 19:42:16 GMT
ADD file:db6cafb0897c5e32510edd0166d1e1b23001bef271dad57e4157d560bd09dd93 in / 
# Mon, 07 Aug 2023 19:42:16 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 20:45:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_VERSION=7.4.1
# Thu, 21 Sep 2023 01:49:29 GMT
ARG DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c
# Thu, 21 Sep 2023 01:49:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Thu, 21 Sep 2023 01:49:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Thu, 21 Sep 2023 01:49:30 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Thu, 21 Sep 2023 01:49:30 GMT
ENV VARNISH_SIZE=100M
# Thu, 21 Sep 2023 01:50:57 GMT
# ARGS: DIST_SHA512=d5a6ce53bd5fd2afc6a56b7d64fbaf3688bf3de1f39149fb4b4b40acda987bd9ead32f1b9050441a6281c0c2f4a5849d179bfa8615ec98640d9a2e030b0cdb0c PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.1 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 21 Sep 2023 01:51:00 GMT
WORKDIR /etc/varnish
# Thu, 21 Sep 2023 01:51:00 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Thu, 21 Sep 2023 01:51:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 21 Sep 2023 01:51:00 GMT
USER varnish
# Thu, 21 Sep 2023 01:51:00 GMT
EXPOSE 80 8443
# Thu, 21 Sep 2023 01:51:00 GMT
CMD []
```

-	Layers:
	-	`sha256:ec103030fda7a896185e8eb8a4f00b7f611725434956faa395cf74a993a2742e`  
		Last Modified: Mon, 07 Aug 2023 19:43:01 GMT  
		Size: 2.6 MB (2609002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c222777618072a84cbc1cc334e324f1cf6549d9aec24add4de60d61b25f04bf`  
		Last Modified: Thu, 21 Sep 2023 01:54:50 GMT  
		Size: 46.3 MB (46326423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f13e8e461de6c2bbbcf5890fd1669c82689bfea1ce6d63af764a6d281a801cf`  
		Last Modified: Thu, 21 Sep 2023 01:54:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
