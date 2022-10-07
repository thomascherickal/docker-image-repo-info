## `varnish:alpine`

```console
$ docker pull varnish@sha256:48a6af21ed8bb8c25caef9c1782ab4632690b7c44d30b332eae1ccaa028de4ef
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
$ docker pull varnish@sha256:07617135423b40d79c0e63a58c444b09921a1ac8af4eba193f7396975e5010da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59397030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeb723f9b60b4f8a8193cee3acac5b67c7c56bd4d94875e13befcb3e39c7015`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 00:23:20 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 00:23:20 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 00:23:20 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 00:23:21 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 00:23:21 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 23 Sep 2022 19:36:01 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 23 Sep 2022 19:36:02 GMT
ENV VARNISH_SIZE=100M
# Fri, 23 Sep 2022 19:37:16 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 23 Sep 2022 19:37:17 GMT
WORKDIR /etc/varnish
# Fri, 23 Sep 2022 19:37:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 23 Sep 2022 19:37:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 23 Sep 2022 19:37:17 GMT
USER varnish
# Fri, 23 Sep 2022 19:37:17 GMT
EXPOSE 80 8443
# Fri, 23 Sep 2022 19:37:17 GMT
CMD []
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c287ddf9b273f136c47aadab6373f9ec90d952855bb4542357ccb5c83967fed5`  
		Last Modified: Fri, 23 Sep 2022 19:42:35 GMT  
		Size: 56.6 MB (56573021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798ce08d84893434cb30191b99e11d9d5307d24791143eee17b0f104dd6158a8`  
		Last Modified: Fri, 23 Sep 2022 19:42:26 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:a8a6cb141f7cff1bcd26c37763fbf42a44e064ba127eea81c600e62ffcbe6d58
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45148535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d94e423bb52f8fa146e3a15e1dae785b7568955f0e77f877184b6254366e4cf8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Fri, 16 Sep 2022 01:01:50 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 16 Sep 2022 01:01:50 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 16 Sep 2022 01:01:51 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 16 Sep 2022 01:01:51 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 23 Sep 2022 20:01:44 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 23 Sep 2022 20:01:44 GMT
ENV VARNISH_SIZE=100M
# Fri, 23 Sep 2022 20:03:58 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 23 Sep 2022 20:03:58 GMT
WORKDIR /etc/varnish
# Fri, 23 Sep 2022 20:03:58 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 23 Sep 2022 20:03:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 23 Sep 2022 20:03:59 GMT
USER varnish
# Fri, 23 Sep 2022 20:03:59 GMT
EXPOSE 80 8443
# Fri, 23 Sep 2022 20:03:59 GMT
CMD []
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c51cff6dfe44712375ee3e8908f374e4c5031d1237a0fafebe79b24b86dad8`  
		Last Modified: Fri, 23 Sep 2022 20:11:30 GMT  
		Size: 42.7 MB (42712944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b0e73956136a384965d109d15da7384ea73d00a7f3adbb2f0443bf029cb901`  
		Last Modified: Fri, 23 Sep 2022 20:11:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:717487768ed81ea94dcd6748da9228cb8fe1b81073556069cb80a5a73295860a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51804094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee536e43e5fad78caf269808dfee93cd9e76b376e813eb5964549278149e59b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:16:46 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:51:52 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:51:53 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:51:54 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:51:55 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:51:56 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:51:57 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:51:58 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:51:59 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:52:00 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:52:01 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:53:20 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:53:20 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:53:22 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:53:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:53:23 GMT
USER varnish
# Thu, 11 Aug 2022 17:53:24 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:53:25 GMT
CMD []
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66637d73d151e7b8d3fe367559b7457ef1203d2aebfd50c2e70fd5bf1e99c081`  
		Last Modified: Thu, 11 Aug 2022 17:58:22 GMT  
		Size: 49.1 MB (49085174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b2c3b885888b477b35c280e036923c88b655803b494242a5f224b80f8ceed`  
		Last Modified: Thu, 11 Aug 2022 17:58:15 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:93605d834595abc7fb113c43a552a115ddc1a5eecf73da0a6e95044a3e80b2c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59567789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e560b9e6f2c39b1e451b47221a36050a0dc729d070ca5c4583894a5f61b5d4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:07:46 GMT
ARG PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2
# Fri, 07 Oct 2022 02:07:47 GMT
ARG VARNISH_VERSION=7.2.0
# Fri, 07 Oct 2022 02:07:48 GMT
ARG DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133
# Fri, 07 Oct 2022 02:07:49 GMT
ARG VARNISH_MODULES_VERSION=0.21.0
# Fri, 07 Oct 2022 02:07:50 GMT
ARG VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35
# Fri, 07 Oct 2022 02:07:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Fri, 07 Oct 2022 02:07:52 GMT
ARG VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597
# Fri, 07 Oct 2022 02:07:53 GMT
ARG VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5
# Fri, 07 Oct 2022 02:07:54 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Fri, 07 Oct 2022 02:07:55 GMT
ENV VMOD_DEPS=automake curl libtool make pkgconfig py3-sphinx
# Fri, 07 Oct 2022 02:07:56 GMT
ENV VARNISH_SIZE=100M
# Fri, 07 Oct 2022 02:09:15 GMT
# ARGS: DIST_SHA512=d9a57d644d1b1456ee96ee84182f816b3b693fe2d9cc4b1859b62a836ee8c7d51025bb96efbc0ebc82349f60b2f186335436d76c12a5257c0560572db9d01133 PKG_COMMIT=ffc59a345217b599fd49f7f0442b5f653fbe6fc2 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=a442f58968b471d713c99a94e5b80302c07ea163d3d5022d768eb0b39ab081f18744fd529b04283b0c6ec942f362197935d8ef1aa04f26eff10a81425a63bd35 VARNISH_MODULES_VERSION=0.21.0 VARNISH_VERSION=7.2.0 VMOD_DYNAMIC_COMMIT=9666973952f62110c872d720af3dae0b85b4b597 VMOD_DYNAMIC_SHA512SUM=e62f1ee801ab2c9e22f5554bbe40c239257e2c46ea3d2ae19b465b1c82edad6f675417be8f7351d4f9eddafc9ad6c0149f88edc44dd0b922ad82e5d75b6b15a5 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Fri, 07 Oct 2022 02:09:15 GMT
WORKDIR /etc/varnish
# Fri, 07 Oct 2022 02:09:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Fri, 07 Oct 2022 02:09:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 07 Oct 2022 02:09:18 GMT
USER varnish
# Fri, 07 Oct 2022 02:09:19 GMT
EXPOSE 80 8443
# Fri, 07 Oct 2022 02:09:20 GMT
CMD []
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbeb1f1d7ada5c4c59e36003a84c143bfbc80a278511d2f0e8f781bc4f4321b`  
		Last Modified: Fri, 07 Oct 2022 02:15:27 GMT  
		Size: 56.7 MB (56738775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef259dee8d48639b6034a28182bb2ecf3b919244e862c6e8ebb64b8e9525120`  
		Last Modified: Fri, 07 Oct 2022 02:15:20 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:30297707c2dea193bfd2f5f51f569d60a07ab77e2c3bbd04fa2d3cd1e5a9ba1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48872146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:198c71b8b6d1f902598d81b5071bfdb145e03dbd456cc6450dbff7b15d3e124a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:13:06 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 18:24:41 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 18:24:41 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 18:24:42 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 18:24:43 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 18:24:43 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 18:24:44 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 18:26:34 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 18:26:37 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 18:26:38 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 18:26:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 18:26:38 GMT
USER varnish
# Thu, 11 Aug 2022 18:26:39 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 18:26:39 GMT
CMD []
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a15064fbadc2b9bce565fe7971fba76bf7ae75f6d59ef2522607a17e18fb60`  
		Last Modified: Thu, 11 Aug 2022 18:35:48 GMT  
		Size: 46.1 MB (46058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ce3575e5c3e8299b4379e48b60fd9a86b324975077480e6b6099c2d229a0c7`  
		Last Modified: Thu, 11 Aug 2022 18:35:36 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:ef0bc428fc8797be18df6dbab001bd40862f568a9b2c21fdb3649b31e4caf168
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47321908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:469bd0d9c7f85d2ba2e3eec193b415418ebc882b89f18eb37d1fde4b613c0f78`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:54:27 GMT
ARG PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83
# Thu, 11 Aug 2022 17:46:35 GMT
ARG VARNISH_VERSION=7.1.1
# Thu, 11 Aug 2022 17:46:35 GMT
ARG DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_VERSION=0.20.0
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36
# Thu, 11 Aug 2022 17:46:36 GMT
ARG VMOD_DYNAMIC_VERSION=2.6.0
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a
# Thu, 11 Aug 2022 17:46:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816
# Thu, 11 Aug 2022 17:46:37 GMT
ARG TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VMOD_DEPS=automake curl gcc libtool make pkgconfig py3-sphinx
# Thu, 11 Aug 2022 17:46:38 GMT
ENV VARNISH_SIZE=100M
# Thu, 11 Aug 2022 17:48:19 GMT
# ARGS: DIST_SHA512=7c3c081bd37c63b429337a25ebc0c14d780b0c4fd235d18b9ac1004e0bb2f65e70664c5bd25c5d941deeb6bc078f344fa2629cf0d641a0149fe29dcfa07ffcd2 PKG_COMMIT=3ba24a8eee8cc5c082714034145b907402bbdb83 TOOLBOX_COMMIT=96bab07cf58b6e04824ffec608199f1780ff0d04 VARNISH_MODULES_SHA512SUM=e63d6da8f63a5ce56bc7a5a1dd1a908e4ab0f6a36b5bdc5709dca2aa9c0b474bd8a06491ed3dee23636d335241ced4c7ef017b57413b05792ad382f6306a0b36 VARNISH_MODULES_VERSION=0.20.0 VARNISH_VERSION=7.1.1 VMOD_DYNAMIC_COMMIT=025e9918f6cba33135e16e0fb0d86b4c34b6dd5a VMOD_DYNAMIC_SHA512SUM=89b7251529c4c63c408b83c59e32b54b94b0f31f83614a34b3ffc4fb96ebdac5b6f8b5fe5b95056d5952a3c0a0217c935c5073c38415f7680af748e58c041816 VMOD_DYNAMIC_VERSION=2.6.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Thu, 11 Aug 2022 17:48:25 GMT
WORKDIR /etc/varnish
# Thu, 11 Aug 2022 17:48:25 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Thu, 11 Aug 2022 17:48:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 11 Aug 2022 17:48:26 GMT
USER varnish
# Thu, 11 Aug 2022 17:48:26 GMT
EXPOSE 80 8443
# Thu, 11 Aug 2022 17:48:27 GMT
CMD []
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694fec8cf4b1f4958bdd7c4941f751e5c9df3eb875c8003dccefe1dd9cfce4e2`  
		Last Modified: Thu, 11 Aug 2022 17:56:53 GMT  
		Size: 44.7 MB (44715342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e69ac324df99a42204cf390757a838e28f80ceb7564f1e690948bcba9a7e14c`  
		Last Modified: Thu, 11 Aug 2022 17:56:48 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
