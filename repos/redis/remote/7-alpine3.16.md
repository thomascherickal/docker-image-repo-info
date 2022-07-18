## `redis:7-alpine3.16`

```console
$ docker pull redis@sha256:9933e4813b1cec9c450b8b46bc9078874f85b1b06523182f1b96505edefde179
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redis:7-alpine3.16` - linux; amd64

```console
$ docker pull redis@sha256:5b5889a877b4229ac3a548cab811bd1aaa309a74522f62a2de89d79c51600f1b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.3 MB (13326664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:760a0c161a4aa176b6cab59a5ebf2745c2e057782ef7ae28f29e50c4f67c60e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 22:04:39 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 22:04:40 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 18 Jul 2022 19:49:21 GMT
ENV REDIS_VERSION=7.0.4
# Mon, 18 Jul 2022 19:49:21 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.4.tar.gz
# Mon, 18 Jul 2022 19:49:21 GMT
ENV REDIS_DOWNLOAD_SHA=f0e65fda74c44a3dd4fa9d512d4d4d833dd0939c934e946a5c622a630d057f2f
# Mon, 18 Jul 2022 19:50:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 18 Jul 2022 19:50:13 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 18 Jul 2022 19:50:13 GMT
VOLUME [/data]
# Mon, 18 Jul 2022 19:50:13 GMT
WORKDIR /data
# Mon, 18 Jul 2022 19:50:13 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 18 Jul 2022 19:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 19:50:13 GMT
EXPOSE 6379
# Mon, 18 Jul 2022 19:50:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90389148883be3c6500b090644113cf690b528e6f057515568a36bfd0b0d87c`  
		Last Modified: Wed, 25 May 2022 22:09:41 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c08b6ea4d56366e32f458bcaeb9933840882cfa4ac9073d0d42649e34d1a16`  
		Last Modified: Wed, 25 May 2022 22:09:41 GMT  
		Size: 406.2 KB (406166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87bc74a45e95bab7c99a23364087aeab73a7305dadbda24acc6d6498a8feae3`  
		Last Modified: Mon, 18 Jul 2022 19:51:53 GMT  
		Size: 10.1 MB (10119627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2e4996ed54001280975b60848d400c429afaa23ba108304432864c1c4d8a1e`  
		Last Modified: Mon, 18 Jul 2022 19:51:52 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d3fa3b9e2cf737282fa4d27923ed7ae4f1ad86354c1c17e1b5084d24392c4`  
		Last Modified: Mon, 18 Jul 2022 19:51:52 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm variant v6

```console
$ docker pull redis@sha256:ae670c7bcca5aee47ea3589508cb8bfbf91894f2c366d1bd62faf94dfe3d8e15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (13022236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4229f23b1d84eff4089272d6090bea49f0dd381f113fa6a9f103ca0d31d10df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 23:49:59 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 23:50:02 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 18 Jul 2022 18:18:18 GMT
ENV REDIS_VERSION=7.0.4
# Mon, 18 Jul 2022 18:18:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.4.tar.gz
# Mon, 18 Jul 2022 18:18:19 GMT
ENV REDIS_DOWNLOAD_SHA=f0e65fda74c44a3dd4fa9d512d4d4d833dd0939c934e946a5c622a630d057f2f
# Mon, 18 Jul 2022 18:19:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 18 Jul 2022 18:19:45 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 18 Jul 2022 18:19:45 GMT
VOLUME [/data]
# Mon, 18 Jul 2022 18:19:46 GMT
WORKDIR /data
# Mon, 18 Jul 2022 18:19:46 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 18 Jul 2022 18:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 18:19:47 GMT
EXPOSE 6379
# Mon, 18 Jul 2022 18:19:48 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa0ad1182fac92be0203541ebed1ed824b228bb8931f84fd331fc2f5e69e26b`  
		Last Modified: Wed, 25 May 2022 23:58:12 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af04e825a985a118c21a144eaa95bdea91b0a9087403f5edb9bc52c7f1238b9a`  
		Last Modified: Wed, 25 May 2022 23:58:13 GMT  
		Size: 410.4 KB (410362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c9faeff88ed37657c073eb1657d2ad13af6aba8bb6ec831e2073b36834ea20`  
		Last Modified: Mon, 18 Jul 2022 18:22:37 GMT  
		Size: 10.0 MB (10003749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf46b3f98567a7ec5aa29b497c49a601333b57e9a3c99d64b73d056efc4bd9`  
		Last Modified: Mon, 18 Jul 2022 18:22:31 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b040cee6042caadb18de31543b6e810baf730e413f744eac983a95ce0a381372`  
		Last Modified: Mon, 18 Jul 2022 18:22:31 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm variant v7

```console
$ docker pull redis@sha256:5d08f4a962866a69252841d13b1c8da684b82439a89b57f6e97a5d130634e775
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.6 MB (12616759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f41993696afec913455cf54b5b6ddd537ab47d7b8edc3547eb2b61a6304a6af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 01:06:31 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 26 May 2022 01:06:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 12 Jul 2022 02:48:51 GMT
ENV REDIS_VERSION=7.0.3
# Tue, 12 Jul 2022 02:48:52 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.3.tar.gz
# Tue, 12 Jul 2022 02:48:52 GMT
ENV REDIS_DOWNLOAD_SHA=2cde7d17214ffe305953da9fff12333e8a72caa57fd4923e4872f6362a208e73
# Tue, 12 Jul 2022 02:50:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 12 Jul 2022 02:50:17 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 12 Jul 2022 02:50:17 GMT
VOLUME [/data]
# Tue, 12 Jul 2022 02:50:18 GMT
WORKDIR /data
# Tue, 12 Jul 2022 02:50:18 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Tue, 12 Jul 2022 02:50:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:50:19 GMT
EXPOSE 6379
# Tue, 12 Jul 2022 02:50:19 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c95dd4ea78393dcf27dfa1aa64dea763e0fc045eaa38376f2a799ced22b8fc3`  
		Last Modified: Thu, 26 May 2022 01:17:43 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf2b46cefeffc1fbcaae2f439cd8a4063ddd994bf5e57cd4b4e34cc9307a99f`  
		Last Modified: Thu, 26 May 2022 01:17:44 GMT  
		Size: 404.1 KB (404098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0100b8d484f022c62197f11413301456338b0681dc40de3ba994e4b8de75ee`  
		Last Modified: Tue, 12 Jul 2022 03:01:10 GMT  
		Size: 9.8 MB (9799030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9f9d41b6e51ceaf0296ca38569ee333c91855323c4892b04f3299c04a557ee`  
		Last Modified: Tue, 12 Jul 2022 03:01:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24173f8476d106e80f97170749a8f70193fa293efd53d9d5c76b8c9230766ad0`  
		Last Modified: Tue, 12 Jul 2022 03:01:05 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:5eb57f371717570f254c6a7370bb5f7e07e3fcbd98d5e53c5c9351fb653f2ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.2 MB (13244373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae6804ce64b5ead0c6dee9d8d7bc2d5c51d064d5e07ee5a0e4108280fc5e78f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 23:41:51 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 23:41:53 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 18 Jul 2022 18:57:21 GMT
ENV REDIS_VERSION=7.0.4
# Mon, 18 Jul 2022 18:57:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.4.tar.gz
# Mon, 18 Jul 2022 18:57:23 GMT
ENV REDIS_DOWNLOAD_SHA=f0e65fda74c44a3dd4fa9d512d4d4d833dd0939c934e946a5c622a630d057f2f
# Mon, 18 Jul 2022 18:58:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 18 Jul 2022 18:58:13 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 18 Jul 2022 18:58:14 GMT
VOLUME [/data]
# Mon, 18 Jul 2022 18:58:15 GMT
WORKDIR /data
# Mon, 18 Jul 2022 18:58:17 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 18 Jul 2022 18:58:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 18:58:18 GMT
EXPOSE 6379
# Mon, 18 Jul 2022 18:58:19 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb7a578000254e0dc90b6df14e94881632ece9dd85884b400a508492be5d9b`  
		Last Modified: Wed, 25 May 2022 23:51:01 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9052ca636db21d422f2e940c13fa5d300d6e2cf7f86f0f73ea58fab01feedb63`  
		Last Modified: Wed, 25 May 2022 23:51:01 GMT  
		Size: 407.2 KB (407213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5783281b9906669e5fb8ca8a41e2af73c59e8634835e107c597550ff6b2d85`  
		Last Modified: Mon, 18 Jul 2022 19:01:03 GMT  
		Size: 10.1 MB (10140777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf76ed93bb3e99baf71f23c83e05acbbf14a2d8e2bc8204fc5d5b3ae9da3701`  
		Last Modified: Mon, 18 Jul 2022 19:01:01 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fccdf4b4d437f212dafd3a74f24aa1d56b596fbc1fe49fb16d55c0ee4b8ea6`  
		Last Modified: Mon, 18 Jul 2022 19:01:01 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; 386

```console
$ docker pull redis@sha256:aab5e7701a5c9d114816ff90785669cf0135378d1f57798427acf80be7dcff6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12978039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dadb420e7c7aa320ca5aed73162748ce8318be2aadac1f8fe7975680cfb002b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 22:12:12 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 22:12:14 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 18 Jul 2022 18:43:05 GMT
ENV REDIS_VERSION=7.0.4
# Mon, 18 Jul 2022 18:43:06 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.4.tar.gz
# Mon, 18 Jul 2022 18:43:07 GMT
ENV REDIS_DOWNLOAD_SHA=f0e65fda74c44a3dd4fa9d512d4d4d833dd0939c934e946a5c622a630d057f2f
# Mon, 18 Jul 2022 18:43:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 18 Jul 2022 18:43:59 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 18 Jul 2022 18:44:00 GMT
VOLUME [/data]
# Mon, 18 Jul 2022 18:44:01 GMT
WORKDIR /data
# Mon, 18 Jul 2022 18:44:03 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 18 Jul 2022 18:44:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 18:44:04 GMT
EXPOSE 6379
# Mon, 18 Jul 2022 18:44:05 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5606fb113d21aa033df3c08bd7a75a5a81b2bdcd6f07088d5361b11a25a30f6`  
		Last Modified: Wed, 25 May 2022 22:19:30 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01878a6bc72011373f1316d7c82f835278bc12d26b93301da233a8499ea2f239`  
		Last Modified: Wed, 25 May 2022 22:19:30 GMT  
		Size: 413.6 KB (413593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b304da6e8623e8ad784c58aae7f654a41ed1ac0437f1f0f8f1862c47167da1dc`  
		Last Modified: Mon, 18 Jul 2022 18:46:57 GMT  
		Size: 9.8 MB (9760643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eee51e77fa02b06b15248d365b7eaea12ef970a27f27238f54e39be971f80f`  
		Last Modified: Mon, 18 Jul 2022 18:46:55 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d57f713ed166eceb271dc6818e71fb6b61687c8e4a849162eccf331f61512a4`  
		Last Modified: Mon, 18 Jul 2022 18:46:56 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; ppc64le

```console
$ docker pull redis@sha256:24c0778666c893564fe1784f153aff4dfebf744728d1449e3c042a40b853ea29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13879235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:962ce40187b8d475001c3e3e42d371c45312cf70a3491714f417a8710886ea0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 00:20:18 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 26 May 2022 00:20:34 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 12 Jul 2022 03:27:49 GMT
ENV REDIS_VERSION=7.0.3
# Tue, 12 Jul 2022 03:27:56 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.3.tar.gz
# Tue, 12 Jul 2022 03:27:59 GMT
ENV REDIS_DOWNLOAD_SHA=2cde7d17214ffe305953da9fff12333e8a72caa57fd4923e4872f6362a208e73
# Tue, 12 Jul 2022 03:29:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 12 Jul 2022 03:29:22 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 12 Jul 2022 03:29:26 GMT
VOLUME [/data]
# Tue, 12 Jul 2022 03:29:33 GMT
WORKDIR /data
# Tue, 12 Jul 2022 03:29:35 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Tue, 12 Jul 2022 03:29:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 03:29:40 GMT
EXPOSE 6379
# Tue, 12 Jul 2022 03:29:43 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829eb500d899e72e6b49a33db765f361e3f6b6e9f8f7022cbd62988a36011b69`  
		Last Modified: Thu, 26 May 2022 00:35:11 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac73a539d726ff67c63af0126efb487ef797bdc2b4f487a546b9babfe784f6`  
		Last Modified: Thu, 26 May 2022 00:35:11 GMT  
		Size: 413.6 KB (413623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4012b9f63a4da223ba38ed828da293d5c0e49a33abfcc5cf9151e3398cbde339`  
		Last Modified: Tue, 12 Jul 2022 03:49:28 GMT  
		Size: 10.7 MB (10673871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a557c4d4e95aee294c40c6e6cf0ff4735bf1de0ea603066c3495d596eea7d29`  
		Last Modified: Tue, 12 Jul 2022 03:49:26 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d55894ccdd28283e6efdec6d1f2a4a42df061842d601ec9b4e4e875c394f9`  
		Last Modified: Tue, 12 Jul 2022 03:49:26 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; s390x

```console
$ docker pull redis@sha256:bb7cbcbe806e9d4382322e7adf9b301aadbb6c60c5340dfd9f5b69d6cceeddc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13118817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e5a6e1cb331c7da92dcf797dfde27f4b0d3de5f126ae38fea665f68ea6a198`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 23:23:38 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 23:23:39 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 18 Jul 2022 19:54:30 GMT
ENV REDIS_VERSION=7.0.4
# Mon, 18 Jul 2022 19:54:30 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.4.tar.gz
# Mon, 18 Jul 2022 19:54:31 GMT
ENV REDIS_DOWNLOAD_SHA=f0e65fda74c44a3dd4fa9d512d4d4d833dd0939c934e946a5c622a630d057f2f
# Mon, 18 Jul 2022 19:55:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 18 Jul 2022 19:55:44 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 18 Jul 2022 19:55:45 GMT
VOLUME [/data]
# Mon, 18 Jul 2022 19:55:45 GMT
WORKDIR /data
# Mon, 18 Jul 2022 19:55:46 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 18 Jul 2022 19:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 19:55:47 GMT
EXPOSE 6379
# Mon, 18 Jul 2022 19:55:48 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152aae9522a42ef726a16c3f39fadb0aa74325b74a43efad7ee7605b4ff68a7b`  
		Last Modified: Wed, 25 May 2022 23:30:19 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e02fe158318d41fa93857ee7ac8c3f7fbe37d1d58f47858c6cb9839fba2210`  
		Last Modified: Wed, 25 May 2022 23:30:19 GMT  
		Size: 410.9 KB (410950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff447aff4aca88fb956ddc673cacedbfc2db7d569e0445363ff53ac1807f413`  
		Last Modified: Mon, 18 Jul 2022 19:59:21 GMT  
		Size: 10.1 MB (10125392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a9448dace7b70e68b8478199f869ba93583ffe6d7541635b80219c22316c6f5`  
		Last Modified: Mon, 18 Jul 2022 19:59:20 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a179ca844ad1c85c27689f353f5186e68491a31dc9dffaa765abc6cac4b18f`  
		Last Modified: Mon, 18 Jul 2022 19:59:20 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
