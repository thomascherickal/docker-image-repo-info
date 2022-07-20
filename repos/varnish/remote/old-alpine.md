## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:a59c066b705ad10b2450a1e7c0077ae34d407b31058f55d05e8fb41abf0052c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:old-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:0f95108ab26337ee406050486ff6188716856c81622a9065814fa1e8c94294fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58350434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af411581b19d6e03c7df7af3b18e3dc7de8deda60ef5650151d17138a978dec0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:29:13 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Jul 2022 02:29:55 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 20 Jul 2022 02:29:55 GMT
WORKDIR /etc/varnish
# Wed, 20 Jul 2022 02:29:55 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 20 Jul 2022 02:29:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Jul 2022 02:29:56 GMT
EXPOSE 80 8443
# Wed, 20 Jul 2022 02:29:56 GMT
CMD []
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286c0571d128d3488e745908c8624d69680820fe3134eb10782f59b7ad54990d`  
		Last Modified: Wed, 20 Jul 2022 02:30:52 GMT  
		Size: 55.5 MB (55531445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759c266b4e5bac5c211ffc88f86f03d49d1ea704a116454fdd4e63d7c74f0284`  
		Last Modified: Wed, 20 Jul 2022 02:30:45 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0a7f4c043c2e21f655c6f0566dcb81d61effbdb1df879cf35e95b51f35f6d35a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44159514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3f3053fb64e860e431017f54395ec210c8aab2f988318196c2083125ecf4068`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:58:08 GMT
ADD file:d2a65f1d7470d13e9d8ff9e0bb0423ef7db0accb324da11d301fb273df11219c in / 
# Tue, 19 Jul 2022 22:58:09 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 07:19:23 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Jul 2022 07:20:49 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 20 Jul 2022 07:20:50 GMT
WORKDIR /etc/varnish
# Wed, 20 Jul 2022 07:20:50 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 20 Jul 2022 07:20:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Jul 2022 07:20:51 GMT
EXPOSE 80 8443
# Wed, 20 Jul 2022 07:20:52 GMT
CMD []
```

-	Layers:
	-	`sha256:9c9353d8b73e41cefa3bc75da295a6ba0845d9938b166d714351be245f30cbc3`  
		Last Modified: Tue, 19 Jul 2022 22:59:48 GMT  
		Size: 2.4 MB (2428241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b31b9968806befa0ca0da5799a1b95779b186c4090c935b8afb968ec31a4662`  
		Last Modified: Wed, 20 Jul 2022 07:23:44 GMT  
		Size: 41.7 MB (41730794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f937247975e7c01bcf89efc68a4e01569de383905fa7109e3ffe22c28d6db6`  
		Last Modified: Wed, 20 Jul 2022 07:23:22 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:9ed00a90bdc84dddbe24d3716539597ba6296ca53a0d31a06824820bbec35ece
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51102312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f49e95dcac5ef5d56b5148462e8d11f9d590a8c9f12c01c45f79e38351994f3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 05:55:14 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Jul 2022 05:55:59 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 20 Jul 2022 05:55:59 GMT
WORKDIR /etc/varnish
# Wed, 20 Jul 2022 05:56:01 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 20 Jul 2022 05:56:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Jul 2022 05:56:02 GMT
EXPOSE 80 8443
# Wed, 20 Jul 2022 05:56:03 GMT
CMD []
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161303575151c5f5cbb14fe8169c9711e013b36b07dcec19f3a0af45925c1faf`  
		Last Modified: Wed, 20 Jul 2022 05:57:28 GMT  
		Size: 48.4 MB (48384087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c921e607a4a4058ed08b35cf5169d784fe034b6dc0899ab222dba3343b576b9`  
		Last Modified: Wed, 20 Jul 2022 05:57:21 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:dcadf2f1589588769716e0d253cf48bc6bc71c29e8cec89a5c5f4a056c1ca1fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.5 MB (58549841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebcb76713d9f0df4e47ce4a43716bf1e8ae754ad3cbe19203a4dec3723055980`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:38:40 GMT
ADD file:4ae4391bf852a3e83cff6c0baebf0241d4955d580e24c180f882a142e4adaf1d in / 
# Tue, 19 Jul 2022 22:38:40 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:24:19 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Jul 2022 02:25:03 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 20 Jul 2022 02:25:03 GMT
WORKDIR /etc/varnish
# Wed, 20 Jul 2022 02:25:05 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 20 Jul 2022 02:25:05 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Jul 2022 02:25:06 GMT
EXPOSE 80 8443
# Wed, 20 Jul 2022 02:25:07 GMT
CMD []
```

-	Layers:
	-	`sha256:cbf9934fc184d27d98bef2567dbcecbee05767c8762c95e63984577a8c23e961`  
		Last Modified: Tue, 19 Jul 2022 22:39:35 GMT  
		Size: 2.8 MB (2821611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43145b3b1aee8cf99942576ad1267e0f452afe1152481810c40973dcc244b234`  
		Last Modified: Wed, 20 Jul 2022 02:26:41 GMT  
		Size: 55.7 MB (55727753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6990782b33d766bd7755f491cf11605d12af947424c24baa3cb99020f1f03002`  
		Last Modified: Wed, 20 Jul 2022 02:26:35 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:fa4da2838ba1c35c497605b02fbaa6495b9b89f2099a893316373e8b042b0258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48200382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbcea45e25448b06ffb34f93d56f24dea75034ac436374461efdd78aacfa8e95`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:26:48 GMT
ADD file:f7d6f7b933d430698b1ac478c38557461cf2d285610a6d61f367cdfbea0ce98d in / 
# Tue, 19 Jul 2022 22:26:50 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 06:19:57 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Jul 2022 06:21:14 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 20 Jul 2022 06:21:21 GMT
WORKDIR /etc/varnish
# Wed, 20 Jul 2022 06:21:23 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 20 Jul 2022 06:21:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Jul 2022 06:21:30 GMT
EXPOSE 80 8443
# Wed, 20 Jul 2022 06:21:35 GMT
CMD []
```

-	Layers:
	-	`sha256:6cd2a055da5ab30190fcb8d96ad641b769d3198bf9c087007cdf2d8775c437b0`  
		Last Modified: Tue, 19 Jul 2022 22:28:07 GMT  
		Size: 2.8 MB (2814561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f2a2797c57525d3bd497655694ec9270a9c7d7d6a71db9a2c0dc9dd8b45f0d`  
		Last Modified: Wed, 20 Jul 2022 06:23:17 GMT  
		Size: 45.4 MB (45385341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fc1a1f6e83d0711f9cd0e86f3d6d46c77331babbf4beca6a91f88816a02ad6`  
		Last Modified: Wed, 20 Jul 2022 06:23:08 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:3503bbd842f4704b6d2f8f914381fd1d4fc8f865d6219deaab7ec066a2082f07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46671092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b56c0f583e4fd60bf94608c50424c3cc6a3ca689bfd7ecb10168c3ad28d76b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:42:10 GMT
ADD file:fda7ba88b3cdb8af6b8fcdc0e28f3e805973b011de9f083c9af0b294998a3b4a in / 
# Tue, 19 Jul 2022 22:42:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 01:41:18 GMT
ENV VARNISH_SIZE=100M
# Wed, 20 Jul 2022 01:42:41 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 20 Jul 2022 01:42:44 GMT
WORKDIR /etc/varnish
# Wed, 20 Jul 2022 01:42:44 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 20 Jul 2022 01:42:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 20 Jul 2022 01:42:45 GMT
EXPOSE 80 8443
# Wed, 20 Jul 2022 01:42:45 GMT
CMD []
```

-	Layers:
	-	`sha256:3955a3cbf194cd4cb6e57e1347e8ec78d800d4db5d2cba99a0dae7da438a3a7f`  
		Last Modified: Tue, 19 Jul 2022 22:43:25 GMT  
		Size: 2.6 MB (2604367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c3a5671d95f9c398cd4ac997d0bcc61be9cdaaeb254f21310bd477b4391362`  
		Last Modified: Wed, 20 Jul 2022 01:44:03 GMT  
		Size: 44.1 MB (44066251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3653f3a07a52408a54b71f4f4f72b6a6114fe1abf02e11e1a1cf6910070b4c3`  
		Last Modified: Wed, 20 Jul 2022 01:43:57 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
