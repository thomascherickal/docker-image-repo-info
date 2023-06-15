## `redis:7-alpine3.18`

```console
$ docker pull redis@sha256:e8cc19a67c7c425aafd2f89e790d83522c3099a745ded346fb03a0183e3288a6
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

### `redis:7-alpine3.18` - linux; amd64

```console
$ docker pull redis@sha256:ed439ea2fd065ac9622bf40b8bdb156e1e2bb2b73f7877f430775b8d728b3eec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.4 MB (12428303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e5fefbc0ede9d0bdea6071e986e1e0f1bafd50bbcd90ba680142da24fb824e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 21:55:02 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 14 Jun 2023 21:55:03 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 14 Jun 2023 21:57:10 GMT
ENV REDIS_VERSION=7.0.11
# Wed, 14 Jun 2023 21:57:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Wed, 14 Jun 2023 21:57:10 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Wed, 14 Jun 2023 21:57:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 14 Jun 2023 21:57:50 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 14 Jun 2023 21:57:50 GMT
VOLUME [/data]
# Wed, 14 Jun 2023 21:57:50 GMT
WORKDIR /data
# Wed, 14 Jun 2023 21:57:50 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 14 Jun 2023 21:57:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 21:57:50 GMT
EXPOSE 6379
# Wed, 14 Jun 2023 21:57:50 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029a81f05585f767fb7549af85a8f24479149e2a73710427a8775593fbe86159`  
		Last Modified: Wed, 14 Jun 2023 22:01:45 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aaf69037d81f66eec59c735ab5ab7e0a7bf9a2206560da4a7f34fb381758417`  
		Last Modified: Wed, 14 Jun 2023 22:01:45 GMT  
		Size: 347.2 KB (347154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91944a72799a833237ecbab7c1b2dc1bdba0d0dfd7d43ee8f26bdae92f0911e2`  
		Last Modified: Wed, 14 Jun 2023 22:02:22 GMT  
		Size: 8.7 MB (8681289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5de2284ef1e9dbb63f847376e19ee4ad8b1962a83067b96dde3fc498ba7ccaf`  
		Last Modified: Wed, 14 Jun 2023 22:02:21 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3505ebdde63518a7018dcc3892f6369fb3d67cc4f289b017da0f8f8c86b330`  
		Last Modified: Wed, 14 Jun 2023 22:02:21 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.18` - linux; arm variant v6

```console
$ docker pull redis@sha256:ab8a8137716f2115b373f3ed77c3e23151d99c3fb569b01f316f0a1dcad47a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.3 MB (12257709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc069e63b8c6b8715c2dcec859388a6f04047d8f5f3a052b59ab57cf375fcca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:20 GMT
ADD file:4213782693bf27a9a6de23bc924ef0c4fb6b2d56010fc07b25f81edeba83b0d4 in / 
# Wed, 14 Jun 2023 18:49:20 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 19:39:35 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 14 Jun 2023 19:39:37 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 14 Jun 2023 19:40:33 GMT
ENV REDIS_VERSION=7.0.11
# Wed, 14 Jun 2023 19:40:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Wed, 14 Jun 2023 19:40:33 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Wed, 14 Jun 2023 19:41:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 14 Jun 2023 19:41:14 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 14 Jun 2023 19:41:14 GMT
VOLUME [/data]
# Wed, 14 Jun 2023 19:41:14 GMT
WORKDIR /data
# Wed, 14 Jun 2023 19:41:14 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 14 Jun 2023 19:41:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 19:41:14 GMT
EXPOSE 6379
# Wed, 14 Jun 2023 19:41:14 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:7836be94d3024e2042069c1095caba0b391f70c4b3d34a0475a503239d73dfba`  
		Last Modified: Wed, 14 Jun 2023 18:49:46 GMT  
		Size: 3.1 MB (3143353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08134307b2d501ac132f682f6420e34beae2815eac7af11ddaf1f0c6e21b5c3f`  
		Last Modified: Wed, 14 Jun 2023 19:42:51 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce110bc6510ed6e4705a2a18fca736cdc4761bdc3807aa523e23c9bee8d06814`  
		Last Modified: Wed, 14 Jun 2023 19:42:51 GMT  
		Size: 346.9 KB (346942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d9c6c789622fd0efbb3cd3755b1a431132a995f03221224ce93c56361d5f3b`  
		Last Modified: Wed, 14 Jun 2023 19:43:09 GMT  
		Size: 8.8 MB (8765430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b950f2f19fc29caf61e38a10d21adbb7dab30d3620ed7725cac9f80f514ba458`  
		Last Modified: Wed, 14 Jun 2023 19:43:07 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e58ca072d13da3adf8f07a4cc88a889299f59a1136adb8339cc14229419296`  
		Last Modified: Wed, 14 Jun 2023 19:43:07 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.18` - linux; arm variant v7

```console
$ docker pull redis@sha256:edd654d72d64ae4fa49e7c8210e66d360a4c3a1e17a7d17f41642978ea9e07fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11888343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c91f64152c734ca8159172f2ef62e7cf7776f25b203b676d0e74db7dce3f83e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:15 GMT
ADD file:082f034323c559f3cb9feb6422c88b1ec8017f436d6109e238a5c5384a32a90a in / 
# Wed, 14 Jun 2023 22:36:15 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 01:23:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Jun 2023 01:23:17 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 15 Jun 2023 01:25:00 GMT
ENV REDIS_VERSION=7.0.11
# Thu, 15 Jun 2023 01:25:00 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Thu, 15 Jun 2023 01:25:01 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Thu, 15 Jun 2023 01:25:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 15 Jun 2023 01:25:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 15 Jun 2023 01:25:37 GMT
VOLUME [/data]
# Thu, 15 Jun 2023 01:25:37 GMT
WORKDIR /data
# Thu, 15 Jun 2023 01:25:38 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:25:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 01:25:38 GMT
EXPOSE 6379
# Thu, 15 Jun 2023 01:25:38 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:633ba29fd335042456b6e2c073636f6fa30de56f1331c442914739b92a479974`  
		Last Modified: Wed, 14 Jun 2023 22:36:49 GMT  
		Size: 2.9 MB (2898508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f416f0a4d9526536e0b8b07fdbb39dae0dc1cb703dd160b8a0959d79ec3149`  
		Last Modified: Thu, 15 Jun 2023 01:29:59 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f142ed3e19bd076e51f2af8f2a237eeb5e7cc45147edc602947a17a85ec8a9a4`  
		Last Modified: Thu, 15 Jun 2023 01:29:59 GMT  
		Size: 346.8 KB (346759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced3aa58202d86e2685ca5ecef22e5f0ad9cf54b45adfe2a1b8e5337081d9ee0`  
		Last Modified: Thu, 15 Jun 2023 01:30:38 GMT  
		Size: 8.6 MB (8641096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7c24851e87ea0602fa93f8b827c8cbc410c8f9bb0c33c6e774841fa5de7bc9`  
		Last Modified: Thu, 15 Jun 2023 01:30:37 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383fec46803fbddd774afdbd2408278e8984c13edf82767c373df39e9dd0ac6f`  
		Last Modified: Thu, 15 Jun 2023 01:30:37 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:5271650d6955664fe5afefa0928617a6e05a794ea5a72cdfcbe311bc6aa49013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.5 MB (12455862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc5c8801dc6c3e523b1df09783ae6aeb30d7791f00ac401857bdbf9bf86b615`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 21:51:23 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 14 Jun 2023 21:51:24 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 14 Jun 2023 21:52:51 GMT
ENV REDIS_VERSION=7.0.11
# Wed, 14 Jun 2023 21:52:51 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Wed, 14 Jun 2023 21:52:51 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Wed, 14 Jun 2023 21:53:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 14 Jun 2023 21:53:21 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 14 Jun 2023 21:53:21 GMT
VOLUME [/data]
# Wed, 14 Jun 2023 21:53:22 GMT
WORKDIR /data
# Wed, 14 Jun 2023 21:53:22 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 14 Jun 2023 21:53:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 21:53:22 GMT
EXPOSE 6379
# Wed, 14 Jun 2023 21:53:22 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0943de4c7d746d0a5d970911570b2a558b401fab28f91a87467f5c0254e52dac`  
		Last Modified: Wed, 14 Jun 2023 21:56:37 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e86621887466535e33778300b0d4d1c589f380a65ae9455235bf38c6938288`  
		Last Modified: Wed, 14 Jun 2023 21:56:37 GMT  
		Size: 347.4 KB (347396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2200bb913588eec8e0699f2e40428f174bb7e107b5f34df6c1bc18febde3df56`  
		Last Modified: Wed, 14 Jun 2023 21:57:15 GMT  
		Size: 8.8 MB (8777234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eef527b5cb2cd0efcc4dd510e0f5070bbea938367fdfc11f4bce1a2523957fb`  
		Last Modified: Wed, 14 Jun 2023 21:57:14 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed966ebe9894672f0995d8cd2c7d455b36648e516d7fa248497584b3ed99fc96`  
		Last Modified: Wed, 14 Jun 2023 21:57:14 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.18` - linux; 386

```console
$ docker pull redis@sha256:55570f1c12eeb5586f85c4ee84f6b53e28692383d821564b43b4dbd051a70698
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11903564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c912c6df827464a9cb026f60b3b8c19afc048ede91ed2f19cf1bd28b0c5f47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:22 GMT
ADD file:94bec00e2c0c7f47c81ec4355a29ca23a81b439797d037b1a5a455f36a25dab4 in / 
# Wed, 14 Jun 2023 22:33:22 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 01:55:06 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Jun 2023 01:55:08 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 15 Jun 2023 01:58:37 GMT
ENV REDIS_VERSION=7.0.11
# Thu, 15 Jun 2023 01:58:37 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Thu, 15 Jun 2023 01:58:37 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Thu, 15 Jun 2023 01:59:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 15 Jun 2023 01:59:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 15 Jun 2023 01:59:48 GMT
VOLUME [/data]
# Thu, 15 Jun 2023 01:59:48 GMT
WORKDIR /data
# Thu, 15 Jun 2023 01:59:48 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:59:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 01:59:49 GMT
EXPOSE 6379
# Thu, 15 Jun 2023 01:59:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b3f50075abd13aad1cb7d8c1427aa59d7fcac88f3690d3f9c3efdbec80fd0856`  
		Last Modified: Wed, 14 Jun 2023 22:33:48 GMT  
		Size: 3.2 MB (3233951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6d1ca2a803d962ff3107f2190d003a1083748cfff0190a56276cc79709f0e`  
		Last Modified: Thu, 15 Jun 2023 02:05:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d97ba838e6b32bc51819f85a24fc31141ac04f0eb0901069ed4189c542053e6`  
		Last Modified: Thu, 15 Jun 2023 02:05:49 GMT  
		Size: 347.2 KB (347161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050ec3d0fd4085a1e3226794a6e7b521faa5b0b02c83d6730afb7dc3269a2401`  
		Last Modified: Thu, 15 Jun 2023 02:06:32 GMT  
		Size: 8.3 MB (8320472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2895d299d436c4a8e7776e0b8064e0967a944b69c6e69b9cad29d6e10f05e9`  
		Last Modified: Thu, 15 Jun 2023 02:06:30 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69da833fa759fc45c8b7fd4802d9831d77aae40ed6aa552a7f4e4aa9fe104826`  
		Last Modified: Thu, 15 Jun 2023 02:06:30 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.18` - linux; ppc64le

```console
$ docker pull redis@sha256:1885bc119bd0602cd5cf83e8deb747667c9c66a9b0c1eef230a26b99f8ae1415
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 MB (12965935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d863c571d52e8c007ed8bb3931dc887e928ed7f440f4a6e7e07c88f357584e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 15 Jun 2023 00:39:49 GMT
ADD file:694c636c0dd19fd01accbc189e4c1dc4d063952692c6e7eb26dce02a7adba833 in / 
# Thu, 15 Jun 2023 00:39:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 07:47:12 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Jun 2023 07:47:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 15 Jun 2023 07:48:38 GMT
ENV REDIS_VERSION=7.0.11
# Thu, 15 Jun 2023 07:48:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Thu, 15 Jun 2023 07:48:39 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Thu, 15 Jun 2023 07:49:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 15 Jun 2023 07:49:42 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 15 Jun 2023 07:49:43 GMT
VOLUME [/data]
# Thu, 15 Jun 2023 07:49:44 GMT
WORKDIR /data
# Thu, 15 Jun 2023 07:49:46 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:49:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Jun 2023 07:49:50 GMT
EXPOSE 6379
# Thu, 15 Jun 2023 07:49:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ffa4a466dbb8eebd7e7f25590a9df12390de9016abf82279c29c9a64aa76491a`  
		Last Modified: Thu, 15 Jun 2023 00:40:26 GMT  
		Size: 3.3 MB (3344781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfef8da4bad204314ce5c08ffe4620ccefd95e9b724ddd53c028c9b9c86879f`  
		Last Modified: Thu, 15 Jun 2023 07:53:07 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fac12ef80ade293e23b345b9b7e14d4ca00aa21553600d4cec21afeb0cc848e`  
		Last Modified: Thu, 15 Jun 2023 07:53:07 GMT  
		Size: 347.4 KB (347436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8a82be6a1234c8ba8427c16e3efc8d480797c96df99bd0a69b3a546c114cdd`  
		Last Modified: Thu, 15 Jun 2023 07:53:27 GMT  
		Size: 9.3 MB (9271734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b881a951700a56910f20b52d513ee7477c884f0394e1559b07e7f97e91eaad7d`  
		Last Modified: Thu, 15 Jun 2023 07:53:25 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b090785b020e0faae24b6db2126fe7a7c6b4c6d5885d4d0acaa35f6221cab743`  
		Last Modified: Thu, 15 Jun 2023 07:53:25 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.18` - linux; s390x

```console
$ docker pull redis@sha256:b2c85d4a6bc070d4cb737123bd8326693c133e228244ad1cb7a2490d034f048b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.5 MB (12469007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e668065926afe408d4d607aa224a9be828b71b15aefafd1b4964bb49042202`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 21:07:48 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 11 May 2023 21:07:49 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 11 May 2023 21:08:50 GMT
ENV REDIS_VERSION=7.0.11
# Thu, 11 May 2023 21:08:50 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Thu, 11 May 2023 21:08:50 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Thu, 11 May 2023 21:09:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 11 May 2023 21:09:36 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 11 May 2023 21:09:36 GMT
VOLUME [/data]
# Thu, 11 May 2023 21:09:37 GMT
WORKDIR /data
# Thu, 11 May 2023 21:09:37 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Thu, 11 May 2023 21:09:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 21:09:38 GMT
EXPOSE 6379
# Thu, 11 May 2023 21:09:38 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1b6d6587d4123810e8827e4196db74ceaa3a8a13dfb2b7fdf1d10a34db38ec`  
		Last Modified: Thu, 11 May 2023 21:12:09 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a20274bd6520a3597212b087d3ebb797a0fedfa01189b2e3587f6b947885d19`  
		Last Modified: Thu, 11 May 2023 21:12:09 GMT  
		Size: 347.2 KB (347151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785bdedc050f98a32fad7c6b263c45958722dff3530635792e1a5f4b85352a08`  
		Last Modified: Thu, 11 May 2023 21:12:22 GMT  
		Size: 8.9 MB (8893567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db78241e19d937be4a667c8c31496146ae6bf4d2f38f00cea0b8e419057eb899`  
		Last Modified: Thu, 11 May 2023 21:12:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ced6ab032e05d37f5736888cdfeca47e6f1e5e7124409393c058d761212d5a0`  
		Last Modified: Thu, 11 May 2023 21:12:21 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
