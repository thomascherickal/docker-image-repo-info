## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:20d7dcdd046171d699ccef2105736b61cf9a6ebaa65b6e3fe30785a44add0ce1
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
$ docker pull varnish@sha256:7f47d96333588d27325c6ffceeef0ad219dfe6ee16a77e6d4dc88a3459649e24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44163426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd8d15e9995875e4f9c6c7d1906fa6fee1feaa179c5cc55b5a18f7a56a9e33c6`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:58:08 GMT
ADD file:d2a65f1d7470d13e9d8ff9e0bb0423ef7db0accb324da11d301fb273df11219c in / 
# Tue, 19 Jul 2022 22:58:09 GMT
CMD ["/bin/sh"]
# Wed, 03 Aug 2022 12:18:41 GMT
ENV VARNISH_SIZE=100M
# Wed, 03 Aug 2022 12:20:29 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 03 Aug 2022 12:20:29 GMT
WORKDIR /etc/varnish
# Wed, 03 Aug 2022 12:20:29 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 03 Aug 2022 12:20:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 03 Aug 2022 12:20:30 GMT
EXPOSE 80 8443
# Wed, 03 Aug 2022 12:20:30 GMT
CMD []
```

-	Layers:
	-	`sha256:9c9353d8b73e41cefa3bc75da295a6ba0845d9938b166d714351be245f30cbc3`  
		Last Modified: Tue, 19 Jul 2022 22:59:48 GMT  
		Size: 2.4 MB (2428241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e60c4952ee9521c5996167d6ceab2c59b99fa04b3c05c329f3c0a204f8a0cf`  
		Last Modified: Wed, 03 Aug 2022 12:22:48 GMT  
		Size: 41.7 MB (41734705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c705c56c8828bdddf9ac5dec6081eb394b5bb17c932a3c4a55400a78f1abce`  
		Last Modified: Wed, 03 Aug 2022 12:22:40 GMT  
		Size: 480.0 B  
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
$ docker pull varnish@sha256:d49441380189577b764cdcbebd5f50638f4ab20559700cc9d535104ba41d4950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48214010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0163e7c5a69ce05aefe95ae93146ff692754f1ef890de0fd7723ed668d69af`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Jul 2022 22:26:48 GMT
ADD file:f7d6f7b933d430698b1ac478c38557461cf2d285610a6d61f367cdfbea0ce98d in / 
# Tue, 19 Jul 2022 22:26:50 GMT
CMD ["/bin/sh"]
# Wed, 03 Aug 2022 01:44:42 GMT
ENV VARNISH_SIZE=100M
# Wed, 03 Aug 2022 01:46:06 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=7.0.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"5eb08345c95152639266b7ad241185188477f8fd04e88e4dfda1579719a1a413790a0616f25d70994f6d3b8f7640ea80926ece7c547555dad856fd9f6960c9a3  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 03 Aug 2022 01:46:08 GMT
WORKDIR /etc/varnish
# Wed, 03 Aug 2022 01:46:08 GMT
COPY dir:846b8f8975487ee292d565d7ea945a1a79fb5f0e418fec900574091bb0a7cffc in /usr/local/bin/ 
# Wed, 03 Aug 2022 01:46:08 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 03 Aug 2022 01:46:09 GMT
EXPOSE 80 8443
# Wed, 03 Aug 2022 01:46:09 GMT
CMD []
```

-	Layers:
	-	`sha256:6cd2a055da5ab30190fcb8d96ad641b769d3198bf9c087007cdf2d8775c437b0`  
		Last Modified: Tue, 19 Jul 2022 22:28:07 GMT  
		Size: 2.8 MB (2814561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed61875fff6ffc25e866ca1d7f5602e7b6f3d8f297dfcf40215d9fc2f5245f`  
		Last Modified: Wed, 03 Aug 2022 01:53:46 GMT  
		Size: 45.4 MB (45398967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e6a6d24bacb7b9e5fcb803deb17c254227784ee6d397388ad151fe1c481847`  
		Last Modified: Wed, 03 Aug 2022 01:53:34 GMT  
		Size: 482.0 B  
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
