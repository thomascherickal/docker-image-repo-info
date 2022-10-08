## `redis:7-alpine3.16`

```console
$ docker pull redis@sha256:cbb77cfe5c69b1d5aba8750d428624b7fe2cbe0d7761838e81f3caa82b852e0f
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
$ docker pull redis@sha256:f0d4e9e7a59a94e096e22b825545d8dc1a04f501a9fff9dbb25c9d15dad19d16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11852242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d29f18e8bc92c5bd50db90a1dd37d8c62bb26220088ae9d97b4b07691f4e5641`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 03:30:17 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 07 Oct 2022 03:30:18 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 07 Oct 2022 03:30:18 GMT
ENV REDIS_VERSION=7.0.5
# Fri, 07 Oct 2022 03:30:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.5.tar.gz
# Fri, 07 Oct 2022 03:30:19 GMT
ENV REDIS_DOWNLOAD_SHA=67054cc37b58c125df93bd78000261ec0ef4436a26b40f38262c780e56315cc3
# Fri, 07 Oct 2022 03:31:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 07 Oct 2022 03:31:05 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 07 Oct 2022 03:31:05 GMT
VOLUME [/data]
# Fri, 07 Oct 2022 03:31:05 GMT
WORKDIR /data
# Fri, 07 Oct 2022 03:31:05 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:31:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 03:31:06 GMT
EXPOSE 6379
# Fri, 07 Oct 2022 03:31:06 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb541f77610a7550755893b11853752742e9b173e4e9967f4db6b02c2e51ce4a`  
		Last Modified: Fri, 07 Oct 2022 03:34:32 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e3041aaa57579fe87bf26fbb56fcf7aef49b3f5a0e0ee37eab519855dd37e`  
		Last Modified: Fri, 07 Oct 2022 03:34:32 GMT  
		Size: 398.4 KB (398361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadae582a31f5fd67d2286cecf95c4045d2c9828c73dd7ffe8a866d7df916cff`  
		Last Modified: Fri, 07 Oct 2022 03:34:34 GMT  
		Size: 8.6 MB (8645843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996b5def187670b227d8b6c6081c0d35a03d4d95bbfd96c005fa9fd9204b97af`  
		Last Modified: Fri, 07 Oct 2022 03:34:32 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed3be2507e6c47aa154ced68ba7f7d2f8f455ac36d73a898af748663ebbe42f`  
		Last Modified: Fri, 07 Oct 2022 03:34:32 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm variant v6

```console
$ docker pull redis@sha256:4561a6acbcf917432514effc5ff5f0d5e0bbb0b8cb379fcd5fe96c1b03801e7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11781787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5f708c3342138d8579357cf6051f9e713ab7edb72bfa64a26ba7fc72fcda1bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 02:44:55 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 08 Oct 2022 02:44:57 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 08 Oct 2022 02:44:57 GMT
ENV REDIS_VERSION=7.0.5
# Sat, 08 Oct 2022 02:44:58 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.5.tar.gz
# Sat, 08 Oct 2022 02:44:58 GMT
ENV REDIS_DOWNLOAD_SHA=67054cc37b58c125df93bd78000261ec0ef4436a26b40f38262c780e56315cc3
# Sat, 08 Oct 2022 02:47:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 08 Oct 2022 02:47:25 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 08 Oct 2022 02:47:25 GMT
VOLUME [/data]
# Sat, 08 Oct 2022 02:47:25 GMT
WORKDIR /data
# Sat, 08 Oct 2022 02:47:25 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 08 Oct 2022 02:47:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 02:47:26 GMT
EXPOSE 6379
# Sat, 08 Oct 2022 02:47:26 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f8d457f34c4d13164cdc05fef95519fae7e0c22d2389c0c4daf804e0f757ee`  
		Last Modified: Sat, 08 Oct 2022 02:56:01 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b67d8c154e248c8dcc9b21c8f4f07834a7ecf01b57daf9aad0985a4cdec83c`  
		Last Modified: Sat, 08 Oct 2022 02:56:02 GMT  
		Size: 403.1 KB (403059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b4ad11dd248e482dad5e7ff86147b53092887f10b0988c8c1fd0706093c01`  
		Last Modified: Sat, 08 Oct 2022 02:56:03 GMT  
		Size: 8.8 MB (8762776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f31e3deed0eb46d0f165ab7e04bfba708090a949ad21f19957b411a9730feaec`  
		Last Modified: Sat, 08 Oct 2022 02:56:01 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabf265627e8b8dba6afe039bb45a8ba3072e19c9c2c4b41131e99a1cdacb0e5`  
		Last Modified: Sat, 08 Oct 2022 02:56:01 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm variant v7

```console
$ docker pull redis@sha256:8ca9439b392fdcd2575b979c57631728e63e8726e354eebf8332b2e5bc0d9fea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.5 MB (11453796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896788178bad661fbbf299c2d5a118f8f5a6ee07e4399d0e377db79a5772090b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Sat, 08 Oct 2022 03:47:01 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 08 Oct 2022 03:47:03 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 08 Oct 2022 03:47:03 GMT
ENV REDIS_VERSION=7.0.5
# Sat, 08 Oct 2022 03:47:03 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.5.tar.gz
# Sat, 08 Oct 2022 03:47:03 GMT
ENV REDIS_DOWNLOAD_SHA=67054cc37b58c125df93bd78000261ec0ef4436a26b40f38262c780e56315cc3
# Sat, 08 Oct 2022 03:49:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 08 Oct 2022 03:49:36 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 08 Oct 2022 03:49:36 GMT
VOLUME [/data]
# Sat, 08 Oct 2022 03:49:36 GMT
WORKDIR /data
# Sat, 08 Oct 2022 03:49:37 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 08 Oct 2022 03:49:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 03:49:37 GMT
EXPOSE 6379
# Sat, 08 Oct 2022 03:49:37 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d433ba043811b3896fd18d316cd101a62eea4ce5da0633fe975cc7fba8f83bc`  
		Last Modified: Sat, 08 Oct 2022 03:58:23 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b44aedfa9edc5317427d2bfb96e3ef30b895bf9980149f9d69b764928bc731`  
		Last Modified: Sat, 08 Oct 2022 03:58:23 GMT  
		Size: 396.7 KB (396683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f7f7bac927117901aa00902f10eba1099eadc3880dfbffd3ead3f1550e8c60`  
		Last Modified: Sat, 08 Oct 2022 03:58:25 GMT  
		Size: 8.6 MB (8638062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f2647b0ad90363975990f22d91bd381e6a7818dc3633c0e13658699e6d9ad`  
		Last Modified: Sat, 08 Oct 2022 03:58:23 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e0e504f60251d44929431a38b78d1edbcf5699c78c584bb8d8520af316e1ad`  
		Last Modified: Sat, 08 Oct 2022 03:58:23 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:6d41c1db47e02fb882a303f2d2f5c2492b7f9e7ce3d8f1dbbebce4ee9f13a75e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11891034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06a6b2d1798c603c662ee524cb2d7490cea84e828fc109d06007ff42586aa0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 06:56:01 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 07 Oct 2022 06:56:03 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 07 Oct 2022 06:56:04 GMT
ENV REDIS_VERSION=7.0.5
# Fri, 07 Oct 2022 06:56:05 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.5.tar.gz
# Fri, 07 Oct 2022 06:56:06 GMT
ENV REDIS_DOWNLOAD_SHA=67054cc37b58c125df93bd78000261ec0ef4436a26b40f38262c780e56315cc3
# Fri, 07 Oct 2022 06:56:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 07 Oct 2022 06:56:56 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 07 Oct 2022 06:56:57 GMT
VOLUME [/data]
# Fri, 07 Oct 2022 06:56:58 GMT
WORKDIR /data
# Fri, 07 Oct 2022 06:57:00 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Fri, 07 Oct 2022 06:57:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 06:57:01 GMT
EXPOSE 6379
# Fri, 07 Oct 2022 06:57:02 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bae97b19a6b5b2019c83e13b160b460852b3565994fe6cc58dd00374ec2ae4`  
		Last Modified: Fri, 07 Oct 2022 07:02:02 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9014ee1b9e39e295d8ae69ccfbb536c9c453b706e59718d163ff72cbefc2c8`  
		Last Modified: Fri, 07 Oct 2022 07:02:03 GMT  
		Size: 399.9 KB (399855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2012cc160433e057a6623ca2c65baae3100ae39c8a42d89e67d8ef95dfe4ec4`  
		Last Modified: Fri, 07 Oct 2022 07:02:04 GMT  
		Size: 8.8 MB (8781595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4094aa30e72601df0699906b7a7fe0f22982927d3ae7d2915750af46b731dea`  
		Last Modified: Fri, 07 Oct 2022 07:02:02 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb7bfccd4557d8a3e9b7bb2f64c0bac028fbcda1c65ef22a297e25867ecf635`  
		Last Modified: Fri, 07 Oct 2022 07:02:02 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; 386

```console
$ docker pull redis@sha256:6af92c911d79fa329b550c37ae94bd937940a12b42f2b6a44a23982cdfea7c52
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.5 MB (11493922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21148e102efc9ca50215a9a05fe6c8d4dc45d34d36c3ec029325a842530bc22f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:29:08 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 07 Oct 2022 01:29:10 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 07 Oct 2022 01:29:11 GMT
ENV REDIS_VERSION=7.0.5
# Fri, 07 Oct 2022 01:29:12 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.5.tar.gz
# Fri, 07 Oct 2022 01:29:13 GMT
ENV REDIS_DOWNLOAD_SHA=67054cc37b58c125df93bd78000261ec0ef4436a26b40f38262c780e56315cc3
# Fri, 07 Oct 2022 01:30:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 07 Oct 2022 01:30:05 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 07 Oct 2022 01:30:06 GMT
VOLUME [/data]
# Fri, 07 Oct 2022 01:30:07 GMT
WORKDIR /data
# Fri, 07 Oct 2022 01:30:09 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Fri, 07 Oct 2022 01:30:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 01:30:10 GMT
EXPOSE 6379
# Fri, 07 Oct 2022 01:30:11 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d753ce7cb7a86176e409fbfed496fbb078d63cd34a5a2c43d5b99a516a11a2c`  
		Last Modified: Fri, 07 Oct 2022 01:35:18 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0890d9a205e664751060d4f2103b2213496b1be5f109712b8a91a7c9b9c5641`  
		Last Modified: Fri, 07 Oct 2022 01:35:19 GMT  
		Size: 405.3 KB (405262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9cfb2dce18ae2e7c2ca7e98936bb98de15016324f772fea1297d3f19b46962`  
		Last Modified: Fri, 07 Oct 2022 01:35:19 GMT  
		Size: 8.3 MB (8279615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efa1599faac16aef38914cde734aa6548d9e628d335a66c43f8412c21f0f2aa`  
		Last Modified: Fri, 07 Oct 2022 01:35:18 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea7ba9878e263c279778f9a557265e8720e488f2715ecd95b2bf4fbc82eb78d`  
		Last Modified: Fri, 07 Oct 2022 01:35:18 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; ppc64le

```console
$ docker pull redis@sha256:ada550f440aca880360e26e886f4011eb029a366b0f6842e688b928033a13795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.5 MB (12470454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6611b778498284c5fb047cd29ec1ea377e74ed440c9854291db37bd45e81d53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 06:53:34 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 07 Oct 2022 06:53:37 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 07 Oct 2022 06:53:37 GMT
ENV REDIS_VERSION=7.0.5
# Fri, 07 Oct 2022 06:53:38 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.5.tar.gz
# Fri, 07 Oct 2022 06:53:38 GMT
ENV REDIS_DOWNLOAD_SHA=67054cc37b58c125df93bd78000261ec0ef4436a26b40f38262c780e56315cc3
# Fri, 07 Oct 2022 06:54:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 07 Oct 2022 06:54:42 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 07 Oct 2022 06:54:42 GMT
VOLUME [/data]
# Fri, 07 Oct 2022 06:54:43 GMT
WORKDIR /data
# Fri, 07 Oct 2022 06:54:43 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Fri, 07 Oct 2022 06:54:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 06:54:44 GMT
EXPOSE 6379
# Fri, 07 Oct 2022 06:54:44 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a40cf9cbcba26de4ca6c60a1af02dfa33aaf568aa79bebaed1e686245b267d4`  
		Last Modified: Fri, 07 Oct 2022 07:00:21 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04762a605fa4de733e39087992868566a08896e7b6956799265cb96da6c75cf5`  
		Last Modified: Fri, 07 Oct 2022 07:00:21 GMT  
		Size: 405.7 KB (405686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c817001953154e19408a8d0d48747ba0b743d4f4423df9d1771047a10b153a`  
		Last Modified: Fri, 07 Oct 2022 07:00:23 GMT  
		Size: 9.3 MB (9259462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc104fb4e03bb315ef23bb9618b486a81621bcda67dcec8c4a36b131c18aad22`  
		Last Modified: Fri, 07 Oct 2022 07:00:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c822ce2a14090c9a31629bbf02d78ebfce083a7ce32d4a23d16e5b8f8118fca8`  
		Last Modified: Fri, 07 Oct 2022 07:00:21 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; s390x

```console
$ docker pull redis@sha256:91c96b3824cff244837c9f971e6544d9336144e450cabe6f17c66c83ec56bb8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11906848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50892674c23eff3b6561aabd11834793c99619ea4532ed4ea57691001b383bd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:12:54 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 07 Oct 2022 09:12:56 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 07 Oct 2022 09:12:57 GMT
ENV REDIS_VERSION=7.0.5
# Fri, 07 Oct 2022 09:12:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.5.tar.gz
# Fri, 07 Oct 2022 09:12:57 GMT
ENV REDIS_DOWNLOAD_SHA=67054cc37b58c125df93bd78000261ec0ef4436a26b40f38262c780e56315cc3
# Fri, 07 Oct 2022 09:14:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 07 Oct 2022 09:14:19 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 07 Oct 2022 09:14:20 GMT
VOLUME [/data]
# Fri, 07 Oct 2022 09:14:20 GMT
WORKDIR /data
# Fri, 07 Oct 2022 09:14:21 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Fri, 07 Oct 2022 09:14:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 09:14:22 GMT
EXPOSE 6379
# Fri, 07 Oct 2022 09:14:23 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c89dcae123a65a4e164a34eaf9b3ccc50b2fd8a8228af00834ca5e7f8628f5`  
		Last Modified: Fri, 07 Oct 2022 09:21:11 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8541131b18b68d1c61a45d2b77f6050a82cc3900bc0a17fa34c872cc47aff9b4`  
		Last Modified: Fri, 07 Oct 2022 09:21:11 GMT  
		Size: 403.8 KB (403777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee7abf818bbf79023251136e85f0382147d152e8a5faabd5adc2562b18c020c`  
		Last Modified: Fri, 07 Oct 2022 09:21:13 GMT  
		Size: 8.9 MB (8910486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d852063873733637008b64a29bd7e7bd2ea9857333410ddeb99088ea50297a`  
		Last Modified: Fri, 07 Oct 2022 09:21:11 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fe44e7585be0f1e0de787e49a32786bc7014f77387282db5714e83fb62b45a`  
		Last Modified: Fri, 07 Oct 2022 09:21:12 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
