## `redis:6-alpine`

```console
$ docker pull redis@sha256:cd8f1488883b8b5e59f0cce2aaa85d235e8718026038482a0e392924adf57dc4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redis:6-alpine` - linux; amd64

```console
$ docker pull redis@sha256:4024a293fbc2ef958aa307753796ba55af7bac513cf8e24dcb8b78155f927a64
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10890055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb4fa30f1cfbbf7a637818d1e8de048e3c3d67421c0e2fdae4ca951c3944fed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:38:17 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Apr 2021 02:38:20 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 03 May 2021 22:56:46 GMT
ENV REDIS_VERSION=6.2.3
# Mon, 03 May 2021 22:56:46 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.3.tar.gz
# Mon, 03 May 2021 22:56:46 GMT
ENV REDIS_DOWNLOAD_SHA=98ed7d532b5e9671f5df0825bb71f0f37483a16546364049384c63db8764512b
# Mon, 03 May 2021 22:57:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 03 May 2021 22:57:48 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 03 May 2021 22:57:48 GMT
VOLUME [/data]
# Mon, 03 May 2021 22:57:48 GMT
WORKDIR /data
# Mon, 03 May 2021 22:57:48 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 03 May 2021 22:57:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 May 2021 22:57:49 GMT
EXPOSE 6379
# Mon, 03 May 2021 22:57:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712d301e8c43bcd4a36da8a8297d5ff7f68c3d4c3f7113244ff03675fa5e9c`  
		Last Modified: Thu, 15 Apr 2021 02:45:21 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8173c12df40f1578a7b2dfbbc0034a4fbc8ec7c870fd32b9236c2e5e1936616a`  
		Last Modified: Thu, 15 Apr 2021 02:45:22 GMT  
		Size: 384.2 KB (384200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77b7ddf4978e74801910f33e5b5b6dd49a4123ef5f93eb2a419e8cc496c24fd`  
		Last Modified: Mon, 03 May 2021 23:01:25 GMT  
		Size: 7.7 MB (7692081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f34a000c6b3a144334a7c4ba90caffacb7c73a5557337c4a08acaac6e8fc38e`  
		Last Modified: Mon, 03 May 2021 23:01:24 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275dfaedaf416be62086875c60fcec4dbe22ab9defd2ed306f2709a2985f1b23`  
		Last Modified: Mon, 03 May 2021 23:01:24 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:998a3d4de8d99a136d5d6852c5bb4e2980740dc390519bdaa7b4c334da9af116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10588534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa64ea8c3eb72397f6875b958db512ed20be26437ac474b3db7bc9ccbd7488d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 02 Jun 2021 00:13:00 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 02 Jun 2021 00:13:02 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 02 Jun 2021 00:13:03 GMT
ENV REDIS_VERSION=6.2.4
# Wed, 02 Jun 2021 00:13:03 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Wed, 02 Jun 2021 00:13:03 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Wed, 02 Jun 2021 00:15:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 02 Jun 2021 00:15:02 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 02 Jun 2021 00:15:02 GMT
VOLUME [/data]
# Wed, 02 Jun 2021 00:15:02 GMT
WORKDIR /data
# Wed, 02 Jun 2021 00:15:02 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 02 Jun 2021 00:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 00:15:03 GMT
EXPOSE 6379
# Wed, 02 Jun 2021 00:15:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c0c5f8e720bcd1e5844ff44994ab50cb78f45b2b227ddc71992945d5b183bc`  
		Last Modified: Wed, 02 Jun 2021 00:20:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771bb6fda7067bc5f684288009da843d2d5d43da94007162224ce0d878320acf`  
		Last Modified: Wed, 02 Jun 2021 00:20:31 GMT  
		Size: 388.1 KB (388122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab01c9b7eb1a74489582bab505fca4340cb946f470115bb1f1cbb8d01cfbda9`  
		Last Modified: Wed, 02 Jun 2021 00:20:33 GMT  
		Size: 7.6 MB (7576474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdaedffadf19b435f77091954a988fce50895da799375a686fb1745e77caa59d`  
		Last Modified: Wed, 02 Jun 2021 00:20:31 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8099c3b7dda9f80999f4a89463cd850012660d8fadf4ea5cf7313cb65d693f79`  
		Last Modified: Wed, 02 Jun 2021 00:20:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:5b22718342af650c68d5fe7fe0423e02bc86f3dba1638d38e9118a13385af7f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10261724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38b6aafd848f2f9e7b4955be3e65c14c5e4b2144d0ed783a50390fa7dd92d53e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 05:53:00 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Apr 2021 05:53:04 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 04 May 2021 00:41:08 GMT
ENV REDIS_VERSION=6.2.3
# Tue, 04 May 2021 00:41:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.3.tar.gz
# Tue, 04 May 2021 00:41:09 GMT
ENV REDIS_DOWNLOAD_SHA=98ed7d532b5e9671f5df0825bb71f0f37483a16546364049384c63db8764512b
# Tue, 04 May 2021 00:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 04 May 2021 00:42:07 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 04 May 2021 00:42:08 GMT
VOLUME [/data]
# Tue, 04 May 2021 00:42:09 GMT
WORKDIR /data
# Tue, 04 May 2021 00:42:09 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 04 May 2021 00:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:42:11 GMT
EXPOSE 6379
# Tue, 04 May 2021 00:42:12 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a20589517e54a354da5d6cb4ea2d35203508b772c35d104b5003a9dd0f2a017`  
		Last Modified: Thu, 15 Apr 2021 05:57:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a8858422eeb975991be458833e2120b9fadbfacfb3530991f0e972c3370bb2`  
		Last Modified: Thu, 15 Apr 2021 05:57:37 GMT  
		Size: 383.0 KB (383040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9aa6d5351c128c031daf8532fd301536c3bed73c6bb172e5408f371e2af5bd8`  
		Last Modified: Tue, 04 May 2021 00:46:26 GMT  
		Size: 7.5 MB (7452731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd63bc4c0d244d6c15e49d8e774eb165113dbb8b40d0438b3a0fe7067ae762`  
		Last Modified: Tue, 04 May 2021 00:46:24 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871101b0b381b35ca932cb3aadc2a28751d141488b2bee14207d35901ac0b137`  
		Last Modified: Tue, 04 May 2021 00:46:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:8ed02f26fdef83b5089b0a83e93e5f0e74640d7754bd4fde2177b933e35f7c45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.8 MB (10798767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05ec8efb4eccd68f8ee73442b61895d1bcaa5ee9687d96f9e6561645496db46c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:14:24 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Apr 2021 07:14:28 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 03 May 2021 23:23:22 GMT
ENV REDIS_VERSION=6.2.3
# Mon, 03 May 2021 23:23:24 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.3.tar.gz
# Mon, 03 May 2021 23:23:25 GMT
ENV REDIS_DOWNLOAD_SHA=98ed7d532b5e9671f5df0825bb71f0f37483a16546364049384c63db8764512b
# Mon, 03 May 2021 23:24:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 03 May 2021 23:24:27 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 03 May 2021 23:24:28 GMT
VOLUME [/data]
# Mon, 03 May 2021 23:24:29 GMT
WORKDIR /data
# Mon, 03 May 2021 23:24:29 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 03 May 2021 23:24:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 May 2021 23:24:31 GMT
EXPOSE 6379
# Mon, 03 May 2021 23:24:32 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f009ede80a4dfb2942ae27d15f3cd96afc249851ba83171edb51346d9e3d975`  
		Last Modified: Thu, 15 Apr 2021 07:19:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea11b4c6f734c1273155ea086da36c719ee65817775dd2a2d3c57cbd531da18`  
		Last Modified: Thu, 15 Apr 2021 07:19:25 GMT  
		Size: 386.0 KB (386003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf7461c80f0c2807e9f8afca98e4ecd0ec0376cab377f76f1906f1dc8071dcb`  
		Last Modified: Mon, 03 May 2021 23:28:41 GMT  
		Size: 7.7 MB (7698932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9dffae7b486cb18ed3632dbb51e17ae6f3cb9a0a4397f1fe937efe6c90634d`  
		Last Modified: Mon, 03 May 2021 23:28:38 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc099b6de0a1f6e273589f39cd0cec63644a2fbedd3b99f3ebf64eb1c929f3c`  
		Last Modified: Mon, 03 May 2021 23:28:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; 386

```console
$ docker pull redis@sha256:858da560de4602625d8c7f5a2cc80ff538fc63160cafe3b29e43c9a0b904acfa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10552928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ef3f645624c33905da6ebd8a17a6552a7869ee3c022ad8da35506667a18382`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:39:44 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Apr 2021 06:39:46 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 03 May 2021 23:04:20 GMT
ENV REDIS_VERSION=6.2.3
# Mon, 03 May 2021 23:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.3.tar.gz
# Mon, 03 May 2021 23:04:21 GMT
ENV REDIS_DOWNLOAD_SHA=98ed7d532b5e9671f5df0825bb71f0f37483a16546364049384c63db8764512b
# Mon, 03 May 2021 23:05:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 03 May 2021 23:05:37 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 03 May 2021 23:05:38 GMT
VOLUME [/data]
# Mon, 03 May 2021 23:05:38 GMT
WORKDIR /data
# Mon, 03 May 2021 23:05:38 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 03 May 2021 23:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 May 2021 23:05:38 GMT
EXPOSE 6379
# Mon, 03 May 2021 23:05:39 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583b1dfa7a770c1329627c5050294279e947bfeba04c300716518c315d1080eb`  
		Last Modified: Thu, 15 Apr 2021 06:45:05 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e736134af79a478b22deba2ad536f80ae78c0cb383a88d66c2c1c5460fcc1a`  
		Last Modified: Thu, 15 Apr 2021 06:45:05 GMT  
		Size: 390.6 KB (390571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2205ff6323d34af38baeb9324c1c1ad7c913a0eabce8bee54ec1cb8adbfdcda`  
		Last Modified: Mon, 03 May 2021 23:10:35 GMT  
		Size: 7.3 MB (7341656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a1a2af4107ba5c65e0895e8c0e078789d9fbec6223de4bbc4b514164838bf`  
		Last Modified: Mon, 03 May 2021 23:10:33 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad42ca34d6b528349729376810677106866f67d60895717326bbeed0cd9a00`  
		Last Modified: Mon, 03 May 2021 23:10:33 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:e74e5a566b36993e76fbd1c737f89f10022db5a03fcd695a218b105ece5f50c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11414012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f455ab4358d4533c5229304aafab4aefc8bf16143fd89e5c6a9d97d1f1f8948a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:55:53 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Apr 2021 07:56:17 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 02 Jun 2021 01:47:07 GMT
ENV REDIS_VERSION=6.2.4
# Wed, 02 Jun 2021 01:47:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Wed, 02 Jun 2021 01:47:21 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Wed, 02 Jun 2021 01:48:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 02 Jun 2021 01:48:56 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 02 Jun 2021 01:49:02 GMT
VOLUME [/data]
# Wed, 02 Jun 2021 01:49:10 GMT
WORKDIR /data
# Wed, 02 Jun 2021 01:49:12 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 02 Jun 2021 01:49:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Jun 2021 01:49:21 GMT
EXPOSE 6379
# Wed, 02 Jun 2021 01:49:27 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846316a488fa621585c7f8607349cf8717e3025cda80dff5a9d73b1761f4c808`  
		Last Modified: Thu, 15 Apr 2021 08:05:10 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963ad60821f381aebcf57e783a69acea22d4bd86e88ebed8b3ce177afe64012f`  
		Last Modified: Thu, 15 Apr 2021 08:05:10 GMT  
		Size: 390.7 KB (390721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc37e000c9f0ebca59cc8b3aae911a50fe23ae4d3b02b82a87bf14f7d561a992`  
		Last Modified: Wed, 02 Jun 2021 01:59:51 GMT  
		Size: 8.2 MB (8208332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11f91cd575121f2b2889fea5cc86d33f59f3828bd7e52deeeb3da2ee9f3a11c`  
		Last Modified: Wed, 02 Jun 2021 01:59:49 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27e68d72a86c541053baa17a4a3403833bc85b9fd1b604fa2e49031f8c449a3`  
		Last Modified: Wed, 02 Jun 2021 01:59:48 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; s390x

```console
$ docker pull redis@sha256:a3b500f716c99bddf4eacb364fda277bc823a0864730387ff37c6c5919d518a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11006227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1749be9c7a2f2f534193ae2ec8b7054a8ded370f3a1cb1b999b1fdc2560733d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:57:34 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 15 Apr 2021 06:57:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 03 May 2021 23:45:59 GMT
ENV REDIS_VERSION=6.2.3
# Mon, 03 May 2021 23:46:00 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.3.tar.gz
# Mon, 03 May 2021 23:46:00 GMT
ENV REDIS_DOWNLOAD_SHA=98ed7d532b5e9671f5df0825bb71f0f37483a16546364049384c63db8764512b
# Mon, 03 May 2021 23:46:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 03 May 2021 23:47:00 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 03 May 2021 23:47:00 GMT
VOLUME [/data]
# Mon, 03 May 2021 23:47:00 GMT
WORKDIR /data
# Mon, 03 May 2021 23:47:01 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 03 May 2021 23:47:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 03 May 2021 23:47:02 GMT
EXPOSE 6379
# Mon, 03 May 2021 23:47:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301b8855bd6607f74a6f0e494262a313b941546f676be3a98ff67cb3921a975`  
		Last Modified: Thu, 15 Apr 2021 07:01:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e8e413247eebdfc21ae64af7664f78b06ca050ca165a1734e375c5db4ee9fd`  
		Last Modified: Thu, 15 Apr 2021 07:01:07 GMT  
		Size: 388.8 KB (388827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e91698f66e268d97c91886a4136fe36e85e04bcd33be57b14523edf7ce22973`  
		Last Modified: Mon, 03 May 2021 23:50:42 GMT  
		Size: 8.0 MB (8012940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03906c09c9c38370eee6c0aec862aa63ac640abdfa64ad39cdd0586e09a9670`  
		Last Modified: Mon, 03 May 2021 23:50:40 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5233bd3a72deb9a34c7b6d837a7420e9882caa0e020456f9bd7045cfe5f4832`  
		Last Modified: Mon, 03 May 2021 23:50:41 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
