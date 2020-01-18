## `redis:rc-alpine3.11`

```console
$ docker pull redis@sha256:a0a282c2699db44b0b6253ac8c31d0926cc2f87403aae798e93472a8edc3d04c
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

### `redis:rc-alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:355a7c41f562c8b0a1db4e5139284da6012c01118d0e11725a6f5c045bd3ded1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10522568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e78e36b108877d0f79b594fbdd8bfb6f1855883d00d83f793f401e7fcf047fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:15:28 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 04:15:29 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 18 Jan 2020 04:15:30 GMT
ENV REDIS_VERSION=6.0-rc1
# Sat, 18 Jan 2020 04:15:30 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc1.tar.gz
# Sat, 18 Jan 2020 04:15:30 GMT
ENV REDIS_DOWNLOAD_SHA=2676012e2fcfe8d41e594b2ae8a05d0a050d2d84c38a0471ae5fe0143e4b0eca
# Sat, 18 Jan 2020 04:16:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 04:16:27 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 04:16:27 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 04:16:27 GMT
WORKDIR /data
# Sat, 18 Jan 2020 04:16:27 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:16:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:16:28 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 04:16:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd5e7a0ba4adb7c7ae1c7d68b7d188015d166d9510d7439fd29ed78bbd95970`  
		Last Modified: Sat, 18 Jan 2020 04:19:10 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20c1cdf5aefec6df08568a3dd0b1207350b1a877a5d50f494b05195159a82e9`  
		Last Modified: Sat, 18 Jan 2020 04:19:11 GMT  
		Size: 402.6 KB (402564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8f18e6b0814d7de90e6254f57ae4bf09a2bd109aaf420c4a268159a47c9f29`  
		Last Modified: Sat, 18 Jan 2020 04:19:16 GMT  
		Size: 7.3 MB (7315306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cdc4dbc57a49039305c206a77c71b7a63945317df7ce3172d3e175afc36c01`  
		Last Modified: Sat, 18 Jan 2020 04:19:11 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9183a2e122037808eb5dfbd8da63a270553b2c5227f7529cc8d10949b0185ef8`  
		Last Modified: Sat, 18 Jan 2020 04:19:10 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:7f9d32e045047c26e86e751c743b0416ecb86f4e4c582bf29de698b23a6fd99f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10229163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f808d3c0b849f87720923a1122a6d398007693fe99026fd1c5c63da7b21578`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:34:20 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 03:34:23 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 18 Jan 2020 03:34:24 GMT
ENV REDIS_VERSION=6.0-rc1
# Sat, 18 Jan 2020 03:34:24 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc1.tar.gz
# Sat, 18 Jan 2020 03:34:25 GMT
ENV REDIS_DOWNLOAD_SHA=2676012e2fcfe8d41e594b2ae8a05d0a050d2d84c38a0471ae5fe0143e4b0eca
# Sat, 18 Jan 2020 03:35:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 03:35:18 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 03:35:18 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 03:35:19 GMT
WORKDIR /data
# Sat, 18 Jan 2020 03:35:20 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:35:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:35:21 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 03:35:22 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e1ba208bc99e98b6e0f1a14d171c251bd7597b9f8d169ad10458d9019829d`  
		Last Modified: Sat, 18 Jan 2020 03:37:48 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43c4e1907d314e253637bc464a11ab0c74455326617093a1c33bf2b218d2e78`  
		Last Modified: Sat, 18 Jan 2020 03:37:48 GMT  
		Size: 405.8 KB (405799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310752bba1ae9a0bfcea536560b9d516a86e61861ccdaa92d36f7667168c37d8`  
		Last Modified: Sat, 18 Jan 2020 03:37:48 GMT  
		Size: 7.2 MB (7203998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e108416b142fc5a594a1ca37bedccf165ee1cdbce38df7818b899f64389561ef`  
		Last Modified: Sat, 18 Jan 2020 03:37:48 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916b4f2584fcf5694b92c50b590ff85ea71f8a9394116a4ad65c92601ad47a3b`  
		Last Modified: Sat, 18 Jan 2020 03:37:49 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:158eecdd3347fe3af17b0d758c6faddcf815b3838c8c7355e35ea18f458da566
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9895350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e657c0b3110f19b95e50f3b1ea20615e6e01b3d694c37b7549c6b1871dea9e00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:21:46 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 03:21:49 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 18 Jan 2020 03:21:50 GMT
ENV REDIS_VERSION=6.0-rc1
# Sat, 18 Jan 2020 03:21:51 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc1.tar.gz
# Sat, 18 Jan 2020 03:21:52 GMT
ENV REDIS_DOWNLOAD_SHA=2676012e2fcfe8d41e594b2ae8a05d0a050d2d84c38a0471ae5fe0143e4b0eca
# Sat, 18 Jan 2020 03:22:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 03:22:45 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 03:22:49 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 03:22:51 GMT
WORKDIR /data
# Sat, 18 Jan 2020 03:22:52 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:22:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:22:54 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 03:22:54 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4c25ff05240204c1b08c2fc7c9f092608801b1112a5563cc87c094d33b2610`  
		Last Modified: Sat, 18 Jan 2020 03:25:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5180ac18cf5d41359489200210414611b31a360dba3115a321dcb0ee7d036`  
		Last Modified: Sat, 18 Jan 2020 03:25:36 GMT  
		Size: 399.8 KB (399774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab714180afb2764a7d87c342e47ffbbc1f7e466d30299f8e744f1d170fd73b7`  
		Last Modified: Sat, 18 Jan 2020 03:25:38 GMT  
		Size: 7.1 MB (7074213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8533ac1eca6ed3106a146c2742ac4a0adf4badc405eb65fcea8c470af5a636f1`  
		Last Modified: Sat, 18 Jan 2020 03:25:36 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f225dc8e3dfceac4b4fb1bc03ff1a03cb327f176723cf61dd4270fed0312331f`  
		Last Modified: Sat, 18 Jan 2020 03:25:36 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:cdc4473ede49f410d8584ad115fea0a8a5abb8f56c03aa5efe9a8ded32e4522e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10440619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16cbf9ba623d72bc69b3bf5150755699d481948d228d768b888f2b6de7d3652a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:33:18 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 04:33:34 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 18 Jan 2020 04:33:44 GMT
ENV REDIS_VERSION=6.0-rc1
# Sat, 18 Jan 2020 04:33:52 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc1.tar.gz
# Sat, 18 Jan 2020 04:33:59 GMT
ENV REDIS_DOWNLOAD_SHA=2676012e2fcfe8d41e594b2ae8a05d0a050d2d84c38a0471ae5fe0143e4b0eca
# Sat, 18 Jan 2020 04:35:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 04:35:17 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 04:35:21 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 04:35:24 GMT
WORKDIR /data
# Sat, 18 Jan 2020 04:35:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:35:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:35:33 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 04:35:37 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b347d21af92f7fa1a81029304142b9a4f1fc27ab54133c379709546365755e28`  
		Last Modified: Sat, 18 Jan 2020 04:40:05 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efbca486ea0050d3522c6bb7c903b3f18ad83367fca11182ef98e5fe857aa19`  
		Last Modified: Sat, 18 Jan 2020 04:40:04 GMT  
		Size: 404.7 KB (404659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1416087f5568174fa3c23aa7d8c8d914f0a58215016e44a0db10ac4f6f52bcd9`  
		Last Modified: Sat, 18 Jan 2020 04:40:06 GMT  
		Size: 7.3 MB (7311075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d801b3d49d1016241e232273d67e594ce0cf389dae4b3d76e3a876dec4708e26`  
		Last Modified: Sat, 18 Jan 2020 04:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d152054c724a895770692e2084fe795fcf6def1678b1b795551ff268ae9d1d21`  
		Last Modified: Sat, 18 Jan 2020 04:40:04 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:b01d7785cd34a4fbe38842d0c8e73964d0171e5c308b43db63c2f226a9eddf49
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10208637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f35e983bd8d545f3cb59311bc1880b08a5a0632abcb835ed946e9a8de1aa0104`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 09:47:28 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 09:47:30 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 18 Jan 2020 09:47:30 GMT
ENV REDIS_VERSION=6.0-rc1
# Sat, 18 Jan 2020 09:47:30 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc1.tar.gz
# Sat, 18 Jan 2020 09:47:30 GMT
ENV REDIS_DOWNLOAD_SHA=2676012e2fcfe8d41e594b2ae8a05d0a050d2d84c38a0471ae5fe0143e4b0eca
# Sat, 18 Jan 2020 09:48:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 09:48:39 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 09:48:39 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 09:48:39 GMT
WORKDIR /data
# Sat, 18 Jan 2020 09:48:40 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 09:48:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 09:48:40 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 09:48:40 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919de76a1740b7c09172635adfe651ff8932cc9a10e907fe8c679f339d9d7f55`  
		Last Modified: Sat, 18 Jan 2020 09:51:38 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a79cec79577d23d585483773eb35aca3e0410ef04a2d46a680547bb670056f1`  
		Last Modified: Sat, 18 Jan 2020 09:51:38 GMT  
		Size: 407.9 KB (407903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3878bb3220ab24950a498653f11664c43eeb4b275eee9daa141b6263e996150`  
		Last Modified: Sat, 18 Jan 2020 09:51:40 GMT  
		Size: 7.0 MB (6992431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60d8e7e91fcaf3893347d78e68422dab401316f75f05c7268d66ccf65b9a3ba`  
		Last Modified: Sat, 18 Jan 2020 09:51:38 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8e81e1e3976b500e666ddc72666e9ff655b19e1989800d9be5c053c1230b0e`  
		Last Modified: Sat, 18 Jan 2020 09:51:38 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:f87e9761951909069f21b191f32d5dcff2808858ee9f579336696612f58460e6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11042745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:373e0932b48c9285e6770719594f5a24416d11c5aa126c6556c94a898fabb464`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:37:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 02:37:22 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 18 Jan 2020 02:37:25 GMT
ENV REDIS_VERSION=6.0-rc1
# Sat, 18 Jan 2020 02:37:26 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc1.tar.gz
# Sat, 18 Jan 2020 02:37:30 GMT
ENV REDIS_DOWNLOAD_SHA=2676012e2fcfe8d41e594b2ae8a05d0a050d2d84c38a0471ae5fe0143e4b0eca
# Sat, 18 Jan 2020 02:38:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 02:38:31 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 02:38:34 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 02:38:36 GMT
WORKDIR /data
# Sat, 18 Jan 2020 02:38:37 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:38:42 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 02:38:47 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d4a026f522563a69e1816b228fd615d5a7657cf58fe1a874fac43b90023819`  
		Last Modified: Sat, 18 Jan 2020 02:42:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c965c69e1c9e4a92575fadc54f86389f10a46d5681a5ba6f1401679f22a6288`  
		Last Modified: Sat, 18 Jan 2020 02:42:55 GMT  
		Size: 409.9 KB (409883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368c5e5dc3e646881c97abcaa37ca7e31531915fc7361e69f2cfc294bc438833`  
		Last Modified: Sat, 18 Jan 2020 02:42:56 GMT  
		Size: 7.8 MB (7808930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4ed8a2c8a9ed19030d0d7516864441e1b0271b912544394067c9e0f7f58d5f`  
		Last Modified: Sat, 18 Jan 2020 02:42:55 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f33efda694932461ab89c8b8adda34701b0bbfcf00aac08cbb969e3ffdbfce`  
		Last Modified: Sat, 18 Jan 2020 02:42:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:07f4984e0e12caa1985953b04ecc812212b2bf20721101bbc0e042575b2dfff4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10561594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb507cbdecbbf61891d73513cfc2b4a77e0d7a3bc9d220bd7edf1f1fc1d1ae2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:47:20 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 02:47:21 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 18 Jan 2020 02:47:21 GMT
ENV REDIS_VERSION=6.0-rc1
# Sat, 18 Jan 2020 02:47:21 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc1.tar.gz
# Sat, 18 Jan 2020 02:47:21 GMT
ENV REDIS_DOWNLOAD_SHA=2676012e2fcfe8d41e594b2ae8a05d0a050d2d84c38a0471ae5fe0143e4b0eca
# Sat, 18 Jan 2020 02:47:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 02:47:51 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 02:47:51 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 02:47:52 GMT
WORKDIR /data
# Sat, 18 Jan 2020 02:47:52 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:47:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:47:52 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 02:47:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87866e3e638ab9b00c8dc1f61818c0a0ce018124ee87bc5b563432dbb3ae216`  
		Last Modified: Sat, 18 Jan 2020 02:49:32 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0904f8797d435556300db89f22f858b75552653853c9f674780fa46054a1a9f`  
		Last Modified: Sat, 18 Jan 2020 02:49:32 GMT  
		Size: 407.4 KB (407362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2162063ba39bedb29a6a4728a32e591492bfb58f36462b52b9141ffa852ec1`  
		Last Modified: Sat, 18 Jan 2020 02:49:33 GMT  
		Size: 7.6 MB (7570454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c6a13c2e0402a60b5e3922d84bb641f38698012ab0a20160575de5f71673e2`  
		Last Modified: Sat, 18 Jan 2020 02:49:32 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c8471e40c5df9a94226eeb284e206df401e16eb3edb118e8ef0317ece895b1`  
		Last Modified: Sat, 18 Jan 2020 02:49:32 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
